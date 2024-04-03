# Comparing `tmp/delaunay_watershed_3d-0.3.3.tar.gz` & `tmp/delaunay_watershed_3d-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delaunay_watershed_3d-0.3.3.tar", last modified: Mon Mar 25 16:10:48 2024, max compression
+gzip compressed data, was "delaunay_watershed_3d-0.3.4.tar", last modified: Wed Apr  3 13:48:41 2024, max compression
```

## Comparing `delaunay_watershed_3d-0.3.3.tar` & `delaunay_watershed_3d-0.3.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 perez     (1000) perez     (1000)        0 2024-03-25 16:10:48.525167 delaunay_watershed_3d-0.3.3/
--rw-r--r--   0 perez     (1000) perez     (1000)     8145 2024-03-25 16:10:48.525167 delaunay_watershed_3d-0.3.3/PKG-INFO
--rw-r--r--   0 perez     (1000) perez     (1000)     7069 2024-03-12 15:12:15.000000 delaunay_watershed_3d-0.3.3/README.md
--rw-r--r--   0 perez     (1000) perez     (1000)     1202 2024-02-13 09:09:41.000000 delaunay_watershed_3d-0.3.3/pyproject.toml
--rw-r--r--   0 perez     (1000) perez     (1000)     1072 2024-03-25 16:10:48.525167 delaunay_watershed_3d-0.3.3/setup.cfg
-drwxr-xr-x   0 perez     (1000) perez     (1000)        0 2024-03-25 16:10:48.521834 delaunay_watershed_3d-0.3.3/src/
-drwxr-xr-x   0 perez     (1000) perez     (1000)        0 2024-03-25 16:10:48.525167 delaunay_watershed_3d-0.3.3/src/delaunay_watershed_3d.egg-info/
--rw-r--r--   0 perez     (1000) perez     (1000)     8145 2024-03-25 16:10:48.000000 delaunay_watershed_3d-0.3.3/src/delaunay_watershed_3d.egg-info/PKG-INFO
--rw-r--r--   0 perez     (1000) perez     (1000)      673 2024-03-25 16:10:48.000000 delaunay_watershed_3d-0.3.3/src/delaunay_watershed_3d.egg-info/SOURCES.txt
--rw-r--r--   0 perez     (1000) perez     (1000)        1 2024-03-25 16:10:48.000000 delaunay_watershed_3d-0.3.3/src/delaunay_watershed_3d.egg-info/dependency_links.txt
--rw-r--r--   0 perez     (1000) perez     (1000)      163 2024-03-25 16:10:48.000000 delaunay_watershed_3d-0.3.3/src/delaunay_watershed_3d.egg-info/requires.txt
--rw-r--r--   0 perez     (1000) perez     (1000)        5 2024-03-25 16:10:48.000000 delaunay_watershed_3d-0.3.3/src/delaunay_watershed_3d.egg-info/top_level.txt
-drwxr-xr-x   0 perez     (1000) perez     (1000)        0 2024-03-25 16:10:48.525167 delaunay_watershed_3d-0.3.3/src/dw3d/
--rw-r--r--   0 perez     (1000) perez     (1000)     2513 2024-03-12 15:11:52.000000 delaunay_watershed_3d-0.3.3/src/dw3d/__init__.py
--rw-r--r--   0 perez     (1000) perez     (1000)     6492 2024-03-11 10:17:34.000000 delaunay_watershed_3d-0.3.3/src/dw3d/edt.py
--rw-r--r--   0 perez     (1000) perez     (1000)     8708 2024-03-12 15:19:46.000000 delaunay_watershed_3d-0.3.3/src/dw3d/io.py
--rw-r--r--   0 perez     (1000) perez     (1000)     4089 2024-03-11 16:02:21.000000 delaunay_watershed_3d-0.3.3/src/dw3d/mask_reconstruction.py
--rw-r--r--   0 perez     (1000) perez     (1000)     5850 2024-03-25 16:07:35.000000 delaunay_watershed_3d-0.3.3/src/dw3d/mesh_surgery.py
--rw-r--r--   0 perez     (1000) perez     (1000)     9302 2024-03-25 10:41:42.000000 delaunay_watershed_3d-0.3.3/src/dw3d/mesh_utilities.py
--rw-r--r--   0 perez     (1000) perez     (1000)     2158 2024-03-13 12:48:34.000000 delaunay_watershed_3d-0.3.3/src/dw3d/points_on_edt.py
--rw-r--r--   0 perez     (1000) perez     (1000)    11078 2024-03-25 16:07:02.000000 delaunay_watershed_3d-0.3.3/src/dw3d/reconstruction_algorithm.py
--rw-r--r--   0 perez     (1000) perez     (1000)     5909 2024-03-13 12:49:12.000000 delaunay_watershed_3d-0.3.3/src/dw3d/reconstruction_algorithm_factory.py
--rw-r--r--   0 perez     (1000) perez     (1000)     4161 2024-03-11 10:43:52.000000 delaunay_watershed_3d-0.3.3/src/dw3d/score_computation.py
--rw-r--r--   0 perez     (1000) perez     (1000)     1835 2024-03-08 08:45:06.000000 delaunay_watershed_3d-0.3.3/src/dw3d/segmentation.py
--rw-r--r--   0 perez     (1000) perez     (1000)      894 2024-03-11 14:41:02.000000 delaunay_watershed_3d-0.3.3/src/dw3d/tesselation.py
--rw-r--r--   0 perez     (1000) perez     (1000)     8959 2024-03-25 15:56:35.000000 delaunay_watershed_3d-0.3.3/src/dw3d/tesselation_graph.py
--rw-r--r--   0 perez     (1000) perez     (1000)     7879 2024-03-11 14:07:22.000000 delaunay_watershed_3d-0.3.3/src/dw3d/viewing.py
--rw-r--r--   0 perez     (1000) perez     (1000)     3797 2024-03-25 10:44:46.000000 delaunay_watershed_3d-0.3.3/src/dw3d/watershed.py
+drwxr-xr-x   0 perez     (1000) perez     (1000)        0 2024-04-03 13:48:41.133749 delaunay_watershed_3d-0.3.4/
+-rw-r--r--   0 perez     (1000) perez     (1000)     8145 2024-04-03 13:48:41.133749 delaunay_watershed_3d-0.3.4/PKG-INFO
+-rw-r--r--   0 perez     (1000) perez     (1000)     7069 2024-03-12 15:12:15.000000 delaunay_watershed_3d-0.3.4/README.md
+-rw-r--r--   0 perez     (1000) perez     (1000)     1202 2024-02-13 09:09:41.000000 delaunay_watershed_3d-0.3.4/pyproject.toml
+-rw-r--r--   0 perez     (1000) perez     (1000)     1072 2024-04-03 13:48:41.133749 delaunay_watershed_3d-0.3.4/setup.cfg
+drwxr-xr-x   0 perez     (1000) perez     (1000)        0 2024-04-03 13:48:41.130415 delaunay_watershed_3d-0.3.4/src/
+drwxr-xr-x   0 perez     (1000) perez     (1000)        0 2024-04-03 13:48:41.133749 delaunay_watershed_3d-0.3.4/src/delaunay_watershed_3d.egg-info/
+-rw-r--r--   0 perez     (1000) perez     (1000)     8145 2024-04-03 13:48:41.000000 delaunay_watershed_3d-0.3.4/src/delaunay_watershed_3d.egg-info/PKG-INFO
+-rw-r--r--   0 perez     (1000) perez     (1000)      673 2024-04-03 13:48:41.000000 delaunay_watershed_3d-0.3.4/src/delaunay_watershed_3d.egg-info/SOURCES.txt
+-rw-r--r--   0 perez     (1000) perez     (1000)        1 2024-04-03 13:48:41.000000 delaunay_watershed_3d-0.3.4/src/delaunay_watershed_3d.egg-info/dependency_links.txt
+-rw-r--r--   0 perez     (1000) perez     (1000)      163 2024-04-03 13:48:41.000000 delaunay_watershed_3d-0.3.4/src/delaunay_watershed_3d.egg-info/requires.txt
+-rw-r--r--   0 perez     (1000) perez     (1000)        5 2024-04-03 13:48:41.000000 delaunay_watershed_3d-0.3.4/src/delaunay_watershed_3d.egg-info/top_level.txt
+drwxr-xr-x   0 perez     (1000) perez     (1000)        0 2024-04-03 13:48:41.133749 delaunay_watershed_3d-0.3.4/src/dw3d/
+-rw-r--r--   0 perez     (1000) perez     (1000)     2513 2024-03-12 15:11:52.000000 delaunay_watershed_3d-0.3.4/src/dw3d/__init__.py
+-rw-r--r--   0 perez     (1000) perez     (1000)     7400 2024-04-03 13:09:24.000000 delaunay_watershed_3d-0.3.4/src/dw3d/edt.py
+-rw-r--r--   0 perez     (1000) perez     (1000)     8708 2024-03-12 15:19:46.000000 delaunay_watershed_3d-0.3.4/src/dw3d/io.py
+-rw-r--r--   0 perez     (1000) perez     (1000)     4089 2024-03-11 16:02:21.000000 delaunay_watershed_3d-0.3.4/src/dw3d/mask_reconstruction.py
+-rw-r--r--   0 perez     (1000) perez     (1000)    12150 2024-03-27 14:21:14.000000 delaunay_watershed_3d-0.3.4/src/dw3d/mesh_surgery.py
+-rw-r--r--   0 perez     (1000) perez     (1000)     9302 2024-03-27 13:46:03.000000 delaunay_watershed_3d-0.3.4/src/dw3d/mesh_utilities.py
+-rw-r--r--   0 perez     (1000) perez     (1000)     4958 2024-04-03 13:37:02.000000 delaunay_watershed_3d-0.3.4/src/dw3d/points_on_edt.py
+-rw-r--r--   0 perez     (1000) perez     (1000)    11143 2024-04-03 13:00:16.000000 delaunay_watershed_3d-0.3.4/src/dw3d/reconstruction_algorithm.py
+-rw-r--r--   0 perez     (1000) perez     (1000)     7981 2024-04-03 13:22:43.000000 delaunay_watershed_3d-0.3.4/src/dw3d/reconstruction_algorithm_factory.py
+-rw-r--r--   0 perez     (1000) perez     (1000)     4161 2024-03-11 10:43:52.000000 delaunay_watershed_3d-0.3.4/src/dw3d/score_computation.py
+-rw-r--r--   0 perez     (1000) perez     (1000)     1835 2024-03-08 08:45:06.000000 delaunay_watershed_3d-0.3.4/src/dw3d/segmentation.py
+-rw-r--r--   0 perez     (1000) perez     (1000)      894 2024-03-11 14:41:02.000000 delaunay_watershed_3d-0.3.4/src/dw3d/tesselation.py
+-rw-r--r--   0 perez     (1000) perez     (1000)     9637 2024-03-27 10:37:08.000000 delaunay_watershed_3d-0.3.4/src/dw3d/tesselation_graph.py
+-rw-r--r--   0 perez     (1000) perez     (1000)     7919 2024-04-03 09:18:03.000000 delaunay_watershed_3d-0.3.4/src/dw3d/viewing.py
+-rw-r--r--   0 perez     (1000) perez     (1000)     3797 2024-03-25 10:44:46.000000 delaunay_watershed_3d-0.3.4/src/dw3d/watershed.py
```

### Comparing `delaunay_watershed_3d-0.3.3/PKG-INFO` & `delaunay_watershed_3d-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delaunay_watershed_3d
-Version: 0.3.3
+Version: 0.3.4
 Summary: Geometrical reconstruction of cell assemblies from instance segmentations
 Home-page: https://github.com/VirtualEmbryo/delaunay-watershed
 Author: Sacha Ichbiah
 Author-email: sacha.ichbiah@college-de-france.fr
 Maintainer: Matthieu Perez
 Maintainer-email: matthieu.perez@college-de-france.fr
 License: CC BY-NC-SA 4.0
```

### Comparing `delaunay_watershed_3d-0.3.3/README.md` & `delaunay_watershed_3d-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.3.3/pyproject.toml` & `delaunay_watershed_3d-0.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.3.3/setup.cfg` & `delaunay_watershed_3d-0.3.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = delaunay_watershed_3d
-version = 0.3.3
+version = 0.3.4
 author = Sacha Ichbiah
 author_email = sacha.ichbiah@college-de-france.fr
 maintainer = Matthieu Perez
 maintainer_email = matthieu.perez@college-de-france.fr
 description = Geometrical reconstruction of cell assemblies from instance segmentations
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `delaunay_watershed_3d-0.3.3/src/delaunay_watershed_3d.egg-info/PKG-INFO` & `delaunay_watershed_3d-0.3.4/src/delaunay_watershed_3d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delaunay_watershed_3d
-Version: 0.3.3
+Version: 0.3.4
 Summary: Geometrical reconstruction of cell assemblies from instance segmentations
 Home-page: https://github.com/VirtualEmbryo/delaunay-watershed
 Author: Sacha Ichbiah
 Author-email: sacha.ichbiah@college-de-france.fr
 Maintainer: Matthieu Perez
 Maintainer-email: matthieu.perez@college-de-france.fr
 License: CC BY-NC-SA 4.0
```

### Comparing `delaunay_watershed_3d-0.3.3/src/delaunay_watershed_3d.egg-info/SOURCES.txt` & `delaunay_watershed_3d-0.3.4/src/delaunay_watershed_3d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.3.3/src/dw3d/__init__.py` & `delaunay_watershed_3d-0.3.4/src/dw3d/__init__.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.3.3/src/dw3d/edt.py` & `delaunay_watershed_3d-0.3.4/src/dw3d/edt.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Compute Euclidean Distance Trasnform out of segmentation image.
 
 Sacha Ichbiah 2021
 Matthieu Perez 2024
 """
+
 from time import time
 
 import numpy as np
 from edt import edt as euclidean_dt
 from numpy.typing import NDArray
 from skimage.segmentation import find_boundaries
 
@@ -125,49 +126,69 @@
         ((pad_size, pad_size), (pad_size, pad_size), (pad_size, pad_size)),
         "constant",
         constant_values=1,
     )
     return padded_mask
 
 
-# Matthieu Perez : tests bias EDT
-# def compute_edt_with_bias(labels, prints=False):
-#     if prints:
-#         print("Computing EDT (bias) ...")
-#     t1 = time()
-
-#     region_indices = np.unique(labels)
-#     total_boundaries = np.zeros(labels.shape)
-
-#     for index in region_indices:
-#         if index == 0:
-#             region_labels = np.where(labels == 0, 1, 0)
-#         else:
-#             region_labels = np.where(labels == index, labels, 0)
-#         total_boundaries += StandardLabelToBoundary()(region_labels)[0]
-
-#     # total_boundaries *= 3
-#     total_boundaries = np.amax(total_boundaries) - total_boundaries
-
-#     # "thick" boundaries are marked by 1, 0 outside
-#     b = StandardLabelToBoundary()(labels)[0]
-#     mask_2 = b
-#     # EDT of the thick boundaries (0 elsewhere)
-#     EDT_2 = euclidean_dt(mask_2)
-#     b = pad_mask(b)  # exterior bbox is marked as 1
-#     mask_1 = 1 - b  # 1 everywhere except bbox and boundaries
-#     # main part of the final EDT. Both inside cells and outside cells. 0 in boundaries & bbox
-#     EDT_1 = euclidean_dt(mask_1)
-#     # max EDT2 everywhere except on thick boundaries where it decreases to 0 on the mid of boundaries
-#     # + total_boundaries which is less on interesting parts of the mesh
-#     inv = np.amax(EDT_2) - EDT_2 + total_boundaries
-#     # total EDT is valid also on thick boundaries
-#     Total_EDT = (EDT_1 + np.amax(inv)) * mask_1 + inv * mask_2
-
-#     # # Matthieu Perez try 2: augment constrast in EDT
-#     # Total_EDT = 255 * ((Total_EDT / 255) ** 0.5)
-
-#     t2 = time()
-#     if prints:
-#         print("EDT computed in ", np.round(t2 - t1, 2))
+# Matthieu Perez : tests bias EDT towards boundaries between interfaces
+def compute_edt_boundary_bias(segmentation_mask: NDArray[np.uint], print_info: bool = False) -> NDArray[np.float64]:
+    """Compute a biased version of the Euclidean Distance Transform of a segmented image.
+
+    It is biased towards the boundaries between interfaces.
+    """
+    if print_info:
+        print("Computing EDT (bias) ...")
+    t1 = time()
+
+    region_indices = np.unique(segmentation_mask)
+    total_boundaries = np.zeros(segmentation_mask.shape)
+
+    for index in region_indices:
+        if index == 0:
+            region_labels = np.where(segmentation_mask == 0, 1, 0)
+        else:
+            region_labels = np.where(segmentation_mask == index, segmentation_mask, 0)
+        total_boundaries += _StandardLabelToBoundary()(region_labels)[0]
+
+    # total_boundaries *= 3
+    total_boundaries = np.amax(total_boundaries) - total_boundaries
+
+    # "thick" boundaries are marked by 1, 0 outside
+    b = _StandardLabelToBoundary()(segmentation_mask)[0]
+    mask_2 = b
+    # EDT of the thick boundaries (0 elsewhere)
+    edt_2 = euclidean_dt(mask_2)
+    b = _pad_mask(b)  # exterior bbox is marked as 1
+    mask_1 = 1 - b  # 1 everywhere except bbox and boundaries
+    # main part of the final EDT. Both inside cells and outside cells. 0 in boundaries & bbox
+    edt_1 = euclidean_dt(mask_1)
+    # max EDT2 everywhere except on thick boundaries where it decreases to 0 on the mid of boundaries
+    # + total_boundaries which is less on interesting parts of the mesh
+    inv = np.amax(edt_2) - edt_2 + total_boundaries
+    # total EDT is valid also on thick boundaries
+    total_edt = (edt_1 + np.amax(inv)) * mask_1 + inv * mask_2
+
+    # Matthieu Perez try 2: augment constrast in EDT
+    # Total_EDT = 255 * ((Total_EDT / 255) ** 0.5)
+
+    t2 = time()
+    if print_info:
+        print("EDT computed in ", np.round(t2 - t1, 2))
+
+    return total_edt
+
+
+def get_total_boundaries(segmented_mask: NDArray[np.uint]) -> NDArray[np.float64]:
+    """Obtain pre-EDT on boundaries from segmentation mask."""
+    region_indices = np.unique(segmented_mask)
+    total_boundaries = np.zeros(segmented_mask.shape)
+
+    for index in region_indices:
+        if index == 0:
+            region_labels = np.where(segmented_mask == 0, 1, 0)
+        else:
+            region_labels = np.where(segmented_mask == index, segmented_mask, 0)
+        total_boundaries += _StandardLabelToBoundary()(region_labels)[0]
 
-#     return Total_EDT
+    total_boundaries = np.amax(total_boundaries) - total_boundaries
+    return total_boundaries
```

### Comparing `delaunay_watershed_3d-0.3.3/src/dw3d/io.py` & `delaunay_watershed_3d-0.3.4/src/dw3d/io.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.3.3/src/dw3d/mask_reconstruction.py` & `delaunay_watershed_3d-0.3.4/src/dw3d/mask_reconstruction.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.3.3/src/dw3d/mesh_utilities.py` & `delaunay_watershed_3d-0.3.4/src/dw3d/mesh_utilities.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.3.3/src/dw3d/reconstruction_algorithm.py` & `delaunay_watershed_3d-0.3.4/src/dw3d/reconstruction_algorithm.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 )
 from dw3d.segmentation import extract_seed_coords_and_indices
 from dw3d.tesselation_graph import TesselationGraph
 from dw3d.watershed import seeded_watershed_map
 
 # segmentation mask -> EDT image
 EdtCreationFunction = Callable[[NDArray[np.uint]], NDArray[np.float64]]
-# EDT image -> array of pixel coordinates
-PointPlacingFunction = Callable[[NDArray[np.float64]], NDArray[np.uint]]
+# optional segmentation mask + EDT image -> array of pixel coordinates
+PointPlacingFunction = Callable[[NDArray[np.uint] | None, NDArray[np.float64]], NDArray[np.uint]]
 # array of pixel coordinates -> tesselation: array of points coordinates + array of tetrahedrons as points indices
 TesselationCreationFunction = Callable[[NDArray[np.uint]], tuple[NDArray[np.float64], NDArray[np.int64]]]
 # EDT image, array of points + triangle faces (from tesselation) -> Array of scores
 ScoreComputationFunction = Callable[[NDArray[np.float64], NDArray[np.float64], NDArray[np.int64]], NDArray[np.float64]]
 # Watershed : one version only
 # Mesh recreation : one version only
 # Mesh surgery : one bool to perform surgery ?
@@ -84,15 +84,15 @@
                - mesh triangles (topology)
                - labels (materials) on each side of the triangles. 0 is exterior.
         """
         self._segmented_image = segmented_image
 
         self._edt_image = self.edt_creation_function(self._segmented_image)
 
-        points_for_tesselation = self.point_placing_function(self._edt_image)
+        points_for_tesselation = self.point_placing_function(self._segmented_image, self._edt_image)
 
         t_init_tesselation = perf_counter()
         tesselation_points, tesselation_tetrahedrons = self.tesselation_creation_function(points_for_tesselation)
         if self.print_info:
             print(f"Delaunay Tesselation built in {perf_counter() - t_init_tesselation:.2} seconds")
 
         self._tesselation_graph = TesselationGraph(
@@ -139,19 +139,20 @@
             self._seeds_indices,
             zero_nodes,
         )
 
         if self.print_info:
             print(f"Watershed done in {perf_counter() - t1:.3} seconds.")
 
-    def _mesh_surgery(self, max_iter: int = 3) -> None:
+    def _mesh_surgery(self) -> None:
         """Try to detect and fix mesh problems while we have all the Watershed data."""
+        # return
         # Optional part
         if self.perform_mesh_postprocess_surgery:
-            post_process_mesh_surgery(self, max_iter)
+            post_process_mesh_surgery(self)
 
         # Always do this part
         # filter unused points
         self._points, self._triangles = filter_unused_points(self._points, self._triangles)
 
     @property
     def last_constructed_mesh(self) -> tuple[NDArray[np.float64], NDArray[np.uint], NDArray[np.uint]]:
```

### Comparing `delaunay_watershed_3d-0.3.3/src/dw3d/reconstruction_algorithm_factory.py` & `delaunay_watershed_3d-0.3.4/src/dw3d/reconstruction_algorithm_factory.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 Matthieu Perez 2024
 """
 
 from functools import partial
 from typing import Self
 
-from dw3d.edt import compute_edt_classical
-from dw3d.points_on_edt import peak_local_points
+from dw3d.edt import compute_edt_boundary_bias, compute_edt_classical
+from dw3d.points_on_edt import peak_local_points, peak_local_points_bias_boundaries
 from dw3d.reconstruction_algorithm import (
     EdtCreationFunction,
     MeshReconstructionAlgorithm,
     PointPlacingFunction,
     ScoreComputationFunction,
     TesselationCreationFunction,
 )
@@ -34,23 +34,37 @@
         self.perform_mesh_postprocess_surgery = perform_mesh_postprocess_surgery
 
     def set_classical_edt_method(self) -> Self:
         """Use the classical method to create the Euclidean Distance Transform from a segmentation mask."""
         self._edt_creation_function = _edt_creation_function_classical(self.print_info)
         return self
 
-    def set_peak_local_points_placement_method(self, min_distance: int = 5) -> Self:
+    def set_edt_boundary_bias_method(self) -> Self:
+        """Use the biased method to create the Euclidean Distance Transform from a segmentation mask."""
+        self._edt_creation_function = _edt_creation_function_boundary_bias(self.print_info)
+        return self
+
+    def set_peak_local_points_placement_method(self, min_distance: int = 3) -> Self:
         """Place points on the EDT image using local extrema of the EDT (and corners).
 
         Args:
-            min_distance (int, optional): Minimum distance between extrema. Defaults to 5.
+            min_distance (int, optional): Minimum distance between extrema. Defaults to 3.
         """
         self._point_placing_function = _point_placing_function_peak_local(min_distance, self.print_info)
         return self
 
+    def set_peak_local_points_bias_boundary_placement_method(self, min_distance: int = 3) -> Self:
+        """Place points on the EDT image using local extrema of the EDT (and corners) and boundaries.
+
+        Args:
+            min_distance (int, optional): Minimum distance between extrema. Defaults to 3.
+        """
+        self._point_placing_function = _point_placing_function_peak_local_bias_boundaries(min_distance, self.print_info)
+        return self
+
     def set_delaunay_tesselation_method(self) -> Self:
         """Use Delaunay algorithm to create the tesselation from a list of points."""
         self._tesselation_creation_function = simple_delaunay_tesselation
         return self
 
     def set_score_computation_by_mean_value(self) -> Self:
         """Use the mean value of the EDT image on triangle faces of the tesselation to compute scores for Watershed."""
@@ -74,15 +88,15 @@
             point_placing_function=self._point_placing_function,
             tesselation_creation_function=self._tesselation_creation_function,
             score_computation_function=self._score_computation_function,
             perform_mesh_postprocess_surgery=self.perform_mesh_postprocess_surgery,
         )
 
     @staticmethod
-    def get_default_algorithm(min_distance: int = 5, print_info: bool = False) -> MeshReconstructionAlgorithm:
+    def get_default_algorithm(min_distance: int = 3, print_info: bool = False) -> MeshReconstructionAlgorithm:
         """Return the default mesh reconstruction algorithm with sensible default values.
 
         Args:
             min_distance (int, optional): Minimum distance (in pixels) between extrema when placing
                 tesselation points. Defaults to 5.
             print_info (bool, optional): Print algorithm details while executing.
         """
@@ -107,23 +121,56 @@
     Returns:
         EdtCreationFunction:
             - the actual function which takes a segmentation mask and return an Euclidean Distance Transform image.
     """
     return partial(compute_edt_classical, print_info=print_info)
 
 
+def _edt_creation_function_boundary_bias(
+    print_info: bool = False,
+) -> EdtCreationFunction:
+    """Get a function that compute an EDT from a segmentation mask.
+
+    Args:
+        print_info (bool, optional): Print detals about the algorithm. Defaults to False.
+
+    Returns:
+        EdtCreationFunction:
+            - the actual function which takes a segmentation mask and return an Euclidean Distance Transform image.
+    """
+    return partial(compute_edt_boundary_bias, print_info=print_info)
+
+
 def _point_placing_function_peak_local(
-    min_distance: int = 5,
+    min_distance: int = 3,
     print_info: bool = False,
 ) -> PointPlacingFunction:
     """Get a function that peaks local min and max points (+ corner points) from an EDT image.
 
     Args:
-        min_distance (int, optional): Minimum distance between extrema. Defaults to 5.
+        min_distance (int, optional): Minimum distance between extrema. Defaults to 3.
         print_info (bool, optional): Print detals about the algorithm. Defaults to False.
 
     Returns:
         Callable[[NDArray[np.float64]], NDArray[np.uint]]:
             - the actual function which takes only an EDT image and return an array of 3D pixel coordinates
               of local min & max of the EDT (+ corners)
     """
     return partial(peak_local_points, min_distance=min_distance, print_info=print_info)
+
+
+def _point_placing_function_peak_local_bias_boundaries(
+    min_distance: int = 3,
+    print_info: bool = False,
+) -> PointPlacingFunction:
+    """Get a function that peaks local min and max points (+ corner points) from an EDT image.
+
+    Args:
+        min_distance (int, optional): Minimum distance between extrema. Defaults to 3.
+        print_info (bool, optional): Print detals about the algorithm. Defaults to False.
+
+    Returns:
+        Callable[[NDArray[np.float64]], NDArray[np.uint]]:
+            - the actual function which takes only an EDT image and return an array of 3D pixel coordinates
+              of local min & max of the EDT (+ corners)
+    """
+    return partial(peak_local_points_bias_boundaries, min_distance=min_distance, print_info=print_info)
```

### Comparing `delaunay_watershed_3d-0.3.3/src/dw3d/score_computation.py` & `delaunay_watershed_3d-0.3.4/src/dw3d/score_computation.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.3.3/src/dw3d/segmentation.py` & `delaunay_watershed_3d-0.3.4/src/dw3d/segmentation.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.3.3/src/dw3d/tesselation.py` & `delaunay_watershed_3d-0.3.4/src/dw3d/tesselation.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.3.3/src/dw3d/tesselation_graph.py` & `delaunay_watershed_3d-0.3.4/src/dw3d/tesselation_graph.py`

 * *Files 6% similar despite different names*

```diff
@@ -140,33 +140,43 @@
                 ),
             )[0],
         )
 
         # Now let's find a cycle
         ordered_tetrahedrons = [adjacent_tetrahedrons[0]]
         del adjacent_tetrahedrons[0]
+        ordered_triangles = []  # transition between each tetra
 
         # We find a cycle by finding tetrahedrons sharing a triangle face
         nb_tetra = len(adjacent_tetrahedrons)
         selected_id = 0
         for _ in range(nb_tetra):
             last_tetra_in_cycle = ordered_tetrahedrons[-1]
             last_triangles = set(self.faces_of_nodes[last_tetra_in_cycle])
 
             to_remove = -1
             for i, tet_id in enumerate(adjacent_tetrahedrons):
                 selected_id = tet_id
                 tet_triangles = self.faces_of_nodes[tet_id]
-                if len(last_triangles.intersection(tet_triangles)) > 0:
+                common_triangles = last_triangles.intersection(tet_triangles)  # normally 0 or 1
+                if len(common_triangles) > 0:
+                    ordered_triangles.append(next(iter(common_triangles)))  # first triangle in intersection (only one)
                     to_remove = i
                     break
 
             ordered_tetrahedrons.append(selected_id)
             del adjacent_tetrahedrons[to_remove]
 
+        # tetrahedrons are sorted
+        first_triangles = self.faces_of_nodes[ordered_tetrahedrons[0]]
+        last_triangles = set(self.faces_of_nodes[ordered_tetrahedrons[-1]])
+        common_triangles = last_triangles.intersection(first_triangles)  # normally 0 or 1
+        if len(common_triangles) > 0:
+            ordered_triangles.append(next(iter(common_triangles)))  # first triangle in intersection (only one)
+
         return ordered_tetrahedrons
 
     def to_networkx_graph(self) -> networkx.Graph:
         """Compute a NetworkX graph with nodes = tetrahedrons, edges = triangle faces and data associated.
 
         Data on nodes = volumes, Data on edges = scores and area.
         """
```

### Comparing `delaunay_watershed_3d-0.3.3/src/dw3d/viewing.py` & `delaunay_watershed_3d-0.3.4/src/dw3d/viewing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """This module gathers all optional viewing utilities for debugging.
 
 Install them with the [viewing] option.
 
 Matthieu Perez, 2024.
 """
+
 from typing import TYPE_CHECKING
 
 from numpy.typing import NDArray
 
 if TYPE_CHECKING:
     import napari
 
@@ -34,20 +35,21 @@
     v = napari.view_image(reconstruct._segmented_image, name="Labels")
     v.add_image(reconstruct._edt_image, name="Distance Transform")
     if original_image is not None:
         v.add_image(original_image, name="Original Image")
     if not add_mesh:
         rng = np.random.default_rng()
         v.add_points(
-            reconstruct._seeds_coords,
+            reconstruct._seeds_coords.astype(np.float64),
             name="Watershed seeds",
             n_dimensional=True,
             face_color=rng.random((len(reconstruct._seeds_coords), 3)),
             size=10,
         )
+
     v.add_points(
         reconstruct._tesselation_graph.vertices,
         name="triangulation_points",
         n_dimensional=False,
         face_color="red",
         size=1,
     )
@@ -90,15 +92,15 @@
             offset += len(vn)
         all_verts.append(np.array([np.mean(np.vstack(all_verts), axis=0)]))
         all_labels.append(np.array([0]))
         all_verts = np.vstack(all_verts)
         all_faces = np.vstack(all_faces)
         all_labels = np.hstack(all_labels)
         v.add_points(
-            reconstruct._seeds_coords,
+            reconstruct._seeds_coords.astype(np.float64),
             name="Watershed seeds",
             n_dimensional=True,
             face_color=np.array(plt.cm.viridis(np.array(sorted(clusters.keys())) / maxkey))[:, :3],
             size=10,
         )
 
         v.add_surface((all_verts, all_faces, all_labels), colormap="viridis")
```

### Comparing `delaunay_watershed_3d-0.3.3/src/dw3d/watershed.py` & `delaunay_watershed_3d-0.3.4/src/dw3d/watershed.py`

 * *Files identical despite different names*

