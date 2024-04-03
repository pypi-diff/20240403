# Comparing `tmp/quadgrid-0.1.3.tar.gz` & `tmp/quadgrid-0.1.4.tar.gz`

## Comparing `quadgrid-0.1.3.tar` & `quadgrid-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 quadgrid-0.1.3/.DS_Store
--rw-r--r--   0        0        0    51548 2020-02-02 00:00:00.000000 quadgrid-0.1.3/README_files/1bd03ad7-9b47-4b9b-b497-5a05cf2ba6cd.png
--rwxr-xr-x   0        0        0   277947 2020-02-02 00:00:00.000000 quadgrid-0.1.3/docs/README.ipynb
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 quadgrid-0.1.3/quadgrid/__init__.py
--rwxr-xr-x   0        0        0     1270 2020-02-02 00:00:00.000000 quadgrid-0.1.3/quadgrid/distance.py
--rwxr-xr-x   0        0        0     4785 2020-02-02 00:00:00.000000 quadgrid-0.1.3/quadgrid/grid.py
--rwxr-xr-x   0        0        0     6719 2020-02-02 00:00:00.000000 quadgrid-0.1.3/quadgrid/qtree.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 quadgrid-0.1.3/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 quadgrid-0.1.3/LICENSE
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 quadgrid-0.1.3/README.md
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 quadgrid-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 quadgrid-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    51548 2020-02-02 00:00:00.000000 quadgrid-0.1.4/README_files/1bd03ad7-9b47-4b9b-b497-5a05cf2ba6cd.png
+-rwxr-xr-x   0        0        0   277947 2020-02-02 00:00:00.000000 quadgrid-0.1.4/docs/README.ipynb
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 quadgrid-0.1.4/quadgrid/__init__.py
+-rwxr-xr-x   0        0        0     1270 2020-02-02 00:00:00.000000 quadgrid-0.1.4/quadgrid/distance.py
+-rwxr-xr-x   0        0        0     4857 2020-02-02 00:00:00.000000 quadgrid-0.1.4/quadgrid/grid.py
+-rwxr-xr-x   0        0        0     6719 2020-02-02 00:00:00.000000 quadgrid-0.1.4/quadgrid/qtree.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 quadgrid-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 quadgrid-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 quadgrid-0.1.4/README.md
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 quadgrid-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 quadgrid-0.1.4/PKG-INFO
```

### Comparing `quadgrid-0.1.3/README_files/1bd03ad7-9b47-4b9b-b497-5a05cf2ba6cd.png` & `quadgrid-0.1.4/README_files/1bd03ad7-9b47-4b9b-b497-5a05cf2ba6cd.png`

 * *Files identical despite different names*

### Comparing `quadgrid-0.1.3/docs/README.ipynb` & `quadgrid-0.1.4/docs/README.ipynb`

 * *Files identical despite different names*

### Comparing `quadgrid-0.1.3/quadgrid/distance.py` & `quadgrid-0.1.4/quadgrid/distance.py`

 * *Files identical despite different names*

### Comparing `quadgrid-0.1.3/quadgrid/grid.py` & `quadgrid-0.1.4/quadgrid/grid.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 # Authalic radius of Earth in kilometres
 R = 6371.007
 
 
 class QuadGrid():
     def __init__(self, res, lon_bounds=(-180,180), lat_bounds=(-90,90)):
-        """Converts a single (lon, lat) quadcell centroid to qid.
+        """Class constructor for QuadGrid.
 
         Parameters
         ----------
             res : float
                 Quadgrid resolution in decimal degrees.
             lon_bounds : (float, float)
                 Longitude bounds to be covered by quadgrid.
@@ -33,16 +33,18 @@
                 Latitude bounds to be covered by quadgrid.
         """
         self.res = res
         self.lon_bounds = lon_bounds
         self.lat_bounds = lat_bounds
 
         # Global centroid lons and lats
-        lons_1d = np.arange(-180+res/2, 180+res/2, res)
-        lats_1d = np.arange(-90+res/2, 90+res/2, res)
+        lons_1d = np.arange(res/2, 180+res/2, res)
+        lons_1d = np.sort(np.r_[-lons_1d, lons_1d])
+        lats_1d = np.arange(res/2, 90+res/2, res)
+        lats_1d = np.sort(np.r_[-lats_1d, lats_1d])
 
         # Apply bounds
         self.lons_1d = lons_1d[(lons_1d>(lon_bounds[0]-res/2)) &
                                (lons_1d<(lon_bounds[1]+res/2))]
         self.lats_1d = lats_1d[(lats_1d>(lat_bounds[0]-res/2)) &
                                (lats_1d<(lat_bounds[1]+res/2))]
         lons_2d, lats_2d = np.meshgrid(self.lons_1d, self.lats_1d, indexing='xy')
```

### Comparing `quadgrid-0.1.3/quadgrid/qtree.py` & `quadgrid-0.1.4/quadgrid/qtree.py`

 * *Files identical despite different names*

### Comparing `quadgrid-0.1.3/.gitignore` & `quadgrid-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `quadgrid-0.1.3/LICENSE` & `quadgrid-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `quadgrid-0.1.3/README.md` & `quadgrid-0.1.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -19,10 +19,13 @@
 
 Individual quadcells at a given resolution are labelled with unique
 quadtreeIDs (qids). In the simplified example below, the red point is in top-level cell '2', then cell '2', then '0' then '3' giving a nominal qid of '2203'. In practice, quadtrees lend themselves to a base-4 encoding, allowing them to be stored and processed efficiently as integers.
 
 ![image.png](README_files/1bd03ad7-9b47-4b9b-b497-5a05cf2ba6cd.png)
 
 ## Versions
+`0.1.4` Fixed bug in quadgrids defined at a resolution coarser than 1 degree
+`0.1.3` Added resolution to DataFrame conversions; apply_mask can accept GeoDataFrames
 `0.1.2` Changed email address in pyproject.toml
 `0.1.1` Bug fix to ensure user-specified bounded grid is consistent with the global grid
-`0.1.0` First release
+`0.1.0` First release
+
```

### Comparing `quadgrid-0.1.3/pyproject.toml` & `quadgrid-0.1.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "quadgrid"
-version = "0.1.3"
+version = "0.1.4"
 description = "Quadtree grid generator"
 authors = [
            { name = "Mutahar Chalmers", email = "mutahar.chalmers@gmail.com" },
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
 classifiers = [
```

### Comparing `quadgrid-0.1.3/PKG-INFO` & `quadgrid-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: quadgrid
-Version: 0.1.3
+Version: 0.1.4
 Summary: Quadtree grid generator
 Project-URL: Homepage, https://github.com/FuzzyDuck79/quadgrid
 Author-email: Mutahar Chalmers <mutahar.chalmers@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Mutahar Chalmers
         
@@ -61,10 +61,13 @@
 
 Individual quadcells at a given resolution are labelled with unique
 quadtreeIDs (qids). In the simplified example below, the red point is in top-level cell '2', then cell '2', then '0' then '3' giving a nominal qid of '2203'. In practice, quadtrees lend themselves to a base-4 encoding, allowing them to be stored and processed efficiently as integers.
 
 ![image.png](README_files/1bd03ad7-9b47-4b9b-b497-5a05cf2ba6cd.png)
 
 ## Versions
+`0.1.4` Fixed bug in quadgrids defined at a resolution coarser than 1 degree
+`0.1.3` Added resolution to DataFrame conversions; apply_mask can accept GeoDataFrames
 `0.1.2` Changed email address in pyproject.toml
 `0.1.1` Bug fix to ensure user-specified bounded grid is consistent with the global grid
-`0.1.0` First release
+`0.1.0` First release
+
```

