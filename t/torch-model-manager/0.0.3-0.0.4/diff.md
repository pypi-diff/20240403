# Comparing `tmp/torch-model-manager-0.0.3.tar.gz` & `tmp/torch-model-manager-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch-model-manager-0.0.3.tar", last modified: Tue Apr  2 22:23:04 2024, max compression
+gzip compressed data, was "torch-model-manager-0.0.4.tar", last modified: Tue Apr  2 22:26:03 2024, max compression
```

## Comparing `torch-model-manager-0.0.3.tar` & `torch-model-manager-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 22:23:04.970721 torch-model-manager-0.0.3/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2751 2024-04-02 22:23:04.970721 torch-model-manager-0.0.3/PKG-INFO
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2233 2024-04-02 22:21:42.000000 torch-model-manager-0.0.3/README.md
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-04-02 22:23:04.970721 torch-model-manager-0.0.3/setup.cfg
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      844 2024-04-02 22:21:26.000000 torch-model-manager-0.0.3/setup.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 22:23:04.926720 torch-model-manager-0.0.3/tests/
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 22:23:04.930720 torch-model-manager-0.0.3/tests/test_torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 16:34:05.000000 torch-model-manager-0.0.3/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-02 21:24:16.000000 torch-model-manager-0.0.3/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 22:23:04.938720 torch-model-manager-0.0.3/tests/test_utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 16:34:05.000000 torch-model-manager-0.0.3/tests/test_utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-02 16:34:05.000000 torch-model-manager-0.0.3/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 22:23:04.954720 torch-model-manager-0.0.3/torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       50 2024-04-02 21:41:02.000000 torch-model-manager-0.0.3/torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    11669 2024-04-02 16:34:05.000000 torch-model-manager-0.0.3/torch_model_manager/torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 22:23:04.970721 torch-model-manager-0.0.3/torch_model_manager.egg-info/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2751 2024-04-02 22:23:04.000000 torch-model-manager-0.0.3/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      471 2024-04-02 22:23:04.000000 torch-model-manager-0.0.3/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-04-02 22:23:04.000000 torch-model-manager-0.0.3/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       30 2024-04-02 22:23:04.000000 torch-model-manager-0.0.3/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       26 2024-04-02 22:23:04.000000 torch-model-manager-0.0.3/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 22:26:03.880429 torch-model-manager-0.0.4/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2746 2024-04-02 22:26:03.880429 torch-model-manager-0.0.4/PKG-INFO
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2228 2024-04-02 22:25:49.000000 torch-model-manager-0.0.4/README.md
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-04-02 22:26:03.880429 torch-model-manager-0.0.4/setup.cfg
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      844 2024-04-02 22:25:52.000000 torch-model-manager-0.0.4/setup.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 22:26:03.872429 torch-model-manager-0.0.4/tests/
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 22:26:03.876429 torch-model-manager-0.0.4/tests/test_torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 16:34:05.000000 torch-model-manager-0.0.4/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-02 21:24:16.000000 torch-model-manager-0.0.4/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 22:26:03.876429 torch-model-manager-0.0.4/tests/test_utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 16:34:05.000000 torch-model-manager-0.0.4/tests/test_utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-02 16:34:05.000000 torch-model-manager-0.0.4/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 22:26:03.876429 torch-model-manager-0.0.4/torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       50 2024-04-02 21:41:02.000000 torch-model-manager-0.0.4/torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    11669 2024-04-02 16:34:05.000000 torch-model-manager-0.0.4/torch_model_manager/torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 22:26:03.880429 torch-model-manager-0.0.4/torch_model_manager.egg-info/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2746 2024-04-02 22:26:03.000000 torch-model-manager-0.0.4/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      471 2024-04-02 22:26:03.000000 torch-model-manager-0.0.4/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-04-02 22:26:03.000000 torch-model-manager-0.0.4/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       30 2024-04-02 22:26:03.000000 torch-model-manager-0.0.4/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       26 2024-04-02 22:26:03.000000 torch-model-manager-0.0.4/torch_model_manager.egg-info/top_level.txt
```

### Comparing `torch-model-manager-0.0.3/PKG-INFO` & `torch-model-manager-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -13,15 +13,15 @@
 Requires-Dist: numpy
 Requires-Dist: torchvision
 Requires-Dist: torch
 
 # Torch Model Manager
 
 
-**Torch Model Manager** is an open-source python project designed for Deep Learning developpers that aims to make the use of pytorch library easy. The version ![version](https://img.shields.io/badge/version-0.0.3.dev1-gray?labelColor=blue&style=flat) is still under developpment. The package allows us to access, search and delete layers by index, attributes or instance.
+**Torch Model Manager** is an open-source python project designed for Deep Learning developpers that aims to make the use of pytorch library easy. The version ![version](https://img.shields.io/badge/version-0.0.4-gray?labelColor=blue&style=flat) is still under developpment. The package allows us to access, search and delete layers by index, attributes or instance.
 
 ### Examples of Use
 1. **Initialization**
 ```python
 from torchvision import
 from torch_model_manager import TorchModelManager
```

### Comparing `torch-model-manager-0.0.3/README.md` & `torch-model-manager-0.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Torch Model Manager
 
 
-**Torch Model Manager** is an open-source python project designed for Deep Learning developpers that aims to make the use of pytorch library easy. The version ![version](https://img.shields.io/badge/version-0.0.3.dev1-gray?labelColor=blue&style=flat) is still under developpment. The package allows us to access, search and delete layers by index, attributes or instance.
+**Torch Model Manager** is an open-source python project designed for Deep Learning developpers that aims to make the use of pytorch library easy. The version ![version](https://img.shields.io/badge/version-0.0.4-gray?labelColor=blue&style=flat) is still under developpment. The package allows us to access, search and delete layers by index, attributes or instance.
 
 ### Examples of Use
 1. **Initialization**
 ```python
 from torchvision import
 from torch_model_manager import TorchModelManager
```

### Comparing `torch-model-manager-0.0.3/setup.py` & `torch-model-manager-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='torch-model-manager',
-    version='0.0.3',
+    version='0.0.4',
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
     packages=find_packages(exclude=['tests', 'docs', 'utils']),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url = 'https://github.com/Billal-MOKHTARI/torch-model-manager',
```

### Comparing `torch-model-manager-0.0.3/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch-model-manager-0.0.4/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch-model-manager-0.0.3/tests/test_utils/test_helpers.py` & `torch-model-manager-0.0.4/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch-model-manager-0.0.3/torch_model_manager/torch_model_manager.py` & `torch-model-manager-0.0.4/torch_model_manager/torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch-model-manager-0.0.3/torch_model_manager.egg-info/PKG-INFO` & `torch-model-manager-0.0.4/torch_model_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -13,15 +13,15 @@
 Requires-Dist: numpy
 Requires-Dist: torchvision
 Requires-Dist: torch
 
 # Torch Model Manager
 
 
-**Torch Model Manager** is an open-source python project designed for Deep Learning developpers that aims to make the use of pytorch library easy. The version ![version](https://img.shields.io/badge/version-0.0.3.dev1-gray?labelColor=blue&style=flat) is still under developpment. The package allows us to access, search and delete layers by index, attributes or instance.
+**Torch Model Manager** is an open-source python project designed for Deep Learning developpers that aims to make the use of pytorch library easy. The version ![version](https://img.shields.io/badge/version-0.0.4-gray?labelColor=blue&style=flat) is still under developpment. The package allows us to access, search and delete layers by index, attributes or instance.
 
 ### Examples of Use
 1. **Initialization**
 ```python
 from torchvision import
 from torch_model_manager import TorchModelManager
```

