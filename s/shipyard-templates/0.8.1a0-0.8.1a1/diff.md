# Comparing `tmp/shipyard_templates-0.8.1a0.tar.gz` & `tmp/shipyard_templates-0.8.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_templates-0.8.1a0.tar", max compression
+gzip compressed data, was "shipyard_templates-0.8.1a1.tar", max compression
```

## Comparing `shipyard_templates-0.8.1a0.tar` & `shipyard_templates-0.8.1a1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0        0 2023-04-18 15:33:24.335210 shipyard_templates-0.8.1a0/README.md
--rw-r--r--   0        0        0      345 2024-04-03 02:10:22.190810 shipyard_templates-0.8.1a0/pyproject.toml
--rw-r--r--   0        0        0      481 2023-12-11 17:36:50.275333 shipyard_templates-0.8.1a0/shipyard_templates/__init__.py
--rw-r--r--   0        0        0      712 2024-04-01 19:04:10.708265 shipyard_templates-0.8.1a0/shipyard_templates/cloudstorage.py
--rw-r--r--   0        0        0      920 2024-03-08 19:26:38.901723 shipyard_templates-0.8.1a0/shipyard_templates/crm.py
--rw-r--r--   0        0        0     4161 2024-04-02 01:11:21.831332 shipyard_templates-0.8.1a0/shipyard_templates/database.py
--rw-r--r--   0        0        0      346 2024-03-08 19:26:38.902243 shipyard_templates-0.8.1a0/shipyard_templates/datavisualization.py
--rw-r--r--   0        0        0     1638 2024-04-03 02:57:58.717413 shipyard_templates-0.8.1a0/shipyard_templates/etl.py
--rw-r--r--   0        0        0      598 2023-10-07 02:13:54.047594 shipyard_templates-0.8.1a0/shipyard_templates/exit_code_exception.py
--rw-r--r--   0        0        0     2648 2024-03-08 19:26:38.902682 shipyard_templates-0.8.1a0/shipyard_templates/messaging.py
--rw-r--r--   0        0        0      116 2024-03-08 19:26:38.903017 shipyard_templates-0.8.1a0/shipyard_templates/notebooks.py
--rw-r--r--   0        0        0      937 2024-04-01 19:04:10.709746 shipyard_templates-0.8.1a0/shipyard_templates/projectmanagement.py
--rw-r--r--   0        0        0     1881 2024-03-08 19:26:38.903738 shipyard_templates-0.8.1a0/shipyard_templates/shipyard_logger.py
--rw-r--r--   0        0        0      575 2024-03-08 19:26:38.904013 shipyard_templates-0.8.1a0/shipyard_templates/spreadsheets.py
--rw-r--r--   0        0        0      511 1970-01-01 00:00:00.000000 shipyard_templates-0.8.1a0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-18 15:33:24.335210 shipyard_templates-0.8.1a1/README.md
+-rw-r--r--   0        0        0      345 2024-04-03 14:32:34.425677 shipyard_templates-0.8.1a1/pyproject.toml
+-rw-r--r--   0        0        0      481 2023-12-11 17:36:50.275333 shipyard_templates-0.8.1a1/shipyard_templates/__init__.py
+-rw-r--r--   0        0        0      712 2024-04-01 19:04:10.708265 shipyard_templates-0.8.1a1/shipyard_templates/cloudstorage.py
+-rw-r--r--   0        0        0      920 2024-03-08 19:26:38.901723 shipyard_templates-0.8.1a1/shipyard_templates/crm.py
+-rw-r--r--   0        0        0     4161 2024-04-02 01:11:21.831332 shipyard_templates-0.8.1a1/shipyard_templates/database.py
+-rw-r--r--   0        0        0      346 2024-03-08 19:26:38.902243 shipyard_templates-0.8.1a1/shipyard_templates/datavisualization.py
+-rw-r--r--   0        0        0     1646 2024-04-03 14:27:32.037649 shipyard_templates-0.8.1a1/shipyard_templates/etl.py
+-rw-r--r--   0        0        0      598 2023-10-07 02:13:54.047594 shipyard_templates-0.8.1a1/shipyard_templates/exit_code_exception.py
+-rw-r--r--   0        0        0     2648 2024-03-08 19:26:38.902682 shipyard_templates-0.8.1a1/shipyard_templates/messaging.py
+-rw-r--r--   0        0        0      116 2024-03-08 19:26:38.903017 shipyard_templates-0.8.1a1/shipyard_templates/notebooks.py
+-rw-r--r--   0        0        0      937 2024-04-01 19:04:10.709746 shipyard_templates-0.8.1a1/shipyard_templates/projectmanagement.py
+-rw-r--r--   0        0        0     1881 2024-03-08 19:26:38.903738 shipyard_templates-0.8.1a1/shipyard_templates/shipyard_logger.py
+-rw-r--r--   0        0        0      575 2024-03-08 19:26:38.904013 shipyard_templates-0.8.1a1/shipyard_templates/spreadsheets.py
+-rw-r--r--   0        0        0      511 1970-01-01 00:00:00.000000 shipyard_templates-0.8.1a1/PKG-INFO
```

### Comparing `shipyard_templates-0.8.1a0/shipyard_templates/cloudstorage.py` & `shipyard_templates-0.8.1a1/shipyard_templates/cloudstorage.py`

 * *Files identical despite different names*

### Comparing `shipyard_templates-0.8.1a0/shipyard_templates/crm.py` & `shipyard_templates-0.8.1a1/shipyard_templates/crm.py`

 * *Files identical despite different names*

### Comparing `shipyard_templates-0.8.1a0/shipyard_templates/database.py` & `shipyard_templates-0.8.1a1/shipyard_templates/database.py`

 * *Files identical despite different names*

### Comparing `shipyard_templates-0.8.1a0/shipyard_templates/etl.py` & `shipyard_templates-0.8.1a1/shipyard_templates/etl.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from abc import ABC, abstractmethod
 from .exit_code_exception import ExitCodeException
 
 
 class UnauthorizedError(ExitCodeException):
     def __init__(self, message: str):
-        self.message = f"Failed to connect to the API. Ensure that the API key provided is correct. Message from the API: {message}"
+        self.message = f"Failed to connect to the API. Ensure that the credential item provided is correct. Message from the API: {message}"
         self.exit_code = Etl.EXIT_CODE_INVALID_CREDENTIALS
 
 
 class BadRequestError(ExitCodeException):
     def __init__(self, message: str):
         self.message = f"The request is malformed. Message from the API: {message}"
         self.exit_code = Etl.EXIT_CODE_BAD_REQUEST
```

### Comparing `shipyard_templates-0.8.1a0/shipyard_templates/exit_code_exception.py` & `shipyard_templates-0.8.1a1/shipyard_templates/exit_code_exception.py`

 * *Files identical despite different names*

### Comparing `shipyard_templates-0.8.1a0/shipyard_templates/messaging.py` & `shipyard_templates-0.8.1a1/shipyard_templates/messaging.py`

 * *Files identical despite different names*

### Comparing `shipyard_templates-0.8.1a0/shipyard_templates/projectmanagement.py` & `shipyard_templates-0.8.1a1/shipyard_templates/projectmanagement.py`

 * *Files identical despite different names*

### Comparing `shipyard_templates-0.8.1a0/shipyard_templates/shipyard_logger.py` & `shipyard_templates-0.8.1a1/shipyard_templates/shipyard_logger.py`

 * *Files identical despite different names*

### Comparing `shipyard_templates-0.8.1a0/shipyard_templates/spreadsheets.py` & `shipyard_templates-0.8.1a1/shipyard_templates/spreadsheets.py`

 * *Files identical despite different names*

