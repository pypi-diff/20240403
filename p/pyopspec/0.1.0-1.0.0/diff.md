# Comparing `tmp/pyopspec-0.1.0.tar.gz` & `tmp/pyopspec-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyopspec-0.1.0.tar", last modified: Wed Mar 27 13:24:53 2024, max compression
+gzip compressed data, was "pyopspec-1.0.0.tar", last modified: Wed Apr  3 11:20:14 2024, max compression
```

## Comparing `pyopspec-0.1.0.tar` & `pyopspec-1.0.0.tar`

### file list

```diff
@@ -1,50 +1,53 @@
-drwxr-xr-x   0 d         (1000) d         (1000)        0 2024-03-27 13:24:53.173155 pyopspec-0.1.0/
--rw-r--r--   0 d         (1000) d         (1000)      597 2024-03-27 13:24:53.173155 pyopspec-0.1.0/PKG-INFO
--rw-r--r--   0 d         (1000) d         (1000)       64 2024-03-19 12:12:42.000000 pyopspec-0.1.0/README.md
-drwxr-xr-x   0 d         (1000) d         (1000)        0 2024-03-27 13:24:53.166489 pyopspec-0.1.0/pyopspec/
--rw-r--r--   0 d         (1000) d         (1000)        0 2024-03-19 12:12:42.000000 pyopspec-0.1.0/pyopspec/__init__.py
--rw-r--r--   0 d         (1000) d         (1000)     2572 2024-03-19 14:52:42.000000 pyopspec-0.1.0/pyopspec/config.py
--rw-r--r--   0 d         (1000) d         (1000)       56 2024-03-19 12:12:42.000000 pyopspec-0.1.0/pyopspec/exceptions.py
-drwxr-xr-x   0 d         (1000) d         (1000)        0 2024-03-27 13:24:53.166489 pyopspec-0.1.0/pyopspec/furnace/
--rw-r--r--   0 d         (1000) d         (1000)        0 2024-03-19 12:12:42.000000 pyopspec-0.1.0/pyopspec/furnace/__init__.py
--rw-r--r--   0 d         (1000) d         (1000)      232 2024-03-19 12:12:42.000000 pyopspec-0.1.0/pyopspec/furnace/exceptions.py
--rw-r--r--   0 d         (1000) d         (1000)      690 2024-03-19 12:12:42.000000 pyopspec-0.1.0/pyopspec/furnace/furnace_controller.py
--rw-r--r--   0 d         (1000) d         (1000)     1033 2024-03-19 14:10:43.000000 pyopspec-0.1.0/pyopspec/furnace/logging.py
--rw-r--r--   0 d         (1000) d         (1000)     8361 2024-03-25 14:43:39.000000 pyopspec-0.1.0/pyopspec/furnace/watlow_furnace_controller.py
-drwxr-xr-x   0 d         (1000) d         (1000)        0 2024-03-27 13:24:53.169822 pyopspec-0.1.0/pyopspec/mass_flow_controller/
--rw-r--r--   0 d         (1000) d         (1000)        0 2024-03-19 12:12:42.000000 pyopspec-0.1.0/pyopspec/mass_flow_controller/__init__.py
--rw-r--r--   0 d         (1000) d         (1000)     3154 2024-03-19 14:47:37.000000 pyopspec-0.1.0/pyopspec/mass_flow_controller/bronkhorst_mass_flow_controller.py
--rw-r--r--   0 d         (1000) d         (1000)      180 2024-03-19 12:12:42.000000 pyopspec-0.1.0/pyopspec/mass_flow_controller/exceptions.py
--rw-r--r--   0 d         (1000) d         (1000)     1039 2024-03-19 14:46:39.000000 pyopspec-0.1.0/pyopspec/mass_flow_controller/logging.py
--rw-r--r--   0 d         (1000) d         (1000)      346 2024-03-19 12:12:42.000000 pyopspec-0.1.0/pyopspec/mass_flow_controller/mass_flow_controller.py
-drwxr-xr-x   0 d         (1000) d         (1000)        0 2024-03-27 13:24:53.169822 pyopspec-0.1.0/pyopspec/plotters/
--rw-r--r--   0 d         (1000) d         (1000)        0 2024-03-19 12:12:42.000000 pyopspec-0.1.0/pyopspec/plotters/__init__.py
--rw-r--r--   0 d         (1000) d         (1000)     1743 2024-03-19 12:12:42.000000 pyopspec-0.1.0/pyopspec/plotters/data.py
--rw-r--r--   0 d         (1000) d         (1000)      786 2024-03-19 12:12:42.000000 pyopspec-0.1.0/pyopspec/plotters/logging.py
--rw-r--r--   0 d         (1000) d         (1000)     3549 2024-03-19 12:12:42.000000 pyopspec-0.1.0/pyopspec/plotters/non_blocking_plotter.py
--rw-r--r--   0 d         (1000) d         (1000)     1124 2024-03-19 12:12:42.000000 pyopspec-0.1.0/pyopspec/plotters/point.py
--rw-r--r--   0 d         (1000) d         (1000)     2507 2024-03-19 12:12:42.000000 pyopspec-0.1.0/pyopspec/plotters/process_plotter.py
-drwxr-xr-x   0 d         (1000) d         (1000)        0 2024-03-27 13:24:53.169822 pyopspec-0.1.0/pyopspec/pressure_controller/
--rw-r--r--   0 d         (1000) d         (1000)        0 2024-03-19 12:12:42.000000 pyopspec-0.1.0/pyopspec/pressure_controller/__init__.py
--rw-r--r--   0 d         (1000) d         (1000)     4458 2024-03-27 13:21:34.000000 pyopspec-0.1.0/pyopspec/pressure_controller/bronkhorst_pressure_controller.py
--rw-r--r--   0 d         (1000) d         (1000)      180 2024-03-19 12:12:42.000000 pyopspec-0.1.0/pyopspec/pressure_controller/exceptions.py
--rw-r--r--   0 d         (1000) d         (1000)     1039 2024-03-19 14:51:05.000000 pyopspec-0.1.0/pyopspec/pressure_controller/logging.py
--rw-r--r--   0 d         (1000) d         (1000)      343 2024-03-19 12:12:42.000000 pyopspec-0.1.0/pyopspec/pressure_controller/pressure_controller.py
--rw-r--r--   0 d         (1000) d         (1000)     2136 2024-03-27 13:21:34.000000 pyopspec-0.1.0/pyopspec/process_config.py
--rw-r--r--   0 d         (1000) d         (1000)     3530 2024-03-27 13:21:34.000000 pyopspec-0.1.0/pyopspec/pyopspec.py
-drwxr-xr-x   0 d         (1000) d         (1000)        0 2024-03-27 13:24:53.173155 pyopspec-0.1.0/pyopspec/steps/
--rw-r--r--   0 d         (1000) d         (1000)        0 2024-03-19 12:12:42.000000 pyopspec-0.1.0/pyopspec/steps/__init__.py
--rw-r--r--   0 d         (1000) d         (1000)      340 2024-03-19 12:12:42.000000 pyopspec-0.1.0/pyopspec/steps/cooling_step.py
--rw-r--r--   0 d         (1000) d         (1000)      257 2024-03-19 12:12:42.000000 pyopspec-0.1.0/pyopspec/steps/final_step.py
--rw-r--r--   0 d         (1000) d         (1000)      340 2024-03-19 12:12:42.000000 pyopspec-0.1.0/pyopspec/steps/heating_step.py
--rw-r--r--   0 d         (1000) d         (1000)      240 2024-03-19 12:33:46.000000 pyopspec-0.1.0/pyopspec/steps/isothermal_step.py
--rw-r--r--   0 d         (1000) d         (1000)      568 2024-03-27 13:21:34.000000 pyopspec-0.1.0/pyopspec/steps/pressure_ramp_step.py
-drwxr-xr-x   0 d         (1000) d         (1000)        0 2024-03-27 13:24:53.173155 pyopspec-0.1.0/pyopspec.egg-info/
--rw-r--r--   0 d         (1000) d         (1000)      597 2024-03-27 13:24:53.000000 pyopspec-0.1.0/pyopspec.egg-info/PKG-INFO
--rw-r--r--   0 d         (1000) d         (1000)     1361 2024-03-27 13:24:53.000000 pyopspec-0.1.0/pyopspec.egg-info/SOURCES.txt
--rw-r--r--   0 d         (1000) d         (1000)        1 2024-03-27 13:24:53.000000 pyopspec-0.1.0/pyopspec.egg-info/dependency_links.txt
--rw-r--r--   0 d         (1000) d         (1000)       52 2024-03-27 13:24:53.000000 pyopspec-0.1.0/pyopspec.egg-info/entry_points.txt
--rw-r--r--   0 d         (1000) d         (1000)       65 2024-03-27 13:24:53.000000 pyopspec-0.1.0/pyopspec.egg-info/requires.txt
--rw-r--r--   0 d         (1000) d         (1000)        9 2024-03-27 13:24:53.000000 pyopspec-0.1.0/pyopspec.egg-info/top_level.txt
--rw-r--r--   0 d         (1000) d         (1000)       38 2024-03-27 13:24:53.173155 pyopspec-0.1.0/setup.cfg
--rw-r--r--   0 d         (1000) d         (1000)     1036 2024-03-27 13:21:34.000000 pyopspec-0.1.0/setup.py
+drwxr-xr-x   0 d         (1000) d         (1000)        0 2024-04-03 11:20:14.158943 pyopspec-1.0.0/
+-rw-r--r--   0 d         (1000) d         (1000)      597 2024-04-03 11:20:14.158943 pyopspec-1.0.0/PKG-INFO
+-rw-r--r--   0 d         (1000) d         (1000)       64 2024-03-19 12:12:42.000000 pyopspec-1.0.0/README.md
+drwxr-xr-x   0 d         (1000) d         (1000)        0 2024-04-03 11:20:14.152276 pyopspec-1.0.0/pyopspec/
+-rw-r--r--   0 d         (1000) d         (1000)        0 2024-03-19 12:12:42.000000 pyopspec-1.0.0/pyopspec/__init__.py
+-rw-r--r--   0 d         (1000) d         (1000)     2572 2024-03-19 14:52:42.000000 pyopspec-1.0.0/pyopspec/config.py
+drwxr-xr-x   0 d         (1000) d         (1000)        0 2024-04-03 11:20:14.152276 pyopspec-1.0.0/pyopspec/data_exporters/
+-rw-r--r--   0 d         (1000) d         (1000)        0 2024-04-03 11:18:04.000000 pyopspec-1.0.0/pyopspec/data_exporters/__init__.py
+-rw-r--r--   0 d         (1000) d         (1000)     2290 2024-04-03 11:18:04.000000 pyopspec-1.0.0/pyopspec/data_exporters/data_exporter.py
+-rw-r--r--   0 d         (1000) d         (1000)       56 2024-03-19 12:12:42.000000 pyopspec-1.0.0/pyopspec/exceptions.py
+drwxr-xr-x   0 d         (1000) d         (1000)        0 2024-04-03 11:20:14.152276 pyopspec-1.0.0/pyopspec/furnace/
+-rw-r--r--   0 d         (1000) d         (1000)        0 2024-03-19 12:12:42.000000 pyopspec-1.0.0/pyopspec/furnace/__init__.py
+-rw-r--r--   0 d         (1000) d         (1000)      232 2024-03-19 12:12:42.000000 pyopspec-1.0.0/pyopspec/furnace/exceptions.py
+-rw-r--r--   0 d         (1000) d         (1000)      690 2024-03-19 12:12:42.000000 pyopspec-1.0.0/pyopspec/furnace/furnace_controller.py
+-rw-r--r--   0 d         (1000) d         (1000)     1034 2024-04-03 11:18:04.000000 pyopspec-1.0.0/pyopspec/furnace/logging.py
+-rw-r--r--   0 d         (1000) d         (1000)     8361 2024-03-25 14:43:39.000000 pyopspec-1.0.0/pyopspec/furnace/watlow_furnace_controller.py
+drwxr-xr-x   0 d         (1000) d         (1000)        0 2024-04-03 11:20:14.152276 pyopspec-1.0.0/pyopspec/mass_flow_controller/
+-rw-r--r--   0 d         (1000) d         (1000)        0 2024-03-19 12:12:42.000000 pyopspec-1.0.0/pyopspec/mass_flow_controller/__init__.py
+-rw-r--r--   0 d         (1000) d         (1000)     3154 2024-03-19 14:47:37.000000 pyopspec-1.0.0/pyopspec/mass_flow_controller/bronkhorst_mass_flow_controller.py
+-rw-r--r--   0 d         (1000) d         (1000)      180 2024-03-19 12:12:42.000000 pyopspec-1.0.0/pyopspec/mass_flow_controller/exceptions.py
+-rw-r--r--   0 d         (1000) d         (1000)     1039 2024-04-03 11:16:49.000000 pyopspec-1.0.0/pyopspec/mass_flow_controller/logging.py
+-rw-r--r--   0 d         (1000) d         (1000)      346 2024-03-19 12:12:42.000000 pyopspec-1.0.0/pyopspec/mass_flow_controller/mass_flow_controller.py
+drwxr-xr-x   0 d         (1000) d         (1000)        0 2024-04-03 11:20:14.155610 pyopspec-1.0.0/pyopspec/plotters/
+-rw-r--r--   0 d         (1000) d         (1000)        0 2024-03-19 12:12:42.000000 pyopspec-1.0.0/pyopspec/plotters/__init__.py
+-rw-r--r--   0 d         (1000) d         (1000)     1743 2024-03-19 12:12:42.000000 pyopspec-1.0.0/pyopspec/plotters/data.py
+-rw-r--r--   0 d         (1000) d         (1000)      786 2024-03-19 12:12:42.000000 pyopspec-1.0.0/pyopspec/plotters/logging.py
+-rw-r--r--   0 d         (1000) d         (1000)     3549 2024-03-19 12:12:42.000000 pyopspec-1.0.0/pyopspec/plotters/non_blocking_plotter.py
+-rw-r--r--   0 d         (1000) d         (1000)     1124 2024-03-19 12:12:42.000000 pyopspec-1.0.0/pyopspec/plotters/point.py
+-rw-r--r--   0 d         (1000) d         (1000)     2507 2024-03-19 12:12:42.000000 pyopspec-1.0.0/pyopspec/plotters/process_plotter.py
+drwxr-xr-x   0 d         (1000) d         (1000)        0 2024-04-03 11:20:14.155610 pyopspec-1.0.0/pyopspec/pressure_controller/
+-rw-r--r--   0 d         (1000) d         (1000)        0 2024-03-19 12:12:42.000000 pyopspec-1.0.0/pyopspec/pressure_controller/__init__.py
+-rw-r--r--   0 d         (1000) d         (1000)     4458 2024-04-03 09:21:01.000000 pyopspec-1.0.0/pyopspec/pressure_controller/bronkhorst_pressure_controller.py
+-rw-r--r--   0 d         (1000) d         (1000)      180 2024-03-19 12:12:42.000000 pyopspec-1.0.0/pyopspec/pressure_controller/exceptions.py
+-rw-r--r--   0 d         (1000) d         (1000)     1039 2024-04-03 11:16:29.000000 pyopspec-1.0.0/pyopspec/pressure_controller/logging.py
+-rw-r--r--   0 d         (1000) d         (1000)      343 2024-03-19 12:12:42.000000 pyopspec-1.0.0/pyopspec/pressure_controller/pressure_controller.py
+-rw-r--r--   0 d         (1000) d         (1000)     2176 2024-04-03 11:18:04.000000 pyopspec-1.0.0/pyopspec/process_config.py
+-rw-r--r--   0 d         (1000) d         (1000)     3877 2024-04-03 11:18:04.000000 pyopspec-1.0.0/pyopspec/pyopspec.py
+drwxr-xr-x   0 d         (1000) d         (1000)        0 2024-04-03 11:20:14.155610 pyopspec-1.0.0/pyopspec/steps/
+-rw-r--r--   0 d         (1000) d         (1000)        0 2024-03-19 12:12:42.000000 pyopspec-1.0.0/pyopspec/steps/__init__.py
+-rw-r--r--   0 d         (1000) d         (1000)      340 2024-03-19 12:12:42.000000 pyopspec-1.0.0/pyopspec/steps/cooling_step.py
+-rw-r--r--   0 d         (1000) d         (1000)      257 2024-03-19 12:12:42.000000 pyopspec-1.0.0/pyopspec/steps/final_step.py
+-rw-r--r--   0 d         (1000) d         (1000)      340 2024-03-19 12:12:42.000000 pyopspec-1.0.0/pyopspec/steps/heating_step.py
+-rw-r--r--   0 d         (1000) d         (1000)      240 2024-03-19 12:33:46.000000 pyopspec-1.0.0/pyopspec/steps/isothermal_step.py
+-rw-r--r--   0 d         (1000) d         (1000)      568 2024-03-27 13:21:34.000000 pyopspec-1.0.0/pyopspec/steps/pressure_ramp_step.py
+drwxr-xr-x   0 d         (1000) d         (1000)        0 2024-04-03 11:20:14.158943 pyopspec-1.0.0/pyopspec.egg-info/
+-rw-r--r--   0 d         (1000) d         (1000)      597 2024-04-03 11:20:14.000000 pyopspec-1.0.0/pyopspec.egg-info/PKG-INFO
+-rw-r--r--   0 d         (1000) d         (1000)     1438 2024-04-03 11:20:14.000000 pyopspec-1.0.0/pyopspec.egg-info/SOURCES.txt
+-rw-r--r--   0 d         (1000) d         (1000)        1 2024-04-03 11:20:14.000000 pyopspec-1.0.0/pyopspec.egg-info/dependency_links.txt
+-rw-r--r--   0 d         (1000) d         (1000)       52 2024-04-03 11:20:14.000000 pyopspec-1.0.0/pyopspec.egg-info/entry_points.txt
+-rw-r--r--   0 d         (1000) d         (1000)       65 2024-04-03 11:20:14.000000 pyopspec-1.0.0/pyopspec.egg-info/requires.txt
+-rw-r--r--   0 d         (1000) d         (1000)        9 2024-04-03 11:20:14.000000 pyopspec-1.0.0/pyopspec.egg-info/top_level.txt
+-rw-r--r--   0 d         (1000) d         (1000)       38 2024-04-03 11:20:14.158943 pyopspec-1.0.0/setup.cfg
+-rw-r--r--   0 d         (1000) d         (1000)     1036 2024-04-03 11:18:19.000000 pyopspec-1.0.0/setup.py
```

### Comparing `pyopspec-0.1.0/PKG-INFO` & `pyopspec-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopspec
-Version: 0.1.0
+Version: 1.0.0
 Summary: Program to control operando spectroscopic experiment
 Home-page: https://github.com/leybodv/pyopspec
 Author: Denis Leybo
 Author-email: denis@leybo.xyz
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyopspec-0.1.0/pyopspec/config.py` & `pyopspec-1.0.0/pyopspec/config.py`

 * *Files identical despite different names*

### Comparing `pyopspec-0.1.0/pyopspec/furnace/furnace_controller.py` & `pyopspec-1.0.0/pyopspec/furnace/furnace_controller.py`

 * *Files identical despite different names*

### Comparing `pyopspec-0.1.0/pyopspec/furnace/logging.py` & `pyopspec-1.0.0/pyopspec/furnace/logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Module for instantiating and configuring logger
 """
 
 import logging
 from pathlib import Path
 
 logging_levels = {
-                    'WatlowFurnaceController':logging.INFO
+                    'WatlowFurnaceController':logging.INFO,
                  }
 
 def get_logger(name:str, logfilename:str) -> logging.Logger:
     """
     Get logger with corresponding name configured to log to stdout.
 
     parameters
```

### Comparing `pyopspec-0.1.0/pyopspec/furnace/watlow_furnace_controller.py` & `pyopspec-1.0.0/pyopspec/furnace/watlow_furnace_controller.py`

 * *Files identical despite different names*

### Comparing `pyopspec-0.1.0/pyopspec/mass_flow_controller/bronkhorst_mass_flow_controller.py` & `pyopspec-1.0.0/pyopspec/mass_flow_controller/bronkhorst_mass_flow_controller.py`

 * *Files identical despite different names*

### Comparing `pyopspec-0.1.0/pyopspec/mass_flow_controller/logging.py` & `pyopspec-1.0.0/pyopspec/mass_flow_controller/logging.py`

 * *Files identical despite different names*

### Comparing `pyopspec-0.1.0/pyopspec/plotters/data.py` & `pyopspec-1.0.0/pyopspec/plotters/data.py`

 * *Files identical despite different names*

### Comparing `pyopspec-0.1.0/pyopspec/plotters/logging.py` & `pyopspec-1.0.0/pyopspec/plotters/logging.py`

 * *Files identical despite different names*

### Comparing `pyopspec-0.1.0/pyopspec/plotters/non_blocking_plotter.py` & `pyopspec-1.0.0/pyopspec/plotters/non_blocking_plotter.py`

 * *Files identical despite different names*

### Comparing `pyopspec-0.1.0/pyopspec/plotters/point.py` & `pyopspec-1.0.0/pyopspec/plotters/point.py`

 * *Files identical despite different names*

### Comparing `pyopspec-0.1.0/pyopspec/plotters/process_plotter.py` & `pyopspec-1.0.0/pyopspec/plotters/process_plotter.py`

 * *Files identical despite different names*

### Comparing `pyopspec-0.1.0/pyopspec/pressure_controller/bronkhorst_pressure_controller.py` & `pyopspec-1.0.0/pyopspec/pressure_controller/bronkhorst_pressure_controller.py`

 * *Files identical despite different names*

### Comparing `pyopspec-0.1.0/pyopspec/pressure_controller/logging.py` & `pyopspec-1.0.0/pyopspec/pressure_controller/logging.py`

 * *Files identical despite different names*

### Comparing `pyopspec-0.1.0/pyopspec/process_config.py` & `pyopspec-1.0.0/pyopspec/process_config.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from pyopspec.steps.heating_step import HeatingStep
 from pyopspec.steps.isothermal_step import IsothermalStep
 from pyopspec.steps.cooling_step import CoolingStep
 from pyopspec.steps.pressure_ramp_step import PressureRampStep
 from pyopspec.steps.final_step import FinalStep
 
+export_folder_path = './exported_data'
+
 steps = [
             HeatingStep(
                 pressure=1,
                 flow_rates={
                                 'Ar' :15,
                                 'H2' :5,
                                 'CO' :0,
```

### Comparing `pyopspec-0.1.0/pyopspec/pyopspec.py` & `pyopspec-1.0.0/pyopspec/pyopspec.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import types
 import sys
 from pathlib import Path
 
 # import pyopspec.process_config as process_config
 import pyopspec.config as config
 from pyopspec.plotters.process_plotter import DataCollectorPlotter
+from pyopspec.data_exporters.data_exporter import DataExporter
 from pyopspec.steps.heating_step import HeatingStep
 from pyopspec.steps.isothermal_step import IsothermalStep
 from pyopspec.steps.cooling_step import CoolingStep
 from pyopspec.steps.final_step import FinalStep
 from pyopspec.steps.pressure_ramp_step import PressureRampStep
 from .exceptions import *
 
@@ -37,15 +38,17 @@
     config.pressure_controller.connect()
     for gas in config.mfcs:
         config.mfcs[gas].connect()
     config.furnace.connect()
     config_path = Path(args.config)
     process_config = _import_config(config_path)
     plotter = DataCollectorPlotter(furnace_controller=config.furnace, mass_flow_controllers=config.mfcs, pressure_controller=config.pressure_controller)
+    data_exporter = DataExporter(folder_path=process_config.export_folder_path, furnace_controller=config.furnace, mass_flow_controllers=config.mfcs, pressure_controller=config.pressure_controller)
     plotter.start()
+    data_exporter.start()
     for step in process_config.steps:
         if isinstance(step, HeatingStep):
             config.pressure_controller.set_pressure(step.pressure)
             for gas in step.flow_rates:
                 config.mfcs[gas].set_flow_rate(step.flow_rates[gas])
             config.furnace.set_ramp_rate(step.heating_rate)
             config.furnace.heat_up_to(step.target_temperature)
@@ -64,14 +67,16 @@
             for gas in step.flow_rates:
                 config.mfcs[gas].set_flow_rate(step.flow_rates[gas])
             config.pressure_controller.ramp_pressure(pressure=step.pressure, ramp_rate=step.pressure_ramp_rate)
         elif isinstance(step, FinalStep):
             config.pressure_controller.set_pressure(step.pressure)
             for gas in step.flow_rates:
                 config.mfcs[gas].set_flow_rate(step.flow_rates[gas])
+            plotter.stop()
+            data_exporter.stop()
             config.furnace.set_temperature(step.temperature)
         else:
             raise UnknownStepException(f'Unknown step: {step}')
 
 def main():
     """
     """
```

### Comparing `pyopspec-0.1.0/pyopspec/steps/pressure_ramp_step.py` & `pyopspec-1.0.0/pyopspec/steps/pressure_ramp_step.py`

 * *Files identical despite different names*

### Comparing `pyopspec-0.1.0/pyopspec.egg-info/PKG-INFO` & `pyopspec-1.0.0/pyopspec.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopspec
-Version: 0.1.0
+Version: 1.0.0
 Summary: Program to control operando spectroscopic experiment
 Home-page: https://github.com/leybodv/pyopspec
 Author: Denis Leybo
 Author-email: denis@leybo.xyz
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyopspec-0.1.0/pyopspec.egg-info/SOURCES.txt` & `pyopspec-1.0.0/pyopspec.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 pyopspec/pyopspec.py
 pyopspec.egg-info/PKG-INFO
 pyopspec.egg-info/SOURCES.txt
 pyopspec.egg-info/dependency_links.txt
 pyopspec.egg-info/entry_points.txt
 pyopspec.egg-info/requires.txt
 pyopspec.egg-info/top_level.txt
+pyopspec/data_exporters/__init__.py
+pyopspec/data_exporters/data_exporter.py
 pyopspec/furnace/__init__.py
 pyopspec/furnace/exceptions.py
 pyopspec/furnace/furnace_controller.py
 pyopspec/furnace/logging.py
 pyopspec/furnace/watlow_furnace_controller.py
 pyopspec/mass_flow_controller/__init__.py
 pyopspec/mass_flow_controller/bronkhorst_mass_flow_controller.py
```

### Comparing `pyopspec-0.1.0/setup.py` & `pyopspec-1.0.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,15 +8,15 @@
             "bronkhorst-propar>=1.0,<2.0",
             "pywatlow>=0.1.4",
             "matplotlib>=3.8,<4.0",
     ]
 
 setuptools.setup(
      name='pyopspec',
-     version='0.1.0',
+     version='1.0.0',
      author="Denis Leybo",
      author_email="denis@leybo.xyz",
      description="Program to control operando spectroscopic experiment",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://github.com/leybodv/pyopspec",
      packages=setuptools.find_packages(),
```

