# Comparing `tmp/pyscreeps-arena-0.1.1.tar.gz` & `tmp/pyscreeps-arena-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscreeps-arena-0.1.1.tar", last modified: Wed Apr  3 04:11:46 2024, max compression
+gzip compressed data, was "pyscreeps-arena-0.1.2.tar", last modified: Wed Apr  3 04:18:32 2024, max compression
```

## Comparing `pyscreeps-arena-0.1.1.tar` & `pyscreeps-arena-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 04:11:46.790000 pyscreeps-arena-0.1.1/
--rw-rw-rw-   0        0        0      652 2024-04-03 04:11:48.000000 pyscreeps-arena-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-03 04:11:46.800000 pyscreeps-arena-0.1.1/pyscreeps-arena/
--rw-rw-rw-   0        0        0      791 2024-04-03 03:59:38.000000 pyscreeps-arena-0.1.1/pyscreeps-arena/__init__.py
--rw-rw-rw-   0        0        0    20454 2024-04-03 02:55:00.000000 pyscreeps-arena-0.1.1/pyscreeps-arena/build.py
-drwxrwxrwx   0        0        0        0 2024-04-03 04:11:46.810000 pyscreeps-arena-0.1.1/pyscreeps_arena.egg-info/
--rw-rw-rw-   0        0        0      652 2024-04-03 04:11:48.000000 pyscreeps-arena-0.1.1/pyscreeps_arena.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2024-04-03 04:11:48.000000 pyscreeps-arena-0.1.1/pyscreeps_arena.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 04:11:48.000000 pyscreeps-arena-0.1.1/pyscreeps_arena.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-04-03 04:11:48.000000 pyscreeps-arena-0.1.1/pyscreeps_arena.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-03 04:11:48.000000 pyscreeps-arena-0.1.1/pyscreeps_arena.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 04:11:48.000000 pyscreeps-arena-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1035 2024-04-03 04:11:36.000000 pyscreeps-arena-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 04:18:32.020000 pyscreeps-arena-0.1.2/
+-rw-rw-rw-   0        0        0      652 2024-04-03 04:18:34.000000 pyscreeps-arena-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-03 04:18:32.030000 pyscreeps-arena-0.1.2/pyscreeps-arena/
+-rw-rw-rw-   0        0        0      791 2024-04-03 03:59:38.000000 pyscreeps-arena-0.1.2/pyscreeps-arena/__init__.py
+-rw-rw-rw-   0        0        0    20454 2024-04-03 02:55:00.000000 pyscreeps-arena-0.1.2/pyscreeps-arena/build.py
+drwxrwxrwx   0        0        0        0 2024-04-03 04:18:32.040000 pyscreeps-arena-0.1.2/pyscreeps_arena.egg-info/
+-rw-rw-rw-   0        0        0      652 2024-04-03 04:18:34.000000 pyscreeps-arena-0.1.2/pyscreeps_arena.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      297 2024-04-03 04:18:34.000000 pyscreeps-arena-0.1.2/pyscreeps_arena.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 04:18:34.000000 pyscreeps-arena-0.1.2/pyscreeps_arena.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2024-04-03 04:18:34.000000 pyscreeps-arena-0.1.2/pyscreeps_arena.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       80 2024-04-03 04:18:34.000000 pyscreeps-arena-0.1.2/pyscreeps_arena.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-03 04:18:34.000000 pyscreeps-arena-0.1.2/pyscreeps_arena.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-03 04:18:34.000000 pyscreeps-arena-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1167 2024-04-03 04:18:22.000000 pyscreeps-arena-0.1.2/setup.py
```

### Comparing `pyscreeps-arena-0.1.1/PKG-INFO` & `pyscreeps-arena-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscreeps-arena
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python api|interface to play steam game: Screeps: Arena.
 Author-email: 2229066748@qq.com
 Maintainer: Eagle'sBaby
 Maintainer-email: 2229066748@qq.com
 License: Apache Licence 2.0
 Keywords: python,screeps:arena,screeps
 Classifier: Programming Language :: Python
```

### Comparing `pyscreeps-arena-0.1.1/pyscreeps-arena/__init__.py` & `pyscreeps-arena-0.1.2/pyscreeps-arena/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscreeps-arena-0.1.1/pyscreeps-arena/build.py` & `pyscreeps-arena-0.1.2/pyscreeps-arena/build.py`

 * *Files identical despite different names*

### Comparing `pyscreeps-arena-0.1.1/pyscreeps_arena.egg-info/PKG-INFO` & `pyscreeps-arena-0.1.2/pyscreeps_arena.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscreeps-arena
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python api|interface to play steam game: Screeps: Arena.
 Author-email: 2229066748@qq.com
 Maintainer: Eagle'sBaby
 Maintainer-email: 2229066748@qq.com
 License: Apache Licence 2.0
 Keywords: python,screeps:arena,screeps
 Classifier: Programming Language :: Python
```

### Comparing `pyscreeps-arena-0.1.1/setup.py` & `pyscreeps-arena-0.1.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,27 +4,32 @@
 from setuptools import setup, find_packages
 
 
 with open(r"T:\New_PC\Import_Project\uploads\pyscreeps-arena_upload\pyscreeps-arena.md", 'r') as f:
     long_description = f.read()
 setup(
     name='pyscreeps-arena',
-    version='0.1.1',
+    version='0.1.2',
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
         'Programming Language :: Python :: 3.10',
     ],
+    entry_points={
+        'console_scripts': [
+            'pyscreeps-arena=pyscreeps_arena:CMD_NewProject',
+        ]
+    },
     keywords = ['python', 'screeps:arena', 'screeps'],
     python_requires='>=3.10',
     install_requires=[
         'pyperclip',
         'colorma',
         'Transcrypt==3.9.1',
         'mkdocs',
```

