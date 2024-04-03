# Comparing `tmp/dolbaram-0.2.3.tar.gz` & `tmp/dolbaram-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolbaram-0.2.3.tar", max compression
+gzip compressed data, was "dolbaram-0.2.4.tar", max compression
```

## Comparing `dolbaram-0.2.3.tar` & `dolbaram-0.2.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-12-01 01:21:09.254669 dolbaram-0.2.3/README.md
--rw-r--r--   0        0        0        0 2023-12-01 01:21:09.254618 dolbaram-0.2.3/dolbaram/__init__.py
--rw-r--r--   0        0        0    19428 2024-04-02 23:38:43.175380 dolbaram-0.2.3/dolbaram/dolbaram.py
--rw-r--r--   0        0        0      576 2024-04-02 23:38:55.490756 dolbaram-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      896 1970-01-01 00:00:00.000000 dolbaram-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-12-01 01:21:09.254669 dolbaram-0.2.4/README.md
+-rw-r--r--   0        0        0        0 2023-12-01 01:21:09.254618 dolbaram-0.2.4/dolbaram/__init__.py
+-rw-r--r--   0        0        0    19429 2024-04-02 23:43:43.521505 dolbaram-0.2.4/dolbaram/dolbaram.py
+-rw-r--r--   0        0        0      576 2024-04-02 23:43:43.525003 dolbaram-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      896 1970-01-01 00:00:00.000000 dolbaram-0.2.4/PKG-INFO
```

### Comparing `dolbaram-0.2.3/dolbaram/dolbaram.py` & `dolbaram-0.2.4/dolbaram/dolbaram.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,15 +192,15 @@
         :return:
         '''
         file_prefix = file_prefix if file_prefix else self.DATA_S3_BUCKET_PREFIX
         return self.spark_datasource.add_csv_asset(
             s3_prefix=file_prefix,
             name=file_name,
             header=True,
-            infer_schema=True
+            infer_schema=False
         )
 
     def add_athena_dataset(self,
                            athena_database_name: Optional[str],
                            athena_table_name: Optional[str]) -> TableAsset:
         '''
         add athena table into GX dataset.
```

### Comparing `dolbaram-0.2.3/pyproject.toml` & `dolbaram-0.2.4/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dolbaram"
-version = "0.2.3"
+version = "0.2.4"
 description = ""
 authors = ["Kwangsik Lee <lks21c@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 fire = "^0.4.0"
```

### Comparing `dolbaram-0.2.3/PKG-INFO` & `dolbaram-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolbaram
-Version: 0.2.3
+Version: 0.2.4
 Summary: 
 Author: Kwangsik Lee
 Author-email: lks21c@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

