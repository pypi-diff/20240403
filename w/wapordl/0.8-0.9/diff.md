# Comparing `tmp/wapordl-0.8.tar.gz` & `tmp/wapordl-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wapordl-0.8.tar", last modified: Tue Jan 23 16:10:01 2024, max compression
+gzip compressed data, was "wapordl-0.9.tar", last modified: Fri Mar 22 10:28:41 2024, max compression
```

## Comparing `wapordl-0.8.tar` & `wapordl-0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-01-23 16:10:01.461091 wapordl-0.8/
--rw-r--r--   0 hmcoerver   (501) staff       (20)    11323 2022-06-23 13:36:53.000000 wapordl-0.8/LICENSE
--rw-r--r--   0 hmcoerver   (501) staff       (20)      245 2024-01-23 16:10:01.460895 wapordl-0.8/PKG-INFO
--rw-r--r--   0 hmcoerver   (501) staff       (20)     4287 2024-01-23 16:02:42.000000 wapordl-0.8/README.md
--rw-r--r--   0 hmcoerver   (501) staff       (20)       38 2024-01-23 16:10:01.461141 wapordl-0.8/setup.cfg
--rw-r--r--   0 hmcoerver   (501) staff       (20)      381 2024-01-23 15:37:15.000000 wapordl-0.8/setup.py
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-01-23 16:10:01.459869 wapordl-0.8/wapordl/
--rw-r--r--   0 hmcoerver   (501) staff       (20)      130 2024-01-23 15:37:26.000000 wapordl-0.8/wapordl/__init__.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    31503 2024-01-23 16:05:33.000000 wapordl-0.8/wapordl/main.py
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-01-23 16:10:01.460686 wapordl-0.8/wapordl.egg-info/
--rw-r--r--   0 hmcoerver   (501) staff       (20)      245 2024-01-23 16:10:01.000000 wapordl-0.8/wapordl.egg-info/PKG-INFO
--rw-r--r--   0 hmcoerver   (501) staff       (20)      216 2024-01-23 16:10:01.000000 wapordl-0.8/wapordl.egg-info/SOURCES.txt
--rw-r--r--   0 hmcoerver   (501) staff       (20)        1 2024-01-23 16:10:01.000000 wapordl-0.8/wapordl.egg-info/dependency_links.txt
--rw-r--r--   0 hmcoerver   (501) staff       (20)       61 2024-01-23 16:10:01.000000 wapordl-0.8/wapordl.egg-info/requires.txt
--rw-r--r--   0 hmcoerver   (501) staff       (20)        8 2024-01-23 16:10:01.000000 wapordl-0.8/wapordl.egg-info/top_level.txt
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-03-22 10:28:41.021870 wapordl-0.9/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    11323 2022-06-23 13:36:53.000000 wapordl-0.9/LICENSE
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      245 2024-03-22 10:28:41.021621 wapordl-0.9/PKG-INFO
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     4261 2024-02-22 09:44:48.000000 wapordl-0.9/README.md
+-rw-r--r--   0 hmcoerver   (501) staff       (20)       38 2024-03-22 10:28:41.021917 wapordl-0.9/setup.cfg
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      381 2024-03-22 10:22:00.000000 wapordl-0.9/setup.py
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-03-22 10:28:41.020564 wapordl-0.9/wapordl/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      130 2024-03-22 10:22:05.000000 wapordl-0.9/wapordl/__init__.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    35786 2024-03-22 10:21:36.000000 wapordl-0.9/wapordl/main.py
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2024-03-22 10:28:41.021421 wapordl-0.9/wapordl.egg-info/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      245 2024-03-22 10:28:40.000000 wapordl-0.9/wapordl.egg-info/PKG-INFO
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      216 2024-03-22 10:28:41.000000 wapordl-0.9/wapordl.egg-info/SOURCES.txt
+-rw-r--r--   0 hmcoerver   (501) staff       (20)        1 2024-03-22 10:28:40.000000 wapordl-0.9/wapordl.egg-info/dependency_links.txt
+-rw-r--r--   0 hmcoerver   (501) staff       (20)       61 2024-03-22 10:28:40.000000 wapordl-0.9/wapordl.egg-info/requires.txt
+-rw-r--r--   0 hmcoerver   (501) staff       (20)        8 2024-03-22 10:28:40.000000 wapordl-0.9/wapordl.egg-info/top_level.txt
```

### Comparing `wapordl-0.8/LICENSE` & `wapordl-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wapordl-0.8/README.md` & `wapordl-0.9/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,116 +1,128 @@
 ![downloads](https://img.shields.io/pypi/dw/wapordl) [![version](https://img.shields.io/pypi/v/wapordl)](https://anaconda.org/conda-forge/wapordl)
 
 # WaPORDL
 
-This package allows users to download data from the WaPOR3 dataset as spatially aggregated timeseries or as spatial data clipped to a bounding-box or shapefile.
+Download data from the WaPOR3 dataset as spatially aggregated timeseries or as spatial data clipped to a bounding-box or shapefile.
 
 ## Installation
 
 ### Conda (recommended)
 `conda install -c conda-forge wapordl`
 
 ### Pip (make sure GDAL is already installed)
 `pip install wapordl`
 
 ## Usage
 
 To download a timeseries for a certain region:
 
-    from wapordl import wapor_ts
+```python
+from wapordl import wapor_ts
 
-    region = "path/to/some/shape.geojson"
-    variable = "L2-AETI-D"
-    period = ["2021-01-01", "2021-07-01"]
-    overview = 3 # set to "NONE" to use native resolution data.
-
-    df = wapor_ts(region, variable, period, overview)
-    
-    df
-
-    >>>     minimum  maximum    mean start_date   end_date number_of_days
-    >>> 0       0.0      7.3  0.5962 2021-01-01 2021-01-10        10 days
-    >>> 1       0.0      6.7  0.3923 2021-01-11 2021-01-20        10 days
-    >>> 2       0.0      6.7  0.3158 2021-01-21 2021-01-31        11 days
-    >>> ...
-    >>> 16      0.0      4.8  0.3192 2021-06-11 2021-06-20        10 days
-    >>> 17      0.0      4.9  0.4197 2021-06-21 2021-06-30        10 days
-    >>> 18      0.0      5.0  0.5727 2021-07-01 2021-07-10        10 days
-
-    df.attrs
-
-    >>> {'long_name': 'Actual EvapoTranspiration and Interception',
-    >>> 'units': 'mm/day',
-    >>> 'overview': 3}
+region = "path/to/some/shape.geojson"
+variable = "L2-AETI-D"
+period = ["2021-01-01", "2021-07-01"]
+overview = 3 # set to "NONE" to use native resolution data.
+
+df = wapor_ts(region, variable, period, overview)
+
+df
+
+>>>     minimum  maximum    mean start_date   end_date number_of_days
+>>> 0       0.0      7.3  0.5962 2021-01-01 2021-01-10        10 days
+>>> 1       0.0      6.7  0.3923 2021-01-11 2021-01-20        10 days
+>>> 2       0.0      6.7  0.3158 2021-01-21 2021-01-31        11 days
+>>> ...
+>>> 16      0.0      4.8  0.3192 2021-06-11 2021-06-20        10 days
+>>> 17      0.0      4.9  0.4197 2021-06-21 2021-06-30        10 days
+>>> 18      0.0      5.0  0.5727 2021-07-01 2021-07-10        10 days
+
+df.attrs
+
+>>> {'long_name': 'Actual EvapoTranspiration and Interception',
+>>> 'units': 'mm/day',
+>>> 'overview': 3}
+```
 
 To download a timerseries and convert its unit provide the `unit_conversion` keyword:
 
-    unit_conversion = "dekad" # or "day", "month", "year", "none".
+```python
+unit = "dekad" # or choose "day", "month", "year", "none" (default).
 
-    df = wapor_ts(region, variable, period, overview, unit_conversion = unit_conversion)
-    
-    df
+df = wapor_ts(region, variable, period, overview, unit_conversion = unit)
 
-    >>>     minimum  maximum    mean start_date   end_date number_of_days
-    >>> 0       0.0     73.0  5.9617 2021-01-01 2021-01-10        10 days
-    >>> 1       0.0     67.0  3.9235 2021-01-11 2021-01-20        10 days
-    >>> 2       0.0     73.7  3.4740 2021-01-21 2021-01-31        11 days
-    >>> ...
-    >>> 16      0.0     48.0  3.1919 2021-06-11 2021-06-20        10 days
-    >>> 17      0.0     49.0  4.1972 2021-06-21 2021-06-30        10 days
-    >>> 18      0.0     50.0  5.7273 2021-07-01 2021-07-10        10 days
-
-    df.attrs
-
-    >>> {'long_name': 'Actual EvapoTranspiration and Interception',
-    >>> 'units': 'mm/dekad',
-    >>> 'overview': 3,
-    >>> 'original_units': 'mm/day'}
+df
+
+>>>     minimum  maximum    mean start_date   end_date number_of_days
+>>> 0       0.0     73.0  5.9617 2021-01-01 2021-01-10        10 days
+>>> 1       0.0     67.0  3.9235 2021-01-11 2021-01-20        10 days
+>>> 2       0.0     73.7  3.4740 2021-01-21 2021-01-31        11 days
+>>> ...
+>>> 16      0.0     48.0  3.1919 2021-06-11 2021-06-20        10 days
+>>> 17      0.0     49.0  4.1972 2021-06-21 2021-06-30        10 days
+>>> 18      0.0     50.0  5.7273 2021-07-01 2021-07-10        10 days
+
+df.attrs
+
+>>> {'long_name': 'Actual EvapoTranspiration and Interception',
+>>> 'units': 'mm/dekad',
+>>> 'overview': 3,
+>>> 'original_units': 'mm/day'}
+```
 
 To download a geotiff for a certain region and period of time:
 
-    from wapordl import wapor_map
+```python
+from wapordl import wapor_map
 
-    region = "path/to/some/my_region.geojson"
-    folder = "path/to/some/output/folder"
-    variable = "L2-AETI-D"
-    period = ["2021-01-01", "2021-07-01"]
+region = "path/to/some/my_region.geojson"
+folder = "path/to/some/output/folder"
+variable = "L2-AETI-D"
+period = ["2021-01-01", "2021-07-01"]
 
-    fp = wapor_map(region, variable, period, folder)
+fp = wapor_map(region, variable, period, folder)
 
-    fp
+fp
 
-    >>> 'path/to/some/output/folder/my_region_L2-AETI-D_NONE_none.tif'
+>>> 'path/to/some/output/folder/my_region_L2-AETI-D_NONE_none.tif'
+```
 
 To download a timeseries and a netcdf for a bounding-box:
 
-    region = [25, -17, 26, -16]
-    folder = "path/to/some/output/folder"
-    variable = "L2-AETI-D"
-    period = ["2021-01-01", "2021-07-01"]
-    overview = 3
-
-    df = wapor_ts(region, variable, period, overview)
-    fp = wapor_map(region, variable, period, folder, extension = ".nc")
+```python
+region = [35.75, 33.70, 35.82, 33.75] # [xmin, ymin, xmax, ymax]
+folder = "path/to/some/output/folder"
+variable = "L3-AETI-D"
+period = ["2021-01-01", "2021-07-01"]
+overview = 3
+
+df = wapor_ts(region, variable, period, overview)
+fp = wapor_map(region, variable, period, folder, extension = ".nc")
+```
 
 When working with level-3 data, an entire L3 region can be downloaded by specifying a three letter region code:
     
-    region = "BKA"
-    folder = "path/to/some/output/folder"
-    variable = "L3-T-D"
-    period = ["2021-01-01", "2021-07-01"]
-    overview = 3
-    unit_conversion = "year"
-
-    df = wapor_ts(region, variable, period, overview)
-    fp = wapor_map(region, variable, period, folder, unit_conversion = unit_conversion)
+```python
+region = "BKA"
+folder = "path/to/some/output/folder"
+variable = "L3-T-D"
+period = ["2021-01-01", "2021-07-01"]
+overview = 3
+
+df = wapor_ts(region, variable, period, overview)
+fp = wapor_map(region, variable, period, folder, unit_conversion = "year")
+```
 
 ## Upcoming
 
 - Automatic overview selection based on the size of the shape.
+- Support for variables with daily resolution (i.e. `L1-PCP-E` and `L1-RET-E`).
+- Easily download a lower level variable for a level-3 region.
+- Support for agERA5 variables.
 - ~~Determine `l3_region` automatically from `region`.~~ ✅
 - ~~Select unit of output.~~ ✅
 - ~~Download a region from a bounding-box (i.e. without a shape).~~ ✅
 - ~~A progress bar.~~ ✅
 - ~~A warning if the given shape doesnt cover an area for which data is available.~~ ✅
 - ~~Support for other output formats besides geotiff (e.g. netcdf).~~ ✅
 - ~~Installation with conda.~~ ✅
```

### Comparing `wapordl-0.8/wapordl/main.py` & `wapordl-0.9/wapordl/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import os
 import requests
 import logging
 import shapely
 import numpy as np
 import pandas as pd
 from tqdm import tqdm
-from osgeo import gdal
+from osgeo import gdal, gdalconst
 from osgeo_utils import gdal_calc
-from osgeo import gdalconst
 from string import ascii_lowercase, ascii_uppercase
 gdal.UseExceptions()
 logging.basicConfig(encoding='utf-8', level=logging.INFO, format='%(levelname)s: %(message)s')
 
 L3_BBS = {
     'AWA': [[39.1751869, 8.9148245], [39.1749088, 8.3098793], [40.0254231, 8.3085969], [40.0270531, 8.9134473], [39.1751869, 8.9148245]], 
     'BKA': [[35.7339813, 34.0450172], [35.7204902, 33.6205171], [36.2189392, 33.6085397], [36.2348925, 34.0328476], [35.7339813, 34.0450172]], 
@@ -31,14 +30,20 @@
     'MIT': [[2.3861237, 36.804671], [2.3893986, 36.3901832], [3.403877, 36.3910611], [3.4060432, 36.8055622], [2.3861237, 36.804671]], 
     'MUV': [[30.2315244, -1.0474462], [30.2323749, -1.6835342], [30.474523, -1.6831148], [30.4736091, -1.0471853], [30.2315244, -1.0474462]], 
     'ODN': [[-6.2554174, 14.5579879], [-6.2650165, 13.7577987], [-5.8657445, 13.7530413], [-5.8547493, 14.5529423], [-6.2554174, 14.5579879]], 
     'PAL': [[35.3712698, 32.1997283], [35.359621, 31.7457763], [35.5587674, 31.7419309], [35.5713968, 32.1958148], [35.3712698, 32.1997283]], 
     'SAN': [[43.9733487, 15.607452], [43.9752772, 15.2142363], [44.4893856, 15.2159917], [44.4884245, 15.609255], [43.9733487, 15.607452]], 
     'SED': [[-16.2610895, 16.4920046], [-16.2593842, 16.2262901], [-15.8685096, 16.22825], [-15.8696858, 16.4939983], [-16.2610895, 16.4920046]], 
     'YAN': [[29.9186281, -1.7554126], [29.9189336, -1.9422648], [30.0389016, -1.9420519], [30.0385836, -1.7552203], [29.9186281, -1.7554126]],
+    'ENO': [[29.0486593, 31.5729461], [29.2216818, 26.984181], [33.0969909, 27.0348598], [33.1014462, 31.6340632], [29.0486593, 31.5729461]],
+    'KMW': [[37.1712454, -0.5521456], [37.1711311, -0.847298], [37.5827814, -0.8474716], [37.58287, -0.5522587], [37.1712454, -0.5521456]],
+    'KTB': [[39.8040688, -1.0763414], [39.8042047, -1.5083961], [40.0334158, -1.5082987], [40.0332412, -1.0762719], [39.8040688, -1.0763414]],
+    'LAK': [[30.5461141, -1.8405081], [30.5456327, -2.1639182], [30.8439607, -2.1643744], [30.8443837, -1.8408961], [30.5461141, -1.8405081]],
+    'LOT': [[13.5784136, 32.4380383], [13.5814622, 32.2428769], [13.7011675, 32.2441643], [13.698376, 32.4393353], [13.5784136, 32.4380383]],
+    'MBL': [[32.8061235, -24.386931], [32.8049677, -25.1294871], [33.7920054, -25.1274992], [33.7873122, -24.3850094], [32.8061235, -24.386931]],
     }
 
 L2_BB = """
 {
 "type": "FeatureCollection",
 "name": "L2_BB",
 "crs": { "type": "name", "properties": { "name": "urn:ogc:def:crs:OGC:1.3:CRS84" } },
@@ -89,65 +94,120 @@
             output.append(data)
     if isinstance(info, list):
         output = sorted(output)
     return output
 
 def date_func(url, tres):
     if tres == "D":
+        # if "AGERA5" in url:
+        #     year_acc_dekad = os.path.split(url)[-1].split("_")[-1].split(".")[0]
+        #     year = year_acc_dekad[:4]
+        #     acc_dekad = int(year_acc_dekad[-2:])
+        #     month = str((acc_dekad - 1) // 3 + 1).zfill(2)
+        #     dekad = str((acc_dekad - 1) % 3 + 1)
+        # else:
         year, month, dekad = os.path.split(url)[-1].split(".")[-2].split("-")
-        start_day = {'D1': '01', 'D2': '11', 'D3': '21'}[dekad]
+        start_day = {'D1': '01', 'D2': '11', 'D3': '21', '1': '01', '2': '11', '3': '21'}[dekad]
         start_date = f"{year}-{month}-{start_day}"
-        end_day = {'D1': '10', 'D2': '20', 'D3': pd.Timestamp(start_date).daysinmonth}[dekad]
+        end_day = {'D1': '10', 'D2': '20', 'D3': pd.Timestamp(start_date).daysinmonth, '1': '10', '2': '20', '3': pd.Timestamp(start_date).daysinmonth}[dekad]
         end_date = f"{year}-{month}-{end_day}"
     elif tres == "M":
         year, month = os.path.split(url)[-1].split(".")[-2].split("-")
         start_date = f"{year}-{month}-01"
         end_date = f"{year}-{month}-{pd.Timestamp(start_date).days_in_month}"
     elif tres == "A":
         year = os.path.split(url)[-1].split(".")[-2]
         start_date = f"{year}-01-01"
         end_date = f"{year}-12-31"
+    elif tres == "E":
+        year, month, start_day = os.path.split(url)[-1].split(".")[-2].split("-")
+        start_date = end_date = f"{year}-{month}-{start_day}"
     else:
         raise ValueError("Invalid temporal resolution.") # NOTE: TESTED
     number_of_days = (pd.Timestamp(end_date) - pd.Timestamp(start_date) + pd.Timedelta(1, "D")).days
     return {"start_date": start_date, "end_date": end_date, "number_of_days": number_of_days}
 
 def collect_metadata(variable):
+
+    # if variable == "L1-ET0-D":
+    #     return {"long_name": "Reference Evapotranspiration", "units": "mm/dekad", "source": "FAO56 with agERA5"}
+    
     if "L1" in variable:
         base_url = f"https://data.apps.fao.org/gismgr/api/v2/catalog/workspaces/WAPOR-3/mapsets"
     elif "L2" in variable:
         base_url = f"https://data.apps.fao.org/gismgr/api/v2/catalog/workspaces/WAPOR-3/mapsets"
     elif "L3" in variable:
         base_url = f"https://data.apps.fao.org/gismgr/api/v2/catalog/workspaces/WAPOR-3/mosaicsets"
     else:
         raise ValueError(f"Invalid variable name {variable}.") # NOTE: TESTED
     info = ["code", "measureCaption", "measureUnit"]
     var_codes = {x[0]: {"long_name": x[1], "units": x[2]} for x in collect_responses(base_url, info = info)}
     return var_codes[variable]
 
+def make_dekad_dates(period):
+    period_ = [pd.Timestamp(x) for x in period]
+
+    syear = period_[0].year
+    smonth = period_[0].month
+    eyear = period_[1].year
+    emonth = period_[1].month
+
+    x1 = pd.date_range(f"{syear}-{smonth}-01", f"{eyear}-{emonth}-01", freq = "MS")
+    x2 = x1 + pd.Timedelta("10 days")
+    x3 = x1 + pd.Timedelta("20 days")
+    x = np.sort(np.concatenate((x1, x2, x3)))
+
+    x_filtered = [pd.Timestamp(x_) for x_ in x if x_ >= period_[0] and x_ < period_[1]]
+    return x_filtered
+
+def generate_urls_agERA5(variable, period = None):
+    agera_vars = [
+            "AGERA5_ET0"
+            "AGERA5_ET0_D"
+            "AGERA5_ET0_M"
+            "AGERA5_ET0_A"
+            "AGERA5_TMIN"
+            "AGERA5_TMAX"
+            "AGERA5_SRF"
+            "AGERA5_WS"
+            "AGERA5_RH06"
+            "AGERA5_RH09"
+            "AGERA5_RH12"
+            "AGERA5_RH15"
+            "AGERA5_RH18"
+            "AGERA5_PF"
+            "AGERA5_PF_D"
+            "AGERA5_PF_M"
+            "AGERA5_PF_A"
+            ]
+    list_url = "https://data.apps.fao.org/static/data/index.html?prefix=static%2Fdata%2Fc3s%2FAGERA5_ET0"
+    base_url = "https://data.apps.fao.org/static/data/c3s/AGERA5_ET0_D/AGERA5_ET0_{year}D{acc_dekad:>02}.tif"
+    x_filtered = make_dekad_dates(period)
+    urls = [base_url.format(year = x.year, acc_dekad = (x.month - 1)*3 + {1: 1, 11: 2, 21: 3}[x.day]) for x in x_filtered]
+    return tuple(sorted(urls))
+
 def generate_urls_v3(variable, l3_region = None, period = None):
     
     level, _, tres = variable.split("-")
 
     if (level == "L1") or (level == "L2"):
         base_url = f"https://data.apps.fao.org/gismgr/api/v2/catalog/workspaces/WAPOR-3/mapsets"
     elif level == "L3":
         base_url = f"https://data.apps.fao.org/gismgr/api/v2/catalog/workspaces/WAPOR-3/mosaicsets"
     else:
         raise ValueError(f"Invalid level {level}.") # NOTE: TESTED
-    
+
     mapset_url = f"{base_url}/{variable}/rasters?filter="
     if not isinstance(l3_region, type(None)):
         mapset_url += f"code:CONTAINS:{l3_region};"
     if not isinstance(period, type(None)):
-        tres_translator = {"D": "dekad", "M": "month", "A": "year"}
-        mapset_url += f"{tres_translator[tres]}:OVERLAPS:{period[0]}:{period[1]};"
-    
+        mapset_url += f"time:OVERLAPS:{period[0]}:{period[1]};"
+
     urls = [x[0] for x in collect_responses(mapset_url, info = ["downloadUrl"])]
-    
+
     return tuple(sorted(urls))
 
 def __make_band_names__(length):
     letters = [x for x in ascii_lowercase + ascii_uppercase]
     i = 2
     while len(letters) < length:
         for letter in letters[:52]:
@@ -171,15 +231,15 @@
         number_of_days = md.get("number_of_days", "unknown")
         days_in_month = pd.Timestamp(md.get("start_date", "nat")).daysinmonth
         source_unit = md.get("units", "unknown")
         source_unit_split = source_unit.split("/")
         source_unit_q = "/".join(source_unit_split[:-1])
         source_unit_time = source_unit_split[-1]
         if any([
-                source_unit_time not in ["day", "month", "year"],
+                source_unit_time not in ["day", "month", "year", "dekad"],
                 number_of_days == "unknown",
                 source_unit == "unknown",
                 pd.isnull(days_in_month)
             ]):
             calc.append(f"{letter}.astype(numpy.float64)")
             md["units"] = source_unit
             md["units_conversion_factor"] = "N/A"
@@ -187,14 +247,18 @@
             should_convert.append(False)
         else:
             conversion = {
                 ("day", "day"): 1,
                 ("day", "dekad"): number_of_days,
                 ("day", "month"): days_in_month,
                 ("day", "year"): 365,
+                ("dekad", "day"): 1/number_of_days,
+                ("dekad", "month"): 3,
+                ("dekad", "year"): 36,
+                ("dekad", "dekad"): 1,
                 ("month", "day"): 1/days_in_month,
                 ("month", "dekad"): 1/3,
                 ("month", "month"): 1,
                 ("month", "year"): 12,
                 ("year", "dekad"): 1/36,
                 ("year", "day"): 1/365,
                 ("year", "month"): 1/12,
@@ -260,15 +324,16 @@
         raise ValueError(f"Please use one of {list(valid_ext.keys())} as extension for `out_fn`, not {out_ext}") # NOTE: TESTED
     vrt_fn = out_fn.replace(out_ext, ".vrt")
 
     ## Build VRT with all the required data.
     vrt_options_ = gdal.BuildVRTOptions(
         **vrt_options
     )
-    vrt = gdal.BuildVRT(vrt_fn, ["/vsicurl/" + x[1] for x in urls], options = vrt_options_)
+    prepend = {False: "/vsicurl/", True: "/vsigzip//vsicurl/"}
+    vrt = gdal.BuildVRT(vrt_fn, [prepend[".gz" in x[1]] + x[1] for x in urls], options = vrt_options_)
     vrt.FlushCache()
 
     n_urls = len(urls)
 
     # Create waitbar.
     waitbar = tqdm(desc = f"Downloading {n_urls} COGs", leave = False, total = 100, bar_format='{l_bar}{bar}|')
     # Define callback function for waitbar progress.
@@ -334,26 +399,45 @@
         Folder to store output files, by default None
 
     Returns
     -------
     str, pd.Dataframe
         If `req_stats` is not None, returns a pd.Dataframe. Otherwise a path to file is returned.
     """
+    global L3_BBS
+
     ## Retrieve info from variable name.
     level, var_code, tres = variable.split("-")
 
     ## Check if region is valid.
-    if all([isinstance(region, str), 
-            # not os.path.isfile(region),
-            region in list(L3_BBS.keys()), 
-            len(region) == 3]):
-        l3_region = region[:]
-        region = None
-        region_code = l3_region[:]
-        region_shape = None
+    if all([isinstance(region, str), len(region) == 3]):
+        
+        if not region == region.upper():
+            raise ValueError(f"Invalid region code `{region}`, region codes have three capitalized letters.")
+        
+        if region not in list(L3_BBS.keys()):
+            logging.info(f"Searching bounding-box for `{region}`.")
+            bb = l3_bounding_boxes(l3_region = region)
+            if len(bb) == 0:
+                raise ValueError(f"Unkown L3 region `{region}`.")
+            else:
+                logging.info(f"Bounding-box found for `{region}`.")
+                L3_BBS = {**L3_BBS, **bb}
+
+        if level == "L3":
+            l3_region = region[:] # three letter code to filter L3 datasets in GISMGR2.
+            region = None   # used for clipping, can be None, list(bb) or path/to/file.geojson.
+            region_code = l3_region[:] # string to name the region in filenames etc.
+            region_shape = None # polygon used to check if there is data for the region.
+        else:
+            l3_region = None
+            region_shape = shapely.Polygon(np.array(L3_BBS[region]))
+            region_code = region[:]
+            region = list(region_shape.bounds)
+
     elif isinstance(region, str):
         if not os.path.isfile(region) or os.path.splitext(region)[-1] != ".geojson":
             raise ValueError(f"Geojson file not found.") # NOTE: TESTED
         else:
             region_code = os.path.split(region)[-1].replace(".geojson", "")
             region_shape = shapely.from_geojson(open(region,'r').read())
         l3_region = None
@@ -387,30 +471,24 @@
     urls = generate_urls_v3(variable, l3_region = l3_region, period = period)
 
     if len(urls) == 0:
         raise ValueError("No files found for selected region, variable and period.")  # NOTE: TESTED
 
     ## Determine date for each url.
     md = collect_metadata(variable)
-    ## NOTE This should be corrected in the GISMGR2.0 API instead of here:
-    if all([
-        "NPP" in var_code, 
-        "year" not in md["units"], 
-        "month" not in md["units"], 
-        "day" not in md["units"]
-        ]):
-        md["units"] += {"D": "/day", "M": "/month", "A": "/year"}[tres]
     md["overview"] = overview
     md_urls = [({**date_func(url, tres), **md}, url) for url in urls]
 
     logging.info(f"Found {len(md_urls)} files for {variable}.")
 
     ## Determine required output resolution.
     # NOTE maybe move this to external function (assumes info the same for all urls)
-    info = gdal.Info("/vsicurl/" + md_urls[0][1], format = "json")
+    info_url = md_urls[0][1]
+    info_url = {False: "/vsicurl/", True: "/vsigzip//vsicurl/"}[".gz" in info_url] + info_url
+    info = gdal.Info(info_url, format = "json")
     overview_ = -1 if overview == "NONE" else overview
     xres, yres = info["geoTransform"][1::4]
     warp_kwargs = {
         "xRes": abs(xres) * 2**(overview_ + 1),
         "yRes": abs(yres) * 2**(overview_ + 1),
     }
 
@@ -424,22 +502,23 @@
 
     ## Check if region overlaps with datasets bounding-box.
     if not isinstance(region_shape, type(None)):
         if level == "L2":
             data_bb = shapely.from_geojson(L2_BB)
         else:
             data_bb = shapely.Polygon(np.array(info["wgs84Extent"]["coordinates"])[0])
+        
         if not data_bb.intersects(region_shape):
             info_lbl1 = region_code if region_code != "bb" else str(region)
             info_lbl2 = variable if isinstance(l3_region, type(None)) else f"{variable}.{l3_region}"
             raise ValueError(f"Selected region ({info_lbl1}) has no overlap with the datasets ({info_lbl2}) bounding-box.")
 
     ## Get scale and offset factor.
-    scale = info["bands"][0]["scale"]
-    offset = info["bands"][0]["offset"]
+    scale = info["bands"][0].get("scale", 1)
+    offset = info["bands"][0].get("offset", 0)
 
     ## Check offset factor.
     if offset != 0:
         logging.warning("Offset factor is not zero, statistics might be wrong.")
 
     if folder:
         if not os.path.isdir(folder):
@@ -544,31 +623,44 @@
     return df
 
 def __l3_codes__(variable = "L3-T-A"):
     public_urls = generate_urls_v3(variable, period = ["2019-01-01", "2019-02-01"])
     valids = np.unique([os.path.split(x)[-1].split(".")[2] for x in public_urls])
     return valids.tolist()
 
-def __l3_bounding_boxes__(variable = "L3-T-A"):
-    urls = generate_urls_v3(variable, period = ["2019-01-01", "2019-02-01"])
+def l3_bounding_boxes(variable = "L3-T-A", l3_region = None):
+    urls = generate_urls_v3(variable, l3_region = l3_region, period = ["2019-01-01", "2019-02-01"])
     l3_bbs = {}
     for region_code, url in zip([os.path.split(x)[-1].split(".")[-3] for x in urls], urls):
         info = gdal.Info("/vsicurl/" + url, format = "json")
         bb = info["wgs84Extent"]["coordinates"][0]
         l3_bbs[region_code] = bb
     return l3_bbs
 
 if __name__ == "__main__":
 
-    region = "/Users/hmcoerver/Library/Mobile Documents/com~apple~CloudDocs/GitHub/wapordl/wapordl/test_data/1237500.geojson"
-    variable = "L1-AETI-D"
-    period = ["2021-01-12", "2021-01-28"]
-    overview = 3
-    unit_conversion = "none"
-    req_stats = ["minimum", "maximum", "mean"]
-    extension = ".nc"
-    unit_conversion = "dekad"
+    # region = r"/Users/hmcoerver/Library/Mobile Documents/com~apple~CloudDocs/GitHub/wapordl/wapordl/test_data/1237500.geojson"
+    # variable = "L1-AETI-D"
+    # period = ["2021-01-12", "2021-01-28"]
+    # overview = 3
+    # unit_conversion = "none"
+    # req_stats = ["minimum", "maximum", "mean"]
+    # extension = ".nc"
+    # unit_conversion = "dekad"
     folder = r"/Users/hmcoerver/Local/test"
 
+    region = "MBL"
+    
+    variable = "L1-PCP-E"
+    # variable = "L3-T-A"
+
+    period = ["2023-01-01", "2023-01-04"]
+    unit_conversion = "none"
+    overview = "NONE"
+    extension = ".tif"
+    req_stats = None
+
+    # out = l3_bounding_boxes(variable = "L3-T-A")
+
     map1 = wapor_map(region, variable, period, folder, unit_conversion=unit_conversion)
-    map2 = wapor_map(region, variable, period, folder, unit_conversion=unit_conversion, extension=extension)
+    # map2 = wapor_map(region, variable, period, folder, unit_conversion=unit_conversion, extension=extension)
```

