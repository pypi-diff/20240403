# Comparing `tmp/galaxy-test-base-23.2.1.tar.gz` & `tmp/galaxy-test-base-24.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/test_base/dist/.tmp-2atcgdlm/galaxy-test-base-23.2.1.tar", last modified: Thu Feb 22 03:54:47 2024, max compression
+gzip compressed data, was "galaxy-test-base-24.0.0.tar", last modified: Wed Apr  3 02:45:41 2024, max compression
```

## Comparing `galaxy-test-base-23.2.1.tar` & `galaxy-test-base-24.0.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:54:47.000000 galaxy-test-base-23.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-02-22 03:50:43.000000 galaxy-test-base-23.2.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-02-22 03:50:43.000000 galaxy-test-base-23.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-02-22 03:50:43.000000 galaxy-test-base-23.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-02-22 03:54:47.000000 galaxy-test-base-23.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-02-22 03:50:43.000000 galaxy-test-base-23.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-22 03:50:43.000000 galaxy-test-base-23.2.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:54:47.000000 galaxy-test-base-23.2.1/galaxy_test/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-22 03:50:43.000000 galaxy-test-base-23.2.1/galaxy_test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:54:47.000000 galaxy-test-base-23.2.1/galaxy_test/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-test-base-23.2.1/galaxy_test/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8527 2024-02-22 03:50:43.000000 galaxy-test-base-23.2.1/galaxy_test/base/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-02-22 03:50:43.000000 galaxy-test-base-23.2.1/galaxy_test/base/api_asserts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-02-22 03:50:43.000000 galaxy-test-base-23.2.1/galaxy_test/base/api_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-02-22 03:50:43.000000 galaxy-test-base-23.2.1/galaxy_test/base/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:54:47.000000 galaxy-test-base-23.2.1/galaxy_test/base/data/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-02-22 03:50:43.000000 galaxy-test-base-23.2.1/galaxy_test/base/data/minimal_tool_no_id.json
--rw-r--r--   0 runner    (1001) docker     (127)    16151 2024-02-22 03:50:43.000000 galaxy-test-base-23.2.1/galaxy_test/base/data/test_subworkflow_with_integer_input.ga
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-02-22 03:50:43.000000 galaxy-test-base-23.2.1/galaxy_test/base/data/test_workflow_1.ga
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-02-22 03:50:43.000000 galaxy-test-base-23.2.1/galaxy_test/base/data/test_workflow_2.ga
--rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-02-22 03:50:43.000000 galaxy-test-base-23.2.1/galaxy_test/base/data/test_workflow_batch.ga
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-02-22 03:50:43.000000 galaxy-test-base-23.2.1/galaxy_test/base/data/test_workflow_map_reduce_pause.ga
--rw-r--r--   0 runner    (1001) docker     (127)     3740 2024-02-22 03:50:43.000000 galaxy-test-base-23.2.1/galaxy_test/base/data/test_workflow_matching_lists.ga
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-02-22 03:50:43.000000 galaxy-test-base-23.2.1/galaxy_test/base/data/test_workflow_missing_tool.ga
--rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-02-22 03:50:43.000000 galaxy-test-base-23.2.1/galaxy_test/base/data/test_workflow_pause.ga
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-02-22 03:50:43.000000 galaxy-test-base-23.2.1/galaxy_test/base/data/test_workflow_randomlines_legacy_params.ga
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-02-22 03:50:43.000000 galaxy-test-base-23.2.1/galaxy_test/base/data/test_workflow_randomlines_legacy_params_mixed_types.ga
--rw-r--r--   0 runner    (1001) docker     (127)    13049 2024-02-22 03:50:43.000000 galaxy-test-base-23.2.1/galaxy_test/base/data/test_workflow_topoambigouity.ga
--rw-r--r--   0 runner    (1001) docker     (127)    13050 2024-02-22 03:50:43.000000 galaxy-test-base-23.2.1/galaxy_test/base/data/test_workflow_topoambigouity_auto_laidout.ga
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-02-22 03:50:43.000000 galaxy-test-base-23.2.1/galaxy_test/base/data/test_workflow_two_random_lines.ga
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-02-22 03:50:43.000000 galaxy-test-base-23.2.1/galaxy_test/base/data/test_workflow_validation_1.ga
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-02-22 03:50:43.000000 galaxy-test-base-23.2.1/galaxy_test/base/data/test_workflow_with_input_tags.ga
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-02-22 03:50:43.000000 galaxy-test-base-23.2.1/galaxy_test/base/data/test_workflow_with_runtime_input.ga
--rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-02-22 03:50:43.000000 galaxy-test-base-23.2.1/galaxy_test/base/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-02-22 03:50:43.000000 galaxy-test-base-23.2.1/galaxy_test/base/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-02-22 03:50:43.000000 galaxy-test-base-23.2.1/galaxy_test/base/interactor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-02-22 03:50:43.000000 galaxy-test-base-23.2.1/galaxy_test/base/json_schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)   134427 2024-02-22 03:50:43.000000 galaxy-test-base-23.2.1/galaxy_test/base/populators.py
--rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-02-22 03:50:43.000000 galaxy-test-base-23.2.1/galaxy_test/base/rules_test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-02-22 03:50:43.000000 galaxy-test-base-23.2.1/galaxy_test/base/testcase.py
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-02-22 03:50:43.000000 galaxy-test-base-23.2.1/galaxy_test/base/uses_shed_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    24278 2024-02-22 03:50:43.000000 galaxy-test-base-23.2.1/galaxy_test/base/workflow_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-test-base-23.2.1/galaxy_test/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:54:47.000000 galaxy-test-base-23.2.1/galaxy_test_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-02-22 03:54:47.000000 galaxy-test-base-23.2.1/galaxy_test_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-02-22 03:54:47.000000 galaxy-test-base-23.2.1/galaxy_test_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 03:54:47.000000 galaxy-test-base-23.2.1/galaxy_test_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-22 03:54:47.000000 galaxy-test-base-23.2.1/galaxy_test_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-22 03:54:47.000000 galaxy-test-base-23.2.1/galaxy_test_base.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-22 03:50:43.000000 galaxy-test-base-23.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-02-22 03:54:47.000000 galaxy-test-base-23.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-22 03:50:43.000000 galaxy-test-base-23.2.1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:41.007406 galaxy-test-base-24.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7739 2024-04-03 02:45:41.007406 galaxy-test-base-24.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:40.999406 galaxy-test-base-24.0.0/galaxy_test/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:41.003406 galaxy-test-base-24.0.0/galaxy_test/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8582 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/api_asserts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/api_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:41.007406 galaxy-test-base-24.0.0/galaxy_test/base/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/data/minimal_tool_no_id.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16151 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/data/test_subworkflow_with_integer_input.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_1.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_2.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_batch.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_map_reduce_pause.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     3740 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_matching_lists.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_missing_tool.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_pause.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_randomlines_legacy_params.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_randomlines_legacy_params_mixed_types.ga
+-rw-r--r--   0 runner    (1001) docker     (127)    13049 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_topoambigouity.ga
+-rw-r--r--   0 runner    (1001) docker     (127)    13050 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_topoambigouity_auto_laidout.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_two_random_lines.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_validation_1.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_with_input_tags.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_with_runtime_input.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/interactor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/json_schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)   135178 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/populators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/rules_test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/testcase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/uses_shed_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24278 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/workflow_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:41.007406 galaxy-test-base-24.0.0/galaxy_test_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7739 2024-04-03 02:45:40.000000 galaxy-test-base-24.0.0/galaxy_test_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-03 02:45:40.000000 galaxy-test-base-24.0.0/galaxy_test_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:45:40.000000 galaxy-test-base-24.0.0/galaxy_test_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-03 02:45:40.000000 galaxy-test-base-24.0.0/galaxy_test_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-03 02:45:40.000000 galaxy-test-base-24.0.0/galaxy_test_base.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-03 02:45:41.007406 galaxy-test-base-24.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/test-requirements.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `galaxy-test-base-23.2.1/HISTORY.rst` & `galaxy-test-base-24.0.0/HISTORY.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,32 @@
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.0 (2024-04-02)
+-------------------
+
+
+============
+Enhancements
+============
+
+* port invocation API to fastapi by `@martenson <https://github.com/martenson>`_ in `#16707 <https://github.com/galaxyproject/galaxy/pull/16707>`_
+* Python 3.8 as minimum by `@mr-c <https://github.com/mr-c>`_ in `#16954 <https://github.com/galaxyproject/galaxy/pull/16954>`_
+* Support for OIDC API Auth and OIDC integration tests by `@nuwang <https://github.com/nuwang>`_ in `#16977 <https://github.com/galaxyproject/galaxy/pull/16977>`_
+* Reuse test instance during non-integration tests by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17234 <https://github.com/galaxyproject/galaxy/pull/17234>`_
+* API endpoint that allows "changing" the objectstore for "safe" scenarios.  by `@jmchilton <https://github.com/jmchilton>`_ in `#17329 <https://github.com/galaxyproject/galaxy/pull/17329>`_
+* Update to black 2024 stable style by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17391 <https://github.com/galaxyproject/galaxy/pull/17391>`_
+* Allow filtering history datasets by object store ID and quota source. by `@jmchilton <https://github.com/jmchilton>`_ in `#17460 <https://github.com/galaxyproject/galaxy/pull/17460>`_
+* Refactor Workflow API routes - Part 1 by `@heisner-tillman <https://github.com/heisner-tillman>`_ in `#17463 <https://github.com/galaxyproject/galaxy/pull/17463>`_
+* Filter out subworkflow invocations by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17558 <https://github.com/galaxyproject/galaxy/pull/17558>`_
+
+-------------------
 23.2.1 (2024-02-21)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy-test-base-23.2.1/LICENSE` & `galaxy-test-base-24.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.2.1/PKG-INFO` & `galaxy-test-base-24.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 Metadata-Version: 2.1
 Name: galaxy-test-base
-Version: 23.2.1
+Version: 24.0.0
 Summary: Galaxy testing utilities
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Academic Free License (AFL)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: galaxy-tool-util
+Requires-Dist: galaxy-util
+Requires-Dist: bioblend
+Requires-Dist: cwltest
+Requires-Dist: gxformat2
+Requires-Dist: pytest
+Requires-Dist: PyYAML
+Requires-Dist: requests
 
 
 .. image:: https://badge.fury.io/py/galaxy-test-base.svg
    :target: https://pypi.org/project/galaxy-test-base/
 
 
 
@@ -43,14 +51,33 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.0 (2024-04-02)
+-------------------
+
+
+============
+Enhancements
+============
+
+* port invocation API to fastapi by `@martenson <https://github.com/martenson>`_ in `#16707 <https://github.com/galaxyproject/galaxy/pull/16707>`_
+* Python 3.8 as minimum by `@mr-c <https://github.com/mr-c>`_ in `#16954 <https://github.com/galaxyproject/galaxy/pull/16954>`_
+* Support for OIDC API Auth and OIDC integration tests by `@nuwang <https://github.com/nuwang>`_ in `#16977 <https://github.com/galaxyproject/galaxy/pull/16977>`_
+* Reuse test instance during non-integration tests by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17234 <https://github.com/galaxyproject/galaxy/pull/17234>`_
+* API endpoint that allows "changing" the objectstore for "safe" scenarios.  by `@jmchilton <https://github.com/jmchilton>`_ in `#17329 <https://github.com/galaxyproject/galaxy/pull/17329>`_
+* Update to black 2024 stable style by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17391 <https://github.com/galaxyproject/galaxy/pull/17391>`_
+* Allow filtering history datasets by object store ID and quota source. by `@jmchilton <https://github.com/jmchilton>`_ in `#17460 <https://github.com/galaxyproject/galaxy/pull/17460>`_
+* Refactor Workflow API routes - Part 1 by `@heisner-tillman <https://github.com/heisner-tillman>`_ in `#17463 <https://github.com/galaxyproject/galaxy/pull/17463>`_
+* Filter out subworkflow invocations by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17558 <https://github.com/galaxyproject/galaxy/pull/17558>`_
+
+-------------------
 23.2.1 (2024-02-21)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy-test-base-23.2.1/galaxy_test/base/api.py` & `galaxy-test-base-24.0.0/galaxy_test/base/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,27 +94,28 @@
 class UsesApiTestCaseMixin:
     url: str
     _galaxy_interactor: Optional["ApiTestInteractor"] = None
 
     def tearDown(self):
         if os.environ.get("GALAXY_TEST_EXTERNAL") is None:
             # Only kill running jobs after test for managed test instances
-            for job in self.galaxy_interactor.get("jobs?state=running").json():
-                self._delete(f"jobs/{job['id']}")
+            response = self.galaxy_interactor.get("jobs?state=running")
+            if response.ok:
+                for job in response.json():
+                    self._delete(f"jobs/{job['id']}")
 
     def _api_url(self, path, params=None, use_key=None, use_admin_key=None):
         if not params:
             params = {}
         url = urljoin(self.url, f"api/{path}")
         if use_key:
             params["key"] = self.galaxy_interactor.api_key
         if use_admin_key:
             params["key"] = self.galaxy_interactor.master_api_key
-        query = urlencode(params)
-        if query:
+        if query := urlencode(params):
             url = f"{url}?{query}"
         return url
 
     def _setup_interactor(self):
         self.user_api_key = get_user_api_key()
         self.master_api_key = get_admin_api_key()
         self._galaxy_interactor = self._get_interactor()
```

### Comparing `galaxy-test-base-23.2.1/galaxy_test/base/api_asserts.py` & `galaxy-test-base-24.0.0/galaxy_test/base/api_asserts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Utility methods for making assertions about Galaxy API responses, etc...
 """
+
 from typing import (
     Any,
     cast,
     Dict,
     Optional,
     Union,
 )
```

### Comparing `galaxy-test-base-23.2.1/galaxy_test/base/api_util.py` & `galaxy-test-base-24.0.0/galaxy_test/base/api_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.2.1/galaxy_test/base/data/test_subworkflow_with_integer_input.ga` & `galaxy-test-base-24.0.0/galaxy_test/base/data/test_subworkflow_with_integer_input.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.2.1/galaxy_test/base/data/test_workflow_1.ga` & `galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_1.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.2.1/galaxy_test/base/data/test_workflow_2.ga` & `galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_2.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.2.1/galaxy_test/base/data/test_workflow_batch.ga` & `galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_batch.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.2.1/galaxy_test/base/data/test_workflow_map_reduce_pause.ga` & `galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_map_reduce_pause.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.2.1/galaxy_test/base/data/test_workflow_matching_lists.ga` & `galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_matching_lists.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.2.1/galaxy_test/base/data/test_workflow_missing_tool.ga` & `galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_missing_tool.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.2.1/galaxy_test/base/data/test_workflow_pause.ga` & `galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_pause.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.2.1/galaxy_test/base/data/test_workflow_randomlines_legacy_params.ga` & `galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_randomlines_legacy_params.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.2.1/galaxy_test/base/data/test_workflow_randomlines_legacy_params_mixed_types.ga` & `galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_randomlines_legacy_params_mixed_types.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.2.1/galaxy_test/base/data/test_workflow_topoambigouity.ga` & `galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_topoambigouity.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.2.1/galaxy_test/base/data/test_workflow_topoambigouity_auto_laidout.ga` & `galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_topoambigouity_auto_laidout.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.2.1/galaxy_test/base/data/test_workflow_two_random_lines.ga` & `galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_two_random_lines.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.2.1/galaxy_test/base/data/test_workflow_validation_1.ga` & `galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_validation_1.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.2.1/galaxy_test/base/data/test_workflow_with_input_tags.ga` & `galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_with_input_tags.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.2.1/galaxy_test/base/data/test_workflow_with_runtime_input.ga` & `galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_with_runtime_input.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.2.1/galaxy_test/base/decorators.py` & `galaxy-test-base-24.0.0/galaxy_test/base/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 are appropriate for the API and Selenium tests that are meant to be executable on
 external Galaxies.
 
 Running this class of tests should implicitly come with the expectation that new
 jobs, workflows, and datasets will be created. But tests creating new published objects,
 histories, libraries, etc... should be annotated ideally.
 """
+
 import os
 import unittest
 from functools import wraps
 from typing import Union
 
 import pytest
 from typing_extensions import Literal
@@ -39,16 +40,15 @@
 def using_requirement(tag: KnownRequirementT):
     """At runtime, indicate we're using a Galaxy feature.
 
     This allows runtime test skips if the appropriate environment variable is set.
     """
     requirement = f"requires_{tag}"
     skip_environment_variable = f"GALAXY_TEST_SKIP_IF_{requirement.upper()}"
-    env_value = os.environ.get(skip_environment_variable, "0")
-    if env_value != "0":
+    if (env_value := os.environ.get(skip_environment_variable, "0")) != "0":
         raise unittest.SkipTest(f"[{env_value}] Skipping due to {skip_environment_variable} being set to {env_value}")
 
 
 def _attach_requirements(method, tag: KnownRequirementT):
     requirement = f"requires_{tag}"
     if not hasattr(method, "__required_galaxy_features"):
         method.__required_galaxy_features = []
```

### Comparing `galaxy-test-base-23.2.1/galaxy_test/base/env.py` & `galaxy-test-base-24.0.0/galaxy_test/base/env.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Base utilities for working Galaxy test environments.
 """
+
 import fcntl
 import os
 import socket
 import struct
 from typing import (
     Optional,
     Tuple,
```

### Comparing `galaxy-test-base-23.2.1/galaxy_test/base/interactor.py` & `galaxy-test-base-24.0.0/galaxy_test/base/interactor.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.2.1/galaxy_test/base/json_schema_utils.py` & `galaxy-test-base-24.0.0/galaxy_test/base/json_schema_utils.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.2.1/galaxy_test/base/populators.py` & `galaxy-test-base-24.0.0/galaxy_test/base/populators.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 is a bit ugly and this ugliness again stems from these organically growing from a
 framework that originally didn't use requests at all.
 
 API tests and Selenium tests routinely use requests directly and that is totally fine,
 requests should just be filtered through the verb abstractions if that functionality
 is then added to populators to be shared across tests or across testing frameworks.
 """
+
 import base64
 import contextlib
 import json
 import os
 import tarfile
 import tempfile
 import time
@@ -1083,16 +1084,16 @@
                 if kwds.get("history_content_type"):
                     history_contents = [
                         c for c in history_contents if c["history_content_type"] == kwds["history_content_type"]
                     ]
                 history_content_id = history_contents[-1]["id"]
         return history_content_id
 
-    def get_history_contents(self, history_id: str) -> List[Dict[str, Any]]:
-        contents_response = self._get_contents_request(history_id)
+    def get_history_contents(self, history_id: str, data=None) -> List[Dict[str, Any]]:
+        contents_response = self._get_contents_request(history_id, data=data)
         contents_response.raise_for_status()
         return contents_response.json()
 
     def _get_contents_request(self, history_id: str, suffix: str = "", data=None) -> Response:
         if data is None:
             data = {}
         url = f"histories/{history_id}/contents"
@@ -1177,14 +1178,21 @@
     def total_disk_usage(self) -> float:
         response = self._get("users/current")
         response.raise_for_status()
         user_object = response.json()
         assert "total_disk_usage" in user_object
         return user_object["total_disk_usage"]
 
+    def update_object_store_id(self, dataset_id: str, object_store_id: str):
+        payload = {"object_store_id": object_store_id}
+        url = f"datasets/{dataset_id}/object_store_id"
+        update_response = self._put(url, payload, json=True)
+        update_response.raise_for_status()
+        return update_response
+
     def create_role(self, user_ids: list, description: Optional[str] = None) -> dict:
         using_requirement("admin")
         payload = {
             "name": self.get_random_name(prefix="testpop"),
             "description": description or "Test Role",
             "user_ids": user_ids,
         }
@@ -1304,16 +1312,15 @@
     def get_export_url(self, export_url) -> Response:
         download_response = self._get(export_url)
         api_asserts.assert_status_code_is(download_response, 200)
         return download_response
 
     def import_history(self, import_data):
         files = {}
-        archive_file = import_data.pop("archive_file", None)
-        if archive_file:
+        if archive_file := import_data.pop("archive_file", None):
             files["archive_file"] = archive_file
         import_response = self._post("histories", data=import_data, files=files)
         api_asserts.assert_status_code_is(import_response, 200)
         return import_response.json()["id"]
 
     def wait_for_history_with_name(self, history_name: str, desc: str) -> Dict[str, Any]:
         def has_history_with_name():
@@ -1690,26 +1697,28 @@
         url = f"invocations/{invocation_id}"
 
         def workflow_state():
             return self._get(url)
 
         return wait_on_state(workflow_state, desc="workflow invocation state", timeout=timeout, assert_ok=assert_ok)
 
-    def workflow_invocations(self, workflow_id: str) -> List[Dict[str, Any]]:
+    def workflow_invocations(self, workflow_id: str, include_nested_invocations=True) -> List[Dict[str, Any]]:
         response = self._get(f"workflows/{workflow_id}/invocations")
         api_asserts.assert_status_code_is(response, 200)
         return response.json()
 
     def cancel_invocation(self, invocation_id: str):
         response = self._delete(f"invocations/{invocation_id}")
         api_asserts.assert_status_code_is(response, 200)
         return response.json()
 
-    def history_invocations(self, history_id: str) -> List[Dict[str, Any]]:
-        history_invocations_response = self._get("invocations", {"history_id": history_id})
+    def history_invocations(self, history_id: str, include_nested_invocations: bool = True) -> List[Dict[str, Any]]:
+        history_invocations_response = self._get(
+            "invocations", {"history_id": history_id, "include_nested_invocations": include_nested_invocations}
+        )
         api_asserts.assert_status_code_is(history_invocations_response, 200)
         return history_invocations_response.json()
 
     def wait_for_history_workflows(
         self,
         history_id: str,
         assert_ok: bool = True,
@@ -1810,15 +1819,15 @@
         metadata_json_path = crate_directory / "ro-crate-metadata.json"
         with metadata_json_path.open() as f:
             metadata_json = json.load(f)
             assert metadata_json["@context"] == "https://w3id.org/ro/crate/1.1/context"
 
     def invoke_workflow_raw(self, workflow_id: str, request: dict, assert_ok: bool = False) -> Response:
         url = f"workflows/{workflow_id}/invocations"
-        invocation_response = self._post(url, data=request)
+        invocation_response = self._post(url, data=request, json=True)
         if assert_ok:
             invocation_response.raise_for_status()
         return invocation_response
 
     def invoke_workflow(
         self,
         workflow_id: str,
@@ -1880,14 +1889,19 @@
         return invoke_return
 
     def workflow_report_json(self, workflow_id: str, invocation_id: str) -> dict:
         response = self._get(f"workflows/{workflow_id}/invocations/{invocation_id}/report")
         api_asserts.assert_status_code_is(response, 200)
         return response.json()
 
+    def workflow_report_pdf(self, workflow_id: str, invocation_id: str) -> Response:
+        response = self._get(f"workflows/{workflow_id}/invocations/{invocation_id}/report.pdf")
+        api_asserts.assert_status_code_is(response, 200)
+        return response
+
     def download_workflow(
         self, workflow_id: str, style: Optional[str] = None, history_id: Optional[str] = None
     ) -> dict:
         params = {}
         if style is not None:
             params["style"] = style
         if history_id is not None:
@@ -3202,42 +3216,39 @@
         if route.startswith("/api/"):
             route = route[len("/api/") :]
 
         return f"{self._api_url()}/{route}"
 
 
 class GiDatasetPopulator(GiHttpMixin, BaseDatasetPopulator):
-
     """Implementation of BaseDatasetPopulator backed by bioblend."""
 
     def __init__(self, gi):
         """Construct a dataset populator from a bioblend GalaxyInstance."""
         self._gi = gi
 
     def _summarize_history(self, history_id: str) -> None:
         pass
 
 
 class GiDatasetCollectionPopulator(GiHttpMixin, BaseDatasetCollectionPopulator):
-
     """Implementation of BaseDatasetCollectionPopulator backed by bioblend."""
 
     def __init__(self, gi):
         """Construct a dataset collection populator from a bioblend GalaxyInstance."""
         self._gi = gi
         self.dataset_populator = GiDatasetPopulator(gi)
         self.dataset_collection_populator = GiDatasetCollectionPopulator(gi)
 
     def _create_collection(self, payload):
         create_response = self._post("dataset_collections", data=payload, json=True)
         return create_response
 
 
 class GiWorkflowPopulator(GiHttpMixin, BaseWorkflowPopulator):
-
     """Implementation of BaseWorkflowPopulator backed by bioblend."""
 
     def __init__(self, gi):
         """Construct a workflow populator from a bioblend GalaxyInstance."""
         self._gi = gi
         self.dataset_populator = GiDatasetPopulator(gi)
```

### Comparing `galaxy-test-base-23.2.1/galaxy_test/base/rules_test_data.py` & `galaxy-test-base-24.0.0/galaxy_test/base/rules_test_data.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.2.1/galaxy_test/base/testcase.py` & `galaxy-test-base-24.0.0/galaxy_test/base/testcase.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import logging
-import os
 from typing import (
     Any,
     Optional,
 )
 
+import pytest
+
 from galaxy.tool_util.verify.test_data import TestDataResolver
 from galaxy.util.unittest import TestCase
 from galaxy_test.base.env import (
     setup_keep_outdir,
     target_url_parts,
 )
 
 log = logging.getLogger(__name__)
 
 
+@pytest.mark.usefixtures("embedded_driver")
 class FunctionalTestCase(TestCase):
     """Base class for tests targetting actual Galaxy servers.
 
     Subclass should override galaxy_driver_class if a Galaxy server
     needs to be launched to run the test, this base class assumes a
     server is already running.
     """
@@ -42,22 +44,17 @@
             self.url = f"http://{self.host}:{self.port}{server_wrapper.prefix.rstrip('/')}/"
         self.test_data_resolver = TestDataResolver()
         self.keepOutdir = setup_keep_outdir()
 
     @classmethod
     def setUpClass(cls):
         """Configure and start Galaxy for a test."""
-        cls._test_driver = None
-
-        if cls.galaxy_driver_class is not None and not os.environ.get("GALAXY_TEST_ENVIRONMENT_CONFIGURED"):
-            cls._test_driver = cls.galaxy_driver_class()
-            cls._test_driver.setup(config_object=cls)
+        pass
 
     @classmethod
     def tearDownClass(cls):
         """Shutdown Galaxy server and cleanup temp directory."""
-        if cls._test_driver:
-            cls._test_driver.tear_down()
+        pass
 
     def get_filename(self, filename: str) -> str:
         # No longer used by tool tests - drop if isn't used else where.
         return self.test_data_resolver.get_filename(filename)
```

### Comparing `galaxy-test-base-23.2.1/galaxy_test/base/uses_shed_api.py` & `galaxy-test-base-24.0.0/galaxy_test/base/uses_shed_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,15 @@
 
 OperationT = Callable[[Dict[str, Any]], Response]
 
 
 class UsesShedApi:
     @property
     @abc.abstractmethod
-    def galaxy_interactor(self) -> GalaxyInteractorApi:
-        ...
+    def galaxy_interactor(self) -> GalaxyInteractorApi: ...
 
     def delete_repo_request(self, payload: Dict[str, Any]) -> Response:
         return self.galaxy_interactor._delete("tool_shed_repositories", data=payload, admin=True)
 
     def install_repo_request(self, payload: Dict[str, Any]) -> Response:
         return self.galaxy_interactor._post(
             "tool_shed_repositories/new/install_repository_revision", data=payload, admin=True
```

### Comparing `galaxy-test-base-23.2.1/galaxy_test/base/workflow_fixtures.py` & `galaxy-test-base-24.0.0/galaxy_test/base/workflow_fixtures.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.2.1/galaxy_test_base.egg-info/PKG-INFO` & `galaxy-test-base-24.0.0/galaxy_test_base.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 Metadata-Version: 2.1
 Name: galaxy-test-base
-Version: 23.2.1
+Version: 24.0.0
 Summary: Galaxy testing utilities
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Academic Free License (AFL)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: galaxy-tool-util
+Requires-Dist: galaxy-util
+Requires-Dist: bioblend
+Requires-Dist: cwltest
+Requires-Dist: gxformat2
+Requires-Dist: pytest
+Requires-Dist: PyYAML
+Requires-Dist: requests
 
 
 .. image:: https://badge.fury.io/py/galaxy-test-base.svg
    :target: https://pypi.org/project/galaxy-test-base/
 
 
 
@@ -43,14 +51,33 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.0 (2024-04-02)
+-------------------
+
+
+============
+Enhancements
+============
+
+* port invocation API to fastapi by `@martenson <https://github.com/martenson>`_ in `#16707 <https://github.com/galaxyproject/galaxy/pull/16707>`_
+* Python 3.8 as minimum by `@mr-c <https://github.com/mr-c>`_ in `#16954 <https://github.com/galaxyproject/galaxy/pull/16954>`_
+* Support for OIDC API Auth and OIDC integration tests by `@nuwang <https://github.com/nuwang>`_ in `#16977 <https://github.com/galaxyproject/galaxy/pull/16977>`_
+* Reuse test instance during non-integration tests by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17234 <https://github.com/galaxyproject/galaxy/pull/17234>`_
+* API endpoint that allows "changing" the objectstore for "safe" scenarios.  by `@jmchilton <https://github.com/jmchilton>`_ in `#17329 <https://github.com/galaxyproject/galaxy/pull/17329>`_
+* Update to black 2024 stable style by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17391 <https://github.com/galaxyproject/galaxy/pull/17391>`_
+* Allow filtering history datasets by object store ID and quota source. by `@jmchilton <https://github.com/jmchilton>`_ in `#17460 <https://github.com/galaxyproject/galaxy/pull/17460>`_
+* Refactor Workflow API routes - Part 1 by `@heisner-tillman <https://github.com/heisner-tillman>`_ in `#17463 <https://github.com/galaxyproject/galaxy/pull/17463>`_
+* Filter out subworkflow invocations by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17558 <https://github.com/galaxyproject/galaxy/pull/17558>`_
+
+-------------------
 23.2.1 (2024-02-21)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy-test-base-23.2.1/galaxy_test_base.egg-info/SOURCES.txt` & `galaxy-test-base-24.0.0/galaxy_test_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.2.1/setup.cfg` & `galaxy-test-base-24.0.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -5,47 +5,47 @@
 	Development Status :: 5 - Production/Stable
 	Environment :: Console
 	Intended Audience :: Developers
 	License :: OSI Approved :: Academic Free License (AFL)
 	Natural Language :: English
 	Operating System :: POSIX
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Topic :: Software Development
 	Topic :: Software Development :: Code Generators
 	Topic :: Software Development :: Testing
 description = Galaxy testing utilities
 keywords = 
 	Galaxy
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-test-base
 url = https://github.com/galaxyproject/galaxy
-version = 23.2.1
+version = 24.0.0
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-tool-util
 	galaxy-util
 	bioblend
 	cwltest
 	gxformat2
 	pytest
 	PyYAML
 	requests
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.8
 
 [options.packages.find]
 exclude = 
 	tests*
 
 [egg_info]
 tag_build =
```

