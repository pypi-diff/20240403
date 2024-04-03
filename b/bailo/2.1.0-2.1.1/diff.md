# Comparing `tmp/bailo-2.1.0.tar.gz` & `tmp/bailo-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bailo-2.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "bailo-2.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `bailo-2.1.0.tar` & `bailo-2.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     2241 2024-04-02 10:54:52.927553 bailo-2.1.0/README.md
--rw-r--r--   0        0        0     4869 2024-04-02 10:54:52.927553 bailo-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      631 2024-04-02 10:54:52.927553 bailo-2.1.0/src/bailo/__init__.py
--rw-r--r--   0        0        0      153 2024-04-02 10:54:52.927553 bailo-2.1.0/src/bailo/core/__init__.py
--rw-r--r--   0        0        0     3571 2024-04-02 10:54:52.927553 bailo-2.1.0/src/bailo/core/agent.py
--rw-r--r--   0        0        0    19039 2024-04-02 10:54:52.927553 bailo-2.1.0/src/bailo/core/client.py
--rw-r--r--   0        0        0      564 2024-04-02 10:54:52.927553 bailo-2.1.0/src/bailo/core/enums.py
--rw-r--r--   0        0        0      221 2024-04-02 10:54:52.927553 bailo-2.1.0/src/bailo/core/exceptions.py
--rw-r--r--   0        0        0     1057 2024-04-02 10:54:52.927553 bailo-2.1.0/src/bailo/core/utils.py
--rw-r--r--   0        0        0      521 2024-04-02 10:54:52.927553 bailo-2.1.0/src/bailo/helper/__init__.py
--rw-r--r--   0        0        0     3923 2024-04-02 10:54:52.927553 bailo-2.1.0/src/bailo/helper/access_request.py
--rw-r--r--   0        0        0    15195 2024-04-02 10:54:52.927553 bailo-2.1.0/src/bailo/helper/model.py
--rw-r--r--   0        0        0     7043 2024-04-02 10:54:52.927553 bailo-2.1.0/src/bailo/helper/release.py
--rw-r--r--   0        0        0     2976 2024-04-02 10:54:52.927553 bailo-2.1.0/src/bailo/helper/schema.py
--rw-r--r--   0        0        0     3646 1970-01-01 00:00:00.000000 bailo-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2241 2024-04-03 16:38:22.025113 bailo-2.1.1/README.md
+-rw-r--r--   0        0        0     4869 2024-04-03 16:38:22.025113 bailo-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0      605 2024-04-03 16:38:22.025113 bailo-2.1.1/src/bailo/__init__.py
+-rw-r--r--   0        0        0      153 2024-04-03 16:38:22.025113 bailo-2.1.1/src/bailo/core/__init__.py
+-rw-r--r--   0        0        0     3458 2024-04-03 16:38:22.029113 bailo-2.1.1/src/bailo/core/agent.py
+-rw-r--r--   0        0        0    19039 2024-04-03 16:38:22.029113 bailo-2.1.1/src/bailo/core/client.py
+-rw-r--r--   0        0        0      564 2024-04-03 16:38:22.029113 bailo-2.1.1/src/bailo/core/enums.py
+-rw-r--r--   0        0        0      221 2024-04-03 16:38:22.029113 bailo-2.1.1/src/bailo/core/exceptions.py
+-rw-r--r--   0        0        0     1057 2024-04-03 16:38:22.029113 bailo-2.1.1/src/bailo/core/utils.py
+-rw-r--r--   0        0        0      521 2024-04-03 16:38:22.029113 bailo-2.1.1/src/bailo/helper/__init__.py
+-rw-r--r--   0        0        0     3923 2024-04-03 16:38:22.029113 bailo-2.1.1/src/bailo/helper/access_request.py
+-rw-r--r--   0        0        0    15195 2024-04-03 16:38:22.029113 bailo-2.1.1/src/bailo/helper/model.py
+-rw-r--r--   0        0        0     7043 2024-04-03 16:38:22.029113 bailo-2.1.1/src/bailo/helper/release.py
+-rw-r--r--   0        0        0     2976 2024-04-03 16:38:22.029113 bailo-2.1.1/src/bailo/helper/schema.py
+-rw-r--r--   0        0        0     3646 1970-01-01 00:00:00.000000 bailo-2.1.1/PKG-INFO
```

### Comparing `bailo-2.1.0/README.md` & `bailo-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `bailo-2.1.0/pyproject.toml` & `bailo-2.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bailo-2.1.0/src/bailo/core/agent.py` & `bailo-2.1.1/src/bailo/core/agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,20 +7,17 @@
 from bailo.core.exceptions import BailoException, ResponseException
 
 
 class Agent:
     """Base API Agent for talking with Bailo.
 
     Wraps each request in an exception handler that maps API errors to Python Bailo errors, among status codes less than 400.
-    Defaults request timeout to 5 seconds.
     """
 
     def __request(self, method, *args, **kwargs):
-        if "timeout" not in kwargs:
-            kwargs["timeout"] = 5
         if "verify" not in kwargs:
             kwargs["verify"] = True
 
         res = requests.request(method, *args, **kwargs)
 
         # Check response for a valid range
         if res.status_code < 400:
```

### Comparing `bailo-2.1.0/src/bailo/core/client.py` & `bailo-2.1.1/src/bailo/core/client.py`

 * *Files identical despite different names*

### Comparing `bailo-2.1.0/src/bailo/core/enums.py` & `bailo-2.1.1/src/bailo/core/enums.py`

 * *Files identical despite different names*

### Comparing `bailo-2.1.0/src/bailo/core/utils.py` & `bailo-2.1.1/src/bailo/core/utils.py`

 * *Files identical despite different names*

### Comparing `bailo-2.1.0/src/bailo/helper/__init__.py` & `bailo-2.1.1/src/bailo/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `bailo-2.1.0/src/bailo/helper/access_request.py` & `bailo-2.1.1/src/bailo/helper/access_request.py`

 * *Files identical despite different names*

### Comparing `bailo-2.1.0/src/bailo/helper/model.py` & `bailo-2.1.1/src/bailo/helper/model.py`

 * *Files identical despite different names*

### Comparing `bailo-2.1.0/src/bailo/helper/release.py` & `bailo-2.1.1/src/bailo/helper/release.py`

 * *Files identical despite different names*

### Comparing `bailo-2.1.0/src/bailo/helper/schema.py` & `bailo-2.1.1/src/bailo/helper/schema.py`

 * *Files identical despite different names*

### Comparing `bailo-2.1.0/PKG-INFO` & `bailo-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bailo
-Version: 2.1.0
+Version: 2.1.1
 Summary: Simplifies interacting with Bailo
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bailo Version: 2.1.0 Summary: Simplifies
+Metadata-Version: 2.1 Name: bailo Version: 2.1.1 Summary: Simplifies
 interacting with Bailo Requires-Python: >=3.8.1 Description-Content-Type: text/
 markdown Classifier: Development Status :: 3 - Alpha Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: semantic-version==2.10.0 Requires-Dist: requests>=2.22 Requires-
 Dist: black==23.3.0 ; extra == "test" Requires-Dist: check-manifest==0.49 ;
```

