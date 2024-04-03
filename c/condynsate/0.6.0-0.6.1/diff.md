# Comparing `tmp/condynsate-0.6.0.tar.gz` & `tmp/condynsate-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "condynsate-0.6.0.tar", last modified: Tue Apr  2 20:16:51 2024, max compression
+gzip compressed data, was "condynsate-0.6.1.tar", last modified: Wed Apr  3 15:36:02 2024, max compression
```

## Comparing `condynsate-0.6.0.tar` & `condynsate-0.6.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 20:16:51.961443 condynsate-0.6.0/
--rw-rw-rw-   0        0        0     1092 2023-11-24 19:50:22.000000 condynsate-0.6.0/LICENSE
--rw-rw-rw-   0        0        0     4875 2024-04-02 20:16:51.961443 condynsate-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     2391 2024-03-21 21:05:21.000000 condynsate-0.6.0/README.md
--rw-rw-rw-   0        0        0     1439 2024-04-02 20:16:17.000000 condynsate-0.6.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-02 20:16:51.961443 condynsate-0.6.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-02 20:16:51.895143 condynsate-0.6.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-02 20:16:51.918182 condynsate-0.6.0/src/condynsate/
-drwxrwxrwx   0        0        0        0 2024-04-02 20:16:51.961443 condynsate-0.6.0/src/condynsate/__assets__/
--rw-rw-rw-   0        0        0    36584 2023-11-24 19:50:22.000000 condynsate-0.6.0/src/condynsate/__assets__/arrow_ccw.stl
--rw-rw-rw-   0        0        0    36584 2023-11-24 19:50:22.000000 condynsate-0.6.0/src/condynsate/__assets__/arrow_cw.stl
--rw-rw-rw-   0        0        0     6784 2023-11-24 19:50:22.000000 condynsate-0.6.0/src/condynsate/__assets__/arrow_lin.stl
--rw-rw-rw-   0        0        0     6379 2023-11-24 19:50:22.000000 condynsate-0.6.0/src/condynsate/__assets__/check.png
--rw-rw-rw-   0        0        0      684 2023-11-24 19:50:22.000000 condynsate-0.6.0/src/condynsate/__assets__/cube.stl
--rw-rw-rw-   0        0        0    12684 2023-12-12 22:20:42.000000 condynsate-0.6.0/src/condynsate/__assets__/cylinder.stl
--rw-rw-rw-   0        0        0    12684 2023-12-12 22:33:34.000000 condynsate-0.6.0/src/condynsate/__assets__/cylinder_lower_origin.stl
--rw-rw-rw-   0        0        0    11484 2024-01-05 02:07:25.000000 condynsate-0.6.0/src/condynsate/__assets__/gate_med.stl
--rw-rw-rw-   0        0        0     4084 2024-01-05 02:03:45.000000 condynsate-0.6.0/src/condynsate/__assets__/gate_short.stl
--rw-rw-rw-   0        0        0    11484 2024-01-05 02:08:19.000000 condynsate-0.6.0/src/condynsate/__assets__/gate_tall.stl
--rw-rw-rw-   0        0        0      344 2023-11-24 19:50:22.000000 condynsate-0.6.0/src/condynsate/__assets__/plane_big.obj
--rw-rw-rw-   0        0        0      332 2023-11-24 19:50:22.000000 condynsate-0.6.0/src/condynsate/__assets__/plane_med.obj
--rw-rw-rw-   0        0        0      320 2023-11-24 19:50:22.000000 condynsate-0.6.0/src/condynsate/__assets__/plane_small.obj
--rw-rw-rw-   0        0        0      384 2023-11-24 19:50:22.000000 condynsate-0.6.0/src/condynsate/__assets__/pyramid.stl
--rw-rw-rw-   0        0        0    61284 2023-11-24 19:50:22.000000 condynsate-0.6.0/src/condynsate/__assets__/sphere.stl
--rw-rw-rw-   0        0        0      153 2024-04-02 20:16:17.000000 condynsate-0.6.0/src/condynsate/__init__.py
--rw-rw-rw-   0        0        0    44652 2023-12-15 21:36:13.000000 condynsate-0.6.0/src/condynsate/animator.py
--rw-rw-rw-   0        0        0     8209 2024-02-06 15:55:34.000000 condynsate-0.6.0/src/condynsate/keyboard.py
--rw-rw-rw-   0        0        0   144586 2024-04-02 19:53:04.000000 condynsate-0.6.0/src/condynsate/simulator.py
--rw-rw-rw-   0        0        0    10335 2024-03-26 22:00:32.000000 condynsate-0.6.0/src/condynsate/utils.py
--rw-rw-rw-   0        0        0    22362 2024-04-02 19:38:52.000000 condynsate-0.6.0/src/condynsate/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:16:51.961443 condynsate-0.6.0/src/condynsate.egg-info/
--rw-rw-rw-   0        0        0     4875 2024-04-02 20:16:51.000000 condynsate-0.6.0/src/condynsate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      981 2024-04-02 20:16:51.000000 condynsate-0.6.0/src/condynsate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 20:16:51.000000 condynsate-0.6.0/src/condynsate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2024-04-02 20:16:51.000000 condynsate-0.6.0/src/condynsate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-02 20:16:51.000000 condynsate-0.6.0/src/condynsate.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 15:36:02.383364 condynsate-0.6.1/
+-rw-rw-rw-   0        0        0     1092 2023-11-24 19:50:22.000000 condynsate-0.6.1/LICENSE
+-rw-rw-rw-   0        0        0     4875 2024-04-03 15:36:02.383364 condynsate-0.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2391 2024-03-21 21:05:21.000000 condynsate-0.6.1/README.md
+-rw-rw-rw-   0        0        0     1439 2024-04-03 15:35:20.000000 condynsate-0.6.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-03 15:36:02.383364 condynsate-0.6.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-03 15:36:02.289544 condynsate-0.6.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-03 15:36:02.305170 condynsate-0.6.1/src/condynsate/
+drwxrwxrwx   0        0        0        0 2024-04-03 15:36:02.383364 condynsate-0.6.1/src/condynsate/__assets__/
+-rw-rw-rw-   0        0        0    36584 2023-11-24 19:50:22.000000 condynsate-0.6.1/src/condynsate/__assets__/arrow_ccw.stl
+-rw-rw-rw-   0        0        0    36584 2023-11-24 19:50:22.000000 condynsate-0.6.1/src/condynsate/__assets__/arrow_cw.stl
+-rw-rw-rw-   0        0        0     6784 2023-11-24 19:50:22.000000 condynsate-0.6.1/src/condynsate/__assets__/arrow_lin.stl
+-rw-rw-rw-   0        0        0     6379 2023-11-24 19:50:22.000000 condynsate-0.6.1/src/condynsate/__assets__/check.png
+-rw-rw-rw-   0        0        0      684 2023-11-24 19:50:22.000000 condynsate-0.6.1/src/condynsate/__assets__/cube.stl
+-rw-rw-rw-   0        0        0    12684 2023-12-12 22:20:42.000000 condynsate-0.6.1/src/condynsate/__assets__/cylinder.stl
+-rw-rw-rw-   0        0        0    12684 2023-12-12 22:33:34.000000 condynsate-0.6.1/src/condynsate/__assets__/cylinder_lower_origin.stl
+-rw-rw-rw-   0        0        0    11484 2024-01-05 02:07:25.000000 condynsate-0.6.1/src/condynsate/__assets__/gate_med.stl
+-rw-rw-rw-   0        0        0     4084 2024-01-05 02:03:45.000000 condynsate-0.6.1/src/condynsate/__assets__/gate_short.stl
+-rw-rw-rw-   0        0        0    11484 2024-01-05 02:08:19.000000 condynsate-0.6.1/src/condynsate/__assets__/gate_tall.stl
+-rw-rw-rw-   0        0        0      344 2023-11-24 19:50:22.000000 condynsate-0.6.1/src/condynsate/__assets__/plane_big.obj
+-rw-rw-rw-   0        0        0      332 2023-11-24 19:50:22.000000 condynsate-0.6.1/src/condynsate/__assets__/plane_med.obj
+-rw-rw-rw-   0        0        0      320 2023-11-24 19:50:22.000000 condynsate-0.6.1/src/condynsate/__assets__/plane_small.obj
+-rw-rw-rw-   0        0        0      384 2023-11-24 19:50:22.000000 condynsate-0.6.1/src/condynsate/__assets__/pyramid.stl
+-rw-rw-rw-   0        0        0    61284 2023-11-24 19:50:22.000000 condynsate-0.6.1/src/condynsate/__assets__/sphere.stl
+-rw-rw-rw-   0        0        0      153 2024-04-03 15:35:20.000000 condynsate-0.6.1/src/condynsate/__init__.py
+-rw-rw-rw-   0        0        0    44652 2023-12-15 21:36:13.000000 condynsate-0.6.1/src/condynsate/animator.py
+-rw-rw-rw-   0        0        0     8209 2024-02-06 15:55:34.000000 condynsate-0.6.1/src/condynsate/keyboard.py
+-rw-rw-rw-   0        0        0   145626 2024-04-03 15:34:39.000000 condynsate-0.6.1/src/condynsate/simulator.py
+-rw-rw-rw-   0        0        0    10335 2024-03-26 22:00:32.000000 condynsate-0.6.1/src/condynsate/utils.py
+-rw-rw-rw-   0        0        0    22362 2024-04-02 19:38:52.000000 condynsate-0.6.1/src/condynsate/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-04-03 15:36:02.383364 condynsate-0.6.1/src/condynsate.egg-info/
+-rw-rw-rw-   0        0        0     4875 2024-04-03 15:36:02.000000 condynsate-0.6.1/src/condynsate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      981 2024-04-03 15:36:02.000000 condynsate-0.6.1/src/condynsate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 15:36:02.000000 condynsate-0.6.1/src/condynsate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2024-04-03 15:36:02.000000 condynsate-0.6.1/src/condynsate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-03 15:36:02.000000 condynsate-0.6.1/src/condynsate.egg-info/top_level.txt
```

### Comparing `condynsate-0.6.0/LICENSE` & `condynsate-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.0/PKG-INFO` & `condynsate-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: condynsate
-Version: 0.6.0
+Version: 0.6.1
 Summary: Simulates and visualizes articulated systems in real time
 Author-email: Grayson Schaer <gschaer2@illinois.edu>
 License: MIT License
         
         Copyright (c) 2023 Grayson Schaer
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `condynsate-0.6.0/README.md` & `condynsate-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.0/pyproject.toml` & `condynsate-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "condynsate"
-version = "0.6.0"
+version = "0.6.1"
 description = "Simulates and visualizes articulated systems in real time"
 readme = "README.md"
 authors = [{ name = "Grayson Schaer", email = "gschaer2@illinois.edu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `condynsate-0.6.0/src/condynsate/__assets__/arrow_ccw.stl` & `condynsate-0.6.1/src/condynsate/__assets__/arrow_ccw.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.0/src/condynsate/__assets__/arrow_cw.stl` & `condynsate-0.6.1/src/condynsate/__assets__/arrow_cw.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.0/src/condynsate/__assets__/arrow_lin.stl` & `condynsate-0.6.1/src/condynsate/__assets__/arrow_lin.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.0/src/condynsate/__assets__/check.png` & `condynsate-0.6.1/src/condynsate/__assets__/check.png`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.0/src/condynsate/__assets__/cylinder.stl` & `condynsate-0.6.1/src/condynsate/__assets__/cylinder.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.0/src/condynsate/__assets__/cylinder_lower_origin.stl` & `condynsate-0.6.1/src/condynsate/__assets__/cylinder_lower_origin.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.0/src/condynsate/__assets__/gate_med.stl` & `condynsate-0.6.1/src/condynsate/__assets__/gate_med.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.0/src/condynsate/__assets__/gate_short.stl` & `condynsate-0.6.1/src/condynsate/__assets__/gate_short.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.0/src/condynsate/__assets__/gate_tall.stl` & `condynsate-0.6.1/src/condynsate/__assets__/gate_tall.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.0/src/condynsate/__assets__/sphere.stl` & `condynsate-0.6.1/src/condynsate/__assets__/sphere.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.0/src/condynsate/animator.py` & `condynsate-0.6.1/src/condynsate/animator.py`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.0/src/condynsate/keyboard.py` & `condynsate-0.6.1/src/condynsate/keyboard.py`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.0/src/condynsate/simulator.py` & `condynsate-0.6.1/src/condynsate/simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,20 +112,21 @@
         
         # Connect to pybullet
         self.engine = bc.BulletClient(connection_mode=pybullet.DIRECT)
         
         # Configure gravity
         self.set_gravity(gravity)
         
-        # Configure physics engine parameters
+        # Time tracking variables
+        self.start_epoch = -1.0
         self.time = 0.0
         self.dt = 0.01
-        self.last_step_time = time.time()
-        self.last_vis_time = time.time()
-        self.visualization_fr = visualization_fr
+        self.num_steps = 0
+        
+        # Configure physics engine parameters
         self.engine.setPhysicsEngineParameter(
             fixedTimeStep=self.dt,
             numSubSteps=4,
             restitutionVelocityThreshold=0.05,
             enableFileCaching=0)
         
         # Keep track of all urdfs loaded to simulator
@@ -136,14 +137,19 @@
         self.ccw_arr_map = {}
         
         # Create a visualizer
         if visualization:
             self.vis = Visualizer(grid_vis=False,axes_vis=False)
         else:
             self.vis=None
+        
+        # Create variables to keep track of visualizer frame rate
+        self.visualization_fr = visualization_fr
+        self.frame_time_target = 0.0
+        self.prev_frame_time = -1.0 / self.visualization_fr
         self.vis_time_okay = True
         
         # Create an animator
         if animation:
             self.ani = Animator(fr=animation_fr)
         else:
             self.ani=None
@@ -3501,16 +3507,21 @@
         """
         # Do nothing if paused
         if self.paused:
             return
         
         # Note the simulation is no longer done and reset the time
         self.is_done = False
+        self.start_epoch = -1.0
         self.time = 0.
-        self.last_step_time = time.time()
+        self.num_steps = 0
+
+        # Reset visualizer frame rate
+        self.frame_time_target = 0.0
+        self.prev_frame_time = -1.0 / self.visualization_fr
         self.vis_time_okay = True
         
         # Reset each urdf
         for urdf_obj in self.urdf_objs:
             
             # Reset the base position and orientation of all urdfs
             i = urdf_obj.urdf_id
@@ -3620,51 +3631,67 @@
         # Reset upon request
         if self.is_pressed("backspace"):
             self.reset()
             time.sleep(0.2)
             print("RESET")
             return 3 # Return reset code
 
-        # IF NOT PAUSED, NOT ENDING, AND NOT RESETTING
+        # Get the real time elapsed since simulation was last reset
+        if self.start_epoch == -1.0:
+            self.start_epoch = time.time()
+        current_time = time.time() - self.start_epoch
+
         # Step the physics engine
-        curr_step_time = time.time()
         self.engine.stepSimulation()
         self.time = self.time + self.dt
-
-        # Update the visualizer if it exists
-        time_since_last_vis = curr_step_time - self.last_vis_time
-        self.vis_time_okay=time_since_last_vis >= (1. / self.visualization_fr)
+        self.num_steps += 1
+    
+        # Based on the visualizer frame rate, determine if it is time to 
+        # frame update
+        frame_cond_1 = current_time >= self.frame_time_target
+        frame_cond_2 = self.prev_frame_time < self.frame_time_target
+        frame_cond_3 = self.prev_frame_time >= self.frame_time_target
+        self.vis_time_okay = (frame_cond_1 and frame_cond_2) or frame_cond_3
+    
+        # Update the visualizer
         vis_exists = isinstance(self.vis, Visualizer)
         if self.vis_time_okay and update_vis and vis_exists:
-            self.last_vis_time = curr_step_time
+            
+            # Keep track of number of frames and target frame time
+            self.frame_time_target += 1.0/self.visualization_fr
+            self.prev_frame_time = current_time
+                        
+            # Update all urdfs
             for urdf_obj in self.urdf_objs:
                 if urdf_obj.update_vis:
                     self._update_urdf_visual(urdf_obj)
        
         # Update the animator if it exists
         if update_ani and isinstance(self.ani, Animator):
             self.ani.step()
 
+        # Calculate suspend time if running simulation in real time
+        if real_time:
+            # Get the amount of time to wait to place in real time
+            real_time_target = self.num_steps * self.dt
+            time_to_wait = real_time_target - current_time
+            
+            # Wait for the perscribed amount of time to put in real time
+            if time_to_wait > 0:
+                time.sleep(time_to_wait)
+
         # Pause upon request
         if self.is_pressed("space"):
             self.paused = True
             if isinstance(self.ani, Animator):
                 self.ani.flush_events()
             print("PAUSED")
             time.sleep(0.2)
             return 4 # Return start pause code
 
-        # Calculate suspend time if running in real time
-        if real_time:
-            time_since_last_step = curr_step_time - self.last_step_time
-            time_to_wait = self.dt - time_since_last_step
-            if time_to_wait > 0:
-                time.sleep(time_to_wait)
-        self.last_step_time = curr_step_time
-
         # Check for max time
         if max_time != None:
             if self.time > max_time:
                 self.is_done = True
                 return 5 # Return time out code
 
         return 0 # Return normal code
```

### Comparing `condynsate-0.6.0/src/condynsate/utils.py` & `condynsate-0.6.1/src/condynsate/utils.py`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.0/src/condynsate/visualizer.py` & `condynsate-0.6.1/src/condynsate/visualizer.py`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.0/src/condynsate.egg-info/PKG-INFO` & `condynsate-0.6.1/src/condynsate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: condynsate
-Version: 0.6.0
+Version: 0.6.1
 Summary: Simulates and visualizes articulated systems in real time
 Author-email: Grayson Schaer <gschaer2@illinois.edu>
 License: MIT License
         
         Copyright (c) 2023 Grayson Schaer
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `condynsate-0.6.0/src/condynsate.egg-info/SOURCES.txt` & `condynsate-0.6.1/src/condynsate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

