# Comparing `tmp/dynamojo-1.0.0.tar.gz` & `tmp/dynamojo-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamojo-1.0.0.tar", max compression
+gzip compressed data, was "dynamojo-1.0.1.tar", max compression
```

## Comparing `dynamojo-1.0.0.tar` & `dynamojo-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     4181 2024-03-28 19:01:25.019286 dynamojo-1.0.0/README.md
--rw-r--r--   0        0        0      449 2024-04-03 21:30:22.401274 dynamojo-1.0.0/dynamojo/__init__.py
--rwxr-xr-x   0        0        0    20356 2024-04-03 21:31:37.755246 dynamojo-1.0.0/dynamojo/base.py
--rw-r--r--   0        0        0       89 2024-04-03 20:38:31.250208 dynamojo-1.0.0/dynamojo/boto.py
--rw-r--r--   0        0        0     2098 2024-04-03 21:30:22.427738 dynamojo-1.0.0/dynamojo/config.py
--rw-r--r--   0        0        0      445 2024-04-03 20:38:31.251170 dynamojo-1.0.0/dynamojo/exceptions.py
--rw-r--r--   0        0        0     4404 2024-04-03 21:30:22.449865 dynamojo-1.0.0/dynamojo/index.py
--rw-r--r--   0        0        0     1991 2024-04-03 21:30:22.437078 dynamojo-1.0.0/dynamojo/utils.py
--rw-r--r--   0        0        0      643 2024-04-03 21:30:19.509805 dynamojo-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4676 1970-01-01 00:00:00.000000 dynamojo-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     4600 2024-04-03 21:45:32.767591 dynamojo-1.0.1/README.md
+-rw-r--r--   0        0        0      449 2024-04-03 21:30:22.401274 dynamojo-1.0.1/dynamojo/__init__.py
+-rwxr-xr-x   0        0        0    20356 2024-04-03 21:31:37.755246 dynamojo-1.0.1/dynamojo/base.py
+-rw-r--r--   0        0        0       89 2024-04-03 20:38:31.250208 dynamojo-1.0.1/dynamojo/boto.py
+-rw-r--r--   0        0        0     2098 2024-04-03 21:30:22.427738 dynamojo-1.0.1/dynamojo/config.py
+-rw-r--r--   0        0        0      445 2024-04-03 20:38:31.251170 dynamojo-1.0.1/dynamojo/exceptions.py
+-rw-r--r--   0        0        0     4404 2024-04-03 21:30:22.449865 dynamojo-1.0.1/dynamojo/index.py
+-rw-r--r--   0        0        0     1991 2024-04-03 21:30:22.437078 dynamojo-1.0.1/dynamojo/utils.py
+-rw-r--r--   0        0        0      643 2024-04-03 21:47:15.479763 dynamojo-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5095 1970-01-01 00:00:00.000000 dynamojo-1.0.1/PKG-INFO
```

### Comparing `dynamojo-1.0.0/README.md` & `dynamojo-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,22 @@
 # Dynamojo
+
+---
+###  :exclamation: Important Notice :exclamation:
+Version 1.0.0 is an important update that introduces breaking changes:
+  * Pydantic dependency is not at 2.x
+    * `DynamojoBase._config` attribute is now `DynamojoBase.__config__`
+  * The following methods are now async:
+    * `DynamojoBase.delete`
+    * `DynamojoBase.fetch`
+    * `DynamojoBase.query`
+    * `DynamojoBase.save`
+    * `DynamojoBase.update`
+---
+
 ## Because one table is better than more
 
 Dynamojo takes the concept of Dynamodb Single Table design and creates a modeling framework for it. This library is opinionated in the following ways:
 - Indexes should be generic. They could mean different things for different types of items. **An index attribute shouldn't imply that it is always a date, color, etc**.
 - When using generic indexes the attributes should shadow a human readable attribute. For instance if you have a partition key named "pk" that for items that represent users stores their  userid, then there should also be an attribute named userid.
 - When creating models for item types that will be stored in the database the developer should only have to worry about their access patterns in terms of the human readable attributes, not be in the weeds of the index design of the table. Mapping items to indexes should happen in code, not in the table definition itself
 - Table and Global Secondary indexes should always define a sortkey. There is no reason not to. It's better to have it in cases where you don't need it than to need it and not have it.
@@ -95,8 +109,8 @@
     content {
       name            = "lsi${local_secondary_index.value}"
       range_key       = "lsi${local_secondary_index.value}_sk"
       projection_type = "ALL"
     }
   }
 }
-```
+```
```

### Comparing `dynamojo-1.0.0/dynamojo/base.py` & `dynamojo-1.0.1/dynamojo/base.py`

 * *Files identical despite different names*

### Comparing `dynamojo-1.0.0/dynamojo/config.py` & `dynamojo-1.0.1/dynamojo/config.py`

 * *Files identical despite different names*

### Comparing `dynamojo-1.0.0/dynamojo/index.py` & `dynamojo-1.0.1/dynamojo/index.py`

 * *Files identical despite different names*

### Comparing `dynamojo-1.0.0/dynamojo/utils.py` & `dynamojo-1.0.1/dynamojo/utils.py`

 * *Files identical despite different names*

### Comparing `dynamojo-1.0.0/pyproject.toml` & `dynamojo-1.0.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Dynamojo"
-version = "1.0.0"
+version = "1.0.1"
 description = "ORM For dynamodb"
 authors = ["Mathew Moon <me@mathewmoon.net>"]
 homepage = "https://github.com/mathewmoon/dynamojo"
 repository = "https://github.com/mathewmoon/dynamojo"
 
 readme = "README.md"
 packages = [{include = "dynamojo", from = "."}]
```

### Comparing `dynamojo-1.0.0/PKG-INFO` & `dynamojo-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,37 @@
 Metadata-Version: 2.1
 Name: Dynamojo
-Version: 1.0.0
+Version: 1.0.1
 Summary: ORM For dynamodb
 Home-page: https://github.com/mathewmoon/dynamojo
 Author: Mathew Moon
 Author-email: me@mathewmoon.net
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: boto3 (>=1.34.56,<2.0.0)
 Requires-Dist: pydantic (>=2.0.0,<3.0.0)
 Project-URL: Repository, https://github.com/mathewmoon/dynamojo
 Description-Content-Type: text/markdown
 
 # Dynamojo
+
+---
+###  :exclamation: Important Notice :exclamation:
+Version 1.0.0 is an important update that introduces breaking changes:
+  * Pydantic dependency is not at 2.x
+    * `DynamojoBase._config` attribute is now `DynamojoBase.__config__`
+  * The following methods are now async:
+    * `DynamojoBase.delete`
+    * `DynamojoBase.fetch`
+    * `DynamojoBase.query`
+    * `DynamojoBase.save`
+    * `DynamojoBase.update`
+---
+
 ## Because one table is better than more
 
 Dynamojo takes the concept of Dynamodb Single Table design and creates a modeling framework for it. This library is opinionated in the following ways:
 - Indexes should be generic. They could mean different things for different types of items. **An index attribute shouldn't imply that it is always a date, color, etc**.
 - When using generic indexes the attributes should shadow a human readable attribute. For instance if you have a partition key named "pk" that for items that represent users stores their  userid, then there should also be an attribute named userid.
 - When creating models for item types that will be stored in the database the developer should only have to worry about their access patterns in terms of the human readable attributes, not be in the weeds of the index design of the table. Mapping items to indexes should happen in code, not in the table definition itself
 - Table and Global Secondary indexes should always define a sortkey. There is no reason not to. It's better to have it in cases where you don't need it than to need it and not have it.
@@ -111,7 +125,8 @@
       name            = "lsi${local_secondary_index.value}"
       range_key       = "lsi${local_secondary_index.value}_sk"
       projection_type = "ALL"
     }
   }
 }
 ```
+
```

