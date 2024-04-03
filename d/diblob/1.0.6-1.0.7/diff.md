# Comparing `tmp/diblob-1.0.6.tar.gz` & `tmp/diblob-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diblob-1.0.6.tar", last modified: Thu Feb 22 21:57:37 2024, max compression
+gzip compressed data, was "diblob-1.0.7.tar", last modified: Wed Apr  3 17:44:04 2024, max compression
```

## Comparing `diblob-1.0.6.tar` & `diblob-1.0.7.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 jakub      (501) staff       (20)        0 2024-02-22 21:57:37.851927 diblob-1.0.6/
--rw-r--r--   0 jakub      (501) staff       (20)    22462 2024-02-22 21:57:37.851667 diblob-1.0.6/PKG-INFO
--rw-r--r--   0 jakub      (501) staff       (20)    22018 2024-02-22 18:28:33.000000 diblob-1.0.6/README.md
--rw-r--r--   0 jakub      (501) staff       (20)       38 2024-02-22 21:57:37.851961 diblob-1.0.6/setup.cfg
--rw-r--r--   0 jakub      (501) staff       (20)      695 2024-02-22 21:55:55.000000 diblob-1.0.6/setup.py
-drwxr-xr-x   0 jakub      (501) staff       (20)        0 2024-02-22 21:57:37.849688 diblob-1.0.6/src/
-drwxr-xr-x   0 jakub      (501) staff       (20)        0 2024-02-22 21:57:37.850633 diblob-1.0.6/src/diblob/
--rw-r--r--   0 jakub      (501) staff       (20)       80 2024-02-11 18:09:23.000000 diblob-1.0.6/src/diblob/__init__.py
--rw-r--r--   0 jakub      (501) staff       (20)     3964 2024-02-22 17:41:02.000000 diblob-1.0.6/src/diblob/algorithms.py
--rw-r--r--   0 jakub      (501) staff       (20)     4134 2024-02-22 17:19:30.000000 diblob-1.0.6/src/diblob/components.py
--rw-r--r--   0 jakub      (501) staff       (20)    20753 2024-02-22 18:30:00.000000 diblob-1.0.6/src/diblob/digraph_manager.py
--rw-r--r--   0 jakub      (501) staff       (20)     1681 2024-02-11 18:16:55.000000 diblob-1.0.6/src/diblob/exceptions.py
--rw-r--r--   0 jakub      (501) staff       (20)     3888 2024-02-18 17:18:38.000000 diblob-1.0.6/src/diblob/factory.py
--rw-r--r--   0 jakub      (501) staff       (20)     3090 2024-02-22 17:39:46.000000 diblob-1.0.6/src/diblob/tools.py
-drwxr-xr-x   0 jakub      (501) staff       (20)        0 2024-02-22 21:57:37.851048 diblob-1.0.6/src/diblob.egg-info/
--rw-r--r--   0 jakub      (501) staff       (20)    22462 2024-02-22 21:57:37.000000 diblob-1.0.6/src/diblob.egg-info/PKG-INFO
--rw-r--r--   0 jakub      (501) staff       (20)      438 2024-02-22 21:57:37.000000 diblob-1.0.6/src/diblob.egg-info/SOURCES.txt
--rw-r--r--   0 jakub      (501) staff       (20)        1 2024-02-22 21:57:37.000000 diblob-1.0.6/src/diblob.egg-info/dependency_links.txt
--rw-r--r--   0 jakub      (501) staff       (20)        7 2024-02-22 21:57:37.000000 diblob-1.0.6/src/diblob.egg-info/top_level.txt
-drwxr-xr-x   0 jakub      (501) staff       (20)        0 2024-02-22 21:57:37.851471 diblob-1.0.6/tests/
--rw-r--r--   0 jakub      (501) staff       (20)     1958 2024-02-18 17:18:38.000000 diblob-1.0.6/tests/test_components.py
--rw-r--r--   0 jakub      (501) staff       (20)    11048 2024-02-18 17:18:38.000000 diblob-1.0.6/tests/test_digraph_manager.py
--rw-r--r--   0 jakub      (501) staff       (20)     6876 2024-02-19 19:23:58.000000 diblob-1.0.6/tests/test_exploratory_unit_tests.py
--rw-r--r--   0 jakub      (501) staff       (20)     9180 2024-02-18 17:18:38.000000 diblob-1.0.6/tests/test_factory.py
+drwxr-xr-x   0 jakub      (501) staff       (20)        0 2024-04-03 17:44:04.149492 diblob-1.0.7/
+-rw-r--r--   0 jakub      (501) staff       (20)    23332 2024-04-03 17:44:04.149165 diblob-1.0.7/PKG-INFO
+-rw-r--r--   0 jakub      (501) staff       (20)    22908 2024-03-24 13:32:23.000000 diblob-1.0.7/README.md
+-rw-r--r--   0 jakub      (501) staff       (20)       38 2024-04-03 17:44:04.149529 diblob-1.0.7/setup.cfg
+-rw-r--r--   0 jakub      (501) staff       (20)      675 2024-04-03 17:43:02.000000 diblob-1.0.7/setup.py
+drwxr-xr-x   0 jakub      (501) staff       (20)        0 2024-04-03 17:44:04.143990 diblob-1.0.7/src/
+drwxr-xr-x   0 jakub      (501) staff       (20)        0 2024-04-03 17:44:04.147031 diblob-1.0.7/src/diblob/
+-rw-r--r--   0 jakub      (501) staff       (20)      126 2024-04-03 17:30:37.000000 diblob-1.0.7/src/diblob/__init__.py
+-rw-r--r--   0 jakub      (501) staff       (20)     3964 2024-02-22 17:41:02.000000 diblob-1.0.7/src/diblob/algorithms.py
+-rw-r--r--   0 jakub      (501) staff       (20)     4134 2024-02-22 17:19:30.000000 diblob-1.0.7/src/diblob/components.py
+-rw-r--r--   0 jakub      (501) staff       (20)    21469 2024-04-03 17:30:58.000000 diblob-1.0.7/src/diblob/digraph_manager.py
+-rw-r--r--   0 jakub      (501) staff       (20)     2546 2024-04-03 16:40:02.000000 diblob-1.0.7/src/diblob/exceptions.py
+-rw-r--r--   0 jakub      (501) staff       (20)     5171 2024-03-24 13:32:23.000000 diblob-1.0.7/src/diblob/factory.py
+-rw-r--r--   0 jakub      (501) staff       (20)     6725 2024-04-03 16:40:02.000000 diblob-1.0.7/src/diblob/generators.py
+-rw-r--r--   0 jakub      (501) staff       (20)     3090 2024-04-03 17:15:55.000000 diblob-1.0.7/src/diblob/tools.py
+drwxr-xr-x   0 jakub      (501) staff       (20)        0 2024-04-03 17:44:04.147569 diblob-1.0.7/src/diblob.egg-info/
+-rw-r--r--   0 jakub      (501) staff       (20)    23332 2024-04-03 17:44:04.000000 diblob-1.0.7/src/diblob.egg-info/PKG-INFO
+-rw-r--r--   0 jakub      (501) staff       (20)      463 2024-04-03 17:44:04.000000 diblob-1.0.7/src/diblob.egg-info/SOURCES.txt
+-rw-r--r--   0 jakub      (501) staff       (20)        1 2024-04-03 17:44:04.000000 diblob-1.0.7/src/diblob.egg-info/dependency_links.txt
+-rw-r--r--   0 jakub      (501) staff       (20)        7 2024-04-03 17:44:04.000000 diblob-1.0.7/src/diblob.egg-info/top_level.txt
+drwxr-xr-x   0 jakub      (501) staff       (20)        0 2024-04-03 17:44:04.148797 diblob-1.0.7/tests/
+-rw-r--r--   0 jakub      (501) staff       (20)     1958 2024-02-18 17:18:38.000000 diblob-1.0.7/tests/test_components.py
+-rw-r--r--   0 jakub      (501) staff       (20)    12368 2024-03-24 13:32:23.000000 diblob-1.0.7/tests/test_digraph_manager.py
+-rw-r--r--   0 jakub      (501) staff       (20)     6876 2024-02-19 19:23:58.000000 diblob-1.0.7/tests/test_exploratory_unit_tests.py
+-rw-r--r--   0 jakub      (501) staff       (20)    11271 2024-03-24 13:32:23.000000 diblob-1.0.7/tests/test_factory.py
```

### Comparing `diblob-1.0.6/PKG-INFO` & `diblob-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: diblob
-Version: 1.0.6
+Version: 1.0.7
 Summary: A simple example package
-Home-page: https://github.com/Zeleczek-kodowniczek/Diblob/tree/main
+Home-page: https://github.com/JakubZelek/Diblob
 Author: Jakub Zelek
 Author-email: jakub.zelek@doctoral.uj.edu.pl
 License: MIT
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -261,14 +261,21 @@
 
 - `compress_diblob(self, diblob_id: str)`
   - `diblob_id: str`: The ID of the Diblob that is to be compressed.
  <br /><br /> This method compresses the specified Diblob into a single node, effectively consolidating its structure for simplified representation:
 
 <img width="939" alt="image" src="https://github.com/Zeleczek-kodowniczek/Diblob/assets/72871011/589d935f-0dab-49c7-aec3-22be0be92404">
 
+- `join_diblobs(self, diblob_fst_id: str, diblob_snd_id: str, join_id: str)`
+  - `diblob_fst_id: str`: The ID of the first Diblob that is to be joined.
+  - `diblob_snd_id: str`: The ID of the second Diblob that is to be compressed.
+  - `join_id: str`: The ID of the joined Diblob.
+ <br /><br /> This method join two diblobs which have the same `parent_id`:
+
+<img width="1028" alt="image" src="https://github.com/JakubZelek/Diblob/assets/72871011/a74ecf81-bee4-4e81-b598-e890fa14ec21">
 
 - `merge_edges(self, edge_1: Edge, edge_2: Edge)`
   - `edge_1: Edge`: The first edge to be merged.
   - `edge_2: Edge`: The second edge to be merged.
  <br /><br /> Merges two compatible edges into one, provided the head of edge_1 is the same as the tail of edge_2, and edge_2 has exactly one incoming and one outgoing edge.
 - `get_multiple_edge_ids(self, *edge_ids : tuple[str])`
   - `*edge_ids : tuple[str]`: The edge IDs for which the operation will be performed.
@@ -392,23 +399,28 @@
 
 - `generate_bipartite_digraph(digraph_manager: DigraphManager)`
   - `digraph_manager: DigraphManager` - DigraphManager which is the base for bipartite digraph contruction.
  <br><br> enable bipartite digraph creation:
 
 <img width="1028" alt="image" src="https://github.com/Zeleczek-kodowniczek/Diblob/assets/72871011/1f3a686e-c1ef-4a41-8fa2-58a67a83fd12">
 
+- `generate_flow_digraph(digraph_manager: DigraphManager)`
+  - `digraph_manager: DigraphManager` - DigraphManager which is the base for flow digraph contruction.
+ <br><br> enable flow digraph creation (commonly used in control flow algorithm like the Ford-Fulkerson algorithm):
+
+<img width="944" alt="image" src="https://github.com/JakubZelek/Diblob/assets/72871011/9739207a-73d9-4ca4-98c8-e41116a17509">
 
-## Aghoritms
+## Algorithms
 In order to working with diblob explanation, DFS, DFSA and Dijkstra algorithms are created. 
 
 - DFS - Deep first search alghoritm.
 - DFSA - modification of the DFS (with the nodes visit time)
 - DijkstraAlgorithm - the shortes paths between node and the others.
 
-Alghoritms use duck typing. GraphManager instance have to be delivered during creation. Then `run` methon can be used on selected node_id (in DijkstraAlgorithm `cost_function` as a dict can be also delivered)
+Algorithm use duck typing. GraphManager instance have to be delivered during creation. Then `run` methon can be used on selected node_id (in DijkstraAlgorithm `cost_function` as a dict can be also delivered)
 
 Example of run:
 
  <br><br>
 ```python
 from diblob import DigraphManager
 from diblob.algorithms import DFS, DFSA, DijkstraAlgorithm
```

### Comparing `diblob-1.0.6/README.md` & `diblob-1.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -247,14 +247,21 @@
 
 - `compress_diblob(self, diblob_id: str)`
   - `diblob_id: str`: The ID of the Diblob that is to be compressed.
  <br /><br /> This method compresses the specified Diblob into a single node, effectively consolidating its structure for simplified representation:
 
 <img width="939" alt="image" src="https://github.com/Zeleczek-kodowniczek/Diblob/assets/72871011/589d935f-0dab-49c7-aec3-22be0be92404">
 
+- `join_diblobs(self, diblob_fst_id: str, diblob_snd_id: str, join_id: str)`
+  - `diblob_fst_id: str`: The ID of the first Diblob that is to be joined.
+  - `diblob_snd_id: str`: The ID of the second Diblob that is to be compressed.
+  - `join_id: str`: The ID of the joined Diblob.
+ <br /><br /> This method join two diblobs which have the same `parent_id`:
+
+<img width="1028" alt="image" src="https://github.com/JakubZelek/Diblob/assets/72871011/a74ecf81-bee4-4e81-b598-e890fa14ec21">
 
 - `merge_edges(self, edge_1: Edge, edge_2: Edge)`
   - `edge_1: Edge`: The first edge to be merged.
   - `edge_2: Edge`: The second edge to be merged.
  <br /><br /> Merges two compatible edges into one, provided the head of edge_1 is the same as the tail of edge_2, and edge_2 has exactly one incoming and one outgoing edge.
 - `get_multiple_edge_ids(self, *edge_ids : tuple[str])`
   - `*edge_ids : tuple[str]`: The edge IDs for which the operation will be performed.
@@ -378,23 +385,28 @@
 
 - `generate_bipartite_digraph(digraph_manager: DigraphManager)`
   - `digraph_manager: DigraphManager` - DigraphManager which is the base for bipartite digraph contruction.
  <br><br> enable bipartite digraph creation:
 
 <img width="1028" alt="image" src="https://github.com/Zeleczek-kodowniczek/Diblob/assets/72871011/1f3a686e-c1ef-4a41-8fa2-58a67a83fd12">
 
+- `generate_flow_digraph(digraph_manager: DigraphManager)`
+  - `digraph_manager: DigraphManager` - DigraphManager which is the base for flow digraph contruction.
+ <br><br> enable flow digraph creation (commonly used in control flow algorithm like the Ford-Fulkerson algorithm):
+
+<img width="944" alt="image" src="https://github.com/JakubZelek/Diblob/assets/72871011/9739207a-73d9-4ca4-98c8-e41116a17509">
 
-## Aghoritms
+## Algorithms
 In order to working with diblob explanation, DFS, DFSA and Dijkstra algorithms are created. 
 
 - DFS - Deep first search alghoritm.
 - DFSA - modification of the DFS (with the nodes visit time)
 - DijkstraAlgorithm - the shortes paths between node and the others.
 
-Alghoritms use duck typing. GraphManager instance have to be delivered during creation. Then `run` methon can be used on selected node_id (in DijkstraAlgorithm `cost_function` as a dict can be also delivered)
+Algorithm use duck typing. GraphManager instance have to be delivered during creation. Then `run` methon can be used on selected node_id (in DijkstraAlgorithm `cost_function` as a dict can be also delivered)
 
 Example of run:
 
  <br><br>
 ```python
 from diblob import DigraphManager
 from diblob.algorithms import DFS, DFSA, DijkstraAlgorithm
```

### Comparing `diblob-1.0.6/setup.py` & `diblob-1.0.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='diblob',
-    version='1.0.6',
+    version='1.0.7',
     package_dir={'': 'src'},
     packages=find_packages(where='src'),
     description='A simple example package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Jakub Zelek',
     author_email='jakub.zelek@doctoral.uj.edu.pl',
-    url='https://github.com/Zeleczek-kodowniczek/Diblob/tree/main',
+    url='https://github.com/JakubZelek/Diblob',
     license='MIT',
     install_requires=[],
     classifiers=[
         'Programming Language :: Python :: 3.10',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
```

### Comparing `diblob-1.0.6/src/diblob/algorithms.py` & `diblob-1.0.7/src/diblob/algorithms.py`

 * *Files identical despite different names*

### Comparing `diblob-1.0.6/src/diblob/components.py` & `diblob-1.0.7/src/diblob/components.py`

 * *Files identical despite different names*

### Comparing `diblob-1.0.6/src/diblob/digraph_manager.py` & `diblob-1.0.7/src/diblob/digraph_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,17 @@
                                DiblobKeyAlreadyExistsException,
                                InvalidDiblobId,
                                RootDiblobException,
                                DiblobGatherException,
                                EdgeAdditionException,
                                InvalidDigraphDictException,
                                InvalidConstructionJSON,
-                               CommonResourcesInjection)
+                               CommonResourcesInjection,
+                               IllegalJoinException)
+
 
 
 class DigraphManager:
     """
     DigraphManager operates on Node, Edge and Diblob class. 
     All operations on the digraph are managed indirectly by manager.
 
@@ -181,15 +183,14 @@
                         edges_to_connect.append((key, head))
             else:
                 raise InvalidConstructionJSON('Invalid json delivered!')
 
             gather_dict[diblob_id].append(key)
 
 
-
     def get_diblobs_common_ancestor(self, diblob_id1: str, diblob_id2: str):
         """
         Returns common ancestor diblob_id for diblob_id1 and diblob_id2.
         """
 
         ancestors_of_diblob_id1 = []
         ancestors_of_diblob_id2 = []
@@ -392,15 +393,14 @@
         self.diblobs[diblob.parent_id].children.remove(diblob_id)
         self[diblob_id] = Node(diblob_id, diblob.parent_id, [], [])
 
         self.connect_nodes(*incoming_edges)
         self.connect_nodes(*outgoing_edges)
 
 
-
     def merge_edges(self, edge_1: Edge, edge_2: Edge):
         """
         Merges two edges.
         """
 
         if edge_1.path != edge_2.path:
             if edge_1.path[-1] != edge_2.path[0]:
@@ -458,15 +458,15 @@
         Adds edges in existing graph structure.
         """
 
         for edge_id in edge_ids:
             tail, head = edge_id[0], edge_id[1]
             self[tail].outgoing_nodes.append(head)
             self[head].incoming_nodes.append(tail)
-            self[(tail,head)] = Edge(path=[tail, head])
+            self[(tail,head)] = Edge(path=[tail, head])        
 
 
     def remove_nodes(self, *nodes: tuple[Node, ...]):
         """
         Removes nodes from the graph.
         """
 
@@ -528,15 +528,14 @@
                 if len(edge.path) > 2:
                     node_ids = edge.path
                     self.remove_edges(edge)
                     self.add_nodes(*node_ids[1:-1])
                     self.connect_nodes(*list(zip(node_ids[:-1], node_ids[1:])))
 
 
-
     def inject(self, digraph_manager: "DigraphManager", node_id: str):
         """
         Replace node by diblob.
         """
         namespace = (set(digraph_manager.diblobs) & set(self.diblobs)) |\
                     (set(digraph_manager.nodes) & set(self.nodes))
         if namespace:
@@ -561,14 +560,31 @@
                                for incoming_node_id in node.incoming_nodes])
             self.connect_nodes(*[(injected_node_id, outgoing_node_id)
                                for outgoing_node_id in node.outgoing_nodes])
 
         self.remove_nodes(node)
 
 
+    def join_diblobs(self, diblob_fst_id: str, diblob_snd_id: str, join_id: str):
+        """
+        Join two diblobs to diblob with join_id.
+        """
+
+        fst_diblob = self[diblob_fst_id]
+        snd_diblob = self[diblob_snd_id]
+
+        if fst_diblob.parent_id != snd_diblob.parent_id:
+            raise IllegalJoinException(f"Diblobs during joining must have the same parent_id:\
+                                       {fst_diblob.parent_id} != {snd_diblob.parent_id}")
+
+        join_node_ids = self[diblob_fst_id].nodes | self[diblob_snd_id].nodes
+        self.flatten(diblob_fst_id, diblob_snd_id)
+        self.gather(join_id, join_node_ids)
+
+
     def decouple_edges(self):
         """
         In pseudoghraph transforms multiple edges into different ones with point in the middle.
         """
 
         edge_dict = dict(self.edges)
```

### Comparing `diblob-1.0.6/src/diblob/exceptions.py` & `diblob-1.0.7/src/diblob/exceptions.py`

 * *Files 26% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 class RemoveRootDiblobException(Exception):
     """
     Raised when we try flat root diblob.
     """
 
 class RootDiblobException(Exception):
     """
-    Raised when operation is forbidden for root diblob.
+    Raised when operation is forbidden for root diblob, or operations are 
+    available just for diblobs with only one root (root_diblob)
     """
 
 class EdgeAdditionException(Exception):
     """
     Raised when we try add incompatible edges.
     """
 
@@ -61,7 +62,37 @@
     Raised when algorithm try perform operation reserved only for digraphs (not pseudographs).
     """
 
 class CommonResourcesInjection(Exception):
     """
     Raised when we use inject method with the same ids for both of digraphs.
     """
+
+class IllegalJoinException(Exception):
+    """
+    Raised when we try join blobs with different parent_ids.
+    """
+
+class InvalidAdditionException(Exception):
+    """
+    Raised when we try add two digraphs with more than one diblob (with root_id).
+    """
+
+class RandomCycleException(Exception):
+    """
+    Raised when we try create cycle with node space < size of cycle in the generator.
+    """
+
+class RandomDAGException(Exception):
+    """
+    Raised when we try create random DAG with too many edges.
+    """
+
+class InvalidGeneratorParameterException(Exception):
+    """
+    Raised when we try create random digraph using impossible parameters.
+    """
+
+class RenamingException(Exception):
+    """
+    Raised when an component id try to be changed into occupied id.
+    """
```

### Comparing `diblob-1.0.6/src/diblob/factory.py` & `diblob-1.0.7/src/diblob/factory.py`

 * *Files 15% similar despite different names*

```diff
@@ -89,7 +89,40 @@
         bipartite_digraph_dict = {digraph_manager.root_diblob_id: {node_id + '`': [] for node_id\
                                 in digraph_manager.nodes} | {node_id + '``': []
                                                            for node_id in digraph_manager.nodes}}
         for node in digraph_manager.nodes.values():
             bipartite_digraph_dict[digraph_manager.root_diblob_id][node.node_id + '`'] =\
                                 [node_id + '``' for node_id in sorted(node.outgoing_nodes)]
         return DigraphManager(bipartite_digraph_dict)
+
+
+    @staticmethod
+    def generate_flow_digraph(digraph_manager: DigraphManager):
+        """
+        Generates digraph with splitted nodes. Splitted node is divided 
+        to two connected nodes, where the first one and the second one inherit 
+        incoming_nodes and outgoing_nodes respectively.
+        """
+
+        root_diblob_id = digraph_manager.root_diblob_id
+        flow_graph_manager = DigraphManager({root_diblob_id: {}})
+
+        node_ids = {node_id + '`' for node_id in digraph_manager.nodes} |\
+                   {node_id + '``' for node_id in digraph_manager.nodes}
+        flow_graph_manager.add_nodes(*node_ids)
+
+        edges_to_connect = set()
+
+        for node_id, node in digraph_manager.nodes.items():
+
+            node_split_tail = node_id + '`'
+            node_split_head = node_id + '``'
+
+            edges_to_connect |= {(incoming_node + '``', node_split_tail)
+                                 for incoming_node in node.incoming_nodes}
+            edges_to_connect |= {(node_split_head, outgoing_node + '`')
+                                 for outgoing_node in node.outgoing_nodes}
+
+            edges_to_connect.add((node_split_tail, node_split_head))
+
+        flow_graph_manager.connect_nodes(*edges_to_connect)
+        return flow_graph_manager
```

### Comparing `diblob-1.0.6/src/diblob/tools.py` & `diblob-1.0.7/src/diblob/tools.py`

 * *Files identical despite different names*

### Comparing `diblob-1.0.6/src/diblob.egg-info/PKG-INFO` & `diblob-1.0.7/src/diblob.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: diblob
-Version: 1.0.6
+Version: 1.0.7
 Summary: A simple example package
-Home-page: https://github.com/Zeleczek-kodowniczek/Diblob/tree/main
+Home-page: https://github.com/JakubZelek/Diblob
 Author: Jakub Zelek
 Author-email: jakub.zelek@doctoral.uj.edu.pl
 License: MIT
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -261,14 +261,21 @@
 
 - `compress_diblob(self, diblob_id: str)`
   - `diblob_id: str`: The ID of the Diblob that is to be compressed.
  <br /><br /> This method compresses the specified Diblob into a single node, effectively consolidating its structure for simplified representation:
 
 <img width="939" alt="image" src="https://github.com/Zeleczek-kodowniczek/Diblob/assets/72871011/589d935f-0dab-49c7-aec3-22be0be92404">
 
+- `join_diblobs(self, diblob_fst_id: str, diblob_snd_id: str, join_id: str)`
+  - `diblob_fst_id: str`: The ID of the first Diblob that is to be joined.
+  - `diblob_snd_id: str`: The ID of the second Diblob that is to be compressed.
+  - `join_id: str`: The ID of the joined Diblob.
+ <br /><br /> This method join two diblobs which have the same `parent_id`:
+
+<img width="1028" alt="image" src="https://github.com/JakubZelek/Diblob/assets/72871011/a74ecf81-bee4-4e81-b598-e890fa14ec21">
 
 - `merge_edges(self, edge_1: Edge, edge_2: Edge)`
   - `edge_1: Edge`: The first edge to be merged.
   - `edge_2: Edge`: The second edge to be merged.
  <br /><br /> Merges two compatible edges into one, provided the head of edge_1 is the same as the tail of edge_2, and edge_2 has exactly one incoming and one outgoing edge.
 - `get_multiple_edge_ids(self, *edge_ids : tuple[str])`
   - `*edge_ids : tuple[str]`: The edge IDs for which the operation will be performed.
@@ -392,23 +399,28 @@
 
 - `generate_bipartite_digraph(digraph_manager: DigraphManager)`
   - `digraph_manager: DigraphManager` - DigraphManager which is the base for bipartite digraph contruction.
  <br><br> enable bipartite digraph creation:
 
 <img width="1028" alt="image" src="https://github.com/Zeleczek-kodowniczek/Diblob/assets/72871011/1f3a686e-c1ef-4a41-8fa2-58a67a83fd12">
 
+- `generate_flow_digraph(digraph_manager: DigraphManager)`
+  - `digraph_manager: DigraphManager` - DigraphManager which is the base for flow digraph contruction.
+ <br><br> enable flow digraph creation (commonly used in control flow algorithm like the Ford-Fulkerson algorithm):
+
+<img width="944" alt="image" src="https://github.com/JakubZelek/Diblob/assets/72871011/9739207a-73d9-4ca4-98c8-e41116a17509">
 
-## Aghoritms
+## Algorithms
 In order to working with diblob explanation, DFS, DFSA and Dijkstra algorithms are created. 
 
 - DFS - Deep first search alghoritm.
 - DFSA - modification of the DFS (with the nodes visit time)
 - DijkstraAlgorithm - the shortes paths between node and the others.
 
-Alghoritms use duck typing. GraphManager instance have to be delivered during creation. Then `run` methon can be used on selected node_id (in DijkstraAlgorithm `cost_function` as a dict can be also delivered)
+Algorithm use duck typing. GraphManager instance have to be delivered during creation. Then `run` methon can be used on selected node_id (in DijkstraAlgorithm `cost_function` as a dict can be also delivered)
 
 Example of run:
 
  <br><br>
 ```python
 from diblob import DigraphManager
 from diblob.algorithms import DFS, DFSA, DijkstraAlgorithm
```

### Comparing `diblob-1.0.6/tests/test_components.py` & `diblob-1.0.7/tests/test_components.py`

 * *Files identical despite different names*

### Comparing `diblob-1.0.6/tests/test_digraph_manager.py` & `diblob-1.0.7/tests/test_digraph_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 """
 
 import os
 import json
 import pytest
 from diblob.digraph_manager import DigraphManager
 from diblob.exceptions import (InvalidDigraphDictException,
-                            RemoveRootDiblobException,
-                            CommonResourcesInjection)
+                               RemoveRootDiblobException,
+                               CommonResourcesInjection,
+                               IllegalJoinException)
 
 DIGRAPHS_PATH = 'tests/digraphs'
 
 @pytest.fixture()
 def digraph_dict():
     """
     Reads digraphs json representations from test/graphs dictionary.
@@ -278,7 +279,30 @@
                                             'B0`': {'C`': ['A`', 'B`', {'B0': ['F']}], 
                                                     'B`': ['C`', {'B0': ['F']}],
                                                     'A`': ['B`', 'C`', {'B0': ['F']}]}, 
                                             'B': ['C'], 
                                             'A': ['B'], 
                                             'D': [{'B0`': ['A`', 'B`', 'C`']}], 
                                             'G': ['A']}}
+
+
+def test_digraph_joining(digraph_dict):
+    """
+    test joining diblobs.
+    """
+    digraph_manager = DigraphManager(digraph_dict["g11_graph_with_diblobs"])
+    with pytest.raises(IllegalJoinException):
+        digraph_manager.join_diblobs(diblob_fst_id='B3', diblob_snd_id='B2', join_id='BJoin')
+
+    digraph_manager.join_diblobs(diblob_fst_id='B1', diblob_snd_id='B2', join_id='BJoin')
+    digraph_manager.sorted()
+
+    assert digraph_manager('B0') == {'B0': {'I': ['A', 'H', {'BJoin': ['C', 'G']}], 
+                                            'H': ['A', {'BJoin': ['B']}], 
+                                            'B3': {'BJoin': {'C': ['D'], 
+                                                             'D': [], 
+                                                             'B': ['D', {'B0': ['A']}], 
+                                                             'G': ['C', 'D', 'E', 'F'], 
+                                                             'E': ['B', 'D', {'B0': ['A']}], 
+                                                             'F': ['C', 'D', {'B0': ['H']}]}, 
+                                                    'J': [{'BJoin': ['D']}]}, 
+                                                    'A': [{'BJoin': ['B', 'C', 'D']}]}}
```

### Comparing `diblob-1.0.6/tests/test_exploratory_unit_tests.py` & `diblob-1.0.7/tests/test_exploratory_unit_tests.py`

 * *Files identical despite different names*

### Comparing `diblob-1.0.6/tests/test_factory.py` & `diblob-1.0.7/tests/test_factory.py`

 * *Files 17% similar despite different names*

```diff
@@ -159,7 +159,46 @@
                                             'G`': ['A``', 'D``'], 
                                             'D``': [], 
                                             'E``': [], 
                                             'B``': [], 
                                             'E`': ['A``', 'F``'], 
                                             'A``': [], 
                                             'A`': ['B``', 'F``']}}
+
+def test_flow_digraph():
+    """
+    test for flow digraph creation.
+    """
+    digraph_manager = DigraphManager({"B0": {"A": ["D"],
+                                             "B": ["D"],
+                                             "C": ["D"],
+                                             "D": ["E", "F"],
+                                             "E": ["G", "H"],
+                                             "F": ["H", "I"],
+                                             "G": ["J"],
+                                             "H": ["J"],
+                                             "I": ["J"],
+                                             "J": []}})
+
+    flow_digraph_manager = DiblobFactory.generate_flow_digraph(digraph_manager)
+    flow_digraph_manager.sorted()
+
+    assert flow_digraph_manager('B0') == {'B0': {'B``': ['D`'],
+                                                 'A``': ['D`'], 
+                                                 'C`': ['C``'], 
+                                                 'G`': ['G``'], 
+                                                 'I`': ['I``'], 
+                                                 'C``': ['D`'], 
+                                                 'F``': ['H`', 'I`'], 
+                                                 'F`': ['F``'], 
+                                                 'J`': ['J``'], 
+                                                 'H``': ['J`'], 
+                                                 'D``': ['E`', 'F`'], 
+                                                 'E``': ['G`', 'H`'], 
+                                                 'A`': ['A``'], 
+                                                 'D`': ['D``'], 
+                                                 'G``': ['J`'], 
+                                                 'I``': ['J`'], 
+                                                 'H`': ['H``'], 
+                                                 'B`': ['B``'], 
+                                                 'J``': [], 
+                                                 'E`': ['E``']}}
```

