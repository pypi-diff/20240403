# Comparing `tmp/aioairzone-cloud-0.4.6.tar.gz` & `tmp/aioairzone-cloud-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioairzone-cloud-0.4.6.tar", last modified: Mon Mar  4 12:09:50 2024, max compression
+gzip compressed data, was "aioairzone-cloud-0.4.7.tar", last modified: Wed Apr  3 16:39:10 2024, max compression
```

## Comparing `aioairzone-cloud-0.4.6.tar` & `aioairzone-cloud-0.4.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2024-03-04 12:09:50.169852 aioairzone-cloud-0.4.6/
--rw-r--r--   0 noltari   (1000) noltari   (1000)    11357 2023-12-27 17:30:29.000000 aioairzone-cloud-0.4.6/LICENSE
--rw-r--r--   0 noltari   (1000) noltari   (1000)       59 2023-12-27 17:30:29.000000 aioairzone-cloud-0.4.6/MANIFEST.in
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1551 2024-03-04 12:09:50.169852 aioairzone-cloud-0.4.6/PKG-INFO
--rw-r--r--   0 noltari   (1000) noltari   (1000)      746 2023-12-27 17:30:29.000000 aioairzone-cloud-0.4.6/README.md
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2024-03-04 12:09:50.169852 aioairzone-cloud-0.4.6/aioairzone_cloud/
--rw-r--r--   0 noltari   (1000) noltari   (1000)       33 2023-12-27 17:30:29.000000 aioairzone-cloud-0.4.6/aioairzone_cloud/__init__.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     3234 2024-02-28 12:49:43.000000 aioairzone-cloud-0.4.6/aioairzone_cloud/aidoo.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    30073 2024-03-04 12:07:51.000000 aioairzone-cloud-0.4.6/aioairzone_cloud/cloudapi.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     2206 2024-02-28 17:18:10.000000 aioairzone-cloud-0.4.6/aioairzone_cloud/common.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     9556 2024-02-28 17:57:26.000000 aioairzone-cloud-0.4.6/aioairzone_cloud/const.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     8681 2024-02-28 12:49:43.000000 aioairzone-cloud-0.4.6/aioairzone_cloud/device.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    10924 2024-02-28 08:54:11.000000 aioairzone-cloud-0.4.6/aioairzone_cloud/device_group.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     3081 2024-02-28 14:34:38.000000 aioairzone-cloud-0.4.6/aioairzone_cloud/entity.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)      807 2024-02-28 08:54:11.000000 aioairzone-cloud-0.4.6/aioairzone_cloud/exceptions.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)      925 2024-02-28 08:54:11.000000 aioairzone-cloud-0.4.6/aioairzone_cloud/group.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    25730 2024-02-28 12:49:43.000000 aioairzone-cloud-0.4.6/aioairzone_cloud/hvac.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1821 2024-02-28 08:54:11.000000 aioairzone-cloud-0.4.6/aioairzone_cloud/installation.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)        0 2023-12-27 17:30:29.000000 aioairzone-cloud-0.4.6/aioairzone_cloud/py.typed
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1463 2024-02-28 08:54:11.000000 aioairzone-cloud-0.4.6/aioairzone_cloud/system.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     2495 2024-02-28 12:49:43.000000 aioairzone-cloud-0.4.6/aioairzone_cloud/token.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     5835 2024-02-28 12:49:43.000000 aioairzone-cloud-0.4.6/aioairzone_cloud/webserver.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     8581 2024-03-04 12:07:51.000000 aioairzone-cloud-0.4.6/aioairzone_cloud/websockets.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     3409 2024-02-28 14:34:38.000000 aioairzone-cloud-0.4.6/aioairzone_cloud/zone.py
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2024-03-04 12:09:50.169852 aioairzone-cloud-0.4.6/aioairzone_cloud.egg-info/
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1551 2024-03-04 12:09:50.000000 aioairzone-cloud-0.4.6/aioairzone_cloud.egg-info/PKG-INFO
--rw-r--r--   0 noltari   (1000) noltari   (1000)      803 2024-03-04 12:09:50.000000 aioairzone-cloud-0.4.6/aioairzone_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2024-03-04 12:09:50.000000 aioairzone-cloud-0.4.6/aioairzone_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2024-03-04 12:09:50.000000 aioairzone-cloud-0.4.6/aioairzone_cloud.egg-info/not-zip-safe
--rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2024-03-04 12:09:50.000000 aioairzone-cloud-0.4.6/aioairzone_cloud.egg-info/requires.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)       17 2024-03-04 12:09:50.000000 aioairzone-cloud-0.4.6/aioairzone_cloud.egg-info/top_level.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)     2327 2024-03-04 12:08:01.000000 aioairzone-cloud-0.4.6/pyproject.toml
--rw-r--r--   0 noltari   (1000) noltari   (1000)       77 2023-12-27 17:30:29.000000 aioairzone-cloud-0.4.6/requirements.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)       38 2024-03-04 12:09:50.169852 aioairzone-cloud-0.4.6/setup.cfg
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2024-04-03 16:39:10.896730 aioairzone-cloud-0.4.7/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    11357 2023-12-27 17:30:29.000000 aioairzone-cloud-0.4.7/LICENSE
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       59 2023-12-27 17:30:29.000000 aioairzone-cloud-0.4.7/MANIFEST.in
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1551 2024-04-03 16:39:10.896730 aioairzone-cloud-0.4.7/PKG-INFO
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      746 2023-12-27 17:30:29.000000 aioairzone-cloud-0.4.7/README.md
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2024-04-03 16:39:10.896730 aioairzone-cloud-0.4.7/aioairzone_cloud/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       33 2023-12-27 17:30:29.000000 aioairzone-cloud-0.4.7/aioairzone_cloud/__init__.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     3306 2024-04-03 16:34:41.000000 aioairzone-cloud-0.4.7/aioairzone_cloud/aidoo.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    30073 2024-04-03 16:04:15.000000 aioairzone-cloud-0.4.7/aioairzone_cloud/cloudapi.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     2777 2024-04-03 16:28:32.000000 aioairzone-cloud-0.4.7/aioairzone_cloud/common.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     9556 2024-02-28 17:57:26.000000 aioairzone-cloud-0.4.7/aioairzone_cloud/const.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     8796 2024-04-03 16:34:41.000000 aioairzone-cloud-0.4.7/aioairzone_cloud/device.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    10924 2024-02-28 08:54:11.000000 aioairzone-cloud-0.4.7/aioairzone_cloud/device_group.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     3081 2024-02-28 14:34:38.000000 aioairzone-cloud-0.4.7/aioairzone_cloud/entity.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      807 2024-02-28 08:54:11.000000 aioairzone-cloud-0.4.7/aioairzone_cloud/exceptions.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      925 2024-04-03 16:08:52.000000 aioairzone-cloud-0.4.7/aioairzone_cloud/group.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    25143 2024-04-03 16:34:41.000000 aioairzone-cloud-0.4.7/aioairzone_cloud/hvac.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1821 2024-04-03 16:08:59.000000 aioairzone-cloud-0.4.7/aioairzone_cloud/installation.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        0 2023-12-27 17:30:29.000000 aioairzone-cloud-0.4.7/aioairzone_cloud/py.typed
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1463 2024-04-03 16:09:19.000000 aioairzone-cloud-0.4.7/aioairzone_cloud/system.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     2495 2024-02-28 12:49:43.000000 aioairzone-cloud-0.4.7/aioairzone_cloud/token.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     5948 2024-04-03 16:34:41.000000 aioairzone-cloud-0.4.7/aioairzone_cloud/webserver.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     8581 2024-04-03 16:04:15.000000 aioairzone-cloud-0.4.7/aioairzone_cloud/websockets.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     3483 2024-04-03 16:34:41.000000 aioairzone-cloud-0.4.7/aioairzone_cloud/zone.py
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2024-04-03 16:39:10.896730 aioairzone-cloud-0.4.7/aioairzone_cloud.egg-info/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1551 2024-04-03 16:39:10.000000 aioairzone-cloud-0.4.7/aioairzone_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      803 2024-04-03 16:39:10.000000 aioairzone-cloud-0.4.7/aioairzone_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2024-04-03 16:39:10.000000 aioairzone-cloud-0.4.7/aioairzone_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2024-04-03 16:39:10.000000 aioairzone-cloud-0.4.7/aioairzone_cloud.egg-info/not-zip-safe
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2024-04-03 16:39:10.000000 aioairzone-cloud-0.4.7/aioairzone_cloud.egg-info/requires.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       17 2024-04-03 16:39:10.000000 aioairzone-cloud-0.4.7/aioairzone_cloud.egg-info/top_level.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     2327 2024-04-03 16:35:39.000000 aioairzone-cloud-0.4.7/pyproject.toml
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       77 2023-12-27 17:30:29.000000 aioairzone-cloud-0.4.7/requirements.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       38 2024-04-03 16:39:10.896730 aioairzone-cloud-0.4.7/setup.cfg
```

### Comparing `aioairzone-cloud-0.4.6/LICENSE` & `aioairzone-cloud-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.4.6/PKG-INFO` & `aioairzone-cloud-0.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioairzone-cloud
-Version: 0.4.6
+Version: 0.4.7
 Summary: Library to control Airzone Cloud devices
 Author-email: Álvaro Fernández Rojas <noltari@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Noltari/aioairzone-cloud
 Project-URL: Bug Tracker, https://github.com/Noltari/aioairzone-cloud/issues
 Keywords: airzone,cloud,hvac,home
 Platform: any
```

### Comparing `aioairzone-cloud-0.4.6/README.md` & `aioairzone-cloud-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.4.6/aioairzone_cloud/aidoo.py` & `aioairzone-cloud-0.4.7/aioairzone_cloud/aidoo.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Airzone Cloud API Aidoo device."""
 
 from __future__ import annotations
 
 from typing import Any
 
-from .common import SpeedType
+from .common import SpeedType, parse_int, parse_str
 from .const import (
     API_MODE,
     API_NAME,
     API_POWER,
     API_SETPOINT,
     API_SPEED_CONF,
     API_SPEED_TYPE,
@@ -29,16 +29,17 @@
         """Airzone Cloud Aidoo device init."""
         super().__init__(inst_id, ws_id, device_data)
 
         self.speed: int | None = None
         self.speeds: dict[int, int] = {}
         self.speed_type: SpeedType | None = None
 
-        if API_NAME in device_data:
-            self.name = str(device_data[API_NAME])
+        device_name = parse_str(device_data.get(API_NAME))
+        if device_name is not None:
+            self.name = device_name
         else:
             self.name = f"Aidoo {ws_id}"
 
     def data(self) -> dict[str, Any]:
         """Return Aidoo device data."""
         data = super().data()
 
@@ -88,17 +89,17 @@
 
     def update_data(self, update: EntityUpdate) -> None:
         """Update Aidoo data."""
         super().update_data(update)
 
         data = update.get_data()
 
-        speed = data.get(API_SPEED_CONF)
+        speed = parse_int(data.get(API_SPEED_CONF))
         if speed is not None:
-            self.speed = int(speed)
+            self.speed = speed
 
         speed_type = data.get(API_SPEED_TYPE)
         if speed_type is not None:
             self.speed_type = SpeedType(speed_type)
 
         speeds_values: list[int] | None = data.get(API_SPEED_VALUES)
         if speeds_values is not None:
```

### Comparing `aioairzone-cloud-0.4.6/aioairzone_cloud/cloudapi.py` & `aioairzone-cloud-0.4.7/aioairzone_cloud/cloudapi.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.4.6/aioairzone_cloud/common.py` & `aioairzone-cloud-0.4.7/aioairzone_cloud/common.py`

 * *Files 18% similar despite different names*

```diff
@@ -102,7 +102,35 @@
 
 
 class TemperatureUnit(IntEnum):
     """Airzone Cloud temperature units."""
 
     CELSIUS = 0
     FAHRENHEIT = 1
+
+
+def parse_bool(data: Any) -> bool | None:
+    """Convert data to bool."""
+    if data is not None:
+        return bool(data)
+    return None
+
+
+def parse_float(data: Any) -> float | None:
+    """Convert data to float."""
+    if data is not None:
+        return float(data)
+    return None
+
+
+def parse_int(data: Any) -> int | None:
+    """Convert data to int."""
+    if data is not None:
+        return int(data)
+    return None
+
+
+def parse_str(data: Any) -> str | None:
+    """Convert data to string."""
+    if data is not None:
+        return str(data)
+    return None
```

### Comparing `aioairzone-cloud-0.4.6/aioairzone_cloud/const.py` & `aioairzone-cloud-0.4.7/aioairzone_cloud/const.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.4.6/aioairzone_cloud/device.py` & `aioairzone-cloud-0.4.7/aioairzone_cloud/device.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from __future__ import annotations
 
 from abc import abstractmethod
 import logging
 from typing import Any
 
-from .common import OperationMode
+from .common import OperationMode, parse_bool, parse_int, parse_str
 from .const import (
     API_AQ_PM_1,
     API_AQ_PM_2P5,
     API_AQ_PM_10,
     API_AQ_PRESENT,
     API_AQ_QUALITY,
     API_AQ_STATUS,
@@ -68,16 +68,17 @@
         self.mode: OperationMode | None = None
         self.modes: list[OperationMode] = []
         self.name: str = "Device"
         self.warnings: list[str] = []
         self.webserver_id = ws_id
         self.ws_connected: bool = True
 
-        if API_IS_CONNECTED in device_data:
-            self.is_connected = bool(device_data[API_IS_CONNECTED])
+        is_connected = parse_bool(device_data.get(API_IS_CONNECTED))
+        if is_connected is not None:
+            self.is_connected = is_connected
         else:
             self.is_connected = True
 
     def sub_data(self, device_data: dict[str, Any]) -> dict[str, Any]:
         """Get Device sub data."""
         if API_META in device_data:
             meta: dict[str, Any] = device_data.get(API_META, {})
@@ -241,40 +242,40 @@
     def set_param(self, param: str, data: dict[str, Any]) -> None:
         """Update device parameter from API request."""
 
     def update_data(self, update: EntityUpdate) -> None:
         """Update Device data."""
         data = update.get_data()
 
-        is_connected = data.get(API_IS_CONNECTED)
+        is_connected = parse_bool(data.get(API_IS_CONNECTED))
         if is_connected is not None:
-            self.is_connected = bool(is_connected)
-        ws_connected = data.get(API_WS_CONNECTED)
+            self.is_connected = is_connected
+        ws_connected = parse_bool(data.get(API_WS_CONNECTED))
         if ws_connected is not None:
-            self.ws_connected = bool(ws_connected)
+            self.ws_connected = ws_connected
 
-        aq_pm_1 = data.get(API_AQ_PM_1)
+        aq_pm_1 = parse_int(data.get(API_AQ_PM_1))
         if aq_pm_1 is not None:
-            self.aq_pm_1 = int(aq_pm_1)
+            self.aq_pm_1 = aq_pm_1
 
-        aq_pm_2p5 = data.get(API_AQ_PM_2P5)
+        aq_pm_2p5 = parse_int(data.get(API_AQ_PM_2P5))
         if aq_pm_2p5 is not None:
-            self.aq_pm_2p5 = int(aq_pm_2p5)
+            self.aq_pm_2p5 = aq_pm_2p5
 
-        aq_pm_10 = data.get(API_AQ_PM_10)
+        aq_pm_10 = parse_int(data.get(API_AQ_PM_10))
         if aq_pm_10 is not None:
-            self.aq_pm_10 = int(aq_pm_10)
+            self.aq_pm_10 = aq_pm_10
 
-        aq_present = data.get(API_AQ_PRESENT)
+        aq_present = parse_bool(data.get(API_AQ_PRESENT))
         if aq_present is not None:
-            self.aq_present = bool(aq_present)
+            self.aq_present = aq_present
 
-        aq_status = data.get(API_AQ_QUALITY)
+        aq_status = parse_str(data.get(API_AQ_QUALITY))
         if aq_status is not None:
-            self.aq_status = str(aq_status)
+            self.aq_status = aq_status
 
         errors = data.get(API_ERRORS)
         if errors is not None:
             self.errors = []
             for error in errors:
                 self.errors += [error]
```

### Comparing `aioairzone-cloud-0.4.6/aioairzone_cloud/device_group.py` & `aioairzone-cloud-0.4.7/aioairzone_cloud/device_group.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.4.6/aioairzone_cloud/entity.py` & `aioairzone-cloud-0.4.7/aioairzone_cloud/entity.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.4.6/aioairzone_cloud/exceptions.py` & `aioairzone-cloud-0.4.7/aioairzone_cloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.4.6/aioairzone_cloud/group.py` & `aioairzone-cloud-0.4.7/aioairzone_cloud/group.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.4.6/aioairzone_cloud/hvac.py` & `aioairzone-cloud-0.4.7/aioairzone_cloud/hvac.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 """Airzone Cloud API HVAC device."""
 
 from __future__ import annotations
 
 from typing import Any
 
-from .common import AirQualityMode, OperationAction, OperationMode
+from .common import (
+    AirQualityMode,
+    OperationAction,
+    OperationMode,
+    parse_bool,
+    parse_float,
+    parse_int,
+)
 from .const import (
     API_ACTIVE,
     API_AQ_ACTIVE,
     API_AQ_MODE_CONF,
     API_AQ_MODE_VALUES,
     API_CELSIUS,
     API_DEFAULT_TEMP_STEP,
@@ -495,139 +502,140 @@
     def update_data(self, update: EntityUpdate) -> None:
         """Update HVAC device data."""
         super().update_data(update)
 
         data = update.get_data()
 
         if API_ACTIVE in data:
-            active = data.get(API_ACTIVE)
+            active = parse_bool(data.get(API_ACTIVE))
             if active is not None:
-                self.active = bool(active)
+                self.active = active
             else:
                 # API sends active as null instead of False
                 self.active = False
         else:
             if update.get_type() != UpdateType.WS_PARTIAL:
                 self.active = None
 
-        aq_active = data.get(API_AQ_ACTIVE)
+        aq_active = parse_bool(data.get(API_AQ_ACTIVE))
         if aq_active is not None:
-            self.aq_active = bool(aq_active)
+            self.aq_active = aq_active
 
         aq_mode_conf = data.get(API_AQ_MODE_CONF)
         if aq_mode_conf is not None:
             self.aq_mode_conf = AirQualityMode(aq_mode_conf)
 
         aq_mode_values = data.get(API_AQ_MODE_VALUES)
         if aq_mode_values is not None:
             self.aq_mode_values = []
             for aq_mode_value in aq_mode_values:
                 self.aq_mode_values += [AirQualityMode(aq_mode_value)]
 
-        humidity = data.get(API_HUMIDITY)
+        humidity = parse_int(data.get(API_HUMIDITY))
         if humidity is not None:
-            self.humidity = int(humidity)
+            self.humidity = humidity
 
-        local_temp = data.get(API_LOCAL_TEMP)
+        local_temp = parse_float(data.get(API_LOCAL_TEMP, {}).get(API_CELSIUS))
         if local_temp is not None:
-            if API_CELSIUS in local_temp:
-                self.temp = float(local_temp[API_CELSIUS])
+            self.temp = local_temp
 
-        power = data.get(API_POWER)
+        power = parse_bool(data.get(API_POWER))
         if power is not None:
-            self.power = bool(power)
+            self.power = power
 
-        range_max_air = data.get(API_RANGE_MAX_AIR)
+        range_max_air = parse_float(data.get(API_RANGE_MAX_AIR, {}).get(API_CELSIUS))
         if range_max_air is not None:
-            if API_CELSIUS in range_max_air:
-                self.temp_set_max = float(range_max_air[API_CELSIUS])
-        range_sp_max_auto_air = data.get(API_RANGE_SP_MAX_AUTO_AIR)
+            self.temp_set_max = range_max_air
+        range_sp_max_auto_air = parse_float(
+            data.get(API_RANGE_SP_MAX_AUTO_AIR, {}).get(API_CELSIUS)
+        )
         if range_sp_max_auto_air is not None:
-            if API_CELSIUS in range_sp_max_auto_air:
-                self.temp_set_max_auto_air = float(range_sp_max_auto_air[API_CELSIUS])
-        range_sp_max_cool_air = data.get(API_RANGE_SP_MAX_COOL_AIR)
+            self.temp_set_max_auto_air = range_sp_max_auto_air
+        range_sp_max_cool_air = parse_float(
+            data.get(API_RANGE_SP_MAX_COOL_AIR, {}).get(API_CELSIUS)
+        )
         if range_sp_max_cool_air is not None:
-            if API_CELSIUS in range_sp_max_cool_air:
-                self.temp_set_max_cool_air = float(range_sp_max_cool_air[API_CELSIUS])
-        range_sp_max_dry_air = data.get(API_RANGE_SP_MAX_DRY_AIR)
+            self.temp_set_max_cool_air = range_sp_max_cool_air
+        range_sp_max_dry_air = parse_float(
+            data.get(API_RANGE_SP_MAX_DRY_AIR, {}).get(API_CELSIUS)
+        )
         if range_sp_max_dry_air is not None:
-            if API_CELSIUS in range_sp_max_dry_air:
-                self.temp_set_max_dry_air = float(range_sp_max_dry_air[API_CELSIUS])
-        range_sp_max_emerheat_air = data.get(API_RANGE_SP_MAX_EMERHEAT_AIR)
+            self.temp_set_max_dry_air = range_sp_max_dry_air
+        range_sp_max_emerheat_air = parse_float(
+            data.get(API_RANGE_SP_MAX_EMERHEAT_AIR, {}).get(API_CELSIUS)
+        )
         if range_sp_max_emerheat_air is not None:
-            if API_CELSIUS in range_sp_max_emerheat_air:
-                self.temp_set_max_emerheat_air = float(
-                    range_sp_max_emerheat_air[API_CELSIUS]
-                )
-        range_sp_max_hot_air = data.get(API_RANGE_SP_MAX_HOT_AIR)
+            self.temp_set_max_emerheat_air = range_sp_max_emerheat_air
+        range_sp_max_hot_air = parse_float(
+            data.get(API_RANGE_SP_MAX_HOT_AIR, {}).get(API_CELSIUS)
+        )
         if range_sp_max_hot_air is not None:
-            if API_CELSIUS in range_sp_max_hot_air:
-                self.temp_set_max_hot_air = float(range_sp_max_hot_air[API_CELSIUS])
-        range_sp_max_stop_air = data.get(API_RANGE_SP_MAX_STOP_AIR)
+            self.temp_set_max_hot_air = range_sp_max_hot_air
+        range_sp_max_stop_air = parse_float(
+            data.get(API_RANGE_SP_MAX_STOP_AIR, {}).get(API_CELSIUS)
+        )
         if range_sp_max_stop_air is not None:
-            if API_CELSIUS in range_sp_max_stop_air:
-                self.temp_set_max_stop_air = float(range_sp_max_stop_air[API_CELSIUS])
-        range_sp_max_vent_air = data.get(API_RANGE_SP_MAX_VENT_AIR)
+            self.temp_set_max_stop_air = range_sp_max_stop_air
+        range_sp_max_vent_air = parse_float(
+            data.get(API_RANGE_SP_MAX_VENT_AIR, {}).get(API_CELSIUS)
+        )
         if range_sp_max_vent_air is not None:
-            if API_CELSIUS in range_sp_max_vent_air:
-                self.temp_set_max_vent_air = float(range_sp_max_vent_air[API_CELSIUS])
+            self.temp_set_max_vent_air = range_sp_max_vent_air
 
-        range_min_air = data.get(API_RANGE_MIN_AIR)
+        range_min_air = parse_float(data.get(API_RANGE_MIN_AIR, {}).get(API_CELSIUS))
         if range_min_air is not None:
-            if API_CELSIUS in range_min_air:
-                self.temp_set_min = float(range_min_air[API_CELSIUS])
-        range_sp_min_auto_air = data.get(API_RANGE_SP_MIN_AUTO_AIR)
+            self.temp_set_min = range_min_air
+        range_sp_min_auto_air = parse_float(
+            data.get(API_RANGE_SP_MIN_AUTO_AIR, {}).get(API_CELSIUS)
+        )
         if range_sp_min_auto_air is not None:
-            if API_CELSIUS in range_sp_min_auto_air:
-                self.temp_set_min_auto_air = float(range_sp_min_auto_air[API_CELSIUS])
-        range_sp_min_cool_air = data.get(API_RANGE_SP_MIN_COOL_AIR)
+            self.temp_set_min_auto_air = range_sp_min_auto_air
+        range_sp_min_cool_air = parse_float(
+            data.get(API_RANGE_SP_MIN_COOL_AIR, {}).get(API_CELSIUS)
+        )
         if range_sp_min_cool_air is not None:
-            if API_CELSIUS in range_sp_min_cool_air:
-                self.temp_set_min_cool_air = float(range_sp_min_cool_air[API_CELSIUS])
-        range_sp_min_dry_air = data.get(API_RANGE_SP_MIN_DRY_AIR)
+            self.temp_set_min_cool_air = range_sp_min_cool_air
+        range_sp_min_dry_air = parse_float(
+            data.get(API_RANGE_SP_MIN_DRY_AIR, {}).get(API_CELSIUS)
+        )
         if range_sp_min_dry_air is not None:
-            if API_CELSIUS in range_sp_min_dry_air:
-                self.temp_set_min_dry_air = float(range_sp_min_dry_air[API_CELSIUS])
-        range_sp_min_emerheat_air = data.get(API_RANGE_SP_MIN_EMERHEAT_AIR)
+            self.temp_set_min_dry_air = range_sp_min_dry_air
+        range_sp_min_emerheat_air = parse_float(
+            data.get(API_RANGE_SP_MIN_EMERHEAT_AIR, {}).get(API_CELSIUS)
+        )
         if range_sp_min_emerheat_air is not None:
-            if API_CELSIUS in range_sp_min_emerheat_air:
-                self.temp_set_min_emerheat_air = float(
-                    range_sp_min_emerheat_air[API_CELSIUS]
-                )
-        range_sp_min_hot_air = data.get(API_RANGE_SP_MIN_HOT_AIR)
+            self.temp_set_min_emerheat_air = range_sp_min_emerheat_air
+        range_sp_min_hot_air = parse_float(
+            data.get(API_RANGE_SP_MIN_HOT_AIR, {}).get(API_CELSIUS)
+        )
         if range_sp_min_hot_air is not None:
-            if API_CELSIUS in range_sp_min_hot_air:
-                self.temp_set_min_hot_air = float(range_sp_min_hot_air[API_CELSIUS])
-        range_sp_min_stop_air = data.get(API_RANGE_SP_MIN_STOP_AIR)
+            self.temp_set_min_hot_air = range_sp_min_hot_air
+        range_sp_min_stop_air = parse_float(
+            data.get(API_RANGE_SP_MIN_STOP_AIR, {}).get(API_CELSIUS)
+        )
         if range_sp_min_stop_air is not None:
-            if API_CELSIUS in range_sp_min_stop_air:
-                self.temp_set_min_stop_air = float(range_sp_min_stop_air[API_CELSIUS])
-        range_sp_min_vent_air = data.get(API_RANGE_SP_MIN_VENT_AIR)
+            self.temp_set_min_stop_air = range_sp_min_stop_air
+        range_sp_min_vent_air = parse_float(
+            data.get(API_RANGE_SP_MIN_VENT_AIR, {}).get(API_CELSIUS)
+        )
         if range_sp_min_vent_air is not None:
-            if API_CELSIUS in range_sp_min_vent_air:
-                self.temp_set_min_vent_air = float(range_sp_min_vent_air[API_CELSIUS])
+            self.temp_set_min_vent_air = range_sp_min_vent_air
 
-        sp_air_cool = data.get(API_SP_AIR_COOL)
+        sp_air_cool = parse_float(data.get(API_SP_AIR_COOL, {}).get(API_CELSIUS))
         if sp_air_cool is not None:
-            if API_CELSIUS in sp_air_cool:
-                self.temp_set_cool_air = float(sp_air_cool[API_CELSIUS])
-        sp_air_dry = data.get(API_SP_AIR_DRY)
+            self.temp_set_cool_air = sp_air_cool
+        sp_air_dry = parse_float(data.get(API_SP_AIR_DRY, {}).get(API_CELSIUS))
         if sp_air_dry is not None:
-            if API_CELSIUS in sp_air_dry:
-                self.temp_set_dry_air = float(data[API_SP_AIR_DRY][API_CELSIUS])
-        sp_air_heat = data.get(API_SP_AIR_HEAT)
+            self.temp_set_dry_air = sp_air_dry
+        sp_air_heat = parse_float(data.get(API_SP_AIR_HEAT, {}).get(API_CELSIUS))
         if sp_air_heat is not None:
-            if API_CELSIUS in sp_air_heat:
-                self.temp_set_hot_air = float(sp_air_heat[API_CELSIUS])
-        sp_air_stop = data.get(API_SP_AIR_STOP)
+            self.temp_set_hot_air = sp_air_heat
+        sp_air_stop = parse_float(data.get(API_SP_AIR_STOP, {}).get(API_CELSIUS))
         if sp_air_stop is not None:
-            if API_CELSIUS in sp_air_stop:
-                self.temp_set_stop_air = float(sp_air_stop[API_CELSIUS])
-        sp_air_vent = data.get(API_SP_AIR_VENT)
+            self.temp_set_stop_air = sp_air_stop
+        sp_air_vent = parse_float(data.get(API_SP_AIR_VENT, {}).get(API_CELSIUS))
         if sp_air_vent is not None:
-            if API_CELSIUS in sp_air_vent:
-                self.temp_set_vent_air = float(sp_air_vent[API_CELSIUS])
+            self.temp_set_vent_air = sp_air_vent
 
-        step = data.get(API_STEP)
+        step = parse_float(data.get(API_STEP, {}).get(API_CELSIUS))
         if step is not None:
-            if API_CELSIUS in step:
-                self.temp_step = float(step[API_CELSIUS])
+            self.temp_step = step
```

### Comparing `aioairzone-cloud-0.4.6/aioairzone_cloud/installation.py` & `aioairzone-cloud-0.4.7/aioairzone_cloud/installation.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.4.6/aioairzone_cloud/system.py` & `aioairzone-cloud-0.4.7/aioairzone_cloud/system.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.4.6/aioairzone_cloud/token.py` & `aioairzone-cloud-0.4.7/aioairzone_cloud/token.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.4.6/aioairzone_cloud/webserver.py` & `aioairzone-cloud-0.4.7/aioairzone_cloud/webserver.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Airzone Cloud Local API based device."""
 
 from __future__ import annotations
 
 import logging
 from typing import Any
 
+from .common import parse_bool, parse_int, parse_str
 from .const import (
     API_CONFIG,
     API_CONNECTION_DATE,
     API_DISCONNECTION_DATE,
     API_IS_CONNECTED,
     API_STAT_AP_MAC,
     API_STAT_CHANNEL,
@@ -59,50 +60,50 @@
         self.wifi_rssi: int | None = None
         self.wifi_ssid: str | None = None
 
     def update_data(self, update: EntityUpdate) -> None:
         """Update WebServer data."""
         data = update.get_data()
 
-        ws_type = data.get(API_WS_TYPE)
+        ws_type = parse_str(data.get(API_WS_TYPE))
         if ws_type is not None:
-            self.type = str(ws_type)
+            self.type = ws_type
 
         ws_config = data.get(API_CONFIG)
         if ws_config is not None:
-            stat_ap_mac = ws_config.get(API_STAT_AP_MAC)
+            stat_ap_mac = parse_str(ws_config.get(API_STAT_AP_MAC))
             if stat_ap_mac is not None:
-                self.wifi_mac = str(stat_ap_mac)
-            stat_channel = ws_config.get(API_STAT_CHANNEL)
+                self.wifi_mac = stat_ap_mac
+            stat_channel = parse_int(ws_config.get(API_STAT_CHANNEL))
             if stat_channel is not None:
-                self.wifi_channel = int(stat_channel)
-            stat_ssid = ws_config.get(API_STAT_SSID)
+                self.wifi_channel = stat_channel
+            stat_ssid = parse_str(ws_config.get(API_STAT_SSID))
             if stat_ssid is not None:
-                self.wifi_ssid = str(stat_ssid)
-            ws_fw = ws_config.get(API_WS_FW)
+                self.wifi_ssid = stat_ssid
+            ws_fw = parse_str(ws_config.get(API_WS_FW))
             if ws_fw is not None:
-                self.firmware = str(ws_fw)
+                self.firmware = ws_fw
 
         ws_status = data.get(API_STATUS)
         if ws_status is not None:
-            connection_date = ws_status.get(API_CONNECTION_DATE)
+            connection_date = parse_str(ws_status.get(API_CONNECTION_DATE))
             if connection_date is not None:
-                self.connection_date = str(connection_date)
-            disconnection_date = ws_status.get(API_DISCONNECTION_DATE)
+                self.connection_date = connection_date
+            disconnection_date = parse_str(ws_status.get(API_DISCONNECTION_DATE))
             if disconnection_date is not None:
-                self.disconnection_date = str(disconnection_date)
-            is_connected = ws_status.get(API_IS_CONNECTED)
+                self.disconnection_date = disconnection_date
+            is_connected = parse_bool(ws_status.get(API_IS_CONNECTED))
             if is_connected is not None:
-                self.is_connected = bool(is_connected)
-            stat_quality = ws_status.get(API_STAT_QUALITY)
+                self.is_connected = is_connected
+            stat_quality = parse_int(ws_status.get(API_STAT_QUALITY))
             if stat_quality is not None:
-                self.wifi_quality = int(stat_quality)
-            stat_rssi = ws_status.get(API_STAT_RSSI)
+                self.wifi_quality = stat_quality
+            stat_rssi = parse_int(ws_status.get(API_STAT_RSSI))
             if stat_rssi is not None:
-                self.wifi_rssi = int(stat_rssi)
+                self.wifi_rssi = stat_rssi
 
     def data(self) -> dict[str, Any]:
         """Return WebServer data."""
         data: dict[str, Any] = {
             AZD_AVAILABLE: self.get_available(),
             AZD_CONNECTION_DATE: self.get_connection_date(),
             AZD_DISCONNECTION_DATE: self.get_disconnection_date(),
```

### Comparing `aioairzone-cloud-0.4.6/aioairzone_cloud/websockets.py` & `aioairzone-cloud-0.4.7/aioairzone_cloud/websockets.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.4.6/aioairzone_cloud/zone.py` & `aioairzone-cloud-0.4.7/aioairzone_cloud/zone.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 from aioairzone_cloud.common import OperationMode
 
+from .common import parse_str
 from .const import (
     API_AQ_MODE_CONF,
     API_MODE,
     API_MODE_AVAIL,
     API_NAME,
     API_POWER,
     API_SETPOINT,
@@ -38,16 +39,17 @@
         self.master: bool | None = None
         self.system: System | None = None
 
         sub_data = self.sub_data(device_data)
         self.system_number = int(sub_data[API_SYSTEM_NUMBER])
         self.zone_number = int(sub_data[API_ZONE_NUMBER])
 
-        if API_NAME in device_data:
-            self.name = str(device_data[API_NAME])
+        device_name = parse_str(device_data.get(API_NAME))
+        if device_name is not None:
+            self.name = device_name
         else:
             self.name = f"Zone {self.system_number}:{self.zone_number}"
 
     def data(self) -> dict[str, Any]:
         """Return Zone data."""
         data = super().data()
```

### Comparing `aioairzone-cloud-0.4.6/aioairzone_cloud.egg-info/PKG-INFO` & `aioairzone-cloud-0.4.7/aioairzone_cloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioairzone-cloud
-Version: 0.4.6
+Version: 0.4.7
 Summary: Library to control Airzone Cloud devices
 Author-email: Álvaro Fernández Rojas <noltari@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Noltari/aioairzone-cloud
 Project-URL: Bug Tracker, https://github.com/Noltari/aioairzone-cloud/issues
 Keywords: airzone,cloud,hvac,home
 Platform: any
```

### Comparing `aioairzone-cloud-0.4.6/aioairzone_cloud.egg-info/SOURCES.txt` & `aioairzone-cloud-0.4.7/aioairzone_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.4.6/pyproject.toml` & `aioairzone-cloud-0.4.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "aioairzone-cloud"
-version = "0.4.6"
+version = "0.4.7"
 description = "Library to control Airzone Cloud devices"
 readme = "README.md"
 requires-python = ">=3.11"
 license = {text = "Apache-2.0"}
 keywords = ["airzone", "cloud", "hvac", "home"] 
 authors = [
   {name = "Álvaro Fernández Rojas", email = "noltari@gmail.com" }
```

