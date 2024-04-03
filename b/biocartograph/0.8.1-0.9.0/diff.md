# Comparing `tmp/biocartograph-0.8.1.tar.gz` & `tmp/biocartograph-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biocartograph-0.8.1.tar", last modified: Sun Nov 19 10:28:23 2023, max compression
+gzip compressed data, was "biocartograph-0.9.0.tar", last modified: Mon Dec 11 17:01:00 2023, max compression
```

## Comparing `biocartograph-0.8.1.tar` & `biocartograph-0.9.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-11-19 10:28:23.487079 biocartograph-0.8.1/
--rw-r--r--   0 rictjo    (1000) users      (100)    11357 2023-11-19 10:27:55.000000 biocartograph-0.8.1/LICENSE
--rw-r--r--   0 rictjo    (1000) users      (100)     9796 2023-11-19 10:28:23.487079 biocartograph-0.8.1/PKG-INFO
--rw-r--r--   0 rictjo    (1000) users      (100)     9290 2023-11-19 10:27:55.000000 biocartograph-0.8.1/README.md
-drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-11-19 10:28:23.486079 biocartograph-0.8.1/biocartograph.egg-info/
--rw-r--r--   0 rictjo    (1000) users      (100)     9796 2023-11-19 10:28:23.000000 biocartograph-0.8.1/biocartograph.egg-info/PKG-INFO
--rw-r--r--   0 rictjo    (1000) users      (100)      362 2023-11-19 10:28:23.000000 biocartograph-0.8.1/biocartograph.egg-info/SOURCES.txt
--rw-r--r--   0 rictjo    (1000) users      (100)        1 2023-11-19 10:28:23.000000 biocartograph-0.8.1/biocartograph.egg-info/dependency_links.txt
--rw-r--r--   0 rictjo    (1000) users      (100)       14 2023-11-19 10:28:23.000000 biocartograph-0.8.1/biocartograph.egg-info/top_level.txt
--rw-r--r--   0 rictjo    (1000) users      (100)       38 2023-11-19 10:28:23.487079 biocartograph-0.8.1/setup.cfg
--rw-r--r--   0 rictjo    (1000) users      (100)      978 2023-11-19 10:27:55.000000 biocartograph-0.8.1/setup.py
-drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-11-19 10:28:23.486079 biocartograph-0.8.1/src/
-drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-11-19 10:28:23.487079 biocartograph-0.8.1/src/biocartograph/
--rw-r--r--   0 rictjo    (1000) users      (100)       23 2023-11-19 10:27:55.000000 biocartograph-0.8.1/src/biocartograph/__init__.py
--rw-r--r--   0 rictjo    (1000) users      (100)     4623 2023-11-19 10:27:55.000000 biocartograph-0.8.1/src/biocartograph/composition.py
--rw-r--r--   0 rictjo    (1000) users      (100)    20104 2023-11-19 10:27:55.000000 biocartograph-0.8.1/src/biocartograph/enrichment.py
--rw-r--r--   0 rictjo    (1000) users      (100)     7587 2023-11-19 10:27:55.000000 biocartograph-0.8.1/src/biocartograph/models.py
--rw-r--r--   0 rictjo    (1000) users      (100)    25902 2023-11-19 10:27:55.000000 biocartograph-0.8.1/src/biocartograph/quantification.py
--rw-r--r--   0 rictjo    (1000) users      (100)    31258 2023-11-19 10:27:55.000000 biocartograph-0.8.1/src/biocartograph/special.py
+drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-12-11 17:01:00.294617 biocartograph-0.9.0/
+-rw-r--r--   0 rictjo    (1000) users      (100)    11357 2023-11-19 10:27:55.000000 biocartograph-0.9.0/LICENSE
+-rw-r--r--   0 rictjo    (1000) users      (100)     9796 2023-12-11 17:01:00.294617 biocartograph-0.9.0/PKG-INFO
+-rw-r--r--   0 rictjo    (1000) users      (100)     9290 2023-11-19 10:27:55.000000 biocartograph-0.9.0/README.md
+drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-12-11 17:01:00.293617 biocartograph-0.9.0/biocartograph.egg-info/
+-rw-r--r--   0 rictjo    (1000) users      (100)     9796 2023-12-11 17:01:00.000000 biocartograph-0.9.0/biocartograph.egg-info/PKG-INFO
+-rw-r--r--   0 rictjo    (1000) users      (100)      362 2023-12-11 17:01:00.000000 biocartograph-0.9.0/biocartograph.egg-info/SOURCES.txt
+-rw-r--r--   0 rictjo    (1000) users      (100)        1 2023-12-11 17:01:00.000000 biocartograph-0.9.0/biocartograph.egg-info/dependency_links.txt
+-rw-r--r--   0 rictjo    (1000) users      (100)       14 2023-12-11 17:01:00.000000 biocartograph-0.9.0/biocartograph.egg-info/top_level.txt
+-rw-r--r--   0 rictjo    (1000) users      (100)       38 2023-12-11 17:01:00.294617 biocartograph-0.9.0/setup.cfg
+-rw-r--r--   0 rictjo    (1000) users      (100)      978 2023-12-11 17:00:35.000000 biocartograph-0.9.0/setup.py
+drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-12-11 17:01:00.293617 biocartograph-0.9.0/src/
+drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-12-11 17:01:00.294617 biocartograph-0.9.0/src/biocartograph/
+-rw-r--r--   0 rictjo    (1000) users      (100)       23 2023-11-19 10:27:55.000000 biocartograph-0.9.0/src/biocartograph/__init__.py
+-rw-r--r--   0 rictjo    (1000) users      (100)     4623 2023-11-19 10:27:55.000000 biocartograph-0.9.0/src/biocartograph/composition.py
+-rw-r--r--   0 rictjo    (1000) users      (100)    20104 2023-11-19 10:27:55.000000 biocartograph-0.9.0/src/biocartograph/enrichment.py
+-rw-r--r--   0 rictjo    (1000) users      (100)    13824 2023-12-11 17:00:35.000000 biocartograph-0.9.0/src/biocartograph/models.py
+-rw-r--r--   0 rictjo    (1000) users      (100)    25902 2023-11-19 10:27:55.000000 biocartograph-0.9.0/src/biocartograph/quantification.py
+-rw-r--r--   0 rictjo    (1000) users      (100)    31258 2023-11-19 10:27:55.000000 biocartograph-0.9.0/src/biocartograph/special.py
```

### Comparing `biocartograph-0.8.1/LICENSE` & `biocartograph-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `biocartograph-0.8.1/PKG-INFO` & `biocartograph-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biocartograph
-Version: 0.8.1
+Version: 0.9.0
 Summary: Package was renamed from Biocarta v0.2.27 to Biocartograph because of an unintentional name clash
 Home-page: https://github.com/rictjo/biocarta
 Author: Richard Tjörnhammar
 Author-email: richard.tjornhammar@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `biocartograph-0.8.1/README.md` & `biocartograph-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `biocartograph-0.8.1/biocartograph.egg-info/PKG-INFO` & `biocartograph-0.9.0/biocartograph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biocartograph
-Version: 0.8.1
+Version: 0.9.0
 Summary: Package was renamed from Biocarta v0.2.27 to Biocartograph because of an unintentional name clash
 Home-page: https://github.com/rictjo/biocarta
 Author: Richard Tjörnhammar
 Author-email: richard.tjornhammar@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `biocartograph-0.8.1/setup.py` & `biocartograph-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name         = "biocartograph",
-    version      = "0.8.1",
+    version      = "0.9.0",
     author       = "Richard Tjörnhammar",
     author_email = "richard.tjornhammar@gmail.com",
     description  = "Package was renamed from Biocarta v0.2.27 to Biocartograph because of an unintentional name clash",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/rictjo/biocarta",
     packages = setuptools.find_packages('src'),
```

### Comparing `biocartograph-0.8.1/src/biocartograph/composition.py` & `biocartograph-0.9.0/src/biocartograph/composition.py`

 * *Files identical despite different names*

### Comparing `biocartograph-0.8.1/src/biocartograph/enrichment.py` & `biocartograph-0.9.0/src/biocartograph/enrichment.py`

 * *Files identical despite different names*

### Comparing `biocartograph-0.8.1/src/biocartograph/quantification.py` & `biocartograph-0.9.0/src/biocartograph/quantification.py`

 * *Files identical despite different names*

### Comparing `biocartograph-0.8.1/src/biocartograph/special.py` & `biocartograph-0.9.0/src/biocartograph/special.py`

 * *Files identical despite different names*

