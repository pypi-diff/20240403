# Comparing `tmp/th2_grpc_act_uiframework_win_demo-1.3.0.dev8383647490.tar.gz` & `tmp/th2_grpc_act_uiframework_win_demo-1.3.0.dev8544485212.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_grpc_act_uiframework_win_demo-1.3.0.dev8383647490.tar", last modified: Fri Mar 22 00:39:00 2024, max compression
+gzip compressed data, was "dist/th2_grpc_act_uiframework_win_demo-1.3.0.dev8544485212.tar", last modified: Wed Apr  3 19:35:39 2024, max compression
```

## Comparing `th2_grpc_act_uiframework_win_demo-1.3.0.dev8383647490.tar` & `th2_grpc_act_uiframework_win_demo-1.3.0.dev8544485212.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 00:39:00.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8383647490/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-03-22 00:39:00.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8383647490/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-22 00:37:57.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8383647490/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-22 00:37:57.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8383647490/package_info.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 00:39:00.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8383647490/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-03-22 00:37:57.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8383647490/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 00:39:00.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8383647490/th2_grpc_act_uiframework_win_demo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 00:38:59.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8383647490/th2_grpc_act_uiframework_win_demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 00:38:59.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8383647490/th2_grpc_act_uiframework_win_demo/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-03-22 00:38:29.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8383647490/th2_grpc_act_uiframework_win_demo/u_i_framework_act_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-03-22 00:37:57.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8383647490/th2_grpc_act_uiframework_win_demo/uiframework_win_demo.proto
--rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-03-22 00:38:59.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8383647490/th2_grpc_act_uiframework_win_demo/uiframework_win_demo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10912 2024-03-22 00:38:59.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8383647490/th2_grpc_act_uiframework_win_demo/uiframework_win_demo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    17630 2024-03-22 00:38:59.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8383647490/th2_grpc_act_uiframework_win_demo/uiframework_win_demo_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 00:39:00.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8383647490/th2_grpc_act_uiframework_win_demo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-03-22 00:38:59.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8383647490/th2_grpc_act_uiframework_win_demo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-03-22 00:39:00.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8383647490/th2_grpc_act_uiframework_win_demo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 00:38:59.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8383647490/th2_grpc_act_uiframework_win_demo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-22 00:38:59.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8383647490/th2_grpc_act_uiframework_win_demo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-22 00:38:59.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8383647490/th2_grpc_act_uiframework_win_demo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:35:39.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8544485212/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-03 19:35:39.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8544485212/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-03 19:34:08.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8544485212/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-03 19:34:09.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8544485212/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:35:39.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8544485212/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-04-03 19:34:08.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8544485212/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:35:39.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8544485212/th2_grpc_act_uiframework_win_demo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 19:35:39.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8544485212/th2_grpc_act_uiframework_win_demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 19:35:39.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8544485212/th2_grpc_act_uiframework_win_demo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-03 19:35:08.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8544485212/th2_grpc_act_uiframework_win_demo/u_i_framework_act_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-03 19:34:08.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8544485212/th2_grpc_act_uiframework_win_demo/uiframework_win_demo.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-04-03 19:35:39.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8544485212/th2_grpc_act_uiframework_win_demo/uiframework_win_demo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10912 2024-04-03 19:35:39.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8544485212/th2_grpc_act_uiframework_win_demo/uiframework_win_demo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    17630 2024-04-03 19:35:39.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8544485212/th2_grpc_act_uiframework_win_demo/uiframework_win_demo_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:35:39.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8544485212/th2_grpc_act_uiframework_win_demo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-03 19:35:39.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8544485212/th2_grpc_act_uiframework_win_demo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-03 19:35:39.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8544485212/th2_grpc_act_uiframework_win_demo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:35:39.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8544485212/th2_grpc_act_uiframework_win_demo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-03 19:35:39.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8544485212/th2_grpc_act_uiframework_win_demo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-03 19:35:39.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8544485212/th2_grpc_act_uiframework_win_demo.egg-info/top_level.txt
```

### Comparing `th2_grpc_act_uiframework_win_demo-1.3.0.dev8383647490/setup.py` & `th2_grpc_act_uiframework_win_demo-1.3.0.dev8544485212/setup.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_act_uiframework_win_demo-1.3.0.dev8383647490/th2_grpc_act_uiframework_win_demo/u_i_framework_act_service.py` & `th2_grpc_act_uiframework_win_demo-1.3.0.dev8544485212/th2_grpc_act_uiframework_win_demo/u_i_framework_act_service.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_act_uiframework_win_demo-1.3.0.dev8383647490/th2_grpc_act_uiframework_win_demo/uiframework_win_demo.proto` & `th2_grpc_act_uiframework_win_demo-1.3.0.dev8544485212/th2_grpc_act_uiframework_win_demo/uiframework_win_demo.proto`

 * *Files identical despite different names*

### Comparing `th2_grpc_act_uiframework_win_demo-1.3.0.dev8383647490/th2_grpc_act_uiframework_win_demo/uiframework_win_demo_pb2.py` & `th2_grpc_act_uiframework_win_demo-1.3.0.dev8544485212/th2_grpc_act_uiframework_win_demo/uiframework_win_demo_pb2.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_act_uiframework_win_demo-1.3.0.dev8383647490/th2_grpc_act_uiframework_win_demo/uiframework_win_demo_pb2.pyi` & `th2_grpc_act_uiframework_win_demo-1.3.0.dev8544485212/th2_grpc_act_uiframework_win_demo/uiframework_win_demo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `th2_grpc_act_uiframework_win_demo-1.3.0.dev8383647490/th2_grpc_act_uiframework_win_demo/uiframework_win_demo_pb2_grpc.py` & `th2_grpc_act_uiframework_win_demo-1.3.0.dev8544485212/th2_grpc_act_uiframework_win_demo/uiframework_win_demo_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_act_uiframework_win_demo-1.3.0.dev8383647490/th2_grpc_act_uiframework_win_demo.egg-info/SOURCES.txt` & `th2_grpc_act_uiframework_win_demo-1.3.0.dev8544485212/th2_grpc_act_uiframework_win_demo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

