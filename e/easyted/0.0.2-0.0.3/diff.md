# Comparing `tmp/easyted-0.0.2.tar.gz` & `tmp/easyted-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyted-0.0.2.tar", last modified: Wed Apr  3 17:34:24 2024, max compression
+gzip compressed data, was "easyted-0.0.3.tar", last modified: Wed Apr  3 19:30:27 2024, max compression
```

## Comparing `easyted-0.0.2.tar` & `easyted-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-sr-x   0 jovyan    (1000) jovyan    (1000)        0 2024-04-03 17:34:24.575372 easyted-0.0.2/
-drwxr-sr-x   0 jovyan    (1000) jovyan    (1000)        0 2024-04-03 17:34:24.571372 easyted-0.0.2/EasyTED/
--rw-r--r--   0 jovyan    (1000) jovyan    (1000)        0 2024-04-03 16:52:43.000000 easyted-0.0.2/EasyTED/__init__.py
--rw-r--r--   0 jovyan    (1000) jovyan    (1000)     7003 2024-04-03 16:59:38.000000 easyted-0.0.2/EasyTED/ted.py
--rw-r--r--   0 jovyan    (1000) jovyan    (1000)     1063 2024-04-03 17:01:50.000000 easyted-0.0.2/LICENSE
--rw-r--r--   0 jovyan    (1000) jovyan    (1000)     6992 2024-04-03 17:34:24.575372 easyted-0.0.2/PKG-INFO
--rw-r--r--   0 jovyan    (1000) jovyan    (1000)     6414 2024-04-03 17:29:33.000000 easyted-0.0.2/README.md
-drwxr-sr-x   0 jovyan    (1000) jovyan    (1000)        0 2024-04-03 17:34:24.575372 easyted-0.0.2/easyted.egg-info/
--rw-r--r--   0 jovyan    (1000) jovyan    (1000)     6992 2024-04-03 17:34:24.000000 easyted-0.0.2/easyted.egg-info/PKG-INFO
--rw-r--r--   0 jovyan    (1000) jovyan    (1000)      215 2024-04-03 17:34:24.000000 easyted-0.0.2/easyted.egg-info/SOURCES.txt
--rw-r--r--   0 jovyan    (1000) jovyan    (1000)        1 2024-04-03 17:34:24.000000 easyted-0.0.2/easyted.egg-info/dependency_links.txt
--rw-r--r--   0 jovyan    (1000) jovyan    (1000)       33 2024-04-03 17:34:24.000000 easyted-0.0.2/easyted.egg-info/requires.txt
--rw-r--r--   0 jovyan    (1000) jovyan    (1000)        8 2024-04-03 17:34:24.000000 easyted-0.0.2/easyted.egg-info/top_level.txt
--rw-r--r--   0 jovyan    (1000) jovyan    (1000)       38 2024-04-03 17:34:24.575372 easyted-0.0.2/setup.cfg
--rw-r--r--   0 jovyan    (1000) jovyan    (1000)      840 2024-04-03 17:32:09.000000 easyted-0.0.2/setup.py
+drwxr-sr-x   0 jovyan    (1000) jovyan    (1000)        0 2024-04-03 19:30:27.777169 easyted-0.0.3/
+-rw-r--r--   0 jovyan    (1000) jovyan    (1000)     1063 2024-04-03 17:01:50.000000 easyted-0.0.3/LICENSE
+-rw-r--r--   0 jovyan    (1000) jovyan    (1000)     7000 2024-04-03 19:30:27.777169 easyted-0.0.3/PKG-INFO
+-rw-r--r--   0 jovyan    (1000) jovyan    (1000)     6422 2024-04-03 19:29:38.000000 easyted-0.0.3/README.md
+drwxr-sr-x   0 jovyan    (1000) jovyan    (1000)        0 2024-04-03 19:30:27.773169 easyted-0.0.3/easyted/
+-rw-r--r--   0 jovyan    (1000) jovyan    (1000)        0 2024-04-03 16:52:43.000000 easyted-0.0.3/easyted/__init__.py
+-rw-r--r--   0 jovyan    (1000) jovyan    (1000)     7003 2024-04-03 16:59:38.000000 easyted-0.0.3/easyted/ted.py
+drwxr-sr-x   0 jovyan    (1000) jovyan    (1000)        0 2024-04-03 19:30:27.777169 easyted-0.0.3/easyted.egg-info/
+-rw-r--r--   0 jovyan    (1000) jovyan    (1000)     7000 2024-04-03 19:30:27.000000 easyted-0.0.3/easyted.egg-info/PKG-INFO
+-rw-r--r--   0 jovyan    (1000) jovyan    (1000)      215 2024-04-03 19:30:27.000000 easyted-0.0.3/easyted.egg-info/SOURCES.txt
+-rw-r--r--   0 jovyan    (1000) jovyan    (1000)        1 2024-04-03 19:30:27.000000 easyted-0.0.3/easyted.egg-info/dependency_links.txt
+-rw-r--r--   0 jovyan    (1000) jovyan    (1000)       33 2024-04-03 19:30:27.000000 easyted-0.0.3/easyted.egg-info/requires.txt
+-rw-r--r--   0 jovyan    (1000) jovyan    (1000)        8 2024-04-03 19:30:27.000000 easyted-0.0.3/easyted.egg-info/top_level.txt
+-rw-r--r--   0 jovyan    (1000) jovyan    (1000)       38 2024-04-03 19:30:27.777169 easyted-0.0.3/setup.cfg
+-rw-r--r--   0 jovyan    (1000) jovyan    (1000)      840 2024-04-03 19:30:22.000000 easyted-0.0.3/setup.py
```

### Comparing `easyted-0.0.2/EasyTED/ted.py` & `easyted-0.0.3/easyted/ted.py`

 * *Files identical despite different names*

### Comparing `easyted-0.0.2/LICENSE` & `easyted-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `easyted-0.0.2/PKG-INFO` & `easyted-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyted
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python library for easy calculation of tree edit distances with visualization capabilities.
 Home-page: https://github.com/LasalJayawardena/easyted
 Author: Lasal Jayawardena
 Author-email: lasalcjl@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -35,27 +35,27 @@
 pip install easyted
 ```
 
 ## High-Level Usage
 
 ### Calculating Full Tree Edit Distance
 ```python
-from easyted import TreeEditDistanceCalculator
+from easyted.ted import TreeEditDistanceCalculator
 
 # Initialize the calculator
 calculator = TreeEditDistanceCalculator()
 
 # Calculate the tree edit distance between two sentences
 distance = calculator.calculate_ted("This is a test.", "This is only a test.")
 print(f"Tree Edit Distance: {distance}")
 ```
 
 ### Calculating N Tree Edit Distance
 ```python
-from easyted import TreeEditDistanceCalculator
+from easyted.ted import TreeEditDistanceCalculator
 
 # Initialize the calculator
 calculator = TreeEditDistanceCalculator()
 
 # Calculate the tree edit distance between two sentences for first 3 layers
 distance = calculator.calculate_ted("This is a test.", "This is only a test.", 3)
 print(f"Tree Edit Distance for first 3 layers: {distance}")
```

### Comparing `easyted-0.0.2/README.md` & `easyted-0.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -18,27 +18,27 @@
 pip install easyted
 ```
 
 ## High-Level Usage
 
 ### Calculating Full Tree Edit Distance
 ```python
-from easyted import TreeEditDistanceCalculator
+from easyted.ted import TreeEditDistanceCalculator
 
 # Initialize the calculator
 calculator = TreeEditDistanceCalculator()
 
 # Calculate the tree edit distance between two sentences
 distance = calculator.calculate_ted("This is a test.", "This is only a test.")
 print(f"Tree Edit Distance: {distance}")
 ```
 
 ### Calculating N Tree Edit Distance
 ```python
-from easyted import TreeEditDistanceCalculator
+from easyted.ted import TreeEditDistanceCalculator
 
 # Initialize the calculator
 calculator = TreeEditDistanceCalculator()
 
 # Calculate the tree edit distance between two sentences for first 3 layers
 distance = calculator.calculate_ted("This is a test.", "This is only a test.", 3)
 print(f"Tree Edit Distance for first 3 layers: {distance}")
```

### Comparing `easyted-0.0.2/easyted.egg-info/PKG-INFO` & `easyted-0.0.3/easyted.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyted
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python library for easy calculation of tree edit distances with visualization capabilities.
 Home-page: https://github.com/LasalJayawardena/easyted
 Author: Lasal Jayawardena
 Author-email: lasalcjl@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -35,27 +35,27 @@
 pip install easyted
 ```
 
 ## High-Level Usage
 
 ### Calculating Full Tree Edit Distance
 ```python
-from easyted import TreeEditDistanceCalculator
+from easyted.ted import TreeEditDistanceCalculator
 
 # Initialize the calculator
 calculator = TreeEditDistanceCalculator()
 
 # Calculate the tree edit distance between two sentences
 distance = calculator.calculate_ted("This is a test.", "This is only a test.")
 print(f"Tree Edit Distance: {distance}")
 ```
 
 ### Calculating N Tree Edit Distance
 ```python
-from easyted import TreeEditDistanceCalculator
+from easyted.ted import TreeEditDistanceCalculator
 
 # Initialize the calculator
 calculator = TreeEditDistanceCalculator()
 
 # Calculate the tree edit distance between two sentences for first 3 layers
 distance = calculator.calculate_ted("This is a test.", "This is only a test.", 3)
 print(f"Tree Edit Distance for first 3 layers: {distance}")
```

### Comparing `easyted-0.0.2/setup.py` & `easyted-0.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="easyted",  
-    version="0.0.2",
+    version="0.0.3",
     author="Lasal Jayawardena",  
     author_email="lasalcjl@gmail.com", 
     description="A Python library for easy calculation of tree edit distances with visualization capabilities.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LasalJayawardena/easyted", 
     packages=find_packages(),
```

