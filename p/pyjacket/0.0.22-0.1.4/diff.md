# Comparing `tmp/pyjacket-0.0.22.tar.gz` & `tmp/pyjacket-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjacket-0.0.22.tar", last modified: Fri Sep  1 09:19:42 2023, max compression
+gzip compressed data, was "pyjacket-0.1.4.tar", last modified: Wed Apr  3 16:43:17 2024, max compression
```

## Comparing `pyjacket-0.0.22.tar` & `pyjacket-0.1.4.tar`

### file list

```diff
@@ -1,33 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 09:19:42.774132 pyjacket-0.0.22/
--rw-r--r--   0 runner    (1001) docker     (999)     1063 2023-09-01 09:19:23.000000 pyjacket-0.0.22/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)      607 2023-09-01 09:19:42.774132 pyjacket-0.0.22/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)       29 2023-09-01 09:19:23.000000 pyjacket-0.0.22/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 09:19:42.770132 pyjacket-0.0.22/pyjacket/
--rw-r--r--   0 runner    (1001) docker     (999)       45 2023-09-01 09:19:23.000000 pyjacket-0.0.22/pyjacket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 09:19:42.770132 pyjacket-0.0.22/pyjacket/cvtools/
--rw-r--r--   0 runner    (1001) docker     (999)       29 2023-09-01 09:19:23.000000 pyjacket-0.0.22/pyjacket/cvtools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 09:19:42.770132 pyjacket-0.0.22/pyjacket/cvtools/_imwrite/
--rw-r--r--   0 runner    (1001) docker     (999)      894 2023-09-01 09:19:23.000000 pyjacket-0.0.22/pyjacket/cvtools/_imwrite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      101 2023-09-01 09:19:23.000000 pyjacket-0.0.22/pyjacket/cvtools/_imwrite/imwrite_tif.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 09:19:42.770132 pyjacket-0.0.22/pyjacket/cvtools/filetools/
--rw-r--r--   0 runner    (1001) docker     (999)       97 2023-09-01 09:19:23.000000 pyjacket-0.0.22/pyjacket/cvtools/filetools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 09:19:42.770132 pyjacket-0.0.22/pyjacket/cvtools/imread/
--rw-r--r--   0 runner    (1001) docker     (999)     1336 2023-09-01 09:19:23.000000 pyjacket-0.0.22/pyjacket/cvtools/imread/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     3452 2023-09-01 09:19:23.000000 pyjacket-0.0.22/pyjacket/cvtools/imread/imread_nd2.py
--rw-r--r--   0 runner    (1001) docker     (999)      189 2023-09-01 09:19:23.000000 pyjacket-0.0.22/pyjacket/cvtools/imread/imread_tif.py
--rw-r--r--   0 runner    (1001) docker     (999)      253 2023-09-01 09:19:23.000000 pyjacket-0.0.22/pyjacket/cvtools/imread/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 09:19:42.770132 pyjacket-0.0.22/pyjacket/cvtools/roi/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-01 09:19:23.000000 pyjacket-0.0.22/pyjacket/cvtools/roi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1338 2023-09-01 09:19:23.000000 pyjacket-0.0.22/pyjacket/cvtools/roi/select.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 09:19:42.770132 pyjacket-0.0.22/pyjacket/graphs/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-01 09:19:23.000000 pyjacket-0.0.22/pyjacket/graphs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      185 2023-09-01 09:19:23.000000 pyjacket-0.0.22/pyjacket/graphs/markov.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 09:19:42.774132 pyjacket-0.0.22/pyjacket/ntheory/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-01 09:19:23.000000 pyjacket-0.0.22/pyjacket/ntheory/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 09:19:42.770132 pyjacket-0.0.22/pyjacket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)      607 2023-09-01 09:19:42.000000 pyjacket-0.0.22/pyjacket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      617 2023-09-01 09:19:42.000000 pyjacket-0.0.22/pyjacket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-01 09:19:42.000000 pyjacket-0.0.22/pyjacket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)        9 2023-09-01 09:19:42.000000 pyjacket-0.0.22/pyjacket.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-09-01 09:19:42.774132 pyjacket-0.0.22/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)     1114 2023-09-01 09:19:23.000000 pyjacket-0.0.22/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:43:17.454429 pyjacket-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-03 16:43:07.000000 pyjacket-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-03 16:43:17.454429 pyjacket-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-03 16:43:07.000000 pyjacket-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:43:17.446429 pyjacket-0.1.4/pyjacket/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:43:17.450429 pyjacket-0.1.4/pyjacket/arrtools/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/arrtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/arrtools/arrtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/arrtools/bitdepth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/arrtools/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/arrtools/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/arrtools/rois.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/arrtools/sizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/arrtools/skeletonize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/arrtools/slicing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/arrtools/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:43:17.450429 pyjacket-0.1.4/pyjacket/chemistry/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/chemistry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:43:17.450429 pyjacket-0.1.4/pyjacket/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/core/all_same.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/core/batched.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/core/digits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/core/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/core/find_nth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/core/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/core/iterations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/core/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/core/python_ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/core/rounding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/core/sortby.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/core/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:43:17.450429 pyjacket-0.1.4/pyjacket/cvtools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/cvtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/cvtools/color_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/cvtools/color_picker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/cvtools/color_slicing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:43:17.450429 pyjacket-0.1.4/pyjacket/filetools/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/filetools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:43:17.454429 pyjacket-0.1.4/pyjacket/filetools/_imread/
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/filetools/_imread/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/filetools/_imread/imread_nd2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/filetools/_imread/imread_tif.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/filetools/_imread/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:43:17.454429 pyjacket-0.1.4/pyjacket/filetools/_imwrite/
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/filetools/_imwrite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/filetools/_imwrite/imwrite_tif.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/filetools/filemanager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:43:17.454429 pyjacket-0.1.4/pyjacket/graphs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/graphs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/graphs/absorbing_markov.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/graphs/markov.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:43:17.454429 pyjacket-0.1.4/pyjacket/ntheory/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/ntheory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/ntheory/factors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:43:17.454429 pyjacket-0.1.4/pyjacket/ntheory/modulo/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/ntheory/modulo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/ntheory/modulo/modular_arithmetic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:43:17.454429 pyjacket-0.1.4/pyjacket/ntheory/primes/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/ntheory/primes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/ntheory/primes/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/ntheory/primes/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:43:17.454429 pyjacket-0.1.4/pyjacket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-03 16:43:17.000000 pyjacket-0.1.4/pyjacket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-03 16:43:17.000000 pyjacket-0.1.4/pyjacket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 16:43:17.000000 pyjacket-0.1.4/pyjacket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 16:43:17.000000 pyjacket-0.1.4/pyjacket.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 16:43:17.454429 pyjacket-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-03 16:43:07.000000 pyjacket-0.1.4/setup.py
```

### Comparing `pyjacket-0.0.22/LICENSE` & `pyjacket-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjacket-0.0.22/PKG-INFO` & `pyjacket-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjacket
-Version: 0.0.22
+Version: 0.1.4
 Summary: Lorem ipsum
 Home-page: https://github.com/Kasper-Arfman/pyjacket
 Download-URL: http://pypi.python.org/pypi/pyjacket
 Author: Kasper Arfman
 Author-email: Kasper.arf@gmail.com
 Project-URL: Source, https://github.com/Kasper-Arfman/pyjacket
 Project-URL: Tracker, https://github.com/Kasper-Arfman/pyjacket/issues
```

### Comparing `pyjacket-0.0.22/pyjacket/cvtools/_imwrite/__init__.py` & `pyjacket-0.1.4/pyjacket/filetools/_imwrite/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjacket-0.0.22/pyjacket/cvtools/imread/__init__.py` & `pyjacket-0.1.4/pyjacket/filetools/_imread/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,72 +1,65 @@
+from abc import ABC
+import numpy as np
 
-x = 5
+from .imread_nd2 import imread_nd2, MetadataND2
+from .imread_tif import imread_tif
 
 
-def imread():
-    return 'x'
 
-# from abc import ABC
-# import numpy as np
 
-# from .imread_nd2 import imread_nd2, MetadataND2
-# from .imread_tif import imread_tif
 
-
-
-
-
-# def imread(filepath: str) -> np.ndarray:
-#     """
-#     """
-#     if not '.' in filepath: raise ValueError(f"missing extension in filename: {filepath}")
+def imread(filepath: str) -> np.ndarray:
+    """
+    """
+    if not '.' in filepath: raise ValueError(f"missing extension in filename: {filepath}")
     
-#     ext = filepath.split('.')[-1]
+    ext = filepath.split('.')[-1]
     
-#     # allow reading various data formats
-#     read_function = {
-#         'nd2': imread_nd2,
-#         'tif': imread_tif,
-#     }.get(ext)
+    # allow reading various data formats
+    read_function = {
+        'nd2': imread_nd2,
+        'tif': imread_tif,
+    }.get(ext)
     
-#     if not read_function:
-#         raise NotImplementedError(f'Cannot read image of type {ext}')
+    if not read_function:
+        raise NotImplementedError(f'Cannot read image of type {ext}')
     
-#     return read_function(filepath)
+    return read_function(filepath)
 
 
 
-# class Metadata(ABC):
+class Metadata(ABC):
             
-#     @property        
-#     def exposure_time(self): ...
+    @property        
+    def exposure_time(self): ...
     
-#     @property
-#     def light_intensity(self): ...
+    @property
+    def light_intensity(self): ...
     
-#     @property
-#     def period(self): ...
+    @property
+    def period(self): ...
     
-#     @property
-#     def fps(self): ...
+    @property
+    def fps(self): ...
     
-#     @property
-#     def total_duration(self): ...
+    @property
+    def total_duration(self): ...
 
 
 
 
 
 
-# def imread_meta(filepath: str) -> Metadata:
-#     """
-#     """
-#     if not '.' in filepath: raise ValueError(f"missing extension in filename: {filepath}")
+def imread_meta(filepath: str) -> Metadata:
+    """
+    """
+    if not '.' in filepath: raise ValueError(f"missing extension in filename: {filepath}")
     
-#     ext = filepath.split('.')[-1]
+    ext = filepath.split('.')[-1]
     
-#     # allow reading various data formats
-#     Constructor = {
-#         'nd2': MetadataND2,
-#     }.get(ext)
+    # allow reading various data formats
+    Constructor = {
+        'nd2': MetadataND2,
+    }.get(ext)
     
-#     return Constructor(filepath)
+    return Constructor(filepath)
```

### Comparing `pyjacket-0.0.22/pyjacket/cvtools/imread/imread_nd2.py` & `pyjacket-0.1.4/pyjacket/filetools/_imread/imread_nd2.py`

 * *Files identical despite different names*

### Comparing `pyjacket-0.0.22/pyjacket.egg-info/PKG-INFO` & `pyjacket-0.1.4/pyjacket.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjacket
-Version: 0.0.22
+Version: 0.1.4
 Summary: Lorem ipsum
 Home-page: https://github.com/Kasper-Arfman/pyjacket
 Download-URL: http://pypi.python.org/pypi/pyjacket
 Author: Kasper Arfman
 Author-email: Kasper.arf@gmail.com
 Project-URL: Source, https://github.com/Kasper-Arfman/pyjacket
 Project-URL: Tracker, https://github.com/Kasper-Arfman/pyjacket/issues
```

### Comparing `pyjacket-0.0.22/setup.py` & `pyjacket-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-__version__ = '0.0.22'
+__version__ = '0.1.4'
 
 GIT_USER = 'Kasper-Arfman'
 NAME = 'pyjacket'
 
 setuptools.setup(
     name=NAME,
     version=__version__,
@@ -31,8 +31,8 @@
     # python_requires="",
     # entry_points=[],
     install_requires=[],
 
     # # Add _ prefix to the names of temporary build dirs
     # options={'build': {'build_base': '_build'}, },
     # zip_safe=True,
-)
+)
```

