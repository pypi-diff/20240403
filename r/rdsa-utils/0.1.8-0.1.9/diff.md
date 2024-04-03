# Comparing `tmp/rdsa-utils-0.1.8.tar.gz` & `tmp/rdsa-utils-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdsa-utils-0.1.8.tar", last modified: Wed Feb 28 16:16:59 2024, max compression
+gzip compressed data, was "rdsa-utils-0.1.9.tar", last modified: Wed Apr  3 11:07:34 2024, max compression
```

## Comparing `rdsa-utils-0.1.8.tar` & `rdsa-utils-0.1.9.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:16:59.722688 rdsa-utils-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-02-28 16:16:45.000000 rdsa-utils-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-02-28 16:16:59.722688 rdsa-utils-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-02-28 16:16:45.000000 rdsa-utils-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-28 16:16:45.000000 rdsa-utils-0.1.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:16:59.714688 rdsa-utils-0.1.8/rdsa_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-28 16:16:45.000000 rdsa-utils-0.1.8/rdsa_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:16:59.718688 rdsa-utils-0.1.8/rdsa_utils/cdsw/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 16:16:45.000000 rdsa-utils-0.1.8/rdsa_utils/cdsw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:16:59.718688 rdsa-utils-0.1.8/rdsa_utils/cdsw/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 16:16:45.000000 rdsa-utils-0.1.8/rdsa_utils/cdsw/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10006 2024-02-28 16:16:45.000000 rdsa-utils-0.1.8/rdsa_utils/cdsw/helpers/hdfs_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-02-28 16:16:45.000000 rdsa-utils-0.1.8/rdsa_utils/cdsw/helpers/impala.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:16:59.718688 rdsa-utils-0.1.8/rdsa_utils/cdsw/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 16:16:45.000000 rdsa-utils-0.1.8/rdsa_utils/cdsw/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-02-28 16:16:45.000000 rdsa-utils-0.1.8/rdsa_utils/cdsw/io/input.py
--rw-r--r--   0 runner    (1001) docker     (127)    11310 2024-02-28 16:16:45.000000 rdsa-utils-0.1.8/rdsa_utils/cdsw/io/output.py
--rw-r--r--   0 runner    (1001) docker     (127)    10629 2024-02-28 16:16:45.000000 rdsa-utils-0.1.8/rdsa_utils/cdsw/io/pipeline_runlog.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-02-28 16:16:45.000000 rdsa-utils-0.1.8/rdsa_utils/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:16:59.718688 rdsa-utils-0.1.8/rdsa_utils/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 16:16:45.000000 rdsa-utils-0.1.8/rdsa_utils/gcp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:16:59.718688 rdsa-utils-0.1.8/rdsa_utils/gcp/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 16:16:45.000000 rdsa-utils-0.1.8/rdsa_utils/gcp/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-02-28 16:16:45.000000 rdsa-utils-0.1.8/rdsa_utils/gcp/helpers/gcp_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:16:59.718688 rdsa-utils-0.1.8/rdsa_utils/gcp/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 16:16:45.000000 rdsa-utils-0.1.8/rdsa_utils/gcp/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-02-28 16:16:45.000000 rdsa-utils-0.1.8/rdsa_utils/gcp/io/inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6397 2024-02-28 16:16:45.000000 rdsa-utils-0.1.8/rdsa_utils/gcp/io/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:16:59.718688 rdsa-utils-0.1.8/rdsa_utils/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 16:16:45.000000 rdsa-utils-0.1.8/rdsa_utils/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25205 2024-02-28 16:16:45.000000 rdsa-utils-0.1.8/rdsa_utils/helpers/pyspark.py
--rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-02-28 16:16:45.000000 rdsa-utils-0.1.8/rdsa_utils/helpers/python.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:16:59.718688 rdsa-utils-0.1.8/rdsa_utils/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 16:16:45.000000 rdsa-utils-0.1.8/rdsa_utils/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-02-28 16:16:45.000000 rdsa-utils-0.1.8/rdsa_utils/io/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-02-28 16:16:45.000000 rdsa-utils-0.1.8/rdsa_utils/io/input.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-28 16:16:45.000000 rdsa-utils-0.1.8/rdsa_utils/io/output.py
--rw-r--r--   0 runner    (1001) docker     (127)    18025 2024-02-28 16:16:45.000000 rdsa-utils-0.1.8/rdsa_utils/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:16:59.718688 rdsa-utils-0.1.8/rdsa_utils/methods/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 16:16:45.000000 rdsa-utils-0.1.8/rdsa_utils/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-02-28 16:16:45.000000 rdsa-utils-0.1.8/rdsa_utils/methods/averaging_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     5564 2024-02-28 16:16:45.000000 rdsa-utils-0.1.8/rdsa_utils/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-02-28 16:16:45.000000 rdsa-utils-0.1.8/rdsa_utils/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-02-28 16:16:45.000000 rdsa-utils-0.1.8/rdsa_utils/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:16:59.718688 rdsa-utils-0.1.8/rdsa_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-02-28 16:16:59.000000 rdsa-utils-0.1.8/rdsa_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-02-28 16:16:59.000000 rdsa-utils-0.1.8/rdsa_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 16:16:59.000000 rdsa-utils-0.1.8/rdsa_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-02-28 16:16:59.000000 rdsa-utils-0.1.8/rdsa_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-28 16:16:59.000000 rdsa-utils-0.1.8/rdsa_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-02-28 16:16:59.722688 rdsa-utils-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-28 16:16:45.000000 rdsa-utils-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:16:59.718688 rdsa-utils-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-02-28 16:16:45.000000 rdsa-utils-0.1.8/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-02-28 16:16:45.000000 rdsa-utils-0.1.8/tests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:34.168247 rdsa-utils-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-04-03 11:07:34.168247 rdsa-utils-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:34.160247 rdsa-utils-0.1.9/rdsa_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:34.160247 rdsa-utils-0.1.9/rdsa_utils/cdsw/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/cdsw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:34.164247 rdsa-utils-0.1.9/rdsa_utils/cdsw/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/cdsw/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11636 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/cdsw/helpers/hdfs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/cdsw/helpers/impala.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:34.164247 rdsa-utils-0.1.9/rdsa_utils/cdsw/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/cdsw/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/cdsw/io/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10022 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/cdsw/io/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10629 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/cdsw/io/pipeline_runlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:34.164247 rdsa-utils-0.1.9/rdsa_utils/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/gcp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:34.164247 rdsa-utils-0.1.9/rdsa_utils/gcp/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/gcp/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/gcp/helpers/gcp_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:34.164247 rdsa-utils-0.1.9/rdsa_utils/gcp/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/gcp/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/gcp/io/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6397 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/gcp/io/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:34.164247 rdsa-utils-0.1.9/rdsa_utils/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25083 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/helpers/pyspark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/helpers/python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:34.164247 rdsa-utils-0.1.9/rdsa_utils/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/io/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/io/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/io/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18025 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:34.164247 rdsa-utils-0.1.9/rdsa_utils/methods/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/methods/averaging_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5564 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:34.168247 rdsa-utils-0.1.9/rdsa_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-04-03 11:07:34.000000 rdsa-utils-0.1.9/rdsa_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-03 11:07:34.000000 rdsa-utils-0.1.9/rdsa_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 11:07:34.000000 rdsa-utils-0.1.9/rdsa_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-03 11:07:34.000000 rdsa-utils-0.1.9/rdsa_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 11:07:34.000000 rdsa-utils-0.1.9/rdsa_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-03 11:07:34.168247 rdsa-utils-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:34.164247 rdsa-utils-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/tests/test_validation.py
```

### Comparing `rdsa-utils-0.1.8/LICENSE` & `rdsa-utils-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rdsa-utils-0.1.8/PKG-INFO` & `rdsa-utils-0.1.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,67 +1,79 @@
 Metadata-Version: 2.1
 Name: rdsa-utils
-Version: 0.1.8
-Summary: A suite of pyspark, pandas and general pipeline utils for Reproducible Data Science and Analysis projects.
+Version: 0.1.9
+Summary: A suite of PySpark, Pandas, and general pipeline utils for Reproducible Data Science and Analysis (RDSA) projects.
 Home-page: https://github.com/ONSdigital/rdsa-utils
 Author: Reproducible Data Science & Analysis, ONS
 Author-email: Diego.Lara.De.Andres@ons.gov.uk, Meg.Scammell@ons.gov.uk, Dominic.Bean@ons.gov.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: <3.11,>=3.8
+Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cloudpathlib[gs]>=0.15.1
 Requires-Dist: humanfriendly>=9.1
 Requires-Dist: more-itertools>=9.0.0
 Requires-Dist: pandas==1.5.3
-Requires-Dist: pydantic==2.0
-Requires-Dist: pyspark==3.3.1
+Requires-Dist: pydantic>=2.6.2
 Requires-Dist: pyyaml>=6.0.1
 Requires-Dist: tomli>=2.0.1
-Requires-Dist: google-cloud-bigquery==3.3.5
-Requires-Dist: google-cloud-storage==2.5.0
+Requires-Dist: google-cloud-bigquery>=3.17.2
+Requires-Dist: google-cloud-storage>=2.14.0
 Provides-Extra: dev
 Requires-Dist: bump2version>=1.0.0; extra == "dev"
 Requires-Dist: pre-commit>=2.6.0; extra == "dev"
 Requires-Dist: ruff>=0.0.270; extra == "dev"
 Requires-Dist: chispa>=0.9.2; extra == "dev"
 Requires-Dist: coverage[toml]>=7.1.0; extra == "dev"
 Requires-Dist: pytest<8.0.0,>=7.1.0; extra == "dev"
 Requires-Dist: pytest-cov>=4.0.0; extra == "dev"
 Requires-Dist: pytest-lazy-fixture>=0.6.0; extra == "dev"
 Requires-Dist: pytest-mock>=3.8.0; extra == "dev"
+Requires-Dist: pyspark==3.5.1; extra == "dev"
 Provides-Extra: doc
 Requires-Dist: mkdocs>=1.4.2; extra == "doc"
 Requires-Dist: mkdocs-tech-docs-template>=0.1.2; extra == "doc"
 Requires-Dist: mkdocstrings[python]>=0.22.0; extra == "doc"
 Requires-Dist: mkdocs-git-revision-date-localized-plugin>=1.2.1; extra == "doc"
 Requires-Dist: mkdocs-jupyter>=0.24.3; extra == "doc"
+Requires-Dist: mkdocs-mermaid2-plugin>=1.1.1; extra == "doc"
 
-# rdsa-utils
+# 🧰 rdsa-utils 
 
-A suite of pyspark, pandas and general pipeline utils for **Reproducible Data Science and Analysis (RDSA)** projects.
+A suite of PySpark, Pandas, and general pipeline utils for **Reproducible Data Science and Analysis (RDSA)** projects.
 
-The RDSA team sits within the Economic Statistics Change Directorate, and uses cutting-edge data science and engineering skills to produce the next generation of economic statistics. Current priorities include overhauling legacy systems and developing new systems for key statistics.
+The RDSA team sits within the Economic Statistics Change Directorate, and uses cutting-edge data science and engineering skills to produce the next generation of economic statistics. Current priorities include overhauling legacy systems and developing new systems for key statistics. More information about work at RDSA can be found here: [Using Data Science for Next-Gen Statistics](https://dataingovernment.blog.gov.uk/2023/02/14/using-data-science-for-next-gen-statistics/).
 
-`rdsa-utils` is a Python codebase built with Python 3.8 and higher, and uses `setup.py` for dependency management and packaging.
+`rdsa-utils` is a Python codebase built with Python 3.8 and higher, and uses `setup.py`, `setup.cfg`, and `pyproject.toml` for dependency management and packaging.
 
-## Prerequisites
+## 📋 Prerequisites 
 
 - Python 3.8 or higher
 
-## Documentation and Further Information
+## 💾 Installation 
+
+`rdsa-utils` is available for installation via [PyPI](https://pypi.org/project/rdsa-utils/) and can also be found on [GitHub Releases](https://github.com/ONSdigital/rdsa-utils/releases) for direct downloads and version history.
+
+To install via `pip`, simply run:
+
+```bash
+pip install rdsa-utils
+```
+
+## 📖 Documentation and Further Information 
 
 Our documentation is automatically generated using **GitHub Actions** and **MkDocs**. For an in-depth understanding of `rdsa-utils`, how to contribute to `rdsa-utils`, and more, please refer to our [MkDocs-generated documentation](https://onsdigital.github.io/rdsa-utils/).
 
-## Licence
+## 🛡️ Licence
 
 Unless stated otherwise, the codebase is released under the [MIT License][mit].
 This covers both the codebase and any sample code in the documentation.
 
 The documentation is [© Crown copyright][copyright] and available under the terms of the [Open Government 3.0][ogl] licence.
 
 [mit]: LICENSE
```

### Comparing `rdsa-utils-0.1.8/README.md` & `rdsa-utils-0.1.9/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,34 @@
-# rdsa-utils
+# 🧰 rdsa-utils 
 
-A suite of pyspark, pandas and general pipeline utils for **Reproducible Data Science and Analysis (RDSA)** projects.
+A suite of PySpark, Pandas, and general pipeline utils for **Reproducible Data Science and Analysis (RDSA)** projects.
 
-The RDSA team sits within the Economic Statistics Change Directorate, and uses cutting-edge data science and engineering skills to produce the next generation of economic statistics. Current priorities include overhauling legacy systems and developing new systems for key statistics.
+The RDSA team sits within the Economic Statistics Change Directorate, and uses cutting-edge data science and engineering skills to produce the next generation of economic statistics. Current priorities include overhauling legacy systems and developing new systems for key statistics. More information about work at RDSA can be found here: [Using Data Science for Next-Gen Statistics](https://dataingovernment.blog.gov.uk/2023/02/14/using-data-science-for-next-gen-statistics/).
 
-`rdsa-utils` is a Python codebase built with Python 3.8 and higher, and uses `setup.py` for dependency management and packaging.
+`rdsa-utils` is a Python codebase built with Python 3.8 and higher, and uses `setup.py`, `setup.cfg`, and `pyproject.toml` for dependency management and packaging.
 
-## Prerequisites
+## 📋 Prerequisites 
 
 - Python 3.8 or higher
 
-## Documentation and Further Information
+## 💾 Installation 
+
+`rdsa-utils` is available for installation via [PyPI](https://pypi.org/project/rdsa-utils/) and can also be found on [GitHub Releases](https://github.com/ONSdigital/rdsa-utils/releases) for direct downloads and version history.
+
+To install via `pip`, simply run:
+
+```bash
+pip install rdsa-utils
+```
+
+## 📖 Documentation and Further Information 
 
 Our documentation is automatically generated using **GitHub Actions** and **MkDocs**. For an in-depth understanding of `rdsa-utils`, how to contribute to `rdsa-utils`, and more, please refer to our [MkDocs-generated documentation](https://onsdigital.github.io/rdsa-utils/).
 
-## Licence
+## 🛡️ Licence
 
 Unless stated otherwise, the codebase is released under the [MIT License][mit].
 This covers both the codebase and any sample code in the documentation.
 
 The documentation is [© Crown copyright][copyright] and available under the terms of the [Open Government 3.0][ogl] licence.
 
 [mit]: LICENSE
```

### Comparing `rdsa-utils-0.1.8/rdsa_utils/cdsw/helpers/hdfs_utils.py` & `rdsa-utils-0.1.9/rdsa_utils/cdsw/helpers/hdfs_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -183,33 +183,46 @@
     subprocess.call(
         [f'echo "{string_to_write}" | hadoop fs -put - {path}'],
         shell=True,
     )
 
 
 def delete_dir(path: str) -> bool:
-    """Delete a directory from HDFS.
+    """Delete an empty directory from HDFS.
+
+    This function attempts to delete an empty directory in HDFS.
+    If the directory is not empty, the deletion will fail.
 
     Parameters
     ----------
     path
         The HDFS path to the directory to be deleted.
 
     Returns
     -------
     bool
         True if the operation is successful (directory deleted),
         otherwise False.
+
+    Note
+    ----
+    This function will only succeed if the directory is empty.
+    To delete directories containing files or other directories,
+    consider using `delete_path` instead.
     """
     command = ['hadoop', 'fs', '-rmdir', path]
     return _perform(command)
 
 
 def delete_file(path: str) -> bool:
-    """Delete a file in HDFS.
+    """Delete a specific file in HDFS.
+
+    This function is used to delete a single file located
+    at the specified HDFS path. If the path points to a
+    directory, the command will fail.
 
     Parameters
     ----------
     path
         The path to the file in HDFS to be deleted.
 
     Returns
@@ -218,19 +231,57 @@
         True if the file was successfully deleted (command return code 0),
         otherwise False.
 
     Raises
     ------
     subprocess.TimeoutExpired
         If the process does not complete within the default timeout.
+
+    Note
+    ----
+    This function is intended for files only. For directory deletions,
+    use `delete_dir` or `delete_path`.
     """
     command = ['hadoop', 'fs', '-rm', path]
     return _perform(command)
 
 
+def delete_path(path: str) -> bool:
+    """Delete a file or directory in HDFS, including non-empty directories.
+
+    This function is capable of deleting both files and directories.
+    When applied to directories, it will recursively delete all contents
+    within the directory, making it suitable for removing directories regardless
+    of whether they are empty or contain files or other directories.
+
+    Parameters
+    ----------
+    path
+        The path to the file or directory in HDFS to be deleted.
+
+    Returns
+    -------
+    bool
+        True if the file was successfully deleted (command return code 0),
+        otherwise False.
+
+    Raises
+    ------
+    subprocess.TimeoutExpired
+        If the process does not complete within the default timeout.
+
+    Warning
+    -------
+    Use with caution: applying this function to a directory will
+    remove all contained files and subdirectories without confirmation.
+    """
+    command = ['hadoop', 'fs', '-rm', '-r', path]
+    return _perform(command)
+
+
 def file_exists(path: str) -> bool:
     """Check whether a file exists in HDFS.
 
     Parameters
     ----------
     path
         The path to the file in HDFS to be checked for existence.
@@ -266,15 +317,15 @@
         f'hadoop fs -stat %y {filepath}',
         stdout=subprocess.PIPE,
         shell=True,
     )
     return command.stdout.read().decode('utf-8')[0:10]
 
 
-def isdir(path: str) -> bool:
+def is_dir(path: str) -> bool:
     """Test if a directory exists in HDFS.
 
     Parameters
     ----------
     path
         The HDFS path to the directory to be tested.
```

### Comparing `rdsa-utils-0.1.8/rdsa_utils/cdsw/helpers/impala.py` & `rdsa-utils-0.1.9/rdsa_utils/cdsw/helpers/impala.py`

 * *Files identical despite different names*

### Comparing `rdsa-utils-0.1.8/rdsa_utils/cdsw/io/input.py` & `rdsa-utils-0.1.9/rdsa_utils/cdsw/io/input.py`

 * *Files identical despite different names*

### Comparing `rdsa-utils-0.1.8/rdsa_utils/cdsw/io/output.py` & `rdsa-utils-0.1.9/rdsa_utils/cdsw/io/output.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 import logging
 from typing import Union
 
 from pyspark.sql import DataFrame as SparkDF
 from pyspark.sql import SparkSession
 from pyspark.sql import functions as F
 from pyspark.sql.utils import AnalysisException
-from py4j.java_gateway import java_import
 
+from rdsa_utils.cdsw.helpers.hdfs_utils import delete_path, file_exists, rename
+from rdsa_utils.cdsw.io.input import load_and_validate_table
 from rdsa_utils.exceptions import (
     ColumnNotInDataframeError,
     DataframeEmptyError,
     TableNotFoundError,
 )
 from rdsa_utils.helpers.pyspark import is_df_empty
-from rdsa_utils.cdsw.io.input import load_and_validate_table
 
 logger = logging.getLogger(__name__)
 
 
 def insert_df_to_hive_table(
     spark: SparkSession,
     df: SparkDF,
@@ -205,144 +205,106 @@
 
     except Exception as e:
         logger.error(f'An error occurred: {e}')
         raise
 
 
 def save_csv_to_hdfs(
-    spark: SparkSession,
     df: SparkDF,
     file_name: str,
     file_path: str,
     overwrite: bool = True,
-    coalesce_data: bool = True,
 ) -> None:
-    """Save DataFrame as CSV on HDFS, with optional coalescing.
-
-    This function saves a PySpark DataFrame to HDFS in CSV format.
-    Coalescing the DataFrame into a single partition is optional.
+    """Save DataFrame as CSV on HDFS, coalescing to a single partition.
 
-    Without coalescing, the DataFrame is saved in multiple parts, and
-    these parts are merged into a single file. However, this does not
-    guarantee the order of rows as in the original DataFrame.
+    This function saves a PySpark DataFrame to HDFS in CSV format. By
+    coalescing the DataFrame into a single partition before saving, it
+    accomplishes two main objectives:
+
+    1. Single Part File: The output is a single CSV file rather than
+       multiple part files. This method reduces complexity and
+       cuts through the clutter of multi-part files, offering users
+       and systems a more cohesive and hassle-free experience.
+
+    2. Preserving Row Order: Coalescing into a single partition maintains
+       the order of rows as they appear in the DataFrame. This is essential
+       when the row order matters for subsequent processing or analysis.
+       It's important to note, however, that coalescing can have performance
+       implications for very large DataFrames by concentrating
+       all data processing on a single node.
 
     Parameters
     ----------
-    spark
-        Active SparkSession instance.
     df
-        PySpark DataFrame to save.
+        PySpark DataFrame to be saved.
     file_name
-        The name of the CSV file. The file name must include
-        the ".csv" extension.
+        Name of the CSV file. Must include the ".csv" extension.
     file_path
-        The path in HDFS where the CSV file should be saved.
+        HDFS path where the CSV file should be saved.
     overwrite
-        If True, any existing file with the same name in the
-        given path will be overwritten.
-        If False, an exception will be raised if a file with
-        the same name already exists.
-    coalesce_data
-        If True, coalesces the DataFrame into a single partition
-        before saving. This preserves the order of rows but may
-        impact performance for large DataFrames.
+        If True, overwrite any existing file with the same name. If False
+        and the file exists, the function will raise an error.
 
     Raises
     ------
     ValueError
-        If the provided file_name doesn't end with ".csv".
+        If the file_name does not end with ".csv".
     IOError
-        If `overwrite` is False and the file already exists.
+        If overwrite is False and the target file already exists.
 
     Examples
     --------
-    >>> save_to_hdfs_csv(df, "example.csv", "/user/hadoop/data/")
+    Saving to an S3 bucket using the `s3a://` scheme:
+
+    ```python
+    # Assume `df` is a pre-defined PySpark DataFrame
+    file_name = "data_output.csv"
+    file_path = "s3a://my-bucket/data_folder/"
+    save_csv_to_hdfs(df, file_name, file_path, overwrite=True)
+    ```
+
+    Saving to a normal HDFS path:
+
+    ```python
+    # Assume `df` is a pre-defined PySpark DataFrame
+    file_name = "data_output.csv"
+    file_path = "/user/hdfs/data_folder/"
+    save_csv_to_hdfs(df, file_name, file_path, overwrite=True)
+    ```
     """
     if not file_name.endswith('.csv'):
-        msg = "The file_name must end with '.csv' extension."
-        raise ValueError(msg)
+        error_msg = "The file_name must end with '.csv' extension."
+        raise ValueError(error_msg)
 
     destination_path = f"{file_path.rstrip('/')}/{file_name}"
 
-    # Access Hadoop FileSystem
-    java_import(spark._jvm, 'org.apache.hadoop.fs.FileSystem')
-    java_import(spark._jvm, 'org.apache.hadoop.fs.Path')
-    java_import(spark._jvm, 'org.apache.hadoop.io.IOUtils')
-    fs = spark._jvm.org.apache.hadoop.fs.FileSystem.get(
-        spark._jsc.hadoopConfiguration(),
-    )
-
-    if not overwrite and fs.exists(spark._jvm.Path(destination_path)):
-        msg = (
+    if not overwrite and file_exists(destination_path):
+        error_msg = (
             f"File '{destination_path}' already exists "
             "and overwrite is set to False."
         )
-        raise IOError(
-            msg,
-        )
+        raise IOError(error_msg)
 
     logger.info(f'Saving DataFrame to {file_name} in HDFS at {file_path}')
 
-    # Coalesce the DataFrame to a single partition if required
-    if coalesce_data:
-        df = df.coalesce(1)
+    # Coalesce the DataFrame to a single partition
+    df = df.coalesce(1)
 
-    # Temporary directory for saving the data
-    temp_path = f"{file_path.rstrip('/')}/{file_name}_temp"
+    # Temporary path for saving the single part file
+    temp_path = f"{file_path.rstrip('/')}/temp_{file_name}"
 
-    # Save the DataFrame to HDFS in CSV format
+    # Save the DataFrame to HDFS in CSV format in a temporary directory
     df.write.csv(temp_path, header=True, mode='overwrite')
-    logger.info(f'DataFrame saved temporarily at {temp_path}')
 
-    # HDFS Path objects for source and destination
-    destination_file_path = spark._jvm.Path(destination_path)
-    temp_dir_path = spark._jvm.Path(temp_path)
-
-    # Open the merged file for writing
-    merged_file_path = spark._jvm.Path(temp_path + '/merged.csv')
-    merged_file = fs.create(merged_file_path)
+    # Identify the part file: pattern matching for the single part file
+    part_file = f'{temp_path}/part-00000*.csv'
 
-    try:
-        first_file = True
-        for file_status in fs.listStatus(temp_dir_path):
-            file_name = file_status.getPath().getName()
-            if file_name.startswith('part-'):
-                part_file = fs.open(file_status.getPath())
-                try:
-                    # Skip header for non-first files
-                    if not first_file:
-                        part_file.readLine()
-                    else:
-                        first_file = False
-                    spark._jvm.org.apache.hadoop.io.IOUtils.copyBytes(
-                        part_file,
-                        merged_file,
-                        spark._jsc.hadoopConfiguration(),
-                        False,
-                    )
-                finally:
-                    part_file.close()
-    finally:
-        merged_file.close()
-
-    # Check if the destination file already exists and delete if necessary
-    if fs.exists(destination_file_path):
-        if not fs.delete(destination_file_path, False):
-            logger.error(
-                f'Failed to delete existing file at {destination_path}',
-            )
-            msg = f'Could not delete existing file at {destination_path}'
-            raise IOError(
-                msg,
-            )
+    # Rename the part file to the final file name
+    if not rename(part_file, destination_path, overwrite):
+        error_msg = f"Failed to rename the part file to '{destination_path}'"
+        raise IOError(error_msg)
 
-    # Rename merged file to final destination
-    if not fs.rename(merged_file_path, destination_file_path):
-        logger.error(f'Failed to rename file to {destination_path}')
-        msg = f'Could not rename file to {destination_path}'
-        raise IOError(msg)
-    else:
-        logger.info(f'Renamed the file to {file_name}')
+    logger.info(f'DataFrame successfully saved to {destination_path}')
 
-    # Clean up temporary directory
-    fs.delete(spark._jvm.Path(temp_path), True)
+    # Clean up the temporary directory
+    delete_path(temp_path)
     logger.info(f'Temporary directory {temp_path} deleted')
```

### Comparing `rdsa-utils-0.1.8/rdsa_utils/cdsw/io/pipeline_runlog.py` & `rdsa-utils-0.1.9/rdsa_utils/cdsw/io/pipeline_runlog.py`

 * *Files identical despite different names*

### Comparing `rdsa-utils-0.1.8/rdsa_utils/exceptions.py` & `rdsa-utils-0.1.9/rdsa_utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `rdsa-utils-0.1.8/rdsa_utils/gcp/helpers/gcp_utils.py` & `rdsa-utils-0.1.9/rdsa_utils/gcp/helpers/gcp_utils.py`

 * *Files identical despite different names*

### Comparing `rdsa-utils-0.1.8/rdsa_utils/gcp/io/inputs.py` & `rdsa-utils-0.1.9/rdsa_utils/gcp/io/inputs.py`

 * *Files identical despite different names*

### Comparing `rdsa-utils-0.1.8/rdsa_utils/gcp/io/outputs.py` & `rdsa-utils-0.1.9/rdsa_utils/gcp/io/outputs.py`

 * *Files identical despite different names*

### Comparing `rdsa-utils-0.1.8/rdsa_utils/helpers/pyspark.py` & `rdsa-utils-0.1.9/rdsa_utils/helpers/pyspark.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,15 @@
 
 from pyspark.sql import Column as SparkCol
 from pyspark.sql import DataFrame as SparkDF
 from pyspark.sql import SparkSession, Window, WindowSpec
 from pyspark.sql import functions as F
 from pyspark.sql import types as T
 
-from rdsa_utils.logging import (
-    log_spark_df_schema,
-)
+from rdsa_utils.logging import log_spark_df_schema
 
 logger = logging.getLogger(__name__)
 
 
 def create_colname_to_value_map(cols: Sequence[str]) -> SparkCol:
     """Create a column name to value MapType column."""
     colname_value_tups = [(F.lit(name), F.col(name)) for name in cols]
@@ -740,17 +738,14 @@
 
         logger.info(
             f"Creating a '{size}' Spark session..."
             if size
             else 'Creating a basic Spark session...',
         )
 
-        logger.info('Stopping any existing Spark session...')
-        SparkSession.builder.getOrCreate().stop()
-
         if app_name:
             builder = SparkSession.builder.appName(f'{app_name}')
         else:
             builder = SparkSession.builder
 
         # fmt: off
         if size == 'small':
```

### Comparing `rdsa-utils-0.1.8/rdsa_utils/helpers/python.py` & `rdsa-utils-0.1.9/rdsa_utils/helpers/python.py`

 * *Files identical despite different names*

### Comparing `rdsa-utils-0.1.8/rdsa_utils/io/config.py` & `rdsa-utils-0.1.9/rdsa_utils/io/config.py`

 * *Files identical despite different names*

### Comparing `rdsa-utils-0.1.8/rdsa_utils/io/input.py` & `rdsa-utils-0.1.9/rdsa_utils/io/input.py`

 * *Files identical despite different names*

### Comparing `rdsa-utils-0.1.8/rdsa_utils/logging.py` & `rdsa-utils-0.1.9/rdsa_utils/logging.py`

 * *Files identical despite different names*

### Comparing `rdsa-utils-0.1.8/rdsa_utils/methods/averaging_methods.py` & `rdsa-utils-0.1.9/rdsa_utils/methods/averaging_methods.py`

 * *Files identical despite different names*

### Comparing `rdsa-utils-0.1.8/rdsa_utils/test_utils.py` & `rdsa-utils-0.1.9/rdsa_utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `rdsa-utils-0.1.8/rdsa_utils/typing.py` & `rdsa-utils-0.1.9/rdsa_utils/typing.py`

 * *Files identical despite different names*

### Comparing `rdsa-utils-0.1.8/rdsa_utils/validation.py` & `rdsa-utils-0.1.9/rdsa_utils/validation.py`

 * *Files identical despite different names*

### Comparing `rdsa-utils-0.1.8/rdsa_utils.egg-info/PKG-INFO` & `rdsa-utils-0.1.9/rdsa_utils.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,67 +1,79 @@
 Metadata-Version: 2.1
 Name: rdsa-utils
-Version: 0.1.8
-Summary: A suite of pyspark, pandas and general pipeline utils for Reproducible Data Science and Analysis projects.
+Version: 0.1.9
+Summary: A suite of PySpark, Pandas, and general pipeline utils for Reproducible Data Science and Analysis (RDSA) projects.
 Home-page: https://github.com/ONSdigital/rdsa-utils
 Author: Reproducible Data Science & Analysis, ONS
 Author-email: Diego.Lara.De.Andres@ons.gov.uk, Meg.Scammell@ons.gov.uk, Dominic.Bean@ons.gov.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: <3.11,>=3.8
+Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cloudpathlib[gs]>=0.15.1
 Requires-Dist: humanfriendly>=9.1
 Requires-Dist: more-itertools>=9.0.0
 Requires-Dist: pandas==1.5.3
-Requires-Dist: pydantic==2.0
-Requires-Dist: pyspark==3.3.1
+Requires-Dist: pydantic>=2.6.2
 Requires-Dist: pyyaml>=6.0.1
 Requires-Dist: tomli>=2.0.1
-Requires-Dist: google-cloud-bigquery==3.3.5
-Requires-Dist: google-cloud-storage==2.5.0
+Requires-Dist: google-cloud-bigquery>=3.17.2
+Requires-Dist: google-cloud-storage>=2.14.0
 Provides-Extra: dev
 Requires-Dist: bump2version>=1.0.0; extra == "dev"
 Requires-Dist: pre-commit>=2.6.0; extra == "dev"
 Requires-Dist: ruff>=0.0.270; extra == "dev"
 Requires-Dist: chispa>=0.9.2; extra == "dev"
 Requires-Dist: coverage[toml]>=7.1.0; extra == "dev"
 Requires-Dist: pytest<8.0.0,>=7.1.0; extra == "dev"
 Requires-Dist: pytest-cov>=4.0.0; extra == "dev"
 Requires-Dist: pytest-lazy-fixture>=0.6.0; extra == "dev"
 Requires-Dist: pytest-mock>=3.8.0; extra == "dev"
+Requires-Dist: pyspark==3.5.1; extra == "dev"
 Provides-Extra: doc
 Requires-Dist: mkdocs>=1.4.2; extra == "doc"
 Requires-Dist: mkdocs-tech-docs-template>=0.1.2; extra == "doc"
 Requires-Dist: mkdocstrings[python]>=0.22.0; extra == "doc"
 Requires-Dist: mkdocs-git-revision-date-localized-plugin>=1.2.1; extra == "doc"
 Requires-Dist: mkdocs-jupyter>=0.24.3; extra == "doc"
+Requires-Dist: mkdocs-mermaid2-plugin>=1.1.1; extra == "doc"
 
-# rdsa-utils
+# 🧰 rdsa-utils 
 
-A suite of pyspark, pandas and general pipeline utils for **Reproducible Data Science and Analysis (RDSA)** projects.
+A suite of PySpark, Pandas, and general pipeline utils for **Reproducible Data Science and Analysis (RDSA)** projects.
 
-The RDSA team sits within the Economic Statistics Change Directorate, and uses cutting-edge data science and engineering skills to produce the next generation of economic statistics. Current priorities include overhauling legacy systems and developing new systems for key statistics.
+The RDSA team sits within the Economic Statistics Change Directorate, and uses cutting-edge data science and engineering skills to produce the next generation of economic statistics. Current priorities include overhauling legacy systems and developing new systems for key statistics. More information about work at RDSA can be found here: [Using Data Science for Next-Gen Statistics](https://dataingovernment.blog.gov.uk/2023/02/14/using-data-science-for-next-gen-statistics/).
 
-`rdsa-utils` is a Python codebase built with Python 3.8 and higher, and uses `setup.py` for dependency management and packaging.
+`rdsa-utils` is a Python codebase built with Python 3.8 and higher, and uses `setup.py`, `setup.cfg`, and `pyproject.toml` for dependency management and packaging.
 
-## Prerequisites
+## 📋 Prerequisites 
 
 - Python 3.8 or higher
 
-## Documentation and Further Information
+## 💾 Installation 
+
+`rdsa-utils` is available for installation via [PyPI](https://pypi.org/project/rdsa-utils/) and can also be found on [GitHub Releases](https://github.com/ONSdigital/rdsa-utils/releases) for direct downloads and version history.
+
+To install via `pip`, simply run:
+
+```bash
+pip install rdsa-utils
+```
+
+## 📖 Documentation and Further Information 
 
 Our documentation is automatically generated using **GitHub Actions** and **MkDocs**. For an in-depth understanding of `rdsa-utils`, how to contribute to `rdsa-utils`, and more, please refer to our [MkDocs-generated documentation](https://onsdigital.github.io/rdsa-utils/).
 
-## Licence
+## 🛡️ Licence
 
 Unless stated otherwise, the codebase is released under the [MIT License][mit].
 This covers both the codebase and any sample code in the documentation.
 
 The documentation is [© Crown copyright][copyright] and available under the terms of the [Open Government 3.0][ogl] licence.
 
 [mit]: LICENSE
```

### Comparing `rdsa-utils-0.1.8/rdsa_utils.egg-info/SOURCES.txt` & `rdsa-utils-0.1.9/rdsa_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rdsa-utils-0.1.8/rdsa_utils.egg-info/requires.txt` & `rdsa-utils-0.1.9/rdsa_utils.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 cloudpathlib[gs]>=0.15.1
 humanfriendly>=9.1
 more-itertools>=9.0.0
 pandas==1.5.3
-pydantic==2.0
-pyspark==3.3.1
+pydantic>=2.6.2
 pyyaml>=6.0.1
 tomli>=2.0.1
-google-cloud-bigquery==3.3.5
-google-cloud-storage==2.5.0
+google-cloud-bigquery>=3.17.2
+google-cloud-storage>=2.14.0
 
 [dev]
 bump2version>=1.0.0
 pre-commit>=2.6.0
 ruff>=0.0.270
 chispa>=0.9.2
 coverage[toml]>=7.1.0
 pytest<8.0.0,>=7.1.0
 pytest-cov>=4.0.0
 pytest-lazy-fixture>=0.6.0
 pytest-mock>=3.8.0
+pyspark==3.5.1
 
 [doc]
 mkdocs>=1.4.2
 mkdocs-tech-docs-template>=0.1.2
 mkdocstrings[python]>=0.22.0
 mkdocs-git-revision-date-localized-plugin>=1.2.1
 mkdocs-jupyter>=0.24.3
+mkdocs-mermaid2-plugin>=1.1.1
```

### Comparing `rdsa-utils-0.1.8/setup.cfg` & `rdsa-utils-0.1.9/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,58 +1,60 @@
 [metadata]
 name = rdsa-utils
 version = attr: rdsa_utils.__version__
 author = Reproducible Data Science & Analysis, ONS
 author_email = Diego.Lara.De.Andres@ons.gov.uk, Meg.Scammell@ons.gov.uk, Dominic.Bean@ons.gov.uk
-description = A suite of pyspark, pandas and general pipeline utils for Reproducible Data Science and Analysis projects.
+description = A suite of PySpark, Pandas, and general pipeline utils for Reproducible Data Science and Analysis (RDSA) projects.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ONSdigital/rdsa-utils
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 packages = find:
-python_requires = >=3.8, <3.11
+python_requires = >=3.8, <3.12
 install_requires = 
 	cloudpathlib[gs]>=0.15.1
 	humanfriendly>=9.1
 	more-itertools>=9.0.0
 	pandas==1.5.3
-	pydantic==2.0
-	pyspark==3.3.1
+	pydantic>=2.6.2
 	pyyaml>=6.0.1
 	tomli>=2.0.1
-	google-cloud-bigquery==3.3.5
-	google-cloud-storage==2.5.0
+	google-cloud-bigquery>=3.17.2
+	google-cloud-storage>=2.14.0
 
 [options.packages.find]
 where = .
 include = rdsa_utils*
 
 [options.extras_require]
 dev = 
 	bump2version>=1.0.0
 	pre-commit>=2.6.0
 	ruff>=0.0.270
 	chispa>=0.9.2
 	coverage[toml]>=7.1.0
-	pytest>=7.1.0, <8.0.0  # Temporarily pin pytest due to compatibility issues
+	pytest>=7.1.0, <8.0.0  # Temporarily pin pytest due to https://github.com/TvoroG/pytest-lazy-fixture/issues/65
 	pytest-cov>=4.0.0
 	pytest-lazy-fixture>=0.6.0
 	pytest-mock>=3.8.0
+	pyspark==3.5.1
 doc = 
 	mkdocs>=1.4.2
 	mkdocs-tech-docs-template>=0.1.2
 	mkdocstrings[python]>=0.22.0
 	mkdocs-git-revision-date-localized-plugin>=1.2.1
 	mkdocs-jupyter>=0.24.3
+	mkdocs-mermaid2-plugin>=1.1.1
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `rdsa-utils-0.1.8/tests/test_logging.py` & `rdsa-utils-0.1.9/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `rdsa-utils-0.1.8/tests/test_validation.py` & `rdsa-utils-0.1.9/tests/test_validation.py`

 * *Files identical despite different names*

