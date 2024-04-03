# Comparing `tmp/cloudstructs-0.9.1.tar.gz` & `tmp/cloudstructs-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudstructs-0.9.1.tar", last modified: Mon Mar 18 14:18:34 2024, max compression
+gzip compressed data, was "cloudstructs-0.9.2.tar", last modified: Wed Apr  3 09:52:49 2024, max compression
```

## Comparing `cloudstructs-0.9.1.tar` & `cloudstructs-0.9.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:18:34.781565 cloudstructs-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-18 14:18:23.000000 cloudstructs-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-18 14:18:23.000000 cloudstructs-0.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-03-18 14:18:34.781565 cloudstructs-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-03-18 14:18:23.000000 cloudstructs-0.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-18 14:18:23.000000 cloudstructs-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 14:18:34.781565 cloudstructs-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-03-18 14:18:23.000000 cloudstructs-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:18:34.777565 cloudstructs-0.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:18:34.777565 cloudstructs-0.9.1/src/cloudstructs/
--rw-r--r--   0 runner    (1001) docker     (127)   181069 2024-03-18 14:18:23.000000 cloudstructs-0.9.1/src/cloudstructs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:18:34.777565 cloudstructs-0.9.1/src/cloudstructs/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-03-18 14:18:23.000000 cloudstructs-0.9.1/src/cloudstructs/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  3194805 2024-03-18 14:18:23.000000 cloudstructs-0.9.1/src/cloudstructs/_jsii/cloudstructs@0.9.1.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 14:18:23.000000 cloudstructs-0.9.1/src/cloudstructs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:18:34.777565 cloudstructs-0.9.1/src/cloudstructs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-03-18 14:18:34.000000 cloudstructs-0.9.1/src/cloudstructs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-03-18 14:18:34.000000 cloudstructs-0.9.1/src/cloudstructs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 14:18:34.000000 cloudstructs-0.9.1/src/cloudstructs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-18 14:18:34.000000 cloudstructs-0.9.1/src/cloudstructs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-18 14:18:34.000000 cloudstructs-0.9.1/src/cloudstructs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:52:49.427351 cloudstructs-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-03 09:52:35.000000 cloudstructs-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-03 09:52:35.000000 cloudstructs-0.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-03 09:52:49.427351 cloudstructs-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-03 09:52:35.000000 cloudstructs-0.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-03 09:52:35.000000 cloudstructs-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 09:52:49.427351 cloudstructs-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-03 09:52:35.000000 cloudstructs-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:52:49.419351 cloudstructs-0.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:52:49.423351 cloudstructs-0.9.2/src/cloudstructs/
+-rw-r--r--   0 runner    (1001) docker     (127)   181145 2024-04-03 09:52:35.000000 cloudstructs-0.9.2/src/cloudstructs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:52:49.423351 cloudstructs-0.9.2/src/cloudstructs/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-03 09:52:35.000000 cloudstructs-0.9.2/src/cloudstructs/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  3235187 2024-04-03 09:52:35.000000 cloudstructs-0.9.2/src/cloudstructs/_jsii/cloudstructs@0.9.2.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 09:52:35.000000 cloudstructs-0.9.2/src/cloudstructs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:52:49.423351 cloudstructs-0.9.2/src/cloudstructs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-03 09:52:49.000000 cloudstructs-0.9.2/src/cloudstructs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-03 09:52:49.000000 cloudstructs-0.9.2/src/cloudstructs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 09:52:49.000000 cloudstructs-0.9.2/src/cloudstructs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-03 09:52:49.000000 cloudstructs-0.9.2/src/cloudstructs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 09:52:49.000000 cloudstructs-0.9.2/src/cloudstructs.egg-info/top_level.txt
```

### Comparing `cloudstructs-0.9.1/LICENSE` & `cloudstructs-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudstructs-0.9.1/PKG-INFO` & `cloudstructs-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudstructs
-Version: 0.9.1
+Version: 0.9.2
 Summary: High-level constructs for AWS CDK
 Home-page: https://github.com/jogold/cloudstructs.git
 Author: Jonathan Goldwasser<jonathan.goldwasser@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/jogold/cloudstructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudstructs-0.9.1/README.md` & `cloudstructs-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `cloudstructs-0.9.1/setup.py` & `cloudstructs-0.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cloudstructs",
-    "version": "0.9.1",
+    "version": "0.9.2",
     "description": "High-level constructs for AWS CDK",
     "license": "Apache-2.0",
     "url": "https://github.com/jogold/cloudstructs.git",
     "long_description_content_type": "text/markdown",
     "author": "Jonathan Goldwasser<jonathan.goldwasser@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "cloudstructs",
         "cloudstructs._jsii"
     ],
     "package_data": {
         "cloudstructs._jsii": [
-            "cloudstructs@0.9.1.jsii.tgz"
+            "cloudstructs@0.9.2.jsii.tgz"
         ],
         "cloudstructs": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
         "aws-cdk-lib>=2.133.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.95.0, <2.0.0",
+        "jsii>=1.96.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cloudstructs-0.9.1/src/cloudstructs/__init__.py` & `cloudstructs-0.9.2/src/cloudstructs/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,17 @@
 * [`StaticWebsite`](src/static-website) A CloudFront static website hosted on S3 with
   HTTPS redirect, SPA redirect, HTTP security headers and backend configuration saved
   to the bucket.
 * [`ToolkitCleaner`](src/toolkit-cleaner) Clean unused S3 and ECR assets from your CDK
   Toolkit.
 * [`UrlShortener`](src/url-shortener) Deploy an URL shortener API
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
```

### Comparing `cloudstructs-0.9.1/src/cloudstructs.egg-info/PKG-INFO` & `cloudstructs-0.9.2/src/cloudstructs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudstructs
-Version: 0.9.1
+Version: 0.9.2
 Summary: High-level constructs for AWS CDK
 Home-page: https://github.com/jogold/cloudstructs.git
 Author: Jonathan Goldwasser<jonathan.goldwasser@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/jogold/cloudstructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

