# Comparing `tmp/bitmat-tl-0.2.0.tar.gz` & `tmp/bitmat-tl-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitmat-tl-0.2.0.tar", last modified: Tue Apr  2 16:39:51 2024, max compression
+gzip compressed data, was "bitmat-tl-0.2.2.tar", last modified: Wed Apr  3 09:15:57 2024, max compression
```

## Comparing `bitmat-tl-0.2.0.tar` & `bitmat-tl-0.2.2.tar`

### file list

```diff
@@ -1,28 +1,33 @@
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-02 16:39:51.050594 bitmat-tl-0.2.0/
--rw-rw-r--   0 marco     (1000) marco     (1000)    11357 2024-04-01 22:08:01.000000 bitmat-tl-0.2.0/LICENSE
--rw-r--r--   0 marco     (1000) marco     (1000)     3255 2024-04-02 16:39:51.050594 bitmat-tl-0.2.0/PKG-INFO
--rw-rw-r--   0 marco     (1000) marco     (1000)     2623 2024-04-01 22:08:01.000000 bitmat-tl-0.2.0/README.md
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-02 16:39:51.046594 bitmat-tl-0.2.0/bitmat/
--rw-rw-r--   0 marco     (1000) marco     (1000)      489 2024-04-02 10:34:53.000000 bitmat-tl-0.2.0/bitmat/__init__.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     5851 2024-04-02 16:34:32.000000 bitmat-tl-0.2.0/bitmat/bitlinear.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-02 16:39:51.046594 bitmat-tl-0.2.0/bitmat/triton_kernels/
--rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-04-01 22:08:01.000000 bitmat-tl-0.2.0/bitmat/triton_kernels/__init__.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    12750 2024-04-01 22:08:01.000000 bitmat-tl-0.2.0/bitmat/triton_kernels/bitmat_kernel.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     5241 2024-04-01 22:08:01.000000 bitmat-tl-0.2.0/bitmat/triton_kernels/rmsnorm_kernel.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     7037 2024-04-01 22:08:01.000000 bitmat-tl-0.2.0/bitmat/triton_kernels/utils.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-02 16:39:51.050594 bitmat-tl-0.2.0/bitmat/utils/
--rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-04-01 22:08:01.000000 bitmat-tl-0.2.0/bitmat/utils/__init__.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     2754 2024-04-02 16:10:34.000000 bitmat-tl-0.2.0/bitmat/utils/bitmat.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     2978 2024-04-02 10:12:51.000000 bitmat-tl-0.2.0/bitmat/utils/convert_hf_model.py
--rw-rw-r--   0 marco     (1000) marco     (1000)      497 2024-04-02 12:56:59.000000 bitmat-tl-0.2.0/bitmat/utils/pack_model_before_save.py
--rw-rw-r--   0 marco     (1000) marco     (1000)      416 2024-04-02 15:47:47.000000 bitmat-tl-0.2.0/bitmat/utils/packed_parameter.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     2106 2024-04-02 15:23:36.000000 bitmat-tl-0.2.0/bitmat/utils/packing.py
--rw-rw-r--   0 marco     (1000) marco     (1000)      400 2024-04-02 10:11:50.000000 bitmat-tl-0.2.0/bitmat/utils/rmsnorm.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-02 16:39:51.050594 bitmat-tl-0.2.0/bitmat_tl.egg-info/
--rw-r--r--   0 marco     (1000) marco     (1000)     3255 2024-04-02 16:39:50.000000 bitmat-tl-0.2.0/bitmat_tl.egg-info/PKG-INFO
--rw-rw-r--   0 marco     (1000) marco     (1000)      574 2024-04-02 16:39:51.000000 bitmat-tl-0.2.0/bitmat_tl.egg-info/SOURCES.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)        1 2024-04-02 16:39:50.000000 bitmat-tl-0.2.0/bitmat_tl.egg-info/dependency_links.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)       50 2024-04-02 16:39:50.000000 bitmat-tl-0.2.0/bitmat_tl.egg-info/requires.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)        7 2024-04-02 16:39:50.000000 bitmat-tl-0.2.0/bitmat_tl.egg-info/top_level.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)       38 2024-04-02 16:39:51.050594 bitmat-tl-0.2.0/setup.cfg
--rw-rw-r--   0 marco     (1000) marco     (1000)      796 2024-04-02 16:39:35.000000 bitmat-tl-0.2.0/setup.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-03 09:15:57.927591 bitmat-tl-0.2.2/
+-rw-rw-r--   0 marco     (1000) marco     (1000)    11357 2024-04-01 22:08:01.000000 bitmat-tl-0.2.2/LICENSE
+-rw-r--r--   0 marco     (1000) marco     (1000)     3255 2024-04-03 09:15:57.927591 bitmat-tl-0.2.2/PKG-INFO
+-rw-rw-r--   0 marco     (1000) marco     (1000)     2623 2024-04-01 22:08:01.000000 bitmat-tl-0.2.2/README.md
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-03 09:15:57.923590 bitmat-tl-0.2.2/bitmat/
+-rw-rw-r--   0 marco     (1000) marco     (1000)      489 2024-04-02 10:34:53.000000 bitmat-tl-0.2.2/bitmat/__init__.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     5851 2024-04-02 16:34:32.000000 bitmat-tl-0.2.2/bitmat/bitlinear.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-03 09:15:57.927591 bitmat-tl-0.2.2/bitmat/triton_kernels/
+-rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-04-01 22:08:01.000000 bitmat-tl-0.2.2/bitmat/triton_kernels/__init__.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    12750 2024-04-01 22:08:01.000000 bitmat-tl-0.2.2/bitmat/triton_kernels/bitmat_kernel.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     5241 2024-04-01 22:08:01.000000 bitmat-tl-0.2.2/bitmat/triton_kernels/rmsnorm_kernel.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     7037 2024-04-01 22:08:01.000000 bitmat-tl-0.2.2/bitmat/triton_kernels/utils.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-03 09:15:57.927591 bitmat-tl-0.2.2/bitmat/utils/
+-rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-04-01 22:08:01.000000 bitmat-tl-0.2.2/bitmat/utils/__init__.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     2754 2024-04-02 16:10:34.000000 bitmat-tl-0.2.2/bitmat/utils/bitmat.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     2978 2024-04-02 10:12:51.000000 bitmat-tl-0.2.2/bitmat/utils/convert_hf_model.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-03 09:15:57.927591 bitmat-tl-0.2.2/bitmat/utils/model_hijacks/
+-rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-04-03 09:15:16.000000 bitmat-tl-0.2.2/bitmat/utils/model_hijacks/__init__.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    61162 2024-04-02 16:34:32.000000 bitmat-tl-0.2.2/bitmat/utils/model_hijacks/gemma_1_58b.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    73501 2024-04-02 16:37:27.000000 bitmat-tl-0.2.2/bitmat/utils/model_hijacks/llama_1_58b.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    64563 2024-04-02 16:37:27.000000 bitmat-tl-0.2.2/bitmat/utils/model_hijacks/mistral_1_58b.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)      497 2024-04-02 12:56:59.000000 bitmat-tl-0.2.2/bitmat/utils/pack_model_before_save.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)      416 2024-04-02 15:47:47.000000 bitmat-tl-0.2.2/bitmat/utils/packed_parameter.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     2106 2024-04-02 15:23:36.000000 bitmat-tl-0.2.2/bitmat/utils/packing.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)      400 2024-04-02 10:11:50.000000 bitmat-tl-0.2.2/bitmat/utils/rmsnorm.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-03 09:15:57.927591 bitmat-tl-0.2.2/bitmat_tl.egg-info/
+-rw-r--r--   0 marco     (1000) marco     (1000)     3255 2024-04-03 09:15:57.000000 bitmat-tl-0.2.2/bitmat_tl.egg-info/PKG-INFO
+-rw-rw-r--   0 marco     (1000) marco     (1000)      741 2024-04-03 09:15:57.000000 bitmat-tl-0.2.2/bitmat_tl.egg-info/SOURCES.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)        1 2024-04-03 09:15:57.000000 bitmat-tl-0.2.2/bitmat_tl.egg-info/dependency_links.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)       50 2024-04-03 09:15:57.000000 bitmat-tl-0.2.2/bitmat_tl.egg-info/requires.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)        7 2024-04-03 09:15:57.000000 bitmat-tl-0.2.2/bitmat_tl.egg-info/top_level.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)       38 2024-04-03 09:15:57.927591 bitmat-tl-0.2.2/setup.cfg
+-rw-rw-r--   0 marco     (1000) marco     (1000)      796 2024-04-03 09:15:56.000000 bitmat-tl-0.2.2/setup.py
```

### Comparing `bitmat-tl-0.2.0/LICENSE` & `bitmat-tl-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.0/PKG-INFO` & `bitmat-tl-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitmat-tl
-Version: 0.2.0
+Version: 0.2.2
 Summary: An efficent implementation for the paper: "The Era of 1-bit LLMs"
 Home-page: https://github.com/astramind-ai/BitMat/tree/main
 Author: Marco Lironi
 Author-email: marcolironi@astramind.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `bitmat-tl-0.2.0/README.md` & `bitmat-tl-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.0/bitmat/bitlinear.py` & `bitmat-tl-0.2.2/bitmat/bitlinear.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.0/bitmat/triton_kernels/bitmat_kernel.py` & `bitmat-tl-0.2.2/bitmat/triton_kernels/bitmat_kernel.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.0/bitmat/triton_kernels/rmsnorm_kernel.py` & `bitmat-tl-0.2.2/bitmat/triton_kernels/rmsnorm_kernel.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.0/bitmat/triton_kernels/utils.py` & `bitmat-tl-0.2.2/bitmat/triton_kernels/utils.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.0/bitmat/utils/bitmat.py` & `bitmat-tl-0.2.2/bitmat/utils/bitmat.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.0/bitmat/utils/convert_hf_model.py` & `bitmat-tl-0.2.2/bitmat/utils/convert_hf_model.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.0/bitmat/utils/packing.py` & `bitmat-tl-0.2.2/bitmat/utils/packing.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.0/bitmat_tl.egg-info/PKG-INFO` & `bitmat-tl-0.2.2/bitmat_tl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitmat-tl
-Version: 0.2.0
+Version: 0.2.2
 Summary: An efficent implementation for the paper: "The Era of 1-bit LLMs"
 Home-page: https://github.com/astramind-ai/BitMat/tree/main
 Author: Marco Lironi
 Author-email: marcolironi@astramind.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `bitmat-tl-0.2.0/setup.py` & `bitmat-tl-0.2.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='bitmat-tl',
-    version='0.2.0',
+    version='0.2.2',
     author='Marco Lironi',
     author_email='marcolironi@astramind.ai',
     description='An efficent implementation for the paper: "The Era of 1-bit LLMs"',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/astramind-ai/BitMat/tree/main',
     packages=find_packages(),
```

