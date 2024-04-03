# Comparing `tmp/geometool-0.0.7.tar.gz` & `tmp/geometool-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geometool-0.0.7.tar", last modified: Wed Apr  3 09:31:10 2024, max compression
+gzip compressed data, was "geometool-0.0.9.tar", last modified: Wed Apr  3 16:26:37 2024, max compression
```

## Comparing `geometool-0.0.7.tar` & `geometool-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:31:10.466688 geometool-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-03 09:31:05.000000 geometool-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-03 09:31:10.466688 geometool-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-03 09:31:05.000000 geometool-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:31:10.466688 geometool-0.0.7/geometool/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-03 09:31:05.000000 geometool-0.0.7/geometool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-03 09:31:05.000000 geometool-0.0.7/geometool/geometry_tool.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-03 09:31:05.000000 geometool-0.0.7/geometool/test_geometry_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:31:10.466688 geometool-0.0.7/geometool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-03 09:31:10.000000 geometool-0.0.7/geometool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-03 09:31:10.000000 geometool-0.0.7/geometool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 09:31:10.000000 geometool-0.0.7/geometool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 09:31:10.000000 geometool-0.0.7/geometool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 09:31:10.000000 geometool-0.0.7/geometool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 09:31:10.466688 geometool-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-03 09:31:05.000000 geometool-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:26:37.656508 geometool-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-03 16:26:34.000000 geometool-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-03 16:26:37.656508 geometool-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-03 16:26:34.000000 geometool-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:26:37.656508 geometool-0.0.9/geometool/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-03 16:26:34.000000 geometool-0.0.9/geometool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-03 16:26:34.000000 geometool-0.0.9/geometool/geometry_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-03 16:26:34.000000 geometool-0.0.9/geometool/test_geometry_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:26:37.656508 geometool-0.0.9/geometool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-03 16:26:37.000000 geometool-0.0.9/geometool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-03 16:26:37.000000 geometool-0.0.9/geometool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 16:26:37.000000 geometool-0.0.9/geometool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 16:26:37.000000 geometool-0.0.9/geometool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 16:26:37.000000 geometool-0.0.9/geometool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 16:26:37.656508 geometool-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-03 16:26:34.000000 geometool-0.0.9/setup.py
```

### Comparing `geometool-0.0.7/LICENSE` & `geometool-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `geometool-0.0.7/PKG-INFO` & `geometool-0.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: geometool
-Version: 0.0.7
+Version: 0.0.9
 Summary: A Geometric Shape Calculator Tool
 Home-page: https://github.com/K4speeer/Geometry_Tool
 Author: Idris Taha
 Author-email: dri.taha24@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mathabc
+Requires-Dist: math
+Requires-Dist: abc
 
 # Geometool - Geometric Shape Calculation Library
 
 **```MB Task-1```**
 
 This Python package provides functions to calculate the area and perimeter of various geometric shapes.
```

### Comparing `geometool-0.0.7/README.md` & `geometool-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `geometool-0.0.7/geometool/geometry_tool.py` & `geometool-0.0.9/geometool/geometry_tool.py`

 * *Files identical despite different names*

### Comparing `geometool-0.0.7/geometool/test_geometry_tool.py` & `geometool-0.0.9/geometool/test_geometry_tool.py`

 * *Files identical despite different names*

### Comparing `geometool-0.0.7/geometool.egg-info/PKG-INFO` & `geometool-0.0.9/geometool.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: geometool
-Version: 0.0.7
+Version: 0.0.9
 Summary: A Geometric Shape Calculator Tool
 Home-page: https://github.com/K4speeer/Geometry_Tool
 Author: Idris Taha
 Author-email: dri.taha24@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mathabc
+Requires-Dist: math
+Requires-Dist: abc
 
 # Geometool - Geometric Shape Calculation Library
 
 **```MB Task-1```**
 
 This Python package provides functions to calculate the area and perimeter of various geometric shapes.
```

### Comparing `geometool-0.0.7/setup.py` & `geometool-0.0.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
+
+
+    
+    
 setup(
     name='geometool',
-    version='0.0.7',
+    version='0.0.9',
     packages=['geometool'],
-    install_requires=[
-        'math'
+    install_requires= [
+        'math',
         'abc'
     ],
     author='Idris Taha',
     author_email='dri.taha24@gmail.com',
     description='A Geometric Shape Calculator Tool',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

