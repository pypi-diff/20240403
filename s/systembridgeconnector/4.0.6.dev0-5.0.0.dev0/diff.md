# Comparing `tmp/systembridgeconnector-4.0.6.dev0.tar.gz` & `tmp/systembridgeconnector-5.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systembridgeconnector-4.0.6.dev0.tar", last modified: Wed Apr  3 17:11:03 2024, max compression
+gzip compressed data, was "systembridgeconnector-5.0.0.dev0.tar", last modified: Wed Apr  3 17:13:40 2024, max compression
```

## Comparing `systembridgeconnector-4.0.6.dev0.tar` & `systembridgeconnector-5.0.0.dev0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:03.374973 systembridgeconnector-4.0.6.dev0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-03 17:10:43.000000 systembridgeconnector-4.0.6.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-03 17:11:03.374973 systembridgeconnector-4.0.6.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-03 17:10:43.000000 systembridgeconnector-4.0.6.dev0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7953 2024-04-03 17:10:43.000000 systembridgeconnector-4.0.6.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 17:11:03.374973 systembridgeconnector-4.0.6.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-03 17:10:43.000000 systembridgeconnector-4.0.6.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:03.374973 systembridgeconnector-4.0.6.dev0/systembridgeconnector/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-03 17:10:43.000000 systembridgeconnector-4.0.6.dev0/systembridgeconnector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-03 17:10:43.000000 systembridgeconnector-4.0.6.dev0/systembridgeconnector/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-03 17:10:43.000000 systembridgeconnector-4.0.6.dev0/systembridgeconnector/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-03 17:10:43.000000 systembridgeconnector-4.0.6.dev0/systembridgeconnector/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-03 17:10:43.000000 systembridgeconnector-4.0.6.dev0/systembridgeconnector/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-04-03 17:10:43.000000 systembridgeconnector-4.0.6.dev0/systembridgeconnector/http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-03 17:10:43.000000 systembridgeconnector-4.0.6.dev0/systembridgeconnector/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    21321 2024-04-03 17:10:43.000000 systembridgeconnector-4.0.6.dev0/systembridgeconnector/websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:03.374973 systembridgeconnector-4.0.6.dev0/systembridgeconnector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-03 17:11:03.000000 systembridgeconnector-4.0.6.dev0/systembridgeconnector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-03 17:11:03.000000 systembridgeconnector-4.0.6.dev0/systembridgeconnector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 17:11:03.000000 systembridgeconnector-4.0.6.dev0/systembridgeconnector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-03 17:11:03.000000 systembridgeconnector-4.0.6.dev0/systembridgeconnector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 17:11:03.000000 systembridgeconnector-4.0.6.dev0/systembridgeconnector.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:03.374973 systembridgeconnector-4.0.6.dev0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-03 17:10:43.000000 systembridgeconnector-4.0.6.dev0/tests/test__version.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-03 17:10:43.000000 systembridgeconnector-4.0.6.dev0/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-03 17:10:43.000000 systembridgeconnector-4.0.6.dev0/tests/test_const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-03 17:10:43.000000 systembridgeconnector-4.0.6.dev0/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-03 17:10:43.000000 systembridgeconnector-4.0.6.dev0/tests/test_http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-04-03 17:10:43.000000 systembridgeconnector-4.0.6.dev0/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    16794 2024-04-03 17:10:43.000000 systembridgeconnector-4.0.6.dev0/tests/test_websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:13:40.864965 systembridgeconnector-5.0.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-03 17:13:17.000000 systembridgeconnector-5.0.0.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-03 17:13:40.864965 systembridgeconnector-5.0.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-03 17:13:17.000000 systembridgeconnector-5.0.0.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7953 2024-04-03 17:13:17.000000 systembridgeconnector-5.0.0.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 17:13:40.864965 systembridgeconnector-5.0.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-03 17:13:17.000000 systembridgeconnector-5.0.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:13:40.860965 systembridgeconnector-5.0.0.dev0/systembridgeconnector/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-03 17:13:17.000000 systembridgeconnector-5.0.0.dev0/systembridgeconnector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-03 17:13:17.000000 systembridgeconnector-5.0.0.dev0/systembridgeconnector/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-03 17:13:17.000000 systembridgeconnector-5.0.0.dev0/systembridgeconnector/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-03 17:13:17.000000 systembridgeconnector-5.0.0.dev0/systembridgeconnector/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-03 17:13:17.000000 systembridgeconnector-5.0.0.dev0/systembridgeconnector/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-04-03 17:13:17.000000 systembridgeconnector-5.0.0.dev0/systembridgeconnector/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-03 17:13:17.000000 systembridgeconnector-5.0.0.dev0/systembridgeconnector/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21321 2024-04-03 17:13:17.000000 systembridgeconnector-5.0.0.dev0/systembridgeconnector/websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:13:40.864965 systembridgeconnector-5.0.0.dev0/systembridgeconnector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-03 17:13:40.000000 systembridgeconnector-5.0.0.dev0/systembridgeconnector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-03 17:13:40.000000 systembridgeconnector-5.0.0.dev0/systembridgeconnector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 17:13:40.000000 systembridgeconnector-5.0.0.dev0/systembridgeconnector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-03 17:13:40.000000 systembridgeconnector-5.0.0.dev0/systembridgeconnector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 17:13:40.000000 systembridgeconnector-5.0.0.dev0/systembridgeconnector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:13:40.864965 systembridgeconnector-5.0.0.dev0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-03 17:13:17.000000 systembridgeconnector-5.0.0.dev0/tests/test__version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-03 17:13:17.000000 systembridgeconnector-5.0.0.dev0/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-03 17:13:17.000000 systembridgeconnector-5.0.0.dev0/tests/test_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-03 17:13:17.000000 systembridgeconnector-5.0.0.dev0/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-03 17:13:17.000000 systembridgeconnector-5.0.0.dev0/tests/test_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-04-03 17:13:17.000000 systembridgeconnector-5.0.0.dev0/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16794 2024-04-03 17:13:17.000000 systembridgeconnector-5.0.0.dev0/tests/test_websocket_client.py
```

### Comparing `systembridgeconnector-4.0.6.dev0/LICENSE` & `systembridgeconnector-5.0.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-4.0.6.dev0/PKG-INFO` & `systembridgeconnector-5.0.0.dev0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: systembridgeconnector
-Version: 4.0.6.dev0
+Version: 5.0.0.dev0
 Summary: System Bridge Connector
 Home-page: https://github.com/timmo001/system-bridge-connector
 Author: Aidan Timson (Timmo)
 Author-email: aidan@timmo.dev
 License: Apache-2.0
 Keywords: system-bridge
 Requires-Python: >=3.11
```

### Comparing `systembridgeconnector-4.0.6.dev0/pyproject.toml` & `systembridgeconnector-5.0.0.dev0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-4.0.6.dev0/setup.py` & `systembridgeconnector-5.0.0.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-4.0.6.dev0/systembridgeconnector/const.py` & `systembridgeconnector-5.0.0.dev0/systembridgeconnector/const.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-4.0.6.dev0/systembridgeconnector/exceptions.py` & `systembridgeconnector-5.0.0.dev0/systembridgeconnector/exceptions.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-4.0.6.dev0/systembridgeconnector/http_client.py` & `systembridgeconnector-5.0.0.dev0/systembridgeconnector/http_client.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-4.0.6.dev0/systembridgeconnector/version.py` & `systembridgeconnector-5.0.0.dev0/systembridgeconnector/version.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-4.0.6.dev0/systembridgeconnector/websocket_client.py` & `systembridgeconnector-5.0.0.dev0/systembridgeconnector/websocket_client.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-4.0.6.dev0/systembridgeconnector.egg-info/PKG-INFO` & `systembridgeconnector-5.0.0.dev0/systembridgeconnector.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: systembridgeconnector
-Version: 4.0.6.dev0
+Version: 5.0.0.dev0
 Summary: System Bridge Connector
 Home-page: https://github.com/timmo001/system-bridge-connector
 Author: Aidan Timson (Timmo)
 Author-email: aidan@timmo.dev
 License: Apache-2.0
 Keywords: system-bridge
 Requires-Python: >=3.11
```

### Comparing `systembridgeconnector-4.0.6.dev0/systembridgeconnector.egg-info/SOURCES.txt` & `systembridgeconnector-5.0.0.dev0/systembridgeconnector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-4.0.6.dev0/tests/test_const.py` & `systembridgeconnector-5.0.0.dev0/tests/test_const.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-4.0.6.dev0/tests/test_exceptions.py` & `systembridgeconnector-5.0.0.dev0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-4.0.6.dev0/tests/test_http_client.py` & `systembridgeconnector-5.0.0.dev0/tests/test_http_client.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-4.0.6.dev0/tests/test_version.py` & `systembridgeconnector-5.0.0.dev0/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-4.0.6.dev0/tests/test_websocket_client.py` & `systembridgeconnector-5.0.0.dev0/tests/test_websocket_client.py`

 * *Files identical despite different names*

