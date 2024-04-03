# Comparing `tmp/catframes-2024.3.0.tar.gz` & `tmp/catframes-2024.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catframes-2024.3.0.tar", last modified: Sun Mar 31 01:03:46 2024, max compression
+gzip compressed data, was "catframes-2024.3.1.tar", last modified: Wed Apr  3 00:23:10 2024, max compression
```

## Comparing `catframes-2024.3.0.tar` & `catframes-2024.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-sr-x   0 me        (1000) me        (1000)        0 2024-03-31 01:03:46.481793 catframes-2024.3.0/
--rw-r--r--   0 me        (1000) me        (1000)      875 2024-03-30 23:50:03.000000 catframes-2024.3.0/LICENSE.txt
--rw-r--r--   0 me        (1000) me        (1000)     6311 2024-03-31 01:03:46.481793 catframes-2024.3.0/PKG-INFO
--rw-r--r--   0 me        (1000) me        (1000)     4808 2024-03-30 23:50:03.000000 catframes-2024.3.0/README.md
--rw-r--r--   0 me        (1000) me        (1000)      875 2024-03-30 23:50:03.000000 catframes-2024.3.0/pyproject.toml
--rw-r--r--   0 me        (1000) me        (1000)       38 2024-03-31 01:03:46.481793 catframes-2024.3.0/setup.cfg
-drwxr-sr-x   0 me        (1000) me        (1000)        0 2024-03-31 01:03:46.441802 catframes-2024.3.0/src/
-drwxr-sr-x   0 me        (1000) me        (1000)        0 2024-03-31 01:03:46.451800 catframes-2024.3.0/src/catframes/
--rw-r--r--   0 me        (1000) me        (1000)       18 2023-09-24 19:02:05.000000 catframes-2024.3.0/src/catframes/__init__.py
--rw-r--r--   0 me        (1000) me        (1000)   138204 2024-03-30 23:52:39.000000 catframes-2024.3.0/src/catframes/catframes.py
-drwxr-sr-x   0 me        (1000) me        (1000)        0 2024-03-31 01:03:46.471795 catframes-2024.3.0/src/catframes.egg-info/
--rw-r--r--   0 me        (1000) me        (1000)     6311 2024-03-31 01:03:46.000000 catframes-2024.3.0/src/catframes.egg-info/PKG-INFO
--rw-r--r--   0 me        (1000) me        (1000)      313 2024-03-31 01:03:46.000000 catframes-2024.3.0/src/catframes.egg-info/SOURCES.txt
--rw-r--r--   0 me        (1000) me        (1000)        1 2024-03-31 01:03:46.000000 catframes-2024.3.0/src/catframes.egg-info/dependency_links.txt
--rw-r--r--   0 me        (1000) me        (1000)       55 2024-03-31 01:03:46.000000 catframes-2024.3.0/src/catframes.egg-info/entry_points.txt
--rw-r--r--   0 me        (1000) me        (1000)       14 2024-03-31 01:03:46.000000 catframes-2024.3.0/src/catframes.egg-info/requires.txt
--rw-r--r--   0 me        (1000) me        (1000)       10 2024-03-31 01:03:46.000000 catframes-2024.3.0/src/catframes.egg-info/top_level.txt
+drwxr-sr-x   0 me        (1000) me        (1000)        0 2024-04-03 00:23:10.862280 catframes-2024.3.1/
+-rw-r--r--   0 me        (1000) me        (1000)      875 2024-04-02 23:58:18.000000 catframes-2024.3.1/LICENSE.txt
+-rw-r--r--   0 me        (1000) me        (1000)     6311 2024-04-03 00:23:10.862280 catframes-2024.3.1/PKG-INFO
+-rw-r--r--   0 me        (1000) me        (1000)     4808 2024-04-02 23:58:18.000000 catframes-2024.3.1/README.md
+-rw-r--r--   0 me        (1000) me        (1000)      875 2024-04-03 00:00:14.000000 catframes-2024.3.1/pyproject.toml
+-rw-r--r--   0 me        (1000) me        (1000)       38 2024-04-03 00:23:10.862280 catframes-2024.3.1/setup.cfg
+drwxr-sr-x   0 me        (1000) me        (1000)        0 2024-04-03 00:23:10.812279 catframes-2024.3.1/src/
+drwxr-sr-x   0 me        (1000) me        (1000)        0 2024-04-03 00:23:10.832279 catframes-2024.3.1/src/catframes/
+-rw-r--r--   0 me        (1000) me        (1000)       18 2023-09-24 19:02:05.000000 catframes-2024.3.1/src/catframes/__init__.py
+-rw-r--r--   0 me        (1000) me        (1000)   138208 2024-04-03 00:03:15.000000 catframes-2024.3.1/src/catframes/catframes.py
+drwxr-sr-x   0 me        (1000) me        (1000)        0 2024-04-03 00:23:10.862280 catframes-2024.3.1/src/catframes.egg-info/
+-rw-r--r--   0 me        (1000) me        (1000)     6311 2024-04-03 00:23:10.000000 catframes-2024.3.1/src/catframes.egg-info/PKG-INFO
+-rw-r--r--   0 me        (1000) me        (1000)      313 2024-04-03 00:23:10.000000 catframes-2024.3.1/src/catframes.egg-info/SOURCES.txt
+-rw-r--r--   0 me        (1000) me        (1000)        1 2024-04-03 00:23:10.000000 catframes-2024.3.1/src/catframes.egg-info/dependency_links.txt
+-rw-r--r--   0 me        (1000) me        (1000)       55 2024-04-03 00:23:10.000000 catframes-2024.3.1/src/catframes.egg-info/entry_points.txt
+-rw-r--r--   0 me        (1000) me        (1000)       14 2024-04-03 00:23:10.000000 catframes-2024.3.1/src/catframes.egg-info/requires.txt
+-rw-r--r--   0 me        (1000) me        (1000)       10 2024-04-03 00:23:10.000000 catframes-2024.3.1/src/catframes.egg-info/top_level.txt
```

### Comparing `catframes-2024.3.0/LICENSE.txt` & `catframes-2024.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `catframes-2024.3.0/PKG-INFO` & `catframes-2024.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catframes
-Version: 2024.3.0
+Version: 2024.3.1
 Summary: A handy tool for combining images into videos via FFmpeg.
 Author-email: Georgy Ustinov <inbox@itustinov.ru>
 License: © Устинов Г.М., 2022–2024
         
         This software is provided 'as-is', without any express or implied
         warranty.  In no event will the authors be held liable for any damages
         arising from the use of this software.
```

### Comparing `catframes-2024.3.0/README.md` & `catframes-2024.3.1/README.md`

 * *Files identical despite different names*

### Comparing `catframes-2024.3.0/pyproject.toml` & `catframes-2024.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "catframes"
-version = "2024.3.0"
+version = "2024.3.1"
 
 description = "A handy tool for combining images into videos via FFmpeg."
 
 readme = "README.md"
 license = {file = "LICENSE.txt"}
 
 requires-python = ">=3.7"
```

### Comparing `catframes-2024.3.0/src/catframes/catframes.py` & `catframes-2024.3.1/src/catframes/catframes.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 import http.client
 from time import sleep, monotonic
 from unittest import TestCase
 
 from PIL import Image, ImageColor, ImageDraw, ImageFont
 
 
-__version__ = '2024.3.0'
+__version__ = '2024.3.1'
 __license__ = 'Zlib'
 
 
 TITLE = f'Catframes {__version__}'
 
 DESCRIPTION = f"""{TITLE}
 
@@ -170,16 +170,16 @@
             httpd = make_server(host='', port=port, app=self._app)
             try:
                 web_thread = threading.Thread(target = httpd.serve_forever)
                 web_thread.daemon = True
                 web_thread.start()
                 self._do_the_job(port)
             finally:
-                # WSGIServer inherits this method from socketserver.BaseServer
-                httpd.shutdown()
+                httpd.shutdown()        # Exit loop.
+                httpd.server_close()    # Clean up the server.
 
             return True
         except OSError:
             return False
 
 
 class _JobServerTest(TestCase):
```

### Comparing `catframes-2024.3.0/src/catframes.egg-info/PKG-INFO` & `catframes-2024.3.1/src/catframes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catframes
-Version: 2024.3.0
+Version: 2024.3.1
 Summary: A handy tool for combining images into videos via FFmpeg.
 Author-email: Georgy Ustinov <inbox@itustinov.ru>
 License: © Устинов Г.М., 2022–2024
         
         This software is provided 'as-is', without any express or implied
         warranty.  In no event will the authors be held liable for any damages
         arising from the use of this software.
```

