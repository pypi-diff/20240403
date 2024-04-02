# Comparing `tmp/nectarclient-lib-1.2.0.tar.gz` & `tmp/nectarclient-lib-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nectarclient-lib-1.2.0.tar", last modified: Fri Mar  1 05:17:03 2024, max compression
+gzip compressed data, was "nectarclient-lib-1.3.0.tar", last modified: Thu Mar 28 02:56:35 2024, max compression
```

## Comparing `nectarclient-lib-1.2.0.tar` & `nectarclient-lib-1.3.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-01 05:17:03.000000 nectarclient-lib-1.2.0/
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-01 05:17:03.000000 nectarclient-lib-1.2.0/nectarclient_lib.egg-info/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      423 2024-03-01 05:17:02.000000 nectarclient-lib-1.2.0/nectarclient_lib.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       20 2024-03-01 05:17:02.000000 nectarclient-lib-1.2.0/nectarclient_lib.egg-info/requires.txt
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        1 2024-03-01 05:17:02.000000 nectarclient-lib-1.2.0/nectarclient_lib.egg-info/not-zip-safe
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      680 2024-03-01 05:17:02.000000 nectarclient-lib-1.2.0/nectarclient_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       17 2024-03-01 05:17:02.000000 nectarclient-lib-1.2.0/nectarclient_lib.egg-info/top_level.txt
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        1 2024-03-01 05:17:02.000000 nectarclient-lib-1.2.0/nectarclient_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1279 2024-03-01 05:16:55.000000 nectarclient-lib-1.2.0/setup.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      134 2024-03-01 05:16:55.000000 nectarclient-lib-1.2.0/MANIFEST.in
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      423 2024-03-01 05:17:03.000000 nectarclient-lib-1.2.0/PKG-INFO
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       81 2024-03-01 05:16:55.000000 nectarclient-lib-1.2.0/README.md
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       61 2024-03-01 05:17:03.000000 nectarclient-lib-1.2.0/setup.cfg
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-01 05:17:03.000000 nectarclient-lib-1.2.0/nectarclient_lib/
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-01 05:17:03.000000 nectarclient-lib-1.2.0/nectarclient_lib/osc/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1476 2024-03-01 05:16:55.000000 nectarclient-lib-1.2.0/nectarclient_lib/osc/utils.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2024-03-01 05:16:55.000000 nectarclient-lib-1.2.0/nectarclient_lib/osc/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15694 2024-03-01 05:16:55.000000 nectarclient-lib-1.2.0/nectarclient_lib/base.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5462 2024-03-01 05:16:55.000000 nectarclient-lib-1.2.0/nectarclient_lib/exceptions.py
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-01 05:17:03.000000 nectarclient-lib-1.2.0/nectarclient_lib/tests/
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-01 05:17:03.000000 nectarclient-lib-1.2.0/nectarclient_lib/tests/unit/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5935 2024-03-01 05:16:55.000000 nectarclient-lib-1.2.0/nectarclient_lib/tests/unit/test_base.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1148 2024-03-01 05:16:55.000000 nectarclient-lib-1.2.0/nectarclient_lib/tests/unit/test_exceptions.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3132 2024-03-01 05:16:55.000000 nectarclient-lib-1.2.0/nectarclient_lib/tests/unit/utils.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6548 2024-03-01 05:16:55.000000 nectarclient-lib-1.2.0/nectarclient_lib/tests/unit/fakes.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2024-03-01 05:16:55.000000 nectarclient-lib-1.2.0/nectarclient_lib/tests/unit/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2024-03-01 05:16:55.000000 nectarclient-lib-1.2.0/nectarclient_lib/tests/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2024-03-01 05:16:55.000000 nectarclient-lib-1.2.0/nectarclient_lib/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       20 2024-03-01 05:16:55.000000 nectarclient-lib-1.2.0/requirements.txt
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2024-03-28 02:56:35.010579 nectarclient-lib-1.3.0/
+-rw-rw-r--   0 sam       (1000) sam       (1000)    10143 2023-12-13 22:55:35.000000 nectarclient-lib-1.3.0/LICENSE
+-rw-rw-r--   0 sam       (1000) sam       (1000)      134 2023-12-13 22:55:35.000000 nectarclient-lib-1.3.0/MANIFEST.in
+-rw-rw-r--   0 sam       (1000) sam       (1000)      434 2024-03-28 02:56:35.010579 nectarclient-lib-1.3.0/PKG-INFO
+-rw-rw-r--   0 sam       (1000) sam       (1000)       81 2023-12-13 22:55:35.000000 nectarclient-lib-1.3.0/README.md
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2024-03-28 02:56:35.006579 nectarclient-lib-1.3.0/nectarclient_lib/
+-rw-rw-r--   0 sam       (1000) sam       (1000)        0 2023-12-13 22:55:35.000000 nectarclient-lib-1.3.0/nectarclient_lib/__init__.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)    15779 2024-03-28 02:45:12.000000 nectarclient-lib-1.3.0/nectarclient_lib/base.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     5462 2023-12-13 22:55:35.000000 nectarclient-lib-1.3.0/nectarclient_lib/exceptions.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2024-03-28 02:56:35.006579 nectarclient-lib-1.3.0/nectarclient_lib/osc/
+-rw-rw-r--   0 sam       (1000) sam       (1000)        0 2023-12-13 22:55:35.000000 nectarclient-lib-1.3.0/nectarclient_lib/osc/__init__.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1476 2023-12-13 22:55:35.000000 nectarclient-lib-1.3.0/nectarclient_lib/osc/utils.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2024-03-28 02:56:35.006579 nectarclient-lib-1.3.0/nectarclient_lib/tests/
+-rw-rw-r--   0 sam       (1000) sam       (1000)        0 2023-12-13 22:55:35.000000 nectarclient-lib-1.3.0/nectarclient_lib/tests/__init__.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2024-03-28 02:56:35.010579 nectarclient-lib-1.3.0/nectarclient_lib/tests/unit/
+-rw-rw-r--   0 sam       (1000) sam       (1000)        0 2023-12-13 22:55:35.000000 nectarclient-lib-1.3.0/nectarclient_lib/tests/unit/__init__.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     6548 2023-12-13 22:55:35.000000 nectarclient-lib-1.3.0/nectarclient_lib/tests/unit/fakes.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     5935 2023-12-13 23:45:59.000000 nectarclient-lib-1.3.0/nectarclient_lib/tests/unit/test_base.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1148 2023-12-13 22:55:35.000000 nectarclient-lib-1.3.0/nectarclient_lib/tests/unit/test_exceptions.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     3132 2023-12-13 22:55:35.000000 nectarclient-lib-1.3.0/nectarclient_lib/tests/unit/utils.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2024-03-28 02:56:35.006579 nectarclient-lib-1.3.0/nectarclient_lib.egg-info/
+-rw-rw-r--   0 sam       (1000) sam       (1000)      434 2024-03-28 02:56:35.000000 nectarclient-lib-1.3.0/nectarclient_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 sam       (1000) sam       (1000)      688 2024-03-28 02:56:35.000000 nectarclient-lib-1.3.0/nectarclient_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)        1 2024-03-28 02:56:35.000000 nectarclient-lib-1.3.0/nectarclient_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)        1 2023-11-09 00:03:28.000000 nectarclient-lib-1.3.0/nectarclient_lib.egg-info/not-zip-safe
+-rw-rw-r--   0 sam       (1000) sam       (1000)       20 2024-03-28 02:56:35.000000 nectarclient-lib-1.3.0/nectarclient_lib.egg-info/requires.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)       17 2024-03-28 02:56:35.000000 nectarclient-lib-1.3.0/nectarclient_lib.egg-info/top_level.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)       20 2023-12-13 22:55:35.000000 nectarclient-lib-1.3.0/requirements.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)       61 2024-03-28 02:56:35.010579 nectarclient-lib-1.3.0/setup.cfg
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1279 2024-03-28 02:45:12.000000 nectarclient-lib-1.3.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `nectarclient-lib-1.2.0/nectarclient_lib.egg-info/SOURCES.txt` & `nectarclient-lib-1.3.0/nectarclient_lib.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.cfg
 setup.py
 nectarclient_lib/__init__.py
 nectarclient_lib/base.py
```

### Comparing `nectarclient-lib-1.2.0/setup.py` & `nectarclient-lib-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 import setuptools
 
 from pbr.packaging import parse_requirements
 
 setuptools.setup(
     name='nectarclient-lib',
-    version='1.2.0',
+    version='1.3.0',
     description=('Common lib for nectar clients'),
     author='Sam Morrison',
     author_email='sorrison@gmail.com',
     url='https://github.com/NeCTAR-RC/nectarclient-lib',
     packages=[
         'nectarclient_lib',
     ],
```

### Comparing `nectarclient-lib-1.2.0/nectarclient_lib/osc/utils.py` & `nectarclient-lib-1.3.0/nectarclient_lib/osc/utils.py`

 * *Files identical despite different names*

### Comparing `nectarclient-lib-1.2.0/nectarclient_lib/base.py` & `nectarclient-lib-1.3.0/nectarclient_lib/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,14 +181,16 @@
     def _search(self, url, data, response_key='results', obj_class=None,
               items=None, headers=None, limit=None):
 
         if items is None:
             items = []
         if headers is None:
             headers = {}
+        headers["Content-Type"] = "application/json"
+        data = json.dumps(data)
         resp, body = self.api.post(url, headers=headers, data=data)
 
         if obj_class is None:
             obj_class = self.resource_class
 
         if response_key and response_key in body:
             data = body[response_key]
```

### Comparing `nectarclient-lib-1.2.0/nectarclient_lib/exceptions.py` & `nectarclient-lib-1.3.0/nectarclient_lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `nectarclient-lib-1.2.0/nectarclient_lib/tests/unit/test_base.py` & `nectarclient-lib-1.3.0/nectarclient_lib/tests/unit/test_base.py`

 * *Files identical despite different names*

### Comparing `nectarclient-lib-1.2.0/nectarclient_lib/tests/unit/test_exceptions.py` & `nectarclient-lib-1.3.0/nectarclient_lib/tests/unit/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `nectarclient-lib-1.2.0/nectarclient_lib/tests/unit/utils.py` & `nectarclient-lib-1.3.0/nectarclient_lib/tests/unit/utils.py`

 * *Files identical despite different names*

### Comparing `nectarclient-lib-1.2.0/nectarclient_lib/tests/unit/fakes.py` & `nectarclient-lib-1.3.0/nectarclient_lib/tests/unit/fakes.py`

 * *Files identical despite different names*

