# Comparing `tmp/tmprofile-0.0.3.tar.gz` & `tmp/tmprofile-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmprofile-0.0.3.tar", last modified: Wed Apr  3 15:14:02 2024, max compression
+gzip compressed data, was "tmprofile-0.0.4.tar", last modified: Wed Apr  3 16:15:13 2024, max compression
```

## Comparing `tmprofile-0.0.3.tar` & `tmprofile-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 vedrenne (271197) images    (7000)        0 2024-04-03 15:14:02.596050 tmprofile-0.0.3/
--rw-r--r--   0 vedrenne (271197) images    (7000)     1074 2024-04-03 14:04:43.000000 tmprofile-0.0.3/LICENSE
--rw-r--r--   0 vedrenne (271197) images    (7000)     2182 2024-04-03 15:14:02.596050 tmprofile-0.0.3/PKG-INFO
--rw-r--r--   0 vedrenne (271197) images    (7000)     1520 2024-04-03 15:00:02.000000 tmprofile-0.0.3/README.md
--rw-r--r--   0 vedrenne (271197) images    (7000)      835 2024-04-03 15:12:47.000000 tmprofile-0.0.3/pyproject.toml
--rw-r--r--   0 vedrenne (271197) images    (7000)       38 2024-04-03 15:14:02.596050 tmprofile-0.0.3/setup.cfg
-drwxr-xr-x   0 vedrenne (271197) images    (7000)        0 2024-04-03 15:14:02.592050 tmprofile-0.0.3/tmprofile/
--rw-r--r--   0 vedrenne (271197) images    (7000)       40 2024-04-03 14:04:17.000000 tmprofile-0.0.3/tmprofile/__init__.py
--rw-r--r--   0 vedrenne (271197) images    (7000)    12259 2024-04-03 15:10:47.000000 tmprofile-0.0.3/tmprofile/pyprofile.py
-drwxr-xr-x   0 vedrenne (271197) images    (7000)        0 2024-04-03 15:14:02.596050 tmprofile-0.0.3/tmprofile.egg-info/
--rw-r--r--   0 vedrenne (271197) images    (7000)     2182 2024-04-03 15:14:02.000000 tmprofile-0.0.3/tmprofile.egg-info/PKG-INFO
--rw-r--r--   0 vedrenne (271197) images    (7000)      241 2024-04-03 15:14:02.000000 tmprofile-0.0.3/tmprofile.egg-info/SOURCES.txt
--rw-r--r--   0 vedrenne (271197) images    (7000)        1 2024-04-03 15:14:02.000000 tmprofile-0.0.3/tmprofile.egg-info/dependency_links.txt
--rw-r--r--   0 vedrenne (271197) images    (7000)       50 2024-04-03 15:14:02.000000 tmprofile-0.0.3/tmprofile.egg-info/requires.txt
--rw-r--r--   0 vedrenne (271197) images    (7000)       10 2024-04-03 15:14:02.000000 tmprofile-0.0.3/tmprofile.egg-info/top_level.txt
+drwxr-xr-x   0 vedrenne (271197) images    (7000)        0 2024-04-03 16:15:13.963051 tmprofile-0.0.4/
+-rw-r--r--   0 vedrenne (271197) images    (7000)     1074 2024-04-03 14:04:43.000000 tmprofile-0.0.4/LICENSE
+-rw-r--r--   0 vedrenne (271197) images    (7000)     2726 2024-04-03 16:15:13.963051 tmprofile-0.0.4/PKG-INFO
+-rw-r--r--   0 vedrenne (271197) images    (7000)     2064 2024-04-03 16:11:58.000000 tmprofile-0.0.4/README.md
+-rw-r--r--   0 vedrenne (271197) images    (7000)      835 2024-04-03 16:15:00.000000 tmprofile-0.0.4/pyproject.toml
+-rw-r--r--   0 vedrenne (271197) images    (7000)       38 2024-04-03 16:15:13.963051 tmprofile-0.0.4/setup.cfg
+drwxr-xr-x   0 vedrenne (271197) images    (7000)        0 2024-04-03 16:15:13.963051 tmprofile-0.0.4/tmprofile/
+-rw-r--r--   0 vedrenne (271197) images    (7000)       40 2024-04-03 14:04:17.000000 tmprofile-0.0.4/tmprofile/__init__.py
+-rw-r--r--   0 vedrenne (271197) images    (7000)    13140 2024-04-03 16:09:27.000000 tmprofile-0.0.4/tmprofile/pyprofile.py
+drwxr-xr-x   0 vedrenne (271197) images    (7000)        0 2024-04-03 16:15:13.963051 tmprofile-0.0.4/tmprofile.egg-info/
+-rw-r--r--   0 vedrenne (271197) images    (7000)     2726 2024-04-03 16:15:13.000000 tmprofile-0.0.4/tmprofile.egg-info/PKG-INFO
+-rw-r--r--   0 vedrenne (271197) images    (7000)      241 2024-04-03 16:15:13.000000 tmprofile-0.0.4/tmprofile.egg-info/SOURCES.txt
+-rw-r--r--   0 vedrenne (271197) images    (7000)        1 2024-04-03 16:15:13.000000 tmprofile-0.0.4/tmprofile.egg-info/dependency_links.txt
+-rw-r--r--   0 vedrenne (271197) images    (7000)       50 2024-04-03 16:15:13.000000 tmprofile-0.0.4/tmprofile.egg-info/requires.txt
+-rw-r--r--   0 vedrenne (271197) images    (7000)       10 2024-04-03 16:15:13.000000 tmprofile-0.0.4/tmprofile.egg-info/top_level.txt
```

### Comparing `tmprofile-0.0.3/LICENSE` & `tmprofile-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tmprofile-0.0.3/PKG-INFO` & `tmprofile-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmprofile
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple time, ram & vram python profiler.
 Author-email: Luc Vedrenne <vedrenneluc@gmail.com>
 Project-URL: Homepage, https://github.com/ListIndexOutOfRange/pyprofile
 Project-URL: Issues, https://github.com/ListIndexOutOfRange/pyprofile/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -47,21 +47,34 @@
 @profile()
 f(...) # some intensive code
 # profile is automatically saved as a json file.
 ```
 
 ## Parameters
 
-- `name (str)`: Name of the profiler. Will be used to name the saved file. Required for context manager. For decorator, will use fonction'name if no name is provided.
+- `name (str)`: Name of the profiler. Will be used to name the saved file. Required for context manager. For decorator, will use fonction' name if no name is provided.
 - `verbose (bool)`: If True, will print logged values at the end of profiling (i.e. on exit as a context manager, on function's return as a decorator). Defaults to False.
 - `gpu_idx (int)`: Which gpu's VRAM consumption has to be monitored. Default to `0`.
 - `time_delta (float)`: Time to wait (in second) between two RAM / VRAM consumption logging. Defaults to `0.2`.
 - `output_dir (str | Path)`: Where to write the logged values (as json). Defaults to `.tmprofile`.
 - `filename (str | Path, optional)`: Name of the saved json file. If no name is given, will used the profiler name (see `name` above).
 
 
+## Saved logs
+
+Each time it is called, the profiler will saved a file.         
+The filepath will be `<output_dir>/filename.json`. By default, `<output_dir>` is `.tmprofile/` and `<filename>` is:
+- `<name>.json` if `name` was specified.
+- `profile.json` if the profiler is a context manager and `name` was NOT specified.
+- `<module>::<function>.json` if the profiler is a decorator and `name` was NOT specified.
+
+
+## Interrupt
+
+Since this profiler runs in a separate process, it will gracefully shutdown if the main programm is interrupted. 
+
 ## Disclaimer
 
 The core of this code (asynchronous RAM/VRAM logging) is taken from Thomas Rouch's code [here](https://betterprogramming.pub/ram-and-vram-profiling-in-python-bf99876e985f).
```

### Comparing `tmprofile-0.0.3/README.md` & `tmprofile-0.0.4/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -28,21 +28,34 @@
 @profile()
 f(...) # some intensive code
 # profile is automatically saved as a json file.
 ```
 
 ## Parameters
 
-- `name (str)`: Name of the profiler. Will be used to name the saved file. Required for context manager. For decorator, will use fonction'name if no name is provided.
+- `name (str)`: Name of the profiler. Will be used to name the saved file. Required for context manager. For decorator, will use fonction' name if no name is provided.
 - `verbose (bool)`: If True, will print logged values at the end of profiling (i.e. on exit as a context manager, on function's return as a decorator). Defaults to False.
 - `gpu_idx (int)`: Which gpu's VRAM consumption has to be monitored. Default to `0`.
 - `time_delta (float)`: Time to wait (in second) between two RAM / VRAM consumption logging. Defaults to `0.2`.
 - `output_dir (str | Path)`: Where to write the logged values (as json). Defaults to `.tmprofile`.
 - `filename (str | Path, optional)`: Name of the saved json file. If no name is given, will used the profiler name (see `name` above).
 
 
+## Saved logs
+
+Each time it is called, the profiler will saved a file.         
+The filepath will be `<output_dir>/filename.json`. By default, `<output_dir>` is `.tmprofile/` and `<filename>` is:
+- `<name>.json` if `name` was specified.
+- `profile.json` if the profiler is a context manager and `name` was NOT specified.
+- `<module>::<function>.json` if the profiler is a decorator and `name` was NOT specified.
+
+
+## Interrupt
+
+Since this profiler runs in a separate process, it will gracefully shutdown if the main programm is interrupted. 
+
 ## Disclaimer
 
 The core of this code (asynchronous RAM/VRAM logging) is taken from Thomas Rouch's code [here](https://betterprogramming.pub/ram-and-vram-profiling-in-python-bf99876e985f).
```

### Comparing `tmprofile-0.0.3/pyproject.toml` & `tmprofile-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "tmprofile"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Luc Vedrenne", email="vedrenneluc@gmail.com" },
 ]
 description = "A simple time, ram & vram python profiler."
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `tmprofile-0.0.3/tmprofile/pyprofile.py` & `tmprofile-0.0.4/tmprofile/pyprofile.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
     https://betterprogramming.pub/ram-and-vram-profiling-in-python-bf99876e985f
 """
 from __future__ import annotations
 import os
 import re
 import time
 import json
+import signal
 import psutil
 import inspect
 from functools import wraps
 from pathlib import Path
 from datetime import timedelta
 from matplotlib import pyplot as plt
 from IPython import get_ipython  # type: ignore
@@ -21,15 +22,14 @@
 from prettytable import PrettyTable
 import numpy as np
 import nvidia_smi  # nvidia-ml-py3
 
 
 # __________________________________________ Utilities __________________________________________ #
 
-
 def alphanumeric_sort(iterable: Iterable[str | Path]) -> list[str]:
     """ Sort the given iterable in alphanumeric order, e.g. ['string1', 'string2', 'string10'].
 
     Args:
         iterable (Iterable[str]): Any iterable sequence of strings.
 
     Returns:
@@ -82,101 +82,132 @@
             return f"{float(number)/value:.2f}{symbol}{suffix}"
 
     return f"{number} B"
 
 
 # _______________________________________ parallel logger _______________________________________ #
 
+class GracefulInterruptHandler(object):
+
+    """ From https://gist.github.com/nonZero/2907502. """
+
+    def __init__(self, sig=signal.SIGINT):
+        self.sig = sig
+
+    def __enter__(self):
+        self.interrupted = False
+        self.released = False
+        self.original_handler = signal.getsignal(self.sig)
+        def handler(signum, frame):
+            self.release()
+            self.interrupted = True
+        signal.signal(self.sig, handler)
+        return self
+
+    def __exit__(self, type, value, tb):
+        self.release()
+
+    def release(self):
+        if self.released:
+            return False
+        signal.signal(self.sig, self.original_handler)
+        self.released = True
+        return True
+
+
 def _monitor(pid: int, stop_event: EventClass,
-             gpu_idx: int, time_delta: float, output_file: str | Path) -> None:
+             gpu_idx: int, time_delta: float, output_file: Path) -> None:
     """ Monitor Memory consumption in parallel to a given process (RAM and VRAM).
 
     Args:
         pid (int): ID of the Process to monitor
         stop_event (EventClass): Shared event triggered when the monitoring has to stop
         gpu_idx (int): Which gpu's VRAM consumption has to be monitored.
         time_delta (float): Time to wait between two RAM / VRAM consumption logging.
-        output_file (_type_): Where to write the logged values (as json).
+        output_file (Path): Where to write the logged values (as json).
     """
     # 1. prepare containers
     ram_pid_values = list()
     ram_values = list()
     vram_values = list()
     # 2. init NVIDIA GPU logger
     nvidia_smi.nvmlInit()
     handle = nvidia_smi.nvmlDeviceGetHandleByIndex(gpu_idx)
     # 3. get base values
     total_ram_value = get_total_ram_available_bytes()
     total_vram_value = int(nvidia_smi.nvmlDeviceGetMemoryInfo(handle).total)
     # 4. monitor
     tic = time.perf_counter()
-    while not stop_event.is_set():
-        ram_pid_values.append(get_pid_ram_used_bytes(pid))
-        ram_values.append(get_total_ram_used_bytes())
-        gpu_info = nvidia_smi.nvmlDeviceGetMemoryInfo(handle)
-        vram_values.append(gpu_info.used)
-        time.sleep(time_delta)  # in s
-    toc = time.perf_counter()
-    elapsed_time = toc - tic
-    # 5. shutdown NVIDIA GPU logger
-    nvidia_smi.nvmlShutdown()
-    # 6. save logged values
-    data = dict(ram=ram_values, ram_pid=ram_pid_values, vram=vram_values,
-                total_ram=total_ram_value, total_vram=total_vram_value,
-                elapsed_time=elapsed_time, time_delta=time_delta)
-    json_object = json.dumps(data, indent=4)
-    with open(output_file, "w") as outfile:
-        outfile.write(json_object)
+    def on_end():
+        toc = time.perf_counter()
+        elapsed_time = toc - tic
+        data = dict(ram=ram_values, ram_pid=ram_pid_values, vram=vram_values,
+                    total_ram=total_ram_value, total_vram=total_vram_value,
+                    elapsed_time=elapsed_time, time_delta=time_delta)
+        json_object = json.dumps(data, indent=4)
+        with open(output_file, "w") as outfile:
+            outfile.write(json_object)
+    with GracefulInterruptHandler() as h:
+        while not stop_event.is_set():
+            ram_pid_values.append(get_pid_ram_used_bytes(pid))
+            ram_values.append(get_total_ram_used_bytes())
+            gpu_info = nvidia_smi.nvmlDeviceGetMemoryInfo(handle)
+            vram_values.append(gpu_info.used)
+            time.sleep(time_delta)  # in s
+            if h.interrupted:
+                on_end()
+    on_end()
 
 
 # _______________________________________ Context manager _______________________________________ #
 
 class Profile:
 
     def __init__(
         self,
-        name: str,
+        name: str = 'profile',
         verbose: bool = False,
         gpu_idx: int = 0,
         time_delta: float = 0.2,
         output_dir: str | Path = '.tmprofile',
         filename: Optional[str | Path] = None
     ) -> None:
         """ Create a context usable as `with MemoryScope(name, ...) as profiler:`.
 
         Args:
-            name (str): Name of the profiler. Will be used to name the saved file.
+            name (str): Name of the profiler. Can be used to name the saved file.
+                Defaults to 'profile'.
             verbose (bool, optional): If True, will print logged values on exit. Defaults to False.
             gpu_idx (int, optional): Which gpu's VRAM consumption has to be monitored.
                 Defaults to 0.
             time_delta (float, optional): Time to wait (in second) between two RAM / VRAM
                 consumption logging. Defaults to 0.2.
             output_dir (str | Path, optional): Directory in which to write the logged values
                 (as json). Defaults to '.tmprofile'.
-            filename (str | Path, optional):Name of the saved json file. If no name is given, will
+            filename (str | Path, optional): Name of the saved json file. If no name is given, will
                 use the profiler name (see `name` above). Defaults to None.
         """
         self._stop_event = Event()
         self._monitor_process: Optional[Process] = None
         self._name = name
         self._verbose = verbose
         self._gpu_idx = gpu_idx
         self._time_delta = time_delta
         self._output_file = self._prepare_output(output_dir, filename)
 
     def get_run_idx(self, output_dir: Path) -> int:
-        runs = alphanumeric_sort(Path(output_dir).glob(f"run*_profile__{self._name}.json"))
+        runs = alphanumeric_sort(Path(output_dir).glob(f"run*_{self._name}.json"))
         if len(runs) == 0:
             return 1
         return int(Path(runs[-1]).stem.split('run')[1].split('_')[0]) + 1
 
     def _prepare_output(self, output_dir: str | Path, filename: Optional[str | Path]) -> Path:
         output_dir = Path(output_dir).resolve()
         output_dir.mkdir(exist_ok=True)
-        filename = filename if filename is not None else f'profile__{self._name}'
+        filename = filename if filename is not None else self._name
         filename = Path(Path(filename).stem).with_suffix('.json')  # works w/ or w/o extension
         if (output_dir / filename).exists():
             idx = self.get_run_idx(output_dir)
             filename = f'run{idx}_{filename.stem}'
             filename = Path(Path(filename).stem).with_suffix('.json')
         return output_dir / filename
 
@@ -279,24 +310,25 @@
 
     ```
     @profile(verbose=True)
     def f(...):
     ```
 
     Args:
-        name (str): Name of the profiler. Will be used to name the saved file.
+        name (str): Name of the profiler. Can be used to name the saved file.
+            Defaults to 'profile'.
         verbose (bool, optional): If True, will print logged values on exit. Defaults to False.
         gpu_idx (int, optional): Which gpu's VRAM consumption has to be monitored.
             Defaults to 0.
         time_delta (float, optional): Time to wait (in second) between two RAM / VRAM
             consumption logging. Defaults to 0.2.
         output_dir (str | Path, optional): Directory in which to write the logged values
             (as json). Defaults to '.tmprofile'.
-        name (str | Path, optional): Name of the saved json file. If no name is given, will use the
-            decorated function's name and module as module::function_name. Defaults to None.
+        filename (str | Path, optional): Name of the saved json file. If no name is given, will use
+            the decorated function's name and module as module::function_name. Defaults to None.
 
     Returns:
         FuncT: Function to be profiled.
     """
     def profile_inner(func: FuncT) -> FuncT:
         """ Time & Memory (RAM and VRAM) Profiling decorator. """
         @wraps(func)
```

### Comparing `tmprofile-0.0.3/tmprofile.egg-info/PKG-INFO` & `tmprofile-0.0.4/tmprofile.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmprofile
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple time, ram & vram python profiler.
 Author-email: Luc Vedrenne <vedrenneluc@gmail.com>
 Project-URL: Homepage, https://github.com/ListIndexOutOfRange/pyprofile
 Project-URL: Issues, https://github.com/ListIndexOutOfRange/pyprofile/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -47,21 +47,34 @@
 @profile()
 f(...) # some intensive code
 # profile is automatically saved as a json file.
 ```
 
 ## Parameters
 
-- `name (str)`: Name of the profiler. Will be used to name the saved file. Required for context manager. For decorator, will use fonction'name if no name is provided.
+- `name (str)`: Name of the profiler. Will be used to name the saved file. Required for context manager. For decorator, will use fonction' name if no name is provided.
 - `verbose (bool)`: If True, will print logged values at the end of profiling (i.e. on exit as a context manager, on function's return as a decorator). Defaults to False.
 - `gpu_idx (int)`: Which gpu's VRAM consumption has to be monitored. Default to `0`.
 - `time_delta (float)`: Time to wait (in second) between two RAM / VRAM consumption logging. Defaults to `0.2`.
 - `output_dir (str | Path)`: Where to write the logged values (as json). Defaults to `.tmprofile`.
 - `filename (str | Path, optional)`: Name of the saved json file. If no name is given, will used the profiler name (see `name` above).
 
 
+## Saved logs
+
+Each time it is called, the profiler will saved a file.         
+The filepath will be `<output_dir>/filename.json`. By default, `<output_dir>` is `.tmprofile/` and `<filename>` is:
+- `<name>.json` if `name` was specified.
+- `profile.json` if the profiler is a context manager and `name` was NOT specified.
+- `<module>::<function>.json` if the profiler is a decorator and `name` was NOT specified.
+
+
+## Interrupt
+
+Since this profiler runs in a separate process, it will gracefully shutdown if the main programm is interrupted. 
+
 ## Disclaimer
 
 The core of this code (asynchronous RAM/VRAM logging) is taken from Thomas Rouch's code [here](https://betterprogramming.pub/ram-and-vram-profiling-in-python-bf99876e985f).
```

