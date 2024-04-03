# Comparing `tmp/pressio-linalg-0.1.0rc6.tar.gz` & `tmp/pressio-linalg-0.1.0rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pressio-linalg-0.1.0rc6.tar", last modified: Fri Mar  8 21:07:42 2024, max compression
+gzip compressed data, was "pressio-linalg-0.1.0rc7.tar", last modified: Wed Apr  3 16:41:49 2024, max compression
```

## Comparing `pressio-linalg-0.1.0rc6.tar` & `pressio-linalg-0.1.0rc7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:07:42.590822 pressio-linalg-0.1.0rc6/
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-03-08 21:07:42.586822 pressio-linalg-0.1.0rc6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-03-08 21:07:39.000000 pressio-linalg-0.1.0rc6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:07:42.586822 pressio-linalg-0.1.0rc6/pressio_linalg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-03-08 21:07:42.000000 pressio-linalg-0.1.0rc6/pressio_linalg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-08 21:07:42.000000 pressio-linalg-0.1.0rc6/pressio_linalg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 21:07:42.000000 pressio-linalg-0.1.0rc6/pressio_linalg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 21:07:42.000000 pressio-linalg-0.1.0rc6/pressio_linalg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-08 21:07:42.000000 pressio-linalg-0.1.0rc6/pressio_linalg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-08 21:07:42.000000 pressio-linalg-0.1.0rc6/pressio_linalg.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:07:42.586822 pressio-linalg-0.1.0rc6/pressiolinalg/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-08 21:07:39.000000 pressio-linalg-0.1.0rc6/pressiolinalg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27963 2024-03-08 21:07:39.000000 pressio-linalg-0.1.0rc6/pressiolinalg/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-03-08 21:07:39.000000 pressio-linalg-0.1.0rc6/pressiolinalg/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-08 21:07:39.000000 pressio-linalg-0.1.0rc6/pressiolinalg/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-08 21:07:39.000000 pressio-linalg-0.1.0rc6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-08 21:07:42.590822 pressio-linalg-0.1.0rc6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    11865 2024-03-08 21:07:39.000000 pressio-linalg-0.1.0rc6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:07:42.586822 pressio-linalg-0.1.0rc6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-03-08 21:07:39.000000 pressio-linalg-0.1.0rc6/tests/test_basic_mean_via_python.py
--rw-r--r--   0 runner    (1001) docker     (127)     8033 2024-03-08 21:07:39.000000 pressio-linalg-0.1.0rc6/tests/test_basic_min_max_via_python.py
--rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-03-08 21:07:39.000000 pressio-linalg-0.1.0rc6/tests/test_basic_product_via_python.py
--rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-03-08 21:07:39.000000 pressio-linalg-0.1.0rc6/tests/test_basic_std_via_python.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-03-08 21:07:39.000000 pressio-linalg-0.1.0rc6/tests/test_basic_svd_method_of_snapshots_via_python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:41:49.447139 pressio-linalg-0.1.0rc7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-03 16:41:49.447139 pressio-linalg-0.1.0rc7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-03 16:41:43.000000 pressio-linalg-0.1.0rc7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:41:49.447139 pressio-linalg-0.1.0rc7/pressio_linalg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-03 16:41:49.000000 pressio-linalg-0.1.0rc7/pressio_linalg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-03 16:41:49.000000 pressio-linalg-0.1.0rc7/pressio_linalg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 16:41:49.000000 pressio-linalg-0.1.0rc7/pressio_linalg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 16:41:49.000000 pressio-linalg-0.1.0rc7/pressio_linalg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-03 16:41:49.000000 pressio-linalg-0.1.0rc7/pressio_linalg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-03 16:41:49.000000 pressio-linalg-0.1.0rc7/pressio_linalg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:41:49.447139 pressio-linalg-0.1.0rc7/pressiolinalg/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-03 16:41:43.000000 pressio-linalg-0.1.0rc7/pressiolinalg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30556 2024-04-03 16:41:43.000000 pressio-linalg-0.1.0rc7/pressiolinalg/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-03 16:41:43.000000 pressio-linalg-0.1.0rc7/pressiolinalg/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-03 16:41:43.000000 pressio-linalg-0.1.0rc7/pressiolinalg/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-03 16:41:43.000000 pressio-linalg-0.1.0rc7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 16:41:49.447139 pressio-linalg-0.1.0rc7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    11865 2024-04-03 16:41:43.000000 pressio-linalg-0.1.0rc7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:41:49.447139 pressio-linalg-0.1.0rc7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4779 2024-04-03 16:41:43.000000 pressio-linalg-0.1.0rc7/tests/test_basic_mean_via_python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7523 2024-04-03 16:41:43.000000 pressio-linalg-0.1.0rc7/tests/test_basic_min_max_via_python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-04-03 16:41:43.000000 pressio-linalg-0.1.0rc7/tests/test_basic_product_via_python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-04-03 16:41:43.000000 pressio-linalg-0.1.0rc7/tests/test_basic_std_via_python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-03 16:41:43.000000 pressio-linalg-0.1.0rc7/tests/test_basic_svd_method_of_snapshots_via_python.py
```

### Comparing `pressio-linalg-0.1.0rc6/PKG-INFO` & `pressio-linalg-0.1.0rc7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pressio-linalg
-Version: 0.1.0rc6
+Version: 0.1.0rc7
 Summary: Parallel linear algebra library
 Author-email: francesco.rizzi@ng-analytics.com
 Keywords: model reduction,scientific computing,dense linear algebra,parallel computing,hyper-reduction,HPC
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Unix
 Classifier: Environment :: MacOS X
 Classifier: Programming Language :: C++
```

### Comparing `pressio-linalg-0.1.0rc6/README.md` & `pressio-linalg-0.1.0rc7/README.md`

 * *Files identical despite different names*

### Comparing `pressio-linalg-0.1.0rc6/pressio_linalg.egg-info/PKG-INFO` & `pressio-linalg-0.1.0rc7/pressio_linalg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pressio-linalg
-Version: 0.1.0rc6
+Version: 0.1.0rc7
 Summary: Parallel linear algebra library
 Author-email: francesco.rizzi@ng-analytics.com
 Keywords: model reduction,scientific computing,dense linear algebra,parallel computing,hyper-reduction,HPC
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Unix
 Classifier: Environment :: MacOS X
 Classifier: Programming Language :: C++
```

### Comparing `pressio-linalg-0.1.0rc6/pressio_linalg.egg-info/SOURCES.txt` & `pressio-linalg-0.1.0rc7/pressio_linalg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pressio-linalg-0.1.0rc6/pressiolinalg/linalg.py` & `pressio-linalg-0.1.0rc7/pressiolinalg/linalg.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,21 +16,23 @@
 
     Parameters:
         a (np.ndarray): input data
         axis (None or int): the axis along which to compute the maximum. If None, computes the max of the flattened array. (default: None)
         comm (MPI_Comm): MPI communicator (default: None)
 
     Returns:
-        if axis==None, returns a scalar
-        if axis is not None, returns an array of dimension a.dim - 1
+        if axis == None, returns a scalar
+        if axis is not None, returns an array of dimension a.ndim - 1
 
     Preconditions:
-      - a is at most a rank-3 tensor and
-      - if a is distributed, it must be so along the 0-th axis,
-        and every rank must have the same a.shape[1] and a.shape[2]
+      - a is at most a rank-3 tensor
+      - if a is a distributed 2-D array, it must be distributed along axis=0,
+        and every rank must have the same a.shape[1]
+      - if a is a distributed 3-D tensor, it must be distributed along axis=1,
+        and every rank must have the same a.shape[0] and a.shape[2]
       - if axis != None, then it must be an int
 
     Postconditions:
       - a and comm are not modified
 
     Example 1:
     **********
@@ -90,123 +92,108 @@
     so this operation is purely local and the result has the same distribution
     as the original array.
 
 
     Example 3:
     **********
 
-                / 3.  6. -7.
-       rank 0  /2.  1.  4.
-               --------------
+       / 3.   4.   /  2.   8.   2.   1.   / 2.
+      /  6.  -1.  /  -2.  -1.   0.  -6.  /  0.    -> slice T(:,:,1)
+     /  -7.   5. /    5.   0.   3.   1. /   3.
+    |-----------|----------------------|--------
+    | 2.   3.   |  4.   5.  -2.   4.   | -4.
+    | 1.   5.   | -2.   4.   8.  -3.   |  8.    ->  slice T(:,:,0)
+    | 4.   3.   | -4.   6.   9.  -4.   |  9.
 
-                / 4.  -1.  5.
-               /3.  5.  3.
-      =======================
+        r0                r1              r2
 
-       rank 1   / 2.  -2.  5.
-               /4.  -2.  -4.
-               --------------
+    Suppose that we do:
 
-                / 8.  -1.  0.
-               /5.   4.   6.
-               --------------
+        res = pla.max(a, axis=0, comm)
 
-                / 2.   0.   3.
-               /-2.   8.   9.
-               --------------
+    then res is now a rank-2 array as follows:
 
-                / 1.  -6.  1.
-               /4.  -3.  -4.
-      =======================
+       /  6.  5.   /  5.   8.   3.   1.  /  3.
+      / 4.   5.   / 4.   6.   9.   4.   /  9.
+     /           /                     /
+    /    r1     /         r2          /  r3
 
-       rank 2   / 2.   0.  3.
-               /-4.  8.   9.
-               --------------
+    because the axis queried for the max is NOT a distributed axis
+    and this is effectively a reduction over the 0-th axis
+    so this operation is purely local and the result has the same distribution
+    as the original array.
 
     Suppose that we do:
 
-       res = pla.max(a, axis=0, comm)
+      res = pla.max(a, axis=1, comm)
 
-    then this is effectively a reduction over the 0-th axis
+    then this is effectively a reduction over axis=1,
     and every rank will contain the same res which is a rank-2 array as follows
 
-          ([[5. 8.]
-            [8. 6.]
-            [9. 5.]])
+                  5.  8.
+                  8.  6.
+                  9.  5.
 
     this is because the max is queried for the 0-th axis which is the
     axis along which the data array is distributed.
     So this operation must be a collective operation and we know that
     memory-wise it is feasible to hold because this is no larger than the
     local allocation on each rank.
 
     Suppose that we do:
 
-      res = pla.max(a, axis=1, comm)
-
-    then res is now a rank-2 array as follows
-
-       rank 0  4, 6
-               5, 5
-      =======================
-       rank 1  4, 5
-               6, 8
-               9, 3
-               4, 1
-      =======================
-       rank 2  9, 3
-
-    because the axis queried for the max is NOT a distributed axis
-    and this is effectively a reduction over the 1-th axis
-    so this operation is purely local and the result has the same distribution
-    as the original array.
-
-    Suppose that we do:
-
       res = pla.max(a, axis=2, comm)
 
     then res is now a rank-2 array as follows
 
-       rank 0  3, 6, 4
-               4, 5, 5
-      =======================
-       rank 1  4, -2, 5
-               8, 4, 6
-               2, 8, 9
-               4, -3, 1
-      =======================
-       rank 2  2, 8, 9
+            r0     ||          r1           ||  r2
+                   ||                       ||
+          3.   4.  ||   4.   8.   2.   4.   ||   2.
+          6.   5.  ||  -2.   4.   8.  -3.   ||   8.
+          4.   5.  ||   5.   6.   9.   1.   ||   9.
+                   ||                       ||
 
     because the axis queried for the max is NOT a distributed axis
-    and this is effectively a reduction over the 1-th axis
+    and this is effectively a reduction over the 2-th axis
     so this operation is purely local and the result has the same distribution
     as the original array.
 
     '''
+    # Enforce preconditions
     assert a.ndim <= 3, "a must be at most a rank-3 tensor"
     utils.assert_axis_is_none_or_within_rank(a, axis)
 
+    # Return np.max if running serial
     if comm is None or comm.Get_size() == 1:
         return np.max(a, axis=axis)
 
+    # Otherwise, calculate distributed max
     else:
-
         import mpi4py
         from mpi4py import MPI
 
+        # Get the max on the current process
         local_max = np.max(a, axis=axis)
 
+        # Identify the axis along which the data is the distributed
+        distributed_axis = 0 if a.ndim < 3 else 1
+
+        # Return the max of the flattened array if no axis is given
         if axis is None:
             return comm.allreduce(local_max, op=MPI.MAX)
-        elif axis==0:
+
+        # If queried axis is the same as distributed axis, perform collective operation
+        elif axis==distributed_axis:
             if a.ndim == 1:
                 local_max = a
             global_max = np.zeros_like(local_max, dtype=local_max.dtype)
             comm.Allreduce(local_max, global_max, op=MPI.MAX)
             return global_max
+
+        # Otherwise, return the local_max on the current process
         else:
             return local_max
 
 
 # # ----------------------------------------------------
 def _basic_min_via_python(a: np.ndarray, axis=None, comm=None):
     '''
@@ -214,21 +201,23 @@
 
     Parameters:
         a (np.ndarray): input data
         axis (None or int): the axis along which to compute the minimum. If None, computes the min of the flattened array. (default: None)
         comm (MPI_Comm): MPI communicator (default: None)
 
     Returns:
-        if axis==None, returns a scalar
-        if axis is not None, returns an array of dimension a.dim - 1
+        if axis == None, returns a scalar
+        if axis is not None, returns an array of dimension a.ndim - 1
 
     Preconditions:
-      - a is at most a rank-3 tensor and
-      - if a is distributed, it must be so along the 0-th axis,
-        and every rank must have the same a.shape[1] and a.shape[2]
+      - a is at most a rank-3 tensor
+      - if a is a distributed 2-D array, it must be distributed along axis=0,
+        and every rank must have the same a.shape[1]
+      - if a is a distributed 3-D tensor, it must be distributed along axis=1,
+        and every rank must have the same a.shape[0] and a.shape[2]
       - if axis != None, then it must be an int
 
     Postconditions:
       - a and comm are not modified
 
     Example 1:
     **********
@@ -288,120 +277,108 @@
     so this operation is purely local and the result has the same distribution
     as the original array.
 
 
     Example 3:
     **********
 
-                / 3.  6. -7.
-       rank 0  /2.  1.  4.
-               --------------
+       / 3.   4.   /  2.   8.   2.   1.   / 2.
+      /  6.  -1.  /  -2.  -1.   0.  -6.  /  0.    -> slice T(:,:,1)
+     /  -7.   5. /    5.   0.   3.   1. /   3.
+    |-----------|----------------------|--------
+    | 2.   3.   |  4.   5.  -2.   4.   | -4.
+    | 1.   5.   | -2.   4.   8.  -3.   |  8.    ->  slice T(:,:,0)
+    | 4.   3.   | -4.   6.   9.  -4.   |  9.
 
-                / 4.  -1.  5.
-               /3.  5.  3.
-      =======================
+        r0                r1              r2
 
-       rank 1   / 2.  -2.  5.
-               /4.  -2.  -4.
-               --------------
+    Suppose that we do:
 
-                / 8.  -1.  0.
-               /5.   4.   6.
-               --------------
+        res = pla.max(a, axis=0, comm)
 
-                / 2.   0.  3.
-               /-2.   8.   9.
-               --------------
+    then res is now a rank-2 array as follows:
 
-                / 1.  -6.  1.
-               /4.  -3.  -4.
-      =======================
+       /  -7.  -1.  /  -2.   -1.   0.   -6.  /  0.
+      / 1.    3.   / -4.    4.   -2.   -4.  /  -4.
+     /            /                        /
+    /     r1     /           r2           /   r3
 
-       rank 2   / 2.   0.  3.
-               /-4.  8.   9.
-               --------------
+    because the axis queried for the max is NOT a distributed axis
+    and this is effectively a reduction over the 0-th axis
+    so this operation is purely local and the result has the same distribution
+    as the original array.
 
     Suppose that we do:
 
-       res = pla.min(a, axis=0, comm)
+      res = pla.max(a, axis=1, comm)
 
-    then this is effectively a reduction over the 0-th axis
+    then this is effectively a reduction over axis=1,
     and every rank will contain the same res which is a rank-2 array as follows
 
-          ([[8., 6., 5.],
-            [5, 8., 9.]])
+                    -4.   1.
+                    -3.  -6.
+                    -4.  -7.
 
-    this is because the min is queried for the 0-th axis which is the
+    this is because the max is queried for the 0-th axis which is the
     axis along which the data array is distributed.
     So this operation must be a collective operation and we know that
     memory-wise it is feasible to hold because this is no larger than the
     local allocation on each rank.
 
     Suppose that we do:
 
-      res = pla.min(a, axis=1, comm)
-
-    then res is now a rank-2 array as follows
-
-       rank 0  4, 6
-               5, 5
-      =======================
-       rank 1  4, 5
-               6, 8
-               9, 3
-               4, 1
-      =======================
-       rank 2  9, 3
-
-    because the axis queried for the min is NOT a distributed axis
-    and this is effectively a reduction over the 1-th axis
-    so this operation is purely local and the result has the same distribution
-    as the original array.
-
-    Suppose that we do:
-
-      res = pla.min(a, axis=2, comm)
+      res = pla.max(a, axis=2, comm)
 
     then res is now a rank-2 array as follows
 
-       rank 0  3, 6, 4
-               4, 5, 5
-      =======================
-       rank 1  4, -2, 5
-               8, 4, 6
-               2, 8, 9
-               4, -3, -4
-      =======================
-       rank 2  2, 8, 9
+             r0    ||          r1           ||  r2
+                   ||                       ||
+           2.  3.  ||   2.   5.  -2.   1.   ||  -4.
+           1. -1.  ||  -2.  -1.   0.  -6.   ||   0.
+          -7.  3.  ||  -4.   0.   3.  -4.   ||   3.
+                   ||                       ||
 
-    because the axis queried for the min is NOT a distributed axis
-    and this is effectively a reduction over the 1-th axis
+    because the axis queried for the max is NOT a distributed axis
+    and this is effectively a reduction over the 2-th axis
     so this operation is purely local and the result has the same distribution
     as the original array.
 
     '''
+    # Enforce preconditions
     assert a.ndim <= 3, "a must be at most a rank-3 tensor"
     utils.assert_axis_is_none_or_within_rank(a, axis)
 
+    # Return np.min if running serial
     if comm is None or comm.Get_size() == 1:
         return np.min(a, axis=axis)
+
+    # Otherwise, calculate distributed min
     else:
         import mpi4py
         from mpi4py import MPI
 
+        # Get the min on the current process
         local_min = np.min(a, axis=axis)
 
+        # Identify the axis along which the data is the distributed
+        distributed_axis = 0 if a.ndim < 3 else 1
+
+        # Return the min of the flattened array if no axis is given
         if axis is None:
             return comm.allreduce(local_min, op=MPI.MIN)
-        elif axis==0:
+
+        # If queried axis is the same as distributed axis, perform collective operation
+        elif axis==distributed_axis:
             if a.ndim == 1:
                 local_min = a
             global_min = np.zeros_like(local_min, dtype=local_min.dtype)
             comm.Allreduce(local_min, global_min, op=MPI.MIN)
             return global_min
+
+        # Otherwise, return the local_min on the current process
         else:
             return local_min
 
 
 # # ----------------------------------------------------
 def _basic_mean_via_python(a: np.ndarray, dtype=None, axis=None, comm=None):
     '''
@@ -410,21 +387,23 @@
     Parameters:
         a (np.ndarray): input data
         dtype (data-type): Type to use in computing the mean (default: float64 for int arrays, same type as input for float arrays)
         axis (None or int): the axis along which to compute the mean. If None, computes the mean of the flattened array. (default: None)
         comm (MPI_Comm): MPI communicator (default: None)
 
     Returns:
-        if axis==None, returns a scalar
-        if axis is not None, returns an array of dimension a.dim - 1
+        if axis == None, returns a scalar
+        if axis is not None, returns an array of dimension a.ndim - 1
 
     Preconditions:
-      - a is at most a rank-3 tensor and
-      - if a is distributed, it must be so along the 0-th axis,
-        and every rank must have the same a.shape[1] and a.shape[2]
+      - a is at most a rank-3 tensor
+      - if a is a distributed 2-D array, it must be distributed along axis=0,
+        and every rank must have the same a.shape[1]
+      - if a is a distributed 3-D tensor, it must be distributed along axis=1,
+        and every rank must have the same a.shape[0] and a.shape[2]
       - if axis != None, then it must be an int
 
     Postconditions:
       - a and comm are not modified
 
     Example 1:
     **********
@@ -488,154 +467,139 @@
     so this operation is purely local and the result has the same distribution
     as the original array.
 
 
     Example 3:
     **********
 
-                / 3.  6. -7.
-       rank 0  /2.  1.  4.
-               --------------
+       / 3.   4.   /  2.   8.   2.   1.   / 2.
+      /  6.  -1.  /  -2.  -1.   0.  -6.  /  0.    -> slice T(:,:,1)
+     /  -7.   5. /    5.   0.   3.   1. /   3.
+    |-----------|----------------------|--------
+    | 2.   3.   |  4.   5.  -2.   4.   | -4.
+    | 1.   5.   | -2.   4.   8.  -3.   |  8.    ->  slice T(:,:,0)
+    | 4.   3.   | -4.   6.   9.  -4.   |  9.
 
-                / 4.  -1.  5.
-               /3.  5.  3.
-      =======================
+        r0                r1              r2
 
-       rank 1   / 2.  -2.  5.
-               /4.  -2.  -4.
-               --------------
+    Suppose that we do:
 
-                / 8.  -1.  0.
-               /5.   4.   6.
-               --------------
+        res = pla.mean(a, axis=0, comm)
 
-                / 2.   0.  3.
-               /-2.   8.   9.
-               --------------
+    then res is now a rank-2 array as follows:
 
-                / 1.  -6.  1.
-               /4.  -3.  -4.
-      =======================
+       /   0.6667   2.6667  /    1.6667   2.3333   1.6667   -1.3333  /   1.6667
+      / 2.3333  3.6667     / -0.6667.   5.       5.      -1.        /  4.3333
+     /                    /                                        /
+    /         r1         /                  r2                    /    r3
 
-       rank 2   / 2.   0.  3.
-               /-4.  8.   9.
-               --------------
+    because the axis queried for the mean is NOT a distributed axis
+    and this is effectively a reduction over the 0-th axis
+    so this operation is purely local and the result has the same distribution
+    as the original array.
 
     Suppose that we do:
 
-       res = pla.mean(a, axis=0, comm)
+      res = pla.mean(a, axis=1, comm)
 
-    then this is effectively a reduction over the 0-th axis
+    then this is effectively a reduction over axis=1,
     and every rank will contain the same res which is a rank-2 array as follows
 
-          ([[ 1.71,  3.14],
-            [ 3.  , -0.57],
-            [ 3.29,  1.43]])
+              1.71428571  3.1428571
+              3.         -0.5714285
+              3.28571429  1.4285714
 
     this is because the mean is queried for the 0-th axis which is the
     axis along which the data array is distributed.
     So this operation must be a collective operation and we know that
     memory-wise it is feasible to hold because this is no larger than the
     local allocation on each rank.
 
     Suppose that we do:
 
-      res = pla.mean(a, axis=1, comm)
-
-    then res is now a rank-2 array as follows
-
-       rank 0   2.33,  0.67
-                3.67, -0.57
-      =======================
-       rank 1  -0.67,  1.67
-                5.  ,  2.33
-                5.  ,  1.67
-               -1.  , -1.33
-      =======================
-       rank 2   4.33,  1.67
-
-    because the axis queried for the mean is NOT a distributed axis
-    and this is effectively a reduction over the 1-th axis
-    so this operation is purely local and the result has the same distribution
-    as the original array
-
-    Suppose that we do:
-
       res = pla.mean(a, axis=2, comm)
 
     then res is now a rank-2 array as follows
 
-      rank 0   2.5,  3.5, -1.5
-               3.5,  2. ,  4.
-      ===========================
-      rank 1   3. , -2. ,  0.5
-               6.5,  1.5,  3.
-               0. ,  4. ,  6.
-               2.5, -4.5, -1.5
-      ===========================
-      rank 2   -1. ,  4. ,  6.
+           r0      ||          r1           ||  r2
+                   ||                       ||
+         2.5  3.5  ||   3.   6.5  0.   2.5  || -1.
+         3.5  2.   ||  -2.   1.5  4.  -4.5  ||  4.
+        -1.5  4.   ||   0.5  3.   6.  -1.5  ||  6.
+                   ||                       ||
 
     because the axis queried for the mean is NOT a distributed axis
-    and this is effectively a reduction over the 1-th axis
+    and this is effectively a reduction over the 2-th axis
     so this operation is purely local and the result has the same distribution
-    as the original array
+    as the original array.
 
     '''
+    # Enforce preconditions
     assert a.ndim <= 3, "a must be at most a rank-3 tensor"
     utils.assert_axis_is_none_or_within_rank(a, axis)
 
+    # Return np.mean if running serial
     if comm is None or comm.Get_size() == 1:
         return np.mean(a, dtype=dtype, axis=axis)
 
+    # Otherwise calculate distributed mean
     else:
-
         import mpi4py
         from mpi4py import MPI
 
-        local_size = a.size if axis is None else a.shape[0]
+        # Get the size (mean = sum/size) -- num elements if axis is None, or num rows along given axis
+        local_size = a.size if axis is None else a.shape[axis]
         global_size = comm.allreduce(local_size, op=MPI.SUM)
 
+        # Warn if dividing by 0
         if global_size == 0:
             warnings.warn("Invalid value encountered in scalar divide (global_size = 0)")
             return np.nan
 
+        # Identify the axis along which the input array is distributed
+        distributed_axis = 0 if a.ndim < 3 else 1
+
+        # Calculate mean of flattened array if no axis is given
         if axis is None:
             local_sum = np.sum(a)
             global_sum = comm.allreduce(local_sum, op=MPI.SUM)
             return global_sum / global_size
 
-        elif axis == 0:
+        # Get mean along distributed axis and perform collective operation
+        elif axis == distributed_axis:
             local_sum = np.sum(a, axis=axis)
             global_sum = np.zeros_like(np.mean(a, axis=axis))
             comm.Allreduce(local_sum, global_sum, op=MPI.SUM)
             return global_sum / global_size
 
+        # Return the local mean if queried axis is not the distributed axis
         else:
             return np.mean(a, dtype=dtype, axis=axis)
 
 # ----------------------------------------------------
-def _basic_std_via_python(a: np.ndarray, dtype=None, axis=None, ddof=0, comm=None):
+def _basic_std_via_python(a: np.ndarray, dtype=None, axis=None, testing=False, comm=None):
     '''
     Return the standard deviation of a possibly distributed array over a given axis.
 
     Parameters:
         a (np.ndarray): input data
         dtype (data-type): Type to use in computing the mean (default: float64 for int arrays, same type as input for float arrays)
         axis (None or int): the axis along which to compute the mean. If None, computes the mean of the flattened array. (default: None)
-        ddof (int): Delta degrees of freedom used in divisor N - ddof (default: 0)
         comm (MPI_Comm): MPI communicator (default: None)
 
     Returns:
-        if axis==None, returns a scalar
-        if axis is not None, returns an array of dimension a.dim - 1
+        if axis == None, returns a scalar
+        if axis is not None, returns an array of dimension a.ndim - 1
 
     Preconditions:
-      - a is at most a rank-3 tensor and
-      - if a is distributed, it must be so along the 0-th axis,
-        and every rank must have the same a.shape[1] and a.shape[2]
+      - a is at most a rank-3 tensor
+      - if a is a distributed 2-D array, it must be distributed along axis=0,
+        and every rank must have the same a.shape[1]
+      - if a is a distributed 3-D tensor, it must be distributed along axis=1,
+        and every rank must have the same a.shape[0] and a.shape[2]
       - if axis != None, then it must be an int
 
     Postconditions:
       - a and comm are not modified
 
     Example 1:
     **********
@@ -697,130 +661,129 @@
     because the axis queried for the standard deviation is NOT a distributed axis
     so this operation is purely local and the result has the same distribution
     as the original array.
 
     Example 3:
     **********
 
-                / 3.  6. -7.
-       rank 0  /2.  1.  4.
-               --------------
+       / 3.   4.   /  2.   8.   2.   1.   / 2.
+      /  6.  -1.  /  -2.  -1.   0.  -6.  /  0.    -> slice T(:,:,1)
+     /  -7.   5. /    5.   0.   3.   1. /   3.
+    |-----------|----------------------|--------
+    | 2.   3.   |  4.   5.  -2.   4.   | -4.
+    | 1.   5.   | -2.   4.   8.  -3.   |  8.    ->  slice T(:,:,0)
+    | 4.   3.   | -4.   6.   9.  -4.   |  9.
 
-                / 4.  -1.  5.
-               /3.  5.  3.
-      =======================
+        r0                r1              r2
 
-       rank 1   / 2.  -2.  5.
-               /4.  -2.  -4.
-               --------------
+    Suppose that we do:
 
-                / 8.  -1.  0.
-               /5.   4.   6.
-               --------------
+        res = pla.std(a, axis=0, comm)
 
-                / 2.   0.  3.
-               /-2.   8.   9.
-               --------------
+    then res is now a rank-2 array as follows:
 
-                / 1.  -6.  1.
-               /4.  -3.  -4.
-      =======================
+       /   5.5578   2.6247   /    2.8674   4.0277   1.2472   3.2998   /   1.2472
+      / 1.2472   0.9428     / 3.3993   0.8165   4.9666   3.5590      / 5.9067
+     /                     /                                        /
+    /          r1         /                  r2                    /     r3
 
-       rank 2   / 2.   0.  3.
-               /-4.  8.   9.
-               --------------
+    because the axis queried for the standard deviation is NOT a distributed axis
+    and this is effectively a reduction over the 0-th axis
+    so this operation is purely local and the result has the same distribution
+    as the original array.
 
     Suppose that we do:
 
-       res = pla.std(a, axis=0, comm)
+      res = pla.std(a, axis=1, comm)
 
-    then this is effectively a reduction over the 0-th axis
+    then this is effectively a reduction over axis=1,
     and every rank will contain the same res which is a rank-2 array as follows
 
-      ([[3.14934396, 2.16653584],
-       [4.14039336, 3.28881841],
-       [5.06287004, 3.84919817]])
+              3.14934396  2.16653584
+              4.14039336  3.28881841
+              5.06287004  3.84919817
 
     this is because the standard deviation is queried for the 0-th axis which is the
     axis along which the data array is distributed.
     So this operation must be a collective operation and we know that
     memory-wise it is feasible to hold because this is no larger than the
     local allocation on each rank.
 
     Suppose that we do:
 
-      res = pla.std(a, axis=1, comm)
-
-    then res is now a rank-2 array as follows
-
-       rank 0   1.24721913, 5.55777733
-                0.94280904, 2.62466929
-      ===================================
-       rank 1   3.39934634, 2.86744176
-                0.81649658, 4.02768199
-                4.96655481, 1.24721913
-                3.55902608, 3.29983165
-      ===================================
-       rank 2   5.90668172, 1.24721913
-
-    because the axis queried for the standard deviation is NOT a distributed axis
-    and this is effectively a reduction over the 1-th axis
-    so this operation is purely local and the result has the same distribution
-    as the original array.
-
-    Suppose that we do:
-
       res = pla.std(a, axis=2, comm)
 
     then res is now a rank-2 array as follows
 
-       rank 0   0.5, 2.5, 5.5
-                0.5, 3. , 1.
-      ===========================
-       rank 1   1. , 0. , 4.5
-                1.5, 2.5, 3.
-                2. , 4. , 3.
-                1.5, 1.5, 2.5
-      ===========================
-       rank 2   3. , 4. , 3.
+           r0      ||          r1           ||  r2
+                   ||                       ||
+         0.5  0.5  ||   1.   1.5  2.  1.5   ||   3.
+         2.5  3.   ||   0.   2.5  4.  1.5   ||   4.
+         5.5  1.   ||   4.5  3.   3.  2.5   ||   3.
+                   ||                       ||
 
     because the axis queried for the standard deviation is NOT a distributed axis
-    and this is effectively a reduction over the 1-th axis
+    and this is effectively a reduction over the 2-th axis
     so this operation is purely local and the result has the same distribution
     as the original array.
     '''
+    # Enforce preconditions
     assert a.ndim <= 3, "a must be at most a rank-3 tensor"
     utils.assert_axis_is_none_or_within_rank(a, axis)
 
+    # Return np.std if running serial
     if comm is None or comm.Get_size() == 1:
-        return np.std(a, dtype=dtype, axis=axis, ddof=ddof)
+        return np.std(a, dtype=dtype, axis=axis)
+
+    # Otherwis, calculate distributed standard deviation
     else:
         import mpi4py
         from mpi4py import MPI
 
-        # Calculate quanities shared among axis=None or axis=0
-        if axis is None or axis == 0:
+        # Determine the axis along which the data is distributed
+        distributed_axis = 0 if a.ndim < 3 else 1
+
+        # Calculate standard deviation of flattened array
+        if axis is None:
             global_mean = _basic_mean_via_python(a, dtype=dtype, axis=axis, comm=comm)
+
+            # Compute the sum of the squared differences from the mean
             local_sq_diff = np.sum(np.square(a - global_mean), axis=axis)
-            local_size = a.size if axis is None else a.shape[0]
+            local_size = a.size
             global_size = comm.allreduce(local_size, op=MPI.SUM)
-
-        if axis is None:
             global_sq_diff = comm.allreduce(local_sq_diff, op=MPI.SUM)
-            global_std_dev = np.sqrt(global_sq_diff / (global_size - ddof))
+
+            # Return the standard deviation
+            global_std_dev = np.sqrt(global_sq_diff / (global_size))
             return global_std_dev
 
-        elif axis == 0:
+        # Calculate standard deviation along specified axis
+        elif axis == distributed_axis:
+            global_mean = _basic_mean_via_python(a, dtype=dtype, axis=axis, comm=comm)
+
+            # Compute the sum of the squared differences from the mean
+            if distributed_axis == 0:
+                local_sq_diff = np.sum(np.square(a - global_mean), axis=axis)
+            else:
+                # Must specify how to broadcast the global_mean to match dimensions of a
+                local_sq_diff = np.sum(np.square(a - global_mean[:,np.newaxis,:]), axis=axis)
+
+            # Get global squared differences
+            local_size = a.shape[axis]
+            global_size = comm.allreduce(local_size, op=MPI.SUM)
             global_sq_diff = np.zeros_like(local_sq_diff)
             comm.Allreduce(local_sq_diff, global_sq_diff, op=MPI.SUM)
-            global_std_dev = np.sqrt(global_sq_diff / (global_size - ddof))
+
+            # Return the standard deviation
+            global_std_dev = np.sqrt(global_sq_diff / (global_size))
             return global_std_dev
 
+        # Return the local standard deviation if queried axis is not the distributed axis
         else:
-            return np.std(a, dtype=dtype, axis=axis, ddof=ddof)
+            return np.std(a, dtype=dtype, axis=axis)
 
 # ----------------------------------------------------
 def _basic_product_via_python(flagA, flagB, alpha, A, B, beta, C, comm=None):
     '''
     Computes C = beta*C + alpha*op(A)*op(B), where A and B are row-distributed matrices.
 
     Parameters:
```

### Comparing `pressio-linalg-0.1.0rc6/pressiolinalg/test_utils.py` & `pressio-linalg-0.1.0rc7/pressiolinalg/test_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,26 @@
     print("module 'mpi4py' is not installed")
 
 
 #####################################################
 ########             MPI Helpers             ########
 #####################################################
 
-def distribute_array_impl(global_array, comm, axis=0):
+def distribute_array_impl(global_array, comm, dist_axis=0):
     '''
-    Splts an np.array and distributes to all available MPI processes as evenly as possible
+    Splts an np.array and distributes to all available MPI processes as evenly as possible.
+
+    For example, distributing an array with 6 rows over 3 processes will result in 2 rows
+    per process.
+    If the array has 7 rows, 2 processors will hold 2 rows, and the third will hold 3 rows.
 
     Inputs:
         global_array: The global np.array to be distributed.
         comm: The MPI communicator
-        axis: The axis along which to split the input array. By default, splits along the first axis (rows).
+        dist_axis: The axis along which to split the input array. By default, splits along the first axis (rows).
 
     Returns:
         local_array: The subset of global_array sent to the current MPI process.
 
     '''
     # Get comm info
     n_procs = comm.Get_size()
@@ -29,47 +33,54 @@
 
     # Handle null case
     if global_array.size == 0:
         return np.empty(0)
 
     # Split the global_array and send to corresponding MPI rank
     if rank == 0:
-        splits = np.array_split(global_array, n_procs, axis=axis)
+        splits = np.array_split(global_array, n_procs, axis=dist_axis)
         for proc in range(n_procs):
             if proc == 0:
                 local_array = splits[proc]
             else:
                 comm.send(splits[proc], dest=proc)
     else:
         local_array = comm.recv(source=0)
 
     return local_array
 
 def generate_random_local_and_global_arrays_impl(shape, comm):
-    '''Randomly generates both local and global arrays using optional dim<x> arguments to specify the shape'''
+    '''
+    Randomly generates a global array of the specified shape and distributes to all available
+    MPI processes.
+
+    Returns both the local and global arrays.
+    '''
     # Get comm info
     rank = comm.Get_rank()
 
     # Create global_array (using optional dim<x> arguments)
     if shape == tuple():
         global_arr = np.empty(0)
     elif len(shape) <=3:
         global_arr = np.random.rand(*shape) if rank == 0 else np.empty(shape)
     else:
         raise ValueError(f"This function only supports arrays up to rank 3 (received rank {ndim})")
 
     # Broadcast global_array and create local_array
     comm.Bcast(global_arr, root=0)
-    local_arr = distribute_array_impl(global_arr.copy(), comm)
+    dist_axis = 0 if len(shape) < 3 else 1
+    local_arr = distribute_array_impl(global_arr.copy(), comm, dist_axis)
 
     return local_arr, global_arr
 
 def generate_local_and_global_arrays_from_example_impl(rank, slices, example: int):
-    '''Generates both local and global arrays built from the example tensors in the documentation.
-       Also returns "slices," which tells how the arrays have been distributed.'''
+    '''
+    Generates and returns the local and global arrays built from the example tensors in the documentation.
+    '''
     # Create arrays
     if example == 1:
         global_arr = np.array([2.2, 3.3, 40., 51., -24., 45., -4.])
         local_arr = global_arr[slices[rank][0]:slices[rank][1]]
 
     elif example == 2:
         global_arr = np.array([[2.2, 1.3, 4.],
@@ -78,20 +89,16 @@
                                [51., 4., 6.],
                                [-24., 8., 9.],
                                [45., -3., -4.],
                                [-4., 8., 9.]])
         local_arr = global_arr[slices[rank][0]:slices[rank][1],:]
 
     elif example == 3:
-        global_arr = np.array([[[2.,3.],[1.,6.],[4.,-7]],
-                               [[3.,4.],[5.,-1.],[3.,5.]],
-                               [[4.,2],[-2.,-2.],[-4.,5]],
-                               [[5.,8.],[4.,-1.],[6.,0]],
-                               [[-2.,2,],[8.,0.],[9.,3]],
-                               [[4.,1],[-3.,-6.],[-4.,1]],
-                               [[-4.,2.],[8.,0.],[9.,3.]]])
-        local_arr = global_arr[slices[rank][0]:slices[rank][1],:,:]
+        global_arr = np.array([[[2.,3.],[3.,4.],[4.,2.],[5.,8.],[-2.,2.],[4.,1.],[-4.,2.]],
+                               [[1.,6.],[5.,-1.],[-2.,-2.],[4.,-1.],[8.,0.],[-3.,-6.],[8.,0.]],
+                               [[4.,-7.],[3.,5.],[-4.,5.],[6.,0.],[9.,3.],[-4.,1.],[9.,3.]]])
+        local_arr = global_arr[:,slices[rank][0]:slices[rank][1],:]
 
     else:
         return None, None
 
     return local_arr, global_arr
```

### Comparing `pressio-linalg-0.1.0rc6/setup.py` & `pressio-linalg-0.1.0rc7/setup.py`

 * *Files identical despite different names*

### Comparing `pressio-linalg-0.1.0rc6/tests/test_basic_mean_via_python.py` & `pressio-linalg-0.1.0rc7/tests/test_basic_mean_via_python.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,27 +50,26 @@
     res_ex2_ax1 = _basic_mean_via_python(local_arr_2, axis=1, comm=comm)
     full_ex2_ax1_mean = np.mean(global_arr_2, axis=1)
     exp_ex2_ax1 = full_ex2_ax1_mean[slices[rank][0]:slices[rank][1]]
     assert np.allclose(res_ex2_ax1, exp_ex2_ax1)
 
     # Example 3
     local_arr_3, global_arr_3 = test_utils.generate_local_and_global_arrays_from_example_impl(rank, slices, example=3)
-
     res_ex3_ax0 = _basic_mean_via_python(local_arr_3, axis=0, comm=comm)
-    exp_ex3_ax0 = np.mean(global_arr_3, axis=0)
+    full_ex3_ax0_mean = np.mean(global_arr_3, axis=0)
+    exp_ex3_ax0 = full_ex3_ax0_mean[slices[rank][0]:slices[rank][1],:]
     assert np.allclose(res_ex3_ax0, exp_ex3_ax0)
 
     res_ex3_ax1 = _basic_mean_via_python(local_arr_3, axis=1, comm=comm)
-    full_ex3_ax1_mean = np.mean(global_arr_3, axis=1)
-    exp_ex3_ax1 = full_ex3_ax1_mean[slices[rank][0]:slices[rank][1],:]
+    exp_ex3_ax1 = np.mean(global_arr_3, axis=1)
     assert np.allclose(res_ex3_ax1, exp_ex3_ax1)
 
     res_ex3_ax2 = _basic_mean_via_python(local_arr_3, axis=2, comm=comm)
     full_ex3_ax2_mean = np.mean(global_arr_3, axis=2)
-    exp_ex3_ax2 = full_ex3_ax2_mean[slices[rank][0]:slices[rank][1],:]
+    exp_ex3_ax2 = full_ex3_ax2_mean[:,slices[rank][0]:slices[rank][1]]
     assert np.allclose(res_ex3_ax2, exp_ex3_ax2)
 
 @pytest.mark.mpi(min_size=3)
 def test_python_mean_vector_mpi():
     comm = MPI.COMM_WORLD
     result, expected = _mean_setup(ndim=1, comm=comm)
     np.testing.assert_almost_equal(result, expected, decimal=10)
@@ -97,17 +96,26 @@
 
 @pytest.mark.mpi(min_size=3)
 def test_python_mean_array_axis_mpi():
     comm = MPI.COMM_WORLD
     result_01, expected_01 = _mean_setup(ndim=2, axis=0, comm=comm)
     assert np.allclose(result_01, expected_01)
 
-    result_02, expected_02 = _mean_setup(ndim=3, axis=1, comm=comm)
+    result_02, expected_02 = _mean_setup(ndim=2, axis=1, comm=comm)
     assert len(np.setdiff1d(result_02, expected_02)) == 0
 
+@pytest.mark.mpi(min_size=3)
+def test_python_mean_tensor_axis_mpi():
+    comm = MPI.COMM_WORLD
+    result_01, expected_01 = _mean_setup(ndim=3, axis=0, comm=comm)
+    assert len(np.setdiff1d(result_01, expected_01)) == 0
+
+    result_02, expected_02 = _mean_setup(ndim=3, axis=1, comm=comm)
+    assert np.allclose(result_02, expected_02)
+
     result_03, expected_03 = _mean_setup(ndim=3, axis=2, comm=comm)
     assert len(np.setdiff1d(result_03, expected_03)) == 0
 
 def test_python_mean_serial():
     vector = np.random.rand(10)
     np.testing.assert_almost_equal(_basic_mean_via_python(vector), np.mean(vector), decimal=10)
 
@@ -117,8 +125,9 @@
 
 if __name__ == "__main__":
     test_python_mean_examples_mpi()
     test_python_mean_null_vector_mpi()
     test_python_mean_vector_mpi()
     test_python_mean_array_mpi()
     test_python_mean_array_axis_mpi()
+    test_python_mean_tensor_axis_mpi()
     test_python_mean_serial()
```

### Comparing `pressio-linalg-0.1.0rc6/tests/test_basic_min_max_via_python.py` & `pressio-linalg-0.1.0rc7/tests/test_basic_min_max_via_python.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 
 ########################
 ###  Set up problem  ###
 ########################
 
 def _min_max_setup(operation, ndim, axis=None, comm=None):
-    num_processors = comm.Get_size()
     shape = (7,5,6)
     local_arr, global_arr = test_utils.generate_random_local_and_global_arrays_impl(shape[:ndim], comm)
 
     if operation == "min":
         min_result = _basic_min_via_python(local_arr, comm=comm)
         return min_result, np.min(global_arr)
     elif operation == "max":
@@ -40,109 +39,85 @@
     """Specifically tests the documented examples in _basic_max_via_python."""
     comm = MPI.COMM_WORLD
     rank = comm.Get_rank()
     slices = [(0,2), (2,6), (6,7)]
 
     # Example 1
     local_arr_1, global_arr_1 = test_utils.generate_local_and_global_arrays_from_example_impl(rank, slices, example=1)
-    res = _basic_max_via_python(local_arr_1, comm=comm)
-    assert res == 51.
+
+    res_ex1 = _basic_max_via_python(local_arr_1, comm=comm)
+    assert res_ex1 == np.max(global_arr_1)
 
     # Example 2
     local_arr_2, global_arr_2 = test_utils.generate_local_and_global_arrays_from_example_impl(rank, slices, example=2)
 
-    res_0 = _basic_max_via_python(local_arr_2, axis=0, comm=comm)
-    assert np.allclose(res_0, np.array([51., 8., 33.]))
-
-    res_1 = _basic_max_via_python(local_arr_2, axis=1, comm=comm)
-    if rank == 0:
-        assert np.allclose(res_1, np.array([4., 33.]))
-    elif rank == 1:
-        assert np.allclose(res_1, np.array([40., 51., 9., 45.]))
-    elif rank == 2:
-        assert np.allclose(res_1, np.array([9.]))
+    res_ex2_ax0 = _basic_max_via_python(local_arr_2, axis=0, comm=comm)
+    exp_ex2_ax0 = np.max(global_arr_2, axis=0)
+    assert np.allclose(res_ex2_ax0, exp_ex2_ax0)
+
+    res_ex2_ax1 = _basic_max_via_python(local_arr_2, axis=1, comm=comm)
+    full_ex2_ax1_max = np.max(global_arr_2, axis=1)
+    exp_ex2_ax1 = full_ex2_ax1_max[slices[rank][0]:slices[rank][1]]
+    assert np.allclose(res_ex2_ax1, exp_ex2_ax1)
 
     # Example 3
     local_arr_3, global_arr_3 = test_utils.generate_local_and_global_arrays_from_example_impl(rank, slices, example=3)
+    res_ex3_ax0 = _basic_max_via_python(local_arr_3, axis=0, comm=comm)
+    full_ex3_ax0_max = np.max(global_arr_3, axis=0)
+    exp_ex3_ax0 = full_ex3_ax0_max[slices[rank][0]:slices[rank][1],:]
+    assert np.allclose(res_ex3_ax0, exp_ex3_ax0)
+
+    res_ex3_ax1 = _basic_max_via_python(local_arr_3, axis=1, comm=comm)
+    exp_ex3_ax1 = np.max(global_arr_3, axis=1)
+    assert np.allclose(res_ex3_ax1, exp_ex3_ax1)
 
-    # Axis 0
-    res_ex3_0 = _basic_max_via_python(local_arr_3, axis=0, comm=comm)
-    assert np.allclose(res_ex3_0, np.max(global_arr_3, axis=0))
-
-    # Axis 1
-    res_ex3_1 = _basic_max_via_python(local_arr_3, axis=1, comm=comm)
-    if rank == 0:
-        expected_1 = np.array([[4., 6.],
-                               [5., 5.]])
-    elif rank == 1:
-        expected_1 = np.array([[4., 5.],
-                               [6., 8.],
-                               [9., 3.],
-                               [4., 1.]])
-    elif rank == 2:
-        expected_1 = np.array([[9., 3.]])
-    assert np.allclose(res_ex3_1, expected_1)
-
-    # Axis 2
-    res_ex3_2 = _basic_max_via_python(local_arr_3, axis=2, comm=comm)
-    if rank == 0:
-        expected_2 = np.array([[3., 6., 4.],
-                               [4., 5., 5.]])
-    elif rank == 1:
-        expected_2 = np.array([[4., -2., 5.],
-                               [8., 4., 6.],
-                               [2., 8., 9.],
-                               [4., -3., 1.]])
-    elif rank == 2:
-        expected_2 = np.array([[2., 8., 9.]])
-    assert np.allclose(res_ex3_2, expected_2)
+    res_ex3_ax2 = _basic_max_via_python(local_arr_3, axis=2, comm=comm)
+    full_ex3_ax2_max = np.max(global_arr_3, axis=2)
+    exp_ex3_ax2 = full_ex3_ax2_max[:,slices[rank][0]:slices[rank][1]]
+    assert np.allclose(res_ex3_ax2, exp_ex3_ax2)
 
 @pytest.mark.mpi(min_size=3)
 def test_python_min_examples_mpi():
     """Specifically tests the documented examples in _basic_min_via_python."""
     comm = MPI.COMM_WORLD
     rank = comm.Get_rank()
     slices = [(0,2), (2,6), (6,7)]
 
     # Example 1
     local_arr_1, global_arr_1 = test_utils.generate_local_and_global_arrays_from_example_impl(rank, slices, example=1)
-    res = _basic_min_via_python(local_arr_1, comm=comm)
-    assert res == -24.
+
+    res_ex1 = _basic_min_via_python(local_arr_1, comm=comm)
+    assert res_ex1 == np.min(global_arr_1)
 
     # Example 2
     local_arr_2, global_arr_2 = test_utils.generate_local_and_global_arrays_from_example_impl(rank, slices, example=2)
 
-    # Axis 0
-    res_0 = _basic_min_via_python(local_arr_2, axis=0, comm=comm)
-    assert np.allclose(res_0, np.array([-24., -3., -4.]))
-
-    # Axis 1
-    res_1 = _basic_min_via_python(local_arr_2, axis=1, comm=comm)
-    if rank == 0:
-        assert np.allclose(res_1, np.array([1.3, 3.3]))
-    elif rank == 1:
-        assert np.allclose(res_1, np.array([-4., 4., -24., -4.]))
-    elif rank == 2:
-        assert np.allclose(res_1, np.array([-4.]))
+    res_ex2_ax0 = _basic_min_via_python(local_arr_2, axis=0, comm=comm)
+    exp_ex2_ax0 = np.min(global_arr_2, axis=0)
+    assert np.allclose(res_ex2_ax0, exp_ex2_ax0)
+
+    res_ex2_ax1 = _basic_min_via_python(local_arr_2, axis=1, comm=comm)
+    full_ex2_ax1_min = np.min(global_arr_2, axis=1)
+    exp_ex2_ax1 = full_ex2_ax1_min[slices[rank][0]:slices[rank][1]]
+    assert np.allclose(res_ex2_ax1, exp_ex2_ax1)
 
     # Example 3
     local_arr_3, global_arr_3 = test_utils.generate_local_and_global_arrays_from_example_impl(rank, slices, example=3)
-
     res_ex3_ax0 = _basic_min_via_python(local_arr_3, axis=0, comm=comm)
-    exp_ex3_ax0 = np.min(global_arr_3, axis=0)
+    full_ex3_ax0_min = np.min(global_arr_3, axis=0)
+    exp_ex3_ax0 = full_ex3_ax0_min[slices[rank][0]:slices[rank][1],:]
     assert np.allclose(res_ex3_ax0, exp_ex3_ax0)
 
     res_ex3_ax1 = _basic_min_via_python(local_arr_3, axis=1, comm=comm)
-    full_ex3_ax1_min = np.min(global_arr_3, axis=1)
-    exp_ex3_ax1 = full_ex3_ax1_min[slices[rank][0]:slices[rank][1],:]
+    exp_ex3_ax1 = np.min(global_arr_3, axis=1)
     assert np.allclose(res_ex3_ax1, exp_ex3_ax1)
 
     res_ex3_ax2 = _basic_min_via_python(local_arr_3, axis=2, comm=comm)
     full_ex3_ax2_min = np.min(global_arr_3, axis=2)
-    exp_ex3_ax2 = full_ex3_ax2_min[slices[rank][0]:slices[rank][1],:]
+    exp_ex3_ax2 = full_ex3_ax2_min[:,slices[rank][0]:slices[rank][1]]
     assert np.allclose(res_ex3_ax2, exp_ex3_ax2)
 
 @pytest.mark.mpi(min_size=3)
 def test_python_max_vector_mpi():
     comm = MPI.COMM_WORLD
     result, expected = _min_max_setup(operation="max", ndim=1, comm=comm)
     assert result == expected
```

### Comparing `pressio-linalg-0.1.0rc6/tests/test_basic_product_via_python.py` & `pressio-linalg-0.1.0rc7/tests/test_basic_product_via_python.py`

 * *Files identical despite different names*

### Comparing `pressio-linalg-0.1.0rc6/tests/test_basic_std_via_python.py` & `pressio-linalg-0.1.0rc7/tests/test_basic_std_via_python.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 from pressiolinalg.linalg import _basic_std_via_python
 
 
 ########################
 ###  Set up problem  ###
 ########################
 
-def _std_setup(ndim, dtype=None, axis=None, ddof=0, comm=None):
+def _std_setup(ndim, dtype=None, axis=None, comm=None):
     n_procs = comm.Get_size()
     shape = (7,5,6)
     local_arr, global_arr = test_utils.generate_random_local_and_global_arrays_impl(shape[:ndim], comm)
 
-    std_result = _basic_std_via_python(local_arr, dtype=dtype, axis=axis, ddof=ddof, comm=comm)
-    return std_result, np.std(global_arr, dtype=dtype, axis=axis, ddof=ddof)
+    std_result = _basic_std_via_python(local_arr, dtype=dtype, axis=axis, comm=comm)
+    return std_result, np.std(global_arr, dtype=dtype, axis=axis)
 
 
 ########################
 ###   Define Tests   ###
 ########################
 
 @pytest.mark.mpi(min_size=3)
@@ -33,15 +33,15 @@
     comm = MPI.COMM_WORLD
     rank = comm.Get_rank()
     slices = [(0,2), (2,6), (6,7)]
 
     # Example 1
     local_arr_1, global_arr_1 = test_utils.generate_local_and_global_arrays_from_example_impl(rank, slices, example=1)
     res_ex1 = _basic_std_via_python(local_arr_1, comm=comm)
-    np.testing.assert_almost_equal(res_ex1, np.std(global_arr_1))
+    np.testing.assert_almost_equal(res_ex1, np.std(global_arr_1), decimal=10)
 
     # Example 2
     local_arr_2, global_arr_2 = test_utils.generate_local_and_global_arrays_from_example_impl(rank, slices, example=2)
 
     res_ex2_ax0 = _basic_std_via_python(local_arr_2, axis=0, comm=comm)
     exp_ex2_ax0 = np.std(global_arr_2, axis=0)
     assert np.allclose(res_ex2_ax0, exp_ex2_ax0)
@@ -49,59 +49,53 @@
     res_ex2_ax1 = _basic_std_via_python(local_arr_2, axis=1, comm=comm)
     full_ex2_ax1_std = np.std(global_arr_2, axis=1)
     exp_ex2_ax1 = full_ex2_ax1_std[slices[rank][0]:slices[rank][1]]
     assert np.allclose(res_ex2_ax1, exp_ex2_ax1)
 
     # Example 3
     local_arr_3, global_arr_3 = test_utils.generate_local_and_global_arrays_from_example_impl(rank, slices, example=3)
-
     res_ex3_ax0 = _basic_std_via_python(local_arr_3, axis=0, comm=comm)
-    exp_ex3_ax0 = np.std(global_arr_3, axis=0)
+    full_ex3_ax0_std = np.std(global_arr_3, axis=0)
+    exp_ex3_ax0 = full_ex3_ax0_std[slices[rank][0]:slices[rank][1],:]
     assert np.allclose(res_ex3_ax0, exp_ex3_ax0)
 
-    res_ex3_ax1 = _basic_std_via_python(local_arr_3, axis=1, comm=comm)
-    full_ex3_ax1_std = np.std(global_arr_3, axis=1)
-    exp_ex3_ax1 = full_ex3_ax1_std[slices[rank][0]:slices[rank][1],:]
+    res_ex3_ax1 = _basic_std_via_python(local_arr_3, axis=1, testing=True, comm=comm)
+    exp_ex3_ax1 = np.std(global_arr_3, axis=1)
     assert np.allclose(res_ex3_ax1, exp_ex3_ax1)
 
     res_ex3_ax2 = _basic_std_via_python(local_arr_3, axis=2, comm=comm)
     full_ex3_ax2_std = np.std(global_arr_3, axis=2)
-    exp_ex3_ax2 = full_ex3_ax2_std[slices[rank][0]:slices[rank][1],:]
+    exp_ex3_ax2 = full_ex3_ax2_std[:,slices[rank][0]:slices[rank][1]]
     assert np.allclose(res_ex3_ax2, exp_ex3_ax2)
 
 @pytest.mark.mpi(min_size=3)
 def test_python_std_vector_mpi():
     comm = MPI.COMM_WORLD
     result, expected = _std_setup(ndim=1, comm=comm)
     np.testing.assert_almost_equal(result, expected, decimal=10)
 
 @pytest.mark.mpi(min_size=3)
 def test_python_std_array_mpi():
     comm = MPI.COMM_WORLD
     result_01, expected_01 = _std_setup(ndim=2, dtype=np.float32, comm=comm)
     assert np.allclose(result_01, expected_01)
 
-    result_02, expected_02 = _std_setup(ndim=3, ddof=1, comm=comm)
+    result_02, expected_02 = _std_setup(ndim=3, comm=comm)
     assert np.allclose(result_02, expected_02)
 
 @pytest.mark.mpi(min_size=3)
 def test_python_std_array_axis_mpi():
     comm = MPI.COMM_WORLD
     result_01, expected_01 = _std_setup(ndim=2, dtype=np.float32, axis=0, comm=comm)
-    print("result_01")
-    print(result_01)
-    print("expected_01")
-    print(expected_01)
-
     assert np.allclose(result_01, expected_01)
 
     result_02, expected_02 = _std_setup(ndim=2, dtype=np.float32, axis=1, comm=comm)
     assert len(np.setdiff1d(result_02, expected_02)) == 0
 
-    result_03, expected_03 = _std_setup(ndim=3, ddof=1, axis=2, comm=comm)
+    result_03, expected_03 = _std_setup(ndim=3, axis=2, comm=comm)
     assert len(np.setdiff1d(result_03, expected_03)) == 0
 
 def test_python_std_serial():
     vector = np.random.rand(10)
     np.testing.assert_almost_equal(_basic_std_via_python(vector), np.std(vector), decimal=10)
 
     array = np.random.rand(3, 10)
```

### Comparing `pressio-linalg-0.1.0rc6/tests/test_basic_svd_method_of_snapshots_via_python.py` & `pressio-linalg-0.1.0rc7/tests/test_basic_svd_method_of_snapshots_via_python.py`

 * *Files identical despite different names*

