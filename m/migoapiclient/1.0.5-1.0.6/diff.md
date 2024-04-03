# Comparing `tmp/migoapiclient-1.0.5.tar.gz` & `tmp/migoapiclient-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "migoapiclient-1.0.5.tar", last modified: Wed Apr  3 08:54:19 2024, max compression
+gzip compressed data, was "migoapiclient-1.0.6.tar", last modified: Wed Apr  3 09:05:39 2024, max compression
```

## Comparing `migoapiclient-1.0.5.tar` & `migoapiclient-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 08:54:19.931084 migoapiclient-1.0.5/
--rw-rw-rw-   0        0        0     3900 2024-04-03 08:54:19.930084 migoapiclient-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3288 2024-04-03 07:12:56.000000 migoapiclient-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 08:54:19.926083 migoapiclient-1.0.5/migoapiclient/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:53:54.000000 migoapiclient-1.0.5/migoapiclient/__init__.py
--rw-rw-rw-   0        0        0     9834 2024-04-03 08:53:54.000000 migoapiclient-1.0.5/migoapiclient/api_client.py
--rw-rw-rw-   0        0        0      986 2024-04-03 08:53:54.000000 migoapiclient-1.0.5/migoapiclient/file_manager.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:54:19.929083 migoapiclient-1.0.5/migoapiclient.egg-info/
--rw-rw-rw-   0        0        0     3900 2024-04-03 08:54:19.000000 migoapiclient-1.0.5/migoapiclient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2024-04-03 08:54:19.000000 migoapiclient-1.0.5/migoapiclient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 08:54:19.000000 migoapiclient-1.0.5/migoapiclient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-03 08:54:19.000000 migoapiclient-1.0.5/migoapiclient.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 08:54:19.931084 migoapiclient-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     3898 2024-04-03 08:52:10.000000 migoapiclient-1.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:54:19.929083 migoapiclient-1.0.5/src/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:01:08.000000 migoapiclient-1.0.5/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 09:05:39.435269 migoapiclient-1.0.6/
+-rw-rw-rw-   0        0        0     3900 2024-04-03 09:05:39.434264 migoapiclient-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3288 2024-04-03 07:12:56.000000 migoapiclient-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 09:05:39.430766 migoapiclient-1.0.6/migoapiclient/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:53:54.000000 migoapiclient-1.0.6/migoapiclient/__init__.py
+-rw-rw-rw-   0        0        0     9835 2024-04-03 09:05:26.000000 migoapiclient-1.0.6/migoapiclient/api_client.py
+-rw-rw-rw-   0        0        0      986 2024-04-03 08:53:54.000000 migoapiclient-1.0.6/migoapiclient/file_manager.py
+drwxrwxrwx   0        0        0        0 2024-04-03 09:05:39.434264 migoapiclient-1.0.6/migoapiclient.egg-info/
+-rw-rw-rw-   0        0        0     3900 2024-04-03 09:05:39.000000 migoapiclient-1.0.6/migoapiclient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2024-04-03 09:05:39.000000 migoapiclient-1.0.6/migoapiclient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 09:05:39.000000 migoapiclient-1.0.6/migoapiclient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-03 09:05:39.000000 migoapiclient-1.0.6/migoapiclient.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-03 09:05:39.435269 migoapiclient-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     3898 2024-04-03 09:05:36.000000 migoapiclient-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 09:05:39.433760 migoapiclient-1.0.6/src/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:01:08.000000 migoapiclient-1.0.6/src/__init__.py
```

### Comparing `migoapiclient-1.0.5/PKG-INFO` & `migoapiclient-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: migoapiclient
-Version: 1.0.5
+Version: 1.0.6
 Summary: 米果请求API客户端
 Home-page: https://github.com/me/myproject
 Author: pykira
 Author-email: 2920167524@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `migoapiclient-1.0.5/README.md` & `migoapiclient-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `migoapiclient-1.0.5/migoapiclient/api_client.py` & `migoapiclient-1.0.6/migoapiclient/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 from datetime import datetime
 
 from dateutil.tz import tz
 
-from file_manager import LogFileManager
+from .file_manager import LogFileManager
 import time
 import requests
 
 ERROR_MSG = """
 ---------------------------------- {0} begin ----------------------------------
 请求URL是：{1}
 请求headers是：{2}
```

### Comparing `migoapiclient-1.0.5/migoapiclient/file_manager.py` & `migoapiclient-1.0.6/migoapiclient/file_manager.py`

 * *Files identical despite different names*

### Comparing `migoapiclient-1.0.5/migoapiclient.egg-info/PKG-INFO` & `migoapiclient-1.0.6/migoapiclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: migoapiclient
-Version: 1.0.5
+Version: 1.0.6
 Summary: 米果请求API客户端
 Home-page: https://github.com/me/myproject
 Author: pykira
 Author-email: 2920167524@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `migoapiclient-1.0.5/setup.py` & `migoapiclient-1.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'migoapiclient'
 DESCRIPTION = '米果请求API客户端'
 URL = 'https://github.com/me/myproject'
 EMAIL = '2920167524@qq.com'
 AUTHOR = 'pykira'
 REQUIRES_PYTHON = '>=3.5.0'
-VERSION = '1.0.5'
+VERSION = '1.0.6'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

