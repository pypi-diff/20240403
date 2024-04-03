# Comparing `tmp/countess-0.0.55.tar.gz` & `tmp/countess-0.0.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "countess-0.0.55.tar", last modified: Tue Apr  2 03:30:16 2024, max compression
+gzip compressed data, was "countess-0.0.56.tar", last modified: Wed Apr  3 05:26:15 2024, max compression
```

## Comparing `countess-0.0.55.tar` & `countess-0.0.56.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-02 03:30:16.761914 countess-0.0.55/
--rw-rw-r--   0 nick      (1000) nick      (1000)     1470 2023-10-25 21:13:29.000000 countess-0.0.55/LICENSE.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)       59 2024-03-27 01:45:29.000000 countess-0.0.55/MANIFEST.in
--rw-r--r--   0 nick      (1000) nick      (1000)     2012 2024-04-02 03:30:16.761914 countess-0.0.55/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)      685 2024-04-02 03:29:37.000000 countess-0.0.55/README.md
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-02 03:30:16.753913 countess-0.0.55/countess/
--rw-rw-r--   0 nick      (1000) nick      (1000)       43 2024-04-02 03:29:37.000000 countess-0.0.55/countess/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-02 03:30:16.753913 countess-0.0.55/countess/core/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:48:22.000000 countess-0.0.55/countess/core/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)      466 2024-03-14 22:01:54.000000 countess-0.0.55/countess/core/cmd.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     4764 2024-04-02 01:29:15.000000 countess-0.0.55/countess/core/config.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2799 2023-11-09 02:30:05.000000 countess-0.0.55/countess/core/logger.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    19161 2024-04-02 03:04:31.000000 countess-0.0.55/countess/core/parameters.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    13908 2024-04-02 03:04:33.000000 countess-0.0.55/countess/core/pipeline.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    25925 2024-04-02 03:04:33.000000 countess-0.0.55/countess/core/plugins.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-02 03:30:16.753913 countess-0.0.55/countess/gui/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-05-25 01:44:18.000000 countess-0.0.55/countess/gui/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    18436 2024-04-02 03:04:33.000000 countess-0.0.55/countess/gui/config.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-02 03:30:16.757913 countess-0.0.55/countess/gui/icons/
--rw-rw-r--   0 nick      (1000) nick      (1000)       90 2024-03-27 01:45:29.000000 countess-0.0.55/countess/gui/icons/add.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       98 2024-03-27 01:45:29.000000 countess-0.0.55/countess/gui/icons/check.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       98 2024-03-27 01:45:29.000000 countess-0.0.55/countess/gui/icons/del.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       62 2024-03-28 00:06:21.000000 countess-0.0.55/countess/gui/icons/hbar.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       84 2024-03-27 01:45:29.000000 countess-0.0.55/countess/gui/icons/info.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       71 2024-03-28 00:06:21.000000 countess-0.0.55/countess/gui/icons/redbar.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       84 2024-03-28 00:06:21.000000 countess-0.0.55/countess/gui/icons/sort_dn.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       86 2024-03-28 00:06:21.000000 countess-0.0.55/countess/gui/icons/sort_un.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       88 2024-03-28 00:06:21.000000 countess-0.0.55/countess/gui/icons/sort_up.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       88 2024-03-27 01:45:29.000000 countess-0.0.55/countess/gui/icons/uncheck.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       71 2024-03-28 00:06:21.000000 countess-0.0.55/countess/gui/icons/vbar.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)     5105 2024-03-18 03:56:53.000000 countess-0.0.55/countess/gui/logger.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    20092 2024-04-02 03:04:33.000000 countess-0.0.55/countess/gui/main.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1730 2024-03-28 00:06:21.000000 countess-0.0.55/countess/gui/mini_browser.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    15129 2024-04-02 01:54:52.000000 countess-0.0.55/countess/gui/tabular.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    23070 2024-04-02 01:39:26.000000 countess-0.0.55/countess/gui/tree.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3520 2024-04-02 03:01:22.000000 countess-0.0.55/countess/gui/widgets.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-02 03:30:16.757913 countess-0.0.55/countess/plugins/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-05-25 01:44:18.000000 countess-0.0.55/countess/plugins/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2402 2024-04-02 03:04:33.000000 countess-0.0.55/countess/plugins/collate.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2116 2024-04-02 03:04:33.000000 countess-0.0.55/countess/plugins/column.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2245 2024-04-02 03:04:33.000000 countess-0.0.55/countess/plugins/correlation.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     7274 2024-04-02 03:04:33.000000 countess-0.0.55/countess/plugins/csv.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3844 2024-04-02 03:04:33.000000 countess-0.0.55/countess/plugins/data_table.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1842 2024-04-02 03:04:33.000000 countess-0.0.55/countess/plugins/expression.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2938 2024-04-02 02:23:40.000000 countess-0.0.55/countess/plugins/fastq.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     4735 2024-04-02 03:04:33.000000 countess-0.0.55/countess/plugins/group_by.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3339 2024-04-02 03:04:33.000000 countess-0.0.55/countess/plugins/hgvs_parser.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     4541 2024-04-02 03:04:33.000000 countess-0.0.55/countess/plugins/join.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3348 2023-11-28 03:30:23.000000 countess-0.0.55/countess/plugins/mutagenize.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3649 2024-03-28 07:10:57.000000 countess-0.0.55/countess/plugins/pivot.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2977 2024-03-28 00:06:21.000000 countess-0.0.55/countess/plugins/python.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     6758 2024-04-02 03:04:33.000000 countess-0.0.55/countess/plugins/regex.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1902 2024-04-02 03:04:33.000000 countess-0.0.55/countess/plugins/sequence.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3705 2024-04-02 03:04:33.000000 countess-0.0.55/countess/plugins/variant.py
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:39:01.000000 countess-0.0.55/countess/py.typed
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-02 03:30:16.757913 countess-0.0.55/countess/utils/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-09-26 22:30:04.000000 countess-0.0.55/countess/utils/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2768 2024-03-14 02:50:26.000000 countess-0.0.55/countess/utils/pandas.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2996 2024-03-18 21:32:56.000000 countess-0.0.55/countess/utils/parallel.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    17825 2024-03-19 05:10:25.000000 countess-0.0.55/countess/utils/variant.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-02 03:30:16.757913 countess-0.0.55/countess.egg-info/
--rw-r--r--   0 nick      (1000) nick      (1000)     2012 2024-04-02 03:30:16.000000 countess-0.0.55/countess.egg-info/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)     1619 2024-04-02 03:30:16.000000 countess-0.0.55/countess.egg-info/SOURCES.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        1 2024-04-02 03:30:16.000000 countess-0.0.55/countess.egg-info/dependency_links.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)     1056 2024-04-02 03:30:16.000000 countess-0.0.55/countess.egg-info/entry_points.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)      310 2024-04-02 03:30:16.000000 countess-0.0.55/countess.egg-info/requires.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        9 2024-04-02 03:30:16.000000 countess-0.0.55/countess.egg-info/top_level.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)     3236 2024-04-01 22:33:53.000000 countess-0.0.55/pyproject.toml
--rw-rw-r--   0 nick      (1000) nick      (1000)       38 2024-04-02 03:30:16.761914 countess-0.0.55/setup.cfg
--rw-rw-r--   0 nick      (1000) nick      (1000)       39 2023-05-25 01:44:18.000000 countess-0.0.55/setup.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-02 03:30:16.757913 countess-0.0.55/tests/
--rw-rw-r--   0 nick      (1000) nick      (1000)      476 2024-04-02 01:28:13.000000 countess-0.0.55/tests/test_cmd.py
--rw-rw-r--   0 nick      (1000) nick      (1000)      498 2024-04-02 01:28:13.000000 countess-0.0.55/tests/test_gui.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1060 2023-11-09 02:44:32.000000 countess-0.0.55/tests/test_plugins.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-03 05:26:15.267245 countess-0.0.56/
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1470 2023-10-25 21:13:29.000000 countess-0.0.56/LICENSE.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)       59 2024-04-03 00:27:43.000000 countess-0.0.56/MANIFEST.in
+-rw-r--r--   0 nick      (1000) nick      (1000)     2050 2024-04-03 05:26:15.267245 countess-0.0.56/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)      723 2024-04-03 05:25:56.000000 countess-0.0.56/README.md
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-03 05:26:15.263245 countess-0.0.56/countess/
+-rw-rw-r--   0 nick      (1000) nick      (1000)       43 2024-04-03 05:25:56.000000 countess-0.0.56/countess/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-03 05:26:15.263245 countess-0.0.56/countess/core/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:48:22.000000 countess-0.0.56/countess/core/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)      466 2024-04-03 00:27:43.000000 countess-0.0.56/countess/core/cmd.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     4764 2024-04-03 00:27:43.000000 countess-0.0.56/countess/core/config.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2799 2023-11-09 02:30:05.000000 countess-0.0.56/countess/core/logger.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    19161 2024-04-03 00:27:43.000000 countess-0.0.56/countess/core/parameters.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    13908 2024-04-03 05:16:18.000000 countess-0.0.56/countess/core/pipeline.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    25925 2024-04-03 05:16:18.000000 countess-0.0.56/countess/core/plugins.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-03 05:26:15.263245 countess-0.0.56/countess/gui/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-05-25 01:44:18.000000 countess-0.0.56/countess/gui/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    18458 2024-04-03 05:18:33.000000 countess-0.0.56/countess/gui/config.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-03 05:26:15.263245 countess-0.0.56/countess/gui/icons/
+-rw-rw-r--   0 nick      (1000) nick      (1000)       90 2024-04-03 00:27:43.000000 countess-0.0.56/countess/gui/icons/add.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       98 2024-04-03 00:27:43.000000 countess-0.0.56/countess/gui/icons/check.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       98 2024-04-03 00:27:43.000000 countess-0.0.56/countess/gui/icons/del.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       62 2024-04-03 00:27:43.000000 countess-0.0.56/countess/gui/icons/hbar.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       84 2024-04-03 00:27:43.000000 countess-0.0.56/countess/gui/icons/info.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       71 2024-04-03 00:27:43.000000 countess-0.0.56/countess/gui/icons/redbar.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       84 2024-04-03 00:27:43.000000 countess-0.0.56/countess/gui/icons/sort_dn.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       86 2024-04-03 00:27:43.000000 countess-0.0.56/countess/gui/icons/sort_un.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       88 2024-04-03 00:27:43.000000 countess-0.0.56/countess/gui/icons/sort_up.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       88 2024-04-03 00:27:43.000000 countess-0.0.56/countess/gui/icons/uncheck.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       71 2024-04-03 00:27:43.000000 countess-0.0.56/countess/gui/icons/vbar.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)     5105 2024-04-03 00:27:43.000000 countess-0.0.56/countess/gui/logger.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    20088 2024-04-03 05:16:18.000000 countess-0.0.56/countess/gui/main.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1730 2024-04-03 00:27:43.000000 countess-0.0.56/countess/gui/mini_browser.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    15188 2024-04-03 00:42:47.000000 countess-0.0.56/countess/gui/tabular.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    23070 2024-04-03 01:42:58.000000 countess-0.0.56/countess/gui/tree.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3565 2024-04-03 05:15:43.000000 countess-0.0.56/countess/gui/widgets.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-03 05:26:15.267245 countess-0.0.56/countess/plugins/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-05-25 01:44:18.000000 countess-0.0.56/countess/plugins/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2402 2024-04-03 05:16:18.000000 countess-0.0.56/countess/plugins/collate.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2116 2024-04-03 05:16:18.000000 countess-0.0.56/countess/plugins/column.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2245 2024-04-03 05:16:18.000000 countess-0.0.56/countess/plugins/correlation.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     7274 2024-04-03 05:16:18.000000 countess-0.0.56/countess/plugins/csv.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3844 2024-04-03 05:16:18.000000 countess-0.0.56/countess/plugins/data_table.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1842 2024-04-03 05:16:18.000000 countess-0.0.56/countess/plugins/expression.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2938 2024-04-03 00:27:43.000000 countess-0.0.56/countess/plugins/fastq.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     4735 2024-04-03 05:16:18.000000 countess-0.0.56/countess/plugins/group_by.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3339 2024-04-03 05:16:18.000000 countess-0.0.56/countess/plugins/hgvs_parser.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     4541 2024-04-03 05:16:18.000000 countess-0.0.56/countess/plugins/join.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3348 2023-11-28 03:30:23.000000 countess-0.0.56/countess/plugins/mutagenize.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3660 2024-04-03 00:44:33.000000 countess-0.0.56/countess/plugins/pivot.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2977 2024-04-03 00:27:43.000000 countess-0.0.56/countess/plugins/python.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     6758 2024-04-03 05:16:18.000000 countess-0.0.56/countess/plugins/regex.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1902 2024-04-03 05:16:18.000000 countess-0.0.56/countess/plugins/sequence.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3705 2024-04-03 05:16:18.000000 countess-0.0.56/countess/plugins/variant.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:39:01.000000 countess-0.0.56/countess/py.typed
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-03 05:26:15.267245 countess-0.0.56/countess/utils/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-09-26 22:30:04.000000 countess-0.0.56/countess/utils/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2768 2024-03-14 02:50:26.000000 countess-0.0.56/countess/utils/pandas.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2996 2024-04-03 00:27:43.000000 countess-0.0.56/countess/utils/parallel.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    17825 2024-04-03 00:27:43.000000 countess-0.0.56/countess/utils/variant.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-03 05:26:15.267245 countess-0.0.56/countess.egg-info/
+-rw-r--r--   0 nick      (1000) nick      (1000)     2050 2024-04-03 05:26:15.000000 countess-0.0.56/countess.egg-info/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1619 2024-04-03 05:26:15.000000 countess-0.0.56/countess.egg-info/SOURCES.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        1 2024-04-03 05:26:15.000000 countess-0.0.56/countess.egg-info/dependency_links.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1056 2024-04-03 05:26:15.000000 countess-0.0.56/countess.egg-info/entry_points.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)      310 2024-04-03 05:26:15.000000 countess-0.0.56/countess.egg-info/requires.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        9 2024-04-03 05:26:15.000000 countess-0.0.56/countess.egg-info/top_level.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3236 2024-04-03 00:27:43.000000 countess-0.0.56/pyproject.toml
+-rw-rw-r--   0 nick      (1000) nick      (1000)       38 2024-04-03 05:26:15.267245 countess-0.0.56/setup.cfg
+-rw-rw-r--   0 nick      (1000) nick      (1000)       39 2023-05-25 01:44:18.000000 countess-0.0.56/setup.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-03 05:26:15.267245 countess-0.0.56/tests/
+-rw-rw-r--   0 nick      (1000) nick      (1000)      476 2024-04-03 00:27:43.000000 countess-0.0.56/tests/test_cmd.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)      498 2024-04-03 00:27:43.000000 countess-0.0.56/tests/test_gui.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1060 2023-11-09 02:44:32.000000 countess-0.0.56/tests/test_plugins.py
```

### Comparing `countess-0.0.55/LICENSE.txt` & `countess-0.0.56/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `countess-0.0.55/PKG-INFO` & `countess-0.0.56/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: countess
-Version: 0.0.55
+Version: 0.0.56
 Summary: CountESS
 Author-email: Nick Moore <nick@zoic.org>, Alan Rubin <alan@rubin.id.au>
 Maintainer-email: Nick Moore <nick@zoic.org>
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -30,27 +30,28 @@
 Requires-Dist: pylint~=2.17; extra == "dev"
 Requires-Dist: types-psutil~=5.9.5; extra == "dev"
 Requires-Dist: types-ttkthemes~=3.2; extra == "dev"
 Requires-Dist: twine==4.0.2; extra == "dev"
 Requires-Dist: pandas-stubs~=2.1.0; extra == "dev"
 Requires-Dist: pytest~=7.2; extra == "dev"
 
-# CountESS 0.0.55
+# CountESS 0.0.56
 
 This is CountESS, a modular, Python 3 reimplementation of Enrich2.
 
 ## License
 
 BSD 3-clause.  See [LICENSE.txt](LICENSE.txt)
 
 Source code is available at [https://github.com/CountESS-Project/CountESS](https://github.com/CountESS-Project/CountESS) and contributions are welcomed.
 
 ## Installing
 
-The latest version of CountESS can be installed from pypi:
+The latest version of
+[CountESS can be installed from pypi](https://pypi.org/project/countess/):
 ```
 pip install CountESS
 ```
 
 For other options, see the documentation below ...
 
 ## Documentation
```

### Comparing `countess-0.0.55/README.md` & `countess-0.0.56/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-# CountESS 0.0.55
+# CountESS 0.0.56
 
 This is CountESS, a modular, Python 3 reimplementation of Enrich2.
 
 ## License
 
 BSD 3-clause.  See [LICENSE.txt](LICENSE.txt)
 
 Source code is available at [https://github.com/CountESS-Project/CountESS](https://github.com/CountESS-Project/CountESS) and contributions are welcomed.
 
 ## Installing
 
-The latest version of CountESS can be installed from pypi:
+The latest version of
+[CountESS can be installed from pypi](https://pypi.org/project/countess/):
 ```
 pip install CountESS
 ```
 
 For other options, see the documentation below ...
 
 ## Documentation
```

### Comparing `countess-0.0.55/countess/core/config.py` & `countess-0.0.56/countess/core/config.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.55/countess/core/logger.py` & `countess-0.0.56/countess/core/logger.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.55/countess/core/parameters.py` & `countess-0.0.56/countess/core/parameters.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.55/countess/core/pipeline.py` & `countess-0.0.56/countess/core/pipeline.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.55/countess/core/plugins.py` & `countess-0.0.56/countess/core/plugins.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.55/countess/gui/config.py` & `countess-0.0.56/countess/gui/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -322,15 +322,15 @@
             self.entry.grid(row=row, column=2)
 
     def add_row_callback(self, *_):
         assert isinstance(self.parameter, ArrayParam)
 
         if isinstance(self.parameter, FileSaveParam):
             file_types = self.parameter.file_types
-            filename = ask_saveas_filename(file_types)
+            filename = ask_saveas_filename(self.parameter.value, file_types)
             self.parameter.value = filename
         if isinstance(self.parameter, FileArrayParam):
             file_types = self.parameter.file_types
             filenames = ask_open_filenames(file_types)
             self.parameter.add_files(filenames)
         else:
             self.parameter.add_row()
```

### Comparing `countess-0.0.55/countess/gui/logger.py` & `countess-0.0.56/countess/gui/logger.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.55/countess/gui/main.py` & `countess-0.0.56/countess/gui/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import multiprocessing
 import re
 import sys
 import threading
 import tkinter as tk
-from tkinter import filedialog, messagebox, ttk
+from tkinter import messagebox, ttk
 from typing import Optional
 
 import psutil
 
 from countess import VERSION
 from countess.core.config import export_config_graphviz, read_config, write_config
 from countess.core.pipeline import PipelineGraph
 from countess.core.plugins import get_plugin_classes
 from countess.gui.config import PluginConfigurator
 from countess.gui.logger import LoggerFrame
 from countess.gui.mini_browser import MiniBrowserFrame
 from countess.gui.tabular import TabularDataFrame
 from countess.gui.tree import FlippyCanvas, GraphWrapper
-from countess.gui.widgets import info_button
+from countess.gui.widgets import ask_open_filename, ask_saveas_filename, info_button
 from countess.utils.pandas import concat_dataframes
 
 # import faulthandler
 # faulthandler.enable(all_threads=True)
 
 
 plugin_classes = sorted(get_plugin_classes(), key=lambda x: x.name)
@@ -120,16 +120,15 @@
             )
             if self.node.plugin.link:
                 info_button(self.frame, command=self.on_info_button_press).place(anchor=tk.NE, relx=1, y=50)
             # self.node.prepare(self.logger)
             # self.node.plugin.update()
             self.configurator = PluginConfigurator(self.config_canvas, self.node.plugin, self.config_change_callback)
             self.config_subframe = self.configurator.frame
-            self.frame.rowconfigure(3, weight=1)
-            self.frame.rowconfigure(4, weight=1)
+            self.frame.rowconfigure(3, weight=1, minsize=self.frame.winfo_height() / 2)
 
         else:
             has_parents = len(self.node.parent_nodes) > 0
             has_children = len(self.node.child_nodes) > 0
             self.config_subframe = PluginChooserFrame(
                 self.config_canvas, "Choose Plugin", self.choose_plugin, has_parents, has_children
             )
@@ -416,29 +415,29 @@
             self.graph_wrapper.destroy()
         self.graph = PipelineGraph()
         self.graph_wrapper = GraphWrapper(self.canvas, self.graph, self.node_select)
         self.graph_wrapper.add_new_node()
 
     def config_load(self, filename=None):
         if not filename:
-            filename = filedialog.askopenfilename(filetypes=[(".INI Config File", "*.ini")])
+            filename = ask_open_filename(file_types=[(".INI Config File", "*.ini")])
         if not filename:
             return
         self.config_filename = filename
         if self.graph_wrapper:
             self.graph_wrapper.destroy()
         self.graph = read_config(filename)
         self.graph_wrapper = GraphWrapper(self.canvas, self.graph, self.node_select)
         self.node_select(None)
 
     def config_save(self, filename=None):
         if not filename:
-            filename = filedialog.asksaveasfilename(
-                initialfile=self.config_filename,
-                filetypes=[(".INI Config File", "*.ini")],
+            filename = ask_saveas_filename(
+                initial_file=self.config_filename,
+                file_types=[(".INI Config File", "*.ini")],
             )
         if not filename:
             return
         write_config(self.graph, filename)
         self.config_changed = False
         # XXX there should be a self.graph_wrapper.refresh()
         # Names may have changed on save
@@ -447,15 +446,15 @@
 
     def config_export(self, filename=None):
         if not filename:
             if self.config_filename:
                 initialfile = self.config_filename.removesuffix(".ini") + ".dot"
             else:
                 initialfile = None
-            filename = filedialog.asksaveasfilename(initialfile=initialfile, filetypes=[("Graphviz File", "*.dot")])
+            filename = ask_saveas_filename(initial_file=initialfile, file_types=[("Graphviz File", "*.dot")])
         if not filename:
             return
         export_config_graphviz(self.graph, filename)
 
     def graph_tidy(self):
         self.graph.tidy()
         # XXX there should be a self.graph_wrapper.refresh()
```

### Comparing `countess-0.0.55/countess/gui/mini_browser.py` & `countess-0.0.56/countess/gui/mini_browser.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.55/countess/gui/tabular.py` & `countess-0.0.56/countess/gui/tabular.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,15 +265,15 @@
         if descending is None and column_num == self.sort_by_col:
             self.sort_ascending = not self.sort_ascending
         else:
             self.sort_by_col = column_num
             self.sort_ascending = not descending
         if column_num < self.index_cols:
             self.dataframe = self.dataframe.sort_index(level=column_num, ascending=self.sort_ascending)
-        else:
+        elif column_num < self.index_cols + len(self.dataframe.columns):
             self.dataframe = self.dataframe.sort_values(
                 self.dataframe.columns[column_num - self.index_cols], ascending=self.sort_ascending
             )
 
         for n, label in enumerate(self.labels):
             icon = "sort_un" if n != column_num else "sort_up" if self.sort_ascending else "sort_dn"
             label.configure(image=get_icon(self, icon))
```

### Comparing `countess-0.0.55/countess/gui/tree.py` & `countess-0.0.56/countess/gui/tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -355,18 +355,18 @@
         yy = float(label.place_info()["rely"]) * height
         node.position = self.new_node_position(xx, yy)
         label.update_node(node, width < height)
 
         # Adapt label sizes to suit the window size, as best we can ...
         # XXX very arbitrary and definitely open to tweaking
         if height > width:
-            label_max_width = max(width // 9, 25)
+            label_max_width = max(width // 6, 25)
             label_font_size = int(math.sqrt(width) / 3)
         else:
-            label_max_width = max(width // 20, 16)
+            label_max_width = max(width // 12, 16)
             label_font_size = int(math.sqrt(width) / 5)
         label["wraplength"] = label_max_width
         label["font"] = ("TkDefaultFont", label_font_size)
 
     def on_enter(self, node, event):
         """Mouse has entered a label"""
         # don't outline labels while dragging
```

### Comparing `countess-0.0.55/countess/gui/widgets.py` & `countess-0.0.56/countess/gui/widgets.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,16 +90,16 @@
     return [_clean_filetype_extension(ext) for ext in extensions]
 
 
 def _clean_filetypes(file_types: Sequence[Tuple[str, Union[str, List[str]]]]):
     return [(label, _clean_filetype_extensions(extensions)) for label, extensions in file_types]
 
 
-def ask_saveas_filename(file_types: Sequence[Tuple[str, Union[str, List[str]]]]):
-    return filedialog.asksaveasfilename(filetypes=_clean_filetypes(file_types))
+def ask_saveas_filename(initial_file: str, file_types: Sequence[Tuple[str, Union[str, List[str]]]]):
+    return filedialog.asksaveasfilename(initialfile=initial_file, filetypes=_clean_filetypes(file_types))
 
 
 def ask_open_filenames(file_types: Sequence[Tuple[str, Union[str, List[str]]]]):
     return filedialog.askopenfilenames(filetypes=_clean_filetypes(file_types))
 
 
 def ask_open_filename(file_types: Sequence[Tuple[str, Union[str, List[str]]]]):
```

### Comparing `countess-0.0.55/countess/plugins/collate.py` & `countess-0.0.56/countess/plugins/collate.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.55/countess/plugins/column.py` & `countess-0.0.56/countess/plugins/column.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.55/countess/plugins/correlation.py` & `countess-0.0.56/countess/plugins/correlation.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.55/countess/plugins/csv.py` & `countess-0.0.56/countess/plugins/csv.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.55/countess/plugins/data_table.py` & `countess-0.0.56/countess/plugins/data_table.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.55/countess/plugins/expression.py` & `countess-0.0.56/countess/plugins/expression.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.55/countess/plugins/fastq.py` & `countess-0.0.56/countess/plugins/fastq.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.55/countess/plugins/group_by.py` & `countess-0.0.56/countess/plugins/group_by.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.55/countess/plugins/hgvs_parser.py` & `countess-0.0.56/countess/plugins/hgvs_parser.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.55/countess/plugins/join.py` & `countess-0.0.56/countess/plugins/join.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.55/countess/plugins/mutagenize.py` & `countess-0.0.56/countess/plugins/mutagenize.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.55/countess/plugins/pivot.py` & `countess-0.0.56/countess/plugins/pivot.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,16 @@
     return functools.reduce(lambda x, y: x * y, iterable, 1)
 
 
 class PivotPlugin(PandasProcessPlugin):
     """Groups a Pandas Dataframe by an arbitrary column and rolls up rows"""
 
     name = "Pivot Tool"
-    description = """Groups a dataframe and pivots column values into columns.
-        Expanded column values are duplicated for each combination of pivot values.
+    description = "Groups a dataframe and pivots column values into columns."
+    additional = """Expanded column values are duplicated for each combination of pivot values.
         Missing values default to 0, and duplicate values are summed."""
     version = VERSION
     link = "https://countess-project.github.io/CountESS/included-plugins/#pivot-tool"
 
     parameters = {
         "columns": PerColumnArrayParam(
             "Columns", ChoiceParam("Role", "Drop", choices=["Index", "Pivot", "Expand", "Drop"])
```

### Comparing `countess-0.0.55/countess/plugins/python.py` & `countess-0.0.56/countess/plugins/python.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.55/countess/plugins/regex.py` & `countess-0.0.56/countess/plugins/regex.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.55/countess/plugins/sequence.py` & `countess-0.0.56/countess/plugins/sequence.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.55/countess/plugins/variant.py` & `countess-0.0.56/countess/plugins/variant.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.55/countess/utils/pandas.py` & `countess-0.0.56/countess/utils/pandas.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.55/countess/utils/parallel.py` & `countess-0.0.56/countess/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.55/countess/utils/variant.py` & `countess-0.0.56/countess/utils/variant.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.55/countess.egg-info/PKG-INFO` & `countess-0.0.56/countess.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: countess
-Version: 0.0.55
+Version: 0.0.56
 Summary: CountESS
 Author-email: Nick Moore <nick@zoic.org>, Alan Rubin <alan@rubin.id.au>
 Maintainer-email: Nick Moore <nick@zoic.org>
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -30,27 +30,28 @@
 Requires-Dist: pylint~=2.17; extra == "dev"
 Requires-Dist: types-psutil~=5.9.5; extra == "dev"
 Requires-Dist: types-ttkthemes~=3.2; extra == "dev"
 Requires-Dist: twine==4.0.2; extra == "dev"
 Requires-Dist: pandas-stubs~=2.1.0; extra == "dev"
 Requires-Dist: pytest~=7.2; extra == "dev"
 
-# CountESS 0.0.55
+# CountESS 0.0.56
 
 This is CountESS, a modular, Python 3 reimplementation of Enrich2.
 
 ## License
 
 BSD 3-clause.  See [LICENSE.txt](LICENSE.txt)
 
 Source code is available at [https://github.com/CountESS-Project/CountESS](https://github.com/CountESS-Project/CountESS) and contributions are welcomed.
 
 ## Installing
 
-The latest version of CountESS can be installed from pypi:
+The latest version of
+[CountESS can be installed from pypi](https://pypi.org/project/countess/):
 ```
 pip install CountESS
 ```
 
 For other options, see the documentation below ...
 
 ## Documentation
```

### Comparing `countess-0.0.55/countess.egg-info/SOURCES.txt` & `countess-0.0.56/countess.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `countess-0.0.55/countess.egg-info/entry_points.txt` & `countess-0.0.56/countess.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `countess-0.0.55/pyproject.toml` & `countess-0.0.56/pyproject.toml`

 * *Files identical despite different names*

### Comparing `countess-0.0.55/tests/test_plugins.py` & `countess-0.0.56/tests/test_plugins.py`

 * *Files identical despite different names*

