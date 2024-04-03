# Comparing `tmp/fameio-1.8.2.tar.gz` & `tmp/fameio-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fameio-1.8.2.tar", last modified: Fri Mar 22 07:28:36 2024, max compression
+gzip compressed data, was "fameio-2.0.0.tar", max compression
```

## Comparing `fameio-1.8.2.tar` & `fameio-2.0.0.tar`

### file list

```diff
@@ -1,63 +1,52 @@
-drwxrwxrwx   0        0        0        0 2024-03-22 07:28:36.102702 fameio-1.8.2/
--rw-rw-rw-   0        0        0    10391 2024-02-14 11:04:50.000000 fameio-1.8.2/LICENSE.txt
--rw-rw-rw-   0        0        0    30291 2024-03-22 07:28:36.086999 fameio-1.8.2/PKG-INFO
--rw-rw-rw-   0        0        0    29433 2024-03-22 07:20:44.000000 fameio-1.8.2/README.md
--rw-rw-rw-   0        0        0       42 2024-03-22 07:28:36.102702 fameio-1.8.2/setup.cfg
--rw-rw-rw-   0        0        0     1762 2024-03-22 07:21:15.000000 fameio-1.8.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-22 07:28:36.037377 fameio-1.8.2/src/
-drwxrwxrwx   0        0        0        0 2024-03-22 07:28:36.053090 fameio-1.8.2/src/fameio/
--rw-rw-rw-   0        0        0      109 2024-02-14 11:04:50.000000 fameio-1.8.2/src/fameio/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-22 07:28:36.068706 fameio-1.8.2/src/fameio/scripts/
--rw-rw-rw-   0        0        0      746 2024-03-22 07:20:44.000000 fameio-1.8.2/src/fameio/scripts/__init__.py
--rw-rw-rw-   0        0        0     3296 2024-03-22 07:20:44.000000 fameio-1.8.2/src/fameio/scripts/convert_results.py
--rw-rw-rw-   0        0        0     1339 2024-03-22 07:20:44.000000 fameio-1.8.2/src/fameio/scripts/make_config.py
-drwxrwxrwx   0        0        0        0 2024-03-22 07:28:36.068706 fameio-1.8.2/src/fameio/source/
--rw-rw-rw-   0        0        0      278 2024-02-14 11:04:50.000000 fameio-1.8.2/src/fameio/source/__init__.py
--rw-rw-rw-   0        0        0     9384 2024-03-22 07:20:44.000000 fameio-1.8.2/src/fameio/source/cli.py
--rw-rw-rw-   0        0        0     7403 2024-03-22 07:20:44.000000 fameio-1.8.2/src/fameio/source/loader.py
--rw-rw-rw-   0        0        0     1929 2024-03-22 07:20:44.000000 fameio-1.8.2/src/fameio/source/logs.py
--rw-rw-rw-   0        0        0     1321 2024-02-14 11:04:50.000000 fameio-1.8.2/src/fameio/source/path_resolver.py
-drwxrwxrwx   0        0        0        0 2024-03-22 07:28:36.084374 fameio-1.8.2/src/fameio/source/results/
--rw-rw-rw-   0        0        0      109 2024-02-14 11:04:50.000000 fameio-1.8.2/src/fameio/source/results/__init__.py
--rw-rw-rw-   0        0        0     4321 2024-02-14 11:04:50.000000 fameio-1.8.2/src/fameio/source/results/agent_type.py
--rw-rw-rw-   0        0        0     3785 2024-03-22 07:22:59.000000 fameio-1.8.2/src/fameio/source/results/conversion.py
--rw-rw-rw-   0        0        0     4216 2024-03-22 07:20:44.000000 fameio-1.8.2/src/fameio/source/results/csv_writer.py
--rw-rw-rw-   0        0        0     6222 2024-03-22 07:20:44.000000 fameio-1.8.2/src/fameio/source/results/data_transformer.py
--rw-rw-rw-   0        0        0     3960 2024-02-14 11:04:50.000000 fameio-1.8.2/src/fameio/source/results/output_dao.py
--rw-rw-rw-   0        0        0     4791 2024-03-22 07:20:44.000000 fameio-1.8.2/src/fameio/source/results/reader.py
-drwxrwxrwx   0        0        0        0 2024-03-22 07:28:36.086999 fameio-1.8.2/src/fameio/source/scenario/
--rw-rw-rw-   0        0        0      372 2024-02-14 11:04:50.000000 fameio-1.8.2/src/fameio/source/scenario/__init__.py
--rw-rw-rw-   0        0        0     3830 2024-03-22 07:20:44.000000 fameio-1.8.2/src/fameio/source/scenario/agent.py
--rw-rw-rw-   0        0        0     5002 2024-03-22 07:20:44.000000 fameio-1.8.2/src/fameio/source/scenario/attribute.py
--rw-rw-rw-   0        0        0     8853 2024-03-22 07:20:44.000000 fameio-1.8.2/src/fameio/source/scenario/contract.py
--rw-rw-rw-   0        0        0     1455 2024-03-22 07:20:44.000000 fameio-1.8.2/src/fameio/source/scenario/exception.py
--rw-rw-rw-   0        0        0     1376 2024-02-14 11:04:50.000000 fameio-1.8.2/src/fameio/source/scenario/fameiofactory.py
--rw-rw-rw-   0        0        0     4593 2024-03-22 07:20:44.000000 fameio-1.8.2/src/fameio/source/scenario/generalproperties.py
--rw-rw-rw-   0        0        0     3582 2024-03-22 07:20:44.000000 fameio-1.8.2/src/fameio/source/scenario/scenario.py
-drwxrwxrwx   0        0        0        0 2024-03-22 07:28:36.086999 fameio-1.8.2/src/fameio/source/schema/
--rw-rw-rw-   0        0        0      270 2024-02-14 11:04:50.000000 fameio-1.8.2/src/fameio/source/schema/__init__.py
--rw-rw-rw-   0        0        0     3331 2024-03-22 07:20:44.000000 fameio-1.8.2/src/fameio/source/schema/agenttype.py
--rw-rw-rw-   0        0        0     8214 2024-03-22 07:20:44.000000 fameio-1.8.2/src/fameio/source/schema/attribute.py
--rw-rw-rw-   0        0        0      224 2024-02-14 11:04:50.000000 fameio-1.8.2/src/fameio/source/schema/exception.py
--rw-rw-rw-   0        0        0     1715 2024-03-22 07:20:44.000000 fameio-1.8.2/src/fameio/source/schema/schema.py
--rw-rw-rw-   0        0        0     1924 2024-03-22 07:20:44.000000 fameio-1.8.2/src/fameio/source/series.py
--rw-rw-rw-   0        0        0     6943 2024-03-22 07:20:44.000000 fameio-1.8.2/src/fameio/source/time.py
--rw-rw-rw-   0        0        0      630 2024-03-22 07:20:44.000000 fameio-1.8.2/src/fameio/source/tools.py
--rw-rw-rw-   0        0        0    11409 2024-03-22 07:20:44.000000 fameio-1.8.2/src/fameio/source/validator.py
--rw-rw-rw-   0        0        0    11633 2024-03-22 07:20:44.000000 fameio-1.8.2/src/fameio/source/writer.py
-drwxrwxrwx   0        0        0        0 2024-03-22 07:28:36.068706 fameio-1.8.2/src/fameio.egg-info/
--rw-rw-rw-   0        0        0    30291 2024-03-22 07:28:35.000000 fameio-1.8.2/src/fameio.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1640 2024-03-22 07:28:35.000000 fameio-1.8.2/src/fameio.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-22 07:28:35.000000 fameio-1.8.2/src/fameio.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      126 2024-03-22 07:28:35.000000 fameio-1.8.2/src/fameio.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-03-22 07:26:08.000000 fameio-1.8.2/src/fameio.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       70 2024-03-22 07:28:35.000000 fameio-1.8.2/src/fameio.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-03-22 07:28:35.000000 fameio-1.8.2/src/fameio.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-22 07:28:36.086999 fameio-1.8.2/tests/
--rw-rw-rw-   0        0        0    13962 2024-03-22 07:20:44.000000 fameio-1.8.2/tests/test_cli.py
--rw-rw-rw-   0        0        0     4625 2024-03-22 07:20:44.000000 fameio-1.8.2/tests/test_load_save_reload_compare_outputs.py
--rw-rw-rw-   0        0        0     2462 2024-02-14 11:04:50.000000 fameio-1.8.2/tests/test_loader.py
--rw-rw-rw-   0        0        0     1077 2024-03-22 07:20:44.000000 fameio-1.8.2/tests/test_series.py
--rw-rw-rw-   0        0        0     6485 2024-03-22 07:20:44.000000 fameio-1.8.2/tests/test_time.py
--rw-rw-rw-   0        0        0     1226 2024-03-22 07:20:44.000000 fameio-1.8.2/tests/test_tools.py
--rw-rw-rw-   0        0        0    22455 2024-03-22 07:20:44.000000 fameio-1.8.2/tests/test_validator.py
+-rw-r--r--   0        0        0     9874 2024-04-03 16:31:37.396336 fameio-2.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0    10391 2023-04-14 05:55:34.824015 fameio-2.0.0/LICENSE.txt
+drwxr-xr-x   0        0        0        0 2023-05-03 15:01:38.291067 fameio-2.0.0/LICENSES/
+-rw-r--r--   0        0        0    10391 2023-04-14 05:55:34.824015 fameio-2.0.0/LICENSES/Apache-2.0.txt
+-rw-r--r--   0        0        0    19051 2023-05-03 15:01:38.291067 fameio-2.0.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0        0        0     7169 2023-04-14 05:55:34.825013 fameio-2.0.0/LICENSES/CC0-1.0.txt
+-rw-r--r--   0        0        0     1850 2024-04-03 16:31:37.396336 fameio-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0    30287 2024-03-07 15:03:46.249549 fameio-2.0.0/README.md
+-rw-r--r--   0        0        0      109 2023-04-14 05:55:34.826011 fameio-2.0.0/src/fameio/__init__.py
+-rw-r--r--   0        0        0      741 2024-03-07 15:03:46.250611 fameio-2.0.0/src/fameio/scripts/__init__.py
+-rw-r--r--   0        0        0      107 2024-03-07 15:03:46.251544 fameio-2.0.0/src/fameio/scripts/__init__.py.license
+-rw-r--r--   0        0        0     3635 2024-04-03 06:43:28.347153 fameio-2.0.0/src/fameio/scripts/convert_results.py
+-rw-r--r--   0        0        0      107 2024-02-26 16:17:50.230821 fameio-2.0.0/src/fameio/scripts/convert_results.py.license
+-rw-r--r--   0        0        0     1349 2024-04-03 06:43:28.347153 fameio-2.0.0/src/fameio/scripts/make_config.py
+-rw-r--r--   0        0        0      107 2024-03-07 15:03:46.252566 fameio-2.0.0/src/fameio/scripts/make_config.py.license
+-rw-r--r--   0        0        0      278 2023-04-14 05:55:34.828008 fameio-2.0.0/src/fameio/source/__init__.py
+-rw-r--r--   0        0        0      112 2024-03-07 15:03:46.252566 fameio-2.0.0/src/fameio/source/cli/__init__.py
+-rw-r--r--   0        0        0     3072 2024-03-07 15:03:46.253544 fameio-2.0.0/src/fameio/source/cli/convert_results.py
+-rw-r--r--   0        0        0     2369 2024-03-07 15:03:46.253544 fameio-2.0.0/src/fameio/source/cli/make_config.py
+-rw-r--r--   0        0        0     1413 2024-03-07 15:03:46.253544 fameio-2.0.0/src/fameio/source/cli/options.py
+-rw-r--r--   0        0        0     9366 2024-03-07 15:03:46.254559 fameio-2.0.0/src/fameio/source/cli/parser.py
+-rw-r--r--   0        0        0     7433 2024-01-17 10:31:27.021124 fameio-2.0.0/src/fameio/source/loader.py
+-rw-r--r--   0        0        0     2806 2024-01-17 10:31:27.021124 fameio-2.0.0/src/fameio/source/logs.py
+-rw-r--r--   0        0        0     1321 2024-01-17 10:31:27.022038 fameio-2.0.0/src/fameio/source/path_resolver.py
+-rw-r--r--   0        0        0      109 2023-04-14 05:55:34.829005 fameio-2.0.0/src/fameio/source/results/__init__.py
+-rw-r--r--   0        0        0     4321 2024-01-17 10:31:27.022038 fameio-2.0.0/src/fameio/source/results/agent_type.py
+-rw-r--r--   0        0        0     3721 2024-03-07 15:03:46.255599 fameio-2.0.0/src/fameio/source/results/conversion.py
+-rw-r--r--   0        0        0     4868 2024-02-26 16:17:50.231821 fameio-2.0.0/src/fameio/source/results/csv_writer.py
+-rw-r--r--   0        0        0     6264 2024-03-07 15:03:46.255599 fameio-2.0.0/src/fameio/source/results/data_transformer.py
+-rw-r--r--   0        0        0     6928 2024-03-07 15:03:46.256605 fameio-2.0.0/src/fameio/source/results/input_dao.py
+-rw-r--r--   0        0        0     3960 2024-01-17 10:31:27.024035 fameio-2.0.0/src/fameio/source/results/output_dao.py
+-rw-r--r--   0        0        0     5078 2024-04-03 06:43:28.349147 fameio-2.0.0/src/fameio/source/results/reader.py
+-rw-r--r--   0        0        0      843 2024-04-03 16:25:46.569642 fameio-2.0.0/src/fameio/source/results/yaml_writer.py
+-rw-r--r--   0        0        0      372 2023-04-14 05:55:34.830003 fameio-2.0.0/src/fameio/source/scenario/__init__.py
+-rw-r--r--   0        0        0     4713 2024-02-26 16:17:50.232821 fameio-2.0.0/src/fameio/source/scenario/agent.py
+-rw-r--r--   0        0        0     4834 2024-02-26 16:17:50.233821 fameio-2.0.0/src/fameio/source/scenario/attribute.py
+-rw-r--r--   0        0        0     9448 2024-02-26 16:17:50.233821 fameio-2.0.0/src/fameio/source/scenario/contract.py
+-rw-r--r--   0        0        0     1560 2023-11-28 14:30:17.776761 fameio-2.0.0/src/fameio/source/scenario/exception.py
+-rw-r--r--   0        0        0     1376 2024-01-26 10:13:38.847488 fameio-2.0.0/src/fameio/source/scenario/fameiofactory.py
+-rw-r--r--   0        0        0     4545 2024-02-14 10:56:32.725583 fameio-2.0.0/src/fameio/source/scenario/generalproperties.py
+-rw-r--r--   0        0        0     3727 2024-04-03 06:43:28.349147 fameio-2.0.0/src/fameio/source/scenario/scenario.py
+-rw-r--r--   0        0        0      270 2023-04-14 05:55:34.831001 fameio-2.0.0/src/fameio/source/schema/__init__.py
+-rw-r--r--   0        0        0     5198 2024-01-17 10:31:27.026034 fameio-2.0.0/src/fameio/source/schema/agenttype.py
+-rw-r--r--   0        0        0     8308 2024-01-17 10:31:27.027034 fameio-2.0.0/src/fameio/source/schema/attribute.py
+-rw-r--r--   0        0        0      224 2023-04-14 05:55:34.832000 fameio-2.0.0/src/fameio/source/schema/exception.py
+-rw-r--r--   0        0        0     2240 2024-01-17 10:31:27.027034 fameio-2.0.0/src/fameio/source/schema/schema.py
+-rw-r--r--   0        0        0     8120 2024-03-07 15:03:46.257542 fameio-2.0.0/src/fameio/source/series.py
+-rw-r--r--   0        0        0     6984 2024-01-17 10:31:27.028034 fameio-2.0.0/src/fameio/source/time.py
+-rw-r--r--   0        0        0     1052 2024-03-07 15:03:46.257542 fameio-2.0.0/src/fameio/source/tools.py
+-rw-r--r--   0        0        0    15734 2024-04-03 06:43:28.350143 fameio-2.0.0/src/fameio/source/validator.py
+-rw-r--r--   0        0        0    11353 2024-04-03 06:43:28.351141 fameio-2.0.0/src/fameio/source/writer.py
+-rw-r--r--   0        0        0    30769 1970-01-01 00:00:00.000000 fameio-2.0.0/PKG-INFO
```

### Comparing `fameio-1.8.2/LICENSE.txt` & `fameio-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fameio-1.8.2/PKG-INFO` & `fameio-2.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,61 +1,40 @@
-Metadata-Version: 2.1
-Name: fameio
-Version: 1.8.2
-Summary: Python scripts for operation of FAME models
-Home-page: https://gitlab.com/fame-framework/fame-io/
-Author: Felix Nitsch, Christoph Schimeczek, Ulrich Frey, Marc Deissenroth-Uhrig, Benjamin Fuchs, A. Achraf El Ghazi
-Author-email: fame@dlr.de
-License: Apache License 2.0
-Keywords: FAME,agent-based modelling
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: pandas
-Requires-Dist: fameprotobuf<1.3,>=1.2
-Requires-Dist: pyyaml
-Provides-Extra: dev
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: mockito; extra == "dev"
-Requires-Dist: pre-commit; extra == "dev"
-
 <!-- SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
 
 SPDX-License-Identifier: Apache-2.0 -->
 [![PyPI version](https://badge.fury.io/py/fameio.svg)](https://badge.fury.io/py/fameio)
 [![JOSS](https://joss.theoj.org/papers/10.21105/joss.04958/status.svg)](https://doi.org/10.21105/joss.04958)
 [![Zenodo](https://zenodo.org/badge/DOI/10.5281/zenodo.4314337.svg)](https://doi.org/10.5281/zenodo.4314337)
 [![PyPI license](https://img.shields.io/pypi/l/fameio.svg)](https://badge.fury.io/py/fameio)
 [![pipeline status](https://gitlab.com/fame-framework/fame-io/badges/main/pipeline.svg)](https://gitlab.com/fame-framework/fame-io/commits/main)
 [![coverage report](https://gitlab.com/fame-framework/fame-io/badges/main/coverage.svg)](https://gitlab.com/fame-framework/fame-io/-/commits/main)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![REUSE status](https://api.reuse.software/badge/gitlab.com/fame-framework/fame-io)](https://api.reuse.software/info/gitlab.com/fame-framework/fame-io)
+[![Common Changelog](https://common-changelog.org/badge.svg)](https://common-changelog.org)
+![GitLab last commit](https://img.shields.io/gitlab/last-commit/fame-framework%2Ffame-io)
+![GitLab closed issues by-label](https://img.shields.io/gitlab/issues/closed/fame-framework%2Ffame-io)
+
 
 # FAME-Io
 Python scripts for FAME models, generation of protobuf input files and conversion of protobuf output files.
 Please visit the [FAME-Wiki](https://gitlab.com/fame-framework/wiki/-/wikis/home) to get an explanation of FAME and its components.
-The package is also formerly known as [FAME-Py](https://doi.org/10.5281/zenodo.4314338).
 
 # Installation
-
 We recommend installing `fameio` using PyPI:
 
     pip install fameio
 
 You may also use `pipx`. For detailed information please refer to the official `pipx` [documentation](https://github.com/pypa/pipx).
 
     pipx install fameio
 
-`fameio` is currently developed and tested for Python 3.8 or higher. 
-See the `setup.py` for a complete listing of dependencies. 
+`fameio` is currently developed and tested for Python 3.8 or higher.
+See the `pyproject.toml` for a complete listing of dependencies.
 
 # Usage
-
 FAME-Io currently offers two main scripts `makeFameRunConfig` and `convertFameResults`.
 Both are automatically installed with the package.
 The first one creates a protobuf file for FAME applications using YAML definition files and CSV files.
 The latter one reads output files from FAME applications in protobuf format and converts them to CSV files.
 
 You may use the [example data](https://gitlab.com/dlr-ve/esy/amiris/examples) provided for the [AMIRIS](https://gitlab.com/dlr-ve/esy/amiris/amiris) model which can be used to simulate electricity markets in [Germany](https://gitlab.com/dlr-ve/esy/amiris/examples/-/tree/main/Germany2019), [Austria](https://gitlab.com/dlr-ve/esy/amiris/examples/-/tree/main/Austria2019), and a simple [proof-of-concept model](https://gitlab.com/dlr-ve/esy/amiris/examples/-/tree/main/Simple).
 
@@ -73,35 +52,51 @@
 | `-lf` or `--logfile` | Sets the logging file. Default is `None`. If `None` is provided, all logs get only printed to the console.      |
 | `-o` or `--output`   | Sets the path of the compiled protobuf output file. Default is `config.pb`.                                     |
 
 This could look as follows:
 
     makeFameRunConfig -f <path/to/scenario.yaml> -l debug -lf <path/to/scenario.log> -o <path/to/config.pb>
 
-
 You may also call the configuration builder from any Python script with
 
 ```python
-from fameio.scripts.make_config import run as make_config
+from fameio.scripts.make_config import Options, run as make_config
 
-make_config("path/to/scenario.yaml")
+make_config({Options.FILE: "path/to/scenario.yaml", })
 ```
 
 Similar to the console call you may also specify custom run config arguments and add it in a dictionary to the function call.
 
 ```python
-from fameio.scripts.make_config import run as make_config
-from fameio.source.cli import Options
+from fameio.scripts.make_config import Options, run as make_config
 
-run_config = {Options.LOG_LEVEL: "info",
+run_config = {Options.FILE: "path/to/scenario.yaml",
+              Options.LOG_LEVEL: "info",
               Options.OUTPUT: "output.pb",
               Options.LOG_FILE: "scenario.log",
               }
 
-make_config("path/to/scenario.yaml", run_config)
+make_config(run_config)
+```
+
+You can also use the associated argument parser, to extract the run_config dynamically from a string:
+
+```python
+from fameio.scripts.make_config import Options, run as make_config
+from fameio.source.cli.make_config import handle_args
+
+my_defaults = {Options.FILE: "path/to/scenario.yaml",
+                 Options.LOG_LEVEL: "info",
+                 Options.OUTPUT: "output.pb",
+                 Options.LOG_FILE: "scenario.log",
+                 }
+my_arg_string = ['-f', 'my/other/scenario.yaml', '-l', 'error']
+
+run_config = handle_args(my_arg_string, my_defaults)
+make_config(run_config)
 ```
 
 ### Scenario YAML
 The "scenario.yaml" file contains all configuration options for a FAME-based simulation.
 It consists of the sections `Schema`, `GeneralProperties`, `Agents` and `Contracts`, all of them described below.
 
 #### Schema
@@ -114,15 +109,16 @@
 * what type of Products an Agent can send in Contracts.
 
 The Schema consists of the sections `Header` and `AgentTypes`.
 
 ##### Header
 Scientific applications often evolve, and so do their required input parameters.
 Therefore, the header specifies information what FAME-based application the schema is corresponding to.
-In this way a schema.yaml is tied to a specific version an application, ensuring a match between the inputs required by the application, and those provided by the files created with FAME-Io.
+In this way a schema.yaml is tied to a specific version an application, ensuring a match between the inputs required by
+the application, and those provided by the files created with FAME-Io.
 
 ```yaml
 Header:
   Project: MyProjectName
   RepoUrl: https://mygithosting.com/myProject
   CommitHash: abc123
 ```
@@ -136,17 +132,17 @@
 The structure of this section
 
 ```yaml
 AgentTypes:
   MyAgentType:
     Attributes:
       MyAttribute:
-         ...
+        ...
       MyOtherAttribute:
-         ...
+        ...
     Products: [ 'Product1', 'Product2', 'Product3' ]
   MyOtherAgentWithoutProductsOrAttributes:
 ```
 
 * `MyAgentType` Java's simple class name of the Agent type
 * `Attributes` indicates that beginning of the attribute definition section for this Agent type
 * `MyAttribute` Name of an attribute as specified in the corresponding Java source code of this Agent type (annotated with "@Input")
@@ -176,34 +172,34 @@
       AttributeType: double
 ```
 
 * `MySimpleAttribute`, `MyDoubleList`, `MyComplexAttribute` Names of the attributes as specified in the Java enum annotated with "@Input"
 * `AttributeType` (required) data type of the attribute; see options in table below
 * `Mandatory` (optional - true by default) if true: the attribute is required for this agent and validation will fail if the attribute is missing in the scenario **and** no default is provided
 * `List` (optional - false by default)
-  * `AttributeType: time_series` cannot be true
-  * `AttributeType: block`
-    * if true: any nested element in the scenario must be part of a list element and thus can appear multiple times
-    * if false: any nested element in the scenario can only appear once
-  * any other AttributeType: the attribute is interpreted as list, i.e. multiple values can be assigned to this attribute in the scenario
+    * `AttributeType: time_series` cannot be true
+    * `AttributeType: block`
+        * if true: any nested element in the scenario must be part of a list element and thus can appear multiple times
+        * if false: any nested element in the scenario can only appear once
+    * any other AttributeType: the attribute is interpreted as list, i.e. multiple values can be assigned to this attribute in the scenario
 * `NestedAttributes` (required only if `AttributeType: block`, otherwise disallowed) starts an inner Attribute definition block - defined Attributes are sub-elements of `MyComplexAttribute`
 * `Values` (optional - None by default): if present defines a list of allowed values for this attribute
 * `Default` (optional - None by default): if present defines a default value to be used in case the scenario does not specify it
 * `Help` (optional - None by default): if present defines a help text to you attribute
 
-| AttributeType   | value                                                                                                                   |
-|-----------------|-------------------------------------------------------------------------------------------------------------------------|
-| `integer`       | a 32-bit integer value                                                                                                  |
-| `double`        | a 64-bit floating-point value (integers also allowed)                                                                   |
-| `long`          | a 64-bit integer value                                                                                                  |
-| `time_stamp`    | either a FAME time stamp string or 64-bit integer value                                                                 |
-| `string`        | any string                                                                                                              |
-| `enum`          | any string, however, usually tied to a set of allowed `Values`                                                          |
-| `time_series`   | either a path to a .csv-file or a single 64-bit floating-point value; does not support `List: true`                     |
-| `block`         | this attribute has no value of its own but hosts a group of nested Attributes; implies `NestedAttributes` to be defined |
+| AttributeType | value                                                                                                                   |
+|---------------|-------------------------------------------------------------------------------------------------------------------------|
+| `integer`     | a 32-bit integer value                                                                                                  |
+| `double`      | a 64-bit floating-point value (integers also allowed)                                                                   |
+| `long`        | a 64-bit integer value                                                                                                  |
+| `time_stamp`  | either a FAME time stamp string or 64-bit integer value                                                                 |
+| `string`      | any string                                                                                                              |
+| `enum`        | any string, however, usually tied to a set of allowed `Values`                                                          |
+| `time_series` | either a path to a .csv-file or a single 64-bit floating-point value; does not support `List: true`                     |
+| `block`       | this attribute has no value of its own but hosts a group of nested Attributes; implies `NestedAttributes` to be defined |
 
 #### GeneralProperties
 Specifies FAME-specific properties of the simulation. Structure:
 
 ```yaml
 GeneralProperties:
   RunId: 1
@@ -215,22 +211,24 @@
     Interval: 100
     Process: 0
 ```
 
 Parameters:
 * `RunId` an ID that can be given to the simulation; use at your discretion
 * `StartTime` time stamp in the format YYYY-MM-DD_hh:mm:ss; first moment of the simulation.
-* `StopTime` time stamp in the format YYYY-MM-DD_hh:mm:ss; last moment of the simulation - i.e. simulation terminates after passing that time stamp
+* `StopTime` time stamp in the format YYYY-MM-DD_hh:mm:ss; last moment of the simulation - i.e. simulation terminates
+  after passing that time stamp
 * `RandomSeed` seed to initialise random number generation; each value leads to a unique series of random numbers.
 * `Interval` number of simulation ticks in between write-to-disk events; may be used for performance optimisations;
 * `Process` id of process that performs write-to-disk operations; leave at 0 to be compatible with single-processes;
 
 #### Agents
 Specifies all Agents to be created in the simulation in a list. Each Agent has its own entry.
 Structure:
+
 ```yaml
 Agents:
   - Type: MyAgentWithInputs
     Id: 1
     Attributes:
       MyEnum: SAME_SHARES
       MyInteger: 2
@@ -239,16 +237,18 @@
 
   - Type: MyAgentWithoutInputs
     Id: 2
 ```
 
 Agent Parameters:
 * `Type` Mandatory; Java's simple class name of the agent to be created
-* `Id` Mandatory; simulation-unique id of this agent; if two agents have the same ID, the configuration process will stop.
-* `Attributes` Optional; if the agent has any attributes, specify them here in the format "AttributeName: value"; please see attribute table above
+* `Id` Mandatory; simulation-unique id of this agent; if two agents have the same ID, the configuration process will
+  stop.
+* `Attributes` Optional; if the agent has any attributes, specify them here in the format "AttributeName: value"; please
+  see attribute table above
 
 The specified `Attributes` for each agent must match the specified `Attributes` options in the linked Schema (see above).
 For better structure and readability of the `scenario.yaml`, `Attributes` may also be specified in a nested way as demonstrated below.
 
 ```yaml
 Agents:
   - Type: MyAgentWithInputs
@@ -263,15 +263,15 @@
           MyTimeSeries: "./path/to/time_series.csv"
 ```
 
 In case Attributes are defined with `List: true` option, lists are assigned to an Attribute or Group:
 
 ```yaml
 Attributes:
-  MyDoubleList: [5.2, 4.5, 7, 9.9]
+  MyDoubleList: [ 5.2, 4.5, 7, 9.9 ]
   MyListGroup:
     - IntValueA: 5
       IntValueB: 42
     - IntValueA: 7
       IntValueB: 100
 ```
 
@@ -316,43 +316,43 @@
 `SenderId` and `ReceiverId` can both be lists and support One-to-N, N-to-One and N-to-N relations like in the following example:
 
 ```yaml
 Contracts:
   # effectively 3 similar contracts (0 -> 11), (0 -> 12), (0 -> 13)
   # with otherwise identical ProductName, FirstDeliveryTime & DeliveryIntervalInSteps
   - SenderId: 0
-    ReceiverId: [11, 12, 13]
+    ReceiverId: [ 11, 12, 13 ]
     ProductName: MyOtherProduct
     FirstDeliveryTime: 100
     DeliveryIntervalInSteps: 3600
 
   # effectively 3 similar contracts (1 -> 10), (2 -> 10), (3 -> 10)
   # with otherwise identical ProductName, FirstDeliveryTime & DeliveryIntervalInSteps
-  - SenderId: [1, 2, 3]
+  - SenderId: [ 1, 2, 3 ]
     ReceiverId: 10
     ProductName: MyProduct
     FirstDeliveryTime: 100
     DeliveryIntervalInSteps: 3600
 
   # effectively 3 similar contracts (1 -> 11), (2 -> 12), (3 -> 13)
   # with otherwise identical ProductName, FirstDeliveryTime & DeliveryIntervalInSteps
-  - SenderId: [1, 2, 3]
-    ReceiverId: [11, 12, 13]
+  - SenderId: [ 1, 2, 3 ]
+    ReceiverId: [ 11, 12, 13 ]
     ProductName: MyThirdProduct
     FirstDeliveryTime: 100
     DeliveryIntervalInSteps: 3600
 ```
 
 Combined with YAML anchors complex contract chains can be easily reduced to a minimum of required configuration.
 The following example is equivalent to the previous one and allows a quick extension of contracts to a new couple of agents e.g. (4;14):
 
 ```yaml
 Groups:
-  - &agentList1: [1,2,3]
-  - &agentList2: [11,12,13]
+  - &agentList1: [ 1,2,3 ]
+  - &agentList2: [ 11,12,13 ]
 
 Contracts:
   - SenderId: 0
     ReceiverId: *agentList2
     ProductName: MyOtherProduct
     FirstDeliveryTime: 100
     DeliveryIntervalInSteps: 3600
@@ -374,22 +374,25 @@
 TIME_SERIES inputs are not directly fed into the Scenario YAML file.
 Instead, TIME_SERIES reference a CSV file that can be stored some place else.
 These CSV files follow a specific structure:
 * They must contain exactly two columns.
 * The first column must be a time stamp in form `YYYY-MM-DD_hh:mm:ss`
 * The second column must be a numerical value (either integer or floating-point)
 * The separator of the two columns is a semicolon
+* The data must **not** have headers, except for comments marked with `#`
 
+You may add comments using `#`.
 Exemplary content of a valid CSV file:
 
+    # If you want an optional header, you must use a comment
     2012-01-01_00:00:00;400
     2013-01-01_00:00:00;720.5
     2014-01-01_00:00:00;650
     2015-01-01_00:00:00;99.27772
-    2016-01-01_00:00:00;42
+    2016-01-01_00:00:00;42  # optional comment on this particular data point
     2017-01-01_00:00:00;0.1
 
 Please refer also to the detailed article about `TimeStamps` in the [FAME-Wiki](https://gitlab.com/fame-framework/wiki/-/wikis/TimeStamp).
 
 ### Split and join multiple YAML files
 The user may include other YAML files into a YAML file to divide the content across files as convenient.
 We explicitly recommend using this feature for the `Schema` and `Contracts` sections.
@@ -404,14 +407,15 @@
 ###### file-structure
 ```
 a.yaml
 folder/b.yaml
 folder/c.yaml
 folder/deeper_folder/d.yaml
 ```
+
 the following !include commands work
 
 ###### in a.yaml
 ```
 ToBe: !include "folder/b.yaml"
 OrNot: !include "folder/deeper_folder/d.yaml"
 ```
@@ -423,18 +427,20 @@
 ```
 
 Provided that
 ###### in c.yaml
 ```
 Or: maybe
 ```
+
 ###### d.yaml
 ```
 not: "?"
 ```
+
 the resulting file would look like this:
 
 ###### THe Joined file a.yaml
 ```
 ToBe:
   ThatIs:
     Or: maybe
@@ -446,14 +452,15 @@
 
 You may also specify absolute file paths if preferred by starting with a "/".
 
 When specifying only a file path, the complete content of the file is assigned to the given key.
 You always need a key to assign the !include command to.
 However, you cannot combine the value returned from !include with other values in the same key.
 Thus, the following combinations do not work:
+
 ###### caveats.yml
 ```
 !include "file.yaml" # no key assigned
 
 Key:
   Some: OtherItem
   !include "file.yaml" # cannot join with other named items
@@ -478,15 +485,15 @@
   OtherKey: OtherValue
 ```
 
 ###### including_file.yaml
 ```yaml
 - Type: MyAgentWithInputs
   Id: 1
-  Attributes: !include_node [file_to_be_included.yaml, Set1:Subset1]
+  Attributes: !include_node [ file_to_be_included.yaml, Set1:Subset1 ]
 ```
 
 Compiling "including_file.yaml" results in
 
 ###### resulting_file.yaml
 ```yaml
 - Type: MyAgentWithInputs
@@ -498,33 +505,37 @@
 #### Load multiple files
 Using wildcards in the given path (e.g. "path/to/many/*.yaml") will lead to loading multiple files and assigning their content to the same key.
 You can make use of this feature with or without specifying a node selector.
 However, the elements to be joined across multiple files must be lists.
 These lists are then concatenated into a single list and then assigned to the key in the file calling !include.
 This feature is especially useful for Contracts: You can split the Contracts list into several files and place them in a separate folder.
 Then use !include to re-integrate them into your configuration. An example:
+
 ###### my_contract1.yaml
 ```
 Contracts:
  - ContractA
  - ContractB
 ```
+
 ###### my_contract2.yaml
 ```
 Contracts:
  - ContractC
  - ContractD
  - ContractE
 ```
+
 ###### including_file.yaml
 ```
 Contracts: [!include "my_contract*.yaml", "Contracts"]
 ```
 
 results in
+
 ###### result.yaml
 ```
 Contracts:
  - ContractA
  - ContractB
  - ContractC
  - ContractD
@@ -541,28 +552,29 @@
 An individual file for each type of Agent is created in a folder named after the protobuf input file.
 Call structure:
 
     convertFameResults -f <./path/to/protobuf_file.pb>
 
 You may also specify any of the following arguments:
 
-| Command                              | Action                                                                                                                                                                                                                                              |
-|--------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| `-l` or `--log` <option>             | Sets the logging level. Default is `info`. Options are `debug`, `info`, `warning`, `warn`, `error`, `critical`.                                                                                                                                     |
-| `-lf` or `--logfile` <file>          | Sets the logging file. Default is `None`. If `None` is provided, all logs get only printed to the console.                                                                                                                                          |
-| `-a` or `--agents` <list-of-agents>  | If specified, only a subset of agents is extracted from the protobuf file. Default is to extract all agents.                                                                                                                                        |
-| `-o` or `--output`                   | Sets the path to where the generated output files are written to. If not specified, the folder's name is derived from the input file's name. Folder will be created if it does not exist.                                                           |
-| `-se` or `--single-export`           | Enables export of individual agents to individual files, when present. If not present (the default) one file per `AgentType` is created.                                                                                                            |
-| `-m` or `--memory-saving`            | When specified, reduces memory usage profile at the cost of runtime. Use only when necessary.                                                                                                                                                       |
-| `-cc` or `--complex-column` <option> | Defines how to deal with complex indexed output columns (if any). `IGNORE` ignores complex columns. `MERGE` squashes all data from complex columns in one big string entry. `SPLIT` creates a separate file for each complex indexed output column. |
-| `-t` or `--time` <option>            | Option to define conversion of time steps to given format (default=`UTC`) by `-t/--time {UTC, INT, FAME}`                                                                                                                                           |
+| Command                                     | Action                                                                                                                                                                                                                                              |
+|---------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `-l` or `--log` <option>                    | Sets the logging level. Default is `info`. Options are `debug`, `info`, `warning`, `warn`, `error`, `critical`.                                                                                                                                     |
+| `-lf` or `--logfile` <file>                 | Sets the logging file. Default is `None`. If `None` is provided, all logs get only printed to the console.                                                                                                                                          |
+| `-a` or `--agents` <list-of-agents>         | If specified, only a subset of agents is extracted from the protobuf file. Default is to extract all agents.                                                                                                                                        |
+| `-o` or `--output`                          | Sets the path to where the generated output files are written to. If not specified, the folder's name is derived from the input file's name. Folder will be created if it does not exist.                                                           |
+| `-se` or `--single-export`                  | Enables export of individual agents to individual files, when present. If not present (the default) one file per `AgentType` is created.                                                                                                            |
+| `-m` or `--memory-saving`                   | When specified, reduces memory usage profile at the cost of runtime. Use only when necessary.                                                                                                                                                       |
+| `-cc` or `--complex-column` <option>        | Defines how to deal with complex indexed output columns (if any). `IGNORE` ignores complex columns. `MERGE` squashes all data from complex columns in one big string entry. `SPLIT` creates a separate file for each complex indexed output column. |
+| `-t` or `--time` <option>                   | Option to define conversion of time steps to given format (default=`UTC`) by `-t/--time {UTC, INT, FAME}`                                                                                                                                           |
+| `--input-recovery` or `--no-input-recovery` | If True, all input data are recovered as well as the outputs (default=False).                                                                                                                                                                       |
 
 Additionally, you may merge TimeSteps of a certain range of steps in the output files to
-  i) associate multiple time steps with a common logical time in your simulation
-  ii) reduce number of lines in output files
+i) associate multiple time steps with a common logical time in your simulation
+ii) reduce number of lines in output files
 
 For this, add the option `merge-times` and specify the arguments as follows:
 
 | Command                   | Action                                                                                   |
 |---------------------------|------------------------------------------------------------------------------------------|
 | `-fp` or `--focal-point`  | TimeStep on which `steps-before` earlier and `steps-after` later TimeSteps are merged on |
 | `-sb` or `--steps-before` | Range of TimeSteps before the `focal-point` they get merged to                           |
@@ -574,87 +586,79 @@
 
 Make sure that in the range of time steps you specify for merging there is only one value per column in the merged time range.
 If multiple values per column are merged values will get concatenated and might yield unexpected results.
 
 You may also call the conversion script from any Python script with:
 
 ```python
-from fameio.scripts.convert_results import run as convert_results
+from fameio.scripts.convert_results import Options, run as convert_results
 
-convert_results("./path/to/protobuf_file.pb")
+convert_results({Options.FILE: "./path/to/protobuf_file.pb"})
 ```
 
 Similar to the console call you may also specify custom run config arguments and add it in a dictionary to the function call.
 
 ```python
-from fameio.scripts.convert_results import run as convert_results
-from fameio.source.cli import Options
+from fameio.scripts.convert_results import Options, run as convert_results
 
-run_config = {Options.LOG_LEVEL: "info",
+run_config = {Options.FILE: "./path/to/protobuf_file.pb",
+              Options.LOG_LEVEL: "info",
               Options.LOG_FILE: "scenario.log",
               Options.OUTPUT: "Output",
               Options.AGENT_LIST: ['AgentType1', 'AgentType2'],
               Options.MEMORY_SAVING: False,
               Options.SINGLE_AGENT_EXPORT: False,
               Options.RESOLVE_COMPLEX_FIELD: "SPLIT",
               Options.TIME: "INT",
               Options.TIME_MERGING: {},
               }
 
-convert_results("./path/to/protobuf_file.pb", run_config)
+convert_results(run_config)
+```
+
+You can also use the associated argument parser, to extract the run_config dynamically from a string:
+
+```python
+from fameio.scripts.convert_results import Options, run as convert_results
+from fameio.source.cli.convert_results import handle_args
+
+my_defaults = {Options.FILE: "./path/to/protobuf_file.pb",
+               Options.LOG_LEVEL: "info",
+               Options.LOG_FILE: "scenario.log",
+               Options.OUTPUT: "Output",
+               Options.AGENT_LIST: ['AgentType1', 'AgentType2'],
+               Options.MEMORY_SAVING: False,
+               Options.SINGLE_AGENT_EXPORT: False,
+               Options.RESOLVE_COMPLEX_FIELD: "SPLIT",
+               Options.TIME: "INT",
+               Options.TIME_MERGING: {},
+               }
+my_arg_string = ['-f', 'my/other/scenario.yaml', '-l', 'error']
+
+run_config = handle_args(my_arg_string, my_defaults)
+convert_results(run_config)
 ```
 
 ## Cite FAME-Io
 If you use FAME-Io for academic work, please cite as follows.
 
 Bibtex entry:
+
 ```
 @article{fameio2023joss,
   author  = {Felix Nitsch and Christoph Schimeczek and Ulrich Frey and Benjamin Fuchs},
   title   = {FAME-Io: Configuration tools for complex agent-based simulations},
   journal = {Journal of Open Source Software},
   year    = {2023},
   doi     = {doi: https://doi.org/10.21105/joss.04958}
 }
 ```
 
 ## Available Support
-This is a purely scientific project by (at the moment) one research group. 
+This is a purely scientific project by (at the moment) one research group.
 Thus, there is no paid technical support available.
 However, we will give our best to answer your questions and provide support.
 
 If you experience any trouble with FAME-Io, you may contact the developers via [fame@dlr.de](mailto:fame@dlr.de).
-Please report bugs and make feature requests by filing issues following the provided templates (see also [Contribute](#Contribute)).
-For substantial enhancements, we recommend that you contact us via [fame@dlr.de](mailto:fame@dlr.de) for working together on the code in common projects or towards common publications and thus further develop FAME-Io.
-
-# Contribute
-Please read the Contributors License Agreement `cla.md`, sign it and send it to [`fame@dlr.de`](mailto:fame@dlr.de) before contributing.
-
-You will also find templates for [bug reports](https://gitlab.com/fame-framework/fame-io/-/blob/main/.gitlab/issue_templates/bug_report.md),
-[feature requests](https://gitlab.com/fame-framework/fame-io/-/blob/main/.gitlab/issue_templates/feature_request.md), and 
-[pull requests](https://gitlab.com/fame-framework/fame-io/-/blob/main/.gitlab/issue_templates/pull_request.md).
-
-We kindly ask you to read the Contributors License Agreement `cla.md`, sign it, and send it to [`fame@dlr.de`](mailto:fame@dlr.de) before contributing. Please see our [conventions of contribution](https://gitlab.com/fame-framework/wiki/-/wikis/developers/contribute/Conventions) which are described in the Wiki.
-
-## Testing changes locally 
-
-Once some changes have been performed on the local git clone, use the following command to override your local installation with your modified copy in order to test the result:
-
-```bash
-python3 setup.py bdist_wheel && pip3 install --force-reinstall --no-dependencies ./dist/*.whl
-```
-
-## Code style
-
-We use the code formatting library [`black`](https://pypi.org/project/black/).
-The maximum line length is defined as 120 characters. 
-Therefore, before committing, run `black --line-length 120 .`
-
-## Pre-Commit hooks
-
-FAME-Io uses several pre-commit hooks to ensure high code quality.
-To use them, install `dev` packages and then initialise pre-commit in FAME-Io's base folder:
-
-```
-    pip install fameio[dev]
-    pre-commit install -t pre-commit -t pre-push
-```
+Please report bugs and make feature requests by filing issues following the provided templates (see also [Contribute](CONTRIBUTING.md)).
+For substantial enhancements, we recommend that you contact us via [fame@dlr.de](mailto:fame@dlr.de) for working
+together on the code in common projects or towards common publications and thus further develop FAME-Io.
```

### Comparing `fameio-1.8.2/README.md` & `fameio-2.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,637 +1,694 @@
-<!-- SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
-
-SPDX-License-Identifier: Apache-2.0 -->
-[![PyPI version](https://badge.fury.io/py/fameio.svg)](https://badge.fury.io/py/fameio)
-[![JOSS](https://joss.theoj.org/papers/10.21105/joss.04958/status.svg)](https://doi.org/10.21105/joss.04958)
-[![Zenodo](https://zenodo.org/badge/DOI/10.5281/zenodo.4314337.svg)](https://doi.org/10.5281/zenodo.4314337)
-[![PyPI license](https://img.shields.io/pypi/l/fameio.svg)](https://badge.fury.io/py/fameio)
-[![pipeline status](https://gitlab.com/fame-framework/fame-io/badges/main/pipeline.svg)](https://gitlab.com/fame-framework/fame-io/commits/main)
-[![coverage report](https://gitlab.com/fame-framework/fame-io/badges/main/coverage.svg)](https://gitlab.com/fame-framework/fame-io/-/commits/main)
-[![REUSE status](https://api.reuse.software/badge/gitlab.com/fame-framework/fame-io)](https://api.reuse.software/info/gitlab.com/fame-framework/fame-io)
-
-# FAME-Io
-Python scripts for FAME models, generation of protobuf input files and conversion of protobuf output files.
-Please visit the [FAME-Wiki](https://gitlab.com/fame-framework/wiki/-/wikis/home) to get an explanation of FAME and its components.
-The package is also formerly known as [FAME-Py](https://doi.org/10.5281/zenodo.4314338).
-
-# Installation
-
-We recommend installing `fameio` using PyPI:
-
-    pip install fameio
-
-You may also use `pipx`. For detailed information please refer to the official `pipx` [documentation](https://github.com/pypa/pipx).
-
-    pipx install fameio
-
-`fameio` is currently developed and tested for Python 3.8 or higher. 
-See the `setup.py` for a complete listing of dependencies. 
-
-# Usage
-
-FAME-Io currently offers two main scripts `makeFameRunConfig` and `convertFameResults`.
-Both are automatically installed with the package.
-The first one creates a protobuf file for FAME applications using YAML definition files and CSV files.
-The latter one reads output files from FAME applications in protobuf format and converts them to CSV files.
-
-You may use the [example data](https://gitlab.com/dlr-ve/esy/amiris/examples) provided for the [AMIRIS](https://gitlab.com/dlr-ve/esy/amiris/amiris) model which can be used to simulate electricity markets in [Germany](https://gitlab.com/dlr-ve/esy/amiris/examples/-/tree/main/Germany2019), [Austria](https://gitlab.com/dlr-ve/esy/amiris/examples/-/tree/main/Austria2019), and a simple [proof-of-concept model](https://gitlab.com/dlr-ve/esy/amiris/examples/-/tree/main/Simple).
-
-## Make a FAME run configuration
-Digests configuration files in YAML format, combines them with CSV data files and creates a single input file for FAME applications in protobuf format.
-Call structure:
-
-    makeFameRunConfig -f <path/to/scenario.yaml>
-
-You may also specify any of the following arguments:
-
-| Command              | Action                                                                                                          |
-|----------------------|-----------------------------------------------------------------------------------------------------------------|
-| `-l` or `--log`      | Sets the logging level. Default is `info`. Options are `debug`, `info`, `warning`, `warn`, `error`, `critical`. |
-| `-lf` or `--logfile` | Sets the logging file. Default is `None`. If `None` is provided, all logs get only printed to the console.      |
-| `-o` or `--output`   | Sets the path of the compiled protobuf output file. Default is `config.pb`.                                     |
-
-This could look as follows:
-
-    makeFameRunConfig -f <path/to/scenario.yaml> -l debug -lf <path/to/scenario.log> -o <path/to/config.pb>
-
-
-You may also call the configuration builder from any Python script with
-
-```python
-from fameio.scripts.make_config import run as make_config
-
-make_config("path/to/scenario.yaml")
-```
-
-Similar to the console call you may also specify custom run config arguments and add it in a dictionary to the function call.
-
-```python
-from fameio.scripts.make_config import run as make_config
-from fameio.source.cli import Options
-
-run_config = {Options.LOG_LEVEL: "info",
-              Options.OUTPUT: "output.pb",
-              Options.LOG_FILE: "scenario.log",
-              }
-
-make_config("path/to/scenario.yaml", run_config)
-```
-
-### Scenario YAML
-The "scenario.yaml" file contains all configuration options for a FAME-based simulation.
-It consists of the sections `Schema`, `GeneralProperties`, `Agents` and `Contracts`, all of them described below.
-
-#### Schema
-The Schema is used to validate the inputs of the "scenario.yaml".
-Since the Schema should be valid across multiple scenarios, it is recommended to defined it in a separate file and include the file here.
-
-Currently, the schema specifies:
-* which type of Agents can be created
-* what type of input attributes an Agent uses
-* what type of Products an Agent can send in Contracts.
-
-The Schema consists of the sections `Header` and `AgentTypes`.
-
-##### Header
-Scientific applications often evolve, and so do their required input parameters.
-Therefore, the header specifies information what FAME-based application the schema is corresponding to.
-In this way a schema.yaml is tied to a specific version an application, ensuring a match between the inputs required by the application, and those provided by the files created with FAME-Io.
-
-```yaml
-Header:
-  Project: MyProjectName
-  RepoUrl: https://mygithosting.com/myProject
-  CommitHash: abc123
-```
-
-* `Project` name of your project / FAME-based application
-* `RepoUrl` URL of your project
-* `CommitHash` hash of the commit / version of your project
-
-##### AgentTypes
-Here, each type of agent that can be created in your FAME-based application is listed, its attributes and its available Products for Contracts.
-The structure of this section
-
-```yaml
-AgentTypes:
-  MyAgentType:
-    Attributes:
-      MyAttribute:
-         ...
-      MyOtherAttribute:
-         ...
-    Products: [ 'Product1', 'Product2', 'Product3' ]
-  MyOtherAgentWithoutProductsOrAttributes:
-```
-
-* `MyAgentType` Java's simple class name of the Agent type
-* `Attributes` indicates that beginning of the attribute definition section for this Agent type
-* `MyAttribute` Name of an attribute as specified in the corresponding Java source code of this Agent type (annotated with "@Input")
-* `MyOtherAttribute` Name of another attribute derived from Java source code
-* `Products` list of Products that this Agent can send in Contracts; derived from Java source code of this Agent type (annotated with "@Product")
-* `MyOtherAgentWithoutProductsOrAttributes` an Agent type that requires neither Attributes nor Products
-
-Both Attributes and Products are optional - there could be useful Agents that require neither of them.
-In the above example attribute definition was not shown (indicated by `...`).
-The next example provides details on how to define an attribute:
-
-```yaml
-MySimpleAttribute:
-  AttributeType: enum
-  Mandatory: true
-  List: false
-  Values: [ 'AllowedValue1', 'AllowedValue2' ]
-  Default: 'AllowedValue1'
-  Help: 'My help text'
-
-MyComplexAttribute:
-  AttributeType: block
-  NestedAttributes:
-    InnerAttributeA:
-      AttributeType: integer
-    InnerAttributeB:
-      AttributeType: double
-```
-
-* `MySimpleAttribute`, `MyDoubleList`, `MyComplexAttribute` Names of the attributes as specified in the Java enum annotated with "@Input"
-* `AttributeType` (required) data type of the attribute; see options in table below
-* `Mandatory` (optional - true by default) if true: the attribute is required for this agent and validation will fail if the attribute is missing in the scenario **and** no default is provided
-* `List` (optional - false by default)
-  * `AttributeType: time_series` cannot be true
-  * `AttributeType: block`
-    * if true: any nested element in the scenario must be part of a list element and thus can appear multiple times
-    * if false: any nested element in the scenario can only appear once
-  * any other AttributeType: the attribute is interpreted as list, i.e. multiple values can be assigned to this attribute in the scenario
-* `NestedAttributes` (required only if `AttributeType: block`, otherwise disallowed) starts an inner Attribute definition block - defined Attributes are sub-elements of `MyComplexAttribute`
-* `Values` (optional - None by default): if present defines a list of allowed values for this attribute
-* `Default` (optional - None by default): if present defines a default value to be used in case the scenario does not specify it
-* `Help` (optional - None by default): if present defines a help text to you attribute
-
-| AttributeType   | value                                                                                                                   |
-|-----------------|-------------------------------------------------------------------------------------------------------------------------|
-| `integer`       | a 32-bit integer value                                                                                                  |
-| `double`        | a 64-bit floating-point value (integers also allowed)                                                                   |
-| `long`          | a 64-bit integer value                                                                                                  |
-| `time_stamp`    | either a FAME time stamp string or 64-bit integer value                                                                 |
-| `string`        | any string                                                                                                              |
-| `enum`          | any string, however, usually tied to a set of allowed `Values`                                                          |
-| `time_series`   | either a path to a .csv-file or a single 64-bit floating-point value; does not support `List: true`                     |
-| `block`         | this attribute has no value of its own but hosts a group of nested Attributes; implies `NestedAttributes` to be defined |
-
-#### GeneralProperties
-Specifies FAME-specific properties of the simulation. Structure:
-
-```yaml
-GeneralProperties:
-  RunId: 1
-  Simulation:
-    StartTime: 2011-12-31_23:58:00
-    StopTime: 2012-12-30_23:58:00
-    RandomSeed: 1
-  Output:
-    Interval: 100
-    Process: 0
-```
-
-Parameters:
-* `RunId` an ID that can be given to the simulation; use at your discretion
-* `StartTime` time stamp in the format YYYY-MM-DD_hh:mm:ss; first moment of the simulation.
-* `StopTime` time stamp in the format YYYY-MM-DD_hh:mm:ss; last moment of the simulation - i.e. simulation terminates after passing that time stamp
-* `RandomSeed` seed to initialise random number generation; each value leads to a unique series of random numbers.
-* `Interval` number of simulation ticks in between write-to-disk events; may be used for performance optimisations;
-* `Process` id of process that performs write-to-disk operations; leave at 0 to be compatible with single-processes;
-
-#### Agents
-Specifies all Agents to be created in the simulation in a list. Each Agent has its own entry.
-Structure:
-```yaml
-Agents:
-  - Type: MyAgentWithInputs
-    Id: 1
-    Attributes:
-      MyEnum: SAME_SHARES
-      MyInteger: 2
-      MyDouble: 4.2
-      MyTimeSeries: "./path/to/time_series.csv"
-
-  - Type: MyAgentWithoutInputs
-    Id: 2
-```
-
-Agent Parameters:
-* `Type` Mandatory; Java's simple class name of the agent to be created
-* `Id` Mandatory; simulation-unique id of this agent; if two agents have the same ID, the configuration process will stop.
-* `Attributes` Optional; if the agent has any attributes, specify them here in the format "AttributeName: value"; please see attribute table above
-
-The specified `Attributes` for each agent must match the specified `Attributes` options in the linked Schema (see above).
-For better structure and readability of the `scenario.yaml`, `Attributes` may also be specified in a nested way as demonstrated below.
-
-```yaml
-Agents:
-  - Type: MyAgentWithInputs
-    Id: 1
-    Attributes:
-      Parent:
-        MyEnum: SAME_SHARES
-        MyInteger: 2
-      Parent2:
-        MyDouble: 4.2
-        Child:
-          MyTimeSeries: "./path/to/time_series.csv"
-```
-
-In case Attributes are defined with `List: true` option, lists are assigned to an Attribute or Group:
-
-```yaml
-Attributes:
-  MyDoubleList: [5.2, 4.5, 7, 9.9]
-  MyListGroup:
-    - IntValueA: 5
-      IntValueB: 42
-    - IntValueA: 7
-      IntValueB: 100
-```
-
-Here, `MyDoubleList` and `MyListGroup` need to specify `List: true` in the corresponding Schema.
-The shorter `[]`-notation was used to assign a list of floating-point values to `MyDoubleList`.
-Nested items `IntValueA` and `IntValueB` of `MyListGroup` are assigned within a list, allowing the specification of these nested items several times.
-
-#### Contracts
-Specifies all Contracts, i.e. repetitive bilateral transactions in between agents.
-Contracts are given as a list.
-We recommend moving Contracts to separate files and to use the `!include` command to integrate them in the scenario.
-
-```yaml
-Contracts:
-  - SenderId: 1
-    ReceiverId: 2
-    ProductName: ProductOfAgent_1
-    FirstDeliveryTime: -25
-    DeliveryIntervalInSteps: 3600
-
-  - SenderId: 2
-    ReceiverId: 1
-    ProductName: ProductOfAgent_2
-    FirstDeliveryTime: -22
-    DeliveryIntervalInSteps: 3600
-    Attributes:
-      ProductAppendix: value
-      TimeOffset: 42
-```
-
-Contract Parameters:
-* `SenderId` unique ID of agent sending the product
-* `ReceiverId` unique ID of agent receiving the product
-* `ProductName` name of the product to be sent
-* `FirstDeliveryTime` first time of delivery in the format "seconds after the January 1st 2000, 00:00:00"
-* `DeliveryIntervalInSteps` delay time in between deliveries in seconds
-* `Attributes` can be set to include additional information as `int`, `float`, `enum` or `dict` data types
-
-##### Definition of Multiple Similar Contracts
-Often, scenarios contain multiple agents of similar type that also have similar chains of contracts.
-Therefore, FAME-Io supports a compact definition of multiple similar contracts.
-`SenderId` and `ReceiverId` can both be lists and support One-to-N, N-to-One and N-to-N relations like in the following example:
-
-```yaml
-Contracts:
-  # effectively 3 similar contracts (0 -> 11), (0 -> 12), (0 -> 13)
-  # with otherwise identical ProductName, FirstDeliveryTime & DeliveryIntervalInSteps
-  - SenderId: 0
-    ReceiverId: [11, 12, 13]
-    ProductName: MyOtherProduct
-    FirstDeliveryTime: 100
-    DeliveryIntervalInSteps: 3600
-
-  # effectively 3 similar contracts (1 -> 10), (2 -> 10), (3 -> 10)
-  # with otherwise identical ProductName, FirstDeliveryTime & DeliveryIntervalInSteps
-  - SenderId: [1, 2, 3]
-    ReceiverId: 10
-    ProductName: MyProduct
-    FirstDeliveryTime: 100
-    DeliveryIntervalInSteps: 3600
-
-  # effectively 3 similar contracts (1 -> 11), (2 -> 12), (3 -> 13)
-  # with otherwise identical ProductName, FirstDeliveryTime & DeliveryIntervalInSteps
-  - SenderId: [1, 2, 3]
-    ReceiverId: [11, 12, 13]
-    ProductName: MyThirdProduct
-    FirstDeliveryTime: 100
-    DeliveryIntervalInSteps: 3600
-```
-
-Combined with YAML anchors complex contract chains can be easily reduced to a minimum of required configuration.
-The following example is equivalent to the previous one and allows a quick extension of contracts to a new couple of agents e.g. (4;14):
-
-```yaml
-Groups:
-  - &agentList1: [1,2,3]
-  - &agentList2: [11,12,13]
-
-Contracts:
-  - SenderId: 0
-    ReceiverId: *agentList2
-    ProductName: MyOtherProduct
-    FirstDeliveryTime: 100
-    DeliveryIntervalInSteps: 3600
-
-  - SenderId: *agentList1
-    ReceiverId: 10
-    ProductName: MyProduct
-    FirstDeliveryTime: 100
-    DeliveryIntervalInSteps: 3600
-
-  - SenderId: *agentList1
-    ReceiverId: *agentList2
-    ProductName: MyThirdProduct
-    FirstDeliveryTime: 100
-    DeliveryIntervalInSteps: 3600
-```
-
-### CSV files
-TIME_SERIES inputs are not directly fed into the Scenario YAML file.
-Instead, TIME_SERIES reference a CSV file that can be stored some place else.
-These CSV files follow a specific structure:
-* They must contain exactly two columns.
-* The first column must be a time stamp in form `YYYY-MM-DD_hh:mm:ss`
-* The second column must be a numerical value (either integer or floating-point)
-* The separator of the two columns is a semicolon
-
-Exemplary content of a valid CSV file:
-
-    2012-01-01_00:00:00;400
-    2013-01-01_00:00:00;720.5
-    2014-01-01_00:00:00;650
-    2015-01-01_00:00:00;99.27772
-    2016-01-01_00:00:00;42
-    2017-01-01_00:00:00;0.1
-
-Please refer also to the detailed article about `TimeStamps` in the [FAME-Wiki](https://gitlab.com/fame-framework/wiki/-/wikis/TimeStamp).
-
-### Split and join multiple YAML files
-The user may include other YAML files into a YAML file to divide the content across files as convenient.
-We explicitly recommend using this feature for the `Schema` and `Contracts` sections.
-Otherwise, the scenario.yaml may become crowded.
-
-#### Command: !Include
-To hint YAML to load the content of another file use `!include "path/relative/to/including/yaml/file.yml"`.
-You can concatenate !include commands and can use !include in the included file as well.
-The path to the included file is always relative to the file using the !include command.
-So with the following file structure
-
-###### file-structure
-```
-a.yaml
-folder/b.yaml
-folder/c.yaml
-folder/deeper_folder/d.yaml
-```
-the following !include commands work
-
-###### in a.yaml
-```
-ToBe: !include "folder/b.yaml"
-OrNot: !include "folder/deeper_folder/d.yaml"
-```
-
-###### in b.yaml
-```
-ThatIs: !include "c.yaml"
-TheQuestion: !include "deeper_folder/d.yaml"
-```
-
-Provided that
-###### in c.yaml
-```
-Or: maybe
-```
-###### d.yaml
-```
-not: "?"
-```
-the resulting file would look like this:
-
-###### THe Joined file a.yaml
-```
-ToBe:
-  ThatIs:
-    Or: maybe
-  TheQuestion:
-    not: "?"
-OrNot:
-  not: "?"
-```
-
-You may also specify absolute file paths if preferred by starting with a "/".
-
-When specifying only a file path, the complete content of the file is assigned to the given key.
-You always need a key to assign the !include command to.
-However, you cannot combine the value returned from !include with other values in the same key.
-Thus, the following combinations do not work:
-###### caveats.yml
-```
-!include "file.yaml" # no key assigned
-
-Key:
-  Some: OtherItem
-  !include "file.yaml" # cannot join with other named items
-
-List:
-  - an: entry
-  !include "file.yaml" # cannot directly join with list items, even if !include returns a list
-```
-
-#### Integrate specific nodes of YAML files
-Instead of including *all* content in the included file, you may also pick a specific node within that file.
-For this use `!include [<relative/path/to/file.yaml>, Path:To:Field:In:Yaml]`.
-Here, `:` is used in the node-specifying string to select a sequence of nodes to follow - with custom depth.
-Consider the following two files:
-
-###### file_to_be_included.yaml
-```yaml
-Set1:
-  Subset1:
-    Key: Value
-Set2:
-  OtherKey: OtherValue
-```
-
-###### including_file.yaml
-```yaml
-- Type: MyAgentWithInputs
-  Id: 1
-  Attributes: !include_node [file_to_be_included.yaml, Set1:Subset1]
-```
-
-Compiling "including_file.yaml" results in
-
-###### resulting_file.yaml
-```yaml
-- Type: MyAgentWithInputs
-  Id: 1
-  Attributes:
-    Key: Value
-```
-
-#### Load multiple files
-Using wildcards in the given path (e.g. "path/to/many/*.yaml") will lead to loading multiple files and assigning their content to the same key.
-You can make use of this feature with or without specifying a node selector.
-However, the elements to be joined across multiple files must be lists.
-These lists are then concatenated into a single list and then assigned to the key in the file calling !include.
-This feature is especially useful for Contracts: You can split the Contracts list into several files and place them in a separate folder.
-Then use !include to re-integrate them into your configuration. An example:
-###### my_contract1.yaml
-```
-Contracts:
- - ContractA
- - ContractB
-```
-###### my_contract2.yaml
-```
-Contracts:
- - ContractC
- - ContractD
- - ContractE
-```
-###### including_file.yaml
-```
-Contracts: [!include "my_contract*.yaml", "Contracts"]
-```
-
-results in
-###### result.yaml
-```
-Contracts:
- - ContractA
- - ContractB
- - ContractC
- - ContractD
- - ContractE
-```
-
-#### Ignoring files
-Files that have their name start with "IGNORE_" are not included with the !include command.
-You will see a debug output to notify you that the file was ignored.
-Use this to temporarily take files out ouf your configuration without deleting or moving them.
-
-## Read FAME results
-Takes an output file in protobuf format of FAME-based applications and converts it into files in CSV format.
-An individual file for each type of Agent is created in a folder named after the protobuf input file.
-Call structure:
-
-    convertFameResults -f <./path/to/protobuf_file.pb>
-
-You may also specify any of the following arguments:
-
-| Command                              | Action                                                                                                                                                                                                                                              |
-|--------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| `-l` or `--log` <option>             | Sets the logging level. Default is `info`. Options are `debug`, `info`, `warning`, `warn`, `error`, `critical`.                                                                                                                                     |
-| `-lf` or `--logfile` <file>          | Sets the logging file. Default is `None`. If `None` is provided, all logs get only printed to the console.                                                                                                                                          |
-| `-a` or `--agents` <list-of-agents>  | If specified, only a subset of agents is extracted from the protobuf file. Default is to extract all agents.                                                                                                                                        |
-| `-o` or `--output`                   | Sets the path to where the generated output files are written to. If not specified, the folder's name is derived from the input file's name. Folder will be created if it does not exist.                                                           |
-| `-se` or `--single-export`           | Enables export of individual agents to individual files, when present. If not present (the default) one file per `AgentType` is created.                                                                                                            |
-| `-m` or `--memory-saving`            | When specified, reduces memory usage profile at the cost of runtime. Use only when necessary.                                                                                                                                                       |
-| `-cc` or `--complex-column` <option> | Defines how to deal with complex indexed output columns (if any). `IGNORE` ignores complex columns. `MERGE` squashes all data from complex columns in one big string entry. `SPLIT` creates a separate file for each complex indexed output column. |
-| `-t` or `--time` <option>            | Option to define conversion of time steps to given format (default=`UTC`) by `-t/--time {UTC, INT, FAME}`                                                                                                                                           |
-
-Additionally, you may merge TimeSteps of a certain range of steps in the output files to
-  i) associate multiple time steps with a common logical time in your simulation
-  ii) reduce number of lines in output files
-
-For this, add the option `merge-times` and specify the arguments as follows:
-
-| Command                   | Action                                                                                   |
-|---------------------------|------------------------------------------------------------------------------------------|
-| `-fp` or `--focal-point`  | TimeStep on which `steps-before` earlier and `steps-after` later TimeSteps are merged on |
-| `-sb` or `--steps-before` | Range of TimeSteps before the `focal-point` they get merged to                           |
-| `-sa` or `--steps-after`  | Range of TimeSteps after the `focal-point` they get merged to                            |
-
-This could look as follows:
-
-    convertFameResults -f <./path/to/protobuf_file.pb> -l debug -lf <path/to/output.log> -a AgentType1 AgentType2 -o myCsvFolder -m -cc SPLIT merge-times -fp 0 -sb 1799 -sa 1800
-
-Make sure that in the range of time steps you specify for merging there is only one value per column in the merged time range.
-If multiple values per column are merged values will get concatenated and might yield unexpected results.
-
-You may also call the conversion script from any Python script with:
-
-```python
-from fameio.scripts.convert_results import run as convert_results
-
-convert_results("./path/to/protobuf_file.pb")
-```
-
-Similar to the console call you may also specify custom run config arguments and add it in a dictionary to the function call.
-
-```python
-from fameio.scripts.convert_results import run as convert_results
-from fameio.source.cli import Options
-
-run_config = {Options.LOG_LEVEL: "info",
-              Options.LOG_FILE: "scenario.log",
-              Options.OUTPUT: "Output",
-              Options.AGENT_LIST: ['AgentType1', 'AgentType2'],
-              Options.MEMORY_SAVING: False,
-              Options.SINGLE_AGENT_EXPORT: False,
-              Options.RESOLVE_COMPLEX_FIELD: "SPLIT",
-              Options.TIME: "INT",
-              Options.TIME_MERGING: {},
-              }
-
-convert_results("./path/to/protobuf_file.pb", run_config)
-```
-
-## Cite FAME-Io
-If you use FAME-Io for academic work, please cite as follows.
-
-Bibtex entry:
-```
-@article{fameio2023joss,
-  author  = {Felix Nitsch and Christoph Schimeczek and Ulrich Frey and Benjamin Fuchs},
-  title   = {FAME-Io: Configuration tools for complex agent-based simulations},
-  journal = {Journal of Open Source Software},
-  year    = {2023},
-  doi     = {doi: https://doi.org/10.21105/joss.04958}
-}
-```
-
-## Available Support
-This is a purely scientific project by (at the moment) one research group. 
-Thus, there is no paid technical support available.
-However, we will give our best to answer your questions and provide support.
-
-If you experience any trouble with FAME-Io, you may contact the developers via [fame@dlr.de](mailto:fame@dlr.de).
-Please report bugs and make feature requests by filing issues following the provided templates (see also [Contribute](#Contribute)).
-For substantial enhancements, we recommend that you contact us via [fame@dlr.de](mailto:fame@dlr.de) for working together on the code in common projects or towards common publications and thus further develop FAME-Io.
-
-# Contribute
-Please read the Contributors License Agreement `cla.md`, sign it and send it to [`fame@dlr.de`](mailto:fame@dlr.de) before contributing.
-
-You will also find templates for [bug reports](https://gitlab.com/fame-framework/fame-io/-/blob/main/.gitlab/issue_templates/bug_report.md),
-[feature requests](https://gitlab.com/fame-framework/fame-io/-/blob/main/.gitlab/issue_templates/feature_request.md), and 
-[pull requests](https://gitlab.com/fame-framework/fame-io/-/blob/main/.gitlab/issue_templates/pull_request.md).
-
-We kindly ask you to read the Contributors License Agreement `cla.md`, sign it, and send it to [`fame@dlr.de`](mailto:fame@dlr.de) before contributing. Please see our [conventions of contribution](https://gitlab.com/fame-framework/wiki/-/wikis/developers/contribute/Conventions) which are described in the Wiki.
-
-## Testing changes locally 
-
-Once some changes have been performed on the local git clone, use the following command to override your local installation with your modified copy in order to test the result:
-
-```bash
-python3 setup.py bdist_wheel && pip3 install --force-reinstall --no-dependencies ./dist/*.whl
-```
-
-## Code style
-
-We use the code formatting library [`black`](https://pypi.org/project/black/).
-The maximum line length is defined as 120 characters. 
-Therefore, before committing, run `black --line-length 120 .`
-
-## Pre-Commit hooks
-
-FAME-Io uses several pre-commit hooks to ensure high code quality.
-To use them, install `dev` packages and then initialise pre-commit in FAME-Io's base folder:
-
-```
-    pip install fameio[dev]
-    pre-commit install -t pre-commit -t pre-push
-```
+Metadata-Version: 2.1
+Name: fameio
+Version: 2.0.0
+Summary: Python scripts for operation of FAME models
+Home-page: https://gitlab.com/fame-framework/wiki/-/wikis/home
+License: Apache-2.0
+Keywords: FAME,fameio,agent-based modelling,energy systems
+Author: Felix Nitsch
+Author-email: fame@dlr.de
+Maintainer: Felix Nitsch
+Maintainer-email: fame@dlr.de
+Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Scientific/Engineering
+Requires-Dist: fameprotobuf (>=1.4.0,<2.0.0)
+Requires-Dist: pandas (>=1.0,<3.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
+Project-URL: Repository, https://gitlab.com/fame-framework/fame-io/
+Description-Content-Type: text/markdown
+
+<!-- SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
+
+SPDX-License-Identifier: Apache-2.0 -->
+[![PyPI version](https://badge.fury.io/py/fameio.svg)](https://badge.fury.io/py/fameio)
+[![JOSS](https://joss.theoj.org/papers/10.21105/joss.04958/status.svg)](https://doi.org/10.21105/joss.04958)
+[![Zenodo](https://zenodo.org/badge/DOI/10.5281/zenodo.4314337.svg)](https://doi.org/10.5281/zenodo.4314337)
+[![PyPI license](https://img.shields.io/pypi/l/fameio.svg)](https://badge.fury.io/py/fameio)
+[![pipeline status](https://gitlab.com/fame-framework/fame-io/badges/main/pipeline.svg)](https://gitlab.com/fame-framework/fame-io/commits/main)
+[![coverage report](https://gitlab.com/fame-framework/fame-io/badges/main/coverage.svg)](https://gitlab.com/fame-framework/fame-io/-/commits/main)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![REUSE status](https://api.reuse.software/badge/gitlab.com/fame-framework/fame-io)](https://api.reuse.software/info/gitlab.com/fame-framework/fame-io)
+[![Common Changelog](https://common-changelog.org/badge.svg)](https://common-changelog.org)
+![GitLab last commit](https://img.shields.io/gitlab/last-commit/fame-framework%2Ffame-io)
+![GitLab closed issues by-label](https://img.shields.io/gitlab/issues/closed/fame-framework%2Ffame-io)
+
+
+# FAME-Io
+Python scripts for FAME models, generation of protobuf input files and conversion of protobuf output files.
+Please visit the [FAME-Wiki](https://gitlab.com/fame-framework/wiki/-/wikis/home) to get an explanation of FAME and its components.
+
+# Installation
+We recommend installing `fameio` using PyPI:
+
+    pip install fameio
+
+You may also use `pipx`. For detailed information please refer to the official `pipx` [documentation](https://github.com/pypa/pipx).
+
+    pipx install fameio
+
+`fameio` is currently developed and tested for Python 3.8 or higher.
+See the `pyproject.toml` for a complete listing of dependencies.
+
+# Usage
+FAME-Io currently offers two main scripts `makeFameRunConfig` and `convertFameResults`.
+Both are automatically installed with the package.
+The first one creates a protobuf file for FAME applications using YAML definition files and CSV files.
+The latter one reads output files from FAME applications in protobuf format and converts them to CSV files.
+
+You may use the [example data](https://gitlab.com/dlr-ve/esy/amiris/examples) provided for the [AMIRIS](https://gitlab.com/dlr-ve/esy/amiris/amiris) model which can be used to simulate electricity markets in [Germany](https://gitlab.com/dlr-ve/esy/amiris/examples/-/tree/main/Germany2019), [Austria](https://gitlab.com/dlr-ve/esy/amiris/examples/-/tree/main/Austria2019), and a simple [proof-of-concept model](https://gitlab.com/dlr-ve/esy/amiris/examples/-/tree/main/Simple).
+
+## Make a FAME run configuration
+Digests configuration files in YAML format, combines them with CSV data files and creates a single input file for FAME applications in protobuf format.
+Call structure:
+
+    makeFameRunConfig -f <path/to/scenario.yaml>
+
+You may also specify any of the following arguments:
+
+| Command              | Action                                                                                                          |
+|----------------------|-----------------------------------------------------------------------------------------------------------------|
+| `-l` or `--log`      | Sets the logging level. Default is `info`. Options are `debug`, `info`, `warning`, `warn`, `error`, `critical`. |
+| `-lf` or `--logfile` | Sets the logging file. Default is `None`. If `None` is provided, all logs get only printed to the console.      |
+| `-o` or `--output`   | Sets the path of the compiled protobuf output file. Default is `config.pb`.                                     |
+
+This could look as follows:
+
+    makeFameRunConfig -f <path/to/scenario.yaml> -l debug -lf <path/to/scenario.log> -o <path/to/config.pb>
+
+You may also call the configuration builder from any Python script with
+
+```python
+from fameio.scripts.make_config import Options, run as make_config
+
+make_config({Options.FILE: "path/to/scenario.yaml", })
+```
+
+Similar to the console call you may also specify custom run config arguments and add it in a dictionary to the function call.
+
+```python
+from fameio.scripts.make_config import Options, run as make_config
+
+run_config = {Options.FILE: "path/to/scenario.yaml",
+              Options.LOG_LEVEL: "info",
+              Options.OUTPUT: "output.pb",
+              Options.LOG_FILE: "scenario.log",
+              }
+
+make_config(run_config)
+```
+
+You can also use the associated argument parser, to extract the run_config dynamically from a string:
+
+```python
+from fameio.scripts.make_config import Options, run as make_config
+from fameio.source.cli.make_config import handle_args
+
+my_defaults = {Options.FILE: "path/to/scenario.yaml",
+                 Options.LOG_LEVEL: "info",
+                 Options.OUTPUT: "output.pb",
+                 Options.LOG_FILE: "scenario.log",
+                 }
+my_arg_string = ['-f', 'my/other/scenario.yaml', '-l', 'error']
+
+run_config = handle_args(my_arg_string, my_defaults)
+make_config(run_config)
+```
+
+### Scenario YAML
+The "scenario.yaml" file contains all configuration options for a FAME-based simulation.
+It consists of the sections `Schema`, `GeneralProperties`, `Agents` and `Contracts`, all of them described below.
+
+#### Schema
+The Schema is used to validate the inputs of the "scenario.yaml".
+Since the Schema should be valid across multiple scenarios, it is recommended to defined it in a separate file and include the file here.
+
+Currently, the schema specifies:
+* which type of Agents can be created
+* what type of input attributes an Agent uses
+* what type of Products an Agent can send in Contracts.
+
+The Schema consists of the sections `Header` and `AgentTypes`.
+
+##### Header
+Scientific applications often evolve, and so do their required input parameters.
+Therefore, the header specifies information what FAME-based application the schema is corresponding to.
+In this way a schema.yaml is tied to a specific version an application, ensuring a match between the inputs required by
+the application, and those provided by the files created with FAME-Io.
+
+```yaml
+Header:
+  Project: MyProjectName
+  RepoUrl: https://mygithosting.com/myProject
+  CommitHash: abc123
+```
+
+* `Project` name of your project / FAME-based application
+* `RepoUrl` URL of your project
+* `CommitHash` hash of the commit / version of your project
+
+##### AgentTypes
+Here, each type of agent that can be created in your FAME-based application is listed, its attributes and its available Products for Contracts.
+The structure of this section
+
+```yaml
+AgentTypes:
+  MyAgentType:
+    Attributes:
+      MyAttribute:
+        ...
+      MyOtherAttribute:
+        ...
+    Products: [ 'Product1', 'Product2', 'Product3' ]
+  MyOtherAgentWithoutProductsOrAttributes:
+```
+
+* `MyAgentType` Java's simple class name of the Agent type
+* `Attributes` indicates that beginning of the attribute definition section for this Agent type
+* `MyAttribute` Name of an attribute as specified in the corresponding Java source code of this Agent type (annotated with "@Input")
+* `MyOtherAttribute` Name of another attribute derived from Java source code
+* `Products` list of Products that this Agent can send in Contracts; derived from Java source code of this Agent type (annotated with "@Product")
+* `MyOtherAgentWithoutProductsOrAttributes` an Agent type that requires neither Attributes nor Products
+
+Both Attributes and Products are optional - there could be useful Agents that require neither of them.
+In the above example attribute definition was not shown (indicated by `...`).
+The next example provides details on how to define an attribute:
+
+```yaml
+MySimpleAttribute:
+  AttributeType: enum
+  Mandatory: true
+  List: false
+  Values: [ 'AllowedValue1', 'AllowedValue2' ]
+  Default: 'AllowedValue1'
+  Help: 'My help text'
+
+MyComplexAttribute:
+  AttributeType: block
+  NestedAttributes:
+    InnerAttributeA:
+      AttributeType: integer
+    InnerAttributeB:
+      AttributeType: double
+```
+
+* `MySimpleAttribute`, `MyDoubleList`, `MyComplexAttribute` Names of the attributes as specified in the Java enum annotated with "@Input"
+* `AttributeType` (required) data type of the attribute; see options in table below
+* `Mandatory` (optional - true by default) if true: the attribute is required for this agent and validation will fail if the attribute is missing in the scenario **and** no default is provided
+* `List` (optional - false by default)
+    * `AttributeType: time_series` cannot be true
+    * `AttributeType: block`
+        * if true: any nested element in the scenario must be part of a list element and thus can appear multiple times
+        * if false: any nested element in the scenario can only appear once
+    * any other AttributeType: the attribute is interpreted as list, i.e. multiple values can be assigned to this attribute in the scenario
+* `NestedAttributes` (required only if `AttributeType: block`, otherwise disallowed) starts an inner Attribute definition block - defined Attributes are sub-elements of `MyComplexAttribute`
+* `Values` (optional - None by default): if present defines a list of allowed values for this attribute
+* `Default` (optional - None by default): if present defines a default value to be used in case the scenario does not specify it
+* `Help` (optional - None by default): if present defines a help text to you attribute
+
+| AttributeType | value                                                                                                                   |
+|---------------|-------------------------------------------------------------------------------------------------------------------------|
+| `integer`     | a 32-bit integer value                                                                                                  |
+| `double`      | a 64-bit floating-point value (integers also allowed)                                                                   |
+| `long`        | a 64-bit integer value                                                                                                  |
+| `time_stamp`  | either a FAME time stamp string or 64-bit integer value                                                                 |
+| `string`      | any string                                                                                                              |
+| `enum`        | any string, however, usually tied to a set of allowed `Values`                                                          |
+| `time_series` | either a path to a .csv-file or a single 64-bit floating-point value; does not support `List: true`                     |
+| `block`       | this attribute has no value of its own but hosts a group of nested Attributes; implies `NestedAttributes` to be defined |
+
+#### GeneralProperties
+Specifies FAME-specific properties of the simulation. Structure:
+
+```yaml
+GeneralProperties:
+  RunId: 1
+  Simulation:
+    StartTime: 2011-12-31_23:58:00
+    StopTime: 2012-12-30_23:58:00
+    RandomSeed: 1
+  Output:
+    Interval: 100
+    Process: 0
+```
+
+Parameters:
+* `RunId` an ID that can be given to the simulation; use at your discretion
+* `StartTime` time stamp in the format YYYY-MM-DD_hh:mm:ss; first moment of the simulation.
+* `StopTime` time stamp in the format YYYY-MM-DD_hh:mm:ss; last moment of the simulation - i.e. simulation terminates
+  after passing that time stamp
+* `RandomSeed` seed to initialise random number generation; each value leads to a unique series of random numbers.
+* `Interval` number of simulation ticks in between write-to-disk events; may be used for performance optimisations;
+* `Process` id of process that performs write-to-disk operations; leave at 0 to be compatible with single-processes;
+
+#### Agents
+Specifies all Agents to be created in the simulation in a list. Each Agent has its own entry.
+Structure:
+
+```yaml
+Agents:
+  - Type: MyAgentWithInputs
+    Id: 1
+    Attributes:
+      MyEnum: SAME_SHARES
+      MyInteger: 2
+      MyDouble: 4.2
+      MyTimeSeries: "./path/to/time_series.csv"
+
+  - Type: MyAgentWithoutInputs
+    Id: 2
+```
+
+Agent Parameters:
+* `Type` Mandatory; Java's simple class name of the agent to be created
+* `Id` Mandatory; simulation-unique id of this agent; if two agents have the same ID, the configuration process will
+  stop.
+* `Attributes` Optional; if the agent has any attributes, specify them here in the format "AttributeName: value"; please
+  see attribute table above
+
+The specified `Attributes` for each agent must match the specified `Attributes` options in the linked Schema (see above).
+For better structure and readability of the `scenario.yaml`, `Attributes` may also be specified in a nested way as demonstrated below.
+
+```yaml
+Agents:
+  - Type: MyAgentWithInputs
+    Id: 1
+    Attributes:
+      Parent:
+        MyEnum: SAME_SHARES
+        MyInteger: 2
+      Parent2:
+        MyDouble: 4.2
+        Child:
+          MyTimeSeries: "./path/to/time_series.csv"
+```
+
+In case Attributes are defined with `List: true` option, lists are assigned to an Attribute or Group:
+
+```yaml
+Attributes:
+  MyDoubleList: [ 5.2, 4.5, 7, 9.9 ]
+  MyListGroup:
+    - IntValueA: 5
+      IntValueB: 42
+    - IntValueA: 7
+      IntValueB: 100
+```
+
+Here, `MyDoubleList` and `MyListGroup` need to specify `List: true` in the corresponding Schema.
+The shorter `[]`-notation was used to assign a list of floating-point values to `MyDoubleList`.
+Nested items `IntValueA` and `IntValueB` of `MyListGroup` are assigned within a list, allowing the specification of these nested items several times.
+
+#### Contracts
+Specifies all Contracts, i.e. repetitive bilateral transactions in between agents.
+Contracts are given as a list.
+We recommend moving Contracts to separate files and to use the `!include` command to integrate them in the scenario.
+
+```yaml
+Contracts:
+  - SenderId: 1
+    ReceiverId: 2
+    ProductName: ProductOfAgent_1
+    FirstDeliveryTime: -25
+    DeliveryIntervalInSteps: 3600
+
+  - SenderId: 2
+    ReceiverId: 1
+    ProductName: ProductOfAgent_2
+    FirstDeliveryTime: -22
+    DeliveryIntervalInSteps: 3600
+    Attributes:
+      ProductAppendix: value
+      TimeOffset: 42
+```
+
+Contract Parameters:
+* `SenderId` unique ID of agent sending the product
+* `ReceiverId` unique ID of agent receiving the product
+* `ProductName` name of the product to be sent
+* `FirstDeliveryTime` first time of delivery in the format "seconds after the January 1st 2000, 00:00:00"
+* `DeliveryIntervalInSteps` delay time in between deliveries in seconds
+* `Attributes` can be set to include additional information as `int`, `float`, `enum` or `dict` data types
+
+##### Definition of Multiple Similar Contracts
+Often, scenarios contain multiple agents of similar type that also have similar chains of contracts.
+Therefore, FAME-Io supports a compact definition of multiple similar contracts.
+`SenderId` and `ReceiverId` can both be lists and support One-to-N, N-to-One and N-to-N relations like in the following example:
+
+```yaml
+Contracts:
+  # effectively 3 similar contracts (0 -> 11), (0 -> 12), (0 -> 13)
+  # with otherwise identical ProductName, FirstDeliveryTime & DeliveryIntervalInSteps
+  - SenderId: 0
+    ReceiverId: [ 11, 12, 13 ]
+    ProductName: MyOtherProduct
+    FirstDeliveryTime: 100
+    DeliveryIntervalInSteps: 3600
+
+  # effectively 3 similar contracts (1 -> 10), (2 -> 10), (3 -> 10)
+  # with otherwise identical ProductName, FirstDeliveryTime & DeliveryIntervalInSteps
+  - SenderId: [ 1, 2, 3 ]
+    ReceiverId: 10
+    ProductName: MyProduct
+    FirstDeliveryTime: 100
+    DeliveryIntervalInSteps: 3600
+
+  # effectively 3 similar contracts (1 -> 11), (2 -> 12), (3 -> 13)
+  # with otherwise identical ProductName, FirstDeliveryTime & DeliveryIntervalInSteps
+  - SenderId: [ 1, 2, 3 ]
+    ReceiverId: [ 11, 12, 13 ]
+    ProductName: MyThirdProduct
+    FirstDeliveryTime: 100
+    DeliveryIntervalInSteps: 3600
+```
+
+Combined with YAML anchors complex contract chains can be easily reduced to a minimum of required configuration.
+The following example is equivalent to the previous one and allows a quick extension of contracts to a new couple of agents e.g. (4;14):
+
+```yaml
+Groups:
+  - &agentList1: [ 1,2,3 ]
+  - &agentList2: [ 11,12,13 ]
+
+Contracts:
+  - SenderId: 0
+    ReceiverId: *agentList2
+    ProductName: MyOtherProduct
+    FirstDeliveryTime: 100
+    DeliveryIntervalInSteps: 3600
+
+  - SenderId: *agentList1
+    ReceiverId: 10
+    ProductName: MyProduct
+    FirstDeliveryTime: 100
+    DeliveryIntervalInSteps: 3600
+
+  - SenderId: *agentList1
+    ReceiverId: *agentList2
+    ProductName: MyThirdProduct
+    FirstDeliveryTime: 100
+    DeliveryIntervalInSteps: 3600
+```
+
+### CSV files
+TIME_SERIES inputs are not directly fed into the Scenario YAML file.
+Instead, TIME_SERIES reference a CSV file that can be stored some place else.
+These CSV files follow a specific structure:
+* They must contain exactly two columns.
+* The first column must be a time stamp in form `YYYY-MM-DD_hh:mm:ss`
+* The second column must be a numerical value (either integer or floating-point)
+* The separator of the two columns is a semicolon
+* The data must **not** have headers, except for comments marked with `#`
+
+You may add comments using `#`.
+Exemplary content of a valid CSV file:
+
+    # If you want an optional header, you must use a comment
+    2012-01-01_00:00:00;400
+    2013-01-01_00:00:00;720.5
+    2014-01-01_00:00:00;650
+    2015-01-01_00:00:00;99.27772
+    2016-01-01_00:00:00;42  # optional comment on this particular data point
+    2017-01-01_00:00:00;0.1
+
+Please refer also to the detailed article about `TimeStamps` in the [FAME-Wiki](https://gitlab.com/fame-framework/wiki/-/wikis/TimeStamp).
+
+### Split and join multiple YAML files
+The user may include other YAML files into a YAML file to divide the content across files as convenient.
+We explicitly recommend using this feature for the `Schema` and `Contracts` sections.
+Otherwise, the scenario.yaml may become crowded.
+
+#### Command: !Include
+To hint YAML to load the content of another file use `!include "path/relative/to/including/yaml/file.yml"`.
+You can concatenate !include commands and can use !include in the included file as well.
+The path to the included file is always relative to the file using the !include command.
+So with the following file structure
+
+###### file-structure
+```
+a.yaml
+folder/b.yaml
+folder/c.yaml
+folder/deeper_folder/d.yaml
+```
+
+the following !include commands work
+
+###### in a.yaml
+```
+ToBe: !include "folder/b.yaml"
+OrNot: !include "folder/deeper_folder/d.yaml"
+```
+
+###### in b.yaml
+```
+ThatIs: !include "c.yaml"
+TheQuestion: !include "deeper_folder/d.yaml"
+```
+
+Provided that
+###### in c.yaml
+```
+Or: maybe
+```
+
+###### d.yaml
+```
+not: "?"
+```
+
+the resulting file would look like this:
+
+###### THe Joined file a.yaml
+```
+ToBe:
+  ThatIs:
+    Or: maybe
+  TheQuestion:
+    not: "?"
+OrNot:
+  not: "?"
+```
+
+You may also specify absolute file paths if preferred by starting with a "/".
+
+When specifying only a file path, the complete content of the file is assigned to the given key.
+You always need a key to assign the !include command to.
+However, you cannot combine the value returned from !include with other values in the same key.
+Thus, the following combinations do not work:
+
+###### caveats.yml
+```
+!include "file.yaml" # no key assigned
+
+Key:
+  Some: OtherItem
+  !include "file.yaml" # cannot join with other named items
+
+List:
+  - an: entry
+  !include "file.yaml" # cannot directly join with list items, even if !include returns a list
+```
+
+#### Integrate specific nodes of YAML files
+Instead of including *all* content in the included file, you may also pick a specific node within that file.
+For this use `!include [<relative/path/to/file.yaml>, Path:To:Field:In:Yaml]`.
+Here, `:` is used in the node-specifying string to select a sequence of nodes to follow - with custom depth.
+Consider the following two files:
+
+###### file_to_be_included.yaml
+```yaml
+Set1:
+  Subset1:
+    Key: Value
+Set2:
+  OtherKey: OtherValue
+```
+
+###### including_file.yaml
+```yaml
+- Type: MyAgentWithInputs
+  Id: 1
+  Attributes: !include_node [ file_to_be_included.yaml, Set1:Subset1 ]
+```
+
+Compiling "including_file.yaml" results in
+
+###### resulting_file.yaml
+```yaml
+- Type: MyAgentWithInputs
+  Id: 1
+  Attributes:
+    Key: Value
+```
+
+#### Load multiple files
+Using wildcards in the given path (e.g. "path/to/many/*.yaml") will lead to loading multiple files and assigning their content to the same key.
+You can make use of this feature with or without specifying a node selector.
+However, the elements to be joined across multiple files must be lists.
+These lists are then concatenated into a single list and then assigned to the key in the file calling !include.
+This feature is especially useful for Contracts: You can split the Contracts list into several files and place them in a separate folder.
+Then use !include to re-integrate them into your configuration. An example:
+
+###### my_contract1.yaml
+```
+Contracts:
+ - ContractA
+ - ContractB
+```
+
+###### my_contract2.yaml
+```
+Contracts:
+ - ContractC
+ - ContractD
+ - ContractE
+```
+
+###### including_file.yaml
+```
+Contracts: [!include "my_contract*.yaml", "Contracts"]
+```
+
+results in
+
+###### result.yaml
+```
+Contracts:
+ - ContractA
+ - ContractB
+ - ContractC
+ - ContractD
+ - ContractE
+```
+
+#### Ignoring files
+Files that have their name start with "IGNORE_" are not included with the !include command.
+You will see a debug output to notify you that the file was ignored.
+Use this to temporarily take files out ouf your configuration without deleting or moving them.
+
+## Read FAME results
+Takes an output file in protobuf format of FAME-based applications and converts it into files in CSV format.
+An individual file for each type of Agent is created in a folder named after the protobuf input file.
+Call structure:
+
+    convertFameResults -f <./path/to/protobuf_file.pb>
+
+You may also specify any of the following arguments:
+
+| Command                                     | Action                                                                                                                                                                                                                                              |
+|---------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `-l` or `--log` <option>                    | Sets the logging level. Default is `info`. Options are `debug`, `info`, `warning`, `warn`, `error`, `critical`.                                                                                                                                     |
+| `-lf` or `--logfile` <file>                 | Sets the logging file. Default is `None`. If `None` is provided, all logs get only printed to the console.                                                                                                                                          |
+| `-a` or `--agents` <list-of-agents>         | If specified, only a subset of agents is extracted from the protobuf file. Default is to extract all agents.                                                                                                                                        |
+| `-o` or `--output`                          | Sets the path to where the generated output files are written to. If not specified, the folder's name is derived from the input file's name. Folder will be created if it does not exist.                                                           |
+| `-se` or `--single-export`                  | Enables export of individual agents to individual files, when present. If not present (the default) one file per `AgentType` is created.                                                                                                            |
+| `-m` or `--memory-saving`                   | When specified, reduces memory usage profile at the cost of runtime. Use only when necessary.                                                                                                                                                       |
+| `-cc` or `--complex-column` <option>        | Defines how to deal with complex indexed output columns (if any). `IGNORE` ignores complex columns. `MERGE` squashes all data from complex columns in one big string entry. `SPLIT` creates a separate file for each complex indexed output column. |
+| `-t` or `--time` <option>                   | Option to define conversion of time steps to given format (default=`UTC`) by `-t/--time {UTC, INT, FAME}`                                                                                                                                           |
+| `--input-recovery` or `--no-input-recovery` | If True, all input data are recovered as well as the outputs (default=False).                                                                                                                                                                       |
+
+Additionally, you may merge TimeSteps of a certain range of steps in the output files to
+i) associate multiple time steps with a common logical time in your simulation
+ii) reduce number of lines in output files
+
+For this, add the option `merge-times` and specify the arguments as follows:
+
+| Command                   | Action                                                                                   |
+|---------------------------|------------------------------------------------------------------------------------------|
+| `-fp` or `--focal-point`  | TimeStep on which `steps-before` earlier and `steps-after` later TimeSteps are merged on |
+| `-sb` or `--steps-before` | Range of TimeSteps before the `focal-point` they get merged to                           |
+| `-sa` or `--steps-after`  | Range of TimeSteps after the `focal-point` they get merged to                            |
+
+This could look as follows:
+
+    convertFameResults -f <./path/to/protobuf_file.pb> -l debug -lf <path/to/output.log> -a AgentType1 AgentType2 -o myCsvFolder -m -cc SPLIT merge-times -fp 0 -sb 1799 -sa 1800
+
+Make sure that in the range of time steps you specify for merging there is only one value per column in the merged time range.
+If multiple values per column are merged values will get concatenated and might yield unexpected results.
+
+You may also call the conversion script from any Python script with:
+
+```python
+from fameio.scripts.convert_results import Options, run as convert_results
+
+convert_results({Options.FILE: "./path/to/protobuf_file.pb"})
+```
+
+Similar to the console call you may also specify custom run config arguments and add it in a dictionary to the function call.
+
+```python
+from fameio.scripts.convert_results import Options, run as convert_results
+
+run_config = {Options.FILE: "./path/to/protobuf_file.pb",
+              Options.LOG_LEVEL: "info",
+              Options.LOG_FILE: "scenario.log",
+              Options.OUTPUT: "Output",
+              Options.AGENT_LIST: ['AgentType1', 'AgentType2'],
+              Options.MEMORY_SAVING: False,
+              Options.SINGLE_AGENT_EXPORT: False,
+              Options.RESOLVE_COMPLEX_FIELD: "SPLIT",
+              Options.TIME: "INT",
+              Options.TIME_MERGING: {},
+              }
+
+convert_results(run_config)
+```
+
+You can also use the associated argument parser, to extract the run_config dynamically from a string:
+
+```python
+from fameio.scripts.convert_results import Options, run as convert_results
+from fameio.source.cli.convert_results import handle_args
+
+my_defaults = {Options.FILE: "./path/to/protobuf_file.pb",
+               Options.LOG_LEVEL: "info",
+               Options.LOG_FILE: "scenario.log",
+               Options.OUTPUT: "Output",
+               Options.AGENT_LIST: ['AgentType1', 'AgentType2'],
+               Options.MEMORY_SAVING: False,
+               Options.SINGLE_AGENT_EXPORT: False,
+               Options.RESOLVE_COMPLEX_FIELD: "SPLIT",
+               Options.TIME: "INT",
+               Options.TIME_MERGING: {},
+               }
+my_arg_string = ['-f', 'my/other/scenario.yaml', '-l', 'error']
+
+run_config = handle_args(my_arg_string, my_defaults)
+convert_results(run_config)
+```
+
+## Cite FAME-Io
+If you use FAME-Io for academic work, please cite as follows.
+
+Bibtex entry:
+
+```
+@article{fameio2023joss,
+  author  = {Felix Nitsch and Christoph Schimeczek and Ulrich Frey and Benjamin Fuchs},
+  title   = {FAME-Io: Configuration tools for complex agent-based simulations},
+  journal = {Journal of Open Source Software},
+  year    = {2023},
+  doi     = {doi: https://doi.org/10.21105/joss.04958}
+}
+```
+
+## Available Support
+This is a purely scientific project by (at the moment) one research group.
+Thus, there is no paid technical support available.
+However, we will give our best to answer your questions and provide support.
+
+If you experience any trouble with FAME-Io, you may contact the developers via [fame@dlr.de](mailto:fame@dlr.de).
+Please report bugs and make feature requests by filing issues following the provided templates (see also [Contribute](CONTRIBUTING.md)).
+For substantial enhancements, we recommend that you contact us via [fame@dlr.de](mailto:fame@dlr.de) for working
+together on the code in common projects or towards common publications and thus further develop FAME-Io.
+
```

### Comparing `fameio-1.8.2/src/fameio/source/cli.py` & `fameio-2.0.0/src/fameio/source/cli/parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,216 +1,163 @@
-# SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
+# SPDX-FileCopyrightText: 2024 German Aerospace Center <fame@dlr.de>
 #
 # SPDX-License-Identifier: Apache-2.0
-
-import argparse
 import copy
-from enum import Enum, auto
+from argparse import ArgumentParser, ArgumentTypeError, BooleanOptionalAction, Namespace
+from enum import Enum
 from pathlib import Path
-from typing import Optional, Dict, Any, List, Tuple
+from typing import Optional, Dict, Any, List, Union
 
+from fameio.source.cli.options import MergingOptions, TimeOptions, ResolveOptions, Options
 from fameio.source.logs import LOG_LEVELS
 
-ERR_NEGATIVE_INT = "Given value `{}` is not a non-negative int."
-
-
-class Options(Enum):
-    """Specifies command line configuration options"""
-
-    FILE = auto()
-    LOG_LEVEL = auto()
-    LOG_FILE = auto()
-    OUTPUT = auto()
-    AGENT_LIST = auto()
-    SINGLE_AGENT_EXPORT = auto()
-    MEMORY_SAVING = auto()
-    RESOLVE_COMPLEX_FIELD = auto()
-    TIME = auto()
-    TIME_MERGING = auto()
-
-
-class TimeOptions(Enum):
-    """Specifies options for conversion of time in output"""
-
-    INT = auto()
-    UTC = auto()
-    FAME = auto()
-
-
-class ResolveOptions(Enum):
-    """Specifies options for resolving complex fields in output files"""
-
-    IGNORE = auto()
-    SPLIT = auto()
-    MERGE = auto()
-
-
-class MergingOptions(Enum):
-    """Specifies options for merging TimeSteps"""
+_ERR_NEGATIVE_INT = "Given value `{}` is not a non-negative int."
 
-    FOCAL_POINT = auto()
-    STEPS_BEFORE = auto()
-    STEPS_AFTER = auto()
+_OPTION_ARGUMENT_NAME: Dict[str, Union[Options, Dict]] = {
+    "file": Options.FILE,
+    "log": Options.LOG_LEVEL,
+    "logfile": Options.LOG_FILE,
+    "output": Options.OUTPUT,
+    "agents": Options.AGENT_LIST,
+    "single_export": Options.SINGLE_AGENT_EXPORT,
+    "memory_saving": Options.MEMORY_SAVING,
+    "time": Options.TIME,
+    "input_recovery": Options.INPUT_RECOVERY,
+    "complex_column": Options.RESOLVE_COMPLEX_FIELD,
+    "time_merging": {
+        "name": Options.TIME_MERGING,
+        "inner_elements": {
+            "focal_point": MergingOptions.FOCAL_POINT,
+            "steps_before": MergingOptions.STEPS_BEFORE,
+            "steps_after": MergingOptions.STEPS_AFTER,
+        },
+    },
+}
 
 
-def arg_handling_make_config(args: List[str], defaults: Dict) -> Tuple[str, Dict]:
-    """Handles command line arguments and returns `input_file` and `run_config` for make_config script"""
-    parser = argparse.ArgumentParser()
-
-    add_file_argument(parser, "provide path to configuration file")
-    add_log_level_argument(parser, defaults[Options.LOG_LEVEL])
-    add_logfile_argument(parser)
-    add_output_argument(parser, defaults[Options.OUTPUT], "provide file-path for the file to generate")
-
-    args = parser.parse_args(args)
-    run_config = {
-        Options.LOG_LEVEL: args.log,
-        Options.LOG_FILE: args.logfile,
-        Options.OUTPUT: args.output,
-    }
-    return args.file, run_config
-
-
-def arg_handling_convert_results(args: List[str], defaults: Dict) -> Tuple[str, Dict]:
-    """Handles command line arguments and returns `input_file` and `run_config` for convert_results script"""
-    parser = argparse.ArgumentParser()
-
-    add_file_argument(parser, "provide path to protobuf file")
-    add_log_level_argument(parser, defaults[Options.LOG_LEVEL])
-    add_logfile_argument(parser)
-    add_output_argument(
-        parser,
-        defaults[Options.OUTPUT],
-        "provide path to folder to store output .csv files",
-    )
-    add_select_agents_argument(parser)
-    add_single_export_argument(parser, defaults[Options.SINGLE_AGENT_EXPORT])
-    add_memory_saving_argument(parser, defaults[Options.MEMORY_SAVING])
-    add_resolve_complex_argument(parser, defaults[Options.RESOLVE_COMPLEX_FIELD])
-    add_time_argument(parser, defaults[Options.TIME])
-    add_merge_time_parser(parser)
-
-    args = parser.parse_args(args)
-
-    run_config = {
-        Options.LOG_LEVEL: args.log,
-        Options.LOG_FILE: args.logfile,
-        Options.OUTPUT: args.output,
-        Options.AGENT_LIST: args.agents,
-        Options.SINGLE_AGENT_EXPORT: args.single_export,
-        Options.MEMORY_SAVING: args.memory_saving,
-        Options.RESOLVE_COMPLEX_FIELD: ResolveOptions[args.complex_column],
-        Options.TIME: args.time,
-        Options.TIME_MERGING: get_merging_args(args),
-    }
-    return args.file, run_config
-
+def add_file_argument(parser: ArgumentParser, default: Optional[Path], help_text: str) -> None:
+    """
+    Adds 'file' argument to the provided `parser` with the provided `help_text`.
+    If a default is not specified, the argument is required (optional otherwise)
 
-def add_file_argument(parser: argparse.ArgumentParser, help_text: str) -> None:
-    """Adds required 'file' argument to the provided `parser` with the provided `help_text`"""
-    parser.add_argument("-f", "--file", type=Path, required=True, help=help_text)
+    Args:
+        parser: to add the argument to
+        default: optional, if it is a valid Path, it is added as default and the argument becomes optional
+        help_text: to be displayed
+    """
+    if default is not None and isinstance(default, (Path, str)):
+        parser.add_argument("-f", "--file", type=Path, required=False, default=default, help=help_text)
+    else:
+        parser.add_argument("-f", "--file", type=Path, required=True, help=help_text)
 
 
-def add_select_agents_argument(parser: argparse.ArgumentParser) -> None:
+def add_select_agents_argument(parser: ArgumentParser, default: List[str]) -> None:
     """Adds optional repeatable string argument 'agent' to given `parser`"""
     help_text = "Provide list of agents to extract (default=None)"
-    parser.add_argument("-a", "--agents", nargs="*", type=str, help=help_text)
+    parser.add_argument("-a", "--agents", nargs="*", type=str, default=default, help=help_text)
 
 
-def add_logfile_argument(parser: argparse.ArgumentParser) -> None:
+def add_logfile_argument(parser: ArgumentParser, default: Path) -> None:
     """Adds optional argument 'logfile' to given `parser`"""
     help_text = "provide logging file (default=None)"
-    parser.add_argument("-lf", "--logfile", type=Path, help=help_text)
+    parser.add_argument("-lf", "--logfile", type=Path, default=default, help=help_text)
 
 
-def add_output_argument(parser: argparse.ArgumentParser, default_value, help_text: str) -> None:
+def add_output_argument(parser: ArgumentParser, default_value, help_text: str) -> None:
     """Adds optional argument 'output' to given `parser` using the given `help_text` and `default_value`"""
     parser.add_argument("-o", "--output", type=Path, default=default_value, help=help_text)
 
 
-def add_log_level_argument(parser: argparse.ArgumentParser, default_value: str) -> None:
+def add_log_level_argument(parser: ArgumentParser, default_value: str) -> None:
     """Adds optional argument 'log' to given `parser`"""
     help_text = "choose logging level (default: {})".format(default_value)
     parser.add_argument(
         "-l",
         "--log",
         default=default_value,
         choices=list(LOG_LEVELS.keys()),
         type=str.lower,
         help=help_text,
     )
 
 
-def add_single_export_argument(parser: argparse.ArgumentParser, default_value: bool) -> None:
+def add_single_export_argument(parser: ArgumentParser, default_value: bool) -> None:
     """Adds optional repeatable string argument 'agent' to given `parser`"""
     help_text = "Enable export of single agents (default=False)"
     parser.add_argument(
         "-se",
         "--single-export",
         default=default_value,
         action="store_true",
         help=help_text,
     )
 
 
-def add_memory_saving_argument(parser: argparse.ArgumentParser, default_value: bool) -> None:
+def add_memory_saving_argument(parser: ArgumentParser, default_value: bool) -> None:
     """Adds optional bool argument to given `parser` to enable memory saving mode"""
     help_text = "Reduces memory usage profile at the cost of runtime (default=False)"
     parser.add_argument(
         "-m",
         "--memory-saving",
         default=default_value,
         action="store_true",
         help=help_text,
     )
 
 
-def add_resolve_complex_argument(parser, default_value: str):
+def add_resolve_complex_argument(parser: ArgumentParser, default_value: Union[ResolveOptions, str]):
     """Instructs given `parser` how to deal with complex field outputs"""
+    default_value = default_value if isinstance(default_value, ResolveOptions) else ResolveOptions[default_value]
     help_text = f"How to deal with complex index columns? (default={default_value})"
     parser.add_argument(
         "-cc",
         "--complex-column",
+        type=ResolveOptions.instantiate,
         default=default_value,
-        choices=[e.name for e in ResolveOptions],
+        choices=ResolveOptions,
         help=help_text,
-        type=str.upper,
     )
 
 
-def add_time_argument(parser: argparse.ArgumentParser, default_value: str) -> None:
+def add_time_argument(parser: ArgumentParser, default_value: Union[TimeOptions, str]) -> None:
     """Adds optional argument to given `parser` to define conversion of TimeSteps"""
+    default_value = default_value if isinstance(default_value, TimeOptions) else TimeOptions[default_value]
     help_text = "Apply conversion of time steps to given format (default=UTC)"
     parser.add_argument(
-        "-t", "--time", default=default_value, choices=[e.name for e in TimeOptions], help=help_text, type=str.upper
+        "-t",
+        "--time",
+        type=TimeOptions.instantiate,
+        default=default_value,
+        choices=TimeOptions,
+        help=help_text,
     )
 
 
-def add_merge_time_parser(parser: argparse.ArgumentParser) -> None:
+def add_merge_time_parser(parser: ArgumentParser) -> None:
     """Adds subparser for merging of TimeSteps to given `parser`"""
     subparser = parser.add_subparsers(dest="time_merging", required=False, help="Optional merging of TimeSteps")
     group_parser = subparser.add_parser("merge-times")
     add_focal_point_argument(group_parser)
     add_steps_before_argument(group_parser)
     add_steps_after_argument(group_parser)
 
 
-def add_focal_point_argument(parser: argparse.ArgumentParser) -> None:
+def add_focal_point_argument(parser: ArgumentParser) -> None:
     """Adds `focal-point` argument to given `parser`"""
     help_text = "TimeStep on which `steps_before` earlier and `steps_after` later TimeSteps are merged on"
     parser.add_argument("-fp", "--focal-point", required=True, type=int, help=help_text)
 
 
-def add_steps_before_argument(parser: argparse.ArgumentParser) -> None:
+def add_steps_before_argument(parser: ArgumentParser) -> None:
     """Adds `steps-before` argument to given `parser`"""
     help_text = "Range of TimeSteps before the `focal-point` they get merged to"
-    parser.add_argument("-sb", "--steps-before", required=True, type=non_negative_int, help=help_text)
+    parser.add_argument("-sb", "--steps-before", required=True, type=_non_negative_int, help=help_text)
 
 
-def non_negative_int(value: Any) -> int:
+def _non_negative_int(value: Any) -> int:
     """
     Casts a given ´value` to int and checks it for non-negativity
 
     Args:
         value: to check and parse
 
     Returns:
@@ -220,34 +167,72 @@
         TypeError: if `value` is None
         ValueError: if `value` cannot be parsed to int
         argparse.ArgumentTypeError: if `value` is a negative int
 
     """
     value = int(value)
     if value < 0:
-        raise argparse.ArgumentTypeError(ERR_NEGATIVE_INT.format(value))
+        raise ArgumentTypeError(_ERR_NEGATIVE_INT.format(value))
     return value
 
 
-def add_steps_after_argument(parser: argparse.ArgumentParser) -> None:
+def add_steps_after_argument(parser: ArgumentParser) -> None:
     """Adds `steps-after` argument to given `parser`"""
     help_text = "Range of TimeSteps after the `focal-point` they get merged to"
-    parser.add_argument("-sa", "--steps-after", required=True, type=non_negative_int, help=help_text)
+    parser.add_argument("-sa", "--steps-after", required=True, type=_non_negative_int, help=help_text)
 
 
-def get_merging_args(args: argparse.Namespace) -> Dict[MergingOptions, int]:
-    """Returns a dictionary of GroupingOptions with their values if `time_merging` entry exists"""
-    merging_args = {}
-    if vars(args).get("time_merging"):
-        merging_args[MergingOptions.FOCAL_POINT] = args.focal_point
-        merging_args[MergingOptions.STEPS_BEFORE] = args.steps_before
-        merging_args[MergingOptions.STEPS_AFTER] = args.steps_after
-    return merging_args
+def add_inputs_recovery_argument(parser: ArgumentParser, default: bool) -> None:
+    """Adds optional bool argument to given `parser` to recover inputs"""
+    help_text = "If --(no-)input-recovery is specified, (no) inputs will be recovered"
+    parser.add_argument(
+        "--input-recovery",
+        action=BooleanOptionalAction,
+        default=default,
+        help=help_text,
+    )
 
 
 def update_default_config(config: Optional[dict], default: dict) -> dict:
     """Returns `default` config with updated fields received from `config`"""
     result = copy.deepcopy(default)
     if config:
         for name, option in config.items():
             result[name] = option
     return result
+
+
+def map_namespace_to_options_dict(parsed: Namespace) -> Dict[Options, Any]:
+    """
+    Maps given parsing results to their corresponding configuration option
+
+    Args:
+        parsed: result of a parsing
+
+    Returns:
+        Map of each parsed argument to their configuration option
+    """
+    return _map_namespace_to_options(parsed, _OPTION_ARGUMENT_NAME)
+
+
+def _map_namespace_to_options(parsed: Namespace, names_to_options: Dict[str, Enum]) -> Dict[Options, Any]:
+    """
+    Maps given parsing results to their corresponding configuration option; elements that cannot be mapped are ignored.
+    If a configuration option has inner elements, these well be also read and added as inner dictionary.
+
+    Args:
+        parsed: result of a parsing
+        names_to_options: dict to search for configuration option specifications
+
+    Returns:
+         Map parsed arguments to their configuration option if they exist in the given `names_to_options` dict
+    """
+    config = {}
+    for name, value in vars(parsed).items():
+        option = names_to_options.get(name, None)
+        if option:
+            if isinstance(option, dict):
+                inner_element_map = option["inner_elements"]
+                option = option["name"]
+                value = _map_namespace_to_options(parsed, inner_element_map)
+            config[option] = value
+    return config
```

### Comparing `fameio-1.8.2/src/fameio/source/loader.py` & `fameio-2.0.0/src/fameio/source/loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
 #
 # SPDX-License-Identifier: Apache-2.0
 
-import logging as log
 import os
 from pathlib import Path
 from fnmatch import fnmatch
 from typing import IO, Any, Callable
 
 import yaml
-from fameio.source.logs import log_and_raise_critical
+from fameio.source.logs import log_and_raise_critical, logger
 from fameio.source.path_resolver import PathResolver
 
 DISABLING_YAML_FILE_PREFIX = "IGNORE_"
 
 CRIT_ERR_NO_YAML_GIVEN = "Please provide a valid YAML file. Received `-f/--file {}` instead."
 
 
@@ -25,23 +24,23 @@
 
 def read_args(loader, args):
     """Returns two Strings to be interpreted as files to be read and a sub-node_address from the given `args`"""
     node_string = ""
     file_string = None
     if isinstance(args, yaml.nodes.ScalarNode):
         file_string = loader.construct_scalar(args)
-        log.debug("Found instance `ScalarNode` in {}".format(file_string))
+        logger().debug("Found instance `ScalarNode` in {}".format(file_string))
     elif isinstance(args, yaml.nodes.SequenceNode):
         argument_list = loader.construct_sequence(args)
         if len(argument_list) not in [1, 2]:
             log_and_raise_critical("!include supports but one or two arguments in list")
         elif len(argument_list) == 2:
             node_string = argument_list[1]
         file_string = argument_list[0]
-        log.debug("Found instance `SequenceNode` in {}".format(file_string))
+        logger().debug("Found instance `SequenceNode` in {}".format(file_string))
     elif isinstance(args, yaml.nodes.MappingNode):
         argument_map = loader.construct_mapping(args)
         for key, value in argument_map.items():
             if key.lower() == "file":
                 file_string = value
             elif key.lower() == "node":
                 node_string = value
@@ -52,23 +51,23 @@
     else:
         log_and_raise_critical("YAML node type not implemented: {}".format(args))
     return Args(file_string, node_string)
 
 
 def split_nodes(node_string):
     """Returns a list of nodes created from the given `node_string`"""
-    log.debug("Splitting given node_string `{}`".format(node_string))
+    logger().debug("Splitting given node_string `{}`".format(node_string))
     return node_string.split(":")
 
 
 class FameYamlLoader(yaml.SafeLoader):
     """Custom YAML Loader for `!include` constructor"""
 
     def __init__(self, stream: IO, path_resolver=PathResolver()) -> None:
-        log.debug("Initialize custom YAML loader")
+        logger().debug("Initialize custom YAML loader")
         self._path_resolver = path_resolver
         try:
             self._root_path = os.path.split(stream.name)[0]
         except AttributeError:
             self._root_path = os.path.curdir
         super().__init__(stream)
 
@@ -96,33 +95,33 @@
     """
     file_list = loader.path_resolver.resolve_yaml_imported_file_pattern(loader.root_path, included_path)
 
     ignore_filter = "*" + DISABLING_YAML_FILE_PREFIX + "*"
     cleaned_file_list = []
     for file in file_list:
         if fnmatch(file, ignore_filter):
-            log.debug("Ignoring file {} due to prefix {}".format(file, DISABLING_YAML_FILE_PREFIX))
+            logger().debug("Ignoring file {} due to prefix {}".format(file, DISABLING_YAML_FILE_PREFIX))
         else:
             cleaned_file_list.append(file)
     if not cleaned_file_list:
         log_and_raise_critical("Failed to find any file matching the `!include` directive `{}`".format(included_path))
-    log.debug("Collected file(s) `{}` from given included path `{}`".format(cleaned_file_list, included_path))
+    logger().debug("Collected file(s) `{}` from given included path `{}`".format(cleaned_file_list, included_path))
     return cleaned_file_list
 
 
 def read_data_from_file(file, node_address, path_resolver: PathResolver):
     """Returns data of the specified `node_address` from the specified `file`"""
     data = yaml.load(file, make_yaml_loader_builder(path_resolver))
     for node in node_address:
         if node:
             try:
                 data = data[node]
             except KeyError:
                 log_and_raise_critical("'!include_node [{}, {}]': Cannot find '{}'.".format(file, node_address, node))
-    log.debug("Searched file `{}` for node `{}`".format(file, node_address))
+    logger().debug("Searched file `{}` for node `{}`".format(file, node_address))
     return data
 
 
 def join_data(new_data, previous_data):
     """Joins data from multiple files if both are in list format, otherwise returns"""
     if not previous_data:
         return new_data
@@ -153,24 +152,24 @@
     files = resolve_imported_path(loader, args.file_string)
 
     joined_data = None
     for file_name in files:
         with open(file_name, "r") as open_file:
             data = read_data_from_file(open_file, nodes, loader.path_resolver)
             joined_data = join_data(data, joined_data)
-    log.debug("Joined all files `{}` to joined data `{}`".format(files, joined_data))
+    logger().debug("Joined all files `{}` to joined data `{}`".format(files, joined_data))
     return joined_data
 
 
 FameYamlLoader.add_constructor("!include", construct_include)
 
 
 def load_yaml(yaml_file_path: Path, path_resolver=PathResolver()):
     """Loads the yaml file from given `yaml_file_path` and returns its content"""
-    log.info("Loading yaml from {}".format(yaml_file_path))
+    logger().info("Loading yaml from {}".format(yaml_file_path))
     with open(yaml_file_path, "r") as configfile:
         data = yaml.load(configfile, make_yaml_loader_builder(path_resolver))
     return data
 
 
 def check_for_yaml_file_type(yaml_file_path: Path) -> None:
     """Raises Exception if given `yaml_file_path` is not a valid YAML file"""
```

### Comparing `fameio-1.8.2/src/fameio/source/logs.py` & `fameio-2.0.0/src/fameio/source/logs.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,59 +1,83 @@
 # SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
 #
 # SPDX-License-Identifier: Apache-2.0
 
 import logging as log
 from pathlib import Path
-from typing import NoReturn
+from typing import NoReturn, Optional, List
 
 LOG_LEVELS = {
     "critical": log.CRITICAL,
     "error": log.ERROR,
     "warn": log.WARNING,
     "warning": log.WARNING,
     "info": log.INFO,
     "debug": log.DEBUG,
 }
 
+_loggers: List[log.Logger] = []
+
+_FORMAT_NORMAL = "%(asctime)s — %(levelname)s — %(message)s"  # noqa
+_FORMAT_DETAILLED = "%(asctime)s.%(msecs)03d — %(levelname)s — %(module)s:%(funcName)s:%(lineno)d — %(message)s"  # noqa
+_TIME_FORMAT = "%H:%M:%S"
+
+_WARN_ALREADY_INITIALIZED = "Cannot set up new FAMEIO logger: using existing logger with previous settings."
+_WARN_NOT_INITIALIZED = "Logger not initialised for FAMEIO - using default root logger"
+
+LOGGER_NAME = "fameio"
+
+
+def logger() -> log.Logger:
+    """Returns already set up FAME-Io's logger or - if not set up - a new logger with level `INFO`"""
+    if not _loggers:
+        set_up_logger("info")
+        log.warning(_WARN_NOT_INITIALIZED)
+    return _loggers[0]
+
 
 def log_and_raise_critical(message: str) -> NoReturn:
     """Raises a critical error and logs with given `error_message`"""
-    log.critical(message)
+    logger().critical(message)
     raise Exception(message)
 
 
 def log_error_and_raise(exception: Exception) -> NoReturn:
     """Raises the specified `exception` and logs an error with the same `message`"""
-    log.error(str(exception))
+    logger().error(str(exception))
     raise exception
 
 
-def set_up_logger(level_name: str, file_name: Path) -> None:
+def set_up_logger(level_name: str, file_name: Optional[Path] = None) -> None:
     """Uses existing logger or sets up logger"""
-    if not log.getLogger().hasHandlers():
-        _set_up_new_logger(level_name, file_name)
+    if not _loggers:
+        _loggers.append(log.getLogger(LOGGER_NAME))
+        level = LOG_LEVELS.get(level_name.lower())
+        _set_log_level(level)
+        formatter = _get_formatter(level)
+        _add_handler(log.StreamHandler(), formatter)
+        if file_name:
+            _add_handler(log.FileHandler(file_name, mode="w"), formatter)
+    else:
+        log.warning(_WARN_ALREADY_INITIALIZED)
 
 
-def _set_up_new_logger(level_name: str, file_name: Path) -> None:
-    """Sets up new logger which always writes to the console and if provided also to `file_name`"""
-    level = LOG_LEVELS.get(level_name.lower())
-    if level is log.DEBUG:
-        formatter_string = (
-            "%(asctime)s.%(msecs)03d — %(levelname)s — %(module)s:%(funcName)s:%(lineno)d — %(message)s"  # noqa
-        )
-    else:
-        formatter_string = "%(asctime)s — %(levelname)s — %(message)s"  # noqa
+def _set_log_level(level: int) -> None:
+    """Set the global log level to given `level`"""
+    logger().setLevel(level)
 
-    log_formatter = log.Formatter(formatter_string, "%H:%M:%S")
 
-    root_logger = log.getLogger()
-    root_logger.setLevel(level)
+def _get_formatter(level: int) -> log.Formatter:
+    """
+    Returns a log formatter depending on the given log `level`
+    Args:
+        level: this log level determines how detailed the logger's output is
+    Returns:
+        new log formatter
+    """
+    return log.Formatter(_FORMAT_DETAILLED if level is log.DEBUG else _FORMAT_NORMAL, _TIME_FORMAT)
 
-    if file_name:
-        file_handler = log.FileHandler(file_name, mode="w")
-        file_handler.setFormatter(log_formatter)
-        root_logger.addHandler(file_handler)
 
-    console_handler = log.StreamHandler()
-    console_handler.setFormatter(log_formatter)
-    root_logger.addHandler(console_handler)
+def _add_handler(handler: log.Handler, formatter: log.Formatter) -> None:
+    """Adds given `handler` to root logger using the specified `formatter`"""
+    handler.setFormatter(formatter)
+    logger().addHandler(handler)
```

### Comparing `fameio-1.8.2/src/fameio/source/path_resolver.py` & `fameio-2.0.0/src/fameio/source/path_resolver.py`

 * *Files identical despite different names*

### Comparing `fameio-1.8.2/src/fameio/source/results/agent_type.py` & `fameio-2.0.0/src/fameio/source/results/agent_type.py`

 * *Files identical despite different names*

### Comparing `fameio-1.8.2/src/fameio/source/results/conversion.py` & `fameio-2.0.0/src/fameio/source/results/conversion.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
 #
 # SPDX-License-Identifier: Apache-2.0
 
 import math
 from typing import Dict, Optional
-import logging as log
 
 import pandas as pd
 
 from fameio.source import FameTime
-from fameio.source.cli import TimeOptions, MergingOptions
-from fameio.source.logs import log_error_and_raise
+from fameio.source.cli.options import TimeOptions, MergingOptions
+from fameio.source.logs import log_error_and_raise, logger
 from fameio.source.time import ConversionException
 
 _ERR_UNIMPLEMENTED = "Time conversion mode '{}' not implemented."
 
 
 def apply_time_merging(data: Dict[Optional[str], pd.DataFrame], config: Optional[Dict[MergingOptions, int]]) -> None:
     """
@@ -24,15 +23,15 @@
         data: one or multiple DataFrames of time series; column `TimeStep` might be modified
         config: dict of MergingOptions defining how to merge the TimeSteps
 
     Returns:
         Nothing - data is modified inplace
     """
     if config:
-        log.debug(f"Grouping TimeSteps...")
+        logger().debug(f"Grouping TimeSteps...")
         offset = config[MergingOptions.STEPS_BEFORE]
         period = config[MergingOptions.STEPS_AFTER] + config[MergingOptions.STEPS_BEFORE] + 1
         first_positive_focal_point = config[MergingOptions.FOCAL_POINT] % period
         for key in data.keys():
             df = data[key]
             index_columns = df.index.names
             df.reset_index(inplace=True)
@@ -52,47 +51,46 @@
 
     Returns:
         Corresponding focal point
     """
     return math.floor((time_step + offset - focal_time) / period) * period + focal_time
 
 
-def apply_time_option(data: Dict[Optional[str], pd.DataFrame], mode_name: str) -> None:
+def apply_time_option(data: Dict[Optional[str], pd.DataFrame], mode: TimeOptions) -> None:
     """
     Applies time option based on given `mode` inplace of given `data`
 
     Args:
         data: one or multiple DataFrames of time series; column `TimeStep` might be modified (depending on mode)
-        mode_name: name of time conversion mode (derived from Enum)
+        mode: name of time conversion mode (derived from Enum)
 
     Returns:
         Nothing - data is modified inplace
     """
-    mode_name = mode_name.upper()
-    if mode_name == TimeOptions.INT.name:
-        log.debug("No time conversion...")
-    elif mode_name == TimeOptions.UTC.name:
+    if mode == TimeOptions.INT:
+        logger().debug("No time conversion...")
+    elif mode == TimeOptions.UTC:
         _convert_time_index(data, "%Y-%m-%d %H:%M:%S")
-    elif mode_name == TimeOptions.FAME.name:
+    elif mode == TimeOptions.FAME:
         _convert_time_index(data, "%Y-%m-%d_%H:%M:%S")
     else:
-        log_error_and_raise(ConversionException(_ERR_UNIMPLEMENTED.format(mode_name)))
+        log_error_and_raise(ConversionException(_ERR_UNIMPLEMENTED.format(mode)))
 
 
 def _convert_time_index(data: Dict[Optional[str], pd.DataFrame], datetime_format: str) -> None:
     """
     Inplace replacement of `TimeStep` column in MultiIndex of each item of `data` from FAME's time steps` to DateTime
     in given `date_format`
 
     Args:
         data: one or multiple DataFrames of time series; column `TimeStep` will be modified
         datetime_format: used for the conversion
 
     Returns:
         Nothing - data is modified inplace
     """
-    log.debug(f"Converting TimeStep to format '{datetime_format}'...")
+    logger().debug(f"Converting TimeStep to format '{datetime_format}'...")
     for _, df in data.items():
         index_columns = df.index.names
         df.reset_index(inplace=True)
         df["TimeStep"] = df["TimeStep"].apply(lambda t: FameTime.convert_fame_time_step_to_datetime(t, datetime_format))
         df.set_index(keys=index_columns, inplace=True)
```

### Comparing `fameio-1.8.2/src/fameio/source/results/csv_writer.py` & `fameio-2.0.0/src/fameio/source/results/csv_writer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-# SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
+# SPDX-FileCopyrightText: 2024 German Aerospace Center <fame@dlr.de>
 #
 # SPDX-License-Identifier: Apache-2.0
 
-import logging as log
 from pathlib import Path
 from typing import Dict, Union
 
 import pandas as pd
 
+from fameio.source.logs import logger
 from fameio.source.results.data_transformer import INDEX
+from fameio.source.series import TimeSeriesManager
+from fameio.source.tools import ensure_path_exists
 
 
 class CsvWriter:
     """Writes dataframes to different csv files"""
 
     _INFO_USING_PATH = "Using specified output path: {}"
     _INFO_USING_DERIVED_PATH = "No output path specified - writing to new local folder: {}"
@@ -24,23 +26,23 @@
         self._create_output_folder()
 
     @staticmethod
     def _get_output_folder_name(config_output: Path, input_file_path: Path) -> Path:
         """Returns name of the output folder derived either from the specified `config_output` or `input_file_path`"""
         if config_output:
             output_folder_name = config_output
-            log.info(CsvWriter._INFO_USING_PATH.format(config_output))
+            logger().info(CsvWriter._INFO_USING_PATH.format(config_output))
         else:
             output_folder_name = input_file_path.stem
-            log.info(CsvWriter._INFO_USING_DERIVED_PATH.format(output_folder_name))
+            logger().info(CsvWriter._INFO_USING_DERIVED_PATH.format(output_folder_name))
         return Path(output_folder_name)
 
     def _create_output_folder(self) -> None:
         """Creates output folder if not yet present"""
-        log.debug("Creating output folder if required...")
+        logger().debug("Creating output folder if required...")
         if not self._output_folder.is_dir():
             self._output_folder.mkdir(parents=True)
 
     def write_to_files(self, agent_name: str, data: Dict[Union[None, str], pd.DataFrame]) -> None:
         """Writes `data` for given `agent_name` to .csv file(s)"""
         for column_name, column_data in data.items():
             column_data.sort_index(inplace=True)
@@ -48,14 +50,23 @@
                 for agent_id, agent_data in column_data.groupby(INDEX[0]):
                     identifier = self._get_identifier(agent_name, column_name, str(agent_id))
                     self._write_data_frame(agent_data, identifier)
             else:
                 identifier = self._get_identifier(agent_name, column_name)
                 self._write_data_frame(column_data, identifier)
 
+    def write_time_series_to_disk(self, timeseries_manager: TimeSeriesManager) -> None:
+        """Writes time_series of given `timeseries_manager` to disk"""
+        for _, name, data in timeseries_manager.get_all_series():
+            if data is not None:
+                target_path = Path(self._output_folder, name)
+                ensure_path_exists(target_path.parent)
+                # noinspection PyTypeChecker
+                data.to_csv(path_or_buf=target_path, sep=";", header=None, index=None)
+
     @staticmethod
     def _get_identifier(agent_name: str, column_name: str, agent_id: str = None) -> str:
         """Returns unique identifier for given `agent_name` and (optional) `agent_id` and `column_name`"""
         identifier = str(agent_name)
         if column_name:
             identifier += f"_{column_name}"
         if agent_id:
```

### Comparing `fameio-1.8.2/src/fameio/source/results/data_transformer.py` & `fameio-2.0.0/src/fameio/source/results/data_transformer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
 #
 # SPDX-License-Identifier: Apache-2.0
+from __future__ import annotations
 
 from abc import ABC
 from builtins import staticmethod
 from typing import List, Dict, Tuple, Union, Optional
 
 import pandas as pd
 from fameprotobuf.Services_pb2 import Output
 from pandas import DataFrame
 
-from fameio.source.cli import ResolveOptions
+from fameio.source.cli.options import ResolveOptions
 from fameio.source.results.agent_type import AgentType
 
 INDEX = ("AgentId", "TimeStep")
 
 
 class DataTransformer(ABC):
     """Extracts and provides series data from parsed and processed output files for requested agents"""
@@ -23,15 +24,15 @@
         ResolveOptions.IGNORE: lambda: DataTransformerIgnore(),
         ResolveOptions.MERGE: lambda: DataTransformerMerge(),
         ResolveOptions.SPLIT: lambda: DataTransformerSplit(),
     }
     SIMPLE_COLUMN_INDEX = -1
 
     @staticmethod
-    def build(complex_column_mode: ResolveOptions) -> "DataTransformer":
+    def build(complex_column_mode: ResolveOptions) -> DataTransformer:
         return DataTransformer.MODES[complex_column_mode]()
 
     def extract_agent_data(
         self, series: List[Output.Series], agent_type: AgentType
     ) -> Dict[Optional[str], pd.DataFrame]:
         """
         Returns dict of DataFrame(s) containing all data from given `series` of given `agent_type`.
```

### Comparing `fameio-1.8.2/src/fameio/source/results/output_dao.py` & `fameio-2.0.0/src/fameio/source/results/output_dao.py`

 * *Files identical despite different names*

### Comparing `fameio-1.8.2/src/fameio/source/results/reader.py` & `fameio-2.0.0/src/fameio/source/results/reader.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,66 +1,77 @@
 # SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
 #
 # SPDX-License-Identifier: Apache-2.0
+from __future__ import annotations
 
-import logging as log
 import struct
 import typing
 from abc import ABC, abstractmethod
 from typing import IO, List
 
 from fameprotobuf.DataStorage_pb2 import DataStorage
 from google.protobuf.message import DecodeError
 
+from fameio.source.logs import logger
+
 
 class Reader(ABC):
     """Abstract base class for protobuf file readers"""
 
     _WARN_NO_HEADER = "No header recognised in file. File might be deprecated or corrupted."  # noqa
     _ERR_FILE_CORRUPT_NEGATIVE_LENGTH = "Corrupt file, message length must be positive."
     _ERR_FILE_CORRUPT_MISSING_DATA = "Trying to read corrupt file caused by inconsistent message length."
     _ERR_UNSUPPORTED_MODE = "Ignoring memory saving mode: not supported for files created with `fame-core<1.4`."
     _ERR_PARSING_FAILED = "File Corrupt. Could not parse file content."
     _DEBUG_FILE_END_REACHED = "Reached expected end of file."
 
     _HEADER_LENGTH = 30
-    _HEADER_ENCODING = "utf-8"
-    _BYTES_DEFINING_MESSAGE_LENGTH = 4
+    HEADER_ENCODING = "utf-8"
+    BYTES_DEFINING_MESSAGE_LENGTH = 4
     _READER_HEADERS = {
         "famecoreprotobufstreamfilev001": lambda file, mode: ReaderV1(file, mode),  # noqa
     }
 
     def __init__(self, file: IO, read_single) -> None:
         self._file = file
         self._read_single = read_single
 
     @abstractmethod
     def read(self) -> List[DataStorage]:
         """Reads associated filestream and returns one or multiple DataStorage(s) or empty list"""
 
     @staticmethod
-    def get_reader(file: IO, read_single: bool = False) -> "Reader":
-        """Returns reader matching the given file header - if `read_one` is True, read() gets one messages at a time"""
-        log.debug("Reading file headers...")
+    def get_reader(file: IO, read_single: bool = False) -> Reader:
+        """
+        Returns reader matching the given file header
+
+        Args:
+            file: to be read by the returned Reader
+            read_single: if True, the returned Reader's `read()` method gets one messages at a time
+
+        Returns:
+            Reader that can read the specified file
+        """
+        logger().debug("Reading file headers...")
         try:
-            header = file.read(Reader._HEADER_LENGTH).decode(Reader._HEADER_ENCODING)
+            header = file.read(Reader._HEADER_LENGTH).decode(Reader.HEADER_ENCODING)
             return Reader._READER_HEADERS[header](file, read_single)
         except (KeyError, UnicodeDecodeError):
-            log.warning(Reader._WARN_NO_HEADER)
+            logger().warning(Reader._WARN_NO_HEADER)
             file.seek(0)
             if read_single:
-                log.error(Reader._ERR_UNSUPPORTED_MODE)
+                logger().error(Reader._ERR_UNSUPPORTED_MODE)
             return ReaderV0(file, False)
 
     @typing.final
     def _read_message_length(self) -> int:
         """Returns length of next DataStorage message in file"""
-        message_length_byte = self._file.read(self._BYTES_DEFINING_MESSAGE_LENGTH)
+        message_length_byte = self._file.read(self.BYTES_DEFINING_MESSAGE_LENGTH)
         if not message_length_byte:
-            log.debug(self._DEBUG_FILE_END_REACHED)
+            logger().debug(self._DEBUG_FILE_END_REACHED)
             message_length_int = 0
         else:
             message_length_int = struct.unpack(">i", message_length_byte)[0]
         return message_length_int
 
     @typing.final
     def _read_data_storage_message(self, message_length: int = None) -> DataStorage:
@@ -71,15 +82,15 @@
         if message_length is None:
             message = self._file.read()
         elif message_length > 0:
             message = self._file.read(message_length)
         else:
             raise IOError(self._ERR_FILE_CORRUPT_NEGATIVE_LENGTH)
         if message_length and len(message) != message_length:
-            log.error(self._ERR_FILE_CORRUPT_MISSING_DATA)
+            logger().error(self._ERR_FILE_CORRUPT_MISSING_DATA)
         return self._parse_to_data_storage(message) if message else None
 
     @staticmethod
     @typing.final
     def _parse_to_data_storage(message: bytes) -> DataStorage:
         data_storage = DataStorage()
         try:
@@ -92,15 +103,15 @@
 class ReaderV0(Reader):
     """Reader class for deprecated `fame-core<1.4` output without any header"""
 
     _WARN_DEPRECATED = "DeprecationWarning: Please consider updating to `FAME-Core>=1.4` and `fameio>=1.6`"
 
     def __init__(self, file: IO, read_single):
         super().__init__(file, read_single)
-        log.warning(self._WARN_DEPRECATED)
+        logger().warning(self._WARN_DEPRECATED)
 
     def read(self) -> List[DataStorage]:
         result = self._read_data_storage_message()
         return [result] if result else []
 
 
 class ReaderV1(Reader):
@@ -111,9 +122,9 @@
         while True:
             message_length = self._read_message_length()
             if message_length == 0:
                 break
             messages.append(self._read_data_storage_message(message_length))
             if self._read_single:
                 break
-        log.debug(f"Read {len(messages)} messages from file.")
+        logger().debug(f"Read {len(messages)} messages from file.")
         return messages
```

### Comparing `fameio-1.8.2/src/fameio/source/scenario/agent.py` & `fameio-2.0.0/src/fameio/source/scenario/agent.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-# SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
+# SPDX-FileCopyrightText: 2024 German Aerospace Center <fame@dlr.de>
 #
 # SPDX-License-Identifier: Apache-2.0
+from __future__ import annotations
 
-from typing import Any, Dict
+import ast
+from typing import Any, Dict, Optional
 
 from fameio.source.scenario.attribute import Attribute
 from fameio.source.scenario.exception import (
     assert_or_raise,
     get_or_default,
     get_or_raise,
 )
@@ -15,54 +17,79 @@
 
 class Agent:
     """Contains specifications for an agent in a scenario"""
 
     _KEY_TYPE = "Type".lower()
     _KEY_ID = "Id".lower()
     _KEY_ATTRIBUTES = "Attributes".lower()
+    _KEY_METADATA = "MetaData".lower()
 
-    _MISSING_KEY = "Agent requires `key` '{}' but is missing it."
-    _MISSING_TYPE = "Agent requires `type` but is missing it."
-    _MISSING_ID = "Agent requires a positive integer `id` but was '{}'."
-    _DOUBLE_ATTRIBUTE = "Cannot add attribute '{}' to agent {} because it already exists."
+    _ERR_MISSING_KEY = "Agent requires `key` '{}' but is missing it."
+    _ERR_MISSING_TYPE = "Agent requires `type` but is missing it."
+    _ERR_MISSING_ID = "Agent requires a positive integer `id` but was '{}'."
+    _ERR_DOUBLE_ATTRIBUTE = "Cannot add attribute '{}' to agent {} because it already exists."
+    _ERR_ATTRIBUTE_OVERWRITE = "Agent's attributes are already set and would be overwritten."
 
-    def __init__(self, agent_id: int, type_name: str) -> None:
+    def __init__(self, agent_id: int, type_name: str, meta_data: Optional[Dict] = None) -> None:
         """Constructs a new Agent"""
-        assert_or_raise(type(agent_id) is int and agent_id >= 0, self._MISSING_ID.format(agent_id))
-        assert_or_raise(type_name and len(type_name.strip()) > 0, self._MISSING_TYPE)
-        self._id = agent_id
-        self._type_name = type_name.strip()
-        self._attributes = {}
+        assert_or_raise(type(agent_id) is int and agent_id >= 0, self._ERR_MISSING_ID.format(agent_id))
+        assert_or_raise(bool(type_name and type_name.strip()), self._ERR_MISSING_TYPE)
+        self._id: int = agent_id
+        self._type_name: str = type_name.strip()
+        self._attributes: Dict = {}
+        self._meta_data: Optional[Dict] = meta_data if meta_data else {}
 
     @classmethod
-    def from_dict(cls, definitions: dict) -> "Agent":
+    def from_dict(cls, definitions: dict) -> Agent:
         """Parses an agent from provided `definitions`"""
         definitions = keys_to_lower(definitions)
-        agent_type = get_or_raise(definitions, Agent._KEY_TYPE, Agent._MISSING_KEY)
-        agent_id = get_or_raise(definitions, Agent._KEY_ID, Agent._MISSING_KEY)
-        result = cls(agent_id, agent_type)
-        attribute_definitions = get_or_default(definitions, Agent._KEY_ATTRIBUTES, dict())
-        result.__init_attributes_from_dict(attribute_definitions)
-        return result
+        agent_type = get_or_raise(definitions, Agent._KEY_TYPE, Agent._ERR_MISSING_TYPE)
+        agent_id = get_or_raise(definitions, Agent._KEY_ID, Agent._ERR_MISSING_ID)
+        agent = cls(agent_id, agent_type)
+        attribute_definitions = get_or_default(definitions, Agent._KEY_ATTRIBUTES, {})
+        agent.init_attributes_from_dict(attribute_definitions)
+        agent._meta_data = get_or_default(definitions, Agent._KEY_METADATA, {})
+        return agent
+
+    def init_attributes_from_dict(self, attributes: Dict[str, Any]) -> None:
+        """Initialize Agent `attributes` from dict; Must only be called when creating a new Agent"""
+        assert_or_raise(not self._attributes, self._ERR_ATTRIBUTE_OVERWRITE)
+        self._attributes = {}
+        for name, value in attributes.items():
+            full_name = f"{self.type_name}({self.id}): {name}"
+            self.add_attribute(name, Attribute(full_name, value))
+
+    def add_attribute(self, name: str, value: Attribute) -> None:
+        """Adds a new attribute to the Agent (raise an error if it already exists)"""
+        if name in self._attributes:
+            raise ValueError(self._ERR_DOUBLE_ATTRIBUTE.format(name, self.display_id))
+        self._attributes[name] = value
+        self._notify_data_changed()
 
     def to_dict(self) -> dict:
         """Serializes the Agent content to a dict"""
-        result = {}
-
-        result[Agent._KEY_TYPE] = self.type_name
-        result[Agent._KEY_ID] = self.id
+        result = {Agent._KEY_TYPE: self.type_name, Agent._KEY_ID: self.id}
 
-        if len(self.attributes) > 0:
+        if self.attributes:
             attributes_dict = {}
             for attr_name, attr_value in self.attributes.items():
                 attributes_dict[attr_name] = attr_value.generic_content
             result[self._KEY_ATTRIBUTES] = attributes_dict
-
+        if self.meta_data:
+            result[self._KEY_METADATA] = self.meta_data
         return result
 
+    def to_string(self) -> str:
+        """Serializes this agent to a string"""
+        return repr(self.to_dict())
+
+    @classmethod
+    def from_string(cls, definitions: str) -> Agent:
+        return cls.from_dict(ast.literal_eval(definitions))
+
     def _notify_data_changed(self):
         """Placeholder method used to signal data changes to derived types"""
         pass
 
     @property
     def id(self) -> int:
         """Returns the ID of the Agent"""
@@ -79,21 +106,11 @@
         return self._type_name
 
     @property
     def attributes(self) -> Dict[str, Attribute]:
         """Returns dictionary of all Attributes of this agent"""
         return self._attributes
 
-    def add_attribute(self, name: str, value: Attribute):
-        """Adds a new attribute to the Agent (raise an error if it already exists)"""
-        if name in self._attributes:
-            raise ValueError(self._DOUBLE_ATTRIBUTE.format(name, self.display_id))
-        self._attributes[name] = value
-        self._notify_data_changed()
-
-    def __init_attributes_from_dict(self, attributes: Dict[str, Any]) -> None:
-        """Initialize Agent `attributes` from dict; Must only be called when creating a new Agent"""
-        assert len(self._attributes) == 0
-        self._attributes = {}
-        for name, value in attributes.items():
-            full_name = str(self.type_name) + "(" + str(self.id) + "): " + name
-            self.add_attribute(name, Attribute(full_name, value))
+    @property
+    def meta_data(self) -> dict:
+        """Returns dictionary of all MetaData of this agent"""
+        return self._meta_data
```

### Comparing `fameio-1.8.2/src/fameio/source/scenario/attribute.py` & `fameio-2.0.0/src/fameio/source/scenario/attribute.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
 #
 # SPDX-License-Identifier: Apache-2.0
+from __future__ import annotations
 
-import logging as log
 from typing import Any, Dict, List
 
 from fameio.source.scenario.exception import log_and_raise
 
 
 class Attribute:
     """An Attribute of an agent in a scenario"""
 
     _VALUE_MISSING = "Value not specified for Attribute '{}' - leave out if default shall be used (if defined)."
-    _OVERWRITE = "Value already defined for Attribute '{}' - overwriting value with new one!"
     _LIST_EMPTY = "Attribute '{}' was assigned an empty list - please remove or fill empty assignments."
     _DICT_EMPTY = "Attribute '{}' was assigned an empty dictionary - please remove or fill empty assignments."
     _MIXED_DATA = "Attribute '{}' was assigned a list with mixed complex and simple entries - please fix."
 
     def __init__(self, name: str, definitions) -> None:
         """Parses an Attribute's definition"""
         self._full_name = name
@@ -41,21 +40,19 @@
 
     @staticmethod
     def _build_attribute_dict(name: str, definitions: Dict[str, Any]) -> Dict[str, "Attribute"]:
         """Returns a new dictionary containing Attributes generated from given `definitions`"""
         if not definitions:
             log_and_raise(Attribute._DICT_EMPTY.format(name))
 
-        dictionary = {}
+        inner_elements = {}
         for nested_name, value in definitions.items():
             full_name = name + "." + nested_name
-            if nested_name in dictionary:
-                log.warning(Attribute._OVERWRITE.format(full_name))
-            dictionary[nested_name] = Attribute(full_name, value)
-        return dictionary
+            inner_elements[nested_name] = Attribute(full_name, value)
+        return inner_elements
 
     @staticmethod
     def _is_list_of_dict(name: str, definitions: Any) -> bool:
         """Returns True if given `definitions` is a list of dict"""
         if isinstance(definitions, list):
             if not definitions:
                 log_and_raise(Attribute._LIST_EMPTY.format(name))
@@ -75,18 +72,18 @@
     def generic_content(self) -> Any:
         """Returns the full content of the attribute (and its children) as a generic value"""
         if self.has_value:
             return self.value
         elif self.has_nested_list:
             result = []
             for attr_dict in self.nested_list:
-                sub_dict = {}
+                inner_elements = {}
                 for name, attr in attr_dict.items():
-                    sub_dict[name] = attr.generic_content
-                result.append(sub_dict)
+                    inner_elements[name] = attr.generic_content
+                result.append(inner_elements)
             return result
         elif self.has_nested:
             result = {}
             for name, attr in self.nested.items():
                 result[name] = attr.generic_content
             return result
         else:
@@ -103,20 +100,20 @@
 
     @property
     def has_nested(self) -> bool:
         """Returns True if nested Attributes are present"""
         return bool(self._nested)
 
     @property
-    def nested(self) -> Dict[str, "Attribute"]:
+    def nested(self) -> Dict[str, Attribute]:
         """Returns dictionary of all nested Attributes"""
         assert self.has_nested
         return self._nested
 
-    def get_nested_by_name(self, key: str) -> "Attribute":
+    def get_nested_by_name(self, key: str) -> Attribute:
         """Returns nested Attribute by specified name"""
         return self._nested[key]
 
     @property
     def has_nested_list(self) -> bool:
         """Returns True if list of nested items is present"""
         return bool(self._nested_list)
```

### Comparing `fameio-1.8.2/src/fameio/source/scenario/contract.py` & `fameio-2.0.0/src/fameio/source/scenario/contract.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
 #
 # SPDX-License-Identifier: Apache-2.0
+from __future__ import annotations
 
-import logging as log
 from typing import Any, Dict, List, Optional
 
+from fameio.source.logs import logger
 from fameio.source.scenario.attribute import Attribute
 from fameio.source.scenario.exception import get_or_default, get_or_raise, log_and_raise
 from fameio.source.time import FameTime
 from fameio.source.tools import ensure_is_list, keys_to_lower
 
 
 class Contract:
@@ -16,47 +17,50 @@
 
     _KEY_SENDER = "SenderId".lower()
     _KEY_RECEIVER = "ReceiverId".lower()
     _KEY_PRODUCT = "ProductName".lower()
     _KEY_FIRST_DELIVERY = "FirstDeliveryTime".lower()
     _KEY_INTERVAL = "DeliveryIntervalInSteps".lower()
     _KEY_EXPIRE = "ExpirationTime".lower()
+    _KEY_METADATA = "MetaData".lower()
     _KEY_ATTRIBUTES = "Attributes".lower()
 
-    _MISSING_KEY = "Contract requires key '{}' but is missing it."
-    _MULTI_CONTRACT_CORRUPT = (
+    _ERR_MISSING_KEY = "Contract requires key '{}' but is missing it."
+    _ERR_MULTI_CONTRACT_CORRUPT = (
         "Definition of Contracts is valid only for One-to-One, One-to-many, Many-to-one, "
         "or N-to-N sender-to-receiver numbers. Found M-to-N pairing in Contract with "
         "Senders: {} and Receivers: {}."
     )
-    _NEGATIVE_INTERVAL = "Contract delivery interval must be a positive integer but was: {}"
-    _SENDER_IS_RECEIVER = "Contract sender and receiver have the same id: {}"
-    _DOUBLE_ATTRIBUTE = "Cannot add attribute '{}' to contract because it already exists."
+    _ERR_INTERVAL_NOT_POSITIVE = "Contract delivery interval must be a positive integer but was: {}"
+    _ERR_SENDER_IS_RECEIVER = "Contract sender and receiver have the same id: {}"
+    _ERR_DOUBLE_ATTRIBUTE = "Cannot add attribute '{}' to contract because it already exists."
 
     def __init__(
         self,
         sender_id: int,
         receiver_id: int,
         product_name: str,
         delivery_interval: int,
         first_delivery_time: int,
         expiration_time: Optional[int] = None,
-    ):
+        meta_data: Optional[dict] = None,
+    ) -> None:
         """Constructs a new Contract"""
         assert product_name != ""
         if sender_id == receiver_id:
-            log.warning(self._SENDER_IS_RECEIVER.format(sender_id))
-        if delivery_interval < 0:
-            raise ValueError(self._NEGATIVE_INTERVAL.format(delivery_interval))
+            logger().warning(self._ERR_SENDER_IS_RECEIVER.format(sender_id))
+        if delivery_interval <= 0:
+            raise ValueError(self._ERR_INTERVAL_NOT_POSITIVE.format(delivery_interval))
         self._sender_id = sender_id
         self._receiver_id = receiver_id
         self._product_name = product_name
         self._delivery_interval = delivery_interval
         self._first_delivery_time = first_delivery_time
         self._expiration_time = expiration_time
+        self._meta_data = meta_data
         self._attributes = {}
 
     def _notify_data_changed(self):
         """Placeholder method used to signal data changes to derived types"""
         pass
 
     @property
@@ -96,110 +100,121 @@
 
     @property
     def expiration_time(self) -> Optional[int]:
         """Returns the expiration time of the contract if available, None otherwise"""
         return self._expiration_time
 
     @property
+    def meta_data(self) -> Optional[dict]:
+        """Returns the metadata of the contract if available, None otherwise"""
+        return self._meta_data
+
+    @property
     def attributes(self) -> Dict[str, Attribute]:
         """Returns dictionary of all Attributes of the contract"""
         return self._attributes
 
-    def add_attribute(self, name: str, value: Attribute):
+    def add_attribute(self, name: str, value: Attribute) -> None:
         """Adds a new attribute to the Contract (raise an error if it already exists)"""
         if name in self._attributes:
-            raise ValueError(self._DOUBLE_ATTRIBUTE.format(name))
+            raise ValueError(self._ERR_DOUBLE_ATTRIBUTE.format(name))
         self._attributes[name] = value
         self._notify_data_changed()
 
-    def __init_attributes_from_dict(self, attributes: Dict[str, Any]) -> None:
-        """Resets Contract `attributes` from dict; Must only be called when creating a new Contract"""
-        assert len(self._attributes) == 0
-        self._attributes = {}
-        for name, value in attributes.items():
-            full_name = str(type) + "." + str(id) + name
-            self.add_attribute(name, Attribute(full_name, value))
-
     @classmethod
-    def from_dict(cls, definitions: dict) -> "Contract":
+    def from_dict(cls, definitions: dict) -> Contract:
         """Parses Contract from given `definitions`"""
         definitions = keys_to_lower(definitions)
-        sender_id = get_or_raise(definitions, Contract._KEY_SENDER, Contract._MISSING_KEY)
-        receiver_id = get_or_raise(definitions, Contract._KEY_RECEIVER, Contract._MISSING_KEY)
-        product_name = get_or_raise(definitions, Contract._KEY_PRODUCT, Contract._MISSING_KEY)
+        sender_id = get_or_raise(definitions, Contract._KEY_SENDER, Contract._ERR_MISSING_KEY)
+        receiver_id = get_or_raise(definitions, Contract._KEY_RECEIVER, Contract._ERR_MISSING_KEY)
+        product_name = get_or_raise(definitions, Contract._KEY_PRODUCT, Contract._ERR_MISSING_KEY)
         first_delivery_time = FameTime.convert_string_if_is_datetime(
-            get_or_raise(definitions, Contract._KEY_FIRST_DELIVERY, Contract._MISSING_KEY)
+            get_or_raise(definitions, Contract._KEY_FIRST_DELIVERY, Contract._ERR_MISSING_KEY)
         )
-        delivery_interval = get_or_raise(definitions, Contract._KEY_INTERVAL, Contract._MISSING_KEY)
+        delivery_interval = get_or_raise(definitions, Contract._KEY_INTERVAL, Contract._ERR_MISSING_KEY)
         expiration_time = get_or_default(definitions, Contract._KEY_EXPIRE, None)
         expiration_time = FameTime.convert_string_if_is_datetime(expiration_time) if expiration_time else None
+        meta_data = get_or_default(definitions, Contract._KEY_METADATA, None)
         result = cls(
             sender_id,
             receiver_id,
             product_name,
             delivery_interval,
             first_delivery_time,
             expiration_time,
+            meta_data,
         )
         attribute_definitions = get_or_default(definitions, Contract._KEY_ATTRIBUTES, dict())
-        result.__init_attributes_from_dict(attribute_definitions)
+        result._init_attributes_from_dict(attribute_definitions)
         return result
 
+    def _init_attributes_from_dict(self, attributes: Dict[str, Any]) -> None:
+        """Resets Contract `attributes` from dict; Must only be called when creating a new Contract"""
+        assert len(self._attributes) == 0
+        self._attributes = {}
+        for name, value in attributes.items():
+            full_name = f"{type}.{id}{name}"
+            self.add_attribute(name, Attribute(full_name, value))
+
     def to_dict(self) -> dict:
         """Serializes the Contract content to a dict"""
-        result = {}
-        result[self._KEY_SENDER] = self.sender_id
-        result[self._KEY_RECEIVER] = self.receiver_id
-        result[self._KEY_PRODUCT] = self.product_name
-        result[self._KEY_FIRST_DELIVERY] = self.first_delivery_time
-        result[self._KEY_INTERVAL] = self.delivery_interval
+        result = {
+            self._KEY_SENDER: self.sender_id,
+            self._KEY_RECEIVER: self.receiver_id,
+            self._KEY_PRODUCT: self.product_name,
+            self._KEY_FIRST_DELIVERY: self.first_delivery_time,
+            self._KEY_INTERVAL: self.delivery_interval,
+        }
 
         if self.expiration_time is not None:
             result[self._KEY_EXPIRE] = self.expiration_time
 
         if len(self.attributes) > 0:
             attributes_dict = {}
             for attr_name, attr_value in self.attributes.items():
                 attributes_dict[attr_name] = attr_value.generic_content
             result[self._KEY_ATTRIBUTES] = attributes_dict
+        if self.meta_data:
+            result[self._KEY_METADATA] = self._meta_data
 
         return result
 
     @staticmethod
     def split_contract_definitions(multi_definition: dict) -> List[dict]:
         """Splits given `multi_definition` dictionary into list of individual Contract definitions"""
         contracts = []
         base_data = {}
         multi_definition = keys_to_lower(multi_definition)
         for key in [
             Contract._KEY_PRODUCT,
             Contract._KEY_FIRST_DELIVERY,
-            Contract._KEY_FIRST_DELIVERY,
             Contract._KEY_INTERVAL,
             Contract._KEY_EXPIRE,
+            Contract._KEY_METADATA,
             Contract._KEY_ATTRIBUTES,
         ]:
             if key in multi_definition:
                 base_data[key] = multi_definition[key]
-        senders = ensure_is_list(get_or_raise(multi_definition, Contract._KEY_SENDER, Contract._MISSING_KEY))
-        receivers = ensure_is_list(get_or_raise(multi_definition, Contract._KEY_RECEIVER, Contract._MISSING_KEY))
+        senders = ensure_is_list(get_or_raise(multi_definition, Contract._KEY_SENDER, Contract._ERR_MISSING_KEY))
+        receivers = ensure_is_list(get_or_raise(multi_definition, Contract._KEY_RECEIVER, Contract._ERR_MISSING_KEY))
         if len(senders) > 1 and len(receivers) == 1:
             for index in range(len(senders)):
                 contracts.append(Contract._copy_contract(senders[index], receivers[0], base_data))
         elif len(senders) == 1 and len(receivers) > 1:
             for index in range(len(receivers)):
                 contracts.append(Contract._copy_contract(senders[0], receivers[index], base_data))
         elif len(senders) == len(receivers):
             for index in range(len(senders)):
                 contracts.append(Contract._copy_contract(senders[index], receivers[index], base_data))
         else:
-            log_and_raise(Contract._MULTI_CONTRACT_CORRUPT.format(senders, receivers))
+            log_and_raise(Contract._ERR_MULTI_CONTRACT_CORRUPT.format(senders, receivers))
         return contracts
 
     @staticmethod
     def _copy_contract(sender: int, receiver: int, base_data: dict) -> dict:
         """Returns a new contract definition dictionary, with given `sender` and `receiver` and copied `base_data`"""
-        contract = {}
-        contract[Contract._KEY_SENDER] = sender
-        contract[Contract._KEY_RECEIVER] = receiver
+        contract = {
+            Contract._KEY_SENDER: sender,
+            Contract._KEY_RECEIVER: receiver,
+        }
         contract.update(base_data)
         return contract
```

### Comparing `fameio-1.8.2/src/fameio/source/scenario/exception.py` & `fameio-2.0.0/src/fameio/source/scenario/exception.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 # SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
 #
 # SPDX-License-Identifier: Apache-2.0
 
-import logging as log
+from typing import NoReturn, Any, Union
 
-from fameio.source.logs import log_error_and_raise
+from fameio.source.logs import log_error_and_raise, logger
 
+_DEFAULT_USED = "Using default value '{}' for missing key '{}'"
 
-def log_and_raise(message: str):
+
+def log_and_raise(message: str) -> NoReturn:
     """Raises ScenarioException with given `message`"""
     log_error_and_raise(ScenarioException(message))
 
 
-def get_or_raise(dictionary: dict, key: str, message: str):
+def get_or_raise(dictionary: dict, key: str, message: str) -> Union[Any, NoReturn]:
     """Returns value associated with `key` in given `dictionary`, or raises ScenarioException if key is missing"""
     if key not in dictionary or dictionary[key] is None:
         log_error_and_raise(ScenarioException(message.format(key)))
     else:
         return dictionary[key]
 
 
-def assert_or_raise(assertion: bool, message: str):
-    """Raises ScenarioException with given `message` if `assertion` is `False`"""
+def assert_or_raise(assertion: bool, msg: str) -> None:
+    """Raises new ScenarioException with given `msg` if `assertion` is False"""
     if not assertion:
-        log_error_and_raise(ScenarioException(message))
+        log_error_and_raise(ScenarioException(msg))
 
 
-def get_or_default(dictionary: dict, key: str, default_value):
+def get_or_default(dictionary: dict, key: str, default_value) -> Any:
     """Returns value associated with `key` in given `dictionary`, or the given `default_value` if key is missing"""
     if key in dictionary and dictionary[key] is not None:
         return dictionary[key]
     else:
-        log.debug("Using default value '{}' for missing key '{}'".format(default_value, key))
+        logger().debug(_DEFAULT_USED.format(default_value, key))
         return default_value
 
 
 class ScenarioException(Exception):
     """Indicates an error while parsing a scenario or one of its components"""
 
     pass
```

### Comparing `fameio-1.8.2/src/fameio/source/scenario/fameiofactory.py` & `fameio-2.0.0/src/fameio/source/scenario/fameiofactory.py`

 * *Files identical despite different names*

### Comparing `fameio-1.8.2/src/fameio/source/scenario/generalproperties.py` & `fameio-2.0.0/src/fameio/source/scenario/generalproperties.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
 #
 # SPDX-License-Identifier: Apache-2.0
+from __future__ import annotations
 
-import logging as log
-
+from fameio.source.logs import logger
 from fameio.source.scenario.exception import get_or_default, get_or_raise
 from fameio.source.time import FameTime
 from fameio.source.tools import keys_to_lower
 
 
 class GeneralProperties:
     """Hosts general properties of a scenario"""
@@ -30,24 +30,24 @@
         simulation_start_time: int,
         simulation_stop_time: int,
         simulation_random_seed: int,
         output_interval: int,
         output_process: int,
     ) -> None:
         if simulation_stop_time < simulation_start_time:
-            log.warning(GeneralProperties._SIMULATION_DURATION)
+            logger().warning(GeneralProperties._SIMULATION_DURATION)
         self._run_id = run_id
         self._simulation_start_time = simulation_start_time
         self._simulation_stop_time = simulation_stop_time
         self._simulation_random_seed = simulation_random_seed
         self._output_interval = output_interval
         self._output_process = output_process
 
     @classmethod
-    def from_dict(cls, definitions: dict) -> "GeneralProperties":
+    def from_dict(cls, definitions: dict) -> GeneralProperties:
         """Parse general properties from provided `definitions`"""
         definitions = keys_to_lower(definitions)
         run_id = get_or_default(definitions, GeneralProperties._KEY_RUN, 1)
 
         simulation_definition = keys_to_lower(
             get_or_raise(
                 definitions,
@@ -75,29 +75,23 @@
         output_interval = get_or_default(output_definitions, GeneralProperties._KEY_INTERVAL, 100)
         output_process = get_or_default(output_definitions, GeneralProperties._KEY_PROCESS, 0)
 
         return cls(run_id, start_time, stop_time, random_seed, output_interval, output_process)
 
     def to_dict(self) -> dict:
         """Serializes the general properties to a dict"""
-        result = {}
-
-        result[self._KEY_RUN] = self.run_id
-
-        simulation_dict = {}
-        simulation_dict[self._KEY_START] = self.simulation_start_time
-        simulation_dict[self._KEY_STOP] = self.simulation_stop_time
-        simulation_dict[self._KEY_SEED] = self.simulation_random_seed
+        result = {self._KEY_RUN: self._run_id}
+        simulation_dict = {
+            self._KEY_START: self.simulation_start_time,
+            self._KEY_STOP: self.simulation_stop_time,
+            self._KEY_SEED: self.simulation_random_seed,
+        }
         result[self._KEY_SIMULATION] = simulation_dict
-
-        output_dict = {}
-        output_dict[self._KEY_INTERVAL] = self.output_interval
-        output_dict[self._KEY_PROCESS] = self.output_process
+        output_dict = {self._KEY_INTERVAL: self.output_interval, self._KEY_PROCESS: self.output_process}
         result[self._KEY_OUTPUT] = output_dict
-
         return result
 
     @property
     def run_id(self) -> int:
         """Returns the run ID"""
         return self._run_id
```

### Comparing `fameio-1.8.2/src/fameio/source/scenario/scenario.py` & `fameio-2.0.0/src/fameio/source/scenario/scenario.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-# SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
+# SPDX-FileCopyrightText: 2024 German Aerospace Center <fame@dlr.de>
 #
 # SPDX-License-Identifier: Apache-2.0
+from __future__ import annotations
 
 from typing import List
 
 from fameio.source.scenario.agent import Agent
 from fameio.source.scenario.contract import Contract
 from fameio.source.scenario.exception import get_or_default, get_or_raise
 from fameio.source.scenario.fameiofactory import FameIOFactory
@@ -26,45 +27,49 @@
     def __init__(self, schema: Schema, general_props: GeneralProperties) -> None:
         self._schema = schema
         self._general_props = general_props
         self._agents = []
         self._contracts = []
 
     @classmethod
-    def from_dict(cls, definitions: dict, factory=FameIOFactory()) -> "Scenario":
+    def from_dict(cls, definitions: dict, factory=FameIOFactory()) -> Scenario:
         """Parse scenario from provided `definitions` using given `factory`"""
         definitions = keys_to_lower(definitions)
 
         schema = factory.new_schema_from_dict(get_or_raise(definitions, Scenario._KEY_SCHEMA, Scenario._MISSING_KEY))
         general_props = factory.new_general_properties_from_dict(
             get_or_raise(definitions, Scenario._KEY_GENERAL, Scenario._MISSING_KEY)
         )
-        result = cls(schema, general_props)
+        scenario = cls(schema, general_props)
 
         for agent_definition in get_or_default(definitions, Scenario._KEY_AGENTS, []):
-            result.add_agent(factory.new_agent_from_dict(agent_definition))
+            scenario.add_agent(factory.new_agent_from_dict(agent_definition))
 
-        for multi_definition in get_or_default(definitions, Scenario._KEY_CONTRACTS, []):
-            for single_contract_definition in Contract.split_contract_definitions(multi_definition):
-                result.add_contract(factory.new_contract_from_dict(single_contract_definition))
+        for multi_contract_definition in get_or_default(definitions, Scenario._KEY_CONTRACTS, []):
+            for single_contract_definition in Contract.split_contract_definitions(multi_contract_definition):
+                scenario.add_contract(factory.new_contract_from_dict(single_contract_definition))
 
-        return result
+        return scenario
 
     def to_dict(self) -> dict:
         """Serializes the scenario content to a dict"""
         result = {
             Scenario._KEY_GENERAL: self.general_properties.to_dict(),
             Scenario._KEY_SCHEMA: self.schema.to_dict(),
-            Scenario._KEY_AGENTS: [],
         }
-        for agent in self.agents:
-            result[Scenario._KEY_AGENTS].append(agent.to_dict())
-        result[Scenario._KEY_CONTRACTS] = []
-        for contract in self.contracts:
-            result[Scenario._KEY_CONTRACTS].append(contract.to_dict())
+
+        if self.agents:
+            result[Scenario._KEY_AGENTS] = []
+            for agent in self.agents:
+                result[Scenario._KEY_AGENTS].append(agent.to_dict())
+
+        if self.contracts:
+            result[Scenario._KEY_CONTRACTS] = []
+            for contract in self.contracts:
+                result[Scenario._KEY_CONTRACTS].append(contract.to_dict())
         return result
 
     @property
     def agents(self) -> List[Agent]:
         """Returns all the agents of this scenario as a list"""
         return self._agents
```

### Comparing `fameio-1.8.2/src/fameio/source/schema/agenttype.py` & `fameio-2.0.0/src/fameio/source/schema/agenttype.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,84 +1,132 @@
 # SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
 #
 # SPDX-License-Identifier: Apache-2.0
+from __future__ import annotations
 
-import logging as log
 from typing import Dict, List, Any
 
-from fameio.source.logs import log_error_and_raise
+from fameio.source.logs import log_error_and_raise, logger
 from fameio.source.schema.exception import SchemaException
 from fameio.source.schema.attribute import AttributeSpecs
 from fameio.source.tools import keys_to_lower
 
 
 class AgentType:
     """Schema definitions for an Agent type"""
 
-    _ERR_PRODUCTS_NO_STRING_LIST = "Product definition of AgentType '{}' contains item(s) other than string: '{}'"
+    _ERR_NAME_INVALID = "'{}' is not a valid name for AgentTypes"
+    _ERR_PRODUCTS_NO_STRING = "Product definition of AgentType '{}' contains item(s) / key(s) other than string: '{}'"
     _ERR_PRODUCTS_UNKNOWN_STRUCTURE = "Product definition of AgentType '{}' is neither list nor dictionary: '{}'"
 
     _NO_ATTRIBUTES = "Agent '{}' has no specified 'Attributes'."
     _NO_PRODUCTS = "Agent '{}' has no specified 'Products'."
+    _NO_OUTPUTS = "Agent '{}' has no specified 'Outputs'."
+    _NO_METADATA = "Agent '{}' has no specified 'Metadata'."
 
     _KEY_ATTRIBUTES = "Attributes".lower()
     _KEY_PRODUCTS = "Products".lower()
+    _KEY_OUTPUTS = "Outputs".lower()
+    _KEY_METADATA = "MetaData".lower()
 
     def __init__(self, name: str):
+        """
+        Initialise a new AgentType
+
+        Args:
+            name: name of the AgenType - must not be None or empty
+        """
+        if not name or name.isspace():
+            log_error_and_raise(SchemaException(AgentType._ERR_NAME_INVALID.format(name)))
         self._name = name
         self._attributes = {}
-        self._products = []
+        self._products = {}
+        self._outputs = {}
+        self._metadata = {}
 
     @classmethod
-    def from_dict(cls, name: str, definitions: dict) -> "AgentType":
-        """Loads an agent type `definition` from the given input dict"""
-        definition = keys_to_lower(definitions)
+    def from_dict(cls, name: str, definitions: dict) -> AgentType:
+        """
+        Creates AgentType with given `name` from specified dictionary
+
+        Args:
+            name: of the agent type
+            definitions: of the agent type specifying, e.g., its attributes and products
+
+        Returns:
+            a new instance of AgentType
+        """
+        agent_type = cls(name)
 
-        result = cls(name)
+        definition = keys_to_lower(definitions)
         if AgentType._KEY_ATTRIBUTES in definition:
             for attribute_name, attribute_details in definition[AgentType._KEY_ATTRIBUTES].items():
                 full_name = name + "." + attribute_name
-                result._attributes[attribute_name] = AttributeSpecs(full_name, attribute_details)
+                agent_type._attributes[attribute_name] = AttributeSpecs(full_name, attribute_details)
+        else:
+            logger().info(AgentType._NO_ATTRIBUTES.format(name))
+
+        if AgentType._KEY_PRODUCTS in definition and definition[AgentType._KEY_PRODUCTS]:
+            agent_type._products.update(AgentType._read_products(definition[AgentType._KEY_PRODUCTS], name))
+        else:
+            logger().info(AgentType._NO_PRODUCTS.format(name))
+
+        if AgentType._KEY_OUTPUTS in definition:
+            outputs_to_add = definition[AgentType._KEY_OUTPUTS]
+            if outputs_to_add:
+                agent_type._outputs.update(outputs_to_add)
+        else:
+            logger().debug(AgentType._NO_OUTPUTS.format(name))
+
+        if AgentType._KEY_METADATA in definition:
+            metadata_to_add = definition[AgentType._KEY_METADATA]
+            if metadata_to_add:
+                agent_type._metadata.update(metadata_to_add)
         else:
-            log.info(AgentType._NO_ATTRIBUTES.format(name))
+            logger().debug(AgentType._NO_METADATA.format(name))
 
-        if AgentType._KEY_PRODUCTS in definition:
-            products_to_add = definition[AgentType._KEY_PRODUCTS]
-            if products_to_add:
-                result._products.extend(AgentType.read_products(products_to_add, name))
-
-        if not result._products:
-            log.info(AgentType._NO_PRODUCTS.format(name))
-        return result
+        return agent_type
 
     @staticmethod
-    def read_products(products: Any, agent_type: str) -> List[str]:
-        """Returns a list of product names obtained from given `products` defined for `agent_type`"""
+    def _read_products(products: Any, agent_type: str) -> Dict[str, Any]:
+        """Returns a dict obtained from given `products` defined for `agent_type`"""
         product_names = None
         if isinstance(products, dict):
-            product_names = [key for key in products.keys()]
-        elif isinstance(products, list):
             product_names = products
+        elif isinstance(products, list):
+            product_names = {key: None for key in products}
         else:
             log_error_and_raise(SchemaException(AgentType._ERR_PRODUCTS_UNKNOWN_STRUCTURE.format(agent_type, products)))
 
-        if all([isinstance(item, str) for item in product_names]):
+        if all([isinstance(item, str) for item in product_names.keys()]):
             return product_names
         else:
-            log_error_and_raise(
-                SchemaException(AgentType._ERR_PRODUCTS_NO_STRING_LIST.format(agent_type, product_names))
-            )
+            log_error_and_raise(SchemaException(AgentType._ERR_PRODUCTS_NO_STRING.format(agent_type, product_names)))
 
     @property
     def name(self) -> str:
         """Returns the agent type name"""
         return self._name
 
     @property
-    def products(self) -> list:
-        """Returns list of products or an empty list if no products are defined"""
+    def products(self) -> dict:
+        """Returns dict of products or an empty dict if no products are defined"""
         return self._products
 
+    def get_product_names(self) -> List[str]:
+        """Returns list of product names or an empty list if no products are defined"""
+        return list(self._products.keys())
+
     @property
     def attributes(self) -> Dict[str, AttributeSpecs]:
         """Returns list of Attributes of this agent or an empty list if no attributes are defined"""
         return self._attributes
+
+    @property
+    def outputs(self) -> dict:
+        """Returns list of outputs or an empty list if no outputs are defined"""
+        return self._outputs
+
+    @property
+    def metadata(self) -> dict:
+        """Returns list of metadata or an empty list if no metadata are defined"""
+        return self._metadata
```

### Comparing `fameio-1.8.2/src/fameio/source/schema/attribute.py` & `fameio-2.0.0/src/fameio/source/schema/attribute.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
 #
 # SPDX-License-Identifier: Apache-2.0
+from __future__ import annotations
 
-import logging as log
 import typing
 from enum import Enum, auto
 from typing import Any, Dict
 
+from fameio.source.logs import logger
 from fameio.source.schema.exception import SchemaException
 from fameio.source.time import FameTime
 from fameio.source.tools import keys_to_lower
 
 
 class AttributeType(Enum):
     """Specifies known types that Attributes can take"""
@@ -45,15 +46,15 @@
 
     _MISSING_SPEC_DEFAULT = "Missing '{}' specification for Attribute '{}' - assuming {}."
     _MISSING_TYPE = "'AttributeType' not declare for Attribute '{}'."
     _INVALID_TYPE = "'{}' is not a valid type for an Attribute."
     _DEFAULT_NOT_LIST = "Attribute is list, but provided Default '{}' is not a list."
     _DEFAULT_INCOMPATIBLE = "Default '{}' can not be converted to AttributeType '{}'."
     _DEFAULT_DISALLOWED = "Default '{}' is not an allowed value."
-    _LIST_DISALLOWED = "Attribute '{}' of type TIME_SERIES cannot be list."
+    _LIST_DISALLOWED = "Attribute '{}' of type TIME_SERIES cannot be a list."
     _VALUES_ILL_FORMAT = "Only List and Dictionary is supported for 'Values' but was: {}"
 
     _KEY_MANDATORY = "Mandatory".lower()
     _KEY_LIST = "List".lower()
     _KEY_TYPE = "AttributeType".lower()
     _KEY_NESTED = "NestedAttributes".lower()
     _KEY_VALUES = "Values".lower()
@@ -65,26 +66,26 @@
         self._full_name = name
         definition = keys_to_lower(definition)
 
         if AttributeSpecs._KEY_MANDATORY in definition:
             self._is_mandatory = definition[AttributeSpecs._KEY_MANDATORY]
         else:
             self._is_mandatory = True
-            log.warning(AttributeSpecs._MISSING_SPEC_DEFAULT.format(AttributeSpecs._KEY_MANDATORY, name, True))
+            logger().warning(AttributeSpecs._MISSING_SPEC_DEFAULT.format(AttributeSpecs._KEY_MANDATORY, name, True))
 
         if AttributeSpecs._KEY_LIST in definition:
             self._is_list = definition[AttributeSpecs._KEY_LIST]
         else:
             self._is_list = False
-            log.warning(AttributeSpecs._MISSING_SPEC_DEFAULT.format(AttributeSpecs._KEY_LIST, name, False))
+            logger().warning(AttributeSpecs._MISSING_SPEC_DEFAULT.format(AttributeSpecs._KEY_LIST, name, False))
 
         if AttributeSpecs._KEY_TYPE in definition:
             self._attr_type = AttributeSpecs._get_type_for_name(definition[AttributeSpecs._KEY_TYPE])
         else:
-            log.error(AttributeSpecs._MISSING_TYPE.format(name))
+            logger().error(AttributeSpecs._MISSING_TYPE.format(name))
             raise SchemaException(AttributeSpecs._MISSING_TYPE.format(name))
 
         if self._attr_type == AttributeType.TIME_SERIES and self._is_list:
             raise SchemaException(AttributeSpecs._LIST_DISALLOWED.format(name))
 
         self._values = []
         if AttributeSpecs._KEY_VALUES in definition:
@@ -179,23 +180,23 @@
 
     @property
     def full_name(self) -> str:
         """Returns name including name of enclosing parent attributes"""
         return self._full_name
 
     @staticmethod
-    def _get_type_for_name(name: str) -> "AttributeType":
+    def _get_type_for_name(name: str) -> AttributeType:
         """Returns the AttributeType matching the given `name` converted to upper case"""
         try:
             return AttributeType[name.upper()]
         except KeyError:
             raise SchemaException(AttributeSpecs._INVALID_TYPE.format(name))
 
     @property
     def has_help_text(self) -> bool:
         """Return True if a help_text is available"""
         return bool(self._help)
 
     @property
     def help_text(self) -> str:
-        """Return the help_text of this attribute, if any"""
+        """Return the help_text of this attribute, if any, otherwise an empty string"""
         return self._help if self.has_help_text else ""
```

### Comparing `fameio-1.8.2/src/fameio/source/time.py` & `fameio-2.0.0/src/fameio/source/time.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
 #
 # SPDX-License-Identifier: Apache-2.0
 
 import datetime as dt
 import math
 import re
-from enum import Enum
+from enum import Enum, auto
 from typing import Union
 
 from fameio.source.logs import log_error_and_raise
 
 START_IN_REAL_TIME = "2000-01-01_00:00:00"
 DATE_FORMAT = "%Y-%m-%d_%H:%M:%S"
 DATE_REGEX = re.compile("[0-9]{4}-[0-9]{2}-[0-9]{2}_[0-9]{2}:[0-9]{2}:[0-9]{2}")
@@ -21,21 +21,21 @@
 
     pass
 
 
 class TimeUnit(Enum):
     """Time units defined in FAME"""
 
-    SECONDS = 0
-    MINUTES = 1
-    HOURS = 2
-    DAYS = 3
-    WEEKS = 4
-    MONTHS = 5
-    YEARS = 6
+    SECONDS = auto()
+    MINUTES = auto()
+    HOURS = auto()
+    DAYS = auto()
+    WEEKS = auto()
+    MONTHS = auto()
+    YEARS = auto()
 
 
 class Constants:
     """Time steps in FAME simulations associated with corresponding TimeUnits"""
 
     FIRST_YEAR = 2000
     STEPS_PER_SECOND = 1
```

### Comparing `fameio-1.8.2/src/fameio/source/validator.py` & `fameio-2.0.0/src/fameio/source/validator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
 #
 # SPDX-License-Identifier: Apache-2.0
 
-import logging as log
+import math
 from collections import Counter
 from typing import Any, Dict, List
 
-from fameio.source.logs import log_error_and_raise
+from fameio.source import PathResolver
+from fameio.source.logs import log_error_and_raise, logger
 from fameio.source.scenario import Agent, Attribute, Contract, Scenario
 from fameio.source.schema.agenttype import AgentType
 from fameio.source.schema.attribute import AttributeSpecs, AttributeType
 from fameio.source.schema.schema import Schema
+from fameio.source.series import TimeSeriesManager, TimeSeriesException
 from fameio.source.time import FameTime
 
 
 class ValidationException(Exception):
     """Indicates an error occurred during validation of any data with a connected schema"""
 
     pass
@@ -32,136 +34,231 @@
     _AGENT_MISSING = "Contract mentions Agent with ID '{}' but Agent was not declared."
     _PRODUCT_MISSING = "Product '{}' not declared in Schema for AgentType '{}'."
     _KEY_MISSING = "Required key '{}' missing in dictionary '{}'."
     _ATTRIBUTE_MISSING = "Mandatory attribute '{}' is missing."
     _DEFAULT_IGNORED = "Optional Attribute: '{}': not specified - provided Default ignored for optional Attributes."
     _OPTIONAL_MISSING = "Optional Attribute: '{}': not specified."
     _IS_NO_LIST = "Attribute '{}' is list but assigned value '{}' is not a list."
+    _TIME_SERIES_INVALID = "Timeseries at '{}' is invalid."
+    _MISSING_CONTRACTS_FOR_AGENTS = "No contracts defined for Agent '{}' of type '{}'"
+
+    @staticmethod
+    def validate_scenario_and_timeseries(
+        scenario: Scenario, path_resolver: PathResolver = PathResolver()
+    ) -> TimeSeriesManager:
+        """
+        Validates the given `scenario` and its timeseries using given `path_resolver`
+        Raises an exception if schema requirements are not met or timeseries data are erroneous.
+
+        Args:
+            scenario: to be validated against the encompassed schema
+            path_resolver: to resolve paths of timeseries
+
+        Returns:
+            a new TimeSeriesManager initialised with validated time series from scenario
+        Raises:
+            ValidationException: if an error in the scenario or in timeseries is spotted
+        """
+        schema = scenario.schema
+        agents = scenario.agents
+        timeseries_manager = TimeSeriesManager(path_resolver)
+
+        SchemaValidator.ensure_unique_agent_ids(agents)
+        for agent in agents:
+            SchemaValidator.ensure_agent_and_timeseries_are_valid(agent, schema, timeseries_manager)
+
+        agent_types_by_id = {agent.id: agent.type_name for agent in agents}
+        for contract in scenario.contracts:
+            SchemaValidator.ensure_is_valid_contract(contract, schema, agent_types_by_id)
+
+        return timeseries_manager
+
+    @staticmethod
+    def ensure_unique_agent_ids(agents: List[Agent]) -> None:
+        """Raises exception if any id for given `agents` is not unique"""
+        list_of_ids = [agent.id for agent in agents]
+        non_unique_ids = [agent_id for agent_id, count in Counter(list_of_ids).items() if count > 1]
+        if non_unique_ids:
+            log_error_and_raise(ValidationException(SchemaValidator._AGENT_ID_NOT_UNIQUE.format(non_unique_ids)))
+
+    @staticmethod
+    def ensure_agent_and_timeseries_are_valid(agent: Agent, schema: Schema, timeseries_manager: TimeSeriesManager):
+        """Validates given `agent` against `schema` plus loads and validates its timeseries"""
+        SchemaValidator.ensure_agent_type_in_schema(agent, schema)
+        SchemaValidator.ensure_is_valid_agent(agent, schema)
+        SchemaValidator.load_and_validate_timeseries(agent, schema, timeseries_manager)
+
+    @staticmethod
+    def ensure_agent_type_in_schema(agent: Agent, schema: Schema) -> None:
+        """Raises exception if type for given `agent` is not specified in given `schema`"""
+        if agent.type_name not in schema.agent_types:
+            log_error_and_raise(ValidationException(SchemaValidator._AGENT_TYPE_UNKNOWN.format(agent.type_name)))
+
+    @staticmethod
+    def ensure_is_valid_agent(agent: Agent, schema: Schema) -> None:
+        """Raises an exception if given `agent` does not meet the specified `schema` requirements"""
+        scenario_attributes = agent.attributes
+        schema_attributes = SchemaValidator._get_agent(schema, agent.type_name).attributes
+        SchemaValidator._ensure_mandatory_present(scenario_attributes, schema_attributes)
+        SchemaValidator._ensure_attributes_exist(scenario_attributes, schema_attributes)
+        SchemaValidator._ensure_value_and_type_match(scenario_attributes, schema_attributes)
+
+    @staticmethod
+    def _get_agent(schema: Schema, name: str) -> AgentType:
+        """Returns agent specified by `name` or raises Exception if this agent is not present in given `schema`"""
+        if name in schema.agent_types:
+            return schema.agent_types[name]
+        else:
+            log_error_and_raise(ValidationException(SchemaValidator._AGENT_TYPE_UNKNOWN.format(name)))
 
     @staticmethod
     def _ensure_mandatory_present(attributes: Dict[str, Attribute], specifications: Dict[str, AttributeSpecs]) -> None:
         """
         Raises Exception if in given list of `specifications` at least one item is mandatory,
         provides no defaults and is not contained in given `attributes` dictionary
         """
         for name, specification in specifications.items():
             if name not in attributes:
                 if specification.is_mandatory:
                     if not specification.has_default_value:
-                        log_error_and_raise(ValidationException(SchemaValidator._ATTRIBUTE_MISSING.format(name)))
+                        log_error_and_raise(
+                            ValidationException(SchemaValidator._ATTRIBUTE_MISSING.format(specification.full_name))
+                        )
                 else:
                     if specification.has_default_value:
-                        log.warning(SchemaValidator._DEFAULT_IGNORED.format(name))
+                        logger().warning(SchemaValidator._DEFAULT_IGNORED.format(specification.full_name))
                     else:
-                        log.info(SchemaValidator._OPTIONAL_MISSING.format(name))
+                        logger().info(SchemaValidator._OPTIONAL_MISSING.format(specification.full_name))
             if name in attributes and specification.has_nested_attributes:
                 attribute = attributes[name]
                 if specification.is_list:
                     for entry in attribute.nested_list:
                         SchemaValidator._ensure_mandatory_present(entry, specification.nested_attributes)
                 else:
                     SchemaValidator._ensure_mandatory_present(attribute.nested, specification.nested_attributes)
 
     @staticmethod
-    def _get_agent(schema: Schema, name: str) -> AgentType:
-        """Returns agent specified by `name` or raises Exception if this agent is not present in given `schema`"""
-        if name in schema.agent_types:
-            return schema.agent_types[name]
-        else:
-            log_error_and_raise(ValidationException(SchemaValidator._AGENT_TYPE_UNKNOWN.format(name)))
-
-    @staticmethod
-    def ensure_is_valid_agent(agent: Agent, schema: Schema) -> None:
-        """Raises an exception if given `agent` does not meet the specified `schema` requirements"""
-        scenario_attributes = agent.attributes
-        schema_attributes = SchemaValidator._get_agent(schema, agent.type_name).attributes
-        SchemaValidator._ensure_mandatory_present(scenario_attributes, schema_attributes)
-        SchemaValidator._ensure_attributes_exist(scenario_attributes, schema_attributes)
-        SchemaValidator._ensure_value_matches_type(scenario_attributes, schema_attributes)
-
-    @staticmethod
     def _ensure_attributes_exist(attributes: Dict[str, Attribute], specifications: Dict[str, AttributeSpecs]) -> None:
         """Raises exception any entry of given `attributes` has no corresponding type `specification`"""
         for name, attribute in attributes.items():
             if name not in specifications:
                 log_error_and_raise(ValidationException(SchemaValidator._ATTRIBUTE_UNKNOWN.format(attribute)))
             if attribute.has_nested:
                 specification = specifications[name]
                 SchemaValidator._ensure_attributes_exist(attribute.nested, specification.nested_attributes)
             if attribute.has_nested_list:
                 specification = specifications[name]
                 for entry in attribute.nested_list:
                     SchemaValidator._ensure_attributes_exist(entry, specification.nested_attributes)
 
     @staticmethod
-    def _ensure_value_matches_type(attributes: Dict[str, Attribute], specifications: Dict[str, AttributeSpecs]) -> None:
+    def _ensure_value_and_type_match(
+        attributes: Dict[str, Attribute], specifications: Dict[str, AttributeSpecs]
+    ) -> None:
         """Raises exception if in given list of `attributes` its value does not match associated type `specification`"""
         for name, attribute in attributes.items():
             specification = specifications[name]
             if attribute.has_value:
                 value = attribute.value
                 type_spec = specification.attr_type
                 if not SchemaValidator._is_compatible(specification, value):
                     message = SchemaValidator._INCOMPATIBLE.format(value, type_spec, specification.full_name)
                     log_error_and_raise(ValidationException(message))
                 if not SchemaValidator._is_allowed_value(specification, value):
-                    log_error_and_raise(
-                        ValidationException(SchemaValidator._DISALLOWED.format(value, specification.full_name))
-                    )
+                    message = SchemaValidator._DISALLOWED.format(value, specification.full_name)
+                    log_error_and_raise(ValidationException(message))
             if attribute.has_nested:
-                SchemaValidator._ensure_value_matches_type(attribute.nested, specification.nested_attributes)
+                SchemaValidator._ensure_value_and_type_match(attribute.nested, specification.nested_attributes)
             if attribute.has_nested_list:
                 for entry in attribute.nested_list:
-                    SchemaValidator._ensure_value_matches_type(entry, specification.nested_attributes)
+                    SchemaValidator._ensure_value_and_type_match(entry, specification.nested_attributes)
 
     @staticmethod
     def _is_compatible(specification: AttributeSpecs, value_or_values: Any) -> bool:
         """Returns True if given `value_or_values` is compatible to specified `attribute_type` and `should_be_list`"""
         is_list = isinstance(value_or_values, list)
         attribute_type = specification.attr_type
         if specification.is_list:
             if not is_list:
-                log.warning(SchemaValidator._IS_NO_LIST.format(specification.full_name, value_or_values))
+                logger().warning(SchemaValidator._IS_NO_LIST.format(specification.full_name, value_or_values))
                 return SchemaValidator._is_compatible_value(attribute_type, value_or_values)
             for value in value_or_values:
                 if not SchemaValidator._is_compatible_value(attribute_type, value):
                     return False
             return True
         else:
             return (not is_list) and SchemaValidator._is_compatible_value(attribute_type, value_or_values)
 
     @staticmethod
     def _is_compatible_value(attribute_type: AttributeType, value) -> bool:
-        """Returns True if given single value is compatible to specified `attribute_type`"""
+        """Returns True if given single value is compatible to specified `attribute_type` and is not a NaN float"""
         if attribute_type is AttributeType.INTEGER:
             if isinstance(value, int):
                 return -2147483648 < value < 2147483647
             return False
         if attribute_type is AttributeType.LONG:
             return isinstance(value, int)
         elif attribute_type is AttributeType.DOUBLE:
-            return isinstance(value, (int, float))
+            return isinstance(value, (int, float)) and not math.isnan(value)
         elif attribute_type in (AttributeType.ENUM, AttributeType.STRING):
             return isinstance(value, str)
         elif attribute_type is AttributeType.TIME_STAMP:
             return FameTime.is_fame_time_compatible(value)
         elif attribute_type is AttributeType.TIME_SERIES:
-            return isinstance(value, (str, int, float))
+            return isinstance(value, (str, int)) or (isinstance(value, float) and not math.isnan(value))
         else:
             log_error_and_raise(ValidationException(SchemaValidator._TYPE_NOT_IMPLEMENTED.format(attribute_type)))
 
     @staticmethod
     def _is_allowed_value(attribute: AttributeSpecs, value) -> bool:
         """Returns True if `value` matches an entry of given `Attribute`'s value list or if this list is empty"""
         if not attribute.values:
             return True
         else:
             return value in attribute.values
 
     @staticmethod
+    def load_and_validate_timeseries(agent: Agent, schema: Schema, timeseries_manager: TimeSeriesManager) -> None:
+        """
+        Loads all timeseries specified in given `schema` of given `agent` into given `timeseries_manager`
+
+        Args:
+            agent: definition in scenario
+            schema: schema encompassed in scenario
+            timeseries_manager: to be filled with timeseries
+
+        Raises:
+            ValidationException: if timeseries is not found, ill-formatted or invalid
+        """
+        scenario_attributes = agent.attributes
+        schema_attributes = SchemaValidator._get_agent(schema, agent.type_name).attributes
+        SchemaValidator._ensure_valid_timeseries(scenario_attributes, schema_attributes, timeseries_manager)
+
+    @staticmethod
+    def _ensure_valid_timeseries(
+        attributes: Dict[str, Attribute], specifications: Dict[str, AttributeSpecs], manager: TimeSeriesManager
+    ) -> None:
+        """Recursively searches for time_series in agent attributes and registers them at given `manager`"""
+        for name, attribute in attributes.items():
+            specification = specifications[name]
+            if attribute.has_value:
+                attribute_type = specification.attr_type
+                if attribute_type is AttributeType.TIME_SERIES:
+                    try:
+                        manager.register_and_validate(attribute.value)
+                    except TimeSeriesException as e:
+                        message = SchemaValidator._TIME_SERIES_INVALID.format(specification.full_name)
+                        log_error_and_raise(ValidationException(message, e))
+            if attribute.has_nested:
+                SchemaValidator._ensure_valid_timeseries(attribute.nested, specification.nested_attributes, manager)
+            if attribute.has_nested_list:
+                for entry in attribute.nested_list:
+                    SchemaValidator._ensure_valid_timeseries(entry, specification.nested_attributes, manager)
+
+    @staticmethod
     def ensure_is_valid_contract(contract: Contract, schema: Schema, agent_types_by_id: Dict[int, str]) -> None:
         """Raises exception if given `contract` does not meet the `schema`'s requirements, using `agent_types_by_id`"""
         sender_id = contract.sender_id
         if sender_id not in agent_types_by_id:
             log_error_and_raise(ValidationException(SchemaValidator._AGENT_MISSING.format(sender_id)))
         if contract.receiver_id not in agent_types_by_id:
             log_error_and_raise(ValidationException(SchemaValidator._AGENT_MISSING.format(contract.receiver_id)))
@@ -170,34 +267,17 @@
             log_error_and_raise(ValidationException(SchemaValidator._AGENT_TYPE_UNKNOWN.format(sender_type_name)))
         sender_type = schema.agent_types[sender_type_name]
         product = contract.product_name
         if product not in sender_type.products:
             log_error_and_raise(ValidationException(SchemaValidator._PRODUCT_MISSING.format(product, sender_type_name)))
 
     @staticmethod
-    def ensure_unique_agent_ids(agents: List[Agent]) -> None:
-        """Raises exception if any id for given `agents` is not unique"""
-        list_of_ids = [agent.id for agent in agents]
-        non_unique_ids = [agent_id for agent_id, count in Counter(list_of_ids).items() if count > 1]
-        if non_unique_ids:
-            log_error_and_raise(ValidationException(SchemaValidator._AGENT_ID_NOT_UNIQUE.format(non_unique_ids)))
-
-    @staticmethod
-    def ensure_agent_type_in_schema(agent: Agent, schema: Schema) -> None:
-        """Raises exception if type for given `agent` is not specified in given `schema`"""
-        if agent.type_name not in schema.agent_types:
-            log_error_and_raise(ValidationException(SchemaValidator._AGENT_TYPE_UNKNOWN.format(agent.type_name)))
-
-    @staticmethod
-    def ensure_is_valid_scenario(scenario: Scenario) -> None:
-        """Raises exception if given `scenario` does not meet its own schema requirements"""
-        schema = scenario.schema
-        agents = scenario.agents
-
-        SchemaValidator.ensure_unique_agent_ids(agents)
-        for agent in agents:
-            SchemaValidator.ensure_agent_type_in_schema(agent, schema)
-            SchemaValidator.ensure_is_valid_agent(agent, schema)
-
-        agent_types_by_id = {agent.id: agent.type_name for agent in agents}
-        for contract in scenario.contracts:
-            SchemaValidator.ensure_is_valid_contract(contract, schema, agent_types_by_id)
+    def check_agents_have_contracts(scenario: Scenario) -> None:
+        """Raises warning for each agent without any assigned contract"""
+        senders = [contract.sender_id for contract in scenario.contracts]
+        receivers = [contract.receiver_id for contract in scenario.contracts]
+        active_agents = set(senders + receivers)
+        inactive_agents = {agent.id: agent.type_name for agent in scenario.agents if agent.id not in active_agents}
+
+        if inactive_agents:
+            for agent_id, agent_name in inactive_agents.items():
+                logger().warning(SchemaValidator._MISSING_CONTRACTS_FOR_AGENTS.format(agent_id, agent_name))
```

### Comparing `fameio-1.8.2/src/fameio/source/writer.py` & `fameio-2.0.0/src/fameio/source/writer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,234 +1,230 @@
 # SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
 #
 # SPDX-License-Identifier: Apache-2.0
 
-import logging as log
-import os.path
 from pathlib import Path
-from typing import Any, Dict
+from typing import Any, Dict, List, Union
 
-import pandas as pd
-from fameio.source.logs import log_error_and_raise
+from fameprotobuf.DataStorage_pb2 import DataStorage
+from fameprotobuf.InputFile_pb2 import InputData
+from fameprotobuf.Field_pb2 import NestedField
+from fameprotobuf.Contract_pb2 import ProtoContract
+
+from fameio.source.logs import log_error_and_raise, logger
+from fameio.source.results.reader import Reader
 from fameio.source.scenario import (
     Agent,
     Attribute,
     Contract,
     GeneralProperties,
     Scenario,
 )
-from fameio.source.path_resolver import PathResolver
+from fameio.source.schema import Schema
 from fameio.source.schema.attribute import AttributeSpecs, AttributeType
 from fameio.source.series import TimeSeriesManager
-from fameio.source.time import START_IN_REAL_TIME, ConversionException, FameTime
+from fameio.source.time import FameTime
 from fameio.source.tools import ensure_is_list
-from fameprotobuf import DataStorage_pb2
 
 
 class ProtoWriterException(Exception):
     """Indicates an error during writing of protobuf file"""
 
     pass
 
 
 class ProtoWriter:
     """Writes a given scenario to protobuf file"""
 
+    _FAME_PROTOBUF_STREAM_HEADER = "famecoreprotobufstreamfilev001"  # noqa
+
     _TYPE_NOT_IMPLEMENTED = "AttributeType '{}' not implemented."
-    _NOT_TIME_SERIES = "Cannot convert value '{}' to TimeSeries."
     _CONTRACT_UNSUPPORTED = (
         "Unsupported value for Contract Attribute '{}'; "
         "Only support `int`, `float`, `enum` or `dict` types are supported here."
     )
     _USING_DEFAULT = "Using provided Default for Attribute: '{}'."
-    _CORRUPT_TIME_SERIES_VALUE = "TimeSeries file '{}' is corrupt: At least one entry in value column is not numeric."
-    _CORRUPT_TIME_SERIES_KEY = "TimeSeries file '{}' is corrupt: At least one entry in first column is not a timestamp."
-    _TIME_SERIES_FILE_NOT_FOUND = "Cannot find TimeSeries file '{}'."
     _NO_FILE_SPECIFIED = "Could not write to '{}'. Please specify a valid output file."
 
-    def __init__(self, file_path: Path, path_resolver=PathResolver()) -> None:
-        self.file_path = file_path
-        self.time_series_manager = TimeSeriesManager()
-        self._path_resolver = path_resolver
+    _INFO_WRITING = "Writing scenario to protobuf file `{}`"
+    _INFO_WRITING_COMPLETED = "Saved protobuf file `{}` to disk"
+
+    def __init__(self, file_path: Path, time_series_manager: TimeSeriesManager) -> None:
+        self.file_path: Path = file_path
+        self._time_series_manager: TimeSeriesManager = time_series_manager
 
     def write_validated_scenario(self, scenario: Scenario) -> None:
         """Writes given validated Scenario to file"""
-        log.info("Writing scenario to protobuf file `{}`".format(self.file_path))
-        pb_data_storage = DataStorage_pb2.DataStorage()
-        pb_input = pb_data_storage.input
-
-        log.info("Adding General Properties")
-        ProtoWriter._set_general_properties(pb_input, scenario.general_properties)
-
-        log.info("Adding Agents")
-        schema = scenario.schema
-        for agent in scenario.agents:
-            pb_agent = ProtoWriter._set_agent(pb_input.agent.add(), agent)
-            attribute_specs = schema.agent_types[agent.type_name].attributes
-            self._set_attributes(pb_agent, agent.attributes, attribute_specs)
+        pb_data_storage = self._create_protobuf_from_scenario(scenario)
+        self._write_protobuf_to_disk(pb_data_storage)
 
-        log.info("Adding Contracts")
-        for contract in scenario.contracts:
-            pb_contract = ProtoWriter._set_contract(pb_input.contract.add(), contract)
-            ProtoWriter._set_contract_attributes(pb_contract, contract.attributes)
+    def _create_protobuf_from_scenario(self, scenario: Scenario) -> DataStorage:
+        """Returns given `scenario` written to new DataStorage protobuf"""
+        logger().info("Converting scenario to protobuf.")
+        pb_data_storage = DataStorage()
+        pb_input = pb_data_storage.input
 
-        log.info("Adding TimeSeries")
+        self._set_general_properties(pb_input, scenario.general_properties)
+        self._add_agents(pb_input, scenario.agents, scenario.schema)
+        self._add_contracts(pb_input, scenario.contracts)
         self._set_time_series(pb_input)
-        log.info("Writing to disk")
-        self._write_protobuf_to_disk(pb_data_storage)
+        self._set_schema(pb_input, scenario.schema)
+
+        return pb_data_storage
 
     @staticmethod
-    def _set_general_properties(pb_input, gen_props: GeneralProperties) -> None:
-        """Saves Scenario's general properties to specified protobuf `pb_input` container"""
-        pb_input.runId = gen_props.run_id
-        pb_input.simulation.startTime = gen_props.simulation_start_time
-        pb_input.simulation.stopTime = gen_props.simulation_stop_time
-        pb_input.simulation.randomSeed = gen_props.simulation_random_seed
-        pb_input.output.interval = gen_props.output_interval
-        pb_input.output.process = gen_props.output_process
+    def _set_general_properties(pb_input: InputData, general_properties: GeneralProperties) -> None:
+        """Saves a scenario's general properties to specified protobuf `pb_input` container"""
+        logger().info("Adding General Properties")
+        pb_input.runId = general_properties.run_id
+        pb_input.simulation.startTime = general_properties.simulation_start_time
+        pb_input.simulation.stopTime = general_properties.simulation_stop_time
+        pb_input.simulation.randomSeed = general_properties.simulation_random_seed
+        pb_input.output.interval = general_properties.output_interval
+        pb_input.output.process = general_properties.output_process
+
+    def _add_agents(self, pb_input: InputData, agents: List[Agent], schema: Schema) -> None:
+        """Triggers setting of `agents` to `pb_input`"""
+        logger().info("Adding Agents")
+        for agent in agents:
+            pb_agent = self._set_agent(pb_input.agent.add(), agent)
+            attribute_specs = schema.agent_types[agent.type_name].attributes
+            self._set_attributes(pb_agent, agent.attributes, attribute_specs)
+            pb_agent.metadata = repr(agent.meta_data)
 
     @staticmethod
-    def _set_agent(pb_agent, agent: Agent):
-        """Saves type and id of given `agent` to protobuf `pb_agent` container. Returns given `pb_agent`."""
+    def _set_agent(pb_agent: InputData.AgentDao, agent: Agent) -> InputData.AgentDao:
+        """Saves type and id of given `agent` to protobuf `pb_agent` container. Returns given `pb_agent`"""
         pb_agent.className = agent.type_name
         pb_agent.id = agent.id
         return pb_agent
 
     def _set_attributes(
         self,
-        pb_parent,
+        pb_parent: Union[InputData.AgentDao, NestedField],
         attributes: Dict[str, Attribute],
         specs: Dict[str, AttributeSpecs],
     ) -> None:
         """Assigns `attributes` to protobuf fields of given `pb_parent` - cascades for nested Attributes"""
         values_not_set = [key for key in specs.keys()]
         for name, attribute in attributes.items():
-            pb_field = ProtoWriter._add_field(pb_parent, name)
+            pb_field = self._add_field(pb_parent, name)
             attribute_specs = specs[name]
             values_not_set.remove(name)
             attribute_type = attribute_specs.attr_type
             if attribute_type is AttributeType.BLOCK:
                 if attribute_specs.is_list:
                     for index, entry in enumerate(attribute.nested_list):
-                        pb_inner = ProtoWriter._add_field(pb_field, str(index))
+                        pb_inner = self._add_field(pb_field, str(index))
                         self._set_attributes(pb_inner, entry, attribute_specs.nested_attributes)
                 else:
-                    self._set_attributes(
-                        pb_field,
-                        attribute.nested,
-                        attribute_specs.nested_attributes,
-                    )
+                    self._set_attributes(pb_field, attribute.nested, attribute_specs.nested_attributes)
             else:
                 self._set_attribute(pb_field, attribute.value, attribute_type)
         for name in values_not_set:
             attribute_specs = specs[name]
             if attribute_specs.is_mandatory:
-                pb_field = ProtoWriter._add_field(pb_parent, name)
+                pb_field = self._add_field(pb_parent, name)
                 self._set_attribute(pb_field, attribute_specs.default_value, attribute_specs.attr_type)
-                log.info(ProtoWriter._USING_DEFAULT.format(name))
+                logger().info(self._USING_DEFAULT.format(name))
 
     @staticmethod
-    def _add_field(pb_parent, name: str) -> Any:
+    def _add_field(pb_parent: Union[InputData.AgentDao, NestedField], name: str) -> NestedField:
         """Returns new field with given `name` that is added to given `pb_parent`"""
         pb_field = pb_parent.field.add()
         pb_field.fieldName = name
         return pb_field
 
-    def _set_attribute(self, pb_field, value, attribute_type: AttributeType) -> None:
+    def _set_attribute(self, pb_field: NestedField, value: Any, attribute_type: AttributeType) -> None:
         """Sets given `value` to given protobuf `pb_field` depending on specified `attribute_type`"""
         if attribute_type is AttributeType.INTEGER:
             pb_field.intValue.extend(ensure_is_list(value))
         elif attribute_type is AttributeType.DOUBLE:
             pb_field.doubleValue.extend(ensure_is_list(value))
         elif attribute_type is AttributeType.LONG:
             pb_field.longValue.extend(ensure_is_list(value))
         elif attribute_type is AttributeType.TIME_STAMP:
             pb_field.longValue.extend(ensure_is_list(FameTime.convert_string_if_is_datetime(value)))
         elif attribute_type in (AttributeType.ENUM, AttributeType.STRING):
             pb_field.stringValue.extend(ensure_is_list(value))
         elif attribute_type is AttributeType.TIME_SERIES:
-            self._set_time_series_from_value(pb_field, value)
+            pb_field.seriesId = self._time_series_manager.get_series_id_by_identifier(value)
         else:
-            log_error_and_raise(ProtoWriterException(ProtoWriter._TYPE_NOT_IMPLEMENTED.format(attribute_type)))
-
-    def _set_time_series_from_value(self, pb_field, value):
-        """Hands given `value` to TimeSeriesManager to assign a unique id which is then set to `pb_field`.seriesId"""
-        if not isinstance(value, (str, int, float)):
-            log_error_and_raise(ProtoWriterException(ProtoWriter._NOT_TIME_SERIES.format(str(value))))
-        elif isinstance(value, str):
-            value = Path(value).as_posix()
-        pb_field.seriesId = self.time_series_manager.save_get_time_series_id(value)
-
-    def _set_time_series(self, pb_input):
-        """Adds all time series from TimeSeriesManager to given `pb_input`"""
-        ids_of_series_by_name = self.time_series_manager.get_ids_of_series_by_name()
-        for identifier, unique_id in ids_of_series_by_name.items():
-            pb_series = pb_input.timeSeries.add()
-            pb_series.seriesId = unique_id
-            series_name, data_frame = self._get_series_as_dataframe(identifier)
-            pb_series.seriesName = series_name
-            try:
-                ProtoWriter._add_rows_to_series(pb_series, data_frame)
-            except TypeError:
-                log_error_and_raise(ProtoWriterException(ProtoWriter._CORRUPT_TIME_SERIES_VALUE.format(identifier)))
-            except ConversionException:
-                log_error_and_raise(ProtoWriterException(ProtoWriter._CORRUPT_TIME_SERIES_KEY.format(identifier)))
-
-    def _get_series_as_dataframe(self, identifier) -> (str, pd.DataFrame):
-        """Returns a DataFrame containing the series obtained from the given `identifier` and an associated name"""
-        if isinstance(identifier, str):
-            # expect the string to be a file path
-            series_path = self._path_resolver.resolve_series_file_path(identifier)
-            if series_path and os.path.exists(series_path):
-                return identifier, pd.read_csv(series_path, sep=";", header=None)
-            log_error_and_raise(ProtoWriterException(ProtoWriter._TIME_SERIES_FILE_NOT_FOUND.format(identifier)))
-        else:
-            name = "Constant value: {}".format(identifier)
-            return name, pd.DataFrame({"time": [START_IN_REAL_TIME], "value": [identifier]})
+            log_error_and_raise(ProtoWriterException(self._TYPE_NOT_IMPLEMENTED.format(attribute_type)))
 
     @staticmethod
-    def _add_rows_to_series(series, data_frame):
-        for key, value in data_frame.itertuples(index=False):
-            row = series.row.add()
-            row.timeStep = FameTime.convert_string_if_is_datetime(key)
-            row.value = value
-
-    def _write_protobuf_to_disk(self, pb_data_storage) -> None:
-        """Writes given `protobuf_input_data` to disk"""
-        try:
-            with open(self.file_path, "wb") as file:
-                file.write(pb_data_storage.SerializeToString())
-        except OSError as e:
-            log_error_and_raise(ProtoWriterException(ProtoWriter._NO_FILE_SPECIFIED.format(self.file_path), e))
-        log.info("Saved protobuf file `{}` to disk".format(self.file_path))
+    def _add_contracts(pb_input: InputData, contracts: List[Contract]) -> None:
+        """Triggers setting of `contracts` to `pb_input`"""
+        logger().info("Adding Contracts")
+        for contract in contracts:
+            pb_contract = ProtoWriter._set_contract(pb_input.contract.add(), contract)
+            ProtoWriter._set_contract_attributes(pb_contract, contract.attributes)
+            pb_contract.metadata = repr(contract.meta_data)
 
     @staticmethod
-    def _set_contract(pb_contract, contract: Contract):
+    def _set_contract(pb_contract: ProtoContract, contract: Contract) -> ProtoContract:
         """Saves given `contract` details to protobuf container `pb_contract`. Returns given `pb_contract`"""
         pb_contract.senderId = contract.sender_id
         pb_contract.receiverId = contract.receiver_id
         pb_contract.productName = contract.product_name
         pb_contract.firstDeliveryTime = contract.first_delivery_time
         pb_contract.deliveryIntervalInSteps = contract.delivery_interval
         if contract.expiration_time:
             pb_contract.expirationTime = contract.expiration_time
         return pb_contract
 
     @staticmethod
-    def _set_contract_attributes(pb_parent, attributes: Dict[str, Attribute]) -> None:
+    def _set_contract_attributes(
+        pb_parent: Union[ProtoContract, NestedField], attributes: Dict[str, Attribute]
+    ) -> None:
         """Assign (nested) Attributes to given protobuf container `pb_parent`"""
         for name, attribute in attributes.items():
-            log.debug("Assigning contract attribute `{}`.".format(name))
+            logger().debug("Assigning contract attribute `{}`.".format(name))
             pb_field = ProtoWriter._add_field(pb_parent, name)
 
             if attribute.has_value:
                 value = attribute.value
                 if isinstance(value, int):
                     pb_field.intValue.extend([value])
                 elif isinstance(value, float):
                     pb_field.doubleValue.extend([value])
                 elif isinstance(value, str):
                     pb_field.stringValue.extend([value])
                 else:
                     log_error_and_raise(ProtoWriterException(ProtoWriter._CONTRACT_UNSUPPORTED.format(str(attribute))))
             elif attribute.has_nested:
                 ProtoWriter._set_contract_attributes(pb_field, attribute.nested)
+
+    def _set_time_series(self, pb_input: InputData) -> None:
+        """Adds all time series from TimeSeriesManager to given `pb_input`"""
+        logger().info("Adding TimeSeries")
+        for unique_id, identifier, data in self._time_series_manager.get_all_series():
+            pb_series = pb_input.timeSeries.add()
+            pb_series.seriesId = unique_id
+            pb_series.seriesName = identifier
+            ProtoWriter._add_rows_to_series(pb_series, data)
+
+    @staticmethod
+    def _add_rows_to_series(series: InputData.TimeSeriesDao, data_frame) -> None:
+        for key, value in data_frame.itertuples(index=False):
+            row = series.row.add()
+            row.timeStep = int(key)
+            row.value = value
+
+    @staticmethod
+    def _set_schema(pb_input: InputData, schema: Schema) -> None:
+        """Sets the given `schema` `pb_input`"""
+        logger().info("Adding Schema")
+        pb_input.schema = schema.to_string()
+
+    def _write_protobuf_to_disk(self, pb_data_storage: DataStorage) -> None:
+        """Writes given `protobuf_input_data` to disk"""
+        logger().info(self._INFO_WRITING.format(self.file_path))
+        try:
+            with open(self.file_path, "wb") as file:
+                serialised_data_storage = pb_data_storage.SerializeToString()
+                file.write(self._FAME_PROTOBUF_STREAM_HEADER.encode(Reader.HEADER_ENCODING))
+                file.write(len(serialised_data_storage).to_bytes(Reader.BYTES_DEFINING_MESSAGE_LENGTH, byteorder="big"))
+                file.write(serialised_data_storage)
+        except OSError as e:
+            log_error_and_raise(ProtoWriterException(ProtoWriter._NO_FILE_SPECIFIED.format(self.file_path), e))
+        logger().info(self._INFO_WRITING_COMPLETED.format(self.file_path))
```

