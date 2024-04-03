# Comparing `tmp/trustauthx-0.6.7.tar.gz` & `tmp/trustauthx-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trustauthx-0.6.7.tar", last modified: Wed Apr  3 18:14:27 2024, max compression
+gzip compressed data, was "trustauthx-0.6.8.tar", last modified: Wed Apr  3 18:15:04 2024, max compression
```

## Comparing `trustauthx-0.6.7.tar` & `trustauthx-0.6.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:14:27.336525 trustauthx-0.6.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-03 18:14:17.000000 trustauthx-0.6.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10024 2024-04-03 18:14:27.336525 trustauthx-0.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9100 2024-04-03 18:14:17.000000 trustauthx-0.6.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 18:14:27.336525 trustauthx-0.6.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-03 18:14:17.000000 trustauthx-0.6.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:14:27.332525 trustauthx-0.6.7/test/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-03 18:14:17.000000 trustauthx-0.6.7/test/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:14:27.336525 trustauthx-0.6.7/trustauthx/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 18:14:17.000000 trustauthx-0.6.7/trustauthx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32888 2024-04-03 18:14:17.000000 trustauthx-0.6.7/trustauthx/authlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-04-03 18:14:17.000000 trustauthx-0.6.7/trustauthx/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-04-03 18:14:17.000000 trustauthx-0.6.7/trustauthx/llmai.py
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-03 18:14:17.000000 trustauthx-0.6.7/trustauthx/scheme.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:14:27.336525 trustauthx-0.6.7/trustauthx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10024 2024-04-03 18:14:27.000000 trustauthx-0.6.7/trustauthx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-03 18:14:27.000000 trustauthx-0.6.7/trustauthx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 18:14:27.000000 trustauthx-0.6.7/trustauthx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-03 18:14:27.000000 trustauthx-0.6.7/trustauthx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-03 18:14:27.000000 trustauthx-0.6.7/trustauthx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 18:14:27.000000 trustauthx-0.6.7/trustauthx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:15:04.752955 trustauthx-0.6.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-03 18:14:53.000000 trustauthx-0.6.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10024 2024-04-03 18:15:04.752955 trustauthx-0.6.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9100 2024-04-03 18:14:53.000000 trustauthx-0.6.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 18:15:04.752955 trustauthx-0.6.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-03 18:14:53.000000 trustauthx-0.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:15:04.748955 trustauthx-0.6.8/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-03 18:14:53.000000 trustauthx-0.6.8/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:15:04.752955 trustauthx-0.6.8/trustauthx/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 18:14:53.000000 trustauthx-0.6.8/trustauthx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32888 2024-04-03 18:14:53.000000 trustauthx-0.6.8/trustauthx/authlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-04-03 18:14:53.000000 trustauthx-0.6.8/trustauthx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-04-03 18:14:53.000000 trustauthx-0.6.8/trustauthx/llmai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-03 18:14:53.000000 trustauthx-0.6.8/trustauthx/scheme.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:15:04.752955 trustauthx-0.6.8/trustauthx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10024 2024-04-03 18:15:04.000000 trustauthx-0.6.8/trustauthx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-03 18:15:04.000000 trustauthx-0.6.8/trustauthx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 18:15:04.000000 trustauthx-0.6.8/trustauthx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-03 18:15:04.000000 trustauthx-0.6.8/trustauthx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-03 18:15:04.000000 trustauthx-0.6.8/trustauthx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 18:15:04.000000 trustauthx-0.6.8/trustauthx.egg-info/top_level.txt
```

### Comparing `trustauthx-0.6.7/LICENSE` & `trustauthx-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `trustauthx-0.6.7/PKG-INFO` & `trustauthx-0.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trustauthx
-Version: 0.6.7
+Version: 0.6.8
 Summary: Official connector SDK for TrustAuthx
 Home-page: https://github.com/One-Click-Auth/TrustAuthx-Py-SDK.git
 Author: moonlightnexus
 Author-email: nexus@trustauthx.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `trustauthx-0.6.7/README.md` & `trustauthx-0.6.8/README.md`

 * *Files identical despite different names*

### Comparing `trustauthx-0.6.7/setup.py` & `trustauthx-0.6.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='trustauthx',
-    version='0.6.7',
+    version='0.6.8',
     description='Official connector SDK for TrustAuthx',
     long_description=long_description,
     long_description_content_type='text/markdown',  # This is important!
     author='moonlightnexus',
     author_email='nexus@trustauthx.com',
     url="https://github.com/One-Click-Auth/TrustAuthx-Py-SDK.git",
     license="MIT",
```

### Comparing `trustauthx-0.6.7/trustauthx/authlite.py` & `trustauthx-0.6.8/trustauthx/authlite.py`

 * *Files identical despite different names*

### Comparing `trustauthx-0.6.7/trustauthx/cli.py` & `trustauthx-0.6.8/trustauthx/cli.py`

 * *Files identical despite different names*

### Comparing `trustauthx-0.6.7/trustauthx/llmai.py` & `trustauthx-0.6.8/trustauthx/llmai.py`

 * *Files identical despite different names*

### Comparing `trustauthx-0.6.7/trustauthx/scheme.py` & `trustauthx-0.6.8/trustauthx/scheme.py`

 * *Files identical despite different names*

### Comparing `trustauthx-0.6.7/trustauthx.egg-info/PKG-INFO` & `trustauthx-0.6.8/trustauthx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trustauthx
-Version: 0.6.7
+Version: 0.6.8
 Summary: Official connector SDK for TrustAuthx
 Home-page: https://github.com/One-Click-Auth/TrustAuthx-Py-SDK.git
 Author: moonlightnexus
 Author-email: nexus@trustauthx.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

