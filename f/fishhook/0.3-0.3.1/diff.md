# Comparing `tmp/fishhook-0.3.tar.gz` & `tmp/fishhook-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fishhook-0.3.tar", last modified: Wed Apr  3 01:53:49 2024, max compression
+gzip compressed data, was "fishhook-0.3.1.tar", last modified: Wed Apr  3 19:50:40 2024, max compression
```

## Comparing `fishhook-0.3.tar` & `fishhook-0.3.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 chilaxan   (501) staff       (20)        0 2024-04-03 01:53:49.003678 fishhook-0.3/
--rw-r--r--   0 chilaxan   (501) staff       (20)     1065 2023-02-05 02:31:28.000000 fishhook-0.3/LICENSE
--rw-r--r--   0 chilaxan   (501) staff       (20)     2378 2024-04-03 01:53:49.003399 fishhook-0.3/PKG-INFO
--rw-r--r--   0 chilaxan   (501) staff       (20)     1881 2024-04-03 01:45:54.000000 fishhook-0.3/README.md
-drwxr-xr-x   0 chilaxan   (501) staff       (20)        0 2024-04-03 01:53:49.002057 fishhook-0.3/fishhook/
--rw-r--r--   0 chilaxan   (501) staff       (20)      601 2023-08-24 22:03:59.000000 fishhook-0.3/fishhook/__init__.py
--rw-r--r--   0 chilaxan   (501) staff       (20)     3639 2024-04-03 00:58:11.000000 fishhook-0.3/fishhook/_asmmodule.c
--rw-r--r--   0 chilaxan   (501) staff       (20)     3592 2024-04-03 01:02:38.000000 fishhook-0.3/fishhook/asm.py
--rw-r--r--   0 chilaxan   (501) staff       (20)    16540 2023-08-10 03:41:07.000000 fishhook-0.3/fishhook/fishhook.py
--rw-r--r--   0 chilaxan   (501) staff       (20)     3609 2023-08-10 03:42:20.000000 fishhook-0.3/fishhook/tests.py
-drwxr-xr-x   0 chilaxan   (501) staff       (20)        0 2024-04-03 01:53:49.003114 fishhook-0.3/fishhook.egg-info/
--rw-r--r--   0 chilaxan   (501) staff       (20)     2378 2024-04-03 01:53:48.000000 fishhook-0.3/fishhook.egg-info/PKG-INFO
--rw-r--r--   0 chilaxan   (501) staff       (20)      283 2024-04-03 01:53:48.000000 fishhook-0.3/fishhook.egg-info/SOURCES.txt
--rw-r--r--   0 chilaxan   (501) staff       (20)        1 2024-04-03 01:53:48.000000 fishhook-0.3/fishhook.egg-info/dependency_links.txt
--rw-r--r--   0 chilaxan   (501) staff       (20)       25 2024-04-03 01:53:48.000000 fishhook-0.3/fishhook.egg-info/requires.txt
--rw-r--r--   0 chilaxan   (501) staff       (20)        9 2024-04-03 01:53:48.000000 fishhook-0.3/fishhook.egg-info/top_level.txt
--rw-r--r--   0 chilaxan   (501) staff       (20)       38 2024-04-03 01:53:49.003743 fishhook-0.3/setup.cfg
--rw-r--r--   0 chilaxan   (501) staff       (20)      789 2024-04-03 01:39:01.000000 fishhook-0.3/setup.py
+drwxr-xr-x   0 chilaxan   (501) staff       (20)        0 2024-04-03 19:50:40.108704 fishhook-0.3.1/
+-rw-r--r--   0 chilaxan   (501) staff       (20)     1065 2023-02-05 02:31:28.000000 fishhook-0.3.1/LICENSE
+-rw-r--r--   0 chilaxan   (501) staff       (20)     2380 2024-04-03 19:50:40.108511 fishhook-0.3.1/PKG-INFO
+-rw-r--r--   0 chilaxan   (501) staff       (20)     1881 2024-04-03 01:45:54.000000 fishhook-0.3.1/README.md
+drwxr-xr-x   0 chilaxan   (501) staff       (20)        0 2024-04-03 19:50:40.107359 fishhook-0.3.1/fishhook/
+-rw-r--r--   0 chilaxan   (501) staff       (20)      601 2023-08-24 22:03:59.000000 fishhook-0.3.1/fishhook/__init__.py
+-rw-r--r--   0 chilaxan   (501) staff       (20)     3639 2024-04-03 14:19:23.000000 fishhook-0.3.1/fishhook/_asmmodule.c
+-rw-r--r--   0 chilaxan   (501) staff       (20)     2390 2024-04-03 19:48:44.000000 fishhook-0.3.1/fishhook/asm.py
+-rw-r--r--   0 chilaxan   (501) staff       (20)    16540 2023-08-10 03:41:07.000000 fishhook-0.3.1/fishhook/fishhook.py
+-rw-r--r--   0 chilaxan   (501) staff       (20)     2778 2024-04-03 19:49:21.000000 fishhook-0.3.1/fishhook/jit.py
+-rw-r--r--   0 chilaxan   (501) staff       (20)     3609 2023-08-10 03:42:20.000000 fishhook-0.3.1/fishhook/tests.py
+drwxr-xr-x   0 chilaxan   (501) staff       (20)        0 2024-04-03 19:50:40.108277 fishhook-0.3.1/fishhook.egg-info/
+-rw-r--r--   0 chilaxan   (501) staff       (20)     2380 2024-04-03 19:50:40.000000 fishhook-0.3.1/fishhook.egg-info/PKG-INFO
+-rw-r--r--   0 chilaxan   (501) staff       (20)      299 2024-04-03 19:50:40.000000 fishhook-0.3.1/fishhook.egg-info/SOURCES.txt
+-rw-r--r--   0 chilaxan   (501) staff       (20)        1 2024-04-03 19:50:40.000000 fishhook-0.3.1/fishhook.egg-info/dependency_links.txt
+-rw-r--r--   0 chilaxan   (501) staff       (20)       25 2024-04-03 19:50:40.000000 fishhook-0.3.1/fishhook.egg-info/requires.txt
+-rw-r--r--   0 chilaxan   (501) staff       (20)        9 2024-04-03 19:50:40.000000 fishhook-0.3.1/fishhook.egg-info/top_level.txt
+-rw-r--r--   0 chilaxan   (501) staff       (20)       38 2024-04-03 19:50:40.108753 fishhook-0.3.1/setup.cfg
+-rw-r--r--   0 chilaxan   (501) staff       (20)      791 2024-04-03 19:50:15.000000 fishhook-0.3.1/setup.py
```

### Comparing `fishhook-0.3/LICENSE` & `fishhook-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fishhook-0.3/PKG-INFO` & `fishhook-0.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fishhook
-Version: 0.3
+Version: 0.3.1
 Summary: Allows for runtime hooking of static class functions
 Home-page: https://github.com/chilaxan/fishhook
 Author: chilaxan
 Author-email: chilaxan@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fishhook-0.3/README.md` & `fishhook-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `fishhook-0.3/fishhook/__init__.py` & `fishhook-0.3.1/fishhook/__init__.py`

 * *Files identical despite different names*

### Comparing `fishhook-0.3/fishhook/_asmmodule.c` & `fishhook-0.3.1/fishhook/_asmmodule.c`

 * *Files identical despite different names*

### Comparing `fishhook-0.3/fishhook/fishhook.py` & `fishhook-0.3.1/fishhook/fishhook.py`

 * *Files identical despite different names*

### Comparing `fishhook-0.3/fishhook/tests.py` & `fishhook-0.3.1/fishhook/tests.py`

 * *Files identical despite different names*

### Comparing `fishhook-0.3/fishhook.egg-info/PKG-INFO` & `fishhook-0.3.1/fishhook.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fishhook
-Version: 0.3
+Version: 0.3.1
 Summary: Allows for runtime hooking of static class functions
 Home-page: https://github.com/chilaxan/fishhook
 Author: chilaxan
 Author-email: chilaxan@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fishhook-0.3/setup.py` & `fishhook-0.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="fishhook",
-    version="0.3",
+    version="0.3.1",
     author="chilaxan",
     author_email="chilaxan@gmail.com",
     description="Allows for runtime hooking of static class functions",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/chilaxan/fishhook",
     packages=['fishhook'],
```

