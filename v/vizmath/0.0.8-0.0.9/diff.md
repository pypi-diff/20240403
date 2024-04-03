# Comparing `tmp/vizmath-0.0.8.tar.gz` & `tmp/vizmath-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\vizmath-0.0.8.tar", last modified: Tue Nov 28 03:57:40 2023, max compression
+gzip compressed data, was "dist\vizmath-0.0.9.tar", last modified: Tue Nov 28 04:13:43 2023, max compression
```

## Comparing `vizmath-0.0.8.tar` & `vizmath-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-11-28 03:57:40.000000 vizmath-0.0.8/
--rw-rw-rw-   0        0        0      491 2023-11-28 03:57:40.000000 vizmath-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       78 2023-06-27 01:09:47.000000 vizmath-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-11-28 03:57:40.000000 vizmath-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      881 2023-11-28 03:56:47.000000 vizmath-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-11-28 03:57:40.000000 vizmath-0.0.8/vizmath/
--rw-rw-rw-   0        0        0      135 2023-11-28 03:56:37.000000 vizmath-0.0.8/vizmath/__init__.py
--rw-rw-rw-   0        0        0     6285 2023-11-27 04:38:53.000000 vizmath-0.0.8/vizmath/binary_tree.py
--rw-rw-rw-   0        0        0     1825 2023-11-27 05:49:46.000000 vizmath-0.0.8/vizmath/draw.py
--rw-rw-rw-   0        0        0      624 2023-11-27 06:12:31.000000 vizmath-0.0.8/vizmath/examples.py
--rw-rw-rw-   0        0        0    14628 2023-11-26 00:36:20.000000 vizmath-0.0.8/vizmath/functions.py
--rw-rw-rw-   0        0        0    14853 2023-11-27 06:10:51.000000 vizmath-0.0.8/vizmath/radial_treemap.py
-drwxrwxrwx   0        0        0        0 2023-11-28 03:57:40.000000 vizmath-0.0.8/vizmath.egg-info/
--rw-rw-rw-   0        0        0      491 2023-11-28 03:57:40.000000 vizmath-0.0.8/vizmath.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-11-28 03:57:40.000000 vizmath-0.0.8/vizmath.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-28 03:57:40.000000 vizmath-0.0.8/vizmath.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-11-28 03:57:40.000000 vizmath-0.0.8/vizmath.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-11-28 03:57:40.000000 vizmath-0.0.8/vizmath.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-11-28 04:13:43.000000 vizmath-0.0.9/
+-rw-rw-rw-   0        0        0      491 2023-11-28 04:13:43.000000 vizmath-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       78 2023-06-27 01:09:47.000000 vizmath-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-11-28 04:13:43.000000 vizmath-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      881 2023-11-28 04:12:55.000000 vizmath-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-11-28 04:13:43.000000 vizmath-0.0.9/vizmath/
+-rw-rw-rw-   0        0        0      135 2023-11-28 04:12:49.000000 vizmath-0.0.9/vizmath/__init__.py
+-rw-rw-rw-   0        0        0     6285 2023-11-27 04:38:53.000000 vizmath-0.0.9/vizmath/binary_tree.py
+-rw-rw-rw-   0        0        0     1832 2023-11-28 04:07:07.000000 vizmath-0.0.9/vizmath/draw.py
+-rw-rw-rw-   0        0        0      624 2023-11-27 06:12:31.000000 vizmath-0.0.9/vizmath/examples.py
+-rw-rw-rw-   0        0        0    14628 2023-11-26 00:36:20.000000 vizmath-0.0.9/vizmath/functions.py
+-rw-rw-rw-   0        0        0    14861 2023-11-28 04:12:16.000000 vizmath-0.0.9/vizmath/radial_treemap.py
+drwxrwxrwx   0        0        0        0 2023-11-28 04:13:43.000000 vizmath-0.0.9/vizmath.egg-info/
+-rw-rw-rw-   0        0        0      491 2023-11-28 04:13:42.000000 vizmath-0.0.9/vizmath.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2023-11-28 04:13:43.000000 vizmath-0.0.9/vizmath.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-11-28 04:13:42.000000 vizmath-0.0.9/vizmath.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-11-28 04:13:42.000000 vizmath-0.0.9/vizmath.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-11-28 04:13:42.000000 vizmath-0.0.9/vizmath.egg-info/top_level.txt
```

### Comparing `vizmath-0.0.8/setup.py` & `vizmath-0.0.9/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools as st
 from setuptools import setup
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 setup(
     name="vizmath",
-    version="0.0.8",
+    version="0.0.9",
     description="Visualization math toolkit.",
     long_description="Welcome to vizmath! Please visit [GitHub](https://github.com/nickgerend/vizmath/blob/main/README.md)",
     long_description_content_type="text/markdown",
     url="https://github.com/nickgerend/vizmath",
     author="Nick Gerend",
     author_email="nickgerend@gmail.com",
     license="MIT",
```

### Comparing `vizmath-0.0.8/vizmath/binary_tree.py` & `vizmath-0.0.9/vizmath/binary_tree.py`

 * *Files identical despite different names*

### Comparing `vizmath-0.0.8/vizmath/draw.py` & `vizmath-0.0.9/vizmath/draw.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # vizmath
 # Author: Nick Gerend
 
 import pandas as pd
 import os
 import matplotlib.pyplot as plt
-import functions as vf
+from . import functions as vf
 
 class points:
 
     def __init__(self):
             self.viz=[]
             self.df = pd.DataFrame()
```

### Comparing `vizmath-0.0.8/vizmath/examples.py` & `vizmath-0.0.9/vizmath/examples.py`

 * *Files identical despite different names*

### Comparing `vizmath-0.0.8/vizmath/functions.py` & `vizmath-0.0.9/vizmath/functions.py`

 * *Files identical despite different names*

### Comparing `vizmath-0.0.8/vizmath/radial_treemap.py` & `vizmath-0.0.9/vizmath/radial_treemap.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import pandas as pd
 import numpy as np
 from math import pi, cos, sin, sqrt
 import random
 import matplotlib.pyplot as plt
 import copy
 
-import functions as vf
-from draw import points as dp
+from . import functions as vf
+from .draw import points as dp
 
 class rad_treemap:
 
     def __init__(self, df, groupers, value=None, r1=1, r2=2, a1=0, a2=360, points=200,
         default_sort=False, default_sort_override=True, default_sort_override_reversed=True,
         mode='smart', no_groups=False, rotate_deg=0, full=False):
```

