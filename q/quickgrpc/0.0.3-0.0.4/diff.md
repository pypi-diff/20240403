# Comparing `tmp/quickgrpc-0.0.3.tar.gz` & `tmp/quickgrpc-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickgrpc-0.0.3.tar", last modified: Wed Apr  3 21:04:44 2024, max compression
+gzip compressed data, was "quickgrpc-0.0.4.tar", last modified: Wed Apr  3 21:06:49 2024, max compression
```

## Comparing `quickgrpc-0.0.3.tar` & `quickgrpc-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 21:04:44.116519 quickgrpc-0.0.3/
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)       58 2024-04-03 21:04:09.000000 quickgrpc-0.0.3/MANIFEST.in
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     5236 2024-04-03 21:04:44.116343 quickgrpc-0.0.3/PKG-INFO
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     4345 2024-04-03 20:37:11.000000 quickgrpc-0.0.3/README.md
-drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 21:04:44.114580 quickgrpc-0.0.3/quickgrpc/
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 20:37:11.000000 quickgrpc-0.0.3/quickgrpc/__init__.py
-drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 21:04:44.115594 quickgrpc-0.0.3/quickgrpc/helpers/
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 20:37:11.000000 quickgrpc-0.0.3/quickgrpc/helpers/__init__.py
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     2168 2024-04-03 20:37:11.000000 quickgrpc-0.0.3/quickgrpc/helpers/file.py
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     3762 2024-04-03 20:37:11.000000 quickgrpc-0.0.3/quickgrpc/helpers/misc.py
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     1367 2024-04-03 20:37:11.000000 quickgrpc-0.0.3/quickgrpc/helpers/vcs.py
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     1106 2024-04-03 20:37:11.000000 quickgrpc-0.0.3/quickgrpc/utils.py
-drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 21:04:44.116172 quickgrpc-0.0.3/quickgrpc.egg-info/
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     5236 2024-04-03 21:04:44.000000 quickgrpc-0.0.3/quickgrpc.egg-info/PKG-INFO
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)      452 2024-04-03 21:04:44.000000 quickgrpc-0.0.3/quickgrpc.egg-info/SOURCES.txt
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)        1 2024-04-03 21:04:44.000000 quickgrpc-0.0.3/quickgrpc.egg-info/dependency_links.txt
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)      140 2024-04-03 21:04:44.000000 quickgrpc-0.0.3/quickgrpc.egg-info/requires.txt
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)       10 2024-04-03 21:04:44.000000 quickgrpc-0.0.3/quickgrpc.egg-info/top_level.txt
--rwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)      146 2024-04-03 20:37:11.000000 quickgrpc-0.0.3/requirements.txt
-drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 21:04:44.115905 quickgrpc-0.0.3/scripts/
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     3328 2024-04-03 20:37:11.000000 quickgrpc-0.0.3/scripts/create_grpc_service
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     1317 2024-04-03 20:37:11.000000 quickgrpc-0.0.3/scripts/publish_grpc_service
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     1099 2024-04-03 20:37:11.000000 quickgrpc-0.0.3/scripts/servegrpc
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)       38 2024-04-03 21:04:44.116565 quickgrpc-0.0.3/setup.cfg
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     2019 2024-04-03 21:04:32.000000 quickgrpc-0.0.3/setup.py
-drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 21:04:44.116025 quickgrpc-0.0.3/tests/
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     1128 2024-04-03 20:37:11.000000 quickgrpc-0.0.3/tests/test_vcs.py
+drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 21:06:49.187369 quickgrpc-0.0.4/
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)       58 2024-04-03 21:04:09.000000 quickgrpc-0.0.4/MANIFEST.in
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     5236 2024-04-03 21:06:49.187203 quickgrpc-0.0.4/PKG-INFO
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     4345 2024-04-03 20:37:11.000000 quickgrpc-0.0.4/README.md
+drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 21:06:49.185508 quickgrpc-0.0.4/quickgrpc/
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 20:37:11.000000 quickgrpc-0.0.4/quickgrpc/__init__.py
+drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 21:06:49.186437 quickgrpc-0.0.4/quickgrpc/helpers/
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 20:37:11.000000 quickgrpc-0.0.4/quickgrpc/helpers/__init__.py
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     2168 2024-04-03 20:37:11.000000 quickgrpc-0.0.4/quickgrpc/helpers/file.py
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     3742 2024-04-03 21:05:54.000000 quickgrpc-0.0.4/quickgrpc/helpers/misc.py
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     1367 2024-04-03 20:37:11.000000 quickgrpc-0.0.4/quickgrpc/helpers/vcs.py
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     1106 2024-04-03 20:37:11.000000 quickgrpc-0.0.4/quickgrpc/utils.py
+drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 21:06:49.187028 quickgrpc-0.0.4/quickgrpc.egg-info/
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     5236 2024-04-03 21:06:49.000000 quickgrpc-0.0.4/quickgrpc.egg-info/PKG-INFO
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)      452 2024-04-03 21:06:49.000000 quickgrpc-0.0.4/quickgrpc.egg-info/SOURCES.txt
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)        1 2024-04-03 21:06:49.000000 quickgrpc-0.0.4/quickgrpc.egg-info/dependency_links.txt
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)      140 2024-04-03 21:06:49.000000 quickgrpc-0.0.4/quickgrpc.egg-info/requires.txt
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)       10 2024-04-03 21:06:49.000000 quickgrpc-0.0.4/quickgrpc.egg-info/top_level.txt
+-rwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)      146 2024-04-03 20:37:11.000000 quickgrpc-0.0.4/requirements.txt
+drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 21:06:49.186743 quickgrpc-0.0.4/scripts/
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     3328 2024-04-03 20:37:11.000000 quickgrpc-0.0.4/scripts/create_grpc_service
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     1317 2024-04-03 20:37:11.000000 quickgrpc-0.0.4/scripts/publish_grpc_service
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     1099 2024-04-03 20:37:11.000000 quickgrpc-0.0.4/scripts/servegrpc
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)       38 2024-04-03 21:06:49.187406 quickgrpc-0.0.4/setup.cfg
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     2019 2024-04-03 21:06:40.000000 quickgrpc-0.0.4/setup.py
+drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 21:06:49.186863 quickgrpc-0.0.4/tests/
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     1128 2024-04-03 20:37:11.000000 quickgrpc-0.0.4/tests/test_vcs.py
```

### Comparing `quickgrpc-0.0.3/PKG-INFO` & `quickgrpc-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickgrpc
-Version: 0.0.3
+Version: 0.0.4
 Summary: quickgrpc lib library
 Home-page: https://github.com/ashupednekar
 Author: Ashutosh Pednekar
 Author-email: ashupednekar49@gmail.com
 Project-URL: Source, https://github.com/ashupednekar/quickgrpc
 Project-URL: Documentation, https://ashupednekar.github.io/quickgrpc
 Project-URL: Bug Tracker, https://github.com/ashupednekar/quickgrpc/issues
```

### Comparing `quickgrpc-0.0.3/README.md` & `quickgrpc-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `quickgrpc-0.0.3/quickgrpc/helpers/file.py` & `quickgrpc-0.0.4/quickgrpc/helpers/file.py`

 * *Files identical despite different names*

### Comparing `quickgrpc-0.0.3/quickgrpc/helpers/misc.py` & `quickgrpc-0.0.4/quickgrpc/helpers/misc.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import site
 import sysconfig
 from pathlib import Path
 
 import black
 import isort
 
-from boilerplate_grpc.helpers.file import write_file
+from quickgrpc.helpers.file import write_file
 
 
 def create_package(name):
     """
     The create_package function creates a directory with the name of the package, and then
     creates an empty __init__.py file in that directory.
 
@@ -52,16 +52,15 @@
                 format_with_black(os.path.join(root, file_name))
 
 
 def check_library_installation(library_name):
     try:
         importlib.import_module(library_name)
     except ImportError as e:
-        raise ImportError(
-            f"The library '{library_name}' is not installed.") from e
+        raise ImportError(f"The library '{library_name}' is not installed.") from e
 
 
 def install_library(library_name, token, version=None):
     from pip._internal import main as pip_main
 
     pkg = f"git+https://{token}@github.com/BankBuddy/bud-core-{library_name}-lib"
     if version:
```

### Comparing `quickgrpc-0.0.3/quickgrpc/helpers/vcs.py` & `quickgrpc-0.0.4/quickgrpc/helpers/vcs.py`

 * *Files identical despite different names*

### Comparing `quickgrpc-0.0.3/quickgrpc/utils.py` & `quickgrpc-0.0.4/quickgrpc/utils.py`

 * *Files identical despite different names*

### Comparing `quickgrpc-0.0.3/quickgrpc.egg-info/PKG-INFO` & `quickgrpc-0.0.4/quickgrpc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickgrpc
-Version: 0.0.3
+Version: 0.0.4
 Summary: quickgrpc lib library
 Home-page: https://github.com/ashupednekar
 Author: Ashutosh Pednekar
 Author-email: ashupednekar49@gmail.com
 Project-URL: Source, https://github.com/ashupednekar/quickgrpc
 Project-URL: Documentation, https://ashupednekar.github.io/quickgrpc
 Project-URL: Bug Tracker, https://github.com/ashupednekar/quickgrpc/issues
```

### Comparing `quickgrpc-0.0.3/scripts/create_grpc_service` & `quickgrpc-0.0.4/scripts/create_grpc_service`

 * *Files identical despite different names*

### Comparing `quickgrpc-0.0.3/scripts/publish_grpc_service` & `quickgrpc-0.0.4/scripts/publish_grpc_service`

 * *Files identical despite different names*

### Comparing `quickgrpc-0.0.3/scripts/servegrpc` & `quickgrpc-0.0.4/scripts/servegrpc`

 * *Files identical despite different names*

### Comparing `quickgrpc-0.0.3/setup.py` & `quickgrpc-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     with open("requirements.txt", "r") as f:
         return [x for x in f.read().split("\n") if x]
 
 
 # This call to setup() does all the work
 setup(
     name="quickgrpc",
-    version="0.0.3",
+    version="0.0.4",
     description="quickgrpc lib library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ashupednekar",
     author="Ashutosh Pednekar",
     author_email="ashupednekar49@gmail.com",
     license="",
```

### Comparing `quickgrpc-0.0.3/tests/test_vcs.py` & `quickgrpc-0.0.4/tests/test_vcs.py`

 * *Files identical despite different names*

