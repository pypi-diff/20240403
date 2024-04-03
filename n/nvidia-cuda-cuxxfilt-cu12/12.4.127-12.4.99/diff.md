# Comparing `tmp/nvidia_cuda_cuxxfilt_cu12-12.4.127-py3-none-manylinux2014_x86_64.whl.zip` & `tmp/nvidia_cuda_cuxxfilt_cu12-12.4.99-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 17634 bytes, number of entries: 9
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-15 22:52 nvidia/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-15 22:52 nvidia/cuda_cuxxfilt/__init__.py
--rw-r--r--  2.0 unx     1912 b- defN 24-Mar-15 22:52 nvidia/cuda_cuxxfilt/include/nv_decode.h
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-15 22:52 nvidia/cuda_cuxxfilt/lib/__init__.py
--rw-r--r--  2.0 unx    59262 b- defN 24-Mar-15 22:52 nvidia_cuda_cuxxfilt_cu12-12.4.127.dist-info/License.txt
--rw-r--r--  2.0 unx     1730 b- defN 24-Mar-15 22:52 nvidia_cuda_cuxxfilt_cu12-12.4.127.dist-info/METADATA
--rw-r--r--  2.0 unx      109 b- defN 24-Mar-15 22:52 nvidia_cuda_cuxxfilt_cu12-12.4.127.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 24-Mar-15 22:52 nvidia_cuda_cuxxfilt_cu12-12.4.127.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      841 b- defN 24-Mar-15 22:52 nvidia_cuda_cuxxfilt_cu12-12.4.127.dist-info/RECORD
-9 files, 63861 bytes uncompressed, 16140 bytes compressed:  74.7%
+Zip file size: 68098 bytes, number of entries: 9
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-28 02:57 nvidia/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-28 02:57 nvidia/cuda_cuxxfilt/__init__.py
+-rw-r--r--  2.0 unx     1970 b- defN 24-Feb-28 02:57 nvidia/cuda_cuxxfilt/include/nv_decode.h
+-rw-r--r--  2.0 unx   157666 b- defN 24-Feb-28 02:57 nvidia/cuda_cuxxfilt/lib/x64/cufilt.lib
+-rw-r--r--  2.0 unx    59262 b- defN 24-Feb-28 02:57 nvidia_cuda_cuxxfilt_cu12-12.4.99.dist-info/License.txt
+-rw-r--r--  2.0 unx     1729 b- defN 24-Feb-28 02:57 nvidia_cuda_cuxxfilt_cu12-12.4.99.dist-info/METADATA
+-rw-r--r--  2.0 unx       98 b- defN 24-Feb-28 02:57 nvidia_cuda_cuxxfilt_cu12-12.4.99.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-Feb-28 02:57 nvidia_cuda_cuxxfilt_cu12-12.4.99.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      843 b- defN 24-Feb-28 02:57 nvidia_cuda_cuxxfilt_cu12-12.4.99.dist-info/RECORD
+9 files, 221575 bytes uncompressed, 66608 bytes compressed:  69.9%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: nvidia/cuda_cuxxfilt/__init__.py
 Comment: 
 
 Filename: nvidia/cuda_cuxxfilt/include/nv_decode.h
 Comment: 
 
-Filename: nvidia/cuda_cuxxfilt/lib/__init__.py
+Filename: nvidia/cuda_cuxxfilt/lib/x64/cufilt.lib
 Comment: 
 
-Filename: nvidia_cuda_cuxxfilt_cu12-12.4.127.dist-info/License.txt
+Filename: nvidia_cuda_cuxxfilt_cu12-12.4.99.dist-info/License.txt
 Comment: 
 
-Filename: nvidia_cuda_cuxxfilt_cu12-12.4.127.dist-info/METADATA
+Filename: nvidia_cuda_cuxxfilt_cu12-12.4.99.dist-info/METADATA
 Comment: 
 
-Filename: nvidia_cuda_cuxxfilt_cu12-12.4.127.dist-info/WHEEL
+Filename: nvidia_cuda_cuxxfilt_cu12-12.4.99.dist-info/WHEEL
 Comment: 
 
-Filename: nvidia_cuda_cuxxfilt_cu12-12.4.127.dist-info/top_level.txt
+Filename: nvidia_cuda_cuxxfilt_cu12-12.4.99.dist-info/top_level.txt
 Comment: 
 
-Filename: nvidia_cuda_cuxxfilt_cu12-12.4.127.dist-info/RECORD
+Filename: nvidia_cuda_cuxxfilt_cu12-12.4.99.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nvidia/cuda_cuxxfilt/include/nv_decode.h

 * *Ordering differences only*

```diff
@@ -1,58 +1,58 @@
-/*
- * NVIDIA_COPYRIGHT_BEGIN
- *
- * Copyright (c) 2021, NVIDIA CORPORATION.  All rights reserved.
- *
- * NVIDIA_COPYRIGHT_END
- */
-
-/*
-nv_decode.h -- API for the CUDA C++ name demangler.
-*/
-
-/* Avoid including these declarations more than once: */
-#ifndef DECODE_H
-#define DECODE_H 1
-
-#ifdef __cplusplus
-extern "C" {
-#endif
-
-/* Cuda C++ demangling API.
-
-   Parameters:
-     id: Input mangled string
-     output_buffer: Pointer to where the demangled buffer will
-                    be stored. This memory must be allocated with malloc.
-                    If output-buffer is NULL, memory will be malloc'd to
-                    store the demangled name and returned through the 
-                    function return value.
-                    If the output-buffer is too small, it is expanded using
-                    realloc.
-     length: It is necessary to provide the size of the output buffer if the user
-             is providing pre-allocated memory. This is needed by the demangler 
-             in case the size needs to be reallocated.
-             If the length is non-null, the length of the demangled buffer
-             is placed in length.
-     status: *status is set to one of the following values. 0 - The
-             demangling operation succeeded; -1 - A memory allocation
-             failure occurred. -2 - Not a valid mangled id. -3 - An
-             input validation failure has occurred (one or more
-             arguments are invalid).
-
-   Return Value: A pointer to the start of the NUL-terminated demangled name,
-                 or NULL if the demangling fails. The caller is responsible for
-                 deallocating this memory using free.
-
-   Note: This function is thread-safe.
-*/
-
-char* __cu_demangle(const char *id,
-	                char *output_buffer,
-	                size_t *length,
-	                int *status);
-
-#ifdef __cplusplus
-}
-#endif
-#endif /* ifndef DECODE_H */
+/*
+ * NVIDIA_COPYRIGHT_BEGIN
+ *
+ * Copyright (c) 2021, NVIDIA CORPORATION.  All rights reserved.
+ *
+ * NVIDIA_COPYRIGHT_END
+ */
+
+/*
+nv_decode.h -- API for the CUDA C++ name demangler.
+*/
+
+/* Avoid including these declarations more than once: */
+#ifndef DECODE_H
+#define DECODE_H 1
+
+#ifdef __cplusplus
+extern "C" {
+#endif
+
+/* Cuda C++ demangling API.
+
+   Parameters:
+     id: Input mangled string
+     output_buffer: Pointer to where the demangled buffer will
+                    be stored. This memory must be allocated with malloc.
+                    If output-buffer is NULL, memory will be malloc'd to
+                    store the demangled name and returned through the 
+                    function return value.
+                    If the output-buffer is too small, it is expanded using
+                    realloc.
+     length: It is necessary to provide the size of the output buffer if the user
+             is providing pre-allocated memory. This is needed by the demangler 
+             in case the size needs to be reallocated.
+             If the length is non-null, the length of the demangled buffer
+             is placed in length.
+     status: *status is set to one of the following values. 0 - The
+             demangling operation succeeded; -1 - A memory allocation
+             failure occurred. -2 - Not a valid mangled id. -3 - An
+             input validation failure has occurred (one or more
+             arguments are invalid).
+
+   Return Value: A pointer to the start of the NUL-terminated demangled name,
+                 or NULL if the demangling fails. The caller is responsible for
+                 deallocating this memory using free.
+
+   Note: This function is thread-safe.
+*/
+
+char* __cu_demangle(const char *id,
+	                char *output_buffer,
+	                size_t *length,
+	                int *status);
+
+#ifdef __cplusplus
+}
+#endif
+#endif /* ifndef DECODE_H */
```

## Comparing `nvidia_cuda_cuxxfilt_cu12-12.4.127.dist-info/License.txt` & `nvidia_cuda_cuxxfilt_cu12-12.4.99.dist-info/License.txt`

 * *Files identical despite different names*

## Comparing `nvidia_cuda_cuxxfilt_cu12-12.4.127.dist-info/METADATA` & `nvidia_cuda_cuxxfilt_cu12-12.4.99.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-cuda-cuxxfilt-cu12
-Version: 12.4.127
+Version: 12.4.99
 Summary: CUDA cuxxfilt
 Home-page: https://developer.nvidia.com/cuda-zone
 Author: Nvidia CUDA Installer Team
 Author-email: cuda_installer@nvidia.com
 License: NVIDIA Proprietary Software
 Keywords: cuda,nvidia,runtime,machine learning,deep learning
 Classifier: Development Status :: 4 - Beta
```

## Comparing `nvidia_cuda_cuxxfilt_cu12-12.4.127.dist-info/RECORD` & `nvidia_cuda_cuxxfilt_cu12-12.4.99.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 nvidia/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 nvidia/cuda_cuxxfilt/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-nvidia/cuda_cuxxfilt/include/nv_decode.h,sha256=nLqAQ0_QpbNaQF3tXTPdfF5S54X_QroctTOf0fgOeyE,1912
-nvidia/cuda_cuxxfilt/lib/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-nvidia_cuda_cuxxfilt_cu12-12.4.127.dist-info/License.txt,sha256=rW9YU_ugyg0VnQ9Y1JrkmDDC-Mk_epJki5zpCttMbM0,59262
-nvidia_cuda_cuxxfilt_cu12-12.4.127.dist-info/METADATA,sha256=2Y_-3siWQvGW9LTUNNFf3BLWMBO36uQqe6ESaivuntU,1730
-nvidia_cuda_cuxxfilt_cu12-12.4.127.dist-info/WHEEL,sha256=XDTs3wIbcE-BcRO08VJlZpA6z9OaC1mOKPCGGGwuM2g,109
-nvidia_cuda_cuxxfilt_cu12-12.4.127.dist-info/top_level.txt,sha256=fTkAtiFuL16nUrB9ytDDtpytz2t0B4NvYTnRzwAhO14,7
-nvidia_cuda_cuxxfilt_cu12-12.4.127.dist-info/RECORD,,
+nvidia/cuda_cuxxfilt/include/nv_decode.h,sha256=emnz0H-B3cjUh9UaY0jYze7ETJvn5GXTZEAbfrtiG7c,1970
+nvidia/cuda_cuxxfilt/lib/x64/cufilt.lib,sha256=oKPFRksw9-KqcfKJvy_MPEnaYksmSQLEcxG-mfzDQE0,157666
+nvidia_cuda_cuxxfilt_cu12-12.4.99.dist-info/License.txt,sha256=rW9YU_ugyg0VnQ9Y1JrkmDDC-Mk_epJki5zpCttMbM0,59262
+nvidia_cuda_cuxxfilt_cu12-12.4.99.dist-info/METADATA,sha256=qe2z7hA08uzAhEsyIc_xlWFeBuEROIPUpr6Hy0pW5hI,1729
+nvidia_cuda_cuxxfilt_cu12-12.4.99.dist-info/WHEEL,sha256=6iYPr8vTHsyDK75jr9X0V3I9wPSVmtwr_8fdATBciGk,98
+nvidia_cuda_cuxxfilt_cu12-12.4.99.dist-info/top_level.txt,sha256=fTkAtiFuL16nUrB9ytDDtpytz2t0B4NvYTnRzwAhO14,7
+nvidia_cuda_cuxxfilt_cu12-12.4.99.dist-info/RECORD,,
```

