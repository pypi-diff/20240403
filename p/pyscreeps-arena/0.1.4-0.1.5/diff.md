# Comparing `tmp/pyscreeps-arena-0.1.4.tar.gz` & `tmp/pyscreeps-arena-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscreeps-arena-0.1.4.tar", last modified: Wed Apr  3 04:38:06 2024, max compression
+gzip compressed data, was "pyscreeps-arena-0.1.5.tar", last modified: Wed Apr  3 04:52:17 2024, max compression
```

## Comparing `pyscreeps-arena-0.1.4.tar` & `pyscreeps-arena-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 04:38:06.270000 pyscreeps-arena-0.1.4/
--rw-rw-rw-   0        0        0      650 2024-04-03 04:38:08.000000 pyscreeps-arena-0.1.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-03 04:38:06.280000 pyscreeps-arena-0.1.4/pyscreeps-arena/
--rw-rw-rw-   0        0        0      791 2024-04-03 03:59:38.000000 pyscreeps-arena-0.1.4/pyscreeps-arena/__init__.py
--rw-rw-rw-   0        0        0    20454 2024-04-03 02:55:00.000000 pyscreeps-arena-0.1.4/pyscreeps-arena/build.py
-drwxrwxrwx   0        0        0        0 2024-04-03 04:38:06.290000 pyscreeps-arena-0.1.4/pyscreeps_arena.egg-info/
--rw-rw-rw-   0        0        0      650 2024-04-03 04:38:08.000000 pyscreeps-arena-0.1.4/pyscreeps_arena.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      297 2024-04-03 04:38:08.000000 pyscreeps-arena-0.1.4/pyscreeps_arena.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 04:38:08.000000 pyscreeps-arena-0.1.4/pyscreeps_arena.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2024-04-03 04:38:08.000000 pyscreeps-arena-0.1.4/pyscreeps_arena.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       81 2024-04-03 04:38:08.000000 pyscreeps-arena-0.1.4/pyscreeps_arena.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-03 04:38:08.000000 pyscreeps-arena-0.1.4/pyscreeps_arena.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 04:38:08.000000 pyscreeps-arena-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1161 2024-04-03 04:37:54.000000 pyscreeps-arena-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 04:52:17.400000 pyscreeps-arena-0.1.5/
+-rw-rw-rw-   0        0        0      650 2024-04-03 04:52:18.000000 pyscreeps-arena-0.1.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-03 04:52:17.410000 pyscreeps-arena-0.1.5/pyscreeps_arena.egg-info/
+-rw-rw-rw-   0        0        0      650 2024-04-03 04:52:18.000000 pyscreeps-arena-0.1.5/pyscreeps_arena.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2024-04-03 04:52:18.000000 pyscreeps-arena-0.1.5/pyscreeps_arena.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 04:52:18.000000 pyscreeps-arena-0.1.5/pyscreeps_arena.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2024-04-03 04:52:18.000000 pyscreeps-arena-0.1.5/pyscreeps_arena.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       81 2024-04-03 04:52:18.000000 pyscreeps-arena-0.1.5/pyscreeps_arena.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 04:52:18.000000 pyscreeps-arena-0.1.5/pyscreeps_arena.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-03 04:52:18.000000 pyscreeps-arena-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1364 2024-04-03 04:52:06.000000 pyscreeps-arena-0.1.5/setup.py
```

### Comparing `pyscreeps-arena-0.1.4/setup.py` & `pyscreeps-arena-0.1.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,22 +3,30 @@
 import os
 from setuptools import setup, find_packages
 
 with open(r"T:\New_PC\Import_Project\uploads\pyscreeps-arena_upload\pyscreeps-arena.md", 'r') as f:
     long_description = f.read()
 setup(
     name='pyscreeps-arena',
-    version='0.1.4',
+    version='0.1.5',
     description='Python api|interface to play steam game: Screeps: Arena.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author_email='2229066748@qq.com',
     maintainer="Eagle'sBaby",
     maintainer_email='2229066748@qq.com',
     packages=find_packages(),
+    package_data={
+        'src': ['*.py'],
+        'game': ['*.py'],
+        'docs': ['*.md'],
+        'docs/game': ['*.md'],
+        'docs/src': ['*.md'],
+        '': ['*.yml', '*.py'],
+    },
     license='Apache Licence 2.0',
     classifiers=[
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
     ],
     entry_points={
         'console_scripts': [
```

