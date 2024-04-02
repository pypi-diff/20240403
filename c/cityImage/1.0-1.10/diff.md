# Comparing `tmp/cityImage-1.0.tar.gz` & `tmp/cityImage-1.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cityImage-1.0.tar", last modified: Sun Jun 18 11:05:33 2023, max compression
+gzip compressed data, was "cityImage-1.10.tar", last modified: Tue Apr  2 22:40:29 2024, max compression
```

## Comparing `cityImage-1.0.tar` & `cityImage-1.10.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 11:05:33.853129 cityImage-1.0/
--rw-rw-rw-   0        0        0     1105 2023-06-13 10:34:08.000000 cityImage-1.0/LICENSE.txt
--rw-rw-rw-   0        0        0     1712 2023-06-18 11:05:33.853129 cityImage-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1317 2023-06-18 11:01:42.000000 cityImage-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-18 11:05:33.837504 cityImage-1.0/cityImage/
--rw-rw-rw-   0        0        0      693 2023-06-13 10:34:08.000000 cityImage-1.0/cityImage/__init__.py
--rw-rw-rw-   0        0        0    12908 2023-06-14 13:31:22.000000 cityImage-1.0/cityImage/angles.py
--rw-rw-rw-   0        0        0    21283 2023-06-16 15:35:52.000000 cityImage-1.0/cityImage/barriers.py
--rw-rw-rw-   0        0        0     9698 2023-06-13 17:53:34.000000 cityImage-1.0/cityImage/centrality.py
--rw-rw-rw-   0        0        0    30563 2023-06-17 10:40:51.000000 cityImage-1.0/cityImage/clean.py
--rw-rw-rw-   0        0        0     5161 2023-06-13 17:49:40.000000 cityImage-1.0/cityImage/colors.py
--rw-rw-rw-   0        0        0    12650 2023-06-13 17:48:06.000000 cityImage-1.0/cityImage/graph.py
--rw-rw-rw-   0        0        0     6449 2023-06-13 17:44:49.000000 cityImage-1.0/cityImage/land_use.py
--rw-rw-rw-   0        0        0    41705 2023-06-14 12:35:20.000000 cityImage-1.0/cityImage/landmarks.py
--rw-rw-rw-   0        0        0    12026 2023-06-14 12:36:11.000000 cityImage-1.0/cityImage/load.py
--rw-rw-rw-   0        0        0    33476 2023-06-17 10:40:08.000000 cityImage-1.0/cityImage/plot.py
--rw-rw-rw-   0        0        0    18360 2023-06-14 13:40:03.000000 cityImage-1.0/cityImage/regions.py
--rw-rw-rw-   0        0        0    21890 2023-06-14 16:52:24.000000 cityImage-1.0/cityImage/utilities.py
-drwxrwxrwx   0        0        0        0 2023-06-18 11:05:33.853129 cityImage-1.0/cityImage.egg-info/
--rw-rw-rw-   0        0        0     1712 2023-06-18 11:05:33.000000 cityImage-1.0/cityImage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      517 2023-06-18 11:05:33.000000 cityImage-1.0/cityImage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 11:05:33.000000 cityImage-1.0/cityImage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-06-18 11:05:33.000000 cityImage-1.0/cityImage.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-18 11:05:33.000000 cityImage-1.0/cityImage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-18 11:05:33.853129 cityImage-1.0/setup.cfg
--rw-rw-rw-   0        0        0      713 2023-06-18 11:01:38.000000 cityImage-1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-18 11:05:33.853129 cityImage-1.0/tests/
--rw-rw-rw-   0        0        0        0 2023-06-13 10:34:08.000000 cityImage-1.0/tests/__init__.py
--rw-rw-rw-   0        0        0    19016 2023-06-14 19:45:27.000000 cityImage-1.0/tests/test_cityImage.py
+drwxrwxrwx   0        0        0        0 2024-04-02 22:40:29.085066 cityImage-1.10/
+-rw-rw-rw-   0        0        0    35823 2024-04-02 17:39:20.000000 cityImage-1.10/LICENSE.txt
+-rw-rw-rw-   0        0        0     2246 2024-04-02 22:40:29.083031 cityImage-1.10/PKG-INFO
+-rw-rw-rw-   0        0        0     1730 2023-06-18 21:23:10.000000 cityImage-1.10/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 22:40:29.052069 cityImage-1.10/cityImage/
+-rw-rw-rw-   0        0        0      693 2024-02-01 14:20:07.000000 cityImage-1.10/cityImage/__init__.py
+-rw-rw-rw-   0        0        0    12908 2024-02-01 14:20:07.000000 cityImage-1.10/cityImage/angles.py
+-rw-rw-rw-   0        0        0    21294 2024-02-21 09:29:16.000000 cityImage-1.10/cityImage/barriers.py
+-rw-rw-rw-   0        0        0     9698 2024-02-01 14:20:07.000000 cityImage-1.10/cityImage/centrality.py
+-rw-rw-rw-   0        0        0    30607 2024-04-01 14:22:52.000000 cityImage-1.10/cityImage/clean.py
+-rw-rw-rw-   0        0        0     5161 2024-02-01 14:20:07.000000 cityImage-1.10/cityImage/colors.py
+-rw-rw-rw-   0        0        0    12644 2024-03-06 12:10:53.000000 cityImage-1.10/cityImage/graph.py
+-rw-rw-rw-   0        0        0     6449 2024-02-01 14:20:07.000000 cityImage-1.10/cityImage/land_use.py
+-rw-rw-rw-   0        0        0    42095 2024-04-02 22:24:45.000000 cityImage-1.10/cityImage/landmarks.py
+-rw-rw-rw-   0        0        0    12026 2024-02-01 14:20:07.000000 cityImage-1.10/cityImage/load.py
+-rw-rw-rw-   0        0        0    33558 2024-02-01 16:51:16.000000 cityImage-1.10/cityImage/plot.py
+-rw-rw-rw-   0        0        0    18360 2024-02-01 14:20:07.000000 cityImage-1.10/cityImage/regions.py
+-rw-rw-rw-   0        0        0    22543 2024-04-01 15:26:57.000000 cityImage-1.10/cityImage/utilities.py
+drwxrwxrwx   0        0        0        0 2024-04-02 22:40:29.072032 cityImage-1.10/cityImage.egg-info/
+-rw-rw-rw-   0        0        0     2246 2024-04-02 22:40:28.000000 cityImage-1.10/cityImage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      517 2024-04-02 22:40:28.000000 cityImage-1.10/cityImage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 22:40:28.000000 cityImage-1.10/cityImage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2024-04-02 22:40:28.000000 cityImage-1.10/cityImage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-02 22:40:28.000000 cityImage-1.10/cityImage.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-02 22:40:29.088035 cityImage-1.10/setup.cfg
+-rw-rw-rw-   0        0        0      755 2024-04-02 22:32:54.000000 cityImage-1.10/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 22:40:29.079034 cityImage-1.10/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-13 10:34:08.000000 cityImage-1.10/tests/__init__.py
+-rw-rw-rw-   0        0        0    19019 2024-04-01 14:03:11.000000 cityImage-1.10/tests/test_cityImage.py
```

### Comparing `cityImage-1.0/PKG-INFO` & `cityImage-1.10/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,39 @@
 Metadata-Version: 2.1
 Name: cityImage
-Version: 1.0
+Version: 1.10
 Summary: A package for studying urban form and obtaining the computational Image of the City
 Author: Gabriele Filomena
 Author-email: gabriele.filomena@liverpool.ac.uk
 Keywords: urban Form Analysis,Computational Image of the City,Kevin Lynch,cognitive maps
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: osmnx>=1.9.1
+Requires-Dist: python-louvain>=0.16
+Requires-Dist: pyvista>=0.37
+Requires-Dist: mapclassify>=2.5.0
 
 [![CodeFactor](https://www.codefactor.io/repository/github/g-filomena/cityimage/badge)](https://www.codefactor.io/repository/github/g-filomena/cityimage)
 [![Actions Status](https://github.com/g-filomena/cityimage/workflows/tests/badge.svg)](https://github.com//g-filomena/cityimage/actions?query=workflow%3Atests)
 [![codecov](https://codecov.io/gh/g-filomena/cityImage/branch/master/graph/badge.svg)](https://codecov.io/gh/g-filomena/cityImage)
+[![PyPI version](https://badge.fury.io/py/cityImage.svg)](https://badge.fury.io/py/cityImage)
 
 # cityImage
 
 **A tool for analysing urban legibility and extracting The Computational Image of the City**
+For full documentation and examples see [the user manual](https://cityimage-docs.readthedocs.io/en/latest/).
 
 This repository provides a set of functions to extract salient urban features in line with the definitions laid down by Kevin Lynch in [The Image of The City](https://mitpress.mit.edu/books/image-city) using open and freely available geospatial datasets.
+The methods are fully documented in *A Computational approach to The Image of the City* by Filomena, Verstegen, and Manley, published in [Cities](https://doi.org/10.1016/j.cities.2019.01.006).
 
-The tools are written in Python and uses a series of libraries, including [Geopandas](http://geopandas.org), [OSMNx](https://osmnx.readthedocs.io/en/stable/), [PyVista](https://docs.pyvista.org/version/stable/) and related dependencies.
+The tools are written in Python and requires:
 
-The methods are fully documented in *A Computational approach to â€˜The Image of the Cityâ€™* by Filomena, Verstegen, and Manley, published in [Cities](https://doi.org/10.1016/j.cities.2019.01.006).
-The full documentation is available at 
+* [OSMNx](https://osmnx.readthedocs.io/en/stable/).
+* [PyVista](https://docs.pyvista.org/version/stable/).
+* [python-louvain](https://github.com/taynaud/python-louvain).
+* [mapclassify](https://github.com/pysal/mapclassify).
 
-## Introduction
+It is built on [GeoPandas](https://github.com/geopandas/geopandas), [NetworkX](https://github.com/networkx/networkx), and [Shapely](https://github.com/shapely/shapely).
+
+## How to install *cityImage*
+
+    pip install cityImage
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cityImage-1.0/README.md` & `cityImage-1.10/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,25 @@
 [![CodeFactor](https://www.codefactor.io/repository/github/g-filomena/cityimage/badge)](https://www.codefactor.io/repository/github/g-filomena/cityimage)
 [![Actions Status](https://github.com/g-filomena/cityimage/workflows/tests/badge.svg)](https://github.com//g-filomena/cityimage/actions?query=workflow%3Atests)
 [![codecov](https://codecov.io/gh/g-filomena/cityImage/branch/master/graph/badge.svg)](https://codecov.io/gh/g-filomena/cityImage)
+[![PyPI version](https://badge.fury.io/py/cityImage.svg)](https://badge.fury.io/py/cityImage)
 
 # cityImage
 
 **A tool for analysing urban legibility and extracting The Computational Image of the City**
+For full documentation and examples see [the user manual](https://cityimage-docs.readthedocs.io/en/latest/).
 
 This repository provides a set of functions to extract salient urban features in line with the definitions laid down by Kevin Lynch in [The Image of The City](https://mitpress.mit.edu/books/image-city) using open and freely available geospatial datasets.
+The methods are fully documented in *A Computational approach to The Image of the City* by Filomena, Verstegen, and Manley, published in [Cities](https://doi.org/10.1016/j.cities.2019.01.006).
 
-The tools are written in Python and uses a series of libraries, including [Geopandas](http://geopandas.org), [OSMNx](https://osmnx.readthedocs.io/en/stable/), [PyVista](https://docs.pyvista.org/version/stable/) and related dependencies.
+The tools are written in Python and requires:
 
-The methods are fully documented in *A Computational approach to ‘The Image of the City’* by Filomena, Verstegen, and Manley, published in [Cities](https://doi.org/10.1016/j.cities.2019.01.006).
-The full documentation is available at 
+* [OSMNx](https://osmnx.readthedocs.io/en/stable/).
+* [PyVista](https://docs.pyvista.org/version/stable/).
+* [python-louvain](https://github.com/taynaud/python-louvain).
+* [mapclassify](https://github.com/pysal/mapclassify).
 
-## Introduction
+It is built on [GeoPandas](https://github.com/geopandas/geopandas), [NetworkX](https://github.com/networkx/networkx), and [Shapely](https://github.com/shapely/shapely).
+
+## How to install *cityImage*
+
+    pip install cityImage
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cityImage-1.0/cityImage/__init__.py` & `cityImage-1.10/cityImage/__init__.py`

 * *Files identical despite different names*

### Comparing `cityImage-1.0/cityImage/angles.py` & `cityImage-1.10/cityImage/angles.py`

 * *Files identical despite different names*

### Comparing `cityImage-1.0/cityImage/barriers.py` & `cityImage-1.10/cityImage/barriers.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             to_keep.append('secondary')
 
     tags = {'highway': True}
     roads = downloader(place = place, download_method = download_method, tags = tags, distance = distance).to_crs(crs)
     roads = roads[roads.highway.isin(to_keep)]
     # exclude tunnels
     if "tunnel" in roads.columns:
-        roads['tunnel'].fillna(0, inplace=True)
+        roads['tunnel'] = roads['tunnel'].fillna(0)
         roads = roads[roads.tunnel == 0]
         
     roads = roads.unary_union
     roads = _simplify_barrier(roads)
     df = pd.DataFrame({'geometry': roads, 'barrier_type': ['road'] * len(roads)})
     road_barriers = gpd.GeoDataFrame(df, geometry = df['geometry'], crs = crs)
        
@@ -159,15 +159,15 @@
     crs = 'EPSG:' + str(epsg)
     tags = {"railway":"rail"}
     railways = downloader(place = place, download_method = download_method, tags = tags, distance = distance).to_crs(crs)
     # removing light_rail, in case
     if not keep_light_rail:
         railways = railways[railways.railway != 'light_rail']
     if "tunnel" in railways.columns:
-        railways['tunnel'].fillna(0, inplace=True)
+        railways['tunnel'] = railways['tunnel'].fillna(0)
         railways = railways[railways.tunnel == 0]
         
     r = railways.unary_union
     p = polygonize_full(r)
     railways = unary_union(p).buffer(10).boundary # to simpify a bit
     railways = _simplify_barrier(railways)
```

### Comparing `cityImage-1.0/cityImage/centrality.py` & `cityImage-1.10/cityImage/centrality.py`

 * *Files identical despite different names*

### Comparing `cityImage-1.0/cityImage/clean.py` & `cityImage-1.10/cityImage/clean.py`

 * *Files 1% similar despite different names*

```diff
@@ -428,17 +428,18 @@
         # simplify the graph                           
         nodes_gdf, edges_gdf = simplify_graph(nodes_gdf, edges_gdf, nodes_to_keep_regardless) 
     
     if remove_islands:
         nodes_gdf, edges_gdf = remove_disconnected_islands(nodes_gdf, edges_gdf, 'nodeID')
     
     nodes_gdf['x'], nodes_gdf['y'] = list(zip(*[(r.coords[0][0], r.coords[0][1]) for r in nodes_gdf.geometry]))
-    edges_gdf.drop(['coords', 'tmp', 'code'], axis = 1, inplace = True, errors = 'ignore') # remove temporary columns
+    
     nodes_gdf['nodeID'] = nodes_gdf.nodeID.astype(int)
     edges_gdf = correct_edges(nodes_gdf, edges_gdf) # correct edges coordinates
+    edges_gdf.drop(['coords', 'tmp', 'code', 'wkt', 'fixing', 'to_fix'], axis = 1, inplace = True, errors = 'ignore') # remove temporary columns
     edges_gdf['length'] = edges_gdf['geometry'].length
     edges_gdf.set_index('edgeID', drop = False, inplace = True, append = False)
     nodes_gdf, edges_gdf = reset_index_graph_gdfs(nodes_gdf, edges_gdf, nodeID = "nodeID")
     edges_gdf.index.name = None
     
     return nodes_gdf, edges_gdf
 
@@ -621,15 +622,15 @@
 
     # assign the results to self_loops['to_fix']
     edges_gdf['to_fix'] = to_fix
     edges_gdf['fixing'] = [True if len(to_fix) > 0 else False for to_fix in edges_gdf['to_fix']]
     to_fix = edges_gdf[edges_gdf['fixing'] == True].copy()
     edges_gdf = edges_gdf[edges_gdf['fixing'] == False]
     if len(to_fix) == 0:
-        return edges_gdf
+        return nodes_gdf, edges_gdf
     return add_fixed_edges(edges_gdf, to_fix)    
     
 def remove_disconnected_islands(nodes_gdf, edges_gdf, nodeID):
     """
     Remove disconnected islands from a graph.
 
     Parameters:
```

### Comparing `cityImage-1.0/cityImage/colors.py` & `cityImage-1.10/cityImage/colors.py`

 * *Files identical despite different names*

### Comparing `cityImage-1.0/cityImage/graph.py` & `cityImage-1.10/cityImage/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import warnings
 warnings.simplefilter(action="ignore", category=FutureWarning)
+
+
 import osmnx as ox
 import pandas as pd
 import numpy as np
 import geopandas as gpd
 import networkx as nx
 
 import math
@@ -149,15 +151,15 @@
                                                 (centroids_gdf['u'] == row['u']) | ((centroids_gdf['v'] == row['u']) & (centroids_gdf['oneway'] == 0))].index), axis = 1)
     
     # creating vertexes representing street segments (centroids)
     centroids_data = centroids_gdf.drop(['geometry', 'centroid'], axis = 1)
     if epsg is None: 
         crs = nodes_gdf.crs
     else: 
-        crs = {'init': 'epsg:' + str(epsg)}
+        crs = 'EPSG:' + str(epsg)
     nodes_dual = gpd.GeoDataFrame(centroids_data, crs=crs, geometry=centroids_gdf['centroid'])
     nodes_dual['x'], nodes_dual['y'] = [x.coords.xy[0][0] for x in centroids_gdf['centroid']],[y.coords.xy[1][0] for y in centroids_gdf['centroid']]
     nodes_dual.index = nodes_dual.edgeID
     nodes_dual.index.name = None
         
     # creating fictious links between centroids
     edges_dual = pd.DataFrame(columns=['u','v', 'geometry', 'length'])
```

### Comparing `cityImage-1.0/cityImage/land_use.py` & `cityImage-1.10/cityImage/land_use.py`

 * *Files identical despite different names*

### Comparing `cityImage-1.0/cityImage/landmarks.py` & `cityImage-1.10/cityImage/landmarks.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     buildings_gdf = obstructions_gdf[obstructions_gdf.geometry.within(case_study_area)]
     # clipping buildings in the case-study area
 
     return buildings_gdf, obstructions_gdf
     
 def get_buildings_fromOSM(place, download_method: str, epsg = None, distance = 1000):
     """    
-    The function downloads and cleans buildings footprint geometries and create a buildings GeoDataFrames for the area of interest.
+    The function downloads and cleans building footprint geometries and create a buildings GeoDataFrames for the area of interest.
     The function exploits OSMNx functions for downloading the data as well as for projecting it.
     The land use classification for each building is extracted. Only relevant columns are kept.   
             
     Parameters
     ----------
     place: str, tuple, Shapely Polygon
         Name of cities or areas in OSM: 
@@ -118,21 +118,27 @@
     buildings_gdf['land_use_raw'] = None
     buildings_gdf['land_use_raw'] = buildings_gdf.filter(regex='^building:use:').apply(lambda x: x.name[13:] if x.notnull().any() else None)
     buildings_gdf.drop(columns=[col for col in buildings_gdf.columns if col not in columns_to_keep], inplace=True)
 
     # remove the empty geometries
     buildings_gdf = buildings_gdf[~buildings_gdf['geometry'].is_empty]
     # replace 'yes' with NaN in 'building' column
-    buildings_gdf['building'].replace('yes', np.nan, inplace=True)
+    buildings_gdf['building'] = buildings_gdf['building'].replace('yes', np.nan)
     # fill missing values in 'building' column with 'amenity' values
-    buildings_gdf['building'].fillna(value=buildings_gdf['amenity'], inplace=True)
+    buildings_gdf['building'] = buildings_gdf['building'].fillna(value=buildings_gdf['amenity'])
+
     # fill missing values in 'land_use_raw' column with 'building' values
-    buildings_gdf['land_use_raw'].fillna(value=buildings_gdf['building'], inplace=True)
+    # Create a mask for rows where the 'building' column is NA
+    mask = buildings_gdf['building'].isna()
+    # Use the mask to assign values from 'amenity' to 'building' only where 'building' is NA
+    buildings_gdf.loc[mask, 'building'] = buildings_gdf.loc[mask, 'amenity']
+
+    buildings_gdf['land_use_raw'] = buildings_gdf['land_use_raw'].fillna(value=buildings_gdf['building'])
     # fill remaining missing values in 'land_use_raw' column with 'residential'
-    buildings_gdf['land_use_raw'].fillna(value='residential', inplace=True)
+    buildings_gdf['land_use_raw'] = buildings_gdf['land_use_raw'].fillna(value='residential')
 
     buildings_gdf = buildings_gdf[['geometry', 'historic', 'land_use_raw']]
     buildings_gdf['area'] = buildings_gdf.geometry.area
     buildings_gdf = buildings_gdf[buildings_gdf['area'] >= 50] 
     
     # reset index
     buildings_gdf = buildings_gdf.reset_index(drop = True)
@@ -455,17 +461,16 @@
     coords = mapping(envelope)["coordinates"][0]
     d = [(Point(coords[0])).distance(Point(coords[1])), (Point(coords[1])).distance(Point(coords[2]))]
     width = min(d)
     return width*building_height
  
 def get_historical_buildings_fromOSM(place, download_method, epsg = None, distance = 1000):
     """    
-    The function downloads and cleans buildings footprint geometries and create a buildings GeoDataFrames for the area of interest.
-    The function exploits OSMNx functions for downloading the data as well as for projecting it.
-    The land use classification for each building is extracted. Only relevant columns are kept.   
+    The function downloads and cleans building footprint geometries and create a buildings GeoDataFrames for the area of interest.
+    However, it only keeps the buildings that are considered historical buildings or heritage buildings in OSM. 
             
     Parameters
     ----------
     place: str, tuple, Shapely Polygon
         Name of cities or areas in OSM: 
         - when using "distance_from_point" please provide a (lat, lon) tuple to create the bounding box around it; 
         - when using "distance_from_address" provide an existing OSM address; 
@@ -505,15 +510,15 @@
 
     historic_buildings.loc[historic_buildings["historic"] != 0, "historic"] = 1
     historic_buildings = historic_buildings[['geometry', 'historic']]
     historic_buildings['area'] = historic_buildings.geometry.area
        
     return historic_buildings
  
-def cultural_score(buildings_gdf, historical_elements_gdf = pd.DataFrame({'a': []}), historical_score = None, from_OSM = False, ):
+def cultural_score(buildings_gdf, historical_elements_gdf = pd.DataFrame({'a': []}), historical_score = None, from_OSM = False):
     """
     The function computes the "Cultural Landmark Component" based on the number of features listed in historical/cultural landmarks datasets. It can be
     obtained either on the basis of a score given by the data-provider or on the number of features intersecting the buildings object 
     of analysis.
     
     "historical_score" indicates the attribute field containing scores assigned to historical buildings, if existing.
     Alternatively, if the column has been already assigned to the buildings_gdf, one can use OSM historic categorisation (binbary).
@@ -534,16 +539,18 @@
     buildings_gdf: Polygon GeoDataFrame
         The updated buildings GeoDataFrame.
     """  
     buildings_gdf = buildings_gdf.copy()
     buildings_gdf["cult"] = 0
     # using OSM binary value
     if (from_OSM) & ("historic" in buildings_gdf.columns):
-        buildings_gdf["historic"][buildings_gdf["historic"].isnull()] = 0
-        buildings_gdf["historic"][buildings_gdf["historic"] != 0] = 1
+        # Set 'historic' column to 0 where it is currently null
+        buildings_gdf.loc[buildings_gdf["historic"].isnull(), "historic"] = 0
+        # Set 'historic' column to 1 where it is not 0
+        buildings_gdf.loc[buildings_gdf["historic"] != 0, "historic"] = 1
         buildings_gdf["cult"] = buildings_gdf["historic"]
         return buildings_gdf
     
     def _cultural_score_building(building_geometry, historical_elements_gdf, historical_elements_gdf_sindex, score = None):
         """
         Compute the cultural score for a single building based on its intersection with historical elements.
```

### Comparing `cityImage-1.0/cityImage/load.py` & `cityImage-1.10/cityImage/load.py`

 * *Files identical despite different names*

### Comparing `cityImage-1.0/cityImage/plot.py` & `cityImage-1.10/cityImage/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,14 +55,16 @@
         self.black_background = black_background
         self.text_color = "white" if black_background else "black"
         
         rect = self.fig.patch 
         rect.set_facecolor("black" if black_background else "white")      
         if title is not None:
             self.fig.suptitle(title, color = self.text_color, fontsize = self.font_size_primary, fontfamily = 'Times New Roman')
+            
+        self.fig.tight_layout();
                
 class MultiPlot():
     """
     A class for creating multi-plot figures.
     
     Attributes:
     ----------
@@ -106,14 +108,15 @@
         rect.set_facecolor("black" if black_background else "white")   
         self.font_size_primary = fontsize
         self.font_size_secondary = fontsize*0.90
         
         if title is not None:
             self.fig.suptitle(title, color = self.text_color, fontsize = self.font_size_primary, fontfamily = 'Times New Roman', 
                          ha = 'center', va = 'center') 
+        self.fig.tight_layout();
               
 def plot_gdf(gdf, column = None, title = None, black_background = True, figsize = (15,15), scheme = None, bins = None, 
             classes = None, norm = None, cmap = None, color = None, alpha = None, geometry_size = 1.0, 
             geometry_size_column = None, geometry_size_factor = None, legend = False, fontsize = 15, cbar = False, cbar_ticks = 5, 
             cbar_max_symbol = False, cbar_min_max = False, cbar_shrink = 0.75, axes_frame = False, 
             base_map_gdf = pd.DataFrame({"a": []}), base_map_color = None, base_map_alpha = 0.4, base_map_geometry_size = 1.1,  
             base_map_zorder = 0):
```

### Comparing `cityImage-1.0/cityImage/regions.py` & `cityImage-1.10/cityImage/regions.py`

 * *Files identical despite different names*

### Comparing `cityImage-1.0/cityImage/utilities.py` & `cityImage-1.10/cityImage/utilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import pandas as pd
 import numpy as np
 import geopandas as gpd
 import math
 import pyproj
 import osmnx as ox
+import networkx as nx
 
 from typing import List
 from math import sqrt
 from shapely.geometry import LineString, Point, Polygon, MultiPoint, mapping
 from shapely.ops import unary_union, transform, nearest_points, split, linemerge
 from shapely.affinity import scale
 from shapely.geometry.base import BaseGeometry
-from functools import partial
 import pyvista as pv
 pd.set_option("display.precision", 3)
 
 class Error(Exception):
     """Base class for other exceptions"""
 
 class downloadError(Error):
@@ -51,18 +51,18 @@
         The resulting Graph (when downloading_graph) or a GeoDataFrame.
     """    
     download_options = {"distance_from_address", "distance_from_point", "OSMplace", "polygon"}
     if download_method not in download_options:
         raise downloadError('Provide a download method amongst {}'.format(download_options))
 
     download_method_dict = {
-        'distance_from_address': ox.geometries_from_address,
-        'distance_from_point': ox.geometries_from_point,
-        'OSMplace': ox.geometries_from_place,
-        'polygon': ox.geometries_from_polygon
+        'distance_from_address': ox.features_from_address,
+        'distance_from_point': ox.features_from_point,
+        'OSMplace': ox.features_from_place,
+        'polygon': ox.features_from_polygon
         }
     if downloading_graph:
         download_method_dict = {
         'distance_from_address': ox.graph_from_address,
         'distance_from_point': ox.graph_from_point,
         'OSMplace': ox.graph_from_place,
         'polygon': ox.graph_from_polygon
@@ -78,16 +78,17 @@
                 else:
                     geometries_gdf = download_func(place, tags = tags, dist = distance)
             else:
                 if downloading_graph:
                     G = download_func(place, network_type = network_type, simplify = True)
                 else:
                     geometries_gdf = download_func(place, tags = tags) 
-    except ox._errors.EmptyOverpassResponse:
-        # Handle the EmptyOverpassResponse error by returning an empty GeoDataFrame
+                    
+    except ox._errors.InsufficientResponseError:
+        # Handle the InsufficientResponseError error by returning an empty GeoDataFrame
         geometries_gdf = gpd.GeoDataFrame(columns=['id', 'geometry'], geometry='geometry').set_crs('EPSG:4326')
         if downloading_graph:
             G=nx.empty_graph()
     if downloading_graph:
         return G
     return geometries_gdf
     
@@ -305,20 +306,18 @@
     
     Return
     ----------
     envelope_wgs: Polygon
         The resulting envelope.
     """
     envelope = gdf.unary_union.envelope.buffer(100)
-    project = partial(
-        pyproj.transform,
-        pyproj.Proj(gdf.crs), # source coordinate system
-        pyproj.Proj(init='epsg:4326')) # destination coordinate system
-
-    envelope_wgs = transform(project, envelope)
+    
+    # Define a transformer for projecting from the GeoDataFrame's CRS to WGS84
+    transformer = pyproj.Transformer.from_crs(gdf.crs, 'epsg:4326', always_xy=True)
+    envelope_wgs = transform(transformer.transform, envelope)
     return envelope_wgs 
     
 def convex_hull_wgs(gdf):
     """
     Given a GeoDataFrame it derives its convex hull in the WGS coordinate system.
     
     Parameters
@@ -326,21 +325,22 @@
     gdf: GeoDataFrame
         
     Return
     ----------
     convex_hull_wgs: Polygon
         The resulting hexagon.
     """
+    # Compute the convex hull without buffering
     convex_hull = gdf.unary_union.convex_hull
-    project = partial(
-        pyproj.transform,
-        pyproj.Proj(gdf.crs), # source coordinate system
-        pyproj.Proj(init='epsg:4326')) # destination coordinate system
 
-    convex_hull_wgs = transform(project, convex_hull)
+    # Define a transformer for projecting from the GeoDataFrame's CRS to WGS84
+    transformer = pyproj.Transformer.from_crs(gdf.crs, 'epsg:4326', always_xy=True)
+    
+    # Apply the transformation
+    convex_hull_wgs = transform(transformer.transform, convex_hull)
     return convex_hull_wgs      
         
 def rescale_ranges(n, range1, range2):
     """
     Given a value n and the range which it belongs to, the function rescale the value, between a different range.
         
     Parameters
@@ -491,15 +491,35 @@
             gdf = gdf[gdf.geometry.type == 'LineString']
             # explode the MultiLineString geometries into individual LineString geometries
             multi_gdf = multi_gdf.explode(ignore_index=True)
             # append the exploded LineString geometries back to the original GeoDataFrame
             gdf = gdf.append(multi_gdf, ignore_index=True)
 
     return gdf
-    
+ 
+def remove_lists_columns(df):
+    """
+    For each cell in the DataFrame, if the cell contains a list, update it to keep only the first element of the list.
+
+    Parameters
+    ----------
+    df: DataFrame
+        The input DataFrame.
+
+    Returns
+    -------
+    df: DataFrame
+        A DataFrame with the transformation applied to the relevant cells.
+    """
+    df = df.copy()
+    for column in df.columns:
+        df[column] = df[column].apply(lambda x: x[0] if isinstance(x, list) and len(x) > 0 else x)
+        
+    return df
+  
 def polygon_2d_to_3d(building_polygon, base, height):
     """
     Convert a 2D polygon to a 3D polygon. This function takes a 2D polygon (building_polygon) and extrudes it into 3D space, creating a pv.PolyData,
     creating a 3D polygon with a base and a height elevation.
     
     Parameters
     ----------
```

### Comparing `cityImage-1.0/cityImage.egg-info/PKG-INFO` & `cityImage-1.10/cityImage.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,39 @@
 Metadata-Version: 2.1
 Name: cityImage
-Version: 1.0
+Version: 1.10
 Summary: A package for studying urban form and obtaining the computational Image of the City
 Author: Gabriele Filomena
 Author-email: gabriele.filomena@liverpool.ac.uk
 Keywords: urban Form Analysis,Computational Image of the City,Kevin Lynch,cognitive maps
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: osmnx>=1.9.1
+Requires-Dist: python-louvain>=0.16
+Requires-Dist: pyvista>=0.37
+Requires-Dist: mapclassify>=2.5.0
 
 [![CodeFactor](https://www.codefactor.io/repository/github/g-filomena/cityimage/badge)](https://www.codefactor.io/repository/github/g-filomena/cityimage)
 [![Actions Status](https://github.com/g-filomena/cityimage/workflows/tests/badge.svg)](https://github.com//g-filomena/cityimage/actions?query=workflow%3Atests)
 [![codecov](https://codecov.io/gh/g-filomena/cityImage/branch/master/graph/badge.svg)](https://codecov.io/gh/g-filomena/cityImage)
+[![PyPI version](https://badge.fury.io/py/cityImage.svg)](https://badge.fury.io/py/cityImage)
 
 # cityImage
 
 **A tool for analysing urban legibility and extracting The Computational Image of the City**
+For full documentation and examples see [the user manual](https://cityimage-docs.readthedocs.io/en/latest/).
 
 This repository provides a set of functions to extract salient urban features in line with the definitions laid down by Kevin Lynch in [The Image of The City](https://mitpress.mit.edu/books/image-city) using open and freely available geospatial datasets.
+The methods are fully documented in *A Computational approach to The Image of the City* by Filomena, Verstegen, and Manley, published in [Cities](https://doi.org/10.1016/j.cities.2019.01.006).
 
-The tools are written in Python and uses a series of libraries, including [Geopandas](http://geopandas.org), [OSMNx](https://osmnx.readthedocs.io/en/stable/), [PyVista](https://docs.pyvista.org/version/stable/) and related dependencies.
+The tools are written in Python and requires:
 
-The methods are fully documented in *A Computational approach to â€˜The Image of the Cityâ€™* by Filomena, Verstegen, and Manley, published in [Cities](https://doi.org/10.1016/j.cities.2019.01.006).
-The full documentation is available at 
+* [OSMNx](https://osmnx.readthedocs.io/en/stable/).
+* [PyVista](https://docs.pyvista.org/version/stable/).
+* [python-louvain](https://github.com/taynaud/python-louvain).
+* [mapclassify](https://github.com/pysal/mapclassify).
 
-## Introduction
+It is built on [GeoPandas](https://github.com/geopandas/geopandas), [NetworkX](https://github.com/networkx/networkx), and [Shapely](https://github.com/shapely/shapely).
+
+## How to install *cityImage*
+
+    pip install cityImage
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cityImage-1.0/cityImage.egg-info/SOURCES.txt` & `cityImage-1.10/cityImage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cityImage-1.0/setup.py` & `cityImage-1.10/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
-with open("README.md", "r") as readme_file: 
+with open("README.md", "r", encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
-requirements = ["osmnx>=1.3", "python-louvain>=0.16", "pyvista>=0.37"]
+requirements = ["osmnx>=1.9.1", "python-louvain>=0.16", "pyvista>=0.37", "mapclassify>=2.5.0"]
     
 setup(
     name="cityImage",
     description="A package for studying urban form and obtaining the computational Image of the City",
     long_description = readme,
     long_description_content_type="text/markdown",
     packages=find_packages(),
-    version="1.0",
+    version="1.10",
     author="Gabriele Filomena",
     author_email="gabriele.filomena@liverpool.ac.uk",
     install_requires=requirements,
     keywords=["urban Form Analysis","Computational Image of the City", "Kevin Lynch", "cognitive maps"],
     )
```

### Comparing `cityImage-1.0/tests/test_cityImage.py` & `cityImage-1.10/tests/test_cityImage.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # define queries to use throughout tests
 
 place = "Susa, Italy"
 download_method = 'OSMplace'
 epsg_york = 2019
 epsg_susa = 3003
 OSMPolygon = 'Susa (44287)'
-address = 'Susa, via Roma 1'
+address = 'Susa, Corso Francia'
 distance = 1500
 location = (45.1383, 7.0509)
 
 buildings_gdf = None
 nodes_gdf, edges_gdf = None, None
 nodes_gdf_y, edges_gdf_y = None, None
 barriers_gdf = None
```

