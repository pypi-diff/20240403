# Comparing `tmp/a3exception-0.1.3.tar.gz` & `tmp/a3exception-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "a3exception-0.1.3.tar", last modified: Tue Mar 26 02:46:29 2024, max compression
+gzip compressed data, was "a3exception-0.1.4.tar", last modified: Wed Apr  3 06:06:39 2024, max compression
```

## Comparing `a3exception-0.1.3.tar` & `a3exception-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 guqiang   (1000) guqiang   (1000)        0 2024-03-26 02:46:29.472527 a3exception-0.1.3/
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)    11357 2024-02-08 11:23:49.000000 a3exception-0.1.3/LICENSE
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)       69 2024-02-20 08:10:34.000000 a3exception-0.1.3/MANIFEST.in
--rw-r--r--   0 guqiang   (1000) guqiang   (1000)     1232 2024-03-26 02:46:29.472527 a3exception-0.1.3/PKG-INFO
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)      137 2024-02-20 08:10:34.000000 a3exception-0.1.3/README.md
-drwxrwxr-x   0 guqiang   (1000) guqiang   (1000)        0 2024-03-26 02:46:29.472527 a3exception-0.1.3/a3exception/
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)       47 2024-03-26 02:45:19.000000 a3exception-0.1.3/a3exception/__init__.py
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)     1054 2024-03-26 02:44:30.000000 a3exception-0.1.3/a3exception/dynamic_error_factory.py
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)     2429 2024-03-11 10:27:11.000000 a3exception-0.1.3/a3exception/errors.py
-drwxrwxr-x   0 guqiang   (1000) guqiang   (1000)        0 2024-03-26 02:46:29.472527 a3exception-0.1.3/a3exception.egg-info/
--rw-r--r--   0 guqiang   (1000) guqiang   (1000)     1232 2024-03-26 02:46:29.000000 a3exception-0.1.3/a3exception.egg-info/PKG-INFO
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)      339 2024-03-26 02:46:29.000000 a3exception-0.1.3/a3exception.egg-info/SOURCES.txt
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)        1 2024-03-26 02:46:29.000000 a3exception-0.1.3/a3exception.egg-info/dependency_links.txt
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)        1 2024-03-26 02:46:29.000000 a3exception-0.1.3/a3exception.egg-info/not-zip-safe
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)        5 2024-03-26 02:46:29.000000 a3exception-0.1.3/a3exception.egg-info/requires.txt
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)       12 2024-03-26 02:46:29.000000 a3exception-0.1.3/a3exception.egg-info/top_level.txt
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)     1133 2024-03-26 02:46:29.472527 a3exception-0.1.3/setup.cfg
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)       39 2024-02-08 11:23:49.000000 a3exception-0.1.3/setup.py
+drwxrwxr-x   0 guqiang   (1000) guqiang   (1000)        0 2024-04-03 06:06:39.978828 a3exception-0.1.4/
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)    11357 2024-02-08 11:23:49.000000 a3exception-0.1.4/LICENSE
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)       69 2024-02-20 08:10:34.000000 a3exception-0.1.4/MANIFEST.in
+-rw-r--r--   0 guqiang   (1000) guqiang   (1000)     1232 2024-04-03 06:06:39.978828 a3exception-0.1.4/PKG-INFO
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)      137 2024-02-20 08:10:34.000000 a3exception-0.1.4/README.md
+drwxrwxr-x   0 guqiang   (1000) guqiang   (1000)        0 2024-04-03 06:06:39.974828 a3exception-0.1.4/a3exception/
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)       47 2024-04-03 06:04:48.000000 a3exception-0.1.4/a3exception/__init__.py
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)     1054 2024-03-26 02:44:30.000000 a3exception-0.1.4/a3exception/dynamic_error_factory.py
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)     2610 2024-04-03 06:04:33.000000 a3exception-0.1.4/a3exception/errors.py
+drwxrwxr-x   0 guqiang   (1000) guqiang   (1000)        0 2024-04-03 06:06:39.978828 a3exception-0.1.4/a3exception.egg-info/
+-rw-r--r--   0 guqiang   (1000) guqiang   (1000)     1232 2024-04-03 06:06:39.000000 a3exception-0.1.4/a3exception.egg-info/PKG-INFO
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)      339 2024-04-03 06:06:39.000000 a3exception-0.1.4/a3exception.egg-info/SOURCES.txt
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)        1 2024-04-03 06:06:39.000000 a3exception-0.1.4/a3exception.egg-info/dependency_links.txt
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)        1 2024-04-03 06:06:39.000000 a3exception-0.1.4/a3exception.egg-info/not-zip-safe
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)        5 2024-04-03 06:06:39.000000 a3exception-0.1.4/a3exception.egg-info/requires.txt
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)       12 2024-04-03 06:06:39.000000 a3exception-0.1.4/a3exception.egg-info/top_level.txt
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)     1133 2024-04-03 06:06:39.978828 a3exception-0.1.4/setup.cfg
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)       39 2024-02-08 11:23:49.000000 a3exception-0.1.4/setup.py
```

### Comparing `a3exception-0.1.3/LICENSE` & `a3exception-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `a3exception-0.1.3/PKG-INFO` & `a3exception-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: a3exception
-Version: 0.1.3
+Version: 0.1.4
 Summary: Framework-agnostic exception component.
 Home-page: https://github.com/three-kinds/a3exception
 Author: three-kinds
 Author-email: 3179158552@qq.com
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/three-kinds/a3exception
 Project-URL: Source, https://github.com/three-kinds/a3exception
```

### Comparing `a3exception-0.1.3/a3exception/dynamic_error_factory.py` & `a3exception-0.1.4/a3exception/dynamic_error_factory.py`

 * *Files identical despite different names*

### Comparing `a3exception-0.1.3/a3exception/errors.py` & `a3exception-0.1.4/a3exception/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,21 @@
     def __str__(self):
         return self.message
 
     def __repr__(self):
         return self.cause
 
 
+class AuthenticationFailed(Error):
+    error_type = ErrorType.ClientSideError
+
+    def __init__(self, message: str, **kwargs):
+        super().__init__(message=message, **kwargs)
+
+
 class ClientKnownError(Error):
     error_type = ErrorType.ClientSideError
 
     def __init__(self, message: str, **kwargs):
         super().__init__(message=message, **kwargs)
```

### Comparing `a3exception-0.1.3/a3exception.egg-info/PKG-INFO` & `a3exception-0.1.4/a3exception.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: a3exception
-Version: 0.1.3
+Version: 0.1.4
 Summary: Framework-agnostic exception component.
 Home-page: https://github.com/three-kinds/a3exception
 Author: three-kinds
 Author-email: 3179158552@qq.com
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/three-kinds/a3exception
 Project-URL: Source, https://github.com/three-kinds/a3exception
```

### Comparing `a3exception-0.1.3/setup.cfg` & `a3exception-0.1.4/setup.cfg`

 * *Files identical despite different names*

