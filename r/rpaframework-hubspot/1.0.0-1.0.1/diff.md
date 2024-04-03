# Comparing `tmp/rpaframework_hubspot-1.0.0.tar.gz` & `tmp/rpaframework_hubspot-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpaframework_hubspot-1.0.0.tar", max compression
+gzip compressed data, was "rpaframework_hubspot-1.0.1.tar", max compression
```

## Comparing `rpaframework_hubspot-1.0.0.tar` & `rpaframework_hubspot-1.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11560 2023-11-29 15:48:49.824469 rpaframework_hubspot-1.0.0/LICENSE
--rw-r--r--   0        0        0     2052 2023-12-18 19:08:39.321697 rpaframework_hubspot-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      413 2023-12-18 14:50:40.816701 rpaframework_hubspot-1.0.0/README.rst
--rw-r--r--   0        0        0    63378 2023-12-18 19:20:44.208380 rpaframework_hubspot-1.0.0/RPA_Hubspot.libspec
--rw-r--r--   0        0        0    89445 2023-12-18 19:09:11.218386 rpaframework_hubspot-1.0.0/src/RPA/Hubspot.py
--rw-r--r--   0        0        0     1829 1970-01-01 00:00:00.000000 rpaframework_hubspot-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11560 2023-12-18 15:49:28.634901 rpaframework_hubspot-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2052 2024-04-03 09:27:35.924437 rpaframework_hubspot-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      413 2023-12-18 15:49:28.635934 rpaframework_hubspot-1.0.1/README.rst
+-rw-r--r--   0        0        0    63378 2024-04-03 09:28:49.601934 rpaframework_hubspot-1.0.1/RPA_Hubspot.libspec
+-rw-r--r--   0        0        0    89445 2023-12-18 20:08:33.053592 rpaframework_hubspot-1.0.1/src/RPA/Hubspot.py
+-rw-r--r--   0        0        0     1829 1970-01-01 00:00:00.000000 rpaframework_hubspot-1.0.1/PKG-INFO
```

### Comparing `rpaframework_hubspot-1.0.0/LICENSE` & `rpaframework_hubspot-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rpaframework_hubspot-1.0.0/pyproject.toml` & `rpaframework_hubspot-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rpaframework-hubspot"
-version = "1.0.0"
+version = "1.0.1"
 description = "Robot Framework wrapper around the hubspot-api-client library."
 authors = ["RPA Framework <rpafw@robocorp.com>"]
 license = "Apache-2.0"
 readme = "README.rst"
 
 homepage = "https://rpaframework.org/"
 documentation = "https://rpaframework.org/"
@@ -28,15 +28,15 @@
 include = ["*.libspec"]
 
 packages = [{ include = "RPA", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 robotframework = ">=4.0.0,!=4.0.1,!=6.1.0,<7.0.0"
-rpaframework-core = "^11.2.3"
+rpaframework-core = "^11.3.1"
 tenacity = "^8.0.1"
 hubspot-api-client = "^4.0.6"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.3.0"
 flake8 = "^3.7.9"
 pylint = "^2.4.4, <2.13"
```

### Comparing `rpaframework_hubspot-1.0.0/RPA_Hubspot.libspec` & `rpaframework_hubspot-1.0.1/RPA_Hubspot.libspec`

 * *Files 0% similar despite different names*

#### Comparing `rpaframework_hubspot-1.0.0/RPA_Hubspot.libspec` & `rpaframework_hubspot-1.0.1/RPA_Hubspot.libspec`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<keywordspec name="RPA.Hubspot" type="LIBRARY" format="REST" scope="GLOBAL" generated="2023-12-18T19:20:44+00:00" specversion="5" source="./RPA/Hubspot.py" lineno="410">
+<keywordspec name="RPA.Hubspot" type="LIBRARY" format="REST" scope="GLOBAL" generated="2024-04-03T09:28:49+00:00" specversion="5" source="./RPA/Hubspot.py" lineno="410">
   <version/>
   <doc>*Hubspot* is a library for accessing HubSpot using REST API. It
 extends `hubspot-api-client &lt;https://pypi.org/project/hubspot-api-client/&gt;`_.
 
 Current features of this library focus on retrieving CRM object data
 from HubSpot via API. For additional information, see
 `Understanding the CRM &lt;https://developers.hubspot.com/docs/api/crm/understanding-the-crm&gt;`_.
```

### Comparing `rpaframework_hubspot-1.0.0/src/RPA/Hubspot.py` & `rpaframework_hubspot-1.0.1/src/RPA/Hubspot.py`

 * *Files identical despite different names*

### Comparing `rpaframework_hubspot-1.0.0/PKG-INFO` & `rpaframework_hubspot-1.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpaframework-hubspot
-Version: 1.0.0
+Version: 1.0.1
 Summary: Robot Framework wrapper around the hubspot-api-client library.
 Home-page: https://rpaframework.org/
 License: Apache-2.0
 Keywords: robotframework,rpa,automation,hubspot
 Author: RPA Framework
 Author-email: rpafw@robocorp.com
 Requires-Python: >=3.8.1,<4.0.0
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: hubspot-api-client (>=4.0.6,<5.0.0)
 Requires-Dist: robotframework (>=4.0.0,!=4.0.1,!=6.1.0,<7.0.0)
-Requires-Dist: rpaframework-core (>=11.2.3,<12.0.0)
+Requires-Dist: rpaframework-core (>=11.3.1,<12.0.0)
 Requires-Dist: tenacity (>=8.0.1,<9.0.0)
 Project-URL: Documentation, https://rpaframework.org/
 Project-URL: Repository, https://github.com/robocorp/rpaframework
 Description-Content-Type: text/x-rst
 
 rpaframework-hubspot
 ====================
```

