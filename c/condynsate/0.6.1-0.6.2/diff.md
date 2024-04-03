# Comparing `tmp/condynsate-0.6.1.tar.gz` & `tmp/condynsate-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "condynsate-0.6.1.tar", last modified: Wed Apr  3 15:36:02 2024, max compression
+gzip compressed data, was "condynsate-0.6.2.tar", last modified: Wed Apr  3 18:09:52 2024, max compression
```

## Comparing `condynsate-0.6.1.tar` & `condynsate-0.6.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 15:36:02.383364 condynsate-0.6.1/
--rw-rw-rw-   0        0        0     1092 2023-11-24 19:50:22.000000 condynsate-0.6.1/LICENSE
--rw-rw-rw-   0        0        0     4875 2024-04-03 15:36:02.383364 condynsate-0.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     2391 2024-03-21 21:05:21.000000 condynsate-0.6.1/README.md
--rw-rw-rw-   0        0        0     1439 2024-04-03 15:35:20.000000 condynsate-0.6.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-03 15:36:02.383364 condynsate-0.6.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-03 15:36:02.289544 condynsate-0.6.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-03 15:36:02.305170 condynsate-0.6.1/src/condynsate/
-drwxrwxrwx   0        0        0        0 2024-04-03 15:36:02.383364 condynsate-0.6.1/src/condynsate/__assets__/
--rw-rw-rw-   0        0        0    36584 2023-11-24 19:50:22.000000 condynsate-0.6.1/src/condynsate/__assets__/arrow_ccw.stl
--rw-rw-rw-   0        0        0    36584 2023-11-24 19:50:22.000000 condynsate-0.6.1/src/condynsate/__assets__/arrow_cw.stl
--rw-rw-rw-   0        0        0     6784 2023-11-24 19:50:22.000000 condynsate-0.6.1/src/condynsate/__assets__/arrow_lin.stl
--rw-rw-rw-   0        0        0     6379 2023-11-24 19:50:22.000000 condynsate-0.6.1/src/condynsate/__assets__/check.png
--rw-rw-rw-   0        0        0      684 2023-11-24 19:50:22.000000 condynsate-0.6.1/src/condynsate/__assets__/cube.stl
--rw-rw-rw-   0        0        0    12684 2023-12-12 22:20:42.000000 condynsate-0.6.1/src/condynsate/__assets__/cylinder.stl
--rw-rw-rw-   0        0        0    12684 2023-12-12 22:33:34.000000 condynsate-0.6.1/src/condynsate/__assets__/cylinder_lower_origin.stl
--rw-rw-rw-   0        0        0    11484 2024-01-05 02:07:25.000000 condynsate-0.6.1/src/condynsate/__assets__/gate_med.stl
--rw-rw-rw-   0        0        0     4084 2024-01-05 02:03:45.000000 condynsate-0.6.1/src/condynsate/__assets__/gate_short.stl
--rw-rw-rw-   0        0        0    11484 2024-01-05 02:08:19.000000 condynsate-0.6.1/src/condynsate/__assets__/gate_tall.stl
--rw-rw-rw-   0        0        0      344 2023-11-24 19:50:22.000000 condynsate-0.6.1/src/condynsate/__assets__/plane_big.obj
--rw-rw-rw-   0        0        0      332 2023-11-24 19:50:22.000000 condynsate-0.6.1/src/condynsate/__assets__/plane_med.obj
--rw-rw-rw-   0        0        0      320 2023-11-24 19:50:22.000000 condynsate-0.6.1/src/condynsate/__assets__/plane_small.obj
--rw-rw-rw-   0        0        0      384 2023-11-24 19:50:22.000000 condynsate-0.6.1/src/condynsate/__assets__/pyramid.stl
--rw-rw-rw-   0        0        0    61284 2023-11-24 19:50:22.000000 condynsate-0.6.1/src/condynsate/__assets__/sphere.stl
--rw-rw-rw-   0        0        0      153 2024-04-03 15:35:20.000000 condynsate-0.6.1/src/condynsate/__init__.py
--rw-rw-rw-   0        0        0    44652 2023-12-15 21:36:13.000000 condynsate-0.6.1/src/condynsate/animator.py
--rw-rw-rw-   0        0        0     8209 2024-02-06 15:55:34.000000 condynsate-0.6.1/src/condynsate/keyboard.py
--rw-rw-rw-   0        0        0   145626 2024-04-03 15:34:39.000000 condynsate-0.6.1/src/condynsate/simulator.py
--rw-rw-rw-   0        0        0    10335 2024-03-26 22:00:32.000000 condynsate-0.6.1/src/condynsate/utils.py
--rw-rw-rw-   0        0        0    22362 2024-04-02 19:38:52.000000 condynsate-0.6.1/src/condynsate/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-04-03 15:36:02.383364 condynsate-0.6.1/src/condynsate.egg-info/
--rw-rw-rw-   0        0        0     4875 2024-04-03 15:36:02.000000 condynsate-0.6.1/src/condynsate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      981 2024-04-03 15:36:02.000000 condynsate-0.6.1/src/condynsate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 15:36:02.000000 condynsate-0.6.1/src/condynsate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2024-04-03 15:36:02.000000 condynsate-0.6.1/src/condynsate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-03 15:36:02.000000 condynsate-0.6.1/src/condynsate.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 18:09:52.144684 condynsate-0.6.2/
+-rw-rw-rw-   0        0        0     1092 2023-11-24 19:50:22.000000 condynsate-0.6.2/LICENSE
+-rw-rw-rw-   0        0        0     4875 2024-04-03 18:09:52.142734 condynsate-0.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2391 2024-03-21 21:05:21.000000 condynsate-0.6.2/README.md
+-rw-rw-rw-   0        0        0     1439 2024-04-03 18:00:15.000000 condynsate-0.6.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-03 18:09:52.144684 condynsate-0.6.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-03 18:09:52.085695 condynsate-0.6.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-03 18:09:52.105223 condynsate-0.6.2/src/condynsate/
+drwxrwxrwx   0        0        0        0 2024-04-03 18:09:52.139737 condynsate-0.6.2/src/condynsate/__assets__/
+-rw-rw-rw-   0        0        0    36584 2023-11-24 19:50:22.000000 condynsate-0.6.2/src/condynsate/__assets__/arrow_ccw.stl
+-rw-rw-rw-   0        0        0    36584 2023-11-24 19:50:22.000000 condynsate-0.6.2/src/condynsate/__assets__/arrow_cw.stl
+-rw-rw-rw-   0        0        0     6784 2023-11-24 19:50:22.000000 condynsate-0.6.2/src/condynsate/__assets__/arrow_lin.stl
+-rw-rw-rw-   0        0        0     6379 2023-11-24 19:50:22.000000 condynsate-0.6.2/src/condynsate/__assets__/check.png
+-rw-rw-rw-   0        0        0      684 2023-11-24 19:50:22.000000 condynsate-0.6.2/src/condynsate/__assets__/cube.stl
+-rw-rw-rw-   0        0        0    12684 2023-12-12 22:20:42.000000 condynsate-0.6.2/src/condynsate/__assets__/cylinder.stl
+-rw-rw-rw-   0        0        0    12684 2023-12-12 22:33:34.000000 condynsate-0.6.2/src/condynsate/__assets__/cylinder_lower_origin.stl
+-rw-rw-rw-   0        0        0    11484 2024-01-05 02:07:25.000000 condynsate-0.6.2/src/condynsate/__assets__/gate_med.stl
+-rw-rw-rw-   0        0        0     4084 2024-01-05 02:03:45.000000 condynsate-0.6.2/src/condynsate/__assets__/gate_short.stl
+-rw-rw-rw-   0        0        0    11484 2024-01-05 02:08:19.000000 condynsate-0.6.2/src/condynsate/__assets__/gate_tall.stl
+-rw-rw-rw-   0        0        0      344 2023-11-24 19:50:22.000000 condynsate-0.6.2/src/condynsate/__assets__/plane_big.obj
+-rw-rw-rw-   0        0        0      332 2023-11-24 19:50:22.000000 condynsate-0.6.2/src/condynsate/__assets__/plane_med.obj
+-rw-rw-rw-   0        0        0      320 2023-11-24 19:50:22.000000 condynsate-0.6.2/src/condynsate/__assets__/plane_small.obj
+-rw-rw-rw-   0        0        0      384 2023-11-24 19:50:22.000000 condynsate-0.6.2/src/condynsate/__assets__/pyramid.stl
+-rw-rw-rw-   0        0        0    61284 2023-11-24 19:50:22.000000 condynsate-0.6.2/src/condynsate/__assets__/sphere.stl
+-rw-rw-rw-   0        0        0      153 2024-04-03 18:00:15.000000 condynsate-0.6.2/src/condynsate/__init__.py
+-rw-rw-rw-   0        0        0    44652 2023-12-15 21:36:13.000000 condynsate-0.6.2/src/condynsate/animator.py
+-rw-rw-rw-   0        0        0     8209 2024-02-06 15:55:34.000000 condynsate-0.6.2/src/condynsate/keyboard.py
+-rw-rw-rw-   0        0        0   145857 2024-04-03 18:00:09.000000 condynsate-0.6.2/src/condynsate/simulator.py
+-rw-rw-rw-   0        0        0    10335 2024-03-26 22:00:32.000000 condynsate-0.6.2/src/condynsate/utils.py
+-rw-rw-rw-   0        0        0    22362 2024-04-02 19:38:52.000000 condynsate-0.6.2/src/condynsate/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:09:52.141721 condynsate-0.6.2/src/condynsate.egg-info/
+-rw-rw-rw-   0        0        0     4875 2024-04-03 18:09:52.000000 condynsate-0.6.2/src/condynsate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      981 2024-04-03 18:09:52.000000 condynsate-0.6.2/src/condynsate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 18:09:52.000000 condynsate-0.6.2/src/condynsate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2024-04-03 18:09:52.000000 condynsate-0.6.2/src/condynsate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-03 18:09:52.000000 condynsate-0.6.2/src/condynsate.egg-info/top_level.txt
```

### Comparing `condynsate-0.6.1/LICENSE` & `condynsate-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.1/PKG-INFO` & `condynsate-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: condynsate
-Version: 0.6.1
+Version: 0.6.2
 Summary: Simulates and visualizes articulated systems in real time
 Author-email: Grayson Schaer <gschaer2@illinois.edu>
 License: MIT License
         
         Copyright (c) 2023 Grayson Schaer
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `condynsate-0.6.1/README.md` & `condynsate-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.1/pyproject.toml` & `condynsate-0.6.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "condynsate"
-version = "0.6.1"
+version = "0.6.2"
 description = "Simulates and visualizes articulated systems in real time"
 readme = "README.md"
 authors = [{ name = "Grayson Schaer", email = "gschaer2@illinois.edu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `condynsate-0.6.1/src/condynsate/__assets__/arrow_ccw.stl` & `condynsate-0.6.2/src/condynsate/__assets__/arrow_ccw.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.1/src/condynsate/__assets__/arrow_cw.stl` & `condynsate-0.6.2/src/condynsate/__assets__/arrow_cw.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.1/src/condynsate/__assets__/arrow_lin.stl` & `condynsate-0.6.2/src/condynsate/__assets__/arrow_lin.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.1/src/condynsate/__assets__/check.png` & `condynsate-0.6.2/src/condynsate/__assets__/check.png`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.1/src/condynsate/__assets__/cylinder.stl` & `condynsate-0.6.2/src/condynsate/__assets__/cylinder.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.1/src/condynsate/__assets__/cylinder_lower_origin.stl` & `condynsate-0.6.2/src/condynsate/__assets__/cylinder_lower_origin.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.1/src/condynsate/__assets__/gate_med.stl` & `condynsate-0.6.2/src/condynsate/__assets__/gate_med.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.1/src/condynsate/__assets__/gate_short.stl` & `condynsate-0.6.2/src/condynsate/__assets__/gate_short.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.1/src/condynsate/__assets__/gate_tall.stl` & `condynsate-0.6.2/src/condynsate/__assets__/gate_tall.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.1/src/condynsate/__assets__/sphere.stl` & `condynsate-0.6.2/src/condynsate/__assets__/sphere.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.1/src/condynsate/animator.py` & `condynsate-0.6.2/src/condynsate/animator.py`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.1/src/condynsate/keyboard.py` & `condynsate-0.6.2/src/condynsate/keyboard.py`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.1/src/condynsate/simulator.py` & `condynsate-0.6.2/src/condynsate/simulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,14 +114,15 @@
         self.engine = bc.BulletClient(connection_mode=pybullet.DIRECT)
         
         # Configure gravity
         self.set_gravity(gravity)
         
         # Time tracking variables
         self.start_epoch = -1.0
+        self.pause_elapsed_time = 0.0
         self.time = 0.0
         self.dt = 0.01
         self.num_steps = 0
         
         # Configure physics engine parameters
         self.engine.setPhysicsEngineParameter(
             fixedTimeStep=self.dt,
@@ -3508,14 +3509,15 @@
         # Do nothing if paused
         if self.paused:
             return
         
         # Note the simulation is no longer done and reset the time
         self.is_done = False
         self.start_epoch = -1.0
+        self.pause_elapsed_time = 0.0
         self.time = 0.
         self.num_steps = 0
 
         # Reset visualizer frame rate
         self.frame_time_target = 0.0
         self.prev_frame_time = -1.0 / self.visualization_fr
         self.vis_time_okay = True
@@ -3621,28 +3623,29 @@
             time.sleep(0.05)
             if isinstance(self.ani, Animator):
                 self.ani.flush_events()
             if self.is_pressed("space"):
                 self.paused = False
                 print("RESUME")
                 time.sleep(0.2)
+                self.pause_elapsed_time += time.time()-self.pause_start_time
                 return 1 # Return end pause code
             return 2 # Return paused code
   
         # Reset upon request
         if self.is_pressed("backspace"):
             self.reset()
             time.sleep(0.2)
             print("RESET")
             return 3 # Return reset code
 
         # Get the real time elapsed since simulation was last reset
         if self.start_epoch == -1.0:
             self.start_epoch = time.time()
-        current_time = time.time() - self.start_epoch
+        current_time = time.time() - self.start_epoch - self.pause_elapsed_time
 
         # Step the physics engine
         self.engine.stepSimulation()
         self.time = self.time + self.dt
         self.num_steps += 1
     
         # Based on the visualizer frame rate, determine if it is time to 
@@ -3677,14 +3680,15 @@
             
             # Wait for the perscribed amount of time to put in real time
             if time_to_wait > 0:
                 time.sleep(time_to_wait)
 
         # Pause upon request
         if self.is_pressed("space"):
+            self.pause_start_time = time.time()
             self.paused = True
             if isinstance(self.ani, Animator):
                 self.ani.flush_events()
             print("PAUSED")
             time.sleep(0.2)
             return 4 # Return start pause code
```

### Comparing `condynsate-0.6.1/src/condynsate/utils.py` & `condynsate-0.6.2/src/condynsate/utils.py`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.1/src/condynsate/visualizer.py` & `condynsate-0.6.2/src/condynsate/visualizer.py`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.1/src/condynsate.egg-info/PKG-INFO` & `condynsate-0.6.2/src/condynsate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: condynsate
-Version: 0.6.1
+Version: 0.6.2
 Summary: Simulates and visualizes articulated systems in real time
 Author-email: Grayson Schaer <gschaer2@illinois.edu>
 License: MIT License
         
         Copyright (c) 2023 Grayson Schaer
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `condynsate-0.6.1/src/condynsate.egg-info/SOURCES.txt` & `condynsate-0.6.2/src/condynsate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

