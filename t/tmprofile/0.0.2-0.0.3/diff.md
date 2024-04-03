# Comparing `tmp/tmprofile-0.0.2.tar.gz` & `tmp/tmprofile-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmprofile-0.0.2.tar", last modified: Wed Apr  3 14:28:34 2024, max compression
+gzip compressed data, was "tmprofile-0.0.3.tar", last modified: Wed Apr  3 15:14:02 2024, max compression
```

## Comparing `tmprofile-0.0.2.tar` & `tmprofile-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 vedrenne (271197) images    (7000)        0 2024-04-03 14:28:34.381188 tmprofile-0.0.2/
--rw-r--r--   0 vedrenne (271197) images    (7000)     1074 2024-04-03 14:04:43.000000 tmprofile-0.0.2/LICENSE
--rw-r--r--   0 vedrenne (271197) images    (7000)     2180 2024-04-03 14:28:34.381188 tmprofile-0.0.2/PKG-INFO
--rw-r--r--   0 vedrenne (271197) images    (7000)     1518 2024-04-03 14:18:13.000000 tmprofile-0.0.2/README.md
--rw-r--r--   0 vedrenne (271197) images    (7000)      835 2024-04-03 14:17:45.000000 tmprofile-0.0.2/pyproject.toml
--rw-r--r--   0 vedrenne (271197) images    (7000)       38 2024-04-03 14:28:34.381188 tmprofile-0.0.2/setup.cfg
-drwxr-xr-x   0 vedrenne (271197) images    (7000)        0 2024-04-03 14:28:34.381188 tmprofile-0.0.2/tmprofile/
--rw-r--r--   0 vedrenne (271197) images    (7000)       40 2024-04-03 14:04:17.000000 tmprofile-0.0.2/tmprofile/__init__.py
--rw-r--r--   0 vedrenne (271197) images    (7000)    12251 2024-04-03 14:24:48.000000 tmprofile-0.0.2/tmprofile/pyprofile.py
-drwxr-xr-x   0 vedrenne (271197) images    (7000)        0 2024-04-03 14:28:34.381188 tmprofile-0.0.2/tmprofile.egg-info/
--rw-r--r--   0 vedrenne (271197) images    (7000)     2180 2024-04-03 14:28:34.000000 tmprofile-0.0.2/tmprofile.egg-info/PKG-INFO
--rw-r--r--   0 vedrenne (271197) images    (7000)      241 2024-04-03 14:28:34.000000 tmprofile-0.0.2/tmprofile.egg-info/SOURCES.txt
--rw-r--r--   0 vedrenne (271197) images    (7000)        1 2024-04-03 14:28:34.000000 tmprofile-0.0.2/tmprofile.egg-info/dependency_links.txt
--rw-r--r--   0 vedrenne (271197) images    (7000)       50 2024-04-03 14:28:34.000000 tmprofile-0.0.2/tmprofile.egg-info/requires.txt
--rw-r--r--   0 vedrenne (271197) images    (7000)       10 2024-04-03 14:28:34.000000 tmprofile-0.0.2/tmprofile.egg-info/top_level.txt
+drwxr-xr-x   0 vedrenne (271197) images    (7000)        0 2024-04-03 15:14:02.596050 tmprofile-0.0.3/
+-rw-r--r--   0 vedrenne (271197) images    (7000)     1074 2024-04-03 14:04:43.000000 tmprofile-0.0.3/LICENSE
+-rw-r--r--   0 vedrenne (271197) images    (7000)     2182 2024-04-03 15:14:02.596050 tmprofile-0.0.3/PKG-INFO
+-rw-r--r--   0 vedrenne (271197) images    (7000)     1520 2024-04-03 15:00:02.000000 tmprofile-0.0.3/README.md
+-rw-r--r--   0 vedrenne (271197) images    (7000)      835 2024-04-03 15:12:47.000000 tmprofile-0.0.3/pyproject.toml
+-rw-r--r--   0 vedrenne (271197) images    (7000)       38 2024-04-03 15:14:02.596050 tmprofile-0.0.3/setup.cfg
+drwxr-xr-x   0 vedrenne (271197) images    (7000)        0 2024-04-03 15:14:02.592050 tmprofile-0.0.3/tmprofile/
+-rw-r--r--   0 vedrenne (271197) images    (7000)       40 2024-04-03 14:04:17.000000 tmprofile-0.0.3/tmprofile/__init__.py
+-rw-r--r--   0 vedrenne (271197) images    (7000)    12259 2024-04-03 15:10:47.000000 tmprofile-0.0.3/tmprofile/pyprofile.py
+drwxr-xr-x   0 vedrenne (271197) images    (7000)        0 2024-04-03 15:14:02.596050 tmprofile-0.0.3/tmprofile.egg-info/
+-rw-r--r--   0 vedrenne (271197) images    (7000)     2182 2024-04-03 15:14:02.000000 tmprofile-0.0.3/tmprofile.egg-info/PKG-INFO
+-rw-r--r--   0 vedrenne (271197) images    (7000)      241 2024-04-03 15:14:02.000000 tmprofile-0.0.3/tmprofile.egg-info/SOURCES.txt
+-rw-r--r--   0 vedrenne (271197) images    (7000)        1 2024-04-03 15:14:02.000000 tmprofile-0.0.3/tmprofile.egg-info/dependency_links.txt
+-rw-r--r--   0 vedrenne (271197) images    (7000)       50 2024-04-03 15:14:02.000000 tmprofile-0.0.3/tmprofile.egg-info/requires.txt
+-rw-r--r--   0 vedrenne (271197) images    (7000)       10 2024-04-03 15:14:02.000000 tmprofile-0.0.3/tmprofile.egg-info/top_level.txt
```

### Comparing `tmprofile-0.0.2/LICENSE` & `tmprofile-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tmprofile-0.0.2/PKG-INFO` & `tmprofile-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmprofile
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple time, ram & vram python profiler.
 Author-email: Luc Vedrenne <vedrenneluc@gmail.com>
 Project-URL: Homepage, https://github.com/ListIndexOutOfRange/pyprofile
 Project-URL: Issues, https://github.com/ListIndexOutOfRange/pyprofile/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -51,15 +51,15 @@
 
 ## Parameters
 
 - `name (str)`: Name of the profiler. Will be used to name the saved file. Required for context manager. For decorator, will use fonction'name if no name is provided.
 - `verbose (bool)`: If True, will print logged values at the end of profiling (i.e. on exit as a context manager, on function's return as a decorator). Defaults to False.
 - `gpu_idx (int)`: Which gpu's VRAM consumption has to be monitored. Default to `0`.
 - `time_delta (float)`: Time to wait (in second) between two RAM / VRAM consumption logging. Defaults to `0.2`.
-- `output_dir (str | Path)`: Where to write the logged values (as json). Defaults to `.profile`.
+- `output_dir (str | Path)`: Where to write the logged values (as json). Defaults to `.tmprofile`.
 - `filename (str | Path, optional)`: Name of the saved json file. If no name is given, will used the profiler name (see `name` above).
 
 
 ## Disclaimer
 
 The core of this code (asynchronous RAM/VRAM logging) is taken from Thomas Rouch's code [here](https://betterprogramming.pub/ram-and-vram-profiling-in-python-bf99876e985f).
```

### Comparing `tmprofile-0.0.2/README.md` & `tmprofile-0.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 ## Parameters
 
 - `name (str)`: Name of the profiler. Will be used to name the saved file. Required for context manager. For decorator, will use fonction'name if no name is provided.
 - `verbose (bool)`: If True, will print logged values at the end of profiling (i.e. on exit as a context manager, on function's return as a decorator). Defaults to False.
 - `gpu_idx (int)`: Which gpu's VRAM consumption has to be monitored. Default to `0`.
 - `time_delta (float)`: Time to wait (in second) between two RAM / VRAM consumption logging. Defaults to `0.2`.
-- `output_dir (str | Path)`: Where to write the logged values (as json). Defaults to `.profile`.
+- `output_dir (str | Path)`: Where to write the logged values (as json). Defaults to `.tmprofile`.
 - `filename (str | Path, optional)`: Name of the saved json file. If no name is given, will used the profiler name (see `name` above).
 
 
 ## Disclaimer
 
 The core of this code (asynchronous RAM/VRAM logging) is taken from Thomas Rouch's code [here](https://betterprogramming.pub/ram-and-vram-profiling-in-python-bf99876e985f).
```

### Comparing `tmprofile-0.0.2/pyproject.toml` & `tmprofile-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "tmprofile"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Luc Vedrenne", email="vedrenneluc@gmail.com" },
 ]
 description = "A simple time, ram & vram python profiler."
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `tmprofile-0.0.2/tmprofile/pyprofile.py` & `tmprofile-0.0.3/tmprofile/pyprofile.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,28 +134,28 @@
 
     def __init__(
         self,
         name: str,
         verbose: bool = False,
         gpu_idx: int = 0,
         time_delta: float = 0.2,
-        output_dir: str | Path = '.profile',
+        output_dir: str | Path = '.tmprofile',
         filename: Optional[str | Path] = None
     ) -> None:
         """ Create a context usable as `with MemoryScope(name, ...) as profiler:`.
 
         Args:
             name (str): Name of the profiler. Will be used to name the saved file.
             verbose (bool, optional): If True, will print logged values on exit. Defaults to False.
             gpu_idx (int, optional): Which gpu's VRAM consumption has to be monitored.
                 Defaults to 0.
             time_delta (float, optional): Time to wait (in second) between two RAM / VRAM
                 consumption logging. Defaults to 0.2.
             output_dir (str | Path, optional): Directory in which to write the logged values
-                (as json). Defaults to '.profile'.
+                (as json). Defaults to '.tmprofile'.
             filename (str | Path, optional):Name of the saved json file. If no name is given, will
                 use the profiler name (see `name` above). Defaults to None.
         """
         self._stop_event = Event()
         self._monitor_process: Optional[Process] = None
         self._name = name
         self._verbose = verbose
@@ -268,15 +268,15 @@
 
 def profile(
     name: Optional[str] = None,
     *,
     verbose: bool = False,
     gpu_idx: int = 0,
     time_delta: float = 0.2,
-    output_dir: str | Path = '.profile',
+    output_dir: str | Path = '.tmprofile',
     filename: Optional[str | Path] = None
 ) -> FuncT:  # type: ignore
     """ A decorator to profile any function, e.g. :
 
     ```
     @profile(verbose=True)
     def f(...):
@@ -286,15 +286,15 @@
         name (str): Name of the profiler. Will be used to name the saved file.
         verbose (bool, optional): If True, will print logged values on exit. Defaults to False.
         gpu_idx (int, optional): Which gpu's VRAM consumption has to be monitored.
             Defaults to 0.
         time_delta (float, optional): Time to wait (in second) between two RAM / VRAM
             consumption logging. Defaults to 0.2.
         output_dir (str | Path, optional): Directory in which to write the logged values
-            (as json). Defaults to '.profile'.
+            (as json). Defaults to '.tmprofile'.
         name (str | Path, optional): Name of the saved json file. If no name is given, will use the
             decorated function's name and module as module::function_name. Defaults to None.
 
     Returns:
         FuncT: Function to be profiled.
     """
     def profile_inner(func: FuncT) -> FuncT:
```

### Comparing `tmprofile-0.0.2/tmprofile.egg-info/PKG-INFO` & `tmprofile-0.0.3/tmprofile.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmprofile
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple time, ram & vram python profiler.
 Author-email: Luc Vedrenne <vedrenneluc@gmail.com>
 Project-URL: Homepage, https://github.com/ListIndexOutOfRange/pyprofile
 Project-URL: Issues, https://github.com/ListIndexOutOfRange/pyprofile/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -51,15 +51,15 @@
 
 ## Parameters
 
 - `name (str)`: Name of the profiler. Will be used to name the saved file. Required for context manager. For decorator, will use fonction'name if no name is provided.
 - `verbose (bool)`: If True, will print logged values at the end of profiling (i.e. on exit as a context manager, on function's return as a decorator). Defaults to False.
 - `gpu_idx (int)`: Which gpu's VRAM consumption has to be monitored. Default to `0`.
 - `time_delta (float)`: Time to wait (in second) between two RAM / VRAM consumption logging. Defaults to `0.2`.
-- `output_dir (str | Path)`: Where to write the logged values (as json). Defaults to `.profile`.
+- `output_dir (str | Path)`: Where to write the logged values (as json). Defaults to `.tmprofile`.
 - `filename (str | Path, optional)`: Name of the saved json file. If no name is given, will used the profiler name (see `name` above).
 
 
 ## Disclaimer
 
 The core of this code (asynchronous RAM/VRAM logging) is taken from Thomas Rouch's code [here](https://betterprogramming.pub/ram-and-vram-profiling-in-python-bf99876e985f).
```

