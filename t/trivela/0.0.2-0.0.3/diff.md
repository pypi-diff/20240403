# Comparing `tmp/trivela-0.0.2.tar.gz` & `tmp/trivela-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trivela-0.0.2.tar", last modified: Wed Apr  3 15:39:14 2024, max compression
+gzip compressed data, was "trivela-0.0.3.tar", last modified: Wed Apr  3 15:47:55 2024, max compression
```

## Comparing `trivela-0.0.2.tar` & `trivela-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 sanjayarai  (1000) sanjayarai  (1000)        0 2024-04-03 15:39:14.158609 trivela-0.0.2/
--rw-r--r--   0 sanjayarai  (1000) sanjayarai  (1000)     4004 2024-04-03 15:39:14.158609 trivela-0.0.2/PKG-INFO
--rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)     3507 2024-04-03 15:38:46.000000 trivela-0.0.2/README.md
--rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)       38 2024-04-03 15:39:14.158609 trivela-0.0.2/setup.cfg
--rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)     1657 2024-04-03 15:39:00.000000 trivela-0.0.2/setup.py
-drwxrwxr-x   0 sanjayarai  (1000) sanjayarai  (1000)        0 2024-04-03 15:39:14.154609 trivela-0.0.2/trivela/
--rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)        1 2024-03-27 16:31:23.000000 trivela-0.0.2/trivela/__init__.py
--rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)     5301 2024-04-03 14:39:41.000000 trivela-0.0.2/trivela/api.py
--rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)      673 2024-03-27 01:46:38.000000 trivela-0.0.2/trivela/middleware.py
--rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)      953 2024-01-03 14:20:30.000000 trivela-0.0.2/trivela/response.py
-drwxrwxr-x   0 sanjayarai  (1000) sanjayarai  (1000)        0 2024-04-03 15:39:14.158609 trivela-0.0.2/trivela.egg-info/
--rw-r--r--   0 sanjayarai  (1000) sanjayarai  (1000)     4004 2024-04-03 15:39:14.000000 trivela-0.0.2/trivela.egg-info/PKG-INFO
--rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)      249 2024-04-03 15:39:14.000000 trivela-0.0.2/trivela.egg-info/SOURCES.txt
--rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)        1 2024-04-03 15:39:14.000000 trivela-0.0.2/trivela.egg-info/dependency_links.txt
--rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)      104 2024-04-03 15:39:14.000000 trivela-0.0.2/trivela.egg-info/requires.txt
--rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)        8 2024-04-03 15:39:14.000000 trivela-0.0.2/trivela.egg-info/top_level.txt
+drwxrwxr-x   0 sanjayarai  (1000) sanjayarai  (1000)        0 2024-04-03 15:47:55.872951 trivela-0.0.3/
+-rw-r--r--   0 sanjayarai  (1000) sanjayarai  (1000)     3991 2024-04-03 15:47:55.872951 trivela-0.0.3/PKG-INFO
+-rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)     3494 2024-04-03 15:47:30.000000 trivela-0.0.3/README.md
+-rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)       38 2024-04-03 15:47:55.872951 trivela-0.0.3/setup.cfg
+-rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)     1657 2024-04-03 15:43:28.000000 trivela-0.0.3/setup.py
+drwxrwxr-x   0 sanjayarai  (1000) sanjayarai  (1000)        0 2024-04-03 15:47:55.872951 trivela-0.0.3/trivela/
+-rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)        1 2024-03-27 16:31:23.000000 trivela-0.0.3/trivela/__init__.py
+-rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)     5301 2024-04-03 14:39:41.000000 trivela-0.0.3/trivela/api.py
+-rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)      673 2024-03-27 01:46:38.000000 trivela-0.0.3/trivela/middleware.py
+-rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)      953 2024-01-03 14:20:30.000000 trivela-0.0.3/trivela/response.py
+drwxrwxr-x   0 sanjayarai  (1000) sanjayarai  (1000)        0 2024-04-03 15:47:55.872951 trivela-0.0.3/trivela.egg-info/
+-rw-r--r--   0 sanjayarai  (1000) sanjayarai  (1000)     3991 2024-04-03 15:47:55.000000 trivela-0.0.3/trivela.egg-info/PKG-INFO
+-rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)      249 2024-04-03 15:47:55.000000 trivela-0.0.3/trivela.egg-info/SOURCES.txt
+-rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)        1 2024-04-03 15:47:55.000000 trivela-0.0.3/trivela.egg-info/dependency_links.txt
+-rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)      104 2024-04-03 15:47:55.000000 trivela-0.0.3/trivela.egg-info/requires.txt
+-rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)        8 2024-04-03 15:47:55.000000 trivela-0.0.3/trivela.egg-info/top_level.txt
```

### Comparing `trivela-0.0.2/PKG-INFO` & `trivela-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trivela
-Version: 0.0.2
+Version: 0.0.3
 Summary: Trivela Python Web Framework build for learning purpose.
 Author: Sanjaya Rai
 Author-email: rainamite@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.12.0
 Description-Content-Type: text/markdown
@@ -14,16 +14,16 @@
 Requires-Dist: requests-wsgi-adapter==0.4.1
 Requires-Dist: WebOb==1.8.7
 Requires-Dist: whitenoise==4.1.4
 
 
 # Trivela: Python Web Framework built for learning purposes
 
-![purpose](https://img.shields.io/badge/any_text-you_like-blue)
-![PyPI](https://img.shields.io/badge/just%20the%20message-8A2BE2)
+![purpose](https://img.shields.io/badge/learining-purpose-blue)
+![PyPI](https://img.shields.io/badge/Trivela-8A2BE2)
 
 Trivela is a Python web framework build for learning purposes.
 
 It's a WSGI framework and can be used with any WSGI application server such as Gunicorn.
 
 ## Installation
 ```shell
```

### Comparing `trivela-0.0.2/README.md` & `trivela-0.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Trivela: Python Web Framework built for learning purposes
 
-![purpose](https://img.shields.io/badge/any_text-you_like-blue)
-![PyPI](https://img.shields.io/badge/just%20the%20message-8A2BE2)
+![purpose](https://img.shields.io/badge/learining-purpose-blue)
+![PyPI](https://img.shields.io/badge/Trivela-8A2BE2)
 
 Trivela is a Python web framework build for learning purposes.
 
 It's a WSGI framework and can be used with any WSGI application server such as Gunicorn.
 
 ## Installation
 ```shell
```

### Comparing `trivela-0.0.2/setup.py` & `trivela-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # package meta-data
 NAME = "trivela"
 DESCRIPTION = "Trivela Python Web Framework build for learning purpose."
 EMAIL = "rainamite@gmail.com"
 AUTHOR = "Sanjaya Rai"
 REQUIRES_PYTHON = ">=3.12.0"
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 
 # which packages are required for this module to be executed?
 REQUIRED = [
     "Jinja==3.1.2",
     "parse==1.20.0",
     "requests==2.31.0",
     "requests-wsgi-adapter==0.4.1",
```

### Comparing `trivela-0.0.2/trivela/api.py` & `trivela-0.0.3/trivela/api.py`

 * *Files identical despite different names*

### Comparing `trivela-0.0.2/trivela/middleware.py` & `trivela-0.0.3/trivela/middleware.py`

 * *Files identical despite different names*

### Comparing `trivela-0.0.2/trivela/response.py` & `trivela-0.0.3/trivela/response.py`

 * *Files identical despite different names*

### Comparing `trivela-0.0.2/trivela.egg-info/PKG-INFO` & `trivela-0.0.3/trivela.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trivela
-Version: 0.0.2
+Version: 0.0.3
 Summary: Trivela Python Web Framework build for learning purpose.
 Author: Sanjaya Rai
 Author-email: rainamite@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.12.0
 Description-Content-Type: text/markdown
@@ -14,16 +14,16 @@
 Requires-Dist: requests-wsgi-adapter==0.4.1
 Requires-Dist: WebOb==1.8.7
 Requires-Dist: whitenoise==4.1.4
 
 
 # Trivela: Python Web Framework built for learning purposes
 
-![purpose](https://img.shields.io/badge/any_text-you_like-blue)
-![PyPI](https://img.shields.io/badge/just%20the%20message-8A2BE2)
+![purpose](https://img.shields.io/badge/learining-purpose-blue)
+![PyPI](https://img.shields.io/badge/Trivela-8A2BE2)
 
 Trivela is a Python web framework build for learning purposes.
 
 It's a WSGI framework and can be used with any WSGI application server such as Gunicorn.
 
 ## Installation
 ```shell
```

