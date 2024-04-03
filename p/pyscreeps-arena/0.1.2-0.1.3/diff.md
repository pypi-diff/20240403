# Comparing `tmp/pyscreeps-arena-0.1.2.tar.gz` & `tmp/pyscreeps-arena-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscreeps-arena-0.1.2.tar", last modified: Wed Apr  3 04:18:32 2024, max compression
+gzip compressed data, was "pyscreeps-arena-0.1.3.tar", last modified: Wed Apr  3 04:35:43 2024, max compression
```

## Comparing `pyscreeps-arena-0.1.2.tar` & `pyscreeps-arena-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 04:18:32.020000 pyscreeps-arena-0.1.2/
--rw-rw-rw-   0        0        0      652 2024-04-03 04:18:34.000000 pyscreeps-arena-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-03 04:18:32.030000 pyscreeps-arena-0.1.2/pyscreeps-arena/
--rw-rw-rw-   0        0        0      791 2024-04-03 03:59:38.000000 pyscreeps-arena-0.1.2/pyscreeps-arena/__init__.py
--rw-rw-rw-   0        0        0    20454 2024-04-03 02:55:00.000000 pyscreeps-arena-0.1.2/pyscreeps-arena/build.py
-drwxrwxrwx   0        0        0        0 2024-04-03 04:18:32.040000 pyscreeps-arena-0.1.2/pyscreeps_arena.egg-info/
--rw-rw-rw-   0        0        0      652 2024-04-03 04:18:34.000000 pyscreeps-arena-0.1.2/pyscreeps_arena.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      297 2024-04-03 04:18:34.000000 pyscreeps-arena-0.1.2/pyscreeps_arena.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 04:18:34.000000 pyscreeps-arena-0.1.2/pyscreeps_arena.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2024-04-03 04:18:34.000000 pyscreeps-arena-0.1.2/pyscreeps_arena.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       80 2024-04-03 04:18:34.000000 pyscreeps-arena-0.1.2/pyscreeps_arena.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-03 04:18:34.000000 pyscreeps-arena-0.1.2/pyscreeps_arena.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 04:18:34.000000 pyscreeps-arena-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1167 2024-04-03 04:18:22.000000 pyscreeps-arena-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 04:35:42.950000 pyscreeps-arena-0.1.3/
+-rw-rw-rw-   0        0        0      649 2024-04-03 04:35:44.000000 pyscreeps-arena-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-03 04:35:42.960000 pyscreeps-arena-0.1.3/pyscreeps-arena/
+-rw-rw-rw-   0        0        0      791 2024-04-03 03:59:38.000000 pyscreeps-arena-0.1.3/pyscreeps-arena/__init__.py
+-rw-rw-rw-   0        0        0    20454 2024-04-03 02:55:00.000000 pyscreeps-arena-0.1.3/pyscreeps-arena/build.py
+drwxrwxrwx   0        0        0        0 2024-04-03 04:35:42.970000 pyscreeps-arena-0.1.3/pyscreeps_arena.egg-info/
+-rw-rw-rw-   0        0        0      649 2024-04-03 04:35:44.000000 pyscreeps-arena-0.1.3/pyscreeps_arena.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      297 2024-04-03 04:35:44.000000 pyscreeps-arena-0.1.3/pyscreeps_arena.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 04:35:44.000000 pyscreeps-arena-0.1.3/pyscreeps_arena.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2024-04-03 04:35:44.000000 pyscreeps-arena-0.1.3/pyscreeps_arena.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       80 2024-04-03 04:35:44.000000 pyscreeps-arena-0.1.3/pyscreeps_arena.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-03 04:35:44.000000 pyscreeps-arena-0.1.3/pyscreeps_arena.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-03 04:35:44.000000 pyscreeps-arena-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1160 2024-04-03 04:35:32.000000 pyscreeps-arena-0.1.3/setup.py
```

### Comparing `pyscreeps-arena-0.1.2/PKG-INFO` & `pyscreeps-arena-0.1.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pyscreeps-arena
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python api|interface to play steam game: Screeps: Arena.
 Author-email: 2229066748@qq.com
 Maintainer: Eagle'sBaby
 Maintainer-email: 2229066748@qq.com
 License: Apache Licence 2.0
 Keywords: python,screeps:arena,screeps
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pyperclip
 Requires-Dist: colorma
 Requires-Dist: Transcrypt==3.9.1
 Requires-Dist: mkdocs
 Requires-Dist: mkdocstrings[python]
```

### Comparing `pyscreeps-arena-0.1.2/pyscreeps-arena/__init__.py` & `pyscreeps-arena-0.1.3/pyscreeps-arena/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscreeps-arena-0.1.2/pyscreeps-arena/build.py` & `pyscreeps-arena-0.1.3/pyscreeps-arena/build.py`

 * *Files identical despite different names*

### Comparing `pyscreeps-arena-0.1.2/pyscreeps_arena.egg-info/PKG-INFO` & `pyscreeps-arena-0.1.3/pyscreeps_arena.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pyscreeps-arena
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python api|interface to play steam game: Screeps: Arena.
 Author-email: 2229066748@qq.com
 Maintainer: Eagle'sBaby
 Maintainer-email: 2229066748@qq.com
 License: Apache Licence 2.0
 Keywords: python,screeps:arena,screeps
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pyperclip
 Requires-Dist: colorma
 Requires-Dist: Transcrypt==3.9.1
 Requires-Dist: mkdocs
 Requires-Dist: mkdocstrings[python]
```

### Comparing `pyscreeps-arena-0.1.2/setup.py` & `pyscreeps-arena-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 #!/usr/bin/env python
 # coding:utf-8
 import os
 from setuptools import setup, find_packages
 
-
 with open(r"T:\New_PC\Import_Project\uploads\pyscreeps-arena_upload\pyscreeps-arena.md", 'r') as f:
     long_description = f.read()
 setup(
     name='pyscreeps-arena',
-    version='0.1.2',
+    version='0.1.3',
     description='Python api|interface to play steam game: Screeps: Arena.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author_email='2229066748@qq.com',
     maintainer="Eagle'sBaby",
     maintainer_email='2229066748@qq.com',
     packages=find_packages(),
     license='Apache Licence 2.0',
     classifiers=[
         'Programming Language :: Python',
-        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3',
     ],
     entry_points={
         'console_scripts': [
             'pyscreeps-arena=pyscreeps_arena:CMD_NewProject',
         ]
     },
-    keywords = ['python', 'screeps:arena', 'screeps'],
+    keywords=['python', 'screeps:arena', 'screeps'],
     python_requires='>=3.10',
     install_requires=[
         'pyperclip',
         'colorma',
         'Transcrypt==3.9.1',
         'mkdocs',
         'mkdocstrings[python]',
```

