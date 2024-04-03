# Comparing `tmp/reasoner-transpiler-2.0.7.tar.gz` & `tmp/reasoner-transpiler-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner-transpiler-2.0.7.tar", last modified: Fri Mar  8 17:02:56 2024, max compression
+gzip compressed data, was "reasoner-transpiler-2.0.8.tar", last modified: Fri Mar 22 18:59:06 2024, max compression
```

## Comparing `reasoner-transpiler-2.0.7.tar` & `reasoner-transpiler-2.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 17:02:56.950867 reasoner-transpiler-2.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-03-08 17:02:56.950867 reasoner-transpiler-2.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-03-08 17:02:54.000000 reasoner-transpiler-2.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 17:02:56.950867 reasoner-transpiler-2.0.7/reasoner_transpiler/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-08 17:02:54.000000 reasoner-transpiler-2.0.7/reasoner_transpiler/attribute_types.json
--rw-r--r--   0 runner    (1001) docker     (127)     6967 2024-03-08 17:02:54.000000 reasoner-transpiler-2.0.7/reasoner_transpiler/cypher.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-03-08 17:02:54.000000 reasoner-transpiler-2.0.7/reasoner_transpiler/cypher_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-08 17:02:54.000000 reasoner-transpiler-2.0.7/reasoner_transpiler/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19908 2024-03-08 17:02:54.000000 reasoner-transpiler-2.0.7/reasoner_transpiler/matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     8780 2024-03-08 17:02:54.000000 reasoner-transpiler-2.0.7/reasoner_transpiler/nesting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-03-08 17:02:54.000000 reasoner-transpiler-2.0.7/reasoner_transpiler/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 17:02:56.950867 reasoner-transpiler-2.0.7/reasoner_transpiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-03-08 17:02:56.000000 reasoner-transpiler-2.0.7/reasoner_transpiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-03-08 17:02:56.000000 reasoner-transpiler-2.0.7/reasoner_transpiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 17:02:56.000000 reasoner-transpiler-2.0.7/reasoner_transpiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 17:02:56.000000 reasoner-transpiler-2.0.7/reasoner_transpiler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-08 17:02:56.000000 reasoner-transpiler-2.0.7/reasoner_transpiler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-08 17:02:56.000000 reasoner-transpiler-2.0.7/reasoner_transpiler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-08 17:02:56.950867 reasoner-transpiler-2.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-08 17:02:54.000000 reasoner-transpiler-2.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:59:06.497718 reasoner-transpiler-2.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-03-22 18:59:06.497718 reasoner-transpiler-2.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-03-22 18:59:04.000000 reasoner-transpiler-2.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:59:06.493718 reasoner-transpiler-2.0.8/reasoner_transpiler/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-22 18:59:04.000000 reasoner-transpiler-2.0.8/reasoner_transpiler/attribute_types.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6951 2024-03-22 18:59:04.000000 reasoner-transpiler-2.0.8/reasoner_transpiler/cypher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-03-22 18:59:04.000000 reasoner-transpiler-2.0.8/reasoner_transpiler/cypher_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-22 18:59:04.000000 reasoner-transpiler-2.0.8/reasoner_transpiler/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19908 2024-03-22 18:59:04.000000 reasoner-transpiler-2.0.8/reasoner_transpiler/matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8780 2024-03-22 18:59:04.000000 reasoner-transpiler-2.0.8/reasoner_transpiler/nesting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-03-22 18:59:04.000000 reasoner-transpiler-2.0.8/reasoner_transpiler/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:59:06.497718 reasoner-transpiler-2.0.8/reasoner_transpiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-03-22 18:59:06.000000 reasoner-transpiler-2.0.8/reasoner_transpiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-03-22 18:59:06.000000 reasoner-transpiler-2.0.8/reasoner_transpiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 18:59:06.000000 reasoner-transpiler-2.0.8/reasoner_transpiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 18:59:06.000000 reasoner-transpiler-2.0.8/reasoner_transpiler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-22 18:59:06.000000 reasoner-transpiler-2.0.8/reasoner_transpiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-22 18:59:06.000000 reasoner-transpiler-2.0.8/reasoner_transpiler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 18:59:06.497718 reasoner-transpiler-2.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-22 18:59:04.000000 reasoner-transpiler-2.0.8/setup.py
```

### Comparing `reasoner-transpiler-2.0.7/README.md` & `reasoner-transpiler-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `reasoner-transpiler-2.0.7/reasoner_transpiler/cypher.py` & `reasoner-transpiler-2.0.8/reasoner_transpiler/cypher.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 ]
 RESERVED_EDGE_PROPS = [
     "id",
     "predicate",
 ]
 
 EDGE_SOURCE_PROPS = [
-    "biolink:aggregator_knowledge_source",
-    "biolink:primary_knowledge_source"
+    "aggregator_knowledge_source",
+    "primary_knowledge_source"
 ]
 
 def nest_op(operator, *args):
     """Generate a nested set of operations from a flat expression."""
     if len(args) > 2:
         return [operator, args[0], nest_op(operator, *args[1:])]
     else:
```

### Comparing `reasoner-transpiler-2.0.7/reasoner_transpiler/cypher_expression.py` & `reasoner-transpiler-2.0.8/reasoner_transpiler/cypher_expression.py`

 * *Files identical despite different names*

### Comparing `reasoner-transpiler-2.0.7/reasoner_transpiler/matching.py` & `reasoner-transpiler-2.0.8/reasoner_transpiler/matching.py`

 * *Files identical despite different names*

### Comparing `reasoner-transpiler-2.0.7/reasoner_transpiler/nesting.py` & `reasoner-transpiler-2.0.8/reasoner_transpiler/nesting.py`

 * *Files identical despite different names*

### Comparing `reasoner-transpiler-2.0.7/reasoner_transpiler/util.py` & `reasoner-transpiler-2.0.8/reasoner_transpiler/util.py`

 * *Files identical despite different names*

### Comparing `reasoner-transpiler-2.0.7/setup.py` & `reasoner-transpiler-2.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Setup reasoner-transpiler package."""
 from setuptools import setup
 
 setup(
     name="reasoner-transpiler",
-    version="2.0.7",
+    version="2.0.8",
     author="Patrick Wang",
     author_email="patrick@covar.com",
     maintainer="Yaphet Kebede",
     maintainer_email="kebedey@renci.org",
     url="https://github.com/ranking-agent/reasoner-transpiler",
     description="TRAPI → Cypher transpiler",
     packages=["reasoner_transpiler"],
```

