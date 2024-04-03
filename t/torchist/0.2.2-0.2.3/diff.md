# Comparing `tmp/torchist-0.2.2.tar.gz` & `tmp/torchist-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchist-0.2.2.tar", last modified: Wed Nov 29 15:23:18 2023, max compression
+gzip compressed data, was "torchist-0.2.3.tar", last modified: Wed Apr  3 14:48:44 2024, max compression
```

## Comparing `torchist-0.2.2.tar` & `torchist-0.2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 francois  (1000) francois  (1000)        0 2023-11-29 15:23:18.769453 torchist-0.2.2/
--rw-r--r--   0 francois  (1000) francois  (1000)     1072 2023-11-29 12:55:29.000000 torchist-0.2.2/LICENSE
--rw-r--r--   0 francois  (1000) francois  (1000)     2345 2023-11-29 15:23:18.769453 torchist-0.2.2/PKG-INFO
--rw-r--r--   0 francois  (1000) francois  (1000)     1762 2023-11-29 12:55:29.000000 torchist-0.2.2/README.md
--rw-r--r--   0 francois  (1000) francois  (1000)       13 2023-11-29 12:55:29.000000 torchist-0.2.2/requirements.txt
--rw-r--r--   0 francois  (1000) francois  (1000)      659 2023-11-29 15:23:18.769453 torchist-0.2.2/setup.cfg
--rw-r--r--   0 francois  (1000) francois  (1000)       76 2023-11-29 12:55:29.000000 torchist-0.2.2/setup.py
-drwxr-xr-x   0 francois  (1000) francois  (1000)        0 2023-11-29 15:23:18.769453 torchist-0.2.2/torchist/
--rw-r--r--   0 francois  (1000) francois  (1000)    12995 2023-11-29 15:19:19.000000 torchist-0.2.2/torchist/__init__.py
--rw-r--r--   0 francois  (1000) francois  (1000)     4140 2023-11-29 12:55:29.000000 torchist-0.2.2/torchist/metrics.py
-drwxr-xr-x   0 francois  (1000) francois  (1000)        0 2023-11-29 15:23:18.769453 torchist-0.2.2/torchist.egg-info/
--rw-r--r--   0 francois  (1000) francois  (1000)     2345 2023-11-29 15:23:18.000000 torchist-0.2.2/torchist.egg-info/PKG-INFO
--rw-r--r--   0 francois  (1000) francois  (1000)      253 2023-11-29 15:23:18.000000 torchist-0.2.2/torchist.egg-info/SOURCES.txt
--rw-r--r--   0 francois  (1000) francois  (1000)        1 2023-11-29 15:23:18.000000 torchist-0.2.2/torchist.egg-info/dependency_links.txt
--rw-r--r--   0 francois  (1000) francois  (1000)       13 2023-11-29 15:23:18.000000 torchist-0.2.2/torchist.egg-info/requires.txt
--rw-r--r--   0 francois  (1000) francois  (1000)        9 2023-11-29 15:23:18.000000 torchist-0.2.2/torchist.egg-info/top_level.txt
+drwxrwxr-x   0 francois  (1000) francois  (1000)        0 2024-04-03 14:48:44.027745 torchist-0.2.3/
+-rw-r--r--   0 francois  (1000) francois  (1000)     1072 2023-11-29 12:55:29.000000 torchist-0.2.3/LICENSE
+-rw-r--r--   0 francois  (1000) francois  (1000)     2345 2024-04-03 14:48:44.027745 torchist-0.2.3/PKG-INFO
+-rw-r--r--   0 francois  (1000) francois  (1000)     1762 2023-11-29 12:55:29.000000 torchist-0.2.3/README.md
+-rw-r--r--   0 francois  (1000) francois  (1000)       13 2023-11-29 12:55:29.000000 torchist-0.2.3/requirements.txt
+-rw-r--r--   0 francois  (1000) francois  (1000)      659 2024-04-03 14:48:44.027745 torchist-0.2.3/setup.cfg
+-rw-r--r--   0 francois  (1000) francois  (1000)       76 2023-11-29 12:55:29.000000 torchist-0.2.3/setup.py
+drwxrwxr-x   0 francois  (1000) francois  (1000)        0 2024-04-03 14:48:44.027745 torchist-0.2.3/torchist/
+-rw-rw-r--   0 francois  (1000) francois  (1000)    13583 2024-04-03 14:46:07.000000 torchist-0.2.3/torchist/__init__.py
+-rw-r--r--   0 francois  (1000) francois  (1000)     4140 2023-11-29 12:55:29.000000 torchist-0.2.3/torchist/metrics.py
+drwxrwxr-x   0 francois  (1000) francois  (1000)        0 2024-04-03 14:48:44.027745 torchist-0.2.3/torchist.egg-info/
+-rw-r--r--   0 francois  (1000) francois  (1000)     2345 2024-04-03 14:48:44.000000 torchist-0.2.3/torchist.egg-info/PKG-INFO
+-rw-rw-r--   0 francois  (1000) francois  (1000)      253 2024-04-03 14:48:44.000000 torchist-0.2.3/torchist.egg-info/SOURCES.txt
+-rw-rw-r--   0 francois  (1000) francois  (1000)        1 2024-04-03 14:48:44.000000 torchist-0.2.3/torchist.egg-info/dependency_links.txt
+-rw-rw-r--   0 francois  (1000) francois  (1000)       13 2024-04-03 14:48:44.000000 torchist-0.2.3/torchist.egg-info/requires.txt
+-rw-rw-r--   0 francois  (1000) francois  (1000)        9 2024-04-03 14:48:44.000000 torchist-0.2.3/torchist.egg-info/top_level.txt
```

### Comparing `torchist-0.2.2/LICENSE` & `torchist-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `torchist-0.2.2/PKG-INFO` & `torchist-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchist
-Version: 0.2.2
+Version: 0.2.3
 Summary: NumPy-style histograms in PyTorch
 Home-page: https://github.com/francois-rozet/torchist
 Author: François Rozet
 Author-email: francois.rozet@outlook.com
 Keywords: torch,histogram
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `torchist-0.2.2/README.md` & `torchist-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `torchist-0.2.2/setup.cfg` & `torchist-0.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `torchist-0.2.2/torchist/__init__.py` & `torchist-0.2.3/torchist/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 r"""NumPy-style histograms in PyTorch"""
 
-__version__ = '0.2.2'
+__version__ = '0.2.3'
 
 import torch
 
 from torch import Size, Tensor, BoolTensor
 from typing import *
 
 
@@ -120,15 +120,15 @@
 
     Returns:
         The histogram, (*bins,).
     """
 
     # Preprocess
     D = x.size(-1)
-    x = x.reshape(-1, D).squeeze(-1)
+    x = x.reshape(-1, D)
 
     if edges is None:
         bounded = bounded or (low is None and upp is None)
 
         if low is None:
             low = x.min(dim=0).values
 
@@ -190,16 +190,15 @@
             idx, inverse = torch.unique(idx, dim=0, return_inverse=True)
             values = weights.new_zeros(len(idx))
             values = values.scatter_add(dim=0, index=inverse, src=weights)
 
         hist = torch.sparse_coo_tensor(idx.t(), values, shape)
         hist._coalesced_(True)
     else:
-        if D > 1:
-            idx = ravel_multi_index(idx, shape)
+        idx = ravel_multi_index(idx, shape)
         hist = idx.bincount(weights, minlength=shape.numel()).reshape(shape)
 
     return hist
 
 
 def histogramdd_edges(
     x: Tensor,
@@ -396,14 +395,26 @@
     edges100 = np.linspace(0.0, 1.0, 101) ** 1.5
 
     x_t = torch.from_numpy(x)
     xdd_t = torch.from_numpy(xdd)
     edges10_t = torch.from_numpy(edges10)
     edges100_t = torch.from_numpy(edges100)
 
+    ## Correctness
+    hdd, _ = np.histogramdd(xdd, bins=10)
+    hdd_t = histogramdd(xdd_t, bins=10)
+
+    assert np.all(hdd == hdd_t.numpy())
+
+    hdd, _ = np.histogramdd(xdd, bins=[edges10] * 5)
+    hdd_t = histogramdd(xdd_t, edges=[edges10_t] * 5)
+
+    assert np.all(hdd == hdd_t.numpy())
+
+    ## Speed
     for key, f in {
         'np.histogram': lambda: np.histogram(x, bins=100),
         'np.histogramdd': lambda: np.histogramdd(xdd, bins=10),
         'np.histogram (non-uniform)': lambda: np.histogram(x, bins=edges100),
         'np.histogramdd (non-uniform)': lambda: np.histogramdd(xdd, bins=[edges10] * 5),
         'torchist.histogram': lambda: histogram(x_t, bins=100),
         'torchist.histogramdd': lambda: histogramdd(xdd_t, bins=10),
@@ -421,14 +432,26 @@
     print('----')
 
     x_t = x_t.cuda()
     xdd_t = xdd_t.cuda()
     edges10_t = edges10_t.cuda()
     edges100_t = edges100_t.cuda()
 
+    ## Correctness
+    hdd, _ = np.histogramdd(xdd, bins=10)
+    hdd_t = histogramdd(xdd_t, bins=10)
+
+    assert np.all(hdd == hdd_t.cpu().numpy())
+
+    hdd, _ = np.histogramdd(xdd, bins=[edges10] * 5)
+    hdd_t = histogramdd(xdd_t, edges=[edges10_t] * 5)
+
+    assert np.all(hdd == hdd_t.cpu().numpy())
+
+    ## Speed
     for key, f in {
         'torchist.histogram': lambda: histogram(x_t, bins=100),
         'torchist.histogramdd': lambda: histogramdd(xdd_t, bins=10),
         'torchist.histogram (non-uniform)': lambda: histogram(x_t, edges=edges100_t),
         'torchist.histogramdd (non-uniform)': lambda: histogramdd(xdd_t, edges=[edges10_t] * 5),
     }.items():
         start = torch.cuda.Event(enable_timing=True)
```

### Comparing `torchist-0.2.2/torchist/metrics.py` & `torchist-0.2.3/torchist/metrics.py`

 * *Files identical despite different names*

### Comparing `torchist-0.2.2/torchist.egg-info/PKG-INFO` & `torchist-0.2.3/torchist.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchist
-Version: 0.2.2
+Version: 0.2.3
 Summary: NumPy-style histograms in PyTorch
 Home-page: https://github.com/francois-rozet/torchist
 Author: François Rozet
 Author-email: francois.rozet@outlook.com
 Keywords: torch,histogram
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

