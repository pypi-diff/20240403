# Comparing `tmp/llama_index_graph_stores_falkordb-0.1.2.tar.gz` & `tmp/llama_index_graph_stores_falkordb-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_graph_stores_falkordb-0.1.2.tar", max compression
+gzip compressed data, was "llama_index_graph_stores_falkordb-0.1.3.tar", max compression
```

## Comparing `llama_index_graph_stores_falkordb-0.1.2.tar` & `llama_index_graph_stores_falkordb-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       48 2024-02-13 13:53:01.639136 llama_index_graph_stores_falkordb-0.1.2/README.md
--rw-r--r--   0        0        0      104 2024-02-13 13:53:01.639341 llama_index_graph_stores_falkordb-0.1.2/llama_index/graph_stores/falkordb/__init__.py
--rw-r--r--   0        0        0     5946 2024-02-13 13:53:01.639414 llama_index_graph_stores_falkordb-0.1.2/llama_index/graph_stores/falkordb/base.py
--rw-r--r--   0        0        0     1480 2024-02-21 17:09:37.081955 llama_index_graph_stores_falkordb-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      704 1970-01-01 00:00:00.000000 llama_index_graph_stores_falkordb-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       48 2024-04-03 01:39:40.431653 llama_index_graph_stores_falkordb-0.1.3/README.md
+-rw-r--r--   0        0        0      104 2024-04-03 01:39:40.431653 llama_index_graph_stores_falkordb-0.1.3/llama_index/graph_stores/falkordb/__init__.py
+-rw-r--r--   0        0        0     5967 2024-04-03 01:39:40.431653 llama_index_graph_stores_falkordb-0.1.3/llama_index/graph_stores/falkordb/base.py
+-rw-r--r--   0        0        0     1483 2024-04-03 01:39:40.431653 llama_index_graph_stores_falkordb-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      656 1970-01-01 00:00:00.000000 llama_index_graph_stores_falkordb-0.1.3/PKG-INFO
```

### Comparing `llama_index_graph_stores_falkordb-0.1.2/llama_index/graph_stores/falkordb/base.py` & `llama_index_graph_stores_falkordb-0.1.3/llama_index/graph_stores/falkordb/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Simple graph store index."""
 
 import logging
 from typing import Any, Dict, List, Optional
 
-import redis
+from falkordb import FalkorDB
 from llama_index.core.graph_stores.types import GraphStore
 
 logger = logging.getLogger(__name__)
 
 
 class FalkorDBGraphStore(GraphStore):
     """FalkorDB Graph Store.
@@ -26,15 +26,15 @@
         database: str = "falkor",
         node_label: str = "Entity",
         **kwargs: Any,
     ) -> None:
         """Initialize params."""
         self._node_label = node_label
 
-        self._driver = redis.Redis.from_url(url).graph(database)
+        self._driver = FalkorDB.from_url(url).select_graph(database)
         self._driver.query(f"CREATE INDEX FOR (n:`{self._node_label}`) ON (n.id)")
 
         self._database = database
 
         self.schema = ""
         self.get_query = f"""
             MATCH (n1:`{self._node_label}`)-[r]->(n2:`{self._node_label}`)
```

### Comparing `llama_index_graph_stores_falkordb-0.1.2/pyproject.toml` & `llama_index_graph_stores_falkordb-0.1.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index graph stores falkordb integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-graph-stores-falkordb"
 readme = "README.md"
-version = "0.1.2"
+version = "0.1.3"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
-redis = "^5.0.1"
+falkordb = "^1.0.4"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
 pre-commit = "3.2.0"
 pylint = "2.15.10"
```

### Comparing `llama_index_graph_stores_falkordb-0.1.2/PKG-INFO` & `llama_index_graph_stores_falkordb-0.1.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: llama-index-graph-stores-falkordb
-Version: 0.1.2
+Version: 0.1.3
 Summary: llama-index graph stores falkordb integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: falkordb (>=1.0.4,<2.0.0)
 Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
-Requires-Dist: redis (>=5.0.1,<6.0.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Graph Stores Integration: Falkordb
```

