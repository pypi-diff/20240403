# Comparing `tmp/basin3d-1.0.2.tar.gz` & `tmp/basin3d-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basin3d-1.0.2.tar", last modified: Mon Jan  8 16:13:18 2024, max compression
+gzip compressed data, was "basin3d-1.0.3.tar", last modified: Wed Apr  3 03:55:59 2024, max compression
```

## Comparing `basin3d-1.0.2.tar` & `basin3d-1.0.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 16:13:18.140942 basin3d-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-01-08 16:13:09.000000 basin3d-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-01-08 16:13:09.000000 basin3d-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8701 2024-01-08 16:13:18.140942 basin3d-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-01-08 16:13:09.000000 basin3d-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 16:13:18.132942 basin3d-1.0.2/basin3d/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-01-08 16:13:09.000000 basin3d-1.0.2/basin3d/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 16:13:18.136942 basin3d-1.0.2/basin3d/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 16:13:09.000000 basin3d-1.0.2/basin3d/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-01-08 16:13:09.000000 basin3d-1.0.2/basin3d/core/access.py
--rw-r--r--   0 runner    (1001) docker     (127)    29927 2024-01-08 16:13:09.000000 basin3d-1.0.2/basin3d/core/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    13765 2024-01-08 16:13:09.000000 basin3d-1.0.2/basin3d/core/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-08 16:13:09.000000 basin3d-1.0.2/basin3d/core/logging.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    54076 2024-01-08 16:13:09.000000 basin3d-1.0.2/basin3d/core/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-01-08 16:13:09.000000 basin3d-1.0.2/basin3d/core/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-01-08 16:13:09.000000 basin3d-1.0.2/basin3d/core/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 16:13:18.136942 basin3d-1.0.2/basin3d/core/schema/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 16:13:09.000000 basin3d-1.0.2/basin3d/core/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-01-08 16:13:09.000000 basin3d-1.0.2/basin3d/core/schema/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-01-08 16:13:09.000000 basin3d-1.0.2/basin3d/core/schema/query.py
--rw-r--r--   0 runner    (1001) docker     (127)    19527 2024-01-08 16:13:09.000000 basin3d-1.0.2/basin3d/core/synthesis.py
--rw-r--r--   0 runner    (1001) docker     (127)    18007 2024-01-08 16:13:09.000000 basin3d-1.0.2/basin3d/core/translate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-01-08 16:13:09.000000 basin3d-1.0.2/basin3d/core/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 16:13:18.136942 basin3d-1.0.2/basin3d/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 16:13:09.000000 basin3d-1.0.2/basin3d/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10191 2024-01-08 16:13:09.000000 basin3d-1.0.2/basin3d/data/basin3d_observed_property_vocabulary.csv
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-01-08 16:13:09.000000 basin3d-1.0.2/basin3d/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 16:13:18.136942 basin3d-1.0.2/basin3d/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 16:13:09.000000 basin3d-1.0.2/basin3d/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30999 2024-01-08 16:13:09.000000 basin3d-1.0.2/basin3d/plugins/epa.py
--rw-r--r--   0 runner    (1001) docker     (127)    10536 2024-01-08 16:13:09.000000 basin3d-1.0.2/basin3d/plugins/epa_mapping.csv
--rw-r--r--   0 runner    (1001) docker     (127)    71930 2024-01-08 16:13:09.000000 basin3d-1.0.2/basin3d/plugins/essdive.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-01-08 16:13:09.000000 basin3d-1.0.2/basin3d/plugins/essdive_mapping.csv
--rw-r--r--   0 runner    (1001) docker     (127)    32884 2024-01-08 16:13:09.000000 basin3d-1.0.2/basin3d/plugins/usgs.py
--rw-r--r--   0 runner    (1001) docker     (127)    66040 2024-01-08 16:13:09.000000 basin3d-1.0.2/basin3d/plugins/usgs_huc_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-01-08 16:13:09.000000 basin3d-1.0.2/basin3d/plugins/usgs_mapping.csv
--rw-r--r--   0 runner    (1001) docker     (127)    20469 2024-01-08 16:13:09.000000 basin3d-1.0.2/basin3d/synthesis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 16:13:18.136942 basin3d-1.0.2/basin3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8701 2024-01-08 16:13:18.000000 basin3d-1.0.2/basin3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-01-08 16:13:18.000000 basin3d-1.0.2/basin3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-08 16:13:18.000000 basin3d-1.0.2/basin3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-01-08 16:13:18.000000 basin3d-1.0.2/basin3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-08 16:13:18.000000 basin3d-1.0.2/basin3d.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-01-08 16:13:09.000000 basin3d-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-08 16:13:18.140942 basin3d-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:55:59.720528 basin3d-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-03 03:55:54.000000 basin3d-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-03 03:55:54.000000 basin3d-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8701 2024-04-03 03:55:59.720528 basin3d-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-03 03:55:54.000000 basin3d-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:55:59.712528 basin3d-1.0.3/basin3d/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-03 03:55:54.000000 basin3d-1.0.3/basin3d/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:55:59.716528 basin3d-1.0.3/basin3d/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 03:55:54.000000 basin3d-1.0.3/basin3d/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-03 03:55:54.000000 basin3d-1.0.3/basin3d/core/access.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29927 2024-04-03 03:55:54.000000 basin3d-1.0.3/basin3d/core/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13765 2024-04-03 03:55:54.000000 basin3d-1.0.3/basin3d/core/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-03 03:55:54.000000 basin3d-1.0.3/basin3d/core/logging.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    54076 2024-04-03 03:55:54.000000 basin3d-1.0.3/basin3d/core/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-04-03 03:55:54.000000 basin3d-1.0.3/basin3d/core/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-04-03 03:55:54.000000 basin3d-1.0.3/basin3d/core/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:55:59.716528 basin3d-1.0.3/basin3d/core/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 03:55:54.000000 basin3d-1.0.3/basin3d/core/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-04-03 03:55:54.000000 basin3d-1.0.3/basin3d/core/schema/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-04-03 03:55:54.000000 basin3d-1.0.3/basin3d/core/schema/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19527 2024-04-03 03:55:54.000000 basin3d-1.0.3/basin3d/core/synthesis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18007 2024-04-03 03:55:54.000000 basin3d-1.0.3/basin3d/core/translate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-03 03:55:54.000000 basin3d-1.0.3/basin3d/core/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:55:59.716528 basin3d-1.0.3/basin3d/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 03:55:54.000000 basin3d-1.0.3/basin3d/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10191 2024-04-03 03:55:54.000000 basin3d-1.0.3/basin3d/data/basin3d_observed_property_vocabulary.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-03 03:55:54.000000 basin3d-1.0.3/basin3d/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:55:59.716528 basin3d-1.0.3/basin3d/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 03:55:54.000000 basin3d-1.0.3/basin3d/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31070 2024-04-03 03:55:54.000000 basin3d-1.0.3/basin3d/plugins/epa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10536 2024-04-03 03:55:54.000000 basin3d-1.0.3/basin3d/plugins/epa_mapping.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    71930 2024-04-03 03:55:54.000000 basin3d-1.0.3/basin3d/plugins/essdive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-03 03:55:54.000000 basin3d-1.0.3/basin3d/plugins/essdive_mapping.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    32884 2024-04-03 03:55:54.000000 basin3d-1.0.3/basin3d/plugins/usgs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66040 2024-04-03 03:55:54.000000 basin3d-1.0.3/basin3d/plugins/usgs_huc_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-04-03 03:55:54.000000 basin3d-1.0.3/basin3d/plugins/usgs_mapping.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    20469 2024-04-03 03:55:54.000000 basin3d-1.0.3/basin3d/synthesis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:55:59.716528 basin3d-1.0.3/basin3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8701 2024-04-03 03:55:59.000000 basin3d-1.0.3/basin3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-03 03:55:59.000000 basin3d-1.0.3/basin3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 03:55:59.000000 basin3d-1.0.3/basin3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-03 03:55:59.000000 basin3d-1.0.3/basin3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 03:55:59.000000 basin3d-1.0.3/basin3d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-03 03:55:54.000000 basin3d-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 03:55:59.720528 basin3d-1.0.3/setup.cfg
```

### Comparing `basin3d-1.0.2/LICENSE` & `basin3d-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `basin3d-1.0.2/PKG-INFO` & `basin3d-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basin3d
-Version: 1.0.2
+Version: 1.0.3
 Summary: BASIN-3D Core Framework
 Author-email: Valerie C Hendrix <vchendrix@lbl.gov>, Danielle Svehla Christianson <dschristianson@lbl.gov>, Charuleka Varadharajan <cvaradharajan@lbl.gov>, Catherine Wong <catwong@lbl.gov>
 Maintainer-email: Valerie C Hendrix <vchendrix@lbl.gov>, Danielle Svehla Christianson <dschristianson@lbl.gov>
 License: Broker for Assimilation, Synthesis and Integration of eNvironmental Diverse, Distributed Datasets (BASIN-3D) Copyright (c) 2019, The
         Regents of the University of California, through Lawrence Berkeley National
         Laboratory (subject to receipt of any required approvals from the U.S.
         Dept. of Energy).  All rights reserved.
```

### Comparing `basin3d-1.0.2/README.md` & `basin3d-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `basin3d-1.0.2/basin3d/core/access.py` & `basin3d-1.0.3/basin3d/core/access.py`

 * *Files identical despite different names*

### Comparing `basin3d-1.0.2/basin3d/core/catalog.py` & `basin3d-1.0.3/basin3d/core/catalog.py`

 * *Files identical despite different names*

### Comparing `basin3d-1.0.2/basin3d/core/connection.py` & `basin3d-1.0.3/basin3d/core/connection.py`

 * *Files identical despite different names*

### Comparing `basin3d-1.0.2/basin3d/core/models.py` & `basin3d-1.0.3/basin3d/core/models.py`

 * *Files identical despite different names*

### Comparing `basin3d-1.0.2/basin3d/core/monitor.py` & `basin3d-1.0.3/basin3d/core/monitor.py`

 * *Files identical despite different names*

### Comparing `basin3d-1.0.2/basin3d/core/plugin.py` & `basin3d-1.0.3/basin3d/core/plugin.py`

 * *Files identical despite different names*

### Comparing `basin3d-1.0.2/basin3d/core/schema/enum.py` & `basin3d-1.0.3/basin3d/core/schema/enum.py`

 * *Files identical despite different names*

### Comparing `basin3d-1.0.2/basin3d/core/schema/query.py` & `basin3d-1.0.3/basin3d/core/schema/query.py`

 * *Files identical despite different names*

### Comparing `basin3d-1.0.2/basin3d/core/synthesis.py` & `basin3d-1.0.3/basin3d/core/synthesis.py`

 * *Files identical despite different names*

### Comparing `basin3d-1.0.2/basin3d/core/translate.py` & `basin3d-1.0.3/basin3d/core/translate.py`

 * *Files identical despite different names*

### Comparing `basin3d-1.0.2/basin3d/core/types.py` & `basin3d-1.0.3/basin3d/core/types.py`

 * *Files identical despite different names*

### Comparing `basin3d-1.0.2/basin3d/data/basin3d_observed_property_vocabulary.csv` & `basin3d-1.0.3/basin3d/data/basin3d_observed_property_vocabulary.csv`

 * *Files identical despite different names*

### Comparing `basin3d-1.0.2/basin3d/monitor.py` & `basin3d-1.0.3/basin3d/monitor.py`

 * *Files identical despite different names*

### Comparing `basin3d-1.0.2/basin3d/plugins/epa.py` & `basin3d-1.0.3/basin3d/plugins/epa.py`

 * *Files 0% similar despite different names*

```diff
@@ -571,23 +571,26 @@
 
         if query.end_date:
             params.update({"startDateHi": _reformat_date_for_epa_query(query.end_date)})
 
         # get data from resultPhysChem; possible extension biological results (sample based data)
         epa_data = _post_wqp_data_search(params)
 
+        mf_list = []
         if epa_data and epa_data.status_code == 200:
             # Because the data are all mixed together and we support multiple mappings,
             #   group the variables by the BASIN-3D vocab. Create a look up store for the variables in the query.
             op_map = self._get_observed_property_map(query.observed_property)
 
             results = {}  # type: ignore[var-annotated]
             mf_set = _parse_epa_results_phys_chem(epa_data, query, op_map, results, synthesis_messages)
+            mf_list = list(mf_set)
 
-            mf_query_str = _make_mf_query_str(list(mf_set))
+        if mf_list:
+            mf_query_str = _make_mf_query_str(mf_list)
             loc_info = _get_location_info(mf_query_str)
             loc_info_store = {}
             for loc_info_obj in loc_info:
                 loc_properties = loc_info_obj.get('properties')
                 if not loc_properties:
                     continue
                 loc_id = loc_properties.get('name')
```

### Comparing `basin3d-1.0.2/basin3d/plugins/epa_mapping.csv` & `basin3d-1.0.3/basin3d/plugins/epa_mapping.csv`

 * *Files identical despite different names*

### Comparing `basin3d-1.0.2/basin3d/plugins/essdive.py` & `basin3d-1.0.3/basin3d/plugins/essdive.py`

 * *Files identical despite different names*

### Comparing `basin3d-1.0.2/basin3d/plugins/essdive_mapping.csv` & `basin3d-1.0.3/basin3d/plugins/essdive_mapping.csv`

 * *Files identical despite different names*

### Comparing `basin3d-1.0.2/basin3d/plugins/usgs.py` & `basin3d-1.0.3/basin3d/plugins/usgs.py`

 * *Files identical despite different names*

### Comparing `basin3d-1.0.2/basin3d/plugins/usgs_huc_codes.py` & `basin3d-1.0.3/basin3d/plugins/usgs_huc_codes.py`

 * *Files identical despite different names*

### Comparing `basin3d-1.0.2/basin3d/plugins/usgs_mapping.csv` & `basin3d-1.0.3/basin3d/plugins/usgs_mapping.csv`

 * *Files identical despite different names*

### Comparing `basin3d-1.0.2/basin3d/synthesis.py` & `basin3d-1.0.3/basin3d/synthesis.py`

 * *Files identical despite different names*

### Comparing `basin3d-1.0.2/basin3d.egg-info/PKG-INFO` & `basin3d-1.0.3/basin3d.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basin3d
-Version: 1.0.2
+Version: 1.0.3
 Summary: BASIN-3D Core Framework
 Author-email: Valerie C Hendrix <vchendrix@lbl.gov>, Danielle Svehla Christianson <dschristianson@lbl.gov>, Charuleka Varadharajan <cvaradharajan@lbl.gov>, Catherine Wong <catwong@lbl.gov>
 Maintainer-email: Valerie C Hendrix <vchendrix@lbl.gov>, Danielle Svehla Christianson <dschristianson@lbl.gov>
 License: Broker for Assimilation, Synthesis and Integration of eNvironmental Diverse, Distributed Datasets (BASIN-3D) Copyright (c) 2019, The
         Regents of the University of California, through Lawrence Berkeley National
         Laboratory (subject to receipt of any required approvals from the U.S.
         Dept. of Energy).  All rights reserved.
```

### Comparing `basin3d-1.0.2/basin3d.egg-info/SOURCES.txt` & `basin3d-1.0.3/basin3d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `basin3d-1.0.2/pyproject.toml` & `basin3d-1.0.3/pyproject.toml`

 * *Files identical despite different names*

