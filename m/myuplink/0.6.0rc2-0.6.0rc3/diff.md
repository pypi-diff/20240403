# Comparing `tmp/myuplink-0.6.0rc2.tar.gz` & `tmp/myuplink-0.6.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myuplink-0.6.0rc2.tar", last modified: Mon Mar 11 08:19:08 2024, max compression
+gzip compressed data, was "myuplink-0.6.0rc3.tar", last modified: Wed Apr  3 06:29:57 2024, max compression
```

## Comparing `myuplink-0.6.0rc2.tar` & `myuplink-0.6.0rc3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 08:19:08.785215 myuplink-0.6.0rc2/
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-03-11 08:19:08.785215 myuplink-0.6.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-03-11 08:18:55.000000 myuplink-0.6.0rc2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-11 08:18:55.000000 myuplink-0.6.0rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-03-11 08:19:08.785215 myuplink-0.6.0rc2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 08:19:08.781215 myuplink-0.6.0rc2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 08:19:08.781215 myuplink-0.6.0rc2/src/myuplink/
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-03-11 08:18:55.000000 myuplink-0.6.0rc2/src/myuplink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6705 2024-03-11 08:18:55.000000 myuplink-0.6.0rc2/src/myuplink/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-03-11 08:18:55.000000 myuplink-0.6.0rc2/src/myuplink/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-03-11 08:18:55.000000 myuplink-0.6.0rc2/src/myuplink/auth_abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    13581 2024-03-11 08:18:55.000000 myuplink-0.6.0rc2/src/myuplink/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-03-11 08:18:55.000000 myuplink-0.6.0rc2/src/myuplink/names.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 08:18:55.000000 myuplink-0.6.0rc2/src/myuplink/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 08:19:08.785215 myuplink-0.6.0rc2/src/myuplink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-03-11 08:19:08.000000 myuplink-0.6.0rc2/src/myuplink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-03-11 08:19:08.000000 myuplink-0.6.0rc2/src/myuplink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 08:19:08.000000 myuplink-0.6.0rc2/src/myuplink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-11 08:19:08.000000 myuplink-0.6.0rc2/src/myuplink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-11 08:19:08.000000 myuplink-0.6.0rc2/src/myuplink.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:29:57.641595 myuplink-0.6.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-03 06:29:57.641595 myuplink-0.6.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-03 06:29:47.000000 myuplink-0.6.0rc3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-03 06:29:47.000000 myuplink-0.6.0rc3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-03 06:29:57.645595 myuplink-0.6.0rc3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:29:57.641595 myuplink-0.6.0rc3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:29:57.641595 myuplink-0.6.0rc3/src/myuplink/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-03 06:29:47.000000 myuplink-0.6.0rc3/src/myuplink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6705 2024-04-03 06:29:47.000000 myuplink-0.6.0rc3/src/myuplink/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-03 06:29:47.000000 myuplink-0.6.0rc3/src/myuplink/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-03 06:29:47.000000 myuplink-0.6.0rc3/src/myuplink/auth_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13581 2024-04-03 06:29:47.000000 myuplink-0.6.0rc3/src/myuplink/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-03 06:29:47.000000 myuplink-0.6.0rc3/src/myuplink/names.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:29:47.000000 myuplink-0.6.0rc3/src/myuplink/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:29:57.641595 myuplink-0.6.0rc3/src/myuplink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-03 06:29:57.000000 myuplink-0.6.0rc3/src/myuplink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-03 06:29:57.000000 myuplink-0.6.0rc3/src/myuplink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 06:29:57.000000 myuplink-0.6.0rc3/src/myuplink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-03 06:29:57.000000 myuplink-0.6.0rc3/src/myuplink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 06:29:57.000000 myuplink-0.6.0rc3/src/myuplink.egg-info/top_level.txt
```

### Comparing `myuplink-0.6.0rc2/PKG-INFO` & `myuplink-0.6.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myuplink
-Version: 0.6.0rc2
+Version: 0.6.0rc3
 Summary: API package for myUplink
 Home-page: https://github.com/pajzo/myuplink
 Author: Peter Winkler
 Author-email: peter@fluxi.dk
 Project-URL: Bug Tracker, https://github.com/pajzo/myuplink/issues
 Project-URL: repository, https://github.com/pajzo/myuplink
 Classifier: Programming Language :: Python :: 3
```

### Comparing `myuplink-0.6.0rc2/setup.cfg` & `myuplink-0.6.0rc3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = myuplink
-version = 0.6.0rc2
+version = 0.6.0rc3
 author = Peter Winkler
 author_email = peter@fluxi.dk
 description = API package for myUplink
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pajzo/myuplink
 project_urls =
```

### Comparing `myuplink-0.6.0rc2/src/myuplink/api.py` & `myuplink-0.6.0rc3/src/myuplink/api.py`

 * *Files identical despite different names*

### Comparing `myuplink-0.6.0rc2/src/myuplink/auth.py` & `myuplink-0.6.0rc3/src/myuplink/auth.py`

 * *Files identical despite different names*

### Comparing `myuplink-0.6.0rc2/src/myuplink/auth_abstract.py` & `myuplink-0.6.0rc3/src/myuplink/auth_abstract.py`

 * *Files identical despite different names*

### Comparing `myuplink-0.6.0rc2/src/myuplink/models.py` & `myuplink-0.6.0rc3/src/myuplink/models.py`

 * *Files identical despite different names*

### Comparing `myuplink-0.6.0rc2/src/myuplink/names.py` & `myuplink-0.6.0rc3/src/myuplink/names.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Methods for getting names etc from API data."""
+
 import re
 from .models import Device, System
 
 
 MAP_NIBEF = {"manufacturer": "Nibe", "series": "F"}
 MAP_NIBES = {"manufacturer": "Nibe", "series": "S"}
 NAME_MAP = {
@@ -53,15 +54,15 @@
 
 def get_model(device: Device) -> str | None:
     """Return model name."""
     for model in NAME_MAP:
         if re.search(model, device.product_name):
             return model
     name_list = device.product_name.split()
-    if len(name_list == 0):
+    if len(name_list) == 1:
         model = name_list[0]
     else:
         model = " ".join(name_list[1:])
     return model
 
 
 def get_series(device: Device) -> str | None:
```

### Comparing `myuplink-0.6.0rc2/src/myuplink.egg-info/PKG-INFO` & `myuplink-0.6.0rc3/src/myuplink.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myuplink
-Version: 0.6.0rc2
+Version: 0.6.0rc3
 Summary: API package for myUplink
 Home-page: https://github.com/pajzo/myuplink
 Author: Peter Winkler
 Author-email: peter@fluxi.dk
 Project-URL: Bug Tracker, https://github.com/pajzo/myuplink/issues
 Project-URL: repository, https://github.com/pajzo/myuplink
 Classifier: Programming Language :: Python :: 3
```

