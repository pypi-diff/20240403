# Comparing `tmp/Python-Algorithm-pyal-1.1.8.tar.gz` & `tmp/Python-Algorithm-pyal-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Python-Algorithm-pyal-1.1.8.tar", last modified: Sun Dec 17 18:56:38 2023, max compression
+gzip compressed data, was "Python-Algorithm-pyal-1.1.9.tar", last modified: Wed Apr  3 01:17:42 2024, max compression
```

## Comparing `Python-Algorithm-pyal-1.1.8.tar` & `Python-Algorithm-pyal-1.1.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 summer     (502) staff       (20)        0 2023-12-17 18:56:38.772621 Python-Algorithm-pyal-1.1.8/
--rw-r--r--   0 summer     (502) staff       (20)     3624 2023-12-17 18:56:38.772399 Python-Algorithm-pyal-1.1.8/PKG-INFO
--rw-r--r--   0 summer     (502) staff       (20)     3055 2023-12-16 02:37:57.000000 Python-Algorithm-pyal-1.1.8/README.md
--rw-r--r--   0 summer     (502) staff       (20)       94 2023-11-02 20:23:19.000000 Python-Algorithm-pyal-1.1.8/pyproject.toml
--rw-r--r--   0 summer     (502) staff       (20)      732 2023-12-17 18:56:38.773699 Python-Algorithm-pyal-1.1.8/setup.cfg
-drwxr-xr-x   0 summer     (502) staff       (20)        0 2023-12-17 18:56:38.746873 Python-Algorithm-pyal-1.1.8/src/
-drwxr-xr-x   0 summer     (502) staff       (20)        0 2023-12-17 18:56:38.771357 Python-Algorithm-pyal-1.1.8/src/Python_Algorithm_pyal.egg-info/
--rw-r--r--   0 summer     (502) staff       (20)     3624 2023-12-17 18:56:38.000000 Python-Algorithm-pyal-1.1.8/src/Python_Algorithm_pyal.egg-info/PKG-INFO
--rw-r--r--   0 summer     (502) staff       (20)     1236 2023-12-17 18:56:38.000000 Python-Algorithm-pyal-1.1.8/src/Python_Algorithm_pyal.egg-info/SOURCES.txt
--rw-r--r--   0 summer     (502) staff       (20)        1 2023-12-17 18:56:38.000000 Python-Algorithm-pyal-1.1.8/src/Python_Algorithm_pyal.egg-info/dependency_links.txt
--rw-r--r--   0 summer     (502) staff       (20)        5 2023-12-17 18:56:38.000000 Python-Algorithm-pyal-1.1.8/src/Python_Algorithm_pyal.egg-info/top_level.txt
-drwxr-xr-x   0 summer     (502) staff       (20)        0 2023-12-17 18:56:38.751216 Python-Algorithm-pyal-1.1.8/src/pyal/
--rw-r--r--   0 summer     (502) staff       (20)      593 2023-12-17 18:56:07.000000 Python-Algorithm-pyal-1.1.8/src/pyal/__init__.py
-drwxr-xr-x   0 summer     (502) staff       (20)        0 2023-12-17 18:56:38.752447 Python-Algorithm-pyal-1.1.8/src/pyal/common/
--rw-r--r--   0 summer     (502) staff       (20)        0 2023-11-03 00:24:21.000000 Python-Algorithm-pyal-1.1.8/src/pyal/common/__init__.py
--rw-r--r--   0 summer     (502) staff       (20)     9153 2023-12-17 18:54:53.000000 Python-Algorithm-pyal-1.1.8/src/pyal/common/algorithm.py
--rw-r--r--   0 summer     (502) staff       (20)     3402 2023-12-17 18:55:22.000000 Python-Algorithm-pyal-1.1.8/src/pyal/common/algorithm_TEST.py
-drwxr-xr-x   0 summer     (502) staff       (20)        0 2023-12-17 18:56:38.756665 Python-Algorithm-pyal-1.1.8/src/pyal/graph/
--rw-r--r--   0 summer     (502) staff       (20)        0 2023-11-03 00:24:25.000000 Python-Algorithm-pyal-1.1.8/src/pyal/graph/__init__.py
--rw-r--r--   0 summer     (502) staff       (20)     1842 2023-11-20 21:03:57.000000 Python-Algorithm-pyal-1.1.8/src/pyal/graph/graph.py
--rw-r--r--   0 summer     (502) staff       (20)      576 2023-11-20 21:03:57.000000 Python-Algorithm-pyal-1.1.8/src/pyal/graph/graph_TEST.py
--rw-r--r--   0 summer     (502) staff       (20)        7 2023-12-16 01:35:27.000000 Python-Algorithm-pyal-1.1.8/src/pyal/graph/minimum_span_tree.py
--rw-r--r--   0 summer     (502) staff       (20)     1387 2023-11-20 21:03:57.000000 Python-Algorithm-pyal-1.1.8/src/pyal/graph/shortest_path.py
--rw-r--r--   0 summer     (502) staff       (20)      780 2023-11-20 21:03:58.000000 Python-Algorithm-pyal-1.1.8/src/pyal/graph/shortest_path_TEST.py
--rw-r--r--   0 summer     (502) staff       (20)      595 2023-11-20 21:03:58.000000 Python-Algorithm-pyal-1.1.8/src/pyal/graph/topological_traversal.py
--rw-r--r--   0 summer     (502) staff       (20)      401 2023-11-20 21:03:57.000000 Python-Algorithm-pyal-1.1.8/src/pyal/graph/topological_traversal_TEST.py
-drwxr-xr-x   0 summer     (502) staff       (20)        0 2023-12-17 18:56:38.763899 Python-Algorithm-pyal-1.1.8/src/pyal/list/
--rw-r--r--   0 summer     (502) staff       (20)        0 2023-11-03 00:24:28.000000 Python-Algorithm-pyal-1.1.8/src/pyal/list/__init__.py
--rw-r--r--   0 summer     (502) staff       (20)      130 2023-12-16 01:45:31.000000 Python-Algorithm-pyal-1.1.8/src/pyal/list/dequeue.py
--rw-r--r--   0 summer     (502) staff       (20)      310 2023-12-16 01:48:08.000000 Python-Algorithm-pyal-1.1.8/src/pyal/list/dequeue_TEST.py
--rw-r--r--   0 summer     (502) staff       (20)     2340 2023-11-23 05:16:03.000000 Python-Algorithm-pyal-1.1.8/src/pyal/list/lfu_cache.py
--rw-r--r--   0 summer     (502) staff       (20)     3973 2023-12-17 17:59:08.000000 Python-Algorithm-pyal-1.1.8/src/pyal/list/linked_list.py
--rw-r--r--   0 summer     (502) staff       (20)     1592 2023-12-17 17:59:08.000000 Python-Algorithm-pyal-1.1.8/src/pyal/list/linked_list_TEST.py
--rw-r--r--   0 summer     (502) staff       (20)     1101 2023-11-23 05:16:03.000000 Python-Algorithm-pyal-1.1.8/src/pyal/list/lru_cache.py
--rw-r--r--   0 summer     (502) staff       (20)      455 2023-12-16 01:38:35.000000 Python-Algorithm-pyal-1.1.8/src/pyal/list/queue.py
--rw-r--r--   0 summer     (502) staff       (20)      259 2023-12-16 01:42:13.000000 Python-Algorithm-pyal-1.1.8/src/pyal/list/queue_TEST.py
--rw-r--r--   0 summer     (502) staff       (20)      484 2023-12-16 01:22:02.000000 Python-Algorithm-pyal-1.1.8/src/pyal/list/stack.py
--rw-r--r--   0 summer     (502) staff       (20)      318 2023-12-16 01:42:13.000000 Python-Algorithm-pyal-1.1.8/src/pyal/list/stack_TEST.py
-drwxr-xr-x   0 summer     (502) staff       (20)        0 2023-12-17 18:56:38.765771 Python-Algorithm-pyal-1.1.8/src/pyal/string/
--rw-r--r--   0 summer     (502) staff       (20)        0 2023-11-03 00:24:32.000000 Python-Algorithm-pyal-1.1.8/src/pyal/string/__init__.py
--rw-r--r--   0 summer     (502) staff       (20)      743 2023-11-20 21:04:00.000000 Python-Algorithm-pyal-1.1.8/src/pyal/string/search.py
--rw-r--r--   0 summer     (502) staff       (20)      337 2023-11-20 21:04:00.000000 Python-Algorithm-pyal-1.1.8/src/pyal/string/search_TEST.py
-drwxr-xr-x   0 summer     (502) staff       (20)        0 2023-12-17 18:56:38.770624 Python-Algorithm-pyal-1.1.8/src/pyal/tree/
--rw-r--r--   0 summer     (502) staff       (20)        0 2023-11-03 00:24:36.000000 Python-Algorithm-pyal-1.1.8/src/pyal/tree/__init__.py
--rw-r--r--   0 summer     (502) staff       (20)      895 2023-11-06 23:23:49.000000 Python-Algorithm-pyal-1.1.8/src/pyal/tree/disjoint_set.py
--rw-r--r--   0 summer     (502) staff       (20)      404 2023-11-20 21:03:56.000000 Python-Algorithm-pyal-1.1.8/src/pyal/tree/disjoint_set_TEST.py
--rw-r--r--   0 summer     (502) staff       (20)     3558 2023-12-16 01:22:02.000000 Python-Algorithm-pyal-1.1.8/src/pyal/tree/dynamic_heap.py
--rw-r--r--   0 summer     (502) staff       (20)      704 2023-11-20 21:03:56.000000 Python-Algorithm-pyal-1.1.8/src/pyal/tree/dynamic_heap_TEST.py
--rw-r--r--   0 summer     (502) staff       (20)      448 2023-12-16 01:22:02.000000 Python-Algorithm-pyal-1.1.8/src/pyal/tree/min_heap.py
--rw-r--r--   0 summer     (502) staff       (20)     7306 2023-12-16 02:04:40.000000 Python-Algorithm-pyal-1.1.8/src/pyal/tree/tree_map.py
--rw-r--r--   0 summer     (502) staff       (20)     2209 2023-12-16 01:22:36.000000 Python-Algorithm-pyal-1.1.8/src/pyal/tree/tree_map_TEST.py
+drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 01:17:42.206059 Python-Algorithm-pyal-1.1.9/
+-rw-r--r--   0 summer     (502) staff       (20)     3624 2024-04-03 01:17:42.205887 Python-Algorithm-pyal-1.1.9/PKG-INFO
+-rw-r--r--   0 summer     (502) staff       (20)     3055 2023-12-16 02:37:57.000000 Python-Algorithm-pyal-1.1.9/README.md
+-rw-r--r--   0 summer     (502) staff       (20)       94 2023-11-02 20:23:19.000000 Python-Algorithm-pyal-1.1.9/pyproject.toml
+-rw-r--r--   0 summer     (502) staff       (20)      732 2024-04-03 01:17:42.206774 Python-Algorithm-pyal-1.1.9/setup.cfg
+drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 01:17:42.170579 Python-Algorithm-pyal-1.1.9/src/
+drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 01:17:42.205289 Python-Algorithm-pyal-1.1.9/src/Python_Algorithm_pyal.egg-info/
+-rw-r--r--   0 summer     (502) staff       (20)     3624 2024-04-03 01:17:42.000000 Python-Algorithm-pyal-1.1.9/src/Python_Algorithm_pyal.egg-info/PKG-INFO
+-rw-r--r--   0 summer     (502) staff       (20)     1236 2024-04-03 01:17:42.000000 Python-Algorithm-pyal-1.1.9/src/Python_Algorithm_pyal.egg-info/SOURCES.txt
+-rw-r--r--   0 summer     (502) staff       (20)        1 2024-04-03 01:17:42.000000 Python-Algorithm-pyal-1.1.9/src/Python_Algorithm_pyal.egg-info/dependency_links.txt
+-rw-r--r--   0 summer     (502) staff       (20)        5 2024-04-03 01:17:42.000000 Python-Algorithm-pyal-1.1.9/src/Python_Algorithm_pyal.egg-info/top_level.txt
+drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 01:17:42.176103 Python-Algorithm-pyal-1.1.9/src/pyal/
+-rw-r--r--   0 summer     (502) staff       (20)      593 2024-04-03 01:16:58.000000 Python-Algorithm-pyal-1.1.9/src/pyal/__init__.py
+drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 01:17:42.179493 Python-Algorithm-pyal-1.1.9/src/pyal/common/
+-rw-r--r--   0 summer     (502) staff       (20)        0 2023-11-03 00:24:21.000000 Python-Algorithm-pyal-1.1.9/src/pyal/common/__init__.py
+-rw-r--r--   0 summer     (502) staff       (20)     9310 2024-03-25 21:11:02.000000 Python-Algorithm-pyal-1.1.9/src/pyal/common/algorithm.py
+-rw-r--r--   0 summer     (502) staff       (20)     3518 2023-12-20 06:27:08.000000 Python-Algorithm-pyal-1.1.9/src/pyal/common/algorithm_TEST.py
+drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 01:17:42.185644 Python-Algorithm-pyal-1.1.9/src/pyal/graph/
+-rw-r--r--   0 summer     (502) staff       (20)        0 2023-11-03 00:24:25.000000 Python-Algorithm-pyal-1.1.9/src/pyal/graph/__init__.py
+-rw-r--r--   0 summer     (502) staff       (20)     1842 2023-11-20 21:03:57.000000 Python-Algorithm-pyal-1.1.9/src/pyal/graph/graph.py
+-rw-r--r--   0 summer     (502) staff       (20)      576 2023-11-20 21:03:57.000000 Python-Algorithm-pyal-1.1.9/src/pyal/graph/graph_TEST.py
+-rw-r--r--   0 summer     (502) staff       (20)        7 2023-12-16 01:35:27.000000 Python-Algorithm-pyal-1.1.9/src/pyal/graph/minimum_span_tree.py
+-rw-r--r--   0 summer     (502) staff       (20)     1387 2023-11-20 21:03:57.000000 Python-Algorithm-pyal-1.1.9/src/pyal/graph/shortest_path.py
+-rw-r--r--   0 summer     (502) staff       (20)      780 2023-11-20 21:03:58.000000 Python-Algorithm-pyal-1.1.9/src/pyal/graph/shortest_path_TEST.py
+-rw-r--r--   0 summer     (502) staff       (20)      595 2023-11-20 21:03:58.000000 Python-Algorithm-pyal-1.1.9/src/pyal/graph/topological_traversal.py
+-rw-r--r--   0 summer     (502) staff       (20)      401 2023-11-20 21:03:57.000000 Python-Algorithm-pyal-1.1.9/src/pyal/graph/topological_traversal_TEST.py
+drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 01:17:42.196910 Python-Algorithm-pyal-1.1.9/src/pyal/list/
+-rw-r--r--   0 summer     (502) staff       (20)        0 2023-11-03 00:24:28.000000 Python-Algorithm-pyal-1.1.9/src/pyal/list/__init__.py
+-rw-r--r--   0 summer     (502) staff       (20)      130 2023-12-16 01:45:31.000000 Python-Algorithm-pyal-1.1.9/src/pyal/list/dequeue.py
+-rw-r--r--   0 summer     (502) staff       (20)      310 2023-12-16 01:48:08.000000 Python-Algorithm-pyal-1.1.9/src/pyal/list/dequeue_TEST.py
+-rw-r--r--   0 summer     (502) staff       (20)     2340 2023-11-23 05:16:03.000000 Python-Algorithm-pyal-1.1.9/src/pyal/list/lfu_cache.py
+-rw-r--r--   0 summer     (502) staff       (20)     4035 2023-12-19 22:17:29.000000 Python-Algorithm-pyal-1.1.9/src/pyal/list/linked_list.py
+-rw-r--r--   0 summer     (502) staff       (20)     1772 2023-12-19 22:16:39.000000 Python-Algorithm-pyal-1.1.9/src/pyal/list/linked_list_TEST.py
+-rw-r--r--   0 summer     (502) staff       (20)     1101 2023-11-23 05:16:03.000000 Python-Algorithm-pyal-1.1.9/src/pyal/list/lru_cache.py
+-rw-r--r--   0 summer     (502) staff       (20)      455 2023-12-16 01:38:35.000000 Python-Algorithm-pyal-1.1.9/src/pyal/list/queue.py
+-rw-r--r--   0 summer     (502) staff       (20)      259 2023-12-16 01:42:13.000000 Python-Algorithm-pyal-1.1.9/src/pyal/list/queue_TEST.py
+-rw-r--r--   0 summer     (502) staff       (20)      484 2023-12-16 01:22:02.000000 Python-Algorithm-pyal-1.1.9/src/pyal/list/stack.py
+-rw-r--r--   0 summer     (502) staff       (20)      318 2023-12-16 01:42:13.000000 Python-Algorithm-pyal-1.1.9/src/pyal/list/stack_TEST.py
+drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 01:17:42.198664 Python-Algorithm-pyal-1.1.9/src/pyal/string/
+-rw-r--r--   0 summer     (502) staff       (20)        0 2023-11-03 00:24:32.000000 Python-Algorithm-pyal-1.1.9/src/pyal/string/__init__.py
+-rw-r--r--   0 summer     (502) staff       (20)      743 2023-11-20 21:04:00.000000 Python-Algorithm-pyal-1.1.9/src/pyal/string/search.py
+-rw-r--r--   0 summer     (502) staff       (20)      337 2023-11-20 21:04:00.000000 Python-Algorithm-pyal-1.1.9/src/pyal/string/search_TEST.py
+drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 01:17:42.204436 Python-Algorithm-pyal-1.1.9/src/pyal/tree/
+-rw-r--r--   0 summer     (502) staff       (20)        0 2023-11-03 00:24:36.000000 Python-Algorithm-pyal-1.1.9/src/pyal/tree/__init__.py
+-rw-r--r--   0 summer     (502) staff       (20)      685 2023-12-25 08:28:48.000000 Python-Algorithm-pyal-1.1.9/src/pyal/tree/disjoint_set.py
+-rw-r--r--   0 summer     (502) staff       (20)      311 2023-12-25 05:29:03.000000 Python-Algorithm-pyal-1.1.9/src/pyal/tree/disjoint_set_TEST.py
+-rw-r--r--   0 summer     (502) staff       (20)     3558 2023-12-16 01:22:02.000000 Python-Algorithm-pyal-1.1.9/src/pyal/tree/dynamic_heap.py
+-rw-r--r--   0 summer     (502) staff       (20)      704 2023-11-20 21:03:56.000000 Python-Algorithm-pyal-1.1.9/src/pyal/tree/dynamic_heap_TEST.py
+-rw-r--r--   0 summer     (502) staff       (20)      448 2023-12-16 01:22:02.000000 Python-Algorithm-pyal-1.1.9/src/pyal/tree/min_heap.py
+-rw-r--r--   0 summer     (502) staff       (20)     7465 2024-04-03 01:16:13.000000 Python-Algorithm-pyal-1.1.9/src/pyal/tree/tree_map.py
+-rw-r--r--   0 summer     (502) staff       (20)     2209 2023-12-16 01:22:36.000000 Python-Algorithm-pyal-1.1.9/src/pyal/tree/tree_map_TEST.py
```

### Comparing `Python-Algorithm-pyal-1.1.8/PKG-INFO` & `Python-Algorithm-pyal-1.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: Python-Algorithm-pyal
-Version: 1.1.8
+Version: 1.1.9
 Summary: PYthon Algorithm Library (pyal) targets at providing a python version substitue of STL in C++, such as linked list, tree map, and other data structures and popular algorithms.
 Home-page: https://github.com/SummerRainET2008/PYthon_Algorithms_Library
 Author-email: tianxia0209@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # PYthon Algorithms Library (pyal)
 
 Python does not have some useful or important data structures, like `linked list`, `tree map`, just like STL in C++. 
 This library aims to provide a python counterpart of C++ STL.
```

### Comparing `Python-Algorithm-pyal-1.1.8/README.md` & `Python-Algorithm-pyal-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.1.8/setup.cfg` & `Python-Algorithm-pyal-1.1.9/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [metadata]
 name = Python-Algorithm-pyal
 authors = Summer Xia
 author_email = tianxia0209@gmail.com
-version = 1.1.8
+version = 1.1.9
 description = PYthon Algorithm Library (pyal) targets at providing a python version substitue of STL in C++, such as linked list, tree map, and other data structures and popular algorithms.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/SummerRainET2008/PYthon_Algorithms_Library
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= src
 packages = find:
-python_requires = >= 3.6
+python_requires = >= 3.8
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `Python-Algorithm-pyal-1.1.8/src/Python_Algorithm_pyal.egg-info/PKG-INFO` & `Python-Algorithm-pyal-1.1.9/src/Python_Algorithm_pyal.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: Python-Algorithm-pyal
-Version: 1.1.8
+Version: 1.1.9
 Summary: PYthon Algorithm Library (pyal) targets at providing a python version substitue of STL in C++, such as linked list, tree map, and other data structures and popular algorithms.
 Home-page: https://github.com/SummerRainET2008/PYthon_Algorithms_Library
 Author-email: tianxia0209@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # PYthon Algorithms Library (pyal)
 
 Python does not have some useful or important data structures, like `linked list`, `tree map`, just like STL in C++. 
 This library aims to provide a python counterpart of C++ STL.
```

### Comparing `Python-Algorithm-pyal-1.1.8/src/Python_Algorithm_pyal.egg-info/SOURCES.txt` & `Python-Algorithm-pyal-1.1.9/src/Python_Algorithm_pyal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.1.8/src/pyal/__init__.py` & `Python-Algorithm-pyal-1.1.9/src/pyal/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 from .tree.min_heap import MinHeap
 from .tree.tree_map import TreeMap
 from .graph.shortest_path import Dijkstra
 from .graph.graph import Graph
 from .graph.topological_traversal import topological_traversal
 from .string.search import search_KMP
 
-__version__ = "1.1.8"
+__version__ = "1.1.9"
```

### Comparing `Python-Algorithm-pyal-1.1.8/src/pyal/common/algorithm.py` & `Python-Algorithm-pyal-1.1.9/src/pyal/common/algorithm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 '''
 Author: Tian Xia (TianXia0209@gmail.com)
 '''
+import copy
 import sys
 import typing
 import functools
 import math
 from math import isinf
 
 INF = math.inf
 EPSILON = 1e-6
 
+def bit_not(m):
+  import ctypes
+  return ctypes.c_uint32(~m).value
+
 
 def is_none_or_empty(data) -> bool:
   '''This applies to any data type which has a __len__ method'''
   if data is None:
     return True
 
   try:
@@ -80,33 +85,24 @@
     for d in data:
       if prev is None or d != prev:
         yield d
         prev = d
 
   return list(run())
 
-def unique_in_place(data: list):
-  '''
-  1 2 3 4
-  1 1 2 3
-  :param data:
-  :return:
-  '''
-  p1 = 1
-  p2 = 1
-  while p2 < len(data):
-    if data[p2] != data[p1 - 1]:
-      data[p1] = data[p2]
-      p1 += 1
-      p2 += 1
-    else:
-      p2 += 1
+def unique_in_place(nums: list):
+  p1 = 0
+  for p2 in range(1, len(nums)):
+    if nums[p2] == nums[p1]:
+      continue
 
-  return p1
+    p1 += 1
+    nums[p1] = nums[p2]
 
+  return p1 + 1
 
 def cmp(a, b) -> int:
   return (a > b) - (a < b)
 
 
 def split_data_by_func(data: list, func):
   data1, data2 = [], []
@@ -195,19 +191,22 @@
   for p in range(1, len(data)):
     if data[p] < data[opt_pos]:
       opt_pos = p
 
   return opt_pos
 
 
-def make_list(shape: tuple, init_value):
+def make_list(shape: tuple, init_value: typing.Any):
   assert len(shape) > 0
 
   if len(shape) == 1:
-    return [init_value] * shape[0]
+    if init_value is None or isinstance(init_value, (int, float, str)):
+      return [init_value] * shape[0]
+    else:
+      return [copy.deepcopy(init_value) for _ in range(shape[0])]
 
   return [make_list(shape[1:], init_value) for _ in range(shape[0])]
 
 
 def swap(data: list, index1, index2):
   if index1 != index2:
     data[index1], data[index2] = data[index2], data[index1]
```

### Comparing `Python-Algorithm-pyal-1.1.8/src/pyal/common/algorithm_TEST.py` & `Python-Algorithm-pyal-1.1.9/src/pyal/common/algorithm_TEST.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,14 +45,19 @@
   assert data[argmin(data)] == 1
 
 
 def test_make_list():
   data = make_list((2, 3, 4), None)
   assert len(data) == 2 and len(data[0]) == 3 and len(data[0][0]) == 4
 
+  data = make_list((3,), [])
+  data[0].append(1)
+  data[1].append(2)
+  assert data[0] == [1]
+  assert data[2] == []
 
 def test_the_kth_element():
   import random
   data = [1, 2, 3, 4, 5, 6]
   random.shuffle(data)
 
   kth_smallest_element(data, 0)
```

### Comparing `Python-Algorithm-pyal-1.1.8/src/pyal/graph/graph.py` & `Python-Algorithm-pyal-1.1.9/src/pyal/graph/graph.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.1.8/src/pyal/graph/graph_TEST.py` & `Python-Algorithm-pyal-1.1.9/src/pyal/graph/graph_TEST.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.1.8/src/pyal/graph/shortest_path.py` & `Python-Algorithm-pyal-1.1.9/src/pyal/graph/shortest_path.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.1.8/src/pyal/graph/shortest_path_TEST.py` & `Python-Algorithm-pyal-1.1.9/src/pyal/graph/shortest_path_TEST.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.1.8/src/pyal/graph/topological_traversal.py` & `Python-Algorithm-pyal-1.1.9/src/pyal/graph/topological_traversal.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.1.8/src/pyal/list/lfu_cache.py` & `Python-Algorithm-pyal-1.1.9/src/pyal/list/lfu_cache.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.1.8/src/pyal/list/linked_list.py` & `Python-Algorithm-pyal-1.1.9/src/pyal/list/linked_list.py`

 * *Files 3% similar despite different names*

```diff
@@ -120,16 +120,16 @@
 
   def rbegin(self):
     return self._fake_tail._prev
 
   def rend(self):
     return self._fake_head
 
-  def insert_element(self, pos_node: ListNode, e):
-    self.insert(pos_node, ListNode(e))
+  def insert_element(self, pos_node: ListNode, e)-> ListNode:
+    return self.insert(pos_node, ListNode(e))
 
   def _check_node_validity(self, node):
     assert node is not None
     assert node not in [self._fake_head, self._fake_tail]
 
   def insert(self, pos_node: ListNode, node: ListNode):
     self._check_node_validity(node)
@@ -137,23 +137,27 @@
     nd1, nd2, nd3 = pos_node._prev, node, pos_node
     nd1._next = nd2
     nd2._prev = nd1
     nd2._next = nd3
     nd3._prev = nd2
     self._num += 1
 
-  def remove(self, node: ListNode):
+    return node
+
+  def remove(self, node: ListNode)-> ListNode:
     self._check_node_validity(node)
 
     nd1, nd2, nd3 = node._prev, node, node._next
     nd1._next = nd3
     nd3._prev = nd1
     nd2._prev = nd2._next = None
     self._num -= 1
 
+    return nd3
+
   def index(self, content) -> ListNode:
     '''
     :param content:
     :return: node if it exists else None
     '''
     node = self.begin()
     while node is not self.end():
```

### Comparing `Python-Algorithm-pyal-1.1.8/src/pyal/list/linked_list_TEST.py` & `Python-Algorithm-pyal-1.1.9/src/pyal/list/linked_list_TEST.py`

 * *Files 27% similar despite different names*

```diff
@@ -42,29 +42,35 @@
 
 def test_insertion():
   list = LinkedList()
   list.push_back(1)
   list.push_back(2)
   list.push_back(3)
   list.push_back(4)
-  list.insert_element(list.begin(), 0)
+  node = list.insert_element(list.begin(), 0)
+  assert node.get() == 0
   list.insert(list.rbegin(), ListNode(100))
+  assert list.to_list() == [0, 1, 2, 3, 100, 4]
 
   iter = list.begin()
   iter = iter.next()
-  list.remove(iter)
+  next_node = list.remove(iter)
+  assert next_node.get() == 2
 
   data = []
   iter = list.begin()
   while iter is not list.end():
     data.append(iter.get())
     iter = iter.next()
 
   assert data == [0, 2, 3, 100, 4]
 
+  list.get(3).set(3.5)
+  assert list.get(3).get() == 3.5
+
   data = []
   iter = list.rbegin()
   while iter is not list.rend():
     data.append(iter.get())
     iter = iter.prev()
 
-  assert data == [0, 2, 3, 100, 4][::-1]
+  assert data == [0, 2, 3, 3.5, 4][::-1]
```

### Comparing `Python-Algorithm-pyal-1.1.8/src/pyal/list/lru_cache.py` & `Python-Algorithm-pyal-1.1.9/src/pyal/list/lru_cache.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.1.8/src/pyal/string/search.py` & `Python-Algorithm-pyal-1.1.9/src/pyal/string/search.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.1.8/src/pyal/tree/disjoint_set.py` & `Python-Algorithm-pyal-1.1.9/src/pyal/tree/disjoint_set.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,30 @@
 '''
 Author: Tian Xia (TianXia0209@gmail.com)
 '''
 
-
 class DisjointSet:
-  def __init__(self, n):
+  def __init__(self):
     self._fathers = {}
     self._sizes = {}
-    self._clusters_num = n
-
-  def combine(self, a, b):
-    assert 0 <= a < self._clusters_num
-    assert 0 <= b < self._clusters_num
 
+  def combine(self, a, b)-> bool:
     c1 = self.get_cluster_id(a)
     c2 = self.get_cluster_id(b)
     if c1 == c2:
-      return
+      return False
 
     if self._sizes.get(c1, 1) > self._sizes.get(c2, 1):
-      self.combine(b, a)
-      return
+      return self.combine(b, a)
 
     self._fathers[c1] = c2
     self._sizes[c2] = self._sizes.get(c2, 1) + self._sizes.get(c1, 1)
-    self._clusters_num -= 1
+    return True
 
   def get_cluster_id(self, a):
-    assert 0 <= a < self._clusters_num
-
-    father = self._fathers.get(a, -1)
-    if father == -1:
+    father = self._fathers.get(a, None)
+    if father is None:
       return a
     cluster_id = self.get_cluster_id(father)
     self._fathers[a] = cluster_id
-    return cluster_id
 
-  def get_cluster_num(self):
-    return self._clusters_num
+    return cluster_id
```

### Comparing `Python-Algorithm-pyal-1.1.8/src/pyal/tree/dynamic_heap.py` & `Python-Algorithm-pyal-1.1.9/src/pyal/tree/dynamic_heap.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.1.8/src/pyal/tree/dynamic_heap_TEST.py` & `Python-Algorithm-pyal-1.1.9/src/pyal/tree/dynamic_heap_TEST.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.1.8/src/pyal/tree/tree_map.py` & `Python-Algorithm-pyal-1.1.9/src/pyal/tree/tree_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,27 +88,27 @@
     return self._get_depth(self._left) - self._get_depth(self._right)
 
   @staticmethod
   def _reset_node(node, from_left: bool):
     node._reset_depth()
     bf = node._get_balance_factor()
 
-    if bf == -2:
+    if bf in [-2, -3]:
       return node._left_rotate()
 
     elif bf == -1:
       return node if not from_left else node._left_rotate()
 
     elif bf == 0:
       return node
 
     elif bf == 1:
       return node if from_left else node._right_rotate()
 
-    elif bf == 2:
+    elif bf in [2, 3]:
       return node._right_rotate()
 
     else:
       assert False
 
   @staticmethod
   def _reset_balance(node, from_left: bool):
@@ -219,14 +219,20 @@
 
   def key_list_begin(self)-> ListNode:
     return self._key_list.begin()
 
   def key_list_end(self)-> ListNode:
     return self._key_list.end()
 
+  def key_list_rbegin(self)-> ListNode:
+    return self._key_list.rbegin()
+
+  def key_list_rend(self)-> ListNode:
+    return self._key_list.rend()
+
   def lower_bound(self, key)-> ListNode:  # return key_list node
     if self._root is None:
       return self.key_list_end()
 
     node = self._root._find_lower_bound(key)
     if node is None:
       return self._key_list.end()
```

### Comparing `Python-Algorithm-pyal-1.1.8/src/pyal/tree/tree_map_TEST.py` & `Python-Algorithm-pyal-1.1.9/src/pyal/tree/tree_map_TEST.py`

 * *Files identical despite different names*

