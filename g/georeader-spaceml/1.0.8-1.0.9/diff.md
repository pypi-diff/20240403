# Comparing `tmp/georeader-spaceml-1.0.8.tar.gz` & `tmp/georeader-spaceml-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "georeader-spaceml-1.0.8.tar", last modified: Mon Dec  4 16:04:33 2023, max compression
+gzip compressed data, was "georeader-spaceml-1.0.9.tar", last modified: Tue Dec  5 17:06:42 2023, max compression
```

## Comparing `georeader-spaceml-1.0.8.tar` & `georeader-spaceml-1.0.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2023-12-04 16:04:33.614062 georeader-spaceml-1.0.8/
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     7652 2023-04-26 06:58:45.000000 georeader-spaceml-1.0.8/LICENSE
--rw-r--r--   0 gonzalo   (1000) gonzalo   (1000)     6573 2023-12-04 16:04:33.614062 georeader-spaceml-1.0.8/PKG-INFO
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     4455 2023-12-04 16:01:46.000000 georeader-spaceml-1.0.8/README.md
-drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2023-12-04 16:04:33.610062 georeader-spaceml-1.0.8/georeader/
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)   118602 2023-10-10 04:52:24.000000 georeader-spaceml-1.0.8/georeader/SolarIrradiance_Thuillier.csv
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2154 2023-12-04 16:03:09.000000 georeader-spaceml-1.0.8/georeader/__init__.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2549 2023-10-02 08:09:01.000000 georeader-spaceml-1.0.8/georeader/abstract_reader.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2777 2023-04-26 06:58:45.000000 georeader-spaceml-1.0.8/georeader/geodataarray.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    27143 2023-10-02 08:21:15.000000 georeader-spaceml-1.0.8/georeader/geotensor.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    11353 2023-12-04 16:03:09.000000 georeader-spaceml-1.0.8/georeader/mosaic.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    10900 2023-12-04 16:00:35.000000 georeader-spaceml-1.0.8/georeader/plot.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    34153 2023-10-03 07:01:34.000000 georeader-spaceml-1.0.8/georeader/rasterio_reader.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     9514 2023-04-26 06:58:45.000000 georeader-spaceml-1.0.8/georeader/rasterize.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    28167 2023-12-04 16:01:46.000000 georeader-spaceml-1.0.8/georeader/read.py
-drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2023-12-04 16:04:33.610062 georeader-spaceml-1.0.8/georeader/readers/
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    57110 2023-07-20 07:42:55.000000 georeader-spaceml-1.0.8/georeader/readers/S2_SAFE_reader.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)        0 2023-04-26 06:58:45.000000 georeader-spaceml-1.0.8/georeader/readers/__init__.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    12416 2023-05-05 11:24:40.000000 georeader-spaceml-1.0.8/georeader/readers/download_pv_product.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2450 2023-09-27 11:03:47.000000 georeader-spaceml-1.0.8/georeader/readers/download_utils.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     6864 2023-12-04 16:00:35.000000 georeader-spaceml-1.0.8/georeader/readers/ee_image.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    14067 2023-12-04 16:00:35.000000 georeader-spaceml-1.0.8/georeader/readers/ee_query.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    22028 2023-10-06 14:06:02.000000 georeader-spaceml-1.0.8/georeader/readers/emit.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    17293 2023-05-05 15:01:48.000000 georeader-spaceml-1.0.8/georeader/readers/probav_image_operational.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2156 2023-04-26 06:58:45.000000 georeader-spaceml-1.0.8/georeader/readers/query_utils.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     3991 2023-04-26 06:58:45.000000 georeader-spaceml-1.0.8/georeader/readers/scihubcopernicus_query.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2199 2023-12-04 16:03:09.000000 georeader-spaceml-1.0.8/georeader/readers/tileserver.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     6764 2023-12-04 16:00:35.000000 georeader-spaceml-1.0.8/georeader/reflectance.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    12131 2023-10-18 15:46:26.000000 georeader-spaceml-1.0.8/georeader/save.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)       46 2023-07-13 10:32:41.000000 georeader-spaceml-1.0.8/georeader/save_cog.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     5414 2023-04-26 06:58:45.000000 georeader-spaceml-1.0.8/georeader/slices.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     3575 2023-09-22 12:24:44.000000 georeader-spaceml-1.0.8/georeader/vectorize.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    10533 2023-10-06 08:27:54.000000 georeader-spaceml-1.0.8/georeader/window_utils.py
-drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2023-12-04 16:04:33.610062 georeader-spaceml-1.0.8/georeader_spaceml.egg-info/
--rw-r--r--   0 gonzalo   (1000) gonzalo   (1000)     6573 2023-12-04 16:04:33.000000 georeader-spaceml-1.0.8/georeader_spaceml.egg-info/PKG-INFO
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     1077 2023-12-04 16:04:33.000000 georeader-spaceml-1.0.8/georeader_spaceml.egg-info/SOURCES.txt
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)        1 2023-12-04 16:04:33.000000 georeader-spaceml-1.0.8/georeader_spaceml.egg-info/dependency_links.txt
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)      502 2023-12-04 16:04:33.000000 georeader-spaceml-1.0.8/georeader_spaceml.egg-info/requires.txt
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)       10 2023-12-04 16:04:33.000000 georeader-spaceml-1.0.8/georeader_spaceml.egg-info/top_level.txt
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)       38 2023-12-04 16:04:33.614062 georeader-spaceml-1.0.8/setup.cfg
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2325 2023-11-14 08:36:01.000000 georeader-spaceml-1.0.8/setup.py
-drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2023-12-04 16:04:33.610062 georeader-spaceml-1.0.8/tests/
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     3796 2023-04-26 06:58:45.000000 georeader-spaceml-1.0.8/tests/test_geotensor.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     3583 2023-04-26 06:58:45.000000 georeader-spaceml-1.0.8/tests/test_rasterio_reader.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    11460 2023-04-26 06:58:45.000000 georeader-spaceml-1.0.8/tests/test_xarray_utils.py
+drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2023-12-05 17:06:42.611644 georeader-spaceml-1.0.9/
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     7652 2023-04-26 06:58:45.000000 georeader-spaceml-1.0.9/LICENSE
+-rw-r--r--   0 gonzalo   (1000) gonzalo   (1000)     6573 2023-12-05 17:06:42.611644 georeader-spaceml-1.0.9/PKG-INFO
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     4455 2023-12-04 16:01:46.000000 georeader-spaceml-1.0.9/README.md
+drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2023-12-05 17:06:42.603644 georeader-spaceml-1.0.9/georeader/
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)   118602 2023-10-10 04:52:24.000000 georeader-spaceml-1.0.9/georeader/SolarIrradiance_Thuillier.csv
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2154 2023-12-05 17:05:46.000000 georeader-spaceml-1.0.9/georeader/__init__.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2549 2023-10-02 08:09:01.000000 georeader-spaceml-1.0.9/georeader/abstract_reader.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2777 2023-04-26 06:58:45.000000 georeader-spaceml-1.0.9/georeader/geodataarray.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    27143 2023-10-02 08:21:15.000000 georeader-spaceml-1.0.9/georeader/geotensor.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    11353 2023-12-04 16:03:09.000000 georeader-spaceml-1.0.9/georeader/mosaic.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    10949 2023-12-05 09:26:06.000000 georeader-spaceml-1.0.9/georeader/plot.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    34153 2023-10-03 07:01:34.000000 georeader-spaceml-1.0.9/georeader/rasterio_reader.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     9514 2023-04-26 06:58:45.000000 georeader-spaceml-1.0.9/georeader/rasterize.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    28167 2023-12-04 16:01:46.000000 georeader-spaceml-1.0.9/georeader/read.py
+drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2023-12-05 17:06:42.607644 georeader-spaceml-1.0.9/georeader/readers/
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    57110 2023-07-20 07:42:55.000000 georeader-spaceml-1.0.9/georeader/readers/S2_SAFE_reader.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)        0 2023-04-26 06:58:45.000000 georeader-spaceml-1.0.9/georeader/readers/__init__.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    12416 2023-05-05 11:24:40.000000 georeader-spaceml-1.0.9/georeader/readers/download_pv_product.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2450 2023-09-27 11:03:47.000000 georeader-spaceml-1.0.9/georeader/readers/download_utils.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     6864 2023-12-04 16:00:35.000000 georeader-spaceml-1.0.9/georeader/readers/ee_image.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    14067 2023-12-04 16:00:35.000000 georeader-spaceml-1.0.9/georeader/readers/ee_query.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    22398 2023-12-05 10:14:29.000000 georeader-spaceml-1.0.9/georeader/readers/emit.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    17293 2023-05-05 15:01:48.000000 georeader-spaceml-1.0.9/georeader/readers/probav_image_operational.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2156 2023-04-26 06:58:45.000000 georeader-spaceml-1.0.9/georeader/readers/query_utils.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     3991 2023-04-26 06:58:45.000000 georeader-spaceml-1.0.9/georeader/readers/scihubcopernicus_query.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2199 2023-12-04 16:03:09.000000 georeader-spaceml-1.0.9/georeader/readers/tileserver.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     6764 2023-12-04 16:00:35.000000 georeader-spaceml-1.0.9/georeader/reflectance.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    12131 2023-10-18 15:46:26.000000 georeader-spaceml-1.0.9/georeader/save.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)       46 2023-07-13 10:32:41.000000 georeader-spaceml-1.0.9/georeader/save_cog.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     5414 2023-04-26 06:58:45.000000 georeader-spaceml-1.0.9/georeader/slices.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     3575 2023-09-22 12:24:44.000000 georeader-spaceml-1.0.9/georeader/vectorize.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    10533 2023-10-06 08:27:54.000000 georeader-spaceml-1.0.9/georeader/window_utils.py
+drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2023-12-05 17:06:42.607644 georeader-spaceml-1.0.9/georeader_spaceml.egg-info/
+-rw-r--r--   0 gonzalo   (1000) gonzalo   (1000)     6573 2023-12-05 17:06:42.000000 georeader-spaceml-1.0.9/georeader_spaceml.egg-info/PKG-INFO
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     1077 2023-12-05 17:06:42.000000 georeader-spaceml-1.0.9/georeader_spaceml.egg-info/SOURCES.txt
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)        1 2023-12-05 17:06:42.000000 georeader-spaceml-1.0.9/georeader_spaceml.egg-info/dependency_links.txt
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)      502 2023-12-05 17:06:42.000000 georeader-spaceml-1.0.9/georeader_spaceml.egg-info/requires.txt
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)       10 2023-12-05 17:06:42.000000 georeader-spaceml-1.0.9/georeader_spaceml.egg-info/top_level.txt
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)       38 2023-12-05 17:06:42.611644 georeader-spaceml-1.0.9/setup.cfg
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2325 2023-11-14 08:36:01.000000 georeader-spaceml-1.0.9/setup.py
+drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2023-12-05 17:06:42.607644 georeader-spaceml-1.0.9/tests/
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     3796 2023-04-26 06:58:45.000000 georeader-spaceml-1.0.9/tests/test_geotensor.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     3583 2023-04-26 06:58:45.000000 georeader-spaceml-1.0.9/tests/test_rasterio_reader.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    11460 2023-04-26 06:58:45.000000 georeader-spaceml-1.0.9/tests/test_xarray_utils.py
```

### Comparing `georeader-spaceml-1.0.8/LICENSE` & `georeader-spaceml-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.0.8/PKG-INFO` & `georeader-spaceml-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: georeader-spaceml
-Version: 1.0.8
+Version: 1.0.9
 Summary: Lightweight reader for raster files
 Author: Gonzalo Mateo-Garcia
 Keywords: raster reading,rasterio
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: rasterio
 Requires-Dist: numpy
```

### Comparing `georeader-spaceml-1.0.8/README.md` & `georeader-spaceml-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.0.8/georeader/SolarIrradiance_Thuillier.csv` & `georeader-spaceml-1.0.9/georeader/SolarIrradiance_Thuillier.csv`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.0.8/georeader/__init__.py` & `georeader-spaceml-1.0.9/georeader/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.0.8"
+__version__ = "1.0.9"
 
 import math
 from typing import Tuple, Any, Union
 from shapely.geometry.base import BaseGeometry
 from shapely import Geometry
 from shapely.geometry import shape, mapping
 import rasterio.warp
```

### Comparing `georeader-spaceml-1.0.8/georeader/abstract_reader.py` & `georeader-spaceml-1.0.9/georeader/abstract_reader.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.0.8/georeader/geodataarray.py` & `georeader-spaceml-1.0.9/georeader/geodataarray.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.0.8/georeader/geotensor.py` & `georeader-spaceml-1.0.9/georeader/geotensor.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.0.8/georeader/mosaic.py` & `georeader-spaceml-1.0.9/georeader/mosaic.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.0.8/georeader/plot.py` & `georeader-spaceml-1.0.9/georeader/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -267,14 +267,15 @@
         if kwargs_scalebar is None:
             kwargs_scalebar = {"dx":1}
         if "dx" not in kwargs_scalebar:
             kwargs_scalebar["dx"] = 1
         
         ax.add_artist(ScaleBar(**kwargs_scalebar))
     
+    # TODO https://github.com/eelcovv/LatLonCalc
     if bounds_in_latlng:
         from matplotlib.ticker import FuncFormatter
 
         xmin, ymin, xmax, ymax = mask.bounds
 
         @FuncFormatter
         def x_formatter(x, pos):
```

### Comparing `georeader-spaceml-1.0.8/georeader/rasterio_reader.py` & `georeader-spaceml-1.0.9/georeader/rasterio_reader.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.0.8/georeader/rasterize.py` & `georeader-spaceml-1.0.9/georeader/rasterize.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.0.8/georeader/read.py` & `georeader-spaceml-1.0.9/georeader/read.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.0.8/georeader/readers/S2_SAFE_reader.py` & `georeader-spaceml-1.0.9/georeader/readers/S2_SAFE_reader.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.0.8/georeader/readers/download_pv_product.py` & `georeader-spaceml-1.0.9/georeader/readers/download_pv_product.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.0.8/georeader/readers/download_utils.py` & `georeader-spaceml-1.0.9/georeader/readers/download_utils.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.0.8/georeader/readers/ee_image.py` & `georeader-spaceml-1.0.9/georeader/readers/ee_image.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.0.8/georeader/readers/ee_query.py` & `georeader-spaceml-1.0.9/georeader/readers/ee_query.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.0.8/georeader/readers/emit.py` & `georeader-spaceml-1.0.9/georeader/readers/emit.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,21 +29,21 @@
     home_dir = os.path.join(os.path.expanduser('~'),".georeader")
     json_file = os.path.join(home_dir, "auth_emit.json")
     if not os.path.exists(json_file):
         os.makedirs(home_dir, exist_ok=True)
         with open(json_file, "w") as fh:
             json.dump({"user": "SET-USER", "password": "SET-PASSWORD"}, fh)
 
-        raise FileNotFoundError(f"In order to download Proba-V images add user and password to file : {json_file}")
+        raise FileNotFoundError(f"In order to download EMIT images add user and password to file : {json_file}")
 
     with open(json_file, "r") as fh:
         data = json.load(fh)
     
     if data["user"] == "SET-USER":
-        raise FileNotFoundError(f"In order to download Proba-V images add user and password to file : {json_file}")
+        raise FileNotFoundError(f"In order to download EMIT images add user and password to file : {json_file}")
 
     return (data["user"], data["password"])
 
 def product_name_from_params(scene_fid:str, orbit:str, daac_scene_number:str)-> str:
     """
     Return the product name from the scene_fid, daac_scene_number and orbit
 
@@ -74,30 +74,35 @@
     date, orbit, daac_scene_number= product_name.split("_")[4:7]
 
     dt = datetime.strptime(date, "%Y%m%dT%H%M%S").replace(tzinfo=timezone.utc)
 
     return scene_fid, orbit, daac_scene_number, dt
 
 def download_product(link_down:str, filename:Optional[str]=None,
-                     display_progress_bar:bool=True) -> str:
+                     display_progress_bar:bool=True,
+                     auth:Optional[Tuple[str, str]] = None) -> str:
     """
-    Download a product from the EMIT website.
-    See: https://git.earthdata.nasa.gov/projects/LPDUR/repos/daac_data_download_python/browse
+    Download a product from the EMIT website (https://search.earthdata.nasa.gov/search). 
+    It requires that you have an account in the NASA Earthdata portal. 
+
+    This code is based on this example: https://git.earthdata.nasa.gov/projects/LPDUR/repos/daac_data_download_python/browse
 
     Args:
         link_down: link to the product
         filename: filename to save the product
         display_progress_bar: display tqdm progress bar
+        auth: tuple with user and password to download the product. If None, it will try to read the user and password from ~/.georeader/auth_emit.json 
 
     Example:
         >>> link_down = 'https://data.lpdaac.earthdatacloud.nasa.gov/lp-prod-protected/EMITL1BRAD.001/EMIT_L1B_RAD_001_20220828T051941_2224004_006/EMIT_L1B_RAD_001_20220828T051941_2224004_006.nc'
         >>> filename = download_product(link_down)
     """
-    auth_emit = get_auth()
-    return download_product_base(link_down, filename=filename, auth=auth_emit,
+    if auth is None:
+        auth = get_auth()
+    return download_product_base(link_down, filename=filename, auth=auth,
                                   display_progress_bar=display_progress_bar, 
                                   verify=False)
 
 
 def get_radiance_link(product_path:str) -> str:
     """
     Get the link to download a product from the EMIT website.
```

### Comparing `georeader-spaceml-1.0.8/georeader/readers/probav_image_operational.py` & `georeader-spaceml-1.0.9/georeader/readers/probav_image_operational.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.0.8/georeader/readers/query_utils.py` & `georeader-spaceml-1.0.9/georeader/readers/query_utils.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.0.8/georeader/readers/scihubcopernicus_query.py` & `georeader-spaceml-1.0.9/georeader/readers/scihubcopernicus_query.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.0.8/georeader/readers/tileserver.py` & `georeader-spaceml-1.0.9/georeader/readers/tileserver.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.0.8/georeader/reflectance.py` & `georeader-spaceml-1.0.9/georeader/reflectance.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.0.8/georeader/save.py` & `georeader-spaceml-1.0.9/georeader/save.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.0.8/georeader/slices.py` & `georeader-spaceml-1.0.9/georeader/slices.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.0.8/georeader/vectorize.py` & `georeader-spaceml-1.0.9/georeader/vectorize.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.0.8/georeader/window_utils.py` & `georeader-spaceml-1.0.9/georeader/window_utils.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.0.8/georeader_spaceml.egg-info/PKG-INFO` & `georeader-spaceml-1.0.9/georeader_spaceml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: georeader-spaceml
-Version: 1.0.8
+Version: 1.0.9
 Summary: Lightweight reader for raster files
 Author: Gonzalo Mateo-Garcia
 Keywords: raster reading,rasterio
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: rasterio
 Requires-Dist: numpy
```

### Comparing `georeader-spaceml-1.0.8/georeader_spaceml.egg-info/SOURCES.txt` & `georeader-spaceml-1.0.9/georeader_spaceml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.0.8/setup.py` & `georeader-spaceml-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.0.8/tests/test_geotensor.py` & `georeader-spaceml-1.0.9/tests/test_geotensor.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.0.8/tests/test_rasterio_reader.py` & `georeader-spaceml-1.0.9/tests/test_rasterio_reader.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.0.8/tests/test_xarray_utils.py` & `georeader-spaceml-1.0.9/tests/test_xarray_utils.py`

 * *Files identical despite different names*

