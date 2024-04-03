# Comparing `tmp/quickgrpc-0.0.7.tar.gz` & `tmp/quickgrpc-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickgrpc-0.0.7.tar", last modified: Wed Apr  3 21:17:09 2024, max compression
+gzip compressed data, was "quickgrpc-0.0.8.tar", last modified: Wed Apr  3 21:21:15 2024, max compression
```

## Comparing `quickgrpc-0.0.7.tar` & `quickgrpc-0.0.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 21:17:09.580840 quickgrpc-0.0.7/
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)       58 2024-04-03 21:04:09.000000 quickgrpc-0.0.7/MANIFEST.in
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     5236 2024-04-03 21:17:09.580684 quickgrpc-0.0.7/PKG-INFO
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     4345 2024-04-03 20:37:11.000000 quickgrpc-0.0.7/README.md
-drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 21:17:09.578941 quickgrpc-0.0.7/quickgrpc/
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 20:37:11.000000 quickgrpc-0.0.7/quickgrpc/__init__.py
-drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 21:17:09.579881 quickgrpc-0.0.7/quickgrpc/helpers/
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 20:37:11.000000 quickgrpc-0.0.7/quickgrpc/helpers/__init__.py
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     2168 2024-04-03 20:37:11.000000 quickgrpc-0.0.7/quickgrpc/helpers/file.py
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     3742 2024-04-03 21:05:54.000000 quickgrpc-0.0.7/quickgrpc/helpers/misc.py
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     1367 2024-04-03 20:37:11.000000 quickgrpc-0.0.7/quickgrpc/helpers/vcs.py
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     1769 2024-04-03 21:14:51.000000 quickgrpc-0.0.7/quickgrpc/utils.py
-drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 21:17:09.580514 quickgrpc-0.0.7/quickgrpc.egg-info/
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     5236 2024-04-03 21:17:09.000000 quickgrpc-0.0.7/quickgrpc.egg-info/PKG-INFO
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)      452 2024-04-03 21:17:09.000000 quickgrpc-0.0.7/quickgrpc.egg-info/SOURCES.txt
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)        1 2024-04-03 21:17:09.000000 quickgrpc-0.0.7/quickgrpc.egg-info/dependency_links.txt
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)      140 2024-04-03 21:17:09.000000 quickgrpc-0.0.7/quickgrpc.egg-info/requires.txt
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)       10 2024-04-03 21:17:09.000000 quickgrpc-0.0.7/quickgrpc.egg-info/top_level.txt
--rwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)      146 2024-04-03 20:37:11.000000 quickgrpc-0.0.7/requirements.txt
-drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 21:17:09.580188 quickgrpc-0.0.7/scripts/
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     3328 2024-04-03 20:37:11.000000 quickgrpc-0.0.7/scripts/create_grpc_service
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     1321 2024-04-03 21:11:36.000000 quickgrpc-0.0.7/scripts/publish_grpc_service
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     1099 2024-04-03 20:37:11.000000 quickgrpc-0.0.7/scripts/servegrpc
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)       38 2024-04-03 21:17:09.580933 quickgrpc-0.0.7/setup.cfg
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     2019 2024-04-03 21:17:01.000000 quickgrpc-0.0.7/setup.py
-drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 21:17:09.580330 quickgrpc-0.0.7/tests/
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     1128 2024-04-03 20:37:11.000000 quickgrpc-0.0.7/tests/test_vcs.py
+drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 21:21:15.757381 quickgrpc-0.0.8/
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)       58 2024-04-03 21:04:09.000000 quickgrpc-0.0.8/MANIFEST.in
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     5236 2024-04-03 21:21:15.757220 quickgrpc-0.0.8/PKG-INFO
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     4345 2024-04-03 20:37:11.000000 quickgrpc-0.0.8/README.md
+drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 21:21:15.755569 quickgrpc-0.0.8/quickgrpc/
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 20:37:11.000000 quickgrpc-0.0.8/quickgrpc/__init__.py
+drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 21:21:15.756470 quickgrpc-0.0.8/quickgrpc/helpers/
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 20:37:11.000000 quickgrpc-0.0.8/quickgrpc/helpers/__init__.py
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     2168 2024-04-03 20:37:11.000000 quickgrpc-0.0.8/quickgrpc/helpers/file.py
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     3742 2024-04-03 21:05:54.000000 quickgrpc-0.0.8/quickgrpc/helpers/misc.py
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     1367 2024-04-03 20:37:11.000000 quickgrpc-0.0.8/quickgrpc/helpers/vcs.py
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     1769 2024-04-03 21:14:51.000000 quickgrpc-0.0.8/quickgrpc/utils.py
+drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 21:21:15.757052 quickgrpc-0.0.8/quickgrpc.egg-info/
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     5236 2024-04-03 21:21:15.000000 quickgrpc-0.0.8/quickgrpc.egg-info/PKG-INFO
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)      452 2024-04-03 21:21:15.000000 quickgrpc-0.0.8/quickgrpc.egg-info/SOURCES.txt
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)        1 2024-04-03 21:21:15.000000 quickgrpc-0.0.8/quickgrpc.egg-info/dependency_links.txt
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)      140 2024-04-03 21:21:15.000000 quickgrpc-0.0.8/quickgrpc.egg-info/requires.txt
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)       10 2024-04-03 21:21:15.000000 quickgrpc-0.0.8/quickgrpc.egg-info/top_level.txt
+-rwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)      146 2024-04-03 20:37:11.000000 quickgrpc-0.0.8/requirements.txt
+drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 21:21:15.756808 quickgrpc-0.0.8/scripts/
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     3327 2024-04-03 21:19:57.000000 quickgrpc-0.0.8/scripts/create_grpc_service
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     1321 2024-04-03 21:11:36.000000 quickgrpc-0.0.8/scripts/publish_grpc_service
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     1099 2024-04-03 20:37:11.000000 quickgrpc-0.0.8/scripts/servegrpc
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)       38 2024-04-03 21:21:15.757415 quickgrpc-0.0.8/setup.cfg
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     2019 2024-04-03 21:21:08.000000 quickgrpc-0.0.8/setup.py
+drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 21:21:15.756909 quickgrpc-0.0.8/tests/
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     1128 2024-04-03 20:37:11.000000 quickgrpc-0.0.8/tests/test_vcs.py
```

### Comparing `quickgrpc-0.0.7/PKG-INFO` & `quickgrpc-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickgrpc
-Version: 0.0.7
+Version: 0.0.8
 Summary: quickgrpc lib library
 Home-page: https://github.com/ashupednekar
 Author: Ashutosh Pednekar
 Author-email: ashupednekar49@gmail.com
 Project-URL: Source, https://github.com/ashupednekar/quickgrpc
 Project-URL: Documentation, https://ashupednekar.github.io/quickgrpc
 Project-URL: Bug Tracker, https://github.com/ashupednekar/quickgrpc/issues
```

### Comparing `quickgrpc-0.0.7/README.md` & `quickgrpc-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `quickgrpc-0.0.7/quickgrpc/helpers/file.py` & `quickgrpc-0.0.8/quickgrpc/helpers/file.py`

 * *Files identical despite different names*

### Comparing `quickgrpc-0.0.7/quickgrpc/helpers/misc.py` & `quickgrpc-0.0.8/quickgrpc/helpers/misc.py`

 * *Files identical despite different names*

### Comparing `quickgrpc-0.0.7/quickgrpc/helpers/vcs.py` & `quickgrpc-0.0.8/quickgrpc/helpers/vcs.py`

 * *Files identical despite different names*

### Comparing `quickgrpc-0.0.7/quickgrpc/utils.py` & `quickgrpc-0.0.8/quickgrpc/utils.py`

 * *Files identical despite different names*

### Comparing `quickgrpc-0.0.7/quickgrpc.egg-info/PKG-INFO` & `quickgrpc-0.0.8/quickgrpc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickgrpc
-Version: 0.0.7
+Version: 0.0.8
 Summary: quickgrpc lib library
 Home-page: https://github.com/ashupednekar
 Author: Ashutosh Pednekar
 Author-email: ashupednekar49@gmail.com
 Project-URL: Source, https://github.com/ashupednekar/quickgrpc
 Project-URL: Documentation, https://ashupednekar.github.io/quickgrpc
 Project-URL: Bug Tracker, https://github.com/ashupednekar/quickgrpc/issues
```

### Comparing `quickgrpc-0.0.7/scripts/create_grpc_service` & `quickgrpc-0.0.8/scripts/create_grpc_service`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     generate_grpc_server(name, file)
     generate_grpc_client(name, file)
 
 
 def generate_grpc_client(name, path):
     click.echo("Generating Client Code...")
     client_code = f"""
-from grpc_assets.stub import get_stub
+from quickgrpc.utils import get_stub
 import grpc_assets.{name}.{name}_pb2 as pb2
 from unittest import TestCase
 
     """
     for service in parse_proto_get_services(path):
         click.echo(f"Adding service: {service['name']}")
         client_code += f"""
```

### Comparing `quickgrpc-0.0.7/scripts/publish_grpc_service` & `quickgrpc-0.0.8/scripts/publish_grpc_service`

 * *Files identical despite different names*

### Comparing `quickgrpc-0.0.7/scripts/servegrpc` & `quickgrpc-0.0.8/scripts/servegrpc`

 * *Files identical despite different names*

### Comparing `quickgrpc-0.0.7/setup.py` & `quickgrpc-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     with open("requirements.txt", "r") as f:
         return [x for x in f.read().split("\n") if x]
 
 
 # This call to setup() does all the work
 setup(
     name="quickgrpc",
-    version="0.0.7",
+    version="0.0.8",
     description="quickgrpc lib library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ashupednekar",
     author="Ashutosh Pednekar",
     author_email="ashupednekar49@gmail.com",
     license="",
```

### Comparing `quickgrpc-0.0.7/tests/test_vcs.py` & `quickgrpc-0.0.8/tests/test_vcs.py`

 * *Files identical despite different names*

