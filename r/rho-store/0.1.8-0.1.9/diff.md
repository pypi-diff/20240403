# Comparing `tmp/rho_store-0.1.8.tar.gz` & `tmp/rho_store-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rho_store-0.1.8.tar", max compression
+gzip compressed data, was "rho_store-0.1.9.tar", max compression
```

## Comparing `rho_store-0.1.8.tar` & `rho_store-0.1.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0       24 2023-12-25 17:13:04.248477 rho_store-0.1.8/README.md
--rw-r--r--   0        0        0      481 2024-02-19 12:35:44.242479 rho_store-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       30 2023-05-30 21:37:44.568387 rho_store-0.1.8/rho_store/__init__.py
--rw-r--r--   0        0        0       50 2023-05-30 13:48:40.365825 rho_store-0.1.8/rho_store/adapters/__init__.py
--rw-r--r--   0        0        0       31 2023-05-28 12:56:48.326331 rho_store-0.1.8/rho_store/adapters/rho_api/__init__.py
--rw-r--r--   0        0        0     4832 2024-02-19 12:19:59.853473 rho_store-0.1.8/rho_store/adapters/rho_api/graphql_adapter.py
--rw-r--r--   0        0        0        0 2023-05-30 13:41:48.563322 rho_store-0.1.8/rho_store/adapters/rho_api/tests/__init__.py
--rw-r--r--   0        0        0     3435 2024-01-06 12:44:03.527794 rho_store-0.1.8/rho_store/adapters/rho_api/tests/test_graphql_adapter_signed_url.py
--rw-r--r--   0        0        0      515 2023-12-28 13:39:11.738602 rho_store-0.1.8/rho_store/adapters/rho_api/utils.py
--rw-r--r--   0        0        0       28 2023-05-28 12:56:48.328015 rho_store-0.1.8/rho_store/adapters/upload_file/__init__.py
--rw-r--r--   0        0        0      997 2023-05-30 14:38:52.357923 rho_store-0.1.8/rho_store/adapters/upload_file/http_adapter.py
--rw-r--r--   0        0        0        0 2023-05-28 13:01:18.867210 rho_store-0.1.8/rho_store/adapters/upload_file/temp/__init__.py
--rw-r--r--   0        0        0     2160 2024-02-19 12:32:33.262591 rho_store-0.1.8/rho_store/client.py
--rw-r--r--   0        0        0      711 2023-12-28 12:56:58.120285 rho_store-0.1.8/rho_store/config.py
--rw-r--r--   0        0        0        0 2023-05-07 09:31:51.724861 rho_store-0.1.8/rho_store/data/__init__.py
--rw-r--r--   0        0        0     2514 2023-03-01 11:56:42.130347 rho_store-0.1.8/rho_store/data/spear_holdings.csv
--rw-r--r--   0        0        0      199 2023-12-28 14:02:10.025307 rho_store-0.1.8/rho_store/exceptions.py
--rw-r--r--   0        0        0      155 2023-05-07 09:33:14.256986 rho_store-0.1.8/rho_store/file_utils.py
--rw-r--r--   0        0        0       48 2023-05-07 09:37:11.867403 rho_store-0.1.8/rho_store/ports/__init__.py
--rw-r--r--   0        0        0      365 2023-05-07 10:48:07.250048 rho_store-0.1.8/rho_store/ports/file_storage_port.py
--rw-r--r--   0        0        0       31 2024-01-06 12:57:21.556449 rho_store-0.1.8/rho_store/types/__init__.py
--rw-r--r--   0        0        0      149 2024-01-06 12:57:10.003498 rho_store-0.1.8/rho_store/types/store_df_result.py
--rw-r--r--   0        0        0        0 2023-05-30 13:44:05.395910 rho_store-0.1.8/rho_store/utils.py
--rw-r--r--   0        0        0      697 1970-01-01 00:00:00.000000 rho_store-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       24 2023-12-25 17:13:04.248477 rho_store-0.1.9/README.md
+-rw-r--r--   0        0        0      504 2024-02-20 06:49:44.461635 rho_store-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       30 2023-05-30 21:37:44.568387 rho_store-0.1.9/rho_store/__init__.py
+-rw-r--r--   0        0        0       50 2023-05-30 13:48:40.365825 rho_store-0.1.9/rho_store/adapters/__init__.py
+-rw-r--r--   0        0        0       31 2023-05-28 12:56:48.326331 rho_store-0.1.9/rho_store/adapters/rho_api/__init__.py
+-rw-r--r--   0        0        0     4832 2024-02-19 12:19:59.853473 rho_store-0.1.9/rho_store/adapters/rho_api/graphql_adapter.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:41:48.563322 rho_store-0.1.9/rho_store/adapters/rho_api/tests/__init__.py
+-rw-r--r--   0        0        0     3435 2024-01-06 12:44:03.527794 rho_store-0.1.9/rho_store/adapters/rho_api/tests/test_graphql_adapter_signed_url.py
+-rw-r--r--   0        0        0      515 2023-12-28 13:39:11.738602 rho_store-0.1.9/rho_store/adapters/rho_api/utils.py
+-rw-r--r--   0        0        0       28 2023-05-28 12:56:48.328015 rho_store-0.1.9/rho_store/adapters/upload_file/__init__.py
+-rw-r--r--   0        0        0      997 2023-05-30 14:38:52.357923 rho_store-0.1.9/rho_store/adapters/upload_file/http_adapter.py
+-rw-r--r--   0        0        0        0 2023-05-28 13:01:18.867210 rho_store-0.1.9/rho_store/adapters/upload_file/temp/__init__.py
+-rw-r--r--   0        0        0     2160 2024-02-19 12:32:33.262591 rho_store-0.1.9/rho_store/client.py
+-rw-r--r--   0        0        0      711 2023-12-28 12:56:58.120285 rho_store-0.1.9/rho_store/config.py
+-rw-r--r--   0        0        0        0 2023-05-07 09:31:51.724861 rho_store-0.1.9/rho_store/data/__init__.py
+-rw-r--r--   0        0        0     2514 2023-03-01 11:56:42.130347 rho_store-0.1.9/rho_store/data/spear_holdings.csv
+-rw-r--r--   0        0        0      199 2023-12-28 14:02:10.025307 rho_store-0.1.9/rho_store/exceptions.py
+-rw-r--r--   0        0        0      155 2023-05-07 09:33:14.256986 rho_store-0.1.9/rho_store/file_utils.py
+-rw-r--r--   0        0        0       48 2023-05-07 09:37:11.867403 rho_store-0.1.9/rho_store/ports/__init__.py
+-rw-r--r--   0        0        0      365 2023-05-07 10:48:07.250048 rho_store-0.1.9/rho_store/ports/file_storage_port.py
+-rw-r--r--   0        0        0       31 2024-01-06 12:57:21.556449 rho_store-0.1.9/rho_store/types/__init__.py
+-rw-r--r--   0        0        0      149 2024-01-06 12:57:10.003498 rho_store-0.1.9/rho_store/types/store_df_result.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:44:05.395910 rho_store-0.1.9/rho_store/utils.py
+-rw-r--r--   0        0        0      742 1970-01-01 00:00:00.000000 rho_store-0.1.9/PKG-INFO
```

### Comparing `rho_store-0.1.8/rho_store/adapters/rho_api/graphql_adapter.py` & `rho_store-0.1.9/rho_store/adapters/rho_api/graphql_adapter.py`

 * *Files identical despite different names*

### Comparing `rho_store-0.1.8/rho_store/adapters/rho_api/tests/test_graphql_adapter_signed_url.py` & `rho_store-0.1.9/rho_store/adapters/rho_api/tests/test_graphql_adapter_signed_url.py`

 * *Files identical despite different names*

### Comparing `rho_store-0.1.8/rho_store/adapters/rho_api/utils.py` & `rho_store-0.1.9/rho_store/adapters/rho_api/utils.py`

 * *Files identical despite different names*

### Comparing `rho_store-0.1.8/rho_store/adapters/upload_file/http_adapter.py` & `rho_store-0.1.9/rho_store/adapters/upload_file/http_adapter.py`

 * *Files identical despite different names*

### Comparing `rho_store-0.1.8/rho_store/client.py` & `rho_store-0.1.9/rho_store/client.py`

 * *Files identical despite different names*

### Comparing `rho_store-0.1.8/rho_store/config.py` & `rho_store-0.1.9/rho_store/config.py`

 * *Files identical despite different names*

### Comparing `rho_store-0.1.8/rho_store/data/spear_holdings.csv` & `rho_store-0.1.9/rho_store/data/spear_holdings.csv`

 * *Files identical despite different names*

### Comparing `rho_store-0.1.8/PKG-INFO` & `rho_store-0.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rho-store
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: Björn Ström
 Author-email: bjornstrom90@gmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -12,13 +12,14 @@
 Requires-Dist: orjson (>=3.9.10,<4.0.0)
 Requires-Dist: pandas (>=2.1.2,<3.0.0)
 Requires-Dist: pyarrow (>=13.0.0,<14.0.0)
 Requires-Dist: pytest (>=7.4.3,<8.0.0)
 Requires-Dist: python-dotenv (==1.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: responses (>=0.23.3,<0.24.0)
+Requires-Dist: setuptools (>=69.1.0,<70.0.0)
 Description-Content-Type: text/markdown
 
 # rho-store
 Python SDK
```

