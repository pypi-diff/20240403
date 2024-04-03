# Comparing `tmp/nvidia_nvml_dev_cu12-12.4.127-py3-none-manylinux2014_x86_64.whl.zip` & `tmp/nvidia_nvml_dev_cu12-12.4.99-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,12 @@
-Zip file size: 104059 bytes, number of entries: 9
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-15 22:01 nvidia/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-15 22:01 nvidia/nvml_dev/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-15 22:01 nvidia/nvml_dev/include/__init__.py
--rw-r--r--  2.0 unx   589454 b- defN 24-Mar-15 22:01 nvidia/nvml_dev/include/nvml.h
--rw-r--r--  2.0 unx    59262 b- defN 24-Mar-15 22:01 nvidia_nvml_dev_cu12-12.4.127.dist-info/License.txt
--rw-r--r--  2.0 unx     1505 b- defN 24-Mar-15 22:01 nvidia_nvml_dev_cu12-12.4.127.dist-info/METADATA
--rw-r--r--  2.0 unx      109 b- defN 24-Mar-15 22:01 nvidia_nvml_dev_cu12-12.4.127.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 24-Mar-15 22:01 nvidia_nvml_dev_cu12-12.4.127.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      802 b- defN 24-Mar-15 22:01 nvidia_nvml_dev_cu12-12.4.127.dist-info/RECORD
-9 files, 651139 bytes uncompressed, 102647 bytes compressed:  84.2%
+Zip file size: 119718 bytes, number of entries: 10
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-28 01:10 nvidia/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-28 01:10 nvidia/nvml_dev/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-28 01:10 nvidia/nvml_dev/include/__init__.py
+-rw-r--r--  2.0 unx   589454 b- defN 24-Feb-28 01:10 nvidia/nvml_dev/include/nvml.h
+-rw-r--r--  2.0 unx    95280 b- defN 24-Feb-28 01:10 nvidia/nvml_dev/lib/x64/nvml.lib
+-rw-r--r--  2.0 unx    59262 b- defN 24-Feb-28 01:10 nvidia_nvml_dev_cu12-12.4.99.dist-info/License.txt
+-rw-r--r--  2.0 unx     1504 b- defN 24-Feb-28 01:10 nvidia_nvml_dev_cu12-12.4.99.dist-info/METADATA
+-rw-r--r--  2.0 unx       98 b- defN 24-Feb-28 01:10 nvidia_nvml_dev_cu12-12.4.99.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-Feb-28 01:10 nvidia_nvml_dev_cu12-12.4.99.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      886 b- defN 24-Feb-28 01:10 nvidia_nvml_dev_cu12-12.4.99.dist-info/RECORD
+10 files, 746491 bytes uncompressed, 118176 bytes compressed:  84.2%
```

## zipnote {}

```diff
@@ -6,23 +6,26 @@
 
 Filename: nvidia/nvml_dev/include/__init__.py
 Comment: 
 
 Filename: nvidia/nvml_dev/include/nvml.h
 Comment: 
 
-Filename: nvidia_nvml_dev_cu12-12.4.127.dist-info/License.txt
+Filename: nvidia/nvml_dev/lib/x64/nvml.lib
 Comment: 
 
-Filename: nvidia_nvml_dev_cu12-12.4.127.dist-info/METADATA
+Filename: nvidia_nvml_dev_cu12-12.4.99.dist-info/License.txt
 Comment: 
 
-Filename: nvidia_nvml_dev_cu12-12.4.127.dist-info/WHEEL
+Filename: nvidia_nvml_dev_cu12-12.4.99.dist-info/METADATA
 Comment: 
 
-Filename: nvidia_nvml_dev_cu12-12.4.127.dist-info/top_level.txt
+Filename: nvidia_nvml_dev_cu12-12.4.99.dist-info/WHEEL
 Comment: 
 
-Filename: nvidia_nvml_dev_cu12-12.4.127.dist-info/RECORD
+Filename: nvidia_nvml_dev_cu12-12.4.99.dist-info/top_level.txt
+Comment: 
+
+Filename: nvidia_nvml_dev_cu12-12.4.99.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `nvidia_nvml_dev_cu12-12.4.127.dist-info/License.txt` & `nvidia_nvml_dev_cu12-12.4.99.dist-info/License.txt`

 * *Files identical despite different names*

## Comparing `nvidia_nvml_dev_cu12-12.4.127.dist-info/METADATA` & `nvidia_nvml_dev_cu12-12.4.99.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-nvml-dev-cu12
-Version: 12.4.127
+Version: 12.4.99
 Summary: NVML native dev links, headers
 Home-page: https://developer.nvidia.com/cuda-zone
 Author: Nvidia CUDA Installer Team
 Author-email: cuda_installer@nvidia.com
 License: NVIDIA Proprietary Software
 Keywords: cuda,nvidia,runtime,machine learning,deep learning
 Classifier: Development Status :: 4 - Beta
```

