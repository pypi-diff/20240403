# Comparing `tmp/nodestream_plugin_neptune-0.12.0a2.tar.gz` & `tmp/nodestream_plugin_neptune-0.12.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodestream_plugin_neptune-0.12.0a2.tar", max compression
+gzip compressed data, was "nodestream_plugin_neptune-0.12.0rc1.tar", max compression
```

## Comparing `nodestream_plugin_neptune-0.12.0a2.tar` & `nodestream_plugin_neptune-0.12.0rc1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1173 2024-03-20 18:34:47.576682 nodestream_plugin_neptune-0.12.0a2/README.md
--rw-r--r--   0        0        0       81 2024-03-13 17:39:23.918836 nodestream_plugin_neptune-0.12.0a2/nodestream_plugin_neptune/__init__.py
--rw-r--r--   0        0        0     1769 2024-03-13 17:39:23.919169 nodestream_plugin_neptune-0.12.0a2/nodestream_plugin_neptune/extractor.py
--rw-r--r--   0        0        0    10309 2024-03-13 17:39:23.919585 nodestream_plugin_neptune-0.12.0a2/nodestream_plugin_neptune/ingest_query_builder.py
--rw-r--r--   0        0        0     4062 2024-03-20 18:34:47.577228 nodestream_plugin_neptune-0.12.0a2/nodestream_plugin_neptune/neptune_connection.py
--rw-r--r--   0        0        0     2902 2024-03-20 18:34:47.577927 nodestream_plugin_neptune-0.12.0a2/nodestream_plugin_neptune/neptune_connector.py
--rw-r--r--   0        0        0     3467 2024-03-20 18:34:47.578627 nodestream_plugin_neptune-0.12.0a2/nodestream_plugin_neptune/neptune_query_executor.py
--rw-r--r--   0        0        0      671 2024-03-13 17:39:23.921161 nodestream_plugin_neptune-0.12.0a2/nodestream_plugin_neptune/query.py
--rw-r--r--   0        0        0     2699 2024-03-13 17:39:23.921464 nodestream_plugin_neptune-0.12.0a2/nodestream_plugin_neptune/type_retriever.py
--rw-r--r--   0        0        0      740 2024-03-20 18:34:47.581368 nodestream_plugin_neptune-0.12.0a2/pyproject.toml
--rw-r--r--   0        0        0     1658 1970-01-01 00:00:00.000000 nodestream_plugin_neptune-0.12.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1173 2024-03-20 18:34:47.576682 nodestream_plugin_neptune-0.12.0rc1/README.md
+-rw-r--r--   0        0        0       81 2024-03-13 17:39:23.918836 nodestream_plugin_neptune-0.12.0rc1/nodestream_plugin_neptune/__init__.py
+-rw-r--r--   0        0        0     1769 2024-03-13 17:39:23.919169 nodestream_plugin_neptune-0.12.0rc1/nodestream_plugin_neptune/extractor.py
+-rw-r--r--   0        0        0    10309 2024-03-13 17:39:23.919585 nodestream_plugin_neptune-0.12.0rc1/nodestream_plugin_neptune/ingest_query_builder.py
+-rw-r--r--   0        0        0     6921 2024-04-03 14:28:46.026267 nodestream_plugin_neptune-0.12.0rc1/nodestream_plugin_neptune/neptune_connection.py
+-rw-r--r--   0        0        0     2992 2024-04-03 14:28:46.027040 nodestream_plugin_neptune-0.12.0rc1/nodestream_plugin_neptune/neptune_connector.py
+-rw-r--r--   0        0        0      431 2024-04-03 14:28:46.027630 nodestream_plugin_neptune-0.12.0rc1/nodestream_plugin_neptune/neptune_migrator.py
+-rw-r--r--   0        0        0     3467 2024-03-20 18:34:47.578627 nodestream_plugin_neptune-0.12.0rc1/nodestream_plugin_neptune/neptune_query_executor.py
+-rw-r--r--   0        0        0      671 2024-03-13 17:39:23.921161 nodestream_plugin_neptune-0.12.0rc1/nodestream_plugin_neptune/query.py
+-rw-r--r--   0        0        0     2699 2024-03-13 17:39:23.921464 nodestream_plugin_neptune-0.12.0rc1/nodestream_plugin_neptune/type_retriever.py
+-rw-r--r--   0        0        0      765 2024-04-03 14:29:06.592253 nodestream_plugin_neptune-0.12.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     1696 1970-01-01 00:00:00.000000 nodestream_plugin_neptune-0.12.0rc1/PKG-INFO
```

### Comparing `nodestream_plugin_neptune-0.12.0a2/README.md` & `nodestream_plugin_neptune-0.12.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_neptune-0.12.0a2/nodestream_plugin_neptune/extractor.py` & `nodestream_plugin_neptune-0.12.0rc1/nodestream_plugin_neptune/extractor.py`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_neptune-0.12.0a2/nodestream_plugin_neptune/ingest_query_builder.py` & `nodestream_plugin_neptune-0.12.0rc1/nodestream_plugin_neptune/ingest_query_builder.py`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_neptune-0.12.0a2/nodestream_plugin_neptune/neptune_connector.py` & `nodestream_plugin_neptune-0.12.0rc1/nodestream_plugin_neptune/neptune_connector.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from nodestream.databases.copy import TypeRetriever
 from nodestream.databases.database_connector import (DatabaseConnector,
                                                      QueryExecutor)
+from nodestream.schema.migrations import Migrator
 
 from .ingest_query_builder import NeptuneIngestQueryBuilder
 from .neptune_connection import NeptuneAnalyticsConnection, NeptuneDBConnection
 from .neptune_query_executor import NeptuneQueryExecutor
+from .neptune_migrator import NeptuneMigrator
 
 
 class NeptuneConnector(DatabaseConnector, alias="neptune"):
     """A Connector for AWS Neptune Database and AWS Neptune Analytics.
 
     This class is responsible for creating the various components needed for
     nodestream to interact with a Neptune graph. It is also responsible
@@ -75,9 +77,9 @@
         )
 
     def make_type_retriever(self) -> TypeRetriever:
         from .type_retriever import NeptuneDBTypeRetriever
 
         return NeptuneDBTypeRetriever(self)
 
-    def make_migrator(self) -> TypeRetriever:
-        raise NotImplementedError
+    def make_migrator(self) -> Migrator:
+        return NeptuneMigrator()
```

### Comparing `nodestream_plugin_neptune-0.12.0a2/nodestream_plugin_neptune/neptune_query_executor.py` & `nodestream_plugin_neptune-0.12.0rc1/nodestream_plugin_neptune/neptune_query_executor.py`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_neptune-0.12.0a2/nodestream_plugin_neptune/query.py` & `nodestream_plugin_neptune-0.12.0rc1/nodestream_plugin_neptune/query.py`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_neptune-0.12.0a2/nodestream_plugin_neptune/type_retriever.py` & `nodestream_plugin_neptune-0.12.0rc1/nodestream_plugin_neptune/type_retriever.py`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_neptune-0.12.0a2/pyproject.toml` & `nodestream_plugin_neptune-0.12.0rc1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [tool.poetry]
 name = "nodestream-plugin-neptune"
-version = "0.12.0a2"
+version = "0.12.0rc1"
 description = ""
 authors = ["Zach Probst <Zach_Probst@intuit.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-nodestream = { version = "0.12.0a3", allow-prereleases = true} # TODO: Change this to 0.12 Final when it is ready
+nodestream = { version = "0.12.0rc2", allow-prereleases = true} # TODO: Change this to 0.12 Final when it is ready
 cymple = "^0.11.0"
 aiobotocore = "^2.12.0"
+botocore = ">=1.34.40"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.12.1"
 pyhamcrest = "^2.1.0"
 freezegun = "^1.4.0"
 pytest = "^7.4.4"
 pytest-mock = "^3.12.0"
```

### Comparing `nodestream_plugin_neptune-0.12.0a2/PKG-INFO` & `nodestream_plugin_neptune-0.12.0rc1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: nodestream-plugin-neptune
-Version: 0.12.0a2
+Version: 0.12.0rc1
 Summary: 
 Author: Zach Probst
 Author-email: Zach_Probst@intuit.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiobotocore (>=2.12.0,<3.0.0)
+Requires-Dist: botocore (>=1.34.40)
 Requires-Dist: cymple (>=0.11.0,<0.12.0)
-Requires-Dist: nodestream (==0.12.0a3)
+Requires-Dist: nodestream (==0.12.0rc2)
 Description-Content-Type: text/markdown
 
 # Neptune Plugin for Nodestream
 
 This plugin provides a [Nodestream](https://github.com/nodestream-proj/nodestream) interface to Amazon Neptune. 
 
 **NOTE: This plugin is currently in development and is not yet ready for production use.**
```

