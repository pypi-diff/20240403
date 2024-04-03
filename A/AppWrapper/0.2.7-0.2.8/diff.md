# Comparing `tmp/AppWrapper-0.2.7.tar.gz` & `tmp/AppWrapper-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AppWrapper-0.2.7.tar", last modified: Wed Apr  3 04:28:01 2024, max compression
+gzip compressed data, was "AppWrapper-0.2.8.tar", last modified: Wed Apr  3 04:45:00 2024, max compression
```

## Comparing `AppWrapper-0.2.7.tar` & `AppWrapper-0.2.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:28:01.803623 AppWrapper-0.2.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:28:01.803623 AppWrapper-0.2.7/AppWrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-03 04:28:01.000000 AppWrapper-0.2.7/AppWrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-03 04:28:01.000000 AppWrapper-0.2.7/AppWrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 04:28:01.000000 AppWrapper-0.2.7/AppWrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-03 04:28:01.000000 AppWrapper-0.2.7/AppWrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-03 04:28:01.000000 AppWrapper-0.2.7/AppWrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-03 04:28:01.803623 AppWrapper-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 04:27:50.000000 AppWrapper-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:28:01.803623 AppWrapper-0.2.7/app_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-03 04:27:50.000000 AppWrapper-0.2.7/app_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10083 2024-04-03 04:27:50.000000 AppWrapper-0.2.7/app_wrapper/app_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-03 04:27:50.000000 AppWrapper-0.2.7/app_wrapper/task_status.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 04:28:01.803623 AppWrapper-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-03 04:27:50.000000 AppWrapper-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:45:00.927497 AppWrapper-0.2.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:45:00.927497 AppWrapper-0.2.8/AppWrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-03 04:45:00.000000 AppWrapper-0.2.8/AppWrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-03 04:45:00.000000 AppWrapper-0.2.8/AppWrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 04:45:00.000000 AppWrapper-0.2.8/AppWrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-03 04:45:00.000000 AppWrapper-0.2.8/AppWrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-03 04:45:00.000000 AppWrapper-0.2.8/AppWrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-03 04:45:00.927497 AppWrapper-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 04:44:27.000000 AppWrapper-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:45:00.927497 AppWrapper-0.2.8/app_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-03 04:44:27.000000 AppWrapper-0.2.8/app_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10095 2024-04-03 04:44:27.000000 AppWrapper-0.2.8/app_wrapper/app_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-03 04:44:27.000000 AppWrapper-0.2.8/app_wrapper/task_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 04:45:00.927497 AppWrapper-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-03 04:44:27.000000 AppWrapper-0.2.8/setup.py
```

### Comparing `AppWrapper-0.2.7/app_wrapper/app_wrapper.py` & `AppWrapper-0.2.8/app_wrapper/app_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import pathlib
 
 import requests
 import boto3
 import logging
 import traceback
 
-from task_status import Status
+from app_wrapper.task_status import Status
 
 logger = logging.getLogger("app_wrapper")
 logger.setLevel(logging.INFO)
 
 # Create console handler and set level to debug
 ch = logging.StreamHandler()
 ch.setLevel(logging.INFO)
```

