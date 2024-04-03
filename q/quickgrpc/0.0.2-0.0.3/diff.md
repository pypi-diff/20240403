# Comparing `tmp/quickgrpc-0.0.2.tar.gz` & `tmp/quickgrpc-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickgrpc-0.0.2.tar", last modified: Wed Apr  3 20:55:42 2024, max compression
+gzip compressed data, was "quickgrpc-0.0.3.tar", last modified: Wed Apr  3 21:04:44 2024, max compression
```

## Comparing `quickgrpc-0.0.2.tar` & `quickgrpc-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,27 @@
-drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 20:55:42.606221 quickgrpc-0.0.2/
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)       57 2024-04-03 20:52:32.000000 quickgrpc-0.0.2/MANIFEST.in
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     5236 2024-04-03 20:55:42.606062 quickgrpc-0.0.2/PKG-INFO
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     4345 2024-04-03 20:37:11.000000 quickgrpc-0.0.2/README.md
-drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 20:55:42.604803 quickgrpc-0.0.2/quickgrpc/
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 20:37:11.000000 quickgrpc-0.0.2/quickgrpc/__init__.py
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     1106 2024-04-03 20:37:11.000000 quickgrpc-0.0.2/quickgrpc/utils.py
-drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 20:55:42.605870 quickgrpc-0.0.2/quickgrpc.egg-info/
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     5236 2024-04-03 20:55:42.000000 quickgrpc-0.0.2/quickgrpc.egg-info/PKG-INFO
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)      345 2024-04-03 20:55:42.000000 quickgrpc-0.0.2/quickgrpc.egg-info/SOURCES.txt
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)        1 2024-04-03 20:55:42.000000 quickgrpc-0.0.2/quickgrpc.egg-info/dependency_links.txt
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)      140 2024-04-03 20:55:42.000000 quickgrpc-0.0.2/quickgrpc.egg-info/requires.txt
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)       10 2024-04-03 20:55:42.000000 quickgrpc-0.0.2/quickgrpc.egg-info/top_level.txt
--rwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)      146 2024-04-03 20:37:11.000000 quickgrpc-0.0.2/requirements.txt
-drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 20:55:42.605627 quickgrpc-0.0.2/scripts/
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     3328 2024-04-03 20:37:11.000000 quickgrpc-0.0.2/scripts/create_grpc_service
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     1317 2024-04-03 20:37:11.000000 quickgrpc-0.0.2/scripts/publish_grpc_service
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     1099 2024-04-03 20:37:11.000000 quickgrpc-0.0.2/scripts/servegrpc
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)       38 2024-04-03 20:55:42.606266 quickgrpc-0.0.2/setup.cfg
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     2147 2024-04-03 20:55:33.000000 quickgrpc-0.0.2/setup.py
-drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 20:55:42.605721 quickgrpc-0.0.2/tests/
--rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     1128 2024-04-03 20:37:11.000000 quickgrpc-0.0.2/tests/test_vcs.py
+drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 21:04:44.116519 quickgrpc-0.0.3/
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)       58 2024-04-03 21:04:09.000000 quickgrpc-0.0.3/MANIFEST.in
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     5236 2024-04-03 21:04:44.116343 quickgrpc-0.0.3/PKG-INFO
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     4345 2024-04-03 20:37:11.000000 quickgrpc-0.0.3/README.md
+drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 21:04:44.114580 quickgrpc-0.0.3/quickgrpc/
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 20:37:11.000000 quickgrpc-0.0.3/quickgrpc/__init__.py
+drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 21:04:44.115594 quickgrpc-0.0.3/quickgrpc/helpers/
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 20:37:11.000000 quickgrpc-0.0.3/quickgrpc/helpers/__init__.py
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     2168 2024-04-03 20:37:11.000000 quickgrpc-0.0.3/quickgrpc/helpers/file.py
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     3762 2024-04-03 20:37:11.000000 quickgrpc-0.0.3/quickgrpc/helpers/misc.py
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     1367 2024-04-03 20:37:11.000000 quickgrpc-0.0.3/quickgrpc/helpers/vcs.py
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     1106 2024-04-03 20:37:11.000000 quickgrpc-0.0.3/quickgrpc/utils.py
+drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 21:04:44.116172 quickgrpc-0.0.3/quickgrpc.egg-info/
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     5236 2024-04-03 21:04:44.000000 quickgrpc-0.0.3/quickgrpc.egg-info/PKG-INFO
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)      452 2024-04-03 21:04:44.000000 quickgrpc-0.0.3/quickgrpc.egg-info/SOURCES.txt
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)        1 2024-04-03 21:04:44.000000 quickgrpc-0.0.3/quickgrpc.egg-info/dependency_links.txt
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)      140 2024-04-03 21:04:44.000000 quickgrpc-0.0.3/quickgrpc.egg-info/requires.txt
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)       10 2024-04-03 21:04:44.000000 quickgrpc-0.0.3/quickgrpc.egg-info/top_level.txt
+-rwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)      146 2024-04-03 20:37:11.000000 quickgrpc-0.0.3/requirements.txt
+drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 21:04:44.115905 quickgrpc-0.0.3/scripts/
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     3328 2024-04-03 20:37:11.000000 quickgrpc-0.0.3/scripts/create_grpc_service
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     1317 2024-04-03 20:37:11.000000 quickgrpc-0.0.3/scripts/publish_grpc_service
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     1099 2024-04-03 20:37:11.000000 quickgrpc-0.0.3/scripts/servegrpc
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)       38 2024-04-03 21:04:44.116565 quickgrpc-0.0.3/setup.cfg
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     2019 2024-04-03 21:04:32.000000 quickgrpc-0.0.3/setup.py
+drwxr-xr-x   0 ashutoshpednekar   (501) staff       (20)        0 2024-04-03 21:04:44.116025 quickgrpc-0.0.3/tests/
+-rw-r--r--   0 ashutoshpednekar   (501) staff       (20)     1128 2024-04-03 20:37:11.000000 quickgrpc-0.0.3/tests/test_vcs.py
```

### Comparing `quickgrpc-0.0.2/PKG-INFO` & `quickgrpc-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickgrpc
-Version: 0.0.2
+Version: 0.0.3
 Summary: quickgrpc lib library
 Home-page: https://github.com/ashupednekar
 Author: Ashutosh Pednekar
 Author-email: ashupednekar49@gmail.com
 Project-URL: Source, https://github.com/ashupednekar/quickgrpc
 Project-URL: Documentation, https://ashupednekar.github.io/quickgrpc
 Project-URL: Bug Tracker, https://github.com/ashupednekar/quickgrpc/issues
```

### Comparing `quickgrpc-0.0.2/README.md` & `quickgrpc-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `quickgrpc-0.0.2/quickgrpc/utils.py` & `quickgrpc-0.0.3/quickgrpc/utils.py`

 * *Files identical despite different names*

### Comparing `quickgrpc-0.0.2/quickgrpc.egg-info/PKG-INFO` & `quickgrpc-0.0.3/quickgrpc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickgrpc
-Version: 0.0.2
+Version: 0.0.3
 Summary: quickgrpc lib library
 Home-page: https://github.com/ashupednekar
 Author: Ashutosh Pednekar
 Author-email: ashupednekar49@gmail.com
 Project-URL: Source, https://github.com/ashupednekar/quickgrpc
 Project-URL: Documentation, https://ashupednekar.github.io/quickgrpc
 Project-URL: Bug Tracker, https://github.com/ashupednekar/quickgrpc/issues
```

### Comparing `quickgrpc-0.0.2/scripts/create_grpc_service` & `quickgrpc-0.0.3/scripts/create_grpc_service`

 * *Files identical despite different names*

### Comparing `quickgrpc-0.0.2/scripts/publish_grpc_service` & `quickgrpc-0.0.3/scripts/publish_grpc_service`

 * *Files identical despite different names*

### Comparing `quickgrpc-0.0.2/scripts/servegrpc` & `quickgrpc-0.0.3/scripts/servegrpc`

 * *Files identical despite different names*

### Comparing `quickgrpc-0.0.2/setup.py` & `quickgrpc-0.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 HERE = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
 with open(path.join(HERE, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
-def get_external_reqs():
+def get_dependencies():
     """
     The get_external_reqs function reads the requirements.txt file and returns a list of strings,
     where each string is an external requirement for this project.
 
     :return: A list of strings
     The get_internal_reqs function is used to get the internal requirements for the project.
     This function will read from a file called &quot;internal-requirements.txt&quot; and parse it into a list of strings that can be passed to pip install as dependencies.
@@ -28,36 +28,35 @@
     with open("requirements.txt", "r") as f:
         return [x for x in f.read().split("\n") if x]
 
 
 # This call to setup() does all the work
 setup(
     name="quickgrpc",
-    version="0.0.2",
+    version="0.0.3",
     description="quickgrpc lib library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ashupednekar",
     author="Ashutosh Pednekar",
     author_email="ashupednekar49@gmail.com",
     license="",
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent",
     ],
     project_urls={
-        "Source": "https://github.com/ashupednekar/quickgrpc",  # URL of the source code repository
-        "Documentation": "https://ashupednekar.github.io/quickgrpc",  # URL of the project documentation
-        "Bug Tracker": "https://github.com/ashupednekar/quickgrpc/issues",  # URL of the bug tracker
+        "Source": "https://github.com/ashupednekar/quickgrpc",
+        "Documentation": "https://ashupednekar.github.io/quickgrpc",
+        "Bug Tracker": "https://github.com/ashupednekar/quickgrpc/issues",
     },
     packages=["quickgrpc"],
     scripts=[
         "scripts/create_grpc_service",
         "scripts/publish_grpc_service",
         "scripts/servegrpc",
     ],
     include_package_data=True,
-    # install_requires=[],
-    install_requires=get_external_reqs(),
+    install_requires=get_dependencies(),
 )
```

### Comparing `quickgrpc-0.0.2/tests/test_vcs.py` & `quickgrpc-0.0.3/tests/test_vcs.py`

 * *Files identical despite different names*

