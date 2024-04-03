# Comparing `tmp/alibabacloud_energyexpertexternal20220923_py2-1.0.0.tar.gz` & `tmp/alibabacloud_energyexpertexternal20220923_py2-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_energyexpertexternal20220923_py2-1.0.0.tar", last modified: Thu Jul 13 03:14:52 2023, max compression
+gzip compressed data, was "dist/alibabacloud_energyexpertexternal20220923_py2-1.1.0.tar", last modified: Wed Apr  3 17:08:43 2024, max compression
```

## Comparing `alibabacloud_energyexpertexternal20220923_py2-1.0.0.tar` & `alibabacloud_energyexpertexternal20220923_py2-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 03:14:52.000000 alibabacloud_energyexpertexternal20220923_py2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      588 2023-07-13 03:14:52.000000 alibabacloud_energyexpertexternal20220923_py2-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-07-13 03:14:52.000000 alibabacloud_energyexpertexternal20220923_py2-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2574 2023-07-13 03:14:52.000000 alibabacloud_energyexpertexternal20220923_py2-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1084 2023-07-13 03:14:52.000000 alibabacloud_energyexpertexternal20220923_py2-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1167 2023-07-13 03:14:52.000000 alibabacloud_energyexpertexternal20220923_py2-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 03:14:52.000000 alibabacloud_energyexpertexternal20220923_py2-1.0.0/alibabacloud_energyexpertexternal20220923/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-13 03:14:52.000000 alibabacloud_energyexpertexternal20220923_py2-1.0.0/alibabacloud_energyexpertexternal20220923/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4638 2023-07-13 03:14:52.000000 alibabacloud_energyexpertexternal20220923_py2-1.0.0/alibabacloud_energyexpertexternal20220923/client.py
--rw-r--r--   0 root         (0) root         (0)    23368 2023-07-13 03:14:52.000000 alibabacloud_energyexpertexternal20220923_py2-1.0.0/alibabacloud_energyexpertexternal20220923/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 03:14:52.000000 alibabacloud_energyexpertexternal20220923_py2-1.0.0/alibabacloud_energyexpertexternal20220923_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2574 2023-07-13 03:14:52.000000 alibabacloud_energyexpertexternal20220923_py2-1.0.0/alibabacloud_energyexpertexternal20220923_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      563 2023-07-13 03:14:52.000000 alibabacloud_energyexpertexternal20220923_py2-1.0.0/alibabacloud_energyexpertexternal20220923_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 03:14:52.000000 alibabacloud_energyexpertexternal20220923_py2-1.0.0/alibabacloud_energyexpertexternal20220923_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-07-13 03:14:52.000000 alibabacloud_energyexpertexternal20220923_py2-1.0.0/alibabacloud_energyexpertexternal20220923_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-07-13 03:14:52.000000 alibabacloud_energyexpertexternal20220923_py2-1.0.0/alibabacloud_energyexpertexternal20220923_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-13 03:14:52.000000 alibabacloud_energyexpertexternal20220923_py2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2988 2023-07-13 03:14:52.000000 alibabacloud_energyexpertexternal20220923_py2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:08:43.000000 alibabacloud_energyexpertexternal20220923_py2-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)       95 2024-04-03 17:08:43.000000 alibabacloud_energyexpertexternal20220923_py2-1.1.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-03 17:08:43.000000 alibabacloud_energyexpertexternal20220923_py2-1.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-03 17:08:43.000000 alibabacloud_energyexpertexternal20220923_py2-1.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2574 2024-04-03 17:08:43.000000 alibabacloud_energyexpertexternal20220923_py2-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1084 2024-04-03 17:08:43.000000 alibabacloud_energyexpertexternal20220923_py2-1.1.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1167 2024-04-03 17:08:43.000000 alibabacloud_energyexpertexternal20220923_py2-1.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:08:43.000000 alibabacloud_energyexpertexternal20220923_py2-1.1.0/alibabacloud_energyexpertexternal20220923/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-03 17:08:43.000000 alibabacloud_energyexpertexternal20220923_py2-1.1.0/alibabacloud_energyexpertexternal20220923/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42300 2024-04-03 17:08:43.000000 alibabacloud_energyexpertexternal20220923_py2-1.1.0/alibabacloud_energyexpertexternal20220923/client.py
+-rw-r--r--   0 root         (0) root         (0)   249356 2024-04-03 17:08:43.000000 alibabacloud_energyexpertexternal20220923_py2-1.1.0/alibabacloud_energyexpertexternal20220923/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:08:43.000000 alibabacloud_energyexpertexternal20220923_py2-1.1.0/alibabacloud_energyexpertexternal20220923_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2574 2024-04-03 17:08:43.000000 alibabacloud_energyexpertexternal20220923_py2-1.1.0/alibabacloud_energyexpertexternal20220923_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      576 2024-04-03 17:08:43.000000 alibabacloud_energyexpertexternal20220923_py2-1.1.0/alibabacloud_energyexpertexternal20220923_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 17:08:43.000000 alibabacloud_energyexpertexternal20220923_py2-1.1.0/alibabacloud_energyexpertexternal20220923_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-03 17:08:43.000000 alibabacloud_energyexpertexternal20220923_py2-1.1.0/alibabacloud_energyexpertexternal20220923_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2024-04-03 17:08:43.000000 alibabacloud_energyexpertexternal20220923_py2-1.1.0/alibabacloud_energyexpertexternal20220923_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-03 17:08:43.000000 alibabacloud_energyexpertexternal20220923_py2-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2988 2024-04-03 17:08:43.000000 alibabacloud_energyexpertexternal20220923_py2-1.1.0/setup.py
```

### Comparing `alibabacloud_energyexpertexternal20220923_py2-1.0.0/LICENSE` & `alibabacloud_energyexpertexternal20220923_py2-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_energyexpertexternal20220923_py2-1.0.0/PKG-INFO` & `alibabacloud_energyexpertexternal20220923_py2-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_energyexpertexternal20220923_py2
-Version: 1.0.0
+Version: 1.1.0
 Summary: Alibaba Cloud energyExpertExternal (20220923) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_energyexpertexternal20220923_py2-1.0.0/README-CN.md` & `alibabacloud_energyexpertexternal20220923_py2-1.1.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_energyexpertexternal20220923_py2-1.0.0/README.md` & `alibabacloud_energyexpertexternal20220923_py2-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_energyexpertexternal20220923_py2-1.0.0/alibabacloud_energyexpertexternal20220923_py2.egg-info/PKG-INFO` & `alibabacloud_energyexpertexternal20220923_py2-1.1.0/alibabacloud_energyexpertexternal20220923_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-energyexpertexternal20220923-py2
-Version: 1.0.0
+Version: 1.1.0
 Summary: Alibaba Cloud energyExpertExternal (20220923) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_energyexpertexternal20220923_py2-1.0.0/alibabacloud_energyexpertexternal20220923_py2.egg-info/SOURCES.txt` & `alibabacloud_energyexpertexternal20220923_py2-1.1.0/alibabacloud_energyexpertexternal20220923_py2.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+ChangeLog.md
 LICENSE
 MANIFEST.in
 README-CN.md
 README.md
 setup.cfg
 setup.py
 alibabacloud_energyexpertexternal20220923/__init__.py
```

### Comparing `alibabacloud_energyexpertexternal20220923_py2-1.0.0/setup.py` & `alibabacloud_energyexpertexternal20220923_py2-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,29 +21,29 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_energyexpertexternal20220923_py2.
 
-Created on 13/07/2023
+Created on 03/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_energyexpertexternal20220923"
 NAME = "alibabacloud_energyexpertexternal20220923_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud energyExpertExternal (20220923) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util_py2>=0.0.8, <1.0.0",
-    "alibabacloud_tea_openapi_py2>=0.1.6, <1.0.0",
+    "alibabacloud_tea_util_py2>=0.0.9, <1.0.0",
+    "alibabacloud_tea_openapi_py2>=0.1.8, <1.0.0",
     "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 
 if os.path.exists('./README.md'):
```

