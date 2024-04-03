# Comparing `tmp/plateaukit-0.9.1.tar.gz` & `tmp/plateaukit-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plateaukit-0.9.1.tar", max compression
+gzip compressed data, was "plateaukit-0.9.2.tar", max compression
```

## Comparing `plateaukit-0.9.1.tar` & `plateaukit-0.9.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1070 2023-12-17 19:01:10.683916 plateaukit-0.9.1/LICENSE.txt
--rw-r--r--   0        0        0     1759 2023-12-16 09:59:59.911832 plateaukit-0.9.1/README.md
--rw-r--r--   0        0        0      175 2023-12-05 11:34:45.256449 plateaukit-0.9.1/plateaukit/__init__.py
--rw-r--r--   0        0        0     3746 2023-12-16 12:18:11.976468 plateaukit-0.9.1/plateaukit/area.py
--rw-r--r--   0        0        0    10835 2024-02-24 05:56:46.533532 plateaukit-0.9.1/plateaukit/cli.py
--rw-r--r--   0        0        0     4349 2023-12-11 09:09:27.788234 plateaukit-0.9.1/plateaukit/config.py
--rw-r--r--   0        0        0     1169 2023-12-06 13:11:13.146014 plateaukit-0.9.1/plateaukit/constants.py
--rw-r--r--   0        0        0     9187 2023-12-17 15:05:22.989564 plateaukit-0.9.1/plateaukit/dataset.py
--rw-r--r--   0        0        0      176 2023-08-05 20:23:37.132711 plateaukit-0.9.1/plateaukit/db.py
--rw-r--r--   0        0        0       28 2023-08-05 20:23:37.133049 plateaukit-0.9.1/plateaukit/download/__init__.py
--rw-r--r--   0        0        0     3256 2024-02-23 18:10:36.000645 plateaukit-0.9.1/plateaukit/download/downloader.py
--rw-r--r--   0        0        0    46890 2023-12-03 20:05:55.280726 plateaukit-0.9.1/plateaukit/download/list.py
--rw-r--r--   0        0        0       40 2023-12-07 10:09:42.824801 plateaukit-0.9.1/plateaukit/extractors/__init__.py
--rw-r--r--   0        0        0      814 2023-12-17 15:02:39.203770 plateaukit-0.9.1/plateaukit/extractors/utils.py
--rw-r--r--   0        0        0      142 2023-12-05 08:44:59.056683 plateaukit-0.9.1/plateaukit/generators/__init__.py
--rw-r--r--   0        0        0     1471 2023-12-04 15:14:53.880047 plateaukit-0.9.1/plateaukit/generators/cityjson.py
--rw-r--r--   0        0        0       52 2023-12-12 12:18:37.379655 plateaukit-0.9.1/plateaukit/generators/geojson/__init__.py
--rw-r--r--   0        0        0     5943 2023-12-17 14:55:36.018621 plateaukit-0.9.1/plateaukit/generators/geojson/_parallel.py
--rw-r--r--   0        0        0     2806 2023-12-16 09:54:32.759576 plateaukit-0.9.1/plateaukit/generators/geojson/_serial.py
--rw-r--r--   0        0        0     3132 2023-12-12 13:05:56.954478 plateaukit-0.9.1/plateaukit/generators/geojson/_single.py
--rw-r--r--   0        0        0     2016 2023-08-05 20:23:37.136162 plateaukit-0.9.1/plateaukit/generators/quantized_mesh.py
--rw-r--r--   0        0        0    15554 2023-12-17 15:04:04.292187 plateaukit-0.9.1/plateaukit/generators/simplecityjson.py
--rw-r--r--   0        0        0      627 2023-12-17 15:04:09.623873 plateaukit-0.9.1/plateaukit/generators/utils.py
--rw-r--r--   0        0        0     7626 2023-12-16 12:49:18.730673 plateaukit-0.9.1/plateaukit/geocoding.py
--rw-r--r--   0        0        0     2760 2023-12-12 10:13:14.732498 plateaukit-0.9.1/plateaukit/installer.py
--rw-r--r--   0        0        0      522 2023-12-10 15:17:40.428281 plateaukit-0.9.1/plateaukit/logger.py
--rw-r--r--   0        0        0       39 2023-12-07 10:03:26.229279 plateaukit-0.9.1/plateaukit/models/__init__.py
--rw-r--r--   0        0        0     2484 2023-12-11 16:43:04.680586 plateaukit-0.9.1/plateaukit/models/building.py
--rw-r--r--   0        0        0     2617 2023-12-17 14:55:28.586441 plateaukit-0.9.1/plateaukit/parallel.py
--rw-r--r--   0        0        0      207 2023-12-11 16:51:27.943720 plateaukit-0.9.1/plateaukit/parsers/__init__.py
--rw-r--r--   0        0        0     1942 2023-12-16 07:29:08.519135 plateaukit-0.9.1/plateaukit/parsers/city_gml_parser.py
--rw-r--r--   0        0        0    12906 2023-12-16 07:34:20.927653 plateaukit-0.9.1/plateaukit/parsers/city_object_parser.py
--rw-r--r--   0        0        0      726 2023-12-11 16:58:51.893753 plateaukit-0.9.1/plateaukit/parsers/codelist_parser.py
--rw-r--r--   0        0        0      494 2023-12-11 16:56:15.893604 plateaukit-0.9.1/plateaukit/parsers/constants.py
--rw-r--r--   0        0        0     2395 2024-02-23 18:46:55.893570 plateaukit-0.9.1/plateaukit/prebuild.py
--rw-r--r--   0        0        0      748 2023-12-17 15:05:41.744614 plateaukit-0.9.1/plateaukit/utils.py
--rw-r--r--   0        0        0     1709 2024-02-24 06:03:14.156948 plateaukit-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     3296 1970-01-01 00:00:00.000000 plateaukit-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-12-17 19:01:10.683916 plateaukit-0.9.2/LICENSE.txt
+-rw-r--r--   0        0        0     1759 2023-12-16 09:59:59.911832 plateaukit-0.9.2/README.md
+-rw-r--r--   0        0        0      175 2023-12-05 11:34:45.256449 plateaukit-0.9.2/plateaukit/__init__.py
+-rw-r--r--   0        0        0     3746 2023-12-16 12:18:11.976468 plateaukit-0.9.2/plateaukit/area.py
+-rw-r--r--   0        0        0    10834 2024-02-24 07:37:27.898402 plateaukit-0.9.2/plateaukit/cli.py
+-rw-r--r--   0        0        0     4349 2023-12-11 09:09:27.788234 plateaukit-0.9.2/plateaukit/config.py
+-rw-r--r--   0        0        0     1169 2023-12-06 13:11:13.146014 plateaukit-0.9.2/plateaukit/constants.py
+-rw-r--r--   0        0        0     9187 2023-12-17 15:05:22.989564 plateaukit-0.9.2/plateaukit/dataset.py
+-rw-r--r--   0        0        0      176 2023-08-05 20:23:37.132711 plateaukit-0.9.2/plateaukit/db.py
+-rw-r--r--   0        0        0       28 2023-08-05 20:23:37.133049 plateaukit-0.9.2/plateaukit/download/__init__.py
+-rw-r--r--   0        0        0     3174 2024-02-24 07:36:45.390598 plateaukit-0.9.2/plateaukit/download/downloader.py
+-rw-r--r--   0        0        0    46890 2023-12-03 20:05:55.280726 plateaukit-0.9.2/plateaukit/download/list.py
+-rw-r--r--   0        0        0       40 2023-12-07 10:09:42.824801 plateaukit-0.9.2/plateaukit/extractors/__init__.py
+-rw-r--r--   0        0        0      814 2023-12-17 15:02:39.203770 plateaukit-0.9.2/plateaukit/extractors/utils.py
+-rw-r--r--   0        0        0      142 2023-12-05 08:44:59.056683 plateaukit-0.9.2/plateaukit/generators/__init__.py
+-rw-r--r--   0        0        0     1471 2023-12-04 15:14:53.880047 plateaukit-0.9.2/plateaukit/generators/cityjson.py
+-rw-r--r--   0        0        0       52 2023-12-12 12:18:37.379655 plateaukit-0.9.2/plateaukit/generators/geojson/__init__.py
+-rw-r--r--   0        0        0     5943 2023-12-17 14:55:36.018621 plateaukit-0.9.2/plateaukit/generators/geojson/_parallel.py
+-rw-r--r--   0        0        0     2806 2023-12-16 09:54:32.759576 plateaukit-0.9.2/plateaukit/generators/geojson/_serial.py
+-rw-r--r--   0        0        0     3132 2023-12-12 13:05:56.954478 plateaukit-0.9.2/plateaukit/generators/geojson/_single.py
+-rw-r--r--   0        0        0     2016 2023-08-05 20:23:37.136162 plateaukit-0.9.2/plateaukit/generators/quantized_mesh.py
+-rw-r--r--   0        0        0    15554 2023-12-17 15:04:04.292187 plateaukit-0.9.2/plateaukit/generators/simplecityjson.py
+-rw-r--r--   0        0        0      627 2023-12-17 15:04:09.623873 plateaukit-0.9.2/plateaukit/generators/utils.py
+-rw-r--r--   0        0        0     7626 2023-12-16 12:49:18.730673 plateaukit-0.9.2/plateaukit/geocoding.py
+-rw-r--r--   0        0        0     2760 2023-12-12 10:13:14.732498 plateaukit-0.9.2/plateaukit/installer.py
+-rw-r--r--   0        0        0      522 2023-12-10 15:17:40.428281 plateaukit-0.9.2/plateaukit/logger.py
+-rw-r--r--   0        0        0       39 2023-12-07 10:03:26.229279 plateaukit-0.9.2/plateaukit/models/__init__.py
+-rw-r--r--   0        0        0     2484 2023-12-11 16:43:04.680586 plateaukit-0.9.2/plateaukit/models/building.py
+-rw-r--r--   0        0        0     2617 2023-12-17 14:55:28.586441 plateaukit-0.9.2/plateaukit/parallel.py
+-rw-r--r--   0        0        0      207 2023-12-11 16:51:27.943720 plateaukit-0.9.2/plateaukit/parsers/__init__.py
+-rw-r--r--   0        0        0     1942 2023-12-16 07:29:08.519135 plateaukit-0.9.2/plateaukit/parsers/city_gml_parser.py
+-rw-r--r--   0        0        0    12906 2023-12-16 07:34:20.927653 plateaukit-0.9.2/plateaukit/parsers/city_object_parser.py
+-rw-r--r--   0        0        0      726 2023-12-11 16:58:51.893753 plateaukit-0.9.2/plateaukit/parsers/codelist_parser.py
+-rw-r--r--   0        0        0      494 2023-12-11 16:56:15.893604 plateaukit-0.9.2/plateaukit/parsers/constants.py
+-rw-r--r--   0        0        0     2395 2024-02-23 18:46:55.893570 plateaukit-0.9.2/plateaukit/prebuild.py
+-rw-r--r--   0        0        0      748 2023-12-17 15:05:41.744614 plateaukit-0.9.2/plateaukit/utils.py
+-rw-r--r--   0        0        0     1709 2024-02-24 07:40:05.801600 plateaukit-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     3296 1970-01-01 00:00:00.000000 plateaukit-0.9.2/PKG-INFO
```

### Comparing `plateaukit-0.9.1/LICENSE.txt` & `plateaukit-0.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plateaukit-0.9.1/README.md` & `plateaukit-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `plateaukit-0.9.1/plateaukit/area.py` & `plateaukit-0.9.2/plateaukit/area.py`

 * *Files identical despite different names*

### Comparing `plateaukit-0.9.1/plateaukit/cli.py` & `plateaukit-0.9.2/plateaukit/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 @click.option(
     "--format",
     type=click.Choice(["citygml", "3dtiles"], case_sensitive=False),
     default="citygml",
 )
 @click.option("--local", help="Install local file. (without copying)")
 @click.option(
-    "--prebuild", "run_prebuild", is_flag=True, default=False, help="Prebuild dataset."
+    "--prebuild", "run_prebuild", is_flag=True, default=True, help="Prebuild dataset."
 )
 @click.option("--force", is_flag=True, default=False, help="Force install.")
 @click.option("--download-only", is_flag=True, default=False)
 @click.option("-l", "--list", is_flag=True, help="List all latest available datasets.")
 @click.option(
     "--list-all", is_flag=True, help="List all available datasets including old ones."
 )
```

### Comparing `plateaukit-0.9.1/plateaukit/config.py` & `plateaukit-0.9.2/plateaukit/config.py`

 * *Files identical despite different names*

### Comparing `plateaukit-0.9.1/plateaukit/constants.py` & `plateaukit-0.9.2/plateaukit/constants.py`

 * *Files identical despite different names*

### Comparing `plateaukit-0.9.1/plateaukit/dataset.py` & `plateaukit-0.9.2/plateaukit/dataset.py`

 * *Files identical despite different names*

### Comparing `plateaukit-0.9.1/plateaukit/download/downloader.py` & `plateaukit-0.9.2/plateaukit/download/downloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 def download_resource(resource_id, dest="/tmp"):
     resp = requests.get(f"{API_URL}/action/resource_show", params={"id": resource_id})
     data = resp.json()
 
     if not data["success"]:
         raise Exception("Failed to download")
 
-    # file_url = data["result"]["url"]
-    file_url = "http://127.0.0.1:8080/13100_tokyo23-ku_2022_citygml_1_2_op.zip"
+    file_url = data["result"]["url"]
     file_name = os.path.basename(urlparse(file_url).path)
 
     destfile_path = str(Path(dest, file_name))
 
     print(f"Download file as: {destfile_path.replace('/Users/nolze/', '~/')}")
 
     with requests.get(file_url, stream=True) as r:
```

### Comparing `plateaukit-0.9.1/plateaukit/download/list.py` & `plateaukit-0.9.2/plateaukit/download/list.py`

 * *Files identical despite different names*

### Comparing `plateaukit-0.9.1/plateaukit/extractors/utils.py` & `plateaukit-0.9.2/plateaukit/extractors/utils.py`

 * *Files identical despite different names*

### Comparing `plateaukit-0.9.1/plateaukit/generators/cityjson.py` & `plateaukit-0.9.2/plateaukit/generators/cityjson.py`

 * *Files identical despite different names*

### Comparing `plateaukit-0.9.1/plateaukit/generators/geojson/_parallel.py` & `plateaukit-0.9.2/plateaukit/generators/geojson/_parallel.py`

 * *Files identical despite different names*

### Comparing `plateaukit-0.9.1/plateaukit/generators/geojson/_serial.py` & `plateaukit-0.9.2/plateaukit/generators/geojson/_serial.py`

 * *Files identical despite different names*

### Comparing `plateaukit-0.9.1/plateaukit/generators/geojson/_single.py` & `plateaukit-0.9.2/plateaukit/generators/geojson/_single.py`

 * *Files identical despite different names*

### Comparing `plateaukit-0.9.1/plateaukit/generators/quantized_mesh.py` & `plateaukit-0.9.2/plateaukit/generators/quantized_mesh.py`

 * *Files identical despite different names*

### Comparing `plateaukit-0.9.1/plateaukit/generators/simplecityjson.py` & `plateaukit-0.9.2/plateaukit/generators/simplecityjson.py`

 * *Files identical despite different names*

### Comparing `plateaukit-0.9.1/plateaukit/generators/utils.py` & `plateaukit-0.9.2/plateaukit/generators/utils.py`

 * *Files identical despite different names*

### Comparing `plateaukit-0.9.1/plateaukit/geocoding.py` & `plateaukit-0.9.2/plateaukit/geocoding.py`

 * *Files identical despite different names*

### Comparing `plateaukit-0.9.1/plateaukit/installer.py` & `plateaukit-0.9.2/plateaukit/installer.py`

 * *Files identical despite different names*

### Comparing `plateaukit-0.9.1/plateaukit/logger.py` & `plateaukit-0.9.2/plateaukit/logger.py`

 * *Files identical despite different names*

### Comparing `plateaukit-0.9.1/plateaukit/models/building.py` & `plateaukit-0.9.2/plateaukit/models/building.py`

 * *Files identical despite different names*

### Comparing `plateaukit-0.9.1/plateaukit/parallel.py` & `plateaukit-0.9.2/plateaukit/parallel.py`

 * *Files identical despite different names*

### Comparing `plateaukit-0.9.1/plateaukit/parsers/city_gml_parser.py` & `plateaukit-0.9.2/plateaukit/parsers/city_gml_parser.py`

 * *Files identical despite different names*

### Comparing `plateaukit-0.9.1/plateaukit/parsers/city_object_parser.py` & `plateaukit-0.9.2/plateaukit/parsers/city_object_parser.py`

 * *Files identical despite different names*

### Comparing `plateaukit-0.9.1/plateaukit/parsers/codelist_parser.py` & `plateaukit-0.9.2/plateaukit/parsers/codelist_parser.py`

 * *Files identical despite different names*

### Comparing `plateaukit-0.9.1/plateaukit/prebuild.py` & `plateaukit-0.9.2/plateaukit/prebuild.py`

 * *Files identical despite different names*

### Comparing `plateaukit-0.9.1/plateaukit/utils.py` & `plateaukit-0.9.2/plateaukit/utils.py`

 * *Files identical despite different names*

### Comparing `plateaukit-0.9.1/pyproject.toml` & `plateaukit-0.9.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "plateaukit"
-version = "0.9.1"
+version = "0.9.2"
 description = "Python library and converter for 3D city models by MLIT Project PLATEAU"
 authors = ["Kentaro Ozeki <32771324+ozekik@users.noreply.github.com>"]
 readme = "README.md"
 homepage = "https://ozekik.github.io/plateaukit/"
 repository = "https://github.com/ozekik/plateaukit"
 license = "MIT"
 packages = [{ include = "plateaukit" }]
```

### Comparing `plateaukit-0.9.1/PKG-INFO` & `plateaukit-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plateaukit
-Version: 0.9.1
+Version: 0.9.2
 Summary: Python library and converter for 3D city models by MLIT Project PLATEAU
 Home-page: https://ozekik.github.io/plateaukit/
 License: MIT
 Author: Kentaro Ozeki
 Author-email: 32771324+ozekik@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: plateaukit Version: 0.9.1 Summary: Python library
+Metadata-Version: 2.1 Name: plateaukit Version: 0.9.2 Summary: Python library
 and converter for 3D city models by MLIT Project PLATEAU Home-page: https://
 ozekik.github.io/plateaukit/ License: MIT Author: Kentaro Ozeki Author-email:
 32771324+ozekik@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Requires-Dist: bidict (>=0.22.1,<0.23.0) Requires-
```

