# Comparing `tmp/beautiful-ternary-1.0.0.tar.gz` & `tmp/beautiful-ternary-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beautiful-ternary-1.0.0.tar", last modified: Mon Apr  1 20:51:40 2024, max compression
+gzip compressed data, was "beautiful-ternary-1.1.0.tar", last modified: Tue Apr  2 23:03:37 2024, max compression
```

## Comparing `beautiful-ternary-1.0.0.tar` & `beautiful-ternary-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 20:51:40.807384 beautiful-ternary-1.0.0/
--rw-rw-rw-   0        0        0     1065 2024-04-01 18:57:10.000000 beautiful-ternary-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1066 2024-04-01 20:51:40.806387 beautiful-ternary-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      298 2024-04-01 20:51:23.000000 beautiful-ternary-1.0.0/README.md
--rw-rw-rw-   0        0        0      859 2024-04-01 20:51:23.000000 beautiful-ternary-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-01 20:51:40.807384 beautiful-ternary-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-01 20:51:40.784352 beautiful-ternary-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-01 20:51:40.805390 beautiful-ternary-1.0.0/src/beautiful_ternary.egg-info/
--rw-rw-rw-   0        0        0     1066 2024-04-01 20:51:40.000000 beautiful-ternary-1.0.0/src/beautiful_ternary.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2024-04-01 20:51:40.000000 beautiful-ternary-1.0.0/src/beautiful_ternary.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 20:51:40.000000 beautiful-ternary-1.0.0/src/beautiful_ternary.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-01 20:51:40.000000 beautiful-ternary-1.0.0/src/beautiful_ternary.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-01 20:51:40.804392 beautiful-ternary-1.0.0/src/ternary/
--rw-rw-rw-   0        0        0       75 2024-04-01 19:31:22.000000 beautiful-ternary-1.0.0/src/ternary/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 20:51:40.805390 beautiful-ternary-1.0.0/tests/
--rw-rw-rw-   0        0        0      245 2024-04-01 20:26:03.000000 beautiful-ternary-1.0.0/tests/test_ternary.py
+drwxrwxrwx   0        0        0        0 2024-04-02 23:03:37.524875 beautiful-ternary-1.1.0/
+-rw-rw-rw-   0        0        0     1065 2024-04-01 18:57:10.000000 beautiful-ternary-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1220 2024-04-02 23:03:37.523878 beautiful-ternary-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      447 2024-04-02 22:49:36.000000 beautiful-ternary-1.1.0/README.md
+-rw-rw-rw-   0        0        0      860 2024-04-02 22:53:53.000000 beautiful-ternary-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-02 23:03:37.524875 beautiful-ternary-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-02 23:03:37.500779 beautiful-ternary-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-02 23:03:37.523878 beautiful-ternary-1.1.0/src/beautiful_ternary.egg-info/
+-rw-rw-rw-   0        0        0     1220 2024-04-02 23:03:37.000000 beautiful-ternary-1.1.0/src/beautiful_ternary.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2024-04-02 23:03:37.000000 beautiful-ternary-1.1.0/src/beautiful_ternary.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 23:03:37.000000 beautiful-ternary-1.1.0/src/beautiful_ternary.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-02 23:03:37.000000 beautiful-ternary-1.1.0/src/beautiful_ternary.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 23:03:37.521885 beautiful-ternary-1.1.0/src/ternary/
+-rw-rw-rw-   0        0        0      268 2024-04-02 22:46:19.000000 beautiful-ternary-1.1.0/src/ternary/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 23:03:37.522881 beautiful-ternary-1.1.0/tests/
+-rw-rw-rw-   0        0        0      982 2024-04-02 22:46:05.000000 beautiful-ternary-1.1.0/tests/test_ternary.py
```

### Comparing `beautiful-ternary-1.0.0/LICENSE` & `beautiful-ternary-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `beautiful-ternary-1.0.0/PKG-INFO` & `beautiful-ternary-1.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 Metadata-Version: 2.1
 Name: beautiful-ternary
-Version: 1.0.0
-Summary: A simple Package to replace the akward built-in ternary operator with a function call.
+Version: 1.1.0
+Summary: A simple Package to replace the awkward built-in ternary operator with a function call.
 Author-email: Christian Witzenberger <christian.witzenberger@triplet.gmbh>
 Project-URL: Homepage, https://github.com/redewing/beautiful-ternary
 Project-URL: Repository, https://github.com/redewing/beautiful-ternary.git
 Project-URL: Issues, https://github.com/redewing/beautiful-ternary/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # beautiful-ternary
-A simple Python Package to replace the akward built-in ternary operator with a function call. Simple.
+A simple Python Package to replace the awkward built-in ternary operator with a function call. Simple.
 
 # Usage
 
     pip install beautiful-ternary
     
-    from ternary import tif
+    from ternary import tif, tlif
     
+    # Use this for non-lazy ternary
     tif(condition, return-if-true, return-if-false)
+    
+    # Use this for lazy ternary
+    tlif(condition, lambda: return-if-true, lambda: return-if-false)
 
 # Dependencies
 
     build, twine, pytest
```

### Comparing `beautiful-ternary-1.0.0/pyproject.toml` & `beautiful-ternary-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "beautiful-ternary"
-version = "1.0.0"
+version = "1.1.0"
 authors = [
   { name="Christian Witzenberger", email="christian.witzenberger@triplet.gmbh" },
 ]
-description = "A simple Package to replace the akward built-in ternary operator with a function call."
+description = "A simple Package to replace the awkward built-in ternary operator with a function call."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `beautiful-ternary-1.0.0/src/beautiful_ternary.egg-info/PKG-INFO` & `beautiful-ternary-1.1.0/src/beautiful_ternary.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 Metadata-Version: 2.1
 Name: beautiful-ternary
-Version: 1.0.0
-Summary: A simple Package to replace the akward built-in ternary operator with a function call.
+Version: 1.1.0
+Summary: A simple Package to replace the awkward built-in ternary operator with a function call.
 Author-email: Christian Witzenberger <christian.witzenberger@triplet.gmbh>
 Project-URL: Homepage, https://github.com/redewing/beautiful-ternary
 Project-URL: Repository, https://github.com/redewing/beautiful-ternary.git
 Project-URL: Issues, https://github.com/redewing/beautiful-ternary/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # beautiful-ternary
-A simple Python Package to replace the akward built-in ternary operator with a function call. Simple.
+A simple Python Package to replace the awkward built-in ternary operator with a function call. Simple.
 
 # Usage
 
     pip install beautiful-ternary
     
-    from ternary import tif
+    from ternary import tif, tlif
     
+    # Use this for non-lazy ternary
     tif(condition, return-if-true, return-if-false)
+    
+    # Use this for lazy ternary
+    tlif(condition, lambda: return-if-true, lambda: return-if-false)
 
 # Dependencies
 
     build, twine, pytest
```

