# Comparing `tmp/dirigera-1.0.8.tar.gz` & `tmp/dirigera-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dirigera-1.0.8.tar", last modified: Fri Feb 16 07:41:10 2024, max compression
+gzip compressed data, was "dirigera-1.0.9.tar", last modified: Thu Feb 22 08:07:21 2024, max compression
```

## Comparing `dirigera-1.0.8.tar` & `dirigera-1.0.9.tar`

### file list

```diff
@@ -1,44 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 07:41:10.090689 dirigera-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-02-16 07:41:02.000000 dirigera-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13378 2024-02-16 07:41:10.090689 dirigera-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11147 2024-02-16 07:41:02.000000 dirigera-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-02-16 07:41:02.000000 dirigera-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-16 07:41:10.094689 dirigera-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-16 07:41:02.000000 dirigera-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 07:41:10.086689 dirigera-1.0.8/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 07:41:02.000000 dirigera-1.0.8/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 07:41:10.086689 dirigera-1.0.8/src/dirigera/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-16 07:41:02.000000 dirigera-1.0.8/src/dirigera/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 07:41:10.090689 dirigera-1.0.8/src/dirigera/devices/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 07:41:02.000000 dirigera-1.0.8/src/dirigera/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-02-16 07:41:02.000000 dirigera-1.0.8/src/dirigera/devices/base_ikea_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-02-16 07:41:02.000000 dirigera-1.0.8/src/dirigera/devices/blinds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-02-16 07:41:02.000000 dirigera-1.0.8/src/dirigera/devices/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-02-16 07:41:02.000000 dirigera-1.0.8/src/dirigera/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-02-16 07:41:02.000000 dirigera-1.0.8/src/dirigera/devices/environment_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-02-16 07:41:02.000000 dirigera-1.0.8/src/dirigera/devices/light.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-02-16 07:41:02.000000 dirigera-1.0.8/src/dirigera/devices/motion_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-02-16 07:41:02.000000 dirigera-1.0.8/src/dirigera/devices/open_close_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-02-16 07:41:02.000000 dirigera-1.0.8/src/dirigera/devices/outlet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-02-16 07:41:02.000000 dirigera-1.0.8/src/dirigera/devices/scene.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 07:41:10.090689 dirigera-1.0.8/src/dirigera/hub/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 07:41:02.000000 dirigera-1.0.8/src/dirigera/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-02-16 07:41:02.000000 dirigera-1.0.8/src/dirigera/hub/abstract_smart_home_hub.py
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-02-16 07:41:02.000000 dirigera-1.0.8/src/dirigera/hub/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    10085 2024-02-16 07:41:02.000000 dirigera-1.0.8/src/dirigera/hub/hub.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 07:41:10.090689 dirigera-1.0.8/src/dirigera.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13378 2024-02-16 07:41:10.000000 dirigera-1.0.8/src/dirigera.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-02-16 07:41:10.000000 dirigera-1.0.8/src/dirigera.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 07:41:10.000000 dirigera-1.0.8/src/dirigera.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-16 07:41:10.000000 dirigera-1.0.8/src/dirigera.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-16 07:41:10.000000 dirigera-1.0.8/src/dirigera.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-16 07:41:10.000000 dirigera-1.0.8/src/dirigera.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 07:41:10.090689 dirigera-1.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-02-16 07:41:02.000000 dirigera-1.0.8/tests/test_blinds.py
--rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-02-16 07:41:02.000000 dirigera-1.0.8/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-02-16 07:41:02.000000 dirigera-1.0.8/tests/test_environment_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    12981 2024-02-16 07:41:02.000000 dirigera-1.0.8/tests/test_light.py
--rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-02-16 07:41:02.000000 dirigera-1.0.8/tests/test_motion_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-02-16 07:41:02.000000 dirigera-1.0.8/tests/test_open_close_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-02-16 07:41:02.000000 dirigera-1.0.8/tests/test_outlet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-02-16 07:41:02.000000 dirigera-1.0.8/tests/test_scenes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 08:07:21.334338 dirigera-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-02-22 08:07:07.000000 dirigera-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14278 2024-02-22 08:07:21.330338 dirigera-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12047 2024-02-22 08:07:07.000000 dirigera-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-02-22 08:07:07.000000 dirigera-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-22 08:07:21.334338 dirigera-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-22 08:07:07.000000 dirigera-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 08:07:21.326338 dirigera-1.0.9/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 08:07:07.000000 dirigera-1.0.9/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 08:07:21.326338 dirigera-1.0.9/src/dirigera/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-22 08:07:07.000000 dirigera-1.0.9/src/dirigera/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 08:07:21.330338 dirigera-1.0.9/src/dirigera/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 08:07:07.000000 dirigera-1.0.9/src/dirigera/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-02-22 08:07:07.000000 dirigera-1.0.9/src/dirigera/devices/air_purifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-02-22 08:07:07.000000 dirigera-1.0.9/src/dirigera/devices/base_ikea_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-02-22 08:07:07.000000 dirigera-1.0.9/src/dirigera/devices/blinds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-02-22 08:07:07.000000 dirigera-1.0.9/src/dirigera/devices/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-02-22 08:07:07.000000 dirigera-1.0.9/src/dirigera/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-02-22 08:07:07.000000 dirigera-1.0.9/src/dirigera/devices/environment_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-02-22 08:07:07.000000 dirigera-1.0.9/src/dirigera/devices/light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-02-22 08:07:07.000000 dirigera-1.0.9/src/dirigera/devices/motion_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-02-22 08:07:07.000000 dirigera-1.0.9/src/dirigera/devices/open_close_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-02-22 08:07:07.000000 dirigera-1.0.9/src/dirigera/devices/outlet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-02-22 08:07:07.000000 dirigera-1.0.9/src/dirigera/devices/scene.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 08:07:21.330338 dirigera-1.0.9/src/dirigera/hub/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 08:07:07.000000 dirigera-1.0.9/src/dirigera/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-02-22 08:07:07.000000 dirigera-1.0.9/src/dirigera/hub/abstract_smart_home_hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-02-22 08:07:07.000000 dirigera-1.0.9/src/dirigera/hub/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10537 2024-02-22 08:07:07.000000 dirigera-1.0.9/src/dirigera/hub/hub.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 08:07:21.330338 dirigera-1.0.9/src/dirigera.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14278 2024-02-22 08:07:21.000000 dirigera-1.0.9/src/dirigera.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-02-22 08:07:21.000000 dirigera-1.0.9/src/dirigera.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 08:07:21.000000 dirigera-1.0.9/src/dirigera.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-22 08:07:21.000000 dirigera-1.0.9/src/dirigera.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-22 08:07:21.000000 dirigera-1.0.9/src/dirigera.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-22 08:07:21.000000 dirigera-1.0.9/src/dirigera.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 08:07:21.330338 dirigera-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-02-22 08:07:07.000000 dirigera-1.0.9/tests/test_air_purifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-02-22 08:07:07.000000 dirigera-1.0.9/tests/test_blinds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-02-22 08:07:07.000000 dirigera-1.0.9/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-02-22 08:07:07.000000 dirigera-1.0.9/tests/test_environment_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12981 2024-02-22 08:07:07.000000 dirigera-1.0.9/tests/test_light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-02-22 08:07:07.000000 dirigera-1.0.9/tests/test_motion_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-02-22 08:07:07.000000 dirigera-1.0.9/tests/test_open_close_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-02-22 08:07:07.000000 dirigera-1.0.9/tests/test_outlet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-02-22 08:07:07.000000 dirigera-1.0.9/tests/test_scenes.py
```

### Comparing `dirigera-1.0.8/LICENSE` & `dirigera-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dirigera-1.0.8/PKG-INFO` & `dirigera-1.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dirigera
-Version: 1.0.8
+Version: 1.0.9
 Summary: An unofficial Python client for controlling the IKEA Dirigera Smart Home Hub
 Author-email: Leggin <legginsun@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Leggin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -52,14 +52,15 @@
 [![Downloads](https://static.pepy.tech/badge/dirigera/month)](https://pepy.tech/project/dirigera)
 ![Downloads](https://img.shields.io/pypi/pyversions/dirigera)
 
 This repository provides an unofficial Python client for controlling the IKEA Dirigera Smart Home Hub. Current features:
 
 - [light control](#controlling-lights)
 - [outlet control](#controlling-outlets)
+- [air purifier control](#controlling-air-purifier)
 - [blinds control](#controlling-blinds)
 - [remote controllers](#remote-controllers) (tested with STYRBAR)
 - [environment sensor](#environment-sensor) (tested with VINDSTYRKA)
 - [scene](#scene)
 - [motion sensor](#motion-sensor)
 - [event listener](#event-listener) for hub events
 
@@ -226,14 +227,52 @@
 outlet.set_name(name="kitchen socket 1")
 
 outlet.set_on(outlet_on=True)
 
 outlet.set_startup_behaviour(behaviour=StartupEnum.START_OFF)
 ```
 
+## [Controlling Air Purifier](./src/dirigera/devices/air_purifier.py)
+
+To get information about the available air purifiers, you can use the `get_air_purifiers()` method:
+
+```python
+air_purifiers = dirigera_hub.get_air_purifiers()
+```
+
+The air purifier object has the following attributes (additional to the core attributes):
+
+```python
+fan_mode: FanModeEnum
+fan_mode_sequence: str
+motor_state: int
+child_lock: bool
+status_light: bool
+motor_runtime: int
+filter_alarm_status: bool
+filter_elapsed_time: int
+filter_lifetime: int
+current_p_m25: int
+```
+
+Available methods for blinds are:
+
+```python
+air_purifier.set_name(name="living room purifier")
+
+air_purifier.set_fan_mode(fan_mode=FanModeEnum.AUTO)
+
+air_purifier.set_motor_state(motor_state=42)
+
+air_purifier.set_child_lock(child_lock=True)
+
+air_purifier.set_status_light(light_state=False)
+```
+
+
 ## [Controlling Blinds](./src/dirigera/devices/blinds.py)
 
 To get information about the available blinds, you can use the `get_blinds()` method:
 
 ```python
 blinds = dirigera_hub.get_blinds()
 ```
```

### Comparing `dirigera-1.0.8/README.md` & `dirigera-1.0.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 [![Downloads](https://static.pepy.tech/badge/dirigera/month)](https://pepy.tech/project/dirigera)
 ![Downloads](https://img.shields.io/pypi/pyversions/dirigera)
 
 This repository provides an unofficial Python client for controlling the IKEA Dirigera Smart Home Hub. Current features:
 
 - [light control](#controlling-lights)
 - [outlet control](#controlling-outlets)
+- [air purifier control](#controlling-air-purifier)
 - [blinds control](#controlling-blinds)
 - [remote controllers](#remote-controllers) (tested with STYRBAR)
 - [environment sensor](#environment-sensor) (tested with VINDSTYRKA)
 - [scene](#scene)
 - [motion sensor](#motion-sensor)
 - [event listener](#event-listener) for hub events
 
@@ -179,14 +180,52 @@
 outlet.set_name(name="kitchen socket 1")
 
 outlet.set_on(outlet_on=True)
 
 outlet.set_startup_behaviour(behaviour=StartupEnum.START_OFF)
 ```
 
+## [Controlling Air Purifier](./src/dirigera/devices/air_purifier.py)
+
+To get information about the available air purifiers, you can use the `get_air_purifiers()` method:
+
+```python
+air_purifiers = dirigera_hub.get_air_purifiers()
+```
+
+The air purifier object has the following attributes (additional to the core attributes):
+
+```python
+fan_mode: FanModeEnum
+fan_mode_sequence: str
+motor_state: int
+child_lock: bool
+status_light: bool
+motor_runtime: int
+filter_alarm_status: bool
+filter_elapsed_time: int
+filter_lifetime: int
+current_p_m25: int
+```
+
+Available methods for blinds are:
+
+```python
+air_purifier.set_name(name="living room purifier")
+
+air_purifier.set_fan_mode(fan_mode=FanModeEnum.AUTO)
+
+air_purifier.set_motor_state(motor_state=42)
+
+air_purifier.set_child_lock(child_lock=True)
+
+air_purifier.set_status_light(light_state=False)
+```
+
+
 ## [Controlling Blinds](./src/dirigera/devices/blinds.py)
 
 To get information about the available blinds, you can use the `get_blinds()` method:
 
 ```python
 blinds = dirigera_hub.get_blinds()
 ```
```

### Comparing `dirigera-1.0.8/pyproject.toml` & `dirigera-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dirigera"
-version = "1.0.8"
+version = "1.0.9"
 description = "An unofficial Python client for controlling the IKEA Dirigera Smart Home Hub"
 readme = "README.md"
 authors = [{ name = "Leggin", email = "legginsun@gmail.com" }]
 license = { file = "LICENSE" }
 keywords = [
     "python",
     "iot",
```

### Comparing `dirigera-1.0.8/src/dirigera/devices/blinds.py` & `dirigera-1.0.9/src/dirigera/devices/blinds.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.0.8/src/dirigera/devices/controller.py` & `dirigera-1.0.9/src/dirigera/devices/controller.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.0.8/src/dirigera/devices/device.py` & `dirigera-1.0.9/src/dirigera/devices/device.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.0.8/src/dirigera/devices/environment_sensor.py` & `dirigera-1.0.9/src/dirigera/devices/environment_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.0.8/src/dirigera/devices/light.py` & `dirigera-1.0.9/src/dirigera/devices/light.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.0.8/src/dirigera/devices/motion_sensor.py` & `dirigera-1.0.9/src/dirigera/devices/motion_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.0.8/src/dirigera/devices/open_close_sensor.py` & `dirigera-1.0.9/src/dirigera/devices/open_close_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.0.8/src/dirigera/devices/outlet.py` & `dirigera-1.0.9/src/dirigera/devices/outlet.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.0.8/src/dirigera/devices/scene.py` & `dirigera-1.0.9/src/dirigera/devices/scene.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.0.8/src/dirigera/hub/abstract_smart_home_hub.py` & `dirigera-1.0.9/src/dirigera/hub/abstract_smart_home_hub.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.0.8/src/dirigera/hub/auth.py` & `dirigera-1.0.9/src/dirigera/hub/auth.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.0.8/src/dirigera/hub/hub.py` & `dirigera-1.0.9/src/dirigera/hub/hub.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import websocket  # type: ignore
 import urllib3
 from requests import HTTPError
 from urllib3.exceptions import InsecureRequestWarning
 
 from ..devices.device import Device
 from .abstract_smart_home_hub import AbstractSmartHomeHub
+from ..devices.air_purifier import AirPurifier, dict_to_air_purifier
 from ..devices.light import Light, dict_to_light
 from ..devices.blinds import Blind, dict_to_blind
 from ..devices.controller import Controller, dict_to_controller
 from ..devices.outlet import Outlet, dict_to_outlet
 from ..devices.environment_sensor import EnvironmentSensor, dict_to_environment_sensor
 from ..devices.motion_sensor import MotionSensor, dict_to_motion_sensor
 from ..devices.open_close_sensor import OpenCloseSensor, dict_to_open_close_sensor
@@ -115,14 +116,22 @@
         try:
             return self.get("/devices/" + id_)
         except HTTPError as err:
             if err.response is not None and err.response.status_code == 404:
                 raise ValueError("Device id not found") from err
             raise err
 
+    def get_air_purifiers(self) -> List[AirPurifier]:
+        """
+        Fetches all air purifiers registered in the Hub
+        """
+        devices = self.get("/devices")
+        airpurifiers = list(filter(lambda x: x["type"] == "airPurifier", devices))
+        return [dict_to_air_purifier(air_p, self) for air_p in airpurifiers]
+
     def get_lights(self) -> List[Light]:
         """
         Fetches all lights registered in the Hub
         """
         devices = self.get("/devices")
         lights = list(filter(lambda x: x["type"] == "light", devices))
         return [dict_to_light(light, self) for light in lights]
@@ -264,14 +273,15 @@
         return dict_to_scene(data, self)
 
     def get_all_devices(self) -> List[Device]:
         """
         Fetches all devices registered in the Hub
         """
         devices: List[Device] = []
+        devices.extend(self.get_air_purifiers())
         devices.extend(self.get_blinds())
         devices.extend(self.get_controllers())
         devices.extend(self.get_environment_sensors())
         devices.extend(self.get_lights())
         devices.extend(self.get_motion_sensors())
         devices.extend(self.get_open_close_sensors())
         devices.extend(self.get_outlets())
```

### Comparing `dirigera-1.0.8/src/dirigera.egg-info/PKG-INFO` & `dirigera-1.0.9/src/dirigera.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dirigera
-Version: 1.0.8
+Version: 1.0.9
 Summary: An unofficial Python client for controlling the IKEA Dirigera Smart Home Hub
 Author-email: Leggin <legginsun@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Leggin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -52,14 +52,15 @@
 [![Downloads](https://static.pepy.tech/badge/dirigera/month)](https://pepy.tech/project/dirigera)
 ![Downloads](https://img.shields.io/pypi/pyversions/dirigera)
 
 This repository provides an unofficial Python client for controlling the IKEA Dirigera Smart Home Hub. Current features:
 
 - [light control](#controlling-lights)
 - [outlet control](#controlling-outlets)
+- [air purifier control](#controlling-air-purifier)
 - [blinds control](#controlling-blinds)
 - [remote controllers](#remote-controllers) (tested with STYRBAR)
 - [environment sensor](#environment-sensor) (tested with VINDSTYRKA)
 - [scene](#scene)
 - [motion sensor](#motion-sensor)
 - [event listener](#event-listener) for hub events
 
@@ -226,14 +227,52 @@
 outlet.set_name(name="kitchen socket 1")
 
 outlet.set_on(outlet_on=True)
 
 outlet.set_startup_behaviour(behaviour=StartupEnum.START_OFF)
 ```
 
+## [Controlling Air Purifier](./src/dirigera/devices/air_purifier.py)
+
+To get information about the available air purifiers, you can use the `get_air_purifiers()` method:
+
+```python
+air_purifiers = dirigera_hub.get_air_purifiers()
+```
+
+The air purifier object has the following attributes (additional to the core attributes):
+
+```python
+fan_mode: FanModeEnum
+fan_mode_sequence: str
+motor_state: int
+child_lock: bool
+status_light: bool
+motor_runtime: int
+filter_alarm_status: bool
+filter_elapsed_time: int
+filter_lifetime: int
+current_p_m25: int
+```
+
+Available methods for blinds are:
+
+```python
+air_purifier.set_name(name="living room purifier")
+
+air_purifier.set_fan_mode(fan_mode=FanModeEnum.AUTO)
+
+air_purifier.set_motor_state(motor_state=42)
+
+air_purifier.set_child_lock(child_lock=True)
+
+air_purifier.set_status_light(light_state=False)
+```
+
+
 ## [Controlling Blinds](./src/dirigera/devices/blinds.py)
 
 To get information about the available blinds, you can use the `get_blinds()` method:
 
 ```python
 blinds = dirigera_hub.get_blinds()
 ```
```

### Comparing `dirigera-1.0.8/src/dirigera.egg-info/SOURCES.txt` & `dirigera-1.0.9/src/dirigera.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -7,28 +7,30 @@
 src/dirigera.egg-info/PKG-INFO
 src/dirigera.egg-info/SOURCES.txt
 src/dirigera.egg-info/dependency_links.txt
 src/dirigera.egg-info/entry_points.txt
 src/dirigera.egg-info/requires.txt
 src/dirigera.egg-info/top_level.txt
 src/dirigera/devices/__init__.py
+src/dirigera/devices/air_purifier.py
 src/dirigera/devices/base_ikea_model.py
 src/dirigera/devices/blinds.py
 src/dirigera/devices/controller.py
 src/dirigera/devices/device.py
 src/dirigera/devices/environment_sensor.py
 src/dirigera/devices/light.py
 src/dirigera/devices/motion_sensor.py
 src/dirigera/devices/open_close_sensor.py
 src/dirigera/devices/outlet.py
 src/dirigera/devices/scene.py
 src/dirigera/hub/__init__.py
 src/dirigera/hub/abstract_smart_home_hub.py
 src/dirigera/hub/auth.py
 src/dirigera/hub/hub.py
+tests/test_air_purifier.py
 tests/test_blinds.py
 tests/test_controller.py
 tests/test_environment_sensor.py
 tests/test_light.py
 tests/test_motion_sensor.py
 tests/test_open_close_sensor.py
 tests/test_outlet.py
```

### Comparing `dirigera-1.0.8/tests/test_blinds.py` & `dirigera-1.0.9/tests/test_blinds.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.0.8/tests/test_controller.py` & `dirigera-1.0.9/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.0.8/tests/test_environment_sensor.py` & `dirigera-1.0.9/tests/test_environment_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.0.8/tests/test_light.py` & `dirigera-1.0.9/tests/test_light.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.0.8/tests/test_motion_sensor.py` & `dirigera-1.0.9/tests/test_motion_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.0.8/tests/test_open_close_sensor.py` & `dirigera-1.0.9/tests/test_open_close_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.0.8/tests/test_outlet.py` & `dirigera-1.0.9/tests/test_outlet.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.0.8/tests/test_scenes.py` & `dirigera-1.0.9/tests/test_scenes.py`

 * *Files identical despite different names*

