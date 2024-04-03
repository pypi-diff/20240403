# Comparing `tmp/bro-0.2.8.tar.gz` & `tmp/bro-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bro-0.2.8.tar", last modified: Fri Oct  6 13:33:45 2023, max compression
+gzip compressed data, was "bro-0.2.9.tar", last modified: Mon Oct 16 09:17:41 2023, max compression
```

## Comparing `bro-0.2.8.tar` & `bro-0.2.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:33:45.749698 bro-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-10-06 13:33:25.000000 bro-0.2.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3741 2023-10-06 13:33:45.749698 bro-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2023-10-06 13:33:25.000000 bro-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:33:45.749698 bro-0.2.8/bro/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-10-06 13:33:25.000000 bro-0.2.8/bro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-10-06 13:33:25.000000 bro-0.2.8/bro/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12809 2023-10-06 13:33:25.000000 bro-0.2.8/bro/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2023-10-06 13:33:25.000000 bro-0.2.8/bro/helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2023-10-06 13:33:25.000000 bro-0.2.8/bro/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:33:45.749698 bro-0.2.8/bro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3741 2023-10-06 13:33:45.000000 bro-0.2.8/bro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      346 2023-10-06 13:33:45.000000 bro-0.2.8/bro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-06 13:33:45.000000 bro-0.2.8/bro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-10-06 13:33:45.000000 bro-0.2.8/bro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-10-06 13:33:45.000000 bro-0.2.8/bro.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:33:45.749698 bro-0.2.8/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 13:33:25.000000 bro-0.2.8/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2023-10-06 13:33:25.000000 bro-0.2.8/examples/examples.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2023-10-06 13:33:25.000000 bro-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-06 13:33:45.749698 bro-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2023-10-06 13:33:25.000000 bro-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:33:45.749698 bro-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5556 2023-10-06 13:33:25.000000 bro-0.2.8/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2023-10-06 13:33:25.000000 bro-0.2.8/tests/test_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 09:17:41.089648 bro-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-10-16 09:17:18.000000 bro-0.2.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3741 2023-10-16 09:17:41.089648 bro-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2023-10-16 09:17:18.000000 bro-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 09:17:41.089648 bro-0.2.9/bro/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2023-10-16 09:17:18.000000 bro-0.2.9/bro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2023-10-16 09:17:18.000000 bro-0.2.9/bro/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12584 2023-10-16 09:17:18.000000 bro-0.2.9/bro/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2023-10-16 09:17:18.000000 bro-0.2.9/bro/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2023-10-16 09:17:18.000000 bro-0.2.9/bro/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 09:17:41.089648 bro-0.2.9/bro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3741 2023-10-16 09:17:41.000000 bro-0.2.9/bro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2023-10-16 09:17:41.000000 bro-0.2.9/bro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-16 09:17:41.000000 bro-0.2.9/bro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2023-10-16 09:17:41.000000 bro-0.2.9/bro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2023-10-16 09:17:41.000000 bro-0.2.9/bro.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 09:17:41.089648 bro-0.2.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 09:17:18.000000 bro-0.2.9/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2023-10-16 09:17:18.000000 bro-0.2.9/examples/examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2023-10-16 09:17:18.000000 bro-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-16 09:17:41.089648 bro-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2023-10-16 09:17:18.000000 bro-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 09:17:41.089648 bro-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5556 2023-10-16 09:17:18.000000 bro-0.2.9/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2023-10-16 09:17:18.000000 bro-0.2.9/tests/test_objects.py
```

### Comparing `bro-0.2.8/LICENSE.txt` & `bro-0.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bro-0.2.8/PKG-INFO` & `bro-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bro
-Version: 0.2.8
+Version: 0.2.9
 Summary: Open source python library for accessing BRO API
 Author: VIKTOR
 Author-email: support@viktor.ai
 License: see LICENSE.txt
 Project-URL: Source code, https://github.com/viktor-platform/bro
 Project-URL: Example VIKTOR application, https://demo.viktor.ai/public/bro-app
 Project-URL: Source code VIKTOR application, https://github.com/viktor-platform/bro-app
@@ -21,15 +21,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: xmltodict==0.13.0
 Requires-Dist: requests==2.28.2
 Requires-Dist: lxml==4.9.2
 Requires-Dist: pyproj==3.4.1
 
-![](https://img.shields.io/badge/release-v0.2.8-green)
+![](https://img.shields.io/badge/release-v0.2.9-green)
 
 # BRO
 This package can access the REST API from the [BRO](https://www.broloket.nl/ondergrondgegevens). Currently, this package provides
 functionality to request CPTs from the BRO when you provide a region of interest. The format is based on the REST API of the BRO, which is described [here](https://publiek.broservices.nl/sr/cpt/v1/swagger-ui/#/default/) for CPTs.
 
 Current options include retrieval of the following objects: 
 1. CPTs (format: bytes, dict)
```

### Comparing `bro-0.2.8/README.md` & `bro-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `bro-0.2.8/bro/api.py` & `bro-0.2.9/bro/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -153,67 +153,61 @@
         self.standardized_location: Point = Point(
             *tuple(elem for elem in parsed_dispatch_document["brocom:standardizedLocation"]["gml:pos"].split(" "))
         )
         self.delivered_location: RDPoint = RDPoint(
             *tuple(elem for elem in parsed_dispatch_document["brocom:deliveredLocation"]["gml:pos"].split(" "))
         )
         self.local_vertical_reference_point: Optional[str] = (
-            parsed_dispatch_document["ns11:localVerticalReferencePoint"]["value"]
-            if parsed_dispatch_document.get("ns11:localVerticalReferencePoint")
+            parsed_dispatch_document["localVerticalReferencePoint"]["value"]
+            if parsed_dispatch_document.get("localVerticalReferencePoint")
             else None
         )
         self.vertical_datum: Optional[str] = (
-            parsed_dispatch_document["ns11:verticalDatum"]["value"]
-            if parsed_dispatch_document.get("ns11:verticalDatum")
+            parsed_dispatch_document["verticalDatum"]["value"]
+            if parsed_dispatch_document.get("verticalDatum")
             else None
         )
         self.cpt_standard: Optional[str] = (
-            parsed_dispatch_document["ns11:cptStandard"]["value"]
-            if parsed_dispatch_document.get("ns11:cptStandard")
-            else None
+            parsed_dispatch_document["cptStandard"]["value"] if parsed_dispatch_document.get("cptStandard") else None
         )
         self.offset: Optional[float] = (
-            float(parsed_dispatch_document["ns11:offset"]["value"])
-            if parsed_dispatch_document.get("ns11:offset")
-            else None
+            float(parsed_dispatch_document["offset"]["value"]) if parsed_dispatch_document.get("offset") else None
         )
         self.quality_class: Optional[str] = (
-            parsed_dispatch_document["ns11:qualityClass"]["value"]
-            if parsed_dispatch_document.get("ns11:qualityClass")
-            else None
+            parsed_dispatch_document["qualityClass"]["value"] if parsed_dispatch_document.get("qualityClass") else None
         )
         self.research_report_date: Optional[str] = (
-            parsed_dispatch_document["ns11:researchReportDate"]["brocom:date"]
-            if parsed_dispatch_document.get("ns11:researchReportDate")
+            parsed_dispatch_document["researchReportDate"]["brocom:date"]
+            if parsed_dispatch_document.get("researchReportDate")
             else None
         )
-        self.start_time: Optional[str] = parsed_dispatch_document.get("ns11:startTime")
+        self.start_time: Optional[str] = parsed_dispatch_document.get("startTime")
         self.predrilled_depth: Optional[float] = (
-            float(parsed_dispatch_document["ns11:predrilledDepth"]["value"])
-            if parsed_dispatch_document.get("ns11:predrilledDepth")
+            float(parsed_dispatch_document["predrilledDepth"]["value"])
+            if parsed_dispatch_document.get("predrilledDepth")
             else None
         )
         self.final_depth: Optional[float] = (
-            float(parsed_dispatch_document["ns11:finalDepth"]["value"])
-            if parsed_dispatch_document.get("ns11:finalDepth")
+            float(parsed_dispatch_document["finalDepth"]["value"])
+            if parsed_dispatch_document.get("finalDepth")
             else None
         )
         self.survey_purpose: Optional[str] = (
-            parsed_dispatch_document["ns11:surveyPurpose"]["value"]
-            if parsed_dispatch_document.get("ns11:surveyPurpose")
+            parsed_dispatch_document["surveyPurpose"]["value"]
+            if parsed_dispatch_document.get("surveyPurpose")
             else None
         )
         self.dissipation_test_performed: Optional[bool] = (
-            _str2bool(parsed_dispatch_document["ns11:dissipationTestPerformed"])
-            if parsed_dispatch_document.get("ns11:dissipationTestPerformed")
+            _str2bool(parsed_dispatch_document["dissipationTestPerformed"])
+            if parsed_dispatch_document.get("dissipationTestPerformed")
             else None
         )
         self.stop_criterion: Optional[str] = (
-            parsed_dispatch_document["ns11:stopCriterion"]["value"]
-            if parsed_dispatch_document.get("ns11:stopCriterion")
+            parsed_dispatch_document["stopCriterion"]["value"]
+            if parsed_dispatch_document.get("stopCriterion")
             else None
         )
 
     @property
     def to_geojson_feature(self) -> dict:
         return {
             "type": "Feature",
@@ -285,30 +279,30 @@
 
     response = requests.post(CPT_CHARACTERISTICS_URL, headers=headers, json=json, timeout=10)
 
     available_cpt_objects = []
     # TODO: Check status codes in BRO REST API documentation.
     if response.status_code == 200:
         parsed = xmltodict.parse(response.content, attr_prefix="", cdata_key="value")
-        rejection_reason = parsed["dispatchCharacteristicsResponseType"].get("brocom:rejectionReason")
+        rejection_reason = parsed["dispatchCharacteristicsResponse"].get("brocom:rejectionReason")
         if rejection_reason:
             raise ValueError(f"{rejection_reason}")
 
-        nr_of_documents = parsed["dispatchCharacteristicsResponseType"].get("ns11:numberOfDocuments")
+        nr_of_documents = parsed["dispatchCharacteristicsResponse"].get("numberOfDocuments")
         if nr_of_documents is None or nr_of_documents == "0":
             raise ValueError(
                 "No available objects have been found in given date + area range. Retry with different parameters."
             )
 
-        for document in parsed["dispatchCharacteristicsResponseType"]["ns11:dispatchDocument"]:
+        for document in parsed["dispatchCharacteristicsResponse"]["dispatchDocument"]:
             # TODO: Hard skip, this is likely to happen when it's deregistered. document will have key ["BRO_DO"]["brocom:deregistered"] = "ja"
             # TODO: Add this information to logger
-            if "ns11:CPT_C" not in document.keys():
+            if "CPT_C" not in document.keys():
                 continue
-            available_cpt_objects.append(CPTCharacteristics(document["ns11:CPT_C"]))
+            available_cpt_objects.append(CPTCharacteristics(document["CPT_C"]))
         return available_cpt_objects
     response.raise_for_status()
 
 
 def get_cpt_object(bro_cpt_id: str, as_dict: bool = False) -> Union[bytes, dict]:
     """Performs GET request on BRO API to retrieve a CPT object.
```

### Comparing `bro-0.2.8/bro/helper_functions.py` & `bro-0.2.9/bro/helper_functions.py`

 * *Files identical despite different names*

### Comparing `bro-0.2.8/bro/objects.py` & `bro-0.2.9/bro/objects.py`

 * *Files identical despite different names*

### Comparing `bro-0.2.8/bro.egg-info/PKG-INFO` & `bro-0.2.9/bro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bro
-Version: 0.2.8
+Version: 0.2.9
 Summary: Open source python library for accessing BRO API
 Author: VIKTOR
 Author-email: support@viktor.ai
 License: see LICENSE.txt
 Project-URL: Source code, https://github.com/viktor-platform/bro
 Project-URL: Example VIKTOR application, https://demo.viktor.ai/public/bro-app
 Project-URL: Source code VIKTOR application, https://github.com/viktor-platform/bro-app
@@ -21,15 +21,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: xmltodict==0.13.0
 Requires-Dist: requests==2.28.2
 Requires-Dist: lxml==4.9.2
 Requires-Dist: pyproj==3.4.1
 
-![](https://img.shields.io/badge/release-v0.2.8-green)
+![](https://img.shields.io/badge/release-v0.2.9-green)
 
 # BRO
 This package can access the REST API from the [BRO](https://www.broloket.nl/ondergrondgegevens). Currently, this package provides
 functionality to request CPTs from the BRO when you provide a region of interest. The format is based on the REST API of the BRO, which is described [here](https://publiek.broservices.nl/sr/cpt/v1/swagger-ui/#/default/) for CPTs.
 
 Current options include retrieval of the following objects: 
 1. CPTs (format: bytes, dict)
```

### Comparing `bro-0.2.8/examples/examples.py` & `bro-0.2.9/examples/examples.py`

 * *Files identical despite different names*

### Comparing `bro-0.2.8/pyproject.toml` & `bro-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bro-0.2.8/setup.py` & `bro-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `bro-0.2.8/tests/test_api.py` & `bro-0.2.9/tests/test_api.py`

 * *Files identical despite different names*

