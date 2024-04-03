# Comparing `tmp/Python-Algorithm-pyal-1.1.9.tar.gz` & `tmp/Python-Algorithm-pyal-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Python-Algorithm-pyal-1.1.9.tar", last modified: Wed Apr  3 01:17:42 2024, max compression
+gzip compressed data, was "Python-Algorithm-pyal-1.2.0.tar", last modified: Wed Apr  3 19:44:13 2024, max compression
```

## Comparing `Python-Algorithm-pyal-1.1.9.tar` & `Python-Algorithm-pyal-1.2.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 01:17:42.206059 Python-Algorithm-pyal-1.1.9/
--rw-r--r--   0 summer     (502) staff       (20)     3624 2024-04-03 01:17:42.205887 Python-Algorithm-pyal-1.1.9/PKG-INFO
--rw-r--r--   0 summer     (502) staff       (20)     3055 2023-12-16 02:37:57.000000 Python-Algorithm-pyal-1.1.9/README.md
--rw-r--r--   0 summer     (502) staff       (20)       94 2023-11-02 20:23:19.000000 Python-Algorithm-pyal-1.1.9/pyproject.toml
--rw-r--r--   0 summer     (502) staff       (20)      732 2024-04-03 01:17:42.206774 Python-Algorithm-pyal-1.1.9/setup.cfg
-drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 01:17:42.170579 Python-Algorithm-pyal-1.1.9/src/
-drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 01:17:42.205289 Python-Algorithm-pyal-1.1.9/src/Python_Algorithm_pyal.egg-info/
--rw-r--r--   0 summer     (502) staff       (20)     3624 2024-04-03 01:17:42.000000 Python-Algorithm-pyal-1.1.9/src/Python_Algorithm_pyal.egg-info/PKG-INFO
--rw-r--r--   0 summer     (502) staff       (20)     1236 2024-04-03 01:17:42.000000 Python-Algorithm-pyal-1.1.9/src/Python_Algorithm_pyal.egg-info/SOURCES.txt
--rw-r--r--   0 summer     (502) staff       (20)        1 2024-04-03 01:17:42.000000 Python-Algorithm-pyal-1.1.9/src/Python_Algorithm_pyal.egg-info/dependency_links.txt
--rw-r--r--   0 summer     (502) staff       (20)        5 2024-04-03 01:17:42.000000 Python-Algorithm-pyal-1.1.9/src/Python_Algorithm_pyal.egg-info/top_level.txt
-drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 01:17:42.176103 Python-Algorithm-pyal-1.1.9/src/pyal/
--rw-r--r--   0 summer     (502) staff       (20)      593 2024-04-03 01:16:58.000000 Python-Algorithm-pyal-1.1.9/src/pyal/__init__.py
-drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 01:17:42.179493 Python-Algorithm-pyal-1.1.9/src/pyal/common/
--rw-r--r--   0 summer     (502) staff       (20)        0 2023-11-03 00:24:21.000000 Python-Algorithm-pyal-1.1.9/src/pyal/common/__init__.py
--rw-r--r--   0 summer     (502) staff       (20)     9310 2024-03-25 21:11:02.000000 Python-Algorithm-pyal-1.1.9/src/pyal/common/algorithm.py
--rw-r--r--   0 summer     (502) staff       (20)     3518 2023-12-20 06:27:08.000000 Python-Algorithm-pyal-1.1.9/src/pyal/common/algorithm_TEST.py
-drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 01:17:42.185644 Python-Algorithm-pyal-1.1.9/src/pyal/graph/
--rw-r--r--   0 summer     (502) staff       (20)        0 2023-11-03 00:24:25.000000 Python-Algorithm-pyal-1.1.9/src/pyal/graph/__init__.py
--rw-r--r--   0 summer     (502) staff       (20)     1842 2023-11-20 21:03:57.000000 Python-Algorithm-pyal-1.1.9/src/pyal/graph/graph.py
--rw-r--r--   0 summer     (502) staff       (20)      576 2023-11-20 21:03:57.000000 Python-Algorithm-pyal-1.1.9/src/pyal/graph/graph_TEST.py
--rw-r--r--   0 summer     (502) staff       (20)        7 2023-12-16 01:35:27.000000 Python-Algorithm-pyal-1.1.9/src/pyal/graph/minimum_span_tree.py
--rw-r--r--   0 summer     (502) staff       (20)     1387 2023-11-20 21:03:57.000000 Python-Algorithm-pyal-1.1.9/src/pyal/graph/shortest_path.py
--rw-r--r--   0 summer     (502) staff       (20)      780 2023-11-20 21:03:58.000000 Python-Algorithm-pyal-1.1.9/src/pyal/graph/shortest_path_TEST.py
--rw-r--r--   0 summer     (502) staff       (20)      595 2023-11-20 21:03:58.000000 Python-Algorithm-pyal-1.1.9/src/pyal/graph/topological_traversal.py
--rw-r--r--   0 summer     (502) staff       (20)      401 2023-11-20 21:03:57.000000 Python-Algorithm-pyal-1.1.9/src/pyal/graph/topological_traversal_TEST.py
-drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 01:17:42.196910 Python-Algorithm-pyal-1.1.9/src/pyal/list/
--rw-r--r--   0 summer     (502) staff       (20)        0 2023-11-03 00:24:28.000000 Python-Algorithm-pyal-1.1.9/src/pyal/list/__init__.py
--rw-r--r--   0 summer     (502) staff       (20)      130 2023-12-16 01:45:31.000000 Python-Algorithm-pyal-1.1.9/src/pyal/list/dequeue.py
--rw-r--r--   0 summer     (502) staff       (20)      310 2023-12-16 01:48:08.000000 Python-Algorithm-pyal-1.1.9/src/pyal/list/dequeue_TEST.py
--rw-r--r--   0 summer     (502) staff       (20)     2340 2023-11-23 05:16:03.000000 Python-Algorithm-pyal-1.1.9/src/pyal/list/lfu_cache.py
--rw-r--r--   0 summer     (502) staff       (20)     4035 2023-12-19 22:17:29.000000 Python-Algorithm-pyal-1.1.9/src/pyal/list/linked_list.py
--rw-r--r--   0 summer     (502) staff       (20)     1772 2023-12-19 22:16:39.000000 Python-Algorithm-pyal-1.1.9/src/pyal/list/linked_list_TEST.py
--rw-r--r--   0 summer     (502) staff       (20)     1101 2023-11-23 05:16:03.000000 Python-Algorithm-pyal-1.1.9/src/pyal/list/lru_cache.py
--rw-r--r--   0 summer     (502) staff       (20)      455 2023-12-16 01:38:35.000000 Python-Algorithm-pyal-1.1.9/src/pyal/list/queue.py
--rw-r--r--   0 summer     (502) staff       (20)      259 2023-12-16 01:42:13.000000 Python-Algorithm-pyal-1.1.9/src/pyal/list/queue_TEST.py
--rw-r--r--   0 summer     (502) staff       (20)      484 2023-12-16 01:22:02.000000 Python-Algorithm-pyal-1.1.9/src/pyal/list/stack.py
--rw-r--r--   0 summer     (502) staff       (20)      318 2023-12-16 01:42:13.000000 Python-Algorithm-pyal-1.1.9/src/pyal/list/stack_TEST.py
-drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 01:17:42.198664 Python-Algorithm-pyal-1.1.9/src/pyal/string/
--rw-r--r--   0 summer     (502) staff       (20)        0 2023-11-03 00:24:32.000000 Python-Algorithm-pyal-1.1.9/src/pyal/string/__init__.py
--rw-r--r--   0 summer     (502) staff       (20)      743 2023-11-20 21:04:00.000000 Python-Algorithm-pyal-1.1.9/src/pyal/string/search.py
--rw-r--r--   0 summer     (502) staff       (20)      337 2023-11-20 21:04:00.000000 Python-Algorithm-pyal-1.1.9/src/pyal/string/search_TEST.py
-drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 01:17:42.204436 Python-Algorithm-pyal-1.1.9/src/pyal/tree/
--rw-r--r--   0 summer     (502) staff       (20)        0 2023-11-03 00:24:36.000000 Python-Algorithm-pyal-1.1.9/src/pyal/tree/__init__.py
--rw-r--r--   0 summer     (502) staff       (20)      685 2023-12-25 08:28:48.000000 Python-Algorithm-pyal-1.1.9/src/pyal/tree/disjoint_set.py
--rw-r--r--   0 summer     (502) staff       (20)      311 2023-12-25 05:29:03.000000 Python-Algorithm-pyal-1.1.9/src/pyal/tree/disjoint_set_TEST.py
--rw-r--r--   0 summer     (502) staff       (20)     3558 2023-12-16 01:22:02.000000 Python-Algorithm-pyal-1.1.9/src/pyal/tree/dynamic_heap.py
--rw-r--r--   0 summer     (502) staff       (20)      704 2023-11-20 21:03:56.000000 Python-Algorithm-pyal-1.1.9/src/pyal/tree/dynamic_heap_TEST.py
--rw-r--r--   0 summer     (502) staff       (20)      448 2023-12-16 01:22:02.000000 Python-Algorithm-pyal-1.1.9/src/pyal/tree/min_heap.py
--rw-r--r--   0 summer     (502) staff       (20)     7465 2024-04-03 01:16:13.000000 Python-Algorithm-pyal-1.1.9/src/pyal/tree/tree_map.py
--rw-r--r--   0 summer     (502) staff       (20)     2209 2023-12-16 01:22:36.000000 Python-Algorithm-pyal-1.1.9/src/pyal/tree/tree_map_TEST.py
+drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 19:44:13.130190 Python-Algorithm-pyal-1.2.0/
+-rw-r--r--   0 summer     (502) staff       (20)     3624 2024-04-03 19:44:13.129993 Python-Algorithm-pyal-1.2.0/PKG-INFO
+-rw-r--r--   0 summer     (502) staff       (20)     3055 2023-12-16 02:37:57.000000 Python-Algorithm-pyal-1.2.0/README.md
+-rw-r--r--   0 summer     (502) staff       (20)       94 2023-11-02 20:23:19.000000 Python-Algorithm-pyal-1.2.0/pyproject.toml
+-rw-r--r--   0 summer     (502) staff       (20)      732 2024-04-03 19:44:13.130994 Python-Algorithm-pyal-1.2.0/setup.cfg
+drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 19:44:13.102186 Python-Algorithm-pyal-1.2.0/src/
+drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 19:44:13.129182 Python-Algorithm-pyal-1.2.0/src/Python_Algorithm_pyal.egg-info/
+-rw-r--r--   0 summer     (502) staff       (20)     3624 2024-04-03 19:44:13.000000 Python-Algorithm-pyal-1.2.0/src/Python_Algorithm_pyal.egg-info/PKG-INFO
+-rw-r--r--   0 summer     (502) staff       (20)     1236 2024-04-03 19:44:13.000000 Python-Algorithm-pyal-1.2.0/src/Python_Algorithm_pyal.egg-info/SOURCES.txt
+-rw-r--r--   0 summer     (502) staff       (20)        1 2024-04-03 19:44:13.000000 Python-Algorithm-pyal-1.2.0/src/Python_Algorithm_pyal.egg-info/dependency_links.txt
+-rw-r--r--   0 summer     (502) staff       (20)        5 2024-04-03 19:44:13.000000 Python-Algorithm-pyal-1.2.0/src/Python_Algorithm_pyal.egg-info/top_level.txt
+drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 19:44:13.106181 Python-Algorithm-pyal-1.2.0/src/pyal/
+-rw-r--r--   0 summer     (502) staff       (20)      593 2024-04-03 19:43:40.000000 Python-Algorithm-pyal-1.2.0/src/pyal/__init__.py
+drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 19:44:13.108081 Python-Algorithm-pyal-1.2.0/src/pyal/common/
+-rw-r--r--   0 summer     (502) staff       (20)        0 2023-11-03 00:24:21.000000 Python-Algorithm-pyal-1.2.0/src/pyal/common/__init__.py
+-rw-r--r--   0 summer     (502) staff       (20)     9310 2024-03-25 21:11:02.000000 Python-Algorithm-pyal-1.2.0/src/pyal/common/algorithm.py
+-rw-r--r--   0 summer     (502) staff       (20)     3518 2023-12-20 06:27:08.000000 Python-Algorithm-pyal-1.2.0/src/pyal/common/algorithm_TEST.py
+drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 19:44:13.113408 Python-Algorithm-pyal-1.2.0/src/pyal/graph/
+-rw-r--r--   0 summer     (502) staff       (20)        0 2023-11-03 00:24:25.000000 Python-Algorithm-pyal-1.2.0/src/pyal/graph/__init__.py
+-rw-r--r--   0 summer     (502) staff       (20)     1842 2023-11-20 21:03:57.000000 Python-Algorithm-pyal-1.2.0/src/pyal/graph/graph.py
+-rw-r--r--   0 summer     (502) staff       (20)      576 2023-11-20 21:03:57.000000 Python-Algorithm-pyal-1.2.0/src/pyal/graph/graph_TEST.py
+-rw-r--r--   0 summer     (502) staff       (20)        7 2023-12-16 01:35:27.000000 Python-Algorithm-pyal-1.2.0/src/pyal/graph/minimum_span_tree.py
+-rw-r--r--   0 summer     (502) staff       (20)     1387 2023-11-20 21:03:57.000000 Python-Algorithm-pyal-1.2.0/src/pyal/graph/shortest_path.py
+-rw-r--r--   0 summer     (502) staff       (20)      780 2023-11-20 21:03:58.000000 Python-Algorithm-pyal-1.2.0/src/pyal/graph/shortest_path_TEST.py
+-rw-r--r--   0 summer     (502) staff       (20)      595 2023-11-20 21:03:58.000000 Python-Algorithm-pyal-1.2.0/src/pyal/graph/topological_traversal.py
+-rw-r--r--   0 summer     (502) staff       (20)      401 2023-11-20 21:03:57.000000 Python-Algorithm-pyal-1.2.0/src/pyal/graph/topological_traversal_TEST.py
+drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 19:44:13.120067 Python-Algorithm-pyal-1.2.0/src/pyal/list/
+-rw-r--r--   0 summer     (502) staff       (20)        0 2023-11-03 00:24:28.000000 Python-Algorithm-pyal-1.2.0/src/pyal/list/__init__.py
+-rw-r--r--   0 summer     (502) staff       (20)      130 2023-12-16 01:45:31.000000 Python-Algorithm-pyal-1.2.0/src/pyal/list/dequeue.py
+-rw-r--r--   0 summer     (502) staff       (20)      310 2023-12-16 01:48:08.000000 Python-Algorithm-pyal-1.2.0/src/pyal/list/dequeue_TEST.py
+-rw-r--r--   0 summer     (502) staff       (20)     2340 2023-11-23 05:16:03.000000 Python-Algorithm-pyal-1.2.0/src/pyal/list/lfu_cache.py
+-rw-r--r--   0 summer     (502) staff       (20)     4035 2023-12-19 22:17:29.000000 Python-Algorithm-pyal-1.2.0/src/pyal/list/linked_list.py
+-rw-r--r--   0 summer     (502) staff       (20)     1772 2023-12-19 22:16:39.000000 Python-Algorithm-pyal-1.2.0/src/pyal/list/linked_list_TEST.py
+-rw-r--r--   0 summer     (502) staff       (20)     1101 2023-11-23 05:16:03.000000 Python-Algorithm-pyal-1.2.0/src/pyal/list/lru_cache.py
+-rw-r--r--   0 summer     (502) staff       (20)      455 2023-12-16 01:38:35.000000 Python-Algorithm-pyal-1.2.0/src/pyal/list/queue.py
+-rw-r--r--   0 summer     (502) staff       (20)      259 2023-12-16 01:42:13.000000 Python-Algorithm-pyal-1.2.0/src/pyal/list/queue_TEST.py
+-rw-r--r--   0 summer     (502) staff       (20)      484 2023-12-16 01:22:02.000000 Python-Algorithm-pyal-1.2.0/src/pyal/list/stack.py
+-rw-r--r--   0 summer     (502) staff       (20)      318 2023-12-16 01:42:13.000000 Python-Algorithm-pyal-1.2.0/src/pyal/list/stack_TEST.py
+drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 19:44:13.121646 Python-Algorithm-pyal-1.2.0/src/pyal/string/
+-rw-r--r--   0 summer     (502) staff       (20)        0 2023-11-03 00:24:32.000000 Python-Algorithm-pyal-1.2.0/src/pyal/string/__init__.py
+-rw-r--r--   0 summer     (502) staff       (20)      743 2023-11-20 21:04:00.000000 Python-Algorithm-pyal-1.2.0/src/pyal/string/search.py
+-rw-r--r--   0 summer     (502) staff       (20)      337 2023-11-20 21:04:00.000000 Python-Algorithm-pyal-1.2.0/src/pyal/string/search_TEST.py
+drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 19:44:13.128213 Python-Algorithm-pyal-1.2.0/src/pyal/tree/
+-rw-r--r--   0 summer     (502) staff       (20)        0 2023-11-03 00:24:36.000000 Python-Algorithm-pyal-1.2.0/src/pyal/tree/__init__.py
+-rw-r--r--   0 summer     (502) staff       (20)      685 2023-12-25 08:28:48.000000 Python-Algorithm-pyal-1.2.0/src/pyal/tree/disjoint_set.py
+-rw-r--r--   0 summer     (502) staff       (20)      311 2023-12-25 05:29:03.000000 Python-Algorithm-pyal-1.2.0/src/pyal/tree/disjoint_set_TEST.py
+-rw-r--r--   0 summer     (502) staff       (20)     3558 2023-12-16 01:22:02.000000 Python-Algorithm-pyal-1.2.0/src/pyal/tree/dynamic_heap.py
+-rw-r--r--   0 summer     (502) staff       (20)      704 2023-11-20 21:03:56.000000 Python-Algorithm-pyal-1.2.0/src/pyal/tree/dynamic_heap_TEST.py
+-rw-r--r--   0 summer     (502) staff       (20)      448 2023-12-16 01:22:02.000000 Python-Algorithm-pyal-1.2.0/src/pyal/tree/min_heap.py
+-rw-r--r--   0 summer     (502) staff       (20)     7179 2024-04-03 19:41:02.000000 Python-Algorithm-pyal-1.2.0/src/pyal/tree/tree_map.py
+-rw-r--r--   0 summer     (502) staff       (20)     2212 2024-04-03 17:11:32.000000 Python-Algorithm-pyal-1.2.0/src/pyal/tree/tree_map_TEST.py
```

### Comparing `Python-Algorithm-pyal-1.1.9/PKG-INFO` & `Python-Algorithm-pyal-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Python-Algorithm-pyal
-Version: 1.1.9
+Version: 1.2.0
 Summary: PYthon Algorithm Library (pyal) targets at providing a python version substitue of STL in C++, such as linked list, tree map, and other data structures and popular algorithms.
 Home-page: https://github.com/SummerRainET2008/PYthon_Algorithms_Library
 Author-email: tianxia0209@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `Python-Algorithm-pyal-1.1.9/README.md` & `Python-Algorithm-pyal-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.1.9/setup.cfg` & `Python-Algorithm-pyal-1.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = Python-Algorithm-pyal
 authors = Summer Xia
 author_email = tianxia0209@gmail.com
-version = 1.1.9
+version = 1.2.0
 description = PYthon Algorithm Library (pyal) targets at providing a python version substitue of STL in C++, such as linked list, tree map, and other data structures and popular algorithms.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/SummerRainET2008/PYthon_Algorithms_Library
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
```

### Comparing `Python-Algorithm-pyal-1.1.9/src/Python_Algorithm_pyal.egg-info/PKG-INFO` & `Python-Algorithm-pyal-1.2.0/src/Python_Algorithm_pyal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Python-Algorithm-pyal
-Version: 1.1.9
+Version: 1.2.0
 Summary: PYthon Algorithm Library (pyal) targets at providing a python version substitue of STL in C++, such as linked list, tree map, and other data structures and popular algorithms.
 Home-page: https://github.com/SummerRainET2008/PYthon_Algorithms_Library
 Author-email: tianxia0209@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `Python-Algorithm-pyal-1.1.9/src/Python_Algorithm_pyal.egg-info/SOURCES.txt` & `Python-Algorithm-pyal-1.2.0/src/Python_Algorithm_pyal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.1.9/src/pyal/__init__.py` & `Python-Algorithm-pyal-1.2.0/src/pyal/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 from .tree.min_heap import MinHeap
 from .tree.tree_map import TreeMap
 from .graph.shortest_path import Dijkstra
 from .graph.graph import Graph
 from .graph.topological_traversal import topological_traversal
 from .string.search import search_KMP
 
-__version__ = "1.1.9"
+__version__ = "1.2.0"
```

### Comparing `Python-Algorithm-pyal-1.1.9/src/pyal/common/algorithm.py` & `Python-Algorithm-pyal-1.2.0/src/pyal/common/algorithm.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.1.9/src/pyal/common/algorithm_TEST.py` & `Python-Algorithm-pyal-1.2.0/src/pyal/common/algorithm_TEST.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.1.9/src/pyal/graph/graph.py` & `Python-Algorithm-pyal-1.2.0/src/pyal/graph/graph.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.1.9/src/pyal/graph/graph_TEST.py` & `Python-Algorithm-pyal-1.2.0/src/pyal/graph/graph_TEST.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.1.9/src/pyal/graph/shortest_path.py` & `Python-Algorithm-pyal-1.2.0/src/pyal/graph/shortest_path.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.1.9/src/pyal/graph/shortest_path_TEST.py` & `Python-Algorithm-pyal-1.2.0/src/pyal/graph/shortest_path_TEST.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.1.9/src/pyal/graph/topological_traversal.py` & `Python-Algorithm-pyal-1.2.0/src/pyal/graph/topological_traversal.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.1.9/src/pyal/list/lfu_cache.py` & `Python-Algorithm-pyal-1.2.0/src/pyal/list/lfu_cache.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.1.9/src/pyal/list/linked_list.py` & `Python-Algorithm-pyal-1.2.0/src/pyal/list/linked_list.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.1.9/src/pyal/list/linked_list_TEST.py` & `Python-Algorithm-pyal-1.2.0/src/pyal/list/linked_list_TEST.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.1.9/src/pyal/list/lru_cache.py` & `Python-Algorithm-pyal-1.2.0/src/pyal/list/lru_cache.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.1.9/src/pyal/string/search.py` & `Python-Algorithm-pyal-1.2.0/src/pyal/string/search.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.1.9/src/pyal/tree/disjoint_set.py` & `Python-Algorithm-pyal-1.2.0/src/pyal/tree/disjoint_set.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.1.9/src/pyal/tree/dynamic_heap.py` & `Python-Algorithm-pyal-1.2.0/src/pyal/tree/dynamic_heap.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.1.9/src/pyal/tree/dynamic_heap_TEST.py` & `Python-Algorithm-pyal-1.2.0/src/pyal/tree/dynamic_heap_TEST.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.1.9/src/pyal/tree/tree_map.py` & `Python-Algorithm-pyal-1.2.0/src/pyal/tree/tree_map.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 class _AVLTreeNode:
   def __init__(self, key: int):
     self._key = key
     self._left = None
     self._right = None
     self._depth = 1
-    self._next_value = None
 
   def _print_tree(self):
     import nltk
     tree_expr = str(self)
     tree = nltk.Tree.fromstring(tree_expr)
     tree.pretty_print()
     print()
@@ -58,135 +57,129 @@
         return self if node is None else node
       return self
     else:
       if self._right is not None:
         return self._right._find_lower_bound(key)
       return None
 
-  def _insert(self, key, next_key: list, from_left: bool):
+  def _insert(self, key, next_key: list):
     assert key != self._key
 
     if key < self._key:
       next_key[0] = self._key
       if self._left is None:
         self._left = _AVLTreeNode(key)
       else:
-        self._left = self._left._insert(key, next_key, True)
+        self._left = self._left._insert(key, next_key)
 
     else:
       if self._right is None:
         self._right = _AVLTreeNode(key)
       else:
-        self._right = self._right._insert(key, next_key, False)
+        self._right = self._right._insert(key, next_key)
 
-    return _AVLTreeNode._reset_balance(self, from_left)
+    self._depth = 1 + max(self._get_depth(self._left),
+                          self._get_depth(self._right))
 
-  def _is_balanced(self, from_left: bool):
-    bf = self._get_balance_factor()
-    return bf == 0 or (from_left and bf == 1) or (not from_left and bf == -1)
-
-  def _get_balance_factor(self):
-    return self._get_depth(self._left) - self._get_depth(self._right)
-
-  @staticmethod
-  def _reset_node(node, from_left: bool):
-    node._reset_depth()
-    bf = node._get_balance_factor()
-
-    if bf in [-2, -3]:
-      return node._left_rotate()
-
-    elif bf == -1:
-      return node if not from_left else node._left_rotate()
-
-    elif bf == 0:
-      return node
-
-    elif bf == 1:
-      return node if from_left else node._right_rotate()
-
-    elif bf in [2, 3]:
-      return node._right_rotate()
+    bf = self._get_balance_factor(self)
+    if bf > 1:
+      if key > self._left._key:
+        self._left = self._left._left_rotate()
+      return self._right_rotate()
+
+    elif bf < -1:
+      if key < self._right._key:
+        self._right = self._right._right_rotate()
+      return self._left_rotate()
 
     else:
-      assert False
-
-  @staticmethod
-  def _reset_balance(node, from_left: bool):
-    if node is None:
-      return node
-
-    new_root = node
-    while True:
-      new_root = _AVLTreeNode._reset_node(new_root, from_left)
-      if new_root._is_balanced(from_left):
-        return new_root
+      return self
 
   def _right_rotate(self):
-    bf = self._get_balance_factor()
-    # assert bf >= 2
-
     left = self._left
-    self._left = _AVLTreeNode._reset_balance(left._right, True)
-    self._reset_depth()
+    left_right = left._right
 
-    left._right = _AVLTreeNode._reset_balance(self, False)
-    left._reset_depth()
+    # Perform rotation
+    left._right = self
+    self._left = left_right
+
+    # Update heights
+    self._depth = 1 + max(self._get_depth(self._left),
+                          self._get_depth(self._right))
+    left._depth = 1 + max(self._get_depth(left._left),
+                          self._get_depth(left._right))
 
     return left
 
   def _get_depth(self, node):
     return 0 if node is None else node._depth
 
   def _reset_depth(self):
     self._depth = max(self._get_depth(self._left), self._get_depth(
         self._right)) + 1
 
   def _left_rotate(self):
-    bf = self._get_balance_factor()
-    # assert bf <= -2
-
     right = self._right
-    self._right = _AVLTreeNode._reset_balance(right._left, False)
-    self._reset_depth()
+    right_left = right._left
 
-    right._left = _AVLTreeNode._reset_balance(self, True)
-    right._reset_depth()
+    # Perform rotation
+    right._left = self
+    self._right = right_left
+
+    # Update heights
+    self._depth = 1 + max(self._get_depth(self._left),
+                          self._get_depth(self._right))
+    right._depth = 1 + max(self._get_depth(right._left),
+                       self._get_depth(right._right))
 
     return right
 
-  def _remove(self, key, from_left: bool):
+  def _get_min_value_node(self):
+    if self._left is None:
+      return self
+    return self._left._get_min_value_node()
+
+  def _get_balance_factor(self, node):
+    if node is None:
+      return 0
+
+    return self._get_depth(node._left) - self._get_depth(node._right)
+
+  def _remove(self, key):
     # Key must be existent
     if key < self._key:
-      self._left = self._left._remove(key, True)
-      return self
+      self._left = self._left._remove(key)
     elif key > self._key:
-      self._right = self._right._remove(key, False)
-      return self
+      self._right = self._right._remove(key)
 
     else:
-      if self._right is None:
-        return _AVLTreeNode._reset_balance(self._left, from_left)
-      elif self._left is None:
-        return _AVLTreeNode._reset_balance(self._right, from_left)
+      if self._left is None:
+        return self._right
+      elif self._right is None:
+        return self._left
+
       else:
-        left_right_list = []
-        node = self._left
-        while node is not None:
-          left_right_list.append(node)
-          node = node._right
-
-        left_right_list[-1]._right = self._right._left
-        while left_right_list != []:
-          left_right_list[-1]._right = _AVLTreeNode._reset_balance(
-              left_right_list[-1]._right, False)
-          left_right_list.pop()
+        min_node = self._right._get_min_value_node()
+        self._key = min_node._key
+        self._right = self._right._remove(min_node._key)
+
+    self._reset_depth()
+    bf = self._get_balance_factor(self)
+
+    if bf > 1:
+      if self._get_balance_factor(self._left) < 0:
+        self._left = self._left._left_rotate()
+      return self._right_rotate()
+
+    elif bf < -1:
+      if self._get_balance_factor(self._right) > 0:
+        self._right = self._right._right_rotate()
+      return self._left_rotate()
 
-        self._right._left = self._left
-        return _AVLTreeNode._reset_balance(self._right, from_left)
+    return self
 
 
 class TreeMap:
   def __init__(self):
     from collections import namedtuple
 
     self._root = None
@@ -253,15 +246,15 @@
   def remove(self, key):
     info = self._key2info.get(key, None)
     if info is None:
       return
 
     self._key_list.remove(info.key_list_node)
     del self._key2info[key]
-    self._root = self._root._remove(key, True)
+    self._root = self._root._remove(key)
 
   def __getitem__(self, key):
     return self._key2info[key].value
 
   def __setitem__(self, key, value):
     rd = self._key2info.get(key, None)
     if rd is not None:
@@ -272,15 +265,15 @@
       self._root = _AVLTreeNode(key)
       self._key_list.push_back(key)
       self._key2info[key] = self._KeyInfo(
           value=value, key_list_node=self._key_list.rbegin())
 
     else:
       next_key = [None]
-      self._root = self._root._insert(key, next_key, True)
+      self._root = self._root._insert(key, next_key)
 
       if next_key[0] is None:
         next_node = self._key_list.end()
       else:
         next_node = self._key2info[next_key[0]].key_list_node
       self._key_list.insert_element(next_node, key)
```

### Comparing `Python-Algorithm-pyal-1.1.9/src/pyal/tree/tree_map_TEST.py` & `Python-Algorithm-pyal-1.2.0/src/pyal/tree/tree_map_TEST.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,16 +84,16 @@
   print(f"Removed 4")
   tree._print_tree()
   node = tree.lower_bound(4.1)
   assert node.get() == 6
 
 
 def test_many_remove():
-  for _ in range(10):
-    data = list(range(50))
+  for _ in range(100):
+    data = list(range(5000))
     data_random = data[::]
     random.shuffle(data_random)
     tree = TreeMap()
     for d in data_random:
       tree[d] = d
 
     for pos, d in enumerate(data):
```

