# Comparing `tmp/systembridgeconnector-4.0.5.tar.gz` & `tmp/systembridgeconnector-4.0.6.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systembridgeconnector-4.0.5.tar", last modified: Fri Mar 29 09:31:38 2024, max compression
+gzip compressed data, was "systembridgeconnector-4.0.6.dev0.tar", last modified: Wed Apr  3 17:11:03 2024, max compression
```

## Comparing `systembridgeconnector-4.0.5.tar` & `systembridgeconnector-4.0.6.dev0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 09:31:38.418959 systembridgeconnector-4.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-29 09:31:18.000000 systembridgeconnector-4.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-03-29 09:31:38.418959 systembridgeconnector-4.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-03-29 09:31:18.000000 systembridgeconnector-4.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7953 2024-03-29 09:31:18.000000 systembridgeconnector-4.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 09:31:38.418959 systembridgeconnector-4.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-03-29 09:31:18.000000 systembridgeconnector-4.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 09:31:38.414959 systembridgeconnector-4.0.5/systembridgeconnector/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-29 09:31:18.000000 systembridgeconnector-4.0.5/systembridgeconnector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-29 09:31:36.000000 systembridgeconnector-4.0.5/systembridgeconnector/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-29 09:31:18.000000 systembridgeconnector-4.0.5/systembridgeconnector/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-03-29 09:31:18.000000 systembridgeconnector-4.0.5/systembridgeconnector/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-03-29 09:31:18.000000 systembridgeconnector-4.0.5/systembridgeconnector/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-03-29 09:31:18.000000 systembridgeconnector-4.0.5/systembridgeconnector/http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-03-29 09:31:18.000000 systembridgeconnector-4.0.5/systembridgeconnector/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    20297 2024-03-29 09:31:18.000000 systembridgeconnector-4.0.5/systembridgeconnector/websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 09:31:38.418959 systembridgeconnector-4.0.5/systembridgeconnector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-03-29 09:31:38.000000 systembridgeconnector-4.0.5/systembridgeconnector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-03-29 09:31:38.000000 systembridgeconnector-4.0.5/systembridgeconnector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 09:31:38.000000 systembridgeconnector-4.0.5/systembridgeconnector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-29 09:31:38.000000 systembridgeconnector-4.0.5/systembridgeconnector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-29 09:31:38.000000 systembridgeconnector-4.0.5/systembridgeconnector.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 09:31:38.418959 systembridgeconnector-4.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-29 09:31:18.000000 systembridgeconnector-4.0.5/tests/test__version.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-29 09:31:18.000000 systembridgeconnector-4.0.5/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-03-29 09:31:18.000000 systembridgeconnector-4.0.5/tests/test_const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-03-29 09:31:18.000000 systembridgeconnector-4.0.5/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-03-29 09:31:18.000000 systembridgeconnector-4.0.5/tests/test_http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-03-29 09:31:18.000000 systembridgeconnector-4.0.5/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    18469 2024-03-29 09:31:18.000000 systembridgeconnector-4.0.5/tests/test_websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:03.374973 systembridgeconnector-4.0.6.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-03 17:10:43.000000 systembridgeconnector-4.0.6.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-03 17:11:03.374973 systembridgeconnector-4.0.6.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-03 17:10:43.000000 systembridgeconnector-4.0.6.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7953 2024-04-03 17:10:43.000000 systembridgeconnector-4.0.6.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 17:11:03.374973 systembridgeconnector-4.0.6.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-03 17:10:43.000000 systembridgeconnector-4.0.6.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:03.374973 systembridgeconnector-4.0.6.dev0/systembridgeconnector/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-03 17:10:43.000000 systembridgeconnector-4.0.6.dev0/systembridgeconnector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-03 17:10:43.000000 systembridgeconnector-4.0.6.dev0/systembridgeconnector/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-03 17:10:43.000000 systembridgeconnector-4.0.6.dev0/systembridgeconnector/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-03 17:10:43.000000 systembridgeconnector-4.0.6.dev0/systembridgeconnector/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-03 17:10:43.000000 systembridgeconnector-4.0.6.dev0/systembridgeconnector/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-04-03 17:10:43.000000 systembridgeconnector-4.0.6.dev0/systembridgeconnector/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-03 17:10:43.000000 systembridgeconnector-4.0.6.dev0/systembridgeconnector/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21321 2024-04-03 17:10:43.000000 systembridgeconnector-4.0.6.dev0/systembridgeconnector/websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:03.374973 systembridgeconnector-4.0.6.dev0/systembridgeconnector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-03 17:11:03.000000 systembridgeconnector-4.0.6.dev0/systembridgeconnector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-03 17:11:03.000000 systembridgeconnector-4.0.6.dev0/systembridgeconnector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 17:11:03.000000 systembridgeconnector-4.0.6.dev0/systembridgeconnector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-03 17:11:03.000000 systembridgeconnector-4.0.6.dev0/systembridgeconnector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 17:11:03.000000 systembridgeconnector-4.0.6.dev0/systembridgeconnector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:03.374973 systembridgeconnector-4.0.6.dev0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-03 17:10:43.000000 systembridgeconnector-4.0.6.dev0/tests/test__version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-03 17:10:43.000000 systembridgeconnector-4.0.6.dev0/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-03 17:10:43.000000 systembridgeconnector-4.0.6.dev0/tests/test_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-03 17:10:43.000000 systembridgeconnector-4.0.6.dev0/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-03 17:10:43.000000 systembridgeconnector-4.0.6.dev0/tests/test_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-04-03 17:10:43.000000 systembridgeconnector-4.0.6.dev0/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16794 2024-04-03 17:10:43.000000 systembridgeconnector-4.0.6.dev0/tests/test_websocket_client.py
```

### Comparing `systembridgeconnector-4.0.5/LICENSE` & `systembridgeconnector-4.0.6.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-4.0.5/PKG-INFO` & `systembridgeconnector-4.0.6.dev0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: systembridgeconnector
-Version: 4.0.5
+Version: 4.0.6.dev0
 Summary: System Bridge Connector
 Home-page: https://github.com/timmo001/system-bridge-connector
 Author: Aidan Timson (Timmo)
 Author-email: aidan@timmo.dev
 License: Apache-2.0
 Keywords: system-bridge
 Requires-Python: >=3.11
```

### Comparing `systembridgeconnector-4.0.5/pyproject.toml` & `systembridgeconnector-4.0.6.dev0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-4.0.5/setup.py` & `systembridgeconnector-4.0.6.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-4.0.5/systembridgeconnector/const.py` & `systembridgeconnector-4.0.6.dev0/systembridgeconnector/const.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-4.0.5/systembridgeconnector/http_client.py` & `systembridgeconnector-4.0.6.dev0/systembridgeconnector/http_client.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-4.0.5/systembridgeconnector/version.py` & `systembridgeconnector-4.0.6.dev0/systembridgeconnector/version.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-4.0.5/systembridgeconnector/websocket_client.py` & `systembridgeconnector-4.0.6.dev0/systembridgeconnector/websocket_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from systembridgemodels.keyboard_key import KeyboardKey
 from systembridgemodels.keyboard_text import KeyboardText
 from systembridgemodels.media_control import MediaControl
 from systembridgemodels.media_directories import MediaDirectory
 from systembridgemodels.media_files import MediaFile, MediaFiles
 from systembridgemodels.media_get_file import MediaGetFile
 from systembridgemodels.media_get_files import MediaGetFiles
-from systembridgemodels.modules import GetData, RegisterDataListener
+from systembridgemodels.modules import GetData, ModulesData, RegisterDataListener
 from systembridgemodels.notification import Notification
 from systembridgemodels.open_path import OpenPath
 from systembridgemodels.open_url import OpenUrl
 from systembridgemodels.request import Request
 from systembridgemodels.response import Response
 from systembridgemodels.update import Update
 
@@ -74,14 +74,15 @@
     TYPE_REGISTER_DATA_LISTENER,
 )
 from .exceptions import (
     AuthenticationException,
     BadMessageException,
     ConnectionClosedException,
     ConnectionErrorException,
+    DataMissingException,
 )
 
 
 class WebSocketClient(Base):
     """WebSocket Client."""
 
     def __init__(
@@ -227,25 +228,57 @@
             wait_for_response=False,
         )
 
     async def get_data(
         self,
         model: GetData,
         request_id: str = uuid4().hex,
-    ) -> Response:
+        timeout: int = 10,
+    ) -> ModulesData:
         """Get data from server."""
         self._logger.info("Getting data from server: %s", model)
-        return await self._send_message(
+
+        modules_data = ModulesData()
+
+        async def handle_module(
+            module_name: str,
+            module: Any,
+        ) -> None:
+            """Handle returned data."""
+            self._logger.debug("Set new data for: %s", module_name)
+            setattr(modules_data, module_name, module)
+
+        await self.listen(
+            callback=handle_module,
+            accept_other_types=False,
+        )
+
+        await self._send_message(
             TYPE_GET_DATA,
             request_id,
             asdict(model),
             wait_for_response=True,
             response_type=TYPE_DATA_GET,
         )
 
+        # Wait for all data modules to be set
+        try:
+            async with asyncio.timeout(timeout):
+                while not all(
+                    getattr(modules_data, module_name) is not None
+                    for module_name in model.modules
+                ):
+                    await asyncio.sleep(0.1)
+        except asyncio.TimeoutError as exception:
+            raise DataMissingException(
+                f"Timeout waiting for data after {timeout} seconds"
+            ) from exception
+
+        return modules_data
+
     async def get_directories(
         self,
         request_id: str = uuid4().hex,
     ) -> list[MediaDirectory]:
         """Get directories."""
         self._logger.info("Getting directories..")
         response = await self._send_message(
```

### Comparing `systembridgeconnector-4.0.5/systembridgeconnector.egg-info/PKG-INFO` & `systembridgeconnector-4.0.6.dev0/systembridgeconnector.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: systembridgeconnector
-Version: 4.0.5
+Version: 4.0.6.dev0
 Summary: System Bridge Connector
 Home-page: https://github.com/timmo001/system-bridge-connector
 Author: Aidan Timson (Timmo)
 Author-email: aidan@timmo.dev
 License: Apache-2.0
 Keywords: system-bridge
 Requires-Python: >=3.11
```

### Comparing `systembridgeconnector-4.0.5/systembridgeconnector.egg-info/SOURCES.txt` & `systembridgeconnector-4.0.6.dev0/systembridgeconnector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-4.0.5/tests/test_const.py` & `systembridgeconnector-4.0.6.dev0/tests/test_const.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-4.0.5/tests/test_exceptions.py` & `systembridgeconnector-4.0.6.dev0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-4.0.5/tests/test_http_client.py` & `systembridgeconnector-4.0.6.dev0/tests/test_http_client.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-4.0.5/tests/test_version.py` & `systembridgeconnector-4.0.6.dev0/tests/test_version.py`

 * *Files identical despite different names*

