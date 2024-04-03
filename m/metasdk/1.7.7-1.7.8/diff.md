# Comparing `tmp/metasdk-1.7.7.tar.gz` & `tmp/metasdk-1.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metasdk-1.7.7.tar", last modified: Mon Apr  1 15:10:02 2024, max compression
+gzip compressed data, was "metasdk-1.7.8.tar", last modified: Wed Apr  3 11:34:54 2024, max compression
```

## Comparing `metasdk-1.7.7.tar` & `metasdk-1.7.8.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-04-01 15:10:02.145038 metasdk-1.7.7/
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1074 2022-08-11 12:23:20.000000 metasdk-1.7.7/LICENSE
--rw-rw-r--   0 zhas      (1000) zhas      (1000)        0 2022-08-11 12:23:20.000000 metasdk-1.7.7/MANIFEST.in
--rw-r--r--   0 zhas      (1000) zhas      (1000)     2830 2024-04-01 15:10:02.145038 metasdk-1.7.7/PKG-INFO
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     2236 2024-02-12 19:35:51.000000 metasdk-1.7.7/README.md
-drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-04-01 15:10:02.145038 metasdk-1.7.7/metasdk/
--rw-rw-r--   0 zhas      (1000) zhas      (1000)    16426 2024-02-12 19:35:51.000000 metasdk-1.7.7/metasdk/__init__.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)      190 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/__state.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     3803 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/apiclient.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     6152 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/event_bus.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     3523 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/exceptions.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)      102 2024-04-01 14:33:24.000000 metasdk-1.7.7/metasdk/info.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1815 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/internal.py
-drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-04-01 15:10:02.145038 metasdk-1.7.7/metasdk/logger/
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     6374 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/logger/__init__.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1862 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/logger/bulk_logger.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     3478 2024-01-25 19:39:16.000000 metasdk-1.7.7/metasdk/logger/logger.py
-drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-04-01 15:10:02.145038 metasdk-1.7.7/metasdk/services/
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     8667 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/services/ApiProxyService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     5098 2024-04-01 14:33:24.000000 metasdk-1.7.7/metasdk/services/AuthService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)      634 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/services/CacheService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     5086 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/services/DbQueryService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     2924 2024-01-25 19:39:16.000000 metasdk-1.7.7/metasdk/services/DbService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1355 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/services/DevService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1066 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/services/ExportService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     2563 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/services/ExternalSystemService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)    18707 2024-04-01 15:06:59.000000 metasdk-1.7.7/metasdk/services/FeedService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1939 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/services/IssueService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     5823 2024-01-25 19:39:16.000000 metasdk-1.7.7/metasdk/services/LockService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1394 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/services/MailService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1936 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/services/MediaService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1362 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/services/MetaqlService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)      968 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/services/ObjectLogService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     2554 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/services/SettingsService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     8731 2023-12-07 09:05:36.000000 metasdk-1.7.7/metasdk/services/StarterService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)      691 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/services/UserManagementService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1157 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/services/__init__.py
-drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-04-01 15:10:02.145038 metasdk-1.7.7/metasdk/tools/
--rw-rw-r--   0 zhas      (1000) zhas      (1000)        0 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/tools/__init__.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1079 2024-01-25 19:39:16.000000 metasdk-1.7.7/metasdk/tools/extract_event_handlers.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     2252 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/utils.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     2051 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/worker.py
-drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-04-01 15:10:02.145038 metasdk-1.7.7/metasdk.egg-info/
--rw-r--r--   0 zhas      (1000) zhas      (1000)     2830 2024-04-01 15:10:02.000000 metasdk-1.7.7/metasdk.egg-info/PKG-INFO
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1172 2024-04-01 15:10:02.000000 metasdk-1.7.7/metasdk.egg-info/SOURCES.txt
--rw-rw-r--   0 zhas      (1000) zhas      (1000)        1 2024-04-01 15:10:02.000000 metasdk-1.7.7/metasdk.egg-info/dependency_links.txt
--rw-rw-r--   0 zhas      (1000) zhas      (1000)      172 2024-04-01 15:10:02.000000 metasdk-1.7.7/metasdk.egg-info/requires.txt
--rw-rw-r--   0 zhas      (1000) zhas      (1000)        8 2024-04-01 15:10:02.000000 metasdk-1.7.7/metasdk.egg-info/top_level.txt
--rw-rw-r--   0 zhas      (1000) zhas      (1000)      205 2024-04-01 15:10:02.145038 metasdk-1.7.7/setup.cfg
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1193 2022-08-11 12:23:20.000000 metasdk-1.7.7/setup.py
+drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-04-03 11:34:54.063845 metasdk-1.7.8/
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1074 2022-08-11 12:23:20.000000 metasdk-1.7.8/LICENSE
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)        0 2022-08-11 12:23:20.000000 metasdk-1.7.8/MANIFEST.in
+-rw-r--r--   0 zhas      (1000) zhas      (1000)     2830 2024-04-03 11:34:54.063845 metasdk-1.7.8/PKG-INFO
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     2236 2024-02-12 19:35:51.000000 metasdk-1.7.8/README.md
+drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-04-03 11:34:54.055845 metasdk-1.7.8/metasdk/
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)    16426 2024-02-12 19:35:51.000000 metasdk-1.7.8/metasdk/__init__.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)      190 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/__state.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     3803 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/apiclient.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     6152 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/event_bus.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     3523 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/exceptions.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)      102 2024-04-03 11:33:07.000000 metasdk-1.7.8/metasdk/info.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1815 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/internal.py
+drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-04-03 11:34:54.059845 metasdk-1.7.8/metasdk/logger/
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     6374 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/logger/__init__.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1862 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/logger/bulk_logger.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     3478 2024-01-25 19:39:16.000000 metasdk-1.7.8/metasdk/logger/logger.py
+drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-04-03 11:34:54.063845 metasdk-1.7.8/metasdk/services/
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     8667 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/services/ApiProxyService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     5098 2024-04-01 14:33:24.000000 metasdk-1.7.8/metasdk/services/AuthService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)      634 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/services/CacheService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     5086 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/services/DbQueryService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     2924 2024-01-25 19:39:16.000000 metasdk-1.7.8/metasdk/services/DbService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1355 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/services/DevService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1066 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/services/ExportService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     2563 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/services/ExternalSystemService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)    21782 2024-04-03 11:33:07.000000 metasdk-1.7.8/metasdk/services/FeedService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1939 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/services/IssueService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     5823 2024-01-25 19:39:16.000000 metasdk-1.7.8/metasdk/services/LockService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1394 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/services/MailService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1936 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/services/MediaService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1362 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/services/MetaqlService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)      968 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/services/ObjectLogService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     2554 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/services/SettingsService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     8731 2023-12-07 09:05:36.000000 metasdk-1.7.8/metasdk/services/StarterService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)      691 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/services/UserManagementService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1157 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/services/__init__.py
+drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-04-03 11:34:54.063845 metasdk-1.7.8/metasdk/tools/
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)        0 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/tools/__init__.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1079 2024-01-25 19:39:16.000000 metasdk-1.7.8/metasdk/tools/extract_event_handlers.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     2252 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/utils.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     2051 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/worker.py
+drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-04-03 11:34:54.059845 metasdk-1.7.8/metasdk.egg-info/
+-rw-r--r--   0 zhas      (1000) zhas      (1000)     2830 2024-04-03 11:34:54.000000 metasdk-1.7.8/metasdk.egg-info/PKG-INFO
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1172 2024-04-03 11:34:54.000000 metasdk-1.7.8/metasdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)        1 2024-04-03 11:34:54.000000 metasdk-1.7.8/metasdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)      172 2024-04-03 11:34:54.000000 metasdk-1.7.8/metasdk.egg-info/requires.txt
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)        8 2024-04-03 11:34:54.000000 metasdk-1.7.8/metasdk.egg-info/top_level.txt
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)      205 2024-04-03 11:34:54.063845 metasdk-1.7.8/setup.cfg
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1193 2022-08-11 12:23:20.000000 metasdk-1.7.8/setup.py
```

### Comparing `metasdk-1.7.7/LICENSE` & `metasdk-1.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.7/PKG-INFO` & `metasdk-1.7.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metasdk
-Version: 1.7.7
+Version: 1.7.8
 Summary: Devision Meta SDK
 Home-page: https://github.com/devision-io/metasdk
 Author: Artur Geraschenko
 Author-email: arturgspb@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
```

### Comparing `metasdk-1.7.7/README.md` & `metasdk-1.7.8/README.md`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.7/metasdk/__init__.py` & `metasdk-1.7.8/metasdk/__init__.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.7/metasdk/apiclient.py` & `metasdk-1.7.8/metasdk/apiclient.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.7/metasdk/event_bus.py` & `metasdk-1.7.8/metasdk/event_bus.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.7/metasdk/exceptions.py` & `metasdk-1.7.8/metasdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.7/metasdk/internal.py` & `metasdk-1.7.8/metasdk/internal.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.7/metasdk/logger/__init__.py` & `metasdk-1.7.8/metasdk/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.7/metasdk/logger/bulk_logger.py` & `metasdk-1.7.8/metasdk/logger/bulk_logger.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.7/metasdk/logger/logger.py` & `metasdk-1.7.8/metasdk/logger/logger.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.7/metasdk/services/ApiProxyService.py` & `metasdk-1.7.8/metasdk/services/ApiProxyService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.7/metasdk/services/AuthService.py` & `metasdk-1.7.8/metasdk/services/AuthService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.7/metasdk/services/CacheService.py` & `metasdk-1.7.8/metasdk/services/CacheService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.7/metasdk/services/DbQueryService.py` & `metasdk-1.7.8/metasdk/services/DbQueryService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.7/metasdk/services/DbService.py` & `metasdk-1.7.8/metasdk/services/DbService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.7/metasdk/services/DevService.py` & `metasdk-1.7.8/metasdk/services/DevService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.7/metasdk/services/ExportService.py` & `metasdk-1.7.8/metasdk/services/ExportService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.7/metasdk/services/ExternalSystemService.py` & `metasdk-1.7.8/metasdk/services/ExternalSystemService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.7/metasdk/services/FeedService.py` & `metasdk-1.7.8/metasdk/services/FeedService.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,14 +19,16 @@
     @functools.wraps(func)
     def wrapper(self, *args, **kwargs):
         user_info = self.auth_service.verify_access_token(self.token, self.required_scopes)
         self.auth_user_info = user_info
 
         if kwargs.get("feed_id"):
             self.check_feed_permissions(feed_id=kwargs["feed_id"], auth_user_info=user_info)
+        if kwargs.get("task_id"):
+            self.check_task_permissions(task_id=kwargs["task_id"], auth_user_info=user_info)
         return func(self, *args, **kwargs)
     return wrapper
 
 
 class FeedService:
     def __init__(self, app, token: str = ""):
         """
@@ -44,17 +46,21 @@
         self.required_scopes = ["datahub"]
         self.auth_user_info = None
 
     def check_feed_permissions(self, feed_id: str, auth_user_info: AuthUserInfo) -> bool:
         """
         Проверяет права доступа к фиду.
 
+        Если пользователь админ, то проверяется принадлежность фида к его компании.
+        Если без прав админа, то пользователб должен быть автором фида.
+
+        Если feed_id не существует, также вызываем исключение ForbiddenError.
         :param feed_id: ID фида.
         :param auth_user_info: данные о пользователе, предоставившем валидный токен.
-        :return: True, если есть доступ к фиду, иначе - исключение PermissionError.
+        :return: True, если есть доступ к фиду, иначе - исключение ForbiddenError.
         """
         company_id = auth_user_info["company_id"]
         author_user_id = auth_user_info["auth_user_id"]
         query_params = {"feed_id": feed_id, "company_id": company_id, "author_user_id": author_user_id}
 
         base_query = """
         SELECT
@@ -70,14 +76,31 @@
 
         result = self.__metadb.one(query, query_params)
         if result and result["feed_id"]:
             return True
         else:
             raise ForbiddenError("Do not have permissions to access this feed")
 
+    def check_task_permissions(self, task_id: str, auth_user_info: AuthUserInfo) -> bool:
+        """
+        Проверяет права доступа к таску.
+
+        Таск запускается в рамках фида, поэтому проверяем права доступа к фиду.
+        :param task_id: ID таска.
+        :param auth_user_info: данные о пользователе, предоставившем валидный токен.
+        :return: True, если есть доступ к фиду, иначе - исключение ForbiddenError.
+        """
+        query = "SELECT data ->> 'ds_id' AS feed_id FROM job.task WHERE id = :task_id::uuid"
+        result = self.__metadb.one(query, params={"task_id": task_id})
+        if result:
+            feed_id = result["feed_id"]
+            return self.check_feed_permissions(feed_id, auth_user_info)
+        else:
+            raise ForbiddenError("Do not have permissions to access this feed")
+
     def get_feed(self, datasource_id: str):
         """
         Получение настроек для фида
         :param datasource_id: идентификатор фида
         :return: FeedDataSource
         """
         info = self.__metadb.one(
@@ -336,30 +359,30 @@
         ), agg_tasks AS (
             SELECT array_agg(id) AS last_tasks, ds_id FROM last_tasks GROUP BY ds_id
         )
         """
         return sqlparse.format(base_query, reindent=True)
 
     @auth_required
-    def get_tasks(self, feed_id: str) -> list[dict]:
+    def list_tasks(self, feed_id: str) -> list[dict]:
         """
         Получает список тасков фида.
 
         :param feed_id: ID фида.
         :param token: токен авторизации.
         :return: данные о таске. '{id: status}'
         """
         if not feed_id:
             raise ValueError("'feed_id' обязательный параметр")
 
         query_params = {"feed_id": feed_id}
-        query = self._generate_tasks_query()
+        query = self._generate_list_tasks_query()
         return self.__metadb.all(query, query_params)
 
-    def _generate_tasks_query(self) -> str:
+    def _generate_list_tasks_query(self) -> str:
         """
         Генерирует SQL запрос для получения списка фидов.
 
         Таблица 'job.task' переодически очищается, поэтому там будут таски только за последние несколько дней.
         Фильтрация по 'service_id' ускоряет запрос.
         :param is_admin: флаг админа компании.
         :return: SQL запрос для получения списка тасков фида.
@@ -370,20 +393,55 @@
         LEFT JOIN meta.feed_datasource fd ON (ta.data ->> 'ds_id')::uuid = fd.id
         LEFT JOIN public.users us ON fd.author_user_id =us.id 
         WHERE service_id = 'meta.datasource_share' AND data->>'ds_id' = :feed_id::text
         """
         return sqlparse.format(base_query, reindent=True)
 
     @auth_required
+    def get_task(self, task_id: str) -> dict:
+        """
+        Получает данные о таске.
+
+        :param task_id: ID таска.
+        :return: данные о таске.
+        """
+        query = self._generate_get_task_query()
+        return self.__metadb.one(query, params={"task_id": task_id})
+
+    def _generate_get_task_query(self) -> str:
+        """
+        Генерирует запрос для получения данных о таске.
+
+        :return: строку с SQL-запросом.
+        """
+        query = """
+        SELECT
+            id as task_id,
+            status,
+            origin,
+            start_time,
+            end_time,
+            creation_time,
+            last_error,
+            data
+        FROM job.task 
+        WHERE service_id = 'meta.datasource_share' AND id = :task_id::uuid;
+        """
+        return sqlparse.format(query, reindent=True)
+
+    @auth_required
     def update_feed(self, feed_id: str, update_values: dict) -> dict:
         """
         Обновляет данные о фиде.
 
         Для обновления доступны колонки ["name", "user_status", "tags"].
         Для обновления tags нужно передать строку вида "tag1, tag2, tag3".
+
+        Существование feed_id проверяется до выполнения этой функции.
+        Поэтому если SQL-запрос ничего не вернул, то значит фид является автоматическим и его нельзя обновлять.
         :param feed_id: ID фида.
         :param update_values: данные для обвноления в формате {col_name: value}
         :return: результаты выполнения запроса от Meta API.
         """
         allowed_cols = ["name", "user_status", "tags"]
 
         allowed_updates = {}
@@ -396,15 +454,18 @@
                 raise BadParametersError(f"Column '{col_name}' is not allowed for update")
 
         if allowed_updates.get("tags"):
             allowed_updates["tags"] = f"{{{allowed_updates['tags']}}}"  # получится строка вида '{tag1, tag2}'
 
         query_params = {"feed_id": feed_id, **allowed_updates}
         query = self._generate_update_feed_query(allowed_update_col_names)
-        return self.__metadb.update(query, query_params)
+        result = self.__metadb.one(query, query_params)
+        if not result:
+            raise BadParametersError("The feed was created automatically and cannot be modified")
+        return result
 
     def _generate_update_feed_query(self, col_names: list[str]) -> str:
         """
         Формирует SQL запрс для обновления данных фида.
 
         :param col_names: список колонок для обновления.
         :return: строка SQL запроса.
@@ -418,15 +479,16 @@
             if special_types.get(col_name):
                 col_upd_expr = f"{col_name} = :{col_name}::{special_types[col_name]}"
             else:
                 col_upd_expr = f"{col_name} = :{col_name}"
             col_updates.append(col_upd_expr)
         col_updates_expr = ", ".join(col_updates)
 
-        query = f"UPDATE meta.feed_datasource SET {col_updates_expr} WHERE id = :feed_id::uuid"
+        returning_sql = "RETURNING id, name, user_status, state, last_launch_time, is_automated, tags;"
+        query = f"UPDATE meta.feed_datasource SET {col_updates_expr} WHERE id = :feed_id::uuid AND is_automated = false {returning_sql}"
         return sqlparse.format(query, reindent=True)
 
 
 class FeedDataSource:
     """
     Класс хранения данных по коннектору
     """
```

### Comparing `metasdk-1.7.7/metasdk/services/IssueService.py` & `metasdk-1.7.8/metasdk/services/IssueService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.7/metasdk/services/LockService.py` & `metasdk-1.7.8/metasdk/services/LockService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.7/metasdk/services/MailService.py` & `metasdk-1.7.8/metasdk/services/MailService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.7/metasdk/services/MediaService.py` & `metasdk-1.7.8/metasdk/services/MediaService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.7/metasdk/services/MetaqlService.py` & `metasdk-1.7.8/metasdk/services/MetaqlService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.7/metasdk/services/ObjectLogService.py` & `metasdk-1.7.8/metasdk/services/ObjectLogService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.7/metasdk/services/SettingsService.py` & `metasdk-1.7.8/metasdk/services/SettingsService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.7/metasdk/services/StarterService.py` & `metasdk-1.7.8/metasdk/services/StarterService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.7/metasdk/services/UserManagementService.py` & `metasdk-1.7.8/metasdk/services/UserManagementService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.7/metasdk/services/__init__.py` & `metasdk-1.7.8/metasdk/services/__init__.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.7/metasdk/tools/extract_event_handlers.py` & `metasdk-1.7.8/metasdk/tools/extract_event_handlers.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.7/metasdk/utils.py` & `metasdk-1.7.8/metasdk/utils.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.7/metasdk/worker.py` & `metasdk-1.7.8/metasdk/worker.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.7/metasdk.egg-info/PKG-INFO` & `metasdk-1.7.8/metasdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metasdk
-Version: 1.7.7
+Version: 1.7.8
 Summary: Devision Meta SDK
 Home-page: https://github.com/devision-io/metasdk
 Author: Artur Geraschenko
 Author-email: arturgspb@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
```

### Comparing `metasdk-1.7.7/metasdk.egg-info/SOURCES.txt` & `metasdk-1.7.8/metasdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.7/setup.py` & `metasdk-1.7.8/setup.py`

 * *Files identical despite different names*

