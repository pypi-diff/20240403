# Comparing `tmp/shipyard_templates-0.8.0a2.tar.gz` & `tmp/shipyard_templates-0.8.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_templates-0.8.0a2.tar", max compression
+gzip compressed data, was "shipyard_templates-0.8.1a0.tar", max compression
```

## Comparing `shipyard_templates-0.8.0a2.tar` & `shipyard_templates-0.8.1a0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0        0 2023-04-18 15:33:24.335210 shipyard_templates-0.8.0a2/README.md
--rw-r--r--   0        0        0      345 2024-03-21 21:57:25.909838 shipyard_templates-0.8.0a2/pyproject.toml
--rw-r--r--   0        0        0      481 2023-12-11 17:36:50.275333 shipyard_templates-0.8.0a2/shipyard_templates/__init__.py
--rw-r--r--   0        0        0      712 2024-03-18 18:43:57.589216 shipyard_templates-0.8.0a2/shipyard_templates/cloudstorage.py
--rw-r--r--   0        0        0      920 2024-03-08 19:26:38.901723 shipyard_templates-0.8.0a2/shipyard_templates/crm.py
--rw-r--r--   0        0        0     4160 2024-03-21 21:58:48.131038 shipyard_templates-0.8.0a2/shipyard_templates/database.py
--rw-r--r--   0        0        0      346 2024-03-08 19:26:38.902243 shipyard_templates-0.8.0a2/shipyard_templates/datavisualization.py
--rw-r--r--   0        0        0     1094 2024-03-18 18:43:57.589761 shipyard_templates-0.8.0a2/shipyard_templates/etl.py
--rw-r--r--   0        0        0      598 2023-10-07 02:13:54.047594 shipyard_templates-0.8.0a2/shipyard_templates/exit_code_exception.py
--rw-r--r--   0        0        0     2648 2024-03-08 19:26:38.902682 shipyard_templates-0.8.0a2/shipyard_templates/messaging.py
--rw-r--r--   0        0        0      116 2024-03-08 19:26:38.903017 shipyard_templates-0.8.0a2/shipyard_templates/notebooks.py
--rw-r--r--   0        0        0      937 2024-03-18 18:43:57.590773 shipyard_templates-0.8.0a2/shipyard_templates/projectmanagement.py
--rw-r--r--   0        0        0     1881 2024-03-08 19:26:38.903738 shipyard_templates-0.8.0a2/shipyard_templates/shipyard_logger.py
--rw-r--r--   0        0        0      575 2024-03-08 19:26:38.904013 shipyard_templates-0.8.0a2/shipyard_templates/spreadsheets.py
--rw-r--r--   0        0        0      511 1970-01-01 00:00:00.000000 shipyard_templates-0.8.0a2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-18 15:33:24.335210 shipyard_templates-0.8.1a0/README.md
+-rw-r--r--   0        0        0      345 2024-04-03 02:10:22.190810 shipyard_templates-0.8.1a0/pyproject.toml
+-rw-r--r--   0        0        0      481 2023-12-11 17:36:50.275333 shipyard_templates-0.8.1a0/shipyard_templates/__init__.py
+-rw-r--r--   0        0        0      712 2024-04-01 19:04:10.708265 shipyard_templates-0.8.1a0/shipyard_templates/cloudstorage.py
+-rw-r--r--   0        0        0      920 2024-03-08 19:26:38.901723 shipyard_templates-0.8.1a0/shipyard_templates/crm.py
+-rw-r--r--   0        0        0     4161 2024-04-02 01:11:21.831332 shipyard_templates-0.8.1a0/shipyard_templates/database.py
+-rw-r--r--   0        0        0      346 2024-03-08 19:26:38.902243 shipyard_templates-0.8.1a0/shipyard_templates/datavisualization.py
+-rw-r--r--   0        0        0     1638 2024-04-03 02:57:58.717413 shipyard_templates-0.8.1a0/shipyard_templates/etl.py
+-rw-r--r--   0        0        0      598 2023-10-07 02:13:54.047594 shipyard_templates-0.8.1a0/shipyard_templates/exit_code_exception.py
+-rw-r--r--   0        0        0     2648 2024-03-08 19:26:38.902682 shipyard_templates-0.8.1a0/shipyard_templates/messaging.py
+-rw-r--r--   0        0        0      116 2024-03-08 19:26:38.903017 shipyard_templates-0.8.1a0/shipyard_templates/notebooks.py
+-rw-r--r--   0        0        0      937 2024-04-01 19:04:10.709746 shipyard_templates-0.8.1a0/shipyard_templates/projectmanagement.py
+-rw-r--r--   0        0        0     1881 2024-03-08 19:26:38.903738 shipyard_templates-0.8.1a0/shipyard_templates/shipyard_logger.py
+-rw-r--r--   0        0        0      575 2024-03-08 19:26:38.904013 shipyard_templates-0.8.1a0/shipyard_templates/spreadsheets.py
+-rw-r--r--   0        0        0      511 1970-01-01 00:00:00.000000 shipyard_templates-0.8.1a0/PKG-INFO
```

### Comparing `shipyard_templates-0.8.0a2/shipyard_templates/cloudstorage.py` & `shipyard_templates-0.8.1a0/shipyard_templates/cloudstorage.py`

 * *Files identical despite different names*

### Comparing `shipyard_templates-0.8.0a2/shipyard_templates/crm.py` & `shipyard_templates-0.8.1a0/shipyard_templates/crm.py`

 * *Files identical despite different names*

### Comparing `shipyard_templates-0.8.0a2/shipyard_templates/database.py` & `shipyard_templates-0.8.1a0/shipyard_templates/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,17 +23,18 @@
 class QueryError(ExitCodeException):
     def __init__(self, error_msg: Exception):
         self.message = (
             f"Error in executing query. Message from the server is: {error_msg}"
         )
         self.exit_code = Database.EXIT_CODE_QUERY_ERROR
 
+
 class ConnectionError(ExitCodeException):
-    def __init__(self, message:str):
-        self.message = message 
+    def __init__(self, message: str):
+        self.message = message
         self.exit_code = Database.EXIT_CODE_INVALID_CREDENTIALS
 
 
 class Database(ABC):
     EXIT_CODE_INVALID_CREDENTIALS = 200
     EXIT_CODE_INVALID_ACCOUNT = 201  # snowflake specific
     EXIT_CODE_INVALID_WAREHOUSE = 202
```

### Comparing `shipyard_templates-0.8.0a2/shipyard_templates/etl.py` & `shipyard_templates-0.8.1a0/shipyard_templates/projectmanagement.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 from abc import ABC, abstractmethod
 
 
-class Etl(ABC):
+class ExitCodeError(Exception):
+    def __init__(self, message, exit_code):
+        super().__init__(message)
+        self.message = message
+        self.exit_code = exit_code
+
+
+class ProjectManagement(ABC):
     # Class level exit codes
     # general exit codes
-    EXIT_CODE_FINAL_STATUS_COMPLETED = 0
     EXIT_CODE_INVALID_CREDENTIALS = 200
     EXIT_CODE_BAD_REQUEST = 201
-    EXIT_CODE_INVALID_INPUT = 206
-    # trigger sync exit codes
-    EXIT_CODE_SYNC_REFRESH_ERROR = 202
-    EXIT_CODE_SYNC_ALREADY_RUNNING = 203
-    EXIT_CODE_SYNC_INVALID_SOURCE_ID = 204
-    EXIT_CODE_SYNC_INVALID_POKE_INTERVAL = 205
-    EXIT_CODE_SYNC_CHECK_ERROR = 220
-    # verify status exit codes
-    EXIT_CODE_FINAL_STATUS_INCOMPLETE = 210
-    EXIT_CODE_FINAL_STATUS_ERRORED = 211
-    EXIT_CODE_FINAL_STATUS_INVALID = 212
-    EXIT_CODE_FINAL_STATUS_CANCELLED = 213
-    EXIT_CODE_FINAL_STATUS_PENDING = 214
-    EXIT_CODE_UNKNOWN_STATUS = 215
+    EXIT_CODE_TICKET_NOT_FOUND = 202
+    EXIT_CODE_INVALID_ISSUE_TYPE = 203
+    EXIT_CODE_INVALID_STATUS = 204
+    EXIT_CODE_INVALID_INPUT = 205
     EXIT_CODE_UNKNOWN_ERROR = 299
 
-    # API TIMEOUT
-    TIMEOUT = 30
-
     def __init__(self, access_token: str, **kwargs) -> None:
         self.access_token = access_token
 
     @abstractmethod
-    def trigger_sync(self, **kwargs):
+    def create_ticket(self, **kwargs):
+        pass
+
+    @abstractmethod
+    def get_ticket(self, **kwargs):
+        pass
+
+    @abstractmethod
+    def update_ticket(self, **kwargs):
         pass
 
     @abstractmethod
-    def determine_sync_status(self, **kwargs):
+    def connect(self, **kwargs):
         pass
```

### Comparing `shipyard_templates-0.8.0a2/shipyard_templates/exit_code_exception.py` & `shipyard_templates-0.8.1a0/shipyard_templates/exit_code_exception.py`

 * *Files identical despite different names*

### Comparing `shipyard_templates-0.8.0a2/shipyard_templates/messaging.py` & `shipyard_templates-0.8.1a0/shipyard_templates/messaging.py`

 * *Files identical despite different names*

### Comparing `shipyard_templates-0.8.0a2/shipyard_templates/shipyard_logger.py` & `shipyard_templates-0.8.1a0/shipyard_templates/shipyard_logger.py`

 * *Files identical despite different names*

### Comparing `shipyard_templates-0.8.0a2/shipyard_templates/spreadsheets.py` & `shipyard_templates-0.8.1a0/shipyard_templates/spreadsheets.py`

 * *Files identical despite different names*

