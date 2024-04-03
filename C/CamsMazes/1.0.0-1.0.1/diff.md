# Comparing `tmp/CamsMazes-1.0.0.tar.gz` & `tmp/CamsMazes-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CamsMazes-1.0.0.tar", last modified: Wed Apr  3 16:27:29 2024, max compression
+gzip compressed data, was "CamsMazes-1.0.1.tar", last modified: Wed Apr  3 16:37:03 2024, max compression
```

## Comparing `CamsMazes-1.0.0.tar` & `CamsMazes-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 16:27:29.637013 CamsMazes-1.0.0/
--rw-rw-rw-   0        0        0     3480 2024-04-03 16:27:29.635074 CamsMazes-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3078 2024-04-03 15:18:03.000000 CamsMazes-1.0.0/README.md
--rw-rw-rw-   0        0        0      427 2024-04-03 16:27:19.000000 CamsMazes-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-03 16:27:29.638014 CamsMazes-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-03 16:27:29.606914 CamsMazes-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-03 16:27:29.633063 CamsMazes-1.0.0/src/CamsMazes.egg-info/
--rw-rw-rw-   0        0        0     3480 2024-04-03 16:27:29.000000 CamsMazes-1.0.0/src/CamsMazes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2024-04-03 16:27:29.000000 CamsMazes-1.0.0/src/CamsMazes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 16:27:29.000000 CamsMazes-1.0.0/src/CamsMazes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-03 16:27:29.000000 CamsMazes-1.0.0/src/CamsMazes.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-03 16:27:29.000000 CamsMazes-1.0.0/src/CamsMazes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    12405 2024-04-03 15:07:44.000000 CamsMazes-1.0.0/src/Maze.py
--rw-rw-rw-   0        0        0     3523 2024-04-03 01:26:16.000000 CamsMazes-1.0.0/src/MazeVisualizer.py
+drwxrwxrwx   0        0        0        0 2024-04-03 16:37:03.538463 CamsMazes-1.0.1/
+-rw-rw-rw-   0        0        0     3480 2024-04-03 16:37:03.536465 CamsMazes-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3078 2024-04-03 15:18:03.000000 CamsMazes-1.0.1/README.md
+-rw-rw-rw-   0        0        0      427 2024-04-03 16:36:52.000000 CamsMazes-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-03 16:37:03.539464 CamsMazes-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-03 16:37:03.498941 CamsMazes-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-03 16:37:03.503933 CamsMazes-1.0.1/src/CamsMazes/
+-rw-rw-rw-   0        0        0    12405 2024-04-03 15:07:44.000000 CamsMazes-1.0.1/src/CamsMazes/Maze.py
+-rw-rw-rw-   0        0        0     3523 2024-04-03 01:26:16.000000 CamsMazes-1.0.1/src/CamsMazes/MazeVisualizer.py
+drwxrwxrwx   0        0        0        0 2024-04-03 16:37:03.533457 CamsMazes-1.0.1/src/CamsMazes.egg-info/
+-rw-rw-rw-   0        0        0     3480 2024-04-03 16:37:03.000000 CamsMazes-1.0.1/src/CamsMazes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2024-04-03 16:37:03.000000 CamsMazes-1.0.1/src/CamsMazes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 16:37:03.000000 CamsMazes-1.0.1/src/CamsMazes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-03 16:37:03.000000 CamsMazes-1.0.1/src/CamsMazes.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-03 16:37:03.000000 CamsMazes-1.0.1/src/CamsMazes.egg-info/top_level.txt
```

### Comparing `CamsMazes-1.0.0/PKG-INFO` & `CamsMazes-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CamsMazes
-Version: 1.0.0
+Version: 1.0.1
 Summary: Maze Generator and Solver using DFS
 Author-email: Cameron Rolfe <cameronrolfedev@example.com>
 Project-URL: Homepage, https://github.com/CameronRolfe/MazeGenerator
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 Requires-Dist: Pillow
```

### Comparing `CamsMazes-1.0.0/README.md` & `CamsMazes-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `CamsMazes-1.0.0/src/CamsMazes.egg-info/PKG-INFO` & `CamsMazes-1.0.1/src/CamsMazes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CamsMazes
-Version: 1.0.0
+Version: 1.0.1
 Summary: Maze Generator and Solver using DFS
 Author-email: Cameron Rolfe <cameronrolfedev@example.com>
 Project-URL: Homepage, https://github.com/CameronRolfe/MazeGenerator
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 Requires-Dist: Pillow
```

### Comparing `CamsMazes-1.0.0/src/Maze.py` & `CamsMazes-1.0.1/src/CamsMazes/Maze.py`

 * *Files identical despite different names*

### Comparing `CamsMazes-1.0.0/src/MazeVisualizer.py` & `CamsMazes-1.0.1/src/CamsMazes/MazeVisualizer.py`

 * *Files identical despite different names*

