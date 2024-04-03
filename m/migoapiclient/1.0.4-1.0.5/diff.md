# Comparing `tmp/migoapiclient-1.0.4.tar.gz` & `tmp/migoapiclient-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "migoapiclient-1.0.4.tar", last modified: Wed Apr  3 08:50:10 2024, max compression
+gzip compressed data, was "migoapiclient-1.0.5.tar", last modified: Wed Apr  3 08:54:19 2024, max compression
```

## Comparing `migoapiclient-1.0.4.tar` & `migoapiclient-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 08:50:10.758402 migoapiclient-1.0.4/
--rw-rw-rw-   0        0        0     3900 2024-04-03 08:50:10.758402 migoapiclient-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3288 2024-04-03 07:12:56.000000 migoapiclient-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 08:50:10.753846 migoapiclient-1.0.4/migoapiclient/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:07:00.000000 migoapiclient-1.0.4/migoapiclient/__init__.py
--rw-rw-rw-   0        0        0     9834 2024-04-03 08:48:29.000000 migoapiclient-1.0.4/migoapiclient/api_client.py
--rw-rw-rw-   0        0        0      986 2024-04-03 04:05:29.000000 migoapiclient-1.0.4/migoapiclient/file_manager.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:50:10.757395 migoapiclient-1.0.4/migoapiclient.egg-info/
--rw-rw-rw-   0        0        0     3900 2024-04-03 08:50:10.000000 migoapiclient-1.0.4/migoapiclient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2024-04-03 08:50:10.000000 migoapiclient-1.0.4/migoapiclient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 08:50:10.000000 migoapiclient-1.0.4/migoapiclient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-03 08:50:10.000000 migoapiclient-1.0.4/migoapiclient.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 08:50:10.758402 migoapiclient-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     3940 2024-04-03 08:50:05.000000 migoapiclient-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:50:10.756891 migoapiclient-1.0.4/src/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:01:08.000000 migoapiclient-1.0.4/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:54:19.931084 migoapiclient-1.0.5/
+-rw-rw-rw-   0        0        0     3900 2024-04-03 08:54:19.930084 migoapiclient-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3288 2024-04-03 07:12:56.000000 migoapiclient-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 08:54:19.926083 migoapiclient-1.0.5/migoapiclient/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:53:54.000000 migoapiclient-1.0.5/migoapiclient/__init__.py
+-rw-rw-rw-   0        0        0     9834 2024-04-03 08:53:54.000000 migoapiclient-1.0.5/migoapiclient/api_client.py
+-rw-rw-rw-   0        0        0      986 2024-04-03 08:53:54.000000 migoapiclient-1.0.5/migoapiclient/file_manager.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:54:19.929083 migoapiclient-1.0.5/migoapiclient.egg-info/
+-rw-rw-rw-   0        0        0     3900 2024-04-03 08:54:19.000000 migoapiclient-1.0.5/migoapiclient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2024-04-03 08:54:19.000000 migoapiclient-1.0.5/migoapiclient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 08:54:19.000000 migoapiclient-1.0.5/migoapiclient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-03 08:54:19.000000 migoapiclient-1.0.5/migoapiclient.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-03 08:54:19.931084 migoapiclient-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     3898 2024-04-03 08:52:10.000000 migoapiclient-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:54:19.929083 migoapiclient-1.0.5/src/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:01:08.000000 migoapiclient-1.0.5/src/__init__.py
```

### Comparing `migoapiclient-1.0.4/PKG-INFO` & `migoapiclient-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: migoapiclient
-Version: 1.0.4
+Version: 1.0.5
 Summary: 米果请求API客户端
 Home-page: https://github.com/me/myproject
 Author: pykira
 Author-email: 2920167524@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `migoapiclient-1.0.4/README.md` & `migoapiclient-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `migoapiclient-1.0.4/migoapiclient/api_client.py` & `migoapiclient-1.0.5/migoapiclient/api_client.py`

 * *Files identical despite different names*

### Comparing `migoapiclient-1.0.4/migoapiclient/file_manager.py` & `migoapiclient-1.0.5/migoapiclient/file_manager.py`

 * *Files identical despite different names*

### Comparing `migoapiclient-1.0.4/migoapiclient.egg-info/PKG-INFO` & `migoapiclient-1.0.5/migoapiclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: migoapiclient
-Version: 1.0.4
+Version: 1.0.5
 Summary: 米果请求API客户端
 Home-page: https://github.com/me/myproject
 Author: pykira
 Author-email: 2920167524@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `migoapiclient-1.0.4/setup.py` & `migoapiclient-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'migoapiclient'
 DESCRIPTION = '米果请求API客户端'
 URL = 'https://github.com/me/myproject'
 EMAIL = '2920167524@qq.com'
 AUTHOR = 'pykira'
 REQUIRES_PYTHON = '>=3.5.0'
-VERSION = input('请输入程序版本，例如：1.0.3\n')
+VERSION = '1.0.5'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

