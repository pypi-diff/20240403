# Comparing `tmp/airflow_tools-0.8.0.tar.gz` & `tmp/airflow_tools-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow_tools-0.8.0.tar", max compression
+gzip compressed data, was "airflow_tools-0.8.1.tar", max compression
```

## Comparing `airflow_tools-0.8.0.tar` & `airflow_tools-0.8.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    11358 2024-02-26 10:29:12.681236 airflow_tools-0.8.0/LICENSE.txt
--rw-r--r--   0        0        0     8788 2024-04-03 08:24:08.137208 airflow_tools-0.8.0/README.md
--rw-r--r--   0        0        0     1312 2024-04-03 09:10:33.612823 airflow_tools-0.8.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-02 17:33:48.422489 airflow_tools-0.8.0/src/airflow_tools/__init__.py
--rw-r--r--   0        0        0       22 2024-04-03 09:10:33.612823 airflow_tools-0.8.0/src/airflow_tools/_version.py
--rw-r--r--   0        0        0     1794 2024-01-18 10:00:14.774290 airflow_tools-0.8.0/src/airflow_tools/compression_utils.py
--rw-r--r--   0        0        0     4426 2024-04-03 08:24:08.197207 airflow_tools-0.8.0/src/airflow_tools/data_lake_facade.py
--rw-r--r--   0        0        0      115 2024-01-03 14:54:38.107397 airflow_tools-0.8.0/src/airflow_tools/exceptions.py
--rw-r--r--   0        0        0        0 2024-02-26 10:29:12.701235 airflow_tools-0.8.0/src/airflow_tools/filesystems/__init__.py
--rw-r--r--   0        0        0     2298 2024-03-20 11:42:50.252535 airflow_tools-0.8.0/src/airflow_tools/filesystems/filesystem_factory.py
--rw-r--r--   0        0        0      561 2024-04-03 08:24:08.209207 airflow_tools-0.8.0/src/airflow_tools/filesystems/filesystem_protocol.py
--rw-r--r--   0        0        0        0 2024-02-26 10:29:12.713235 airflow_tools-0.8.0/src/airflow_tools/filesystems/impl/__init__.py
--rw-r--r--   0        0        0     2169 2024-04-03 08:24:08.209207 airflow_tools-0.8.0/src/airflow_tools/filesystems/impl/azure_databricks_volume_filesystem.py
--rw-r--r--   0        0        0     1974 2024-04-03 08:24:08.213207 airflow_tools-0.8.0/src/airflow_tools/filesystems/impl/azure_file_share_filesystem.py
--rw-r--r--   0        0        0     2472 2024-04-03 08:24:08.213207 airflow_tools-0.8.0/src/airflow_tools/filesystems/impl/blob_storage_filesystem.py
--rw-r--r--   0        0        0     1586 2024-04-03 08:24:08.213207 airflow_tools-0.8.0/src/airflow_tools/filesystems/impl/local_filesystem.py
--rw-r--r--   0        0        0     2185 2024-04-03 08:24:08.213207 airflow_tools-0.8.0/src/airflow_tools/filesystems/impl/s3_filesystem.py
--rw-r--r--   0        0        0     1396 2024-04-03 08:24:08.213207 airflow_tools-0.8.0/src/airflow_tools/filesystems/impl/sftp_filesystem.py
--rw-r--r--   0        0        0     3877 2024-02-26 10:29:12.737235 airflow_tools-0.8.0/src/airflow_tools/notifications/slack/webhook.py
--rw-r--r--   0        0        0        0 2024-01-02 17:33:48.422489 airflow_tools-0.8.0/src/airflow_tools/providers/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 11:42:50.252535 airflow_tools-0.8.0/src/airflow_tools/providers/azure/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 11:42:50.252535 airflow_tools-0.8.0/src/airflow_tools/providers/azure/hooks/__init__.py
--rw-r--r--   0        0        0     3396 2024-03-20 11:42:50.252535 airflow_tools-0.8.0/src/airflow_tools/providers/azure/hooks/azure_databricks.py
--rw-r--r--   0        0        0     1619 2024-03-20 11:42:50.268535 airflow_tools-0.8.0/src/airflow_tools/providers/azure/hooks/azure_file_share.py
--rw-r--r--   0        0        0        0 2024-01-18 10:00:14.774290 airflow_tools-0.8.0/src/airflow_tools/providers/data_lake/__init__.py
--rw-r--r--   0        0        0        0 2024-01-18 10:00:14.774290 airflow_tools-0.8.0/src/airflow_tools/providers/data_lake/operators/__init__.py
--rw-r--r--   0        0        0     2355 2024-04-03 08:24:08.213207 airflow_tools-0.8.0/src/airflow_tools/providers/data_lake/operators/data_lake.py
--rw-r--r--   0        0        0        0 2024-02-26 10:29:12.737235 airflow_tools-0.8.0/src/airflow_tools/providers/filesystem/__init__.py
--rw-r--r--   0        0        0        0 2024-02-26 10:29:12.737235 airflow_tools-0.8.0/src/airflow_tools/providers/filesystem/operators/__init__.py
--rw-r--r--   0        0        0     5437 2024-04-03 08:24:08.225207 airflow_tools-0.8.0/src/airflow_tools/providers/filesystem/operators/filesystem.py
--rw-r--r--   0        0        0     9233 2024-04-03 08:24:08.241207 airflow_tools-0.8.0/src/airflow_tools/providers/filesystem/operators/http_to_filesystem.py
--rw-r--r--   0        0        0        0 2024-01-02 17:33:48.422489 airflow_tools-0.8.0/src/airflow_tools/providers/http_to_data_lake/__init__.py
--rw-r--r--   0        0        0        0 2024-01-02 17:33:48.422489 airflow_tools-0.8.0/src/airflow_tools/providers/http_to_data_lake/operators/__init__.py
--rw-r--r--   0        0        0     9037 2024-04-03 08:24:08.257207 airflow_tools-0.8.0/src/airflow_tools/providers/http_to_data_lake/operators/http_to_data_lake.py
--rw-r--r--   0        0        0     1108 2024-03-20 11:42:50.268535 airflow_tools-0.8.0/src/airflow_tools/providers/package.py
--rw-r--r--   0        0        0        0 2024-01-02 17:33:48.422489 airflow_tools-0.8.0/src/airflow_tools/py.typed
--rw-r--r--   0        0        0    10026 1970-01-01 00:00:00.000000 airflow_tools-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-02-26 10:29:12.681236 airflow_tools-0.8.1/LICENSE.txt
+-rw-r--r--   0        0        0     8788 2024-04-03 08:24:08.137208 airflow_tools-0.8.1/README.md
+-rw-r--r--   0        0        0     1312 2024-04-03 14:37:46.958244 airflow_tools-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-02 17:33:48.422489 airflow_tools-0.8.1/src/airflow_tools/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-03 14:50:25.840684 airflow_tools-0.8.1/src/airflow_tools/_version.py
+-rw-r--r--   0        0        0     1794 2024-01-18 10:00:14.774290 airflow_tools-0.8.1/src/airflow_tools/compression_utils.py
+-rw-r--r--   0        0        0     4426 2024-04-03 08:24:08.197207 airflow_tools-0.8.1/src/airflow_tools/data_lake_facade.py
+-rw-r--r--   0        0        0      115 2024-01-03 14:54:38.107397 airflow_tools-0.8.1/src/airflow_tools/exceptions.py
+-rw-r--r--   0        0        0        0 2024-02-26 10:29:12.701235 airflow_tools-0.8.1/src/airflow_tools/filesystems/__init__.py
+-rw-r--r--   0        0        0     2298 2024-03-20 11:42:50.252535 airflow_tools-0.8.1/src/airflow_tools/filesystems/filesystem_factory.py
+-rw-r--r--   0        0        0      561 2024-04-03 08:24:08.209207 airflow_tools-0.8.1/src/airflow_tools/filesystems/filesystem_protocol.py
+-rw-r--r--   0        0        0        0 2024-02-26 10:29:12.713235 airflow_tools-0.8.1/src/airflow_tools/filesystems/impl/__init__.py
+-rw-r--r--   0        0        0     2382 2024-04-03 14:39:01.369156 airflow_tools-0.8.1/src/airflow_tools/filesystems/impl/azure_databricks_volume_filesystem.py
+-rw-r--r--   0        0        0     1974 2024-04-03 08:24:08.213207 airflow_tools-0.8.1/src/airflow_tools/filesystems/impl/azure_file_share_filesystem.py
+-rw-r--r--   0        0        0     2472 2024-04-03 08:24:08.213207 airflow_tools-0.8.1/src/airflow_tools/filesystems/impl/blob_storage_filesystem.py
+-rw-r--r--   0        0        0     1586 2024-04-03 08:24:08.213207 airflow_tools-0.8.1/src/airflow_tools/filesystems/impl/local_filesystem.py
+-rw-r--r--   0        0        0     2185 2024-04-03 08:24:08.213207 airflow_tools-0.8.1/src/airflow_tools/filesystems/impl/s3_filesystem.py
+-rw-r--r--   0        0        0     1396 2024-04-03 08:24:08.213207 airflow_tools-0.8.1/src/airflow_tools/filesystems/impl/sftp_filesystem.py
+-rw-r--r--   0        0        0     3877 2024-02-26 10:29:12.737235 airflow_tools-0.8.1/src/airflow_tools/notifications/slack/webhook.py
+-rw-r--r--   0        0        0        0 2024-01-02 17:33:48.422489 airflow_tools-0.8.1/src/airflow_tools/providers/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-20 11:42:50.252535 airflow_tools-0.8.1/src/airflow_tools/providers/azure/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-20 11:42:50.252535 airflow_tools-0.8.1/src/airflow_tools/providers/azure/hooks/__init__.py
+-rw-r--r--   0        0        0     3396 2024-03-20 11:42:50.252535 airflow_tools-0.8.1/src/airflow_tools/providers/azure/hooks/azure_databricks.py
+-rw-r--r--   0        0        0     1619 2024-03-20 11:42:50.268535 airflow_tools-0.8.1/src/airflow_tools/providers/azure/hooks/azure_file_share.py
+-rw-r--r--   0        0        0        0 2024-01-18 10:00:14.774290 airflow_tools-0.8.1/src/airflow_tools/providers/data_lake/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-18 10:00:14.774290 airflow_tools-0.8.1/src/airflow_tools/providers/data_lake/operators/__init__.py
+-rw-r--r--   0        0        0     2355 2024-04-03 08:24:08.213207 airflow_tools-0.8.1/src/airflow_tools/providers/data_lake/operators/data_lake.py
+-rw-r--r--   0        0        0        0 2024-02-26 10:29:12.737235 airflow_tools-0.8.1/src/airflow_tools/providers/filesystem/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-26 10:29:12.737235 airflow_tools-0.8.1/src/airflow_tools/providers/filesystem/operators/__init__.py
+-rw-r--r--   0        0        0     5437 2024-04-03 08:24:08.225207 airflow_tools-0.8.1/src/airflow_tools/providers/filesystem/operators/filesystem.py
+-rw-r--r--   0        0        0     9233 2024-04-03 14:35:27.096443 airflow_tools-0.8.1/src/airflow_tools/providers/filesystem/operators/http_to_filesystem.py
+-rw-r--r--   0        0        0        0 2024-01-02 17:33:48.422489 airflow_tools-0.8.1/src/airflow_tools/providers/http_to_data_lake/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-02 17:33:48.422489 airflow_tools-0.8.1/src/airflow_tools/providers/http_to_data_lake/operators/__init__.py
+-rw-r--r--   0        0        0     9037 2024-04-03 08:24:08.257207 airflow_tools-0.8.1/src/airflow_tools/providers/http_to_data_lake/operators/http_to_data_lake.py
+-rw-r--r--   0        0        0     1108 2024-03-20 11:42:50.268535 airflow_tools-0.8.1/src/airflow_tools/providers/package.py
+-rw-r--r--   0        0        0        0 2024-01-02 17:33:48.422489 airflow_tools-0.8.1/src/airflow_tools/py.typed
+-rw-r--r--   0        0        0    10026 1970-01-01 00:00:00.000000 airflow_tools-0.8.1/PKG-INFO
```

### Comparing `airflow_tools-0.8.0/LICENSE.txt` & `airflow_tools-0.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.0/README.md` & `airflow_tools-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.0/pyproject.toml` & `airflow_tools-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "airflow-tools"
-version = "0.8.0"
+version = "0.8.1"
 
 description = ""
 authors = ["Biel Llobera <biel_llobera@dkl.digital>"]
 readme = "README.md"
 include = ["src/airflow_tools"]
 
 [tool.poetry.dependencies]
```

### Comparing `airflow_tools-0.8.0/src/airflow_tools/compression_utils.py` & `airflow_tools-0.8.1/src/airflow_tools/compression_utils.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.0/src/airflow_tools/data_lake_facade.py` & `airflow_tools-0.8.1/src/airflow_tools/data_lake_facade.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.0/src/airflow_tools/filesystems/filesystem_factory.py` & `airflow_tools-0.8.1/src/airflow_tools/filesystems/filesystem_factory.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.0/src/airflow_tools/filesystems/filesystem_protocol.py` & `airflow_tools-0.8.1/src/airflow_tools/filesystems/filesystem_protocol.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.0/src/airflow_tools/filesystems/impl/azure_databricks_volume_filesystem.py` & `airflow_tools-0.8.1/src/airflow_tools/filesystems/impl/azure_databricks_volume_filesystem.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,25 +44,36 @@
                 self.delete_prefix(entry.path)
             else:
                 conn.files.delete(entry.path)
         conn.files.delete_directory(prefix)
 
     def check_file(self, path: str) -> bool:
         prefix = path.rsplit("/", 1)[0]
-        return bool(
-            entry.path == path
-            for entry in self.hook.get_conn().files.list_directory_contents(prefix)
-            if not entry.is_directory
-        )
+
+        try:
+            file_list_path = [
+                entry.path == path
+                for entry in self.hook.get_conn().files.list_directory_contents(prefix)
+                if not entry.is_directory
+            ]
+            return any(file_list_path)
+
+        except NotFound:
+            return False
 
     def check_prefix(self, prefix: str) -> bool:
         try:
-            return bool(
-                self.hook.get_conn().files.list_directory_contents(prefix, page_size=1)
-            )
+            _ = [
+                f
+                for f in self.hook.get_conn().files.list_directory_contents(
+                    prefix, page_size=1
+                )
+            ]
+            return True
+
         except NotFound:
             return False
 
     def list_files(self, prefix: str) -> list[str]:
         return [
             entry.path
             for entry in self.hook.get_conn().files.list_directory_contents(prefix)
```

### Comparing `airflow_tools-0.8.0/src/airflow_tools/filesystems/impl/azure_file_share_filesystem.py` & `airflow_tools-0.8.1/src/airflow_tools/filesystems/impl/azure_file_share_filesystem.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.0/src/airflow_tools/filesystems/impl/blob_storage_filesystem.py` & `airflow_tools-0.8.1/src/airflow_tools/filesystems/impl/blob_storage_filesystem.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.0/src/airflow_tools/filesystems/impl/local_filesystem.py` & `airflow_tools-0.8.1/src/airflow_tools/filesystems/impl/local_filesystem.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.0/src/airflow_tools/filesystems/impl/s3_filesystem.py` & `airflow_tools-0.8.1/src/airflow_tools/filesystems/impl/s3_filesystem.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.0/src/airflow_tools/filesystems/impl/sftp_filesystem.py` & `airflow_tools-0.8.1/src/airflow_tools/filesystems/impl/sftp_filesystem.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.0/src/airflow_tools/notifications/slack/webhook.py` & `airflow_tools-0.8.1/src/airflow_tools/notifications/slack/webhook.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.0/src/airflow_tools/providers/azure/hooks/azure_databricks.py` & `airflow_tools-0.8.1/src/airflow_tools/providers/azure/hooks/azure_databricks.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.0/src/airflow_tools/providers/azure/hooks/azure_file_share.py` & `airflow_tools-0.8.1/src/airflow_tools/providers/azure/hooks/azure_file_share.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.0/src/airflow_tools/providers/data_lake/operators/data_lake.py` & `airflow_tools-0.8.1/src/airflow_tools/providers/data_lake/operators/data_lake.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.0/src/airflow_tools/providers/filesystem/operators/filesystem.py` & `airflow_tools-0.8.1/src/airflow_tools/providers/filesystem/operators/filesystem.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.0/src/airflow_tools/providers/filesystem/operators/http_to_filesystem.py` & `airflow_tools-0.8.1/src/airflow_tools/providers/filesystem/operators/http_to_filesystem.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.0/src/airflow_tools/providers/http_to_data_lake/operators/http_to_data_lake.py` & `airflow_tools-0.8.1/src/airflow_tools/providers/http_to_data_lake/operators/http_to_data_lake.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.0/src/airflow_tools/providers/package.py` & `airflow_tools-0.8.1/src/airflow_tools/providers/package.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.0/PKG-INFO` & `airflow_tools-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-tools
-Version: 0.8.0
+Version: 0.8.1
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
-Metadata-Version: 2.1 Name: airflow-tools Version: 0.8.0 Summary: Author: Biel
+Metadata-Version: 2.1 Name: airflow-tools Version: 0.8.1 Summary: Author: Biel
 Llobera Author-email: biel_llobera@dkl.digital Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: apache-
 airflow (>=2.8,<3.0) Requires-Dist: apache-airflow-providers-amazon
 (>=8.8.0,<9.0.0) Requires-Dist: apache-airflow-providers-microsoft-azure
 (>=8.0.0,<9.0.0) Requires-Dist: apache-airflow-providers-sftp (>=4.8.1,<5.0.0)
```

