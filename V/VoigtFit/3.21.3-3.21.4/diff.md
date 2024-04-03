# Comparing `tmp/VoigtFit-3.21.3.tar.gz` & `tmp/VoigtFit-3.21.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VoigtFit-3.21.3.tar", last modified: Tue Dec 12 10:34:21 2023, max compression
+gzip compressed data, was "VoigtFit-3.21.4.tar", last modified: Wed Apr  3 14:56:34 2024, max compression
```

## Comparing `VoigtFit-3.21.3.tar` & `VoigtFit-3.21.4.tar`

### file list

```diff
@@ -1,53 +1,55 @@
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-12-12 10:34:21.632074 VoigtFit-3.21.3/
--rw-r--r--   0 krogager   (501) staff       (20)      248 2022-03-27 13:11:46.000000 VoigtFit-3.21.3/AUTHORS.rst
--rw-r--r--   0 krogager   (501) staff       (20)     1095 2022-03-27 13:11:46.000000 VoigtFit-3.21.3/LICENSE
--rw-r--r--   0 krogager   (501) staff       (20)       90 2022-03-27 13:11:46.000000 VoigtFit-3.21.3/MANIFEST.in
--rw-r--r--   0 krogager   (501) staff       (20)     2976 2023-12-12 10:34:21.631927 VoigtFit-3.21.3/PKG-INFO
--rw-r--r--   0 krogager   (501) staff       (20)     2393 2022-05-03 11:48:30.000000 VoigtFit-3.21.3/README.rst
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-12-12 10:34:21.621463 VoigtFit-3.21.3/VoigtFit/
--rw-r--r--   0 krogager   (501) staff       (20)        7 2023-12-12 10:33:57.000000 VoigtFit-3.21.3/VoigtFit/VERSION
--rw-r--r--   0 krogager   (501) staff       (20)     1313 2022-03-27 13:11:46.000000 VoigtFit-3.21.3/VoigtFit/__init__.py
--rw-r--r--   0 krogager   (501) staff       (20)     1842 2023-11-28 11:43:49.000000 VoigtFit-3.21.3/VoigtFit/__main__.py
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-12-12 10:34:21.623615 VoigtFit-3.21.3/VoigtFit/container/
--rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:11:46.000000 VoigtFit-3.21.3/VoigtFit/container/__init__.py
--rw-r--r--   0 krogager   (501) staff       (20)     5401 2022-03-27 13:11:46.000000 VoigtFit-3.21.3/VoigtFit/container/components.py
--rw-r--r--   0 krogager   (501) staff       (20)   105654 2023-12-11 16:42:50.000000 VoigtFit-3.21.3/VoigtFit/container/dataset.py
--rw-r--r--   0 krogager   (501) staff       (20)     4466 2022-07-21 13:29:16.000000 VoigtFit-3.21.3/VoigtFit/container/lines.py
--rw-r--r--   0 krogager   (501) staff       (20)    23426 2022-07-21 13:29:16.000000 VoigtFit-3.21.3/VoigtFit/container/regions.py
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-12-12 10:34:21.624327 VoigtFit-3.21.3/VoigtFit/funcs/
--rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:11:46.000000 VoigtFit-3.21.3/VoigtFit/funcs/__init__.py
--rw-r--r--   0 krogager   (501) staff       (20)     4009 2022-03-27 13:11:46.000000 VoigtFit-3.21.3/VoigtFit/funcs/limits.py
--rw-r--r--   0 krogager   (501) staff       (20)    13301 2023-12-11 17:16:18.000000 VoigtFit-3.21.3/VoigtFit/funcs/voigt.py
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-12-12 10:34:21.625786 VoigtFit-3.21.3/VoigtFit/io/
--rw-r--r--   0 krogager   (501) staff       (20)       43 2022-03-27 13:11:46.000000 VoigtFit-3.21.3/VoigtFit/io/__init__.py
--rw-r--r--   0 krogager   (501) staff       (20)    16646 2023-12-10 21:17:13.000000 VoigtFit-3.21.3/VoigtFit/io/fits_input.py
--rw-r--r--   0 krogager   (501) staff       (20)    16812 2022-03-27 13:11:46.000000 VoigtFit-3.21.3/VoigtFit/io/hdf5_save.py
--rw-r--r--   0 krogager   (501) staff       (20)    81493 2023-12-10 21:17:13.000000 VoigtFit-3.21.3/VoigtFit/io/output.py
--rw-r--r--   0 krogager   (501) staff       (20)    31727 2023-12-11 16:17:40.000000 VoigtFit-3.21.3/VoigtFit/io/parse_input.py
--rw-r--r--   0 krogager   (501) staff       (20)    26196 2023-12-11 16:14:40.000000 VoigtFit-3.21.3/VoigtFit/main.py
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-12-12 10:34:21.627754 VoigtFit-3.21.3/VoigtFit/static/
--rw-r--r--   0 krogager   (501) staff       (20)     2116 2022-03-27 13:11:46.000000 VoigtFit-3.21.3/VoigtFit/static/Asplund2009.dat
--rw-r--r--   0 krogager   (501) staff       (20)     2747 2022-07-21 13:05:22.000000 VoigtFit-3.21.3/VoigtFit/static/Asplund2021.dat
--rw-r--r--   0 krogager   (501) staff       (20)     2435 2022-03-27 13:11:46.000000 VoigtFit-3.21.3/VoigtFit/static/C_complexes.dat
--rw-r--r--   0 krogager   (501) staff       (20)     5437 2022-03-27 13:11:46.000000 VoigtFit-3.21.3/VoigtFit/static/C_full_labels.txt
--rw-r--r--   0 krogager   (501) staff       (20)      561 2023-05-17 08:46:43.000000 VoigtFit-3.21.3/VoigtFit/static/Konstantopoulou2022.dat
--rw-r--r--   0 krogager   (501) staff       (20)     2750 2022-03-27 13:11:46.000000 VoigtFit-3.21.3/VoigtFit/static/Lodders2009.dat
--rw-r--r--   0 krogager   (501) staff       (20)     5705 2023-11-28 11:43:49.000000 VoigtFit-3.21.3/VoigtFit/static/input_template.txt
--rw-r--r--   0 krogager   (501) staff       (20)   168929 2023-12-12 10:33:48.000000 VoigtFit-3.21.3/VoigtFit/static/linelist.dat
--rw-r--r--   0 krogager   (501) staff       (20)  2536616 2022-03-27 13:11:46.000000 VoigtFit-3.21.3/VoigtFit/static/telluric_em_abs.npz
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-12-12 10:34:21.631650 VoigtFit-3.21.3/VoigtFit/utils/
--rw-r--r--   0 krogager   (501) staff       (20)     1285 2022-07-21 13:29:16.000000 VoigtFit-3.21.3/VoigtFit/utils/Asplund.py
--rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:11:46.000000 VoigtFit-3.21.3/VoigtFit/utils/__init__.py
--rw-r--r--   0 krogager   (501) staff       (20)      638 2023-05-17 08:46:43.000000 VoigtFit-3.21.3/VoigtFit/utils/depletion.py
--rw-r--r--   0 krogager   (501) staff       (20)     2625 2022-07-21 13:29:16.000000 VoigtFit-3.21.3/VoigtFit/utils/line_complexes.py
--rw-r--r--   0 krogager   (501) staff       (20)    23052 2022-05-03 11:57:56.000000 VoigtFit-3.21.3/VoigtFit/utils/molecules.py
--rw-r--r--   0 krogager   (501) staff       (20)      603 2022-03-27 13:11:46.000000 VoigtFit-3.21.3/VoigtFit/utils/terminal_attributes.py
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-12-12 10:34:21.622437 VoigtFit-3.21.3/VoigtFit.egg-info/
--rw-r--r--   0 krogager   (501) staff       (20)     2976 2023-12-12 10:34:21.000000 VoigtFit-3.21.3/VoigtFit.egg-info/PKG-INFO
--rw-r--r--   0 krogager   (501) staff       (20)     1155 2023-12-12 10:34:21.000000 VoigtFit-3.21.3/VoigtFit.egg-info/SOURCES.txt
--rw-r--r--   0 krogager   (501) staff       (20)        1 2023-12-12 10:34:21.000000 VoigtFit-3.21.3/VoigtFit.egg-info/dependency_links.txt
--rw-r--r--   0 krogager   (501) staff       (20)      120 2023-12-12 10:34:21.000000 VoigtFit-3.21.3/VoigtFit.egg-info/entry_points.txt
--rw-r--r--   0 krogager   (501) staff       (20)       54 2023-12-12 10:34:21.000000 VoigtFit-3.21.3/VoigtFit.egg-info/requires.txt
--rw-r--r--   0 krogager   (501) staff       (20)        9 2023-12-12 10:34:21.000000 VoigtFit-3.21.3/VoigtFit.egg-info/top_level.txt
--rw-r--r--   0 krogager   (501) staff       (20)       38 2023-12-12 10:34:21.632107 VoigtFit-3.21.3/setup.cfg
--rw-r--r--   0 krogager   (501) staff       (20)     5234 2023-11-28 11:43:49.000000 VoigtFit-3.21.3/setup.py
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2024-04-03 14:56:34.605471 VoigtFit-3.21.4/
+-rw-r--r--   0 krogager   (501) staff       (20)      248 2022-03-27 13:11:46.000000 VoigtFit-3.21.4/AUTHORS.rst
+-rw-r--r--   0 krogager   (501) staff       (20)     1095 2022-03-27 13:11:46.000000 VoigtFit-3.21.4/LICENSE
+-rw-r--r--   0 krogager   (501) staff       (20)       90 2022-03-27 13:11:46.000000 VoigtFit-3.21.4/MANIFEST.in
+-rw-r--r--   0 krogager   (501) staff       (20)     3135 2024-04-03 14:56:34.605229 VoigtFit-3.21.4/PKG-INFO
+-rw-r--r--   0 krogager   (501) staff       (20)     2393 2022-05-03 11:48:30.000000 VoigtFit-3.21.4/README.rst
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2024-04-03 14:56:34.591271 VoigtFit-3.21.4/VoigtFit/
+-rw-r--r--   0 krogager   (501) staff       (20)        7 2024-04-03 14:50:24.000000 VoigtFit-3.21.4/VoigtFit/VERSION
+-rw-r--r--   0 krogager   (501) staff       (20)     1313 2022-03-27 13:11:46.000000 VoigtFit-3.21.4/VoigtFit/__init__.py
+-rw-r--r--   0 krogager   (501) staff       (20)     1842 2023-11-28 11:43:49.000000 VoigtFit-3.21.4/VoigtFit/__main__.py
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2024-04-03 14:56:34.594140 VoigtFit-3.21.4/VoigtFit/container/
+-rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:11:46.000000 VoigtFit-3.21.4/VoigtFit/container/__init__.py
+-rw-r--r--   0 krogager   (501) staff       (20)     5401 2022-03-27 13:11:46.000000 VoigtFit-3.21.4/VoigtFit/container/components.py
+-rw-r--r--   0 krogager   (501) staff       (20)   105654 2023-12-11 16:42:50.000000 VoigtFit-3.21.4/VoigtFit/container/dataset.py
+-rw-r--r--   0 krogager   (501) staff       (20)     4466 2022-07-21 13:29:16.000000 VoigtFit-3.21.4/VoigtFit/container/lines.py
+-rw-r--r--   0 krogager   (501) staff       (20)    23426 2022-07-21 13:29:16.000000 VoigtFit-3.21.4/VoigtFit/container/regions.py
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2024-04-03 14:56:34.594993 VoigtFit-3.21.4/VoigtFit/funcs/
+-rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:11:46.000000 VoigtFit-3.21.4/VoigtFit/funcs/__init__.py
+-rw-r--r--   0 krogager   (501) staff       (20)     4009 2022-03-27 13:11:46.000000 VoigtFit-3.21.4/VoigtFit/funcs/limits.py
+-rw-r--r--   0 krogager   (501) staff       (20)    13301 2023-12-11 17:16:18.000000 VoigtFit-3.21.4/VoigtFit/funcs/voigt.py
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2024-04-03 14:56:34.596438 VoigtFit-3.21.4/VoigtFit/io/
+-rw-r--r--   0 krogager   (501) staff       (20)       43 2022-03-27 13:11:46.000000 VoigtFit-3.21.4/VoigtFit/io/__init__.py
+-rw-r--r--   0 krogager   (501) staff       (20)    16646 2023-12-10 21:17:13.000000 VoigtFit-3.21.4/VoigtFit/io/fits_input.py
+-rw-r--r--   0 krogager   (501) staff       (20)    16812 2022-03-27 13:11:46.000000 VoigtFit-3.21.4/VoigtFit/io/hdf5_save.py
+-rw-r--r--   0 krogager   (501) staff       (20)    81493 2023-12-10 21:17:13.000000 VoigtFit-3.21.4/VoigtFit/io/output.py
+-rw-r--r--   0 krogager   (501) staff       (20)    31727 2023-12-11 16:17:40.000000 VoigtFit-3.21.4/VoigtFit/io/parse_input.py
+-rw-r--r--   0 krogager   (501) staff       (20)    26196 2023-12-11 16:14:40.000000 VoigtFit-3.21.4/VoigtFit/main.py
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2024-04-03 14:56:34.599434 VoigtFit-3.21.4/VoigtFit/static/
+-rw-r--r--   0 krogager   (501) staff       (20)     2116 2022-03-27 13:11:46.000000 VoigtFit-3.21.4/VoigtFit/static/Asplund2009.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     2747 2022-07-21 13:05:22.000000 VoigtFit-3.21.4/VoigtFit/static/Asplund2021.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     2435 2022-03-27 13:11:46.000000 VoigtFit-3.21.4/VoigtFit/static/C_complexes.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     5437 2022-03-27 13:11:46.000000 VoigtFit-3.21.4/VoigtFit/static/C_full_labels.txt
+-rw-r--r--   0 krogager   (501) staff       (20)      561 2023-05-17 08:46:43.000000 VoigtFit-3.21.4/VoigtFit/static/Konstantopoulou2022.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     2750 2022-03-27 13:11:46.000000 VoigtFit-3.21.4/VoigtFit/static/Lodders2009.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     5705 2023-11-28 11:43:49.000000 VoigtFit-3.21.4/VoigtFit/static/input_template.txt
+-rw-r--r--   0 krogager   (501) staff       (20)   168996 2024-04-03 14:49:41.000000 VoigtFit-3.21.4/VoigtFit/static/linelist.dat
+-rw-r--r--   0 krogager   (501) staff       (20)  2536616 2022-03-27 13:11:46.000000 VoigtFit-3.21.4/VoigtFit/static/telluric_em_abs.npz
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2024-04-03 14:56:34.604274 VoigtFit-3.21.4/VoigtFit/utils/
+-rw-r--r--   0 krogager   (501) staff       (20)     1285 2022-07-21 13:29:16.000000 VoigtFit-3.21.4/VoigtFit/utils/Asplund.py
+-rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:11:46.000000 VoigtFit-3.21.4/VoigtFit/utils/__init__.py
+-rw-r--r--   0 krogager   (501) staff       (20)      638 2023-05-17 08:46:43.000000 VoigtFit-3.21.4/VoigtFit/utils/depletion.py
+-rw-r--r--   0 krogager   (501) staff       (20)     2625 2022-07-21 13:29:16.000000 VoigtFit-3.21.4/VoigtFit/utils/line_complexes.py
+-rw-r--r--   0 krogager   (501) staff       (20)    23052 2022-05-03 11:57:56.000000 VoigtFit-3.21.4/VoigtFit/utils/molecules.py
+-rw-r--r--   0 krogager   (501) staff       (20)      603 2022-03-27 13:11:46.000000 VoigtFit-3.21.4/VoigtFit/utils/terminal_attributes.py
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2024-04-03 14:56:34.604948 VoigtFit-3.21.4/VoigtFit.egg-info/
+-rw-r--r--   0 krogager   (501) staff       (20)     3135 2024-04-03 14:56:34.000000 VoigtFit-3.21.4/VoigtFit.egg-info/PKG-INFO
+-rw-r--r--   0 krogager   (501) staff       (20)     1178 2024-04-03 14:56:34.000000 VoigtFit-3.21.4/VoigtFit.egg-info/SOURCES.txt
+-rw-r--r--   0 krogager   (501) staff       (20)        1 2024-04-03 14:56:34.000000 VoigtFit-3.21.4/VoigtFit.egg-info/dependency_links.txt
+-rw-r--r--   0 krogager   (501) staff       (20)      120 2024-04-03 14:56:34.000000 VoigtFit-3.21.4/VoigtFit.egg-info/entry_points.txt
+-rw-r--r--   0 krogager   (501) staff       (20)       54 2024-04-03 14:56:34.000000 VoigtFit-3.21.4/VoigtFit.egg-info/requires.txt
+-rw-r--r--   0 krogager   (501) staff       (20)        9 2024-04-03 14:56:34.000000 VoigtFit-3.21.4/VoigtFit.egg-info/top_level.txt
+-rw-r--r--   0 krogager   (501) staff       (20)       38 2024-04-03 14:56:34.605514 VoigtFit-3.21.4/setup.cfg
+-rw-r--r--   0 krogager   (501) staff       (20)     5234 2023-11-28 11:43:49.000000 VoigtFit-3.21.4/setup.py
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2024-04-03 14:56:34.604563 VoigtFit-3.21.4/tests/
+-rw-r--r--   0 krogager   (501) staff       (20)     5372 2023-12-10 21:17:13.000000 VoigtFit-3.21.4/tests/test_voigtfit.py
```

### Comparing `VoigtFit-3.21.3/LICENSE` & `VoigtFit-3.21.4/LICENSE`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.3/PKG-INFO` & `VoigtFit-3.21.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 Metadata-Version: 2.1
 Name: VoigtFit
-Version: 3.21.3
+Version: 3.21.4
 Summary: Voigt Profile Fitting in Python
 Home-page: https://github.com/jkrogager/VoigtFit
 Author: Jens-Kristian Krogager
 Author-email: krogager.jk@gmail.com
 License: MIT
 Keywords: voigtfit absorption analysis
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.5
 License-File: LICENSE
 License-File: AUTHORS.rst
+Requires-Dist: astropy
+Requires-Dist: future
+Requires-Dist: h5py>=2.1
+Requires-Dist: lmfit
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: scipy
 
 
 ========
 VoigtFit
 ========
 
 Absorption line fitting implemented in Python.
```

### Comparing `VoigtFit-3.21.3/README.rst` & `VoigtFit-3.21.4/README.rst`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.3/VoigtFit/__init__.py` & `VoigtFit-3.21.4/VoigtFit/__init__.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.3/VoigtFit/__main__.py` & `VoigtFit-3.21.4/VoigtFit/__main__.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.3/VoigtFit/container/components.py` & `VoigtFit-3.21.4/VoigtFit/container/components.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.3/VoigtFit/container/dataset.py` & `VoigtFit-3.21.4/VoigtFit/container/dataset.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.3/VoigtFit/container/lines.py` & `VoigtFit-3.21.4/VoigtFit/container/lines.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.3/VoigtFit/container/regions.py` & `VoigtFit-3.21.4/VoigtFit/container/regions.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.3/VoigtFit/funcs/limits.py` & `VoigtFit-3.21.4/VoigtFit/funcs/limits.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.3/VoigtFit/funcs/voigt.py` & `VoigtFit-3.21.4/VoigtFit/funcs/voigt.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.3/VoigtFit/io/fits_input.py` & `VoigtFit-3.21.4/VoigtFit/io/fits_input.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.3/VoigtFit/io/hdf5_save.py` & `VoigtFit-3.21.4/VoigtFit/io/hdf5_save.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.3/VoigtFit/io/output.py` & `VoigtFit-3.21.4/VoigtFit/io/output.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.3/VoigtFit/io/parse_input.py` & `VoigtFit-3.21.4/VoigtFit/io/parse_input.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.3/VoigtFit/main.py` & `VoigtFit-3.21.4/VoigtFit/main.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.3/VoigtFit/static/Asplund2009.dat` & `VoigtFit-3.21.4/VoigtFit/static/Asplund2009.dat`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.3/VoigtFit/static/Asplund2021.dat` & `VoigtFit-3.21.4/VoigtFit/static/Asplund2021.dat`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.3/VoigtFit/static/C_complexes.dat` & `VoigtFit-3.21.4/VoigtFit/static/C_complexes.dat`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.3/VoigtFit/static/C_full_labels.txt` & `VoigtFit-3.21.4/VoigtFit/static/C_full_labels.txt`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.3/VoigtFit/static/Konstantopoulou2022.dat` & `VoigtFit-3.21.4/VoigtFit/static/Konstantopoulou2022.dat`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.3/VoigtFit/static/Lodders2009.dat` & `VoigtFit-3.21.4/VoigtFit/static/Lodders2009.dat`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.3/VoigtFit/static/input_template.txt` & `VoigtFit-3.21.4/VoigtFit/static/input_template.txt`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.3/VoigtFit/static/linelist.dat` & `VoigtFit-3.21.4/VoigtFit/static/linelist.dat`

 * *Files 0% similar despite different names*

```diff
@@ -1684,15 +1684,16 @@
 CIa_1656         CIa        1656.2660  5.98e-02  3.981e+08  12.011
 CIb_1657         CIb        1657.0080  1.07e-01  3.981e+08  12.011
 CIa_1657         CIa        1657.3792  3.56e-02  3.981e+08  12.011
 CIa_1657.9       CIa        1657.9070  4.76e-02  3.981e+08  12.011
 CIb_1658         CIb        1658.1211  3.57e-02  3.981e+08  12.011
 
 # Manual Entries, check references from source file.
-SiIIa_1264       SiIIa      1264.7377  1.05e+00  2.93E+09   28.085
+SiIIa_1264       SiIIa      1264.7377  1.05e+00  2.95E+09   28.085
+SiIIa_1265       SiIIa      1265.0020  1.17e-01  2.95E+09   28.085
 FeIIa_2333       FeIIa      2333.5156  7.78E-02  2.62e+08   55.847
 C13I_1328        C13I       1328.8250  5.81e-02  4.571e+08  13.003
 C13Ia_1329       C13Ia      1329.0790  1.96e-02  4.571e+08  13.003
 C13Ia_1329.1     C13Ia      1329.0940  2.38e-02  4.467e+08  13.003
 C13Ia_1329.12    C13Ia      1329.1150  1.47e-02  4.571e+08  13.003
 C13Ib_1329       C13Ib      1329.5699  4.36e-02  4.467e+08  13.003
 C13Ib_1329.6     C13Ib      1329.5920  1.46e-02  4.571e+08  13.003
```

### Comparing `VoigtFit-3.21.3/VoigtFit/static/telluric_em_abs.npz` & `VoigtFit-3.21.4/VoigtFit/static/telluric_em_abs.npz`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.3/VoigtFit/utils/Asplund.py` & `VoigtFit-3.21.4/VoigtFit/utils/Asplund.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.3/VoigtFit/utils/depletion.py` & `VoigtFit-3.21.4/VoigtFit/utils/depletion.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.3/VoigtFit/utils/line_complexes.py` & `VoigtFit-3.21.4/VoigtFit/utils/line_complexes.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.3/VoigtFit/utils/molecules.py` & `VoigtFit-3.21.4/VoigtFit/utils/molecules.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.3/VoigtFit/utils/terminal_attributes.py` & `VoigtFit-3.21.4/VoigtFit/utils/terminal_attributes.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.3/VoigtFit.egg-info/PKG-INFO` & `VoigtFit-3.21.4/VoigtFit.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 Metadata-Version: 2.1
 Name: VoigtFit
-Version: 3.21.3
+Version: 3.21.4
 Summary: Voigt Profile Fitting in Python
 Home-page: https://github.com/jkrogager/VoigtFit
 Author: Jens-Kristian Krogager
 Author-email: krogager.jk@gmail.com
 License: MIT
 Keywords: voigtfit absorption analysis
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.5
 License-File: LICENSE
 License-File: AUTHORS.rst
+Requires-Dist: astropy
+Requires-Dist: future
+Requires-Dist: h5py>=2.1
+Requires-Dist: lmfit
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: scipy
 
 
 ========
 VoigtFit
 ========
 
 Absorption line fitting implemented in Python.
```

### Comparing `VoigtFit-3.21.3/VoigtFit.egg-info/SOURCES.txt` & `VoigtFit-3.21.4/VoigtFit.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -36,8 +36,9 @@
 VoigtFit/static/linelist.dat
 VoigtFit/static/telluric_em_abs.npz
 VoigtFit/utils/Asplund.py
 VoigtFit/utils/__init__.py
 VoigtFit/utils/depletion.py
 VoigtFit/utils/line_complexes.py
 VoigtFit/utils/molecules.py
-VoigtFit/utils/terminal_attributes.py
+VoigtFit/utils/terminal_attributes.py
+tests/test_voigtfit.py
```

### Comparing `VoigtFit-3.21.3/setup.py` & `VoigtFit-3.21.4/setup.py`

 * *Files identical despite different names*

