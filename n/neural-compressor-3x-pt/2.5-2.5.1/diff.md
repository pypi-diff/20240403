# Comparing `tmp/neural_compressor_3x_pt-2.5.tar.gz` & `tmp/neural_compressor_3x_pt-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neural_compressor_3x_pt-2.5.tar", last modified: Tue Mar 26 09:10:39 2024, max compression
+gzip compressed data, was "neural_compressor_3x_pt-2.5.1.tar", last modified: Wed Apr  3 13:34:24 2024, max compression
```

## Comparing `neural_compressor_3x_pt-2.5.tar` & `neural_compressor_3x_pt-2.5.1.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:10:39.938958 neural_compressor_3x_pt-2.5/
--rw-r--r--   0 root         (0) root         (0)    11360 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)    15038 2024-03-26 09:10:39.938958 neural_compressor_3x_pt-2.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    14096 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:10:39.927958 neural_compressor_3x_pt-2.5/neural_compressor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:10:39.929958 neural_compressor_3x_pt-2.5/neural_compressor/common/
--rw-r--r--   0 root         (0) root         (0)     1059 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23884 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/common/base_config.py
--rw-r--r--   0 root         (0) root         (0)    12807 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/common/base_tuning.py
--rw-r--r--   0 root         (0) root         (0)     3298 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/common/tuning_param.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:10:39.930958 neural_compressor_3x_pt-2.5/neural_compressor/common/utils/
--rw-r--r--   0 root         (0) root         (0)      932 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/common/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1284 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/common/utils/constants.py
--rw-r--r--   0 root         (0) root         (0)     6009 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/common/utils/logger.py
--rw-r--r--   0 root         (0) root         (0)     2147 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/common/utils/save_load.py
--rw-r--r--   0 root         (0) root         (0)     2484 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/common/utils/utility.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:10:39.930958 neural_compressor_3x_pt-2.5/neural_compressor/torch/
--rw-r--r--   0 root         (0) root         (0)      584 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:10:39.930958 neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/
--rw-r--r--   0 root         (0) root         (0)      584 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:10:39.931958 neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/habana_fp8/
--rw-r--r--   0 root         (0) root         (0)      681 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/habana_fp8/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8332 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/habana_fp8/fp8_quant.py
--rw-r--r--   0 root         (0) root         (0)    16036 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/habana_fp8/modules.py
--rw-r--r--   0 root         (0) root         (0)    18747 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/habana_fp8/observer.py
--rw-r--r--   0 root         (0) root         (0)     4016 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/habana_fp8/save_load.py
--rw-r--r--   0 root         (0) root         (0)     1689 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/habana_fp8/scale.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:10:39.931958 neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/habana_fp8/tensor/
--rw-r--r--   0 root         (0) root         (0)      584 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/habana_fp8/tensor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:10:39.932958 neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/layer_wise/
--rw-r--r--   0 root         (0) root         (0)      696 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/layer_wise/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12959 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/layer_wise/load.py
--rw-r--r--   0 root         (0) root         (0)    64065 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/layer_wise/modified_pickle.py
--rw-r--r--   0 root         (0) root         (0)    10545 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/layer_wise/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:10:39.932958 neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/smooth_quant/
--rw-r--r--   0 root         (0) root         (0)      728 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/smooth_quant/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3144 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/smooth_quant/save_load.py
--rw-r--r--   0 root         (0) root         (0)    10938 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/smooth_quant/smooth_quant.py
--rw-r--r--   0 root         (0) root         (0)   104961 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/smooth_quant/utility.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:10:39.933958 neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/static_quant/
--rw-r--r--   0 root         (0) root         (0)      703 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/static_quant/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1809 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/static_quant/save_load.py
--rw-r--r--   0 root         (0) root         (0)     5337 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/static_quant/static_quant.py
--rw-r--r--   0 root         (0) root         (0)    29460 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/static_quant/utility.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:10:39.934958 neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/weight_only/
--rw-r--r--   0 root         (0) root         (0)      840 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/weight_only/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8857 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/weight_only/autoround.py
--rw-r--r--   0 root         (0) root         (0)    24261 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/weight_only/awq.py
--rw-r--r--   0 root         (0) root         (0)    51755 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/weight_only/gptq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:10:39.935958 neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/weight_only/hqq/
--rw-r--r--   0 root         (0) root         (0)      707 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/weight_only/hqq/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5299 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/weight_only/hqq/bitpack.py
--rw-r--r--   0 root         (0) root         (0)     2677 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/weight_only/hqq/config.py
--rw-r--r--   0 root         (0) root         (0)    10404 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/weight_only/hqq/core.py
--rw-r--r--   0 root         (0) root         (0)     2716 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/weight_only/hqq/optimizer.py
--rw-r--r--   0 root         (0) root         (0)     3482 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/weight_only/hqq/qtensor.py
--rw-r--r--   0 root         (0) root         (0)     2459 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/weight_only/hqq/quant_api.py
--rw-r--r--   0 root         (0) root         (0)     3817 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/weight_only/hqq/quantizer.py
--rw-r--r--   0 root         (0) root         (0)     2494 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/weight_only/hqq/utility.py
--rw-r--r--   0 root         (0) root         (0)    18331 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/weight_only/modules.py
--rw-r--r--   0 root         (0) root         (0)     7827 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/weight_only/rtn.py
--rw-r--r--   0 root         (0) root         (0)    14188 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/weight_only/teq.py
--rw-r--r--   0 root         (0) root         (0)    40105 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/weight_only/utility.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:10:39.936958 neural_compressor_3x_pt-2.5/neural_compressor/torch/amp/
--rw-r--r--   0 root         (0) root         (0)      616 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/amp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4253 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/amp/autocast.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:10:39.936958 neural_compressor_3x_pt-2.5/neural_compressor/torch/amp/fp8/
--rw-r--r--   0 root         (0) root         (0)      584 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/amp/fp8/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4410 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/amp/fp8/functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:10:39.937958 neural_compressor_3x_pt-2.5/neural_compressor/torch/quantization/
--rw-r--r--   0 root         (0) root         (0)     1525 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/quantization/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17379 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/quantization/algorithm_entry.py
--rw-r--r--   0 root         (0) root         (0)     3850 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/quantization/autotune.py
--rw-r--r--   0 root         (0) root         (0)    41405 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/quantization/config.py
--rw-r--r--   0 root         (0) root         (0)     1489 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/quantization/load_entry.py
--rw-r--r--   0 root         (0) root         (0)     3429 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/quantization/quantize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:10:39.937958 neural_compressor_3x_pt-2.5/neural_compressor/torch/utils/
--rw-r--r--   0 root         (0) root         (0)      656 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8468 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/utils/auto_accelerator.py
--rw-r--r--   0 root         (0) root         (0)     1565 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/utils/constants.py
--rw-r--r--   0 root         (0) root         (0)     1915 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/utils/environ.py
--rw-r--r--   0 root         (0) root         (0)     3911 2024-03-26 08:53:13.000000 neural_compressor_3x_pt-2.5/neural_compressor/torch/utils/utility.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:10:39.938958 neural_compressor_3x_pt-2.5/neural_compressor_3x_pt.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15038 2024-03-26 09:10:39.000000 neural_compressor_3x_pt-2.5/neural_compressor_3x_pt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3596 2024-03-26 09:10:39.000000 neural_compressor_3x_pt-2.5/neural_compressor_3x_pt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-26 09:10:39.000000 neural_compressor_3x_pt-2.5/neural_compressor_3x_pt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       70 2024-03-26 09:10:39.000000 neural_compressor_3x_pt-2.5/neural_compressor_3x_pt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-03-26 09:10:39.000000 neural_compressor_3x_pt-2.5/neural_compressor_3x_pt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2418 2024-03-26 08:53:14.000000 neural_compressor_3x_pt-2.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      102 2024-03-26 09:10:39.939958 neural_compressor_3x_pt-2.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     8675 2024-03-26 08:53:14.000000 neural_compressor_3x_pt-2.5/setup.py
--rw-r--r--   0 root         (0) root         (0)    95740 2024-03-26 08:53:14.000000 neural_compressor_3x_pt-2.5/third-party-programs.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:24.434451 neural_compressor_3x_pt-2.5.1/
+-rw-r--r--   0 root         (0) root         (0)    11360 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    15062 2024-04-03 13:34:24.434451 neural_compressor_3x_pt-2.5.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14096 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:24.422451 neural_compressor_3x_pt-2.5.1/neural_compressor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:24.424451 neural_compressor_3x_pt-2.5.1/neural_compressor/common/
+-rw-r--r--   0 root         (0) root         (0)     1059 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23884 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/common/base_config.py
+-rw-r--r--   0 root         (0) root         (0)    12807 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/common/base_tuning.py
+-rw-r--r--   0 root         (0) root         (0)     3298 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/common/tuning_param.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:24.425451 neural_compressor_3x_pt-2.5.1/neural_compressor/common/utils/
+-rw-r--r--   0 root         (0) root         (0)      932 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/common/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1284 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/common/utils/constants.py
+-rw-r--r--   0 root         (0) root         (0)     6009 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/common/utils/logger.py
+-rw-r--r--   0 root         (0) root         (0)     2147 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/common/utils/save_load.py
+-rw-r--r--   0 root         (0) root         (0)     6548 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/common/utils/utility.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:24.425451 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/
+-rw-r--r--   0 root         (0) root         (0)      584 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:24.425451 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/
+-rw-r--r--   0 root         (0) root         (0)      584 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:24.426451 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/habana_fp8/
+-rw-r--r--   0 root         (0) root         (0)      681 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/habana_fp8/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8332 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/habana_fp8/fp8_quant.py
+-rw-r--r--   0 root         (0) root         (0)    16036 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/habana_fp8/modules.py
+-rw-r--r--   0 root         (0) root         (0)    18747 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/habana_fp8/observer.py
+-rw-r--r--   0 root         (0) root         (0)     4016 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/habana_fp8/save_load.py
+-rw-r--r--   0 root         (0) root         (0)     1689 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/habana_fp8/scale.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:24.426451 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/habana_fp8/tensor/
+-rw-r--r--   0 root         (0) root         (0)      584 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/habana_fp8/tensor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:24.427451 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/layer_wise/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/layer_wise/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12959 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/layer_wise/load.py
+-rw-r--r--   0 root         (0) root         (0)    64065 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/layer_wise/modified_pickle.py
+-rw-r--r--   0 root         (0) root         (0)    10545 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/layer_wise/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:24.427451 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/smooth_quant/
+-rw-r--r--   0 root         (0) root         (0)      728 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/smooth_quant/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3144 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/smooth_quant/save_load.py
+-rw-r--r--   0 root         (0) root         (0)    10938 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/smooth_quant/smooth_quant.py
+-rw-r--r--   0 root         (0) root         (0)   104961 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/smooth_quant/utility.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:24.428451 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/static_quant/
+-rw-r--r--   0 root         (0) root         (0)      703 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/static_quant/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1809 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/static_quant/save_load.py
+-rw-r--r--   0 root         (0) root         (0)     5337 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/static_quant/static_quant.py
+-rw-r--r--   0 root         (0) root         (0)    29460 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/static_quant/utility.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:24.429451 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/weight_only/
+-rw-r--r--   0 root         (0) root         (0)      840 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/weight_only/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8857 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/weight_only/autoround.py
+-rw-r--r--   0 root         (0) root         (0)    24261 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/weight_only/awq.py
+-rw-r--r--   0 root         (0) root         (0)    52210 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/weight_only/gptq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:24.431451 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/weight_only/hqq/
+-rw-r--r--   0 root         (0) root         (0)      707 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/weight_only/hqq/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5299 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/weight_only/hqq/bitpack.py
+-rw-r--r--   0 root         (0) root         (0)     2677 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/weight_only/hqq/config.py
+-rw-r--r--   0 root         (0) root         (0)    10404 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/weight_only/hqq/core.py
+-rw-r--r--   0 root         (0) root         (0)     2716 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/weight_only/hqq/optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     3482 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/weight_only/hqq/qtensor.py
+-rw-r--r--   0 root         (0) root         (0)     2459 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/weight_only/hqq/quant_api.py
+-rw-r--r--   0 root         (0) root         (0)     3817 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/weight_only/hqq/quantizer.py
+-rw-r--r--   0 root         (0) root         (0)     2494 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/weight_only/hqq/utility.py
+-rw-r--r--   0 root         (0) root         (0)    18331 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/weight_only/modules.py
+-rw-r--r--   0 root         (0) root         (0)     7826 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/weight_only/rtn.py
+-rw-r--r--   0 root         (0) root         (0)    14188 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/weight_only/teq.py
+-rw-r--r--   0 root         (0) root         (0)    40354 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/weight_only/utility.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:24.431451 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/amp/
+-rw-r--r--   0 root         (0) root         (0)      616 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/amp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4253 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/amp/autocast.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:24.431451 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/amp/fp8/
+-rw-r--r--   0 root         (0) root         (0)      584 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/amp/fp8/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4410 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/amp/fp8/functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:24.432451 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/quantization/
+-rw-r--r--   0 root         (0) root         (0)     1525 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/quantization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17379 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/quantization/algorithm_entry.py
+-rw-r--r--   0 root         (0) root         (0)     3850 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/quantization/autotune.py
+-rw-r--r--   0 root         (0) root         (0)    41405 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/quantization/config.py
+-rw-r--r--   0 root         (0) root         (0)     1489 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/quantization/load_entry.py
+-rw-r--r--   0 root         (0) root         (0)     3429 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/quantization/quantize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:24.433451 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/utils/
+-rw-r--r--   0 root         (0) root         (0)      656 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8772 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/utils/auto_accelerator.py
+-rw-r--r--   0 root         (0) root         (0)     1565 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/utils/constants.py
+-rw-r--r--   0 root         (0) root         (0)     1915 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/utils/environ.py
+-rw-r--r--   0 root         (0) root         (0)     3911 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/neural_compressor/torch/utils/utility.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:24.434451 neural_compressor_3x_pt-2.5.1/neural_compressor_3x_pt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15062 2024-04-03 13:34:24.000000 neural_compressor_3x_pt-2.5.1/neural_compressor_3x_pt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3596 2024-04-03 13:34:24.000000 neural_compressor_3x_pt-2.5.1/neural_compressor_3x_pt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 13:34:24.000000 neural_compressor_3x_pt-2.5.1/neural_compressor_3x_pt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       77 2024-04-03 13:34:24.000000 neural_compressor_3x_pt-2.5.1/neural_compressor_3x_pt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-04-03 13:34:24.000000 neural_compressor_3x_pt-2.5.1/neural_compressor_3x_pt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2418 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      102 2024-04-03 13:34:24.434451 neural_compressor_3x_pt-2.5.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8675 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/setup.py
+-rw-r--r--   0 root         (0) root         (0)    95740 2024-04-03 13:33:19.000000 neural_compressor_3x_pt-2.5.1/third-party-programs.txt
```

### Comparing `neural_compressor_3x_pt-2.5/LICENSE` & `neural_compressor_3x_pt-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/PKG-INFO` & `neural_compressor_3x_pt-2.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neural_compressor_3x_pt
-Version: 2.5
+Version: 2.5.1
 Summary: Repository of Intel® Neural Compressor
 Home-page: https://github.com/intel/neural-compressor
 Author: Intel AIPT Team
 Author-email: feng.tian@intel.com, haihao.shen@intel.com, suyue.chen@intel.com
 License: Apache 2.0
 Keywords: quantization,auto-tuning,post-training static quantization,post-training dynamic quantization,quantization-aware training
 Classifier: Intended Audience :: Science/Research
@@ -14,14 +14,15 @@
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: third-party-programs.txt
 Requires-Dist: auto-round
 Requires-Dist: intel_extension_for_pytorch
 Requires-Dist: peft
+Requires-Dist: psutil
 Requires-Dist: py-cpuinfo
 Requires-Dist: pydantic
 Requires-Dist: torch
 
 <div align="center">
 
 Intel® Neural Compressor
```

### Comparing `neural_compressor_3x_pt-2.5/README.md` & `neural_compressor_3x_pt-2.5.1/README.md`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/common/__init__.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/common/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/common/base_config.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/common/base_config.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/common/base_tuning.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/common/base_tuning.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/common/tuning_param.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/common/tuning_param.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/common/utils/__init__.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/common/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/common/utils/constants.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/common/utils/constants.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/common/utils/logger.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/common/utils/logger.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/common/utils/save_load.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/common/utils/save_load.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/__init__.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/__init__.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/habana_fp8/__init__.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/habana_fp8/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/habana_fp8/fp8_quant.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/habana_fp8/fp8_quant.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/habana_fp8/modules.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/habana_fp8/modules.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/habana_fp8/observer.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/habana_fp8/observer.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/habana_fp8/save_load.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/habana_fp8/save_load.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/habana_fp8/scale.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/habana_fp8/scale.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/habana_fp8/tensor/__init__.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/habana_fp8/tensor/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/layer_wise/__init__.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/layer_wise/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/layer_wise/load.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/layer_wise/load.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/layer_wise/modified_pickle.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/layer_wise/modified_pickle.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/layer_wise/utils.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/layer_wise/utils.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/smooth_quant/__init__.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/smooth_quant/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/smooth_quant/save_load.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/smooth_quant/save_load.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/smooth_quant/smooth_quant.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/smooth_quant/smooth_quant.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/smooth_quant/utility.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/smooth_quant/utility.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/static_quant/__init__.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/static_quant/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/static_quant/save_load.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/static_quant/save_load.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/static_quant/static_quant.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/static_quant/static_quant.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/static_quant/utility.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/static_quant/utility.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/weight_only/__init__.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/weight_only/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/weight_only/autoround.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/weight_only/autoround.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/weight_only/awq.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/weight_only/awq.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/weight_only/gptq.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/weight_only/gptq.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
 from neural_compressor.torch.utils import fetch_module, get_device, logger, set_module
 from neural_compressor.torch.utils.auto_accelerator import auto_detect_accelerator
 
 from .modules import WeightOnlyLinear
 
 DEBUG = False
+accelerator = auto_detect_accelerator()
 
 
 # ================ device related ===================
 def move_input_to_device(input, device=torch.device("cpu")):
     if isinstance(input, dict) or isinstance(input, UserDict):
         for inp in input.keys():
             input[inp] = input[inp].to(device) if isinstance(input[inp], torch.Tensor) else input[inp]
@@ -538,16 +539,18 @@
 
         # Step3: run forward to obtain calibration datasets
         logger.info("Collecting calibration inputs...")
         logger.info("Collecting calibration inputs by running the run_fn provided by user.")
         if self.run_fn:
             if self.run_args:
                 self.run_fn(self.model, *self.run_args)
+                accelerator.mark_step()
             else:
                 self.run_fn(self.model)
+                accelerator.mark_step()
         else:
             for batch in tqdm(self.dataloader):
                 if not self.use_layer_wise:
                     batch = move_input_to_device(batch, self.device)
                 try:
                     if isinstance(batch, tuple) or isinstance(batch, list):
                         self.model(batch[0])
@@ -659,14 +662,15 @@
             handles = []  # register handles which add inputs and outputs to gptq object
             for layer_name in sub_layers:
                 handles.append(sub_layers[layer_name].register_forward_hook(add_batch(layer_name)))
             batch_num = self.cache_key_arguments.pop("batch_num")
             for j in range(batch_num):
                 cache_keyword_batch = self.gather_single_batch_from_dict(self.cache_key_arguments, j)
                 cache_positional_batch = self.gather_single_batch_from_list(self.cache_positional_arguments, j)
+                accelerator.mark_step()
                 out = transformer_block(*cache_positional_batch, **cache_keyword_batch)
                 out = self.track_hidden_states(out)
             self.cache_key_arguments["batch_num"] = batch_num
             for h in handles:
                 h.remove()
             # Step 2.4: everything is prepared, so start quantization!
             for layer_name in sub_layers:
@@ -678,14 +682,17 @@
                 if self.use_layer_wise:
                     from neural_compressor.torch.algorithms.layer_wise import load_value
 
                     full_layer_name = self.get_full_layer_name(layer_name, block_idx)
                     W = load_value(self.model, full_layer_name + ".weight", model_path)
                 else:
                     W = sub_layers[layer_name].weight.data.clone()
+                accelerator.mark_step()
+                if "hpu" in self.device:
+                    W = W.to("cpu")
                 scale, zp, Q = gptq_for_this_block[layer_name].fasterquant(
                     W,
                     blocksize=weight_config_this_layer["block_size"],
                     percdamp=weight_config_this_layer["percdamp"],
                     groupsize=weight_config_this_layer["group_size"],
                     act_order=weight_config_this_layer["act_order"],
                     static_groups=weight_config_this_layer["static_groups"],
@@ -850,14 +857,16 @@
 
         tick = time.time()
 
         if not self.quantizer.ready():
             self.quantizer.find_params(W, weight=True)
 
         H = self.H
+        if "hpu" in self.device:
+            H = H.to("cpu")
         del self.H
         dead = torch.diag(H) == 0
         H[dead, dead] = 1
         W[:, dead] = 0  # such channel makes no contribution to quantization computation
 
         # enable static_groups
         # calculate the quantization parameters for original group in advance.
@@ -954,14 +963,18 @@
             logger.info(f"{torch.sum((self.layer(self.inp1) - self.out1) ** 2)}")
 
         if scale == []:
             scale.append(self.quantizer.scale)
             zero.append(self.quantizer.zero)
         scale = torch.cat(scale, dim=1)
         zero = torch.cat(zero, dim=1)
+        if "hpu" in self.device:
+            scale = scale.to(self.device)
+            zero = zero.to(self.device)
+            Q = Q.to(self.device)
         return scale, zero, Q
 
     def free(self):
         if DEBUG:
             self.inp1 = None
             self.out1 = None
         self.H = None
@@ -969,33 +982,33 @@
         self.Trace = None
         torch.cuda.empty_cache()
 
 
 class Quantizer(nn.Module):
     def __init__(self, shape=1):
         super(Quantizer, self).__init__()
-        self.register_buffer("maxq", torch.tensor(0))
+        self.maxq = 0
         self.register_buffer("scale", torch.zeros(shape))
         self.register_buffer("zero", torch.zeros(shape))
 
     def configure(self, weight_config_this_layer, norm=2.4, grid=100, maxshrink=0.8, trits=False):
         for k, v in weight_config_this_layer.items():
             setattr(self, k, v)
-        self.maxq = torch.tensor(2**self.bits - 1)
+        # self.maxq = torch.tensor(2**self.bits - 1)
+        self.maxq = 2**self.bits - 1
         self.scheme = "sym" if self.sym else "asym"
         self.double_quant_scheme = "sym" if self.double_quant_sym else "asym"
         self.norm = norm
         self.grid = grid
         self.maxshrink = maxshrink
         if trits:
-            self.maxq = torch.tensor(-1)
+            self.maxq = -1
 
     def find_params(self, x, weight=False):
         dev = x.device
-        self.maxq = self.maxq.to(dev)
         # NF4 FP4
         if self.dtype != "int":
             from .utility import quant_tensor
 
             tmp = x.clone()  # tmp will be replaced after quant_tensor
             _, scale, zero = quant_tensor(
                 tmp,
```

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/weight_only/hqq/__init__.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/weight_only/hqq/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/weight_only/hqq/bitpack.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/weight_only/hqq/bitpack.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/weight_only/hqq/config.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/weight_only/hqq/config.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/weight_only/hqq/core.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/weight_only/hqq/core.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/weight_only/hqq/optimizer.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/weight_only/hqq/optimizer.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/weight_only/hqq/qtensor.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/weight_only/hqq/qtensor.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/weight_only/hqq/quant_api.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/weight_only/hqq/quant_api.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/weight_only/hqq/quantizer.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/weight_only/hqq/quantizer.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/weight_only/hqq/utility.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/weight_only/hqq/utility.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/weight_only/modules.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/weight_only/modules.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/weight_only/rtn.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/weight_only/rtn.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,27 +77,27 @@
     device = get_device(kwargs.pop("device", "auto"))
 
     # Put model on device explicitly
     # TODO: refine it later, Put module on device one by one instead of the whole model
     model.to(device)
 
     assert isinstance(model, torch.nn.Module), "only support torch module"
-    supported_layers = ["Linear"]
+    supported_layers = (torch.nn.Linear,)
     # initialize global configuration
     double_quant_config = {
         "double_quant": kwargs.get("use_double_quant", False),
         "double_quant_dtype": kwargs.get("double_quant_dtype", "int"),
         "double_quant_bits": kwargs.get("double_quant_bits", 8),
         "double_quant_scheme": kwargs.get("double_quant_scheme", "sym"),
         "double_quant_group_size": kwargs.get("double_quant_group_size", 256),
     }
     if export_compressed_model:
         use_optimum_format = kwargs.get("use_optimum_format", True)
     for name, m in model.named_modules():
-        if m.__class__.__name__ not in supported_layers:
+        if not isinstance(m, supported_layers):
             continue
         if name in weight_config:  # pragma: no cover
             # initialize op configuration
             dtype = weight_config[name].get("dtype", "int")
             if dtype == "fp32":
                 continue
             logger.debug("Apply RTN on module %s.", name)
```

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/weight_only/teq.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/weight_only/teq.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/algorithms/weight_only/utility.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/algorithms/weight_only/utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -262,35 +262,40 @@
     if bits <= 0:  # pragma: no cover
         return weight
     # case 1, group size = -1
     if group_size == -1 or weight.shape[1] < group_size:
         group_size = weight.shape[1]
     # case 2, reshape based on group size
     orig_shape = weight.shape
+    orig_weight = weight
     if weight.shape[1] % group_size == 0:
         weight = weight.reshape(-1, group_size)
+        # return weight for unpacking scale and zp
         weight = qdq_weight_actor(
             weight,
             bits,
             scheme=scheme,
             quantile=quantile,
             return_int=return_int,
             full_range=full_range,
             dtype=dtype,
             **kwargs,
         )
         if return_int or quant_scale:
             weight, scale, zp = weight
             weight = weight.reshape(orig_shape)
+            orig_weight.copy_(weight)
             scale = scale.reshape(orig_shape[0], -1)
             if zp is not None:
                 zp = zp.reshape(orig_shape[0], -1)
-            q_state = weight, scale, zp
+            q_state = orig_weight, scale, zp
         else:
-            return weight.reshape(orig_shape)
+            weight = weight.reshape(orig_shape)
+            orig_weight.copy_(weight)
+            return orig_weight
     else:
         # case 3, process left part split by group size
         split_index = weight.shape[1] // group_size * group_size
         weight1 = weight[:, :split_index]
         weight1 = weight1.reshape(-1, group_size)
         weight1 = qdq_weight_actor(
             weight1,
@@ -317,21 +322,21 @@
             quantile=quantile,
             return_int=return_int,
             full_range=full_range,
             **kwargs,
         )
         if return_int or quant_scale:
             weight2, scale2, zp2 = weight2
-            weight.copy_(torch.cat([weight1, weight2], dim=1))
+            orig_weight.copy_(torch.cat([weight1, weight2], dim=1))
             scale = torch.cat([scale1, scale2], dim=1)
             zp = None if zp2 is None else torch.cat([zp1, zp2], dim=1)
             q_state = (weight, scale, zp)
         else:
-            weight.copy_(torch.cat([weight1, weight2], dim=1))
-            return weight
+            orig_weight.copy_(torch.cat([weight1, weight2], dim=1))
+            return orig_weight
     if quant_scale:
         weight, scale, zp = q_state
         scale_dtype = kwargs.get("double_quant_dtype", "int")
         scale_bits = kwargs.get("double_quant_bits", 8)
         scale_scheme = kwargs.get("double_quant_scheme", "asym")
         scale_group_size = kwargs.get("double_quant_group_size", 256)
         scale_return_int = kwargs.get("double_quant_return_int", return_int)
@@ -339,15 +344,15 @@
         scale = scale.reshape(1, -1)
         # pre-process: scale_mean
         if scale_scheme == "asym":
             scale_mean = scale.mean()
             scale.sub_(scale_mean)
             scale_scheme = "sym"
         # process: scale
-        scale = quant_tensor(
+        quant_tensor(
             scale,
             dtype=scale_dtype,
             bits=scale_bits,
             group_size=scale_group_size,
             scheme=scale_scheme,
             quantile=1.0,
             return_int=scale_return_int,
@@ -371,23 +376,24 @@
                     weight1 = weight1.reshape(-1, group_size).sub_(zp[:, :-1].reshape(-1, 1))
                     weight2 = weight2.sub_(zp[:, -1].reshape(-1, 1))
                 else:
                     weight1 = weight1.reshape(-1, group_size)
                 weight1 = weight1.mul_(scale[:, :-1].reshape(-1, 1))
                 weight1 = weight1.reshape(orig_shape[0], -1)
                 weight2 = weight2.mul_(scale[:, -1].reshape(-1, 1))
-                weight.copy_(torch.cat([weight1, weight2], dim=1))
+                orig_weight.copy_(torch.cat([weight1, weight2], dim=1))
             else:
                 if zp is not None:
                     weight = weight.reshape(-1, group_size) - zp.reshape(-1, 1)
                 else:
                     weight = weight.reshape(-1, group_size)
                 weight = weight.mul_(scale.reshape(-1, 1))
                 weight = weight.reshape(orig_shape[0], -1)
-            return weight
+                orig_weight.copy_(weight)
+            return orig_weight
     else:
         return q_state
 
 
 def search_clip(m, bits=4, group_size=32, scheme="asym", dtype="int", enable_full_range=False):
     """Search best clip range of each linear in current block. It's not an in-place function.
```

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/amp/__init__.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/amp/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/amp/autocast.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/amp/autocast.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/amp/fp8/__init__.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/amp/fp8/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/amp/fp8/functions.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/amp/fp8/functions.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/quantization/__init__.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/quantization/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/quantization/algorithm_entry.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/quantization/algorithm_entry.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/quantization/autotune.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/quantization/autotune.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/quantization/config.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/quantization/config.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/quantization/load_entry.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/quantization/load_entry.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/quantization/quantize.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/quantization/quantize.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/utils/__init__.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/utils/auto_accelerator.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/utils/auto_accelerator.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,16 +25,19 @@
 
 import os
 from abc import ABC, abstractmethod
 from typing import Any, Callable, List
 
 import torch
 
+from neural_compressor.common.utils import LazyImport
 from neural_compressor.torch.utils import logger
 
+htcore = LazyImport("habana_frameworks.torch.core")
+
 PRIORITY_HPU = 100
 PRIORITY_CUDA = 95
 PRIORITY_CPU = 90
 
 
 class AcceleratorRegistry:
     registered_accelerators = {}
@@ -129,14 +132,18 @@
     def empty_cache(self):
         pass
 
     @abstractmethod
     def synchronize(self):
         pass
 
+    @abstractmethod
+    def mark_step(self):
+        pass
+
 
 @register_accelerator(name="cpu", priority=PRIORITY_CPU)
 class CPU_Accelerator(Auto_Accelerator):
     def __init__(self) -> None:
         self._name = "cpu"
 
     def name(self) -> str:
@@ -163,14 +170,17 @@
 
     def empty_cache(self):
         pass
 
     def synchronize(self):
         pass
 
+    def mark_step(self):
+        pass
+
 
 @register_accelerator(name="cuda", priority=PRIORITY_CUDA)
 class CUDA_Accelerator(Auto_Accelerator):
     def __init__(self) -> None:
         self._name = "cuda"
 
     def name(self) -> str:
@@ -199,14 +209,17 @@
 
     def device(self, device_index=None):
         return torch.cuda.device(device_index)
 
     def empty_cache(self):
         return torch.cuda.empty_cache()
 
+    def mark_step(self):
+        pass
+
 
 @register_accelerator(name="hpu", priority=PRIORITY_HPU)
 class HPU_Accelerator(Auto_Accelerator):
     def __init__(self) -> None:
         self._name = "hpu"
 
     def name(self) -> str:
@@ -240,14 +253,17 @@
 
     def device(self, device_index=None):
         return torch.hpu.device(device_index)
 
     def empty_cache(self):
         return torch.hpu.empty_cache()
 
+    def mark_step(self):
+        return htcore.mark_step()
+
 
 def auto_detect_accelerator(device_name="auto") -> Auto_Accelerator:
     # Force use the cpu on node has both cpu and gpu: `FORCE_DEVICE=cpu` python main.py ...
     # The `FORCE_DEVICE` is case insensitive.
     # The environment variable `FORCE_DEVICE` has higher priority than the `device_name`.
     # TODO: refine the docs and logic later
     # 1. Get the device setting from environment variable `FORCE_DEVICE`.
```

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/utils/constants.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/utils/constants.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/utils/environ.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/utils/environ.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor/torch/utils/utility.py` & `neural_compressor_3x_pt-2.5.1/neural_compressor/torch/utils/utility.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor_3x_pt.egg-info/PKG-INFO` & `neural_compressor_3x_pt-2.5.1/neural_compressor_3x_pt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neural_compressor_3x_pt
-Version: 2.5
+Version: 2.5.1
 Summary: Repository of Intel® Neural Compressor
 Home-page: https://github.com/intel/neural-compressor
 Author: Intel AIPT Team
 Author-email: feng.tian@intel.com, haihao.shen@intel.com, suyue.chen@intel.com
 License: Apache 2.0
 Keywords: quantization,auto-tuning,post-training static quantization,post-training dynamic quantization,quantization-aware training
 Classifier: Intended Audience :: Science/Research
@@ -14,14 +14,15 @@
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: third-party-programs.txt
 Requires-Dist: auto-round
 Requires-Dist: intel_extension_for_pytorch
 Requires-Dist: peft
+Requires-Dist: psutil
 Requires-Dist: py-cpuinfo
 Requires-Dist: pydantic
 Requires-Dist: torch
 
 <div align="center">
 
 Intel® Neural Compressor
```

### Comparing `neural_compressor_3x_pt-2.5/neural_compressor_3x_pt.egg-info/SOURCES.txt` & `neural_compressor_3x_pt-2.5.1/neural_compressor_3x_pt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/pyproject.toml` & `neural_compressor_3x_pt-2.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/setup.py` & `neural_compressor_3x_pt-2.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_pt-2.5/third-party-programs.txt` & `neural_compressor_3x_pt-2.5.1/third-party-programs.txt`

 * *Files identical despite different names*

