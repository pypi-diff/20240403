# Comparing `tmp/claimed-0.1.4.tar.gz` & `tmp/claimed-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "claimed-0.1.4.tar", last modified: Mon Mar 25 11:03:30 2024, max compression
+gzip compressed data, was "claimed-0.1.5.tar", last modified: Wed Apr  3 15:19:48 2024, max compression
```

## Comparing `claimed-0.1.4.tar` & `claimed-0.1.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 romeokienzler  (1000) romeokienzler  (1000)        0 2024-03-25 11:03:30.345433 claimed-0.1.4/
--rw-r--r--   0 romeokienzler  (1000) romeokienzler  (1000)      908 2024-03-25 11:03:30.344433 claimed-0.1.4/PKG-INFO
--rw-r--r--   0 romeokienzler  (1000) romeokienzler  (1000)      252 2024-03-25 10:52:30.000000 claimed-0.1.4/README.md
-drwxr-xr-x   0 romeokienzler  (1000) romeokienzler  (1000)        0 2024-03-25 11:03:30.344433 claimed-0.1.4/claimed.egg-info/
--rw-r--r--   0 romeokienzler  (1000) romeokienzler  (1000)      908 2024-03-25 11:03:30.000000 claimed-0.1.4/claimed.egg-info/PKG-INFO
--rw-r--r--   0 romeokienzler  (1000) romeokienzler  (1000)      178 2024-03-25 11:03:30.000000 claimed-0.1.4/claimed.egg-info/SOURCES.txt
--rw-r--r--   0 romeokienzler  (1000) romeokienzler  (1000)        1 2024-03-25 11:03:30.000000 claimed-0.1.4/claimed.egg-info/dependency_links.txt
--rw-r--r--   0 romeokienzler  (1000) romeokienzler  (1000)       37 2024-03-25 11:03:30.000000 claimed-0.1.4/claimed.egg-info/requires.txt
--rw-r--r--   0 romeokienzler  (1000) romeokienzler  (1000)        1 2024-03-25 11:03:30.000000 claimed-0.1.4/claimed.egg-info/top_level.txt
--rw-r--r--   0 romeokienzler  (1000) romeokienzler  (1000)      788 2024-03-25 11:02:27.000000 claimed-0.1.4/pyproject.toml
--rw-r--r--   0 romeokienzler  (1000) romeokienzler  (1000)       38 2024-03-25 11:03:30.345433 claimed-0.1.4/setup.cfg
+drwxr-xr-x   0 romeokienzler  (1000) romeokienzler  (1000)        0 2024-04-03 15:19:48.282868 claimed-0.1.5/
+-rw-r--r--   0 romeokienzler  (1000) romeokienzler  (1000)     1091 2024-04-03 15:19:48.282868 claimed-0.1.5/PKG-INFO
+-rw-r--r--   0 romeokienzler  (1000) romeokienzler  (1000)      436 2024-04-03 10:52:33.000000 claimed-0.1.5/README.md
+drwxr-xr-x   0 romeokienzler  (1000) romeokienzler  (1000)        0 2024-04-03 15:19:48.282868 claimed-0.1.5/claimed.egg-info/
+-rw-r--r--   0 romeokienzler  (1000) romeokienzler  (1000)     1091 2024-04-03 15:19:48.000000 claimed-0.1.5/claimed.egg-info/PKG-INFO
+-rw-r--r--   0 romeokienzler  (1000) romeokienzler  (1000)      178 2024-04-03 15:19:48.000000 claimed-0.1.5/claimed.egg-info/SOURCES.txt
+-rw-r--r--   0 romeokienzler  (1000) romeokienzler  (1000)        1 2024-04-03 15:19:48.000000 claimed-0.1.5/claimed.egg-info/dependency_links.txt
+-rw-r--r--   0 romeokienzler  (1000) romeokienzler  (1000)       37 2024-04-03 15:19:48.000000 claimed-0.1.5/claimed.egg-info/requires.txt
+-rw-r--r--   0 romeokienzler  (1000) romeokienzler  (1000)        1 2024-04-03 15:19:48.000000 claimed-0.1.5/claimed.egg-info/top_level.txt
+-rw-r--r--   0 romeokienzler  (1000) romeokienzler  (1000)      788 2024-04-03 11:51:57.000000 claimed-0.1.5/pyproject.toml
+-rw-r--r--   0 romeokienzler  (1000) romeokienzler  (1000)       38 2024-04-03 15:19:48.282868 claimed-0.1.5/setup.cfg
```

### Comparing `claimed-0.1.4/PKG-INFO` & `claimed-0.1.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 Metadata-Version: 2.1
 Name: claimed
-Version: 0.1.4
+Version: 0.1.5
 Summary: The CLAIMED framework includes reusable operators and the CLAIMED Component Compiler (C3).
 Author-email: The CLAIMED authors <claimed-framework@proton.me>
 Maintainer: Benedikt Blumenstiel
 Maintainer-email: Romeo Kienzler <claimed-framework@proton.me>
 Project-URL: Homepage, https://github.com/claimed-framework
 Keywords: CLAIMED
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Requires-Dist: claimed-c3>=0.3.3
+Requires-Dist: claimed-c3>=0.3.6
 Requires-Dist: claimed-cli>=0.1.5
 
 # Install
 
 ```bash
 pip install claimed
 ```
 
 This package installs the [CLAIMED Component Compiler (C3)](https://pypi.org/project/claimed-c3/) and the [CLAIMED CLI tool](https://pypi.org/project/claimed-cli/) which can be used to run operators locally. 
+
+
+# Build & Publish
+```bash
+python -m build # might require a 'pip install build'
+python -m twine upload --repository pypi dist/* # might require a 'pip install twine'
+rm -r dist
+```
```

### Comparing `claimed-0.1.4/claimed.egg-info/PKG-INFO` & `claimed-0.1.5/claimed.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 Metadata-Version: 2.1
 Name: claimed
-Version: 0.1.4
+Version: 0.1.5
 Summary: The CLAIMED framework includes reusable operators and the CLAIMED Component Compiler (C3).
 Author-email: The CLAIMED authors <claimed-framework@proton.me>
 Maintainer: Benedikt Blumenstiel
 Maintainer-email: Romeo Kienzler <claimed-framework@proton.me>
 Project-URL: Homepage, https://github.com/claimed-framework
 Keywords: CLAIMED
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Requires-Dist: claimed-c3>=0.3.3
+Requires-Dist: claimed-c3>=0.3.6
 Requires-Dist: claimed-cli>=0.1.5
 
 # Install
 
 ```bash
 pip install claimed
 ```
 
 This package installs the [CLAIMED Component Compiler (C3)](https://pypi.org/project/claimed-c3/) and the [CLAIMED CLI tool](https://pypi.org/project/claimed-cli/) which can be used to run operators locally. 
+
+
+# Build & Publish
+```bash
+python -m build # might require a 'pip install build'
+python -m twine upload --repository pypi dist/* # might require a 'pip install twine'
+rm -r dist
+```
```

### Comparing `claimed-0.1.4/pyproject.toml` & `claimed-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "claimed"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="The CLAIMED authors", email="claimed-framework@proton.me"},
 ]
 maintainers = [
   { name="Romeo Kienzler", email="claimed-framework@proton.me"},
   { name="Benedikt Blumenstiel"},
 ]
@@ -17,13 +17,13 @@
 keywords = ["CLAIMED"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    'claimed-c3 >= 0.3.3',
+    'claimed-c3 >= 0.3.6',
     'claimed-cli >= 0.1.5',
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/claimed-framework"
```

