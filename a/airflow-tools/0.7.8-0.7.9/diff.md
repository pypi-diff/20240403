# Comparing `tmp/airflow_tools-0.7.8.tar.gz` & `tmp/airflow_tools-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow_tools-0.7.8.tar", max compression
+gzip compressed data, was "airflow_tools-0.7.9.tar", max compression
```

## Comparing `airflow_tools-0.7.8.tar` & `airflow_tools-0.7.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0    11358 2024-03-15 09:01:15.875283 airflow_tools-0.7.8/LICENSE.txt
--rw-r--r--   0        0        0     8912 2024-03-20 09:34:25.219293 airflow_tools-0.7.8/README.md
--rw-r--r--   0        0        0     1312 2024-03-26 11:55:40.215218 airflow_tools-0.7.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-15 09:01:15.879171 airflow_tools-0.7.8/src/airflow_tools/__init__.py
--rw-r--r--   0        0        0       22 2024-03-26 11:55:53.283269 airflow_tools-0.7.8/src/airflow_tools/_version.py
--rw-r--r--   0        0        0     1794 2024-03-15 09:01:15.879695 airflow_tools-0.7.8/src/airflow_tools/compression_utils.py
--rw-r--r--   0        0        0     4426 2024-03-23 22:52:20.616265 airflow_tools-0.7.8/src/airflow_tools/data_lake_facade.py
--rw-r--r--   0        0        0      115 2024-03-15 09:01:15.880246 airflow_tools-0.7.8/src/airflow_tools/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-15 09:01:15.880736 airflow_tools-0.7.8/src/airflow_tools/filesystems/__init__.py
--rw-r--r--   0        0        0     2298 2024-03-15 14:21:53.853567 airflow_tools-0.7.8/src/airflow_tools/filesystems/filesystem_factory.py
--rw-r--r--   0        0        0      561 2024-03-23 23:14:28.037837 airflow_tools-0.7.8/src/airflow_tools/filesystems/filesystem_protocol.py
--rw-r--r--   0        0        0        0 2024-03-15 09:01:15.882284 airflow_tools-0.7.8/src/airflow_tools/filesystems/impl/__init__.py
--rw-r--r--   0        0        0     1946 2024-03-25 00:36:28.134372 airflow_tools-0.7.8/src/airflow_tools/filesystems/impl/azure_databricks_volume_filesystem.py
--rw-r--r--   0        0        0     1974 2024-03-24 00:50:06.290603 airflow_tools-0.7.8/src/airflow_tools/filesystems/impl/azure_file_share_filesystem.py
--rw-r--r--   0        0        0     2472 2024-03-25 16:17:00.235954 airflow_tools-0.7.8/src/airflow_tools/filesystems/impl/blob_storage_filesystem.py
--rw-r--r--   0        0        0     1586 2024-03-24 00:21:54.773711 airflow_tools-0.7.8/src/airflow_tools/filesystems/impl/local_filesystem.py
--rw-r--r--   0        0        0     2185 2024-03-24 00:50:06.294839 airflow_tools-0.7.8/src/airflow_tools/filesystems/impl/s3_filesystem.py
--rw-r--r--   0        0        0     1396 2024-03-24 00:21:54.788482 airflow_tools-0.7.8/src/airflow_tools/filesystems/impl/sftp_filesystem.py
--rw-r--r--   0        0        0     3877 2024-03-15 09:01:15.884092 airflow_tools-0.7.8/src/airflow_tools/notifications/slack/webhook.py
--rw-r--r--   0        0        0        0 2024-03-15 09:01:15.884537 airflow_tools-0.7.8/src/airflow_tools/providers/__init__.py
--rw-r--r--   0        0        0        0 2024-03-15 09:01:15.884904 airflow_tools-0.7.8/src/airflow_tools/providers/azure/__init__.py
--rw-r--r--   0        0        0        0 2024-03-15 09:01:15.885232 airflow_tools-0.7.8/src/airflow_tools/providers/azure/hooks/__init__.py
--rw-r--r--   0        0        0     3396 2024-03-18 14:38:56.888663 airflow_tools-0.7.8/src/airflow_tools/providers/azure/hooks/azure_databricks.py
--rw-r--r--   0        0        0     1619 2024-03-15 09:01:15.885704 airflow_tools-0.7.8/src/airflow_tools/providers/azure/hooks/azure_file_share.py
--rw-r--r--   0        0        0        0 2024-03-15 09:01:15.886187 airflow_tools-0.7.8/src/airflow_tools/providers/data_lake/__init__.py
--rw-r--r--   0        0        0        0 2024-03-15 09:01:15.886773 airflow_tools-0.7.8/src/airflow_tools/providers/data_lake/operators/__init__.py
--rw-r--r--   0        0        0     2355 2024-03-23 22:52:20.625836 airflow_tools-0.7.8/src/airflow_tools/providers/data_lake/operators/data_lake.py
--rw-r--r--   0        0        0        0 2024-03-15 09:01:15.887444 airflow_tools-0.7.8/src/airflow_tools/providers/filesystem/__init__.py
--rw-r--r--   0        0        0        0 2024-03-15 09:01:15.888053 airflow_tools-0.7.8/src/airflow_tools/providers/filesystem/operators/__init__.py
--rw-r--r--   0        0        0     5385 2024-03-26 11:53:51.801039 airflow_tools-0.7.8/src/airflow_tools/providers/filesystem/operators/filesystem.py
--rw-r--r--   0        0        0        0 2024-03-15 09:01:15.890235 airflow_tools-0.7.8/src/airflow_tools/providers/http_to_data_lake/__init__.py
--rw-r--r--   0        0        0        0 2024-03-15 09:01:15.891091 airflow_tools-0.7.8/src/airflow_tools/providers/http_to_data_lake/operators/__init__.py
--rw-r--r--   0        0        0     8762 2024-03-24 22:53:13.055997 airflow_tools-0.7.8/src/airflow_tools/providers/http_to_data_lake/operators/http_to_data_lake.py
--rw-r--r--   0        0        0     1108 2024-03-18 14:38:56.889184 airflow_tools-0.7.8/src/airflow_tools/providers/package.py
--rw-r--r--   0        0        0        0 2024-03-15 09:01:15.891899 airflow_tools-0.7.8/src/airflow_tools/py.typed
--rw-r--r--   0        0        0    10150 1970-01-01 00:00:00.000000 airflow_tools-0.7.8/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-03-15 09:01:15.875283 airflow_tools-0.7.9/LICENSE.txt
+-rw-r--r--   0        0        0     8912 2024-03-20 09:34:25.219293 airflow_tools-0.7.9/README.md
+-rw-r--r--   0        0        0     1312 2024-03-26 13:08:04.481048 airflow_tools-0.7.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-15 09:01:15.879171 airflow_tools-0.7.9/src/airflow_tools/__init__.py
+-rw-r--r--   0        0        0       22 2024-03-26 13:08:15.557289 airflow_tools-0.7.9/src/airflow_tools/_version.py
+-rw-r--r--   0        0        0     1794 2024-03-15 09:01:15.879695 airflow_tools-0.7.9/src/airflow_tools/compression_utils.py
+-rw-r--r--   0        0        0     4426 2024-03-23 22:52:20.616265 airflow_tools-0.7.9/src/airflow_tools/data_lake_facade.py
+-rw-r--r--   0        0        0      115 2024-03-15 09:01:15.880246 airflow_tools-0.7.9/src/airflow_tools/exceptions.py
+-rw-r--r--   0        0        0        0 2024-03-15 09:01:15.880736 airflow_tools-0.7.9/src/airflow_tools/filesystems/__init__.py
+-rw-r--r--   0        0        0     2298 2024-03-15 14:21:53.853567 airflow_tools-0.7.9/src/airflow_tools/filesystems/filesystem_factory.py
+-rw-r--r--   0        0        0      561 2024-03-23 23:14:28.037837 airflow_tools-0.7.9/src/airflow_tools/filesystems/filesystem_protocol.py
+-rw-r--r--   0        0        0        0 2024-03-15 09:01:15.882284 airflow_tools-0.7.9/src/airflow_tools/filesystems/impl/__init__.py
+-rw-r--r--   0        0        0     2162 2024-03-26 13:07:54.227883 airflow_tools-0.7.9/src/airflow_tools/filesystems/impl/azure_databricks_volume_filesystem.py
+-rw-r--r--   0        0        0     1974 2024-03-24 00:50:06.290603 airflow_tools-0.7.9/src/airflow_tools/filesystems/impl/azure_file_share_filesystem.py
+-rw-r--r--   0        0        0     2472 2024-03-25 16:17:00.235954 airflow_tools-0.7.9/src/airflow_tools/filesystems/impl/blob_storage_filesystem.py
+-rw-r--r--   0        0        0     1586 2024-03-24 00:21:54.773711 airflow_tools-0.7.9/src/airflow_tools/filesystems/impl/local_filesystem.py
+-rw-r--r--   0        0        0     2185 2024-03-24 00:50:06.294839 airflow_tools-0.7.9/src/airflow_tools/filesystems/impl/s3_filesystem.py
+-rw-r--r--   0        0        0     1396 2024-03-24 00:21:54.788482 airflow_tools-0.7.9/src/airflow_tools/filesystems/impl/sftp_filesystem.py
+-rw-r--r--   0        0        0     3877 2024-03-15 09:01:15.884092 airflow_tools-0.7.9/src/airflow_tools/notifications/slack/webhook.py
+-rw-r--r--   0        0        0        0 2024-03-15 09:01:15.884537 airflow_tools-0.7.9/src/airflow_tools/providers/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-15 09:01:15.884904 airflow_tools-0.7.9/src/airflow_tools/providers/azure/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-15 09:01:15.885232 airflow_tools-0.7.9/src/airflow_tools/providers/azure/hooks/__init__.py
+-rw-r--r--   0        0        0     3396 2024-03-18 14:38:56.888663 airflow_tools-0.7.9/src/airflow_tools/providers/azure/hooks/azure_databricks.py
+-rw-r--r--   0        0        0     1619 2024-03-15 09:01:15.885704 airflow_tools-0.7.9/src/airflow_tools/providers/azure/hooks/azure_file_share.py
+-rw-r--r--   0        0        0        0 2024-03-15 09:01:15.886187 airflow_tools-0.7.9/src/airflow_tools/providers/data_lake/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-15 09:01:15.886773 airflow_tools-0.7.9/src/airflow_tools/providers/data_lake/operators/__init__.py
+-rw-r--r--   0        0        0     2355 2024-03-23 22:52:20.625836 airflow_tools-0.7.9/src/airflow_tools/providers/data_lake/operators/data_lake.py
+-rw-r--r--   0        0        0        0 2024-03-15 09:01:15.887444 airflow_tools-0.7.9/src/airflow_tools/providers/filesystem/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-15 09:01:15.888053 airflow_tools-0.7.9/src/airflow_tools/providers/filesystem/operators/__init__.py
+-rw-r--r--   0        0        0     5385 2024-03-26 11:53:51.801039 airflow_tools-0.7.9/src/airflow_tools/providers/filesystem/operators/filesystem.py
+-rw-r--r--   0        0        0        0 2024-03-15 09:01:15.890235 airflow_tools-0.7.9/src/airflow_tools/providers/http_to_data_lake/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-15 09:01:15.891091 airflow_tools-0.7.9/src/airflow_tools/providers/http_to_data_lake/operators/__init__.py
+-rw-r--r--   0        0        0     8762 2024-03-24 22:53:13.055997 airflow_tools-0.7.9/src/airflow_tools/providers/http_to_data_lake/operators/http_to_data_lake.py
+-rw-r--r--   0        0        0     1108 2024-03-18 14:38:56.889184 airflow_tools-0.7.9/src/airflow_tools/providers/package.py
+-rw-r--r--   0        0        0        0 2024-03-15 09:01:15.891899 airflow_tools-0.7.9/src/airflow_tools/py.typed
+-rw-r--r--   0        0        0    10150 1970-01-01 00:00:00.000000 airflow_tools-0.7.9/PKG-INFO
```

### Comparing `airflow_tools-0.7.8/LICENSE.txt` & `airflow_tools-0.7.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.7.8/README.md` & `airflow_tools-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.7.8/pyproject.toml` & `airflow_tools-0.7.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "airflow-tools"
-version = "0.7.8"
+version = "0.7.9"
 
 description = ""
 authors = ["Biel Llobera <biel_llobera@dkl.digital>"]
 readme = "README.md"
 include = ["src/airflow_tools"]
 
 [tool.poetry.dependencies]
```

### Comparing `airflow_tools-0.7.8/src/airflow_tools/compression_utils.py` & `airflow_tools-0.7.9/src/airflow_tools/compression_utils.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.7.8/src/airflow_tools/data_lake_facade.py` & `airflow_tools-0.7.9/src/airflow_tools/data_lake_facade.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.7.8/src/airflow_tools/filesystems/filesystem_factory.py` & `airflow_tools-0.7.9/src/airflow_tools/filesystems/filesystem_factory.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.7.8/src/airflow_tools/filesystems/filesystem_protocol.py` & `airflow_tools-0.7.9/src/airflow_tools/filesystems/filesystem_protocol.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.7.8/src/airflow_tools/filesystems/impl/azure_databricks_volume_filesystem.py` & `airflow_tools-0.7.9/src/airflow_tools/filesystems/impl/azure_databricks_volume_filesystem.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 from io import BytesIO
 
+from databricks.sdk.errors.platform import NotFound
 from airflow_tools.filesystems.filesystem_protocol import FilesystemProtocol
 from airflow_tools.providers.azure.hooks.azure_databricks import (
     AzureDatabricksVolumeHook,
 )
 
 logger = logging.getLogger(__file__)
 
@@ -27,15 +28,21 @@
         self.hook.get_conn().files.delete(path)
 
     def create_prefix(self, prefix: str):
         self.hook.get_conn().files.create_directory(prefix)
 
     def delete_prefix(self, prefix: str):
         conn = self.hook.get_conn()
-        for entry in conn.files.list_directory_contents(prefix):
+
+        try:
+            entries = conn.files.list_directory_contents(prefix)
+        except NotFound:
+            return
+
+        for entry in entries:
             if entry.is_directory:
                 self.delete_prefix(entry.path)
             else:
                 conn.files.delete(entry.path)
         conn.files.delete_directory(prefix)
 
     def check_file(self, path: str) -> bool:
@@ -43,17 +50,20 @@
         return bool(
             entry.path == path
             for entry in self.hook.get_conn().files.list_directory_contents(prefix)
             if not entry.is_directory
         )
 
     def check_prefix(self, prefix: str) -> bool:
-        return bool(
-            self.hook.get_conn().files.list_directory_contents(prefix, page_size=1)
-        )
+        try:
+            return bool(
+                self.hook.get_conn().files.list_directory_contents(prefix, page_size=1)
+            )
+        except NotFound:
+            return False
 
     def list_files(self, prefix: str) -> list[str]:
         return [
             entry.path
             for entry in self.hook.get_conn().files.list_directory_contents(prefix)
             if not entry.is_directory
         ]
```

### Comparing `airflow_tools-0.7.8/src/airflow_tools/filesystems/impl/azure_file_share_filesystem.py` & `airflow_tools-0.7.9/src/airflow_tools/filesystems/impl/azure_file_share_filesystem.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.7.8/src/airflow_tools/filesystems/impl/blob_storage_filesystem.py` & `airflow_tools-0.7.9/src/airflow_tools/filesystems/impl/blob_storage_filesystem.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.7.8/src/airflow_tools/filesystems/impl/local_filesystem.py` & `airflow_tools-0.7.9/src/airflow_tools/filesystems/impl/local_filesystem.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.7.8/src/airflow_tools/filesystems/impl/s3_filesystem.py` & `airflow_tools-0.7.9/src/airflow_tools/filesystems/impl/s3_filesystem.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.7.8/src/airflow_tools/filesystems/impl/sftp_filesystem.py` & `airflow_tools-0.7.9/src/airflow_tools/filesystems/impl/sftp_filesystem.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.7.8/src/airflow_tools/notifications/slack/webhook.py` & `airflow_tools-0.7.9/src/airflow_tools/notifications/slack/webhook.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.7.8/src/airflow_tools/providers/azure/hooks/azure_databricks.py` & `airflow_tools-0.7.9/src/airflow_tools/providers/azure/hooks/azure_databricks.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.7.8/src/airflow_tools/providers/azure/hooks/azure_file_share.py` & `airflow_tools-0.7.9/src/airflow_tools/providers/azure/hooks/azure_file_share.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.7.8/src/airflow_tools/providers/data_lake/operators/data_lake.py` & `airflow_tools-0.7.9/src/airflow_tools/providers/data_lake/operators/data_lake.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.7.8/src/airflow_tools/providers/filesystem/operators/filesystem.py` & `airflow_tools-0.7.9/src/airflow_tools/providers/filesystem/operators/filesystem.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.7.8/src/airflow_tools/providers/http_to_data_lake/operators/http_to_data_lake.py` & `airflow_tools-0.7.9/src/airflow_tools/providers/http_to_data_lake/operators/http_to_data_lake.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.7.8/src/airflow_tools/providers/package.py` & `airflow_tools-0.7.9/src/airflow_tools/providers/package.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.7.8/PKG-INFO` & `airflow_tools-0.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-tools
-Version: 0.7.8
+Version: 0.7.9
 Summary: 
 Author: Biel Llobera
 Author-email: biel_llobera@dkl.digital
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: airflow-tools Version: 0.7.8 Summary: Author: Biel
+Metadata-Version: 2.1 Name: airflow-tools Version: 0.7.9 Summary: Author: Biel
 Llobera Author-email: biel_llobera@dkl.digital Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: apache-
 airflow (>=2.8,<3.0) Requires-Dist: apache-airflow-providers-amazon
 (>=8.8.0,<9.0.0) Requires-Dist: apache-airflow-providers-microsoft-azure
 (>=8.0.0,<9.0.0) Requires-Dist: apache-airflow-providers-sftp (>=4.8.1,<5.0.0)
```

