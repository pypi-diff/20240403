# Comparing `tmp/dolbaram-0.2.2.tar.gz` & `tmp/dolbaram-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolbaram-0.2.2.tar", max compression
+gzip compressed data, was "dolbaram-0.2.3.tar", max compression
```

## Comparing `dolbaram-0.2.2.tar` & `dolbaram-0.2.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-12-01 01:21:09.254669 dolbaram-0.2.2/README.md
--rw-r--r--   0        0        0        0 2023-12-01 01:21:09.254618 dolbaram-0.2.2/dolbaram/__init__.py
--rw-r--r--   0        0        0    19348 2024-04-02 06:09:01.338454 dolbaram-0.2.2/dolbaram/dolbaram.py
--rw-r--r--   0        0        0      576 2024-04-02 06:09:01.341018 dolbaram-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      896 1970-01-01 00:00:00.000000 dolbaram-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-12-01 01:21:09.254669 dolbaram-0.2.3/README.md
+-rw-r--r--   0        0        0        0 2023-12-01 01:21:09.254618 dolbaram-0.2.3/dolbaram/__init__.py
+-rw-r--r--   0        0        0    19428 2024-04-02 23:38:43.175380 dolbaram-0.2.3/dolbaram/dolbaram.py
+-rw-r--r--   0        0        0      576 2024-04-02 23:38:55.490756 dolbaram-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      896 1970-01-01 00:00:00.000000 dolbaram-0.2.3/PKG-INFO
```

### Comparing `dolbaram-0.2.2/dolbaram/dolbaram.py` & `dolbaram-0.2.3/dolbaram/dolbaram.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,19 @@
         if athena_workgroup:
             connection_string += f'&work_group={athena_workgroup}'
         self.athena_datasource = self.context.sources.add_sql(
             name=self.DATASOURCE_ATHENA_NAME,
             connection_string=connection_string
         )
         self.spark_datasource = self.context.sources.add_or_update_spark_s3(
-            name=self.DATASOURCE_S3_SPARK_NAME, bucket=self.DATA_S3_BUCKET_NAME, boto3_options={}
+            name=self.DATASOURCE_S3_SPARK_NAME,
+            header=True,
+            infer_schema=True,
+            bucket=self.DATA_S3_BUCKET_NAME,
+            boto3_options={}
         )
 
     def make_suite(self, suite_name: str) -> ExpectationSuite:
         '''
         generate GX suite on S3.
 
         :param suite_name: suite name
```

### Comparing `dolbaram-0.2.2/pyproject.toml` & `dolbaram-0.2.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dolbaram"
-version = "0.2.2"
+version = "0.2.3"
 description = ""
 authors = ["Kwangsik Lee <lks21c@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 fire = "^0.4.0"
```

### Comparing `dolbaram-0.2.2/PKG-INFO` & `dolbaram-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolbaram
-Version: 0.2.2
+Version: 0.2.3
 Summary: 
 Author: Kwangsik Lee
 Author-email: lks21c@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

