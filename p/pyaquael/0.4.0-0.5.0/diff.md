# Comparing `tmp/pyaquael-0.4.0.tar.gz` & `tmp/pyaquael-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaquael-0.4.0.tar", last modified: Sat Mar  9 18:47:37 2024, max compression
+gzip compressed data, was "pyaquael-0.5.0.tar", last modified: Wed Apr  3 19:23:52 2024, max compression
```

## Comparing `pyaquael-0.4.0.tar` & `pyaquael-0.5.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 secfha     (501) staff       (20)        0 2024-03-09 18:47:37.301360 pyaquael-0.4.0/
--rw-r--r--   0 secfha     (501) staff       (20)      860 2024-03-09 18:47:37.300965 pyaquael-0.4.0/PKG-INFO
--rw-r--r--   0 secfha     (501) staff       (20)      357 2024-03-09 18:34:36.000000 pyaquael-0.4.0/README.md
--rw-r--r--   0 secfha     (501) staff       (20)      648 2024-03-09 18:46:56.000000 pyaquael-0.4.0/pyproject.toml
--rw-r--r--   0 secfha     (501) staff       (20)       38 2024-03-09 18:47:37.301479 pyaquael-0.4.0/setup.cfg
-drwxr-xr-x   0 secfha     (501) staff       (20)        0 2024-03-09 18:47:37.296520 pyaquael-0.4.0/src/
-drwxr-xr-x   0 secfha     (501) staff       (20)        0 2024-03-09 18:47:37.297745 pyaquael-0.4.0/src/pyaquael/
--rw-r--r--   0 secfha     (501) staff       (20)     1132 2024-03-09 18:43:12.000000 pyaquael-0.4.0/src/pyaquael/__init__.py
--rwxr-xr-x   0 secfha     (501) staff       (20)     2395 2024-03-09 18:46:02.000000 pyaquael-0.4.0/src/pyaquael/aquael.py
-drwxr-xr-x   0 secfha     (501) staff       (20)        0 2024-03-09 18:47:37.300548 pyaquael-0.4.0/src/pyaquael.egg-info/
--rw-r--r--   0 secfha     (501) staff       (20)      860 2024-03-09 18:47:37.000000 pyaquael-0.4.0/src/pyaquael.egg-info/PKG-INFO
--rw-r--r--   0 secfha     (501) staff       (20)      290 2024-03-09 18:47:37.000000 pyaquael-0.4.0/src/pyaquael.egg-info/SOURCES.txt
--rw-r--r--   0 secfha     (501) staff       (20)        1 2024-03-09 18:47:37.000000 pyaquael-0.4.0/src/pyaquael.egg-info/dependency_links.txt
--rw-r--r--   0 secfha     (501) staff       (20)       49 2024-03-09 18:47:37.000000 pyaquael-0.4.0/src/pyaquael.egg-info/entry_points.txt
--rw-r--r--   0 secfha     (501) staff       (20)        7 2024-03-09 18:47:37.000000 pyaquael-0.4.0/src/pyaquael.egg-info/requires.txt
--rw-r--r--   0 secfha     (501) staff       (20)        9 2024-03-09 18:47:37.000000 pyaquael-0.4.0/src/pyaquael.egg-info/top_level.txt
+drwxr-xr-x   0 secfha     (501) staff       (20)        0 2024-04-03 19:23:52.382509 pyaquael-0.5.0/
+-rw-r--r--   0 secfha     (501) staff       (20)      984 2024-04-03 19:23:52.381863 pyaquael-0.5.0/PKG-INFO
+-rw-r--r--   0 secfha     (501) staff       (20)      458 2024-04-03 19:03:45.000000 pyaquael-0.5.0/README.md
+-rw-r--r--   0 secfha     (501) staff       (20)      659 2024-04-03 19:02:25.000000 pyaquael-0.5.0/pyproject.toml
+-rw-r--r--   0 secfha     (501) staff       (20)       38 2024-04-03 19:23:52.382640 pyaquael-0.5.0/setup.cfg
+drwxr-xr-x   0 secfha     (501) staff       (20)        0 2024-04-03 19:23:52.376820 pyaquael-0.5.0/src/
+drwxr-xr-x   0 secfha     (501) staff       (20)        0 2024-04-03 19:23:52.378083 pyaquael-0.5.0/src/pyaquael/
+-rw-r--r--   0 secfha     (501) staff       (20)     1132 2024-03-11 07:03:11.000000 pyaquael-0.5.0/src/pyaquael/__init__.py
+-rwxr-xr-x   0 secfha     (501) staff       (20)     3367 2024-04-03 19:23:09.000000 pyaquael-0.5.0/src/pyaquael/aquael.py
+drwxr-xr-x   0 secfha     (501) staff       (20)        0 2024-04-03 19:23:52.381167 pyaquael-0.5.0/src/pyaquael.egg-info/
+-rw-r--r--   0 secfha     (501) staff       (20)      984 2024-04-03 19:23:52.000000 pyaquael-0.5.0/src/pyaquael.egg-info/PKG-INFO
+-rw-r--r--   0 secfha     (501) staff       (20)      290 2024-04-03 19:23:52.000000 pyaquael-0.5.0/src/pyaquael.egg-info/SOURCES.txt
+-rw-r--r--   0 secfha     (501) staff       (20)        1 2024-04-03 19:23:52.000000 pyaquael-0.5.0/src/pyaquael.egg-info/dependency_links.txt
+-rw-r--r--   0 secfha     (501) staff       (20)       49 2024-04-03 19:23:52.000000 pyaquael-0.5.0/src/pyaquael.egg-info/entry_points.txt
+-rw-r--r--   0 secfha     (501) staff       (20)       15 2024-04-03 19:23:52.000000 pyaquael-0.5.0/src/pyaquael.egg-info/requires.txt
+-rw-r--r--   0 secfha     (501) staff       (20)        9 2024-04-03 19:23:52.000000 pyaquael-0.5.0/src/pyaquael.egg-info/top_level.txt
```

### Comparing `pyaquael-0.4.0/PKG-INFO` & `pyaquael-0.5.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: pyaquael
-Version: 0.4.0
+Version: 0.5.0
 Summary: A python library for the Aquael Leddy link unofficial API
 Author: Christopher Haglund
 Project-URL: Homepage, https://github.com/choffah/pyaquael
 Project-URL: Issues, https://github.com/choffah/pyaquael/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: docopt
+Requires-Dist: asyncio
 
 # pyaquael
 A python library for the Aquael Leddy link unofficial API
 
 ## Usage
 See [simple.py](examples/simple.py) for examples on using library through import.
 
@@ -23,7 +24,13 @@
 ## Build and push to PyPI
 
 ```
 rm -rf dist
 python3 -m build
 python3 -m twine upload dist/*
 ```
+
+## Install local build
+
+```
+python3 -m pip install --force dist/pyaquael-0.5.0-py3-none-any.whl
+```
```

### Comparing `pyaquael-0.4.0/pyproject.toml` & `pyaquael-0.5.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyaquael"
-version = "0.4.0"
+version = "0.5.0"
 authors = [
   { name="Christopher Haglund" },
 ]
 description = "A python library for the Aquael Leddy link unofficial API"
 readme = "README.md"
 requires-python = ">=3.8"
-dependencies = ["docopt"]
+dependencies = ["docopt", "asyncio"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
 ]
 
 [project.scripts]
```

### Comparing `pyaquael-0.4.0/src/pyaquael/__init__.py` & `pyaquael-0.5.0/src/pyaquael/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaquael-0.4.0/src/pyaquael.egg-info/PKG-INFO` & `pyaquael-0.5.0/src/pyaquael.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: pyaquael
-Version: 0.4.0
+Version: 0.5.0
 Summary: A python library for the Aquael Leddy link unofficial API
 Author: Christopher Haglund
 Project-URL: Homepage, https://github.com/choffah/pyaquael
 Project-URL: Issues, https://github.com/choffah/pyaquael/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: docopt
+Requires-Dist: asyncio
 
 # pyaquael
 A python library for the Aquael Leddy link unofficial API
 
 ## Usage
 See [simple.py](examples/simple.py) for examples on using library through import.
 
@@ -23,7 +24,13 @@
 ## Build and push to PyPI
 
 ```
 rm -rf dist
 python3 -m build
 python3 -m twine upload dist/*
 ```
+
+## Install local build
+
+```
+python3 -m pip install --force dist/pyaquael-0.5.0-py3-none-any.whl
+```
```

