# Comparing `tmp/trustauthx-0.6.5.tar.gz` & `tmp/trustauthx-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trustauthx-0.6.5.tar", last modified: Wed Apr  3 17:04:43 2024, max compression
+gzip compressed data, was "trustauthx-0.6.6.tar", last modified: Wed Apr  3 17:40:35 2024, max compression
```

## Comparing `trustauthx-0.6.5.tar` & `trustauthx-0.6.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:04:43.182959 trustauthx-0.6.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-03 17:04:34.000000 trustauthx-0.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10024 2024-04-03 17:04:43.182959 trustauthx-0.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9100 2024-04-03 17:04:34.000000 trustauthx-0.6.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 17:04:43.182959 trustauthx-0.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-03 17:04:34.000000 trustauthx-0.6.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:04:43.178959 trustauthx-0.6.5/test/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-03 17:04:34.000000 trustauthx-0.6.5/test/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:04:43.178959 trustauthx-0.6.5/trustauthx/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 17:04:34.000000 trustauthx-0.6.5/trustauthx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32857 2024-04-03 17:04:34.000000 trustauthx-0.6.5/trustauthx/authlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-04-03 17:04:34.000000 trustauthx-0.6.5/trustauthx/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-04-03 17:04:34.000000 trustauthx-0.6.5/trustauthx/llmai.py
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-03 17:04:34.000000 trustauthx-0.6.5/trustauthx/scheme.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:04:43.182959 trustauthx-0.6.5/trustauthx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10024 2024-04-03 17:04:43.000000 trustauthx-0.6.5/trustauthx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-03 17:04:43.000000 trustauthx-0.6.5/trustauthx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 17:04:43.000000 trustauthx-0.6.5/trustauthx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-03 17:04:43.000000 trustauthx-0.6.5/trustauthx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-03 17:04:43.000000 trustauthx-0.6.5/trustauthx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 17:04:43.000000 trustauthx-0.6.5/trustauthx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:40:35.773429 trustauthx-0.6.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-03 17:40:26.000000 trustauthx-0.6.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10024 2024-04-03 17:40:35.773429 trustauthx-0.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9100 2024-04-03 17:40:26.000000 trustauthx-0.6.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 17:40:35.773429 trustauthx-0.6.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-03 17:40:26.000000 trustauthx-0.6.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:40:35.769429 trustauthx-0.6.6/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-03 17:40:26.000000 trustauthx-0.6.6/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:40:35.769429 trustauthx-0.6.6/trustauthx/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 17:40:26.000000 trustauthx-0.6.6/trustauthx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32888 2024-04-03 17:40:26.000000 trustauthx-0.6.6/trustauthx/authlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-04-03 17:40:26.000000 trustauthx-0.6.6/trustauthx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-04-03 17:40:26.000000 trustauthx-0.6.6/trustauthx/llmai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-03 17:40:26.000000 trustauthx-0.6.6/trustauthx/scheme.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:40:35.769429 trustauthx-0.6.6/trustauthx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10024 2024-04-03 17:40:35.000000 trustauthx-0.6.6/trustauthx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-03 17:40:35.000000 trustauthx-0.6.6/trustauthx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 17:40:35.000000 trustauthx-0.6.6/trustauthx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-03 17:40:35.000000 trustauthx-0.6.6/trustauthx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-03 17:40:35.000000 trustauthx-0.6.6/trustauthx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 17:40:35.000000 trustauthx-0.6.6/trustauthx.egg-info/top_level.txt
```

### Comparing `trustauthx-0.6.5/LICENSE` & `trustauthx-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `trustauthx-0.6.5/PKG-INFO` & `trustauthx-0.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trustauthx
-Version: 0.6.5
+Version: 0.6.6
 Summary: Official connector SDK for TrustAuthx
 Home-page: https://github.com/One-Click-Auth/TrustAuthx-Py-SDK.git
 Author: moonlightnexus
 Author-email: nexus@trustauthx.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `trustauthx-0.6.5/README.md` & `trustauthx-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `trustauthx-0.6.5/setup.py` & `trustauthx-0.6.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='trustauthx',
-    version='0.6.5',
+    version='0.6.6',
     description='Official connector SDK for TrustAuthx',
     long_description=long_description,
     long_description_content_type='text/markdown',  # This is important!
     author='moonlightnexus',
     author_email='nexus@trustauthx.com',
     url="https://github.com/One-Click-Auth/TrustAuthx-Py-SDK.git",
     license="MIT",
```

### Comparing `trustauthx-0.6.5/trustauthx/authlite.py` & `trustauthx-0.6.6/trustauthx/authlite.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,16 +151,17 @@
     def _EDGE_Wrapper(func):
         @wraps(func)
         def wrapper(*args, **kwargs):
             # Call the function
             response = func(*args, **kwargs)
             # Check for "X-EDGE"
             x_edge = response.headers.get("X-EDGE")
-            if int(x_edge) != _EdgeDBRoleQuery.total_roles:
-                _EdgeDBRoleQuery.reinitialize_all() # Add data
+            if x_edge:
+                if int(x_edge) != _EdgeDBRoleQuery.total_roles:
+                    _EdgeDBRoleQuery.reinitialize_all() # Add data
             return response
         return wrapper
 
 requests.get = _EdgeDBRoleQuery._EDGE_Wrapper(requests.get)
 requests.post = _EdgeDBRoleQuery._EDGE_Wrapper(requests.post)
 requests.delete = _EdgeDBRoleQuery._EDGE_Wrapper(requests.delete)
```

### Comparing `trustauthx-0.6.5/trustauthx/cli.py` & `trustauthx-0.6.6/trustauthx/cli.py`

 * *Files identical despite different names*

### Comparing `trustauthx-0.6.5/trustauthx/llmai.py` & `trustauthx-0.6.6/trustauthx/llmai.py`

 * *Files identical despite different names*

### Comparing `trustauthx-0.6.5/trustauthx/scheme.py` & `trustauthx-0.6.6/trustauthx/scheme.py`

 * *Files identical despite different names*

### Comparing `trustauthx-0.6.5/trustauthx.egg-info/PKG-INFO` & `trustauthx-0.6.6/trustauthx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trustauthx
-Version: 0.6.5
+Version: 0.6.6
 Summary: Official connector SDK for TrustAuthx
 Home-page: https://github.com/One-Click-Auth/TrustAuthx-Py-SDK.git
 Author: moonlightnexus
 Author-email: nexus@trustauthx.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

