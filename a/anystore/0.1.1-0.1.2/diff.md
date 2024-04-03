# Comparing `tmp/anystore-0.1.1.tar.gz` & `tmp/anystore-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anystore-0.1.1.tar", max compression
+gzip compressed data, was "anystore-0.1.2.tar", max compression
```

## Comparing `anystore-0.1.1.tar` & `anystore-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    35149 2024-01-30 17:13:21.261633 anystore-0.1.1/LICENSE
--rw-r--r--   0        0        0     3908 2024-03-13 14:16:50.778774 anystore-0.1.1/README.md
--rw-r--r--   0        0        0      289 2024-03-14 08:42:42.563376 anystore-0.1.1/anystore/__init__.py
--rw-r--r--   0        0        0     2739 2024-03-13 14:16:50.778774 anystore-0.1.1/anystore/cli.py
--rw-r--r--   0        0        0      946 2024-03-13 14:16:50.778774 anystore-0.1.1/anystore/decorators.py
--rw-r--r--   0        0        0       48 2024-01-31 04:09:17.694069 anystore-0.1.1/anystore/exceptions.py
--rw-r--r--   0        0        0     2237 2024-03-13 14:16:50.778774 anystore-0.1.1/anystore/io.py
--rw-r--r--   0        0        0     1909 2024-03-13 14:16:50.778774 anystore-0.1.1/anystore/mixins.py
--rw-r--r--   0        0        0     1321 2024-03-13 14:16:50.778774 anystore-0.1.1/anystore/serialize.py
--rw-r--r--   0        0        0      539 2024-03-13 14:16:50.778774 anystore-0.1.1/anystore/settings.py
--rw-r--r--   0        0        0     1027 2024-03-13 14:16:50.778774 anystore-0.1.1/anystore/store/__init__.py
--rw-r--r--   0        0        0     2882 2024-03-13 14:16:50.782774 anystore-0.1.1/anystore/store/base.py
--rw-r--r--   0        0        0     1240 2024-03-13 14:16:50.782774 anystore-0.1.1/anystore/store/fs.py
--rw-r--r--   0        0        0     1969 2024-03-13 14:16:50.782774 anystore-0.1.1/anystore/store/redis.py
--rw-r--r--   0        0        0     4307 2024-03-13 14:16:50.782774 anystore-0.1.1/anystore/store/sql.py
--rw-r--r--   0        0        0      150 2024-03-13 14:16:50.782774 anystore-0.1.1/anystore/types.py
--rw-r--r--   0        0        0     1576 2024-03-13 14:16:50.782774 anystore-0.1.1/anystore/util.py
--rw-r--r--   0        0        0     1647 2024-03-14 08:42:42.563376 anystore-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5472 1970-01-01 00:00:00.000000 anystore-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-01-30 17:13:21.261633 anystore-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3908 2024-03-13 14:16:50.778774 anystore-0.1.2/README.md
+-rw-r--r--   0        0        0      289 2024-04-03 18:27:33.205097 anystore-0.1.2/anystore/__init__.py
+-rw-r--r--   0        0        0     2794 2024-03-18 07:58:57.406424 anystore-0.1.2/anystore/cli.py
+-rw-r--r--   0        0        0     1021 2024-04-02 13:08:44.544199 anystore-0.1.2/anystore/decorators.py
+-rw-r--r--   0        0        0       48 2024-01-31 04:09:17.694069 anystore-0.1.2/anystore/exceptions.py
+-rw-r--r--   0        0        0     2237 2024-03-13 14:16:50.778774 anystore-0.1.2/anystore/io.py
+-rw-r--r--   0        0        0     1909 2024-03-13 14:16:50.778774 anystore-0.1.2/anystore/mixins.py
+-rw-r--r--   0        0        0     1321 2024-03-13 14:16:50.778774 anystore-0.1.2/anystore/serialize.py
+-rw-r--r--   0        0        0      539 2024-03-13 14:16:50.778774 anystore-0.1.2/anystore/settings.py
+-rw-r--r--   0        0        0     1027 2024-03-13 14:16:50.778774 anystore-0.1.2/anystore/store/__init__.py
+-rw-r--r--   0        0        0     3658 2024-03-19 20:18:15.500121 anystore-0.1.2/anystore/store/base.py
+-rw-r--r--   0        0        0     1544 2024-03-19 20:18:25.476053 anystore-0.1.2/anystore/store/fs.py
+-rw-r--r--   0        0        0     1969 2024-03-13 14:16:50.782774 anystore-0.1.2/anystore/store/redis.py
+-rw-r--r--   0        0        0     4307 2024-03-19 20:56:07.690434 anystore-0.1.2/anystore/store/sql.py
+-rw-r--r--   0        0        0      150 2024-03-13 14:16:50.782774 anystore-0.1.2/anystore/types.py
+-rw-r--r--   0        0        0     1576 2024-03-13 14:16:50.782774 anystore-0.1.2/anystore/util.py
+-rw-r--r--   0        0        0     1656 2024-04-03 18:27:33.205097 anystore-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5468 1970-01-01 00:00:00.000000 anystore-0.1.2/PKG-INFO
```

### Comparing `anystore-0.1.1/LICENSE` & `anystore-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `anystore-0.1.1/README.md` & `anystore-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `anystore-0.1.1/anystore/cli.py` & `anystore-0.1.2/anystore/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,17 +78,20 @@
 
 
 @cli.command("keys")
 def cli_keys(
     prefix: Annotated[Optional[str], typer.Argument(..., help="Key prefix")] = None,
     o: Annotated[str, typer.Option("-o", help="Output uri")] = "-",
 ):
+    """
+    Iterate keys in given store
+    """
     with ErrorHandler():
         S = get_store(uri=state["uri"], use_pickle=state["pickle"])
-        keys = "\n".join(S.iterate_keys(prefix))
+        keys = "\n".join(S.iterate_keys(prefix)) + "\n"
         smart_write(o, keys.encode())
 
 
 @cli.command("io")
 def cli_io(
     i: Annotated[str, typer.Option("-i", help="Input uri")] = "-",
     o: Annotated[str, typer.Option("-o", help="Output uri")] = "-",
```

### Comparing `anystore-0.1.1/anystore/decorators.py` & `anystore-0.1.2/anystore/decorators.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,15 +11,17 @@
     store = store.model_copy()
     store.raise_on_nonexist = True
 
     def _decorator(func):
         def _inner(*args, **kwargs):
             key = key_func(*args, **kwargs)
             try:
-                return store.get(key)
+                if key is not None:
+                    return store.get(key)
+                raise DoesNotExist
             except DoesNotExist:
                 res = func(*args, **kwargs)
                 if serialize_func is not None:
                     res = serialize_func(res)
                 if key is not None:
                     store.put(key, res)
                 return res
```

### Comparing `anystore-0.1.1/anystore/io.py` & `anystore-0.1.2/anystore/io.py`

 * *Files identical despite different names*

### Comparing `anystore-0.1.1/anystore/mixins.py` & `anystore-0.1.2/anystore/mixins.py`

 * *Files identical despite different names*

### Comparing `anystore-0.1.1/anystore/serialize.py` & `anystore-0.1.2/anystore/serialize.py`

 * *Files identical despite different names*

### Comparing `anystore-0.1.1/anystore/settings.py` & `anystore-0.1.2/anystore/settings.py`

 * *Files identical despite different names*

### Comparing `anystore-0.1.1/anystore/store/__init__.py` & `anystore-0.1.2/anystore/store/__init__.py`

 * *Files identical despite different names*

### Comparing `anystore-0.1.1/anystore/store/base.py` & `anystore-0.1.2/anystore/store/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -27,14 +27,20 @@
 
     def _read(self, key: Uri, raise_on_nonexist: bool | None = True, **kwargs) -> Any:
         """
         Read key from actual backend
         """
         raise NotImplementedError
 
+    def _stream(self, key: Uri, raise_on_nonexist: bool | None = True, **kwargs) -> Any:
+        """
+        Stream key line by line from actual backend (for file-like powered backend)
+        """
+        raise NotImplementedError
+
     def _get_key_prefix(self) -> str:
         """
         Get backend specific key prefix
         """
         raise NotImplementedError
 
     def _iterate_keys(self, prefix: str | None = None) -> Generator[str, None, None]:
@@ -60,14 +66,30 @@
                 self._read(key, raise_on_nonexist, **kwargs), serialization_mode
             )
         except FileNotFoundError:  # fsspec
             if raise_on_nonexist:
                 raise DoesNotExist(f"Key does not exist: `{key}`")
             return None
 
+    def stream(
+        self,
+        key: Uri,
+        raise_on_nonexist: bool | None = None,
+        serialization_mode: Mode | None = None,
+        **kwargs,
+    ) -> Generator[Any, None, None]:
+        key = self.get_key(key)
+        try:
+            for line in self._stream(key, raise_on_nonexist, **kwargs):
+                yield from_store(line, serialization_mode)
+        except FileNotFoundError:  # fsspec
+            if raise_on_nonexist:
+                raise DoesNotExist(f"Key does not exist: `{key}`")
+            return None
+
     def put(
         self, key: Uri, value: Any, serialization_mode: Mode | None = None, **kwargs
     ):
         serialization_mode = serialization_mode or self.serialization_mode
         kwargs = self.ensure_kwargs(**kwargs)
         key = self.get_key(key)
         self._write(key, to_store(value, serialization_mode))
```

### Comparing `anystore-0.1.1/anystore/store/fs.py` & `anystore-0.1.2/anystore/store/fs.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 from typing import Generator
 
 import fsspec
 from banal import ensure_dict
 
-from anystore.io import smart_read, smart_write
+from anystore.io import smart_read, smart_stream, smart_write
 from anystore.exceptions import DoesNotExist
 from anystore.store.base import BaseStore
 from anystore.types import Uri, Value
 
 
 class Store(BaseStore):
     def _write(self, key: Uri, value: Value, **kwargs) -> None:
@@ -23,15 +23,23 @@
         try:
             return smart_read(str(key), **kwargs)
         except FileNotFoundError:
             if raise_on_nonexist:
                 raise DoesNotExist(f"Key does not exist: `{key}`")
             return None
 
-    # def _exists(self, key: Uri) -> bool:
+    def _stream(
+        self, key: Uri, raise_on_nonexist: bool | None = True, **kwargs
+    ) -> Generator[Value, None, None]:
+        try:
+            yield from smart_stream(str(key), **kwargs)
+        except FileNotFoundError:
+            if raise_on_nonexist:
+                raise DoesNotExist(f"Key does not exist: `{key}`")
+
     def _get_key_prefix(self) -> str:
         return str(self.uri).rstrip("/")
 
     def _iterate_keys(self, prefix: str | None = None) -> Generator[str, None, None]:
         path = self.get_key(prefix or "")
         mapper = fsspec.get_mapper(path, **ensure_dict(self.backend_config))
         for key in mapper.keys():
```

### Comparing `anystore-0.1.1/anystore/store/redis.py` & `anystore-0.1.2/anystore/store/redis.py`

 * *Files identical despite different names*

### Comparing `anystore-0.1.1/anystore/store/sql.py` & `anystore-0.1.2/anystore/store/sql.py`

 * *Files identical despite different names*

### Comparing `anystore-0.1.1/anystore/util.py` & `anystore-0.1.2/anystore/util.py`

 * *Files identical despite different names*

### Comparing `anystore-0.1.1/pyproject.toml` & `anystore-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anystore"
-version = "0.1.1"
+version = "0.1.2"
 description = "Store and cache things anywhere"
 authors = ["Simon Wörpel <simon.woerpel@pm.me>"]
 license = "GPL-3.0"
 readme = "README.md"
 homepage = "https://github.com/investigativedata/anystore"
 repository = "https://github.com/investigativedata/anystore"
 documentation = "https://github.com/investigativedata/anystore"
@@ -31,25 +31,25 @@
 fsspec = ">2023.10,<2025"
 s3fs = ">2023.10,<2025"
 gcsfs = ">2023.10,<2025"
 adlfs = ">2023.10,<2025"
 sqlalchemy = "^2.0.28"
 redis = "^5.0.2"
 fakeredis = "^2.21.1"
-typer = "^0.9.0"
+typer = ">=0.9,<0.13"
 pyaml = "^23.12.0"
 cloudpickle = "^3.0.0"
 pydantic-settings = "^2.2.1"
 rich = "^13.7.0"
 pytest = "^8.0.2"
 cryptography = ">=42.0.4"
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.4.3,<9.0.0"
-pytest-cov = "^4.1.0"
+pytest-cov = ">=4.1,<6.0"
 pytest-env = "^1.1.1"
 black = ">=23.11,<25.0"
 isort = "^5.12.0"
 mypy = "^1.7.0"
 pre-commit = "^3.5.0"
 flake8 = ">=6.1,<8.0"
 ipdb = "^0.13.13"
```

### Comparing `anystore-0.1.1/PKG-INFO` & `anystore-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anystore
-Version: 0.1.1
+Version: 0.1.2
 Summary: Store and cache things anywhere
 Home-page: https://github.com/investigativedata/anystore
 License: GPL-3.0
 Author: Simon Wörpel
 Author-email: simon.woerpel@pm.me
 Requires-Python: >=3.11,<4
 Classifier: Intended Audience :: Developers
@@ -26,15 +26,15 @@
 Requires-Dist: pydantic (>=2.6.3,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
 Requires-Dist: pytest (>=8.0.2,<9.0.0)
 Requires-Dist: redis (>=5.0.2,<6.0.0)
 Requires-Dist: rich (>=13.7.0,<14.0.0)
 Requires-Dist: s3fs (>2023.10,<2025)
 Requires-Dist: sqlalchemy (>=2.0.28,<3.0.0)
-Requires-Dist: typer (>=0.9.0,<0.10.0)
+Requires-Dist: typer (>=0.9,<0.13)
 Project-URL: Bug Tracker, https://github.com/investigativedata/anystore/issues
 Project-URL: Documentation, https://github.com/investigativedata/anystore
 Project-URL: Repository, https://github.com/investigativedata/anystore
 Description-Content-Type: text/markdown
 
 [![anystore on pypi](https://img.shields.io/pypi/v/anystore)](https://pypi.org/project/anystore/)
 [![Python test and package](https://github.com/investigativedata/anystore/actions/workflows/python.yml/badge.svg)](https://github.com/investigativedata/anystore/actions/workflows/python.yml)
```

