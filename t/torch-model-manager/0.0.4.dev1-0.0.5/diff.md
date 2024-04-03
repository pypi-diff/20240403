# Comparing `tmp/torch-model-manager-0.0.4.dev1.tar.gz` & `tmp/torch-model-manager-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch-model-manager-0.0.4.dev1.tar", last modified: Wed Apr  3 00:13:47 2024, max compression
+gzip compressed data, was "torch-model-manager-0.0.5.tar", last modified: Wed Apr  3 00:46:10 2024, max compression
```

## Comparing `torch-model-manager-0.0.4.dev1.tar` & `torch-model-manager-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-03 00:13:47.952578 torch-model-manager-0.0.4.dev1/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     5372 2024-04-03 00:13:47.952578 torch-model-manager-0.0.4.dev1/PKG-INFO
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     4849 2024-04-03 00:13:33.000000 torch-model-manager-0.0.4.dev1/README.md
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-04-03 00:13:47.952578 torch-model-manager-0.0.4.dev1/setup.cfg
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      840 2024-04-03 00:13:10.000000 torch-model-manager-0.0.4.dev1/setup.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-03 00:13:47.908578 torch-model-manager-0.0.4.dev1/tests/
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-03 00:13:47.912578 torch-model-manager-0.0.4.dev1/tests/test_torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 16:34:05.000000 torch-model-manager-0.0.4.dev1/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-02 21:24:16.000000 torch-model-manager-0.0.4.dev1/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-03 00:13:47.924578 torch-model-manager-0.0.4.dev1/tests/test_utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 16:34:05.000000 torch-model-manager-0.0.4.dev1/tests/test_utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-02 16:34:05.000000 torch-model-manager-0.0.4.dev1/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-03 00:13:47.948578 torch-model-manager-0.0.4.dev1/torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       50 2024-04-02 21:41:02.000000 torch-model-manager-0.0.4.dev1/torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    11669 2024-04-02 16:34:05.000000 torch-model-manager-0.0.4.dev1/torch_model_manager/torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-03 00:13:47.952578 torch-model-manager-0.0.4.dev1/torch_model_manager.egg-info/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     5372 2024-04-03 00:13:47.000000 torch-model-manager-0.0.4.dev1/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      506 2024-04-03 00:13:47.000000 torch-model-manager-0.0.4.dev1/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-04-03 00:13:47.000000 torch-model-manager-0.0.4.dev1/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       30 2024-04-03 00:13:47.000000 torch-model-manager-0.0.4.dev1/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-04-03 00:13:47.000000 torch-model-manager-0.0.4.dev1/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-03 00:13:47.952578 torch-model-manager-0.0.4.dev1/utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 16:34:05.000000 torch-model-manager-0.0.4.dev1/utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     1585 2024-04-02 16:34:05.000000 torch-model-manager-0.0.4.dev1/utils/helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-03 00:46:10.155179 torch-model-manager-0.0.5/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8694 2024-04-03 00:46:10.155179 torch-model-manager-0.0.5/PKG-INFO
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-03 00:37:24.000000 torch-model-manager-0.0.5/README.md
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-04-03 00:46:10.155179 torch-model-manager-0.0.5/setup.cfg
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)      936 2024-04-03 00:43:00.000000 torch-model-manager-0.0.5/setup.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-03 00:46:10.123179 torch-model-manager-0.0.5/tests/
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-03 00:46:10.127179 torch-model-manager-0.0.5/tests/test_torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 16:34:05.000000 torch-model-manager-0.0.5/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-02 21:24:16.000000 torch-model-manager-0.0.5/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-03 00:46:10.127179 torch-model-manager-0.0.5/tests/test_utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 16:34:05.000000 torch-model-manager-0.0.5/tests/test_utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-02 16:34:05.000000 torch-model-manager-0.0.5/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-03 00:46:10.127179 torch-model-manager-0.0.5/torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       50 2024-04-02 21:41:02.000000 torch-model-manager-0.0.5/torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    11669 2024-04-02 16:34:05.000000 torch-model-manager-0.0.5/torch_model_manager/torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-03 00:46:10.155179 torch-model-manager-0.0.5/torch_model_manager.egg-info/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8694 2024-04-03 00:46:10.000000 torch-model-manager-0.0.5/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      506 2024-04-03 00:46:10.000000 torch-model-manager-0.0.5/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-04-03 00:46:10.000000 torch-model-manager-0.0.5/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       30 2024-04-03 00:46:10.000000 torch-model-manager-0.0.5/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-04-03 00:46:10.000000 torch-model-manager-0.0.5/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-03 00:46:10.151179 torch-model-manager-0.0.5/utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 16:34:05.000000 torch-model-manager-0.0.5/utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     1585 2024-04-02 16:34:05.000000 torch-model-manager-0.0.5/utils/helpers.py
```

### Comparing `torch-model-manager-0.0.4.dev1/setup.py` & `torch-model-manager-0.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='torch-model-manager',
-    version='0.0.4.dev1',
+    version='0.0.5',
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
-    packages=find_packages(exclude=['tests', 'docs']),
+    packages=find_packages(exclude=['tests', 'docs', 'build.sh']),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url = 'https://github.com/Billal-MOKHTARI/torch-model-manager',
+    keywords=['PyTorch', 'Deep Learning', 'Machine Learning', 'High Level Programming'],
     install_requires=[
         'torch',
         'numpy',
         'torchvision',
         'torch'
         # Add any other dependencies here
     ],
```

### Comparing `torch-model-manager-0.0.4.dev1/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch-model-manager-0.0.5/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch-model-manager-0.0.4.dev1/tests/test_utils/test_helpers.py` & `torch-model-manager-0.0.5/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch-model-manager-0.0.4.dev1/torch_model_manager/torch_model_manager.py` & `torch-model-manager-0.0.5/torch_model_manager/torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch-model-manager-0.0.4.dev1/utils/helpers.py` & `torch-model-manager-0.0.5/utils/helpers.py`

 * *Files identical despite different names*

