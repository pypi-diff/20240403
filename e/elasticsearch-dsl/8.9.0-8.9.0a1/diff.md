# Comparing `tmp/elasticsearch-dsl-8.9.0.tar.gz` & `tmp/elasticsearch-dsl-8.9.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elasticsearch-dsl-8.9.0.tar", last modified: Thu Sep  7 09:36:11 2023, max compression
+gzip compressed data, was "elasticsearch-dsl-8.9.0a1.tar", last modified: Tue Aug 29 16:42:17 2023, max compression
```

## Comparing `elasticsearch-dsl-8.9.0.tar` & `elasticsearch-dsl-8.9.0a1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-09-07 09:36:11.140226 elasticsearch-dsl-8.9.0/
--rw-r--r--   0 q         (1000) q         (1000)      136 2022-05-23 12:42:04.000000 elasticsearch-dsl-8.9.0/AUTHORS
--rw-r--r--   0 q         (1000) q         (1000)     2255 2022-05-23 12:42:04.000000 elasticsearch-dsl-8.9.0/CONTRIBUTING.rst
--rw-r--r--   0 q         (1000) q         (1000)    15683 2023-09-07 09:34:47.000000 elasticsearch-dsl-8.9.0/Changelog.rst
--rw-r--r--   0 q         (1000) q         (1000)    10143 2022-05-23 12:42:04.000000 elasticsearch-dsl-8.9.0/LICENSE
--rw-r--r--   0 q         (1000) q         (1000)       94 2022-05-23 12:42:04.000000 elasticsearch-dsl-8.9.0/MANIFEST.in
--rw-r--r--   0 q         (1000) q         (1000)    10498 2023-09-07 09:36:11.140226 elasticsearch-dsl-8.9.0/PKG-INFO
--rw-r--r--   0 q         (1000) q         (1000)     9365 2023-09-07 09:25:59.000000 elasticsearch-dsl-8.9.0/README
-drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-09-07 09:36:11.137225 elasticsearch-dsl-8.9.0/elasticsearch_dsl/
--rw-r--r--   0 q         (1000) q         (1000)     3438 2023-09-07 09:34:47.000000 elasticsearch-dsl-8.9.0/elasticsearch_dsl/__init__.py
--rw-r--r--   0 q         (1000) q         (1000)     9449 2023-08-23 05:46:16.000000 elasticsearch-dsl-8.9.0/elasticsearch_dsl/aggs.py
--rw-r--r--   0 q         (1000) q         (1000)     8050 2023-08-23 05:46:16.000000 elasticsearch-dsl-8.9.0/elasticsearch_dsl/analysis.py
--rw-r--r--   0 q         (1000) q         (1000)     4193 2023-08-29 09:27:45.000000 elasticsearch-dsl-8.9.0/elasticsearch_dsl/connections.py
--rw-r--r--   0 q         (1000) q         (1000)    17985 2023-08-29 09:27:45.000000 elasticsearch-dsl-8.9.0/elasticsearch_dsl/document.py
--rw-r--r--   0 q         (1000) q         (1000)     1043 2022-05-23 12:42:04.000000 elasticsearch-dsl-8.9.0/elasticsearch_dsl/exceptions.py
--rw-r--r--   0 q         (1000) q         (1000)    13356 2023-08-28 11:08:30.000000 elasticsearch-dsl-8.9.0/elasticsearch_dsl/faceted_search.py
--rw-r--r--   0 q         (1000) q         (1000)    13601 2023-08-23 05:46:16.000000 elasticsearch-dsl-8.9.0/elasticsearch_dsl/field.py
--rw-r--r--   0 q         (1000) q         (1000)     3388 2023-08-23 05:46:16.000000 elasticsearch-dsl-8.9.0/elasticsearch_dsl/function.py
--rw-r--r--   0 q         (1000) q         (1000)    23499 2023-08-24 16:42:33.000000 elasticsearch-dsl-8.9.0/elasticsearch_dsl/index.py
--rw-r--r--   0 q         (1000) q         (1000)     7286 2023-08-23 05:46:16.000000 elasticsearch-dsl-8.9.0/elasticsearch_dsl/mapping.py
--rw-r--r--   0 q         (1000) q         (1000)    12213 2023-08-23 05:46:16.000000 elasticsearch-dsl-8.9.0/elasticsearch_dsl/query.py
-drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-09-07 09:36:11.139226 elasticsearch-dsl-8.9.0/elasticsearch_dsl/response/
--rw-r--r--   0 q         (1000) q         (1000)     4039 2023-08-28 10:52:59.000000 elasticsearch-dsl-8.9.0/elasticsearch_dsl/response/__init__.py
--rw-r--r--   0 q         (1000) q         (1000)     2603 2023-08-23 05:46:16.000000 elasticsearch-dsl-8.9.0/elasticsearch_dsl/response/aggs.py
--rw-r--r--   0 q         (1000) q         (1000)     1835 2023-08-23 05:46:16.000000 elasticsearch-dsl-8.9.0/elasticsearch_dsl/response/hit.py
--rw-r--r--   0 q         (1000) q         (1000)    25221 2023-08-29 09:27:45.000000 elasticsearch-dsl-8.9.0/elasticsearch_dsl/search.py
--rw-r--r--   0 q         (1000) q         (1000)     1153 2023-08-28 10:24:32.000000 elasticsearch-dsl-8.9.0/elasticsearch_dsl/serializer.py
--rw-r--r--   0 q         (1000) q         (1000)     5070 2023-08-23 05:56:33.000000 elasticsearch-dsl-8.9.0/elasticsearch_dsl/update_by_query.py
--rw-r--r--   0 q         (1000) q         (1000)    17900 2023-08-23 05:46:16.000000 elasticsearch-dsl-8.9.0/elasticsearch_dsl/utils.py
--rw-r--r--   0 q         (1000) q         (1000)     2512 2023-08-23 05:46:16.000000 elasticsearch-dsl-8.9.0/elasticsearch_dsl/wrappers.py
-drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-09-07 09:36:11.138226 elasticsearch-dsl-8.9.0/elasticsearch_dsl.egg-info/
--rw-r--r--   0 q         (1000) q         (1000)    10498 2023-09-07 09:36:11.000000 elasticsearch-dsl-8.9.0/elasticsearch_dsl.egg-info/PKG-INFO
--rw-r--r--   0 q         (1000) q         (1000)      907 2023-09-07 09:36:11.000000 elasticsearch-dsl-8.9.0/elasticsearch_dsl.egg-info/SOURCES.txt
--rw-r--r--   0 q         (1000) q         (1000)        1 2023-09-07 09:36:11.000000 elasticsearch-dsl-8.9.0/elasticsearch_dsl.egg-info/dependency_links.txt
--rw-r--r--   0 q         (1000) q         (1000)      129 2023-09-07 09:36:11.000000 elasticsearch-dsl-8.9.0/elasticsearch_dsl.egg-info/requires.txt
--rw-r--r--   0 q         (1000) q         (1000)       18 2023-09-07 09:36:11.000000 elasticsearch-dsl-8.9.0/elasticsearch_dsl.egg-info/top_level.txt
--rw-r--r--   0 q         (1000) q         (1000)      367 2023-09-07 09:36:11.140226 elasticsearch-dsl-8.9.0/setup.cfg
--rw-r--r--   0 q         (1000) q         (1000)     2663 2023-09-07 09:34:47.000000 elasticsearch-dsl-8.9.0/setup.py
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-08-29 16:42:17.531669 elasticsearch-dsl-8.9.0a1/
+-rw-r--r--   0 q         (1000) q         (1000)      136 2022-05-23 12:42:04.000000 elasticsearch-dsl-8.9.0a1/AUTHORS
+-rw-r--r--   0 q         (1000) q         (1000)     2255 2022-05-23 12:42:04.000000 elasticsearch-dsl-8.9.0a1/CONTRIBUTING.rst
+-rw-r--r--   0 q         (1000) q         (1000)    15687 2023-08-29 16:36:08.000000 elasticsearch-dsl-8.9.0a1/Changelog.rst
+-rw-r--r--   0 q         (1000) q         (1000)    10143 2022-05-23 12:42:04.000000 elasticsearch-dsl-8.9.0a1/LICENSE
+-rw-r--r--   0 q         (1000) q         (1000)       94 2022-05-23 12:42:04.000000 elasticsearch-dsl-8.9.0a1/MANIFEST.in
+-rw-r--r--   0 q         (1000) q         (1000)    10329 2023-08-29 16:42:17.531669 elasticsearch-dsl-8.9.0a1/PKG-INFO
+-rw-r--r--   0 q         (1000) q         (1000)     9194 2022-05-23 12:42:04.000000 elasticsearch-dsl-8.9.0a1/README
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-08-29 16:42:17.529669 elasticsearch-dsl-8.9.0a1/elasticsearch_dsl/
+-rw-r--r--   0 q         (1000) q         (1000)     3444 2023-08-29 16:36:08.000000 elasticsearch-dsl-8.9.0a1/elasticsearch_dsl/__init__.py
+-rw-r--r--   0 q         (1000) q         (1000)     9449 2023-08-23 05:46:16.000000 elasticsearch-dsl-8.9.0a1/elasticsearch_dsl/aggs.py
+-rw-r--r--   0 q         (1000) q         (1000)     8050 2023-08-23 05:46:16.000000 elasticsearch-dsl-8.9.0a1/elasticsearch_dsl/analysis.py
+-rw-r--r--   0 q         (1000) q         (1000)     4193 2023-08-29 09:27:45.000000 elasticsearch-dsl-8.9.0a1/elasticsearch_dsl/connections.py
+-rw-r--r--   0 q         (1000) q         (1000)    17985 2023-08-29 09:27:45.000000 elasticsearch-dsl-8.9.0a1/elasticsearch_dsl/document.py
+-rw-r--r--   0 q         (1000) q         (1000)     1043 2022-05-23 12:42:04.000000 elasticsearch-dsl-8.9.0a1/elasticsearch_dsl/exceptions.py
+-rw-r--r--   0 q         (1000) q         (1000)    13356 2023-08-28 11:08:30.000000 elasticsearch-dsl-8.9.0a1/elasticsearch_dsl/faceted_search.py
+-rw-r--r--   0 q         (1000) q         (1000)    13601 2023-08-23 05:46:16.000000 elasticsearch-dsl-8.9.0a1/elasticsearch_dsl/field.py
+-rw-r--r--   0 q         (1000) q         (1000)     3388 2023-08-23 05:46:16.000000 elasticsearch-dsl-8.9.0a1/elasticsearch_dsl/function.py
+-rw-r--r--   0 q         (1000) q         (1000)    23499 2023-08-24 16:42:33.000000 elasticsearch-dsl-8.9.0a1/elasticsearch_dsl/index.py
+-rw-r--r--   0 q         (1000) q         (1000)     7286 2023-08-23 05:46:16.000000 elasticsearch-dsl-8.9.0a1/elasticsearch_dsl/mapping.py
+-rw-r--r--   0 q         (1000) q         (1000)    12213 2023-08-23 05:46:16.000000 elasticsearch-dsl-8.9.0a1/elasticsearch_dsl/query.py
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-08-29 16:42:17.531669 elasticsearch-dsl-8.9.0a1/elasticsearch_dsl/response/
+-rw-r--r--   0 q         (1000) q         (1000)     4039 2023-08-28 10:52:59.000000 elasticsearch-dsl-8.9.0a1/elasticsearch_dsl/response/__init__.py
+-rw-r--r--   0 q         (1000) q         (1000)     2603 2023-08-23 05:46:16.000000 elasticsearch-dsl-8.9.0a1/elasticsearch_dsl/response/aggs.py
+-rw-r--r--   0 q         (1000) q         (1000)     1835 2023-08-23 05:46:16.000000 elasticsearch-dsl-8.9.0a1/elasticsearch_dsl/response/hit.py
+-rw-r--r--   0 q         (1000) q         (1000)    25221 2023-08-29 09:27:45.000000 elasticsearch-dsl-8.9.0a1/elasticsearch_dsl/search.py
+-rw-r--r--   0 q         (1000) q         (1000)     1153 2023-08-28 10:24:32.000000 elasticsearch-dsl-8.9.0a1/elasticsearch_dsl/serializer.py
+-rw-r--r--   0 q         (1000) q         (1000)     5070 2023-08-23 05:56:33.000000 elasticsearch-dsl-8.9.0a1/elasticsearch_dsl/update_by_query.py
+-rw-r--r--   0 q         (1000) q         (1000)    17900 2023-08-23 05:46:16.000000 elasticsearch-dsl-8.9.0a1/elasticsearch_dsl/utils.py
+-rw-r--r--   0 q         (1000) q         (1000)     2512 2023-08-23 05:46:16.000000 elasticsearch-dsl-8.9.0a1/elasticsearch_dsl/wrappers.py
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-08-29 16:42:17.530669 elasticsearch-dsl-8.9.0a1/elasticsearch_dsl.egg-info/
+-rw-r--r--   0 q         (1000) q         (1000)    10329 2023-08-29 16:42:17.000000 elasticsearch-dsl-8.9.0a1/elasticsearch_dsl.egg-info/PKG-INFO
+-rw-r--r--   0 q         (1000) q         (1000)      907 2023-08-29 16:42:17.000000 elasticsearch-dsl-8.9.0a1/elasticsearch_dsl.egg-info/SOURCES.txt
+-rw-r--r--   0 q         (1000) q         (1000)        1 2023-08-29 16:42:17.000000 elasticsearch-dsl-8.9.0a1/elasticsearch_dsl.egg-info/dependency_links.txt
+-rw-r--r--   0 q         (1000) q         (1000)      123 2023-08-29 16:42:17.000000 elasticsearch-dsl-8.9.0a1/elasticsearch_dsl.egg-info/requires.txt
+-rw-r--r--   0 q         (1000) q         (1000)       18 2023-08-29 16:42:17.000000 elasticsearch-dsl-8.9.0a1/elasticsearch_dsl.egg-info/top_level.txt
+-rw-r--r--   0 q         (1000) q         (1000)      367 2023-08-29 16:42:17.531669 elasticsearch-dsl-8.9.0a1/setup.cfg
+-rw-r--r--   0 q         (1000) q         (1000)     2590 2023-08-29 16:36:08.000000 elasticsearch-dsl-8.9.0a1/setup.py
```

### Comparing `elasticsearch-dsl-8.9.0/CONTRIBUTING.rst` & `elasticsearch-dsl-8.9.0a1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `elasticsearch-dsl-8.9.0/Changelog.rst` & `elasticsearch-dsl-8.9.0a1/Changelog.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 .. _changelog:
 
 Changelog
 =========
 
-8.9.0 (2023-09-07)
-------------------
+8.9.0a1 (2023-08-29)
+--------------------
 
 * Added Elasticsearch 8.x support (`#1664`_)
 * Dropped support for Python 2.7 and 3.5 (`#1606`_, contributed by `@hugovk`_)
 * Added support for Python 3.10 and 3.11 (`#1608`_, contributed by `@hugovk`_)
 * Added the ``MultiTerms`` aggregation (`#1543`_, contributed by `@Telomeraz`_)
 * Added the ``CombinedFields`` query (`#1557`_, contributed by `@Telomeraz`_)
```

### Comparing `elasticsearch-dsl-8.9.0/LICENSE` & `elasticsearch-dsl-8.9.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `elasticsearch-dsl-8.9.0/PKG-INFO` & `elasticsearch-dsl-8.9.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elasticsearch-dsl
-Version: 8.9.0
+Version: 8.9.0a1
 Summary: Python client for Elasticsearch
 Home-page: https://github.com/elasticsearch/elasticsearch-dsl-py
 Author: Elastic Client Library Maintainers
 Author-email: client-libs@elastic.co
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
@@ -61,59 +61,54 @@
 
 Compatibility
 -------------
 
 The library is compatible with all Elasticsearch versions since ``2.x`` but you
 **have to use a matching major version**:
 
-For **Elasticsearch 8.0** and later, use the major version 8 (``8.x.y``) of the
-library.
-
 For **Elasticsearch 7.0** and later, use the major version 7 (``7.x.y``) of the
 library.
 
 For **Elasticsearch 6.0** and later, use the major version 6 (``6.x.y``) of the
 library.
 
 For **Elasticsearch 5.0** and later, use the major version 5 (``5.x.y``) of the
 library.
 
 For **Elasticsearch 2.0** and later, use the major version 2 (``2.x.y``) of the
 library.
 
+
 The recommended way to set your requirements in your `setup.py` or
 `requirements.txt` is::
 
-    # Elasticsearch 8.x
-    elasticsearch-dsl>=8.0.0,<9.0.0
-
     # Elasticsearch 7.x
     elasticsearch-dsl>=7.0.0,<8.0.0
 
     # Elasticsearch 6.x
     elasticsearch-dsl>=6.0.0,<7.0.0
 
     # Elasticsearch 5.x
     elasticsearch-dsl>=5.0.0,<6.0.0
 
     # Elasticsearch 2.x
     elasticsearch-dsl>=2.0.0,<3.0.0
 
 
-The development is happening on ``main``, older branches only get bugfix releases
+The development is happening on ``master``, older branches only get bugfix releases
 
 Search Example
 --------------
 
 Let's have a typical search request written directly as a ``dict``:
 
 .. code:: python
 
     from elasticsearch import Elasticsearch
-    client = Elasticsearch("https://localhost:9200")
+    client = Elasticsearch()
 
     response = client.search(
         index="my-index",
         body={
           "query": {
             "bool": {
               "must": [{"match": {"title": "python"}}],
@@ -147,15 +142,15 @@
 Let's rewrite the example using the Python DSL:
 
 .. code:: python
 
     from elasticsearch import Elasticsearch
     from elasticsearch_dsl import Search
 
-    client = Elasticsearch("https://localhost:9200")
+    client = Elasticsearch()
 
     s = Search(using=client, index="my-index") \
         .filter("term", category="search") \
         .query("match", title="python")   \
         .exclude("match", description="beta")
 
     s.aggs.bucket('per_tag', 'terms', field='tags') \
@@ -167,33 +162,37 @@
         print(hit.meta.score, hit.title)
 
     for tag in response.aggregations.per_tag.buckets:
         print(tag.key, tag.max_lines.value)
 
 As you see, the library took care of:
 
-- creating appropriate ``Query`` objects by name (eq. "match")
-- composing queries into a compound ``bool`` query
-- putting the ``term`` query in a filter context of the ``bool`` query
-- providing a convenient access to response data
-- no curly or square brackets everywhere
+  * creating appropriate ``Query`` objects by name (eq. "match")
+
+  * composing queries into a compound ``bool`` query
+
+  * putting the ``term`` query in a filter context of the ``bool`` query
+
+  * providing a convenient access to response data
+
+  * no curly or square brackets everywhere
 
 
 Persistence Example
 -------------------
 
 Let's have a simple Python class representing an article in a blogging system:
 
 .. code:: python
 
     from datetime import datetime
     from elasticsearch_dsl import Document, Date, Integer, Keyword, Text, connections
 
     # Define a default Elasticsearch client
-    connections.create_connection(hosts="https://localhost:9200")
+    connections.create_connection(hosts=['localhost'])
 
     class Article(Document):
         title = Text(analyzer='snowball', fields={'raw': Keyword()})
         body = Text(analyzer='snowball')
         tags = Keyword()
         published_from = Date()
         lines = Integer()
@@ -225,22 +224,28 @@
 
     # Display cluster health
     print(connections.get_connection().cluster.health())
 
 
 In this example you can see:
 
-- providing a default connection
-- defining fields with mapping configuration
-- setting index name
-- defining custom methods
-- overriding the built-in ``.save()`` method to hook into the persistence
-  life cycle
-- retrieving and saving the object into Elasticsearch
-- accessing the underlying client for other APIs
+  * providing a default connection
+
+  * defining fields with mapping configuration
+
+  * setting index name
+
+  * defining custom methods
+
+  * overriding the built-in ``.save()`` method to hook into the persistence
+    life cycle
+
+  * retrieving and saving the object into Elasticsearch
+
+  * accessing the underlying client for other APIs
 
 You can see more in the persistence chapter of the documentation.
 
 Migration from ``elasticsearch-py``
 -----------------------------------
 
 You don't have to port your entire application to get the benefits of the
```

### Comparing `elasticsearch-dsl-8.9.0/README` & `elasticsearch-dsl-8.9.0a1/README`

 * *Files 2% similar despite different names*

```diff
@@ -33,59 +33,54 @@
 
 Compatibility
 -------------
 
 The library is compatible with all Elasticsearch versions since ``2.x`` but you
 **have to use a matching major version**:
 
-For **Elasticsearch 8.0** and later, use the major version 8 (``8.x.y``) of the
-library.
-
 For **Elasticsearch 7.0** and later, use the major version 7 (``7.x.y``) of the
 library.
 
 For **Elasticsearch 6.0** and later, use the major version 6 (``6.x.y``) of the
 library.
 
 For **Elasticsearch 5.0** and later, use the major version 5 (``5.x.y``) of the
 library.
 
 For **Elasticsearch 2.0** and later, use the major version 2 (``2.x.y``) of the
 library.
 
+
 The recommended way to set your requirements in your `setup.py` or
 `requirements.txt` is::
 
-    # Elasticsearch 8.x
-    elasticsearch-dsl>=8.0.0,<9.0.0
-
     # Elasticsearch 7.x
     elasticsearch-dsl>=7.0.0,<8.0.0
 
     # Elasticsearch 6.x
     elasticsearch-dsl>=6.0.0,<7.0.0
 
     # Elasticsearch 5.x
     elasticsearch-dsl>=5.0.0,<6.0.0
 
     # Elasticsearch 2.x
     elasticsearch-dsl>=2.0.0,<3.0.0
 
 
-The development is happening on ``main``, older branches only get bugfix releases
+The development is happening on ``master``, older branches only get bugfix releases
 
 Search Example
 --------------
 
 Let's have a typical search request written directly as a ``dict``:
 
 .. code:: python
 
     from elasticsearch import Elasticsearch
-    client = Elasticsearch("https://localhost:9200")
+    client = Elasticsearch()
 
     response = client.search(
         index="my-index",
         body={
           "query": {
             "bool": {
               "must": [{"match": {"title": "python"}}],
@@ -119,15 +114,15 @@
 Let's rewrite the example using the Python DSL:
 
 .. code:: python
 
     from elasticsearch import Elasticsearch
     from elasticsearch_dsl import Search
 
-    client = Elasticsearch("https://localhost:9200")
+    client = Elasticsearch()
 
     s = Search(using=client, index="my-index") \
         .filter("term", category="search") \
         .query("match", title="python")   \
         .exclude("match", description="beta")
 
     s.aggs.bucket('per_tag', 'terms', field='tags') \
@@ -139,33 +134,37 @@
         print(hit.meta.score, hit.title)
 
     for tag in response.aggregations.per_tag.buckets:
         print(tag.key, tag.max_lines.value)
 
 As you see, the library took care of:
 
-- creating appropriate ``Query`` objects by name (eq. "match")
-- composing queries into a compound ``bool`` query
-- putting the ``term`` query in a filter context of the ``bool`` query
-- providing a convenient access to response data
-- no curly or square brackets everywhere
+  * creating appropriate ``Query`` objects by name (eq. "match")
+
+  * composing queries into a compound ``bool`` query
+
+  * putting the ``term`` query in a filter context of the ``bool`` query
+
+  * providing a convenient access to response data
+
+  * no curly or square brackets everywhere
 
 
 Persistence Example
 -------------------
 
 Let's have a simple Python class representing an article in a blogging system:
 
 .. code:: python
 
     from datetime import datetime
     from elasticsearch_dsl import Document, Date, Integer, Keyword, Text, connections
 
     # Define a default Elasticsearch client
-    connections.create_connection(hosts="https://localhost:9200")
+    connections.create_connection(hosts=['localhost'])
 
     class Article(Document):
         title = Text(analyzer='snowball', fields={'raw': Keyword()})
         body = Text(analyzer='snowball')
         tags = Keyword()
         published_from = Date()
         lines = Integer()
@@ -197,22 +196,28 @@
 
     # Display cluster health
     print(connections.get_connection().cluster.health())
 
 
 In this example you can see:
 
-- providing a default connection
-- defining fields with mapping configuration
-- setting index name
-- defining custom methods
-- overriding the built-in ``.save()`` method to hook into the persistence
-  life cycle
-- retrieving and saving the object into Elasticsearch
-- accessing the underlying client for other APIs
+  * providing a default connection
+
+  * defining fields with mapping configuration
+
+  * setting index name
+
+  * defining custom methods
+
+  * overriding the built-in ``.save()`` method to hook into the persistence
+    life cycle
+
+  * retrieving and saving the object into Elasticsearch
+
+  * accessing the underlying client for other APIs
 
 You can see more in the persistence chapter of the documentation.
 
 Migration from ``elasticsearch-py``
 -----------------------------------
 
 You don't have to port your entire application to get the benefits of the
```

### Comparing `elasticsearch-dsl-8.9.0/elasticsearch_dsl/__init__.py` & `elasticsearch-dsl-8.9.0a1/elasticsearch_dsl/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 from .mapping import Mapping
 from .query import Q
 from .search import MultiSearch, Search
 from .update_by_query import UpdateByQuery
 from .utils import AttrDict, AttrList, DslBase
 from .wrappers import Range
 
-VERSION = (8, 9, 0)
+VERSION = (8, 9, 0, "a1")
 __version__ = VERSION
 __versionstr__ = ".".join(map(str, VERSION))
 __all__ = [
     "A",
     "AttrDict",
     "AttrList",
     "Binary",
```

### Comparing `elasticsearch-dsl-8.9.0/elasticsearch_dsl/aggs.py` & `elasticsearch-dsl-8.9.0a1/elasticsearch_dsl/aggs.py`

 * *Files identical despite different names*

### Comparing `elasticsearch-dsl-8.9.0/elasticsearch_dsl/analysis.py` & `elasticsearch-dsl-8.9.0a1/elasticsearch_dsl/analysis.py`

 * *Files identical despite different names*

### Comparing `elasticsearch-dsl-8.9.0/elasticsearch_dsl/connections.py` & `elasticsearch-dsl-8.9.0a1/elasticsearch_dsl/connections.py`

 * *Files identical despite different names*

### Comparing `elasticsearch-dsl-8.9.0/elasticsearch_dsl/document.py` & `elasticsearch-dsl-8.9.0a1/elasticsearch_dsl/document.py`

 * *Files identical despite different names*

### Comparing `elasticsearch-dsl-8.9.0/elasticsearch_dsl/exceptions.py` & `elasticsearch-dsl-8.9.0a1/elasticsearch_dsl/exceptions.py`

 * *Files identical despite different names*

### Comparing `elasticsearch-dsl-8.9.0/elasticsearch_dsl/faceted_search.py` & `elasticsearch-dsl-8.9.0a1/elasticsearch_dsl/faceted_search.py`

 * *Files identical despite different names*

### Comparing `elasticsearch-dsl-8.9.0/elasticsearch_dsl/field.py` & `elasticsearch-dsl-8.9.0a1/elasticsearch_dsl/field.py`

 * *Files identical despite different names*

### Comparing `elasticsearch-dsl-8.9.0/elasticsearch_dsl/function.py` & `elasticsearch-dsl-8.9.0a1/elasticsearch_dsl/function.py`

 * *Files identical despite different names*

### Comparing `elasticsearch-dsl-8.9.0/elasticsearch_dsl/index.py` & `elasticsearch-dsl-8.9.0a1/elasticsearch_dsl/index.py`

 * *Files identical despite different names*

### Comparing `elasticsearch-dsl-8.9.0/elasticsearch_dsl/mapping.py` & `elasticsearch-dsl-8.9.0a1/elasticsearch_dsl/mapping.py`

 * *Files identical despite different names*

### Comparing `elasticsearch-dsl-8.9.0/elasticsearch_dsl/query.py` & `elasticsearch-dsl-8.9.0a1/elasticsearch_dsl/query.py`

 * *Files identical despite different names*

### Comparing `elasticsearch-dsl-8.9.0/elasticsearch_dsl/response/__init__.py` & `elasticsearch-dsl-8.9.0a1/elasticsearch_dsl/response/__init__.py`

 * *Files identical despite different names*

### Comparing `elasticsearch-dsl-8.9.0/elasticsearch_dsl/response/aggs.py` & `elasticsearch-dsl-8.9.0a1/elasticsearch_dsl/response/aggs.py`

 * *Files identical despite different names*

### Comparing `elasticsearch-dsl-8.9.0/elasticsearch_dsl/response/hit.py` & `elasticsearch-dsl-8.9.0a1/elasticsearch_dsl/response/hit.py`

 * *Files identical despite different names*

### Comparing `elasticsearch-dsl-8.9.0/elasticsearch_dsl/search.py` & `elasticsearch-dsl-8.9.0a1/elasticsearch_dsl/search.py`

 * *Files identical despite different names*

### Comparing `elasticsearch-dsl-8.9.0/elasticsearch_dsl/serializer.py` & `elasticsearch-dsl-8.9.0a1/elasticsearch_dsl/serializer.py`

 * *Files identical despite different names*

### Comparing `elasticsearch-dsl-8.9.0/elasticsearch_dsl/update_by_query.py` & `elasticsearch-dsl-8.9.0a1/elasticsearch_dsl/update_by_query.py`

 * *Files identical despite different names*

### Comparing `elasticsearch-dsl-8.9.0/elasticsearch_dsl/utils.py` & `elasticsearch-dsl-8.9.0a1/elasticsearch_dsl/utils.py`

 * *Files identical despite different names*

### Comparing `elasticsearch-dsl-8.9.0/elasticsearch_dsl/wrappers.py` & `elasticsearch-dsl-8.9.0a1/elasticsearch_dsl/wrappers.py`

 * *Files identical despite different names*

### Comparing `elasticsearch-dsl-8.9.0/elasticsearch_dsl.egg-info/PKG-INFO` & `elasticsearch-dsl-8.9.0a1/elasticsearch_dsl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elasticsearch-dsl
-Version: 8.9.0
+Version: 8.9.0a1
 Summary: Python client for Elasticsearch
 Home-page: https://github.com/elasticsearch/elasticsearch-dsl-py
 Author: Elastic Client Library Maintainers
 Author-email: client-libs@elastic.co
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
@@ -61,59 +61,54 @@
 
 Compatibility
 -------------
 
 The library is compatible with all Elasticsearch versions since ``2.x`` but you
 **have to use a matching major version**:
 
-For **Elasticsearch 8.0** and later, use the major version 8 (``8.x.y``) of the
-library.
-
 For **Elasticsearch 7.0** and later, use the major version 7 (``7.x.y``) of the
 library.
 
 For **Elasticsearch 6.0** and later, use the major version 6 (``6.x.y``) of the
 library.
 
 For **Elasticsearch 5.0** and later, use the major version 5 (``5.x.y``) of the
 library.
 
 For **Elasticsearch 2.0** and later, use the major version 2 (``2.x.y``) of the
 library.
 
+
 The recommended way to set your requirements in your `setup.py` or
 `requirements.txt` is::
 
-    # Elasticsearch 8.x
-    elasticsearch-dsl>=8.0.0,<9.0.0
-
     # Elasticsearch 7.x
     elasticsearch-dsl>=7.0.0,<8.0.0
 
     # Elasticsearch 6.x
     elasticsearch-dsl>=6.0.0,<7.0.0
 
     # Elasticsearch 5.x
     elasticsearch-dsl>=5.0.0,<6.0.0
 
     # Elasticsearch 2.x
     elasticsearch-dsl>=2.0.0,<3.0.0
 
 
-The development is happening on ``main``, older branches only get bugfix releases
+The development is happening on ``master``, older branches only get bugfix releases
 
 Search Example
 --------------
 
 Let's have a typical search request written directly as a ``dict``:
 
 .. code:: python
 
     from elasticsearch import Elasticsearch
-    client = Elasticsearch("https://localhost:9200")
+    client = Elasticsearch()
 
     response = client.search(
         index="my-index",
         body={
           "query": {
             "bool": {
               "must": [{"match": {"title": "python"}}],
@@ -147,15 +142,15 @@
 Let's rewrite the example using the Python DSL:
 
 .. code:: python
 
     from elasticsearch import Elasticsearch
     from elasticsearch_dsl import Search
 
-    client = Elasticsearch("https://localhost:9200")
+    client = Elasticsearch()
 
     s = Search(using=client, index="my-index") \
         .filter("term", category="search") \
         .query("match", title="python")   \
         .exclude("match", description="beta")
 
     s.aggs.bucket('per_tag', 'terms', field='tags') \
@@ -167,33 +162,37 @@
         print(hit.meta.score, hit.title)
 
     for tag in response.aggregations.per_tag.buckets:
         print(tag.key, tag.max_lines.value)
 
 As you see, the library took care of:
 
-- creating appropriate ``Query`` objects by name (eq. "match")
-- composing queries into a compound ``bool`` query
-- putting the ``term`` query in a filter context of the ``bool`` query
-- providing a convenient access to response data
-- no curly or square brackets everywhere
+  * creating appropriate ``Query`` objects by name (eq. "match")
+
+  * composing queries into a compound ``bool`` query
+
+  * putting the ``term`` query in a filter context of the ``bool`` query
+
+  * providing a convenient access to response data
+
+  * no curly or square brackets everywhere
 
 
 Persistence Example
 -------------------
 
 Let's have a simple Python class representing an article in a blogging system:
 
 .. code:: python
 
     from datetime import datetime
     from elasticsearch_dsl import Document, Date, Integer, Keyword, Text, connections
 
     # Define a default Elasticsearch client
-    connections.create_connection(hosts="https://localhost:9200")
+    connections.create_connection(hosts=['localhost'])
 
     class Article(Document):
         title = Text(analyzer='snowball', fields={'raw': Keyword()})
         body = Text(analyzer='snowball')
         tags = Keyword()
         published_from = Date()
         lines = Integer()
@@ -225,22 +224,28 @@
 
     # Display cluster health
     print(connections.get_connection().cluster.health())
 
 
 In this example you can see:
 
-- providing a default connection
-- defining fields with mapping configuration
-- setting index name
-- defining custom methods
-- overriding the built-in ``.save()`` method to hook into the persistence
-  life cycle
-- retrieving and saving the object into Elasticsearch
-- accessing the underlying client for other APIs
+  * providing a default connection
+
+  * defining fields with mapping configuration
+
+  * setting index name
+
+  * defining custom methods
+
+  * overriding the built-in ``.save()`` method to hook into the persistence
+    life cycle
+
+  * retrieving and saving the object into Elasticsearch
+
+  * accessing the underlying client for other APIs
 
 You can see more in the persistence chapter of the documentation.
 
 Migration from ``elasticsearch-py``
 -----------------------------------
 
 You don't have to port your entire application to get the benefits of the
```

### Comparing `elasticsearch-dsl-8.9.0/elasticsearch_dsl.egg-info/SOURCES.txt` & `elasticsearch-dsl-8.9.0a1/elasticsearch_dsl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elasticsearch-dsl-8.9.0/setup.py` & `elasticsearch-dsl-8.9.0a1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #  specific language governing permissions and limitations
 #  under the License.
 
 from os.path import dirname, join
 
 from setuptools import find_packages, setup
 
-VERSION = (8, 9, 0)
+VERSION = (8, 9, 0, "a1")
 __version__ = VERSION
 __versionstr__ = ".".join(map(str, VERSION))
 
 f = open(join(dirname(__file__), "README"))
 long_description = f.read().strip()
 f.close()
 
@@ -34,17 +34,16 @@
 
 develop_requires = [
     "pytest",
     "pytest-cov",
     "pytest-mock",
     "pytz",
     "coverage",
-    # Override Read the Docs default (sphinx<2 and sphinx-rtd-theme<0.5)
-    "sphinx>2",
-    "sphinx-rtd-theme>0.5",
+    "sphinx",
+    "sphinx_rtd_theme",
 ]
 
 setup(
     name="elasticsearch-dsl",
     description="Python client for Elasticsearch",
     license="Apache-2.0",
     url="https://github.com/elasticsearch/elasticsearch-dsl-py",
```

