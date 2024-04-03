# Comparing `tmp/pypeeringmanager-1.1.0.tar.gz` & `tmp/pypeeringmanager-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypeeringmanager-1.1.0.tar", last modified: Thu Jan 18 10:54:02 2024, max compression
+gzip compressed data, was "pypeeringmanager-1.1.1.tar", last modified: Wed Apr  3 11:33:38 2024, max compression
```

## Comparing `pypeeringmanager-1.1.0.tar` & `pypeeringmanager-1.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 vista     (1000) vista     (1000)        0 2024-01-18 10:54:02.754434 pypeeringmanager-1.1.0/
--rw-r--r--   0 vista     (1000) vista     (1000)     9612 2024-01-18 10:30:37.000000 pypeeringmanager-1.1.0/LICENSE
--rw-r--r--   0 vista     (1000) vista     (1000)      903 2024-01-18 10:54:02.754434 pypeeringmanager-1.1.0/PKG-INFO
--rw-r--r--   0 vista     (1000) vista     (1000)      280 2024-01-18 10:45:27.000000 pypeeringmanager-1.1.0/README.md
--rw-r--r--   0 vista     (1000) vista     (1000)      104 2024-01-18 10:30:37.000000 pypeeringmanager-1.1.0/pyproject.toml
--rw-r--r--   0 vista     (1000) vista     (1000)      729 2024-01-18 10:54:02.755434 pypeeringmanager-1.1.0/setup.cfg
-drwxr-xr-x   0 vista     (1000) vista     (1000)        0 2024-01-18 10:54:02.751434 pypeeringmanager-1.1.0/src/
-drwxr-xr-x   0 vista     (1000) vista     (1000)        0 2024-01-18 10:54:02.752434 pypeeringmanager-1.1.0/src/pypeeringmanager/
--rw-r--r--   0 vista     (1000) vista     (1000)      288 2024-01-18 10:30:37.000000 pypeeringmanager-1.1.0/src/pypeeringmanager/__init__.py
-drwxr-xr-x   0 vista     (1000) vista     (1000)        0 2024-01-18 10:54:02.753434 pypeeringmanager-1.1.0/src/pypeeringmanager/core/
--rw-r--r--   0 vista     (1000) vista     (1000)        0 2024-01-18 10:30:37.000000 pypeeringmanager-1.1.0/src/pypeeringmanager/core/__init__.py
--rw-r--r--   0 vista     (1000) vista     (1000)     2267 2024-01-18 10:33:04.000000 pypeeringmanager-1.1.0/src/pypeeringmanager/core/api.py
--rw-r--r--   0 vista     (1000) vista     (1000)      487 2024-01-18 10:33:35.000000 pypeeringmanager-1.1.0/src/pypeeringmanager/core/app.py
-drwxr-xr-x   0 vista     (1000) vista     (1000)        0 2024-01-18 10:54:02.753434 pypeeringmanager-1.1.0/src/pypeeringmanager/models/
--rw-r--r--   0 vista     (1000) vista     (1000)        0 2024-01-18 10:30:37.000000 pypeeringmanager-1.1.0/src/pypeeringmanager/models/__init__.py
--rw-r--r--   0 vista     (1000) vista     (1000)      229 2024-01-18 10:31:52.000000 pypeeringmanager-1.1.0/src/pypeeringmanager/models/extras.py
--rw-r--r--   0 vista     (1000) vista     (1000)      211 2024-01-18 10:31:27.000000 pypeeringmanager-1.1.0/src/pypeeringmanager/models/net.py
--rw-r--r--   0 vista     (1000) vista     (1000)     1053 2024-01-18 10:30:37.000000 pypeeringmanager-1.1.0/src/pypeeringmanager/models/peering.py
-drwxr-xr-x   0 vista     (1000) vista     (1000)        0 2024-01-18 10:54:02.754434 pypeeringmanager-1.1.0/src/pypeeringmanager.egg-info/
--rw-r--r--   0 vista     (1000) vista     (1000)      903 2024-01-18 10:54:02.000000 pypeeringmanager-1.1.0/src/pypeeringmanager.egg-info/PKG-INFO
--rw-r--r--   0 vista     (1000) vista     (1000)      550 2024-01-18 10:54:02.000000 pypeeringmanager-1.1.0/src/pypeeringmanager.egg-info/SOURCES.txt
--rw-r--r--   0 vista     (1000) vista     (1000)        1 2024-01-18 10:54:02.000000 pypeeringmanager-1.1.0/src/pypeeringmanager.egg-info/dependency_links.txt
--rw-r--r--   0 vista     (1000) vista     (1000)       16 2024-01-18 10:54:02.000000 pypeeringmanager-1.1.0/src/pypeeringmanager.egg-info/requires.txt
--rw-r--r--   0 vista     (1000) vista     (1000)       17 2024-01-18 10:54:02.000000 pypeeringmanager-1.1.0/src/pypeeringmanager.egg-info/top_level.txt
+drwxr-xr-x   0 vista     (1000) vista     (1000)        0 2024-04-03 11:33:38.668393 pypeeringmanager-1.1.1/
+-rw-r--r--   0 vista     (1000) vista     (1000)     9612 2024-01-18 10:30:37.000000 pypeeringmanager-1.1.1/LICENSE
+-rw-r--r--   0 vista     (1000) vista     (1000)      903 2024-04-03 11:33:38.668393 pypeeringmanager-1.1.1/PKG-INFO
+-rw-r--r--   0 vista     (1000) vista     (1000)      280 2024-01-18 10:45:27.000000 pypeeringmanager-1.1.1/README.md
+-rw-r--r--   0 vista     (1000) vista     (1000)      104 2024-01-18 10:30:37.000000 pypeeringmanager-1.1.1/pyproject.toml
+-rw-r--r--   0 vista     (1000) vista     (1000)      729 2024-04-03 11:33:38.672393 pypeeringmanager-1.1.1/setup.cfg
+drwxr-xr-x   0 vista     (1000) vista     (1000)        0 2024-04-03 11:33:38.664393 pypeeringmanager-1.1.1/src/
+drwxr-xr-x   0 vista     (1000) vista     (1000)        0 2024-04-03 11:33:38.665393 pypeeringmanager-1.1.1/src/pypeeringmanager/
+-rw-r--r--   0 vista     (1000) vista     (1000)      288 2024-01-18 10:30:37.000000 pypeeringmanager-1.1.1/src/pypeeringmanager/__init__.py
+drwxr-xr-x   0 vista     (1000) vista     (1000)        0 2024-04-03 11:33:38.667393 pypeeringmanager-1.1.1/src/pypeeringmanager/core/
+-rw-r--r--   0 vista     (1000) vista     (1000)        0 2024-01-18 10:30:37.000000 pypeeringmanager-1.1.1/src/pypeeringmanager/core/__init__.py
+-rw-r--r--   0 vista     (1000) vista     (1000)     2267 2024-01-18 10:33:04.000000 pypeeringmanager-1.1.1/src/pypeeringmanager/core/api.py
+-rw-r--r--   0 vista     (1000) vista     (1000)      614 2024-04-03 11:30:14.000000 pypeeringmanager-1.1.1/src/pypeeringmanager/core/app.py
+drwxr-xr-x   0 vista     (1000) vista     (1000)        0 2024-04-03 11:33:38.667393 pypeeringmanager-1.1.1/src/pypeeringmanager/models/
+-rw-r--r--   0 vista     (1000) vista     (1000)        0 2024-01-18 10:30:37.000000 pypeeringmanager-1.1.1/src/pypeeringmanager/models/__init__.py
+-rw-r--r--   0 vista     (1000) vista     (1000)      229 2024-01-18 10:31:52.000000 pypeeringmanager-1.1.1/src/pypeeringmanager/models/extras.py
+-rw-r--r--   0 vista     (1000) vista     (1000)      211 2024-01-18 10:31:27.000000 pypeeringmanager-1.1.1/src/pypeeringmanager/models/net.py
+-rw-r--r--   0 vista     (1000) vista     (1000)     1053 2024-01-18 10:30:37.000000 pypeeringmanager-1.1.1/src/pypeeringmanager/models/peering.py
+drwxr-xr-x   0 vista     (1000) vista     (1000)        0 2024-04-03 11:33:38.667393 pypeeringmanager-1.1.1/src/pypeeringmanager.egg-info/
+-rw-r--r--   0 vista     (1000) vista     (1000)      903 2024-04-03 11:33:38.000000 pypeeringmanager-1.1.1/src/pypeeringmanager.egg-info/PKG-INFO
+-rw-r--r--   0 vista     (1000) vista     (1000)      550 2024-04-03 11:33:38.000000 pypeeringmanager-1.1.1/src/pypeeringmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 vista     (1000) vista     (1000)        1 2024-04-03 11:33:38.000000 pypeeringmanager-1.1.1/src/pypeeringmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 vista     (1000) vista     (1000)       16 2024-04-03 11:33:38.000000 pypeeringmanager-1.1.1/src/pypeeringmanager.egg-info/requires.txt
+-rw-r--r--   0 vista     (1000) vista     (1000)       17 2024-04-03 11:33:38.000000 pypeeringmanager-1.1.1/src/pypeeringmanager.egg-info/top_level.txt
```

### Comparing `pypeeringmanager-1.1.0/LICENSE` & `pypeeringmanager-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pypeeringmanager-1.1.0/PKG-INFO` & `pypeeringmanager-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypeeringmanager
-Version: 1.1.0
+Version: 1.1.1
 Summary: Peering-Manager API client library
 Home-page: https://github.com/vista-/pypeeringmanager
 Author: vista
 Author-email: vista@birb.network
 License: Apache2
 Keywords: peering-manager,peeringmanager,network-automation
 Classifier: Intended Audience :: Developers
```

### Comparing `pypeeringmanager-1.1.0/setup.cfg` & `pypeeringmanager-1.1.1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pypeeringmanager
-version = 1.1.0
+version = 1.1.1
 author = vista
 author_email = vista@birb.network
 description = Peering-Manager API client library
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Apache2
 url = https://github.com/vista-/pypeeringmanager
```

### Comparing `pypeeringmanager-1.1.0/src/pypeeringmanager/core/api.py` & `pypeeringmanager-1.1.1/src/pypeeringmanager/core/api.py`

 * *Files identical despite different names*

### Comparing `pypeeringmanager-1.1.0/src/pypeeringmanager/models/peering.py` & `pypeeringmanager-1.1.1/src/pypeeringmanager/models/peering.py`

 * *Files identical despite different names*

### Comparing `pypeeringmanager-1.1.0/src/pypeeringmanager.egg-info/PKG-INFO` & `pypeeringmanager-1.1.1/src/pypeeringmanager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypeeringmanager
-Version: 1.1.0
+Version: 1.1.1
 Summary: Peering-Manager API client library
 Home-page: https://github.com/vista-/pypeeringmanager
 Author: vista
 Author-email: vista@birb.network
 License: Apache2
 Keywords: peering-manager,peeringmanager,network-automation
 Classifier: Intended Audience :: Developers
```

### Comparing `pypeeringmanager-1.1.0/src/pypeeringmanager.egg-info/SOURCES.txt` & `pypeeringmanager-1.1.1/src/pypeeringmanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

