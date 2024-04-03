# Comparing `tmp/nwpeval-1.4.0.tar.gz` & `tmp/nwpeval-1.5.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nwpeval-1.4.0.tar", last modified: Tue Apr  2 07:21:31 2024, max compression
+gzip compressed data, was "nwpeval-1.5.0b2.tar", last modified: Wed Apr  3 19:59:08 2024, max compression
```

## Comparing `nwpeval-1.4.0.tar` & `nwpeval-1.5.0b2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 dev        (501) staff       (20)        0 2024-04-02 07:21:31.497841 nwpeval-1.4.0/
--rw-r--r--   0 dev        (501) staff       (20)      739 2024-04-02 07:21:31.497667 nwpeval-1.4.0/PKG-INFO
--rw-r--r--   0 dev        (501) staff       (20)     4624 2024-04-02 06:56:12.000000 nwpeval-1.4.0/README.md
-drwxr-xr-x   0 dev        (501) staff       (20)        0 2024-04-02 07:21:31.496860 nwpeval-1.4.0/nwpeval/
--rw-r--r--   0 dev        (501) staff       (20)       30 2024-04-02 04:51:47.000000 nwpeval-1.4.0/nwpeval/__init__.py
--rw-r--r--   0 dev        (501) staff       (20)    57993 2024-04-02 04:51:09.000000 nwpeval-1.4.0/nwpeval/nwpeval.py
--rw-r--r--   0 dev        (501) staff       (20)      624 2024-04-01 07:19:46.000000 nwpeval-1.4.0/nwpeval/utils.py
-drwxr-xr-x   0 dev        (501) staff       (20)        0 2024-04-02 07:21:31.497497 nwpeval-1.4.0/nwpeval.egg-info/
--rw-r--r--   0 dev        (501) staff       (20)      739 2024-04-02 07:21:31.000000 nwpeval-1.4.0/nwpeval.egg-info/PKG-INFO
--rw-r--r--   0 dev        (501) staff       (20)      228 2024-04-02 07:21:31.000000 nwpeval-1.4.0/nwpeval.egg-info/SOURCES.txt
--rw-r--r--   0 dev        (501) staff       (20)        1 2024-04-02 07:21:31.000000 nwpeval-1.4.0/nwpeval.egg-info/dependency_links.txt
--rw-r--r--   0 dev        (501) staff       (20)       26 2024-04-02 07:21:31.000000 nwpeval-1.4.0/nwpeval.egg-info/requires.txt
--rw-r--r--   0 dev        (501) staff       (20)        8 2024-04-02 07:21:31.000000 nwpeval-1.4.0/nwpeval.egg-info/top_level.txt
--rw-r--r--   0 dev        (501) staff       (20)       38 2024-04-02 07:21:31.497877 nwpeval-1.4.0/setup.cfg
--rw-r--r--   0 dev        (501) staff       (20)      864 2024-04-02 07:18:52.000000 nwpeval-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:59:08.574311 nwpeval-1.5.0b2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-03 19:59:02.000000 nwpeval-1.5.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11054 2024-04-03 19:59:08.574311 nwpeval-1.5.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10159 2024-04-03 19:59:02.000000 nwpeval-1.5.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:59:08.574311 nwpeval-1.5.0b2/nwpeval/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-03 19:59:02.000000 nwpeval-1.5.0b2/nwpeval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58416 2024-04-03 19:59:02.000000 nwpeval-1.5.0b2/nwpeval/nwpeval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-03 19:59:02.000000 nwpeval-1.5.0b2/nwpeval/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:59:08.574311 nwpeval-1.5.0b2/nwpeval.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11054 2024-04-03 19:59:08.000000 nwpeval-1.5.0b2/nwpeval.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-03 19:59:08.000000 nwpeval-1.5.0b2/nwpeval.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:59:08.000000 nwpeval-1.5.0b2/nwpeval.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-03 19:59:08.000000 nwpeval-1.5.0b2/nwpeval.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 19:59:08.000000 nwpeval-1.5.0b2/nwpeval.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:59:08.574311 nwpeval-1.5.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-03 19:59:02.000000 nwpeval-1.5.0b2/setup.py
```

### Comparing `nwpeval-1.4.0/nwpeval/nwpeval.py` & `nwpeval-1.5.0b2/nwpeval/nwpeval.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,24 @@
 import numpy as np
 import xarray as xr
+import pandas as pd
 from scipy.stats import pearsonr
+import matplotlib.pyplot as plt
+
+
+def help(cls):
+    print("Available methods in the NWP_Stats class:")
+    print("-------------------------------------------")
+    for method_name in dir(cls):
+        if method_name.startswith("compute_"):
+            method = getattr(cls, method_name)
+            print(f"{method_name}:")
+            print(method.__doc__)
+            print("---")
+
 
 class NWP_Stats:
     def __init__(self, obs_data, model_data):
         """
         Initialize the NWPMetrics object with observed and modeled data.
         
         Args:
@@ -1384,8 +1398,10 @@
             xarray.DataArray: The computed Tsallis Divergence values.
         """
         obs_prob = self.obs_data / self.obs_data.sum(dim=dim)
         model_prob = self.model_data / self.model_data.sum(dim=dim)
         return (1 / (alpha - 1)) * ((obs_prob ** alpha / model_prob ** (alpha - 1)).sum(dim=dim) - 1)
     
     
-    #Further addition to the code. 
+    #Further addition of metrics to the code. 
+    
+
```

