# Comparing `tmp/airbyte-source-google-drive-0.0.8.tar.gz` & `tmp/airbyte-source-google-drive-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-google-drive-0.0.8.tar", last modified: Thu Feb  1 14:00:30 2024, max compression
+gzip compressed data, was "airbyte-source-google-drive-0.0.9.tar", last modified: Wed Feb  7 01:11:14 2024, max compression
```

## Comparing `airbyte-source-google-drive-0.0.8.tar` & `airbyte-source-google-drive-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 14:00:30.745006 airbyte-source-google-drive-0.0.8/
--rw-r--r--   0 root         (0) root         (0)     5630 2024-02-01 14:00:30.745006 airbyte-source-google-drive-0.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5460 2024-02-01 13:41:31.000000 airbyte-source-google-drive-0.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 14:00:30.745006 airbyte-source-google-drive-0.0.8/airbyte_source_google_drive.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5630 2024-02-01 14:00:30.000000 airbyte-source-google-drive-0.0.8/airbyte_source_google_drive.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      727 2024-02-01 14:00:30.000000 airbyte-source-google-drive-0.0.8/airbyte_source_google_drive.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-01 14:00:30.000000 airbyte-source-google-drive-0.0.8/airbyte_source_google_drive.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       68 2024-02-01 14:00:30.000000 airbyte-source-google-drive-0.0.8/airbyte_source_google_drive.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      201 2024-02-01 14:00:30.000000 airbyte-source-google-drive-0.0.8/airbyte_source_google_drive.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-01 14:00:30.000000 airbyte-source-google-drive-0.0.8/airbyte_source_google_drive.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 14:00:30.745006 airbyte-source-google-drive-0.0.8/integration_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-01 13:41:31.000000 airbyte-source-google-drive-0.0.8/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      986 2024-02-01 13:41:31.000000 airbyte-source-google-drive-0.0.8/integration_tests/abnormal_state.json
--rw-r--r--   0 root         (0) root         (0)      361 2024-02-01 13:41:31.000000 airbyte-source-google-drive-0.0.8/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)     1600 2024-02-01 13:41:31.000000 airbyte-source-google-drive-0.0.8/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)      403 2024-02-01 13:41:31.000000 airbyte-source-google-drive-0.0.8/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)    21010 2024-02-01 13:41:31.000000 airbyte-source-google-drive-0.0.8/integration_tests/spec.json
--rw-r--r--   0 root         (0) root         (0)     5367 2024-02-01 14:00:30.745006 airbyte-source-google-drive-0.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1083 2024-02-01 14:00:28.000000 airbyte-source-google-drive-0.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 14:00:30.745006 airbyte-source-google-drive-0.0.8/source_google_drive/
--rw-r--r--   0 root         (0) root         (0)      132 2024-02-01 13:41:31.000000 airbyte-source-google-drive-0.0.8/source_google_drive/__init__.py
--rw-r--r--   0 root         (0) root         (0)      711 2024-02-01 13:41:31.000000 airbyte-source-google-drive-0.0.8/source_google_drive/run.py
--rw-r--r--   0 root         (0) root         (0)     2827 2024-02-01 13:41:31.000000 airbyte-source-google-drive-0.0.8/source_google_drive/source.py
--rw-r--r--   0 root         (0) root         (0)     3401 2024-02-01 13:41:31.000000 airbyte-source-google-drive-0.0.8/source_google_drive/spec.py
--rw-r--r--   0 root         (0) root         (0)     8533 2024-02-01 13:41:31.000000 airbyte-source-google-drive-0.0.8/source_google_drive/stream_reader.py
--rw-r--r--   0 root         (0) root         (0)      941 2024-02-01 13:41:31.000000 airbyte-source-google-drive-0.0.8/source_google_drive/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 01:11:14.247172 airbyte-source-google-drive-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)     5630 2024-02-07 01:11:14.247172 airbyte-source-google-drive-0.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5460 2024-02-07 00:13:16.000000 airbyte-source-google-drive-0.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 01:11:14.247172 airbyte-source-google-drive-0.0.9/airbyte_source_google_drive.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5630 2024-02-07 01:11:14.000000 airbyte-source-google-drive-0.0.9/airbyte_source_google_drive.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      727 2024-02-07 01:11:14.000000 airbyte-source-google-drive-0.0.9/airbyte_source_google_drive.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-07 01:11:14.000000 airbyte-source-google-drive-0.0.9/airbyte_source_google_drive.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       68 2024-02-07 01:11:14.000000 airbyte-source-google-drive-0.0.9/airbyte_source_google_drive.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      201 2024-02-07 01:11:14.000000 airbyte-source-google-drive-0.0.9/airbyte_source_google_drive.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-02-07 01:11:14.000000 airbyte-source-google-drive-0.0.9/airbyte_source_google_drive.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 01:11:14.243172 airbyte-source-google-drive-0.0.9/integration_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-07 00:13:16.000000 airbyte-source-google-drive-0.0.9/integration_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      986 2024-02-07 00:13:16.000000 airbyte-source-google-drive-0.0.9/integration_tests/abnormal_state.json
+-rw-r--r--   0 root         (0) root         (0)      361 2024-02-07 00:13:16.000000 airbyte-source-google-drive-0.0.9/integration_tests/acceptance.py
+-rw-r--r--   0 root         (0) root         (0)     1600 2024-02-07 00:13:16.000000 airbyte-source-google-drive-0.0.9/integration_tests/configured_catalog.json
+-rw-r--r--   0 root         (0) root         (0)      403 2024-02-07 00:13:16.000000 airbyte-source-google-drive-0.0.9/integration_tests/invalid_config.json
+-rw-r--r--   0 root         (0) root         (0)    21010 2024-02-07 00:13:16.000000 airbyte-source-google-drive-0.0.9/integration_tests/spec.json
+-rw-r--r--   0 root         (0) root         (0)     5367 2024-02-07 01:11:14.247172 airbyte-source-google-drive-0.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1083 2024-02-07 01:11:12.000000 airbyte-source-google-drive-0.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 01:11:14.247172 airbyte-source-google-drive-0.0.9/source_google_drive/
+-rw-r--r--   0 root         (0) root         (0)      132 2024-02-07 00:13:16.000000 airbyte-source-google-drive-0.0.9/source_google_drive/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      711 2024-02-07 00:13:16.000000 airbyte-source-google-drive-0.0.9/source_google_drive/run.py
+-rw-r--r--   0 root         (0) root         (0)     2827 2024-02-07 00:13:16.000000 airbyte-source-google-drive-0.0.9/source_google_drive/source.py
+-rw-r--r--   0 root         (0) root         (0)     3401 2024-02-07 00:13:16.000000 airbyte-source-google-drive-0.0.9/source_google_drive/spec.py
+-rw-r--r--   0 root         (0) root         (0)     8533 2024-02-07 00:13:16.000000 airbyte-source-google-drive-0.0.9/source_google_drive/stream_reader.py
+-rw-r--r--   0 root         (0) root         (0)      941 2024-02-07 00:13:16.000000 airbyte-source-google-drive-0.0.9/source_google_drive/utils.py
```

### Comparing `airbyte-source-google-drive-0.0.8/PKG-INFO` & `airbyte-source-google-drive-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: airbyte-source-google-drive
-Version: 0.0.8
+Version: 0.0.9
 Summary: Source implementation for Google Drive.
 Author: Airbyte
 Author-email: contact@airbyte.io
 Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk[file-based]>=0.60.1
+Requires-Dist: airbyte-cdk[file-based]>=0.61.0
 Requires-Dist: google-api-python-client==2.104.0
 Requires-Dist: google-auth-httplib2==0.1.1
 Requires-Dist: google-auth-oauthlib==1.1.0
 Requires-Dist: google-api-python-client-stubs==1.18.0
 Provides-Extra: tests
 Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
 Requires-Dist: pytest~=6.1; extra == "tests"
```

### Comparing `airbyte-source-google-drive-0.0.8/README.md` & `airbyte-source-google-drive-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `airbyte-source-google-drive-0.0.8/airbyte_source_google_drive.egg-info/PKG-INFO` & `airbyte-source-google-drive-0.0.9/airbyte_source_google_drive.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: airbyte-source-google-drive
-Version: 0.0.8
+Version: 0.0.9
 Summary: Source implementation for Google Drive.
 Author: Airbyte
 Author-email: contact@airbyte.io
 Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk[file-based]>=0.60.1
+Requires-Dist: airbyte-cdk[file-based]>=0.61.0
 Requires-Dist: google-api-python-client==2.104.0
 Requires-Dist: google-auth-httplib2==0.1.1
 Requires-Dist: google-auth-oauthlib==1.1.0
 Requires-Dist: google-api-python-client-stubs==1.18.0
 Provides-Extra: tests
 Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
 Requires-Dist: pytest~=6.1; extra == "tests"
```

### Comparing `airbyte-source-google-drive-0.0.8/airbyte_source_google_drive.egg-info/SOURCES.txt` & `airbyte-source-google-drive-0.0.9/airbyte_source_google_drive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `airbyte-source-google-drive-0.0.8/integration_tests/abnormal_state.json` & `airbyte-source-google-drive-0.0.9/integration_tests/abnormal_state.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-google-drive-0.0.8/integration_tests/configured_catalog.json` & `airbyte-source-google-drive-0.0.9/integration_tests/configured_catalog.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-google-drive-0.0.8/integration_tests/spec.json` & `airbyte-source-google-drive-0.0.9/integration_tests/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-google-drive-0.0.8/setup.cfg` & `airbyte-source-google-drive-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = airbyte-source-google-drive
-version = 0.0.8
+version = 0.0.9
 author = Airbyte
 author_email = contact@airbyte.io
 long_description = # Google Drive Source
 	
 	This is the repository for the Google Drive source connector, written in Python.
 	For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/google-drive).
```

### Comparing `airbyte-source-google-drive-0.0.8/setup.py` & `airbyte-source-google-drive-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 
 from setuptools import find_packages, setup
 
 MAIN_REQUIREMENTS = [
-    "airbyte-cdk[file-based]>=0.60.1",
+    "airbyte-cdk[file-based]>=0.61.0",
     "google-api-python-client==2.104.0",
     "google-auth-httplib2==0.1.1",
     "google-auth-oauthlib==1.1.0",
     "google-api-python-client-stubs==1.18.0",
 ]
 
 TEST_REQUIREMENTS = [
```

### Comparing `airbyte-source-google-drive-0.0.8/source_google_drive/run.py` & `airbyte-source-google-drive-0.0.9/source_google_drive/run.py`

 * *Files identical despite different names*

### Comparing `airbyte-source-google-drive-0.0.8/source_google_drive/source.py` & `airbyte-source-google-drive-0.0.9/source_google_drive/source.py`

 * *Files identical despite different names*

### Comparing `airbyte-source-google-drive-0.0.8/source_google_drive/spec.py` & `airbyte-source-google-drive-0.0.9/source_google_drive/spec.py`

 * *Files identical despite different names*

### Comparing `airbyte-source-google-drive-0.0.8/source_google_drive/stream_reader.py` & `airbyte-source-google-drive-0.0.9/source_google_drive/stream_reader.py`

 * *Files identical despite different names*

### Comparing `airbyte-source-google-drive-0.0.8/source_google_drive/utils.py` & `airbyte-source-google-drive-0.0.9/source_google_drive/utils.py`

 * *Files identical despite different names*

