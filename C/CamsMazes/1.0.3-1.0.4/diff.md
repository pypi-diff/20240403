# Comparing `tmp/CamsMazes-1.0.3.tar.gz` & `tmp/CamsMazes-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CamsMazes-1.0.3.tar", last modified: Wed Apr  3 18:11:41 2024, max compression
+gzip compressed data, was "CamsMazes-1.0.4.tar", last modified: Wed Apr  3 18:17:49 2024, max compression
```

## Comparing `CamsMazes-1.0.3.tar` & `CamsMazes-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 18:11:41.238385 CamsMazes-1.0.3/
--rw-rw-rw-   0        0        0     3480 2024-04-03 18:11:41.235381 CamsMazes-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3078 2024-04-03 15:18:03.000000 CamsMazes-1.0.3/README.md
--rw-rw-rw-   0        0        0      427 2024-04-03 18:11:27.000000 CamsMazes-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-03 18:11:41.238385 CamsMazes-1.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-03 18:11:41.172137 CamsMazes-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-03 18:11:41.199235 CamsMazes-1.0.3/src/CamsMazes/
--rw-rw-rw-   0        0        0    12405 2024-04-03 18:05:06.000000 CamsMazes-1.0.3/src/CamsMazes/maze.py
--rw-rw-rw-   0        0        0     3521 2024-04-03 18:10:59.000000 CamsMazes-1.0.3/src/CamsMazes/maze_visualizer.py
-drwxrwxrwx   0        0        0        0 2024-04-03 18:11:41.234378 CamsMazes-1.0.3/src/CamsMazes.egg-info/
--rw-rw-rw-   0        0        0     3480 2024-04-03 18:11:41.000000 CamsMazes-1.0.3/src/CamsMazes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2024-04-03 18:11:41.000000 CamsMazes-1.0.3/src/CamsMazes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 18:11:41.000000 CamsMazes-1.0.3/src/CamsMazes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-03 18:11:41.000000 CamsMazes-1.0.3/src/CamsMazes.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-03 18:11:41.000000 CamsMazes-1.0.3/src/CamsMazes.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 18:17:49.275166 CamsMazes-1.0.4/
+-rw-rw-rw-   0        0        0     3480 2024-04-03 18:17:49.274166 CamsMazes-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3078 2024-04-03 15:18:03.000000 CamsMazes-1.0.4/README.md
+-rw-rw-rw-   0        0        0      427 2024-04-03 18:17:35.000000 CamsMazes-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-03 18:17:49.275166 CamsMazes-1.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-03 18:17:49.252214 CamsMazes-1.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-03 18:17:49.256213 CamsMazes-1.0.4/src/CamsMazes/
+-rw-rw-rw-   0        0        0    12405 2024-04-03 18:05:06.000000 CamsMazes-1.0.4/src/CamsMazes/maze.py
+-rw-rw-rw-   0        0        0     3535 2024-04-03 18:17:07.000000 CamsMazes-1.0.4/src/CamsMazes/maze_visualizer.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:17:49.273166 CamsMazes-1.0.4/src/CamsMazes.egg-info/
+-rw-rw-rw-   0        0        0     3480 2024-04-03 18:17:49.000000 CamsMazes-1.0.4/src/CamsMazes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2024-04-03 18:17:49.000000 CamsMazes-1.0.4/src/CamsMazes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 18:17:49.000000 CamsMazes-1.0.4/src/CamsMazes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-03 18:17:49.000000 CamsMazes-1.0.4/src/CamsMazes.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-03 18:17:49.000000 CamsMazes-1.0.4/src/CamsMazes.egg-info/top_level.txt
```

### Comparing `CamsMazes-1.0.3/PKG-INFO` & `CamsMazes-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CamsMazes
-Version: 1.0.3
+Version: 1.0.4
 Summary: Maze Generator and Solver using DFS
 Author-email: Cameron Rolfe <cameronrolfedev@example.com>
 Project-URL: Homepage, https://github.com/CameronRolfe/MazeGenerator
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 Requires-Dist: Pillow
```

### Comparing `CamsMazes-1.0.3/README.md` & `CamsMazes-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `CamsMazes-1.0.3/src/CamsMazes/maze.py` & `CamsMazes-1.0.4/src/CamsMazes/maze.py`

 * *Files identical despite different names*

### Comparing `CamsMazes-1.0.3/src/CamsMazes/maze_visualizer.py` & `CamsMazes-1.0.4/src/CamsMazes/maze_visualizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from tkinter import *
 import time
-from maze import Maze
+from src.CamsMazes.maze import Maze
 
 class MazeVisualizer:
     class CellVisualizer:
         def __init__(self, canvas, cell_size):
             self.canvas = canvas
             self.cell_size = cell_size
             self.visited = False
```

### Comparing `CamsMazes-1.0.3/src/CamsMazes.egg-info/PKG-INFO` & `CamsMazes-1.0.4/src/CamsMazes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CamsMazes
-Version: 1.0.3
+Version: 1.0.4
 Summary: Maze Generator and Solver using DFS
 Author-email: Cameron Rolfe <cameronrolfedev@example.com>
 Project-URL: Homepage, https://github.com/CameronRolfe/MazeGenerator
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 Requires-Dist: Pillow
```

