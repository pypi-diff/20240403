# Comparing `tmp/bitmat-tl-0.2.6.tar.gz` & `tmp/bitmat-tl-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitmat-tl-0.2.6.tar", last modified: Wed Apr  3 15:29:57 2024, max compression
+gzip compressed data, was "bitmat-tl-0.2.7.tar", last modified: Wed Apr  3 15:45:18 2024, max compression
```

## Comparing `bitmat-tl-0.2.6.tar` & `bitmat-tl-0.2.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-03 15:29:57.322961 bitmat-tl-0.2.6/
--rw-rw-r--   0 marco     (1000) marco     (1000)    11357 2024-04-01 22:08:01.000000 bitmat-tl-0.2.6/LICENSE
--rw-r--r--   0 marco     (1000) marco     (1000)     4490 2024-04-03 15:29:57.322961 bitmat-tl-0.2.6/PKG-INFO
--rw-rw-r--   0 marco     (1000) marco     (1000)     3858 2024-04-03 15:23:23.000000 bitmat-tl-0.2.6/README.md
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-03 15:29:57.318961 bitmat-tl-0.2.6/bitmat/
--rw-rw-r--   0 marco     (1000) marco     (1000)      489 2024-04-02 10:34:53.000000 bitmat-tl-0.2.6/bitmat/__init__.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     3601 2024-04-03 15:28:54.000000 bitmat-tl-0.2.6/bitmat/bitlinear.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-03 15:29:57.318961 bitmat-tl-0.2.6/bitmat/triton_kernels/
--rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-04-01 22:08:01.000000 bitmat-tl-0.2.6/bitmat/triton_kernels/__init__.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    12833 2024-04-03 15:23:23.000000 bitmat-tl-0.2.6/bitmat/triton_kernels/bitmat_kernel.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     5241 2024-04-01 22:08:01.000000 bitmat-tl-0.2.6/bitmat/triton_kernels/rmsnorm_kernel.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     7037 2024-04-01 22:08:01.000000 bitmat-tl-0.2.6/bitmat/triton_kernels/utils.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-03 15:29:57.318961 bitmat-tl-0.2.6/bitmat/utils/
--rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-04-01 22:08:01.000000 bitmat-tl-0.2.6/bitmat/utils/__init__.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     2661 2024-04-03 15:23:23.000000 bitmat-tl-0.2.6/bitmat/utils/bitmat.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     2978 2024-04-02 10:12:51.000000 bitmat-tl-0.2.6/bitmat/utils/convert_hf_model.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-03 15:29:57.322961 bitmat-tl-0.2.6/bitmat/utils/model_hijacks/
--rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-04-03 09:15:16.000000 bitmat-tl-0.2.6/bitmat/utils/model_hijacks/__init__.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    61141 2024-04-03 11:12:23.000000 bitmat-tl-0.2.6/bitmat/utils/model_hijacks/gemma_1_58b.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    73507 2024-04-03 09:20:11.000000 bitmat-tl-0.2.6/bitmat/utils/model_hijacks/llama_1_58b.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    64569 2024-04-03 09:20:11.000000 bitmat-tl-0.2.6/bitmat/utils/model_hijacks/mistral_1_58b.py
--rw-rw-r--   0 marco     (1000) marco     (1000)      497 2024-04-02 12:56:59.000000 bitmat-tl-0.2.6/bitmat/utils/pack_model_before_save.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     2106 2024-04-02 15:23:36.000000 bitmat-tl-0.2.6/bitmat/utils/packing.py
--rw-rw-r--   0 marco     (1000) marco     (1000)      384 2024-04-03 11:10:02.000000 bitmat-tl-0.2.6/bitmat/utils/rmsnorm.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-03 15:29:57.322961 bitmat-tl-0.2.6/bitmat_tl.egg-info/
--rw-r--r--   0 marco     (1000) marco     (1000)     4490 2024-04-03 15:29:57.000000 bitmat-tl-0.2.6/bitmat_tl.egg-info/PKG-INFO
--rw-rw-r--   0 marco     (1000) marco     (1000)      708 2024-04-03 15:29:57.000000 bitmat-tl-0.2.6/bitmat_tl.egg-info/SOURCES.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)        1 2024-04-03 15:29:57.000000 bitmat-tl-0.2.6/bitmat_tl.egg-info/dependency_links.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)       50 2024-04-03 15:29:57.000000 bitmat-tl-0.2.6/bitmat_tl.egg-info/requires.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)        7 2024-04-03 15:29:57.000000 bitmat-tl-0.2.6/bitmat_tl.egg-info/top_level.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)       38 2024-04-03 15:29:57.322961 bitmat-tl-0.2.6/setup.cfg
--rw-rw-r--   0 marco     (1000) marco     (1000)      796 2024-04-03 15:29:52.000000 bitmat-tl-0.2.6/setup.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-03 15:45:18.652308 bitmat-tl-0.2.7/
+-rw-rw-r--   0 marco     (1000) marco     (1000)    11357 2024-04-01 22:08:01.000000 bitmat-tl-0.2.7/LICENSE
+-rw-r--r--   0 marco     (1000) marco     (1000)     4490 2024-04-03 15:45:18.652308 bitmat-tl-0.2.7/PKG-INFO
+-rw-rw-r--   0 marco     (1000) marco     (1000)     3858 2024-04-03 15:23:23.000000 bitmat-tl-0.2.7/README.md
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-03 15:45:18.648308 bitmat-tl-0.2.7/bitmat/
+-rw-rw-r--   0 marco     (1000) marco     (1000)      489 2024-04-02 10:34:53.000000 bitmat-tl-0.2.7/bitmat/__init__.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     3594 2024-04-03 15:45:15.000000 bitmat-tl-0.2.7/bitmat/bitlinear.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-03 15:45:18.648308 bitmat-tl-0.2.7/bitmat/triton_kernels/
+-rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-04-01 22:08:01.000000 bitmat-tl-0.2.7/bitmat/triton_kernels/__init__.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    12833 2024-04-03 15:23:23.000000 bitmat-tl-0.2.7/bitmat/triton_kernels/bitmat_kernel.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     5241 2024-04-01 22:08:01.000000 bitmat-tl-0.2.7/bitmat/triton_kernels/rmsnorm_kernel.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     7037 2024-04-01 22:08:01.000000 bitmat-tl-0.2.7/bitmat/triton_kernels/utils.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-03 15:45:18.652308 bitmat-tl-0.2.7/bitmat/utils/
+-rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-04-01 22:08:01.000000 bitmat-tl-0.2.7/bitmat/utils/__init__.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     2661 2024-04-03 15:23:23.000000 bitmat-tl-0.2.7/bitmat/utils/bitmat.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     2978 2024-04-02 10:12:51.000000 bitmat-tl-0.2.7/bitmat/utils/convert_hf_model.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-03 15:45:18.652308 bitmat-tl-0.2.7/bitmat/utils/model_hijacks/
+-rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-04-03 09:15:16.000000 bitmat-tl-0.2.7/bitmat/utils/model_hijacks/__init__.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    61141 2024-04-03 11:12:23.000000 bitmat-tl-0.2.7/bitmat/utils/model_hijacks/gemma_1_58b.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    73507 2024-04-03 09:20:11.000000 bitmat-tl-0.2.7/bitmat/utils/model_hijacks/llama_1_58b.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    64569 2024-04-03 09:20:11.000000 bitmat-tl-0.2.7/bitmat/utils/model_hijacks/mistral_1_58b.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)      497 2024-04-02 12:56:59.000000 bitmat-tl-0.2.7/bitmat/utils/pack_model_before_save.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     2106 2024-04-02 15:23:36.000000 bitmat-tl-0.2.7/bitmat/utils/packing.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)      384 2024-04-03 11:10:02.000000 bitmat-tl-0.2.7/bitmat/utils/rmsnorm.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-03 15:45:18.652308 bitmat-tl-0.2.7/bitmat_tl.egg-info/
+-rw-r--r--   0 marco     (1000) marco     (1000)     4490 2024-04-03 15:45:18.000000 bitmat-tl-0.2.7/bitmat_tl.egg-info/PKG-INFO
+-rw-rw-r--   0 marco     (1000) marco     (1000)      708 2024-04-03 15:45:18.000000 bitmat-tl-0.2.7/bitmat_tl.egg-info/SOURCES.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)        1 2024-04-03 15:45:18.000000 bitmat-tl-0.2.7/bitmat_tl.egg-info/dependency_links.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)       50 2024-04-03 15:45:18.000000 bitmat-tl-0.2.7/bitmat_tl.egg-info/requires.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)        7 2024-04-03 15:45:18.000000 bitmat-tl-0.2.7/bitmat_tl.egg-info/top_level.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)       38 2024-04-03 15:45:18.652308 bitmat-tl-0.2.7/setup.cfg
+-rw-rw-r--   0 marco     (1000) marco     (1000)      796 2024-04-03 15:45:15.000000 bitmat-tl-0.2.7/setup.py
```

### Comparing `bitmat-tl-0.2.6/LICENSE` & `bitmat-tl-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.6/PKG-INFO` & `bitmat-tl-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitmat-tl
-Version: 0.2.6
+Version: 0.2.7
 Summary: An efficent implementation for the paper: "The Era of 1-bit LLMs"
 Home-page: https://github.com/astramind-ai/BitMat/tree/main
 Author: Marco Lironi
 Author-email: marcolironi@astramind.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `bitmat-tl-0.2.6/README.md` & `bitmat-tl-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.6/bitmat/bitlinear.py` & `bitmat-tl-0.2.7/bitmat/bitlinear.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         if mode:
             self.convert_weights_to_parameters()
         else:
             self.convert_weights_to_packed()
         return self.to(device)
 
     def forward(self, x):
-        if self.training and isinstance(self.weight, PackedParameter):
+        if self.training and (self.weight.dtype == torch.int8):
             # Just to make sure the weights are in the right format even if the user forgot to call train()
             self.convert_weights_to_parameters()
         x_dtype = x.dtype
         x = self.norm(x.to(self.norm.weight.dtype)).to(x_dtype)
         output = bitmat(self.weight.data, x, scale_w=self.scale_w)
         if self.bias is not None:
             output += self.bias.unsqueeze(0).expand_as(output)
```

### Comparing `bitmat-tl-0.2.6/bitmat/triton_kernels/bitmat_kernel.py` & `bitmat-tl-0.2.7/bitmat/triton_kernels/bitmat_kernel.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.6/bitmat/triton_kernels/rmsnorm_kernel.py` & `bitmat-tl-0.2.7/bitmat/triton_kernels/rmsnorm_kernel.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.6/bitmat/triton_kernels/utils.py` & `bitmat-tl-0.2.7/bitmat/triton_kernels/utils.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.6/bitmat/utils/bitmat.py` & `bitmat-tl-0.2.7/bitmat/utils/bitmat.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.6/bitmat/utils/convert_hf_model.py` & `bitmat-tl-0.2.7/bitmat/utils/convert_hf_model.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.6/bitmat/utils/model_hijacks/gemma_1_58b.py` & `bitmat-tl-0.2.7/bitmat/utils/model_hijacks/gemma_1_58b.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.6/bitmat/utils/model_hijacks/llama_1_58b.py` & `bitmat-tl-0.2.7/bitmat/utils/model_hijacks/llama_1_58b.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.6/bitmat/utils/model_hijacks/mistral_1_58b.py` & `bitmat-tl-0.2.7/bitmat/utils/model_hijacks/mistral_1_58b.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.6/bitmat/utils/packing.py` & `bitmat-tl-0.2.7/bitmat/utils/packing.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.6/bitmat_tl.egg-info/PKG-INFO` & `bitmat-tl-0.2.7/bitmat_tl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitmat-tl
-Version: 0.2.6
+Version: 0.2.7
 Summary: An efficent implementation for the paper: "The Era of 1-bit LLMs"
 Home-page: https://github.com/astramind-ai/BitMat/tree/main
 Author: Marco Lironi
 Author-email: marcolironi@astramind.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `bitmat-tl-0.2.6/bitmat_tl.egg-info/SOURCES.txt` & `bitmat-tl-0.2.7/bitmat_tl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.6/setup.py` & `bitmat-tl-0.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='bitmat-tl',
-    version='0.2.6',
+    version='0.2.7',
     author='Marco Lironi',
     author_email='marcolironi@astramind.ai',
     description='An efficent implementation for the paper: "The Era of 1-bit LLMs"',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/astramind-ai/BitMat/tree/main',
     packages=find_packages(),
```

