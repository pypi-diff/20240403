# Comparing `tmp/piimasking-0.0.2.tar.gz` & `tmp/piimasking-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piimasking-0.0.2.tar", last modified: Tue Apr  2 17:21:59 2024, max compression
+gzip compressed data, was "piimasking-0.0.3.tar", last modified: Tue Apr  2 18:00:28 2024, max compression
```

## Comparing `piimasking-0.0.2.tar` & `piimasking-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxr-xr-x   0 fahadpatel   (501) staff       (20)        0 2024-04-02 17:21:59.736521 piimasking-0.0.2/
--rw-rw-r--   0 fahadpatel   (501) staff       (20)     1067 2024-04-02 14:22:52.000000 piimasking-0.0.2/LICENSE
--rw-rw-r--   0 fahadpatel   (501) staff       (20)      209 2024-04-02 14:51:11.000000 piimasking-0.0.2/MANIFEST.in
--rw-r--r--   0 fahadpatel   (501) staff       (20)     1789 2024-04-02 17:21:59.736428 piimasking-0.0.2/PKG-INFO
--rw-rw-r--   0 fahadpatel   (501) staff       (20)     1232 2024-04-02 14:14:05.000000 piimasking-0.0.2/README.md
-drwxr-xr-x   0 fahadpatel   (501) staff       (20)        0 2024-04-02 17:21:59.736123 piimasking-0.0.2/piimasking.egg-info/
--rw-r--r--   0 fahadpatel   (501) staff       (20)     1789 2024-04-02 17:21:59.000000 piimasking-0.0.2/piimasking.egg-info/PKG-INFO
--rw-r--r--   0 fahadpatel   (501) staff       (20)      232 2024-04-02 17:21:59.000000 piimasking-0.0.2/piimasking.egg-info/SOURCES.txt
--rw-r--r--   0 fahadpatel   (501) staff       (20)        1 2024-04-02 17:21:59.000000 piimasking-0.0.2/piimasking.egg-info/dependency_links.txt
--rw-r--r--   0 fahadpatel   (501) staff       (20)       57 2024-04-02 17:21:59.000000 piimasking-0.0.2/piimasking.egg-info/requires.txt
--rw-r--r--   0 fahadpatel   (501) staff       (20)        1 2024-04-02 17:21:59.000000 piimasking-0.0.2/piimasking.egg-info/top_level.txt
--rw-rw-r--   0 fahadpatel   (501) staff       (20)      107 2024-04-02 14:11:45.000000 piimasking-0.0.2/pyproject.toml
--rw-rw-r--   0 fahadpatel   (501) staff       (20)      522 2024-04-02 17:21:59.736930 piimasking-0.0.2/setup.cfg
--rw-rw-r--   0 fahadpatel   (501) staff       (20)      853 2024-04-02 17:20:43.000000 piimasking-0.0.2/setup.py
+drwxr-xr-x   0 fahadpatel   (501) staff       (20)        0 2024-04-02 18:00:28.377719 piimasking-0.0.3/
+-rw-rw-r--   0 fahadpatel   (501) staff       (20)     1067 2024-04-02 14:22:52.000000 piimasking-0.0.3/LICENSE
+-rw-rw-r--   0 fahadpatel   (501) staff       (20)      209 2024-04-02 14:51:11.000000 piimasking-0.0.3/MANIFEST.in
+-rw-r--r--   0 fahadpatel   (501) staff       (20)     1789 2024-04-02 18:00:28.377629 piimasking-0.0.3/PKG-INFO
+-rw-rw-r--   0 fahadpatel   (501) staff       (20)     1232 2024-04-02 14:14:05.000000 piimasking-0.0.3/README.md
+drwxr-xr-x   0 fahadpatel   (501) staff       (20)        0 2024-04-02 18:00:28.375670 piimasking-0.0.3/piimasking/
+-rw-rw-r--   0 fahadpatel   (501) staff       (20)        0 2024-04-02 17:59:35.000000 piimasking-0.0.3/piimasking/__init__.py
+-rw-r--r--   0 fahadpatel   (501) staff       (20)     3420 2024-04-02 17:17:58.000000 piimasking-0.0.3/piimasking/masking_pipeline.py
+drwxr-xr-x   0 fahadpatel   (501) staff       (20)        0 2024-04-02 18:00:28.377325 piimasking-0.0.3/piimasking.egg-info/
+-rw-r--r--   0 fahadpatel   (501) staff       (20)     1789 2024-04-02 18:00:28.000000 piimasking-0.0.3/piimasking.egg-info/PKG-INFO
+-rw-r--r--   0 fahadpatel   (501) staff       (20)      286 2024-04-02 18:00:28.000000 piimasking-0.0.3/piimasking.egg-info/SOURCES.txt
+-rw-r--r--   0 fahadpatel   (501) staff       (20)        1 2024-04-02 18:00:28.000000 piimasking-0.0.3/piimasking.egg-info/dependency_links.txt
+-rw-r--r--   0 fahadpatel   (501) staff       (20)       57 2024-04-02 18:00:28.000000 piimasking-0.0.3/piimasking.egg-info/requires.txt
+-rw-r--r--   0 fahadpatel   (501) staff       (20)       11 2024-04-02 18:00:28.000000 piimasking-0.0.3/piimasking.egg-info/top_level.txt
+-rw-rw-r--   0 fahadpatel   (501) staff       (20)      108 2024-04-02 17:26:49.000000 piimasking-0.0.3/pyproject.toml
+-rw-rw-r--   0 fahadpatel   (501) staff       (20)      522 2024-04-02 18:00:28.378051 piimasking-0.0.3/setup.cfg
+-rw-rw-r--   0 fahadpatel   (501) staff       (20)      853 2024-04-02 17:59:45.000000 piimasking-0.0.3/setup.py
```

### Comparing `piimasking-0.0.2/LICENSE` & `piimasking-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `piimasking-0.0.2/PKG-INFO` & `piimasking-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piimasking
-Version: 0.0.2
+Version: 0.0.3
 Summary: This repository contains a Python program designed to execute Pii Masking
 Home-page: 
 Author: Amaan Patel
 Author-email: amaanpatel7868@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `piimasking-0.0.2/README.md` & `piimasking-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `piimasking-0.0.2/piimasking.egg-info/PKG-INFO` & `piimasking-0.0.3/piimasking.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piimasking
-Version: 0.0.2
+Version: 0.0.3
 Summary: This repository contains a Python program designed to execute Pii Masking
 Home-page: 
 Author: Amaan Patel
 Author-email: amaanpatel7868@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `piimasking-0.0.2/setup.cfg` & `piimasking-0.0.3/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = piimasking
-version = 0.0.2
+version = 0.0.3
 author = Amaan Patel
 author_email = amaanpatel7868@gmail.com
 description = This repository contains a Python program designed to execute Pii masking
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
```

### Comparing `piimasking-0.0.2/setup.py` & `piimasking-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     required = f.read().splitlines()
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="piimasking",
-    version="0.0.2",
+    version="0.0.3",
     author="Amaan Patel", 
     author_email="amaanpatel7868@gmail.com",
     description=("This repository contains a Python program designed to execute Pii Masking"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     classifiers=[
```

