# Comparing `tmp/galaxy-util-23.2.dev0.tar.gz` & `tmp/galaxy-util-24.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy-util-23.2.dev0.tar", last modified: Fri Dec  8 17:38:26 2023, max compression
+gzip compressed data, was "galaxy-util-24.0.0.tar", last modified: Wed Apr  3 02:43:58 2024, max compression
```

## Comparing `galaxy-util-23.2.dev0.tar` & `galaxy-util-24.0.0.tar`

### file list

```diff
@@ -1,98 +1,99 @@
-drwxr-xr-x   0 mvandenb   (501) wheel        (0)        0 2023-12-08 17:38:26.451256 galaxy-util-23.2.dev0/
--rw-r--r--   0 mvandenb   (501) wheel        (0)     5189 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/HISTORY.rst
--rw-r--r--   0 mvandenb   (501) wheel        (0)    12875 2023-12-08 17:18:17.000000 galaxy-util-23.2.dev0/LICENSE
--rw-r--r--   0 mvandenb   (501) wheel        (0)      163 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/MANIFEST.in
--rw-r--r--   0 mvandenb   (501) wheel        (0)     6980 2023-12-08 17:38:26.451193 galaxy-util-23.2.dev0/PKG-INFO
--rw-r--r--   0 mvandenb   (501) wheel        (0)      242 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/README.rst
--rw-r--r--   0 mvandenb   (501) wheel        (0)       89 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/dev-requirements.txt
-drwxr-xr-x   0 mvandenb   (501) wheel        (0)        0 2023-12-08 17:38:26.435036 galaxy-util-23.2.dev0/galaxy/
--rw-r--r--   0 mvandenb   (501) wheel        (0)       91 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/__init__.py
-drwxr-xr-x   0 mvandenb   (501) wheel        (0)        0 2023-12-08 17:38:26.435988 galaxy-util-23.2.dev0/galaxy/exceptions/
--rw-r--r--   0 mvandenb   (501) wheel        (0)     8388 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/exceptions/__init__.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     6062 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/exceptions/error_codes.json
--rw-r--r--   0 mvandenb   (501) wheel        (0)     1910 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/exceptions/error_codes.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)        0 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/py.typed
-drwxr-xr-x   0 mvandenb   (501) wheel        (0)        0 2023-12-08 17:38:26.447883 galaxy-util-23.2.dev0/galaxy/util/
--rw-r--r--   0 mvandenb   (501) wheel        (0)    61039 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/__init__.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)      872 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/aliaspickler.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     5746 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/bool_expressions.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     1086 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/bunch.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     1881 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/bytesize.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     5938 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/checkers.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     6383 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/commands.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)    13411 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/compression_utils.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)      680 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/config_parsers.py
-drwxr-xr-x   0 mvandenb   (501) wheel        (0)        0 2023-12-08 17:38:26.448243 galaxy-util-23.2.dev0/galaxy/util/custom_logging/
--rw-r--r--   0 mvandenb   (501) wheel        (0)      413 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/custom_logging/__init__.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     1377 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/custom_logging/fluent_log.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     2496 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/dictifiable.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)        9 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/docutils_template.txt
--rw-r--r--   0 mvandenb   (501) wheel        (0)     5513 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/drs.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)      225 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/dynamic.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     1542 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/expressions.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     1935 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/facts.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     2606 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/filelock.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     5469 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/form_builder.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     4303 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/hash_util.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     8119 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/heartbeat.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)      873 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/image_util.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     4961 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/inflection.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     7167 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/json.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     6284 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/jstree.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     1628 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/lazy_process.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)      391 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/markdown.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     1525 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/monitors.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     2545 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/odict.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     1708 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/oset.py
-drwxr-xr-x   0 mvandenb   (501) wheel        (0)        0 2023-12-08 17:38:26.448770 galaxy-util-23.2.dev0/galaxy/util/path/
--rw-r--r--   0 mvandenb   (501) wheel        (0)    16890 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/path/__init__.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)      204 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/path/ntpath.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)      208 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/path/posixpath.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     3940 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/permutations.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     4756 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/plugin_config.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     7913 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/properties.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     1601 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/renamed_temporary_file.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     1123 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/resources.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     2114 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/rst_to_html.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)    18165 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/rules_dsl.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)    11738 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/rules_dsl_spec.yml
--rw-r--r--   0 mvandenb   (501) wheel        (0)     3716 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/sanitize_html.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     3654 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/script.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     3717 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/search.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     4616 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/simplegraph.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)      619 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/sleeper.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     1678 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/sockets.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)      557 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/specs.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)      745 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/sqlite.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     1735 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/submodules.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     1362 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/task.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     6170 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/template.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)      614 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/themes.py
-drwxr-xr-x   0 mvandenb   (501) wheel        (0)        0 2023-12-08 17:38:26.449558 galaxy-util-23.2.dev0/galaxy/util/tool_shed/
--rw-r--r--   0 mvandenb   (501) wheel        (0)        0 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/tool_shed/__init__.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)    12130 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/tool_shed/common_util.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)      930 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/tool_shed/encoding_util.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     4639 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/tool_shed/tool_shed_registry.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     1324 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/tool_shed/xml_util.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)      216 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/tool_version.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     6755 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/topsort.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     2110 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/tree_dict.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     1001 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/ucsc.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     1021 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/unittest.py
-drwxr-xr-x   0 mvandenb   (501) wheel        (0)        0 2023-12-08 17:38:26.449707 galaxy-util-23.2.dev0/galaxy/util/unittest_utils/
--rw-r--r--   0 mvandenb   (501) wheel        (0)     1047 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/unittest_utils/__init__.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     1115 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/validation.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     6907 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/watcher.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)    12063 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/xml_macros.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     2836 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/yaml_util.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     3261 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/util/zipstream.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)      118 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/galaxy/version.py
-drwxr-xr-x   0 mvandenb   (501) wheel        (0)        0 2023-12-08 17:38:26.450803 galaxy-util-23.2.dev0/galaxy_util.egg-info/
--rw-r--r--   0 mvandenb   (501) wheel        (0)     6980 2023-12-08 17:38:26.000000 galaxy-util-23.2.dev0/galaxy_util.egg-info/PKG-INFO
--rw-r--r--   0 mvandenb   (501) wheel        (0)     2287 2023-12-08 17:38:26.000000 galaxy-util-23.2.dev0/galaxy_util.egg-info/SOURCES.txt
--rw-r--r--   0 mvandenb   (501) wheel        (0)        1 2023-12-08 17:38:26.000000 galaxy-util-23.2.dev0/galaxy_util.egg-info/dependency_links.txt
--rw-r--r--   0 mvandenb   (501) wheel        (0)      165 2023-12-08 17:38:26.000000 galaxy-util-23.2.dev0/galaxy_util.egg-info/requires.txt
--rw-r--r--   0 mvandenb   (501) wheel        (0)        7 2023-12-08 17:38:26.000000 galaxy-util-23.2.dev0/galaxy_util.egg-info/top_level.txt
--rw-r--r--   0 mvandenb   (501) wheel        (0)       81 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/pyproject.toml
--rw-r--r--   0 mvandenb   (501) wheel        (0)     1356 2023-12-08 17:38:26.451515 galaxy-util-23.2.dev0/setup.cfg
--rw-r--r--   0 mvandenb   (501) wheel        (0)       35 2023-12-08 17:18:18.000000 galaxy-util-23.2.dev0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:58.010371 galaxy-util-24.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     9006 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10891 2024-04-03 02:43:58.010371 galaxy-util-24.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:57.994371 galaxy-util-24.0.0/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:57.994371 galaxy-util-24.0.0/galaxy/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)     8388 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6062 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/exceptions/error_codes.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/exceptions/error_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/exceptions/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:58.006371 galaxy-util-24.0.0/galaxy/util/
+-rw-r--r--   0 runner    (1001) docker     (127)    63297 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/aliaspickler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/bool_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/bunch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/bytesize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/checkers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16988 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/compression_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/config_parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:58.006371 galaxy-util-24.0.0/galaxy/util/custom_logging/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/custom_logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/custom_logging/fluent_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/dictifiable.py
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/docutils_template.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5513 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/drs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/facts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/filelock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/form_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/hash_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8119 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/image_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4961 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/inflection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7167 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/jstree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/lazy_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/monitors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/odict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/oset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:58.006371 galaxy-util-24.0.0/galaxy/util/path/
+-rw-r--r--   0 runner    (1001) docker     (127)    16890 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/path/ntpath.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/path/posixpath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/permutations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/plugin_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7914 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/renamed_temporary_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/rst_to_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18165 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/rules_dsl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11738 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/rules_dsl_spec.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/sanitize_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/simplegraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/sleeper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/sockets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/specs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/submodules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/themes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:58.006371 galaxy-util-24.0.0/galaxy/util/tool_shed/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/tool_shed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12130 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/tool_shed/common_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/tool_shed/encoding_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/tool_shed/tool_shed_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/tool_shed/xml_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/tool_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/topsort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/tree_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/ucsc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/unittest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:58.006371 galaxy-util-24.0.0/galaxy/util/unittest_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/unittest_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11865 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/xml_macros.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/yaml_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/util/zipstream.py
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/galaxy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:58.010371 galaxy-util-24.0.0/galaxy_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10891 2024-04-03 02:43:57.000000 galaxy-util-24.0.0/galaxy_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-03 02:43:57.000000 galaxy-util-24.0.0/galaxy_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:43:57.000000 galaxy-util-24.0.0/galaxy_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-03 02:43:57.000000 galaxy-util-24.0.0/galaxy_util.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:43:57.000000 galaxy-util-24.0.0/galaxy_util.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-03 02:43:58.010371 galaxy-util-24.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-03 02:43:42.000000 galaxy-util-24.0.0/test-requirements.txt
```

### Comparing `galaxy-util-23.2.dev0/HISTORY.rst` & `galaxy-util-24.0.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,132 @@
+Metadata-Version: 2.1
+Name: galaxy-util
+Version: 24.0.0
+Summary: Galaxy generic utilities
+Home-page: https://github.com/galaxyproject/galaxy
+Author: Galaxy Project and Community
+Author-email: galaxy-committers@lists.galaxyproject.org
+License: AFL
+Keywords: Galaxy
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Academic Free License (AFL)
+Classifier: Natural Language :: English
+Classifier: Operating System :: POSIX
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Code Generators
+Classifier: Topic :: Software Development :: Testing
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: bleach
+Requires-Dist: boltons
+Requires-Dist: docutils!=0.17,!=0.17.1
+Requires-Dist: importlib-resources; python_version < "3.9"
+Requires-Dist: packaging
+Requires-Dist: pyparsing
+Requires-Dist: PyYAML
+Requires-Dist: requests
+Requires-Dist: Routes
+Requires-Dist: typing-extensions
+Requires-Dist: zipstream-new
+Provides-Extra: jstree
+Requires-Dist: dictobj; extra == "jstree"
+Provides-Extra: template
+Requires-Dist: Cheetah3; extra == "template"
+Requires-Dist: future>=1.0.0; extra == "template"
+
+
+.. image:: https://badge.fury.io/py/galaxy-util.svg
+   :target: https://pypi.org/project/galaxy-util/
+
+
+Overview
+--------
+
+The Galaxy_ utilities module.
+
+* Code: https://github.com/galaxyproject/galaxy
+
+.. _Galaxy: http://galaxyproject.org/
+
 History
 -------
 
 .. to_doc
 
--------
-23.2rc1
--------
+-------------------
+24.0.0 (2024-04-02)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Optional Reply-to SMTP header in tool error reports by `@neoformit <https://github.com/neoformit>`_ in `#17243 <https://github.com/galaxyproject/galaxy/pull/17243>`_
+* Follow-up on #17274 and #17262 by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17302 <https://github.com/galaxyproject/galaxy/pull/17302>`_
+* Fixes for flake8-bugbear 24.1.17 by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17340 <https://github.com/galaxyproject/galaxy/pull/17340>`_
+
+============
+Enhancements
+============
 
+* Add support for Python 3.12 by `@tuncK <https://github.com/tuncK>`_ in `#16796 <https://github.com/galaxyproject/galaxy/pull/16796>`_
+* Python 3.8 as minimum by `@mr-c <https://github.com/mr-c>`_ in `#16954 <https://github.com/galaxyproject/galaxy/pull/16954>`_
+* Remove web framework dependency from tools by `@davelopez <https://github.com/davelopez>`_ in `#17058 <https://github.com/galaxyproject/galaxy/pull/17058>`_
+* Add support for (fast5.tar).xz binary compressed files by `@tuncK <https://github.com/tuncK>`_ in `#17106 <https://github.com/galaxyproject/galaxy/pull/17106>`_
+* Reuse test instance during non-integration tests by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17234 <https://github.com/galaxyproject/galaxy/pull/17234>`_
+* Add OIDC backend configuration schema and validation by `@uwwint <https://github.com/uwwint>`_ in `#17274 <https://github.com/galaxyproject/galaxy/pull/17274>`_
+* Enable ``warn_unreachable`` mypy option by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17365 <https://github.com/galaxyproject/galaxy/pull/17365>`_
+* Fix type annotation of code using XML etree by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17367 <https://github.com/galaxyproject/galaxy/pull/17367>`_
+* Update to black 2024 stable style by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17391 <https://github.com/galaxyproject/galaxy/pull/17391>`_
+* Add `image_diff` comparison method for test output verification using images by `@kostrykin <https://github.com/kostrykin>`_ in `#17556 <https://github.com/galaxyproject/galaxy/pull/17556>`_
 
+-------------------
+23.2.1 (2024-02-21)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Ruff and flake8 fixes by `@nsoranzo <https://github.com/nsoranzo>`_ in `#16884 <https://github.com/galaxyproject/galaxy/pull/16884>`_
+
+============
+Enhancements
+============
+
+* Tool Shed 2.0 by `@jmchilton <https://github.com/jmchilton>`_ in `#15639 <https://github.com/galaxyproject/galaxy/pull/15639>`_
+* Move database access code out of ``galaxy.util`` by `@jdavcs <https://github.com/jdavcs>`_ in `#16526 <https://github.com/galaxyproject/galaxy/pull/16526>`_
+* Tweak tool memory use and optimize shared memory when using preload by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16536 <https://github.com/galaxyproject/galaxy/pull/16536>`_
+* Updated path-based interactive tools with entry point path injection, support for ITs with relative links, shortened URLs, doc and config updates including Podman job_conf by `@sveinugu <https://github.com/sveinugu>`_ in `#16795 <https://github.com/galaxyproject/galaxy/pull/16795>`_
+* Allow partial matches in workflow name tag search and search all tags for unquoted query by `@ahmedhamidawan <https://github.com/ahmedhamidawan>`_ in `#16860 <https://github.com/galaxyproject/galaxy/pull/16860>`_
+* Use python-isal for fast zip deflate compression in rocrate export by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17342 <https://github.com/galaxyproject/galaxy/pull/17342>`_
+
+=============
+Other changes
+=============
+
+* Merge 23.1 into dev by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16534 <https://github.com/galaxyproject/galaxy/pull/16534>`_
+
+-------------------
+23.1.4 (2024-01-04)
+-------------------
+
+No recorded changes since last release
 
 -------------------
 23.1.3 (2023-12-01)
 -------------------
 
 No recorded changes since last release
 
@@ -45,15 +160,14 @@
 * Fix allowlist deserialization in file sources by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16729 <https://github.com/galaxyproject/galaxy/pull/16729>`_
 * Exclude on_opened and on_closed from watcher events by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16850 <https://github.com/galaxyproject/galaxy/pull/16850>`_
 
 ============
 Enhancements
 ============
 
-* 
 * Various Tool Shed Cleanup by `@jmchilton <https://github.com/jmchilton>`_ in `#15247 <https://github.com/galaxyproject/galaxy/pull/15247>`_
 * Protection against problematic boolean parameters. by `@jmchilton <https://github.com/jmchilton>`_ in `#15493 <https://github.com/galaxyproject/galaxy/pull/15493>`_
 * Unify url handling with filesources by `@nuwang <https://github.com/nuwang>`_ in `#15497 <https://github.com/galaxyproject/galaxy/pull/15497>`_
 * Explore tool remote test data by `@davelopez <https://github.com/davelopez>`_ in `#15510 <https://github.com/galaxyproject/galaxy/pull/15510>`_
 * Drop database views by `@jdavcs <https://github.com/jdavcs>`_ in `#15876 <https://github.com/galaxyproject/galaxy/pull/15876>`_
 * Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#15890 <https://github.com/galaxyproject/galaxy/pull/15890>`_
 * Record input datasets and collections at full parameter path by `@mvdbeek <https://github.com/mvdbeek>`_ in `#15978 <https://github.com/galaxyproject/galaxy/pull/15978>`_
@@ -97,16 +211,14 @@
 -------------------
 
 
 =========
 Bug fixes
 =========
 
-* 
-* 
 * Replace httpbin service with pytest-httpserver by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16042 <https://github.com/galaxyproject/galaxy/pull/16042>`_
 
 -------------------
 22.1.2 (2022-12-08)
 -------------------
 
 * Pin packaging dependency to < 22, fixes ``LegacyVersion`` import errors
```

### Comparing `galaxy-util-23.2.dev0/LICENSE` & `galaxy-util-24.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.2.dev0/galaxy/exceptions/__init__.py` & `galaxy-util-24.0.0/galaxy/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.2.dev0/galaxy/exceptions/error_codes.json` & `galaxy-util-24.0.0/galaxy/exceptions/error_codes.json`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.2.dev0/galaxy/exceptions/error_codes.py` & `galaxy-util-24.0.0/galaxy/exceptions/error_codes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Defines the :class:`ErrorCode` class and instantiates concrete objects from JSON.
 
 See the file error_codes.json for actual error code descriptions.
 """
+
 from json import loads
 from typing import Dict
 
 from galaxy.util.resources import resource_string
 
 # Error codes are provided as a convience to Galaxy API clients, but at this
 # time they do represent part of the more stable interface. They can change
```

### Comparing `galaxy-util-23.2.dev0/galaxy/util/__init__.py` & `galaxy-util-24.0.0/galaxy/util/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,17 +31,20 @@
 )
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
 from hashlib import md5
 from os.path import relpath
 from typing import (
     Any,
+    cast,
+    Dict,
     Iterable,
     Iterator,
     List,
+    Mapping,
     Optional,
     overload,
     Tuple,
     TypeVar,
     Union,
 )
 from urllib.parse import (
@@ -53,41 +56,74 @@
 
 import requests
 from boltons.iterutils import (
     default_enter,
     remap,
 )
 from requests.adapters import HTTPAdapter
-from requests.packages.urllib3.util.retry import Retry
-from typing_extensions import Literal
+from requests.packages.urllib3.util.retry import Retry  # type: ignore[import-untyped]
+from typing_extensions import (
+    Literal,
+    Self,
+)
 
 try:
     import grp
 except ImportError:
     # For Pulsar on Windows (which does not use the function that uses grp)
     grp = None  # type: ignore[assignment]
 LXML_AVAILABLE = True
 try:
     from lxml import etree
-    from lxml.etree import _Element as Element
+
+    # lxml.etree.Element is a function that returns a new instance of the
+    # lxml.etree._Element class. This class doesn't have a proper __init__()
+    # method, so we can add a __new__() constructor that mimicks the
+    # xml.etree.ElementTree.Element initialization.
+    class Element(etree._Element):
+        def __new__(cls, tag, attrib={}, **extra) -> Self:  # noqa: B006
+            return cast(Self, etree.Element(tag, attrib, **extra))
+
+        def __iter__(self) -> Iterator[Self]:  # type: ignore[override]
+            return cast(Iterator[Self], super().__iter__())
+
+        def find(self, path: str, namespaces: Optional[Mapping[str, str]] = None) -> Union[Self, None]:
+            ret = super().find(path, namespaces)
+            if ret is not None:
+                return cast(Self, ret)
+            else:
+                return None
+
+        def findall(self, path: str, namespaces: Optional[Mapping[str, str]] = None) -> List[Self]:  # type: ignore[override]
+            return cast(List[Self], super().findall(path, namespaces))
+
+    def SubElement(parent: Element, tag: str, attrib: Optional[Dict[str, str]] = None, **extra) -> Element:
+        return cast(Element, etree.SubElement(parent, tag, attrib, **extra))
 
     # lxml.etree.ElementTree is a function that returns a new instance of the
-    # lxml.etree._ElementTree class. This class doesn't have a proper
-    # __init__() method, so we can add a __new__() constructor that mimicks
+    # lxml.etree._ElementTree class. This class doesn't have a proper __init__()
+    # method, so we can add a __new__() constructor that mimicks the
     # xml.etree.ElementTree.ElementTree initialization.
     class ElementTree(etree._ElementTree):
-        def __new__(cls, element=None, file=None) -> etree.ElementTree:
-            return etree.ElementTree(element, file=file)
+        def __new__(cls, element=None, file=None) -> Self:
+            return cast(Self, etree.ElementTree(element, file=file))
+
+        def getroot(self) -> Element:
+            return cast(Element, super().getroot())
+
+    def XML(text: Union[str, bytes]) -> Element:
+        return cast(Element, etree.XML(text))
 
 except ImportError:
     LXML_AVAILABLE = False
     import xml.etree.ElementTree as etree  # type: ignore[assignment,no-redef]
-    from xml.etree.ElementTree import (  # type: ignore[assignment]
+    from xml.etree.ElementTree import (  # type: ignore[assignment]  # noqa: F401
         Element,
         ElementTree,
+        XML,
     )
 
 from .custom_logging import get_logger
 from .inflection import Inflector
 from .path import (  # noqa: F401
     safe_contains,
     safe_makedirs,
@@ -116,37 +152,36 @@
 DATABASE_MAX_STRING_SIZE = 32768
 DATABASE_MAX_STRING_SIZE_PRETTY = "32K"
 
 DEFAULT_SOCKET_TIMEOUT = 600
 
 gzip_magic = b"\x1f\x8b"
 bz2_magic = b"BZh"
+xz_magic = b"\xfd7zXZ\x00"
 DEFAULT_ENCODING = os.environ.get("GALAXY_DEFAULT_ENCODING", "utf-8")
 NULL_CHAR = b"\x00"
 BINARY_CHARS = [NULL_CHAR]
 FILENAME_VALID_CHARS = ".,^_-()[]0123456789abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ"
 
 RW_R__R__ = stat.S_IRUSR | stat.S_IWUSR | stat.S_IRGRP | stat.S_IROTH
 RWXR_XR_X = stat.S_IRWXU | stat.S_IRGRP | stat.S_IXGRP | stat.S_IROTH | stat.S_IXOTH
 RWXRWXRWX = stat.S_IRWXU | stat.S_IRWXG | stat.S_IRWXO
 
-XML = etree.XML
-
 defaultdict = collections.defaultdict
 
 UNKNOWN = "unknown"
 
 
 def str_removeprefix(s: str, prefix: str):
     """
     str.removeprefix() equivalent for Python < 3.9
     """
     if sys.version_info >= (3, 9):
         return s.removeprefix(prefix)
-    if s.startswith(prefix):
+    if s.startswith(prefix):  # type: ignore[unreachable]
         return s[len(prefix) :]
     return s
 
 
 def remove_protocol_from_url(url):
     """Supplied URL may be null, if not ensure http:// or https://
     etc... is stripped off.
@@ -290,47 +325,62 @@
     >>> len(set(ids))
     1000
     """
     random_bits = str(random.getrandbits(KEY_SIZE)).encode("UTF-8")
     return md5(random_bits).hexdigest()
 
 
-def parse_xml(fname: StrPath, strip_whitespace=True, remove_comments=True) -> ElementTree:
+def parse_xml(
+    fname: StrPath, strip_whitespace=True, remove_comments=True, schemafname: Union[StrPath, None] = None
+) -> ElementTree:
     """Returns a parsed xml tree"""
     parser = None
+    schema = None
     if remove_comments and LXML_AVAILABLE:
         # If using stdlib etree comments are always removed,
         # but lxml doesn't do this by default
         parser = etree.XMLParser(remove_comments=remove_comments)
+
+    if LXML_AVAILABLE and schemafname:
+        with open(str(schemafname), "rb") as schema_file:
+            schema_root = etree.XML(schema_file.read())
+            schema = etree.XMLSchema(schema_root)
+
     try:
-        tree = etree.parse(str(fname), parser=parser)
+        tree = cast(ElementTree, etree.parse(str(fname), parser=parser))
         root = tree.getroot()
         if strip_whitespace:
             for elem in root.iter("*"):
                 if elem.text is not None:
                     elem.text = elem.text.strip()
                 if elem.tail is not None:
                     elem.tail = elem.tail.strip()
+        if schema:
+            schema.assertValid(tree)
     except OSError as e:
-        if e.errno is None and not os.path.exists(fname):
+        if e.errno is None and not os.path.exists(fname):  # type: ignore[unreachable]
             # lxml doesn't set errno
-            e.errno = errno.ENOENT
+            e.errno = errno.ENOENT  # type: ignore[unreachable]
         raise
     except etree.ParseError:
         log.exception("Error parsing file %s", fname)
         raise
+    except etree.DocumentInvalid:
+        log.exception("Validation of file %s failed", fname)
+        raise
     return tree
 
 
 def parse_xml_string(xml_string: str, strip_whitespace: bool = True) -> Element:
     try:
-        elem = etree.fromstring(xml_string)
+        elem = XML(xml_string)
     except ValueError as e:
         if "strings with encoding declaration are not supported" in unicodify(e):
-            elem = etree.fromstring(xml_string.encode("utf-8"))
+            # This happens with lxml for a string that starts with e.g. `<?xml version="1.0" encoding="UTF-8"?>`
+            elem = XML(xml_string.encode("utf-8"))
         else:
             raise e
     if strip_whitespace:
         for sub_elem in elem.iter("*"):
             if sub_elem.text is not None:
                 sub_elem.text = sub_elem.text.strip()
             if sub_elem.tail is not None:
@@ -338,23 +388,22 @@
     return elem
 
 
 def parse_xml_string_to_etree(xml_string: str, strip_whitespace: bool = True) -> ElementTree:
     return ElementTree(parse_xml_string(xml_string=xml_string, strip_whitespace=strip_whitespace))
 
 
-def xml_to_string(elem: Element, pretty: bool = False) -> str:
+def xml_to_string(elem: Optional[Element], pretty: bool = False) -> str:
     """
     Returns a string from an xml tree.
     """
+    if elem is None:
+        return ""
     try:
-        if elem is not None:
-            xml_str = etree.tostring(elem, encoding="unicode")
-        else:
-            xml_str = ""
+        xml_str = etree.tostring(elem, encoding="unicode")
     except TypeError as e:
         # we assume this is a comment
         if hasattr(elem, "text"):
             return f"<!-- {elem.text} -->\n"
         else:
             raise e
     if xml_str and pretty:
@@ -975,15 +1024,15 @@
     """
     resource_parameters = {}
     if os.path.exists(resource_param_file):
         resource_definitions = parse_xml(resource_param_file)
         resource_definitions_root = resource_definitions.getroot()
         for parameter_elem in resource_definitions_root.findall("param"):
             name = parameter_elem.get("name")
-            resource_parameters[name] = etree.tostring(parameter_elem)
+            resource_parameters[name] = etree.tostring(parameter_elem, encoding="unicode")
 
     return resource_parameters
 
 
 # asbool implementation pulled from PasteDeploy
 truthy = frozenset({"true", "yes", "on", "y", "t", "1"})
 falsy = frozenset({"false", "no", "off", "n", "f", "0"})
@@ -1027,33 +1076,29 @@
         return False
 
 
 ItemType = TypeVar("ItemType")
 
 
 @overload
-def listify(item: Union[None, Literal[False]], do_strip: bool = False) -> List:
-    ...
+def listify(item: Union[None, Literal[False]], do_strip: bool = False) -> List: ...
 
 
 @overload
-def listify(item: str, do_strip: bool = False) -> List[str]:
-    ...
+def listify(item: str, do_strip: bool = False) -> List[str]: ...
 
 
 @overload
-def listify(item: Union[List[ItemType], Tuple[ItemType, ...]], do_strip: bool = False) -> List[ItemType]:
-    ...
+def listify(item: Union[List[ItemType], Tuple[ItemType, ...]], do_strip: bool = False) -> List[ItemType]: ...
 
 
 # Unfortunately we cannot use ItemType .. -> List[ItemType] in the next overload
 # because then that would also match Union types.
 @overload
-def listify(item: Any, do_strip: bool = False) -> List:
-    ...
+def listify(item: Any, do_strip: bool = False) -> List: ...
 
 
 def listify(item: Any, do_strip: bool = False) -> List:
     """
     Make a single item a single item list.
 
     If *item* is a string, it is split on comma (``,``) characters to produce the list. Optionally, if *do_strip* is
@@ -1104,27 +1149,25 @@
 @overload
 def unicodify(  # type: ignore[misc]
     value: Literal[None],
     encoding: str = DEFAULT_ENCODING,
     error: str = "replace",
     strip_null: bool = False,
     log_exception: bool = True,
-) -> None:
-    ...
+) -> None: ...
 
 
 @overload
 def unicodify(
     value: Any,
     encoding: str = DEFAULT_ENCODING,
     error: str = "replace",
     strip_null: bool = False,
     log_exception: bool = True,
-) -> str:
-    ...
+) -> str: ...
 
 
 def unicodify(
     value: Any,
     encoding: str = DEFAULT_ENCODING,
     error: str = "replace",
     strip_null: bool = False,
@@ -1502,15 +1545,15 @@
         return int(number * 1024**5)
     elif multiple.startswith("e"):
         return int(number * 1024**6)
     else:
         raise ValueError(f"Unknown multiplier '{multiple}' in '{size}'")
 
 
-def send_mail(frm, to, subject, body, config, html=None):
+def send_mail(frm, to, subject, body, config, html=None, reply_to=None):
     """
     Sends an email.
 
     :type  frm: str
     :param frm: from address
 
     :type  to: str
@@ -1523,27 +1566,33 @@
     :param body: Body text (should be plain text)
 
     :type  config: object
     :param config: Galaxy configuration object
 
     :type  html: str
     :param html: Alternative HTML representation of the body content. If
-                 provided will convert the message to a MIMEMultipart. (Default 'None')
+                 provided will convert the message to a MIMEMultipart. (Default None)
+
+    :type  reply_to: str
+    :param reply_to: Reply-to address (Default None)
     """
 
     to = listify(to)
     if html:
         msg = MIMEMultipart("alternative")
     else:
         msg = MIMEText(body, "plain", "utf-8")
 
     msg["To"] = ", ".join(to)
     msg["From"] = frm
     msg["Subject"] = subject
 
+    if reply_to:
+        msg["Reply-To"] = reply_to
+
     if config.smtp_server is None:
         log.error("Mail is not configured for this Galaxy instance.")
         log.info(msg)
         return
 
     if html:
         mp_text = MIMEText(body, "plain", "utf-8")
@@ -1730,15 +1779,15 @@
     if params is None:
         params = dict()
     if pathspec is None:
         pathspec = []
     parsed_url = urlparse(base_url)
     if scheme != "http":
         parsed_url.scheme = scheme
-    assert parsed_url.scheme in ("http", "https", "ftp"), f"Invalid URL scheme: {scheme}"
+    assert parsed_url.scheme in ("http", "https", "ftp"), f"Invalid URL scheme: {parsed_url.scheme}"
     if port != 80:
         url = "%s://%s:%d/%s" % (parsed_url.scheme, parsed_url.netloc.rstrip("/"), int(port), parsed_url.path)
     else:
         url = f"{parsed_url.scheme}://{parsed_url.netloc.rstrip('/')}/{parsed_url.path.lstrip('/')}"
     if len(pathspec) > 0:
         url = f"{url.rstrip('/')}/{'/'.join(pathspec)}"
     if parsed_url.query:
```

### Comparing `galaxy-util-23.2.dev0/galaxy/util/aliaspickler.py` & `galaxy-util-24.0.0/galaxy/util/aliaspickler.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.2.dev0/galaxy/util/bool_expressions.py` & `galaxy-util-24.0.0/galaxy/util/bool_expressions.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.2.dev0/galaxy/util/bunch.py` & `galaxy-util-24.0.0/galaxy/util/bunch.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.2.dev0/galaxy/util/bytesize.py` & `galaxy-util-24.0.0/galaxy/util/bytesize.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.2.dev0/galaxy/util/checkers.py` & `galaxy-util-24.0.0/galaxy/util/checkers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import bz2
 import gzip
+import lzma
 import os
 import re
 import tarfile
 import zipfile
 from io import (
     BytesIO,
     StringIO,
@@ -27,16 +28,15 @@
     re.compile(r"<FRAMESET[^>]*>", re.I),
     re.compile(r"<META[\W][^>]*>", re.I),
     re.compile(r"<SCRIPT[^>]*>", re.I),
 )
 
 
 class CompressionChecker(Protocol):
-    def __call__(self, file_path: str, check_content: bool = True) -> Tuple[bool, bool]:
-        ...
+    def __call__(self, file_path: str, check_content: bool = True) -> Tuple[bool, bool]: ...
 
 
 def check_html(name, file_path: bool = True) -> bool:
     """
     Returns True if the file/string contains HTML code.
     """
     # Handles files if file_path is True or text if file_path is False
@@ -114,14 +114,34 @@
         chunk = gzipped_file.read(CHUNK_SIZE)
     # See if we have a compressed HTML file
     if check_html(chunk, file_path=False):
         return (True, False)
     return (True, True)
 
 
+def check_xz(file_path: str, check_content: bool = True) -> Tuple[bool, bool]:
+    try:
+        with open(file_path, "rb") as temp:
+            magic_check = temp.read(6)
+        if magic_check != util.xz_magic:
+            return (False, False)
+    except Exception:
+        return (False, False)
+
+    if not check_content:
+        return (True, True)
+
+    with lzma.LZMAFile(file_path, mode="rb") as xzipped_file:
+        chunk = xzipped_file.read(CHUNK_SIZE)
+    # See if we have a compressed HTML file
+    if check_html(chunk, file_path=False):
+        return (True, False)
+    return (True, True)
+
+
 def check_bz2(file_path: str, check_content: bool = True) -> Tuple[bool, bool]:
     try:
         with open(file_path, "rb") as temp:
             magic_check = temp.read(3)
         if magic_check != util.bz2_magic:
             return (False, False)
     except Exception:
@@ -162,14 +182,19 @@
 
 
 def is_gzip(file_path: str) -> bool:
     is_gzipped, is_valid = check_gzip(file_path, check_content=False)
     return is_gzipped
 
 
+def is_xz(file_path: str) -> bool:
+    is_xzipped, is_valid = check_xz(file_path, check_content=False)
+    return is_xzipped
+
+
 def is_zip(file_path: str) -> bool:
     is_zipped, is_valid = check_zip(file_path, check_content=False)
     return is_zipped
 
 
 def is_single_file_zip(file_path: str) -> bool:
     for i, _ in enumerate(iter_zip(file_path)):
@@ -184,33 +209,33 @@
 
 def iter_zip(file_path: str):
     with zipfile.ZipFile(file_path) as z:
         for f in filter(lambda x: not x.endswith("/"), z.namelist()):
             yield (z.open(f), f)
 
 
-def check_image(file_path: str):
+def check_image(file_path: str) -> bool:
     """Simple wrapper around image_type to yield a True/False verdict"""
-    if image_type(file_path):
-        return True
-    return False
+    return bool(image_type(file_path))
 
 
 COMPRESSION_CHECK_FUNCTIONS: Dict[str, CompressionChecker] = {
     "gzip": check_gzip,
     "bz2": check_bz2,
+    "xz": check_xz,
     "zip": check_zip,
 }
 
 
 __all__ = (
     "check_binary",
     "check_bz2",
     "check_gzip",
     "check_html",
     "check_image",
     "check_zip",
     "COMPRESSION_CHECK_FUNCTIONS",
     "is_gzip",
     "is_bz2",
+    "is_xz",
     "is_zip",
 )
```

### Comparing `galaxy-util-23.2.dev0/galaxy/util/commands.py` & `galaxy-util-24.0.0/galaxy/util/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Generic I/O and shell processing code used by Galaxy tool dependencies."""
+
 import logging
 import os
 import shlex
 import subprocess
 import sys as _sys
 import tempfile
 from typing import (
@@ -51,30 +52,28 @@
         if err:
             err = unicodify(err)
             sys.stderr.write(err)
             err = None
     return out, err
 
 
-def shell(cmds: Union[List[str], str], env: Optional[Dict[str, str]] = None, **kwds: Dict[str, Any]) -> int:
+def shell(cmds: Union[List[str], str], env: Optional[Dict[str, str]] = None, **kwds: Any) -> int:
     """Run shell commands with `shell_process` and wait."""
     sys = kwds.get("sys", _sys)
     assert sys is not None
     p = shell_process(cmds, env, **kwds)
     if redirecting_io(sys=sys):
         redirect_aware_commmunicate(p, sys=sys)
         exit = p.returncode
         return exit
     else:
         return p.wait()
 
 
-def shell_process(
-    cmds: Union[List[str], str], env: Optional[Dict[str, str]] = None, **kwds: Dict[str, Any]
-) -> subprocess.Popen:
+def shell_process(cmds: Union[List[str], str], env: Optional[Dict[str, str]] = None, **kwds: Any) -> subprocess.Popen:
     """A high-level method wrapping subprocess.Popen.
 
     Handles details such as environment extension and in process I/O
     redirection.
     """
     sys = kwds.get("sys", _sys)
     popen_kwds: Dict[str, Any] = dict()
```

### Comparing `galaxy-util-23.2.dev0/galaxy/util/compression_utils.py` & `galaxy-util-24.0.0/galaxy/util/compression_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import bz2
 import gzip
 import io
 import logging
+import lzma
 import os
+import shutil
 import tarfile
 import tempfile
 import zipfile
 from typing import (
     Any,
     cast,
     Generator,
@@ -24,100 +26,107 @@
 from galaxy.util.path import (
     safe_relpath,
     StrPath,
 )
 from .checkers import (
     is_bz2,
     is_gzip,
+    is_xz,
 )
 
+try:
+    from isal import isal_zlib
+except ImportError:
+    isal_zlib = None  # type: ignore[assignment,unused-ignore]
+
+
 log = logging.getLogger(__name__)
 
 FileObjTypeStr = Union[IO[str], io.TextIOWrapper]
-FileObjTypeBytes = Union[gzip.GzipFile, bz2.BZ2File, IO[bytes]]
+FileObjTypeBytes = Union[gzip.GzipFile, bz2.BZ2File, lzma.LZMAFile, IO[bytes]]
 FileObjType = Union[FileObjTypeStr, FileObjTypeBytes]
 
 
 @overload
-def get_fileobj(filename: str, mode: Literal["r"], compressed_formats: Optional[List[str]] = None) -> FileObjTypeStr:
-    ...
+def get_fileobj(
+    filename: str, mode: Literal["r"], compressed_formats: Optional[List[str]] = None
+) -> FileObjTypeStr: ...
 
 
 @overload
-def get_fileobj(filename: str, mode: Literal["rb"], compressed_formats: Optional[List[str]] = None) -> FileObjTypeBytes:
-    ...
+def get_fileobj(
+    filename: str, mode: Literal["rb"], compressed_formats: Optional[List[str]] = None
+) -> FileObjTypeBytes: ...
 
 
 @overload
-def get_fileobj(filename: str) -> FileObjTypeStr:
-    ...
+def get_fileobj(filename: str) -> FileObjTypeStr: ...
 
 
 @overload
-def get_fileobj(filename: str, mode: str = "r", compressed_formats: Optional[List[str]] = None) -> FileObjType:
-    ...
+def get_fileobj(filename: str, mode: str = "r", compressed_formats: Optional[List[str]] = None) -> FileObjType: ...
 
 
 def get_fileobj(filename: str, mode: str = "r", compressed_formats: Optional[List[str]] = None) -> FileObjType:
     """
     Returns a fileobj. If the file is compressed, return an appropriate file
     reader. In text mode, always use 'utf-8' encoding.
 
     :param filename: path to file that should be opened
     :param mode: mode to pass to opener
     :param compressed_formats: list of allowed compressed file formats among
-      'bz2', 'gzip' and 'zip'. If left to None, all 3 formats are allowed
+      'bz2', 'gzip', 'xz' and 'zip'. If left to None, all 3 formats are allowed
     """
     return get_fileobj_raw(filename, mode, compressed_formats)[1]
 
 
 @overload
 def get_fileobj_raw(
     filename: str, mode: Literal["r"], compressed_formats: Optional[List[str]] = None
-) -> Tuple[Optional[str], FileObjTypeStr]:
-    ...
+) -> Tuple[Optional[str], FileObjTypeStr]: ...
 
 
 @overload
 def get_fileobj_raw(
     filename: str, mode: Literal["rb"], compressed_formats: Optional[List[str]] = None
-) -> Tuple[Optional[str], FileObjTypeBytes]:
-    ...
+) -> Tuple[Optional[str], FileObjTypeBytes]: ...
 
 
 @overload
-def get_fileobj_raw(filename: str) -> Tuple[Optional[str], FileObjTypeStr]:
-    ...
+def get_fileobj_raw(filename: str) -> Tuple[Optional[str], FileObjTypeStr]: ...
 
 
 @overload
 def get_fileobj_raw(
     filename: str, mode: str = "r", compressed_formats: Optional[List[str]] = None
-) -> Tuple[Optional[str], FileObjType]:
-    ...
+) -> Tuple[Optional[str], FileObjType]: ...
 
 
 def get_fileobj_raw(
     filename: str, mode: str = "r", compressed_formats: Optional[List[str]] = None
 ) -> Tuple[Optional[str], FileObjType]:
     if compressed_formats is None:
-        compressed_formats = ["bz2", "gzip", "zip"]
+        compressed_formats = ["bz2", "gzip", "xz", "zip"]
     # Remove 't' from mode, which may cause an error for compressed files
     mode = mode.replace("t", "")
     # 'U' mode is deprecated, we open in 'r'.
     if mode == "U":
         mode = "r"
     compressed_format = None
     if "gzip" in compressed_formats and is_gzip(filename):
-        fh: Union[gzip.GzipFile, bz2.BZ2File, IO[bytes]] = gzip.GzipFile(filename, mode)
+        fh: Union[gzip.GzipFile, bz2.BZ2File, lzma.LZMAFile, IO[bytes]] = gzip.GzipFile(filename, mode)
         compressed_format = "gzip"
     elif "bz2" in compressed_formats and is_bz2(filename):
         mode = cast(Literal["a", "ab", "r", "rb", "w", "wb", "x", "xb"], mode)
         fh = bz2.BZ2File(filename, mode)
         compressed_format = "bz2"
+    elif "xz" in compressed_formats and is_xz(filename):
+        mode = cast(Literal["a", "ab", "r", "rb", "w", "wb", "x", "xb"], mode)
+        fh = lzma.LZMAFile(filename, mode)
+        compressed_format = "xz"
     elif "zip" in compressed_formats and zipfile.is_zipfile(filename):
         # Return fileobj for the first file in a zip file.
         # 'b' is not allowed in the ZipFile mode argument
         # since it always opens files in binary mode.
         # For emulating text mode, we will be returning the binary fh in a
         # TextIOWrapper.
         zf_mode = cast(Literal["r", "w"], mode.replace("b", ""))
@@ -341,7 +350,88 @@
         basename = os.path.realpath(os.path.dirname(path_to_archive))
         zip_archive = zipfile.ZipFile(path_to_archive)
         for member in zip_archive.namelist():
             member_path = os.path.realpath(os.path.join(basename, member))
             if not member_path.startswith(basename):
                 return False
         return True
+
+
+class FastZipFile(zipfile.ZipFile):
+    """
+    Simple wrapper around ZipFile that uses the default compression strategy of ISA-L
+    to write zip files. Ignores compresslevel and compresstype arguments, and is
+    3 to 4 times faster than the zlib implementation at the default compression level.
+    """
+
+    def _open_to_write(self, *args, **kwargs):  # type: ignore[no-untyped-def]
+        zwf = super()._open_to_write(*args, **kwargs)  # type: ignore[misc]
+        if isal_zlib and self.compression == zipfile.ZIP_DEFLATED:
+            zwf._compressor = isal_zlib.compressobj(isal_zlib.ISAL_DEFAULT_COMPRESSION, isal_zlib.DEFLATED, -15, 9)
+        return zwf
+
+
+# modified from shutil._make_zipfile
+def make_fast_zipfile(
+    base_name: str,
+    base_dir: str,
+    verbose: int = 0,
+    dry_run: int = 0,
+    logger: Optional[logging.Logger] = None,
+    owner: Optional[str] = None,
+    group: Optional[str] = None,
+    root_dir: Optional[str] = None,
+) -> str:
+    """Create a zip file from all the files under 'base_dir'.
+
+    The output zip file will be named 'base_name' + ".zip".  Returns the
+    name of the output zip file.
+    """
+
+    zip_filename = base_name + ".zip"
+    archive_dir = os.path.dirname(base_name)
+
+    if archive_dir and not os.path.exists(archive_dir):
+        if logger is not None:
+            logger.info("creating %s", archive_dir)
+        if not dry_run:
+            os.makedirs(archive_dir)
+
+    if logger is not None:
+        logger.info("creating '%s' and adding '%s' to it", zip_filename, base_dir)
+
+    if not dry_run:
+        with FastZipFile(zip_filename, mode="w", compression=zipfile.ZIP_DEFLATED) as zf:
+            arcname = os.path.normpath(base_dir)
+            if root_dir is not None:
+                base_dir = os.path.join(root_dir, base_dir)
+            base_dir = os.path.normpath(base_dir)
+            if arcname != os.curdir:
+                zf.write(base_dir, arcname)
+                if logger is not None:
+                    logger.info("adding '%s'", base_dir)
+            for dirpath, dirnames, filenames in os.walk(base_dir):
+                arcdirpath = dirpath
+                if root_dir is not None:
+                    arcdirpath = os.path.relpath(arcdirpath, root_dir)
+                arcdirpath = os.path.normpath(arcdirpath)
+                for name in sorted(dirnames):
+                    path = os.path.join(dirpath, name)
+                    arcname = os.path.join(arcdirpath, name)
+                    zf.write(path, arcname)
+                    if logger is not None:
+                        logger.info("adding '%s'", path)
+                for name in filenames:
+                    path = os.path.join(dirpath, name)
+                    path = os.path.normpath(path)
+                    if os.path.isfile(path):
+                        arcname = os.path.join(arcdirpath, name)
+                        zf.write(path, arcname)
+                        if logger is not None:
+                            logger.info("adding '%s'", path)
+
+    if root_dir is not None:
+        zip_filename = os.path.abspath(zip_filename)
+    return zip_filename
+
+
+shutil.register_archive_format("fastzip", make_fast_zipfile)
```

### Comparing `galaxy-util-23.2.dev0/galaxy/util/config_parsers.py` & `galaxy-util-24.0.0/galaxy/util/config_parsers.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,13 +9,15 @@
 IpAddressT = Union[ipaddress.IPv4Address, ipaddress.IPv6Address]
 IpNetworkT = Union[ipaddress.IPv4Network, ipaddress.IPv6Network]
 IpAllowedListEntryT = Union[IpAddressT, IpNetworkT]
 
 
 def parse_allowlist_ips(fetch_url_allowlist: List[str]) -> List[IpAllowedListEntryT]:
     return [
-        ipaddress.ip_network(unicodify(ip.strip()))  # If it has a slash, assume 127.0.0.1/24 notation
-        if "/" in ip
-        else ipaddress.ip_address(unicodify(ip.strip()))  # Otherwise interpret it as an ip address.
+        (
+            ipaddress.ip_network(unicodify(ip.strip()))  # If it has a slash, assume 127.0.0.1/24 notation
+            if "/" in ip
+            else ipaddress.ip_address(unicodify(ip.strip()))
+        )  # Otherwise interpret it as an ip address.
         for ip in fetch_url_allowlist
         if len(ip.strip()) > 0
     ]
```

### Comparing `galaxy-util-23.2.dev0/galaxy/util/custom_logging/fluent_log.py` & `galaxy-util-24.0.0/galaxy/util/custom_logging/fluent_log.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.2.dev0/galaxy/util/dictifiable.py` & `galaxy-util-24.0.0/galaxy/util/dictifiable.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.2.dev0/galaxy/util/drs.py` & `galaxy-util-24.0.0/galaxy/util/drs.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.2.dev0/galaxy/util/expressions.py` & `galaxy-util-24.0.0/galaxy/util/expressions.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.2.dev0/galaxy/util/facts.py` & `galaxy-util-24.0.0/galaxy/util/facts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Return various facts for string formatting.
 """
+
 import socket
 from collections.abc import MutableMapping
 
 
 class Facts(MutableMapping):
     """A dict-like object that evaluates values at access time."""
```

### Comparing `galaxy-util-23.2.dev0/galaxy/util/filelock.py` & `galaxy-util-24.0.0/galaxy/util/filelock.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Code obtained from https://github.com/dmfrey/FileLock.
 
 See full license at:
 
 https://github.com/dmfrey/FileLock/blob/master/LICENSE.txt
 
 """
+
 import errno
 import os
 import time
 
 
 class FileLockException(Exception):
     pass
```

### Comparing `galaxy-util-23.2.dev0/galaxy/util/form_builder.py` & `galaxy-util-24.0.0/galaxy/util/form_builder.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.2.dev0/galaxy/util/hash_util.py` & `galaxy-util-24.0.0/galaxy/util/hash_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.2.dev0/galaxy/util/heartbeat.py` & `galaxy-util-24.0.0/galaxy/util/heartbeat.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.2.dev0/galaxy/util/inflection.py` & `galaxy-util-24.0.0/galaxy/util/inflection.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.2.dev0/galaxy/util/json.py` & `galaxy-util-24.0.0/galaxy/util/json.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.2.dev0/galaxy/util/jstree.py` & `galaxy-util-24.0.0/galaxy/util/jstree.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.2.dev0/galaxy/util/lazy_process.py` & `galaxy-util-24.0.0/galaxy/util/lazy_process.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.2.dev0/galaxy/util/monitors.py` & `galaxy-util-24.0.0/galaxy/util/monitors.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.2.dev0/galaxy/util/odict.py` & `galaxy-util-24.0.0/galaxy/util/odict.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.2.dev0/galaxy/util/oset.py` & `galaxy-util-24.0.0/galaxy/util/oset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Ordered set implementation from https://code.activestate.com/recipes/576694/
 """
+
 from collections.abc import MutableSet
 
 
 class OrderedSet(MutableSet):
     def __init__(self, iterable=None):
         self.end = end = []
         end += [None, end, end]  # sentinel node for doubly linked list
```

### Comparing `galaxy-util-23.2.dev0/galaxy/util/path/__init__.py` & `galaxy-util-24.0.0/galaxy/util/path/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.2.dev0/galaxy/util/permutations.py` & `galaxy-util-24.0.0/galaxy/util/permutations.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 and tools. This module is meant to capture some general permutation logic that
 can be applicable for both cases but will only be used in the newer tools case
 first.
 
 Maybe this doesn't make sense and maybe much of this stuff could be replaced
 with itertools product and permutations. These are open questions.
 """
+
 from typing import (
     Dict,
     TypeVar,
 )
 
 from galaxy.exceptions import MessageException
 from galaxy.util.bunch import Bunch
```

### Comparing `galaxy-util-23.2.dev0/galaxy/util/plugin_config.py` & `galaxy-util-24.0.0/galaxy/util/plugin_config.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.2.dev0/galaxy/util/properties.py` & `galaxy-util-24.0.0/galaxy/util/properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """ Module used to blend ini, environment, and explicit dictionary properties
 to determine application configuration. Some hard coded defaults for Galaxy but
 this should be reusable by tool shed and pulsar as well.
 """
+
 import os
 import os.path
 import sys
 from configparser import (
     BasicInterpolation,
     ConfigParser,
     InterpolationError,
```

### Comparing `galaxy-util-23.2.dev0/galaxy/util/renamed_temporary_file.py` & `galaxy-util-24.0.0/galaxy/util/renamed_temporary_file.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Safely write file to temporary file and then move file into place."""
+
 # Copied from https://stackoverflow.com/a/12007885.
 import os
 import tempfile
 
 from galaxy.util.path import StrOrBytesPath
```

### Comparing `galaxy-util-23.2.dev0/galaxy/util/rst_to_html.py` & `galaxy-util-24.0.0/galaxy/util/rst_to_html.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.2.dev0/galaxy/util/rules_dsl.py` & `galaxy-util-24.0.0/galaxy/util/rules_dsl.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.2.dev0/galaxy/util/rules_dsl_spec.yml` & `galaxy-util-24.0.0/galaxy/util/rules_dsl_spec.yml`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.2.dev0/galaxy/util/sanitize_html.py` & `galaxy-util-24.0.0/galaxy/util/sanitize_html.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 HTML Sanitizer (lists of acceptable_* ripped from feedparser)
 """
+
 import bleach
 
 from galaxy.util import unicodify
 
 _acceptable_elements = [
     "a",
     "abbr",
```

### Comparing `galaxy-util-23.2.dev0/galaxy/util/script.py` & `galaxy-util-24.0.0/galaxy/util/script.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Utilities for Galaxy scripts
 """
+
 import argparse
 import logging
 import os
 import sys
 
 from galaxy.util.properties import (
     find_config_file,
```

### Comparing `galaxy-util-23.2.dev0/galaxy/util/search.py` & `galaxy-util-24.0.0/galaxy/util/search.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.2.dev0/galaxy/util/simplegraph.py` & `galaxy-util-24.0.0/galaxy/util/simplegraph.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Fencepost-simple graph structure implementation.
 """
+
 # Currently (2013.7.12) only used in easing the parsing of graph datatype data.
 
 
 class SimpleGraphNode:
     """
     Node representation.
     """
```

### Comparing `galaxy-util-23.2.dev0/galaxy/util/sleeper.py` & `galaxy-util-24.0.0/galaxy/util/sleeper.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.2.dev0/galaxy/util/sockets.py` & `galaxy-util-24.0.0/galaxy/util/sockets.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.2.dev0/galaxy/util/specs.py` & `galaxy-util-24.0.0/galaxy/util/specs.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.2.dev0/galaxy/util/sqlite.py` & `galaxy-util-24.0.0/galaxy/util/sqlite.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.2.dev0/galaxy/util/submodules.py` & `galaxy-util-24.0.0/galaxy/util/submodules.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,12 +41,12 @@
     for _, name, is_pkg in pkgutil.walk_packages(module.__path__):
         full_name = f"{module.__name__}.{name}"
         try:
             submodule = importlib.import_module(full_name)
             submodules.append(submodule)
             if recursive and is_pkg:
                 submodules.update(__import_submodules_impl(submodule, recursive=True))
-        except BaseException:
+        except Exception:
             message = f"{full_name} dynamic module could not be loaded (traceback follows):"
             log.exception(message)
             continue
     return submodules
```

### Comparing `galaxy-util-23.2.dev0/galaxy/util/task.py` & `galaxy-util-24.0.0/galaxy/util/task.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.2.dev0/galaxy/util/template.py` & `galaxy-util-24.0.0/galaxy/util/template.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.2.dev0/galaxy/util/themes.py` & `galaxy-util-24.0.0/galaxy/util/themes.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.2.dev0/galaxy/util/tool_shed/common_util.py` & `galaxy-util-24.0.0/galaxy/util/tool_shed/common_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.2.dev0/galaxy/util/tool_shed/encoding_util.py` & `galaxy-util-24.0.0/galaxy/util/tool_shed/encoding_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.2.dev0/galaxy/util/tool_shed/tool_shed_registry.py` & `galaxy-util-24.0.0/galaxy/util/tool_shed/tool_shed_registry.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.2.dev0/galaxy/util/tool_shed/xml_util.py` & `galaxy-util-24.0.0/galaxy/util/tool_shed/xml_util.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,44 +3,44 @@
 import tempfile
 from typing import (
     Optional,
     Tuple,
 )
 
 from galaxy.util import (
-    etree,
+    Element,
+    ElementTree,
     parse_xml as galaxy_parse_xml,
-    unicodify,
     xml_to_string,
 )
 from galaxy.util.path import StrPath
 
 log = logging.getLogger(__name__)
 
 
-def create_and_write_tmp_file(elem: etree.Element) -> str:
+def create_and_write_tmp_file(elem: Element) -> str:
     tmp_str = xml_to_string(elem, pretty=True)
     with tempfile.NamedTemporaryFile(prefix="tmp-toolshed-cawrf", delete=False) as fh:
         tmp_filename = fh.name
     with open(tmp_filename, mode="w", encoding="utf-8") as fh:
         fh.write(tmp_str)
     return tmp_filename
 
 
-def parse_xml(file_name: StrPath, check_exists=True) -> Tuple[Optional[etree.ElementTree], str]:
+def parse_xml(file_name: StrPath, check_exists=True) -> Tuple[Optional[ElementTree], str]:
     """Returns a parsed xml tree with comments intact."""
     error_message = ""
     if check_exists and not os.path.exists(file_name):
         return None, f"File does not exist {str(file_name)}"
     try:
         tree = galaxy_parse_xml(file_name, remove_comments=False, strip_whitespace=False)
     except OSError:
         raise
     except Exception as e:
-        error_message = f"Exception attempting to parse {str(file_name)}: {unicodify(e)}"
+        error_message = f"Exception attempting to parse {file_name}: {e}"
         log.exception(error_message)
         return None, error_message
     return tree, error_message
 
 
 __all__ = (
     "create_and_write_tmp_file",
```

### Comparing `galaxy-util-23.2.dev0/galaxy/util/topsort.py` & `galaxy-util-24.0.0/galaxy/util/topsort.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,15 @@
     for x in answer:
         assert numpreds[x] == 0
         del numpreds[x]
         if x in successors:
             for y in successors[x]:
                 numpreds[y] = numpreds[y] - 1
                 if numpreds[y] == 0:
-                    answer.append(y)
+                    answer.append(y)  # noqa: B038
             # following "del" isn't needed; just makes
             # CycleError details easier to grasp
             del successors[x]
 
     if numpreds:
         # everything in numpreds has at least one predecessor ->
         # there's a cycle
```

### Comparing `galaxy-util-23.2.dev0/galaxy/util/tree_dict.py` & `galaxy-util-24.0.0/galaxy/util/tree_dict.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.2.dev0/galaxy/util/ucsc.py` & `galaxy-util-24.0.0/galaxy/util/ucsc.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.2.dev0/galaxy/util/unittest.py` & `galaxy-util-24.0.0/galaxy/util/unittest.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.2.dev0/galaxy/util/unittest_utils/__init__.py` & `galaxy-util-24.0.0/galaxy/util/unittest_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.2.dev0/galaxy/util/validation.py` & `galaxy-util-24.0.0/galaxy/util/validation.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.2.dev0/galaxy/util/watcher.py` & `galaxy-util-24.0.0/galaxy/util/watcher.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.2.dev0/galaxy/util/xml_macros.py` & `galaxy-util-24.0.0/galaxy/util/xml_macros.py`

 * *Files 2% similar despite different names*

```diff
@@ -279,21 +279,14 @@
 
 def _load_macro_file(path: StrPath, xml_base_dir, macros) -> List[str]:
     tree = parse_xml(path, strip_whitespace=False)
     root = tree.getroot()
     return _load_macros(root, xml_base_dir, macros)
 
 
-def _xml_set_children(element, new_children):
-    for old_child in element:
-        element.remove(old_child)
-    for i, new_child in enumerate(new_children):
-        element.insert(i, new_child)
-
-
 def _xml_replace(query, targets):
     parent_el = query.find("..")
     matching_index = -1
     # for index, el in enumerate(parent_el.iter('.')):  ## Something like this for newer implementation
     for index, el in enumerate(list(parent_el)):
         if el == query:
             matching_index = index
```

### Comparing `galaxy-util-23.2.dev0/galaxy/util/yaml_util.py` & `galaxy-util-24.0.0/galaxy/util/yaml_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.2.dev0/galaxy/util/zipstream.py` & `galaxy-util-24.0.0/galaxy/util/zipstream.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.2.dev0/galaxy_util.egg-info/SOURCES.txt` & `galaxy-util-24.0.0/galaxy_util.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 test-requirements.txt
 galaxy/__init__.py
 galaxy/py.typed
 galaxy/version.py
 galaxy/exceptions/__init__.py
 galaxy/exceptions/error_codes.json
 galaxy/exceptions/error_codes.py
+galaxy/exceptions/utils.py
 galaxy/util/__init__.py
 galaxy/util/aliaspickler.py
 galaxy/util/bool_expressions.py
 galaxy/util/bunch.py
 galaxy/util/bytesize.py
 galaxy/util/checkers.py
 galaxy/util/commands.py
```

### Comparing `galaxy-util-23.2.dev0/setup.cfg` & `galaxy-util-24.0.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -10,36 +10,37 @@
 	Operating System :: POSIX
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Topic :: Software Development
 	Topic :: Software Development :: Code Generators
 	Topic :: Software Development :: Testing
 description = Galaxy generic utilities
 keywords = 
 	Galaxy
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-util
 url = https://github.com/galaxyproject/galaxy
-version = 23.2.dev0
+version = 24.0.0
 
 [options]
 include_package_data = True
 install_requires = 
 	bleach
 	boltons
-	docutils
-	importlib_resources
+	docutils!=0.17,!=0.17.1
+	importlib-resources;python_version<'3.9'
 	packaging
 	pyparsing
 	PyYAML
 	requests
 	Routes
 	typing-extensions
 	zipstream-new
@@ -47,15 +48,15 @@
 python_requires = >=3.7
 
 [options.extras_require]
 jstree = 
 	dictobj
 template = 
 	Cheetah3
-	future
+	future>=1.0.0
 
 [options.packages.find]
 exclude = 
 	tests*
 
 [egg_info]
 tag_build =
```

