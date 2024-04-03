# Comparing `tmp/labtech-0.4.3.tar.gz` & `tmp/labtech-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labtech-0.4.3.tar", max compression
+gzip compressed data, was "labtech-0.5.0.tar", max compression
```

## Comparing `labtech-0.4.3.tar` & `labtech-0.5.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0    35149 2023-09-13 02:58:38.522441 labtech-0.4.3/LICENSE
--rw-r--r--   0        0        0     5293 2024-03-31 09:09:20.297767 labtech-0.4.3/README.md
--rw-r--r--   0        0        0      706 2024-03-31 09:11:17.093709 labtech-0.4.3/labtech/__init__.py
--rw-r--r--   0        0        0     6537 2024-03-29 09:37:59.071385 labtech-0.4.3/labtech/cache.py
--rw-r--r--   0        0        0      741 2023-09-13 02:58:38.538441 labtech-0.4.3/labtech/exceptions.py
--rw-r--r--   0        0        0     1388 2024-02-06 08:56:58.895422 labtech-0.4.3/labtech/executors.py
--rw-r--r--   0        0        0    23199 2024-03-31 09:09:20.297767 labtech-0.4.3/labtech/lab.py
--rw-r--r--   0        0        0     3597 2024-03-29 09:37:59.071385 labtech-0.4.3/labtech/mypy_plugin.py
--rw-r--r--   0        0        0        0 2024-02-13 05:01:34.041748 labtech-0.4.3/labtech/py.typed
--rw-r--r--   0        0        0     4630 2024-02-06 01:46:44.484931 labtech-0.4.3/labtech/serialization.py
--rw-r--r--   0        0        0     2455 2024-03-31 09:09:14.445769 labtech-0.4.3/labtech/storage.py
--rw-r--r--   0        0        0     8603 2024-03-31 09:09:20.297767 labtech-0.4.3/labtech/tasks.py
--rw-r--r--   0        0        0     4824 2024-03-29 09:37:59.075384 labtech-0.4.3/labtech/types.py
--rw-r--r--   0        0        0     3090 2024-02-06 01:43:13.057829 labtech-0.4.3/labtech/utils.py
--rw-r--r--   0        0        0     1138 2024-03-31 09:10:58.441718 labtech-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     6348 1970-01-01 00:00:00.000000 labtech-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-09-13 02:58:38.522441 labtech-0.5.0/LICENSE
+-rw-r--r--   0        0        0     5998 2024-04-03 07:44:55.423715 labtech-0.5.0/README.md
+-rw-r--r--   0        0        0      706 2024-04-03 08:02:18.143240 labtech-0.5.0/labtech/__init__.py
+-rw-r--r--   0        0        0     6688 2024-04-03 08:01:09.692172 labtech-0.5.0/labtech/cache.py
+-rw-r--r--   0        0        0     6554 2024-04-03 08:25:41.385705 labtech-0.5.0/labtech/diagram.py
+-rw-r--r--   0        0        0      741 2023-09-13 02:58:38.538441 labtech-0.5.0/labtech/exceptions.py
+-rw-r--r--   0        0        0     1396 2024-04-03 08:25:57.589634 labtech-0.5.0/labtech/executors.py
+-rw-r--r--   0        0        0    22346 2024-04-03 08:01:09.692172 labtech-0.5.0/labtech/lab.py
+-rw-r--r--   0        0        0     4059 2024-04-03 08:27:41.813199 labtech-0.5.0/labtech/mypy_plugin.py
+-rw-r--r--   0        0        0        0 2024-02-13 05:01:34.041748 labtech-0.5.0/labtech/py.typed
+-rw-r--r--   0        0        0     4630 2024-02-06 01:46:44.484931 labtech-0.5.0/labtech/serialization.py
+-rw-r--r--   0        0        0     2455 2024-03-31 09:09:14.445769 labtech-0.5.0/labtech/storage.py
+-rw-r--r--   0        0        0     9763 2024-04-03 08:01:09.696173 labtech-0.5.0/labtech/tasks.py
+-rw-r--r--   0        0        0     5230 2024-04-03 08:41:02.359333 labtech-0.5.0/labtech/types.py
+-rw-r--r--   0        0        0     3090 2024-02-06 01:43:13.057829 labtech-0.5.0/labtech/utils.py
+-rw-r--r--   0        0        0     1025 2024-04-03 08:18:31.776056 labtech-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     6949 1970-01-01 00:00:00.000000 labtech-0.5.0/PKG-INFO
```

### Comparing `labtech-0.4.3/LICENSE` & `labtech-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `labtech-0.4.3/README.md` & `labtech-0.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -139,20 +139,54 @@
     results = lab.run_tasks(dependent_tasks)
     print([results[task] for task in dependent_tasks])
 
 if __name__ == '__main__':
     main()
 ```
 
+Labtech can even generate a [Mermaid diagram](https://mermaid.js.org/syntax/classDiagram.html)
+to visualise your tasks:
+
+```python
+from labtech.diagram import display_task_diagram
+
+some_slow_task = SlowTask(base=42)
+dependent_tasks = [
+    DependentTask(
+        slow_task=some_slow_task,
+        multiplier=multiplier,
+    )
+    for multiplier in range(10)
+]
+
+display_task_diagram(dependent_tasks)
+```
+
+```mermaid
+classDiagram
+    direction BT
+
+    class DependentTask
+    DependentTask : SlowTask slow_task
+    DependentTask : int multiplier
+
+    class SlowTask
+    SlowTask : int base
+
+
+    DependentTask <-- SlowTask: slow_task
+```
+
 To learn more, dive into the following resources:
 
 * [The labtech tutorial](https://ben-denham.github.io/labtech/tutorial) ([as an interactive notebook](https://mybinder.org/v2/gh/ben-denham/labtech/main?filepath=examples/tutorial.ipynb))
 * [Cookbook of common patterns](https://ben-denham.github.io/labtech/cookbook) ([as an interactive notebook](https://mybinder.org/v2/gh/ben-denham/labtech/main?filepath=examples/cookbook.ipynb))
 * [API reference for Labs and Tasks](https://ben-denham.github.io/labtech/core)
 * [More options for cache formats and storage providers](https://ben-denham.github.io/labtech/caching)
+* [Diagramming tools](https://ben-denham.github.io/labtech/diagram)
 * [More examples](https://github.com/ben-denham/labtech/tree/main/examples)
 
 
 ## Mypy Plugin
 
 For [mypy](https://mypy-lang.org/) type-checking of classes decorated
 with `labtech.task`, simply enable the labtech mypy plugin in your
```

### Comparing `labtech-0.4.3/labtech/__init__.py` & `labtech-0.5.0/labtech/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 results = lab.run_tasks(experiments)
 print(results)
 
 ```
 
 """
 
-__version__ = '0.4.3'
+__version__ = '0.5.0'
 
 from .types import is_task, is_task_type
 from .tasks import task
 from .lab import Lab
 from .utils import logger
 
 __all__ = [
```

### Comparing `labtech-0.4.3/labtech/cache.py` & `labtech-0.5.0/labtech/cache.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,35 +5,35 @@
 from datetime import datetime, timedelta
 import hashlib
 import json
 import pickle
 from typing import Any, Optional, Type
 
 from . import __version__ as labtech_version
-from .types import Task, TaskResult, ResultMeta, Cache, Storage
+from .types import Task, TaskT, ResultT, ResultMeta, TaskResult, Cache, Storage
 from .exceptions import CacheError, TaskNotFound
 from .serialization import Serializer
 
 
 class NullCache(Cache):
     """Cache that never stores results in the storage provider."""
 
     def cache_key(self, task: Task) -> str:
         return 'null'
 
     def is_cached(self, storage: Storage, task: Task) -> bool:
         return False
 
-    def save(self, storage: Storage, task: Task, result: Any):
+    def save(self, storage: Storage, task: Task[ResultT], result: TaskResult[ResultT]):
         pass
 
-    def load_task(self, storage: Storage, task_type: Type[Task], key: str) -> Task:
+    def load_task(self, storage: Storage, task_type: Type[TaskT], key: str) -> TaskT:
         raise TaskNotFound
 
-    def load_result_with_meta(self, storage: Storage, task: Task) -> TaskResult:
+    def load_result_with_meta(self, storage: Storage, task: Task[ResultT]) -> TaskResult[ResultT]:
         raise CacheError('Loading a result from a NullCache is not supported.')
 
     def load_cache_timestamp(self, storage: Storage, task: Task) -> Any:
         raise CacheError('Loading a cache_timestamp from a NullCache is not supported.')
 
     def delete(self, storage: Storage, task: Task):
         pass
@@ -59,15 +59,15 @@
         # our use case.
         hashed = hashlib.sha1(serialized_str).hexdigest()
         return f'{self.KEY_PREFIX}{task.__class__.__qualname__}__{hashed}'
 
     def is_cached(self, storage: Storage, task: Task) -> bool:
         return storage.exists(task.cache_key)
 
-    def save(self, storage: Storage, task: Task, task_result: TaskResult):
+    def save(self, storage: Storage, task: Task[ResultT], task_result: TaskResult[ResultT]):
         start_timestamp = None
         if task_result.meta.start is not None:
             start_timestamp = task_result.meta.start.isoformat()
 
         duration_seconds = None
         if task_result.meta.duration is not None:
             duration_seconds = task_result.meta.duration.total_seconds()
@@ -104,45 +104,45 @@
             duration = timedelta(seconds=metadata['duration_seconds'])
 
         return ResultMeta(
             start=start,
             duration=duration,
         )
 
-    def load_task(self, storage: Storage, task_type: Type[Task], key: str) -> Task:
+    def load_task(self, storage: Storage, task_type: Type[TaskT], key: str) -> TaskT:
         metadata = self.load_metadata(storage, task_type, key)
         result_meta = self.build_result_meta(metadata)
         task = self.serializer.deserialize_task(metadata['task'], result_meta=result_meta)
         if not isinstance(task, task_type):
             raise TaskNotFound
         return task
 
-    def load_result_with_meta(self, storage: Storage, task: Task) -> TaskResult:
+    def load_result_with_meta(self, storage: Storage, task: Task[ResultT]) -> TaskResult[ResultT]:
         result = self.load_result(storage, task)
         metadata = self.load_metadata(storage, type(task), task.cache_key)
         return TaskResult(
             value=result,
             meta=self.build_result_meta(metadata),
         )
 
     def delete(self, storage: Storage, task: Task):
         storage.delete(task.cache_key)
 
     @abstractmethod
-    def load_result(self, storage: Storage, task: Task) -> Any:
+    def load_result(self, storage: Storage, task: Task[ResultT]) -> ResultT:
         """Loads the result for the given task from the storage provider.
 
         Args:
             storage: Storage provider to load the result from
             task: task instance to load the result for
 
         """
 
     @abstractmethod
-    def save_result(self, storage: Storage, task: Task, result: Any):
+    def save_result(self, storage: Storage, task: Task[ResultT], result: ResultT):
         """Saves the given task result into the storage provider.
 
         Args:
             storage: Storage provider to save the result into
             task: task instance the result belongs to
             result: result to save
 
@@ -163,16 +163,16 @@
     RESULT_FILENAME = 'data.pickle'
 
     def __init__(self, *, serializer: Optional[Serializer] = None,
                  pickle_protocol: int = pickle.HIGHEST_PROTOCOL):
         super().__init__(serializer=serializer)
         self.pickle_protocol = pickle_protocol
 
-    def save_result(self, storage: Storage, task: Task, result: Any):
+    def save_result(self, storage: Storage, task: Task[ResultT], result: ResultT):
         data_file = storage.file_handle(task.cache_key, self.RESULT_FILENAME, mode='wb')
         with data_file:
             pickle.dump(result, data_file, protocol=self.pickle_protocol)
 
-    def load_result(self, storage: Storage, task: Task) -> Any:
+    def load_result(self, storage: Storage, task: Task[ResultT]) -> ResultT:
         data_file = storage.file_handle(task.cache_key, self.RESULT_FILENAME, mode='rb')
         with data_file:
             return pickle.load(data_file)
```

### Comparing `labtech-0.4.3/labtech/exceptions.py` & `labtech-0.5.0/labtech/exceptions.py`

 * *Files identical despite different names*

### Comparing `labtech-0.4.3/labtech/executors.py` & `labtech-0.5.0/labtech/executors.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             self.set_exception(ex)
         else:
             self.set_result(result)
 
 
 class SerialExecutor(Executor):
 
-    def __init__(self):
+    def __init__(self) -> None:
         self.futures: list[SerialFuture] = []
 
     def submit(self, fn: Callable, /, *args, **kwargs):
         future = SerialFuture(fn, *args, **kwargs)
         self.futures.append(future)
         return future
```

### Comparing `labtech-0.4.3/labtech/lab.py` & `labtech-0.5.0/labtech/lab.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 from typing import Any, Dict, Iterable, List, Optional, Sequence, Set, Type, Union
 
 from frozendict import frozendict
 from tqdm import tqdm
 from tqdm.notebook import tqdm as tqdm_notebook
 from tqdm.contrib.logging import logging_redirect_tqdm
 
-from .types import Task, TaskResult, ResultMeta, ResultsMap, Storage, is_task
+from .types import Task, TaskT, ResultT, ResultMeta, ResultsMap, TaskResult, Storage, is_task
+from .tasks import find_tasks_in_param
 from .exceptions import LabError, TaskNotFound
 from .utils import OrderedSet, LoggerFileProxy, logger
 from .storage import NullStorage, LocalStorage
 from .executors import SerialExecutor, wait_for_first_future
 
 _IN_TASK_SUBPROCESS = False
 
@@ -92,53 +93,27 @@
         # ensure all are updated. Duplicated task instances may occur
         # in dependencies of different tasks.
         self.task_to_instances: Dict[Task, List[Task]] = defaultdict(list)
 
         self.process_tasks(tasks)
         self.check_cyclic_dependences()
 
-    def find_tasks(self, value, searched_coll_ids: Optional[Set[int]] = None) -> Sequence[Task]:
-        if searched_coll_ids is None:
-            searched_coll_ids = set()
-        if id(value) in searched_coll_ids:
-            return []
-
-        if is_task(value):
-            return [value]
-        elif isinstance(value, list) or isinstance(value, tuple):
-            searched_coll_ids = searched_coll_ids | {id(value)}
-            return [
-                task
-                for item in value
-                for task in self.find_tasks(item, searched_coll_ids)
-            ]
-        elif isinstance(value, dict):
-            searched_coll_ids = searched_coll_ids | {id(value)}
-            return [
-                task
-                # We only need to search the values, as all parameter
-                # dictionary keys must be strings.
-                for item in value.values()
-                for task in self.find_tasks(item, searched_coll_ids)
-            ]
-        return []
-
     def process_tasks(self, tasks: Iterable[Task]):
         all_dependencies: List[Task] = []
         for task in tasks:
             if id(task) in self.processed_task_ids:
                 continue
             self.processed_task_ids.add(id(task))
 
             dependent_tasks: List[Task] = []
             if not self.runner.use_cache(task):
                 # Find all dependent tasks inside task fields
                 for field in fields(task):
                     field_value = getattr(task, field.name)
-                    dependent_tasks += self.find_tasks(field_value)
+                    dependent_tasks += find_tasks_in_param(field_value)
 
             # We insert all of the top-level tasks before processing
             # discovered dependencies, so that we will attempt to run
             # higher-level tasks as soon as possible.
             self.insert_task(task, dependent_tasks)
             all_dependencies += dependent_tasks
         if len(all_dependencies) > 0:
@@ -418,17 +393,18 @@
                  continue_on_failure: bool = True,
                  max_workers: Optional[int] = None,
                  notebook: bool = False,
                  context: Optional[dict[str, Any]] = None):
         """
         Args:
             storage: Where task results should be cached to. A string or
-                [`Path`][pathlib.Path] will be interpreted as the path to a
-                local directory, `None` will result in no caching. Any
-                [Storage][labtech.types.Storage] instance may also be specified.
+                [`Path`](https://docs.python.org/3/library/pathlib.html#pathlib.Path)
+                will be interpreted as the path to a local directory, `None`
+                will result in no caching. Any [Storage][labtech.types.Storage]
+                instance may also be specified.
             continue_on_failure: If `True`, exceptions raised by tasks will be
                 logged, but execution of other tasks will continue.
             max_workers: The maximum number of parallel worker processes for
                 running tasks. Uses the same default as
                 `concurrent.futures.ProcessPoolExecutor`: the number of
                 processors on the machine. When `max_workers=1`, all tasks will
                 be run in the main process, without multi-processing.
@@ -447,18 +423,18 @@
         self.continue_on_failure = continue_on_failure
         self.max_workers = max_workers
         self.notebook = notebook
         if context is None:
             context = {}
         self.context = context
 
-    def run_tasks(self, tasks: Sequence[Task], *,
+    def run_tasks(self, tasks: Sequence[TaskT], *,
                   bust_cache: bool = False,
                   keep_nested_results: bool = False,
-                  disable_progress: bool = False) -> Dict[Task, Any]:
+                  disable_progress: bool = False) -> Dict[TaskT, Any]:
         """Run the given tasks with as much process parallelism as possible.
         Loads task results from the cache storage where possible and
         caches results of executed tasks.
 
         Any attribute of a task that is itself a task object is
         considered a "nested task", and will be executed or loaded so
         that it's result is made available to its parent task. If the
@@ -489,29 +465,29 @@
                             bust_cache=bust_cache,
                             keep_nested_results=keep_nested_results,
                             disable_progress=disable_progress)
         results = runner.run(tasks)
         # Return results in the same order as tasks
         return {task: results[task] for task in tasks}
 
-    def run_task(self, task: Task, **kwargs) -> Any:
+    def run_task(self, task: Task[ResultT], **kwargs) -> ResultT:
         """Run a single task and return its result. Supports the same keyword
         arguments as `run_tasks`.
 
         NOTE: If you have many tasks to run, you should use
         `run_tasks` instead to parallelise their execution.
 
         Returns:
             The result of the given task.
 
         """
         results = self.run_tasks([task], **kwargs)
         return results[task]
 
-    def cached_tasks(self, task_types: Sequence[Type[Task]]) -> Sequence[Task]:
+    def cached_tasks(self, task_types: Sequence[Type[TaskT]]) -> Sequence[TaskT]:
         """Returns all task instances present in the Lab's cache storage for
         the given `task_types`, each of which should be a task class
         decorated with [`labtech.task`][labtech.task].
 
         Does not load task results from the cache storage, but they
         can be loaded by calling
         [`run_tasks()`][labtech.Lab.run_tasks] with the returned task
```

### Comparing `labtech-0.4.3/labtech/mypy_plugin.py` & `labtech-0.5.0/labtech/mypy_plugin.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,40 @@
 """Mypy plugin for classes decorated with `labtech.task`."""
 
 from typing import Type
 import mypy.plugins.dataclasses
+from mypy.nodes import COVARIANT
 from mypy.plugin import Plugin, ClassDefContext
 from mypy.plugins.common import add_attribute_to_class
-from mypy.types import Instance, LiteralType, AnyType, TypeOfAny, CallableType, NoneType, UnionType
+from mypy.types import Instance, LiteralType, AnyType, TypeOfAny, TypeVarType, CallableType, NoneType, UnionType
 from mypy.nodes import ArgKind
 
 task_makers = {'labtech.tasks.task'}
 """Set of decorator functions that return "task" classes."""
 
 
 def task_tag_callback(ctx: ClassDefContext):
     """Add attributes to a "task" class."""
-
+    covariant_result_t_type = TypeVarType(
+        name='CovariantResultT',
+        fullname=ctx.cls.info.fullname + '.CovariantResultT',
+        # TODO: Unsure if id of -1 is valid.
+        id=-1,
+        values=[],
+        upper_bound=ctx.api.named_type('builtins.object'),
+        variance=COVARIANT,
+        default=AnyType(TypeOfAny.from_omitted_generics),
+    )
     results_map_type = Instance(
         typ=ctx.api.named_type('builtins.dict').type,
         args=[
-            ctx.api.named_type('labtech.types.Task'),
-            AnyType(TypeOfAny.explicit),
+            ctx.api.named_type('labtech.types.Task', [
+                covariant_result_t_type
+            ]),
+            covariant_result_t_type,
         ],
     )
     context_type = Instance(
         typ=ctx.api.named_type('builtins.dict').type,
         args=[
             ctx.api.named_type('builtins.str'),
             AnyType(TypeOfAny.explicit),
@@ -65,15 +77,15 @@
         name='cache_key',
         typ=ctx.api.named_type('builtins.str'),
     )
     add_attribute_to_class(
         api=ctx.api,
         cls=ctx.cls,
         name='result',
-        typ=AnyType(TypeOfAny.explicit),
+        typ=covariant_result_t_type,
     )
     add_attribute_to_class(
         api=ctx.api,
         cls=ctx.cls,
         name='set_context',
         typ=CallableType(
             arg_types=[context_type],
```

### Comparing `labtech-0.4.3/labtech/serialization.py` & `labtech-0.5.0/labtech/serialization.py`

 * *Files identical despite different names*

### Comparing `labtech-0.4.3/labtech/storage.py` & `labtech-0.5.0/labtech/storage.py`

 * *Files identical despite different names*

### Comparing `labtech-0.4.3/labtech/tasks.py` & `labtech-0.5.0/labtech/tasks.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Utilities for defining tasks."""
 
 from dataclasses import dataclass, fields
 from enum import Enum
 from inspect import isclass
-from typing import cast, Any, Dict, Optional, Union
+from typing import cast, Any, Dict, Optional, Sequence, Set, Union
 
 from frozendict import frozendict
 
-from .types import TaskInfo, ResultMeta, ResultsMap, Cache, is_task_type, is_task
+from .types import Task, ResultT, TaskInfo, ResultMeta, ResultsMap, Cache, is_task_type, is_task
 from .cache import PickleCache, NullCache
 from .exceptions import TaskError
 from .utils import ensure_dict_key_str
 
 
 class CacheDefault:
     pass
@@ -38,51 +38,51 @@
         or isinstance(value, Enum)
     )
     if is_scalar or is_task(value):
         return value
     raise TaskError(f"Unsupported type '{type(value).__qualname__}' in parameter value '{key}'.")
 
 
-def _task_post_init(self):
+def _task_post_init(self: Task):
     # Ensure parameter values are immutable.
     for f in fields(self):
         object.__setattr__(self, f.name, immutable_param_value(f.name, getattr(self, f.name)))
 
     object.__setattr__(self, '_is_task', True)
     object.__setattr__(self, 'cache_key', self._lt.cache.cache_key(self))
     object.__setattr__(self, '_results_map', None)
     object.__setattr__(self, 'context', None)
     object.__setattr__(self, 'result_meta', None)
     if self._lt.orig_post_init is not None:
         self._lt.orig_post_init(self)
 
 
-def _task_set_results_map(self, results_map: ResultsMap):
+def _task_set_results_map(self: Task, results_map: ResultsMap):
     object.__setattr__(self, '_results_map', results_map)
 
 
-def _task_set_result_meta(self, result_meta: ResultMeta):
+def _task_set_result_meta(self: Task, result_meta: ResultMeta):
     object.__setattr__(self, 'result_meta', result_meta)
 
 
-def _task_set_context(self, context: dict[str, Any]):
+def _task_set_context(self: Task, context: dict[str, Any]):
     object.__setattr__(self, 'context', context)
 
 
-def _task_result(self) -> Any:
+def _task_result(self: Task[ResultT]) -> ResultT:
     if hasattr(self, '_result'):
         return self._result
     if self._results_map is None:
         raise TaskError(f"Task '{self}' has no active results map")
     if self not in self._results_map:
         raise TaskError(f"Result for task '{self}' is not available in memory")
     return self._results_map[self]
 
 
-def _task__getstate__(self) -> Dict[str, Any]:
+def _task__getstate__(self: Task) -> Dict[str, Any]:
     state = {
         **{f.name: getattr(self, f.name) for f in fields(self)},
         '_lt': self._lt,
         '_is_task': self._is_task,
         'cache_key': self.cache_key,
         # We will never pickle the full _results_map
         '_results_map': None,
@@ -92,15 +92,15 @@
     elif self._results_map is not None:
         # Avoid pickling the whole _results_map, and also avoid
         # AttributeError when attempting to pickle self inside object.
         state['_result'] = self._results_map.get(self)
     return state
 
 
-def _task__setstate__(self, state: Dict[str, Any]) -> None:
+def _task__setstate__(self: Task, state: Dict[str, Any]) -> None:
     field_set = set(f.name for f in fields(self))
     for key, value in state.items():
         value = immutable_param_value(key, value) if key in field_set else value
         object.__setattr__(self, key, value)
 
 
 def task(*args,
@@ -224,7 +224,35 @@
         cls.set_context = _task_set_context
         return cls
 
     if len(args) > 0 and isclass(args[0]):
         return decorator(args[0], *args[1:])
     else:
         return decorator
+
+
+def find_tasks_in_param(param_value: Any, searched_coll_ids: Optional[Set[int]] = None) -> Sequence[Task]:
+    """Given a parameter value, return all tasks within it found through a recursive search."""
+    if searched_coll_ids is None:
+        searched_coll_ids = set()
+    if id(param_value) in searched_coll_ids:
+        return []
+
+    if is_task(param_value):
+        return [param_value]
+    elif isinstance(param_value, list) or isinstance(param_value, tuple):
+        searched_coll_ids = searched_coll_ids | {id(param_value)}
+        return [
+            task
+            for item in param_value
+            for task in find_tasks_in_param(item, searched_coll_ids)
+        ]
+    elif isinstance(param_value, dict):
+        searched_coll_ids = searched_coll_ids | {id(param_value)}
+        return [
+            task
+            # We only need to search the values, as all parameter
+            # dictionary keys must be strings.
+            for item in param_value.values()
+            for task in find_tasks_in_param(item, searched_coll_ids)
+        ]
+    return []
```

### Comparing `labtech-0.4.3/labtech/types.py` & `labtech-0.5.0/labtech/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,52 @@
 """Core types of labtech."""
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from datetime import datetime, timedelta
 from inspect import isclass
-from typing import Any, Callable, Dict, IO, Literal, Optional, Protocol, Sequence, Type
+from typing import (
+    Any, Callable, Dict, Generic, IO, Literal,
+    Optional, Protocol, Sequence, Type, TypeVar,
+)
 
 
 @dataclass(frozen=True)
 class TaskInfo:
     orig_post_init: Optional[Callable]
     cache: 'Cache'
     max_parallel: Optional[int]
     mlflow_run: bool
 
 
+CovariantResultT = TypeVar('CovariantResultT', covariant=True)
+ResultT = TypeVar('ResultT')
+"""Type variable for result returned by the `run` method of a
+[`Task`][labtech.types.Task]."""
+ResultsMap = Dict['Task[CovariantResultT]', CovariantResultT]
+
+
 @dataclass(frozen=True)
 class ResultMeta:
     """Metadata about the execution of a task. If the task is loaded from
     cache, the metadata is also loaded from the cache."""
     start: Optional[datetime]
     """The timestamp when the task's execution began."""
     duration: Optional[timedelta]
     """The time that the task took to execute."""
 
 
 @dataclass(frozen=True)
-class TaskResult:
-    value: Any
+class TaskResult(Generic[ResultT]):
+    value: ResultT
     meta: ResultMeta
 
 
-ResultsMap = Dict['Task', Any]
-
-
-class Task(Protocol):
+@dataclass
+class Task(Protocol, Generic[CovariantResultT]):
     """Interface provided by any class that is decorated by
     [`labtech.task`][labtech.task]."""
     _lt: TaskInfo
     _is_task: Literal[True]
     _results_map: Optional[ResultsMap]
     cache_key: str
     """The key that uniquely identifies the location for this task within cache storage."""
@@ -50,15 +58,15 @@
     def _set_results_map(self, results_map: ResultsMap):
         pass
 
     def _set_result_meta(self, result_meta: ResultMeta):
         pass
 
     @property
-    def result(self) -> Any:
+    def result(self) -> CovariantResultT:
         """Returns the result executed/loaded for this task. If no result is
         available in memory, accessing this property raises a `TaskError`."""
 
     def set_context(self, context: dict[str, Any]):
         """Set the context that is made available to the task while it is
         running."""
 
@@ -68,14 +76,17 @@
 
         Usually executed by [`Lab.run_tasks()`][labtech.Lab.run_tasks]
         instead of being called directly.
 
         """
 
 
+TaskT = TypeVar("TaskT", bound=Task)
+
+
 def is_task_type(cls):
     """Returns `True` if the given `cls` is a class decorated with
     [`labtech.task`][labtech.task]."""
     return isclass(cls) and hasattr(cls, '_lt')
 
 
 def is_task(obj):
@@ -122,28 +133,28 @@
 
     @abstractmethod
     def is_cached(self, storage: Storage, task: Task) -> bool:
         """Returns `True` if a result is cached for the given `task` within
         the given `storage`."""
 
     @abstractmethod
-    def save(self, storage: Storage, task: Task, result: Any) -> None:
+    def save(self, storage: Storage, task: Task[ResultT], result: TaskResult[ResultT]) -> None:
         """Save the given `result` for the given `task` into the given
         `storage`."""
 
     @abstractmethod
-    def load_task(self, storage: Storage, task_type: Type[Task], key: str) -> Task:
+    def load_task(self, storage: Storage, task_type: Type[TaskT], key: str) -> TaskT:
         """Loads the task instance of the given `task_type` for the given
         `key` from the given `storage`.
 
         The task's result is not loaded by this method.
         """
 
     @abstractmethod
-    def load_result_with_meta(self, storage: Storage, task: Task) -> TaskResult:
+    def load_result_with_meta(self, storage: Storage, task: Task[ResultT]) -> TaskResult[ResultT]:
         """Loads the result and metadata for the given task from the storage
         provider.
 
         Args:
             storage: Storage provider to load the result from
             task: task instance to load the result for
```

### Comparing `labtech-0.4.3/labtech/utils.py` & `labtech-0.5.0/labtech/utils.py`

 * *Files identical despite different names*

### Comparing `labtech-0.4.3/pyproject.toml` & `labtech-0.5.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "labtech"
-version = "0.4.3"
+version = "0.5.0"
 license = "GPL-3.0-only"
 description = "Easily run experiment permutations with multi-processing and caching."
 authors = ["Ben Denham <ben@denham.nz>"]
 readme = "README.md"
 repository = "https://github.com/ben-denham/labtech"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
@@ -12,29 +12,28 @@
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 
 
 [tool.poetry.dependencies]
-python = "^3.8"
-tqdm = "^4.64.1"
+python = ">=3.10"
+tqdm = "^4.66.2"
 frozendict = "^2.4.0"
 
 [tool.poetry.dev-dependencies]
 flake8 = "^5.0.4"
 pytest = "^7.1.3"
 pytest-cov = "^3.0.0"
 pytest-mock = "^3.10.0"
 mkdocs = "^1.5.2"
 mkdocstrings-python = "^1.5.2"
 mkdocs-material = "^9.2.4"
-# Use very recent mypy in order to support recursive types.
-mypy = { git = "https://github.com/python/mypy.git", rev = "0f17aff" }
-jupyterlab = "^3.4.6"
-IPython = "8.12.0"
-ipywidgets = "^7.0.0"
+mypy = "^1.9.0"
+jupyterlab = "^4.1.5"
+IPython = "8.23.0"
+ipywidgets = "^8.1.2"
 mlflow = "^2.10.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `labtech-0.4.3/PKG-INFO` & `labtech-0.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 Metadata-Version: 2.1
 Name: labtech
-Version: 0.4.3
+Version: 0.5.0
 Summary: Easily run experiment permutations with multi-processing and caching.
 Home-page: https://github.com/ben-denham/labtech
 License: GPL-3.0-only
 Author: Ben Denham
 Author-email: ben@denham.nz
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.10
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: frozendict (>=2.4.0,<3.0.0)
-Requires-Dist: tqdm (>=4.64.1,<5.0.0)
+Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Project-URL: Repository, https://github.com/ben-denham/labtech
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 <h1>labtech</h1>
 
@@ -164,20 +162,54 @@
     results = lab.run_tasks(dependent_tasks)
     print([results[task] for task in dependent_tasks])
 
 if __name__ == '__main__':
     main()
 ```
 
+Labtech can even generate a [Mermaid diagram](https://mermaid.js.org/syntax/classDiagram.html)
+to visualise your tasks:
+
+```python
+from labtech.diagram import display_task_diagram
+
+some_slow_task = SlowTask(base=42)
+dependent_tasks = [
+    DependentTask(
+        slow_task=some_slow_task,
+        multiplier=multiplier,
+    )
+    for multiplier in range(10)
+]
+
+display_task_diagram(dependent_tasks)
+```
+
+```mermaid
+classDiagram
+    direction BT
+
+    class DependentTask
+    DependentTask : SlowTask slow_task
+    DependentTask : int multiplier
+
+    class SlowTask
+    SlowTask : int base
+
+
+    DependentTask <-- SlowTask: slow_task
+```
+
 To learn more, dive into the following resources:
 
 * [The labtech tutorial](https://ben-denham.github.io/labtech/tutorial) ([as an interactive notebook](https://mybinder.org/v2/gh/ben-denham/labtech/main?filepath=examples/tutorial.ipynb))
 * [Cookbook of common patterns](https://ben-denham.github.io/labtech/cookbook) ([as an interactive notebook](https://mybinder.org/v2/gh/ben-denham/labtech/main?filepath=examples/cookbook.ipynb))
 * [API reference for Labs and Tasks](https://ben-denham.github.io/labtech/core)
 * [More options for cache formats and storage providers](https://ben-denham.github.io/labtech/caching)
+* [Diagramming tools](https://ben-denham.github.io/labtech/diagram)
 * [More examples](https://github.com/ben-denham/labtech/tree/main/examples)
 
 
 ## Mypy Plugin
 
 For [mypy](https://mypy-lang.org/) type-checking of classes decorated
 with `labtech.task`, simply enable the labtech mypy plugin in your
```

