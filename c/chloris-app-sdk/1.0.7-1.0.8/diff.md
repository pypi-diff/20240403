# Comparing `tmp/chloris_app_sdk-1.0.7.tar.gz` & `tmp/chloris_app_sdk-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chloris_app_sdk-1.0.7.tar", last modified: Wed Feb 14 21:25:34 2024, max compression
+gzip compressed data, was "chloris_app_sdk-1.0.8.tar", last modified: Wed Apr  3 14:47:54 2024, max compression
```

## Comparing `chloris_app_sdk-1.0.7.tar` & `chloris_app_sdk-1.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jay       (1000) jay       (1000)        0 2024-02-14 21:25:34.464070 chloris_app_sdk-1.0.7/
--rw-r--r--   0 jay       (1000) jay       (1000)     1079 2024-01-30 16:22:16.000000 chloris_app_sdk-1.0.7/LICENSE
--rw-r--r--   0 jay       (1000) jay       (1000)     2816 2024-02-14 21:25:34.464070 chloris_app_sdk-1.0.7/PKG-INFO
--rw-r--r--   0 jay       (1000) jay       (1000)     2493 2024-01-30 21:42:42.000000 chloris_app_sdk-1.0.7/README.md
--rw-r--r--   0 jay       (1000) jay       (1000)      100 2024-01-29 15:28:34.000000 chloris_app_sdk-1.0.7/pyproject.toml
--rw-r--r--   0 jay       (1000) jay       (1000)      506 2024-02-14 21:25:34.464070 chloris_app_sdk-1.0.7/setup.cfg
--rw-r--r--   0 jay       (1000) jay       (1000)       39 2024-01-29 15:27:09.000000 chloris_app_sdk-1.0.7/setup.py
-drwxr-xr-x   0 jay       (1000) jay       (1000)        0 2024-02-14 21:25:34.464070 chloris_app_sdk-1.0.7/src/
-drwxr-xr-x   0 jay       (1000) jay       (1000)        0 2024-02-14 21:25:34.464070 chloris_app_sdk-1.0.7/src/chloris_app_sdk/
--rw-r--r--   0 jay       (1000) jay       (1000)       37 2024-01-30 15:35:13.000000 chloris_app_sdk-1.0.7/src/chloris_app_sdk/__init__.py
--rw-r--r--   0 jay       (1000) jay       (1000)    34624 2024-02-14 21:25:14.000000 chloris_app_sdk-1.0.7/src/chloris_app_sdk/client.py
--rw-r--r--   0 jay       (1000) jay       (1000)     2111 2024-01-30 15:37:10.000000 chloris_app_sdk-1.0.7/src/chloris_app_sdk/utils.py
-drwxr-xr-x   0 jay       (1000) jay       (1000)        0 2024-02-14 21:25:34.464070 chloris_app_sdk-1.0.7/src/chloris_app_sdk.egg-info/
--rw-r--r--   0 jay       (1000) jay       (1000)     2816 2024-02-14 21:25:34.000000 chloris_app_sdk-1.0.7/src/chloris_app_sdk.egg-info/PKG-INFO
--rw-r--r--   0 jay       (1000) jay       (1000)      356 2024-02-14 21:25:34.000000 chloris_app_sdk-1.0.7/src/chloris_app_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 jay       (1000) jay       (1000)        1 2024-02-14 21:25:34.000000 chloris_app_sdk-1.0.7/src/chloris_app_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 jay       (1000) jay       (1000)       14 2024-02-14 21:25:34.000000 chloris_app_sdk-1.0.7/src/chloris_app_sdk.egg-info/requires.txt
--rw-r--r--   0 jay       (1000) jay       (1000)       16 2024-02-14 21:25:34.000000 chloris_app_sdk-1.0.7/src/chloris_app_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 jay       (1000) jay       (1000)        0 2024-04-03 14:47:54.082259 chloris_app_sdk-1.0.8/
+-rw-r--r--   0 jay       (1000) jay       (1000)     1079 2024-01-30 16:22:16.000000 chloris_app_sdk-1.0.8/LICENSE
+-rw-r--r--   0 jay       (1000) jay       (1000)     2816 2024-04-03 14:47:54.082259 chloris_app_sdk-1.0.8/PKG-INFO
+-rw-r--r--   0 jay       (1000) jay       (1000)     2493 2024-01-30 21:42:42.000000 chloris_app_sdk-1.0.8/README.md
+-rw-r--r--   0 jay       (1000) jay       (1000)      100 2024-01-29 15:28:34.000000 chloris_app_sdk-1.0.8/pyproject.toml
+-rw-r--r--   0 jay       (1000) jay       (1000)      506 2024-04-03 14:47:54.082259 chloris_app_sdk-1.0.8/setup.cfg
+-rw-r--r--   0 jay       (1000) jay       (1000)       39 2024-01-29 15:27:09.000000 chloris_app_sdk-1.0.8/setup.py
+drwxr-xr-x   0 jay       (1000) jay       (1000)        0 2024-04-03 14:47:54.072259 chloris_app_sdk-1.0.8/src/
+drwxr-xr-x   0 jay       (1000) jay       (1000)        0 2024-04-03 14:47:54.072259 chloris_app_sdk-1.0.8/src/chloris_app_sdk/
+-rw-r--r--   0 jay       (1000) jay       (1000)       37 2024-01-30 15:35:13.000000 chloris_app_sdk-1.0.8/src/chloris_app_sdk/__init__.py
+-rw-r--r--   0 jay       (1000) jay       (1000)    34876 2024-04-02 18:50:16.000000 chloris_app_sdk-1.0.8/src/chloris_app_sdk/client.py
+-rw-r--r--   0 jay       (1000) jay       (1000)     2111 2024-01-30 15:37:10.000000 chloris_app_sdk-1.0.8/src/chloris_app_sdk/utils.py
+drwxr-xr-x   0 jay       (1000) jay       (1000)        0 2024-04-03 14:47:54.082259 chloris_app_sdk-1.0.8/src/chloris_app_sdk.egg-info/
+-rw-r--r--   0 jay       (1000) jay       (1000)     2816 2024-04-03 14:47:54.000000 chloris_app_sdk-1.0.8/src/chloris_app_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 jay       (1000) jay       (1000)      356 2024-04-03 14:47:54.000000 chloris_app_sdk-1.0.8/src/chloris_app_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 jay       (1000) jay       (1000)        1 2024-04-03 14:47:54.000000 chloris_app_sdk-1.0.8/src/chloris_app_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 jay       (1000) jay       (1000)       14 2024-04-03 14:47:54.000000 chloris_app_sdk-1.0.8/src/chloris_app_sdk.egg-info/requires.txt
+-rw-r--r--   0 jay       (1000) jay       (1000)       16 2024-04-03 14:47:54.000000 chloris_app_sdk-1.0.8/src/chloris_app_sdk.egg-info/top_level.txt
```

### Comparing `chloris_app_sdk-1.0.7/LICENSE` & `chloris_app_sdk-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `chloris_app_sdk-1.0.7/PKG-INFO` & `chloris_app_sdk-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chloris_app_sdk
-Version: 1.0.7
+Version: 1.0.8
 Summary: A package created with a setuptools tutorial.  See article link for more details.
 Home-page: https://app.chloris.earth/docs/index.html
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: boto3
 Requires-Dist: urllib3
```

### Comparing `chloris_app_sdk-1.0.7/README.md` & `chloris_app_sdk-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `chloris_app_sdk-1.0.7/src/chloris_app_sdk/client.py` & `chloris_app_sdk-1.0.8/src/chloris_app_sdk/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -612,15 +612,19 @@
         # remove areaKm2 due to naming conflict with the reporting unit vector area
         result.pop("areaKm2", None)
         return result
 
     def _get_data_path(self, reporting_unit_entry: Mapping[str, Any]) -> str:
         data_path = reporting_unit_entry.get("dataPath")
         if data_path is None:
-            data_path = '/'.join([self.data_path.rstrip('/'), reporting_unit_entry['organizationId'], reporting_unit_entry['reportingUnitId'], ''])
+            versioned_reporting_unit_id = reporting_unit_entry['reportingUnitId']
+            version_id = reporting_unit_entry.get("versionId")
+            if version_id:
+                versioned_reporting_unit_id = f"{versioned_reporting_unit_id}_{version_id}"
+            data_path = '/'.join([self.data_path.rstrip('/'), reporting_unit_entry['organizationId'], versioned_reporting_unit_id, ''])
         else:
             data_path = data_path.rstrip("/") + "/"
         if data_path.startswith("s3://"):
             data_path = data_path.replace("s3://chloris-app-data/data/", self.data_path)
         return data_path
 
     def get_reporting_unit_layers_config(self, reporting_unit_entry: Mapping[str, Any]) -> Mapping[str, Any]:
```

### Comparing `chloris_app_sdk-1.0.7/src/chloris_app_sdk/utils.py` & `chloris_app_sdk-1.0.8/src/chloris_app_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `chloris_app_sdk-1.0.7/src/chloris_app_sdk.egg-info/PKG-INFO` & `chloris_app_sdk-1.0.8/src/chloris_app_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chloris_app_sdk
-Version: 1.0.7
+Version: 1.0.8
 Summary: A package created with a setuptools tutorial.  See article link for more details.
 Home-page: https://app.chloris.earth/docs/index.html
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: boto3
 Requires-Dist: urllib3
```

