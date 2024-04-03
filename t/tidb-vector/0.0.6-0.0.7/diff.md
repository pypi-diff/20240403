# Comparing `tmp/tidb_vector-0.0.6.tar.gz` & `tmp/tidb_vector-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidb_vector-0.0.6.tar", max compression
+gzip compressed data, was "tidb_vector-0.0.7.tar", max compression
```

## Comparing `tidb_vector-0.0.6.tar` & `tidb_vector-0.0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11294 2024-03-04 08:01:44.610607 tidb_vector-0.0.6/LICENSE
--rw-r--r--   0        0        0     4617 2024-03-18 06:08:42.030577 tidb_vector-0.0.6/README.md
--rw-r--r--   0        0        0      821 2024-03-19 06:04:05.079811 tidb_vector-0.0.6/pyproject.toml
--rw-r--r--   0        0        0       22 2024-04-01 08:10:20.248726 tidb_vector-0.0.6/tidb_vector/__init__.py
--rw-r--r--   0        0        0      109 2024-03-14 03:53:20.150919 tidb_vector-0.0.6/tidb_vector/constants.py
--rw-r--r--   0        0        0      356 2024-03-05 22:28:11.819145 tidb_vector-0.0.6/tidb_vector/integrations/__init__.py
--rw-r--r--   0        0        0     3472 2024-04-01 07:50:10.330613 tidb_vector-0.0.6/tidb_vector/integrations/utils.py
--rw-r--r--   0        0        0    18592 2024-04-01 07:50:10.331513 tidb_vector-0.0.6/tidb_vector/integrations/vector_client.py
--rw-r--r--   0        0        0      962 2024-03-14 03:59:19.124632 tidb_vector-0.0.6/tidb_vector/peewee/__init__.py
--rw-r--r--   0        0        0     2775 2024-03-16 06:37:36.615096 tidb_vector-0.0.6/tidb_vector/sqlalchemy/__init__.py
--rw-r--r--   0        0        0      863 2024-03-14 03:59:19.126501 tidb_vector-0.0.6/tidb_vector/utils.py
--rw-r--r--   0        0        0     5254 1970-01-01 00:00:00.000000 tidb_vector-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    11294 2024-03-04 08:01:44.610607 tidb_vector-0.0.7/LICENSE
+-rw-r--r--   0        0        0     4617 2024-03-18 06:08:42.030577 tidb_vector-0.0.7/README.md
+-rw-r--r--   0        0        0      852 2024-04-01 08:18:14.580905 tidb_vector-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-03 09:41:38.451647 tidb_vector-0.0.7/tidb_vector/__init__.py
+-rw-r--r--   0        0        0      109 2024-03-14 03:53:20.150919 tidb_vector-0.0.7/tidb_vector/constants.py
+-rw-r--r--   0        0        0      356 2024-03-05 22:28:11.819145 tidb_vector-0.0.7/tidb_vector/integrations/__init__.py
+-rw-r--r--   0        0        0     3478 2024-04-03 09:40:56.455876 tidb_vector-0.0.7/tidb_vector/integrations/utils.py
+-rw-r--r--   0        0        0    18592 2024-04-01 07:50:10.331513 tidb_vector-0.0.7/tidb_vector/integrations/vector_client.py
+-rw-r--r--   0        0        0      962 2024-03-14 03:59:19.124632 tidb_vector-0.0.7/tidb_vector/peewee/__init__.py
+-rw-r--r--   0        0        0     2775 2024-03-16 06:37:36.615096 tidb_vector-0.0.7/tidb_vector/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      863 2024-03-14 03:59:19.126501 tidb_vector-0.0.7/tidb_vector/utils.py
+-rw-r--r--   0        0        0     5285 1970-01-01 00:00:00.000000 tidb_vector-0.0.7/PKG-INFO
```

### Comparing `tidb_vector-0.0.6/LICENSE` & `tidb_vector-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tidb_vector-0.0.6/README.md` & `tidb_vector-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `tidb_vector-0.0.6/pyproject.toml` & `tidb_vector-0.0.7/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "tidb-vector"
 # this version is usless, now read the version from __init__.py
 version = "0.0.0"
-description = ""
+description = "A Python client for TiDB Vector"
 authors = ["IANTHEREAL <argregoryian@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "tidb_vector"}]
 
 [tool.poetry-version-plugin]
 source = "init"
```

### Comparing `tidb_vector-0.0.6/tidb_vector/integrations/utils.py` & `tidb_vector-0.0.7/tidb_vector/integrations/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
                         WHERE TABLE_NAME = '{table_name}' AND COLUMN_NAME = '{column_name}'"""
             result = connection.execute(sqlalchemy.text(query)).fetchone()
             if result:
                 return extract_info_from_column_definition(result[0], result[1])
     finally:
         engine.dispose()
 
-    return None
+    return None, None
 
 
 def extract_info_from_column_definition(column_type, column_comment):
     """
     Extracts the dimension and distance metric from a column definition,
     supporting both optional dimension and optional comment.
```

### Comparing `tidb_vector-0.0.6/tidb_vector/integrations/vector_client.py` & `tidb_vector-0.0.7/tidb_vector/integrations/vector_client.py`

 * *Files identical despite different names*

### Comparing `tidb_vector-0.0.6/tidb_vector/peewee/__init__.py` & `tidb_vector-0.0.7/tidb_vector/peewee/__init__.py`

 * *Files identical despite different names*

### Comparing `tidb_vector-0.0.6/tidb_vector/sqlalchemy/__init__.py` & `tidb_vector-0.0.7/tidb_vector/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `tidb_vector-0.0.6/tidb_vector/utils.py` & `tidb_vector-0.0.7/tidb_vector/utils.py`

 * *Files identical despite different names*

### Comparing `tidb_vector-0.0.6/PKG-INFO` & `tidb_vector-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: tidb-vector
-Version: 0.0.6
-Summary: 
+Version: 0.0.7
+Summary: A Python client for TiDB Vector
 License: Apache-2.0
 Author: IANTHEREAL
 Author-email: argregoryian@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

