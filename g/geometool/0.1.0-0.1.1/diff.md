# Comparing `tmp/geometool-0.1.0.tar.gz` & `tmp/geometool-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geometool-0.1.0.tar", last modified: Wed Apr  3 16:44:17 2024, max compression
+gzip compressed data, was "geometool-0.1.1.tar", last modified: Wed Apr  3 16:49:05 2024, max compression
```

## Comparing `geometool-0.1.0.tar` & `geometool-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:44:17.732992 geometool-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-03 16:44:13.000000 geometool-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-03 16:44:17.732992 geometool-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-03 16:44:13.000000 geometool-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:44:17.728992 geometool-0.1.0/geometool/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-03 16:44:13.000000 geometool-0.1.0/geometool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-03 16:44:13.000000 geometool-0.1.0/geometool/geometry_tool.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-03 16:44:13.000000 geometool-0.1.0/geometool/test_geometry_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:44:17.732992 geometool-0.1.0/geometool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-03 16:44:17.000000 geometool-0.1.0/geometool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-03 16:44:17.000000 geometool-0.1.0/geometool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 16:44:17.000000 geometool-0.1.0/geometool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-03 16:44:17.000000 geometool-0.1.0/geometool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 16:44:17.000000 geometool-0.1.0/geometool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 16:44:17.732992 geometool-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-03 16:44:13.000000 geometool-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:49:05.890499 geometool-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-03 16:49:02.000000 geometool-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-03 16:49:05.890499 geometool-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-03 16:49:02.000000 geometool-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:49:05.890499 geometool-0.1.1/geometool/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-03 16:49:02.000000 geometool-0.1.1/geometool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-03 16:49:02.000000 geometool-0.1.1/geometool/geometry_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-03 16:49:02.000000 geometool-0.1.1/geometool/test_geometry_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:49:05.890499 geometool-0.1.1/geometool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-03 16:49:05.000000 geometool-0.1.1/geometool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-03 16:49:05.000000 geometool-0.1.1/geometool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 16:49:05.000000 geometool-0.1.1/geometool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 16:49:05.000000 geometool-0.1.1/geometool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 16:49:05.890499 geometool-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-03 16:49:02.000000 geometool-0.1.1/setup.py
```

### Comparing `geometool-0.1.0/LICENSE` & `geometool-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geometool-0.1.0/PKG-INFO` & `geometool-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: geometool
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Geometric Shape Calculator Tool
 Home-page: https://github.com/K4speeer/Geometry_Tool
 Author: Idris Taha
 Author-email: dri.taha24@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: abc
 
 # Geometool - Geometric Shape Calculation Library
 
 **```MB Task-1```**
 
 This Python package provides functions to calculate the area and perimeter of various geometric shapes.
```

### Comparing `geometool-0.1.0/README.md` & `geometool-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `geometool-0.1.0/geometool/geometry_tool.py` & `geometool-0.1.1/geometool/geometry_tool.py`

 * *Files identical despite different names*

### Comparing `geometool-0.1.0/geometool/test_geometry_tool.py` & `geometool-0.1.1/geometool/test_geometry_tool.py`

 * *Files identical despite different names*

### Comparing `geometool-0.1.0/geometool.egg-info/PKG-INFO` & `geometool-0.1.1/geometool.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: geometool
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Geometric Shape Calculator Tool
 Home-page: https://github.com/K4speeer/Geometry_Tool
 Author: Idris Taha
 Author-email: dri.taha24@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: abc
 
 # Geometool - Geometric Shape Calculation Library
 
 **```MB Task-1```**
 
 This Python package provides functions to calculate the area and perimeter of various geometric shapes.
```

### Comparing `geometool-0.1.0/setup.py` & `geometool-0.1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,19 +5,17 @@
 
 
 
     
     
 setup(
     name='geometool',
-    version='0.1.0',
+    version='0.1.1',
     packages=['geometool'],
-    install_requires= [
-        'abc'
-    ],
+    install_requires= [],
     author='Idris Taha',
     author_email='dri.taha24@gmail.com',
     description='A Geometric Shape Calculator Tool',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/K4speeer/Geometry_Tool',
     classifiers=[
```

