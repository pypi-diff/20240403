# Comparing `tmp/AppWrapper-0.2.6.tar.gz` & `tmp/AppWrapper-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AppWrapper-0.2.6.tar", last modified: Tue Apr  2 07:26:57 2024, max compression
+gzip compressed data, was "AppWrapper-0.2.7.tar", last modified: Wed Apr  3 04:28:01 2024, max compression
```

## Comparing `AppWrapper-0.2.6.tar` & `AppWrapper-0.2.7.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:26:57.888891 AppWrapper-0.2.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:26:57.888891 AppWrapper-0.2.6/AppWrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-02 07:26:57.000000 AppWrapper-0.2.6/AppWrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-02 07:26:57.000000 AppWrapper-0.2.6/AppWrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 07:26:57.000000 AppWrapper-0.2.6/AppWrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 07:26:57.000000 AppWrapper-0.2.6/AppWrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-02 07:26:57.000000 AppWrapper-0.2.6/AppWrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-02 07:26:57.888891 AppWrapper-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-02 07:26:46.000000 AppWrapper-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:26:57.888891 AppWrapper-0.2.6/app_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-02 07:26:46.000000 AppWrapper-0.2.6/app_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10463 2024-04-02 07:26:46.000000 AppWrapper-0.2.6/app_wrapper/app_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 07:26:57.888891 AppWrapper-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-02 07:26:46.000000 AppWrapper-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:28:01.803623 AppWrapper-0.2.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:28:01.803623 AppWrapper-0.2.7/AppWrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-03 04:28:01.000000 AppWrapper-0.2.7/AppWrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-03 04:28:01.000000 AppWrapper-0.2.7/AppWrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 04:28:01.000000 AppWrapper-0.2.7/AppWrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-03 04:28:01.000000 AppWrapper-0.2.7/AppWrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-03 04:28:01.000000 AppWrapper-0.2.7/AppWrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-03 04:28:01.803623 AppWrapper-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 04:27:50.000000 AppWrapper-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:28:01.803623 AppWrapper-0.2.7/app_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-03 04:27:50.000000 AppWrapper-0.2.7/app_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10083 2024-04-03 04:27:50.000000 AppWrapper-0.2.7/app_wrapper/app_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-03 04:27:50.000000 AppWrapper-0.2.7/app_wrapper/task_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 04:28:01.803623 AppWrapper-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-03 04:27:50.000000 AppWrapper-0.2.7/setup.py
```

### Comparing `AppWrapper-0.2.6/app_wrapper/app_wrapper.py` & `AppWrapper-0.2.7/app_wrapper/app_wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import ast
 import json
 import os
 import pathlib
-from enum import Enum
 
 import requests
 import boto3
 import logging
 import traceback
 
+from task_status import Status
 
 logger = logging.getLogger("app_wrapper")
 logger.setLevel(logging.INFO)
 
 # Create console handler and set level to debug
 ch = logging.StreamHandler()
 ch.setLevel(logging.INFO)
@@ -46,23 +46,14 @@
         ):
             self._seen_percentages[percentage] = True
             logger.info(
                 f"Download progress for '{self._filename}': {percentage}%"
             )
 
 
-class Status(str, Enum):
-    Complete = "Complete"
-    Processing = "Processing"
-    Failed = "Failed"
-    Canceled = "Canceled"
-    Scheduled = "Scheduled"
-    Paused = "Paused"
-
-
 class AppWrapper:
     LOCAL_MODE = None
     AWS_ACCESS_KEY_ID = None
     AWS_SECRET_ACCESS_KEY = None
     AWS_DEFAULT_REGION = None
 
     def __init__(
@@ -251,23 +242,17 @@
                     result = func(*args, **kwargs)
                 except Exception as e:
                     logger.error(e)
             else:
                 try:
                     result = func(*args, **kwargs)
                 except Exception as e:
-                    print(f"temp: Exception {str(e)}")
-                    logger.error(e)
                     logger.error(traceback.format_exc())
                     self.send_pod_log_to_s3()
-                    print(f"after send_pod_log_to_s3")
-
                     self.update_status(Status.Failed.value, str(e))
-                finally:
-                    logger.info("")
 
                 try:
                     self.validate_result_format(result)
 
                     if result["type"] == "download":
                         self.upload_file_to_s3(result)
```

