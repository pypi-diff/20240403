# Comparing `tmp/splotch-0.6.9.1.tar.gz` & `tmp/splotch-0.6.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splotch-0.6.9.1.tar", last modified: Wed Mar 27 23:53:37 2024, max compression
+gzip compressed data, was "splotch-0.6.9.2.tar", last modified: Wed Apr  3 01:40:36 2024, max compression
```

## Comparing `splotch-0.6.9.1.tar` & `splotch-0.6.9.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 mbravo    (1000) mbravo    (1000)        0 2024-03-27 23:53:37.955525 splotch-0.6.9.1/
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     1527 2020-05-15 14:21:48.000000 splotch-0.6.9.1/LICENSE
--rw-r--r--   0 mbravo    (1000) mbravo    (1000)      584 2024-03-27 23:53:37.954525 splotch-0.6.9.1/PKG-INFO
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     1802 2024-03-27 23:51:22.000000 splotch-0.6.9.1/README.md
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)       38 2024-03-27 23:53:37.955525 splotch-0.6.9.1/setup.cfg
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)      869 2024-03-27 23:52:31.000000 splotch-0.6.9.1/setup.py
-drwxrwxr-x   0 mbravo    (1000) mbravo    (1000)        0 2024-03-27 23:53:37.954525 splotch-0.6.9.1/splotch.egg-info/
--rw-r--r--   0 mbravo    (1000) mbravo    (1000)      584 2024-03-27 23:53:37.000000 splotch-0.6.9.1/splotch.egg-info/PKG-INFO
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)      402 2024-03-27 23:53:37.000000 splotch-0.6.9.1/splotch.egg-info/SOURCES.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)        1 2024-03-27 23:53:37.000000 splotch-0.6.9.1/splotch.egg-info/dependency_links.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)        1 2024-03-27 23:53:37.000000 splotch-0.6.9.1/splotch.egg-info/not-zip-safe
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)       84 2024-03-27 23:53:37.000000 splotch-0.6.9.1/splotch.egg-info/requires.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)        8 2024-03-27 23:53:37.000000 splotch-0.6.9.1/splotch.egg-info/top_level.txt
-drwxrwxr-x   0 mbravo    (1000) mbravo    (1000)        0 2024-03-27 23:53:37.949525 splotch-0.6.9.1/src/
-drwxrwxr-x   0 mbravo    (1000) mbravo    (1000)        0 2024-03-27 23:53:37.953525 splotch-0.6.9.1/src/splotch/
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)      413 2022-11-04 23:14:41.000000 splotch-0.6.9.1/src/splotch/__init__.py
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)    35092 2024-03-27 23:52:31.000000 splotch-0.6.9.1/src/splotch/axis_func.py
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)    24461 2024-03-27 23:52:31.000000 splotch-0.6.9.1/src/splotch/base_func.py
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)    12507 2022-11-04 23:14:41.000000 splotch-0.6.9.1/src/splotch/colorbar.py
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)      977 2023-02-02 21:18:26.000000 splotch-0.6.9.1/src/splotch/defaults.py
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)    62592 2024-03-27 23:52:31.000000 splotch-0.6.9.1/src/splotch/plots_1d.py
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)    75369 2024-03-27 23:52:31.000000 splotch-0.6.9.1/src/splotch/plots_2d.py
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     3180 2022-11-04 23:14:41.000000 splotch-0.6.9.1/src/splotch/styles.py
+drwxrwxr-x   0 mbravo    (1000) mbravo    (1000)        0 2024-04-03 01:40:36.367654 splotch-0.6.9.2/
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     1527 2020-05-15 14:21:48.000000 splotch-0.6.9.2/LICENSE
+-rw-r--r--   0 mbravo    (1000) mbravo    (1000)      584 2024-04-03 01:40:36.367654 splotch-0.6.9.2/PKG-INFO
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     1802 2024-04-03 01:38:05.000000 splotch-0.6.9.2/README.md
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)       38 2024-04-03 01:40:36.367654 splotch-0.6.9.2/setup.cfg
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)      869 2024-04-03 01:40:17.000000 splotch-0.6.9.2/setup.py
+drwxrwxr-x   0 mbravo    (1000) mbravo    (1000)        0 2024-04-03 01:40:36.366654 splotch-0.6.9.2/splotch.egg-info/
+-rw-r--r--   0 mbravo    (1000) mbravo    (1000)      584 2024-04-03 01:40:35.000000 splotch-0.6.9.2/splotch.egg-info/PKG-INFO
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)      402 2024-04-03 01:40:35.000000 splotch-0.6.9.2/splotch.egg-info/SOURCES.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)        1 2024-04-03 01:40:35.000000 splotch-0.6.9.2/splotch.egg-info/dependency_links.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)        1 2024-04-03 01:40:35.000000 splotch-0.6.9.2/splotch.egg-info/not-zip-safe
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)       84 2024-04-03 01:40:35.000000 splotch-0.6.9.2/splotch.egg-info/requires.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)        8 2024-04-03 01:40:35.000000 splotch-0.6.9.2/splotch.egg-info/top_level.txt
+drwxrwxr-x   0 mbravo    (1000) mbravo    (1000)        0 2024-04-03 01:40:36.361655 splotch-0.6.9.2/src/
+drwxrwxr-x   0 mbravo    (1000) mbravo    (1000)        0 2024-04-03 01:40:36.366654 splotch-0.6.9.2/src/splotch/
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)      413 2022-11-04 23:14:41.000000 splotch-0.6.9.2/src/splotch/__init__.py
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)    35092 2024-03-27 23:52:31.000000 splotch-0.6.9.2/src/splotch/axis_func.py
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)    24461 2024-03-27 23:52:31.000000 splotch-0.6.9.2/src/splotch/base_func.py
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)    12507 2022-11-04 23:14:41.000000 splotch-0.6.9.2/src/splotch/colorbar.py
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)      977 2023-02-02 21:18:26.000000 splotch-0.6.9.2/src/splotch/defaults.py
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)    62592 2024-03-27 23:52:31.000000 splotch-0.6.9.2/src/splotch/plots_1d.py
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)    75406 2024-04-03 01:40:17.000000 splotch-0.6.9.2/src/splotch/plots_2d.py
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     3180 2022-11-04 23:14:41.000000 splotch-0.6.9.2/src/splotch/styles.py
```

### Comparing `splotch-0.6.9.1/LICENSE` & `splotch-0.6.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `splotch-0.6.9.1/PKG-INFO` & `splotch-0.6.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splotch
-Version: 0.6.9.1
+Version: 0.6.9.2
 Summary: Simple PLOTs, Contours and Histograms is a small package with wrapper functions designed to simplify plotting calls from matplotlib.
 Home-page: https://github.com/MBravoS/splot
 Author: Matías A. Bravo Santa Cruz
 Author-email: matias.bravo@icrar.org
 License: BSD-3-Clause
 Requires-Python: >=3.3
 License-File: LICENSE
```

### Comparing `splotch-0.6.9.1/README.md` & `splotch-0.6.9.2/README.md`

 * *Files identical despite different names*

### Comparing `splotch-0.6.9.1/setup.py` & `splotch-0.6.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import atexit
 from setuptools import setup
 from setuptools.command.install import install
 
 setup(name='splotch',
-    version='0.6.9.1',
+    version='0.6.9.2',
     description='Simple PLOTs, Contours and Histograms is a small package with wrapper functions designed to simplify plotting calls from matplotlib.',
     url='https://github.com/MBravoS/splot',
     author='Matías A. Bravo Santa Cruz',
     author_email='matias.bravo@icrar.org',
     license='BSD-3-Clause',
     packages=['splotch'],
     package_dir={'splotch': 'src/splotch'},
```

### Comparing `splotch-0.6.9.1/splotch.egg-info/PKG-INFO` & `splotch-0.6.9.2/splotch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splotch
-Version: 0.6.9.1
+Version: 0.6.9.2
 Summary: Simple PLOTs, Contours and Histograms is a small package with wrapper functions designed to simplify plotting calls from matplotlib.
 Home-page: https://github.com/MBravoS/splot
 Author: Matías A. Bravo Santa Cruz
 Author-email: matias.bravo@icrar.org
 License: BSD-3-Clause
 Requires-Python: >=3.3
 License-File: LICENSE
```

### Comparing `splotch-0.6.9.1/src/splotch/axis_func.py` & `splotch-0.6.9.2/src/splotch/axis_func.py`

 * *Files identical despite different names*

### Comparing `splotch-0.6.9.1/src/splotch/base_func.py` & `splotch-0.6.9.2/src/splotch/base_func.py`

 * *Files identical despite different names*

### Comparing `splotch-0.6.9.1/src/splotch/colorbar.py` & `splotch-0.6.9.2/src/splotch/colorbar.py`

 * *Files identical despite different names*

### Comparing `splotch-0.6.9.1/src/splotch/defaults.py` & `splotch-0.6.9.2/src/splotch/defaults.py`

 * *Files identical despite different names*

### Comparing `splotch-0.6.9.1/src/splotch/plots_1d.py` & `splotch-0.6.9.2/src/splotch/plots_1d.py`

 * *Files identical despite different names*

### Comparing `splotch-0.6.9.1/src/splotch/plots_2d.py` & `splotch-0.6.9.2/src/splotch/plots_2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,21 +227,21 @@
     ylim = lims_handler(ylim, ax)
     
     # Check for list-like behaviour
     if not is_listlike(percent):
         percent = array([percent]).flatten()
     
     if not is_listlike(bin_type):
-        if not isinstance(bin_type, str):
+        if not isinstance(bin_type, str) and bin_type is not None:
             raise TypeError("bin_type must be a list-like object or a string")
         bin_type = [bin_type] * 2
 
     for btype in bin_type:
-        if btype not in ['number', 'width', 'edges', 'equal']:
-            raise ValueError(f"bin_type must be one of: 'number', 'width', 'edges', 'equal'. Instead got {btype}")
+        if btype not in ['number', 'width', 'edges', 'equal', None]:
+            raise ValueError(f"bin_type must be one of: 'number', 'width', 'edges', 'equal', None. Instead got {btype}")
     
     if not is_listlike(bins):
         if bins is None:
             bins = max([10, int(len(x)**0.4)])  # Defaults to min of 10 bins
         bins = [bins] * 2
     
     percent = percent[::-1]  # reverse the order of percent
```

### Comparing `splotch-0.6.9.1/src/splotch/styles.py` & `splotch-0.6.9.2/src/splotch/styles.py`

 * *Files identical despite different names*

