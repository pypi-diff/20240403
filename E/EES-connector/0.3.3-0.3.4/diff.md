# Comparing `tmp/EES_connector-0.3.3.tar.gz` & `tmp/EES_connector-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EES_connector-0.3.3.tar", last modified: Tue Feb 28 11:27:29 2023, max compression
+gzip compressed data, was "EES_connector-0.3.4.tar", last modified: Wed Apr  3 15:47:02 2024, max compression
```

## Comparing `EES_connector-0.3.3.tar` & `EES_connector-0.3.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-02-28 11:27:29.314293 EES_connector-0.3.3/
-drwxrwxrwx   0        0        0        0 2023-02-28 11:27:29.297293 EES_connector-0.3.3/EESConnect/
--rw-rw-rw-   0        0        0     8574 2023-02-28 11:26:16.000000 EES_connector-0.3.3/EESConnect/EES_connect.py
--rw-rw-rw-   0        0        0       78 2022-05-04 08:01:59.000000 EES_connector-0.3.3/EESConnect/__init__.py
--rw-rw-rw-   0        0        0     3568 2022-05-05 08:56:49.000000 EES_connector-0.3.3/EESConnect/constants.py
-drwxrwxrwx   0        0        0        0 2023-02-28 11:27:29.314293 EES_connector-0.3.3/EES_connector.egg-info/
--rw-rw-rw-   0        0        0     4349 2023-02-28 11:27:28.000000 EES_connector-0.3.3/EES_connector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-02-28 11:27:29.000000 EES_connector-0.3.3/EES_connector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-28 11:27:28.000000 EES_connector-0.3.3/EES_connector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-02-28 11:27:28.000000 EES_connector-0.3.3/EES_connector.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-02-28 11:27:28.000000 EES_connector-0.3.3/EES_connector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2022-05-04 08:01:59.000000 EES_connector-0.3.3/LICENSE
--rw-rw-rw-   0        0        0     4349 2023-02-28 11:27:29.314293 EES_connector-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     3521 2023-02-08 10:04:16.000000 EES_connector-0.3.3/README.md
--rw-rw-rw-   0        0        0       86 2023-02-28 11:27:29.318294 EES_connector-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0     1266 2023-02-28 11:26:16.000000 EES_connector-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 15:47:02.876477 EES_connector-0.3.4/
+drwxrwxrwx   0        0        0        0 2024-04-03 15:47:02.856494 EES_connector-0.3.4/EESConnect/
+-rw-rw-rw-   0        0        0     8987 2024-04-03 15:43:45.000000 EES_connector-0.3.4/EESConnect/EES_connect.py
+-rw-rw-rw-   0        0        0       78 2022-05-04 08:01:59.000000 EES_connector-0.3.4/EESConnect/__init__.py
+-rw-rw-rw-   0        0        0     3568 2022-05-05 08:56:49.000000 EES_connector-0.3.4/EESConnect/constants.py
+drwxrwxrwx   0        0        0        0 2024-04-03 15:47:02.875494 EES_connector-0.3.4/EES_connector.egg-info/
+-rw-rw-rw-   0        0        0     4349 2024-04-03 15:47:02.000000 EES_connector-0.3.4/EES_connector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2024-04-03 15:47:02.000000 EES_connector-0.3.4/EES_connector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 15:47:02.000000 EES_connector-0.3.4/EES_connector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-03 15:47:02.000000 EES_connector-0.3.4/EES_connector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-03 15:47:02.000000 EES_connector-0.3.4/EES_connector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2022-05-04 08:01:59.000000 EES_connector-0.3.4/LICENSE
+-rw-rw-rw-   0        0        0     4349 2024-04-03 15:47:02.876477 EES_connector-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3521 2023-02-08 10:04:16.000000 EES_connector-0.3.4/README.md
+-rw-rw-rw-   0        0        0       86 2024-04-03 15:47:02.879493 EES_connector-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     1266 2024-04-03 15:44:52.000000 EES_connector-0.3.4/setup.py
```

### Comparing `EES_connector-0.3.3/EESConnect/EES_connect.py` & `EES_connector-0.3.4/EESConnect/EES_connect.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 import EESConnect.constants as constants
 from tkinter import filedialog
+from tqdm import tqdm
 import tkinter as tk
 import shutil, os
 
 
 class EESConnector:
 
     def __init__(
 
             self, ees_file_path=None,
             keep_refprop=False, solve_with_macro=False,
-            ees_decimal_separator=","
+            ees_decimal_separator=",", display_progress_bar=False
 
     ):
 
         self.__clear_files()
 
         self.__ees_file_path = None
         self.__with_initialization = False
         self.__keep_refprop = keep_refprop
         self.__solve_with_macro = solve_with_macro
         self.__decimal_separator = ees_decimal_separator
+        self.__display_progress_bar = display_progress_bar
 
         if ees_file_path is not None:
             self.ees_file_path = ees_file_path
 
     def __enter__(self):
 
         self.__with_initialization = True
@@ -76,22 +78,31 @@
 
             return self.__direct_calculation_passage(input_list)
 
         elif type(input_list) == dict:
 
             return_dict = dict()
 
+            if self.__display_progress_bar:
+                pbar = tqdm(desc="EES Calculation Ongoing", total=len(input_list.keys()))
+
             for key in input_list.keys():
 
                 return_dict.update({
 
                     key: self.__direct_calculation_passage(input_list[key])
 
                 })
 
+                if self.__display_progress_bar:
+                    pbar.update(1)
+
+            if self.__display_progress_bar:
+                pbar.close()
+
             return return_dict
 
         else:
 
             return None
 
     def __direct_calculation_passage(self, input_list):
```

### Comparing `EES_connector-0.3.3/EESConnect/constants.py` & `EES_connector-0.3.4/EESConnect/constants.py`

 * *Files identical despite different names*

### Comparing `EES_connector-0.3.3/EES_connector.egg-info/PKG-INFO` & `EES_connector-0.3.4/EES_connector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EES-connector
-Version: 0.3.3
+Version: 0.3.4
 Summary: Tools for launching EES calculation and retrieving results from python
 Home-page: https://www.dief.unifi.it/vp-177-serg-group-english-version.html
 Download-URL: https://github.com/SERGGroup/EESConnector/archive/refs/tags/0.2.5.tar.gz
 Author: Pietro Ungar
 Author-email: pietro.ungar@unifi.it
 License: GNU GPLv3
 Project-URL: Source, https://github.com/SERGGroup/EESConnector
```

### Comparing `EES_connector-0.3.3/LICENSE` & `EES_connector-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `EES_connector-0.3.3/PKG-INFO` & `EES_connector-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EES_connector
-Version: 0.3.3
+Version: 0.3.4
 Summary: Tools for launching EES calculation and retrieving results from python
 Home-page: https://www.dief.unifi.it/vp-177-serg-group-english-version.html
 Download-URL: https://github.com/SERGGroup/EESConnector/archive/refs/tags/0.2.5.tar.gz
 Author: Pietro Ungar
 Author-email: pietro.ungar@unifi.it
 License: GNU GPLv3
 Project-URL: Source, https://github.com/SERGGroup/EESConnector
```

### Comparing `EES_connector-0.3.3/README.md` & `EES_connector-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `EES_connector-0.3.3/setup.py` & `EES_connector-0.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
 
     name='EES_connector',
-    version='0.3.3',
+    version='0.3.4',
     license='GNU GPLv3',
 
     author='Pietro Ungar',
     author_email='pietro.ungar@unifi.it',
 
     description='Tools for launching EES calculation and retrieving results from python',
     long_description=long_description,
```

