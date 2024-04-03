# Comparing `tmp/pyscreeps-arena-0.1.6.tar.gz` & `tmp/pyscreeps-arena-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscreeps-arena-0.1.6.tar", last modified: Wed Apr  3 05:21:26 2024, max compression
+gzip compressed data, was "pyscreeps-arena-0.1.7.tar", last modified: Wed Apr  3 05:33:11 2024, max compression
```

## Comparing `pyscreeps-arena-0.1.6.tar` & `pyscreeps-arena-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 05:21:26.330000 pyscreeps-arena-0.1.6/
--rw-rw-rw-   0        0        0      672 2024-04-03 05:21:28.000000 pyscreeps-arena-0.1.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-03 05:21:26.340000 pyscreeps-arena-0.1.6/pyscreeps-arena/
--rw-rw-rw-   0        0        0      749 2024-04-03 05:19:58.000000 pyscreeps-arena-0.1.6/pyscreeps-arena/__init__.py
--rw-rw-rw-   0        0        0    69012 2024-04-03 05:19:44.000000 pyscreeps-arena-0.1.6/pyscreeps-arena/project.7z
-drwxrwxrwx   0        0        0        0 2024-04-03 05:21:26.350000 pyscreeps-arena-0.1.6/pyscreeps_arena.egg-info/
--rw-rw-rw-   0        0        0      672 2024-04-03 05:21:28.000000 pyscreeps-arena-0.1.6/pyscreeps_arena.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2024-04-03 05:21:28.000000 pyscreeps-arena-0.1.6/pyscreeps_arena.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 05:21:28.000000 pyscreeps-arena-0.1.6/pyscreeps_arena.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2024-04-03 05:21:28.000000 pyscreeps-arena-0.1.6/pyscreeps_arena.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       87 2024-04-03 05:21:28.000000 pyscreeps-arena-0.1.6/pyscreeps_arena.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-03 05:21:28.000000 pyscreeps-arena-0.1.6/pyscreeps_arena.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 05:21:28.000000 pyscreeps-arena-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1230 2024-04-03 05:21:12.000000 pyscreeps-arena-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 05:33:11.170000 pyscreeps-arena-0.1.7/
+-rw-rw-rw-   0        0        0      672 2024-04-03 05:33:12.000000 pyscreeps-arena-0.1.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-03 05:33:11.180000 pyscreeps-arena-0.1.7/pyscreeps_arena/
+-rw-rw-rw-   0        0        0      749 2024-04-03 05:26:32.000000 pyscreeps-arena-0.1.7/pyscreeps_arena/__init__.py
+-rw-rw-rw-   0        0        0    69012 2024-04-03 05:26:32.000000 pyscreeps-arena-0.1.7/pyscreeps_arena/project.7z
+drwxrwxrwx   0        0        0        0 2024-04-03 05:33:11.180000 pyscreeps-arena-0.1.7/pyscreeps_arena.egg-info/
+-rw-rw-rw-   0        0        0      672 2024-04-03 05:33:12.000000 pyscreeps-arena-0.1.7/pyscreeps_arena.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2024-04-03 05:33:12.000000 pyscreeps-arena-0.1.7/pyscreeps_arena.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 05:33:12.000000 pyscreeps-arena-0.1.7/pyscreeps_arena.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2024-04-03 05:33:12.000000 pyscreeps-arena-0.1.7/pyscreeps_arena.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       87 2024-04-03 05:33:12.000000 pyscreeps-arena-0.1.7/pyscreeps_arena.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-03 05:33:12.000000 pyscreeps-arena-0.1.7/pyscreeps_arena.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-03 05:33:12.000000 pyscreeps-arena-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1230 2024-04-03 05:32:58.000000 pyscreeps-arena-0.1.7/setup.py
```

### Comparing `pyscreeps-arena-0.1.6/PKG-INFO` & `pyscreeps-arena-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscreeps-arena
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python api|interface to play steam game: Screeps: Arena.
 Author-email: 2229066748@qq.com
 Maintainer: Eagle'sBaby
 Maintainer-email: 2229066748@qq.com
 License: Apache Licence 2.0
 Keywords: python,screeps:arena,screeps
 Classifier: Programming Language :: Python
```

### Comparing `pyscreeps-arena-0.1.6/pyscreeps-arena/__init__.py` & `pyscreeps-arena-0.1.7/pyscreeps_arena/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscreeps-arena-0.1.6/pyscreeps-arena/project.7z` & `pyscreeps-arena-0.1.7/pyscreeps_arena/project.7z`

 * *Files identical despite different names*

### Comparing `pyscreeps-arena-0.1.6/pyscreeps_arena.egg-info/PKG-INFO` & `pyscreeps-arena-0.1.7/pyscreeps_arena.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscreeps-arena
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python api|interface to play steam game: Screeps: Arena.
 Author-email: 2229066748@qq.com
 Maintainer: Eagle'sBaby
 Maintainer-email: 2229066748@qq.com
 License: Apache Licence 2.0
 Keywords: python,screeps:arena,screeps
 Classifier: Programming Language :: Python
```

### Comparing `pyscreeps-arena-0.1.6/setup.py` & `pyscreeps-arena-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 from setuptools import setup, find_packages
 
 with open(r"T:\New_PC\Import_Project\uploads\pyscreeps-arena_upload\pyscreeps-arena.md", 'r') as f:
     long_description = f.read()
 setup(
     name='pyscreeps-arena',
-    version='0.1.6',
+    version='0.1.7',
     description='Python api|interface to play steam game: Screeps: Arena.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author_email='2229066748@qq.com',
     maintainer="Eagle'sBaby",
     maintainer_email='2229066748@qq.com',
     packages=find_packages(),
```

