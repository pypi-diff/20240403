# Comparing `tmp/arion_library-1.1rc1.dev2.tar.gz` & `tmp/arion_library-1.1rc1.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arion_library-1.1rc1.dev2.tar", last modified: Wed Apr  3 14:36:39 2024, max compression
+gzip compressed data, was "arion_library-1.1rc1.dev3.tar", last modified: Wed Apr  3 16:21:06 2024, max compression
```

## Comparing `arion_library-1.1rc1.dev2.tar` & `arion_library-1.1rc1.dev3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:36:39.672605 arion_library-1.1rc1.dev2/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-03 14:36:39.672605 arion_library-1.1rc1.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-03 14:36:26.000000 arion_library-1.1rc1.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:36:39.668605 arion_library-1.1rc1.dev2/arion_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-03 14:36:39.000000 arion_library-1.1rc1.dev2/arion_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-03 14:36:39.000000 arion_library-1.1rc1.dev2/arion_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 14:36:39.000000 arion_library-1.1rc1.dev2/arion_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-03 14:36:39.000000 arion_library-1.1rc1.dev2/arion_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 14:36:39.000000 arion_library-1.1rc1.dev2/arion_library.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:36:39.668605 arion_library-1.1rc1.dev2/processors/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:36:39.668605 arion_library-1.1rc1.dev2/processors/SFTP/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:36:26.000000 arion_library-1.1rc1.dev2/processors/SFTP/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:36:39.668605 arion_library-1.1rc1.dev2/processors/SFTP/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:36:26.000000 arion_library-1.1rc1.dev2/processors/SFTP/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-03 14:36:26.000000 arion_library-1.1rc1.dev2/processors/SFTP/lib/sftp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:36:39.668605 arion_library-1.1rc1.dev2/processors/TableStorage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:36:26.000000 arion_library-1.1rc1.dev2/processors/TableStorage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:36:39.668605 arion_library-1.1rc1.dev2/processors/TableStorage/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-03 14:36:26.000000 arion_library-1.1rc1.dev2/processors/TableStorage/lib/TableStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:36:26.000000 arion_library-1.1rc1.dev2/processors/TableStorage/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:36:26.000000 arion_library-1.1rc1.dev2/processors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:36:39.668605 arion_library-1.1rc1.dev2/processors/azure_blob_storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:36:26.000000 arion_library-1.1rc1.dev2/processors/azure_blob_storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:36:39.672605 arion_library-1.1rc1.dev2/processors/azure_blob_storage/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:36:26.000000 arion_library-1.1rc1.dev2/processors/azure_blob_storage/lib/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3072 2024-04-03 14:36:26.000000 arion_library-1.1rc1.dev2/processors/azure_blob_storage/lib/azureBlobStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-03 14:36:26.000000 arion_library-1.1rc1.dev2/processors/azure_blob_storage/lib/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:36:39.672605 arion_library-1.1rc1.dev2/processors/azure_blob_storage/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:36:26.000000 arion_library-1.1rc1.dev2/processors/azure_blob_storage/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-03 14:36:26.000000 arion_library-1.1rc1.dev2/processors/azure_blob_storage/tests/test_blob.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-03 14:36:26.000000 arion_library-1.1rc1.dev2/processors/azure_blob_storage/tests/test_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:36:39.672605 arion_library-1.1rc1.dev2/processors/azure_storage_provider/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:36:26.000000 arion_library-1.1rc1.dev2/processors/azure_storage_provider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:36:39.672605 arion_library-1.1rc1.dev2/processors/azure_storage_provider/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:36:26.000000 arion_library-1.1rc1.dev2/processors/azure_storage_provider/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-04-03 14:36:26.000000 arion_library-1.1rc1.dev2/processors/azure_storage_provider/lib/azureBlobStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-04-03 14:36:26.000000 arion_library-1.1rc1.dev2/processors/azure_storage_provider/lib/azureTableStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-03 14:36:26.000000 arion_library-1.1rc1.dev2/processors/azure_storage_provider/lib/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:36:39.672605 arion_library-1.1rc1.dev2/processors/azure_storage_provider/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:36:26.000000 arion_library-1.1rc1.dev2/processors/azure_storage_provider/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-03 14:36:26.000000 arion_library-1.1rc1.dev2/processors/azure_storage_provider/tests/test_blob.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-03 14:36:26.000000 arion_library-1.1rc1.dev2/processors/azure_storage_provider/tests/test_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:36:39.672605 arion_library-1.1rc1.dev2/processors/msserversql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:36:26.000000 arion_library-1.1rc1.dev2/processors/msserversql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:36:39.672605 arion_library-1.1rc1.dev2/processors/msserversql/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-03 14:36:26.000000 arion_library-1.1rc1.dev2/processors/msserversql/lib/MsServerSQL.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:36:26.000000 arion_library-1.1rc1.dev2/processors/msserversql/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:36:39.672605 arion_library-1.1rc1.dev2/processors/msserversql/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:36:26.000000 arion_library-1.1rc1.dev2/processors/msserversql/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-03 14:36:26.000000 arion_library-1.1rc1.dev2/processors/msserversql/tests/test_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-03 14:36:26.000000 arion_library-1.1rc1.dev2/processors/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 14:36:39.672605 arion_library-1.1rc1.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:21:06.710143 arion_library-1.1rc1.dev3/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-03 16:21:06.710143 arion_library-1.1rc1.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 16:20:53.000000 arion_library-1.1rc1.dev3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:21:06.706143 arion_library-1.1rc1.dev3/arion_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-03 16:21:06.000000 arion_library-1.1rc1.dev3/arion_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-03 16:21:06.000000 arion_library-1.1rc1.dev3/arion_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 16:21:06.000000 arion_library-1.1rc1.dev3/arion_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-03 16:21:06.000000 arion_library-1.1rc1.dev3/arion_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 16:21:06.000000 arion_library-1.1rc1.dev3/arion_library.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:21:06.706143 arion_library-1.1rc1.dev3/processors/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:21:06.706143 arion_library-1.1rc1.dev3/processors/SFTP/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:20:53.000000 arion_library-1.1rc1.dev3/processors/SFTP/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:21:06.706143 arion_library-1.1rc1.dev3/processors/SFTP/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:20:53.000000 arion_library-1.1rc1.dev3/processors/SFTP/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-03 16:20:53.000000 arion_library-1.1rc1.dev3/processors/SFTP/lib/sftp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:21:06.706143 arion_library-1.1rc1.dev3/processors/TableStorage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:20:53.000000 arion_library-1.1rc1.dev3/processors/TableStorage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:21:06.706143 arion_library-1.1rc1.dev3/processors/TableStorage/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-03 16:20:53.000000 arion_library-1.1rc1.dev3/processors/TableStorage/lib/TableStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:20:53.000000 arion_library-1.1rc1.dev3/processors/TableStorage/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:20:53.000000 arion_library-1.1rc1.dev3/processors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:21:06.706143 arion_library-1.1rc1.dev3/processors/azure_blob_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:20:53.000000 arion_library-1.1rc1.dev3/processors/azure_blob_storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:21:06.706143 arion_library-1.1rc1.dev3/processors/azure_blob_storage/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:20:53.000000 arion_library-1.1rc1.dev3/processors/azure_blob_storage/lib/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3072 2024-04-03 16:20:53.000000 arion_library-1.1rc1.dev3/processors/azure_blob_storage/lib/azureBlobStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-03 16:20:53.000000 arion_library-1.1rc1.dev3/processors/azure_blob_storage/lib/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:21:06.706143 arion_library-1.1rc1.dev3/processors/azure_blob_storage/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:20:53.000000 arion_library-1.1rc1.dev3/processors/azure_blob_storage/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-03 16:20:53.000000 arion_library-1.1rc1.dev3/processors/azure_blob_storage/tests/test_blob.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-03 16:20:53.000000 arion_library-1.1rc1.dev3/processors/azure_blob_storage/tests/test_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:21:06.706143 arion_library-1.1rc1.dev3/processors/azure_storage_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:20:53.000000 arion_library-1.1rc1.dev3/processors/azure_storage_provider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:21:06.706143 arion_library-1.1rc1.dev3/processors/azure_storage_provider/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:20:53.000000 arion_library-1.1rc1.dev3/processors/azure_storage_provider/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-04-03 16:20:53.000000 arion_library-1.1rc1.dev3/processors/azure_storage_provider/lib/azureBlobStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-04-03 16:20:53.000000 arion_library-1.1rc1.dev3/processors/azure_storage_provider/lib/azureTableStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-03 16:20:53.000000 arion_library-1.1rc1.dev3/processors/azure_storage_provider/lib/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:21:06.710143 arion_library-1.1rc1.dev3/processors/azure_storage_provider/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:20:53.000000 arion_library-1.1rc1.dev3/processors/azure_storage_provider/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-03 16:20:53.000000 arion_library-1.1rc1.dev3/processors/azure_storage_provider/tests/test_blob.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-03 16:20:53.000000 arion_library-1.1rc1.dev3/processors/azure_storage_provider/tests/test_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:21:06.710143 arion_library-1.1rc1.dev3/processors/msserversql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:20:53.000000 arion_library-1.1rc1.dev3/processors/msserversql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:21:06.710143 arion_library-1.1rc1.dev3/processors/msserversql/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-03 16:20:53.000000 arion_library-1.1rc1.dev3/processors/msserversql/lib/MsServerSQL.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:20:53.000000 arion_library-1.1rc1.dev3/processors/msserversql/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:21:06.710143 arion_library-1.1rc1.dev3/processors/msserversql/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:20:53.000000 arion_library-1.1rc1.dev3/processors/msserversql/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-03 16:20:53.000000 arion_library-1.1rc1.dev3/processors/msserversql/tests/test_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-03 16:20:53.000000 arion_library-1.1rc1.dev3/processors/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 16:21:06.710143 arion_library-1.1rc1.dev3/setup.cfg
```

### Comparing `arion_library-1.1rc1.dev2/arion_library.egg-info/SOURCES.txt` & `arion_library-1.1rc1.dev3/arion_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc1.dev2/processors/SFTP/lib/sftp.py` & `arion_library-1.1rc1.dev3/processors/SFTP/lib/sftp.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc1.dev2/processors/TableStorage/lib/TableStorage.py` & `arion_library-1.1rc1.dev3/processors/TableStorage/lib/TableStorage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc1.dev2/processors/azure_blob_storage/lib/azureBlobStorage.py` & `arion_library-1.1rc1.dev3/processors/azure_blob_storage/lib/azureBlobStorage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc1.dev2/processors/azure_blob_storage/lib/config.py` & `arion_library-1.1rc1.dev3/processors/azure_blob_storage/lib/config.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc1.dev2/processors/azure_blob_storage/tests/test_blob.py` & `arion_library-1.1rc1.dev3/processors/azure_blob_storage/tests/test_blob.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc1.dev2/processors/azure_blob_storage/tests/test_env.py` & `arion_library-1.1rc1.dev3/processors/azure_blob_storage/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc1.dev2/processors/azure_storage_provider/lib/azureBlobStorage.py` & `arion_library-1.1rc1.dev3/processors/azure_storage_provider/lib/azureBlobStorage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc1.dev2/processors/azure_storage_provider/lib/azureTableStorage.py` & `arion_library-1.1rc1.dev3/processors/azure_storage_provider/lib/azureTableStorage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc1.dev2/processors/azure_storage_provider/lib/config.py` & `arion_library-1.1rc1.dev3/processors/azure_storage_provider/lib/config.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc1.dev2/processors/azure_storage_provider/tests/test_blob.py` & `arion_library-1.1rc1.dev3/processors/azure_storage_provider/tests/test_blob.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc1.dev2/processors/azure_storage_provider/tests/test_env.py` & `arion_library-1.1rc1.dev3/processors/azure_storage_provider/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc1.dev2/processors/msserversql/lib/MsServerSQL.py` & `arion_library-1.1rc1.dev3/processors/msserversql/lib/MsServerSQL.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc1.dev2/processors/msserversql/tests/test_methods.py` & `arion_library-1.1rc1.dev3/processors/msserversql/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc1.dev2/processors/setup.py` & `arion_library-1.1rc1.dev3/processors/setup.py`

 * *Files identical despite different names*

