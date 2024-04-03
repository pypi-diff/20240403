# Comparing `tmp/foamlib-0.2.2.tar.gz` & `tmp/foamlib-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foamlib-0.2.2.tar", last modified: Fri Mar 29 17:27:46 2024, max compression
+gzip compressed data, was "foamlib-0.2.3.tar", last modified: Wed Apr  3 01:51:44 2024, max compression
```

## Comparing `foamlib-0.2.2.tar` & `foamlib-0.2.3.tar`

### file list

```diff
@@ -1,25 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:27:46.412703 foamlib-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35131 2024-03-29 17:27:41.000000 foamlib-0.2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-03-29 17:27:46.412703 foamlib-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-03-29 17:27:41.000000 foamlib-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:27:46.408703 foamlib-0.2.2/foamlib/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-03-29 17:27:41.000000 foamlib-0.2.2/foamlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21213 2024-03-29 17:27:41.000000 foamlib-0.2.2/foamlib/_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)    14874 2024-03-29 17:27:41.000000 foamlib-0.2.2/foamlib/_dictionaries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-03-29 17:27:41.000000 foamlib-0.2.2/foamlib/_subprocesses.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 17:27:41.000000 foamlib-0.2.2/foamlib/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:27:46.408703 foamlib-0.2.2/foamlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-03-29 17:27:46.000000 foamlib-0.2.2/foamlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-03-29 17:27:46.000000 foamlib-0.2.2/foamlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 17:27:46.000000 foamlib-0.2.2/foamlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-29 17:27:46.000000 foamlib-0.2.2/foamlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-29 17:27:46.000000 foamlib-0.2.2/foamlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-03-29 17:27:41.000000 foamlib-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 17:27:46.412703 foamlib-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:27:46.408703 foamlib-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-29 17:27:41.000000 foamlib-0.2.2/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-03-29 17:27:41.000000 foamlib-0.2.2/tests/test_dictionaries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-03-29 17:27:41.000000 foamlib-0.2.2/tests/test_flange.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-03-29 17:27:41.000000 foamlib-0.2.2/tests/test_flange_async.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-03-29 17:27:41.000000 foamlib-0.2.2/tests/test_pitz.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-03-29 17:27:41.000000 foamlib-0.2.2/tests/test_pitz_async.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:51:44.298906 foamlib-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35131 2024-04-03 01:51:39.000000 foamlib-0.2.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-04-03 01:51:44.298906 foamlib-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-03 01:51:39.000000 foamlib-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:51:44.294906 foamlib-0.2.3/foamlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-03 01:51:39.000000 foamlib-0.2.3/foamlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21213 2024-04-03 01:51:39.000000 foamlib-0.2.3/foamlib/_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:51:44.298906 foamlib-0.2.3/foamlib/_dictionaries/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-03 01:51:39.000000 foamlib-0.2.3/foamlib/_dictionaries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-03 01:51:39.000000 foamlib-0.2.3/foamlib/_dictionaries/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11582 2024-04-03 01:51:39.000000 foamlib-0.2.3/foamlib/_dictionaries/_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-04-03 01:51:39.000000 foamlib-0.2.3/foamlib/_dictionaries/_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-04-03 01:51:39.000000 foamlib-0.2.3/foamlib/_dictionaries/_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-04-03 01:51:39.000000 foamlib-0.2.3/foamlib/_subprocesses.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:51:39.000000 foamlib-0.2.3/foamlib/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:51:44.298906 foamlib-0.2.3/foamlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-04-03 01:51:44.000000 foamlib-0.2.3/foamlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-03 01:51:44.000000 foamlib-0.2.3/foamlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 01:51:44.000000 foamlib-0.2.3/foamlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-03 01:51:44.000000 foamlib-0.2.3/foamlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 01:51:44.000000 foamlib-0.2.3/foamlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-03 01:51:39.000000 foamlib-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 01:51:44.298906 foamlib-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:51:44.298906 foamlib-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-03 01:51:39.000000 foamlib-0.2.3/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-04-03 01:51:39.000000 foamlib-0.2.3/tests/test_dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-03 01:51:39.000000 foamlib-0.2.3/tests/test_flange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-03 01:51:39.000000 foamlib-0.2.3/tests/test_flange_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-03 01:51:39.000000 foamlib-0.2.3/tests/test_pitz.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-03 01:51:39.000000 foamlib-0.2.3/tests/test_pitz_async.py
```

### Comparing `foamlib-0.2.2/LICENSE.txt` & `foamlib-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foamlib-0.2.2/PKG-INFO` & `foamlib-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foamlib
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python interface for interacting with OpenFOAM
 Author-email: "Gabriel S. Gerlero" <ggerlero@cimec.unl.edu.ar>
 Project-URL: Homepage, https://github.com/gerlero/foamlib
 Project-URL: Repository, https://github.com/gerlero/foamlib
 Project-URL: Documentation, https://foamlib.readthedocs.io
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
```

### Comparing `foamlib-0.2.2/README.md` & `foamlib-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `foamlib-0.2.2/foamlib/_cases.py` & `foamlib-0.2.3/foamlib/_cases.py`

 * *Files identical despite different names*

### Comparing `foamlib-0.2.2/foamlib/_subprocesses.py` & `foamlib-0.2.3/foamlib/_subprocesses.py`

 * *Files identical despite different names*

### Comparing `foamlib-0.2.2/foamlib.egg-info/PKG-INFO` & `foamlib-0.2.3/foamlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foamlib
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python interface for interacting with OpenFOAM
 Author-email: "Gabriel S. Gerlero" <ggerlero@cimec.unl.edu.ar>
 Project-URL: Homepage, https://github.com/gerlero/foamlib
 Project-URL: Repository, https://github.com/gerlero/foamlib
 Project-URL: Documentation, https://foamlib.readthedocs.io
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
```

### Comparing `foamlib-0.2.2/pyproject.toml` & `foamlib-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `foamlib-0.2.2/tests/test_dictionaries.py` & `foamlib-0.2.3/tests/test_dictionaries.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,71 +3,65 @@
 import os
 from pathlib import Path
 from typing import Sequence
 
 import numpy as np
 
 from foamlib import *
-from foamlib._dictionaries import _VALUE
+from foamlib._dictionaries._parsing import _VALUE
 
 
 def test_parse_value() -> None:
-    assert _VALUE.parse_string("1").as_list()[0] == 1
-    assert _VALUE.parse_string("1.0").as_list()[0] == 1.0
-    assert _VALUE.parse_string("1.0e-3").as_list()[0] == 1.0e-3
-    assert _VALUE.parse_string("yes").as_list()[0] is True
-    assert _VALUE.parse_string("no").as_list()[0] is False
-    assert _VALUE.parse_string("word").as_list()[0] == "word"
-    assert _VALUE.parse_string("word word").as_list()[0] == "word word"
-    assert _VALUE.parse_string('"a string"').as_list()[0] == '"a string"'
-    assert _VALUE.parse_string("uniform 1").as_list()[0] == 1
-    assert _VALUE.parse_string("uniform 1.0").as_list()[0] == 1.0
-    assert _VALUE.parse_string("uniform 1.0e-3").as_list()[0] == 1.0e-3
-    assert _VALUE.parse_string("(1.0 2.0 3.0)").as_list()[0] == [1.0, 2.0, 3.0]
-    assert _VALUE.parse_string("uniform (1 2 3)").as_list()[0] == [1, 2, 3]
-    assert _VALUE.parse_string("nonuniform List<scalar> 2(1 2)").as_list()[0] == [1, 2]
-    assert _VALUE.parse_string("nonuniform List<scalar> 2{1}").as_list()[0] == [1, 1]
-    assert _VALUE.parse_string("3(1 2 3)").as_list()[0] == [1, 2, 3]
-    assert _VALUE.parse_string("2((1 2 3) (4 5 6))").as_list()[0] == [
+    assert _VALUE.parse_string("1")[0] == 1
+    assert _VALUE.parse_string("1.0")[0] == 1.0
+    assert _VALUE.parse_string("1.0e-3")[0] == 1.0e-3
+    assert _VALUE.parse_string("yes")[0] is True
+    assert _VALUE.parse_string("no")[0] is False
+    assert _VALUE.parse_string("word")[0] == "word"
+    assert _VALUE.parse_string("word word")[0] == "word word"
+    assert _VALUE.parse_string('"a string"')[0] == '"a string"'
+    assert _VALUE.parse_string("uniform 1")[0] == 1
+    assert _VALUE.parse_string("uniform 1.0")[0] == 1.0
+    assert _VALUE.parse_string("uniform 1.0e-3")[0] == 1.0e-3
+    assert _VALUE.parse_string("(1.0 2.0 3.0)")[0] == [1.0, 2.0, 3.0]
+    assert _VALUE.parse_string("uniform (1 2 3)")[0] == [1, 2, 3]
+    assert _VALUE.parse_string("nonuniform List<scalar> 2(1 2)")[0] == [1, 2]
+    assert _VALUE.parse_string("nonuniform List<scalar> 2{1}")[0] == [1, 1]
+    assert _VALUE.parse_string("3(1 2 3)")[0] == [1, 2, 3]
+    assert _VALUE.parse_string("2((1 2 3) (4 5 6))")[0] == [
         [1, 2, 3],
         [4, 5, 6],
     ]
-    assert _VALUE.parse_string("2{(1 2 3)}").as_list()[0] == [
+    assert _VALUE.parse_string("2{(1 2 3)}")[0] == [
         [1, 2, 3],
         [1, 2, 3],
     ]
-    assert _VALUE.parse_string("nonuniform List<vector> 2((1 2 3) (4 5 6))").as_list()[
-        0
-    ] == [
+    assert _VALUE.parse_string("nonuniform List<vector> 2((1 2 3) (4 5 6))")[0] == [
         [1, 2, 3],
         [4, 5, 6],
     ]
-    assert _VALUE.parse_string("nonuniform List<vector> 2{(1 2 3)}").as_list()[0] == [
+    assert _VALUE.parse_string("nonuniform List<vector> 2{(1 2 3)}")[0] == [
         [1, 2, 3],
         [1, 2, 3],
     ]
-    assert _VALUE.parse_string("[1 1 -2 0 0 0 0]").as_list()[
-        0
-    ] == FoamFile.DimensionSet(mass=1, length=1, time=-2)
-    assert _VALUE.parse_string("g [1 1 -2 0 0 0 0] (0 0 -9.81)").as_list()[
+    assert _VALUE.parse_string("[1 1 -2 0 0 0 0]")[0] == FoamFile.DimensionSet(
+        mass=1, length=1, time=-2
+    )
+    assert _VALUE.parse_string("g [1 1 -2 0 0 0 0] (0 0 -9.81)")[
         0
     ] == FoamFile.Dimensioned(
         name="g",
         dimensions=FoamFile.DimensionSet(mass=1, length=1, time=-2),
         value=[0, 0, -9.81],
     )
-    assert _VALUE.parse_string("[1 1 -2 0 0 0 0] 9.81").as_list()[
-        0
-    ] == FoamFile.Dimensioned(
+    assert _VALUE.parse_string("[1 1 -2 0 0 0 0] 9.81")[0] == FoamFile.Dimensioned(
         dimensions=FoamFile.DimensionSet(mass=1, length=1, time=-2), value=9.81
     )
     assert (
-        _VALUE.parse_string(
-            "hex (0 1 2 3 4 5 6 7) (1 1 1) simpleGrading (1 1 1)"
-        ).as_list()[0]
+        _VALUE.parse_string("hex (0 1 2 3 4 5 6 7) (1 1 1) simpleGrading (1 1 1)")[0]
         == "hex (0 1 2 3 4 5 6 7) (1 1 1) simpleGrading (1 1 1)"
     )
 
 
 def test_write_read(tmp_path: Path) -> None:
     path = tmp_path / "testDict"
     path.touch()
```

### Comparing `foamlib-0.2.2/tests/test_flange.py` & `foamlib-0.2.3/tests/test_flange.py`

 * *Files identical despite different names*

### Comparing `foamlib-0.2.2/tests/test_flange_async.py` & `foamlib-0.2.3/tests/test_flange_async.py`

 * *Files identical despite different names*

### Comparing `foamlib-0.2.2/tests/test_pitz.py` & `foamlib-0.2.3/tests/test_pitz.py`

 * *Files identical despite different names*

### Comparing `foamlib-0.2.2/tests/test_pitz_async.py` & `foamlib-0.2.3/tests/test_pitz_async.py`

 * *Files identical despite different names*

