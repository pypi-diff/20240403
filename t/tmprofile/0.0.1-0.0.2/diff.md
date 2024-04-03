# Comparing `tmp/tmprofile-0.0.1.tar.gz` & `tmp/tmprofile-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmprofile-0.0.1.tar", last modified: Wed Apr  3 14:11:23 2024, max compression
+gzip compressed data, was "tmprofile-0.0.2.tar", last modified: Wed Apr  3 14:28:34 2024, max compression
```

## Comparing `tmprofile-0.0.1.tar` & `tmprofile-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 vedrenne (271197) images    (7000)        0 2024-04-03 14:11:23.971964 tmprofile-0.0.1/
--rw-r--r--   0 vedrenne (271197) images    (7000)     1074 2024-04-03 14:04:43.000000 tmprofile-0.0.1/LICENSE
--rw-r--r--   0 vedrenne (271197) images    (7000)     2012 2024-04-03 14:11:23.971964 tmprofile-0.0.1/PKG-INFO
--rw-r--r--   0 vedrenne (271197) images    (7000)     1475 2024-04-03 14:03:53.000000 tmprofile-0.0.1/README.md
--rw-r--r--   0 vedrenne (271197) images    (7000)      607 2024-04-03 14:11:03.000000 tmprofile-0.0.1/pyproject.toml
--rw-r--r--   0 vedrenne (271197) images    (7000)       38 2024-04-03 14:11:23.971964 tmprofile-0.0.1/setup.cfg
-drwxr-xr-x   0 vedrenne (271197) images    (7000)        0 2024-04-03 14:11:23.971964 tmprofile-0.0.1/tmprofile/
--rw-r--r--   0 vedrenne (271197) images    (7000)       40 2024-04-03 14:04:17.000000 tmprofile-0.0.1/tmprofile/__init__.py
--rw-r--r--   0 vedrenne (271197) images    (7000)    12251 2024-04-03 13:43:57.000000 tmprofile-0.0.1/tmprofile/pyprofile.py
-drwxr-xr-x   0 vedrenne (271197) images    (7000)        0 2024-04-03 14:11:23.971964 tmprofile-0.0.1/tmprofile.egg-info/
--rw-r--r--   0 vedrenne (271197) images    (7000)     2012 2024-04-03 14:11:23.000000 tmprofile-0.0.1/tmprofile.egg-info/PKG-INFO
--rw-r--r--   0 vedrenne (271197) images    (7000)      209 2024-04-03 14:11:23.000000 tmprofile-0.0.1/tmprofile.egg-info/SOURCES.txt
--rw-r--r--   0 vedrenne (271197) images    (7000)        1 2024-04-03 14:11:23.000000 tmprofile-0.0.1/tmprofile.egg-info/dependency_links.txt
--rw-r--r--   0 vedrenne (271197) images    (7000)       10 2024-04-03 14:11:23.000000 tmprofile-0.0.1/tmprofile.egg-info/top_level.txt
+drwxr-xr-x   0 vedrenne (271197) images    (7000)        0 2024-04-03 14:28:34.381188 tmprofile-0.0.2/
+-rw-r--r--   0 vedrenne (271197) images    (7000)     1074 2024-04-03 14:04:43.000000 tmprofile-0.0.2/LICENSE
+-rw-r--r--   0 vedrenne (271197) images    (7000)     2180 2024-04-03 14:28:34.381188 tmprofile-0.0.2/PKG-INFO
+-rw-r--r--   0 vedrenne (271197) images    (7000)     1518 2024-04-03 14:18:13.000000 tmprofile-0.0.2/README.md
+-rw-r--r--   0 vedrenne (271197) images    (7000)      835 2024-04-03 14:17:45.000000 tmprofile-0.0.2/pyproject.toml
+-rw-r--r--   0 vedrenne (271197) images    (7000)       38 2024-04-03 14:28:34.381188 tmprofile-0.0.2/setup.cfg
+drwxr-xr-x   0 vedrenne (271197) images    (7000)        0 2024-04-03 14:28:34.381188 tmprofile-0.0.2/tmprofile/
+-rw-r--r--   0 vedrenne (271197) images    (7000)       40 2024-04-03 14:04:17.000000 tmprofile-0.0.2/tmprofile/__init__.py
+-rw-r--r--   0 vedrenne (271197) images    (7000)    12251 2024-04-03 14:24:48.000000 tmprofile-0.0.2/tmprofile/pyprofile.py
+drwxr-xr-x   0 vedrenne (271197) images    (7000)        0 2024-04-03 14:28:34.381188 tmprofile-0.0.2/tmprofile.egg-info/
+-rw-r--r--   0 vedrenne (271197) images    (7000)     2180 2024-04-03 14:28:34.000000 tmprofile-0.0.2/tmprofile.egg-info/PKG-INFO
+-rw-r--r--   0 vedrenne (271197) images    (7000)      241 2024-04-03 14:28:34.000000 tmprofile-0.0.2/tmprofile.egg-info/SOURCES.txt
+-rw-r--r--   0 vedrenne (271197) images    (7000)        1 2024-04-03 14:28:34.000000 tmprofile-0.0.2/tmprofile.egg-info/dependency_links.txt
+-rw-r--r--   0 vedrenne (271197) images    (7000)       50 2024-04-03 14:28:34.000000 tmprofile-0.0.2/tmprofile.egg-info/requires.txt
+-rw-r--r--   0 vedrenne (271197) images    (7000)       10 2024-04-03 14:28:34.000000 tmprofile-0.0.2/tmprofile.egg-info/top_level.txt
```

### Comparing `tmprofile-0.0.1/LICENSE` & `tmprofile-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tmprofile-0.0.1/PKG-INFO` & `tmprofile-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 Metadata-Version: 2.1
 Name: tmprofile
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple time, ram & vram python profiler.
 Author-email: Luc Vedrenne <vedrenneluc@gmail.com>
 Project-URL: Homepage, https://github.com/ListIndexOutOfRange/pyprofile
 Project-URL: Issues, https://github.com/ListIndexOutOfRange/pyprofile/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: matplotlib
+Requires-Dist: psutil
+Requires-Dist: prettytable
+Requires-Dist: nvidia_ml_py3
 
 # A simple time and memory Python profiler
 
+## Installation
+
+`pip install tmprofile`
+
+
 ## Usage
 
 ### 1. As a context manager
 
 ```python
 from tmprofile import Profile
```

### Comparing `tmprofile-0.0.1/README.md` & `tmprofile-0.0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # A simple time and memory Python profiler
 
+## Installation
+
+`pip install tmprofile`
+
+
 ## Usage
 
 ### 1. As a context manager
 
 ```python
 from tmprofile import Profile
```

### Comparing `tmprofile-0.0.1/tmprofile/pyprofile.py` & `tmprofile-0.0.2/tmprofile/pyprofile.py`

 * *Files identical despite different names*

### Comparing `tmprofile-0.0.1/tmprofile.egg-info/PKG-INFO` & `tmprofile-0.0.2/tmprofile.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 Metadata-Version: 2.1
 Name: tmprofile
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple time, ram & vram python profiler.
 Author-email: Luc Vedrenne <vedrenneluc@gmail.com>
 Project-URL: Homepage, https://github.com/ListIndexOutOfRange/pyprofile
 Project-URL: Issues, https://github.com/ListIndexOutOfRange/pyprofile/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: matplotlib
+Requires-Dist: psutil
+Requires-Dist: prettytable
+Requires-Dist: nvidia_ml_py3
 
 # A simple time and memory Python profiler
 
+## Installation
+
+`pip install tmprofile`
+
+
 ## Usage
 
 ### 1. As a context manager
 
 ```python
 from tmprofile import Profile
```

