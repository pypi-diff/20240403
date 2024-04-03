# Comparing `tmp/pyscreeps-arena-0.1.3.tar.gz` & `tmp/pyscreeps-arena-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscreeps-arena-0.1.3.tar", last modified: Wed Apr  3 04:35:43 2024, max compression
+gzip compressed data, was "pyscreeps-arena-0.1.4.tar", last modified: Wed Apr  3 04:38:06 2024, max compression
```

## Comparing `pyscreeps-arena-0.1.3.tar` & `pyscreeps-arena-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 04:35:42.950000 pyscreeps-arena-0.1.3/
--rw-rw-rw-   0        0        0      649 2024-04-03 04:35:44.000000 pyscreeps-arena-0.1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-03 04:35:42.960000 pyscreeps-arena-0.1.3/pyscreeps-arena/
--rw-rw-rw-   0        0        0      791 2024-04-03 03:59:38.000000 pyscreeps-arena-0.1.3/pyscreeps-arena/__init__.py
--rw-rw-rw-   0        0        0    20454 2024-04-03 02:55:00.000000 pyscreeps-arena-0.1.3/pyscreeps-arena/build.py
-drwxrwxrwx   0        0        0        0 2024-04-03 04:35:42.970000 pyscreeps-arena-0.1.3/pyscreeps_arena.egg-info/
--rw-rw-rw-   0        0        0      649 2024-04-03 04:35:44.000000 pyscreeps-arena-0.1.3/pyscreeps_arena.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      297 2024-04-03 04:35:44.000000 pyscreeps-arena-0.1.3/pyscreeps_arena.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 04:35:44.000000 pyscreeps-arena-0.1.3/pyscreeps_arena.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2024-04-03 04:35:44.000000 pyscreeps-arena-0.1.3/pyscreeps_arena.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       80 2024-04-03 04:35:44.000000 pyscreeps-arena-0.1.3/pyscreeps_arena.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-03 04:35:44.000000 pyscreeps-arena-0.1.3/pyscreeps_arena.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 04:35:44.000000 pyscreeps-arena-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1160 2024-04-03 04:35:32.000000 pyscreeps-arena-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 04:38:06.270000 pyscreeps-arena-0.1.4/
+-rw-rw-rw-   0        0        0      650 2024-04-03 04:38:08.000000 pyscreeps-arena-0.1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-03 04:38:06.280000 pyscreeps-arena-0.1.4/pyscreeps-arena/
+-rw-rw-rw-   0        0        0      791 2024-04-03 03:59:38.000000 pyscreeps-arena-0.1.4/pyscreeps-arena/__init__.py
+-rw-rw-rw-   0        0        0    20454 2024-04-03 02:55:00.000000 pyscreeps-arena-0.1.4/pyscreeps-arena/build.py
+drwxrwxrwx   0        0        0        0 2024-04-03 04:38:06.290000 pyscreeps-arena-0.1.4/pyscreeps_arena.egg-info/
+-rw-rw-rw-   0        0        0      650 2024-04-03 04:38:08.000000 pyscreeps-arena-0.1.4/pyscreeps_arena.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      297 2024-04-03 04:38:08.000000 pyscreeps-arena-0.1.4/pyscreeps_arena.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 04:38:08.000000 pyscreeps-arena-0.1.4/pyscreeps_arena.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2024-04-03 04:38:08.000000 pyscreeps-arena-0.1.4/pyscreeps_arena.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       81 2024-04-03 04:38:08.000000 pyscreeps-arena-0.1.4/pyscreeps_arena.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-03 04:38:08.000000 pyscreeps-arena-0.1.4/pyscreeps_arena.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-03 04:38:08.000000 pyscreeps-arena-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1161 2024-04-03 04:37:54.000000 pyscreeps-arena-0.1.4/setup.py
```

### Comparing `pyscreeps-arena-0.1.3/PKG-INFO` & `pyscreeps-arena-0.1.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pyscreeps-arena
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python api|interface to play steam game: Screeps: Arena.
 Author-email: 2229066748@qq.com
 Maintainer: Eagle'sBaby
 Maintainer-email: 2229066748@qq.com
 License: Apache Licence 2.0
 Keywords: python,screeps:arena,screeps
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pyperclip
-Requires-Dist: colorma
+Requires-Dist: colorama
 Requires-Dist: Transcrypt==3.9.1
 Requires-Dist: mkdocs
 Requires-Dist: mkdocstrings[python]
 Requires-Dist: mkdocs-material
 
 # PyScreeps-Arena
```

### Comparing `pyscreeps-arena-0.1.3/pyscreeps-arena/__init__.py` & `pyscreeps-arena-0.1.4/pyscreeps-arena/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscreeps-arena-0.1.3/pyscreeps-arena/build.py` & `pyscreeps-arena-0.1.4/pyscreeps-arena/build.py`

 * *Files identical despite different names*

### Comparing `pyscreeps-arena-0.1.3/pyscreeps_arena.egg-info/PKG-INFO` & `pyscreeps-arena-0.1.4/pyscreeps_arena.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pyscreeps-arena
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python api|interface to play steam game: Screeps: Arena.
 Author-email: 2229066748@qq.com
 Maintainer: Eagle'sBaby
 Maintainer-email: 2229066748@qq.com
 License: Apache Licence 2.0
 Keywords: python,screeps:arena,screeps
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pyperclip
-Requires-Dist: colorma
+Requires-Dist: colorama
 Requires-Dist: Transcrypt==3.9.1
 Requires-Dist: mkdocs
 Requires-Dist: mkdocstrings[python]
 Requires-Dist: mkdocs-material
 
 # PyScreeps-Arena
```

### Comparing `pyscreeps-arena-0.1.3/setup.py` & `pyscreeps-arena-0.1.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 from setuptools import setup, find_packages
 
 with open(r"T:\New_PC\Import_Project\uploads\pyscreeps-arena_upload\pyscreeps-arena.md", 'r') as f:
     long_description = f.read()
 setup(
     name='pyscreeps-arena',
-    version='0.1.3',
+    version='0.1.4',
     description='Python api|interface to play steam game: Screeps: Arena.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author_email='2229066748@qq.com',
     maintainer="Eagle'sBaby",
     maintainer_email='2229066748@qq.com',
     packages=find_packages(),
@@ -25,14 +25,14 @@
             'pyscreeps-arena=pyscreeps_arena:CMD_NewProject',
         ]
     },
     keywords=['python', 'screeps:arena', 'screeps'],
     python_requires='>=3.10',
     install_requires=[
         'pyperclip',
-        'colorma',
+        'colorama',
         'Transcrypt==3.9.1',
         'mkdocs',
         'mkdocstrings[python]',
         'mkdocs-material',
     ],
 )
```

