# Comparing `tmp/GHEDesigner-1.4.tar.gz` & `tmp/GHEDesigner-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GHEDesigner-1.4.tar", last modified: Thu Feb 29 02:06:00 2024, max compression
+gzip compressed data, was "GHEDesigner-1.5.tar", last modified: Wed Apr  3 20:56:58 2024, max compression
```

## Comparing `GHEDesigner-1.4.tar` & `GHEDesigner-1.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:06:00.833208 GHEDesigner-1.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:06:00.829208 GHEDesigner-1.4/GHEDesigner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13868 2024-02-29 02:06:00.000000 GHEDesigner-1.4/GHEDesigner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-02-29 02:06:00.000000 GHEDesigner-1.4/GHEDesigner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 02:06:00.000000 GHEDesigner-1.4/GHEDesigner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-29 02:06:00.000000 GHEDesigner-1.4/GHEDesigner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-29 02:06:00.000000 GHEDesigner-1.4/GHEDesigner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-29 02:06:00.000000 GHEDesigner-1.4/GHEDesigner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-02-29 02:05:57.000000 GHEDesigner-1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13868 2024-02-29 02:06:00.833208 GHEDesigner-1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11641 2024-02-29 02:05:57.000000 GHEDesigner-1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:06:00.833208 GHEDesigner-1.4/ghedesigner/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-29 02:05:57.000000 GHEDesigner-1.4/ghedesigner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-02-29 02:05:57.000000 GHEDesigner-1.4/ghedesigner/borehole.py
--rw-r--r--   0 runner    (1001) docker     (127)    21430 2024-02-29 02:05:57.000000 GHEDesigner-1.4/ghedesigner/borehole_heat_exchangers.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-29 02:05:57.000000 GHEDesigner-1.4/ghedesigner/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-02-29 02:05:57.000000 GHEDesigner-1.4/ghedesigner/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)    13519 2024-02-29 02:05:57.000000 GHEDesigner-1.4/ghedesigner/design.py
--rw-r--r--   0 runner    (1001) docker     (127)    13825 2024-02-29 02:05:57.000000 GHEDesigner-1.4/ghedesigner/domains.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-02-29 02:05:57.000000 GHEDesigner-1.4/ghedesigner/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-02-29 02:05:57.000000 GHEDesigner-1.4/ghedesigner/feature_recognition.py
--rw-r--r--   0 runner    (1001) docker     (127)     5235 2024-02-29 02:05:57.000000 GHEDesigner-1.4/ghedesigner/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)    13593 2024-02-29 02:05:57.000000 GHEDesigner-1.4/ghedesigner/gfunction.py
--rw-r--r--   0 runner    (1001) docker     (127)    13684 2024-02-29 02:05:57.000000 GHEDesigner-1.4/ghedesigner/ground_heat_exchangers.py
--rw-r--r--   0 runner    (1001) docker     (127)    34422 2024-02-29 02:05:57.000000 GHEDesigner-1.4/ghedesigner/ground_loads.py
--rw-r--r--   0 runner    (1001) docker     (127)    40230 2024-02-29 02:05:57.000000 GHEDesigner-1.4/ghedesigner/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4595 2024-02-29 02:05:57.000000 GHEDesigner-1.4/ghedesigner/media.py
--rw-r--r--   0 runner    (1001) docker     (127)    34923 2024-02-29 02:05:57.000000 GHEDesigner-1.4/ghedesigner/output.py
--rw-r--r--   0 runner    (1001) docker     (127)    15065 2024-02-29 02:05:57.000000 GHEDesigner-1.4/ghedesigner/radial_numerical_borehole.py
--rw-r--r--   0 runner    (1001) docker     (127)    32742 2024-02-29 02:05:57.000000 GHEDesigner-1.4/ghedesigner/rowwise.py
--rw-r--r--   0 runner    (1001) docker     (127)    37846 2024-02-29 02:05:57.000000 GHEDesigner-1.4/ghedesigner/search_routines.py
--rw-r--r--   0 runner    (1001) docker     (127)     8864 2024-02-29 02:05:57.000000 GHEDesigner-1.4/ghedesigner/shape.py
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-02-29 02:05:57.000000 GHEDesigner-1.4/ghedesigner/simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8037 2024-02-29 02:05:57.000000 GHEDesigner-1.4/ghedesigner/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     5417 2024-02-29 02:05:57.000000 GHEDesigner-1.4/ghedesigner/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-02-29 02:06:00.833208 GHEDesigner-1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-02-29 02:05:57.000000 GHEDesigner-1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:56:58.097120 GHEDesigner-1.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:56:58.093120 GHEDesigner-1.5/GHEDesigner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13868 2024-04-03 20:56:57.000000 GHEDesigner-1.5/GHEDesigner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-03 20:56:57.000000 GHEDesigner-1.5/GHEDesigner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 20:56:57.000000 GHEDesigner-1.5/GHEDesigner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-03 20:56:57.000000 GHEDesigner-1.5/GHEDesigner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-03 20:56:57.000000 GHEDesigner-1.5/GHEDesigner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-03 20:56:57.000000 GHEDesigner-1.5/GHEDesigner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-03 20:56:55.000000 GHEDesigner-1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13868 2024-04-03 20:56:58.097120 GHEDesigner-1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11641 2024-04-03 20:56:55.000000 GHEDesigner-1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:56:58.097120 GHEDesigner-1.5/ghedesigner/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-03 20:56:55.000000 GHEDesigner-1.5/ghedesigner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-03 20:56:55.000000 GHEDesigner-1.5/ghedesigner/borehole.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21430 2024-04-03 20:56:55.000000 GHEDesigner-1.5/ghedesigner/borehole_heat_exchangers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-03 20:56:55.000000 GHEDesigner-1.5/ghedesigner/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-04-03 20:56:55.000000 GHEDesigner-1.5/ghedesigner/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13585 2024-04-03 20:56:55.000000 GHEDesigner-1.5/ghedesigner/design.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14034 2024-04-03 20:56:55.000000 GHEDesigner-1.5/ghedesigner/domains.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-03 20:56:55.000000 GHEDesigner-1.5/ghedesigner/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-03 20:56:55.000000 GHEDesigner-1.5/ghedesigner/feature_recognition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5570 2024-04-03 20:56:55.000000 GHEDesigner-1.5/ghedesigner/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13593 2024-04-03 20:56:55.000000 GHEDesigner-1.5/ghedesigner/gfunction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13684 2024-04-03 20:56:55.000000 GHEDesigner-1.5/ghedesigner/ground_heat_exchangers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34422 2024-04-03 20:56:55.000000 GHEDesigner-1.5/ghedesigner/ground_loads.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40230 2024-04-03 20:56:55.000000 GHEDesigner-1.5/ghedesigner/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4595 2024-04-03 20:56:55.000000 GHEDesigner-1.5/ghedesigner/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34923 2024-04-03 20:56:55.000000 GHEDesigner-1.5/ghedesigner/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15065 2024-04-03 20:56:55.000000 GHEDesigner-1.5/ghedesigner/radial_numerical_borehole.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32742 2024-04-03 20:56:55.000000 GHEDesigner-1.5/ghedesigner/rowwise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37846 2024-04-03 20:56:55.000000 GHEDesigner-1.5/ghedesigner/search_routines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8858 2024-04-03 20:56:55.000000 GHEDesigner-1.5/ghedesigner/shape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-03 20:56:55.000000 GHEDesigner-1.5/ghedesigner/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8037 2024-04-03 20:56:55.000000 GHEDesigner-1.5/ghedesigner/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5417 2024-04-03 20:56:55.000000 GHEDesigner-1.5/ghedesigner/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-03 20:56:58.097120 GHEDesigner-1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-03 20:56:55.000000 GHEDesigner-1.5/setup.py
```

### Comparing `GHEDesigner-1.4/GHEDesigner.egg-info/PKG-INFO` & `GHEDesigner-1.5/GHEDesigner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GHEDesigner
-Version: 1.4
+Version: 1.5
 Summary: A ground heat exchanger design tool with the capability to select and size flexibly configured borehole fields that are customized for specific building and property constraints.
 Home-page: https://github.com/BETSRG/GHEDesigner
 Author: Jeffrey D. Spitler
 Author-email: spitler@okstate.edu
 License: BSD-3
 Description: # GHEDesigner - A Flexible and Automatic Ground Heat Exchanger Design Tool
```

### Comparing `GHEDesigner-1.4/GHEDesigner.egg-info/SOURCES.txt` & `GHEDesigner-1.5/GHEDesigner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GHEDesigner-1.4/LICENSE` & `GHEDesigner-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `GHEDesigner-1.4/PKG-INFO` & `GHEDesigner-1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GHEDesigner
-Version: 1.4
+Version: 1.5
 Summary: A ground heat exchanger design tool with the capability to select and size flexibly configured borehole fields that are customized for specific building and property constraints.
 Home-page: https://github.com/BETSRG/GHEDesigner
 Author: Jeffrey D. Spitler
 Author-email: spitler@okstate.edu
 License: BSD-3
 Description: # GHEDesigner - A Flexible and Automatic Ground Heat Exchanger Design Tool
```

### Comparing `GHEDesigner-1.4/README.md` & `GHEDesigner-1.5/README.md`

 * *Files identical despite different names*

### Comparing `GHEDesigner-1.4/ghedesigner/borehole_heat_exchangers.py` & `GHEDesigner-1.5/ghedesigner/borehole_heat_exchangers.py`

 * *Files identical despite different names*

### Comparing `GHEDesigner-1.4/ghedesigner/coordinates.py` & `GHEDesigner-1.5/ghedesigner/coordinates.py`

 * *Files identical despite different names*

### Comparing `GHEDesigner-1.4/ghedesigner/design.py` & `GHEDesigner-1.5/ghedesigner/design.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,31 +225,32 @@
 
 
 class DesignBiRectangleConstrained(DesignBase):
     def __init__(self, v_flow: float, _borehole: GHEBorehole, bhe_type: BHPipeType,
                  fluid: GHEFluid, pipe: Pipe, grout: Grout, soil: Soil, sim_params: SimulationParameters,
                  geometric_constraints: GeometricConstraintsBiRectangleConstrained,
                  hourly_extraction_ground_loads: list, method: TimestepType,
-                 flow_type: FlowConfigType = FlowConfigType.BOREHOLE, load_years=None):
+                 flow_type: FlowConfigType = FlowConfigType.BOREHOLE, load_years=None, keep_contour=[True, False]):
         super().__init__(v_flow, _borehole, bhe_type, fluid, pipe, grout, soil, sim_params, geometric_constraints,
                          hourly_extraction_ground_loads, method, flow_type, load_years)
         self.geometric_constraints = geometric_constraints
         self.coordinates_domain_nested, self.fieldDescriptors = polygonal_land_constraint(
             self.geometric_constraints.b_min,
             self.geometric_constraints.b_max_x,
             self.geometric_constraints.b_max_y,
             self.geometric_constraints.property_boundary,
             self.geometric_constraints.no_go_boundaries,
+            keep_contour=keep_contour
         )
 
-    def find_design(self, disp=False) -> Bisection2D:
+    def find_design(self, disp=False) -> BisectionZD:
         if disp:
             title = "Find bi-rectangle_constrained..."
             print(title + "\n" + len(title) * "=")
-        return Bisection2D(
+        return BisectionZD(
             self.coordinates_domain_nested,
             self.fieldDescriptors,
             self.V_flow,
             self.borehole,
             self.bhe_type,
             self.fluid,
             self.pipe,
```

### Comparing `GHEDesigner-1.4/ghedesigner/domains.py` & `GHEDesigner-1.5/ghedesigner/domains.py`

 * *Files 1% similar despite different names*

```diff
@@ -358,15 +358,16 @@
 
     bi_rectangle_zoned_nested_domain.append(domain)
     field_descriptors.append(f_d)
 
     return bi_rectangle_zoned_nested_domain, field_descriptors
 
 
-def polygonal_land_constraint(b_min, b_max_x, b_max_y, property_boundary, no_go_boundaries=None):
+def polygonal_land_constraint(b_min, b_max_x, b_max_y, property_boundary, no_go_boundaries=None,
+                              keep_contour=[True, False]):
     if no_go_boundaries is None:
         no_go_boundaries = []
 
     outer_rectangle = determine_largest_rectangle(property_boundary)
 
     x, y = list(zip(*outer_rectangle))
     length = max(x)
@@ -375,21 +376,24 @@
 
     coordinates_domain_nested_cutout = []
 
     for domain in coordinates_domain_nested:
         new_coordinates_domain = []
         for coordinates in domain:
             # Remove boreholes outside of property
-            new_coordinates = remove_cutout(coordinates, property_boundary, remove_inside=False)
+            new_coordinates = remove_cutout(coordinates, property_boundary, remove_inside=False,
+                                            keep_contour=keep_contour[0])
+            if len(new_coordinates) == 0:
+                continue
             # Remove boreholes inside of building
+            if len(no_go_boundaries) > 0:
+                new_coordinates = remove_cutout(new_coordinates, no_go_boundaries, remove_inside=True,
+                                                keep_contour=keep_contour[1])
             if len(new_coordinates) == 0:
                 continue
-            for no_go_zone in no_go_boundaries:
-                new_coordinates = remove_cutout(new_coordinates, no_go_zone, remove_inside=True,
-                                                keep_contour=False)
             new_coordinates_domain.append(new_coordinates)
         coordinates_domain_nested_cutout.append(new_coordinates_domain)
 
     coordinates_domain_nested_cutout_reordered = []
     field_descriptors_reordered = []
     for idx, domain in enumerate(coordinates_domain_nested_cutout):
         domain_reordered, f_d_reordered = reorder_domain(domain, field_descriptors[idx])
```

### Comparing `GHEDesigner-1.4/ghedesigner/enums.py` & `GHEDesigner-1.5/ghedesigner/enums.py`

 * *Files identical despite different names*

### Comparing `GHEDesigner-1.4/ghedesigner/geometry.py` & `GHEDesigner-1.5/ghedesigner/geometry.py`

 * *Files 8% similar despite different names*

```diff
@@ -80,16 +80,25 @@
     """
 
     def __init__(self, b_min: float, b_max_x: float, b_max_y: float, property_boundary, no_go_boundaries):
         super().__init__()
         self.b_min = b_min
         self.b_max_x = b_max_x
         self.b_max_y = b_max_y
-        self.property_boundary = property_boundary
-        self.no_go_boundaries = no_go_boundaries
+
+        if len(no_go_boundaries) > 0 and isinstance(no_go_boundaries[0][0], (int, float)):
+            self.no_go_boundaries = [no_go_boundaries]
+        else:
+            self.no_go_boundaries = no_go_boundaries
+
+        if len(property_boundary) > 0 and isinstance(property_boundary[0][0], (int, float)):
+            self.property_boundary = [property_boundary]
+        else:
+            self.property_boundary = property_boundary
+
         self.type = DesignGeomType.BIRECTANGLECONSTRAINED
 
     def to_input(self) -> dict:
         return {'b_min': self.b_min,
                 'b_max_x': self.b_max_x,
                 'b_max_y': self.b_max_y,
                 'property_boundary': self.property_boundary,
```

### Comparing `GHEDesigner-1.4/ghedesigner/gfunction.py` & `GHEDesigner-1.5/ghedesigner/gfunction.py`

 * *Files identical despite different names*

### Comparing `GHEDesigner-1.4/ghedesigner/ground_heat_exchangers.py` & `GHEDesigner-1.5/ghedesigner/ground_heat_exchangers.py`

 * *Files identical despite different names*

### Comparing `GHEDesigner-1.4/ghedesigner/ground_loads.py` & `GHEDesigner-1.5/ghedesigner/ground_loads.py`

 * *Files identical despite different names*

### Comparing `GHEDesigner-1.4/ghedesigner/manager.py` & `GHEDesigner-1.5/ghedesigner/manager.py`

 * *Files identical despite different names*

### Comparing `GHEDesigner-1.4/ghedesigner/media.py` & `GHEDesigner-1.5/ghedesigner/media.py`

 * *Files identical despite different names*

### Comparing `GHEDesigner-1.4/ghedesigner/output.py` & `GHEDesigner-1.5/ghedesigner/output.py`

 * *Files identical despite different names*

### Comparing `GHEDesigner-1.4/ghedesigner/radial_numerical_borehole.py` & `GHEDesigner-1.5/ghedesigner/radial_numerical_borehole.py`

 * *Files identical despite different names*

### Comparing `GHEDesigner-1.4/ghedesigner/rowwise.py` & `GHEDesigner-1.5/ghedesigner/rowwise.py`

 * *Files identical despite different names*

### Comparing `GHEDesigner-1.4/ghedesigner/search_routines.py` & `GHEDesigner-1.5/ghedesigner/search_routines.py`

 * *Files identical despite different names*

### Comparing `GHEDesigner-1.4/ghedesigner/shape.py` & `GHEDesigner-1.5/ghedesigner/shape.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,15 +213,15 @@
         else:
             return []
     rx = (c2 - c1) / (a1 - a2)
     ry = a1 * (c2 - c1) / (a1 - a2) + c1
     return [[rx, ry]]
 
 
-def point_polygon_check(contour, point):
+def point_polygon_check(contour, point, on_edge_tolerance=0.001):
     """
     Mimics pointPolygonTest from OpenCV-Python
 
     Adapted from the methods outlined in the links below.
     https://stackoverflow.com/a/63436180/5965685
     https://stackoverflow.com/a/17693146/5965685
 
@@ -237,16 +237,14 @@
     # and the line vertices add to the distance between the line vertices
     # if they are within tolerance, the point is co-linear
     # if not, it is off the line
 
     def distance(pt_1, pt_2) -> float:
         return sqrt((pt_1[0] - pt_2[0]) ** 2 + (pt_1[1] - pt_2[1]) ** 2)
 
-    on_edge_tolerance = 0.001
-
     for idx, vertex in enumerate(contour):
         v1 = contour[idx - 1]
         v2 = vertex
         test_dist = distance(v1, point) + distance(v2, point)
         v12_dist = distance(v1, v2)
 
         if abs(test_dist - v12_dist) < on_edge_tolerance:
```

### Comparing `GHEDesigner-1.4/ghedesigner/simulation.py` & `GHEDesigner-1.5/ghedesigner/simulation.py`

 * *Files identical despite different names*

### Comparing `GHEDesigner-1.4/ghedesigner/utilities.py` & `GHEDesigner-1.5/ghedesigner/utilities.py`

 * *Files identical despite different names*

### Comparing `GHEDesigner-1.4/ghedesigner/validate.py` & `GHEDesigner-1.5/ghedesigner/validate.py`

 * *Files identical despite different names*

### Comparing `GHEDesigner-1.4/setup.py` & `GHEDesigner-1.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 short_description = """A ground heat exchanger design tool with the capability
 to select and size flexibly configured borehole fields that are customized
 for specific building and property constraints."""
 
 setup(
     name='GHEDesigner',
     install_requires=[
-        'click>=8.1.7',
-        'jsonschema>=4.19.1',
-        'numpy>=1.24.2',
-        'pygfunction>=2.2.2',
-        'scipy>=1.10.1'
+        'click~=8.1',
+        'jsonschema~=4.19',
+        'numpy~=1.24',
+        'pygfunction~=2.2',
+        'scipy~=1.10'
     ],
     url='https://github.com/BETSRG/GHEDesigner',
     description=short_description,
     license='BSD-3',
     long_description=readme_contents,
     long_description_content_type='text/markdown',
     version=VERSION,
```

