# Comparing `tmp/lmcloud-1.1.7.tar.gz` & `tmp/lmcloud-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmcloud-1.1.7.tar", last modified: Tue Apr  2 07:46:28 2024, max compression
+gzip compressed data, was "lmcloud-1.1.8.tar", last modified: Wed Apr  3 06:42:23 2024, max compression
```

## Comparing `lmcloud-1.1.7.tar` & `lmcloud-1.1.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:46:28.240892 lmcloud-1.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-02 07:46:09.000000 lmcloud-1.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-04-02 07:46:28.236892 lmcloud-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-04-02 07:46:09.000000 lmcloud-1.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:46:28.236892 lmcloud-1.1.7/lmcloud/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-02 07:46:09.000000 lmcloud-1.1.7/lmcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-02 07:46:09.000000 lmcloud-1.1.7/lmcloud/client_bluetooth.py
--rw-r--r--   0 runner    (1001) docker     (127)    14859 2024-04-02 07:46:09.000000 lmcloud-1.1.7/lmcloud/client_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-04-02 07:46:09.000000 lmcloud-1.1.7/lmcloud/client_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-04-02 07:46:09.000000 lmcloud-1.1.7/lmcloud/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-02 07:46:09.000000 lmcloud-1.1.7/lmcloud/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6866 2024-04-02 07:46:09.000000 lmcloud-1.1.7/lmcloud/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-04-02 07:46:09.000000 lmcloud-1.1.7/lmcloud/lm_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-02 07:46:09.000000 lmcloud-1.1.7/lmcloud/lm_grinder.py
--rw-r--r--   0 runner    (1001) docker     (127)    17749 2024-04-02 07:46:09.000000 lmcloud-1.1.7/lmcloud/lm_machine.py
--rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-04-02 07:46:09.000000 lmcloud-1.1.7/lmcloud/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 07:46:09.000000 lmcloud-1.1.7/lmcloud/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:46:28.236892 lmcloud-1.1.7/lmcloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-04-02 07:46:28.000000 lmcloud-1.1.7/lmcloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-02 07:46:28.000000 lmcloud-1.1.7/lmcloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 07:46:28.000000 lmcloud-1.1.7/lmcloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-02 07:46:28.000000 lmcloud-1.1.7/lmcloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-02 07:46:28.000000 lmcloud-1.1.7/lmcloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 07:46:28.240892 lmcloud-1.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-02 07:46:09.000000 lmcloud-1.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:46:28.236892 lmcloud-1.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-02 07:46:09.000000 lmcloud-1.1.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-02 07:46:09.000000 lmcloud-1.1.7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-02 07:46:09.000000 lmcloud-1.1.7/tests/test_grinder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6407 2024-04-02 07:46:09.000000 lmcloud-1.1.7/tests/test_machine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:42:23.841335 lmcloud-1.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-03 06:42:05.000000 lmcloud-1.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-04-03 06:42:23.841335 lmcloud-1.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-04-03 06:42:05.000000 lmcloud-1.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:42:23.841335 lmcloud-1.1.8/lmcloud/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-03 06:42:05.000000 lmcloud-1.1.8/lmcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-03 06:42:05.000000 lmcloud-1.1.8/lmcloud/client_bluetooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14859 2024-04-03 06:42:05.000000 lmcloud-1.1.8/lmcloud/client_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-04-03 06:42:05.000000 lmcloud-1.1.8/lmcloud/client_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-04-03 06:42:05.000000 lmcloud-1.1.8/lmcloud/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-03 06:42:05.000000 lmcloud-1.1.8/lmcloud/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-04-03 06:42:05.000000 lmcloud-1.1.8/lmcloud/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-04-03 06:42:05.000000 lmcloud-1.1.8/lmcloud/lm_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-03 06:42:05.000000 lmcloud-1.1.8/lmcloud/lm_grinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17615 2024-04-03 06:42:05.000000 lmcloud-1.1.8/lmcloud/lm_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-04-03 06:42:05.000000 lmcloud-1.1.8/lmcloud/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:42:05.000000 lmcloud-1.1.8/lmcloud/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:42:23.841335 lmcloud-1.1.8/lmcloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-04-03 06:42:23.000000 lmcloud-1.1.8/lmcloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-03 06:42:23.000000 lmcloud-1.1.8/lmcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 06:42:23.000000 lmcloud-1.1.8/lmcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-03 06:42:23.000000 lmcloud-1.1.8/lmcloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-03 06:42:23.000000 lmcloud-1.1.8/lmcloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 06:42:23.841335 lmcloud-1.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-03 06:42:05.000000 lmcloud-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:42:23.841335 lmcloud-1.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-03 06:42:05.000000 lmcloud-1.1.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-03 06:42:05.000000 lmcloud-1.1.8/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-03 06:42:05.000000 lmcloud-1.1.8/tests/test_grinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6407 2024-04-03 06:42:05.000000 lmcloud-1.1.8/tests/test_machine.py
```

### Comparing `lmcloud-1.1.7/LICENSE` & `lmcloud-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lmcloud-1.1.7/PKG-INFO` & `lmcloud-1.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmcloud
-Version: 1.1.7
+Version: 1.1.8
 Summary: A Python implementation of the new La Marzocco API
 Home-page: https://github.com/zweckj/lmcloud
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `lmcloud-1.1.7/README.md` & `lmcloud-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `lmcloud-1.1.7/lmcloud/client_bluetooth.py` & `lmcloud-1.1.8/lmcloud/client_bluetooth.py`

 * *Files identical despite different names*

### Comparing `lmcloud-1.1.7/lmcloud/client_cloud.py` & `lmcloud-1.1.8/lmcloud/client_cloud.py`

 * *Files identical despite different names*

### Comparing `lmcloud-1.1.7/lmcloud/client_local.py` & `lmcloud-1.1.8/lmcloud/client_local.py`

 * *Files identical despite different names*

### Comparing `lmcloud-1.1.7/lmcloud/const.py` & `lmcloud-1.1.8/lmcloud/const.py`

 * *Files identical despite different names*

### Comparing `lmcloud-1.1.7/lmcloud/exceptions.py` & `lmcloud-1.1.8/lmcloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `lmcloud-1.1.7/lmcloud/helpers.py` & `lmcloud-1.1.8/lmcloud/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -191,22 +191,21 @@
         minutes=smart_standby_config.get("minutes", 10),
         mode=SmartStandbyMode(smart_standby_config.get("mode", "PowerOn")),
     )
 
 
 def parse_wakeup_sleep_entries(
     entries: list[dict[str, Any]]
-) -> list[LaMarzoccoWakeUpSleepEntry]:
+) -> dict[str, LaMarzoccoWakeUpSleepEntry]:
     """Parse wake up sleep entries from API config object."""
-    parsed = []
+    parsed = {}
     for entry in entries:
-        parsed.append(
-            LaMarzoccoWakeUpSleepEntry(
-                enabled=entry["enabled"],
-                days=[WeekDay(day) for day in entry["days"]],
-                entry_id=entry["id"],
-                steam=entry["steam"],
-                time_on=entry["timeOn"],
-                time_off=entry["timeOff"],
-            )
+        wake_up_sleep_entry = LaMarzoccoWakeUpSleepEntry(
+            enabled=entry["enabled"],
+            days=[WeekDay(day) for day in entry["days"]],
+            entry_id=entry["id"],
+            steam=entry["steam"],
+            time_on=entry["timeOn"],
+            time_off=entry["timeOff"],
         )
+        parsed[wake_up_sleep_entry.entry_id] = wake_up_sleep_entry
     return parsed
```

### Comparing `lmcloud-1.1.7/lmcloud/lm_device.py` & `lmcloud-1.1.8/lmcloud/lm_device.py`

 * *Files identical despite different names*

### Comparing `lmcloud-1.1.7/lmcloud/lm_grinder.py` & `lmcloud-1.1.8/lmcloud/lm_grinder.py`

 * *Files identical despite different names*

### Comparing `lmcloud-1.1.7/lmcloud/lm_machine.py` & `lmcloud-1.1.8/lmcloud/lm_machine.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
             brew_active=False,
             brew_active_duration=0,
             smart_standby=LaMarzoccoSmartStandby(
                 enabled=False,
                 minutes=10,
                 mode=SmartStandbyMode.POWER_ON,
             ),
-            wake_up_sleep_entries=[],
+            wake_up_sleep_entries={},
         )
         self.statistics: LaMarzoccoCoffeeStatistics = LaMarzoccoCoffeeStatistics(
             drink_stats={},
             continous=0,
             total_flushes=0,
         )
 
@@ -336,18 +336,16 @@
 
     async def set_wake_up_sleep(self, wake_up_sleep_entry: LaMarzoccoWakeUpSleepEntry):
         """Set wake up sleep"""
 
         if await self.cloud_client.set_wake_up_sleep(
             self.serial_number, wake_up_sleep_entry
         ):
-            for idx, entry in enumerate(self.config.wake_up_sleep_entries):
-                if entry.entry_id == wake_up_sleep_entry.entry_id:
-                    self.config.wake_up_sleep_entries[idx] = wake_up_sleep_entry
-                    return True
+            self.config.wake_up_sleep_entries[wake_up_sleep_entry.entry_id] = wake_up_sleep_entry
+            return True
         return False
 
     async def set_smart_standby(
         self, enabled: bool, minutes: int, mode: SmartStandbyMode
     ) -> bool:
         """Set smart standby"""
```

### Comparing `lmcloud-1.1.7/lmcloud/models.py` & `lmcloud-1.1.8/lmcloud/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
 
     boilers: dict[BoilerType, LaMarzoccoBoiler]
     prebrew_mode: PrebrewMode
     plumbed_in: bool
     prebrew_configuration: dict[PhysicalKey, LaMarzoccoPrebrewConfiguration]
     dose_hot_water: int
     water_contact: bool
-    wake_up_sleep_entries: list[LaMarzoccoWakeUpSleepEntry]
+    wake_up_sleep_entries: dict[str, LaMarzoccoWakeUpSleepEntry]
     smart_standby: LaMarzoccoSmartStandby
     brew_active: bool
     brew_active_duration: float
 
     @property
     def steam_level(self) -> SteamLevel:
         """Return the steam level"""
```

### Comparing `lmcloud-1.1.7/lmcloud.egg-info/PKG-INFO` & `lmcloud-1.1.8/lmcloud.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmcloud
-Version: 1.1.7
+Version: 1.1.8
 Summary: A Python implementation of the new La Marzocco API
 Home-page: https://github.com/zweckj/lmcloud
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `lmcloud-1.1.7/lmcloud.egg-info/SOURCES.txt` & `lmcloud-1.1.8/lmcloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lmcloud-1.1.7/setup.py` & `lmcloud-1.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools  # type: ignore[import]
 
 with open("README.md", "r", encoding="utf-8") as f:
     readme = f.read()
 
 setuptools.setup(
     name="lmcloud",
-    version="1.1.7",
+    version="1.1.8",
     description="A Python implementation of the new La Marzocco API",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/zweckj/lmcloud",
     author="Josef Zweck",
     author_email="24647999+zweckj@users.noreply.github.com",
     license="MIT",
```

### Comparing `lmcloud-1.1.7/tests/__init__.py` & `lmcloud-1.1.8/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `lmcloud-1.1.7/tests/conftest.py` & `lmcloud-1.1.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lmcloud-1.1.7/tests/test_grinder.py` & `lmcloud-1.1.8/tests/test_grinder.py`

 * *Files identical despite different names*

### Comparing `lmcloud-1.1.7/tests/test_machine.py` & `lmcloud-1.1.8/tests/test_machine.py`

 * *Files identical despite different names*

