# Comparing `tmp/vmk-0.0.1.tar.gz` & `tmp/vmk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vmk-0.0.1.tar", last modified: Wed Apr  3 18:21:18 2024, max compression
+gzip compressed data, was "vmk-0.0.2.tar", last modified: Wed Apr  3 18:31:36 2024, max compression
```

## Comparing `vmk-0.0.1.tar` & `vmk-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 gabriel    (501) staff       (20)        0 2024-04-03 18:21:18.814568 vmk-0.0.1/
--rw-r--r--   0 gabriel    (501) staff       (20)     1068 2024-04-03 18:00:39.000000 vmk-0.0.1/LICENSE
--rw-r--r--   0 gabriel    (501) staff       (20)      547 2024-04-03 18:21:18.814269 vmk-0.0.1/PKG-INFO
--rw-r--r--   0 gabriel    (501) staff       (20)       41 2024-04-03 17:58:32.000000 vmk-0.0.1/README.md
--rw-r--r--   0 gabriel    (501) staff       (20)      662 2024-04-03 18:09:47.000000 vmk-0.0.1/pyproject.toml
--rw-r--r--   0 gabriel    (501) staff       (20)       38 2024-04-03 18:21:18.814611 vmk-0.0.1/setup.cfg
-drwxr-xr-x   0 gabriel    (501) staff       (20)        0 2024-04-03 18:21:18.810027 vmk-0.0.1/src/
-drwxr-xr-x   0 gabriel    (501) staff       (20)        0 2024-04-03 18:21:18.811686 vmk-0.0.1/src/vmk/
--rw-r--r--   0 gabriel    (501) staff       (20)     1098 2024-04-03 18:08:16.000000 vmk-0.0.1/src/vmk/__init__.py
-drwxr-xr-x   0 gabriel    (501) staff       (20)        0 2024-04-03 18:21:18.813835 vmk-0.0.1/src/vmk.egg-info/
--rw-r--r--   0 gabriel    (501) staff       (20)      547 2024-04-03 18:21:18.000000 vmk-0.0.1/src/vmk.egg-info/PKG-INFO
--rw-r--r--   0 gabriel    (501) staff       (20)      210 2024-04-03 18:21:18.000000 vmk-0.0.1/src/vmk.egg-info/SOURCES.txt
--rw-r--r--   0 gabriel    (501) staff       (20)        1 2024-04-03 18:21:18.000000 vmk-0.0.1/src/vmk.egg-info/dependency_links.txt
--rw-r--r--   0 gabriel    (501) staff       (20)       33 2024-04-03 18:21:18.000000 vmk-0.0.1/src/vmk.egg-info/entry_points.txt
--rw-r--r--   0 gabriel    (501) staff       (20)        4 2024-04-03 18:21:18.000000 vmk-0.0.1/src/vmk.egg-info/top_level.txt
+drwxr-xr-x   0 gabriel    (501) staff       (20)        0 2024-04-03 18:31:36.654377 vmk-0.0.2/
+-rw-r--r--   0 gabriel    (501) staff       (20)     1068 2024-04-03 18:00:39.000000 vmk-0.0.2/LICENSE
+-rw-r--r--   0 gabriel    (501) staff       (20)      576 2024-04-03 18:31:36.653908 vmk-0.0.2/PKG-INFO
+-rw-r--r--   0 gabriel    (501) staff       (20)       41 2024-04-03 17:58:32.000000 vmk-0.0.2/README.md
+-rw-r--r--   0 gabriel    (501) staff       (20)      682 2024-04-03 18:31:02.000000 vmk-0.0.2/pyproject.toml
+-rw-r--r--   0 gabriel    (501) staff       (20)       38 2024-04-03 18:31:36.654427 vmk-0.0.2/setup.cfg
+drwxr-xr-x   0 gabriel    (501) staff       (20)        0 2024-04-03 18:31:36.650219 vmk-0.0.2/src/
+drwxr-xr-x   0 gabriel    (501) staff       (20)        0 2024-04-03 18:31:36.651297 vmk-0.0.2/src/vmk/
+-rw-r--r--   0 gabriel    (501) staff       (20)     1098 2024-04-03 18:08:16.000000 vmk-0.0.2/src/vmk/__init__.py
+drwxr-xr-x   0 gabriel    (501) staff       (20)        0 2024-04-03 18:31:36.653585 vmk-0.0.2/src/vmk.egg-info/
+-rw-r--r--   0 gabriel    (501) staff       (20)      576 2024-04-03 18:31:36.000000 vmk-0.0.2/src/vmk.egg-info/PKG-INFO
+-rw-r--r--   0 gabriel    (501) staff       (20)      240 2024-04-03 18:31:36.000000 vmk-0.0.2/src/vmk.egg-info/SOURCES.txt
+-rw-r--r--   0 gabriel    (501) staff       (20)        1 2024-04-03 18:31:36.000000 vmk-0.0.2/src/vmk.egg-info/dependency_links.txt
+-rw-r--r--   0 gabriel    (501) staff       (20)       33 2024-04-03 18:31:36.000000 vmk-0.0.2/src/vmk.egg-info/entry_points.txt
+-rw-r--r--   0 gabriel    (501) staff       (20)       14 2024-04-03 18:31:36.000000 vmk-0.0.2/src/vmk.egg-info/requires.txt
+-rw-r--r--   0 gabriel    (501) staff       (20)        4 2024-04-03 18:31:36.000000 vmk-0.0.2/src/vmk.egg-info/top_level.txt
```

### Comparing `vmk-0.0.1/LICENSE` & `vmk-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vmk-0.0.1/PKG-INFO` & `vmk-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: vmk
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple PDF bundler
 Author: disk, Vormak
 Maintainer-email: chikorito <webmaster@chikorito.land>
 Project-URL: Homepage, https://github.com/fizzy-drinks/vmk
 Project-URL: Issues, https://github.com/fizzy-drinks/vmk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: PyPDF2==3.0.1
 
 # vmk
 
 Simple command-line PDF combiner.
```

### Comparing `vmk-0.0.1/pyproject.toml` & `vmk-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools>=61.0", "PyPDF2==3.0.1"]
+requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vmk"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="disk" },
   { name="Vormak" },
 ]
 maintainers = [
   { name="chikorito", email="webmaster@chikorito.land" },
 ]
@@ -16,14 +16,17 @@
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+  "PyPDF2==3.0.1"
+]
 
 [project.urls]
 Homepage = "https://github.com/fizzy-drinks/vmk"
 Issues = "https://github.com/fizzy-drinks/vmk/issues"
 
 [project.scripts]
 vmk = "vmk:main"
```

### Comparing `vmk-0.0.1/src/vmk/__init__.py` & `vmk-0.0.2/src/vmk/__init__.py`

 * *Files identical despite different names*

### Comparing `vmk-0.0.1/src/vmk.egg-info/PKG-INFO` & `vmk-0.0.2/src/vmk.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: vmk
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple PDF bundler
 Author: disk, Vormak
 Maintainer-email: chikorito <webmaster@chikorito.land>
 Project-URL: Homepage, https://github.com/fizzy-drinks/vmk
 Project-URL: Issues, https://github.com/fizzy-drinks/vmk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: PyPDF2==3.0.1
 
 # vmk
 
 Simple command-line PDF combiner.
```

