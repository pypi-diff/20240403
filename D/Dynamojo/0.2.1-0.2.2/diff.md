# Comparing `tmp/dynamojo-0.2.1.tar.gz` & `tmp/dynamojo-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamojo-0.2.1.tar", max compression
+gzip compressed data, was "dynamojo-0.2.2.tar", max compression
```

## Comparing `dynamojo-0.2.1.tar` & `dynamojo-0.2.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     4181 2024-03-28 19:01:25.019286 dynamojo-0.2.1/README.md
--rw-r--r--   0        0        0      449 2024-03-28 19:01:25.019636 dynamojo-0.2.1/dynamojo/__init__.py
--rwxr-xr-x   0        0        0    19880 2024-03-28 19:01:25.019853 dynamojo-0.2.1/dynamojo/base.py
--rw-r--r--   0        0        0       89 2024-03-28 19:01:25.020045 dynamojo-0.2.1/dynamojo/boto.py
--rw-r--r--   0        0        0     2212 2024-03-28 19:01:25.020184 dynamojo-0.2.1/dynamojo/config.py
--rw-r--r--   0        0        0      445 2024-03-28 19:01:25.020304 dynamojo-0.2.1/dynamojo/exceptions.py
--rw-r--r--   0        0        0     4406 2024-03-28 19:01:25.020555 dynamojo-0.2.1/dynamojo/index.py
--rw-r--r--   0        0        0     1882 2024-03-28 19:01:25.020700 dynamojo-0.2.1/dynamojo/utils.py
--rw-r--r--   0        0        0      644 2024-03-28 21:03:40.934002 dynamojo-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4677 1970-01-01 00:00:00.000000 dynamojo-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     4181 2024-03-28 19:01:25.019286 dynamojo-0.2.2/README.md
+-rw-r--r--   0        0        0      449 2024-03-28 19:01:25.019636 dynamojo-0.2.2/dynamojo/__init__.py
+-rwxr-xr-x   0        0        0    19977 2024-04-01 20:21:05.180906 dynamojo-0.2.2/dynamojo/base.py
+-rw-r--r--   0        0        0       89 2024-03-28 19:01:25.020045 dynamojo-0.2.2/dynamojo/boto.py
+-rw-r--r--   0        0        0     2212 2024-03-28 19:01:25.020184 dynamojo-0.2.2/dynamojo/config.py
+-rw-r--r--   0        0        0      445 2024-03-28 19:01:25.020304 dynamojo-0.2.2/dynamojo/exceptions.py
+-rw-r--r--   0        0        0     4406 2024-03-28 19:01:25.020555 dynamojo-0.2.2/dynamojo/index.py
+-rw-r--r--   0        0        0     1882 2024-03-28 19:01:25.020700 dynamojo-0.2.2/dynamojo/utils.py
+-rw-r--r--   0        0        0      644 2024-04-03 20:18:30.948916 dynamojo-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4677 1970-01-01 00:00:00.000000 dynamojo-0.2.2/PKG-INFO
```

### Comparing `dynamojo-0.2.1/README.md` & `dynamojo-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `dynamojo-0.2.1/dynamojo/base.py` & `dynamojo-0.2.2/dynamojo/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -283,25 +283,26 @@
         return cls.construct(**(res))
 
     def delete(self) -> None:
         """
         Deletes an item from the table
         """
         key = {
-            self._config.indexes.table.partitionkey: self.__index_values__[
-                self._config.indexes.table.partitionkey
-            ]
+            self._config.indexes.table.partitionkey: self.index_attributes()[self._config.indexes.table.partitionkey]
         }
 
         if self._config.indexes.table.is_composite:
-            key[self._config.indexes.table.sortkey] = self.__index_values__[
-                self._config.indexes.table.sortkey
-            ]
+            key[self._config.indexes.table.sortkey] = self.index_attributes()[self._config.indexes.table.sortkey]
 
-        res = self._config.table.delete_item(Key=key)
+        serialized_key = {k: TYPE_SERIALIZER.serialize(v) for k, v in key.items()}
+
+        res = DYNAMOCLIENT.delete_item(
+            Key=serialized_key,
+            TableName=self._config.table
+        )
 
         return res
 
     @staticmethod
     def _deserialize_dynamo(data: Dict[str, Any]) -> Dict[str, Any]:
         """
         Deserializes the results from a low-level boto3 Dynamodb client query/get_item
```

### Comparing `dynamojo-0.2.1/dynamojo/config.py` & `dynamojo-0.2.2/dynamojo/config.py`

 * *Files identical despite different names*

### Comparing `dynamojo-0.2.1/dynamojo/index.py` & `dynamojo-0.2.2/dynamojo/index.py`

 * *Files identical despite different names*

### Comparing `dynamojo-0.2.1/dynamojo/utils.py` & `dynamojo-0.2.2/dynamojo/utils.py`

 * *Files identical despite different names*

### Comparing `dynamojo-0.2.1/pyproject.toml` & `dynamojo-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Dynamojo"
-version = "0.2.1"
+version = "0.2.2"
 description = "ORM For dynamodb"
 authors = ["Mathew Moon <me@mathewmoon.net>"]
 homepage = "https://github.com/mathewmoon/dynamojo"
 repository = "https://github.com/mathewmoon/dynamojo"
 
 readme = "README.md"
 packages = [{include = "dynamojo", from = "."}]
```

### Comparing `dynamojo-0.2.1/PKG-INFO` & `dynamojo-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Dynamojo
-Version: 0.2.1
+Version: 0.2.2
 Summary: ORM For dynamodb
 Home-page: https://github.com/mathewmoon/dynamojo
 Author: Mathew Moon
 Author-email: me@mathewmoon.net
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
```

