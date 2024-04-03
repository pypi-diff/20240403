# Comparing `tmp/bitmat-tl-0.1.8.tar.gz` & `tmp/bitmat-tl-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitmat-tl-0.1.8.tar", last modified: Mon Apr  1 22:02:38 2024, max compression
+gzip compressed data, was "bitmat-tl-0.2.0.tar", last modified: Tue Apr  2 16:39:51 2024, max compression
```

## Comparing `bitmat-tl-0.1.8.tar` & `bitmat-tl-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-01 22:02:38.054128 bitmat-tl-0.1.8/
--rw-rw-r--   0 marco     (1000) marco     (1000)    11357 2024-03-31 16:42:10.000000 bitmat-tl-0.1.8/LICENSE
--rw-r--r--   0 marco     (1000) marco     (1000)     3227 2024-04-01 22:02:38.054128 bitmat-tl-0.1.8/PKG-INFO
--rw-rw-r--   0 marco     (1000) marco     (1000)     2615 2024-04-01 21:58:58.000000 bitmat-tl-0.1.8/README.md
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-01 22:02:38.054128 bitmat-tl-0.1.8/bitmat/
--rw-rw-r--   0 marco     (1000) marco     (1000)      216 2024-04-01 22:00:24.000000 bitmat-tl-0.1.8/bitmat/__init__.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     1061 2024-04-01 19:33:07.000000 bitmat-tl-0.1.8/bitmat/bitlinear.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-01 22:02:38.054128 bitmat-tl-0.1.8/bitmat/triton_kernels/
--rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-03-31 10:45:17.000000 bitmat-tl-0.1.8/bitmat/triton_kernels/__init__.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    12750 2024-04-01 19:35:36.000000 bitmat-tl-0.1.8/bitmat/triton_kernels/bitmat_kernel.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     5241 2024-03-26 17:02:00.000000 bitmat-tl-0.1.8/bitmat/triton_kernels/rmsnorm_kernel.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     7037 2024-03-26 17:02:00.000000 bitmat-tl-0.1.8/bitmat/triton_kernels/utils.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-01 22:02:38.054128 bitmat-tl-0.1.8/bitmat/utils/
--rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-03-26 17:02:00.000000 bitmat-tl-0.1.8/bitmat/utils/__init__.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     2413 2024-04-01 21:28:16.000000 bitmat-tl-0.1.8/bitmat/utils/bitmat.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     2987 2024-04-01 21:28:16.000000 bitmat-tl-0.1.8/bitmat/utils/convert_hf_model.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     2161 2024-03-31 10:09:31.000000 bitmat-tl-0.1.8/bitmat/utils/packing.py
--rw-rw-r--   0 marco     (1000) marco     (1000)      379 2024-03-31 17:11:38.000000 bitmat-tl-0.1.8/bitmat/utils/rmsnorm.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-01 22:02:38.054128 bitmat-tl-0.1.8/bitmat_tl.egg-info/
--rw-r--r--   0 marco     (1000) marco     (1000)     3227 2024-04-01 22:02:38.000000 bitmat-tl-0.1.8/bitmat_tl.egg-info/PKG-INFO
--rw-rw-r--   0 marco     (1000) marco     (1000)      502 2024-04-01 22:02:38.000000 bitmat-tl-0.1.8/bitmat_tl.egg-info/SOURCES.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)        1 2024-04-01 22:02:38.000000 bitmat-tl-0.1.8/bitmat_tl.egg-info/dependency_links.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)       45 2024-04-01 22:02:38.000000 bitmat-tl-0.1.8/bitmat_tl.egg-info/requires.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)        7 2024-04-01 22:02:38.000000 bitmat-tl-0.1.8/bitmat_tl.egg-info/top_level.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)       38 2024-04-01 22:02:38.054128 bitmat-tl-0.1.8/setup.cfg
--rw-rw-r--   0 marco     (1000) marco     (1000)      780 2024-04-01 21:59:16.000000 bitmat-tl-0.1.8/setup.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-02 16:39:51.050594 bitmat-tl-0.2.0/
+-rw-rw-r--   0 marco     (1000) marco     (1000)    11357 2024-04-01 22:08:01.000000 bitmat-tl-0.2.0/LICENSE
+-rw-r--r--   0 marco     (1000) marco     (1000)     3255 2024-04-02 16:39:51.050594 bitmat-tl-0.2.0/PKG-INFO
+-rw-rw-r--   0 marco     (1000) marco     (1000)     2623 2024-04-01 22:08:01.000000 bitmat-tl-0.2.0/README.md
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-02 16:39:51.046594 bitmat-tl-0.2.0/bitmat/
+-rw-rw-r--   0 marco     (1000) marco     (1000)      489 2024-04-02 10:34:53.000000 bitmat-tl-0.2.0/bitmat/__init__.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     5851 2024-04-02 16:34:32.000000 bitmat-tl-0.2.0/bitmat/bitlinear.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-02 16:39:51.046594 bitmat-tl-0.2.0/bitmat/triton_kernels/
+-rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-04-01 22:08:01.000000 bitmat-tl-0.2.0/bitmat/triton_kernels/__init__.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    12750 2024-04-01 22:08:01.000000 bitmat-tl-0.2.0/bitmat/triton_kernels/bitmat_kernel.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     5241 2024-04-01 22:08:01.000000 bitmat-tl-0.2.0/bitmat/triton_kernels/rmsnorm_kernel.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     7037 2024-04-01 22:08:01.000000 bitmat-tl-0.2.0/bitmat/triton_kernels/utils.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-02 16:39:51.050594 bitmat-tl-0.2.0/bitmat/utils/
+-rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-04-01 22:08:01.000000 bitmat-tl-0.2.0/bitmat/utils/__init__.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     2754 2024-04-02 16:10:34.000000 bitmat-tl-0.2.0/bitmat/utils/bitmat.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     2978 2024-04-02 10:12:51.000000 bitmat-tl-0.2.0/bitmat/utils/convert_hf_model.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)      497 2024-04-02 12:56:59.000000 bitmat-tl-0.2.0/bitmat/utils/pack_model_before_save.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)      416 2024-04-02 15:47:47.000000 bitmat-tl-0.2.0/bitmat/utils/packed_parameter.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     2106 2024-04-02 15:23:36.000000 bitmat-tl-0.2.0/bitmat/utils/packing.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)      400 2024-04-02 10:11:50.000000 bitmat-tl-0.2.0/bitmat/utils/rmsnorm.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-02 16:39:51.050594 bitmat-tl-0.2.0/bitmat_tl.egg-info/
+-rw-r--r--   0 marco     (1000) marco     (1000)     3255 2024-04-02 16:39:50.000000 bitmat-tl-0.2.0/bitmat_tl.egg-info/PKG-INFO
+-rw-rw-r--   0 marco     (1000) marco     (1000)      574 2024-04-02 16:39:51.000000 bitmat-tl-0.2.0/bitmat_tl.egg-info/SOURCES.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)        1 2024-04-02 16:39:50.000000 bitmat-tl-0.2.0/bitmat_tl.egg-info/dependency_links.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)       50 2024-04-02 16:39:50.000000 bitmat-tl-0.2.0/bitmat_tl.egg-info/requires.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)        7 2024-04-02 16:39:50.000000 bitmat-tl-0.2.0/bitmat_tl.egg-info/top_level.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)       38 2024-04-02 16:39:51.050594 bitmat-tl-0.2.0/setup.cfg
+-rw-rw-r--   0 marco     (1000) marco     (1000)      796 2024-04-02 16:39:35.000000 bitmat-tl-0.2.0/setup.py
```

### Comparing `bitmat-tl-0.1.8/LICENSE` & `bitmat-tl-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.1.8/PKG-INFO` & `bitmat-tl-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitmat-tl
-Version: 0.1.8
+Version: 0.2.0
 Summary: An efficent implementation for the paper: "The Era of 1-bit LLMs"
 Home-page: https://github.com/astramind-ai/BitMat/tree/main
 Author: Marco Lironi
 Author-email: marcolironi@astramind.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -12,16 +12,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch
 Requires-Dist: triton
 Requires-Dist: transformers
 Requires-Dist: bitsandbytes
 Requires-Dist: numpy
+Requires-Dist: tqdm
 
-# BitMat: Improving Matrix Multiplication with Triton
+# BitMat: Improving Ternary Matrix Multiplication with Triton
 
 ## 0️⃣1️⃣ Introduction
 BitMat is a Python package designed to optimize matrix multiplication operations by utilizing custom kernels written in Triton. Our package leverages the principles outlined in the "1bit-LLM Era" paper, specifically utilizing packed int8 data to enhance computational efficiency and performance in deep learning and numerical computing tasks.
 
 ## 🎛 Features
 Custom Triton Kernels: Utilize highly optimized kernels for matrix multiplication, tailored for performance and efficiency.
```

### Comparing `bitmat-tl-0.1.8/README.md` & `bitmat-tl-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# BitMat: Improving Matrix Multiplication with Triton
+# BitMat: Improving Ternary Matrix Multiplication with Triton
 
 ## 0️⃣1️⃣ Introduction
 BitMat is a Python package designed to optimize matrix multiplication operations by utilizing custom kernels written in Triton. Our package leverages the principles outlined in the "1bit-LLM Era" paper, specifically utilizing packed int8 data to enhance computational efficiency and performance in deep learning and numerical computing tasks.
 
 ## 🎛 Features
 Custom Triton Kernels: Utilize highly optimized kernels for matrix multiplication, tailored for performance and efficiency.
```

### Comparing `bitmat-tl-0.1.8/bitmat/triton_kernels/bitmat_kernel.py` & `bitmat-tl-0.2.0/bitmat/triton_kernels/bitmat_kernel.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.1.8/bitmat/triton_kernels/rmsnorm_kernel.py` & `bitmat-tl-0.2.0/bitmat/triton_kernels/rmsnorm_kernel.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.1.8/bitmat/triton_kernels/utils.py` & `bitmat-tl-0.2.0/bitmat/triton_kernels/utils.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.1.8/bitmat/utils/convert_hf_model.py` & `bitmat-tl-0.2.0/bitmat/utils/convert_hf_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 import torch
 from torch import nn
-
+from tqdm import tqdm
 from ..bitlinear import BitLinear
 
-from transformers import AutoModel, GemmaForCausalLM, MistralForCausalLM, LlamaForCausalLM
+from transformers import AutoModel, GemmaConfig, MistralConfig, LlamaConfig
 
 # Importing custom hijack classes for specific models
-from .model_hijacks.gemma_hijack import HijackedGemmaForCausalLM
-from .model_hijacks.mistral_hijack import HijackedMistralForCausalLM
-from .model_hijacks.llama_hijack import HijackedLlamaForCausalLM
+from .model_hijacks.gemma_1_58b import Gemma158ForCausalLM
+from .model_hijacks.mistral_1_58b import Mistral158ForCausalLM
+from .model_hijacks.llama_1_58b import Llama158ForCausalLM
+
 
 def convert_hf_model(model: AutoModel) -> AutoModel:
     """
     Convert a Hugging Face model to use BitLinear layers instead of Linear layers.
     """
+    model_config = model.config
+    del model
+
+    # initialize a tqdm progress bar
+    pbar = tqdm(total=1, desc="Converting model to 1.58Bit")
     # Check the type of the model and initialize the corresponding hijacked model
-    if isinstance(model, GemmaForCausalLM):
-        hijacked_model = HijackedGemmaForCausalLM(model.config)
-    elif isinstance(model, MistralForCausalLM):
-        hijacked_model = HijackedMistralForCausalLM(model.config)
-    elif isinstance(model, LlamaForCausalLM):
-        hijacked_model = HijackedLlamaForCausalLM(model.config)
+    if isinstance(model_config, GemmaConfig):
+        hijacked_model = Gemma158ForCausalLM(model_config)
+    elif isinstance(model_config, MistralConfig):
+        hijacked_model = Mistral158ForCausalLM(model_config)
+    elif isinstance(model_config, LlamaConfig):
+        hijacked_model = Llama158ForCausalLM(model_config)
     else:
-        raise RuntimeError("Unsupported model type.")
+        raise RuntimeError("Unsupported model type. Please open an issue on GitHub citing the model you are using")
 
-    # Load the original model's state dict into the hijacked model
-    hijacked_model.load_state_dict(model.state_dict(), strict=False)
-
-    # Apply the BitLinear conversion to the hijacked model
-    apply_bitlinear_to_hf_model(hijacked_model)
-    print("Model converted successfully")
+    pbar.update(1)
     return hijacked_model
 
+
 def apply_bitlinear_to_hf_model(model: AutoModel, parent_name='') -> AutoModel:
     """
     Recursively replace Linear layers with BitLinear layers in the model,
     except for layers within 'lm_head'.
     """
     # Store any RMS layer configurations encountered
     rms_layers = {}
@@ -59,14 +61,16 @@
             delattr(model, name)
     # Replace Linear layers with BitLinear layers
     for name, module in model.named_children():
         full_name = f'{parent_name}.{name}' if parent_name else name
 
         if 'lm_head' not in full_name and isinstance(module, nn.Linear):
             # Replace Linear layer with BitLinear
-            bit_linear = BitLinear(module.in_features, module.out_features, rms_layers.get(f"{name}_rms", {}).get('eps', torch.tensor(1e-5)), module.bias is not None)
+            bit_linear = BitLinear(module.in_features, module.out_features,
+                                   rms_layers.get(f"{name}_rms", {}).get('eps', torch.tensor(1e-5)),
+                                   module.bias is not None)
             setattr(model, name, bit_linear)
         else:
             # Recursively apply to child modules
             apply_bitlinear_to_hf_model(module, full_name)
 
     return model
```

### Comparing `bitmat-tl-0.1.8/bitmat/utils/packing.py` & `bitmat-tl-0.2.0/bitmat/utils/packing.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Pack ternary values into integers.
     x: tensor of shape (*, K, N)
     n_element_in_one_int: int, number of elements in one integer
     return: tensor of shape (*, K, N // n_element_in_one_int)
     """
     assert x.shape[-1] % n_element_in_one_int == 0, "K must be divisible by n_bits"
     assert n_element_in_one_int in [4, 8, 16, 32], "n_element_in_one_int must be 4, 8, 16, 32"
-
+    device = x.device
     x_mapped = x.clone()
     x_mapped[x == -1] = 2
 
     shift = torch.arange(n_element_in_one_int, device=x.device) * 2
 
     shape = x.shape[:-1]
     x = x_mapped.view(-1, x.shape[-2], x.shape[-1] // n_element_in_one_int, n_element_in_one_int)
@@ -31,15 +31,15 @@
     elif n_element_in_one_int == 8:
         dtype = torch.int16
     elif n_element_in_one_int == 16:
         dtype = torch.int32
     else:
         dtype = torch.int64
 
-    return x.to(dtype)
+    return x.to(dtype).to(device)
 
 
 
 def unpack_ternary(x, n_bits=4):
     """
     Unpack ternary values from integers.
     x: tensor of shape (*, K // n_bits, N), where K is the total number of ternary values
@@ -55,12 +55,11 @@
     x_expanded = x_expanded * torch.ones_like(masks)
 
     # Apply mask and shift values
     unpacked = (x_expanded & masks) >> (2 * torch.arange(n_bits, device=x.device)).view(1, 1, 1, -1)
 
     # Mappa i valori di nuovo a -1, 0, 1
     unpacked = torch.where(unpacked == 2, torch.tensor(-1, device=x.device), unpacked)
-    #unpacked = torch.where(unpacked == 3, torch.tensor(1, device=x.device), unpacked)
 
     # Riorganizza le dimensioni per ottenere il formato desiderato (*, K, N)
     return unpacked.view(*x.shape[:-1], -1)
```

### Comparing `bitmat-tl-0.1.8/bitmat_tl.egg-info/PKG-INFO` & `bitmat-tl-0.2.0/bitmat_tl.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitmat-tl
-Version: 0.1.8
+Version: 0.2.0
 Summary: An efficent implementation for the paper: "The Era of 1-bit LLMs"
 Home-page: https://github.com/astramind-ai/BitMat/tree/main
 Author: Marco Lironi
 Author-email: marcolironi@astramind.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -12,16 +12,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch
 Requires-Dist: triton
 Requires-Dist: transformers
 Requires-Dist: bitsandbytes
 Requires-Dist: numpy
+Requires-Dist: tqdm
 
-# BitMat: Improving Matrix Multiplication with Triton
+# BitMat: Improving Ternary Matrix Multiplication with Triton
 
 ## 0️⃣1️⃣ Introduction
 BitMat is a Python package designed to optimize matrix multiplication operations by utilizing custom kernels written in Triton. Our package leverages the principles outlined in the "1bit-LLM Era" paper, specifically utilizing packed int8 data to enhance computational efficiency and performance in deep learning and numerical computing tasks.
 
 ## 🎛 Features
 Custom Triton Kernels: Utilize highly optimized kernels for matrix multiplication, tailored for performance and efficiency.
```

### Comparing `bitmat-tl-0.1.8/setup.py` & `bitmat-tl-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
     name='bitmat-tl',
-    version='0.1.8',
+    version='0.2.0',
     author='Marco Lironi',
     author_email='marcolironi@astramind.ai',
     description='An efficent implementation for the paper: "The Era of 1-bit LLMs"',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/astramind-ai/BitMat/tree/main',
     packages=find_packages(),
     install_requires=[
         'torch',
         'triton',
         'transformers',
         'bitsandbytes',
-        'numpy'
+        'numpy',
+        'tqdm'
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.6',
```

