# Comparing `tmp/naja-atra-1.0.1.tar.gz` & `tmp/naja-atra-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naja-atra-1.0.1.tar", last modified: Tue Apr  2 11:28:00 2024, max compression
+gzip compressed data, was "naja-atra-1.0.2.tar", last modified: Wed Apr  3 08:02:02 2024, max compression
```

## Comparing `naja-atra-1.0.1.tar` & `naja-atra-1.0.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-04-02 11:28:00.181149 naja-atra-1.0.1/
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     1066 2023-01-29 02:07:01.000000 naja-atra-1.0.1/LICENSE
--rw-r--r--   0 keijack   (1000) keijack   (1000)     3012 2024-04-02 11:28:00.177147 naja-atra-1.0.1/PKG-INFO
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     1031 2024-04-02 02:23:04.000000 naja-atra-1.0.1/README.md
-drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-04-02 11:28:00.161139 naja-atra-1.0.1/naja_atra/
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     1172 2024-04-02 11:09:26.000000 naja-atra-1.0.1/naja_atra/__init__.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     2049 2024-04-02 11:24:10.000000 naja-atra-1.0.1/naja_atra/__main__.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)    28716 2024-04-01 10:12:01.000000 naja-atra-1.0.1/naja_atra/app_conf.py
-drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-04-02 11:28:00.169143 naja-atra-1.0.1/naja_atra/http_servers/
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     1087 2024-03-07 02:15:37.000000 naja-atra-1.0.1/naja_atra/http_servers/__init__.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     3740 2024-03-11 09:12:30.000000 naja-atra-1.0.1/naja_atra/http_servers/coroutine_http_server.py
--rwxrwxr-x   0 keijack   (1000) keijack   (1000)     5587 2024-03-12 01:27:45.000000 naja-atra-1.0.1/naja_atra/http_servers/http_server.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)    17237 2024-03-11 09:43:12.000000 naja-atra-1.0.1/naja_atra/http_servers/routing_server.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     3337 2024-03-11 09:15:29.000000 naja-atra-1.0.1/naja_atra/http_servers/threading_http_server.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)    18383 2024-03-11 09:38:20.000000 naja-atra-1.0.1/naja_atra/models.py
-drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-04-02 11:28:00.173145 naja-atra-1.0.1/naja_atra/request_handlers/
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     1087 2024-03-07 02:12:14.000000 naja-atra-1.0.1/naja_atra/request_handlers/__init__.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)    28102 2024-03-11 09:42:45.000000 naja-atra-1.0.1/naja_atra/request_handlers/http_controller_handler.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)    17638 2024-03-11 09:39:40.000000 naja-atra-1.0.1/naja_atra/request_handlers/http_request_handler.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     5914 2024-03-11 09:39:40.000000 naja-atra-1.0.1/naja_atra/request_handlers/http_session_local_impl.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)    14419 2024-03-11 09:39:40.000000 naja-atra-1.0.1/naja_atra/request_handlers/model_bindings.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)    23851 2024-03-11 09:39:40.000000 naja-atra-1.0.1/naja_atra/request_handlers/websocket_controller_handler.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     8848 2024-03-11 09:58:15.000000 naja-atra-1.0.1/naja_atra/server.py
-drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-04-02 11:28:00.173145 naja-atra-1.0.1/naja_atra/utils/
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     1087 2024-03-07 02:23:26.000000 naja-atra-1.0.1/naja_atra/utils/__init__.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     6987 2024-03-11 09:39:40.000000 naja-atra-1.0.1/naja_atra/utils/http_utils.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     6668 2024-03-07 03:33:13.000000 naja-atra-1.0.1/naja_atra/utils/logger.py
-drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-04-02 11:28:00.177147 naja-atra-1.0.1/naja_atra.egg-info/
--rw-r--r--   0 keijack   (1000) keijack   (1000)     3012 2024-04-02 11:28:00.000000 naja-atra-1.0.1/naja_atra.egg-info/PKG-INFO
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     1077 2024-04-02 11:28:00.000000 naja-atra-1.0.1/naja_atra.egg-info/SOURCES.txt
--rw-rw-r--   0 keijack   (1000) keijack   (1000)        1 2024-04-02 11:28:00.000000 naja-atra-1.0.1/naja_atra.egg-info/dependency_links.txt
--rw-rw-r--   0 keijack   (1000) keijack   (1000)       56 2024-04-02 11:28:00.000000 naja-atra-1.0.1/naja_atra.egg-info/requires.txt
--rw-rw-r--   0 keijack   (1000) keijack   (1000)       10 2024-04-02 11:28:00.000000 naja-atra-1.0.1/naja_atra.egg-info/top_level.txt
--rw-rw-r--   0 keijack   (1000) keijack   (1000)      929 2024-03-08 09:12:59.000000 naja-atra-1.0.1/pyproject.toml
--rw-rw-r--   0 keijack   (1000) keijack   (1000)       38 2024-04-02 11:28:00.181149 naja-atra-1.0.1/setup.cfg
--rw-rw-r--   0 keijack   (1000) keijack   (1000)       62 2023-01-29 02:07:01.000000 naja-atra-1.0.1/setup.py
-drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-04-02 11:28:00.177147 naja-atra-1.0.1/tests/
--rw-rw-r--   0 keijack   (1000) keijack   (1000)        0 2023-01-29 02:07:01.000000 naja-atra-1.0.1/tests/__init__.py
-drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-04-02 11:28:00.177147 naja-atra-1.0.1/tests/ctrls/
--rw-rw-r--   0 keijack   (1000) keijack   (1000)        0 2023-01-29 02:07:01.000000 naja-atra-1.0.1/tests/ctrls/__init__.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     9970 2024-03-11 09:19:38.000000 naja-atra-1.0.1/tests/ctrls/my_controllers.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     1890 2024-03-11 08:58:23.000000 naja-atra-1.0.1/tests/ctrls/my_controllers_model_binding.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     3538 2024-03-07 03:14:28.000000 naja-atra-1.0.1/tests/ctrls/ws_controllers.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     8064 2024-03-08 02:52:49.000000 naja-atra-1.0.1/tests/test_all_ctrls.py
+drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-04-03 08:02:02.256513 naja-atra-1.0.2/
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     1066 2023-01-29 02:07:01.000000 naja-atra-1.0.2/LICENSE
+-rw-r--r--   0 keijack   (1000) keijack   (1000)     3012 2024-04-03 08:02:02.256513 naja-atra-1.0.2/PKG-INFO
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     1031 2024-04-02 02:23:04.000000 naja-atra-1.0.2/README.md
+drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-04-03 08:02:02.236513 naja-atra-1.0.2/naja_atra/
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     1172 2024-04-03 08:01:09.000000 naja-atra-1.0.2/naja_atra/__init__.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     2049 2024-04-02 11:35:53.000000 naja-atra-1.0.2/naja_atra/__main__.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)    28716 2024-04-01 10:12:01.000000 naja-atra-1.0.2/naja_atra/app_conf.py
+drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-04-03 08:02:02.240513 naja-atra-1.0.2/naja_atra/http_servers/
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     1087 2024-03-07 02:15:37.000000 naja-atra-1.0.2/naja_atra/http_servers/__init__.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     3740 2024-03-11 09:12:30.000000 naja-atra-1.0.2/naja_atra/http_servers/coroutine_http_server.py
+-rwxrwxr-x   0 keijack   (1000) keijack   (1000)     5587 2024-03-12 01:27:45.000000 naja-atra-1.0.2/naja_atra/http_servers/http_server.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)    17237 2024-03-11 09:43:12.000000 naja-atra-1.0.2/naja_atra/http_servers/routing_server.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     3337 2024-03-11 09:15:29.000000 naja-atra-1.0.2/naja_atra/http_servers/threading_http_server.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)    18383 2024-03-11 09:38:20.000000 naja-atra-1.0.2/naja_atra/models.py
+drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-04-03 08:02:02.244513 naja-atra-1.0.2/naja_atra/request_handlers/
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     1087 2024-03-07 02:12:14.000000 naja-atra-1.0.2/naja_atra/request_handlers/__init__.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)    28102 2024-03-11 09:42:45.000000 naja-atra-1.0.2/naja_atra/request_handlers/http_controller_handler.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)    17638 2024-03-11 09:39:40.000000 naja-atra-1.0.2/naja_atra/request_handlers/http_request_handler.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     5914 2024-03-11 09:39:40.000000 naja-atra-1.0.2/naja_atra/request_handlers/http_session_local_impl.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)    14419 2024-03-11 09:39:40.000000 naja-atra-1.0.2/naja_atra/request_handlers/model_bindings.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)    23851 2024-03-11 09:39:40.000000 naja-atra-1.0.2/naja_atra/request_handlers/websocket_controller_handler.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     8848 2024-03-11 09:58:15.000000 naja-atra-1.0.2/naja_atra/server.py
+drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-04-03 08:02:02.244513 naja-atra-1.0.2/naja_atra/utils/
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     1087 2024-03-07 02:23:26.000000 naja-atra-1.0.2/naja_atra/utils/__init__.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     6987 2024-03-11 09:39:40.000000 naja-atra-1.0.2/naja_atra/utils/http_utils.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     6668 2024-03-07 03:33:13.000000 naja-atra-1.0.2/naja_atra/utils/logger.py
+drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-04-03 08:02:02.256513 naja-atra-1.0.2/naja_atra.egg-info/
+-rw-r--r--   0 keijack   (1000) keijack   (1000)     3012 2024-04-03 08:02:02.000000 naja-atra-1.0.2/naja_atra.egg-info/PKG-INFO
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     1077 2024-04-03 08:02:02.000000 naja-atra-1.0.2/naja_atra.egg-info/SOURCES.txt
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)        1 2024-04-03 08:02:02.000000 naja-atra-1.0.2/naja_atra.egg-info/dependency_links.txt
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)       56 2024-04-03 08:02:02.000000 naja-atra-1.0.2/naja_atra.egg-info/requires.txt
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)       10 2024-04-03 08:02:02.000000 naja-atra-1.0.2/naja_atra.egg-info/top_level.txt
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)      929 2024-03-08 09:12:59.000000 naja-atra-1.0.2/pyproject.toml
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)       38 2024-04-03 08:02:02.256513 naja-atra-1.0.2/setup.cfg
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)       62 2023-01-29 02:07:01.000000 naja-atra-1.0.2/setup.py
+drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-04-03 08:02:02.248513 naja-atra-1.0.2/tests/
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)        0 2023-01-29 02:07:01.000000 naja-atra-1.0.2/tests/__init__.py
+drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-04-03 08:02:02.252513 naja-atra-1.0.2/tests/ctrls/
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)        0 2023-01-29 02:07:01.000000 naja-atra-1.0.2/tests/ctrls/__init__.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     9970 2024-03-11 09:19:38.000000 naja-atra-1.0.2/tests/ctrls/my_controllers.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     1890 2024-03-11 08:58:23.000000 naja-atra-1.0.2/tests/ctrls/my_controllers_model_binding.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     3538 2024-03-07 03:14:28.000000 naja-atra-1.0.2/tests/ctrls/ws_controllers.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     8064 2024-03-08 02:52:49.000000 naja-atra-1.0.2/tests/test_all_ctrls.py
```

### Comparing `naja-atra-1.0.1/LICENSE` & `naja-atra-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `naja-atra-1.0.1/PKG-INFO` & `naja-atra-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naja-atra
-Version: 1.0.1
+Version: 1.0.2
 Summary: This is a simple http server, use MVC like design.
 Author-email: keijack <keijack.wu@gmail.com>
 License: MIT License
         
         Copyright (c) 2018 Keijack Wu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `naja-atra-1.0.1/README.md` & `naja-atra-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `naja-atra-1.0.1/naja_atra/__init__.py` & `naja-atra-1.0.2/naja_atra/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 SOFTWARE.
 """
 
 from .app_conf import *
 from .models import *
 
 name = "naja-atra"
-version = "1.0.1"
+version = "1.0.2"
```

### Comparing `naja-atra-1.0.1/naja_atra/__main__.py` & `naja-atra-1.0.2/naja_atra/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from .utils import logger
 
 _logger = logger.get_logger("naja_atra.__main__")
 
 
 def print_help():
     print("""
-    python3 -m naja-atra [options]
+    python3 -m naja_atra [options]
 
     Options:
     -h    --help        Show this message and exit.
     -p    --port        Specify alternate port (default: 9090)
     -b    --bind        Specify alternate bind address (default: all interfaces)
     -s    --scan        Scan this path to find controllers, if absent, will scan the current work directory
           --regex       Only import the files that macthes this regular expresseion.
```

### Comparing `naja-atra-1.0.1/naja_atra/app_conf.py` & `naja-atra-1.0.2/naja_atra/app_conf.py`

 * *Files identical despite different names*

### Comparing `naja-atra-1.0.1/naja_atra/http_servers/__init__.py` & `naja-atra-1.0.2/naja_atra/http_servers/__init__.py`

 * *Files identical despite different names*

### Comparing `naja-atra-1.0.1/naja_atra/http_servers/coroutine_http_server.py` & `naja-atra-1.0.2/naja_atra/http_servers/coroutine_http_server.py`

 * *Files identical despite different names*

### Comparing `naja-atra-1.0.1/naja_atra/http_servers/http_server.py` & `naja-atra-1.0.2/naja_atra/http_servers/http_server.py`

 * *Files identical despite different names*

### Comparing `naja-atra-1.0.1/naja_atra/http_servers/routing_server.py` & `naja-atra-1.0.2/naja_atra/http_servers/routing_server.py`

 * *Files identical despite different names*

### Comparing `naja-atra-1.0.1/naja_atra/http_servers/threading_http_server.py` & `naja-atra-1.0.2/naja_atra/http_servers/threading_http_server.py`

 * *Files identical despite different names*

### Comparing `naja-atra-1.0.1/naja_atra/models.py` & `naja-atra-1.0.2/naja_atra/models.py`

 * *Files identical despite different names*

### Comparing `naja-atra-1.0.1/naja_atra/request_handlers/__init__.py` & `naja-atra-1.0.2/naja_atra/request_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `naja-atra-1.0.1/naja_atra/request_handlers/http_controller_handler.py` & `naja-atra-1.0.2/naja_atra/request_handlers/http_controller_handler.py`

 * *Files identical despite different names*

### Comparing `naja-atra-1.0.1/naja_atra/request_handlers/http_request_handler.py` & `naja-atra-1.0.2/naja_atra/request_handlers/http_request_handler.py`

 * *Files identical despite different names*

### Comparing `naja-atra-1.0.1/naja_atra/request_handlers/http_session_local_impl.py` & `naja-atra-1.0.2/naja_atra/request_handlers/http_session_local_impl.py`

 * *Files identical despite different names*

### Comparing `naja-atra-1.0.1/naja_atra/request_handlers/model_bindings.py` & `naja-atra-1.0.2/naja_atra/request_handlers/model_bindings.py`

 * *Files identical despite different names*

### Comparing `naja-atra-1.0.1/naja_atra/request_handlers/websocket_controller_handler.py` & `naja-atra-1.0.2/naja_atra/request_handlers/websocket_controller_handler.py`

 * *Files identical despite different names*

### Comparing `naja-atra-1.0.1/naja_atra/server.py` & `naja-atra-1.0.2/naja_atra/server.py`

 * *Files identical despite different names*

### Comparing `naja-atra-1.0.1/naja_atra/utils/__init__.py` & `naja-atra-1.0.2/naja_atra/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `naja-atra-1.0.1/naja_atra/utils/http_utils.py` & `naja-atra-1.0.2/naja_atra/utils/http_utils.py`

 * *Files identical despite different names*

### Comparing `naja-atra-1.0.1/naja_atra/utils/logger.py` & `naja-atra-1.0.2/naja_atra/utils/logger.py`

 * *Files identical despite different names*

### Comparing `naja-atra-1.0.1/naja_atra.egg-info/PKG-INFO` & `naja-atra-1.0.2/naja_atra.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naja-atra
-Version: 1.0.1
+Version: 1.0.2
 Summary: This is a simple http server, use MVC like design.
 Author-email: keijack <keijack.wu@gmail.com>
 License: MIT License
         
         Copyright (c) 2018 Keijack Wu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `naja-atra-1.0.1/naja_atra.egg-info/SOURCES.txt` & `naja-atra-1.0.2/naja_atra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `naja-atra-1.0.1/pyproject.toml` & `naja-atra-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `naja-atra-1.0.1/tests/ctrls/my_controllers.py` & `naja-atra-1.0.2/tests/ctrls/my_controllers.py`

 * *Files identical despite different names*

### Comparing `naja-atra-1.0.1/tests/ctrls/my_controllers_model_binding.py` & `naja-atra-1.0.2/tests/ctrls/my_controllers_model_binding.py`

 * *Files identical despite different names*

### Comparing `naja-atra-1.0.1/tests/ctrls/ws_controllers.py` & `naja-atra-1.0.2/tests/ctrls/ws_controllers.py`

 * *Files identical despite different names*

### Comparing `naja-atra-1.0.1/tests/test_all_ctrls.py` & `naja-atra-1.0.2/tests/test_all_ctrls.py`

 * *Files identical despite different names*

