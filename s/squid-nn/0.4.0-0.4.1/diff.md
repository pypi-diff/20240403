# Comparing `tmp/squid-nn-0.4.0.tar.gz` & `tmp/squid-nn-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squid-nn-0.4.0.tar", last modified: Tue Feb 20 21:15:33 2024, max compression
+gzip compressed data, was "squid-nn-0.4.1.tar", last modified: Wed Apr  3 20:46:09 2024, max compression
```

## Comparing `squid-nn-0.4.0.tar` & `squid-nn-0.4.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 evanseitz   (501) staff       (20)        0 2024-02-20 21:15:33.000000 squid-nn-0.4.0/
--rw-r--r--   0 evanseitz   (501) staff       (20)     1116 2023-10-29 01:33:37.000000 squid-nn-0.4.0/LICENSE
--rw-r--r--   0 evanseitz   (501) staff       (20)      553 2024-02-20 21:15:33.000000 squid-nn-0.4.0/PKG-INFO
--rw-r--r--   0 evanseitz   (501) staff       (20)     6085 2024-02-20 21:14:19.000000 squid-nn-0.4.0/README.md
--rw-r--r--   0 evanseitz   (501) staff       (20)       38 2024-02-20 21:15:33.000000 squid-nn-0.4.0/setup.cfg
--rw-r--r--   0 evanseitz   (501) staff       (20)      653 2024-02-20 21:14:57.000000 squid-nn-0.4.0/setup.py
-drwxr-xr-x   0 evanseitz   (501) staff       (20)        0 2024-02-20 21:15:33.000000 squid-nn-0.4.0/squid/
--rw-r--r--   0 evanseitz   (501) staff       (20)      145 2023-10-29 01:33:37.000000 squid-nn-0.4.0/squid/__init__.py
--rw-r--r--   0 evanseitz   (501) staff       (20)    13396 2023-12-01 19:34:26.000000 squid-nn-0.4.0/squid/impress.py
--rw-r--r--   0 evanseitz   (501) staff       (20)    14977 2024-01-04 20:58:35.000000 squid-nn-0.4.0/squid/mave.py
--rw-r--r--   0 evanseitz   (501) staff       (20)     4784 2024-01-04 21:01:19.000000 squid-nn-0.4.0/squid/mutagenizer.py
--rw-r--r--   0 evanseitz   (501) staff       (20)     9537 2024-02-18 20:23:31.000000 squid-nn-0.4.0/squid/predictor.py
--rw-r--r--   0 evanseitz   (501) staff       (20)    34550 2024-02-20 20:45:17.000000 squid-nn-0.4.0/squid/surrogate_zoo.py
--rw-r--r--   0 evanseitz   (501) staff       (20)     4324 2023-11-10 13:16:19.000000 squid-nn-0.4.0/squid/utils.py
-drwxr-xr-x   0 evanseitz   (501) staff       (20)        0 2024-02-20 21:15:33.000000 squid-nn-0.4.0/squid_nn.egg-info/
--rw-r--r--   0 evanseitz   (501) staff       (20)      553 2024-02-20 21:15:32.000000 squid-nn-0.4.0/squid_nn.egg-info/PKG-INFO
--rw-r--r--   0 evanseitz   (501) staff       (20)      312 2024-02-20 21:15:32.000000 squid-nn-0.4.0/squid_nn.egg-info/SOURCES.txt
--rw-r--r--   0 evanseitz   (501) staff       (20)        1 2024-02-20 21:15:32.000000 squid-nn-0.4.0/squid_nn.egg-info/dependency_links.txt
--rw-r--r--   0 evanseitz   (501) staff       (20)       36 2024-02-20 21:15:32.000000 squid-nn-0.4.0/squid_nn.egg-info/requires.txt
--rw-r--r--   0 evanseitz   (501) staff       (20)        6 2024-02-20 21:15:32.000000 squid-nn-0.4.0/squid_nn.egg-info/top_level.txt
+drwxr-xr-x   0 evanseitz   (501) staff       (20)        0 2024-04-03 20:46:09.000000 squid-nn-0.4.1/
+-rw-r--r--   0 evanseitz   (501) staff       (20)     1116 2023-10-29 01:33:37.000000 squid-nn-0.4.1/LICENSE
+-rw-r--r--   0 evanseitz   (501) staff       (20)      553 2024-04-03 20:46:09.000000 squid-nn-0.4.1/PKG-INFO
+-rw-r--r--   0 evanseitz   (501) staff       (20)     6085 2024-02-20 21:14:19.000000 squid-nn-0.4.1/README.md
+-rw-r--r--   0 evanseitz   (501) staff       (20)       38 2024-04-03 20:46:09.000000 squid-nn-0.4.1/setup.cfg
+-rw-r--r--   0 evanseitz   (501) staff       (20)      653 2024-04-03 20:45:53.000000 squid-nn-0.4.1/setup.py
+drwxr-xr-x   0 evanseitz   (501) staff       (20)        0 2024-04-03 20:46:09.000000 squid-nn-0.4.1/squid/
+-rw-r--r--   0 evanseitz   (501) staff       (20)      145 2023-10-29 01:33:37.000000 squid-nn-0.4.1/squid/__init__.py
+-rw-r--r--   0 evanseitz   (501) staff       (20)    13396 2023-12-01 19:34:26.000000 squid-nn-0.4.1/squid/impress.py
+-rw-r--r--   0 evanseitz   (501) staff       (20)    14977 2024-01-04 20:58:35.000000 squid-nn-0.4.1/squid/mave.py
+-rw-r--r--   0 evanseitz   (501) staff       (20)     9740 2024-04-03 20:36:12.000000 squid-nn-0.4.1/squid/mutagenizer.py
+-rw-r--r--   0 evanseitz   (501) staff       (20)     9537 2024-02-18 20:23:31.000000 squid-nn-0.4.1/squid/predictor.py
+-rw-r--r--   0 evanseitz   (501) staff       (20)    34550 2024-02-20 20:45:17.000000 squid-nn-0.4.1/squid/surrogate_zoo.py
+-rw-r--r--   0 evanseitz   (501) staff       (20)     4324 2023-11-10 13:16:19.000000 squid-nn-0.4.1/squid/utils.py
+drwxr-xr-x   0 evanseitz   (501) staff       (20)        0 2024-04-03 20:46:09.000000 squid-nn-0.4.1/squid_nn.egg-info/
+-rw-r--r--   0 evanseitz   (501) staff       (20)      553 2024-04-03 20:46:09.000000 squid-nn-0.4.1/squid_nn.egg-info/PKG-INFO
+-rw-r--r--   0 evanseitz   (501) staff       (20)      312 2024-04-03 20:46:09.000000 squid-nn-0.4.1/squid_nn.egg-info/SOURCES.txt
+-rw-r--r--   0 evanseitz   (501) staff       (20)        1 2024-04-03 20:46:09.000000 squid-nn-0.4.1/squid_nn.egg-info/dependency_links.txt
+-rw-r--r--   0 evanseitz   (501) staff       (20)       36 2024-04-03 20:46:09.000000 squid-nn-0.4.1/squid_nn.egg-info/requires.txt
+-rw-r--r--   0 evanseitz   (501) staff       (20)        6 2024-04-03 20:46:09.000000 squid-nn-0.4.1/squid_nn.egg-info/top_level.txt
```

### Comparing `squid-nn-0.4.0/LICENSE` & `squid-nn-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `squid-nn-0.4.0/PKG-INFO` & `squid-nn-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squid-nn
-Version: 0.4.0
+Version: 0.4.1
 Summary: SQUID is a TensorFlow package to interpret sequence-based deep learning models for regulatory genomics data with domain-specific surrogate models.
 Author: Evan Seitz
 Author-email: evan.e.seitz@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7.2
```

### Comparing `squid-nn-0.4.0/README.md` & `squid-nn-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `squid-nn-0.4.0/setup.py` & `squid-nn-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="squid-nn",
-    version="0.4.0",
+    version="0.4.1",
     author="Evan Seitz",
     author_email="evan.e.seitz@gmail.com",
     packages=find_packages(),
     description = "SQUID is a TensorFlow package to interpret sequence-based deep learning models for regulatory genomics data with domain-specific surrogate models.",
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
```

### Comparing `squid-nn-0.4.0/squid/impress.py` & `squid-nn-0.4.1/squid/impress.py`

 * *Files identical despite different names*

### Comparing `squid-nn-0.4.0/squid/mave.py` & `squid-nn-0.4.1/squid/mave.py`

 * *Files identical despite different names*

### Comparing `squid-nn-0.4.0/squid/predictor.py` & `squid-nn-0.4.1/squid/predictor.py`

 * *Files identical despite different names*

### Comparing `squid-nn-0.4.0/squid/surrogate_zoo.py` & `squid-nn-0.4.1/squid/surrogate_zoo.py`

 * *Files identical despite different names*

### Comparing `squid-nn-0.4.0/squid/utils.py` & `squid-nn-0.4.1/squid/utils.py`

 * *Files identical despite different names*

### Comparing `squid-nn-0.4.0/squid_nn.egg-info/PKG-INFO` & `squid-nn-0.4.1/squid_nn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squid-nn
-Version: 0.4.0
+Version: 0.4.1
 Summary: SQUID is a TensorFlow package to interpret sequence-based deep learning models for regulatory genomics data with domain-specific surrogate models.
 Author: Evan Seitz
 Author-email: evan.e.seitz@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7.2
```

