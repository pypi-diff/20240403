# Comparing `tmp/eikon_api_wrapper-0.0.3.tar.gz` & `tmp/eikon_api_wrapper-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eikon_api_wrapper-0.0.3.tar", max compression
+gzip compressed data, was "eikon_api_wrapper-0.0.4.tar", max compression
```

## Comparing `eikon_api_wrapper-0.0.3.tar` & `eikon_api_wrapper-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       70 2024-04-02 15:48:49.794399 eikon_api_wrapper-0.0.3/eikon_api_wrapper/__init__.py
--rw-r--r--   0        0        0    20844 2024-04-02 13:44:32.525596 eikon_api_wrapper-0.0.3/eikon_api_wrapper/docs/images/eikon_front_end_pic1.PNG
--rw-r--r--   0        0        0    10412 2024-04-02 13:44:32.536205 eikon_api_wrapper-0.0.3/eikon_api_wrapper/docs/images/eikon_front_end_pic2.PNG
--rw-r--r--   0        0        0     3791 2024-04-02 14:52:03.726133 eikon_api_wrapper-0.0.3/eikon_api_wrapper/eikon_data_extractor.py
--rw-r--r--   0        0        0     4156 2024-04-02 15:09:07.614800 eikon_api_wrapper-0.0.3/eikon_api_wrapper/session.py
--rw-r--r--   0        0        0     1091 2024-04-02 13:44:32.525596 eikon_api_wrapper-0.0.3/LICENSE
--rw-r--r--   0        0        0      510 2024-04-02 16:58:20.534035 eikon_api_wrapper-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1448 2024-04-02 15:28:59.434863 eikon_api_wrapper-0.0.3/README.md
--rw-r--r--   0        0        0     2090 1970-01-01 00:00:00.000000 eikon_api_wrapper-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       70 2024-04-03 07:47:31.403167 eikon_api_wrapper-0.0.4/eikon_api_wrapper/__init__.py
+-rw-r--r--   0        0        0    20844 2024-04-03 07:47:31.403167 eikon_api_wrapper-0.0.4/eikon_api_wrapper/docs/images/eikon_front_end_pic1.PNG
+-rw-r--r--   0        0        0    10412 2024-04-03 07:47:31.403167 eikon_api_wrapper-0.0.4/eikon_api_wrapper/docs/images/eikon_front_end_pic2.PNG
+-rw-r--r--   0        0        0     3791 2024-04-03 07:47:31.403167 eikon_api_wrapper-0.0.4/eikon_api_wrapper/eikon_data_extractor.py
+-rw-r--r--   0        0        0     4299 2024-04-03 21:15:40.002088 eikon_api_wrapper-0.0.4/eikon_api_wrapper/session.py
+-rw-r--r--   0        0        0     1091 2023-05-17 14:15:16.648265 eikon_api_wrapper-0.0.4/LICENSE
+-rw-r--r--   0        0        0      570 2024-04-03 21:15:39.999975 eikon_api_wrapper-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1448 2024-04-03 07:47:31.401165 eikon_api_wrapper-0.0.4/README.md
+-rw-r--r--   0        0        0     2132 1970-01-01 00:00:00.000000 eikon_api_wrapper-0.0.4/PKG-INFO
```

### Comparing `eikon_api_wrapper-0.0.3/eikon_api_wrapper/docs/images/eikon_front_end_pic1.PNG` & `eikon_api_wrapper-0.0.4/eikon_api_wrapper/docs/images/eikon_front_end_pic1.PNG`

 * *Files identical despite different names*

### Comparing `eikon_api_wrapper-0.0.3/eikon_api_wrapper/docs/images/eikon_front_end_pic2.PNG` & `eikon_api_wrapper-0.0.4/eikon_api_wrapper/docs/images/eikon_front_end_pic2.PNG`

 * *Files identical despite different names*

### Comparing `eikon_api_wrapper-0.0.3/eikon_api_wrapper/eikon_data_extractor.py` & `eikon_api_wrapper-0.0.4/eikon_api_wrapper/eikon_data_extractor.py`

 * *Files identical despite different names*

### Comparing `eikon_api_wrapper-0.0.3/eikon_api_wrapper/session.py` & `eikon_api_wrapper-0.0.4/eikon_api_wrapper/session.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import eikon as ek
 
-from eikon_data_extractor import EikonDataExtractor
+from eikon_api_wrapper.eikon_data_extractor import EikonDataExtractor
 
 
 class Session:
 
     def __init__(self, key, start_date=None, freq="D", **kwargs):
         ek.set_app_key(key)
         self.start_date = start_date
@@ -58,32 +58,33 @@
     def get_market_cap_data(self, isins):
         market_cap_cols = ["TR.CompanyMarketCap.Date", "TR.CompanyMarketCap"]
         extractor = EikonDataExtractor(
             isins, "market_cap", market_cap_cols, "M", block_size=200, precision=0
         )
         return extractor.download_data(self.start_date)
 
-    def get_climate_indicators(self, isins):
-        indicator_cols = [
-            "TR.TRESGScore.Date",
-            "TR.TRESGScore",
-            "TR.TRESGEmissionsScore",
-            "TR.TRESGInnovationScore",
-            "TR.TRESGResourceUseScore",
-            "TR.CO2DirectScope1",
-            "TR.CO2IndirectScope2",
-            "TR.CO2IndirectScope3",
-            "TR.TRESGManagementScore",
-            "TR.TRESGShareholdersScore",
-            "TR.TRESGCSRStrategyScore",
-            "TR.TRESGWorkforceScore",
-            "TR.TRESGHumanRightsScore",
-            "TR.TRESGCommunityScore",
-            "TR.TRESGProductResponsibilityScore",
-        ]
+    def get_climate_indicators(self, isins, indicator_cols=None):
+        if indicator_cols is None:
+            indicator_cols = [
+                "TR.TRESGScore.Date",
+                "TR.TRESGScore",
+                "TR.TRESGEmissionsScore",
+                "TR.TRESGInnovationScore",
+                "TR.TRESGResourceUseScore",
+                "TR.CO2DirectScope1",
+                "TR.CO2IndirectScope2",
+                "TR.CO2IndirectScope3",
+                "TR.TRESGManagementScore",
+                "TR.TRESGShareholdersScore",
+                "TR.TRESGCSRStrategyScore",
+                "TR.TRESGWorkforceScore",
+                "TR.TRESGHumanRightsScore",
+                "TR.TRESGCommunityScore",
+                "TR.TRESGProductResponsibilityScore",
+            ]
         extractor = EikonDataExtractor(
             isins, "indicators", indicator_cols, "FY", block_size=1000, precision=2
         )
         return extractor.download_data(self.start_date)
 
     def get_cusips(self, isins):
         extractor = EikonDataExtractor(
```

### Comparing `eikon_api_wrapper-0.0.3/LICENSE` & `eikon_api_wrapper-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `eikon_api_wrapper-0.0.3/README.md` & `eikon_api_wrapper-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `eikon_api_wrapper-0.0.3/PKG-INFO` & `eikon_api_wrapper-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: eikon_api_wrapper
-Version: 0.0.3
+Version: 0.0.4
 Summary: Enables effective and resilient Eikon data extracts.
 License: MIT
+Keywords: eikon,api,wrapper,data,extracts
 Author: Marcus Rockel
 Author-email: marcus.rockel@finance.uni-freiburg.de
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

