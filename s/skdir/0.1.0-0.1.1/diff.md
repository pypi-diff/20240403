# Comparing `tmp/skdir-0.1.0.tar.gz` & `tmp/skdir-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skdir-0.1.0.tar", last modified: Wed Apr  3 19:02:21 2024, max compression
+gzip compressed data, was "skdir-0.1.1.tar", last modified: Wed Apr  3 19:06:32 2024, max compression
```

## Comparing `skdir-0.1.0.tar` & `skdir-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 sharathchandrak   (501) staff       (20)        0 2024-04-03 19:02:21.016141 skdir-0.1.0/
--rw-rw-r--   0 sharathchandrak   (501) staff       (20)     1064 2021-07-27 04:28:46.000000 skdir-0.1.0/LICENSE
--rw-r--r--   0 sharathchandrak   (501) staff       (20)      620 2024-04-03 19:02:21.015938 skdir-0.1.0/PKG-INFO
--rw-rw-r--   0 sharathchandrak   (501) staff       (20)      981 2021-07-27 04:28:46.000000 skdir-0.1.0/README.md
-drwxr-xr-x   0 sharathchandrak   (501) staff       (20)        0 2024-04-03 19:02:21.014691 skdir-0.1.0/lab/
--rw-r--r--   0 sharathchandrak   (501) staff       (20)      680 2024-04-03 18:46:31.000000 skdir-0.1.0/lab/__init__.py
--rw-rw-r--   0 sharathchandrak   (501) staff       (20)     2873 2024-04-03 16:35:15.000000 skdir-0.1.0/lab/p1.py
--rw-rw-r--   0 sharathchandrak   (501) staff       (20)      985 2024-04-03 16:35:24.000000 skdir-0.1.0/lab/p2.py
--rw-rw-r--   0 sharathchandrak   (501) staff       (20)     4208 2024-04-03 16:35:34.000000 skdir-0.1.0/lab/p3.py
--rw-r--r--   0 sharathchandrak   (501) staff       (20)     1701 2024-04-03 16:36:03.000000 skdir-0.1.0/lab/p4.py
--rw-r--r--   0 sharathchandrak   (501) staff       (20)     1808 2024-04-03 16:36:40.000000 skdir-0.1.0/lab/p5.py
--rw-r--r--   0 sharathchandrak   (501) staff       (20)     1798 2024-04-03 16:36:57.000000 skdir-0.1.0/lab/p6.py
--rw-r--r--   0 sharathchandrak   (501) staff       (20)     1869 2024-04-03 16:37:20.000000 skdir-0.1.0/lab/p7.py
--rw-r--r--   0 sharathchandrak   (501) staff       (20)     1111 2024-04-03 16:38:04.000000 skdir-0.1.0/lab/p8.py
--rw-r--r--   0 sharathchandrak   (501) staff       (20)       38 2024-04-03 19:02:21.016221 skdir-0.1.0/setup.cfg
--rw-rw-r--   0 sharathchandrak   (501) staff       (20)      930 2024-04-03 18:46:47.000000 skdir-0.1.0/setup.py
-drwxr-xr-x   0 sharathchandrak   (501) staff       (20)        0 2024-04-03 19:02:21.015664 skdir-0.1.0/skdir.egg-info/
--rw-r--r--   0 sharathchandrak   (501) staff       (20)      620 2024-04-03 19:02:21.000000 skdir-0.1.0/skdir.egg-info/PKG-INFO
--rw-r--r--   0 sharathchandrak   (501) staff       (20)      266 2024-04-03 19:02:21.000000 skdir-0.1.0/skdir.egg-info/SOURCES.txt
--rw-r--r--   0 sharathchandrak   (501) staff       (20)        1 2024-04-03 19:02:21.000000 skdir-0.1.0/skdir.egg-info/dependency_links.txt
--rw-r--r--   0 sharathchandrak   (501) staff       (20)       53 2024-04-03 19:02:21.000000 skdir-0.1.0/skdir.egg-info/requires.txt
--rw-r--r--   0 sharathchandrak   (501) staff       (20)        4 2024-04-03 19:02:21.000000 skdir-0.1.0/skdir.egg-info/top_level.txt
+drwxr-xr-x   0 sharathchandrak   (501) staff       (20)        0 2024-04-03 19:06:32.795573 skdir-0.1.1/
+-rw-rw-r--   0 sharathchandrak   (501) staff       (20)     1064 2021-07-27 04:28:46.000000 skdir-0.1.1/LICENSE
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)      620 2024-04-03 19:06:32.795316 skdir-0.1.1/PKG-INFO
+-rw-rw-r--   0 sharathchandrak   (501) staff       (20)      981 2021-07-27 04:28:46.000000 skdir-0.1.1/README.md
+drwxr-xr-x   0 sharathchandrak   (501) staff       (20)        0 2024-04-03 19:06:32.793530 skdir-0.1.1/lab/
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)      632 2024-04-03 19:05:40.000000 skdir-0.1.1/lab/__init__.py
+-rw-rw-r--   0 sharathchandrak   (501) staff       (20)     2873 2024-04-03 16:35:15.000000 skdir-0.1.1/lab/p1.py
+-rw-rw-r--   0 sharathchandrak   (501) staff       (20)      985 2024-04-03 16:35:24.000000 skdir-0.1.1/lab/p2.py
+-rw-rw-r--   0 sharathchandrak   (501) staff       (20)     4208 2024-04-03 16:35:34.000000 skdir-0.1.1/lab/p3.py
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)     1701 2024-04-03 16:36:03.000000 skdir-0.1.1/lab/p4.py
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)     1808 2024-04-03 16:36:40.000000 skdir-0.1.1/lab/p5.py
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)     1798 2024-04-03 16:36:57.000000 skdir-0.1.1/lab/p6.py
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)     1869 2024-04-03 16:37:20.000000 skdir-0.1.1/lab/p7.py
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)     1111 2024-04-03 16:38:04.000000 skdir-0.1.1/lab/p8.py
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)       38 2024-04-03 19:06:32.795698 skdir-0.1.1/setup.cfg
+-rw-rw-r--   0 sharathchandrak   (501) staff       (20)      930 2024-04-03 19:06:25.000000 skdir-0.1.1/setup.py
+drwxr-xr-x   0 sharathchandrak   (501) staff       (20)        0 2024-04-03 19:06:32.794819 skdir-0.1.1/skdir.egg-info/
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)      620 2024-04-03 19:06:32.000000 skdir-0.1.1/skdir.egg-info/PKG-INFO
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)      266 2024-04-03 19:06:32.000000 skdir-0.1.1/skdir.egg-info/SOURCES.txt
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)        1 2024-04-03 19:06:32.000000 skdir-0.1.1/skdir.egg-info/dependency_links.txt
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)       53 2024-04-03 19:06:32.000000 skdir-0.1.1/skdir.egg-info/requires.txt
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)        4 2024-04-03 19:06:32.000000 skdir-0.1.1/skdir.egg-info/top_level.txt
```

### Comparing `skdir-0.1.0/LICENSE` & `skdir-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `skdir-0.1.0/PKG-INFO` & `skdir-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skdir
-Version: 0.1.0
+Version: 0.1.1
 Summary: skdir
 Home-page: UNKNOWN
 Author: Sk
 Author-email: karnamsharath3@gmail.com
 License: UNKNOWN
 Keywords: arithmetic,math,mathematics,python tutorial,avi upadhyay
 Platform: UNKNOWN
```

### Comparing `skdir-0.1.0/README.md` & `skdir-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `skdir-0.1.0/lab/__init__.py` & `skdir-0.1.1/lab/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 # __init__.py
 
 # Import any modules or symbols needed for printing the AIML code files
-import os
-import numpy
-import sklearn
-import matplotlib
 
+import os
 # Define the directory path where the AIML code files are located
-AIML_CODE_DIR = ''
+AIML_CODE_DIR = 'lab'
 
 # Function to print the contents of AIML code files
 def print_aiml_code_file(filename):
     file_path = os.path.join(AIML_CODE_DIR, filename)
     if os.path.exists(file_path):
         with open(file_path, 'r') as file:
             print(f"Contents of {filename}:")
             print(file.read())
     else:
         print(f"File {filename} does not exist.")
 def Print(filename):
     print_aiml_code_file(filename)
 # Example usage:
-Print('example.py') 
+Print('p2.py')
```

### Comparing `skdir-0.1.0/lab/p1.py` & `skdir-0.1.1/lab/p1.py`

 * *Files identical despite different names*

### Comparing `skdir-0.1.0/lab/p2.py` & `skdir-0.1.1/lab/p2.py`

 * *Files identical despite different names*

### Comparing `skdir-0.1.0/lab/p3.py` & `skdir-0.1.1/lab/p3.py`

 * *Files identical despite different names*

### Comparing `skdir-0.1.0/lab/p4.py` & `skdir-0.1.1/lab/p4.py`

 * *Files identical despite different names*

### Comparing `skdir-0.1.0/lab/p5.py` & `skdir-0.1.1/lab/p5.py`

 * *Files identical despite different names*

### Comparing `skdir-0.1.0/lab/p6.py` & `skdir-0.1.1/lab/p6.py`

 * *Files identical despite different names*

### Comparing `skdir-0.1.0/lab/p7.py` & `skdir-0.1.1/lab/p7.py`

 * *Files identical despite different names*

### Comparing `skdir-0.1.0/lab/p8.py` & `skdir-0.1.1/lab/p8.py`

 * *Files identical despite different names*

### Comparing `skdir-0.1.0/setup.py` & `skdir-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 DESCRIPTION = 'skdir'
 LONG_DESCRIPTION = 'A package to perform arithmetic operations'
 
 # Setting up
 setup(
     name="skdir",
     version=VERSION,
```

### Comparing `skdir-0.1.0/skdir.egg-info/PKG-INFO` & `skdir-0.1.1/skdir.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skdir
-Version: 0.1.0
+Version: 0.1.1
 Summary: skdir
 Home-page: UNKNOWN
 Author: Sk
 Author-email: karnamsharath3@gmail.com
 License: UNKNOWN
 Keywords: arithmetic,math,mathematics,python tutorial,avi upadhyay
 Platform: UNKNOWN
```

