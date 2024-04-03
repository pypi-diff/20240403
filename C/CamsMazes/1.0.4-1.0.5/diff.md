# Comparing `tmp/CamsMazes-1.0.4.tar.gz` & `tmp/CamsMazes-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CamsMazes-1.0.4.tar", last modified: Wed Apr  3 18:17:49 2024, max compression
+gzip compressed data, was "CamsMazes-1.0.5.tar", last modified: Wed Apr  3 18:55:45 2024, max compression
```

## Comparing `CamsMazes-1.0.4.tar` & `CamsMazes-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 18:17:49.275166 CamsMazes-1.0.4/
--rw-rw-rw-   0        0        0     3480 2024-04-03 18:17:49.274166 CamsMazes-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3078 2024-04-03 15:18:03.000000 CamsMazes-1.0.4/README.md
--rw-rw-rw-   0        0        0      427 2024-04-03 18:17:35.000000 CamsMazes-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-03 18:17:49.275166 CamsMazes-1.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-03 18:17:49.252214 CamsMazes-1.0.4/src/
-drwxrwxrwx   0        0        0        0 2024-04-03 18:17:49.256213 CamsMazes-1.0.4/src/CamsMazes/
--rw-rw-rw-   0        0        0    12405 2024-04-03 18:05:06.000000 CamsMazes-1.0.4/src/CamsMazes/maze.py
--rw-rw-rw-   0        0        0     3535 2024-04-03 18:17:07.000000 CamsMazes-1.0.4/src/CamsMazes/maze_visualizer.py
-drwxrwxrwx   0        0        0        0 2024-04-03 18:17:49.273166 CamsMazes-1.0.4/src/CamsMazes.egg-info/
--rw-rw-rw-   0        0        0     3480 2024-04-03 18:17:49.000000 CamsMazes-1.0.4/src/CamsMazes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2024-04-03 18:17:49.000000 CamsMazes-1.0.4/src/CamsMazes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 18:17:49.000000 CamsMazes-1.0.4/src/CamsMazes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-03 18:17:49.000000 CamsMazes-1.0.4/src/CamsMazes.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-03 18:17:49.000000 CamsMazes-1.0.4/src/CamsMazes.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 18:55:45.337355 CamsMazes-1.0.5/
+-rw-rw-rw-   0        0        0     3480 2024-04-03 18:55:45.336318 CamsMazes-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3078 2024-04-03 15:18:03.000000 CamsMazes-1.0.5/README.md
+-rw-rw-rw-   0        0        0      427 2024-04-03 18:53:53.000000 CamsMazes-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-03 18:55:45.337355 CamsMazes-1.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-03 18:55:45.303310 CamsMazes-1.0.5/src/
+drwxrwxrwx   0        0        0        0 2024-04-03 18:55:45.316351 CamsMazes-1.0.5/src/CamsMazes/
+-rw-rw-rw-   0        0        0        0 2024-04-03 18:44:45.000000 CamsMazes-1.0.5/src/CamsMazes/__init__.py
+-rw-rw-rw-   0        0        0    12405 2024-04-03 18:55:28.000000 CamsMazes-1.0.5/src/CamsMazes/maze.py
+-rw-rw-rw-   0        0        0     3522 2024-04-03 18:55:30.000000 CamsMazes-1.0.5/src/CamsMazes/maze_visualizer.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:55:45.335395 CamsMazes-1.0.5/src/CamsMazes.egg-info/
+-rw-rw-rw-   0        0        0     3480 2024-04-03 18:55:45.000000 CamsMazes-1.0.5/src/CamsMazes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2024-04-03 18:55:45.000000 CamsMazes-1.0.5/src/CamsMazes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 18:55:45.000000 CamsMazes-1.0.5/src/CamsMazes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-03 18:55:45.000000 CamsMazes-1.0.5/src/CamsMazes.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-03 18:55:45.000000 CamsMazes-1.0.5/src/CamsMazes.egg-info/top_level.txt
```

### Comparing `CamsMazes-1.0.4/PKG-INFO` & `CamsMazes-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CamsMazes
-Version: 1.0.4
+Version: 1.0.5
 Summary: Maze Generator and Solver using DFS
 Author-email: Cameron Rolfe <cameronrolfedev@example.com>
 Project-URL: Homepage, https://github.com/CameronRolfe/MazeGenerator
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 Requires-Dist: Pillow
```

### Comparing `CamsMazes-1.0.4/README.md` & `CamsMazes-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `CamsMazes-1.0.4/src/CamsMazes/maze.py` & `CamsMazes-1.0.5/src/CamsMazes/maze.py`

 * *Files identical despite different names*

### Comparing `CamsMazes-1.0.4/src/CamsMazes/maze_visualizer.py` & `CamsMazes-1.0.5/src/CamsMazes/maze_visualizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from tkinter import *
 import time
-from src.CamsMazes.maze import Maze
+from .maze import Maze
 
 class MazeVisualizer:
     class CellVisualizer:
         def __init__(self, canvas, cell_size):
             self.canvas = canvas
             self.cell_size = cell_size
             self.visited = False
```

### Comparing `CamsMazes-1.0.4/src/CamsMazes.egg-info/PKG-INFO` & `CamsMazes-1.0.5/src/CamsMazes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CamsMazes
-Version: 1.0.4
+Version: 1.0.5
 Summary: Maze Generator and Solver using DFS
 Author-email: Cameron Rolfe <cameronrolfedev@example.com>
 Project-URL: Homepage, https://github.com/CameronRolfe/MazeGenerator
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 Requires-Dist: Pillow
```

