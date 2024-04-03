# Comparing `tmp/lasp_opensearch_data_center-0.3.0.tar.gz` & `tmp/lasp_opensearch_data_center-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lasp_opensearch_data_center-0.3.0.tar", max compression
+gzip compressed data, was "lasp_opensearch_data_center-0.5.0.tar", max compression
```

## Comparing `lasp_opensearch_data_center-0.3.0.tar` & `lasp_opensearch_data_center-0.5.0.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0       73 2024-01-12 18:19:32.607286 lasp_opensearch_data_center-0.3.0/README.md
--rw-r--r--   0        0        0        0 2024-01-12 18:19:32.607441 lasp_opensearch_data_center-0.3.0/lasp_opensearch_data_center/__init__.py
--rw-r--r--   0        0        0     4412 2024-03-04 17:03:36.472958 lasp_opensearch_data_center-0.3.0/lasp_opensearch_data_center/backend_storage.py
--rw-r--r--   0        0        0     8905 2024-03-19 16:45:40.867926 lasp_opensearch_data_center-0.3.0/lasp_opensearch_data_center/frontend.py
--rw-r--r--   0        0        0     3247 2024-02-19 17:09:16.082311 lasp_opensearch_data_center-0.3.0/lasp_opensearch_data_center/frontend_storage.py
--rw-r--r--   0        0        0      559 2024-03-19 16:45:40.869017 lasp_opensearch_data_center-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      798 1970-01-01 00:00:00.000000 lasp_opensearch_data_center-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       73 2024-01-12 18:19:32.607286 lasp_opensearch_data_center-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2024-01-12 18:19:32.607441 lasp_opensearch_data_center-0.5.0/lasp_opensearch_data_center/__init__.py
+-rw-r--r--   0        0        0     4412 2024-03-04 17:03:36.472958 lasp_opensearch_data_center-0.5.0/lasp_opensearch_data_center/backend_storage.py
+-rw-r--r--   0        0        0     2071 2024-04-03 15:49:53.061124 lasp_opensearch_data_center-0.5.0/lasp_opensearch_data_center/certificate.py
+-rw-r--r--   0        0        0     8905 2024-03-19 16:45:40.867926 lasp_opensearch_data_center-0.5.0/lasp_opensearch_data_center/frontend.py
+-rw-r--r--   0        0        0     3247 2024-02-19 17:09:16.082311 lasp_opensearch_data_center-0.5.0/lasp_opensearch_data_center/frontend_storage.py
+-rw-r--r--   0        0        0     1534 2024-04-03 15:49:53.061904 lasp_opensearch_data_center-0.5.0/lasp_opensearch_data_center/networking.py
+-rw-r--r--   0        0        0      559 2024-04-03 15:49:53.062295 lasp_opensearch_data_center-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      798 1970-01-01 00:00:00.000000 lasp_opensearch_data_center-0.5.0/PKG-INFO
```

### Comparing `lasp_opensearch_data_center-0.3.0/lasp_opensearch_data_center/backend_storage.py` & `lasp_opensearch_data_center-0.5.0/lasp_opensearch_data_center/backend_storage.py`

 * *Files identical despite different names*

### Comparing `lasp_opensearch_data_center-0.3.0/lasp_opensearch_data_center/frontend.py` & `lasp_opensearch_data_center-0.5.0/lasp_opensearch_data_center/frontend.py`

 * *Files identical despite different names*

### Comparing `lasp_opensearch_data_center-0.3.0/lasp_opensearch_data_center/frontend_storage.py` & `lasp_opensearch_data_center-0.5.0/lasp_opensearch_data_center/frontend_storage.py`

 * *Files identical despite different names*

### Comparing `lasp_opensearch_data_center-0.3.0/pyproject.toml` & `lasp_opensearch_data_center-0.5.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lasp_opensearch_data_center"
-version = "0.3.0"
+version = "0.5.0"
 description = "Construct library for creating a CSV ingest pipeline into OpenSearch with a front end website."
 authors = [
     "Gavin Medley <gavin.medley@lasp.colorado.edu>",
 ]
 maintainers = [
     "Gavin Medley <gavin.medley@lasp.colorado.edu>",
 ]
```

### Comparing `lasp_opensearch_data_center-0.3.0/PKG-INFO` & `lasp_opensearch_data_center-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lasp_opensearch_data_center
-Version: 0.3.0
+Version: 0.5.0
 Summary: Construct library for creating a CSV ingest pipeline into OpenSearch with a front end website.
 Author: Gavin Medley
 Author-email: gavin.medley@lasp.colorado.edu
 Maintainer: Gavin Medley
 Maintainer-email: gavin.medley@lasp.colorado.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
```

