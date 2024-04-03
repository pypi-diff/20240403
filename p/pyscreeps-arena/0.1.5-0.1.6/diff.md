# Comparing `tmp/pyscreeps-arena-0.1.5.tar.gz` & `tmp/pyscreeps-arena-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscreeps-arena-0.1.5.tar", last modified: Wed Apr  3 04:52:17 2024, max compression
+gzip compressed data, was "pyscreeps-arena-0.1.6.tar", last modified: Wed Apr  3 05:21:26 2024, max compression
```

## Comparing `pyscreeps-arena-0.1.5.tar` & `pyscreeps-arena-0.1.6.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 04:52:17.400000 pyscreeps-arena-0.1.5/
--rw-rw-rw-   0        0        0      650 2024-04-03 04:52:18.000000 pyscreeps-arena-0.1.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-03 04:52:17.410000 pyscreeps-arena-0.1.5/pyscreeps_arena.egg-info/
--rw-rw-rw-   0        0        0      650 2024-04-03 04:52:18.000000 pyscreeps-arena-0.1.5/pyscreeps_arena.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2024-04-03 04:52:18.000000 pyscreeps-arena-0.1.5/pyscreeps_arena.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 04:52:18.000000 pyscreeps-arena-0.1.5/pyscreeps_arena.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2024-04-03 04:52:18.000000 pyscreeps-arena-0.1.5/pyscreeps_arena.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       81 2024-04-03 04:52:18.000000 pyscreeps-arena-0.1.5/pyscreeps_arena.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 04:52:18.000000 pyscreeps-arena-0.1.5/pyscreeps_arena.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 04:52:18.000000 pyscreeps-arena-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1364 2024-04-03 04:52:06.000000 pyscreeps-arena-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 05:21:26.330000 pyscreeps-arena-0.1.6/
+-rw-rw-rw-   0        0        0      672 2024-04-03 05:21:28.000000 pyscreeps-arena-0.1.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-03 05:21:26.340000 pyscreeps-arena-0.1.6/pyscreeps-arena/
+-rw-rw-rw-   0        0        0      749 2024-04-03 05:19:58.000000 pyscreeps-arena-0.1.6/pyscreeps-arena/__init__.py
+-rw-rw-rw-   0        0        0    69012 2024-04-03 05:19:44.000000 pyscreeps-arena-0.1.6/pyscreeps-arena/project.7z
+drwxrwxrwx   0        0        0        0 2024-04-03 05:21:26.350000 pyscreeps-arena-0.1.6/pyscreeps_arena.egg-info/
+-rw-rw-rw-   0        0        0      672 2024-04-03 05:21:28.000000 pyscreeps-arena-0.1.6/pyscreeps_arena.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2024-04-03 05:21:28.000000 pyscreeps-arena-0.1.6/pyscreeps_arena.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 05:21:28.000000 pyscreeps-arena-0.1.6/pyscreeps_arena.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2024-04-03 05:21:28.000000 pyscreeps-arena-0.1.6/pyscreeps_arena.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       87 2024-04-03 05:21:28.000000 pyscreeps-arena-0.1.6/pyscreeps_arena.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-03 05:21:28.000000 pyscreeps-arena-0.1.6/pyscreeps_arena.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-03 05:21:28.000000 pyscreeps-arena-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1230 2024-04-03 05:21:12.000000 pyscreeps-arena-0.1.6/setup.py
```

### Comparing `pyscreeps-arena-0.1.5/PKG-INFO` & `pyscreeps-arena-0.1.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: pyscreeps-arena
-Version: 0.1.5
+Version: 0.1.6
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
 Requires-Dist: colorama
+Requires-Dist: py7zr
 Requires-Dist: Transcrypt==3.9.1
 Requires-Dist: mkdocs
 Requires-Dist: mkdocstrings[python]
 Requires-Dist: mkdocs-material
 
 # PyScreeps-Arena
```

### Comparing `pyscreeps-arena-0.1.5/pyscreeps_arena.egg-info/PKG-INFO` & `pyscreeps-arena-0.1.6/pyscreeps_arena.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: pyscreeps-arena
-Version: 0.1.5
+Version: 0.1.6
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
 Requires-Dist: colorama
+Requires-Dist: py7zr
 Requires-Dist: Transcrypt==3.9.1
 Requires-Dist: mkdocs
 Requires-Dist: mkdocstrings[python]
 Requires-Dist: mkdocs-material
 
 # PyScreeps-Arena
```

### Comparing `pyscreeps-arena-0.1.5/setup.py` & `pyscreeps-arena-0.1.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,29 +3,24 @@
 import os
 from setuptools import setup, find_packages
 
 with open(r"T:\New_PC\Import_Project\uploads\pyscreeps-arena_upload\pyscreeps-arena.md", 'r') as f:
     long_description = f.read()
 setup(
     name='pyscreeps-arena',
-    version='0.1.5',
+    version='0.1.6',
     description='Python api|interface to play steam game: Screeps: Arena.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author_email='2229066748@qq.com',
     maintainer="Eagle'sBaby",
     maintainer_email='2229066748@qq.com',
     packages=find_packages(),
     package_data={
-        'src': ['*.py'],
-        'game': ['*.py'],
-        'docs': ['*.md'],
-        'docs/game': ['*.md'],
-        'docs/src': ['*.md'],
-        '': ['*.yml', '*.py'],
+        '': ['*.7z'],
     },
     license='Apache Licence 2.0',
     classifiers=[
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
     ],
     entry_points={
@@ -34,13 +29,14 @@
         ]
     },
     keywords=['python', 'screeps:arena', 'screeps'],
     python_requires='>=3.10',
     install_requires=[
         'pyperclip',
         'colorama',
+        'py7zr',
         'Transcrypt==3.9.1',
         'mkdocs',
         'mkdocstrings[python]',
         'mkdocs-material',
     ],
 )
```

