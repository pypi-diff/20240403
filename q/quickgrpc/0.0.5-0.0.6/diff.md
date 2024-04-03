# Comparing `tmp/quickgrpc-0.0.5.tar.gz` & `tmp/quickgrpc-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickgrpc-0.0.5.tar", last modified: Wed Apr  3 21:11:00 2024, max compression
+gzip compressed data, was "quickgrpc-0.0.6.tar", last modified: Wed Apr  3 21:12:03 2024, max compression
```

## Comparing `quickgrpc-0.0.5.tar` & `quickgrpc-0.0.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 21:11:00.856302 quickgrpc-0.0.5/
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)       58 2024-04-03 21:04:09.000000 quickgrpc-0.0.5/MANIFEST.in
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     5236 2024-04-03 21:11:00.856139 quickgrpc-0.0.5/PKG-INFO
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     4345 2024-04-03 20:37:11.000000 quickgrpc-0.0.5/README.md
-drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 21:11:00.854436 quickgrpc-0.0.5/quickgrpc/
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 20:37:11.000000 quickgrpc-0.0.5/quickgrpc/__init__.py
-drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 21:11:00.855377 quickgrpc-0.0.5/quickgrpc/helpers/
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 20:37:11.000000 quickgrpc-0.0.5/quickgrpc/helpers/__init__.py
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     2168 2024-04-03 20:37:11.000000 quickgrpc-0.0.5/quickgrpc/helpers/file.py
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     3742 2024-04-03 21:05:54.000000 quickgrpc-0.0.5/quickgrpc/helpers/misc.py
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     1367 2024-04-03 20:37:11.000000 quickgrpc-0.0.5/quickgrpc/helpers/vcs.py
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     1106 2024-04-03 20:37:11.000000 quickgrpc-0.0.5/quickgrpc/utils.py
-drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 21:11:00.855961 quickgrpc-0.0.5/quickgrpc.egg-info/
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     5236 2024-04-03 21:11:00.000000 quickgrpc-0.0.5/quickgrpc.egg-info/PKG-INFO
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)      452 2024-04-03 21:11:00.000000 quickgrpc-0.0.5/quickgrpc.egg-info/SOURCES.txt
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)        1 2024-04-03 21:11:00.000000 quickgrpc-0.0.5/quickgrpc.egg-info/dependency_links.txt
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)      140 2024-04-03 21:11:00.000000 quickgrpc-0.0.5/quickgrpc.egg-info/requires.txt
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)       10 2024-04-03 21:11:00.000000 quickgrpc-0.0.5/quickgrpc.egg-info/top_level.txt
--rwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)      146 2024-04-03 20:37:11.000000 quickgrpc-0.0.5/requirements.txt
-drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 21:11:00.855674 quickgrpc-0.0.5/scripts/
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     3328 2024-04-03 20:37:11.000000 quickgrpc-0.0.5/scripts/create_grpc_service
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     1317 2024-04-03 20:37:11.000000 quickgrpc-0.0.5/scripts/publish_grpc_service
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     1099 2024-04-03 20:37:11.000000 quickgrpc-0.0.5/scripts/servegrpc
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)       38 2024-04-03 21:11:00.856340 quickgrpc-0.0.5/setup.cfg
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     2019 2024-04-03 21:10:52.000000 quickgrpc-0.0.5/setup.py
-drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 21:11:00.855792 quickgrpc-0.0.5/tests/
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     1128 2024-04-03 20:37:11.000000 quickgrpc-0.0.5/tests/test_vcs.py
+drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 21:12:03.110441 quickgrpc-0.0.6/
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)       58 2024-04-03 21:04:09.000000 quickgrpc-0.0.6/MANIFEST.in
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     5236 2024-04-03 21:12:03.110275 quickgrpc-0.0.6/PKG-INFO
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     4345 2024-04-03 20:37:11.000000 quickgrpc-0.0.6/README.md
+drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 21:12:03.108635 quickgrpc-0.0.6/quickgrpc/
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 20:37:11.000000 quickgrpc-0.0.6/quickgrpc/__init__.py
+drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 21:12:03.109550 quickgrpc-0.0.6/quickgrpc/helpers/
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 20:37:11.000000 quickgrpc-0.0.6/quickgrpc/helpers/__init__.py
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     2168 2024-04-03 20:37:11.000000 quickgrpc-0.0.6/quickgrpc/helpers/file.py
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     3742 2024-04-03 21:05:54.000000 quickgrpc-0.0.6/quickgrpc/helpers/misc.py
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     1367 2024-04-03 20:37:11.000000 quickgrpc-0.0.6/quickgrpc/helpers/vcs.py
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     1106 2024-04-03 20:37:11.000000 quickgrpc-0.0.6/quickgrpc/utils.py
+drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 21:12:03.110100 quickgrpc-0.0.6/quickgrpc.egg-info/
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     5236 2024-04-03 21:12:03.000000 quickgrpc-0.0.6/quickgrpc.egg-info/PKG-INFO
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)      452 2024-04-03 21:12:03.000000 quickgrpc-0.0.6/quickgrpc.egg-info/SOURCES.txt
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)        1 2024-04-03 21:12:03.000000 quickgrpc-0.0.6/quickgrpc.egg-info/dependency_links.txt
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)      140 2024-04-03 21:12:03.000000 quickgrpc-0.0.6/quickgrpc.egg-info/requires.txt
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)       10 2024-04-03 21:12:03.000000 quickgrpc-0.0.6/quickgrpc.egg-info/top_level.txt
+-rwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)      146 2024-04-03 20:37:11.000000 quickgrpc-0.0.6/requirements.txt
+drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 21:12:03.109848 quickgrpc-0.0.6/scripts/
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     3328 2024-04-03 20:37:11.000000 quickgrpc-0.0.6/scripts/create_grpc_service
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     1321 2024-04-03 21:11:36.000000 quickgrpc-0.0.6/scripts/publish_grpc_service
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     1099 2024-04-03 20:37:11.000000 quickgrpc-0.0.6/scripts/servegrpc
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)       38 2024-04-03 21:12:03.110488 quickgrpc-0.0.6/setup.cfg
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     2019 2024-04-03 21:11:55.000000 quickgrpc-0.0.6/setup.py
+drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 21:12:03.109951 quickgrpc-0.0.6/tests/
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     1128 2024-04-03 20:37:11.000000 quickgrpc-0.0.6/tests/test_vcs.py
```

### Comparing `quickgrpc-0.0.5/PKG-INFO` & `quickgrpc-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickgrpc
-Version: 0.0.5
+Version: 0.0.6
 Summary: quickgrpc lib library
 Home-page: https://github.com/ashupednekar
 Author: Ashutosh Pednekar
 Author-email: ashupednekar49@gmail.com
 Project-URL: Source, https://github.com/ashupednekar/quickgrpc
 Project-URL: Documentation, https://ashupednekar.github.io/quickgrpc
 Project-URL: Bug Tracker, https://github.com/ashupednekar/quickgrpc/issues
```

### Comparing `quickgrpc-0.0.5/README.md` & `quickgrpc-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `quickgrpc-0.0.5/quickgrpc/helpers/file.py` & `quickgrpc-0.0.6/quickgrpc/helpers/file.py`

 * *Files identical despite different names*

### Comparing `quickgrpc-0.0.5/quickgrpc/helpers/misc.py` & `quickgrpc-0.0.6/quickgrpc/helpers/misc.py`

 * *Files identical despite different names*

### Comparing `quickgrpc-0.0.5/quickgrpc/helpers/vcs.py` & `quickgrpc-0.0.6/quickgrpc/helpers/vcs.py`

 * *Files identical despite different names*

### Comparing `quickgrpc-0.0.5/quickgrpc/utils.py` & `quickgrpc-0.0.6/quickgrpc/utils.py`

 * *Files identical despite different names*

### Comparing `quickgrpc-0.0.5/quickgrpc.egg-info/PKG-INFO` & `quickgrpc-0.0.6/quickgrpc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickgrpc
-Version: 0.0.5
+Version: 0.0.6
 Summary: quickgrpc lib library
 Home-page: https://github.com/ashupednekar
 Author: Ashutosh Pednekar
 Author-email: ashupednekar49@gmail.com
 Project-URL: Source, https://github.com/ashupednekar/quickgrpc
 Project-URL: Documentation, https://ashupednekar.github.io/quickgrpc
 Project-URL: Bug Tracker, https://github.com/ashupednekar/quickgrpc/issues
```

### Comparing `quickgrpc-0.0.5/scripts/create_grpc_service` & `quickgrpc-0.0.6/scripts/create_grpc_service`

 * *Files identical despite different names*

### Comparing `quickgrpc-0.0.5/scripts/publish_grpc_service` & `quickgrpc-0.0.6/scripts/publish_grpc_service`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 import shutil
 
 import typer
 import os
 
-from fastgrpc.helpers.misc import get_python_lib
-from fastgrpc.helpers.file import write_file
-from fastgrpc.helpers.vcs import clone, commit, push
+from quickgrpc.helpers.misc import get_python_lib
+from quickgrpc.helpers.file import write_file
+from quickgrpc.helpers.vcs import clone, commit, push
 
 ASSETS_PATH = "/tmp/grpc_assets"
 
 
 def publish_grpc_service(assets_repo_url: str, name: str, message: str):
     clone(assets_repo_url, ASSETS_PATH)
     pb_path = f"{get_python_lib()}/grpc_assets/{name}"
@@ -31,15 +31,15 @@
 
 setup(
     name="grpc_assets",
     version="0.1.0",
     description="grpc assets library",
     license="MIT",
     classifiers=[
-        "Intended Audience :: fastgrpc lib"
+        "Intended Audience :: quickgrpc lib"
     ],
     packages=["grpc_assets"],
     scripts=[],
     include_package_data=True,
 )
         """,
         )
```

### Comparing `quickgrpc-0.0.5/scripts/servegrpc` & `quickgrpc-0.0.6/scripts/servegrpc`

 * *Files identical despite different names*

### Comparing `quickgrpc-0.0.5/setup.py` & `quickgrpc-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     with open("requirements.txt", "r") as f:
         return [x for x in f.read().split("\n") if x]
 
 
 # This call to setup() does all the work
 setup(
     name="quickgrpc",
-    version="0.0.5",
+    version="0.0.6",
     description="quickgrpc lib library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ashupednekar",
     author="Ashutosh Pednekar",
     author_email="ashupednekar49@gmail.com",
     license="",
```

### Comparing `quickgrpc-0.0.5/tests/test_vcs.py` & `quickgrpc-0.0.6/tests/test_vcs.py`

 * *Files identical despite different names*

