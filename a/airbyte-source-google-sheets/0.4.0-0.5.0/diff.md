# Comparing `tmp/airbyte_source_google_sheets-0.4.0.tar.gz` & `tmp/airbyte_source_google_sheets-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_google_sheets-0.4.0.tar", max compression
+gzip compressed data, was "airbyte_source_google_sheets-0.5.0.tar", max compression
```

## Comparing `airbyte_source_google_sheets-0.4.0.tar` & `airbyte_source_google_sheets-0.5.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     4622 2024-03-21 01:47:20.485994 airbyte_source_google_sheets-0.4.0/README.md
--rw-r--r--   0        0        0      952 2024-03-21 02:18:34.115799 airbyte_source_google_sheets-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       73 2024-03-21 01:47:20.485994 airbyte_source_google_sheets-0.4.0/source_google_sheets/__init__.py
--rw-r--r--   0        0        0     2390 2024-03-21 01:47:20.485994 airbyte_source_google_sheets-0.4.0/source_google_sheets/client.py
--rw-r--r--   0        0        0    10501 2024-03-21 01:47:20.485994 airbyte_source_google_sheets-0.4.0/source_google_sheets/helpers.py
--rw-r--r--   0        0        0       61 2024-03-21 01:47:20.485994 airbyte_source_google_sheets-0.4.0/source_google_sheets/models/__init__.py
--rw-r--r--   0        0        0     1109 2024-03-21 01:47:20.485994 airbyte_source_google_sheets-0.4.0/source_google_sheets/models/spreadsheet.py
--rw-r--r--   0        0        0      437 2024-03-21 01:47:20.485994 airbyte_source_google_sheets-0.4.0/source_google_sheets/models/spreadsheet_values.py
--rw-r--r--   0        0        0      237 2024-03-21 01:47:20.485994 airbyte_source_google_sheets-0.4.0/source_google_sheets/run.py
--rw-r--r--   0        0        0    11681 2024-03-21 01:47:20.485994 airbyte_source_google_sheets-0.4.0/source_google_sheets/source.py
--rw-r--r--   0        0        0     4149 2024-03-21 01:47:20.485994 airbyte_source_google_sheets-0.4.0/source_google_sheets/spec.yaml
--rw-r--r--   0        0        0     2289 2024-03-21 01:47:20.485994 airbyte_source_google_sheets-0.4.0/source_google_sheets/utils.py
--rw-r--r--   0        0        0     5661 1970-01-01 00:00:00.000000 airbyte_source_google_sheets-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     4622 2024-04-03 16:36:04.000000 airbyte_source_google_sheets-0.5.0/README.md
+-rw-r--r--   0        0        0      870 2024-04-03 16:59:41.662228 airbyte_source_google_sheets-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       73 2024-04-03 16:36:04.000000 airbyte_source_google_sheets-0.5.0/source_google_sheets/__init__.py
+-rw-r--r--   0        0        0     2390 2024-04-03 16:36:04.000000 airbyte_source_google_sheets-0.5.0/source_google_sheets/client.py
+-rw-r--r--   0        0        0    10501 2024-04-03 16:36:04.000000 airbyte_source_google_sheets-0.5.0/source_google_sheets/helpers.py
+-rw-r--r--   0        0        0       61 2024-04-03 16:36:04.000000 airbyte_source_google_sheets-0.5.0/source_google_sheets/models/__init__.py
+-rw-r--r--   0        0        0     1109 2024-04-03 16:36:04.000000 airbyte_source_google_sheets-0.5.0/source_google_sheets/models/spreadsheet.py
+-rw-r--r--   0        0        0      437 2024-04-03 16:36:04.000000 airbyte_source_google_sheets-0.5.0/source_google_sheets/models/spreadsheet_values.py
+-rw-r--r--   0        0        0      237 2024-04-03 16:36:04.000000 airbyte_source_google_sheets-0.5.0/source_google_sheets/run.py
+-rw-r--r--   0        0        0    11688 2024-04-03 16:36:04.000000 airbyte_source_google_sheets-0.5.0/source_google_sheets/source.py
+-rw-r--r--   0        0        0     4149 2024-04-03 16:36:04.000000 airbyte_source_google_sheets-0.5.0/source_google_sheets/spec.yaml
+-rw-r--r--   0        0        0     2289 2024-04-03 16:36:04.000000 airbyte_source_google_sheets-0.5.0/source_google_sheets/utils.py
+-rw-r--r--   0        0        0     5527 1970-01-01 00:00:00.000000 airbyte_source_google_sheets-0.5.0/PKG-INFO
```

### Comparing `airbyte_source_google_sheets-0.4.0/README.md` & `airbyte_source_google_sheets-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_sheets-0.4.0/pyproject.toml` & `airbyte_source_google_sheets-0.5.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.4.0"
+version = "0.5.0"
 name = "airbyte-source-google-sheets"
 description = "Source implementation for Google Sheets."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "Elv2"
 readme = "README.md"
@@ -18,22 +18,18 @@
 repository = "https://github.com/airbytehq/airbyte"
 packages = [
     { include = "source_google_sheets" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-requests = "==2.31.0"
-backoff = "==2.2.1"
+airbyte-cdk = "^0"
 google-auth-httplib2 = "==0.2.0"
 Unidecode = "==1.3.8"
-pydantic = "==1.9.2"
-airbyte-cdk = "^0"
 google-api-python-client = "==2.114.0"
-PyYAML = "==6.0.1"
 
 [tool.poetry.scripts]
 source-google-sheets = "source_google_sheets.run:run"
 
 [tool.poetry.group.dev.dependencies]
 requests-mock = "^1.9.3"
 pytest-mock = "^3.6.1"
```

### Comparing `airbyte_source_google_sheets-0.4.0/source_google_sheets/client.py` & `airbyte_source_google_sheets-0.5.0/source_google_sheets/client.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_sheets-0.4.0/source_google_sheets/helpers.py` & `airbyte_source_google_sheets-0.5.0/source_google_sheets/helpers.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_sheets-0.4.0/source_google_sheets/models/spreadsheet.py` & `airbyte_source_google_sheets-0.5.0/source_google_sheets/models/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_sheets-0.4.0/source_google_sheets/source.py` & `airbyte_source_google_sheets-0.5.0/source_google_sheets/source.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
         sheet_to_column_index_to_name = Helpers.get_available_sheets_to_column_index_to_name(
             client, spreadsheet_id, sheet_to_column_name, config.get("names_conversion")
         )
         sheet_row_counts = Helpers.get_sheet_row_count(client, spreadsheet_id)
         logger.info(f"Row counts: {sheet_row_counts}")
         for sheet in sheet_to_column_index_to_name.keys():
             logger.info(f"Syncing sheet {sheet}")
-            stream = stream_name_to_stream.get(sheet)
+            stream = stream_name_to_stream.get(sheet).stream
             yield as_airbyte_message(stream, AirbyteStreamStatus.STARTED)
             # We revalidate the sheet here to avoid errors in case the sheet was changed after the sync started
             is_valid, reason = Helpers.check_sheet_is_valid(client, spreadsheet_id, sheet)
             if is_valid:
                 column_index_to_name = sheet_to_column_index_to_name[sheet]
                 row_cursor = 2  # we start syncing past the header row
                 # For the loop, it is necessary that the initial row exists when we send a request to the API,
```

### Comparing `airbyte_source_google_sheets-0.4.0/source_google_sheets/spec.yaml` & `airbyte_source_google_sheets-0.5.0/source_google_sheets/spec.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_sheets-0.4.0/source_google_sheets/utils.py` & `airbyte_source_google_sheets-0.5.0/source_google_sheets/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_sheets-0.4.0/PKG-INFO` & `airbyte_source_google_sheets-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 Metadata-Version: 2.1
 Name: airbyte-source-google-sheets
-Version: 0.4.0
+Version: 0.5.0
 Summary: Source implementation for Google Sheets.
 Home-page: https://airbyte.com
 License: Elv2
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: PyYAML (==6.0.1)
 Requires-Dist: Unidecode (==1.3.8)
 Requires-Dist: airbyte-cdk (>=0,<1)
-Requires-Dist: backoff (==2.2.1)
 Requires-Dist: google-api-python-client (==2.114.0)
 Requires-Dist: google-auth-httplib2 (==0.2.0)
-Requires-Dist: pydantic (==1.9.2)
-Requires-Dist: requests (==2.31.0)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/google-sheets
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Google-Sheets source connector
```

