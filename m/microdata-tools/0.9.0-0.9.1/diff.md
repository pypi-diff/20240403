# Comparing `tmp/microdata_tools-0.9.0.tar.gz` & `tmp/microdata_tools-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microdata_tools-0.9.0.tar", max compression
+gzip compressed data, was "microdata_tools-0.9.1.tar", max compression
```

## Comparing `microdata_tools-0.9.0.tar` & `microdata_tools-0.9.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1074 2023-11-08 13:04:21.893034 microdata_tools-0.9.0/LICENSE.md
--rw-r--r--   0        0        0     3764 2023-11-08 13:04:21.893034 microdata_tools-0.9.0/README.md
--rw-r--r--   0        0        0      384 2023-11-08 13:04:21.893034 microdata_tools-0.9.0/microdata_tools/__init__.py
--rw-r--r--   0        0        0     4368 2023-11-08 13:04:21.897035 microdata_tools-0.9.0/microdata_tools/packaging/__init__.py
--rw-r--r--   0        0        0     6072 2023-11-08 13:04:21.897035 microdata_tools-0.9.0/microdata_tools/packaging/_decrypt.py
--rw-r--r--   0        0        0     4950 2023-11-08 13:04:21.897035 microdata_tools-0.9.0/microdata_tools/packaging/_encrypt.py
--rw-r--r--   0        0        0     1188 2023-11-08 13:04:21.897035 microdata_tools-0.9.0/microdata_tools/packaging/_utils.py
--rw-r--r--   0        0        0      238 2023-11-08 13:04:21.897035 microdata_tools-0.9.0/microdata_tools/packaging/exceptions/__init__.py
--rw-r--r--   0        0        0     5818 2023-11-08 13:04:21.897035 microdata_tools-0.9.0/microdata_tools/validation/__init__.py
--rw-r--r--   0        0        0     2648 2023-11-08 13:04:21.897035 microdata_tools-0.9.0/microdata_tools/validation/adapter/local_storage.py
--rw-r--r--   0        0        0     5612 2023-11-08 13:04:21.897035 microdata_tools-0.9.0/microdata_tools/validation/components/temporal_attributes.py
--rw-r--r--   0        0        0     1130 2023-11-08 13:04:21.897035 microdata_tools-0.9.0/microdata_tools/validation/components/unit_id_types.py
--rw-r--r--   0        0        0     1551 2023-11-08 13:04:21.897035 microdata_tools-0.9.0/microdata_tools/validation/components/unit_type_variables/BK_HELSESTASJONSKONSULTASJON.json
--rw-r--r--   0        0        0     2093 2023-11-08 13:04:21.897035 microdata_tools-0.9.0/microdata_tools/validation/components/unit_type_variables/FAMILIE.json
--rw-r--r--   0        0        0     1527 2023-11-08 13:04:21.897035 microdata_tools-0.9.0/microdata_tools/validation/components/unit_type_variables/FORETAK.json
--rw-r--r--   0        0        0     1427 2023-11-08 13:04:21.897035 microdata_tools-0.9.0/microdata_tools/validation/components/unit_type_variables/HKDIR_STUDIESOKNAD.json
--rw-r--r--   0        0        0     2126 2023-11-08 13:04:21.897035 microdata_tools-0.9.0/microdata_tools/validation/components/unit_type_variables/HUSHOLDNING.json
--rw-r--r--   0        0        0     1431 2023-11-08 13:04:21.897035 microdata_tools-0.9.0/microdata_tools/validation/components/unit_type_variables/JOBB.json
--rw-r--r--   0        0        0     1380 2023-11-08 13:04:21.897035 microdata_tools-0.9.0/microdata_tools/validation/components/unit_type_variables/KJORETOY.json
--rw-r--r--   0        0        0   232471 2023-11-08 13:04:21.897035 microdata_tools-0.9.0/microdata_tools/validation/components/unit_type_variables/KOMMUNE.json
--rw-r--r--   0        0        0     1244 2023-11-08 13:04:21.897035 microdata_tools-0.9.0/microdata_tools/validation/components/unit_type_variables/KURS.json
--rw-r--r--   0        0        0     1823 2023-11-08 13:04:21.897035 microdata_tools-0.9.0/microdata_tools/validation/components/unit_type_variables/NPR_EPISODE.json
--rw-r--r--   0        0        0     1203 2023-11-08 13:04:21.897035 microdata_tools-0.9.0/microdata_tools/validation/components/unit_type_variables/PERSON.json
--rw-r--r--   0        0        0     1547 2023-11-08 13:04:21.897035 microdata_tools-0.9.0/microdata_tools/validation/components/unit_type_variables/SOSTIL.json
--rw-r--r--   0        0        0     1537 2023-11-08 13:04:21.897035 microdata_tools-0.9.0/microdata_tools/validation/components/unit_type_variables/VIRKSOMHET.json
--rw-r--r--   0        0        0     1427 2023-11-08 13:04:21.897035 microdata_tools-0.9.0/microdata_tools/validation/components/unit_type_variables/__init__.py
--rw-r--r--   0        0        0      490 2023-11-08 13:04:21.897035 microdata_tools-0.9.0/microdata_tools/validation/exceptions/__init__.py
--rw-r--r--   0        0        0      907 2023-11-08 13:04:21.897035 microdata_tools-0.9.0/microdata_tools/validation/model/__init__.py
--rw-r--r--   0        0        0     6208 2023-11-08 13:04:21.897035 microdata_tools-0.9.0/microdata_tools/validation/model/metadata.py
--rw-r--r--   0        0        0     6182 2023-11-08 13:04:21.897035 microdata_tools-0.9.0/microdata_tools/validation/steps/data_reader.py
--rw-r--r--   0        0        0    11699 2023-11-08 13:04:21.897035 microdata_tools-0.9.0/microdata_tools/validation/steps/dataset_validator.py
--rw-r--r--   0        0        0      680 2023-11-08 13:04:21.897035 microdata_tools-0.9.0/microdata_tools/validation/steps/metadata_enricher.py
--rw-r--r--   0        0        0     1501 2023-11-08 13:04:21.897035 microdata_tools-0.9.0/microdata_tools/validation/steps/metadata_reader.py
--rw-r--r--   0        0        0      602 2023-11-08 13:04:21.897035 microdata_tools-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     4412 1970-01-01 00:00:00.000000 microdata_tools-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-11-10 12:36:07.269935 microdata_tools-0.9.1/LICENSE.md
+-rw-r--r--   0        0        0     3764 2023-11-10 12:36:07.269935 microdata_tools-0.9.1/README.md
+-rw-r--r--   0        0        0      384 2023-11-10 12:36:07.273935 microdata_tools-0.9.1/microdata_tools/__init__.py
+-rw-r--r--   0        0        0     4368 2023-11-10 12:36:07.273935 microdata_tools-0.9.1/microdata_tools/packaging/__init__.py
+-rw-r--r--   0        0        0     6072 2023-11-10 12:36:07.273935 microdata_tools-0.9.1/microdata_tools/packaging/_decrypt.py
+-rw-r--r--   0        0        0     4950 2023-11-10 12:36:07.273935 microdata_tools-0.9.1/microdata_tools/packaging/_encrypt.py
+-rw-r--r--   0        0        0     1188 2023-11-10 12:36:07.273935 microdata_tools-0.9.1/microdata_tools/packaging/_utils.py
+-rw-r--r--   0        0        0      238 2023-11-10 12:36:07.273935 microdata_tools-0.9.1/microdata_tools/packaging/exceptions/__init__.py
+-rw-r--r--   0        0        0     5818 2023-11-10 12:36:07.273935 microdata_tools-0.9.1/microdata_tools/validation/__init__.py
+-rw-r--r--   0        0        0     2648 2023-11-10 12:36:07.273935 microdata_tools-0.9.1/microdata_tools/validation/adapter/local_storage.py
+-rw-r--r--   0        0        0     5612 2023-11-10 12:36:07.273935 microdata_tools-0.9.1/microdata_tools/validation/components/temporal_attributes.py
+-rw-r--r--   0        0        0     1130 2023-11-10 12:36:07.273935 microdata_tools-0.9.1/microdata_tools/validation/components/unit_id_types.py
+-rw-r--r--   0        0        0     1551 2023-11-10 12:36:07.273935 microdata_tools-0.9.1/microdata_tools/validation/components/unit_type_variables/BK_HELSESTASJONSKONSULTASJON.json
+-rw-r--r--   0        0        0     2093 2023-11-10 12:36:07.273935 microdata_tools-0.9.1/microdata_tools/validation/components/unit_type_variables/FAMILIE.json
+-rw-r--r--   0        0        0     1527 2023-11-10 12:36:07.273935 microdata_tools-0.9.1/microdata_tools/validation/components/unit_type_variables/FORETAK.json
+-rw-r--r--   0        0        0     1427 2023-11-10 12:36:07.273935 microdata_tools-0.9.1/microdata_tools/validation/components/unit_type_variables/HKDIR_STUDIESOKNAD.json
+-rw-r--r--   0        0        0     2126 2023-11-10 12:36:07.273935 microdata_tools-0.9.1/microdata_tools/validation/components/unit_type_variables/HUSHOLDNING.json
+-rw-r--r--   0        0        0     1431 2023-11-10 12:36:07.273935 microdata_tools-0.9.1/microdata_tools/validation/components/unit_type_variables/JOBB.json
+-rw-r--r--   0        0        0     1380 2023-11-10 12:36:07.273935 microdata_tools-0.9.1/microdata_tools/validation/components/unit_type_variables/KJORETOY.json
+-rw-r--r--   0        0        0   232471 2023-11-10 12:36:07.273935 microdata_tools-0.9.1/microdata_tools/validation/components/unit_type_variables/KOMMUNE.json
+-rw-r--r--   0        0        0     1244 2023-11-10 12:36:07.273935 microdata_tools-0.9.1/microdata_tools/validation/components/unit_type_variables/KURS.json
+-rw-r--r--   0        0        0     1823 2023-11-10 12:36:07.273935 microdata_tools-0.9.1/microdata_tools/validation/components/unit_type_variables/NPR_EPISODE.json
+-rw-r--r--   0        0        0     1203 2023-11-10 12:36:07.273935 microdata_tools-0.9.1/microdata_tools/validation/components/unit_type_variables/PERSON.json
+-rw-r--r--   0        0        0     1547 2023-11-10 12:36:07.273935 microdata_tools-0.9.1/microdata_tools/validation/components/unit_type_variables/SOSTIL.json
+-rw-r--r--   0        0        0     1537 2023-11-10 12:36:07.273935 microdata_tools-0.9.1/microdata_tools/validation/components/unit_type_variables/VIRKSOMHET.json
+-rw-r--r--   0        0        0     1427 2023-11-10 12:36:07.273935 microdata_tools-0.9.1/microdata_tools/validation/components/unit_type_variables/__init__.py
+-rw-r--r--   0        0        0      490 2023-11-10 12:36:07.273935 microdata_tools-0.9.1/microdata_tools/validation/exceptions/__init__.py
+-rw-r--r--   0        0        0      907 2023-11-10 12:36:07.273935 microdata_tools-0.9.1/microdata_tools/validation/model/__init__.py
+-rw-r--r--   0        0        0     6208 2023-11-10 12:36:07.273935 microdata_tools-0.9.1/microdata_tools/validation/model/metadata.py
+-rw-r--r--   0        0        0     6182 2023-11-10 12:36:07.273935 microdata_tools-0.9.1/microdata_tools/validation/steps/data_reader.py
+-rw-r--r--   0        0        0    11710 2023-11-10 12:36:07.273935 microdata_tools-0.9.1/microdata_tools/validation/steps/dataset_validator.py
+-rw-r--r--   0        0        0      680 2023-11-10 12:36:07.273935 microdata_tools-0.9.1/microdata_tools/validation/steps/metadata_enricher.py
+-rw-r--r--   0        0        0     1501 2023-11-10 12:36:07.273935 microdata_tools-0.9.1/microdata_tools/validation/steps/metadata_reader.py
+-rw-r--r--   0        0        0      602 2023-11-10 12:36:07.273935 microdata_tools-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     4412 1970-01-01 00:00:00.000000 microdata_tools-0.9.1/PKG-INFO
```

### Comparing `microdata_tools-0.9.0/LICENSE.md` & `microdata_tools-0.9.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.9.0/README.md` & `microdata_tools-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.9.0/microdata_tools/packaging/__init__.py` & `microdata_tools-0.9.1/microdata_tools/packaging/__init__.py`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.9.0/microdata_tools/packaging/_decrypt.py` & `microdata_tools-0.9.1/microdata_tools/packaging/_decrypt.py`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.9.0/microdata_tools/packaging/_encrypt.py` & `microdata_tools-0.9.1/microdata_tools/packaging/_encrypt.py`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.9.0/microdata_tools/packaging/_utils.py` & `microdata_tools-0.9.1/microdata_tools/packaging/_utils.py`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.9.0/microdata_tools/validation/__init__.py` & `microdata_tools-0.9.1/microdata_tools/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.9.0/microdata_tools/validation/adapter/local_storage.py` & `microdata_tools-0.9.1/microdata_tools/validation/adapter/local_storage.py`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.9.0/microdata_tools/validation/components/temporal_attributes.py` & `microdata_tools-0.9.1/microdata_tools/validation/components/temporal_attributes.py`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.9.0/microdata_tools/validation/components/unit_id_types.py` & `microdata_tools-0.9.1/microdata_tools/validation/components/unit_id_types.py`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.9.0/microdata_tools/validation/components/unit_type_variables/BK_HELSESTASJONSKONSULTASJON.json` & `microdata_tools-0.9.1/microdata_tools/validation/components/unit_type_variables/BK_HELSESTASJONSKONSULTASJON.json`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.9.0/microdata_tools/validation/components/unit_type_variables/FAMILIE.json` & `microdata_tools-0.9.1/microdata_tools/validation/components/unit_type_variables/FAMILIE.json`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.9.0/microdata_tools/validation/components/unit_type_variables/FORETAK.json` & `microdata_tools-0.9.1/microdata_tools/validation/components/unit_type_variables/FORETAK.json`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.9.0/microdata_tools/validation/components/unit_type_variables/HKDIR_STUDIESOKNAD.json` & `microdata_tools-0.9.1/microdata_tools/validation/components/unit_type_variables/HKDIR_STUDIESOKNAD.json`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.9.0/microdata_tools/validation/components/unit_type_variables/HUSHOLDNING.json` & `microdata_tools-0.9.1/microdata_tools/validation/components/unit_type_variables/HUSHOLDNING.json`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.9.0/microdata_tools/validation/components/unit_type_variables/JOBB.json` & `microdata_tools-0.9.1/microdata_tools/validation/components/unit_type_variables/JOBB.json`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.9.0/microdata_tools/validation/components/unit_type_variables/KJORETOY.json` & `microdata_tools-0.9.1/microdata_tools/validation/components/unit_type_variables/KJORETOY.json`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.9.0/microdata_tools/validation/components/unit_type_variables/KOMMUNE.json` & `microdata_tools-0.9.1/microdata_tools/validation/components/unit_type_variables/KOMMUNE.json`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.9.0/microdata_tools/validation/components/unit_type_variables/KURS.json` & `microdata_tools-0.9.1/microdata_tools/validation/components/unit_type_variables/KURS.json`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.9.0/microdata_tools/validation/components/unit_type_variables/NPR_EPISODE.json` & `microdata_tools-0.9.1/microdata_tools/validation/components/unit_type_variables/NPR_EPISODE.json`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.9.0/microdata_tools/validation/components/unit_type_variables/PERSON.json` & `microdata_tools-0.9.1/microdata_tools/validation/components/unit_type_variables/PERSON.json`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.9.0/microdata_tools/validation/components/unit_type_variables/SOSTIL.json` & `microdata_tools-0.9.1/microdata_tools/validation/components/unit_type_variables/SOSTIL.json`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.9.0/microdata_tools/validation/components/unit_type_variables/VIRKSOMHET.json` & `microdata_tools-0.9.1/microdata_tools/validation/components/unit_type_variables/VIRKSOMHET.json`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.9.0/microdata_tools/validation/components/unit_type_variables/__init__.py` & `microdata_tools-0.9.1/microdata_tools/validation/components/unit_type_variables/__init__.py`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.9.0/microdata_tools/validation/model/__init__.py` & `microdata_tools-0.9.1/microdata_tools/validation/model/__init__.py`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.9.0/microdata_tools/validation/model/metadata.py` & `microdata_tools-0.9.1/microdata_tools/validation/model/metadata.py`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.9.0/microdata_tools/validation/steps/data_reader.py` & `microdata_tools-0.9.1/microdata_tools/validation/steps/data_reader.py`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.9.0/microdata_tools/validation/steps/dataset_validator.py` & `microdata_tools-0.9.1/microdata_tools/validation/steps/dataset_validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,23 +146,23 @@
         )
 
 
 def _event_temporal_variables_check(data: FileSystemDataset):
     """
     Any given row in a table with temporalityType=EVENT is valid only if:
     * The start_epoch_days column contains a non-null value (int32)
-    * The stop_epoch_days is either a non-null value bigger than
+    * The stop_epoch_days is either a non-null value bigger than or equal to
       start_epoch_days (int32), or null (empty)
     """
     start_is_null_filter = dataset.field("start_epoch_days").is_null()
-    start_be_stop_filter = dataset.field("start_epoch_days") >= dataset.field(
+    start_bt_stop_filter = dataset.field("start_epoch_days") > dataset.field(
         "stop_epoch_days"
     )  # If stop_epoch_days is null this test will be ignored by pyarrow
     invalid_rows = data.to_table(
-        filter=(start_is_null_filter | start_be_stop_filter),
+        filter=(start_is_null_filter | start_bt_stop_filter),
         columns=["unit_id"],
     )
     if len(invalid_rows) > 0:
         raise ValidationError(
             "#3 and #4 columns",
             errors=_get_error_list(
                 invalid_rows, "Invalid #3 and/or #4 columns"
```

### Comparing `microdata_tools-0.9.0/microdata_tools/validation/steps/metadata_enricher.py` & `microdata_tools-0.9.1/microdata_tools/validation/steps/metadata_enricher.py`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.9.0/microdata_tools/validation/steps/metadata_reader.py` & `microdata_tools-0.9.1/microdata_tools/validation/steps/metadata_reader.py`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.9.0/pyproject.toml` & `microdata_tools-0.9.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "microdata-tools"
-version = "0.9.0"
+version = "0.9.1"
 description = "Tools for the microdata.no platform"
 authors = ["microdata-developers"]
 license = "MIT License"
 readme = "README.md"
 packages = [{include = "microdata_tools"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 cryptography = "^41.0.1"
 pydantic = "^1.10.9"
-pyarrow = "^12.0.1"
+pyarrow = "^14.0.1"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 ruff = "^0.0.272"
 pytest = "^7.3.2"
 pytest-cov = "^4.1.0"
```

### Comparing `microdata_tools-0.9.0/PKG-INFO` & `microdata_tools-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: microdata-tools
-Version: 0.9.0
+Version: 0.9.1
 Summary: Tools for the microdata.no platform
 License: MIT
 Author: microdata-developers
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cryptography (>=41.0.1,<42.0.0)
-Requires-Dist: pyarrow (>=12.0.1,<13.0.0)
+Requires-Dist: pyarrow (>=14.0.1,<15.0.0)
 Requires-Dist: pydantic (>=1.10.9,<2.0.0)
 Description-Content-Type: text/markdown
 
 # microdata-tools
 Tools for the [microdata.no](https://www.microdata.no/) platform
 
 ## Installation
```

