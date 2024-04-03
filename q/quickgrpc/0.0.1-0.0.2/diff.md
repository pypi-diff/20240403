# Comparing `tmp/quickgrpc-0.0.1.tar.gz` & `tmp/quickgrpc-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickgrpc-0.0.1.tar", last modified: Wed Apr  3 20:44:26 2024, max compression
+gzip compressed data, was "quickgrpc-0.0.2.tar", last modified: Wed Apr  3 20:55:42 2024, max compression
```

## Comparing `quickgrpc-0.0.1.tar` & `quickgrpc-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 20:44:26.317116 quickgrpc-0.0.1/
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)       32 2024-04-03 20:37:11.000000 quickgrpc-0.0.1/MANIFEST.in
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     5236 2024-04-03 20:44:26.316931 quickgrpc-0.0.1/PKG-INFO
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     4345 2024-04-03 20:37:11.000000 quickgrpc-0.0.1/README.md
-drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 20:44:26.315670 quickgrpc-0.0.1/quickgrpc/
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 20:37:11.000000 quickgrpc-0.0.1/quickgrpc/__init__.py
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     1106 2024-04-03 20:37:11.000000 quickgrpc-0.0.1/quickgrpc/utils.py
-drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 20:44:26.316756 quickgrpc-0.0.1/quickgrpc.egg-info/
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     5236 2024-04-03 20:44:26.000000 quickgrpc-0.0.1/quickgrpc.egg-info/PKG-INFO
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)      328 2024-04-03 20:44:26.000000 quickgrpc-0.0.1/quickgrpc.egg-info/SOURCES.txt
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)        1 2024-04-03 20:44:26.000000 quickgrpc-0.0.1/quickgrpc.egg-info/dependency_links.txt
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)      140 2024-04-03 20:44:26.000000 quickgrpc-0.0.1/quickgrpc.egg-info/requires.txt
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)       10 2024-04-03 20:44:26.000000 quickgrpc-0.0.1/quickgrpc.egg-info/top_level.txt
-drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 20:44:26.316513 quickgrpc-0.0.1/scripts/
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     3328 2024-04-03 20:37:11.000000 quickgrpc-0.0.1/scripts/create_grpc_service
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     1317 2024-04-03 20:37:11.000000 quickgrpc-0.0.1/scripts/publish_grpc_service
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     1099 2024-04-03 20:37:11.000000 quickgrpc-0.0.1/scripts/servegrpc
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)       38 2024-04-03 20:44:26.317157 quickgrpc-0.0.1/setup.cfg
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     2147 2024-04-03 20:44:18.000000 quickgrpc-0.0.1/setup.py
-drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 20:44:26.316610 quickgrpc-0.0.1/tests/
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     1128 2024-04-03 20:37:11.000000 quickgrpc-0.0.1/tests/test_vcs.py
+drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 20:55:42.606221 quickgrpc-0.0.2/
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)       57 2024-04-03 20:52:32.000000 quickgrpc-0.0.2/MANIFEST.in
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     5236 2024-04-03 20:55:42.606062 quickgrpc-0.0.2/PKG-INFO
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     4345 2024-04-03 20:37:11.000000 quickgrpc-0.0.2/README.md
+drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 20:55:42.604803 quickgrpc-0.0.2/quickgrpc/
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 20:37:11.000000 quickgrpc-0.0.2/quickgrpc/__init__.py
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     1106 2024-04-03 20:37:11.000000 quickgrpc-0.0.2/quickgrpc/utils.py
+drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 20:55:42.605870 quickgrpc-0.0.2/quickgrpc.egg-info/
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     5236 2024-04-03 20:55:42.000000 quickgrpc-0.0.2/quickgrpc.egg-info/PKG-INFO
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)      345 2024-04-03 20:55:42.000000 quickgrpc-0.0.2/quickgrpc.egg-info/SOURCES.txt
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)        1 2024-04-03 20:55:42.000000 quickgrpc-0.0.2/quickgrpc.egg-info/dependency_links.txt
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)      140 2024-04-03 20:55:42.000000 quickgrpc-0.0.2/quickgrpc.egg-info/requires.txt
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)       10 2024-04-03 20:55:42.000000 quickgrpc-0.0.2/quickgrpc.egg-info/top_level.txt
+-rwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)      146 2024-04-03 20:37:11.000000 quickgrpc-0.0.2/requirements.txt
+drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 20:55:42.605627 quickgrpc-0.0.2/scripts/
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     3328 2024-04-03 20:37:11.000000 quickgrpc-0.0.2/scripts/create_grpc_service
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     1317 2024-04-03 20:37:11.000000 quickgrpc-0.0.2/scripts/publish_grpc_service
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     1099 2024-04-03 20:37:11.000000 quickgrpc-0.0.2/scripts/servegrpc
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)       38 2024-04-03 20:55:42.606266 quickgrpc-0.0.2/setup.cfg
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     2147 2024-04-03 20:55:33.000000 quickgrpc-0.0.2/setup.py
+drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 20:55:42.605721 quickgrpc-0.0.2/tests/
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     1128 2024-04-03 20:37:11.000000 quickgrpc-0.0.2/tests/test_vcs.py
```

### Comparing `quickgrpc-0.0.1/PKG-INFO` & `quickgrpc-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickgrpc
-Version: 0.0.1
+Version: 0.0.2
 Summary: quickgrpc lib library
 Home-page: https://github.com/ashupednekar
 Author: Ashutosh Pednekar
 Author-email: ashupednekar49@gmail.com
 Project-URL: Source, https://github.com/ashupednekar/quickgrpc
 Project-URL: Documentation, https://ashupednekar.github.io/quickgrpc
 Project-URL: Bug Tracker, https://github.com/ashupednekar/quickgrpc/issues
```

### Comparing `quickgrpc-0.0.1/README.md` & `quickgrpc-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `quickgrpc-0.0.1/quickgrpc/utils.py` & `quickgrpc-0.0.2/quickgrpc/utils.py`

 * *Files identical despite different names*

### Comparing `quickgrpc-0.0.1/quickgrpc.egg-info/PKG-INFO` & `quickgrpc-0.0.2/quickgrpc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickgrpc
-Version: 0.0.1
+Version: 0.0.2
 Summary: quickgrpc lib library
 Home-page: https://github.com/ashupednekar
 Author: Ashutosh Pednekar
 Author-email: ashupednekar49@gmail.com
 Project-URL: Source, https://github.com/ashupednekar/quickgrpc
 Project-URL: Documentation, https://ashupednekar.github.io/quickgrpc
 Project-URL: Bug Tracker, https://github.com/ashupednekar/quickgrpc/issues
```

### Comparing `quickgrpc-0.0.1/scripts/create_grpc_service` & `quickgrpc-0.0.2/scripts/create_grpc_service`

 * *Files identical despite different names*

### Comparing `quickgrpc-0.0.1/scripts/publish_grpc_service` & `quickgrpc-0.0.2/scripts/publish_grpc_service`

 * *Files identical despite different names*

### Comparing `quickgrpc-0.0.1/scripts/servegrpc` & `quickgrpc-0.0.2/scripts/servegrpc`

 * *Files identical despite different names*

### Comparing `quickgrpc-0.0.1/setup.py` & `quickgrpc-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     with open("requirements.txt", "r") as f:
         return [x for x in f.read().split("\n") if x]
 
 
 # This call to setup() does all the work
 setup(
     name="quickgrpc",
-    version="0.0.1",
+    version="0.0.2",
     description="quickgrpc lib library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ashupednekar",
     author="Ashutosh Pednekar",
     author_email="ashupednekar49@gmail.com",
     license="",
```

### Comparing `quickgrpc-0.0.1/tests/test_vcs.py` & `quickgrpc-0.0.2/tests/test_vcs.py`

 * *Files identical despite different names*

