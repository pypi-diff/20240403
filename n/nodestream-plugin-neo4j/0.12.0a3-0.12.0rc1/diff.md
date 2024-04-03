# Comparing `tmp/nodestream_plugin_neo4j-0.12.0a3.tar.gz` & `tmp/nodestream_plugin_neo4j-0.12.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodestream_plugin_neo4j-0.12.0a3.tar", max compression
+gzip compressed data, was "nodestream_plugin_neo4j-0.12.0rc1.tar", max compression
```

## Comparing `nodestream_plugin_neo4j-0.12.0a3.tar` & `nodestream_plugin_neo4j-0.12.0rc1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     2547 2024-01-18 16:53:12.239701 nodestream_plugin_neo4j-0.12.0a3/README.md
--rw-r--r--   0        0        0       94 2024-03-08 15:43:02.882311 nodestream_plugin_neo4j-0.12.0a3/nodestream_plugin_neo4j/__init__.py
--rw-r--r--   0        0        0     2703 2024-03-08 17:46:33.350050 nodestream_plugin_neo4j-0.12.0a3/nodestream_plugin_neo4j/database_connector.py
--rw-r--r--   0        0        0     1744 2024-03-08 15:43:02.886882 nodestream_plugin_neo4j-0.12.0a3/nodestream_plugin_neo4j/extractor.py
--rw-r--r--   0        0        0     9475 2024-03-08 17:46:33.351553 nodestream_plugin_neo4j-0.12.0a3/nodestream_plugin_neo4j/ingest_query_builder.py
--rw-r--r--   0        0        0    16927 2024-03-20 18:23:46.523855 nodestream_plugin_neo4j-0.12.0a3/nodestream_plugin_neo4j/migrator.py
--rw-r--r--   0        0        0     1678 2024-03-08 15:43:02.893352 nodestream_plugin_neo4j-0.12.0a3/nodestream_plugin_neo4j/neo4j_database.py
--rw-r--r--   0        0        0     2195 2024-03-08 17:46:33.352799 nodestream_plugin_neo4j-0.12.0a3/nodestream_plugin_neo4j/query.py
--rw-r--r--   0        0        0     2821 2024-03-08 17:46:33.354141 nodestream_plugin_neo4j-0.12.0a3/nodestream_plugin_neo4j/query_executor.py
--rw-r--r--   0        0        0     2762 2024-03-08 15:43:02.896795 nodestream_plugin_neo4j-0.12.0a3/nodestream_plugin_neo4j/type_retriever.py
--rw-r--r--   0        0        0     1060 2024-03-20 18:37:15.208053 nodestream_plugin_neo4j-0.12.0a3/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 nodestream_plugin_neo4j-0.12.0a3/PKG-INFO
+-rw-r--r--   0        0        0     2547 2024-01-18 16:53:12.239701 nodestream_plugin_neo4j-0.12.0rc1/README.md
+-rw-r--r--   0        0        0       94 2024-03-08 15:43:02.882311 nodestream_plugin_neo4j-0.12.0rc1/nodestream_plugin_neo4j/__init__.py
+-rw-r--r--   0        0        0     2703 2024-03-08 17:46:33.350050 nodestream_plugin_neo4j-0.12.0rc1/nodestream_plugin_neo4j/database_connector.py
+-rw-r--r--   0        0        0     1744 2024-03-08 15:43:02.886882 nodestream_plugin_neo4j-0.12.0rc1/nodestream_plugin_neo4j/extractor.py
+-rw-r--r--   0        0        0     9475 2024-03-08 17:46:33.351553 nodestream_plugin_neo4j-0.12.0rc1/nodestream_plugin_neo4j/ingest_query_builder.py
+-rw-r--r--   0        0        0    16927 2024-03-20 18:23:46.523855 nodestream_plugin_neo4j-0.12.0rc1/nodestream_plugin_neo4j/migrator.py
+-rw-r--r--   0        0        0     1807 2024-04-03 14:25:34.326336 nodestream_plugin_neo4j-0.12.0rc1/nodestream_plugin_neo4j/neo4j_database.py
+-rw-r--r--   0        0        0     2195 2024-03-08 17:46:33.352799 nodestream_plugin_neo4j-0.12.0rc1/nodestream_plugin_neo4j/query.py
+-rw-r--r--   0        0        0     2821 2024-03-08 17:46:33.354141 nodestream_plugin_neo4j-0.12.0rc1/nodestream_plugin_neo4j/query_executor.py
+-rw-r--r--   0        0        0     2762 2024-03-08 15:43:02.896795 nodestream_plugin_neo4j-0.12.0rc1/nodestream_plugin_neo4j/type_retriever.py
+-rw-r--r--   0        0        0     1012 2024-04-03 14:28:10.722380 nodestream_plugin_neo4j-0.12.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     3026 1970-01-01 00:00:00.000000 nodestream_plugin_neo4j-0.12.0rc1/PKG-INFO
```

### Comparing `nodestream_plugin_neo4j-0.12.0a3/README.md` & `nodestream_plugin_neo4j-0.12.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_neo4j-0.12.0a3/nodestream_plugin_neo4j/database_connector.py` & `nodestream_plugin_neo4j-0.12.0rc1/nodestream_plugin_neo4j/database_connector.py`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_neo4j-0.12.0a3/nodestream_plugin_neo4j/extractor.py` & `nodestream_plugin_neo4j-0.12.0rc1/nodestream_plugin_neo4j/extractor.py`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_neo4j-0.12.0a3/nodestream_plugin_neo4j/ingest_query_builder.py` & `nodestream_plugin_neo4j-0.12.0rc1/nodestream_plugin_neo4j/ingest_query_builder.py`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_neo4j-0.12.0a3/nodestream_plugin_neo4j/migrator.py` & `nodestream_plugin_neo4j-0.12.0rc1/nodestream_plugin_neo4j/migrator.py`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_neo4j-0.12.0a3/nodestream_plugin_neo4j/neo4j_database.py` & `nodestream_plugin_neo4j-0.12.0rc1/nodestream_plugin_neo4j/neo4j_database.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,18 +39,21 @@
 
         result = await self.driver.execute_query(
             query.query_statement,
             query.parameters,
             database_=self.database_name,
             routing_=routing,
         )
-        for record in result.records:
-            if log_result:
+        if log_result:
+            for record in result.records:
                 self.logger.info(
                     "Gathered Query Results",
-                    extra=dict(**record, query=query.query_statement),
+                    extra=dict(
+                        **record,
+                        query=query.query_statement,
+                        uri=self.driver._pool.address.host
+                    ),
                 )
-
         return result.records
 
     def session(self) -> AsyncSession:
         return self.driver.session(database=self.database_name)
```

### Comparing `nodestream_plugin_neo4j-0.12.0a3/nodestream_plugin_neo4j/query.py` & `nodestream_plugin_neo4j-0.12.0rc1/nodestream_plugin_neo4j/query.py`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_neo4j-0.12.0a3/nodestream_plugin_neo4j/query_executor.py` & `nodestream_plugin_neo4j-0.12.0rc1/nodestream_plugin_neo4j/query_executor.py`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_neo4j-0.12.0a3/nodestream_plugin_neo4j/type_retriever.py` & `nodestream_plugin_neo4j-0.12.0rc1/nodestream_plugin_neo4j/type_retriever.py`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_neo4j-0.12.0a3/pyproject.toml` & `nodestream_plugin_neo4j-0.12.0rc1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "nodestream-plugin-neo4j"
-version = "0.12.0a3"
+version = "0.12.0rc1"
 description = ""
 authors = ["Zach Probst <Zach_Probst@intuit.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 neo4j = "^5.16.0"
-nodestream = { version = "0.12.0a3", allow-prereleases = true} # TODO: Change this to 0.12 Final when it is ready
+nodestream = { version = "0.12.0rc2", allow-prereleases = true} 
 cymple = "^0.11.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.12.1"
 pyhamcrest = "^2.1.0"
 freezegun = "^1.4.0"
 pytest = "^7.4.4"
```

### Comparing `nodestream_plugin_neo4j-0.12.0a3/PKG-INFO` & `nodestream_plugin_neo4j-0.12.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: nodestream-plugin-neo4j
-Version: 0.12.0a3
+Version: 0.12.0rc1
 Summary: 
 Author: Zach Probst
 Author-email: Zach_Probst@intuit.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cymple (>=0.11.0,<0.12.0)
 Requires-Dist: neo4j (>=5.16.0,<6.0.0)
-Requires-Dist: nodestream (==0.12.0a3)
+Requires-Dist: nodestream (==0.12.0rc2)
 Description-Content-Type: text/markdown
 
 # Neo4j Nodestream Plugin for Nodestream
 
 This plugin provides a [Nodestream](https://github.com/nodestream-proj/nodestream) interface to Neo4j. 
 
 **THIS PLUGIN IS IN BETA. USE AT YOUR OWN RISK.**
```

