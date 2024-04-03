# Comparing `tmp/nheri_simcenter-0.9.8.tar.gz` & `tmp/nheri_simcenter-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nheri_simcenter-0.9.8.tar", last modified: Thu Apr 20 23:41:54 2023, max compression
+gzip compressed data, was "nheri_simcenter-0.9.9.tar", last modified: Wed Jul  5 17:36:44 2023, max compression
```

## Comparing `nheri_simcenter-0.9.8.tar` & `nheri_simcenter-0.9.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2023-04-20 23:41:54.613474 nheri_simcenter-0.9.8/
--rw-r--r--   0 adamzs     (504) staff       (20)     1669 2021-01-11 23:23:41.000000 nheri_simcenter-0.9.8/LICENSE
--rw-r--r--   0 adamzs     (504) staff       (20)     2071 2023-04-20 23:41:54.613307 nheri_simcenter-0.9.8/PKG-INFO
--rw-r--r--   0 adamzs     (504) staff       (20)     1051 2021-01-11 23:36:45.000000 nheri_simcenter-0.9.8/README.md
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2023-04-20 23:41:54.612333 nheri_simcenter-0.9.8/nheri_simcenter/
--rw-r--r--   0 adamzs     (504) staff       (20)     2116 2023-04-20 23:39:12.000000 nheri_simcenter-0.9.8/nheri_simcenter/__init__.py
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2023-04-20 23:41:54.612979 nheri_simcenter-0.9.8/nheri_simcenter.egg-info/
--rw-r--r--   0 adamzs     (504) staff       (20)     2071 2023-04-20 23:41:54.000000 nheri_simcenter-0.9.8/nheri_simcenter.egg-info/PKG-INFO
--rw-r--r--   0 adamzs     (504) staff       (20)      248 2023-04-20 23:41:54.000000 nheri_simcenter-0.9.8/nheri_simcenter.egg-info/SOURCES.txt
--rw-r--r--   0 adamzs     (504) staff       (20)        1 2023-04-20 23:41:54.000000 nheri_simcenter-0.9.8/nheri_simcenter.egg-info/dependency_links.txt
--rw-r--r--   0 adamzs     (504) staff       (20)      155 2023-04-20 23:41:54.000000 nheri_simcenter-0.9.8/nheri_simcenter.egg-info/requires.txt
--rw-r--r--   0 adamzs     (504) staff       (20)       16 2023-04-20 23:41:54.000000 nheri_simcenter-0.9.8/nheri_simcenter.egg-info/top_level.txt
--rw-r--r--   0 adamzs     (504) staff       (20)       38 2023-04-20 23:41:54.613522 nheri_simcenter-0.9.8/setup.cfg
--rw-r--r--   0 adamzs     (504) staff       (20)     2050 2023-04-20 23:38:54.000000 nheri_simcenter-0.9.8/setup.py
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2023-07-05 17:36:44.563764 nheri_simcenter-0.9.9/
+-rw-r--r--   0 adamzs     (504) staff       (20)     1669 2021-01-11 23:23:41.000000 nheri_simcenter-0.9.9/LICENSE
+-rw-r--r--   0 adamzs     (504) staff       (20)     2071 2023-07-05 17:36:44.563651 nheri_simcenter-0.9.9/PKG-INFO
+-rw-r--r--   0 adamzs     (504) staff       (20)     1051 2021-01-11 23:36:45.000000 nheri_simcenter-0.9.9/README.md
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2023-07-05 17:36:44.562818 nheri_simcenter-0.9.9/nheri_simcenter/
+-rw-r--r--   0 adamzs     (504) staff       (20)     2116 2023-07-05 17:35:15.000000 nheri_simcenter-0.9.9/nheri_simcenter/__init__.py
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2023-07-05 17:36:44.563490 nheri_simcenter-0.9.9/nheri_simcenter.egg-info/
+-rw-r--r--   0 adamzs     (504) staff       (20)     2071 2023-07-05 17:36:44.000000 nheri_simcenter-0.9.9/nheri_simcenter.egg-info/PKG-INFO
+-rw-r--r--   0 adamzs     (504) staff       (20)      248 2023-07-05 17:36:44.000000 nheri_simcenter-0.9.9/nheri_simcenter.egg-info/SOURCES.txt
+-rw-r--r--   0 adamzs     (504) staff       (20)        1 2023-07-05 17:36:44.000000 nheri_simcenter-0.9.9/nheri_simcenter.egg-info/dependency_links.txt
+-rw-r--r--   0 adamzs     (504) staff       (20)      162 2023-07-05 17:36:44.000000 nheri_simcenter-0.9.9/nheri_simcenter.egg-info/requires.txt
+-rw-r--r--   0 adamzs     (504) staff       (20)       16 2023-07-05 17:36:44.000000 nheri_simcenter-0.9.9/nheri_simcenter.egg-info/top_level.txt
+-rw-r--r--   0 adamzs     (504) staff       (20)       38 2023-07-05 17:36:44.563799 nheri_simcenter-0.9.9/setup.cfg
+-rw-r--r--   0 adamzs     (504) staff       (20)     2069 2023-07-05 17:34:58.000000 nheri_simcenter-0.9.9/setup.py
```

### Comparing `nheri_simcenter-0.9.8/LICENSE` & `nheri_simcenter-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nheri_simcenter-0.9.8/PKG-INFO` & `nheri_simcenter-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nheri_simcenter
-Version: 0.9.8
+Version: 0.9.9
 Summary: NHERI SimCenter Python Dependencies
 Home-page: http://nheri-simcenter.github.io/nheri_simcenter/
 Author: Adam Zsarnóczay
 Author-email: adamzs@stanford.edu
 License: BSD License
 Platform: any
 Classifier: Programming Language :: Python
```

### Comparing `nheri_simcenter-0.9.8/README.md` & `nheri_simcenter-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `nheri_simcenter-0.9.8/nheri_simcenter/__init__.py` & `nheri_simcenter-0.9.9/nheri_simcenter/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 # nheri_simcenter. If not, see <http://www.opensource.org/licenses/>.
 #
 # Contributors:
 # Adam Zsarnóczay
 
 name = "nheri_simcenter"
 
-__version__ = '0.9.8'
+__version__ = '0.9.9'
 
 __copyright__ = """Copyright (c) 2018 Leland Stanford Junior University and
 The Regents of the University of California"""
 
 __license__ = "BSD 3-Clause License"
```

### Comparing `nheri_simcenter-0.9.8/nheri_simcenter.egg-info/PKG-INFO` & `nheri_simcenter-0.9.9/nheri_simcenter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nheri-simcenter
-Version: 0.9.8
+Version: 0.9.9
 Summary: NHERI SimCenter Python Dependencies
 Home-page: http://nheri-simcenter.github.io/nheri_simcenter/
 Author: Adam Zsarnóczay
 Author-email: adamzs@stanford.edu
 License: BSD License
 Platform: any
 Classifier: Programming Language :: Python
```

### Comparing `nheri_simcenter-0.9.8/setup.py` & `nheri_simcenter-0.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,16 @@
         'openseespy',
         'scikit-learn',
         'plotly',
         'colorlover',
         'jpype1',
         'tqdm',
         'gpy',
-        'emukit'
+        'emukit',
+        'psutil'
     ],
     classifiers = [
         'Programming Language :: Python',
         'Development Status :: 5 - Production/Stable',
         'Natural Language :: English',
         'Environment :: Console',
         'Framework :: Jupyter',
```

