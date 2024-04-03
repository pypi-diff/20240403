# Comparing `tmp/dtrc-0.0.6.tar.gz` & `tmp/dtrc-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtrc-0.0.6.tar", last modified: Sun Mar 24 19:20:20 2024, max compression
+gzip compressed data, was "dtrc-0.0.7.tar", last modified: Wed Apr  3 11:43:36 2024, max compression
```

## Comparing `dtrc-0.0.6.tar` & `dtrc-0.0.7.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-03-24 19:20:20.938223 dtrc-0.0.6/
--rw-r--r--   0 solst      (501) staff       (20)    11337 2023-11-17 13:08:05.000000 dtrc-0.0.6/LICENSE
--rw-r--r--   0 solst      (501) staff       (20)      111 2023-11-17 13:08:05.000000 dtrc-0.0.6/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     3833 2024-03-24 19:20:20.938007 dtrc-0.0.6/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)     2720 2023-12-22 19:25:54.000000 dtrc-0.0.6/README.md
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-03-24 19:20:20.936616 dtrc-0.0.6/dtrc/
--rw-r--r--   0 solst      (501) staff       (20)      515 2024-03-24 19:19:33.000000 dtrc-0.0.6/dtrc/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)     2885 2024-03-24 19:19:33.000000 dtrc-0.0.6/dtrc/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)      376 2024-03-24 19:19:33.000000 dtrc-0.0.6/dtrc/atyp.py
--rw-r--r--   0 solst      (501) staff       (20)      375 2024-03-24 19:19:33.000000 dtrc-0.0.6/dtrc/cons.py
--rw-r--r--   0 solst      (501) staff       (20)      599 2024-03-24 19:19:33.000000 dtrc-0.0.6/dtrc/data.py
--rw-r--r--   0 solst      (501) staff       (20)      518 2024-03-24 19:19:33.000000 dtrc-0.0.6/dtrc/enum.py
--rw-r--r--   0 solst      (501) staff       (20)     5053 2024-03-24 19:19:33.000000 dtrc-0.0.6/dtrc/make.py
--rw-r--r--   0 solst      (501) staff       (20)     2256 2024-03-24 19:19:33.000000 dtrc-0.0.6/dtrc/poly.py
--rw-r--r--   0 solst      (501) staff       (20)     5745 2024-03-24 19:19:33.000000 dtrc-0.0.6/dtrc/util.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-03-24 19:20:20.937514 dtrc-0.0.6/dtrc.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     3833 2024-03-24 19:20:20.000000 dtrc-0.0.6/dtrc.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      372 2024-03-24 19:20:20.000000 dtrc-0.0.6/dtrc.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2024-03-24 19:20:20.000000 dtrc-0.0.6/dtrc.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)       30 2024-03-24 19:20:20.000000 dtrc-0.0.6/dtrc.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2024-03-24 17:50:00.000000 dtrc-0.0.6/dtrc.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)      137 2024-03-24 19:20:20.000000 dtrc-0.0.6/dtrc.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        5 2024-03-24 19:20:20.000000 dtrc-0.0.6/dtrc.egg-info/top_level.txt
--rw-r--r--   0 solst      (501) staff       (20)      912 2024-03-24 17:52:27.000000 dtrc-0.0.6/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2024-03-24 19:20:20.938268 dtrc-0.0.6/setup.cfg
--rw-r--r--   0 solst      (501) staff       (20)     2585 2023-11-17 13:08:05.000000 dtrc-0.0.6/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-03 11:43:36.551129 dtrc-0.0.7/
+-rw-r--r--   0 solst      (501) staff       (20)    11337 2023-11-17 13:08:05.000000 dtrc-0.0.7/LICENSE
+-rw-r--r--   0 solst      (501) staff       (20)      111 2023-11-17 13:08:05.000000 dtrc-0.0.7/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     3853 2024-04-03 11:43:36.550914 dtrc-0.0.7/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     2720 2023-12-22 19:25:54.000000 dtrc-0.0.7/README.md
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-03 11:43:36.549393 dtrc-0.0.7/dtrc/
+-rw-r--r--   0 solst      (501) staff       (20)      579 2024-04-03 11:43:20.000000 dtrc-0.0.7/dtrc/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)     2976 2024-04-03 11:43:20.000000 dtrc-0.0.7/dtrc/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)      626 2024-04-03 11:43:20.000000 dtrc-0.0.7/dtrc/atyp.py
+-rw-r--r--   0 solst      (501) staff       (20)     2893 2024-04-03 11:43:20.000000 dtrc-0.0.7/dtrc/cats.py
+-rw-r--r--   0 solst      (501) staff       (20)      375 2024-04-03 11:43:20.000000 dtrc-0.0.7/dtrc/cons.py
+-rw-r--r--   0 solst      (501) staff       (20)     4674 2024-04-03 11:43:20.000000 dtrc-0.0.7/dtrc/data.py
+-rw-r--r--   0 solst      (501) staff       (20)      498 2024-04-03 11:43:20.000000 dtrc-0.0.7/dtrc/enum.py
+-rw-r--r--   0 solst      (501) staff       (20)    16565 2024-04-03 11:43:20.000000 dtrc-0.0.7/dtrc/make.py
+-rw-r--r--   0 solst      (501) staff       (20)     4791 2024-04-03 11:43:20.000000 dtrc-0.0.7/dtrc/poly.py
+-rw-r--r--   0 solst      (501) staff       (20)     5350 2024-04-03 11:43:20.000000 dtrc-0.0.7/dtrc/trig.py
+-rw-r--r--   0 solst      (501) staff       (20)      498 2024-04-03 11:43:20.000000 dtrc-0.0.7/dtrc/util.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-03 11:43:36.550445 dtrc-0.0.7/dtrc.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     3853 2024-04-03 11:43:36.000000 dtrc-0.0.7/dtrc.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      398 2024-04-03 11:43:36.000000 dtrc-0.0.7/dtrc.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2024-04-03 11:43:36.000000 dtrc-0.0.7/dtrc.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)       30 2024-04-03 11:43:36.000000 dtrc-0.0.7/dtrc.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2024-03-24 17:50:00.000000 dtrc-0.0.7/dtrc.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)      142 2024-04-03 11:43:36.000000 dtrc-0.0.7/dtrc.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        5 2024-04-03 11:43:36.000000 dtrc-0.0.7/dtrc.egg-info/top_level.txt
+-rw-r--r--   0 solst      (501) staff       (20)      917 2024-04-03 11:43:17.000000 dtrc-0.0.7/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2024-04-03 11:43:36.551173 dtrc-0.0.7/setup.cfg
+-rw-r--r--   0 solst      (501) staff       (20)     2585 2023-11-17 13:08:05.000000 dtrc-0.0.7/setup.py
```

### Comparing `dtrc-0.0.6/LICENSE` & `dtrc-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dtrc-0.0.6/PKG-INFO` & `dtrc-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtrc
-Version: 0.0.6
+Version: 0.0.7
 Summary: data torch
 Home-page: https://github.com/dsm-72/dtrc
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: dtrc data pytorch torch trc
 Classifier: Development Status :: 4 - Beta
@@ -25,14 +25,15 @@
 Requires-Dist: quac
 Requires-Dist: uscr
 Requires-Dist: etrc
 Requires-Dist: slcs
 Requires-Dist: lmsg
 Requires-Dist: dtyp
 Requires-Dist: utrc
+Requires-Dist: zipr
 Provides-Extra: dev
 Requires-Dist: numpy; extra == "dev"
 Requires-Dist: pandas; extra == "dev"
 Requires-Dist: matplotlib; extra == "dev"
 Requires-Dist: torch; extra == "dev"
 Requires-Dist: pytorch_lightning; extra == "dev"
 Requires-Dist: torchvision; extra == "dev"
```

### Comparing `dtrc-0.0.6/README.md` & `dtrc-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `dtrc-0.0.6/dtrc/__init__.py` & `dtrc-0.0.7/dtrc/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-__version__ = "0.0.6"
+__version__ = "0.0.7"
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00__init__.ipynb.
 
 # %% auto 0
 __all__ = []
 
 # %% ../nbs/00__init__.ipynb 3
 from itertools import chain
-from . import (cons, atyp, enum, util, data, poly, make, )
+from . import (cons, atyp, enum, util, trig, cats, data, poly, make, )
 from .cons import *
 from .atyp import *
 from .enum import *
 from .util import *
+from .trig import *
+from .cats import *
 from .data import *
 from .poly import *
 from .make import *
 
 # %% ../nbs/00__init__.ipynb 4
 __all__ = sorted(set(chain(*[
-    mod.__all__ for mod in (cons, atyp, enum, util, data, poly, make, )
+    mod.__all__ for mod in (cons, atyp, enum, util, trig, cats, data, poly, make, )
 ])))
```

### Comparing `dtrc-0.0.6/dtrc/_modidx.py` & `dtrc-0.0.7/dtrc/_modidx.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,16 +2,22 @@
 
 d = { 'settings': { 'branch': 'main',
                 'doc_baseurl': '/dtrc',
                 'doc_host': 'https://dsm-72.github.io',
                 'git_url': 'https://github.com/dsm-72/dtrc',
                 'lib_path': 'dtrc'},
   'syms': { 'dtrc.atyp': {},
+            'dtrc.cats': { 'dtrc.cats.catdists': ('cats.html#catdists', 'dtrc/cats.py'),
+                           'dtrc.cats.catx': ('cats.html#catx', 'dtrc/cats.py'),
+                           'dtrc.cats.negcats': ('cats.html#negcats', 'dtrc/cats.py')},
             'dtrc.cons': {},
-            'dtrc.data': {},
+            'dtrc.data': { 'dtrc.data.addx': ('data.html#addx', 'dtrc/data.py'),
+                           'dtrc.data.addz': ('data.html#addz', 'dtrc/data.py'),
+                           'dtrc.data.dfxy': ('data.html#dfxy', 'dtrc/data.py'),
+                           'dtrc.data.npxy': ('data.html#npxy', 'dtrc/data.py')},
             'dtrc.enum': {},
             'dtrc.make': { 'dtrc.make.circles': ('make.html#circles', 'dtrc/make.py'),
                            'dtrc.make.diamonds': ('make.html#diamonds', 'dtrc/make.py'),
                            'dtrc.make.jacks': ('make.html#jacks', 'dtrc/make.py'),
                            'dtrc.make.make_circles': ('make.html#make_circles', 'dtrc/make.py'),
                            'dtrc.make.make_diamonds': ('make.html#make_diamonds', 'dtrc/make.py'),
                            'dtrc.make.make_orbits': ('make.html#make_orbits', 'dtrc/make.py'),
@@ -20,21 +26,16 @@
                            'dtrc.make.rings': ('make.html#rings', 'dtrc/make.py')},
             'dtrc.poly': { 'dtrc.poly.circle': ('poly.html#circle', 'dtrc/poly.py'),
                            'dtrc.poly.diamond': ('poly.html#diamond', 'dtrc/poly.py'),
                            'dtrc.poly.diamond_quadrant': ('poly.html#diamond_quadrant', 'dtrc/poly.py'),
                            'dtrc.poly.ellipse': ('poly.html#ellipse', 'dtrc/poly.py'),
                            'dtrc.poly.orbit': ('poly.html#orbit', 'dtrc/poly.py'),
                            'dtrc.poly.subring': ('poly.html#subring', 'dtrc/poly.py')},
-            'dtrc.util': { 'dtrc.util._': ('util.html#_', 'dtrc/util.py'),
-                           'dtrc.util.addx': ('util.html#addx', 'dtrc/util.py'),
-                           'dtrc.util.addz': ('util.html#addz', 'dtrc/util.py'),
-                           'dtrc.util.catrad': ('util.html#catrad', 'dtrc/util.py'),
-                           'dtrc.util.catx': ('util.html#catx', 'dtrc/util.py'),
-                           'dtrc.util.chord': ('util.html#chord', 'dtrc/util.py'),
-                           'dtrc.util.ctheta': ('util.html#ctheta', 'dtrc/util.py'),
-                           'dtrc.util.dfxy': ('util.html#dfxy', 'dtrc/util.py'),
-                           'dtrc.util.negcats': ('util.html#negcats', 'dtrc/util.py'),
-                           'dtrc.util.npxy': ('util.html#npxy', 'dtrc/util.py'),
-                           'dtrc.util.ntheta': ('util.html#ntheta', 'dtrc/util.py'),
-                           'dtrc.util.rad2pnt': ('util.html#rad2pnt', 'dtrc/util.py'),
-                           'dtrc.util.rotate': ('util.html#rotate', 'dtrc/util.py'),
-                           'dtrc.util.rotmat': ('util.html#rotmat', 'dtrc/util.py')}}}
+            'dtrc.trig': { 'dtrc.trig._': ('trig.html#_', 'dtrc/trig.py'),
+                           'dtrc.trig.catrad': ('trig.html#catrad', 'dtrc/trig.py'),
+                           'dtrc.trig.chord': ('trig.html#chord', 'dtrc/trig.py'),
+                           'dtrc.trig.ctheta': ('trig.html#ctheta', 'dtrc/trig.py'),
+                           'dtrc.trig.ntheta': ('trig.html#ntheta', 'dtrc/trig.py'),
+                           'dtrc.trig.rad2pnt': ('trig.html#rad2pnt', 'dtrc/trig.py'),
+                           'dtrc.trig.rotate': ('trig.html#rotate', 'dtrc/trig.py'),
+                           'dtrc.trig.rotmat': ('trig.html#rotmat', 'dtrc/trig.py')},
+            'dtrc.util': {}}}
```

### Comparing `dtrc-0.0.6/dtrc.egg-info/PKG-INFO` & `dtrc-0.0.7/dtrc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtrc
-Version: 0.0.6
+Version: 0.0.7
 Summary: data torch
 Home-page: https://github.com/dsm-72/dtrc
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: dtrc data pytorch torch trc
 Classifier: Development Status :: 4 - Beta
@@ -25,14 +25,15 @@
 Requires-Dist: quac
 Requires-Dist: uscr
 Requires-Dist: etrc
 Requires-Dist: slcs
 Requires-Dist: lmsg
 Requires-Dist: dtyp
 Requires-Dist: utrc
+Requires-Dist: zipr
 Provides-Extra: dev
 Requires-Dist: numpy; extra == "dev"
 Requires-Dist: pandas; extra == "dev"
 Requires-Dist: matplotlib; extra == "dev"
 Requires-Dist: torch; extra == "dev"
 Requires-Dist: pytorch_lightning; extra == "dev"
 Requires-Dist: torchvision; extra == "dev"
```

### Comparing `dtrc-0.0.6/settings.ini` & `dtrc-0.0.7/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = dtrc
 lib_name = dtrc
-version = 0.0.6
+version = 0.0.7
 min_python = 3.11
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = dtrc
 nbs_path = nbs
 recursive = True
@@ -29,10 +29,10 @@
 conda_user = dsm-72
 jupyter_hooks = True
 clean_ids = True
 clear_all = False
 readme_nb = index.ipynb
 allowed_metadata_keys = 
 allowed_cell_metadata_keys = 
-requirements = astr atup chck dref lull nchr nlit quac uscr etrc slcs lmsg dtyp utrc
+requirements = astr atup chck dref lull nchr nlit quac uscr etrc slcs lmsg dtyp utrc zipr
 dev_requirements = numpy pandas matplotlib torch pytorch_lightning torchvision
```

### Comparing `dtrc-0.0.6/setup.py` & `dtrc-0.0.7/setup.py`

 * *Files identical despite different names*

