# Comparing `tmp/ran-bst-2.0.2.tar.gz` & `tmp/ran-bst-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ran-bst-2.0.2.tar", last modified: Sat Mar 30 01:44:35 2024, max compression
+gzip compressed data, was "ran-bst-2.1.0.tar", last modified: Tue Apr  2 23:39:11 2024, max compression
```

## Comparing `ran-bst-2.0.2.tar` & `ran-bst-2.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-30 01:44:35.106389 ran-bst-2.0.2/
--rw-rw-r--   0 user      (1000) user      (1000)     1069 2024-03-29 00:43:00.000000 ran-bst-2.0.2/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)     4925 2024-03-30 01:44:35.102389 ran-bst-2.0.2/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     4497 2024-03-29 21:38:31.000000 ran-bst-2.0.2/README.md
--rw-rw-r--   0 user      (1000) user      (1000)       38 2024-03-30 01:44:35.106389 ran-bst-2.0.2/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      648 2024-03-30 01:43:17.000000 ran-bst-2.0.2/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-30 01:44:35.102389 ran-bst-2.0.2/src/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-30 01:44:35.102389 ran-bst-2.0.2/src/bst/
--rw-rw-r--   0 user      (1000) user      (1000)       34 2024-03-29 21:00:03.000000 ran-bst-2.0.2/src/bst/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    22463 2024-03-29 21:34:03.000000 ran-bst-2.0.2/src/bst/lib.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-30 01:44:35.102389 ran-bst-2.0.2/src/ran_bst.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     4925 2024-03-30 01:44:35.000000 ran-bst-2.0.2/src/ran_bst.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      201 2024-03-30 01:44:35.000000 ran-bst-2.0.2/src/ran_bst.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-03-30 01:44:35.000000 ran-bst-2.0.2/src/ran_bst.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        4 2024-03-30 01:44:35.000000 ran-bst-2.0.2/src/ran_bst.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-02 23:39:11.537336 ran-bst-2.1.0/
+-rw-rw-r--   0 user      (1000) user      (1000)     1069 2024-03-29 00:43:00.000000 ran-bst-2.1.0/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)     7399 2024-04-02 23:39:11.537336 ran-bst-2.1.0/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     6971 2024-04-02 23:12:52.000000 ran-bst-2.1.0/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2024-04-02 23:39:11.537336 ran-bst-2.1.0/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)      648 2024-04-01 17:37:19.000000 ran-bst-2.1.0/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-02 23:39:11.533336 ran-bst-2.1.0/src/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-02 23:39:11.533336 ran-bst-2.1.0/src/bst/
+-rw-rw-r--   0 user      (1000) user      (1000)       34 2024-04-02 23:19:50.000000 ran-bst-2.1.0/src/bst/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    27856 2024-04-02 23:29:56.000000 ran-bst-2.1.0/src/bst/lib.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-02 23:39:11.537336 ran-bst-2.1.0/src/ran_bst.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     7399 2024-04-02 23:39:11.000000 ran-bst-2.1.0/src/ran_bst.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      201 2024-04-02 23:39:11.000000 ran-bst-2.1.0/src/ran_bst.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-02 23:39:11.000000 ran-bst-2.1.0/src/ran_bst.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        4 2024-04-02 23:39:11.000000 ran-bst-2.1.0/src/ran_bst.egg-info/top_level.txt
```

### Comparing `ran-bst-2.0.2/LICENSE` & `ran-bst-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ran-bst-2.0.2/setup.py` & `ran-bst-2.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ran-bst',
-    version='2.0.2',
+    version='2.1.0',
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     author='Ran',
     author_email='star01-fym@gmail.com',
     description='A class for binary search trees.',
     long_description=open('README.md', "r", encoding="utf-8").read(),
     long_description_content_type='text/markdown',
```

