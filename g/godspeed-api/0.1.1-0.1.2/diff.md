# Comparing `tmp/godspeed_api-0.1.1.tar.gz` & `tmp/godspeed_api-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "godspeed_api-0.1.1.tar", last modified: Wed Apr  3 14:44:02 2024, max compression
+gzip compressed data, was "godspeed_api-0.1.2.tar", last modified: Wed Apr  3 14:46:32 2024, max compression
```

## Comparing `godspeed_api-0.1.1.tar` & `godspeed_api-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:44:02.658239 godspeed_api-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-03 14:43:58.000000 godspeed_api-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-03 14:44:02.658239 godspeed_api-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-03 14:43:58.000000 godspeed_api-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:44:02.658239 godspeed_api-0.1.1/godspeed_api/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-03 14:43:58.000000 godspeed_api-0.1.1/godspeed_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-03 14:43:58.000000 godspeed_api-0.1.1/godspeed_api/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:44:02.658239 godspeed_api-0.1.1/godspeed_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-03 14:44:02.000000 godspeed_api-0.1.1/godspeed_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-03 14:44:02.000000 godspeed_api-0.1.1/godspeed_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 14:44:02.000000 godspeed_api-0.1.1/godspeed_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 14:44:02.000000 godspeed_api-0.1.1/godspeed_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 14:44:02.000000 godspeed_api-0.1.1/godspeed_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 14:44:02.658239 godspeed_api-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-03 14:43:58.000000 godspeed_api-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:46:32.580023 godspeed_api-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-03 14:46:28.000000 godspeed_api-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-03 14:46:32.580023 godspeed_api-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-03 14:46:28.000000 godspeed_api-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:46:32.580023 godspeed_api-0.1.2/godspeed_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-03 14:46:28.000000 godspeed_api-0.1.2/godspeed_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-03 14:46:28.000000 godspeed_api-0.1.2/godspeed_api/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:46:32.580023 godspeed_api-0.1.2/godspeed_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-03 14:46:32.000000 godspeed_api-0.1.2/godspeed_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-03 14:46:32.000000 godspeed_api-0.1.2/godspeed_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 14:46:32.000000 godspeed_api-0.1.2/godspeed_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 14:46:32.000000 godspeed_api-0.1.2/godspeed_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 14:46:32.000000 godspeed_api-0.1.2/godspeed_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 14:46:32.580023 godspeed_api-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-03 14:46:28.000000 godspeed_api-0.1.2/setup.py
```

### Comparing `godspeed_api-0.1.1/LICENSE` & `godspeed_api-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `godspeed_api-0.1.1/PKG-INFO` & `godspeed_api-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: godspeed_api
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Godspeed task manager API wrapper
 Author: Artem Trubacheev
 Author-email: almaz5200@gmail.com
 Keywords: python,godspeed
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `godspeed_api-0.1.1/godspeed_api/api.py` & `godspeed_api-0.1.2/godspeed_api/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     def __init__(
         self,
         username: str,
         password: str,
         hostname: str = "https://api.godspeedapp.com/",
     ):
         self.hostname = hostname
+        self.token = None
 
         try:
             auth_result = self._send_post_request(
                 "/auth/login",
                 {
                     "username": username,
                     "password": password,
```

### Comparing `godspeed_api-0.1.1/godspeed_api.egg-info/PKG-INFO` & `godspeed_api-0.1.2/godspeed_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: godspeed_api
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Godspeed task manager API wrapper
 Author: Artem Trubacheev
 Author-email: almaz5200@gmail.com
 Keywords: python,godspeed
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `godspeed_api-0.1.1/setup.py` & `godspeed_api-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.1.1"
+VERSION = "0.1.2"
 DESCRIPTION = "A Godspeed task manager API wrapper"
 
 setup(
     name="godspeed_api",
     version=VERSION,
     author="Artem Trubacheev",
     author_email="almaz5200@gmail.com",
```

