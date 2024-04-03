# Comparing `tmp/basefunctions-0.3.7.tar.gz` & `tmp/basefunctions-0.3.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basefunctions-0.3.7.tar", last modified: Tue Apr  2 18:09:34 2024, max compression
+gzip compressed data, was "basefunctions-0.3.7.1.tar", last modified: Wed Apr  3 19:28:18 2024, max compression
```

## Comparing `basefunctions-0.3.7.tar` & `basefunctions-0.3.7.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-02 18:09:34.223413 basefunctions-0.3.7/
--rw-r--r--   0 neutro2    (501) staff       (20)     7051 2024-04-02 18:09:34.222602 basefunctions-0.3.7/PKG-INFO
--rw-r--r--   0 neutro2    (501) staff       (20)     1074 2024-03-22 21:23:12.000000 basefunctions-0.3.7/license
--rw-r--r--   0 neutro2    (501) staff       (20)     1068 2024-03-29 12:54:00.000000 basefunctions-0.3.7/pyproject.toml
--rw-r--r--   0 neutro2    (501) staff       (20)     5040 2024-03-24 19:45:37.000000 basefunctions-0.3.7/readme.md
--rw-r--r--   0 neutro2    (501) staff       (20)       38 2024-04-02 18:09:34.223556 basefunctions-0.3.7/setup.cfg
-drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-02 18:09:34.210922 basefunctions-0.3.7/src/
-drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-02 18:09:34.216618 basefunctions-0.3.7/src/basefunctions/
--rw-r--r--   0 neutro2    (501) staff       (20)     2502 2024-03-28 15:03:07.000000 basefunctions-0.3.7/src/basefunctions/__init__.py
--rw-r--r--   0 neutro2    (501) staff       (20)     5349 2024-04-02 17:30:05.000000 basefunctions-0.3.7/src/basefunctions/database.py
--rw-r--r--   0 neutro2    (501) staff       (20)    14876 2024-03-22 21:23:12.000000 basefunctions-0.3.7/src/basefunctions/filefunctions.py
--rw-r--r--   0 neutro2    (501) staff       (20)    17600 2024-03-29 20:35:19.000000 basefunctions-0.3.7/src/basefunctions/threadpool.py
-drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-02 18:09:34.221340 basefunctions-0.3.7/src/basefunctions.egg-info/
--rw-r--r--   0 neutro2    (501) staff       (20)     7051 2024-04-02 18:09:34.000000 basefunctions-0.3.7/src/basefunctions.egg-info/PKG-INFO
--rw-r--r--   0 neutro2    (501) staff       (20)      409 2024-04-02 18:09:34.000000 basefunctions-0.3.7/src/basefunctions.egg-info/SOURCES.txt
--rw-r--r--   0 neutro2    (501) staff       (20)        1 2024-04-02 18:09:34.000000 basefunctions-0.3.7/src/basefunctions.egg-info/dependency_links.txt
--rw-r--r--   0 neutro2    (501) staff       (20)       97 2024-04-02 18:09:34.000000 basefunctions-0.3.7/src/basefunctions.egg-info/requires.txt
--rw-r--r--   0 neutro2    (501) staff       (20)       14 2024-04-02 18:09:34.000000 basefunctions-0.3.7/src/basefunctions.egg-info/top_level.txt
-drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-02 18:09:34.219979 basefunctions-0.3.7/tests/
--rw-r--r--   0 neutro2    (501) staff       (20)    23668 2024-03-22 21:23:12.000000 basefunctions-0.3.7/tests/test_filefunctions.py
+drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-03 19:28:18.143923 basefunctions-0.3.7.1/
+-rw-r--r--   0 neutro2    (501) staff       (20)     7248 2024-04-03 19:28:18.142898 basefunctions-0.3.7.1/PKG-INFO
+-rw-r--r--   0 neutro2    (501) staff       (20)     1074 2024-03-22 21:23:12.000000 basefunctions-0.3.7.1/license
+-rw-r--r--   0 neutro2    (501) staff       (20)     1070 2024-04-03 19:25:39.000000 basefunctions-0.3.7.1/pyproject.toml
+-rw-r--r--   0 neutro2    (501) staff       (20)     5231 2024-04-03 19:23:19.000000 basefunctions-0.3.7.1/readme.md
+-rw-r--r--   0 neutro2    (501) staff       (20)       38 2024-04-03 19:28:18.144083 basefunctions-0.3.7.1/setup.cfg
+drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-03 19:28:18.129774 basefunctions-0.3.7.1/src/
+drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-03 19:28:18.135901 basefunctions-0.3.7.1/src/basefunctions/
+-rw-r--r--   0 neutro2    (501) staff       (20)     2502 2024-03-28 15:03:07.000000 basefunctions-0.3.7.1/src/basefunctions/__init__.py
+-rw-r--r--   0 neutro2    (501) staff       (20)     5349 2024-04-02 17:30:05.000000 basefunctions-0.3.7.1/src/basefunctions/database.py
+-rw-r--r--   0 neutro2    (501) staff       (20)    14876 2024-03-22 21:23:12.000000 basefunctions-0.3.7.1/src/basefunctions/filefunctions.py
+-rw-r--r--   0 neutro2    (501) staff       (20)    17600 2024-03-29 20:35:19.000000 basefunctions-0.3.7.1/src/basefunctions/threadpool.py
+drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-03 19:28:18.141744 basefunctions-0.3.7.1/src/basefunctions.egg-info/
+-rw-r--r--   0 neutro2    (501) staff       (20)     7248 2024-04-03 19:28:18.000000 basefunctions-0.3.7.1/src/basefunctions.egg-info/PKG-INFO
+-rw-r--r--   0 neutro2    (501) staff       (20)      409 2024-04-03 19:28:18.000000 basefunctions-0.3.7.1/src/basefunctions.egg-info/SOURCES.txt
+-rw-r--r--   0 neutro2    (501) staff       (20)        1 2024-04-03 19:28:18.000000 basefunctions-0.3.7.1/src/basefunctions.egg-info/dependency_links.txt
+-rw-r--r--   0 neutro2    (501) staff       (20)       97 2024-04-03 19:28:18.000000 basefunctions-0.3.7.1/src/basefunctions.egg-info/requires.txt
+-rw-r--r--   0 neutro2    (501) staff       (20)       14 2024-04-03 19:28:18.000000 basefunctions-0.3.7.1/src/basefunctions.egg-info/top_level.txt
+drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-03 19:28:18.139763 basefunctions-0.3.7.1/tests/
+-rw-r--r--   0 neutro2    (501) staff       (20)    23668 2024-03-22 21:23:12.000000 basefunctions-0.3.7.1/tests/test_filefunctions.py
```

### Comparing `basefunctions-0.3.7/PKG-INFO` & `basefunctions-0.3.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basefunctions
-Version: 0.3.7
+Version: 0.3.7.1
 Summary: simple library to have some commonly used functions for everyday purpose
 Author-email: NeuralDevelopment <neutro2@outlook.de>
 License: MIT License
         
         Copyright (c) 2023 NeuralDevelopment
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -72,14 +72,16 @@
 
 bf.get_current_directory()
 /Users/neutro2/
 ```
 
 ## Using threadpool class
 
+The code below is a small example of the threadpool usage. If you want to see more complex examples on how to use the threadpool, please see package <https://pypi.org/project/eod2pd/> where I've used the framework in order to speed up the downloads.
+
 ```python
 """
     Summary:
     This script demonstrates the usage of the basefunctions module to create a
     ThreadPool and execute tasks concurrently.
 
     It defines two classes A & B of ThreadPoolUserObjects which contains the working functions
@@ -187,20 +189,14 @@
 basefunctions.default_threadpool.get_input_queue().put(msg1)
 basefunctions.default_threadpool.get_input_queue().put(msg2)
 basefunctions.default_threadpool.get_input_queue().put(msg3)
 basefunctions.default_threadpool.get_input_queue().join()
 print("finished")
 ```
 
-## Installation
-
-```bash
-pip install basefunctions
-```
-
 ## Project Homepage
 
 <https://dev.azure.com/neuraldevelopment/basefunctions>
 
 ## Contribute
 
 If you find a defect or suggest a new function, please send an eMail to <neutro2@outlook.de>
```

### Comparing `basefunctions-0.3.7/license` & `basefunctions-0.3.7.1/license`

 * *Files identical despite different names*

### Comparing `basefunctions-0.3.7/pyproject.toml` & `basefunctions-0.3.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "basefunctions"
-version = "0.3.7"
+version = "0.3.7.1"
 
 authors = [{ name = "NeuralDevelopment", email = "neutro2@outlook.de" }]
 description = "simple library to have some commonly used functions for everyday purpose"
 
 readme = "readme.md"
 license = { file = "license" }
 requires-python = ">=3.9"
```

### Comparing `basefunctions-0.3.7/readme.md` & `basefunctions-0.3.7.1/readme.md`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 
 bf.get_current_directory()
 /Users/neutro2/
 ```
 
 ## Using threadpool class
 
+The code below is a small example of the threadpool usage. If you want to see more complex examples on how to use the threadpool, please see package <https://pypi.org/project/eod2pd/> where I've used the framework in order to speed up the downloads.
+
 ```python
 """
     Summary:
     This script demonstrates the usage of the basefunctions module to create a
     ThreadPool and execute tasks concurrently.
 
     It defines two classes A & B of ThreadPoolUserObjects which contains the working functions
@@ -141,20 +143,14 @@
 basefunctions.default_threadpool.get_input_queue().put(msg1)
 basefunctions.default_threadpool.get_input_queue().put(msg2)
 basefunctions.default_threadpool.get_input_queue().put(msg3)
 basefunctions.default_threadpool.get_input_queue().join()
 print("finished")
 ```
 
-## Installation
-
-```bash
-pip install basefunctions
-```
-
 ## Project Homepage
 
 <https://dev.azure.com/neuraldevelopment/basefunctions>
 
 ## Contribute
 
 If you find a defect or suggest a new function, please send an eMail to <neutro2@outlook.de>
```

### Comparing `basefunctions-0.3.7/src/basefunctions/__init__.py` & `basefunctions-0.3.7.1/src/basefunctions/__init__.py`

 * *Files identical despite different names*

### Comparing `basefunctions-0.3.7/src/basefunctions/database.py` & `basefunctions-0.3.7.1/src/basefunctions/database.py`

 * *Files identical despite different names*

### Comparing `basefunctions-0.3.7/src/basefunctions/filefunctions.py` & `basefunctions-0.3.7.1/src/basefunctions/filefunctions.py`

 * *Files identical despite different names*

### Comparing `basefunctions-0.3.7/src/basefunctions/threadpool.py` & `basefunctions-0.3.7.1/src/basefunctions/threadpool.py`

 * *Files identical despite different names*

### Comparing `basefunctions-0.3.7/src/basefunctions.egg-info/PKG-INFO` & `basefunctions-0.3.7.1/src/basefunctions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basefunctions
-Version: 0.3.7
+Version: 0.3.7.1
 Summary: simple library to have some commonly used functions for everyday purpose
 Author-email: NeuralDevelopment <neutro2@outlook.de>
 License: MIT License
         
         Copyright (c) 2023 NeuralDevelopment
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -72,14 +72,16 @@
 
 bf.get_current_directory()
 /Users/neutro2/
 ```
 
 ## Using threadpool class
 
+The code below is a small example of the threadpool usage. If you want to see more complex examples on how to use the threadpool, please see package <https://pypi.org/project/eod2pd/> where I've used the framework in order to speed up the downloads.
+
 ```python
 """
     Summary:
     This script demonstrates the usage of the basefunctions module to create a
     ThreadPool and execute tasks concurrently.
 
     It defines two classes A & B of ThreadPoolUserObjects which contains the working functions
@@ -187,20 +189,14 @@
 basefunctions.default_threadpool.get_input_queue().put(msg1)
 basefunctions.default_threadpool.get_input_queue().put(msg2)
 basefunctions.default_threadpool.get_input_queue().put(msg3)
 basefunctions.default_threadpool.get_input_queue().join()
 print("finished")
 ```
 
-## Installation
-
-```bash
-pip install basefunctions
-```
-
 ## Project Homepage
 
 <https://dev.azure.com/neuraldevelopment/basefunctions>
 
 ## Contribute
 
 If you find a defect or suggest a new function, please send an eMail to <neutro2@outlook.de>
```

### Comparing `basefunctions-0.3.7/tests/test_filefunctions.py` & `basefunctions-0.3.7.1/tests/test_filefunctions.py`

 * *Files identical despite different names*

