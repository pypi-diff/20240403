# Comparing `tmp/pyfds-0.2.0.tar.gz` & `tmp/pyfds-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfds-0.2.0.tar", last modified: Fri Jun 30 08:52:36 2023, max compression
+gzip compressed data, was "pyfds-0.3.0.tar", last modified: Wed Apr  3 14:54:51 2024, max compression
```

## Comparing `pyfds-0.2.0.tar` & `pyfds-0.3.0.tar`

### file list

```diff
@@ -1,48 +1,52 @@
-drwxrwx---   0 leanderc (50967) user     (10000)        0 2023-06-30 08:52:36.700352 pyfds-0.2.0/
-drwxrwx---   0 leanderc (50967) user     (10000)        0 2023-06-30 08:52:36.370438 pyfds-0.2.0/.github/
-drwxrwx---   0 leanderc (50967) user     (10000)        0 2023-06-30 08:52:36.440495 pyfds-0.2.0/.github/workflows/
--rwxrwx---   0 leanderc (50967) user     (10000)     1321 2023-06-30 08:00:31.000000 pyfds-0.2.0/.github/workflows/python-package.yml
--rwxrwx---   0 leanderc (50967) user     (10000)     2194 2017-01-02 12:00:53.000000 pyfds-0.2.0/.gitignore
--rwxrwx---   0 leanderc (50967) user     (10000)      118 2021-10-20 12:26:35.000000 pyfds-0.2.0/AUTHORS.rst
--rwxrwx---   0 leanderc (50967) user     (10000)     2476 2023-06-30 08:29:53.000000 pyfds-0.2.0/CHANGELOG.rst
--rwxrwx---   0 leanderc (50967) user     (10000)     1477 2017-05-16 12:52:30.000000 pyfds-0.2.0/LICENSE
--rwxrwx---   0 leanderc (50967) user     (10000)     3108 2023-06-30 08:52:36.697927 pyfds-0.2.0/PKG-INFO
--rwxrwx---   0 leanderc (50967) user     (10000)      641 2023-03-30 12:28:36.000000 pyfds-0.2.0/README.rst
-drwxrwx---   0 leanderc (50967) user     (10000)        0 2023-06-30 08:52:36.548937 pyfds-0.2.0/doc/
--rwxrwx---   0 leanderc (50967) user     (10000)       79 2023-03-30 12:24:43.000000 pyfds-0.2.0/doc/acoustic_flow.rst
--rwxrwx---   0 leanderc (50967) user     (10000)       67 2017-02-02 09:31:23.000000 pyfds-0.2.0/doc/acoustics.rst
--rwxrwx---   0 leanderc (50967) user     (10000)     2551 2023-06-30 07:07:46.000000 pyfds-0.2.0/doc/conf.py
--rwxrwx---   0 leanderc (50967) user     (10000)       82 2021-12-20 08:34:47.000000 pyfds-0.2.0/doc/electrostatics.rst
--rwxrwx---   0 leanderc (50967) user     (10000)     3790 2017-06-13 12:30:59.000000 pyfds-0.2.0/doc/ex_acoustics.rst
--rwxrwx---   0 leanderc (50967) user     (10000)     3339 2017-06-12 15:06:37.000000 pyfds-0.2.0/doc/ex_visualization.rst
--rwxrwx---   0 leanderc (50967) user     (10000)       78 2017-06-08 09:07:55.000000 pyfds-0.2.0/doc/examples.rst
--rwxrwx---   0 leanderc (50967) user     (10000)       58 2017-01-02 09:14:37.000000 pyfds-0.2.0/doc/fields.rst
--rwxrwx---   0 leanderc (50967) user     (10000)       49 2017-02-02 09:31:55.000000 pyfds-0.2.0/doc/gfx.rst
--rwxrwx---   0 leanderc (50967) user     (10000)      440 2023-06-29 15:37:34.000000 pyfds-0.2.0/doc/index.rst
--rwxrwx---   0 leanderc (50967) user     (10000)       97 2017-06-06 12:12:26.000000 pyfds-0.2.0/doc/nonlinear_acoustics.rst
--rwxrwx---   0 leanderc (50967) user     (10000)       61 2017-02-02 09:30:58.000000 pyfds-0.2.0/doc/regions.rst
--rwxrwx---   0 leanderc (50967) user     (10000)       61 2021-12-20 08:34:52.000000 pyfds-0.2.0/doc/thermal.rst
--rwxrwx---   0 leanderc (50967) user     (10000)     8935 2021-10-20 12:13:52.000000 pyfds-0.2.0/doc/usage.rst
-drwxrwx---   0 leanderc (50967) user     (10000)        0 2023-06-30 08:52:36.623709 pyfds-0.2.0/pyfds/
--rwxrwx---   0 leanderc (50967) user     (10000)      469 2023-06-07 14:22:40.000000 pyfds-0.2.0/pyfds/__init__.py
--rwxrwx---   0 leanderc (50967) user     (10000)     2140 2023-06-07 14:42:38.000000 pyfds-0.2.0/pyfds/acoustic_flow.py
--rwxrwx---   0 leanderc (50967) user     (10000)    12683 2023-06-07 14:42:36.000000 pyfds-0.2.0/pyfds/acoustics.py
--rwxrwx---   0 leanderc (50967) user     (10000)     4793 2023-06-07 14:52:41.000000 pyfds-0.2.0/pyfds/electrostatics.py
--rwxrwx---   0 leanderc (50967) user     (10000)    24599 2023-06-29 15:28:24.000000 pyfds-0.2.0/pyfds/fields.py
--rwxrwx---   0 leanderc (50967) user     (10000)    17365 2023-06-30 07:22:59.000000 pyfds-0.2.0/pyfds/gfx.py
--rwxrwx---   0 leanderc (50967) user     (10000)     8125 2023-06-30 06:47:34.000000 pyfds-0.2.0/pyfds/nonlinear_acoustics.py
--rwxrwx---   0 leanderc (50967) user     (10000)     5127 2023-06-07 14:45:45.000000 pyfds-0.2.0/pyfds/regions.py
--rwxrwx---   0 leanderc (50967) user     (10000)     8213 2023-06-07 14:45:55.000000 pyfds-0.2.0/pyfds/thermal.py
-drwxrwx---   0 leanderc (50967) user     (10000)        0 2023-06-30 08:52:36.664885 pyfds-0.2.0/pyfds.egg-info/
--rwxrwx---   0 leanderc (50967) user     (10000)     3108 2023-06-30 08:52:36.000000 pyfds-0.2.0/pyfds.egg-info/PKG-INFO
--rwxrwx---   0 leanderc (50967) user     (10000)      753 2023-06-30 08:52:36.000000 pyfds-0.2.0/pyfds.egg-info/SOURCES.txt
--rwxrwx---   0 leanderc (50967) user     (10000)        1 2023-06-30 08:52:36.000000 pyfds-0.2.0/pyfds.egg-info/dependency_links.txt
--rwxrwx---   0 leanderc (50967) user     (10000)       84 2023-06-30 08:52:36.000000 pyfds-0.2.0/pyfds.egg-info/requires.txt
--rwxrwx---   0 leanderc (50967) user     (10000)        6 2023-06-30 08:52:36.000000 pyfds-0.2.0/pyfds.egg-info/top_level.txt
--rwxrwx---   0 leanderc (50967) user     (10000)     1032 2023-06-29 15:49:48.000000 pyfds-0.2.0/pyproject.toml
--rwxrwx---   0 leanderc (50967) user     (10000)       38 2023-06-30 08:52:36.701856 pyfds-0.2.0/setup.cfg
--rwxrwx---   0 leanderc (50967) user     (10000)     1261 2023-06-29 15:48:20.000000 pyfds-0.2.0/setup.py
-drwxrwx---   0 leanderc (50967) user     (10000)        0 2023-06-30 08:52:36.689468 pyfds-0.2.0/test/
--rwxrwx---   0 leanderc (50967) user     (10000)     3700 2023-06-30 07:12:49.000000 pyfds-0.2.0/test/test_acoustics.py
--rwxrwx---   0 leanderc (50967) user     (10000)     6098 2023-06-30 08:21:57.000000 pyfds-0.2.0/test/test_fields.py
--rwxrwx---   0 leanderc (50967) user     (10000)      286 2017-02-02 09:14:25.000000 pyfds-0.2.0/test/test_regions.py
+drwxrwx---   0 leanderc (50967) user     (10000)        0 2024-04-03 14:54:51.749745 pyfds-0.3.0/
+drwxrwx---   0 leanderc (50967) user     (10000)        0 2024-04-03 14:54:51.354226 pyfds-0.3.0/.github/
+drwxrwx---   0 leanderc (50967) user     (10000)        0 2024-04-03 14:54:51.443249 pyfds-0.3.0/.github/workflows/
+-rwxrwx---   0 leanderc (50967) user     (10000)     1321 2023-06-30 08:00:31.000000 pyfds-0.3.0/.github/workflows/python-package.yml
+-rwxrwx---   0 leanderc (50967) user     (10000)     2194 2017-01-02 12:00:53.000000 pyfds-0.3.0/.gitignore
+-rwxrwx---   0 leanderc (50967) user     (10000)      118 2021-10-20 12:26:35.000000 pyfds-0.3.0/AUTHORS.rst
+-rwxrwx---   0 leanderc (50967) user     (10000)     2810 2024-04-03 14:41:44.000000 pyfds-0.3.0/CHANGELOG.rst
+-rwxrwx---   0 leanderc (50967) user     (10000)     1477 2017-05-16 12:52:30.000000 pyfds-0.3.0/LICENSE
+-rwxrwxr--   0 leanderc (50967) user     (10000)     3426 2024-04-03 14:54:51.743363 pyfds-0.3.0/PKG-INFO
+-rwxrwx---   0 leanderc (50967) user     (10000)      722 2024-04-03 14:45:15.000000 pyfds-0.3.0/README.rst
+drwxrwx---   0 leanderc (50967) user     (10000)        0 2024-04-03 14:54:51.559044 pyfds-0.3.0/doc/
+-rwxrwx---   0 leanderc (50967) user     (10000)       79 2023-03-30 12:24:43.000000 pyfds-0.3.0/doc/acoustic_flow.rst
+-rwxrwx---   0 leanderc (50967) user     (10000)       67 2017-02-02 09:31:23.000000 pyfds-0.3.0/doc/acoustics.rst
+-rwxrwx---   0 leanderc (50967) user     (10000)     2551 2023-06-30 07:07:46.000000 pyfds-0.3.0/doc/conf.py
+-rwxrwx---   0 leanderc (50967) user     (10000)      172 2024-01-17 13:05:40.000000 pyfds-0.3.0/doc/coupling.rst
+-rwxrwx---   0 leanderc (50967) user     (10000)       82 2021-12-20 08:34:47.000000 pyfds-0.3.0/doc/electrostatics.rst
+-rwxrwx---   0 leanderc (50967) user     (10000)     3790 2017-06-13 12:30:59.000000 pyfds-0.3.0/doc/ex_acoustics.rst
+-rwxrwx---   0 leanderc (50967) user     (10000)     3339 2017-06-12 15:06:37.000000 pyfds-0.3.0/doc/ex_visualization.rst
+-rwxrwx---   0 leanderc (50967) user     (10000)       78 2017-06-08 09:07:55.000000 pyfds-0.3.0/doc/examples.rst
+-rwxrwx---   0 leanderc (50967) user     (10000)       58 2017-01-02 09:14:37.000000 pyfds-0.3.0/doc/fields.rst
+-rwxrwx---   0 leanderc (50967) user     (10000)       49 2017-02-02 09:31:55.000000 pyfds-0.3.0/doc/gfx.rst
+-rwxrwx---   0 leanderc (50967) user     (10000)      454 2024-01-17 13:06:27.000000 pyfds-0.3.0/doc/index.rst
+-rwxrwx---   0 leanderc (50967) user     (10000)       97 2017-06-06 12:12:26.000000 pyfds-0.3.0/doc/nonlinear_acoustics.rst
+-rwxrwx---   0 leanderc (50967) user     (10000)       61 2017-02-02 09:30:58.000000 pyfds-0.3.0/doc/regions.rst
+-rwxrwx---   0 leanderc (50967) user     (10000)       61 2021-12-20 08:34:52.000000 pyfds-0.3.0/doc/thermal.rst
+-rwxrwx---   0 leanderc (50967) user     (10000)     8935 2021-10-20 12:13:52.000000 pyfds-0.3.0/doc/usage.rst
+drwxrwx---   0 leanderc (50967) user     (10000)        0 2024-04-03 14:54:51.649724 pyfds-0.3.0/pyfds/
+-rwxrwx---   0 leanderc (50967) user     (10000)      247 2024-01-17 09:00:31.000000 pyfds-0.3.0/pyfds/__init__.py
+-rwxrwx---   0 leanderc (50967) user     (10000)     2179 2024-01-17 13:15:07.000000 pyfds-0.3.0/pyfds/acoustic_flow.py
+-rwxrwx---   0 leanderc (50967) user     (10000)    12771 2024-01-10 14:09:57.000000 pyfds-0.3.0/pyfds/acoustics.py
+-rwxrwx---   0 leanderc (50967) user     (10000)     2603 2024-01-17 13:16:14.000000 pyfds-0.3.0/pyfds/coupled_fields.py
+-rwxrwx---   0 leanderc (50967) user     (10000)    10341 2024-01-17 14:10:14.000000 pyfds-0.3.0/pyfds/coupling.py
+-rwxrwx---   0 leanderc (50967) user     (10000)     4636 2024-01-10 14:13:02.000000 pyfds-0.3.0/pyfds/electrostatics.py
+-rwxrwx---   0 leanderc (50967) user     (10000)    24352 2024-01-09 15:07:20.000000 pyfds-0.3.0/pyfds/fields.py
+-rwxrwx---   0 leanderc (50967) user     (10000)    17416 2024-01-10 14:13:44.000000 pyfds-0.3.0/pyfds/gfx.py
+-rwxrwx---   0 leanderc (50967) user     (10000)     8211 2024-01-10 14:10:37.000000 pyfds-0.3.0/pyfds/nonlinear_acoustics.py
+-rwxrwx---   0 leanderc (50967) user     (10000)     5190 2024-01-18 07:57:16.000000 pyfds-0.3.0/pyfds/regions.py
+-rwxrwx---   0 leanderc (50967) user     (10000)     8296 2024-01-10 14:12:11.000000 pyfds-0.3.0/pyfds/thermal.py
+drwxrwx---   0 leanderc (50967) user     (10000)        0 2024-04-03 14:54:51.733615 pyfds-0.3.0/pyfds.egg-info/
+-rwxrwxr--   0 leanderc (50967) user     (10000)     3426 2024-04-03 14:54:51.000000 pyfds-0.3.0/pyfds.egg-info/PKG-INFO
+-rwxrwx---   0 leanderc (50967) user     (10000)      834 2024-04-03 14:54:51.000000 pyfds-0.3.0/pyfds.egg-info/SOURCES.txt
+-rwxrwx---   0 leanderc (50967) user     (10000)        1 2024-04-03 14:54:51.000000 pyfds-0.3.0/pyfds.egg-info/dependency_links.txt
+-rwxrwx---   0 leanderc (50967) user     (10000)       84 2024-04-03 14:54:51.000000 pyfds-0.3.0/pyfds.egg-info/requires.txt
+-rwxrwx---   0 leanderc (50967) user     (10000)        6 2024-04-03 14:54:51.000000 pyfds-0.3.0/pyfds.egg-info/top_level.txt
+-rwxrwx---   0 leanderc (50967) user     (10000)     1032 2023-06-29 15:49:48.000000 pyfds-0.3.0/pyproject.toml
+-rwxrwx---   0 leanderc (50967) user     (10000)       38 2024-04-03 14:54:51.751370 pyfds-0.3.0/setup.cfg
+-rwxrwx---   0 leanderc (50967) user     (10000)     1261 2023-06-29 15:48:20.000000 pyfds-0.3.0/setup.py
+drwxrwx---   0 leanderc (50967) user     (10000)        0 2024-04-03 14:54:51.724663 pyfds-0.3.0/test/
+-rwxrwx---   0 leanderc (50967) user     (10000)     3700 2023-06-30 07:12:49.000000 pyfds-0.3.0/test/test_acoustics.py
+-rwxrwx---   0 leanderc (50967) user     (10000)     3788 2024-01-10 13:49:00.000000 pyfds-0.3.0/test/test_coupling.py
+-rwxrwx---   0 leanderc (50967) user     (10000)     6098 2023-06-30 08:21:57.000000 pyfds-0.3.0/test/test_fields.py
+-rwxrwx---   0 leanderc (50967) user     (10000)      286 2017-02-02 09:14:25.000000 pyfds-0.3.0/test/test_regions.py
```

### Comparing `pyfds-0.2.0/.github/workflows/python-package.yml` & `pyfds-0.3.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `pyfds-0.2.0/.gitignore` & `pyfds-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyfds-0.2.0/CHANGELOG.rst` & `pyfds-0.3.0/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,27 @@
 .. _Semantic versioning: https://semver.org/
 
 
 `Unreleased`_
 =============
 
 
+`0.3.0`_ - 2024-04-03
+=====================
+
+Added
+-----
+* Generic API for simulation of coupled fields using boundary conditions and dependent material parameters.
+* One-dimensional thermo-acoustic simulation.
+
+Changed
+-------
+* Internal import structure.
+
+
 `0.2.0`_ - 2023-06-30
 =====================
 
 Added
 -----
 * Support for elliptic regions.
 
@@ -115,14 +128,15 @@
 
 Added
 -----
 * First preview release.
 
 
 .. _Unreleased: https://github.com/emtpb/pyfds
+.. _0.3.0: https://github.com/emtpb/pyfds/releases/tag/0.3.0
 .. _0.2.0: https://github.com/emtpb/pyfds/releases/tag/0.2.0
 .. _0.1.6: https://github.com/emtpb/pyfds/releases/tag/0.1.6
 .. _0.1.5: https://github.com/emtpb/pyfds/releases/tag/0.1.5
 .. _0.1.4: https://github.com/emtpb/pyfds/releases/tag/0.1.4
 .. _0.1.3: https://github.com/emtpb/pyfds/releases/tag/0.1.3
 .. _0.1.2: https://github.com/emtpb/pyfds/releases/tag/0.1.2
 .. _0.1.1: https://github.com/emtpb/pyfds/releases/tag/0.1.1
```

### Comparing `pyfds-0.2.0/LICENSE` & `pyfds-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfds-0.2.0/PKG-INFO` & `pyfds-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfds
-Version: 0.2.0
+Version: 0.3.0
 Summary: Modular field simulation tool using finite differences.
 Home-page: https://emt.uni-paderborn.de
 Author: Leander Claes
 Author-email: Leander Claes <claes@emt.uni-paderborn.de>
 License: Copyright (c) 2017 Leander Claes
         
         Redistribution and use in source and binary forms, with or without
@@ -38,18 +38,25 @@
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
-Provides-Extra: doc
-Provides-Extra: test
 License-File: LICENSE
 License-File: AUTHORS.rst
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: scipy
+Provides-Extra: doc
+Requires-Dist: setuptools_scm; extra == "doc"
+Requires-Dist: sphinx; extra == "doc"
+Requires-Dist: sphinx-rtd-theme; extra == "doc"
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
 
 =====
 pyfds
 =====
 .. image:: https://zenodo.org/badge/92026828.svg
    :target: https://zenodo.org/badge/latestdoi/92026828
 
@@ -59,7 +66,9 @@
 --------
  
 * One-dimensional, two-dimensional, and axial-symmetric linear acoustic field simulation.
 * One-dimensional nonlinear acoustic field simulation in ideal gases and arbitrary fluids using second order approximation.
 * Two-dimensional acoustic simulation with moving medium.
 * One-dimensional, two-dimensional, and axial-symmetric thermal field simulation.
 * One-dimensional and two-dimensional electrostatic field simulation.
+* Options to couple simulations.
+* One-dimensional thermo-acoustic simulation.
```

### Comparing `pyfds-0.2.0/README.rst` & `pyfds-0.3.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -10,7 +10,9 @@
 --------
  
 * One-dimensional, two-dimensional, and axial-symmetric linear acoustic field simulation.
 * One-dimensional nonlinear acoustic field simulation in ideal gases and arbitrary fluids using second order approximation.
 * Two-dimensional acoustic simulation with moving medium.
 * One-dimensional, two-dimensional, and axial-symmetric thermal field simulation.
 * One-dimensional and two-dimensional electrostatic field simulation.
+* Options to couple simulations.
+* One-dimensional thermo-acoustic simulation.
```

### Comparing `pyfds-0.2.0/doc/conf.py` & `pyfds-0.3.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `pyfds-0.2.0/doc/ex_acoustics.rst` & `pyfds-0.3.0/doc/ex_acoustics.rst`

 * *Files identical despite different names*

### Comparing `pyfds-0.2.0/doc/ex_visualization.rst` & `pyfds-0.3.0/doc/ex_visualization.rst`

 * *Files identical despite different names*

### Comparing `pyfds-0.2.0/doc/usage.rst` & `pyfds-0.3.0/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `pyfds-0.2.0/pyfds/acoustic_flow.py` & `pyfds-0.3.0/pyfds/acoustic_flow.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import logging as lo
 import numpy as np
 import warnings as wn
 from . import acoustics as acs
 
+__all__ = [
+    'AcousticFlow2D',
+]
+
 logger = lo.getLogger('pyfds')
 
 
 class AcousticFlow2D(acs.Acoustic2D):
     """Class for simulation of two-dimensional acoustic fields with moving medium.
 
     The implementation is an approximation realised by moving the values in the field components
@@ -14,15 +18,15 @@
     """
 
     def __init__(self, flow, *args, **kwargs):
         """Class constructor.
 
         Args:
             flow: Flow velocity in x direction (scalar or vector with length of y_samples).
-            *args, **kwargs: See pyfds.fields.Field2D constructor arguments.
+            *args, \\**kwargs: See pyfds.fields.Field2D constructor arguments.
         """
         super().__init__(*args, **kwargs)
 
         if isinstance(flow, (list, np.ndarray)) and \
                 len(flow) == self.y.samples:
             self.flow = np.asarray(flow)
         elif isinstance(flow, (float, int)):
```

### Comparing `pyfds-0.2.0/pyfds/acoustics.py` & `pyfds-0.3.0/pyfds/acoustics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 import numpy as np
 from . import fields as fld
 
+__all__ = [
+    'Acoustic1D', 'Acoustic2D', 'Acoustic3DAxi', 'AcousticMaterial',
+]
+
 
 class Acoustic1D(fld.Field1D):
     """Class for simulation of one-dimensional acoustic fields."""
 
     def __init__(self, *args, **kwargs):
         """Class constructor.
```

### Comparing `pyfds-0.2.0/pyfds/electrostatics.py` & `pyfds-0.3.0/pyfds/electrostatics.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import logging as lo
 import numpy as np
 import scipy.sparse as sp
 import scipy.sparse.linalg as sl
-import warnings as wn
 from . import fields as fld
 
+__all__ = [
+    'Electrostatic1D', 'Electrostatic2D', 'ElectrostaticMaterial',
+]
+
 logger = lo.getLogger('pyfds')
 
 
 class Electrostatic1D(fld.Field1D):
     """Class for simulation of one-dimensional electrostatic fields."""
 
     def __init__(self, x_samples, x_delta, material):
@@ -42,18 +45,16 @@
 
         self.charge_density.apply_bounds(self.step)
         self.charge_density.write_outputs()
 
         self.potential.values = -self.a_phi_rho.dot(self.charge_density.values)
 
         if len(self.potential.boundaries) != 0:
-            wn.warn('Boundary conditions for electric potential are currently not supported.',
-                    stacklevel=2)
-            logger.warning(
-                'Boundary conditions for electric potential are currently not supported.')
+            raise RuntimeError('Boundary conditions for electric potential are currently not '
+                               'supported.')
 
 
 class Electrostatic2D(fld.Field2D):
     """Class for simulation of two-dimensional electrostatic fields."""
 
     def __init__(self, x_samples, x_delta, y_samples, y_delta, material):
         """Class constructor.
@@ -90,18 +91,16 @@
 
         self.charge_density.apply_bounds(self.step)
         self.charge_density.write_outputs()
 
         self.potential.values = -self.a_phi_rho.dot(self.charge_density.values)
 
         if len(self.potential.boundaries) != 0:
-            wn.warn('Boundary conditions for electric potential are currently not supported.',
-                    stacklevel=2)
-            logger.warning(
-                'Boundary conditions for electric potential are currently not supported.')
+            raise RuntimeError('Boundary conditions for electric potential are currently not '
+                               'supported.')
 
 
 class ElectrostaticMaterial:
     """Class for specification of electrostatic material parameters."""
 
     def __init__(self, permittivity=8.8541878128e-12):
         """Class constructor. Default values create vacuum.
```

### Comparing `pyfds-0.2.0/pyfds/fields.py` & `pyfds-0.3.0/pyfds/fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import logging as lo
 import numpy as np
 import scipy.sparse as sp
-import warnings as wn
 from . import regions as reg
 
 logger = lo.getLogger('pyfds')
 
 
 class Field:
     """Base class for all fields."""
@@ -49,19 +48,15 @@
         for mat_reg in self.material_regions:
             for mat in mat_reg.materials:
                 if hasattr(mat, mat_parameter):
                     mat_vector[mat_reg.region.indices] = getattr(mat, mat_parameter)
                     param_found = True
 
         if not param_found:
-            wn.warn('Material parameter {} not found in set materials. Returning zeros.'
-                    .format(mat_parameter), stacklevel=2)
-            logger.warning(
-                'Material parameter {} not found in set materials. Returning zeros.'
-                .format(mat_parameter))
+            raise KeyError('Material parameter {} not found in set materials.')
 
         return mat_vector
 
     def assemble_matrices(self):
         """Assemble the matrices and vectors required for simulation."""
         raise NotImplementedError
```

### Comparing `pyfds-0.2.0/pyfds/gfx.py` & `pyfds-0.3.0/pyfds/gfx.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 import matplotlib.pyplot as pp
 import multiprocessing as mp
 import numpy as np
 import os
 from . import fields as fld
 from . import regions as reg
 
+__all__ = [
+    'Animator1D', 'Animator2D',
+]
+
 
 class Animator:
     """Base class for pyfds' live field animation during simulation."""
 
     def __init__(self, field, observed_component=None, steps_per_frame=10, scale=1,
                  frame_delay=1e-2, save_video=False, video_file_name='pyfds_vid.mp4'):
         """Class constructor.
```

### Comparing `pyfds-0.2.0/pyfds/nonlinear_acoustics.py` & `pyfds-0.3.0/pyfds/nonlinear_acoustics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import numpy as np
-import warnings as wn
 from . import fields as fld
 from . import acoustics as ac
 
+__all__ = [
+    'IdealGas1D', 'Acoustic2ndOrder1D', 'AcousticMaterial2ndOrder',
+]
+
 
 class IdealGas1D(fld.Field1D):
     """Class for simulation of one-dimensional nonlinear acoustic fields in ideal gases."""
 
     def __init__(self, convective=True, nl_state=True, *args, **kwargs):
         """Class constructor.
 
@@ -106,16 +109,16 @@
 
         Args:
             See pyfds.fields.Field1D constructor arguments.
         """
 
         if not (hasattr(kwargs['material'], 'd_rho_p')
                 and hasattr(kwargs['material'], 'd_rho2_p')):
-            wn.warn('Material with properties d_rho_p and d_rho2_p is required for 2nd order '
-                    'nonlinear acoustic simulation.')
+            raise RuntimeError('Material with properties d_rho_p and d_rho2_p is required for '
+                               '2nd order nonlinear acoustic simulation.')
         super().__init__(*args, **kwargs)
 
         self.pressure = fld.FieldComponent(self.num_points)
         self.velocity = fld.FieldComponent(self.num_points)
         self.density = fld.FieldComponent(self.num_points)
 
         # initialize attributes sparse matrices and buffered material parameters
```

### Comparing `pyfds-0.2.0/pyfds/regions.py` & `pyfds-0.3.0/pyfds/regions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 import numpy as np
 
+__all__ = [
+    'Boundary', 'MaterialRegion', 'Output',
+]
+
 
 class Region:
     """Storage for the indices of points and metadata for which specific behaviour is to be
     applied (boundaries, materials, output, etc.)."""
 
     def __init__(self, indices, name=''):
         """Class constructor.
```

### Comparing `pyfds-0.2.0/pyfds/thermal.py` & `pyfds-0.3.0/pyfds/thermal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 import logging as lo
 import numpy as np
 from . import fields as fld
 
+__all__ = [
+    'Thermal1D', 'Thermal2D', 'Thermal3DAxi', 'ThermalMaterial'
+]
+
 logger = lo.getLogger('pyfds')
 
 
 class Thermal1D(fld.Field1D):
     """Class for simulation of one-dimensional thermal fields."""
 
     def __init__(self, *args, **kwargs):
```

### Comparing `pyfds-0.2.0/pyfds.egg-info/PKG-INFO` & `pyfds-0.3.0/pyfds.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfds
-Version: 0.2.0
+Version: 0.3.0
 Summary: Modular field simulation tool using finite differences.
 Home-page: https://emt.uni-paderborn.de
 Author: Leander Claes
 Author-email: Leander Claes <claes@emt.uni-paderborn.de>
 License: Copyright (c) 2017 Leander Claes
         
         Redistribution and use in source and binary forms, with or without
@@ -38,18 +38,25 @@
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
-Provides-Extra: doc
-Provides-Extra: test
 License-File: LICENSE
 License-File: AUTHORS.rst
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: scipy
+Provides-Extra: doc
+Requires-Dist: setuptools_scm; extra == "doc"
+Requires-Dist: sphinx; extra == "doc"
+Requires-Dist: sphinx-rtd-theme; extra == "doc"
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
 
 =====
 pyfds
 =====
 .. image:: https://zenodo.org/badge/92026828.svg
    :target: https://zenodo.org/badge/latestdoi/92026828
 
@@ -59,7 +66,9 @@
 --------
  
 * One-dimensional, two-dimensional, and axial-symmetric linear acoustic field simulation.
 * One-dimensional nonlinear acoustic field simulation in ideal gases and arbitrary fluids using second order approximation.
 * Two-dimensional acoustic simulation with moving medium.
 * One-dimensional, two-dimensional, and axial-symmetric thermal field simulation.
 * One-dimensional and two-dimensional electrostatic field simulation.
+* Options to couple simulations.
+* One-dimensional thermo-acoustic simulation.
```

### Comparing `pyfds-0.2.0/pyfds.egg-info/SOURCES.txt` & `pyfds-0.3.0/pyfds.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -5,35 +5,39 @@
 README.rst
 pyproject.toml
 setup.py
 .github/workflows/python-package.yml
 doc/acoustic_flow.rst
 doc/acoustics.rst
 doc/conf.py
+doc/coupling.rst
 doc/electrostatics.rst
 doc/ex_acoustics.rst
 doc/ex_visualization.rst
 doc/examples.rst
 doc/fields.rst
 doc/gfx.rst
 doc/index.rst
 doc/nonlinear_acoustics.rst
 doc/regions.rst
 doc/thermal.rst
 doc/usage.rst
 pyfds/__init__.py
 pyfds/acoustic_flow.py
 pyfds/acoustics.py
+pyfds/coupled_fields.py
+pyfds/coupling.py
 pyfds/electrostatics.py
 pyfds/fields.py
 pyfds/gfx.py
 pyfds/nonlinear_acoustics.py
 pyfds/regions.py
 pyfds/thermal.py
 pyfds.egg-info/PKG-INFO
 pyfds.egg-info/SOURCES.txt
 pyfds.egg-info/dependency_links.txt
 pyfds.egg-info/requires.txt
 pyfds.egg-info/top_level.txt
 test/test_acoustics.py
+test/test_coupling.py
 test/test_fields.py
 test/test_regions.py
```

### Comparing `pyfds-0.2.0/pyproject.toml` & `pyfds-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyfds-0.2.0/setup.py` & `pyfds-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `pyfds-0.2.0/test/test_acoustics.py` & `pyfds-0.3.0/test/test_acoustics.py`

 * *Files identical despite different names*

### Comparing `pyfds-0.2.0/test/test_fields.py` & `pyfds-0.3.0/test/test_fields.py`

 * *Files identical despite different names*

