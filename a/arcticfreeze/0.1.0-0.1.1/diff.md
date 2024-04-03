# Comparing `tmp/arcticfreeze-0.1.0.tar.gz` & `tmp/arcticfreeze-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcticfreeze-0.1.0.tar", last modified: Tue Apr  2 08:44:06 2024, max compression
+gzip compressed data, was "arcticfreeze-0.1.1.tar", last modified: Wed Apr  3 08:26:03 2024, max compression
```

## Comparing `arcticfreeze-0.1.0.tar` & `arcticfreeze-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:44:06.446785 arcticfreeze-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11351 2024-04-02 08:43:58.000000 arcticfreeze-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-02 08:44:06.446785 arcticfreeze-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-02 08:43:58.000000 arcticfreeze-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-02 08:43:58.000000 arcticfreeze-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 08:44:06.446785 arcticfreeze-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:44:06.438785 arcticfreeze-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:44:06.442785 arcticfreeze-0.1.0/src/arcticfreeze/
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-02 08:43:58.000000 arcticfreeze-0.1.0/src/arcticfreeze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-02 08:43:58.000000 arcticfreeze-0.1.0/src/arcticfreeze/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:44:06.442785 arcticfreeze-0.1.0/src/arcticfreeze/_internal/
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-02 08:43:58.000000 arcticfreeze-0.1.0/src/arcticfreeze/_internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:44:06.442785 arcticfreeze-0.1.0/src/arcticfreeze/_internal/_converters/
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-02 08:43:58.000000 arcticfreeze-0.1.0/src/arcticfreeze/_internal/_converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-02 08:43:58.000000 arcticfreeze-0.1.0/src/arcticfreeze/_internal/_converters/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-02 08:43:58.000000 arcticfreeze-0.1.0/src/arcticfreeze/_internal/_converters/standard.py
--rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-04-02 08:43:58.000000 arcticfreeze-0.1.0/src/arcticfreeze/_internal/freeze.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-02 08:43:58.000000 arcticfreeze-0.1.0/src/arcticfreeze/_internal/frozendict.py
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-04-02 08:43:58.000000 arcticfreeze-0.1.0/src/arcticfreeze/_internal/resolve.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-02 08:43:58.000000 arcticfreeze-0.1.0/src/arcticfreeze/_internal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:44:06.446785 arcticfreeze-0.1.0/src/arcticfreeze.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-02 08:44:06.000000 arcticfreeze-0.1.0/src/arcticfreeze.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-02 08:44:06.000000 arcticfreeze-0.1.0/src/arcticfreeze.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 08:44:06.000000 arcticfreeze-0.1.0/src/arcticfreeze.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-02 08:44:06.000000 arcticfreeze-0.1.0/src/arcticfreeze.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-02 08:44:06.000000 arcticfreeze-0.1.0/src/arcticfreeze.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:44:06.446785 arcticfreeze-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-02 08:43:58.000000 arcticfreeze-0.1.0/tests/test_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-02 08:43:58.000000 arcticfreeze-0.1.0/tests/test_freeze.py
--rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-04-02 08:43:58.000000 arcticfreeze-0.1.0/tests/test_frozendict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:26:03.594259 arcticfreeze-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11351 2024-04-03 08:25:59.000000 arcticfreeze-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-04-03 08:26:03.594259 arcticfreeze-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-03 08:25:59.000000 arcticfreeze-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-04-03 08:25:59.000000 arcticfreeze-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 08:26:03.594259 arcticfreeze-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:26:03.586259 arcticfreeze-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:26:03.590259 arcticfreeze-0.1.1/src/arcticfreeze/
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-03 08:25:59.000000 arcticfreeze-0.1.1/src/arcticfreeze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-03 08:25:59.000000 arcticfreeze-0.1.1/src/arcticfreeze/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:26:03.590259 arcticfreeze-0.1.1/src/arcticfreeze/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-03 08:25:59.000000 arcticfreeze-0.1.1/src/arcticfreeze/_internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:26:03.590259 arcticfreeze-0.1.1/src/arcticfreeze/_internal/_converters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-03 08:25:59.000000 arcticfreeze-0.1.1/src/arcticfreeze/_internal/_converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-03 08:25:59.000000 arcticfreeze-0.1.1/src/arcticfreeze/_internal/_converters/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-03 08:25:59.000000 arcticfreeze-0.1.1/src/arcticfreeze/_internal/_converters/standard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-04-03 08:25:59.000000 arcticfreeze-0.1.1/src/arcticfreeze/_internal/freeze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-04-03 08:25:59.000000 arcticfreeze-0.1.1/src/arcticfreeze/_internal/frozendict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-04-03 08:25:59.000000 arcticfreeze-0.1.1/src/arcticfreeze/_internal/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-03 08:25:59.000000 arcticfreeze-0.1.1/src/arcticfreeze/_internal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:26:03.594259 arcticfreeze-0.1.1/src/arcticfreeze.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-04-03 08:26:03.000000 arcticfreeze-0.1.1/src/arcticfreeze.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-03 08:26:03.000000 arcticfreeze-0.1.1/src/arcticfreeze.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 08:26:03.000000 arcticfreeze-0.1.1/src/arcticfreeze.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-03 08:26:03.000000 arcticfreeze-0.1.1/src/arcticfreeze.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 08:26:03.000000 arcticfreeze-0.1.1/src/arcticfreeze.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:26:03.594259 arcticfreeze-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-03 08:25:59.000000 arcticfreeze-0.1.1/tests/test_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-03 08:25:59.000000 arcticfreeze-0.1.1/tests/test_freeze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5650 2024-04-03 08:25:59.000000 arcticfreeze-0.1.1/tests/test_frozendict_pydantic.py
```

### Comparing `arcticfreeze-0.1.0/LICENSE` & `arcticfreeze-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arcticfreeze-0.1.0/PKG-INFO` & `arcticfreeze-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcticfreeze
-Version: 0.1.0
+Version: 0.1.1
 Summary: Enjoy Python on the rocks with deeply (recursively) frozen data structures.
 Author-email: KerstenBreuer <kersten-breuer@outlook.com>
 License: Apache 2.0
 Project-URL: Repository, https://github.com/kerstenbreuer/arcticfreeze
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -15,15 +15,14 @@
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: immutabledict<5,>=4
 Provides-Extra: pydantic
 Requires-Dist: pydantic<3,>=2; extra == "pydantic"
-Requires-Dist: pydantic_core<3,>=2; extra == "pydantic"
 
 [![tests](https://github.com/kerstenbreuer/arcticfreeze/actions/workflows/tests.yaml/badge.svg)](https://github.com/kerstenbreuer/arcticfreeze/actions/workflows/tests.yaml)
 
 # articfreeze
 
 Enjoy Python on the rocks with deeply (recursively) frozen data structures.
```

### Comparing `arcticfreeze-0.1.0/README.md` & `arcticfreeze-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `arcticfreeze-0.1.0/pyproject.toml` & `arcticfreeze-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -17,24 +17,23 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: Apache Software License",
     "Topic :: Software Development :: Libraries",
     "Intended Audience :: Developers",
 ]
 name = "arcticfreeze"
-version = "0.1.0"
+version = "0.1.1"
 description = "Enjoy Python on the rocks with deeply (recursively) frozen data structures."
 dependencies = [
     "immutabledict >=4, <5"
 ]
 
 [project.optional-dependencies]
 pydantic = [
     "pydantic >=2, <3",
-    "pydantic_core >=2, <3",
 ]
 
 [project.license]
 text = "Apache 2.0"
 
 [project.urls]
 Repository = "https://github.com/kerstenbreuer/arcticfreeze"
```

### Comparing `arcticfreeze-0.1.0/src/arcticfreeze/__init__.py` & `arcticfreeze-0.1.1/src/arcticfreeze/__init__.py`

 * *Files identical despite different names*

### Comparing `arcticfreeze-0.1.0/src/arcticfreeze/__main__.py` & `arcticfreeze-0.1.1/src/arcticfreeze/__main__.py`

 * *Files identical despite different names*

### Comparing `arcticfreeze-0.1.0/src/arcticfreeze/_internal/__init__.py` & `arcticfreeze-0.1.1/src/arcticfreeze/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `arcticfreeze-0.1.0/src/arcticfreeze/_internal/_converters/__init__.py` & `arcticfreeze-0.1.1/src/arcticfreeze/_internal/_converters/__init__.py`

 * *Files identical despite different names*

### Comparing `arcticfreeze-0.1.0/src/arcticfreeze/_internal/_converters/base.py` & `arcticfreeze-0.1.1/src/arcticfreeze/_internal/_converters/base.py`

 * *Files identical despite different names*

### Comparing `arcticfreeze-0.1.0/src/arcticfreeze/_internal/_converters/standard.py` & `arcticfreeze-0.1.1/src/arcticfreeze/_internal/_converters/standard.py`

 * *Files identical despite different names*

### Comparing `arcticfreeze-0.1.0/src/arcticfreeze/_internal/freeze.py` & `arcticfreeze-0.1.1/src/arcticfreeze/_internal/freeze.py`

 * *Files identical despite different names*

### Comparing `arcticfreeze-0.1.0/src/arcticfreeze/_internal/resolve.py` & `arcticfreeze-0.1.1/src/arcticfreeze/_internal/resolve.py`

 * *Files identical despite different names*

### Comparing `arcticfreeze-0.1.0/src/arcticfreeze.egg-info/PKG-INFO` & `arcticfreeze-0.1.1/src/arcticfreeze.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcticfreeze
-Version: 0.1.0
+Version: 0.1.1
 Summary: Enjoy Python on the rocks with deeply (recursively) frozen data structures.
 Author-email: KerstenBreuer <kersten-breuer@outlook.com>
 License: Apache 2.0
 Project-URL: Repository, https://github.com/kerstenbreuer/arcticfreeze
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -15,15 +15,14 @@
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: immutabledict<5,>=4
 Provides-Extra: pydantic
 Requires-Dist: pydantic<3,>=2; extra == "pydantic"
-Requires-Dist: pydantic_core<3,>=2; extra == "pydantic"
 
 [![tests](https://github.com/kerstenbreuer/arcticfreeze/actions/workflows/tests.yaml/badge.svg)](https://github.com/kerstenbreuer/arcticfreeze/actions/workflows/tests.yaml)
 
 # articfreeze
 
 Enjoy Python on the rocks with deeply (recursively) frozen data structures.
```

### Comparing `arcticfreeze-0.1.0/src/arcticfreeze.egg-info/SOURCES.txt` & `arcticfreeze-0.1.1/src/arcticfreeze.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 src/arcticfreeze/_internal/resolve.py
 src/arcticfreeze/_internal/utils.py
 src/arcticfreeze/_internal/_converters/__init__.py
 src/arcticfreeze/_internal/_converters/base.py
 src/arcticfreeze/_internal/_converters/standard.py
 tests/test_converters.py
 tests/test_freeze.py
-tests/test_frozendict.py
+tests/test_frozendict_pydantic.py
```

### Comparing `arcticfreeze-0.1.0/tests/test_converters.py` & `arcticfreeze-0.1.1/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `arcticfreeze-0.1.0/tests/test_freeze.py` & `arcticfreeze-0.1.1/tests/test_freeze.py`

 * *Files identical despite different names*

