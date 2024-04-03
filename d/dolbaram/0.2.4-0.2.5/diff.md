# Comparing `tmp/dolbaram-0.2.4.tar.gz` & `tmp/dolbaram-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolbaram-0.2.4.tar", max compression
+gzip compressed data, was "dolbaram-0.2.5.tar", max compression
```

## Comparing `dolbaram-0.2.4.tar` & `dolbaram-0.2.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-12-01 01:21:09.254669 dolbaram-0.2.4/README.md
--rw-r--r--   0        0        0        0 2023-12-01 01:21:09.254618 dolbaram-0.2.4/dolbaram/__init__.py
--rw-r--r--   0        0        0    19429 2024-04-02 23:43:43.521505 dolbaram-0.2.4/dolbaram/dolbaram.py
--rw-r--r--   0        0        0      576 2024-04-02 23:43:43.525003 dolbaram-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      896 1970-01-01 00:00:00.000000 dolbaram-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-12-01 01:21:09.254669 dolbaram-0.2.5/README.md
+-rw-r--r--   0        0        0        0 2023-12-01 01:21:09.254618 dolbaram-0.2.5/dolbaram/__init__.py
+-rw-r--r--   0        0        0    19347 2024-04-02 23:57:02.472195 dolbaram-0.2.5/dolbaram/dolbaram.py
+-rw-r--r--   0        0        0      576 2024-04-02 23:57:02.475254 dolbaram-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      896 1970-01-01 00:00:00.000000 dolbaram-0.2.5/PKG-INFO
```

### Comparing `dolbaram-0.2.4/dolbaram/dolbaram.py` & `dolbaram-0.2.5/dolbaram/dolbaram.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from pprint import pprint
 from typing import Union, List, Optional
 
 from baram.s3_manager import S3Manager
 from great_expectations.checkpoint.types.checkpoint_result import CheckpointResult
 from great_expectations.core import ExpectationSuite, ExpectationConfiguration
 from great_expectations.core import ExpectationSuiteValidationResult
 from great_expectations.core import ExpectationValidationResult
@@ -121,16 +120,14 @@
             connection_string += f'&work_group={athena_workgroup}'
         self.athena_datasource = self.context.sources.add_sql(
             name=self.DATASOURCE_ATHENA_NAME,
             connection_string=connection_string
         )
         self.spark_datasource = self.context.sources.add_or_update_spark_s3(
             name=self.DATASOURCE_S3_SPARK_NAME,
-            header=True,
-            infer_schema=True,
             bucket=self.DATA_S3_BUCKET_NAME,
             boto3_options={}
         )
 
     def make_suite(self, suite_name: str) -> ExpectationSuite:
         '''
         generate GX suite on S3.
```

### Comparing `dolbaram-0.2.4/pyproject.toml` & `dolbaram-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dolbaram"
-version = "0.2.4"
+version = "0.2.5"
 description = ""
 authors = ["Kwangsik Lee <lks21c@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 fire = "^0.4.0"
```

### Comparing `dolbaram-0.2.4/PKG-INFO` & `dolbaram-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolbaram
-Version: 0.2.4
+Version: 0.2.5
 Summary: 
 Author: Kwangsik Lee
 Author-email: lks21c@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

