# Comparing `tmp/bo_slf-1.0.4.tar.gz` & `tmp/bo_slf-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bo_slf-1.0.4.tar", last modified: Wed Apr  3 10:36:16 2024, max compression
+gzip compressed data, was "bo_slf-1.0.5.tar", last modified: Wed Apr  3 10:46:31 2024, max compression
```

## Comparing `bo_slf-1.0.4.tar` & `bo_slf-1.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 javiermorlet   (501) staff       (20)        0 2024-04-03 10:36:16.576434 bo_slf-1.0.4/
--rw-r--r--   0 javiermorlet   (501) staff       (20)     1079 2024-03-23 20:53:34.000000 bo_slf-1.0.4/LICENSE.txt
--rw-r--r--   0 javiermorlet   (501) staff       (20)      513 2024-04-03 10:36:16.576211 bo_slf-1.0.4/PKG-INFO
-drwxr-xr-x   0 javiermorlet   (501) staff       (20)        0 2024-04-03 10:36:16.575227 bo_slf-1.0.4/bo_slf/
--rw-r--r--   0 javiermorlet   (501) staff       (20)       49 2024-04-03 10:34:41.000000 bo_slf-1.0.4/bo_slf/__init__.py
-drwxr-xr-x   0 javiermorlet   (501) staff       (20)        0 2024-04-03 10:36:16.575945 bo_slf-1.0.4/bo_slf.egg-info/
--rw-r--r--   0 javiermorlet   (501) staff       (20)      513 2024-04-03 10:36:16.000000 bo_slf-1.0.4/bo_slf.egg-info/PKG-INFO
--rw-r--r--   0 javiermorlet   (501) staff       (20)      188 2024-04-03 10:36:16.000000 bo_slf-1.0.4/bo_slf.egg-info/SOURCES.txt
--rw-r--r--   0 javiermorlet   (501) staff       (20)        1 2024-04-03 10:36:16.000000 bo_slf-1.0.4/bo_slf.egg-info/dependency_links.txt
--rw-r--r--   0 javiermorlet   (501) staff       (20)      140 2024-04-03 10:36:16.000000 bo_slf-1.0.4/bo_slf.egg-info/requires.txt
--rw-r--r--   0 javiermorlet   (501) staff       (20)        7 2024-04-03 10:36:16.000000 bo_slf-1.0.4/bo_slf.egg-info/top_level.txt
--rw-r--r--   0 javiermorlet   (501) staff       (20)       38 2024-04-03 10:36:16.576479 bo_slf-1.0.4/setup.cfg
--rw-r--r--   0 javiermorlet   (501) staff       (20)      631 2024-04-03 10:35:04.000000 bo_slf-1.0.4/setup.py
+drwxr-xr-x   0 javiermorlet   (501) staff       (20)        0 2024-04-03 10:46:31.817051 bo_slf-1.0.5/
+-rw-r--r--   0 javiermorlet   (501) staff       (20)     1079 2024-03-23 20:53:34.000000 bo_slf-1.0.5/LICENSE.txt
+-rw-r--r--   0 javiermorlet   (501) staff       (20)      513 2024-04-03 10:46:31.816825 bo_slf-1.0.5/PKG-INFO
+drwxr-xr-x   0 javiermorlet   (501) staff       (20)        0 2024-04-03 10:46:31.815915 bo_slf-1.0.5/bo_slf/
+-rw-r--r--   0 javiermorlet   (501) staff       (20)      110 2024-04-03 10:46:13.000000 bo_slf-1.0.5/bo_slf/__init__.py
+drwxr-xr-x   0 javiermorlet   (501) staff       (20)        0 2024-04-03 10:46:31.816543 bo_slf-1.0.5/bo_slf.egg-info/
+-rw-r--r--   0 javiermorlet   (501) staff       (20)      513 2024-04-03 10:46:31.000000 bo_slf-1.0.5/bo_slf.egg-info/PKG-INFO
+-rw-r--r--   0 javiermorlet   (501) staff       (20)      188 2024-04-03 10:46:31.000000 bo_slf-1.0.5/bo_slf.egg-info/SOURCES.txt
+-rw-r--r--   0 javiermorlet   (501) staff       (20)        1 2024-04-03 10:46:31.000000 bo_slf-1.0.5/bo_slf.egg-info/dependency_links.txt
+-rw-r--r--   0 javiermorlet   (501) staff       (20)      140 2024-04-03 10:46:31.000000 bo_slf-1.0.5/bo_slf.egg-info/requires.txt
+-rw-r--r--   0 javiermorlet   (501) staff       (20)        7 2024-04-03 10:46:31.000000 bo_slf-1.0.5/bo_slf.egg-info/top_level.txt
+-rw-r--r--   0 javiermorlet   (501) staff       (20)       38 2024-04-03 10:46:31.817096 bo_slf-1.0.5/setup.cfg
+-rw-r--r--   0 javiermorlet   (501) staff       (20)      631 2024-04-03 10:45:18.000000 bo_slf-1.0.5/setup.py
```

### Comparing `bo_slf-1.0.4/LICENSE.txt` & `bo_slf-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bo_slf-1.0.4/PKG-INFO` & `bo_slf-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bo_slf
-Version: 1.0.4
+Version: 1.0.5
 Summary: Bayesian optimization for constrained or unconstrained, continuous, discrete or mixed data problems
 Author: Javier Morlet
 Author-email: a00833961@tec.mx
 License-File: LICENSE.txt
 Requires-Dist: numpy>=1.23.5
 Requires-Dist: sympy>=1.11.1
 Requires-Dist: pandas>=2.0.3
```

### Comparing `bo_slf-1.0.4/bo_slf.egg-info/PKG-INFO` & `bo_slf-1.0.5/bo_slf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bo-slf
-Version: 1.0.4
+Version: 1.0.5
 Summary: Bayesian optimization for constrained or unconstrained, continuous, discrete or mixed data problems
 Author: Javier Morlet
 Author-email: a00833961@tec.mx
 License-File: LICENSE.txt
 Requires-Dist: numpy>=1.23.5
 Requires-Dist: sympy>=1.11.1
 Requires-Dist: pandas>=2.0.3
```

### Comparing `bo_slf-1.0.4/setup.py` & `bo_slf-1.0.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 
 setup(name='bo_slf',
-      version='1.0.4',
+      version='1.0.5',
       description='Bayesian optimization for constrained or unconstrained, continuous, discrete or mixed data problems',
       author='Javier Morlet',
       author_email='a00833961@tec.mx',
       packages = find_packages(include=['bo_slf']),
       install_requires=[
           'numpy>=1.23.5',
           'sympy>=1.11.1',
```

