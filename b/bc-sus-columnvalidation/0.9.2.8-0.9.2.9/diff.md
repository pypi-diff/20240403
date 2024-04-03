# Comparing `tmp/bc_sus_columnvalidation-0.9.2.8.tar.gz` & `tmp/bc_sus_columnvalidation-0.9.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bc_sus_columnvalidation-0.9.2.8.tar", last modified: Wed Apr  3 03:41:40 2024, max compression
+gzip compressed data, was "bc_sus_columnvalidation-0.9.2.9.tar", last modified: Wed Apr  3 10:03:27 2024, max compression
```

## Comparing `bc_sus_columnvalidation-0.9.2.8.tar` & `bc_sus_columnvalidation-0.9.2.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-03 03:41:40.755562 bc_sus_columnvalidation-0.9.2.8/
--rw-r--r--   0 vsts      (1001) docker     (127)      150 2024-04-03 03:41:40.755562 bc_sus_columnvalidation-0.9.2.8/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      855 2024-04-03 03:41:25.000000 bc_sus_columnvalidation-0.9.2.8/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-03 03:41:40.755562 bc_sus_columnvalidation-0.9.2.8/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)      334 2024-04-03 03:41:25.000000 bc_sus_columnvalidation-0.9.2.8/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-03 03:41:40.751562 bc_sus_columnvalidation-0.9.2.8/src/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-03 03:41:40.755562 bc_sus_columnvalidation-0.9.2.8/src/bc_sus_columnvalidation/
--rw-r--r--   0 vsts      (1001) docker     (127)      321 2024-04-03 03:41:25.000000 bc_sus_columnvalidation-0.9.2.8/src/bc_sus_columnvalidation/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-03 03:41:40.755562 bc_sus_columnvalidation-0.9.2.8/src/bc_sus_columnvalidation/validation_scripts/
--rw-r--r--   0 vsts      (1001) docker     (127)      234 2024-04-03 03:41:25.000000 bc_sus_columnvalidation-0.9.2.8/src/bc_sus_columnvalidation/validation_scripts/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1002 2024-04-03 03:41:25.000000 bc_sus_columnvalidation-0.9.2.8/src/bc_sus_columnvalidation/validation_scripts/datatype_check_bool.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1127 2024-04-03 03:41:25.000000 bc_sus_columnvalidation-0.9.2.8/src/bc_sus_columnvalidation/validation_scripts/datatype_check_date.py
--rw-r--r--   0 vsts      (1001) docker     (127)      839 2024-04-03 03:41:25.000000 bc_sus_columnvalidation-0.9.2.8/src/bc_sus_columnvalidation/validation_scripts/datatype_check_integer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6688 2024-04-03 03:41:25.000000 bc_sus_columnvalidation-0.9.2.8/src/bc_sus_columnvalidation/validation_scripts/master_data_check.py
--rw-r--r--   0 vsts      (1001) docker     (127)      444 2024-04-03 03:41:25.000000 bc_sus_columnvalidation-0.9.2.8/src/bc_sus_columnvalidation/validation_scripts/missing_data_check.py
--rw-r--r--   0 vsts      (1001) docker     (127)      466 2024-04-03 03:41:25.000000 bc_sus_columnvalidation-0.9.2.8/src/bc_sus_columnvalidation/validation_scripts/primary_key_check.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1057 2024-04-03 03:41:25.000000 bc_sus_columnvalidation-0.9.2.8/src/bc_sus_columnvalidation/validation_scripts/value_restriction_check.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-03 03:41:40.755562 bc_sus_columnvalidation-0.9.2.8/src/bc_sus_columnvalidation.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)      150 2024-04-03 03:41:40.000000 bc_sus_columnvalidation-0.9.2.8/src/bc_sus_columnvalidation.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      876 2024-04-03 03:41:40.000000 bc_sus_columnvalidation-0.9.2.8/src/bc_sus_columnvalidation.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-03 03:41:40.000000 bc_sus_columnvalidation-0.9.2.8/src/bc_sus_columnvalidation.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       16 2024-04-03 03:41:40.000000 bc_sus_columnvalidation-0.9.2.8/src/bc_sus_columnvalidation.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       24 2024-04-03 03:41:40.000000 bc_sus_columnvalidation-0.9.2.8/src/bc_sus_columnvalidation.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-03 03:41:40.755562 bc_sus_columnvalidation-0.9.2.8/test/
--rw-r--r--   0 vsts      (1001) docker     (127)     8852 2024-04-03 03:41:25.000000 bc_sus_columnvalidation-0.9.2.8/test/test.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-03 10:03:27.392472 bc_sus_columnvalidation-0.9.2.9/
+-rw-r--r--   0 vsts      (1001) docker     (127)      150 2024-04-03 10:03:27.392472 bc_sus_columnvalidation-0.9.2.9/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      855 2024-04-03 10:03:03.000000 bc_sus_columnvalidation-0.9.2.9/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-03 10:03:27.392472 bc_sus_columnvalidation-0.9.2.9/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)      334 2024-04-03 10:03:03.000000 bc_sus_columnvalidation-0.9.2.9/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-03 10:03:27.388472 bc_sus_columnvalidation-0.9.2.9/src/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-03 10:03:27.388472 bc_sus_columnvalidation-0.9.2.9/src/bc_sus_columnvalidation/
+-rw-r--r--   0 vsts      (1001) docker     (127)      321 2024-04-03 10:03:03.000000 bc_sus_columnvalidation-0.9.2.9/src/bc_sus_columnvalidation/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-03 10:03:27.392472 bc_sus_columnvalidation-0.9.2.9/src/bc_sus_columnvalidation/validation_scripts/
+-rw-r--r--   0 vsts      (1001) docker     (127)      234 2024-04-03 10:03:03.000000 bc_sus_columnvalidation-0.9.2.9/src/bc_sus_columnvalidation/validation_scripts/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1002 2024-04-03 10:03:03.000000 bc_sus_columnvalidation-0.9.2.9/src/bc_sus_columnvalidation/validation_scripts/datatype_check_bool.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1127 2024-04-03 10:03:03.000000 bc_sus_columnvalidation-0.9.2.9/src/bc_sus_columnvalidation/validation_scripts/datatype_check_date.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      839 2024-04-03 10:03:03.000000 bc_sus_columnvalidation-0.9.2.9/src/bc_sus_columnvalidation/validation_scripts/datatype_check_integer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6712 2024-04-03 10:03:03.000000 bc_sus_columnvalidation-0.9.2.9/src/bc_sus_columnvalidation/validation_scripts/master_data_check.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      444 2024-04-03 10:03:03.000000 bc_sus_columnvalidation-0.9.2.9/src/bc_sus_columnvalidation/validation_scripts/missing_data_check.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      466 2024-04-03 10:03:03.000000 bc_sus_columnvalidation-0.9.2.9/src/bc_sus_columnvalidation/validation_scripts/primary_key_check.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1057 2024-04-03 10:03:03.000000 bc_sus_columnvalidation-0.9.2.9/src/bc_sus_columnvalidation/validation_scripts/value_restriction_check.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-03 10:03:27.392472 bc_sus_columnvalidation-0.9.2.9/src/bc_sus_columnvalidation.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)      150 2024-04-03 10:03:27.000000 bc_sus_columnvalidation-0.9.2.9/src/bc_sus_columnvalidation.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      876 2024-04-03 10:03:27.000000 bc_sus_columnvalidation-0.9.2.9/src/bc_sus_columnvalidation.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-03 10:03:27.000000 bc_sus_columnvalidation-0.9.2.9/src/bc_sus_columnvalidation.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       16 2024-04-03 10:03:27.000000 bc_sus_columnvalidation-0.9.2.9/src/bc_sus_columnvalidation.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       24 2024-04-03 10:03:27.000000 bc_sus_columnvalidation-0.9.2.9/src/bc_sus_columnvalidation.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-03 10:03:27.392472 bc_sus_columnvalidation-0.9.2.9/test/
+-rw-r--r--   0 vsts      (1001) docker     (127)     8852 2024-04-03 10:03:03.000000 bc_sus_columnvalidation-0.9.2.9/test/test.py
```

### Comparing `bc_sus_columnvalidation-0.9.2.8/README.md` & `bc_sus_columnvalidation-0.9.2.9/README.md`

 * *Files identical despite different names*

### Comparing `bc_sus_columnvalidation-0.9.2.8/src/bc_sus_columnvalidation/validation_scripts/datatype_check_bool.py` & `bc_sus_columnvalidation-0.9.2.9/src/bc_sus_columnvalidation/validation_scripts/datatype_check_bool.py`

 * *Files identical despite different names*

### Comparing `bc_sus_columnvalidation-0.9.2.8/src/bc_sus_columnvalidation/validation_scripts/datatype_check_date.py` & `bc_sus_columnvalidation-0.9.2.9/src/bc_sus_columnvalidation/validation_scripts/datatype_check_date.py`

 * *Files identical despite different names*

### Comparing `bc_sus_columnvalidation-0.9.2.8/src/bc_sus_columnvalidation/validation_scripts/datatype_check_integer.py` & `bc_sus_columnvalidation-0.9.2.9/src/bc_sus_columnvalidation/validation_scripts/datatype_check_integer.py`

 * *Files identical despite different names*

### Comparing `bc_sus_columnvalidation-0.9.2.8/src/bc_sus_columnvalidation/validation_scripts/master_data_check.py` & `bc_sus_columnvalidation-0.9.2.9/src/bc_sus_columnvalidation/validation_scripts/master_data_check.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
             "No of rows failed": len(wrong_master_data_rows),
             "rows_which_failed": wrong_master_data_rows,
         }
     elif "BC Farmer" in excel_df and lookup_column_name == "FARMER_CODE":
         # for the case where we need to check farmer code in master data only if they are BC Farmers.
         master_data_column_df = master_df[lookup_column_name]
         excel_df = excel_df[excel_df["BC Farmer"] == True]
-        bc_farmer_excel_filter_df = excel_df[excel_column_name]
+        bc_farmer_excel_filter_df = excel_df[excel_column_name].astype(str)
 
         def lowercase_if_string(value):
             if isinstance(value, str):
                 return value.lower()
             return value
 
         # check for and filter for empty strings, null values in excel and master data column df
@@ -117,15 +117,15 @@
         return {
             "No of rows failed": len(wrong_master_data_rows),
             "rows_which_failed": wrong_master_data_rows,
         }
 
     else:
         master_data_column_df = master_df[lookup_column_name]
-        column_df = excel_df[excel_column_name]
+        column_df = excel_df[excel_column_name].astype(str)
 
         def lowercase_if_string(value):
             if isinstance(value, str):
                 return value.lower()
             return value
 
         # check for and filter for empty strings, null values in excel and master data column df
```

### Comparing `bc_sus_columnvalidation-0.9.2.8/src/bc_sus_columnvalidation/validation_scripts/value_restriction_check.py` & `bc_sus_columnvalidation-0.9.2.9/src/bc_sus_columnvalidation/validation_scripts/value_restriction_check.py`

 * *Files identical despite different names*

### Comparing `bc_sus_columnvalidation-0.9.2.8/src/bc_sus_columnvalidation.egg-info/SOURCES.txt` & `bc_sus_columnvalidation-0.9.2.9/src/bc_sus_columnvalidation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bc_sus_columnvalidation-0.9.2.8/test/test.py` & `bc_sus_columnvalidation-0.9.2.9/test/test.py`

 * *Files identical despite different names*

