# Comparing `tmp/asto-0.0.8.tar.gz` & `tmp/asto-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asto-0.0.8.tar", last modified: Fri Nov 17 14:29:12 2023, max compression
+gzip compressed data, was "asto-0.0.9.tar", last modified: Mon Nov 20 16:03:33 2023, max compression
```

## Comparing `asto-0.0.8.tar` & `asto-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-11-17 14:29:12.041345 asto-0.0.8/
--rw-r--r--   0 solst      (501) staff       (20)    11337 2023-11-07 15:11:12.000000 asto-0.0.8/LICENSE
--rw-r--r--   0 solst      (501) staff       (20)      111 2023-11-07 15:11:12.000000 asto-0.0.8/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     2020 2023-11-17 14:29:12.041192 asto-0.0.8/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)     1431 2023-11-07 15:18:51.000000 asto-0.0.8/README.md
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-11-17 14:29:12.040027 asto-0.0.8/asto/
--rw-r--r--   0 solst      (501) staff       (20)      818 2023-11-17 13:51:49.000000 asto-0.0.8/asto/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)     3367 2023-11-17 13:51:49.000000 asto-0.0.8/asto/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)     1683 2023-11-17 13:51:49.000000 asto-0.0.8/asto/arng.py
--rw-r--r--   0 solst      (501) staff       (20)     3891 2023-11-17 13:51:49.000000 asto-0.0.8/asto/arrs.py
--rw-r--r--   0 solst      (501) staff       (20)      917 2023-11-17 13:51:49.000000 asto-0.0.8/asto/cast.py
--rw-r--r--   0 solst      (501) staff       (20)      376 2023-11-17 13:51:49.000000 asto-0.0.8/asto/dict.py
--rw-r--r--   0 solst      (501) staff       (20)     1128 2023-11-17 13:51:49.000000 asto-0.0.8/asto/nums.py
--rw-r--r--   0 solst      (501) staff       (20)      731 2023-11-17 13:51:49.000000 asto-0.0.8/asto/time.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-11-17 14:29:12.041010 asto-0.0.8/asto.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     2020 2023-11-17 14:29:12.000000 asto-0.0.8/asto.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      359 2023-11-17 14:29:12.000000 asto-0.0.8/asto.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-11-17 14:29:12.000000 asto-0.0.8/asto.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)       30 2023-11-17 14:29:12.000000 asto-0.0.8/asto.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-11-07 15:18:43.000000 asto-0.0.8/asto.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)       83 2023-11-17 14:29:12.000000 asto-0.0.8/asto.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        5 2023-11-17 14:29:12.000000 asto-0.0.8/asto.egg-info/top_level.txt
--rw-r--r--   0 solst      (501) staff       (20)      860 2023-11-13 14:36:26.000000 asto-0.0.8/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2023-11-17 14:29:12.041385 asto-0.0.8/setup.cfg
--rw-r--r--   0 solst      (501) staff       (20)     2580 2023-11-07 15:11:12.000000 asto-0.0.8/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-11-20 16:03:33.985983 asto-0.0.9/
+-rw-r--r--   0 solst      (501) staff       (20)    11337 2023-11-07 15:11:12.000000 asto-0.0.9/LICENSE
+-rw-r--r--   0 solst      (501) staff       (20)      111 2023-11-07 15:11:12.000000 asto-0.0.9/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     2020 2023-11-20 16:03:33.985854 asto-0.0.9/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     1431 2023-11-07 15:18:51.000000 asto-0.0.9/README.md
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-11-20 16:03:33.984736 asto-0.0.9/asto/
+-rw-r--r--   0 solst      (501) staff       (20)      818 2023-11-20 16:03:30.000000 asto-0.0.9/asto/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)     3811 2023-11-20 16:03:30.000000 asto-0.0.9/asto/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)     1721 2023-11-20 16:03:30.000000 asto-0.0.9/asto/arng.py
+-rw-r--r--   0 solst      (501) staff       (20)     3891 2023-11-20 16:03:30.000000 asto-0.0.9/asto/arrs.py
+-rw-r--r--   0 solst      (501) staff       (20)      917 2023-11-20 16:03:30.000000 asto-0.0.9/asto/cast.py
+-rw-r--r--   0 solst      (501) staff       (20)      376 2023-11-20 16:03:30.000000 asto-0.0.9/asto/dict.py
+-rw-r--r--   0 solst      (501) staff       (20)     1128 2023-11-20 16:03:30.000000 asto-0.0.9/asto/nums.py
+-rw-r--r--   0 solst      (501) staff       (20)     1448 2023-11-20 16:03:30.000000 asto-0.0.9/asto/slcs.py
+-rw-r--r--   0 solst      (501) staff       (20)      731 2023-11-20 16:03:30.000000 asto-0.0.9/asto/time.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-11-20 16:03:33.985688 asto-0.0.9/asto.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     2020 2023-11-20 16:03:33.000000 asto-0.0.9/asto.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      372 2023-11-20 16:03:33.000000 asto-0.0.9/asto.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-11-20 16:03:33.000000 asto-0.0.9/asto.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)       30 2023-11-20 16:03:33.000000 asto-0.0.9/asto.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-11-07 15:18:43.000000 asto-0.0.9/asto.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)       83 2023-11-20 16:03:33.000000 asto-0.0.9/asto.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        5 2023-11-20 16:03:33.000000 asto-0.0.9/asto.egg-info/top_level.txt
+-rw-r--r--   0 solst      (501) staff       (20)      860 2023-11-17 14:30:40.000000 asto-0.0.9/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2023-11-20 16:03:33.986024 asto-0.0.9/setup.cfg
+-rw-r--r--   0 solst      (501) staff       (20)     2580 2023-11-07 15:11:12.000000 asto-0.0.9/setup.py
```

### Comparing `asto-0.0.8/LICENSE` & `asto-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `asto-0.0.8/PKG-INFO` & `asto-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asto
-Version: 0.0.8
+Version: 0.0.9
 Summary: asto
 Home-page: https://github.com/dsm-72/asto
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: as to convert from one type another
 Classifier: Development Status :: 4 - Beta
```

### Comparing `asto-0.0.8/README.md` & `asto-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `asto-0.0.8/asto/__init__.py` & `asto-0.0.9/asto/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00__init__.ipynb.
 
 # %% auto 0
 __all__ = []
 
 # %% ../nbs/00__init__.ipynb 3
 import itertools
```

### Comparing `asto-0.0.8/asto/_modidx.py` & `asto-0.0.9/asto/_modidx.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,9 +35,14 @@
                            'asto.arrs.try2arr': ('arrs.html#try2arr', 'asto/arrs.py')},
             'asto.cast': {'asto.cast.cast': ('cast.html#cast', 'asto/cast.py'), 'asto.cast.caster': ('cast.html#caster', 'asto/cast.py')},
             'asto.dict': {},
             'asto.nums': { 'asto.nums.ascomplex': ('nums.html#ascomplex', 'asto/nums.py'),
                            'asto.nums.asfloat': ('nums.html#asfloat', 'asto/nums.py'),
                            'asto.nums.asint': ('nums.html#asint', 'asto/nums.py'),
                            'asto.nums.asnum': ('nums.html#asnum', 'asto/nums.py')},
+            'asto.slcs': { 'asto.slcs.asslc': ('slcs.html#asslc', 'asto/slcs.py'),
+                           'asto.slcs.safeslice': ('slcs.html#safeslice', 'asto/slcs.py'),
+                           'asto.slcs.slcchain': ('slcs.html#slcchain', 'asto/slcs.py'),
+                           'asto.slcs.slice2list': ('slcs.html#slice2list', 'asto/slcs.py'),
+                           'asto.slcs.try2slc': ('slcs.html#try2slc', 'asto/slcs.py')},
             'asto.time': { 'asto.time.day2hours': ('time.html#day2hours', 'asto/time.py'),
                            'asto.time.day2hrs': ('time.html#day2hrs', 'asto/time.py')}}}
```

### Comparing `asto-0.0.8/asto/arng.py` & `asto-0.0.9/asto/arng.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,16 +38,18 @@
     return isarr(a) and np.all(np.ediff1d(a) == 1)
 
 def arngchain(x, funcs, *args, **kwargs): 
     return applyfns(x, funcs, isarng, *args, **kwargs)
 
 def try2arng(a) -> NPArray:
     if isarng(a): return a
-    arange = np.arange(_safe_len(a))
-    return arange
+    try:
+        arange = np.arange(_safe_len(a))
+        return arange
+    except: return a
 
 def arr2arng(a: IndexLike) -> NPArray:
     if isarng(a): return a
     arange = np.arange(len(asarr(a)))
     return arange
 
 def df2arng(df: DataFrame) -> NPArray:
```

### Comparing `asto-0.0.8/asto/arrs.py` & `asto-0.0.9/asto/arrs.py`

 * *Files identical despite different names*

### Comparing `asto-0.0.8/asto/cast.py` & `asto-0.0.9/asto/cast.py`

 * *Files identical despite different names*

### Comparing `asto-0.0.8/asto/nums.py` & `asto-0.0.9/asto/nums.py`

 * *Files identical despite different names*

### Comparing `asto-0.0.8/asto/time.py` & `asto-0.0.9/asto/time.py`

 * *Files identical despite different names*

### Comparing `asto-0.0.8/asto.egg-info/PKG-INFO` & `asto-0.0.9/asto.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asto
-Version: 0.0.8
+Version: 0.0.9
 Summary: asto
 Home-page: https://github.com/dsm-72/asto
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: as to convert from one type another
 Classifier: Development Status :: 4 - Beta
```

### Comparing `asto-0.0.8/settings.ini` & `asto-0.0.9/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = asto
 lib_name = asto
-version = 0.0.8
+version = 0.0.9
 min_python = 3.11
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = asto
 nbs_path = nbs
 recursive = True
```

### Comparing `asto-0.0.8/setup.py` & `asto-0.0.9/setup.py`

 * *Files identical despite different names*

