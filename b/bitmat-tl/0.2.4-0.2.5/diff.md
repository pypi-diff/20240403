# Comparing `tmp/bitmat-tl-0.2.4.tar.gz` & `tmp/bitmat-tl-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitmat-tl-0.2.4.tar", last modified: Wed Apr  3 11:20:24 2024, max compression
+gzip compressed data, was "bitmat-tl-0.2.5.tar", last modified: Wed Apr  3 15:25:08 2024, max compression
```

## Comparing `bitmat-tl-0.2.4.tar` & `bitmat-tl-0.2.5.tar`

### file list

```diff
@@ -1,33 +1,32 @@
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-03 11:20:24.834937 bitmat-tl-0.2.4/
--rw-rw-r--   0 marco     (1000) marco     (1000)    11357 2024-04-01 22:08:01.000000 bitmat-tl-0.2.4/LICENSE
--rw-r--r--   0 marco     (1000) marco     (1000)     4379 2024-04-03 11:20:24.834937 bitmat-tl-0.2.4/PKG-INFO
--rw-rw-r--   0 marco     (1000) marco     (1000)     3747 2024-04-03 11:17:45.000000 bitmat-tl-0.2.4/README.md
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-03 11:20:24.830937 bitmat-tl-0.2.4/bitmat/
--rw-rw-r--   0 marco     (1000) marco     (1000)      489 2024-04-02 10:34:53.000000 bitmat-tl-0.2.4/bitmat/__init__.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     6325 2024-04-03 11:14:27.000000 bitmat-tl-0.2.4/bitmat/bitlinear.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-03 11:20:24.834937 bitmat-tl-0.2.4/bitmat/triton_kernels/
--rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-04-01 22:08:01.000000 bitmat-tl-0.2.4/bitmat/triton_kernels/__init__.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    12750 2024-04-01 22:08:01.000000 bitmat-tl-0.2.4/bitmat/triton_kernels/bitmat_kernel.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     5241 2024-04-01 22:08:01.000000 bitmat-tl-0.2.4/bitmat/triton_kernels/rmsnorm_kernel.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     7037 2024-04-01 22:08:01.000000 bitmat-tl-0.2.4/bitmat/triton_kernels/utils.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-03 11:20:24.834937 bitmat-tl-0.2.4/bitmat/utils/
--rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-04-01 22:08:01.000000 bitmat-tl-0.2.4/bitmat/utils/__init__.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     2754 2024-04-02 16:10:34.000000 bitmat-tl-0.2.4/bitmat/utils/bitmat.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     2978 2024-04-02 10:12:51.000000 bitmat-tl-0.2.4/bitmat/utils/convert_hf_model.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-03 11:20:24.834937 bitmat-tl-0.2.4/bitmat/utils/model_hijacks/
--rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-04-03 09:15:16.000000 bitmat-tl-0.2.4/bitmat/utils/model_hijacks/__init__.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    61141 2024-04-03 11:12:23.000000 bitmat-tl-0.2.4/bitmat/utils/model_hijacks/gemma_1_58b.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    73507 2024-04-03 09:20:11.000000 bitmat-tl-0.2.4/bitmat/utils/model_hijacks/llama_1_58b.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    64569 2024-04-03 09:20:11.000000 bitmat-tl-0.2.4/bitmat/utils/model_hijacks/mistral_1_58b.py
--rw-rw-r--   0 marco     (1000) marco     (1000)      497 2024-04-02 12:56:59.000000 bitmat-tl-0.2.4/bitmat/utils/pack_model_before_save.py
--rw-rw-r--   0 marco     (1000) marco     (1000)      416 2024-04-02 15:47:47.000000 bitmat-tl-0.2.4/bitmat/utils/packed_parameter.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     2106 2024-04-02 15:23:36.000000 bitmat-tl-0.2.4/bitmat/utils/packing.py
--rw-rw-r--   0 marco     (1000) marco     (1000)      384 2024-04-03 11:10:02.000000 bitmat-tl-0.2.4/bitmat/utils/rmsnorm.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-03 11:20:24.834937 bitmat-tl-0.2.4/bitmat_tl.egg-info/
--rw-r--r--   0 marco     (1000) marco     (1000)     4379 2024-04-03 11:20:24.000000 bitmat-tl-0.2.4/bitmat_tl.egg-info/PKG-INFO
--rw-rw-r--   0 marco     (1000) marco     (1000)      741 2024-04-03 11:20:24.000000 bitmat-tl-0.2.4/bitmat_tl.egg-info/SOURCES.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)        1 2024-04-03 11:20:24.000000 bitmat-tl-0.2.4/bitmat_tl.egg-info/dependency_links.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)       50 2024-04-03 11:20:24.000000 bitmat-tl-0.2.4/bitmat_tl.egg-info/requires.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)        7 2024-04-03 11:20:24.000000 bitmat-tl-0.2.4/bitmat_tl.egg-info/top_level.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)       38 2024-04-03 11:20:24.834937 bitmat-tl-0.2.4/setup.cfg
--rw-rw-r--   0 marco     (1000) marco     (1000)      796 2024-04-03 11:20:11.000000 bitmat-tl-0.2.4/setup.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-03 15:25:08.241686 bitmat-tl-0.2.5/
+-rw-rw-r--   0 marco     (1000) marco     (1000)    11357 2024-04-01 22:08:01.000000 bitmat-tl-0.2.5/LICENSE
+-rw-r--r--   0 marco     (1000) marco     (1000)     4490 2024-04-03 15:25:08.241686 bitmat-tl-0.2.5/PKG-INFO
+-rw-rw-r--   0 marco     (1000) marco     (1000)     3858 2024-04-03 15:23:23.000000 bitmat-tl-0.2.5/README.md
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-03 15:25:08.237686 bitmat-tl-0.2.5/bitmat/
+-rw-rw-r--   0 marco     (1000) marco     (1000)      489 2024-04-02 10:34:53.000000 bitmat-tl-0.2.5/bitmat/__init__.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     3653 2024-04-03 15:23:23.000000 bitmat-tl-0.2.5/bitmat/bitlinear.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-03 15:25:08.237686 bitmat-tl-0.2.5/bitmat/triton_kernels/
+-rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-04-01 22:08:01.000000 bitmat-tl-0.2.5/bitmat/triton_kernels/__init__.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    12833 2024-04-03 15:23:23.000000 bitmat-tl-0.2.5/bitmat/triton_kernels/bitmat_kernel.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     5241 2024-04-01 22:08:01.000000 bitmat-tl-0.2.5/bitmat/triton_kernels/rmsnorm_kernel.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     7037 2024-04-01 22:08:01.000000 bitmat-tl-0.2.5/bitmat/triton_kernels/utils.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-03 15:25:08.237686 bitmat-tl-0.2.5/bitmat/utils/
+-rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-04-01 22:08:01.000000 bitmat-tl-0.2.5/bitmat/utils/__init__.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     2661 2024-04-03 15:23:23.000000 bitmat-tl-0.2.5/bitmat/utils/bitmat.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     2978 2024-04-02 10:12:51.000000 bitmat-tl-0.2.5/bitmat/utils/convert_hf_model.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-03 15:25:08.241686 bitmat-tl-0.2.5/bitmat/utils/model_hijacks/
+-rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-04-03 09:15:16.000000 bitmat-tl-0.2.5/bitmat/utils/model_hijacks/__init__.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    61141 2024-04-03 11:12:23.000000 bitmat-tl-0.2.5/bitmat/utils/model_hijacks/gemma_1_58b.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    73507 2024-04-03 09:20:11.000000 bitmat-tl-0.2.5/bitmat/utils/model_hijacks/llama_1_58b.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    64569 2024-04-03 09:20:11.000000 bitmat-tl-0.2.5/bitmat/utils/model_hijacks/mistral_1_58b.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)      497 2024-04-02 12:56:59.000000 bitmat-tl-0.2.5/bitmat/utils/pack_model_before_save.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     2106 2024-04-02 15:23:36.000000 bitmat-tl-0.2.5/bitmat/utils/packing.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)      384 2024-04-03 11:10:02.000000 bitmat-tl-0.2.5/bitmat/utils/rmsnorm.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-03 15:25:08.241686 bitmat-tl-0.2.5/bitmat_tl.egg-info/
+-rw-r--r--   0 marco     (1000) marco     (1000)     4490 2024-04-03 15:25:08.000000 bitmat-tl-0.2.5/bitmat_tl.egg-info/PKG-INFO
+-rw-rw-r--   0 marco     (1000) marco     (1000)      708 2024-04-03 15:25:08.000000 bitmat-tl-0.2.5/bitmat_tl.egg-info/SOURCES.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)        1 2024-04-03 15:25:08.000000 bitmat-tl-0.2.5/bitmat_tl.egg-info/dependency_links.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)       50 2024-04-03 15:25:08.000000 bitmat-tl-0.2.5/bitmat_tl.egg-info/requires.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)        7 2024-04-03 15:25:08.000000 bitmat-tl-0.2.5/bitmat_tl.egg-info/top_level.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)       38 2024-04-03 15:25:08.241686 bitmat-tl-0.2.5/setup.cfg
+-rw-rw-r--   0 marco     (1000) marco     (1000)      796 2024-04-03 15:23:23.000000 bitmat-tl-0.2.5/setup.py
```

### Comparing `bitmat-tl-0.2.4/LICENSE` & `bitmat-tl-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.4/PKG-INFO` & `bitmat-tl-0.2.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitmat-tl
-Version: 0.2.4
+Version: 0.2.5
 Summary: An efficent implementation for the paper: "The Era of 1-bit LLMs"
 Home-page: https://github.com/astramind-ai/BitMat/tree/main
 Author: Marco Lironi
 Author-email: marcolironi@astramind.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -16,14 +16,17 @@
 Requires-Dist: transformers
 Requires-Dist: bitsandbytes
 Requires-Dist: numpy
 Requires-Dist: tqdm
 
 # BitMat: Improving Ternary Matrix Multiplication with Triton
 
+## ⚠️ We're currently investigating as the method .to() seems not working, hold on tight while we fix it
+
+
 ## 0️⃣1️⃣ Introduction
 BitMat is a Python package designed to optimize matrix multiplication operations by utilizing custom kernels written in Triton. Our package leverages the principles outlined in the "1bit-LLM Era" paper, specifically utilizing packed int8 data to enhance computational efficiency and performance in deep learning and numerical computing tasks.
 
 ## 🎛 Features
 Custom Triton Kernels: Utilize highly optimized kernels for matrix multiplication, tailored for performance and efficiency.
 
 Packed int8 Operations: During inference the model uses packed int8 data to reduce memory usage and improve computational efficiency.
```

### Comparing `bitmat-tl-0.2.4/README.md` & `bitmat-tl-0.2.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # BitMat: Improving Ternary Matrix Multiplication with Triton
 
+## ⚠️ We're currently investigating as the method .to() seems not working, hold on tight while we fix it
+
+
 ## 0️⃣1️⃣ Introduction
 BitMat is a Python package designed to optimize matrix multiplication operations by utilizing custom kernels written in Triton. Our package leverages the principles outlined in the "1bit-LLM Era" paper, specifically utilizing packed int8 data to enhance computational efficiency and performance in deep learning and numerical computing tasks.
 
 ## 🎛 Features
 Custom Triton Kernels: Utilize highly optimized kernels for matrix multiplication, tailored for performance and efficiency.
 
 Packed int8 Operations: During inference the model uses packed int8 data to reduce memory usage and improve computational efficiency.
```

### Comparing `bitmat-tl-0.2.4/bitmat/triton_kernels/bitmat_kernel.py` & `bitmat-tl-0.2.5/bitmat/triton_kernels/bitmat_kernel.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,15 +202,14 @@
     # Write back the block of the output matrix C with masks.
     offs_cm = pid_m * BLOCK_SIZE_M + tl.arange(0, BLOCK_SIZE_M)
     offs_cn = pid_n * BLOCK_SIZE_N + tl.arange(0, BLOCK_SIZE_N)
     c_ptrs = c_ptr + stride_cm * offs_cm[:, None] + stride_cn * offs_cn[None, :] + pid_batch * stride_batch_c
     c_mask = (offs_cm[:, None] < M) & (offs_cn[None, :] < N)
     tl.store(c_ptrs, c, mask=c_mask)
 
-
 def bitmat(a, b, int_per_2_bits=4, activation=""):
     """
         a: float tensor (M, K // n_bits)
         b: int tensor (K, N)
         n_bits: int, number of bits that each element in b represents
     """
     # Check constraints.
@@ -266,36 +265,38 @@
 
     B, M, K = a.shape
     N, _ = b.shape
 
     b = b.t()
     b = b.expand(a.shape[0], b.shape[-2], b.shape[-1])
     # Allocates output.
-    c = torch.empty((B, M, N), device=b.device, dtype=torch.float16)
+    c = torch.empty((B, M, N), device=b.device, dtype=torch.float16).contiguous()
     # 1D launch kernel where each block gets its own program.
     grid = lambda META: (
         triton.cdiv(M, META['BLOCK_SIZE_M']) * triton.cdiv(N, META['BLOCK_SIZE_N']),
         B
     )
 
     # print(f"Launching kernel with M = {M}, N = {N}, K = {K}, n_bits = {n_bits}, activation = {activation}")
-
+    a_shape = a.shape
+    b_shape = b.shape
+    c_shape = c.shape
     # wrap this, otherwise triton tries to launch from cuda:0
     with torch.cuda.device(a.device):
         _ternary_bmm_kernel[grid](
             a, b, c,
             M, N, K,
             int_per_2_bits,
             a.stride(1), a.stride(2),
             b.stride(1), b.stride(2),
             c.stride(1), c.stride(2),
             a.stride(0), b.stride(0), c.stride(0),
             ACTIVATION=activation
         )
         try:
             c[0][0][0].item()
-        except RuntimeError:
+        except RuntimeError as err:
+            print(str(err))
             raise RuntimeError("Illegal memory access, it means that the kernel failed most probably to OOM, try to reduce batch size or matrix size.")
-    torch.cuda.empty_cache()
     return c
```

### Comparing `bitmat-tl-0.2.4/bitmat/triton_kernels/rmsnorm_kernel.py` & `bitmat-tl-0.2.5/bitmat/triton_kernels/rmsnorm_kernel.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.4/bitmat/triton_kernels/utils.py` & `bitmat-tl-0.2.5/bitmat/triton_kernels/utils.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.4/bitmat/utils/bitmat.py` & `bitmat-tl-0.2.5/bitmat/utils/bitmat.py`

 * *Files 16% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         packing:
         packed_w = 4 int8 -> 1 int8                             | STE
         quantization:
         scale_x = 127 / max(abs(X))                             | STE
         X = clip(round(X * scale_x), -127, 128)                 | STE
         bit matrix multiplication:
         Y = X @ w_packed.t()                                    | dot product
-        Y = Y / (scale_w * scale_x)                             | STE
+        Y = Y / scale_w / scale_x)                              | STE
         """
         if scale_w is None:
             dtype = W.dtype
             W, scale_w = terniarize(W)
             #packed_w = pack_ternary(W, 4) -> this is actually not efficent atm
             ctx.save_for_backward(X)
             X, scale_x = quantize_activations(X)
@@ -56,16 +56,14 @@
             y = batched_bitmat(X, W)
             return y / scale_w / scale_x
 
 
     @staticmethod
     @torch.cuda.amp.custom_bwd
     def backward(ctx, grad_output):
-        import pydevd
-        pydevd.settrace(suspend=False, trace_only_current_thread=True)
         X = ctx.saved_tensors[0]
         # get dW
         grad_W =  (grad_output.transpose(1,2) @ X).mean(dim=0)
         return grad_W, None, None
 
 def bitmat(W: torch.Tensor, X: torch.Tensor, scale_w) -> torch.Tensor:
     return BitMat.apply(W, X, scale_w)
```

### Comparing `bitmat-tl-0.2.4/bitmat/utils/convert_hf_model.py` & `bitmat-tl-0.2.5/bitmat/utils/convert_hf_model.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.4/bitmat/utils/model_hijacks/gemma_1_58b.py` & `bitmat-tl-0.2.5/bitmat/utils/model_hijacks/gemma_1_58b.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.4/bitmat/utils/model_hijacks/llama_1_58b.py` & `bitmat-tl-0.2.5/bitmat/utils/model_hijacks/llama_1_58b.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.4/bitmat/utils/model_hijacks/mistral_1_58b.py` & `bitmat-tl-0.2.5/bitmat/utils/model_hijacks/mistral_1_58b.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.4/bitmat/utils/packing.py` & `bitmat-tl-0.2.5/bitmat/utils/packing.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.4/bitmat_tl.egg-info/PKG-INFO` & `bitmat-tl-0.2.5/bitmat_tl.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitmat-tl
-Version: 0.2.4
+Version: 0.2.5
 Summary: An efficent implementation for the paper: "The Era of 1-bit LLMs"
 Home-page: https://github.com/astramind-ai/BitMat/tree/main
 Author: Marco Lironi
 Author-email: marcolironi@astramind.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -16,14 +16,17 @@
 Requires-Dist: transformers
 Requires-Dist: bitsandbytes
 Requires-Dist: numpy
 Requires-Dist: tqdm
 
 # BitMat: Improving Ternary Matrix Multiplication with Triton
 
+## ⚠️ We're currently investigating as the method .to() seems not working, hold on tight while we fix it
+
+
 ## 0️⃣1️⃣ Introduction
 BitMat is a Python package designed to optimize matrix multiplication operations by utilizing custom kernels written in Triton. Our package leverages the principles outlined in the "1bit-LLM Era" paper, specifically utilizing packed int8 data to enhance computational efficiency and performance in deep learning and numerical computing tasks.
 
 ## 🎛 Features
 Custom Triton Kernels: Utilize highly optimized kernels for matrix multiplication, tailored for performance and efficiency.
 
 Packed int8 Operations: During inference the model uses packed int8 data to reduce memory usage and improve computational efficiency.
```

### Comparing `bitmat-tl-0.2.4/bitmat_tl.egg-info/SOURCES.txt` & `bitmat-tl-0.2.5/bitmat_tl.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 bitmat/triton_kernels/bitmat_kernel.py
 bitmat/triton_kernels/rmsnorm_kernel.py
 bitmat/triton_kernels/utils.py
 bitmat/utils/__init__.py
 bitmat/utils/bitmat.py
 bitmat/utils/convert_hf_model.py
 bitmat/utils/pack_model_before_save.py
-bitmat/utils/packed_parameter.py
 bitmat/utils/packing.py
 bitmat/utils/rmsnorm.py
 bitmat/utils/model_hijacks/__init__.py
 bitmat/utils/model_hijacks/gemma_1_58b.py
 bitmat/utils/model_hijacks/llama_1_58b.py
 bitmat/utils/model_hijacks/mistral_1_58b.py
 bitmat_tl.egg-info/PKG-INFO
```

