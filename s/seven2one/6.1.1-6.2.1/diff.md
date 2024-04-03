# Comparing `tmp/seven2one-6.1.1.tar.gz` & `tmp/seven2one-6.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seven2one-6.1.1.tar", last modified: Wed Mar  6 13:02:36 2024, max compression
+gzip compressed data, was "seven2one-6.2.1.tar", last modified: Wed Apr  3 17:11:18 2024, max compression
```

## Comparing `seven2one-6.1.1.tar` & `seven2one-6.2.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 13:02:36.573901 seven2one-6.1.1/
--rw-r--r--   0 root         (0) root         (0)     1105 2024-02-14 12:57:01.000000 seven2one-6.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-14 12:57:01.000000 seven2one-6.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3618 2024-03-06 13:02:36.573901 seven2one-6.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2900 2024-02-14 12:57:01.000000 seven2one-6.1.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-06 13:02:36.573901 seven2one-6.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1409 2024-02-14 12:57:01.000000 seven2one-6.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 13:02:36.569901 seven2one-6.1.1/seven2one/
--rw-r--r--   0 root         (0) root         (0)       51 2024-03-06 13:02:30.000000 seven2one-6.1.1/seven2one/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15031 2024-03-05 16:59:04.000000 seven2one-6.1.1/seven2one/authorization.py
--rw-r--r--   0 root         (0) root         (0)    13131 2024-02-14 12:57:01.000000 seven2one-6.1.1/seven2one/automation.py
--rw-r--r--   0 root         (0) root         (0)    72493 2024-03-05 16:59:04.000000 seven2one-6.1.1/seven2one/core.py
--rw-r--r--   0 root         (0) root         (0)     4415 2024-02-14 12:57:01.000000 seven2one-6.1.1/seven2one/email.py
--rw-r--r--   0 root         (0) root         (0)    51882 2024-03-05 16:59:04.000000 seven2one-6.1.1/seven2one/fileimport.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 13:02:36.569901 seven2one-6.1.1/seven2one/logging_loki/
--rw-r--r--   0 root         (0) root         (0)      189 2024-02-14 12:57:01.000000 seven2one-6.1.1/seven2one/logging_loki/__init__.py
--rw-r--r--   0 root         (0) root         (0)      756 2024-02-14 12:57:01.000000 seven2one-6.1.1/seven2one/logging_loki/const.py
--rw-r--r--   0 root         (0) root         (0)     5720 2024-02-14 12:57:01.000000 seven2one-6.1.1/seven2one/logging_loki/emitter.py
--rw-r--r--   0 root         (0) root         (0)     2929 2024-02-14 12:57:01.000000 seven2one-6.1.1/seven2one/logging_loki/handlers.py
--rw-r--r--   0 root         (0) root         (0)    15797 2024-02-14 12:57:01.000000 seven2one-6.1.1/seven2one/programming.py
--rw-r--r--   0 root         (0) root         (0)     9977 2024-02-14 12:57:01.000000 seven2one-6.1.1/seven2one/schedule.py
--rw-r--r--   0 root         (0) root         (0)    70316 2024-03-05 16:59:04.000000 seven2one-6.1.1/seven2one/timeseries.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 13:02:36.573901 seven2one-6.1.1/seven2one/utils/
--rw-r--r--   0 root         (0) root         (0)     4197 2024-02-14 12:57:01.000000 seven2one-6.1.1/seven2one/utils/DeviceClient.py
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-06 13:02:30.000000 seven2one-6.1.1/seven2one/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    37980 2024-03-05 16:59:04.000000 seven2one-6.1.1/seven2one/utils/ut.py
--rw-r--r--   0 root         (0) root         (0)      396 2024-02-14 12:57:01.000000 seven2one-6.1.1/seven2one/utils/ut_auth.py
--rw-r--r--   0 root         (0) root         (0)     2005 2024-02-14 12:57:01.000000 seven2one-6.1.1/seven2one/utils/ut_autprog.py
--rw-r--r--   0 root         (0) root         (0)    27578 2024-02-14 12:57:01.000000 seven2one-6.1.1/seven2one/utils/ut_fileimport.py
--rw-r--r--   0 root         (0) root         (0)     6091 2024-02-14 12:57:01.000000 seven2one-6.1.1/seven2one/utils/ut_init.py
--rw-r--r--   0 root         (0) root         (0)     1000 2024-02-14 12:57:01.000000 seven2one-6.1.1/seven2one/utils/ut_log.py
--rw-r--r--   0 root         (0) root         (0)     4229 2024-02-14 12:57:01.000000 seven2one-6.1.1/seven2one/utils/ut_meta.py
--rw-r--r--   0 root         (0) root         (0)     4711 2024-03-05 16:59:04.000000 seven2one-6.1.1/seven2one/utils/ut_time.py
--rw-r--r--   0 root         (0) root         (0)     7336 2024-03-05 16:59:04.000000 seven2one-6.1.1/seven2one/utils/ut_timeseries.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 13:02:36.573901 seven2one-6.1.1/seven2one.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3618 2024-03-06 13:02:36.000000 seven2one-6.1.1/seven2one.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      887 2024-03-06 13:02:36.000000 seven2one-6.1.1/seven2one.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-06 13:02:36.000000 seven2one-6.1.1/seven2one.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-06 13:02:36.000000 seven2one-6.1.1/seven2one.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      115 2024-03-06 13:02:36.000000 seven2one-6.1.1/seven2one.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-03-06 13:02:36.000000 seven2one-6.1.1/seven2one.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:11:18.652079 seven2one-6.2.1/
+-rw-r--r--   0 root         (0) root         (0)     1105 2024-02-14 12:57:01.000000 seven2one-6.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-14 12:57:01.000000 seven2one-6.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3618 2024-04-03 17:11:18.648079 seven2one-6.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2900 2024-02-14 12:57:01.000000 seven2one-6.2.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 17:11:18.652079 seven2one-6.2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1409 2024-02-14 12:57:01.000000 seven2one-6.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:11:18.644080 seven2one-6.2.1/seven2one/
+-rw-r--r--   0 root         (0) root         (0)       51 2024-04-03 17:11:12.000000 seven2one-6.2.1/seven2one/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28177 2024-03-28 08:35:44.000000 seven2one-6.2.1/seven2one/authorization.py
+-rw-r--r--   0 root         (0) root         (0)    13131 2024-02-14 12:57:01.000000 seven2one-6.2.1/seven2one/automation.py
+-rw-r--r--   0 root         (0) root         (0)    72493 2024-03-05 16:59:04.000000 seven2one-6.2.1/seven2one/core.py
+-rw-r--r--   0 root         (0) root         (0)     4415 2024-02-14 12:57:01.000000 seven2one-6.2.1/seven2one/email.py
+-rw-r--r--   0 root         (0) root         (0)    51882 2024-03-05 16:59:04.000000 seven2one-6.2.1/seven2one/fileimport.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:11:18.648079 seven2one-6.2.1/seven2one/logging_loki/
+-rw-r--r--   0 root         (0) root         (0)      189 2024-02-14 12:57:01.000000 seven2one-6.2.1/seven2one/logging_loki/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      756 2024-02-14 12:57:01.000000 seven2one-6.2.1/seven2one/logging_loki/const.py
+-rw-r--r--   0 root         (0) root         (0)     5720 2024-02-14 12:57:01.000000 seven2one-6.2.1/seven2one/logging_loki/emitter.py
+-rw-r--r--   0 root         (0) root         (0)     2929 2024-02-14 12:57:01.000000 seven2one-6.2.1/seven2one/logging_loki/handlers.py
+-rw-r--r--   0 root         (0) root         (0)    15797 2024-02-14 12:57:01.000000 seven2one-6.2.1/seven2one/programming.py
+-rw-r--r--   0 root         (0) root         (0)     9977 2024-02-14 12:57:01.000000 seven2one-6.2.1/seven2one/schedule.py
+-rw-r--r--   0 root         (0) root         (0)    70316 2024-03-05 16:59:04.000000 seven2one-6.2.1/seven2one/timeseries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:11:18.648079 seven2one-6.2.1/seven2one/utils/
+-rw-r--r--   0 root         (0) root         (0)     4197 2024-02-14 12:57:01.000000 seven2one-6.2.1/seven2one/utils/DeviceClient.py
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-03 17:11:12.000000 seven2one-6.2.1/seven2one/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    37980 2024-03-05 16:59:04.000000 seven2one-6.2.1/seven2one/utils/ut.py
+-rw-r--r--   0 root         (0) root         (0)      396 2024-02-14 12:57:01.000000 seven2one-6.2.1/seven2one/utils/ut_auth.py
+-rw-r--r--   0 root         (0) root         (0)     2005 2024-02-14 12:57:01.000000 seven2one-6.2.1/seven2one/utils/ut_autprog.py
+-rw-r--r--   0 root         (0) root         (0)    27578 2024-02-14 12:57:01.000000 seven2one-6.2.1/seven2one/utils/ut_fileimport.py
+-rw-r--r--   0 root         (0) root         (0)     6091 2024-02-14 12:57:01.000000 seven2one-6.2.1/seven2one/utils/ut_init.py
+-rw-r--r--   0 root         (0) root         (0)     1000 2024-02-14 12:57:01.000000 seven2one-6.2.1/seven2one/utils/ut_log.py
+-rw-r--r--   0 root         (0) root         (0)     4229 2024-02-14 12:57:01.000000 seven2one-6.2.1/seven2one/utils/ut_meta.py
+-rw-r--r--   0 root         (0) root         (0)     4711 2024-03-05 16:59:04.000000 seven2one-6.2.1/seven2one/utils/ut_time.py
+-rw-r--r--   0 root         (0) root         (0)     7336 2024-03-05 16:59:04.000000 seven2one-6.2.1/seven2one/utils/ut_timeseries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:11:18.648079 seven2one-6.2.1/seven2one.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3618 2024-04-03 17:11:18.000000 seven2one-6.2.1/seven2one.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      887 2024-04-03 17:11:18.000000 seven2one-6.2.1/seven2one.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 17:11:18.000000 seven2one-6.2.1/seven2one.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 17:11:18.000000 seven2one-6.2.1/seven2one.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      115 2024-04-03 17:11:18.000000 seven2one-6.2.1/seven2one.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-03 17:11:18.000000 seven2one-6.2.1/seven2one.egg-info/top_level.txt
```

### Comparing `seven2one-6.1.1/LICENSE` & `seven2one-6.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `seven2one-6.1.1/PKG-INFO` & `seven2one-6.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seven2one
-Version: 6.1.1
+Version: 6.2.1
 Summary: Functions to interact with the Seven2one TechStack
 Home-page: http://www.seven2one.de
 Author: Seven2one Informationssysteme GmbH
 Author-email: info@seven2one.de
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
```

### Comparing `seven2one-6.1.1/README.md` & `seven2one-6.2.1/README.md`

 * *Files identical despite different names*

### Comparing `seven2one-6.1.1/setup.py` & `seven2one-6.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `seven2one-6.1.1/seven2one/automation.py` & `seven2one-6.2.1/seven2one/automation.py`

 * *Files identical despite different names*

### Comparing `seven2one-6.1.1/seven2one/core.py` & `seven2one-6.2.1/seven2one/core.py`

 * *Files identical despite different names*

### Comparing `seven2one-6.1.1/seven2one/email.py` & `seven2one-6.2.1/seven2one/email.py`

 * *Files identical despite different names*

### Comparing `seven2one-6.1.1/seven2one/fileimport.py` & `seven2one-6.2.1/seven2one/fileimport.py`

 * *Files identical despite different names*

### Comparing `seven2one-6.1.1/seven2one/logging_loki/const.py` & `seven2one-6.2.1/seven2one/logging_loki/const.py`

 * *Files identical despite different names*

### Comparing `seven2one-6.1.1/seven2one/logging_loki/emitter.py` & `seven2one-6.2.1/seven2one/logging_loki/emitter.py`

 * *Files identical despite different names*

### Comparing `seven2one-6.1.1/seven2one/logging_loki/handlers.py` & `seven2one-6.2.1/seven2one/logging_loki/handlers.py`

 * *Files identical despite different names*

### Comparing `seven2one-6.1.1/seven2one/programming.py` & `seven2one-6.2.1/seven2one/programming.py`

 * *Files identical despite different names*

### Comparing `seven2one-6.1.1/seven2one/schedule.py` & `seven2one-6.2.1/seven2one/schedule.py`

 * *Files identical despite different names*

### Comparing `seven2one-6.1.1/seven2one/timeseries.py` & `seven2one-6.2.1/seven2one/timeseries.py`

 * *Files identical despite different names*

### Comparing `seven2one-6.1.1/seven2one/utils/DeviceClient.py` & `seven2one-6.2.1/seven2one/utils/DeviceClient.py`

 * *Files identical despite different names*

### Comparing `seven2one-6.1.1/seven2one/utils/ut.py` & `seven2one-6.2.1/seven2one/utils/ut.py`

 * *Files identical despite different names*

### Comparing `seven2one-6.1.1/seven2one/utils/ut_autprog.py` & `seven2one-6.2.1/seven2one/utils/ut_autprog.py`

 * *Files identical despite different names*

### Comparing `seven2one-6.1.1/seven2one/utils/ut_fileimport.py` & `seven2one-6.2.1/seven2one/utils/ut_fileimport.py`

 * *Files identical despite different names*

### Comparing `seven2one-6.1.1/seven2one/utils/ut_init.py` & `seven2one-6.2.1/seven2one/utils/ut_init.py`

 * *Files identical despite different names*

### Comparing `seven2one-6.1.1/seven2one/utils/ut_log.py` & `seven2one-6.2.1/seven2one/utils/ut_log.py`

 * *Files identical despite different names*

### Comparing `seven2one-6.1.1/seven2one/utils/ut_meta.py` & `seven2one-6.2.1/seven2one/utils/ut_meta.py`

 * *Files identical despite different names*

### Comparing `seven2one-6.1.1/seven2one/utils/ut_time.py` & `seven2one-6.2.1/seven2one/utils/ut_time.py`

 * *Files identical despite different names*

### Comparing `seven2one-6.1.1/seven2one/utils/ut_timeseries.py` & `seven2one-6.2.1/seven2one/utils/ut_timeseries.py`

 * *Files identical despite different names*

### Comparing `seven2one-6.1.1/seven2one.egg-info/PKG-INFO` & `seven2one-6.2.1/seven2one.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seven2one
-Version: 6.1.1
+Version: 6.2.1
 Summary: Functions to interact with the Seven2one TechStack
 Home-page: http://www.seven2one.de
 Author: Seven2one Informationssysteme GmbH
 Author-email: info@seven2one.de
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
```

### Comparing `seven2one-6.1.1/seven2one.egg-info/SOURCES.txt` & `seven2one-6.2.1/seven2one.egg-info/SOURCES.txt`

 * *Files identical despite different names*

