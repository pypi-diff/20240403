# Comparing `tmp/CamsMazes-1.0.6.tar.gz` & `tmp/CamsMazes-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CamsMazes-1.0.6.tar", last modified: Wed Apr  3 19:11:22 2024, max compression
+gzip compressed data, was "CamsMazes-1.0.7.tar", last modified: Wed Apr  3 19:18:44 2024, max compression
```

## Comparing `CamsMazes-1.0.6.tar` & `CamsMazes-1.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 19:11:22.486562 CamsMazes-1.0.6/
--rw-rw-rw-   0        0        0     3215 2024-04-03 19:11:22.484562 CamsMazes-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2813 2024-04-03 19:10:52.000000 CamsMazes-1.0.6/README.md
--rw-rw-rw-   0        0        0      427 2024-04-03 19:11:05.000000 CamsMazes-1.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-03 19:11:22.486562 CamsMazes-1.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-03 19:11:22.458567 CamsMazes-1.0.6/src/
-drwxrwxrwx   0        0        0        0 2024-04-03 19:11:22.463567 CamsMazes-1.0.6/src/CamsMazes/
--rw-rw-rw-   0        0        0        0 2024-04-03 19:04:55.000000 CamsMazes-1.0.6/src/CamsMazes/__init__.py
--rw-rw-rw-   0        0        0    12405 2024-04-03 19:04:58.000000 CamsMazes-1.0.6/src/CamsMazes/maze.py
--rw-rw-rw-   0        0        0     3546 2024-04-03 19:03:20.000000 CamsMazes-1.0.6/src/CamsMazes/maze_visualizer.py
-drwxrwxrwx   0        0        0        0 2024-04-03 19:11:22.483562 CamsMazes-1.0.6/src/CamsMazes.egg-info/
--rw-rw-rw-   0        0        0     3215 2024-04-03 19:11:22.000000 CamsMazes-1.0.6/src/CamsMazes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      289 2024-04-03 19:11:22.000000 CamsMazes-1.0.6/src/CamsMazes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 19:11:22.000000 CamsMazes-1.0.6/src/CamsMazes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-03 19:11:22.000000 CamsMazes-1.0.6/src/CamsMazes.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-03 19:11:22.000000 CamsMazes-1.0.6/src/CamsMazes.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 19:18:44.717388 CamsMazes-1.0.7/
+-rw-rw-rw-   0        0        0     3413 2024-04-03 19:18:44.716389 CamsMazes-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3011 2024-04-03 19:17:18.000000 CamsMazes-1.0.7/README.md
+-rw-rw-rw-   0        0        0      427 2024-04-03 19:18:31.000000 CamsMazes-1.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-03 19:18:44.717388 CamsMazes-1.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-03 19:18:44.690389 CamsMazes-1.0.7/src/
+drwxrwxrwx   0        0        0        0 2024-04-03 19:18:44.694392 CamsMazes-1.0.7/src/CamsMazes/
+-rw-rw-rw-   0        0        0        0 2024-04-03 19:04:55.000000 CamsMazes-1.0.7/src/CamsMazes/__init__.py
+-rw-rw-rw-   0        0        0    12405 2024-04-03 19:04:58.000000 CamsMazes-1.0.7/src/CamsMazes/maze.py
+-rw-rw-rw-   0        0        0     3546 2024-04-03 19:03:20.000000 CamsMazes-1.0.7/src/CamsMazes/maze_visualizer.py
+drwxrwxrwx   0        0        0        0 2024-04-03 19:18:44.715417 CamsMazes-1.0.7/src/CamsMazes.egg-info/
+-rw-rw-rw-   0        0        0     3413 2024-04-03 19:18:44.000000 CamsMazes-1.0.7/src/CamsMazes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2024-04-03 19:18:44.000000 CamsMazes-1.0.7/src/CamsMazes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 19:18:44.000000 CamsMazes-1.0.7/src/CamsMazes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-03 19:18:44.000000 CamsMazes-1.0.7/src/CamsMazes.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-03 19:18:44.000000 CamsMazes-1.0.7/src/CamsMazes.egg-info/top_level.txt
```

### Comparing `CamsMazes-1.0.6/PKG-INFO` & `CamsMazes-1.0.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,13 @@
-Metadata-Version: 2.1
-Name: CamsMazes
-Version: 1.0.6
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
 
 ## Install
+[CamsMazes PyPi](https://pypi.org/project/CamsMazes/)
+
 ```
 pip install CamsMazes
 ```
 
 ## How to use Maze and MazeVisualizer
 Use Maze and MazeVisulizer to open a GUI to view maze generation
 ```python
@@ -41,57 +32,57 @@
 
 maze_visualizer3 = Maze(maze_3, cell_size=10, delay_ms=2) # Delay (in milliseconds) between each maze update during maze generation
 ```
 
 ## Exporting maze to image
 Use Maze.to_image to export maze to png
 ```python
-from src.Maze import Maze 
+from CamsMazes.maze import Maze
 maze = Maze(num_rows=40, num_cols=40)
 maze.to_img(file_name="maze") # Creates maze.png
 maze.to_img(file_name="maze_solution", solution=True) # Creates maze_solution.png (Image contains solution)
 maze.to_img(file_name="maze_2", cell_size=10) # Creates maze_2.png where each cell is 10 pixels by 10 pixels
 ```
 
 ## Exporting maze generation to gif
 Use Maze.to_gif to export maze generation to gif
 ```python
-from src.Maze import Maze
+from CamsMazes.maze import Maze
 maze = Maze(num_rows=40, num_cols=40)
 maze.to_gif(file_name="maze") # Creates maze.gif
 maze.to_gif(file_name="maze_2", cell_size=10) # Creates maze_2.gif where each cell is 10 pixels by 10 pixels
 ```
 
 ## Exporting maze to txt file
 Use Maze.to_txt to export maze to txt
 ```python
-from src.Maze import Maze
+from CamsMazes.maze import Maze
 maze = Maze(num_rows=40, num_cols=40)
 maze.to_txt() # Creates maze.txt
 maze.to_txt(file_name="maze_2") # file_name can be supplied (maze_2.txt is created)
 maze.to_txt(solution=True) # Populates txt with solution
 ```
 
 ## Exporting maze to JSON
 Use Maze.to_json to export maze to JSON. 
 
 See [to_json()](docs/Maze.md#to_json) for JSON format
 ```python
-from src.Maze import Maze
+from CamsMazes.maze import Maze
 maze = Maze(num_rows=40, num_cols=40)
 json = maze.to_json()
 ```
 
 ## Printing maze to console
 Use Maze.print to print maze to console
 ```python
-from src.Maze import Maze
+from CamsMazes.maze import Maze
 maze = Maze(num_rows=40, num_cols=40)
 maze.print()
 maze.print(show_solution=True) # Maze Text will include solution path
 ```
 
-# [Maze](docs/Maze.md)
+# [Maze](https://github.com/CameronRolfe/MazeGenerator/blob/main/docs/Maze.md)
 Exhaustive documentation for Maze
 
-# [MazeVisualizer](docs/MazeVisualizer.md)
-Exhaustive documentation for MazeVisualizer
+# [MazeVisualizer](https://github.com/CameronRolfe/MazeGenerator/blob/main/docs/MazeVisualizer.md)
+Exhaustive documentation for MazeVisualizer
```

### Comparing `CamsMazes-1.0.6/README.md` & `CamsMazes-1.0.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,24 @@
+Metadata-Version: 2.1
+Name: CamsMazes
+Version: 1.0.7
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
 
 ## Install
+[CamsMazes PyPi](https://pypi.org/project/CamsMazes/)
+
 ```
 pip install CamsMazes
 ```
 
 ## How to use Maze and MazeVisualizer
 Use Maze and MazeVisulizer to open a GUI to view maze generation
 ```python
@@ -30,57 +43,57 @@
 
 maze_visualizer3 = Maze(maze_3, cell_size=10, delay_ms=2) # Delay (in milliseconds) between each maze update during maze generation
 ```
 
 ## Exporting maze to image
 Use Maze.to_image to export maze to png
 ```python
-from src.Maze import Maze 
+from CamsMazes.maze import Maze
 maze = Maze(num_rows=40, num_cols=40)
 maze.to_img(file_name="maze") # Creates maze.png
 maze.to_img(file_name="maze_solution", solution=True) # Creates maze_solution.png (Image contains solution)
 maze.to_img(file_name="maze_2", cell_size=10) # Creates maze_2.png where each cell is 10 pixels by 10 pixels
 ```
 
 ## Exporting maze generation to gif
 Use Maze.to_gif to export maze generation to gif
 ```python
-from src.Maze import Maze
+from CamsMazes.maze import Maze
 maze = Maze(num_rows=40, num_cols=40)
 maze.to_gif(file_name="maze") # Creates maze.gif
 maze.to_gif(file_name="maze_2", cell_size=10) # Creates maze_2.gif where each cell is 10 pixels by 10 pixels
 ```
 
 ## Exporting maze to txt file
 Use Maze.to_txt to export maze to txt
 ```python
-from src.Maze import Maze
+from CamsMazes.maze import Maze
 maze = Maze(num_rows=40, num_cols=40)
 maze.to_txt() # Creates maze.txt
 maze.to_txt(file_name="maze_2") # file_name can be supplied (maze_2.txt is created)
 maze.to_txt(solution=True) # Populates txt with solution
 ```
 
 ## Exporting maze to JSON
 Use Maze.to_json to export maze to JSON. 
 
 See [to_json()](docs/Maze.md#to_json) for JSON format
 ```python
-from src.Maze import Maze
+from CamsMazes.maze import Maze
 maze = Maze(num_rows=40, num_cols=40)
 json = maze.to_json()
 ```
 
 ## Printing maze to console
 Use Maze.print to print maze to console
 ```python
-from src.Maze import Maze
+from CamsMazes.maze import Maze
 maze = Maze(num_rows=40, num_cols=40)
 maze.print()
 maze.print(show_solution=True) # Maze Text will include solution path
 ```
 
-# [Maze](docs/Maze.md)
+# [Maze](https://github.com/CameronRolfe/MazeGenerator/blob/main/docs/Maze.md)
 Exhaustive documentation for Maze
 
-# [MazeVisualizer](docs/MazeVisualizer.md)
-Exhaustive documentation for MazeVisualizer
+# [MazeVisualizer](https://github.com/CameronRolfe/MazeGenerator/blob/main/docs/MazeVisualizer.md)
+Exhaustive documentation for MazeVisualizer
```

### Comparing `CamsMazes-1.0.6/src/CamsMazes/maze.py` & `CamsMazes-1.0.7/src/CamsMazes/maze.py`

 * *Files identical despite different names*

### Comparing `CamsMazes-1.0.6/src/CamsMazes/maze_visualizer.py` & `CamsMazes-1.0.7/src/CamsMazes/maze_visualizer.py`

 * *Files identical despite different names*

### Comparing `CamsMazes-1.0.6/src/CamsMazes.egg-info/PKG-INFO` & `CamsMazes-1.0.7/src/CamsMazes.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: CamsMazes
-Version: 1.0.6
+Version: 1.0.7
 Summary: Maze Generator and Solver using DFS
 Author-email: Cameron Rolfe <cameronrolfedev@example.com>
 Project-URL: Homepage, https://github.com/CameronRolfe/MazeGenerator
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 Requires-Dist: Pillow
 
 # About Project
 Maze Generator and Solver built with Python
 
 ## Install
+[CamsMazes PyPi](https://pypi.org/project/CamsMazes/)
+
 ```
 pip install CamsMazes
 ```
 
 ## How to use Maze and MazeVisualizer
 Use Maze and MazeVisulizer to open a GUI to view maze generation
 ```python
@@ -41,57 +43,57 @@
 
 maze_visualizer3 = Maze(maze_3, cell_size=10, delay_ms=2) # Delay (in milliseconds) between each maze update during maze generation
 ```
 
 ## Exporting maze to image
 Use Maze.to_image to export maze to png
 ```python
-from src.Maze import Maze 
+from CamsMazes.maze import Maze
 maze = Maze(num_rows=40, num_cols=40)
 maze.to_img(file_name="maze") # Creates maze.png
 maze.to_img(file_name="maze_solution", solution=True) # Creates maze_solution.png (Image contains solution)
 maze.to_img(file_name="maze_2", cell_size=10) # Creates maze_2.png where each cell is 10 pixels by 10 pixels
 ```
 
 ## Exporting maze generation to gif
 Use Maze.to_gif to export maze generation to gif
 ```python
-from src.Maze import Maze
+from CamsMazes.maze import Maze
 maze = Maze(num_rows=40, num_cols=40)
 maze.to_gif(file_name="maze") # Creates maze.gif
 maze.to_gif(file_name="maze_2", cell_size=10) # Creates maze_2.gif where each cell is 10 pixels by 10 pixels
 ```
 
 ## Exporting maze to txt file
 Use Maze.to_txt to export maze to txt
 ```python
-from src.Maze import Maze
+from CamsMazes.maze import Maze
 maze = Maze(num_rows=40, num_cols=40)
 maze.to_txt() # Creates maze.txt
 maze.to_txt(file_name="maze_2") # file_name can be supplied (maze_2.txt is created)
 maze.to_txt(solution=True) # Populates txt with solution
 ```
 
 ## Exporting maze to JSON
 Use Maze.to_json to export maze to JSON. 
 
 See [to_json()](docs/Maze.md#to_json) for JSON format
 ```python
-from src.Maze import Maze
+from CamsMazes.maze import Maze
 maze = Maze(num_rows=40, num_cols=40)
 json = maze.to_json()
 ```
 
 ## Printing maze to console
 Use Maze.print to print maze to console
 ```python
-from src.Maze import Maze
+from CamsMazes.maze import Maze
 maze = Maze(num_rows=40, num_cols=40)
 maze.print()
 maze.print(show_solution=True) # Maze Text will include solution path
 ```
 
-# [Maze](docs/Maze.md)
+# [Maze](https://github.com/CameronRolfe/MazeGenerator/blob/main/docs/Maze.md)
 Exhaustive documentation for Maze
 
-# [MazeVisualizer](docs/MazeVisualizer.md)
+# [MazeVisualizer](https://github.com/CameronRolfe/MazeGenerator/blob/main/docs/MazeVisualizer.md)
 Exhaustive documentation for MazeVisualizer
```

