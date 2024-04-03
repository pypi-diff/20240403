# Comparing `tmp/defect_detection-0.2.0.tar.gz` & `tmp/defect_detection-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "defect_detection-0.2.0.tar", last modified: Wed Apr  3 02:54:48 2024, max compression
+gzip compressed data, was "defect_detection-0.2.1.tar", last modified: Wed Apr  3 06:19:44 2024, max compression
```

## Comparing `defect_detection-0.2.0.tar` & `defect_detection-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:54:48.945947 defect_detection-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-03 02:54:44.000000 defect_detection-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-03 02:54:44.000000 defect_detection-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-03 02:54:48.945947 defect_detection-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-03 02:54:44.000000 defect_detection-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-03 02:54:44.000000 defect_detection-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 02:54:48.945947 defect_detection-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:54:48.941947 defect_detection-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:54:48.941947 defect_detection-0.2.0/src/defect_detection/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-03 02:54:44.000000 defect_detection-0.2.0/src/defect_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9650 2024-04-03 02:54:44.000000 defect_detection-0.2.0/src/defect_detection/deep_AE.py
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-03 02:54:44.000000 defect_detection-0.2.0/src/defect_detection/filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-03 02:54:44.000000 defect_detection-0.2.0/src/defect_detection/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7945 2024-04-03 02:54:44.000000 defect_detection-0.2.0/src/defect_detection/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-03 02:54:48.000000 defect_detection-0.2.0/src/defect_detection/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:54:48.945947 defect_detection-0.2.0/src/defect_detection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-03 02:54:48.000000 defect_detection-0.2.0/src/defect_detection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-03 02:54:48.000000 defect_detection-0.2.0/src/defect_detection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:54:48.000000 defect_detection-0.2.0/src/defect_detection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 02:54:48.000000 defect_detection-0.2.0/src/defect_detection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-03 02:54:48.000000 defect_detection-0.2.0/src/defect_detection.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:19:44.700165 defect_detection-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-03 06:19:40.000000 defect_detection-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-03 06:19:40.000000 defect_detection-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-03 06:19:44.700165 defect_detection-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-03 06:19:40.000000 defect_detection-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-03 06:19:40.000000 defect_detection-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 06:19:44.700165 defect_detection-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:19:44.696165 defect_detection-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:19:44.700165 defect_detection-0.2.1/src/defect_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-03 06:19:40.000000 defect_detection-0.2.1/src/defect_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9650 2024-04-03 06:19:40.000000 defect_detection-0.2.1/src/defect_detection/deep_AE.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-03 06:19:40.000000 defect_detection-0.2.1/src/defect_detection/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-03 06:19:40.000000 defect_detection-0.2.1/src/defect_detection/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-04-03 06:19:40.000000 defect_detection-0.2.1/src/defect_detection/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-03 06:19:44.000000 defect_detection-0.2.1/src/defect_detection/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:19:44.700165 defect_detection-0.2.1/src/defect_detection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-03 06:19:44.000000 defect_detection-0.2.1/src/defect_detection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-03 06:19:44.000000 defect_detection-0.2.1/src/defect_detection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 06:19:44.000000 defect_detection-0.2.1/src/defect_detection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 06:19:44.000000 defect_detection-0.2.1/src/defect_detection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-03 06:19:44.000000 defect_detection-0.2.1/src/defect_detection.egg-info/top_level.txt
```

### Comparing `defect_detection-0.2.0/LICENSE` & `defect_detection-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `defect_detection-0.2.0/PKG-INFO` & `defect_detection-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: defect_detection
-Version: 0.2.0
+Version: 0.2.1
 Summary: API for defect detection in PCB and other components.
 Author-email: Louis Vaslin <lovaslin@post.kek.jp>
 Maintainer-email: Louis Vaslin <lovaslin@post.kek.jp>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Louis VASLIN
```

### Comparing `defect_detection-0.2.0/README.md` & `defect_detection-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `defect_detection-0.2.0/pyproject.toml` & `defect_detection-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `defect_detection-0.2.0/src/defect_detection/deep_AE.py` & `defect_detection-0.2.1/src/defect_detection/deep_AE.py`

 * *Files identical despite different names*

### Comparing `defect_detection-0.2.0/src/defect_detection/filtering.py` & `defect_detection-0.2.1/src/defect_detection/filtering.py`

 * *Files 18% similar despite different names*

```diff
@@ -32,21 +32,21 @@
     
     # Add the pix_th criteria
     if pix_th:
         # Remove small cluster and remove noisy labels
         lab, count = np.unique(fil, return_counts=True)
         lab = lab[1:]
         count = count[1:]
-        pix2 = pix[np.isin(fil, lab[count >= pix_th])] #FIXME store and return both raw and clean list for testing
+        pix = pix[np.isin(fil, lab[count >= pix_th])]
         del lab
         del count
     else:
         # Only filter out noisy labels
-        pix2 = pix[fil > -1] #FIXME store and return both raw and clean list for testing
+        pix = pix[fil > -1]
     
     # Return the filtered pixel list
-    return pix, pix2
+    return pix
```

### Comparing `defect_detection-0.2.0/src/defect_detection/functions.py` & `defect_detection-0.2.1/src/defect_detection/functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 import torch
 from .deep_AE import AE_cls
 
 
 # Error map using mean
 def emap_mean(x, y):
-    return torch.mean(torch.square(x - y), (0))
+    return torch.mean(torch.square(x - y), (0)).detach().to('cpu').numpy()
 
 # Error map using sum
 def emap_sum(x, y):
-    return torch.mean(torch.square(x - y), (0))
+    return torch.sum(torch.square(x - y), (0)).detach().to('cpu').numpy()
 
 # Load a trained model
 def deepAE_load(path, use_only=True, loss_fn=None, opt=None, opt_param=None):
     '''
     Function to load a trained deepAE model.
     
     Arguments :
```

### Comparing `defect_detection-0.2.0/src/defect_detection/preprocessing.py` & `defect_detection-0.2.1/src/defect_detection/preprocessing.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ## Includes data augmentation and image spliting.                                     ##
 ## This function can be used to generate a training dataset for a new model.          ##
 ########################################################################################
 
 
 import numpy as np
 import cv2 as cv
-from torch.cuda import is_available as cuda_check
+import torch
 import os
 import sys
 import getopt
 import itertools
 import concurrent.futures as thd
 
 
@@ -225,15 +225,15 @@
         dev : (str)
             Define the device that torch should use to handle the tensor.
             Support 'CPU', 'cuda' and 'auto'.
     '''
     # Device automatic selection (if needed)
     if dev == 'auto':
         # Check for CUDA availability
-        if cuda_check:
+        if torch.cuda.is_available():
             dev = 'cuda'
         else:
             dev = 'cpu'
     
     # Type conversion (to float image)
     im = im.astype(np.float32)
     im = im / 255.
```

### Comparing `defect_detection-0.2.0/src/defect_detection.egg-info/PKG-INFO` & `defect_detection-0.2.1/src/defect_detection.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: defect_detection
-Version: 0.2.0
+Version: 0.2.1
 Summary: API for defect detection in PCB and other components.
 Author-email: Louis Vaslin <lovaslin@post.kek.jp>
 Maintainer-email: Louis Vaslin <lovaslin@post.kek.jp>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Louis VASLIN
```

