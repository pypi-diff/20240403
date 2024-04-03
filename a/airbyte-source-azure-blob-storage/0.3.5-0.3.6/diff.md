# Comparing `tmp/airbyte_source_azure_blob_storage-0.3.5.tar.gz` & `tmp/airbyte_source_azure_blob_storage-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_azure_blob_storage-0.3.5.tar", max compression
+gzip compressed data, was "airbyte_source_azure_blob_storage-0.3.6.tar", max compression
```

## Comparing `airbyte_source_azure_blob_storage-0.3.5.tar` & `airbyte_source_azure_blob_storage-0.3.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     4712 2024-03-26 18:40:49.000000 airbyte_source_azure_blob_storage-0.3.5/README.md
--rw-r--r--   0        0        0      983 2024-03-27 10:20:33.075687 airbyte_source_azure_blob_storage-0.3.5/pyproject.toml
--rw-r--r--   0        0        0      281 2024-03-26 18:40:49.000000 airbyte_source_azure_blob_storage-0.3.5/source_azure_blob_storage/__init__.py
--rw-r--r--   0        0        0     2499 2024-03-26 18:40:49.000000 airbyte_source_azure_blob_storage-0.3.5/source_azure_blob_storage/config.py
--rw-r--r--   0        0        0     1306 2024-03-26 18:40:49.000000 airbyte_source_azure_blob_storage-0.3.5/source_azure_blob_storage/legacy_config_transformer.py
--rw-r--r--   0        0        0     1758 2024-03-26 18:40:49.000000 airbyte_source_azure_blob_storage-0.3.5/source_azure_blob_storage/run.py
--rw-r--r--   0        0        0     1186 2024-03-26 18:40:49.000000 airbyte_source_azure_blob_storage-0.3.5/source_azure_blob_storage/source.py
--rw-r--r--   0        0        0     2940 2024-03-26 18:40:49.000000 airbyte_source_azure_blob_storage-0.3.5/source_azure_blob_storage/stream_reader.py
--rw-r--r--   0        0        0     5536 1970-01-01 00:00:00.000000 airbyte_source_azure_blob_storage-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     4712 2024-04-02 17:08:49.000000 airbyte_source_azure_blob_storage-0.3.6/README.md
+-rw-r--r--   0        0        0     1016 2024-04-03 12:19:39.803145 airbyte_source_azure_blob_storage-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0      281 2024-04-02 17:08:49.000000 airbyte_source_azure_blob_storage-0.3.6/source_azure_blob_storage/__init__.py
+-rw-r--r--   0        0        0     2499 2024-04-02 17:08:49.000000 airbyte_source_azure_blob_storage-0.3.6/source_azure_blob_storage/config.py
+-rw-r--r--   0        0        0     1306 2024-04-02 17:08:49.000000 airbyte_source_azure_blob_storage-0.3.6/source_azure_blob_storage/legacy_config_transformer.py
+-rw-r--r--   0        0        0     1758 2024-04-02 17:08:49.000000 airbyte_source_azure_blob_storage-0.3.6/source_azure_blob_storage/run.py
+-rw-r--r--   0        0        0     1186 2024-04-02 17:08:49.000000 airbyte_source_azure_blob_storage-0.3.6/source_azure_blob_storage/source.py
+-rw-r--r--   0        0        0     2902 2024-04-02 17:08:49.000000 airbyte_source_azure_blob_storage-0.3.6/source_azure_blob_storage/stream_reader.py
+-rw-r--r--   0        0        0     5536 1970-01-01 00:00:00.000000 airbyte_source_azure_blob_storage-0.3.6/PKG-INFO
```

### Comparing `airbyte_source_azure_blob_storage-0.3.5/README.md` & `airbyte_source_azure_blob_storage-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_azure_blob_storage-0.3.5/pyproject.toml` & `airbyte_source_azure_blob_storage-0.3.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.3.5"
+version = "0.3.6"
 name = "airbyte-source-azure-blob-storage"
 description = "Source implementation for Azure Blob Storage."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
@@ -21,25 +21,27 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
 pytz = "==2024.1"
 
 [tool.poetry.dependencies.airbyte-cdk]
-version = "0.75"
 extras = [
     "file-based",
 ]
+version = "^0"
 
 [tool.poetry.dependencies.smart-open]
 extras = [
     "azure",
 ]
 version = "==6.4.0"
 
 [tool.poetry.scripts]
 source-azure-blob-storage = "source_azure_blob_storage.run:run"
 
 [tool.poetry.group.dev.dependencies]
+docker = "^7.0.0"
 pytest-mock = "^3.6.1"
 requests-mock = "^1.9.3"
+pandas = "2.2.1"
 pytest = "^6.2"
```

### Comparing `airbyte_source_azure_blob_storage-0.3.5/source_azure_blob_storage/config.py` & `airbyte_source_azure_blob_storage-0.3.6/source_azure_blob_storage/config.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_azure_blob_storage-0.3.5/source_azure_blob_storage/legacy_config_transformer.py` & `airbyte_source_azure_blob_storage-0.3.6/source_azure_blob_storage/legacy_config_transformer.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_azure_blob_storage-0.3.5/source_azure_blob_storage/run.py` & `airbyte_source_azure_blob_storage-0.3.6/source_azure_blob_storage/run.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_azure_blob_storage-0.3.5/source_azure_blob_storage/source.py` & `airbyte_source_azure_blob_storage-0.3.6/source_azure_blob_storage/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_azure_blob_storage-0.3.5/source_azure_blob_storage/stream_reader.py` & `airbyte_source_azure_blob_storage-0.3.6/source_azure_blob_storage/stream_reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 
 import logging
-from contextlib import contextmanager
 from io import IOBase
 from typing import Iterable, List, Optional
 
 import pytz
 from airbyte_cdk.sources.file_based.file_based_stream_reader import AbstractFileBasedStreamReader, FileReadMode
 from airbyte_cdk.sources.file_based.remote_file import RemoteFile
 from azure.storage.blob import BlobServiceClient, ContainerClient
```

### Comparing `airbyte_source_azure_blob_storage-0.3.5/PKG-INFO` & `airbyte_source_azure_blob_storage-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: airbyte-source-azure-blob-storage
-Version: 0.3.5
+Version: 0.3.6
 Summary: Source implementation for Azure Blob Storage.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: airbyte-cdk[file-based] (==0.75)
+Requires-Dist: airbyte-cdk[file-based] (>=0,<1)
 Requires-Dist: pytz (==2024.1)
 Requires-Dist: smart-open[azure] (==6.4.0)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/azure-blob-storage
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Azure-Blob-Storage source connector
```

