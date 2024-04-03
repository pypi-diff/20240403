# Comparing `tmp/icalreporting-0.1.3.tar.gz` & `tmp/icalreporting-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icalreporting-0.1.3.tar", last modified: Wed Apr  3 08:43:21 2024, max compression
+gzip compressed data, was "icalreporting-0.1.4.tar", last modified: Wed Apr  3 13:51:19 2024, max compression
```

## Comparing `icalreporting-0.1.3.tar` & `icalreporting-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:43:21.618393 icalreporting-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-03 08:43:10.000000 icalreporting-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-04-03 08:43:21.618393 icalreporting-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-03 08:43:10.000000 icalreporting-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:43:21.614393 icalreporting-0.1.3/icalreporting/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 08:43:10.000000 icalreporting-0.1.3/icalreporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6521 2024-04-03 08:43:10.000000 icalreporting-0.1.3/icalreporting/reporting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:43:21.614393 icalreporting-0.1.3/icalreporting.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-04-03 08:43:21.000000 icalreporting-0.1.3/icalreporting.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-03 08:43:21.000000 icalreporting-0.1.3/icalreporting.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 08:43:21.000000 icalreporting-0.1.3/icalreporting.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-03 08:43:21.000000 icalreporting-0.1.3/icalreporting.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-03 08:43:21.000000 icalreporting-0.1.3/icalreporting.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-03 08:43:10.000000 icalreporting-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 08:43:21.618393 icalreporting-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:43:21.614393 icalreporting-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-03 08:43:10.000000 icalreporting-0.1.3/tests/test_icalimport.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:51:19.494150 icalreporting-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-03 13:51:09.000000 icalreporting-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-04-03 13:51:19.494150 icalreporting-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-03 13:51:09.000000 icalreporting-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:51:19.494150 icalreporting-0.1.4/icalreporting/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 13:51:09.000000 icalreporting-0.1.4/icalreporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6521 2024-04-03 13:51:09.000000 icalreporting-0.1.4/icalreporting/reporting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:51:19.494150 icalreporting-0.1.4/icalreporting.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-04-03 13:51:19.000000 icalreporting-0.1.4/icalreporting.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-03 13:51:19.000000 icalreporting-0.1.4/icalreporting.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 13:51:19.000000 icalreporting-0.1.4/icalreporting.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-03 13:51:19.000000 icalreporting-0.1.4/icalreporting.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-03 13:51:19.000000 icalreporting-0.1.4/icalreporting.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-03 13:51:09.000000 icalreporting-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 13:51:19.494150 icalreporting-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:51:19.494150 icalreporting-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-03 13:51:09.000000 icalreporting-0.1.4/tests/test_icalimport.py
```

### Comparing `icalreporting-0.1.3/LICENSE` & `icalreporting-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `icalreporting-0.1.3/PKG-INFO` & `icalreporting-0.1.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icalreporting
-Version: 0.1.3
+Version: 0.1.4
 Summary: Reporting tools from ical files
 Author-email: "J. Gressier" <jeremie.gressier@isae-supaero.fr>
 License: MIT License
         
         Copyright (c) 2023 Jérémie GRESSIER
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -33,18 +33,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy>=1.15
-Requires-Dist: scipy>=1.6
-Requires-Dist: h5py>=3.1
-Requires-Dist: pyvista>=0.38
+Requires-Dist: pandas>=2.1
+Requires-Dist: openpyxl>=3.1
+Requires-Dist: ical>=4.5
 Provides-Extra: dev
 Requires-Dist: pytest>=6.0; extra == "dev"
 Requires-Dist: pytest-cov>=2.11.1; extra == "dev"
 Requires-Dist: pylint>=2.6.0; extra == "dev"
 
 icalreporting
 -----
```

### Comparing `icalreporting-0.1.3/README.md` & `icalreporting-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `icalreporting-0.1.3/icalreporting/reporting.py` & `icalreporting-0.1.4/icalreporting/reporting.py`

 * *Files identical despite different names*

### Comparing `icalreporting-0.1.3/icalreporting.egg-info/PKG-INFO` & `icalreporting-0.1.4/icalreporting.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icalreporting
-Version: 0.1.3
+Version: 0.1.4
 Summary: Reporting tools from ical files
 Author-email: "J. Gressier" <jeremie.gressier@isae-supaero.fr>
 License: MIT License
         
         Copyright (c) 2023 Jérémie GRESSIER
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -33,18 +33,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy>=1.15
-Requires-Dist: scipy>=1.6
-Requires-Dist: h5py>=3.1
-Requires-Dist: pyvista>=0.38
+Requires-Dist: pandas>=2.1
+Requires-Dist: openpyxl>=3.1
+Requires-Dist: ical>=4.5
 Provides-Extra: dev
 Requires-Dist: pytest>=6.0; extra == "dev"
 Requires-Dist: pytest-cov>=2.11.1; extra == "dev"
 Requires-Dist: pylint>=2.6.0; extra == "dev"
 
 icalreporting
 -----
```

### Comparing `icalreporting-0.1.3/pyproject.toml` & `icalreporting-0.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "icalreporting"
-version = "0.1.3"
+version = "0.1.4"
 description = "Reporting tools from ical files"
 authors = [{name="J. Gressier", email="jeremie.gressier@isae-supaero.fr"}]
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: MIT License",
@@ -13,17 +13,17 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries :: Python Modules" ]
 requires-python = ">=3.9"
 dependencies = [
-    "numpy >= 1.15",
-    "scipy >= 1.6",
-    "h5py >= 3.1", "pyvista >= 0.38" ]
+    "pandas >= 2.1",
+    "openpyxl >= 3.1",
+    "ical >= 4.5" ]
 
 [project.urls]
 Homepage = "https://github.com/jgressier/icalreporting"
 
 [tool.setuptools.packages.find] # to help find cfdtools folder as a package
 include = ["icalreporting*"]
 
@@ -41,15 +41,15 @@
 minversion = "6.0"
 addopts = "--cov -v"
 testpaths = [
     "tests"
 ]
 
 [tool.bumpver]
-current_version = "v0.1.3"
+current_version = "v0.1.4"
 version_pattern = "vMAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} to {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `icalreporting-0.1.3/tests/test_icalimport.py` & `icalreporting-0.1.4/tests/test_icalimport.py`

 * *Files identical despite different names*

