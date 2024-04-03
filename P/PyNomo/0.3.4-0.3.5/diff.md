# Comparing `tmp/PyNomo-0.3.4.tar.gz` & `tmp/PyNomo-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyNomo-0.3.4.tar", last modified: Sun Mar 19 18:58:36 2023, max compression
+gzip compressed data, was "PyNomo-0.3.5.tar", last modified: Wed Apr  3 18:20:51 2024, max compression
```

## Comparing `PyNomo-0.3.4.tar` & `PyNomo-0.3.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 kayttaja   (501) staff       (20)        0 2023-03-19 18:58:36.546251 PyNomo-0.3.4/
--rw-r--r--   0 kayttaja   (501) staff       (20)       77 2023-03-19 17:59:10.000000 PyNomo-0.3.4/AUTHORS.txt
--rw-r--r--   0 kayttaja   (501) staff       (20)    35142 2023-03-19 17:59:10.000000 PyNomo-0.3.4/LICENSE
--rw-r--r--   0 kayttaja   (501) staff       (20)    32473 2023-03-19 17:59:10.000000 PyNomo-0.3.4/LICENSE.txt
--rw-r--r--   0 kayttaja   (501) staff       (20)     1214 2023-03-19 18:58:36.546319 PyNomo-0.3.4/PKG-INFO
-drwxr-xr-x   0 kayttaja   (501) staff       (20)        0 2023-03-19 18:58:36.544197 PyNomo-0.3.4/PyNomo.egg-info/
--rw-r--r--   0 kayttaja   (501) staff       (20)     1214 2023-03-19 18:58:36.000000 PyNomo-0.3.4/PyNomo.egg-info/PKG-INFO
--rw-r--r--   0 kayttaja   (501) staff       (20)      448 2023-03-19 18:58:36.000000 PyNomo-0.3.4/PyNomo.egg-info/SOURCES.txt
--rw-r--r--   0 kayttaja   (501) staff       (20)        1 2023-03-19 18:58:36.000000 PyNomo-0.3.4/PyNomo.egg-info/dependency_links.txt
--rw-r--r--   0 kayttaja   (501) staff       (20)        7 2023-03-19 18:58:36.000000 PyNomo-0.3.4/PyNomo.egg-info/top_level.txt
--rw-r--r--   0 kayttaja   (501) staff       (20)      478 2023-03-19 17:59:10.000000 PyNomo-0.3.4/README.rst
-drwxr-xr-x   0 kayttaja   (501) staff       (20)        0 2023-03-19 18:58:36.546099 PyNomo-0.3.4/pynomo/
--rw-r--r--   0 kayttaja   (501) staff       (20)     1102 2023-03-19 17:59:10.000000 PyNomo-0.3.4/pynomo/__init__.py
--rw-r--r--   0 kayttaja   (501) staff       (20)    24368 2023-03-19 17:59:10.000000 PyNomo-0.3.4/pynomo/circ_scale.py
--rw-r--r--   0 kayttaja   (501) staff       (20)    63491 2023-03-19 17:59:10.000000 PyNomo-0.3.4/pynomo/isopleth.py
--rw-r--r--   0 kayttaja   (501) staff       (20)    12133 2023-03-19 17:59:10.000000 PyNomo-0.3.4/pynomo/math_utilities.py
--rw-r--r--   0 kayttaja   (501) staff       (20)   139151 2023-03-19 17:59:10.000000 PyNomo-0.3.4/pynomo/nomo_axis.py
--rw-r--r--   0 kayttaja   (501) staff       (20)    30253 2023-03-19 17:59:10.000000 PyNomo-0.3.4/pynomo/nomo_axis_func.py
--rw-r--r--   0 kayttaja   (501) staff       (20)    15931 2023-03-19 17:59:10.000000 PyNomo-0.3.4/pynomo/nomo_grid.py
--rw-r--r--   0 kayttaja   (501) staff       (20)    28141 2023-03-19 17:59:10.000000 PyNomo-0.3.4/pynomo/nomo_grid_box.py
--rw-r--r--   0 kayttaja   (501) staff       (20)     2946 2023-03-19 17:59:10.000000 PyNomo-0.3.4/pynomo/nomo_low_level_ex.py
--rw-r--r--   0 kayttaja   (501) staff       (20)   178546 2023-03-19 17:59:10.000000 PyNomo-0.3.4/pynomo/nomo_wrapper.py
--rw-r--r--   0 kayttaja   (501) staff       (20)     9025 2023-03-19 17:59:10.000000 PyNomo-0.3.4/pynomo/nomograph3.py
--rwxr-xr-x   0 kayttaja   (501) staff       (20)    42923 2023-03-19 17:59:10.000000 PyNomo-0.3.4/pynomo/nomographer.py
--rw-r--r--   0 kayttaja   (501) staff       (20)       67 2023-03-19 18:58:36.546604 PyNomo-0.3.4/setup.cfg
--rw-r--r--   0 kayttaja   (501) staff       (20)     2308 2023-03-19 18:58:05.000000 PyNomo-0.3.4/setup.py
+drwxr-xr-x   0 kayttaja   (501) staff       (20)        0 2024-04-03 18:20:51.595032 PyNomo-0.3.5/
+-rw-r--r--   0 kayttaja   (501) staff       (20)       77 2024-04-03 17:31:38.000000 PyNomo-0.3.5/AUTHORS.txt
+-rw-r--r--   0 kayttaja   (501) staff       (20)    35142 2024-04-03 17:31:38.000000 PyNomo-0.3.5/LICENSE
+-rw-r--r--   0 kayttaja   (501) staff       (20)    32473 2024-04-03 17:31:38.000000 PyNomo-0.3.5/LICENSE.txt
+-rw-r--r--   0 kayttaja   (501) staff       (20)     1214 2024-04-03 18:20:51.594974 PyNomo-0.3.5/PKG-INFO
+drwxr-xr-x   0 kayttaja   (501) staff       (20)        0 2024-04-03 18:20:51.594775 PyNomo-0.3.5/PyNomo.egg-info/
+-rw-r--r--   0 kayttaja   (501) staff       (20)     1214 2024-04-03 18:20:51.000000 PyNomo-0.3.5/PyNomo.egg-info/PKG-INFO
+-rw-r--r--   0 kayttaja   (501) staff       (20)      448 2024-04-03 18:20:51.000000 PyNomo-0.3.5/PyNomo.egg-info/SOURCES.txt
+-rw-r--r--   0 kayttaja   (501) staff       (20)        1 2024-04-03 18:20:51.000000 PyNomo-0.3.5/PyNomo.egg-info/dependency_links.txt
+-rw-r--r--   0 kayttaja   (501) staff       (20)        7 2024-04-03 18:20:51.000000 PyNomo-0.3.5/PyNomo.egg-info/top_level.txt
+-rw-r--r--   0 kayttaja   (501) staff       (20)      478 2024-04-03 17:31:38.000000 PyNomo-0.3.5/README.rst
+drwxr-xr-x   0 kayttaja   (501) staff       (20)        0 2024-04-03 18:20:51.594230 PyNomo-0.3.5/pynomo/
+-rw-r--r--   0 kayttaja   (501) staff       (20)     1102 2024-04-03 17:31:38.000000 PyNomo-0.3.5/pynomo/__init__.py
+-rw-r--r--   0 kayttaja   (501) staff       (20)    24368 2024-04-03 17:31:38.000000 PyNomo-0.3.5/pynomo/circ_scale.py
+-rw-r--r--   0 kayttaja   (501) staff       (20)    63491 2024-04-03 17:31:38.000000 PyNomo-0.3.5/pynomo/isopleth.py
+-rw-r--r--   0 kayttaja   (501) staff       (20)    12133 2024-04-03 17:31:38.000000 PyNomo-0.3.5/pynomo/math_utilities.py
+-rw-r--r--   0 kayttaja   (501) staff       (20)   139151 2024-04-03 17:31:38.000000 PyNomo-0.3.5/pynomo/nomo_axis.py
+-rw-r--r--   0 kayttaja   (501) staff       (20)    30253 2024-04-03 17:31:38.000000 PyNomo-0.3.5/pynomo/nomo_axis_func.py
+-rw-r--r--   0 kayttaja   (501) staff       (20)    15931 2024-04-03 17:31:38.000000 PyNomo-0.3.5/pynomo/nomo_grid.py
+-rw-r--r--   0 kayttaja   (501) staff       (20)    28141 2024-04-03 17:31:38.000000 PyNomo-0.3.5/pynomo/nomo_grid_box.py
+-rw-r--r--   0 kayttaja   (501) staff       (20)     2946 2024-04-03 17:31:38.000000 PyNomo-0.3.5/pynomo/nomo_low_level_ex.py
+-rw-r--r--   0 kayttaja   (501) staff       (20)   178546 2024-04-03 17:31:38.000000 PyNomo-0.3.5/pynomo/nomo_wrapper.py
+-rw-r--r--   0 kayttaja   (501) staff       (20)     9025 2024-04-03 17:31:38.000000 PyNomo-0.3.5/pynomo/nomograph3.py
+-rwxr-xr-x   0 kayttaja   (501) staff       (20)    42923 2024-04-03 17:31:38.000000 PyNomo-0.3.5/pynomo/nomographer.py
+-rw-r--r--   0 kayttaja   (501) staff       (20)       67 2024-04-03 18:20:51.595305 PyNomo-0.3.5/setup.cfg
+-rw-r--r--   0 kayttaja   (501) staff       (20)     2308 2024-04-03 18:20:09.000000 PyNomo-0.3.5/setup.py
```

### Comparing `PyNomo-0.3.4/LICENSE` & `PyNomo-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `PyNomo-0.3.4/LICENSE.txt` & `PyNomo-0.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyNomo-0.3.4/PKG-INFO` & `PyNomo-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyNomo
-Version: 0.3.4
+Version: 0.3.5
 Summary: PyNomo - Python Nomograms
 Home-page: http://pynomo.org/
 Download-URL: https://github.com/lefakkomies/pynomo
 Author: Leif Roschier
 Author-email: leif.roschier@iki.fi
 License: GPL
 Keywords: nomograph nomogram graphics calculator visualization
```

### Comparing `PyNomo-0.3.4/PyNomo.egg-info/PKG-INFO` & `PyNomo-0.3.5/PyNomo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyNomo
-Version: 0.3.4
+Version: 0.3.5
 Summary: PyNomo - Python Nomograms
 Home-page: http://pynomo.org/
 Download-URL: https://github.com/lefakkomies/pynomo
 Author: Leif Roschier
 Author-email: leif.roschier@iki.fi
 License: GPL
 Keywords: nomograph nomogram graphics calculator visualization
```

### Comparing `PyNomo-0.3.4/pynomo/__init__.py` & `PyNomo-0.3.5/pynomo/__init__.py`

 * *Files identical despite different names*

### Comparing `PyNomo-0.3.4/pynomo/circ_scale.py` & `PyNomo-0.3.5/pynomo/circ_scale.py`

 * *Files identical despite different names*

### Comparing `PyNomo-0.3.4/pynomo/isopleth.py` & `PyNomo-0.3.5/pynomo/isopleth.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 #
 #    You should have received a copy of the GNU General Public License
 #    along with this program.  If not, see <http://www.gnu.org/licenses/>.
 import math
 import pyx
 import copy, re
 from scipy.optimize import *
-from scipy import arange
+from numpy import arange
 import warnings
 
 
 class Isopleth_Wrapper(object):
     """
     class to hold all isopleths and control everything related to them
     """
```

### Comparing `PyNomo-0.3.4/pynomo/math_utilities.py` & `PyNomo-0.3.5/pynomo/math_utilities.py`

 * *Files identical despite different names*

### Comparing `PyNomo-0.3.4/pynomo/nomo_axis.py` & `PyNomo-0.3.5/pynomo/nomo_axis.py`

 * *Files identical despite different names*

### Comparing `PyNomo-0.3.4/pynomo/nomo_axis_func.py` & `PyNomo-0.3.5/pynomo/nomo_axis_func.py`

 * *Files identical despite different names*

### Comparing `PyNomo-0.3.4/pynomo/nomo_grid.py` & `PyNomo-0.3.5/pynomo/nomo_grid.py`

 * *Files identical despite different names*

### Comparing `PyNomo-0.3.4/pynomo/nomo_grid_box.py` & `PyNomo-0.3.5/pynomo/nomo_grid_box.py`

 * *Files identical despite different names*

### Comparing `PyNomo-0.3.4/pynomo/nomo_low_level_ex.py` & `PyNomo-0.3.5/pynomo/nomo_low_level_ex.py`

 * *Files identical despite different names*

### Comparing `PyNomo-0.3.4/pynomo/nomo_wrapper.py` & `PyNomo-0.3.5/pynomo/nomo_wrapper.py`

 * *Files identical despite different names*

### Comparing `PyNomo-0.3.4/pynomo/nomograph3.py` & `PyNomo-0.3.5/pynomo/nomograph3.py`

 * *Files identical despite different names*

### Comparing `PyNomo-0.3.4/pynomo/nomographer.py` & `PyNomo-0.3.5/pynomo/nomographer.py`

 * *Files identical despite different names*

### Comparing `PyNomo-0.3.4/setup.py` & `PyNomo-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- encoding: utf-8 -*-
 #
 #    PyNomo - nomographs with Python
-#    Copyright (C) 2007- 2020  Leif Roschier
+#    Copyright (C) 2007- 2023  Leif Roschier
 #
 #    This program is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
 #    (at your option) any later version.
 #
 #    This program is distributed in the hope that it will be useful,
@@ -29,15 +29,15 @@
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='PyNomo',
-      version='0.3.4',
+      version='0.3.5',
       description='PyNomo - Python Nomograms',
       long_description=long_description,
       author='Leif Roschier',
       author_email='leif.roschier@iki.fi',
       url='http://pynomo.org/',
       download_url='https://github.com/lefakkomies/pynomo',
       packages=['pynomo'],
```

