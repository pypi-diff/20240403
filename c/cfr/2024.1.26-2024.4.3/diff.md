# Comparing `tmp/cfr-2024.1.26.tar.gz` & `tmp/cfr-2024.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfr-2024.1.26.tar", last modified: Fri Jan 26 09:26:49 2024, max compression
+gzip compressed data, was "cfr-2024.4.3.tar", last modified: Wed Apr  3 20:14:11 2024, max compression
```

## Comparing `cfr-2024.1.26.tar` & `cfr-2024.4.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 fzhu       (501) staff       (20)        0 2024-01-26 09:26:49.234410 cfr-2024.1.26/
--rw-r--r--   0 fzhu       (501) staff       (20)     1516 2023-09-04 03:20:51.000000 cfr-2024.1.26/LICENSE
--rw-r--r--   0 fzhu       (501) staff       (20)     2684 2024-01-26 09:26:49.234139 cfr-2024.1.26/PKG-INFO
--rw-r--r--   0 fzhu       (501) staff       (20)     1421 2023-09-04 03:20:51.000000 cfr-2024.1.26/README.md
-drwxr-xr-x   0 fzhu       (501) staff       (20)        0 2024-01-26 09:26:49.223856 cfr-2024.1.26/bin/
--rw-r--r--   0 fzhu       (501) staff       (20)     5134 2023-09-04 03:20:51.000000 cfr-2024.1.26/bin/cfr
-drwxr-xr-x   0 fzhu       (501) staff       (20)        0 2024-01-26 09:26:49.229801 cfr-2024.1.26/cfr/
--rw-r--r--   0 fzhu       (501) staff       (20)      732 2023-09-04 03:20:51.000000 cfr-2024.1.26/cfr/__init__.py
--rw-r--r--   0 fzhu       (501) staff       (20)    27431 2024-01-26 09:16:29.000000 cfr-2024.1.26/cfr/climate.py
-drwxr-xr-x   0 fzhu       (501) staff       (20)        0 2024-01-26 09:26:49.232085 cfr-2024.1.26/cfr/da/
--rw-r--r--   0 fzhu       (501) staff       (20)       22 2023-09-04 03:20:51.000000 cfr-2024.1.26/cfr/da/__init__.py
--rw-r--r--   0 fzhu       (501) staff       (20)    16319 2023-09-04 03:20:51.000000 cfr-2024.1.26/cfr/da/enkf.py
--rw-r--r--   0 fzhu       (501) staff       (20)    22484 2023-09-04 03:20:51.000000 cfr-2024.1.26/cfr/gcm.py
--rw-r--r--   0 fzhu       (501) staff       (20)     7623 2023-09-04 03:20:51.000000 cfr-2024.1.26/cfr/ml.py
--rw-r--r--   0 fzhu       (501) staff       (20)    80829 2024-01-16 01:02:16.000000 cfr-2024.1.26/cfr/proxy.py
--rw-r--r--   0 fzhu       (501) staff       (20)    45570 2024-01-26 09:02:02.000000 cfr-2024.1.26/cfr/psm.py
--rw-r--r--   0 fzhu       (501) staff       (20)    60527 2024-01-26 08:57:21.000000 cfr-2024.1.26/cfr/reconjob.py
--rw-r--r--   0 fzhu       (501) staff       (20)     6083 2024-01-26 03:02:24.000000 cfr-2024.1.26/cfr/reconres.py
--rw-r--r--   0 fzhu       (501) staff       (20)    19837 2023-09-04 03:20:51.000000 cfr-2024.1.26/cfr/ts.py
--rw-r--r--   0 fzhu       (501) staff       (20)    25857 2024-01-26 08:35:41.000000 cfr-2024.1.26/cfr/utils.py
--rw-r--r--   0 fzhu       (501) staff       (20)    62418 2024-01-25 04:20:15.000000 cfr-2024.1.26/cfr/visual.py
-drwxr-xr-x   0 fzhu       (501) staff       (20)        0 2024-01-26 09:26:49.231738 cfr-2024.1.26/cfr.egg-info/
--rw-r--r--   0 fzhu       (501) staff       (20)     2684 2024-01-26 09:26:49.000000 cfr-2024.1.26/cfr.egg-info/PKG-INFO
--rw-r--r--   0 fzhu       (501) staff       (20)      373 2024-01-26 09:26:49.000000 cfr-2024.1.26/cfr.egg-info/SOURCES.txt
--rw-r--r--   0 fzhu       (501) staff       (20)        1 2024-01-26 09:26:49.000000 cfr-2024.1.26/cfr.egg-info/dependency_links.txt
--rw-r--r--   0 fzhu       (501) staff       (20)        1 2023-09-07 19:26:50.000000 cfr-2024.1.26/cfr.egg-info/not-zip-safe
--rw-r--r--   0 fzhu       (501) staff       (20)      201 2024-01-26 09:26:49.000000 cfr-2024.1.26/cfr.egg-info/requires.txt
--rw-r--r--   0 fzhu       (501) staff       (20)        4 2024-01-26 09:26:49.000000 cfr-2024.1.26/cfr.egg-info/top_level.txt
--rw-r--r--   0 fzhu       (501) staff       (20)       38 2024-01-26 09:26:49.234465 cfr-2024.1.26/setup.cfg
--rw-r--r--   0 fzhu       (501) staff       (20)     1454 2024-01-26 03:03:41.000000 cfr-2024.1.26/setup.py
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2024-04-03 20:14:11.879259 cfr-2024.4.3/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1516 2023-03-03 14:30:05.000000 cfr-2024.4.3/LICENSE
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     2683 2024-04-03 20:14:11.877837 cfr-2024.4.3/PKG-INFO
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1421 2024-03-13 16:55:21.000000 cfr-2024.4.3/README.md
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2024-04-03 20:14:11.790999 cfr-2024.4.3/bin/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     5134 2023-07-10 00:08:10.000000 cfr-2024.4.3/bin/cfr
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2024-04-03 20:14:11.807922 cfr-2024.4.3/cfr/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      732 2023-07-10 00:08:10.000000 cfr-2024.4.3/cfr/__init__.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    27431 2024-04-03 20:06:27.000000 cfr-2024.4.3/cfr/climate.py
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2024-04-03 20:14:11.873979 cfr-2024.4.3/cfr/da/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)       22 2023-03-03 14:30:05.000000 cfr-2024.4.3/cfr/da/__init__.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    16319 2023-03-26 05:47:23.000000 cfr-2024.4.3/cfr/da/enkf.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    22484 2023-04-17 17:43:24.000000 cfr-2024.4.3/cfr/gcm.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     7623 2023-03-03 14:30:05.000000 cfr-2024.4.3/cfr/ml.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    80829 2024-03-13 16:55:21.000000 cfr-2024.4.3/cfr/proxy.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    45544 2024-04-03 20:12:58.000000 cfr-2024.4.3/cfr/psm.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    60527 2024-03-13 16:55:21.000000 cfr-2024.4.3/cfr/reconjob.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     6083 2024-03-13 16:55:21.000000 cfr-2024.4.3/cfr/reconres.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    19837 2023-07-10 00:08:11.000000 cfr-2024.4.3/cfr/ts.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    25886 2024-04-03 20:09:47.000000 cfr-2024.4.3/cfr/utils.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    62418 2024-03-13 16:55:21.000000 cfr-2024.4.3/cfr/visual.py
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2024-04-03 20:14:11.876168 cfr-2024.4.3/cfr.egg-info/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     2683 2024-04-03 20:14:10.000000 cfr-2024.4.3/cfr.egg-info/PKG-INFO
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      373 2024-04-03 20:14:10.000000 cfr-2024.4.3/cfr.egg-info/SOURCES.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2024-04-03 20:14:10.000000 cfr-2024.4.3/cfr.egg-info/dependency_links.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2023-03-03 14:35:18.000000 cfr-2024.4.3/cfr.egg-info/not-zip-safe
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      201 2024-04-03 20:14:10.000000 cfr-2024.4.3/cfr.egg-info/requires.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)        4 2024-04-03 20:14:10.000000 cfr-2024.4.3/cfr.egg-info/top_level.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)       38 2024-04-03 20:14:11.879402 cfr-2024.4.3/setup.cfg
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1453 2024-04-03 20:10:08.000000 cfr-2024.4.3/setup.py
```

### Comparing `cfr-2024.1.26/LICENSE` & `cfr-2024.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cfr-2024.1.26/PKG-INFO` & `cfr-2024.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfr
-Version: 2024.1.26
+Version: 2024.4.3
 Summary: cfr: a Python package for Climate Field Reconstruction
 Home-page: https://github.com/fzhu2e/cfr
 Author: Feng Zhu, Julien Emile-Geay
 Author-email: fengzhu@ucar.edu, julieneg@usc.edu
 License: BSD 3-Clause
 Keywords: climate field reconstruction
 Classifier: Natural Language :: English
@@ -35,15 +35,15 @@
 Requires-Dist: torchvision; extra == "ml"
 Provides-Extra: graphem
 Requires-Dist: cython; extra == "graphem"
 Requires-Dist: scikit-learn; extra == "graphem"
 Requires-Dist: cfr-graphem; extra == "graphem"
 
 [![PyPI version](https://badge.fury.io/py/cfr.svg)](https://badge.fury.io/py/cfr)
-[![PyPI](https://img.shields.io/badge/python-3.10-blue.svg)]()
+[![PyPI](https://img.shields.io/badge/python-3.11-blue.svg)]()
 [![license](https://img.shields.io/github/license/fzhu2e/cfr.svg)]()
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7855587.svg)](https://doi.org/10.5281/zenodo.7855587)
 
 # `cfr`: a Python package for Climate Field Reconstruction
 
 `cfr` aims to provide a universal framework for climate field reconstruction (CFR).
 It provides a toolkit for
```

### Comparing `cfr-2024.1.26/README.md` & `cfr-2024.4.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [![PyPI version](https://badge.fury.io/py/cfr.svg)](https://badge.fury.io/py/cfr)
-[![PyPI](https://img.shields.io/badge/python-3.10-blue.svg)]()
+[![PyPI](https://img.shields.io/badge/python-3.11-blue.svg)]()
 [![license](https://img.shields.io/github/license/fzhu2e/cfr.svg)]()
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7855587.svg)](https://doi.org/10.5281/zenodo.7855587)
 
 # `cfr`: a Python package for Climate Field Reconstruction
 
 `cfr` aims to provide a universal framework for climate field reconstruction (CFR).
 It provides a toolkit for
```

### Comparing `cfr-2024.1.26/bin/cfr` & `cfr-2024.4.3/bin/cfr`

 * *Files identical despite different names*

### Comparing `cfr-2024.1.26/cfr/__init__.py` & `cfr-2024.4.3/cfr/__init__.py`

 * *Files identical despite different names*

### Comparing `cfr-2024.1.26/cfr/climate.py` & `cfr-2024.4.3/cfr/climate.py`

 * *Files identical despite different names*

### Comparing `cfr-2024.1.26/cfr/da/enkf.py` & `cfr-2024.4.3/cfr/da/enkf.py`

 * *Files identical despite different names*

### Comparing `cfr-2024.1.26/cfr/gcm.py` & `cfr-2024.4.3/cfr/gcm.py`

 * *Files identical despite different names*

### Comparing `cfr-2024.1.26/cfr/ml.py` & `cfr-2024.4.3/cfr/ml.py`

 * *Files identical despite different names*

### Comparing `cfr-2024.1.26/cfr/proxy.py` & `cfr-2024.4.3/cfr/proxy.py`

 * *Files identical despite different names*

### Comparing `cfr-2024.1.26/cfr/psm.py` & `cfr-2024.4.3/cfr/psm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from turtle import color
 import numpy as np
 import pandas as pd
 from datetime import datetime
 from scipy import integrate, signal, stats
 from tqdm import tqdm
 from multiprocessing import cpu_count
 try:
@@ -1139,8 +1138,8 @@
             ptype=self.pobj.ptype,
             value_name=self.pobj.value_name,
             value_unit=self.pobj.value_unit,
             time_name=self.pobj.time_name,
             time_unit=self.pobj.time_unit,
         )
 
-        return pp
+        return pp
```

### Comparing `cfr-2024.1.26/cfr/reconjob.py` & `cfr-2024.4.3/cfr/reconjob.py`

 * *Files identical despite different names*

### Comparing `cfr-2024.1.26/cfr/reconres.py` & `cfr-2024.4.3/cfr/reconres.py`

 * *Files identical despite different names*

### Comparing `cfr-2024.1.26/cfr/ts.py` & `cfr-2024.4.3/cfr/ts.py`

 * *Files identical despite different names*

### Comparing `cfr-2024.1.26/cfr/utils.py` & `cfr-2024.4.3/cfr/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -630,16 +630,16 @@
             replace_text = v
             text = text.replace(search_text, replace_text)
 
     with open(fpath, 'w') as f:
         f.write(text)
 
 
-def download(url: str, fname: str, chunk_size=1024, show_bar=True):
-    resp = requests.get(url, stream=True)
+def download(url: str, fname: str, chunk_size=1024, show_bar=True, verify=False):
+    resp = requests.get(url, stream=True, verify=verify)
     total = int(resp.headers.get('content-length', 0))
     if show_bar:
         with open(fname, 'wb') as file, tqdm(
             desc='Fetching data',
             total=total,
             unit='iB',
             unit_scale=True,
```

### Comparing `cfr-2024.1.26/cfr/visual.py` & `cfr-2024.4.3/cfr/visual.py`

 * *Files identical despite different names*

### Comparing `cfr-2024.1.26/cfr.egg-info/PKG-INFO` & `cfr-2024.4.3/cfr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfr
-Version: 2024.1.26
+Version: 2024.4.3
 Summary: cfr: a Python package for Climate Field Reconstruction
 Home-page: https://github.com/fzhu2e/cfr
 Author: Feng Zhu, Julien Emile-Geay
 Author-email: fengzhu@ucar.edu, julieneg@usc.edu
 License: BSD 3-Clause
 Keywords: climate field reconstruction
 Classifier: Natural Language :: English
@@ -35,15 +35,15 @@
 Requires-Dist: torchvision; extra == "ml"
 Provides-Extra: graphem
 Requires-Dist: cython; extra == "graphem"
 Requires-Dist: scikit-learn; extra == "graphem"
 Requires-Dist: cfr-graphem; extra == "graphem"
 
 [![PyPI version](https://badge.fury.io/py/cfr.svg)](https://badge.fury.io/py/cfr)
-[![PyPI](https://img.shields.io/badge/python-3.10-blue.svg)]()
+[![PyPI](https://img.shields.io/badge/python-3.11-blue.svg)]()
 [![license](https://img.shields.io/github/license/fzhu2e/cfr.svg)]()
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7855587.svg)](https://doi.org/10.5281/zenodo.7855587)
 
 # `cfr`: a Python package for Climate Field Reconstruction
 
 `cfr` aims to provide a universal framework for climate field reconstruction (CFR).
 It provides a toolkit for
```

### Comparing `cfr-2024.1.26/setup.py` & `cfr-2024.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='cfr',  # required
-    version='2024.1.26',
+    version='2024.4.3',
     description='cfr: a Python package for Climate Field Reconstruction',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author='Feng Zhu, Julien Emile-Geay',
     author_email='fengzhu@ucar.edu, julieneg@usc.edu',
     url='https://github.com/fzhu2e/cfr',
     packages=find_packages(),
```

