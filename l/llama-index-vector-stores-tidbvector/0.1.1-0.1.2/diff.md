# Comparing `tmp/llama_index_vector_stores_tidbvector-0.1.1.tar.gz` & `tmp/llama_index_vector_stores_tidbvector-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_vector_stores_tidbvector-0.1.1.tar", max compression
+gzip compressed data, was "llama_index_vector_stores_tidbvector-0.1.2.tar", max compression
```

## Comparing `llama_index_vector_stores_tidbvector-0.1.1.tar` & `llama_index_vector_stores_tidbvector-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       51 2024-03-08 15:57:28.904526 llama_index_vector_stores_tidbvector-0.1.1/README.md
--rw-r--r--   0        0        0      102 2024-03-08 15:57:28.904526 llama_index_vector_stores_tidbvector-0.1.1/llama_index/vector_stores/tidbvector/__init__.py
--rw-r--r--   0        0        0    10144 2024-03-08 15:57:28.904526 llama_index_vector_stores_tidbvector-0.1.1/llama_index/vector_stores/tidbvector/base.py
--rw-r--r--   0        0        0     1693 2024-03-08 15:57:28.904526 llama_index_vector_stores_tidbvector-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      737 1970-01-01 00:00:00.000000 llama_index_vector_stores_tidbvector-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       51 2024-04-03 02:41:11.245921 llama_index_vector_stores_tidbvector-0.1.2/README.md
+-rw-r--r--   0        0        0      102 2024-04-03 02:41:11.245921 llama_index_vector_stores_tidbvector-0.1.2/llama_index/vector_stores/tidbvector/__init__.py
+-rw-r--r--   0        0        0    10100 2024-04-03 02:41:11.245921 llama_index_vector_stores_tidbvector-0.1.2/llama_index/vector_stores/tidbvector/base.py
+-rw-r--r--   0        0        0     1726 2024-04-03 02:41:11.245921 llama_index_vector_stores_tidbvector-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      745 1970-01-01 00:00:00.000000 llama_index_vector_stores_tidbvector-0.1.2/PKG-INFO
```

### Comparing `llama_index_vector_stores_tidbvector-0.1.1/llama_index/vector_stores/tidbvector/base.py` & `llama_index_vector_stores_tidbvector-0.1.2/llama_index/vector_stores/tidbvector/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     metadata_dict_to_node,
     node_to_metadata_dict,
 )
 
 _logger = logging.getLogger(__name__)
 
 DEFAULT_VECTOR_TABLE_NAME = "llama_index_vector_store"
-DEFAULT_DISTANCE_STRATEGY = "cosine"  # or "l2", "inner_product"
+DEFAULT_DISTANCE_STRATEGY = "cosine"  # or "l2"
 
 
 class TiDBVectorStore(BasePydanticVectorStore):
     stores_text = True
     flat_metadata = False
 
     _connection_string: str = PrivateAttr()
@@ -31,15 +31,15 @@
     _tidb: Any = PrivateAttr()
 
     def __init__(
         self,
         connection_string: str,
         table_name: str = DEFAULT_VECTOR_TABLE_NAME,
         distance_strategy: str = DEFAULT_DISTANCE_STRATEGY,
-        vector_dimension: Optional[int] = None,
+        vector_dimension: int = 1536,
         *,
         engine_args: Optional[Dict[str, Any]] = None,
         drop_existing_table: bool = False,
         **kwargs: Any,
     ) -> None:
         """
         Initialize a TiDB Vector Store in Llama Index with a flexible
@@ -60,16 +60,16 @@
         Args:
             connection_string (str): The connection string for the TiDB database.
                 format: "mysql+pymysql://root@34.212.137.91:4000/test".
             table_name (str, optional): The name of the table that will be used to
                 store vector data. If you do not provide a table name,
                 a default table named `llama_index_vector_store` will be created automatically
             distance_strategy: The strategy used for similarity search,
-                defaults to "cosine", valid values: "l2", "cosine", "inner_product".
-            vector_dimension: The dimension of the vector, defaults to None.
+                defaults to "cosine", valid values: "l2", "cosine".
+            vector_dimension: The dimension of the vector, defaults to 1536.
             engine_args (Optional[Dict[str, Any]], optional): Additional engine arguments. Defaults to None.
             drop_existing_table: Drop the existing TiDB table before initializing,
                 defaults to False.
             **kwargs (Any): Additional keyword arguments.
 
         Raises:
             ImportError: If the tidbvec python package is not installed.
```

### Comparing `llama_index_vector_stores_tidbvector-0.1.1/pyproject.toml` & `llama_index_vector_stores_tidbvector-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -27,21 +27,21 @@
 authors = ["Your Name <you@example.com>"]
 description = "llama-index vector-stores tidbvector integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-vector-stores-tidbvector"
 packages = [{include = "llama_index/"}]
 readme = "README.md"
-version = "0.1.1"
+version = "0.1.2"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = ">=0.10.1"
 sqlalchemy = ">=1.4,<3"
-tidb-vector = ">=0.0.3,<1.0.0"
+tidb-vector = {extras = ["client"], version = ">=0.0.3,<1.0.0"}
 pymysql = "^1.1.0"
 
 [tool.poetry.group.dev.dependencies]
 black = {extras = ["jupyter"], version = "<=23.9.1,>=23.7.0"}
 codespell = {extras = ["toml"], version = ">=v2.2.6"}
 ipython = "8.10.0"
 jupyter = "^1.0.0"
```

### Comparing `llama_index_vector_stores_tidbvector-0.1.1/PKG-INFO` & `llama_index_vector_stores_tidbvector-0.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: llama-index-vector-stores-tidbvector
-Version: 0.1.1
+Version: 0.1.2
 Summary: llama-index vector-stores tidbvector integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: llama-index-core (>=0.10.1)
 Requires-Dist: pymysql (>=1.1.0,<2.0.0)
 Requires-Dist: sqlalchemy (>=1.4,<3)
-Requires-Dist: tidb-vector (>=0.0.3,<1.0.0)
+Requires-Dist: tidb-vector[client] (>=0.0.3,<1.0.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Vector-Stores Integration: Tidbvector
```

