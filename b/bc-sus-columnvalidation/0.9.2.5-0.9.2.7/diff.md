# Comparing `tmp/bc_sus_columnvalidation-0.9.2.5.tar.gz` & `tmp/bc_sus_columnvalidation-0.9.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bc_sus_columnvalidation-0.9.2.5.tar", last modified: Mon Apr  1 09:09:53 2024, max compression
+gzip compressed data, was "bc_sus_columnvalidation-0.9.2.7.tar", last modified: Wed Apr  3 02:21:49 2024, max compression
```

## Comparing `bc_sus_columnvalidation-0.9.2.5.tar` & `bc_sus_columnvalidation-0.9.2.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 09:09:53.335894 bc_sus_columnvalidation-0.9.2.5/
--rw-r--r--   0 vsts      (1001) docker     (127)      150 2024-04-01 09:09:53.335894 bc_sus_columnvalidation-0.9.2.5/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      855 2024-04-01 09:09:37.000000 bc_sus_columnvalidation-0.9.2.5/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-01 09:09:53.335894 bc_sus_columnvalidation-0.9.2.5/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)      334 2024-04-01 09:09:37.000000 bc_sus_columnvalidation-0.9.2.5/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 09:09:53.331894 bc_sus_columnvalidation-0.9.2.5/src/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 09:09:53.335894 bc_sus_columnvalidation-0.9.2.5/src/bc_sus_columnvalidation/
--rw-r--r--   0 vsts      (1001) docker     (127)      321 2024-04-01 09:09:37.000000 bc_sus_columnvalidation-0.9.2.5/src/bc_sus_columnvalidation/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 09:09:53.335894 bc_sus_columnvalidation-0.9.2.5/src/bc_sus_columnvalidation/validation_scripts/
--rw-r--r--   0 vsts      (1001) docker     (127)      234 2024-04-01 09:09:37.000000 bc_sus_columnvalidation-0.9.2.5/src/bc_sus_columnvalidation/validation_scripts/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      995 2024-04-01 09:09:37.000000 bc_sus_columnvalidation-0.9.2.5/src/bc_sus_columnvalidation/validation_scripts/datatype_check_bool.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1127 2024-04-01 09:09:37.000000 bc_sus_columnvalidation-0.9.2.5/src/bc_sus_columnvalidation/validation_scripts/datatype_check_date.py
--rw-r--r--   0 vsts      (1001) docker     (127)      829 2024-04-01 09:09:37.000000 bc_sus_columnvalidation-0.9.2.5/src/bc_sus_columnvalidation/validation_scripts/datatype_check_integer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6688 2024-04-01 09:09:37.000000 bc_sus_columnvalidation-0.9.2.5/src/bc_sus_columnvalidation/validation_scripts/master_data_check.py
--rw-r--r--   0 vsts      (1001) docker     (127)      514 2024-04-01 09:09:37.000000 bc_sus_columnvalidation-0.9.2.5/src/bc_sus_columnvalidation/validation_scripts/missing_data_check.py
--rw-r--r--   0 vsts      (1001) docker     (127)      466 2024-04-01 09:09:37.000000 bc_sus_columnvalidation-0.9.2.5/src/bc_sus_columnvalidation/validation_scripts/primary_key_check.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1057 2024-04-01 09:09:37.000000 bc_sus_columnvalidation-0.9.2.5/src/bc_sus_columnvalidation/validation_scripts/value_restriction_check.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 09:09:53.335894 bc_sus_columnvalidation-0.9.2.5/src/bc_sus_columnvalidation.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)      150 2024-04-01 09:09:53.000000 bc_sus_columnvalidation-0.9.2.5/src/bc_sus_columnvalidation.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      876 2024-04-01 09:09:53.000000 bc_sus_columnvalidation-0.9.2.5/src/bc_sus_columnvalidation.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-01 09:09:53.000000 bc_sus_columnvalidation-0.9.2.5/src/bc_sus_columnvalidation.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       16 2024-04-01 09:09:53.000000 bc_sus_columnvalidation-0.9.2.5/src/bc_sus_columnvalidation.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       24 2024-04-01 09:09:53.000000 bc_sus_columnvalidation-0.9.2.5/src/bc_sus_columnvalidation.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 09:09:53.335894 bc_sus_columnvalidation-0.9.2.5/test/
--rw-r--r--   0 vsts      (1001) docker     (127)     8852 2024-04-01 09:09:37.000000 bc_sus_columnvalidation-0.9.2.5/test/test.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-03 02:21:49.918458 bc_sus_columnvalidation-0.9.2.7/
+-rw-r--r--   0 vsts      (1001) docker     (127)      150 2024-04-03 02:21:49.918458 bc_sus_columnvalidation-0.9.2.7/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      855 2024-04-03 02:21:34.000000 bc_sus_columnvalidation-0.9.2.7/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-03 02:21:49.918458 bc_sus_columnvalidation-0.9.2.7/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)      334 2024-04-03 02:21:34.000000 bc_sus_columnvalidation-0.9.2.7/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-03 02:21:49.914457 bc_sus_columnvalidation-0.9.2.7/src/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-03 02:21:49.914457 bc_sus_columnvalidation-0.9.2.7/src/bc_sus_columnvalidation/
+-rw-r--r--   0 vsts      (1001) docker     (127)      321 2024-04-03 02:21:34.000000 bc_sus_columnvalidation-0.9.2.7/src/bc_sus_columnvalidation/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-03 02:21:49.918458 bc_sus_columnvalidation-0.9.2.7/src/bc_sus_columnvalidation/validation_scripts/
+-rw-r--r--   0 vsts      (1001) docker     (127)      234 2024-04-03 02:21:34.000000 bc_sus_columnvalidation-0.9.2.7/src/bc_sus_columnvalidation/validation_scripts/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1002 2024-04-03 02:21:34.000000 bc_sus_columnvalidation-0.9.2.7/src/bc_sus_columnvalidation/validation_scripts/datatype_check_bool.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1127 2024-04-03 02:21:34.000000 bc_sus_columnvalidation-0.9.2.7/src/bc_sus_columnvalidation/validation_scripts/datatype_check_date.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      839 2024-04-03 02:21:34.000000 bc_sus_columnvalidation-0.9.2.7/src/bc_sus_columnvalidation/validation_scripts/datatype_check_integer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6688 2024-04-03 02:21:34.000000 bc_sus_columnvalidation-0.9.2.7/src/bc_sus_columnvalidation/validation_scripts/master_data_check.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      522 2024-04-03 02:21:34.000000 bc_sus_columnvalidation-0.9.2.7/src/bc_sus_columnvalidation/validation_scripts/missing_data_check.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      466 2024-04-03 02:21:34.000000 bc_sus_columnvalidation-0.9.2.7/src/bc_sus_columnvalidation/validation_scripts/primary_key_check.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1057 2024-04-03 02:21:34.000000 bc_sus_columnvalidation-0.9.2.7/src/bc_sus_columnvalidation/validation_scripts/value_restriction_check.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-03 02:21:49.918458 bc_sus_columnvalidation-0.9.2.7/src/bc_sus_columnvalidation.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)      150 2024-04-03 02:21:49.000000 bc_sus_columnvalidation-0.9.2.7/src/bc_sus_columnvalidation.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      876 2024-04-03 02:21:49.000000 bc_sus_columnvalidation-0.9.2.7/src/bc_sus_columnvalidation.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-03 02:21:49.000000 bc_sus_columnvalidation-0.9.2.7/src/bc_sus_columnvalidation.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       16 2024-04-03 02:21:49.000000 bc_sus_columnvalidation-0.9.2.7/src/bc_sus_columnvalidation.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       24 2024-04-03 02:21:49.000000 bc_sus_columnvalidation-0.9.2.7/src/bc_sus_columnvalidation.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-03 02:21:49.918458 bc_sus_columnvalidation-0.9.2.7/test/
+-rw-r--r--   0 vsts      (1001) docker     (127)     8852 2024-04-03 02:21:34.000000 bc_sus_columnvalidation-0.9.2.7/test/test.py
```

### Comparing `bc_sus_columnvalidation-0.9.2.5/README.md` & `bc_sus_columnvalidation-0.9.2.7/README.md`

 * *Files identical despite different names*

### Comparing `bc_sus_columnvalidation-0.9.2.5/src/bc_sus_columnvalidation/validation_scripts/datatype_check_bool.py` & `bc_sus_columnvalidation-0.9.2.7/src/bc_sus_columnvalidation/validation_scripts/datatype_check_bool.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         # if not then check if it is a string. It could be "true"/"false"
         # convert to lower and check
         if isinstance(value, str):
             return value.lower() in ["true", "false"]
         # everything else is a fail case
         return False
 
-    non_missing_df = column_df.dropna()  # drop empty values
+    non_missing_df = column_df[column_df != ""] # drop empty values
     # column_df = column_df == 1.0
 
     non_bool_mask = ~non_missing_df.apply(is_bool)
 
     non_bool_rows = non_missing_df[non_bool_mask]
 
     if non_bool_rows.empty:
```

### Comparing `bc_sus_columnvalidation-0.9.2.5/src/bc_sus_columnvalidation/validation_scripts/datatype_check_date.py` & `bc_sus_columnvalidation-0.9.2.7/src/bc_sus_columnvalidation/validation_scripts/datatype_check_date.py`

 * *Files identical despite different names*

### Comparing `bc_sus_columnvalidation-0.9.2.5/src/bc_sus_columnvalidation/validation_scripts/datatype_check_integer.py` & `bc_sus_columnvalidation-0.9.2.7/src/bc_sus_columnvalidation/validation_scripts/datatype_check_integer.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 def datatype_check_integer(column_df):
     def is_integer(value):
         try:
             return float(value).is_integer()
         except ValueError:
             return False
 
-    non_missing_df = column_df.dropna()
+    non_missing_df = column_df[column_df != ""]
 
     non_integer_mask = ~non_missing_df.apply(is_integer)
     # get a list as o/p with the datatype check result(True or false); invert it;
     #  filter the column with that mask and get the failed row indices alone
 
     non_integer_rows = non_missing_df[non_integer_mask]
 
     if non_integer_rows.empty:
         return True
     non_integer_row_numbers = non_integer_rows.index.tolist()
     non_integer_row_numbers = [x + 2 for x in non_integer_row_numbers]
     return {
         "No of rows failed": len(non_integer_row_numbers),
         "rows_which_failed": non_integer_row_numbers,
-    }
+    }
+
```

### Comparing `bc_sus_columnvalidation-0.9.2.5/src/bc_sus_columnvalidation/validation_scripts/master_data_check.py` & `bc_sus_columnvalidation-0.9.2.7/src/bc_sus_columnvalidation/validation_scripts/master_data_check.py`

 * *Files identical despite different names*

### Comparing `bc_sus_columnvalidation-0.9.2.5/src/bc_sus_columnvalidation/validation_scripts/missing_data_check.py` & `bc_sus_columnvalidation-0.9.2.7/src/bc_sus_columnvalidation/validation_scripts/missing_data_check.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import pandas as pd
 
 
 def missing_data_check(column_df):
 
     
-    missing_data = column_df.isnull()
+    missing_data = column_df[column_df != ""]
 
     if missing_data.any():
 
         missing_rows = missing_data[missing_data].index.tolist()
 
         missing_count = missing_data.sum()
```

### Comparing `bc_sus_columnvalidation-0.9.2.5/src/bc_sus_columnvalidation/validation_scripts/value_restriction_check.py` & `bc_sus_columnvalidation-0.9.2.7/src/bc_sus_columnvalidation/validation_scripts/value_restriction_check.py`

 * *Files identical despite different names*

### Comparing `bc_sus_columnvalidation-0.9.2.5/src/bc_sus_columnvalidation.egg-info/SOURCES.txt` & `bc_sus_columnvalidation-0.9.2.7/src/bc_sus_columnvalidation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bc_sus_columnvalidation-0.9.2.5/test/test.py` & `bc_sus_columnvalidation-0.9.2.7/test/test.py`

 * *Files identical despite different names*

