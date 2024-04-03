# Comparing `tmp/defect_detection-0.1.0.tar.gz` & `tmp/defect_detection-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "defect_detection-0.1.0.tar", last modified: Tue Apr  2 08:42:33 2024, max compression
+gzip compressed data, was "defect_detection-0.2.0.tar", last modified: Wed Apr  3 02:54:48 2024, max compression
```

## Comparing `defect_detection-0.1.0.tar` & `defect_detection-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:42:33.156568 defect_detection-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-02 08:42:29.000000 defect_detection-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-02 08:42:29.000000 defect_detection-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-04-02 08:42:33.156568 defect_detection-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-02 08:42:29.000000 defect_detection-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-02 08:42:29.000000 defect_detection-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 08:42:33.156568 defect_detection-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:42:33.156568 defect_detection-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:42:33.156568 defect_detection-0.1.0/src/defect_detection/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-02 08:42:29.000000 defect_detection-0.1.0/src/defect_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8977 2024-04-02 08:42:29.000000 defect_detection-0.1.0/src/defect_detection/deep_AE.py
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-02 08:42:29.000000 defect_detection-0.1.0/src/defect_detection/filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-02 08:42:29.000000 defect_detection-0.1.0/src/defect_detection/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7975 2024-04-02 08:42:29.000000 defect_detection-0.1.0/src/defect_detection/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-02 08:42:33.000000 defect_detection-0.1.0/src/defect_detection/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:42:33.156568 defect_detection-0.1.0/src/defect_detection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-04-02 08:42:33.000000 defect_detection-0.1.0/src/defect_detection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-02 08:42:33.000000 defect_detection-0.1.0/src/defect_detection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 08:42:33.000000 defect_detection-0.1.0/src/defect_detection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-02 08:42:33.000000 defect_detection-0.1.0/src/defect_detection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-02 08:42:33.000000 defect_detection-0.1.0/src/defect_detection.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:54:48.945947 defect_detection-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-03 02:54:44.000000 defect_detection-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-03 02:54:44.000000 defect_detection-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-03 02:54:48.945947 defect_detection-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-03 02:54:44.000000 defect_detection-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-03 02:54:44.000000 defect_detection-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 02:54:48.945947 defect_detection-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:54:48.941947 defect_detection-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:54:48.941947 defect_detection-0.2.0/src/defect_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-03 02:54:44.000000 defect_detection-0.2.0/src/defect_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9650 2024-04-03 02:54:44.000000 defect_detection-0.2.0/src/defect_detection/deep_AE.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-03 02:54:44.000000 defect_detection-0.2.0/src/defect_detection/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-03 02:54:44.000000 defect_detection-0.2.0/src/defect_detection/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7945 2024-04-03 02:54:44.000000 defect_detection-0.2.0/src/defect_detection/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-03 02:54:48.000000 defect_detection-0.2.0/src/defect_detection/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:54:48.945947 defect_detection-0.2.0/src/defect_detection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-03 02:54:48.000000 defect_detection-0.2.0/src/defect_detection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-03 02:54:48.000000 defect_detection-0.2.0/src/defect_detection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:54:48.000000 defect_detection-0.2.0/src/defect_detection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 02:54:48.000000 defect_detection-0.2.0/src/defect_detection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-03 02:54:48.000000 defect_detection-0.2.0/src/defect_detection.egg-info/top_level.txt
```

### Comparing `defect_detection-0.1.0/LICENSE` & `defect_detection-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `defect_detection-0.1.0/PKG-INFO` & `defect_detection-0.2.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: defect_detection
-Version: 0.1.0
+Version: 0.2.0
 Summary: API for defect detection in PCB and other components.
 Author-email: Louis Vaslin <lovaslin@post.kek.jp>
 Maintainer-email: Louis Vaslin <lovaslin@post.kek.jp>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Louis VASLIN
         
@@ -56,21 +56,43 @@
 Requires-Dist: opencv-python
 Requires-Dist: numpy
 Requires-Dist: torch
 Requires-Dist: scikit-learn
 
 # defect_detection
 
+[![PyPI](https://img.shields.io/pypi/v/defect_detection)](https://pypi.org/project/defect_detection/)
+[![Build](https://github.com/lovaslin/defect_detection/actions/workflows/cd.yml/badge.svg)](https://github.com/lovaslin/defect_detection/actions)
+
 This packge provides a basic API to implement defect detection algorithms. 
-These algorithms can be tune in order to automatically detect any defect in a PCB or other components.
+These algorithms can be tune in order to automatically detect any defects in a PCB or other components.
 
 ## Requirement
 
+The following package are required :
+- numpy
+- opencv-python
+- torch
+- scikit-learn
+
+Recommended python version >= 3.8
+
+## Installation
+
+To install the latest stable release from PyPI :
+```bash
+pip install defect_detection
+```
+
+For developper who wants to work with a local and editable version :
+```bash
+git clone https://github.com/lovaslin/defect_detection.git
+cd defect_detection
+pip install -e .
+```
 
-
-## Instalation
-
-
+For the local install, you should of course run the commands using a clean python environment.
+I recommend to use `venv` to setup a pip-friendly environemnt.
 
 ## Usage
```

### Comparing `defect_detection-0.1.0/pyproject.toml` & `defect_detection-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `defect_detection-0.1.0/src/defect_detection/deep_AE.py` & `defect_detection-0.2.0/src/defect_detection/deep_AE.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 class AE_cls(torch.nn.Module):
     '''
     Class inplementing the deep AE architecture using pyTorch.
     Provides also methods for training and appalying model using input batches.
     '''
     
     # Initialization method
-    def __init__(self, p, apply_only=False loss_fn=None, opt=None, opt_param=None):
+    def __init__(self, p, apply_only=False, loss_fn=None, opt=None, opt_param=None):
         '''
         Arguments :
             p : dict()
                 Python dict containing all the information about the AE architecture.
             
-            apply_only : (boolean)
+            apply_only : (bool)
                 Specify if the model is used only for application (default: False).
                 Note that the training method is not usable if set to True.
             
             loss_fn : (function)
                 The loss function used to train the model.
                 Must be compatible with torch API.
                 If you plan to use event weights, use a loss that returns one value per individual inputs.
@@ -128,14 +128,38 @@
             self.loss_fn = loss_fn
             if opt_param is None:
                 opt_param = dict()
             self.opt = opt(self.parameters(), **opt_param)
         
         return
     
+    # Device selection method (includes automatic selection)
+    def to_dev(self, dev):
+        '''
+        Select the device torch should use for this model.
+        Supports automatic selection.
+        
+        Arguments :
+            dev : (str)
+                Specify the device to use for this model.
+                Supported values are 'cuda', 'cpu' and 'auto'.
+        '''
+        # Check if auto
+        if dev=='auto':
+            # Check if cuda is available
+            if torch.cuda.is_available():
+                dev = 'cuda'
+            else:
+                dev = 'cpu'
+        
+        # Set device
+        self.to(dev)
+        
+        return
+    
     # Forward pass method (internal use only)
     def forward(self, x):
         '''
         Return the output of the model given input x.
         '''
         return self.decoder(self.encoder(x))
     
@@ -219,19 +243,19 @@
                 Path to the directory in which save files are created.
         '''
         # Check if path exits and try to create it if not
         if not os.path.exists(path):
             os.mkdir(path, 0o755)
         
         # Save config in text file
-        with open(path + 'config.txt', 'w') as f:
+        with open(path + 'AE_config.txt', 'w') as f:
             print(self.config, file=f)
         
         # Save state_dict
-        torch.save(self.state_dict(), path + 'state.save')
+        torch.save(self.state_dict(), path + 'AE_state.save')
         
         return
     
     ##END OF AE_cls##
```

### Comparing `defect_detection-0.1.0/src/defect_detection/filtering.py` & `defect_detection-0.2.0/src/defect_detection/filtering.py`

 * *Files identical despite different names*

### Comparing `defect_detection-0.1.0/src/defect_detection/preprocessing.py` & `defect_detection-0.2.0/src/defect_detection/preprocessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 ## Includes data augmentation and image spliting.                                     ##
 ## This function can be used to generate a training dataset for a new model.          ##
 ########################################################################################
 
 
 import numpy as np
 import cv2 as cv
-import matplotlib.pyplot as plt
 from torch.cuda import is_available as cuda_check
 import os
 import sys
 import getopt
 import itertools
 import concurrent.futures as thd
 
@@ -107,15 +106,15 @@
         'Ncore': Ncore,
         'seed': seed
     }
     with open(param['opath'] + param['name'] + '.txt', 'w') as f:
         print(param, file=f)
     
     print('Preprocessing parameters :')
-    for k, i in param.items()
+    for k, i in param.items():
         print(f'\t{k} : {i}')
     
     # Load initial croping if needed
     if param['fcrop'] is not None:
         with open(param['fcrop'], 'r') as f:
             cr = eval(f.read())
     else:
@@ -224,15 +223,15 @@
         im : (numpy array)
             The image in numpy array format.
         dev : (str)
             Define the device that torch should use to handle the tensor.
             Support 'CPU', 'cuda' and 'auto'.
     '''
     # Device automatic selection (if needed)
-    if dev = 'auto':
+    if dev == 'auto':
         # Check for CUDA availability
         if cuda_check:
             dev = 'cuda'
         else:
             dev = 'cpu'
     
     # Type conversion (to float image)
```

### Comparing `defect_detection-0.1.0/src/defect_detection.egg-info/PKG-INFO` & `defect_detection-0.2.0/src/defect_detection.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: defect_detection
-Version: 0.1.0
+Version: 0.2.0
 Summary: API for defect detection in PCB and other components.
 Author-email: Louis Vaslin <lovaslin@post.kek.jp>
 Maintainer-email: Louis Vaslin <lovaslin@post.kek.jp>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Louis VASLIN
         
@@ -56,21 +56,43 @@
 Requires-Dist: opencv-python
 Requires-Dist: numpy
 Requires-Dist: torch
 Requires-Dist: scikit-learn
 
 # defect_detection
 
+[![PyPI](https://img.shields.io/pypi/v/defect_detection)](https://pypi.org/project/defect_detection/)
+[![Build](https://github.com/lovaslin/defect_detection/actions/workflows/cd.yml/badge.svg)](https://github.com/lovaslin/defect_detection/actions)
+
 This packge provides a basic API to implement defect detection algorithms. 
-These algorithms can be tune in order to automatically detect any defect in a PCB or other components.
+These algorithms can be tune in order to automatically detect any defects in a PCB or other components.
 
 ## Requirement
 
+The following package are required :
+- numpy
+- opencv-python
+- torch
+- scikit-learn
+
+Recommended python version >= 3.8
+
+## Installation
+
+To install the latest stable release from PyPI :
+```bash
+pip install defect_detection
+```
+
+For developper who wants to work with a local and editable version :
+```bash
+git clone https://github.com/lovaslin/defect_detection.git
+cd defect_detection
+pip install -e .
+```
 
-
-## Instalation
-
-
+For the local install, you should of course run the commands using a clean python environment.
+I recommend to use `venv` to setup a pip-friendly environemnt.
 
 ## Usage
```

