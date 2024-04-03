# Comparing `tmp/prophecy-libs-1.8.8.tar.gz` & `tmp/prophecy-libs-1.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prophecy-libs-1.8.8.tar", last modified: Wed Feb 28 07:49:46 2024, max compression
+gzip compressed data, was "prophecy-libs-1.8.9.tar", last modified: Wed Mar  6 13:11:26 2024, max compression
```

## Comparing `prophecy-libs-1.8.8.tar` & `prophecy-libs-1.8.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-02-28 07:49:46.289015 prophecy-libs-1.8.8/
--rw-r--r--   0 jenkins    (109) jenkins    (114)      313 2024-02-28 07:49:46.289015 prophecy-libs-1.8.8/PKG-INFO
--rw-r--r--   0 jenkins    (109) jenkins    (114)       22 2023-03-12 14:51:36.000000 prophecy-libs-1.8.8/README.md
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-02-28 07:49:46.281015 prophecy-libs-1.8.8/prophecy/
--rw-r--r--   0 jenkins    (109) jenkins    (114)        0 2023-03-12 14:51:36.000000 prophecy-libs-1.8.8/prophecy/__init__.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-02-28 07:49:46.281015 prophecy-libs-1.8.8/prophecy/config/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       27 2023-03-12 14:51:36.000000 prophecy-libs-1.8.8/prophecy/config/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     5643 2024-02-28 07:49:44.000000 prophecy-libs-1.8.8/prophecy/config/config_base.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     4442 2023-06-09 08:12:50.000000 prophecy-libs-1.8.8/prophecy/config/utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-02-28 07:49:46.281015 prophecy-libs-1.8.8/prophecy/libs/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       20 2023-03-12 14:51:36.000000 prophecy-libs-1.8.8/prophecy/libs/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     1630 2023-08-26 18:29:07.000000 prophecy-libs-1.8.8/prophecy/libs/utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-02-28 07:49:46.281015 prophecy-libs-1.8.8/prophecy/lookups/
--rw-r--r--   0 jenkins    (109) jenkins    (114)     4678 2023-10-10 05:11:33.000000 prophecy-libs-1.8.8/prophecy/lookups/LookupsBase.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)       27 2023-03-12 14:51:36.000000 prophecy-libs-1.8.8/prophecy/lookups/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     3118 2023-03-12 14:51:36.000000 prophecy-libs-1.8.8/prophecy/random_data_creator.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-02-28 07:49:46.281015 prophecy-libs-1.8.8/prophecy/streaming/
--rw-r--r--   0 jenkins    (109) jenkins    (114)        0 2023-03-12 14:51:36.000000 prophecy-libs-1.8.8/prophecy/streaming/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     5283 2023-03-12 14:51:36.000000 prophecy-libs-1.8.8/prophecy/streaming/delta_lake_utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-02-28 07:49:46.285015 prophecy-libs-1.8.8/prophecy/test/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       30 2023-03-12 14:51:36.000000 prophecy-libs-1.8.8/prophecy/test/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     1944 2023-09-29 15:23:20.000000 prophecy-libs-1.8.8/prophecy/test/base_test_case.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     9645 2023-12-26 06:16:49.000000 prophecy-libs-1.8.8/prophecy/test/utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-02-28 07:49:46.285015 prophecy-libs-1.8.8/prophecy/udfs/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       87 2023-03-12 14:51:36.000000 prophecy-libs-1.8.8/prophecy/udfs/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     2306 2024-02-23 07:14:39.000000 prophecy-libs-1.8.8/prophecy/udfs/rest_api_udf.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)      172 2023-03-12 14:51:36.000000 prophecy-libs-1.8.8/prophecy/udfs/sample_udf.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)      988 2023-05-26 15:20:32.000000 prophecy-libs-1.8.8/prophecy/udfs/scala_udf_wrapper.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-02-28 07:49:46.285015 prophecy-libs-1.8.8/prophecy/utils/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       75 2024-01-25 15:47:15.000000 prophecy-libs-1.8.8/prophecy/utils/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)      303 2024-01-25 15:47:15.000000 prophecy-libs-1.8.8/prophecy/utils/gems_utils.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     2824 2024-01-25 15:47:15.000000 prophecy-libs-1.8.8/prophecy/utils/metagem_utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-02-28 07:49:46.289015 prophecy-libs-1.8.8/prophecy/utils/transpiler/
--rw-r--r--   0 jenkins    (109) jenkins    (114)      143 2023-08-26 18:29:07.000000 prophecy-libs-1.8.8/prophecy/utils/transpiler/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)      789 2023-08-26 18:29:07.000000 prophecy-libs-1.8.8/prophecy/utils/transpiler/abi_base.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)    22842 2023-08-30 12:14:40.000000 prophecy-libs-1.8.8/prophecy/utils/transpiler/abi_core_fcns.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     4406 2024-01-25 15:47:15.000000 prophecy-libs-1.8.8/prophecy/utils/transpiler/abi_fcn_wrapper.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     8387 2023-12-05 10:49:13.000000 prophecy-libs-1.8.8/prophecy/utils/transpiler/dataframe_fcns.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)      692 2023-10-10 05:11:33.000000 prophecy-libs-1.8.8/prophecy/utils/transpiler/dml_schema.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     6399 2023-08-26 18:29:07.000000 prophecy-libs-1.8.8/prophecy/utils/transpiler/fixed_file_schema.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)    29141 2024-02-11 09:01:20.000000 prophecy-libs-1.8.8/prophecy/utils/utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-02-28 07:49:46.289015 prophecy-libs-1.8.8/prophecy_libs.egg-info/
--rw-r--r--   0 jenkins    (109) jenkins    (114)      313 2024-02-28 07:49:46.000000 prophecy-libs-1.8.8/prophecy_libs.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (109) jenkins    (114)     1162 2024-02-28 07:49:46.000000 prophecy-libs-1.8.8/prophecy_libs.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (109) jenkins    (114)        1 2024-02-28 07:49:46.000000 prophecy-libs-1.8.8/prophecy_libs.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (109) jenkins    (114)        1 2023-03-12 14:51:37.000000 prophecy-libs-1.8.8/prophecy_libs.egg-info/not-zip-safe
--rw-r--r--   0 jenkins    (109) jenkins    (114)       33 2024-02-28 07:49:46.000000 prophecy-libs-1.8.8/prophecy_libs.egg-info/requires.txt
--rw-r--r--   0 jenkins    (109) jenkins    (114)        9 2024-02-28 07:49:46.000000 prophecy-libs-1.8.8/prophecy_libs.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (109) jenkins    (114)       38 2024-02-28 07:49:46.289015 prophecy-libs-1.8.8/setup.cfg
--rw-r--r--   0 jenkins    (109) jenkins    (114)      497 2024-02-28 07:49:44.000000 prophecy-libs-1.8.8/setup.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-03-06 13:11:26.285146 prophecy-libs-1.8.9/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      313 2024-03-06 13:11:26.285146 prophecy-libs-1.8.9/PKG-INFO
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       22 2023-03-12 14:51:36.000000 prophecy-libs-1.8.9/README.md
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-03-06 13:11:26.273145 prophecy-libs-1.8.9/prophecy/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        0 2023-03-12 14:51:36.000000 prophecy-libs-1.8.9/prophecy/__init__.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-03-06 13:11:26.273145 prophecy-libs-1.8.9/prophecy/config/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       27 2023-03-12 14:51:36.000000 prophecy-libs-1.8.9/prophecy/config/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     5645 2024-03-06 12:39:38.000000 prophecy-libs-1.8.9/prophecy/config/config_base.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     4442 2023-06-09 08:12:50.000000 prophecy-libs-1.8.9/prophecy/config/utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-03-06 13:11:26.277145 prophecy-libs-1.8.9/prophecy/libs/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       20 2023-03-12 14:51:36.000000 prophecy-libs-1.8.9/prophecy/libs/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     1630 2023-08-26 18:29:07.000000 prophecy-libs-1.8.9/prophecy/libs/utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-03-06 13:11:26.277145 prophecy-libs-1.8.9/prophecy/lookups/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     4678 2023-10-10 05:11:33.000000 prophecy-libs-1.8.9/prophecy/lookups/LookupsBase.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       27 2023-03-12 14:51:36.000000 prophecy-libs-1.8.9/prophecy/lookups/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     3118 2023-03-12 14:51:36.000000 prophecy-libs-1.8.9/prophecy/random_data_creator.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-03-06 13:11:26.277145 prophecy-libs-1.8.9/prophecy/streaming/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        0 2023-03-12 14:51:36.000000 prophecy-libs-1.8.9/prophecy/streaming/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     5283 2023-03-12 14:51:36.000000 prophecy-libs-1.8.9/prophecy/streaming/delta_lake_utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-03-06 13:11:26.277145 prophecy-libs-1.8.9/prophecy/test/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       30 2023-03-12 14:51:36.000000 prophecy-libs-1.8.9/prophecy/test/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     1944 2023-09-29 15:23:20.000000 prophecy-libs-1.8.9/prophecy/test/base_test_case.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     9645 2023-12-26 06:16:49.000000 prophecy-libs-1.8.9/prophecy/test/utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-03-06 13:11:26.281145 prophecy-libs-1.8.9/prophecy/udfs/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       87 2023-03-12 14:51:36.000000 prophecy-libs-1.8.9/prophecy/udfs/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     2306 2024-02-23 07:14:39.000000 prophecy-libs-1.8.9/prophecy/udfs/rest_api_udf.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      172 2023-03-12 14:51:36.000000 prophecy-libs-1.8.9/prophecy/udfs/sample_udf.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      988 2023-05-26 15:20:32.000000 prophecy-libs-1.8.9/prophecy/udfs/scala_udf_wrapper.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-03-06 13:11:26.281145 prophecy-libs-1.8.9/prophecy/utils/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       75 2024-01-25 15:47:15.000000 prophecy-libs-1.8.9/prophecy/utils/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      303 2024-01-25 15:47:15.000000 prophecy-libs-1.8.9/prophecy/utils/gems_utils.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     2824 2024-01-25 15:47:15.000000 prophecy-libs-1.8.9/prophecy/utils/metagem_utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-03-06 13:11:26.285146 prophecy-libs-1.8.9/prophecy/utils/transpiler/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      143 2023-08-26 18:29:07.000000 prophecy-libs-1.8.9/prophecy/utils/transpiler/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      789 2023-08-26 18:29:07.000000 prophecy-libs-1.8.9/prophecy/utils/transpiler/abi_base.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)    22842 2023-08-30 12:14:40.000000 prophecy-libs-1.8.9/prophecy/utils/transpiler/abi_core_fcns.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     4406 2024-01-25 15:47:15.000000 prophecy-libs-1.8.9/prophecy/utils/transpiler/abi_fcn_wrapper.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     8387 2023-12-05 10:49:13.000000 prophecy-libs-1.8.9/prophecy/utils/transpiler/dataframe_fcns.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      692 2023-10-10 05:11:33.000000 prophecy-libs-1.8.9/prophecy/utils/transpiler/dml_schema.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     6399 2023-08-26 18:29:07.000000 prophecy-libs-1.8.9/prophecy/utils/transpiler/fixed_file_schema.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)    29141 2024-02-11 09:01:20.000000 prophecy-libs-1.8.9/prophecy/utils/utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-03-06 13:11:26.285146 prophecy-libs-1.8.9/prophecy_libs.egg-info/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      313 2024-03-06 13:11:26.000000 prophecy-libs-1.8.9/prophecy_libs.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     1162 2024-03-06 13:11:26.000000 prophecy-libs-1.8.9/prophecy_libs.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        1 2024-03-06 13:11:26.000000 prophecy-libs-1.8.9/prophecy_libs.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        1 2023-03-12 14:51:37.000000 prophecy-libs-1.8.9/prophecy_libs.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       33 2024-03-06 13:11:26.000000 prophecy-libs-1.8.9/prophecy_libs.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        9 2024-03-06 13:11:26.000000 prophecy-libs-1.8.9/prophecy_libs.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       38 2024-03-06 13:11:26.285146 prophecy-libs-1.8.9/setup.cfg
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      497 2024-03-06 13:11:25.000000 prophecy-libs-1.8.9/setup.py
```

### Comparing `prophecy-libs-1.8.8/prophecy/config/config_base.py` & `prophecy-libs-1.8.9/prophecy/config/config_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     class SecretValue:
         def __init__(self, prophecy_spark=None, secretScope: str="", secretKey: str="", providerType: str="Databricks", **kwargs):
             self.prophecy_spark = prophecy_spark
             self.secretScope = secretScope
             self.secretKey = secretKey
             self.providerType = providerType
 
-        @lru_cache
+        @lru_cache()
         def __str__(self):
             self.jvm = self.prophecy_spark.sparkContext._jvm
             self.secret_manager = self.jvm.io.prophecy.libs.secrets.ProphecySecrets
             return self.secret_manager.get(self.secretScope, self.secretKey, self.providerType)
 
     def updateSpark(self, spark):
         self.spark = spark
```

### Comparing `prophecy-libs-1.8.8/prophecy/config/utils.py` & `prophecy-libs-1.8.9/prophecy/config/utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.8.8/prophecy/libs/utils.py` & `prophecy-libs-1.8.9/prophecy/libs/utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.8.8/prophecy/lookups/LookupsBase.py` & `prophecy-libs-1.8.9/prophecy/lookups/LookupsBase.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.8.8/prophecy/random_data_creator.py` & `prophecy-libs-1.8.9/prophecy/random_data_creator.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.8.8/prophecy/streaming/delta_lake_utils.py` & `prophecy-libs-1.8.9/prophecy/streaming/delta_lake_utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.8.8/prophecy/test/base_test_case.py` & `prophecy-libs-1.8.9/prophecy/test/base_test_case.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.8.8/prophecy/test/utils.py` & `prophecy-libs-1.8.9/prophecy/test/utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.8.8/prophecy/udfs/rest_api_udf.py` & `prophecy-libs-1.8.9/prophecy/udfs/rest_api_udf.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.8.8/prophecy/udfs/scala_udf_wrapper.py` & `prophecy-libs-1.8.9/prophecy/udfs/scala_udf_wrapper.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.8.8/prophecy/utils/metagem_utils.py` & `prophecy-libs-1.8.9/prophecy/utils/metagem_utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.8.8/prophecy/utils/transpiler/abi_base.py` & `prophecy-libs-1.8.9/prophecy/utils/transpiler/abi_base.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.8.8/prophecy/utils/transpiler/abi_core_fcns.py` & `prophecy-libs-1.8.9/prophecy/utils/transpiler/abi_core_fcns.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.8.8/prophecy/utils/transpiler/abi_fcn_wrapper.py` & `prophecy-libs-1.8.9/prophecy/utils/transpiler/abi_fcn_wrapper.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.8.8/prophecy/utils/transpiler/dataframe_fcns.py` & `prophecy-libs-1.8.9/prophecy/utils/transpiler/dataframe_fcns.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.8.8/prophecy/utils/transpiler/dml_schema.py` & `prophecy-libs-1.8.9/prophecy/utils/transpiler/dml_schema.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.8.8/prophecy/utils/transpiler/fixed_file_schema.py` & `prophecy-libs-1.8.9/prophecy/utils/transpiler/fixed_file_schema.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.8.8/prophecy/utils/utils.py` & `prophecy-libs-1.8.9/prophecy/utils/utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.8.8/prophecy_libs.egg-info/SOURCES.txt` & `prophecy-libs-1.8.9/prophecy_libs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

