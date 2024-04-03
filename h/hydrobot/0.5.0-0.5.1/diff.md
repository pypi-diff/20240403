# Comparing `tmp/hydrobot-0.5.0.tar.gz` & `tmp/hydrobot-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydrobot-0.5.0.tar", last modified: Tue Apr  2 20:04:32 2024, max compression
+gzip compressed data, was "hydrobot-0.5.1.tar", last modified: Wed Apr  3 20:11:46 2024, max compression
```

## Comparing `hydrobot-0.5.0.tar` & `hydrobot-0.5.1.tar`

### file list

```diff
@@ -1,93 +1,90 @@
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-02 20:04:32.582867 hydrobot-0.5.0/
--rw-r--r--   0 nic       (1000) nic       (1000)      292 2023-09-27 02:03:08.000000 hydrobot-0.5.0/.editorconfig
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-02 20:04:32.562867 hydrobot-0.5.0/.github/
--rw-r--r--   0 nic       (1000) nic       (1000)      333 2023-09-27 02:03:08.000000 hydrobot-0.5.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 nic       (1000) nic       (1000)     1207 2023-10-16 02:52:42.000000 hydrobot-0.5.0/.gitignore
--rw-r--r--   0 nic       (1000) nic       (1000)      514 2024-03-11 01:19:58.000000 hydrobot-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0 nic       (1000) nic       (1000)     1068 2024-03-11 01:19:58.000000 hydrobot-0.5.0/.readthedocs.yaml
--rw-r--r--   0 nic       (1000) nic       (1000)      212 2023-10-16 02:52:42.000000 hydrobot-0.5.0/AUTHORS.rst
--rw-r--r--   0 nic       (1000) nic       (1000)     7004 2024-03-11 01:19:58.000000 hydrobot-0.5.0/CONTRIBUTING.rst
--rw-r--r--   0 nic       (1000) nic       (1000)     1368 2024-04-02 19:57:10.000000 hydrobot-0.5.0/HISTORY.rst
--rw-r--r--   0 nic       (1000) nic       (1000)     1610 2023-10-16 02:47:23.000000 hydrobot-0.5.0/LICENSE
--rw-r--r--   0 nic       (1000) nic       (1000)      298 2024-03-11 01:19:58.000000 hydrobot-0.5.0/MANIFEST.in
--rw-r--r--   0 nic       (1000) nic       (1000)     2336 2024-03-11 01:19:58.000000 hydrobot-0.5.0/Makefile
--rw-r--r--   0 nic       (1000) nic       (1000)     6556 2024-04-02 20:04:32.582867 hydrobot-0.5.0/PKG-INFO
--rw-r--r--   0 nic       (1000) nic       (1000)     4823 2024-04-02 19:49:26.000000 hydrobot-0.5.0/README.rst
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-02 20:04:32.562867 hydrobot-0.5.0/docs/
--rw-r--r--   0 nic       (1000) nic       (1000)      609 2023-11-02 03:51:37.000000 hydrobot-0.5.0/docs/Makefile
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-02 20:04:32.552868 hydrobot-0.5.0/docs/_build/
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-02 20:04:32.552868 hydrobot-0.5.0/docs/_build/html/
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-02 20:04:32.562867 hydrobot-0.5.0/docs/_build/html/_static/
--rw-r--r--   0 nic       (1000) nic       (1000)      286 2023-12-12 21:10:33.000000 hydrobot-0.5.0/docs/_build/html/_static/file.png
--rw-r--r--   0 nic       (1000) nic       (1000)       90 2023-12-12 21:10:33.000000 hydrobot-0.5.0/docs/_build/html/_static/minus.png
--rw-r--r--   0 nic       (1000) nic       (1000)       90 2023-12-12 21:10:33.000000 hydrobot-0.5.0/docs/_build/html/_static/plus.png
--rw-r--r--   0 nic       (1000) nic       (1000)       28 2023-09-27 02:03:08.000000 hydrobot-0.5.0/docs/authors.rst
--rwxr-xr-x   0 nic       (1000) nic       (1000)     5087 2024-03-11 01:19:58.000000 hydrobot-0.5.0/docs/conf.py
--rw-r--r--   0 nic       (1000) nic       (1000)       33 2023-09-27 02:03:08.000000 hydrobot-0.5.0/docs/contributing.rst
--rw-r--r--   0 nic       (1000) nic       (1000)       28 2023-09-27 02:03:08.000000 hydrobot-0.5.0/docs/history.rst
--rw-r--r--   0 nic       (1000) nic       (1000)     1190 2024-03-11 01:19:58.000000 hydrobot-0.5.0/docs/hydrobot.rst
--rw-r--r--   0 nic       (1000) nic       (1000)      305 2023-11-02 03:51:37.000000 hydrobot-0.5.0/docs/index.rst
--rw-r--r--   0 nic       (1000) nic       (1000)     1555 2024-03-11 01:19:58.000000 hydrobot-0.5.0/docs/installation.rst
--rw-r--r--   0 nic       (1000) nic       (1000)      806 2023-11-02 03:51:37.000000 hydrobot-0.5.0/docs/make.bat
--rw-r--r--   0 nic       (1000) nic       (1000)       61 2023-12-12 21:10:41.000000 hydrobot-0.5.0/docs/modules.rst
--rw-r--r--   0 nic       (1000) nic       (1000)       27 2023-09-27 02:03:08.000000 hydrobot-0.5.0/docs/readme.rst
--rw-r--r--   0 nic       (1000) nic       (1000)       71 2023-11-02 03:51:37.000000 hydrobot-0.5.0/docs/usage.rst
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-02 20:04:32.572867 hydrobot-0.5.0/hydrobot/
--rw-r--r--   0 nic       (1000) nic       (1000)      153 2024-04-02 20:01:08.000000 hydrobot-0.5.0/hydrobot/__init__.py
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-02 20:04:32.572867 hydrobot-0.5.0/hydrobot/config/
--rw-r--r--   0 nic       (1000) nic       (1000)      105 2024-03-11 01:19:58.000000 hydrobot-0.5.0/hydrobot/config/QualityCodeEvaluator_QC_config.csv
--rw-r--r--   0 nic       (1000) nic       (1000)       55 2024-03-11 01:19:58.000000 hydrobot-0.5.0/hydrobot/config/TwoLevelQualityCodeEvaluator_QC_config.csv
--rw-r--r--   0 nic       (1000) nic       (1000)     5728 2024-04-01 22:51:29.000000 hydrobot-0.5.0/hydrobot/data_acquisition.py
--rw-r--r--   0 nic       (1000) nic       (1000)     8005 2024-04-02 01:09:54.000000 hydrobot-0.5.0/hydrobot/data_sources.py
--rw-r--r--   0 nic       (1000) nic       (1000)    32675 2024-04-02 00:34:08.000000 hydrobot-0.5.0/hydrobot/data_structure.py
--rw-r--r--   0 nic       (1000) nic       (1000)    13768 2024-04-01 22:51:29.000000 hydrobot-0.5.0/hydrobot/evaluator.py
--rw-r--r--   0 nic       (1000) nic       (1000)     7516 2024-03-11 01:19:58.000000 hydrobot-0.5.0/hydrobot/filters.py
--rw-r--r--   0 nic       (1000) nic       (1000)    20727 2024-04-01 22:51:29.000000 hydrobot-0.5.0/hydrobot/plotter.py
--rw-r--r--   0 nic       (1000) nic       (1000)    52042 2024-04-02 20:02:29.000000 hydrobot-0.5.0/hydrobot/processor.py
--rw-r--r--   0 nic       (1000) nic       (1000)     7778 2024-04-01 22:51:29.000000 hydrobot-0.5.0/hydrobot/utils.py
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-02 20:04:32.572867 hydrobot-0.5.0/hydrobot.egg-info/
--rw-r--r--   0 nic       (1000) nic       (1000)     6556 2024-04-02 20:04:32.000000 hydrobot-0.5.0/hydrobot.egg-info/PKG-INFO
--rw-r--r--   0 nic       (1000) nic       (1000)     1981 2024-04-02 20:04:32.000000 hydrobot-0.5.0/hydrobot.egg-info/SOURCES.txt
--rw-r--r--   0 nic       (1000) nic       (1000)        1 2024-04-02 20:04:32.000000 hydrobot-0.5.0/hydrobot.egg-info/dependency_links.txt
--rw-r--r--   0 nic       (1000) nic       (1000)      311 2024-04-02 20:04:32.000000 hydrobot-0.5.0/hydrobot.egg-info/requires.txt
--rw-r--r--   0 nic       (1000) nic       (1000)        9 2024-04-02 20:04:32.000000 hydrobot-0.5.0/hydrobot.egg-info/top_level.txt
--rw-r--r--   0 nic       (1000) nic       (1000)      422 2024-03-11 01:19:58.000000 hydrobot-0.5.0/old_setup.cfg
--rw-r--r--   0 nic       (1000) nic       (1000)     1571 2024-03-11 01:19:58.000000 hydrobot-0.5.0/old_setup.py
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-02 20:04:32.572867 hydrobot-0.5.0/prototypes/
--rw-r--r--   0 nic       (1000) nic       (1000)     4257 2024-04-02 20:02:29.000000 hydrobot-0.5.0/prototypes/Class_script.py
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-02 20:04:32.572867 hydrobot-0.5.0/prototypes/output_dump/
--rw-r--r--   0 nic       (1000) nic       (1000)      144 2023-11-02 01:24:43.000000 hydrobot-0.5.0/prototypes/output_dump/.gitignore
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-02 20:04:32.572867 hydrobot-0.5.0/prototypes/py_scripts/
--rw-r--r--   0 nic       (1000) nic       (1000)     1515 2024-03-11 01:19:58.000000 hydrobot-0.5.0/prototypes/py_scripts/atmospheric_spike_removal.py
--rw-r--r--   0 nic       (1000) nic       (1000)     1051 2024-03-11 01:19:58.000000 hydrobot-0.5.0/prototypes/py_scripts/example_plot_script.py
--rw-r--r--   0 nic       (1000) nic       (1000)     1581 2024-04-01 22:51:29.000000 hydrobot-0.5.0/prototypes/py_scripts/gap_finder.py
--rw-r--r--   0 nic       (1000) nic       (1000)     1319 2024-03-11 01:19:58.000000 hydrobot-0.5.0/prototypes/py_scripts/new_ws_plot_with_check_data.py
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-02 20:04:32.572867 hydrobot-0.5.0/prototypes/py_scripts/output_dump/
--rw-r--r--   0 nic       (1000) nic       (1000)      144 2023-11-02 01:24:43.000000 hydrobot-0.5.0/prototypes/py_scripts/output_dump/.gitignore
--rw-r--r--   0 nic       (1000) nic       (1000)     1001 2024-03-11 01:19:58.000000 hydrobot-0.5.0/prototypes/py_scripts/plot_with_check_data.py
--rw-r--r--   0 nic       (1000) nic       (1000)     4222 2024-03-11 01:19:58.000000 hydrobot-0.5.0/prototypes/py_scripts/process_script.py
--rw-r--r--   0 nic       (1000) nic       (1000)      933 2023-12-03 22:14:39.000000 hydrobot-0.5.0/prototypes/py_scripts/spike_removal_util.py
--rw-r--r--   0 nic       (1000) nic       (1000)     3509 2024-03-11 01:19:58.000000 hydrobot-0.5.0/prototypes/py_scripts/stage_full_process.py
--rw-r--r--   0 nic       (1000) nic       (1000)     3627 2024-03-11 01:19:58.000000 hydrobot-0.5.0/prototypes/py_scripts/water_temp_full_process.py
--rw-r--r--   0 nic       (1000) nic       (1000)     1927 2023-11-02 02:57:00.000000 hydrobot-0.5.0/prototypes/py_scripts/water_temp_spike_removal.py
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-02 20:04:32.572867 hydrobot-0.5.0/prototypes/script_dump/
--rw-r--r--   0 nic       (1000) nic       (1000)      144 2024-03-11 01:19:58.000000 hydrobot-0.5.0/prototypes/script_dump/.gitignore
--rw-r--r--   0 nic       (1000) nic       (1000)     1419 2024-03-11 01:19:58.000000 hydrobot-0.5.0/prototypes/site_list_reader.py
--rw-r--r--   0 nic       (1000) nic       (1000)      443 2024-03-11 01:19:58.000000 hydrobot-0.5.0/prototypes/site_parameters.json
--rw-r--r--   0 nic       (1000) nic       (1000)     3088 2024-04-02 20:01:08.000000 hydrobot-0.5.0/pyproject.toml
--rw-r--r--   0 nic       (1000) nic       (1000)     2419 2024-04-02 20:02:29.000000 hydrobot-0.5.0/requirements_dev.txt
--rw-r--r--   0 nic       (1000) nic       (1000)      506 2024-03-11 01:19:58.000000 hydrobot-0.5.0/requirements_test.txt
--rw-r--r--   0 nic       (1000) nic       (1000)       38 2024-04-02 20:04:32.582867 hydrobot-0.5.0/setup.cfg
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-02 20:04:32.572867 hydrobot-0.5.0/tests/
--rw-r--r--   0 nic       (1000) nic       (1000)    53248 2024-02-26 00:40:14.000000 hydrobot-0.5.0/tests/.coverage
--rw-r--r--   0 nic       (1000) nic       (1000)       38 2023-11-02 02:57:00.000000 hydrobot-0.5.0/tests/__init__.py
--rw-r--r--   0 nic       (1000) nic       (1000)     1007 2024-03-11 01:19:58.000000 hydrobot-0.5.0/tests/conftest.py
--rw-r--r--   0 nic       (1000) nic       (1000)      245 2023-11-02 01:24:43.000000 hydrobot-0.5.0/tests/site_list_response.xml
--rw-r--r--   0 nic       (1000) nic       (1000)     2929 2024-03-11 01:19:58.000000 hydrobot-0.5.0/tests/test_data_sources.py
--rw-r--r--   0 nic       (1000) nic       (1000)     9730 2024-04-02 00:40:43.000000 hydrobot-0.5.0/tests/test_data_structure.py
--rw-r--r--   0 nic       (1000) nic       (1000)    12753 2024-03-11 01:19:58.000000 hydrobot-0.5.0/tests/test_evaluator.py
--rw-r--r--   0 nic       (1000) nic       (1000)     9481 2024-03-11 01:19:58.000000 hydrobot-0.5.0/tests/test_filters.py
--rw-r--r--   0 nic       (1000) nic       (1000)    24981 2024-04-02 01:02:45.000000 hydrobot-0.5.0/tests/test_processor.py
--rw-r--r--   0 nic       (1000) nic       (1000)     2557 2024-04-01 22:51:29.000000 hydrobot-0.5.0/tests/test_utils.py
--rw-r--r--   0 nic       (1000) nic       (1000)    24135 2024-04-02 01:19:50.000000 hydrobot-0.5.0/tests/test_web_integration.py
--rw-r--r--   0 nic       (1000) nic       (1000)    13995 2024-04-02 00:42:31.000000 hydrobot-0.5.0/tests/xml_test_data_file.xml
+drwxrwxrwx   0        0        0        0 2024-04-03 20:11:46.690471 hydrobot-0.5.1/
+-rw-rw-rw-   0        0        0      313 2023-10-15 22:10:03.000000 hydrobot-0.5.1/.editorconfig
+drwxrwxrwx   0        0        0        0 2024-04-03 20:11:46.594548 hydrobot-0.5.1/.github/
+-rw-rw-rw-   0        0        0      348 2023-10-12 20:23:48.000000 hydrobot-0.5.1/.github/ISSUE_TEMPLATE.md
+-rw-rw-rw-   0        0        0     1313 2023-10-29 22:37:56.000000 hydrobot-0.5.1/.gitignore
+-rw-rw-rw-   0        0        0      538 2023-12-11 20:49:23.000000 hydrobot-0.5.1/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0     1106 2023-12-12 22:15:59.000000 hydrobot-0.5.1/.readthedocs.yaml
+-rw-rw-rw-   0        0        0      226 2023-10-16 01:04:07.000000 hydrobot-0.5.1/AUTHORS.rst
+-rw-rw-rw-   0        0        0     7528 2024-04-03 19:51:02.000000 hydrobot-0.5.1/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     1574 2024-04-03 04:44:04.000000 hydrobot-0.5.1/HISTORY.rst
+-rw-rw-rw-   0        0        0     1642 2023-10-16 03:16:48.000000 hydrobot-0.5.1/LICENSE
+-rw-rw-rw-   0        0        0      310 2023-12-12 22:15:59.000000 hydrobot-0.5.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2424 2023-12-12 22:23:23.000000 hydrobot-0.5.1/Makefile
+-rw-rw-rw-   0        0        0     7183 2024-04-03 20:11:46.688435 hydrobot-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5409 2024-04-03 04:44:04.000000 hydrobot-0.5.1/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-03 20:11:46.610221 hydrobot-0.5.1/docs/
+-rw-rw-rw-   0        0        0      629 2023-11-19 21:41:44.000000 hydrobot-0.5.1/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2023-10-12 20:23:48.000000 hydrobot-0.5.1/docs/authors.rst
+-rw-rw-rw-   0        0        0     5266 2023-12-12 22:15:59.000000 hydrobot-0.5.1/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-10-12 20:23:48.000000 hydrobot-0.5.1/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-10-12 20:23:48.000000 hydrobot-0.5.1/docs/history.rst
+-rw-rw-rw-   0        0        0     1259 2023-12-11 20:49:23.000000 hydrobot-0.5.1/docs/hydrobot.rst
+-rw-rw-rw-   0        0        0      325 2023-11-19 21:41:44.000000 hydrobot-0.5.1/docs/index.rst
+-rw-rw-rw-   0        0        0     1626 2023-12-10 21:58:59.000000 hydrobot-0.5.1/docs/installation.rst
+-rwxrwxrwx   0        0        0      806 2023-11-19 21:41:44.000000 hydrobot-0.5.1/docs/make.bat
+-rw-rw-rw-   0        0        0       68 2023-11-20 00:56:14.000000 hydrobot-0.5.1/docs/modules.rst
+-rw-rw-rw-   0        0        0       28 2023-10-12 20:23:48.000000 hydrobot-0.5.1/docs/readme.rst
+-rw-rw-rw-   0        0        0       78 2023-11-19 21:41:44.000000 hydrobot-0.5.1/docs/usage.rst
+drwxrwxrwx   0        0        0        0 2024-04-03 20:11:46.625817 hydrobot-0.5.1/hydrobot/
+-rw-rw-rw-   0        0        0      158 2024-04-03 19:54:28.000000 hydrobot-0.5.1/hydrobot/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 20:11:46.636265 hydrobot-0.5.1/hydrobot/config/
+-rw-rw-rw-   0        0        0      108 2024-02-04 21:42:36.000000 hydrobot-0.5.1/hydrobot/config/QualityCodeEvaluator_QC_config.csv
+-rw-rw-rw-   0        0        0       56 2024-01-29 01:11:26.000000 hydrobot-0.5.1/hydrobot/config/TwoLevelQualityCodeEvaluator_QC_config.csv
+-rw-rw-rw-   0        0        0     5944 2024-04-02 01:26:24.000000 hydrobot-0.5.1/hydrobot/data_acquisition.py
+-rw-rw-rw-   0        0        0     8291 2024-04-02 01:26:24.000000 hydrobot-0.5.1/hydrobot/data_sources.py
+-rw-rw-rw-   0        0        0    33643 2024-04-02 01:26:24.000000 hydrobot-0.5.1/hydrobot/data_structure.py
+-rw-rw-rw-   0        0        0    14223 2024-04-02 01:26:24.000000 hydrobot-0.5.1/hydrobot/evaluator.py
+-rw-rw-rw-   0        0        0     7765 2024-01-29 01:11:26.000000 hydrobot-0.5.1/hydrobot/filters.py
+-rw-rw-rw-   0        0        0    21458 2024-04-02 01:26:24.000000 hydrobot-0.5.1/hydrobot/plotter.py
+-rw-rw-rw-   0        0        0    53652 2024-04-03 04:44:04.000000 hydrobot-0.5.1/hydrobot/processor.py
+-rw-rw-rw-   0        0        0     8034 2024-04-02 01:26:24.000000 hydrobot-0.5.1/hydrobot/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-03 20:11:46.686381 hydrobot-0.5.1/hydrobot.egg-info/
+-rw-rw-rw-   0        0        0     7183 2024-04-03 20:11:46.000000 hydrobot-0.5.1/hydrobot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1984 2024-04-03 20:11:46.000000 hydrobot-0.5.1/hydrobot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 20:11:46.000000 hydrobot-0.5.1/hydrobot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      311 2024-04-03 20:11:46.000000 hydrobot-0.5.1/hydrobot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-03 20:11:46.000000 hydrobot-0.5.1/hydrobot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      446 2023-12-12 22:25:27.000000 hydrobot-0.5.1/old_setup.cfg
+-rw-rw-rw-   0        0        0     1624 2023-12-12 22:25:27.000000 hydrobot-0.5.1/old_setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 20:11:46.641418 hydrobot-0.5.1/prototypes/
+-rw-rw-rw-   0        0        0     4395 2024-04-02 01:30:48.000000 hydrobot-0.5.1/prototypes/Class_script.py
+drwxrwxrwx   0        0        0        0 2024-04-03 20:11:46.645569 hydrobot-0.5.1/prototypes/example_script/
+-rw-rw-rw-   0        0        0    10156 2024-04-03 02:34:16.000000 hydrobot-0.5.1/prototypes/example_script/WaterTemp_CheckData.R
+-rw-rw-rw-   0        0        0     1136 2024-04-03 02:34:16.000000 hydrobot-0.5.1/prototypes/example_script/config.yaml
+-rw-rw-rw-   0        0        0     5466 2024-04-03 04:44:04.000000 hydrobot-0.5.1/prototypes/example_script/script.py
+drwxrwxrwx   0        0        0        0 2024-04-03 20:11:46.646569 hydrobot-0.5.1/prototypes/output_dump/
+-rw-rw-rw-   0        0        0      144 2023-10-29 23:49:09.000000 hydrobot-0.5.1/prototypes/output_dump/.gitignore
+drwxrwxrwx   0        0        0        0 2024-04-03 20:11:46.662304 hydrobot-0.5.1/prototypes/py_scripts/
+-rw-rw-rw-   0        0        0     1592 2024-01-29 01:11:26.000000 hydrobot-0.5.1/prototypes/py_scripts/atmospheric_spike_removal.py
+-rw-rw-rw-   0        0        0     1085 2023-12-11 20:49:23.000000 hydrobot-0.5.1/prototypes/py_scripts/example_plot_script.py
+-rw-rw-rw-   0        0        0     1643 2024-04-02 01:26:24.000000 hydrobot-0.5.1/prototypes/py_scripts/gap_finder.py
+-rw-rw-rw-   0        0        0     1376 2023-12-11 20:49:23.000000 hydrobot-0.5.1/prototypes/py_scripts/new_ws_plot_with_check_data.py
+drwxrwxrwx   0        0        0        0 2024-04-03 20:11:46.663365 hydrobot-0.5.1/prototypes/py_scripts/output_dump/
+-rw-rw-rw-   0        0        0      144 2023-10-29 23:49:09.000000 hydrobot-0.5.1/prototypes/py_scripts/output_dump/.gitignore
+-rw-rw-rw-   0        0        0     1050 2023-12-11 20:49:23.000000 hydrobot-0.5.1/prototypes/py_scripts/plot_with_check_data.py
+-rw-rw-rw-   0        0        0     4356 2024-01-29 01:11:26.000000 hydrobot-0.5.1/prototypes/py_scripts/process_script.py
+-rw-rw-rw-   0        0        0      970 2023-11-19 21:41:44.000000 hydrobot-0.5.1/prototypes/py_scripts/spike_removal_util.py
+-rw-rw-rw-   0        0        0     3634 2024-01-29 01:11:26.000000 hydrobot-0.5.1/prototypes/py_scripts/stage_full_process.py
+-rw-rw-rw-   0        0        0     3763 2024-01-29 01:11:26.000000 hydrobot-0.5.1/prototypes/py_scripts/water_temp_full_process.py
+-rw-rw-rw-   0        0        0     2000 2023-11-19 21:41:44.000000 hydrobot-0.5.1/prototypes/py_scripts/water_temp_spike_removal.py
+drwxrwxrwx   0        0        0        0 2024-04-03 20:11:46.664365 hydrobot-0.5.1/prototypes/script_dump/
+-rw-rw-rw-   0        0        0      147 2024-02-04 21:42:36.000000 hydrobot-0.5.1/prototypes/script_dump/.gitignore
+-rw-rw-rw-   0        0        0     1474 2024-01-29 01:11:26.000000 hydrobot-0.5.1/prototypes/site_list_reader.py
+-rw-rw-rw-   0        0        0      444 2024-01-29 01:11:26.000000 hydrobot-0.5.1/prototypes/site_parameters.json
+-rw-rw-rw-   0        0        0     3204 2024-04-03 19:54:28.000000 hydrobot-0.5.1/pyproject.toml
+-rw-rw-rw-   0        0        0     2555 2024-04-02 01:29:55.000000 hydrobot-0.5.1/requirements_dev.txt
+-rw-rw-rw-   0        0        0      535 2023-12-10 20:57:09.000000 hydrobot-0.5.1/requirements_test.txt
+-rw-rw-rw-   0        0        0       42 2024-04-03 20:11:46.690471 hydrobot-0.5.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-03 20:11:46.684348 hydrobot-0.5.1/tests/
+-rw-rw-rw-   0        0        0       39 2023-11-19 21:41:44.000000 hydrobot-0.5.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     1038 2024-01-29 01:11:26.000000 hydrobot-0.5.1/tests/conftest.py
+-rw-rw-rw-   0        0        0      252 2023-11-02 01:26:39.000000 hydrobot-0.5.1/tests/site_list_response.xml
+-rw-rw-rw-   0        0        0     3005 2024-03-08 01:46:33.000000 hydrobot-0.5.1/tests/test_data_sources.py
+-rw-rw-rw-   0        0        0     9995 2024-04-02 01:26:24.000000 hydrobot-0.5.1/tests/test_data_structure.py
+-rw-rw-rw-   0        0        0    13060 2024-01-29 03:22:08.000000 hydrobot-0.5.1/tests/test_evaluator.py
+-rw-rw-rw-   0        0        0     9782 2024-01-29 01:11:26.000000 hydrobot-0.5.1/tests/test_filters.py
+-rw-rw-rw-   0        0        0    25737 2024-04-02 01:26:24.000000 hydrobot-0.5.1/tests/test_processor.py
+-rw-rw-rw-   0        0        0     2651 2024-04-02 01:26:24.000000 hydrobot-0.5.1/tests/test_utils.py
+-rw-rw-rw-   0        0        0    24805 2024-04-02 01:26:24.000000 hydrobot-0.5.1/tests/test_web_integration.py
+-rw-rw-rw-   0        0        0    14403 2024-03-08 03:10:28.000000 hydrobot-0.5.1/tests/xml_test_data_file.xml
```

### Comparing `hydrobot-0.5.0/.readthedocs.yaml` & `hydrobot-0.5.1/.readthedocs.yaml`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-# Read the Docs configuration file for Sphinx projects
-# See https://docs.readthedocs.io/en/stable/config-file/v2.html for details
-
-# Required
-version: 2
-
-# Set the OS, Python version and other tools you might need
-build:
-  os: ubuntu-22.04
-  tools:
-    python: "3.11"
-    # You can also specify other tool versions:
-    # nodejs: "20"
-    # rust: "1.70"
-    # golang: "1.20"
-
-# Build documentation in the "docs/" directory with Sphinx
-sphinx:
-  configuration: docs/conf.py
-  # You can configure Sphinx to use a different builder, for instance use the dirhtml builder for simpler URLs
-  # builder: "dirhtml"
-  # Fail on all warnings to avoid broken references
-  # fail_on_warning: true
-
-# Optionally build your docs in additional formats such as PDF and ePub
-formats:
-   - pdf
-#    - epub
-
-# Optional but recommended, declare the Python requirements required
-# to build your documentation
-# See https://docs.readthedocs.io/en/stable/guides/reproducible-builds.html
-python:
-   install:
-      - method: pip
-        path: .
-        extra_requirements:
-            - docs
+# Read the Docs configuration file for Sphinx projects
+# See https://docs.readthedocs.io/en/stable/config-file/v2.html for details
+
+# Required
+version: 2
+
+# Set the OS, Python version and other tools you might need
+build:
+  os: ubuntu-22.04
+  tools:
+    python: "3.11"
+    # You can also specify other tool versions:
+    # nodejs: "20"
+    # rust: "1.70"
+    # golang: "1.20"
+
+# Build documentation in the "docs/" directory with Sphinx
+sphinx:
+  configuration: docs/conf.py
+  # You can configure Sphinx to use a different builder, for instance use the dirhtml builder for simpler URLs
+  # builder: "dirhtml"
+  # Fail on all warnings to avoid broken references
+  # fail_on_warning: true
+
+# Optionally build your docs in additional formats such as PDF and ePub
+formats:
+   - pdf
+#    - epub
+
+# Optional but recommended, declare the Python requirements required
+# to build your documentation
+# See https://docs.readthedocs.io/en/stable/guides/reproducible-builds.html
+python:
+   install:
+      - method: pip
+        path: .
+        extra_requirements:
+            - docs
```

### Comparing `hydrobot-0.5.0/CONTRIBUTING.rst` & `hydrobot-0.5.1/CONTRIBUTING.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,209 +1,219 @@
-.. highlight:: shell
-
-============
-Contributing
-============
-
-Contributions are welcome, and they are greatly appreciated! Every little bit
-helps, and credit will always be given.
-
-You can contribute in many ways:
-
-Types of Contributions
-----------------------
-
-Report Bugs
-~~~~~~~~~~~
-
-Report bugs at https://github.com/nicmostert/hydrobot/issues.
-
-If you are reporting a bug, please include:
-
-* Your operating system name and version.
-* Any details about your local setup that might be helpful in troubleshooting.
-* Detailed steps to reproduce the bug.
-
-Fix Bugs
-~~~~~~~~
-
-Look through the GitHub issues for bugs. Anything tagged with "bug" and "help
-wanted" is open to whoever wants to implement it.
-
-Implement Features
-~~~~~~~~~~~~~~~~~~
-
-Look through the GitHub issues for features. Anything tagged with "enhancement"
-and "help wanted" is open to whoever wants to implement it.
-
-Write Documentation
-~~~~~~~~~~~~~~~~~~~
-
-Hydro Processing Tools could always use more documentation, whether as part of the
-official Hydro Processing Tools docs, in docstrings, or even on the web in blog posts,
-articles, and such.
-
-Submit Feedback
-~~~~~~~~~~~~~~~
-
-The best way to send feedback is to file an issue at https://github.com/nicmostert/hydrobot/issues.
-
-If you are proposing a feature:
-
-* Explain in detail how it would work.
-* Keep the scope as narrow as possible, to make it easier to implement.
-* Remember that this is a volunteer-driven project, and that contributions
-  are welcome :)
-
-Get Started!
-------------
-
-Ready to contribute? Here's how to set up `hydrobot` for local development.
-
-1. Fork the `hydrobot` repo on GitHub.
-2. Clone your fork locally::
-
-    $ git clone git@github.com:your_name_here/hydrobot.git
-
-3. Install your local copy into a venv. This is how you set up your fork for local development
-
-Switch to the newly created root directory of the project::
-
-    $ cd hydrobot/
-
-Create a virtual environment for this project::
-
-    $ python -m venv path/to/venv/location/
-
-Activate the virtual environment:
-
-Unix::
-
-    $ source path/to/venv/location/bin/activate
-
-Windows (Powershell)::
-
-    $ ./path/to/venv/location/Scripts/Activate.ps1
-
-Windows (cmd)::
-
-    $ ./path/to/venv/location/Scripts/activate.bat
-
-Once within the venv, install the required packages for development::
-
-    $ python -m pip install -r requirements_dev.txt
-
-Finally, install the hydrobot in "editable" (or "develop") mode.
-This allows you to import the package into test scripts and prototypes, while allowing you to edit the package in-place without reinstallation.::
-
-    $ python -m pip install -e .
-
-4. Create a branch for local development
-
-In order to track local changes, you must create a branch for local development.
-This command creates a local brach, then switches to that branch.::
-
-    $ git checkout -b name-of-your-bugfix-or-feature
-
-Now you can make your changes locally.
-
-   *NOTE: It is good practice to give your branch a name based on the changes you are planning to make. E.g. "adding-signal-processing-feature" or "fixing-bug-in-spike-filter".*
-
-5. When you're done making changes, verify that all tests still pass on your branch::
-
-    $ pytest
-
-Your branch will not be allowed to merge if all tests do not pass. [*NOTE: This is not technically true yet, but it will be once I figure it out.*]
-
-6. When you're done making changes, commit your changes and push your branch to GitHub::
-
-    $ git add .
-    $ git commit -m "Your detailed description of your changes."
-
-This project makes use of various pre-commit hooks. Importantly, this code-base conforms to `black` formatting.
-If your test fails, follow the instructions on how to fix any problems, and then repeat the commit command. In some cases, the pre-commit hooks will automatically fix all problems. In such cases, the changes need to be staged with `git add .` again then commit again. Since the failed commit didn't go through, feel free to use the same commit message as before.
-
-To run all the pre-commit hooks without making a commit (e.g. to check if the auto-fixes solved all the problems), you can run::
-
-    $ pre-commit run --all-files
-
-When all checks pass and your changes are committed sucessfully, you may push your changes to the remote version of your branch::
-
-    $ git push origin name-of-your-bugfix-or-feature
-
-7. Submit a pull request through the GitHub website. Provide a detailed description of the changes you have made to ensure that they can be merged efficiently.
-
-Pull Request Guidelines
------------------------
-
-Before you submit a pull request, check that it meets these guidelines:
-
-1. The pull request should include tests.
-2. If the pull request adds functionality, the docs should be updated. Put
-   your new functionality into a function with a docstring, and add the
-   feature to the appropriate location in the documentation.
-
-Tips
-----
-
-To run a subset of tests::
-
-$ pytest tests.test_hydrobot
-
-
-Releasing to PyPI
-------------------
-
-A reminder for the maintainers on how to deploy.
-
-1. Make sure all your changes are committed (including an entry in HISTORY.rst, documentation, etc.).
-
-2. Then run `bump-my-version` to increment the release tags in the appropriate places. Consider using the `--dry-run` flag to make sure there are no errors first::
-
-    $ bump-my-version bump -v --dry-run patch # Optional, just to test if it runs without errors
-    $ bump-my-version bump patch # For real this time. Possible values: major / minor / patch
-
-3. Install the local development version of the package (make sure you're in the package root directory where setup.py is). You should see the package install with the correct version number.::
-
-    $ pip install -e .[all]
-
-4. Run the tests to see that they still work with this local install::
-
-    $ pytest
-
-5. Push the commit::
-
-    $ git push
-
-6. Push the tags to GitHub. (Note that we don't actually release on GitHub though. We want to keep the releases to PyPI so there's less ambiguity about how to install it.)::
-
-    $ git push --tags
-
-7. Do the release.
-
-    * If using the Makefile (i.e. you have `make` installed and can run `make help` without errors) you can simply run::
-
-        $ make release
-
-    * Otherwise, you would have to do the release manually.
-
-        a. Clean up all the artifact files::
-
-            $ rm -fr build/
-            $ rm -fr dist/
-            $ rm -fr .eggs/
-            $ find . -name '*.egg-info' -exec rm -fr {} +
-            $ find . -name '*.egg' -exec rm -f {} +
-            $ find . -name '*.pyc' -exec rm -f {} +
-            $ find . -name '*.pyo' -exec rm -f {} +
-            $ find . -name '*~' -exec rm -f {} +
-            $ find . -name '__pycache__' -exec rm -fr {} +
-	        $ rm -fr .pytest_cache
-
-        b. Build the source and wheel packages::
-
-            $ python -m build
-            $ ls -l dist
-
-        c. Use twine to release to PyPI. You'll be asked for authentication. Use the username `__token__`, along with the API key I gave you.::
-
-            $ twine upload dist/*
+.. highlight:: shell
+
+============
+Contributing
+============
+
+Contributions are welcome, and they are greatly appreciated! Every little bit
+helps, and credit will always be given.
+
+You can contribute in many ways:
+
+Types of Contributions
+----------------------
+
+Report Bugs
+~~~~~~~~~~~
+
+Report bugs at https://github.com/nicmostert/hydrobot/issues.
+
+If you are reporting a bug, please include:
+
+* Your operating system name and version.
+* Any details about your local setup that might be helpful in troubleshooting.
+* Detailed steps to reproduce the bug.
+
+Fix Bugs
+~~~~~~~~
+
+Look through the GitHub issues for bugs. Anything tagged with "bug" and "help
+wanted" is open to whoever wants to implement it.
+
+Implement Features
+~~~~~~~~~~~~~~~~~~
+
+Look through the GitHub issues for features. Anything tagged with "enhancement"
+and "help wanted" is open to whoever wants to implement it.
+
+Write Documentation
+~~~~~~~~~~~~~~~~~~~
+
+Hydro Processing Tools could always use more documentation, whether as part of the
+official Hydro Processing Tools docs, in docstrings, or even on the web in blog posts,
+articles, and such.
+
+Submit Feedback
+~~~~~~~~~~~~~~~
+
+The best way to send feedback is to file an issue at https://github.com/nicmostert/hydrobot/issues.
+
+If you are proposing a feature:
+
+* Explain in detail how it would work.
+* Keep the scope as narrow as possible, to make it easier to implement.
+* Remember that this is a volunteer-driven project, and that contributions
+  are welcome :)
+
+Get Started!
+------------
+
+Ready to contribute? Here's how to set up `hydrobot` for local development.
+
+1. Fork the `hydrobot` repo on GitHub.
+2. Clone your fork locally::
+
+    $ git clone git@github.com:your_name_here/hydrobot.git
+
+3. Install your local copy into a venv. This is how you set up your fork for local development
+
+Switch to the newly created root directory of the project::
+
+    $ cd hydrobot/
+
+Create a virtual environment for this project::
+
+    $ python -m venv path/to/venv/location/
+
+Activate the virtual environment:
+
+Unix::
+
+    $ source path/to/venv/location/bin/activate
+
+Windows (Powershell)::
+
+    $ ./path/to/venv/location/Scripts/Activate.ps1
+
+Windows (cmd)::
+
+    $ ./path/to/venv/location/Scripts/activate.bat
+
+Once within the venv, install the required packages for development::
+
+    $ python -m pip install -r requirements_dev.txt
+
+Finally, install the hydrobot in "editable" (or "develop") mode.
+This allows you to import the package into test scripts and prototypes, while allowing you to edit the package in-place without reinstallation.::
+
+    $ python -m pip install -e .
+
+4. Create a branch for local development
+
+In order to track local changes, you must create a branch for local development.
+This command creates a local brach, then switches to that branch.::
+
+    $ git checkout -b name-of-your-bugfix-or-feature
+
+Now you can make your changes locally.
+
+   *NOTE: It is good practice to give your branch a name based on the changes you are planning to make. E.g. "adding-signal-processing-feature" or "fixing-bug-in-spike-filter".*
+
+5. When you're done making changes, verify that all tests still pass on your branch::
+
+    $ pytest
+
+Your branch will not be allowed to merge if all tests do not pass. [*NOTE: This is not technically true yet, but it will be once I figure it out.*]
+
+6. When you're done making changes, commit your changes and push your branch to GitHub::
+
+    $ git add .
+    $ git commit -m "Your detailed description of your changes."
+
+This project makes use of various pre-commit hooks. Importantly, this code-base conforms to `black` formatting.
+If your test fails, follow the instructions on how to fix any problems, and then repeat the commit command. In some cases, the pre-commit hooks will automatically fix all problems. In such cases, the changes need to be staged with `git add .` again then commit again. Since the failed commit didn't go through, feel free to use the same commit message as before.
+
+To run all the pre-commit hooks without making a commit (e.g. to check if the auto-fixes solved all the problems), you can run::
+
+    $ pre-commit run --all-files
+
+When all checks pass and your changes are committed sucessfully, you may push your changes to the remote version of your branch::
+
+    $ git push origin name-of-your-bugfix-or-feature
+
+7. Submit a pull request through the GitHub website. Provide a detailed description of the changes you have made to ensure that they can be merged efficiently.
+
+Pull Request Guidelines
+-----------------------
+
+Before you submit a pull request, check that it meets these guidelines:
+
+1. The pull request should include tests.
+2. If the pull request adds functionality, the docs should be updated. Put
+   your new functionality into a function with a docstring, and add the
+   feature to the appropriate location in the documentation.
+
+Tips
+----
+
+To run a subset of tests::
+
+$ pytest tests.test_hydrobot
+
+
+Releasing to PyPI
+------------------
+
+A reminder for the maintainers on how to deploy.
+
+1. Make sure all your changes are committed (including an entry in HISTORY.rst, documentation, etc.).
+
+2. Confirm the repo is an a good state::
+
+    $ pre-commit run --all-files
+    $ pytest
+
+3. Then run `bump-my-version` to increment the release tags in the appropriate places. Consider using the `--dry-run`
+flag to make sure there are no errors first. bump-my-version has a dependency on a modern version of pydantic (and
+hilltop-py requires an older version) so bump-my-version needs to be installed fresh (don't pip freeze after)::
+
+    $ pip install bump-my-version
+    $ bump-my-version bump -v --dry-run patch # Optional, just to test if it runs without errors
+    $ bump-my-version bump patch # For real this time. Possible values: major / minor / patch
+
+4. Install the local development version of the package (make sure you're in the package root directory where setup
+.py is). You should see the package install with the correct version number.::
+
+    $ pip install -e .[all]
+
+5. Run the tests to see that they still work with this local install::
+
+    $ pytest
+
+6. Push the commit::
+
+    $ git push
+
+7. Push the tags to GitHub. (Note that we don't actually release on GitHub though. We want to keep the releases to
+PyPI so there's less ambiguity about how to install it.)::
+
+    $ git push --tags
+
+8. Do the release.
+
+    * If using the Makefile (i.e. you have `make` installed and can run `make help` without errors) you can simply run::
+
+        $ make release
+
+    * Otherwise, you would have to do the release manually.
+
+        a. Clean up all the artifact files::
+
+            $ rm -fr build/
+            $ rm -fr dist/
+            $ rm -fr .eggs/
+            $ find . -name '*.egg-info' -exec rm -fr {} +
+            $ find . -name '*.egg' -exec rm -f {} +
+            $ find . -name '*.pyc' -exec rm -f {} +
+            $ find . -name '*.pyo' -exec rm -f {} +
+            $ find . -name '*~' -exec rm -f {} +
+            $ find . -name '__pycache__' -exec rm -fr {} +
+	        $ rm -fr .pytest_cache
+
+        b. Build the source and wheel packages::
+
+            $ python -m build
+            $ ls -l dist
+
+        c. Use twine to release to PyPI. You'll be asked for authentication. Use the username `__token__`, along with the API key I gave you.::
+
+            $ twine upload dist/*
```

### Comparing `hydrobot-0.5.0/HISTORY.rst` & `hydrobot-0.5.1/HISTORY.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,66 +1,72 @@
-=======
-History
-=======
-
-0.1.0 (2023-09-27)
-------------------
-
-* First release on PyPI.
-
-0.2.0 (2023-09-27)
-------------------
-
-* Hydrobot now annals the "Processor" class, which has capabilities to process data within the single object. Class_script gives an example of this method of processing.
-
-0.2.1 (2023-09-27)
-------------------
-
-* Including the config files, + getting wheeled boi
-
-0.2.2 (2023-09-27)
-------------------
-
-* Ok, actually including the config files (promise, but my fingers are crossed behind my back)
-
-0.2.3 (2023-11-30)
-------------------
-
-* Fixed some tests and hopefully fixed the config file issue this time.
-
-0.3.0 (2023-12-11)
-------------------
-
-* Can delete data now.
-
-0.3.1 (2023-12-12)
-------------------
-
-* No longer exports the ending QC0 data.
-* Changed to pyproject.toml to get with the times.
-
-0.3.2 (2023-12-12)
-------------------
-
-* Fixed a documentation build bug
-
-0.3.3 (2023-12-12)
-------------------
-
-* Fixed a documentation build bug again.
-
-0.3.4 (2023-12-12)
-------------------
-
-* Implementing the QC0 data removal tool promised in 0.3.1
-
-0.4.0 (2024-01-30)
-------------------
-
-* XML backend and exporting support added.
-
-0.5.0 (2024-04-03) - Alpha Release
-----------------------------------
-
-* Plotly diagnostics added.
-* Support for external (to Hilltop) check data added.
-* Hybrid workflow supported and documented.
+=======
+History
+=======
+
+0.1.0 (2023-09-27)
+------------------
+
+* First release on PyPI.
+
+0.2.0 (2023-09-27)
+------------------
+
+* Hydrobot now annals the "Processor" class, which has capabilities to process data within the single object. Class_script gives an example of this method of processing.
+
+0.2.1 (2023-09-27)
+------------------
+
+* Including the config files, + getting wheeled boi
+
+0.2.2 (2023-09-27)
+------------------
+
+* Ok, actually including the config files (promise, but my fingers are crossed behind my back)
+
+0.2.3 (2023-11-30)
+------------------
+
+* Fixed some tests and hopefully fixed the config file issue this time.
+
+0.3.0 (2023-12-11)
+------------------
+
+* Can delete data now.
+
+0.3.1 (2023-12-12)
+------------------
+
+* No longer exports the ending QC0 data.
+* Changed to pyproject.toml to get with the times.
+
+0.3.2 (2023-12-12)
+------------------
+
+* Fixed a documentation build bug
+
+0.3.3 (2023-12-12)
+------------------
+
+* Fixed a documentation build bug again.
+
+0.3.4 (2023-12-12)
+------------------
+
+* Implementing the QC0 data removal tool promised in 0.3.1
+
+0.4.0 (2024-01-30)
+------------------
+
+* XML backend and exporting support added.
+
+0.5.0 (2024-04-03) - Alpha Release
+----------------------------------
+
+* Plotly diagnostics added.
+* Support for external (to Hilltop) check data added.
+* Hybrid workflow supported and documented.
+
+0.5.1 (2024-04-03)
+----------------------------------
+
+* Updated documentation for workflow
+* Added a supplementary R script to repo
```

### Comparing `hydrobot-0.5.0/LICENSE` & `hydrobot-0.5.1/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-GNU GENERAL PUBLIC LICENSE
-                      Version 3, 29 June 2007
-
-    Python Package providing a suite of processing tools and utilities for Hilltop hydrological data.
-    Copyright (C) 2023  Nic Mostert
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<http://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<http://www.gnu.org/philosophy/why-not-lgpl.html>.
+GNU GENERAL PUBLIC LICENSE
+                      Version 3, 29 June 2007
+
+    Python Package providing a suite of processing tools and utilities for Hilltop hydrological data.
+    Copyright (C) 2023  Nic Mostert
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<http://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<http://www.gnu.org/philosophy/why-not-lgpl.html>.
```

### Comparing `hydrobot-0.5.0/Makefile` & `hydrobot-0.5.1/Makefile`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-.PHONY: clean clean-build clean-pyc clean-test coverage dist docs help install lint lint/flake8 lint/black
-.DEFAULT_GOAL := help
-
-define BROWSER_PYSCRIPT
-import os, webbrowser, sys
-
-from urllib.request import pathname2url
-
-webbrowser.open("file://" + pathname2url(os.path.abspath(sys.argv[1])))
-endef
-export BROWSER_PYSCRIPT
-
-define PRINT_HELP_PYSCRIPT
-import re, sys
-
-for line in sys.stdin:
-	match = re.match(r'^([a-zA-Z_-]+):.*?## (.*)$$', line)
-	if match:
-		target, help = match.groups()
-		print("%-20s %s" % (target, help))
-endef
-export PRINT_HELP_PYSCRIPT
-
-BROWSER := python -c "$$BROWSER_PYSCRIPT"
-
-help:
-	@python -c "$$PRINT_HELP_PYSCRIPT" < $(MAKEFILE_LIST)
-
-clean: clean-build clean-pyc clean-test ## remove all build, test, coverage and Python artifacts
-
-clean-build: ## remove build artifacts
-	rm -fr build/
-	rm -fr dist/
-	rm -fr .eggs/
-	find . -name '*.egg-info' -exec rm -fr {} +
-	find . -name '*.egg' -exec rm -f {} +
-
-clean-pyc: ## remove Python file artifacts
-	find . -name '*.pyc' -exec rm -f {} +
-	find . -name '*.pyo' -exec rm -f {} +
-	find . -name '*~' -exec rm -f {} +
-	find . -name '__pycache__' -exec rm -fr {} +
-
-clean-test: ## remove test and coverage artifacts
-	rm -fr .tox/
-	rm -f .coverage
-	rm -fr htmlcov/
-	rm -fr .pytest_cache
-
-lint/flake8: ## check style with flake8
-	flake8 hydrobot tests
-lint/black: ## check style with black
-	black --check hydrobot tests
-
-lint: lint/flake8 lint/black ## check style
-
-test: ## run tests quickly with the default Python
-	pytest
-
-test-all: ## run tests on every Python version with tox
-	tox
-
-coverage: ## check code coverage quickly with the default Python
-	coverage run --source hydrobot -m pytest
-	coverage report -m
-	coverage html
-	$(BROWSER) htmlcov/index.html
-
-docs: ## generate Sphinx HTML documentation, including API docs
-	rm -f docs/hydrobot.rst
-	rm -f docs/modules.rst
-	sphinx-apidoc -o docs/ hydrobot
-	$(MAKE) -C docs clean
-	$(MAKE) -C docs html
-	$(BROWSER) docs/_build/html/index.html
-
-servedocs: docs ## compile the docs watching for changes
-	watchmedo shell-command -p '*.rst' -c '$(MAKE) -C docs html' -R -D .
-
-release: dist ## package and upload a release
-	twine upload dist/*
-
-dist: clean ## builds source and wheel package
-	python -m build
-	ls -l dist
-
-install: clean ## install the package to the active Python's site-packages
-	python setup.py install
+.PHONY: clean clean-build clean-pyc clean-test coverage dist docs help install lint lint/flake8 lint/black
+.DEFAULT_GOAL := help
+
+define BROWSER_PYSCRIPT
+import os, webbrowser, sys
+
+from urllib.request import pathname2url
+
+webbrowser.open("file://" + pathname2url(os.path.abspath(sys.argv[1])))
+endef
+export BROWSER_PYSCRIPT
+
+define PRINT_HELP_PYSCRIPT
+import re, sys
+
+for line in sys.stdin:
+	match = re.match(r'^([a-zA-Z_-]+):.*?## (.*)$$', line)
+	if match:
+		target, help = match.groups()
+		print("%-20s %s" % (target, help))
+endef
+export PRINT_HELP_PYSCRIPT
+
+BROWSER := python -c "$$BROWSER_PYSCRIPT"
+
+help:
+	@python -c "$$PRINT_HELP_PYSCRIPT" < $(MAKEFILE_LIST)
+
+clean: clean-build clean-pyc clean-test ## remove all build, test, coverage and Python artifacts
+
+clean-build: ## remove build artifacts
+	rm -fr build/
+	rm -fr dist/
+	rm -fr .eggs/
+	find . -name '*.egg-info' -exec rm -fr {} +
+	find . -name '*.egg' -exec rm -f {} +
+
+clean-pyc: ## remove Python file artifacts
+	find . -name '*.pyc' -exec rm -f {} +
+	find . -name '*.pyo' -exec rm -f {} +
+	find . -name '*~' -exec rm -f {} +
+	find . -name '__pycache__' -exec rm -fr {} +
+
+clean-test: ## remove test and coverage artifacts
+	rm -fr .tox/
+	rm -f .coverage
+	rm -fr htmlcov/
+	rm -fr .pytest_cache
+
+lint/flake8: ## check style with flake8
+	flake8 hydrobot tests
+lint/black: ## check style with black
+	black --check hydrobot tests
+
+lint: lint/flake8 lint/black ## check style
+
+test: ## run tests quickly with the default Python
+	pytest
+
+test-all: ## run tests on every Python version with tox
+	tox
+
+coverage: ## check code coverage quickly with the default Python
+	coverage run --source hydrobot -m pytest
+	coverage report -m
+	coverage html
+	$(BROWSER) htmlcov/index.html
+
+docs: ## generate Sphinx HTML documentation, including API docs
+	rm -f docs/hydrobot.rst
+	rm -f docs/modules.rst
+	sphinx-apidoc -o docs/ hydrobot
+	$(MAKE) -C docs clean
+	$(MAKE) -C docs html
+	$(BROWSER) docs/_build/html/index.html
+
+servedocs: docs ## compile the docs watching for changes
+	watchmedo shell-command -p '*.rst' -c '$(MAKE) -C docs html' -R -D .
+
+release: dist ## package and upload a release
+	twine upload dist/*
+
+dist: clean ## builds source and wheel package
+	python -m build
+	ls -l dist
+
+install: clean ## install the package to the active Python's site-packages
+	python setup.py install
```

### Comparing `hydrobot-0.5.0/PKG-INFO` & `hydrobot-0.5.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,143 +1,155 @@
-Metadata-Version: 2.1
-Name: hydrobot
-Version: 0.5.0
-Summary: A suite of processing tools for Hilltop hydrological data.
-Author-email: Nic Mostert <nicolas.mostert@horizons.govt.nz>, Sam Irvine <sam.irvine@horizons.govt.nz>
-License: GNU General Public License v3
-Project-URL: Homepage, https://github.com/HorizonsRC/hydrobot
-Project-URL: Issues, https://github.com/HorizonsRC/hydrobot/issues
-Project-URL: Documentation, https://hydrobot.readthedocs.io
-Project-URL: Package, https://pypi.org/project/hydrobot
-Keywords: hydrology, automation, pandas, hilltop, hilltop-py, HorizonsRC
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: ==3.11.*
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-License-File: AUTHORS.rst
-Requires-Dist: hilltop-py>=2.3.1
-Requires-Dist: data-annalist>=0.4.1
-Requires-Dist: matplotlib>=3.8.0
-Requires-Dist: defusedxml>=0.7.1
-Requires-Dist: plotly>=5.20.0
-Provides-Extra: test
-Requires-Dist: pytest>=7.4.2; extra == "test"
-Requires-Dist: pytest-cov>=4.1.0; extra == "test"
-Requires-Dist: pytest-dependency>=0.5.1; extra == "test"
-Requires-Dist: pytest-mock>=3.12.0; extra == "test"
-Provides-Extra: dev
-Requires-Dist: ruff>=0.1.6; extra == "dev"
-Requires-Dist: ruff-lsp>=0.0.45; extra == "dev"
-Requires-Dist: pre-commit>=3.5.0; extra == "dev"
-Requires-Dist: build>=1.0.0; extra == "dev"
-Provides-Extra: docs
-Requires-Dist: Sphinx>=7.2.6; extra == "docs"
-Requires-Dist: furo>=2023.9.10; extra == "docs"
-Provides-Extra: all
-Requires-Dist: hydrobot[dev,docs,test]; extra == "all"
-
-======================
-Hydrobot
-======================
-
-
-.. image:: https://img.shields.io/pypi/v/hydrobot.svg
-        :target: https://pypi.python.org/pypi/hydrobot
-
-.. image:: https://readthedocs.org/projects/hydrobot/badge/?version=latest
-        :target: https://hydrobot.readthedocs.io/en/latest/?version=latest
-        :alt: Documentation Status
-
-Python Package providing a suite of processing tools and utilities for Hilltop hydrological data.
-
-
-* Free software: GNU General Public License v3
-* Documentation: https://hydrobot.readthedocs.io.
-
-
-Features
---------
-
-* Processes data downloaded from Hilltop Server
-* Uses annalist to record all changes to data
-* Capable of various automated processing techniques, including:
-
-  * Clipping data
-  * Removing spikes based on FBEWMA smoothing
-  * Identifying and removing 'flatlining' data, where an instrument repeats it's last collected data point (NOTE: It's unclear if this actually happening.)
-  * Identifying gaps and gap lengths and closing small gaps
-  * Aggregating check data from various sources.
-  * Quality coding data based on NEMS standards
-
-* Plotting data, including:
-
-  * Processed data with quality codes
-  * Comparing raw data to processed data
-  * Showing all changes to the data
-  * Visualizing check points from various sources.
-
-Usage (Alpha)
--------------
-
-The Alpha release of Hydrobot supports a "hybrid" workflow. This means that some external tools are still required to do a full processing. Importantly, the hybrid workflow relies on some R scripts to obtain check data from sources other than Hilltop. Further processing using Hilltop manager is also supported.
-
-NOTE: Hydrobot 0.5.0 supports only Water Temperature processing at the moment, but more measurements will be supported in patches as the processing progresses.
-
-Initial Setup (Repeat for each release)
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-#. Install a Python 3.11 interpreter. Note that 3.12 is not supported just yet.
-#. In your favourite shell, create a new virtual environment using this python interpreter and name it "hydrobot0.5.0". It's important that this is stored somewhere locally. I suggest creating a folder for virtual environments in your home folder::
-
-    python -m venv path/to/venv/hydrobot0.5.0/
-
-#. Activate this virtual environment. In powershell this should be something like::
-
-    ./path/to/venv/hydrobot0.5.0/Scripts/Activate.ps1
-
-#. If you're sure your venv is active (ensure with `which python` and confirm that you're using the interpreter in your venv folder), install the latest version of Hydrobot using pip::
-
-    pip install hydrobot
-
-#. Navigate to the processing folder that you create as part of the Processing Steps below::
-
-    cd //ares/hydro/processing/whatever/watertemp/site/30X/
-
-
-Processing Steps
-^^^^^^^^^^^^^^^^
-
-#. Open Logsheet Loader. Fill it as normal, and note the start date of your processing period (i.e. end date of the previous period).
-#. Navigate to the data source and site folder, and create your processing folder.
-#. Copy all the processing files in this folder into your processing folder::
-
-    \\ares\Environmental Data Validation\Water Temperature\Documents\Hydrobot_0.5.0_Files\
-
-    //ares/Environmental\ Data\ Validation/Water\ Temperature/Documents/Hydrobot_0.5.0_Files/
-
-#. In your processing folder, open the `config.yaml` file and change the fields `site`, `from_date`, `to_date`, `analyst_name`. Feel free to mess with the other values once you get the hang of it. No one will die.
-
-#. Run the R script. I'm not an R guy so I'm not sure how to do this other than to open it in R studio, highlighting all the code, and hitting `Ctrl+Enter`. This should create a bunch of `.csv` files containing the check data from various sources. This is a good reasource for perusal during processing, but will be imbibed by hydrobot to for QC encoding.
-
-#. Make sure your virtual environment is set up and active. Ensure with `which python` and confirm that your python interpreter is running from your venv folder.
-
-#. Run the hydrobot processing script::
-
-    python processing_script.py
-
-#. If all goes well, the processing script will open a browser tab showing a diagnostic dash for your site. Use this to identify issues in the site.
-
-#. Use your python skills to solve some issues, like removing erroneous check data points or deleting chunks of data. More extensive documentation on actually using hydrobot will follow in future releases.
-
-#. Happy processing!
-
-Credits
--------
-
-This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template. Furthermore, Sam is a real champ with the coding and whatnot. Thanks Sam.
-
-.. _Cookiecutter: https://github.com/audreyr/cookiecutter
-.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
+Metadata-Version: 2.1
+Name: hydrobot
+Version: 0.5.1
+Summary: A suite of processing tools for Hilltop hydrological data.
+Author-email: Nic Mostert <nicolas.mostert@horizons.govt.nz>, Sam Irvine <sam.irvine@horizons.govt.nz>
+License: GNU General Public License v3
+Project-URL: Homepage, https://github.com/HorizonsRC/hydrobot
+Project-URL: Issues, https://github.com/HorizonsRC/hydrobot/issues
+Project-URL: Documentation, https://hydrobot.readthedocs.io
+Project-URL: Package, https://pypi.org/project/hydrobot
+Keywords: hydrology, automation, pandas, hilltop, hilltop-py, HorizonsRC
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: ==3.11.*
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+License-File: AUTHORS.rst
+Requires-Dist: hilltop-py>=2.3.1
+Requires-Dist: data-annalist>=0.4.1
+Requires-Dist: matplotlib>=3.8.0
+Requires-Dist: defusedxml>=0.7.1
+Requires-Dist: plotly>=5.20.0
+Provides-Extra: test
+Requires-Dist: pytest>=7.4.2; extra == "test"
+Requires-Dist: pytest-cov>=4.1.0; extra == "test"
+Requires-Dist: pytest-dependency>=0.5.1; extra == "test"
+Requires-Dist: pytest-mock>=3.12.0; extra == "test"
+Provides-Extra: dev
+Requires-Dist: ruff>=0.1.6; extra == "dev"
+Requires-Dist: ruff-lsp>=0.0.45; extra == "dev"
+Requires-Dist: pre-commit>=3.5.0; extra == "dev"
+Requires-Dist: build>=1.0.0; extra == "dev"
+Provides-Extra: docs
+Requires-Dist: Sphinx>=7.2.6; extra == "docs"
+Requires-Dist: furo>=2023.9.10; extra == "docs"
+Provides-Extra: all
+Requires-Dist: hydrobot[dev,docs,test]; extra == "all"
+
+======================
+Hydrobot
+======================
+
+
+.. image:: https://img.shields.io/pypi/v/hydrobot.svg
+        :target: https://pypi.python.org/pypi/hydrobot
+
+.. image:: https://readthedocs.org/projects/hydrobot/badge/?version=latest
+        :target: https://hydrobot.readthedocs.io/en/latest/?version=latest
+        :alt: Documentation Status
+
+Python Package providing a suite of processing tools and utilities for Hilltop hydrological data.
+
+
+* Free software: GNU General Public License v3
+* Documentation: https://hydrobot.readthedocs.io.
+
+
+Features
+--------
+
+* Processes data downloaded from Hilltop Server
+* Uses annalist to record all changes to data
+* Capable of various automated processing techniques, including:
+
+  * Clipping data
+  * Removing spikes based on FBEWMA smoothing
+  * Identifying and removing 'flatlining' data, where an instrument repeats it's last collected data point (NOTE: It's unclear if this actually happening.)
+  * Identifying gaps and gap lengths and closing small gaps
+  * Aggregating check data from various sources.
+  * Quality coding data based on NEMS standards
+
+* Plotting data, including:
+
+  * Processed data with quality codes
+  * Comparing raw data to processed data
+  * Showing all changes to the data
+  * Visualizing check points from various sources.
+
+Usage (Alpha)
+-------------
+
+The Alpha release of Hydrobot supports a "hybrid" workflow. This means that some external tools are still required to do a full processing. Importantly, the hybrid workflow relies on some R scripts to obtain check data from sources other than Hilltop. Further processing using Hilltop manager is also supported.
+
+NOTE: Hydrobot 0.5.0 supports only Water Temperature processing at the moment, but more measurements will be supported in patches as the processing progresses.
+
+Initial Setup (Repeat for each release)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+#. Install a Python 3.11 interpreter. Note that 3.12 is not supported just yet.
+#. In your favourite shell, create a new virtual environment using this python interpreter and name it "hydrobot0.5.0". It's important that this is stored somewhere locally. I suggest creating a folder for virtual environments in your home folder::
+
+    python -m venv path/to/venv/hydrobot0.5.0/
+
+#. Activate this virtual environment. In powershell this should be something like::
+
+    ./path/to/venv/hydrobot0.5.0/Scripts/Activate.ps1
+
+#. If you're sure your venv is active (ensure with `which python` and confirm that you're using the interpreter in your venv folder), install the latest version of Hydrobot using pip::
+
+    pip install hydrobot
+
+#. Record which version of dependencies you have installed. The following pip freeze records which dependencies are
+installed by the hydrobot install process for if auditing/reprocessing is required later::
+
+    pip freeze > dependencies.txt
+
+#. Navigate to the processing folder that you create as part of the Processing Steps below::
+
+    cd //ares/hydro/processing/whatever/watertemp/site/30X/
+
+
+Processing Steps
+^^^^^^^^^^^^^^^^
+
+#. Open Logsheet Loader. Fill it as normal, and note the start date of your processing period (i.e. end date of the previous period).
+#. Navigate to the data source and site folder, and create your processing folder.
+#. Copy all the processing files in this folder into your processing folder::
+
+    \\ares\Environmental Data Validation\Water Temperature\Documents\Hydrobot_0.5.0_Files\
+
+    //ares/Environmental\ Data\ Validation/Water\ Temperature/Documents/Hydrobot_0.5.0_Files/
+
+#. In your processing folder, open the `config.yaml` file and change the fields `site`, `from_date`, `to_date`, `analyst_name`. Feel free to mess with the other values once you get the hang of it. No one will die.
+
+#. Run the R script. I'm not an R guy so I'm not sure how to do this other than to open it in R studio, highlighting all the code, and hitting `Ctrl+Enter`. This should create a bunch of `.csv` files containing the check data from various sources. This is a good reasource for perusal during processing, but will be imbibed by hydrobot to for QC encoding.
+
+#. Make sure your virtual environment is set up and active. Ensure with `which python` and confirm that your python interpreter is running from your venv folder.
+
+#. Run the hydrobot processing script::
+
+    python processing_script.py
+
+#. If all goes well, the processing script will open a browser tab showing a diagnostic dash for your site. Use this to identify issues in the site.
+
+#. Use your python skills to solve some issues, like removing erroneous check data points or deleting chunks of data. More extensive documentation on actually using hydrobot will follow in future releases.
+
+#. Open the resulting processed.xml in manager, and copy it over to a hts file.
+
+#. Open the WaterTemp_check_data.csv outputed from the R file in a spreadsheet (sorry) and copy into hts file.
+
+#. Happy processing!
+
+Credits
+-------
+
+This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template. Furthermore,
+Sam is a real champ with the coding and whatnot. Thanks Sam.
+
+Aww thanks Nic. You also da man <3
+
+.. _Cookiecutter: https://github.com/audreyr/cookiecutter
+.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
```

### Comparing `hydrobot-0.5.0/README.rst` & `hydrobot-0.5.1/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,102 +1,114 @@
-======================
-Hydrobot
-======================
-
-
-.. image:: https://img.shields.io/pypi/v/hydrobot.svg
-        :target: https://pypi.python.org/pypi/hydrobot
-
-.. image:: https://readthedocs.org/projects/hydrobot/badge/?version=latest
-        :target: https://hydrobot.readthedocs.io/en/latest/?version=latest
-        :alt: Documentation Status
-
-Python Package providing a suite of processing tools and utilities for Hilltop hydrological data.
-
-
-* Free software: GNU General Public License v3
-* Documentation: https://hydrobot.readthedocs.io.
-
-
-Features
---------
-
-* Processes data downloaded from Hilltop Server
-* Uses annalist to record all changes to data
-* Capable of various automated processing techniques, including:
-
-  * Clipping data
-  * Removing spikes based on FBEWMA smoothing
-  * Identifying and removing 'flatlining' data, where an instrument repeats it's last collected data point (NOTE: It's unclear if this actually happening.)
-  * Identifying gaps and gap lengths and closing small gaps
-  * Aggregating check data from various sources.
-  * Quality coding data based on NEMS standards
-
-* Plotting data, including:
-
-  * Processed data with quality codes
-  * Comparing raw data to processed data
-  * Showing all changes to the data
-  * Visualizing check points from various sources.
-
-Usage (Alpha)
--------------
-
-The Alpha release of Hydrobot supports a "hybrid" workflow. This means that some external tools are still required to do a full processing. Importantly, the hybrid workflow relies on some R scripts to obtain check data from sources other than Hilltop. Further processing using Hilltop manager is also supported.
-
-NOTE: Hydrobot 0.5.0 supports only Water Temperature processing at the moment, but more measurements will be supported in patches as the processing progresses.
-
-Initial Setup (Repeat for each release)
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-#. Install a Python 3.11 interpreter. Note that 3.12 is not supported just yet.
-#. In your favourite shell, create a new virtual environment using this python interpreter and name it "hydrobot0.5.0". It's important that this is stored somewhere locally. I suggest creating a folder for virtual environments in your home folder::
-
-    python -m venv path/to/venv/hydrobot0.5.0/
-
-#. Activate this virtual environment. In powershell this should be something like::
-
-    ./path/to/venv/hydrobot0.5.0/Scripts/Activate.ps1
-
-#. If you're sure your venv is active (ensure with `which python` and confirm that you're using the interpreter in your venv folder), install the latest version of Hydrobot using pip::
-
-    pip install hydrobot
-
-#. Navigate to the processing folder that you create as part of the Processing Steps below::
-
-    cd //ares/hydro/processing/whatever/watertemp/site/30X/
-
-
-Processing Steps
-^^^^^^^^^^^^^^^^
-
-#. Open Logsheet Loader. Fill it as normal, and note the start date of your processing period (i.e. end date of the previous period).
-#. Navigate to the data source and site folder, and create your processing folder.
-#. Copy all the processing files in this folder into your processing folder::
-
-    \\ares\Environmental Data Validation\Water Temperature\Documents\Hydrobot_0.5.0_Files\
-
-    //ares/Environmental\ Data\ Validation/Water\ Temperature/Documents/Hydrobot_0.5.0_Files/
-
-#. In your processing folder, open the `config.yaml` file and change the fields `site`, `from_date`, `to_date`, `analyst_name`. Feel free to mess with the other values once you get the hang of it. No one will die.
-
-#. Run the R script. I'm not an R guy so I'm not sure how to do this other than to open it in R studio, highlighting all the code, and hitting `Ctrl+Enter`. This should create a bunch of `.csv` files containing the check data from various sources. This is a good reasource for perusal during processing, but will be imbibed by hydrobot to for QC encoding.
-
-#. Make sure your virtual environment is set up and active. Ensure with `which python` and confirm that your python interpreter is running from your venv folder.
-
-#. Run the hydrobot processing script::
-
-    python processing_script.py
-
-#. If all goes well, the processing script will open a browser tab showing a diagnostic dash for your site. Use this to identify issues in the site.
-
-#. Use your python skills to solve some issues, like removing erroneous check data points or deleting chunks of data. More extensive documentation on actually using hydrobot will follow in future releases.
-
-#. Happy processing!
-
-Credits
--------
-
-This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template. Furthermore, Sam is a real champ with the coding and whatnot. Thanks Sam.
-
-.. _Cookiecutter: https://github.com/audreyr/cookiecutter
-.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
+======================
+Hydrobot
+======================
+
+
+.. image:: https://img.shields.io/pypi/v/hydrobot.svg
+        :target: https://pypi.python.org/pypi/hydrobot
+
+.. image:: https://readthedocs.org/projects/hydrobot/badge/?version=latest
+        :target: https://hydrobot.readthedocs.io/en/latest/?version=latest
+        :alt: Documentation Status
+
+Python Package providing a suite of processing tools and utilities for Hilltop hydrological data.
+
+
+* Free software: GNU General Public License v3
+* Documentation: https://hydrobot.readthedocs.io.
+
+
+Features
+--------
+
+* Processes data downloaded from Hilltop Server
+* Uses annalist to record all changes to data
+* Capable of various automated processing techniques, including:
+
+  * Clipping data
+  * Removing spikes based on FBEWMA smoothing
+  * Identifying and removing 'flatlining' data, where an instrument repeats it's last collected data point (NOTE: It's unclear if this actually happening.)
+  * Identifying gaps and gap lengths and closing small gaps
+  * Aggregating check data from various sources.
+  * Quality coding data based on NEMS standards
+
+* Plotting data, including:
+
+  * Processed data with quality codes
+  * Comparing raw data to processed data
+  * Showing all changes to the data
+  * Visualizing check points from various sources.
+
+Usage (Alpha)
+-------------
+
+The Alpha release of Hydrobot supports a "hybrid" workflow. This means that some external tools are still required to do a full processing. Importantly, the hybrid workflow relies on some R scripts to obtain check data from sources other than Hilltop. Further processing using Hilltop manager is also supported.
+
+NOTE: Hydrobot 0.5.0 supports only Water Temperature processing at the moment, but more measurements will be supported in patches as the processing progresses.
+
+Initial Setup (Repeat for each release)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+#. Install a Python 3.11 interpreter. Note that 3.12 is not supported just yet.
+#. In your favourite shell, create a new virtual environment using this python interpreter and name it "hydrobot0.5.0". It's important that this is stored somewhere locally. I suggest creating a folder for virtual environments in your home folder::
+
+    python -m venv path/to/venv/hydrobot0.5.0/
+
+#. Activate this virtual environment. In powershell this should be something like::
+
+    ./path/to/venv/hydrobot0.5.0/Scripts/Activate.ps1
+
+#. If you're sure your venv is active (ensure with `which python` and confirm that you're using the interpreter in your venv folder), install the latest version of Hydrobot using pip::
+
+    pip install hydrobot
+
+#. Record which version of dependencies you have installed. The following pip freeze records which dependencies are
+installed by the hydrobot install process for if auditing/reprocessing is required later::
+
+    pip freeze > dependencies.txt
+
+#. Navigate to the processing folder that you create as part of the Processing Steps below::
+
+    cd //ares/hydro/processing/whatever/watertemp/site/30X/
+
+
+Processing Steps
+^^^^^^^^^^^^^^^^
+
+#. Open Logsheet Loader. Fill it as normal, and note the start date of your processing period (i.e. end date of the previous period).
+#. Navigate to the data source and site folder, and create your processing folder.
+#. Copy all the processing files in this folder into your processing folder::
+
+    \\ares\Environmental Data Validation\Water Temperature\Documents\Hydrobot_0.5.0_Files\
+
+    //ares/Environmental\ Data\ Validation/Water\ Temperature/Documents/Hydrobot_0.5.0_Files/
+
+#. In your processing folder, open the `config.yaml` file and change the fields `site`, `from_date`, `to_date`, `analyst_name`. Feel free to mess with the other values once you get the hang of it. No one will die.
+
+#. Run the R script. I'm not an R guy so I'm not sure how to do this other than to open it in R studio, highlighting all the code, and hitting `Ctrl+Enter`. This should create a bunch of `.csv` files containing the check data from various sources. This is a good reasource for perusal during processing, but will be imbibed by hydrobot to for QC encoding.
+
+#. Make sure your virtual environment is set up and active. Ensure with `which python` and confirm that your python interpreter is running from your venv folder.
+
+#. Run the hydrobot processing script::
+
+    python processing_script.py
+
+#. If all goes well, the processing script will open a browser tab showing a diagnostic dash for your site. Use this to identify issues in the site.
+
+#. Use your python skills to solve some issues, like removing erroneous check data points or deleting chunks of data. More extensive documentation on actually using hydrobot will follow in future releases.
+
+#. Open the resulting processed.xml in manager, and copy it over to a hts file.
+
+#. Open the WaterTemp_check_data.csv outputed from the R file in a spreadsheet (sorry) and copy into hts file.
+
+#. Happy processing!
+
+Credits
+-------
+
+This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template. Furthermore,
+Sam is a real champ with the coding and whatnot. Thanks Sam.
+
+Aww thanks Nic. You also da man <3
+
+.. _Cookiecutter: https://github.com/audreyr/cookiecutter
+.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
```

### Comparing `hydrobot-0.5.0/docs/conf.py` & `hydrobot-0.5.1/docs/conf.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,179 +1,179 @@
-#!/usr/bin/env python
-
-"""Configuration for Sphinx docs."""
-#
-# hydrobot documentation build configuration file, created by
-# sphinx-quickstart on Fri Jun  9 13:47:02 2017.
-#
-# This file is execfile()d with the current directory set to its
-# containing dir.
-#
-# Note that not all possible configuration values are present in this
-# autogenerated file.
-#
-# All configuration values have a default; values that are commented out
-# serve to show the default.
-
-# If extensions (or modules to document with autodoc) are in another
-# directory, add these directories to sys.path here. If the directory is
-# relative to the documentation root, use os.path.abspath to make it
-# absolute, like shown here.
-#
-import os
-import sys
-
-sys.path.insert(0, os.path.abspath(".."))
-
-import hydrobot
-
-
-# -- General configuration ---------------------------------------------
-
-# If your documentation needs a minimal Sphinx version, state it here.
-#
-# needs_sphinx = '1.0'
-
-# Add any Sphinx extension module names here, as strings. They can be
-# extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = [
-    "sphinx.ext.autodoc",
-    "sphinx.ext.viewcode",
-    "sphinx.ext.autosectionlabel",
-    "sphinx.ext.autosummary",
-    "sphinx.ext.coverage",
-    "sphinx.ext.napoleon",
-    "sphinx.ext.todo",
-]
-
-# Add any paths that contain templates here, relative to this directory.
-templates_path = ["_templates"]
-
-# The suffix(es) of source filenames.
-# You can specify multiple suffix as a list of string:
-#
-# source_suffix = ['.rst', '.md']
-source_suffix = ".rst"
-
-# The master toctree document.
-master_doc = "index"
-
-# General information about the project.
-project = "Hydrobot"
-copyright = "2023, Nic Mostert"
-author = "Nic Mostert"
-
-# The version info for the project you're documenting, acts as replacement
-# for |version| and |release|, also used in various other places throughout
-# the built documents.
-#
-# The short X.Y version.
-version = hydrobot.__version__
-# The full version, including alpha/beta/rc tags.
-release = hydrobot.__version__
-
-# The language for content autogenerated by Sphinx. Refer to documentation
-# for a list of supported languages.
-#
-# This is also used if you do content translation via gettext catalogs.
-# Usually you set "language" from the command line for these cases.
-language = "en"
-
-# List of patterns, relative to source directory, that match files and
-# directories to ignore when looking for source files.
-# This patterns also effect to html_static_path and html_extra_path
-exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
-
-# The name of the Pygments (syntax highlighting) style to use.
-pygments_style = "sphinx"
-
-# If true, `todo` and `todoList` produce output, else they produce nothing.
-todo_include_todos = False
-
-
-# -- Options for HTML output -------------------------------------------
-
-# The theme to use for HTML and HTML Help pages.  See the documentation for
-# a list of builtin themes.
-#
-html_theme = "furo"
-
-# Theme options are theme-specific and customize the look and feel of a
-# theme further.  For a list of options available for each theme, see the
-# documentation.
-#
-# html_theme_options = {}
-
-# Add any paths that contain custom static files (such as style sheets) here,
-# relative to this directory. They are copied after the builtin static files,
-# so a file named "default.css" will overwrite the builtin "default.css".
-# html_static_path = ["_static"]
-
-
-# -- Options for HTMLHelp output ---------------------------------------
-
-# Output file base name for HTML help builder.
-htmlhelp_basename = "hydrobotdoc"
-
-
-# -- Options for LaTeX output ------------------------------------------
-
-latex_elements = {
-    # The paper size ('letterpaper' or 'a4paper').
-    #
-    # 'papersize': 'letterpaper',
-    # The font size ('10pt', '11pt' or '12pt').
-    #
-    # 'pointsize': '10pt',
-    # Additional stuff for the LaTeX preamble.
-    #
-    # 'preamble': '',
-    # Latex figure (float) alignment
-    #
-    # 'figure_align': 'htbp',
-}
-
-# Grouping the document tree into LaTeX files. List of tuples
-# (source start file, target name, title, author, documentclass
-# [howto, manual, or own class]).
-latex_documents = [
-    (
-        master_doc,
-        "hydrobot.tex",
-        "Hydrobot Documentation",
-        "Nic Mostert",
-        "manual",
-    ),
-]
-
-
-# -- Options for manual page output ------------------------------------
-
-# One entry per manual page. List of tuples
-# (source start file, name, description, authors, manual section).
-man_pages = [
-    (
-        master_doc,
-        "hydrobot",
-        "Hydrobot Documentation",
-        [author],
-        1,
-    )
-]
-
-
-# -- Options for Texinfo output ----------------------------------------
-
-# Grouping the document tree into Texinfo files. List of tuples
-# (source start file, target name, title, author,
-#  dir menu entry, description, category)
-texinfo_documents = [
-    (
-        master_doc,
-        "hydrobot",
-        "Hydrobot Documentation",
-        author,
-        "hydrobot",
-        "Hydrological Data Processing Suite.",
-        "Miscellaneous",
-    ),
-]
+#!/usr/bin/env python
+
+"""Configuration for Sphinx docs."""
+#
+# hydrobot documentation build configuration file, created by
+# sphinx-quickstart on Fri Jun  9 13:47:02 2017.
+#
+# This file is execfile()d with the current directory set to its
+# containing dir.
+#
+# Note that not all possible configuration values are present in this
+# autogenerated file.
+#
+# All configuration values have a default; values that are commented out
+# serve to show the default.
+
+# If extensions (or modules to document with autodoc) are in another
+# directory, add these directories to sys.path here. If the directory is
+# relative to the documentation root, use os.path.abspath to make it
+# absolute, like shown here.
+#
+import os
+import sys
+
+sys.path.insert(0, os.path.abspath(".."))
+
+import hydrobot
+
+
+# -- General configuration ---------------------------------------------
+
+# If your documentation needs a minimal Sphinx version, state it here.
+#
+# needs_sphinx = '1.0'
+
+# Add any Sphinx extension module names here, as strings. They can be
+# extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
+extensions = [
+    "sphinx.ext.autodoc",
+    "sphinx.ext.viewcode",
+    "sphinx.ext.autosectionlabel",
+    "sphinx.ext.autosummary",
+    "sphinx.ext.coverage",
+    "sphinx.ext.napoleon",
+    "sphinx.ext.todo",
+]
+
+# Add any paths that contain templates here, relative to this directory.
+templates_path = ["_templates"]
+
+# The suffix(es) of source filenames.
+# You can specify multiple suffix as a list of string:
+#
+# source_suffix = ['.rst', '.md']
+source_suffix = ".rst"
+
+# The master toctree document.
+master_doc = "index"
+
+# General information about the project.
+project = "Hydrobot"
+copyright = "2023, Nic Mostert"
+author = "Nic Mostert"
+
+# The version info for the project you're documenting, acts as replacement
+# for |version| and |release|, also used in various other places throughout
+# the built documents.
+#
+# The short X.Y version.
+version = hydrobot.__version__
+# The full version, including alpha/beta/rc tags.
+release = hydrobot.__version__
+
+# The language for content autogenerated by Sphinx. Refer to documentation
+# for a list of supported languages.
+#
+# This is also used if you do content translation via gettext catalogs.
+# Usually you set "language" from the command line for these cases.
+language = "en"
+
+# List of patterns, relative to source directory, that match files and
+# directories to ignore when looking for source files.
+# This patterns also effect to html_static_path and html_extra_path
+exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
+
+# The name of the Pygments (syntax highlighting) style to use.
+pygments_style = "sphinx"
+
+# If true, `todo` and `todoList` produce output, else they produce nothing.
+todo_include_todos = False
+
+
+# -- Options for HTML output -------------------------------------------
+
+# The theme to use for HTML and HTML Help pages.  See the documentation for
+# a list of builtin themes.
+#
+html_theme = "furo"
+
+# Theme options are theme-specific and customize the look and feel of a
+# theme further.  For a list of options available for each theme, see the
+# documentation.
+#
+# html_theme_options = {}
+
+# Add any paths that contain custom static files (such as style sheets) here,
+# relative to this directory. They are copied after the builtin static files,
+# so a file named "default.css" will overwrite the builtin "default.css".
+# html_static_path = ["_static"]
+
+
+# -- Options for HTMLHelp output ---------------------------------------
+
+# Output file base name for HTML help builder.
+htmlhelp_basename = "hydrobotdoc"
+
+
+# -- Options for LaTeX output ------------------------------------------
+
+latex_elements = {
+    # The paper size ('letterpaper' or 'a4paper').
+    #
+    # 'papersize': 'letterpaper',
+    # The font size ('10pt', '11pt' or '12pt').
+    #
+    # 'pointsize': '10pt',
+    # Additional stuff for the LaTeX preamble.
+    #
+    # 'preamble': '',
+    # Latex figure (float) alignment
+    #
+    # 'figure_align': 'htbp',
+}
+
+# Grouping the document tree into LaTeX files. List of tuples
+# (source start file, target name, title, author, documentclass
+# [howto, manual, or own class]).
+latex_documents = [
+    (
+        master_doc,
+        "hydrobot.tex",
+        "Hydrobot Documentation",
+        "Nic Mostert",
+        "manual",
+    ),
+]
+
+
+# -- Options for manual page output ------------------------------------
+
+# One entry per manual page. List of tuples
+# (source start file, name, description, authors, manual section).
+man_pages = [
+    (
+        master_doc,
+        "hydrobot",
+        "Hydrobot Documentation",
+        [author],
+        1,
+    )
+]
+
+
+# -- Options for Texinfo output ----------------------------------------
+
+# Grouping the document tree into Texinfo files. List of tuples
+# (source start file, target name, title, author,
+#  dir menu entry, description, category)
+texinfo_documents = [
+    (
+        master_doc,
+        "hydrobot",
+        "Hydrobot Documentation",
+        author,
+        "hydrobot",
+        "Hydrological Data Processing Suite.",
+        "Miscellaneous",
+    ),
+]
```

### Comparing `hydrobot-0.5.0/docs/installation.rst` & `hydrobot-0.5.1/docs/installation.rst`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-.. highlight:: shell
-
-============
-Installation
-============
-
-
-Stable release
---------------
-
-To install Hydrobot, run this command in your terminal:
-
-.. code-block:: console
-
-    $ pip install hydrobot
-
-This is the preferred method to install Hydrobot, as it will always install the most recent stable release.
-
-If you don't have `pip`_ installed, this `Python installation guide`_ can guide
-you through the process.
-
-.. _pip: https://pip.pypa.io
-.. _Python installation guide: http://docs.python-guide.org/en/latest/starting/installation/
-
-
-From sources
-------------
-
-The sources for Hydrobot can be downloaded from the `Github repo`_.
-
-You can either clone the public repository:
-
-.. code-block:: console
-
-    $ git clone git://github.com/nicmostert/hydrobot
-
-Or download the `tarball`_:
-
-.. code-block:: console
-
-    $ curl -OJL https://github.com/nicmostert/hydrobot/tarball/master
-
-Once you have a copy of the source, you can install it with:
-
-.. code-block:: console
-
-    $ python setup.py install
-
-
-.. _Github repo: https://github.com/nicmostert/hydrobot
-.. _tarball: https://github.com/nicmostert/hydrobot/tarball/master
-
-
-Usage
------
-
-For purposes of auditing data changes, you may want to track what changes to
-the data are made, and what version of hydrobot (and it's dependencies) are
-used.
-
-    Windows
-
-In Powershell:
-
-.. code-block:: console
-
-    cd path/to/Hydrobot_install
-    python -m venv /path/to/Hydrobot_install/venv
-    path/to/Hydrobot_install/venv/Scripts/Activate.ps1
-    pip install hydrobot
-    pip freeze > requirements.txt
+.. highlight:: shell
+
+============
+Installation
+============
+
+
+Stable release
+--------------
+
+To install Hydrobot, run this command in your terminal:
+
+.. code-block:: console
+
+    $ pip install hydrobot
+
+This is the preferred method to install Hydrobot, as it will always install the most recent stable release.
+
+If you don't have `pip`_ installed, this `Python installation guide`_ can guide
+you through the process.
+
+.. _pip: https://pip.pypa.io
+.. _Python installation guide: http://docs.python-guide.org/en/latest/starting/installation/
+
+
+From sources
+------------
+
+The sources for Hydrobot can be downloaded from the `Github repo`_.
+
+You can either clone the public repository:
+
+.. code-block:: console
+
+    $ git clone git://github.com/nicmostert/hydrobot
+
+Or download the `tarball`_:
+
+.. code-block:: console
+
+    $ curl -OJL https://github.com/nicmostert/hydrobot/tarball/master
+
+Once you have a copy of the source, you can install it with:
+
+.. code-block:: console
+
+    $ python setup.py install
+
+
+.. _Github repo: https://github.com/nicmostert/hydrobot
+.. _tarball: https://github.com/nicmostert/hydrobot/tarball/master
+
+
+Usage
+-----
+
+For purposes of auditing data changes, you may want to track what changes to
+the data are made, and what version of hydrobot (and it's dependencies) are
+used.
+
+    Windows
+
+In Powershell:
+
+.. code-block:: console
+
+    cd path/to/Hydrobot_install
+    python -m venv /path/to/Hydrobot_install/venv
+    path/to/Hydrobot_install/venv/Scripts/Activate.ps1
+    pip install hydrobot
+    pip freeze > requirements.txt
```

### Comparing `hydrobot-0.5.0/docs/make.bat` & `hydrobot-0.5.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hydrobot-0.5.0/hydrobot/data_acquisition.py` & `hydrobot-0.5.1/hydrobot/data_acquisition.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,216 +1,216 @@
-"""Main module."""
-
-from xml.etree import ElementTree
-
-import pandas as pd
-from annalist.annalist import Annalist
-from hilltoppy.utils import build_url, get_hilltop_xml
-
-from hydrobot.data_structure import parse_xml
-
-annalizer = Annalist()
-
-
-def get_data(
-    base_url,
-    hts,
-    site,
-    measurement,
-    from_date,
-    to_date,
-    tstype="Standard",
-):
-    """Acquire time series data from a web service and return it as a DataFrame.
-
-    Parameters
-    ----------
-    base_url : str
-        The base URL of the web service.
-    hts : str
-        The Hilltop Time Series (HTS) identifier.
-    site : str
-        The site name or location.
-    measurement : str
-        The type of measurement to retrieve.
-    from_date : str
-        The start date and time for data retrieval
-        in the format 'YYYY-MM-DD HH:mm'.
-    to_date : str
-        The end date and time for data retrieval
-        in the format 'YYYY-MM-DD HH:mm'.
-    tstype : str
-        Type of data that is sought
-        (default is Standard, can be Standard, Check, or Quality)
-
-    Returns
-    -------
-    pandas.DataFrame
-        A DataFrame containing the acquired time series data.
-    """
-    url = build_url(
-        base_url,
-        hts,
-        "GetData",
-        site=site,
-        measurement=measurement,
-        from_date=from_date,
-        to_date=to_date,
-        tstype=tstype,
-    )
-
-    hilltop_xml = get_hilltop_xml(url)
-
-    data_object = parse_xml(hilltop_xml)
-
-    return hilltop_xml, data_object
-
-
-def get_time_range(
-    base_url,
-    hts,
-    site,
-    measurement,
-    tstype="Standard",
-):
-    """Acquire time series data from a web service and return it as a DataFrame.
-
-    Parameters
-    ----------
-    base_url : str
-        The base URL of the web service.
-    hts : str
-        The Hilltop Time Series (HTS) identifier.
-    site : str
-        The site name or location.
-    measurement : str
-        The type of measurement to retrieve.
-    from_date : str
-        The start date and time for data retrieval
-        in the format 'YYYY-MM-DD HH:mm'.
-    to_date : str
-        The end date and time for data retrieval
-        in the format 'YYYY-MM-DD HH:mm'.
-    tstype : str
-        Type of data that is sought
-        (default is Standard, can be Standard, Check, or Quality)
-
-    Returns
-    -------
-    pandas.DataFrame
-        A DataFrame containing the acquired time series data.
-    """
-    url = build_url(
-        base_url,
-        hts,
-        "TimeRange",
-        site=site,
-        measurement=measurement,
-        tstype=tstype,
-    )
-
-    hilltop_xml = get_hilltop_xml(url)
-    print(url)
-
-    data_object = parse_xml(hilltop_xml)
-
-    return hilltop_xml, data_object
-
-
-def get_series(
-    base_url,
-    hts,
-    site,
-    measurement,
-    from_date,
-    to_date,
-    tstype="Standard",
-) -> tuple[ElementTree.Element, pd.Series | pd.DataFrame]:
-    """Pack data from get_data as a pd.Series.
-
-    Parameters
-    ----------
-    base_url : str
-        The base URL of the web service.
-    hts : str
-        The Hilltop Time Series (HTS) identifier.
-    site : str
-        The site name or location.
-    measurement : str
-        The type of measurement to retrieve.
-    from_date : str
-        The start date and time for data retrieval
-        in the format 'YYYY-MM-DD HH:mm'.
-    to_date : str
-        The end date and time for data retrieval
-        in the format 'YYYY-MM-DD HH:mm'.
-    tstype : str
-        Type of data that is sought
-        (default 'Standard', can be Standard, Check, or Quality)
-
-    Returns
-    -------
-    pandas.Series or pandas.DataFrame
-        A pd.Series containing the acquired time series data.
-    """
-    xml, data_object = get_data(
-        base_url,
-        hts,
-        site,
-        measurement,
-        from_date,
-        to_date,
-        tstype,
-    )
-    if data_object is not None:
-        data = data_object[0].data.timeseries
-        if not data.empty:
-            mowsecs_offset = 946771200
-            if data_object[0].data.date_format == "mowsecs":
-                timestamps = data.index.map(
-                    lambda x: pd.Timestamp(int(x) - mowsecs_offset, unit="s")
-                )
-                data.index = pd.to_datetime(timestamps)
-            else:
-                data.index = pd.to_datetime(data.index)
-    else:
-        data = pd.Series({})
-    return xml, data
-
-
-def import_inspections(filename):
-    """Import inspections as generated by R script."""
-    insp_df = pd.read_csv(filename)
-    if not insp_df.empty:
-        insp_df["Time"] = pd.to_datetime(insp_df["Date"] + " " + insp_df["Time"])
-        insp_df = insp_df.set_index("Time")
-        insp_df = insp_df.drop(columns=["Date"])
-        insp_df["Comment"] = insp_df.apply(
-            lambda x: f"{x['InspectionStaff']}: {x['Notes']}", axis=1
-        )
-    return insp_df
-
-
-def import_prov_wq(filename):
-    """Import prov_wq checks as obtained by R script."""
-    prov_df = pd.read_csv(filename)
-    if not prov_df.empty:
-        prov_df["Time"] = pd.to_datetime(prov_df["Date"] + " " + prov_df["Time"])
-        prov_df = prov_df.set_index("Time")
-        prov_df = prov_df.drop(columns=["Date"])
-        prov_df["Comment"] = prov_df.apply(
-            lambda x: f"{x['InspectionStaff']}: {x['Notes']}", axis=1
-        )
-    return prov_df
-
-
-def import_ncr(filename):
-    """Import non conformance data as obtained by R script."""
-    ncr_df = pd.read_csv(filename)
-    ncr_df = ncr_df.rename(columns={"Entrydate": "Time"})
-    ncr_df["Time"] = pd.to_datetime(ncr_df["Time"])
-    ncr_df["Comment"] = ncr_df.apply(
-        lambda x: f"{x['Reportby']}: {x['NC_Summary']}; {x['CorrectiveAction']}",
-        axis=1,
-    )
-    ncr_df = ncr_df.set_index("Time")
-    return ncr_df
+"""Main module."""
+
+from xml.etree import ElementTree
+
+import pandas as pd
+from annalist.annalist import Annalist
+from hilltoppy.utils import build_url, get_hilltop_xml
+
+from hydrobot.data_structure import parse_xml
+
+annalizer = Annalist()
+
+
+def get_data(
+    base_url,
+    hts,
+    site,
+    measurement,
+    from_date,
+    to_date,
+    tstype="Standard",
+):
+    """Acquire time series data from a web service and return it as a DataFrame.
+
+    Parameters
+    ----------
+    base_url : str
+        The base URL of the web service.
+    hts : str
+        The Hilltop Time Series (HTS) identifier.
+    site : str
+        The site name or location.
+    measurement : str
+        The type of measurement to retrieve.
+    from_date : str
+        The start date and time for data retrieval
+        in the format 'YYYY-MM-DD HH:mm'.
+    to_date : str
+        The end date and time for data retrieval
+        in the format 'YYYY-MM-DD HH:mm'.
+    tstype : str
+        Type of data that is sought
+        (default is Standard, can be Standard, Check, or Quality)
+
+    Returns
+    -------
+    pandas.DataFrame
+        A DataFrame containing the acquired time series data.
+    """
+    url = build_url(
+        base_url,
+        hts,
+        "GetData",
+        site=site,
+        measurement=measurement,
+        from_date=from_date,
+        to_date=to_date,
+        tstype=tstype,
+    )
+
+    hilltop_xml = get_hilltop_xml(url)
+
+    data_object = parse_xml(hilltop_xml)
+
+    return hilltop_xml, data_object
+
+
+def get_time_range(
+    base_url,
+    hts,
+    site,
+    measurement,
+    tstype="Standard",
+):
+    """Acquire time series data from a web service and return it as a DataFrame.
+
+    Parameters
+    ----------
+    base_url : str
+        The base URL of the web service.
+    hts : str
+        The Hilltop Time Series (HTS) identifier.
+    site : str
+        The site name or location.
+    measurement : str
+        The type of measurement to retrieve.
+    from_date : str
+        The start date and time for data retrieval
+        in the format 'YYYY-MM-DD HH:mm'.
+    to_date : str
+        The end date and time for data retrieval
+        in the format 'YYYY-MM-DD HH:mm'.
+    tstype : str
+        Type of data that is sought
+        (default is Standard, can be Standard, Check, or Quality)
+
+    Returns
+    -------
+    pandas.DataFrame
+        A DataFrame containing the acquired time series data.
+    """
+    url = build_url(
+        base_url,
+        hts,
+        "TimeRange",
+        site=site,
+        measurement=measurement,
+        tstype=tstype,
+    )
+
+    hilltop_xml = get_hilltop_xml(url)
+    print(url)
+
+    data_object = parse_xml(hilltop_xml)
+
+    return hilltop_xml, data_object
+
+
+def get_series(
+    base_url,
+    hts,
+    site,
+    measurement,
+    from_date,
+    to_date,
+    tstype="Standard",
+) -> tuple[ElementTree.Element, pd.Series | pd.DataFrame]:
+    """Pack data from get_data as a pd.Series.
+
+    Parameters
+    ----------
+    base_url : str
+        The base URL of the web service.
+    hts : str
+        The Hilltop Time Series (HTS) identifier.
+    site : str
+        The site name or location.
+    measurement : str
+        The type of measurement to retrieve.
+    from_date : str
+        The start date and time for data retrieval
+        in the format 'YYYY-MM-DD HH:mm'.
+    to_date : str
+        The end date and time for data retrieval
+        in the format 'YYYY-MM-DD HH:mm'.
+    tstype : str
+        Type of data that is sought
+        (default 'Standard', can be Standard, Check, or Quality)
+
+    Returns
+    -------
+    pandas.Series or pandas.DataFrame
+        A pd.Series containing the acquired time series data.
+    """
+    xml, data_object = get_data(
+        base_url,
+        hts,
+        site,
+        measurement,
+        from_date,
+        to_date,
+        tstype,
+    )
+    if data_object is not None:
+        data = data_object[0].data.timeseries
+        if not data.empty:
+            mowsecs_offset = 946771200
+            if data_object[0].data.date_format == "mowsecs":
+                timestamps = data.index.map(
+                    lambda x: pd.Timestamp(int(x) - mowsecs_offset, unit="s")
+                )
+                data.index = pd.to_datetime(timestamps)
+            else:
+                data.index = pd.to_datetime(data.index)
+    else:
+        data = pd.Series({})
+    return xml, data
+
+
+def import_inspections(filename):
+    """Import inspections as generated by R script."""
+    insp_df = pd.read_csv(filename)
+    if not insp_df.empty:
+        insp_df["Time"] = pd.to_datetime(insp_df["Date"] + " " + insp_df["Time"])
+        insp_df = insp_df.set_index("Time")
+        insp_df = insp_df.drop(columns=["Date"])
+        insp_df["Comment"] = insp_df.apply(
+            lambda x: f"{x['InspectionStaff']}: {x['Notes']}", axis=1
+        )
+    return insp_df
+
+
+def import_prov_wq(filename):
+    """Import prov_wq checks as obtained by R script."""
+    prov_df = pd.read_csv(filename)
+    if not prov_df.empty:
+        prov_df["Time"] = pd.to_datetime(prov_df["Date"] + " " + prov_df["Time"])
+        prov_df = prov_df.set_index("Time")
+        prov_df = prov_df.drop(columns=["Date"])
+        prov_df["Comment"] = prov_df.apply(
+            lambda x: f"{x['InspectionStaff']}: {x['Notes']}", axis=1
+        )
+    return prov_df
+
+
+def import_ncr(filename):
+    """Import non conformance data as obtained by R script."""
+    ncr_df = pd.read_csv(filename)
+    ncr_df = ncr_df.rename(columns={"Entrydate": "Time"})
+    ncr_df["Time"] = pd.to_datetime(ncr_df["Time"])
+    ncr_df["Comment"] = ncr_df.apply(
+        lambda x: f"{x['Reportby']}: {x['NC_Summary']}; {x['CorrectiveAction']}",
+        axis=1,
+    )
+    ncr_df = ncr_df.set_index("Time")
+    return ncr_df
```

### Comparing `hydrobot-0.5.0/hydrobot/data_sources.py` & `hydrobot-0.5.1/hydrobot/data_sources.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,286 +1,286 @@
-"""Handling for different types of data sources."""
-import csv
-from pathlib import Path
-
-import numpy as np
-import pandas as pd
-
-
-class QualityCodeEvaluator:
-    """Basic QualityCodeEvaluator only compares magnitude of differences."""
-
-    def __init__(self, qc_500_limit, qc_600_limit, name=""):
-        """Initialize QualityCodeEvaluator.
-
-        Parameters
-        ----------
-        qc_500_limit : numerical
-            Threshold between QC 400 and QC 500
-        qc_600_limit : numerical
-            Threshold between QC 500 and QC 600
-        name : str
-            Name of the data source
-        """
-        self.qc_500_limit = qc_500_limit
-        self.qc_600_limit = qc_600_limit
-        self.name = name
-
-    def __repr__(self):
-        """QualityCodeEvaluator representation."""
-        return repr(f"QualityCodeEvaluator '{self.name}'")
-
-    def find_qc(self, base_datum, check_datum):
-        """Find the base quality codes.
-
-        Parameters
-        ----------
-        base_datum : numerical
-            Closest continuum datum point to the check
-        check_datum : numerical
-            The check data to verify the continuous data
-
-        Returns
-        -------
-        int
-            The Quality code
-
-        """
-        diff = np.abs(base_datum - check_datum)
-        if diff < self.qc_600_limit:
-            qc = 600
-        elif diff < self.qc_500_limit:
-            qc = 500
-        else:
-            qc = 400
-        return qc
-
-
-class TwoLevelQualityCodeEvaluator(QualityCodeEvaluator):
-    """QualityCodeEvaluator for standards such as water level.
-
-    Fixed error up to given threshold, percentage error after that.
-    """
-
-    def __init__(
-        self,
-        qc_500_limit,
-        qc_600_limit,
-        qc_500_percent,
-        qc_600_percent,
-        limit_percent_threshold,
-        name="",
-    ):
-        """Initialize TwoLevelQualityCodeEvaluator.
-
-        Parameters
-        ----------
-        qc_500_limit : numerical
-            Threshold between QC 400 and QC 500 for linear portion
-        qc_600_limit : numerical
-            Threshold between QC 500 and QC 600 for linear portion
-        qc_500_percent : numerical
-            Threshold between QC 400 and QC 500 for percentage portion
-        qc_600_percent : numerical
-            Threshold between QC 500 and QC 600 for percentage portion
-        limit_percent_threshold
-            Value at which the evaluator transitions between linear and percentage
-            QC comparison
-        name : str
-            Name of the data source
-        """
-        QualityCodeEvaluator.__init__(self, qc_500_limit, qc_600_limit, name)
-        self.qc_500_percent = qc_500_percent
-        self.qc_600_percent = qc_600_percent
-        self.limit_percent_threshold = limit_percent_threshold
-
-    def find_qc(self, base_datum, check_datum):
-        """Find the base quality codes with two stages.
-
-        The two stages are: a flat and percentage QC threshold.
-
-        Parameters
-        ----------
-        base_datum : numerical
-            Closest continuum datum point to the check
-        check_datum : numerical
-            The check data to verify the continuous data
-
-        Returns
-        -------
-        int
-            The Quality code
-
-        """
-        if base_datum < self.limit_percent_threshold:
-            # flat qc check
-            diff = np.abs(base_datum - check_datum)
-            if diff < self.qc_600_limit:
-                qc = 600
-            elif diff < self.qc_500_limit:
-                qc = 500
-            else:
-                qc = 400
-        else:
-            # percent qc check
-            diff = np.abs(base_datum / check_datum - 1) * 100
-            if diff < self.qc_600_percent:
-                qc = 600
-            elif diff < self.qc_500_percent:
-                qc = 500
-            else:
-                qc = 400
-        return qc
-
-
-def get_qc_evaluator_dict():
-    """Return all qc_evaluators in a dictionary.
-
-    Returns
-    -------
-    dict of string-qc_evaluator pairs
-    """
-    qc_evaluator_dict = {}
-    script_dir = Path(__file__).parent
-    # script_dir = os.path.dirname(os.path.abspath(__file__))
-
-    # Plain QualityCodeEvaluators
-    template_path = (script_dir / "config/QualityCodeEvaluator_QC_config.csv").resolve()
-    with open(template_path) as csv_file:
-        reader = csv.reader(csv_file)
-
-        for row in reader:
-            qc_evaluator_dict[row[0]] = QualityCodeEvaluator(
-                float(row[1]), float(row[2]), row[0]
-            )
-        csv_file.close()
-
-    # Two stage QualityCodeEvaluators
-    template_path = (
-        script_dir / "config/TwoLevelQualityCodeEvaluator_QC_config.csv"
-    ).resolve()
-    with open(template_path) as csv_file:
-        reader = csv.reader(csv_file)
-
-        for row in reader:
-            qc_evaluator_dict[row[0]] = TwoLevelQualityCodeEvaluator(
-                float(row[1]),
-                float(row[2]),
-                float(row[3]),
-                float(row[4]),
-                float(row[5]),
-                row[0],
-            )
-        csv_file.close()
-    return qc_evaluator_dict
-
-
-def get_qc_evaluator(qc_evaluator_name):
-    """Return qc_evaluator that matches the given name.
-
-    Raises exception if evaluator is not in the config.
-
-    Parameters
-    ----------
-    qc_evaluator_name : string
-        Name of the qc_evaluator as defined in the config
-
-    Returns
-    -------
-    QualityCodeEvaluator
-        The QualityCodeEvaluator class initiated with the standard config data
-    """
-    qce_dict = get_qc_evaluator_dict()
-    if qc_evaluator_name in qce_dict:
-        return qce_dict[qc_evaluator_name]
-    raise Exception(
-        f"qc_evaluator {qc_evaluator_name} not found in the config file. "
-        f"Available qc_evaluators are {list(qce_dict.keys())}."
-    )
-
-
-def series_export_to_csv(
-    file_location: str,
-    series: list[pd.Series],
-) -> None:
-    """Export the 3 main series to csv.
-
-    Parameters
-    ----------
-    file_location : str
-        Where the files are exported to
-    series : pd.Series
-        Pandas series to be exported
-
-    Returns
-    -------
-    None, but makes files
-    """
-    export_df = pd.DataFrame(series).T
-    export_df.to_csv(str(file_location))
-
-
-def hilltop_export(
-    file_location: str,
-    site_name: str,
-    measurement_name: str,
-    std_series: pd.Series,
-    check_series: pd.Series,
-    qc_series: pd.Series,
-):
-    """
-    Export the 3 main series to csv files ready to import into hilltop.
-
-    Parameters
-    ----------
-    file_location : str
-        Where the files are exported to
-    site_name : str
-        Site name
-    measurement_name : str
-        measurement name
-    std_series : pd.Series
-        Standard series
-    check_series : pd.Series
-        Check series
-    qc_series : pd.Series
-        Quality code series
-
-    Returns
-    -------
-    None, but makes files
-    """
-    qc_series = qc_series.reindex(std_series.index, method="ffill")
-    std_series.name = "std"
-    qc_series.name = "qual"
-    export_df = std_series.to_frame().join(qc_series)
-    export_df.to_csv(str(file_location) + "_std_qc.csv")
-
-    keys = [
-        "Sitename",
-        "Inspection_Date",
-        "Inspection_Time",
-        "External S.G.",
-        "Recorder Time",
-        "Internal S.G.",
-        "Comment",
-    ]
-
-    export_check_df = pd.concat(
-        [
-            pd.Series(site_name, index=check_series.index),
-            pd.Series(
-                [str(dt.date()) for dt in check_series.index], index=check_series.index
-            ),
-            pd.Series(
-                [str(dt.time()) for dt in check_series.index], index=check_series.index
-            ),
-            check_series,
-            pd.Series(check_series.index, index=check_series.index),
-            pd.Series(-1, index=check_series.index),
-            pd.Series("hydrobot comment", index=check_series.index),
-        ],
-        axis=1,
-        keys=keys,
-    )
-
-    export_check_df.to_csv(str(file_location) + "_check.csv")
+"""Handling for different types of data sources."""
+import csv
+from pathlib import Path
+
+import numpy as np
+import pandas as pd
+
+
+class QualityCodeEvaluator:
+    """Basic QualityCodeEvaluator only compares magnitude of differences."""
+
+    def __init__(self, qc_500_limit, qc_600_limit, name=""):
+        """Initialize QualityCodeEvaluator.
+
+        Parameters
+        ----------
+        qc_500_limit : numerical
+            Threshold between QC 400 and QC 500
+        qc_600_limit : numerical
+            Threshold between QC 500 and QC 600
+        name : str
+            Name of the data source
+        """
+        self.qc_500_limit = qc_500_limit
+        self.qc_600_limit = qc_600_limit
+        self.name = name
+
+    def __repr__(self):
+        """QualityCodeEvaluator representation."""
+        return repr(f"QualityCodeEvaluator '{self.name}'")
+
+    def find_qc(self, base_datum, check_datum):
+        """Find the base quality codes.
+
+        Parameters
+        ----------
+        base_datum : numerical
+            Closest continuum datum point to the check
+        check_datum : numerical
+            The check data to verify the continuous data
+
+        Returns
+        -------
+        int
+            The Quality code
+
+        """
+        diff = np.abs(base_datum - check_datum)
+        if diff < self.qc_600_limit:
+            qc = 600
+        elif diff < self.qc_500_limit:
+            qc = 500
+        else:
+            qc = 400
+        return qc
+
+
+class TwoLevelQualityCodeEvaluator(QualityCodeEvaluator):
+    """QualityCodeEvaluator for standards such as water level.
+
+    Fixed error up to given threshold, percentage error after that.
+    """
+
+    def __init__(
+        self,
+        qc_500_limit,
+        qc_600_limit,
+        qc_500_percent,
+        qc_600_percent,
+        limit_percent_threshold,
+        name="",
+    ):
+        """Initialize TwoLevelQualityCodeEvaluator.
+
+        Parameters
+        ----------
+        qc_500_limit : numerical
+            Threshold between QC 400 and QC 500 for linear portion
+        qc_600_limit : numerical
+            Threshold between QC 500 and QC 600 for linear portion
+        qc_500_percent : numerical
+            Threshold between QC 400 and QC 500 for percentage portion
+        qc_600_percent : numerical
+            Threshold between QC 500 and QC 600 for percentage portion
+        limit_percent_threshold
+            Value at which the evaluator transitions between linear and percentage
+            QC comparison
+        name : str
+            Name of the data source
+        """
+        QualityCodeEvaluator.__init__(self, qc_500_limit, qc_600_limit, name)
+        self.qc_500_percent = qc_500_percent
+        self.qc_600_percent = qc_600_percent
+        self.limit_percent_threshold = limit_percent_threshold
+
+    def find_qc(self, base_datum, check_datum):
+        """Find the base quality codes with two stages.
+
+        The two stages are: a flat and percentage QC threshold.
+
+        Parameters
+        ----------
+        base_datum : numerical
+            Closest continuum datum point to the check
+        check_datum : numerical
+            The check data to verify the continuous data
+
+        Returns
+        -------
+        int
+            The Quality code
+
+        """
+        if base_datum < self.limit_percent_threshold:
+            # flat qc check
+            diff = np.abs(base_datum - check_datum)
+            if diff < self.qc_600_limit:
+                qc = 600
+            elif diff < self.qc_500_limit:
+                qc = 500
+            else:
+                qc = 400
+        else:
+            # percent qc check
+            diff = np.abs(base_datum / check_datum - 1) * 100
+            if diff < self.qc_600_percent:
+                qc = 600
+            elif diff < self.qc_500_percent:
+                qc = 500
+            else:
+                qc = 400
+        return qc
+
+
+def get_qc_evaluator_dict():
+    """Return all qc_evaluators in a dictionary.
+
+    Returns
+    -------
+    dict of string-qc_evaluator pairs
+    """
+    qc_evaluator_dict = {}
+    script_dir = Path(__file__).parent
+    # script_dir = os.path.dirname(os.path.abspath(__file__))
+
+    # Plain QualityCodeEvaluators
+    template_path = (script_dir / "config/QualityCodeEvaluator_QC_config.csv").resolve()
+    with open(template_path) as csv_file:
+        reader = csv.reader(csv_file)
+
+        for row in reader:
+            qc_evaluator_dict[row[0]] = QualityCodeEvaluator(
+                float(row[1]), float(row[2]), row[0]
+            )
+        csv_file.close()
+
+    # Two stage QualityCodeEvaluators
+    template_path = (
+        script_dir / "config/TwoLevelQualityCodeEvaluator_QC_config.csv"
+    ).resolve()
+    with open(template_path) as csv_file:
+        reader = csv.reader(csv_file)
+
+        for row in reader:
+            qc_evaluator_dict[row[0]] = TwoLevelQualityCodeEvaluator(
+                float(row[1]),
+                float(row[2]),
+                float(row[3]),
+                float(row[4]),
+                float(row[5]),
+                row[0],
+            )
+        csv_file.close()
+    return qc_evaluator_dict
+
+
+def get_qc_evaluator(qc_evaluator_name):
+    """Return qc_evaluator that matches the given name.
+
+    Raises exception if evaluator is not in the config.
+
+    Parameters
+    ----------
+    qc_evaluator_name : string
+        Name of the qc_evaluator as defined in the config
+
+    Returns
+    -------
+    QualityCodeEvaluator
+        The QualityCodeEvaluator class initiated with the standard config data
+    """
+    qce_dict = get_qc_evaluator_dict()
+    if qc_evaluator_name in qce_dict:
+        return qce_dict[qc_evaluator_name]
+    raise Exception(
+        f"qc_evaluator {qc_evaluator_name} not found in the config file. "
+        f"Available qc_evaluators are {list(qce_dict.keys())}."
+    )
+
+
+def series_export_to_csv(
+    file_location: str,
+    series: list[pd.Series],
+) -> None:
+    """Export the 3 main series to csv.
+
+    Parameters
+    ----------
+    file_location : str
+        Where the files are exported to
+    series : pd.Series
+        Pandas series to be exported
+
+    Returns
+    -------
+    None, but makes files
+    """
+    export_df = pd.DataFrame(series).T
+    export_df.to_csv(str(file_location))
+
+
+def hilltop_export(
+    file_location: str,
+    site_name: str,
+    measurement_name: str,
+    std_series: pd.Series,
+    check_series: pd.Series,
+    qc_series: pd.Series,
+):
+    """
+    Export the 3 main series to csv files ready to import into hilltop.
+
+    Parameters
+    ----------
+    file_location : str
+        Where the files are exported to
+    site_name : str
+        Site name
+    measurement_name : str
+        measurement name
+    std_series : pd.Series
+        Standard series
+    check_series : pd.Series
+        Check series
+    qc_series : pd.Series
+        Quality code series
+
+    Returns
+    -------
+    None, but makes files
+    """
+    qc_series = qc_series.reindex(std_series.index, method="ffill")
+    std_series.name = "std"
+    qc_series.name = "qual"
+    export_df = std_series.to_frame().join(qc_series)
+    export_df.to_csv(str(file_location) + "_std_qc.csv")
+
+    keys = [
+        "Sitename",
+        "Inspection_Date",
+        "Inspection_Time",
+        "External S.G.",
+        "Recorder Time",
+        "Internal S.G.",
+        "Comment",
+    ]
+
+    export_check_df = pd.concat(
+        [
+            pd.Series(site_name, index=check_series.index),
+            pd.Series(
+                [str(dt.date()) for dt in check_series.index], index=check_series.index
+            ),
+            pd.Series(
+                [str(dt.time()) for dt in check_series.index], index=check_series.index
+            ),
+            check_series,
+            pd.Series(check_series.index, index=check_series.index),
+            pd.Series(-1, index=check_series.index),
+            pd.Series("hydrobot comment", index=check_series.index),
+        ],
+        axis=1,
+        keys=keys,
+    )
+
+    export_check_df.to_csv(str(file_location) + "_check.csv")
```

### Comparing `hydrobot-0.5.0/hydrobot/evaluator.py` & `hydrobot-0.5.1/hydrobot/evaluator.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,455 +1,455 @@
-"""Tools for checking quality and finding problems in the data."""
-import warnings
-
-import numpy as np
-import pandas as pd
-from annalist.annalist import Annalist
-
-from hydrobot.data_sources import QualityCodeEvaluator
-
-annalizer = Annalist()
-
-
-def gap_finder(data: pd.Series):
-    """
-    Find gaps in a series of data (indicated by np.isnan()).
-
-    Returns a list of tuples indicating the start of the gap, and the number
-    of entries that are NaN
-
-    Parameters
-    ----------
-    data : pandas.Series
-        Input data to be clipped.
-
-    Returns
-    -------
-    List of Tuples
-        Each element in the list gives the index value for the start of the gap
-        and the length of the gap
-    """
-    idx0 = np.flatnonzero(np.r_[True, np.diff(np.isnan(data)) != 0, True])
-    count = np.diff(idx0)
-    idx = idx0[:-1]
-    valid_mask = pd.isna(data.iloc[idx])
-    out_idx = idx[valid_mask]
-    out_count = count[valid_mask]
-    indices = data.iloc[out_idx].index
-    out = zip(indices, out_count, strict=True)
-
-    return list(out)
-
-
-def small_gap_closer(series: pd.Series, gap_limit: int) -> pd.Series:
-    """
-    Remove small gaps from a series.
-
-    Gaps are defined by a sequential number of np.NaN values
-    Small gaps are defined as gaps of length gap_length or less.
-
-    Will return series with the nan values in the short gaps removed, and the
-    long gaps untouched.
-
-    Parameters
-    ----------
-    series : pandas.Series
-        Data which has gaps to be closed
-    gap_limit : integer
-        Maximum length of gaps removed, will remove all np.NaN's in consecutive runs
-        of gap_length or less
-
-    Returns
-    -------
-    pandas.Series
-        Data with any short gaps removed
-    """
-    gaps = gap_finder(series)
-    for gap in gaps:
-        if gap[1] <= gap_limit:
-            # Determine the range of rows to remove
-            mask = ~series.index.isin(
-                series.index[
-                    series.index.get_loc(gap[0]) : series.index.get_loc(gap[0]) + gap[1]
-                ]
-            )
-            # Remove the bad rows
-            series = pd.Series(series[mask])
-    return series
-
-
-def check_data_quality_code(
-    series: pd.Series,
-    check_series: pd.Series,
-    qc_evaluator: QualityCodeEvaluator,
-    gap_limit=10800,
-) -> pd.Series:
-    """
-    Quality Code Check Data.
-
-    Quality codes data based on the difference between the standard series and
-    the check data
-
-    Parameters
-    ----------
-    series : pd.Series
-        Data to be quality coded
-    check_series : pd.Series
-        Check data
-    qc_evaluator : data_sources.QualityCodeEvaluator
-        Handler for QC comparisons
-    gap_limit : integer (seconds)
-        If the nearest real data point is more than this many seconds away, return 200
-
-    Returns
-    -------
-    pd.Series
-        The QC values of the series, indexed by the END time of the QC period
-    """
-    first_data_date = series.index[0]
-    last_data_date = series.index[-1]
-    if check_series.empty and isinstance(first_data_date, pd.Timestamp):
-        # Maybe you should go find that check data
-        warnings.warn("Warning: No check data", stacklevel=2)
-        return pd.Series({first_data_date: np.NaN})
-    first_check_date = check_series.index[0]
-    last_check_date = check_series.index[-1]
-    if (
-        isinstance(first_data_date, pd.Timestamp)
-        and isinstance(last_data_date, pd.Timestamp)
-        and isinstance(first_check_date, pd.Timestamp)
-        and isinstance(last_check_date, pd.Timestamp)
-    ):
-        qc_series = pd.Series({first_data_date: np.NaN})
-        if first_check_date < first_data_date or last_check_date > last_data_date:
-            # Can't check something that's not there
-            raise KeyError(
-                "Error: check data out of range. "
-                f"First check date: {first_check_date}. "
-                f"First data date: {first_data_date}. "
-                f"Last check date: {last_check_date}. "
-                f"Last data date: {last_data_date}. "
-            )
-        else:
-            # Stuff actually working (hopefully)
-            for check_time, check_value in check_series.items():
-                if isinstance(check_time, pd.Timestamp):
-                    adjusted_time = find_nearest_valid_time(series, check_time)
-                    if abs((adjusted_time - check_time).total_seconds()) < gap_limit:
-                        qc_value = qc_evaluator.find_qc(
-                            series[adjusted_time], check_value
-                        )
-                    else:
-                        qc_value = 200
-                    qc_series[check_time] = qc_value
-                else:
-                    raise KeyError("Series indices should be pandas.Timestamp.")
-            qc_series = qc_series.shift(-1, fill_value=0)
-        return pd.Series(qc_series)
-    else:
-        raise KeyError("Series indices should be pandas.Timestamp.")
-
-
-def missing_data_quality_code(series, qc_series, gap_limit):
-    """
-    Make sure that missing data is QC100.
-
-    Returns qc_series with QC100 values added where series is NaN
-
-    Parameters
-    ----------
-    series : pd.Series
-        Base series which may contain NaNs
-    qc_series
-        QC series for base series without QC100 values
-    gap_limit
-        Maximum size of gaps which will be ignored
-
-    Returns
-    -------
-    pd.Series
-        The modified QC series, indexed by the start time of the QC period
-    """
-    for gap in gap_finder(series):
-        if gap[1] > gap_limit:
-            end_idx = series.index.get_loc(gap[0]) + gap[1]
-            # end of gap should recover the value from previous
-            if end_idx < len(series):
-                prev_values = qc_series[qc_series.index <= series.index[end_idx]]
-                prev_values = prev_values[prev_values > 100]
-                prev_values = prev_values.sort_index()
-                qc_series[series.index[end_idx]] = prev_values.iloc[-1]
-                qc_series = qc_series.sort_index()
-
-            # getting rid of any stray QC codes in the middle
-
-            drop_series = qc_series
-            drop_series = drop_series[drop_series.index > gap[0]]
-            drop_series = drop_series[drop_series.index <= series.index[end_idx - 1]]
-            qc_series = qc_series.drop(drop_series.index)
-
-            # start of gap
-            qc_series[gap[0]] = 100
-
-    return qc_series.sort_index()
-
-
-def find_nearest_time(series, dt):
-    """
-    Find the time in the series that is closest to dt.
-
-    For example for the series::
-
-        pd.Timestamp("2021-01-01 02:00"): 0.0,
-        pd.Timestamp("2021-01-01 02:15"): 0.0,
-
-    with dt::
-
-        pd.Timestamp("2021-01-01 02:13"): 0.0,
-
-    the result should be the closer ``pd.Timestamp("2021-01-01 02:15")`` value
-
-    Parameters
-    ----------
-    series : pd.Series
-        The series indexed by time
-
-    dt : Datetime
-        Time that may or may nor exactly line up with the series
-
-    Returns
-    -------
-    Datetime
-        The value of dt rounded to the nearest timestamp of the series
-
-    """
-    # Make sure it is in the range
-
-    first_timestamp = series.index[0]
-    last_timestamp = series.index[-1]
-    if dt < first_timestamp or dt > last_timestamp:
-        raise KeyError("Timestamp not within data range")
-
-    output_index = series.index.get_indexer([dt], method="nearest")
-    return series.index[output_index][0]
-
-
-def find_nearest_valid_time(series, dt) -> pd.Timestamp:
-    """
-    Find the time in the series that is closest to dt, but ignoring NaN values (gaps).
-
-    Parameters
-    ----------
-    series : pd.Series
-        The series indexed by time
-    dt : Datetime
-        Time that may or may nor exactly line up with the series
-
-    Returns
-    -------
-    Datetime
-        The value of dt rounded to the nearest timestamp of the series
-
-    """
-    # Make sure it is in the range
-    first_timestamp = series.index[0]
-    last_timestamp = series.index[-1]
-    if dt < first_timestamp or dt > last_timestamp:
-        raise KeyError("Timestamp not within data range")
-
-    series = series.dropna()
-    output_index = series.index.get_indexer([dt], method="nearest")
-    return series.index[output_index][0]
-
-
-def base_data_qc_filter(base_series, qc_filter):
-    """
-    Filter out data based on quality code filter.
-
-    Return only the base series data for which the next date in the qc_filter
-    is 'true'
-
-    Parameters
-    ----------
-    base_series : pandas.Series
-        Data to be filtered
-    qc_filter : pandas.Series of booleans
-        Dates for which some condition is met or not
-
-    Returns
-    -------
-    pandas.Series
-        The filtered data
-
-    """
-    base_filter = qc_filter.reindex(base_series.index, method="ffill").fillna(False)
-    return base_series[base_filter]
-
-
-def base_data_meets_qc(base_series, qc_series, target_qc):
-    """
-    Find all data where QC targets are met.
-
-    Returns only the base series data for which the next date in the qc_filter is
-    equal to target_qc
-
-    Parameters
-    ----------
-    base_series: pandas.Series
-        Data to be filtered
-    qc_series: pandas.Series
-        quality code data series, some of which are presumably target_qc
-    target_qc: int
-        target quality code
-
-    Returns
-    -------
-    pandas.Series
-        Filtered data
-    """
-    return base_data_qc_filter(base_series, qc_series == target_qc)
-
-
-def diagnose_data(base_series, check_series, qc_series, frequency):
-    """
-    Return description of how much missing data, how much for each QC, etc.
-
-    This function feels like a mess, I'm sorry.
-    The good news is that it is only a diagnostic, so feel free to change the hell
-    out of it
-
-    Parameters
-    ----------
-    raw_data : pandas.Series
-        unprocessed base time series data
-    base_series : pandas.Series
-        processed base time series data
-    check_series : pandas.Series
-        Check datatime series
-    qc_series : pandas.Series
-        QC time series
-    frequency : DateOffset or str
-        Frequency to which the data gets set to
-
-    Returns
-    -------
-    None
-        Prints statements that describe the state of the data
-    """
-    # total time
-    first_timestamp = base_series.index[0]
-    last_timestamp = base_series.index[-1]
-    total_time = last_timestamp - first_timestamp
-    print(f"Time examined is {total_time} from {first_timestamp} to {last_timestamp}")
-    print(
-        f"Have check data for {check_series.index[-1] - first_timestamp} "
-        f"(last check {check_series.index[-1]})"
-    )
-
-    # periods
-    ave_period = pd.to_timedelta(frequency)  # total_time / (len(raw_data) - 1)
-    gap_time = ave_period * (len(base_series) - len(base_series.dropna()) + 1)
-    print(f"Missing {gap_time} of data, that's {gap_time/total_time*100}%")
-
-    # QCs
-    split_data = splitter(base_series, qc_series, frequency)
-    for qc in split_data:
-        print(
-            f"Data that is QC{qc} makes up {len(split_data[qc].dropna()) / len(base_series.dropna()) * 100:.2f}% of "
-            f"the "
-            f"workable data and {len(split_data[qc].dropna()) / len(base_series) * 100:.2f}% of the time period"
-        )
-
-
-def splitter(base_series, qc_series, frequency):
-    """
-    Split the data up by QC code.
-
-    Selects all data which meets a given QC code, pads the rest with NaN values
-    Does this for all current NEMs values ([0, 100, 200, 300, 400, 500, 600])
-
-    Parameters
-    ----------
-    base_series
-        Time series data to be split up
-    qc_series : pd.Series
-        QC values to split the data by
-    frequency : DateOffset or str
-        Frequency to which the data gets set to
-
-    Returns
-    -------
-    dict of int:pd.Series pairs
-        Keys are the QC values as ints, values are series of data that fits
-    """
-    qc_list = [0, 100, 200, 300, 400, 500, 600]
-    return_dict = {}
-    for qc in qc_list:
-        if qc == 100:
-            return_dict[qc] = (
-                base_data_meets_qc(base_series, qc_series, qc)
-                .fillna(base_series.median())
-                .asfreq(frequency)
-            )
-        else:
-            return_dict[qc] = base_data_meets_qc(base_series, qc_series, qc).asfreq(
-                frequency
-            )
-
-    return return_dict
-
-
-def max_qc_limiter(qc_series: pd.Series, max_qc) -> pd.Series:
-    """
-    Enforce max_qc on a QC series.
-
-    Replaces all values with QCs above max_qc with max_qc
-
-    Parameters
-    ----------
-    qc_series : pd.Series
-        The series to be limited.
-    max_qc : numerical
-        maximum allowed value. None imposes no limit.
-
-    Returns
-    -------
-    pd.Series
-        qc_series with too high QCs limited to max_qc
-    """
-    return pd.Series(qc_series.clip(np.NaN, max_qc))
-
-
-def quality_encoder(
-    base_series: pd.Series,
-    check_series: pd.Series,
-    qc_evaluator: QualityCodeEvaluator,
-    gap_limit: int,
-    max_qc=np.NaN,
-) -> pd.Series:
-    """
-    Return complete QC series.
-
-    Parameters
-    ----------
-    base_series : pd.Series
-        Base time series data
-    check_series : pd.Series
-        Check data time series
-    qc_evaluator : data_sources.QualityCodeEvaluator
-        Handler for QC comparisons
-    gap_limit
-        Maximum size of gaps which will be ignored
-    max_qc
-        Maximum allowed QC value
-
-    Returns
-    -------
-    pd.Series
-        The modified QC series, indexed by the start time of the QC period
-    """
-    qc_series = check_data_quality_code(base_series, check_series, qc_evaluator)
-    qc_series = missing_data_quality_code(base_series, qc_series, gap_limit=gap_limit)
-    qc_series = max_qc_limiter(qc_series, max_qc)
-    # qc_series.index.name = "Time"
-    # qc_series.name = "Value"
-    return qc_series
+"""Tools for checking quality and finding problems in the data."""
+import warnings
+
+import numpy as np
+import pandas as pd
+from annalist.annalist import Annalist
+
+from hydrobot.data_sources import QualityCodeEvaluator
+
+annalizer = Annalist()
+
+
+def gap_finder(data: pd.Series):
+    """
+    Find gaps in a series of data (indicated by np.isnan()).
+
+    Returns a list of tuples indicating the start of the gap, and the number
+    of entries that are NaN
+
+    Parameters
+    ----------
+    data : pandas.Series
+        Input data to be clipped.
+
+    Returns
+    -------
+    List of Tuples
+        Each element in the list gives the index value for the start of the gap
+        and the length of the gap
+    """
+    idx0 = np.flatnonzero(np.r_[True, np.diff(np.isnan(data)) != 0, True])
+    count = np.diff(idx0)
+    idx = idx0[:-1]
+    valid_mask = pd.isna(data.iloc[idx])
+    out_idx = idx[valid_mask]
+    out_count = count[valid_mask]
+    indices = data.iloc[out_idx].index
+    out = zip(indices, out_count, strict=True)
+
+    return list(out)
+
+
+def small_gap_closer(series: pd.Series, gap_limit: int) -> pd.Series:
+    """
+    Remove small gaps from a series.
+
+    Gaps are defined by a sequential number of np.NaN values
+    Small gaps are defined as gaps of length gap_length or less.
+
+    Will return series with the nan values in the short gaps removed, and the
+    long gaps untouched.
+
+    Parameters
+    ----------
+    series : pandas.Series
+        Data which has gaps to be closed
+    gap_limit : integer
+        Maximum length of gaps removed, will remove all np.NaN's in consecutive runs
+        of gap_length or less
+
+    Returns
+    -------
+    pandas.Series
+        Data with any short gaps removed
+    """
+    gaps = gap_finder(series)
+    for gap in gaps:
+        if gap[1] <= gap_limit:
+            # Determine the range of rows to remove
+            mask = ~series.index.isin(
+                series.index[
+                    series.index.get_loc(gap[0]) : series.index.get_loc(gap[0]) + gap[1]
+                ]
+            )
+            # Remove the bad rows
+            series = pd.Series(series[mask])
+    return series
+
+
+def check_data_quality_code(
+    series: pd.Series,
+    check_series: pd.Series,
+    qc_evaluator: QualityCodeEvaluator,
+    gap_limit=10800,
+) -> pd.Series:
+    """
+    Quality Code Check Data.
+
+    Quality codes data based on the difference between the standard series and
+    the check data
+
+    Parameters
+    ----------
+    series : pd.Series
+        Data to be quality coded
+    check_series : pd.Series
+        Check data
+    qc_evaluator : data_sources.QualityCodeEvaluator
+        Handler for QC comparisons
+    gap_limit : integer (seconds)
+        If the nearest real data point is more than this many seconds away, return 200
+
+    Returns
+    -------
+    pd.Series
+        The QC values of the series, indexed by the END time of the QC period
+    """
+    first_data_date = series.index[0]
+    last_data_date = series.index[-1]
+    if check_series.empty and isinstance(first_data_date, pd.Timestamp):
+        # Maybe you should go find that check data
+        warnings.warn("Warning: No check data", stacklevel=2)
+        return pd.Series({first_data_date: np.NaN})
+    first_check_date = check_series.index[0]
+    last_check_date = check_series.index[-1]
+    if (
+        isinstance(first_data_date, pd.Timestamp)
+        and isinstance(last_data_date, pd.Timestamp)
+        and isinstance(first_check_date, pd.Timestamp)
+        and isinstance(last_check_date, pd.Timestamp)
+    ):
+        qc_series = pd.Series({first_data_date: np.NaN})
+        if first_check_date < first_data_date or last_check_date > last_data_date:
+            # Can't check something that's not there
+            raise KeyError(
+                "Error: check data out of range. "
+                f"First check date: {first_check_date}. "
+                f"First data date: {first_data_date}. "
+                f"Last check date: {last_check_date}. "
+                f"Last data date: {last_data_date}. "
+            )
+        else:
+            # Stuff actually working (hopefully)
+            for check_time, check_value in check_series.items():
+                if isinstance(check_time, pd.Timestamp):
+                    adjusted_time = find_nearest_valid_time(series, check_time)
+                    if abs((adjusted_time - check_time).total_seconds()) < gap_limit:
+                        qc_value = qc_evaluator.find_qc(
+                            series[adjusted_time], check_value
+                        )
+                    else:
+                        qc_value = 200
+                    qc_series[check_time] = qc_value
+                else:
+                    raise KeyError("Series indices should be pandas.Timestamp.")
+            qc_series = qc_series.shift(-1, fill_value=0)
+        return pd.Series(qc_series)
+    else:
+        raise KeyError("Series indices should be pandas.Timestamp.")
+
+
+def missing_data_quality_code(series, qc_series, gap_limit):
+    """
+    Make sure that missing data is QC100.
+
+    Returns qc_series with QC100 values added where series is NaN
+
+    Parameters
+    ----------
+    series : pd.Series
+        Base series which may contain NaNs
+    qc_series
+        QC series for base series without QC100 values
+    gap_limit
+        Maximum size of gaps which will be ignored
+
+    Returns
+    -------
+    pd.Series
+        The modified QC series, indexed by the start time of the QC period
+    """
+    for gap in gap_finder(series):
+        if gap[1] > gap_limit:
+            end_idx = series.index.get_loc(gap[0]) + gap[1]
+            # end of gap should recover the value from previous
+            if end_idx < len(series):
+                prev_values = qc_series[qc_series.index <= series.index[end_idx]]
+                prev_values = prev_values[prev_values > 100]
+                prev_values = prev_values.sort_index()
+                qc_series[series.index[end_idx]] = prev_values.iloc[-1]
+                qc_series = qc_series.sort_index()
+
+            # getting rid of any stray QC codes in the middle
+
+            drop_series = qc_series
+            drop_series = drop_series[drop_series.index > gap[0]]
+            drop_series = drop_series[drop_series.index <= series.index[end_idx - 1]]
+            qc_series = qc_series.drop(drop_series.index)
+
+            # start of gap
+            qc_series[gap[0]] = 100
+
+    return qc_series.sort_index()
+
+
+def find_nearest_time(series, dt):
+    """
+    Find the time in the series that is closest to dt.
+
+    For example for the series::
+
+        pd.Timestamp("2021-01-01 02:00"): 0.0,
+        pd.Timestamp("2021-01-01 02:15"): 0.0,
+
+    with dt::
+
+        pd.Timestamp("2021-01-01 02:13"): 0.0,
+
+    the result should be the closer ``pd.Timestamp("2021-01-01 02:15")`` value
+
+    Parameters
+    ----------
+    series : pd.Series
+        The series indexed by time
+
+    dt : Datetime
+        Time that may or may nor exactly line up with the series
+
+    Returns
+    -------
+    Datetime
+        The value of dt rounded to the nearest timestamp of the series
+
+    """
+    # Make sure it is in the range
+
+    first_timestamp = series.index[0]
+    last_timestamp = series.index[-1]
+    if dt < first_timestamp or dt > last_timestamp:
+        raise KeyError("Timestamp not within data range")
+
+    output_index = series.index.get_indexer([dt], method="nearest")
+    return series.index[output_index][0]
+
+
+def find_nearest_valid_time(series, dt) -> pd.Timestamp:
+    """
+    Find the time in the series that is closest to dt, but ignoring NaN values (gaps).
+
+    Parameters
+    ----------
+    series : pd.Series
+        The series indexed by time
+    dt : Datetime
+        Time that may or may nor exactly line up with the series
+
+    Returns
+    -------
+    Datetime
+        The value of dt rounded to the nearest timestamp of the series
+
+    """
+    # Make sure it is in the range
+    first_timestamp = series.index[0]
+    last_timestamp = series.index[-1]
+    if dt < first_timestamp or dt > last_timestamp:
+        raise KeyError("Timestamp not within data range")
+
+    series = series.dropna()
+    output_index = series.index.get_indexer([dt], method="nearest")
+    return series.index[output_index][0]
+
+
+def base_data_qc_filter(base_series, qc_filter):
+    """
+    Filter out data based on quality code filter.
+
+    Return only the base series data for which the next date in the qc_filter
+    is 'true'
+
+    Parameters
+    ----------
+    base_series : pandas.Series
+        Data to be filtered
+    qc_filter : pandas.Series of booleans
+        Dates for which some condition is met or not
+
+    Returns
+    -------
+    pandas.Series
+        The filtered data
+
+    """
+    base_filter = qc_filter.reindex(base_series.index, method="ffill").fillna(False)
+    return base_series[base_filter]
+
+
+def base_data_meets_qc(base_series, qc_series, target_qc):
+    """
+    Find all data where QC targets are met.
+
+    Returns only the base series data for which the next date in the qc_filter is
+    equal to target_qc
+
+    Parameters
+    ----------
+    base_series: pandas.Series
+        Data to be filtered
+    qc_series: pandas.Series
+        quality code data series, some of which are presumably target_qc
+    target_qc: int
+        target quality code
+
+    Returns
+    -------
+    pandas.Series
+        Filtered data
+    """
+    return base_data_qc_filter(base_series, qc_series == target_qc)
+
+
+def diagnose_data(base_series, check_series, qc_series, frequency):
+    """
+    Return description of how much missing data, how much for each QC, etc.
+
+    This function feels like a mess, I'm sorry.
+    The good news is that it is only a diagnostic, so feel free to change the hell
+    out of it
+
+    Parameters
+    ----------
+    raw_data : pandas.Series
+        unprocessed base time series data
+    base_series : pandas.Series
+        processed base time series data
+    check_series : pandas.Series
+        Check datatime series
+    qc_series : pandas.Series
+        QC time series
+    frequency : DateOffset or str
+        Frequency to which the data gets set to
+
+    Returns
+    -------
+    None
+        Prints statements that describe the state of the data
+    """
+    # total time
+    first_timestamp = base_series.index[0]
+    last_timestamp = base_series.index[-1]
+    total_time = last_timestamp - first_timestamp
+    print(f"Time examined is {total_time} from {first_timestamp} to {last_timestamp}")
+    print(
+        f"Have check data for {check_series.index[-1] - first_timestamp} "
+        f"(last check {check_series.index[-1]})"
+    )
+
+    # periods
+    ave_period = pd.to_timedelta(frequency)  # total_time / (len(raw_data) - 1)
+    gap_time = ave_period * (len(base_series) - len(base_series.dropna()) + 1)
+    print(f"Missing {gap_time} of data, that's {gap_time/total_time*100}%")
+
+    # QCs
+    split_data = splitter(base_series, qc_series, frequency)
+    for qc in split_data:
+        print(
+            f"Data that is QC{qc} makes up {len(split_data[qc].dropna()) / len(base_series.dropna()) * 100:.2f}% of "
+            f"the "
+            f"workable data and {len(split_data[qc].dropna()) / len(base_series) * 100:.2f}% of the time period"
+        )
+
+
+def splitter(base_series, qc_series, frequency):
+    """
+    Split the data up by QC code.
+
+    Selects all data which meets a given QC code, pads the rest with NaN values
+    Does this for all current NEMs values ([0, 100, 200, 300, 400, 500, 600])
+
+    Parameters
+    ----------
+    base_series
+        Time series data to be split up
+    qc_series : pd.Series
+        QC values to split the data by
+    frequency : DateOffset or str
+        Frequency to which the data gets set to
+
+    Returns
+    -------
+    dict of int:pd.Series pairs
+        Keys are the QC values as ints, values are series of data that fits
+    """
+    qc_list = [0, 100, 200, 300, 400, 500, 600]
+    return_dict = {}
+    for qc in qc_list:
+        if qc == 100:
+            return_dict[qc] = (
+                base_data_meets_qc(base_series, qc_series, qc)
+                .fillna(base_series.median())
+                .asfreq(frequency)
+            )
+        else:
+            return_dict[qc] = base_data_meets_qc(base_series, qc_series, qc).asfreq(
+                frequency
+            )
+
+    return return_dict
+
+
+def max_qc_limiter(qc_series: pd.Series, max_qc) -> pd.Series:
+    """
+    Enforce max_qc on a QC series.
+
+    Replaces all values with QCs above max_qc with max_qc
+
+    Parameters
+    ----------
+    qc_series : pd.Series
+        The series to be limited.
+    max_qc : numerical
+        maximum allowed value. None imposes no limit.
+
+    Returns
+    -------
+    pd.Series
+        qc_series with too high QCs limited to max_qc
+    """
+    return pd.Series(qc_series.clip(np.NaN, max_qc))
+
+
+def quality_encoder(
+    base_series: pd.Series,
+    check_series: pd.Series,
+    qc_evaluator: QualityCodeEvaluator,
+    gap_limit: int,
+    max_qc=np.NaN,
+) -> pd.Series:
+    """
+    Return complete QC series.
+
+    Parameters
+    ----------
+    base_series : pd.Series
+        Base time series data
+    check_series : pd.Series
+        Check data time series
+    qc_evaluator : data_sources.QualityCodeEvaluator
+        Handler for QC comparisons
+    gap_limit
+        Maximum size of gaps which will be ignored
+    max_qc
+        Maximum allowed QC value
+
+    Returns
+    -------
+    pd.Series
+        The modified QC series, indexed by the start time of the QC period
+    """
+    qc_series = check_data_quality_code(base_series, check_series, qc_evaluator)
+    qc_series = missing_data_quality_code(base_series, qc_series, gap_limit=gap_limit)
+    qc_series = max_qc_limiter(qc_series, max_qc)
+    # qc_series.index.name = "Time"
+    # qc_series.name = "Value"
+    return qc_series
```

### Comparing `hydrobot-0.5.0/hydrobot/filters.py` & `hydrobot-0.5.1/hydrobot/filters.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,249 +1,249 @@
-"""General filtering utilities."""
-
-
-import numpy as np
-import pandas as pd
-from annalist.annalist import Annalist
-
-annalizer = Annalist()
-
-
-def clip(unclipped: pd.Series, low_clip: float, high_clip: float):
-    """Clip values in a pandas Series within a specified range.
-
-    Parameters
-    ----------
-    unclipped : pandas.Series
-        Input data to be clipped.
-    high_clip : float
-        Upper bound for clipping. Values greater than this will be set to NaN.
-    low_clip : float
-        Lower bound for clipping. Values less than this will be set to NaN.
-
-    Returns
-    -------
-    pandas.Series
-        A Series containing the clipped values with the same index as the
-        input Series.
-    """
-    unclipped_arr = unclipped.to_numpy()
-
-    # Create a boolean condition for values that need to be clipped
-    clip_cond = (unclipped_arr > high_clip) | (unclipped_arr < low_clip)
-
-    # Use pandas' where function to clip values to NaN where the condition is
-    # True
-    clipped_series = unclipped.where(~clip_cond, np.nan)
-
-    return clipped_series
-
-
-# noinspection SpellCheckingInspection
-def fbewma(input_data, span: int):
-    """Calculate the Forward-Backward Exponentially Weighted Moving Average (FBEWMA).
-
-    Parameters
-    ----------
-    input_data : pandas.Series
-        Input time series data to calculate the FBEWMA on.
-    span : int
-        Span parameter for exponential weighting.
-
-    Returns
-    -------
-    pandas.Series
-        A Series containing the FBEWMA values with the same index as the
-        input Series.
-    """
-    # Calculate the Forward EWMA.
-    fwd = input_data.ewm(span=span).mean()
-
-    # Calculate the Backward EWMA. (x[::-1] is the reverse of x)
-    bwd = input_data[::-1].ewm(span=span).mean()
-
-    # Stack fwd and the reverse of bwd on top of each other.
-    stacked_ewma = pd.concat([fwd, bwd[::-1]])
-
-    # Calculate the FB-EWMA by taking the mean between fwd and bwd.
-    return stacked_ewma.groupby(level=0).mean()
-
-
-def remove_outliers(input_data: pd.Series, span: int, delta: float):
-    """Remove outliers.
-
-    Remove outliers from a time series by comparing it to the
-    Forward-Backward Exponentially Weighted Moving Average (FBEWMA).
-
-    Parameters
-    ----------
-    input_data : pandas.Series
-        Input time series data.
-    span : int
-        Span parameter for exponential weighting used in the FBEWMA.
-    delta : float
-        Threshold for identifying outliers. Values greater than this
-        threshold will be set to NaN.
-
-    Returns
-    -------
-    pandas.Series
-        A Series containing the time series with outliers removed with
-        the same index as the input Series.
-    """
-    # Calculate the FBEWMA of the time series
-    fbewma_series = fbewma(input_data, span)
-
-    # Create a condition to identify outliers based on the absolute difference
-    # between input_data and fbewma_series
-    delta_cond = np.abs(input_data - fbewma_series) > delta
-
-    # Set values to NaN where the condition is True
-    return input_data.where(~delta_cond, np.nan)
-
-
-def remove_spikes(
-    input_data: pd.Series, span: int, low_clip: float, high_clip: float, delta: float
-) -> pd.Series:
-    """Remove spikes.
-
-    Remove spikes from a time series data using a combination of clipping and
-    interpolation.
-
-    Parameters
-    ----------
-    input_data : pandas.Series
-        Input time series data.
-    span : int
-        Span parameter for exponential weighting used in outlier detection.
-    low_clip : float
-        Lower bound for clipping. Values less than this will be set to NaN.
-    high_clip : float
-        Upper bound for clipping. Values greater than this will be set to NaN.
-    delta : float
-        Threshold for identifying outliers. Values greater than this threshold
-        will be considered spikes.
-
-    Returns
-    -------
-    pandas.Series
-        A Series containing the time series with spikes removed with the same
-        index as the input Series.
-    """
-    # Clip values in the input data within the specified range
-    clipped = clip(input_data, low_clip, high_clip)
-
-    # Remove outliers using the remove_outliers function
-    gaps_series = remove_outliers(clipped, span, delta)
-
-    # Could use pandas' .interpolate() on the Series
-    # interp_series = gaps_series.interpolate()
-
-    return gaps_series
-
-
-def remove_range(
-    input_series: pd.Series,
-    from_date: str | None,
-    to_date: str | None,
-    insert_gaps: bool | int = False,
-):
-    """
-    Remove data from series in given range.
-
-    Returns the input series without data between from_date and to_date
-    inclusive.
-
-    A None to_date will remove all data since the from_date (and vice versa).
-    A double None for to_date/from_date removes all data.
-
-    Inserts gaps or not depending on insert_gaps
-
-    Parameters
-    ----------
-    input_series : pd.Series
-        The series to have a section removed
-    from_date : str | None
-        Start of removed section
-    to_date : str | None
-        End of removed section
-    insert_gaps : bool or int
-        If True, inserts a gap.
-        If False, does not insert a gap.
-        If int, will insert gaps if missing more data points than insert_gaps
-
-    Returns
-    -------
-    pd.Series
-        The series with relevant slice removed
-    """
-    slice_to_remove = input_series.loc[from_date:to_date]
-    series_to_return = input_series.drop(slice_to_remove.index)
-    if isinstance(insert_gaps, bool):
-        if insert_gaps:
-            series_to_return[from_date] = np.NaN
-    else:
-        if len(slice_to_remove) > insert_gaps:
-            series_to_return[from_date] = np.NaN
-    return series_to_return.sort_index()
-
-
-def trim_series(std_series: pd.Series, check_series: pd.Series) -> pd.Series:
-    """
-    Remove end of std series to match check series.
-
-    All data after the last entry in check_series is presumed to be unchecked,
-    so that data is removed from the std_series
-
-    If check_series is empty, returns the entire std_series
-
-    Parameters
-    ----------
-    std_series : pd.Series
-        The series to be trimmed
-    check_series : pd.Series | pd.DataFrame
-        Indicates the end of the usable data
-
-    Returns
-    -------
-    pd.Series
-        std_series with the unchecked elements trimmed
-    """
-    if check_series.empty:
-        return std_series
-    else:
-        last_check_date = check_series.index[-1]
-        return std_series.loc[:last_check_date]
-
-
-def flatline_value_remover(
-    series: pd.Series,
-    span: int = 3,
-):
-    """
-    Remove repeated (flatlined) values in a series.
-
-    Examines the data to see if any values are exactly repeated over a period.
-    Where values exactly repeat it probably indicates a broken instrument.
-    Replaces all values after the first with NaN.
-    Uses math.isclose() to measure float "equality"
-
-    Parameters
-    ----------
-    series : pd.Series
-        Data to examine for flatlined values
-    span : int
-        Amount of allowed repeated values in a row before duplicates are removed
-
-    Returns
-    -------
-    pd.Series
-        Data with the flatlined values NaN'ed
-    """
-    # pandas bad day
-    consecutive_values = (
-        series.groupby((series != series.shift()).cumsum()).cumcount() + 1
-    )
-    working_step = consecutive_values.loc[~consecutive_values.between(2, span)]
-    length_filter = working_step.reindex(consecutive_values.index).bfill()
-    filtered_data = pd.Series(series[length_filter < span])
-    return filtered_data.reindex(series.index)
+"""General filtering utilities."""
+
+
+import numpy as np
+import pandas as pd
+from annalist.annalist import Annalist
+
+annalizer = Annalist()
+
+
+def clip(unclipped: pd.Series, low_clip: float, high_clip: float):
+    """Clip values in a pandas Series within a specified range.
+
+    Parameters
+    ----------
+    unclipped : pandas.Series
+        Input data to be clipped.
+    high_clip : float
+        Upper bound for clipping. Values greater than this will be set to NaN.
+    low_clip : float
+        Lower bound for clipping. Values less than this will be set to NaN.
+
+    Returns
+    -------
+    pandas.Series
+        A Series containing the clipped values with the same index as the
+        input Series.
+    """
+    unclipped_arr = unclipped.to_numpy()
+
+    # Create a boolean condition for values that need to be clipped
+    clip_cond = (unclipped_arr > high_clip) | (unclipped_arr < low_clip)
+
+    # Use pandas' where function to clip values to NaN where the condition is
+    # True
+    clipped_series = unclipped.where(~clip_cond, np.nan)
+
+    return clipped_series
+
+
+# noinspection SpellCheckingInspection
+def fbewma(input_data, span: int):
+    """Calculate the Forward-Backward Exponentially Weighted Moving Average (FBEWMA).
+
+    Parameters
+    ----------
+    input_data : pandas.Series
+        Input time series data to calculate the FBEWMA on.
+    span : int
+        Span parameter for exponential weighting.
+
+    Returns
+    -------
+    pandas.Series
+        A Series containing the FBEWMA values with the same index as the
+        input Series.
+    """
+    # Calculate the Forward EWMA.
+    fwd = input_data.ewm(span=span).mean()
+
+    # Calculate the Backward EWMA. (x[::-1] is the reverse of x)
+    bwd = input_data[::-1].ewm(span=span).mean()
+
+    # Stack fwd and the reverse of bwd on top of each other.
+    stacked_ewma = pd.concat([fwd, bwd[::-1]])
+
+    # Calculate the FB-EWMA by taking the mean between fwd and bwd.
+    return stacked_ewma.groupby(level=0).mean()
+
+
+def remove_outliers(input_data: pd.Series, span: int, delta: float):
+    """Remove outliers.
+
+    Remove outliers from a time series by comparing it to the
+    Forward-Backward Exponentially Weighted Moving Average (FBEWMA).
+
+    Parameters
+    ----------
+    input_data : pandas.Series
+        Input time series data.
+    span : int
+        Span parameter for exponential weighting used in the FBEWMA.
+    delta : float
+        Threshold for identifying outliers. Values greater than this
+        threshold will be set to NaN.
+
+    Returns
+    -------
+    pandas.Series
+        A Series containing the time series with outliers removed with
+        the same index as the input Series.
+    """
+    # Calculate the FBEWMA of the time series
+    fbewma_series = fbewma(input_data, span)
+
+    # Create a condition to identify outliers based on the absolute difference
+    # between input_data and fbewma_series
+    delta_cond = np.abs(input_data - fbewma_series) > delta
+
+    # Set values to NaN where the condition is True
+    return input_data.where(~delta_cond, np.nan)
+
+
+def remove_spikes(
+    input_data: pd.Series, span: int, low_clip: float, high_clip: float, delta: float
+) -> pd.Series:
+    """Remove spikes.
+
+    Remove spikes from a time series data using a combination of clipping and
+    interpolation.
+
+    Parameters
+    ----------
+    input_data : pandas.Series
+        Input time series data.
+    span : int
+        Span parameter for exponential weighting used in outlier detection.
+    low_clip : float
+        Lower bound for clipping. Values less than this will be set to NaN.
+    high_clip : float
+        Upper bound for clipping. Values greater than this will be set to NaN.
+    delta : float
+        Threshold for identifying outliers. Values greater than this threshold
+        will be considered spikes.
+
+    Returns
+    -------
+    pandas.Series
+        A Series containing the time series with spikes removed with the same
+        index as the input Series.
+    """
+    # Clip values in the input data within the specified range
+    clipped = clip(input_data, low_clip, high_clip)
+
+    # Remove outliers using the remove_outliers function
+    gaps_series = remove_outliers(clipped, span, delta)
+
+    # Could use pandas' .interpolate() on the Series
+    # interp_series = gaps_series.interpolate()
+
+    return gaps_series
+
+
+def remove_range(
+    input_series: pd.Series,
+    from_date: str | None,
+    to_date: str | None,
+    insert_gaps: bool | int = False,
+):
+    """
+    Remove data from series in given range.
+
+    Returns the input series without data between from_date and to_date
+    inclusive.
+
+    A None to_date will remove all data since the from_date (and vice versa).
+    A double None for to_date/from_date removes all data.
+
+    Inserts gaps or not depending on insert_gaps
+
+    Parameters
+    ----------
+    input_series : pd.Series
+        The series to have a section removed
+    from_date : str | None
+        Start of removed section
+    to_date : str | None
+        End of removed section
+    insert_gaps : bool or int
+        If True, inserts a gap.
+        If False, does not insert a gap.
+        If int, will insert gaps if missing more data points than insert_gaps
+
+    Returns
+    -------
+    pd.Series
+        The series with relevant slice removed
+    """
+    slice_to_remove = input_series.loc[from_date:to_date]
+    series_to_return = input_series.drop(slice_to_remove.index)
+    if isinstance(insert_gaps, bool):
+        if insert_gaps:
+            series_to_return[from_date] = np.NaN
+    else:
+        if len(slice_to_remove) > insert_gaps:
+            series_to_return[from_date] = np.NaN
+    return series_to_return.sort_index()
+
+
+def trim_series(std_series: pd.Series, check_series: pd.Series) -> pd.Series:
+    """
+    Remove end of std series to match check series.
+
+    All data after the last entry in check_series is presumed to be unchecked,
+    so that data is removed from the std_series
+
+    If check_series is empty, returns the entire std_series
+
+    Parameters
+    ----------
+    std_series : pd.Series
+        The series to be trimmed
+    check_series : pd.Series | pd.DataFrame
+        Indicates the end of the usable data
+
+    Returns
+    -------
+    pd.Series
+        std_series with the unchecked elements trimmed
+    """
+    if check_series.empty:
+        return std_series
+    else:
+        last_check_date = check_series.index[-1]
+        return std_series.loc[:last_check_date]
+
+
+def flatline_value_remover(
+    series: pd.Series,
+    span: int = 3,
+):
+    """
+    Remove repeated (flatlined) values in a series.
+
+    Examines the data to see if any values are exactly repeated over a period.
+    Where values exactly repeat it probably indicates a broken instrument.
+    Replaces all values after the first with NaN.
+    Uses math.isclose() to measure float "equality"
+
+    Parameters
+    ----------
+    series : pd.Series
+        Data to examine for flatlined values
+    span : int
+        Amount of allowed repeated values in a row before duplicates are removed
+
+    Returns
+    -------
+    pd.Series
+        Data with the flatlined values NaN'ed
+    """
+    # pandas bad day
+    consecutive_values = (
+        series.groupby((series != series.shift()).cumsum()).cumcount() + 1
+    )
+    working_step = consecutive_values.loc[~consecutive_values.between(2, span)]
+    length_filter = working_step.reindex(consecutive_values.index).bfill()
+    filtered_data = pd.Series(series[length_filter < span])
+    return filtered_data.reindex(series.index)
```

### Comparing `hydrobot-0.5.0/hydrobot/plotter.py` & `hydrobot-0.5.1/hydrobot/plotter.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,731 +1,731 @@
-"""Tools for displaying potentially problematic data."""
-import warnings
-
-import matplotlib.pyplot as plt
-import numpy as np
-import pandas as pd
-import plotly.graph_objects as go
-from plotly.subplots import make_subplots
-
-from hydrobot.evaluator import find_nearest_time, gap_finder, splitter
-from hydrobot.utils import change_blocks, merge_all_comments
-
-
-def gap_plotter(base_series, span=20, show=True):
-    """Plot the areas around NaN.to_numpy() to visually check for dodgy spike removal.
-
-    Parameters
-    ----------
-    base_series : pd.Series
-        Data to have the gaps found and plotted
-    span : int
-        How many points around the gap gets plotted
-    show : bool
-        Whether to show the plot directly when called
-
-    Returns
-    -------
-    None
-        Outputs a series of plots
-    """
-    for gap in gap_finder(base_series):
-        plt.figure()
-        idx = base_series.index.get_loc(gap[0])
-        lower_idx = idx - span
-        upper_idx = idx + span + gap[1]
-        if lower_idx < 0:
-            # below range
-            upper_idx -= lower_idx
-            lower_idx -= lower_idx
-        if upper_idx > len(base_series):
-            # above range
-            lower_idx -= len(base_series) - upper_idx
-            upper_idx -= len(base_series) - upper_idx
-            if lower_idx < 0:
-                # span is too big or not enough data
-                warnings.warn("Warning: Span bigger than data", stacklevel=2)
-                lower_idx = 0
-        gap_range = base_series.iloc[lower_idx:upper_idx]
-        plt.plot(gap_range.index, gap_range)
-        plt.title(f"Gap starting at {gap[0]}")
-    if show:
-        plt.show()
-
-
-def check_plotter(base_series, check_series, span=20, show=True):
-    """Plot the areas around check.to_numpy() to visually check for dodgy data from inspections.
-
-    Parameters
-    ----------
-    base_series : pd.Series
-        Data to plot
-    check_series : pd.Series
-        Check data which determines where the data is plotted
-    span : int
-        How much space around the check data is shown
-    show : bool
-        Whether to show the plot directly when called
-
-    Returns
-    -------
-    None
-        Outputs a series of plots
-
-    """
-    for check in check_series.index:
-        plt.figure()
-        idx = base_series.index.get_loc(find_nearest_time(base_series, check))
-        lower_idx = idx - span
-        upper_idx = idx + span
-        if lower_idx < 0:
-            # below range
-            upper_idx -= lower_idx
-            lower_idx -= lower_idx
-        if upper_idx > len(base_series):
-            # above range
-            lower_idx -= len(base_series) - upper_idx
-            upper_idx -= len(base_series) - upper_idx
-            if lower_idx < 0:
-                # span is too big or not enough data
-                warnings.warn("Warning: Span bigger than data", stacklevel=2)
-                lower_idx = 0
-        gap_range = base_series.iloc[lower_idx:upper_idx]
-        plt.plot(gap_range.index, gap_range)
-        plt.plot(
-            check,
-            check_series[check],
-            label="Check data",
-            marker="o",
-            color="darkturquoise",
-        )
-        plt.title(f"Check at {check}")
-    if show:
-        plt.show()
-
-
-def qc_colour(qc):
-    """Give the colour of the QC.
-
-    Parameters
-    ----------
-    qc : int
-        Quality code
-
-    Returns
-    -------
-    String
-        Hex code for the colour of the QC
-    """
-    qc_dict = {
-        None: "darkslategrey",
-        "nan": "darkslategrey",
-        0: "#9900ff",
-        100: "#ff0000",
-        200: "#8B5A00",
-        300: "#d3d3d3",
-        400: "#ffa500",
-        500: "#00bfff",
-        600: "#006400",
-    }
-    return qc_dict[qc]
-
-
-def qc_plotter(base_series, check_series, qc_series, frequency, show=True):
-    """Plot data with correct qc colour.
-
-    Parameters
-    ----------
-    base_series : pd.Series
-        Data to be sorted by colour
-    check_series : pd.Series
-        Check data to plot
-    qc_series : pd.Series
-        QC ranges for colour coding
-    frequency : DateOffset or str
-        Frequency to which the data gets set to
-    show : bool
-        Whether to show the plot directly when called
-
-    Returns
-    -------
-    None
-        Displays a plot
-    """
-    split_data = splitter(base_series, qc_series, frequency)
-    plt.figure()
-    for qc in split_data:
-        plt.plot(
-            split_data[qc].index,
-            split_data[qc],
-            label=f"QC{qc}",
-            color=qc_colour(qc),
-            marker=f"{'x' if qc==100 else '.'}",
-        )
-    plt.plot(
-        check_series.index,
-        check_series,
-        label="Check data",
-        marker="o",
-        color="gray",
-        linestyle="None",
-    )
-    plt.xticks(rotation=45, ha="right")
-
-    plt.legend()
-    if show:
-        plt.show()
-
-
-def qc_plotter_plotly(
-    base_series, check_series, qc_series, frequency, show=True, **kwargs
-):
-    """Plot data with correct qc colour.
-
-    Parameters
-    ----------
-    base_series : pd.Series
-        Data to be sorted by colour
-    check_series : pd.Series
-        Check data to plot
-    qc_series : pd.Series
-        QC ranges for colour coding
-    frequency : DateOffset or str
-        Frequency to which the data gets set to
-    show : bool
-        Whether to show the plot directly when called
-
-    Returns
-    -------
-    None
-        Displays a plot
-    """
-    split_data = splitter(base_series, qc_series, frequency)
-    fig = go.Figure()
-    for qc in split_data:
-        fig.add_trace(
-            go.Scatter(
-                x=split_data[qc].index,
-                y=split_data[qc],
-                mode="lines",
-                name=f"QC{qc}",
-                line=dict(color=qc_colour(qc)),
-            )
-        )
-    if check_series is not None:
-        fig.add_trace(
-            go.Scatter(
-                x=check_series.index,
-                y=check_series,
-                mode="markers",
-                name="Check data",
-                marker=dict(color="darkturquoise", size=10),
-            )
-        )
-    fig.update_layout(
-        title="Quality Control Plot",
-        xaxis=dict(title="Date"),
-        yaxis=dict(title="Value"),
-        legend=dict(yanchor="top", y=0.99, xanchor="left", x=0.01),
-        xaxis_tickangle=-45,
-        **kwargs,
-    )
-    if show:
-        fig.show()
-    return fig
-
-
-def comparison_qc_plotter(
-    base_series, raw_series, check_series, qc_series, frequency, show=True
-):
-    """Plot data with correct qc colour a la qc_plotter(), and the raw data overlaid.
-
-    Parameters
-    ----------
-    base_series : pd.Series
-        Data to be sorted by colour
-    raw_series : pd.Series
-        Data that has not been processed
-    check_series : pd.Series
-        Check data to plot
-    qc_series : pd.Series
-        QC ranges for colour coding
-    frequency : DateOffset or str
-        Frequency to which the data gets set to
-    show : bool
-        Whether to show the plot directly when called
-
-    Returns
-    -------
-    None
-        Displays a plot
-    """
-    qc_plotter(base_series, check_series, qc_series, frequency, show=False)
-    plt.plot(
-        raw_series.index,
-        raw_series,
-        label="Raw data",
-        color="black",
-        marker="",
-        linestyle="dashed",
-    )
-    plt.legend()
-    if show:
-        plt.show()
-
-
-def comparison_qc_plotter_plotly(
-    base_series,
-    raw_series,
-    check_series,
-    qc_series,
-    frequency,
-    show=True,
-    **kwargs,
-):
-    """Plot data with correct qc colour a la qc_plotter(), and the raw data overlaid.
-
-    Parameters
-    ----------
-    base_series : pd.Series
-        Data to be sorted by colour
-    raw_series : pd.Series
-        Data that has not been processed
-    check_series : pd.Series
-        Check data to plot
-    qc_series : pd.Series
-        QC ranges for colour coding
-    frequency : DateOffset or str
-        Frequency to which the data gets set to
-    show : bool
-        Whether to show the plot directly when called
-
-    Returns
-    -------
-    None
-        Displays a plot
-    """
-    fig = qc_plotter_plotly(
-        base_series, check_series, qc_series, frequency, show=False, **kwargs
-    )
-
-    fig.add_trace(
-        go.Scatter(
-            x=raw_series.index,
-            y=raw_series,
-            mode="lines",
-            name="Raw data",
-            line=dict(color="black", dash="dash"),
-        )
-    )
-    if show:
-        fig.show()
-    return fig
-
-
-def make_processing_dash(
-    fig,
-    title,
-    raw_standard_series,
-    hilltop_standard_series,
-    raw_check_series,
-    prov_wq,
-    inspections,
-    ncrs,
-):
-    """Make the processing dash.
-
-    Sorry about these docs I'm in a rush.
-    """
-    fig.add_trace(
-        go.Scatter(
-            x=raw_standard_series.index,
-            y=raw_standard_series.to_numpy(),
-            mode="lines",
-            name="Raw data",
-            line=dict(color="darkslategray", width=0.5),
-            opacity=0.5,
-        )
-    )
-    fig.add_trace(
-        go.Scatter(
-            x=raw_check_series.index,
-            y=raw_check_series["Water Temperature Check"],
-            mode="markers",
-            name="Check data",
-            marker=dict(color="darkturquoise", size=10),
-        )
-    )
-    fig.add_trace(
-        go.Scatter(
-            x=prov_wq.index,
-            y=prov_wq["Temp Check"],
-            mode="markers",
-            name="ProvWQ Check",
-            marker=dict(color="darkslategray", size=10, symbol="square-open"),
-        )
-    )
-    fig.add_trace(
-        go.Scatter(
-            x=inspections.index,
-            y=inspections["Temp Check"],
-            mode="markers",
-            name="S123 Check",
-            marker=dict(color="darkslategray", size=10, symbol="circle-open-dot"),
-        )
-    )
-    fig.add_trace(
-        go.Scatter(
-            x=inspections.index,
-            y=inspections["Temp Logger"],
-            mode="markers",
-            name="S123 Logger",
-            marker=dict(color="darkslategray", size=10, symbol="x-thin-open"),
-        )
-    )
-    fig_subplots = make_subplots(
-        rows=3,
-        cols=1,
-        shared_xaxes=True,
-        vertical_spacing=0.02,
-        specs=[
-            [{"type": "scatter"}],
-            [{"type": "scatter"}],
-            [{"type": "table"}],
-        ],
-        row_heights=[0.4, 0.2, 0.4],
-    )
-
-    for trace in fig.data:
-        fig_subplots.add_trace(trace, row=1, col=1)
-
-    fig_subplots.update_layout(title=title)
-
-    def find_nearest_periodic_indices(periodic_series, check_series):
-        nearest_periodic_indices = []
-        for check_index in check_series.index:
-            # Calculate the difference between the check_index and every periodic index
-            time_diff = np.abs(periodic_series.index - check_index)
-
-            # Find the index in standard_series with the minimum time difference
-            nearest_index = np.argmin(time_diff)
-
-            nearest_periodic_indices.append(nearest_index)
-
-        return nearest_periodic_indices
-
-    nearest_check_indices = find_nearest_periodic_indices(
-        hilltop_standard_series, raw_check_series["Water Temperature Check"]
-    )
-
-    nearest_prov_indices = find_nearest_periodic_indices(
-        hilltop_standard_series, prov_wq
-    )
-
-    nearest_inspection_indices = find_nearest_periodic_indices(
-        hilltop_standard_series, inspections
-    )
-
-    edited_blocks = change_blocks(raw_standard_series, hilltop_standard_series)
-
-    first_change = True
-    for change_start, change_end in edited_blocks:
-        fig_subplots.add_vrect(
-            x0=change_start,
-            x1=change_end,
-            showlegend=first_change,
-            fillcolor="blue",
-            opacity=0.25,
-            line_width=0,
-            name="Changes",
-            row=1,
-            col=1,
-        )
-        first_change = False
-
-    fig_subplots.add_trace(
-        go.Scatter(
-            x=raw_check_series["Water Temperature Check"].index,
-            y=hilltop_standard_series.iloc[nearest_check_indices].to_numpy()
-            - raw_check_series["Water Temperature Check"].to_numpy(),
-            mode="markers",
-            name="Check data",
-            marker=dict(color="darkturquoise", size=10, symbol="circle"),
-            showlegend=False,
-        ),
-        row=2,
-        col=1,
-    )
-
-    fig_subplots.add_trace(
-        go.Scatter(
-            x=hilltop_standard_series.iloc[nearest_check_indices].index,
-            y=hilltop_standard_series.iloc[nearest_check_indices].to_numpy()
-            - raw_check_series["Water Temperature Check"].to_numpy(),
-            mode="markers",
-            name="Check Align",
-            marker=dict(color="darkturquoise", size=10, symbol="circle"),
-            showlegend=False,
-            opacity=0.5,
-            hoverinfo="skip",
-        ),
-        row=2,
-        col=1,
-    )
-    arrow_annotations = []
-    for stand, check in zip(
-        hilltop_standard_series.iloc[nearest_check_indices].items(),
-        raw_check_series["Water Temperature Check"].items(),
-        strict=True,
-    ):
-        # If the timestamps are not the same
-        if stand[0] != check[0]:
-            arrow_annotations.append(
-                dict(
-                    ax=check[0],
-                    ay=stand[1] - check[1],
-                    x=stand[0],
-                    y=stand[1] - check[1],
-                    axref="x2",
-                    ayref="y2",
-                    xref="x2",
-                    yref="y2",
-                    arrowhead=2,
-                    arrowcolor="darkturquoise",
-                    showarrow=True,
-                    opacity=0.5,
-                    standoff=6,
-                )
-            )
-
-    fig_subplots.add_trace(
-        go.Scatter(
-            x=prov_wq.index,
-            y=hilltop_standard_series.iloc[nearest_prov_indices].to_numpy()
-            - prov_wq["Temp Check"].to_numpy(),
-            mode="markers",
-            name="ProvWQ Check",
-            marker=dict(color="darkslategray", size=10, symbol="square-open"),
-            showlegend=False,
-        ),
-        row=2,
-        col=1,
-    )
-    fig_subplots.add_trace(
-        go.Scatter(
-            x=hilltop_standard_series.iloc[nearest_prov_indices].index,
-            y=hilltop_standard_series.iloc[nearest_prov_indices].to_numpy()
-            - prov_wq["Temp Check"].to_numpy(),
-            mode="markers",
-            name="ProvWQ Align",
-            marker=dict(color="darkslategray", size=10, symbol="square-open"),
-            showlegend=False,
-            opacity=0.5,
-            hoverinfo="skip",
-        ),
-        row=2,
-        col=1,
-    )
-    for stand, prov in zip(
-        hilltop_standard_series.iloc[nearest_prov_indices].items(),
-        prov_wq.iterrows(),
-        strict=True,
-    ):
-        # If the timestamps are not the same
-        if stand[0] != prov[0]:
-            arrow_annotations.append(
-                dict(
-                    ax=prov[0],
-                    ay=stand[1] - prov[1]["Temp Check"],
-                    x=stand[0],
-                    y=stand[1] - prov[1]["Temp Check"],
-                    axref="x2",
-                    ayref="y2",
-                    xref="x2",
-                    yref="y2",
-                    arrowhead=2,
-                    arrowcolor="darkslategray",
-                    showarrow=True,
-                    opacity=0.5,
-                    standoff=6,
-                )
-            )
-
-    fig_subplots.add_trace(
-        go.Scatter(
-            x=inspections.index,
-            y=hilltop_standard_series.iloc[nearest_inspection_indices].to_numpy()
-            - inspections["Temp Check"].to_numpy(),
-            mode="markers",
-            name="S123 Check",
-            marker=dict(color="darkslategray", size=10, symbol="circle-open-dot"),
-            showlegend=False,
-        ),
-        row=2,
-        col=1,
-    )
-
-    fig_subplots.add_trace(
-        go.Scatter(
-            x=hilltop_standard_series.iloc[nearest_inspection_indices].index,
-            y=hilltop_standard_series.iloc[nearest_inspection_indices].to_numpy()
-            - inspections["Temp Check"].to_numpy(),
-            mode="markers",
-            name="S123 Check Aligned",
-            marker=dict(color="darkslategray", size=10, symbol="circle-open-dot"),
-            showlegend=False,
-            opacity=0.5,
-            hoverinfo="skip",
-        ),
-        row=2,
-        col=1,
-    )
-
-    for stand, insp in zip(
-        hilltop_standard_series.iloc[nearest_inspection_indices].items(),
-        inspections.iterrows(),
-        strict=True,
-    ):
-        # If the timestamps are not the same
-        if stand[0] != insp[0] and not pd.isna(insp[1]["Temp Logger"]):
-            arrow_annotations.append(
-                dict(
-                    ax=insp[0],
-                    ay=stand[1] - insp[1]["Temp Check"],
-                    x=stand[0],
-                    y=stand[1] - insp[1]["Temp Check"],
-                    axref="x2",
-                    ayref="y2",
-                    xref="x2",
-                    yref="y2",
-                    arrowhead=2,
-                    arrowcolor="darkslategray",
-                    showarrow=True,
-                    opacity=0.5,
-                    standoff=6,
-                )
-            )
-
-    fig_subplots.add_trace(
-        go.Scatter(
-            x=inspections.index,
-            y=hilltop_standard_series.iloc[nearest_inspection_indices].to_numpy()
-            - inspections["Temp Logger"].to_numpy(),
-            mode="markers",
-            name="S123 Logger",
-            marker=dict(color="darkslategray", size=10, symbol="x-thin-open"),
-            showlegend=False,
-        ),
-        row=2,
-        col=1,
-    )
-
-    fig_subplots.add_trace(
-        go.Scatter(
-            x=hilltop_standard_series.iloc[nearest_inspection_indices].index,
-            y=hilltop_standard_series.iloc[nearest_inspection_indices].to_numpy()
-            - inspections["Temp Logger"].to_numpy(),
-            mode="markers",
-            name="S123 Logger Aligned",
-            marker=dict(color="darkslategray", size=10, symbol="x-thin-open"),
-            showlegend=False,
-            opacity=0.5,
-            hoverinfo="skip",
-        ),
-        row=2,
-        col=1,
-    )
-
-    for stand, insp in zip(
-        hilltop_standard_series.iloc[nearest_inspection_indices].items(),
-        inspections.iterrows(),
-        strict=True,
-    ):
-        # If the timestamps are not the same
-        if stand[0] != insp[0] and not pd.isna(insp[1]["Temp Logger"]):
-            arrow_annotations.append(
-                dict(
-                    ax=insp[0],
-                    ay=stand[1] - insp[1]["Temp Logger"],
-                    x=stand[0],
-                    y=stand[1] - insp[1]["Temp Logger"],
-                    axref="x2",
-                    ayref="y2",
-                    xref="x2",
-                    yref="y2",
-                    arrowhead=2,
-                    arrowcolor="darkslategray",
-                    showarrow=True,
-                    opacity=0.5,
-                    standoff=6,
-                )
-            )
-
-    fig_subplots.update_layout(annotations=arrow_annotations)
-
-    qc400 = 1.2
-    qc500 = 0.8
-
-    fig_subplots.add_hline(
-        y=qc400,
-        line=dict(color="#ffa500", width=1, dash="dash"),
-        name="QC400",
-        row=2,
-        col=1,
-        showlegend=True,
-        legendgroup="QC400",
-    )
-
-    fig_subplots.add_hline(
-        y=-qc400,
-        line=dict(color="#ffa500", width=1, dash="dash"),
-        name="QC400",
-        row=2,
-        col=1,
-        showlegend=False,
-        legendgroup="QC400",
-        visible=True,
-    )
-    fig_subplots.add_hline(
-        y=qc500,
-        line=dict(color="#00bfff", width=1, dash="dash"),
-        name="QC500",
-        row=2,
-        col=1,
-        showlegend=True,
-        legendgroup="QC500",
-        visible=True,
-    )
-    fig_subplots.add_hline(
-        y=-qc500,
-        line=dict(color="#00bfff", width=1, dash="dash"),
-        name="QC500",
-        row=2,
-        col=1,
-        showlegend=False,
-        legendgroup="QC500",
-        visible=True,
-    )
-
-    all_comments = merge_all_comments(raw_check_series, prov_wq, inspections, ncrs)
-
-    fig_subplots.add_trace(
-        go.Table(
-            columnwidth=[1, 3, 1],
-            header=dict(
-                values=list(all_comments.columns),
-                align="left",
-            ),
-            cells=dict(
-                values=[all_comments[cn] for cn in all_comments.columns],
-                align="left",
-            ),
-        ),
-        row=3,
-        col=1,
-    )
-
-    fig_subplots.update_layout(
-        hovermode="x unified",
-    )
-
-    return fig_subplots
+"""Tools for displaying potentially problematic data."""
+import warnings
+
+import matplotlib.pyplot as plt
+import numpy as np
+import pandas as pd
+import plotly.graph_objects as go
+from plotly.subplots import make_subplots
+
+from hydrobot.evaluator import find_nearest_time, gap_finder, splitter
+from hydrobot.utils import change_blocks, merge_all_comments
+
+
+def gap_plotter(base_series, span=20, show=True):
+    """Plot the areas around NaN.to_numpy() to visually check for dodgy spike removal.
+
+    Parameters
+    ----------
+    base_series : pd.Series
+        Data to have the gaps found and plotted
+    span : int
+        How many points around the gap gets plotted
+    show : bool
+        Whether to show the plot directly when called
+
+    Returns
+    -------
+    None
+        Outputs a series of plots
+    """
+    for gap in gap_finder(base_series):
+        plt.figure()
+        idx = base_series.index.get_loc(gap[0])
+        lower_idx = idx - span
+        upper_idx = idx + span + gap[1]
+        if lower_idx < 0:
+            # below range
+            upper_idx -= lower_idx
+            lower_idx -= lower_idx
+        if upper_idx > len(base_series):
+            # above range
+            lower_idx -= len(base_series) - upper_idx
+            upper_idx -= len(base_series) - upper_idx
+            if lower_idx < 0:
+                # span is too big or not enough data
+                warnings.warn("Warning: Span bigger than data", stacklevel=2)
+                lower_idx = 0
+        gap_range = base_series.iloc[lower_idx:upper_idx]
+        plt.plot(gap_range.index, gap_range)
+        plt.title(f"Gap starting at {gap[0]}")
+    if show:
+        plt.show()
+
+
+def check_plotter(base_series, check_series, span=20, show=True):
+    """Plot the areas around check.to_numpy() to visually check for dodgy data from inspections.
+
+    Parameters
+    ----------
+    base_series : pd.Series
+        Data to plot
+    check_series : pd.Series
+        Check data which determines where the data is plotted
+    span : int
+        How much space around the check data is shown
+    show : bool
+        Whether to show the plot directly when called
+
+    Returns
+    -------
+    None
+        Outputs a series of plots
+
+    """
+    for check in check_series.index:
+        plt.figure()
+        idx = base_series.index.get_loc(find_nearest_time(base_series, check))
+        lower_idx = idx - span
+        upper_idx = idx + span
+        if lower_idx < 0:
+            # below range
+            upper_idx -= lower_idx
+            lower_idx -= lower_idx
+        if upper_idx > len(base_series):
+            # above range
+            lower_idx -= len(base_series) - upper_idx
+            upper_idx -= len(base_series) - upper_idx
+            if lower_idx < 0:
+                # span is too big or not enough data
+                warnings.warn("Warning: Span bigger than data", stacklevel=2)
+                lower_idx = 0
+        gap_range = base_series.iloc[lower_idx:upper_idx]
+        plt.plot(gap_range.index, gap_range)
+        plt.plot(
+            check,
+            check_series[check],
+            label="Check data",
+            marker="o",
+            color="darkturquoise",
+        )
+        plt.title(f"Check at {check}")
+    if show:
+        plt.show()
+
+
+def qc_colour(qc):
+    """Give the colour of the QC.
+
+    Parameters
+    ----------
+    qc : int
+        Quality code
+
+    Returns
+    -------
+    String
+        Hex code for the colour of the QC
+    """
+    qc_dict = {
+        None: "darkslategrey",
+        "nan": "darkslategrey",
+        0: "#9900ff",
+        100: "#ff0000",
+        200: "#8B5A00",
+        300: "#d3d3d3",
+        400: "#ffa500",
+        500: "#00bfff",
+        600: "#006400",
+    }
+    return qc_dict[qc]
+
+
+def qc_plotter(base_series, check_series, qc_series, frequency, show=True):
+    """Plot data with correct qc colour.
+
+    Parameters
+    ----------
+    base_series : pd.Series
+        Data to be sorted by colour
+    check_series : pd.Series
+        Check data to plot
+    qc_series : pd.Series
+        QC ranges for colour coding
+    frequency : DateOffset or str
+        Frequency to which the data gets set to
+    show : bool
+        Whether to show the plot directly when called
+
+    Returns
+    -------
+    None
+        Displays a plot
+    """
+    split_data = splitter(base_series, qc_series, frequency)
+    plt.figure()
+    for qc in split_data:
+        plt.plot(
+            split_data[qc].index,
+            split_data[qc],
+            label=f"QC{qc}",
+            color=qc_colour(qc),
+            marker=f"{'x' if qc==100 else '.'}",
+        )
+    plt.plot(
+        check_series.index,
+        check_series,
+        label="Check data",
+        marker="o",
+        color="gray",
+        linestyle="None",
+    )
+    plt.xticks(rotation=45, ha="right")
+
+    plt.legend()
+    if show:
+        plt.show()
+
+
+def qc_plotter_plotly(
+    base_series, check_series, qc_series, frequency, show=True, **kwargs
+):
+    """Plot data with correct qc colour.
+
+    Parameters
+    ----------
+    base_series : pd.Series
+        Data to be sorted by colour
+    check_series : pd.Series
+        Check data to plot
+    qc_series : pd.Series
+        QC ranges for colour coding
+    frequency : DateOffset or str
+        Frequency to which the data gets set to
+    show : bool
+        Whether to show the plot directly when called
+
+    Returns
+    -------
+    None
+        Displays a plot
+    """
+    split_data = splitter(base_series, qc_series, frequency)
+    fig = go.Figure()
+    for qc in split_data:
+        fig.add_trace(
+            go.Scatter(
+                x=split_data[qc].index,
+                y=split_data[qc],
+                mode="lines",
+                name=f"QC{qc}",
+                line=dict(color=qc_colour(qc)),
+            )
+        )
+    if check_series is not None:
+        fig.add_trace(
+            go.Scatter(
+                x=check_series.index,
+                y=check_series,
+                mode="markers",
+                name="Check data",
+                marker=dict(color="darkturquoise", size=10),
+            )
+        )
+    fig.update_layout(
+        title="Quality Control Plot",
+        xaxis=dict(title="Date"),
+        yaxis=dict(title="Value"),
+        legend=dict(yanchor="top", y=0.99, xanchor="left", x=0.01),
+        xaxis_tickangle=-45,
+        **kwargs,
+    )
+    if show:
+        fig.show()
+    return fig
+
+
+def comparison_qc_plotter(
+    base_series, raw_series, check_series, qc_series, frequency, show=True
+):
+    """Plot data with correct qc colour a la qc_plotter(), and the raw data overlaid.
+
+    Parameters
+    ----------
+    base_series : pd.Series
+        Data to be sorted by colour
+    raw_series : pd.Series
+        Data that has not been processed
+    check_series : pd.Series
+        Check data to plot
+    qc_series : pd.Series
+        QC ranges for colour coding
+    frequency : DateOffset or str
+        Frequency to which the data gets set to
+    show : bool
+        Whether to show the plot directly when called
+
+    Returns
+    -------
+    None
+        Displays a plot
+    """
+    qc_plotter(base_series, check_series, qc_series, frequency, show=False)
+    plt.plot(
+        raw_series.index,
+        raw_series,
+        label="Raw data",
+        color="black",
+        marker="",
+        linestyle="dashed",
+    )
+    plt.legend()
+    if show:
+        plt.show()
+
+
+def comparison_qc_plotter_plotly(
+    base_series,
+    raw_series,
+    check_series,
+    qc_series,
+    frequency,
+    show=True,
+    **kwargs,
+):
+    """Plot data with correct qc colour a la qc_plotter(), and the raw data overlaid.
+
+    Parameters
+    ----------
+    base_series : pd.Series
+        Data to be sorted by colour
+    raw_series : pd.Series
+        Data that has not been processed
+    check_series : pd.Series
+        Check data to plot
+    qc_series : pd.Series
+        QC ranges for colour coding
+    frequency : DateOffset or str
+        Frequency to which the data gets set to
+    show : bool
+        Whether to show the plot directly when called
+
+    Returns
+    -------
+    None
+        Displays a plot
+    """
+    fig = qc_plotter_plotly(
+        base_series, check_series, qc_series, frequency, show=False, **kwargs
+    )
+
+    fig.add_trace(
+        go.Scatter(
+            x=raw_series.index,
+            y=raw_series,
+            mode="lines",
+            name="Raw data",
+            line=dict(color="black", dash="dash"),
+        )
+    )
+    if show:
+        fig.show()
+    return fig
+
+
+def make_processing_dash(
+    fig,
+    title,
+    raw_standard_series,
+    hilltop_standard_series,
+    raw_check_series,
+    prov_wq,
+    inspections,
+    ncrs,
+):
+    """Make the processing dash.
+
+    Sorry about these docs I'm in a rush.
+    """
+    fig.add_trace(
+        go.Scatter(
+            x=raw_standard_series.index,
+            y=raw_standard_series.to_numpy(),
+            mode="lines",
+            name="Raw data",
+            line=dict(color="darkslategray", width=0.5),
+            opacity=0.5,
+        )
+    )
+    fig.add_trace(
+        go.Scatter(
+            x=raw_check_series.index,
+            y=raw_check_series["Water Temperature Check"],
+            mode="markers",
+            name="Check data",
+            marker=dict(color="darkturquoise", size=10),
+        )
+    )
+    fig.add_trace(
+        go.Scatter(
+            x=prov_wq.index,
+            y=prov_wq["Temp Check"],
+            mode="markers",
+            name="ProvWQ Check",
+            marker=dict(color="darkslategray", size=10, symbol="square-open"),
+        )
+    )
+    fig.add_trace(
+        go.Scatter(
+            x=inspections.index,
+            y=inspections["Temp Check"],
+            mode="markers",
+            name="S123 Check",
+            marker=dict(color="darkslategray", size=10, symbol="circle-open-dot"),
+        )
+    )
+    fig.add_trace(
+        go.Scatter(
+            x=inspections.index,
+            y=inspections["Temp Logger"],
+            mode="markers",
+            name="S123 Logger",
+            marker=dict(color="darkslategray", size=10, symbol="x-thin-open"),
+        )
+    )
+    fig_subplots = make_subplots(
+        rows=3,
+        cols=1,
+        shared_xaxes=True,
+        vertical_spacing=0.02,
+        specs=[
+            [{"type": "scatter"}],
+            [{"type": "scatter"}],
+            [{"type": "table"}],
+        ],
+        row_heights=[0.4, 0.2, 0.4],
+    )
+
+    for trace in fig.data:
+        fig_subplots.add_trace(trace, row=1, col=1)
+
+    fig_subplots.update_layout(title=title)
+
+    def find_nearest_periodic_indices(periodic_series, check_series):
+        nearest_periodic_indices = []
+        for check_index in check_series.index:
+            # Calculate the difference between the check_index and every periodic index
+            time_diff = np.abs(periodic_series.index - check_index)
+
+            # Find the index in standard_series with the minimum time difference
+            nearest_index = np.argmin(time_diff)
+
+            nearest_periodic_indices.append(nearest_index)
+
+        return nearest_periodic_indices
+
+    nearest_check_indices = find_nearest_periodic_indices(
+        hilltop_standard_series, raw_check_series["Water Temperature Check"]
+    )
+
+    nearest_prov_indices = find_nearest_periodic_indices(
+        hilltop_standard_series, prov_wq
+    )
+
+    nearest_inspection_indices = find_nearest_periodic_indices(
+        hilltop_standard_series, inspections
+    )
+
+    edited_blocks = change_blocks(raw_standard_series, hilltop_standard_series)
+
+    first_change = True
+    for change_start, change_end in edited_blocks:
+        fig_subplots.add_vrect(
+            x0=change_start,
+            x1=change_end,
+            showlegend=first_change,
+            fillcolor="blue",
+            opacity=0.25,
+            line_width=0,
+            name="Changes",
+            row=1,
+            col=1,
+        )
+        first_change = False
+
+    fig_subplots.add_trace(
+        go.Scatter(
+            x=raw_check_series["Water Temperature Check"].index,
+            y=hilltop_standard_series.iloc[nearest_check_indices].to_numpy()
+            - raw_check_series["Water Temperature Check"].to_numpy(),
+            mode="markers",
+            name="Check data",
+            marker=dict(color="darkturquoise", size=10, symbol="circle"),
+            showlegend=False,
+        ),
+        row=2,
+        col=1,
+    )
+
+    fig_subplots.add_trace(
+        go.Scatter(
+            x=hilltop_standard_series.iloc[nearest_check_indices].index,
+            y=hilltop_standard_series.iloc[nearest_check_indices].to_numpy()
+            - raw_check_series["Water Temperature Check"].to_numpy(),
+            mode="markers",
+            name="Check Align",
+            marker=dict(color="darkturquoise", size=10, symbol="circle"),
+            showlegend=False,
+            opacity=0.5,
+            hoverinfo="skip",
+        ),
+        row=2,
+        col=1,
+    )
+    arrow_annotations = []
+    for stand, check in zip(
+        hilltop_standard_series.iloc[nearest_check_indices].items(),
+        raw_check_series["Water Temperature Check"].items(),
+        strict=True,
+    ):
+        # If the timestamps are not the same
+        if stand[0] != check[0]:
+            arrow_annotations.append(
+                dict(
+                    ax=check[0],
+                    ay=stand[1] - check[1],
+                    x=stand[0],
+                    y=stand[1] - check[1],
+                    axref="x2",
+                    ayref="y2",
+                    xref="x2",
+                    yref="y2",
+                    arrowhead=2,
+                    arrowcolor="darkturquoise",
+                    showarrow=True,
+                    opacity=0.5,
+                    standoff=6,
+                )
+            )
+
+    fig_subplots.add_trace(
+        go.Scatter(
+            x=prov_wq.index,
+            y=hilltop_standard_series.iloc[nearest_prov_indices].to_numpy()
+            - prov_wq["Temp Check"].to_numpy(),
+            mode="markers",
+            name="ProvWQ Check",
+            marker=dict(color="darkslategray", size=10, symbol="square-open"),
+            showlegend=False,
+        ),
+        row=2,
+        col=1,
+    )
+    fig_subplots.add_trace(
+        go.Scatter(
+            x=hilltop_standard_series.iloc[nearest_prov_indices].index,
+            y=hilltop_standard_series.iloc[nearest_prov_indices].to_numpy()
+            - prov_wq["Temp Check"].to_numpy(),
+            mode="markers",
+            name="ProvWQ Align",
+            marker=dict(color="darkslategray", size=10, symbol="square-open"),
+            showlegend=False,
+            opacity=0.5,
+            hoverinfo="skip",
+        ),
+        row=2,
+        col=1,
+    )
+    for stand, prov in zip(
+        hilltop_standard_series.iloc[nearest_prov_indices].items(),
+        prov_wq.iterrows(),
+        strict=True,
+    ):
+        # If the timestamps are not the same
+        if stand[0] != prov[0]:
+            arrow_annotations.append(
+                dict(
+                    ax=prov[0],
+                    ay=stand[1] - prov[1]["Temp Check"],
+                    x=stand[0],
+                    y=stand[1] - prov[1]["Temp Check"],
+                    axref="x2",
+                    ayref="y2",
+                    xref="x2",
+                    yref="y2",
+                    arrowhead=2,
+                    arrowcolor="darkslategray",
+                    showarrow=True,
+                    opacity=0.5,
+                    standoff=6,
+                )
+            )
+
+    fig_subplots.add_trace(
+        go.Scatter(
+            x=inspections.index,
+            y=hilltop_standard_series.iloc[nearest_inspection_indices].to_numpy()
+            - inspections["Temp Check"].to_numpy(),
+            mode="markers",
+            name="S123 Check",
+            marker=dict(color="darkslategray", size=10, symbol="circle-open-dot"),
+            showlegend=False,
+        ),
+        row=2,
+        col=1,
+    )
+
+    fig_subplots.add_trace(
+        go.Scatter(
+            x=hilltop_standard_series.iloc[nearest_inspection_indices].index,
+            y=hilltop_standard_series.iloc[nearest_inspection_indices].to_numpy()
+            - inspections["Temp Check"].to_numpy(),
+            mode="markers",
+            name="S123 Check Aligned",
+            marker=dict(color="darkslategray", size=10, symbol="circle-open-dot"),
+            showlegend=False,
+            opacity=0.5,
+            hoverinfo="skip",
+        ),
+        row=2,
+        col=1,
+    )
+
+    for stand, insp in zip(
+        hilltop_standard_series.iloc[nearest_inspection_indices].items(),
+        inspections.iterrows(),
+        strict=True,
+    ):
+        # If the timestamps are not the same
+        if stand[0] != insp[0] and not pd.isna(insp[1]["Temp Logger"]):
+            arrow_annotations.append(
+                dict(
+                    ax=insp[0],
+                    ay=stand[1] - insp[1]["Temp Check"],
+                    x=stand[0],
+                    y=stand[1] - insp[1]["Temp Check"],
+                    axref="x2",
+                    ayref="y2",
+                    xref="x2",
+                    yref="y2",
+                    arrowhead=2,
+                    arrowcolor="darkslategray",
+                    showarrow=True,
+                    opacity=0.5,
+                    standoff=6,
+                )
+            )
+
+    fig_subplots.add_trace(
+        go.Scatter(
+            x=inspections.index,
+            y=hilltop_standard_series.iloc[nearest_inspection_indices].to_numpy()
+            - inspections["Temp Logger"].to_numpy(),
+            mode="markers",
+            name="S123 Logger",
+            marker=dict(color="darkslategray", size=10, symbol="x-thin-open"),
+            showlegend=False,
+        ),
+        row=2,
+        col=1,
+    )
+
+    fig_subplots.add_trace(
+        go.Scatter(
+            x=hilltop_standard_series.iloc[nearest_inspection_indices].index,
+            y=hilltop_standard_series.iloc[nearest_inspection_indices].to_numpy()
+            - inspections["Temp Logger"].to_numpy(),
+            mode="markers",
+            name="S123 Logger Aligned",
+            marker=dict(color="darkslategray", size=10, symbol="x-thin-open"),
+            showlegend=False,
+            opacity=0.5,
+            hoverinfo="skip",
+        ),
+        row=2,
+        col=1,
+    )
+
+    for stand, insp in zip(
+        hilltop_standard_series.iloc[nearest_inspection_indices].items(),
+        inspections.iterrows(),
+        strict=True,
+    ):
+        # If the timestamps are not the same
+        if stand[0] != insp[0] and not pd.isna(insp[1]["Temp Logger"]):
+            arrow_annotations.append(
+                dict(
+                    ax=insp[0],
+                    ay=stand[1] - insp[1]["Temp Logger"],
+                    x=stand[0],
+                    y=stand[1] - insp[1]["Temp Logger"],
+                    axref="x2",
+                    ayref="y2",
+                    xref="x2",
+                    yref="y2",
+                    arrowhead=2,
+                    arrowcolor="darkslategray",
+                    showarrow=True,
+                    opacity=0.5,
+                    standoff=6,
+                )
+            )
+
+    fig_subplots.update_layout(annotations=arrow_annotations)
+
+    qc400 = 1.2
+    qc500 = 0.8
+
+    fig_subplots.add_hline(
+        y=qc400,
+        line=dict(color="#ffa500", width=1, dash="dash"),
+        name="QC400",
+        row=2,
+        col=1,
+        showlegend=True,
+        legendgroup="QC400",
+    )
+
+    fig_subplots.add_hline(
+        y=-qc400,
+        line=dict(color="#ffa500", width=1, dash="dash"),
+        name="QC400",
+        row=2,
+        col=1,
+        showlegend=False,
+        legendgroup="QC400",
+        visible=True,
+    )
+    fig_subplots.add_hline(
+        y=qc500,
+        line=dict(color="#00bfff", width=1, dash="dash"),
+        name="QC500",
+        row=2,
+        col=1,
+        showlegend=True,
+        legendgroup="QC500",
+        visible=True,
+    )
+    fig_subplots.add_hline(
+        y=-qc500,
+        line=dict(color="#00bfff", width=1, dash="dash"),
+        name="QC500",
+        row=2,
+        col=1,
+        showlegend=False,
+        legendgroup="QC500",
+        visible=True,
+    )
+
+    all_comments = merge_all_comments(raw_check_series, prov_wq, inspections, ncrs)
+
+    fig_subplots.add_trace(
+        go.Table(
+            columnwidth=[1, 3, 1],
+            header=dict(
+                values=list(all_comments.columns),
+                align="left",
+            ),
+            cells=dict(
+                values=[all_comments[cn] for cn in all_comments.columns],
+                align="left",
+            ),
+        ),
+        row=3,
+        col=1,
+    )
+
+    fig_subplots.update_layout(
+        hovermode="x unified",
+    )
+
+    return fig_subplots
```

### Comparing `hydrobot-0.5.0/hydrobot/utils.py` & `hydrobot-0.5.1/hydrobot/utils.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,256 +1,256 @@
-"""General utilities."""
-
-import numpy as np
-import pandas as pd
-
-MOWSECS_OFFSET = 946771200
-
-
-def mowsecs_to_timestamp(mowsecs):
-    """
-    Convert MOWSECS (Ministry of Works Seconds) index to datetime index.
-
-    Parameters
-    ----------
-    index : pd.Index
-        The input index in MOWSECS format.
-
-    Returns
-    -------
-    pd.DatetimeIndex
-        The converted datetime index.
-
-    Notes
-    -----
-    This function takes an index representing time in Ministry of Works Seconds
-    (MOWSECS) format and converts it to a pandas DatetimeIndex.
-
-    Examples
-    --------
-    >>> mowsecs_index = pd.Index([0, 1440, 2880], name="Time")
-    >>> converted_index = mowsecs_to_datetime_index(mowsecs_index)
-    >>> isinstance(converted_index, pd.DatetimeIndex)
-    True
-    """
-    try:
-        mowsec_time = int(mowsecs)
-    except ValueError as e:
-        raise TypeError("Expected something that is parseable as an integer") from e
-
-    unix_time = mowsec_time - MOWSECS_OFFSET
-    timestamp = pd.Timestamp(unix_time, unit="s")
-    return timestamp
-
-
-def timestamp_to_mowsecs(timestamp):
-    """
-    Convert MOWSECS (Ministry of Works Seconds) index to datetime index.
-
-    Parameters
-    ----------
-    index : pd.Index
-        The input index in MOWSECS format.
-
-    Returns
-    -------
-    pd.DatetimeIndex
-        The converted datetime index.
-
-    Notes
-    -----
-    This function takes an index representing time in Ministry of Works Seconds
-    (MOWSECS) format and converts it to a pandas DatetimeIndex.
-
-    Examples
-    --------
-    >>> mowsecs_index = pd.Index([0, 1440, 2880], name="Time")
-    >>> converted_index = mowsecs_to_datetime_index(mowsecs_index)
-    >>> isinstance(converted_index, pd.DatetimeIndex)
-    True
-    """
-    try:
-        timestamp = pd.Timestamp(timestamp)
-    except ValueError as e:
-        raise TypeError("Expected something that is parseable as an integer") from e
-
-    return int((timestamp.timestamp()) + MOWSECS_OFFSET)
-
-
-def mowsecs_to_datetime_index(index):
-    """
-    Convert MOWSECS (Ministry of Works Seconds) index to datetime index.
-
-    Parameters
-    ----------
-    index : pd.Index
-        The input index in MOWSECS format.
-
-    Returns
-    -------
-    pd.DatetimeIndex
-        The converted datetime index.
-
-    Notes
-    -----
-    This function takes an index representing time in Ministry of Works Seconds
-    (MOWSECS) format and converts it to a pandas DatetimeIndex.
-
-    Examples
-    --------
-    >>> mowsecs_index = pd.Index([0, 1440, 2880], name="Time")
-    >>> converted_index = mowsecs_to_datetime_index(mowsecs_index)
-    >>> isinstance(converted_index, pd.DatetimeIndex)
-    True
-    """
-    try:
-        mowsec_time = index.astype(np.int64)
-    except ValueError as e:
-        raise TypeError("These don't look like mowsecs. Expecting an integer.") from e
-    unix_time = mowsec_time.map(lambda x: x - MOWSECS_OFFSET)
-    timestamps = unix_time.map(
-        lambda x: pd.Timestamp(x, unit="s") if x is not None else None
-    )
-    datetime_index = pd.to_datetime(timestamps)
-    return datetime_index
-
-
-def datetime_index_to_mowsecs(index):
-    """
-    Convert datetime index to MOWSECS (Ministry of Works Seconds).
-
-    Parameters
-    ----------
-    index : pd.DatetimeIndex
-        The input datetime index.
-
-    Returns
-    -------
-    pd.Index
-        The converted MOWSECS index.
-
-    Notes
-    -----
-    This function takes a pandas DatetimeIndex and converts it to an index
-    representing time in Ministry of Works Seconds (MOWSECS) format.
-
-    Examples
-    --------
-    >>> datetime_index = pd.date_range("2023-01-01", periods=3, freq="D")
-    >>> mowsecs_index = datetime_index_to_mowsecs(datetime_index)
-    >>> isinstance(mowsecs_index, pd.Index)
-    True
-    """
-    return (index.astype(np.int64) // 10**9) + MOWSECS_OFFSET
-
-
-def merge_series(series_a, series_b, tolerance=1e-09):
-    """
-    Combine two series which contain partial elements of the same dataset.
-
-    For series 1:a, 2:b and series 1:a, 3:c, will give 1:a, 2:b, 3:c
-
-    Will give an error if series contains contradicting data
-
-    If difference in data is smaller than tolerance, the values of the first series are used
-
-    Parameters
-    ----------
-    series_a : pd.Series
-        One series to combine (preferred when differences are below tolerance)
-    series_b : pd.Series
-        Second series to combine (overwritten when differences are below tolerance)
-    tolerance : numeric
-        Maximum allowed difference between the two series for the same timestamp
-
-    Returns
-    -------
-    pd.Series
-        Combined series
-    """
-    combined = series_a.combine_first(series_b)
-    diff = abs(series_b.combine_first(series_a) - combined)
-    if max(diff) > tolerance:
-        raise ValueError
-    else:
-        return combined
-
-
-def change_blocks(raw_series, changed_series):
-    """Find all changes between two series."""
-    changed_block_list = []
-    start_index = None
-
-    raw_iter = iter(raw_series.items())
-    changed_iter = iter(changed_series.items())
-    raw_next = next(raw_iter, None)
-    changed_next = next(changed_iter, None)
-
-    while raw_next is not None or changed_next is not None:
-        raw_date, raw_val = raw_next if raw_next else (None, None)
-        changed_date, changed_val = changed_next if changed_next else (None, None)
-
-        if raw_date != changed_date:
-            # If one series has a timestamp that the other doesn't, treat it as a change
-            # Change block goes from the raw timestamp that is missing in the edit to the
-            # next value in the edit, i.e the entire gap.
-            if start_index is None:
-                start_index = raw_date
-        elif raw_val != changed_val:
-            # If the values at the same timestamp are different, treat it as a change
-            if start_index is None:
-                # Start of a changed block
-                start_index = raw_date
-        else:
-            if start_index is not None:
-                # End of a changed block
-                changed_block_list.append((start_index, raw_date))
-                start_index = None
-
-        # Move to the next timestamp in each series
-        if raw_date == changed_date:
-            raw_next = next(raw_iter, None)
-            changed_next = next(changed_iter, None)
-        elif (raw_date is None) or raw_date < changed_date:
-            raw_next = next(raw_iter, None)
-        else:
-            changed_next = next(changed_iter, None)
-
-    if start_index is not None:
-        changed_block_list.append((start_index, raw_series.index[-1]))
-
-    return changed_block_list
-
-
-def merge_all_comments(hill_checks, pwq_checks, s123_checks, ncrs):
-    """Merge all comments coming in from various sources.
-
-    Sorry, not sure where to put this.
-    """
-    hill_checks = hill_checks.rename(columns={"Water Temperature Check": "Temp Check"})
-    hill_checks = hill_checks.reset_index()
-    pwq_checks = pwq_checks.reset_index()
-    s123_checks = s123_checks.reset_index()
-    ncrs = ncrs.reset_index()
-
-    hill_checks["Source"] = "Hilltop Check Data"
-    pwq_checks["Source"] = "Provisional Water Quality"
-    s123_checks["Source"] = "Survey123 Inspections"
-    ncrs["Source"] = "Non-conformance Reports"
-
-    all_comments = pd.concat(
-        [
-            hill_checks[["Time", "Comment", "Source"]],
-            pwq_checks[["Time", "Comment", "Source"]],
-            s123_checks[["Time", "Comment", "Source"]],
-            ncrs[["Time", "Comment", "Source"]],
-        ],
-        ignore_index=True,
-        sort=False,
-    )
-    all_comments = all_comments.dropna(axis=1, how="all")
-
-    all_comments["Time"] = all_comments["Time"].dt.strftime("%Y-%m-%d %H:%M:%S")
-
-    all_comments = all_comments.sort_values(by="Time")
-
-    return all_comments
+"""General utilities."""
+
+import numpy as np
+import pandas as pd
+
+MOWSECS_OFFSET = 946771200
+
+
+def mowsecs_to_timestamp(mowsecs):
+    """
+    Convert MOWSECS (Ministry of Works Seconds) index to datetime index.
+
+    Parameters
+    ----------
+    index : pd.Index
+        The input index in MOWSECS format.
+
+    Returns
+    -------
+    pd.DatetimeIndex
+        The converted datetime index.
+
+    Notes
+    -----
+    This function takes an index representing time in Ministry of Works Seconds
+    (MOWSECS) format and converts it to a pandas DatetimeIndex.
+
+    Examples
+    --------
+    >>> mowsecs_index = pd.Index([0, 1440, 2880], name="Time")
+    >>> converted_index = mowsecs_to_datetime_index(mowsecs_index)
+    >>> isinstance(converted_index, pd.DatetimeIndex)
+    True
+    """
+    try:
+        mowsec_time = int(mowsecs)
+    except ValueError as e:
+        raise TypeError("Expected something that is parseable as an integer") from e
+
+    unix_time = mowsec_time - MOWSECS_OFFSET
+    timestamp = pd.Timestamp(unix_time, unit="s")
+    return timestamp
+
+
+def timestamp_to_mowsecs(timestamp):
+    """
+    Convert MOWSECS (Ministry of Works Seconds) index to datetime index.
+
+    Parameters
+    ----------
+    index : pd.Index
+        The input index in MOWSECS format.
+
+    Returns
+    -------
+    pd.DatetimeIndex
+        The converted datetime index.
+
+    Notes
+    -----
+    This function takes an index representing time in Ministry of Works Seconds
+    (MOWSECS) format and converts it to a pandas DatetimeIndex.
+
+    Examples
+    --------
+    >>> mowsecs_index = pd.Index([0, 1440, 2880], name="Time")
+    >>> converted_index = mowsecs_to_datetime_index(mowsecs_index)
+    >>> isinstance(converted_index, pd.DatetimeIndex)
+    True
+    """
+    try:
+        timestamp = pd.Timestamp(timestamp)
+    except ValueError as e:
+        raise TypeError("Expected something that is parseable as an integer") from e
+
+    return int((timestamp.timestamp()) + MOWSECS_OFFSET)
+
+
+def mowsecs_to_datetime_index(index):
+    """
+    Convert MOWSECS (Ministry of Works Seconds) index to datetime index.
+
+    Parameters
+    ----------
+    index : pd.Index
+        The input index in MOWSECS format.
+
+    Returns
+    -------
+    pd.DatetimeIndex
+        The converted datetime index.
+
+    Notes
+    -----
+    This function takes an index representing time in Ministry of Works Seconds
+    (MOWSECS) format and converts it to a pandas DatetimeIndex.
+
+    Examples
+    --------
+    >>> mowsecs_index = pd.Index([0, 1440, 2880], name="Time")
+    >>> converted_index = mowsecs_to_datetime_index(mowsecs_index)
+    >>> isinstance(converted_index, pd.DatetimeIndex)
+    True
+    """
+    try:
+        mowsec_time = index.astype(np.int64)
+    except ValueError as e:
+        raise TypeError("These don't look like mowsecs. Expecting an integer.") from e
+    unix_time = mowsec_time.map(lambda x: x - MOWSECS_OFFSET)
+    timestamps = unix_time.map(
+        lambda x: pd.Timestamp(x, unit="s") if x is not None else None
+    )
+    datetime_index = pd.to_datetime(timestamps)
+    return datetime_index
+
+
+def datetime_index_to_mowsecs(index):
+    """
+    Convert datetime index to MOWSECS (Ministry of Works Seconds).
+
+    Parameters
+    ----------
+    index : pd.DatetimeIndex
+        The input datetime index.
+
+    Returns
+    -------
+    pd.Index
+        The converted MOWSECS index.
+
+    Notes
+    -----
+    This function takes a pandas DatetimeIndex and converts it to an index
+    representing time in Ministry of Works Seconds (MOWSECS) format.
+
+    Examples
+    --------
+    >>> datetime_index = pd.date_range("2023-01-01", periods=3, freq="D")
+    >>> mowsecs_index = datetime_index_to_mowsecs(datetime_index)
+    >>> isinstance(mowsecs_index, pd.Index)
+    True
+    """
+    return (index.astype(np.int64) // 10**9) + MOWSECS_OFFSET
+
+
+def merge_series(series_a, series_b, tolerance=1e-09):
+    """
+    Combine two series which contain partial elements of the same dataset.
+
+    For series 1:a, 2:b and series 1:a, 3:c, will give 1:a, 2:b, 3:c
+
+    Will give an error if series contains contradicting data
+
+    If difference in data is smaller than tolerance, the values of the first series are used
+
+    Parameters
+    ----------
+    series_a : pd.Series
+        One series to combine (preferred when differences are below tolerance)
+    series_b : pd.Series
+        Second series to combine (overwritten when differences are below tolerance)
+    tolerance : numeric
+        Maximum allowed difference between the two series for the same timestamp
+
+    Returns
+    -------
+    pd.Series
+        Combined series
+    """
+    combined = series_a.combine_first(series_b)
+    diff = abs(series_b.combine_first(series_a) - combined)
+    if max(diff) > tolerance:
+        raise ValueError
+    else:
+        return combined
+
+
+def change_blocks(raw_series, changed_series):
+    """Find all changes between two series."""
+    changed_block_list = []
+    start_index = None
+
+    raw_iter = iter(raw_series.items())
+    changed_iter = iter(changed_series.items())
+    raw_next = next(raw_iter, None)
+    changed_next = next(changed_iter, None)
+
+    while raw_next is not None or changed_next is not None:
+        raw_date, raw_val = raw_next if raw_next else (None, None)
+        changed_date, changed_val = changed_next if changed_next else (None, None)
+
+        if raw_date != changed_date:
+            # If one series has a timestamp that the other doesn't, treat it as a change
+            # Change block goes from the raw timestamp that is missing in the edit to the
+            # next value in the edit, i.e the entire gap.
+            if start_index is None:
+                start_index = raw_date
+        elif raw_val != changed_val:
+            # If the values at the same timestamp are different, treat it as a change
+            if start_index is None:
+                # Start of a changed block
+                start_index = raw_date
+        else:
+            if start_index is not None:
+                # End of a changed block
+                changed_block_list.append((start_index, raw_date))
+                start_index = None
+
+        # Move to the next timestamp in each series
+        if raw_date == changed_date:
+            raw_next = next(raw_iter, None)
+            changed_next = next(changed_iter, None)
+        elif (raw_date is None) or raw_date < changed_date:
+            raw_next = next(raw_iter, None)
+        else:
+            changed_next = next(changed_iter, None)
+
+    if start_index is not None:
+        changed_block_list.append((start_index, raw_series.index[-1]))
+
+    return changed_block_list
+
+
+def merge_all_comments(hill_checks, pwq_checks, s123_checks, ncrs):
+    """Merge all comments coming in from various sources.
+
+    Sorry, not sure where to put this.
+    """
+    hill_checks = hill_checks.rename(columns={"Water Temperature Check": "Temp Check"})
+    hill_checks = hill_checks.reset_index()
+    pwq_checks = pwq_checks.reset_index()
+    s123_checks = s123_checks.reset_index()
+    ncrs = ncrs.reset_index()
+
+    hill_checks["Source"] = "Hilltop Check Data"
+    pwq_checks["Source"] = "Provisional Water Quality"
+    s123_checks["Source"] = "Survey123 Inspections"
+    ncrs["Source"] = "Non-conformance Reports"
+
+    all_comments = pd.concat(
+        [
+            hill_checks[["Time", "Comment", "Source"]],
+            pwq_checks[["Time", "Comment", "Source"]],
+            s123_checks[["Time", "Comment", "Source"]],
+            ncrs[["Time", "Comment", "Source"]],
+        ],
+        ignore_index=True,
+        sort=False,
+    )
+    all_comments = all_comments.dropna(axis=1, how="all")
+
+    all_comments["Time"] = all_comments["Time"].dt.strftime("%Y-%m-%d %H:%M:%S")
+
+    all_comments = all_comments.sort_values(by="Time")
+
+    return all_comments
```

### Comparing `hydrobot-0.5.0/hydrobot.egg-info/PKG-INFO` & `hydrobot-0.5.1/hydrobot.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,143 +1,155 @@
-Metadata-Version: 2.1
-Name: hydrobot
-Version: 0.5.0
-Summary: A suite of processing tools for Hilltop hydrological data.
-Author-email: Nic Mostert <nicolas.mostert@horizons.govt.nz>, Sam Irvine <sam.irvine@horizons.govt.nz>
-License: GNU General Public License v3
-Project-URL: Homepage, https://github.com/HorizonsRC/hydrobot
-Project-URL: Issues, https://github.com/HorizonsRC/hydrobot/issues
-Project-URL: Documentation, https://hydrobot.readthedocs.io
-Project-URL: Package, https://pypi.org/project/hydrobot
-Keywords: hydrology, automation, pandas, hilltop, hilltop-py, HorizonsRC
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: ==3.11.*
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-License-File: AUTHORS.rst
-Requires-Dist: hilltop-py>=2.3.1
-Requires-Dist: data-annalist>=0.4.1
-Requires-Dist: matplotlib>=3.8.0
-Requires-Dist: defusedxml>=0.7.1
-Requires-Dist: plotly>=5.20.0
-Provides-Extra: test
-Requires-Dist: pytest>=7.4.2; extra == "test"
-Requires-Dist: pytest-cov>=4.1.0; extra == "test"
-Requires-Dist: pytest-dependency>=0.5.1; extra == "test"
-Requires-Dist: pytest-mock>=3.12.0; extra == "test"
-Provides-Extra: dev
-Requires-Dist: ruff>=0.1.6; extra == "dev"
-Requires-Dist: ruff-lsp>=0.0.45; extra == "dev"
-Requires-Dist: pre-commit>=3.5.0; extra == "dev"
-Requires-Dist: build>=1.0.0; extra == "dev"
-Provides-Extra: docs
-Requires-Dist: Sphinx>=7.2.6; extra == "docs"
-Requires-Dist: furo>=2023.9.10; extra == "docs"
-Provides-Extra: all
-Requires-Dist: hydrobot[dev,docs,test]; extra == "all"
-
-======================
-Hydrobot
-======================
-
-
-.. image:: https://img.shields.io/pypi/v/hydrobot.svg
-        :target: https://pypi.python.org/pypi/hydrobot
-
-.. image:: https://readthedocs.org/projects/hydrobot/badge/?version=latest
-        :target: https://hydrobot.readthedocs.io/en/latest/?version=latest
-        :alt: Documentation Status
-
-Python Package providing a suite of processing tools and utilities for Hilltop hydrological data.
-
-
-* Free software: GNU General Public License v3
-* Documentation: https://hydrobot.readthedocs.io.
-
-
-Features
---------
-
-* Processes data downloaded from Hilltop Server
-* Uses annalist to record all changes to data
-* Capable of various automated processing techniques, including:
-
-  * Clipping data
-  * Removing spikes based on FBEWMA smoothing
-  * Identifying and removing 'flatlining' data, where an instrument repeats it's last collected data point (NOTE: It's unclear if this actually happening.)
-  * Identifying gaps and gap lengths and closing small gaps
-  * Aggregating check data from various sources.
-  * Quality coding data based on NEMS standards
-
-* Plotting data, including:
-
-  * Processed data with quality codes
-  * Comparing raw data to processed data
-  * Showing all changes to the data
-  * Visualizing check points from various sources.
-
-Usage (Alpha)
--------------
-
-The Alpha release of Hydrobot supports a "hybrid" workflow. This means that some external tools are still required to do a full processing. Importantly, the hybrid workflow relies on some R scripts to obtain check data from sources other than Hilltop. Further processing using Hilltop manager is also supported.
-
-NOTE: Hydrobot 0.5.0 supports only Water Temperature processing at the moment, but more measurements will be supported in patches as the processing progresses.
-
-Initial Setup (Repeat for each release)
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-#. Install a Python 3.11 interpreter. Note that 3.12 is not supported just yet.
-#. In your favourite shell, create a new virtual environment using this python interpreter and name it "hydrobot0.5.0". It's important that this is stored somewhere locally. I suggest creating a folder for virtual environments in your home folder::
-
-    python -m venv path/to/venv/hydrobot0.5.0/
-
-#. Activate this virtual environment. In powershell this should be something like::
-
-    ./path/to/venv/hydrobot0.5.0/Scripts/Activate.ps1
-
-#. If you're sure your venv is active (ensure with `which python` and confirm that you're using the interpreter in your venv folder), install the latest version of Hydrobot using pip::
-
-    pip install hydrobot
-
-#. Navigate to the processing folder that you create as part of the Processing Steps below::
-
-    cd //ares/hydro/processing/whatever/watertemp/site/30X/
-
-
-Processing Steps
-^^^^^^^^^^^^^^^^
-
-#. Open Logsheet Loader. Fill it as normal, and note the start date of your processing period (i.e. end date of the previous period).
-#. Navigate to the data source and site folder, and create your processing folder.
-#. Copy all the processing files in this folder into your processing folder::
-
-    \\ares\Environmental Data Validation\Water Temperature\Documents\Hydrobot_0.5.0_Files\
-
-    //ares/Environmental\ Data\ Validation/Water\ Temperature/Documents/Hydrobot_0.5.0_Files/
-
-#. In your processing folder, open the `config.yaml` file and change the fields `site`, `from_date`, `to_date`, `analyst_name`. Feel free to mess with the other values once you get the hang of it. No one will die.
-
-#. Run the R script. I'm not an R guy so I'm not sure how to do this other than to open it in R studio, highlighting all the code, and hitting `Ctrl+Enter`. This should create a bunch of `.csv` files containing the check data from various sources. This is a good reasource for perusal during processing, but will be imbibed by hydrobot to for QC encoding.
-
-#. Make sure your virtual environment is set up and active. Ensure with `which python` and confirm that your python interpreter is running from your venv folder.
-
-#. Run the hydrobot processing script::
-
-    python processing_script.py
-
-#. If all goes well, the processing script will open a browser tab showing a diagnostic dash for your site. Use this to identify issues in the site.
-
-#. Use your python skills to solve some issues, like removing erroneous check data points or deleting chunks of data. More extensive documentation on actually using hydrobot will follow in future releases.
-
-#. Happy processing!
-
-Credits
--------
-
-This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template. Furthermore, Sam is a real champ with the coding and whatnot. Thanks Sam.
-
-.. _Cookiecutter: https://github.com/audreyr/cookiecutter
-.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
+Metadata-Version: 2.1
+Name: hydrobot
+Version: 0.5.1
+Summary: A suite of processing tools for Hilltop hydrological data.
+Author-email: Nic Mostert <nicolas.mostert@horizons.govt.nz>, Sam Irvine <sam.irvine@horizons.govt.nz>
+License: GNU General Public License v3
+Project-URL: Homepage, https://github.com/HorizonsRC/hydrobot
+Project-URL: Issues, https://github.com/HorizonsRC/hydrobot/issues
+Project-URL: Documentation, https://hydrobot.readthedocs.io
+Project-URL: Package, https://pypi.org/project/hydrobot
+Keywords: hydrology, automation, pandas, hilltop, hilltop-py, HorizonsRC
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: ==3.11.*
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+License-File: AUTHORS.rst
+Requires-Dist: hilltop-py>=2.3.1
+Requires-Dist: data-annalist>=0.4.1
+Requires-Dist: matplotlib>=3.8.0
+Requires-Dist: defusedxml>=0.7.1
+Requires-Dist: plotly>=5.20.0
+Provides-Extra: test
+Requires-Dist: pytest>=7.4.2; extra == "test"
+Requires-Dist: pytest-cov>=4.1.0; extra == "test"
+Requires-Dist: pytest-dependency>=0.5.1; extra == "test"
+Requires-Dist: pytest-mock>=3.12.0; extra == "test"
+Provides-Extra: dev
+Requires-Dist: ruff>=0.1.6; extra == "dev"
+Requires-Dist: ruff-lsp>=0.0.45; extra == "dev"
+Requires-Dist: pre-commit>=3.5.0; extra == "dev"
+Requires-Dist: build>=1.0.0; extra == "dev"
+Provides-Extra: docs
+Requires-Dist: Sphinx>=7.2.6; extra == "docs"
+Requires-Dist: furo>=2023.9.10; extra == "docs"
+Provides-Extra: all
+Requires-Dist: hydrobot[dev,docs,test]; extra == "all"
+
+======================
+Hydrobot
+======================
+
+
+.. image:: https://img.shields.io/pypi/v/hydrobot.svg
+        :target: https://pypi.python.org/pypi/hydrobot
+
+.. image:: https://readthedocs.org/projects/hydrobot/badge/?version=latest
+        :target: https://hydrobot.readthedocs.io/en/latest/?version=latest
+        :alt: Documentation Status
+
+Python Package providing a suite of processing tools and utilities for Hilltop hydrological data.
+
+
+* Free software: GNU General Public License v3
+* Documentation: https://hydrobot.readthedocs.io.
+
+
+Features
+--------
+
+* Processes data downloaded from Hilltop Server
+* Uses annalist to record all changes to data
+* Capable of various automated processing techniques, including:
+
+  * Clipping data
+  * Removing spikes based on FBEWMA smoothing
+  * Identifying and removing 'flatlining' data, where an instrument repeats it's last collected data point (NOTE: It's unclear if this actually happening.)
+  * Identifying gaps and gap lengths and closing small gaps
+  * Aggregating check data from various sources.
+  * Quality coding data based on NEMS standards
+
+* Plotting data, including:
+
+  * Processed data with quality codes
+  * Comparing raw data to processed data
+  * Showing all changes to the data
+  * Visualizing check points from various sources.
+
+Usage (Alpha)
+-------------
+
+The Alpha release of Hydrobot supports a "hybrid" workflow. This means that some external tools are still required to do a full processing. Importantly, the hybrid workflow relies on some R scripts to obtain check data from sources other than Hilltop. Further processing using Hilltop manager is also supported.
+
+NOTE: Hydrobot 0.5.0 supports only Water Temperature processing at the moment, but more measurements will be supported in patches as the processing progresses.
+
+Initial Setup (Repeat for each release)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+#. Install a Python 3.11 interpreter. Note that 3.12 is not supported just yet.
+#. In your favourite shell, create a new virtual environment using this python interpreter and name it "hydrobot0.5.0". It's important that this is stored somewhere locally. I suggest creating a folder for virtual environments in your home folder::
+
+    python -m venv path/to/venv/hydrobot0.5.0/
+
+#. Activate this virtual environment. In powershell this should be something like::
+
+    ./path/to/venv/hydrobot0.5.0/Scripts/Activate.ps1
+
+#. If you're sure your venv is active (ensure with `which python` and confirm that you're using the interpreter in your venv folder), install the latest version of Hydrobot using pip::
+
+    pip install hydrobot
+
+#. Record which version of dependencies you have installed. The following pip freeze records which dependencies are
+installed by the hydrobot install process for if auditing/reprocessing is required later::
+
+    pip freeze > dependencies.txt
+
+#. Navigate to the processing folder that you create as part of the Processing Steps below::
+
+    cd //ares/hydro/processing/whatever/watertemp/site/30X/
+
+
+Processing Steps
+^^^^^^^^^^^^^^^^
+
+#. Open Logsheet Loader. Fill it as normal, and note the start date of your processing period (i.e. end date of the previous period).
+#. Navigate to the data source and site folder, and create your processing folder.
+#. Copy all the processing files in this folder into your processing folder::
+
+    \\ares\Environmental Data Validation\Water Temperature\Documents\Hydrobot_0.5.0_Files\
+
+    //ares/Environmental\ Data\ Validation/Water\ Temperature/Documents/Hydrobot_0.5.0_Files/
+
+#. In your processing folder, open the `config.yaml` file and change the fields `site`, `from_date`, `to_date`, `analyst_name`. Feel free to mess with the other values once you get the hang of it. No one will die.
+
+#. Run the R script. I'm not an R guy so I'm not sure how to do this other than to open it in R studio, highlighting all the code, and hitting `Ctrl+Enter`. This should create a bunch of `.csv` files containing the check data from various sources. This is a good reasource for perusal during processing, but will be imbibed by hydrobot to for QC encoding.
+
+#. Make sure your virtual environment is set up and active. Ensure with `which python` and confirm that your python interpreter is running from your venv folder.
+
+#. Run the hydrobot processing script::
+
+    python processing_script.py
+
+#. If all goes well, the processing script will open a browser tab showing a diagnostic dash for your site. Use this to identify issues in the site.
+
+#. Use your python skills to solve some issues, like removing erroneous check data points or deleting chunks of data. More extensive documentation on actually using hydrobot will follow in future releases.
+
+#. Open the resulting processed.xml in manager, and copy it over to a hts file.
+
+#. Open the WaterTemp_check_data.csv outputed from the R file in a spreadsheet (sorry) and copy into hts file.
+
+#. Happy processing!
+
+Credits
+-------
+
+This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template. Furthermore,
+Sam is a real champ with the coding and whatnot. Thanks Sam.
+
+Aww thanks Nic. You also da man <3
+
+.. _Cookiecutter: https://github.com/audreyr/cookiecutter
+.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
```

### Comparing `hydrobot-0.5.0/hydrobot.egg-info/SOURCES.txt` & `hydrobot-0.5.1/hydrobot.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -23,17 +23,14 @@
 docs/hydrobot.rst
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/modules.rst
 docs/readme.rst
 docs/usage.rst
-docs/_build/html/_static/file.png
-docs/_build/html/_static/minus.png
-docs/_build/html/_static/plus.png
 hydrobot/__init__.py
 hydrobot/data_acquisition.py
 hydrobot/data_sources.py
 hydrobot/data_structure.py
 hydrobot/evaluator.py
 hydrobot/filters.py
 hydrobot/plotter.py
@@ -45,28 +42,30 @@
 hydrobot.egg-info/requires.txt
 hydrobot.egg-info/top_level.txt
 hydrobot/config/QualityCodeEvaluator_QC_config.csv
 hydrobot/config/TwoLevelQualityCodeEvaluator_QC_config.csv
 prototypes/Class_script.py
 prototypes/site_list_reader.py
 prototypes/site_parameters.json
+prototypes/example_script/WaterTemp_CheckData.R
+prototypes/example_script/config.yaml
+prototypes/example_script/script.py
 prototypes/output_dump/.gitignore
 prototypes/py_scripts/atmospheric_spike_removal.py
 prototypes/py_scripts/example_plot_script.py
 prototypes/py_scripts/gap_finder.py
 prototypes/py_scripts/new_ws_plot_with_check_data.py
 prototypes/py_scripts/plot_with_check_data.py
 prototypes/py_scripts/process_script.py
 prototypes/py_scripts/spike_removal_util.py
 prototypes/py_scripts/stage_full_process.py
 prototypes/py_scripts/water_temp_full_process.py
 prototypes/py_scripts/water_temp_spike_removal.py
 prototypes/py_scripts/output_dump/.gitignore
 prototypes/script_dump/.gitignore
-tests/.coverage
 tests/__init__.py
 tests/conftest.py
 tests/site_list_response.xml
 tests/test_data_sources.py
 tests/test_data_structure.py
 tests/test_evaluator.py
 tests/test_filters.py
```

### Comparing `hydrobot-0.5.0/prototypes/py_scripts/example_plot_script.py` & `hydrobot-0.5.1/prototypes/py_scripts/example_plot_script.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-"""Just a dummy script."""
-import numpy as np
-import pandas as pd
-from annalist.annalist import Annalist
-
-from hydrobot.plotter import check_plotter, gap_plotter
-
-ann = Annalist()
-ann.configure("Processing Water Temp Data.", "Hot Dameul, Sameul!")
-
-gap_data_dict = pd.Series(
-    {
-        pd.Timestamp("2021-01-01 00:00"): 1.0,
-        pd.Timestamp("2021-01-01 00:15"): 2.0,
-        pd.Timestamp("2021-01-01 00:30"): np.NaN,
-        pd.Timestamp("2021-01-01 00:45"): 1.0,
-        pd.Timestamp("2021-01-01 01:00"): 5.0,
-        pd.Timestamp("2021-01-01 01:15"): np.NaN,
-        pd.Timestamp("2021-01-01 01:30"): np.NaN,
-        pd.Timestamp("2021-01-01 01:45"): np.NaN,
-        pd.Timestamp("2021-01-01 02:00"): 0.0,
-        pd.Timestamp("2021-01-01 02:15"): 0.0,
-        pd.Timestamp("2021-01-01 02:30"): 1.0,
-        pd.Timestamp("2021-01-01 02:45"): 1.0,
-    }
-)
-
-raw_data_dict = {
-    pd.Timestamp("2021-01-01 00:00"): 1.0,
-    pd.Timestamp("2021-01-01 01:00"): 5.0,
-}
-
-gap_plotter(gap_data_dict, 3)
-check_plotter(gap_data_dict, raw_data_dict, 3)
+"""Just a dummy script."""
+import numpy as np
+import pandas as pd
+from annalist.annalist import Annalist
+
+from hydrobot.plotter import check_plotter, gap_plotter
+
+ann = Annalist()
+ann.configure("Processing Water Temp Data.", "Hot Dameul, Sameul!")
+
+gap_data_dict = pd.Series(
+    {
+        pd.Timestamp("2021-01-01 00:00"): 1.0,
+        pd.Timestamp("2021-01-01 00:15"): 2.0,
+        pd.Timestamp("2021-01-01 00:30"): np.NaN,
+        pd.Timestamp("2021-01-01 00:45"): 1.0,
+        pd.Timestamp("2021-01-01 01:00"): 5.0,
+        pd.Timestamp("2021-01-01 01:15"): np.NaN,
+        pd.Timestamp("2021-01-01 01:30"): np.NaN,
+        pd.Timestamp("2021-01-01 01:45"): np.NaN,
+        pd.Timestamp("2021-01-01 02:00"): 0.0,
+        pd.Timestamp("2021-01-01 02:15"): 0.0,
+        pd.Timestamp("2021-01-01 02:30"): 1.0,
+        pd.Timestamp("2021-01-01 02:45"): 1.0,
+    }
+)
+
+raw_data_dict = {
+    pd.Timestamp("2021-01-01 00:00"): 1.0,
+    pd.Timestamp("2021-01-01 01:00"): 5.0,
+}
+
+gap_plotter(gap_data_dict, 3)
+check_plotter(gap_data_dict, raw_data_dict, 3)
```

### Comparing `hydrobot-0.5.0/prototypes/py_scripts/gap_finder.py` & `hydrobot-0.5.1/prototypes/py_scripts/gap_finder.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-"""Gap Finder Script."""
-import matplotlib.pyplot as plt
-import numpy as np
-import pandas as pd
-
-from hydrobot.data_acquisition import get_data
-
-base_url = "http://hilltopdev.horizons.govt.nz/"
-standard_hts = "RawLogger.hts"
-site = "Manawatu at Foxton"
-measurement = "Atmospheric Pressure"
-from_date = "2021-01-01 00:00"
-to_date = "2023-10-12 8:30"
-
-base_data = get_data(
-    base_url,
-    standard_hts,
-    site,
-    measurement,
-    from_date,
-    to_date,
-)
-
-base_data = base_data.set_index("Time")
-base_data.index = pd.to_datetime(base_data.index)
-base_data = base_data.asfreq("15T")
-
-base_data.loc["2023-04-01 13:00:00"] = pd.NA
-print(f"Missing datastamps: {base_data['Value'].isna()}")
-print(base_data[(base_data.Value.isna()) & ~(base_data.Value.shift().isna())])
-gaps = len(base_data[(base_data.Value.isna()) & ~(base_data.Value.shift().isna())])
-print(f"Gaps: {gaps}")
-thresh = 3
-
-
-idx0 = np.flatnonzero(np.r_[True, np.diff(np.isnan(base_data["Value"])) != 0, True])
-count = np.diff(idx0)
-idx = idx0[:-1]
-valid_mask = np.isnan(base_data["Value"][idx])
-out_idx = idx[valid_mask]
-out_count = count[valid_mask]
-out = zip(base_data.index[out_idx], out_count, strict=True)
-print([o for o in out])
-
-
-nans = base_data[base_data["Value"].isna()]
-fake_nans = nans
-fake_nans["Value"] = 1000
-
-plt.figure(figsize=(10, 6))
-plt.plot(base_data["Value"], label="Data")
-plt.plot(
-    fake_nans["Value"],
-    color="red",
-    marker="|",
-    linestyle="None",
-    label="Gaps",
-    markersize=100,
-)
-plt.title(f"Gaps in da data = {base_data['Value'].isna().sum()}")
-plt.legend()
-plt.show()
+"""Gap Finder Script."""
+import matplotlib.pyplot as plt
+import numpy as np
+import pandas as pd
+
+from hydrobot.data_acquisition import get_data
+
+base_url = "http://hilltopdev.horizons.govt.nz/"
+standard_hts = "RawLogger.hts"
+site = "Manawatu at Foxton"
+measurement = "Atmospheric Pressure"
+from_date = "2021-01-01 00:00"
+to_date = "2023-10-12 8:30"
+
+base_data = get_data(
+    base_url,
+    standard_hts,
+    site,
+    measurement,
+    from_date,
+    to_date,
+)
+
+base_data = base_data.set_index("Time")
+base_data.index = pd.to_datetime(base_data.index)
+base_data = base_data.asfreq("15T")
+
+base_data.loc["2023-04-01 13:00:00"] = pd.NA
+print(f"Missing datastamps: {base_data['Value'].isna()}")
+print(base_data[(base_data.Value.isna()) & ~(base_data.Value.shift().isna())])
+gaps = len(base_data[(base_data.Value.isna()) & ~(base_data.Value.shift().isna())])
+print(f"Gaps: {gaps}")
+thresh = 3
+
+
+idx0 = np.flatnonzero(np.r_[True, np.diff(np.isnan(base_data["Value"])) != 0, True])
+count = np.diff(idx0)
+idx = idx0[:-1]
+valid_mask = np.isnan(base_data["Value"][idx])
+out_idx = idx[valid_mask]
+out_count = count[valid_mask]
+out = zip(base_data.index[out_idx], out_count, strict=True)
+print([o for o in out])
+
+
+nans = base_data[base_data["Value"].isna()]
+fake_nans = nans
+fake_nans["Value"] = 1000
+
+plt.figure(figsize=(10, 6))
+plt.plot(base_data["Value"], label="Data")
+plt.plot(
+    fake_nans["Value"],
+    color="red",
+    marker="|",
+    linestyle="None",
+    label="Gaps",
+    markersize=100,
+)
+plt.title(f"Gaps in da data = {base_data['Value'].isna().sum()}")
+plt.legend()
+plt.show()
```

### Comparing `hydrobot-0.5.0/prototypes/py_scripts/new_ws_plot_with_check_data.py` & `hydrobot-0.5.1/prototypes/py_scripts/new_ws_plot_with_check_data.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-"""Using the utilities functions for various data sets."""
-
-import matplotlib.pyplot as plt
-
-from hydrobot.data_acquisition import get_data
-
-# Location and attributes of data to be obtained
-base_url = "http://hilltopdev.horizons.govt.nz/"
-standard_hts = "RawLogger.hts"
-check_hts = "boo.hts"
-
-site = "Manawatu at Teachers College"
-from_date = "2021-01-01 00:00"
-to_date = "2023-10-12 8:30"
-
-
-# Measurements used
-measurement = "Water Temperature [Dissolved Oxygen sensor]"
-check_measurement = "Water Temperature Check [Water Temperature]"
-
-base_data = get_data(
-    base_url,
-    standard_hts,
-    site,
-    measurement,
-    from_date,
-    to_date,
-)
-base_data = base_data[base_data["Value"] != -1]
-
-check_data = get_data(
-    base_url,
-    check_hts,
-    site,
-    check_measurement,
-    from_date,
-    to_date,
-    tstype="Check",
-)
-# Filter
-check_data = check_data[check_data["Value"] != -1]
-
-base_data.to_csv("output_dump/base_" + site + "-" + measurement + ".csv")
-check_data.to_csv("output_dump/check_" + site + "-" + check_measurement + ".csv")
-
-plt.figure(figsize=(10, 6))
-plt.subplot(1, 1, 1)
-plt.plot(base_data["Time"], base_data["Value"], label="Original Data")
-plt.plot(
-    check_data["Time"],
-    check_data["Value"],
-    label="Check Data",
-    marker="o",
-    linestyle="None",
-)
-plt.legend()
-plt.show()
+"""Using the utilities functions for various data sets."""
+
+import matplotlib.pyplot as plt
+
+from hydrobot.data_acquisition import get_data
+
+# Location and attributes of data to be obtained
+base_url = "http://hilltopdev.horizons.govt.nz/"
+standard_hts = "RawLogger.hts"
+check_hts = "boo.hts"
+
+site = "Manawatu at Teachers College"
+from_date = "2021-01-01 00:00"
+to_date = "2023-10-12 8:30"
+
+
+# Measurements used
+measurement = "Water Temperature [Dissolved Oxygen sensor]"
+check_measurement = "Water Temperature Check [Water Temperature]"
+
+base_data = get_data(
+    base_url,
+    standard_hts,
+    site,
+    measurement,
+    from_date,
+    to_date,
+)
+base_data = base_data[base_data["Value"] != -1]
+
+check_data = get_data(
+    base_url,
+    check_hts,
+    site,
+    check_measurement,
+    from_date,
+    to_date,
+    tstype="Check",
+)
+# Filter
+check_data = check_data[check_data["Value"] != -1]
+
+base_data.to_csv("output_dump/base_" + site + "-" + measurement + ".csv")
+check_data.to_csv("output_dump/check_" + site + "-" + check_measurement + ".csv")
+
+plt.figure(figsize=(10, 6))
+plt.subplot(1, 1, 1)
+plt.plot(base_data["Time"], base_data["Value"], label="Original Data")
+plt.plot(
+    check_data["Time"],
+    check_data["Value"],
+    label="Check Data",
+    marker="o",
+    linestyle="None",
+)
+plt.legend()
+plt.show()
```

### Comparing `hydrobot-0.5.0/prototypes/py_scripts/process_script.py` & `hydrobot-0.5.1/prototypes/py_scripts/process_script.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,134 +1,134 @@
-"""Script to run through various processing tasks."""
-import matplotlib.pyplot as plt
-import pandas as pd
-
-# import pandas as pd
-from annalist.annalist import Annalist
-
-import hydrobot.plotter as plotter
-from hydrobot.data_acquisition import get_series
-from hydrobot.data_sources import get_qc_evaluator
-from hydrobot.evaluator import diagnose_data, quality_encoder, small_gap_closer
-from hydrobot.filters import clip, remove_spikes
-
-
-def process_data(processing_parameters):
-    """Script to run through all processing."""
-    # Location and attributes of data to be obtained
-
-    ann = Annalist()
-    ann.configure(
-        logfile="output_dump/Processing Water Temp Data.",
-        analyst_name="Hot Dameul, Sameul!",
-    )
-
-    base_series = get_series(
-        processing_parameters["base_url"],
-        processing_parameters["standard_hts_filename"],
-        processing_parameters["site"],
-        processing_parameters["standard_measurement_name"],
-        processing_parameters["from_date"],
-        processing_parameters["to_date"],
-    )
-    base_series = base_series.asfreq(processing_parameters["frequency"])
-    if not isinstance(base_series, pd.Series):
-        raise TypeError("This should be a pd.Series, but it's a pd.DataFrame")
-
-    check_data = get_series(
-        processing_parameters["base_url"],
-        processing_parameters["check_hts_filename"],
-        processing_parameters["site"],
-        processing_parameters["check_measurement_name"],
-        processing_parameters["from_date"],
-        processing_parameters["to_date"],
-        tstype="Check",
-    )
-    if not isinstance(base_series, pd.Series):
-        raise TypeError("This should be a pd.Series, but it's a pd.DataFrame")
-
-    # Clip check data
-    check_series = clip(
-        pd.Series(check_data["Check Guage Total"]),
-        processing_parameters["defaults"]["low_clip"],
-        processing_parameters["defaults"]["high_clip"],
-    )
-
-    # Removing spikes from base data
-    base_series = remove_spikes(
-        base_series,
-        processing_parameters["defaults"]["span"],
-        processing_parameters["defaults"]["low_clip"],
-        processing_parameters["defaults"]["high_clip"],
-        processing_parameters["defaults"]["delta"],
-    )
-
-    # Removing small np.NaN gaps
-    base_series = small_gap_closer(
-        base_series, gap_limit=parameters["defaults"]["gap_limit"]
-    )
-
-    # Find the QC values
-    qc_series = quality_encoder(
-        base_series,
-        check_series,
-        get_qc_evaluator(processing_parameters["standard_measurement_name"]),
-        gap_limit=parameters["defaults"]["gap_limit"],
-    )
-
-    # Export the data
-    base_series.to_csv(
-        "output_dump/base_"
-        + processing_parameters["site"]
-        + "-"
-        + processing_parameters["standard_measurement_name"]
-        + ".csv"
-    )
-    check_series.to_csv(
-        "output_dump/check_"
-        + processing_parameters["site"]
-        + "-"
-        + processing_parameters["check_measurement_name"]
-        + ".csv"
-    )
-    qc_series.to_csv(
-        "output_dump/QC_"
-        + processing_parameters["site"]
-        + "-"
-        + processing_parameters["standard_measurement_name"]
-        + ".csv"
-    )
-
-    diagnose_data(
-        base_series,
-        check_series,
-        qc_series,
-        parameters["frequency"],
-    )
-    with plt.rc_context(rc={"figure.max_open_warning": 0}):
-        plotter.qc_plotter(
-            base_series, check_series, qc_series, parameters["frequency"], show=False
-        )
-        plotter.check_plotter(base_series, check_series, show=False)
-        plotter.gap_plotter(base_series)
-
-
-parameters = {
-    "base_url": "http://hilltopdev.horizons.govt.nz/",
-    "standard_hts_filename": "RawLogger.hts",
-    "check_hts_filename": "boo.hts",
-    "site": "Whanganui at Te Rewa",
-    "from_date": "2021-06-01 00:00",
-    "to_date": "2023-08-12 8:30",
-    "frequency": "5T",
-    "standard_measurement_name": "Water level statistics: Point Sample",
-    "check_measurement_name": "External S.G. [Water Level NRT]",
-    "defaults": {
-        "high_clip": 20000,
-        "low_clip": 0,
-        "delta": 1000,
-        "span": 10,
-        "gap_limit": 12,
-    },
-}
-
-process_data(parameters)
+"""Script to run through various processing tasks."""
+import matplotlib.pyplot as plt
+import pandas as pd
+
+# import pandas as pd
+from annalist.annalist import Annalist
+
+import hydrobot.plotter as plotter
+from hydrobot.data_acquisition import get_series
+from hydrobot.data_sources import get_qc_evaluator
+from hydrobot.evaluator import diagnose_data, quality_encoder, small_gap_closer
+from hydrobot.filters import clip, remove_spikes
+
+
+def process_data(processing_parameters):
+    """Script to run through all processing."""
+    # Location and attributes of data to be obtained
+
+    ann = Annalist()
+    ann.configure(
+        logfile="output_dump/Processing Water Temp Data.",
+        analyst_name="Hot Dameul, Sameul!",
+    )
+
+    base_series = get_series(
+        processing_parameters["base_url"],
+        processing_parameters["standard_hts_filename"],
+        processing_parameters["site"],
+        processing_parameters["standard_measurement_name"],
+        processing_parameters["from_date"],
+        processing_parameters["to_date"],
+    )
+    base_series = base_series.asfreq(processing_parameters["frequency"])
+    if not isinstance(base_series, pd.Series):
+        raise TypeError("This should be a pd.Series, but it's a pd.DataFrame")
+
+    check_data = get_series(
+        processing_parameters["base_url"],
+        processing_parameters["check_hts_filename"],
+        processing_parameters["site"],
+        processing_parameters["check_measurement_name"],
+        processing_parameters["from_date"],
+        processing_parameters["to_date"],
+        tstype="Check",
+    )
+    if not isinstance(base_series, pd.Series):
+        raise TypeError("This should be a pd.Series, but it's a pd.DataFrame")
+
+    # Clip check data
+    check_series = clip(
+        pd.Series(check_data["Check Guage Total"]),
+        processing_parameters["defaults"]["low_clip"],
+        processing_parameters["defaults"]["high_clip"],
+    )
+
+    # Removing spikes from base data
+    base_series = remove_spikes(
+        base_series,
+        processing_parameters["defaults"]["span"],
+        processing_parameters["defaults"]["low_clip"],
+        processing_parameters["defaults"]["high_clip"],
+        processing_parameters["defaults"]["delta"],
+    )
+
+    # Removing small np.NaN gaps
+    base_series = small_gap_closer(
+        base_series, gap_limit=parameters["defaults"]["gap_limit"]
+    )
+
+    # Find the QC values
+    qc_series = quality_encoder(
+        base_series,
+        check_series,
+        get_qc_evaluator(processing_parameters["standard_measurement_name"]),
+        gap_limit=parameters["defaults"]["gap_limit"],
+    )
+
+    # Export the data
+    base_series.to_csv(
+        "output_dump/base_"
+        + processing_parameters["site"]
+        + "-"
+        + processing_parameters["standard_measurement_name"]
+        + ".csv"
+    )
+    check_series.to_csv(
+        "output_dump/check_"
+        + processing_parameters["site"]
+        + "-"
+        + processing_parameters["check_measurement_name"]
+        + ".csv"
+    )
+    qc_series.to_csv(
+        "output_dump/QC_"
+        + processing_parameters["site"]
+        + "-"
+        + processing_parameters["standard_measurement_name"]
+        + ".csv"
+    )
+
+    diagnose_data(
+        base_series,
+        check_series,
+        qc_series,
+        parameters["frequency"],
+    )
+    with plt.rc_context(rc={"figure.max_open_warning": 0}):
+        plotter.qc_plotter(
+            base_series, check_series, qc_series, parameters["frequency"], show=False
+        )
+        plotter.check_plotter(base_series, check_series, show=False)
+        plotter.gap_plotter(base_series)
+
+
+parameters = {
+    "base_url": "http://hilltopdev.horizons.govt.nz/",
+    "standard_hts_filename": "RawLogger.hts",
+    "check_hts_filename": "boo.hts",
+    "site": "Whanganui at Te Rewa",
+    "from_date": "2021-06-01 00:00",
+    "to_date": "2023-08-12 8:30",
+    "frequency": "5T",
+    "standard_measurement_name": "Water level statistics: Point Sample",
+    "check_measurement_name": "External S.G. [Water Level NRT]",
+    "defaults": {
+        "high_clip": 20000,
+        "low_clip": 0,
+        "delta": 1000,
+        "span": 10,
+        "gap_limit": 12,
+    },
+}
+
+process_data(parameters)
```

### Comparing `hydrobot-0.5.0/prototypes/py_scripts/spike_removal_util.py` & `hydrobot-0.5.1/prototypes/py_scripts/spike_removal_util.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-"""Using the filters functions for various data sets."""
-
-import matplotlib.pyplot as plt
-
-import hydrobot.data_acquisition as data_acquisition
-import hydrobot.filters as filters
-
-# Location and attributes of data to be obtained
-base_url = "http://hilltopdev.horizons.govt.nz/"
-hts = "RawLoggerNet.hts"
-site = "HDC Foxton Beach 1"
-measurement = "Water Temperature"
-from_date = "2021-01-01 00:00"
-to_date = "2023-10-12 8:30"
-
-# Spike removal parameters
-span = 10
-high_clip = 40
-low_clip = 0
-delta = 1
-
-# Obtain data
-data = data_acquisition.get_data(
-    base_url, hts, site, measurement, from_date, to_date, "standard"
-)
-
-
-# Remove high values and low values
-cleaned_data = filters.remove_spikes(data["Value"], span, high_clip, low_clip, delta)
-
-# Display cleaned data
-plt.figure(figsize=(10, 6))
-plt.subplot(1, 1, 1)
-plt.plot(data["Value"], label="Original Data")
-plt.plot(cleaned_data, label="Cleaned Data")
-plt.legend()
-plt.show()
+"""Using the filters functions for various data sets."""
+
+import matplotlib.pyplot as plt
+
+import hydrobot.data_acquisition as data_acquisition
+import hydrobot.filters as filters
+
+# Location and attributes of data to be obtained
+base_url = "http://hilltopdev.horizons.govt.nz/"
+hts = "RawLoggerNet.hts"
+site = "HDC Foxton Beach 1"
+measurement = "Water Temperature"
+from_date = "2021-01-01 00:00"
+to_date = "2023-10-12 8:30"
+
+# Spike removal parameters
+span = 10
+high_clip = 40
+low_clip = 0
+delta = 1
+
+# Obtain data
+data = data_acquisition.get_data(
+    base_url, hts, site, measurement, from_date, to_date, "standard"
+)
+
+
+# Remove high values and low values
+cleaned_data = filters.remove_spikes(data["Value"], span, high_clip, low_clip, delta)
+
+# Display cleaned data
+plt.figure(figsize=(10, 6))
+plt.subplot(1, 1, 1)
+plt.plot(data["Value"], label="Original Data")
+plt.plot(cleaned_data, label="Cleaned Data")
+plt.legend()
+plt.show()
```

### Comparing `hydrobot-0.5.0/prototypes/py_scripts/stage_full_process.py` & `hydrobot-0.5.1/prototypes/py_scripts/stage_full_process.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,125 +1,125 @@
-"""Script to run through various processing tasks."""
-# import time
-import matplotlib.pyplot as plt
-import pandas as pd
-from annalist.annalist import Annalist
-
-from hydrobot.data_acquisition import get_data
-from hydrobot.data_sources import get_qc_evaluator
-from hydrobot.evaluator import (
-    base_data_meets_qc,
-    check_data_quality_code,
-    diagnose_data,
-    small_gap_closer,
-)
-from hydrobot.filters import clip, remove_spikes
-
-# Location and attributes of data to be obtained
-base_url = "http://hilltopdev.horizons.govt.nz/"
-standard_hts = "RawLogger.hts"
-check_hts = "boo.hts"
-
-site = "Whanganui at Te Rewa"
-from_date = "2021-01-01 00:00"
-to_date = "2023-10-12 8:30"
-frequency = "5T"
-
-high_clip = 20000
-low_clip = 0
-delta = 1000
-span = 10
-
-# Measurements used
-measurement = "Water level statistics: Point Sample"
-check_measurement = "External S.G. [Water Level NRT]"
-
-ann = Annalist()
-ann.configure("output_dump/Processing Water Temp Data.", "Hot Dameul, Sameul!")
-
-base_data = get_data(
-    base_url,
-    standard_hts,
-    site,
-    measurement,
-    from_date,
-    to_date,
-)
-base_series = pd.Series(base_data["Value"].values, base_data["Time"])
-base_series = base_series.asfreq(frequency)
-raw_data = base_series
-
-base_series.index.name = "Time"
-base_series.name = "Value"
-
-check_data = get_data(
-    base_url,
-    check_hts,
-    site,
-    check_measurement,
-    from_date,
-    to_date,
-    tstype="Check",
-)
-check_series = pd.Series(check_data["Value"].values, check_data["Time"])
-check_series.index.name = "Time"
-check_series.name = "Value"
-# Clip check data
-check_series = clip(check_series, low_clip, high_clip)
-
-# Removing spikes from base data
-base_series = remove_spikes(base_series, span, low_clip, high_clip, delta)
-
-# Removing small np.NaN gaps
-base_series = small_gap_closer(base_series, 12)
-
-
-# Find the QC values
-qc_series = check_data_quality_code(
-    base_series, check_series, get_qc_evaluator(measurement)
-)
-qc_series.index.name = "Time"
-qc_series.name = "Value"
-
-# Export the data
-base_series.to_csv("output_dump/base_" + site + "-" + measurement + ".csv")
-check_series.to_csv("output_dump/check_" + site + "-" + check_measurement + ".csv")
-qc_series.to_csv("output_dump/QC_" + site + "-" + check_measurement + ".csv")
-
-# filters for each QC
-check_400 = check_series[qc_series == 400]
-check_500 = check_series[qc_series == 500]
-check_600 = check_series[qc_series == 600]
-check_other = check_series[(qc_series != 400) & (qc_series != 500) & (qc_series != 600)]
-base_200 = base_data_meets_qc(base_series, qc_series, 200).asfreq(frequency)
-base_400 = base_data_meets_qc(base_series, qc_series, 400).asfreq(frequency)
-base_500 = base_data_meets_qc(base_series, qc_series, 500).asfreq(frequency)
-base_600 = base_data_meets_qc(base_series, qc_series, 600).asfreq(frequency)
-
-
-print(
-    diagnose_data(
-        raw_data,
-        base_series,
-        [base_600, base_500, base_400, base_200],
-        [600, 500, 400, 200],
-        check_series,
-    )
-)
-
-plt.figure(figsize=(10, 6))
-# plt.plot(base_series.index, base_series, label="All data") # for all data
-plt.plot(base_600.index, base_600, label="QC600", color="#006400")
-plt.plot(base_500.index, base_500, label="QC500", color="#00bfff")
-plt.plot(base_400.index, base_400, label="QC400", color="#ffa500")
-plt.plot(base_200.index, base_200, label="QC200", color="#8b5902")
-plt.plot(
-    check_series.index,
-    check_series,
-    label="Check data",
-    marker="o",
-    color="black",
-    linestyle="None",
-)
-
-plt.legend()
-plt.show()
+"""Script to run through various processing tasks."""
+# import time
+import matplotlib.pyplot as plt
+import pandas as pd
+from annalist.annalist import Annalist
+
+from hydrobot.data_acquisition import get_data
+from hydrobot.data_sources import get_qc_evaluator
+from hydrobot.evaluator import (
+    base_data_meets_qc,
+    check_data_quality_code,
+    diagnose_data,
+    small_gap_closer,
+)
+from hydrobot.filters import clip, remove_spikes
+
+# Location and attributes of data to be obtained
+base_url = "http://hilltopdev.horizons.govt.nz/"
+standard_hts = "RawLogger.hts"
+check_hts = "boo.hts"
+
+site = "Whanganui at Te Rewa"
+from_date = "2021-01-01 00:00"
+to_date = "2023-10-12 8:30"
+frequency = "5T"
+
+high_clip = 20000
+low_clip = 0
+delta = 1000
+span = 10
+
+# Measurements used
+measurement = "Water level statistics: Point Sample"
+check_measurement = "External S.G. [Water Level NRT]"
+
+ann = Annalist()
+ann.configure("output_dump/Processing Water Temp Data.", "Hot Dameul, Sameul!")
+
+base_data = get_data(
+    base_url,
+    standard_hts,
+    site,
+    measurement,
+    from_date,
+    to_date,
+)
+base_series = pd.Series(base_data["Value"].values, base_data["Time"])
+base_series = base_series.asfreq(frequency)
+raw_data = base_series
+
+base_series.index.name = "Time"
+base_series.name = "Value"
+
+check_data = get_data(
+    base_url,
+    check_hts,
+    site,
+    check_measurement,
+    from_date,
+    to_date,
+    tstype="Check",
+)
+check_series = pd.Series(check_data["Value"].values, check_data["Time"])
+check_series.index.name = "Time"
+check_series.name = "Value"
+# Clip check data
+check_series = clip(check_series, low_clip, high_clip)
+
+# Removing spikes from base data
+base_series = remove_spikes(base_series, span, low_clip, high_clip, delta)
+
+# Removing small np.NaN gaps
+base_series = small_gap_closer(base_series, 12)
+
+
+# Find the QC values
+qc_series = check_data_quality_code(
+    base_series, check_series, get_qc_evaluator(measurement)
+)
+qc_series.index.name = "Time"
+qc_series.name = "Value"
+
+# Export the data
+base_series.to_csv("output_dump/base_" + site + "-" + measurement + ".csv")
+check_series.to_csv("output_dump/check_" + site + "-" + check_measurement + ".csv")
+qc_series.to_csv("output_dump/QC_" + site + "-" + check_measurement + ".csv")
+
+# filters for each QC
+check_400 = check_series[qc_series == 400]
+check_500 = check_series[qc_series == 500]
+check_600 = check_series[qc_series == 600]
+check_other = check_series[(qc_series != 400) & (qc_series != 500) & (qc_series != 600)]
+base_200 = base_data_meets_qc(base_series, qc_series, 200).asfreq(frequency)
+base_400 = base_data_meets_qc(base_series, qc_series, 400).asfreq(frequency)
+base_500 = base_data_meets_qc(base_series, qc_series, 500).asfreq(frequency)
+base_600 = base_data_meets_qc(base_series, qc_series, 600).asfreq(frequency)
+
+
+print(
+    diagnose_data(
+        raw_data,
+        base_series,
+        [base_600, base_500, base_400, base_200],
+        [600, 500, 400, 200],
+        check_series,
+    )
+)
+
+plt.figure(figsize=(10, 6))
+# plt.plot(base_series.index, base_series, label="All data") # for all data
+plt.plot(base_600.index, base_600, label="QC600", color="#006400")
+plt.plot(base_500.index, base_500, label="QC500", color="#00bfff")
+plt.plot(base_400.index, base_400, label="QC400", color="#ffa500")
+plt.plot(base_200.index, base_200, label="QC200", color="#8b5902")
+plt.plot(
+    check_series.index,
+    check_series,
+    label="Check data",
+    marker="o",
+    color="black",
+    linestyle="None",
+)
+
+plt.legend()
+plt.show()
```

### Comparing `hydrobot-0.5.0/prototypes/py_scripts/water_temp_full_process.py` & `hydrobot-0.5.1/prototypes/py_scripts/water_temp_full_process.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,136 +1,136 @@
-"""Script to run through various processing tasks."""
-
-import matplotlib.pyplot as plt
-import pandas as pd
-from annalist.annalist import Annalist
-
-from hydrobot.data_acquisition import get_data
-from hydrobot.data_sources import get_qc_evaluator
-from hydrobot.evaluator import (
-    base_data_meets_qc,
-    check_data_quality_code,
-    diagnose_data,
-    missing_data_quality_code,
-    small_gap_closer,
-)
-from hydrobot.filters import clip, remove_spikes
-
-# Location and attributes of data to be obtained
-base_url = "http://hilltopdev.horizons.govt.nz/"
-standard_hts = "RawLogger.hts"
-check_hts = "boo.hts"
-
-site = "Rangitikei at Mangaweka"
-from_date = "2021-01-01 00:00"
-to_date = "2023-10-12 8:30"
-
-high_clip = 40
-low_clip = 0
-delta = 1
-span = 10
-
-# Measurements used
-measurement = "Water Temperature [Dissolved Oxygen sensor]"
-check_measurement = "Water Temperature Check [Water Temperature]"
-
-ann = Annalist()
-ann.configure(
-    logfile="output_dump/Processing Water Temp Data.",
-    analyst_name="Hot Dameul, Sameul!",
-)
-
-base_data = get_data(
-    base_url,
-    standard_hts,
-    site,
-    measurement,
-    from_date,
-    to_date,
-)
-base_series = pd.Series(base_data["Value"].values, base_data["Time"])
-base_series = base_series.asfreq("15T")
-raw_data = base_series
-
-base_series.index.name = "Time"
-base_series.name = "Value"
-
-check_data = get_data(
-    base_url,
-    check_hts,
-    site,
-    check_measurement,
-    from_date,
-    to_date,
-    tstype="Check",
-)
-check_series = pd.Series(check_data["Value"].values, check_data["Time"])
-check_series.index.name = "Time"
-check_series.name = "Value"
-# Clip check data
-check_series = clip(check_series, low_clip, high_clip)
-
-# Removing spikes from base data
-base_series = remove_spikes(base_series, span, low_clip, high_clip, delta)
-
-# Removing small np.NaN gaps
-base_series = small_gap_closer(base_series, 12)
-
-# Find the QC values
-qc_series = check_data_quality_code(
-    base_series, check_series, get_qc_evaluator(measurement)
-)
-qc_series = missing_data_quality_code(base_series, qc_series, 12)
-# qc_series[from_date] = np.NaN
-# qc_series.sort_index(inplace=True)
-# qc_series = qc_series.shift(-1, fill_value=0)
-qc_series.index.name = "Time"
-qc_series.name = "Value"
-
-# Export the data
-base_series.to_csv("output_dump/base_" + site + "-" + measurement + ".csv")
-check_series.to_csv("output_dump/check_" + site + "-" + check_measurement + ".csv")
-qc_series.to_csv("output_dump/QC_" + site + "-" + check_measurement + ".csv")
-
-# filters for each QC
-base_100 = (
-    base_data_meets_qc(base_series, qc_series, 100)
-    .fillna(base_series.median())
-    .asfreq("15T")
-)
-base_200 = base_data_meets_qc(base_series, qc_series, 200).asfreq("15T")
-base_400 = base_data_meets_qc(base_series, qc_series, 400).asfreq("15T")
-base_500 = base_data_meets_qc(base_series, qc_series, 500).asfreq("15T")
-base_600 = base_data_meets_qc(base_series, qc_series, 600).asfreq("15T")
-
-
-diagnose_data(
-    base_series,
-    check_series,
-    qc_series,
-    "15T",
-)
-
-plt.figure(figsize=(10, 6))
-# plt.plot(base_series.index, base_series, label="All data") # for all data
-plt.plot(base_600.index, base_600, label="QC600", color="#006400")
-plt.plot(base_500.index, base_500, label="QC500", color="#00bfff")
-plt.plot(base_400.index, base_400, label="QC400", color="#ffa500")
-plt.plot(base_200.index, base_200, label="QC200", color="#8b5902")
-plt.plot(
-    base_100.index,
-    base_100,
-    marker="x",
-    label="QC100",
-    color="#ff0000",
-)
-plt.plot(
-    check_series.index,
-    check_series,
-    label="Check data",
-    marker="o",
-    color="black",
-    linestyle="None",
-)
-
-plt.legend()
-plt.show()
+"""Script to run through various processing tasks."""
+
+import matplotlib.pyplot as plt
+import pandas as pd
+from annalist.annalist import Annalist
+
+from hydrobot.data_acquisition import get_data
+from hydrobot.data_sources import get_qc_evaluator
+from hydrobot.evaluator import (
+    base_data_meets_qc,
+    check_data_quality_code,
+    diagnose_data,
+    missing_data_quality_code,
+    small_gap_closer,
+)
+from hydrobot.filters import clip, remove_spikes
+
+# Location and attributes of data to be obtained
+base_url = "http://hilltopdev.horizons.govt.nz/"
+standard_hts = "RawLogger.hts"
+check_hts = "boo.hts"
+
+site = "Rangitikei at Mangaweka"
+from_date = "2021-01-01 00:00"
+to_date = "2023-10-12 8:30"
+
+high_clip = 40
+low_clip = 0
+delta = 1
+span = 10
+
+# Measurements used
+measurement = "Water Temperature [Dissolved Oxygen sensor]"
+check_measurement = "Water Temperature Check [Water Temperature]"
+
+ann = Annalist()
+ann.configure(
+    logfile="output_dump/Processing Water Temp Data.",
+    analyst_name="Hot Dameul, Sameul!",
+)
+
+base_data = get_data(
+    base_url,
+    standard_hts,
+    site,
+    measurement,
+    from_date,
+    to_date,
+)
+base_series = pd.Series(base_data["Value"].values, base_data["Time"])
+base_series = base_series.asfreq("15T")
+raw_data = base_series
+
+base_series.index.name = "Time"
+base_series.name = "Value"
+
+check_data = get_data(
+    base_url,
+    check_hts,
+    site,
+    check_measurement,
+    from_date,
+    to_date,
+    tstype="Check",
+)
+check_series = pd.Series(check_data["Value"].values, check_data["Time"])
+check_series.index.name = "Time"
+check_series.name = "Value"
+# Clip check data
+check_series = clip(check_series, low_clip, high_clip)
+
+# Removing spikes from base data
+base_series = remove_spikes(base_series, span, low_clip, high_clip, delta)
+
+# Removing small np.NaN gaps
+base_series = small_gap_closer(base_series, 12)
+
+# Find the QC values
+qc_series = check_data_quality_code(
+    base_series, check_series, get_qc_evaluator(measurement)
+)
+qc_series = missing_data_quality_code(base_series, qc_series, 12)
+# qc_series[from_date] = np.NaN
+# qc_series.sort_index(inplace=True)
+# qc_series = qc_series.shift(-1, fill_value=0)
+qc_series.index.name = "Time"
+qc_series.name = "Value"
+
+# Export the data
+base_series.to_csv("output_dump/base_" + site + "-" + measurement + ".csv")
+check_series.to_csv("output_dump/check_" + site + "-" + check_measurement + ".csv")
+qc_series.to_csv("output_dump/QC_" + site + "-" + check_measurement + ".csv")
+
+# filters for each QC
+base_100 = (
+    base_data_meets_qc(base_series, qc_series, 100)
+    .fillna(base_series.median())
+    .asfreq("15T")
+)
+base_200 = base_data_meets_qc(base_series, qc_series, 200).asfreq("15T")
+base_400 = base_data_meets_qc(base_series, qc_series, 400).asfreq("15T")
+base_500 = base_data_meets_qc(base_series, qc_series, 500).asfreq("15T")
+base_600 = base_data_meets_qc(base_series, qc_series, 600).asfreq("15T")
+
+
+diagnose_data(
+    base_series,
+    check_series,
+    qc_series,
+    "15T",
+)
+
+plt.figure(figsize=(10, 6))
+# plt.plot(base_series.index, base_series, label="All data") # for all data
+plt.plot(base_600.index, base_600, label="QC600", color="#006400")
+plt.plot(base_500.index, base_500, label="QC500", color="#00bfff")
+plt.plot(base_400.index, base_400, label="QC400", color="#ffa500")
+plt.plot(base_200.index, base_200, label="QC200", color="#8b5902")
+plt.plot(
+    base_100.index,
+    base_100,
+    marker="x",
+    label="QC100",
+    color="#ff0000",
+)
+plt.plot(
+    check_series.index,
+    check_series,
+    label="Check data",
+    marker="o",
+    color="black",
+    linestyle="None",
+)
+
+plt.legend()
+plt.show()
```

### Comparing `hydrobot-0.5.0/prototypes/py_scripts/water_temp_spike_removal.py` & `hydrobot-0.5.1/prototypes/py_scripts/water_temp_spike_removal.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-"""Using the filters functions for various data sets."""
-
-import matplotlib.pyplot as plt
-
-import hydrobot.data_acquisition as data_acquisition
-import hydrobot.filters as filters
-
-# Location and attributes of data to be obtained
-base_url = "http://hilltopdev.horizons.govt.nz/"
-hts = "RawLoggerNet.hts"
-site = "HDC Foxton Beach 1"
-measurement = "Water Temperature"
-from_date = "2021-01-01 00:00"
-to_date = "2023-10-12 8:30"
-
-# Spike removal parameters
-span = 10
-high_clip = 40
-low_clip = 0
-delta = 1
-
-# Choose whether to display extra plots
-display_working_plots = False
-
-# Obtain data
-data = data_acquisition.get_data(
-    base_url, hts, site, measurement, from_date, to_date, "standard"
-)
-
-
-# Base data display
-if display_working_plots:
-    plt.figure(figsize=(10, 6))
-    plt.subplot(1, 1, 1)
-    plt.plot(data["Value"], label="Original Data")
-    plt.title("Data before spike removal")
-    plt.legend()
-
-
-# Remove high values and low values
-clip_data = filters.clip(data["Value"], high_clip, low_clip)
-
-# Base vs clipped data display
-if display_working_plots:
-    plt.figure(figsize=(10, 6))
-    plt.subplot(1, 1, 1)
-    plt.plot(data["Value"], label="Original Data")
-    plt.plot(clip_data, label="Clipped Data")
-    plt.legend()
-
-# Create smoothed data using forwards-backwards exponential weighted moving
-# average (FBEWMA)
-fbewma_data = filters.fbewma(clip_data, span)
-
-# Base vs smoothed data
-if display_working_plots:
-    plt.figure(figsize=(10, 6))
-    plt.subplot(1, 1, 1)
-    plt.plot(data["Value"], label="Original Data")
-    plt.plot(fbewma_data, label="FBEWMA Data")
-    plt.legend()
-
-
-# Compare base data to smoothed data, remove any large differences
-delta_clip_data = filters.remove_outliers(clip_data, span, delta)
-
-# Display cleaned data
-plt.figure(figsize=(10, 6))
-plt.subplot(1, 1, 1)
-plt.plot(data["Value"], label="Original Data")
-plt.plot(delta_clip_data, label="Cleaned Data")
-plt.legend()
-plt.show()
+"""Using the filters functions for various data sets."""
+
+import matplotlib.pyplot as plt
+
+import hydrobot.data_acquisition as data_acquisition
+import hydrobot.filters as filters
+
+# Location and attributes of data to be obtained
+base_url = "http://hilltopdev.horizons.govt.nz/"
+hts = "RawLoggerNet.hts"
+site = "HDC Foxton Beach 1"
+measurement = "Water Temperature"
+from_date = "2021-01-01 00:00"
+to_date = "2023-10-12 8:30"
+
+# Spike removal parameters
+span = 10
+high_clip = 40
+low_clip = 0
+delta = 1
+
+# Choose whether to display extra plots
+display_working_plots = False
+
+# Obtain data
+data = data_acquisition.get_data(
+    base_url, hts, site, measurement, from_date, to_date, "standard"
+)
+
+
+# Base data display
+if display_working_plots:
+    plt.figure(figsize=(10, 6))
+    plt.subplot(1, 1, 1)
+    plt.plot(data["Value"], label="Original Data")
+    plt.title("Data before spike removal")
+    plt.legend()
+
+
+# Remove high values and low values
+clip_data = filters.clip(data["Value"], high_clip, low_clip)
+
+# Base vs clipped data display
+if display_working_plots:
+    plt.figure(figsize=(10, 6))
+    plt.subplot(1, 1, 1)
+    plt.plot(data["Value"], label="Original Data")
+    plt.plot(clip_data, label="Clipped Data")
+    plt.legend()
+
+# Create smoothed data using forwards-backwards exponential weighted moving
+# average (FBEWMA)
+fbewma_data = filters.fbewma(clip_data, span)
+
+# Base vs smoothed data
+if display_working_plots:
+    plt.figure(figsize=(10, 6))
+    plt.subplot(1, 1, 1)
+    plt.plot(data["Value"], label="Original Data")
+    plt.plot(fbewma_data, label="FBEWMA Data")
+    plt.legend()
+
+
+# Compare base data to smoothed data, remove any large differences
+delta_clip_data = filters.remove_outliers(clip_data, span, delta)
+
+# Display cleaned data
+plt.figure(figsize=(10, 6))
+plt.subplot(1, 1, 1)
+plt.plot(data["Value"], label="Original Data")
+plt.plot(delta_clip_data, label="Cleaned Data")
+plt.legend()
+plt.show()
```

### Comparing `hydrobot-0.5.0/pyproject.toml` & `hydrobot-0.5.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,116 +1,116 @@
-[build-system]
-requires = ["setuptools", "setuptools-scm"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "hydrobot"
-description = "A suite of processing tools for Hilltop hydrological data."
-version = "0.5.0"
-authors = [
-    { name = "Nic Mostert", email = "nicolas.mostert@horizons.govt.nz" },
-    { name = "Sam Irvine", email = "sam.irvine@horizons.govt.nz" }
-]
-requires-python = "==3.11.*"
-dependencies = [
-    "hilltop-py>=2.3.1",
-    "data-annalist>=0.4.1",
-    "matplotlib>=3.8.0",
-    "defusedxml>=0.7.1",
-    "plotly>=5.20.0"
-]
-classifiers=[
-    "Development Status :: 3 - Alpha",
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-    "Natural Language :: English",
-    "Programming Language :: Python :: 3.11",
-]
-license = {text = "GNU General Public License v3"}
-readme = "README.rst"
-keywords = ["hydrology, automation, pandas, hilltop, hilltop-py, HorizonsRC"]
-
-[project.urls]
-Homepage = "https://github.com/HorizonsRC/hydrobot"
-Issues = "https://github.com/HorizonsRC/hydrobot/issues"
-Documentation = "https://hydrobot.readthedocs.io"
-Package = "https://pypi.org/project/hydrobot"
-
-
-[project.optional-dependencies]
-test = [
-    "pytest>=7.4.2",
-    "pytest-cov>=4.1.0",
-    "pytest-dependency>=0.5.1",
-    "pytest-mock>=3.12.0",
-]
-dev = [
-    "ruff>=0.1.6",
-    "ruff-lsp>=0.0.45",
-    "pre-commit>=3.5.0",
-    "build>=1.0.0"
-]
-docs = [
-    "Sphinx>=7.2.6",
-    "furo>=2023.9.10",
-]
-all = [
-    "hydrobot[test, dev, docs]"
-]
-
-[tool.setuptools]
-packages = ["hydrobot"]
-
-[tool.setuptools.package-data]
-hydrobot = ["hydrobot/config/*"]
-
-[tool.pytest.ini_options]
-addopts = "--cov --cov-fail-under 100 --strict-markers"
-markers = [
-    "slow: marks tests as slow (deselect with '-m \"not slow\"')",
-    "remote: depends on remote server calls (deselect with '-m \"not remote\"')"
-]
-
-[tool.coverage.run]
-source = ["hydrobot"]
-
-
-[tool.ruff]
-extend-exclude = ["docs/*"]
-extend-select = [
-    "W505", # Line too long as a warning, not an error. Default set to 88.
-    "UP", # pyupgrade: Checks for out-dated syntax use.
-	"B", # Flake8 Bugbears:
-	"PD", # Pandas pro-gamer tips and conventions
-	"S", # Flake8 Bandit: Common security flaws.
-	"SLF", # Checks that private members are not accessed outside of classes.
-    "SIM", # Flake8 simplify: Mostly checks for code duplication and such.
-	"I", # Isort. Import order sorting? Why not.
-    "N", # pep8-naming: naming conventions
-	"D", # pydocstyle.
-	"PT", # flake8-pytest-style checking for pytests
-]
-extend-ignore = ["D401", "D203", "D212"]
-
-[tool.ruff.lint.pydocstyle]
-convention = "numpy"
-
-[tool.ruff.per-file-ignores]
-"tests/*" = ["S311", "S101", "F841"]
-"docs/*" = ["I001"]
-"prototypes" = ["D"]
-
-[tool.bumpversion]
-current_version = "0.5.0"
-commit = true
-tag = true
-tag_name = "{new_version}"
-
-[[tool.bumpversion.files]]
-filename = "pyproject.toml"
-search = "{current_version}"
-replace = "{new_version}"
-
-[[tool.bumpversion.files]]
-filename = "hydrobot/__init__.py"
-search = "__version__ = \"{current_version}\""
-replace = "__version__ = \"{new_version}\""
+[build-system]
+requires = ["setuptools", "setuptools-scm"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "hydrobot"
+description = "A suite of processing tools for Hilltop hydrological data."
+version = "0.5.1"
+authors = [
+    { name = "Nic Mostert", email = "nicolas.mostert@horizons.govt.nz" },
+    { name = "Sam Irvine", email = "sam.irvine@horizons.govt.nz" }
+]
+requires-python = "==3.11.*"
+dependencies = [
+    "hilltop-py>=2.3.1",
+    "data-annalist>=0.4.1",
+    "matplotlib>=3.8.0",
+    "defusedxml>=0.7.1",
+    "plotly>=5.20.0"
+]
+classifiers=[
+    "Development Status :: 3 - Alpha",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+    "Natural Language :: English",
+    "Programming Language :: Python :: 3.11",
+]
+license = {text = "GNU General Public License v3"}
+readme = "README.rst"
+keywords = ["hydrology, automation, pandas, hilltop, hilltop-py, HorizonsRC"]
+
+[project.urls]
+Homepage = "https://github.com/HorizonsRC/hydrobot"
+Issues = "https://github.com/HorizonsRC/hydrobot/issues"
+Documentation = "https://hydrobot.readthedocs.io"
+Package = "https://pypi.org/project/hydrobot"
+
+
+[project.optional-dependencies]
+test = [
+    "pytest>=7.4.2",
+    "pytest-cov>=4.1.0",
+    "pytest-dependency>=0.5.1",
+    "pytest-mock>=3.12.0",
+]
+dev = [
+    "ruff>=0.1.6",
+    "ruff-lsp>=0.0.45",
+    "pre-commit>=3.5.0",
+    "build>=1.0.0"
+]
+docs = [
+    "Sphinx>=7.2.6",
+    "furo>=2023.9.10",
+]
+all = [
+    "hydrobot[test, dev, docs]"
+]
+
+[tool.setuptools]
+packages = ["hydrobot"]
+
+[tool.setuptools.package-data]
+hydrobot = ["hydrobot/config/*"]
+
+[tool.pytest.ini_options]
+addopts = "--cov --cov-fail-under 100 --strict-markers"
+markers = [
+    "slow: marks tests as slow (deselect with '-m \"not slow\"')",
+    "remote: depends on remote server calls (deselect with '-m \"not remote\"')"
+]
+
+[tool.coverage.run]
+source = ["hydrobot"]
+
+
+[tool.ruff]
+extend-exclude = ["docs/*"]
+extend-select = [
+    "W505", # Line too long as a warning, not an error. Default set to 88.
+    "UP", # pyupgrade: Checks for out-dated syntax use.
+	"B", # Flake8 Bugbears:
+	"PD", # Pandas pro-gamer tips and conventions
+	"S", # Flake8 Bandit: Common security flaws.
+	"SLF", # Checks that private members are not accessed outside of classes.
+    "SIM", # Flake8 simplify: Mostly checks for code duplication and such.
+	"I", # Isort. Import order sorting? Why not.
+    "N", # pep8-naming: naming conventions
+	"D", # pydocstyle.
+	"PT", # flake8-pytest-style checking for pytests
+]
+extend-ignore = ["D401", "D203", "D212"]
+
+[tool.ruff.lint.pydocstyle]
+convention = "numpy"
+
+[tool.ruff.per-file-ignores]
+"tests/*" = ["S311", "S101", "F841"]
+"docs/*" = ["I001"]
+"prototypes" = ["D"]
+
+[tool.bumpversion]
+current_version = "0.5.1"
+commit = true
+tag = true
+tag_name = "{new_version}"
+
+[[tool.bumpversion.files]]
+filename = "pyproject.toml"
+search = "{current_version}"
+replace = "{new_version}"
+
+[[tool.bumpversion.files]]
+filename = "hydrobot/__init__.py"
+search = "__version__ = \"{current_version}\""
+replace = "__version__ = \"{new_version}\""
```

### Comparing `hydrobot-0.5.0/tests/conftest.py` & `hydrobot-0.5.1/tests/conftest.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-"""Fixtures to be shared across many pytests."""
-import pytest
-
-
-@pytest.fixture()
-def sample_data_source_xml_file():
-    """
-    PyTest fixture providing the path to a sample XML file for testing.
-
-    Returns
-    -------
-    str
-        The file path to the sample XML file.
-
-    Notes
-    -----
-    This fixture is intended to be used in tests that require a sample XML file.
-    The XML file contains output from Hilltop. The file contains Standard, Check and
-    Quality data for Rainfall and General Nastiness Mid Stream at Cowtoilet Farm.
-
-    Example Usage
-    -------------
-    def test_xml_parsing_function(sample_data_source_xml_file)
-        # Ensure the XML parsing function correctly handles the provided XML file.
-        with open(sample_data_source_xml_file) as f:
-            sample_data_source_xml = f.read()
-        result = example_xml_function(sample_data_source_xml)
-        assert result == expected_result
-    """
-    file_path = "tests/xml_test_data_file.xml"
-    return file_path
+"""Fixtures to be shared across many pytests."""
+import pytest
+
+
+@pytest.fixture()
+def sample_data_source_xml_file():
+    """
+    PyTest fixture providing the path to a sample XML file for testing.
+
+    Returns
+    -------
+    str
+        The file path to the sample XML file.
+
+    Notes
+    -----
+    This fixture is intended to be used in tests that require a sample XML file.
+    The XML file contains output from Hilltop. The file contains Standard, Check and
+    Quality data for Rainfall and General Nastiness Mid Stream at Cowtoilet Farm.
+
+    Example Usage
+    -------------
+    def test_xml_parsing_function(sample_data_source_xml_file)
+        # Ensure the XML parsing function correctly handles the provided XML file.
+        with open(sample_data_source_xml_file) as f:
+            sample_data_source_xml = f.read()
+        result = example_xml_function(sample_data_source_xml)
+        assert result == expected_result
+    """
+    file_path = "tests/xml_test_data_file.xml"
+    return file_path
```

### Comparing `hydrobot-0.5.0/tests/test_data_sources.py` & `hydrobot-0.5.1/tests/test_data_sources.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-"""Test the data_sources module."""
-import pytest
-from annalist.annalist import Annalist
-
-import hydrobot.data_sources as data_sources
-
-ann = Annalist()
-ann.configure()
-
-
-@pytest.mark.dependency(name="test_get_measurement_dict")
-def test_get_measurement_dict():
-    """Testing the measurement dictionary."""
-    m_dict = data_sources.get_qc_evaluator_dict()
-    assert isinstance(m_dict, dict), "not a dict somehow"
-    assert (
-        "Water Temperature [Dissolved Oxygen sensor]" in m_dict
-    ), "Missing data source water temp"
-    assert (
-        m_dict["Water Temperature [Dissolved Oxygen sensor]"].qc_500_limit > 0
-    ), "Water temp qc_500 limit not set up correctly"
-
-
-@pytest.mark.dependency(depends=["test_get_measurement_dict"])
-def test_get_measurement():
-    """Testing the get_measurement method."""
-    wt_meas = data_sources.get_qc_evaluator(
-        "Water Temperature [Dissolved Oxygen sensor]"
-    )
-    assert wt_meas.qc_500_limit > 0, "Water temp qc_500 limit not set up correctly"
-    assert wt_meas.find_qc(1.3, 0) == 400, "bad data not given bad qc"
-    assert wt_meas.find_qc(1, 0) == 500, "fair data not given fair qc"
-    assert wt_meas.find_qc(0.7, 0) == 600, "good data not given good qc"
-
-    stage_meas = data_sources.get_qc_evaluator("Water level statistics: Point Sample")
-    assert stage_meas.find_qc(1999, 1988) == 400, "bad data not given bad qc, static"
-    assert (
-        stage_meas.find_qc(1999, 1990) == 500
-    ), "fair data not given fair qc, static low"
-    assert (
-        stage_meas.find_qc(1999, 1995) == 500
-    ), "fair data not given fair qc, static high"
-    assert stage_meas.find_qc(1999, 1997) == 600, "good data not given good qc, perc"
-
-    assert stage_meas.find_qc(2001, 1990) == 400, "bad data not given bad qc, perc"
-    assert (
-        stage_meas.find_qc(2001, 1992) == 500
-    ), "fair data not given fair qc, perc low"
-    assert (
-        stage_meas.find_qc(2001, 1996) == 500
-    ), "fair data not given fair qc, perc high"
-    assert stage_meas.find_qc(2001, 1998) == 600, "good data not given good qc, perc"
-
-    assert (
-        stage_meas.find_qc(10000, 9949) == 400
-    ), "bad data not given bad qc, high perc"
-    assert (
-        stage_meas.find_qc(10000, 9951) == 500
-    ), "fair data not given fair qc, high perc low"
-    assert (
-        stage_meas.find_qc(10000, 9979) == 500
-    ), "fair data not given fair qc, high perc high"
-    assert (
-        stage_meas.find_qc(10000, 9981) == 600
-    ), "good data not given good qc, high perc"
-
-    assert stage_meas.find_qc(0, 11) == 400, "bad data not given bad qc, low static"
-    assert (
-        stage_meas.find_qc(0, 9) == 500
-    ), "fair data not given fair qc, low static low"
-    assert (
-        stage_meas.find_qc(0, 4) == 500
-    ), "fair data not given fair qc, low static high"
-    assert (
-        stage_meas.find_qc(0, 2) == 600
-    ), "good data not given good qc, low static perc"
+"""Test the data_sources module."""
+import pytest
+from annalist.annalist import Annalist
+
+import hydrobot.data_sources as data_sources
+
+ann = Annalist()
+ann.configure()
+
+
+@pytest.mark.dependency(name="test_get_measurement_dict")
+def test_get_measurement_dict():
+    """Testing the measurement dictionary."""
+    m_dict = data_sources.get_qc_evaluator_dict()
+    assert isinstance(m_dict, dict), "not a dict somehow"
+    assert (
+        "Water Temperature [Dissolved Oxygen sensor]" in m_dict
+    ), "Missing data source water temp"
+    assert (
+        m_dict["Water Temperature [Dissolved Oxygen sensor]"].qc_500_limit > 0
+    ), "Water temp qc_500 limit not set up correctly"
+
+
+@pytest.mark.dependency(depends=["test_get_measurement_dict"])
+def test_get_measurement():
+    """Testing the get_measurement method."""
+    wt_meas = data_sources.get_qc_evaluator(
+        "Water Temperature [Dissolved Oxygen sensor]"
+    )
+    assert wt_meas.qc_500_limit > 0, "Water temp qc_500 limit not set up correctly"
+    assert wt_meas.find_qc(1.3, 0) == 400, "bad data not given bad qc"
+    assert wt_meas.find_qc(1, 0) == 500, "fair data not given fair qc"
+    assert wt_meas.find_qc(0.7, 0) == 600, "good data not given good qc"
+
+    stage_meas = data_sources.get_qc_evaluator("Water level statistics: Point Sample")
+    assert stage_meas.find_qc(1999, 1988) == 400, "bad data not given bad qc, static"
+    assert (
+        stage_meas.find_qc(1999, 1990) == 500
+    ), "fair data not given fair qc, static low"
+    assert (
+        stage_meas.find_qc(1999, 1995) == 500
+    ), "fair data not given fair qc, static high"
+    assert stage_meas.find_qc(1999, 1997) == 600, "good data not given good qc, perc"
+
+    assert stage_meas.find_qc(2001, 1990) == 400, "bad data not given bad qc, perc"
+    assert (
+        stage_meas.find_qc(2001, 1992) == 500
+    ), "fair data not given fair qc, perc low"
+    assert (
+        stage_meas.find_qc(2001, 1996) == 500
+    ), "fair data not given fair qc, perc high"
+    assert stage_meas.find_qc(2001, 1998) == 600, "good data not given good qc, perc"
+
+    assert (
+        stage_meas.find_qc(10000, 9949) == 400
+    ), "bad data not given bad qc, high perc"
+    assert (
+        stage_meas.find_qc(10000, 9951) == 500
+    ), "fair data not given fair qc, high perc low"
+    assert (
+        stage_meas.find_qc(10000, 9979) == 500
+    ), "fair data not given fair qc, high perc high"
+    assert (
+        stage_meas.find_qc(10000, 9981) == 600
+    ), "good data not given good qc, high perc"
+
+    assert stage_meas.find_qc(0, 11) == 400, "bad data not given bad qc, low static"
+    assert (
+        stage_meas.find_qc(0, 9) == 500
+    ), "fair data not given fair qc, low static low"
+    assert (
+        stage_meas.find_qc(0, 4) == 500
+    ), "fair data not given fair qc, low static high"
+    assert (
+        stage_meas.find_qc(0, 2) == 600
+    ), "good data not given good qc, low static perc"
```

### Comparing `hydrobot-0.5.0/tests/test_data_structure.py` & `hydrobot-0.5.1/tests/test_data_structure.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,265 +1,265 @@
-"""Test the XML data structure module."""
-
-from xml.etree import ElementTree
-
-import pandas as pd
-import pytest
-from defusedxml import ElementTree as DefusedElementTree
-
-from hydrobot import data_structure
-
-
-@pytest.fixture()
-def correct_blobs():
-    """
-    PyTest fixture providing a list of correct DataSourceBlob dictionaries for testing.
-
-    Returns
-    -------
-    list
-        A list of dictionaries representing correct DataSourceBlob instances.
-
-    Notes
-    -----
-    This fixture is intended for use in combination with sample_data_source_xml_file.
-    If the xml file is parsed correctly, it should contain the same data as in these
-    fields.
-
-    Example Usage
-    -------------
-    def test_xml_parsing_function(sample_data_source_xml_file, correct_blobs)
-        # Ensure the XML parsing function correctly handles the provided XML file.
-        with open(sample_data_source_xml_file) as f:
-            sample_data_source_xml = f.read()
-        result = example_xml_function(sample_data_source_xml)
-        assert result[0].site_name == correct_blobs[0]["site_name"]
-    """
-    sitename = "Mid Stream at Cowtoilet Farm"
-    datasources = [
-        "General Nastiness",
-        "Number of Actual Whole Human Turds Floating By",
-        "Dead Cow Concentration",
-    ]
-
-    tstypes = [
-        "StdSeries",
-        "StdQualSeries",
-        "CheckSeries",
-    ]
-
-    data_types = [
-        pd.Series,
-        pd.Series,
-        pd.DataFrame,
-    ]
-
-    blob_list = []
-    for ds in datasources:
-        for ts, dt in zip(tstypes, data_types, strict=True):
-            blob = {
-                "site_name": sitename,
-                "data_source_name": ds,
-                "ts_type": ts,
-                "data_type": dt,
-            }
-            blob_list.append(blob)
-
-    return blob_list
-
-
-def test_parse_xml_file_object(sample_data_source_xml_file, correct_blobs):
-    """
-    Test the parse_xml function with an XML file object.
-
-    Parameters
-    ----------
-    sample_data_source_xml_file : pytest fixture
-        The path to a sample XML file for testing.
-    correct_blobs : pytest fixture
-        A list of correct DataSourceBlob dictionaries for comparison.
-
-    Notes
-    -----
-    This test function checks the behavior of the parse_xml function when provided
-    with an open file object representing an XML file. It compares the parsed
-    DataSourceBlob instances with a list of correct configurations.
-
-    Assertions
-    ----------
-    - For each parsed DataSourceBlob instance, assert that the 'site_name' matches
-      the corresponding value in the correct_blobs list.
-    - For each parsed DataSourceBlob instance, assert that the 'data_source.name'
-      matches the corresponding value in the correct_blobs list.
-    - For each parsed DataSourceBlob instance, assert that the 'data_source.ts_type'
-      matches the corresponding value in the correct_blobs list.
-    """
-    with open(sample_data_source_xml_file) as f:
-        sample_data_source_xml = f
-
-        blob_list = data_structure.parse_xml(sample_data_source_xml)
-
-        for i, blob in enumerate(blob_list):
-            assert blob.site_name == correct_blobs[i]["site_name"]
-            assert blob.data_source.name == correct_blobs[i]["data_source_name"]
-            assert blob.data_source.ts_type == correct_blobs[i]["ts_type"]
-            assert isinstance(blob.data.timeseries, correct_blobs[i]["data_type"])
-
-
-def test_parse_xml_string(sample_data_source_xml_file, correct_blobs):
-    """
-    Test the parse_xml function with an XML string.
-
-    Parameters
-    ----------
-    sample_data_source_xml_file : pytest fixture
-        The path to a sample XML file for testing.
-    correct_blobs : pytest fixture
-        A list of correct DataSourceBlob dictionaries for comparison.
-
-    Notes
-    -----
-    This test function checks the behavior of the parse_xml function when provided
-    with an XML string. It compares the parsed DataSourceBlob instances with a list
-    of correct configurations.
-
-    Assertions
-    ----------
-    - For each parsed DataSourceBlob instance, assert that the 'site_name' matches
-      the corresponding value in the correct_blobs list.
-    - For each parsed DataSourceBlob instance, assert that the 'data_source.name'
-      matches the corresponding value in the correct_blobs list.
-    - For each parsed DataSourceBlob instance, assert that the 'data_source.ts_type'
-      matches the corresponding value in the correct_blobs list.
-    """
-    with open(sample_data_source_xml_file) as f:
-        sample_data_source_xml = f.read()
-
-    blob_list = data_structure.parse_xml(sample_data_source_xml)
-
-    for i, blob in enumerate(blob_list):
-        assert blob.site_name == correct_blobs[i]["site_name"]
-        assert blob.data_source.name == correct_blobs[i]["data_source_name"]
-        assert blob.data_source.ts_type == correct_blobs[i]["ts_type"]
-        assert isinstance(blob.data.timeseries, correct_blobs[i]["data_type"])
-
-
-def test_parse_xml_bytes(sample_data_source_xml_file, correct_blobs):
-    """
-    Test the parse_xml function with XML content provided as bytes.
-
-    Parameters
-    ----------
-    sample_data_source_xml_file : pytest fixture
-        The path to a sample XML file for testing.
-    correct_blobs : pytest fixture
-        A list of correct DataSourceBlob dictionaries for comparison.
-
-    Notes
-    -----
-    This test function checks the behavior of the parse_xml function when provided
-    with XML content read as bytes. It compares the parsed DataSourceBlob instances
-    with a list of correct configurations.
-
-    Assertions
-    ----------
-    - For each parsed DataSourceBlob instance, assert that the 'site_name' matches
-      the corresponding value in the correct_blobs list.
-    - For each parsed DataSourceBlob instance, assert that the 'data_source.name'
-      matches the corresponding value in the correct_blobs list.
-    - For each parsed DataSourceBlob instance, assert that the 'data_source.ts_type'
-      matches the corresponding value in the correct_blobs list.
-    """
-    with open(sample_data_source_xml_file, "rb") as f:
-        sample_data_source_xml = f.read()
-
-    blob_list = data_structure.parse_xml(sample_data_source_xml)
-
-    for i, blob in enumerate(blob_list):
-        assert blob.site_name == correct_blobs[i]["site_name"]
-        assert blob.data_source.name == correct_blobs[i]["data_source_name"]
-        assert blob.data_source.ts_type == correct_blobs[i]["ts_type"]
-        assert isinstance(blob.data.timeseries, correct_blobs[i]["data_type"])
-
-
-def test_parse_xml_etree(sample_data_source_xml_file, correct_blobs):
-    """
-    Test the parse_xml function with an XML ElementTree object.
-
-    Parameters
-    ----------
-    sample_data_source_xml_file : pytest fixture
-        The path to a sample XML file for testing.
-    correct_blobs : pytest fixture
-        A list of correct DataSourceBlob dictionaries for comparison.
-
-    Notes
-    -----
-    This test function checks the behavior of the parse_xml function when provided
-    with an XML ElementTree object. It compares the parsed DataSourceBlob instances
-    with a list of correct configurations.
-
-    Assertions
-    ----------
-    - For each parsed DataSourceBlob instance, assert that the 'site_name' matches
-      the corresponding value in the correct_blobs list.
-    - For each parsed DataSourceBlob instance, assert that the 'data_source.name'
-      matches the corresponding value in the correct_blobs list.
-    - For each parsed DataSourceBlob instance, assert that the 'data_source.ts_type'
-      matches the corresponding value in the correct_blobs list.
-    """
-    with open(sample_data_source_xml_file) as f:
-        xml_string = f.read()
-        sample_data_source_xml = DefusedElementTree.fromstring(xml_string)
-
-    blob_list = data_structure.parse_xml(sample_data_source_xml)
-
-    for i, blob in enumerate(blob_list):
-        assert blob.site_name == correct_blobs[i]["site_name"]
-        assert blob.data_source.name == correct_blobs[i]["data_source_name"]
-        assert blob.data_source.ts_type == correct_blobs[i]["ts_type"]
-        assert isinstance(blob.data.timeseries, correct_blobs[i]["data_type"])
-
-
-def test_data_source_to_xml_tree(tmp_path, sample_data_source_xml_file):
-    """
-    Test the to_xml_tree method of DataSourceBlob for generating correct XML output.
-
-    Parameters
-    ----------
-    tmp_path : pytest fixture
-        A fixture providing a temporary directory path for storing the test output.
-    sample_data_source_xml_file : pytest fixture
-        The path to a sample XML file for testing.
-
-    Notes
-    -----
-    This test function checks the correctness of the to_xml_tree method of
-    DataSourceBlob when generating XML output. It compares the generated XML with the
-    expected XML from the sample data source XML file. Before comparison, the xml from
-    both sources are canonicalized (reformatted into a standardized format),
-    and whitespace is removed.
-
-    Assertions
-    ----------
-    - Assert that the canonicalized content of the generated XML matches the
-        canonicalized content of the expected XML from the sample data source XML file.
-    """
-    with open(sample_data_source_xml_file) as f:
-        sample_data_source_xml = f.read()
-
-    blob_list = data_structure.parse_xml(sample_data_source_xml)
-
-    output_path = tmp_path / "output.xml"
-    # output_path = "output.xml"
-    data_structure.write_hilltop_xml(blob_list, output_path)
-
-    with open(output_path) as f:
-        output_xml = f.read()
-
-    assert ElementTree.canonicalize(
-        sample_data_source_xml,
-        strip_text=True,
-    ) == ElementTree.canonicalize(
-        output_xml,
-        strip_text=True,
-    )
+"""Test the XML data structure module."""
+
+from xml.etree import ElementTree
+
+import pandas as pd
+import pytest
+from defusedxml import ElementTree as DefusedElementTree
+
+from hydrobot import data_structure
+
+
+@pytest.fixture()
+def correct_blobs():
+    """
+    PyTest fixture providing a list of correct DataSourceBlob dictionaries for testing.
+
+    Returns
+    -------
+    list
+        A list of dictionaries representing correct DataSourceBlob instances.
+
+    Notes
+    -----
+    This fixture is intended for use in combination with sample_data_source_xml_file.
+    If the xml file is parsed correctly, it should contain the same data as in these
+    fields.
+
+    Example Usage
+    -------------
+    def test_xml_parsing_function(sample_data_source_xml_file, correct_blobs)
+        # Ensure the XML parsing function correctly handles the provided XML file.
+        with open(sample_data_source_xml_file) as f:
+            sample_data_source_xml = f.read()
+        result = example_xml_function(sample_data_source_xml)
+        assert result[0].site_name == correct_blobs[0]["site_name"]
+    """
+    sitename = "Mid Stream at Cowtoilet Farm"
+    datasources = [
+        "General Nastiness",
+        "Number of Actual Whole Human Turds Floating By",
+        "Dead Cow Concentration",
+    ]
+
+    tstypes = [
+        "StdSeries",
+        "StdQualSeries",
+        "CheckSeries",
+    ]
+
+    data_types = [
+        pd.Series,
+        pd.Series,
+        pd.DataFrame,
+    ]
+
+    blob_list = []
+    for ds in datasources:
+        for ts, dt in zip(tstypes, data_types, strict=True):
+            blob = {
+                "site_name": sitename,
+                "data_source_name": ds,
+                "ts_type": ts,
+                "data_type": dt,
+            }
+            blob_list.append(blob)
+
+    return blob_list
+
+
+def test_parse_xml_file_object(sample_data_source_xml_file, correct_blobs):
+    """
+    Test the parse_xml function with an XML file object.
+
+    Parameters
+    ----------
+    sample_data_source_xml_file : pytest fixture
+        The path to a sample XML file for testing.
+    correct_blobs : pytest fixture
+        A list of correct DataSourceBlob dictionaries for comparison.
+
+    Notes
+    -----
+    This test function checks the behavior of the parse_xml function when provided
+    with an open file object representing an XML file. It compares the parsed
+    DataSourceBlob instances with a list of correct configurations.
+
+    Assertions
+    ----------
+    - For each parsed DataSourceBlob instance, assert that the 'site_name' matches
+      the corresponding value in the correct_blobs list.
+    - For each parsed DataSourceBlob instance, assert that the 'data_source.name'
+      matches the corresponding value in the correct_blobs list.
+    - For each parsed DataSourceBlob instance, assert that the 'data_source.ts_type'
+      matches the corresponding value in the correct_blobs list.
+    """
+    with open(sample_data_source_xml_file) as f:
+        sample_data_source_xml = f
+
+        blob_list = data_structure.parse_xml(sample_data_source_xml)
+
+        for i, blob in enumerate(blob_list):
+            assert blob.site_name == correct_blobs[i]["site_name"]
+            assert blob.data_source.name == correct_blobs[i]["data_source_name"]
+            assert blob.data_source.ts_type == correct_blobs[i]["ts_type"]
+            assert isinstance(blob.data.timeseries, correct_blobs[i]["data_type"])
+
+
+def test_parse_xml_string(sample_data_source_xml_file, correct_blobs):
+    """
+    Test the parse_xml function with an XML string.
+
+    Parameters
+    ----------
+    sample_data_source_xml_file : pytest fixture
+        The path to a sample XML file for testing.
+    correct_blobs : pytest fixture
+        A list of correct DataSourceBlob dictionaries for comparison.
+
+    Notes
+    -----
+    This test function checks the behavior of the parse_xml function when provided
+    with an XML string. It compares the parsed DataSourceBlob instances with a list
+    of correct configurations.
+
+    Assertions
+    ----------
+    - For each parsed DataSourceBlob instance, assert that the 'site_name' matches
+      the corresponding value in the correct_blobs list.
+    - For each parsed DataSourceBlob instance, assert that the 'data_source.name'
+      matches the corresponding value in the correct_blobs list.
+    - For each parsed DataSourceBlob instance, assert that the 'data_source.ts_type'
+      matches the corresponding value in the correct_blobs list.
+    """
+    with open(sample_data_source_xml_file) as f:
+        sample_data_source_xml = f.read()
+
+    blob_list = data_structure.parse_xml(sample_data_source_xml)
+
+    for i, blob in enumerate(blob_list):
+        assert blob.site_name == correct_blobs[i]["site_name"]
+        assert blob.data_source.name == correct_blobs[i]["data_source_name"]
+        assert blob.data_source.ts_type == correct_blobs[i]["ts_type"]
+        assert isinstance(blob.data.timeseries, correct_blobs[i]["data_type"])
+
+
+def test_parse_xml_bytes(sample_data_source_xml_file, correct_blobs):
+    """
+    Test the parse_xml function with XML content provided as bytes.
+
+    Parameters
+    ----------
+    sample_data_source_xml_file : pytest fixture
+        The path to a sample XML file for testing.
+    correct_blobs : pytest fixture
+        A list of correct DataSourceBlob dictionaries for comparison.
+
+    Notes
+    -----
+    This test function checks the behavior of the parse_xml function when provided
+    with XML content read as bytes. It compares the parsed DataSourceBlob instances
+    with a list of correct configurations.
+
+    Assertions
+    ----------
+    - For each parsed DataSourceBlob instance, assert that the 'site_name' matches
+      the corresponding value in the correct_blobs list.
+    - For each parsed DataSourceBlob instance, assert that the 'data_source.name'
+      matches the corresponding value in the correct_blobs list.
+    - For each parsed DataSourceBlob instance, assert that the 'data_source.ts_type'
+      matches the corresponding value in the correct_blobs list.
+    """
+    with open(sample_data_source_xml_file, "rb") as f:
+        sample_data_source_xml = f.read()
+
+    blob_list = data_structure.parse_xml(sample_data_source_xml)
+
+    for i, blob in enumerate(blob_list):
+        assert blob.site_name == correct_blobs[i]["site_name"]
+        assert blob.data_source.name == correct_blobs[i]["data_source_name"]
+        assert blob.data_source.ts_type == correct_blobs[i]["ts_type"]
+        assert isinstance(blob.data.timeseries, correct_blobs[i]["data_type"])
+
+
+def test_parse_xml_etree(sample_data_source_xml_file, correct_blobs):
+    """
+    Test the parse_xml function with an XML ElementTree object.
+
+    Parameters
+    ----------
+    sample_data_source_xml_file : pytest fixture
+        The path to a sample XML file for testing.
+    correct_blobs : pytest fixture
+        A list of correct DataSourceBlob dictionaries for comparison.
+
+    Notes
+    -----
+    This test function checks the behavior of the parse_xml function when provided
+    with an XML ElementTree object. It compares the parsed DataSourceBlob instances
+    with a list of correct configurations.
+
+    Assertions
+    ----------
+    - For each parsed DataSourceBlob instance, assert that the 'site_name' matches
+      the corresponding value in the correct_blobs list.
+    - For each parsed DataSourceBlob instance, assert that the 'data_source.name'
+      matches the corresponding value in the correct_blobs list.
+    - For each parsed DataSourceBlob instance, assert that the 'data_source.ts_type'
+      matches the corresponding value in the correct_blobs list.
+    """
+    with open(sample_data_source_xml_file) as f:
+        xml_string = f.read()
+        sample_data_source_xml = DefusedElementTree.fromstring(xml_string)
+
+    blob_list = data_structure.parse_xml(sample_data_source_xml)
+
+    for i, blob in enumerate(blob_list):
+        assert blob.site_name == correct_blobs[i]["site_name"]
+        assert blob.data_source.name == correct_blobs[i]["data_source_name"]
+        assert blob.data_source.ts_type == correct_blobs[i]["ts_type"]
+        assert isinstance(blob.data.timeseries, correct_blobs[i]["data_type"])
+
+
+def test_data_source_to_xml_tree(tmp_path, sample_data_source_xml_file):
+    """
+    Test the to_xml_tree method of DataSourceBlob for generating correct XML output.
+
+    Parameters
+    ----------
+    tmp_path : pytest fixture
+        A fixture providing a temporary directory path for storing the test output.
+    sample_data_source_xml_file : pytest fixture
+        The path to a sample XML file for testing.
+
+    Notes
+    -----
+    This test function checks the correctness of the to_xml_tree method of
+    DataSourceBlob when generating XML output. It compares the generated XML with the
+    expected XML from the sample data source XML file. Before comparison, the xml from
+    both sources are canonicalized (reformatted into a standardized format),
+    and whitespace is removed.
+
+    Assertions
+    ----------
+    - Assert that the canonicalized content of the generated XML matches the
+        canonicalized content of the expected XML from the sample data source XML file.
+    """
+    with open(sample_data_source_xml_file) as f:
+        sample_data_source_xml = f.read()
+
+    blob_list = data_structure.parse_xml(sample_data_source_xml)
+
+    output_path = tmp_path / "output.xml"
+    # output_path = "output.xml"
+    data_structure.write_hilltop_xml(blob_list, output_path)
+
+    with open(output_path) as f:
+        output_xml = f.read()
+
+    assert ElementTree.canonicalize(
+        sample_data_source_xml,
+        strip_text=True,
+    ) == ElementTree.canonicalize(
+        output_xml,
+        strip_text=True,
+    )
```

### Comparing `hydrobot-0.5.0/tests/test_evaluator.py` & `hydrobot-0.5.1/tests/test_evaluator.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,307 +1,307 @@
-"""Test the evaluator module."""
-# import warnings
-# pyright: reportGeneralTypeIssues=false
-
-import numpy as np
-import pandas as pd
-import pytest
-from annalist.annalist import Annalist
-
-import hydrobot.data_sources as data_sources
-import hydrobot.evaluator as evaluator
-
-ann = Annalist()
-ann.configure()
-
-raw_data_dict = {
-    pd.Timestamp("2021-01-01 00:00"): 1.0,
-    pd.Timestamp("2021-01-01 00:15"): 2.0,
-    pd.Timestamp("2021-01-01 00:30"): 10.0,
-    pd.Timestamp("2021-01-01 00:45"): 4.0,
-    pd.Timestamp("2021-01-01 01:00"): 5.0,
-}
-
-gap_data_dict = {
-    pd.Timestamp("2021-01-01 00:00"): np.NaN,
-    pd.Timestamp("2021-01-01 00:15"): 2.0,
-    pd.Timestamp("2021-01-01 00:30"): np.NaN,
-    pd.Timestamp("2021-01-01 00:45"): np.NaN,
-    pd.Timestamp("2021-01-01 01:00"): 5.0,
-    pd.Timestamp("2021-01-01 01:15"): np.NaN,
-    pd.Timestamp("2021-01-01 01:30"): np.NaN,
-    pd.Timestamp("2021-01-01 01:45"): np.NaN,
-    pd.Timestamp("2021-01-01 02:00"): 0.0,
-    pd.Timestamp("2021-01-01 02:15"): 0.0,
-    pd.Timestamp("2021-01-01 02:30"): np.NaN,
-    pd.Timestamp("2021-01-01 02:45"): np.NaN,
-}
-
-check_data_dict = {
-    pd.Timestamp("2021-01-01 00:15"): 2.1,
-    pd.Timestamp("2021-01-01 00:45"): 7.0,
-    pd.Timestamp("2021-01-01 01:00"): 25.0,
-}
-
-qc_data_dict = {
-    pd.Timestamp("2021-01-01 00:00"): 600,
-    pd.Timestamp("2021-01-01 00:15"): 500,
-    pd.Timestamp("2021-01-01 00:45"): 600,
-    pd.Timestamp("2021-01-01 01:00"): 500,
-    pd.Timestamp("2021-01-01 01:30"): 500,
-    pd.Timestamp("2021-01-01 02:15"): 600,
-    pd.Timestamp("2021-01-01 02:45"): 600,
-}
-
-
-@pytest.fixture()
-def raw_data():
-    """Example data for testing. Do not change these values."""
-    data_series = pd.Series(raw_data_dict)
-    return data_series
-
-
-@pytest.fixture()
-def gap_data():
-    """Example data for testing. Do not change these values."""
-    data_series = pd.Series(gap_data_dict)
-    return data_series
-
-
-@pytest.fixture()
-def check_data():
-    """Example data for testing. Do not change these values."""
-    data_series = pd.Series(check_data_dict)
-    return data_series
-
-
-@pytest.fixture()
-def qc_data():
-    """Example data for testing. Do not change these values."""
-    data_series = pd.Series(qc_data_dict)
-    return data_series
-
-
-@pytest.mark.dependency(name="test_gap_finder")
-def test_gap_finder(raw_data, gap_data):
-    """Test the gap finder function."""
-    no_gap_list = evaluator.gap_finder(raw_data)
-    assert no_gap_list == [], "Gap found where there should be no gap"
-
-    gap_list = evaluator.gap_finder(gap_data)
-    assert len(gap_list) >= 4, "gap_finder did not find one or more of the gaps"
-    assert len(gap_list) <= 4, "gap_finder found too many gaps"
-    assert gap_list[0][1] == 1, "gap length of 1 not calculated correctly"
-    assert gap_list[1][1] == 2, "gap length of 2 not calculated correctly"
-    assert gap_list[2][1] == 3, "gap length of 3 not calculated correctly"
-
-
-@pytest.mark.dependency(name="test_small_gap_closer")
-def test_small_gap_closer(raw_data, gap_data):
-    """Test the small gap closer function."""
-    # No gaps here, nothing should happen
-    no_gaps = evaluator.small_gap_closer(raw_data, 1)
-    assert no_gaps.equals(raw_data), "Data without gaps should not be modified, but was"
-
-    # All gaps should be closed
-    removed_gaps = evaluator.small_gap_closer(gap_data, 5)
-    assert len(removed_gaps) == 4, "Data changed during gap closing"
-
-    # Should still have one gap of len 3, others closed
-    some_gaps = evaluator.small_gap_closer(gap_data, 2)
-    assert len(some_gaps) == 7, "gap_finder did not find one or more of the gaps"
-
-
-@pytest.mark.dependency(depends=["test_gap_finder", "test_small_gap_closer"])
-def test_small_gap_closer_part2(gap_data):
-    """Test the small gap closer some more."""
-    # All gaps should be closed
-    removed_gaps = evaluator.small_gap_closer(gap_data, 5)
-    assert evaluator.gap_finder(removed_gaps) == [], "Gap not closed!"
-
-    # Should still have one gap of len 3, others closed
-    some_gaps = evaluator.small_gap_closer(gap_data, 2)
-    assert len(evaluator.gap_finder(some_gaps)) < 2, "Not enough gaps were removed"
-    assert len(evaluator.gap_finder(some_gaps)) > 0, "Too many gaps were removed"
-    assert (
-        evaluator.gap_finder(some_gaps)[0][1] == 3
-    ), "incorrect gap length after gap closure"
-
-
-def test_find_nearest_time(gap_data):
-    """Test the find nearest time function."""
-    assert evaluator.find_nearest_time(
-        gap_data, pd.Timestamp("2021-01-01 01:00")
-    ) == pd.Timestamp("2021-01-01 01:00"), "does not find exact value"
-    assert evaluator.find_nearest_time(
-        gap_data, pd.Timestamp("2021-01-01 01:07")
-    ) == pd.Timestamp("2021-01-01 01:00"), "does not round down correctly"
-    assert evaluator.find_nearest_time(
-        gap_data, pd.Timestamp("2021-01-01 01:08")
-    ) == pd.Timestamp(
-        "2021-01-01 01:15"
-    ), "does not round up or does not round up to null correctly"
-    assert evaluator.find_nearest_time(
-        gap_data, pd.Timestamp("2021-01-01 01:23")
-    ) == pd.Timestamp("2021-01-01 01:30"), "middle of nulls not reading correctly"
-    assert evaluator.find_nearest_time(
-        gap_data, pd.Timestamp("2021-01-01 00:00")
-    ) == pd.Timestamp("2021-01-01 00:00"), "start time not accepted"
-    assert evaluator.find_nearest_time(
-        gap_data, pd.Timestamp("2021-01-01 02:45")
-    ) == pd.Timestamp("2021-01-01 02:45"), "end time not accepted"
-    with pytest.raises(KeyError):
-        # out of range forwards
-        evaluator.find_nearest_time(gap_data, pd.Timestamp("2021-01-01 02:46"))
-    with pytest.raises(KeyError):
-        # out of range backwards
-        evaluator.find_nearest_time(gap_data, pd.Timestamp("2020-12-31 23:59"))
-
-
-def test_find_nearest_valid_time(gap_data, qc_data):
-    """Test the finc nearest valid time function."""
-    assert evaluator.find_nearest_valid_time(
-        qc_data, pd.Timestamp("2021-01-01 01:00")
-    ) == pd.Timestamp("2021-01-01 01:00"), "does not find exact value"
-    assert evaluator.find_nearest_valid_time(
-        qc_data, pd.Timestamp("2021-01-01 01:07")
-    ) == pd.Timestamp("2021-01-01 01:00"), "does not round down correctly"
-    assert evaluator.find_nearest_valid_time(
-        qc_data, pd.Timestamp("2021-01-01 01:08")
-    ) == pd.Timestamp(
-        "2021-01-01 01:00"
-    ), "does not round down when round up would lead to null"
-    assert evaluator.find_nearest_valid_time(
-        gap_data, pd.Timestamp("2021-01-01 01:23")
-    ) == pd.Timestamp("2021-01-01 01:00"), "middle of nulls not reading correctly"
-    assert evaluator.find_nearest_valid_time(
-        qc_data, pd.Timestamp("2021-01-01 00:00")
-    ) == pd.Timestamp("2021-01-01 00:00"), "start time not accepted"
-    assert evaluator.find_nearest_valid_time(
-        qc_data, pd.Timestamp("2021-01-01 02:45")
-    ) == pd.Timestamp("2021-01-01 02:45"), "end time not accepted"
-    with pytest.raises(KeyError):
-        # out of range forwards
-        evaluator.find_nearest_valid_time(gap_data, pd.Timestamp("2021-01-01 02:46"))
-    with pytest.raises(KeyError):
-        # out of range backwards
-        evaluator.find_nearest_valid_time(gap_data, pd.Timestamp("2020-12-31 23:59"))
-
-
-def test_check_data_quality_code(raw_data, check_data):
-    """Test check data quality code function."""
-    meas = data_sources.QualityCodeEvaluator(10, 2.0)
-    with pytest.warns(Warning):
-        assert (
-            len(evaluator.check_data_quality_code(raw_data, pd.Series({}), meas)) == 1
-        ), "fails for empty check data series"
-    output = evaluator.check_data_quality_code(raw_data, check_data, meas)
-    assert (
-        len(output) == len(check_data) + 1
-    ), "different amount of QC values than check data values"
-    assert output.iloc[0] == 600, "QC 600 test failed"
-    assert output.iloc[1] == 500, "QC 500 test failed"
-    assert output.iloc[2] == 400, "QC 400 test failed"
-    assert output.iloc[3] == 0, "Should have QC 0 at the end"
-
-
-def test_base_data_qc_filter(gap_data, qc_data):
-    """Test base data QC filter function."""
-    assert len(
-        evaluator.base_data_qc_filter(
-            gap_data, pd.Series({pd.Timestamp("2021-01-01 00:00"): True})
-        )
-    ) == len(gap_data), "True filter removed data"
-    assert (
-        len(
-            evaluator.base_data_qc_filter(
-                gap_data, pd.Series({pd.Timestamp("2021-01-01 00:00"): False})
-            )
-        )
-        == 0
-    ), "False filter did not delete all data"
-    data_600 = evaluator.base_data_qc_filter(gap_data, qc_data == 600)
-    assert pd.Timestamp("2021-01-01 00:00") in data_600
-    assert pd.Timestamp("2021-01-01 00:15") not in data_600
-    assert pd.Timestamp("2021-01-01 00:30") not in data_600
-    assert pd.Timestamp("2021-01-01 00:45") in data_600
-    assert pd.Timestamp("2021-01-01 01:00") not in data_600
-    assert pd.Timestamp("2021-01-01 01:15") not in data_600
-    assert pd.Timestamp("2021-01-01 02:30") in data_600
-    assert pd.Timestamp("2021-01-01 02:45") in data_600
-
-    data_500 = evaluator.base_data_qc_filter(gap_data, qc_data == 500)
-    assert pd.Timestamp("2021-01-01 00:00") not in data_500
-    assert pd.Timestamp("2021-01-01 00:15") in data_500
-    assert pd.Timestamp("2021-01-01 00:30") in data_500
-    assert pd.Timestamp("2021-01-01 00:45") not in data_500
-    assert pd.Timestamp("2021-01-01 01:00") in data_500
-    assert pd.Timestamp("2021-01-01 01:15") in data_500
-    assert pd.Timestamp("2021-01-01 02:30") not in data_500
-    assert pd.Timestamp("2021-01-01 02:45") not in data_500
-
-
-def test_base_data_meets_qc(gap_data, qc_data):
-    """Test the base data meets QC function."""
-    assert len(
-        evaluator.base_data_meets_qc(
-            gap_data, pd.Series({pd.Timestamp("2021-01-01 00:00"): 600}), 600
-        )
-    ) == len(gap_data), "True filter removed data"
-    assert (
-        len(
-            evaluator.base_data_meets_qc(
-                gap_data, pd.Series({pd.Timestamp("2021-01-01 00:00"): 500}), 600
-            )
-        )
-        == 0
-    ), "False filter did not delete all data"
-    data_600 = evaluator.base_data_meets_qc(gap_data, qc_data, 600)
-    assert pd.Timestamp("2021-01-01 00:00") in data_600
-    assert pd.Timestamp("2021-01-01 00:15") not in data_600
-    assert pd.Timestamp("2021-01-01 00:30") not in data_600
-    assert pd.Timestamp("2021-01-01 00:45") in data_600
-    assert pd.Timestamp("2021-01-01 01:00") not in data_600
-    assert pd.Timestamp("2021-01-01 01:15") not in data_600
-    assert pd.Timestamp("2021-01-01 02:30") in data_600
-    assert pd.Timestamp("2021-01-01 02:45") in data_600
-
-    data_500 = evaluator.base_data_meets_qc(gap_data, qc_data, 500)
-    assert pd.Timestamp("2021-01-01 00:00") not in data_500
-    assert pd.Timestamp("2021-01-01 00:15") in data_500
-    assert pd.Timestamp("2021-01-01 00:30") in data_500
-    assert pd.Timestamp("2021-01-01 00:45") not in data_500
-    assert pd.Timestamp("2021-01-01 01:00") in data_500
-    assert pd.Timestamp("2021-01-01 01:15") in data_500
-    assert pd.Timestamp("2021-01-01 02:30") not in data_500
-    assert pd.Timestamp("2021-01-01 02:45") not in data_500
-
-
-def test_missing_data_quality_code(gap_data, qc_data):
-    """Test the missing data quality code function."""
-    no_gap_qc = evaluator.missing_data_quality_code(
-        gap_data.fillna(3), qc_data, gap_limit=0
-    )
-    assert no_gap_qc.equals(qc_data), "QC data modified when there are no gaps"
-
-    new_qc = evaluator.missing_data_quality_code(gap_data, qc_data, gap_limit=0)
-    assert new_qc[pd.Timestamp("2021-01-01 00:00")] == 100, "Starting gap not added"
-    assert new_qc[pd.Timestamp("2021-01-01 00:15")] == 500, "Starting gap not closed"
-    assert new_qc[pd.Timestamp("2021-01-01 02:30")] == 100, "Ending gap not added"
-    assert pd.Timestamp("2021-01-01 01:30") not in new_qc, "Mid-gap QC not replaced"
-    assert new_qc[pd.Timestamp("2021-01-01 02:00")] == 500, "Gap in middle not closed"
-
-
-def test_max_qc_limiter(qc_data):
-    """Test max_QC_limiter."""
-    limited_qcs = evaluator.max_qc_limiter(qc_data, 500)
-    assert (limited_qcs == 500).all(), "maximum not enforced"
-    assert len(limited_qcs) == len(qc_data), "data going missing or being added"
-    assert (limited_qcs.index == qc_data.index).all(), "index modified"
-
-    unlimited_power = evaluator.max_qc_limiter(qc_data, 600)
-    assert (unlimited_power == qc_data).all(), "maximum over enforced"
-    assert len(unlimited_power) == len(qc_data), "data going missing or being added"
-    assert (unlimited_power.index == qc_data.index).all(), "index modified"
-
-    whoops_maybe_the_power_had_a_limit = evaluator.max_qc_limiter(pd.Series({}), 600)
-    assert (whoops_maybe_the_power_had_a_limit == pd.Series({})).all(), "trivial case"
+"""Test the evaluator module."""
+# import warnings
+# pyright: reportGeneralTypeIssues=false
+
+import numpy as np
+import pandas as pd
+import pytest
+from annalist.annalist import Annalist
+
+import hydrobot.data_sources as data_sources
+import hydrobot.evaluator as evaluator
+
+ann = Annalist()
+ann.configure()
+
+raw_data_dict = {
+    pd.Timestamp("2021-01-01 00:00"): 1.0,
+    pd.Timestamp("2021-01-01 00:15"): 2.0,
+    pd.Timestamp("2021-01-01 00:30"): 10.0,
+    pd.Timestamp("2021-01-01 00:45"): 4.0,
+    pd.Timestamp("2021-01-01 01:00"): 5.0,
+}
+
+gap_data_dict = {
+    pd.Timestamp("2021-01-01 00:00"): np.NaN,
+    pd.Timestamp("2021-01-01 00:15"): 2.0,
+    pd.Timestamp("2021-01-01 00:30"): np.NaN,
+    pd.Timestamp("2021-01-01 00:45"): np.NaN,
+    pd.Timestamp("2021-01-01 01:00"): 5.0,
+    pd.Timestamp("2021-01-01 01:15"): np.NaN,
+    pd.Timestamp("2021-01-01 01:30"): np.NaN,
+    pd.Timestamp("2021-01-01 01:45"): np.NaN,
+    pd.Timestamp("2021-01-01 02:00"): 0.0,
+    pd.Timestamp("2021-01-01 02:15"): 0.0,
+    pd.Timestamp("2021-01-01 02:30"): np.NaN,
+    pd.Timestamp("2021-01-01 02:45"): np.NaN,
+}
+
+check_data_dict = {
+    pd.Timestamp("2021-01-01 00:15"): 2.1,
+    pd.Timestamp("2021-01-01 00:45"): 7.0,
+    pd.Timestamp("2021-01-01 01:00"): 25.0,
+}
+
+qc_data_dict = {
+    pd.Timestamp("2021-01-01 00:00"): 600,
+    pd.Timestamp("2021-01-01 00:15"): 500,
+    pd.Timestamp("2021-01-01 00:45"): 600,
+    pd.Timestamp("2021-01-01 01:00"): 500,
+    pd.Timestamp("2021-01-01 01:30"): 500,
+    pd.Timestamp("2021-01-01 02:15"): 600,
+    pd.Timestamp("2021-01-01 02:45"): 600,
+}
+
+
+@pytest.fixture()
+def raw_data():
+    """Example data for testing. Do not change these values."""
+    data_series = pd.Series(raw_data_dict)
+    return data_series
+
+
+@pytest.fixture()
+def gap_data():
+    """Example data for testing. Do not change these values."""
+    data_series = pd.Series(gap_data_dict)
+    return data_series
+
+
+@pytest.fixture()
+def check_data():
+    """Example data for testing. Do not change these values."""
+    data_series = pd.Series(check_data_dict)
+    return data_series
+
+
+@pytest.fixture()
+def qc_data():
+    """Example data for testing. Do not change these values."""
+    data_series = pd.Series(qc_data_dict)
+    return data_series
+
+
+@pytest.mark.dependency(name="test_gap_finder")
+def test_gap_finder(raw_data, gap_data):
+    """Test the gap finder function."""
+    no_gap_list = evaluator.gap_finder(raw_data)
+    assert no_gap_list == [], "Gap found where there should be no gap"
+
+    gap_list = evaluator.gap_finder(gap_data)
+    assert len(gap_list) >= 4, "gap_finder did not find one or more of the gaps"
+    assert len(gap_list) <= 4, "gap_finder found too many gaps"
+    assert gap_list[0][1] == 1, "gap length of 1 not calculated correctly"
+    assert gap_list[1][1] == 2, "gap length of 2 not calculated correctly"
+    assert gap_list[2][1] == 3, "gap length of 3 not calculated correctly"
+
+
+@pytest.mark.dependency(name="test_small_gap_closer")
+def test_small_gap_closer(raw_data, gap_data):
+    """Test the small gap closer function."""
+    # No gaps here, nothing should happen
+    no_gaps = evaluator.small_gap_closer(raw_data, 1)
+    assert no_gaps.equals(raw_data), "Data without gaps should not be modified, but was"
+
+    # All gaps should be closed
+    removed_gaps = evaluator.small_gap_closer(gap_data, 5)
+    assert len(removed_gaps) == 4, "Data changed during gap closing"
+
+    # Should still have one gap of len 3, others closed
+    some_gaps = evaluator.small_gap_closer(gap_data, 2)
+    assert len(some_gaps) == 7, "gap_finder did not find one or more of the gaps"
+
+
+@pytest.mark.dependency(depends=["test_gap_finder", "test_small_gap_closer"])
+def test_small_gap_closer_part2(gap_data):
+    """Test the small gap closer some more."""
+    # All gaps should be closed
+    removed_gaps = evaluator.small_gap_closer(gap_data, 5)
+    assert evaluator.gap_finder(removed_gaps) == [], "Gap not closed!"
+
+    # Should still have one gap of len 3, others closed
+    some_gaps = evaluator.small_gap_closer(gap_data, 2)
+    assert len(evaluator.gap_finder(some_gaps)) < 2, "Not enough gaps were removed"
+    assert len(evaluator.gap_finder(some_gaps)) > 0, "Too many gaps were removed"
+    assert (
+        evaluator.gap_finder(some_gaps)[0][1] == 3
+    ), "incorrect gap length after gap closure"
+
+
+def test_find_nearest_time(gap_data):
+    """Test the find nearest time function."""
+    assert evaluator.find_nearest_time(
+        gap_data, pd.Timestamp("2021-01-01 01:00")
+    ) == pd.Timestamp("2021-01-01 01:00"), "does not find exact value"
+    assert evaluator.find_nearest_time(
+        gap_data, pd.Timestamp("2021-01-01 01:07")
+    ) == pd.Timestamp("2021-01-01 01:00"), "does not round down correctly"
+    assert evaluator.find_nearest_time(
+        gap_data, pd.Timestamp("2021-01-01 01:08")
+    ) == pd.Timestamp(
+        "2021-01-01 01:15"
+    ), "does not round up or does not round up to null correctly"
+    assert evaluator.find_nearest_time(
+        gap_data, pd.Timestamp("2021-01-01 01:23")
+    ) == pd.Timestamp("2021-01-01 01:30"), "middle of nulls not reading correctly"
+    assert evaluator.find_nearest_time(
+        gap_data, pd.Timestamp("2021-01-01 00:00")
+    ) == pd.Timestamp("2021-01-01 00:00"), "start time not accepted"
+    assert evaluator.find_nearest_time(
+        gap_data, pd.Timestamp("2021-01-01 02:45")
+    ) == pd.Timestamp("2021-01-01 02:45"), "end time not accepted"
+    with pytest.raises(KeyError):
+        # out of range forwards
+        evaluator.find_nearest_time(gap_data, pd.Timestamp("2021-01-01 02:46"))
+    with pytest.raises(KeyError):
+        # out of range backwards
+        evaluator.find_nearest_time(gap_data, pd.Timestamp("2020-12-31 23:59"))
+
+
+def test_find_nearest_valid_time(gap_data, qc_data):
+    """Test the finc nearest valid time function."""
+    assert evaluator.find_nearest_valid_time(
+        qc_data, pd.Timestamp("2021-01-01 01:00")
+    ) == pd.Timestamp("2021-01-01 01:00"), "does not find exact value"
+    assert evaluator.find_nearest_valid_time(
+        qc_data, pd.Timestamp("2021-01-01 01:07")
+    ) == pd.Timestamp("2021-01-01 01:00"), "does not round down correctly"
+    assert evaluator.find_nearest_valid_time(
+        qc_data, pd.Timestamp("2021-01-01 01:08")
+    ) == pd.Timestamp(
+        "2021-01-01 01:00"
+    ), "does not round down when round up would lead to null"
+    assert evaluator.find_nearest_valid_time(
+        gap_data, pd.Timestamp("2021-01-01 01:23")
+    ) == pd.Timestamp("2021-01-01 01:00"), "middle of nulls not reading correctly"
+    assert evaluator.find_nearest_valid_time(
+        qc_data, pd.Timestamp("2021-01-01 00:00")
+    ) == pd.Timestamp("2021-01-01 00:00"), "start time not accepted"
+    assert evaluator.find_nearest_valid_time(
+        qc_data, pd.Timestamp("2021-01-01 02:45")
+    ) == pd.Timestamp("2021-01-01 02:45"), "end time not accepted"
+    with pytest.raises(KeyError):
+        # out of range forwards
+        evaluator.find_nearest_valid_time(gap_data, pd.Timestamp("2021-01-01 02:46"))
+    with pytest.raises(KeyError):
+        # out of range backwards
+        evaluator.find_nearest_valid_time(gap_data, pd.Timestamp("2020-12-31 23:59"))
+
+
+def test_check_data_quality_code(raw_data, check_data):
+    """Test check data quality code function."""
+    meas = data_sources.QualityCodeEvaluator(10, 2.0)
+    with pytest.warns(Warning):
+        assert (
+            len(evaluator.check_data_quality_code(raw_data, pd.Series({}), meas)) == 1
+        ), "fails for empty check data series"
+    output = evaluator.check_data_quality_code(raw_data, check_data, meas)
+    assert (
+        len(output) == len(check_data) + 1
+    ), "different amount of QC values than check data values"
+    assert output.iloc[0] == 600, "QC 600 test failed"
+    assert output.iloc[1] == 500, "QC 500 test failed"
+    assert output.iloc[2] == 400, "QC 400 test failed"
+    assert output.iloc[3] == 0, "Should have QC 0 at the end"
+
+
+def test_base_data_qc_filter(gap_data, qc_data):
+    """Test base data QC filter function."""
+    assert len(
+        evaluator.base_data_qc_filter(
+            gap_data, pd.Series({pd.Timestamp("2021-01-01 00:00"): True})
+        )
+    ) == len(gap_data), "True filter removed data"
+    assert (
+        len(
+            evaluator.base_data_qc_filter(
+                gap_data, pd.Series({pd.Timestamp("2021-01-01 00:00"): False})
+            )
+        )
+        == 0
+    ), "False filter did not delete all data"
+    data_600 = evaluator.base_data_qc_filter(gap_data, qc_data == 600)
+    assert pd.Timestamp("2021-01-01 00:00") in data_600
+    assert pd.Timestamp("2021-01-01 00:15") not in data_600
+    assert pd.Timestamp("2021-01-01 00:30") not in data_600
+    assert pd.Timestamp("2021-01-01 00:45") in data_600
+    assert pd.Timestamp("2021-01-01 01:00") not in data_600
+    assert pd.Timestamp("2021-01-01 01:15") not in data_600
+    assert pd.Timestamp("2021-01-01 02:30") in data_600
+    assert pd.Timestamp("2021-01-01 02:45") in data_600
+
+    data_500 = evaluator.base_data_qc_filter(gap_data, qc_data == 500)
+    assert pd.Timestamp("2021-01-01 00:00") not in data_500
+    assert pd.Timestamp("2021-01-01 00:15") in data_500
+    assert pd.Timestamp("2021-01-01 00:30") in data_500
+    assert pd.Timestamp("2021-01-01 00:45") not in data_500
+    assert pd.Timestamp("2021-01-01 01:00") in data_500
+    assert pd.Timestamp("2021-01-01 01:15") in data_500
+    assert pd.Timestamp("2021-01-01 02:30") not in data_500
+    assert pd.Timestamp("2021-01-01 02:45") not in data_500
+
+
+def test_base_data_meets_qc(gap_data, qc_data):
+    """Test the base data meets QC function."""
+    assert len(
+        evaluator.base_data_meets_qc(
+            gap_data, pd.Series({pd.Timestamp("2021-01-01 00:00"): 600}), 600
+        )
+    ) == len(gap_data), "True filter removed data"
+    assert (
+        len(
+            evaluator.base_data_meets_qc(
+                gap_data, pd.Series({pd.Timestamp("2021-01-01 00:00"): 500}), 600
+            )
+        )
+        == 0
+    ), "False filter did not delete all data"
+    data_600 = evaluator.base_data_meets_qc(gap_data, qc_data, 600)
+    assert pd.Timestamp("2021-01-01 00:00") in data_600
+    assert pd.Timestamp("2021-01-01 00:15") not in data_600
+    assert pd.Timestamp("2021-01-01 00:30") not in data_600
+    assert pd.Timestamp("2021-01-01 00:45") in data_600
+    assert pd.Timestamp("2021-01-01 01:00") not in data_600
+    assert pd.Timestamp("2021-01-01 01:15") not in data_600
+    assert pd.Timestamp("2021-01-01 02:30") in data_600
+    assert pd.Timestamp("2021-01-01 02:45") in data_600
+
+    data_500 = evaluator.base_data_meets_qc(gap_data, qc_data, 500)
+    assert pd.Timestamp("2021-01-01 00:00") not in data_500
+    assert pd.Timestamp("2021-01-01 00:15") in data_500
+    assert pd.Timestamp("2021-01-01 00:30") in data_500
+    assert pd.Timestamp("2021-01-01 00:45") not in data_500
+    assert pd.Timestamp("2021-01-01 01:00") in data_500
+    assert pd.Timestamp("2021-01-01 01:15") in data_500
+    assert pd.Timestamp("2021-01-01 02:30") not in data_500
+    assert pd.Timestamp("2021-01-01 02:45") not in data_500
+
+
+def test_missing_data_quality_code(gap_data, qc_data):
+    """Test the missing data quality code function."""
+    no_gap_qc = evaluator.missing_data_quality_code(
+        gap_data.fillna(3), qc_data, gap_limit=0
+    )
+    assert no_gap_qc.equals(qc_data), "QC data modified when there are no gaps"
+
+    new_qc = evaluator.missing_data_quality_code(gap_data, qc_data, gap_limit=0)
+    assert new_qc[pd.Timestamp("2021-01-01 00:00")] == 100, "Starting gap not added"
+    assert new_qc[pd.Timestamp("2021-01-01 00:15")] == 500, "Starting gap not closed"
+    assert new_qc[pd.Timestamp("2021-01-01 02:30")] == 100, "Ending gap not added"
+    assert pd.Timestamp("2021-01-01 01:30") not in new_qc, "Mid-gap QC not replaced"
+    assert new_qc[pd.Timestamp("2021-01-01 02:00")] == 500, "Gap in middle not closed"
+
+
+def test_max_qc_limiter(qc_data):
+    """Test max_QC_limiter."""
+    limited_qcs = evaluator.max_qc_limiter(qc_data, 500)
+    assert (limited_qcs == 500).all(), "maximum not enforced"
+    assert len(limited_qcs) == len(qc_data), "data going missing or being added"
+    assert (limited_qcs.index == qc_data.index).all(), "index modified"
+
+    unlimited_power = evaluator.max_qc_limiter(qc_data, 600)
+    assert (unlimited_power == qc_data).all(), "maximum over enforced"
+    assert len(unlimited_power) == len(qc_data), "data going missing or being added"
+    assert (unlimited_power.index == qc_data.index).all(), "index modified"
+
+    whoops_maybe_the_power_had_a_limit = evaluator.max_qc_limiter(pd.Series({}), 600)
+    assert (whoops_maybe_the_power_had_a_limit == pd.Series({})).all(), "trivial case"
```

### Comparing `hydrobot-0.5.0/tests/test_processor.py` & `hydrobot-0.5.1/tests/test_processor.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,756 +1,756 @@
-# pyright: reportUnusedImport=false
-"""Test the processor module."""
-
-from xml.etree import ElementTree
-
-import numpy as np
-import pandas as pd
-import pytest
-from annalist.annalist import Annalist
-from defusedxml import ElementTree as DefusedElementTree
-from hilltoppy import Hilltop
-
-from hydrobot import data_sources, data_structure, processor, utils
-from hydrobot.data_sources import QualityCodeEvaluator
-from hydrobot.data_structure import parse_xml
-
-ann = Annalist()
-
-SITES = [
-    "Slimy Bog at Dirt Road",
-    "Mid Stream at Cowtoilet Farm",
-    "Mostly Cowpiss River at Greenwash Pastures",
-]
-
-MEASUREMENTS = [
-    "General Nastiness",
-    "Number of Actual Whole Human Turds Floating By",
-    "Dead Cow Concentration",
-]
-
-CHECK_MEASUREMENTS = [
-    "General Nastiness",
-    "Turdidity Sensor Reading [Number of Actual Whole Human Turds Floating By]",
-    "Dead Cow Concentration",
-]
-
-
-@pytest.fixture(autouse=True)
-def _no_requests(monkeypatch):
-    """Don't allow requests to make requests."""
-    monkeypatch.delattr("requests.sessions.Session.request")
-
-
-@pytest.fixture()
-def mock_site_list():
-    """Mock response from SiteList server call method."""
-    data = {
-        "SiteName": SITES,
-    }
-
-    return pd.DataFrame(data)
-
-
-@pytest.fixture()
-def mock_measurement_list():
-    """Mock response from MeasurementList server call method."""
-    data = {
-        "MeasurementName": MEASUREMENTS + CHECK_MEASUREMENTS,
-    }
-
-    return pd.DataFrame(data)
-
-
-@pytest.fixture()
-def mock_qc_evaluator_dict():
-    """Mock response from get_qc_evaluator_dict lookup method."""
-    qc_500_limits = [2.5, 5.4, 230]
-    qc_600_limits = [4, 0.9, 480]
-    config_data = {}
-    for i, meas in enumerate(MEASUREMENTS):
-        config_data[meas] = QualityCodeEvaluator(
-            qc_500_limits[i],
-            qc_600_limits[i],
-            meas,
-        )
-
-    return config_data
-
-
-@pytest.fixture()
-def mock_xml_data():
-    """Mock response from get_hilltop_xml server call method."""
-    with open("tests/xml_test_data_file.xml") as f:
-        xml_string = f.read()
-
-    return xml_string
-
-
-@pytest.fixture()
-def mock_get_data():
-    """
-    Fixture to mock the response from the get_data server call method.
-
-    Parameters
-    ----------
-    No direct parameters; indirectly passed into the inner function.
-
-    Notes
-    -----
-    This fixture simulates the response from the get_data server call method.
-    It reads XML test data from the specified file and provides a function that extracts
-    relevant data based on input parameters.
-
-    Example Usage
-    -------------
-    To use this fixture in a test, include it as a parameter in the test function.
-    For example:
-
-    ```python
-    def test_my_function(mock_get_data):
-        # Your test code here
-        result = my_function_that_uses_get_data(mock_get_data)
-        assert result == expected_result
-    ```
-    """
-    with open("tests/xml_test_data_file.xml") as f:
-        xml_string = f.read()
-
-    xml_root = ElementTree.Element(xml_string)
-
-    def _extract_data(
-        base_url,
-        hts,
-        site,
-        measurement,
-        from_date,
-        to_date,
-        tstype,
-    ):
-        _ = base_url, hts, site
-        data_blobs = parse_xml(xml_string)
-
-        keep_blobs = []
-
-        type_map = {
-            "Standard": "StdSeries",
-            "Quality": "StdQualSeries",
-            "Check": "CheckSeries",
-        }
-        if data_blobs is not None:
-            for blob in data_blobs:
-                if (
-                    blob.data_source.name == measurement
-                    and blob.data_source.ts_type == type_map[tstype]
-                ):
-                    conv_timestamps = utils.mowsecs_to_datetime_index(
-                        blob.data.timeseries.index
-                    )
-                    if from_date is None:
-                        from_date = conv_timestamps[0]
-                    if to_date is None:
-                        to_date = conv_timestamps[-1]
-                    mask = (conv_timestamps >= pd.to_datetime(from_date)) & (
-                        conv_timestamps <= pd.to_datetime(to_date)
-                    )
-                    blob.data.timeseries = blob.data.timeseries[mask]  # type: ignore
-                    keep_blobs += [blob]
-        else:
-            return None
-
-        return keep_blobs
-
-    return xml_root, _extract_data
-
-
-def test_processor_init(
-    capsys,
-    monkeypatch,
-    mock_site_list,
-    mock_measurement_list,
-    mock_xml_data,
-    mock_qc_evaluator_dict,
-):
-    """
-    Test the initialization of the Processor class.
-
-    Parameters
-    ----------
-    capsys : _pytest.capture.CaptureFixture
-        pytest fixture to capture stdout and stderr output.
-    monkeypatch : _pytest.monkeypatch.MonkeyPatch
-        pytest fixture to modify attributes or behavior during testing.
-    mock_site_list : Any
-        Mocked data for the site list.
-    mock_measurement_list : Any
-        Mocked data for the measurement list.
-    mock_xml_data : Any
-        Mocked data for Hilltop XML.
-    mock_qc_evaluator_dict : Any
-        Mocked data for the QC evaluator dictionary.
-
-    Notes
-    -----
-    This test function initializes a Processor instance and checks if the attributes
-    and initializations are as expected. It also validates the log outputs using
-    the captured output from capsys.
-
-    It patches several functions using monkeypatch to provide the necessary mock data.
-    The patched functions include Hilltop class methods for site and measurement lists,
-    as well as the get_hilltop_xml function from data_acquisition.
-
-    Assertions
-    ----------
-    - Log outputs are validated to ensure proper initialization and function calls.
-    - Attributes of the Processor instance, such as standard_series, are checked.
-    - The data in the standard_series is verified for correctness.
-
-    """
-
-    def get_mock_site_list(*args, **kwargs):
-        _ = args, kwargs
-        return mock_site_list
-
-    def get_mock_measurement_list(*args, **kwargs):
-        _ = args, kwargs
-        return mock_measurement_list
-
-    def get_mock_xml_data(*args, **kwargs):
-        _ = args, kwargs
-        return mock_xml_data
-
-    def get_mock_qc_evaluator_dict(*args, **kwargs):
-        _ = args, kwargs
-        return mock_qc_evaluator_dict
-
-    ann.configure(stream_format_str="%(function_name)s | %(site)s")
-
-    # Here we patch the Hilltop Class
-    monkeypatch.setattr(Hilltop, "get_site_list", get_mock_site_list)
-    monkeypatch.setattr(Hilltop, "get_measurement_list", get_mock_measurement_list)
-    monkeypatch.setattr(
-        data_sources,
-        "get_qc_evaluator_dict",
-        get_mock_qc_evaluator_dict,
-    )
-
-    # However, in these cases, we need to patch the INSTANCE as imported in
-    # data_acquisition. Not sure if this makes sense to me, but it works.
-    monkeypatch.setattr("hydrobot.data_acquisition.get_hilltop_xml", get_mock_xml_data)
-
-    pr = processor.Processor(
-        base_url="https://greenwashed.and.pleasant/",
-        site=SITES[1],
-        standard_hts="GreenPasturesAreNaturalAndEcoFriendlyISwear.hts",
-        standard_measurement_name=MEASUREMENTS[1],
-        check_measurement_name=CHECK_MEASUREMENTS[1],
-        frequency="5min",
-    )
-
-    captured = capsys.readouterr()
-    ann_output = captured.err.split("\n")
-
-    correct = [
-        "standard_series | Mid Stream at Cowtoilet Farm",
-        "import_standard | Mid Stream at Cowtoilet Farm",
-        "quality_series | Mid Stream at Cowtoilet Farm",
-        "import_quality | Mid Stream at Cowtoilet Farm",
-        "check_series | Mid Stream at Cowtoilet Farm",
-        "import_check | Mid Stream at Cowtoilet Farm",
-        "__init__ | Mid Stream at Cowtoilet Farm",
-    ]
-
-    for i, out in enumerate(ann_output[0:-1]):
-        assert out == correct[i], f"Failed on log number {i} with output {out}"
-
-    assert isinstance(pr.standard_series, pd.Series)
-    assert pr.raw_standard_blob is not None
-    assert pr.standard_measurement_name == pr.raw_standard_blob.data_source.name
-    assert float(pr.standard_series.loc["2023-01-01 00:10:00"]) == pytest.approx(1882.1)
-    assert pr.standard_series.index.dtype == np.dtype("datetime64[ns]")
-
-
-def test_to_xml_data_structure(
-    monkeypatch,
-    mock_site_list,
-    mock_measurement_list,
-    mock_xml_data,
-    mock_qc_evaluator_dict,
-    tmp_path,
-    sample_data_source_xml_file,
-):
-    """
-    Test the conversion of Processor data to XML data structure.
-
-    Parameters
-    ----------
-    monkeypatch : pytest.MonkeyPatch
-        Pytest fixture for monkeypatching.
-    mock_site_list : List[str]
-        Mocked list of site names.
-    mock_measurement_list : List[str]
-        Mocked list of measurement names.
-    mock_xml_data : str
-        Mocked XML data content.
-    mock_qc_evaluator_dict : Dict[str, Any]
-        Mocked QC evaluator dictionary.
-    sample_data_source_xml_file : str
-        Path to the sample XML data file.
-
-    Notes
-    -----
-    This test function checks the conversion of Processor data to the XML data structure.
-    It mocks relevant functions and classes for the test.
-
-    Assertions
-    ----------
-    - The canonicalized content of the generated XML file matches the sample XML content.
-    - Each data source blob in the list has a site name matching the specified site.
-
-    """
-
-    def get_mock_site_list(*args, **kwargs):
-        _ = args, kwargs
-        return mock_site_list
-
-    def get_mock_measurement_list(*args, **kwargs):
-        _ = args, kwargs
-        return mock_measurement_list
-
-    def get_mock_xml_data(*args, **kwargs):
-        _ = args, kwargs
-        return mock_xml_data
-
-    def get_mock_qc_evaluator_dict(*args, **kwargs):
-        _ = args, kwargs
-        return mock_qc_evaluator_dict
-
-    ann.configure(stream_format_str="%(function_name)s | %(site)s")
-
-    # Here we patch the Hilltop Class
-    monkeypatch.setattr(Hilltop, "get_site_list", get_mock_site_list)
-    monkeypatch.setattr(Hilltop, "get_measurement_list", get_mock_measurement_list)
-    monkeypatch.setattr(
-        data_sources,
-        "get_qc_evaluator_dict",
-        get_mock_qc_evaluator_dict,
-    )
-
-    # However, in this case, we need to patch the INSTANCE as imported in
-    # data_acquisition. Not sure if this makes sense to me, but it works.
-    monkeypatch.setattr("hydrobot.data_acquisition.get_hilltop_xml", get_mock_xml_data)
-
-    data_source_blob_list = []
-
-    for check, meas in zip(CHECK_MEASUREMENTS, MEASUREMENTS, strict=True):
-        pr = processor.Processor(
-            base_url="https://greenwashed.and.pleasant/",
-            site=SITES[1],
-            standard_hts="GreenPasturesAreNaturalAndEcoFriendlyISwear.hts",
-            standard_measurement_name=meas,
-            check_measurement_name=check,
-            frequency="5min",
-        )
-
-        data_source_blob_list += pr.to_xml_data_structure()
-
-    output_path = tmp_path / "output.xml"
-    data_structure.write_hilltop_xml(data_source_blob_list, output_path)
-
-    with open(output_path) as f:
-        output_xml = f.read()
-
-    with open(sample_data_source_xml_file) as f:
-        sample_data_source_xml = f.read()
-
-    input_tree = DefusedElementTree.fromstring(sample_data_source_xml)
-    output_tree = DefusedElementTree.fromstring(output_xml)
-
-    assert ElementTree.indent(input_tree) == ElementTree.indent(output_tree)
-
-    for blob in data_source_blob_list:
-        assert blob.site_name == SITES[1]
-
-
-def test_import_data(
-    monkeypatch,
-    mock_site_list,
-    mock_measurement_list,
-    mock_get_data,
-    mock_qc_evaluator_dict,
-):
-    """
-    Test the import_data method of the Processor class.
-
-    Parameters
-    ----------
-    monkeypatch : pytest.MonkeyPatch
-        Pytest fixture for monkeypatching.
-    mock_site_list : List[str]
-        Mocked list of site names.
-    mock_measurement_list : List[str]
-        Mocked list of measurement names.
-    mock_get_data : Callable
-        Mocked get_data function.
-    mock_qc_evaluator_dict : Dict[str, Any]
-        Mocked QC evaluator dictionary.
-
-    Notes
-    -----
-    This test function checks the import_data method of the Processor class.
-    It mocks relevant functions and classes for the test.
-
-    Assertions
-    ----------
-    - For each index in standard_series, quality_series, and check_series, it is within
-        the specified date range.
-    - The import_data method updates the series with new data and retains existing
-        changes without overwriting.
-    - The import_data method overwrites existing data when the 'overwrite' parameter
-        is set to True.
-
-    """
-
-    def get_mock_site_list(*args, **kwargs):
-        _ = args, kwargs
-        return mock_site_list
-
-    def get_mock_measurement_list(*args, **kwargs):
-        _ = args, kwargs
-        return mock_measurement_list
-
-    def get_mock_get_data(*args, **kwargs):
-        xml, data_func = mock_get_data
-        return xml, data_func(*args, **kwargs)
-
-    def get_mock_qc_evaluator_dict(*args, **kwargs):
-        _ = args, kwargs
-        return mock_qc_evaluator_dict
-
-    ann.configure(stream_format_str="%(function_name)s | %(site)s")
-
-    # Here we patch the Hilltop Class
-    monkeypatch.setattr(Hilltop, "get_site_list", get_mock_site_list)
-    monkeypatch.setattr(Hilltop, "get_measurement_list", get_mock_measurement_list)
-    monkeypatch.setattr(
-        data_sources,
-        "get_qc_evaluator_dict",
-        get_mock_qc_evaluator_dict,
-    )
-
-    # However, in this case, we need to patch the INSTANCE as imported in
-    # data_acquisition. Not sure if this makes sense to me, but it works.
-    monkeypatch.setattr("hydrobot.data_acquisition.get_data", get_mock_get_data)
-
-    from_date = "2023-01-01"
-    to_date = "2023/01/01 00:20"
-
-    pr = processor.Processor(
-        base_url="https://greenwashed.and.pleasant/",
-        site=SITES[1],
-        standard_hts="GreenPasturesAreNaturalAndEcoFriendlyISwear.hts",
-        standard_measurement_name=MEASUREMENTS[0],
-        frequency="5min",
-        from_date=from_date,
-        to_date=to_date,
-    )
-
-    for idx in pr.standard_series.index:
-        assert idx >= pd.to_datetime(from_date)
-        assert idx <= pd.to_datetime(to_date)
-
-    for idx in pr.quality_series.index:
-        assert idx >= pd.to_datetime(from_date)
-        assert idx <= pd.to_datetime(to_date)
-
-    for idx in pr.check_series.index:
-        assert idx >= pd.to_datetime(from_date)
-        assert idx <= pd.to_datetime(to_date)
-
-
-def test_gap_closer(
-    monkeypatch,
-    mock_site_list,
-    mock_measurement_list,
-    mock_get_data,
-    mock_qc_evaluator_dict,
-):
-    """
-    Test the 'gap_closer' method of the Processor class.
-
-    Parameters
-    ----------
-    monkeypatch : pytest.MonkeyPatch
-        Pytest fixture to modify or mock modules during testing.
-    mock_site_list : pytest fixture
-        Mocked response for the site list.
-    mock_measurement_list : pytest fixture
-        Mocked response for the measurement list.
-    mock_get_data : pytest fixture
-        Mock response for the get_data server call method.
-    mock_qc_evaluator_dict : pytest fixture
-        Mocked response for the quality control evaluator dictionary.
-
-    Notes
-    -----
-    - This test checks the functionality of the 'gap_closer' method in the Processor
-        class.
-    - It involves creating a Processor object, making a gap in the data, inserting NaNs,
-        and then closing the gap.
-    - Assertions are made to ensure that the gap is properly created, NaNs are inserted,
-        and the gap is closed.
-
-    Assertions
-    ----------
-    - The data points that are intended to be deleted actually exist before the gap
-        creation.
-    - After creating a small gap, check that the gap was made by confirming the absence
-        of the specified data points.
-    - Check that NaNs are correctly inserted into the specified positions in the data.
-    - After closing the gaps, verify that the specified data points are no longer
-        present in the data.
-
-    """
-
-    def get_mock_site_list(*args, **kwargs):
-        _ = args, kwargs
-        return mock_site_list
-
-    def get_mock_measurement_list(*args, **kwargs):
-        _ = args, kwargs
-        return mock_measurement_list
-
-    def get_mock_get_data(*args, **kwargs):
-        xml, data_func = mock_get_data
-        return xml, data_func(*args, **kwargs)
-
-    def get_mock_qc_evaluator_dict(*args, **kwargs):
-        _ = args, kwargs
-        return mock_qc_evaluator_dict
-
-    ann.configure(stream_format_str="%(function_name)s | %(site)s")
-
-    # Here we patch the Hilltop Class
-    monkeypatch.setattr(Hilltop, "get_site_list", get_mock_site_list)
-    monkeypatch.setattr(Hilltop, "get_measurement_list", get_mock_measurement_list)
-    monkeypatch.setattr(
-        data_sources,
-        "get_qc_evaluator_dict",
-        get_mock_qc_evaluator_dict,
-    )
-
-    # However, in this case, we need to patch the INSTANCE as imported in
-    # data_acquisition. Not sure if this makes sense to me, but it works.
-    monkeypatch.setattr("hydrobot.data_acquisition.get_data", get_mock_get_data)
-
-    pr = processor.Processor(
-        base_url="https://greenwashed.and.pleasant/",
-        site=SITES[1],
-        standard_hts="GreenPasturesAreNaturalAndEcoFriendlyISwear.hts",
-        standard_measurement_name=MEASUREMENTS[0],
-        frequency="5min",
-    )
-
-    # Checking that the data points I want to delete actually exist:
-    start_idx = "2023-01-01 00:20:00"
-    end_idx = "2023-01-01 00:25:00"
-    assert pd.to_datetime(start_idx) in pr.standard_series
-    assert pd.to_datetime(end_idx) in pr.standard_series
-
-    # Make a small gap
-    pr.delete_range(start_idx, end_idx)
-
-    # Check that gap was made
-    assert (
-        pd.to_datetime(start_idx) not in pr.standard_series
-    ), "processor.delete_range appears to be broken."
-    assert (
-        pd.to_datetime(end_idx) not in pr.standard_series
-    ), "processor.delete_range appears to be broken."
-
-    # Insert nans where values are missing
-    pr.insert_missing_nans()
-
-    # Check that NaNs are inserted
-    assert pd.isna(
-        pr.standard_series[start_idx]
-    ), "processor.insert_missing_nans appears to be broken."
-    assert pd.isna(
-        pr.standard_series[end_idx]
-    ), "processor.insert_missing_nans appears to be broken."
-
-    # "Close" gaps (i.e. remove nan rows)
-    pr.gap_closer()
-
-    # Check that gap was closed
-    assert (
-        pd.to_datetime(start_idx) not in pr.standard_series
-    ), "processor.gap_closer appears to be broken."
-    assert (
-        pd.to_datetime(end_idx) not in pr.standard_series
-    ), "processor.gap_closer appears to be broken."
-
-
-def test_data_export(
-    monkeypatch,
-    mock_site_list,
-    mock_measurement_list,
-    mock_get_data,
-    mock_qc_evaluator_dict,
-    tmp_path,
-):
-    """
-    Test the 'gap_closer' method of the Processor class.
-
-    Parameters
-    ----------
-    monkeypatch : pytest.MonkeyPatch
-        Pytest fixture to modify or mock modules during testing.
-    mock_site_list : pytest fixture
-        Mocked response for the site list.
-    mock_measurement_list : pytest fixture
-        Mocked response for the measurement list.
-    mock_get_data : pytest fixture
-        Mock response for the get_data server call method.
-    mock_qc_evaluator_dict : pytest fixture
-        Mocked response for the quality control evaluator dictionary.
-
-    Notes
-    -----
-    - This test checks the functionality of the 'gap_closer' method in the Processor
-        class.
-    - It involves creating a Processor object, making a gap in the data, inserting NaNs,
-        and then closing the gap.
-    - Assertions are made to ensure that the gap is properly created, NaNs are inserted,
-        and the gap is closed.
-
-    Assertions
-    ----------
-    - The data points that are intended to be deleted actually exist before the gap
-        creation.
-    - After creating a small gap, check that the gap was made by confirming the absence
-        of the specified data points.
-    - Check that NaNs are correctly inserted into the specified positions in the data.
-    - After closing the gaps, verify that the specified data points are no longer
-        present in the data.
-
-    """
-
-    def get_mock_site_list(*args, **kwargs):
-        _ = args, kwargs
-        return mock_site_list
-
-    def get_mock_measurement_list(*args, **kwargs):
-        _ = args, kwargs
-        return mock_measurement_list
-
-    def get_mock_get_data(*args, **kwargs):
-        xml, data_func = mock_get_data
-        return xml, data_func(*args, **kwargs)
-
-    def get_mock_qc_evaluator_dict(*args, **kwargs):
-        _ = args, kwargs
-        return mock_qc_evaluator_dict
-
-    ann.configure(stream_format_str="%(function_name)s | %(site)s")
-
-    # Here we patch the Hilltop Class
-    monkeypatch.setattr(Hilltop, "get_site_list", get_mock_site_list)
-    monkeypatch.setattr(Hilltop, "get_measurement_list", get_mock_measurement_list)
-    monkeypatch.setattr(
-        data_sources,
-        "get_qc_evaluator_dict",
-        get_mock_qc_evaluator_dict,
-    )
-
-    # However, in this case, we need to patch the INSTANCE as imported in
-    # data_acquisition. Not sure if this makes sense to me, but it works.
-    monkeypatch.setattr("hydrobot.data_acquisition.get_data", get_mock_get_data)
-
-    pr = processor.Processor(
-        base_url="https://greenwashed.and.pleasant/",
-        site=SITES[1],
-        standard_hts="GreenPasturesAreNaturalAndEcoFriendlyISwear.hts",
-        standard_measurement_name=MEASUREMENTS[0],
-        frequency="5min",
-    )
-
-    # Checking that the data points I want to delete actually exist:
-    start_idx = "2023-01-01 00:20:00"
-    end_idx = "2023-01-01 00:25:00"
-    assert pd.to_datetime(start_idx) in pr.standard_series
-    assert pd.to_datetime(end_idx) in pr.standard_series
-
-    # =======================Make a small gap========================
-    print("Gappy Chappy")
-    pr.delete_range(start_idx, end_idx)
-
-    gap_path_csv = tmp_path / "gap_output.csv"
-    gap_path_hilltop_csv = tmp_path / "gap_output_hilltop"
-    gap_path_xml = tmp_path / "gap_output.xml"
-
-    pr.data_exporter(gap_path_csv, ftype="csv")
-
-    read_csv_df = pd.read_csv(gap_path_csv)
-    # Check that the csv was filled in with nans where there are no quality values
-    assert pd.isna(read_csv_df["General Nastiness [Quality]"].iloc[1])
-
-    # The hilltop_csv format outputs two files:
-    # one for standard and qc together,
-    # and one for check data alone.
-    pr.data_exporter(gap_path_hilltop_csv, ftype="hilltop_csv")
-    hilltop_path_std_qc = tmp_path / "gap_output_hilltop_std_qc.csv"
-    hilltop_path_check = tmp_path / "gap_output_hilltop_check.csv"
-
-    read_hilltop_std_qc_csv_df = pd.read_csv(hilltop_path_std_qc)
-    read_hilltop_check_csv_df = pd.read_csv(hilltop_path_check)
-
-    # Check that the deleted values have not been filled somehow
-    assert start_idx not in list(read_hilltop_std_qc_csv_df.index)
-    assert start_idx not in list(read_hilltop_check_csv_df.index)
-
-    print("Before xml export:", pr.quality_series.index)
-    pr.data_exporter(gap_path_xml, ftype="xml")
-    print("After xml export:", pr.quality_series.index)
-    gap_path_xml_tree = DefusedElementTree.fromstring(gap_path_xml.read_text())
-    gap_path_blob = data_structure.parse_xml(gap_path_xml_tree)
-
-    std_indices = gap_path_blob[0].data.timeseries.index
-    assert pd.Timestamp(start_idx) not in list(std_indices)
-
-    # =======================Insert Nans========================
-    # This is how we internally represent gaps. They need to be converted to the Gap
-    # tag for xml export.
-    print("Before nans:", pr.quality_series.index)
-    pr.insert_missing_nans()
-    print("After nans:", pr.quality_series.index)
-
-    pr.data_exporter(gap_path_csv, ftype="csv")
-
-    read_csv_df = pd.read_csv(gap_path_csv)
-    # Check that the csv was filled in with nans where there are no quality values
-    # assert pd.isna(read_csv_df["General Nastiness [Quality]"].iloc[1])
-
-    # The hilltop_csv format outputs two files:
-    # one for standard and qc together,
-    # and one for check data alone.
-    pr.data_exporter(gap_path_hilltop_csv, ftype="hilltop_csv")
-
-    read_hilltop_std_qc_csv_df = pd.read_csv(hilltop_path_std_qc)
-    read_hilltop_check_csv_df = pd.read_csv(hilltop_path_check)
-
-    # Check that the deleted values have not been filled somehow
-    # assert start_idx not in list(read_hilltop_std_qc_csv_df.index)
-    # assert start_idx not in list(read_hilltop_check_csv_df.index)
-    print(read_hilltop_std_qc_csv_df)
-    print(read_hilltop_check_csv_df)
-    # assert start_idx not in list(read_hilltop_std_qc_csv_df.index)
-
-    pr.data_exporter(gap_path_xml, ftype="xml")
-
-    print(gap_path_xml.read_text())
-    gap_path_xml_tree = DefusedElementTree.fromstring(gap_path_xml.read_text())
-    gap_path_blob = data_structure.parse_xml(gap_path_xml_tree)
-
-    std_indices = gap_path_blob[0].data.timeseries.index
-    assert start_idx not in list(std_indices)
+# pyright: reportUnusedImport=false
+"""Test the processor module."""
+
+from xml.etree import ElementTree
+
+import numpy as np
+import pandas as pd
+import pytest
+from annalist.annalist import Annalist
+from defusedxml import ElementTree as DefusedElementTree
+from hilltoppy import Hilltop
+
+from hydrobot import data_sources, data_structure, processor, utils
+from hydrobot.data_sources import QualityCodeEvaluator
+from hydrobot.data_structure import parse_xml
+
+ann = Annalist()
+
+SITES = [
+    "Slimy Bog at Dirt Road",
+    "Mid Stream at Cowtoilet Farm",
+    "Mostly Cowpiss River at Greenwash Pastures",
+]
+
+MEASUREMENTS = [
+    "General Nastiness",
+    "Number of Actual Whole Human Turds Floating By",
+    "Dead Cow Concentration",
+]
+
+CHECK_MEASUREMENTS = [
+    "General Nastiness",
+    "Turdidity Sensor Reading [Number of Actual Whole Human Turds Floating By]",
+    "Dead Cow Concentration",
+]
+
+
+@pytest.fixture(autouse=True)
+def _no_requests(monkeypatch):
+    """Don't allow requests to make requests."""
+    monkeypatch.delattr("requests.sessions.Session.request")
+
+
+@pytest.fixture()
+def mock_site_list():
+    """Mock response from SiteList server call method."""
+    data = {
+        "SiteName": SITES,
+    }
+
+    return pd.DataFrame(data)
+
+
+@pytest.fixture()
+def mock_measurement_list():
+    """Mock response from MeasurementList server call method."""
+    data = {
+        "MeasurementName": MEASUREMENTS + CHECK_MEASUREMENTS,
+    }
+
+    return pd.DataFrame(data)
+
+
+@pytest.fixture()
+def mock_qc_evaluator_dict():
+    """Mock response from get_qc_evaluator_dict lookup method."""
+    qc_500_limits = [2.5, 5.4, 230]
+    qc_600_limits = [4, 0.9, 480]
+    config_data = {}
+    for i, meas in enumerate(MEASUREMENTS):
+        config_data[meas] = QualityCodeEvaluator(
+            qc_500_limits[i],
+            qc_600_limits[i],
+            meas,
+        )
+
+    return config_data
+
+
+@pytest.fixture()
+def mock_xml_data():
+    """Mock response from get_hilltop_xml server call method."""
+    with open("tests/xml_test_data_file.xml") as f:
+        xml_string = f.read()
+
+    return xml_string
+
+
+@pytest.fixture()
+def mock_get_data():
+    """
+    Fixture to mock the response from the get_data server call method.
+
+    Parameters
+    ----------
+    No direct parameters; indirectly passed into the inner function.
+
+    Notes
+    -----
+    This fixture simulates the response from the get_data server call method.
+    It reads XML test data from the specified file and provides a function that extracts
+    relevant data based on input parameters.
+
+    Example Usage
+    -------------
+    To use this fixture in a test, include it as a parameter in the test function.
+    For example:
+
+    ```python
+    def test_my_function(mock_get_data):
+        # Your test code here
+        result = my_function_that_uses_get_data(mock_get_data)
+        assert result == expected_result
+    ```
+    """
+    with open("tests/xml_test_data_file.xml") as f:
+        xml_string = f.read()
+
+    xml_root = ElementTree.Element(xml_string)
+
+    def _extract_data(
+        base_url,
+        hts,
+        site,
+        measurement,
+        from_date,
+        to_date,
+        tstype,
+    ):
+        _ = base_url, hts, site
+        data_blobs = parse_xml(xml_string)
+
+        keep_blobs = []
+
+        type_map = {
+            "Standard": "StdSeries",
+            "Quality": "StdQualSeries",
+            "Check": "CheckSeries",
+        }
+        if data_blobs is not None:
+            for blob in data_blobs:
+                if (
+                    blob.data_source.name == measurement
+                    and blob.data_source.ts_type == type_map[tstype]
+                ):
+                    conv_timestamps = utils.mowsecs_to_datetime_index(
+                        blob.data.timeseries.index
+                    )
+                    if from_date is None:
+                        from_date = conv_timestamps[0]
+                    if to_date is None:
+                        to_date = conv_timestamps[-1]
+                    mask = (conv_timestamps >= pd.to_datetime(from_date)) & (
+                        conv_timestamps <= pd.to_datetime(to_date)
+                    )
+                    blob.data.timeseries = blob.data.timeseries[mask]  # type: ignore
+                    keep_blobs += [blob]
+        else:
+            return None
+
+        return keep_blobs
+
+    return xml_root, _extract_data
+
+
+def test_processor_init(
+    capsys,
+    monkeypatch,
+    mock_site_list,
+    mock_measurement_list,
+    mock_xml_data,
+    mock_qc_evaluator_dict,
+):
+    """
+    Test the initialization of the Processor class.
+
+    Parameters
+    ----------
+    capsys : _pytest.capture.CaptureFixture
+        pytest fixture to capture stdout and stderr output.
+    monkeypatch : _pytest.monkeypatch.MonkeyPatch
+        pytest fixture to modify attributes or behavior during testing.
+    mock_site_list : Any
+        Mocked data for the site list.
+    mock_measurement_list : Any
+        Mocked data for the measurement list.
+    mock_xml_data : Any
+        Mocked data for Hilltop XML.
+    mock_qc_evaluator_dict : Any
+        Mocked data for the QC evaluator dictionary.
+
+    Notes
+    -----
+    This test function initializes a Processor instance and checks if the attributes
+    and initializations are as expected. It also validates the log outputs using
+    the captured output from capsys.
+
+    It patches several functions using monkeypatch to provide the necessary mock data.
+    The patched functions include Hilltop class methods for site and measurement lists,
+    as well as the get_hilltop_xml function from data_acquisition.
+
+    Assertions
+    ----------
+    - Log outputs are validated to ensure proper initialization and function calls.
+    - Attributes of the Processor instance, such as standard_series, are checked.
+    - The data in the standard_series is verified for correctness.
+
+    """
+
+    def get_mock_site_list(*args, **kwargs):
+        _ = args, kwargs
+        return mock_site_list
+
+    def get_mock_measurement_list(*args, **kwargs):
+        _ = args, kwargs
+        return mock_measurement_list
+
+    def get_mock_xml_data(*args, **kwargs):
+        _ = args, kwargs
+        return mock_xml_data
+
+    def get_mock_qc_evaluator_dict(*args, **kwargs):
+        _ = args, kwargs
+        return mock_qc_evaluator_dict
+
+    ann.configure(stream_format_str="%(function_name)s | %(site)s")
+
+    # Here we patch the Hilltop Class
+    monkeypatch.setattr(Hilltop, "get_site_list", get_mock_site_list)
+    monkeypatch.setattr(Hilltop, "get_measurement_list", get_mock_measurement_list)
+    monkeypatch.setattr(
+        data_sources,
+        "get_qc_evaluator_dict",
+        get_mock_qc_evaluator_dict,
+    )
+
+    # However, in these cases, we need to patch the INSTANCE as imported in
+    # data_acquisition. Not sure if this makes sense to me, but it works.
+    monkeypatch.setattr("hydrobot.data_acquisition.get_hilltop_xml", get_mock_xml_data)
+
+    pr = processor.Processor(
+        base_url="https://greenwashed.and.pleasant/",
+        site=SITES[1],
+        standard_hts="GreenPasturesAreNaturalAndEcoFriendlyISwear.hts",
+        standard_measurement_name=MEASUREMENTS[1],
+        check_measurement_name=CHECK_MEASUREMENTS[1],
+        frequency="5min",
+    )
+
+    captured = capsys.readouterr()
+    ann_output = captured.err.split("\n")
+
+    correct = [
+        "standard_series | Mid Stream at Cowtoilet Farm",
+        "import_standard | Mid Stream at Cowtoilet Farm",
+        "quality_series | Mid Stream at Cowtoilet Farm",
+        "import_quality | Mid Stream at Cowtoilet Farm",
+        "check_series | Mid Stream at Cowtoilet Farm",
+        "import_check | Mid Stream at Cowtoilet Farm",
+        "__init__ | Mid Stream at Cowtoilet Farm",
+    ]
+
+    for i, out in enumerate(ann_output[0:-1]):
+        assert out == correct[i], f"Failed on log number {i} with output {out}"
+
+    assert isinstance(pr.standard_series, pd.Series)
+    assert pr.raw_standard_blob is not None
+    assert pr.standard_measurement_name == pr.raw_standard_blob.data_source.name
+    assert float(pr.standard_series.loc["2023-01-01 00:10:00"]) == pytest.approx(1882.1)
+    assert pr.standard_series.index.dtype == np.dtype("datetime64[ns]")
+
+
+def test_to_xml_data_structure(
+    monkeypatch,
+    mock_site_list,
+    mock_measurement_list,
+    mock_xml_data,
+    mock_qc_evaluator_dict,
+    tmp_path,
+    sample_data_source_xml_file,
+):
+    """
+    Test the conversion of Processor data to XML data structure.
+
+    Parameters
+    ----------
+    monkeypatch : pytest.MonkeyPatch
+        Pytest fixture for monkeypatching.
+    mock_site_list : List[str]
+        Mocked list of site names.
+    mock_measurement_list : List[str]
+        Mocked list of measurement names.
+    mock_xml_data : str
+        Mocked XML data content.
+    mock_qc_evaluator_dict : Dict[str, Any]
+        Mocked QC evaluator dictionary.
+    sample_data_source_xml_file : str
+        Path to the sample XML data file.
+
+    Notes
+    -----
+    This test function checks the conversion of Processor data to the XML data structure.
+    It mocks relevant functions and classes for the test.
+
+    Assertions
+    ----------
+    - The canonicalized content of the generated XML file matches the sample XML content.
+    - Each data source blob in the list has a site name matching the specified site.
+
+    """
+
+    def get_mock_site_list(*args, **kwargs):
+        _ = args, kwargs
+        return mock_site_list
+
+    def get_mock_measurement_list(*args, **kwargs):
+        _ = args, kwargs
+        return mock_measurement_list
+
+    def get_mock_xml_data(*args, **kwargs):
+        _ = args, kwargs
+        return mock_xml_data
+
+    def get_mock_qc_evaluator_dict(*args, **kwargs):
+        _ = args, kwargs
+        return mock_qc_evaluator_dict
+
+    ann.configure(stream_format_str="%(function_name)s | %(site)s")
+
+    # Here we patch the Hilltop Class
+    monkeypatch.setattr(Hilltop, "get_site_list", get_mock_site_list)
+    monkeypatch.setattr(Hilltop, "get_measurement_list", get_mock_measurement_list)
+    monkeypatch.setattr(
+        data_sources,
+        "get_qc_evaluator_dict",
+        get_mock_qc_evaluator_dict,
+    )
+
+    # However, in this case, we need to patch the INSTANCE as imported in
+    # data_acquisition. Not sure if this makes sense to me, but it works.
+    monkeypatch.setattr("hydrobot.data_acquisition.get_hilltop_xml", get_mock_xml_data)
+
+    data_source_blob_list = []
+
+    for check, meas in zip(CHECK_MEASUREMENTS, MEASUREMENTS, strict=True):
+        pr = processor.Processor(
+            base_url="https://greenwashed.and.pleasant/",
+            site=SITES[1],
+            standard_hts="GreenPasturesAreNaturalAndEcoFriendlyISwear.hts",
+            standard_measurement_name=meas,
+            check_measurement_name=check,
+            frequency="5min",
+        )
+
+        data_source_blob_list += pr.to_xml_data_structure()
+
+    output_path = tmp_path / "output.xml"
+    data_structure.write_hilltop_xml(data_source_blob_list, output_path)
+
+    with open(output_path) as f:
+        output_xml = f.read()
+
+    with open(sample_data_source_xml_file) as f:
+        sample_data_source_xml = f.read()
+
+    input_tree = DefusedElementTree.fromstring(sample_data_source_xml)
+    output_tree = DefusedElementTree.fromstring(output_xml)
+
+    assert ElementTree.indent(input_tree) == ElementTree.indent(output_tree)
+
+    for blob in data_source_blob_list:
+        assert blob.site_name == SITES[1]
+
+
+def test_import_data(
+    monkeypatch,
+    mock_site_list,
+    mock_measurement_list,
+    mock_get_data,
+    mock_qc_evaluator_dict,
+):
+    """
+    Test the import_data method of the Processor class.
+
+    Parameters
+    ----------
+    monkeypatch : pytest.MonkeyPatch
+        Pytest fixture for monkeypatching.
+    mock_site_list : List[str]
+        Mocked list of site names.
+    mock_measurement_list : List[str]
+        Mocked list of measurement names.
+    mock_get_data : Callable
+        Mocked get_data function.
+    mock_qc_evaluator_dict : Dict[str, Any]
+        Mocked QC evaluator dictionary.
+
+    Notes
+    -----
+    This test function checks the import_data method of the Processor class.
+    It mocks relevant functions and classes for the test.
+
+    Assertions
+    ----------
+    - For each index in standard_series, quality_series, and check_series, it is within
+        the specified date range.
+    - The import_data method updates the series with new data and retains existing
+        changes without overwriting.
+    - The import_data method overwrites existing data when the 'overwrite' parameter
+        is set to True.
+
+    """
+
+    def get_mock_site_list(*args, **kwargs):
+        _ = args, kwargs
+        return mock_site_list
+
+    def get_mock_measurement_list(*args, **kwargs):
+        _ = args, kwargs
+        return mock_measurement_list
+
+    def get_mock_get_data(*args, **kwargs):
+        xml, data_func = mock_get_data
+        return xml, data_func(*args, **kwargs)
+
+    def get_mock_qc_evaluator_dict(*args, **kwargs):
+        _ = args, kwargs
+        return mock_qc_evaluator_dict
+
+    ann.configure(stream_format_str="%(function_name)s | %(site)s")
+
+    # Here we patch the Hilltop Class
+    monkeypatch.setattr(Hilltop, "get_site_list", get_mock_site_list)
+    monkeypatch.setattr(Hilltop, "get_measurement_list", get_mock_measurement_list)
+    monkeypatch.setattr(
+        data_sources,
+        "get_qc_evaluator_dict",
+        get_mock_qc_evaluator_dict,
+    )
+
+    # However, in this case, we need to patch the INSTANCE as imported in
+    # data_acquisition. Not sure if this makes sense to me, but it works.
+    monkeypatch.setattr("hydrobot.data_acquisition.get_data", get_mock_get_data)
+
+    from_date = "2023-01-01"
+    to_date = "2023/01/01 00:20"
+
+    pr = processor.Processor(
+        base_url="https://greenwashed.and.pleasant/",
+        site=SITES[1],
+        standard_hts="GreenPasturesAreNaturalAndEcoFriendlyISwear.hts",
+        standard_measurement_name=MEASUREMENTS[0],
+        frequency="5min",
+        from_date=from_date,
+        to_date=to_date,
+    )
+
+    for idx in pr.standard_series.index:
+        assert idx >= pd.to_datetime(from_date)
+        assert idx <= pd.to_datetime(to_date)
+
+    for idx in pr.quality_series.index:
+        assert idx >= pd.to_datetime(from_date)
+        assert idx <= pd.to_datetime(to_date)
+
+    for idx in pr.check_series.index:
+        assert idx >= pd.to_datetime(from_date)
+        assert idx <= pd.to_datetime(to_date)
+
+
+def test_gap_closer(
+    monkeypatch,
+    mock_site_list,
+    mock_measurement_list,
+    mock_get_data,
+    mock_qc_evaluator_dict,
+):
+    """
+    Test the 'gap_closer' method of the Processor class.
+
+    Parameters
+    ----------
+    monkeypatch : pytest.MonkeyPatch
+        Pytest fixture to modify or mock modules during testing.
+    mock_site_list : pytest fixture
+        Mocked response for the site list.
+    mock_measurement_list : pytest fixture
+        Mocked response for the measurement list.
+    mock_get_data : pytest fixture
+        Mock response for the get_data server call method.
+    mock_qc_evaluator_dict : pytest fixture
+        Mocked response for the quality control evaluator dictionary.
+
+    Notes
+    -----
+    - This test checks the functionality of the 'gap_closer' method in the Processor
+        class.
+    - It involves creating a Processor object, making a gap in the data, inserting NaNs,
+        and then closing the gap.
+    - Assertions are made to ensure that the gap is properly created, NaNs are inserted,
+        and the gap is closed.
+
+    Assertions
+    ----------
+    - The data points that are intended to be deleted actually exist before the gap
+        creation.
+    - After creating a small gap, check that the gap was made by confirming the absence
+        of the specified data points.
+    - Check that NaNs are correctly inserted into the specified positions in the data.
+    - After closing the gaps, verify that the specified data points are no longer
+        present in the data.
+
+    """
+
+    def get_mock_site_list(*args, **kwargs):
+        _ = args, kwargs
+        return mock_site_list
+
+    def get_mock_measurement_list(*args, **kwargs):
+        _ = args, kwargs
+        return mock_measurement_list
+
+    def get_mock_get_data(*args, **kwargs):
+        xml, data_func = mock_get_data
+        return xml, data_func(*args, **kwargs)
+
+    def get_mock_qc_evaluator_dict(*args, **kwargs):
+        _ = args, kwargs
+        return mock_qc_evaluator_dict
+
+    ann.configure(stream_format_str="%(function_name)s | %(site)s")
+
+    # Here we patch the Hilltop Class
+    monkeypatch.setattr(Hilltop, "get_site_list", get_mock_site_list)
+    monkeypatch.setattr(Hilltop, "get_measurement_list", get_mock_measurement_list)
+    monkeypatch.setattr(
+        data_sources,
+        "get_qc_evaluator_dict",
+        get_mock_qc_evaluator_dict,
+    )
+
+    # However, in this case, we need to patch the INSTANCE as imported in
+    # data_acquisition. Not sure if this makes sense to me, but it works.
+    monkeypatch.setattr("hydrobot.data_acquisition.get_data", get_mock_get_data)
+
+    pr = processor.Processor(
+        base_url="https://greenwashed.and.pleasant/",
+        site=SITES[1],
+        standard_hts="GreenPasturesAreNaturalAndEcoFriendlyISwear.hts",
+        standard_measurement_name=MEASUREMENTS[0],
+        frequency="5min",
+    )
+
+    # Checking that the data points I want to delete actually exist:
+    start_idx = "2023-01-01 00:20:00"
+    end_idx = "2023-01-01 00:25:00"
+    assert pd.to_datetime(start_idx) in pr.standard_series
+    assert pd.to_datetime(end_idx) in pr.standard_series
+
+    # Make a small gap
+    pr.delete_range(start_idx, end_idx)
+
+    # Check that gap was made
+    assert (
+        pd.to_datetime(start_idx) not in pr.standard_series
+    ), "processor.delete_range appears to be broken."
+    assert (
+        pd.to_datetime(end_idx) not in pr.standard_series
+    ), "processor.delete_range appears to be broken."
+
+    # Insert nans where values are missing
+    pr.insert_missing_nans()
+
+    # Check that NaNs are inserted
+    assert pd.isna(
+        pr.standard_series[start_idx]
+    ), "processor.insert_missing_nans appears to be broken."
+    assert pd.isna(
+        pr.standard_series[end_idx]
+    ), "processor.insert_missing_nans appears to be broken."
+
+    # "Close" gaps (i.e. remove nan rows)
+    pr.gap_closer()
+
+    # Check that gap was closed
+    assert (
+        pd.to_datetime(start_idx) not in pr.standard_series
+    ), "processor.gap_closer appears to be broken."
+    assert (
+        pd.to_datetime(end_idx) not in pr.standard_series
+    ), "processor.gap_closer appears to be broken."
+
+
+def test_data_export(
+    monkeypatch,
+    mock_site_list,
+    mock_measurement_list,
+    mock_get_data,
+    mock_qc_evaluator_dict,
+    tmp_path,
+):
+    """
+    Test the 'gap_closer' method of the Processor class.
+
+    Parameters
+    ----------
+    monkeypatch : pytest.MonkeyPatch
+        Pytest fixture to modify or mock modules during testing.
+    mock_site_list : pytest fixture
+        Mocked response for the site list.
+    mock_measurement_list : pytest fixture
+        Mocked response for the measurement list.
+    mock_get_data : pytest fixture
+        Mock response for the get_data server call method.
+    mock_qc_evaluator_dict : pytest fixture
+        Mocked response for the quality control evaluator dictionary.
+
+    Notes
+    -----
+    - This test checks the functionality of the 'gap_closer' method in the Processor
+        class.
+    - It involves creating a Processor object, making a gap in the data, inserting NaNs,
+        and then closing the gap.
+    - Assertions are made to ensure that the gap is properly created, NaNs are inserted,
+        and the gap is closed.
+
+    Assertions
+    ----------
+    - The data points that are intended to be deleted actually exist before the gap
+        creation.
+    - After creating a small gap, check that the gap was made by confirming the absence
+        of the specified data points.
+    - Check that NaNs are correctly inserted into the specified positions in the data.
+    - After closing the gaps, verify that the specified data points are no longer
+        present in the data.
+
+    """
+
+    def get_mock_site_list(*args, **kwargs):
+        _ = args, kwargs
+        return mock_site_list
+
+    def get_mock_measurement_list(*args, **kwargs):
+        _ = args, kwargs
+        return mock_measurement_list
+
+    def get_mock_get_data(*args, **kwargs):
+        xml, data_func = mock_get_data
+        return xml, data_func(*args, **kwargs)
+
+    def get_mock_qc_evaluator_dict(*args, **kwargs):
+        _ = args, kwargs
+        return mock_qc_evaluator_dict
+
+    ann.configure(stream_format_str="%(function_name)s | %(site)s")
+
+    # Here we patch the Hilltop Class
+    monkeypatch.setattr(Hilltop, "get_site_list", get_mock_site_list)
+    monkeypatch.setattr(Hilltop, "get_measurement_list", get_mock_measurement_list)
+    monkeypatch.setattr(
+        data_sources,
+        "get_qc_evaluator_dict",
+        get_mock_qc_evaluator_dict,
+    )
+
+    # However, in this case, we need to patch the INSTANCE as imported in
+    # data_acquisition. Not sure if this makes sense to me, but it works.
+    monkeypatch.setattr("hydrobot.data_acquisition.get_data", get_mock_get_data)
+
+    pr = processor.Processor(
+        base_url="https://greenwashed.and.pleasant/",
+        site=SITES[1],
+        standard_hts="GreenPasturesAreNaturalAndEcoFriendlyISwear.hts",
+        standard_measurement_name=MEASUREMENTS[0],
+        frequency="5min",
+    )
+
+    # Checking that the data points I want to delete actually exist:
+    start_idx = "2023-01-01 00:20:00"
+    end_idx = "2023-01-01 00:25:00"
+    assert pd.to_datetime(start_idx) in pr.standard_series
+    assert pd.to_datetime(end_idx) in pr.standard_series
+
+    # =======================Make a small gap========================
+    print("Gappy Chappy")
+    pr.delete_range(start_idx, end_idx)
+
+    gap_path_csv = tmp_path / "gap_output.csv"
+    gap_path_hilltop_csv = tmp_path / "gap_output_hilltop"
+    gap_path_xml = tmp_path / "gap_output.xml"
+
+    pr.data_exporter(gap_path_csv, ftype="csv")
+
+    read_csv_df = pd.read_csv(gap_path_csv)
+    # Check that the csv was filled in with nans where there are no quality values
+    assert pd.isna(read_csv_df["General Nastiness [Quality]"].iloc[1])
+
+    # The hilltop_csv format outputs two files:
+    # one for standard and qc together,
+    # and one for check data alone.
+    pr.data_exporter(gap_path_hilltop_csv, ftype="hilltop_csv")
+    hilltop_path_std_qc = tmp_path / "gap_output_hilltop_std_qc.csv"
+    hilltop_path_check = tmp_path / "gap_output_hilltop_check.csv"
+
+    read_hilltop_std_qc_csv_df = pd.read_csv(hilltop_path_std_qc)
+    read_hilltop_check_csv_df = pd.read_csv(hilltop_path_check)
+
+    # Check that the deleted values have not been filled somehow
+    assert start_idx not in list(read_hilltop_std_qc_csv_df.index)
+    assert start_idx not in list(read_hilltop_check_csv_df.index)
+
+    print("Before xml export:", pr.quality_series.index)
+    pr.data_exporter(gap_path_xml, ftype="xml")
+    print("After xml export:", pr.quality_series.index)
+    gap_path_xml_tree = DefusedElementTree.fromstring(gap_path_xml.read_text())
+    gap_path_blob = data_structure.parse_xml(gap_path_xml_tree)
+
+    std_indices = gap_path_blob[0].data.timeseries.index
+    assert pd.Timestamp(start_idx) not in list(std_indices)
+
+    # =======================Insert Nans========================
+    # This is how we internally represent gaps. They need to be converted to the Gap
+    # tag for xml export.
+    print("Before nans:", pr.quality_series.index)
+    pr.insert_missing_nans()
+    print("After nans:", pr.quality_series.index)
+
+    pr.data_exporter(gap_path_csv, ftype="csv")
+
+    read_csv_df = pd.read_csv(gap_path_csv)
+    # Check that the csv was filled in with nans where there are no quality values
+    # assert pd.isna(read_csv_df["General Nastiness [Quality]"].iloc[1])
+
+    # The hilltop_csv format outputs two files:
+    # one for standard and qc together,
+    # and one for check data alone.
+    pr.data_exporter(gap_path_hilltop_csv, ftype="hilltop_csv")
+
+    read_hilltop_std_qc_csv_df = pd.read_csv(hilltop_path_std_qc)
+    read_hilltop_check_csv_df = pd.read_csv(hilltop_path_check)
+
+    # Check that the deleted values have not been filled somehow
+    # assert start_idx not in list(read_hilltop_std_qc_csv_df.index)
+    # assert start_idx not in list(read_hilltop_check_csv_df.index)
+    print(read_hilltop_std_qc_csv_df)
+    print(read_hilltop_check_csv_df)
+    # assert start_idx not in list(read_hilltop_std_qc_csv_df.index)
+
+    pr.data_exporter(gap_path_xml, ftype="xml")
+
+    print(gap_path_xml.read_text())
+    gap_path_xml_tree = DefusedElementTree.fromstring(gap_path_xml.read_text())
+    gap_path_blob = data_structure.parse_xml(gap_path_xml_tree)
+
+    std_indices = gap_path_blob[0].data.timeseries.index
+    assert start_idx not in list(std_indices)
```

### Comparing `hydrobot-0.5.0/tests/test_utils.py` & `hydrobot-0.5.1/tests/test_utils.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-"""Test the filters module."""
-
-import numpy as np
-import pandas as pd
-import pytest
-
-import hydrobot.utils as utils
-
-mowsecs_data_dict = {
-    "2619302400": 42,
-    "2619302700": 42,
-    "2619303000": 42,
-    "2619303300": 42,
-    "2619303600": 42,
-    "2619303900": 42,
-    "2619304200": 42,
-    "2619304500": 42,
-    "2619304800": 42,
-    "2619305100": 42,
-}
-
-datetime_data_dict = {
-    "2023-01-01 00:00:00": 42,
-    "2023-01-01 00:05:00": 42,
-    "2023-01-01 00:10:00": 42,
-    "2023-01-01 00:15:00": 42,
-    "2023-01-01 00:20:00": 42,
-    "2023-01-01 00:25:00": 42,
-    "2023-01-01 00:30:00": 42,
-    "2023-01-01 00:35:00": 42,
-    "2023-01-01 00:40:00": 42,
-    "2023-01-01 00:45:00": 42,
-}
-
-
-@pytest.fixture()
-def mowsecs_data():
-    """Get example data for testing.
-
-    Do not change these values!
-    """
-    # Allows parametrization with a list of keys to change to np.nan
-    return pd.Series(mowsecs_data_dict)
-
-
-@pytest.fixture()
-def datetime_data():
-    """Get example data for testing.
-
-    Do not change these values!
-    """
-    # Allows parametrization with a list of keys to change to np.nan
-    data = pd.Series(datetime_data_dict)
-    data.index = pd.to_datetime(data.index)
-    return data
-
-
-def test_mowsecs_to_timestamp(mowsecs_data, datetime_data):
-    """Test mowsecs_to_datetime_index utility."""
-    for mowsec, timestamp in zip(
-        mowsecs_data.index.values, datetime_data.index.values, strict=True
-    ):
-        ms_to_dt = utils.mowsecs_to_timestamp(mowsec)
-        assert ms_to_dt == timestamp
-
-        str_ms_to_dt = utils.mowsecs_to_timestamp(str(mowsec))
-        assert str_ms_to_dt == timestamp
-
-        float_ms_to_dt = utils.mowsecs_to_timestamp(float(mowsec))
-        assert float_ms_to_dt == timestamp
-
-
-def test_timestamp_to_mowsecs(mowsecs_data, datetime_data):
-    """Test mowsecs_to_datetime_index utility."""
-    for timestamp, mowsec in zip(
-        datetime_data.index.values, mowsecs_data.index.values, strict=True
-    ):
-        dt_to_ms = utils.timestamp_to_mowsecs(timestamp)
-
-        assert dt_to_ms == int(mowsec)
-
-
-def test_mowsecs_to_datetime_index(mowsecs_data, datetime_data):
-    """Test mowsecs_to_datetime_index utility."""
-    ms_to_dt = utils.mowsecs_to_datetime_index(mowsecs_data.index)
-
-    assert ms_to_dt.equals(datetime_data.index)
-
-
-def test_datetime_index_to_mowsecs(mowsecs_data, datetime_data):
-    """Test mowsecs_to_datetime_index utility."""
-    dt_to_ms = utils.datetime_index_to_mowsecs(datetime_data.index)
-
-    assert dt_to_ms.equals(mowsecs_data.index.astype(np.int64))
+"""Test the filters module."""
+
+import numpy as np
+import pandas as pd
+import pytest
+
+import hydrobot.utils as utils
+
+mowsecs_data_dict = {
+    "2619302400": 42,
+    "2619302700": 42,
+    "2619303000": 42,
+    "2619303300": 42,
+    "2619303600": 42,
+    "2619303900": 42,
+    "2619304200": 42,
+    "2619304500": 42,
+    "2619304800": 42,
+    "2619305100": 42,
+}
+
+datetime_data_dict = {
+    "2023-01-01 00:00:00": 42,
+    "2023-01-01 00:05:00": 42,
+    "2023-01-01 00:10:00": 42,
+    "2023-01-01 00:15:00": 42,
+    "2023-01-01 00:20:00": 42,
+    "2023-01-01 00:25:00": 42,
+    "2023-01-01 00:30:00": 42,
+    "2023-01-01 00:35:00": 42,
+    "2023-01-01 00:40:00": 42,
+    "2023-01-01 00:45:00": 42,
+}
+
+
+@pytest.fixture()
+def mowsecs_data():
+    """Get example data for testing.
+
+    Do not change these values!
+    """
+    # Allows parametrization with a list of keys to change to np.nan
+    return pd.Series(mowsecs_data_dict)
+
+
+@pytest.fixture()
+def datetime_data():
+    """Get example data for testing.
+
+    Do not change these values!
+    """
+    # Allows parametrization with a list of keys to change to np.nan
+    data = pd.Series(datetime_data_dict)
+    data.index = pd.to_datetime(data.index)
+    return data
+
+
+def test_mowsecs_to_timestamp(mowsecs_data, datetime_data):
+    """Test mowsecs_to_datetime_index utility."""
+    for mowsec, timestamp in zip(
+        mowsecs_data.index.values, datetime_data.index.values, strict=True
+    ):
+        ms_to_dt = utils.mowsecs_to_timestamp(mowsec)
+        assert ms_to_dt == timestamp
+
+        str_ms_to_dt = utils.mowsecs_to_timestamp(str(mowsec))
+        assert str_ms_to_dt == timestamp
+
+        float_ms_to_dt = utils.mowsecs_to_timestamp(float(mowsec))
+        assert float_ms_to_dt == timestamp
+
+
+def test_timestamp_to_mowsecs(mowsecs_data, datetime_data):
+    """Test mowsecs_to_datetime_index utility."""
+    for timestamp, mowsec in zip(
+        datetime_data.index.values, mowsecs_data.index.values, strict=True
+    ):
+        dt_to_ms = utils.timestamp_to_mowsecs(timestamp)
+
+        assert dt_to_ms == int(mowsec)
+
+
+def test_mowsecs_to_datetime_index(mowsecs_data, datetime_data):
+    """Test mowsecs_to_datetime_index utility."""
+    ms_to_dt = utils.mowsecs_to_datetime_index(mowsecs_data.index)
+
+    assert ms_to_dt.equals(datetime_data.index)
+
+
+def test_datetime_index_to_mowsecs(mowsecs_data, datetime_data):
+    """Test mowsecs_to_datetime_index utility."""
+    dt_to_ms = utils.datetime_index_to_mowsecs(datetime_data.index)
+
+    assert dt_to_ms.equals(mowsecs_data.index.astype(np.int64))
```

### Comparing `hydrobot-0.5.0/tests/test_web_integration.py` & `hydrobot-0.5.1/tests/test_web_integration.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,670 +1,670 @@
-"""Test actual integration tests."""
-from xml.etree import ElementTree
-
-import pandas as pd
-import pytest
-from annalist.annalist import Annalist
-from defusedxml import ElementTree as DefusedElementTree
-from hilltoppy.utils import build_url, get_hilltop_xml
-
-from hydrobot.data_structure import parse_xml, write_hilltop_xml
-from hydrobot.processor import Processor
-
-
-@pytest.mark.slow()
-@pytest.mark.remote()
-def test_data_structure_integration(tmp_path):
-    """
-    Test connection to the actual server.
-
-    Parameters
-    ----------
-    tmp_path : pathlib.Path
-        The temporary path for storing log files and exported data.
-
-    Notes
-    -----
-    This test checks the connection to the specified server and various functionalities
-    of the Processor class.
-    The test configuration includes parameters such as base_url, file names,
-    site information, date range, and default settings.
-    Annalist is configured to log information during the test.
-    Processor is instantiated with the provided processing parameters.
-    Assertions are made to ensure that essential series (`standard_series`, `check_data`
-    , `check_series`, `quality_series`) are not empty.
-    Data clipping, removal of flatlined values and spikes, range deletion, insertion of
-    missing NaNs, gap closure, quality encoding, XML data structure creation,
-    data export, and diagnosis are tested.
-
-    Assertions
-    ----------
-    Various assertions are included throughout the test to verify the expected behavior
-    of Processor methods and properties.
-    These assertions cover the state of data series before and after certain operations,
-    ensuring data integrity and functionality.
-    """
-    processing_parameters = {
-        "base_url": "http://hilltopdev.horizons.govt.nz/",
-        "standard_hts_filename": "RawLogger.hts",
-        "check_hts_filename": "boo.hts",
-        "site": "Whanganui at Te Rewa",
-        "from_date": "2021-06-28 00:00",
-        "to_date": "2021-07-01 23:00",
-        "frequency": "5min",
-        "standard_measurement_name": "Stage",
-        "check_measurement_name": "External S.G. [Water Level NRT]",
-        "defaults": {
-            "high_clip": 20000,
-            "low_clip": 0,
-            "delta": 1000,
-            "span": 10,
-            "gap_limit": 12,
-            "max_qc": 600,
-        },
-    }
-
-    # standard data
-
-    standard_url = build_url(
-        processing_parameters["base_url"],
-        processing_parameters["standard_hts_filename"],
-        "GetData",
-        site=processing_parameters["site"],
-        measurement=processing_parameters["standard_measurement_name"],
-        from_date=processing_parameters["from_date"],
-        to_date=processing_parameters["to_date"],
-        tstype="Standard",
-    )
-
-    standard_hilltop_xml = get_hilltop_xml(standard_url)
-
-    standard_root = ElementTree.ElementTree(standard_hilltop_xml)
-
-    standard_input_path = tmp_path / "standard_input.xml"
-
-    standard_root.write(standard_input_path)
-
-    ElementTree.indent(standard_root, space="    ")
-
-    standard_output_path = tmp_path / "standard_output.xml"
-
-    standard_root.write(standard_output_path)
-
-    standard_blobs = parse_xml(standard_root)
-
-    write_hilltop_xml(standard_blobs, standard_output_path)
-
-    with open(standard_input_path) as f:
-        standard_input_xml = f.read()
-
-    with open(standard_output_path) as f:
-        standard_output_xml = f.read()
-
-    standard_input_tree = DefusedElementTree.fromstring(standard_input_xml)
-    standard_output_tree = DefusedElementTree.fromstring(standard_output_xml)
-
-    assert ElementTree.indent(standard_input_tree) == ElementTree.indent(
-        standard_output_tree
-    )
-    # Quality data
-
-    quality_url = build_url(
-        processing_parameters["base_url"],
-        processing_parameters["standard_hts_filename"],
-        "GetData",
-        site=processing_parameters["site"],
-        measurement=processing_parameters["standard_measurement_name"],
-        tstype="Quality",
-    )
-
-    quality_hilltop_xml = get_hilltop_xml(quality_url)
-
-    quality_root = ElementTree.ElementTree(quality_hilltop_xml)
-
-    quality_input_path = tmp_path / "quality_input.xml"
-
-    quality_root.write(quality_input_path)
-
-    ElementTree.indent(quality_root, space="    ")
-
-    quality_blobs = parse_xml(quality_root)
-
-    quality_output_path = tmp_path / "quality_output.xml"
-
-    write_hilltop_xml(quality_blobs, quality_output_path)
-
-    with open(quality_input_path) as f:
-        quality_input_xml = f.read()
-
-    with open(quality_output_path) as f:
-        quality_output_xml = f.read()
-
-    quality_input_tree = DefusedElementTree.fromstring(quality_input_xml)
-    quality_output_tree = DefusedElementTree.fromstring(quality_output_xml)
-
-    assert ElementTree.indent(quality_input_tree) == ElementTree.indent(
-        quality_output_tree
-    )
-
-    # Check data
-
-    check_url = build_url(
-        processing_parameters["base_url"],
-        processing_parameters["check_hts_filename"],
-        "GetData",
-        site=processing_parameters["site"],
-        measurement=processing_parameters["check_measurement_name"],
-        tstype="Check",
-    )
-
-    check_hilltop_xml = get_hilltop_xml(check_url)
-
-    check_root = ElementTree.ElementTree(check_hilltop_xml)
-
-    check_input_path = tmp_path / "check_input.xml"
-
-    check_root.write(check_input_path)
-
-    ElementTree.indent(check_root, space="    ")
-
-    check_blobs = parse_xml(check_root)
-
-    check_output_path = tmp_path / "check_output.xml"
-
-    write_hilltop_xml(check_blobs, check_output_path)
-
-    with open(check_input_path) as f:
-        check_input_xml = f.read()
-
-    with open(check_output_path) as f:
-        check_output_xml = f.read()
-
-    check_input_tree = DefusedElementTree.fromstring(check_input_xml)
-    check_output_tree = DefusedElementTree.fromstring(check_output_xml)
-
-    assert ElementTree.indent(check_input_tree) == ElementTree.indent(check_output_tree)
-
-
-@pytest.mark.slow()
-@pytest.mark.remote()
-def test_processor_integration(tmp_path):
-    """
-    Test connection to the actual server.
-
-    Parameters
-    ----------
-    tmp_path : pathlib.Path
-        The temporary path for storing log files and exported data.
-
-    Notes
-    -----
-    This test checks the connection to the specified server and various functionalities
-    of the Processor class. The test configuration includes parameters such as
-    base_url, file names, site information, date range, and default settings.
-
-    Annalist is configured to log information during the test.
-    Processor is instantiated with the provided processing parameters.
-    Assertions are made to ensure that essential series (standard_series, check_data,
-    check_series, quality_series) are not empty.
-
-    Data clipping, removal of flatlined values and spikes, range deletion, insertion of
-    missing NaNs, gap closure, quality encoding, XML data structure creation, data
-    export, and diagnosis are tested.
-
-    Assertions
-    ----------
-    Various assertions are included throughout the test to verify the expected behavior
-    of Processor methods and properties.
-
-    These assertions cover the state of data series before and after certain
-    operations, ensuring data integrity and functionality.
-    """
-    processing_parameters = {
-        "base_url": "http://hilltopdev.horizons.govt.nz/",
-        "standard_hts_filename": "RawLogger.hts",
-        "check_hts_filename": "boo.hts",
-        "site": "Whanganui at Te Rewa",
-        "from_date": "2021-01-01 00:00",
-        "to_date": "2021-02-02 23:00",
-        "frequency": "5min",
-        "standard_measurement_name": "Water level statistics: Point Sample",
-        "check_measurement_name": "External S.G. [Water Level NRT]",
-        "defaults": {
-            "high_clip": 5000,
-            "low_clip": 0,
-            "delta": 1000,
-            "span": 10,
-            "gap_limit": 12,
-            "max_qc": 600,
-        },
-    }
-
-    ann = Annalist()
-    format_str = format_str = (
-        "%(asctime)s, %(analyst_name)s, %(function_name)s, %(site)s, "
-        "%(measurement)s, %(from_date)s, %(to_date)s, %(message)s"
-    )
-    ann.configure(
-        logfile=tmp_path / "bot_annals.csv",
-        analyst_name="Annie the analyst!",
-        stream_format_str=format_str,
-    )
-
-    data = Processor(
-        processing_parameters["base_url"],
-        processing_parameters["site"],
-        processing_parameters["standard_hts_filename"],
-        processing_parameters["standard_measurement_name"],
-        processing_parameters["frequency"],
-        processing_parameters["from_date"],
-        processing_parameters["to_date"],
-        processing_parameters["check_hts_filename"],
-        processing_parameters["check_measurement_name"],
-        processing_parameters["defaults"],
-    )
-
-    assert not data.standard_series.empty
-    assert not data.check_series.empty
-    assert not data.quality_series.empty
-
-    standard_before_clip = data.standard_series
-    check_before_clip = data.check_series
-
-    data.clip()
-
-    standard_after_clip = data.standard_series
-    check_after_clip = data.check_series
-
-    assert not standard_before_clip.equals(standard_after_clip)
-    assert check_before_clip.equals(check_after_clip)
-
-    assert (
-        data.standard_series[
-            standard_before_clip > processing_parameters["defaults"]["high_clip"]
-        ]
-        .isna()
-        .all()
-    )
-    assert (
-        data.check_series[
-            check_before_clip > processing_parameters["defaults"]["high_clip"]
-        ]
-        .isna()
-        .all()
-    )
-
-    data.remove_flatlined_values()
-    # TODO: Write test for remove_flatlined_values
-
-    data.remove_spikes()
-    # TODO: Write test for remove_spikes
-
-    # Checking that the data points I want to delete actually exist:
-    start_idx = "2021-01-01 11:00"
-    end_idx = "2021-01-01 11:30"
-    assert pd.to_datetime(start_idx) in data.standard_series
-    assert pd.to_datetime(end_idx) in data.standard_series
-
-    # Make a small gap
-    data.delete_range(start_idx, end_idx)
-
-    # Check that gap was made
-    assert (
-        pd.to_datetime(start_idx) not in data.standard_series
-    ), "processor.delete_range appears to be broken."
-    assert (
-        pd.to_datetime(end_idx) not in data.standard_series
-    ), "processor.delete_range appears to be broken."
-
-    # Insert nans where values are missing
-    data.insert_missing_nans()
-
-    # Check that NaNs are inserted
-    assert pd.isna(
-        data.standard_series[start_idx]
-    ), "processor.insert_missing_nans appears to be broken."
-    assert pd.isna(
-        data.standard_series[end_idx]
-    ), "processor.insert_missing_nans appears to be broken."
-
-    # "Close" gaps (i.e. remove nan rows)
-    data.gap_closer()
-
-    # Check that gap was closed
-    assert (
-        pd.to_datetime(start_idx) not in data.standard_series
-    ), "processor.gap_closer appears to be broken."
-    assert (
-        pd.to_datetime(end_idx) not in data.standard_series
-    ), "processor.gap_closer appears to be broken."
-
-    data.quality_encoder()
-
-    # TODO: Write test for quality_encoder
-
-    data.to_xml_data_structure()
-
-    # TODO: Write test for to_xml_data_structure
-
-    data.data_exporter(tmp_path / "xml_data.xml")
-    data.data_exporter(tmp_path / "csv_data.csv", ftype="csv")
-    data.data_exporter(tmp_path / "hilltop_csv_data.csv", ftype="hilltop_csv")
-
-    # TODO: Write tests for data_exporter
-
-    data.diagnosis()
-
-
-@pytest.mark.slow()
-@pytest.mark.remote()
-def test_empty_response(tmp_path):
-    """
-    Test the handling of an empty server response.
-
-    Parameters
-    ----------
-    tmp_path : pathlib.Path
-        The temporary path for storing log files and exported data.
-
-    Notes
-    -----
-    This test checks the connection to the specified server and various functionalities
-    of the Processor class.
-
-    The test configuration includes parameters such as base_url, file names, site
-    information, date range, and default settings.
-
-    Annalist is configured to log information during the test.
-    Processor is instantiated with the provided processing parameters.
-    Assertions are made to ensure that essential series (standard_series, check_data,
-    check_series, quality_series) are not empty.
-
-    Data clipping, removal of flatlined values and spikes, range deletion, insertion of
-    missing NaNs, gap closure, quality encoding, XML data structure creation, data
-    export, and diagnosis are tested.
-
-    Assertions
-    ----------
-    Various assertions are included throughout the test to verify the expected behavior
-    of Processor methods and properties.
-    These assertions cover the state of data series before and after certain
-    operations, ensuring data integrity and functionality.
-    """
-    processing_parameters = {
-        "base_url": "http://hilltopdev.horizons.govt.nz/",
-        "standard_hts_filename": "RawLogger.hts",
-        "check_hts_filename": "boo.hts",
-        "site": "Whanganui at Te Rewa",
-        "from_date": "2003-01-01 00:00",
-        "to_date": "2003-02-02 23:00",
-        "frequency": "5min",
-        "standard_measurement_name": "Water level statistics: Point Sample",
-        "check_measurement_name": "External S.G. [Water Level NRT]",
-        "defaults": {
-            "high_clip": 5000,
-            "low_clip": 0,
-            "delta": 1000,
-            "span": 10,
-            "gap_limit": 12,
-            "max_qc": 600,
-        },
-    }
-
-    with pytest.warns(UserWarning):
-        ann = Annalist()
-        format_str = format_str = (
-            "%(asctime)s, %(analyst_name)s, %(function_name)s, %(site)s, "
-            "%(measurement)s, %(from_date)s, %(to_date)s, %(message)s"
-        )
-        ann.configure(
-            logfile=tmp_path / "bot_annals.csv",
-            analyst_name="Annie the analyst!",
-            stream_format_str=format_str,
-        )
-
-        data = Processor(
-            processing_parameters["base_url"],
-            processing_parameters["site"],
-            processing_parameters["standard_hts_filename"],
-            processing_parameters["standard_measurement_name"],
-            processing_parameters["frequency"],
-            processing_parameters["from_date"],
-            processing_parameters["to_date"],
-            processing_parameters["check_hts_filename"],
-            processing_parameters["check_measurement_name"],
-            processing_parameters["defaults"],
-        )
-
-        assert data.standard_series.empty
-        assert data.check_series.empty
-        assert data.quality_series.empty
-        assert data.raw_standard_series.empty
-        assert data.raw_standard_blob is None
-        assert data.raw_standard_xml is None
-        assert data.raw_quality_series.empty
-        assert data.raw_quality_blob is None
-        assert data.raw_quality_xml is None
-        assert data.raw_check_data.empty
-        assert data.raw_check_blob is None
-        assert data.raw_check_xml is None
-
-
-@pytest.mark.slow()
-@pytest.mark.remote()
-def test_failed_requests(tmp_path):
-    """
-    Test the handling of an empty server response.
-
-    Parameters
-    ----------
-    tmp_path : pathlib.Path
-        The temporary path for storing log files and exported data.
-
-    Notes
-    -----
-    This test checks the connection to the specified server and various functionalities
-    of the Processor class.
-
-    The test configuration includes parameters such as base_url, file names, site
-    information, date range, and default settings.
-
-    Annalist is configured to log information during the test.
-    Processor is instantiated with the provided processing parameters.
-    Assertions are made to ensure that essential series (standard_series, check_data,
-    check_series, quality_series) are not empty.
-
-    Data clipping, removal of flatlined values and spikes, range deletion, insertion of
-    missing NaNs, gap closure, quality encoding, XML data structure creation, data
-    export, and diagnosis are tested.
-
-    Assertions
-    ----------
-    Various assertions are included throughout the test to verify the expected behavior
-    of Processor methods and properties.
-    These assertions cover the state of data series before and after certain
-    operations, ensuring data integrity and functionality.
-    """
-    processing_parameters = {
-        "base_url": "http://hilltopdev.horizons.govt.nz/",
-        "standard_hts_filename": "RawLogger.hts",
-        "check_hts_filename": "boo.hts",
-        "site": "Whanganui at Te Rewa",
-        "from_date": "2003-01-01 00:00",
-        "to_date": "2003-02-02 23:00",
-        "frequency": "4min",
-        "standard_measurement_name": "Water level statistics: Point Sample",
-        "check_measurement_name": "External S.G. [Water Level NRT]",
-        "defaults": {
-            "high_clip": 5000,
-            "low_clip": 0,
-            "delta": 1000,
-            "span": 10,
-            "gap_limit": 12,
-            "max_qc": 600,
-        },
-    }
-
-    with pytest.warns(UserWarning):
-        ann = Annalist()
-        format_str = format_str = (
-            "%(asctime)s, %(analyst_name)s, %(function_name)s, %(site)s, "
-            "%(measurement)s, %(from_date)s, %(to_date)s, %(message)s"
-        )
-        ann.configure(
-            logfile=tmp_path / "bot_annals.csv",
-            analyst_name="Annie the analyst!",
-            stream_format_str=format_str,
-        )
-
-        # with pytest.raises(
-        #     ValueError
-        # ) as excinfo:
-        #     _ = Processor(
-        #         processing_parameters["base_url"],
-        #         processing_parameters["site"],
-        #         processing_parameters["standard_hts_filename"],
-        #         processing_parameters["standard_measurement_name"],
-        #         processing_parameters["frequency"],
-        #         processing_parameters["from_date"],
-        #         processing_parameters["to_date"],
-        #         processing_parameters["check_hts_filename"],
-        #         processing_parameters["check_measurement_name"],
-        #         processing_parameters["defaults"],
-        #     )
-        # print(excinfo.value)
-
-        with pytest.raises(
-            ValueError, match=r"No sites found for the base_url and hts combo."
-        ) as excinfo:
-            _ = Processor(
-                processing_parameters["base_url"],
-                processing_parameters["site"],
-                "Notarealhstfile",
-                # processing_parameters["standard_hts_filename"],
-                processing_parameters["standard_measurement_name"],
-                processing_parameters["frequency"],
-                processing_parameters["from_date"],
-                processing_parameters["to_date"],
-                processing_parameters["check_hts_filename"],
-                processing_parameters["check_measurement_name"],
-                processing_parameters["defaults"],
-            )
-        assert "No sites found for the base_url and hts combo." in str(excinfo.value)
-
-        with pytest.raises(
-            ValueError, match=r"Site 'Notarealsite' not found .*"
-        ) as excinfo:
-            _ = Processor(
-                processing_parameters["base_url"],
-                "Notarealsite",
-                processing_parameters["standard_hts_filename"],
-                processing_parameters["standard_measurement_name"],
-                processing_parameters["frequency"],
-                processing_parameters["from_date"],
-                processing_parameters["to_date"],
-                processing_parameters["check_hts_filename"],
-                processing_parameters["check_measurement_name"],
-                processing_parameters["defaults"],
-            )
-        assert "Site 'Notarealsite' not found for both base_url and hts combos." in str(
-            excinfo.value
-        )
-
-        with pytest.raises(ValueError, match=r"Standard measurement name.*") as excinfo:
-            _ = Processor(
-                processing_parameters["base_url"],
-                processing_parameters["site"],
-                processing_parameters["standard_hts_filename"],
-                # processing_parameters["standard_measurement_name"],
-                "Notarealmeasurement",
-                processing_parameters["frequency"],
-                processing_parameters["from_date"],
-                processing_parameters["to_date"],
-                processing_parameters["check_hts_filename"],
-                processing_parameters["check_measurement_name"],
-                processing_parameters["defaults"],
-            )
-        assert (
-            "Standard measurement name 'Notarealmeasurement' not found at site"
-            in str(excinfo.value)
-        )
-
-        with pytest.raises(
-            ValueError,
-            match=r"Unrecognised start time",
-        ) as excinfo:
-            _ = Processor(
-                processing_parameters["base_url"],
-                processing_parameters["site"],
-                processing_parameters["standard_hts_filename"],
-                processing_parameters["standard_measurement_name"],
-                processing_parameters["frequency"],
-                # processing_parameters["from_date"],
-                "Notarealdate",
-                processing_parameters["to_date"],
-                processing_parameters["check_hts_filename"],
-                processing_parameters["check_measurement_name"],
-                processing_parameters["defaults"],
-            )
-        assert "Unrecognised start time" in str(excinfo.value)
-
-        # with pytest.raises(
-        #     ValueError  #, match=r"Unrecognised start time",
-        # ) as excinfo:
-        _ = Processor(
-            processing_parameters["base_url"],
-            processing_parameters["site"],
-            processing_parameters["standard_hts_filename"],
-            processing_parameters["standard_measurement_name"],
-            # processing_parameters["frequency"],
-            "Notarealfrequency",
-            processing_parameters["from_date"],
-            processing_parameters["to_date"],
-            processing_parameters["check_hts_filename"],
-            processing_parameters["check_measurement_name"],
-            processing_parameters["defaults"],
-        )
-        print(excinfo)
-        # assert (
-        #     "Unrecognised start time"
-        #     in str(excinfo.value)
-        # )
-
-        with pytest.raises(
-            ValueError, match=r"No sites found for the base_url and hts combo."
-        ) as excinfo:
-            _ = Processor(
-                processing_parameters["base_url"],
-                processing_parameters["site"],
-                processing_parameters["standard_hts_filename"],
-                processing_parameters["standard_measurement_name"],
-                processing_parameters["frequency"],
-                processing_parameters["from_date"],
-                processing_parameters["to_date"],
-                # processing_parameters["check_hts_filename"],
-                "Notarealhtsfilename",
-                processing_parameters["check_measurement_name"],
-                processing_parameters["defaults"],
-            )
-        assert "No sites found for the base_url and hts combo." in str(excinfo.value)
-
-        with pytest.raises(
-            ValueError, match=r"Check measurement name 'Notarealmeasurement' not found "
-        ) as excinfo:
-            _ = Processor(
-                processing_parameters["base_url"],
-                processing_parameters["site"],
-                processing_parameters["standard_hts_filename"],
-                processing_parameters["standard_measurement_name"],
-                processing_parameters["frequency"],
-                processing_parameters["from_date"],
-                processing_parameters["to_date"],
-                processing_parameters["check_hts_filename"],
-                # processing_parameters["check_measurement_name"],
-                "Notarealmeasurement",
-                processing_parameters["defaults"],
-            )
-        print(excinfo)
-        assert "Check measurement name 'Notarealmeasurement' not found at site " in str(
-            excinfo.value
-        )
+"""Test actual integration tests."""
+from xml.etree import ElementTree
+
+import pandas as pd
+import pytest
+from annalist.annalist import Annalist
+from defusedxml import ElementTree as DefusedElementTree
+from hilltoppy.utils import build_url, get_hilltop_xml
+
+from hydrobot.data_structure import parse_xml, write_hilltop_xml
+from hydrobot.processor import Processor
+
+
+@pytest.mark.slow()
+@pytest.mark.remote()
+def test_data_structure_integration(tmp_path):
+    """
+    Test connection to the actual server.
+
+    Parameters
+    ----------
+    tmp_path : pathlib.Path
+        The temporary path for storing log files and exported data.
+
+    Notes
+    -----
+    This test checks the connection to the specified server and various functionalities
+    of the Processor class.
+    The test configuration includes parameters such as base_url, file names,
+    site information, date range, and default settings.
+    Annalist is configured to log information during the test.
+    Processor is instantiated with the provided processing parameters.
+    Assertions are made to ensure that essential series (`standard_series`, `check_data`
+    , `check_series`, `quality_series`) are not empty.
+    Data clipping, removal of flatlined values and spikes, range deletion, insertion of
+    missing NaNs, gap closure, quality encoding, XML data structure creation,
+    data export, and diagnosis are tested.
+
+    Assertions
+    ----------
+    Various assertions are included throughout the test to verify the expected behavior
+    of Processor methods and properties.
+    These assertions cover the state of data series before and after certain operations,
+    ensuring data integrity and functionality.
+    """
+    processing_parameters = {
+        "base_url": "http://hilltopdev.horizons.govt.nz/",
+        "standard_hts_filename": "RawLogger.hts",
+        "check_hts_filename": "boo.hts",
+        "site": "Whanganui at Te Rewa",
+        "from_date": "2021-06-28 00:00",
+        "to_date": "2021-07-01 23:00",
+        "frequency": "5min",
+        "standard_measurement_name": "Stage",
+        "check_measurement_name": "External S.G. [Water Level NRT]",
+        "defaults": {
+            "high_clip": 20000,
+            "low_clip": 0,
+            "delta": 1000,
+            "span": 10,
+            "gap_limit": 12,
+            "max_qc": 600,
+        },
+    }
+
+    # standard data
+
+    standard_url = build_url(
+        processing_parameters["base_url"],
+        processing_parameters["standard_hts_filename"],
+        "GetData",
+        site=processing_parameters["site"],
+        measurement=processing_parameters["standard_measurement_name"],
+        from_date=processing_parameters["from_date"],
+        to_date=processing_parameters["to_date"],
+        tstype="Standard",
+    )
+
+    standard_hilltop_xml = get_hilltop_xml(standard_url)
+
+    standard_root = ElementTree.ElementTree(standard_hilltop_xml)
+
+    standard_input_path = tmp_path / "standard_input.xml"
+
+    standard_root.write(standard_input_path)
+
+    ElementTree.indent(standard_root, space="    ")
+
+    standard_output_path = tmp_path / "standard_output.xml"
+
+    standard_root.write(standard_output_path)
+
+    standard_blobs = parse_xml(standard_root)
+
+    write_hilltop_xml(standard_blobs, standard_output_path)
+
+    with open(standard_input_path) as f:
+        standard_input_xml = f.read()
+
+    with open(standard_output_path) as f:
+        standard_output_xml = f.read()
+
+    standard_input_tree = DefusedElementTree.fromstring(standard_input_xml)
+    standard_output_tree = DefusedElementTree.fromstring(standard_output_xml)
+
+    assert ElementTree.indent(standard_input_tree) == ElementTree.indent(
+        standard_output_tree
+    )
+    # Quality data
+
+    quality_url = build_url(
+        processing_parameters["base_url"],
+        processing_parameters["standard_hts_filename"],
+        "GetData",
+        site=processing_parameters["site"],
+        measurement=processing_parameters["standard_measurement_name"],
+        tstype="Quality",
+    )
+
+    quality_hilltop_xml = get_hilltop_xml(quality_url)
+
+    quality_root = ElementTree.ElementTree(quality_hilltop_xml)
+
+    quality_input_path = tmp_path / "quality_input.xml"
+
+    quality_root.write(quality_input_path)
+
+    ElementTree.indent(quality_root, space="    ")
+
+    quality_blobs = parse_xml(quality_root)
+
+    quality_output_path = tmp_path / "quality_output.xml"
+
+    write_hilltop_xml(quality_blobs, quality_output_path)
+
+    with open(quality_input_path) as f:
+        quality_input_xml = f.read()
+
+    with open(quality_output_path) as f:
+        quality_output_xml = f.read()
+
+    quality_input_tree = DefusedElementTree.fromstring(quality_input_xml)
+    quality_output_tree = DefusedElementTree.fromstring(quality_output_xml)
+
+    assert ElementTree.indent(quality_input_tree) == ElementTree.indent(
+        quality_output_tree
+    )
+
+    # Check data
+
+    check_url = build_url(
+        processing_parameters["base_url"],
+        processing_parameters["check_hts_filename"],
+        "GetData",
+        site=processing_parameters["site"],
+        measurement=processing_parameters["check_measurement_name"],
+        tstype="Check",
+    )
+
+    check_hilltop_xml = get_hilltop_xml(check_url)
+
+    check_root = ElementTree.ElementTree(check_hilltop_xml)
+
+    check_input_path = tmp_path / "check_input.xml"
+
+    check_root.write(check_input_path)
+
+    ElementTree.indent(check_root, space="    ")
+
+    check_blobs = parse_xml(check_root)
+
+    check_output_path = tmp_path / "check_output.xml"
+
+    write_hilltop_xml(check_blobs, check_output_path)
+
+    with open(check_input_path) as f:
+        check_input_xml = f.read()
+
+    with open(check_output_path) as f:
+        check_output_xml = f.read()
+
+    check_input_tree = DefusedElementTree.fromstring(check_input_xml)
+    check_output_tree = DefusedElementTree.fromstring(check_output_xml)
+
+    assert ElementTree.indent(check_input_tree) == ElementTree.indent(check_output_tree)
+
+
+@pytest.mark.slow()
+@pytest.mark.remote()
+def test_processor_integration(tmp_path):
+    """
+    Test connection to the actual server.
+
+    Parameters
+    ----------
+    tmp_path : pathlib.Path
+        The temporary path for storing log files and exported data.
+
+    Notes
+    -----
+    This test checks the connection to the specified server and various functionalities
+    of the Processor class. The test configuration includes parameters such as
+    base_url, file names, site information, date range, and default settings.
+
+    Annalist is configured to log information during the test.
+    Processor is instantiated with the provided processing parameters.
+    Assertions are made to ensure that essential series (standard_series, check_data,
+    check_series, quality_series) are not empty.
+
+    Data clipping, removal of flatlined values and spikes, range deletion, insertion of
+    missing NaNs, gap closure, quality encoding, XML data structure creation, data
+    export, and diagnosis are tested.
+
+    Assertions
+    ----------
+    Various assertions are included throughout the test to verify the expected behavior
+    of Processor methods and properties.
+
+    These assertions cover the state of data series before and after certain
+    operations, ensuring data integrity and functionality.
+    """
+    processing_parameters = {
+        "base_url": "http://hilltopdev.horizons.govt.nz/",
+        "standard_hts_filename": "RawLogger.hts",
+        "check_hts_filename": "boo.hts",
+        "site": "Whanganui at Te Rewa",
+        "from_date": "2021-01-01 00:00",
+        "to_date": "2021-02-02 23:00",
+        "frequency": "5min",
+        "standard_measurement_name": "Water level statistics: Point Sample",
+        "check_measurement_name": "External S.G. [Water Level NRT]",
+        "defaults": {
+            "high_clip": 5000,
+            "low_clip": 0,
+            "delta": 1000,
+            "span": 10,
+            "gap_limit": 12,
+            "max_qc": 600,
+        },
+    }
+
+    ann = Annalist()
+    format_str = format_str = (
+        "%(asctime)s, %(analyst_name)s, %(function_name)s, %(site)s, "
+        "%(measurement)s, %(from_date)s, %(to_date)s, %(message)s"
+    )
+    ann.configure(
+        logfile=tmp_path / "bot_annals.csv",
+        analyst_name="Annie the analyst!",
+        stream_format_str=format_str,
+    )
+
+    data = Processor(
+        processing_parameters["base_url"],
+        processing_parameters["site"],
+        processing_parameters["standard_hts_filename"],
+        processing_parameters["standard_measurement_name"],
+        processing_parameters["frequency"],
+        processing_parameters["from_date"],
+        processing_parameters["to_date"],
+        processing_parameters["check_hts_filename"],
+        processing_parameters["check_measurement_name"],
+        processing_parameters["defaults"],
+    )
+
+    assert not data.standard_series.empty
+    assert not data.check_series.empty
+    assert not data.quality_series.empty
+
+    standard_before_clip = data.standard_series
+    check_before_clip = data.check_series
+
+    data.clip()
+
+    standard_after_clip = data.standard_series
+    check_after_clip = data.check_series
+
+    assert not standard_before_clip.equals(standard_after_clip)
+    assert check_before_clip.equals(check_after_clip)
+
+    assert (
+        data.standard_series[
+            standard_before_clip > processing_parameters["defaults"]["high_clip"]
+        ]
+        .isna()
+        .all()
+    )
+    assert (
+        data.check_series[
+            check_before_clip > processing_parameters["defaults"]["high_clip"]
+        ]
+        .isna()
+        .all()
+    )
+
+    data.remove_flatlined_values()
+    # TODO: Write test for remove_flatlined_values
+
+    data.remove_spikes()
+    # TODO: Write test for remove_spikes
+
+    # Checking that the data points I want to delete actually exist:
+    start_idx = "2021-01-01 11:00"
+    end_idx = "2021-01-01 11:30"
+    assert pd.to_datetime(start_idx) in data.standard_series
+    assert pd.to_datetime(end_idx) in data.standard_series
+
+    # Make a small gap
+    data.delete_range(start_idx, end_idx)
+
+    # Check that gap was made
+    assert (
+        pd.to_datetime(start_idx) not in data.standard_series
+    ), "processor.delete_range appears to be broken."
+    assert (
+        pd.to_datetime(end_idx) not in data.standard_series
+    ), "processor.delete_range appears to be broken."
+
+    # Insert nans where values are missing
+    data.insert_missing_nans()
+
+    # Check that NaNs are inserted
+    assert pd.isna(
+        data.standard_series[start_idx]
+    ), "processor.insert_missing_nans appears to be broken."
+    assert pd.isna(
+        data.standard_series[end_idx]
+    ), "processor.insert_missing_nans appears to be broken."
+
+    # "Close" gaps (i.e. remove nan rows)
+    data.gap_closer()
+
+    # Check that gap was closed
+    assert (
+        pd.to_datetime(start_idx) not in data.standard_series
+    ), "processor.gap_closer appears to be broken."
+    assert (
+        pd.to_datetime(end_idx) not in data.standard_series
+    ), "processor.gap_closer appears to be broken."
+
+    data.quality_encoder()
+
+    # TODO: Write test for quality_encoder
+
+    data.to_xml_data_structure()
+
+    # TODO: Write test for to_xml_data_structure
+
+    data.data_exporter(tmp_path / "xml_data.xml")
+    data.data_exporter(tmp_path / "csv_data.csv", ftype="csv")
+    data.data_exporter(tmp_path / "hilltop_csv_data.csv", ftype="hilltop_csv")
+
+    # TODO: Write tests for data_exporter
+
+    data.diagnosis()
+
+
+@pytest.mark.slow()
+@pytest.mark.remote()
+def test_empty_response(tmp_path):
+    """
+    Test the handling of an empty server response.
+
+    Parameters
+    ----------
+    tmp_path : pathlib.Path
+        The temporary path for storing log files and exported data.
+
+    Notes
+    -----
+    This test checks the connection to the specified server and various functionalities
+    of the Processor class.
+
+    The test configuration includes parameters such as base_url, file names, site
+    information, date range, and default settings.
+
+    Annalist is configured to log information during the test.
+    Processor is instantiated with the provided processing parameters.
+    Assertions are made to ensure that essential series (standard_series, check_data,
+    check_series, quality_series) are not empty.
+
+    Data clipping, removal of flatlined values and spikes, range deletion, insertion of
+    missing NaNs, gap closure, quality encoding, XML data structure creation, data
+    export, and diagnosis are tested.
+
+    Assertions
+    ----------
+    Various assertions are included throughout the test to verify the expected behavior
+    of Processor methods and properties.
+    These assertions cover the state of data series before and after certain
+    operations, ensuring data integrity and functionality.
+    """
+    processing_parameters = {
+        "base_url": "http://hilltopdev.horizons.govt.nz/",
+        "standard_hts_filename": "RawLogger.hts",
+        "check_hts_filename": "boo.hts",
+        "site": "Whanganui at Te Rewa",
+        "from_date": "2003-01-01 00:00",
+        "to_date": "2003-02-02 23:00",
+        "frequency": "5min",
+        "standard_measurement_name": "Water level statistics: Point Sample",
+        "check_measurement_name": "External S.G. [Water Level NRT]",
+        "defaults": {
+            "high_clip": 5000,
+            "low_clip": 0,
+            "delta": 1000,
+            "span": 10,
+            "gap_limit": 12,
+            "max_qc": 600,
+        },
+    }
+
+    with pytest.warns(UserWarning):
+        ann = Annalist()
+        format_str = format_str = (
+            "%(asctime)s, %(analyst_name)s, %(function_name)s, %(site)s, "
+            "%(measurement)s, %(from_date)s, %(to_date)s, %(message)s"
+        )
+        ann.configure(
+            logfile=tmp_path / "bot_annals.csv",
+            analyst_name="Annie the analyst!",
+            stream_format_str=format_str,
+        )
+
+        data = Processor(
+            processing_parameters["base_url"],
+            processing_parameters["site"],
+            processing_parameters["standard_hts_filename"],
+            processing_parameters["standard_measurement_name"],
+            processing_parameters["frequency"],
+            processing_parameters["from_date"],
+            processing_parameters["to_date"],
+            processing_parameters["check_hts_filename"],
+            processing_parameters["check_measurement_name"],
+            processing_parameters["defaults"],
+        )
+
+        assert data.standard_series.empty
+        assert data.check_series.empty
+        assert data.quality_series.empty
+        assert data.raw_standard_series.empty
+        assert data.raw_standard_blob is None
+        assert data.raw_standard_xml is None
+        assert data.raw_quality_series.empty
+        assert data.raw_quality_blob is None
+        assert data.raw_quality_xml is None
+        assert data.raw_check_data.empty
+        assert data.raw_check_blob is None
+        assert data.raw_check_xml is None
+
+
+@pytest.mark.slow()
+@pytest.mark.remote()
+def test_failed_requests(tmp_path):
+    """
+    Test the handling of an empty server response.
+
+    Parameters
+    ----------
+    tmp_path : pathlib.Path
+        The temporary path for storing log files and exported data.
+
+    Notes
+    -----
+    This test checks the connection to the specified server and various functionalities
+    of the Processor class.
+
+    The test configuration includes parameters such as base_url, file names, site
+    information, date range, and default settings.
+
+    Annalist is configured to log information during the test.
+    Processor is instantiated with the provided processing parameters.
+    Assertions are made to ensure that essential series (standard_series, check_data,
+    check_series, quality_series) are not empty.
+
+    Data clipping, removal of flatlined values and spikes, range deletion, insertion of
+    missing NaNs, gap closure, quality encoding, XML data structure creation, data
+    export, and diagnosis are tested.
+
+    Assertions
+    ----------
+    Various assertions are included throughout the test to verify the expected behavior
+    of Processor methods and properties.
+    These assertions cover the state of data series before and after certain
+    operations, ensuring data integrity and functionality.
+    """
+    processing_parameters = {
+        "base_url": "http://hilltopdev.horizons.govt.nz/",
+        "standard_hts_filename": "RawLogger.hts",
+        "check_hts_filename": "boo.hts",
+        "site": "Whanganui at Te Rewa",
+        "from_date": "2003-01-01 00:00",
+        "to_date": "2003-02-02 23:00",
+        "frequency": "4min",
+        "standard_measurement_name": "Water level statistics: Point Sample",
+        "check_measurement_name": "External S.G. [Water Level NRT]",
+        "defaults": {
+            "high_clip": 5000,
+            "low_clip": 0,
+            "delta": 1000,
+            "span": 10,
+            "gap_limit": 12,
+            "max_qc": 600,
+        },
+    }
+
+    with pytest.warns(UserWarning):
+        ann = Annalist()
+        format_str = format_str = (
+            "%(asctime)s, %(analyst_name)s, %(function_name)s, %(site)s, "
+            "%(measurement)s, %(from_date)s, %(to_date)s, %(message)s"
+        )
+        ann.configure(
+            logfile=tmp_path / "bot_annals.csv",
+            analyst_name="Annie the analyst!",
+            stream_format_str=format_str,
+        )
+
+        # with pytest.raises(
+        #     ValueError
+        # ) as excinfo:
+        #     _ = Processor(
+        #         processing_parameters["base_url"],
+        #         processing_parameters["site"],
+        #         processing_parameters["standard_hts_filename"],
+        #         processing_parameters["standard_measurement_name"],
+        #         processing_parameters["frequency"],
+        #         processing_parameters["from_date"],
+        #         processing_parameters["to_date"],
+        #         processing_parameters["check_hts_filename"],
+        #         processing_parameters["check_measurement_name"],
+        #         processing_parameters["defaults"],
+        #     )
+        # print(excinfo.value)
+
+        with pytest.raises(
+            ValueError, match=r"No sites found for the base_url and hts combo."
+        ) as excinfo:
+            _ = Processor(
+                processing_parameters["base_url"],
+                processing_parameters["site"],
+                "Notarealhstfile",
+                # processing_parameters["standard_hts_filename"],
+                processing_parameters["standard_measurement_name"],
+                processing_parameters["frequency"],
+                processing_parameters["from_date"],
+                processing_parameters["to_date"],
+                processing_parameters["check_hts_filename"],
+                processing_parameters["check_measurement_name"],
+                processing_parameters["defaults"],
+            )
+        assert "No sites found for the base_url and hts combo." in str(excinfo.value)
+
+        with pytest.raises(
+            ValueError, match=r"Site 'Notarealsite' not found .*"
+        ) as excinfo:
+            _ = Processor(
+                processing_parameters["base_url"],
+                "Notarealsite",
+                processing_parameters["standard_hts_filename"],
+                processing_parameters["standard_measurement_name"],
+                processing_parameters["frequency"],
+                processing_parameters["from_date"],
+                processing_parameters["to_date"],
+                processing_parameters["check_hts_filename"],
+                processing_parameters["check_measurement_name"],
+                processing_parameters["defaults"],
+            )
+        assert "Site 'Notarealsite' not found for both base_url and hts combos." in str(
+            excinfo.value
+        )
+
+        with pytest.raises(ValueError, match=r"Standard measurement name.*") as excinfo:
+            _ = Processor(
+                processing_parameters["base_url"],
+                processing_parameters["site"],
+                processing_parameters["standard_hts_filename"],
+                # processing_parameters["standard_measurement_name"],
+                "Notarealmeasurement",
+                processing_parameters["frequency"],
+                processing_parameters["from_date"],
+                processing_parameters["to_date"],
+                processing_parameters["check_hts_filename"],
+                processing_parameters["check_measurement_name"],
+                processing_parameters["defaults"],
+            )
+        assert (
+            "Standard measurement name 'Notarealmeasurement' not found at site"
+            in str(excinfo.value)
+        )
+
+        with pytest.raises(
+            ValueError,
+            match=r"Unrecognised start time",
+        ) as excinfo:
+            _ = Processor(
+                processing_parameters["base_url"],
+                processing_parameters["site"],
+                processing_parameters["standard_hts_filename"],
+                processing_parameters["standard_measurement_name"],
+                processing_parameters["frequency"],
+                # processing_parameters["from_date"],
+                "Notarealdate",
+                processing_parameters["to_date"],
+                processing_parameters["check_hts_filename"],
+                processing_parameters["check_measurement_name"],
+                processing_parameters["defaults"],
+            )
+        assert "Unrecognised start time" in str(excinfo.value)
+
+        # with pytest.raises(
+        #     ValueError  #, match=r"Unrecognised start time",
+        # ) as excinfo:
+        _ = Processor(
+            processing_parameters["base_url"],
+            processing_parameters["site"],
+            processing_parameters["standard_hts_filename"],
+            processing_parameters["standard_measurement_name"],
+            # processing_parameters["frequency"],
+            "Notarealfrequency",
+            processing_parameters["from_date"],
+            processing_parameters["to_date"],
+            processing_parameters["check_hts_filename"],
+            processing_parameters["check_measurement_name"],
+            processing_parameters["defaults"],
+        )
+        print(excinfo)
+        # assert (
+        #     "Unrecognised start time"
+        #     in str(excinfo.value)
+        # )
+
+        with pytest.raises(
+            ValueError, match=r"No sites found for the base_url and hts combo."
+        ) as excinfo:
+            _ = Processor(
+                processing_parameters["base_url"],
+                processing_parameters["site"],
+                processing_parameters["standard_hts_filename"],
+                processing_parameters["standard_measurement_name"],
+                processing_parameters["frequency"],
+                processing_parameters["from_date"],
+                processing_parameters["to_date"],
+                # processing_parameters["check_hts_filename"],
+                "Notarealhtsfilename",
+                processing_parameters["check_measurement_name"],
+                processing_parameters["defaults"],
+            )
+        assert "No sites found for the base_url and hts combo." in str(excinfo.value)
+
+        with pytest.raises(
+            ValueError, match=r"Check measurement name 'Notarealmeasurement' not found "
+        ) as excinfo:
+            _ = Processor(
+                processing_parameters["base_url"],
+                processing_parameters["site"],
+                processing_parameters["standard_hts_filename"],
+                processing_parameters["standard_measurement_name"],
+                processing_parameters["frequency"],
+                processing_parameters["from_date"],
+                processing_parameters["to_date"],
+                processing_parameters["check_hts_filename"],
+                # processing_parameters["check_measurement_name"],
+                "Notarealmeasurement",
+                processing_parameters["defaults"],
+            )
+        print(excinfo)
+        assert "Check measurement name 'Notarealmeasurement' not found at site " in str(
+            excinfo.value
+        )
```

### Comparing `hydrobot-0.5.0/tests/xml_test_data_file.xml` & `hydrobot-0.5.1/tests/xml_test_data_file.xml`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, ASCII text, with very long lines (322)*

 * *Files 24% similar despite different names*

```diff
@@ -1,875 +1,901 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2731  <?xml version='1
 00000010: 2e30 2720 656e 636f 6469 6e67 3d27 7574  .0' encoding='ut
-00000020: 662d 3827 3f3e 0a3c 4869 6c6c 746f 703e  f-8'?>.<Hilltop>
-00000030: 0a20 2020 203c 4167 656e 6379 3e48 6f72  .    <Agency>Hor
-00000040: 697a 6f6e 733c 2f41 6765 6e63 793e 0a20  izons</Agency>. 
-00000050: 2020 203c 4d65 6173 7572 656d 656e 7420     <Measurement 
-00000060: 5369 7465 4e61 6d65 3d22 4d69 6420 5374  SiteName="Mid St
-00000070: 7265 616d 2061 7420 436f 7774 6f69 6c65  ream at Cowtoile
-00000080: 7420 4661 726d 223e 0a20 2020 2020 2020  t Farm">.       
-00000090: 203c 4461 7461 536f 7572 6365 204e 616d   <DataSource Nam
-000000a0: 653d 2247 656e 6572 616c 204e 6173 7469  e="General Nasti
-000000b0: 6e65 7373 2220 4e75 6d49 7465 6d73 3d22  ness" NumItems="
-000000c0: 3122 3e0a 2020 2020 2020 2020 2020 2020  1">.            
-000000d0: 3c54 5354 7970 653e 5374 6453 6572 6965  <TSType>StdSerie
-000000e0: 733c 2f54 5354 7970 653e 0a20 2020 2020  s</TSType>.     
-000000f0: 2020 2020 2020 203c 4461 7461 5479 7065         <DataType
-00000100: 3e53 696d 706c 6554 696d 6553 6572 6965  >SimpleTimeSerie
-00000110: 733c 2f44 6174 6154 7970 653e 0a20 2020  s</DataType>.   
-00000120: 2020 2020 2020 2020 203c 496e 7465 7270           <Interp
-00000130: 6f6c 6174 696f 6e3e 496e 6372 656d 656e  olation>Incremen
-00000140: 7461 6c3c 2f49 6e74 6572 706f 6c61 7469  tal</Interpolati
-00000150: 6f6e 3e0a 2020 2020 2020 2020 2020 2020  on>.            
-00000160: 3c49 7465 6d46 6f72 6d61 743e 303c 2f49  <ItemFormat>0</I
-00000170: 7465 6d46 6f72 6d61 743e 0a20 2020 2020  temFormat>.     
-00000180: 2020 2020 2020 203c 4974 656d 496e 666f         <ItemInfo
-00000190: 2049 7465 6d4e 756d 6265 723d 2231 223e   ItemNumber="1">
-000001a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000001b0: 203c 4974 656d 4e61 6d65 3e47 656e 6572   <ItemName>Gener
-000001c0: 616c 204e 6173 7469 6e65 7373 3c2f 4974  al Nastiness</It
-000001d0: 656d 4e61 6d65 3e0a 2020 2020 2020 2020  emName>.        
-000001e0: 2020 2020 2020 2020 3c49 7465 6d46 6f72          <ItemFor
-000001f0: 6d61 743e 493c 2f49 7465 6d46 6f72 6d61  mat>I</ItemForma
-00000200: 743e 0a20 2020 2020 2020 2020 2020 2020  t>.             
-00000210: 2020 203c 4469 7669 736f 723e 313c 2f44     <Divisor>1</D
-00000220: 6976 6973 6f72 3e0a 2020 2020 2020 2020  ivisor>.        
-00000230: 2020 2020 2020 2020 3c55 6e69 7473 3e6f          <Units>o
-00000240: 7574 206f 6620 3130 3c2f 556e 6974 733e  ut of 10</Units>
-00000250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000260: 203c 466f 726d 6174 3e23 2e23 2323 3c2f   <Format>#.###</
-00000270: 466f 726d 6174 3e0a 2020 2020 2020 2020  Format>.        
-00000280: 2020 2020 3c2f 4974 656d 496e 666f 3e0a      </ItemInfo>.
-00000290: 2020 2020 2020 2020 3c2f 4461 7461 536f          </DataSo
-000002a0: 7572 6365 3e0a 2020 2020 2020 2020 3c44  urce>.        <D
-000002b0: 6174 6120 4461 7465 466f 726d 6174 3d22  ata DateFormat="
-000002c0: 6d6f 7773 6563 7322 204e 756d 4974 656d  mowsecs" NumItem
-000002d0: 733d 2231 223e 0a20 2020 2020 2020 2020  s="1">.         
-000002e0: 2020 203c 453e 0a20 2020 2020 2020 2020     <E>.         
-000002f0: 2020 2020 2020 203c 543e 3236 3139 3330         <T>261930
-00000300: 3234 3030 3c2f 543e 0a20 2020 2020 2020  2400</T>.       
-00000310: 2020 2020 2020 2020 203c 4931 3e31 303c           <I1>10<
-00000320: 2f49 313e 0a20 2020 2020 2020 2020 2020  /I1>.           
-00000330: 203c 2f45 3e0a 2020 2020 2020 2020 2020   </E>.          
-00000340: 2020 3c45 3e0a 2020 2020 2020 2020 2020    <E>.          
-00000350: 2020 2020 2020 3c54 3e32 3631 3933 3032        <T>2619302
-00000360: 3730 303c 2f54 3e0a 2020 2020 2020 2020  700</T>.        
-00000370: 2020 2020 2020 2020 3c49 313e 393c 2f49          <I1>9</I
-00000380: 313e 0a20 2020 2020 2020 2020 2020 203c  1>.            <
-00000390: 2f45 3e0a 2020 2020 2020 2020 2020 2020  /E>.            
-000003a0: 3c45 3e0a 2020 2020 2020 2020 2020 2020  <E>.            
-000003b0: 2020 2020 3c54 3e32 3631 3933 3033 3030      <T>261930300
-000003c0: 303c 2f54 3e0a 2020 2020 2020 2020 2020  0</T>.          
-000003d0: 2020 2020 2020 3c49 313e 383c 2f49 313e        <I1>8</I1>
-000003e0: 0a20 2020 2020 2020 2020 2020 203c 2f45  .            </E
-000003f0: 3e0a 2020 2020 2020 2020 2020 2020 3c45  >.            <E
-00000400: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00000410: 2020 3c54 3e32 3631 3933 3033 3330 303c    <T>2619303300<
-00000420: 2f54 3e0a 2020 2020 2020 2020 2020 2020  /T>.            
-00000430: 2020 2020 3c49 313e 3130 3c2f 4931 3e0a      <I1>10</I1>.
-00000440: 2020 2020 2020 2020 2020 2020 3c2f 453e              </E>
-00000450: 0a20 2020 2020 2020 2020 2020 203c 453e  .            <E>
-00000460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000470: 203c 543e 3236 3139 3330 3336 3030 3c2f   <T>2619303600</
-00000480: 543e 0a20 2020 2020 2020 2020 2020 2020  T>.             
-00000490: 2020 203c 4931 3e31 303c 2f49 313e 0a20     <I1>10</I1>. 
-000004a0: 2020 2020 2020 2020 2020 203c 2f45 3e0a             </E>.
-000004b0: 2020 2020 2020 2020 2020 2020 3c45 3e0a              <E>.
-000004c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000004d0: 3c54 3e32 3631 3933 3033 3930 303c 2f54  <T>2619303900</T
-000004e0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-000004f0: 2020 3c49 313e 393c 2f49 313e 0a20 2020    <I1>9</I1>.   
-00000500: 2020 2020 2020 2020 203c 2f45 3e0a 2020           </E>.  
-00000510: 2020 2020 2020 2020 2020 3c45 3e0a 2020            <E>.  
-00000520: 2020 2020 2020 2020 2020 2020 2020 3c54                <T
-00000530: 3e32 3631 3933 3034 3230 303c 2f54 3e0a  >2619304200</T>.
-00000540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000550: 3c49 313e 3130 3c2f 4931 3e0a 2020 2020  <I1>10</I1>.    
-00000560: 2020 2020 2020 2020 3c2f 453e 0a20 2020          </E>.   
-00000570: 2020 2020 2020 2020 203c 453e 0a20 2020           <E>.   
-00000580: 2020 2020 2020 2020 2020 2020 203c 543e               <T>
-00000590: 3236 3139 3330 3435 3030 3c2f 543e 0a20  2619304500</T>. 
-000005a0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000005b0: 4931 3e36 3c2f 4931 3e0a 2020 2020 2020  I1>6</I1>.      
-000005c0: 2020 2020 2020 3c2f 453e 0a20 2020 2020        </E>.     
-000005d0: 2020 2020 2020 203c 453e 0a20 2020 2020         <E>.     
-000005e0: 2020 2020 2020 2020 2020 203c 543e 3236             <T>26
-000005f0: 3139 3330 3438 3030 3c2f 543e 0a20 2020  19304800</T>.   
-00000600: 2020 2020 2020 2020 2020 2020 203c 4931               <I1
-00000610: 3e31 303c 2f49 313e 0a20 2020 2020 2020  >10</I1>.       
-00000620: 2020 2020 203c 2f45 3e0a 2020 2020 2020       </E>.      
-00000630: 2020 2020 2020 3c45 3e0a 2020 2020 2020        <E>.      
-00000640: 2020 2020 2020 2020 2020 3c54 3e32 3631            <T>261
-00000650: 3933 3035 3130 303c 2f54 3e0a 2020 2020  9305100</T>.    
-00000660: 2020 2020 2020 2020 2020 2020 3c49 313e              <I1>
-00000670: 3130 3c2f 4931 3e0a 2020 2020 2020 2020  10</I1>.        
-00000680: 2020 2020 3c2f 453e 0a20 2020 2020 2020      </E>.       
-00000690: 203c 2f44 6174 613e 0a20 2020 203c 2f4d   </Data>.    </M
-000006a0: 6561 7375 7265 6d65 6e74 3e0a 2020 2020  easurement>.    
-000006b0: 3c4d 6561 7375 7265 6d65 6e74 2053 6974  <Measurement Sit
-000006c0: 654e 616d 653d 224d 6964 2053 7472 6561  eName="Mid Strea
-000006d0: 6d20 6174 2043 6f77 746f 696c 6574 2046  m at Cowtoilet F
-000006e0: 6172 6d22 3e0a 2020 2020 2020 2020 3c44  arm">.        <D
-000006f0: 6174 6153 6f75 7263 6520 4e61 6d65 3d22  ataSource Name="
-00000700: 4765 6e65 7261 6c20 4e61 7374 696e 6573  General Nastines
-00000710: 7322 204e 756d 4974 656d 733d 2231 223e  s" NumItems="1">
-00000720: 0a20 2020 2020 2020 2020 2020 203c 5453  .            <TS
-00000730: 5479 7065 3e53 7464 5175 616c 5365 7269  Type>StdQualSeri
-00000740: 6573 3c2f 5453 5479 7065 3e0a 2020 2020  es</TSType>.    
-00000750: 2020 2020 2020 2020 3c44 6174 6154 7970          <DataTyp
-00000760: 653e 5369 6d70 6c65 5469 6d65 5365 7269  e>SimpleTimeSeri
-00000770: 6573 3c2f 4461 7461 5479 7065 3e0a 2020  es</DataType>.  
-00000780: 2020 2020 2020 2020 2020 3c49 6e74 6572            <Inter
-00000790: 706f 6c61 7469 6f6e 3e45 7665 6e74 3c2f  polation>Event</
-000007a0: 496e 7465 7270 6f6c 6174 696f 6e3e 0a20  Interpolation>. 
-000007b0: 2020 2020 2020 2020 2020 203c 4974 656d             <Item
-000007c0: 466f 726d 6174 3e30 3c2f 4974 656d 466f  Format>0</ItemFo
-000007d0: 726d 6174 3e0a 2020 2020 2020 2020 3c2f  rmat>.        </
-000007e0: 4461 7461 536f 7572 6365 3e0a 2020 2020  DataSource>.    
-000007f0: 2020 2020 3c44 6174 6120 4461 7465 466f      <Data DateFo
-00000800: 726d 6174 3d22 6d6f 7773 6563 7322 204e  rmat="mowsecs" N
-00000810: 756d 4974 656d 733d 2231 223e 0a20 2020  umItems="1">.   
-00000820: 2020 2020 2020 2020 203c 453e 0a20 2020           <E>.   
-00000830: 2020 2020 2020 2020 2020 2020 203c 543e               <T>
-00000840: 3236 3139 3330 3234 3030 3c2f 543e 0a20  2619302400</T>. 
-00000850: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00000860: 4931 3e35 3030 3c2f 4931 3e0a 2020 2020  I1>500</I1>.    
-00000870: 2020 2020 2020 2020 3c2f 453e 0a20 2020          </E>.   
-00000880: 2020 2020 203c 2f44 6174 613e 0a20 2020       </Data>.   
-00000890: 203c 2f4d 6561 7375 7265 6d65 6e74 3e0a   </Measurement>.
-000008a0: 2020 2020 3c4d 6561 7375 7265 6d65 6e74      <Measurement
-000008b0: 2053 6974 654e 616d 653d 224d 6964 2053   SiteName="Mid S
-000008c0: 7472 6561 6d20 6174 2043 6f77 746f 696c  tream at Cowtoil
-000008d0: 6574 2046 6172 6d22 3e0a 2020 2020 2020  et Farm">.      
-000008e0: 2020 3c44 6174 6153 6f75 7263 6520 4e61    <DataSource Na
-000008f0: 6d65 3d22 4765 6e65 7261 6c20 4e61 7374  me="General Nast
-00000900: 696e 6573 7322 204e 756d 4974 656d 733d  iness" NumItems=
-00000910: 2233 223e 0a20 2020 2020 2020 2020 2020  "3">.           
-00000920: 203c 5453 5479 7065 3e43 6865 636b 5365   <TSType>CheckSe
-00000930: 7269 6573 3c2f 5453 5479 7065 3e0a 2020  ries</TSType>.  
-00000940: 2020 2020 2020 2020 2020 3c44 6174 6154            <DataT
-00000950: 7970 653e 5369 6d70 6c65 5469 6d65 5365  ype>SimpleTimeSe
-00000960: 7269 6573 3c2f 4461 7461 5479 7065 3e0a  ries</DataType>.
-00000970: 2020 2020 2020 2020 2020 2020 3c49 6e74              <Int
-00000980: 6572 706f 6c61 7469 6f6e 3e44 6973 6372  erpolation>Discr
-00000990: 6574 653c 2f49 6e74 6572 706f 6c61 7469  ete</Interpolati
-000009a0: 6f6e 3e0a 2020 2020 2020 2020 2020 2020  on>.            
-000009b0: 3c49 7465 6d46 6f72 6d61 743e 3134 303c  <ItemFormat>140<
-000009c0: 2f49 7465 6d46 6f72 6d61 743e 0a20 2020  /ItemFormat>.   
-000009d0: 2020 2020 2020 2020 203c 4974 656d 496e           <ItemIn
-000009e0: 666f 2049 7465 6d4e 756d 6265 723d 2231  fo ItemNumber="1
-000009f0: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-00000a00: 2020 203c 4974 656d 4e61 6d65 3e47 656e     <ItemName>Gen
-00000a10: 6572 616c 204e 6173 7469 6e65 7373 3c2f  eral Nastiness</
-00000a20: 4974 656d 4e61 6d65 3e0a 2020 2020 2020  ItemName>.      
-00000a30: 2020 2020 2020 2020 2020 3c49 7465 6d46            <ItemF
-00000a40: 6f72 6d61 743e 493c 2f49 7465 6d46 6f72  ormat>I</ItemFor
-00000a50: 6d61 743e 0a20 2020 2020 2020 2020 2020  mat>.           
-00000a60: 2020 2020 203c 4469 7669 736f 723e 313c       <Divisor>1<
-00000a70: 2f44 6976 6973 6f72 3e0a 2020 2020 2020  /Divisor>.      
-00000a80: 2020 2020 2020 2020 2020 3c55 6e69 7473            <Units
-00000a90: 3e6f 7574 206f 6620 3130 3c2f 556e 6974  >out of 10</Unit
-00000aa0: 733e 0a20 2020 2020 2020 2020 2020 2020  s>.             
-00000ab0: 2020 203c 466f 726d 6174 3e23 233c 2f46     <Format>##</F
-00000ac0: 6f72 6d61 743e 0a20 2020 2020 2020 2020  ormat>.         
-00000ad0: 2020 203c 2f49 7465 6d49 6e66 6f3e 0a20     </ItemInfo>. 
-00000ae0: 2020 2020 2020 2020 2020 203c 4974 656d             <Item
-00000af0: 496e 666f 2049 7465 6d4e 756d 6265 723d  Info ItemNumber=
-00000b00: 2232 223e 0a20 2020 2020 2020 2020 2020  "2">.           
-00000b10: 2020 2020 203c 4974 656d 4e61 6d65 3e52       <ItemName>R
-00000b20: 6563 6f72 6465 7220 5469 6d65 3c2f 4974  ecorder Time</It
-00000b30: 656d 4e61 6d65 3e0a 2020 2020 2020 2020  emName>.        
-00000b40: 2020 2020 2020 2020 3c49 7465 6d46 6f72          <ItemFor
-00000b50: 6d61 743e 443c 2f49 7465 6d46 6f72 6d61  mat>D</ItemForma
-00000b60: 743e 0a20 2020 2020 2020 2020 2020 2020  t>.             
-00000b70: 2020 203c 4469 7669 736f 723e 313c 2f44     <Divisor>1</D
-00000b80: 6976 6973 6f72 3e0a 2020 2020 2020 2020  ivisor>.        
-00000b90: 2020 2020 2020 2020 3c55 6e69 7473 202f          <Units /
-00000ba0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00000bb0: 2020 3c46 6f72 6d61 743e 2323 233c 2f46    <Format>###</F
-00000bc0: 6f72 6d61 743e 0a20 2020 2020 2020 2020  ormat>.         
-00000bd0: 2020 203c 2f49 7465 6d49 6e66 6f3e 0a20     </ItemInfo>. 
-00000be0: 2020 2020 2020 2020 2020 203c 4974 656d             <Item
-00000bf0: 496e 666f 2049 7465 6d4e 756d 6265 723d  Info ItemNumber=
-00000c00: 2233 223e 0a20 2020 2020 2020 2020 2020  "3">.           
-00000c10: 2020 2020 203c 4974 656d 4e61 6d65 3e43       <ItemName>C
-00000c20: 6f6d 6d65 6e74 3c2f 4974 656d 4e61 6d65  omment</ItemName
-00000c30: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00000c40: 2020 3c49 7465 6d46 6f72 6d61 743e 533c    <ItemFormat>S<
-00000c50: 2f49 7465 6d46 6f72 6d61 743e 0a20 2020  /ItemFormat>.   
-00000c60: 2020 2020 2020 2020 2020 2020 203c 4469               <Di
-00000c70: 7669 736f 723e 313c 2f44 6976 6973 6f72  visor>1</Divisor
-00000c80: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00000c90: 2020 3c55 6e69 7473 202f 3e0a 2020 2020    <Units />.    
-00000ca0: 2020 2020 2020 2020 2020 2020 3c46 6f72              <For
-00000cb0: 6d61 743e 2323 233c 2f46 6f72 6d61 743e  mat>###</Format>
-00000cc0: 0a20 2020 2020 2020 2020 2020 203c 2f49  .            </I
-00000cd0: 7465 6d49 6e66 6f3e 0a20 2020 2020 2020  temInfo>.       
-00000ce0: 203c 2f44 6174 6153 6f75 7263 653e 0a20   </DataSource>. 
-00000cf0: 2020 2020 2020 203c 4461 7461 2044 6174         <Data Dat
-00000d00: 6546 6f72 6d61 743d 226d 6f77 7365 6373  eFormat="mowsecs
-00000d10: 2220 4e75 6d49 7465 6d73 3d22 3322 3e0a  " NumItems="3">.
-00000d20: 2020 2020 2020 2020 2020 2020 3c45 3e0a              <E>.
-00000d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d40: 3c54 3e32 3631 3933 3032 3430 303c 2f54  <T>2619302400</T
-00000d50: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00000d60: 2020 3c49 313e 393c 2f49 313e 0a20 2020    <I1>9</I1>.   
-00000d70: 2020 2020 2020 2020 2020 2020 203c 4932               <I2
-00000d80: 3e32 3631 3933 3032 3430 303c 2f49 323e  >2619302400</I2>
-00000d90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000da0: 203c 4933 3e0a 2020 2020 2020 2020 2020   <I3>.          
-00000db0: 2020 2020 2020 2020 2020 5369 7465 2068            Site h
-00000dc0: 6173 2062 6565 6e20 7265 706c 6163 6564  as been replaced
-00000dd0: 2062 7920 6120 6461 6972 7920 7365 6c6c   by a dairy sell
-00000de0: 696e 6720 7265 616c 6c79 2067 6f6f 6420  ing really good 
-00000df0: 7265 616c 2066 7275 6974 2069 6365 2063  real fruit ice c
-00000e00: 7265 616d 2e0a 2020 2020 2020 2020 2020  ream..          
-00000e10: 2020 2020 2020 3c2f 4933 3e0a 2020 2020        </I3>.    
-00000e20: 2020 2020 2020 2020 3c2f 453e 0a20 2020          </E>.   
-00000e30: 2020 2020 2020 2020 203c 453e 0a20 2020           <E>.   
-00000e40: 2020 2020 2020 2020 2020 2020 203c 543e               <T>
-00000e50: 3236 3139 3330 3330 3030 3c2f 543e 0a20  2619303000</T>. 
-00000e60: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00000e70: 4931 3e38 3c2f 4931 3e0a 2020 2020 2020  I1>8</I1>.      
-00000e80: 2020 2020 2020 2020 2020 3c49 323e 3236            <I2>26
-00000e90: 3139 3330 3330 3030 3c2f 4932 3e0a 2020  19303000</I2>.  
-00000ea0: 2020 2020 2020 2020 2020 2020 2020 3c49                <I
-00000eb0: 333e 0a20 2020 2020 2020 2020 2020 2020  3>.             
-00000ec0: 2020 2020 2020 2057 6173 2063 6861 7365         Was chase
-00000ed0: 6420 6672 6f6d 2073 6974 6520 6279 2066  d from site by f
-00000ee0: 7572 696f 7573 2070 6561 636f 636b 2e0a  urious peacock..
-00000ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f00: 3c2f 4933 3e0a 2020 2020 2020 2020 2020  </I3>.          
-00000f10: 2020 3c2f 453e 0a20 2020 2020 2020 2020    </E>.         
-00000f20: 2020 203c 453e 0a20 2020 2020 2020 2020     <E>.         
-00000f30: 2020 2020 2020 203c 543e 3236 3139 3330         <T>261930
-00000f40: 3339 3030 3c2f 543e 0a20 2020 2020 2020  3900</T>.       
-00000f50: 2020 2020 2020 2020 203c 4931 3e37 3c2f           <I1>7</
-00000f60: 4931 3e0a 2020 2020 2020 2020 2020 2020  I1>.            
-00000f70: 2020 2020 3c49 323e 3236 3139 3330 3339      <I2>26193039
-00000f80: 3030 3c2f 4932 3e0a 2020 2020 2020 2020  00</I2>.        
-00000f90: 2020 2020 2020 2020 3c49 333e 5574 6520          <I3>Ute 
-00000fa0: 7374 6f6c 656e 2e20 5761 6c6b 696e 6720  stolen. Walking 
-00000fb0: 6261 636b 2074 6f20 7265 6769 6f6e 616c  back to regional
-00000fc0: 2068 6f75 7365 2e3c 2f49 333e 0a20 2020   house.</I3>.   
-00000fd0: 2020 2020 2020 2020 203c 2f45 3e0a 2020           </E>.  
-00000fe0: 2020 2020 2020 2020 2020 3c45 3e0a 2020            <E>.  
-00000ff0: 2020 2020 2020 2020 2020 2020 2020 3c54                <T
-00001000: 3e32 3631 3933 3035 3130 303c 2f54 3e0a  >2619305100</T>.
-00001010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001020: 3c49 313e 3130 3c2f 4931 3e0a 2020 2020  <I1>10</I1>.    
-00001030: 2020 2020 2020 2020 2020 2020 3c49 323e              <I2>
-00001040: 3236 3139 3330 3531 3030 3c2f 4932 3e0a  2619305100</I2>.
-00001050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001060: 3c49 333e 0a20 2020 2020 2020 2020 2020  <I3>.           
-00001070: 2020 2020 2020 2020 2043 616e 2774 2065           Can't e
-00001080: 7665 6e20 6265 6769 6e20 746f 2064 6573  ven begin to des
-00001090: 6372 6962 6520 7468 6520 6361 726e 6167  cribe the carnag
-000010a0: 6520 4920 6861 7665 2077 6974 6e65 7373  e I have witness
-000010b0: 6564 2e20 4920 6361 6e20 7374 696c 6c20  ed. I can still 
-000010c0: 6865 6172 2074 6865 2073 6372 6561 6d73  hear the screams
-000010d0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000010e0: 2020 3c2f 4933 3e0a 2020 2020 2020 2020    </I3>.        
-000010f0: 2020 2020 3c2f 453e 0a20 2020 2020 2020      </E>.       
-00001100: 203c 2f44 6174 613e 0a20 2020 203c 2f4d   </Data>.    </M
-00001110: 6561 7375 7265 6d65 6e74 3e0a 2020 2020  easurement>.    
-00001120: 3c4d 6561 7375 7265 6d65 6e74 2053 6974  <Measurement Sit
-00001130: 654e 616d 653d 224d 6964 2053 7472 6561  eName="Mid Strea
-00001140: 6d20 6174 2043 6f77 746f 696c 6574 2046  m at Cowtoilet F
-00001150: 6172 6d22 3e0a 2020 2020 2020 2020 3c44  arm">.        <D
-00001160: 6174 6153 6f75 7263 6520 4e61 6d65 3d22  ataSource Name="
-00001170: 4e75 6d62 6572 206f 6620 4163 7475 616c  Number of Actual
-00001180: 2057 686f 6c65 2048 756d 616e 2054 7572   Whole Human Tur
-00001190: 6473 2046 6c6f 6174 696e 6720 4279 2220  ds Floating By" 
-000011a0: 4e75 6d49 7465 6d73 3d22 3122 3e0a 2020  NumItems="1">.  
-000011b0: 2020 2020 2020 2020 2020 3c54 5354 7970            <TSTyp
-000011c0: 653e 5374 6453 6572 6965 733c 2f54 5354  e>StdSeries</TST
-000011d0: 7970 653e 0a20 2020 2020 2020 2020 2020  ype>.           
-000011e0: 203c 4461 7461 5479 7065 3e54 7572 6473   <DataType>Turds
-000011f0: 2070 6572 2053 6563 6f6e 643c 2f44 6174   per Second</Dat
-00001200: 6154 7970 653e 0a20 2020 2020 2020 2020  aType>.         
-00001210: 2020 203c 496e 7465 7270 6f6c 6174 696f     <Interpolatio
-00001220: 6e3e 496e 6372 656d 656e 7461 6c3c 2f49  n>Incremental</I
-00001230: 6e74 6572 706f 6c61 7469 6f6e 3e0a 2020  nterpolation>.  
-00001240: 2020 2020 2020 2020 2020 3c49 7465 6d46            <ItemF
-00001250: 6f72 6d61 743e 303c 2f49 7465 6d46 6f72  ormat>0</ItemFor
-00001260: 6d61 743e 0a20 2020 2020 2020 2020 2020  mat>.           
-00001270: 203c 4974 656d 496e 666f 2049 7465 6d4e   <ItemInfo ItemN
-00001280: 756d 6265 723d 2231 223e 0a20 2020 2020  umber="1">.     
-00001290: 2020 2020 2020 2020 2020 203c 4974 656d             <Item
-000012a0: 4e61 6d65 3e4e 756d 6265 7220 6f66 2041  Name>Number of A
-000012b0: 6374 7561 6c20 5768 6f6c 6520 4875 6d61  ctual Whole Huma
-000012c0: 6e20 5475 7264 7320 466c 6f61 7469 6e67  n Turds Floating
-000012d0: 2042 793c 2f49 7465 6d4e 616d 653e 0a20   By</ItemName>. 
-000012e0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000012f0: 4974 656d 466f 726d 6174 3e46 3c2f 4974  ItemFormat>F</It
-00001300: 656d 466f 726d 6174 3e0a 2020 2020 2020  emFormat>.      
-00001310: 2020 2020 2020 2020 2020 3c44 6976 6973            <Divis
-00001320: 6f72 3e31 3c2f 4469 7669 736f 723e 0a20  or>1</Divisor>. 
-00001330: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00001340: 556e 6974 733e 742f 733c 2f55 6e69 7473  Units>t/s</Units
-00001350: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00001360: 2020 3c46 6f72 6d61 743e 2323 2323 2e23    <Format>####.#
-00001370: 3c2f 466f 726d 6174 3e0a 2020 2020 2020  </Format>.      
-00001380: 2020 2020 2020 3c2f 4974 656d 496e 666f        </ItemInfo
-00001390: 3e0a 2020 2020 2020 2020 3c2f 4461 7461  >.        </Data
-000013a0: 536f 7572 6365 3e0a 2020 2020 2020 2020  Source>.        
-000013b0: 3c44 6174 6120 4461 7465 466f 726d 6174  <Data DateFormat
-000013c0: 3d22 6d6f 7773 6563 7322 204e 756d 4974  ="mowsecs" NumIt
-000013d0: 656d 733d 2231 223e 0a20 2020 2020 2020  ems="1">.       
-000013e0: 2020 2020 203c 453e 0a20 2020 2020 2020       <E>.       
-000013f0: 2020 2020 2020 2020 203c 543e 3236 3139           <T>2619
-00001400: 3330 3234 3030 3c2f 543e 0a20 2020 2020  302400</T>.     
-00001410: 2020 2020 2020 2020 2020 203c 4931 3e31             <I1>1
-00001420: 3734 2e33 3c2f 4931 3e0a 2020 2020 2020  74.3</I1>.      
-00001430: 2020 2020 2020 3c2f 453e 0a20 2020 2020        </E>.     
-00001440: 2020 2020 2020 203c 453e 0a20 2020 2020         <E>.     
-00001450: 2020 2020 2020 2020 2020 203c 543e 3236             <T>26
-00001460: 3139 3330 3237 3030 3c2f 543e 0a20 2020  19302700</T>.   
-00001470: 2020 2020 2020 2020 2020 2020 203c 4931               <I1
-00001480: 3e37 2e34 3c2f 4931 3e0a 2020 2020 2020  >7.4</I1>.      
-00001490: 2020 2020 2020 3c2f 453e 0a20 2020 2020        </E>.     
-000014a0: 2020 2020 2020 203c 453e 0a20 2020 2020         <E>.     
-000014b0: 2020 2020 2020 2020 2020 203c 543e 3236             <T>26
-000014c0: 3139 3330 3330 3030 3c2f 543e 0a20 2020  19303000</T>.   
-000014d0: 2020 2020 2020 2020 2020 2020 203c 4931               <I1
-000014e0: 3e31 3838 322e 313c 2f49 313e 0a20 2020  >1882.1</I1>.   
-000014f0: 2020 2020 2020 2020 203c 2f45 3e0a 2020           </E>.  
-00001500: 2020 2020 2020 2020 2020 3c45 3e0a 2020            <E>.  
-00001510: 2020 2020 2020 2020 2020 2020 2020 3c54                <T
-00001520: 3e32 3631 3933 3033 3330 303c 2f54 3e0a  >2619303300</T>.
-00001530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001540: 3c49 313e 3132 2e34 3c2f 4931 3e0a 2020  <I1>12.4</I1>.  
-00001550: 2020 2020 2020 2020 2020 3c2f 453e 0a20            </E>. 
-00001560: 2020 2020 2020 2020 2020 203c 453e 0a20             <E>. 
-00001570: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00001580: 543e 3236 3139 3330 3336 3030 3c2f 543e  T>2619303600</T>
-00001590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000015a0: 203c 4931 3e31 3034 2e30 3c2f 4931 3e0a   <I1>104.0</I1>.
-000015b0: 2020 2020 2020 2020 2020 2020 3c2f 453e              </E>
-000015c0: 0a20 2020 2020 2020 2020 2020 203c 453e  .            <E>
-000015d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000015e0: 203c 543e 3236 3139 3330 3339 3030 3c2f   <T>2619303900</
-000015f0: 543e 0a20 2020 2020 2020 2020 2020 2020  T>.             
-00001600: 2020 203c 4931 3e31 3134 352e 303c 2f49     <I1>1145.0</I
-00001610: 313e 0a20 2020 2020 2020 2020 2020 203c  1>.            <
-00001620: 2f45 3e0a 2020 2020 2020 2020 2020 2020  /E>.            
-00001630: 3c45 3e0a 2020 2020 2020 2020 2020 2020  <E>.            
-00001640: 2020 2020 3c54 3e32 3631 3933 3034 3230      <T>261930420
-00001650: 303c 2f54 3e0a 2020 2020 2020 2020 2020  0</T>.          
-00001660: 2020 2020 2020 3c49 313e 3632 3334 2e36        <I1>6234.6
-00001670: 3c2f 4931 3e0a 2020 2020 2020 2020 2020  </I1>.          
-00001680: 2020 3c2f 453e 0a20 2020 2020 2020 2020    </E>.         
-00001690: 2020 203c 453e 0a20 2020 2020 2020 2020     <E>.         
-000016a0: 2020 2020 2020 203c 543e 3236 3139 3330         <T>261930
-000016b0: 3435 3030 3c2f 543e 0a20 2020 2020 2020  4500</T>.       
-000016c0: 2020 2020 2020 2020 203c 4931 3e36 2e31           <I1>6.1
-000016d0: 3c2f 4931 3e0a 2020 2020 2020 2020 2020  </I1>.          
-000016e0: 2020 3c2f 453e 0a20 2020 2020 2020 2020    </E>.         
-000016f0: 2020 203c 453e 0a20 2020 2020 2020 2020     <E>.         
-00001700: 2020 2020 2020 203c 543e 3236 3139 3330         <T>261930
-00001710: 3438 3030 3c2f 543e 0a20 2020 2020 2020  4800</T>.       
-00001720: 2020 2020 2020 2020 203c 4931 3e39 3939           <I1>999
-00001730: 312e 303c 2f49 313e 0a20 2020 2020 2020  1.0</I1>.       
-00001740: 2020 2020 203c 2f45 3e0a 2020 2020 2020       </E>.      
-00001750: 2020 2020 2020 3c45 3e0a 2020 2020 2020        <E>.      
-00001760: 2020 2020 2020 2020 2020 3c54 3e32 3631            <T>261
-00001770: 3933 3035 3130 303c 2f54 3e0a 2020 2020  9305100</T>.    
-00001780: 2020 2020 2020 2020 2020 2020 3c49 313e              <I1>
-00001790: 342e 303c 2f49 313e 0a20 2020 2020 2020  4.0</I1>.       
-000017a0: 2020 2020 203c 2f45 3e0a 2020 2020 2020       </E>.      
-000017b0: 2020 3c2f 4461 7461 3e0a 2020 2020 3c2f    </Data>.    </
-000017c0: 4d65 6173 7572 656d 656e 743e 0a20 2020  Measurement>.   
-000017d0: 203c 4d65 6173 7572 656d 656e 7420 5369   <Measurement Si
-000017e0: 7465 4e61 6d65 3d22 4d69 6420 5374 7265  teName="Mid Stre
-000017f0: 616d 2061 7420 436f 7774 6f69 6c65 7420  am at Cowtoilet 
-00001800: 4661 726d 223e 0a20 2020 2020 2020 203c  Farm">.        <
-00001810: 4461 7461 536f 7572 6365 204e 616d 653d  DataSource Name=
-00001820: 224e 756d 6265 7220 6f66 2041 6374 7561  "Number of Actua
-00001830: 6c20 5768 6f6c 6520 4875 6d61 6e20 5475  l Whole Human Tu
-00001840: 7264 7320 466c 6f61 7469 6e67 2042 7922  rds Floating By"
-00001850: 204e 756d 4974 656d 733d 2231 223e 0a20   NumItems="1">. 
-00001860: 2020 2020 2020 2020 2020 203c 5453 5479             <TSTy
-00001870: 7065 3e53 7464 5175 616c 5365 7269 6573  pe>StdQualSeries
-00001880: 3c2f 5453 5479 7065 3e0a 2020 2020 2020  </TSType>.      
-00001890: 2020 2020 2020 3c44 6174 6154 7970 653e        <DataType>
-000018a0: 5475 7264 7320 7065 7220 5365 636f 6e64  Turds per Second
-000018b0: 3c2f 4461 7461 5479 7065 3e0a 2020 2020  </DataType>.    
-000018c0: 2020 2020 2020 2020 3c49 6e74 6572 706f          <Interpo
-000018d0: 6c61 7469 6f6e 3e45 7665 6e74 3c2f 496e  lation>Event</In
-000018e0: 7465 7270 6f6c 6174 696f 6e3e 0a20 2020  terpolation>.   
-000018f0: 2020 2020 2020 2020 203c 4974 656d 466f           <ItemFo
-00001900: 726d 6174 3e30 3c2f 4974 656d 466f 726d  rmat>0</ItemForm
-00001910: 6174 3e0a 2020 2020 2020 2020 3c2f 4461  at>.        </Da
-00001920: 7461 536f 7572 6365 3e0a 2020 2020 2020  taSource>.      
-00001930: 2020 3c44 6174 6120 4461 7465 466f 726d    <Data DateForm
-00001940: 6174 3d22 6d6f 7773 6563 7322 204e 756d  at="mowsecs" Num
-00001950: 4974 656d 733d 2231 223e 0a20 2020 2020  Items="1">.     
-00001960: 2020 2020 2020 203c 453e 0a20 2020 2020         <E>.     
-00001970: 2020 2020 2020 2020 2020 203c 543e 3236             <T>26
-00001980: 3139 3330 3234 3030 3c2f 543e 0a20 2020  19302400</T>.   
-00001990: 2020 2020 2020 2020 2020 2020 203c 4931               <I1
-000019a0: 3e32 3030 3c2f 4931 3e0a 2020 2020 2020  >200</I1>.      
-000019b0: 2020 2020 2020 3c2f 453e 0a20 2020 2020        </E>.     
-000019c0: 2020 203c 2f44 6174 613e 0a20 2020 203c     </Data>.    <
-000019d0: 2f4d 6561 7375 7265 6d65 6e74 3e0a 2020  /Measurement>.  
-000019e0: 2020 3c4d 6561 7375 7265 6d65 6e74 2053    <Measurement S
-000019f0: 6974 654e 616d 653d 224d 6964 2053 7472  iteName="Mid Str
-00001a00: 6561 6d20 6174 2043 6f77 746f 696c 6574  eam at Cowtoilet
-00001a10: 2046 6172 6d22 3e0a 2020 2020 2020 2020   Farm">.        
-00001a20: 3c44 6174 6153 6f75 7263 6520 4e61 6d65  <DataSource Name
-00001a30: 3d22 4e75 6d62 6572 206f 6620 4163 7475  ="Number of Actu
-00001a40: 616c 2057 686f 6c65 2048 756d 616e 2054  al Whole Human T
-00001a50: 7572 6473 2046 6c6f 6174 696e 6720 4279  urds Floating By
-00001a60: 2220 4e75 6d49 7465 6d73 3d22 3422 3e0a  " NumItems="4">.
-00001a70: 2020 2020 2020 2020 2020 2020 3c54 5354              <TST
-00001a80: 7970 653e 4368 6563 6b53 6572 6965 733c  ype>CheckSeries<
-00001a90: 2f54 5354 7970 653e 0a20 2020 2020 2020  /TSType>.       
-00001aa0: 2020 2020 203c 4461 7461 5479 7065 3e54       <DataType>T
-00001ab0: 7572 6473 2070 6572 2053 6563 6f6e 643c  urds per Second<
-00001ac0: 2f44 6174 6154 7970 653e 0a20 2020 2020  /DataType>.     
-00001ad0: 2020 2020 2020 203c 496e 7465 7270 6f6c         <Interpol
-00001ae0: 6174 696f 6e3e 4469 7363 7265 7465 3c2f  ation>Discrete</
-00001af0: 496e 7465 7270 6f6c 6174 696f 6e3e 0a20  Interpolation>. 
-00001b00: 2020 2020 2020 2020 2020 203c 4974 656d             <Item
-00001b10: 466f 726d 6174 3e31 3430 3c2f 4974 656d  Format>140</Item
-00001b20: 466f 726d 6174 3e0a 2020 2020 2020 2020  Format>.        
-00001b30: 2020 2020 3c49 7465 6d49 6e66 6f20 4974      <ItemInfo It
-00001b40: 656d 4e75 6d62 6572 3d22 3122 3e0a 2020  emNumber="1">.  
-00001b50: 2020 2020 2020 2020 2020 2020 2020 3c49                <I
-00001b60: 7465 6d4e 616d 653e 5475 7264 6964 6974  temName>Turdidit
-00001b70: 7920 5365 6e73 6f72 2052 6561 6469 6e67  y Sensor Reading
-00001b80: 3c2f 4974 656d 4e61 6d65 3e0a 2020 2020  </ItemName>.    
-00001b90: 2020 2020 2020 2020 2020 2020 3c49 7465              <Ite
-00001ba0: 6d46 6f72 6d61 743e 463c 2f49 7465 6d46  mFormat>F</ItemF
-00001bb0: 6f72 6d61 743e 0a20 2020 2020 2020 2020  ormat>.         
-00001bc0: 2020 2020 2020 203c 4469 7669 736f 723e         <Divisor>
-00001bd0: 313c 2f44 6976 6973 6f72 3e0a 2020 2020  1</Divisor>.    
-00001be0: 2020 2020 2020 2020 2020 2020 3c55 6e69              <Uni
-00001bf0: 7473 3e74 2f73 3c2f 556e 6974 733e 0a20  ts>t/s</Units>. 
-00001c00: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00001c10: 466f 726d 6174 3e23 2323 232e 233c 2f46  Format>####.#</F
-00001c20: 6f72 6d61 743e 0a20 2020 2020 2020 2020  ormat>.         
-00001c30: 2020 203c 2f49 7465 6d49 6e66 6f3e 0a20     </ItemInfo>. 
-00001c40: 2020 2020 2020 2020 2020 203c 4974 656d             <Item
-00001c50: 496e 666f 2049 7465 6d4e 756d 6265 723d  Info ItemNumber=
-00001c60: 2232 223e 0a20 2020 2020 2020 2020 2020  "2">.           
-00001c70: 2020 2020 203c 4974 656d 4e61 6d65 3e52       <ItemName>R
-00001c80: 6563 6f72 6465 7220 5469 6d65 3c2f 4974  ecorder Time</It
-00001c90: 656d 4e61 6d65 3e0a 2020 2020 2020 2020  emName>.        
-00001ca0: 2020 2020 2020 2020 3c49 7465 6d46 6f72          <ItemFor
-00001cb0: 6d61 743e 443c 2f49 7465 6d46 6f72 6d61  mat>D</ItemForma
-00001cc0: 743e 0a20 2020 2020 2020 2020 2020 2020  t>.             
-00001cd0: 2020 203c 4469 7669 736f 723e 303c 2f44     <Divisor>0</D
-00001ce0: 6976 6973 6f72 3e0a 2020 2020 2020 2020  ivisor>.        
-00001cf0: 2020 2020 2020 2020 3c55 6e69 7473 202f          <Units /
-00001d00: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00001d10: 2020 3c46 6f72 6d61 743e 2323 233c 2f46    <Format>###</F
-00001d20: 6f72 6d61 743e 0a20 2020 2020 2020 2020  ormat>.         
-00001d30: 2020 203c 2f49 7465 6d49 6e66 6f3e 0a20     </ItemInfo>. 
-00001d40: 2020 2020 2020 2020 2020 203c 4974 656d             <Item
-00001d50: 496e 666f 2049 7465 6d4e 756d 6265 723d  Info ItemNumber=
-00001d60: 2233 223e 0a20 2020 2020 2020 2020 2020  "3">.           
-00001d70: 2020 2020 203c 4974 656d 4e61 6d65 3e48       <ItemName>H
-00001d80: 616e 6468 656c 6420 5475 7264 6964 6974  andheld Turdidit
-00001d90: 7920 5365 6e73 6f72 2052 6561 6469 6e67  y Sensor Reading
-00001da0: 3c2f 4974 656d 4e61 6d65 3e0a 2020 2020  </ItemName>.    
-00001db0: 2020 2020 2020 2020 2020 2020 3c49 7465              <Ite
-00001dc0: 6d46 6f72 6d61 743e 463c 2f49 7465 6d46  mFormat>F</ItemF
-00001dd0: 6f72 6d61 743e 0a20 2020 2020 2020 2020  ormat>.         
-00001de0: 2020 2020 2020 203c 4469 7669 736f 723e         <Divisor>
-00001df0: 313c 2f44 6976 6973 6f72 3e0a 2020 2020  1</Divisor>.    
-00001e00: 2020 2020 2020 2020 2020 2020 3c55 6e69              <Uni
-00001e10: 7473 202f 3e0a 2020 2020 2020 2020 2020  ts />.          
-00001e20: 2020 2020 2020 3c46 6f72 6d61 743e 2323        <Format>##
-00001e30: 232e 233c 2f46 6f72 6d61 743e 0a20 2020  #.#</Format>.   
-00001e40: 2020 2020 2020 2020 203c 2f49 7465 6d49           </ItemI
-00001e50: 6e66 6f3e 0a20 2020 2020 2020 2020 2020  nfo>.           
-00001e60: 203c 4974 656d 496e 666f 2049 7465 6d4e   <ItemInfo ItemN
-00001e70: 756d 6265 723d 2234 223e 0a20 2020 2020  umber="4">.     
-00001e80: 2020 2020 2020 2020 2020 203c 4974 656d             <Item
-00001e90: 4e61 6d65 3e43 6f6d 6d65 6e74 3c2f 4974  Name>Comment</It
-00001ea0: 656d 4e61 6d65 3e0a 2020 2020 2020 2020  emName>.        
-00001eb0: 2020 2020 2020 2020 3c49 7465 6d46 6f72          <ItemFor
-00001ec0: 6d61 743e 533c 2f49 7465 6d46 6f72 6d61  mat>S</ItemForma
-00001ed0: 743e 0a20 2020 2020 2020 2020 2020 2020  t>.             
-00001ee0: 2020 203c 4469 7669 736f 723e 313c 2f44     <Divisor>1</D
-00001ef0: 6976 6973 6f72 3e0a 2020 2020 2020 2020  ivisor>.        
-00001f00: 2020 2020 2020 2020 3c55 6e69 7473 202f          <Units /
-00001f10: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00001f20: 2020 3c46 6f72 6d61 743e 2323 233c 2f46    <Format>###</F
-00001f30: 6f72 6d61 743e 0a20 2020 2020 2020 2020  ormat>.         
-00001f40: 2020 203c 2f49 7465 6d49 6e66 6f3e 0a20     </ItemInfo>. 
-00001f50: 2020 2020 2020 203c 2f44 6174 6153 6f75         </DataSou
-00001f60: 7263 653e 0a20 2020 2020 2020 203c 4461  rce>.        <Da
-00001f70: 7461 2044 6174 6546 6f72 6d61 743d 226d  ta DateFormat="m
-00001f80: 6f77 7365 6373 2220 4e75 6d49 7465 6d73  owsecs" NumItems
-00001f90: 3d22 3422 3e0a 2020 2020 2020 2020 2020  ="4">.          
-00001fa0: 2020 3c45 3e0a 2020 2020 2020 2020 2020    <E>.          
-00001fb0: 2020 2020 2020 3c54 3e32 3631 3933 3032        <T>2619302
-00001fc0: 3430 303c 2f54 3e0a 2020 2020 2020 2020  400</T>.        
-00001fd0: 2020 2020 2020 2020 3c49 313e 3132 2e34          <I1>12.4
-00001fe0: 3c2f 4931 3e0a 2020 2020 2020 2020 2020  </I1>.          
-00001ff0: 2020 2020 2020 3c49 323e 3236 3139 3330        <I2>261930
-00002000: 3234 3030 3c2f 4932 3e0a 2020 2020 2020  2400</I2>.      
-00002010: 2020 2020 2020 2020 2020 3c49 333e 3132            <I3>12
-00002020: 3435 2e32 3c2f 4933 3e0a 2020 2020 2020  45.2</I3>.      
-00002030: 2020 2020 2020 2020 2020 3c49 343e 0a20            <I4>. 
-00002040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002050: 2020 2053 7475 6d62 6c65 6420 7570 6f6e     Stumbled upon
-00002060: 2061 206e 7564 6973 7420 636f 6c6f 6e79   a nudist colony
-00002070: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002080: 2020 3c2f 4934 3e0a 2020 2020 2020 2020    </I4>.        
-00002090: 2020 2020 3c2f 453e 0a20 2020 2020 2020      </E>.       
-000020a0: 2020 2020 203c 453e 0a20 2020 2020 2020       <E>.       
-000020b0: 2020 2020 2020 2020 203c 543e 3236 3139           <T>2619
-000020c0: 3330 3330 3030 3c2f 543e 0a20 2020 2020  303000</T>.     
-000020d0: 2020 2020 2020 2020 2020 203c 4931 3e31             <I1>1
-000020e0: 3435 312e 323c 2f49 313e 0a20 2020 2020  451.2</I1>.     
-000020f0: 2020 2020 2020 2020 2020 203c 4932 3e32             <I2>2
-00002100: 3631 3933 3033 3030 303c 2f49 323e 0a20  619303000</I2>. 
-00002110: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00002120: 4933 3e31 3233 342e 353c 2f49 333e 0a20  I3>1234.5</I3>. 
-00002130: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00002140: 4934 3e0a 2020 2020 2020 2020 2020 2020  I4>.            
-00002150: 2020 2020 2020 2020 4672 6965 6e64 6c79          Friendly
-00002160: 2063 6f77 2e20 506f 7373 6962 6c79 2061   cow. Possibly a
-00002170: 2073 7079 2e0a 2020 2020 2020 2020 2020   spy..          
-00002180: 2020 2020 2020 3c2f 4934 3e0a 2020 2020        </I4>.    
-00002190: 2020 2020 2020 2020 3c2f 453e 0a20 2020          </E>.   
-000021a0: 2020 2020 2020 2020 203c 453e 0a20 2020           <E>.   
-000021b0: 2020 2020 2020 2020 2020 2020 203c 543e               <T>
-000021c0: 3236 3139 3330 3432 3030 3c2f 543e 0a20  2619304200</T>. 
-000021d0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000021e0: 4931 3e32 3436 362e 323c 2f49 313e 0a20  I1>2466.2</I1>. 
-000021f0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00002200: 4932 3e32 3631 3933 3034 3230 303c 2f49  I2>2619304200</I
-00002210: 323e 0a20 2020 2020 2020 2020 2020 2020  2>.             
-00002220: 2020 203c 4933 3e38 3937 302e 393c 2f49     <I3>8970.9</I
-00002230: 333e 0a20 2020 2020 2020 2020 2020 2020  3>.             
-00002240: 2020 203c 4934 3e48 6164 2061 2063 6f6c     <I4>Had a col
-00002250: 6420 7368 6976 6572 2072 756e 2064 6f77  d shiver run dow
-00002260: 6e20 6d79 2073 7069 6e65 2e20 5368 6f75  n my spine. Shou
-00002270: 6c64 206e 6f74 2068 6176 6520 636f 6d65  ld not have come
-00002280: 2068 6572 6520 6174 2033 616d 2e3c 2f49   here at 3am.</I
-00002290: 343e 0a20 2020 2020 2020 2020 2020 203c  4>.            <
-000022a0: 2f45 3e0a 2020 2020 2020 2020 2020 2020  /E>.            
-000022b0: 3c45 3e0a 2020 2020 2020 2020 2020 2020  <E>.            
-000022c0: 2020 2020 3c54 3e32 3631 3933 3035 3130      <T>261930510
-000022d0: 303c 2f54 3e0a 2020 2020 2020 2020 2020  0</T>.          
-000022e0: 2020 2020 2020 3c49 313e 3739 3030 2e30        <I1>7900.0
-000022f0: 3c2f 4931 3e0a 2020 2020 2020 2020 2020  </I1>.          
+00000020: 662d 3827 3f3e 0d0a 3c48 696c 6c74 6f70  f-8'?>..<Hilltop
+00000030: 3e0d 0a20 2020 203c 4167 656e 6379 3e48  >..    <Agency>H
+00000040: 6f72 697a 6f6e 733c 2f41 6765 6e63 793e  orizons</Agency>
+00000050: 0d0a 2020 2020 3c4d 6561 7375 7265 6d65  ..    <Measureme
+00000060: 6e74 2053 6974 654e 616d 653d 224d 6964  nt SiteName="Mid
+00000070: 2053 7472 6561 6d20 6174 2043 6f77 746f   Stream at Cowto
+00000080: 696c 6574 2046 6172 6d22 3e0d 0a20 2020  ilet Farm">..   
+00000090: 2020 2020 203c 4461 7461 536f 7572 6365       <DataSource
+000000a0: 204e 616d 653d 2247 656e 6572 616c 204e   Name="General N
+000000b0: 6173 7469 6e65 7373 2220 4e75 6d49 7465  astiness" NumIte
+000000c0: 6d73 3d22 3122 3e0d 0a20 2020 2020 2020  ms="1">..       
+000000d0: 2020 2020 203c 5453 5479 7065 3e53 7464       <TSType>Std
+000000e0: 5365 7269 6573 3c2f 5453 5479 7065 3e0d  Series</TSType>.
+000000f0: 0a20 2020 2020 2020 2020 2020 203c 4461  .            <Da
+00000100: 7461 5479 7065 3e53 696d 706c 6554 696d  taType>SimpleTim
+00000110: 6553 6572 6965 733c 2f44 6174 6154 7970  eSeries</DataTyp
+00000120: 653e 0d0a 2020 2020 2020 2020 2020 2020  e>..            
+00000130: 3c49 6e74 6572 706f 6c61 7469 6f6e 3e49  <Interpolation>I
+00000140: 6e63 7265 6d65 6e74 616c 3c2f 496e 7465  ncremental</Inte
+00000150: 7270 6f6c 6174 696f 6e3e 0d0a 2020 2020  rpolation>..    
+00000160: 2020 2020 2020 2020 3c49 7465 6d46 6f72          <ItemFor
+00000170: 6d61 743e 303c 2f49 7465 6d46 6f72 6d61  mat>0</ItemForma
+00000180: 743e 0d0a 2020 2020 2020 2020 2020 2020  t>..            
+00000190: 3c49 7465 6d49 6e66 6f20 4974 656d 4e75  <ItemInfo ItemNu
+000001a0: 6d62 6572 3d22 3122 3e0d 0a20 2020 2020  mber="1">..     
+000001b0: 2020 2020 2020 2020 2020 203c 4974 656d             <Item
+000001c0: 4e61 6d65 3e47 656e 6572 616c 204e 6173  Name>General Nas
+000001d0: 7469 6e65 7373 3c2f 4974 656d 4e61 6d65  tiness</ItemName
+000001e0: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
+000001f0: 2020 203c 4974 656d 466f 726d 6174 3e49     <ItemFormat>I
+00000200: 3c2f 4974 656d 466f 726d 6174 3e0d 0a20  </ItemFormat>.. 
+00000210: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00000220: 4469 7669 736f 723e 313c 2f44 6976 6973  Divisor>1</Divis
+00000230: 6f72 3e0d 0a20 2020 2020 2020 2020 2020  or>..           
+00000240: 2020 2020 203c 556e 6974 733e 6f75 7420       <Units>out 
+00000250: 6f66 2031 303c 2f55 6e69 7473 3e0d 0a20  of 10</Units>.. 
+00000260: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00000270: 466f 726d 6174 3e23 2e23 2323 3c2f 466f  Format>#.###</Fo
+00000280: 726d 6174 3e0d 0a20 2020 2020 2020 2020  rmat>..         
+00000290: 2020 203c 2f49 7465 6d49 6e66 6f3e 0d0a     </ItemInfo>..
+000002a0: 2020 2020 2020 2020 3c2f 4461 7461 536f          </DataSo
+000002b0: 7572 6365 3e0d 0a20 2020 2020 2020 203c  urce>..        <
+000002c0: 4461 7461 2044 6174 6546 6f72 6d61 743d  Data DateFormat=
+000002d0: 226d 6f77 7365 6373 2220 4e75 6d49 7465  "mowsecs" NumIte
+000002e0: 6d73 3d22 3122 3e0d 0a20 2020 2020 2020  ms="1">..       
+000002f0: 2020 2020 203c 453e 0d0a 2020 2020 2020       <E>..      
+00000300: 2020 2020 2020 2020 2020 3c54 3e32 3631            <T>261
+00000310: 3933 3032 3430 303c 2f54 3e0d 0a20 2020  9302400</T>..   
+00000320: 2020 2020 2020 2020 2020 2020 203c 4931               <I1
+00000330: 3e31 303c 2f49 313e 0d0a 2020 2020 2020  >10</I1>..      
+00000340: 2020 2020 2020 3c2f 453e 0d0a 2020 2020        </E>..    
+00000350: 2020 2020 2020 2020 3c45 3e0d 0a20 2020          <E>..   
+00000360: 2020 2020 2020 2020 2020 2020 203c 543e               <T>
+00000370: 3236 3139 3330 3237 3030 3c2f 543e 0d0a  2619302700</T>..
+00000380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000390: 3c49 313e 393c 2f49 313e 0d0a 2020 2020  <I1>9</I1>..    
+000003a0: 2020 2020 2020 2020 3c2f 453e 0d0a 2020          </E>..  
+000003b0: 2020 2020 2020 2020 2020 3c45 3e0d 0a20            <E>.. 
+000003c0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+000003d0: 543e 3236 3139 3330 3330 3030 3c2f 543e  T>2619303000</T>
+000003e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000003f0: 2020 3c49 313e 383c 2f49 313e 0d0a 2020    <I1>8</I1>..  
+00000400: 2020 2020 2020 2020 2020 3c2f 453e 0d0a            </E>..
+00000410: 2020 2020 2020 2020 2020 2020 3c45 3e0d              <E>.
+00000420: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000430: 203c 543e 3236 3139 3330 3333 3030 3c2f   <T>2619303300</
+00000440: 543e 0d0a 2020 2020 2020 2020 2020 2020  T>..            
+00000450: 2020 2020 3c49 313e 3130 3c2f 4931 3e0d      <I1>10</I1>.
+00000460: 0a20 2020 2020 2020 2020 2020 203c 2f45  .            </E
+00000470: 3e0d 0a20 2020 2020 2020 2020 2020 203c  >..            <
+00000480: 453e 0d0a 2020 2020 2020 2020 2020 2020  E>..            
+00000490: 2020 2020 3c54 3e32 3631 3933 3033 3630      <T>261930360
+000004a0: 303c 2f54 3e0d 0a20 2020 2020 2020 2020  0</T>..         
+000004b0: 2020 2020 2020 203c 4931 3e31 303c 2f49         <I1>10</I
+000004c0: 313e 0d0a 2020 2020 2020 2020 2020 2020  1>..            
+000004d0: 3c2f 453e 0d0a 2020 2020 2020 2020 2020  </E>..          
+000004e0: 2020 3c45 3e0d 0a20 2020 2020 2020 2020    <E>..         
+000004f0: 2020 2020 2020 203c 543e 3236 3139 3330         <T>261930
+00000500: 3339 3030 3c2f 543e 0d0a 2020 2020 2020  3900</T>..      
+00000510: 2020 2020 2020 2020 2020 3c49 313e 393c            <I1>9<
+00000520: 2f49 313e 0d0a 2020 2020 2020 2020 2020  /I1>..          
+00000530: 2020 3c2f 453e 0d0a 2020 2020 2020 2020    </E>..        
+00000540: 2020 2020 3c45 3e0d 0a20 2020 2020 2020      <E>..       
+00000550: 2020 2020 2020 2020 203c 543e 3236 3139           <T>2619
+00000560: 3330 3432 3030 3c2f 543e 0d0a 2020 2020  304200</T>..    
+00000570: 2020 2020 2020 2020 2020 2020 3c49 313e              <I1>
+00000580: 3130 3c2f 4931 3e0d 0a20 2020 2020 2020  10</I1>..       
+00000590: 2020 2020 203c 2f45 3e0d 0a20 2020 2020       </E>..     
+000005a0: 2020 2020 2020 203c 453e 0d0a 2020 2020         <E>..    
+000005b0: 2020 2020 2020 2020 2020 2020 3c54 3e32              <T>2
+000005c0: 3631 3933 3034 3530 303c 2f54 3e0d 0a20  619304500</T>.. 
+000005d0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+000005e0: 4931 3e36 3c2f 4931 3e0d 0a20 2020 2020  I1>6</I1>..     
+000005f0: 2020 2020 2020 203c 2f45 3e0d 0a20 2020         </E>..   
+00000600: 2020 2020 2020 2020 203c 453e 0d0a 2020           <E>..  
+00000610: 2020 2020 2020 2020 2020 2020 2020 3c54                <T
+00000620: 3e32 3631 3933 3034 3830 303c 2f54 3e0d  >2619304800</T>.
+00000630: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000640: 203c 4931 3e31 303c 2f49 313e 0d0a 2020   <I1>10</I1>..  
+00000650: 2020 2020 2020 2020 2020 3c2f 453e 0d0a            </E>..
+00000660: 2020 2020 2020 2020 2020 2020 3c45 3e0d              <E>.
+00000670: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000680: 203c 543e 3236 3139 3330 3531 3030 3c2f   <T>2619305100</
+00000690: 543e 0d0a 2020 2020 2020 2020 2020 2020  T>..            
+000006a0: 2020 2020 3c49 313e 3130 3c2f 4931 3e0d      <I1>10</I1>.
+000006b0: 0a20 2020 2020 2020 2020 2020 203c 2f45  .            </E
+000006c0: 3e0d 0a20 2020 2020 2020 203c 2f44 6174  >..        </Dat
+000006d0: 613e 0d0a 2020 2020 3c2f 4d65 6173 7572  a>..    </Measur
+000006e0: 656d 656e 743e 0d0a 2020 2020 3c4d 6561  ement>..    <Mea
+000006f0: 7375 7265 6d65 6e74 2053 6974 654e 616d  surement SiteNam
+00000700: 653d 224d 6964 2053 7472 6561 6d20 6174  e="Mid Stream at
+00000710: 2043 6f77 746f 696c 6574 2046 6172 6d22   Cowtoilet Farm"
+00000720: 3e0d 0a20 2020 2020 2020 203c 4461 7461  >..        <Data
+00000730: 536f 7572 6365 204e 616d 653d 2247 656e  Source Name="Gen
+00000740: 6572 616c 204e 6173 7469 6e65 7373 2220  eral Nastiness" 
+00000750: 4e75 6d49 7465 6d73 3d22 3122 3e0d 0a20  NumItems="1">.. 
+00000760: 2020 2020 2020 2020 2020 203c 5453 5479             <TSTy
+00000770: 7065 3e53 7464 5175 616c 5365 7269 6573  pe>StdQualSeries
+00000780: 3c2f 5453 5479 7065 3e0d 0a20 2020 2020  </TSType>..     
+00000790: 2020 2020 2020 203c 4461 7461 5479 7065         <DataType
+000007a0: 3e53 696d 706c 6554 696d 6553 6572 6965  >SimpleTimeSerie
+000007b0: 733c 2f44 6174 6154 7970 653e 0d0a 2020  s</DataType>..  
+000007c0: 2020 2020 2020 2020 2020 3c49 6e74 6572            <Inter
+000007d0: 706f 6c61 7469 6f6e 3e45 7665 6e74 3c2f  polation>Event</
+000007e0: 496e 7465 7270 6f6c 6174 696f 6e3e 0d0a  Interpolation>..
+000007f0: 2020 2020 2020 2020 2020 2020 3c49 7465              <Ite
+00000800: 6d46 6f72 6d61 743e 303c 2f49 7465 6d46  mFormat>0</ItemF
+00000810: 6f72 6d61 743e 0d0a 2020 2020 2020 2020  ormat>..        
+00000820: 3c2f 4461 7461 536f 7572 6365 3e0d 0a20  </DataSource>.. 
+00000830: 2020 2020 2020 203c 4461 7461 2044 6174         <Data Dat
+00000840: 6546 6f72 6d61 743d 226d 6f77 7365 6373  eFormat="mowsecs
+00000850: 2220 4e75 6d49 7465 6d73 3d22 3122 3e0d  " NumItems="1">.
+00000860: 0a20 2020 2020 2020 2020 2020 203c 453e  .            <E>
+00000870: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000880: 2020 3c54 3e32 3631 3933 3032 3430 303c    <T>2619302400<
+00000890: 2f54 3e0d 0a20 2020 2020 2020 2020 2020  /T>..           
+000008a0: 2020 2020 203c 4931 3e35 3030 3c2f 4931       <I1>500</I1
+000008b0: 3e0d 0a20 2020 2020 2020 2020 2020 203c  >..            <
+000008c0: 2f45 3e0d 0a20 2020 2020 2020 203c 2f44  /E>..        </D
+000008d0: 6174 613e 0d0a 2020 2020 3c2f 4d65 6173  ata>..    </Meas
+000008e0: 7572 656d 656e 743e 0d0a 2020 2020 3c4d  urement>..    <M
+000008f0: 6561 7375 7265 6d65 6e74 2053 6974 654e  easurement SiteN
+00000900: 616d 653d 224d 6964 2053 7472 6561 6d20  ame="Mid Stream 
+00000910: 6174 2043 6f77 746f 696c 6574 2046 6172  at Cowtoilet Far
+00000920: 6d22 3e0d 0a20 2020 2020 2020 203c 4461  m">..        <Da
+00000930: 7461 536f 7572 6365 204e 616d 653d 2247  taSource Name="G
+00000940: 656e 6572 616c 204e 6173 7469 6e65 7373  eneral Nastiness
+00000950: 2220 4e75 6d49 7465 6d73 3d22 3322 3e0d  " NumItems="3">.
+00000960: 0a20 2020 2020 2020 2020 2020 203c 5453  .            <TS
+00000970: 5479 7065 3e43 6865 636b 5365 7269 6573  Type>CheckSeries
+00000980: 3c2f 5453 5479 7065 3e0d 0a20 2020 2020  </TSType>..     
+00000990: 2020 2020 2020 203c 4461 7461 5479 7065         <DataType
+000009a0: 3e53 696d 706c 6554 696d 6553 6572 6965  >SimpleTimeSerie
+000009b0: 733c 2f44 6174 6154 7970 653e 0d0a 2020  s</DataType>..  
+000009c0: 2020 2020 2020 2020 2020 3c49 6e74 6572            <Inter
+000009d0: 706f 6c61 7469 6f6e 3e44 6973 6372 6574  polation>Discret
+000009e0: 653c 2f49 6e74 6572 706f 6c61 7469 6f6e  e</Interpolation
+000009f0: 3e0d 0a20 2020 2020 2020 2020 2020 203c  >..            <
+00000a00: 4974 656d 466f 726d 6174 3e31 3430 3c2f  ItemFormat>140</
+00000a10: 4974 656d 466f 726d 6174 3e0d 0a20 2020  ItemFormat>..   
+00000a20: 2020 2020 2020 2020 203c 4974 656d 496e           <ItemIn
+00000a30: 666f 2049 7465 6d4e 756d 6265 723d 2231  fo ItemNumber="1
+00000a40: 223e 0d0a 2020 2020 2020 2020 2020 2020  ">..            
+00000a50: 2020 2020 3c49 7465 6d4e 616d 653e 4765      <ItemName>Ge
+00000a60: 6e65 7261 6c20 4e61 7374 696e 6573 733c  neral Nastiness<
+00000a70: 2f49 7465 6d4e 616d 653e 0d0a 2020 2020  /ItemName>..    
+00000a80: 2020 2020 2020 2020 2020 2020 3c49 7465              <Ite
+00000a90: 6d46 6f72 6d61 743e 493c 2f49 7465 6d46  mFormat>I</ItemF
+00000aa0: 6f72 6d61 743e 0d0a 2020 2020 2020 2020  ormat>..        
+00000ab0: 2020 2020 2020 2020 3c44 6976 6973 6f72          <Divisor
+00000ac0: 3e31 3c2f 4469 7669 736f 723e 0d0a 2020  >1</Divisor>..  
+00000ad0: 2020 2020 2020 2020 2020 2020 2020 3c55                <U
+00000ae0: 6e69 7473 3e6f 7574 206f 6620 3130 3c2f  nits>out of 10</
+00000af0: 556e 6974 733e 0d0a 2020 2020 2020 2020  Units>..        
+00000b00: 2020 2020 2020 2020 3c46 6f72 6d61 743e          <Format>
+00000b10: 2323 3c2f 466f 726d 6174 3e0d 0a20 2020  ##</Format>..   
+00000b20: 2020 2020 2020 2020 203c 2f49 7465 6d49           </ItemI
+00000b30: 6e66 6f3e 0d0a 2020 2020 2020 2020 2020  nfo>..          
+00000b40: 2020 3c49 7465 6d49 6e66 6f20 4974 656d    <ItemInfo Item
+00000b50: 4e75 6d62 6572 3d22 3222 3e0d 0a20 2020  Number="2">..   
+00000b60: 2020 2020 2020 2020 2020 2020 203c 4974               <It
+00000b70: 656d 4e61 6d65 3e52 6563 6f72 6465 7220  emName>Recorder 
+00000b80: 5469 6d65 3c2f 4974 656d 4e61 6d65 3e0d  Time</ItemName>.
+00000b90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000ba0: 203c 4974 656d 466f 726d 6174 3e44 3c2f   <ItemFormat>D</
+00000bb0: 4974 656d 466f 726d 6174 3e0d 0a20 2020  ItemFormat>..   
+00000bc0: 2020 2020 2020 2020 2020 2020 203c 4469               <Di
+00000bd0: 7669 736f 723e 313c 2f44 6976 6973 6f72  visor>1</Divisor
+00000be0: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
+00000bf0: 2020 203c 556e 6974 7320 2f3e 0d0a 2020     <Units />..  
+00000c00: 2020 2020 2020 2020 2020 2020 2020 3c46                <F
+00000c10: 6f72 6d61 743e 2323 233c 2f46 6f72 6d61  ormat>###</Forma
+00000c20: 743e 0d0a 2020 2020 2020 2020 2020 2020  t>..            
+00000c30: 3c2f 4974 656d 496e 666f 3e0d 0a20 2020  </ItemInfo>..   
+00000c40: 2020 2020 2020 2020 203c 4974 656d 496e           <ItemIn
+00000c50: 666f 2049 7465 6d4e 756d 6265 723d 2233  fo ItemNumber="3
+00000c60: 223e 0d0a 2020 2020 2020 2020 2020 2020  ">..            
+00000c70: 2020 2020 3c49 7465 6d4e 616d 653e 436f      <ItemName>Co
+00000c80: 6d6d 656e 743c 2f49 7465 6d4e 616d 653e  mment</ItemName>
+00000c90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000ca0: 2020 3c49 7465 6d46 6f72 6d61 743e 533c    <ItemFormat>S<
+00000cb0: 2f49 7465 6d46 6f72 6d61 743e 0d0a 2020  /ItemFormat>..  
+00000cc0: 2020 2020 2020 2020 2020 2020 2020 3c44                <D
+00000cd0: 6976 6973 6f72 3e31 3c2f 4469 7669 736f  ivisor>1</Diviso
+00000ce0: 723e 0d0a 2020 2020 2020 2020 2020 2020  r>..            
+00000cf0: 2020 2020 3c55 6e69 7473 202f 3e0d 0a20      <Units />.. 
+00000d00: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00000d10: 466f 726d 6174 3e23 2323 3c2f 466f 726d  Format>###</Form
+00000d20: 6174 3e0d 0a20 2020 2020 2020 2020 2020  at>..           
+00000d30: 203c 2f49 7465 6d49 6e66 6f3e 0d0a 2020   </ItemInfo>..  
+00000d40: 2020 2020 2020 3c2f 4461 7461 536f 7572        </DataSour
+00000d50: 6365 3e0d 0a20 2020 2020 2020 203c 4461  ce>..        <Da
+00000d60: 7461 2044 6174 6546 6f72 6d61 743d 226d  ta DateFormat="m
+00000d70: 6f77 7365 6373 2220 4e75 6d49 7465 6d73  owsecs" NumItems
+00000d80: 3d22 3322 3e0d 0a20 2020 2020 2020 2020  ="3">..         
+00000d90: 2020 203c 453e 0d0a 2020 2020 2020 2020     <E>..        
+00000da0: 2020 2020 2020 2020 3c54 3e32 3631 3933          <T>26193
+00000db0: 3032 3430 303c 2f54 3e0d 0a20 2020 2020  02400</T>..     
+00000dc0: 2020 2020 2020 2020 2020 203c 4931 3e39             <I1>9
+00000dd0: 3c2f 4931 3e0d 0a20 2020 2020 2020 2020  </I1>..         
+00000de0: 2020 2020 2020 203c 4932 3e32 3631 3933         <I2>26193
+00000df0: 3032 3430 303c 2f49 323e 0d0a 2020 2020  02400</I2>..    
+00000e00: 2020 2020 2020 2020 2020 2020 3c49 333e              <I3>
+00000e10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000e20: 2020 2020 2020 5369 7465 2068 6173 2062        Site has b
+00000e30: 6565 6e20 7265 706c 6163 6564 2062 7920  een replaced by 
+00000e40: 6120 6461 6972 7920 7365 6c6c 696e 6720  a dairy selling 
+00000e50: 7265 616c 6c79 2067 6f6f 6420 7265 616c  really good real
+00000e60: 2066 7275 6974 2069 6365 2063 7265 616d   fruit ice cream
+00000e70: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00000e80: 2020 203c 2f49 333e 0d0a 2020 2020 2020     </I3>..      
+00000e90: 2020 2020 2020 3c2f 453e 0d0a 2020 2020        </E>..    
+00000ea0: 2020 2020 2020 2020 3c45 3e0d 0a20 2020          <E>..   
+00000eb0: 2020 2020 2020 2020 2020 2020 203c 543e               <T>
+00000ec0: 3236 3139 3330 3330 3030 3c2f 543e 0d0a  2619303000</T>..
+00000ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ee0: 3c49 313e 383c 2f49 313e 0d0a 2020 2020  <I1>8</I1>..    
+00000ef0: 2020 2020 2020 2020 2020 2020 3c49 323e              <I2>
+00000f00: 3236 3139 3330 3330 3030 3c2f 4932 3e0d  2619303000</I2>.
+00000f10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000f20: 203c 4933 3e0d 0a20 2020 2020 2020 2020   <I3>..         
+00000f30: 2020 2020 2020 2020 2020 2057 6173 2063             Was c
+00000f40: 6861 7365 6420 6672 6f6d 2073 6974 6520  hased from site 
+00000f50: 6279 2066 7572 696f 7573 2070 6561 636f  by furious peaco
+00000f60: 636b 2e0d 0a20 2020 2020 2020 2020 2020  ck...           
+00000f70: 2020 2020 203c 2f49 333e 0d0a 2020 2020       </I3>..    
+00000f80: 2020 2020 2020 2020 3c2f 453e 0d0a 2020          </E>..  
+00000f90: 2020 2020 2020 2020 2020 3c45 3e0d 0a20            <E>.. 
+00000fa0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00000fb0: 543e 3236 3139 3330 3339 3030 3c2f 543e  T>2619303900</T>
+00000fc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000fd0: 2020 3c49 313e 373c 2f49 313e 0d0a 2020    <I1>7</I1>..  
+00000fe0: 2020 2020 2020 2020 2020 2020 2020 3c49                <I
+00000ff0: 323e 3236 3139 3330 3339 3030 3c2f 4932  2>2619303900</I2
+00001000: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
+00001010: 2020 203c 4933 3e55 7465 2073 746f 6c65     <I3>Ute stole
+00001020: 6e2e 2057 616c 6b69 6e67 2062 6163 6b20  n. Walking back 
+00001030: 746f 2072 6567 696f 6e61 6c20 686f 7573  to regional hous
+00001040: 652e 3c2f 4933 3e0d 0a20 2020 2020 2020  e.</I3>..       
+00001050: 2020 2020 203c 2f45 3e0d 0a20 2020 2020       </E>..     
+00001060: 2020 2020 2020 203c 453e 0d0a 2020 2020         <E>..    
+00001070: 2020 2020 2020 2020 2020 2020 3c54 3e32              <T>2
+00001080: 3631 3933 3035 3130 303c 2f54 3e0d 0a20  619305100</T>.. 
+00001090: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+000010a0: 4931 3e31 303c 2f49 313e 0d0a 2020 2020  I1>10</I1>..    
+000010b0: 2020 2020 2020 2020 2020 2020 3c49 323e              <I2>
+000010c0: 3236 3139 3330 3531 3030 3c2f 4932 3e0d  2619305100</I2>.
+000010d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000010e0: 203c 4933 3e0d 0a20 2020 2020 2020 2020   <I3>..         
+000010f0: 2020 2020 2020 2020 2020 2043 616e 2774             Can't
+00001100: 2065 7665 6e20 6265 6769 6e20 746f 2064   even begin to d
+00001110: 6573 6372 6962 6520 7468 6520 6361 726e  escribe the carn
+00001120: 6167 6520 4920 6861 7665 2077 6974 6e65  age I have witne
+00001130: 7373 6564 2e20 4920 6361 6e20 7374 696c  ssed. I can stil
+00001140: 6c20 6865 6172 2074 6865 2073 6372 6561  l hear the screa
+00001150: 6d73 2e0d 0a20 2020 2020 2020 2020 2020  ms...           
+00001160: 2020 2020 203c 2f49 333e 0d0a 2020 2020       </I3>..    
+00001170: 2020 2020 2020 2020 3c2f 453e 0d0a 2020          </E>..  
+00001180: 2020 2020 2020 3c2f 4461 7461 3e0d 0a20        </Data>.. 
+00001190: 2020 203c 2f4d 6561 7375 7265 6d65 6e74     </Measurement
+000011a0: 3e0d 0a20 2020 203c 4d65 6173 7572 656d  >..    <Measurem
+000011b0: 656e 7420 5369 7465 4e61 6d65 3d22 4d69  ent SiteName="Mi
+000011c0: 6420 5374 7265 616d 2061 7420 436f 7774  d Stream at Cowt
+000011d0: 6f69 6c65 7420 4661 726d 223e 0d0a 2020  oilet Farm">..  
+000011e0: 2020 2020 2020 3c44 6174 6153 6f75 7263        <DataSourc
+000011f0: 6520 4e61 6d65 3d22 4e75 6d62 6572 206f  e Name="Number o
+00001200: 6620 4163 7475 616c 2057 686f 6c65 2048  f Actual Whole H
+00001210: 756d 616e 2054 7572 6473 2046 6c6f 6174  uman Turds Float
+00001220: 696e 6720 4279 2220 4e75 6d49 7465 6d73  ing By" NumItems
+00001230: 3d22 3122 3e0d 0a20 2020 2020 2020 2020  ="1">..         
+00001240: 2020 203c 5453 5479 7065 3e53 7464 5365     <TSType>StdSe
+00001250: 7269 6573 3c2f 5453 5479 7065 3e0d 0a20  ries</TSType>.. 
+00001260: 2020 2020 2020 2020 2020 203c 4461 7461             <Data
+00001270: 5479 7065 3e54 7572 6473 2070 6572 2053  Type>Turds per S
+00001280: 6563 6f6e 643c 2f44 6174 6154 7970 653e  econd</DataType>
+00001290: 0d0a 2020 2020 2020 2020 2020 2020 3c49  ..            <I
+000012a0: 6e74 6572 706f 6c61 7469 6f6e 3e49 6e63  nterpolation>Inc
+000012b0: 7265 6d65 6e74 616c 3c2f 496e 7465 7270  remental</Interp
+000012c0: 6f6c 6174 696f 6e3e 0d0a 2020 2020 2020  olation>..      
+000012d0: 2020 2020 2020 3c49 7465 6d46 6f72 6d61        <ItemForma
+000012e0: 743e 303c 2f49 7465 6d46 6f72 6d61 743e  t>0</ItemFormat>
+000012f0: 0d0a 2020 2020 2020 2020 2020 2020 3c49  ..            <I
+00001300: 7465 6d49 6e66 6f20 4974 656d 4e75 6d62  temInfo ItemNumb
+00001310: 6572 3d22 3122 3e0d 0a20 2020 2020 2020  er="1">..       
+00001320: 2020 2020 2020 2020 203c 4974 656d 4e61           <ItemNa
+00001330: 6d65 3e4e 756d 6265 7220 6f66 2041 6374  me>Number of Act
+00001340: 7561 6c20 5768 6f6c 6520 4875 6d61 6e20  ual Whole Human 
+00001350: 5475 7264 7320 466c 6f61 7469 6e67 2042  Turds Floating B
+00001360: 793c 2f49 7465 6d4e 616d 653e 0d0a 2020  y</ItemName>..  
+00001370: 2020 2020 2020 2020 2020 2020 2020 3c49                <I
+00001380: 7465 6d46 6f72 6d61 743e 463c 2f49 7465  temFormat>F</Ite
+00001390: 6d46 6f72 6d61 743e 0d0a 2020 2020 2020  mFormat>..      
+000013a0: 2020 2020 2020 2020 2020 3c44 6976 6973            <Divis
+000013b0: 6f72 3e31 3c2f 4469 7669 736f 723e 0d0a  or>1</Divisor>..
+000013c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000013d0: 3c55 6e69 7473 3e74 2f73 3c2f 556e 6974  <Units>t/s</Unit
+000013e0: 733e 0d0a 2020 2020 2020 2020 2020 2020  s>..            
+000013f0: 2020 2020 3c46 6f72 6d61 743e 2323 2323      <Format>####
+00001400: 2e23 3c2f 466f 726d 6174 3e0d 0a20 2020  .#</Format>..   
+00001410: 2020 2020 2020 2020 203c 2f49 7465 6d49           </ItemI
+00001420: 6e66 6f3e 0d0a 2020 2020 2020 2020 3c2f  nfo>..        </
+00001430: 4461 7461 536f 7572 6365 3e0d 0a20 2020  DataSource>..   
+00001440: 2020 2020 203c 4461 7461 2044 6174 6546       <Data DateF
+00001450: 6f72 6d61 743d 226d 6f77 7365 6373 2220  ormat="mowsecs" 
+00001460: 4e75 6d49 7465 6d73 3d22 3122 3e0d 0a20  NumItems="1">.. 
+00001470: 2020 2020 2020 2020 2020 203c 453e 0d0a             <E>..
+00001480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001490: 3c54 3e32 3631 3933 3032 3430 303c 2f54  <T>2619302400</T
+000014a0: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
+000014b0: 2020 203c 4931 3e31 3734 2e33 3c2f 4931     <I1>174.3</I1
+000014c0: 3e0d 0a20 2020 2020 2020 2020 2020 203c  >..            <
+000014d0: 2f45 3e0d 0a20 2020 2020 2020 2020 2020  /E>..           
+000014e0: 203c 453e 0d0a 2020 2020 2020 2020 2020   <E>..          
+000014f0: 2020 2020 2020 3c54 3e32 3631 3933 3032        <T>2619302
+00001500: 3730 303c 2f54 3e0d 0a20 2020 2020 2020  700</T>..       
+00001510: 2020 2020 2020 2020 203c 4931 3e37 2e34           <I1>7.4
+00001520: 3c2f 4931 3e0d 0a20 2020 2020 2020 2020  </I1>..         
+00001530: 2020 203c 2f45 3e0d 0a20 2020 2020 2020     </E>..       
+00001540: 2020 2020 203c 453e 0d0a 2020 2020 2020       <E>..      
+00001550: 2020 2020 2020 2020 2020 3c54 3e32 3631            <T>261
+00001560: 3933 3033 3030 303c 2f54 3e0d 0a20 2020  9303000</T>..   
+00001570: 2020 2020 2020 2020 2020 2020 203c 4931               <I1
+00001580: 3e31 3838 322e 313c 2f49 313e 0d0a 2020  >1882.1</I1>..  
+00001590: 2020 2020 2020 2020 2020 3c2f 453e 0d0a            </E>..
+000015a0: 2020 2020 2020 2020 2020 2020 3c45 3e0d              <E>.
+000015b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000015c0: 203c 543e 3236 3139 3330 3333 3030 3c2f   <T>2619303300</
+000015d0: 543e 0d0a 2020 2020 2020 2020 2020 2020  T>..            
+000015e0: 2020 2020 3c49 313e 3132 2e34 3c2f 4931      <I1>12.4</I1
+000015f0: 3e0d 0a20 2020 2020 2020 2020 2020 203c  >..            <
+00001600: 2f45 3e0d 0a20 2020 2020 2020 2020 2020  /E>..           
+00001610: 203c 453e 0d0a 2020 2020 2020 2020 2020   <E>..          
+00001620: 2020 2020 2020 3c54 3e32 3631 3933 3033        <T>2619303
+00001630: 3630 303c 2f54 3e0d 0a20 2020 2020 2020  600</T>..       
+00001640: 2020 2020 2020 2020 203c 4931 3e31 3034           <I1>104
+00001650: 2e30 3c2f 4931 3e0d 0a20 2020 2020 2020  .0</I1>..       
+00001660: 2020 2020 203c 2f45 3e0d 0a20 2020 2020       </E>..     
+00001670: 2020 2020 2020 203c 453e 0d0a 2020 2020         <E>..    
+00001680: 2020 2020 2020 2020 2020 2020 3c54 3e32              <T>2
+00001690: 3631 3933 3033 3930 303c 2f54 3e0d 0a20  619303900</T>.. 
+000016a0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+000016b0: 4931 3e31 3134 352e 303c 2f49 313e 0d0a  I1>1145.0</I1>..
+000016c0: 2020 2020 2020 2020 2020 2020 3c2f 453e              </E>
+000016d0: 0d0a 2020 2020 2020 2020 2020 2020 3c45  ..            <E
+000016e0: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
+000016f0: 2020 203c 543e 3236 3139 3330 3432 3030     <T>2619304200
+00001700: 3c2f 543e 0d0a 2020 2020 2020 2020 2020  </T>..          
+00001710: 2020 2020 2020 3c49 313e 3632 3334 2e36        <I1>6234.6
+00001720: 3c2f 4931 3e0d 0a20 2020 2020 2020 2020  </I1>..         
+00001730: 2020 203c 2f45 3e0d 0a20 2020 2020 2020     </E>..       
+00001740: 2020 2020 203c 453e 0d0a 2020 2020 2020       <E>..      
+00001750: 2020 2020 2020 2020 2020 3c54 3e32 3631            <T>261
+00001760: 3933 3034 3530 303c 2f54 3e0d 0a20 2020  9304500</T>..   
+00001770: 2020 2020 2020 2020 2020 2020 203c 4931               <I1
+00001780: 3e36 2e31 3c2f 4931 3e0d 0a20 2020 2020  >6.1</I1>..     
+00001790: 2020 2020 2020 203c 2f45 3e0d 0a20 2020         </E>..   
+000017a0: 2020 2020 2020 2020 203c 453e 0d0a 2020           <E>..  
+000017b0: 2020 2020 2020 2020 2020 2020 2020 3c54                <T
+000017c0: 3e32 3631 3933 3034 3830 303c 2f54 3e0d  >2619304800</T>.
+000017d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000017e0: 203c 4931 3e39 3939 312e 303c 2f49 313e   <I1>9991.0</I1>
+000017f0: 0d0a 2020 2020 2020 2020 2020 2020 3c2f  ..            </
+00001800: 453e 0d0a 2020 2020 2020 2020 2020 2020  E>..            
+00001810: 3c45 3e0d 0a20 2020 2020 2020 2020 2020  <E>..           
+00001820: 2020 2020 203c 543e 3236 3139 3330 3531       <T>26193051
+00001830: 3030 3c2f 543e 0d0a 2020 2020 2020 2020  00</T>..        
+00001840: 2020 2020 2020 2020 3c49 313e 342e 303c          <I1>4.0<
+00001850: 2f49 313e 0d0a 2020 2020 2020 2020 2020  /I1>..          
+00001860: 2020 3c2f 453e 0d0a 2020 2020 2020 2020    </E>..        
+00001870: 3c2f 4461 7461 3e0d 0a20 2020 203c 2f4d  </Data>..    </M
+00001880: 6561 7375 7265 6d65 6e74 3e0d 0a20 2020  easurement>..   
+00001890: 203c 4d65 6173 7572 656d 656e 7420 5369   <Measurement Si
+000018a0: 7465 4e61 6d65 3d22 4d69 6420 5374 7265  teName="Mid Stre
+000018b0: 616d 2061 7420 436f 7774 6f69 6c65 7420  am at Cowtoilet 
+000018c0: 4661 726d 223e 0d0a 2020 2020 2020 2020  Farm">..        
+000018d0: 3c44 6174 6153 6f75 7263 6520 4e61 6d65  <DataSource Name
+000018e0: 3d22 4e75 6d62 6572 206f 6620 4163 7475  ="Number of Actu
+000018f0: 616c 2057 686f 6c65 2048 756d 616e 2054  al Whole Human T
+00001900: 7572 6473 2046 6c6f 6174 696e 6720 4279  urds Floating By
+00001910: 2220 4e75 6d49 7465 6d73 3d22 3122 3e0d  " NumItems="1">.
+00001920: 0a20 2020 2020 2020 2020 2020 203c 5453  .            <TS
+00001930: 5479 7065 3e53 7464 5175 616c 5365 7269  Type>StdQualSeri
+00001940: 6573 3c2f 5453 5479 7065 3e0d 0a20 2020  es</TSType>..   
+00001950: 2020 2020 2020 2020 203c 4461 7461 5479           <DataTy
+00001960: 7065 3e54 7572 6473 2070 6572 2053 6563  pe>Turds per Sec
+00001970: 6f6e 643c 2f44 6174 6154 7970 653e 0d0a  ond</DataType>..
+00001980: 2020 2020 2020 2020 2020 2020 3c49 6e74              <Int
+00001990: 6572 706f 6c61 7469 6f6e 3e45 7665 6e74  erpolation>Event
+000019a0: 3c2f 496e 7465 7270 6f6c 6174 696f 6e3e  </Interpolation>
+000019b0: 0d0a 2020 2020 2020 2020 2020 2020 3c49  ..            <I
+000019c0: 7465 6d46 6f72 6d61 743e 303c 2f49 7465  temFormat>0</Ite
+000019d0: 6d46 6f72 6d61 743e 0d0a 2020 2020 2020  mFormat>..      
+000019e0: 2020 3c2f 4461 7461 536f 7572 6365 3e0d    </DataSource>.
+000019f0: 0a20 2020 2020 2020 203c 4461 7461 2044  .        <Data D
+00001a00: 6174 6546 6f72 6d61 743d 226d 6f77 7365  ateFormat="mowse
+00001a10: 6373 2220 4e75 6d49 7465 6d73 3d22 3122  cs" NumItems="1"
+00001a20: 3e0d 0a20 2020 2020 2020 2020 2020 203c  >..            <
+00001a30: 453e 0d0a 2020 2020 2020 2020 2020 2020  E>..            
+00001a40: 2020 2020 3c54 3e32 3631 3933 3032 3430      <T>261930240
+00001a50: 303c 2f54 3e0d 0a20 2020 2020 2020 2020  0</T>..         
+00001a60: 2020 2020 2020 203c 4931 3e32 3030 3c2f         <I1>200</
+00001a70: 4931 3e0d 0a20 2020 2020 2020 2020 2020  I1>..           
+00001a80: 203c 2f45 3e0d 0a20 2020 2020 2020 203c   </E>..        <
+00001a90: 2f44 6174 613e 0d0a 2020 2020 3c2f 4d65  /Data>..    </Me
+00001aa0: 6173 7572 656d 656e 743e 0d0a 2020 2020  asurement>..    
+00001ab0: 3c4d 6561 7375 7265 6d65 6e74 2053 6974  <Measurement Sit
+00001ac0: 654e 616d 653d 224d 6964 2053 7472 6561  eName="Mid Strea
+00001ad0: 6d20 6174 2043 6f77 746f 696c 6574 2046  m at Cowtoilet F
+00001ae0: 6172 6d22 3e0d 0a20 2020 2020 2020 203c  arm">..        <
+00001af0: 4461 7461 536f 7572 6365 204e 616d 653d  DataSource Name=
+00001b00: 224e 756d 6265 7220 6f66 2041 6374 7561  "Number of Actua
+00001b10: 6c20 5768 6f6c 6520 4875 6d61 6e20 5475  l Whole Human Tu
+00001b20: 7264 7320 466c 6f61 7469 6e67 2042 7922  rds Floating By"
+00001b30: 204e 756d 4974 656d 733d 2234 223e 0d0a   NumItems="4">..
+00001b40: 2020 2020 2020 2020 2020 2020 3c54 5354              <TST
+00001b50: 7970 653e 4368 6563 6b53 6572 6965 733c  ype>CheckSeries<
+00001b60: 2f54 5354 7970 653e 0d0a 2020 2020 2020  /TSType>..      
+00001b70: 2020 2020 2020 3c44 6174 6154 7970 653e        <DataType>
+00001b80: 5475 7264 7320 7065 7220 5365 636f 6e64  Turds per Second
+00001b90: 3c2f 4461 7461 5479 7065 3e0d 0a20 2020  </DataType>..   
+00001ba0: 2020 2020 2020 2020 203c 496e 7465 7270           <Interp
+00001bb0: 6f6c 6174 696f 6e3e 4469 7363 7265 7465  olation>Discrete
+00001bc0: 3c2f 496e 7465 7270 6f6c 6174 696f 6e3e  </Interpolation>
+00001bd0: 0d0a 2020 2020 2020 2020 2020 2020 3c49  ..            <I
+00001be0: 7465 6d46 6f72 6d61 743e 3134 303c 2f49  temFormat>140</I
+00001bf0: 7465 6d46 6f72 6d61 743e 0d0a 2020 2020  temFormat>..    
+00001c00: 2020 2020 2020 2020 3c49 7465 6d49 6e66          <ItemInf
+00001c10: 6f20 4974 656d 4e75 6d62 6572 3d22 3122  o ItemNumber="1"
+00001c20: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
+00001c30: 2020 203c 4974 656d 4e61 6d65 3e54 7572     <ItemName>Tur
+00001c40: 6469 6469 7479 2053 656e 736f 7220 5265  didity Sensor Re
+00001c50: 6164 696e 673c 2f49 7465 6d4e 616d 653e  ading</ItemName>
+00001c60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001c70: 2020 3c49 7465 6d46 6f72 6d61 743e 463c    <ItemFormat>F<
+00001c80: 2f49 7465 6d46 6f72 6d61 743e 0d0a 2020  /ItemFormat>..  
+00001c90: 2020 2020 2020 2020 2020 2020 2020 3c44                <D
+00001ca0: 6976 6973 6f72 3e31 3c2f 4469 7669 736f  ivisor>1</Diviso
+00001cb0: 723e 0d0a 2020 2020 2020 2020 2020 2020  r>..            
+00001cc0: 2020 2020 3c55 6e69 7473 3e74 2f73 3c2f      <Units>t/s</
+00001cd0: 556e 6974 733e 0d0a 2020 2020 2020 2020  Units>..        
+00001ce0: 2020 2020 2020 2020 3c46 6f72 6d61 743e          <Format>
+00001cf0: 2323 2323 2e23 3c2f 466f 726d 6174 3e0d  ####.#</Format>.
+00001d00: 0a20 2020 2020 2020 2020 2020 203c 2f49  .            </I
+00001d10: 7465 6d49 6e66 6f3e 0d0a 2020 2020 2020  temInfo>..      
+00001d20: 2020 2020 2020 3c49 7465 6d49 6e66 6f20        <ItemInfo 
+00001d30: 4974 656d 4e75 6d62 6572 3d22 3222 3e0d  ItemNumber="2">.
+00001d40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001d50: 203c 4974 656d 4e61 6d65 3e52 6563 6f72   <ItemName>Recor
+00001d60: 6465 7220 5469 6d65 3c2f 4974 656d 4e61  der Time</ItemNa
+00001d70: 6d65 3e0d 0a20 2020 2020 2020 2020 2020  me>..           
+00001d80: 2020 2020 203c 4974 656d 466f 726d 6174       <ItemFormat
+00001d90: 3e44 3c2f 4974 656d 466f 726d 6174 3e0d  >D</ItemFormat>.
+00001da0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001db0: 203c 4469 7669 736f 723e 303c 2f44 6976   <Divisor>0</Div
+00001dc0: 6973 6f72 3e0d 0a20 2020 2020 2020 2020  isor>..         
+00001dd0: 2020 2020 2020 203c 556e 6974 7320 2f3e         <Units />
+00001de0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001df0: 2020 3c46 6f72 6d61 743e 2323 233c 2f46    <Format>###</F
+00001e00: 6f72 6d61 743e 0d0a 2020 2020 2020 2020  ormat>..        
+00001e10: 2020 2020 3c2f 4974 656d 496e 666f 3e0d      </ItemInfo>.
+00001e20: 0a20 2020 2020 2020 2020 2020 203c 4974  .            <It
+00001e30: 656d 496e 666f 2049 7465 6d4e 756d 6265  emInfo ItemNumbe
+00001e40: 723d 2233 223e 0d0a 2020 2020 2020 2020  r="3">..        
+00001e50: 2020 2020 2020 2020 3c49 7465 6d4e 616d          <ItemNam
+00001e60: 653e 4861 6e64 6865 6c64 2054 7572 6469  e>Handheld Turdi
+00001e70: 6469 7479 2053 656e 736f 7220 5265 6164  dity Sensor Read
+00001e80: 696e 673c 2f49 7465 6d4e 616d 653e 0d0a  ing</ItemName>..
+00001e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ea0: 3c49 7465 6d46 6f72 6d61 743e 463c 2f49  <ItemFormat>F</I
+00001eb0: 7465 6d46 6f72 6d61 743e 0d0a 2020 2020  temFormat>..    
+00001ec0: 2020 2020 2020 2020 2020 2020 3c44 6976              <Div
+00001ed0: 6973 6f72 3e31 3c2f 4469 7669 736f 723e  isor>1</Divisor>
+00001ee0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001ef0: 2020 3c55 6e69 7473 202f 3e0d 0a20 2020    <Units />..   
+00001f00: 2020 2020 2020 2020 2020 2020 203c 466f               <Fo
+00001f10: 726d 6174 3e23 2323 2e23 3c2f 466f 726d  rmat>###.#</Form
+00001f20: 6174 3e0d 0a20 2020 2020 2020 2020 2020  at>..           
+00001f30: 203c 2f49 7465 6d49 6e66 6f3e 0d0a 2020   </ItemInfo>..  
+00001f40: 2020 2020 2020 2020 2020 3c49 7465 6d49            <ItemI
+00001f50: 6e66 6f20 4974 656d 4e75 6d62 6572 3d22  nfo ItemNumber="
+00001f60: 3422 3e0d 0a20 2020 2020 2020 2020 2020  4">..           
+00001f70: 2020 2020 203c 4974 656d 4e61 6d65 3e43       <ItemName>C
+00001f80: 6f6d 6d65 6e74 3c2f 4974 656d 4e61 6d65  omment</ItemName
+00001f90: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
+00001fa0: 2020 203c 4974 656d 466f 726d 6174 3e53     <ItemFormat>S
+00001fb0: 3c2f 4974 656d 466f 726d 6174 3e0d 0a20  </ItemFormat>.. 
+00001fc0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00001fd0: 4469 7669 736f 723e 313c 2f44 6976 6973  Divisor>1</Divis
+00001fe0: 6f72 3e0d 0a20 2020 2020 2020 2020 2020  or>..           
+00001ff0: 2020 2020 203c 556e 6974 7320 2f3e 0d0a       <Units />..
+00002000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002010: 3c46 6f72 6d61 743e 2323 233c 2f46 6f72  <Format>###</For
+00002020: 6d61 743e 0d0a 2020 2020 2020 2020 2020  mat>..          
+00002030: 2020 3c2f 4974 656d 496e 666f 3e0d 0a20    </ItemInfo>.. 
+00002040: 2020 2020 2020 203c 2f44 6174 6153 6f75         </DataSou
+00002050: 7263 653e 0d0a 2020 2020 2020 2020 3c44  rce>..        <D
+00002060: 6174 6120 4461 7465 466f 726d 6174 3d22  ata DateFormat="
+00002070: 6d6f 7773 6563 7322 204e 756d 4974 656d  mowsecs" NumItem
+00002080: 733d 2234 223e 0d0a 2020 2020 2020 2020  s="4">..        
+00002090: 2020 2020 3c45 3e0d 0a20 2020 2020 2020      <E>..       
+000020a0: 2020 2020 2020 2020 203c 543e 3236 3139           <T>2619
+000020b0: 3330 3234 3030 3c2f 543e 0d0a 2020 2020  302400</T>..    
+000020c0: 2020 2020 2020 2020 2020 2020 3c49 313e              <I1>
+000020d0: 3132 2e34 3c2f 4931 3e0d 0a20 2020 2020  12.4</I1>..     
+000020e0: 2020 2020 2020 2020 2020 203c 4932 3e32             <I2>2
+000020f0: 3631 3933 3032 3430 303c 2f49 323e 0d0a  619302400</I2>..
+00002100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002110: 3c49 333e 3132 3435 2e32 3c2f 4933 3e0d  <I3>1245.2</I3>.
+00002120: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002130: 203c 4934 3e0d 0a20 2020 2020 2020 2020   <I4>..         
+00002140: 2020 2020 2020 2020 2020 2053 7475 6d62             Stumb
+00002150: 6c65 6420 7570 6f6e 2061 206e 7564 6973  led upon a nudis
+00002160: 7420 636f 6c6f 6e79 2e0d 0a20 2020 2020  t colony...     
+00002170: 2020 2020 2020 2020 2020 203c 2f49 343e             </I4>
+00002180: 0d0a 2020 2020 2020 2020 2020 2020 3c2f  ..            </
+00002190: 453e 0d0a 2020 2020 2020 2020 2020 2020  E>..            
+000021a0: 3c45 3e0d 0a20 2020 2020 2020 2020 2020  <E>..           
+000021b0: 2020 2020 203c 543e 3236 3139 3330 3330       <T>26193030
+000021c0: 3030 3c2f 543e 0d0a 2020 2020 2020 2020  00</T>..        
+000021d0: 2020 2020 2020 2020 3c49 313e 3134 3531          <I1>1451
+000021e0: 2e32 3c2f 4931 3e0d 0a20 2020 2020 2020  .2</I1>..       
+000021f0: 2020 2020 2020 2020 203c 4932 3e32 3631           <I2>261
+00002200: 3933 3033 3030 303c 2f49 323e 0d0a 2020  9303000</I2>..  
+00002210: 2020 2020 2020 2020 2020 2020 2020 3c49                <I
+00002220: 333e 3132 3334 2e35 3c2f 4933 3e0d 0a20  3>1234.5</I3>.. 
+00002230: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00002240: 4934 3e0d 0a20 2020 2020 2020 2020 2020  I4>..           
+00002250: 2020 2020 2020 2020 2046 7269 656e 646c           Friendl
+00002260: 7920 636f 772e 2050 6f73 7369 626c 7920  y cow. Possibly 
+00002270: 6120 7370 792e 0d0a 2020 2020 2020 2020  a spy...        
+00002280: 2020 2020 2020 2020 3c2f 4934 3e0d 0a20          </I4>.. 
+00002290: 2020 2020 2020 2020 2020 203c 2f45 3e0d             </E>.
+000022a0: 0a20 2020 2020 2020 2020 2020 203c 453e  .            <E>
+000022b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000022c0: 2020 3c54 3e32 3631 3933 3034 3230 303c    <T>2619304200<
+000022d0: 2f54 3e0d 0a20 2020 2020 2020 2020 2020  /T>..           
+000022e0: 2020 2020 203c 4931 3e32 3436 362e 323c       <I1>2466.2<
+000022f0: 2f49 313e 0d0a 2020 2020 2020 2020 2020  /I1>..          
 00002300: 2020 2020 2020 3c49 323e 3236 3139 3330        <I2>261930
-00002310: 3531 3030 3c2f 4932 3e0a 2020 2020 2020  5100</I2>.      
-00002320: 2020 2020 2020 2020 2020 3c49 333e 3830            <I3>80
-00002330: 3530 2e30 3c2f 4933 3e0a 2020 2020 2020  50.0</I3>.      
-00002340: 2020 2020 2020 2020 2020 3c49 343e 4d65            <I4>Me
-00002350: 7420 616e 206f 6c64 2077 6f6d 616e 2077  t an old woman w
-00002360: 686f 2063 6c61 696d 6564 2074 6869 7320  ho claimed this 
-00002370: 7369 7465 2077 6173 206f 6e63 6520 616e  site was once an
-00002380: 2061 6e63 6965 6e74 206e 6174 6976 6520   ancient native 
-00002390: 616d 6572 6963 616e 2062 7572 6961 6c20  american burial 
-000023a0: 6772 6f75 6e64 2e20 5365 656d 7320 756e  ground. Seems un
-000023b0: 6c69 6b65 6c79 2e3c 2f49 343e 0a20 2020  likely.</I4>.   
-000023c0: 2020 2020 2020 2020 203c 2f45 3e0a 2020           </E>.  
-000023d0: 2020 2020 2020 3c2f 4461 7461 3e0a 2020        </Data>.  
-000023e0: 2020 3c2f 4d65 6173 7572 656d 656e 743e    </Measurement>
-000023f0: 0a20 2020 203c 4d65 6173 7572 656d 656e  .    <Measuremen
-00002400: 7420 5369 7465 4e61 6d65 3d22 4d69 6420  t SiteName="Mid 
-00002410: 5374 7265 616d 2061 7420 436f 7774 6f69  Stream at Cowtoi
-00002420: 6c65 7420 4661 726d 223e 0a20 2020 2020  let Farm">.     
-00002430: 2020 203c 4461 7461 536f 7572 6365 204e     <DataSource N
-00002440: 616d 653d 2244 6561 6420 436f 7720 436f  ame="Dead Cow Co
-00002450: 6e63 656e 7472 6174 696f 6e22 204e 756d  ncentration" Num
-00002460: 4974 656d 733d 2231 223e 0a20 2020 2020  Items="1">.     
-00002470: 2020 2020 2020 203c 5453 5479 7065 3e53         <TSType>S
-00002480: 7464 5365 7269 6573 3c2f 5453 5479 7065  tdSeries</TSType
-00002490: 3e0a 2020 2020 2020 2020 2020 2020 3c44  >.            <D
-000024a0: 6174 6154 7970 653e 5061 7274 7320 7065  ataType>Parts pe
-000024b0: 7220 4d69 6c6c 696f 6e3c 2f44 6174 6154  r Million</DataT
-000024c0: 7970 653e 0a20 2020 2020 2020 2020 2020  ype>.           
-000024d0: 203c 496e 7465 7270 6f6c 6174 696f 6e3e   <Interpolation>
-000024e0: 496e 6372 656d 656e 7461 6c3c 2f49 6e74  Incremental</Int
-000024f0: 6572 706f 6c61 7469 6f6e 3e0a 2020 2020  erpolation>.    
-00002500: 2020 2020 2020 2020 3c49 7465 6d46 6f72          <ItemFor
-00002510: 6d61 743e 303c 2f49 7465 6d46 6f72 6d61  mat>0</ItemForma
-00002520: 743e 0a20 2020 2020 2020 2020 2020 203c  t>.            <
-00002530: 4974 656d 496e 666f 2049 7465 6d4e 756d  ItemInfo ItemNum
-00002540: 6265 723d 2231 223e 0a20 2020 2020 2020  ber="1">.       
-00002550: 2020 2020 2020 2020 203c 4974 656d 4e61           <ItemNa
-00002560: 6d65 3e44 6561 6420 436f 7720 436f 6e63  me>Dead Cow Conc
-00002570: 656e 7472 6174 696f 6e3c 2f49 7465 6d4e  entration</ItemN
-00002580: 616d 653e 0a20 2020 2020 2020 2020 2020  ame>.           
-00002590: 2020 2020 203c 4974 656d 466f 726d 6174       <ItemFormat
-000025a0: 3e49 3c2f 4974 656d 466f 726d 6174 3e0a  >I</ItemFormat>.
-000025b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025c0: 3c44 6976 6973 6f72 3e31 3c2f 4469 7669  <Divisor>1</Divi
-000025d0: 736f 723e 0a20 2020 2020 2020 2020 2020  sor>.           
-000025e0: 2020 2020 203c 556e 6974 733e 7070 6d3c       <Units>ppm<
-000025f0: 2f55 6e69 7473 3e0a 2020 2020 2020 2020  /Units>.        
-00002600: 2020 2020 2020 2020 3c46 6f72 6d61 743e          <Format>
-00002610: 2323 3c2f 466f 726d 6174 3e0a 2020 2020  ##</Format>.    
-00002620: 2020 2020 2020 2020 3c2f 4974 656d 496e          </ItemIn
-00002630: 666f 3e0a 2020 2020 2020 2020 3c2f 4461  fo>.        </Da
-00002640: 7461 536f 7572 6365 3e0a 2020 2020 2020  taSource>.      
-00002650: 2020 3c44 6174 6120 4461 7465 466f 726d    <Data DateForm
-00002660: 6174 3d22 6d6f 7773 6563 7322 204e 756d  at="mowsecs" Num
-00002670: 4974 656d 733d 2231 223e 0a20 2020 2020  Items="1">.     
-00002680: 2020 2020 2020 203c 453e 0a20 2020 2020         <E>.     
-00002690: 2020 2020 2020 2020 2020 203c 543e 3236             <T>26
-000026a0: 3139 3330 3234 3030 3c2f 543e 0a20 2020  19302400</T>.   
-000026b0: 2020 2020 2020 2020 2020 2020 203c 4931               <I1
-000026c0: 3e31 3c2f 4931 3e0a 2020 2020 2020 2020  >1</I1>.        
-000026d0: 2020 2020 3c2f 453e 0a20 2020 2020 2020      </E>.       
-000026e0: 2020 2020 203c 453e 0a20 2020 2020 2020       <E>.       
-000026f0: 2020 2020 2020 2020 203c 543e 3236 3139           <T>2619
-00002700: 3330 3237 3030 3c2f 543e 0a20 2020 2020  302700</T>.     
-00002710: 2020 2020 2020 2020 2020 203c 4931 3e37             <I1>7
-00002720: 3c2f 4931 3e0a 2020 2020 2020 2020 2020  </I1>.          
-00002730: 2020 3c2f 453e 0a20 2020 2020 2020 2020    </E>.         
-00002740: 2020 203c 453e 0a20 2020 2020 2020 2020     <E>.         
-00002750: 2020 2020 2020 203c 543e 3236 3139 3330         <T>261930
-00002760: 3330 3030 3c2f 543e 0a20 2020 2020 2020  3000</T>.       
-00002770: 2020 2020 2020 2020 203c 4931 3e31 3c2f           <I1>1</
-00002780: 4931 3e0a 2020 2020 2020 2020 2020 2020  I1>.            
-00002790: 3c2f 453e 0a20 2020 2020 2020 2020 2020  </E>.           
-000027a0: 203c 453e 0a20 2020 2020 2020 2020 2020   <E>.           
-000027b0: 2020 2020 203c 543e 3236 3139 3330 3333       <T>26193033
-000027c0: 3030 3c2f 543e 0a20 2020 2020 2020 2020  00</T>.         
-000027d0: 2020 2020 2020 203c 4931 3e31 3c2f 4931         <I1>1</I1
-000027e0: 3e0a 2020 2020 2020 2020 2020 2020 3c2f  >.            </
-000027f0: 453e 0a20 2020 2020 2020 2020 2020 203c  E>.            <
-00002800: 453e 0a20 2020 2020 2020 2020 2020 2020  E>.             
-00002810: 2020 203c 543e 3236 3139 3330 3336 3030     <T>2619303600
-00002820: 3c2f 543e 0a20 2020 2020 2020 2020 2020  </T>.           
-00002830: 2020 2020 203c 4931 3e31 3c2f 4931 3e0a       <I1>1</I1>.
-00002840: 2020 2020 2020 2020 2020 2020 3c2f 453e              </E>
-00002850: 0a20 2020 2020 2020 2020 2020 203c 453e  .            <E>
-00002860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002870: 203c 543e 3236 3139 3330 3339 3030 3c2f   <T>2619303900</
-00002880: 543e 0a20 2020 2020 2020 2020 2020 2020  T>.             
-00002890: 2020 203c 4931 3e31 3c2f 4931 3e0a 2020     <I1>1</I1>.  
-000028a0: 2020 2020 2020 2020 2020 3c2f 453e 0a20            </E>. 
-000028b0: 2020 2020 2020 2020 2020 203c 453e 0a20             <E>. 
-000028c0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000028d0: 543e 3236 3139 3330 3432 3030 3c2f 543e  T>2619304200</T>
-000028e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000028f0: 203c 4931 3e36 3c2f 4931 3e0a 2020 2020   <I1>6</I1>.    
-00002900: 2020 2020 2020 2020 3c2f 453e 0a20 2020          </E>.   
-00002910: 2020 2020 2020 2020 203c 453e 0a20 2020           <E>.   
-00002920: 2020 2020 2020 2020 2020 2020 203c 543e               <T>
-00002930: 3236 3139 3330 3435 3030 3c2f 543e 0a20  2619304500</T>. 
-00002940: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00002950: 4931 3e36 3c2f 4931 3e0a 2020 2020 2020  I1>6</I1>.      
-00002960: 2020 2020 2020 3c2f 453e 0a20 2020 2020        </E>.     
-00002970: 2020 2020 2020 203c 453e 0a20 2020 2020         <E>.     
-00002980: 2020 2020 2020 2020 2020 203c 543e 3236             <T>26
-00002990: 3139 3330 3438 3030 3c2f 543e 0a20 2020  19304800</T>.   
-000029a0: 2020 2020 2020 2020 2020 2020 203c 4931               <I1
-000029b0: 3e39 3c2f 4931 3e0a 2020 2020 2020 2020  >9</I1>.        
-000029c0: 2020 2020 3c2f 453e 0a20 2020 2020 2020      </E>.       
-000029d0: 2020 2020 203c 453e 0a20 2020 2020 2020       <E>.       
-000029e0: 2020 2020 2020 2020 203c 543e 3236 3139           <T>2619
-000029f0: 3330 3531 3030 3c2f 543e 0a20 2020 2020  305100</T>.     
-00002a00: 2020 2020 2020 2020 2020 203c 4931 3e34             <I1>4
-00002a10: 3c2f 4931 3e0a 2020 2020 2020 2020 2020  </I1>.          
-00002a20: 2020 3c2f 453e 0a20 2020 2020 2020 203c    </E>.        <
-00002a30: 2f44 6174 613e 0a20 2020 203c 2f4d 6561  /Data>.    </Mea
-00002a40: 7375 7265 6d65 6e74 3e0a 2020 2020 3c4d  surement>.    <M
-00002a50: 6561 7375 7265 6d65 6e74 2053 6974 654e  easurement SiteN
-00002a60: 616d 653d 224d 6964 2053 7472 6561 6d20  ame="Mid Stream 
-00002a70: 6174 2043 6f77 746f 696c 6574 2046 6172  at Cowtoilet Far
-00002a80: 6d22 3e0a 2020 2020 2020 2020 3c44 6174  m">.        <Dat
-00002a90: 6153 6f75 7263 6520 4e61 6d65 3d22 4465  aSource Name="De
-00002aa0: 6164 2043 6f77 2043 6f6e 6365 6e74 7261  ad Cow Concentra
-00002ab0: 7469 6f6e 2220 4e75 6d49 7465 6d73 3d22  tion" NumItems="
-00002ac0: 3122 3e0a 2020 2020 2020 2020 2020 2020  1">.            
-00002ad0: 3c54 5354 7970 653e 5374 6451 7561 6c53  <TSType>StdQualS
-00002ae0: 6572 6965 733c 2f54 5354 7970 653e 0a20  eries</TSType>. 
-00002af0: 2020 2020 2020 2020 2020 203c 4461 7461             <Data
-00002b00: 5479 7065 3e44 6561 6420 436f 7773 3c2f  Type>Dead Cows</
-00002b10: 4461 7461 5479 7065 3e0a 2020 2020 2020  DataType>.      
-00002b20: 2020 2020 2020 3c49 6e74 6572 706f 6c61        <Interpola
-00002b30: 7469 6f6e 3e45 7665 6e74 3c2f 496e 7465  tion>Event</Inte
-00002b40: 7270 6f6c 6174 696f 6e3e 0a20 2020 2020  rpolation>.     
-00002b50: 2020 2020 2020 203c 4974 656d 466f 726d         <ItemForm
-00002b60: 6174 3e30 3c2f 4974 656d 466f 726d 6174  at>0</ItemFormat
-00002b70: 3e0a 2020 2020 2020 2020 3c2f 4461 7461  >.        </Data
-00002b80: 536f 7572 6365 3e0a 2020 2020 2020 2020  Source>.        
-00002b90: 3c44 6174 6120 4461 7465 466f 726d 6174  <Data DateFormat
-00002ba0: 3d22 6d6f 7773 6563 7322 204e 756d 4974  ="mowsecs" NumIt
-00002bb0: 656d 733d 2231 223e 0a20 2020 2020 2020  ems="1">.       
-00002bc0: 2020 2020 203c 453e 0a20 2020 2020 2020       <E>.       
-00002bd0: 2020 2020 2020 2020 203c 543e 3236 3139           <T>2619
-00002be0: 3330 3233 3939 3c2f 543e 0a20 2020 2020  302399</T>.     
-00002bf0: 2020 2020 2020 2020 2020 203c 4931 3e36             <I1>6
-00002c00: 3030 3c2f 4931 3e0a 2020 2020 2020 2020  00</I1>.        
-00002c10: 2020 2020 3c2f 453e 0a20 2020 2020 2020      </E>.       
-00002c20: 203c 2f44 6174 613e 0a20 2020 203c 2f4d   </Data>.    </M
-00002c30: 6561 7375 7265 6d65 6e74 3e0a 2020 2020  easurement>.    
-00002c40: 3c4d 6561 7375 7265 6d65 6e74 2053 6974  <Measurement Sit
-00002c50: 654e 616d 653d 224d 6964 2053 7472 6561  eName="Mid Strea
-00002c60: 6d20 6174 2043 6f77 746f 696c 6574 2046  m at Cowtoilet F
-00002c70: 6172 6d22 3e0a 2020 2020 2020 2020 3c44  arm">.        <D
-00002c80: 6174 6153 6f75 7263 6520 4e61 6d65 3d22  ataSource Name="
-00002c90: 4465 6164 2043 6f77 2043 6f6e 6365 6e74  Dead Cow Concent
-00002ca0: 7261 7469 6f6e 2220 4e75 6d49 7465 6d73  ration" NumItems
-00002cb0: 3d22 3322 3e0a 2020 2020 2020 2020 2020  ="3">.          
-00002cc0: 2020 3c54 5354 7970 653e 4368 6563 6b53    <TSType>CheckS
-00002cd0: 6572 6965 733c 2f54 5354 7970 653e 0a20  eries</TSType>. 
-00002ce0: 2020 2020 2020 2020 2020 203c 4461 7461             <Data
-00002cf0: 5479 7065 3e44 6561 6420 436f 7773 3c2f  Type>Dead Cows</
-00002d00: 4461 7461 5479 7065 3e0a 2020 2020 2020  DataType>.      
-00002d10: 2020 2020 2020 3c49 6e74 6572 706f 6c61        <Interpola
-00002d20: 7469 6f6e 3e44 6973 6372 6574 653c 2f49  tion>Discrete</I
-00002d30: 6e74 6572 706f 6c61 7469 6f6e 3e0a 2020  nterpolation>.  
-00002d40: 2020 2020 2020 2020 2020 3c49 7465 6d46            <ItemF
-00002d50: 6f72 6d61 743e 3134 303c 2f49 7465 6d46  ormat>140</ItemF
-00002d60: 6f72 6d61 743e 0a20 2020 2020 2020 2020  ormat>.         
-00002d70: 2020 203c 4974 656d 496e 666f 2049 7465     <ItemInfo Ite
-00002d80: 6d4e 756d 6265 723d 2231 223e 0a20 2020  mNumber="1">.   
-00002d90: 2020 2020 2020 2020 2020 2020 203c 4974               <It
-00002da0: 656d 4e61 6d65 3e44 6561 6420 436f 7720  emName>Dead Cow 
-00002db0: 436f 6e63 656e 7472 6174 696f 6e3c 2f49  Concentration</I
-00002dc0: 7465 6d4e 616d 653e 0a20 2020 2020 2020  temName>.       
-00002dd0: 2020 2020 2020 2020 203c 4974 656d 466f           <ItemFo
-00002de0: 726d 6174 3e49 3c2f 4974 656d 466f 726d  rmat>I</ItemForm
-00002df0: 6174 3e0a 2020 2020 2020 2020 2020 2020  at>.            
-00002e00: 2020 2020 3c44 6976 6973 6f72 3e31 3c2f      <Divisor>1</
-00002e10: 4469 7669 736f 723e 0a20 2020 2020 2020  Divisor>.       
-00002e20: 2020 2020 2020 2020 203c 556e 6974 733e           <Units>
-00002e30: 7070 6d3c 2f55 6e69 7473 3e0a 2020 2020  ppm</Units>.    
-00002e40: 2020 2020 2020 2020 2020 2020 3c46 6f72              <For
-00002e50: 6d61 743e 2323 3c2f 466f 726d 6174 3e0a  mat>##</Format>.
-00002e60: 2020 2020 2020 2020 2020 2020 3c2f 4974              </It
-00002e70: 656d 496e 666f 3e0a 2020 2020 2020 2020  emInfo>.        
-00002e80: 2020 2020 3c49 7465 6d49 6e66 6f20 4974      <ItemInfo It
-00002e90: 656d 4e75 6d62 6572 3d22 3222 3e0a 2020  emNumber="2">.  
-00002ea0: 2020 2020 2020 2020 2020 2020 2020 3c49                <I
-00002eb0: 7465 6d4e 616d 653e 5265 636f 7264 6572  temName>Recorder
-00002ec0: 2054 696d 653c 2f49 7465 6d4e 616d 653e   Time</ItemName>
-00002ed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002ee0: 203c 4974 656d 466f 726d 6174 3e44 3c2f   <ItemFormat>D</
-00002ef0: 4974 656d 466f 726d 6174 3e0a 2020 2020  ItemFormat>.    
-00002f00: 2020 2020 2020 2020 2020 2020 3c44 6976              <Div
-00002f10: 6973 6f72 3e31 3c2f 4469 7669 736f 723e  isor>1</Divisor>
-00002f20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002f30: 203c 556e 6974 7320 2f3e 0a20 2020 2020   <Units />.     
-00002f40: 2020 2020 2020 2020 2020 203c 466f 726d             <Form
-00002f50: 6174 3e23 2323 3c2f 466f 726d 6174 3e0a  at>###</Format>.
-00002f60: 2020 2020 2020 2020 2020 2020 3c2f 4974              </It
-00002f70: 656d 496e 666f 3e0a 2020 2020 2020 2020  emInfo>.        
-00002f80: 2020 2020 3c49 7465 6d49 6e66 6f20 4974      <ItemInfo It
-00002f90: 656d 4e75 6d62 6572 3d22 3322 3e0a 2020  emNumber="3">.  
-00002fa0: 2020 2020 2020 2020 2020 2020 2020 3c49                <I
-00002fb0: 7465 6d4e 616d 653e 436f 6d6d 656e 743c  temName>Comment<
-00002fc0: 2f49 7465 6d4e 616d 653e 0a20 2020 2020  /ItemName>.     
-00002fd0: 2020 2020 2020 2020 2020 203c 4974 656d             <Item
-00002fe0: 466f 726d 6174 3e53 3c2f 4974 656d 466f  Format>S</ItemFo
-00002ff0: 726d 6174 3e0a 2020 2020 2020 2020 2020  rmat>.          
-00003000: 2020 2020 2020 3c44 6976 6973 6f72 3e31        <Divisor>1
-00003010: 3c2f 4469 7669 736f 723e 0a20 2020 2020  </Divisor>.     
-00003020: 2020 2020 2020 2020 2020 203c 556e 6974             <Unit
-00003030: 7320 2f3e 0a20 2020 2020 2020 2020 2020  s />.           
-00003040: 2020 2020 203c 466f 726d 6174 3e23 2323       <Format>###
-00003050: 3c2f 466f 726d 6174 3e0a 2020 2020 2020  </Format>.      
-00003060: 2020 2020 2020 3c2f 4974 656d 496e 666f        </ItemInfo
-00003070: 3e0a 2020 2020 2020 2020 3c2f 4461 7461  >.        </Data
-00003080: 536f 7572 6365 3e0a 2020 2020 2020 2020  Source>.        
-00003090: 3c44 6174 6120 4461 7465 466f 726d 6174  <Data DateFormat
-000030a0: 3d22 6d6f 7773 6563 7322 204e 756d 4974  ="mowsecs" NumIt
-000030b0: 656d 733d 2233 223e 0a20 2020 2020 2020  ems="3">.       
-000030c0: 2020 2020 203c 453e 0a20 2020 2020 2020       <E>.       
-000030d0: 2020 2020 2020 2020 203c 543e 3236 3139           <T>2619
-000030e0: 3330 3234 3030 3c2f 543e 0a20 2020 2020  302400</T>.     
-000030f0: 2020 2020 2020 2020 2020 203c 4931 3e35             <I1>5
-00003100: 3c2f 4931 3e0a 2020 2020 2020 2020 2020  </I1>.          
-00003110: 2020 2020 2020 3c49 323e 3236 3139 3330        <I2>261930
-00003120: 3234 3030 3c2f 4932 3e0a 2020 2020 2020  2400</I2>.      
-00003130: 2020 2020 2020 2020 2020 3c49 333e 0a20            <I3>. 
-00003140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003150: 2020 2043 6172 626f 6e20 6f66 6673 6574     Carbon offset
-00003160: 7320 6172 6520 6120 6d61 7373 6976 6520  s are a massive 
-00003170: 7363 616d 2e0a 2020 2020 2020 2020 2020  scam..          
-00003180: 2020 2020 2020 3c2f 4933 3e0a 2020 2020        </I3>.    
-00003190: 2020 2020 2020 2020 3c2f 453e 0a20 2020          </E>.   
-000031a0: 2020 2020 2020 2020 203c 453e 0a20 2020           <E>.   
-000031b0: 2020 2020 2020 2020 2020 2020 203c 543e               <T>
-000031c0: 3236 3139 3330 3330 3030 3c2f 543e 0a20  2619303000</T>. 
-000031d0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000031e0: 4931 3e33 3c2f 4931 3e0a 2020 2020 2020  I1>3</I1>.      
-000031f0: 2020 2020 2020 2020 2020 3c49 323e 3236            <I2>26
-00003200: 3139 3330 3330 3030 3c2f 4932 3e0a 2020  19303000</I2>.  
-00003210: 2020 2020 2020 2020 2020 2020 2020 3c49                <I
-00003220: 333e 0a20 2020 2020 2020 2020 2020 2020  3>.             
-00003230: 2020 2020 2020 2022 4361 7262 6f6e 2063         "Carbon c
-00003240: 7265 6469 7473 2220 6172 6520 6e6f 7468  redits" are noth
-00003250: 696e 6720 6d6f 7265 2074 6861 6e20 6120  ing more than a 
-00003260: 6672 6565 2074 6963 6b65 7420 746f 2070  free ticket to p
-00003270: 6f6c 6c75 7465 2069 6e20 7265 7475 726e  ollute in return
-00003280: 2066 6f72 2061 2070 726f 6d69 7365 2074   for a promise t
-00003290: 6861 7420 6120 7069 6563 6520 6f66 2066  hat a piece of f
-000032a0: 6f72 6573 7420 6973 2070 7265 7365 7276  orest is preserv
-000032b0: 6564 2e0a 2020 2020 2020 2020 2020 2020  ed..            
-000032c0: 2020 2020 3c2f 4933 3e0a 2020 2020 2020      </I3>.      
-000032d0: 2020 2020 2020 3c2f 453e 0a20 2020 2020        </E>.     
-000032e0: 2020 2020 2020 203c 453e 0a20 2020 2020         <E>.     
-000032f0: 2020 2020 2020 2020 2020 203c 543e 3236             <T>26
-00003300: 3139 3330 3339 3030 3c2f 543e 0a20 2020  19303900</T>.   
-00003310: 2020 2020 2020 2020 2020 2020 203c 4931               <I1
-00003320: 3e31 3c2f 4931 3e0a 2020 2020 2020 2020  >1</I1>.        
-00003330: 2020 2020 2020 2020 3c49 323e 3236 3139          <I2>2619
-00003340: 3330 3339 3030 3c2f 4932 3e0a 2020 2020  303900</I2>.    
-00003350: 2020 2020 2020 2020 2020 2020 3c49 333e              <I3>
-00003360: 5052 4553 4552 5645 442c 206e 6f74 2072  PRESERVED, not r
-00003370: 6573 746f 7265 642e 2049 6e20 6d6f 7374  estored. In most
-00003380: 2063 6173 6573 2c20 616c 6c20 7468 6520   cases, all the 
-00003390: 6d6f 6e65 7920 7468 6174 2064 6f65 7320  money that does 
-000033a0: 6e6f 7420 676f 2074 6f77 6172 6473 206d  not go towards m
-000033b0: 6964 646c 656d 656e 2c20 676f 2074 6f77  iddlemen, go tow
-000033c0: 6172 6473 2070 7265 7665 6e74 696e 6720  ards preventing 
-000033d0: 616e 2061 6c72 6561 6479 2070 726f 7465  an already prote
-000033e0: 6374 6564 2066 6f72 6573 7420 6672 6f6d  cted forest from
-000033f0: 2062 6569 6e67 2063 7574 2064 6f77 6e20   being cut down 
-00003400: 6261 7365 6420 6f6e 206d 6173 7369 7665  based on massive
-00003410: 6c79 206f 7665 7262 6c6f 776e 2070 6f70  ly overblown pop
-00003420: 756c 6174 696f 6e20 616e 642f 6f72 2065  ulation and/or e
-00003430: 636f 6e6f 6d69 6320 6772 6f77 7468 2065  conomic growth e
-00003440: 7374 696d 6174 6573 2e3c 2f49 333e 0a20  stimates.</I3>. 
-00003450: 2020 2020 2020 2020 2020 203c 2f45 3e0a             </E>.
-00003460: 2020 2020 2020 2020 2020 2020 3c45 3e0a              <E>.
-00003470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003480: 3c54 3e32 3631 3933 3034 3830 303c 2f54  <T>2619304800</T
-00003490: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-000034a0: 2020 3c49 313e 343c 2f49 313e 0a20 2020    <I1>4</I1>.   
-000034b0: 2020 2020 2020 2020 2020 2020 203c 4932               <I2
-000034c0: 3e32 3631 3933 3034 3830 303c 2f49 323e  >2619304800</I2>
-000034d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000034e0: 203c 4933 3e49 6e20 6573 7365 6e63 653a   <I3>In essence:
-000034f0: 2022 4361 6e20 7765 2070 6f6c 6c75 7465   "Can we pollute
-00003500: 3f20 5765 2077 696c 6c20 6769 7665 2073  ? We will give s
-00003510: 6f6d 6520 6d6f 6e65 7920 746f 2074 6869  ome money to thi
-00003520: 7320 7065 7273 6f6e 2077 686f 2077 696c  s person who wil
-00003530: 6c20 7573 6520 7468 6174 206d 6f6e 6579  l use that money
-00003540: 2074 6f20 6f76 6572 6573 7469 6d61 7465   to overestimate
-00003550: 2074 6865 2070 6f74 656e 7469 616c 2064   the potential d
-00003560: 616d 6167 6520 746f 2061 2064 6973 7461  amage to a dista
-00003570: 6e74 2074 696e 7920 6368 756e 6b20 6f66  nt tiny chunk of
-00003580: 2072 6169 6e66 6f72 6573 7420 7468 6174   rainforest that
-00003590: 2069 7320 616c 7265 6164 7920 7072 6f74   is already prot
-000035a0: 6563 7465 642e 2054 6865 2073 6d61 6c6c  ected. The small
-000035b0: 2061 6d6f 756e 7420 6f66 206c 6566 746f   amount of lefto
-000035c0: 7665 7220 6d6f 6e65 7920 6361 6e20 7468  ver money can th
-000035d0: 656e 2067 6f20 746f 2074 6865 2063 6f72  en go to the cor
-000035e0: 7275 7074 2067 6f76 6572 6e6d 656e 7420  rupt government 
-000035f0: 6f66 2074 6861 7420 736d 616c 6c20 7468  of that small th
-00003600: 6972 6420 776f 726c 6420 636f 756e 7472  ird world countr
-00003610: 792e 220a 2020 2020 2020 2020 2020 2020  y.".            
-00003620: 2020 2020 4e6f 7468 696e 6720 6973 2064      Nothing is d
-00003630: 6f6e 652c 206e 6f20 6368 616e 6765 7320  one, no changes 
-00003640: 6172 6520 6d61 6465 2c20 736f 6d65 2072  are made, some r
-00003650: 6963 6820 7065 6f70 6c65 2067 6574 2072  ich people get r
-00003660: 6963 6865 722e 3c2f 4933 3e0a 2020 2020  icher.</I3>.    
-00003670: 2020 2020 2020 2020 3c2f 453e 0a20 2020          </E>.   
-00003680: 2020 2020 203c 2f44 6174 613e 0a20 2020       </Data>.   
-00003690: 203c 2f4d 6561 7375 7265 6d65 6e74 3e0a   </Measurement>.
-000036a0: 3c2f 4869 6c6c 746f 703e 0a              </Hilltop>.
+00002310: 3432 3030 3c2f 4932 3e0d 0a20 2020 2020  4200</I2>..     
+00002320: 2020 2020 2020 2020 2020 203c 4933 3e38             <I3>8
+00002330: 3937 302e 393c 2f49 333e 0d0a 2020 2020  970.9</I3>..    
+00002340: 2020 2020 2020 2020 2020 2020 3c49 343e              <I4>
+00002350: 4861 6420 6120 636f 6c64 2073 6869 7665  Had a cold shive
+00002360: 7220 7275 6e20 646f 776e 206d 7920 7370  r run down my sp
+00002370: 696e 652e 2053 686f 756c 6420 6e6f 7420  ine. Should not 
+00002380: 6861 7665 2063 6f6d 6520 6865 7265 2061  have come here a
+00002390: 7420 3361 6d2e 3c2f 4934 3e0d 0a20 2020  t 3am.</I4>..   
+000023a0: 2020 2020 2020 2020 203c 2f45 3e0d 0a20           </E>.. 
+000023b0: 2020 2020 2020 2020 2020 203c 453e 0d0a             <E>..
+000023c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023d0: 3c54 3e32 3631 3933 3035 3130 303c 2f54  <T>2619305100</T
+000023e0: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
+000023f0: 2020 203c 4931 3e37 3930 302e 303c 2f49     <I1>7900.0</I
+00002400: 313e 0d0a 2020 2020 2020 2020 2020 2020  1>..            
+00002410: 2020 2020 3c49 323e 3236 3139 3330 3531      <I2>26193051
+00002420: 3030 3c2f 4932 3e0d 0a20 2020 2020 2020  00</I2>..       
+00002430: 2020 2020 2020 2020 203c 4933 3e38 3035           <I3>805
+00002440: 302e 303c 2f49 333e 0d0a 2020 2020 2020  0.0</I3>..      
+00002450: 2020 2020 2020 2020 2020 3c49 343e 4d65            <I4>Me
+00002460: 7420 616e 206f 6c64 2077 6f6d 616e 2077  t an old woman w
+00002470: 686f 2063 6c61 696d 6564 2074 6869 7320  ho claimed this 
+00002480: 7369 7465 2077 6173 206f 6e63 6520 616e  site was once an
+00002490: 2061 6e63 6965 6e74 206e 6174 6976 6520   ancient native 
+000024a0: 616d 6572 6963 616e 2062 7572 6961 6c20  american burial 
+000024b0: 6772 6f75 6e64 2e20 5365 656d 7320 756e  ground. Seems un
+000024c0: 6c69 6b65 6c79 2e3c 2f49 343e 0d0a 2020  likely.</I4>..  
+000024d0: 2020 2020 2020 2020 2020 3c2f 453e 0d0a            </E>..
+000024e0: 2020 2020 2020 2020 3c2f 4461 7461 3e0d          </Data>.
+000024f0: 0a20 2020 203c 2f4d 6561 7375 7265 6d65  .    </Measureme
+00002500: 6e74 3e0d 0a20 2020 203c 4d65 6173 7572  nt>..    <Measur
+00002510: 656d 656e 7420 5369 7465 4e61 6d65 3d22  ement SiteName="
+00002520: 4d69 6420 5374 7265 616d 2061 7420 436f  Mid Stream at Co
+00002530: 7774 6f69 6c65 7420 4661 726d 223e 0d0a  wtoilet Farm">..
+00002540: 2020 2020 2020 2020 3c44 6174 6153 6f75          <DataSou
+00002550: 7263 6520 4e61 6d65 3d22 4465 6164 2043  rce Name="Dead C
+00002560: 6f77 2043 6f6e 6365 6e74 7261 7469 6f6e  ow Concentration
+00002570: 2220 4e75 6d49 7465 6d73 3d22 3122 3e0d  " NumItems="1">.
+00002580: 0a20 2020 2020 2020 2020 2020 203c 5453  .            <TS
+00002590: 5479 7065 3e53 7464 5365 7269 6573 3c2f  Type>StdSeries</
+000025a0: 5453 5479 7065 3e0d 0a20 2020 2020 2020  TSType>..       
+000025b0: 2020 2020 203c 4461 7461 5479 7065 3e50       <DataType>P
+000025c0: 6172 7473 2070 6572 204d 696c 6c69 6f6e  arts per Million
+000025d0: 3c2f 4461 7461 5479 7065 3e0d 0a20 2020  </DataType>..   
+000025e0: 2020 2020 2020 2020 203c 496e 7465 7270           <Interp
+000025f0: 6f6c 6174 696f 6e3e 496e 6372 656d 656e  olation>Incremen
+00002600: 7461 6c3c 2f49 6e74 6572 706f 6c61 7469  tal</Interpolati
+00002610: 6f6e 3e0d 0a20 2020 2020 2020 2020 2020  on>..           
+00002620: 203c 4974 656d 466f 726d 6174 3e30 3c2f   <ItemFormat>0</
+00002630: 4974 656d 466f 726d 6174 3e0d 0a20 2020  ItemFormat>..   
+00002640: 2020 2020 2020 2020 203c 4974 656d 496e           <ItemIn
+00002650: 666f 2049 7465 6d4e 756d 6265 723d 2231  fo ItemNumber="1
+00002660: 223e 0d0a 2020 2020 2020 2020 2020 2020  ">..            
+00002670: 2020 2020 3c49 7465 6d4e 616d 653e 4465      <ItemName>De
+00002680: 6164 2043 6f77 2043 6f6e 6365 6e74 7261  ad Cow Concentra
+00002690: 7469 6f6e 3c2f 4974 656d 4e61 6d65 3e0d  tion</ItemName>.
+000026a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000026b0: 203c 4974 656d 466f 726d 6174 3e49 3c2f   <ItemFormat>I</
+000026c0: 4974 656d 466f 726d 6174 3e0d 0a20 2020  ItemFormat>..   
+000026d0: 2020 2020 2020 2020 2020 2020 203c 4469               <Di
+000026e0: 7669 736f 723e 313c 2f44 6976 6973 6f72  visor>1</Divisor
+000026f0: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
+00002700: 2020 203c 556e 6974 733e 7070 6d3c 2f55     <Units>ppm</U
+00002710: 6e69 7473 3e0d 0a20 2020 2020 2020 2020  nits>..         
+00002720: 2020 2020 2020 203c 466f 726d 6174 3e23         <Format>#
+00002730: 233c 2f46 6f72 6d61 743e 0d0a 2020 2020  #</Format>..    
+00002740: 2020 2020 2020 2020 3c2f 4974 656d 496e          </ItemIn
+00002750: 666f 3e0d 0a20 2020 2020 2020 203c 2f44  fo>..        </D
+00002760: 6174 6153 6f75 7263 653e 0d0a 2020 2020  ataSource>..    
+00002770: 2020 2020 3c44 6174 6120 4461 7465 466f      <Data DateFo
+00002780: 726d 6174 3d22 6d6f 7773 6563 7322 204e  rmat="mowsecs" N
+00002790: 756d 4974 656d 733d 2231 223e 0d0a 2020  umItems="1">..  
+000027a0: 2020 2020 2020 2020 2020 3c45 3e0d 0a20            <E>.. 
+000027b0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+000027c0: 543e 3236 3139 3330 3234 3030 3c2f 543e  T>2619302400</T>
+000027d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000027e0: 2020 3c49 313e 313c 2f49 313e 0d0a 2020    <I1>1</I1>..  
+000027f0: 2020 2020 2020 2020 2020 3c2f 453e 0d0a            </E>..
+00002800: 2020 2020 2020 2020 2020 2020 3c45 3e0d              <E>.
+00002810: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002820: 203c 543e 3236 3139 3330 3237 3030 3c2f   <T>2619302700</
+00002830: 543e 0d0a 2020 2020 2020 2020 2020 2020  T>..            
+00002840: 2020 2020 3c49 313e 373c 2f49 313e 0d0a      <I1>7</I1>..
+00002850: 2020 2020 2020 2020 2020 2020 3c2f 453e              </E>
+00002860: 0d0a 2020 2020 2020 2020 2020 2020 3c45  ..            <E
+00002870: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
+00002880: 2020 203c 543e 3236 3139 3330 3330 3030     <T>2619303000
+00002890: 3c2f 543e 0d0a 2020 2020 2020 2020 2020  </T>..          
+000028a0: 2020 2020 2020 3c49 313e 313c 2f49 313e        <I1>1</I1>
+000028b0: 0d0a 2020 2020 2020 2020 2020 2020 3c2f  ..            </
+000028c0: 453e 0d0a 2020 2020 2020 2020 2020 2020  E>..            
+000028d0: 3c45 3e0d 0a20 2020 2020 2020 2020 2020  <E>..           
+000028e0: 2020 2020 203c 543e 3236 3139 3330 3333       <T>26193033
+000028f0: 3030 3c2f 543e 0d0a 2020 2020 2020 2020  00</T>..        
+00002900: 2020 2020 2020 2020 3c49 313e 313c 2f49          <I1>1</I
+00002910: 313e 0d0a 2020 2020 2020 2020 2020 2020  1>..            
+00002920: 3c2f 453e 0d0a 2020 2020 2020 2020 2020  </E>..          
+00002930: 2020 3c45 3e0d 0a20 2020 2020 2020 2020    <E>..         
+00002940: 2020 2020 2020 203c 543e 3236 3139 3330         <T>261930
+00002950: 3336 3030 3c2f 543e 0d0a 2020 2020 2020  3600</T>..      
+00002960: 2020 2020 2020 2020 2020 3c49 313e 313c            <I1>1<
+00002970: 2f49 313e 0d0a 2020 2020 2020 2020 2020  /I1>..          
+00002980: 2020 3c2f 453e 0d0a 2020 2020 2020 2020    </E>..        
+00002990: 2020 2020 3c45 3e0d 0a20 2020 2020 2020      <E>..       
+000029a0: 2020 2020 2020 2020 203c 543e 3236 3139           <T>2619
+000029b0: 3330 3339 3030 3c2f 543e 0d0a 2020 2020  303900</T>..    
+000029c0: 2020 2020 2020 2020 2020 2020 3c49 313e              <I1>
+000029d0: 313c 2f49 313e 0d0a 2020 2020 2020 2020  1</I1>..        
+000029e0: 2020 2020 3c2f 453e 0d0a 2020 2020 2020      </E>..      
+000029f0: 2020 2020 2020 3c45 3e0d 0a20 2020 2020        <E>..     
+00002a00: 2020 2020 2020 2020 2020 203c 543e 3236             <T>26
+00002a10: 3139 3330 3432 3030 3c2f 543e 0d0a 2020  19304200</T>..  
+00002a20: 2020 2020 2020 2020 2020 2020 2020 3c49                <I
+00002a30: 313e 363c 2f49 313e 0d0a 2020 2020 2020  1>6</I1>..      
+00002a40: 2020 2020 2020 3c2f 453e 0d0a 2020 2020        </E>..    
+00002a50: 2020 2020 2020 2020 3c45 3e0d 0a20 2020          <E>..   
+00002a60: 2020 2020 2020 2020 2020 2020 203c 543e               <T>
+00002a70: 3236 3139 3330 3435 3030 3c2f 543e 0d0a  2619304500</T>..
+00002a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a90: 3c49 313e 363c 2f49 313e 0d0a 2020 2020  <I1>6</I1>..    
+00002aa0: 2020 2020 2020 2020 3c2f 453e 0d0a 2020          </E>..  
+00002ab0: 2020 2020 2020 2020 2020 3c45 3e0d 0a20            <E>.. 
+00002ac0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00002ad0: 543e 3236 3139 3330 3438 3030 3c2f 543e  T>2619304800</T>
+00002ae0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002af0: 2020 3c49 313e 393c 2f49 313e 0d0a 2020    <I1>9</I1>..  
+00002b00: 2020 2020 2020 2020 2020 3c2f 453e 0d0a            </E>..
+00002b10: 2020 2020 2020 2020 2020 2020 3c45 3e0d              <E>.
+00002b20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002b30: 203c 543e 3236 3139 3330 3531 3030 3c2f   <T>2619305100</
+00002b40: 543e 0d0a 2020 2020 2020 2020 2020 2020  T>..            
+00002b50: 2020 2020 3c49 313e 343c 2f49 313e 0d0a      <I1>4</I1>..
+00002b60: 2020 2020 2020 2020 2020 2020 3c2f 453e              </E>
+00002b70: 0d0a 2020 2020 2020 2020 3c2f 4461 7461  ..        </Data
+00002b80: 3e0d 0a20 2020 203c 2f4d 6561 7375 7265  >..    </Measure
+00002b90: 6d65 6e74 3e0d 0a20 2020 203c 4d65 6173  ment>..    <Meas
+00002ba0: 7572 656d 656e 7420 5369 7465 4e61 6d65  urement SiteName
+00002bb0: 3d22 4d69 6420 5374 7265 616d 2061 7420  ="Mid Stream at 
+00002bc0: 436f 7774 6f69 6c65 7420 4661 726d 223e  Cowtoilet Farm">
+00002bd0: 0d0a 2020 2020 2020 2020 3c44 6174 6153  ..        <DataS
+00002be0: 6f75 7263 6520 4e61 6d65 3d22 4465 6164  ource Name="Dead
+00002bf0: 2043 6f77 2043 6f6e 6365 6e74 7261 7469   Cow Concentrati
+00002c00: 6f6e 2220 4e75 6d49 7465 6d73 3d22 3122  on" NumItems="1"
+00002c10: 3e0d 0a20 2020 2020 2020 2020 2020 203c  >..            <
+00002c20: 5453 5479 7065 3e53 7464 5175 616c 5365  TSType>StdQualSe
+00002c30: 7269 6573 3c2f 5453 5479 7065 3e0d 0a20  ries</TSType>.. 
+00002c40: 2020 2020 2020 2020 2020 203c 4461 7461             <Data
+00002c50: 5479 7065 3e44 6561 6420 436f 7773 3c2f  Type>Dead Cows</
+00002c60: 4461 7461 5479 7065 3e0d 0a20 2020 2020  DataType>..     
+00002c70: 2020 2020 2020 203c 496e 7465 7270 6f6c         <Interpol
+00002c80: 6174 696f 6e3e 4576 656e 743c 2f49 6e74  ation>Event</Int
+00002c90: 6572 706f 6c61 7469 6f6e 3e0d 0a20 2020  erpolation>..   
+00002ca0: 2020 2020 2020 2020 203c 4974 656d 466f           <ItemFo
+00002cb0: 726d 6174 3e30 3c2f 4974 656d 466f 726d  rmat>0</ItemForm
+00002cc0: 6174 3e0d 0a20 2020 2020 2020 203c 2f44  at>..        </D
+00002cd0: 6174 6153 6f75 7263 653e 0d0a 2020 2020  ataSource>..    
+00002ce0: 2020 2020 3c44 6174 6120 4461 7465 466f      <Data DateFo
+00002cf0: 726d 6174 3d22 6d6f 7773 6563 7322 204e  rmat="mowsecs" N
+00002d00: 756d 4974 656d 733d 2231 223e 0d0a 2020  umItems="1">..  
+00002d10: 2020 2020 2020 2020 2020 3c45 3e0d 0a20            <E>.. 
+00002d20: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00002d30: 543e 3236 3139 3330 3233 3939 3c2f 543e  T>2619302399</T>
+00002d40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002d50: 2020 3c49 313e 3630 303c 2f49 313e 0d0a    <I1>600</I1>..
+00002d60: 2020 2020 2020 2020 2020 2020 3c2f 453e              </E>
+00002d70: 0d0a 2020 2020 2020 2020 3c2f 4461 7461  ..        </Data
+00002d80: 3e0d 0a20 2020 203c 2f4d 6561 7375 7265  >..    </Measure
+00002d90: 6d65 6e74 3e0d 0a20 2020 203c 4d65 6173  ment>..    <Meas
+00002da0: 7572 656d 656e 7420 5369 7465 4e61 6d65  urement SiteName
+00002db0: 3d22 4d69 6420 5374 7265 616d 2061 7420  ="Mid Stream at 
+00002dc0: 436f 7774 6f69 6c65 7420 4661 726d 223e  Cowtoilet Farm">
+00002dd0: 0d0a 2020 2020 2020 2020 3c44 6174 6153  ..        <DataS
+00002de0: 6f75 7263 6520 4e61 6d65 3d22 4465 6164  ource Name="Dead
+00002df0: 2043 6f77 2043 6f6e 6365 6e74 7261 7469   Cow Concentrati
+00002e00: 6f6e 2220 4e75 6d49 7465 6d73 3d22 3322  on" NumItems="3"
+00002e10: 3e0d 0a20 2020 2020 2020 2020 2020 203c  >..            <
+00002e20: 5453 5479 7065 3e43 6865 636b 5365 7269  TSType>CheckSeri
+00002e30: 6573 3c2f 5453 5479 7065 3e0d 0a20 2020  es</TSType>..   
+00002e40: 2020 2020 2020 2020 203c 4461 7461 5479           <DataTy
+00002e50: 7065 3e44 6561 6420 436f 7773 3c2f 4461  pe>Dead Cows</Da
+00002e60: 7461 5479 7065 3e0d 0a20 2020 2020 2020  taType>..       
+00002e70: 2020 2020 203c 496e 7465 7270 6f6c 6174       <Interpolat
+00002e80: 696f 6e3e 4469 7363 7265 7465 3c2f 496e  ion>Discrete</In
+00002e90: 7465 7270 6f6c 6174 696f 6e3e 0d0a 2020  terpolation>..  
+00002ea0: 2020 2020 2020 2020 2020 3c49 7465 6d46            <ItemF
+00002eb0: 6f72 6d61 743e 3134 303c 2f49 7465 6d46  ormat>140</ItemF
+00002ec0: 6f72 6d61 743e 0d0a 2020 2020 2020 2020  ormat>..        
+00002ed0: 2020 2020 3c49 7465 6d49 6e66 6f20 4974      <ItemInfo It
+00002ee0: 656d 4e75 6d62 6572 3d22 3122 3e0d 0a20  emNumber="1">.. 
+00002ef0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00002f00: 4974 656d 4e61 6d65 3e44 6561 6420 436f  ItemName>Dead Co
+00002f10: 7720 436f 6e63 656e 7472 6174 696f 6e3c  w Concentration<
+00002f20: 2f49 7465 6d4e 616d 653e 0d0a 2020 2020  /ItemName>..    
+00002f30: 2020 2020 2020 2020 2020 2020 3c49 7465              <Ite
+00002f40: 6d46 6f72 6d61 743e 493c 2f49 7465 6d46  mFormat>I</ItemF
+00002f50: 6f72 6d61 743e 0d0a 2020 2020 2020 2020  ormat>..        
+00002f60: 2020 2020 2020 2020 3c44 6976 6973 6f72          <Divisor
+00002f70: 3e31 3c2f 4469 7669 736f 723e 0d0a 2020  >1</Divisor>..  
+00002f80: 2020 2020 2020 2020 2020 2020 2020 3c55                <U
+00002f90: 6e69 7473 3e70 706d 3c2f 556e 6974 733e  nits>ppm</Units>
+00002fa0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002fb0: 2020 3c46 6f72 6d61 743e 2323 3c2f 466f    <Format>##</Fo
+00002fc0: 726d 6174 3e0d 0a20 2020 2020 2020 2020  rmat>..         
+00002fd0: 2020 203c 2f49 7465 6d49 6e66 6f3e 0d0a     </ItemInfo>..
+00002fe0: 2020 2020 2020 2020 2020 2020 3c49 7465              <Ite
+00002ff0: 6d49 6e66 6f20 4974 656d 4e75 6d62 6572  mInfo ItemNumber
+00003000: 3d22 3222 3e0d 0a20 2020 2020 2020 2020  ="2">..         
+00003010: 2020 2020 2020 203c 4974 656d 4e61 6d65         <ItemName
+00003020: 3e52 6563 6f72 6465 7220 5469 6d65 3c2f  >Recorder Time</
+00003030: 4974 656d 4e61 6d65 3e0d 0a20 2020 2020  ItemName>..     
+00003040: 2020 2020 2020 2020 2020 203c 4974 656d             <Item
+00003050: 466f 726d 6174 3e44 3c2f 4974 656d 466f  Format>D</ItemFo
+00003060: 726d 6174 3e0d 0a20 2020 2020 2020 2020  rmat>..         
+00003070: 2020 2020 2020 203c 4469 7669 736f 723e         <Divisor>
+00003080: 313c 2f44 6976 6973 6f72 3e0d 0a20 2020  1</Divisor>..   
+00003090: 2020 2020 2020 2020 2020 2020 203c 556e               <Un
+000030a0: 6974 7320 2f3e 0d0a 2020 2020 2020 2020  its />..        
+000030b0: 2020 2020 2020 2020 3c46 6f72 6d61 743e          <Format>
+000030c0: 2323 233c 2f46 6f72 6d61 743e 0d0a 2020  ###</Format>..  
+000030d0: 2020 2020 2020 2020 2020 3c2f 4974 656d            </Item
+000030e0: 496e 666f 3e0d 0a20 2020 2020 2020 2020  Info>..         
+000030f0: 2020 203c 4974 656d 496e 666f 2049 7465     <ItemInfo Ite
+00003100: 6d4e 756d 6265 723d 2233 223e 0d0a 2020  mNumber="3">..  
+00003110: 2020 2020 2020 2020 2020 2020 2020 3c49                <I
+00003120: 7465 6d4e 616d 653e 436f 6d6d 656e 743c  temName>Comment<
+00003130: 2f49 7465 6d4e 616d 653e 0d0a 2020 2020  /ItemName>..    
+00003140: 2020 2020 2020 2020 2020 2020 3c49 7465              <Ite
+00003150: 6d46 6f72 6d61 743e 533c 2f49 7465 6d46  mFormat>S</ItemF
+00003160: 6f72 6d61 743e 0d0a 2020 2020 2020 2020  ormat>..        
+00003170: 2020 2020 2020 2020 3c44 6976 6973 6f72          <Divisor
+00003180: 3e31 3c2f 4469 7669 736f 723e 0d0a 2020  >1</Divisor>..  
+00003190: 2020 2020 2020 2020 2020 2020 2020 3c55                <U
+000031a0: 6e69 7473 202f 3e0d 0a20 2020 2020 2020  nits />..       
+000031b0: 2020 2020 2020 2020 203c 466f 726d 6174           <Format
+000031c0: 3e23 2323 3c2f 466f 726d 6174 3e0d 0a20  >###</Format>.. 
+000031d0: 2020 2020 2020 2020 2020 203c 2f49 7465             </Ite
+000031e0: 6d49 6e66 6f3e 0d0a 2020 2020 2020 2020  mInfo>..        
+000031f0: 3c2f 4461 7461 536f 7572 6365 3e0d 0a20  </DataSource>.. 
+00003200: 2020 2020 2020 203c 4461 7461 2044 6174         <Data Dat
+00003210: 6546 6f72 6d61 743d 226d 6f77 7365 6373  eFormat="mowsecs
+00003220: 2220 4e75 6d49 7465 6d73 3d22 3322 3e0d  " NumItems="3">.
+00003230: 0a20 2020 2020 2020 2020 2020 203c 453e  .            <E>
+00003240: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003250: 2020 3c54 3e32 3631 3933 3032 3430 303c    <T>2619302400<
+00003260: 2f54 3e0d 0a20 2020 2020 2020 2020 2020  /T>..           
+00003270: 2020 2020 203c 4931 3e35 3c2f 4931 3e0d       <I1>5</I1>.
+00003280: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003290: 203c 4932 3e32 3631 3933 3032 3430 303c   <I2>2619302400<
+000032a0: 2f49 323e 0d0a 2020 2020 2020 2020 2020  /I2>..          
+000032b0: 2020 2020 2020 3c49 333e 0d0a 2020 2020        <I3>..    
+000032c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000032d0: 4361 7262 6f6e 206f 6666 7365 7473 2061  Carbon offsets a
+000032e0: 7265 2061 206d 6173 7369 7665 2073 6361  re a massive sca
+000032f0: 6d2e 0d0a 2020 2020 2020 2020 2020 2020  m...            
+00003300: 2020 2020 3c2f 4933 3e0d 0a20 2020 2020      </I3>..     
+00003310: 2020 2020 2020 203c 2f45 3e0d 0a20 2020         </E>..   
+00003320: 2020 2020 2020 2020 203c 453e 0d0a 2020           <E>..  
+00003330: 2020 2020 2020 2020 2020 2020 2020 3c54                <T
+00003340: 3e32 3631 3933 3033 3030 303c 2f54 3e0d  >2619303000</T>.
+00003350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003360: 203c 4931 3e33 3c2f 4931 3e0d 0a20 2020   <I1>3</I1>..   
+00003370: 2020 2020 2020 2020 2020 2020 203c 4932               <I2
+00003380: 3e32 3631 3933 3033 3030 303c 2f49 323e  >2619303000</I2>
+00003390: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000033a0: 2020 3c49 333e 0d0a 2020 2020 2020 2020    <I3>..        
+000033b0: 2020 2020 2020 2020 2020 2020 2243 6172              "Car
+000033c0: 626f 6e20 6372 6564 6974 7322 2061 7265  bon credits" are
+000033d0: 206e 6f74 6869 6e67 206d 6f72 6520 7468   nothing more th
+000033e0: 616e 2061 2066 7265 6520 7469 636b 6574  an a free ticket
+000033f0: 2074 6f20 706f 6c6c 7574 6520 696e 2072   to pollute in r
+00003400: 6574 7572 6e20 666f 7220 6120 7072 6f6d  eturn for a prom
+00003410: 6973 6520 7468 6174 2061 2070 6965 6365  ise that a piece
+00003420: 206f 6620 666f 7265 7374 2069 7320 7072   of forest is pr
+00003430: 6573 6572 7665 642e 0d0a 2020 2020 2020  eserved...      
+00003440: 2020 2020 2020 2020 2020 3c2f 4933 3e0d            </I3>.
+00003450: 0a20 2020 2020 2020 2020 2020 203c 2f45  .            </E
+00003460: 3e0d 0a20 2020 2020 2020 2020 2020 203c  >..            <
+00003470: 453e 0d0a 2020 2020 2020 2020 2020 2020  E>..            
+00003480: 2020 2020 3c54 3e32 3631 3933 3033 3930      <T>261930390
+00003490: 303c 2f54 3e0d 0a20 2020 2020 2020 2020  0</T>..         
+000034a0: 2020 2020 2020 203c 4931 3e31 3c2f 4931         <I1>1</I1
+000034b0: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
+000034c0: 2020 203c 4932 3e32 3631 3933 3033 3930     <I2>261930390
+000034d0: 303c 2f49 323e 0d0a 2020 2020 2020 2020  0</I2>..        
+000034e0: 2020 2020 2020 2020 3c49 333e 5052 4553          <I3>PRES
+000034f0: 4552 5645 442c 206e 6f74 2072 6573 746f  ERVED, not resto
+00003500: 7265 642e 2049 6e20 6d6f 7374 2063 6173  red. In most cas
+00003510: 6573 2c20 616c 6c20 7468 6520 6d6f 6e65  es, all the mone
+00003520: 7920 7468 6174 2064 6f65 7320 6e6f 7420  y that does not 
+00003530: 676f 2074 6f77 6172 6473 206d 6964 646c  go towards middl
+00003540: 656d 656e 2c20 676f 2074 6f77 6172 6473  emen, go towards
+00003550: 2070 7265 7665 6e74 696e 6720 616e 2061   preventing an a
+00003560: 6c72 6561 6479 2070 726f 7465 6374 6564  lready protected
+00003570: 2066 6f72 6573 7420 6672 6f6d 2062 6569   forest from bei
+00003580: 6e67 2063 7574 2064 6f77 6e20 6261 7365  ng cut down base
+00003590: 6420 6f6e 206d 6173 7369 7665 6c79 206f  d on massively o
+000035a0: 7665 7262 6c6f 776e 2070 6f70 756c 6174  verblown populat
+000035b0: 696f 6e20 616e 642f 6f72 2065 636f 6e6f  ion and/or econo
+000035c0: 6d69 6320 6772 6f77 7468 2065 7374 696d  mic growth estim
+000035d0: 6174 6573 2e3c 2f49 333e 0d0a 2020 2020  ates.</I3>..    
+000035e0: 2020 2020 2020 2020 3c2f 453e 0d0a 2020          </E>..  
+000035f0: 2020 2020 2020 2020 2020 3c45 3e0d 0a20            <E>.. 
+00003600: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00003610: 543e 3236 3139 3330 3438 3030 3c2f 543e  T>2619304800</T>
+00003620: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003630: 2020 3c49 313e 343c 2f49 313e 0d0a 2020    <I1>4</I1>..  
+00003640: 2020 2020 2020 2020 2020 2020 2020 3c49                <I
+00003650: 323e 3236 3139 3330 3438 3030 3c2f 4932  2>2619304800</I2
+00003660: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
+00003670: 2020 203c 4933 3e49 6e20 6573 7365 6e63     <I3>In essenc
+00003680: 653a 2022 4361 6e20 7765 2070 6f6c 6c75  e: "Can we pollu
+00003690: 7465 3f20 5765 2077 696c 6c20 6769 7665  te? We will give
+000036a0: 2073 6f6d 6520 6d6f 6e65 7920 746f 2074   some money to t
+000036b0: 6869 7320 7065 7273 6f6e 2077 686f 2077  his person who w
+000036c0: 696c 6c20 7573 6520 7468 6174 206d 6f6e  ill use that mon
+000036d0: 6579 2074 6f20 6f76 6572 6573 7469 6d61  ey to overestima
+000036e0: 7465 2074 6865 2070 6f74 656e 7469 616c  te the potential
+000036f0: 2064 616d 6167 6520 746f 2061 2064 6973   damage to a dis
+00003700: 7461 6e74 2074 696e 7920 6368 756e 6b20  tant tiny chunk 
+00003710: 6f66 2072 6169 6e66 6f72 6573 7420 7468  of rainforest th
+00003720: 6174 2069 7320 616c 7265 6164 7920 7072  at is already pr
+00003730: 6f74 6563 7465 642e 2054 6865 2073 6d61  otected. The sma
+00003740: 6c6c 2061 6d6f 756e 7420 6f66 206c 6566  ll amount of lef
+00003750: 746f 7665 7220 6d6f 6e65 7920 6361 6e20  tover money can 
+00003760: 7468 656e 2067 6f20 746f 2074 6865 2063  then go to the c
+00003770: 6f72 7275 7074 2067 6f76 6572 6e6d 656e  orrupt governmen
+00003780: 7420 6f66 2074 6861 7420 736d 616c 6c20  t of that small 
+00003790: 7468 6972 6420 776f 726c 6420 636f 756e  third world coun
+000037a0: 7472 792e 220d 0a20 2020 2020 2020 2020  try."..         
+000037b0: 2020 2020 2020 204e 6f74 6869 6e67 2069         Nothing i
+000037c0: 7320 646f 6e65 2c20 6e6f 2063 6861 6e67  s done, no chang
+000037d0: 6573 2061 7265 206d 6164 652c 2073 6f6d  es are made, som
+000037e0: 6520 7269 6368 2070 656f 706c 6520 6765  e rich people ge
+000037f0: 7420 7269 6368 6572 2e3c 2f49 333e 0d0a  t richer.</I3>..
+00003800: 2020 2020 2020 2020 2020 2020 3c2f 453e              </E>
+00003810: 0d0a 2020 2020 2020 2020 3c2f 4461 7461  ..        </Data
+00003820: 3e0d 0a20 2020 203c 2f4d 6561 7375 7265  >..    </Measure
+00003830: 6d65 6e74 3e0d 0a3c 2f48 696c 6c74 6f70  ment>..</Hilltop
+00003840: 3e0d 0a                                  >..
```

