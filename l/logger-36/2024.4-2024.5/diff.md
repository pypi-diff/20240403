# Comparing `tmp/logger-36-2024.4.tar.gz` & `tmp/logger-36-2024.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logger-36-2024.4.tar", last modified: Fri Mar 29 16:24:14 2024, max compression
+gzip compressed data, was "logger-36-2024.5.tar", last modified: Wed Apr  3 07:02:42 2024, max compression
```

## Comparing `logger-36-2024.4.tar` & `logger-36-2024.5.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-03-29 16:24:14.584372 logger-36-2024.4/
--rwx------   0 eric      (1000) users      (984)      114 2022-10-14 06:42:17.000000 logger-36-2024.4/MANIFEST.in
--rw-r--r--   0 eric      (1000) users      (984)     4236 2024-03-29 16:24:14.584372 logger-36-2024.4/PKG-INFO
--rwx------   0 eric      (1000) users      (984)      636 2023-02-17 08:45:51.000000 logger-36-2024.4/README-COPYRIGHT-utf8.txt
--rwx------   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 logger-36-2024.4/README-LICENCE-utf8.txt
--rwx------   0 eric      (1000) users      (984)     3458 2023-02-17 09:17:51.000000 logger-36-2024.4/README.rst
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-03-29 16:24:14.577706 logger-36-2024.4/documentation/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-03-29 16:24:14.577706 logger-36-2024.4/documentation/wiki/
--rwx------   0 eric      (1000) users      (984)     1867 2024-03-29 10:17:44.000000 logger-36-2024.4/documentation/wiki/description.asciidoc
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-03-29 16:24:14.577706 logger-36-2024.4/logger_36/
--rwx------   0 eric      (1000) users      (984)     1756 2024-03-15 21:24:09.000000 logger-36-2024.4/logger_36/__init__.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-03-29 16:24:14.577706 logger-36-2024.4/logger_36/catalog/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-03-29 16:24:14.577706 logger-36-2024.4/logger_36/catalog/config/
--rw-r--r--   0 eric      (1000) users      (984)     2030 2024-03-28 08:18:21.000000 logger-36-2024.4/logger_36/catalog/config/console_rich.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-03-29 16:24:14.581039 logger-36-2024.4/logger_36/catalog/handler/
--rw-r--r--   0 eric      (1000) users      (984)     3092 2024-03-27 17:11:48.000000 logger-36-2024.4/logger_36/catalog/handler/console.py
--rwx------   0 eric      (1000) users      (984)     5395 2024-03-28 09:36:54.000000 logger-36-2024.4/logger_36/catalog/handler/console_rich.py
--rwx------   0 eric      (1000) users      (984)     3507 2024-03-27 17:11:54.000000 logger-36-2024.4/logger_36/catalog/handler/file.py
--rwx------   0 eric      (1000) users      (984)     5931 2024-03-27 17:12:07.000000 logger-36-2024.4/logger_36/catalog/handler/generic.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-03-29 16:24:14.581039 logger-36-2024.4/logger_36/catalog/logging/
--rw-r--r--   0 eric      (1000) users      (984)     1814 2024-03-27 17:05:43.000000 logger-36-2024.4/logger_36/catalog/logging/chronos.py
--rw-r--r--   0 eric      (1000) users      (984)     2465 2024-03-27 17:05:43.000000 logger-36-2024.4/logger_36/catalog/logging/gpu.py
--rw-r--r--   0 eric      (1000) users      (984)     4038 2024-03-28 09:46:44.000000 logger-36-2024.4/logger_36/catalog/logging/memory.py
--rw-r--r--   0 eric      (1000) users      (984)     2447 2024-03-27 17:20:41.000000 logger-36-2024.4/logger_36/catalog/logging/system.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-03-29 16:24:14.581039 logger-36-2024.4/logger_36/config/
--rw-r--r--   0 eric      (1000) users      (984)     1637 2024-03-29 09:47:00.000000 logger-36-2024.4/logger_36/config/issue.py
--rw-r--r--   0 eric      (1000) users      (984)     1587 2024-03-28 09:30:00.000000 logger-36-2024.4/logger_36/config/memory.py
--rwx------   0 eric      (1000) users      (984)     2056 2024-03-28 08:16:13.000000 logger-36-2024.4/logger_36/config/message.py
--rw-r--r--   0 eric      (1000) users      (984)     1847 2024-03-27 17:18:16.000000 logger-36-2024.4/logger_36/config/system.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-03-29 16:24:14.581039 logger-36-2024.4/logger_36/constant/
--rw-r--r--   0 eric      (1000) users      (984)     1614 2024-03-27 18:55:10.000000 logger-36-2024.4/logger_36/constant/generic.py
--rwx------   0 eric      (1000) users      (984)     1681 2024-03-27 18:54:51.000000 logger-36-2024.4/logger_36/constant/handler.py
--rw-r--r--   0 eric      (1000) users      (984)     1656 2024-03-28 09:36:45.000000 logger-36-2024.4/logger_36/constant/issue.py
--rw-r--r--   0 eric      (1000) users      (984)     2150 2024-03-28 09:06:53.000000 logger-36-2024.4/logger_36/constant/logger.py
--rw-r--r--   0 eric      (1000) users      (984)     1795 2024-03-28 09:36:54.000000 logger-36-2024.4/logger_36/constant/memory.py
--rw-r--r--   0 eric      (1000) users      (984)     2084 2024-03-27 18:54:51.000000 logger-36-2024.4/logger_36/constant/message.py
--rw-r--r--   0 eric      (1000) users      (984)     1681 2024-03-27 17:02:29.000000 logger-36-2024.4/logger_36/constant/record.py
--rw-r--r--   0 eric      (1000) users      (984)     1800 2024-03-27 18:54:51.000000 logger-36-2024.4/logger_36/constant/system.py
--rw-r--r--   0 eric      (1000) users      (984)     1616 2024-03-06 14:38:47.000000 logger-36-2024.4/logger_36/instance.py
--rwx------   0 eric      (1000) users      (984)     6134 2024-03-27 18:56:33.000000 logger-36-2024.4/logger_36/main.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-03-29 16:24:14.581039 logger-36-2024.4/logger_36/task/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-03-29 16:24:14.581039 logger-36-2024.4/logger_36/task/format/
--rw-r--r--   0 eric      (1000) users      (984)     3610 2024-03-28 09:36:54.000000 logger-36-2024.4/logger_36/task/format/memory.py
--rw-r--r--   0 eric      (1000) users      (984)     3511 2024-03-27 18:54:51.000000 logger-36-2024.4/logger_36/task/format/message.py
--rw-r--r--   0 eric      (1000) users      (984)     1968 2024-03-12 15:08:33.000000 logger-36-2024.4/logger_36/task/format/rule.py
--rwx------   0 eric      (1000) users      (984)     4397 2024-03-07 16:54:56.000000 logger-36-2024.4/logger_36/task/inspection.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-03-29 16:24:14.581039 logger-36-2024.4/logger_36/task/measure/
--rwx------   0 eric      (1000) users      (984)     2253 2024-03-27 17:27:28.000000 logger-36-2024.4/logger_36/task/measure/chronos.py
--rwx------   0 eric      (1000) users      (984)     1874 2024-03-27 18:39:46.000000 logger-36-2024.4/logger_36/task/measure/memory.py
--rw-r--r--   0 eric      (1000) users      (984)     5026 2024-03-29 09:49:15.000000 logger-36-2024.4/logger_36/task/storage.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-03-29 16:24:14.581039 logger-36-2024.4/logger_36/type/
--rwx------   0 eric      (1000) users      (984)     5198 2024-03-27 18:54:51.000000 logger-36-2024.4/logger_36/type/extension.py
--rw-r--r--   0 eric      (1000) users      (984)     2151 2024-03-29 09:46:52.000000 logger-36-2024.4/logger_36/type/issue.py
--rw-r--r--   0 eric      (1000) users      (984)    12731 2024-03-29 16:18:11.000000 logger-36-2024.4/logger_36/type/logger.py
--rwx------   0 eric      (1000) users      (984)     1575 2024-03-29 16:22:16.000000 logger-36-2024.4/logger_36/version.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-03-29 16:24:14.581039 logger-36-2024.4/logger_36.egg-info/
--rw-r--r--   0 eric      (1000) users      (984)     4236 2024-03-29 16:24:14.000000 logger-36-2024.4/logger_36.egg-info/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)     1320 2024-03-29 16:24:14.000000 logger-36-2024.4/logger_36.egg-info/SOURCES.txt
--rw-r--r--   0 eric      (1000) users      (984)        1 2024-03-29 16:24:14.000000 logger-36-2024.4/logger_36.egg-info/dependency_links.txt
--rw-r--r--   0 eric      (1000) users      (984)       10 2024-03-29 16:24:14.000000 logger-36-2024.4/logger_36.egg-info/top_level.txt
--rwx------   0 eric      (1000) users      (984)      104 2022-06-17 10:26:30.000000 logger-36-2024.4/pyproject.toml
--rw-r--r--   0 eric      (1000) users      (984)       38 2024-03-29 16:24:14.584372 logger-36-2024.4/setup.cfg
--rwx------   0 eric      (1000) users      (984)     5495 2024-03-28 09:58:49.000000 logger-36-2024.4/setup.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 07:02:42.705098 logger-36-2024.5/
+-rwx------   0 eric      (1000) users      (984)      114 2022-10-14 06:42:17.000000 logger-36-2024.5/MANIFEST.in
+-rw-r--r--   0 eric      (1000) users      (984)     4246 2024-04-03 07:02:42.705098 logger-36-2024.5/PKG-INFO
+-rwx------   0 eric      (1000) users      (984)      636 2023-02-17 08:45:51.000000 logger-36-2024.5/README-COPYRIGHT-utf8.txt
+-rwx------   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 logger-36-2024.5/README-LICENCE-utf8.txt
+-rwx------   0 eric      (1000) users      (984)     3458 2023-02-17 09:17:51.000000 logger-36-2024.5/README.rst
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 07:02:42.698431 logger-36-2024.5/documentation/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 07:02:42.698431 logger-36-2024.5/documentation/wiki/
+-rwx------   0 eric      (1000) users      (984)     1867 2024-03-29 10:17:44.000000 logger-36-2024.5/documentation/wiki/description.asciidoc
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 07:02:42.701764 logger-36-2024.5/logger_36/
+-rwx------   0 eric      (1000) users      (984)     1756 2024-03-15 21:24:09.000000 logger-36-2024.5/logger_36/__init__.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 07:02:42.698431 logger-36-2024.5/logger_36/catalog/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 07:02:42.701764 logger-36-2024.5/logger_36/catalog/config/
+-rw-r--r--   0 eric      (1000) users      (984)     2030 2024-03-28 08:18:21.000000 logger-36-2024.5/logger_36/catalog/config/console_rich.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 07:02:42.701764 logger-36-2024.5/logger_36/catalog/handler/
+-rw-r--r--   0 eric      (1000) users      (984)     3092 2024-03-27 17:11:48.000000 logger-36-2024.5/logger_36/catalog/handler/console.py
+-rwx------   0 eric      (1000) users      (984)     5395 2024-03-28 09:36:54.000000 logger-36-2024.5/logger_36/catalog/handler/console_rich.py
+-rwx------   0 eric      (1000) users      (984)     3507 2024-03-27 17:11:54.000000 logger-36-2024.5/logger_36/catalog/handler/file.py
+-rwx------   0 eric      (1000) users      (984)     5931 2024-03-27 17:12:07.000000 logger-36-2024.5/logger_36/catalog/handler/generic.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 07:02:42.701764 logger-36-2024.5/logger_36/catalog/logging/
+-rw-r--r--   0 eric      (1000) users      (984)     1814 2024-03-27 17:05:43.000000 logger-36-2024.5/logger_36/catalog/logging/chronos.py
+-rw-r--r--   0 eric      (1000) users      (984)     2465 2024-03-27 17:05:43.000000 logger-36-2024.5/logger_36/catalog/logging/gpu.py
+-rw-r--r--   0 eric      (1000) users      (984)     4038 2024-03-28 09:46:44.000000 logger-36-2024.5/logger_36/catalog/logging/memory.py
+-rw-r--r--   0 eric      (1000) users      (984)     2447 2024-03-27 17:20:41.000000 logger-36-2024.5/logger_36/catalog/logging/system.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 07:02:42.701764 logger-36-2024.5/logger_36/config/
+-rw-r--r--   0 eric      (1000) users      (984)     1637 2024-03-29 09:47:00.000000 logger-36-2024.5/logger_36/config/issue.py
+-rw-r--r--   0 eric      (1000) users      (984)     1587 2024-03-28 09:30:00.000000 logger-36-2024.5/logger_36/config/memory.py
+-rwx------   0 eric      (1000) users      (984)     2056 2024-03-28 08:16:13.000000 logger-36-2024.5/logger_36/config/message.py
+-rw-r--r--   0 eric      (1000) users      (984)     1847 2024-03-27 17:18:16.000000 logger-36-2024.5/logger_36/config/system.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 07:02:42.701764 logger-36-2024.5/logger_36/constant/
+-rw-r--r--   0 eric      (1000) users      (984)     1614 2024-03-27 18:55:10.000000 logger-36-2024.5/logger_36/constant/generic.py
+-rwx------   0 eric      (1000) users      (984)     1681 2024-03-27 18:54:51.000000 logger-36-2024.5/logger_36/constant/handler.py
+-rw-r--r--   0 eric      (1000) users      (984)     1656 2024-03-28 09:36:45.000000 logger-36-2024.5/logger_36/constant/issue.py
+-rw-r--r--   0 eric      (1000) users      (984)     2150 2024-03-28 09:06:53.000000 logger-36-2024.5/logger_36/constant/logger.py
+-rw-r--r--   0 eric      (1000) users      (984)     1795 2024-03-28 09:36:54.000000 logger-36-2024.5/logger_36/constant/memory.py
+-rw-r--r--   0 eric      (1000) users      (984)     2084 2024-03-27 18:54:51.000000 logger-36-2024.5/logger_36/constant/message.py
+-rw-r--r--   0 eric      (1000) users      (984)     1681 2024-03-27 17:02:29.000000 logger-36-2024.5/logger_36/constant/record.py
+-rw-r--r--   0 eric      (1000) users      (984)     1800 2024-03-27 18:54:51.000000 logger-36-2024.5/logger_36/constant/system.py
+-rw-r--r--   0 eric      (1000) users      (984)     1616 2024-03-06 14:38:47.000000 logger-36-2024.5/logger_36/instance.py
+-rwx------   0 eric      (1000) users      (984)     6587 2024-04-03 06:48:53.000000 logger-36-2024.5/logger_36/main.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 07:02:42.705098 logger-36-2024.5/logger_36/task/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 07:02:42.705098 logger-36-2024.5/logger_36/task/format/
+-rw-r--r--   0 eric      (1000) users      (984)     3610 2024-03-28 09:36:54.000000 logger-36-2024.5/logger_36/task/format/memory.py
+-rw-r--r--   0 eric      (1000) users      (984)     3511 2024-03-27 18:54:51.000000 logger-36-2024.5/logger_36/task/format/message.py
+-rw-r--r--   0 eric      (1000) users      (984)     1968 2024-03-12 15:08:33.000000 logger-36-2024.5/logger_36/task/format/rule.py
+-rwx------   0 eric      (1000) users      (984)     4397 2024-03-07 16:54:56.000000 logger-36-2024.5/logger_36/task/inspection.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 07:02:42.705098 logger-36-2024.5/logger_36/task/measure/
+-rwx------   0 eric      (1000) users      (984)     2253 2024-03-27 17:27:28.000000 logger-36-2024.5/logger_36/task/measure/chronos.py
+-rwx------   0 eric      (1000) users      (984)     1874 2024-03-27 18:39:46.000000 logger-36-2024.5/logger_36/task/measure/memory.py
+-rw-r--r--   0 eric      (1000) users      (984)     5026 2024-03-29 09:49:15.000000 logger-36-2024.5/logger_36/task/storage.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 07:02:42.705098 logger-36-2024.5/logger_36/type/
+-rwx------   0 eric      (1000) users      (984)     5198 2024-03-27 18:54:51.000000 logger-36-2024.5/logger_36/type/extension.py
+-rw-r--r--   0 eric      (1000) users      (984)     2151 2024-03-29 09:46:52.000000 logger-36-2024.5/logger_36/type/issue.py
+-rw-r--r--   0 eric      (1000) users      (984)    12729 2024-04-03 06:51:24.000000 logger-36-2024.5/logger_36/type/logger.py
+-rwx------   0 eric      (1000) users      (984)     1575 2024-04-03 06:53:26.000000 logger-36-2024.5/logger_36/version.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 07:02:42.705098 logger-36-2024.5/logger_36.egg-info/
+-rw-r--r--   0 eric      (1000) users      (984)     4246 2024-04-03 07:02:42.000000 logger-36-2024.5/logger_36.egg-info/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)     1320 2024-04-03 07:02:42.000000 logger-36-2024.5/logger_36.egg-info/SOURCES.txt
+-rw-r--r--   0 eric      (1000) users      (984)        1 2024-04-03 07:02:42.000000 logger-36-2024.5/logger_36.egg-info/dependency_links.txt
+-rw-r--r--   0 eric      (1000) users      (984)       10 2024-04-03 07:02:42.000000 logger-36-2024.5/logger_36.egg-info/top_level.txt
+-rwx------   0 eric      (1000) users      (984)      104 2022-06-17 10:26:30.000000 logger-36-2024.5/pyproject.toml
+-rw-r--r--   0 eric      (1000) users      (984)       38 2024-04-03 07:02:42.705098 logger-36-2024.5/setup.cfg
+-rwx------   0 eric      (1000) users      (984)     5533 2024-04-03 07:02:21.000000 logger-36-2024.5/setup.py
```

### Comparing `logger-36-2024.4/PKG-INFO` & `logger-36-2024.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: logger-36
-Version: 2024.4
+Version: 2024.5
 Summary: Simple logger with a catalog of handlers
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/logger-36/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/logger-36//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/logger-36/
 Keywords: log,warning,error
 Classifier: Topic :: Software Development
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 
 ..
    Copyright CNRS/Inria/UCA
    Contributor(s): Eric Debreuve (since 2023)
```

### Comparing `logger-36-2024.4/README-COPYRIGHT-utf8.txt` & `logger-36-2024.5/README-COPYRIGHT-utf8.txt`

 * *Files identical despite different names*

### Comparing `logger-36-2024.4/README-LICENCE-utf8.txt` & `logger-36-2024.5/README-LICENCE-utf8.txt`

 * *Files identical despite different names*

### Comparing `logger-36-2024.4/README.rst` & `logger-36-2024.5/README.rst`

 * *Files identical despite different names*

### Comparing `logger-36-2024.4/documentation/wiki/description.asciidoc` & `logger-36-2024.5/documentation/wiki/description.asciidoc`

 * *Files identical despite different names*

### Comparing `logger-36-2024.4/logger_36/__init__.py` & `logger-36-2024.5/logger_36/__init__.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.4/logger_36/catalog/config/console_rich.py` & `logger-36-2024.5/logger_36/catalog/config/console_rich.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.4/logger_36/catalog/handler/console.py` & `logger-36-2024.5/logger_36/catalog/handler/console.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.4/logger_36/catalog/handler/console_rich.py` & `logger-36-2024.5/logger_36/catalog/handler/console_rich.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.4/logger_36/catalog/handler/file.py` & `logger-36-2024.5/logger_36/catalog/handler/file.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.4/logger_36/catalog/handler/generic.py` & `logger-36-2024.5/logger_36/catalog/handler/generic.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.4/logger_36/catalog/logging/chronos.py` & `logger-36-2024.5/logger_36/catalog/logging/chronos.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.4/logger_36/catalog/logging/gpu.py` & `logger-36-2024.5/logger_36/catalog/logging/gpu.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.4/logger_36/catalog/logging/memory.py` & `logger-36-2024.5/logger_36/catalog/logging/memory.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.4/logger_36/catalog/logging/system.py` & `logger-36-2024.5/logger_36/catalog/logging/system.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.4/logger_36/config/issue.py` & `logger-36-2024.5/logger_36/config/issue.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.4/logger_36/config/memory.py` & `logger-36-2024.5/logger_36/config/memory.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.4/logger_36/config/message.py` & `logger-36-2024.5/logger_36/config/message.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.4/logger_36/config/system.py` & `logger-36-2024.5/logger_36/config/system.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.4/logger_36/constant/generic.py` & `logger-36-2024.5/logger_36/constant/generic.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.4/logger_36/constant/handler.py` & `logger-36-2024.5/logger_36/constant/handler.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.4/logger_36/constant/issue.py` & `logger-36-2024.5/logger_36/constant/issue.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.4/logger_36/constant/logger.py` & `logger-36-2024.5/logger_36/constant/logger.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.4/logger_36/constant/memory.py` & `logger-36-2024.5/logger_36/constant/memory.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.4/logger_36/constant/message.py` & `logger-36-2024.5/logger_36/constant/message.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.4/logger_36/constant/record.py` & `logger-36-2024.5/logger_36/constant/record.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.4/logger_36/constant/system.py` & `logger-36-2024.5/logger_36/constant/system.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.4/logger_36/instance.py` & `logger-36-2024.5/logger_36/instance.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.4/logger_36/main.py` & `logger-36-2024.5/logger_36/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -57,122 +57,146 @@
 from logger_36.task.format.message import FormattedMessage
 
 
 def AddGenericHandler(
     interface: interface_h,
     /,
     *,
+    logger: lggg.Logger | None = None,
     name: str | None = None,
     level: int = lggg.INFO,
     show_where: bool = True,
     show_memory_usage: bool = False,
     formatter: lggg.Formatter | None = None,
     supports_html: bool = False,
     should_hold_messages: bool = False,
     **kwargs,
 ) -> None:
     """"""
+    if logger is None:
+        logger = LOGGER
+
     handler = generic_handler_t(
         name=name,
         level=level,
         show_where=show_where,
         show_memory_usage=show_memory_usage,
         formatter=formatter,
         supports_html=supports_html,
         rich_kwargs=kwargs,
         interface=interface,
     )
-    LOGGER.AddHandler(handler, should_hold_messages)
+    logger.AddHandler(handler, should_hold_messages)
 
 
 def AddConsoleHandler(
     *,
+    logger: lggg.Logger | None = None,
     name: str | None = None,
     level: int = lggg.INFO,
     show_where: bool = True,
     show_memory_usage: bool = False,
     formatter: lggg.Formatter | None = None,
     should_hold_messages: bool = False,
 ) -> None:
     """"""
+    if logger is None:
+        logger = LOGGER
+
     handler = console_handler_t(
         name=name,
         level=level,
         show_where=show_where,
         show_memory_usage=show_memory_usage,
         formatter=formatter,
     )
-    LOGGER.AddHandler(handler, should_hold_messages)
+    logger.AddHandler(handler, should_hold_messages)
 
 
 def AddRichConsoleHandler(
     *,
+    logger: lggg.Logger | None = None,
     name: str | None = None,
     level: int = lggg.INFO,
     show_where: bool = True,
     show_memory_usage: bool = False,
     formatter: lggg.Formatter | None = None,
     should_hold_messages: bool = False,
     **kwargs,
 ) -> None:
     """"""
     global _RICH_ERROR
     if _RICH_ERROR is not None:
         print(_RICH_ERROR, file=sstm.stderr)
         _RICH_ERROR = None
 
+    if logger is None:
+        logger = LOGGER
+
     handler = console_rich_handler_t(
         name=name,
         level=level,
         show_where=show_where,
         show_memory_usage=show_memory_usage,
         formatter=formatter,
         rich_kwargs=kwargs,
     )
-    LOGGER.AddHandler(handler, should_hold_messages)
+    logger.AddHandler(handler, should_hold_messages)
 
 
 def AddFileHandler(
     path: str | path_t,
     /,
     *args,
+    logger: lggg.Logger | None = None,
     name: str | None = None,
     level: int = lggg.INFO,
     show_where: bool = True,
     show_memory_usage: bool = False,
     formatter: lggg.Formatter | None = None,
     should_hold_messages: bool = False,
     **kwargs,
 ) -> None:
     """"""
     if isinstance(path, str):
         path = path_t(path)
     if path.exists():
         raise ValueError(f"File or folder already exists: {path}.")
+    if logger is None:
+        logger = LOGGER
 
     handler = file_handler_t(
         name=name,
         level=level,
         show_where=show_where,
         show_memory_usage=show_memory_usage,
         formatter=formatter,
         path=path,
         handler_args=args,
         handler_kwargs=kwargs,
     )
-    LOGGER.AddHandler(handler, should_hold_messages)
+    logger.AddHandler(handler, should_hold_messages)
 
 
-def SetLOGLevel(level: int, /, *, which: handler_codes_h | str = "a") -> None:
+def SetLOGLevel(
+    level: int,
+    /,
+    *,
+    logger: lggg.Logger | None = None,
+    which: handler_codes_h | str = "a",
+) -> None:
     """
     which: g=generic, c=console, f=file, a=all, str=name.
     """
+    if logger is None:
+        logger = LOGGER
+
     which_is_name = which not in HANDLER_CODES
     found = False
-    for handler in LOGGER.handlers:
+    for handler in logger.handlers:
         if (
             (which == "a")
             or ((which == "g") and isinstance(handler, generic_handler_t))
             or (
                 (which == "c")
                 and isinstance(handler, (console_handler_t, console_rich_handler_t))
             )
```

### Comparing `logger-36-2024.4/logger_36/task/format/memory.py` & `logger-36-2024.5/logger_36/task/format/memory.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.4/logger_36/task/format/message.py` & `logger-36-2024.5/logger_36/task/format/message.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.4/logger_36/task/format/rule.py` & `logger-36-2024.5/logger_36/task/format/rule.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.4/logger_36/task/inspection.py` & `logger-36-2024.5/logger_36/task/inspection.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.4/logger_36/task/measure/chronos.py` & `logger-36-2024.5/logger_36/task/measure/chronos.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.4/logger_36/task/measure/memory.py` & `logger-36-2024.5/logger_36/task/measure/memory.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.4/logger_36/task/storage.py` & `logger-36-2024.5/logger_36/task/storage.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.4/logger_36/type/extension.py` & `logger-36-2024.5/logger_36/type/extension.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.4/logger_36/type/issue.py` & `logger-36-2024.5/logger_36/type/issue.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.4/logger_36/type/logger.py` & `logger-36-2024.5/logger_36/type/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -292,25 +292,24 @@
 
         if order == "when":
             issues = self.staged_issues
         else:  # order == "context"
             issues = sorted(self.staged_issues, key=lambda _elm: _elm.context)
         issues = "\n".join(issues)
 
-        if issubclass(level, Exception):
+        if isinstance(level, type) and issubclass(level, Exception):
             try:
                 raise level("\n" + issues)
             except Exception as exception:
-                traceback = "Traceback (most recent call last):\n" + "\n".join(
-                    tbck.format_stack()[:-1]
-                )
-                print(traceback[:-1], file=sstm.stderr)
-                print(
-                    "\n".join(tbck.format_exception_only(exception)), file=sstm.stderr
-                )
+                lines = ["Traceback (most recent call last):"] + tbck.format_stack()[
+                    :-1
+                ]
+                lines[-1] = lines[-1][:-1]
+                lines.extend(tbck.format_exception_only(exception))
+                print("\n".join(lines), file=sstm.stderr)
                 sstm.exit(1)
 
         self.log(level, issues, **HIDE_WHERE_KWARG)
         self.staged_issues.clear()
 
     def __enter__(self) -> None:
         """"""
```

### Comparing `logger-36-2024.4/logger_36/version.py` & `logger-36-2024.5/logger_36/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-__version__ = "2024.4"
+__version__ = "2024.5"
```

### Comparing `logger-36-2024.4/logger_36.egg-info/PKG-INFO` & `logger-36-2024.5/logger_36.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: logger-36
-Version: 2024.4
+Version: 2024.5
 Summary: Simple logger with a catalog of handlers
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/logger-36/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/logger-36//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/logger-36/
 Keywords: log,warning,error
 Classifier: Topic :: Software Development
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 
 ..
    Copyright CNRS/Inria/UCA
    Contributor(s): Eric Debreuve (since 2023)
```

### Comparing `logger-36-2024.4/logger_36.egg-info/SOURCES.txt` & `logger-36-2024.5/logger_36.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `logger-36-2024.4/setup.py` & `logger-36-2024.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,22 +55,23 @@
 
 
 DESCRIPTION = DescriptionFromDocumentation(DOCUMENTATION_HOME)
 
 
 LICENSE_SHORT = "CeCILL-2.1"
 LICENCE_LONG = "CEA CNRS Inria Logiciel Libre License, version 2.1"
-PY_VERSION = "3.10"
+PY_VERSION = "3"
+PY_VERSION_MIN = "3.10"
 
 DOCUMENTATION_SITE = "-/wikis/home"
 
 PYPI_NAME = "logger-36"
 PYPI_TOPIC = "Software Development"
 PYPI_AUDIENCE = "Developers"
-PYPI_STATUS = "4 - Beta"
+PYPI_STATUS = "5 - Production/Stable"
 
 IMPORT_NAME = "logger_36"
 PACKAGES = [
     IMPORT_NAME,
     f"{IMPORT_NAME}.catalog",
     f"{IMPORT_NAME}.catalog.config",
     f"{IMPORT_NAME}.catalog.handler",
@@ -160,10 +161,10 @@
         project_urls={
             "Documentation": documentation_url,
             "Source": repository_url,
         },
         #
         packages=PACKAGES,
         entry_points=ENTRY_POINTS,
-        python_requires=f">={PY_VERSION}",
+        python_requires=f">={PY_VERSION_MIN}",
         install_requires=[],
     )
```

