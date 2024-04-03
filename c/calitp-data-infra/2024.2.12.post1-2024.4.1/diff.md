# Comparing `tmp/calitp_data_infra-2024.2.12.post1.tar.gz` & `tmp/calitp_data_infra-2024.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calitp_data_infra-2024.2.12.post1.tar", max compression
+gzip compressed data, was "calitp_data_infra-2024.4.1.tar", max compression
```

## Comparing `calitp_data_infra-2024.2.12.post1.tar` & `calitp_data_infra-2024.4.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2024-02-12 17:09:06.667719 calitp_data_infra-2024.2.12.post1/calitp_data_infra/__init__.py
--rw-r--r--   0        0        0     1210 2024-02-12 17:09:06.667719 calitp_data_infra-2024.2.12.post1/calitp_data_infra/auth.py
--rw-r--r--   0        0        0    25707 2024-02-12 17:09:06.667719 calitp_data_infra-2024.2.12.post1/calitp_data_infra/storage.py
--rw-r--r--   0        0        0      817 2024-02-12 17:09:06.667719 calitp_data_infra-2024.2.12.post1/pyproject.toml
--rw-r--r--   0        0        0      754 1970-01-01 00:00:00.000000 calitp_data_infra-2024.2.12.post1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-03 21:28:50.335850 calitp_data_infra-2024.4.1/calitp_data_infra/__init__.py
+-rw-r--r--   0        0        0     1210 2024-04-03 21:28:50.335850 calitp_data_infra-2024.4.1/calitp_data_infra/auth.py
+-rw-r--r--   0        0        0    25966 2024-04-03 21:28:50.335850 calitp_data_infra-2024.4.1/calitp_data_infra/storage.py
+-rw-r--r--   0        0        0      812 2024-04-03 21:28:50.335850 calitp_data_infra-2024.4.1/pyproject.toml
+-rw-r--r--   0        0        0      747 1970-01-01 00:00:00.000000 calitp_data_infra-2024.4.1/PKG-INFO
```

### Comparing `calitp_data_infra-2024.2.12.post1/calitp_data_infra/auth.py` & `calitp_data_infra-2024.4.1/calitp_data_infra/auth.py`

 * *Files identical despite different names*

### Comparing `calitp_data_infra-2024.2.12.post1/calitp_data_infra/storage.py` & `calitp_data_infra-2024.4.1/calitp_data_infra/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,21 @@
             project=gcs_project, token="google_default", **kwargs
         )
 
 
 def make_name_bq_safe(name: str):
     """Replace non-word characters.
     See: https://cloud.google.com/bigquery/docs/reference/standard-sql/lexical#identifiers.
+    Add underscore if starts with a number.  Also sometimes excel has columns names that are
+    all numbers, not even strings of numbers (ﾉﾟ0ﾟ)ﾉ~
     """
+    if type(name) != str:
+        name = str(name)
+    if name[:1].isdigit():
+        name = "_" + name
     return str.lower(re.sub("[^\w]", "_", name))  # noqa: W605
 
 
 AIRTABLE_BUCKET = os.getenv("CALITP_BUCKET__AIRTABLE")
 GTFS_DOWNLOAD_CONFIG_BUCKET = os.getenv("CALITP_BUCKET__GTFS_DOWNLOAD_CONFIG")
 SCHEDULE_RAW_BUCKET = os.getenv("CALITP_BUCKET__GTFS_SCHEDULE_RAW")
 RT_RAW_BUCKET = os.getenv("CALITP_BUCKET__GTFS_RT_RAW")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `calitp_data_infra-2024.2.12.post1/pyproject.toml` & `calitp_data_infra-2024.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "calitp-data-infra"
-version = "2024.2.12rev1"
+version = "2024.4.1"
 description = "Shared code for developing data pipelines that process Cal-ITP data."
 authors = ["Andrew Vaccaro <andrew.v@jarv.us>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.10"
 # Some of these are pinned oddly to play nicely with Composer
 pydantic = "~1.9"
```

### Comparing `calitp_data_infra-2024.2.12.post1/PKG-INFO` & `calitp_data_infra-2024.4.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calitp-data-infra
-Version: 2024.2.12.post1
+Version: 2024.4.1
 Summary: Shared code for developing data pipelines that process Cal-ITP data.
 Author: Andrew Vaccaro
 Author-email: andrew.v@jarv.us
 Requires-Python: >=3.8,<3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

