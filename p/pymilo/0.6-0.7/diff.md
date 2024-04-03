# Comparing `tmp/pymilo-0.6.tar.gz` & `tmp/pymilo-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymilo-0.6.tar", last modified: Wed Mar 27 11:16:27 2024, max compression
+gzip compressed data, was "pymilo-0.7.tar", last modified: Wed Apr  3 04:56:46 2024, max compression
```

## Comparing `pymilo-0.6.tar` & `pymilo-0.7.tar`

### file list

```diff
@@ -1,50 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:16:27.290066 pymilo-0.6/
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-03-27 11:16:19.000000 pymilo-0.6/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-27 11:16:19.000000 pymilo-0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14092 2024-03-27 11:16:27.290066 pymilo-0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6834 2024-03-27 11:16:19.000000 pymilo-0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:16:27.286066 pymilo-0.6/pymilo/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-27 11:16:19.000000 pymilo-0.6/pymilo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:16:27.286066 pymilo-0.6/pymilo/chains/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-27 11:16:19.000000 pymilo-0.6/pymilo/chains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5267 2024-03-27 11:16:19.000000 pymilo-0.6/pymilo/chains/clustering_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-03-27 11:16:19.000000 pymilo-0.6/pymilo/chains/decision_tree_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     7312 2024-03-27 11:16:19.000000 pymilo-0.6/pymilo/chains/linear_model_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-03-27 11:16:19.000000 pymilo-0.6/pymilo/chains/naive_bayes_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     5294 2024-03-27 11:16:19.000000 pymilo-0.6/pymilo/chains/neural_network_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-03-27 11:16:19.000000 pymilo-0.6/pymilo/chains/svm_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:16:27.286066 pymilo-0.6/pymilo/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-27 11:16:19.000000 pymilo-0.6/pymilo/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-03-27 11:16:19.000000 pymilo-0.6/pymilo/exceptions/deserialize_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-03-27 11:16:19.000000 pymilo-0.6/pymilo/exceptions/pymilo_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-03-27 11:16:19.000000 pymilo-0.6/pymilo/exceptions/serialize_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-03-27 11:16:19.000000 pymilo-0.6/pymilo/pymilo_func.py
--rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-03-27 11:16:19.000000 pymilo-0.6/pymilo/pymilo_obj.py
--rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-03-27 11:16:19.000000 pymilo-0.6/pymilo/pymilo_param.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:16:27.290066 pymilo-0.6/pymilo/transporters/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-27 11:16:19.000000 pymilo-0.6/pymilo/transporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-03-27 11:16:19.000000 pymilo-0.6/pymilo/transporters/adamoptimizer_transporter.py
--rw-r--r--   0 runner    (1001) docker     (127)    12751 2024-03-27 11:16:19.000000 pymilo-0.6/pymilo/transporters/baseloss_transporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-03-27 11:16:19.000000 pymilo-0.6/pymilo/transporters/bisecting_tree_transporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9885 2024-03-27 11:16:19.000000 pymilo-0.6/pymilo/transporters/cfnode_transporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-03-27 11:16:19.000000 pymilo-0.6/pymilo/transporters/function_transporter.py
--rw-r--r--   0 runner    (1001) docker     (127)    16633 2024-03-27 11:16:19.000000 pymilo-0.6/pymilo/transporters/general_data_structure_transporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-03-27 11:16:19.000000 pymilo-0.6/pymilo/transporters/labelbinarizer_transporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-03-27 11:16:19.000000 pymilo-0.6/pymilo/transporters/lossfunction_transporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-03-27 11:16:19.000000 pymilo-0.6/pymilo/transporters/randomstate_transporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-03-27 11:16:19.000000 pymilo-0.6/pymilo/transporters/sgdoptimizer_transporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-03-27 11:16:19.000000 pymilo-0.6/pymilo/transporters/transporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-03-27 11:16:19.000000 pymilo-0.6/pymilo/transporters/tree_transporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:16:27.290066 pymilo-0.6/pymilo/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-27 11:16:19.000000 pymilo-0.6/pymilo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-03-27 11:16:19.000000 pymilo-0.6/pymilo/utils/data_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6073 2024-03-27 11:16:19.000000 pymilo-0.6/pymilo/utils/test_pymilo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-03-27 11:16:19.000000 pymilo-0.6/pymilo/utils/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:16:27.290066 pymilo-0.6/pymilo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14092 2024-03-27 11:16:27.000000 pymilo-0.6/pymilo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-03-27 11:16:27.000000 pymilo-0.6/pymilo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 11:16:27.000000 pymilo-0.6/pymilo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-27 11:16:27.000000 pymilo-0.6/pymilo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-27 11:16:27.000000 pymilo-0.6/pymilo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 11:16:27.290066 pymilo-0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-03-27 11:16:19.000000 pymilo-0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:56:46.668030 pymilo-0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-03 04:56:38.000000 pymilo-0.7/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-03 04:56:38.000000 pymilo-0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14743 2024-04-03 04:56:46.668030 pymilo-0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6833 2024-04-03 04:56:38.000000 pymilo-0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:56:46.660030 pymilo-0.7/pymilo/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:56:46.664030 pymilo-0.7/pymilo/chains/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/chains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5267 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/chains/clustering_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/chains/decision_tree_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7312 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/chains/linear_model_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/chains/naive_bayes_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4688 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/chains/neighbours_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5294 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/chains/neural_network_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/chains/svm_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:56:46.664030 pymilo-0.7/pymilo/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/exceptions/deserialize_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/exceptions/pymilo_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/exceptions/serialize_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/pymilo_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/pymilo_obj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/pymilo_param.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:56:46.664030 pymilo-0.7/pymilo/transporters/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/transporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/transporters/adamoptimizer_transporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12751 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/transporters/baseloss_transporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/transporters/bisecting_tree_transporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9885 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/transporters/cfnode_transporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/transporters/function_transporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16633 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/transporters/general_data_structure_transporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/transporters/labelbinarizer_transporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/transporters/lossfunction_transporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/transporters/neighbors_tree_transporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/transporters/randomstate_transporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/transporters/sgdoptimizer_transporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/transporters/transporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/transporters/tree_transporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:56:46.668030 pymilo-0.7/pymilo/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/utils/data_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7069 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/utils/test_pymilo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/utils/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:56:46.668030 pymilo-0.7/pymilo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14743 2024-04-03 04:56:46.000000 pymilo-0.7/pymilo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-03 04:56:46.000000 pymilo-0.7/pymilo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 04:56:46.000000 pymilo-0.7/pymilo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-03 04:56:46.000000 pymilo-0.7/pymilo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 04:56:46.000000 pymilo-0.7/pymilo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 04:56:46.668030 pymilo-0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-03 04:56:38.000000 pymilo-0.7/setup.py
```

### Comparing `pymilo-0.6/AUTHORS.md` & `pymilo-0.7/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `pymilo-0.6/LICENSE` & `pymilo-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pymilo-0.6/PKG-INFO` & `pymilo-0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pymilo
-Version: 0.6
+Version: 0.7
 Summary: Transportation of ML models
 Home-page: https://github.com/openscilab/pymilo
-Download-URL: https://github.com/openscilab/pymilo/tarball/v0.6
+Download-URL: https://github.com/openscilab/pymilo/tarball/v0.7
 Author: PyMilo Development Team
 Author-email: pymilo@openscilab.com
 License: MIT
 Project-URL: Source, https://github.com/openscilab/pymilo
 Keywords: python3 python machine_learning ML
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -125,17 +125,17 @@
 
 
 ## Installation
 
 ### PyPI
 
 - Check [Python Packaging User Guide](https://packaging.python.org/installing/)
-- Run `pip install pymilo==0.6`
+- Run `pip install pymilo==0.7`
 ### Source code
-- Download [Version 0.6](https://github.com/openscilab/pymilo/archive/v0.6.zip) or [Latest Source](https://github.com/openscilab/pymilo/archive/dev.zip)
+- Download [Version 0.7](https://github.com/openscilab/pymilo/archive/v0.7.zip) or [Latest Source](https://github.com/openscilab/pymilo/archive/dev.zip)
 - Run `pip install .`
 
 ## Usage
 ### Model preparation 
 ```pycon
 >>> from sklearn import datasets
 >>> from pymilo import Export, Import
@@ -172,15 +172,15 @@
 | ---------------- | ---------------- | 
 | Linear Models &#x2705; | - | 
 | Neural networks &#x2705; | -  | 
 | Trees &#x2705; | -  | 
 | Clustering &#x2705; | -  | 
 | Naïve Bayes &#x2705; | -  | 
 | Support vector machines (SVMs) &#x2705; | -  | 
-| Nearest Neighbors &#x274C; | -  | 
+| Nearest Neighbors &#x2705; | -  | 
 | Ensemble Models &#x274C; | - | 
 Details are available in [Supported Models](https://github.com/openscilab/pymilo/blob/main/SUPPORTED_MODELS.md).
 
 ## Issues & bug reports
 
 Just fill an issue and describe it. We'll check it ASAP! or send an email to [pymilo@openscilab.com](mailto:pymilo@openscilab.com "pymilo@openscilab.com"). 
 
@@ -200,25 +200,42 @@
 
 Give a ⭐️ if this project helped you!
 
 ### Donate to our project
 If you do like our project and we hope that you do, can you please support us? Our project is not and is never going to be working for profit. We need the money just so we can continue doing what we do ;-) .			
 
 <a href="https://openscilab.com/#donation" target="_blank"><img src="https://github.com/openscilab/pymilo/raw/main/otherfiles/donation.png" height="90px" width="270px" alt="PyMilo Donation"></a>
-
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 ### Added
 ### Changed
-
+## [0.7] - 2024-04-03
+### Added
+- `pymilo_nearest_neighbor_test` function added to `test_pymilo.py`
+- `NeighborsTreeTransporter` Transporter
+- `LocalOutlierFactor` model
+- `RadiusNeighborsClassifier` model
+- `RadiusNeighborsRegressor` model
+- `NearestCentroid` model
+- `NearestNeighbors` model
+- `KNeighborsClassifier` model
+- `KNeighborsRegressor` model
+- Neighbors models test runner
+- Neighbors chain
+### Changed
+- Tests config modified
+- Neighbors params initialized in `pymilo_param`
+- Neighbors support added to `pymilo_func.py`
+- `SUPPORTED_MODELS.md` updated
+- `README.md` updated
 ## [0.6] - 2024-03-27
 ### Added
 - `deserialize_primitive_type` function in `GeneralDataStructureTransporter`
 - `is_deserialized_ndarray` function in `GeneralDataStructureTransporter`
 - `deep_deserialize_ndarray` function in `GeneralDataStructureTransporter`
 - `deep_serialize_ndarray`  function in `GeneralDataStructureTransporter`
 - `SVR` model
@@ -347,14 +364,15 @@
 - `linear_model_chain` refactored
 ## [0.1] - 2023-06-29
 ### Added
 - scikit-learn linear models support
 - `Export` class
 - `Import` class
 
-[Unreleased]: https://github.com/openscilab/pymilo/compare/v0.6...dev
+[Unreleased]: https://github.com/openscilab/pymilo/compare/v0.7...dev
+[0.7]: https://github.com/openscilab/pymilo/compare/v0.6...v0.7
 [0.6]: https://github.com/openscilab/pymilo/compare/v0.5...v0.6
 [0.5]: https://github.com/openscilab/pymilo/compare/v0.4...v0.5
 [0.4]: https://github.com/openscilab/pymilo/compare/v0.3...v0.4
 [0.3]: https://github.com/openscilab/pymilo/compare/v0.2...v0.3
 [0.2]: https://github.com/openscilab/pymilo/compare/v0.1...v0.2
 [0.1]: https://github.com/openscilab/pymilo/compare/e887108...v0.1
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: pymilo Version: 0.6 Summary: Transportation of ML
+Metadata-Version: 2.1 Name: pymilo Version: 0.7 Summary: Transportation of ML
 models Home-page: https://github.com/openscilab/pymilo Download-URL: https://
-github.com/openscilab/pymilo/tarball/v0.6 Author: PyMilo Development Team
+github.com/openscilab/pymilo/tarball/v0.7 Author: PyMilo Development Team
 Author-email: pymilo@openscilab.com License: MIT Project-URL: Source, https://
 github.com/openscilab/pymilo Keywords: python3 python machine_learning ML
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: Natural Language :: English Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
@@ -52,17 +52,17 @@
         [https://github.com/openscilab/    [https://github.com/openscilab/
    CI  pymilo/actions/workflows/test.yml/ pymilo/actions/workflows/test.yml/
              badge.svg?branch=main]             badge.svg?branch=dev]
                           _[_h_t_t_p_s_:_/_/_a_p_p_._c_o_d_a_c_y_._c_o_m_/_p_r_o_j_e_c_t_/
 Code Quality _[_C_o_d_e_F_a_c_t_o_r_]           _b_a_d_g_e_/_G_r_a_d_e_/            _[_c_o_d_e_b_e_a_t_ _b_a_d_g_e_]
                           _9_e_e_e_c_9_9_e_d_1_1_f_4_d_9_b_8_6_a_f_3_6_d_c_9_0_f_5_f_7_5_3_]
 ## Installation ### PyPI - Check [Python Packaging User Guide](https://
-packaging.python.org/installing/) - Run `pip install pymilo==0.6` ### Source
-code - Download [Version 0.6](https://github.com/openscilab/pymilo/archive/
-v0.6.zip) or [Latest Source](https://github.com/openscilab/pymilo/archive/
+packaging.python.org/installing/) - Run `pip install pymilo==0.7` ### Source
+code - Download [Version 0.7](https://github.com/openscilab/pymilo/archive/
+v0.7.zip) or [Latest Source](https://github.com/openscilab/pymilo/archive/
 dev.zip) - Run `pip install .` ## Usage ### Model preparation ```pycon >>> from
 sklearn import datasets >>> from pymilo import Export, Import >>> from
 sklearn.linear_model import LinearRegression >>> import os >>> X, Y =
 datasets.load_diabetes(return_X_y=True) >>> threshold = 20 >>> X_train, X_test
 = X[:-threshold], X[-threshold:] >>> Y_train, Y_test = Y[:-threshold], Y[-
 threshold:] >>> model = LinearRegression() >>> #### Train the model using the
 training sets >>> model.fit(X_train, Y_train) ``` ### Save model ```pycon >>>
@@ -72,47 +72,56 @@
 Import the pymilo-exported model and get a real scikit model >>> imported_model
 = Import(PATH_TO_JSON_FILE) ``` ### Get the associated model ```pycon >>>
 imported_sklearn_model = imported_model.to_model() ``` #### Note:
 `imported_sklearn_model` has the **exact same** functionality as the `model`
 object earlier. ## Supported ML models | scikit-learn | PyTorch | | -----------
 ----- | ---------------- | | Linear Models ✅ | - | | Neural networks ✅ | - | |
 Trees ✅ | - | | Clustering ✅ | - | | NaÃ¯ve Bayes ✅ | - | | Support vector
-machines (SVMs) ✅ | - | | Nearest Neighbors ❌ | - | | Ensemble Models ❌ | - |
+machines (SVMs) ✅ | - | | Nearest Neighbors ✅ | - | | Ensemble Models ❌ | - |
 Details are available in [Supported Models](https://github.com/openscilab/
 pymilo/blob/main/SUPPORTED_MODELS.md). ## Issues & bug reports Just fill an
 issue and describe it. We'll check it ASAP! or send an email to
 [pymilo@openscilab.com](mailto:pymilo@openscilab.com "pymilo@openscilab.com").
 - Please complete the issue template You can also join our discord server
 _[_D_i_s_c_o_r_d_ _C_h_a_n_n_e_l_]## Show your support ### Star this repo Give a â­ï¸ if this
 project helped you! ### Donate to our project If you do like our project and we
 hope that you do, can you please support us? Our project is not and is never
 going to be working for profit. We need the money just so we can continue doing
 what we do ;-) . _[_P_y_M_i_l_o_ _D_o_n_a_t_i_o_n_]# Changelog All notable changes to this
 project will be documented in this file. The format is based on [Keep a
 Changelog](http://keepachangelog.com/en/1.0.0/) and this project adheres to
 [Semantic Versioning](http://semver.org/spec/v2.0.0.html). ## [Unreleased] ###
-Added ### Changed ## [0.6] - 2024-03-27 ### Added -
-`deserialize_primitive_type` function in `GeneralDataStructureTransporter` -
-`is_deserialized_ndarray` function in `GeneralDataStructureTransporter` -
-`deep_deserialize_ndarray` function in `GeneralDataStructureTransporter` -
-`deep_serialize_ndarray` function in `GeneralDataStructureTransporter` - `SVR`
-model - `SVC` model - `One Class SVM` model - `NuSVR` model - `NuSVC` model -
-`Linear SVR` model - `Linear SVC` model - SVM models test runner - SVM chain
-### Changed - `pymilo_param.py` updated - `pymilo_obj.py` updated to use
-predefined strings - `TreeTransporter` updated - `get_homogeneous_type`
-function in `util.py` updated - `GeneralDataStructureTransporter` updated to
-use deep ndarray serializer & deserializer - `check_str_in_iterable` updated -
-`Label Binarizer` Transporter updated - `Function` Transporter updated -
-`CFNode` Transporter updated - `Bisecting Tree` Transporter updated - Tests
-config modified - SVM params initialized in `pymilo_param` - SVM support added
-to `pymilo_func.py` - `SUPPORTED_MODELS.md` updated - `README.md` updated ##
-[0.5] - 2024-01-31 ### Added - `reset` function in the `Transport` interface -
-`reset` function implementation in `AbstractTransporter` - `Gaussian Naive
-Bayes` declared as `GaussianNB` model - `Multinomial Naive Bayes` model
-declared as `MultinomialNB` model - `Complement Naive Bayes` model declared as
+Added ### Changed ## [0.7] - 2024-04-03 ### Added -
+`pymilo_nearest_neighbor_test` function added to `test_pymilo.py` -
+`NeighborsTreeTransporter` Transporter - `LocalOutlierFactor` model -
+`RadiusNeighborsClassifier` model - `RadiusNeighborsRegressor` model -
+`NearestCentroid` model - `NearestNeighbors` model - `KNeighborsClassifier`
+model - `KNeighborsRegressor` model - Neighbors models test runner - Neighbors
+chain ### Changed - Tests config modified - Neighbors params initialized in
+`pymilo_param` - Neighbors support added to `pymilo_func.py` -
+`SUPPORTED_MODELS.md` updated - `README.md` updated ## [0.6] - 2024-03-27 ###
+Added - `deserialize_primitive_type` function in
+`GeneralDataStructureTransporter` - `is_deserialized_ndarray` function in
+`GeneralDataStructureTransporter` - `deep_deserialize_ndarray` function in
+`GeneralDataStructureTransporter` - `deep_serialize_ndarray` function in
+`GeneralDataStructureTransporter` - `SVR` model - `SVC` model - `One Class SVM`
+model - `NuSVR` model - `NuSVC` model - `Linear SVR` model - `Linear SVC` model
+- SVM models test runner - SVM chain ### Changed - `pymilo_param.py` updated -
+`pymilo_obj.py` updated to use predefined strings - `TreeTransporter` updated -
+`get_homogeneous_type` function in `util.py` updated -
+`GeneralDataStructureTransporter` updated to use deep ndarray serializer &
+deserializer - `check_str_in_iterable` updated - `Label Binarizer` Transporter
+updated - `Function` Transporter updated - `CFNode` Transporter updated -
+`Bisecting Tree` Transporter updated - Tests config modified - SVM params
+initialized in `pymilo_param` - SVM support added to `pymilo_func.py` -
+`SUPPORTED_MODELS.md` updated - `README.md` updated ## [0.5] - 2024-01-31 ###
+Added - `reset` function in the `Transport` interface - `reset` function
+implementation in `AbstractTransporter` - `Gaussian Naive Bayes` declared as
+`GaussianNB` model - `Multinomial Naive Bayes` model declared as
+`MultinomialNB` model - `Complement Naive Bayes` model declared as
 `ComplementNB` model - `Bernoulli Naive Bayes` model declared as `BernoulliNB`
 model - `Categorical Naive Bayes` model declared as `CategoricalNB` model -
 Naive Bayes models test runner - Naive Bayes chain ### Changed - `Transport`
 function of `AbstractTransporter` updated - fix the order of `CFNode` fields
 serialization in `CFNodeTransporter` - `GeneralDataStructureTransporter`
 support list of ndarray with different shapes - Tests config modified - Naive
 Bayes params initialized in `pymilo_param` - Naive Bayes support added to
@@ -150,13 +159,14 @@
 - `GeneralDataStructure` Transporter updated - `LabelBinerizer` Transporter
 updated - `linear model` chain updated - GeneralDataStructure transporter
 enhanced - LabelBinerizer transporter updated - transporters' chain router
 added to `pymilo func` - NeuralNetwork params initialized in `pymilo_param` -
 `pymilo_test` updated to support multiple models - `linear_model_chain`
 refactored ## [0.1] - 2023-06-29 ### Added - scikit-learn linear models support
 - `Export` class - `Import` class [Unreleased]: https://github.com/openscilab/
-pymilo/compare/v0.6...dev [0.6]: https://github.com/openscilab/pymilo/compare/
-v0.5...v0.6 [0.5]: https://github.com/openscilab/pymilo/compare/v0.4...v0.5
-[0.4]: https://github.com/openscilab/pymilo/compare/v0.3...v0.4 [0.3]: https://
-github.com/openscilab/pymilo/compare/v0.2...v0.3 [0.2]: https://github.com/
-openscilab/pymilo/compare/v0.1...v0.2 [0.1]: https://github.com/openscilab/
-pymilo/compare/e887108...v0.1
+pymilo/compare/v0.7...dev [0.7]: https://github.com/openscilab/pymilo/compare/
+v0.6...v0.7 [0.6]: https://github.com/openscilab/pymilo/compare/v0.5...v0.6
+[0.5]: https://github.com/openscilab/pymilo/compare/v0.4...v0.5 [0.4]: https://
+github.com/openscilab/pymilo/compare/v0.3...v0.4 [0.3]: https://github.com/
+openscilab/pymilo/compare/v0.2...v0.3 [0.2]: https://github.com/openscilab/
+pymilo/compare/v0.1...v0.2 [0.1]: https://github.com/openscilab/pymilo/compare/
+e887108...v0.1
```

### Comparing `pymilo-0.6/README.md` & `pymilo-0.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -82,17 +82,17 @@
 
 
 ## Installation
 
 ### PyPI
 
 - Check [Python Packaging User Guide](https://packaging.python.org/installing/)
-- Run `pip install pymilo==0.6`
+- Run `pip install pymilo==0.7`
 ### Source code
-- Download [Version 0.6](https://github.com/openscilab/pymilo/archive/v0.6.zip) or [Latest Source](https://github.com/openscilab/pymilo/archive/dev.zip)
+- Download [Version 0.7](https://github.com/openscilab/pymilo/archive/v0.7.zip) or [Latest Source](https://github.com/openscilab/pymilo/archive/dev.zip)
 - Run `pip install .`
 
 ## Usage
 ### Model preparation 
 ```pycon
 >>> from sklearn import datasets
 >>> from pymilo import Export, Import
@@ -129,15 +129,15 @@
 | ---------------- | ---------------- | 
 | Linear Models &#x2705; | - | 
 | Neural networks &#x2705; | -  | 
 | Trees &#x2705; | -  | 
 | Clustering &#x2705; | -  | 
 | Naïve Bayes &#x2705; | -  | 
 | Support vector machines (SVMs) &#x2705; | -  | 
-| Nearest Neighbors &#x274C; | -  | 
+| Nearest Neighbors &#x2705; | -  | 
 | Ensemble Models &#x274C; | - | 
 Details are available in [Supported Models](https://github.com/openscilab/pymilo/blob/main/SUPPORTED_MODELS.md).
 
 ## Issues & bug reports
 
 Just fill an issue and describe it. We'll check it ASAP! or send an email to [pymilo@openscilab.com](mailto:pymilo@openscilab.com "pymilo@openscilab.com"). 
 
@@ -156,8 +156,8 @@
 ### Star this repo
 
 Give a ⭐️ if this project helped you!
 
 ### Donate to our project
 If you do like our project and we hope that you do, can you please support us? Our project is not and is never going to be working for profit. We need the money just so we can continue doing what we do ;-) .			
 
-<a href="https://openscilab.com/#donation" target="_blank"><img src="https://github.com/openscilab/pymilo/raw/main/otherfiles/donation.png" height="90px" width="270px" alt="PyMilo Donation"></a>
+<a href="https://openscilab.com/#donation" target="_blank"><img src="https://github.com/openscilab/pymilo/raw/main/otherfiles/donation.png" height="90px" width="270px" alt="PyMilo Donation"></a>
```

#### html2text {}

```diff
@@ -28,17 +28,17 @@
         [https://github.com/openscilab/    [https://github.com/openscilab/
    CI  pymilo/actions/workflows/test.yml/ pymilo/actions/workflows/test.yml/
              badge.svg?branch=main]             badge.svg?branch=dev]
                           _[_h_t_t_p_s_:_/_/_a_p_p_._c_o_d_a_c_y_._c_o_m_/_p_r_o_j_e_c_t_/
 Code Quality _[_C_o_d_e_F_a_c_t_o_r_]           _b_a_d_g_e_/_G_r_a_d_e_/            _[_c_o_d_e_b_e_a_t_ _b_a_d_g_e_]
                           _9_e_e_e_c_9_9_e_d_1_1_f_4_d_9_b_8_6_a_f_3_6_d_c_9_0_f_5_f_7_5_3_]
 ## Installation ### PyPI - Check [Python Packaging User Guide](https://
-packaging.python.org/installing/) - Run `pip install pymilo==0.6` ### Source
-code - Download [Version 0.6](https://github.com/openscilab/pymilo/archive/
-v0.6.zip) or [Latest Source](https://github.com/openscilab/pymilo/archive/
+packaging.python.org/installing/) - Run `pip install pymilo==0.7` ### Source
+code - Download [Version 0.7](https://github.com/openscilab/pymilo/archive/
+v0.7.zip) or [Latest Source](https://github.com/openscilab/pymilo/archive/
 dev.zip) - Run `pip install .` ## Usage ### Model preparation ```pycon >>> from
 sklearn import datasets >>> from pymilo import Export, Import >>> from
 sklearn.linear_model import LinearRegression >>> import os >>> X, Y =
 datasets.load_diabetes(return_X_y=True) >>> threshold = 20 >>> X_train, X_test
 = X[:-threshold], X[-threshold:] >>> Y_train, Y_test = Y[:-threshold], Y[-
 threshold:] >>> model = LinearRegression() >>> #### Train the model using the
 training sets >>> model.fit(X_train, Y_train) ``` ### Save model ```pycon >>>
@@ -48,15 +48,15 @@
 Import the pymilo-exported model and get a real scikit model >>> imported_model
 = Import(PATH_TO_JSON_FILE) ``` ### Get the associated model ```pycon >>>
 imported_sklearn_model = imported_model.to_model() ``` #### Note:
 `imported_sklearn_model` has the **exact same** functionality as the `model`
 object earlier. ## Supported ML models | scikit-learn | PyTorch | | -----------
 ----- | ---------------- | | Linear Models ✅ | - | | Neural networks ✅ | - | |
 Trees ✅ | - | | Clustering ✅ | - | | NaÃ¯ve Bayes ✅ | - | | Support vector
-machines (SVMs) ✅ | - | | Nearest Neighbors ❌ | - | | Ensemble Models ❌ | - |
+machines (SVMs) ✅ | - | | Nearest Neighbors ✅ | - | | Ensemble Models ❌ | - |
 Details are available in [Supported Models](https://github.com/openscilab/
 pymilo/blob/main/SUPPORTED_MODELS.md). ## Issues & bug reports Just fill an
 issue and describe it. We'll check it ASAP! or send an email to
 [pymilo@openscilab.com](mailto:pymilo@openscilab.com "pymilo@openscilab.com").
 - Please complete the issue template You can also join our discord server
 _[_D_i_s_c_o_r_d_ _C_h_a_n_n_e_l_]## Show your support ### Star this repo Give a â­ï¸ if this
 project helped you! ### Donate to our project If you do like our project and we
```

### Comparing `pymilo-0.6/pymilo/chains/clustering_chain.py` & `pymilo-0.7/pymilo/chains/clustering_chain.py`

 * *Files identical despite different names*

### Comparing `pymilo-0.6/pymilo/chains/decision_tree_chain.py` & `pymilo-0.7/pymilo/chains/decision_tree_chain.py`

 * *Files identical despite different names*

### Comparing `pymilo-0.6/pymilo/chains/linear_model_chain.py` & `pymilo-0.7/pymilo/chains/linear_model_chain.py`

 * *Files identical despite different names*

### Comparing `pymilo-0.6/pymilo/chains/naive_bayes_chain.py` & `pymilo-0.7/pymilo/chains/naive_bayes_chain.py`

 * *Files identical despite different names*

### Comparing `pymilo-0.6/pymilo/chains/neural_network_chain.py` & `pymilo-0.7/pymilo/chains/neural_network_chain.py`

 * *Files identical despite different names*

### Comparing `pymilo-0.6/pymilo/chains/svm_chain.py` & `pymilo-0.7/pymilo/chains/svm_chain.py`

 * *Files identical despite different names*

### Comparing `pymilo-0.6/pymilo/exceptions/deserialize_exception.py` & `pymilo-0.7/pymilo/exceptions/deserialize_exception.py`

 * *Files identical despite different names*

### Comparing `pymilo-0.6/pymilo/exceptions/pymilo_exception.py` & `pymilo-0.7/pymilo/exceptions/pymilo_exception.py`

 * *Files identical despite different names*

### Comparing `pymilo-0.6/pymilo/exceptions/serialize_exception.py` & `pymilo-0.7/pymilo/exceptions/serialize_exception.py`

 * *Files identical despite different names*

### Comparing `pymilo-0.6/pymilo/pymilo_func.py` & `pymilo-0.7/pymilo/pymilo_func.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from .chains.linear_model_chain import transport_linear_model, is_linear_model
 from .chains.neural_network_chain import transport_neural_network, is_neural_network
 from .chains.decision_tree_chain import transport_decision_tree, is_decision_tree
 from .chains.clustering_chain import transport_clusterer, is_clusterer
 from .chains.naive_bayes_chain import transport_naive_bayes, is_naive_bayes
 from .chains.svm_chain import transport_svm, is_svm
+from .chains.neighbours_chain import transport_neighbor, is_neighbors
 
 from .transporters.transporter import Command
 
 
 def get_sklearn_version():
     """
     Return sklearn version.
@@ -38,14 +39,16 @@
         return transport_decision_tree(model, Command.SERIALIZE)
     elif is_clusterer(model):
         return transport_clusterer(model, Command.SERIALIZE)
     elif is_naive_bayes(model):
         return transport_naive_bayes(model, Command.SERIALIZE)
     elif is_svm(model):
         return transport_svm(model, Command.SERIALIZE)
+    elif is_neighbors(model):
+        return transport_neighbor(model, Command.SERIALIZE)
     else:
         return None
 
 
 def to_sklearn_model(import_obj):
     """
     Deserialize the imported object as a sklearn model.
@@ -62,14 +65,16 @@
         return transport_decision_tree(import_obj, Command.DESERIALZIE)
     elif is_clusterer(import_obj.type):
         return transport_clusterer(import_obj, Command.DESERIALZIE)
     elif is_naive_bayes(import_obj.type):
         return transport_naive_bayes(import_obj, Command.DESERIALZIE)
     elif is_svm(import_obj.type):
         return transport_svm(import_obj, Command.DESERIALZIE)
+    elif is_neighbors(import_obj.type):
+        return transport_neighbor(import_obj, Command.DESERIALZIE)
     else:
         return None
 
 
 def compare_model_outputs(exported_output,
                           imported_output,
                           epsilon_error=10**(-8)):
```

### Comparing `pymilo-0.6/pymilo/pymilo_obj.py` & `pymilo-0.7/pymilo/pymilo_obj.py`

 * *Files identical despite different names*

### Comparing `pymilo-0.6/pymilo/pymilo_param.py` & `pymilo-0.7/pymilo/pymilo_param.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # -*- coding: utf-8 -*-
 """Parameters and constants."""
+from sklearn.neighbors import KNeighborsRegressor
+from sklearn.neighbors import KNeighborsClassifier
+from sklearn.neighbors import RadiusNeighborsRegressor
+from sklearn.neighbors import RadiusNeighborsClassifier
+from sklearn.neighbors import NearestNeighbors
+from sklearn.neighbors import NearestCentroid
+from sklearn.neighbors import LocalOutlierFactor
+
 from sklearn.svm import SVR
 from sklearn.svm import SVC
 from sklearn.svm import OneClassSVM
 from sklearn.svm import NuSVR
 from sklearn.svm import NuSVC
 from sklearn.svm import LinearSVR
 from sklearn.svm import LinearSVC
@@ -84,15 +92,15 @@
 hdbscan_support = False
 try:
     from sklearn.cluster import HDBSCAN
     hdbscan_support = True
 except BaseException:
     pass
 
-PYMILO_VERSION = "0.6"
+PYMILO_VERSION = "0.7"
 NOT_SUPPORTED = "NOT_SUPPORTED"
 PYMILO_VERSION_DOES_NOT_EXIST = "Corrupted JSON file, `pymilo_version` doesn't exist in this file."
 UNEQUAL_PYMILO_VERSIONS = "warning: Installed Pymilo version differes from pymilo version used to create the JSON file."
 
 glm_support = {
     'GammaRegressor': False,
     'PoissonRegressor': False,
@@ -209,14 +217,24 @@
     "NuSVC": NuSVC,
     "NuSVR": NuSVR,
     "OneClassSVM": OneClassSVM,
     "SVC": SVC,
     "SVR": SVR,
 }
 
+SKLEARN_NEIGHBORS_TABLE = {
+    "KNeighborsRegressor": KNeighborsRegressor,
+    "KNeighborsClassifier": KNeighborsClassifier,
+    "RadiusNeighborsRegressor": RadiusNeighborsRegressor,
+    "RadiusNeighborsClassifier": RadiusNeighborsClassifier,
+    "NearestNeighbors": NearestNeighbors,
+    "NearestCentroid": NearestCentroid,
+    "LocalOutlierFactor": LocalOutlierFactor,
+}
+
 KEYS_NEED_PREPROCESSING_BEFORE_DESERIALIZATION = {
     "_label_binarizer": LabelBinarizer,  # in Ridge Classifier
     "active_": int32,  # in Lasso Lars
     "n_nonzero_coefs_": int64,  # in OMP-CV
     "scores_": dict,  # in Logistic Regression CV,
     "_base_loss": {},  # BaseLoss in Logistic Regression,
     "loss_function_": {},  # LossFunction in SGD Classifier,
@@ -235,8 +253,9 @@
 EXPORTED_MODELS_PATH = {
     "LINEAR_MODEL": "exported_linear_models",
     "NEURAL_NETWORK": "exported_neural_networks",
     "DECISION_TREE": "exported_decision_trees",
     "CLUSTERING": "exported_clusterings",
     "NAIVE_BAYES": "exported_naive_bayes",
     "SVM": "exported_svms",
+    "NEIGHBORS": "exported_neighbors"
 }
```

### Comparing `pymilo-0.6/pymilo/transporters/adamoptimizer_transporter.py` & `pymilo-0.7/pymilo/transporters/adamoptimizer_transporter.py`

 * *Files identical despite different names*

### Comparing `pymilo-0.6/pymilo/transporters/baseloss_transporter.py` & `pymilo-0.7/pymilo/transporters/baseloss_transporter.py`

 * *Files identical despite different names*

### Comparing `pymilo-0.6/pymilo/transporters/bisecting_tree_transporter.py` & `pymilo-0.7/pymilo/transporters/bisecting_tree_transporter.py`

 * *Files identical despite different names*

### Comparing `pymilo-0.6/pymilo/transporters/cfnode_transporter.py` & `pymilo-0.7/pymilo/transporters/cfnode_transporter.py`

 * *Files identical despite different names*

### Comparing `pymilo-0.6/pymilo/transporters/function_transporter.py` & `pymilo-0.7/pymilo/transporters/function_transporter.py`

 * *Files identical despite different names*

### Comparing `pymilo-0.6/pymilo/transporters/general_data_structure_transporter.py` & `pymilo-0.7/pymilo/transporters/general_data_structure_transporter.py`

 * *Files identical despite different names*

### Comparing `pymilo-0.6/pymilo/transporters/labelbinarizer_transporter.py` & `pymilo-0.7/pymilo/transporters/labelbinarizer_transporter.py`

 * *Files identical despite different names*

### Comparing `pymilo-0.6/pymilo/transporters/lossfunction_transporter.py` & `pymilo-0.7/pymilo/transporters/lossfunction_transporter.py`

 * *Files identical despite different names*

### Comparing `pymilo-0.6/pymilo/transporters/randomstate_transporter.py` & `pymilo-0.7/pymilo/transporters/randomstate_transporter.py`

 * *Files identical despite different names*

### Comparing `pymilo-0.6/pymilo/transporters/sgdoptimizer_transporter.py` & `pymilo-0.7/pymilo/transporters/sgdoptimizer_transporter.py`

 * *Files identical despite different names*

### Comparing `pymilo-0.6/pymilo/transporters/transporter.py` & `pymilo-0.7/pymilo/transporters/transporter.py`

 * *Files identical despite different names*

### Comparing `pymilo-0.6/pymilo/transporters/tree_transporter.py` & `pymilo-0.7/pymilo/transporters/tree_transporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
                 "node_count": tree_internal_state["node_count"],
                 "nodes": nodes,
                 "values": gdst.list_to_ndarray(tree_internal_state["values"]),
             }
 
             n_classes = np.ndarray(
                 shape=(np.intp(len(tree_params["n_classes"])),), dtype=np.intp)
-            for idx,_ in enumerate(n_classes):
+            for idx, _ in enumerate(n_classes):
                 n_classes[idx] = tree_params["n_classes"][idx]
 
             _tree = Tree(
                 tree_params["n_features"],
                 n_classes,
                 tree_params["n_outputs"]
             )
```

### Comparing `pymilo-0.6/pymilo/utils/data_exporter.py` & `pymilo-0.7/pymilo/utils/data_exporter.py`

 * *Files identical despite different names*

### Comparing `pymilo-0.6/pymilo/utils/test_pymilo.py` & `pymilo-0.7/pymilo/utils/test_pymilo.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 """pymilo test modules."""
 import os
 import copy
+from numpy import array_equal
 
 from ..pymilo_obj import Export
 from ..pymilo_obj import Import
 
 from sklearn.metrics import mean_squared_error, r2_score
 from sklearn.metrics import accuracy_score, hinge_loss
 
@@ -13,14 +14,15 @@
 
 from ..chains.linear_model_chain import is_linear_model
 from ..chains.neural_network_chain import is_neural_network
 from ..chains.decision_tree_chain import is_decision_tree
 from ..chains.clustering_chain import is_clusterer
 from ..chains.naive_bayes_chain import is_naive_bayes
 from ..chains.svm_chain import is_svm
+from ..chains.neighbours_chain import is_neighbors
 
 from ..pymilo_param import EXPORTED_MODELS_PATH
 
 
 def pymilo_export_path(model):
     """
     Return the associated folder name to save the json file generated by pymilo Export(applied to the given model).
@@ -38,14 +40,16 @@
         model_type = "DECISION_TREE"
     elif is_clusterer(model):
         model_type = "CLUSTERING"
     elif is_naive_bayes(model):
         model_type = "NAIVE_BAYES"
     elif is_svm(model):
         model_type = "SVM"
+    elif is_neighbors(model):
+        model_type = "NEIGHBORS"
     else:
         model_type = None
     return EXPORTED_MODELS_PATH[model_type]
 
 
 def pymilo_test(model, model_name):
     """
@@ -152,14 +156,33 @@
         return report_status(mse < epsilon_error, model_name)
     else:
         # TODO, apply peer to peer
         # Evaluation: peer to peer field type & value check
         return report_status(True, model_name)
 
 
+def pymilo_nearest_neighbor_test(nearest_neighbor, model_name, test_data):
+    """
+    Test the package's main structure in nearest neighbor task.
+
+    :param nearest_neighbor: the given nearest neighbor model
+    :type nearest_neighbor: sklearn's nearest neighbor class
+    :param model_name: model name
+    :type model_name: str
+    :param test_data: data for testing
+    :type test_data: np.ndarray or list
+    :return: True if the test succeed
+    """
+    x_test, _ = test_data
+    pre_pymilo_kneighbors = nearest_neighbor.kneighbors([x_test[0]], 3, return_distance=True)
+    post_pymilo_nearest_neighbor = pymilo_test(nearest_neighbor, model_name)
+    post_pymilo_kneighbors = post_pymilo_nearest_neighbor.kneighbors([x_test[0]], 3, return_distance=True)
+    report_status(array_equal(pre_pymilo_kneighbors, post_pymilo_kneighbors), model_name)
+
+
 def report_status(result, model_name):
     """
     Print status for each model.
 
     :param result: the test result
     :type result: bool
     :param model_name: model name
```

### Comparing `pymilo-0.6/pymilo/utils/util.py` & `pymilo-0.7/pymilo/utils/util.py`

 * *Files identical despite different names*

### Comparing `pymilo-0.6/pymilo.egg-info/PKG-INFO` & `pymilo-0.7/pymilo.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pymilo
-Version: 0.6
+Version: 0.7
 Summary: Transportation of ML models
 Home-page: https://github.com/openscilab/pymilo
-Download-URL: https://github.com/openscilab/pymilo/tarball/v0.6
+Download-URL: https://github.com/openscilab/pymilo/tarball/v0.7
 Author: PyMilo Development Team
 Author-email: pymilo@openscilab.com
 License: MIT
 Project-URL: Source, https://github.com/openscilab/pymilo
 Keywords: python3 python machine_learning ML
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -125,17 +125,17 @@
 
 
 ## Installation
 
 ### PyPI
 
 - Check [Python Packaging User Guide](https://packaging.python.org/installing/)
-- Run `pip install pymilo==0.6`
+- Run `pip install pymilo==0.7`
 ### Source code
-- Download [Version 0.6](https://github.com/openscilab/pymilo/archive/v0.6.zip) or [Latest Source](https://github.com/openscilab/pymilo/archive/dev.zip)
+- Download [Version 0.7](https://github.com/openscilab/pymilo/archive/v0.7.zip) or [Latest Source](https://github.com/openscilab/pymilo/archive/dev.zip)
 - Run `pip install .`
 
 ## Usage
 ### Model preparation 
 ```pycon
 >>> from sklearn import datasets
 >>> from pymilo import Export, Import
@@ -172,15 +172,15 @@
 | ---------------- | ---------------- | 
 | Linear Models &#x2705; | - | 
 | Neural networks &#x2705; | -  | 
 | Trees &#x2705; | -  | 
 | Clustering &#x2705; | -  | 
 | Naïve Bayes &#x2705; | -  | 
 | Support vector machines (SVMs) &#x2705; | -  | 
-| Nearest Neighbors &#x274C; | -  | 
+| Nearest Neighbors &#x2705; | -  | 
 | Ensemble Models &#x274C; | - | 
 Details are available in [Supported Models](https://github.com/openscilab/pymilo/blob/main/SUPPORTED_MODELS.md).
 
 ## Issues & bug reports
 
 Just fill an issue and describe it. We'll check it ASAP! or send an email to [pymilo@openscilab.com](mailto:pymilo@openscilab.com "pymilo@openscilab.com"). 
 
@@ -200,25 +200,42 @@
 
 Give a ⭐️ if this project helped you!
 
 ### Donate to our project
 If you do like our project and we hope that you do, can you please support us? Our project is not and is never going to be working for profit. We need the money just so we can continue doing what we do ;-) .			
 
 <a href="https://openscilab.com/#donation" target="_blank"><img src="https://github.com/openscilab/pymilo/raw/main/otherfiles/donation.png" height="90px" width="270px" alt="PyMilo Donation"></a>
-
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 ### Added
 ### Changed
-
+## [0.7] - 2024-04-03
+### Added
+- `pymilo_nearest_neighbor_test` function added to `test_pymilo.py`
+- `NeighborsTreeTransporter` Transporter
+- `LocalOutlierFactor` model
+- `RadiusNeighborsClassifier` model
+- `RadiusNeighborsRegressor` model
+- `NearestCentroid` model
+- `NearestNeighbors` model
+- `KNeighborsClassifier` model
+- `KNeighborsRegressor` model
+- Neighbors models test runner
+- Neighbors chain
+### Changed
+- Tests config modified
+- Neighbors params initialized in `pymilo_param`
+- Neighbors support added to `pymilo_func.py`
+- `SUPPORTED_MODELS.md` updated
+- `README.md` updated
 ## [0.6] - 2024-03-27
 ### Added
 - `deserialize_primitive_type` function in `GeneralDataStructureTransporter`
 - `is_deserialized_ndarray` function in `GeneralDataStructureTransporter`
 - `deep_deserialize_ndarray` function in `GeneralDataStructureTransporter`
 - `deep_serialize_ndarray`  function in `GeneralDataStructureTransporter`
 - `SVR` model
@@ -347,14 +364,15 @@
 - `linear_model_chain` refactored
 ## [0.1] - 2023-06-29
 ### Added
 - scikit-learn linear models support
 - `Export` class
 - `Import` class
 
-[Unreleased]: https://github.com/openscilab/pymilo/compare/v0.6...dev
+[Unreleased]: https://github.com/openscilab/pymilo/compare/v0.7...dev
+[0.7]: https://github.com/openscilab/pymilo/compare/v0.6...v0.7
 [0.6]: https://github.com/openscilab/pymilo/compare/v0.5...v0.6
 [0.5]: https://github.com/openscilab/pymilo/compare/v0.4...v0.5
 [0.4]: https://github.com/openscilab/pymilo/compare/v0.3...v0.4
 [0.3]: https://github.com/openscilab/pymilo/compare/v0.2...v0.3
 [0.2]: https://github.com/openscilab/pymilo/compare/v0.1...v0.2
 [0.1]: https://github.com/openscilab/pymilo/compare/e887108...v0.1
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: pymilo Version: 0.6 Summary: Transportation of ML
+Metadata-Version: 2.1 Name: pymilo Version: 0.7 Summary: Transportation of ML
 models Home-page: https://github.com/openscilab/pymilo Download-URL: https://
-github.com/openscilab/pymilo/tarball/v0.6 Author: PyMilo Development Team
+github.com/openscilab/pymilo/tarball/v0.7 Author: PyMilo Development Team
 Author-email: pymilo@openscilab.com License: MIT Project-URL: Source, https://
 github.com/openscilab/pymilo Keywords: python3 python machine_learning ML
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: Natural Language :: English Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
@@ -52,17 +52,17 @@
         [https://github.com/openscilab/    [https://github.com/openscilab/
    CI  pymilo/actions/workflows/test.yml/ pymilo/actions/workflows/test.yml/
              badge.svg?branch=main]             badge.svg?branch=dev]
                           _[_h_t_t_p_s_:_/_/_a_p_p_._c_o_d_a_c_y_._c_o_m_/_p_r_o_j_e_c_t_/
 Code Quality _[_C_o_d_e_F_a_c_t_o_r_]           _b_a_d_g_e_/_G_r_a_d_e_/            _[_c_o_d_e_b_e_a_t_ _b_a_d_g_e_]
                           _9_e_e_e_c_9_9_e_d_1_1_f_4_d_9_b_8_6_a_f_3_6_d_c_9_0_f_5_f_7_5_3_]
 ## Installation ### PyPI - Check [Python Packaging User Guide](https://
-packaging.python.org/installing/) - Run `pip install pymilo==0.6` ### Source
-code - Download [Version 0.6](https://github.com/openscilab/pymilo/archive/
-v0.6.zip) or [Latest Source](https://github.com/openscilab/pymilo/archive/
+packaging.python.org/installing/) - Run `pip install pymilo==0.7` ### Source
+code - Download [Version 0.7](https://github.com/openscilab/pymilo/archive/
+v0.7.zip) or [Latest Source](https://github.com/openscilab/pymilo/archive/
 dev.zip) - Run `pip install .` ## Usage ### Model preparation ```pycon >>> from
 sklearn import datasets >>> from pymilo import Export, Import >>> from
 sklearn.linear_model import LinearRegression >>> import os >>> X, Y =
 datasets.load_diabetes(return_X_y=True) >>> threshold = 20 >>> X_train, X_test
 = X[:-threshold], X[-threshold:] >>> Y_train, Y_test = Y[:-threshold], Y[-
 threshold:] >>> model = LinearRegression() >>> #### Train the model using the
 training sets >>> model.fit(X_train, Y_train) ``` ### Save model ```pycon >>>
@@ -72,47 +72,56 @@
 Import the pymilo-exported model and get a real scikit model >>> imported_model
 = Import(PATH_TO_JSON_FILE) ``` ### Get the associated model ```pycon >>>
 imported_sklearn_model = imported_model.to_model() ``` #### Note:
 `imported_sklearn_model` has the **exact same** functionality as the `model`
 object earlier. ## Supported ML models | scikit-learn | PyTorch | | -----------
 ----- | ---------------- | | Linear Models ✅ | - | | Neural networks ✅ | - | |
 Trees ✅ | - | | Clustering ✅ | - | | NaÃ¯ve Bayes ✅ | - | | Support vector
-machines (SVMs) ✅ | - | | Nearest Neighbors ❌ | - | | Ensemble Models ❌ | - |
+machines (SVMs) ✅ | - | | Nearest Neighbors ✅ | - | | Ensemble Models ❌ | - |
 Details are available in [Supported Models](https://github.com/openscilab/
 pymilo/blob/main/SUPPORTED_MODELS.md). ## Issues & bug reports Just fill an
 issue and describe it. We'll check it ASAP! or send an email to
 [pymilo@openscilab.com](mailto:pymilo@openscilab.com "pymilo@openscilab.com").
 - Please complete the issue template You can also join our discord server
 _[_D_i_s_c_o_r_d_ _C_h_a_n_n_e_l_]## Show your support ### Star this repo Give a â­ï¸ if this
 project helped you! ### Donate to our project If you do like our project and we
 hope that you do, can you please support us? Our project is not and is never
 going to be working for profit. We need the money just so we can continue doing
 what we do ;-) . _[_P_y_M_i_l_o_ _D_o_n_a_t_i_o_n_]# Changelog All notable changes to this
 project will be documented in this file. The format is based on [Keep a
 Changelog](http://keepachangelog.com/en/1.0.0/) and this project adheres to
 [Semantic Versioning](http://semver.org/spec/v2.0.0.html). ## [Unreleased] ###
-Added ### Changed ## [0.6] - 2024-03-27 ### Added -
-`deserialize_primitive_type` function in `GeneralDataStructureTransporter` -
-`is_deserialized_ndarray` function in `GeneralDataStructureTransporter` -
-`deep_deserialize_ndarray` function in `GeneralDataStructureTransporter` -
-`deep_serialize_ndarray` function in `GeneralDataStructureTransporter` - `SVR`
-model - `SVC` model - `One Class SVM` model - `NuSVR` model - `NuSVC` model -
-`Linear SVR` model - `Linear SVC` model - SVM models test runner - SVM chain
-### Changed - `pymilo_param.py` updated - `pymilo_obj.py` updated to use
-predefined strings - `TreeTransporter` updated - `get_homogeneous_type`
-function in `util.py` updated - `GeneralDataStructureTransporter` updated to
-use deep ndarray serializer & deserializer - `check_str_in_iterable` updated -
-`Label Binarizer` Transporter updated - `Function` Transporter updated -
-`CFNode` Transporter updated - `Bisecting Tree` Transporter updated - Tests
-config modified - SVM params initialized in `pymilo_param` - SVM support added
-to `pymilo_func.py` - `SUPPORTED_MODELS.md` updated - `README.md` updated ##
-[0.5] - 2024-01-31 ### Added - `reset` function in the `Transport` interface -
-`reset` function implementation in `AbstractTransporter` - `Gaussian Naive
-Bayes` declared as `GaussianNB` model - `Multinomial Naive Bayes` model
-declared as `MultinomialNB` model - `Complement Naive Bayes` model declared as
+Added ### Changed ## [0.7] - 2024-04-03 ### Added -
+`pymilo_nearest_neighbor_test` function added to `test_pymilo.py` -
+`NeighborsTreeTransporter` Transporter - `LocalOutlierFactor` model -
+`RadiusNeighborsClassifier` model - `RadiusNeighborsRegressor` model -
+`NearestCentroid` model - `NearestNeighbors` model - `KNeighborsClassifier`
+model - `KNeighborsRegressor` model - Neighbors models test runner - Neighbors
+chain ### Changed - Tests config modified - Neighbors params initialized in
+`pymilo_param` - Neighbors support added to `pymilo_func.py` -
+`SUPPORTED_MODELS.md` updated - `README.md` updated ## [0.6] - 2024-03-27 ###
+Added - `deserialize_primitive_type` function in
+`GeneralDataStructureTransporter` - `is_deserialized_ndarray` function in
+`GeneralDataStructureTransporter` - `deep_deserialize_ndarray` function in
+`GeneralDataStructureTransporter` - `deep_serialize_ndarray` function in
+`GeneralDataStructureTransporter` - `SVR` model - `SVC` model - `One Class SVM`
+model - `NuSVR` model - `NuSVC` model - `Linear SVR` model - `Linear SVC` model
+- SVM models test runner - SVM chain ### Changed - `pymilo_param.py` updated -
+`pymilo_obj.py` updated to use predefined strings - `TreeTransporter` updated -
+`get_homogeneous_type` function in `util.py` updated -
+`GeneralDataStructureTransporter` updated to use deep ndarray serializer &
+deserializer - `check_str_in_iterable` updated - `Label Binarizer` Transporter
+updated - `Function` Transporter updated - `CFNode` Transporter updated -
+`Bisecting Tree` Transporter updated - Tests config modified - SVM params
+initialized in `pymilo_param` - SVM support added to `pymilo_func.py` -
+`SUPPORTED_MODELS.md` updated - `README.md` updated ## [0.5] - 2024-01-31 ###
+Added - `reset` function in the `Transport` interface - `reset` function
+implementation in `AbstractTransporter` - `Gaussian Naive Bayes` declared as
+`GaussianNB` model - `Multinomial Naive Bayes` model declared as
+`MultinomialNB` model - `Complement Naive Bayes` model declared as
 `ComplementNB` model - `Bernoulli Naive Bayes` model declared as `BernoulliNB`
 model - `Categorical Naive Bayes` model declared as `CategoricalNB` model -
 Naive Bayes models test runner - Naive Bayes chain ### Changed - `Transport`
 function of `AbstractTransporter` updated - fix the order of `CFNode` fields
 serialization in `CFNodeTransporter` - `GeneralDataStructureTransporter`
 support list of ndarray with different shapes - Tests config modified - Naive
 Bayes params initialized in `pymilo_param` - Naive Bayes support added to
@@ -150,13 +159,14 @@
 - `GeneralDataStructure` Transporter updated - `LabelBinerizer` Transporter
 updated - `linear model` chain updated - GeneralDataStructure transporter
 enhanced - LabelBinerizer transporter updated - transporters' chain router
 added to `pymilo func` - NeuralNetwork params initialized in `pymilo_param` -
 `pymilo_test` updated to support multiple models - `linear_model_chain`
 refactored ## [0.1] - 2023-06-29 ### Added - scikit-learn linear models support
 - `Export` class - `Import` class [Unreleased]: https://github.com/openscilab/
-pymilo/compare/v0.6...dev [0.6]: https://github.com/openscilab/pymilo/compare/
-v0.5...v0.6 [0.5]: https://github.com/openscilab/pymilo/compare/v0.4...v0.5
-[0.4]: https://github.com/openscilab/pymilo/compare/v0.3...v0.4 [0.3]: https://
-github.com/openscilab/pymilo/compare/v0.2...v0.3 [0.2]: https://github.com/
-openscilab/pymilo/compare/v0.1...v0.2 [0.1]: https://github.com/openscilab/
-pymilo/compare/e887108...v0.1
+pymilo/compare/v0.7...dev [0.7]: https://github.com/openscilab/pymilo/compare/
+v0.6...v0.7 [0.6]: https://github.com/openscilab/pymilo/compare/v0.5...v0.6
+[0.5]: https://github.com/openscilab/pymilo/compare/v0.4...v0.5 [0.4]: https://
+github.com/openscilab/pymilo/compare/v0.3...v0.4 [0.3]: https://github.com/
+openscilab/pymilo/compare/v0.2...v0.3 [0.2]: https://github.com/openscilab/
+pymilo/compare/v0.1...v0.2 [0.1]: https://github.com/openscilab/pymilo/compare/
+e887108...v0.1
```

### Comparing `pymilo-0.6/pymilo.egg-info/SOURCES.txt` & `pymilo-0.7/pymilo.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 pymilo.egg-info/requires.txt
 pymilo.egg-info/top_level.txt
 pymilo/chains/__init__.py
 pymilo/chains/clustering_chain.py
 pymilo/chains/decision_tree_chain.py
 pymilo/chains/linear_model_chain.py
 pymilo/chains/naive_bayes_chain.py
+pymilo/chains/neighbours_chain.py
 pymilo/chains/neural_network_chain.py
 pymilo/chains/svm_chain.py
 pymilo/exceptions/__init__.py
 pymilo/exceptions/deserialize_exception.py
 pymilo/exceptions/pymilo_exception.py
 pymilo/exceptions/serialize_exception.py
 pymilo/transporters/__init__.py
@@ -27,14 +28,15 @@
 pymilo/transporters/baseloss_transporter.py
 pymilo/transporters/bisecting_tree_transporter.py
 pymilo/transporters/cfnode_transporter.py
 pymilo/transporters/function_transporter.py
 pymilo/transporters/general_data_structure_transporter.py
 pymilo/transporters/labelbinarizer_transporter.py
 pymilo/transporters/lossfunction_transporter.py
+pymilo/transporters/neighbors_tree_transporter.py
 pymilo/transporters/randomstate_transporter.py
 pymilo/transporters/sgdoptimizer_transporter.py
 pymilo/transporters/transporter.py
 pymilo/transporters/tree_transporter.py
 pymilo/utils/__init__.py
 pymilo/utils/data_exporter.py
 pymilo/utils/test_pymilo.py
```

### Comparing `pymilo-0.6/setup.py` & `pymilo-0.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,22 +30,22 @@
     name='pymilo',
     packages=[
         'pymilo',
         'pymilo.utils',
         'pymilo.chains',
         'pymilo.transporters',
         'pymilo.exceptions'],
-    version='0.6',
+    version='0.7',
     description='Transportation of ML models',
     long_description=read_description(),
     long_description_content_type='text/markdown',
     author='PyMilo Development Team',
     author_email='pymilo@openscilab.com',
     url='https://github.com/openscilab/pymilo',
-    download_url='https://github.com/openscilab/pymilo/tarball/v0.6',
+    download_url='https://github.com/openscilab/pymilo/tarball/v0.7',
     keywords="python3 python machine_learning ML",
     project_urls={
             'Source': 'https://github.com/openscilab/pymilo',
     },
     install_requires=get_requires(),
     python_requires='>=3.6',
     classifiers=[
```

