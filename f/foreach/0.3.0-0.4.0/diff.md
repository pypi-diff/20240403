# Comparing `tmp/foreach-0.3.0.tar.gz` & `tmp/foreach-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foreach-0.3.0.tar", max compression
+gzip compressed data, was "foreach-0.4.0.tar", max compression
```

## Comparing `foreach-0.3.0.tar` & `foreach-0.4.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1066 2023-12-08 19:35:21.402569 foreach-0.3.0/LICENSE
--rw-r--r--   0        0        0     1871 2024-01-20 04:56:39.844540 foreach-0.3.0/README.md
--rw-r--r--   0        0        0     1423 2024-01-20 04:52:52.604991 foreach-0.3.0/foreach/__init__.py
--rw-r--r--   0        0        0      338 2024-01-20 04:57:45.685577 foreach-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2394 1970-01-01 00:00:00.000000 foreach-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-12-08 19:35:21.402569 foreach-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1923 2024-04-03 19:37:08.834364 foreach-0.4.0/README.md
+-rw-r--r--   0        0        0     1599 2024-04-03 19:35:47.376755 foreach-0.4.0/foreach/__init__.py
+-rw-r--r--   0        0        0      338 2024-04-03 19:35:53.048867 foreach-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2446 1970-01-01 00:00:00.000000 foreach-0.4.0/PKG-INFO
```

### Comparing `foreach-0.3.0/LICENSE` & `foreach-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `foreach-0.3.0/README.md` & `foreach-0.4.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ```bash
 pip install foreach
 ```
 
 ## Usage
 
 ```python
-import foreach
+from foreach import foreach
 
 def square(x):
     return x**2
 
 params = [1, 2, 3, 4, 5]
 result = foreach(square, params)
 print(result)
@@ -43,30 +43,30 @@
 
 
 ## Examples
 
 ### Sequential Execution
 
 ```python
-import foreach
+from foreach import foreach
 
 def square(x):
     return x**2
 
 params = [1, 2, 3, 4, 5]
 result = foreach(square, params, parallel=False)
 print(result)
 # [1, 4, 9, 16, 25]
 ```
 
 
 ### Callback Functionality
 
 ```python
-import foreach
+from foreach import foreach
 
 def square(x):
     return x**2
 
 params = [1, 2, 3, 4, 5]
 
 def callback(x):
@@ -79,15 +79,15 @@
 # Processed: 16
 # Processed: 25
 ```
 
 ### Customizing Number of Processes
 
 ```python
-import foreach
+from foreach import foreach
 
 def square(x):
     return x**2
 
 params = [1, 2, 3, 4, 5]
 result = foreach(square, params, num_processes=2)
 print(result)
```

### Comparing `foreach-0.3.0/foreach/__init__.py` & `foreach-0.4.0/foreach/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,46 @@
 import sys
-from multiprocessing import Pool
-from typing import Callable, Iterable, List
+from multiprocessing import get_context
+from typing import Callable, Iterable, List, Literal, Optional
 
 from tqdm import tqdm
 
 
 def foreach(
     func: Callable,
     params: Iterable,
     parallel: bool = True,
-    processes: int = None,
-    callback: Callable = None,
+    processes: Optional[int] = None,
+    callback: Optional[Callable] = None,
+    context: Optional[Literal["fork", "spawn", "forkserver"]] = None,
 ) -> List:
     """
     Parallelly apply a given function to each element in the input iterable.
 
     Parameters:
     - func (Callable): The function to apply to each element.
     - params (Iterable): The iterable of parameters to apply the function to.
     - parallel (bool): If True, use multiprocessing for parallel execution.
     - processes (int): Number of processes to use in parallel execution (default is None, letting Pool decide).
     - callback (Callable): Optional callback function to execute after each iteration.
-
+    - context (str): Context of how multiprocessing spawns new processes.
     Returns:
     - List: A list of results from applying the function to each element.
     """
 
     N = len(params) if hasattr(params, "__len__") else None
 
     out = []
     if parallel:
-        with Pool(processes=processes) as pool:
+        with get_context(context).Pool(processes=processes) as pool:
             for result in tqdm(pool.imap(func, params), total=N):
                 out.append(result)
                 if callback:
                     callback(result)
         return out
     else:
         for param in tqdm(params):
             result = func(param)
             out.append(result)
             if callback:
                 callback(result)
         return out
-
-
-sys.modules[__name__] = foreach
```

### Comparing `foreach-0.3.0/PKG-INFO` & `foreach-0.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foreach
-Version: 0.3.0
+Version: 0.4.0
 Summary: 
 Author: Jaime Liew
 Author-email: jaimeliew1@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -27,15 +27,15 @@
 ```bash
 pip install foreach
 ```
 
 ## Usage
 
 ```python
-import foreach
+from foreach import foreach
 
 def square(x):
     return x**2
 
 params = [1, 2, 3, 4, 5]
 result = foreach(square, params)
 print(result)
@@ -59,30 +59,30 @@
 
 
 ## Examples
 
 ### Sequential Execution
 
 ```python
-import foreach
+from foreach import foreach
 
 def square(x):
     return x**2
 
 params = [1, 2, 3, 4, 5]
 result = foreach(square, params, parallel=False)
 print(result)
 # [1, 4, 9, 16, 25]
 ```
 
 
 ### Callback Functionality
 
 ```python
-import foreach
+from foreach import foreach
 
 def square(x):
     return x**2
 
 params = [1, 2, 3, 4, 5]
 
 def callback(x):
@@ -95,15 +95,15 @@
 # Processed: 16
 # Processed: 25
 ```
 
 ### Customizing Number of Processes
 
 ```python
-import foreach
+from foreach import foreach
 
 def square(x):
     return x**2
 
 params = [1, 2, 3, 4, 5]
 result = foreach(square, params, num_processes=2)
 print(result)
```

