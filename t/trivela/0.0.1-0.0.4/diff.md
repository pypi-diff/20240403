# Comparing `tmp/trivela-0.0.1.tar.gz` & `tmp/trivela-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trivela-0.0.1.tar", last modified: Wed Apr  3 15:15:15 2024, max compression
+gzip compressed data, was "trivela-0.0.4.tar", last modified: Wed Apr  3 16:00:18 2024, max compression
```

## Comparing `trivela-0.0.1.tar` & `trivela-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 sanjayarai  (1000) sanjayarai  (1000)        0 2024-04-03 15:15:15.971215 trivela-0.0.1/
--rw-r--r--   0 sanjayarai  (1000) sanjayarai  (1000)      503 2024-04-03 15:15:15.971215 trivela-0.0.1/PKG-INFO
--rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)        6 2023-12-29 03:43:11.000000 trivela-0.0.1/README.md
--rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)       38 2024-04-03 15:15:15.971215 trivela-0.0.1/setup.cfg
--rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)     1657 2024-04-03 15:12:02.000000 trivela-0.0.1/setup.py
-drwxrwxr-x   0 sanjayarai  (1000) sanjayarai  (1000)        0 2024-04-03 15:15:15.971215 trivela-0.0.1/trivela/
--rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)        1 2024-03-27 16:31:23.000000 trivela-0.0.1/trivela/__init__.py
--rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)     5301 2024-04-03 14:39:41.000000 trivela-0.0.1/trivela/api.py
--rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)      673 2024-03-27 01:46:38.000000 trivela-0.0.1/trivela/middleware.py
--rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)      953 2024-01-03 14:20:30.000000 trivela-0.0.1/trivela/response.py
-drwxrwxr-x   0 sanjayarai  (1000) sanjayarai  (1000)        0 2024-04-03 15:15:15.971215 trivela-0.0.1/trivela.egg-info/
--rw-r--r--   0 sanjayarai  (1000) sanjayarai  (1000)      503 2024-04-03 15:15:15.000000 trivela-0.0.1/trivela.egg-info/PKG-INFO
--rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)      249 2024-04-03 15:15:15.000000 trivela-0.0.1/trivela.egg-info/SOURCES.txt
--rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)        1 2024-04-03 15:15:15.000000 trivela-0.0.1/trivela.egg-info/dependency_links.txt
--rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)      104 2024-04-03 15:15:15.000000 trivela-0.0.1/trivela.egg-info/requires.txt
--rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)        8 2024-04-03 15:15:15.000000 trivela-0.0.1/trivela.egg-info/top_level.txt
+drwxrwxr-x   0 sanjayarai  (1000) sanjayarai  (1000)        0 2024-04-03 16:00:17.994573 trivela-0.0.4/
+-rw-r--r--   0 sanjayarai  (1000) sanjayarai  (1000)     3999 2024-04-03 16:00:17.994573 trivela-0.0.4/PKG-INFO
+-rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)     3502 2024-04-03 15:59:30.000000 trivela-0.0.4/README.md
+-rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)       38 2024-04-03 16:00:17.994573 trivela-0.0.4/setup.cfg
+-rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)     1657 2024-04-03 15:59:41.000000 trivela-0.0.4/setup.py
+drwxrwxr-x   0 sanjayarai  (1000) sanjayarai  (1000)        0 2024-04-03 16:00:17.994573 trivela-0.0.4/trivela/
+-rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)        1 2024-03-27 16:31:23.000000 trivela-0.0.4/trivela/__init__.py
+-rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)     5301 2024-04-03 14:39:41.000000 trivela-0.0.4/trivela/api.py
+-rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)      673 2024-03-27 01:46:38.000000 trivela-0.0.4/trivela/middleware.py
+-rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)      953 2024-01-03 14:20:30.000000 trivela-0.0.4/trivela/response.py
+drwxrwxr-x   0 sanjayarai  (1000) sanjayarai  (1000)        0 2024-04-03 16:00:17.994573 trivela-0.0.4/trivela.egg-info/
+-rw-r--r--   0 sanjayarai  (1000) sanjayarai  (1000)     3999 2024-04-03 16:00:17.000000 trivela-0.0.4/trivela.egg-info/PKG-INFO
+-rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)      249 2024-04-03 16:00:17.000000 trivela-0.0.4/trivela.egg-info/SOURCES.txt
+-rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)        1 2024-04-03 16:00:17.000000 trivela-0.0.4/trivela.egg-info/dependency_links.txt
+-rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)      104 2024-04-03 16:00:17.000000 trivela-0.0.4/trivela.egg-info/requires.txt
+-rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)        8 2024-04-03 16:00:17.000000 trivela-0.0.4/trivela.egg-info/top_level.txt
```

### Comparing `trivela-0.0.1/setup.py` & `trivela-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # package meta-data
 NAME = "trivela"
 DESCRIPTION = "Trivela Python Web Framework build for learning purpose."
 EMAIL = "rainamite@gmail.com"
 AUTHOR = "Sanjaya Rai"
 REQUIRES_PYTHON = ">=3.12.0"
-VERSION = "0.0.1"
+VERSION = "0.0.4"
 
 # which packages are required for this module to be executed?
 REQUIRED = [
     "Jinja==3.1.2",
     "parse==1.20.0",
     "requests==2.31.0",
     "requests-wsgi-adapter==0.4.1",
```

### Comparing `trivela-0.0.1/trivela/api.py` & `trivela-0.0.4/trivela/api.py`

 * *Files identical despite different names*

### Comparing `trivela-0.0.1/trivela/middleware.py` & `trivela-0.0.4/trivela/middleware.py`

 * *Files identical despite different names*

### Comparing `trivela-0.0.1/trivela/response.py` & `trivela-0.0.4/trivela/response.py`

 * *Files identical despite different names*

