# Comparing `tmp/DeepTile-2.0.6.tar.gz` & `tmp/DeepTile-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DeepTile-2.0.6.tar", last modified: Fri Jan 26 07:04:07 2024, max compression
+gzip compressed data, was "DeepTile-2.0.7.tar", last modified: Wed Apr  3 19:36:09 2024, max compression
```

## Comparing `DeepTile-2.0.6.tar` & `DeepTile-2.0.7.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 wniu      (1003) wniu      (1003)        0 2024-01-26 07:04:07.572807 DeepTile-2.0.6/
-drwxrwxr-x   0 wniu      (1003) wniu      (1003)        0 2024-01-26 07:04:07.572807 DeepTile-2.0.6/DeepTile.egg-info/
--rw-r--r--   0 wniu      (1003) wniu      (1003)     1246 2024-01-26 07:04:07.000000 DeepTile-2.0.6/DeepTile.egg-info/PKG-INFO
--rw-rw-r--   0 wniu      (1003) wniu      (1003)      787 2024-01-26 07:04:07.000000 DeepTile-2.0.6/DeepTile.egg-info/SOURCES.txt
--rw-rw-r--   0 wniu      (1003) wniu      (1003)        1 2024-01-26 07:04:07.000000 DeepTile-2.0.6/DeepTile.egg-info/dependency_links.txt
--rw-rw-r--   0 wniu      (1003) wniu      (1003)       37 2024-01-26 07:04:07.000000 DeepTile-2.0.6/DeepTile.egg-info/requires.txt
--rw-rw-r--   0 wniu      (1003) wniu      (1003)        9 2024-01-26 07:04:07.000000 DeepTile-2.0.6/DeepTile.egg-info/top_level.txt
--rw-rw-r--   0 wniu      (1003) wniu      (1003)     1068 2023-12-24 17:39:11.000000 DeepTile-2.0.6/LICENSE
--rw-r--r--   0 wniu      (1003) wniu      (1003)     1246 2024-01-26 07:04:07.572807 DeepTile-2.0.6/PKG-INFO
--rw-rw-r--   0 wniu      (1003) wniu      (1003)      664 2023-12-24 17:39:11.000000 DeepTile-2.0.6/README.md
-drwxrwxr-x   0 wniu      (1003) wniu      (1003)        0 2024-01-26 07:04:07.572807 DeepTile-2.0.6/deeptile/
--rw-rw-r--   0 wniu      (1003) wniu      (1003)      103 2023-12-24 17:39:12.000000 DeepTile-2.0.6/deeptile/__init__.py
-drwxrwxr-x   0 wniu      (1003) wniu      (1003)        0 2024-01-26 07:04:07.572807 DeepTile-2.0.6/deeptile/core/
--rw-rw-r--   0 wniu      (1003) wniu      (1003)        0 2023-12-24 17:39:12.000000 DeepTile-2.0.6/deeptile/core/__init__.py
--rw-rw-r--   0 wniu      (1003) wniu      (1003)    25933 2024-01-26 07:00:45.000000 DeepTile-2.0.6/deeptile/core/data.py
--rw-rw-r--   0 wniu      (1003) wniu      (1003)     3111 2024-01-26 07:00:45.000000 DeepTile-2.0.6/deeptile/core/iterators.py
--rw-rw-r--   0 wniu      (1003) wniu      (1003)      890 2024-01-26 06:35:52.000000 DeepTile-2.0.6/deeptile/core/jobs.py
--rw-rw-r--   0 wniu      (1003) wniu      (1003)     7783 2024-01-26 06:35:52.000000 DeepTile-2.0.6/deeptile/core/lift.py
--rw-rw-r--   0 wniu      (1003) wniu      (1003)    12405 2024-01-26 06:35:52.000000 DeepTile-2.0.6/deeptile/core/process.py
--rw-rw-r--   0 wniu      (1003) wniu      (1003)     1586 2024-01-26 06:35:52.000000 DeepTile-2.0.6/deeptile/core/profiles.py
--rw-rw-r--   0 wniu      (1003) wniu      (1003)     4868 2024-01-26 06:51:20.000000 DeepTile-2.0.6/deeptile/core/trees.py
--rw-rw-r--   0 wniu      (1003) wniu      (1003)     4375 2023-12-24 17:39:12.000000 DeepTile-2.0.6/deeptile/core/utils.py
--rw-rw-r--   0 wniu      (1003) wniu      (1003)     6770 2024-01-26 07:00:45.000000 DeepTile-2.0.6/deeptile/deeptile.py
-drwxrwxr-x   0 wniu      (1003) wniu      (1003)        0 2024-01-26 07:04:07.572807 DeepTile-2.0.6/deeptile/extensions/
--rw-rw-r--   0 wniu      (1003) wniu      (1003)       53 2023-12-24 17:39:12.000000 DeepTile-2.0.6/deeptile/extensions/__init__.py
--rw-rw-r--   0 wniu      (1003) wniu      (1003)     6204 2024-01-26 07:00:45.000000 DeepTile-2.0.6/deeptile/extensions/segmentation.py
--rw-rw-r--   0 wniu      (1003) wniu      (1003)    14031 2024-01-26 07:00:45.000000 DeepTile-2.0.6/deeptile/extensions/stitch.py
--rw-rw-r--   0 wniu      (1003) wniu      (1003)     3076 2024-01-26 07:00:45.000000 DeepTile-2.0.6/deeptile/io.py
-drwxrwxr-x   0 wniu      (1003) wniu      (1003)        0 2024-01-26 07:04:07.572807 DeepTile-2.0.6/deeptile/sources/
--rw-rw-r--   0 wniu      (1003) wniu      (1003)        0 2023-12-24 17:39:12.000000 DeepTile-2.0.6/deeptile/sources/__init__.py
--rw-rw-r--   0 wniu      (1003) wniu      (1003)      156 2023-12-24 17:39:12.000000 DeepTile-2.0.6/deeptile/sources/array.py
--rw-rw-r--   0 wniu      (1003) wniu      (1003)      894 2023-12-24 17:39:12.000000 DeepTile-2.0.6/deeptile/sources/function.py
--rw-rw-r--   0 wniu      (1003) wniu      (1003)     2135 2023-12-24 17:39:12.000000 DeepTile-2.0.6/deeptile/sources/large_image.py
--rw-rw-r--   0 wniu      (1003) wniu      (1003)     3742 2023-12-24 17:39:12.000000 DeepTile-2.0.6/deeptile/sources/nd2.py
--rw-rw-r--   0 wniu      (1003) wniu      (1003)      353 2023-12-24 17:39:12.000000 DeepTile-2.0.6/deeptile/sources/tiff.py
--rw-rw-r--   0 wniu      (1003) wniu      (1003)      752 2024-01-26 06:35:52.000000 DeepTile-2.0.6/pyproject.toml
--rw-rw-r--   0 wniu      (1003) wniu      (1003)       38 2024-01-26 07:04:07.572807 DeepTile-2.0.6/setup.cfg
-drwxrwxr-x   0 wniu      (1003) wniu      (1003)        0 2024-01-26 07:04:07.572807 DeepTile-2.0.6/tests/
--rw-rw-r--   0 wniu      (1003) wniu      (1003)      217 2023-12-24 17:39:12.000000 DeepTile-2.0.6/tests/test_imports.py
--rw-rw-r--   0 wniu      (1003) wniu      (1003)     3449 2023-12-24 17:39:12.000000 DeepTile-2.0.6/tests/test_io.py
--rw-rw-r--   0 wniu      (1003) wniu      (1003)     1668 2023-12-24 17:39:12.000000 DeepTile-2.0.6/tests/test_stitch.py
+drwxrwxr-x   0 wniu      (1003) wniu      (1003)        0 2024-04-03 19:36:09.537206 DeepTile-2.0.7/
+drwxrwxr-x   0 wniu      (1003) wniu      (1003)        0 2024-04-03 19:36:09.537206 DeepTile-2.0.7/DeepTile.egg-info/
+-rw-r--r--   0 wniu      (1003) wniu      (1003)     1218 2024-04-03 19:36:09.000000 DeepTile-2.0.7/DeepTile.egg-info/PKG-INFO
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)      787 2024-04-03 19:36:09.000000 DeepTile-2.0.7/DeepTile.egg-info/SOURCES.txt
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)        1 2024-04-03 19:36:09.000000 DeepTile-2.0.7/DeepTile.egg-info/dependency_links.txt
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)       24 2024-04-03 19:36:09.000000 DeepTile-2.0.7/DeepTile.egg-info/requires.txt
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)        9 2024-04-03 19:36:09.000000 DeepTile-2.0.7/DeepTile.egg-info/top_level.txt
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)     1068 2023-12-24 17:39:11.000000 DeepTile-2.0.7/LICENSE
+-rw-r--r--   0 wniu      (1003) wniu      (1003)     1218 2024-04-03 19:36:09.537206 DeepTile-2.0.7/PKG-INFO
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)      664 2023-12-24 17:39:11.000000 DeepTile-2.0.7/README.md
+drwxrwxr-x   0 wniu      (1003) wniu      (1003)        0 2024-04-03 19:36:09.533206 DeepTile-2.0.7/deeptile/
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)      103 2023-12-24 17:39:12.000000 DeepTile-2.0.7/deeptile/__init__.py
+drwxrwxr-x   0 wniu      (1003) wniu      (1003)        0 2024-04-03 19:36:09.533206 DeepTile-2.0.7/deeptile/core/
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)        0 2023-12-24 17:39:12.000000 DeepTile-2.0.7/deeptile/core/__init__.py
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)    25933 2024-01-26 07:00:45.000000 DeepTile-2.0.7/deeptile/core/data.py
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)     3111 2024-01-26 07:00:45.000000 DeepTile-2.0.7/deeptile/core/iterators.py
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)      890 2024-01-26 06:35:52.000000 DeepTile-2.0.7/deeptile/core/jobs.py
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)     7783 2024-01-26 06:35:52.000000 DeepTile-2.0.7/deeptile/core/lift.py
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)    12405 2024-01-26 06:35:52.000000 DeepTile-2.0.7/deeptile/core/process.py
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)     1586 2024-01-26 06:35:52.000000 DeepTile-2.0.7/deeptile/core/profiles.py
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)     4868 2024-01-26 06:51:20.000000 DeepTile-2.0.7/deeptile/core/trees.py
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)     4375 2023-12-24 17:39:12.000000 DeepTile-2.0.7/deeptile/core/utils.py
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)     6770 2024-01-26 07:00:45.000000 DeepTile-2.0.7/deeptile/deeptile.py
+drwxrwxr-x   0 wniu      (1003) wniu      (1003)        0 2024-04-03 19:36:09.533206 DeepTile-2.0.7/deeptile/extensions/
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)       53 2023-12-24 17:39:12.000000 DeepTile-2.0.7/deeptile/extensions/__init__.py
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)     6209 2024-04-03 19:17:53.000000 DeepTile-2.0.7/deeptile/extensions/segmentation.py
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)    14045 2024-04-03 19:22:25.000000 DeepTile-2.0.7/deeptile/extensions/stitch.py
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)     3076 2024-01-26 07:00:45.000000 DeepTile-2.0.7/deeptile/io.py
+drwxrwxr-x   0 wniu      (1003) wniu      (1003)        0 2024-04-03 19:36:09.533206 DeepTile-2.0.7/deeptile/sources/
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)        0 2023-12-24 17:39:12.000000 DeepTile-2.0.7/deeptile/sources/__init__.py
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)      156 2023-12-24 17:39:12.000000 DeepTile-2.0.7/deeptile/sources/array.py
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)      894 2023-12-24 17:39:12.000000 DeepTile-2.0.7/deeptile/sources/function.py
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)     2135 2023-12-24 17:39:12.000000 DeepTile-2.0.7/deeptile/sources/large_image.py
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)     3742 2023-12-24 17:39:12.000000 DeepTile-2.0.7/deeptile/sources/nd2.py
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)      353 2023-12-24 17:39:12.000000 DeepTile-2.0.7/deeptile/sources/tiff.py
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)      732 2024-04-03 19:22:25.000000 DeepTile-2.0.7/pyproject.toml
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)       38 2024-04-03 19:36:09.537206 DeepTile-2.0.7/setup.cfg
+drwxrwxr-x   0 wniu      (1003) wniu      (1003)        0 2024-04-03 19:36:09.533206 DeepTile-2.0.7/tests/
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)      217 2023-12-24 17:39:12.000000 DeepTile-2.0.7/tests/test_imports.py
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)     3449 2023-12-24 17:39:12.000000 DeepTile-2.0.7/tests/test_io.py
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)     1668 2023-12-24 17:39:12.000000 DeepTile-2.0.7/tests/test_stitch.py
```

### Comparing `DeepTile-2.0.6/DeepTile.egg-info/PKG-INFO` & `DeepTile-2.0.7/DeepTile.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: DeepTile
-Version: 2.0.6
+Version: 2.0.7
 Summary: Large image tiling and stitching library for scaling Python functions to arbitrary input image sizes.
 Author: William Niu
 Author-email: wniu721@gmail.com
 Keywords: machine learning,deep learning,image tiling,image stitching
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: dask
 Requires-Dist: nd2
 Requires-Dist: numpy
-Requires-Dist: scikit-image
 Requires-Dist: tifffile
 
 # DeepTile
 Large image tiling and stitching library for scaling Python functions to arbitrary input image sizes.
 
 ## General
 DeepTile provides a standardized workflow for splitting large images into tiles of a specified size, processing tiles using regular Python functions, and stitching the processed tiles. DeepTile supports batch processing specifically designed for deep learning algorithms, featuring automatic padding and mini-batch generation.
```

### Comparing `DeepTile-2.0.6/DeepTile.egg-info/SOURCES.txt` & `DeepTile-2.0.7/DeepTile.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DeepTile-2.0.6/LICENSE` & `DeepTile-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `DeepTile-2.0.6/PKG-INFO` & `DeepTile-2.0.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: DeepTile
-Version: 2.0.6
+Version: 2.0.7
 Summary: Large image tiling and stitching library for scaling Python functions to arbitrary input image sizes.
 Author: William Niu
 Author-email: wniu721@gmail.com
 Keywords: machine learning,deep learning,image tiling,image stitching
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: dask
 Requires-Dist: nd2
 Requires-Dist: numpy
-Requires-Dist: scikit-image
 Requires-Dist: tifffile
 
 # DeepTile
 Large image tiling and stitching library for scaling Python functions to arbitrary input image sizes.
 
 ## General
 DeepTile provides a standardized workflow for splitting large images into tiles of a specified size, processing tiles using regular Python functions, and stitching the processed tiles. DeepTile supports batch processing specifically designed for deep learning algorithms, featuring automatic padding and mini-batch generation.
```

### Comparing `DeepTile-2.0.6/README.md` & `DeepTile-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `DeepTile-2.0.6/deeptile/core/data.py` & `DeepTile-2.0.7/deeptile/core/data.py`

 * *Files identical despite different names*

### Comparing `DeepTile-2.0.6/deeptile/core/iterators.py` & `DeepTile-2.0.7/deeptile/core/iterators.py`

 * *Files identical despite different names*

### Comparing `DeepTile-2.0.6/deeptile/core/jobs.py` & `DeepTile-2.0.7/deeptile/core/jobs.py`

 * *Files identical despite different names*

### Comparing `DeepTile-2.0.6/deeptile/core/lift.py` & `DeepTile-2.0.7/deeptile/core/lift.py`

 * *Files identical despite different names*

### Comparing `DeepTile-2.0.6/deeptile/core/process.py` & `DeepTile-2.0.7/deeptile/core/process.py`

 * *Files identical despite different names*

### Comparing `DeepTile-2.0.6/deeptile/core/profiles.py` & `DeepTile-2.0.7/deeptile/core/profiles.py`

 * *Files identical despite different names*

### Comparing `DeepTile-2.0.6/deeptile/core/trees.py` & `DeepTile-2.0.7/deeptile/core/trees.py`

 * *Files identical despite different names*

### Comparing `DeepTile-2.0.6/deeptile/core/utils.py` & `DeepTile-2.0.7/deeptile/core/utils.py`

 * *Files identical despite different names*

### Comparing `DeepTile-2.0.6/deeptile/deeptile.py` & `DeepTile-2.0.7/deeptile/deeptile.py`

 * *Files identical despite different names*

### Comparing `DeepTile-2.0.6/deeptile/extensions/segmentation.py` & `DeepTile-2.0.7/deeptile/extensions/segmentation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import numpy as np
 from deeptile.core.data import Output
 from deeptile.core.lift import lift
 from deeptile.core.utils import compute_dask
 from functools import partial
-from rasterio import features
 
 
 def cellpose_segmentation(model_parameters, eval_parameters, output_format='masks'):
 
     """Generate lifted function for the Cellpose segmentation algorithm.
 
     Parameters
@@ -149,14 +148,16 @@
         return masks
 
     return func_segment
 
 
 def mask_to_polygons(mask, index, tile_index, stitch_index, tiling):
 
+    from rasterio import features
+
     i_tile, j_tile = tile_index
     _, _, i_stitch, j_stitch = stitch_index
 
     offset = np.array((j_tile[0], i_tile[0]))
 
     valid = np.unique(mask[i_stitch[0]:i_stitch[1], j_stitch[0]:j_stitch[1]])
     valid = set(valid[valid > 0])
```

### Comparing `DeepTile-2.0.6/deeptile/extensions/stitch.py` & `DeepTile-2.0.7/deeptile/extensions/stitch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 import numpy as np
 from deeptile.core.data import Stitched
 from deeptile.core.jobs import Job
-from rtree import index
-from shapely.geometry import Polygon
-from skimage import measure
 
 
 def stitch_image(tiles, blend=True, sigma=10):
 
     """Stitch tiled images into a large image.
 
     Parameters
@@ -118,14 +115,16 @@
     stitched_polygons = Stitched(stitched_polygons, job)
 
     return stitched_polygons
 
 
 def stitch_masks(masks, iou_threshold=0.1):
 
+    from skimage import measure
+
     """Stitch tiled masks into a large mask.
 
     Parameters
     ----------
     masks : Tiled
         Array of tiled masks.
     iou_threshold : float, optional, default 0.1
@@ -299,14 +298,17 @@
     taper = tapery[:, None] * taperx
 
     return taper
 
 
 def _overlapping_polygons_rtree(polygons1, polygons2, iou_threshold=0.1):
 
+    from rtree import index
+    from shapely.geometry import Polygon
+
     # Initialize an empty R-tree index
     idx = index.Index()
 
     # Populate R-tree index with each polygon's bounding box in polygons1
     for pos, poly in enumerate(polygons1):
         poly = Polygon(poly)
         idx.insert(pos, poly.bounds)
```

### Comparing `DeepTile-2.0.6/deeptile/io.py` & `DeepTile-2.0.7/deeptile/io.py`

 * *Files identical despite different names*

### Comparing `DeepTile-2.0.6/deeptile/sources/function.py` & `DeepTile-2.0.7/deeptile/sources/function.py`

 * *Files identical despite different names*

### Comparing `DeepTile-2.0.6/deeptile/sources/large_image.py` & `DeepTile-2.0.7/deeptile/sources/large_image.py`

 * *Files identical despite different names*

### Comparing `DeepTile-2.0.6/deeptile/sources/nd2.py` & `DeepTile-2.0.7/deeptile/sources/nd2.py`

 * *Files identical despite different names*

### Comparing `DeepTile-2.0.6/pyproject.toml` & `DeepTile-2.0.7/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "DeepTile"
-version = "2.0.6"
+version = "2.0.7"
 description = "Large image tiling and stitching library for scaling Python functions to arbitrary input image sizes."
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [
     {email = "wniu721@gmail.com"},
     {name = "William Niu"}
 ]
@@ -17,13 +17,12 @@
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python"
 ]
 dependencies = [
     "dask",
     "nd2",
     "numpy",
-    "scikit-image",
     "tifffile"
 ]
 
 [tool.setuptools]
 packages = ["deeptile", "deeptile.core", "deeptile.extensions", "deeptile.sources"]
```

### Comparing `DeepTile-2.0.6/tests/test_io.py` & `DeepTile-2.0.7/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `DeepTile-2.0.6/tests/test_stitch.py` & `DeepTile-2.0.7/tests/test_stitch.py`

 * *Files identical despite different names*

