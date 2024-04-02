# Comparing `tmp/aqlm-1.1.3.tar.gz` & `tmp/aqlm-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aqlm-1.1.3.tar", last modified: Wed Mar 27 15:06:59 2024, max compression
+gzip compressed data, was "aqlm-1.1.4.tar", last modified: Tue Apr  2 22:02:42 2024, max compression
```

## Comparing `aqlm-1.1.3.tar` & `aqlm-1.1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 apanfero (1105122) alistgrp (1000941)        0 2024-03-27 15:06:59.828233 aqlm-1.1.3/
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)       81 2024-02-16 15:38:52.000000 aqlm-1.1.3/MANIFEST.in
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     1679 2024-03-27 15:06:59.828233 aqlm-1.1.3/PKG-INFO
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)      333 2024-02-16 15:38:52.000000 aqlm-1.1.3/pyproject.toml
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     1418 2024-03-27 15:06:59.828233 aqlm-1.1.3/setup.cfg
-drwxr-xr-x   0 apanfero (1105122) alistgrp (1000941)        0 2024-03-27 15:06:59.812232 aqlm-1.1.3/src/
-drwxr-xr-x   0 apanfero (1105122) alistgrp (1000941)        0 2024-03-27 15:06:59.816232 aqlm-1.1.3/src/aqlm/
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)      130 2024-02-22 09:29:16.000000 aqlm-1.1.3/src/aqlm/__init__.py
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     4747 2024-03-27 14:39:14.000000 aqlm-1.1.3/src/aqlm/inference.py
-drwxr-xr-x   0 apanfero (1105122) alistgrp (1000941)        0 2024-03-27 15:06:59.824232 aqlm-1.1.3/src/aqlm/inference_kernels/
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)      102 2024-02-22 09:29:16.000000 aqlm-1.1.3/src/aqlm/inference_kernels/__init__.py
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)    10888 2024-03-27 15:01:55.000000 aqlm-1.1.3/src/aqlm/inference_kernels/cuda_kernel.cpp
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)    14488 2024-03-27 14:39:14.000000 aqlm-1.1.3/src/aqlm/inference_kernels/cuda_kernel.cu
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     3350 2024-03-27 14:39:14.000000 aqlm-1.1.3/src/aqlm/inference_kernels/cuda_kernel.py
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)      716 2024-02-22 09:29:16.000000 aqlm-1.1.3/src/aqlm/inference_kernels/dequantization.py
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     4334 2024-03-27 14:39:14.000000 aqlm-1.1.3/src/aqlm/inference_kernels/kernel_selector.py
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     2499 2024-03-06 14:39:27.000000 aqlm-1.1.3/src/aqlm/inference_kernels/numba_kernel.py
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     7238 2024-02-22 09:29:16.000000 aqlm-1.1.3/src/aqlm/inference_kernels/triton_kernel.py
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     3022 2024-02-16 15:38:52.000000 aqlm-1.1.3/src/aqlm/utils.py
-drwxr-xr-x   0 apanfero (1105122) alistgrp (1000941)        0 2024-03-27 15:06:59.824232 aqlm-1.1.3/src/aqlm.egg-info/
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     1679 2024-03-27 15:06:59.000000 aqlm-1.1.3/src/aqlm.egg-info/PKG-INFO
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)      600 2024-03-27 15:06:59.000000 aqlm-1.1.3/src/aqlm.egg-info/SOURCES.txt
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)        1 2024-03-27 15:06:59.000000 aqlm-1.1.3/src/aqlm.egg-info/dependency_links.txt
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)      199 2024-03-27 15:06:59.000000 aqlm-1.1.3/src/aqlm.egg-info/requires.txt
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)        5 2024-03-27 15:06:59.000000 aqlm-1.1.3/src/aqlm.egg-info/top_level.txt
+drwxr-xr-x   0 apanfero (1105122) alistgrp (1000941)        0 2024-04-02 22:02:42.418248 aqlm-1.1.4/
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)       81 2024-02-16 15:38:52.000000 aqlm-1.1.4/MANIFEST.in
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     1679 2024-04-02 22:02:42.418248 aqlm-1.1.4/PKG-INFO
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)      333 2024-02-16 15:38:52.000000 aqlm-1.1.4/pyproject.toml
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     1418 2024-04-02 22:02:42.422248 aqlm-1.1.4/setup.cfg
+drwxr-xr-x   0 apanfero (1105122) alistgrp (1000941)        0 2024-04-02 22:02:42.398247 aqlm-1.1.4/src/
+drwxr-xr-x   0 apanfero (1105122) alistgrp (1000941)        0 2024-04-02 22:02:42.402247 aqlm-1.1.4/src/aqlm/
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)      130 2024-02-22 09:29:16.000000 aqlm-1.1.4/src/aqlm/__init__.py
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     4747 2024-04-02 21:27:23.000000 aqlm-1.1.4/src/aqlm/inference.py
+drwxr-xr-x   0 apanfero (1105122) alistgrp (1000941)        0 2024-04-02 22:02:42.410247 aqlm-1.1.4/src/aqlm/inference_kernels/
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)      102 2024-02-22 09:29:16.000000 aqlm-1.1.4/src/aqlm/inference_kernels/__init__.py
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)    10888 2024-04-02 21:27:23.000000 aqlm-1.1.4/src/aqlm/inference_kernels/cuda_kernel.cpp
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)    14569 2024-04-02 21:55:38.000000 aqlm-1.1.4/src/aqlm/inference_kernels/cuda_kernel.cu
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     3350 2024-04-02 21:27:23.000000 aqlm-1.1.4/src/aqlm/inference_kernels/cuda_kernel.py
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)      716 2024-02-22 09:29:16.000000 aqlm-1.1.4/src/aqlm/inference_kernels/dequantization.py
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     4334 2024-04-02 21:27:23.000000 aqlm-1.1.4/src/aqlm/inference_kernels/kernel_selector.py
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     2499 2024-03-06 14:39:27.000000 aqlm-1.1.4/src/aqlm/inference_kernels/numba_kernel.py
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     7238 2024-02-22 09:29:16.000000 aqlm-1.1.4/src/aqlm/inference_kernels/triton_kernel.py
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     3022 2024-02-16 15:38:52.000000 aqlm-1.1.4/src/aqlm/utils.py
+drwxr-xr-x   0 apanfero (1105122) alistgrp (1000941)        0 2024-04-02 22:02:42.418248 aqlm-1.1.4/src/aqlm.egg-info/
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     1679 2024-04-02 22:02:42.000000 aqlm-1.1.4/src/aqlm.egg-info/PKG-INFO
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)      600 2024-04-02 22:02:42.000000 aqlm-1.1.4/src/aqlm.egg-info/SOURCES.txt
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)        1 2024-04-02 22:02:42.000000 aqlm-1.1.4/src/aqlm.egg-info/dependency_links.txt
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)      199 2024-04-02 22:02:42.000000 aqlm-1.1.4/src/aqlm.egg-info/requires.txt
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)        5 2024-04-02 22:02:42.000000 aqlm-1.1.4/src/aqlm.egg-info/top_level.txt
```

### Comparing `aqlm-1.1.3/PKG-INFO` & `aqlm-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqlm
-Version: 1.1.3
+Version: 1.1.4
 Summary: Efficiently run models quantized with AQLM
 Home-page: https://github.com/Vahe1994/AQLM
 Author: AQLM paper authors
 Author-email: vahe527887@yandex.ru
 Project-URL: Bug Tracker, https://github.com/Vahe1994/AQLM/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `aqlm-1.1.3/setup.cfg` & `aqlm-1.1.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = aqlm
-version = 1.1.3
+version = 1.1.4
 author = AQLM paper authors
 author_email = vahe527887@yandex.ru
 description = Efficiently run models quantized with AQLM
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Vahe1994/AQLM
 project_urls =
```

### Comparing `aqlm-1.1.3/src/aqlm/inference.py` & `aqlm-1.1.4/src/aqlm/inference.py`

 * *Files identical despite different names*

### Comparing `aqlm-1.1.3/src/aqlm/inference_kernels/cuda_kernel.cpp` & `aqlm-1.1.4/src/aqlm/inference_kernels/cuda_kernel.cpp`

 * *Files identical despite different names*

### Comparing `aqlm-1.1.3/src/aqlm/inference_kernels/cuda_kernel.cu` & `aqlm-1.1.4/src/aqlm/inference_kernels/cuda_kernel.cu`

 * *Files 2% similar despite different names*

```diff
@@ -259,19 +259,21 @@
   while (iters--) {
     if (pred && a_gl_rd < a_gl_end) {
       const uint8_t* enc = reinterpret_cast<const uint8_t*>(&A[a_gl_rd]);
       #pragma unroll
       for (int i = 0; i < 8; i++) {
         int4 chunk;
         if constexpr (use_bfloat16) {
+          #if !defined(__CUDA_ARCH__) || (__CUDA_ARCH__ >= 800)
           nv_bfloat162* a0 = reinterpret_cast<nv_bfloat162*>(&sh_code0[8 * enc[2 * i + 0] + lane]);
           nv_bfloat162* a1 = reinterpret_cast<nv_bfloat162*>(&sh_code1[8 * enc[2 * i + 1] + lane]);
           #pragma unroll
           for (int j = 0; j < 4; j++)
             reinterpret_cast<nv_bfloat162*>(&chunk)[j] = __hadd2(a0[j], a1[j]);
+          #endif
         } else {
           half2* a0 = reinterpret_cast<half2*>(&sh_code0[8 * enc[2 * i + 0] + lane]);
           half2* a1 = reinterpret_cast<half2*>(&sh_code1[8 * enc[2 * i + 1] + lane]);
           #pragma unroll
           for (int j = 0; j < 4; j++)
             reinterpret_cast<half2*>(&chunk)[j] = __hadd2(a0[j], a1[j]);
         }
```

### Comparing `aqlm-1.1.3/src/aqlm/inference_kernels/cuda_kernel.py` & `aqlm-1.1.4/src/aqlm/inference_kernels/cuda_kernel.py`

 * *Files identical despite different names*

### Comparing `aqlm-1.1.3/src/aqlm/inference_kernels/dequantization.py` & `aqlm-1.1.4/src/aqlm/inference_kernels/dequantization.py`

 * *Files identical despite different names*

### Comparing `aqlm-1.1.3/src/aqlm/inference_kernels/kernel_selector.py` & `aqlm-1.1.4/src/aqlm/inference_kernels/kernel_selector.py`

 * *Files identical despite different names*

### Comparing `aqlm-1.1.3/src/aqlm/inference_kernels/numba_kernel.py` & `aqlm-1.1.4/src/aqlm/inference_kernels/numba_kernel.py`

 * *Files identical despite different names*

### Comparing `aqlm-1.1.3/src/aqlm/inference_kernels/triton_kernel.py` & `aqlm-1.1.4/src/aqlm/inference_kernels/triton_kernel.py`

 * *Files identical despite different names*

### Comparing `aqlm-1.1.3/src/aqlm/utils.py` & `aqlm-1.1.4/src/aqlm/utils.py`

 * *Files identical despite different names*

### Comparing `aqlm-1.1.3/src/aqlm.egg-info/PKG-INFO` & `aqlm-1.1.4/src/aqlm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqlm
-Version: 1.1.3
+Version: 1.1.4
 Summary: Efficiently run models quantized with AQLM
 Home-page: https://github.com/Vahe1994/AQLM
 Author: AQLM paper authors
 Author-email: vahe527887@yandex.ru
 Project-URL: Bug Tracker, https://github.com/Vahe1994/AQLM/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `aqlm-1.1.3/src/aqlm.egg-info/SOURCES.txt` & `aqlm-1.1.4/src/aqlm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

