# Comparing `tmp/bigtesty-0.1.0a1.tar.gz` & `tmp/bigtesty-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigtesty-0.1.0a1.tar", last modified: Wed Apr  3 09:49:00 2024, max compression
+gzip compressed data, was "bigtesty-0.1.0a2.tar", last modified: Wed Apr  3 16:55:11 2024, max compression
```

## Comparing `bigtesty-0.1.0a1.tar` & `bigtesty-0.1.0a2.tar`

### file list

```diff
@@ -1,34 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:49:00.975108 bigtesty-0.1.0a1/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-03 09:48:47.000000 bigtesty-0.1.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-03 09:49:00.971108 bigtesty-0.1.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-03 09:48:47.000000 bigtesty-0.1.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:49:00.971108 bigtesty-0.1.0a1/bigtesty/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 09:48:47.000000 bigtesty-0.1.0a1/bigtesty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-03 09:48:47.000000 bigtesty-0.1.0a1/bigtesty/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-03 09:48:47.000000 bigtesty-0.1.0a1/bigtesty/dataset_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-03 09:48:47.000000 bigtesty-0.1.0a1/bigtesty/definition_test_config_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-03 09:48:47.000000 bigtesty-0.1.0a1/bigtesty/definition_test_file_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-03 09:48:47.000000 bigtesty-0.1.0a1/bigtesty/files_loader_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:49:00.971108 bigtesty-0.1.0a1/bigtesty/given/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 09:48:47.000000 bigtesty-0.1.0a1/bigtesty/given/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-03 09:48:47.000000 bigtesty-0.1.0a1/bigtesty/given/insertion_test_data_bigquery.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:49:00.971108 bigtesty-0.1.0a1/bigtesty/infra/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 09:48:47.000000 bigtesty-0.1.0a1/bigtesty/infra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-03 09:48:47.000000 bigtesty-0.1.0a1/bigtesty/infra/create_iac_for_datasets_with_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-03 09:48:47.000000 bigtesty-0.1.0a1/bigtesty/infra/datasets_with_tables_config_file_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-03 09:48:47.000000 bigtesty-0.1.0a1/bigtesty/infra/datasets_with_tables_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-03 09:48:47.000000 bigtesty-0.1.0a1/bigtesty/infra/launch_tests_ephemeral_infra.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-03 09:48:47.000000 bigtesty-0.1.0a1/bigtesty/lambda_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:49:00.971108 bigtesty-0.1.0a1/bigtesty/then/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 09:48:47.000000 bigtesty-0.1.0a1/bigtesty/then/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-04-03 09:48:47.000000 bigtesty-0.1.0a1/bigtesty/then/assertion_and_tests_reports_result.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-03 09:48:47.000000 bigtesty-0.1.0a1/bigtesty/then/failure_test_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:49:00.971108 bigtesty-0.1.0a1/bigtesty.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-03 09:49:00.000000 bigtesty-0.1.0a1/bigtesty.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-03 09:49:00.000000 bigtesty-0.1.0a1/bigtesty.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 09:49:00.000000 bigtesty-0.1.0a1/bigtesty.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-03 09:49:00.000000 bigtesty-0.1.0a1/bigtesty.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-03 09:49:00.000000 bigtesty-0.1.0a1/bigtesty.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 09:49:00.000000 bigtesty-0.1.0a1/bigtesty.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 09:49:00.975108 bigtesty-0.1.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-03 09:48:47.000000 bigtesty-0.1.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:55:11.325067 bigtesty-0.1.0a2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-03 16:54:55.000000 bigtesty-0.1.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-03 16:55:11.325067 bigtesty-0.1.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-03 16:54:55.000000 bigtesty-0.1.0a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:55:11.325067 bigtesty-0.1.0a2/bigtesty/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:54:55.000000 bigtesty-0.1.0a2/bigtesty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-03 16:54:55.000000 bigtesty-0.1.0a2/bigtesty/arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:55:11.325067 bigtesty-0.1.0a2/bigtesty/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:54:55.000000 bigtesty-0.1.0a2/bigtesty/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-03 16:54:55.000000 bigtesty-0.1.0a2/bigtesty/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-03 16:54:55.000000 bigtesty-0.1.0a2/bigtesty/dataset_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-03 16:54:55.000000 bigtesty-0.1.0a2/bigtesty/definition_test_config_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-03 16:54:55.000000 bigtesty-0.1.0a2/bigtesty/definition_test_file_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-03 16:54:55.000000 bigtesty-0.1.0a2/bigtesty/files_loader_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:55:11.325067 bigtesty-0.1.0a2/bigtesty/given/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:54:55.000000 bigtesty-0.1.0a2/bigtesty/given/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-03 16:54:55.000000 bigtesty-0.1.0a2/bigtesty/given/insertion_test_data_bigquery.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:55:11.325067 bigtesty-0.1.0a2/bigtesty/infra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:54:55.000000 bigtesty-0.1.0a2/bigtesty/infra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-03 16:54:55.000000 bigtesty-0.1.0a2/bigtesty/infra/create_iac_for_datasets_with_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-03 16:54:55.000000 bigtesty-0.1.0a2/bigtesty/infra/datasets_with_tables_config_file_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-03 16:54:55.000000 bigtesty-0.1.0a2/bigtesty/infra/datasets_with_tables_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-03 16:54:55.000000 bigtesty-0.1.0a2/bigtesty/infra/launch_tests_ephemeral_infra.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-03 16:54:55.000000 bigtesty-0.1.0a2/bigtesty/lambda_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:55:11.325067 bigtesty-0.1.0a2/bigtesty/then/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:54:55.000000 bigtesty-0.1.0a2/bigtesty/then/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-04-03 16:54:55.000000 bigtesty-0.1.0a2/bigtesty/then/assertion_and_tests_reports_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-03 16:54:55.000000 bigtesty-0.1.0a2/bigtesty/then/failure_test_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:55:11.325067 bigtesty-0.1.0a2/bigtesty.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-03 16:55:11.000000 bigtesty-0.1.0a2/bigtesty.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-03 16:55:11.000000 bigtesty-0.1.0a2/bigtesty.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 16:55:11.000000 bigtesty-0.1.0a2/bigtesty.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-03 16:55:11.000000 bigtesty-0.1.0a2/bigtesty.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-03 16:55:11.000000 bigtesty-0.1.0a2/bigtesty.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 16:55:11.000000 bigtesty-0.1.0a2/bigtesty.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 16:55:11.325067 bigtesty-0.1.0a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-03 16:54:55.000000 bigtesty-0.1.0a2/setup.py
```

### Comparing `bigtesty-0.1.0a1/LICENSE` & `bigtesty-0.1.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `bigtesty-0.1.0a1/PKG-INFO` & `bigtesty-0.1.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigtesty
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: BigTesty is an integration testing framework for BigQuery
 Home-page: https://github.com/tosun-si/bigtesty
 Author: Mazlum TOSUN
 Author-email: mazlum.tosun@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bigtesty-0.1.0a1/README.md` & `bigtesty-0.1.0a2/README.md`

 * *Files identical despite different names*

### Comparing `bigtesty-0.1.0a1/bigtesty/definition_test_config_helper.py` & `bigtesty-0.1.0a2/bigtesty/definition_test_config_helper.py`

 * *Files identical despite different names*

### Comparing `bigtesty-0.1.0a1/bigtesty/given/insertion_test_data_bigquery.py` & `bigtesty-0.1.0a2/bigtesty/given/insertion_test_data_bigquery.py`

 * *Files identical despite different names*

### Comparing `bigtesty-0.1.0a1/bigtesty/infra/create_iac_for_datasets_with_tables.py` & `bigtesty-0.1.0a2/bigtesty/infra/create_iac_for_datasets_with_tables.py`

 * *Files identical despite different names*

### Comparing `bigtesty-0.1.0a1/bigtesty/infra/datasets_with_tables_config_file_loader.py` & `bigtesty-0.1.0a2/bigtesty/infra/datasets_with_tables_config_file_loader.py`

 * *Files identical despite different names*

### Comparing `bigtesty-0.1.0a1/bigtesty/infra/datasets_with_tables_factory.py` & `bigtesty-0.1.0a2/bigtesty/infra/datasets_with_tables_factory.py`

 * *Files identical despite different names*

### Comparing `bigtesty-0.1.0a1/bigtesty/infra/launch_tests_ephemeral_infra.py` & `bigtesty-0.1.0a2/bigtesty/infra/launch_tests_ephemeral_infra.py`

 * *Files identical despite different names*

### Comparing `bigtesty-0.1.0a1/bigtesty/then/assertion_and_tests_reports_result.py` & `bigtesty-0.1.0a2/bigtesty/then/assertion_and_tests_reports_result.py`

 * *Files identical despite different names*

### Comparing `bigtesty-0.1.0a1/bigtesty.egg-info/PKG-INFO` & `bigtesty-0.1.0a2/bigtesty.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigtesty
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: BigTesty is an integration testing framework for BigQuery
 Home-page: https://github.com/tosun-si/bigtesty
 Author: Mazlum TOSUN
 Author-email: mazlum.tosun@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bigtesty-0.1.0a1/bigtesty.egg-info/SOURCES.txt` & `bigtesty-0.1.0a2/bigtesty.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 bigtesty/lambda_functions.py
 bigtesty.egg-info/PKG-INFO
 bigtesty.egg-info/SOURCES.txt
 bigtesty.egg-info/dependency_links.txt
 bigtesty.egg-info/entry_points.txt
 bigtesty.egg-info/requires.txt
 bigtesty.egg-info/top_level.txt
+bigtesty/cli/__init__.py
+bigtesty/cli/main.py
 bigtesty/given/__init__.py
 bigtesty/given/insertion_test_data_bigquery.py
 bigtesty/infra/__init__.py
 bigtesty/infra/create_iac_for_datasets_with_tables.py
 bigtesty/infra/datasets_with_tables_config_file_loader.py
 bigtesty/infra/datasets_with_tables_factory.py
 bigtesty/infra/launch_tests_ephemeral_infra.py
```

### Comparing `bigtesty-0.1.0a1/setup.py` & `bigtesty-0.1.0a2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # The text of the README file
 long_desc = ""
 if os.path.isfile(path):
     long_desc = path.read_text()
 
 setup(
     name="bigtesty",
-    version="0.1.0a1",
+    version="0.1.0a2",
     entry_points='''
         [console_scripts]
         bigtesty=bigtesty.cli.main:run
     ''',
     install_requires=[
         "pulumi-gcp==6.67.0",
         "google-cloud-bigquery==3.7.0",
```

