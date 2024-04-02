# Comparing `tmp/torch-model-manager-0.0.1.dev3.tar.gz` & `tmp/torch-model-manager-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch-model-manager-0.0.1.dev3.tar", last modified: Tue Apr  2 21:45:50 2024, max compression
+gzip compressed data, was "torch-model-manager-0.0.2.tar", last modified: Tue Apr  2 22:19:48 2024, max compression
```

## Comparing `torch-model-manager-0.0.1.dev3.tar` & `torch-model-manager-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,21 @@
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 21:45:50.346218 torch-model-manager-0.0.1.dev3/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2706 2024-04-02 21:45:50.342218 torch-model-manager-0.0.1.dev3/PKG-INFO
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2183 2024-04-02 16:34:05.000000 torch-model-manager-0.0.1.dev3/README.md
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-04-02 21:45:50.346218 torch-model-manager-0.0.1.dev3/setup.cfg
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      840 2024-04-02 21:45:29.000000 torch-model-manager-0.0.1.dev3/setup.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 21:45:50.334218 torch-model-manager-0.0.1.dev3/tests/
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 21:45:50.338218 torch-model-manager-0.0.1.dev3/tests/test_torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 16:34:05.000000 torch-model-manager-0.0.1.dev3/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-02 21:24:16.000000 torch-model-manager-0.0.1.dev3/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 21:45:50.338218 torch-model-manager-0.0.1.dev3/tests/test_utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 16:34:05.000000 torch-model-manager-0.0.1.dev3/tests/test_utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-02 16:34:05.000000 torch-model-manager-0.0.1.dev3/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 21:45:50.338218 torch-model-manager-0.0.1.dev3/torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       50 2024-04-02 21:41:02.000000 torch-model-manager-0.0.1.dev3/torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    11669 2024-04-02 16:34:05.000000 torch-model-manager-0.0.1.dev3/torch_model_manager/torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 21:45:50.342218 torch-model-manager-0.0.1.dev3/torch_model_manager.egg-info/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2706 2024-04-02 21:45:50.000000 torch-model-manager-0.0.1.dev3/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      506 2024-04-02 21:45:50.000000 torch-model-manager-0.0.1.dev3/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-04-02 21:45:50.000000 torch-model-manager-0.0.1.dev3/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       30 2024-04-02 21:45:50.000000 torch-model-manager-0.0.1.dev3/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-04-02 21:45:50.000000 torch-model-manager-0.0.1.dev3/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 21:45:50.342218 torch-model-manager-0.0.1.dev3/utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 16:34:05.000000 torch-model-manager-0.0.1.dev3/utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     1585 2024-04-02 16:34:05.000000 torch-model-manager-0.0.1.dev3/utils/helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 22:19:48.816848 torch-model-manager-0.0.2/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2751 2024-04-02 22:19:48.816848 torch-model-manager-0.0.2/PKG-INFO
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2233 2024-04-02 22:07:16.000000 torch-model-manager-0.0.2/README.md
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-04-02 22:19:48.816848 torch-model-manager-0.0.2/setup.cfg
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      844 2024-04-02 22:19:07.000000 torch-model-manager-0.0.2/setup.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 22:19:48.764847 torch-model-manager-0.0.2/tests/
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 22:19:48.768847 torch-model-manager-0.0.2/tests/test_torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 16:34:05.000000 torch-model-manager-0.0.2/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-02 21:24:16.000000 torch-model-manager-0.0.2/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 22:19:48.776847 torch-model-manager-0.0.2/tests/test_utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 16:34:05.000000 torch-model-manager-0.0.2/tests/test_utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-02 16:34:05.000000 torch-model-manager-0.0.2/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 22:19:48.800847 torch-model-manager-0.0.2/torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       50 2024-04-02 21:41:02.000000 torch-model-manager-0.0.2/torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    11669 2024-04-02 16:34:05.000000 torch-model-manager-0.0.2/torch_model_manager/torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 22:19:48.812847 torch-model-manager-0.0.2/torch_model_manager.egg-info/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2751 2024-04-02 22:19:48.000000 torch-model-manager-0.0.2/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      471 2024-04-02 22:19:48.000000 torch-model-manager-0.0.2/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-04-02 22:19:48.000000 torch-model-manager-0.0.2/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       30 2024-04-02 22:19:48.000000 torch-model-manager-0.0.2/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       26 2024-04-02 22:19:48.000000 torch-model-manager-0.0.2/torch_model_manager.egg-info/top_level.txt
```

### Comparing `torch-model-manager-0.0.1.dev3/PKG-INFO` & `torch-model-manager-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.0.1.dev3
+Version: 0.0.2
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -19,14 +19,15 @@
 
 **Torch Model Manager** is an open-source python project designed for Deep Learning developpers that aims to make the use of pytorch library easy. The version ![version](https://img.shields.io/badge/version-1.0.0.dev1-gray?labelColor=blue&style=flat) is still under developpment. The package allows us to access, search and delete layers by index, attributes or instance.
 
 ### Examples of Use
 1. **Initialization**
 ```python
 from torchvision import
+from torch_model_manager import TorchModelManager
 
 # Assume you have a PyTorch model 'model'
 model = models.vgg16(pretrained=True)
 
 model_manager = TorchModelManager(model)
 ```
```

### Comparing `torch-model-manager-0.0.1.dev3/README.md` & `torch-model-manager-0.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 **Torch Model Manager** is an open-source python project designed for Deep Learning developpers that aims to make the use of pytorch library easy. The version ![version](https://img.shields.io/badge/version-1.0.0.dev1-gray?labelColor=blue&style=flat) is still under developpment. The package allows us to access, search and delete layers by index, attributes or instance.
 
 ### Examples of Use
 1. **Initialization**
 ```python
 from torchvision import
+from torch_model_manager import TorchModelManager
 
 # Assume you have a PyTorch model 'model'
 model = models.vgg16(pretrained=True)
 
 model_manager = TorchModelManager(model)
 ```
```

### Comparing `torch-model-manager-0.0.1.dev3/setup.py` & `torch-model-manager-0.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='torch-model-manager',
-    version='0.0.1.dev3',
+    version='0.0.2',
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
-    packages=find_packages(exclude=['tests', 'docs']),
+    packages=find_packages(exclude=['tests', 'docs', 'utils']),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url = 'https://github.com/Billal-MOKHTARI/torch-model-manager',
     install_requires=[
         'torch',
         'numpy',
         'torchvision',
```

### Comparing `torch-model-manager-0.0.1.dev3/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch-model-manager-0.0.2/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch-model-manager-0.0.1.dev3/tests/test_utils/test_helpers.py` & `torch-model-manager-0.0.2/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch-model-manager-0.0.1.dev3/torch_model_manager/torch_model_manager.py` & `torch-model-manager-0.0.2/torch_model_manager/torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch-model-manager-0.0.1.dev3/torch_model_manager.egg-info/PKG-INFO` & `torch-model-manager-0.0.2/torch_model_manager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.0.1.dev3
+Version: 0.0.2
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -19,14 +19,15 @@
 
 **Torch Model Manager** is an open-source python project designed for Deep Learning developpers that aims to make the use of pytorch library easy. The version ![version](https://img.shields.io/badge/version-1.0.0.dev1-gray?labelColor=blue&style=flat) is still under developpment. The package allows us to access, search and delete layers by index, attributes or instance.
 
 ### Examples of Use
 1. **Initialization**
 ```python
 from torchvision import
+from torch_model_manager import TorchModelManager
 
 # Assume you have a PyTorch model 'model'
 model = models.vgg16(pretrained=True)
 
 model_manager = TorchModelManager(model)
 ```
```

