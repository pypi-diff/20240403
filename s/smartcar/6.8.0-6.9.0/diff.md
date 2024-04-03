# Comparing `tmp/smartcar-6.8.0.tar.gz` & `tmp/smartcar-6.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/smartcar-6.8.0.tar", last modified: Fri Aug 25 17:15:27 2023, max compression
+gzip compressed data, was "dist/smartcar-6.9.0.tar", last modified: Wed Sep  6 20:29:15 2023, max compression
```

## Comparing `smartcar-6.8.0.tar` & `smartcar-6.9.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-08-25 17:15:27.363447 smartcar-6.8.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1092 2023-08-25 17:14:07.000000 smartcar-6.8.0/LICENSE.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     6381 2023-08-25 17:15:27.363447 smartcar-6.8.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     6101 2023-08-25 17:14:07.000000 smartcar-6.8.0/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       67 2023-08-25 17:15:27.363447 smartcar-6.8.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1215 2023-08-25 17:14:07.000000 smartcar-6.8.0/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-08-25 17:15:27.359447 smartcar-6.8.0/smartcar/
--rw-rw-r--   0 travis    (2000) travis    (2000)      372 2023-08-25 17:14:31.000000 smartcar-6.8.0/smartcar/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9282 2023-08-25 17:14:07.000000 smartcar-6.8.0/smartcar/auth_client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      383 2023-08-25 17:14:07.000000 smartcar-6.8.0/smartcar/config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4118 2023-08-25 17:14:07.000000 smartcar-6.8.0/smartcar/exception.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3867 2023-08-25 17:14:07.000000 smartcar-6.8.0/smartcar/helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12224 2023-08-25 17:14:07.000000 smartcar-6.8.0/smartcar/smartcar.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12490 2023-08-25 17:14:07.000000 smartcar-6.8.0/smartcar/types.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20345 2023-08-25 17:14:07.000000 smartcar-6.8.0/smartcar/vehicle.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-08-25 17:15:27.363447 smartcar-6.8.0/smartcar.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6381 2023-08-25 17:15:27.000000 smartcar-6.8.0/smartcar.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      363 2023-08-25 17:15:27.000000 smartcar-6.8.0/smartcar.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-08-25 17:15:27.000000 smartcar-6.8.0/smartcar.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      100 2023-08-25 17:15:27.000000 smartcar-6.8.0/smartcar.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2023-08-25 17:15:27.000000 smartcar-6.8.0/smartcar.egg-info/top_level.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-09-06 20:29:15.836799 smartcar-6.9.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1092 2023-09-06 20:27:55.000000 smartcar-6.9.0/LICENSE.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6469 2023-09-06 20:29:15.836799 smartcar-6.9.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6189 2023-09-06 20:27:55.000000 smartcar-6.9.0/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)       67 2023-09-06 20:29:15.836799 smartcar-6.9.0/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1215 2023-09-06 20:27:55.000000 smartcar-6.9.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-09-06 20:29:15.836799 smartcar-6.9.0/smartcar/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      372 2023-09-06 20:28:18.000000 smartcar-6.9.0/smartcar/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9282 2023-09-06 20:27:55.000000 smartcar-6.9.0/smartcar/auth_client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      383 2023-09-06 20:27:55.000000 smartcar-6.9.0/smartcar/config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4118 2023-09-06 20:27:55.000000 smartcar-6.9.0/smartcar/exception.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3867 2023-09-06 20:27:55.000000 smartcar-6.9.0/smartcar/helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12224 2023-09-06 20:27:55.000000 smartcar-6.9.0/smartcar/smartcar.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12492 2023-09-06 20:27:55.000000 smartcar-6.9.0/smartcar/types.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20345 2023-09-06 20:27:55.000000 smartcar-6.9.0/smartcar/vehicle.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-09-06 20:29:15.836799 smartcar-6.9.0/smartcar.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6469 2023-09-06 20:29:15.000000 smartcar-6.9.0/smartcar.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      363 2023-09-06 20:29:15.000000 smartcar-6.9.0/smartcar.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-09-06 20:29:15.000000 smartcar-6.9.0/smartcar.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      100 2023-09-06 20:29:15.000000 smartcar-6.9.0/smartcar.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        9 2023-09-06 20:29:15.000000 smartcar-6.9.0/smartcar.egg-info/top_level.txt
```

### Comparing `smartcar-6.8.0/LICENSE.md` & `smartcar-6.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `smartcar-6.8.0/PKG-INFO` & `smartcar-6.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartcar
-Version: 6.8.0
+Version: 6.9.0
 Summary: Smartcar Python SDK
 Home-page: https://github.com/smartcar/python-sdk
 Author: Smartcar
 Author-email: hello@smartcar.com
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -139,14 +139,18 @@
 
 odometer = vehicle.odometer()
 print(odometer.distance)
 
 info = vehicle.info()
 print(info.make)
 print(info.model)
+
+batch = vehicle.batch(paths=['/location'])
+location = batch.location()
+print(location)
 ```
 
 - For a lot more examples on everything you can do with a car, see
   the [smartcar developer docs](https://smartcar.com/docs)
 - For the full SDK reference guide, visit [REFERENCES.md][smartcar-python-sdk-reference]
 
 ## Handling Exceptions
```

### Comparing `smartcar-6.8.0/README.md` & `smartcar-6.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -127,14 +127,18 @@
 
 odometer = vehicle.odometer()
 print(odometer.distance)
 
 info = vehicle.info()
 print(info.make)
 print(info.model)
+
+batch = vehicle.batch(paths=['/location'])
+location = batch.location()
+print(location)
 ```
 
 - For a lot more examples on everything you can do with a car, see
   the [smartcar developer docs](https://smartcar.com/docs)
 - For the full SDK reference guide, visit [REFERENCES.md][smartcar-python-sdk-reference]
 
 ## Handling Exceptions
```

### Comparing `smartcar-6.8.0/setup.py` & `smartcar-6.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `smartcar-6.8.0/smartcar/auth_client.py` & `smartcar-6.9.0/smartcar/auth_client.py`

 * *Files identical despite different names*

### Comparing `smartcar-6.8.0/smartcar/exception.py` & `smartcar-6.9.0/smartcar/exception.py`

 * *Files identical despite different names*

### Comparing `smartcar-6.8.0/smartcar/helpers.py` & `smartcar-6.9.0/smartcar/helpers.py`

 * *Files identical despite different names*

### Comparing `smartcar-6.8.0/smartcar/smartcar.py` & `smartcar-6.9.0/smartcar/smartcar.py`

 * *Files identical despite different names*

### Comparing `smartcar-6.8.0/smartcar/types.py` & `smartcar-6.9.0/smartcar/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -267,34 +267,36 @@
 Response = NamedTuple("Response", [("body", dict), ("meta", namedtuple)])
 
 # ===========================================
 # Lock Status Tuples
 # ===========================================
 
 Door = NamedTuple("Door", [("type", str), ("status", str)])
+
 Window = NamedTuple("Window", [("type", str), ("status", str)])
+
 Sunroof = NamedTuple("Sunroof", [("type", str), ("status", str)])
+
 Storage = NamedTuple("Storage", [("type", str), ("status", str)])
-ChargingPort = NamedTuple("ChargingPort", [("type", str), ("status", str)])
 
+ChargingPort = NamedTuple("ChargingPort", [("type", str), ("status", str)])
 
 LockStatus = NamedTuple(
     "LockStatus",
     [
         ("is_locked", bool),
         ("doors", List[Door]),
         ("windows", List[Window]),
         ("sunroof", List[Sunroof]),
         ("storage", List[Storage]),
         ("charging_port", List[ChargingPort]),
         ("meta", namedtuple),
     ],
 )
 
-
 # ===========================================
 # Named Tuple Selector Function
 # ===========================================
 
 
 def select_named_tuple(path: str, response_or_dict) -> NamedTuple:
     """
```

### Comparing `smartcar-6.8.0/smartcar/vehicle.py` & `smartcar-6.9.0/smartcar/vehicle.py`

 * *Files identical despite different names*

### Comparing `smartcar-6.8.0/smartcar.egg-info/PKG-INFO` & `smartcar-6.9.0/smartcar.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartcar
-Version: 6.8.0
+Version: 6.9.0
 Summary: Smartcar Python SDK
 Home-page: https://github.com/smartcar/python-sdk
 Author: Smartcar
 Author-email: hello@smartcar.com
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -139,14 +139,18 @@
 
 odometer = vehicle.odometer()
 print(odometer.distance)
 
 info = vehicle.info()
 print(info.make)
 print(info.model)
+
+batch = vehicle.batch(paths=['/location'])
+location = batch.location()
+print(location)
 ```
 
 - For a lot more examples on everything you can do with a car, see
   the [smartcar developer docs](https://smartcar.com/docs)
 - For the full SDK reference guide, visit [REFERENCES.md][smartcar-python-sdk-reference]
 
 ## Handling Exceptions
```

