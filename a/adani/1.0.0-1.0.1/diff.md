# Comparing `tmp/adani-1.0.0.tar.gz` & `tmp/adani-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adani-1.0.0.tar", last modified: Fri Mar 29 15:05:55 2024, max compression
+gzip compressed data, was "adani-1.0.1.tar", last modified: Wed Apr  3 12:25:15 2024, max compression
```

## Comparing `adani-1.0.0.tar` & `adani-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:05:55.534346 adani-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-29 15:05:47.000000 adani-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-03-29 15:05:55.534346 adani-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-03-29 15:05:47.000000 adani-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:05:55.530346 adani-1.0.0/inc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:05:55.530346 adani-1.0.0/inc/adani/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-29 15:05:47.000000 adani-1.0.0/inc/adani/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-29 15:05:55.534346 adani-1.0.0/inc/adani/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:05:55.534346 adani-1.0.0/inc/adani.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-03-29 15:05:55.000000 adani-1.0.0/inc/adani.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-29 15:05:55.000000 adani-1.0.0/inc/adani.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 15:05:55.000000 adani-1.0.0/inc/adani.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-29 15:05:55.000000 adani-1.0.0/inc/adani.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-03-29 15:05:47.000000 adani-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 15:05:55.534346 adani-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-03-29 15:05:47.000000 adani-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:05:55.534346 adani-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11258 2024-03-29 15:05:47.000000 adani-1.0.0/tests/test_approx_coeff_func.py
--rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-03-29 15:05:47.000000 adani-1.0.0/tests/test_asy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-03-29 15:05:47.000000 adani-1.0.0/tests/test_exact_coeff_func.py
--rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-03-29 15:05:47.000000 adani-1.0.0/tests/test_high_scale.py
--rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-03-29 15:05:47.000000 adani-1.0.0/tests/test_highenergy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-03-29 15:05:47.000000 adani-1.0.0/tests/test_massless.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-03-29 15:05:47.000000 adani-1.0.0/tests/test_mc_integral.py
--rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-03-29 15:05:47.000000 adani-1.0.0/tests/test_splitting_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-03-29 15:05:47.000000 adani-1.0.0/tests/test_threshold.py
--rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-03-29 15:05:47.000000 adani-1.0.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:25:15.014588 adani-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-04-03 12:25:07.000000 adani-1.0.1/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-03 12:25:07.000000 adani-1.0.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:25:14.994588 adani-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:25:14.998588 adani-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-03 12:25:07.000000 adani-1.0.1/.github/workflows/pip.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-03 12:25:07.000000 adani-1.0.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-03 12:25:07.000000 adani-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-03 12:25:07.000000 adani-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-04-03 12:25:07.000000 adani-1.0.1/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-03 12:25:07.000000 adani-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-04-03 12:25:15.014588 adani-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-04-03 12:25:07.000000 adani-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:25:14.998588 adani-1.0.1/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-03 12:25:07.000000 adani-1.0.1/bin/adani-config.in
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-03 12:25:07.000000 adani-1.0.1/bin/adani.pc.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:25:15.002588 adani-1.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)  2182791 2024-04-03 12:25:07.000000 adani-1.0.1/docs/Tesi_Laurenti.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)   150134 2024-04-03 12:25:07.000000 adani-1.0.1/docs/approximation_smallx_nll.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    21151 2024-04-03 12:25:07.000000 adani-1.0.1/docs/approximation_smallx_nll.tex
+-rw-r--r--   0 runner    (1001) docker     (127)    98460 2024-04-03 12:25:07.000000 adani-1.0.1/docs/montecarlointegration.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     7553 2024-04-03 12:25:07.000000 adani-1.0.1/docs/montecarlointegration.tex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:25:15.002588 adani-1.0.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-03 12:25:07.000000 adani-1.0.1/examples/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-03 12:25:07.000000 adani-1.0.1/examples/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:25:14.994588 adani-1.0.1/inc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:25:15.002588 adani-1.0.1/inc/adani/
+-rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-04-03 12:25:07.000000 adani-1.0.1/inc/adani/ApproximateCoefficientFunction.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-03 12:25:07.000000 adani-1.0.1/inc/adani/AsymptoticCoefficientFunction.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-03 12:25:07.000000 adani-1.0.1/inc/adani/CoefficientFunction.h
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-03 12:25:07.000000 adani-1.0.1/inc/adani/Constants.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7126 2024-04-03 12:25:07.000000 adani-1.0.1/inc/adani/Convolution.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-04-03 12:25:07.000000 adani-1.0.1/inc/adani/ExactCoefficientFunction.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10929 2024-04-03 12:25:07.000000 adani-1.0.1/inc/adani/HighEnergyCoefficientFunction.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-04-03 12:25:07.000000 adani-1.0.1/inc/adani/HighScaleCoefficientFunction.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-04-03 12:25:07.000000 adani-1.0.1/inc/adani/HighScaleSplitLogs.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-04-03 12:25:07.000000 adani-1.0.1/inc/adani/MasslessCoefficientFunction.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-03 12:25:07.000000 adani-1.0.1/inc/adani/MatchingCondition.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-04-03 12:25:07.000000 adani-1.0.1/inc/adani/SpecialFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9091 2024-04-03 12:25:07.000000 adani-1.0.1/inc/adani/SplittingFunction.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-04-03 12:25:07.000000 adani-1.0.1/inc/adani/ThresholdCoefficientFunction.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-03 12:25:07.000000 adani-1.0.1/inc/adani/Value.h
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-03 12:25:07.000000 adani-1.0.1/inc/adani/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24502 2024-04-03 12:25:07.000000 adani-1.0.1/inc/adani/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-03 12:25:07.000000 adani-1.0.1/inc/adani/adani.h
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-03 12:25:07.000000 adani-1.0.1/inc/adani/version.h.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:25:15.010588 adani-1.0.1/inc/adani.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-04-03 12:25:14.000000 adani-1.0.1/inc/adani.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-03 12:25:14.000000 adani-1.0.1/inc/adani.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 12:25:14.000000 adani-1.0.1/inc/adani.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-03 12:25:14.000000 adani-1.0.1/inc/adani.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:25:15.006588 adani-1.0.1/output/
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-03 12:25:07.000000 adani-1.0.1/output/Q.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-04-03 12:25:07.000000 adani-1.0.1/output/output_grid.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-03 12:25:07.000000 adani-1.0.1/output/output_grid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:25:15.006588 adani-1.0.1/output/runcards/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-03 12:25:07.000000 adani-1.0.1/output/runcards/runcard_2g.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-03 12:25:07.000000 adani-1.0.1/output/runcards/runcard_2q.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-03 12:25:07.000000 adani-1.0.1/output/runcards/runcard_Lg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-03 12:25:07.000000 adani-1.0.1/output/runcards/runcard_Lq.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12866 2024-04-03 12:25:07.000000 adani-1.0.1/output/x.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-03 12:25:07.000000 adani-1.0.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:25:15.006588 adani-1.0.1/pywrap/
+-rw-r--r--   0 runner    (1001) docker     (127)    13346 2024-04-03 12:25:07.000000 adani-1.0.1/pywrap/pywrap.cc
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 12:25:15.014588 adani-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-03 12:25:07.000000 adani-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:25:15.010588 adani-1.0.1/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    16105 2024-04-03 12:25:07.000000 adani-1.0.1/src/ApproximateCoefficientFunction.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-04-03 12:25:07.000000 adani-1.0.1/src/AsymptoticCoefficientFunction.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-04-03 12:25:07.000000 adani-1.0.1/src/CoefficientFunction.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    21293 2024-04-03 12:25:07.000000 adani-1.0.1/src/Convolution.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    20526 2024-04-03 12:25:07.000000 adani-1.0.1/src/ExactCoefficientFunction.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    45692 2024-04-03 12:25:07.000000 adani-1.0.1/src/HighEnergyCoefficientFunction.cc
+-rw-r--r--   0 runner    (1001) docker     (127)   235403 2024-04-03 12:25:07.000000 adani-1.0.1/src/HighScaleCoefficientFunction.cc
+-rw-r--r--   0 runner    (1001) docker     (127)   215112 2024-04-03 12:25:07.000000 adani-1.0.1/src/HighScaleSplitLogs.cc
+-rw-r--r--   0 runner    (1001) docker     (127)   210010 2024-04-03 12:25:07.000000 adani-1.0.1/src/MasslessCoefficientFunction.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    46992 2024-04-03 12:25:07.000000 adani-1.0.1/src/MatchingCondition.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    12537 2024-04-03 12:25:07.000000 adani-1.0.1/src/SpecialFunctions.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    23952 2024-04-03 12:25:07.000000 adani-1.0.1/src/SplittingFunction.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    16950 2024-04-03 12:25:07.000000 adani-1.0.1/src/ThresholdCoefficientFunction.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7172 2024-04-03 12:25:07.000000 adani-1.0.1/src/Value.cc
+-rw-r--r--   0 runner    (1001) docker     (127)   546646 2024-04-03 12:25:07.000000 adani-1.0.1/src/hplog.f
+-rw-r--r--   0 runner    (1001) docker     (127)   747023 2024-04-03 12:25:07.000000 adani-1.0.1/src/hqcoef.f
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:25:15.010588 adani-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11258 2024-04-03 12:25:07.000000 adani-1.0.1/tests/test_approx_coeff_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-04-03 12:25:07.000000 adani-1.0.1/tests/test_asy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-03 12:25:07.000000 adani-1.0.1/tests/test_exact_coeff_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-04-03 12:25:07.000000 adani-1.0.1/tests/test_high_scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-04-03 12:25:07.000000 adani-1.0.1/tests/test_highenergy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-04-03 12:25:07.000000 adani-1.0.1/tests/test_massless.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-03 12:25:07.000000 adani-1.0.1/tests/test_mc_integral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-04-03 12:25:07.000000 adani-1.0.1/tests/test_splitting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-04-03 12:25:07.000000 adani-1.0.1/tests/test_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-03 12:25:07.000000 adani-1.0.1/versioneer.py
```

### Comparing `adani-1.0.0/LICENSE` & `adani-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adani-1.0.0/PKG-INFO` & `adani-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adani
-Version: 1.0.0
+Version: 1.0.1
 Summary: Code computing approximate DIS N3LO coefficients
 Author: Niccolò Laurenti
 License: AGPLv3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: adani Version: 1.0.0 Summary: Code computing
+Metadata-Version: 2.1 Name: adani Version: 1.0.1 Summary: Code computing
 approximate DIS N3LO coefficients Author: NiccolÃ² Laurenti License: AGPLv3
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE # ADANI ADANI (Approximate DIS At N3LO Implementation) is a C++ code
 that computes an approximation for the DIS coefficient functions at N3LO in
 heavy quark production, that are not fully known yet. ## Citation Policy When
 using this code please cite [![arXiv](https://img.shields.io/badge/arXiv-
 2401.12139-b31b1b?labelColor=222222)](https://arxiv.org/abs/2401.12139) ##
```

### Comparing `adani-1.0.0/README.md` & `adani-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `adani-1.0.0/inc/adani.egg-info/PKG-INFO` & `adani-1.0.1/inc/adani.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adani
-Version: 1.0.0
+Version: 1.0.1
 Summary: Code computing approximate DIS N3LO coefficients
 Author: Niccolò Laurenti
 License: AGPLv3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: adani Version: 1.0.0 Summary: Code computing
+Metadata-Version: 2.1 Name: adani Version: 1.0.1 Summary: Code computing
 approximate DIS N3LO coefficients Author: NiccolÃ² Laurenti License: AGPLv3
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE # ADANI ADANI (Approximate DIS At N3LO Implementation) is a C++ code
 that computes an approximation for the DIS coefficient functions at N3LO in
 heavy quark production, that are not fully known yet. ## Citation Policy When
 using this code please cite [![arXiv](https://img.shields.io/badge/arXiv-
 2401.12139-b31b1b?labelColor=222222)](https://arxiv.org/abs/2401.12139) ##
```

### Comparing `adani-1.0.0/setup.py` & `adani-1.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="adani",
     version=versioneer.get_version(),
-    cmdclass=versioneer.get_cmdclass(),
     description="Code computing approximate DIS N3LO coefficients",
     author="Niccolò Laurenti",
     license="AGPLv3",
     packages=find_packages(where="inc"),
     package_dir={"": "inc"},
     cmake_install_dir="inc/adani",
     cmake_args=['-DPYTHON_ONLY:BOOL=ON'],
```

### Comparing `adani-1.0.0/tests/test_approx_coeff_func.py` & `adani-1.0.1/tests/test_approx_coeff_func.py`

 * *Files identical despite different names*

### Comparing `adani-1.0.0/tests/test_asy.py` & `adani-1.0.1/tests/test_asy.py`

 * *Files identical despite different names*

### Comparing `adani-1.0.0/tests/test_exact_coeff_func.py` & `adani-1.0.1/tests/test_exact_coeff_func.py`

 * *Files identical despite different names*

### Comparing `adani-1.0.0/tests/test_high_scale.py` & `adani-1.0.1/tests/test_high_scale.py`

 * *Files identical despite different names*

### Comparing `adani-1.0.0/tests/test_highenergy.py` & `adani-1.0.1/tests/test_highenergy.py`

 * *Files identical despite different names*

### Comparing `adani-1.0.0/tests/test_massless.py` & `adani-1.0.1/tests/test_massless.py`

 * *Files identical despite different names*

### Comparing `adani-1.0.0/tests/test_mc_integral.py` & `adani-1.0.1/tests/test_mc_integral.py`

 * *Files identical despite different names*

### Comparing `adani-1.0.0/tests/test_splitting_functions.py` & `adani-1.0.1/tests/test_splitting_functions.py`

 * *Files identical despite different names*

### Comparing `adani-1.0.0/tests/test_threshold.py` & `adani-1.0.1/tests/test_threshold.py`

 * *Files identical despite different names*

### Comparing `adani-1.0.0/versioneer.py` & `adani-1.0.1/versioneer.py`

 * *Files identical despite different names*

