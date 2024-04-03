# Comparing `tmp/logger-36-2024.5.tar.gz` & `tmp/logger-36-2024.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logger-36-2024.5.tar", last modified: Wed Apr  3 07:02:42 2024, max compression
+gzip compressed data, was "logger-36-2024.6.tar", last modified: Wed Apr  3 16:11:17 2024, max compression
```

## Comparing `logger-36-2024.5.tar` & `logger-36-2024.6.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 07:02:42.705098 logger-36-2024.5/
--rwx------   0 eric      (1000) users      (984)      114 2022-10-14 06:42:17.000000 logger-36-2024.5/MANIFEST.in
--rw-r--r--   0 eric      (1000) users      (984)     4246 2024-04-03 07:02:42.705098 logger-36-2024.5/PKG-INFO
--rwx------   0 eric      (1000) users      (984)      636 2023-02-17 08:45:51.000000 logger-36-2024.5/README-COPYRIGHT-utf8.txt
--rwx------   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 logger-36-2024.5/README-LICENCE-utf8.txt
--rwx------   0 eric      (1000) users      (984)     3458 2023-02-17 09:17:51.000000 logger-36-2024.5/README.rst
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 07:02:42.698431 logger-36-2024.5/documentation/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 07:02:42.698431 logger-36-2024.5/documentation/wiki/
--rwx------   0 eric      (1000) users      (984)     1867 2024-03-29 10:17:44.000000 logger-36-2024.5/documentation/wiki/description.asciidoc
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 07:02:42.701764 logger-36-2024.5/logger_36/
--rwx------   0 eric      (1000) users      (984)     1756 2024-03-15 21:24:09.000000 logger-36-2024.5/logger_36/__init__.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 07:02:42.698431 logger-36-2024.5/logger_36/catalog/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 07:02:42.701764 logger-36-2024.5/logger_36/catalog/config/
--rw-r--r--   0 eric      (1000) users      (984)     2030 2024-03-28 08:18:21.000000 logger-36-2024.5/logger_36/catalog/config/console_rich.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 07:02:42.701764 logger-36-2024.5/logger_36/catalog/handler/
--rw-r--r--   0 eric      (1000) users      (984)     3092 2024-03-27 17:11:48.000000 logger-36-2024.5/logger_36/catalog/handler/console.py
--rwx------   0 eric      (1000) users      (984)     5395 2024-03-28 09:36:54.000000 logger-36-2024.5/logger_36/catalog/handler/console_rich.py
--rwx------   0 eric      (1000) users      (984)     3507 2024-03-27 17:11:54.000000 logger-36-2024.5/logger_36/catalog/handler/file.py
--rwx------   0 eric      (1000) users      (984)     5931 2024-03-27 17:12:07.000000 logger-36-2024.5/logger_36/catalog/handler/generic.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 07:02:42.701764 logger-36-2024.5/logger_36/catalog/logging/
--rw-r--r--   0 eric      (1000) users      (984)     1814 2024-03-27 17:05:43.000000 logger-36-2024.5/logger_36/catalog/logging/chronos.py
--rw-r--r--   0 eric      (1000) users      (984)     2465 2024-03-27 17:05:43.000000 logger-36-2024.5/logger_36/catalog/logging/gpu.py
--rw-r--r--   0 eric      (1000) users      (984)     4038 2024-03-28 09:46:44.000000 logger-36-2024.5/logger_36/catalog/logging/memory.py
--rw-r--r--   0 eric      (1000) users      (984)     2447 2024-03-27 17:20:41.000000 logger-36-2024.5/logger_36/catalog/logging/system.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 07:02:42.701764 logger-36-2024.5/logger_36/config/
--rw-r--r--   0 eric      (1000) users      (984)     1637 2024-03-29 09:47:00.000000 logger-36-2024.5/logger_36/config/issue.py
--rw-r--r--   0 eric      (1000) users      (984)     1587 2024-03-28 09:30:00.000000 logger-36-2024.5/logger_36/config/memory.py
--rwx------   0 eric      (1000) users      (984)     2056 2024-03-28 08:16:13.000000 logger-36-2024.5/logger_36/config/message.py
--rw-r--r--   0 eric      (1000) users      (984)     1847 2024-03-27 17:18:16.000000 logger-36-2024.5/logger_36/config/system.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 07:02:42.701764 logger-36-2024.5/logger_36/constant/
--rw-r--r--   0 eric      (1000) users      (984)     1614 2024-03-27 18:55:10.000000 logger-36-2024.5/logger_36/constant/generic.py
--rwx------   0 eric      (1000) users      (984)     1681 2024-03-27 18:54:51.000000 logger-36-2024.5/logger_36/constant/handler.py
--rw-r--r--   0 eric      (1000) users      (984)     1656 2024-03-28 09:36:45.000000 logger-36-2024.5/logger_36/constant/issue.py
--rw-r--r--   0 eric      (1000) users      (984)     2150 2024-03-28 09:06:53.000000 logger-36-2024.5/logger_36/constant/logger.py
--rw-r--r--   0 eric      (1000) users      (984)     1795 2024-03-28 09:36:54.000000 logger-36-2024.5/logger_36/constant/memory.py
--rw-r--r--   0 eric      (1000) users      (984)     2084 2024-03-27 18:54:51.000000 logger-36-2024.5/logger_36/constant/message.py
--rw-r--r--   0 eric      (1000) users      (984)     1681 2024-03-27 17:02:29.000000 logger-36-2024.5/logger_36/constant/record.py
--rw-r--r--   0 eric      (1000) users      (984)     1800 2024-03-27 18:54:51.000000 logger-36-2024.5/logger_36/constant/system.py
--rw-r--r--   0 eric      (1000) users      (984)     1616 2024-03-06 14:38:47.000000 logger-36-2024.5/logger_36/instance.py
--rwx------   0 eric      (1000) users      (984)     6587 2024-04-03 06:48:53.000000 logger-36-2024.5/logger_36/main.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 07:02:42.705098 logger-36-2024.5/logger_36/task/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 07:02:42.705098 logger-36-2024.5/logger_36/task/format/
--rw-r--r--   0 eric      (1000) users      (984)     3610 2024-03-28 09:36:54.000000 logger-36-2024.5/logger_36/task/format/memory.py
--rw-r--r--   0 eric      (1000) users      (984)     3511 2024-03-27 18:54:51.000000 logger-36-2024.5/logger_36/task/format/message.py
--rw-r--r--   0 eric      (1000) users      (984)     1968 2024-03-12 15:08:33.000000 logger-36-2024.5/logger_36/task/format/rule.py
--rwx------   0 eric      (1000) users      (984)     4397 2024-03-07 16:54:56.000000 logger-36-2024.5/logger_36/task/inspection.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 07:02:42.705098 logger-36-2024.5/logger_36/task/measure/
--rwx------   0 eric      (1000) users      (984)     2253 2024-03-27 17:27:28.000000 logger-36-2024.5/logger_36/task/measure/chronos.py
--rwx------   0 eric      (1000) users      (984)     1874 2024-03-27 18:39:46.000000 logger-36-2024.5/logger_36/task/measure/memory.py
--rw-r--r--   0 eric      (1000) users      (984)     5026 2024-03-29 09:49:15.000000 logger-36-2024.5/logger_36/task/storage.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 07:02:42.705098 logger-36-2024.5/logger_36/type/
--rwx------   0 eric      (1000) users      (984)     5198 2024-03-27 18:54:51.000000 logger-36-2024.5/logger_36/type/extension.py
--rw-r--r--   0 eric      (1000) users      (984)     2151 2024-03-29 09:46:52.000000 logger-36-2024.5/logger_36/type/issue.py
--rw-r--r--   0 eric      (1000) users      (984)    12729 2024-04-03 06:51:24.000000 logger-36-2024.5/logger_36/type/logger.py
--rwx------   0 eric      (1000) users      (984)     1575 2024-04-03 06:53:26.000000 logger-36-2024.5/logger_36/version.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 07:02:42.705098 logger-36-2024.5/logger_36.egg-info/
--rw-r--r--   0 eric      (1000) users      (984)     4246 2024-04-03 07:02:42.000000 logger-36-2024.5/logger_36.egg-info/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)     1320 2024-04-03 07:02:42.000000 logger-36-2024.5/logger_36.egg-info/SOURCES.txt
--rw-r--r--   0 eric      (1000) users      (984)        1 2024-04-03 07:02:42.000000 logger-36-2024.5/logger_36.egg-info/dependency_links.txt
--rw-r--r--   0 eric      (1000) users      (984)       10 2024-04-03 07:02:42.000000 logger-36-2024.5/logger_36.egg-info/top_level.txt
--rwx------   0 eric      (1000) users      (984)      104 2022-06-17 10:26:30.000000 logger-36-2024.5/pyproject.toml
--rw-r--r--   0 eric      (1000) users      (984)       38 2024-04-03 07:02:42.705098 logger-36-2024.5/setup.cfg
--rwx------   0 eric      (1000) users      (984)     5533 2024-04-03 07:02:21.000000 logger-36-2024.5/setup.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 16:11:17.851893 logger-36-2024.6/
+-rwx------   0 eric      (1000) users      (984)      114 2022-10-14 06:42:17.000000 logger-36-2024.6/MANIFEST.in
+-rw-r--r--   0 eric      (1000) users      (984)     4246 2024-04-03 16:11:17.851893 logger-36-2024.6/PKG-INFO
+-rwx------   0 eric      (1000) users      (984)      636 2023-02-17 08:45:51.000000 logger-36-2024.6/README-COPYRIGHT-utf8.txt
+-rwx------   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 logger-36-2024.6/README-LICENCE-utf8.txt
+-rwx------   0 eric      (1000) users      (984)     3458 2023-02-17 09:17:51.000000 logger-36-2024.6/README.rst
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 16:11:17.838559 logger-36-2024.6/documentation/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 16:11:17.841893 logger-36-2024.6/documentation/wiki/
+-rwx------   0 eric      (1000) users      (984)     1867 2024-03-29 10:17:44.000000 logger-36-2024.6/documentation/wiki/description.asciidoc
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 16:11:17.841893 logger-36-2024.6/logger_36/
+-rwx------   0 eric      (1000) users      (984)     1756 2024-03-15 21:24:09.000000 logger-36-2024.6/logger_36/__init__.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 16:11:17.838559 logger-36-2024.6/logger_36/catalog/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 16:11:17.841893 logger-36-2024.6/logger_36/catalog/config/
+-rw-r--r--   0 eric      (1000) users      (984)     2030 2024-03-28 08:18:21.000000 logger-36-2024.6/logger_36/catalog/config/console_rich.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 16:11:17.845226 logger-36-2024.6/logger_36/catalog/handler/
+-rw-r--r--   0 eric      (1000) users      (984)     3092 2024-03-27 17:11:48.000000 logger-36-2024.6/logger_36/catalog/handler/console.py
+-rwx------   0 eric      (1000) users      (984)     6512 2024-04-03 16:05:44.000000 logger-36-2024.6/logger_36/catalog/handler/console_rich.py
+-rwx------   0 eric      (1000) users      (984)     3507 2024-03-27 17:11:54.000000 logger-36-2024.6/logger_36/catalog/handler/file.py
+-rwx------   0 eric      (1000) users      (984)     5931 2024-03-27 17:12:07.000000 logger-36-2024.6/logger_36/catalog/handler/generic.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 16:11:17.845226 logger-36-2024.6/logger_36/catalog/logging/
+-rw-r--r--   0 eric      (1000) users      (984)     1814 2024-03-27 17:05:43.000000 logger-36-2024.6/logger_36/catalog/logging/chronos.py
+-rw-r--r--   0 eric      (1000) users      (984)     2465 2024-03-27 17:05:43.000000 logger-36-2024.6/logger_36/catalog/logging/gpu.py
+-rw-r--r--   0 eric      (1000) users      (984)     4038 2024-03-28 09:46:44.000000 logger-36-2024.6/logger_36/catalog/logging/memory.py
+-rw-r--r--   0 eric      (1000) users      (984)     2447 2024-03-27 17:20:41.000000 logger-36-2024.6/logger_36/catalog/logging/system.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 16:11:17.845226 logger-36-2024.6/logger_36/config/
+-rw-r--r--   0 eric      (1000) users      (984)     1637 2024-03-29 09:47:00.000000 logger-36-2024.6/logger_36/config/issue.py
+-rw-r--r--   0 eric      (1000) users      (984)     1587 2024-03-28 09:30:00.000000 logger-36-2024.6/logger_36/config/memory.py
+-rwx------   0 eric      (1000) users      (984)     2056 2024-03-28 08:16:13.000000 logger-36-2024.6/logger_36/config/message.py
+-rw-r--r--   0 eric      (1000) users      (984)     1847 2024-03-27 17:18:16.000000 logger-36-2024.6/logger_36/config/system.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 16:11:17.848559 logger-36-2024.6/logger_36/constant/
+-rw-r--r--   0 eric      (1000) users      (984)     1614 2024-03-27 18:55:10.000000 logger-36-2024.6/logger_36/constant/generic.py
+-rwx------   0 eric      (1000) users      (984)     1681 2024-03-27 18:54:51.000000 logger-36-2024.6/logger_36/constant/handler.py
+-rw-r--r--   0 eric      (1000) users      (984)     1656 2024-03-28 09:36:45.000000 logger-36-2024.6/logger_36/constant/issue.py
+-rw-r--r--   0 eric      (1000) users      (984)     2150 2024-03-28 09:06:53.000000 logger-36-2024.6/logger_36/constant/logger.py
+-rw-r--r--   0 eric      (1000) users      (984)     1795 2024-03-28 09:36:54.000000 logger-36-2024.6/logger_36/constant/memory.py
+-rw-r--r--   0 eric      (1000) users      (984)     2084 2024-03-27 18:54:51.000000 logger-36-2024.6/logger_36/constant/message.py
+-rw-r--r--   0 eric      (1000) users      (984)     1681 2024-03-27 17:02:29.000000 logger-36-2024.6/logger_36/constant/record.py
+-rw-r--r--   0 eric      (1000) users      (984)     1800 2024-03-27 18:54:51.000000 logger-36-2024.6/logger_36/constant/system.py
+-rw-r--r--   0 eric      (1000) users      (984)     1616 2024-03-06 14:38:47.000000 logger-36-2024.6/logger_36/instance.py
+-rwx------   0 eric      (1000) users      (984)     6690 2024-04-03 15:42:32.000000 logger-36-2024.6/logger_36/main.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 16:11:17.848559 logger-36-2024.6/logger_36/task/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 16:11:17.848559 logger-36-2024.6/logger_36/task/format/
+-rw-r--r--   0 eric      (1000) users      (984)     3610 2024-03-28 09:36:54.000000 logger-36-2024.6/logger_36/task/format/memory.py
+-rw-r--r--   0 eric      (1000) users      (984)     3511 2024-03-27 18:54:51.000000 logger-36-2024.6/logger_36/task/format/message.py
+-rw-r--r--   0 eric      (1000) users      (984)     1968 2024-03-12 15:08:33.000000 logger-36-2024.6/logger_36/task/format/rule.py
+-rwx------   0 eric      (1000) users      (984)     4397 2024-03-07 16:54:56.000000 logger-36-2024.6/logger_36/task/inspection.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 16:11:17.848559 logger-36-2024.6/logger_36/task/measure/
+-rwx------   0 eric      (1000) users      (984)     2253 2024-03-27 17:27:28.000000 logger-36-2024.6/logger_36/task/measure/chronos.py
+-rwx------   0 eric      (1000) users      (984)     1874 2024-03-27 18:39:46.000000 logger-36-2024.6/logger_36/task/measure/memory.py
+-rw-r--r--   0 eric      (1000) users      (984)     5026 2024-03-29 09:49:15.000000 logger-36-2024.6/logger_36/task/storage.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 16:11:17.851893 logger-36-2024.6/logger_36/type/
+-rwx------   0 eric      (1000) users      (984)     5198 2024-03-27 18:54:51.000000 logger-36-2024.6/logger_36/type/extension.py
+-rw-r--r--   0 eric      (1000) users      (984)     2151 2024-03-29 09:46:52.000000 logger-36-2024.6/logger_36/type/issue.py
+-rw-r--r--   0 eric      (1000) users      (984)    12729 2024-04-03 06:51:24.000000 logger-36-2024.6/logger_36/type/logger.py
+-rwx------   0 eric      (1000) users      (984)     1575 2024-04-03 16:10:56.000000 logger-36-2024.6/logger_36/version.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 16:11:17.851893 logger-36-2024.6/logger_36.egg-info/
+-rw-r--r--   0 eric      (1000) users      (984)     4246 2024-04-03 16:11:17.000000 logger-36-2024.6/logger_36.egg-info/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)     1320 2024-04-03 16:11:17.000000 logger-36-2024.6/logger_36.egg-info/SOURCES.txt
+-rw-r--r--   0 eric      (1000) users      (984)        1 2024-04-03 16:11:17.000000 logger-36-2024.6/logger_36.egg-info/dependency_links.txt
+-rw-r--r--   0 eric      (1000) users      (984)       10 2024-04-03 16:11:17.000000 logger-36-2024.6/logger_36.egg-info/top_level.txt
+-rwx------   0 eric      (1000) users      (984)      104 2022-06-17 10:26:30.000000 logger-36-2024.6/pyproject.toml
+-rw-r--r--   0 eric      (1000) users      (984)       38 2024-04-03 16:11:17.851893 logger-36-2024.6/setup.cfg
+-rwx------   0 eric      (1000) users      (984)     5533 2024-04-03 07:02:21.000000 logger-36-2024.6/setup.py
```

### Comparing `logger-36-2024.5/PKG-INFO` & `logger-36-2024.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logger-36
-Version: 2024.5
+Version: 2024.6
 Summary: Simple logger with a catalog of handlers
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/logger-36/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/logger-36//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/logger-36/
```

### Comparing `logger-36-2024.5/README-COPYRIGHT-utf8.txt` & `logger-36-2024.6/README-COPYRIGHT-utf8.txt`

 * *Files identical despite different names*

### Comparing `logger-36-2024.5/README-LICENCE-utf8.txt` & `logger-36-2024.6/README-LICENCE-utf8.txt`

 * *Files identical despite different names*

### Comparing `logger-36-2024.5/README.rst` & `logger-36-2024.6/README.rst`

 * *Files identical despite different names*

### Comparing `logger-36-2024.5/documentation/wiki/description.asciidoc` & `logger-36-2024.6/documentation/wiki/description.asciidoc`

 * *Files identical despite different names*

### Comparing `logger-36-2024.5/logger_36/__init__.py` & `logger-36-2024.6/logger_36/__init__.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.5/logger_36/catalog/config/console_rich.py` & `logger-36-2024.6/logger_36/catalog/config/console_rich.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.5/logger_36/catalog/handler/console.py` & `logger-36-2024.6/logger_36/catalog/handler/console.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.5/logger_36/catalog/handler/console_rich.py` & `logger-36-2024.6/logger_36/type/extension.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,121 +27,108 @@
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import dataclasses as dtcl
 import logging as lggg
+import sys as sstm
 import typing as h
 
-from logger_36.catalog.config.console_rich import (
-    ACTUAL_COLOR,
-    DATE_TIME_COLOR,
-    ELAPSED_TIME_COLOR,
-    EXPECTED_COLOR,
-    GRAY_STYLE,
-    LEVEL_COLOR,
-)
-from logger_36.config.message import (
-    ACTUAL_PATTERNS,
-    ELAPSED_TIME_SEPARATOR,
-    EXPECTED_PATTERNS,
-    LEVEL_CLOSING,
-    WHERE_SEPARATOR,
-)
-from logger_36.constant.message import TIME_LENGTH
-from logger_36.constant.record import SHOW_W_RULE_ATTR
-from logger_36.task.format.rule import Rule
-from logger_36.type.extension import handler_extension_t
-from rich.console import Console as console_t
-from rich.console import RenderableType as renderable_t
-from rich.markup import escape as EscapedForRich
-from rich.text import Text as text_t
+from logger_36.config.message import TIME_FORMAT, WHERE_FORMAT
+from logger_36.constant.handler import HANDLER_CODES
+from logger_36.constant.memory import MEMORY_MEASURE_ERROR
+from logger_36.constant.message import NEXT_LINE_PROLOGUE
+from logger_36.constant.record import HIDE_WHERE_ATTR, SHOW_WHERE_ATTR
+from logger_36.task.format.message import FormattedMessage, MessageFormat
+from logger_36.task.measure.chronos import TimeStamp
+from logger_36.task.measure.memory import CanCheckMemory
 
 
 @dtcl.dataclass(slots=True, repr=False, eq=False)
-class console_rich_handler_t(lggg.Handler):
-    extension: handler_extension_t = dtcl.field(init=False)
-    console: console_t = dtcl.field(init=False)
-    FormattedLines: h.Callable[..., tuple[str, str | None]] = dtcl.field(init=False)
+class handler_extension_t:
+    name: str | None = None
+    show_where: bool = True
+    show_memory_usage: bool = False
+    FormattedRecord: h.Callable[[lggg.LogRecord], str] = dtcl.field(init=False)
 
-    name: dtcl.InitVar[str | None] = None
+    handler: dtcl.InitVar[lggg.Handler | None] = None
     level: dtcl.InitVar[int] = lggg.NOTSET
-    show_where: dtcl.InitVar[bool] = True
-    show_memory_usage: dtcl.InitVar[bool] = False
     formatter: dtcl.InitVar[lggg.Formatter | None] = None
 
-    rich_kwargs: dtcl.InitVar[dict[str, h.Any] | None] = None
-
     def __post_init__(
-        self,
-        name: str | None,
-        level: int,
-        show_where: bool,
-        show_memory_usage: bool,
-        formatter: lggg.Formatter | None,
-        rich_kwargs: dict[str, h.Any] | None,
+        self, handler: lggg.Handler | None, level: int, formatter: lggg.Formatter | None
     ) -> None:
         """"""
-        lggg.Handler.__init__(self)
-
-        self.extension = handler_extension_t(
-            name=name,
-            show_where=show_where,
-            show_memory_usage=show_memory_usage,
-            handler=self,
-            level=level,
-            formatter=formatter,
-        )
-
-        if rich_kwargs is None:
-            rich_kwargs = {}
-        self.console = console_t(
-            highlight=False,
-            force_terminal=True,
-            record=True,
-            **rich_kwargs,
-        )
+        if self.name in HANDLER_CODES:
+            raise ValueError(
+                FormattedMessage(
+                    "Invalid handler name",
+                    actual=self.name,
+                    expected=f"a name not in {str(HANDLER_CODES)[1:-1]}",
+                )
+            )
+
+        if self.name is None:
+            self.name = TimeStamp()
+
+        if self.show_memory_usage and not CanCheckMemory():
+            self.show_memory_usage = False
+            print(MEMORY_MEASURE_ERROR, file=sstm.stderr)
+
+        handler.setLevel(level)
+
+        if formatter is None:
+            message_format = MessageFormat(self.show_where, self.show_memory_usage)
+            formatter = lggg.Formatter(fmt=message_format, datefmt=TIME_FORMAT)
+        handler.setFormatter(formatter)
+        self.FormattedRecord = handler.formatter.format
 
-        self.FormattedLines = self.extension.FormattedLines
-
-    def emit(self, record: lggg.LogRecord, /) -> None:
-        """"""
-        cls = self.__class__
-        if hasattr(record, SHOW_W_RULE_ATTR):
-            richer = Rule(record.msg, DATE_TIME_COLOR)
+    def FormattedLines(
+        self,
+        record: lggg.LogRecord,
+        /,
+        *,
+        PreProcessed: h.Callable[[str], str] | None = None,
+        should_join_lines: bool = False,
+    ) -> tuple[str, str | None]:
+        """
+        See logger_36.catalog.handler.README.txt.
+        """
+        record.level_first_letter = record.levelname[0]
+
+        message = record.msg
+        if not isinstance(message, str):
+            message = str(message)
+        original_message = message
+
+        if PreProcessed is not None:
+            message = PreProcessed(message)
+        if "\n" in message:
+            lines = message.splitlines()
+            next_lines = NEXT_LINE_PROLOGUE.join(lines[1:])
+            next_lines = f"{NEXT_LINE_PROLOGUE}{next_lines}"
+            message = lines[0]
         else:
-            first, next_s = self.FormattedLines(record, PreProcessed=EscapedForRich)
-            richer = cls.HighlightedVersion(first, next_s, record.levelno)
-        self.console.print(richer, crop=False, overflow="ignore")
-
-    @classmethod
-    def HighlightedVersion(
-        cls, first_line: str, next_lines: str | None, log_level: int, /
-    ) -> renderable_t:
-        """"""
-        output = text_t(first_line)
-
-        # Used instead of _CONTEXT_LENGTH which might include \t, thus creating a
-        # mismatch between character length and length when displayed in console.
-        context_end = first_line.find(LEVEL_CLOSING)
-        elapsed_time_separator = first_line.rfind(ELAPSED_TIME_SEPARATOR)
-        where_separator = first_line.rfind(
-            WHERE_SEPARATOR, context_end, elapsed_time_separator
-        )
-
-        output.stylize(DATE_TIME_COLOR, end=TIME_LENGTH)
-        output.stylize(
-            LEVEL_COLOR[log_level],
-            start=TIME_LENGTH,
-            end=context_end + 1,
-        )
-        output.stylize(GRAY_STYLE, start=where_separator, end=elapsed_time_separator)
-        output.stylize(ELAPSED_TIME_COLOR, start=elapsed_time_separator)
-
-        if next_lines is not None:
-            output.append(next_lines)
+            next_lines = None
 
-        _ = output.highlight_regex(ACTUAL_PATTERNS, style=ACTUAL_COLOR)
-        _ = output.highlight_regex(EXPECTED_PATTERNS, style=EXPECTED_COLOR)
-
-        return output
+        record.msg = message
+        if self.show_where and not hasattr(record, SHOW_WHERE_ATTR):
+            hide_where = getattr(record, HIDE_WHERE_ATTR, False)
+            if hide_where:
+                record.where = ""
+            else:
+                record.where = WHERE_FORMAT.format(
+                    module=record.module, funcName=record.funcName, lineno=record.lineno
+                )
+        first_line = self.FormattedRecord(record).replace("\t", " ")
+
+        # Revert the record message to its original value for subsequent handlers.
+        record.msg = original_message
+
+        if should_join_lines:
+            if next_lines is None:
+                return first_line, None
+            else:
+                return f"{first_line}{next_lines}", None
+        else:
+            return first_line, next_lines
```

### Comparing `logger-36-2024.5/logger_36/catalog/handler/file.py` & `logger-36-2024.6/logger_36/catalog/handler/file.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.5/logger_36/catalog/handler/generic.py` & `logger-36-2024.6/logger_36/catalog/handler/generic.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.5/logger_36/catalog/logging/chronos.py` & `logger-36-2024.6/logger_36/catalog/logging/chronos.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.5/logger_36/catalog/logging/gpu.py` & `logger-36-2024.6/logger_36/catalog/logging/gpu.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.5/logger_36/catalog/logging/memory.py` & `logger-36-2024.6/logger_36/catalog/logging/memory.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.5/logger_36/catalog/logging/system.py` & `logger-36-2024.6/logger_36/catalog/logging/system.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.5/logger_36/config/issue.py` & `logger-36-2024.6/logger_36/config/issue.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.5/logger_36/config/memory.py` & `logger-36-2024.6/logger_36/config/memory.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.5/logger_36/config/message.py` & `logger-36-2024.6/logger_36/config/message.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.5/logger_36/config/system.py` & `logger-36-2024.6/logger_36/config/system.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.5/logger_36/constant/generic.py` & `logger-36-2024.6/logger_36/constant/generic.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.5/logger_36/constant/handler.py` & `logger-36-2024.6/logger_36/constant/handler.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.5/logger_36/constant/issue.py` & `logger-36-2024.6/logger_36/constant/issue.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.5/logger_36/constant/logger.py` & `logger-36-2024.6/logger_36/constant/logger.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.5/logger_36/constant/memory.py` & `logger-36-2024.6/logger_36/constant/memory.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.5/logger_36/constant/message.py` & `logger-36-2024.6/logger_36/constant/message.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.5/logger_36/constant/record.py` & `logger-36-2024.6/logger_36/constant/record.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.5/logger_36/constant/system.py` & `logger-36-2024.6/logger_36/constant/system.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.5/logger_36/instance.py` & `logger-36-2024.6/logger_36/instance.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.5/logger_36/main.py` & `logger-36-2024.6/logger_36/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -117,14 +117,15 @@
     logger: lggg.Logger | None = None,
     name: str | None = None,
     level: int = lggg.INFO,
     show_where: bool = True,
     show_memory_usage: bool = False,
     formatter: lggg.Formatter | None = None,
     should_hold_messages: bool = False,
+    should_install_traceback: bool = False,
     **kwargs,
 ) -> None:
     """"""
     global _RICH_ERROR
     if _RICH_ERROR is not None:
         print(_RICH_ERROR, file=sstm.stderr)
         _RICH_ERROR = None
@@ -134,14 +135,15 @@
 
     handler = console_rich_handler_t(
         name=name,
         level=level,
         show_where=show_where,
         show_memory_usage=show_memory_usage,
         formatter=formatter,
+        should_install_traceback=should_install_traceback,
         rich_kwargs=kwargs,
     )
     logger.AddHandler(handler, should_hold_messages)
 
 
 def AddFileHandler(
     path: str | path_t,
```

### Comparing `logger-36-2024.5/logger_36/task/format/memory.py` & `logger-36-2024.6/logger_36/task/format/memory.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.5/logger_36/task/format/message.py` & `logger-36-2024.6/logger_36/task/format/message.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.5/logger_36/task/format/rule.py` & `logger-36-2024.6/logger_36/task/format/rule.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.5/logger_36/task/inspection.py` & `logger-36-2024.6/logger_36/task/inspection.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.5/logger_36/task/measure/chronos.py` & `logger-36-2024.6/logger_36/task/measure/chronos.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.5/logger_36/task/measure/memory.py` & `logger-36-2024.6/logger_36/task/measure/memory.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.5/logger_36/task/storage.py` & `logger-36-2024.6/logger_36/task/storage.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.5/logger_36/type/extension.py` & `logger-36-2024.6/logger_36/catalog/handler/console_rich.py`

 * *Files 26% similar despite different names*

```diff
@@ -27,108 +27,152 @@
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import dataclasses as dtcl
 import logging as lggg
-import sys as sstm
 import typing as h
 
-from logger_36.config.message import TIME_FORMAT, WHERE_FORMAT
-from logger_36.constant.handler import HANDLER_CODES
-from logger_36.constant.memory import MEMORY_MEASURE_ERROR
-from logger_36.constant.message import NEXT_LINE_PROLOGUE
-from logger_36.constant.record import HIDE_WHERE_ATTR, SHOW_WHERE_ATTR
-from logger_36.task.format.message import FormattedMessage, MessageFormat
-from logger_36.task.measure.chronos import TimeStamp
-from logger_36.task.measure.memory import CanCheckMemory
+from logger_36.catalog.config.console_rich import (
+    ACTUAL_COLOR,
+    DATE_TIME_COLOR,
+    ELAPSED_TIME_COLOR,
+    EXPECTED_COLOR,
+    GRAY_STYLE,
+    LEVEL_COLOR,
+)
+from logger_36.config.message import (
+    ACTUAL_PATTERNS,
+    ELAPSED_TIME_SEPARATOR,
+    EXPECTED_PATTERNS,
+    LEVEL_CLOSING,
+    WHERE_SEPARATOR,
+)
+from logger_36.constant.message import TIME_LENGTH
+from logger_36.constant.record import SHOW_W_RULE_ATTR
+from logger_36.task.format.rule import Rule
+from logger_36.type.extension import handler_extension_t
+from rich.console import Console as console_t
+from rich.console import RenderableType as renderable_t
+from rich.markup import escape as EscapedForRich
+from rich.text import Text as text_t
+from rich.traceback import install as InstallTracebackHandler
+
+
+_COMMON_TRACEBACK_ARGUMENTS = ("theme", "width")
+_EXCLUSIVE_TRACEBACK_ARGUMENTS = (
+    "extra_lines",
+    "indent_guides",
+    "locals_hide_dunder",
+    "locals_hide_sunder",
+    "locals_max_length",
+    "locals_max_string",
+    "max_frames" "show_locals",
+    "suppress",
+    "word_wrap",
+)
 
 
 @dtcl.dataclass(slots=True, repr=False, eq=False)
-class handler_extension_t:
-    name: str | None = None
-    show_where: bool = True
-    show_memory_usage: bool = False
-    FormattedRecord: h.Callable[[lggg.LogRecord], str] = dtcl.field(init=False)
+class console_rich_handler_t(lggg.Handler):
+    extension: handler_extension_t = dtcl.field(init=False)
+    console: console_t = dtcl.field(init=False)
+    FormattedLines: h.Callable[..., tuple[str, str | None]] = dtcl.field(init=False)
 
-    handler: dtcl.InitVar[lggg.Handler | None] = None
+    name: dtcl.InitVar[str | None] = None
     level: dtcl.InitVar[int] = lggg.NOTSET
+    show_where: dtcl.InitVar[bool] = True
+    show_memory_usage: dtcl.InitVar[bool] = False
     formatter: dtcl.InitVar[lggg.Formatter | None] = None
+    should_install_traceback: dtcl.InitVar[bool] = False
+
+    rich_kwargs: dtcl.InitVar[dict[str, h.Any] | None] = None
 
     def __post_init__(
-        self, handler: lggg.Handler | None, level: int, formatter: lggg.Formatter | None
+        self,
+        name: str | None,
+        level: int,
+        show_where: bool,
+        show_memory_usage: bool,
+        formatter: lggg.Formatter | None,
+        should_install_traceback: bool,
+        rich_kwargs: dict[str, h.Any] | None,
     ) -> None:
         """"""
-        if self.name in HANDLER_CODES:
-            raise ValueError(
-                FormattedMessage(
-                    "Invalid handler name",
-                    actual=self.name,
-                    expected=f"a name not in {str(HANDLER_CODES)[1:-1]}",
-                )
-            )
-
-        if self.name is None:
-            self.name = TimeStamp()
-
-        if self.show_memory_usage and not CanCheckMemory():
-            self.show_memory_usage = False
-            print(MEMORY_MEASURE_ERROR, file=sstm.stderr)
-
-        handler.setLevel(level)
-
-        if formatter is None:
-            message_format = MessageFormat(self.show_where, self.show_memory_usage)
-            formatter = lggg.Formatter(fmt=message_format, datefmt=TIME_FORMAT)
-        handler.setFormatter(formatter)
-        self.FormattedRecord = handler.formatter.format
+        lggg.Handler.__init__(self)
 
-    def FormattedLines(
-        self,
-        record: lggg.LogRecord,
-        /,
-        *,
-        PreProcessed: h.Callable[[str], str] | None = None,
-        should_join_lines: bool = False,
-    ) -> tuple[str, str | None]:
-        """
-        See logger_36.catalog.handler.README.txt.
-        """
-        record.level_first_letter = record.levelname[0]
-
-        message = record.msg
-        if not isinstance(message, str):
-            message = str(message)
-        original_message = message
-
-        if PreProcessed is not None:
-            message = PreProcessed(message)
-        if "\n" in message:
-            lines = message.splitlines()
-            next_lines = NEXT_LINE_PROLOGUE.join(lines[1:])
-            next_lines = f"{NEXT_LINE_PROLOGUE}{next_lines}"
-            message = lines[0]
+        self.extension = handler_extension_t(
+            name=name,
+            show_where=show_where,
+            show_memory_usage=show_memory_usage,
+            handler=self,
+            level=level,
+            formatter=formatter,
+        )
+
+        if rich_kwargs is None:
+            rich_console_kwargs = {}
         else:
-            next_lines = None
+            rich_console_kwargs = rich_kwargs
+        rich_traceback_kwargs = {}
+        if should_install_traceback:
+            for key in rich_console_kwargs:
+                if key in _COMMON_TRACEBACK_ARGUMENTS:
+                    rich_traceback_kwargs[key] = rich_console_kwargs[key]
+                elif key in _EXCLUSIVE_TRACEBACK_ARGUMENTS:
+                    rich_traceback_kwargs[key] = rich_console_kwargs[key]
+                    del rich_console_kwargs[key]
+
+        self.console = console_t(
+            highlight=False,
+            force_terminal=True,
+            record=True,
+            **rich_console_kwargs,
+        )
+        if should_install_traceback:
+            rich_traceback_kwargs["console"] = self.console
+            InstallTracebackHandler(**rich_traceback_kwargs)
+
+        self.FormattedLines = self.extension.FormattedLines
 
-        record.msg = message
-        if self.show_where and not hasattr(record, SHOW_WHERE_ATTR):
-            hide_where = getattr(record, HIDE_WHERE_ATTR, False)
-            if hide_where:
-                record.where = ""
-            else:
-                record.where = WHERE_FORMAT.format(
-                    module=record.module, funcName=record.funcName, lineno=record.lineno
-                )
-        first_line = self.FormattedRecord(record).replace("\t", " ")
-
-        # Revert the record message to its original value for subsequent handlers.
-        record.msg = original_message
-
-        if should_join_lines:
-            if next_lines is None:
-                return first_line, None
-            else:
-                return f"{first_line}{next_lines}", None
+    def emit(self, record: lggg.LogRecord, /) -> None:
+        """"""
+        cls = self.__class__
+        if hasattr(record, SHOW_W_RULE_ATTR):
+            richer = Rule(record.msg, DATE_TIME_COLOR)
         else:
-            return first_line, next_lines
+            first, next_s = self.FormattedLines(record, PreProcessed=EscapedForRich)
+            richer = cls.HighlightedVersion(first, next_s, record.levelno)
+        self.console.print(richer, crop=False, overflow="ignore")
+
+    @classmethod
+    def HighlightedVersion(
+        cls, first_line: str, next_lines: str | None, log_level: int, /
+    ) -> renderable_t:
+        """"""
+        output = text_t(first_line)
+
+        # Used instead of _CONTEXT_LENGTH which might include \t, thus creating a
+        # mismatch between character length and length when displayed in console.
+        context_end = first_line.find(LEVEL_CLOSING)
+        elapsed_time_separator = first_line.rfind(ELAPSED_TIME_SEPARATOR)
+        where_separator = first_line.rfind(
+            WHERE_SEPARATOR, context_end, elapsed_time_separator
+        )
+
+        output.stylize(DATE_TIME_COLOR, end=TIME_LENGTH)
+        output.stylize(
+            LEVEL_COLOR[log_level],
+            start=TIME_LENGTH,
+            end=context_end + 1,
+        )
+        output.stylize(GRAY_STYLE, start=where_separator, end=elapsed_time_separator)
+        output.stylize(ELAPSED_TIME_COLOR, start=elapsed_time_separator)
+
+        if next_lines is not None:
+            output.append(next_lines)
+
+        _ = output.highlight_regex(ACTUAL_PATTERNS, style=ACTUAL_COLOR)
+        _ = output.highlight_regex(EXPECTED_PATTERNS, style=EXPECTED_COLOR)
+
+        return output
```

### Comparing `logger-36-2024.5/logger_36/type/issue.py` & `logger-36-2024.6/logger_36/type/issue.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.5/logger_36/type/logger.py` & `logger-36-2024.6/logger_36/type/logger.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.5/logger_36/version.py` & `logger-36-2024.6/logger_36/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-__version__ = "2024.5"
+__version__ = "2024.6"
```

### Comparing `logger-36-2024.5/logger_36.egg-info/PKG-INFO` & `logger-36-2024.6/logger_36.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logger-36
-Version: 2024.5
+Version: 2024.6
 Summary: Simple logger with a catalog of handlers
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/logger-36/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/logger-36//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/logger-36/
```

### Comparing `logger-36-2024.5/logger_36.egg-info/SOURCES.txt` & `logger-36-2024.6/logger_36.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `logger-36-2024.5/setup.py` & `logger-36-2024.6/setup.py`

 * *Files identical despite different names*

