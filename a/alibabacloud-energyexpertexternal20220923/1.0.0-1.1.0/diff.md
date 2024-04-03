# Comparing `tmp/alibabacloud_energyexpertexternal20220923-1.0.0.tar.gz` & `tmp/alibabacloud_energyexpertexternal20220923-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_energyexpertexternal20220923-1.0.0.tar", last modified: Thu Jul 13 03:15:27 2023, max compression
+gzip compressed data, was "dist/alibabacloud_energyexpertexternal20220923-1.1.0.tar", last modified: Wed Apr  3 17:09:36 2024, max compression
```

## Comparing `alibabacloud_energyexpertexternal20220923-1.0.0.tar` & `alibabacloud_energyexpertexternal20220923-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 03:15:27.000000 alibabacloud_energyexpertexternal20220923-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      600 2023-07-13 03:15:27.000000 alibabacloud_energyexpertexternal20220923-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-13 03:15:27.000000 alibabacloud_energyexpertexternal20220923-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2430 2023-07-13 03:15:27.000000 alibabacloud_energyexpertexternal20220923-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1073 2023-07-13 03:15:27.000000 alibabacloud_energyexpertexternal20220923-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1158 2023-07-13 03:15:27.000000 alibabacloud_energyexpertexternal20220923-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 03:15:27.000000 alibabacloud_energyexpertexternal20220923-1.0.0/alibabacloud_energyexpertexternal20220923/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-13 03:15:27.000000 alibabacloud_energyexpertexternal20220923-1.0.0/alibabacloud_energyexpertexternal20220923/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9956 2023-07-13 03:15:27.000000 alibabacloud_energyexpertexternal20220923-1.0.0/alibabacloud_energyexpertexternal20220923/client.py
--rw-r--r--   0 root         (0) root         (0)    23303 2023-07-13 03:15:27.000000 alibabacloud_energyexpertexternal20220923-1.0.0/alibabacloud_energyexpertexternal20220923/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 03:15:27.000000 alibabacloud_energyexpertexternal20220923-1.0.0/alibabacloud_energyexpertexternal20220923.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2430 2023-07-13 03:15:27.000000 alibabacloud_energyexpertexternal20220923-1.0.0/alibabacloud_energyexpertexternal20220923.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      543 2023-07-13 03:15:27.000000 alibabacloud_energyexpertexternal20220923-1.0.0/alibabacloud_energyexpertexternal20220923.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 03:15:27.000000 alibabacloud_energyexpertexternal20220923-1.0.0/alibabacloud_energyexpertexternal20220923.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-07-13 03:15:27.000000 alibabacloud_energyexpertexternal20220923-1.0.0/alibabacloud_energyexpertexternal20220923.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-07-13 03:15:27.000000 alibabacloud_energyexpertexternal20220923-1.0.0/alibabacloud_energyexpertexternal20220923.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-13 03:15:27.000000 alibabacloud_energyexpertexternal20220923-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2695 2023-07-13 03:15:27.000000 alibabacloud_energyexpertexternal20220923-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:09:36.000000 alibabacloud_energyexpertexternal20220923-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)       95 2024-04-03 17:09:36.000000 alibabacloud_energyexpertexternal20220923-1.1.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-03 17:09:36.000000 alibabacloud_energyexpertexternal20220923-1.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-03 17:09:36.000000 alibabacloud_energyexpertexternal20220923-1.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2520 2024-04-03 17:09:36.000000 alibabacloud_energyexpertexternal20220923-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1163 2024-04-03 17:09:36.000000 alibabacloud_energyexpertexternal20220923-1.1.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1248 2024-04-03 17:09:36.000000 alibabacloud_energyexpertexternal20220923-1.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:09:36.000000 alibabacloud_energyexpertexternal20220923-1.1.0/alibabacloud_energyexpertexternal20220923/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-03 17:09:36.000000 alibabacloud_energyexpertexternal20220923-1.1.0/alibabacloud_energyexpertexternal20220923/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   105062 2024-04-03 17:09:36.000000 alibabacloud_energyexpertexternal20220923-1.1.0/alibabacloud_energyexpertexternal20220923/client.py
+-rw-r--r--   0 root         (0) root         (0)   247948 2024-04-03 17:09:36.000000 alibabacloud_energyexpertexternal20220923-1.1.0/alibabacloud_energyexpertexternal20220923/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:09:36.000000 alibabacloud_energyexpertexternal20220923-1.1.0/alibabacloud_energyexpertexternal20220923.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2520 2024-04-03 17:09:36.000000 alibabacloud_energyexpertexternal20220923-1.1.0/alibabacloud_energyexpertexternal20220923.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      556 2024-04-03 17:09:36.000000 alibabacloud_energyexpertexternal20220923-1.1.0/alibabacloud_energyexpertexternal20220923.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 17:09:36.000000 alibabacloud_energyexpertexternal20220923-1.1.0/alibabacloud_energyexpertexternal20220923.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-03 17:09:36.000000 alibabacloud_energyexpertexternal20220923-1.1.0/alibabacloud_energyexpertexternal20220923.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2024-04-03 17:09:36.000000 alibabacloud_energyexpertexternal20220923-1.1.0/alibabacloud_energyexpertexternal20220923.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-03 17:09:36.000000 alibabacloud_energyexpertexternal20220923-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2696 2024-04-03 17:09:36.000000 alibabacloud_energyexpertexternal20220923-1.1.0/setup.py
```

### Comparing `alibabacloud_energyexpertexternal20220923-1.0.0/LICENSE` & `alibabacloud_energyexpertexternal20220923-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_energyexpertexternal20220923-1.0.0/PKG-INFO` & `alibabacloud_energyexpertexternal20220923-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_energyexpertexternal20220923
-Version: 1.0.0
+Version: 1.1.0
 Summary: Alibaba Cloud energyExpertExternal (20220923) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
@@ -32,15 +32,15 @@
         
         ## Usage
         
         [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
         
         ## Changelog
         
-        Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/energyexpertexternal-20220923/ChangeLog.md).
         
         ## References
         
         - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
         
         ## License
```

### Comparing `alibabacloud_energyexpertexternal20220923-1.0.0/README-CN.md` & `alibabacloud_energyexpertexternal20220923-1.1.0/README-CN.md`

 * *Files 14% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 ## 使用说明
 
 [快速使用](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-CN.md#%E5%BF%AB%E9%80%9F%E4%BD%BF%E7%94%A8)
 
 ## 发行说明
 
-每个版本的详细更改记录在[发行说明](./ChangeLog.md)中。
+每个版本的详细更改记录在[发行说明](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/energyexpertexternal-20220923/ChangeLog.md)中。
 
 ## 相关
 
 - [最新源码](https://github.com/aliyun/alibabacloud-python-sdk/)
 
 ## 许可证
```

### Comparing `alibabacloud_energyexpertexternal20220923-1.0.0/README.md` & `alibabacloud_energyexpertexternal20220923-1.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 ## Usage
 
 [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
 
 ## Changelog
 
-Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/energyexpertexternal-20220923/ChangeLog.md).
 
 ## References
 
 - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
 
 ## License
```

### Comparing `alibabacloud_energyexpertexternal20220923-1.0.0/alibabacloud_energyexpertexternal20220923.egg-info/PKG-INFO` & `alibabacloud_energyexpertexternal20220923-1.1.0/alibabacloud_energyexpertexternal20220923.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-energyexpertexternal20220923
-Version: 1.0.0
+Version: 1.1.0
 Summary: Alibaba Cloud energyExpertExternal (20220923) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
@@ -32,15 +32,15 @@
         
         ## Usage
         
         [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
         
         ## Changelog
         
-        Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/energyexpertexternal-20220923/ChangeLog.md).
         
         ## References
         
         - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
         
         ## License
```

### Comparing `alibabacloud_energyexpertexternal20220923-1.0.0/alibabacloud_energyexpertexternal20220923.egg-info/SOURCES.txt` & `alibabacloud_energyexpertexternal20220923-1.1.0/alibabacloud_energyexpertexternal20220923.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

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

### Comparing `alibabacloud_energyexpertexternal20220923-1.0.0/setup.py` & `alibabacloud_energyexpertexternal20220923-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_energyexpertexternal20220923.
 
-Created on 13/07/2023
+Created on 03/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_energyexpertexternal20220923"
 NAME = "alibabacloud_energyexpertexternal20220923" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud energyExpertExternal (20220923) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.9, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
+    "alibabacloud_tea_util>=0.3.11, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.8, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
```

