# Comparing `tmp/elasticsearch_haystack-0.3.0.tar.gz` & `tmp/elasticsearch_haystack-0.4.0.tar.gz`

## Comparing `elasticsearch_haystack-0.3.0.tar` & `elasticsearch_haystack-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.3.0/docker-compose.yml
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.3.0/pydoc/config.yml
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.3.0/src/haystack_integrations/components/retrievers/elasticsearch/__init__.py
--rw-r--r--   0        0        0     4398 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.3.0/src/haystack_integrations/components/retrievers/elasticsearch/bm25_retriever.py
--rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.3.0/src/haystack_integrations/components/retrievers/elasticsearch/embedding_retriever.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.3.0/src/haystack_integrations/document_stores/elasticsearch/__init__.py
--rw-r--r--   0        0        0    15586 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.3.0/src/haystack_integrations/document_stores/elasticsearch/document_store.py
--rw-r--r--   0        0        0     9923 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.3.0/src/haystack_integrations/document_stores/elasticsearch/filters.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.3.0/tests/test_bm25_retriever.py
--rw-r--r--   0        0        0    13313 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.3.0/tests/test_document_store.py
--rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.3.0/tests/test_embedding_retriever.py
--rw-r--r--   0        0        0     8013 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.3.0/tests/test_filters.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.3.0/.gitignore
--rw-r--r--   0        0        0    11342 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.3.0/LICENSE
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.3.0/README.md
--rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.4.0/docker-compose.yml
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.4.0/pydoc/config.yml
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.4.0/src/haystack_integrations/components/retrievers/elasticsearch/__init__.py
+-rw-r--r--   0        0        0     4849 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.4.0/src/haystack_integrations/components/retrievers/elasticsearch/bm25_retriever.py
+-rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.4.0/src/haystack_integrations/components/retrievers/elasticsearch/embedding_retriever.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.4.0/src/haystack_integrations/document_stores/elasticsearch/__init__.py
+-rw-r--r--   0        0        0    17688 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.4.0/src/haystack_integrations/document_stores/elasticsearch/document_store.py
+-rw-r--r--   0        0        0     9923 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.4.0/src/haystack_integrations/document_stores/elasticsearch/filters.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.4.0/tests/test_bm25_retriever.py
+-rw-r--r--   0        0        0    13199 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.4.0/tests/test_document_store.py
+-rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.4.0/tests/test_embedding_retriever.py
+-rw-r--r--   0        0        0     8013 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.4.0/tests/test_filters.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.4.0/.gitignore
+-rw-r--r--   0        0        0    11342 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.4.0/LICENSE
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.4.0/README.md
+-rw-r--r--   0        0        0     3860 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.4.0/PKG-INFO
```

### Comparing `elasticsearch_haystack-0.3.0/pydoc/config.yml` & `elasticsearch_haystack-0.4.0/pydoc/config.yml`

 * *Files 7% similar despite different names*

```diff
@@ -21,11 +21,12 @@
   excerpt: Elasticsearch integration for Haystack
   category_slug: integrations-api
   title: Elasticsearch
   slug: integrations-elasticsearch
   order: 70
   markdown:
     descriptive_class_title: false
+    classdef_code_block: false
     descriptive_module_title: true
     add_method_class_prefix: true
     add_member_class_prefix: false
     filename: _readme_elasticsearch.md
```

### Comparing `elasticsearch_haystack-0.3.0/src/haystack_integrations/components/retrievers/elasticsearch/bm25_retriever.py` & `elasticsearch_haystack-0.4.0/src/haystack_integrations/components/retrievers/elasticsearch/bm25_retriever.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 from haystack.dataclasses import Document
 from haystack_integrations.document_stores.elasticsearch.document_store import ElasticsearchDocumentStore
 
 
 @component
 class ElasticsearchBM25Retriever:
     """
-    ElasticsearchBM25Retriever is a keyword-based retriever that uses BM25 to find the most
-    similar documents to a user's query.
+    ElasticsearchBM25Retriever retrieves documents from the ElasticsearchDocumentStore using BM25 algorithm to find the
+    most similar documents to a user's query.
+
     This retriever is only compatible with ElasticsearchDocumentStore.
 
     Usage example:
     ```python
     from haystack import Document
     from haystack_integrations.document_stores.elasticsearch import ElasticsearchDocumentStore
     from haystack_integrations.components.retrievers.elasticsearch import ElasticsearchBM25Retriever
@@ -31,15 +32,15 @@
         Document(text="My name is Silvano and I live in Matera"),
         Document(text="My name is Usagi Tsukino and I live in Tokyo"),
     ]
     document_store.write_documents(documents)
 
     result = retriever.run(query="Who lives in Berlin?")
     for doc in result["documents"]:
-        print(doc.text)
+        print(doc.content)
     ```
     """
 
     def __init__(
         self,
         *,
         document_store: ElasticsearchDocumentStore,
@@ -49,58 +50,74 @@
         scale_score: bool = False,
     ):
         """
         Initialize ElasticsearchBM25Retriever with an instance ElasticsearchDocumentStore.
 
         :param document_store: An instance of ElasticsearchDocumentStore.
         :param filters: Filters applied to the retrieved Documents, for more info
-                        see `ElasticsearchDocumentStore.filter_documents`, defaults to None
-        :param fuzziness: Fuzziness parameter passed to Elasticsearch, defaults to "AUTO".
-                          see the official documentation for valid values:
-                          https://www.elastic.co/guide/en/elasticsearch/reference/current/common-options.html#fuzziness
-        :param top_k: Maximum number of Documents to return, defaults to 10
-        :param scale_score: If `True` scales the Document`s scores between 0 and 1, defaults to False
+                        see `ElasticsearchDocumentStore.filter_documents`.
+        :param fuzziness: Fuzziness parameter passed to Elasticsearch. See the official
+            [documentation](https://www.elastic.co/guide/en/elasticsearch/reference/current/common-options.html#fuzziness)
+            for more details.
+        :param top_k: Maximum number of Documents to return.
+        :param scale_score: If `True` scales the Document`s scores between 0 and 1.
+        :raises ValueError: If `document_store` is not an instance of `ElasticsearchDocumentStore`.
         """
 
         if not isinstance(document_store, ElasticsearchDocumentStore):
             msg = "document_store must be an instance of ElasticsearchDocumentStore"
             raise ValueError(msg)
 
         self._document_store = document_store
         self._filters = filters or {}
         self._fuzziness = fuzziness
         self._top_k = top_k
         self._scale_score = scale_score
 
     def to_dict(self) -> Dict[str, Any]:
+        """
+        Serializes the component to a dictionary.
+
+        :returns:
+            Dictionary with serialized data.
+        """
         return default_to_dict(
             self,
             filters=self._filters,
             fuzziness=self._fuzziness,
             top_k=self._top_k,
             scale_score=self._scale_score,
             document_store=self._document_store.to_dict(),
         )
 
     @classmethod
     def from_dict(cls, data: Dict[str, Any]) -> "ElasticsearchBM25Retriever":
+        """
+        Deserializes the component from a dictionary.
+
+        :param data:
+            Dictionary to deserialize from.
+        :returns:
+            Deserialized component.
+        """
         data["init_parameters"]["document_store"] = ElasticsearchDocumentStore.from_dict(
             data["init_parameters"]["document_store"]
         )
         return default_from_dict(cls, data)
 
     @component.output_types(documents=List[Document])
     def run(self, query: str, filters: Optional[Dict[str, Any]] = None, top_k: Optional[int] = None):
         """
         Retrieve documents using the BM25 keyword-based algorithm.
 
-        :param query: String to search in Documents' text.
-        :param filters: Filters applied to the retrieved Documents.
-        :param top_k: Maximum number of Documents to return.
-        :return: List of Documents that match the query.
+        :param query: String to search in `Document`s' text.
+        :param filters: Filters applied to the retrieved `Document`s.
+        :param top_k: Maximum number of `Document` to return.
+        :returns: A dictionary with the following keys:
+            - `documents`: List of `Document`s that match the query.
         """
         docs = self._document_store._bm25_retrieval(
             query=query,
             filters=filters or self._filters,
             fuzziness=self._fuzziness,
             top_k=top_k or self._top_k,
             scale_score=self._scale_score,
```

### Comparing `elasticsearch_haystack-0.3.0/src/haystack_integrations/components/retrievers/elasticsearch/embedding_retriever.py` & `elasticsearch_haystack-0.4.0/src/haystack_integrations/components/retrievers/elasticsearch/embedding_retriever.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,74 +7,115 @@
 from haystack.dataclasses import Document
 from haystack_integrations.document_stores.elasticsearch.document_store import ElasticsearchDocumentStore
 
 
 @component
 class ElasticsearchEmbeddingRetriever:
     """
-    Uses a vector similarity metric to retrieve documents from the ElasticsearchDocumentStore.
+    ElasticsearchEmbeddingRetriever retrieves documents from the ElasticsearchDocumentStore using vector similarity.
 
-    Needs to be connected to the ElasticsearchDocumentStore to run.
+    Usage example:
+    ```python
+    from haystack import Document
+    from haystack.components.embedders import SentenceTransformersTextEmbedder
+    from haystack_integrations.document_stores.elasticsearch import ElasticsearchDocumentStore
+    from haystack_integrations.components.retrievers.elasticsearch import ElasticsearchEmbeddingRetriever
+
+    document_store = ElasticsearchDocumentStore(hosts="http://localhost:9200")
+    retriever = ElasticsearchEmbeddingRetriever(document_store=document_store)
+
+    # Add documents to DocumentStore
+    documents = [
+        Document(text="My name is Carla and I live in Berlin"),
+        Document(text="My name is Paul and I live in New York"),
+        Document(text="My name is Silvano and I live in Matera"),
+        Document(text="My name is Usagi Tsukino and I live in Tokyo"),
+    ]
+    document_store.write_documents(documents)
+
+    te = SentenceTransformersTextEmbedder()
+    te.warm_up()
+    query_embeddings = te.run("Who lives in Berlin?")["embedding"]
+
+    result = retriever.run(query=query_embeddings)
+    for doc in result["documents"]:
+        print(doc.content)
+    ```
     """
 
     def __init__(
         self,
         *,
         document_store: ElasticsearchDocumentStore,
         filters: Optional[Dict[str, Any]] = None,
         top_k: int = 10,
         num_candidates: Optional[int] = None,
     ):
         """
         Create the ElasticsearchEmbeddingRetriever component.
 
         :param document_store: An instance of ElasticsearchDocumentStore.
-        :param filters: Filters applied to the retrieved Documents. Defaults to None.
-            Filters are applied during the approximate kNN search to ensure that top_k matching documents are returned.
-        :param top_k: Maximum number of Documents to return, defaults to 10
+        :param filters: Filters applied to the retrieved Documents.
+            Filters are applied during the approximate KNN search to ensure that top_k matching documents are returned.
+        :param top_k: Maximum number of Documents to return.
         :param num_candidates: Number of approximate nearest neighbor candidates on each shard. Defaults to top_k * 10.
             Increasing this value will improve search accuracy at the cost of slower search speeds.
-            You can read more about it in the Elasticsearch documentation:
-            https://www.elastic.co/guide/en/elasticsearch/reference/current/knn-search.html#tune-approximate-knn-for-speed-accuracy
+            You can read more about it in the Elasticsearch
+            [documentation](https://www.elastic.co/guide/en/elasticsearch/reference/current/knn-search.html#tune-approximate-knn-for-speed-accuracy)
         :raises ValueError: If `document_store` is not an instance of ElasticsearchDocumentStore.
         """
         if not isinstance(document_store, ElasticsearchDocumentStore):
             msg = "document_store must be an instance of ElasticsearchDocumentStore"
             raise ValueError(msg)
 
         self._document_store = document_store
         self._filters = filters or {}
         self._top_k = top_k
         self._num_candidates = num_candidates
 
     def to_dict(self) -> Dict[str, Any]:
+        """
+        Serializes the component to a dictionary.
+
+        :returns:
+            Dictionary with serialized data.
+        """
         return default_to_dict(
             self,
             filters=self._filters,
             top_k=self._top_k,
             num_candidates=self._num_candidates,
             document_store=self._document_store.to_dict(),
         )
 
     @classmethod
     def from_dict(cls, data: Dict[str, Any]) -> "ElasticsearchEmbeddingRetriever":
+        """
+        Deserializes the component from a dictionary.
+
+        :param data:
+            Dictionary to deserialize from.
+        :returns:
+            Deserialized component.
+        """
         data["init_parameters"]["document_store"] = ElasticsearchDocumentStore.from_dict(
             data["init_parameters"]["document_store"]
         )
         return default_from_dict(cls, data)
 
     @component.output_types(documents=List[Document])
     def run(self, query_embedding: List[float], filters: Optional[Dict[str, Any]] = None, top_k: Optional[int] = None):
         """
         Retrieve documents using a vector similarity metric.
 
         :param query_embedding: Embedding of the query.
-        :param filters: Filters applied to the retrieved Documents.
-        :param top_k: Maximum number of Documents to return.
-        :return: List of Documents similar to `query_embedding`.
+        :param filters: Filters applied to the retrieved `Document`s.
+        :param top_k: Maximum number of `Document`s to return.
+        :returns: A dictionary with the following keys:
+            - `documents`: List of `Document`s most similar to the given `query_embedding`
         """
         docs = self._document_store._embedding_retrieval(
             query_embedding=query_embedding,
             filters=filters or self._filters,
             top_k=top_k or self._top_k,
             num_candidates=self._num_candidates,
         )
```

### Comparing `elasticsearch_haystack-0.3.0/src/haystack_integrations/document_stores/elasticsearch/document_store.py` & `elasticsearch_haystack-0.4.0/src/haystack_integrations/document_stores/elasticsearch/document_store.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,68 +31,68 @@
 # Increase the default if most unscaled scores are larger than expected (>30) and otherwise would incorrectly
 # all be mapped to scores ~1.
 BM25_SCALING_FACTOR = 8
 
 
 class ElasticsearchDocumentStore:
     """
-    ElasticsearchDocumentStore is a Document Store for Elasticsearch.
-    It can be used with Elastic Cloud or your own Elasticsearch cluster.
+    ElasticsearchDocumentStore is a Document Store for Elasticsearch. It can be used with Elastic Cloud or your own
+    Elasticsearch cluster.
 
-    Simple usage with Elastic Cloud:
+    Usage example (Elastic Cloud):
     ```python
     from haystack.document_store.elasticsearch import ElasticsearchDocumentStore
     document_store = ElasticsearchDocumentStore(cloud_id="YOUR_CLOUD_ID", api_key="YOUR_API_KEY")
     ```
 
-    One can also connect to a self-hosted Elasticsearch instance:
+    Usage example (self-hosted Elasticsearch instance):
     ```python
     from haystack.document_store.elasticsearch import ElasticsearchDocumentStore
     document_store = ElasticsearchDocumentStore(hosts="http://localhost:9200")
     ```
     In the above example we connect with security disabled just to show the basic usage.
     We strongly recommend to enable security so that only authorized users can access your data.
 
     For more details on how to connect to Elasticsearch and configure security,
-    see the official Elasticsearch documentation:
-    https://www.elastic.co/guide/en/elasticsearch/client/python-api/current/connecting.html
+    see the official Elasticsearch
+    [documentation](https://www.elastic.co/guide/en/elasticsearch/client/python-api/current/connecting.html)
 
     All extra keyword arguments will be passed to the Elasticsearch client.
     """
 
     def __init__(
         self,
         *,
         hosts: Optional[Hosts] = None,
         index: str = "default",
         embedding_similarity_function: Literal["cosine", "dot_product", "l2_norm", "max_inner_product"] = "cosine",
         **kwargs,
     ):
         """
         Creates a new ElasticsearchDocumentStore instance.
-        When no index is explicitly specified, it will use the default index "default".
-        It will also try to create that index if it doesn't exist yet. Otherwise it will use the existing one.
+
+        It will also try to create that index if it doesn't exist yet. Otherwise, it will use the existing one.
 
         One can also set the similarity function used to compare Documents embeddings. This is mostly useful
         when using the `ElasticsearchDocumentStore` in a Pipeline with an `ElasticsearchEmbeddingRetriever`.
 
-        For more information on connection parameters, see the official Elasticsearch documentation:
-        https://www.elastic.co/guide/en/elasticsearch/client/python-api/current/connecting.html
+        For more information on connection parameters, see the official Elasticsearch
+        [documentation](https://www.elastic.co/guide/en/elasticsearch/client/python-api/current/connecting.html)
 
-        For the full list of supported kwargs, see the official Elasticsearch reference:
-        https://elasticsearch-py.readthedocs.io/en/stable/api.html#module-elasticsearch
+        For the full list of supported kwargs, see the official Elasticsearch
+        [reference](https://elasticsearch-py.readthedocs.io/en/stable/api.html#module-elasticsearch)
 
-        :param hosts: List of hosts running the Elasticsearch client. Defaults to None
-        :param index: Name of index in Elasticsearch, if it doesn't exist it will be created. Defaults to "default"
+        :param hosts: List of hosts running the Elasticsearch client.
+        :param index: Name of index in Elasticsearch.
         :param embedding_similarity_function: The similarity function used to compare Documents embeddings.
-            Defaults to "cosine". This parameter only takes effect if the index does not yet exist and is created.
+            This parameter only takes effect if the index does not yet exist and is created.
             To choose the most appropriate function, look for information about your embedding model.
-            To understand how document scores are computed, see the Elasticsearch documentation:
-            https://www.elastic.co/guide/en/elasticsearch/reference/current/dense-vector.html#dense-vector-params
-        :param **kwargs: Optional arguments that ``Elasticsearch`` takes.
+            To understand how document scores are computed, see the Elasticsearch
+            [documentation](https://www.elastic.co/guide/en/elasticsearch/reference/current/dense-vector.html#dense-vector-params)
+        :param **kwargs: Optional arguments that `Elasticsearch` takes.
         """
         self._hosts = hosts
         self._client = Elasticsearch(
             hosts,
             headers={"user-agent": f"haystack-py-ds/{haystack_version}"},
             **kwargs,
         )
@@ -102,41 +102,68 @@
 
         # Check client connection, this will raise if not connected
         self._client.info()
 
         # configure mapping for the embedding field
         mappings = {
             "properties": {
-                "embedding": {"type": "dense_vector", "index": True, "similarity": embedding_similarity_function}
-            }
+                "embedding": {"type": "dense_vector", "index": True, "similarity": embedding_similarity_function},
+                "content": {"type": "text"},
+            },
+            "dynamic_templates": [
+                {
+                    "strings": {
+                        "path_match": "*",
+                        "match_mapping_type": "string",
+                        "mapping": {
+                            "type": "keyword",
+                        },
+                    }
+                }
+            ],
         }
 
         # Create the index if it doesn't exist
         if not self._client.indices.exists(index=index):
             self._client.indices.create(index=index, mappings=mappings)
 
     def to_dict(self) -> Dict[str, Any]:
+        """
+        Serializes the component to a dictionary.
+
+        :returns:
+            Dictionary with serialized data.
+        """
         # This is not the best solution to serialise this class but is the fastest to implement.
         # Not all kwargs types can be serialised to text so this can fail. We must serialise each
         # type explicitly to handle this properly.
         return default_to_dict(
             self,
             hosts=self._hosts,
             index=self._index,
             embedding_similarity_function=self._embedding_similarity_function,
             **self._kwargs,
         )
 
     @classmethod
     def from_dict(cls, data: Dict[str, Any]) -> "ElasticsearchDocumentStore":
+        """
+        Deserializes the component from a dictionary.
+
+        :param data:
+            Dictionary to deserialize from.
+        :returns:
+            Deserialized component.
+        """
         return default_from_dict(cls, data)
 
     def count_documents(self) -> int:
         """
         Returns how many documents are present in the document store.
+        :returns: Number of documents in the document store.
         """
         return self._client.count(index=self._index)["count"]
 
     def _search_documents(self, **kwargs) -> List[Document]:
         """
         Calls the Elasticsearch client's search method and handles pagination.
         """
@@ -161,46 +188,74 @@
             if top_k is not None and from_ >= top_k:
                 break
             if from_ >= res["hits"]["total"]["value"]:
                 break
         return documents
 
     def filter_documents(self, filters: Optional[Dict[str, Any]] = None) -> List[Document]:
+        """
+        The main query method for the document store. It retrieves all documents that match the filters.
+
+        :param filters: A dictionary of filters to apply. For more information on the structure of the filters,
+            see the official Elasticsearch
+            [documentation](https://www.elastic.co/guide/en/elasticsearch/reference/current/query-dsl.html)
+        :returns: List of `Document`s that match the filters.
+        """
         if filters and "operator" not in filters and "conditions" not in filters:
             filters = convert(filters)
 
         query = {"bool": {"filter": _normalize_filters(filters)}} if filters else None
         documents = self._search_documents(query=query)
         return documents
 
     def write_documents(self, documents: List[Document], policy: DuplicatePolicy = DuplicatePolicy.NONE) -> int:
         """
-        Writes Documents to Elasticsearch.
-        If policy is not specified or set to DuplicatePolicy.NONE, it will raise an exception if a document with the
-        same ID already exists in the document store.
+        Writes `Document`s to Elasticsearch.
+
+        :param documents: List of Documents to write to the document store.
+        :param policy: DuplicatePolicy to apply when a document with the same ID already exists in the document store.
+        :raises ValueError: If `documents` is not a list of `Document`s.
+        :raises DuplicateDocumentError: If a document with the same ID already exists in the document store and
+            `policy` is set to `DuplicatePolicy.FAIL` or `DuplicatePolicy.NONE`.
+        :raises DocumentStoreError: If an error occurs while writing the documents to the document store.
+        :returns: Number of documents written to the document store.
         """
         if len(documents) > 0:
             if not isinstance(documents[0], Document):
                 msg = "param 'documents' must contain a list of objects of type Document"
                 raise ValueError(msg)
 
         if policy == DuplicatePolicy.NONE:
             policy = DuplicatePolicy.FAIL
 
         action = "index" if policy == DuplicatePolicy.OVERWRITE else "create"
-        documents_written, errors = helpers.bulk(
-            client=self._client,
-            actions=(
+
+        elasticsearch_actions = []
+        for doc in documents:
+            doc_dict = doc.to_dict()
+            if "sparse_embedding" in doc_dict:
+                sparse_embedding = doc_dict.pop("sparse_embedding", None)
+                if sparse_embedding:
+                    logger.warning(
+                        "Document %s has the `sparse_embedding` field set,"
+                        "but storing sparse embeddings in Elasticsearch is not currently supported."
+                        "The `sparse_embedding` field will be ignored.",
+                        doc.id,
+                    )
+            elasticsearch_actions.append(
                 {
                     "_op_type": action,
                     "_id": doc.id,
-                    "_source": doc.to_dict(),
+                    "_source": doc_dict,
                 }
-                for doc in documents
-            ),
+            )
+
+        documents_written, errors = helpers.bulk(
+            client=self._client,
+            actions=elasticsearch_actions,
             refresh="wait_for",
             index=self._index,
             raise_on_error=False,
         )
 
         if errors:
             duplicate_errors_ids = []
@@ -221,35 +276,39 @@
 
             if len(other_errors) > 0:
                 msg = f"Failed to write documents to Elasticsearch. Errors:\n{other_errors}"
                 raise DocumentStoreError(msg)
 
         return documents_written
 
-    def _deserialize_document(self, hit: Dict[str, Any]) -> Document:
+    @staticmethod
+    def _deserialize_document(hit: Dict[str, Any]) -> Document:
         """
-        Creates a Document from the search hit provided.
+        Creates a `Document` from the search hit provided.
+
         This is mostly useful in self.filter_documents().
+
+        :param hit: A search hit from Elasticsearch.
+        :returns: `Document` created from the search hit.
         """
         data = hit["_source"]
 
         if "highlight" in hit:
             data["metadata"]["highlighted"] = hit["highlight"]
         data["score"] = hit["_score"]
 
         return Document.from_dict(data)
 
     def delete_documents(self, document_ids: List[str]) -> None:
         """
-        Deletes all documents with a matching document_ids from the document store.
+        Deletes all `Document`s with a matching `document_ids` from the document store.
 
-        :param object_ids: the object_ids to delete
+        :param document_ids: the object IDs to delete
         """
 
-        #
         helpers.bulk(
             client=self._client,
             actions=({"_op_type": "delete", "_id": id_} for id_ in document_ids),
             refresh="wait_for",
             index=self._index,
             raise_on_error=False,
         )
@@ -260,34 +319,33 @@
         *,
         filters: Optional[Dict[str, Any]] = None,
         fuzziness: str = "AUTO",
         top_k: int = 10,
         scale_score: bool = False,
     ) -> List[Document]:
         """
-        Elasticsearch by defaults uses BM25 search algorithm.
+        Retrieves `Document`s from Elasticsearch using the BM25 search algorithm.
+
         Even though this method is called `bm25_retrieval` it searches for `query`
         using the search algorithm `_client` was configured with.
 
-        This method is not mean to be part of the public interface of
+        This method is not meant to be part of the public interface of
         `ElasticsearchDocumentStore` nor called directly.
         `ElasticsearchBM25Retriever` uses this method directly and is the public interface for it.
 
-        `query` must be a non empty string, otherwise a `ValueError` will be raised.
-
-        :param query: String to search in saved Documents' text.
-        :param filters: Filters applied to the retrieved Documents, for more info
-                        see `ElasticsearchDocumentStore.filter_documents`, defaults to None
-        :param fuzziness: Fuzziness parameter passed to Elasticsearch, defaults to "AUTO".
-                          see the official documentation for valid values:
-                          https://www.elastic.co/guide/en/elasticsearch/reference/current/common-options.html#fuzziness
-        :param top_k: Maximum number of Documents to return, defaults to 10
-        :param scale_score: If `True` scales the Document`s scores between 0 and 1, defaults to False
+        :param query: String to search in saved `Document`s' text.
+        :param filters: Filters applied to the retrieved `Document`s, for more info
+                        see `ElasticsearchDocumentStore.filter_documents`.
+        :param fuzziness: Fuzziness parameter passed to Elasticsearch. See the official
+            [documentation](https://www.elastic.co/guide/en/elasticsearch/reference/current/common-options.html#fuzziness)
+            for valid values.
+        :param top_k: Maximum number of `Document`s to return.
+        :param scale_score: If `True` scales the `Document``s scores between 0 and 1.
         :raises ValueError: If `query` is an empty string
-        :return: List of Document that match `query`
+        :returns: List of `Document` that match `query`
         """
 
         if not query:
             msg = "query must be a non empty string"
             raise ValueError(msg)
 
         body: Dict[str, Any] = {
@@ -325,30 +383,31 @@
         *,
         filters: Optional[Dict[str, Any]] = None,
         top_k: int = 10,
         num_candidates: Optional[int] = None,
     ) -> List[Document]:
         """
         Retrieves documents that are most similar to the query embedding using a vector similarity metric.
+
         It uses the Elasticsearch's Approximate k-Nearest Neighbors search algorithm.
 
-        This method is not mean to be part of the public interface of
+        This method is not meant to be part of the public interface of
         `ElasticsearchDocumentStore` nor called directly.
         `ElasticsearchEmbeddingRetriever` uses this method directly and is the public interface for it.
 
         :param query_embedding: Embedding of the query.
-        :param filters: Filters applied to the retrieved Documents. Defaults to None.
+        :param filters: Filters applied to the retrieved `Document`s.
             Filters are applied during the approximate kNN search to ensure that top_k matching documents are returned.
-        :param top_k: Maximum number of Documents to return, defaults to 10
+        :param top_k: Maximum number of `Document`s to return.
         :param num_candidates: Number of approximate nearest neighbor candidates on each shard. Defaults to top_k * 10.
             Increasing this value will improve search accuracy at the cost of slower search speeds.
-            You can read more about it in the Elasticsearch documentation:
-            https://www.elastic.co/guide/en/elasticsearch/reference/current/knn-search.html#tune-approximate-knn-for-speed-accuracy
-        :raises ValueError: If `query_embedding` is an empty list
-        :return: List of Document that are most similar to `query_embedding`
+            You can read more about it in the Elasticsearch
+            [documentation](https://www.elastic.co/guide/en/elasticsearch/reference/current/knn-search.html#tune-approximate-knn-for-speed-accuracy)
+        :raises ValueError: If `query_embedding` is an empty list.
+        :returns: List of `Document` that are most similar to `query_embedding`.
         """
 
         if not query_embedding:
             msg = "query_embedding must be a non-empty list of floats"
             raise ValueError(msg)
 
         if not num_candidates:
```

### Comparing `elasticsearch_haystack-0.3.0/src/haystack_integrations/document_stores/elasticsearch/filters.py` & `elasticsearch_haystack-0.4.0/src/haystack_integrations/document_stores/elasticsearch/filters.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_haystack-0.3.0/tests/test_bm25_retriever.py` & `elasticsearch_haystack-0.4.0/tests/test_bm25_retriever.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_haystack-0.3.0/tests/test_document_store.py` & `elasticsearch_haystack-0.4.0/tests/test_document_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,44 @@
 from haystack.dataclasses.document import Document
 from haystack.document_stores.errors import DocumentStoreError, DuplicateDocumentError
 from haystack.document_stores.types import DuplicatePolicy
 from haystack.testing.document_store import DocumentStoreBaseTests
 from haystack_integrations.document_stores.elasticsearch import ElasticsearchDocumentStore
 
 
+@patch("haystack_integrations.document_stores.elasticsearch.document_store.Elasticsearch")
+def test_to_dict(_mock_elasticsearch_client):
+    document_store = ElasticsearchDocumentStore(hosts="some hosts")
+    res = document_store.to_dict()
+    assert res == {
+        "type": "haystack_integrations.document_stores.elasticsearch.document_store.ElasticsearchDocumentStore",
+        "init_parameters": {
+            "hosts": "some hosts",
+            "index": "default",
+            "embedding_similarity_function": "cosine",
+        },
+    }
+
+
+@patch("haystack_integrations.document_stores.elasticsearch.document_store.Elasticsearch")
+def test_from_dict(_mock_elasticsearch_client):
+    data = {
+        "type": "haystack_integrations.document_stores.elasticsearch.document_store.ElasticsearchDocumentStore",
+        "init_parameters": {
+            "hosts": "some hosts",
+            "index": "default",
+            "embedding_similarity_function": "cosine",
+        },
+    }
+    document_store = ElasticsearchDocumentStore.from_dict(data)
+    assert document_store._hosts == "some hosts"
+    assert document_store._index == "default"
+    assert document_store._embedding_similarity_function == "cosine"
+
+
 @pytest.mark.integration
 class TestDocumentStore(DocumentStoreBaseTests):
     """
     Common test cases will be provided by `DocumentStoreBaseTests` but
     you can add more to this class.
     """
 
@@ -63,42 +93,14 @@
             }
             expected_meta.append(r)
         for doc in received:
             doc.score = None
 
         super().assert_documents_are_equal(received, expected)
 
-    @patch("haystack_integrations.document_stores.elasticsearch.document_store.Elasticsearch")
-    def test_to_dict(self, _mock_elasticsearch_client):
-        document_store = ElasticsearchDocumentStore(hosts="some hosts")
-        res = document_store.to_dict()
-        assert res == {
-            "type": "haystack_integrations.document_stores.elasticsearch.document_store.ElasticsearchDocumentStore",
-            "init_parameters": {
-                "hosts": "some hosts",
-                "index": "default",
-                "embedding_similarity_function": "cosine",
-            },
-        }
-
-    @patch("haystack_integrations.document_stores.elasticsearch.document_store.Elasticsearch")
-    def test_from_dict(self, _mock_elasticsearch_client):
-        data = {
-            "type": "haystack_integrations.document_stores.elasticsearch.document_store.ElasticsearchDocumentStore",
-            "init_parameters": {
-                "hosts": "some hosts",
-                "index": "default",
-                "embedding_similarity_function": "cosine",
-            },
-        }
-        document_store = ElasticsearchDocumentStore.from_dict(data)
-        assert document_store._hosts == "some hosts"
-        assert document_store._index == "default"
-        assert document_store._embedding_similarity_function == "cosine"
-
     def test_user_agent_header(self, document_store: ElasticsearchDocumentStore):
         assert document_store._client._headers["user-agent"].startswith("haystack-py-ds/")
 
     def test_write_documents(self, document_store: ElasticsearchDocumentStore):
         docs = [Document(id="1")]
         assert document_store.write_documents(docs) == 1
         with pytest.raises(DuplicateDocumentError):
```

### Comparing `elasticsearch_haystack-0.3.0/tests/test_embedding_retriever.py` & `elasticsearch_haystack-0.4.0/tests/test_embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_haystack-0.3.0/tests/test_filters.py` & `elasticsearch_haystack-0.4.0/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_haystack-0.3.0/.gitignore` & `elasticsearch_haystack-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `elasticsearch_haystack-0.3.0/LICENSE` & `elasticsearch_haystack-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `elasticsearch_haystack-0.3.0/README.md` & `elasticsearch_haystack-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `elasticsearch_haystack-0.3.0/pyproject.toml` & `elasticsearch_haystack-0.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -92,20 +92,20 @@
   "typing",
 ]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.black]
-target-version = ["py37"]
+target-version = ["py38"]
 line-length = 120
 skip-string-normalization = true
 
 [tool.ruff]
-target-version = "py37"
+target-version = "py38"
 line-length = 120
 select = [
   "A",
   "ARG",
   "B",
   "C",
   "DTZ",
@@ -152,29 +152,29 @@
 ban-relative-imports = "parents"
 
 [tool.ruff.per-file-ignores]
 # Tests can use magic values, assertions, and relative imports
 "tests/**/*" = ["PLR2004", "S101", "TID252"]
 
 [tool.coverage.run]
-source_pkgs = ["src", "tests"]
+source = ["haystack_integrations"]
 branch = true
-parallel = true
+parallel = false
 
-[tool.coverage.paths]
-elasticsearch_haystack = ["src/haystack_integrations", "*/elasticsearch/src/haystack_integrations"]
-tests = ["tests", "*/elasticsearch/src/tests"]
 
 [tool.coverage.report]
+omit = ["*/tests/*", "*/__init__.py"]
+show_missing=true
 exclude_lines = [
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
 
+
 [tool.pytest.ini_options]
 minversion = "6.0"
 markers = [
   "unit: unit tests",
   "integration: integration tests"
 ]
```

### Comparing `elasticsearch_haystack-0.3.0/PKG-INFO` & `elasticsearch_haystack-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: elasticsearch-haystack
-Version: 0.3.0
+Version: 0.4.0
 Summary: Haystack 2.x Document Store for ElasticSearch
 Project-URL: Documentation, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/elasticsearch#readme
 Project-URL: Issues, https://github.com/deepset-ai/haystack-core-integrations/issues
 Project-URL: Source, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/elasticsearch
 Author-email: Silvano Cerza <silvanocerza@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
```

