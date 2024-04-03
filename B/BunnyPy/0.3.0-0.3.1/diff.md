# Comparing `tmp/BunnyPy-0.3.0.tar.gz` & `tmp/BunnyPy-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BunnyPy-0.3.0.tar", last modified: Thu Feb 23 16:46:58 2023, max compression
+gzip compressed data, was "BunnyPy-0.3.1.tar", last modified: Wed Apr  3 02:14:41 2024, max compression
```

## Comparing `BunnyPy-0.3.0.tar` & `BunnyPy-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:46:58.009631 BunnyPy-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:46:58.009631 BunnyPy-0.3.0/BunnyPy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-02-23 16:46:57.000000 BunnyPy-0.3.0/BunnyPy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-02-23 16:46:57.000000 BunnyPy-0.3.0/BunnyPy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 16:46:57.000000 BunnyPy-0.3.0/BunnyPy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-23 16:46:57.000000 BunnyPy-0.3.0/BunnyPy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-02-23 16:46:47.000000 BunnyPy-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-23 16:46:47.000000 BunnyPy-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-02-23 16:46:58.009631 BunnyPy-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-02-23 16:46:47.000000 BunnyPy-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:46:58.009631 BunnyPy-0.3.0/bunnypy/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-02-23 16:46:47.000000 BunnyPy-0.3.0/bunnypy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:46:58.009631 BunnyPy-0.3.0/bunnypy/asset/
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-02-23 16:46:47.000000 BunnyPy-0.3.0/bunnypy/asset/error.html
--rw-r--r--   0 runner    (1001) docker     (123)    21558 2023-02-23 16:46:47.000000 BunnyPy-0.3.0/bunnypy/bunnypy.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 16:46:58.009631 BunnyPy-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-02-23 16:46:47.000000 BunnyPy-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:14:41.697642 BunnyPy-0.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:14:41.697642 BunnyPy-0.3.1/BunnyPy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-03 02:14:41.000000 BunnyPy-0.3.1/BunnyPy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-03 02:14:41.000000 BunnyPy-0.3.1/BunnyPy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:14:41.000000 BunnyPy-0.3.1/BunnyPy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 02:14:41.000000 BunnyPy-0.3.1/BunnyPy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-03 02:14:31.000000 BunnyPy-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-03 02:14:31.000000 BunnyPy-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-03 02:14:41.697642 BunnyPy-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-03 02:14:31.000000 BunnyPy-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:14:41.697642 BunnyPy-0.3.1/bunnypy/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-03 02:14:31.000000 BunnyPy-0.3.1/bunnypy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:14:41.697642 BunnyPy-0.3.1/bunnypy/asset/
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-03 02:14:31.000000 BunnyPy-0.3.1/bunnypy/asset/error.html
+-rw-r--r--   0 runner    (1001) docker     (127)    21948 2024-04-03 02:14:31.000000 BunnyPy-0.3.1/bunnypy/bunnypy.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 02:14:41.697642 BunnyPy-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-03 02:14:31.000000 BunnyPy-0.3.1/setup.py
```

### Comparing `BunnyPy-0.3.0/BunnyPy.egg-info/PKG-INFO` & `BunnyPy-0.3.1/BunnyPy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BunnyPy
-Version: 0.3.0
+Version: 0.3.1
 Summary: Lightweight Python Web Framework
 Home-page: https://github.com/ivanlulyf/bunnypy
 Author: IvanLuLyf
 Author-email: me@ivanlu.cn
 License: MIT
 Platform: any
 Classifier: Operating System :: OS Independent
```

### Comparing `BunnyPy-0.3.0/LICENSE` & `BunnyPy-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `BunnyPy-0.3.0/PKG-INFO` & `BunnyPy-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BunnyPy
-Version: 0.3.0
+Version: 0.3.1
 Summary: Lightweight Python Web Framework
 Home-page: https://github.com/ivanlulyf/bunnypy
 Author: IvanLuLyf
 Author-email: me@ivanlu.cn
 License: MIT
 Platform: any
 Classifier: Operating System :: OS Independent
```

### Comparing `BunnyPy-0.3.0/README.md` & `BunnyPy-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `BunnyPy-0.3.0/bunnypy/asset/error.html` & `BunnyPy-0.3.1/bunnypy/asset/error.html`

 * *Files identical despite different names*

### Comparing `BunnyPy-0.3.0/bunnypy/bunnypy.py` & `BunnyPy-0.3.1/bunnypy/bunnypy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import json
 import os
 import re
 import traceback
+import types
 from html import escape
 from pathlib import Path
 from urllib.parse import parse_qs
 from wsgiref.simple_server import make_server
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 
 __default_html__ = '''<html lang="en"><head><meta charset="utf-8"><title>Welcome to BunnyPy</title>
 <style>body{width: 35em;margin: 0 auto;text-align: center;}</style></head><body>
 <a href="https://github.com/IvanLuLyf/BunnyPy">
 <img src="https://github.com/IvanLuLyf/BunnyPy/raw/master/logo.png?raw=true" width="400px" style="margin-top: 150px">
 </a>
 <h1>Welcome to <a href="https://github.com/IvanLuLyf/BunnyPy">BunnyPy</a>!</h1>
@@ -35,14 +36,15 @@
 __def_allowed_methods__ = ', '.join(['GET', 'POST', 'PUT', 'DELETE'])
 __def_allowed_headers__ = ', '.join(['Content-Type', 'Authorization'])
 
 
 class Bunny:
     __sub_apps__ = {}
     __controllers__ = {}
+    __cors__ = None
     request_method = 'GET'
 
     def handler(self, environ, start_response):
         if callable(self.__cors__):
             cors_conf = self.__cors__(environ)
         else:
             cors_conf = {}
@@ -71,18 +73,23 @@
         if len(self.__controllers__.keys()) > 0:
             if len(url_array) > 2:
                 action = url_array[2].lower()
             else:
                 action = 'index'
             req = self.Request(environ)
             response = self.__call_action__(req, url_array[1], action)
-            if type(response) == dict or type(response) == list:
+            if isinstance(response, dict) or isinstance(response, list):
                 start_response('200 OK', [('Access-Control-Allow-Origin', allowed_origin),
                                           ('Content-Type', 'application/json;charset=utf-8')])
                 return [json.dumps(response).encode('utf-8')]
+            elif isinstance(response, types.GeneratorType):
+                start_response('200 OK', [('Access-Control-Allow-Origin', allowed_origin),
+                                          ('Content-Type', 'text/event-stream;charset=utf-8')])
+                for chunk in response:
+                    yield f'data: {chunk}\n\n'.encode('utf-8')
             else:
                 start_response('200 OK', [('Access-Control-Allow-Origin', allowed_origin),
                                           ('Content-Type', 'text/html;charset=utf-8')])
                 return [response.encode('utf-8')]
         else:
             start_response('200 OK', [('Access-Control-Allow-Origin', allowed_origin),
                                       ('Content-Type', 'text/html;charset=utf-8')])
```

### Comparing `BunnyPy-0.3.0/setup.py` & `BunnyPy-0.3.1/setup.py`

 * *Files identical despite different names*

