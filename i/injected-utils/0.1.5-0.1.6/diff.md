# Comparing `tmp/injected_utils-0.1.5.tar.gz` & `tmp/injected_utils-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "injected_utils-0.1.5.tar", max compression
+gzip compressed data, was "injected_utils-0.1.6.tar", max compression
```

## Comparing `injected_utils-0.1.5.tar` & `injected_utils-0.1.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2023-07-19 05:19:08.455997 injected_utils-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-07-19 02:58:41.015807 injected_utils-0.1.5/injected_utils/__init__.py
--rw-r--r--   0        0        0        2 2023-11-13 05:36:52.583543 injected_utils-0.1.5/injected_utils/async_cached_function.py
--rw-r--r--   0        0        0    17439 2023-12-27 05:31:12.462515 injected_utils-0.1.5/injected_utils/cached_function.py
--rw-r--r--   0        0        0    18225 2024-01-25 05:52:52.621046 injected_utils-0.1.5/injected_utils/injected_cache_utils.py
--rw-r--r--   0        0        0     3598 2023-11-25 15:03:05.017979 injected_utils-0.1.5/injected_utils/picklability_checker.py
--rw-r--r--   0        0        0     3950 2023-04-18 01:16:04.722640 injected_utils-0.1.5/injected_utils/shelf_util.py
--rw-r--r--   0        0        0      529 2024-01-25 05:53:01.139563 injected_utils-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      710 1970-01-01 00:00:00.000000 injected_utils-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-19 05:19:08.455997 injected_utils-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-07-19 02:58:41.015807 injected_utils-0.1.6/injected_utils/__init__.py
+-rw-r--r--   0        0        0        2 2023-11-13 05:36:52.583543 injected_utils-0.1.6/injected_utils/async_cached_function.py
+-rw-r--r--   0        0        0    17439 2023-12-27 05:31:12.462515 injected_utils-0.1.6/injected_utils/cached_function.py
+-rw-r--r--   0        0        0    19384 2024-04-03 03:47:00.467836 injected_utils-0.1.6/injected_utils/injected_cache_utils.py
+-rw-r--r--   0        0        0     4515 2024-02-15 11:54:53.408850 injected_utils-0.1.6/injected_utils/picklability_checker.py
+-rw-r--r--   0        0        0     3950 2023-04-18 01:16:04.722640 injected_utils-0.1.6/injected_utils/shelf_util.py
+-rw-r--r--   0        0        0      551 2024-04-03 03:48:01.378698 injected_utils-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      753 1970-01-01 00:00:00.000000 injected_utils-0.1.6/PKG-INFO
```

### Comparing `injected_utils-0.1.5/injected_utils/cached_function.py` & `injected_utils-0.1.6/injected_utils/cached_function.py`

 * *Files identical despite different names*

### Comparing `injected_utils-0.1.5/injected_utils/injected_cache_utils.py` & `injected_utils-0.1.6/injected_utils/injected_cache_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 import asyncio
 import inspect
-import threading
 from asyncio import Future
 from dataclasses import dataclass, field
 from hashlib import sha256
 from pathlib import Path
+from pprint import pformat
 from typing import Callable, Dict, ParamSpec, Any
 
 import cloudpickle
 import jsonpickle
 from frozendict import frozendict
-from loguru import logger
+from pinjected.di.metadata.bind_metadata import BindMetadata
 from returns.maybe import Some
 from sqlitedict import SqliteDict
 
-# from data_tree.util import Pickled
-
 from injected_utils.cached_function import AsyncCachedFunction, CachedFunction, KeyEncoder, IStringKeyProtocol, \
     IKeyEncoder
-from pinjected import Injected, injected_function, injected
+from pinjected import Injected, injected_function, injected, instance
 from pinjected.decoration import update_if_registered
-from pinjected.di.bindings import BindMetadata
-from pinjected.di.graph import Providable
 from pinjected.di.proxiable import DelegatedVar
 from pinjected.di.util import get_code_location
+from pinjected.providable import Providable
+
+# from data_tree.util import Pickled
 
 P = ParamSpec('P')
 Hasher = Callable[[P], Any]
 HasherFactory = Callable[[inspect.Signature], Hasher]
 
 
 def ensure_injected(i: Providable):
@@ -47,65 +46,92 @@
 
 
 def pickled_injected(cache_path, injected: Injected):
     from data_tree.util import Pickled
     injected = ensure_injected(injected)
 
     def _impl(session):
-        return Pickled(cache_path, lambda: session[injected]).value
+        return Pickled(cache_path, lambda: session[injected], backend=cloudpickle).value
 
-    return Injected.bind(_impl)
+    return Injected.bind(_impl).add_dynamic_dependencies(*injected.complete_dependencies)
+
+
+@instance
+@dataclass
+class AsyncRunTracker:
+    logger: "Logger"
 
+    def __post_init__(self):
+        self.running_tasks = []
+        self.bound = self.logger.bind(name="AsyncRunTracker")
+
+    def log_status(self):
+        self.bound.info(f"running tasks: {pformat([i[1] for i in self.running_tasks])}\n num:{len(self.running_tasks)}")
+
+    def register(self, fut: Future, fn, *args, **kwargs):
+        self.bound.info(f"adding {fn} to running tasks")
+        self.log_status()
+        self.running_tasks.append((fut, fn, args, kwargs))
+
+        def done(fut):
+            self.bound.info(f"removing {fn} from running tasks")
+            self.running_tasks.remove((fut, fn, args, kwargs))
+            self.log_status()
 
-RUNNING_TASKS = []
+        fut.add_done_callback(done)
 
 
 @injected_function
-async def async_run(thread_pool, /, fn, *args, **kwargs):
+async def async_run(thread_pool, AsyncRunTracker, /, fn, *args, **kwargs):
     # Ah, there are 391 tasks submitted
     # logger.info(f"submitting to thread pool {fn} from {threading.current_thread()}")
-    assert threading.current_thread().name == "MainThread", f"current thread is {threading.current_thread()}"
+    # assert threading.current_thread().name == "MainThread", f"current thread is {threading.current_thread()}"
     fut = thread_pool.submit(fn, *args, **kwargs)
-    RUNNING_TASKS.append(fn)
     # logger.info(f"awaiting {fn} to thread pool")
-    res = await asyncio.wrap_future(fut)
-    RUNNING_TASKS.remove(fn)
+    wrapped = asyncio.wrap_future(fut)
+    AsyncRunTracker.register(wrapped, fn, args, kwargs)
+    res = await wrapped
     # logger.info(f"got result from thread pool")
     # logger.info(f"remaining tasks: {RUNNING_TASKS[:1]} num:{len(RUNNING_TASKS)} ")
 
     return res
 
 
 @injected_function
 async def run_in_new_thread(fn, *args, **kwargs):
     res = Future()
+    import threading
 
     def run_task():
+        from loguru import logger
+        # holy fuck loguru!
         try:
             logger.info(f"running {fn} in new thread :{threading.current_thread()}")
             data = fn(*args, **kwargs)
             logger.info(f"finished {fn} in new thread :{threading.current_thread()}")
             res.set_result(data)
         except Exception as e:
             res.set_exception(e)
 
     thread = threading.Thread(target=run_task)
+    from loguru import logger
     logger.info(f"starting thread {thread} for {fn}")
     thread.start()
     try:
         logger.info(f"waiting for thread {thread} for {fn}")
         await asyncio.sleep(1)  # sleeping here for 1 sec fixes the problem. but why?
         logger.info(f"waiting for thread {thread} for {fn} 2...")
         return await res
     except Exception as e:
         logger.error(f"error in run_in_new_thread: {e}")
         raise e
 
 
 def provide_cached(cache, async_run, func: Callable, additional_key: Injected):
+    from loguru import logger
     async def task(key, *args, **kwargs):
         return await async_run(func, *args, **kwargs)
 
     assert not isinstance(func, DelegatedVar), f"func is DelegatedVar: {func}"
     assert not isinstance(func, Injected)
 
     cached = AsyncCachedFunction(
@@ -188,14 +214,15 @@
     :param cache:
     :param additional_key: additional key to be used for the cache key.
     :return:
     """
     additional_key = Injected.mzip(*[ensure_injected(i) for i in additional_keys])
 
     def _impl(func: Injected[Callable]):
+        from loguru import logger
         assert isinstance(func, Injected)
         logger.info(f"en_async_cached called with: {func}")
         return Injected.bind(
             provide_cached,
             cache=cache,
             func=func,
             additional_key=additional_key
@@ -283,15 +310,15 @@
     src: SqliteDict
 
     def __reduce__(self):
         return PicklableSqliteDict.from_path, (self.src.filename,)
 
     @classmethod
     def from_path(cls, path):
-        if isinstance(path,str):
+        if isinstance(path, str):
             path = Path(path)
         assert isinstance(path, Path), f"path must be a Path object, but got {path}"
         path.parent.mkdir(parents=True, exist_ok=True)
         return cls(SqliteDict(path, autocommit=True))
 
     def __getitem__(self, item):
         return self.src[item]
@@ -332,21 +359,22 @@
 
     def __delitem__(self, instance):
         key = jsonpickle.dumps(instance)
         del self.src[key]
 
 
 @injected
-def sqlite_cache(cache_path: str):
+def sqlite_cache(cache_path: str | Path):
     # TODO wrap this to be serializable for the ray.
     return PicklableSqliteDict.from_path(cache_path)
 
 
 @injected
-def sqlite_dict(cache_path: str):
+def sqlite_dict(cache_path: str | Path):
+    Path(cache_path).parent.mkdir(parents=True, exist_ok=True)
     return JsonBackedSqliteDict.from_path(cache_path)
 
 
 @dataclass
 class CustomKeyHasher:
     signature: inspect.Signature
     key_hasher: dict[str, Callable[[Any], Any]] = field(default_factory=dict)
@@ -466,14 +494,15 @@
     """
     cache = ensure_injected(cache)
     deps = [ensure_injected(d) for d in deps]
     parent_frame = inspect.currentframe().f_back
 
     def provide_blocking_cache(cache, func, _deps, _hasher_factory):
         def new_impl(deps, *arg, **kwargs):
+            from loguru import logger
             # deps are just for cache key purposes
             logger.info(f"new_impl called with: {func.__name__, arg, kwargs}")
             res = func(*arg, **kwargs)
             logger.info(f"new_impl returned: {res}")
             return res
 
         hasher: Hasher = _hasher_factory(inspect.signature(new_impl))
```

### Comparing `injected_utils-0.1.5/injected_utils/picklability_checker.py` & `injected_utils-0.1.6/injected_utils/picklability_checker.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 from inspect import ismethod, isbuiltin
 from typing import Iterable, Any, Optional
 
 import cloudpickle
 from returns.result import safe, Failure, Result
 from tabulate import tabulate
 
+from pinjected.di.ast import Expr
 from pinjected.di.proxiable import DelegatedVar
+from pinjected.di.static_proxy import AstProxyContextImpl
 
 
 def rec_valmap(f, tgt: dict):
     res = dict()
     for k, v in tgt.items():
         if isinstance(v, dict):
             res[k] = rec_valmap(f, v)
@@ -45,14 +47,24 @@
     trace: str
     pkl: Result
     value: Any
 
     def truncated_tuple(self, n: int = 100):
         return self.trace, self.pkl, str(self.value)[:n]
 
+def is_property(obj, attribute):
+    """Check if an attribute of an object is a @property."""
+    # Check if the attribute exists in the class of the object
+    if attribute in dir(obj.__class__):
+        # Get the attribute from the class
+        attr = getattr(obj.__class__, attribute)
+        # Check if the attribute is an instance of property
+        return isinstance(attr, property)
+    return False
+
 
 def dfs_picklability(tgt, trace="root", dumps=cloudpickle.dumps) -> Iterable[PicklingFailure]:
     visited = set()
     safe_pickle = safe(dumps)
 
     def dfs(tgt, trace):
         if len(trace) >= 1000:
@@ -72,24 +84,34 @@
                 yield from dfs(tgt.value, trace + f".value")
             elif isinstance(tgt, Iterable):
                 for i, item in enumerate(tgt):
                     if id(i) not in visited:
                         visited.add(id(i))
                         yield from dfs(item, trace + f"[{i}]")
             else:
+                # I want to stop digging into @property. but how?
                 for k in dir(tgt):
-                    if not k.startswith("__") and not k == "_abc_impl":
-                        attr = getattr(tgt, k)
-                        if not ismethod(attr) and not isbuiltin(attr) and id(attr) not in visited:
-                            new_trace = trace + f".{k}"
-                            yield from dfs(attr, new_trace)
-            if hasattr(tgt, "__closure__") and tgt.__closure__ is not None:
+                    if k.startswith("__"):
+                        continue
+                    if is_property(tgt, k):
+                        continue
+                    if k=="_abc_impl":
+                        continue
+                    attr = getattr(tgt, k)
+                    if not ismethod(attr) and not isbuiltin(attr) and id(attr) not in visited:
+                        new_trace = trace + f".{k}"
+                        yield from dfs(attr, new_trace)
+            if isinstance(tgt,DelegatedVar) or isinstance(tgt, Expr) :
+                pass
+            elif hasattr(tgt, "__closure__") and tgt.__closure__ is not None:
                 for i, cell in enumerate(tgt.__closure__):
+                    from loguru import logger
                     if id(cell) not in visited:
                         visited.add(id(cell))
+                        logger.info(f"trace:{trace}, type:{type(cell)}")
                         yield from dfs(cell, trace + f".__closure__[{i}]")
 
     return dfs(tgt, trace)
 
 
 def assert_picklable(tgt, message: Optional[str] = None, trace="root", dumps=cloudpickle.dumps):
     from loguru import logger
```

### Comparing `injected_utils-0.1.5/injected_utils/shelf_util.py` & `injected_utils-0.1.6/injected_utils/shelf_util.py`

 * *Files identical despite different names*

### Comparing `injected_utils-0.1.5/pyproject.toml` & `injected_utils-0.1.6/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "injected-utils"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = ["Kento Masui <nameissoap@gmail.com>"]
 readme = "README.md"
 packages = [{include = "injected_utils"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -14,12 +14,13 @@
 #pdfminer = "^20191125"
 pymupdf = "^1.22.5"
 chardet = "^5.1.0"
 pathos = "^0.3.0"
 bibtexparser = "^1.4.0"
 rpa = "^1.50.0"
 sqlitedict = "*"
+pinjected = "^0.2.26"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `injected_utils-0.1.5/PKG-INFO` & `injected_utils-0.1.6/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: injected-utils
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: Kento Masui
 Author-email: nameissoap@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bibtexparser (>=1.4.0,<2.0.0)
 Requires-Dist: chardet (>=5.1.0,<6.0.0)
 Requires-Dist: fuzzysearch (>=0.7.3,<0.8.0)
 Requires-Dist: notion-client (>=2.0.0,<3.0.0)
 Requires-Dist: notion-database (>=1.1.0,<2.0.0)
 Requires-Dist: pathos (>=0.3.0,<0.4.0)
+Requires-Dist: pinjected (>=0.2.26,<0.3.0)
 Requires-Dist: pymupdf (>=1.22.5,<2.0.0)
 Requires-Dist: rpa (>=1.50.0,<2.0.0)
 Requires-Dist: sqlitedict
 Description-Content-Type: text/markdown
```

