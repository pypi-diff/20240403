# Comparing `tmp/genice_core-0.9.tar.gz` & `tmp/genice_core-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genice_core-0.9.tar", max compression
+gzip compressed data, was "genice_core-0.9.1.tar", max compression
```

## Comparing `genice_core-0.9.tar` & `genice_core-0.9.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1075 2023-11-23 02:46:52.070348 genice_core-0.9/LICENSE
--rw-r--r--   0        0        0     4830 2023-11-28 04:17:56.453219 genice_core-0.9/genice_core/__init__.py
--rw-r--r--   0        0        0     4428 2023-11-23 05:16:48.369754 genice_core-0.9/genice_core/dipole.py
--rw-r--r--   0        0        0    12450 2023-11-23 02:46:52.071916 genice_core-0.9/genice_core/topology.py
--rw-r--r--   0        0        0     1031 2023-12-10 14:19:49.565645 genice_core-0.9/pyproject.toml
--rw-r--r--   0        0        0      502 1970-01-01 00:00:00.000000 genice_core-0.9/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-11-23 02:46:52.070348 genice_core-0.9.1/LICENSE
+-rw-r--r--   0        0        0     4854 2024-04-03 11:14:30.709369 genice_core-0.9.1/genice_core/__init__.py
+-rw-r--r--   0        0        0     4428 2023-11-23 05:16:48.369754 genice_core-0.9.1/genice_core/dipole.py
+-rw-r--r--   0        0        0    12302 2024-04-03 11:12:25.697451 genice_core-0.9.1/genice_core/topology.py
+-rw-r--r--   0        0        0     1294 2024-04-03 11:17:00.633914 genice_core-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      549 1970-01-01 00:00:00.000000 genice_core-0.9.1/PKG-INFO
```

### Comparing `genice_core-0.9/LICENSE` & `genice_core-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `genice_core-0.9/genice_core/__init__.py` & `genice_core-0.9.1/genice_core/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 """
 .. include:: ../README.md
 """
+
 import numpy as np
 import networkx as nx
 from genice_core.topology import noodlize, split_into_simple_paths, balance
 from genice_core.dipole import optimize, vector_sum, _dipole_moment_pbc
 from typing import Union
 from logging import getLogger, DEBUG
 
+__version__ = "0.9.1"
+
 
 def ice_graph(
     g: nx.Graph,
     vertexPositions: Union[np.ndarray, None] = None,
     isPeriodicBoundary: bool = False,
     dipoleOptimizationCycles: int = 0,
     fixedEdges: nx.DiGraph = nx.DiGraph(),
```

### Comparing `genice_core-0.9/genice_core/dipole.py` & `genice_core-0.9.1/genice_core/dipole.py`

 * *Files identical despite different names*

### Comparing `genice_core-0.9/genice_core/topology.py` & `genice_core-0.9.1/genice_core/topology.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,18 +102,14 @@
     offset = len(g)
 
     # divided graph
     g_noodles = nx.Graph(g)
     for edge in fixed.edges():
         g_noodles.remove_edge(*edge)
 
-    if logger.isEnabledFor(DEBUG):
-        for node in g_noodles:
-            assert g_noodles.degree(node) in (0, 2, 4), "An node of odd-degree."
-
     for v in g:
         if g_fix.has_node(v):
             nfixed = g_fix.degree[v]
         else:
             nfixed = 0
         if nfixed == 0:
             _divide(g_noodles, v, offset)
```

### Comparing `genice_core-0.9/pyproject.toml` & `genice_core-0.9.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,47 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
+# poetry self add poetry-version-plugin
+[tool.poetry-version-plugin]
+source = "init"
 
 [tool.poetry]
 name = "genice-core"
-version = "0.9" # major.minor.fix
+version = "0.0.0"
 authors = [
   "Masakazu Matsumoto <vitroid@gmail.com>", 
 ]
 description = "Core algorithms of GenIce2"
 [tool.poetry.dependencies]
-python = ">=3.9"
+python = ">=3.9,<4.0"
 # readme = "README.md"
 # requires-python = ">=3.9"
 # classifiers = [
 #     "Programming Language :: Python :: 3",
 #     "License :: OSI Approved :: MIT License",
 #     "Operating System :: OS Independent",
 # ]
 # dependencies = ["numpy", "networkx"]
 networkx = "^3.2.1"
 numpy = "^1.26.2"
+pdoc3 = "^0.10.0"
 
 [tool.poetry.group.dev.dependencies]
 pdoc = "^14.1.0"
 toml = "^0.10.2"
 
+
+[tool.poetry.group.test.dependencies]
+pytest = "^7.4.4"
+genice2 = {git = "https://github.com/vitroid/GenIce.git", rev = "genice-core"}
+clustice = {git = "https://github.com/ClustIce/ClustIce.git"}
+
 [project.urls]
 "Homepage" = "https://github.com/genice-dev/genice-core"
 "Bug Tracker" = "https://github.com/genice-dev/genice-core/issues"
 "manual" = "https://genice-dev.github.io/genice-core"
 
-[genice]
+[tool.genice.urls]
 "logo" = "https://raw.githubusercontent.com/vitroid/GenIce/develop/logo/genice-v0.png"
-"url" = "https://github.com/vitroid/GenIce"
-"repo" = "https://pypi.python.org/pypi/GenIce"
+"repository" = "https://pypi.python.org/pypi/GenIce"
```

