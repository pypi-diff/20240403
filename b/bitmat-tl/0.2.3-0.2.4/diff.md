# Comparing `tmp/bitmat-tl-0.2.3.tar.gz` & `tmp/bitmat-tl-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitmat-tl-0.2.3.tar", last modified: Wed Apr  3 09:24:47 2024, max compression
+gzip compressed data, was "bitmat-tl-0.2.4.tar", last modified: Wed Apr  3 11:20:24 2024, max compression
```

## Comparing `bitmat-tl-0.2.3.tar` & `bitmat-tl-0.2.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-03 09:24:47.637995 bitmat-tl-0.2.3/
--rw-rw-r--   0 marco     (1000) marco     (1000)    11357 2024-04-01 22:08:01.000000 bitmat-tl-0.2.3/LICENSE
--rw-r--r--   0 marco     (1000) marco     (1000)     3255 2024-04-03 09:24:47.637995 bitmat-tl-0.2.3/PKG-INFO
--rw-rw-r--   0 marco     (1000) marco     (1000)     2623 2024-04-01 22:08:01.000000 bitmat-tl-0.2.3/README.md
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-03 09:24:47.637995 bitmat-tl-0.2.3/bitmat/
--rw-rw-r--   0 marco     (1000) marco     (1000)      489 2024-04-02 10:34:53.000000 bitmat-tl-0.2.3/bitmat/__init__.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     5851 2024-04-02 16:34:32.000000 bitmat-tl-0.2.3/bitmat/bitlinear.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-03 09:24:47.637995 bitmat-tl-0.2.3/bitmat/triton_kernels/
--rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-04-01 22:08:01.000000 bitmat-tl-0.2.3/bitmat/triton_kernels/__init__.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    12750 2024-04-01 22:08:01.000000 bitmat-tl-0.2.3/bitmat/triton_kernels/bitmat_kernel.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     5241 2024-04-01 22:08:01.000000 bitmat-tl-0.2.3/bitmat/triton_kernels/rmsnorm_kernel.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     7037 2024-04-01 22:08:01.000000 bitmat-tl-0.2.3/bitmat/triton_kernels/utils.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-03 09:24:47.637995 bitmat-tl-0.2.3/bitmat/utils/
--rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-04-01 22:08:01.000000 bitmat-tl-0.2.3/bitmat/utils/__init__.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     2754 2024-04-02 16:10:34.000000 bitmat-tl-0.2.3/bitmat/utils/bitmat.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     2978 2024-04-02 10:12:51.000000 bitmat-tl-0.2.3/bitmat/utils/convert_hf_model.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-03 09:24:47.637995 bitmat-tl-0.2.3/bitmat/utils/model_hijacks/
--rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-04-03 09:15:16.000000 bitmat-tl-0.2.3/bitmat/utils/model_hijacks/__init__.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    61162 2024-04-02 16:34:32.000000 bitmat-tl-0.2.3/bitmat/utils/model_hijacks/gemma_1_58b.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    73507 2024-04-03 09:20:11.000000 bitmat-tl-0.2.3/bitmat/utils/model_hijacks/llama_1_58b.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    64569 2024-04-03 09:20:11.000000 bitmat-tl-0.2.3/bitmat/utils/model_hijacks/mistral_1_58b.py
--rw-rw-r--   0 marco     (1000) marco     (1000)      497 2024-04-02 12:56:59.000000 bitmat-tl-0.2.3/bitmat/utils/pack_model_before_save.py
--rw-rw-r--   0 marco     (1000) marco     (1000)      416 2024-04-02 15:47:47.000000 bitmat-tl-0.2.3/bitmat/utils/packed_parameter.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     2106 2024-04-02 15:23:36.000000 bitmat-tl-0.2.3/bitmat/utils/packing.py
--rw-rw-r--   0 marco     (1000) marco     (1000)      400 2024-04-02 10:11:50.000000 bitmat-tl-0.2.3/bitmat/utils/rmsnorm.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-03 09:24:47.637995 bitmat-tl-0.2.3/bitmat_tl.egg-info/
--rw-r--r--   0 marco     (1000) marco     (1000)     3255 2024-04-03 09:24:47.000000 bitmat-tl-0.2.3/bitmat_tl.egg-info/PKG-INFO
--rw-rw-r--   0 marco     (1000) marco     (1000)      741 2024-04-03 09:24:47.000000 bitmat-tl-0.2.3/bitmat_tl.egg-info/SOURCES.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)        1 2024-04-03 09:24:47.000000 bitmat-tl-0.2.3/bitmat_tl.egg-info/dependency_links.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)       50 2024-04-03 09:24:47.000000 bitmat-tl-0.2.3/bitmat_tl.egg-info/requires.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)        7 2024-04-03 09:24:47.000000 bitmat-tl-0.2.3/bitmat_tl.egg-info/top_level.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)       38 2024-04-03 09:24:47.637995 bitmat-tl-0.2.3/setup.cfg
--rw-rw-r--   0 marco     (1000) marco     (1000)      796 2024-04-03 09:24:46.000000 bitmat-tl-0.2.3/setup.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-03 11:20:24.834937 bitmat-tl-0.2.4/
+-rw-rw-r--   0 marco     (1000) marco     (1000)    11357 2024-04-01 22:08:01.000000 bitmat-tl-0.2.4/LICENSE
+-rw-r--r--   0 marco     (1000) marco     (1000)     4379 2024-04-03 11:20:24.834937 bitmat-tl-0.2.4/PKG-INFO
+-rw-rw-r--   0 marco     (1000) marco     (1000)     3747 2024-04-03 11:17:45.000000 bitmat-tl-0.2.4/README.md
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-03 11:20:24.830937 bitmat-tl-0.2.4/bitmat/
+-rw-rw-r--   0 marco     (1000) marco     (1000)      489 2024-04-02 10:34:53.000000 bitmat-tl-0.2.4/bitmat/__init__.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     6325 2024-04-03 11:14:27.000000 bitmat-tl-0.2.4/bitmat/bitlinear.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-03 11:20:24.834937 bitmat-tl-0.2.4/bitmat/triton_kernels/
+-rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-04-01 22:08:01.000000 bitmat-tl-0.2.4/bitmat/triton_kernels/__init__.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    12750 2024-04-01 22:08:01.000000 bitmat-tl-0.2.4/bitmat/triton_kernels/bitmat_kernel.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     5241 2024-04-01 22:08:01.000000 bitmat-tl-0.2.4/bitmat/triton_kernels/rmsnorm_kernel.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     7037 2024-04-01 22:08:01.000000 bitmat-tl-0.2.4/bitmat/triton_kernels/utils.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-03 11:20:24.834937 bitmat-tl-0.2.4/bitmat/utils/
+-rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-04-01 22:08:01.000000 bitmat-tl-0.2.4/bitmat/utils/__init__.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     2754 2024-04-02 16:10:34.000000 bitmat-tl-0.2.4/bitmat/utils/bitmat.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     2978 2024-04-02 10:12:51.000000 bitmat-tl-0.2.4/bitmat/utils/convert_hf_model.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-03 11:20:24.834937 bitmat-tl-0.2.4/bitmat/utils/model_hijacks/
+-rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-04-03 09:15:16.000000 bitmat-tl-0.2.4/bitmat/utils/model_hijacks/__init__.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    61141 2024-04-03 11:12:23.000000 bitmat-tl-0.2.4/bitmat/utils/model_hijacks/gemma_1_58b.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    73507 2024-04-03 09:20:11.000000 bitmat-tl-0.2.4/bitmat/utils/model_hijacks/llama_1_58b.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    64569 2024-04-03 09:20:11.000000 bitmat-tl-0.2.4/bitmat/utils/model_hijacks/mistral_1_58b.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)      497 2024-04-02 12:56:59.000000 bitmat-tl-0.2.4/bitmat/utils/pack_model_before_save.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)      416 2024-04-02 15:47:47.000000 bitmat-tl-0.2.4/bitmat/utils/packed_parameter.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     2106 2024-04-02 15:23:36.000000 bitmat-tl-0.2.4/bitmat/utils/packing.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)      384 2024-04-03 11:10:02.000000 bitmat-tl-0.2.4/bitmat/utils/rmsnorm.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-03 11:20:24.834937 bitmat-tl-0.2.4/bitmat_tl.egg-info/
+-rw-r--r--   0 marco     (1000) marco     (1000)     4379 2024-04-03 11:20:24.000000 bitmat-tl-0.2.4/bitmat_tl.egg-info/PKG-INFO
+-rw-rw-r--   0 marco     (1000) marco     (1000)      741 2024-04-03 11:20:24.000000 bitmat-tl-0.2.4/bitmat_tl.egg-info/SOURCES.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)        1 2024-04-03 11:20:24.000000 bitmat-tl-0.2.4/bitmat_tl.egg-info/dependency_links.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)       50 2024-04-03 11:20:24.000000 bitmat-tl-0.2.4/bitmat_tl.egg-info/requires.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)        7 2024-04-03 11:20:24.000000 bitmat-tl-0.2.4/bitmat_tl.egg-info/top_level.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)       38 2024-04-03 11:20:24.834937 bitmat-tl-0.2.4/setup.cfg
+-rw-rw-r--   0 marco     (1000) marco     (1000)      796 2024-04-03 11:20:11.000000 bitmat-tl-0.2.4/setup.py
```

### Comparing `bitmat-tl-0.2.3/LICENSE` & `bitmat-tl-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.3/PKG-INFO` & `bitmat-tl-0.2.4/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: bitmat-tl
-Version: 0.2.3
-Summary: An efficent implementation for the paper: "The Era of 1-bit LLMs"
-Home-page: https://github.com/astramind-ai/BitMat/tree/main
-Author: Marco Lironi
-Author-email: marcolironi@astramind.ai
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: torch
-Requires-Dist: triton
-Requires-Dist: transformers
-Requires-Dist: bitsandbytes
-Requires-Dist: numpy
-Requires-Dist: tqdm
-
 # BitMat: Improving Ternary Matrix Multiplication with Triton
 
 ## 0️⃣1️⃣ Introduction
 BitMat is a Python package designed to optimize matrix multiplication operations by utilizing custom kernels written in Triton. Our package leverages the principles outlined in the "1bit-LLM Era" paper, specifically utilizing packed int8 data to enhance computational efficiency and performance in deep learning and numerical computing tasks.
 
 ## 🎛 Features
 Custom Triton Kernels: Utilize highly optimized kernels for matrix multiplication, tailored for performance and efficiency.
@@ -37,19 +17,40 @@
 ## 🏁 Quick Start
 
 ### High-level API (tranformers-compatible)
 ```python
 from transformers import AutoModelForCausalLM
 from bitmat import convert_hf_model
 
-# Initialize your model
+# Initialize your model from an available hf model
 model= AutoModelForCausalLM.from_pretrained("some-repo/some-model")
 # Convert the model to use BitLinear layers
 model = convert_hf_model(model)
+# Save the converted model
+model.save_pretrained('some_local_folder')
 ```
+### Loading the converted 1.58Bit Model
+To utilize the converted 1.58Bit model, such as a customized version of Mistral in this exmaple, you will need to import the specific model class from the library. Below is an example demonstrating how to load the Mistral158ForCausalLM model from a local directory:
+
+```python
+from bitmat import Mistral158ForCausalLM
+
+# Replace 'path_to_your_model' with the actual path to your model's directory
+model = Mistral158ForCausalLM.from_pretrained('path_to_your_model')
+```
+Once loaded, the model operates in two distinct modes:
+
+- Evaluation Mode: By default, the model employs quantized weights, optimizing performance for inference tasks. Activate this mode using model.eval().
+
+- Training Mode: Switching to this mode, via model.train(), allows the model to leverage full-precision weights, which is essential for training and fine-tuning processes, ensuring accurate gradient calculations and effective model updates.
+
+
+This API is **fully compatible** with the HuggingFace's Ecosystem 
+
+
 ### Low-level API
 ```python
 import torch
 from bitmat import BitLinear
 
 layer = BitLinear(in_features=1024, out_features=512, bias=True, eps=1e-5)
 # You can use the layer as a normal torch.nn.Linear layer
@@ -74,11 +75,9 @@
 ```
 ## Support
 For questions, issues, or support regarding BitMat, please open an issue on our GitHub repository.
 
 ## Acknowledgments
 Special thanks to the Triton community and the authors of the "1bit-LLM Era" paper for their groundbreaking work and inspiration.
 
-Also thanks to the developer od [BitDelta](https://github.com/FasterDecoding/BitDelta/) and [UnSloth](https://github.com/unslothai/unsloth) since part of the code is based on their work.
-
-
+Also thanks to the developer of [BitDelta](https://github.com/FasterDecoding/BitDelta/) and [UnSloth](https://github.com/unslothai/unsloth) since part of the code is based on their work.
```

### Comparing `bitmat-tl-0.2.3/bitmat/bitlinear.py` & `bitmat-tl-0.2.4/bitmat/bitlinear.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,36 +7,45 @@
 from .utils.bitmat import terniarize
 
 class BitLinear(torch.nn.Module):
     """
     A linear layer that uses packed terniary matrix multiplication.
     """
 
-    def __init__(self, in_features, out_features, bias=None, eps=1e-5, dtype=torch.float16, rms_dtype=torch.float16):
+    def __init__(self, in_features, out_features, bias=None, eps=1e-5, keep_rms_in_32b=False, dtype=torch.float16):
         super(BitLinear, self).__init__()
         self.eps = eps
         self.dtype = dtype
         self.weight = PackedParameter(torch.zeros(out_features, in_features))
         self.scale_w = torch.Tensor(1)
         if bias:
             self.bias = torch.nn.Parameter(torch.Tensor(out_features))
         else:
             self.register_parameter('bias', None)
-        self.norm = RMSLayerNorm(out_features, eps, rms_dtype) # added this in favor of models like gemma that needs hp normalization
+        self.norm = RMSLayerNorm(out_features, eps) # added this in favor of models like gemma that needs hp normalization
+        self.keep_rms_in_32b = keep_rms_in_32b
         self._post_init()
 
     def to(self, *args, **kwargs):
+        # Calls the parent class' to() method
         super(BitLinear, self).to(*args, **kwargs)
 
+        # Shift weight to the specified device/target
         if isinstance(self.weight, PackedParameter):
-            self.weight.data = self.weight.data.to(*args, **kwargs)
+            # Assicurati che PackedParameter abbia un metodo to() appropriato
+            self.weight.to(*args, **kwargs)
 
+        # Shift scale factor to the specified device/target
         if self.scale_w is not None:
             self.scale_w = self.scale_w.to(*args, **kwargs)
 
+        if self.keep_rms_in_32:
+            device, dtype, non_blocking = torch._C._nn._parse_to(*args, **kwargs)
+            self.norm.to(device, torch.float32, non_blocking)
+
         return self
 
     def cuda(self, *args, **kwargs):
         return self.to('cuda', *args, **kwargs)
 
     def _post_init(self):
         #crea un var dei parametri del modello così da poter inizializzare i pesi e i bias
@@ -116,12 +125,12 @@
             self.convert_weights_to_packed()
         return self.to(device)
 
     def forward(self, x):
         if self.training and isinstance(self.weight, PackedParameter):
             # Solo per sicurezza, in caso il forward venga chiamato direttamente in training senza chiamare .train()
             self.convert_weights_to_parameters()
-        x = self.norm(x)
+        x = self.norm(x.to(self.norm.weight.dtype)).to(self.weight.dtype)
         output = bitmat(self.weight, x, scale_w=self.scale_w)
         if self.bias is not None:
             output += self.bias.unsqueeze(0).expand_as(output)
         return output
```

### Comparing `bitmat-tl-0.2.3/bitmat/triton_kernels/bitmat_kernel.py` & `bitmat-tl-0.2.4/bitmat/triton_kernels/bitmat_kernel.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.3/bitmat/triton_kernels/rmsnorm_kernel.py` & `bitmat-tl-0.2.4/bitmat/triton_kernels/rmsnorm_kernel.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.3/bitmat/triton_kernels/utils.py` & `bitmat-tl-0.2.4/bitmat/triton_kernels/utils.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.3/bitmat/utils/bitmat.py` & `bitmat-tl-0.2.4/bitmat/utils/bitmat.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.3/bitmat/utils/convert_hf_model.py` & `bitmat-tl-0.2.4/bitmat/utils/convert_hf_model.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.3/bitmat/utils/model_hijacks/gemma_1_58b.py` & `bitmat-tl-0.2.4/bitmat/utils/model_hijacks/gemma_1_58b.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,17 +145,17 @@
 # Copied from transformers.models.mistral.modeling_mistral.MistralMLP with Mistral->Gemma158
 class Gemma158MLP(nn.Module):
     def __init__(self, config):
         super().__init__()
         self.config = config
         self.hidden_size = config.hidden_size
         self.intermediate_size = config.intermediate_size
-        self.gate_proj = BitLinear(self.hidden_size, self.intermediate_size, bias=False, eps=config.rms_norm_eps, rms_dtype=torch.float32)
-        self.up_proj = BitLinear(self.hidden_size, self.intermediate_size, bias=False, eps=config.rms_norm_eps, rms_dtype=torch.float32)
-        self.down_proj = BitLinear(self.intermediate_size, self.hidden_size, bias=False, eps=config.rms_norm_eps, rms_dtype=torch.float32)
+        self.gate_proj = BitLinear(self.hidden_size, self.intermediate_size, bias=False, eps=config.rms_norm_eps, keep_rms_in_32b=True)
+        self.up_proj = BitLinear(self.hidden_size, self.intermediate_size, bias=False, eps=config.rms_norm_eps, keep_rms_in_32b=True)
+        self.down_proj = BitLinear(self.intermediate_size, self.hidden_size, bias=False, eps=config.rms_norm_eps, keep_rms_in_32b=True)
         self.act_fn = ACT2FN[config.hidden_act]
 
     def forward(self, x):
         return self.down_proj(self.act_fn(self.gate_proj(x)) * self.up_proj(x))
 
 
 # Copied from transformers.models.llama.modeling_llama.repeat_kv
@@ -198,18 +198,18 @@
 
         if self.hidden_size % self.num_heads != 0:
             raise ValueError(
                 f"hidden_size must be divisible by num_heads (got `hidden_size`: {self.hidden_size}"
                 f" and `num_heads`: {self.num_heads})."
             )
 
-        self.q_proj = BitLinear(self.hidden_size, self.num_heads * self.head_dim, bias=config.attention_bias, eps=config.rms_norm_eps, rms_dtype=torch.float32)
-        self.k_proj = BitLinear(self.hidden_size, self.num_key_value_heads * self.head_dim, bias=config.attention_bias, eps=config.rms_norm_eps, rms_dtype=torch.float32)
-        self.v_proj = BitLinear(self.hidden_size, self.num_key_value_heads * self.head_dim, bias=config.attention_bias, eps=config.rms_norm_eps, rms_dtype=torch.float32)
-        self.o_proj = BitLinear(self.num_heads * self.head_dim, self.hidden_size, bias=config.attention_bias, eps=config.rms_norm_eps, rms_dtype=torch.float32)
+        self.q_proj = BitLinear(self.hidden_size, self.num_heads * self.head_dim, bias=config.attention_bias, eps=config.rms_norm_eps, keep_rms_in_32b=True)
+        self.k_proj = BitLinear(self.hidden_size, self.num_key_value_heads * self.head_dim, bias=config.attention_bias, eps=config.rms_norm_eps, keep_rms_in_32b=True)
+        self.v_proj = BitLinear(self.hidden_size, self.num_key_value_heads * self.head_dim, bias=config.attention_bias, eps=config.rms_norm_eps, keep_rms_in_32b=True)
+        self.o_proj = BitLinear(self.num_heads * self.head_dim, self.hidden_size, bias=config.attention_bias, eps=config.rms_norm_eps, keep_rms_in_32b=True)
         self.rotary_emb = Gemma158RotaryEmbedding(
             self.head_dim,
             max_position_embeddings=self.max_position_embeddings,
             base=self.rope_theta,
         )
 
     def forward(
```

### Comparing `bitmat-tl-0.2.3/bitmat/utils/model_hijacks/llama_1_58b.py` & `bitmat-tl-0.2.4/bitmat/utils/model_hijacks/llama_1_58b.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.3/bitmat/utils/model_hijacks/mistral_1_58b.py` & `bitmat-tl-0.2.4/bitmat/utils/model_hijacks/mistral_1_58b.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.3/bitmat/utils/packing.py` & `bitmat-tl-0.2.4/bitmat/utils/packing.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.3/bitmat_tl.egg-info/PKG-INFO` & `bitmat-tl-0.2.4/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitmat-tl
-Version: 0.2.3
+Version: 0.2.4
 Summary: An efficent implementation for the paper: "The Era of 1-bit LLMs"
 Home-page: https://github.com/astramind-ai/BitMat/tree/main
 Author: Marco Lironi
 Author-email: marcolironi@astramind.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -37,19 +37,40 @@
 ## 🏁 Quick Start
 
 ### High-level API (tranformers-compatible)
 ```python
 from transformers import AutoModelForCausalLM
 from bitmat import convert_hf_model
 
-# Initialize your model
+# Initialize your model from an available hf model
 model= AutoModelForCausalLM.from_pretrained("some-repo/some-model")
 # Convert the model to use BitLinear layers
 model = convert_hf_model(model)
+# Save the converted model
+model.save_pretrained('some_local_folder')
 ```
+### Loading the converted 1.58Bit Model
+To utilize the converted 1.58Bit model, such as a customized version of Mistral in this exmaple, you will need to import the specific model class from the library. Below is an example demonstrating how to load the Mistral158ForCausalLM model from a local directory:
+
+```python
+from bitmat import Mistral158ForCausalLM
+
+# Replace 'path_to_your_model' with the actual path to your model's directory
+model = Mistral158ForCausalLM.from_pretrained('path_to_your_model')
+```
+Once loaded, the model operates in two distinct modes:
+
+- Evaluation Mode: By default, the model employs quantized weights, optimizing performance for inference tasks. Activate this mode using model.eval().
+
+- Training Mode: Switching to this mode, via model.train(), allows the model to leverage full-precision weights, which is essential for training and fine-tuning processes, ensuring accurate gradient calculations and effective model updates.
+
+
+This API is **fully compatible** with the HuggingFace's Ecosystem 
+
+
 ### Low-level API
 ```python
 import torch
 from bitmat import BitLinear
 
 layer = BitLinear(in_features=1024, out_features=512, bias=True, eps=1e-5)
 # You can use the layer as a normal torch.nn.Linear layer
@@ -74,11 +95,9 @@
 ```
 ## Support
 For questions, issues, or support regarding BitMat, please open an issue on our GitHub repository.
 
 ## Acknowledgments
 Special thanks to the Triton community and the authors of the "1bit-LLM Era" paper for their groundbreaking work and inspiration.
 
-Also thanks to the developer od [BitDelta](https://github.com/FasterDecoding/BitDelta/) and [UnSloth](https://github.com/unslothai/unsloth) since part of the code is based on their work.
-
-
+Also thanks to the developer of [BitDelta](https://github.com/FasterDecoding/BitDelta/) and [UnSloth](https://github.com/unslothai/unsloth) since part of the code is based on their work.
```

### Comparing `bitmat-tl-0.2.3/bitmat_tl.egg-info/SOURCES.txt` & `bitmat-tl-0.2.4/bitmat_tl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.3/setup.py` & `bitmat-tl-0.2.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='bitmat-tl',
-    version='0.2.3',
+    version='0.2.4',
     author='Marco Lironi',
     author_email='marcolironi@astramind.ai',
     description='An efficent implementation for the paper: "The Era of 1-bit LLMs"',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/astramind-ai/BitMat/tree/main',
     packages=find_packages(),
```

