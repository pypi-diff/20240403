# Comparing `tmp/CamsMazes-1.0.5.tar.gz` & `tmp/CamsMazes-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CamsMazes-1.0.5.tar", last modified: Wed Apr  3 18:55:45 2024, max compression
+gzip compressed data, was "CamsMazes-1.0.6.tar", last modified: Wed Apr  3 19:11:22 2024, max compression
```

## Comparing `CamsMazes-1.0.5.tar` & `CamsMazes-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 18:55:45.337355 CamsMazes-1.0.5/
--rw-rw-rw-   0        0        0     3480 2024-04-03 18:55:45.336318 CamsMazes-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3078 2024-04-03 15:18:03.000000 CamsMazes-1.0.5/README.md
--rw-rw-rw-   0        0        0      427 2024-04-03 18:53:53.000000 CamsMazes-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-03 18:55:45.337355 CamsMazes-1.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-03 18:55:45.303310 CamsMazes-1.0.5/src/
-drwxrwxrwx   0        0        0        0 2024-04-03 18:55:45.316351 CamsMazes-1.0.5/src/CamsMazes/
--rw-rw-rw-   0        0        0        0 2024-04-03 18:44:45.000000 CamsMazes-1.0.5/src/CamsMazes/__init__.py
--rw-rw-rw-   0        0        0    12405 2024-04-03 18:55:28.000000 CamsMazes-1.0.5/src/CamsMazes/maze.py
--rw-rw-rw-   0        0        0     3522 2024-04-03 18:55:30.000000 CamsMazes-1.0.5/src/CamsMazes/maze_visualizer.py
-drwxrwxrwx   0        0        0        0 2024-04-03 18:55:45.335395 CamsMazes-1.0.5/src/CamsMazes.egg-info/
--rw-rw-rw-   0        0        0     3480 2024-04-03 18:55:45.000000 CamsMazes-1.0.5/src/CamsMazes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      289 2024-04-03 18:55:45.000000 CamsMazes-1.0.5/src/CamsMazes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 18:55:45.000000 CamsMazes-1.0.5/src/CamsMazes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-03 18:55:45.000000 CamsMazes-1.0.5/src/CamsMazes.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-03 18:55:45.000000 CamsMazes-1.0.5/src/CamsMazes.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 19:11:22.486562 CamsMazes-1.0.6/
+-rw-rw-rw-   0        0        0     3215 2024-04-03 19:11:22.484562 CamsMazes-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2813 2024-04-03 19:10:52.000000 CamsMazes-1.0.6/README.md
+-rw-rw-rw-   0        0        0      427 2024-04-03 19:11:05.000000 CamsMazes-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-03 19:11:22.486562 CamsMazes-1.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-03 19:11:22.458567 CamsMazes-1.0.6/src/
+drwxrwxrwx   0        0        0        0 2024-04-03 19:11:22.463567 CamsMazes-1.0.6/src/CamsMazes/
+-rw-rw-rw-   0        0        0        0 2024-04-03 19:04:55.000000 CamsMazes-1.0.6/src/CamsMazes/__init__.py
+-rw-rw-rw-   0        0        0    12405 2024-04-03 19:04:58.000000 CamsMazes-1.0.6/src/CamsMazes/maze.py
+-rw-rw-rw-   0        0        0     3546 2024-04-03 19:03:20.000000 CamsMazes-1.0.6/src/CamsMazes/maze_visualizer.py
+drwxrwxrwx   0        0        0        0 2024-04-03 19:11:22.483562 CamsMazes-1.0.6/src/CamsMazes.egg-info/
+-rw-rw-rw-   0        0        0     3215 2024-04-03 19:11:22.000000 CamsMazes-1.0.6/src/CamsMazes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2024-04-03 19:11:22.000000 CamsMazes-1.0.6/src/CamsMazes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 19:11:22.000000 CamsMazes-1.0.6/src/CamsMazes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-03 19:11:22.000000 CamsMazes-1.0.6/src/CamsMazes.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-03 19:11:22.000000 CamsMazes-1.0.6/src/CamsMazes.egg-info/top_level.txt
```

### Comparing `CamsMazes-1.0.5/PKG-INFO` & `CamsMazes-1.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,31 @@
 Metadata-Version: 2.1
 Name: CamsMazes
-Version: 1.0.5
+Version: 1.0.6
 Summary: Maze Generator and Solver using DFS
 Author-email: Cameron Rolfe <cameronrolfedev@example.com>
 Project-URL: Homepage, https://github.com/CameronRolfe/MazeGenerator
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 Requires-Dist: Pillow
 
 # About Project
 Maze Generator and Solver built with Python
 
-## Install Requirements
-Currently, there is only one requirement for the project and that is the [Pillow](https://pypi.org/project/pillow/) library.
-
-Install the requirements using one of the following commands
-
+## Install
 ```
-Option #1
-pip install -r requirements.txt
-
-Option #2
-py -m pip install -r requirements.txt
+pip install CamsMazes
 ```
 
 ## How to use Maze and MazeVisualizer
 Use Maze and MazeVisulizer to open a GUI to view maze generation
 ```python
-from src.Maze import Maze
-from src.MazeVisualizer import MazeVisualizer
+from CamsMazes.maze import Maze
+from CamsMazes.maze_visaulizer import MazeVisualizer
 
 # How to use Maze
 
 # Create Maze with minimum arguments
 maze = Maze(num_rows=40, num_cols=40)
 # Starts generatring maze at (5, 10). End cell is set to (25, 15)
 maze_2 = Maze(num_rows=60, num_cols=40, start_row=5, start_col=10, end_row=25, end_col=15)
```

### Comparing `CamsMazes-1.0.5/README.md` & `CamsMazes-1.0.6/src/CamsMazes.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,31 @@
+Metadata-Version: 2.1
+Name: CamsMazes
+Version: 1.0.6
+Summary: Maze Generator and Solver using DFS
+Author-email: Cameron Rolfe <cameronrolfedev@example.com>
+Project-URL: Homepage, https://github.com/CameronRolfe/MazeGenerator
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
+Requires-Dist: Pillow
+
 # About Project
 Maze Generator and Solver built with Python
 
-## Install Requirements
-Currently, there is only one requirement for the project and that is the [Pillow](https://pypi.org/project/pillow/) library.
-
-Install the requirements using one of the following commands
-
+## Install
 ```
-Option #1
-pip install -r requirements.txt
-
-Option #2
-py -m pip install -r requirements.txt
+pip install CamsMazes
 ```
 
 ## How to use Maze and MazeVisualizer
 Use Maze and MazeVisulizer to open a GUI to view maze generation
 ```python
-from src.Maze import Maze
-from src.MazeVisualizer import MazeVisualizer
+from CamsMazes.maze import Maze
+from CamsMazes.maze_visaulizer import MazeVisualizer
 
 # How to use Maze
 
 # Create Maze with minimum arguments
 maze = Maze(num_rows=40, num_cols=40)
 # Starts generatring maze at (5, 10). End cell is set to (25, 15)
 maze_2 = Maze(num_rows=60, num_cols=40, start_row=5, start_col=10, end_row=25, end_col=15) 
@@ -87,8 +90,8 @@
 maze.print(show_solution=True) # Maze Text will include solution path
 ```
 
 # [Maze](docs/Maze.md)
 Exhaustive documentation for Maze
 
 # [MazeVisualizer](docs/MazeVisualizer.md)
-Exhaustive documentation for MazeVisualizer
+Exhaustive documentation for MazeVisualizer
```

### Comparing `CamsMazes-1.0.5/src/CamsMazes/maze.py` & `CamsMazes-1.0.6/src/CamsMazes/maze.py`

 * *Files identical despite different names*

### Comparing `CamsMazes-1.0.5/src/CamsMazes/maze_visualizer.py` & `CamsMazes-1.0.6/src/CamsMazes/maze_visualizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from tkinter import *
 import time
-from .maze import Maze
+#from .maze import Maze
+from maze import Maze
 
 class MazeVisualizer:
     class CellVisualizer:
         def __init__(self, canvas, cell_size):
             self.canvas = canvas
             self.cell_size = cell_size
             self.visited = False
```

### Comparing `CamsMazes-1.0.5/src/CamsMazes.egg-info/PKG-INFO` & `CamsMazes-1.0.6/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,20 @@
-Metadata-Version: 2.1
-Name: CamsMazes
-Version: 1.0.5
-Summary: Maze Generator and Solver using DFS
-Author-email: Cameron Rolfe <cameronrolfedev@example.com>
-Project-URL: Homepage, https://github.com/CameronRolfe/MazeGenerator
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-Requires-Dist: Pillow
-
 # About Project
 Maze Generator and Solver built with Python
 
-## Install Requirements
-Currently, there is only one requirement for the project and that is the [Pillow](https://pypi.org/project/pillow/) library.
-
-Install the requirements using one of the following commands
-
+## Install
 ```
-Option #1
-pip install -r requirements.txt
-
-Option #2
-py -m pip install -r requirements.txt
+pip install CamsMazes
 ```
 
 ## How to use Maze and MazeVisualizer
 Use Maze and MazeVisulizer to open a GUI to view maze generation
 ```python
-from src.Maze import Maze
-from src.MazeVisualizer import MazeVisualizer
+from CamsMazes.maze import Maze
+from CamsMazes.maze_visaulizer import MazeVisualizer
 
 # How to use Maze
 
 # Create Maze with minimum arguments
 maze = Maze(num_rows=40, num_cols=40)
 # Starts generatring maze at (5, 10). End cell is set to (25, 15)
 maze_2 = Maze(num_rows=60, num_cols=40, start_row=5, start_col=10, end_row=25, end_col=15) 
@@ -98,8 +79,8 @@
 maze.print(show_solution=True) # Maze Text will include solution path
 ```
 
 # [Maze](docs/Maze.md)
 Exhaustive documentation for Maze
 
 # [MazeVisualizer](docs/MazeVisualizer.md)
-Exhaustive documentation for MazeVisualizer
+Exhaustive documentation for MazeVisualizer
```

