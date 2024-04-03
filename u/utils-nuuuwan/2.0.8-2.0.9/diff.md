# Comparing `tmp/utils-nuuuwan-2.0.8.tar.gz` & `tmp/utils-nuuuwan-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utils-nuuuwan-2.0.8.tar", last modified: Sun Nov  5 14:07:05 2023, max compression
+gzip compressed data, was "utils-nuuuwan-2.0.9.tar", last modified: Wed Apr  3 16:27:54 2024, max compression
```

## Comparing `utils-nuuuwan-2.0.8.tar` & `utils-nuuuwan-2.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-05 14:07:05.572899 utils-nuuuwan-2.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-11-05 14:06:24.000000 utils-nuuuwan-2.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      723 2023-11-05 14:07:05.572899 utils-nuuuwan-2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      793 2023-11-05 14:06:24.000000 utils-nuuuwan-2.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-05 14:07:05.572899 utils-nuuuwan-2.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2023-11-05 14:06:24.000000 utils-nuuuwan-2.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-05 14:07:05.572899 utils-nuuuwan-2.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-05 14:07:05.572899 utils-nuuuwan-2.0.8/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      768 2023-11-05 14:06:24.000000 utils-nuuuwan-2.0.8/src/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-05 14:07:05.572899 utils-nuuuwan-2.0.8/src/utils_nuuuwan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      723 2023-11-05 14:07:05.000000 utils-nuuuwan-2.0.8/src/utils_nuuuwan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      271 2023-11-05 14:07:05.000000 utils-nuuuwan-2.0.8/src/utils_nuuuwan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-05 14:07:05.000000 utils-nuuuwan-2.0.8/src/utils_nuuuwan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2023-11-05 14:07:05.000000 utils-nuuuwan-2.0.8/src/utils_nuuuwan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-11-05 14:07:05.000000 utils-nuuuwan-2.0.8/src/utils_nuuuwan.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-05 14:07:05.572899 utils-nuuuwan-2.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2023-11-05 14:06:24.000000 utils-nuuuwan-2.0.8/tests/test_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:27:54.826784 utils-nuuuwan-2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-03 16:27:00.000000 utils-nuuuwan-2.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-03 16:27:54.822784 utils-nuuuwan-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-03 16:27:00.000000 utils-nuuuwan-2.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 16:27:54.826784 utils-nuuuwan-2.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-03 16:27:00.000000 utils-nuuuwan-2.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:27:54.822784 utils-nuuuwan-2.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:27:54.822784 utils-nuuuwan-2.0.9/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-03 16:27:00.000000 utils-nuuuwan-2.0.9/src/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:27:54.822784 utils-nuuuwan-2.0.9/src/utils_nuuuwan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-03 16:27:54.000000 utils-nuuuwan-2.0.9/src/utils_nuuuwan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-03 16:27:54.000000 utils-nuuuwan-2.0.9/src/utils_nuuuwan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 16:27:54.000000 utils-nuuuwan-2.0.9/src/utils_nuuuwan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-03 16:27:54.000000 utils-nuuuwan-2.0.9/src/utils_nuuuwan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-03 16:27:54.000000 utils-nuuuwan-2.0.9/src/utils_nuuuwan.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:27:54.822784 utils-nuuuwan-2.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-03 16:27:00.000000 utils-nuuuwan-2.0.9/tests/test_init.py
```

### Comparing `utils-nuuuwan-2.0.8/LICENSE` & `utils-nuuuwan-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `utils-nuuuwan-2.0.8/PKG-INFO` & `utils-nuuuwan-2.0.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utils-nuuuwan
-Version: 2.0.8
+Version: 2.0.9
 Summary: Utilities, complementing the Python Standard Library
 Home-page: https://github.com/nuuuwan/utils
 Author: Nuwan I. Senaratna
 Author-email: nuuuwan@gmail.com
 Project-URL: Bug Tracker, https://github.com/nuuuwan/utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `utils-nuuuwan-2.0.8/setup.py` & `utils-nuuuwan-2.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Setup."""
 
 import setuptools
 
 DIST_NAME = 'utils'
-VERSION = "2.0.8"
+VERSION = "2.0.9"
 DESCRIPTION = "Utilities, complementing the Python Standard Library"
 INSTALL_REQUIRES = [
     'utils_ai-nuuuwan',
     'utils_base-nuuuwan',
     'utils_git-nuuuwan',
     'utils_lang-nuuuwan',
     'utils_twitter-nuuuwan',
```

### Comparing `utils-nuuuwan-2.0.8/src/utils/__init__.py` & `utils-nuuuwan-2.0.9/src/utils/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-# non base
+
 from utils_ai import AI
-from utils_base import (COLOR_BACKGROUND, COLOR_FOREGROUND, COLOR_FORMAT,
-                        DAYS_IN, SECONDS_IN, TIME_FORMAT_DATE,
-                        TIME_FORMAT_DATE_ID, TIME_FORMAT_TIME,
-                        TIME_FORMAT_TIME_ID, TIMEZONE_OFFSET, Console, CSVFile,
+from utils_base import (COLOR_BACKGROUND, COLOR_FOREGROUND, COLOR_FORMAT, TimeZoneOffset, Console, CSVFile,
                         Dict, Directory, File, FiledVariable, Image, JSONFile,
                         LatLng, LatLngLK, List, Log, PDFFile, String, Time,
                         TimeDelta, TimeFormat, TimeUnit, TSVFile, XSVFile, Zip,
-                        _, _log, get_date_id, get_time_id, hashx, mr, xmlx)
+                        _, Hash, Parallel, XMLElement, XMLUtils)
 from utils_git import Git
 from utils_lang import TTS, Language, Translator
 from utils_twitter import Tweet, Twitter
 from utils_www import WWW
```

### Comparing `utils-nuuuwan-2.0.8/src/utils_nuuuwan.egg-info/PKG-INFO` & `utils-nuuuwan-2.0.9/src/utils_nuuuwan.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utils-nuuuwan
-Version: 2.0.8
+Version: 2.0.9
 Summary: Utilities, complementing the Python Standard Library
 Home-page: https://github.com/nuuuwan/utils
 Author: Nuwan I. Senaratna
 Author-email: nuuuwan@gmail.com
 Project-URL: Bug Tracker, https://github.com/nuuuwan/utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

