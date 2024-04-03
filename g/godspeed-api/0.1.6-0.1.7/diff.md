# Comparing `tmp/godspeed_api-0.1.6.tar.gz` & `tmp/godspeed_api-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "godspeed_api-0.1.6.tar", last modified: Wed Apr  3 15:31:06 2024, max compression
+gzip compressed data, was "godspeed_api-0.1.7.tar", last modified: Wed Apr  3 15:33:55 2024, max compression
```

## Comparing `godspeed_api-0.1.6.tar` & `godspeed_api-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:31:06.686177 godspeed_api-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-03 15:31:02.000000 godspeed_api-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-03 15:31:06.686177 godspeed_api-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-03 15:31:02.000000 godspeed_api-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:31:06.686177 godspeed_api-0.1.6/godspeed_api/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-03 15:31:02.000000 godspeed_api-0.1.6/godspeed_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-03 15:31:02.000000 godspeed_api-0.1.6/godspeed_api/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:31:06.686177 godspeed_api-0.1.6/godspeed_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-03 15:31:06.000000 godspeed_api-0.1.6/godspeed_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-03 15:31:06.000000 godspeed_api-0.1.6/godspeed_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 15:31:06.000000 godspeed_api-0.1.6/godspeed_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 15:31:06.000000 godspeed_api-0.1.6/godspeed_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 15:31:06.000000 godspeed_api-0.1.6/godspeed_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 15:31:06.686177 godspeed_api-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-03 15:31:02.000000 godspeed_api-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:33:55.935861 godspeed_api-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-03 15:33:51.000000 godspeed_api-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-03 15:33:55.935861 godspeed_api-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-03 15:33:51.000000 godspeed_api-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:33:55.931861 godspeed_api-0.1.7/godspeed_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-03 15:33:51.000000 godspeed_api-0.1.7/godspeed_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-03 15:33:51.000000 godspeed_api-0.1.7/godspeed_api/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:33:55.935861 godspeed_api-0.1.7/godspeed_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-03 15:33:55.000000 godspeed_api-0.1.7/godspeed_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-03 15:33:55.000000 godspeed_api-0.1.7/godspeed_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 15:33:55.000000 godspeed_api-0.1.7/godspeed_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 15:33:55.000000 godspeed_api-0.1.7/godspeed_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-03 15:33:55.000000 godspeed_api-0.1.7/godspeed_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 15:33:55.935861 godspeed_api-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-03 15:33:51.000000 godspeed_api-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:33:55.935861 godspeed_api-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 15:33:51.000000 godspeed_api-0.1.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-03 15:33:51.000000 godspeed_api-0.1.7/tests/test_api.py
```

### Comparing `godspeed_api-0.1.6/LICENSE` & `godspeed_api-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `godspeed_api-0.1.6/PKG-INFO` & `godspeed_api-0.1.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: godspeed_api
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Godspeed task manager API wrapper
 Author: Artem Trubacheev
 Author-email: almaz5200@gmail.com
 Keywords: python,godspeed
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
@@ -16,15 +16,15 @@
 Requires-Dist: requests
 
 # Godspeed-API
 
 [![Python 3.9+](https://img.shields.io/badge/python-3.9%2B-blue)](https://www.python.org/downloads/release/python-390/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
-A Python API package for [Godspeed](https://godspeedapp.com/)'. The package implements basic authentication and task creation functionalities when the API is documented more.
+A Python API package for [Godspeed](https://godspeedapp.com/). The package implements basic authentication and task creation functionalities, this will be extended as the API is documented more.
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install Godspeed-API.
 
 ```bash
 pip install godspeed-api
```

### Comparing `godspeed_api-0.1.6/README.md` & `godspeed_api-0.1.7/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Godspeed-API
 
 [![Python 3.9+](https://img.shields.io/badge/python-3.9%2B-blue)](https://www.python.org/downloads/release/python-390/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
-A Python API package for [Godspeed](https://godspeedapp.com/)'. The package implements basic authentication and task creation functionalities when the API is documented more.
+A Python API package for [Godspeed](https://godspeedapp.com/). The package implements basic authentication and task creation functionalities, this will be extended as the API is documented more.
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install Godspeed-API.
 
 ```bash
 pip install godspeed-api
```

### Comparing `godspeed_api-0.1.6/godspeed_api/api.py` & `godspeed_api-0.1.7/godspeed_api/api.py`

 * *Files identical despite different names*

### Comparing `godspeed_api-0.1.6/godspeed_api.egg-info/PKG-INFO` & `godspeed_api-0.1.7/godspeed_api.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: godspeed_api
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Godspeed task manager API wrapper
 Author: Artem Trubacheev
 Author-email: almaz5200@gmail.com
 Keywords: python,godspeed
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
@@ -16,15 +16,15 @@
 Requires-Dist: requests
 
 # Godspeed-API
 
 [![Python 3.9+](https://img.shields.io/badge/python-3.9%2B-blue)](https://www.python.org/downloads/release/python-390/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
-A Python API package for [Godspeed](https://godspeedapp.com/)'. The package implements basic authentication and task creation functionalities when the API is documented more.
+A Python API package for [Godspeed](https://godspeedapp.com/). The package implements basic authentication and task creation functionalities, this will be extended as the API is documented more.
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install Godspeed-API.
 
 ```bash
 pip install godspeed-api
```

### Comparing `godspeed_api-0.1.6/setup.py` & `godspeed_api-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
-VERSION = "0.1.6"
+VERSION = "0.1.7"
 DESCRIPTION = "A Godspeed task manager API wrapper"
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="godspeed_api",
```

