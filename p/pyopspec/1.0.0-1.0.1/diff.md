# Comparing `tmp/pyopspec-1.0.0.tar.gz` & `tmp/pyopspec-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyopspec-1.0.0.tar", last modified: Wed Apr  3 11:20:14 2024, max compression
+gzip compressed data, was "pyopspec-1.0.1.tar", last modified: Wed Apr  3 12:36:21 2024, max compression
```

## Comparing `pyopspec-1.0.0.tar` & `pyopspec-1.0.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 d         (1000) d         (1000)        0 2024-04-03 11:20:14.158943 pyopspec-1.0.0/
--rw-r--r--   0 d         (1000) d         (1000)      597 2024-04-03 11:20:14.158943 pyopspec-1.0.0/PKG-INFO
--rw-r--r--   0 d         (1000) d         (1000)       64 2024-03-19 12:12:42.000000 pyopspec-1.0.0/README.md
-drwxr-xr-x   0 d         (1000) d         (1000)        0 2024-04-03 11:20:14.152276 pyopspec-1.0.0/pyopspec/
--rw-r--r--   0 d         (1000) d         (1000)        0 2024-03-19 12:12:42.000000 pyopspec-1.0.0/pyopspec/__init__.py
--rw-r--r--   0 d         (1000) d         (1000)     2572 2024-03-19 14:52:42.000000 pyopspec-1.0.0/pyopspec/config.py
-drwxr-xr-x   0 d         (1000) d         (1000)        0 2024-04-03 11:20:14.152276 pyopspec-1.0.0/pyopspec/data_exporters/
--rw-r--r--   0 d         (1000) d         (1000)        0 2024-04-03 11:18:04.000000 pyopspec-1.0.0/pyopspec/data_exporters/__init__.py
--rw-r--r--   0 d         (1000) d         (1000)     2290 2024-04-03 11:18:04.000000 pyopspec-1.0.0/pyopspec/data_exporters/data_exporter.py
--rw-r--r--   0 d         (1000) d         (1000)       56 2024-03-19 12:12:42.000000 pyopspec-1.0.0/pyopspec/exceptions.py
-drwxr-xr-x   0 d         (1000) d         (1000)        0 2024-04-03 11:20:14.152276 pyopspec-1.0.0/pyopspec/furnace/
--rw-r--r--   0 d         (1000) d         (1000)        0 2024-03-19 12:12:42.000000 pyopspec-1.0.0/pyopspec/furnace/__init__.py
--rw-r--r--   0 d         (1000) d         (1000)      232 2024-03-19 12:12:42.000000 pyopspec-1.0.0/pyopspec/furnace/exceptions.py
--rw-r--r--   0 d         (1000) d         (1000)      690 2024-03-19 12:12:42.000000 pyopspec-1.0.0/pyopspec/furnace/furnace_controller.py
--rw-r--r--   0 d         (1000) d         (1000)     1034 2024-04-03 11:18:04.000000 pyopspec-1.0.0/pyopspec/furnace/logging.py
--rw-r--r--   0 d         (1000) d         (1000)     8361 2024-03-25 14:43:39.000000 pyopspec-1.0.0/pyopspec/furnace/watlow_furnace_controller.py
-drwxr-xr-x   0 d         (1000) d         (1000)        0 2024-04-03 11:20:14.152276 pyopspec-1.0.0/pyopspec/mass_flow_controller/
--rw-r--r--   0 d         (1000) d         (1000)        0 2024-03-19 12:12:42.000000 pyopspec-1.0.0/pyopspec/mass_flow_controller/__init__.py
--rw-r--r--   0 d         (1000) d         (1000)     3154 2024-03-19 14:47:37.000000 pyopspec-1.0.0/pyopspec/mass_flow_controller/bronkhorst_mass_flow_controller.py
--rw-r--r--   0 d         (1000) d         (1000)      180 2024-03-19 12:12:42.000000 pyopspec-1.0.0/pyopspec/mass_flow_controller/exceptions.py
--rw-r--r--   0 d         (1000) d         (1000)     1039 2024-04-03 11:16:49.000000 pyopspec-1.0.0/pyopspec/mass_flow_controller/logging.py
--rw-r--r--   0 d         (1000) d         (1000)      346 2024-03-19 12:12:42.000000 pyopspec-1.0.0/pyopspec/mass_flow_controller/mass_flow_controller.py
-drwxr-xr-x   0 d         (1000) d         (1000)        0 2024-04-03 11:20:14.155610 pyopspec-1.0.0/pyopspec/plotters/
--rw-r--r--   0 d         (1000) d         (1000)        0 2024-03-19 12:12:42.000000 pyopspec-1.0.0/pyopspec/plotters/__init__.py
--rw-r--r--   0 d         (1000) d         (1000)     1743 2024-03-19 12:12:42.000000 pyopspec-1.0.0/pyopspec/plotters/data.py
--rw-r--r--   0 d         (1000) d         (1000)      786 2024-03-19 12:12:42.000000 pyopspec-1.0.0/pyopspec/plotters/logging.py
--rw-r--r--   0 d         (1000) d         (1000)     3549 2024-03-19 12:12:42.000000 pyopspec-1.0.0/pyopspec/plotters/non_blocking_plotter.py
--rw-r--r--   0 d         (1000) d         (1000)     1124 2024-03-19 12:12:42.000000 pyopspec-1.0.0/pyopspec/plotters/point.py
--rw-r--r--   0 d         (1000) d         (1000)     2507 2024-03-19 12:12:42.000000 pyopspec-1.0.0/pyopspec/plotters/process_plotter.py
-drwxr-xr-x   0 d         (1000) d         (1000)        0 2024-04-03 11:20:14.155610 pyopspec-1.0.0/pyopspec/pressure_controller/
--rw-r--r--   0 d         (1000) d         (1000)        0 2024-03-19 12:12:42.000000 pyopspec-1.0.0/pyopspec/pressure_controller/__init__.py
--rw-r--r--   0 d         (1000) d         (1000)     4458 2024-04-03 09:21:01.000000 pyopspec-1.0.0/pyopspec/pressure_controller/bronkhorst_pressure_controller.py
--rw-r--r--   0 d         (1000) d         (1000)      180 2024-03-19 12:12:42.000000 pyopspec-1.0.0/pyopspec/pressure_controller/exceptions.py
--rw-r--r--   0 d         (1000) d         (1000)     1039 2024-04-03 11:16:29.000000 pyopspec-1.0.0/pyopspec/pressure_controller/logging.py
--rw-r--r--   0 d         (1000) d         (1000)      343 2024-03-19 12:12:42.000000 pyopspec-1.0.0/pyopspec/pressure_controller/pressure_controller.py
--rw-r--r--   0 d         (1000) d         (1000)     2176 2024-04-03 11:18:04.000000 pyopspec-1.0.0/pyopspec/process_config.py
--rw-r--r--   0 d         (1000) d         (1000)     3877 2024-04-03 11:18:04.000000 pyopspec-1.0.0/pyopspec/pyopspec.py
-drwxr-xr-x   0 d         (1000) d         (1000)        0 2024-04-03 11:20:14.155610 pyopspec-1.0.0/pyopspec/steps/
--rw-r--r--   0 d         (1000) d         (1000)        0 2024-03-19 12:12:42.000000 pyopspec-1.0.0/pyopspec/steps/__init__.py
--rw-r--r--   0 d         (1000) d         (1000)      340 2024-03-19 12:12:42.000000 pyopspec-1.0.0/pyopspec/steps/cooling_step.py
--rw-r--r--   0 d         (1000) d         (1000)      257 2024-03-19 12:12:42.000000 pyopspec-1.0.0/pyopspec/steps/final_step.py
--rw-r--r--   0 d         (1000) d         (1000)      340 2024-03-19 12:12:42.000000 pyopspec-1.0.0/pyopspec/steps/heating_step.py
--rw-r--r--   0 d         (1000) d         (1000)      240 2024-03-19 12:33:46.000000 pyopspec-1.0.0/pyopspec/steps/isothermal_step.py
--rw-r--r--   0 d         (1000) d         (1000)      568 2024-03-27 13:21:34.000000 pyopspec-1.0.0/pyopspec/steps/pressure_ramp_step.py
-drwxr-xr-x   0 d         (1000) d         (1000)        0 2024-04-03 11:20:14.158943 pyopspec-1.0.0/pyopspec.egg-info/
--rw-r--r--   0 d         (1000) d         (1000)      597 2024-04-03 11:20:14.000000 pyopspec-1.0.0/pyopspec.egg-info/PKG-INFO
--rw-r--r--   0 d         (1000) d         (1000)     1438 2024-04-03 11:20:14.000000 pyopspec-1.0.0/pyopspec.egg-info/SOURCES.txt
--rw-r--r--   0 d         (1000) d         (1000)        1 2024-04-03 11:20:14.000000 pyopspec-1.0.0/pyopspec.egg-info/dependency_links.txt
--rw-r--r--   0 d         (1000) d         (1000)       52 2024-04-03 11:20:14.000000 pyopspec-1.0.0/pyopspec.egg-info/entry_points.txt
--rw-r--r--   0 d         (1000) d         (1000)       65 2024-04-03 11:20:14.000000 pyopspec-1.0.0/pyopspec.egg-info/requires.txt
--rw-r--r--   0 d         (1000) d         (1000)        9 2024-04-03 11:20:14.000000 pyopspec-1.0.0/pyopspec.egg-info/top_level.txt
--rw-r--r--   0 d         (1000) d         (1000)       38 2024-04-03 11:20:14.158943 pyopspec-1.0.0/setup.cfg
--rw-r--r--   0 d         (1000) d         (1000)     1036 2024-04-03 11:18:19.000000 pyopspec-1.0.0/setup.py
+drwxr-xr-x   0 d         (1000) d         (1000)        0 2024-04-03 12:36:21.285458 pyopspec-1.0.1/
+-rw-r--r--   0 d         (1000) d         (1000)      597 2024-04-03 12:36:21.285458 pyopspec-1.0.1/PKG-INFO
+-rw-r--r--   0 d         (1000) d         (1000)       64 2024-03-19 12:12:42.000000 pyopspec-1.0.1/README.md
+drwxr-xr-x   0 d         (1000) d         (1000)        0 2024-04-03 12:36:21.278792 pyopspec-1.0.1/pyopspec/
+-rw-r--r--   0 d         (1000) d         (1000)        0 2024-03-19 12:12:42.000000 pyopspec-1.0.1/pyopspec/__init__.py
+-rw-r--r--   0 d         (1000) d         (1000)     2572 2024-03-19 14:52:42.000000 pyopspec-1.0.1/pyopspec/config.py
+drwxr-xr-x   0 d         (1000) d         (1000)        0 2024-04-03 12:36:21.282125 pyopspec-1.0.1/pyopspec/data_exporters/
+-rw-r--r--   0 d         (1000) d         (1000)        0 2024-04-03 12:28:51.000000 pyopspec-1.0.1/pyopspec/data_exporters/__init__.py
+-rw-r--r--   0 d         (1000) d         (1000)     2290 2024-04-03 12:28:51.000000 pyopspec-1.0.1/pyopspec/data_exporters/data_exporter.py
+-rw-r--r--   0 d         (1000) d         (1000)       56 2024-03-19 12:12:42.000000 pyopspec-1.0.1/pyopspec/exceptions.py
+drwxr-xr-x   0 d         (1000) d         (1000)        0 2024-04-03 12:36:21.282125 pyopspec-1.0.1/pyopspec/furnace/
+-rw-r--r--   0 d         (1000) d         (1000)        0 2024-03-19 12:12:42.000000 pyopspec-1.0.1/pyopspec/furnace/__init__.py
+-rw-r--r--   0 d         (1000) d         (1000)      232 2024-03-19 12:12:42.000000 pyopspec-1.0.1/pyopspec/furnace/exceptions.py
+-rw-r--r--   0 d         (1000) d         (1000)      690 2024-03-19 12:12:42.000000 pyopspec-1.0.1/pyopspec/furnace/furnace_controller.py
+-rw-r--r--   0 d         (1000) d         (1000)     1196 2024-04-03 12:30:19.000000 pyopspec-1.0.1/pyopspec/furnace/logging.py
+-rw-r--r--   0 d         (1000) d         (1000)     8361 2024-03-25 14:43:39.000000 pyopspec-1.0.1/pyopspec/furnace/watlow_furnace_controller.py
+drwxr-xr-x   0 d         (1000) d         (1000)        0 2024-04-03 12:36:21.282125 pyopspec-1.0.1/pyopspec/mass_flow_controller/
+-rw-r--r--   0 d         (1000) d         (1000)        0 2024-03-19 12:12:42.000000 pyopspec-1.0.1/pyopspec/mass_flow_controller/__init__.py
+-rw-r--r--   0 d         (1000) d         (1000)     3154 2024-03-19 14:47:37.000000 pyopspec-1.0.1/pyopspec/mass_flow_controller/bronkhorst_mass_flow_controller.py
+-rw-r--r--   0 d         (1000) d         (1000)      180 2024-03-19 12:12:42.000000 pyopspec-1.0.1/pyopspec/mass_flow_controller/exceptions.py
+-rw-r--r--   0 d         (1000) d         (1000)     1166 2024-04-03 12:33:30.000000 pyopspec-1.0.1/pyopspec/mass_flow_controller/logging.py
+-rw-r--r--   0 d         (1000) d         (1000)      346 2024-03-19 12:12:42.000000 pyopspec-1.0.1/pyopspec/mass_flow_controller/mass_flow_controller.py
+drwxr-xr-x   0 d         (1000) d         (1000)        0 2024-04-03 12:36:21.282125 pyopspec-1.0.1/pyopspec/plotters/
+-rw-r--r--   0 d         (1000) d         (1000)        0 2024-03-19 12:12:42.000000 pyopspec-1.0.1/pyopspec/plotters/__init__.py
+-rw-r--r--   0 d         (1000) d         (1000)     1743 2024-03-19 12:12:42.000000 pyopspec-1.0.1/pyopspec/plotters/data.py
+-rw-r--r--   0 d         (1000) d         (1000)     1101 2024-04-03 12:28:57.000000 pyopspec-1.0.1/pyopspec/plotters/logging.py
+-rw-r--r--   0 d         (1000) d         (1000)     3549 2024-03-19 12:12:42.000000 pyopspec-1.0.1/pyopspec/plotters/non_blocking_plotter.py
+-rw-r--r--   0 d         (1000) d         (1000)     1124 2024-03-19 12:12:42.000000 pyopspec-1.0.1/pyopspec/plotters/point.py
+-rw-r--r--   0 d         (1000) d         (1000)     2507 2024-03-19 12:12:42.000000 pyopspec-1.0.1/pyopspec/plotters/process_plotter.py
+drwxr-xr-x   0 d         (1000) d         (1000)        0 2024-04-03 12:36:21.285458 pyopspec-1.0.1/pyopspec/pressure_controller/
+-rw-r--r--   0 d         (1000) d         (1000)        0 2024-03-19 12:12:42.000000 pyopspec-1.0.1/pyopspec/pressure_controller/__init__.py
+-rw-r--r--   0 d         (1000) d         (1000)     4458 2024-04-03 09:21:01.000000 pyopspec-1.0.1/pyopspec/pressure_controller/bronkhorst_pressure_controller.py
+-rw-r--r--   0 d         (1000) d         (1000)      180 2024-03-19 12:12:42.000000 pyopspec-1.0.1/pyopspec/pressure_controller/exceptions.py
+-rw-r--r--   0 d         (1000) d         (1000)     1166 2024-04-03 12:33:46.000000 pyopspec-1.0.1/pyopspec/pressure_controller/logging.py
+-rw-r--r--   0 d         (1000) d         (1000)      343 2024-03-19 12:12:42.000000 pyopspec-1.0.1/pyopspec/pressure_controller/pressure_controller.py
+-rw-r--r--   0 d         (1000) d         (1000)     2176 2024-04-03 12:28:51.000000 pyopspec-1.0.1/pyopspec/process_config.py
+-rw-r--r--   0 d         (1000) d         (1000)     3877 2024-04-03 12:28:51.000000 pyopspec-1.0.1/pyopspec/pyopspec.py
+drwxr-xr-x   0 d         (1000) d         (1000)        0 2024-04-03 12:36:21.285458 pyopspec-1.0.1/pyopspec/steps/
+-rw-r--r--   0 d         (1000) d         (1000)        0 2024-03-19 12:12:42.000000 pyopspec-1.0.1/pyopspec/steps/__init__.py
+-rw-r--r--   0 d         (1000) d         (1000)      340 2024-03-19 12:12:42.000000 pyopspec-1.0.1/pyopspec/steps/cooling_step.py
+-rw-r--r--   0 d         (1000) d         (1000)      257 2024-03-19 12:12:42.000000 pyopspec-1.0.1/pyopspec/steps/final_step.py
+-rw-r--r--   0 d         (1000) d         (1000)      340 2024-03-19 12:12:42.000000 pyopspec-1.0.1/pyopspec/steps/heating_step.py
+-rw-r--r--   0 d         (1000) d         (1000)      240 2024-03-19 12:33:46.000000 pyopspec-1.0.1/pyopspec/steps/isothermal_step.py
+-rw-r--r--   0 d         (1000) d         (1000)      568 2024-03-27 13:21:34.000000 pyopspec-1.0.1/pyopspec/steps/pressure_ramp_step.py
+drwxr-xr-x   0 d         (1000) d         (1000)        0 2024-04-03 12:36:21.285458 pyopspec-1.0.1/pyopspec.egg-info/
+-rw-r--r--   0 d         (1000) d         (1000)      597 2024-04-03 12:36:21.000000 pyopspec-1.0.1/pyopspec.egg-info/PKG-INFO
+-rw-r--r--   0 d         (1000) d         (1000)     1438 2024-04-03 12:36:21.000000 pyopspec-1.0.1/pyopspec.egg-info/SOURCES.txt
+-rw-r--r--   0 d         (1000) d         (1000)        1 2024-04-03 12:36:21.000000 pyopspec-1.0.1/pyopspec.egg-info/dependency_links.txt
+-rw-r--r--   0 d         (1000) d         (1000)       52 2024-04-03 12:36:21.000000 pyopspec-1.0.1/pyopspec.egg-info/entry_points.txt
+-rw-r--r--   0 d         (1000) d         (1000)       65 2024-04-03 12:36:21.000000 pyopspec-1.0.1/pyopspec.egg-info/requires.txt
+-rw-r--r--   0 d         (1000) d         (1000)        9 2024-04-03 12:36:21.000000 pyopspec-1.0.1/pyopspec.egg-info/top_level.txt
+-rw-r--r--   0 d         (1000) d         (1000)       38 2024-04-03 12:36:21.285458 pyopspec-1.0.1/setup.cfg
+-rw-r--r--   0 d         (1000) d         (1000)     1036 2024-04-03 12:35:42.000000 pyopspec-1.0.1/setup.py
```

### Comparing `pyopspec-1.0.0/PKG-INFO` & `pyopspec-1.0.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopspec
-Version: 1.0.0
+Version: 1.0.1
 Summary: Program to control operando spectroscopic experiment
 Home-page: https://github.com/leybodv/pyopspec
 Author: Denis Leybo
 Author-email: denis@leybo.xyz
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyopspec-1.0.0/pyopspec/config.py` & `pyopspec-1.0.1/pyopspec/config.py`

 * *Files identical despite different names*

### Comparing `pyopspec-1.0.0/pyopspec/data_exporters/data_exporter.py` & `pyopspec-1.0.1/pyopspec/data_exporters/data_exporter.py`

 * *Files identical despite different names*

### Comparing `pyopspec-1.0.0/pyopspec/furnace/furnace_controller.py` & `pyopspec-1.0.1/pyopspec/furnace/furnace_controller.py`

 * *Files identical despite different names*

### Comparing `pyopspec-1.0.0/pyopspec/furnace/logging.py` & `pyopspec-1.0.1/pyopspec/furnace/logging.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,17 +26,14 @@
     logger = logging.getLogger(name)
     logger.setLevel(logging_levels[name])
     logger.propagate = False
 
     # ch = logging.StreamHandler()
     logfile = Path(logfilename).absolute()
     logfile.parent.mkdir(parents=True, exist_ok=True)
-    ch = logging.FileHandler(filename=logfile)
-    ch.setLevel(logging_levels[name])
-
-    formatter = logging.Formatter(fmt='[%(asctime)s] %(name)s.%(funcName)s: %(levelname)s: %(message)s', datefmt='%d.%m.%Y %H:%M:%S')
-
-    ch.setFormatter(formatter)
-
-    logger.addHandler(ch)
-
+    if not logger.handlers: # create handlers if there are no handlers with this logger already (see https://stackoverflow.com/a/6729713/5267276)
+        ch = logging.FileHandler(filename=logfile)
+        ch.setLevel(logging_levels[name])
+        formatter = logging.Formatter(fmt='[%(asctime)s] %(name)s.%(funcName)s: %(levelname)s: %(message)s', datefmt='%d.%m.%Y %H:%M:%S')
+        ch.setFormatter(formatter)
+        logger.addHandler(ch)
     return logger
```

### Comparing `pyopspec-1.0.0/pyopspec/furnace/watlow_furnace_controller.py` & `pyopspec-1.0.1/pyopspec/furnace/watlow_furnace_controller.py`

 * *Files identical despite different names*

### Comparing `pyopspec-1.0.0/pyopspec/mass_flow_controller/bronkhorst_mass_flow_controller.py` & `pyopspec-1.0.1/pyopspec/mass_flow_controller/bronkhorst_mass_flow_controller.py`

 * *Files identical despite different names*

### Comparing `pyopspec-1.0.0/pyopspec/mass_flow_controller/logging.py` & `pyopspec-1.0.1/pyopspec/pressure_controller/logging.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Module for instantiating and configuring logger
 """
 
 import logging
 from pathlib import Path
 
 logging_levels = {
-                    'BronkhorstMassFlowController':logging.INFO,
+                    'BronkhorstPressureController':logging.INFO,
                  }
 
 def get_logger(name:str, logfilename:str) -> logging.Logger:
     """
     Get logger with corresponding name configured to log to stdout.
 
     parameters
@@ -23,20 +23,16 @@
     logger:logging.Logger
         configured logger
     """
     logger = logging.getLogger(name)
     logger.setLevel(logging_levels[name])
     logger.propagate = False
 
-    # ch = logging.StreamHandler()
     logfile = Path(logfilename).absolute()
     logfile.parent.mkdir(parents=True, exist_ok=True)
-    ch = logging.FileHandler(filename=logfile)
-    ch.setLevel(logging_levels[name])
-
-    formatter = logging.Formatter(fmt='[%(asctime)s] %(name)s.%(funcName)s: %(levelname)s: %(message)s', datefmt='%d.%m.%Y %H:%M:%S')
-
-    ch.setFormatter(formatter)
-
-    logger.addHandler(ch)
-
+    if not logger.handlers: # create handlers if there are no handlers with this logger already (see https://stackoverflow.com/a/6729713/5267276)
+        ch = logging.FileHandler(filename=logfile)
+        ch.setLevel(logging_levels[name])
+        formatter = logging.Formatter(fmt='[%(asctime)s] %(name)s.%(funcName)s: %(levelname)s: %(message)s', datefmt='%d.%m.%Y %H:%M:%S')
+        ch.setFormatter(formatter)
+        logger.addHandler(ch)
     return logger
```

### Comparing `pyopspec-1.0.0/pyopspec/plotters/data.py` & `pyopspec-1.0.1/pyopspec/plotters/data.py`

 * *Files identical despite different names*

### Comparing `pyopspec-1.0.0/pyopspec/plotters/non_blocking_plotter.py` & `pyopspec-1.0.1/pyopspec/plotters/non_blocking_plotter.py`

 * *Files identical despite different names*

### Comparing `pyopspec-1.0.0/pyopspec/plotters/point.py` & `pyopspec-1.0.1/pyopspec/plotters/point.py`

 * *Files identical despite different names*

### Comparing `pyopspec-1.0.0/pyopspec/plotters/process_plotter.py` & `pyopspec-1.0.1/pyopspec/plotters/process_plotter.py`

 * *Files identical despite different names*

### Comparing `pyopspec-1.0.0/pyopspec/pressure_controller/bronkhorst_pressure_controller.py` & `pyopspec-1.0.1/pyopspec/pressure_controller/bronkhorst_pressure_controller.py`

 * *Files identical despite different names*

### Comparing `pyopspec-1.0.0/pyopspec/pressure_controller/logging.py` & `pyopspec-1.0.1/pyopspec/plotters/logging.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 Module for instantiating and configuring logger
 """
 
 import logging
 from pathlib import Path
 
 logging_levels = {
-                    'BronkhorstPressureController':logging.INFO,
                  }
 
 def get_logger(name:str, logfilename:str) -> logging.Logger:
     """
     Get logger with corresponding name configured to log to stdout.
 
     parameters
@@ -23,20 +22,16 @@
     logger:logging.Logger
         configured logger
     """
     logger = logging.getLogger(name)
     logger.setLevel(logging_levels[name])
     logger.propagate = False
 
-    # ch = logging.StreamHandler()
     logfile = Path(logfilename).absolute()
     logfile.parent.mkdir(parents=True, exist_ok=True)
-    ch = logging.FileHandler(filename=logfile)
-    ch.setLevel(logging_levels[name])
-
-    formatter = logging.Formatter(fmt='[%(asctime)s] %(name)s.%(funcName)s: %(levelname)s: %(message)s', datefmt='%d.%m.%Y %H:%M:%S')
-
-    ch.setFormatter(formatter)
-
-    logger.addHandler(ch)
-
+    if not logger.handlers: # create handlers if there are no handlers with this logger already (see https://stackoverflow.com/a/6729713/5267276)
+        ch = logging.FileHandler(filename=logfile)
+        ch.setLevel(logging_levels[name])
+        formatter = logging.Formatter(fmt='[%(asctime)s] %(name)s.%(funcName)s: %(levelname)s: %(message)s', datefmt='%d.%m.%Y %H:%M:%S')
+        ch.setFormatter(formatter)
+        logger.addHandler(ch)
     return logger
```

### Comparing `pyopspec-1.0.0/pyopspec/process_config.py` & `pyopspec-1.0.1/pyopspec/process_config.py`

 * *Files identical despite different names*

### Comparing `pyopspec-1.0.0/pyopspec/pyopspec.py` & `pyopspec-1.0.1/pyopspec/pyopspec.py`

 * *Files identical despite different names*

### Comparing `pyopspec-1.0.0/pyopspec/steps/pressure_ramp_step.py` & `pyopspec-1.0.1/pyopspec/steps/pressure_ramp_step.py`

 * *Files identical despite different names*

### Comparing `pyopspec-1.0.0/pyopspec.egg-info/PKG-INFO` & `pyopspec-1.0.1/pyopspec.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopspec
-Version: 1.0.0
+Version: 1.0.1
 Summary: Program to control operando spectroscopic experiment
 Home-page: https://github.com/leybodv/pyopspec
 Author: Denis Leybo
 Author-email: denis@leybo.xyz
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyopspec-1.0.0/pyopspec.egg-info/SOURCES.txt` & `pyopspec-1.0.1/pyopspec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyopspec-1.0.0/setup.py` & `pyopspec-1.0.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,15 +8,15 @@
             "bronkhorst-propar>=1.0,<2.0",
             "pywatlow>=0.1.4",
             "matplotlib>=3.8,<4.0",
     ]
 
 setuptools.setup(
      name='pyopspec',
-     version='1.0.0',
+     version='1.0.1',
      author="Denis Leybo",
      author_email="denis@leybo.xyz",
      description="Program to control operando spectroscopic experiment",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://github.com/leybodv/pyopspec",
      packages=setuptools.find_packages(),
```

