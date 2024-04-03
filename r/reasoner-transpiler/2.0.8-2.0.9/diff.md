# Comparing `tmp/reasoner-transpiler-2.0.8.tar.gz` & `tmp/reasoner-transpiler-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner-transpiler-2.0.8.tar", last modified: Fri Mar 22 18:59:06 2024, max compression
+gzip compressed data, was "reasoner-transpiler-2.0.9.tar", last modified: Wed Apr  3 20:22:42 2024, max compression
```

## Comparing `reasoner-transpiler-2.0.8.tar` & `reasoner-transpiler-2.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:59:06.497718 reasoner-transpiler-2.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-03-22 18:59:06.497718 reasoner-transpiler-2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-03-22 18:59:04.000000 reasoner-transpiler-2.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:59:06.493718 reasoner-transpiler-2.0.8/reasoner_transpiler/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-22 18:59:04.000000 reasoner-transpiler-2.0.8/reasoner_transpiler/attribute_types.json
--rw-r--r--   0 runner    (1001) docker     (127)     6951 2024-03-22 18:59:04.000000 reasoner-transpiler-2.0.8/reasoner_transpiler/cypher.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-03-22 18:59:04.000000 reasoner-transpiler-2.0.8/reasoner_transpiler/cypher_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-22 18:59:04.000000 reasoner-transpiler-2.0.8/reasoner_transpiler/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19908 2024-03-22 18:59:04.000000 reasoner-transpiler-2.0.8/reasoner_transpiler/matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     8780 2024-03-22 18:59:04.000000 reasoner-transpiler-2.0.8/reasoner_transpiler/nesting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-03-22 18:59:04.000000 reasoner-transpiler-2.0.8/reasoner_transpiler/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:59:06.497718 reasoner-transpiler-2.0.8/reasoner_transpiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-03-22 18:59:06.000000 reasoner-transpiler-2.0.8/reasoner_transpiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-03-22 18:59:06.000000 reasoner-transpiler-2.0.8/reasoner_transpiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 18:59:06.000000 reasoner-transpiler-2.0.8/reasoner_transpiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 18:59:06.000000 reasoner-transpiler-2.0.8/reasoner_transpiler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-22 18:59:06.000000 reasoner-transpiler-2.0.8/reasoner_transpiler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-22 18:59:06.000000 reasoner-transpiler-2.0.8/reasoner_transpiler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 18:59:06.497718 reasoner-transpiler-2.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-22 18:59:04.000000 reasoner-transpiler-2.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:22:42.200646 reasoner-transpiler-2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-03 20:22:42.200646 reasoner-transpiler-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-03 20:22:38.000000 reasoner-transpiler-2.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:22:42.200646 reasoner-transpiler-2.0.9/reasoner_transpiler/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-03 20:22:38.000000 reasoner-transpiler-2.0.9/reasoner_transpiler/attribute_types.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7199 2024-04-03 20:22:38.000000 reasoner-transpiler-2.0.9/reasoner_transpiler/cypher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-03 20:22:38.000000 reasoner-transpiler-2.0.9/reasoner_transpiler/cypher_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-03 20:22:38.000000 reasoner-transpiler-2.0.9/reasoner_transpiler/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20008 2024-04-03 20:22:38.000000 reasoner-transpiler-2.0.9/reasoner_transpiler/matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8780 2024-04-03 20:22:38.000000 reasoner-transpiler-2.0.9/reasoner_transpiler/nesting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-03 20:22:38.000000 reasoner-transpiler-2.0.9/reasoner_transpiler/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:22:42.200646 reasoner-transpiler-2.0.9/reasoner_transpiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-03 20:22:42.000000 reasoner-transpiler-2.0.9/reasoner_transpiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-03 20:22:42.000000 reasoner-transpiler-2.0.9/reasoner_transpiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 20:22:42.000000 reasoner-transpiler-2.0.9/reasoner_transpiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 20:22:42.000000 reasoner-transpiler-2.0.9/reasoner_transpiler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 20:22:42.000000 reasoner-transpiler-2.0.9/reasoner_transpiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-03 20:22:42.000000 reasoner-transpiler-2.0.9/reasoner_transpiler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 20:22:42.200646 reasoner-transpiler-2.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-03 20:22:38.000000 reasoner-transpiler-2.0.9/setup.py
```

### Comparing `reasoner-transpiler-2.0.8/README.md` & `reasoner-transpiler-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `reasoner-transpiler-2.0.8/reasoner_transpiler/cypher.py` & `reasoner-transpiler-2.0.9/reasoner_transpiler/cypher.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,17 +17,21 @@
     "category",
 ]
 RESERVED_EDGE_PROPS = [
     "id",
     "predicate",
 ]
 
+# this should really be one representation or the other, or be configurable,
+# but we have graphs with each now so temporarily (I hope, hope, hope) looking for both
 EDGE_SOURCE_PROPS = [
     "aggregator_knowledge_source",
-    "primary_knowledge_source"
+    "primary_knowledge_source",
+    "biolink:aggregator_knowledge_source",
+    "biolink:primary_knowledge_source"
 ]
 
 def nest_op(operator, *args):
     """Generate a nested set of operations from a flat expression."""
     if len(args) > 2:
         return [operator, args[0], nest_op(operator, *args[1:])]
     else:
```

### Comparing `reasoner-transpiler-2.0.8/reasoner_transpiler/cypher_expression.py` & `reasoner-transpiler-2.0.9/reasoner_transpiler/cypher_expression.py`

 * *Files identical despite different names*

### Comparing `reasoner-transpiler-2.0.8/reasoner_transpiler/matching.py` & `reasoner-transpiler-2.0.9/reasoner_transpiler/matching.py`

 * *Files 1% similar despite different names*

```diff
@@ -439,20 +439,21 @@
                 "ids": qnode.pop("ids"),
                 "categories": qnode.pop("categories", None),
                 "_return": False,
             }
             for qnode_id, qnode in qgraph["nodes"].items()
             if qnode.get("ids", None) is not None and qnode_id not in qnode_ids_with_hierarchy_edges
         }
+        subclass_depth = kwargs['subclass_depth'] if 'subclass_depth' in kwargs else 1
         subclass_edges = {
             qnode_id[:-11] + "_subclass_edge": {
                 "subject": qnode_id[:-11],
                 "object": qnode_id,
                 "predicates": ["biolink:subclass_of"],
-                "_length": (0, 1),
+                "_length": (0, subclass_depth),
                 "_invert": False,
                 "_return": False,
             }
             for qnode_id in superclasses
         }
         qgraph["nodes"].update(superclasses)
         qgraph["edges"].update(subclass_edges)
```

### Comparing `reasoner-transpiler-2.0.8/reasoner_transpiler/nesting.py` & `reasoner-transpiler-2.0.9/reasoner_transpiler/nesting.py`

 * *Files identical despite different names*

### Comparing `reasoner-transpiler-2.0.8/reasoner_transpiler/util.py` & `reasoner-transpiler-2.0.9/reasoner_transpiler/util.py`

 * *Files identical despite different names*

### Comparing `reasoner-transpiler-2.0.8/setup.py` & `reasoner-transpiler-2.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Setup reasoner-transpiler package."""
 from setuptools import setup
 
 setup(
     name="reasoner-transpiler",
-    version="2.0.8",
+    version="2.0.9",
     author="Patrick Wang",
     author_email="patrick@covar.com",
     maintainer="Yaphet Kebede",
     maintainer_email="kebedey@renci.org",
     url="https://github.com/ranking-agent/reasoner-transpiler",
     description="TRAPI → Cypher transpiler",
     packages=["reasoner_transpiler"],
```

