# Comparing `tmp/skdir-0.0.5.tar.gz` & `tmp/skdir-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skdir-0.0.5.tar", last modified: Wed Apr  3 17:38:35 2024, max compression
+gzip compressed data, was "skdir-0.0.6.tar", last modified: Wed Apr  3 17:53:55 2024, max compression
```

## Comparing `skdir-0.0.5.tar` & `skdir-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 sharathchandrak   (501) staff       (20)        0 2024-04-03 17:38:35.569042 skdir-0.0.5/
--rw-rw-r--   0 sharathchandrak   (501) staff       (20)     1064 2021-07-27 04:28:46.000000 skdir-0.0.5/LICENSE
--rw-r--r--   0 sharathchandrak   (501) staff       (20)      620 2024-04-03 17:38:35.568846 skdir-0.0.5/PKG-INFO
--rw-rw-r--   0 sharathchandrak   (501) staff       (20)      981 2021-07-27 04:28:46.000000 skdir-0.0.5/README.md
-drwxr-xr-x   0 sharathchandrak   (501) staff       (20)        0 2024-04-03 17:38:35.567317 skdir-0.0.5/lab/
--rw-r--r--   0 sharathchandrak   (501) staff       (20)        0 2024-04-03 16:25:48.000000 skdir-0.0.5/lab/__init__.py
--rw-rw-r--   0 sharathchandrak   (501) staff       (20)     2873 2024-04-03 16:35:15.000000 skdir-0.0.5/lab/p1.py
--rw-rw-r--   0 sharathchandrak   (501) staff       (20)      985 2024-04-03 16:35:24.000000 skdir-0.0.5/lab/p2.py
--rw-rw-r--   0 sharathchandrak   (501) staff       (20)     4208 2024-04-03 16:35:34.000000 skdir-0.0.5/lab/p3.py
--rw-r--r--   0 sharathchandrak   (501) staff       (20)     1701 2024-04-03 16:36:03.000000 skdir-0.0.5/lab/p4.py
--rw-r--r--   0 sharathchandrak   (501) staff       (20)     1808 2024-04-03 16:36:40.000000 skdir-0.0.5/lab/p5.py
--rw-r--r--   0 sharathchandrak   (501) staff       (20)     1798 2024-04-03 16:36:57.000000 skdir-0.0.5/lab/p6.py
--rw-r--r--   0 sharathchandrak   (501) staff       (20)     1869 2024-04-03 16:37:20.000000 skdir-0.0.5/lab/p7.py
--rw-r--r--   0 sharathchandrak   (501) staff       (20)     1111 2024-04-03 16:38:04.000000 skdir-0.0.5/lab/p8.py
--rw-r--r--   0 sharathchandrak   (501) staff       (20)       38 2024-04-03 17:38:35.569127 skdir-0.0.5/setup.cfg
--rw-rw-r--   0 sharathchandrak   (501) staff       (20)      930 2024-04-03 17:38:33.000000 skdir-0.0.5/setup.py
-drwxr-xr-x   0 sharathchandrak   (501) staff       (20)        0 2024-04-03 17:38:35.568558 skdir-0.0.5/skdir.egg-info/
--rw-r--r--   0 sharathchandrak   (501) staff       (20)      620 2024-04-03 17:38:35.000000 skdir-0.0.5/skdir.egg-info/PKG-INFO
--rw-r--r--   0 sharathchandrak   (501) staff       (20)      266 2024-04-03 17:38:35.000000 skdir-0.0.5/skdir.egg-info/SOURCES.txt
--rw-r--r--   0 sharathchandrak   (501) staff       (20)        1 2024-04-03 17:38:35.000000 skdir-0.0.5/skdir.egg-info/dependency_links.txt
--rw-r--r--   0 sharathchandrak   (501) staff       (20)       53 2024-04-03 17:38:35.000000 skdir-0.0.5/skdir.egg-info/requires.txt
--rw-r--r--   0 sharathchandrak   (501) staff       (20)        4 2024-04-03 17:38:35.000000 skdir-0.0.5/skdir.egg-info/top_level.txt
+drwxr-xr-x   0 sharathchandrak   (501) staff       (20)        0 2024-04-03 17:53:55.487379 skdir-0.0.6/
+-rw-rw-r--   0 sharathchandrak   (501) staff       (20)     1064 2021-07-27 04:28:46.000000 skdir-0.0.6/LICENSE
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)      620 2024-04-03 17:53:55.487180 skdir-0.0.6/PKG-INFO
+-rw-rw-r--   0 sharathchandrak   (501) staff       (20)      981 2021-07-27 04:28:46.000000 skdir-0.0.6/README.md
+drwxr-xr-x   0 sharathchandrak   (501) staff       (20)        0 2024-04-03 17:53:55.485769 skdir-0.0.6/lab/
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)      744 2024-04-03 17:50:49.000000 skdir-0.0.6/lab/__init__.py
+-rw-rw-r--   0 sharathchandrak   (501) staff       (20)     2873 2024-04-03 16:35:15.000000 skdir-0.0.6/lab/p1.py
+-rw-rw-r--   0 sharathchandrak   (501) staff       (20)      985 2024-04-03 16:35:24.000000 skdir-0.0.6/lab/p2.py
+-rw-rw-r--   0 sharathchandrak   (501) staff       (20)     4208 2024-04-03 16:35:34.000000 skdir-0.0.6/lab/p3.py
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)     1701 2024-04-03 16:36:03.000000 skdir-0.0.6/lab/p4.py
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)     1808 2024-04-03 16:36:40.000000 skdir-0.0.6/lab/p5.py
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)     1798 2024-04-03 16:36:57.000000 skdir-0.0.6/lab/p6.py
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)     1869 2024-04-03 16:37:20.000000 skdir-0.0.6/lab/p7.py
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)     1111 2024-04-03 16:38:04.000000 skdir-0.0.6/lab/p8.py
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)       38 2024-04-03 17:53:55.487462 skdir-0.0.6/setup.cfg
+-rw-rw-r--   0 sharathchandrak   (501) staff       (20)      930 2024-04-03 17:52:22.000000 skdir-0.0.6/setup.py
+drwxr-xr-x   0 sharathchandrak   (501) staff       (20)        0 2024-04-03 17:53:55.486871 skdir-0.0.6/skdir.egg-info/
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)      620 2024-04-03 17:53:55.000000 skdir-0.0.6/skdir.egg-info/PKG-INFO
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)      266 2024-04-03 17:53:55.000000 skdir-0.0.6/skdir.egg-info/SOURCES.txt
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)        1 2024-04-03 17:53:55.000000 skdir-0.0.6/skdir.egg-info/dependency_links.txt
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)       53 2024-04-03 17:53:55.000000 skdir-0.0.6/skdir.egg-info/requires.txt
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)        4 2024-04-03 17:53:55.000000 skdir-0.0.6/skdir.egg-info/top_level.txt
```

### Comparing `skdir-0.0.5/LICENSE` & `skdir-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `skdir-0.0.5/PKG-INFO` & `skdir-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skdir
-Version: 0.0.5
+Version: 0.0.6
 Summary: skdir
 Home-page: UNKNOWN
 Author: Sk
 Author-email: karnamsharath3@gmail.com
 License: UNKNOWN
 Keywords: arithmetic,math,mathematics,python tutorial,avi upadhyay
 Platform: UNKNOWN
```

### Comparing `skdir-0.0.5/README.md` & `skdir-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `skdir-0.0.5/lab/p1.py` & `skdir-0.0.6/lab/p1.py`

 * *Files identical despite different names*

### Comparing `skdir-0.0.5/lab/p2.py` & `skdir-0.0.6/lab/p2.py`

 * *Files identical despite different names*

### Comparing `skdir-0.0.5/lab/p3.py` & `skdir-0.0.6/lab/p3.py`

 * *Files identical despite different names*

### Comparing `skdir-0.0.5/lab/p4.py` & `skdir-0.0.6/lab/p4.py`

 * *Files identical despite different names*

### Comparing `skdir-0.0.5/lab/p5.py` & `skdir-0.0.6/lab/p5.py`

 * *Files identical despite different names*

### Comparing `skdir-0.0.5/lab/p6.py` & `skdir-0.0.6/lab/p6.py`

 * *Files identical despite different names*

### Comparing `skdir-0.0.5/lab/p7.py` & `skdir-0.0.6/lab/p7.py`

 * *Files identical despite different names*

### Comparing `skdir-0.0.5/lab/p8.py` & `skdir-0.0.6/lab/p8.py`

 * *Files identical despite different names*

### Comparing `skdir-0.0.5/setup.py` & `skdir-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 DESCRIPTION = 'skdir'
 LONG_DESCRIPTION = 'A package to perform arithmetic operations'
 
 # Setting up
 setup(
     name="skdir",
     version=VERSION,
```

### Comparing `skdir-0.0.5/skdir.egg-info/PKG-INFO` & `skdir-0.0.6/skdir.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skdir
-Version: 0.0.5
+Version: 0.0.6
 Summary: skdir
 Home-page: UNKNOWN
 Author: Sk
 Author-email: karnamsharath3@gmail.com
 License: UNKNOWN
 Keywords: arithmetic,math,mathematics,python tutorial,avi upadhyay
 Platform: UNKNOWN
```

