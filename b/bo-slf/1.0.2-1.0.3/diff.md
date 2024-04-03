# Comparing `tmp/bo_slf-1.0.2.tar.gz` & `tmp/bo_slf-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bo_slf-1.0.2.tar", last modified: Fri Mar 29 15:40:35 2024, max compression
+gzip compressed data, was "bo_slf-1.0.3.tar", last modified: Wed Apr  3 05:18:44 2024, max compression
```

## Comparing `bo_slf-1.0.2.tar` & `bo_slf-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 javiermorlet   (501) staff       (20)        0 2024-03-29 15:40:35.976861 bo_slf-1.0.2/
--rw-r--r--   0 javiermorlet   (501) staff       (20)     1079 2024-03-23 20:53:34.000000 bo_slf-1.0.2/LICENSE.txt
--rw-r--r--   0 javiermorlet   (501) staff       (20)      513 2024-03-29 15:40:35.976592 bo_slf-1.0.2/PKG-INFO
-drwxr-xr-x   0 javiermorlet   (501) staff       (20)        0 2024-03-29 15:40:35.975495 bo_slf-1.0.2/bo_slf/
--rw-r--r--   0 javiermorlet   (501) staff       (20)       56 2024-03-29 15:32:34.000000 bo_slf-1.0.2/bo_slf/__init__.py
-drwxr-xr-x   0 javiermorlet   (501) staff       (20)        0 2024-03-29 15:40:35.976294 bo_slf-1.0.2/bo_slf.egg-info/
--rw-r--r--   0 javiermorlet   (501) staff       (20)      513 2024-03-29 15:40:35.000000 bo_slf-1.0.2/bo_slf.egg-info/PKG-INFO
--rw-r--r--   0 javiermorlet   (501) staff       (20)      188 2024-03-29 15:40:35.000000 bo_slf-1.0.2/bo_slf.egg-info/SOURCES.txt
--rw-r--r--   0 javiermorlet   (501) staff       (20)        1 2024-03-29 15:40:35.000000 bo_slf-1.0.2/bo_slf.egg-info/dependency_links.txt
--rw-r--r--   0 javiermorlet   (501) staff       (20)      140 2024-03-29 15:40:35.000000 bo_slf-1.0.2/bo_slf.egg-info/requires.txt
--rw-r--r--   0 javiermorlet   (501) staff       (20)        7 2024-03-29 15:40:35.000000 bo_slf-1.0.2/bo_slf.egg-info/top_level.txt
--rw-r--r--   0 javiermorlet   (501) staff       (20)       38 2024-03-29 15:40:35.976907 bo_slf-1.0.2/setup.cfg
--rw-r--r--   0 javiermorlet   (501) staff       (20)      631 2024-03-29 15:39:55.000000 bo_slf-1.0.2/setup.py
+drwxr-xr-x   0 javiermorlet   (501) staff       (20)        0 2024-04-03 05:18:44.623592 bo_slf-1.0.3/
+-rw-r--r--   0 javiermorlet   (501) staff       (20)     1079 2024-03-23 20:53:34.000000 bo_slf-1.0.3/LICENSE.txt
+-rw-r--r--   0 javiermorlet   (501) staff       (20)      513 2024-04-03 05:18:44.623365 bo_slf-1.0.3/PKG-INFO
+drwxr-xr-x   0 javiermorlet   (501) staff       (20)        0 2024-04-03 05:18:44.622360 bo_slf-1.0.3/bo_slf/
+-rw-r--r--   0 javiermorlet   (501) staff       (20)       16 2024-04-03 04:01:04.000000 bo_slf-1.0.3/bo_slf/__init__.py
+drwxr-xr-x   0 javiermorlet   (501) staff       (20)        0 2024-04-03 05:18:44.623093 bo_slf-1.0.3/bo_slf.egg-info/
+-rw-r--r--   0 javiermorlet   (501) staff       (20)      513 2024-04-03 05:18:44.000000 bo_slf-1.0.3/bo_slf.egg-info/PKG-INFO
+-rw-r--r--   0 javiermorlet   (501) staff       (20)      188 2024-04-03 05:18:44.000000 bo_slf-1.0.3/bo_slf.egg-info/SOURCES.txt
+-rw-r--r--   0 javiermorlet   (501) staff       (20)        1 2024-04-03 05:18:44.000000 bo_slf-1.0.3/bo_slf.egg-info/dependency_links.txt
+-rw-r--r--   0 javiermorlet   (501) staff       (20)      140 2024-04-03 05:18:44.000000 bo_slf-1.0.3/bo_slf.egg-info/requires.txt
+-rw-r--r--   0 javiermorlet   (501) staff       (20)        7 2024-04-03 05:18:44.000000 bo_slf-1.0.3/bo_slf.egg-info/top_level.txt
+-rw-r--r--   0 javiermorlet   (501) staff       (20)       38 2024-04-03 05:18:44.623638 bo_slf-1.0.3/setup.cfg
+-rw-r--r--   0 javiermorlet   (501) staff       (20)      631 2024-04-03 04:01:22.000000 bo_slf-1.0.3/setup.py
```

### Comparing `bo_slf-1.0.2/LICENSE.txt` & `bo_slf-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bo_slf-1.0.2/PKG-INFO` & `bo_slf-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bo_slf
-Version: 1.0.2
+Version: 1.0.3
 Summary: Bayesian optimization for constrained or unconstrained, continuous, discrete or mixed data problems
 Author: Javier Morlet
 Author-email: a00833961@tec.mx
 License-File: LICENSE.txt
 Requires-Dist: numpy>=1.23.5
 Requires-Dist: sympy>=1.11.1
 Requires-Dist: pandas>=2.0.3
```

### Comparing `bo_slf-1.0.2/bo_slf.egg-info/PKG-INFO` & `bo_slf-1.0.3/bo_slf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bo-slf
-Version: 1.0.2
+Version: 1.0.3
 Summary: Bayesian optimization for constrained or unconstrained, continuous, discrete or mixed data problems
 Author: Javier Morlet
 Author-email: a00833961@tec.mx
 License-File: LICENSE.txt
 Requires-Dist: numpy>=1.23.5
 Requires-Dist: sympy>=1.11.1
 Requires-Dist: pandas>=2.0.3
```

### Comparing `bo_slf-1.0.2/setup.py` & `bo_slf-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 
 setup(name='bo_slf',
-      version='1.0.2',
+      version='1.0.3',
       description='Bayesian optimization for constrained or unconstrained, continuous, discrete or mixed data problems',
       author='Javier Morlet',
       author_email='a00833961@tec.mx',
       packages = find_packages(include=['bo_slf']),
       install_requires=[
           'numpy>=1.23.5',
           'sympy>=1.11.1',
```

