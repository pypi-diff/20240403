# Comparing `tmp/BunnyPy-0.2.9.tar.gz` & `tmp/BunnyPy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BunnyPy-0.2.9.tar", last modified: Thu Feb 23 16:37:07 2023, max compression
+gzip compressed data, was "BunnyPy-0.3.0.tar", last modified: Thu Feb 23 16:46:58 2023, max compression
```

## Comparing `BunnyPy-0.2.9.tar` & `BunnyPy-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:37:07.450154 BunnyPy-0.2.9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:37:07.450154 BunnyPy-0.2.9/BunnyPy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-02-23 16:37:07.000000 BunnyPy-0.2.9/BunnyPy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-02-23 16:37:07.000000 BunnyPy-0.2.9/BunnyPy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 16:37:07.000000 BunnyPy-0.2.9/BunnyPy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-23 16:37:07.000000 BunnyPy-0.2.9/BunnyPy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-02-23 16:36:52.000000 BunnyPy-0.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-23 16:36:52.000000 BunnyPy-0.2.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-02-23 16:37:07.450154 BunnyPy-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-02-23 16:36:52.000000 BunnyPy-0.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:37:07.450154 BunnyPy-0.2.9/bunnypy/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-02-23 16:36:52.000000 BunnyPy-0.2.9/bunnypy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:37:07.450154 BunnyPy-0.2.9/bunnypy/asset/
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-02-23 16:36:52.000000 BunnyPy-0.2.9/bunnypy/asset/error.html
--rw-r--r--   0 runner    (1001) docker     (123)    21289 2023-02-23 16:36:52.000000 BunnyPy-0.2.9/bunnypy/bunnypy.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 16:37:07.450154 BunnyPy-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-02-23 16:36:52.000000 BunnyPy-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:46:58.009631 BunnyPy-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:46:58.009631 BunnyPy-0.3.0/BunnyPy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-02-23 16:46:57.000000 BunnyPy-0.3.0/BunnyPy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-02-23 16:46:57.000000 BunnyPy-0.3.0/BunnyPy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 16:46:57.000000 BunnyPy-0.3.0/BunnyPy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-23 16:46:57.000000 BunnyPy-0.3.0/BunnyPy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-02-23 16:46:47.000000 BunnyPy-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-23 16:46:47.000000 BunnyPy-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-02-23 16:46:58.009631 BunnyPy-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-02-23 16:46:47.000000 BunnyPy-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:46:58.009631 BunnyPy-0.3.0/bunnypy/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-02-23 16:46:47.000000 BunnyPy-0.3.0/bunnypy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:46:58.009631 BunnyPy-0.3.0/bunnypy/asset/
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-02-23 16:46:47.000000 BunnyPy-0.3.0/bunnypy/asset/error.html
+-rw-r--r--   0 runner    (1001) docker     (123)    21558 2023-02-23 16:46:47.000000 BunnyPy-0.3.0/bunnypy/bunnypy.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 16:46:58.009631 BunnyPy-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-02-23 16:46:47.000000 BunnyPy-0.3.0/setup.py
```

### Comparing `BunnyPy-0.2.9/BunnyPy.egg-info/PKG-INFO` & `BunnyPy-0.3.0/BunnyPy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BunnyPy
-Version: 0.2.9
+Version: 0.3.0
 Summary: Lightweight Python Web Framework
 Home-page: https://github.com/ivanlulyf/bunnypy
 Author: IvanLuLyf
 Author-email: me@ivanlu.cn
 License: MIT
 Platform: any
 Classifier: Operating System :: OS Independent
```

### Comparing `BunnyPy-0.2.9/LICENSE` & `BunnyPy-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `BunnyPy-0.2.9/PKG-INFO` & `BunnyPy-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BunnyPy
-Version: 0.2.9
+Version: 0.3.0
 Summary: Lightweight Python Web Framework
 Home-page: https://github.com/ivanlulyf/bunnypy
 Author: IvanLuLyf
 Author-email: me@ivanlu.cn
 License: MIT
 Platform: any
 Classifier: Operating System :: OS Independent
```

### Comparing `BunnyPy-0.2.9/README.md` & `BunnyPy-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `BunnyPy-0.2.9/bunnypy/asset/error.html` & `BunnyPy-0.3.0/bunnypy/asset/error.html`

 * *Files identical despite different names*

### Comparing `BunnyPy-0.2.9/bunnypy/bunnypy.py` & `BunnyPy-0.3.0/bunnypy/bunnypy.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import re
 import traceback
 from html import escape
 from pathlib import Path
 from urllib.parse import parse_qs
 from wsgiref.simple_server import make_server
 
-__version__ = "0.2.9"
+__version__ = "0.3.0"
 
 __default_html__ = '''<html lang="en"><head><meta charset="utf-8"><title>Welcome to BunnyPy</title>
 <style>body{width: 35em;margin: 0 auto;text-align: center;}</style></head><body>
 <a href="https://github.com/IvanLuLyf/BunnyPy">
 <img src="https://github.com/IvanLuLyf/BunnyPy/raw/master/logo.png?raw=true" width="400px" style="margin-top: 150px">
 </a>
 <h1>Welcome to <a href="https://github.com/IvanLuLyf/BunnyPy">BunnyPy</a>!</h1>
@@ -72,21 +72,24 @@
             if len(url_array) > 2:
                 action = url_array[2].lower()
             else:
                 action = 'index'
             req = self.Request(environ)
             response = self.__call_action__(req, url_array[1], action)
             if type(response) == dict or type(response) == list:
-                start_response('200 OK', [('Content-Type', 'application/json;charset=utf-8')])
+                start_response('200 OK', [('Access-Control-Allow-Origin', allowed_origin),
+                                          ('Content-Type', 'application/json;charset=utf-8')])
                 return [json.dumps(response).encode('utf-8')]
             else:
-                start_response('200 OK', [('Content-Type', 'text/html;charset=utf-8')])
+                start_response('200 OK', [('Access-Control-Allow-Origin', allowed_origin),
+                                          ('Content-Type', 'text/html;charset=utf-8')])
                 return [response.encode('utf-8')]
         else:
-            start_response('200 OK', [('Content-Type', 'text/html;charset=utf-8')])
+            start_response('200 OK', [('Access-Control-Allow-Origin', allowed_origin),
+                                      ('Content-Type', 'text/html;charset=utf-8')])
             return [__default_html__.encode('utf-8')]
 
     def __init__(self, host='127.0.0.1', port=8000, database=None, cors=None):
         self.__host__ = host
         self.__port__ = port
         if isinstance(database, self.Database):
             self.__database__ = database
```

### Comparing `BunnyPy-0.2.9/setup.py` & `BunnyPy-0.3.0/setup.py`

 * *Files identical despite different names*

