# Comparing `tmp/visaplan.tools-1.3.7.tar.gz` & `tmp/visaplan.tools-1.3.7.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/visaplan.tools-1.3.7.tar", last modified: Wed Oct 27 16:38:42 2021, max compression
+gzip compressed data, was "dist/visaplan.tools-1.3.7.dev2.tar", last modified: Mon Oct 11 15:54:55 2021, max compression
```

## Comparing `visaplan.tools-1.3.7.tar` & `visaplan.tools-1.3.7.dev2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2021-10-27 16:38:42.000000 visaplan.tools-1.3.7/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2021-10-27 16:38:42.000000 visaplan.tools-1.3.7/docs/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    18092 2019-01-30 15:38:46.000000 visaplan.tools-1.3.7/docs/LICENSE.GPL
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      667 2019-11-06 16:42:04.000000 visaplan.tools-1.3.7/docs/LICENSE.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      610 2019-01-30 15:38:46.000000 visaplan.tools-1.3.7/docs/Makefile
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     5445 2019-01-30 15:38:46.000000 visaplan.tools-1.3.7/docs/conf.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      485 2019-01-30 15:38:46.000000 visaplan.tools-1.3.7/docs/index.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      817 2019-01-30 15:38:46.000000 visaplan.tools-1.3.7/docs/make.bat
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       52 2019-01-30 15:38:46.000000 visaplan.tools-1.3.7/docs/modules.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1317 2019-01-30 15:38:46.000000 visaplan.tools-1.3.7/docs/tools.rst
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2021-10-27 16:38:41.000000 visaplan.tools-1.3.7/src/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2021-10-27 16:38:42.000000 visaplan.tools-1.3.7/src/visaplan/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2021-10-27 16:38:42.000000 visaplan.tools-1.3.7/src/visaplan/tools/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)        0 2019-01-30 15:38:46.000000 visaplan.tools-1.3.7/src/visaplan/tools/__init__.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     9354 2021-10-27 16:31:55.000000 visaplan.tools-1.3.7/src/visaplan/tools/_builder.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     4723 2021-09-17 08:21:01.000000 visaplan.tools-1.3.7/src/visaplan/tools/batches.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    13928 2021-10-01 12:02:25.000000 visaplan.tools-1.3.7/src/visaplan/tools/buildout.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    42288 2021-10-27 16:31:55.000000 visaplan.tools-1.3.7/src/visaplan/tools/classes.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    10427 2021-10-27 16:25:24.000000 visaplan.tools-1.3.7/src/visaplan/tools/coding.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      532 2021-10-01 12:02:25.000000 visaplan.tools-1.3.7/src/visaplan/tools/configure.zcml
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3228 2021-10-27 16:34:11.000000 visaplan.tools-1.3.7/src/visaplan/tools/csvfiles.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3842 2021-09-08 12:32:56.000000 visaplan.tools-1.3.7/src/visaplan/tools/dates.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    23417 2021-10-01 12:02:25.000000 visaplan.tools-1.3.7/src/visaplan/tools/debug.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    14685 2021-10-01 12:02:25.000000 visaplan.tools-1.3.7/src/visaplan/tools/dicts.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     6200 2021-09-08 12:32:56.000000 visaplan.tools-1.3.7/src/visaplan/tools/files.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    26184 2021-10-27 16:34:11.000000 visaplan.tools-1.3.7/src/visaplan/tools/html.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     5095 2021-10-01 14:43:44.000000 visaplan.tools-1.3.7/src/visaplan/tools/http.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    19360 2021-10-27 16:25:24.000000 visaplan.tools-1.3.7/src/visaplan/tools/lands0.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    11732 2021-10-01 14:32:56.000000 visaplan.tools-1.3.7/src/visaplan/tools/minifuncs.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     2766 2021-09-08 12:32:56.000000 visaplan.tools-1.3.7/src/visaplan/tools/mock.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     5097 2021-10-27 16:25:24.000000 visaplan.tools-1.3.7/src/visaplan/tools/profile.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    12257 2021-09-08 12:32:56.000000 visaplan.tools-1.3.7/src/visaplan/tools/sequences.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    50519 2021-10-27 16:31:38.000000 visaplan.tools-1.3.7/src/visaplan/tools/sql.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    34061 2020-09-07 00:19:52.000000 visaplan.tools-1.3.7/src/visaplan/tools/sql.py.34776
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     4756 2021-10-01 12:02:25.000000 visaplan.tools-1.3.7/src/visaplan/tools/times.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    16441 2021-10-27 16:34:11.000000 visaplan.tools-1.3.7/src/visaplan/tools/words.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    16520 2021-10-11 14:50:45.000000 visaplan.tools-1.3.7/src/visaplan/tools/words.py.1
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      332 2021-09-08 12:32:56.000000 visaplan.tools-1.3.7/src/visaplan/__init__.py
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2021-10-27 16:38:42.000000 visaplan.tools-1.3.7/src/visaplan.tools.egg-info/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    16542 2021-10-27 16:38:41.000000 visaplan.tools-1.3.7/src/visaplan.tools.egg-info/PKG-INFO
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1293 2021-10-27 16:38:41.000000 visaplan.tools-1.3.7/src/visaplan.tools.egg-info/SOURCES.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)        1 2021-10-27 16:38:41.000000 visaplan.tools-1.3.7/src/visaplan.tools.egg-info/dependency_links.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       53 2021-10-27 16:38:41.000000 visaplan.tools-1.3.7/src/visaplan.tools.egg-info/entry_points.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)        9 2021-10-27 16:38:41.000000 visaplan.tools-1.3.7/src/visaplan.tools.egg-info/namespace_packages.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)        1 2019-01-30 16:36:00.000000 visaplan.tools-1.3.7/src/visaplan.tools.egg-info/not-zip-safe
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       15 2021-10-27 16:38:41.000000 visaplan.tools-1.3.7/src/visaplan.tools.egg-info/requires.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)        9 2021-10-27 16:38:41.000000 visaplan.tools-1.3.7/src/visaplan.tools.egg-info/top_level.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     8091 2021-10-27 16:38:37.000000 visaplan.tools-1.3.7/CHANGES.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       67 2019-01-30 15:38:46.000000 visaplan.tools-1.3.7/CONTRIBUTORS.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      183 2020-01-08 08:43:34.000000 visaplan.tools-1.3.7/MANIFEST.in
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3376 2021-09-08 12:32:57.000000 visaplan.tools-1.3.7/README.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)        6 2021-10-27 16:25:24.000000 visaplan.tools-1.3.7/VERSION
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       88 2021-10-06 08:34:26.000000 visaplan.tools-1.3.7/pyproject.toml
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1396 2021-10-27 16:38:42.000000 visaplan.tools-1.3.7/setup.cfg
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     5939 2021-10-06 08:34:26.000000 visaplan.tools-1.3.7/setup.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    16542 2021-10-27 16:38:42.000000 visaplan.tools-1.3.7/PKG-INFO
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2021-10-11 15:54:55.000000 visaplan.tools-1.3.7.dev2/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2021-10-11 15:54:55.000000 visaplan.tools-1.3.7.dev2/docs/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    18092 2019-01-30 15:38:46.000000 visaplan.tools-1.3.7.dev2/docs/LICENSE.GPL
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      667 2019-11-06 16:42:04.000000 visaplan.tools-1.3.7.dev2/docs/LICENSE.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      610 2019-01-30 15:38:46.000000 visaplan.tools-1.3.7.dev2/docs/Makefile
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     5445 2019-01-30 15:38:46.000000 visaplan.tools-1.3.7.dev2/docs/conf.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      485 2019-01-30 15:38:46.000000 visaplan.tools-1.3.7.dev2/docs/index.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      817 2019-01-30 15:38:46.000000 visaplan.tools-1.3.7.dev2/docs/make.bat
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       52 2019-01-30 15:38:46.000000 visaplan.tools-1.3.7.dev2/docs/modules.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1317 2019-01-30 15:38:46.000000 visaplan.tools-1.3.7.dev2/docs/tools.rst
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2021-10-11 15:54:55.000000 visaplan.tools-1.3.7.dev2/src/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2021-10-11 15:54:55.000000 visaplan.tools-1.3.7.dev2/src/visaplan/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2021-10-11 15:54:55.000000 visaplan.tools-1.3.7.dev2/src/visaplan/tools/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)        0 2019-01-30 15:38:46.000000 visaplan.tools-1.3.7.dev2/src/visaplan/tools/__init__.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     4723 2021-09-17 08:21:01.000000 visaplan.tools-1.3.7.dev2/src/visaplan/tools/batches.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    13928 2021-10-01 12:02:25.000000 visaplan.tools-1.3.7.dev2/src/visaplan/tools/buildout.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    42288 2021-10-06 08:54:07.000000 visaplan.tools-1.3.7.dev2/src/visaplan/tools/classes.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    10438 2021-10-06 10:10:32.000000 visaplan.tools-1.3.7.dev2/src/visaplan/tools/coding.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      532 2021-10-01 12:02:25.000000 visaplan.tools-1.3.7.dev2/src/visaplan/tools/configure.zcml
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3247 2021-10-11 08:35:21.000000 visaplan.tools-1.3.7.dev2/src/visaplan/tools/csvfiles.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3842 2021-09-08 12:32:56.000000 visaplan.tools-1.3.7.dev2/src/visaplan/tools/dates.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    23417 2021-10-01 12:02:25.000000 visaplan.tools-1.3.7.dev2/src/visaplan/tools/debug.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    14685 2021-10-01 12:02:25.000000 visaplan.tools-1.3.7.dev2/src/visaplan/tools/dicts.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     6200 2021-09-08 12:32:56.000000 visaplan.tools-1.3.7.dev2/src/visaplan/tools/files.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    25161 2021-10-11 12:18:07.000000 visaplan.tools-1.3.7.dev2/src/visaplan/tools/html.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     5095 2021-10-01 14:43:44.000000 visaplan.tools-1.3.7.dev2/src/visaplan/tools/http.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    19314 2021-10-01 14:43:44.000000 visaplan.tools-1.3.7.dev2/src/visaplan/tools/lands0.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    11732 2021-10-01 14:32:56.000000 visaplan.tools-1.3.7.dev2/src/visaplan/tools/minifuncs.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     2766 2021-09-08 12:32:56.000000 visaplan.tools-1.3.7.dev2/src/visaplan/tools/mock.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     5097 2021-10-11 08:35:21.000000 visaplan.tools-1.3.7.dev2/src/visaplan/tools/profile.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    12257 2021-09-08 12:32:56.000000 visaplan.tools-1.3.7.dev2/src/visaplan/tools/sequences.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    50507 2021-10-06 10:10:32.000000 visaplan.tools-1.3.7.dev2/src/visaplan/tools/sql.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    34061 2020-09-07 00:19:52.000000 visaplan.tools-1.3.7.dev2/src/visaplan/tools/sql.py.34776
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     4756 2021-10-01 12:02:25.000000 visaplan.tools-1.3.7.dev2/src/visaplan/tools/times.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    16405 2021-10-11 15:52:23.000000 visaplan.tools-1.3.7.dev2/src/visaplan/tools/words.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    16520 2021-10-11 14:50:45.000000 visaplan.tools-1.3.7.dev2/src/visaplan/tools/words.py.1
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      332 2021-09-08 12:32:56.000000 visaplan.tools-1.3.7.dev2/src/visaplan/__init__.py
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2021-10-11 15:54:55.000000 visaplan.tools-1.3.7.dev2/src/visaplan.tools.egg-info/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    16504 2021-10-11 15:54:55.000000 visaplan.tools-1.3.7.dev2/src/visaplan.tools.egg-info/PKG-INFO
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1277 2021-10-11 15:54:55.000000 visaplan.tools-1.3.7.dev2/src/visaplan.tools.egg-info/SOURCES.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)        1 2021-10-11 15:54:55.000000 visaplan.tools-1.3.7.dev2/src/visaplan.tools.egg-info/dependency_links.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       53 2021-10-11 15:54:55.000000 visaplan.tools-1.3.7.dev2/src/visaplan.tools.egg-info/entry_points.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)        9 2021-10-11 15:54:55.000000 visaplan.tools-1.3.7.dev2/src/visaplan.tools.egg-info/namespace_packages.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)        1 2019-01-30 16:36:00.000000 visaplan.tools-1.3.7.dev2/src/visaplan.tools.egg-info/not-zip-safe
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       15 2021-10-11 15:54:55.000000 visaplan.tools-1.3.7.dev2/src/visaplan.tools.egg-info/requires.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)        9 2021-10-11 15:54:55.000000 visaplan.tools-1.3.7.dev2/src/visaplan.tools.egg-info/top_level.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     8056 2021-10-11 15:38:59.000000 visaplan.tools-1.3.7.dev2/CHANGES.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       67 2019-01-30 15:38:46.000000 visaplan.tools-1.3.7.dev2/CONTRIBUTORS.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      183 2020-01-08 08:43:34.000000 visaplan.tools-1.3.7.dev2/MANIFEST.in
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3376 2021-09-08 12:32:57.000000 visaplan.tools-1.3.7.dev2/README.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)        6 2021-10-11 08:35:21.000000 visaplan.tools-1.3.7.dev2/VERSION
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)        6 2021-10-11 12:08:02.000000 visaplan.tools-1.3.7.dev2/VERSION_SUFFIX
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       88 2021-10-06 08:34:26.000000 visaplan.tools-1.3.7.dev2/pyproject.toml
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1396 2021-10-11 15:54:55.000000 visaplan.tools-1.3.7.dev2/setup.cfg
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     5939 2021-10-06 08:34:26.000000 visaplan.tools-1.3.7.dev2/setup.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    16504 2021-10-11 15:54:55.000000 visaplan.tools-1.3.7.dev2/PKG-INFO
```

### Comparing `visaplan.tools-1.3.7/docs/LICENSE.GPL` & `visaplan.tools-1.3.7.dev2/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `visaplan.tools-1.3.7/docs/LICENSE.rst` & `visaplan.tools-1.3.7.dev2/docs/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `visaplan.tools-1.3.7/docs/Makefile` & `visaplan.tools-1.3.7.dev2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `visaplan.tools-1.3.7/docs/conf.py` & `visaplan.tools-1.3.7.dev2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `visaplan.tools-1.3.7/docs/make.bat` & `visaplan.tools-1.3.7.dev2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `visaplan.tools-1.3.7/docs/tools.rst` & `visaplan.tools-1.3.7.dev2/docs/tools.rst`

 * *Files identical despite different names*

### Comparing `visaplan.tools-1.3.7/src/visaplan/tools/batches.py` & `visaplan.tools-1.3.7.dev2/src/visaplan/tools/batches.py`

 * *Files identical despite different names*

### Comparing `visaplan.tools-1.3.7/src/visaplan/tools/buildout.py` & `visaplan.tools-1.3.7.dev2/src/visaplan/tools/buildout.py`

 * *Files identical despite different names*

### Comparing `visaplan.tools-1.3.7/src/visaplan/tools/classes.py` & `visaplan.tools-1.3.7.dev2/src/visaplan/tools/classes.py`

 * *Files identical despite different names*

### Comparing `visaplan.tools-1.3.7/src/visaplan/tools/coding.py` & `visaplan.tools-1.3.7.dev2/src/visaplan/tools/coding.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 """\
 Coding/Decoding tools
 """
 
 # Python compatibility:
 from __future__ import absolute_import, print_function
 
+import six
 from six import text_type as six_text_type
 from six.moves import map
 
 __author__ = "Tobias Herp <tobias.herp@visaplan.com>"
 VERSION = (0,
            4,  # make_safe_decoder
            1,  # Bugfix (__all__)
```

### Comparing `visaplan.tools-1.3.7/src/visaplan/tools/configure.zcml` & `visaplan.tools-1.3.7.dev2/src/visaplan/tools/configure.zcml`

 * *Files identical despite different names*

### Comparing `visaplan.tools-1.3.7/src/visaplan/tools/csvfiles.py` & `visaplan.tools-1.3.7.dev2/src/visaplan/tools/csvfiles.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 CSV support: create Excel(tm)-compatible CSV files (semicolon, UTF-8)
 """
 
 # Python compatibility:
 from __future__ import absolute_import
 
 # Standard library:
-import csv
 import sys
-from codecs import BOM_UTF8
-
 if sys.version_info > (3,):
    # Standard library:
    from io.StringIO import StringIO
 else:
    # Standard library (Python 2):
    from StringIO import StringIO
 
+# Standard library:
+import csv
+from codecs import BOM_UTF8
 
 __all__ = ['ExcelSSV',  # Excel+ssv (semicolon-separated values)
            'csv_writer',
            'make_sequencer',
            ]
 
 # ----------------------- [ aus Products.unitracc.tools.csvfiles ... [
```

### Comparing `visaplan.tools-1.3.7/src/visaplan/tools/dates.py` & `visaplan.tools-1.3.7.dev2/src/visaplan/tools/dates.py`

 * *Files identical despite different names*

### Comparing `visaplan.tools-1.3.7/src/visaplan/tools/debug.py` & `visaplan.tools-1.3.7.dev2/src/visaplan/tools/debug.py`

 * *Files identical despite different names*

### Comparing `visaplan.tools-1.3.7/src/visaplan/tools/dicts.py` & `visaplan.tools-1.3.7.dev2/src/visaplan/tools/dicts.py`

 * *Files identical despite different names*

### Comparing `visaplan.tools-1.3.7/src/visaplan/tools/files.py` & `visaplan.tools-1.3.7.dev2/src/visaplan/tools/files.py`

 * *Files identical despite different names*

### Comparing `visaplan.tools-1.3.7/src/visaplan/tools/html.py` & `visaplan.tools-1.3.7.dev2/src/visaplan/tools/html.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,49 +36,18 @@
     ...       'joiner': ' '}  # allow for whitespace normalization
     >>> make_picture(widths=(300, 600), **kw)  # doctest: +NORMALIZE_WHITESPACE
     '<img srcset="/++images++/babyface-300.jpg 300w,
                   /++images++/babyface-600.jpg 600w"
           src="/++images++/babyface-300.jpg"
           alt="">'
 
-The from_plain_text function converts simple text/plain strings to HTML,
-supporting paragraphs and unordered lists:
-
-    >>> plain = (u'''
-    ... %(bull)s foo
-    ... %(bull)s bar
-    ...
-    ... And now for something completely different %(hellip)s'''
-    ... ) % entity
-    >>> print(plain.encode('utf-8'))
-    <BLANKLINE>
-    • foo
-    • bar
-    <BLANKLINE>
-    And now for something completely different …
-    >>> from_plain_text(plain,
-    ...                joiner=u' ')  # doctest: +NORMALIZE_WHITESPACE
-    u'<ul> <li> foo <li> bar
-     </ul>
-      <p> And now for something completely different \u2026'
-
-    >>> from_plain_text(u'''
-    ... %(bull)s foo
-    ... %(bull)s bar
-    ...
-    ... And now for something completely different %(hellip)s'''
-    ... % entity, joiner=u' ')  # doctest: +NORMALIZE_WHITESPACE
-    u'<ul> <li> foo <li> bar
-     </ul>
-      <p> And now for something completely different \u2026'
-
 """
 
 # Python compatibility:
-from __future__ import absolute_import, print_function
+from __future__ import absolute_import
 
 import six
 from six import text_type as six_text_type
 from six import unichr
 from six.moves.html_entities import name2codepoint
 
 # Standard library:
@@ -91,22 +60,20 @@
 except ImportError:
     # Standard library:
     from cgi import escape as cgi_escape
     def html_escape(s):
         return cgi_escape(s, quote=1)
 
 # Local imports:
-from visaplan.tools._builder import from_plain_text
 from visaplan.tools.sequences import sequence_slide
 
 __all__ = [
     'entity',  # an --> HtmlEntityProxy
     'entity_aware',
     'make_picture',
-    'from_plain_text',
     ## caution; not stable yet, regarding breaking vs. non-breaking space:
     # 'collapse_whitespace',
     ]
 
 # ------------------------------------------------------ [ Daten ... [
 # Blockelemente: hier als solche Elemente verstanden, die in einem <p>, <span>
 # oder <a> nicht vorkommen dürfen
@@ -758,12 +725,12 @@
 
 
 if __name__ == '__main__':
   if 0:
       from pdb import set_trace; set_trace()
       generator = entity_aware('Au&#195;&#159;en')
       res = list(generator)
-      print(res)
+      print res
   else:
     # Standard library:
     import doctest
     doctest.testmod()
```

### Comparing `visaplan.tools-1.3.7/src/visaplan/tools/http.py` & `visaplan.tools-1.3.7.dev2/src/visaplan/tools/http.py`

 * *Files identical despite different names*

### Comparing `visaplan.tools-1.3.7/src/visaplan/tools/lands0.py` & `visaplan.tools-1.3.7.dev2/src/visaplan/tools/lands0.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,16 +268,14 @@
     ['abc']
 
     Im einfachsten Fall wird die Zeichenkette wortweise aufgesplittet:
     >>> list_of_strings(' eins  zwei ')
     ['eins', 'zwei']
     >>> list_of_strings('  ')
     []
-    >>> list_of_strings(' all\n')
-    ['all']
 
     Wird ein "falscher" Wert (außer dem Vorgabewert None) als splitfunc
     übergeben, dann wird zumindest strip angewendet
     (was bei split impliziert ist):
 
     >>> list_of_strings(' eins  zwei ', splitfunc=False)
     ['eins  zwei']
```

### Comparing `visaplan.tools-1.3.7/src/visaplan/tools/minifuncs.py` & `visaplan.tools-1.3.7.dev2/src/visaplan/tools/minifuncs.py`

 * *Files identical despite different names*

### Comparing `visaplan.tools-1.3.7/src/visaplan/tools/mock.py` & `visaplan.tools-1.3.7.dev2/src/visaplan/tools/mock.py`

 * *Files identical despite different names*

### Comparing `visaplan.tools-1.3.7/src/visaplan/tools/profile.py` & `visaplan.tools-1.3.7.dev2/src/visaplan/tools/profile.py`

 * *Files identical despite different names*

### Comparing `visaplan.tools-1.3.7/src/visaplan/tools/sequences.py` & `visaplan.tools-1.3.7.dev2/src/visaplan/tools/sequences.py`

 * *Files identical despite different names*

### Comparing `visaplan.tools-1.3.7/src/visaplan/tools/sql.py` & `visaplan.tools-1.3.7.dev2/src/visaplan/tools/sql.py`

 * *Files 0% similar despite different names*

```diff
@@ -741,15 +741,15 @@
             falsy_empty = kwargs.pop('falsy_lists_considered_empty', 0)
             noempty = falsy_empty
 
     def sql_subdict(source, fields=None, pop=do_pop):
         get = pop and source.pop or source.get
         res = {}
         if fields is None:
-            fields = list(source.keys())  # we iterate this once only
+            fields = source.keys()  # we iterate this once only
         elif isinstance(fields, six_string_types):
             fields = fields.split()
         for field in fields:
             if field in source:
                 res[field] = get(field)
         return res
 
@@ -758,15 +758,15 @@
 
     isempty = _make_empty_detector(empty_values, falsy_empty)
 
     def sql_subdict_noempty(source, fields=None, pop=do_pop):
         get = pop and source.pop or source.get
         res = {}
         if fields is None:
-            fields = list(source.keys())  # we iterate this once only
+            fields = source.keys()  # we iterate this once only
         elif isinstance(fields, six_string_types):
             fields = fields.split()
         for field in fields:
             if field in source:
                 val = get(field)
                 if not isempty(val):
                     res[field] = val
```

### Comparing `visaplan.tools-1.3.7/src/visaplan/tools/sql.py.34776` & `visaplan.tools-1.3.7.dev2/src/visaplan/tools/sql.py.34776`

 * *Files identical despite different names*

### Comparing `visaplan.tools-1.3.7/src/visaplan/tools/times.py` & `visaplan.tools-1.3.7.dev2/src/visaplan/tools/times.py`

 * *Files identical despite different names*

### Comparing `visaplan.tools-1.3.7/src/visaplan/tools/words.py` & `visaplan.tools-1.3.7.dev2/src/visaplan/tools/words.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # -*- coding: utf-8 -*- vim: ts=8 sts=4 sw=4 si et tw=79 cc=+1
 """
 words - split strings into words
 """
 
 # Python compatibility:
-from __future__ import absolute_import, print_function
+from __future__ import absolute_import
 
 import six
 from six import string_types as six_string_types
 from six import text_type as six_text_type
 
 # Local imports:
-from visaplan.tools.html import entity_aware
 from visaplan.tools.sequences import sequence_slide
+from visaplan.tools.html import entity_aware
 
 __all__ = [
     'head',  # return the first fuzzy NN characters
     ]
 
 
 def _head_kwargs(kw):
@@ -330,15 +330,15 @@
         'chars_prev': 0,
         'result': None,
         }
     chars = kw['chars']
     words = kw['words']
     ellipsis = kw['ellipsis']
     ellipsis_list = list(ellipsis)
-
+    
     if kw['return_tuple']:
         def RESULT():
             return join(tmp), len(tmp)
     else:
         def RESULT():
             return join(tmp)
 
@@ -464,10 +464,9 @@
   if 0:
       s3 = (' The quick brown fox  jumps over the refrigerator. ')
       from pdb import set_trace; set_trace()
       res3 = head(s3, chars=40, fuzz=2, return_tuple=1)
       res3 == 'The quick brown fox jumps over the refrige...'[0]
       print(res3)
   else:
-    # Standard library:
     import doctest
     doctest.testmod()
```

### Comparing `visaplan.tools-1.3.7/src/visaplan/tools/words.py.1` & `visaplan.tools-1.3.7.dev2/src/visaplan/tools/words.py.1`

 * *Files identical despite different names*

### Comparing `visaplan.tools-1.3.7/src/visaplan.tools.egg-info/PKG-INFO` & `visaplan.tools-1.3.7.dev2/src/visaplan.tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visaplan.tools
-Version: 1.3.7
+Version: 1.3.7.dev2
 Summary: General Python tools
 Home-page: UNKNOWN
 Author: Tobias Herp
 Author-email: tobias.herp@visaplan.com
 License: GPL version 2
 Project-URL: Source, https://github.com/visaplan/visaplan.tools
 Project-URL: Tests, https://travis-ci.org/visaplan/visaplan.tools
@@ -174,22 +174,21 @@
         
           - ``http_statustext``, because of questionable `func` option
           - ``make_url``
         
         [tobiasherp]
         
         
-        1.3.7 (2021-10-27)
+        1.3.7 (unreleased)
         ------------------
         
         New Features:
         
         - ``.html`` module:
         
-          - new function `from_plain_text`
           - new character generator `entity_aware`
         
         - ``.words`` module:
         
           - New options for `head`:
         
             - `detect_entities` (using ``.html.entity_aware``)
```

### Comparing `visaplan.tools-1.3.7/src/visaplan.tools.egg-info/SOURCES.txt` & `visaplan.tools-1.3.7.dev2/src/visaplan.tools.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 CHANGES.rst
 CONTRIBUTORS.rst
 MANIFEST.in
 README.rst
 VERSION
+VERSION_SUFFIX
 pyproject.toml
 setup.cfg
 setup.py
 docs/LICENSE.GPL
 docs/LICENSE.rst
 docs/Makefile
 docs/conf.py
@@ -20,15 +21,14 @@
 src/visaplan.tools.egg-info/dependency_links.txt
 src/visaplan.tools.egg-info/entry_points.txt
 src/visaplan.tools.egg-info/namespace_packages.txt
 src/visaplan.tools.egg-info/not-zip-safe
 src/visaplan.tools.egg-info/requires.txt
 src/visaplan.tools.egg-info/top_level.txt
 src/visaplan/tools/__init__.py
-src/visaplan/tools/_builder.py
 src/visaplan/tools/batches.py
 src/visaplan/tools/buildout.py
 src/visaplan/tools/classes.py
 src/visaplan/tools/coding.py
 src/visaplan/tools/configure.zcml
 src/visaplan/tools/csvfiles.py
 src/visaplan/tools/dates.py
```

### Comparing `visaplan.tools-1.3.7/CHANGES.rst` & `visaplan.tools-1.3.7.dev2/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -20,22 +20,21 @@
 
   - ``http_statustext``, because of questionable `func` option
   - ``make_url``
 
 [tobiasherp]
 
 
-1.3.7 (2021-10-27)
+1.3.7 (unreleased)
 ------------------
 
 New Features:
 
 - ``.html`` module:
 
-  - new function `from_plain_text`
   - new character generator `entity_aware`
 
 - ``.words`` module:
 
   - New options for `head`:
 
     - `detect_entities` (using ``.html.entity_aware``)
```

### Comparing `visaplan.tools-1.3.7/README.rst` & `visaplan.tools-1.3.7.dev2/README.rst`

 * *Files identical despite different names*

### Comparing `visaplan.tools-1.3.7/setup.cfg` & `visaplan.tools-1.3.7.dev2/setup.cfg`

 * *Files identical despite different names*

### Comparing `visaplan.tools-1.3.7/setup.py` & `visaplan.tools-1.3.7.dev2/setup.py`

 * *Files identical despite different names*

### Comparing `visaplan.tools-1.3.7/PKG-INFO` & `visaplan.tools-1.3.7.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visaplan.tools
-Version: 1.3.7
+Version: 1.3.7.dev2
 Summary: General Python tools
 Home-page: UNKNOWN
 Author: Tobias Herp
 Author-email: tobias.herp@visaplan.com
 License: GPL version 2
 Project-URL: Source, https://github.com/visaplan/visaplan.tools
 Project-URL: Tests, https://travis-ci.org/visaplan/visaplan.tools
@@ -174,22 +174,21 @@
         
           - ``http_statustext``, because of questionable `func` option
           - ``make_url``
         
         [tobiasherp]
         
         
-        1.3.7 (2021-10-27)
+        1.3.7 (unreleased)
         ------------------
         
         New Features:
         
         - ``.html`` module:
         
-          - new function `from_plain_text`
           - new character generator `entity_aware`
         
         - ``.words`` module:
         
           - New options for `head`:
         
             - `detect_entities` (using ``.html.entity_aware``)
```

