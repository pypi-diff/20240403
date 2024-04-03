# Comparing `tmp/nwpeval-1.5.0.tar.gz` & `tmp/nwpeval-1.5.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nwpeval-1.5.0.tar", last modified: Wed Apr  3 20:07:33 2024, max compression
+gzip compressed data, was "nwpeval-1.5.0b2.tar", last modified: Wed Apr  3 19:59:08 2024, max compression
```

## Comparing `nwpeval-1.5.0.tar` & `nwpeval-1.5.0b2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:07:33.144698 nwpeval-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-03 20:07:29.000000 nwpeval-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11052 2024-04-03 20:07:33.144698 nwpeval-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10159 2024-04-03 20:07:29.000000 nwpeval-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:07:33.140698 nwpeval-1.5.0/nwpeval/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-03 20:07:29.000000 nwpeval-1.5.0/nwpeval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    58416 2024-04-03 20:07:29.000000 nwpeval-1.5.0/nwpeval/nwpeval.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-03 20:07:29.000000 nwpeval-1.5.0/nwpeval/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:07:33.144698 nwpeval-1.5.0/nwpeval.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11052 2024-04-03 20:07:33.000000 nwpeval-1.5.0/nwpeval.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-03 20:07:33.000000 nwpeval-1.5.0/nwpeval.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 20:07:33.000000 nwpeval-1.5.0/nwpeval.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-03 20:07:33.000000 nwpeval-1.5.0/nwpeval.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 20:07:33.000000 nwpeval-1.5.0/nwpeval.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 20:07:33.144698 nwpeval-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-03 20:07:29.000000 nwpeval-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:59:08.574311 nwpeval-1.5.0b2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-03 19:59:02.000000 nwpeval-1.5.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11054 2024-04-03 19:59:08.574311 nwpeval-1.5.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10159 2024-04-03 19:59:02.000000 nwpeval-1.5.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:59:08.574311 nwpeval-1.5.0b2/nwpeval/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-03 19:59:02.000000 nwpeval-1.5.0b2/nwpeval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58416 2024-04-03 19:59:02.000000 nwpeval-1.5.0b2/nwpeval/nwpeval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-03 19:59:02.000000 nwpeval-1.5.0b2/nwpeval/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:59:08.574311 nwpeval-1.5.0b2/nwpeval.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11054 2024-04-03 19:59:08.000000 nwpeval-1.5.0b2/nwpeval.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-03 19:59:08.000000 nwpeval-1.5.0b2/nwpeval.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:59:08.000000 nwpeval-1.5.0b2/nwpeval.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-03 19:59:08.000000 nwpeval-1.5.0b2/nwpeval.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 19:59:08.000000 nwpeval-1.5.0b2/nwpeval.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:59:08.574311 nwpeval-1.5.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-03 19:59:02.000000 nwpeval-1.5.0b2/setup.py
```

### Comparing `nwpeval-1.5.0/LICENSE` & `nwpeval-1.5.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `nwpeval-1.5.0/PKG-INFO` & `nwpeval-1.5.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwpeval
-Version: 1.5.0
+Version: 1.5.0b2
 Summary: A package for computing metrics for NWP model evaluation
 Author: Debasish Mahapatra
 Author-email: debasish.atmos@gmail.com | debasish.mahapatra@ugent.be
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nwpeval-1.5.0/README.md` & `nwpeval-1.5.0b2/README.md`

 * *Files identical despite different names*

### Comparing `nwpeval-1.5.0/nwpeval/nwpeval.py` & `nwpeval-1.5.0b2/nwpeval/nwpeval.py`

 * *Files identical despite different names*

### Comparing `nwpeval-1.5.0/nwpeval/utils.py` & `nwpeval-1.5.0b2/nwpeval/utils.py`

 * *Files identical despite different names*

### Comparing `nwpeval-1.5.0/nwpeval.egg-info/PKG-INFO` & `nwpeval-1.5.0b2/nwpeval.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwpeval
-Version: 1.5.0
+Version: 1.5.0b2
 Summary: A package for computing metrics for NWP model evaluation
 Author: Debasish Mahapatra
 Author-email: debasish.atmos@gmail.com | debasish.mahapatra@ugent.be
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nwpeval-1.5.0/setup.py` & `nwpeval-1.5.0b2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #with open("CHANGELOG.md", "r") as fh:
  #   changelog = fh.read()
 
 #long_description += "\n\n" + changelog
 
 setup(
     name='nwpeval',
-    version='1.5.0',
+    version='1.5.0b2',
     description='A package for computing metrics for NWP model evaluation',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Debasish Mahapatra',
     author_email='debasish.atmos@gmail.com | debasish.mahapatra@ugent.be',
     
     packages=find_packages(),
```

