# Comparing `tmp/foamlib-0.2.3.tar.gz` & `tmp/foamlib-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foamlib-0.2.3.tar", last modified: Wed Apr  3 01:51:44 2024, max compression
+gzip compressed data, was "foamlib-0.2.4.tar", last modified: Wed Apr  3 13:00:57 2024, max compression
```

## Comparing `foamlib-0.2.3.tar` & `foamlib-0.2.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:51:44.298906 foamlib-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35131 2024-04-03 01:51:39.000000 foamlib-0.2.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-04-03 01:51:44.298906 foamlib-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-03 01:51:39.000000 foamlib-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:51:44.294906 foamlib-0.2.3/foamlib/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-03 01:51:39.000000 foamlib-0.2.3/foamlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21213 2024-04-03 01:51:39.000000 foamlib-0.2.3/foamlib/_cases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:51:44.298906 foamlib-0.2.3/foamlib/_dictionaries/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-03 01:51:39.000000 foamlib-0.2.3/foamlib/_dictionaries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-03 01:51:39.000000 foamlib-0.2.3/foamlib/_dictionaries/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11582 2024-04-03 01:51:39.000000 foamlib-0.2.3/foamlib/_dictionaries/_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-04-03 01:51:39.000000 foamlib-0.2.3/foamlib/_dictionaries/_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-04-03 01:51:39.000000 foamlib-0.2.3/foamlib/_dictionaries/_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-04-03 01:51:39.000000 foamlib-0.2.3/foamlib/_subprocesses.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:51:39.000000 foamlib-0.2.3/foamlib/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:51:44.298906 foamlib-0.2.3/foamlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-04-03 01:51:44.000000 foamlib-0.2.3/foamlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-03 01:51:44.000000 foamlib-0.2.3/foamlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 01:51:44.000000 foamlib-0.2.3/foamlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-03 01:51:44.000000 foamlib-0.2.3/foamlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 01:51:44.000000 foamlib-0.2.3/foamlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-03 01:51:39.000000 foamlib-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 01:51:44.298906 foamlib-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:51:44.298906 foamlib-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-03 01:51:39.000000 foamlib-0.2.3/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-04-03 01:51:39.000000 foamlib-0.2.3/tests/test_dictionaries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-03 01:51:39.000000 foamlib-0.2.3/tests/test_flange.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-03 01:51:39.000000 foamlib-0.2.3/tests/test_flange_async.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-03 01:51:39.000000 foamlib-0.2.3/tests/test_pitz.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-03 01:51:39.000000 foamlib-0.2.3/tests/test_pitz_async.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:00:57.459715 foamlib-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35131 2024-04-03 13:00:50.000000 foamlib-0.2.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-04-03 13:00:57.459715 foamlib-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-03 13:00:50.000000 foamlib-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:00:57.455715 foamlib-0.2.4/foamlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-03 13:00:50.000000 foamlib-0.2.4/foamlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21213 2024-04-03 13:00:50.000000 foamlib-0.2.4/foamlib/_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:00:57.459715 foamlib-0.2.4/foamlib/_dictionaries/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-03 13:00:50.000000 foamlib-0.2.4/foamlib/_dictionaries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-03 13:00:50.000000 foamlib-0.2.4/foamlib/_dictionaries/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12424 2024-04-03 13:00:50.000000 foamlib-0.2.4/foamlib/_dictionaries/_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-04-03 13:00:50.000000 foamlib-0.2.4/foamlib/_dictionaries/_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-03 13:00:50.000000 foamlib-0.2.4/foamlib/_dictionaries/_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-04-03 13:00:50.000000 foamlib-0.2.4/foamlib/_subprocesses.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:00:50.000000 foamlib-0.2.4/foamlib/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:00:57.459715 foamlib-0.2.4/foamlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-04-03 13:00:57.000000 foamlib-0.2.4/foamlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-03 13:00:57.000000 foamlib-0.2.4/foamlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 13:00:57.000000 foamlib-0.2.4/foamlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-03 13:00:57.000000 foamlib-0.2.4/foamlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 13:00:57.000000 foamlib-0.2.4/foamlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-03 13:00:50.000000 foamlib-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 13:00:57.459715 foamlib-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:00:57.459715 foamlib-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-03 13:00:50.000000 foamlib-0.2.4/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-04-03 13:00:50.000000 foamlib-0.2.4/tests/test_dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-03 13:00:50.000000 foamlib-0.2.4/tests/test_flange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-03 13:00:50.000000 foamlib-0.2.4/tests/test_flange_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-03 13:00:50.000000 foamlib-0.2.4/tests/test_pitz.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-03 13:00:50.000000 foamlib-0.2.4/tests/test_pitz_async.py
```

### Comparing `foamlib-0.2.3/LICENSE.txt` & `foamlib-0.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foamlib-0.2.3/PKG-INFO` & `foamlib-0.2.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foamlib
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Python interface for interacting with OpenFOAM
 Author-email: "Gabriel S. Gerlero" <ggerlero@cimec.unl.edu.ar>
 Project-URL: Homepage, https://github.com/gerlero/foamlib
 Project-URL: Repository, https://github.com/gerlero/foamlib
 Project-URL: Documentation, https://foamlib.readthedocs.io
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
@@ -23,14 +23,15 @@
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: aioshutil<2,>=1
 Requires-Dist: pyparsing<4,>=3
+Requires-Dist: typing-extensions<5,>=4
 Provides-Extra: lint
 Requires-Dist: mypy<2,>=1; extra == "lint"
 Requires-Dist: pytest<9,>=7; extra == "lint"
 Requires-Dist: pytest-asyncio<0.24,>=0.21; extra == "lint"
 Requires-Dist: numpy<2,>=1; extra == "lint"
 Requires-Dist: black; extra == "lint"
 Requires-Dist: flake8; extra == "lint"
```

### Comparing `foamlib-0.2.3/README.md` & `foamlib-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `foamlib-0.2.3/foamlib/_cases.py` & `foamlib-0.2.4/foamlib/_cases.py`

 * *Files identical despite different names*

### Comparing `foamlib-0.2.3/foamlib/_dictionaries/_base.py` & `foamlib-0.2.4/foamlib/_dictionaries/_base.py`

 * *Files identical despite different names*

### Comparing `foamlib-0.2.3/foamlib/_dictionaries/_files.py` & `foamlib-0.2.4/foamlib/_dictionaries/_files.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,28 +7,83 @@
     Optional,
     Sequence,
     Tuple,
     Union,
     cast,
 )
 
+from typing_extensions import Self
+
 from ._base import FoamDictionaryBase
 from ._parsing import Parsed, as_dict, get_entry_locn, get_value, parse
-from ._serialization import serialize_value
+from ._serialization import serialize_entry
 
 try:
     import numpy as np
     from numpy.typing import NDArray
 except ModuleNotFoundError:
     pass
 
 
+class _FoamFileBase:
+    def __init__(self, path: Union[str, Path]) -> None:
+        self.path = Path(path).absolute()
+        if self.path.is_dir():
+            raise IsADirectoryError(self.path)
+        elif not self.path.is_file():
+            raise FileNotFoundError(self.path)
+
+        self.__contents: Optional[str] = None
+        self.__parsed: Optional[Parsed] = None
+        self.__defer_io = 0
+        self.__dirty = False
+
+    def __enter__(self) -> Self:
+        if self.__defer_io == 0:
+            self._read()
+        self.__defer_io += 1
+        return self
+
+    def __exit__(self, exc_type: Any, exc_value: Any, traceback: Any) -> None:
+        self.__defer_io -= 1
+        if self.__defer_io == 0 and self.__dirty:
+            assert self.__contents is not None
+            self._write(self.__contents)
+        assert not self.__dirty
+
+    def _read(self) -> Tuple[str, Parsed]:
+        if not self.__defer_io:
+            contents = self.path.read_text()
+            if contents != self.__contents:
+                self.__contents = contents
+                self.__parsed = None
+
+        assert self.__contents is not None
+
+        if self.__parsed is None:
+            self.__parsed = parse(self.__contents)
+
+        return self.__contents, self.__parsed
+
+    def _write(self, contents: str) -> None:
+        self.__contents = contents
+        self.__parsed = None
+        if not self.__defer_io:
+            self.path.write_text(contents)
+            self.__dirty = False
+        else:
+            self.__dirty = True
+
+
 class FoamFile(
+    _FoamFileBase,
     FoamDictionaryBase,
-    MutableMapping[str, Union["FoamFile.Value", "FoamFile.Dictionary"]],
+    MutableMapping[
+        Union[str, Tuple[str, ...]], Union["FoamFile.Value", "FoamFile.Dictionary"]
+    ],
 ):
     """
     An OpenFOAM dictionary file.
 
     Use as a mutable mapping (i.e., like a dict) to access and modify entries.
 
     Use as a context manager to make multiple changes to the file while saving all changes only once at the end.
@@ -71,17 +126,28 @@
 
         def __delitem__(self, keyword: str) -> None:
             del self._file[(*self._keywords, keyword)]
 
         def __iter__(self) -> Iterator[str]:
             return self._file._iter(tuple(self._keywords))
 
+        def __contains__(self, keyword: object) -> bool:
+            return (*self._keywords, keyword) in self._file
+
         def __len__(self) -> int:
             return len(list(iter(self)))
 
+        def update(self, *args: Any, **kwargs: Any) -> None:
+            with self._file:
+                super().update(*args, **kwargs)
+
+        def clear(self) -> None:
+            with self._file:
+                super().clear()
+
         def __repr__(self) -> str:
             return f"{type(self).__qualname__}({self._file}, {self._keywords})"
 
         def as_dict(self) -> FoamDictionaryBase._Dict:
             """
             Return a nested dict representation of the dictionary.
             """
@@ -91,62 +157,14 @@
                 assert isinstance(ret, dict)
                 v = ret[k]
                 assert isinstance(v, dict)
                 ret = v
 
             return ret
 
-    def __init__(self, path: Union[str, Path]) -> None:
-        self.path = Path(path).absolute()
-        if self.path.is_dir():
-            raise IsADirectoryError(self.path)
-        elif not self.path.is_file():
-            raise FileNotFoundError(self.path)
-
-        self._contents: Optional[str] = None
-        self._parsed: Optional[Parsed] = None
-        self._defer_io = 0
-        self._dirty = False
-
-    def __enter__(self) -> "FoamFile":
-        if self._defer_io == 0:
-            self._read()
-        self._defer_io += 1
-        return self
-
-    def __exit__(self, exc_type: Any, exc_value: Any, traceback: Any) -> None:
-        self._defer_io -= 1
-        if self._defer_io == 0 and self._dirty:
-            assert self._contents is not None
-            self._write(self._contents)
-        assert not self._dirty
-
-    def _read(self) -> Tuple[str, Parsed]:
-        if not self._defer_io:
-            contents = self.path.read_text()
-            if contents != self._contents:
-                self._contents = contents
-                self._parsed = None
-
-        assert self._contents is not None
-
-        if self._parsed is None:
-            self._parsed = parse(self._contents)
-
-        return self._contents, self._parsed
-
-    def _write(self, contents: str) -> None:
-        self._contents = contents
-        self._parsed = None
-        if not self._defer_io:
-            self.path.write_text(contents)
-            self._dirty = False
-        else:
-            self._dirty = True
-
     def __getitem__(
         self, keywords: Union[str, Tuple[str, ...]]
     ) -> Union["FoamFile.Value", "FoamFile.Dictionary"]:
         if not isinstance(keywords, tuple):
             keywords = (keywords,)
 
         _, parsed = self._read()
@@ -175,28 +193,24 @@
             with self:
                 if isinstance(value, FoamDictionaryBase):
                     value = value.as_dict()
 
                 start, end = get_entry_locn(parsed, keywords, missing_ok=True)
 
                 self._write(
-                    f"{contents[:start]} {keywords[-1]} {{\n}}\n {contents[end:]}"
+                    f"{contents[:start]}\n{serialize_entry(keywords[-1], {})}\n{contents[end:]}"
                 )
 
                 for k, v in value.items():
                     self[(*keywords, k)] = v
         else:
             start, end = get_entry_locn(parsed, keywords, missing_ok=True)
 
-            value = serialize_value(
-                value, assume_field=assume_field, assume_dimensions=assume_dimensions
-            )
-
             self._write(
-                f"{contents[:start]} {keywords[-1]} {value};\n {contents[end:]}"
+                f"{contents[:start]}\n{serialize_entry(keywords[-1], value, assume_field=assume_field, assume_dimensions=assume_dimensions)}\n{contents[end:]}"
             )
 
     def __setitem__(self, keywords: Union[str, Tuple[str, ...]], value: Any) -> None:
         self._setitem(keywords, value)
 
     def __delitem__(self, keywords: Union[str, Tuple[str, ...]]) -> None:
         if not isinstance(keywords, tuple):
@@ -216,17 +230,31 @@
         parsed = parse(contents)
 
         yield from (k[-1] for k in parsed if k[:-1] == keywords)
 
     def __iter__(self) -> Iterator[str]:
         return self._iter()
 
+    def __contains__(self, keywords: object) -> bool:
+        if not isinstance(keywords, tuple):
+            keywords = (keywords,)
+        _, parsed = self._read()
+        return keywords in parsed
+
     def __len__(self) -> int:
         return len(list(iter(self)))
 
+    def update(self, *args: Any, **kwargs: Any) -> None:
+        with self:
+            super().update(*args, **kwargs)
+
+    def clear(self) -> None:
+        with self:
+            super().clear()
+
     def __fspath__(self) -> str:
         return str(self.path)
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}({self.path})"
 
     def as_dict(self) -> FoamDictionaryBase._Dict:
```

### Comparing `foamlib-0.2.3/foamlib/_dictionaries/_parsing.py` & `foamlib-0.2.4/foamlib/_dictionaries/_parsing.py`

 * *Files identical despite different names*

### Comparing `foamlib-0.2.3/foamlib/_dictionaries/_serialization.py` & `foamlib-0.2.4/foamlib/_dictionaries/_serialization.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from contextlib import suppress
-from typing import Any, Sequence
+from typing import Any, Mapping, Sequence
 
 from ._base import FoamDictionaryBase
 
 try:
     import numpy as np
 except ModuleNotFoundError:
     numpy = False
@@ -27,15 +27,15 @@
         return "no"
     else:
         raise TypeError(f"Not a bool: {type(value)}")
 
 
 def _serialize_list(value: Any) -> str:
     if _is_sequence(value):
-        return f"({' '.join(serialize_value(v) for v in value)})"
+        return f"({' '.join(_serialize_value(v) for v in value)})"
     else:
         raise TypeError(f"Not a valid sequence: {type(value)}")
 
 
 def _serialize_field(value: Any) -> str:
     if _is_sequence(value):
         try:
@@ -69,22 +69,22 @@
     else:
         raise TypeError(f"Not a valid dimension set: {type(value)}")
 
 
 def _serialize_dimensioned(value: Any) -> str:
     if isinstance(value, FoamDictionaryBase.Dimensioned):
         if value.name is not None:
-            return f"{value.name} {_serialize_dimensions(value.dimensions)} {serialize_value(value.value)}"
+            return f"{value.name} {_serialize_dimensions(value.dimensions)} {_serialize_value(value.value)}"
         else:
-            return f"{_serialize_dimensions(value.dimensions)} {serialize_value(value.value)}"
+            return f"{_serialize_dimensions(value.dimensions)} {_serialize_value(value.value)}"
     else:
         raise TypeError(f"Not a valid dimensioned value: {type(value)}")
 
 
-def serialize_value(
+def _serialize_value(
     value: Any, *, assume_field: bool = False, assume_dimensions: bool = False
 ) -> str:
     if isinstance(value, FoamDictionaryBase.DimensionSet) or assume_dimensions:
         with suppress(TypeError):
             return _serialize_dimensions(value)
 
     if assume_field:
@@ -97,7 +97,27 @@
     with suppress(TypeError):
         return _serialize_list(value)
 
     with suppress(TypeError):
         return _serialize_bool(value)
 
     return str(value)
+
+
+def _serialize_dictionary(value: Any) -> str:
+    if isinstance(value, Mapping):
+        return "\n".join(serialize_entry(k, v) for k, v in value.items())
+    else:
+        raise TypeError(f"Not a valid dictionary: {type(value)}")
+
+
+def serialize_entry(
+    keyword: str,
+    value: Any,
+    *,
+    assume_field: bool = False,
+    assume_dimensions: bool = False,
+) -> str:
+    try:
+        return f"{keyword}\n{{\n{_serialize_dictionary(value)}\n}}"
+    except TypeError:
+        return f"{keyword} {_serialize_value(value, assume_field=assume_field, assume_dimensions=assume_dimensions)};"
```

### Comparing `foamlib-0.2.3/foamlib/_subprocesses.py` & `foamlib-0.2.4/foamlib/_subprocesses.py`

 * *Files identical despite different names*

### Comparing `foamlib-0.2.3/foamlib.egg-info/PKG-INFO` & `foamlib-0.2.4/foamlib.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foamlib
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Python interface for interacting with OpenFOAM
 Author-email: "Gabriel S. Gerlero" <ggerlero@cimec.unl.edu.ar>
 Project-URL: Homepage, https://github.com/gerlero/foamlib
 Project-URL: Repository, https://github.com/gerlero/foamlib
 Project-URL: Documentation, https://foamlib.readthedocs.io
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
@@ -23,14 +23,15 @@
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: aioshutil<2,>=1
 Requires-Dist: pyparsing<4,>=3
+Requires-Dist: typing-extensions<5,>=4
 Provides-Extra: lint
 Requires-Dist: mypy<2,>=1; extra == "lint"
 Requires-Dist: pytest<9,>=7; extra == "lint"
 Requires-Dist: pytest-asyncio<0.24,>=0.21; extra == "lint"
 Requires-Dist: numpy<2,>=1; extra == "lint"
 Requires-Dist: black; extra == "lint"
 Requires-Dist: flake8; extra == "lint"
```

### Comparing `foamlib-0.2.3/foamlib.egg-info/SOURCES.txt` & `foamlib-0.2.4/foamlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `foamlib-0.2.3/pyproject.toml` & `foamlib-0.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     "Topic :: Software Development",
     "Typing :: Typed",
 ]
 
 dependencies = [
     "aioshutil>=1,<2",
     "pyparsing>=3,<4",
+    "typing-extensions>=4,<5",
 ]
 
 dynamic = ["version"]
 
 [project.optional-dependencies]
 lint = [
     "mypy>=1,<2",
```

### Comparing `foamlib-0.2.3/tests/test_dictionaries.py` & `foamlib-0.2.4/tests/test_dictionaries.py`

 * *Files identical despite different names*

### Comparing `foamlib-0.2.3/tests/test_flange.py` & `foamlib-0.2.4/tests/test_flange.py`

 * *Files identical despite different names*

### Comparing `foamlib-0.2.3/tests/test_flange_async.py` & `foamlib-0.2.4/tests/test_flange_async.py`

 * *Files identical despite different names*

### Comparing `foamlib-0.2.3/tests/test_pitz.py` & `foamlib-0.2.4/tests/test_pitz.py`

 * *Files identical despite different names*

### Comparing `foamlib-0.2.3/tests/test_pitz_async.py` & `foamlib-0.2.4/tests/test_pitz_async.py`

 * *Files identical despite different names*

