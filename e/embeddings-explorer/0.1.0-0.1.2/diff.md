# Comparing `tmp/embeddings_explorer-0.1.0.tar.gz` & `tmp/embeddings_explorer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embeddings_explorer-0.1.0.tar", last modified: Mon Apr  1 09:51:15 2024, max compression
+gzip compressed data, was "embeddings_explorer-0.1.2.tar", last modified: Wed Apr  3 06:11:11 2024, max compression
```

## Comparing `embeddings_explorer-0.1.0.tar` & `embeddings_explorer-0.1.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 Edo        (501) staff       (20)        0 2024-04-01 09:51:15.029213 embeddings_explorer-0.1.0/
--rw-r--r--   0 Edo        (501) staff       (20)    11357 2024-03-23 14:26:53.000000 embeddings_explorer-0.1.0/LICENSE
--rw-r--r--   0 Edo        (501) staff       (20)      611 2024-04-01 09:51:15.028832 embeddings_explorer-0.1.0/PKG-INFO
--rw-r--r--   0 Edo        (501) staff       (20)      108 2024-03-31 16:27:25.000000 embeddings_explorer-0.1.0/README.md
-drwxr-xr-x   0 Edo        (501) staff       (20)        0 2024-04-01 09:51:15.009493 embeddings_explorer-0.1.0/embeddings_explorer/
--rw-r--r--   0 Edo        (501) staff       (20)        0 2024-03-23 15:12:38.000000 embeddings_explorer-0.1.0/embeddings_explorer/__init__.py
-drwxr-xr-x   0 Edo        (501) staff       (20)        0 2024-04-01 09:51:15.014020 embeddings_explorer-0.1.0/embeddings_explorer/corpus/
--rw-r--r--   0 Edo        (501) staff       (20)       99 2024-04-01 07:41:17.000000 embeddings_explorer-0.1.0/embeddings_explorer/corpus/__init__.py
--rw-r--r--   0 Edo        (501) staff       (20)      793 2024-03-24 08:47:42.000000 embeddings_explorer-0.1.0/embeddings_explorer/corpus/brown_corpus_provider.py
--rw-r--r--   0 Edo        (501) staff       (20)      466 2024-03-24 08:47:27.000000 embeddings_explorer-0.1.0/embeddings_explorer/corpus/corpus_provider.py
--rw-r--r--   0 Edo        (501) staff       (20)     1438 2024-03-24 09:00:55.000000 embeddings_explorer-0.1.0/embeddings_explorer/corpus/food_corpus_provider.py
-drwxr-xr-x   0 Edo        (501) staff       (20)        0 2024-04-01 09:51:15.018616 embeddings_explorer-0.1.0/embeddings_explorer/graph/
--rw-r--r--   0 Edo        (501) staff       (20)      214 2024-04-01 07:41:55.000000 embeddings_explorer-0.1.0/embeddings_explorer/graph/__init__.py
--rw-r--r--   0 Edo        (501) staff       (20)     1083 2024-03-23 18:36:21.000000 embeddings_explorer-0.1.0/embeddings_explorer/graph/bfs_traverser.py
--rw-r--r--   0 Edo        (501) staff       (20)      407 2024-03-23 15:21:00.000000 embeddings_explorer-0.1.0/embeddings_explorer/graph/graph_constructor.py
--rw-r--r--   0 Edo        (501) staff       (20)     2177 2024-03-25 08:20:41.000000 embeddings_explorer-0.1.0/embeddings_explorer/graph/knn_graph.py
--rw-r--r--   0 Edo        (501) staff       (20)      683 2024-03-23 18:30:45.000000 embeddings_explorer-0.1.0/embeddings_explorer/graph/traverser.py
--rw-r--r--   0 Edo        (501) staff       (20)      628 2024-03-23 18:31:36.000000 embeddings_explorer-0.1.0/embeddings_explorer/graph/weighted_traverser.py
-drwxr-xr-x   0 Edo        (501) staff       (20)        0 2024-04-01 09:51:15.023760 embeddings_explorer-0.1.0/embeddings_explorer/models/
--rw-r--r--   0 Edo        (501) staff       (20)      186 2024-04-01 07:42:34.000000 embeddings_explorer-0.1.0/embeddings_explorer/models/__init__.py
--rw-r--r--   0 Edo        (501) staff       (20)     1028 2024-03-24 14:52:53.000000 embeddings_explorer-0.1.0/embeddings_explorer/models/bert.py
--rw-r--r--   0 Edo        (501) staff       (20)      779 2024-03-24 14:41:51.000000 embeddings_explorer-0.1.0/embeddings_explorer/models/generator.py
--rw-r--r--   0 Edo        (501) staff       (20)     1272 2024-03-25 07:36:21.000000 embeddings_explorer-0.1.0/embeddings_explorer/models/openai.py
--rw-r--r--   0 Edo        (501) staff       (20)      686 2024-03-24 14:52:41.000000 embeddings_explorer-0.1.0/embeddings_explorer/models/sentence_bert.py
--rw-r--r--   0 Edo        (501) staff       (20)     1341 2024-03-24 15:01:41.000000 embeddings_explorer-0.1.0/embeddings_explorer/models/voyage.py
-drwxr-xr-x   0 Edo        (501) staff       (20)        0 2024-04-01 09:51:15.025279 embeddings_explorer-0.1.0/embeddings_explorer/orchestrator/
--rw-r--r--   0 Edo        (501) staff       (20)       41 2024-04-01 07:42:55.000000 embeddings_explorer-0.1.0/embeddings_explorer/orchestrator/__init__.py
--rw-r--r--   0 Edo        (501) staff       (20)     2746 2024-03-25 07:11:06.000000 embeddings_explorer-0.1.0/embeddings_explorer/orchestrator/explorer.py
-drwxr-xr-x   0 Edo        (501) staff       (20)        0 2024-04-01 09:51:15.026262 embeddings_explorer-0.1.0/embeddings_explorer/utils/
--rw-r--r--   0 Edo        (501) staff       (20)        0 2024-03-23 15:13:26.000000 embeddings_explorer-0.1.0/embeddings_explorer/utils/__init__.py
--rw-r--r--   0 Edo        (501) staff       (20)     1328 2024-03-24 14:40:46.000000 embeddings_explorer-0.1.0/embeddings_explorer/utils/cache.py
-drwxr-xr-x   0 Edo        (501) staff       (20)        0 2024-04-01 09:51:15.011102 embeddings_explorer-0.1.0/embeddings_explorer.egg-info/
--rw-r--r--   0 Edo        (501) staff       (20)      611 2024-04-01 09:51:14.000000 embeddings_explorer-0.1.0/embeddings_explorer.egg-info/PKG-INFO
--rw-r--r--   0 Edo        (501) staff       (20)     1152 2024-04-01 09:51:14.000000 embeddings_explorer-0.1.0/embeddings_explorer.egg-info/SOURCES.txt
--rw-r--r--   0 Edo        (501) staff       (20)        1 2024-04-01 09:51:14.000000 embeddings_explorer-0.1.0/embeddings_explorer.egg-info/dependency_links.txt
--rw-r--r--   0 Edo        (501) staff       (20)      222 2024-04-01 09:51:14.000000 embeddings_explorer-0.1.0/embeddings_explorer.egg-info/requires.txt
--rw-r--r--   0 Edo        (501) staff       (20)       26 2024-04-01 09:51:14.000000 embeddings_explorer-0.1.0/embeddings_explorer.egg-info/top_level.txt
--rw-r--r--   0 Edo        (501) staff       (20)       38 2024-04-01 09:51:15.029399 embeddings_explorer-0.1.0/setup.cfg
--rw-r--r--   0 Edo        (501) staff       (20)     1023 2024-04-01 09:50:10.000000 embeddings_explorer-0.1.0/setup.py
-drwxr-xr-x   0 Edo        (501) staff       (20)        0 2024-04-01 09:51:15.027772 embeddings_explorer-0.1.0/tests/
--rw-r--r--   0 Edo        (501) staff       (20)        0 2024-03-23 15:13:48.000000 embeddings_explorer-0.1.0/tests/__init__.py
--rw-r--r--   0 Edo        (501) staff       (20)      534 2024-03-23 15:17:07.000000 embeddings_explorer-0.1.0/tests/test_generators.py
+drwxr-xr-x   0 Edo        (501) staff       (20)        0 2024-04-03 06:11:11.511606 embeddings_explorer-0.1.2/
+-rw-r--r--   0 Edo        (501) staff       (20)    11357 2024-03-23 14:26:53.000000 embeddings_explorer-0.1.2/LICENSE
+-rw-r--r--   0 Edo        (501) staff       (20)     2762 2024-04-03 06:11:11.511347 embeddings_explorer-0.1.2/PKG-INFO
+-rw-r--r--   0 Edo        (501) staff       (20)     2259 2024-04-03 06:04:51.000000 embeddings_explorer-0.1.2/README.md
+drwxr-xr-x   0 Edo        (501) staff       (20)        0 2024-04-03 06:11:11.501022 embeddings_explorer-0.1.2/embeddings_explorer/
+-rw-r--r--   0 Edo        (501) staff       (20)        0 2024-03-23 15:12:38.000000 embeddings_explorer-0.1.2/embeddings_explorer/__init__.py
+drwxr-xr-x   0 Edo        (501) staff       (20)        0 2024-04-03 06:11:11.504131 embeddings_explorer-0.1.2/embeddings_explorer/corpus/
+-rw-r--r--   0 Edo        (501) staff       (20)      195 2024-04-02 14:19:21.000000 embeddings_explorer-0.1.2/embeddings_explorer/corpus/__init__.py
+-rw-r--r--   0 Edo        (501) staff       (20)      793 2024-03-24 08:47:42.000000 embeddings_explorer-0.1.2/embeddings_explorer/corpus/brown_corpus_provider.py
+-rw-r--r--   0 Edo        (501) staff       (20)      466 2024-03-24 08:47:27.000000 embeddings_explorer-0.1.2/embeddings_explorer/corpus/corpus_provider.py
+-rw-r--r--   0 Edo        (501) staff       (20)     1438 2024-03-24 09:00:55.000000 embeddings_explorer-0.1.2/embeddings_explorer/corpus/food_corpus_provider.py
+drwxr-xr-x   0 Edo        (501) staff       (20)        0 2024-04-03 06:11:11.506520 embeddings_explorer-0.1.2/embeddings_explorer/graph/
+-rw-r--r--   0 Edo        (501) staff       (20)      214 2024-04-01 07:41:55.000000 embeddings_explorer-0.1.2/embeddings_explorer/graph/__init__.py
+-rw-r--r--   0 Edo        (501) staff       (20)     1083 2024-03-23 18:36:21.000000 embeddings_explorer-0.1.2/embeddings_explorer/graph/bfs_traverser.py
+-rw-r--r--   0 Edo        (501) staff       (20)      407 2024-03-23 15:21:00.000000 embeddings_explorer-0.1.2/embeddings_explorer/graph/graph_constructor.py
+-rw-r--r--   0 Edo        (501) staff       (20)     2169 2024-04-02 15:02:06.000000 embeddings_explorer-0.1.2/embeddings_explorer/graph/knn_graph.py
+-rw-r--r--   0 Edo        (501) staff       (20)      683 2024-04-03 06:08:54.000000 embeddings_explorer-0.1.2/embeddings_explorer/graph/traverser.py
+-rw-r--r--   0 Edo        (501) staff       (20)      628 2024-04-03 06:08:54.000000 embeddings_explorer-0.1.2/embeddings_explorer/graph/weighted_traverser.py
+drwxr-xr-x   0 Edo        (501) staff       (20)        0 2024-04-03 06:11:11.509191 embeddings_explorer-0.1.2/embeddings_explorer/models/
+-rw-r--r--   0 Edo        (501) staff       (20)      186 2024-04-01 07:42:34.000000 embeddings_explorer-0.1.2/embeddings_explorer/models/__init__.py
+-rw-r--r--   0 Edo        (501) staff       (20)     1028 2024-03-24 14:52:53.000000 embeddings_explorer-0.1.2/embeddings_explorer/models/bert.py
+-rw-r--r--   0 Edo        (501) staff       (20)      779 2024-03-24 14:41:51.000000 embeddings_explorer-0.1.2/embeddings_explorer/models/generator.py
+-rw-r--r--   0 Edo        (501) staff       (20)     1272 2024-03-25 07:36:21.000000 embeddings_explorer-0.1.2/embeddings_explorer/models/openai.py
+-rw-r--r--   0 Edo        (501) staff       (20)      686 2024-03-24 14:52:41.000000 embeddings_explorer-0.1.2/embeddings_explorer/models/sentence_bert.py
+-rw-r--r--   0 Edo        (501) staff       (20)     1341 2024-03-24 15:01:41.000000 embeddings_explorer-0.1.2/embeddings_explorer/models/voyage.py
+drwxr-xr-x   0 Edo        (501) staff       (20)        0 2024-04-03 06:11:11.509857 embeddings_explorer-0.1.2/embeddings_explorer/orchestrator/
+-rw-r--r--   0 Edo        (501) staff       (20)       41 2024-04-01 07:42:55.000000 embeddings_explorer-0.1.2/embeddings_explorer/orchestrator/__init__.py
+-rw-r--r--   0 Edo        (501) staff       (20)     2746 2024-03-25 07:11:06.000000 embeddings_explorer-0.1.2/embeddings_explorer/orchestrator/explorer.py
+drwxr-xr-x   0 Edo        (501) staff       (20)        0 2024-04-03 06:11:11.510390 embeddings_explorer-0.1.2/embeddings_explorer/utils/
+-rw-r--r--   0 Edo        (501) staff       (20)        0 2024-03-23 15:13:26.000000 embeddings_explorer-0.1.2/embeddings_explorer/utils/__init__.py
+-rw-r--r--   0 Edo        (501) staff       (20)     1328 2024-03-24 14:40:46.000000 embeddings_explorer-0.1.2/embeddings_explorer/utils/cache.py
+drwxr-xr-x   0 Edo        (501) staff       (20)        0 2024-04-03 06:11:11.502835 embeddings_explorer-0.1.2/embeddings_explorer.egg-info/
+-rw-r--r--   0 Edo        (501) staff       (20)     2762 2024-04-03 06:11:11.000000 embeddings_explorer-0.1.2/embeddings_explorer.egg-info/PKG-INFO
+-rw-r--r--   0 Edo        (501) staff       (20)     1152 2024-04-03 06:11:11.000000 embeddings_explorer-0.1.2/embeddings_explorer.egg-info/SOURCES.txt
+-rw-r--r--   0 Edo        (501) staff       (20)        1 2024-04-03 06:11:11.000000 embeddings_explorer-0.1.2/embeddings_explorer.egg-info/dependency_links.txt
+-rw-r--r--   0 Edo        (501) staff       (20)      222 2024-04-03 06:11:11.000000 embeddings_explorer-0.1.2/embeddings_explorer.egg-info/requires.txt
+-rw-r--r--   0 Edo        (501) staff       (20)       26 2024-04-03 06:11:11.000000 embeddings_explorer-0.1.2/embeddings_explorer.egg-info/top_level.txt
+-rw-r--r--   0 Edo        (501) staff       (20)       38 2024-04-03 06:11:11.511703 embeddings_explorer-0.1.2/setup.cfg
+-rw-r--r--   0 Edo        (501) staff       (20)     1023 2024-04-03 06:10:58.000000 embeddings_explorer-0.1.2/setup.py
+drwxr-xr-x   0 Edo        (501) staff       (20)        0 2024-04-03 06:11:11.510929 embeddings_explorer-0.1.2/tests/
+-rw-r--r--   0 Edo        (501) staff       (20)        0 2024-03-23 15:13:48.000000 embeddings_explorer-0.1.2/tests/__init__.py
+-rw-r--r--   0 Edo        (501) staff       (20)      534 2024-03-23 15:17:07.000000 embeddings_explorer-0.1.2/tests/test_generators.py
```

### Comparing `embeddings_explorer-0.1.0/LICENSE` & `embeddings_explorer-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `embeddings_explorer-0.1.0/embeddings_explorer/corpus/brown_corpus_provider.py` & `embeddings_explorer-0.1.2/embeddings_explorer/corpus/brown_corpus_provider.py`

 * *Files identical despite different names*

### Comparing `embeddings_explorer-0.1.0/embeddings_explorer/corpus/food_corpus_provider.py` & `embeddings_explorer-0.1.2/embeddings_explorer/corpus/food_corpus_provider.py`

 * *Files identical despite different names*

### Comparing `embeddings_explorer-0.1.0/embeddings_explorer/graph/bfs_traverser.py` & `embeddings_explorer-0.1.2/embeddings_explorer/graph/bfs_traverser.py`

 * *Files identical despite different names*

### Comparing `embeddings_explorer-0.1.0/embeddings_explorer/graph/knn_graph.py` & `embeddings_explorer-0.1.2/embeddings_explorer/graph/knn_graph.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,28 +26,28 @@
 
         # Normalize embeddings for cosine metric
         if self.metric == 'cosine':
             embeddings_matrix = embeddings_matrix / \
                 np.linalg.norm(embeddings_matrix, axis=1, keepdims=True)
 
         knn_model = NearestNeighbors(
-            n_neighbors=self.k + 1, metric=self.metric).fit(embeddings_matrix)
+            n_neighbors=self.k, metric=self.metric).fit(embeddings_matrix)
         distances, indices = knn_model.kneighbors(embeddings_matrix)
 
         if self.metric == 'euclidean' and self.normalize_euclidean:
             # Normalize Euclidean distances by the square root of the number of dimensions
             dimensionality = embeddings_matrix.shape[1]
             distances = distances / np.sqrt(dimensionality)
 
         G = nx.Graph()
 
         for i, label in enumerate(labels):
             G.add_node(label, embedding=embeddings[label])
 
-            for j in range(1, self.k + 1):  # Skip the node itself
+            for j in range(1, self.k):  # Skip the node itself
                 neighbor_label = labels[indices[i][j]]
                 if self.weighted:
                     distance = distances[i][j]
                     G.add_edge(label, neighbor_label, weight=distance)
                 else:
                     G.add_edge(label, neighbor_label)
```

### Comparing `embeddings_explorer-0.1.0/embeddings_explorer/graph/traverser.py` & `embeddings_explorer-0.1.2/embeddings_explorer/graph/traverser.py`

 * *Files identical despite different names*

### Comparing `embeddings_explorer-0.1.0/embeddings_explorer/graph/weighted_traverser.py` & `embeddings_explorer-0.1.2/embeddings_explorer/graph/weighted_traverser.py`

 * *Files identical despite different names*

### Comparing `embeddings_explorer-0.1.0/embeddings_explorer/models/bert.py` & `embeddings_explorer-0.1.2/embeddings_explorer/models/bert.py`

 * *Files identical despite different names*

### Comparing `embeddings_explorer-0.1.0/embeddings_explorer/models/generator.py` & `embeddings_explorer-0.1.2/embeddings_explorer/models/generator.py`

 * *Files identical despite different names*

### Comparing `embeddings_explorer-0.1.0/embeddings_explorer/models/openai.py` & `embeddings_explorer-0.1.2/embeddings_explorer/models/openai.py`

 * *Files identical despite different names*

### Comparing `embeddings_explorer-0.1.0/embeddings_explorer/models/sentence_bert.py` & `embeddings_explorer-0.1.2/embeddings_explorer/models/sentence_bert.py`

 * *Files identical despite different names*

### Comparing `embeddings_explorer-0.1.0/embeddings_explorer/models/voyage.py` & `embeddings_explorer-0.1.2/embeddings_explorer/models/voyage.py`

 * *Files identical despite different names*

### Comparing `embeddings_explorer-0.1.0/embeddings_explorer/orchestrator/explorer.py` & `embeddings_explorer-0.1.2/embeddings_explorer/orchestrator/explorer.py`

 * *Files identical despite different names*

### Comparing `embeddings_explorer-0.1.0/embeddings_explorer/utils/cache.py` & `embeddings_explorer-0.1.2/embeddings_explorer/utils/cache.py`

 * *Files identical despite different names*

### Comparing `embeddings_explorer-0.1.0/embeddings_explorer.egg-info/SOURCES.txt` & `embeddings_explorer-0.1.2/embeddings_explorer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `embeddings_explorer-0.1.0/setup.py` & `embeddings_explorer-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='embeddings_explorer',
-    version='0.1.0',
+    version='0.1.2',
     author='Edoardo Lanzini',
     author_email='edoardo.lanzini@gmail.com',
     description='A package for generating, exploring, and visualizing word embeddings graphs.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/elanzini/pineapple_on_pizza',
     packages=find_packages(),
```

### Comparing `embeddings_explorer-0.1.0/tests/test_generators.py` & `embeddings_explorer-0.1.2/tests/test_generators.py`

 * *Files identical despite different names*

