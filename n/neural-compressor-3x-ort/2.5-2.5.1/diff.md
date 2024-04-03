# Comparing `tmp/neural_compressor_3x_ort-2.5.tar.gz` & `tmp/neural_compressor_3x_ort-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neural_compressor_3x_ort-2.5.tar", last modified: Tue Mar 26 10:15:46 2024, max compression
+gzip compressed data, was "neural_compressor_3x_ort-2.5.1.tar", last modified: Wed Apr  3 13:34:43 2024, max compression
```

## Comparing `neural_compressor_3x_ort-2.5.tar` & `neural_compressor_3x_ort-2.5.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 10:15:46.373769 neural_compressor_3x_ort-2.5/
--rw-r--r--   0 root         (0) root         (0)    11360 2024-03-26 10:15:12.000000 neural_compressor_3x_ort-2.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)    15009 2024-03-26 10:15:46.373769 neural_compressor_3x_ort-2.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    14096 2024-03-26 10:15:12.000000 neural_compressor_3x_ort-2.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 10:15:46.367769 neural_compressor_3x_ort-2.5/neural_compressor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 10:15:46.369769 neural_compressor_3x_ort-2.5/neural_compressor/common/
--rw-r--r--   0 root         (0) root         (0)     1059 2024-03-26 10:15:12.000000 neural_compressor_3x_ort-2.5/neural_compressor/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23884 2024-03-26 10:15:12.000000 neural_compressor_3x_ort-2.5/neural_compressor/common/base_config.py
--rw-r--r--   0 root         (0) root         (0)    12807 2024-03-26 10:15:12.000000 neural_compressor_3x_ort-2.5/neural_compressor/common/base_tuning.py
--rw-r--r--   0 root         (0) root         (0)     3298 2024-03-26 10:15:12.000000 neural_compressor_3x_ort-2.5/neural_compressor/common/tuning_param.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 10:15:46.369769 neural_compressor_3x_ort-2.5/neural_compressor/common/utils/
--rw-r--r--   0 root         (0) root         (0)      932 2024-03-26 10:15:12.000000 neural_compressor_3x_ort-2.5/neural_compressor/common/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1284 2024-03-26 10:15:12.000000 neural_compressor_3x_ort-2.5/neural_compressor/common/utils/constants.py
--rw-r--r--   0 root         (0) root         (0)     6009 2024-03-26 10:15:12.000000 neural_compressor_3x_ort-2.5/neural_compressor/common/utils/logger.py
--rw-r--r--   0 root         (0) root         (0)     2147 2024-03-26 10:15:12.000000 neural_compressor_3x_ort-2.5/neural_compressor/common/utils/save_load.py
--rw-r--r--   0 root         (0) root         (0)     2484 2024-03-26 10:15:12.000000 neural_compressor_3x_ort-2.5/neural_compressor/common/utils/utility.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 10:15:46.369769 neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/
--rw-r--r--   0 root         (0) root         (0)     1652 2024-03-26 10:15:12.000000 neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 10:15:46.370769 neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/algorithms/
--rw-r--r--   0 root         (0) root         (0)     1090 2024-03-26 10:15:12.000000 neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/algorithms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 10:15:46.370769 neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/algorithms/layer_wise/
--rw-r--r--   0 root         (0) root         (0)      715 2024-03-26 10:15:12.000000 neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/algorithms/layer_wise/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11436 2024-03-26 10:15:12.000000 neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/algorithms/layer_wise/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 10:15:46.370769 neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/algorithms/smoother/
--rw-r--r--   0 root         (0) root         (0)      680 2024-03-26 10:15:12.000000 neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/algorithms/smoother/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9938 2024-03-26 10:15:12.000000 neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/algorithms/smoother/calibrator.py
--rw-r--r--   0 root         (0) root         (0)    29779 2024-03-26 10:15:12.000000 neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/algorithms/smoother/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 10:15:46.371769 neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/algorithms/weight_only/
--rw-r--r--   0 root         (0) root         (0)      584 2024-03-26 10:15:12.000000 neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/algorithms/weight_only/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19543 2024-03-26 10:15:12.000000 neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/algorithms/weight_only/awq.py
--rw-r--r--   0 root         (0) root         (0)    17436 2024-03-26 10:15:12.000000 neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/algorithms/weight_only/gptq.py
--rw-r--r--   0 root         (0) root         (0)     9444 2024-03-26 10:15:12.000000 neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/algorithms/weight_only/rtn.py
--rw-r--r--   0 root         (0) root         (0)    11468 2024-03-26 10:15:12.000000 neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/algorithms/weight_only/utility.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 10:15:46.372769 neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/quantization/
--rw-r--r--   0 root         (0) root         (0)     1550 2024-03-26 10:15:12.000000 neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/quantization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5968 2024-03-26 10:15:12.000000 neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/quantization/algorithm_entry.py
--rw-r--r--   0 root         (0) root         (0)     5254 2024-03-26 10:15:12.000000 neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/quantization/autotune.py
--rw-r--r--   0 root         (0) root         (0)     1164 2024-03-26 10:15:12.000000 neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/quantization/calibrate.py
--rw-r--r--   0 root         (0) root         (0)    25816 2024-03-26 10:15:12.000000 neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/quantization/config.py
--rw-r--r--   0 root         (0) root         (0)     2775 2024-03-26 10:15:12.000000 neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/quantization/quantize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 10:15:46.372769 neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/utils/
--rw-r--r--   0 root         (0) root         (0)      887 2024-03-26 10:15:12.000000 neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44048 2024-03-26 10:15:12.000000 neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/utils/onnx_model.py
--rw-r--r--   0 root         (0) root         (0)     9876 2024-03-26 10:15:12.000000 neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/utils/utility.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 10:15:46.373769 neural_compressor_3x_ort-2.5/neural_compressor_3x_ort.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15009 2024-03-26 10:15:46.000000 neural_compressor_3x_ort-2.5/neural_compressor_3x_ort.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1776 2024-03-26 10:15:46.000000 neural_compressor_3x_ort-2.5/neural_compressor_3x_ort.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-26 10:15:46.000000 neural_compressor_3x_ort-2.5/neural_compressor_3x_ort.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2024-03-26 10:15:46.000000 neural_compressor_3x_ort-2.5/neural_compressor_3x_ort.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-03-26 10:15:46.000000 neural_compressor_3x_ort-2.5/neural_compressor_3x_ort.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2418 2024-03-26 10:15:13.000000 neural_compressor_3x_ort-2.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      102 2024-03-26 10:15:46.374769 neural_compressor_3x_ort-2.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     8675 2024-03-26 10:15:13.000000 neural_compressor_3x_ort-2.5/setup.py
--rw-r--r--   0 root         (0) root         (0)    95740 2024-03-26 10:15:13.000000 neural_compressor_3x_ort-2.5/third-party-programs.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:43.480173 neural_compressor_3x_ort-2.5.1/
+-rw-r--r--   0 root         (0) root         (0)    11360 2024-04-03 13:33:19.000000 neural_compressor_3x_ort-2.5.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    15059 2024-04-03 13:34:43.480173 neural_compressor_3x_ort-2.5.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14096 2024-04-03 13:33:19.000000 neural_compressor_3x_ort-2.5.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:43.473173 neural_compressor_3x_ort-2.5.1/neural_compressor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:43.475173 neural_compressor_3x_ort-2.5.1/neural_compressor/common/
+-rw-r--r--   0 root         (0) root         (0)     1059 2024-04-03 13:33:19.000000 neural_compressor_3x_ort-2.5.1/neural_compressor/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23884 2024-04-03 13:33:19.000000 neural_compressor_3x_ort-2.5.1/neural_compressor/common/base_config.py
+-rw-r--r--   0 root         (0) root         (0)    12807 2024-04-03 13:33:19.000000 neural_compressor_3x_ort-2.5.1/neural_compressor/common/base_tuning.py
+-rw-r--r--   0 root         (0) root         (0)     3298 2024-04-03 13:33:19.000000 neural_compressor_3x_ort-2.5.1/neural_compressor/common/tuning_param.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:43.476173 neural_compressor_3x_ort-2.5.1/neural_compressor/common/utils/
+-rw-r--r--   0 root         (0) root         (0)      932 2024-04-03 13:33:19.000000 neural_compressor_3x_ort-2.5.1/neural_compressor/common/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1284 2024-04-03 13:33:19.000000 neural_compressor_3x_ort-2.5.1/neural_compressor/common/utils/constants.py
+-rw-r--r--   0 root         (0) root         (0)     6009 2024-04-03 13:33:19.000000 neural_compressor_3x_ort-2.5.1/neural_compressor/common/utils/logger.py
+-rw-r--r--   0 root         (0) root         (0)     2147 2024-04-03 13:33:19.000000 neural_compressor_3x_ort-2.5.1/neural_compressor/common/utils/save_load.py
+-rw-r--r--   0 root         (0) root         (0)     6548 2024-04-03 13:33:19.000000 neural_compressor_3x_ort-2.5.1/neural_compressor/common/utils/utility.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:43.476173 neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/
+-rw-r--r--   0 root         (0) root         (0)     1652 2024-04-03 13:33:19.000000 neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:43.476173 neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/algorithms/
+-rw-r--r--   0 root         (0) root         (0)     1090 2024-04-03 13:33:19.000000 neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/algorithms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:43.477173 neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/algorithms/layer_wise/
+-rw-r--r--   0 root         (0) root         (0)      715 2024-04-03 13:33:19.000000 neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/algorithms/layer_wise/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11436 2024-04-03 13:33:19.000000 neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/algorithms/layer_wise/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:43.477173 neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/algorithms/smoother/
+-rw-r--r--   0 root         (0) root         (0)      680 2024-04-03 13:33:19.000000 neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/algorithms/smoother/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9938 2024-04-03 13:33:19.000000 neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/algorithms/smoother/calibrator.py
+-rw-r--r--   0 root         (0) root         (0)    29779 2024-04-03 13:33:19.000000 neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/algorithms/smoother/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:43.478173 neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/algorithms/weight_only/
+-rw-r--r--   0 root         (0) root         (0)      584 2024-04-03 13:33:19.000000 neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/algorithms/weight_only/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19543 2024-04-03 13:33:19.000000 neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/algorithms/weight_only/awq.py
+-rw-r--r--   0 root         (0) root         (0)    17436 2024-04-03 13:33:19.000000 neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/algorithms/weight_only/gptq.py
+-rw-r--r--   0 root         (0) root         (0)     9444 2024-04-03 13:33:19.000000 neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/algorithms/weight_only/rtn.py
+-rw-r--r--   0 root         (0) root         (0)    11468 2024-04-03 13:33:19.000000 neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/algorithms/weight_only/utility.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:43.479173 neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/quantization/
+-rw-r--r--   0 root         (0) root         (0)     1550 2024-04-03 13:33:19.000000 neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/quantization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5968 2024-04-03 13:33:19.000000 neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/quantization/algorithm_entry.py
+-rw-r--r--   0 root         (0) root         (0)     5254 2024-04-03 13:33:19.000000 neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/quantization/autotune.py
+-rw-r--r--   0 root         (0) root         (0)     1164 2024-04-03 13:33:19.000000 neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/quantization/calibrate.py
+-rw-r--r--   0 root         (0) root         (0)    25816 2024-04-03 13:33:19.000000 neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/quantization/config.py
+-rw-r--r--   0 root         (0) root         (0)     2775 2024-04-03 13:33:19.000000 neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/quantization/quantize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:43.479173 neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/utils/
+-rw-r--r--   0 root         (0) root         (0)      887 2024-04-03 13:33:19.000000 neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44048 2024-04-03 13:33:19.000000 neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/utils/onnx_model.py
+-rw-r--r--   0 root         (0) root         (0)     9876 2024-04-03 13:33:19.000000 neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/utils/utility.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:43.480173 neural_compressor_3x_ort-2.5.1/neural_compressor_3x_ort.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15059 2024-04-03 13:34:43.000000 neural_compressor_3x_ort-2.5.1/neural_compressor_3x_ort.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1776 2024-04-03 13:34:43.000000 neural_compressor_3x_ort-2.5.1/neural_compressor_3x_ort.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 13:34:43.000000 neural_compressor_3x_ort-2.5.1/neural_compressor_3x_ort.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-03 13:34:43.000000 neural_compressor_3x_ort-2.5.1/neural_compressor_3x_ort.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-04-03 13:34:43.000000 neural_compressor_3x_ort-2.5.1/neural_compressor_3x_ort.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2418 2024-04-03 13:33:19.000000 neural_compressor_3x_ort-2.5.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      102 2024-04-03 13:34:43.481173 neural_compressor_3x_ort-2.5.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8675 2024-04-03 13:33:19.000000 neural_compressor_3x_ort-2.5.1/setup.py
+-rw-r--r--   0 root         (0) root         (0)    95740 2024-04-03 13:33:19.000000 neural_compressor_3x_ort-2.5.1/third-party-programs.txt
```

### Comparing `neural_compressor_3x_ort-2.5/LICENSE` & `neural_compressor_3x_ort-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_ort-2.5/PKG-INFO` & `neural_compressor_3x_ort-2.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neural_compressor_3x_ort
-Version: 2.5
+Version: 2.5.1
 Summary: Repository of Intel® Neural Compressor
 Home-page: https://github.com/intel/neural-compressor
 Author: Intel AIPT Team
 Author-email: feng.tian@intel.com, haihao.shen@intel.com, suyue.chen@intel.com
 License: Apache 2.0
 Keywords: quantization,auto-tuning,post-training static quantization,post-training dynamic quantization,quantization-aware training
 Classifier: Intended Audience :: Science/Research
@@ -15,14 +15,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: third-party-programs.txt
 Requires-Dist: numpy
 Requires-Dist: onnx
 Requires-Dist: onnxruntime
 Requires-Dist: onnxruntime-extensions
+Requires-Dist: psutil
+Requires-Dist: py-cpuinfo
 Requires-Dist: pydantic
 
 <div align="center">
 
 Intel® Neural Compressor
 ===========================
 <h3> An open-source Python library supporting popular model compression techniques on all mainstream deep learning frameworks (TensorFlow, PyTorch, ONNX Runtime, and MXNet)</h3>
```

### Comparing `neural_compressor_3x_ort-2.5/README.md` & `neural_compressor_3x_ort-2.5.1/README.md`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_ort-2.5/neural_compressor/common/__init__.py` & `neural_compressor_3x_ort-2.5.1/neural_compressor/common/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_ort-2.5/neural_compressor/common/base_config.py` & `neural_compressor_3x_ort-2.5.1/neural_compressor/common/base_config.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_ort-2.5/neural_compressor/common/base_tuning.py` & `neural_compressor_3x_ort-2.5.1/neural_compressor/common/base_tuning.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_ort-2.5/neural_compressor/common/tuning_param.py` & `neural_compressor_3x_ort-2.5.1/neural_compressor/common/tuning_param.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_ort-2.5/neural_compressor/common/utils/__init__.py` & `neural_compressor_3x_ort-2.5.1/neural_compressor/common/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_ort-2.5/neural_compressor/common/utils/constants.py` & `neural_compressor_3x_ort-2.5.1/neural_compressor/common/utils/constants.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_ort-2.5/neural_compressor/common/utils/logger.py` & `neural_compressor_3x_ort-2.5.1/neural_compressor/common/utils/logger.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_ort-2.5/neural_compressor/common/utils/save_load.py` & `neural_compressor_3x_ort-2.5.1/neural_compressor/common/utils/save_load.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/__init__.py` & `neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/algorithms/__init__.py` & `neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/algorithms/layer_wise/__init__.py` & `neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/algorithms/layer_wise/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/algorithms/layer_wise/core.py` & `neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/algorithms/layer_wise/core.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/algorithms/smoother/__init__.py` & `neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/algorithms/smoother/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/algorithms/smoother/calibrator.py` & `neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/algorithms/smoother/calibrator.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/algorithms/smoother/core.py` & `neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/algorithms/smoother/core.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/algorithms/weight_only/__init__.py` & `neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/algorithms/weight_only/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/algorithms/weight_only/awq.py` & `neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/algorithms/weight_only/awq.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/algorithms/weight_only/gptq.py` & `neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/algorithms/weight_only/gptq.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/algorithms/weight_only/rtn.py` & `neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/algorithms/weight_only/rtn.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/algorithms/weight_only/utility.py` & `neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/algorithms/weight_only/utility.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/quantization/__init__.py` & `neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/quantization/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/quantization/algorithm_entry.py` & `neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/quantization/algorithm_entry.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/quantization/autotune.py` & `neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/quantization/autotune.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/quantization/calibrate.py` & `neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/quantization/calibrate.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/quantization/config.py` & `neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/quantization/config.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/quantization/quantize.py` & `neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/quantization/quantize.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/utils/__init__.py` & `neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/utils/onnx_model.py` & `neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/utils/onnx_model.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_ort-2.5/neural_compressor/onnxrt/utils/utility.py` & `neural_compressor_3x_ort-2.5.1/neural_compressor/onnxrt/utils/utility.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_ort-2.5/neural_compressor_3x_ort.egg-info/PKG-INFO` & `neural_compressor_3x_ort-2.5.1/neural_compressor_3x_ort.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neural_compressor_3x_ort
-Version: 2.5
+Version: 2.5.1
 Summary: Repository of Intel® Neural Compressor
 Home-page: https://github.com/intel/neural-compressor
 Author: Intel AIPT Team
 Author-email: feng.tian@intel.com, haihao.shen@intel.com, suyue.chen@intel.com
 License: Apache 2.0
 Keywords: quantization,auto-tuning,post-training static quantization,post-training dynamic quantization,quantization-aware training
 Classifier: Intended Audience :: Science/Research
@@ -15,14 +15,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: third-party-programs.txt
 Requires-Dist: numpy
 Requires-Dist: onnx
 Requires-Dist: onnxruntime
 Requires-Dist: onnxruntime-extensions
+Requires-Dist: psutil
+Requires-Dist: py-cpuinfo
 Requires-Dist: pydantic
 
 <div align="center">
 
 Intel® Neural Compressor
 ===========================
 <h3> An open-source Python library supporting popular model compression techniques on all mainstream deep learning frameworks (TensorFlow, PyTorch, ONNX Runtime, and MXNet)</h3>
```

### Comparing `neural_compressor_3x_ort-2.5/neural_compressor_3x_ort.egg-info/SOURCES.txt` & `neural_compressor_3x_ort-2.5.1/neural_compressor_3x_ort.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_ort-2.5/pyproject.toml` & `neural_compressor_3x_ort-2.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_ort-2.5/setup.py` & `neural_compressor_3x_ort-2.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_ort-2.5/third-party-programs.txt` & `neural_compressor_3x_ort-2.5.1/third-party-programs.txt`

 * *Files identical despite different names*

