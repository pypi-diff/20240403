# Comparing `tmp/torch-model-manager-0.0.4.tar.gz` & `tmp/torch-model-manager-0.0.4.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch-model-manager-0.0.4.tar", last modified: Tue Apr  2 22:26:03 2024, max compression
+gzip compressed data, was "torch-model-manager-0.0.4.dev1.tar", last modified: Wed Apr  3 00:13:47 2024, max compression
```

## Comparing `torch-model-manager-0.0.4.tar` & `torch-model-manager-0.0.4.dev1.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 22:26:03.880429 torch-model-manager-0.0.4/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2746 2024-04-02 22:26:03.880429 torch-model-manager-0.0.4/PKG-INFO
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2228 2024-04-02 22:25:49.000000 torch-model-manager-0.0.4/README.md
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-04-02 22:26:03.880429 torch-model-manager-0.0.4/setup.cfg
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      844 2024-04-02 22:25:52.000000 torch-model-manager-0.0.4/setup.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 22:26:03.872429 torch-model-manager-0.0.4/tests/
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 22:26:03.876429 torch-model-manager-0.0.4/tests/test_torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 16:34:05.000000 torch-model-manager-0.0.4/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-02 21:24:16.000000 torch-model-manager-0.0.4/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 22:26:03.876429 torch-model-manager-0.0.4/tests/test_utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 16:34:05.000000 torch-model-manager-0.0.4/tests/test_utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-02 16:34:05.000000 torch-model-manager-0.0.4/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 22:26:03.876429 torch-model-manager-0.0.4/torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       50 2024-04-02 21:41:02.000000 torch-model-manager-0.0.4/torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    11669 2024-04-02 16:34:05.000000 torch-model-manager-0.0.4/torch_model_manager/torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 22:26:03.880429 torch-model-manager-0.0.4/torch_model_manager.egg-info/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2746 2024-04-02 22:26:03.000000 torch-model-manager-0.0.4/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      471 2024-04-02 22:26:03.000000 torch-model-manager-0.0.4/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-04-02 22:26:03.000000 torch-model-manager-0.0.4/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       30 2024-04-02 22:26:03.000000 torch-model-manager-0.0.4/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       26 2024-04-02 22:26:03.000000 torch-model-manager-0.0.4/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-03 00:13:47.952578 torch-model-manager-0.0.4.dev1/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     5372 2024-04-03 00:13:47.952578 torch-model-manager-0.0.4.dev1/PKG-INFO
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     4849 2024-04-03 00:13:33.000000 torch-model-manager-0.0.4.dev1/README.md
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-04-03 00:13:47.952578 torch-model-manager-0.0.4.dev1/setup.cfg
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      840 2024-04-03 00:13:10.000000 torch-model-manager-0.0.4.dev1/setup.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-03 00:13:47.908578 torch-model-manager-0.0.4.dev1/tests/
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-03 00:13:47.912578 torch-model-manager-0.0.4.dev1/tests/test_torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 16:34:05.000000 torch-model-manager-0.0.4.dev1/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-02 21:24:16.000000 torch-model-manager-0.0.4.dev1/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-03 00:13:47.924578 torch-model-manager-0.0.4.dev1/tests/test_utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 16:34:05.000000 torch-model-manager-0.0.4.dev1/tests/test_utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-02 16:34:05.000000 torch-model-manager-0.0.4.dev1/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-03 00:13:47.948578 torch-model-manager-0.0.4.dev1/torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       50 2024-04-02 21:41:02.000000 torch-model-manager-0.0.4.dev1/torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    11669 2024-04-02 16:34:05.000000 torch-model-manager-0.0.4.dev1/torch_model_manager/torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-03 00:13:47.952578 torch-model-manager-0.0.4.dev1/torch_model_manager.egg-info/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     5372 2024-04-03 00:13:47.000000 torch-model-manager-0.0.4.dev1/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      506 2024-04-03 00:13:47.000000 torch-model-manager-0.0.4.dev1/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-04-03 00:13:47.000000 torch-model-manager-0.0.4.dev1/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       30 2024-04-03 00:13:47.000000 torch-model-manager-0.0.4.dev1/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-04-03 00:13:47.000000 torch-model-manager-0.0.4.dev1/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-03 00:13:47.952578 torch-model-manager-0.0.4.dev1/utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 16:34:05.000000 torch-model-manager-0.0.4.dev1/utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     1585 2024-04-02 16:34:05.000000 torch-model-manager-0.0.4.dev1/utils/helpers.py
```

### Comparing `torch-model-manager-0.0.4/setup.py` & `torch-model-manager-0.0.4.dev1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='torch-model-manager',
-    version='0.0.4',
+    version='0.0.4.dev1',
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
-    packages=find_packages(exclude=['tests', 'docs', 'utils']),
+    packages=find_packages(exclude=['tests', 'docs']),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url = 'https://github.com/Billal-MOKHTARI/torch-model-manager',
     install_requires=[
         'torch',
         'numpy',
         'torchvision',
```

### Comparing `torch-model-manager-0.0.4/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch-model-manager-0.0.4.dev1/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch-model-manager-0.0.4/tests/test_utils/test_helpers.py` & `torch-model-manager-0.0.4.dev1/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch-model-manager-0.0.4/torch_model_manager/torch_model_manager.py` & `torch-model-manager-0.0.4.dev1/torch_model_manager/torch_model_manager.py`

 * *Files identical despite different names*

