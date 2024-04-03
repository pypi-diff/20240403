# Comparing `tmp/neural_compressor_3x_tf-2.5.tar.gz` & `tmp/neural_compressor_3x_tf-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neural_compressor_3x_tf-2.5.tar", last modified: Tue Mar 26 09:05:56 2024, max compression
+gzip compressed data, was "neural_compressor_3x_tf-2.5.1.tar", last modified: Wed Apr  3 13:34:05 2024, max compression
```

## Comparing `neural_compressor_3x_tf-2.5.tar` & `neural_compressor_3x_tf-2.5.1.tar`

### file list

```diff
@@ -1,172 +1,173 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:05:56.348227 neural_compressor_3x_tf-2.5/
--rw-r--r--   0 root         (0) root         (0)    11360 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)    15025 2024-03-26 09:05:56.348227 neural_compressor_3x_tf-2.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    14096 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:05:56.324226 neural_compressor_3x_tf-2.5/neural_compressor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:05:56.327226 neural_compressor_3x_tf-2.5/neural_compressor/common/
--rw-r--r--   0 root         (0) root         (0)     1059 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23884 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/common/base_config.py
--rw-r--r--   0 root         (0) root         (0)    12807 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/common/base_tuning.py
--rw-r--r--   0 root         (0) root         (0)     3298 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/common/tuning_param.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:05:56.327226 neural_compressor_3x_tf-2.5/neural_compressor/common/utils/
--rw-r--r--   0 root         (0) root         (0)      932 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/common/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1284 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/common/utils/constants.py
--rw-r--r--   0 root         (0) root         (0)     6009 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/common/utils/logger.py
--rw-r--r--   0 root         (0) root         (0)     2147 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/common/utils/save_load.py
--rw-r--r--   0 root         (0) root         (0)     2484 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/common/utils/utility.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:05:56.328226 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/
--rw-r--r--   0 root         (0) root         (0)      841 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:05:56.328226 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/algorithms/
--rw-r--r--   0 root         (0) root         (0)      756 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/algorithms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:05:56.328226 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/algorithms/smoother/
--rw-r--r--   0 root         (0) root         (0)      967 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/algorithms/smoother/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24234 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/algorithms/smoother/calibration.py
--rw-r--r--   0 root         (0) root         (0)     8107 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/algorithms/smoother/core.py
--rw-r--r--   0 root         (0) root         (0)    13846 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/algorithms/smoother/scaler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:05:56.329226 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/algorithms/static_quant/
--rw-r--r--   0 root         (0) root         (0)      763 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/algorithms/static_quant/__init__.py
--rw-r--r--   0 root         (0) root         (0)    34806 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/algorithms/static_quant/keras.py
--rw-r--r--   0 root         (0) root         (0)     5590 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/algorithms/static_quant/keras.yaml
--rw-r--r--   0 root         (0) root         (0)   111221 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/algorithms/static_quant/tensorflow.py
--rw-r--r--   0 root         (0) root         (0)    10015 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/algorithms/static_quant/tensorflow.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:05:56.329226 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/keras/
--rw-r--r--   0 root         (0) root         (0)      709 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/keras/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:05:56.330227 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/keras/layers/
--rw-r--r--   0 root         (0) root         (0)     1124 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/keras/layers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3737 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/keras/layers/conv2d.py
--rw-r--r--   0 root         (0) root         (0)     2568 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/keras/layers/dense.py
--rw-r--r--   0 root         (0) root         (0)     8226 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/keras/layers/depthwise_conv2d.py
--rw-r--r--   0 root         (0) root         (0)     1841 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/keras/layers/pool2d.py
--rw-r--r--   0 root         (0) root         (0)     4490 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/keras/layers/quantizer.py
--rw-r--r--   0 root         (0) root         (0)     8496 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/keras/layers/separable_conv2d.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:05:56.331226 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/keras/quantization/
--rw-r--r--   0 root         (0) root         (0)      716 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/keras/quantization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5236 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/keras/quantization/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:05:56.331226 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/
--rw-r--r--   0 root         (0) root         (0)     1039 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2300 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/algorithm_entry.py
--rw-r--r--   0 root         (0) root         (0)     3047 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/autotune.py
--rw-r--r--   0 root         (0) root         (0)     9219 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/config.py
--rw-r--r--   0 root         (0) root         (0)     3717 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/quantize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:05:56.332227 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/
--rw-r--r--   0 root         (0) root         (0)      584 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44033 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_converter.py
--rw-r--r--   0 root         (0) root         (0)    16692 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_converter_without_calib.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:05:56.333227 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/
--rw-r--r--   0 root         (0) root         (0)      584 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:05:56.333227 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/bf16/
--rw-r--r--   0 root         (0) root         (0)      669 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/bf16/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13962 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/bf16/bf16_convert.py
--rw-r--r--   0 root         (0) root         (0)     3248 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/bf16/dequantize_cast_optimizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:05:56.338227 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/
--rw-r--r--   0 root         (0) root         (0)      673 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3279 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/convert_add_to_biasadd.py
--rw-r--r--   0 root         (0) root         (0)     3897 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/convert_layout.py
--rw-r--r--   0 root         (0) root         (0)     3183 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/convert_leakyrelu.py
--rw-r--r--   0 root         (0) root         (0)     1946 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/convert_nan_to_random.py
--rw-r--r--   0 root         (0) root         (0)     4378 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/convert_placeholder_to_const.py
--rw-r--r--   0 root         (0) root         (0)     4108 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/dilated_contraction.py
--rw-r--r--   0 root         (0) root         (0)     5872 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/dummy_biasadd.py
--rw-r--r--   0 root         (0) root         (0)     3426 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/expanddims_optimizer.py
--rw-r--r--   0 root         (0) root         (0)     3985 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fetch_weight_from_reshape.py
--rw-r--r--   0 root         (0) root         (0)    13182 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fold_batch_norm.py
--rw-r--r--   0 root         (0) root         (0)     7525 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fold_constant.py
--rw-r--r--   0 root         (0) root         (0)     2920 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fuse_biasadd_add.py
--rw-r--r--   0 root         (0) root         (0)     3914 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fuse_column_wise_mul.py
--rw-r--r--   0 root         (0) root         (0)     4971 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fuse_conv_with_math.py
--rw-r--r--   0 root         (0) root         (0)    16463 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fuse_decomposed_bn.py
--rw-r--r--   0 root         (0) root         (0)    15598 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fuse_decomposed_in.py
--rw-r--r--   0 root         (0) root         (0)     9579 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fuse_gelu.py
--rw-r--r--   0 root         (0) root         (0)     9745 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fuse_layer_norm.py
--rw-r--r--   0 root         (0) root         (0)     5558 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fuse_pad_with_conv.py
--rw-r--r--   0 root         (0) root         (0)     5664 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fuse_pad_with_fp32_conv.py
--rw-r--r--   0 root         (0) root         (0)     5918 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fuse_reshape_transpose.py
--rw-r--r--   0 root         (0) root         (0)     5954 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/graph_cse_optimizer.py
--rw-r--r--   0 root         (0) root         (0)     3159 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/grappler_pass.py
--rw-r--r--   0 root         (0) root         (0)    12823 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/insert_print_node.py
--rw-r--r--   0 root         (0) root         (0)     6187 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/move_squeeze_after_relu.py
--rw-r--r--   0 root         (0) root         (0)    13726 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/pre_optimize.py
--rw-r--r--   0 root         (0) root         (0)     2795 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/remove_training_nodes.py
--rw-r--r--   0 root         (0) root         (0)     2345 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/rename_batch_norm.py
--rw-r--r--   0 root         (0) root         (0)     2647 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/split_shared_input.py
--rw-r--r--   0 root         (0) root         (0)     2135 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/strip_equivalent_nodes.py
--rw-r--r--   0 root         (0) root         (0)     1564 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/strip_unused_nodes.py
--rw-r--r--   0 root         (0) root         (0)     3448 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/switch_optimizer.py
--rw-r--r--   0 root         (0) root         (0)     1224 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/graph_base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:05:56.340227 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/
--rw-r--r--   0 root         (0) root         (0)      670 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7086 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/freeze_fake_quant.py
--rw-r--r--   0 root         (0) root         (0)    17685 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/freeze_value.py
--rw-r--r--   0 root         (0) root         (0)     5533 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/freeze_value_without_calib.py
--rw-r--r--   0 root         (0) root         (0)     7161 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/fuse_conv_redundant_dequantize.py
--rw-r--r--   0 root         (0) root         (0)    42984 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/fuse_conv_requantize.py
--rw-r--r--   0 root         (0) root         (0)     8266 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/fuse_matmul_redundant_dequantize.py
--rw-r--r--   0 root         (0) root         (0)    44668 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/fuse_matmul_requantize.py
--rw-r--r--   0 root         (0) root         (0)     5412 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/meta_op_optimizer.py
--rw-r--r--   0 root         (0) root         (0)     1898 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/post_hostconst_converter.py
--rw-r--r--   0 root         (0) root         (0)     5449 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/post_quantized_op_cse.py
--rw-r--r--   0 root         (0) root         (0)    16032 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/rnn_convert.py
--rw-r--r--   0 root         (0) root         (0)     4789 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/scale_propagation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:05:56.340227 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/qdq/
--rw-r--r--   0 root         (0) root         (0)      669 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/qdq/__init__.py
--rw-r--r--   0 root         (0) root         (0)    38007 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/qdq/insert_qdq_pattern.py
--rw-r--r--   0 root         (0) root         (0)     4322 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/qdq/merge_duplicated_qdq.py
--rw-r--r--   0 root         (0) root         (0)     2555 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/qdq/share_qdq_y_pattern.py
--rw-r--r--   0 root         (0) root         (0)    42640 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:05:56.342227 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/
--rw-r--r--   0 root         (0) root         (0)      666 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:05:56.342227 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/qat/
--rw-r--r--   0 root         (0) root         (0)      670 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/qat/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8567 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/qat/fake_quantize.py
--rw-r--r--   0 root         (0) root         (0)     4623 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/qat/quantize_config.py
--rw-r--r--   0 root         (0) root         (0)     3015 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/qat/quantize_helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:05:56.343227 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/qat/quantize_layers/
--rw-r--r--   0 root         (0) root         (0)      675 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/qat/quantize_layers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1265 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/qat/quantize_layers/optimize_layer.py
--rw-r--r--   0 root         (0) root         (0)     3053 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/qat/quantize_layers/quantize_layer_add.py
--rw-r--r--   0 root         (0) root         (0)     3116 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/qat/quantize_layers/quantize_layer_base.py
--rw-r--r--   0 root         (0) root         (0)     2102 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/qat/quantize_layers/quantize_layer_bn.py
--rw-r--r--   0 root         (0) root         (0)    10193 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/qat/quantize_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:05:56.345227 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/qdq/
--rw-r--r--   0 root         (0) root         (0)      670 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/qdq/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13848 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/qdq/fuse_qdq_bn.py
--rw-r--r--   0 root         (0) root         (0)    12302 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/qdq/fuse_qdq_concatv2.py
--rw-r--r--   0 root         (0) root         (0)   112963 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/qdq/fuse_qdq_conv.py
--rw-r--r--   0 root         (0) root         (0)    27122 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/qdq/fuse_qdq_deconv.py
--rw-r--r--   0 root         (0) root         (0)     8248 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/qdq/fuse_qdq_in.py
--rw-r--r--   0 root         (0) root         (0)    55179 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/qdq/fuse_qdq_matmul.py
--rw-r--r--   0 root         (0) root         (0)     6071 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/qdq/fuse_qdq_pooling.py
--rw-r--r--   0 root         (0) root         (0)     7205 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/qdq/optimize_qdq.py
--rw-r--r--   0 root         (0) root         (0)    36918 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/quantize_graph_base.py
--rw-r--r--   0 root         (0) root         (0)    13576 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/quantize_graph_bn.py
--rw-r--r--   0 root         (0) root         (0)     4651 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/quantize_graph_concatv2.py
--rw-r--r--   0 root         (0) root         (0)    20547 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/quantize_graph_conv.py
--rw-r--r--   0 root         (0) root         (0)     5655 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/quantize_graph_for_intel_cpu.py
--rw-r--r--   0 root         (0) root         (0)    17127 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/quantize_graph_matmul.py
--rw-r--r--   0 root         (0) root         (0)     3206 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/quantize_graph_pooling.py
--rw-r--r--   0 root         (0) root         (0)    19111 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph_common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:05:56.345227 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/transform_graph/
--rw-r--r--   0 root         (0) root         (0)      662 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/transform_graph/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6046 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/transform_graph/bias_correction.py
--rw-r--r--   0 root         (0) root         (0)     3432 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/transform_graph/graph_transform_base.py
--rw-r--r--   0 root         (0) root         (0)     8974 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/transform_graph/insert_logging.py
--rw-r--r--   0 root         (0) root         (0)    14946 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/transform_graph/rerange_quantized_concat.py
--rw-r--r--   0 root         (0) root         (0)    30557 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/utility.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:05:56.346227 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/utils/
--rw-r--r--   0 root         (0) root         (0)     1654 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1392 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/utils/constants.py
--rw-r--r--   0 root         (0) root         (0)    15477 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/utils/data.py
--rw-r--r--   0 root         (0) root         (0)     3708 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/utils/model.py
--rw-r--r--   0 root         (0) root         (0)    60032 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/utils/model_wrappers.py
--rw-r--r--   0 root         (0) root         (0)     5906 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/utils/nets_factory.py
--rw-r--r--   0 root         (0) root         (0)    13962 2024-03-26 08:53:13.000000 neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/utils/utility.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:05:56.347227 neural_compressor_3x_tf-2.5/neural_compressor_3x_tf.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15025 2024-03-26 09:05:56.000000 neural_compressor_3x_tf-2.5/neural_compressor_3x_tf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10728 2024-03-26 09:05:56.000000 neural_compressor_3x_tf-2.5/neural_compressor_3x_tf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-26 09:05:56.000000 neural_compressor_3x_tf-2.5/neural_compressor_3x_tf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2024-03-26 09:05:56.000000 neural_compressor_3x_tf-2.5/neural_compressor_3x_tf.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-03-26 09:05:56.000000 neural_compressor_3x_tf-2.5/neural_compressor_3x_tf.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2418 2024-03-26 08:53:14.000000 neural_compressor_3x_tf-2.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      102 2024-03-26 09:05:56.348227 neural_compressor_3x_tf-2.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     8675 2024-03-26 08:53:14.000000 neural_compressor_3x_tf-2.5/setup.py
--rw-r--r--   0 root         (0) root         (0)    95740 2024-03-26 08:53:14.000000 neural_compressor_3x_tf-2.5/third-party-programs.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:05.429731 neural_compressor_3x_tf-2.5.1/
+-rw-r--r--   0 root         (0) root         (0)    11360 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    15035 2024-04-03 13:34:05.429731 neural_compressor_3x_tf-2.5.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14096 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:05.406731 neural_compressor_3x_tf-2.5.1/neural_compressor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:05.409731 neural_compressor_3x_tf-2.5.1/neural_compressor/common/
+-rw-r--r--   0 root         (0) root         (0)     1059 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23884 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/common/base_config.py
+-rw-r--r--   0 root         (0) root         (0)    12807 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/common/base_tuning.py
+-rw-r--r--   0 root         (0) root         (0)     3298 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/common/tuning_param.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:05.410731 neural_compressor_3x_tf-2.5.1/neural_compressor/common/utils/
+-rw-r--r--   0 root         (0) root         (0)      932 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/common/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1284 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/common/utils/constants.py
+-rw-r--r--   0 root         (0) root         (0)     6009 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/common/utils/logger.py
+-rw-r--r--   0 root         (0) root         (0)     2147 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/common/utils/save_load.py
+-rw-r--r--   0 root         (0) root         (0)     6548 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/common/utils/utility.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:05.410731 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/
+-rw-r--r--   0 root         (0) root         (0)      841 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:05.410731 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/algorithms/
+-rw-r--r--   0 root         (0) root         (0)      756 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/algorithms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:05.410731 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/algorithms/smoother/
+-rw-r--r--   0 root         (0) root         (0)      967 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/algorithms/smoother/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24234 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/algorithms/smoother/calibration.py
+-rw-r--r--   0 root         (0) root         (0)     8107 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/algorithms/smoother/core.py
+-rw-r--r--   0 root         (0) root         (0)    13846 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/algorithms/smoother/scaler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:05.411731 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/algorithms/static_quant/
+-rw-r--r--   0 root         (0) root         (0)      763 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/algorithms/static_quant/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    37538 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/algorithms/static_quant/keras.py
+-rw-r--r--   0 root         (0) root         (0)     5590 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/algorithms/static_quant/keras.yaml
+-rw-r--r--   0 root         (0) root         (0)   111221 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/algorithms/static_quant/tensorflow.py
+-rw-r--r--   0 root         (0) root         (0)    10015 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/algorithms/static_quant/tensorflow.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:05.411731 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/keras/
+-rw-r--r--   0 root         (0) root         (0)      709 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/keras/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:05.412731 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/keras/layers/
+-rw-r--r--   0 root         (0) root         (0)     1219 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/keras/layers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6058 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/keras/layers/conv2d.py
+-rw-r--r--   0 root         (0) root         (0)     4453 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/keras/layers/dense.py
+-rw-r--r--   0 root         (0) root         (0)     7229 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/keras/layers/depthwise_conv2d.py
+-rw-r--r--   0 root         (0) root         (0)     1520 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/keras/layers/layer_initializer.py
+-rw-r--r--   0 root         (0) root         (0)     3517 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/keras/layers/pool2d.py
+-rw-r--r--   0 root         (0) root         (0)     4491 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/keras/layers/quantizer.py
+-rw-r--r--   0 root         (0) root         (0)     7541 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/keras/layers/separable_conv2d.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:05.413731 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/keras/quantization/
+-rw-r--r--   0 root         (0) root         (0)      716 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/keras/quantization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5236 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/keras/quantization/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:05.413731 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/
+-rw-r--r--   0 root         (0) root         (0)     1039 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2300 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/algorithm_entry.py
+-rw-r--r--   0 root         (0) root         (0)     3047 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/autotune.py
+-rw-r--r--   0 root         (0) root         (0)     9219 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/config.py
+-rw-r--r--   0 root         (0) root         (0)     3717 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/quantize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:05.414731 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/
+-rw-r--r--   0 root         (0) root         (0)      584 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44033 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_converter.py
+-rw-r--r--   0 root         (0) root         (0)    16692 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_converter_without_calib.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:05.415731 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/
+-rw-r--r--   0 root         (0) root         (0)      584 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:05.415731 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/bf16/
+-rw-r--r--   0 root         (0) root         (0)      669 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/bf16/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13962 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/bf16/bf16_convert.py
+-rw-r--r--   0 root         (0) root         (0)     3248 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/bf16/dequantize_cast_optimizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:05.420731 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/
+-rw-r--r--   0 root         (0) root         (0)      673 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3279 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/convert_add_to_biasadd.py
+-rw-r--r--   0 root         (0) root         (0)     3897 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/convert_layout.py
+-rw-r--r--   0 root         (0) root         (0)     3183 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/convert_leakyrelu.py
+-rw-r--r--   0 root         (0) root         (0)     1946 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/convert_nan_to_random.py
+-rw-r--r--   0 root         (0) root         (0)     4378 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/convert_placeholder_to_const.py
+-rw-r--r--   0 root         (0) root         (0)     4108 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/dilated_contraction.py
+-rw-r--r--   0 root         (0) root         (0)     5872 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/dummy_biasadd.py
+-rw-r--r--   0 root         (0) root         (0)     3426 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/expanddims_optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     3985 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fetch_weight_from_reshape.py
+-rw-r--r--   0 root         (0) root         (0)    13182 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fold_batch_norm.py
+-rw-r--r--   0 root         (0) root         (0)     7525 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fold_constant.py
+-rw-r--r--   0 root         (0) root         (0)     2920 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fuse_biasadd_add.py
+-rw-r--r--   0 root         (0) root         (0)     3914 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fuse_column_wise_mul.py
+-rw-r--r--   0 root         (0) root         (0)     4971 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fuse_conv_with_math.py
+-rw-r--r--   0 root         (0) root         (0)    16463 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fuse_decomposed_bn.py
+-rw-r--r--   0 root         (0) root         (0)    15598 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fuse_decomposed_in.py
+-rw-r--r--   0 root         (0) root         (0)     9579 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fuse_gelu.py
+-rw-r--r--   0 root         (0) root         (0)     9745 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fuse_layer_norm.py
+-rw-r--r--   0 root         (0) root         (0)     5558 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fuse_pad_with_conv.py
+-rw-r--r--   0 root         (0) root         (0)     5664 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fuse_pad_with_fp32_conv.py
+-rw-r--r--   0 root         (0) root         (0)     5918 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fuse_reshape_transpose.py
+-rw-r--r--   0 root         (0) root         (0)     5954 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/graph_cse_optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     3159 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/grappler_pass.py
+-rw-r--r--   0 root         (0) root         (0)    12823 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/insert_print_node.py
+-rw-r--r--   0 root         (0) root         (0)     6187 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/move_squeeze_after_relu.py
+-rw-r--r--   0 root         (0) root         (0)    13726 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/pre_optimize.py
+-rw-r--r--   0 root         (0) root         (0)     2795 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/remove_training_nodes.py
+-rw-r--r--   0 root         (0) root         (0)     2345 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/rename_batch_norm.py
+-rw-r--r--   0 root         (0) root         (0)     2647 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/split_shared_input.py
+-rw-r--r--   0 root         (0) root         (0)     2135 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/strip_equivalent_nodes.py
+-rw-r--r--   0 root         (0) root         (0)     1564 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/strip_unused_nodes.py
+-rw-r--r--   0 root         (0) root         (0)     3448 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/switch_optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     1224 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/graph_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:05.422731 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/
+-rw-r--r--   0 root         (0) root         (0)      670 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7086 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/freeze_fake_quant.py
+-rw-r--r--   0 root         (0) root         (0)    17685 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/freeze_value.py
+-rw-r--r--   0 root         (0) root         (0)     5533 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/freeze_value_without_calib.py
+-rw-r--r--   0 root         (0) root         (0)     7161 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/fuse_conv_redundant_dequantize.py
+-rw-r--r--   0 root         (0) root         (0)    42984 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/fuse_conv_requantize.py
+-rw-r--r--   0 root         (0) root         (0)     8266 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/fuse_matmul_redundant_dequantize.py
+-rw-r--r--   0 root         (0) root         (0)    44668 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/fuse_matmul_requantize.py
+-rw-r--r--   0 root         (0) root         (0)     5412 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/meta_op_optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     1898 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/post_hostconst_converter.py
+-rw-r--r--   0 root         (0) root         (0)     5449 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/post_quantized_op_cse.py
+-rw-r--r--   0 root         (0) root         (0)    16032 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/rnn_convert.py
+-rw-r--r--   0 root         (0) root         (0)     4789 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/scale_propagation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:05.422731 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/qdq/
+-rw-r--r--   0 root         (0) root         (0)      669 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/qdq/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38007 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/qdq/insert_qdq_pattern.py
+-rw-r--r--   0 root         (0) root         (0)     4322 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/qdq/merge_duplicated_qdq.py
+-rw-r--r--   0 root         (0) root         (0)     2555 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/qdq/share_qdq_y_pattern.py
+-rw-r--r--   0 root         (0) root         (0)    42640 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:05.424731 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/
+-rw-r--r--   0 root         (0) root         (0)      666 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:05.424731 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/qat/
+-rw-r--r--   0 root         (0) root         (0)      670 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/qat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8567 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/qat/fake_quantize.py
+-rw-r--r--   0 root         (0) root         (0)     4623 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/qat/quantize_config.py
+-rw-r--r--   0 root         (0) root         (0)     3015 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/qat/quantize_helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:05.425731 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/qat/quantize_layers/
+-rw-r--r--   0 root         (0) root         (0)      675 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/qat/quantize_layers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1265 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/qat/quantize_layers/optimize_layer.py
+-rw-r--r--   0 root         (0) root         (0)     3053 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/qat/quantize_layers/quantize_layer_add.py
+-rw-r--r--   0 root         (0) root         (0)     3116 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/qat/quantize_layers/quantize_layer_base.py
+-rw-r--r--   0 root         (0) root         (0)     2102 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/qat/quantize_layers/quantize_layer_bn.py
+-rw-r--r--   0 root         (0) root         (0)    10193 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/qat/quantize_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:05.426731 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/qdq/
+-rw-r--r--   0 root         (0) root         (0)      670 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/qdq/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13848 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/qdq/fuse_qdq_bn.py
+-rw-r--r--   0 root         (0) root         (0)    12302 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/qdq/fuse_qdq_concatv2.py
+-rw-r--r--   0 root         (0) root         (0)   112963 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/qdq/fuse_qdq_conv.py
+-rw-r--r--   0 root         (0) root         (0)    27122 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/qdq/fuse_qdq_deconv.py
+-rw-r--r--   0 root         (0) root         (0)     8248 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/qdq/fuse_qdq_in.py
+-rw-r--r--   0 root         (0) root         (0)    55179 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/qdq/fuse_qdq_matmul.py
+-rw-r--r--   0 root         (0) root         (0)     6071 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/qdq/fuse_qdq_pooling.py
+-rw-r--r--   0 root         (0) root         (0)     7205 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/qdq/optimize_qdq.py
+-rw-r--r--   0 root         (0) root         (0)    36918 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/quantize_graph_base.py
+-rw-r--r--   0 root         (0) root         (0)    13576 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/quantize_graph_bn.py
+-rw-r--r--   0 root         (0) root         (0)     4651 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/quantize_graph_concatv2.py
+-rw-r--r--   0 root         (0) root         (0)    20547 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/quantize_graph_conv.py
+-rw-r--r--   0 root         (0) root         (0)     5655 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/quantize_graph_for_intel_cpu.py
+-rw-r--r--   0 root         (0) root         (0)    17127 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/quantize_graph_matmul.py
+-rw-r--r--   0 root         (0) root         (0)     3206 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/quantize_graph_pooling.py
+-rw-r--r--   0 root         (0) root         (0)    19111 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph_common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:05.427731 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/transform_graph/
+-rw-r--r--   0 root         (0) root         (0)      662 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/transform_graph/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6046 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/transform_graph/bias_correction.py
+-rw-r--r--   0 root         (0) root         (0)     3432 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/transform_graph/graph_transform_base.py
+-rw-r--r--   0 root         (0) root         (0)     8974 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/transform_graph/insert_logging.py
+-rw-r--r--   0 root         (0) root         (0)    14946 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/transform_graph/rerange_quantized_concat.py
+-rw-r--r--   0 root         (0) root         (0)    30557 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/utility.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:05.428731 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/utils/
+-rw-r--r--   0 root         (0) root         (0)     1654 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1392 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/utils/constants.py
+-rw-r--r--   0 root         (0) root         (0)    15477 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/utils/data.py
+-rw-r--r--   0 root         (0) root         (0)     3708 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/utils/model.py
+-rw-r--r--   0 root         (0) root         (0)    60032 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/utils/model_wrappers.py
+-rw-r--r--   0 root         (0) root         (0)     5906 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/utils/nets_factory.py
+-rw-r--r--   0 root         (0) root         (0)    13962 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/utils/utility.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:34:05.429731 neural_compressor_3x_tf-2.5.1/neural_compressor_3x_tf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15035 2024-04-03 13:34:05.000000 neural_compressor_3x_tf-2.5.1/neural_compressor_3x_tf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10791 2024-04-03 13:34:05.000000 neural_compressor_3x_tf-2.5.1/neural_compressor_3x_tf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 13:34:05.000000 neural_compressor_3x_tf-2.5.1/neural_compressor_3x_tf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-03 13:34:05.000000 neural_compressor_3x_tf-2.5.1/neural_compressor_3x_tf.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-04-03 13:34:05.000000 neural_compressor_3x_tf-2.5.1/neural_compressor_3x_tf.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2418 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      102 2024-04-03 13:34:05.430731 neural_compressor_3x_tf-2.5.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8675 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/setup.py
+-rw-r--r--   0 root         (0) root         (0)    95740 2024-04-03 13:33:19.000000 neural_compressor_3x_tf-2.5.1/third-party-programs.txt
```

### Comparing `neural_compressor_3x_tf-2.5/LICENSE` & `neural_compressor_3x_tf-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/PKG-INFO` & `neural_compressor_3x_tf-2.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neural_compressor_3x_tf
-Version: 2.5
+Version: 2.5.1
 Summary: Repository of Intel® Neural Compressor
 Home-page: https://github.com/intel/neural-compressor
 Author: Intel AIPT Team
 Author-email: feng.tian@intel.com, haihao.shen@intel.com, suyue.chen@intel.com
 License: Apache 2.0
 Keywords: quantization,auto-tuning,post-training static quantization,post-training dynamic quantization,quantization-aware training
 Classifier: Intended Audience :: Science/Research
@@ -16,15 +16,15 @@
 License-File: LICENSE
 License-File: third-party-programs.txt
 Requires-Dist: prettytable
 Requires-Dist: psutil
 Requires-Dist: py-cpuinfo
 Requires-Dist: pydantic
 Requires-Dist: pyyaml
-Requires-Dist: tensorflow
+Requires-Dist: tensorflow<=2.15.1
 
 <div align="center">
 
 Intel® Neural Compressor
 ===========================
 <h3> An open-source Python library supporting popular model compression techniques on all mainstream deep learning frameworks (TensorFlow, PyTorch, ONNX Runtime, and MXNet)</h3>
```

### Comparing `neural_compressor_3x_tf-2.5/README.md` & `neural_compressor_3x_tf-2.5.1/README.md`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/common/__init__.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/common/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/common/base_config.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/common/base_config.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/common/base_tuning.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/common/base_tuning.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/common/tuning_param.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/common/tuning_param.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/common/utils/__init__.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/common/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/common/utils/constants.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/common/utils/constants.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/common/utils/logger.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/common/utils/logger.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/common/utils/save_load.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/common/utils/save_load.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/__init__.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/algorithms/__init__.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/algorithms/smoother/__init__.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/algorithms/smoother/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/algorithms/smoother/calibration.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/algorithms/smoother/calibration.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/algorithms/smoother/core.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/algorithms/smoother/core.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/algorithms/smoother/scaler.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/algorithms/smoother/scaler.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/algorithms/static_quant/__init__.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/algorithms/static_quant/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/algorithms/static_quant/keras.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/algorithms/static_quant/keras.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #
-# Copyright (c) 2023 Intel Corporation
+# Copyright (c) 2024 Intel Corporation
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #   http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,25 +13,24 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import copy
 import json
-import math
 import os
 from collections import OrderedDict, UserDict
 from typing import Callable, Dict
 
-import keras
 import numpy as np
 import tensorflow as tf
 import yaml
 
 from neural_compressor.common import logger
+from neural_compressor.common.utils import DEFAULT_WORKSPACE
 from neural_compressor.tensorflow.keras.layers import (
     DeQuantize,
     FakeQuant,
     QAvgPool2D,
     QConv2D,
     QDense,
     QDepthwiseConv2D,
@@ -39,151 +38,145 @@
     QSeparableConv2D,
     Quantize,
 )
 from neural_compressor.tensorflow.quantization.config import StaticQuantConfig
 from neural_compressor.tensorflow.utils import deep_get, dump_elapsed_time
 
 
-def _add_supported_quantized_objects(custom_objects):
-    """Map all the quantized objects."""
-    custom_objects["Quantize"] = Quantize
-    custom_objects["DeQuantize"] = DeQuantize
-    custom_objects["FakeQuant"] = FakeQuant
-    custom_objects["QConv2D"] = QConv2D
-    custom_objects["QDepthwiseConv2D"] = QDepthwiseConv2D
-    custom_objects["QSeparableConv2D"] = QSeparableConv2D
-    custom_objects["QDense"] = QDense
-    custom_objects["QMaxPool2D"] = QMaxPool2D
-    custom_objects["QAvgPool2D"] = QAvgPool2D
-    custom_objects["QMaxPooling2D"] = QMaxPool2D
-    custom_objects["QAveragePooling2D"] = QAvgPool2D
-    return custom_objects
-
-
 class KerasAdaptor:
     """The keras class of framework adaptor layer."""
 
+    supported_op = [
+        "Conv2D",
+        "Dense",
+        "SeparableConv2D",
+        "DepthwiseConv2D",
+        "AveragePooling2D",
+        "MaxPooling2D",
+        "AvgPool2D",
+        "MaxPool2D",
+    ]
+
+    custom_layers = {
+        "Quantize": Quantize,
+        "DeQuantize": DeQuantize,
+        "FakeQuant": FakeQuant,
+        "QConv2D": QConv2D,
+        "QDepthwiseConv2D": QDepthwiseConv2D,
+        "QSeparableConv2D": QSeparableConv2D,
+        "QDense": QDense,
+        "QMaxPool2D": QMaxPool2D,
+        "QAvgPool2D": QAvgPool2D,
+        "QMaxPooling2D": QMaxPool2D,
+        "QAveragePooling2D": QAvgPool2D,
+    }
+
     def __init__(self, framework_specific_info):
+        """Initialize the KerasAdaptor class with framework specific information."""
         self.framework_specific_info = framework_specific_info
         self.approach = deep_get(self.framework_specific_info, "approach", False)
         self.quantize_config = {"op_wise_config": {}}
         self.device = self.framework_specific_info["device"]
         self.backend = self.framework_specific_info["backend"]
         self.recipes = deep_get(self.framework_specific_info, "recipes", {})
-        self.supported_op = [
-            "Conv2D",
-            "Dense",
-            "SeparableConv2D",
-            "DepthwiseConv2D",
-            "AveragePooling2D",
-            "MaxPooling2D",
-            "AvgPool2D",
-            "MaxPool2D",
-        ]
 
-        self.pre_optimized_object = None
+        self.pre_optimized_model = None
         self.pre_optimizer_handle = None
         self.bf16_ops = []
         self.fp32_ops = []
         self.query_handler = KerasQuery(local_config_file=os.path.join(os.path.dirname(__file__), "keras.yaml"))
 
         self.fp32_results = []
         self.fp32_preds_as_label = False
         self.callbacks = []
 
         self.conv_format = {}
+        self.fold_conv = []
+        if not os.path.exists(DEFAULT_WORKSPACE):
+            os.mkdir(DEFAULT_WORKSPACE)
+        self.tmp_dir = DEFAULT_WORKSPACE + "tmp_model"
 
     def _check_itex(self):
         """Check if the Intel® Extension for TensorFlow has been installed."""
         try:
             import intel_extension_for_tensorflow
         except:
             raise ImportError(
                 "The Intel® Extension for TensorFlow is not installed. "
                 "Please install it to run models on ITEX backend"
             )
 
-    def tuning_cfg_to_fw(self, tuning_cfg):
-        """Parse tune_config and set framework variables."""
-        self.quantize_config["calib_iteration"] = tuning_cfg["calib_iteration"]
-        self.quantize_config["device"] = self.device
-        self.quantize_config["advance"] = deep_get(tuning_cfg, "advance")
-        fp32_ops = []
-        bf16_ops = []
-        bf16_type = set(self.query_handler.get_op_types_by_precision(precision="bf16"))
-        dispatched_op_names = [j[0] for j in tuning_cfg["op"]]
-        invalid_op_names = [i for i in self.quantize_config["op_wise_config"] if i not in dispatched_op_names]
-
-        for op_name in invalid_op_names:
-            self.quantize_config["op_wise_config"].pop(op_name)
+    def convert_bf16(self):
+        """Execute the BF16 conversion."""
+        tf.keras.mixed_precision.set_global_policy("mixed_bfloat16")
+        model = self.pre_optimized_model
 
-        for each_op_info in tuning_cfg["op"]:
-            op_name = each_op_info[0]
+        for layer in model.layers:
+            if layer.name in self.bf16_ops:
+                layer.dtype = "mixed_bfloat16"
 
-            if tuning_cfg["op"][each_op_info]["activation"]["dtype"] == "bf16":
-                if each_op_info[1] in bf16_type:
-                    bf16_ops.append(op_name)
-                continue
+        model.save(self.tmp_dir)
+        converted_model = tf.keras.models.load_model(self.tmp_dir)
+        tf.keras.mixed_precision.set_global_policy("float32")
 
-            if tuning_cfg["op"][each_op_info]["activation"]["dtype"] == "fp32":
-                if op_name in self.quantize_config["op_wise_config"]:
-                    self.quantize_config["op_wise_config"].pop(op_name)
-                    fp32_ops.append(op_name)
-                continue
+        return converted_model
 
-            is_perchannel = False
-            bit = None
-            if "weight" in tuning_cfg["op"][each_op_info]:
-                is_perchannel = tuning_cfg["op"][each_op_info]["weight"]["granularity"] == "per_channel"
-                # bit = tuning_cfg['op'][each_op_info]['weight']['bit']
-            weight_bit = bit if bit else 7.0
-            algorithm = tuning_cfg["op"][each_op_info]["activation"]["algorithm"]
-            is_asymmetric = False
-            if "activation" in tuning_cfg["op"][each_op_info]:
-                is_asymmetric = tuning_cfg["op"][each_op_info]["activation"]["scheme"] == "asym"
-            self.quantize_config["op_wise_config"][op_name] = (is_perchannel, algorithm, is_asymmetric, weight_bit)
-        self.bf16_ops = bf16_ops
-        if self.bf16_ops:
-            self.bf16_ops.pop(-1)
-        self.fp32_ops = fp32_ops
+    # (TODO) choose the properly quantize mode
+    def _check_quantize_mode(self, model):
+        """Check what quantize mode to use."""
+        for layer in model.layers:
+            if "ReLU" in layer.__class__.__name__:
+                return "MIN_FIRST"
+        return "SCALED"
 
-    def _pre_optimize(self, model):
-        """Apply pre-optimization."""
-        model = self._check_quantize_format(model)
-        model = self._fuse_bn(model)
-        return model
+    def _set_weights(self, qmodel, layer_weights):
+        """Set fp32 weights to qmodel."""
+        for qlayer in qmodel.layers:
+            if qlayer.get_weights():
+                if qlayer.name in layer_weights:
+                    qlayer.set_weights(layer_weights[qlayer.name])
+                else:
+                    hit_layer = False
+                    for sub_layer in qlayer.submodules:
+                        if sub_layer.name in layer_weights:
+                            qlayer.set_weights(layer_weights[sub_layer.name])
+                            hit_layer = True
+                            break
+                    if not hit_layer:
+                        raise ValueError("Can not match the module weights....")
+        return qmodel
 
     def _check_quantize_format(self, model):
         """The function that checks format for conv ops."""
-        json_model = copy.deepcopy(json.loads(model.to_json()))
-        config = json_model["config"]
-        fp32_layers = config["layers"]
-        name_op_map = {}
-
-        for idx, layer in enumerate(copy.deepcopy(fp32_layers)):
-            name_op_map[layer["config"]["name"]] = layer
-
-        for idx, layer in enumerate(copy.deepcopy(fp32_layers)):
-            layer_config = layer["config"]
-            if layer["class_name"] in self.supported_op:
-                if "inbound_nodes" in layer:
-                    check_layer = name_op_map[layer["inbound_nodes"][0][0][0]]
-                else:
-                    check_layer = fp32_layers[idx - 1]
-                if check_layer["class_name"] in ["Activation"] and check_layer["config"]["activation"] in ["relu"]:
-                    self.conv_format[layer["config"]["name"]] = "u8"
+        input_layer_dict = {}
+        layer_name_mapping = {}
+
+        for layer in model.layers:
+            layer_name_mapping[layer.name] = layer
+            for node in layer._outbound_nodes:
+                layer_name = node.outbound_layer.name
+                if layer_name not in input_layer_dict:
+                    input_layer_dict[layer_name] = [layer.name]
                 else:
-                    self.conv_format[layer["config"]["name"]] = "s8"
-        return model
+                    input_layer_dict[layer_name].append(layer.name)
+
+        for layer in model.layers:
+            if layer.__class__.__name__ in self.supported_op:
+                self.conv_format[layer.name] = "s8"
+                input_layer_names = input_layer_dict[layer.name]
+                for input_layer_name in input_layer_names:
+                    check_layer = layer_name_mapping[input_layer_name]
+                    if check_layer.__class__.__name__ == "Activation" and check_layer.activation.__name__ in ["relu"]:
+                        self.conv_format[layer.name] = "u8"
+                        break
 
     def _fuse_bn(self, model):
         """Fusing Batch Normalization."""
-        json_model = copy.deepcopy(json.loads(model.to_json()))
-        config = json_model["config"]
-        fp32_layers = config["layers"]
+        fuse_bn_model = copy.deepcopy(model)
+        fp32_layers = fuse_bn_model.layers
 
         def fuse_conv_bn(conv_weight, bn_weight, conv_type="Conv2D", eps=1.0e-5):
             assert conv_type in [
                 "Conv2D",
                 "DepthwiseConv2D",
                 "SeparableConv2D",
             ], "only support Conv2D, DepthwiseConv2D, SeparableConv2D..."
@@ -221,85 +214,90 @@
                 bias = conv_weight[2]
             scale_value = gamma / np.sqrt(var + eps)
             weight = weight * scale_value
             bias = beta + (bias - mean) * scale_value.reshape(-1)
             bias = bias.reshape(-1)
             return [depth_weight, weight, bias] if conv_type == "SeparableConv2D" else [weight, bias]
 
-        node_map = {}
-        for idx, layer in enumerate(copy.deepcopy(fp32_layers)):
-            layer_config = layer["config"]
-            if "inbound_nodes" in layer:
-                node_map[layer["name"]] = layer
-
         fuse_layers = []
-        fold_conv = []
-        for idx, layer in enumerate(copy.deepcopy(fp32_layers)):
-            layer_config = layer["config"]
-            if "inbound_nodes" in layer:
-                if layer["class_name"] in ["BatchNormalization"]:
-                    bn_inbound_node = node_map[layer_config["name"]]["inbound_nodes"][0][0]
-                    if bn_inbound_node[0] in self.conv_weights.keys():
-                        conv_weight = self.conv_weights[bn_inbound_node[0]]
-                        conv_layer = node_map[bn_inbound_node[0]]
-                        bn_weight = self.bn_weights[layer_config["name"]]
-                        self.layer_weights[bn_inbound_node[0]] = fuse_conv_bn(
-                            conv_weight, bn_weight, conv_layer["class_name"], layer["config"]["epsilon"]
-                        )
-                        fold_conv.append(bn_inbound_node[0])
-                    else:
-                        fuse_layers.append(layer)
-                elif len(layer["inbound_nodes"]):
+        for idx, layer in enumerate(fp32_layers):
+            if hasattr(layer, "_inbound_nodes"):
+                if layer.__class__.__name__ in ("BatchNormalization"):
+                    for bn_inbound_node in layer._inbound_nodes:
+                        inbound_layer = bn_inbound_node.inbound_layers
+                        if inbound_layer.name in self.conv_weights.keys():
+                            conv_layer = inbound_layer
+                            conv_weight = self.conv_weights[conv_layer.name]
+                            bn_weight = self.bn_weights[layer.name]
+
+                            self.layer_weights[conv_layer.name] = fuse_conv_bn(
+                                conv_weight, bn_weight, conv_layer.__class__.__name__, layer.epsilon
+                            )
+                            self.fold_conv.append(conv_layer.name)
+                        else:
+                            fuse_layers.append(layer)
+                elif len(layer._inbound_nodes):
                     new_bound_nodes = []
                     # OpLambda node will have different bound node
-                    if layer["class_name"] in ["TFOpLambda", "SlicingOpLambda"]:
+                    if layer.__class__.__name__ in ("TFOpLambda", "SlicingOpLambda"):
                         fuse_layers.append(layer)
                     else:
-                        for bound_node in layer["inbound_nodes"][0]:
-                            if bound_node[0] in self.bn_weights.keys():
-                                bn_inbound_node = node_map[bound_node[0]]["inbound_nodes"][0][0]
-                                if bn_inbound_node[0] in self.conv_weights.keys():
-                                    new_bound_nodes.append(bn_inbound_node)
-                                else:
-                                    new_bound_nodes.append(bound_node)
+                        for bound_node in layer._inbound_nodes:
+                            inbound_layer = bound_node.inbound_layers
+                            if (
+                                not isinstance(inbound_layer, list)
+                                and inbound_layer.name in self.bn_weights.keys()
+                                and inbound_layer._inbound_nodes[0].inbound_layers.name in self.conv_weights.keys()
+                            ):
+                                new_bound_nodes.append(bn_inbound_node)
                             else:
                                 new_bound_nodes.append(bound_node)
-                        layer["inbound_nodes"] = [new_bound_nodes]
+
+                        layer._inbound_nodes.clear()
+                        for bound_node in new_bound_nodes:
+                            layer._inbound_nodes.append(bound_node)
                         fuse_layers.append(layer)
                 else:
                     fuse_layers.append(layer)
             else:
                 if (
                     idx > 0
-                    and layer["class_name"] in ["BatchNormalization"]
-                    and fp32_layers[idx - 1]["class_name"] in ["Conv2D"]
+                    and layer.__class__.__name__ == "BatchNormalization"
+                    and fp32_layers[idx - 1].__class__.__name__ == "Conv2D"
                 ):
-                    conv_name = fp32_layers[idx - 1]["config"]["name"]
+                    conv_name = fp32_layers[idx - 1].name
                     conv_weight = self.conv_weights[conv_name]
-                    bn_weight = self.bn_weights[layer_config["name"]]
-                    conv_type = fp32_layers[idx - 1]["class_name"]
-                    self.layer_weights[conv_name] = fuse_conv_bn(
-                        conv_weight, bn_weight, conv_type, layer["config"]["epsilon"]
-                    )
-                    fold_conv.append(conv_name)
+                    bn_weight = self.bn_weights[layer.name]
+                    conv_type = fp32_layers[idx - 1].__class__.__name__
+
+                    self.layer_weights[conv_name] = fuse_conv_bn(conv_weight, bn_weight, conv_type, layer.epsilon)
+                    self.fold_conv.append(conv_name)
                 else:
                     fuse_layers.append(layer)
 
-        # bn folding will have a shift bias
         for idx, layer in enumerate(fuse_layers):
-            layer_config = layer["config"]
             if (
-                layer["class_name"] in ["Conv2D", "DepthwiseConv2D", "SeparableConv2D"]
-                and layer_config["name"] in fold_conv
+                layer.__class__.__name__ in ("Conv2D", "DepthwiseConv2D", "SeparableConv2D")
+                and layer.name in self.fold_conv
             ):
-                layer_config["use_bias"] = True
+                conv_config = layer.get_config()
+                conv_config["use_bias"] = True
+                conv_layer = type(layer).from_config(conv_config)
+                for node in layer._outbound_nodes:
+                    conv_layer._outbound_nodes.append(node)
+                fuse_layers[idx] = conv_layer
+
+        bn_surgery = KerasSurgery(model)
+        bn_fused_model = bn_surgery.fuse_bn_layers(fuse_layers, self.conv_weights.keys())
+        bn_fused_model = self._set_weights(bn_fused_model, self.layer_weights)
+
+        bn_fused_model.save(self.tmp_dir)
+        bn_fused_model = tf.keras.models.load_model(self.tmp_dir)
 
-        json_model["config"]["layers"] = fuse_layers
-        fused_model = self._restore_model_from_json(json_model)
-        return fused_model
+        return bn_fused_model
 
     @dump_elapsed_time("Pass quantize model")
     def quantize(self, quant_config, model, dataloader, iteration, q_func=None):
         """Execute the quantize process on the specified model.
 
         Args:
             tune_cfg(dict): The user defined 'StaticQuantConfig' class.
@@ -314,224 +312,144 @@
         self.tuning_cfg_to_fw(tune_cfg)
 
         # just convert the input model to mixed_bfloat16
         if self.bf16_ops and not self.quantize_config["op_wise_config"]:
             converted_model = self.convert_bf16()
             return converted_model
 
-        # if self.backend == "itex":
-        #     self._check_itex()
+        if self.backend == "itex":
+            self._check_itex()
+
         logger.debug("Dump quantization configurations:")
         logger.debug(self.quantize_config)
         calib_sampling_size = tune_cfg.get("calib_sampling_size", 1)
 
         if hasattr(dataloader, "batch_size") and calib_sampling_size % dataloader.batch_size != 0:
             iter = self.quantize_config["calib_iteration"]
             logger.warning(
                 "Please note that calibration sampling size {} "
                 "isn't divisible exactly by batch size {}. "
                 "So the real sampling size is {}.".format(
                     calib_sampling_size, dataloader.batch_size, dataloader.batch_size * iter
                 )
             )
 
-        q_layers = []
-        self.inbound_nodes_map = {}
-        for idx, layer in enumerate(copy.deepcopy(self.fp32_layers)):
-            layer_config = layer["config"]
-            if (
-                layer["class_name"] in self.supported_op
-                and layer["config"]["name"] in self.quantize_config["op_wise_config"]
-            ):
-                op_config = self.quantize_config["op_wise_config"][layer["config"]["name"]]
+        fq_layers_dict = {}
+        fq_output_layers = {}
+        for idx, layer in enumerate(self.pre_optimized_model.layers):
+            if layer.__class__.__name__ in self.supported_op and layer.name in self.quantize_config["op_wise_config"]:
+                op_config = self.quantize_config["op_wise_config"][layer.name]
                 mode = "per_channel" if op_config[0] else "per_tensor"
                 fake_q_name = "fake_quant_" + str(idx)
-                fake_q_layer = {
-                    "class_name": "FakeQuant",
-                    "name": fake_q_name,
-                    "T": self.conv_format[layer["config"]["name"]],
-                    "config": {"mode": "per_tensor", "name": fake_q_name},
-                }
-                if "inbound_nodes" in layer:
-                    fake_q_layer["inbound_nodes"] = layer["inbound_nodes"]
-                    layer["inbound_nodes"] = [[[fake_q_name, 0, 0, {}]]]
-                    self.inbound_nodes_map[fake_q_name] = layer
-
-                q_layers.append(fake_q_layer)
-                q_layers.append(layer)
-            else:
-                q_layers.append(layer)
-
-        json_model = copy.deepcopy(json.loads(self.pre_optimized_object.to_json()))
-        json_model["config"]["layers"] = q_layers
-        quantized_model = self._restore_model_from_json(json_model)
+                fake_q_layer = FakeQuant(name=fake_q_name, T=self.conv_format[layer.name], mode="per_tensor")
+                fq_layers_dict[layer.name] = [fake_q_layer]
+                fq_output_layers[fake_q_layer.name] = layer.name
+        self.pre_optimized_model.save(self.tmp_dir)
+
+        fq_surgery = KerasSurgery(self.pre_optimized_model)
+        calibration_model = fq_surgery.insert_quant_layers(fq_layers_dict)
+        calibration_model = self._set_weights(calibration_model, self.layer_weights)
+
+        quantized_model = self._calibrate(
+            calibration_model,
+            dataloader,
+            self.quantize_config["calib_iteration"],
+            fq_output_layers,
+        )
 
-        converted_model = self._calibrate(quantized_model, dataloader, self.quantize_config["calib_iteration"])
+        return quantized_model
 
-        return converted_model
+    def _calibrate(self, model, dataloader, calib_interation, fq_output_layers):
+        """Apply calibration.
 
-    def _calibrate(self, model, dataloader, calib_interation):
-        """Apply calibration."""
+        Args:
+            model (tf.keras.Model): The model inserted with FakeQuant layers for calibration.
+            dataloader(object): The calibration dataloader used to load quantization dataset.
+            iteration(int): The iteration of calibration.
+            fq_output_layers (dict): A dict mapping from names of FakeQuant layers to
+                names of their output layers.
+        """
         # run eagerly to fetch the numpy min/max
-        model.compile(run_eagerly=True)
         results = {}
+        model.compile(run_eagerly=True)
         for idx, (inputs, labels) in enumerate(dataloader):
-            outputs = model.predict_on_batch(inputs)
+            _ = model.predict_on_batch(inputs)
             json_model = copy.deepcopy(json.loads(model.to_json()))
             config = json_model["config"]
             layers = config["layers"]
             for layer in layers:
                 if layer["class_name"] == "FakeQuant":
                     min_value = layer["config"]["min_value"]
                     max_value = layer["config"]["max_value"]
+                    assert min_value < max_value, "The min value must be lower than the max value in quantization."
+
                     if layer["config"]["name"] not in results:
                         results[layer["config"]["name"]] = {"min": [min_value], "max": [max_value]}
                     else:
                         results[layer["config"]["name"]]["min"].append(min_value)
                         results[layer["config"]["name"]]["max"].append(max_value)
             if idx + 1 == calib_interation:
                 break
 
-        # insert the calibrated min/max to Q/DQ
-        json_model = copy.deepcopy(json.loads(model.to_json()))
-        config = json_model["config"]
-        layers = config["layers"]
-        q_layers = []
-        # quantize_mode = self._check_quantize_mode(json_model)
-        inbound_reverse_map = {}
-        for idx, layer in enumerate(layers):
-            layer_config = copy.deepcopy(layer["config"])
-            if layer["class_name"] == "FakeQuant":
-                min_value = min(results[layer["config"]["name"]]["min"])
-                max_value = max(results[layer["config"]["name"]]["max"])
-                quantize_layer = {
-                    "class_name": "Quantize",
-                    "name": "quantize_" + str(idx),
-                    "config": {
-                        "min_range": min_value,
-                        "max_range": max_value,
-                        "T": layer_config["T"],
-                        "name": "quantize_" + str(idx),
-                    },
-                }
-                dequantize_layer = {
-                    "class_name": "DeQuantize",
-                    "name": "dequantize_" + str(idx),
-                    "config": {
-                        "min_range": min_value,
-                        "max_range": max_value,
-                        # 'mode': quantize_mode,
-                        "name": "dequantize_" + str(idx),
-                    },
-                }
-                if "inbound_nodes" in layer:
-                    quantize_layer["inbound_nodes"] = layer["inbound_nodes"]
-                    dequantize_layer["inbound_nodes"] = [[["quantize_" + str(idx), 0, 0, {}]]]
-                    # find the conv/dense layer from fake quant map and
-                    # change the conv/dense node inbound to dequantize
-                    layer_name = self.inbound_nodes_map[layer["name"]]["name"]
-                    inbound_reverse_map[layer_name] = [[["dequantize_" + str(idx), 0, 0, {}]]]
-
-                q_layers.append(quantize_layer)
-                q_layers.append(dequantize_layer)
-            elif (
-                layer["class_name"] in self.supported_op
-                and layer["config"]["name"] in self.quantize_config["op_wise_config"]
-            ):
+        qdq_layer_nums = 0
+        qdq_layers_dict = {}
+        quantized_layers_dict = {}
+        for idx, layer in enumerate(model.layers):
+            if layer.__class__.__name__ == "FakeQuant":
+                min_value = min(results[layer.name]["min"])
+                max_value = max(results[layer.name]["max"])
+
+                quantize_layer = Quantize(
+                    name="quantize_" + str(qdq_layer_nums),
+                    min_range=min_value,
+                    max_range=max_value,
+                    T=layer.T,
+                )
+                dequantize_layer = DeQuantize(
+                    name="dequantize_" + str(qdq_layer_nums),
+                    min_range=min_value,
+                    max_range=max_value,
+                )
+
+                qdq_layer_nums += 1
+                output_layer_name = fq_output_layers[layer.name]
+                qdq_layers_dict[output_layer_name] = [quantize_layer, dequantize_layer]
+            elif layer.__class__.__name__ in self.supported_op and layer.name in self.quantize_config["op_wise_config"]:
                 # index 0 is weight, index 1 is bias
-                q_layer_name = "Q" + layer["class_name"]
-                # this is for inbounds search
-                q_name = layer["config"]["name"]
+                q_layer_class = "Q" + layer.__class__.__name__
                 # for layers that have weights
-                if layer["config"]["name"] in self.layer_weights:
-                    kernel = self.layer_weights[layer["config"]["name"]][0]
+                if layer.name in self.layer_weights:
+                    kernel = self.layer_weights[layer.name][0]
                     dim = list(range(0, kernel.ndim))
                     t_dim = [dim.pop(-1)]
                     t_dim.extend(dim)
                     channel_size = kernel.shape[-1]
                     kernel_channel = kernel.transpose(t_dim).reshape(channel_size, -1)
-                    layer_config["min_value"] = json.dumps(np.min(kernel_channel, axis=1).tolist())
-                    layer_config["max_value"] = json.dumps(np.max(kernel_channel, axis=1).tolist())
+
+                    layer.min_value = np.min(kernel_channel, axis=1).tolist()
+                    layer.max_value = np.max(kernel_channel, axis=1).tolist()
                 else:
                     # default value, but never expected to be used
                     # cause no kernel weights for this layer
-                    layer_config["min_value"] = json.dumps([-10000])
-                    layer_config["max_value"] = json.dumps([10000])
-                layer_config["name"] = q_name
-                q_layer = {"class_name": q_layer_name, "name": q_name, "config": layer_config}
-                if "inbound_nodes" in layer:
-                    q_layer["inbound_nodes"] = inbound_reverse_map[layer["name"]]
-                q_layers.append(q_layer)
-            else:
-                q_layers.append(layer)
+                    layer.min_value = [-10000]
+                    layer.max_value = [10000]
 
-        json_model["config"]["layers"] = q_layers
-        quantized_model = self._restore_model_from_json(json_model)
-        return quantized_model
+                from neural_compressor.tensorflow.keras.layers import layer_initializer_dict
 
-    def convert_bf16(self):
-        """Execute the BF16 conversion."""
-        tf.keras.mixed_precision.set_global_policy("mixed_bfloat16")
-        json_model = copy.deepcopy(json.loads(self.pre_optimized_object.to_json()))
+                q_layer = layer_initializer_dict[q_layer_class](layer)
+                quantized_layers_dict[layer.name] = q_layer
 
-        for layer in json_model["config"]["layers"]:
-            if layer["config"]["name"] in self.bf16_ops:
-                layer["config"]["dtype"] = "mixed_bfloat16"
+        qdq_surgery = KerasSurgery(self.pre_optimized_model)
+        quantized_model = qdq_surgery.insert_quant_layers(qdq_layers_dict, quantized_layers_dict)
+        quantized_model = self._set_weights(quantized_model, self.layer_weights)
 
-        converted_model = self._restore_model_from_json(json_model)
-        tf.keras.mixed_precision.set_global_policy("float32")
+        quantized_model.save(self.tmp_dir)
+        quantized_model = tf.keras.models.load_model(self.tmp_dir)
 
-        return converted_model
-
-    # (TODO) choose the properly quantize mode
-    def _check_quantize_mode(self, json_model):
-        """Check what quantize mode to use."""
-        config = json_model["config"]
-        layers = config["layers"]
-        for idx, layer in enumerate(layers):
-            if "ReLU" in layer["class_name"]:
-                return "MIN_FIRST"
-        return "SCALED"
-
-    def _restore_model_from_json(self, json_model):
-        """Generate a keras model from json files."""
-        from tensorflow.keras.models import model_from_json
-
-        from neural_compressor.tensorflow.utils import version1_gte_version2
-
-        if version1_gte_version2(keras.__version__, "2.13.1"):
-            from keras.src.saving import serialization_lib
-
-            serialization_lib.enable_unsafe_deserialization()
-
-        custom_objects = {}
-        # We need to keep a dictionary of custom objects as our quantized library
-        # is not recognized by keras.
-        custom_objects = _add_supported_quantized_objects(custom_objects)
-        json_model_file = json.dumps(json_model)
-        qmodel = model_from_json(json_model_file, custom_objects=custom_objects)
-        qmodel = self._set_weights(qmodel, self.layer_weights)
-        return qmodel
-
-    # set fp32 weights to qmodel
-    def _set_weights(self, qmodel, layer_weights):
-        for qlayer in qmodel.layers:
-            if qlayer.get_weights():
-                if qlayer.name in layer_weights:
-                    qlayer.set_weights(layer_weights[qlayer.name])
-                else:
-                    hit_layer = False
-                    for sub_layer in qlayer.submodules:
-                        if sub_layer.name in layer_weights:
-                            qlayer.set_weights(layer_weights[sub_layer.name])
-                            hit_layer = True
-                            break
-                    if not hit_layer:
-                        raise ValueError("Can not match the module weights....")
-        return qmodel
+        return quantized_model
 
     @dump_elapsed_time(customized_msg="Model inference")
     def evaluate(
         self,
         model,
         dataloader,
         postprocess=None,
@@ -601,53 +519,50 @@
         conv_config = copy.deepcopy(op_capability["int8"]["DepthwiseConv2D"])
         dense_config = copy.deepcopy(op_capability["int8"]["Dense"])
         maxpool_config = copy.deepcopy(op_capability["int8"]["MaxPooling2D"])
         avgpool_config = copy.deepcopy(op_capability["int8"]["AveragePooling2D"])
         other_config = copy.deepcopy(op_capability["int8"]["default"])
 
         # # get fp32 layer weights
-        keras_object = model
+        self.fp32_model = model
         self.conv_weights = {}
         self.bn_weights = {}
         self.layer_weights = {}
-        for layer in keras_object.layers:
+        for layer in self.fp32_model.layers:
             if layer.get_weights():
                 if (
                     isinstance(layer, tf.keras.layers.Conv2D)
                     or isinstance(layer, tf.keras.layers.DepthwiseConv2D)
                     or isinstance(layer, tf.keras.layers.SeparableConv2D)
                 ):
                     self.conv_weights[layer.name] = copy.deepcopy(layer.get_weights())
                 elif isinstance(layer, tf.keras.layers.BatchNormalization):
                     self.bn_weights[layer.name] = copy.deepcopy(layer.get_weights())
                 self.layer_weights[layer.name] = copy.deepcopy(layer.get_weights())
-        self.pre_optimized_object = self._pre_optimize(keras_object)
 
-        json_model = copy.deepcopy(json.loads(self.pre_optimized_object.to_json()))
-        config = json_model["config"]
-        self.fp32_layers = config["layers"]
-
-        quantizable_op_details = OrderedDict()
-        for details in self.fp32_layers:
-            node_op = details["class_name"]
-            node_name = details["config"]["name"]
-            if node_op == "Conv2D":
-                quantizable_op_details[(node_name, node_op)] = [conv_config, bf16_config, fp32_config]
-            elif node_op == "Dense":
-                quantizable_op_details[(node_name, node_op)] = [dense_config, bf16_config, fp32_config]
-            elif node_op in {"AveragePooling2D", "AvgPool2D"}:
-                quantizable_op_details[(node_name, node_op)] = [avgpool_config, bf16_config, fp32_config]
-            elif node_op in {"MaxPooling2D", "MaxPool2D"}:
-                quantizable_op_details[(node_name, node_op)] = [maxpool_config, bf16_config, fp32_config]
+        self._check_quantize_format(self.fp32_model)
+        self.pre_optimized_model = self._fuse_bn(self.fp32_model)
+
+        quantizable_layer_details = OrderedDict()
+        for layer in self.fp32_model.layers:
+            layer_class = layer.__class__.__name__
+            if layer_class == "Conv2D":
+                quantizable_layer_details[(layer.name, layer_class)] = [conv_config, bf16_config, fp32_config]
+            elif layer_class == "Dense":
+                quantizable_layer_details[(layer.name, layer_class)] = [dense_config, bf16_config, fp32_config]
+            elif layer_class in {"AveragePooling2D", "AvgPool2D"}:
+                quantizable_layer_details[(layer.name, layer_class)] = [avgpool_config, bf16_config, fp32_config]
+            elif layer_class in {"MaxPooling2D", "MaxPool2D"}:
+                quantizable_layer_details[(layer.name, layer_class)] = [maxpool_config, bf16_config, fp32_config]
             else:
-                quantizable_op_details[(node_name, node_op)] = [bf16_config, fp32_config]
+                quantizable_layer_details[(layer.name, layer_class)] = [bf16_config, fp32_config]
 
         capability = {
-            "opwise": copy.deepcopy(quantizable_op_details),
-            "optypewise": self.get_optype_wise_ability(quantizable_op_details),
+            "opwise": copy.deepcopy(quantizable_layer_details),
+            "optypewise": self.get_optype_wise_ability(quantizable_layer_details),
         }
         logger.debug("Dump framework quantization capability:")
         logger.debug(capability)
 
         return capability
 
     def get_optype_wise_ability(self, quantizable_op_details):
@@ -661,14 +576,62 @@
         for op in quantizable_op_details:
             if op[1] not in res:
                 res[op[1]] = {"activation": quantizable_op_details[op][0]["activation"]}
                 if "weight" in quantizable_op_details[op][0]:
                     res[op[1]]["weight"] = quantizable_op_details[op][0]["weight"]
         return res
 
+    def tuning_cfg_to_fw(self, tuning_cfg):
+        """Parse tune_config and set framework variables.
+
+        Args:
+            tuning_cfg (dict): The dict of tuning config.
+        """
+        self.quantize_config["calib_iteration"] = tuning_cfg["calib_iteration"]
+        self.quantize_config["device"] = self.device
+        self.quantize_config["advance"] = deep_get(tuning_cfg, "advance")
+        fp32_ops = []
+        bf16_ops = []
+        bf16_type = set(self.query_handler.get_op_types_by_precision(precision="bf16"))
+        dispatched_op_names = [j[0] for j in tuning_cfg["op"]]
+        invalid_op_names = [i for i in self.quantize_config["op_wise_config"] if i not in dispatched_op_names]
+
+        for op_name in invalid_op_names:
+            self.quantize_config["op_wise_config"].pop(op_name)
+
+        for each_op_info in tuning_cfg["op"]:
+            op_name = each_op_info[0]
+
+            if tuning_cfg["op"][each_op_info]["activation"]["dtype"] == "bf16":
+                if each_op_info[1] in bf16_type:
+                    bf16_ops.append(op_name)
+                continue
+
+            if tuning_cfg["op"][each_op_info]["activation"]["dtype"] == "fp32":
+                if op_name in self.quantize_config["op_wise_config"]:
+                    self.quantize_config["op_wise_config"].pop(op_name)
+                    fp32_ops.append(op_name)
+                continue
+
+            is_perchannel = False
+            bit = None
+            if "weight" in tuning_cfg["op"][each_op_info]:
+                is_perchannel = tuning_cfg["op"][each_op_info]["weight"]["granularity"] == "per_channel"
+                # bit = tuning_cfg['op'][each_op_info]['weight']['bit']
+            weight_bit = bit if bit else 7.0
+            algorithm = tuning_cfg["op"][each_op_info]["activation"]["algorithm"]
+            is_asymmetric = False
+            if "activation" in tuning_cfg["op"][each_op_info]:
+                is_asymmetric = tuning_cfg["op"][each_op_info]["activation"]["scheme"] == "asym"
+            self.quantize_config["op_wise_config"][op_name] = (is_perchannel, algorithm, is_asymmetric, weight_bit)
+        self.bf16_ops = bf16_ops
+        if self.bf16_ops:
+            self.bf16_ops.pop(-1)
+        self.fp32_ops = fp32_ops
+
 
 class KerasQuery:
     """Class that queries configs from yaml settings."""
 
     def __init__(self, local_config_file=None):
         """Initialize KerasQuery."""
         self.version = tf.version.VERSION
@@ -756,15 +719,15 @@
         assert precision in list(self.cur_config["ops"].keys())
         return self.cur_config["ops"][precision]
 
 
 class KerasConfigConverter:
     """Convert `StaticQuantConfig` to the format used by static quant algo."""
 
-    support_int8_weight = {"Dense", "Conv2d", "DepthwiseConv2D", "SeparableConv2D"}
+    support_int8_weight = {"Dense", "Conv2D", "DepthwiseConv2D", "SeparableConv2D"}
 
     def __init__(self, quant_config: StaticQuantConfig, calib_iteration: int):
         """Init parser for keras static quant config.
 
         Args:
             quant_config: the keras static quant config.
             calib_iteration: the iteration of calibration.
@@ -805,7 +768,123 @@
         tune_cfg = {"op": OrderedDict()}
         for op_key, config in self.quant_config.items():
             op_value = self.update_config(config, op_key)
             tune_cfg["op"].update({op_key: op_value})
             tune_cfg["calib_iteration"] = self.calib_iteration
 
         return tune_cfg
+
+
+class KerasSurgery:
+    """The class that inserts FakeQuant or QDQ layers before the target layers."""
+
+    def __init__(self, model):
+        """Init the KerasSurgery class.
+
+        Args:
+            model: the model to be modified.
+        """
+        self.model_outputs = []
+        self.model = copy.deepcopy(model)
+
+    def _create_input_dict(self, fuse_layers=None, conv_weights_keys=None):
+        """Create a input_layer_dict from model.
+
+        Args:
+            fuse_layers: The layers in which fused BNs have been excluded, default to be None.
+            conv_weights_keys: The names of conv layers where BNs are going to be fused, default to be None.
+
+        Returns:
+            input_layer_dict: The dict that mapping for layer names to their input layer names.
+        """
+        input_layer_dict = {}
+        layers = fuse_layers if fuse_layers else self.model.layers
+        for layer in layers:
+            for node in layer._outbound_nodes:
+                out_layer = node.outbound_layer
+                out_layer_names = [out_layer.name]
+                if (
+                    conv_weights_keys
+                    and out_layer.__class__.__name__ in ("BatchNormalization")
+                    and layer.name in conv_weights_keys
+                ):
+                    out_layer_names = [node.outbound_layer.name for node in out_layer._outbound_nodes]
+
+                for out_layer_name in out_layer_names:
+                    if out_layer_name not in input_layer_dict:
+                        input_layer_dict[out_layer_name] = [layer.name]
+                    else:
+                        input_layer_dict[out_layer_name].append(layer.name)
+
+        return input_layer_dict
+
+    def fuse_bn_layers(self, fuse_layers, conv_weights_keys):
+        """Fuse BN layers and rebuild the model.
+
+        Args:
+            fuse_layers: The layers in which fused BNs have been excluded.
+            conv_weights_keys: The names of conv layers where BNs are going to be fused.
+        """
+        self.input_layer_dict = self._create_input_dict(fuse_layers, conv_weights_keys)
+        output_tensor_dict = {"keras.Input": self.model.input}
+
+        for idx, layer in enumerate(fuse_layers):
+            if layer.__class__.__name__ == "InputLayer":
+                output_tensor_dict[layer.name] = output_tensor_dict["keras.Input"]
+                continue
+
+            input_tensors = (
+                output_tensor_dict["keras.Input"]
+                if idx == 0
+                else [output_tensor_dict[input_layer] for input_layer in self.input_layer_dict[layer.name]]
+            )
+
+            while isinstance(input_tensors, list) and len(input_tensors) == 1:
+                input_tensors = input_tensors[0]
+
+            x = layer(input_tensors)
+
+            output_tensor_dict[layer.name] = x
+            if layer.name in self.model.output_names:
+                self.model_outputs.append(x)
+
+        return tf.keras.models.Model(inputs=self.model.inputs, outputs=self.model_outputs)
+
+    def insert_quant_layers(self, qdq_layer_dict, q_layer_dict=None):
+        """Insert FakeQuant or QDQ layers before the target layers and replace
+           Keras layers to Quantized layers.
+
+        Args:
+            qdq_layer_dict: The dict mapping from layers to be quantized to the FakeQuant layer or QDQ layers
+            that are going to be inserted before them.
+            q_layer_dict: The dict mapping from layers to be replacement to the quantized layers.
+        """
+        self.input_layer_dict = self._create_input_dict()
+        output_tensor_dict = {"keras.Input": self.model.input}
+
+        for idx, layer in enumerate(self.model.layers):
+            if layer.__class__.__name__ == "InputLayer":
+                output_tensor_dict[layer.name] = output_tensor_dict["keras.Input"]
+                continue
+
+            input_tensors = (
+                output_tensor_dict["keras.Input"]
+                if idx == 0
+                else [output_tensor_dict[input_layer] for input_layer in self.input_layer_dict[layer.name]]
+            )
+            while isinstance(input_tensors, list) and len(input_tensors) == 1:
+                input_tensors = input_tensors[0]
+
+            if layer.name in qdq_layer_dict:
+                x = input_tensors
+                for inserted_layer in qdq_layer_dict[layer.name]:
+                    x = inserted_layer(x)
+                cur_layer = layer if not q_layer_dict else q_layer_dict[layer.name]
+                x = cur_layer(x)
+            else:
+                x = layer(input_tensors)
+
+            output_tensor_dict[layer.name] = x
+            if layer.name in self.model.output_names:
+                self.model_outputs.append(x)
+
+        return tf.keras.models.Model(inputs=self.model.inputs, outputs=self.model_outputs)
```

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/algorithms/static_quant/keras.yaml` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/algorithms/static_quant/keras.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/algorithms/static_quant/tensorflow.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/algorithms/static_quant/tensorflow.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/algorithms/static_quant/tensorflow.yaml` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/algorithms/static_quant/tensorflow.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/keras/__init__.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/keras/layers/__init__.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/keras/layers/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #
-# Copyright (c) 2022 Intel Corporation
+# Copyright (c) 2024 Intel Corporation
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #   http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -17,7 +17,8 @@
 
 from neural_compressor.tensorflow.keras.layers.conv2d import QConv2D
 from neural_compressor.tensorflow.keras.layers.dense import QDense
 from neural_compressor.tensorflow.keras.layers.depthwise_conv2d import QDepthwiseConv2D
 from neural_compressor.tensorflow.keras.layers.pool2d import QAvgPool2D, QMaxPool2D
 from neural_compressor.tensorflow.keras.layers.quantizer import DeQuantize, FakeQuant, Quantize
 from neural_compressor.tensorflow.keras.layers.separable_conv2d import QSeparableConv2D
+from neural_compressor.tensorflow.keras.layers.layer_initializer import layer_initializer_dict
```

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/keras/layers/dense.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/keras/layers/dense.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #
-# Copyright (c) 2022 Intel Corporation
+# Copyright (c) 2024 Intel Corporation
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #   http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -22,61 +22,121 @@
 from tensorflow.keras import activations, backend, constraints, initializers, regularizers
 from tensorflow.keras.layers import Dense
 
 
 class QDense(Dense):
     def __init__(
         self,
+        name,
         units,
         activation=None,
         use_bias=True,
         kernel_initializer="glorot_uniform",
         bias_initializer="zeros",
         kernel_regularizer=None,
         bias_regularizer=None,
         activity_regularizer=None,
         kernel_constraint=None,
         bias_constraint=None,
-        min_value=-10000,
-        max_value=10000,
+        min_value=None,
+        max_value=None,
         **kwargs
     ):
         super(QDense, self).__init__(
+            name=name,
             units=units,
             activation=activation,
             use_bias=use_bias,
             kernel_initializer=kernel_initializer,
             bias_initializer=bias_initializer,
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
             activity_regularizer=activity_regularizer,
             kernel_constraint=kernel_constraint,
             bias_constraint=bias_constraint,
             **kwargs
         )
-        self.min_value = json.loads(min_value)
-        self.max_value = json.loads(max_value)
+        self.min_value = min_value
+        self.max_value = max_value
 
     def call(self, inputs):
+        kernel_size = self.kernel.shape[-1]
+
+        if not self.min_value:
+            self.min_value = [-10000] * kernel_size
+        if not self.max_value:
+            self.max_value = [10000] * kernel_size
+
         # add the Q/DQ here
         kernel, _, _ = quantization.quantize(
             self.kernel,
             self.min_value,
             self.max_value,
             tf.qint8,
             axis=1,
             mode="SCALED",
         )
+
         kernel = quantization.dequantize(
             kernel,
             self.min_value,
             self.max_value,
             axis=1,
             mode="SCALED",
         )
         outputs = tf.keras.backend.dot(inputs, kernel)
 
         if self.use_bias:
             outputs = tf.keras.backend.bias_add(outputs, self.bias)
         if self.activation is not None:
             outputs = self.activation(outputs)
         return outputs
+
+
+def initialize_int8_dense(fp32_layer):
+    kwargs = fp32_layer.get_config()
+
+    if "name" in kwargs:
+        del kwargs["name"]
+    if "units" in kwargs:
+        del kwargs["units"]
+    if "activation" in kwargs:
+        del kwargs["activation"]
+    if "use_bias" in kwargs:
+        del kwargs["use_bias"]
+    if "kernel_initializer" in kwargs:
+        del kwargs["kernel_initializer"]
+    if "bias_initializer" in kwargs:
+        del kwargs["bias_initializer"]
+    if "kernel_regularizer" in kwargs:
+        del kwargs["kernel_regularizer"]
+    if "activity_regularizer" in kwargs:
+        del kwargs["activity_regularizer"]
+    if "bias_regularizer" in kwargs:
+        del kwargs["bias_regularizer"]
+    if "kernel_constraint" in kwargs:
+        del kwargs["kernel_constraint"]
+    if "bias_constraint" in kwargs:
+        del kwargs["bias_constraint"]
+    if "min_value" in kwargs:
+        del kwargs["min_value"]
+    if "max_value" in kwargs:
+        del kwargs["max_value"]
+
+    q_layer = QDense(
+        name=fp32_layer.name,
+        units=fp32_layer.units,
+        activation=fp32_layer.activation,
+        use_bias=fp32_layer.use_bias,
+        kernel_initializer=fp32_layer.kernel_initializer,
+        bias_initializer=fp32_layer.bias_initializer,
+        kernel_regularizer=fp32_layer.kernel_regularizer,
+        bias_regularizer=fp32_layer.bias_regularizer,
+        activity_regularizer=fp32_layer.activity_regularizer,
+        kernel_constraint=fp32_layer.kernel_constraint,
+        bias_constraint=fp32_layer.bias_constraint,
+        min_value=fp32_layer.min_value,
+        max_value=fp32_layer.max_value,
+        **kwargs
+    )
+
+    return q_layer
```

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/keras/layers/depthwise_conv2d.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/keras/layers/depthwise_conv2d.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #
-# Copyright (c) 2022 Intel Corporation
+# Copyright (c) 2024 Intel Corporation
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #   http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -19,206 +19,192 @@
 
 import tensorflow as tf
 from tensorflow import quantization
 from tensorflow.keras import activations, constraints, initializers, regularizers
 
 from neural_compressor.tensorflow.utils import version1_gte_version2
 
-if version1_gte_version2(tf.__version__, "2.16.1"):
-    from keras.src import ops
-    from keras.src.layers.convolutional.base_depthwise_conv import BaseDepthwiseConv  # pylint: disable=E0401
-elif version1_gte_version2(tf.__version__, "2.13.0"):
+if version1_gte_version2(tf.__version__, "2.13.0"):
     from keras.src.layers.convolutional.base_depthwise_conv import DepthwiseConv  # pylint: disable=E0401
     from keras.src.utils import conv_utils, tf_utils  # pylint: disable=E0401
 else:
     from keras.layers.convolutional.base_depthwise_conv import DepthwiseConv  # pylint: disable=E0401
     from keras.utils import conv_utils, tf_utils  # pylint: disable=E0401
 
-if version1_gte_version2(tf.__version__, "2.16.1"):
 
-    class QDepthwiseConv2D(BaseDepthwiseConv):
-        def __init__(
-            self,
-            kernel_size,
-            min_value,
-            max_value,
-            strides=(1, 1),
-            padding="valid",
-            depth_multiplier=1,
-            data_format=None,
-            dilation_rate=(1, 1),
-            activation=None,
-            use_bias=True,
-            depthwise_initializer="glorot_uniform",
-            bias_initializer="zeros",
-            depthwise_regularizer=None,
-            bias_regularizer=None,
-            activity_regularizer=None,
-            depthwise_constraint=None,
-            bias_constraint=None,
+class QDepthwiseConv2D(DepthwiseConv):
+    def __init__(
+        self,
+        kernel_size,
+        strides=(1, 1),
+        padding="valid",
+        depth_multiplier=1,
+        data_format=None,
+        dilation_rate=(1, 1),
+        activation=None,
+        use_bias=True,
+        depthwise_initializer="glorot_uniform",
+        bias_initializer="zeros",
+        depthwise_regularizer=None,
+        bias_regularizer=None,
+        activity_regularizer=None,
+        depthwise_constraint=None,
+        bias_constraint=None,
+        min_value=None,
+        max_value=None,
+        **kwargs
+    ):
+        super().__init__(
+            2,
+            kernel_size=kernel_size,
+            strides=strides,
+            padding=padding,
+            depth_multiplier=depth_multiplier,
+            data_format=data_format,
+            dilation_rate=dilation_rate,
+            activation=activation,
+            use_bias=use_bias,
+            depthwise_initializer=depthwise_initializer,
+            bias_initializer=bias_initializer,
+            depthwise_regularizer=depthwise_regularizer,
+            bias_regularizer=bias_regularizer,
+            activity_regularizer=activity_regularizer,
+            depthwise_constraint=depthwise_constraint,
+            bias_constraint=bias_constraint,
             **kwargs
-        ):
-            super().__init__(
-                2,
-                kernel_size=kernel_size,
-                strides=strides,
-                padding=padding,
-                depth_multiplier=depth_multiplier,
-                data_format=data_format,
-                dilation_rate=dilation_rate,
-                activation=activation,
-                use_bias=use_bias,
-                depthwise_initializer=depthwise_initializer,
-                bias_initializer=bias_initializer,
-                depthwise_regularizer=depthwise_regularizer,
-                bias_regularizer=bias_regularizer,
-                activity_regularizer=activity_regularizer,
-                depthwise_constraint=depthwise_constraint,
-                bias_constraint=bias_constraint,
-                **kwargs
-            )
-            self.min_value = json.loads(min_value)
-            self.max_value = json.loads(max_value)
-
-        def call(self, inputs):
-            # add the Q/DQ here
-            kernel, _, _ = quantization.quantize(
-                self.depthwise_kernel, self.min_value, self.max_value, tf.qint8, axis=3, mode="SCALED"
-            )
-            kernel = quantization.dequantize(
-                kernel,
-                self.min_value,
-                self.max_value,
-                axis=3,
-                mode="SCALED",
-            )
-
-            input_channel = self._get_input_channel(inputs.shape)
-            outputs = ops.depthwise_conv(
-                inputs,
-                self.kernel,
-                strides=self.strides,
-                padding=self.padding,
-                dilation_rate=self.dilation_rate,
-                data_format=self.data_format,
-            )
-
-            if self.use_bias:
-                if self.data_format == "channels_last":
-                    bias_shape = (1,) * (self.rank + 1) + (self.depth_multiplier * input_channel,)
-                else:
-                    bias_shape = (1, self.depth_multiplier * input_channel) + (1,) * self.rank
-                bias = ops.reshape(self.bias, bias_shape)
-                outputs += bias
-
-            if self.activation is not None:
-                return self.activation(outputs)
-            return outputs
-
-else:
-
-    class QDepthwiseConv2D(DepthwiseConv):
-        def __init__(
-            self,
-            kernel_size,
-            min_value,
-            max_value,
-            strides=(1, 1),
-            padding="valid",
-            depth_multiplier=1,
-            data_format=None,
-            dilation_rate=(1, 1),
-            activation=None,
-            use_bias=True,
-            depthwise_initializer="glorot_uniform",
-            bias_initializer="zeros",
-            depthwise_regularizer=None,
-            bias_regularizer=None,
-            activity_regularizer=None,
-            depthwise_constraint=None,
-            bias_constraint=None,
-            **kwargs
-        ):
-            super().__init__(
-                2,
-                kernel_size=kernel_size,
-                strides=strides,
-                padding=padding,
-                depth_multiplier=depth_multiplier,
-                data_format=data_format,
-                dilation_rate=dilation_rate,
-                activation=activation,
-                use_bias=use_bias,
-                depthwise_initializer=depthwise_initializer,
-                bias_initializer=bias_initializer,
-                depthwise_regularizer=depthwise_regularizer,
-                bias_regularizer=bias_regularizer,
-                activity_regularizer=activity_regularizer,
-                depthwise_constraint=depthwise_constraint,
-                bias_constraint=bias_constraint,
-                **kwargs
-            )
-            self.min_value = json.loads(min_value)
-            self.max_value = json.loads(max_value)
-
-        def call(self, inputs):
-            # add the Q/DQ here
-            kernel, _, _ = quantization.quantize(
-                self.depthwise_kernel, self.min_value, self.max_value, tf.qint8, axis=3, mode="SCALED"
-            )
-            kernel = quantization.dequantize(
-                kernel,
-                self.min_value,
-                self.max_value,
-                axis=3,
-                mode="SCALED",
-            )
-            outputs = tf.keras.backend.depthwise_conv2d(
-                inputs,
-                kernel,
-                strides=self.strides,
-                padding=self.padding,
-                data_format=self.data_format,
-                dilation_rate=self.dilation_rate,
-            )
-
-            if self.use_bias:
-                outputs = tf.keras.backend.bias_add(outputs, self.bias, data_format=self.data_format)
-
-            if self.activation is not None:
-                return self.activation(outputs)
-
-            return outputs
-
-        @classmethod
-        def from_config(cls, config):
-            return cls(**config)
-
-        @tf_utils.shape_type_conversion
-        def compute_output_shape(self, input_shape):
-            if self.data_format == "channels_first":
-                rows = input_shape[2]
-                cols = input_shape[3]
-                out_filters = input_shape[1] * self.depth_multiplier
-            elif self.data_format == "channels_last":
-                rows = input_shape[1]
-                cols = input_shape[2]
-                out_filters = input_shape[3] * self.depth_multiplier
-
-            rows = conv_utils.conv_output_length(
-                rows,
-                self.kernel_size[0],
-                self.padding,
-                self.strides[0],
-                self.dilation_rate[0],
-            )
-            cols = conv_utils.conv_output_length(
-                cols,
-                self.kernel_size[1],
-                self.padding,
-                self.strides[1],
-                self.dilation_rate[1],
-            )
-            if self.data_format == "channels_first":
-                return (input_shape[0], out_filters, rows, cols)
-            elif self.data_format == "channels_last":
-                return (input_shape[0], rows, cols, out_filters)
+        )
+        self.min_value = min_value
+        self.max_value = max_value
+
+    def call(self, inputs):
+        depthwise_kernel_size = self.depthwise_kernel.shape[-1]
+
+        if not self.min_value:
+            self.min_value = [-10000] * depthwise_kernel_size
+        if not self.max_value:
+            self.max_value = [10000] * depthwise_kernel_size
+
+        # add the Q/DQ here
+        kernel, _, _ = quantization.quantize(
+            self.depthwise_kernel, self.min_value, self.max_value, tf.qint8, axis=3, mode="SCALED"
+        )
+        kernel = quantization.dequantize(
+            kernel,
+            self.min_value,
+            self.max_value,
+            axis=3,
+            mode="SCALED",
+        )
+        outputs = tf.keras.backend.depthwise_conv2d(
+            inputs,
+            kernel,
+            strides=self.strides,
+            padding=self.padding,
+            data_format=self.data_format,
+            dilation_rate=self.dilation_rate,
+        )
+
+        if self.use_bias:
+            outputs = tf.keras.backend.bias_add(outputs, self.bias, data_format=self.data_format)
+
+        if self.activation is not None:
+            return self.activation(outputs)
+
+        return outputs
+
+    @classmethod
+    def from_config(cls, config):
+        return cls(**config)
+
+    @tf_utils.shape_type_conversion
+    def compute_output_shape(self, input_shape):
+        if self.data_format == "channels_first":
+            rows = input_shape[2]
+            cols = input_shape[3]
+            out_filters = input_shape[1] * self.depth_multiplier
+        elif self.data_format == "channels_last":
+            rows = input_shape[1]
+            cols = input_shape[2]
+            out_filters = input_shape[3] * self.depth_multiplier
+
+        rows = conv_utils.conv_output_length(
+            rows,
+            self.kernel_size[0],
+            self.padding,
+            self.strides[0],
+            self.dilation_rate[0],
+        )
+        cols = conv_utils.conv_output_length(
+            cols,
+            self.kernel_size[1],
+            self.padding,
+            self.strides[1],
+            self.dilation_rate[1],
+        )
+        if self.data_format == "channels_first":
+            return (input_shape[0], out_filters, rows, cols)
+        elif self.data_format == "channels_last":
+            return (input_shape[0], rows, cols, out_filters)
+
+
+def initialize_int8_depthwise_conv2d(fp32_layer):
+    kwargs = fp32_layer.get_config()
+    q_name = fp32_layer.name
+
+    if "name" in kwargs:
+        del kwargs["name"]
+    if "kernel_size" in kwargs:
+        del kwargs["kernel_size"]
+    if "strides" in kwargs:
+        del kwargs["strides"]
+    if "padding" in kwargs:
+        del kwargs["padding"]
+    if "depth_multiplier" in kwargs:
+        del kwargs["depth_multiplier"]
+    if "data_format" in kwargs:
+        del kwargs["data_format"]
+    if "dilation_rate" in kwargs:
+        del kwargs["dilation_rate"]
+    if "activation" in kwargs:
+        del kwargs["activation"]
+    if "use_bias" in kwargs:
+        del kwargs["use_bias"]
+    if "depthwise_initializer" in kwargs:
+        del kwargs["depthwise_initializer"]
+    if "bias_initializer" in kwargs:
+        del kwargs["bias_initializer"]
+    if "depthwise_regularizer" in kwargs:
+        del kwargs["depthwise_regularizer"]
+    if "activity_regularizer" in kwargs:
+        del kwargs["activity_regularizer"]
+    if "bias_regularizer" in kwargs:
+        del kwargs["bias_regularizer"]
+    if "depthwise_constraint" in kwargs:
+        del kwargs["depthwise_constraint"]
+    if "bias_constraint" in kwargs:
+        del kwargs["bias_constraint"]
+    if "min_value" in kwargs:
+        del kwargs["min_value"]
+    if "max_value" in kwargs:
+        del kwargs["max_value"]
+
+    return QDepthwiseConv2D(
+        name=q_name,
+        kernel_size=fp32_layer.kernel_size,
+        strides=fp32_layer.strides,
+        padding=fp32_layer.padding,
+        depth_multiplier=fp32_layer.depth_multiplier,
+        data_format=fp32_layer.data_format,
+        dilation_rate=fp32_layer.dilation_rate,
+        activation=fp32_layer.activation,
+        use_bias=fp32_layer.use_bias,
+        depthwise_initializer=fp32_layer.depthwise_initializer,
+        bias_initializer=fp32_layer.bias_initializer,
+        depthwise_regularizer=fp32_layer.depthwise_regularizer,
+        bias_regularizer=fp32_layer.bias_regularizer,
+        activity_regularizer=fp32_layer.activity_regularizer,
+        depthwise_constraint=fp32_layer.depthwise_constraint,
+        bias_constraint=fp32_layer.bias_constraint,
+        min_value=fp32_layer.min_value,
+        max_value=fp32_layer.max_value,
+        **kwargs
+    )
```

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/keras/layers/quantizer.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/keras/layers/quantizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #
-# Copyright (c) 2022 Intel Corporation
+# Copyright (c) 2024 Intel Corporation
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #   http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -22,24 +22,25 @@
 
 class FakeQuant(Layer):
     def __init__(self, mode="per_tensor", T="s8", **kwargs):
         super(FakeQuant, self).__init__(**kwargs)
         self.mode = mode
         self.T = T
         self.axis = 1 if mode == "per_channel" else 0
-        self.min_value = tf.constant(np.finfo(np.float32).max, dtype=tf.float32)
-        self.max_value = tf.constant(np.finfo(np.float32).min, dtype=tf.float32)
+        self.min_value = tf.constant(np.finfo(np.float32).min, dtype=tf.float32)
+        self.max_value = tf.constant(np.finfo(np.float32).max, dtype=tf.float32)
 
     def call(self, inputs):
         if self.mode == "per_tensor":
             self.min_value = tf.math.reduce_min(inputs)
             self.max_value = tf.math.reduce_max(inputs)
         else:
             self.min_value = tf.math.reduce_min(inputs, axis=self.axis)
             self.max_value = tf.math.reduce_max(inputs, axis=self.axis)
+
         return inputs
 
     def compute_output_shape(self, input_shape):
         input_shape = tf.TensorShape(input_shape).as_list()
         return input_shape
 
     @classmethod
```

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/keras/layers/separable_conv2d.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/keras/layers/separable_conv2d.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #
-# Copyright (c) 2022 Intel Corporation
+# Copyright (c) 2024 Intel Corporation
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #   http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -19,200 +19,191 @@
 
 import tensorflow as tf
 from tensorflow import quantization
 from tensorflow.keras import activations, constraints, initializers, regularizers
 
 from neural_compressor.tensorflow.utils import version1_gte_version2
 
-if version1_gte_version2(tf.__version__, "2.16.1"):
-    from keras.src import ops
-    from keras.src.layers.convolutional.base_separable_conv import BaseSeparableConv  # pylint: disable=E0401
-elif version1_gte_version2(tf.__version__, "2.13.0"):
+if version1_gte_version2(tf.__version__, "2.13.0"):
     from keras.src.layers.convolutional.base_separable_conv import SeparableConv  # pylint: disable=E0401
     from keras.src.utils import conv_utils  # pylint: disable=E0401
 else:
     from keras.layers.convolutional.base_separable_conv import SeparableConv  # pylint: disable=E0401
     from keras.utils import conv_utils  # pylint: disable=E0401
 
-if version1_gte_version2(tf.__version__, "2.16.1"):
 
-    class QSeparableConv2D(BaseSeparableConv):
-        def __init__(
-            self,
-            filters,
-            kernel_size,
-            min_value,
-            max_value,
-            strides=(1, 1),
-            padding="valid",
-            data_format=None,
-            dilation_rate=(1, 1),
-            depth_multiplier=1,
-            activation=None,
-            use_bias=True,
-            depthwise_initializer="glorot_uniform",
-            pointwise_initializer="glorot_uniform",
-            bias_initializer="zeros",
-            depthwise_regularizer=None,
-            pointwise_regularizer=None,
-            bias_regularizer=None,
-            activity_regularizer=None,
-            depthwise_constraint=None,
-            pointwise_constraint=None,
-            bias_constraint=None,
+class QSeparableConv2D(SeparableConv):
+    def __init__(
+        self,
+        name,
+        filters,
+        kernel_size,
+        strides=(1, 1),
+        padding="valid",
+        data_format=None,
+        dilation_rate=(1, 1),
+        depth_multiplier=1,
+        activation=None,
+        use_bias=True,
+        depthwise_initializer="glorot_uniform",
+        pointwise_initializer="glorot_uniform",
+        bias_initializer="zeros",
+        depthwise_regularizer=None,
+        pointwise_regularizer=None,
+        bias_regularizer=None,
+        activity_regularizer=None,
+        depthwise_constraint=None,
+        pointwise_constraint=None,
+        bias_constraint=None,
+        min_value=None,
+        max_value=None,
+        **kwargs
+    ):
+        super().__init__(
+            name=name,
+            rank=2,
+            filters=filters,
+            kernel_size=kernel_size,
+            strides=strides,
+            padding=padding,
+            data_format=data_format,
+            dilation_rate=dilation_rate,
+            depth_multiplier=depth_multiplier,
+            activation=activations.get(activation),
+            use_bias=use_bias,
+            depthwise_initializer=initializers.get(depthwise_initializer),
+            pointwise_initializer=initializers.get(pointwise_initializer),
+            bias_initializer=initializers.get(bias_initializer),
+            depthwise_regularizer=regularizers.get(depthwise_regularizer),
+            pointwise_regularizer=regularizers.get(pointwise_regularizer),
+            bias_regularizer=regularizers.get(bias_regularizer),
+            activity_regularizer=regularizers.get(activity_regularizer),
+            depthwise_constraint=constraints.get(depthwise_constraint),
+            pointwise_constraint=constraints.get(pointwise_constraint),
+            bias_constraint=constraints.get(bias_constraint),
             **kwargs
-        ):
-            super().__init__(
-                rank=2,
-                filters=filters,
-                kernel_size=kernel_size,
-                strides=strides,
-                padding=padding,
-                data_format=data_format,
-                dilation_rate=dilation_rate,
-                depth_multiplier=depth_multiplier,
-                activation=activations.get(activation),
-                use_bias=use_bias,
-                depthwise_initializer=initializers.get(depthwise_initializer),
-                pointwise_initializer=initializers.get(pointwise_initializer),
-                bias_initializer=initializers.get(bias_initializer),
-                depthwise_regularizer=regularizers.get(depthwise_regularizer),
-                pointwise_regularizer=regularizers.get(pointwise_regularizer),
-                bias_regularizer=regularizers.get(bias_regularizer),
-                activity_regularizer=regularizers.get(activity_regularizer),
-                depthwise_constraint=constraints.get(depthwise_constraint),
-                pointwise_constraint=constraints.get(pointwise_constraint),
-                bias_constraint=constraints.get(bias_constraint),
-                **kwargs
-            )
-
-            self.min_value = json.loads(min_value)
-            self.max_value = json.loads(max_value)
-
-        def call(self, inputs):
-            # (TODO) it's ugly that we can't get the point_wise min/max here
-            depthwise_kernel, _, _ = quantization.quantize(
-                self.depthwise_kernel, self.min_value, self.max_value, tf.qint8, axis=3, mode="SCALED"
-            )
-            depthwise_kernel = quantization.dequantize(
-                depthwise_kernel,
-                self.min_value,
-                self.max_value,
-                axis=3,
-                mode="SCALED",
-            )
-
-            outputs = ops.separable_conv(
-                inputs,
-                self.depthwise_kernel,
-                self.pointwise_kernel,
-                strides=self.strides,
-                padding=self.padding,
-                dilation_rate=self.dilation_rate,
-                data_format=self.data_format,
-            )
-
-            if self.use_bias:
-                if self.data_format == "channels_last":
-                    bias_shape = (1,) * (self.rank + 1) + (self.filters,)
-                else:
-                    bias_shape = (1, self.filters) + (1,) * self.rank
-                bias = ops.reshape(self.bias, bias_shape)
-                outputs += bias
-
-            if self.activation is not None:
-                return self.activation(outputs)
-            return outputs
+        )
 
-else:
+        self.min_value = min_value
+        self.max_value = max_value
 
-    class QSeparableConv2D(SeparableConv):
-        def __init__(
-            self,
-            filters,
-            kernel_size,
-            min_value,
-            max_value,
-            strides=(1, 1),
-            padding="valid",
-            data_format=None,
-            dilation_rate=(1, 1),
-            depth_multiplier=1,
-            activation=None,
-            use_bias=True,
-            depthwise_initializer="glorot_uniform",
-            pointwise_initializer="glorot_uniform",
-            bias_initializer="zeros",
-            depthwise_regularizer=None,
-            pointwise_regularizer=None,
-            bias_regularizer=None,
-            activity_regularizer=None,
-            depthwise_constraint=None,
-            pointwise_constraint=None,
-            bias_constraint=None,
-            **kwargs
-        ):
-            super().__init__(
-                rank=2,
-                filters=filters,
-                kernel_size=kernel_size,
-                strides=strides,
-                padding=padding,
-                data_format=data_format,
-                dilation_rate=dilation_rate,
-                depth_multiplier=depth_multiplier,
-                activation=activations.get(activation),
-                use_bias=use_bias,
-                depthwise_initializer=initializers.get(depthwise_initializer),
-                pointwise_initializer=initializers.get(pointwise_initializer),
-                bias_initializer=initializers.get(bias_initializer),
-                depthwise_regularizer=regularizers.get(depthwise_regularizer),
-                pointwise_regularizer=regularizers.get(pointwise_regularizer),
-                bias_regularizer=regularizers.get(bias_regularizer),
-                activity_regularizer=regularizers.get(activity_regularizer),
-                depthwise_constraint=constraints.get(depthwise_constraint),
-                pointwise_constraint=constraints.get(pointwise_constraint),
-                bias_constraint=constraints.get(bias_constraint),
-                **kwargs
-            )
-
-            self.min_value = json.loads(min_value)
-            self.max_value = json.loads(max_value)
-
-        def call(self, inputs):
-            if self.data_format == "channels_last":
-                strides = (1,) + self.strides + (1,)
-            else:
-                strides = (1, 1) + self.strides
-            # (TODO) it's ugly that we can't get the point_wise min/max here
-            depthwise_kernel, _, _ = quantization.quantize(
-                self.depthwise_kernel, self.min_value, self.max_value, tf.qint8, axis=3, mode="SCALED"
-            )
-            depthwise_kernel = quantization.dequantize(
-                depthwise_kernel,
-                self.min_value,
-                self.max_value,
-                axis=3,
-                mode="SCALED",
-            )
-
-            outputs = tf.compat.v1.nn.separable_conv2d(
-                inputs,
-                depthwise_kernel,
-                self.pointwise_kernel,
-                strides=strides,
-                padding=self.padding.upper(),
-                rate=self.dilation_rate,
-                data_format=conv_utils.convert_data_format(self.data_format, ndim=4),
-            )
-
-            if self.use_bias:
-                outputs = tf.keras.backend.bias_add(outputs, self.bias, data_format=self.data_format)
-
-            if self.activation is not None:
-                return self.activation(outputs)
-
-            return outputs
-
-        @classmethod
-        def from_config(cls, config):
-            return cls(**config)
+    def call(self, inputs):
+        depthwise_kernel_size = self.depthwise_kernel.shape[-1]
+
+        if not self.min_value:
+            self.min_value = [-10000] * depthwise_kernel_size
+        if not self.max_value:
+            self.max_value = [10000] * depthwise_kernel_size
+
+        # TODO it's ugly that we can't get the point_wise min/max here
+        depthwise_kernel, _, _ = quantization.quantize(
+            self.depthwise_kernel, self.min_value, self.max_value, tf.qint8, axis=3, mode="SCALED"
+        )
+        depthwise_kernel = quantization.dequantize(
+            depthwise_kernel,
+            self.min_value,
+            self.max_value,
+            axis=3,
+            mode="SCALED",
+        )
+
+        if self.data_format == "channels_last":
+            strides = (1,) + self.strides + (1,)
+        else:
+            strides = (1, 1) + self.strides
+
+        outputs = tf.compat.v1.nn.separable_conv2d(
+            inputs,
+            depthwise_kernel,
+            self.pointwise_kernel,
+            strides=strides,
+            padding=self.padding.upper(),
+            rate=self.dilation_rate,
+            data_format=conv_utils.convert_data_format(self.data_format, ndim=4),
+        )
+
+        if self.use_bias:
+            outputs = tf.keras.backend.bias_add(outputs, self.bias, data_format=self.data_format)
+
+        if self.activation is not None:
+            return self.activation(outputs)
+
+        return outputs
+
+    @classmethod
+    def from_config(cls, config):
+        return cls(**config)
+
+
+def initialize_int8_separable_conv2d(fp32_layer):
+    kwargs = fp32_layer.get_config()
+
+    if "name" in kwargs:
+        del kwargs["name"]
+    if "filters" in kwargs:
+        del kwargs["filters"]
+    if "kernel_size" in kwargs:
+        del kwargs["kernel_size"]
+    if "strides" in kwargs:
+        del kwargs["strides"]
+    if "padding" in kwargs:
+        del kwargs["padding"]
+    if "data_format" in kwargs:
+        del kwargs["data_format"]
+    if "dilation_rate" in kwargs:
+        del kwargs["dilation_rate"]
+    if "depth_multiplier" in kwargs:
+        del kwargs["depth_multiplier"]
+    if "activation" in kwargs:
+        del kwargs["activation"]
+    if "use_bias" in kwargs:
+        del kwargs["use_bias"]
+    if "depthwise_initializer" in kwargs:
+        del kwargs["depthwise_initializer"]
+    if "pointwise_initializer" in kwargs:
+        del kwargs["pointwise_initializer"]
+    if "bias_initializer" in kwargs:
+        del kwargs["bias_initializer"]
+    if "depthwise_regularizer" in kwargs:
+        del kwargs["depthwise_regularizer"]
+    if "pointwise_regularizer" in kwargs:
+        del kwargs["pointwise_regularizer"]
+    if "activity_regularizer" in kwargs:
+        del kwargs["activity_regularizer"]
+    if "bias_regularizer" in kwargs:
+        del kwargs["bias_regularizer"]
+    if "depthwise_constraint" in kwargs:
+        del kwargs["depthwise_constraint"]
+    if "pointwise_constraint" in kwargs:
+        del kwargs["pointwise_constraint"]
+    if "bias_constraint" in kwargs:
+        del kwargs["bias_constraint"]
+    if "min_value" in kwargs:
+        del kwargs["min_value"]
+    if "max_value" in kwargs:
+        del kwargs["max_value"]
+
+    return QSeparableConv2D(
+        name=fp32_layer.name,
+        filters=fp32_layer.filters,
+        kernel_size=fp32_layer.kernel_size,
+        strides=fp32_layer.strides,
+        padding=fp32_layer.padding,
+        data_format=fp32_layer.data_format,
+        dilation_rate=fp32_layer.dilation_rate,
+        depth_multiplier=fp32_layer.depth_multiplier,
+        activation=fp32_layer.activation,
+        use_bias=fp32_layer.use_bias,
+        depthwise_initializer=fp32_layer.depthwise_initializer,
+        pointwise_initializer=fp32_layer.pointwise_initializer,
+        bias_initializer=fp32_layer.bias_initializer,
+        depthwise_regularizer=fp32_layer.depthwise_regularizer,
+        pointwise_regularizer=fp32_layer.pointwise_regularizer,
+        bias_regularizer=fp32_layer.bias_regularizer,
+        activity_regularizer=fp32_layer.activity_regularizer,
+        depthwise_constraint=fp32_layer.depthwise_constraint,
+        pointwise_constraint=fp32_layer.pointwise_constraint,
+        bias_constraint=fp32_layer.bias_constraint,
+        min_value=fp32_layer.min_value,
+        max_value=fp32_layer.max_value,
+        **kwargs
+    )
```

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/keras/quantization/__init__.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/keras/quantization/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/keras/quantization/config.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/keras/quantization/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         supported_configs.append(OperatorConfig(config=static_quant_config, operators=operators))
         cls.supported_configs = supported_configs
 
     @staticmethod
     def get_model_info(model) -> List[Tuple[str, Callable]]:
         white_list = [
             "Dense",
-            "Conv2d",
+            "Conv2D",
             "DepthwiseConv2D",
             "SeparableConv2D",
             "AvgPool2D",
             "AveragePooling2D",
             "MaxPool2D",
             "MaxPooling2D",
         ]
```

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/__init__.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/algorithm_entry.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/algorithm_entry.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/autotune.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/autotune.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/config.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/config.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/quantize.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/quantize.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/__init__.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_converter.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_converter.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_converter_without_calib.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_converter_without_calib.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/__init__.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/bf16/__init__.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/bf16/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/bf16/bf16_convert.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/bf16/bf16_convert.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/bf16/dequantize_cast_optimizer.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/bf16/dequantize_cast_optimizer.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/__init__.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/convert_add_to_biasadd.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/convert_add_to_biasadd.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/convert_layout.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/convert_layout.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/convert_leakyrelu.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/convert_leakyrelu.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/convert_nan_to_random.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/convert_nan_to_random.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/convert_placeholder_to_const.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/convert_placeholder_to_const.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/dilated_contraction.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/dilated_contraction.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/dummy_biasadd.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/dummy_biasadd.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/expanddims_optimizer.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/expanddims_optimizer.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fetch_weight_from_reshape.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fetch_weight_from_reshape.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fold_batch_norm.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fold_batch_norm.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fold_constant.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fold_constant.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fuse_biasadd_add.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fuse_biasadd_add.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fuse_column_wise_mul.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fuse_column_wise_mul.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fuse_conv_with_math.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fuse_conv_with_math.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fuse_decomposed_bn.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fuse_decomposed_bn.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fuse_decomposed_in.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fuse_decomposed_in.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fuse_gelu.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fuse_gelu.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fuse_layer_norm.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fuse_layer_norm.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fuse_pad_with_conv.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fuse_pad_with_conv.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fuse_pad_with_fp32_conv.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fuse_pad_with_fp32_conv.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fuse_reshape_transpose.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/fuse_reshape_transpose.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/graph_cse_optimizer.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/graph_cse_optimizer.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/grappler_pass.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/grappler_pass.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/insert_print_node.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/insert_print_node.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/move_squeeze_after_relu.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/move_squeeze_after_relu.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/pre_optimize.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/pre_optimize.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/remove_training_nodes.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/remove_training_nodes.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/rename_batch_norm.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/rename_batch_norm.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/split_shared_input.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/split_shared_input.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/strip_equivalent_nodes.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/strip_equivalent_nodes.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/strip_unused_nodes.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/strip_unused_nodes.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/switch_optimizer.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/generic/switch_optimizer.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/graph_base.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/graph_base.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/__init__.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/freeze_fake_quant.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/freeze_fake_quant.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/freeze_value.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/freeze_value.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/freeze_value_without_calib.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/freeze_value_without_calib.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/fuse_conv_redundant_dequantize.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/fuse_conv_redundant_dequantize.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/fuse_conv_requantize.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/fuse_conv_requantize.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/fuse_matmul_redundant_dequantize.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/fuse_matmul_redundant_dequantize.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/fuse_matmul_requantize.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/fuse_matmul_requantize.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/meta_op_optimizer.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/meta_op_optimizer.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/post_hostconst_converter.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/post_hostconst_converter.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/post_quantized_op_cse.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/post_quantized_op_cse.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/rnn_convert.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/rnn_convert.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/scale_propagation.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/int8/scale_propagation.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/qdq/__init__.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/qdq/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/qdq/insert_qdq_pattern.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/qdq/insert_qdq_pattern.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/qdq/merge_duplicated_qdq.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/qdq/merge_duplicated_qdq.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_rewriter/qdq/share_qdq_y_pattern.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_rewriter/qdq/share_qdq_y_pattern.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/graph_util.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/graph_util.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/__init__.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/qat/__init__.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/qat/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/qat/fake_quantize.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/qat/fake_quantize.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/qat/quantize_config.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/qat/quantize_config.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/qat/quantize_helper.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/qat/quantize_helper.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/qat/quantize_layers/__init__.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/qat/quantize_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/qat/quantize_layers/optimize_layer.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/qat/quantize_layers/optimize_layer.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/qat/quantize_layers/quantize_layer_add.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/qat/quantize_layers/quantize_layer_add.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/qat/quantize_layers/quantize_layer_base.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/qat/quantize_layers/quantize_layer_base.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/qat/quantize_layers/quantize_layer_bn.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/qat/quantize_layers/quantize_layer_bn.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/qat/quantize_wrapper.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/qat/quantize_wrapper.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/qdq/__init__.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/qdq/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/qdq/fuse_qdq_bn.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/qdq/fuse_qdq_bn.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/qdq/fuse_qdq_concatv2.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/qdq/fuse_qdq_concatv2.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/qdq/fuse_qdq_conv.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/qdq/fuse_qdq_conv.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/qdq/fuse_qdq_deconv.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/qdq/fuse_qdq_deconv.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/qdq/fuse_qdq_in.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/qdq/fuse_qdq_in.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/qdq/fuse_qdq_matmul.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/qdq/fuse_qdq_matmul.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/qdq/fuse_qdq_pooling.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/qdq/fuse_qdq_pooling.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/qdq/optimize_qdq.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/qdq/optimize_qdq.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/quantize_graph_base.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/quantize_graph_base.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/quantize_graph_bn.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/quantize_graph_bn.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/quantize_graph_concatv2.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/quantize_graph_concatv2.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/quantize_graph_conv.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/quantize_graph_conv.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/quantize_graph_for_intel_cpu.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/quantize_graph_for_intel_cpu.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/quantize_graph_matmul.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/quantize_graph_matmul.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph/quantize_graph_pooling.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph/quantize_graph_pooling.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/quantize_graph_common.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/quantize_graph_common.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/transform_graph/__init__.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/transform_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/transform_graph/bias_correction.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/transform_graph/bias_correction.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/transform_graph/graph_transform_base.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/transform_graph/graph_transform_base.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/transform_graph/insert_logging.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/transform_graph/insert_logging.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/transform_graph/rerange_quantized_concat.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/transform_graph/rerange_quantized_concat.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/quantization/utils/utility.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/quantization/utils/utility.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/utils/__init__.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/utils/constants.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/utils/constants.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/utils/data.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/utils/data.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/utils/model.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/utils/model.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/utils/model_wrappers.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/utils/model_wrappers.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/utils/nets_factory.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/utils/nets_factory.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor/tensorflow/utils/utility.py` & `neural_compressor_3x_tf-2.5.1/neural_compressor/tensorflow/utils/utility.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor_3x_tf.egg-info/PKG-INFO` & `neural_compressor_3x_tf-2.5.1/neural_compressor_3x_tf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neural_compressor_3x_tf
-Version: 2.5
+Version: 2.5.1
 Summary: Repository of Intel® Neural Compressor
 Home-page: https://github.com/intel/neural-compressor
 Author: Intel AIPT Team
 Author-email: feng.tian@intel.com, haihao.shen@intel.com, suyue.chen@intel.com
 License: Apache 2.0
 Keywords: quantization,auto-tuning,post-training static quantization,post-training dynamic quantization,quantization-aware training
 Classifier: Intended Audience :: Science/Research
@@ -16,15 +16,15 @@
 License-File: LICENSE
 License-File: third-party-programs.txt
 Requires-Dist: prettytable
 Requires-Dist: psutil
 Requires-Dist: py-cpuinfo
 Requires-Dist: pydantic
 Requires-Dist: pyyaml
-Requires-Dist: tensorflow
+Requires-Dist: tensorflow<=2.15.1
 
 <div align="center">
 
 Intel® Neural Compressor
 ===========================
 <h3> An open-source Python library supporting popular model compression techniques on all mainstream deep learning frameworks (TensorFlow, PyTorch, ONNX Runtime, and MXNet)</h3>
```

### Comparing `neural_compressor_3x_tf-2.5/neural_compressor_3x_tf.egg-info/SOURCES.txt` & `neural_compressor_3x_tf-2.5.1/neural_compressor_3x_tf.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 neural_compressor/tensorflow/algorithms/static_quant/tensorflow.py
 neural_compressor/tensorflow/algorithms/static_quant/tensorflow.yaml
 neural_compressor/tensorflow/keras/__init__.py
 neural_compressor/tensorflow/keras/layers/__init__.py
 neural_compressor/tensorflow/keras/layers/conv2d.py
 neural_compressor/tensorflow/keras/layers/dense.py
 neural_compressor/tensorflow/keras/layers/depthwise_conv2d.py
+neural_compressor/tensorflow/keras/layers/layer_initializer.py
 neural_compressor/tensorflow/keras/layers/pool2d.py
 neural_compressor/tensorflow/keras/layers/quantizer.py
 neural_compressor/tensorflow/keras/layers/separable_conv2d.py
 neural_compressor/tensorflow/keras/quantization/__init__.py
 neural_compressor/tensorflow/keras/quantization/config.py
 neural_compressor/tensorflow/quantization/__init__.py
 neural_compressor/tensorflow/quantization/algorithm_entry.py
```

### Comparing `neural_compressor_3x_tf-2.5/pyproject.toml` & `neural_compressor_3x_tf-2.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/setup.py` & `neural_compressor_3x_tf-2.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `neural_compressor_3x_tf-2.5/third-party-programs.txt` & `neural_compressor_3x_tf-2.5.1/third-party-programs.txt`

 * *Files identical despite different names*

