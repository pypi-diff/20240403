# Comparing `tmp/neural_compressor-2.5.tar.gz` & `tmp/neural_compressor-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neural_compressor-2.5.tar", last modified: Tue Mar 26 09:01:08 2024, max compression
+gzip compressed data, was "neural_compressor-2.5.1.tar", last modified: Wed Apr  3 13:33:46 2024, max compression
```

## Comparing `neural_compressor-2.5.tar` & `neural_compressor-2.5.1.tar`

### file list

```diff
@@ -1,634 +1,634 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.714343 neural_compressor-2.5/
--rw-r--r--   0 root         (0) root         (0)    11360 2024-03-26 08:53:13.000000 neural_compressor-2.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)    15587 2024-03-26 09:01:08.714343 neural_compressor-2.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    14096 2024-03-26 08:53:13.000000 neural_compressor-2.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.636340 neural_compressor-2.5/neural_coder/
--rw-r--r--   0 root         (0) root         (0)      749 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/__init__.py
--rw-r--r--   0 root         (0) root         (0)      668 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.643340 neural_compressor-2.5/neural_coder/backends/
--rw-r--r--   0 root         (0) root         (0)      583 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1382 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/intel_extension_for_transformers.yaml
--rw-r--r--   0 root         (0) root         (0)     1121 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/keras_inc.yaml
--rw-r--r--   0 root         (0) root         (0)     1039 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/nano_bf16.yaml
--rw-r--r--   0 root         (0) root         (0)     1059 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/nano_bf16_channels_last.yaml
--rw-r--r--   0 root         (0) root         (0)     1054 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/nano_bf16_ipex.yaml
--rw-r--r--   0 root         (0) root         (0)     1074 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/nano_bf16_ipex_channels_last.yaml
--rw-r--r--   0 root         (0) root         (0)     1038 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/nano_fp32_channels_last.yaml
--rw-r--r--   0 root         (0) root         (0)     1033 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/nano_fp32_ipex.yaml
--rw-r--r--   0 root         (0) root         (0)     1053 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/nano_fp32_ipex_channels_last.yaml
--rw-r--r--   0 root         (0) root         (0)      850 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/nano_gpu_to_cpu.yaml
--rw-r--r--   0 root         (0) root         (0)     1039 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/nano_int8.yaml
--rw-r--r--   0 root         (0) root         (0)     1058 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/nano_jit_bf16.yaml
--rw-r--r--   0 root         (0) root         (0)     1078 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/nano_jit_bf16_channels_last.yaml
--rw-r--r--   0 root         (0) root         (0)     1073 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/nano_jit_bf16_ipex.yaml
--rw-r--r--   0 root         (0) root         (0)     1093 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/nano_jit_bf16_ipex_channels_last.yaml
--rw-r--r--   0 root         (0) root         (0)     1038 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/nano_jit_fp32.yaml
--rw-r--r--   0 root         (0) root         (0)     1057 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/nano_jit_fp32_channels_last.yaml
--rw-r--r--   0 root         (0) root         (0)     1053 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/nano_jit_fp32_ipex.yaml
--rw-r--r--   0 root         (0) root         (0)     1072 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/nano_jit_fp32_ipex_channels_last.yaml
--rw-r--r--   0 root         (0) root         (0)     1045 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/nano_onnxruntime_fp32.yaml
--rw-r--r--   0 root         (0) root         (0)     1066 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/nano_onnxruntime_int8_qlinear.yaml
--rw-r--r--   0 root         (0) root         (0)     1042 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/nano_openvino_fp32.yaml
--rw-r--r--   0 root         (0) root         (0)     1063 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/nano_openvino_int8.yaml
--rw-r--r--   0 root         (0) root         (0)     1082 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/onnx_inc_dynamic_quant.yaml
--rw-r--r--   0 root         (0) root         (0)     1082 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/onnx_inc_static_quant_qdq.yaml
--rw-r--r--   0 root         (0) root         (0)     1086 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/onnx_inc_static_quant_qlinear.yaml
--rw-r--r--   0 root         (0) root         (0)      923 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/pytorch_aliblade.yaml
--rw-r--r--   0 root         (0) root         (0)     2655 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/pytorch_benchmark.yaml
--rw-r--r--   0 root         (0) root         (0)     1246 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/pytorch_channels_last.yaml
--rw-r--r--   0 root         (0) root         (0)     1380 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/pytorch_inc_bf16.yaml
--rw-r--r--   0 root         (0) root         (0)     1651 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/pytorch_inc_dynamic_quant.yaml
--rw-r--r--   0 root         (0) root         (0)     1761 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/pytorch_inc_dynamic_quant_fp8.yaml
--rw-r--r--   0 root         (0) root         (0)     1515 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/pytorch_inc_huggingface_optimum_dynamic.yaml
--rw-r--r--   0 root         (0) root         (0)     1548 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/pytorch_inc_huggingface_optimum_static.yaml
--rw-r--r--   0 root         (0) root         (0)     1713 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/pytorch_inc_static_quant_fx.yaml
--rw-r--r--   0 root         (0) root         (0)     1740 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/pytorch_inc_static_quant_fx_fp8.yaml
--rw-r--r--   0 root         (0) root         (0)     1274 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/pytorch_inc_static_quant_ipex.yaml
--rw-r--r--   0 root         (0) root         (0)     1332 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/pytorch_inc_static_quant_ipex_xpu.yaml
--rw-r--r--   0 root         (0) root         (0)     1306 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/pytorch_ipex_bf16.yaml
--rw-r--r--   0 root         (0) root         (0)     1076 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/pytorch_ipex_fp32.yaml
--rw-r--r--   0 root         (0) root         (0)     1540 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/pytorch_ipex_int8_dynamic_quant.yaml
--rw-r--r--   0 root         (0) root         (0)     1539 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/pytorch_ipex_int8_static_quant.yaml
--rw-r--r--   0 root         (0) root         (0)     1261 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/pytorch_jit_script.yaml
--rw-r--r--   0 root         (0) root         (0)     1235 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/pytorch_jit_script_ofi.yaml
--rw-r--r--   0 root         (0) root         (0)     1347 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/pytorch_jit_trace.yaml
--rw-r--r--   0 root         (0) root         (0)     1321 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/pytorch_jit_trace_ofi.yaml
--rw-r--r--   0 root         (0) root         (0)      861 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/pytorch_mixed_precision_cpu.yaml
--rw-r--r--   0 root         (0) root         (0)      861 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/pytorch_mixed_precision_cuda.yaml
--rw-r--r--   0 root         (0) root         (0)      843 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/pytorch_mixed_precision_intel_gpu.yaml
--rw-r--r--   0 root         (0) root         (0)     1201 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/pytorch_torchdynamo_jit_script.yaml
--rw-r--r--   0 root         (0) root         (0)     1235 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/pytorch_torchdynamo_jit_script_ofi.yaml
--rw-r--r--   0 root         (0) root         (0)     1216 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/pytorch_torchdynamo_jit_trace.yaml
--rw-r--r--   0 root         (0) root         (0)     1250 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/pytorch_torchdynamo_jit_trace_ofi.yaml
--rw-r--r--   0 root         (0) root         (0)     1118 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/backends/template.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.643340 neural_compressor-2.5/neural_coder/coders/
--rw-r--r--   0 root         (0) root         (0)      583 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/coders/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.644340 neural_compressor-2.5/neural_coder/coders/autoinc/
--rw-r--r--   0 root         (0) root         (0)      583 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/coders/autoinc/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26608 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/coders/autoinc/autoinc_harness.py
--rw-r--r--   0 root         (0) root         (0)     1752 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/coders/autoinc/calib_dataloader.py
--rw-r--r--   0 root         (0) root         (0)     1337 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/coders/autoinc/domain.py
--rw-r--r--   0 root         (0) root         (0)     4768 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/coders/autoinc/eval_func.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.645341 neural_compressor-2.5/neural_coder/coders/pytorch/
--rw-r--r--   0 root         (0) root         (0)      583 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/coders/pytorch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3192 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/coders/pytorch/batch_size.py
--rw-r--r--   0 root         (0) root         (0)     1460 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/coders/pytorch/change_trainer_to_nlptrainer.py
--rw-r--r--   0 root         (0) root         (0)     2941 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/coders/pytorch/cuda_to_cpu.py
--rw-r--r--   0 root         (0) root         (0)     6779 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/coders/pytorch/dummy_dataloader.py
--rw-r--r--   0 root         (0) root         (0)    23456 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/coders/pytorch/harness.py
--rw-r--r--   0 root         (0) root         (0)     2873 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/coders/pytorch/lightning.py
--rw-r--r--   0 root         (0) root         (0)     3616 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/coders/pytorch/reclaim_inference_transformers_trainer.py
--rw-r--r--   0 root         (0) root         (0)     5205 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/coders/pytorch/reclaim_inputs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.645341 neural_compressor-2.5/neural_coder/coders/tensorflow/
--rw-r--r--   0 root         (0) root         (0)      583 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/coders/tensorflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2728 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/coders/tensorflow/amp.py
--rw-r--r--   0 root         (0) root         (0)     2173 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/coders/tensorflow/inc.py
--rw-r--r--   0 root         (0) root         (0)     3623 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/coders/transform.py
--rw-r--r--   0 root         (0) root         (0)     3403 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/globals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.646340 neural_compressor-2.5/neural_coder/graphers/
--rw-r--r--   0 root         (0) root         (0)      583 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/graphers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11141 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/graphers/code_line.py
--rw-r--r--   0 root         (0) root         (0)     7143 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/graphers/function.py
--rw-r--r--   0 root         (0) root         (0)    12609 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/graphers/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.646340 neural_compressor-2.5/neural_coder/graphers/preloads/
--rw-r--r--   0 root         (0) root         (0)      583 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/graphers/preloads/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58209 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/graphers/preloads/transformers.yaml
--rw-r--r--   0 root         (0) root         (0)    53298 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/interface.py
--rw-r--r--   0 root         (0) root         (0)     3707 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/launcher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.647341 neural_compressor-2.5/neural_coder/utils/
--rw-r--r--   0 root         (0) root         (0)      583 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      902 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/utils/common.py
--rw-r--r--   0 root         (0) root         (0)     1746 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/utils/cpu_info.py
--rw-r--r--   0 root         (0) root         (0)     3014 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/utils/device.py
--rw-r--r--   0 root         (0) root         (0)     7500 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/utils/handle_user_input.py
--rw-r--r--   0 root         (0) root         (0)     5138 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/utils/line_operation.py
--rw-r--r--   0 root         (0) root         (0)    38116 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/utils/numa_launcher.py
--rw-r--r--   0 root         (0) root         (0)    18657 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/utils/pdf_report.py
--rw-r--r--   0 root         (0) root         (0)      604 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_coder/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.649341 neural_compressor-2.5/neural_compressor/
--rw-r--r--   0 root         (0) root         (0)     1190 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.653341 neural_compressor-2.5/neural_compressor/adaptor/
--rw-r--r--   0 root         (0) root         (0)      973 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7481 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/adaptor.py
--rw-r--r--   0 root         (0) root         (0)    45327 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/keras.py
--rw-r--r--   0 root         (0) root         (0)     5590 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/keras.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.653341 neural_compressor-2.5/neural_compressor/adaptor/keras_utils/
--rw-r--r--   0 root         (0) root         (0)      631 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/keras_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3576 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/keras_utils/conv2d.py
--rw-r--r--   0 root         (0) root         (0)     2568 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/keras_utils/dense.py
--rw-r--r--   0 root         (0) root         (0)     4710 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/keras_utils/depthwise_conv2d.py
--rw-r--r--   0 root         (0) root         (0)     1841 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/keras_utils/pool2d.py
--rw-r--r--   0 root         (0) root         (0)     4079 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/keras_utils/quantizer.py
--rw-r--r--   0 root         (0) root         (0)     4466 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/keras_utils/separable_conv2d.py
--rw-r--r--   0 root         (0) root         (0)    21979 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/mxnet.py
--rw-r--r--   0 root         (0) root         (0)    10616 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/mxnet.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.654341 neural_compressor-2.5/neural_compressor/adaptor/mxnet_utils/
--rw-r--r--   0 root         (0) root         (0)      655 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/mxnet_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30686 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/mxnet_utils/util.py
--rw-r--r--   0 root         (0) root         (0)   105870 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/onnxrt.py
--rw-r--r--   0 root         (0) root         (0)    20205 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/onnxrt.yaml
--rw-r--r--   0 root         (0) root         (0)    16912 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/onnxrt_cuda.yaml
--rw-r--r--   0 root         (0) root         (0)     2441 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/onnxrt_dml.yaml
--rw-r--r--   0 root         (0) root         (0)    15046 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/onnxrt_dnnl.yaml
--rw-r--r--   0 root         (0) root         (0)     4873 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/onnxrt_trt.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.655341 neural_compressor-2.5/neural_compressor/adaptor/ox_utils/
--rw-r--r--   0 root         (0) root         (0)      656 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/ox_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42456 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/ox_utils/calibration.py
--rw-r--r--   0 root         (0) root         (0)    15292 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/ox_utils/calibrator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.658341 neural_compressor-2.5/neural_compressor/adaptor/ox_utils/operators/
--rw-r--r--   0 root         (0) root         (0)     1026 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/ox_utils/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5348 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/ox_utils/operators/activation.py
--rw-r--r--   0 root         (0) root         (0)     1791 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/ox_utils/operators/argmax.py
--rw-r--r--   0 root         (0) root         (0)     4626 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/ox_utils/operators/attention.py
--rw-r--r--   0 root         (0) root         (0)     7462 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/ox_utils/operators/binary_op.py
--rw-r--r--   0 root         (0) root         (0)     7210 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/ox_utils/operators/concat.py
--rw-r--r--   0 root         (0) root         (0)    10211 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/ox_utils/operators/conv.py
--rw-r--r--   0 root         (0) root         (0)     3758 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/ox_utils/operators/direct_q8.py
--rw-r--r--   0 root         (0) root         (0)     4288 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/ox_utils/operators/embed_layernorm.py
--rw-r--r--   0 root         (0) root         (0)     5369 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/ox_utils/operators/gather.py
--rw-r--r--   0 root         (0) root         (0)     3500 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/ox_utils/operators/gavgpool.py
--rw-r--r--   0 root         (0) root         (0)     6410 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/ox_utils/operators/gemm.py
--rw-r--r--   0 root         (0) root         (0)     5627 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/ox_utils/operators/lstm.py
--rw-r--r--   0 root         (0) root         (0)     8323 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/ox_utils/operators/matmul.py
--rw-r--r--   0 root         (0) root         (0)     3293 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/ox_utils/operators/maxpool.py
--rw-r--r--   0 root         (0) root         (0)     1722 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/ox_utils/operators/norm.py
--rw-r--r--   0 root         (0) root         (0)     5767 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/ox_utils/operators/ops.py
--rw-r--r--   0 root         (0) root         (0)     4868 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/ox_utils/operators/pad.py
--rw-r--r--   0 root         (0) root         (0)     4513 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/ox_utils/operators/pooling.py
--rw-r--r--   0 root         (0) root         (0)     3375 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/ox_utils/operators/reduce.py
--rw-r--r--   0 root         (0) root         (0)     3412 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/ox_utils/operators/resize.py
--rw-r--r--   0 root         (0) root         (0)     6181 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/ox_utils/operators/split.py
--rw-r--r--   0 root         (0) root         (0)     3267 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/ox_utils/operators/unary_op.py
--rw-r--r--   0 root         (0) root         (0)    61261 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/ox_utils/quantizer.py
--rw-r--r--   0 root         (0) root         (0)    31618 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/ox_utils/smooth_quant.py
--rw-r--r--   0 root         (0) root         (0)    24424 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/ox_utils/util.py
--rw-r--r--   0 root         (0) root         (0)    46355 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/ox_utils/weight_only.py
--rw-r--r--   0 root         (0) root         (0)   234889 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/pytorch.py
--rw-r--r--   0 root         (0) root         (0)    16657 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/pytorch_cpu.yaml
--rw-r--r--   0 root         (0) root         (0)     2625 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/pytorch_gpu.yaml
--rw-r--r--   0 root         (0) root         (0)     6572 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/pytorch_ipex.yaml
--rw-r--r--   0 root         (0) root         (0)     2345 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/query.py
--rw-r--r--   0 root         (0) root         (0)   117093 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tensorflow.py
--rw-r--r--   0 root         (0) root         (0)    10069 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tensorflow.yaml
--rw-r--r--   0 root         (0) root         (0)     6941 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tensorflow_itex.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.659341 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/
--rw-r--r--   0 root         (0) root         (0)      657 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42617 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_converter.py
--rw-r--r--   0 root         (0) root         (0)    15850 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_converter_without_calib.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.660341 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/
--rw-r--r--   0 root         (0) root         (0)      665 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.660341 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/bf16/
--rw-r--r--   0 root         (0) root         (0)      669 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/bf16/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13750 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/bf16/bf16_convert.py
--rw-r--r--   0 root         (0) root         (0)     3229 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/bf16/dequantize_cast_optimizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.665341 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/
--rw-r--r--   0 root         (0) root         (0)      673 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3247 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/convert_add_to_biasadd.py
--rw-r--r--   0 root         (0) root         (0)     3885 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/convert_layout.py
--rw-r--r--   0 root         (0) root         (0)     3154 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/convert_leakyrelu.py
--rw-r--r--   0 root         (0) root         (0)     1933 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/convert_nan_to_random.py
--rw-r--r--   0 root         (0) root         (0)     4349 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/convert_placeholder_to_const.py
--rw-r--r--   0 root         (0) root         (0)     4079 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/dilated_contraction.py
--rw-r--r--   0 root         (0) root         (0)     5856 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/dummy_biasadd.py
--rw-r--r--   0 root         (0) root         (0)     3397 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/expanddims_optimizer.py
--rw-r--r--   0 root         (0) root         (0)     3956 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fetch_weight_from_reshape.py
--rw-r--r--   0 root         (0) root         (0)    13153 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fold_batch_norm.py
--rw-r--r--   0 root         (0) root         (0)     7509 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fold_constant.py
--rw-r--r--   0 root         (0) root         (0)     2894 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_biasadd_add.py
--rw-r--r--   0 root         (0) root         (0)     3885 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_column_wise_mul.py
--rw-r--r--   0 root         (0) root         (0)     4942 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_conv_with_math.py
--rw-r--r--   0 root         (0) root         (0)    16460 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_decomposed_bn.py
--rw-r--r--   0 root         (0) root         (0)    15582 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_decomposed_in.py
--rw-r--r--   0 root         (0) root         (0)     9504 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_gelu.py
--rw-r--r--   0 root         (0) root         (0)     9742 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_layer_norm.py
--rw-r--r--   0 root         (0) root         (0)     5477 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_pad_with_conv.py
--rw-r--r--   0 root         (0) root         (0)     5583 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_pad_with_fp32_conv.py
--rw-r--r--   0 root         (0) root         (0)     5889 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_reshape_transpose.py
--rw-r--r--   0 root         (0) root         (0)     5925 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/graph_cse_optimizer.py
--rw-r--r--   0 root         (0) root         (0)     3147 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/grappler_pass.py
--rw-r--r--   0 root         (0) root         (0)    12742 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/insert_print_node.py
--rw-r--r--   0 root         (0) root         (0)     6171 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/move_squeeze_after_relu.py
--rw-r--r--   0 root         (0) root         (0)    13729 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/pre_optimize.py
--rw-r--r--   0 root         (0) root         (0)     2779 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/remove_training_nodes.py
--rw-r--r--   0 root         (0) root         (0)     2316 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/rename_batch_norm.py
--rw-r--r--   0 root         (0) root         (0)     2618 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/split_shared_input.py
--rw-r--r--   0 root         (0) root         (0)     2115 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/strip_equivalent_nodes.py
--rw-r--r--   0 root         (0) root         (0)     1508 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/strip_unused_nodes.py
--rw-r--r--   0 root         (0) root         (0)     3432 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/switch_optimizer.py
--rw-r--r--   0 root         (0) root         (0)     1224 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/graph_base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.667341 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/
--rw-r--r--   0 root         (0) root         (0)      670 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7070 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/freeze_fake_quant.py
--rw-r--r--   0 root         (0) root         (0)    17659 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/freeze_value.py
--rw-r--r--   0 root         (0) root         (0)     5630 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/freeze_value_without_calib.py
--rw-r--r--   0 root         (0) root         (0)     7135 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/fuse_conv_redundant_dequantize.py
--rw-r--r--   0 root         (0) root         (0)    42958 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/fuse_conv_requantize.py
--rw-r--r--   0 root         (0) root         (0)     8240 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/fuse_matmul_redundant_dequantize.py
--rw-r--r--   0 root         (0) root         (0)    44838 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/fuse_matmul_requantize.py
--rw-r--r--   0 root         (0) root         (0)     5396 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/meta_op_optimizer.py
--rw-r--r--   0 root         (0) root         (0)     1895 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/post_hostconst_converter.py
--rw-r--r--   0 root         (0) root         (0)     5420 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/post_quantized_op_cse.py
--rw-r--r--   0 root         (0) root         (0)    16003 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/rnn_convert.py
--rw-r--r--   0 root         (0) root         (0)     4763 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/scale_propagation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.668341 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/onnx/
--rw-r--r--   0 root         (0) root         (0)      692 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/onnx/__init__.py
--rw-r--r--   0 root         (0) root         (0)    55660 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/onnx/onnx_graph.py
--rw-r--r--   0 root         (0) root         (0)    13491 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/onnx/onnx_node.py
--rw-r--r--   0 root         (0) root         (0)     4580 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/onnx/onnx_schema.py
--rw-r--r--   0 root         (0) root         (0)    22693 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/onnx/tf2onnx_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.668341 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/qdq/
--rw-r--r--   0 root         (0) root         (0)      669 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/qdq/__init__.py
--rw-r--r--   0 root         (0) root         (0)    37978 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/qdq/insert_qdq_pattern.py
--rw-r--r--   0 root         (0) root         (0)     4293 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/qdq/merge_duplicated_qdq.py
--rw-r--r--   0 root         (0) root         (0)     2539 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/qdq/share_qdq_y_pattern.py
--rw-r--r--   0 root         (0) root         (0)    42637 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.669341 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/
--rw-r--r--   0 root         (0) root         (0)      666 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.670341 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/qat/
--rw-r--r--   0 root         (0) root         (0)      670 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/qat/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8567 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/qat/fake_quantize.py
--rw-r--r--   0 root         (0) root         (0)     4623 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_config.py
--rw-r--r--   0 root         (0) root         (0)     3015 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.671342 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_layers/
--rw-r--r--   0 root         (0) root         (0)      675 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_layers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1265 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_layers/optimize_layer.py
--rw-r--r--   0 root         (0) root         (0)     3053 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_layers/quantize_layer_add.py
--rw-r--r--   0 root         (0) root         (0)     3116 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_layers/quantize_layer_base.py
--rw-r--r--   0 root         (0) root         (0)     2102 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_layers/quantize_layer_bn.py
--rw-r--r--   0 root         (0) root         (0)    10193 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.672341 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/
--rw-r--r--   0 root         (0) root         (0)      670 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13835 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_bn.py
--rw-r--r--   0 root         (0) root         (0)    12289 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_concatv2.py
--rw-r--r--   0 root         (0) root         (0)   112937 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_conv.py
--rw-r--r--   0 root         (0) root         (0)    27109 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_deconv.py
--rw-r--r--   0 root         (0) root         (0)     8235 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_in.py
--rw-r--r--   0 root         (0) root         (0)    55166 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_matmul.py
--rw-r--r--   0 root         (0) root         (0)     6063 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_pooling.py
--rw-r--r--   0 root         (0) root         (0)     7189 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/optimize_qdq.py
--rw-r--r--   0 root         (0) root         (0)    36897 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_base.py
--rw-r--r--   0 root         (0) root         (0)    13563 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_bn.py
--rw-r--r--   0 root         (0) root         (0)     4638 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_concatv2.py
--rw-r--r--   0 root         (0) root         (0)    20539 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_conv.py
--rw-r--r--   0 root         (0) root         (0)     5626 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_for_intel_cpu.py
--rw-r--r--   0 root         (0) root         (0)    17114 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_matmul.py
--rw-r--r--   0 root         (0) root         (0)     3198 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_pooling.py
--rw-r--r--   0 root         (0) root         (0)    19111 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph_common.py
--rw-r--r--   0 root         (0) root         (0)    23797 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/smooth_quant_calibration.py
--rw-r--r--   0 root         (0) root         (0)    13820 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/smooth_quant_scaler.py
--rw-r--r--   0 root         (0) root         (0)    14537 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/tf2onnx_converter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.673342 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/transform_graph/
--rw-r--r--   0 root         (0) root         (0)      662 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/transform_graph/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6046 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/transform_graph/bias_correction.py
--rw-r--r--   0 root         (0) root         (0)     3543 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/transform_graph/graph_transform_base.py
--rw-r--r--   0 root         (0) root         (0)     8974 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/transform_graph/insert_logging.py
--rw-r--r--   0 root         (0) root         (0)    14933 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/transform_graph/rerange_quantized_concat.py
--rw-r--r--   0 root         (0) root         (0)    33328 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/tf_utils/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.675342 neural_compressor-2.5/neural_compressor/adaptor/torch_utils/
--rw-r--r--   0 root         (0) root         (0)      657 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/torch_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1051 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/torch_utils/auto_round.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.676342 neural_compressor-2.5/neural_compressor/adaptor/torch_utils/autoround/
--rw-r--r--   0 root         (0) root         (0)      690 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/torch_utils/autoround/__init__.py
--rw-r--r--   0 root         (0) root         (0)    65995 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/torch_utils/autoround/autoround.py
--rw-r--r--   0 root         (0) root         (0)     3936 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/torch_utils/autoround/export.py
--rw-r--r--   0 root         (0) root         (0)    14501 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/torch_utils/autoround/model_wrapper.py
--rw-r--r--   0 root         (0) root         (0)    14977 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/torch_utils/autoround/sign_sgd.py
--rw-r--r--   0 root         (0) root         (0)    21376 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/torch_utils/awq.py
--rw-r--r--   0 root         (0) root         (0)     3492 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/torch_utils/bf16_convert.py
--rw-r--r--   0 root         (0) root         (0)    44360 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/torch_utils/gptq.py
--rw-r--r--   0 root         (0) root         (0)    25511 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/torch_utils/hawq_metric.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.676342 neural_compressor-2.5/neural_compressor/adaptor/torch_utils/layer_wise_quant/
--rw-r--r--   0 root         (0) root         (0)      748 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/torch_utils/layer_wise_quant/__init__.py
--rw-r--r--   0 root         (0) root         (0)    64065 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/torch_utils/layer_wise_quant/modified_pickle.py
--rw-r--r--   0 root         (0) root         (0)    11304 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/torch_utils/layer_wise_quant/quantize.py
--rw-r--r--   0 root         (0) root         (0)    12959 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/torch_utils/layer_wise_quant/torch_load.py
--rw-r--r--   0 root         (0) root         (0)    10151 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/torch_utils/layer_wise_quant/utils.py
--rw-r--r--   0 root         (0) root         (0)     1920 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/torch_utils/mixed_precision.py
--rw-r--r--   0 root         (0) root         (0)    23752 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/torch_utils/model_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     7138 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/torch_utils/pattern_detector.py
--rw-r--r--   0 root         (0) root         (0)     2720 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/torch_utils/symbolic_trace.py
--rw-r--r--   0 root         (0) root         (0)    12834 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/torch_utils/teq.py
--rw-r--r--   0 root         (0) root         (0)    50405 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/torch_utils/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.677342 neural_compressor-2.5/neural_compressor/adaptor/torch_utils/waq/
--rw-r--r--   0 root         (0) root         (0)      743 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/torch_utils/waq/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30061 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/torch_utils/waq/auto_alpha.py
--rw-r--r--   0 root         (0) root         (0)     4118 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/torch_utils/waq/calibration.py
--rw-r--r--   0 root         (0) root         (0)     9480 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/torch_utils/waq/graph_trace.py
--rw-r--r--   0 root         (0) root         (0)    26463 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/torch_utils/waq/smooth_quant.py
--rw-r--r--   0 root         (0) root         (0)    14485 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/torch_utils/waq/utils.py
--rw-r--r--   0 root         (0) root         (0)    30081 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/adaptor/torch_utils/weight_only.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.678342 neural_compressor-2.5/neural_compressor/algorithm/
--rw-r--r--   0 root         (0) root         (0)     1131 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/algorithm/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6362 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/algorithm/algorithm.py
--rw-r--r--   0 root         (0) root         (0)     6258 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/algorithm/fast_bias_correction.py
--rw-r--r--   0 root         (0) root         (0)     3877 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/algorithm/smooth_quant.py
--rw-r--r--   0 root         (0) root         (0)     6102 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/algorithm/weight_correction.py
--rw-r--r--   0 root         (0) root         (0)    22341 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/benchmark.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.678342 neural_compressor-2.5/neural_compressor/compression/
--rw-r--r--   0 root         (0) root         (0)      731 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/compression/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19814 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/compression/callbacks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.679342 neural_compressor-2.5/neural_compressor/compression/distillation/
--rw-r--r--   0 root         (0) root         (0)      658 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/compression/distillation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    67415 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/compression/distillation/criterions.py
--rw-r--r--   0 root         (0) root         (0)     7604 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/compression/distillation/optimizers.py
--rw-r--r--   0 root         (0) root         (0)     2207 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/compression/distillation/utility.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.679342 neural_compressor-2.5/neural_compressor/compression/hpo/
--rw-r--r--   0 root         (0) root         (0)      758 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/compression/hpo/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4293 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/compression/hpo/sa_optimizer.py
--rw-r--r--   0 root         (0) root         (0)    12510 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/compression/hpo/search_algorithms.py
--rw-r--r--   0 root         (0) root         (0)     5809 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/compression/hpo/search_space.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.681342 neural_compressor-2.5/neural_compressor/compression/pruner/
--rw-r--r--   0 root         (0) root         (0)     8050 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/compression/pruner/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13557 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/compression/pruner/criteria.py
--rw-r--r--   0 root         (0) root         (0)    13722 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/compression/pruner/dsnot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.681342 neural_compressor-2.5/neural_compressor/compression/pruner/model_slim/
--rw-r--r--   0 root         (0) root         (0)      750 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/compression/pruner/model_slim/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4999 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/compression/pruner/model_slim/auto_slim.py
--rw-r--r--   0 root         (0) root         (0)    35992 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/compression/pruner/model_slim/pattern_analyzer.py
--rw-r--r--   0 root         (0) root         (0)    17780 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/compression/pruner/model_slim/weight_slim.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.682342 neural_compressor-2.5/neural_compressor/compression/pruner/patterns/
--rw-r--r--   0 root         (0) root         (0)     2043 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/compression/pruner/patterns/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30952 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/compression/pruner/patterns/base.py
--rw-r--r--   0 root         (0) root         (0)     2269 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/compression/pruner/patterns/mha.py
--rw-r--r--   0 root         (0) root         (0)    19320 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/compression/pruner/patterns/ninm.py
--rw-r--r--   0 root         (0) root         (0)    35816 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/compression/pruner/patterns/nxm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.683342 neural_compressor-2.5/neural_compressor/compression/pruner/pruners/
--rw-r--r--   0 root         (0) root         (0)     3318 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/compression/pruner/pruners/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10453 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/compression/pruner/pruners/base.py
--rw-r--r--   0 root         (0) root         (0)     8602 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/compression/pruner/pruners/basic.py
--rw-r--r--   0 root         (0) root         (0)     6709 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/compression/pruner/pruners/block_mask.py
--rw-r--r--   0 root         (0) root         (0)    11925 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/compression/pruner/pruners/mha.py
--rw-r--r--   0 root         (0) root         (0)     2159 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/compression/pruner/pruners/pattern_lock.py
--rw-r--r--   0 root         (0) root         (0)    14028 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/compression/pruner/pruners/progressive.py
--rw-r--r--   0 root         (0) root         (0)     8627 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/compression/pruner/pruners/retrain_free.py
--rw-r--r--   0 root         (0) root         (0)     4492 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/compression/pruner/pruners/sparse_gpt.py
--rw-r--r--   0 root         (0) root         (0)    11500 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/compression/pruner/pruning.py
--rw-r--r--   0 root         (0) root         (0)     5080 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/compression/pruner/regs.py
--rw-r--r--   0 root         (0) root         (0)     6258 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/compression/pruner/schedulers.py
--rw-r--r--   0 root         (0) root         (0)     3170 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/compression/pruner/tf_criteria.py
--rw-r--r--   0 root         (0) root         (0)    30386 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/compression/pruner/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.684342 neural_compressor-2.5/neural_compressor/compression/pruner/wanda/
--rw-r--r--   0 root         (0) root         (0)      683 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/compression/pruner/wanda/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9216 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/compression/pruner/wanda/prune.py
--rw-r--r--   0 root         (0) root         (0)     2105 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/compression/pruner/wanda/utils.py
--rw-r--r--   0 root         (0) root         (0)     2744 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/compression/pruner/wanda/wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.684342 neural_compressor-2.5/neural_compressor/conf/
--rw-r--r--   0 root         (0) root         (0)      631 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/conf/__init__.py
--rw-r--r--   0 root         (0) root         (0)    73546 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/conf/config.py
--rw-r--r--   0 root         (0) root         (0)     2980 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/conf/dotdict.py
--rw-r--r--   0 root         (0) root         (0)    52365 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/conf/pythonic_config.py
--rw-r--r--   0 root         (0) root         (0)    96109 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.685342 neural_compressor-2.5/neural_compressor/contrib/
--rw-r--r--   0 root         (0) root         (0)      712 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/contrib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.685342 neural_compressor-2.5/neural_compressor/contrib/strategy/
--rw-r--r--   0 root         (0) root         (0)      971 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/contrib/strategy/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15560 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/contrib/strategy/sigopt.py
--rw-r--r--   0 root         (0) root         (0)    25177 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/contrib/strategy/tpe.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.685342 neural_compressor-2.5/neural_compressor/data/
--rw-r--r--   0 root         (0) root         (0)     2483 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.686342 neural_compressor-2.5/neural_compressor/data/dataloaders/
--rw-r--r--   0 root         (0) root         (0)      802 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/data/dataloaders/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4978 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/data/dataloaders/base_dataloader.py
--rw-r--r--   0 root         (0) root         (0)     5995 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/data/dataloaders/dataloader.py
--rw-r--r--   0 root         (0) root         (0)     6267 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/data/dataloaders/default_dataloader.py
--rw-r--r--   0 root         (0) root         (0)     4931 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/data/dataloaders/fetcher.py
--rw-r--r--   0 root         (0) root         (0)     1745 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/data/dataloaders/mxnet_dataloader.py
--rw-r--r--   0 root         (0) root         (0)     3770 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/data/dataloaders/onnxrt_dataloader.py
--rw-r--r--   0 root         (0) root         (0)     2585 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/data/dataloaders/pytorch_dataloader.py
--rw-r--r--   0 root         (0) root         (0)     5117 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/data/dataloaders/sampler.py
--rw-r--r--   0 root         (0) root         (0)    15359 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/data/dataloaders/tensorflow_dataloader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.688342 neural_compressor-2.5/neural_compressor/data/datasets/
--rw-r--r--   0 root         (0) root         (0)     1240 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/data/datasets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19357 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/data/datasets/bert_dataset.py
--rw-r--r--   0 root         (0) root         (0)    12572 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/data/datasets/coco_dataset.py
--rw-r--r--   0 root         (0) root         (0)    42400 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/data/datasets/dataset.py
--rw-r--r--   0 root         (0) root         (0)     6680 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/data/datasets/dummy_dataset.py
--rw-r--r--   0 root         (0) root         (0)    13357 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/data/datasets/dummy_dataset_v2.py
--rw-r--r--   0 root         (0) root         (0)     9362 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/data/datasets/imagenet_dataset.py
--rw-r--r--   0 root         (0) root         (0)     3672 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/data/datasets/style_transfer_dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.688342 neural_compressor-2.5/neural_compressor/data/filters/
--rw-r--r--   0 root         (0) root         (0)     1130 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/data/filters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1935 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/data/filters/coco_filter.py
--rw-r--r--   0 root         (0) root         (0)     5858 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/data/filters/filter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.689342 neural_compressor-2.5/neural_compressor/data/transforms/
--rw-r--r--   0 root         (0) root         (0)     2079 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/data/transforms/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2023 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/data/transforms/coco_transform.py
--rw-r--r--   0 root         (0) root         (0)    18418 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/data/transforms/imagenet_transform.py
--rw-r--r--   0 root         (0) root         (0)     1002 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/data/transforms/postprocess.py
--rw-r--r--   0 root         (0) root         (0)    12107 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/data/transforms/tokenization.py
--rw-r--r--   0 root         (0) root         (0)   105024 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/data/transforms/transform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.691342 neural_compressor-2.5/neural_compressor/experimental/
--rw-r--r--   0 root         (0) root         (0)     1367 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30418 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/benchmark.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.692342 neural_compressor-2.5/neural_compressor/experimental/common/
--rw-r--r--   0 root         (0) root         (0)     1033 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)    47431 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/common/criterion.py
--rw-r--r--   0 root         (0) root         (0)     5261 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/common/dataloader.py
--rw-r--r--   0 root         (0) root         (0)     1583 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/common/metric.py
--rw-r--r--   0 root         (0) root         (0)     2728 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/common/model.py
--rw-r--r--   0 root         (0) root         (0)     6799 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/common/optimizer.py
--rw-r--r--   0 root         (0) root         (0)     1063 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/common/postprocess.py
--rw-r--r--   0 root         (0) root         (0)     2295 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/common/torch_utils.py
--rw-r--r--   0 root         (0) root         (0)    24785 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/component.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.692342 neural_compressor-2.5/neural_compressor/experimental/compression/
--rw-r--r--   0 root         (0) root         (0)      664 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/compression/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.692342 neural_compressor-2.5/neural_compressor/experimental/contrib/
--rw-r--r--   0 root         (0) root         (0)      712 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/contrib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.692342 neural_compressor-2.5/neural_compressor/experimental/contrib/strategy/
--rw-r--r--   0 root         (0) root         (0)      970 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/contrib/strategy/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14083 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/contrib/strategy/sigopt.py
--rw-r--r--   0 root         (0) root         (0)    25050 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/contrib/strategy/tpe.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.693342 neural_compressor-2.5/neural_compressor/experimental/data/
--rw-r--r--   0 root         (0) root         (0)     1270 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.694342 neural_compressor-2.5/neural_compressor/experimental/data/dataloaders/
--rw-r--r--   0 root         (0) root         (0)      836 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/data/dataloaders/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5020 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/data/dataloaders/base_dataloader.py
--rw-r--r--   0 root         (0) root         (0)     1410 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/data/dataloaders/dataloader.py
--rw-r--r--   0 root         (0) root         (0)     6284 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/data/dataloaders/default_dataloader.py
--rw-r--r--   0 root         (0) root         (0)     4987 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/data/dataloaders/fetcher.py
--rw-r--r--   0 root         (0) root         (0)     1787 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/data/dataloaders/mxnet_dataloader.py
--rw-r--r--   0 root         (0) root         (0)     3819 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/data/dataloaders/onnxrt_dataloader.py
--rw-r--r--   0 root         (0) root         (0)     2606 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/data/dataloaders/pytorch_dataloader.py
--rw-r--r--   0 root         (0) root         (0)     5180 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/data/dataloaders/sampler.py
--rw-r--r--   0 root         (0) root         (0)    15349 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/data/dataloaders/tensorflow_dataloader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.695342 neural_compressor-2.5/neural_compressor/experimental/data/datasets/
--rw-r--r--   0 root         (0) root         (0)     1127 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/data/datasets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19191 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/data/datasets/bert_dataset.py
--rw-r--r--   0 root         (0) root         (0)    12492 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/data/datasets/coco_dataset.py
--rw-r--r--   0 root         (0) root         (0)    41844 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/data/datasets/dataset.py
--rw-r--r--   0 root         (0) root         (0)     6660 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/data/datasets/dummy_dataset.py
--rw-r--r--   0 root         (0) root         (0)    13317 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/data/datasets/dummy_dataset_v2.py
--rw-r--r--   0 root         (0) root         (0)     9242 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/data/datasets/imagenet_dataset.py
--rw-r--r--   0 root         (0) root         (0)     3652 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/data/datasets/style_transfer_dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.696342 neural_compressor-2.5/neural_compressor/experimental/data/filters/
--rw-r--r--   0 root         (0) root         (0)     1044 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/data/filters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1895 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/data/filters/coco_filter.py
--rw-r--r--   0 root         (0) root         (0)     5697 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/data/filters/filter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.696342 neural_compressor-2.5/neural_compressor/experimental/data/transforms/
--rw-r--r--   0 root         (0) root         (0)     1208 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/data/transforms/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17438 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/data/transforms/imagenet_transform.py
--rw-r--r--   0 root         (0) root         (0)    12107 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/data/transforms/tokenization.py
--rw-r--r--   0 root         (0) root         (0)   105074 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/data/transforms/transform.py
--rw-r--r--   0 root         (0) root         (0)    21663 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/distillation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.697342 neural_compressor-2.5/neural_compressor/experimental/export/
--rw-r--r--   0 root         (0) root         (0)      832 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/export/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3089 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/export/qlinear2qdq.py
--rw-r--r--   0 root         (0) root         (0)     4806 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/export/tf2onnx.py
--rw-r--r--   0 root         (0) root         (0)    16037 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/export/torch2onnx.py
--rw-r--r--   0 root         (0) root         (0)    20023 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/graph_optimization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.698342 neural_compressor-2.5/neural_compressor/experimental/metric/
--rw-r--r--   0 root         (0) root         (0)     1067 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/metric/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4977 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/metric/bleu.py
--rw-r--r--   0 root         (0) root         (0)     5146 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/metric/bleu_util.py
--rw-r--r--   0 root         (0) root         (0)     2188 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/metric/coco_label_map.py
--rw-r--r--   0 root         (0) root         (0)    31804 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/metric/coco_tools.py
--rw-r--r--   0 root         (0) root         (0)     4358 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/metric/evaluate_squad.py
--rw-r--r--   0 root         (0) root         (0)     5323 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/metric/f1.py
--rw-r--r--   0 root         (0) root         (0)    57242 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/metric/metric.py
--rw-r--r--   0 root         (0) root         (0)    10161 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/mixed_precision.py
--rw-r--r--   0 root         (0) root         (0)    15510 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/model_conversion.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.699343 neural_compressor-2.5/neural_compressor/experimental/nas/
--rw-r--r--   0 root         (0) root         (0)      729 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/nas/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5755 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/nas/basic_nas.py
--rw-r--r--   0 root         (0) root         (0)     4237 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/nas/dynas.py
--rw-r--r--   0 root         (0) root         (0)    15265 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/nas/nas.py
--rw-r--r--   0 root         (0) root         (0)     2913 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/nas/nas_utils.py
--rw-r--r--   0 root         (0) root         (0)     6010 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/nas/search_algorithms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.700343 neural_compressor-2.5/neural_compressor/experimental/pruner_legacy/
--rw-r--r--   0 root         (0) root         (0)      994 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/pruner_legacy/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11431 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/pruner_legacy/gradient_sensitivity.py
--rw-r--r--   0 root         (0) root         (0)     2740 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/pruner_legacy/group_lasso.py
--rw-r--r--   0 root         (0) root         (0)     4579 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/pruner_legacy/magnitude.py
--rw-r--r--   0 root         (0) root         (0)     2219 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/pruner_legacy/pattern_lock.py
--rw-r--r--   0 root         (0) root         (0)     4795 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/pruner_legacy/pruner.py
--rw-r--r--   0 root         (0) root         (0)    21661 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/pruning.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.700343 neural_compressor-2.5/neural_compressor/experimental/pruning_recipes/
--rw-r--r--   0 root         (0) root         (0)      738 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/pruning_recipes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.700343 neural_compressor-2.5/neural_compressor/experimental/pruning_recipes/patterns/
--rw-r--r--   0 root         (0) root         (0)     1018 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/pruning_recipes/patterns/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3799 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/pruning_recipes/patterns/pattern.py
--rw-r--r--   0 root         (0) root         (0)     3006 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/pruning_recipes/patterns/tile_pattern.py
--rw-r--r--   0 root         (0) root         (0)    22247 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/pruning_v2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.701343 neural_compressor-2.5/neural_compressor/experimental/pytorch_pruner/
--rw-r--r--   0 root         (0) root         (0)      661 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/pytorch_pruner/__init__.py
--rw-r--r--   0 root         (0) root         (0)      682 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/pytorch_pruner/logger.py
--rw-r--r--   0 root         (0) root         (0)    25049 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/pytorch_pruner/patterns.py
--rw-r--r--   0 root         (0) root         (0)     9243 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/pytorch_pruner/prune_utils.py
--rw-r--r--   0 root         (0) root         (0)    12507 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/pytorch_pruner/pruner.py
--rw-r--r--   0 root         (0) root         (0)     6414 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/pytorch_pruner/pruning.py
--rw-r--r--   0 root         (0) root         (0)     5554 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/pytorch_pruner/scheduler.py
--rw-r--r--   0 root         (0) root         (0)    22801 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/quantization.py
--rw-r--r--   0 root         (0) root         (0)    18339 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.702343 neural_compressor-2.5/neural_compressor/experimental/strategy/
--rw-r--r--   0 root         (0) root         (0)     1022 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/strategy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7684 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/strategy/auto_mixed_precision.py
--rw-r--r--   0 root         (0) root         (0)     9809 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/strategy/basic.py
--rw-r--r--   0 root         (0) root         (0)    15351 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/strategy/bayesian.py
--rw-r--r--   0 root         (0) root         (0)     2156 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/strategy/exhaustive.py
--rw-r--r--   0 root         (0) root         (0)    10626 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/strategy/mse.py
--rw-r--r--   0 root         (0) root         (0)    11339 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/strategy/mse_v2.py
--rw-r--r--   0 root         (0) root         (0)     2508 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/strategy/random.py
--rw-r--r--   0 root         (0) root         (0)    65514 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/strategy/strategy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.703343 neural_compressor-2.5/neural_compressor/experimental/strategy/utils/
--rw-r--r--   0 root         (0) root         (0)      905 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/strategy/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1393 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/strategy/utils/constant.py
--rw-r--r--   0 root         (0) root         (0)    22145 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/strategy/utils/tuning_sampler.py
--rw-r--r--   0 root         (0) root         (0)    30511 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/strategy/utils/tuning_space.py
--rw-r--r--   0 root         (0) root         (0)     3836 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/strategy/utils/tuning_structs.py
--rw-r--r--   0 root         (0) root         (0)     1903 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/experimental/strategy/utils/utility.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.704343 neural_compressor-2.5/neural_compressor/metric/
--rw-r--r--   0 root         (0) root         (0)     1325 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/metric/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4862 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/metric/bleu.py
--rw-r--r--   0 root         (0) root         (0)     5058 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/metric/bleu_util.py
--rw-r--r--   0 root         (0) root         (0)     2188 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/metric/coco_label_map.py
--rw-r--r--   0 root         (0) root         (0)    31581 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/metric/coco_tools.py
--rw-r--r--   0 root         (0) root         (0)     4215 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/metric/evaluate_squad.py
--rw-r--r--   0 root         (0) root         (0)     5234 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/metric/f1.py
--rw-r--r--   0 root         (0) root         (0)    59780 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/metric/metric.py
--rw-r--r--   0 root         (0) root         (0)     8282 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/mix_precision.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.706343 neural_compressor-2.5/neural_compressor/model/
--rw-r--r--   0 root         (0) root         (0)      797 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2095 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/model/base_model.py
--rw-r--r--   0 root         (0) root         (0)     4376 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/model/keras_model.py
--rw-r--r--   0 root         (0) root         (0)    11417 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/model/model.py
--rw-r--r--   0 root         (0) root         (0)     2471 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/model/mxnet_model.py
--rw-r--r--   0 root         (0) root         (0)     5879 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/model/nets_factory.py
--rw-r--r--   0 root         (0) root         (0)    50294 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/model/onnx_model.py
--rw-r--r--   0 root         (0) root         (0)    58843 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/model/tensorflow_model.py
--rw-r--r--   0 root         (0) root         (0)    26177 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/model/torch_model.py
--rw-r--r--   0 root         (0) root         (0)    21840 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/objective.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.706343 neural_compressor-2.5/neural_compressor/profiling/
--rw-r--r--   0 root         (0) root         (0)      663 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/profiling/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.706343 neural_compressor-2.5/neural_compressor/profiling/parser/
--rw-r--r--   0 root         (0) root         (0)      621 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/profiling/parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1766 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/profiling/parser/factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.707343 neural_compressor-2.5/neural_compressor/profiling/parser/onnx_parser/
--rw-r--r--   0 root         (0) root         (0)      621 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/profiling/parser/onnx_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1295 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/profiling/parser/onnx_parser/factory.py
--rw-r--r--   0 root         (0) root         (0)     2943 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/profiling/parser/onnx_parser/parser.py
--rw-r--r--   0 root         (0) root         (0)     2202 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/profiling/parser/parser.py
--rw-r--r--   0 root         (0) root         (0)     2198 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/profiling/parser/result.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.707343 neural_compressor-2.5/neural_compressor/profiling/parser/tensorflow_parser/
--rw-r--r--   0 root         (0) root         (0)      621 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/profiling/parser/tensorflow_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1329 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/profiling/parser/tensorflow_parser/factory.py
--rw-r--r--   0 root         (0) root         (0)     4346 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/profiling/parser/tensorflow_parser/parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.708343 neural_compressor-2.5/neural_compressor/profiling/profiler/
--rw-r--r--   0 root         (0) root         (0)      621 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/profiling/profiler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2076 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/profiling/profiler/factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.708343 neural_compressor-2.5/neural_compressor/profiling/profiler/onnxrt_profiler/
--rw-r--r--   0 root         (0) root         (0)      621 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/profiling/profiler/onnxrt_profiler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1525 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/profiling/profiler/onnxrt_profiler/factory.py
--rw-r--r--   0 root         (0) root         (0)     3310 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/profiling/profiler/onnxrt_profiler/profiler.py
--rw-r--r--   0 root         (0) root         (0)     1284 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/profiling/profiler/onnxrt_profiler/utils.py
--rw-r--r--   0 root         (0) root         (0)     1052 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/profiling/profiler/profiler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.709343 neural_compressor-2.5/neural_compressor/profiling/profiler/tensorflow_profiler/
--rw-r--r--   0 root         (0) root         (0)      621 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/profiling/profiler/tensorflow_profiler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1945 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/profiling/profiler/tensorflow_profiler/factory.py
--rw-r--r--   0 root         (0) root         (0)     5417 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/profiling/profiler/tensorflow_profiler/profiler.py
--rw-r--r--   0 root         (0) root         (0)     2682 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/profiling/profiler/tensorflow_profiler/utils.py
--rw-r--r--   0 root         (0) root         (0)    12315 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/quantization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.710343 neural_compressor-2.5/neural_compressor/strategy/
--rw-r--r--   0 root         (0) root         (0)     1014 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/strategy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6214 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/strategy/auto.py
--rw-r--r--   0 root         (0) root         (0)    11697 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/strategy/auto_mixed_precision.py
--rw-r--r--   0 root         (0) root         (0)    22059 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/strategy/basic.py
--rw-r--r--   0 root         (0) root         (0)    16611 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/strategy/bayesian.py
--rw-r--r--   0 root         (0) root         (0)    11127 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/strategy/conservative.py
--rw-r--r--   0 root         (0) root         (0)     2079 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/strategy/exhaustive.py
--rw-r--r--   0 root         (0) root         (0)     5584 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/strategy/hawq_v2.py
--rw-r--r--   0 root         (0) root         (0)    11845 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/strategy/mse.py
--rw-r--r--   0 root         (0) root         (0)    10617 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/strategy/mse_v2.py
--rw-r--r--   0 root         (0) root         (0)     2348 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/strategy/random.py
--rw-r--r--   0 root         (0) root         (0)   101604 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/strategy/strategy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.711343 neural_compressor-2.5/neural_compressor/strategy/utils/
--rw-r--r--   0 root         (0) root         (0)      905 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/strategy/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2243 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/strategy/utils/constant.py
--rw-r--r--   0 root         (0) root         (0)    28718 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/strategy/utils/tuning_sampler.py
--rw-r--r--   0 root         (0) root         (0)    32978 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/strategy/utils/tuning_space.py
--rw-r--r--   0 root         (0) root         (0)     4130 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/strategy/utils/tuning_structs.py
--rw-r--r--   0 root         (0) root         (0)     4676 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/strategy/utils/utility.py
--rw-r--r--   0 root         (0) root         (0)    21463 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/training.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.713343 neural_compressor-2.5/neural_compressor/utils/
--rw-r--r--   0 root         (0) root         (0)     1057 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2783 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/utils/collect_layer_histogram.py
--rw-r--r--   0 root         (0) root         (0)     2917 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/utils/constant.py
--rw-r--r--   0 root         (0) root         (0)     9390 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/utils/create_obj_from_config.py
--rw-r--r--   0 root         (0) root         (0)     5751 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/utils/kl_divergence.py
--rw-r--r--   0 root         (0) root         (0)    15257 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/utils/load_huggingface.py
--rw-r--r--   0 root         (0) root         (0)     4594 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/utils/logger.py
--rw-r--r--   0 root         (0) root         (0)     6117 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/utils/neural_insights_utils.py
--rw-r--r--   0 root         (0) root         (0)     1231 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/utils/options.py
--rw-r--r--   0 root         (0) root         (0)    23214 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/utils/pytorch.py
--rw-r--r--   0 root         (0) root         (0)    36312 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/utils/utility.py
--rw-r--r--   0 root         (0) root         (0)     2640 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/utils/weights_details.py
--rw-r--r--   0 root         (0) root         (0)      763 2024-03-26 08:53:13.000000 neural_compressor-2.5/neural_compressor/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:01:08.713343 neural_compressor-2.5/neural_compressor.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15587 2024-03-26 09:01:08.000000 neural_compressor-2.5/neural_compressor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    29656 2024-03-26 09:01:08.000000 neural_compressor-2.5/neural_compressor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-26 09:01:08.000000 neural_compressor-2.5/neural_compressor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      381 2024-03-26 09:01:08.000000 neural_compressor-2.5/neural_compressor.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-03-26 09:01:08.000000 neural_compressor-2.5/neural_compressor.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2418 2024-03-26 08:53:14.000000 neural_compressor-2.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      102 2024-03-26 09:01:08.714343 neural_compressor-2.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     8675 2024-03-26 08:53:14.000000 neural_compressor-2.5/setup.py
--rw-r--r--   0 root         (0) root         (0)    95740 2024-03-26 08:53:14.000000 neural_compressor-2.5/third-party-programs.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.254005 neural_compressor-2.5.1/
+-rw-r--r--   0 root         (0) root         (0)    11360 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    15595 2024-04-03 13:33:46.254005 neural_compressor-2.5.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14096 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.176002 neural_compressor-2.5.1/neural_coder/
+-rw-r--r--   0 root         (0) root         (0)      749 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      668 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.184002 neural_compressor-2.5.1/neural_coder/backends/
+-rw-r--r--   0 root         (0) root         (0)      583 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1382 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/intel_extension_for_transformers.yaml
+-rw-r--r--   0 root         (0) root         (0)     1121 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/keras_inc.yaml
+-rw-r--r--   0 root         (0) root         (0)     1039 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/nano_bf16.yaml
+-rw-r--r--   0 root         (0) root         (0)     1059 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/nano_bf16_channels_last.yaml
+-rw-r--r--   0 root         (0) root         (0)     1054 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/nano_bf16_ipex.yaml
+-rw-r--r--   0 root         (0) root         (0)     1074 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/nano_bf16_ipex_channels_last.yaml
+-rw-r--r--   0 root         (0) root         (0)     1038 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/nano_fp32_channels_last.yaml
+-rw-r--r--   0 root         (0) root         (0)     1033 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/nano_fp32_ipex.yaml
+-rw-r--r--   0 root         (0) root         (0)     1053 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/nano_fp32_ipex_channels_last.yaml
+-rw-r--r--   0 root         (0) root         (0)      850 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/nano_gpu_to_cpu.yaml
+-rw-r--r--   0 root         (0) root         (0)     1039 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/nano_int8.yaml
+-rw-r--r--   0 root         (0) root         (0)     1058 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/nano_jit_bf16.yaml
+-rw-r--r--   0 root         (0) root         (0)     1078 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/nano_jit_bf16_channels_last.yaml
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/nano_jit_bf16_ipex.yaml
+-rw-r--r--   0 root         (0) root         (0)     1093 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/nano_jit_bf16_ipex_channels_last.yaml
+-rw-r--r--   0 root         (0) root         (0)     1038 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/nano_jit_fp32.yaml
+-rw-r--r--   0 root         (0) root         (0)     1057 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/nano_jit_fp32_channels_last.yaml
+-rw-r--r--   0 root         (0) root         (0)     1053 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/nano_jit_fp32_ipex.yaml
+-rw-r--r--   0 root         (0) root         (0)     1072 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/nano_jit_fp32_ipex_channels_last.yaml
+-rw-r--r--   0 root         (0) root         (0)     1045 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/nano_onnxruntime_fp32.yaml
+-rw-r--r--   0 root         (0) root         (0)     1066 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/nano_onnxruntime_int8_qlinear.yaml
+-rw-r--r--   0 root         (0) root         (0)     1042 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/nano_openvino_fp32.yaml
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/nano_openvino_int8.yaml
+-rw-r--r--   0 root         (0) root         (0)     1082 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/onnx_inc_dynamic_quant.yaml
+-rw-r--r--   0 root         (0) root         (0)     1082 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/onnx_inc_static_quant_qdq.yaml
+-rw-r--r--   0 root         (0) root         (0)     1086 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/onnx_inc_static_quant_qlinear.yaml
+-rw-r--r--   0 root         (0) root         (0)      923 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/pytorch_aliblade.yaml
+-rw-r--r--   0 root         (0) root         (0)     2655 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/pytorch_benchmark.yaml
+-rw-r--r--   0 root         (0) root         (0)     1246 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/pytorch_channels_last.yaml
+-rw-r--r--   0 root         (0) root         (0)     1380 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/pytorch_inc_bf16.yaml
+-rw-r--r--   0 root         (0) root         (0)     1651 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/pytorch_inc_dynamic_quant.yaml
+-rw-r--r--   0 root         (0) root         (0)     1761 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/pytorch_inc_dynamic_quant_fp8.yaml
+-rw-r--r--   0 root         (0) root         (0)     1515 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/pytorch_inc_huggingface_optimum_dynamic.yaml
+-rw-r--r--   0 root         (0) root         (0)     1548 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/pytorch_inc_huggingface_optimum_static.yaml
+-rw-r--r--   0 root         (0) root         (0)     1713 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/pytorch_inc_static_quant_fx.yaml
+-rw-r--r--   0 root         (0) root         (0)     1740 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/pytorch_inc_static_quant_fx_fp8.yaml
+-rw-r--r--   0 root         (0) root         (0)     1274 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/pytorch_inc_static_quant_ipex.yaml
+-rw-r--r--   0 root         (0) root         (0)     1332 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/pytorch_inc_static_quant_ipex_xpu.yaml
+-rw-r--r--   0 root         (0) root         (0)     1306 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/pytorch_ipex_bf16.yaml
+-rw-r--r--   0 root         (0) root         (0)     1076 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/pytorch_ipex_fp32.yaml
+-rw-r--r--   0 root         (0) root         (0)     1540 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/pytorch_ipex_int8_dynamic_quant.yaml
+-rw-r--r--   0 root         (0) root         (0)     1539 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/pytorch_ipex_int8_static_quant.yaml
+-rw-r--r--   0 root         (0) root         (0)     1261 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/pytorch_jit_script.yaml
+-rw-r--r--   0 root         (0) root         (0)     1235 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/pytorch_jit_script_ofi.yaml
+-rw-r--r--   0 root         (0) root         (0)     1347 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/pytorch_jit_trace.yaml
+-rw-r--r--   0 root         (0) root         (0)     1321 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/pytorch_jit_trace_ofi.yaml
+-rw-r--r--   0 root         (0) root         (0)      861 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/pytorch_mixed_precision_cpu.yaml
+-rw-r--r--   0 root         (0) root         (0)      861 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/pytorch_mixed_precision_cuda.yaml
+-rw-r--r--   0 root         (0) root         (0)      843 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/pytorch_mixed_precision_intel_gpu.yaml
+-rw-r--r--   0 root         (0) root         (0)     1201 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/pytorch_torchdynamo_jit_script.yaml
+-rw-r--r--   0 root         (0) root         (0)     1235 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/pytorch_torchdynamo_jit_script_ofi.yaml
+-rw-r--r--   0 root         (0) root         (0)     1216 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/pytorch_torchdynamo_jit_trace.yaml
+-rw-r--r--   0 root         (0) root         (0)     1250 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/pytorch_torchdynamo_jit_trace_ofi.yaml
+-rw-r--r--   0 root         (0) root         (0)     1118 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/backends/template.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.184002 neural_compressor-2.5.1/neural_coder/coders/
+-rw-r--r--   0 root         (0) root         (0)      583 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/coders/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.185002 neural_compressor-2.5.1/neural_coder/coders/autoinc/
+-rw-r--r--   0 root         (0) root         (0)      583 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/coders/autoinc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26608 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/coders/autoinc/autoinc_harness.py
+-rw-r--r--   0 root         (0) root         (0)     1752 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/coders/autoinc/calib_dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     1337 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/coders/autoinc/domain.py
+-rw-r--r--   0 root         (0) root         (0)     4768 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/coders/autoinc/eval_func.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.186002 neural_compressor-2.5.1/neural_coder/coders/pytorch/
+-rw-r--r--   0 root         (0) root         (0)      583 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/coders/pytorch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3192 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/coders/pytorch/batch_size.py
+-rw-r--r--   0 root         (0) root         (0)     1460 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/coders/pytorch/change_trainer_to_nlptrainer.py
+-rw-r--r--   0 root         (0) root         (0)     2941 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/coders/pytorch/cuda_to_cpu.py
+-rw-r--r--   0 root         (0) root         (0)     6779 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/coders/pytorch/dummy_dataloader.py
+-rw-r--r--   0 root         (0) root         (0)    23456 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/coders/pytorch/harness.py
+-rw-r--r--   0 root         (0) root         (0)     2873 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/coders/pytorch/lightning.py
+-rw-r--r--   0 root         (0) root         (0)     3616 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/coders/pytorch/reclaim_inference_transformers_trainer.py
+-rw-r--r--   0 root         (0) root         (0)     5205 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/coders/pytorch/reclaim_inputs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.186002 neural_compressor-2.5.1/neural_coder/coders/tensorflow/
+-rw-r--r--   0 root         (0) root         (0)      583 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/coders/tensorflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2728 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/coders/tensorflow/amp.py
+-rw-r--r--   0 root         (0) root         (0)     2173 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/coders/tensorflow/inc.py
+-rw-r--r--   0 root         (0) root         (0)     3623 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/coders/transform.py
+-rw-r--r--   0 root         (0) root         (0)     3403 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/globals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.187002 neural_compressor-2.5.1/neural_coder/graphers/
+-rw-r--r--   0 root         (0) root         (0)      583 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/graphers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11141 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/graphers/code_line.py
+-rw-r--r--   0 root         (0) root         (0)     7143 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/graphers/function.py
+-rw-r--r--   0 root         (0) root         (0)    12609 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/graphers/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.187002 neural_compressor-2.5.1/neural_coder/graphers/preloads/
+-rw-r--r--   0 root         (0) root         (0)      583 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/graphers/preloads/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58209 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/graphers/preloads/transformers.yaml
+-rw-r--r--   0 root         (0) root         (0)    53298 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/interface.py
+-rw-r--r--   0 root         (0) root         (0)     3707 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/launcher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.188002 neural_compressor-2.5.1/neural_coder/utils/
+-rw-r--r--   0 root         (0) root         (0)      583 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      902 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/utils/common.py
+-rw-r--r--   0 root         (0) root         (0)     1746 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/utils/cpu_info.py
+-rw-r--r--   0 root         (0) root         (0)     3014 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/utils/device.py
+-rw-r--r--   0 root         (0) root         (0)     7500 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/utils/handle_user_input.py
+-rw-r--r--   0 root         (0) root         (0)     5138 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/utils/line_operation.py
+-rw-r--r--   0 root         (0) root         (0)    38116 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/utils/numa_launcher.py
+-rw-r--r--   0 root         (0) root         (0)    18657 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/utils/pdf_report.py
+-rw-r--r--   0 root         (0) root         (0)      604 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_coder/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.189002 neural_compressor-2.5.1/neural_compressor/
+-rw-r--r--   0 root         (0) root         (0)     1190 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.193003 neural_compressor-2.5.1/neural_compressor/adaptor/
+-rw-r--r--   0 root         (0) root         (0)      973 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7481 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/adaptor.py
+-rw-r--r--   0 root         (0) root         (0)    45327 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/keras.py
+-rw-r--r--   0 root         (0) root         (0)     5590 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/keras.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.194003 neural_compressor-2.5.1/neural_compressor/adaptor/keras_utils/
+-rw-r--r--   0 root         (0) root         (0)      631 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/keras_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3576 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/keras_utils/conv2d.py
+-rw-r--r--   0 root         (0) root         (0)     2568 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/keras_utils/dense.py
+-rw-r--r--   0 root         (0) root         (0)     4710 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/keras_utils/depthwise_conv2d.py
+-rw-r--r--   0 root         (0) root         (0)     1841 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/keras_utils/pool2d.py
+-rw-r--r--   0 root         (0) root         (0)     4079 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/keras_utils/quantizer.py
+-rw-r--r--   0 root         (0) root         (0)     4466 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/keras_utils/separable_conv2d.py
+-rw-r--r--   0 root         (0) root         (0)    21979 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/mxnet.py
+-rw-r--r--   0 root         (0) root         (0)    10616 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/mxnet.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.194003 neural_compressor-2.5.1/neural_compressor/adaptor/mxnet_utils/
+-rw-r--r--   0 root         (0) root         (0)      655 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/mxnet_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30686 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/mxnet_utils/util.py
+-rw-r--r--   0 root         (0) root         (0)   105870 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/onnxrt.py
+-rw-r--r--   0 root         (0) root         (0)    20205 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/onnxrt.yaml
+-rw-r--r--   0 root         (0) root         (0)    16912 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/onnxrt_cuda.yaml
+-rw-r--r--   0 root         (0) root         (0)     2441 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/onnxrt_dml.yaml
+-rw-r--r--   0 root         (0) root         (0)    15046 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/onnxrt_dnnl.yaml
+-rw-r--r--   0 root         (0) root         (0)     4873 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/onnxrt_trt.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.196003 neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/
+-rw-r--r--   0 root         (0) root         (0)      656 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42456 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/calibration.py
+-rw-r--r--   0 root         (0) root         (0)    15292 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/calibrator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.199003 neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/operators/
+-rw-r--r--   0 root         (0) root         (0)     1026 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5348 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/operators/activation.py
+-rw-r--r--   0 root         (0) root         (0)     1791 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/operators/argmax.py
+-rw-r--r--   0 root         (0) root         (0)     4626 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/operators/attention.py
+-rw-r--r--   0 root         (0) root         (0)     7462 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/operators/binary_op.py
+-rw-r--r--   0 root         (0) root         (0)     7210 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/operators/concat.py
+-rw-r--r--   0 root         (0) root         (0)    10211 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/operators/conv.py
+-rw-r--r--   0 root         (0) root         (0)     3758 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/operators/direct_q8.py
+-rw-r--r--   0 root         (0) root         (0)     4288 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/operators/embed_layernorm.py
+-rw-r--r--   0 root         (0) root         (0)     5369 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/operators/gather.py
+-rw-r--r--   0 root         (0) root         (0)     3500 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/operators/gavgpool.py
+-rw-r--r--   0 root         (0) root         (0)     6410 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/operators/gemm.py
+-rw-r--r--   0 root         (0) root         (0)     5627 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/operators/lstm.py
+-rw-r--r--   0 root         (0) root         (0)     8323 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/operators/matmul.py
+-rw-r--r--   0 root         (0) root         (0)     3293 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/operators/maxpool.py
+-rw-r--r--   0 root         (0) root         (0)     1722 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/operators/norm.py
+-rw-r--r--   0 root         (0) root         (0)     5767 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/operators/ops.py
+-rw-r--r--   0 root         (0) root         (0)     4868 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/operators/pad.py
+-rw-r--r--   0 root         (0) root         (0)     4513 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/operators/pooling.py
+-rw-r--r--   0 root         (0) root         (0)     3375 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/operators/reduce.py
+-rw-r--r--   0 root         (0) root         (0)     3412 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/operators/resize.py
+-rw-r--r--   0 root         (0) root         (0)     6181 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/operators/split.py
+-rw-r--r--   0 root         (0) root         (0)     3267 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/operators/unary_op.py
+-rw-r--r--   0 root         (0) root         (0)    61261 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/quantizer.py
+-rw-r--r--   0 root         (0) root         (0)    31618 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/smooth_quant.py
+-rw-r--r--   0 root         (0) root         (0)    24424 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/util.py
+-rw-r--r--   0 root         (0) root         (0)    46355 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/weight_only.py
+-rw-r--r--   0 root         (0) root         (0)   234889 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/pytorch.py
+-rw-r--r--   0 root         (0) root         (0)    16657 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/pytorch_cpu.yaml
+-rw-r--r--   0 root         (0) root         (0)     2625 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/pytorch_gpu.yaml
+-rw-r--r--   0 root         (0) root         (0)     6572 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/pytorch_ipex.yaml
+-rw-r--r--   0 root         (0) root         (0)     2345 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/query.py
+-rw-r--r--   0 root         (0) root         (0)   117093 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tensorflow.py
+-rw-r--r--   0 root         (0) root         (0)    10069 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tensorflow.yaml
+-rw-r--r--   0 root         (0) root         (0)     6941 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tensorflow_itex.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.200003 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/
+-rw-r--r--   0 root         (0) root         (0)      657 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42617 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_converter.py
+-rw-r--r--   0 root         (0) root         (0)    15850 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_converter_without_calib.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.200003 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/
+-rw-r--r--   0 root         (0) root         (0)      665 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.201003 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/bf16/
+-rw-r--r--   0 root         (0) root         (0)      669 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/bf16/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13750 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/bf16/bf16_convert.py
+-rw-r--r--   0 root         (0) root         (0)     3229 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/bf16/dequantize_cast_optimizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.205003 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/
+-rw-r--r--   0 root         (0) root         (0)      673 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3247 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/convert_add_to_biasadd.py
+-rw-r--r--   0 root         (0) root         (0)     3885 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/convert_layout.py
+-rw-r--r--   0 root         (0) root         (0)     3154 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/convert_leakyrelu.py
+-rw-r--r--   0 root         (0) root         (0)     1933 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/convert_nan_to_random.py
+-rw-r--r--   0 root         (0) root         (0)     4349 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/convert_placeholder_to_const.py
+-rw-r--r--   0 root         (0) root         (0)     4079 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/dilated_contraction.py
+-rw-r--r--   0 root         (0) root         (0)     5856 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/dummy_biasadd.py
+-rw-r--r--   0 root         (0) root         (0)     3397 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/expanddims_optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     3956 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fetch_weight_from_reshape.py
+-rw-r--r--   0 root         (0) root         (0)    13153 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fold_batch_norm.py
+-rw-r--r--   0 root         (0) root         (0)     7509 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fold_constant.py
+-rw-r--r--   0 root         (0) root         (0)     2894 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_biasadd_add.py
+-rw-r--r--   0 root         (0) root         (0)     3885 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_column_wise_mul.py
+-rw-r--r--   0 root         (0) root         (0)     4942 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_conv_with_math.py
+-rw-r--r--   0 root         (0) root         (0)    16460 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_decomposed_bn.py
+-rw-r--r--   0 root         (0) root         (0)    15582 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_decomposed_in.py
+-rw-r--r--   0 root         (0) root         (0)     9504 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_gelu.py
+-rw-r--r--   0 root         (0) root         (0)     9742 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_layer_norm.py
+-rw-r--r--   0 root         (0) root         (0)     5477 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_pad_with_conv.py
+-rw-r--r--   0 root         (0) root         (0)     5583 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_pad_with_fp32_conv.py
+-rw-r--r--   0 root         (0) root         (0)     5889 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_reshape_transpose.py
+-rw-r--r--   0 root         (0) root         (0)     5925 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/graph_cse_optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     3147 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/grappler_pass.py
+-rw-r--r--   0 root         (0) root         (0)    12742 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/insert_print_node.py
+-rw-r--r--   0 root         (0) root         (0)     6171 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/move_squeeze_after_relu.py
+-rw-r--r--   0 root         (0) root         (0)    13729 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/pre_optimize.py
+-rw-r--r--   0 root         (0) root         (0)     2779 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/remove_training_nodes.py
+-rw-r--r--   0 root         (0) root         (0)     2316 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/rename_batch_norm.py
+-rw-r--r--   0 root         (0) root         (0)     2618 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/split_shared_input.py
+-rw-r--r--   0 root         (0) root         (0)     2115 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/strip_equivalent_nodes.py
+-rw-r--r--   0 root         (0) root         (0)     1508 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/strip_unused_nodes.py
+-rw-r--r--   0 root         (0) root         (0)     3432 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/switch_optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     1224 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/graph_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.207003 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/
+-rw-r--r--   0 root         (0) root         (0)      670 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7070 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/freeze_fake_quant.py
+-rw-r--r--   0 root         (0) root         (0)    17659 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/freeze_value.py
+-rw-r--r--   0 root         (0) root         (0)     5630 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/freeze_value_without_calib.py
+-rw-r--r--   0 root         (0) root         (0)     7135 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/fuse_conv_redundant_dequantize.py
+-rw-r--r--   0 root         (0) root         (0)    42958 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/fuse_conv_requantize.py
+-rw-r--r--   0 root         (0) root         (0)     8240 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/fuse_matmul_redundant_dequantize.py
+-rw-r--r--   0 root         (0) root         (0)    44838 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/fuse_matmul_requantize.py
+-rw-r--r--   0 root         (0) root         (0)     5396 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/meta_op_optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     1895 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/post_hostconst_converter.py
+-rw-r--r--   0 root         (0) root         (0)     5420 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/post_quantized_op_cse.py
+-rw-r--r--   0 root         (0) root         (0)    16003 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/rnn_convert.py
+-rw-r--r--   0 root         (0) root         (0)     4763 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/scale_propagation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.208003 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/onnx/
+-rw-r--r--   0 root         (0) root         (0)      692 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/onnx/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    55660 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/onnx/onnx_graph.py
+-rw-r--r--   0 root         (0) root         (0)    13491 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/onnx/onnx_node.py
+-rw-r--r--   0 root         (0) root         (0)     4580 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/onnx/onnx_schema.py
+-rw-r--r--   0 root         (0) root         (0)    22693 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/onnx/tf2onnx_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.209003 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/qdq/
+-rw-r--r--   0 root         (0) root         (0)      669 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/qdq/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    37978 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/qdq/insert_qdq_pattern.py
+-rw-r--r--   0 root         (0) root         (0)     4293 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/qdq/merge_duplicated_qdq.py
+-rw-r--r--   0 root         (0) root         (0)     2539 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/qdq/share_qdq_y_pattern.py
+-rw-r--r--   0 root         (0) root         (0)    42637 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.210003 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/
+-rw-r--r--   0 root         (0) root         (0)      666 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.211003 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/qat/
+-rw-r--r--   0 root         (0) root         (0)      670 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/qat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8567 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/qat/fake_quantize.py
+-rw-r--r--   0 root         (0) root         (0)     4623 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_config.py
+-rw-r--r--   0 root         (0) root         (0)     3015 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.211003 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_layers/
+-rw-r--r--   0 root         (0) root         (0)      675 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_layers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1265 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_layers/optimize_layer.py
+-rw-r--r--   0 root         (0) root         (0)     3053 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_layers/quantize_layer_add.py
+-rw-r--r--   0 root         (0) root         (0)     3116 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_layers/quantize_layer_base.py
+-rw-r--r--   0 root         (0) root         (0)     2102 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_layers/quantize_layer_bn.py
+-rw-r--r--   0 root         (0) root         (0)    10193 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.213003 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/
+-rw-r--r--   0 root         (0) root         (0)      670 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13835 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_bn.py
+-rw-r--r--   0 root         (0) root         (0)    12289 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_concatv2.py
+-rw-r--r--   0 root         (0) root         (0)   112937 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_conv.py
+-rw-r--r--   0 root         (0) root         (0)    27109 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_deconv.py
+-rw-r--r--   0 root         (0) root         (0)     8235 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_in.py
+-rw-r--r--   0 root         (0) root         (0)    55166 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_matmul.py
+-rw-r--r--   0 root         (0) root         (0)     6063 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_pooling.py
+-rw-r--r--   0 root         (0) root         (0)     7189 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/optimize_qdq.py
+-rw-r--r--   0 root         (0) root         (0)    36897 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_base.py
+-rw-r--r--   0 root         (0) root         (0)    13563 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_bn.py
+-rw-r--r--   0 root         (0) root         (0)     4638 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_concatv2.py
+-rw-r--r--   0 root         (0) root         (0)    20539 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_conv.py
+-rw-r--r--   0 root         (0) root         (0)     5626 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_for_intel_cpu.py
+-rw-r--r--   0 root         (0) root         (0)    17114 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_matmul.py
+-rw-r--r--   0 root         (0) root         (0)     3198 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_pooling.py
+-rw-r--r--   0 root         (0) root         (0)    19111 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph_common.py
+-rw-r--r--   0 root         (0) root         (0)    23797 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/smooth_quant_calibration.py
+-rw-r--r--   0 root         (0) root         (0)    13820 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/smooth_quant_scaler.py
+-rw-r--r--   0 root         (0) root         (0)    14537 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/tf2onnx_converter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.214003 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/transform_graph/
+-rw-r--r--   0 root         (0) root         (0)      662 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/transform_graph/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6046 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/transform_graph/bias_correction.py
+-rw-r--r--   0 root         (0) root         (0)     3543 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/transform_graph/graph_transform_base.py
+-rw-r--r--   0 root         (0) root         (0)     8974 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/transform_graph/insert_logging.py
+-rw-r--r--   0 root         (0) root         (0)    14933 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/transform_graph/rerange_quantized_concat.py
+-rw-r--r--   0 root         (0) root         (0)    33328 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.215003 neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/
+-rw-r--r--   0 root         (0) root         (0)      657 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1051 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/auto_round.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.216004 neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/autoround/
+-rw-r--r--   0 root         (0) root         (0)      690 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/autoround/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    65995 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/autoround/autoround.py
+-rw-r--r--   0 root         (0) root         (0)     3936 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/autoround/export.py
+-rw-r--r--   0 root         (0) root         (0)    14501 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/autoround/model_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)    14977 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/autoround/sign_sgd.py
+-rw-r--r--   0 root         (0) root         (0)    21376 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/awq.py
+-rw-r--r--   0 root         (0) root         (0)     3492 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/bf16_convert.py
+-rw-r--r--   0 root         (0) root         (0)    44360 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/gptq.py
+-rw-r--r--   0 root         (0) root         (0)    25511 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/hawq_metric.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.217003 neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/layer_wise_quant/
+-rw-r--r--   0 root         (0) root         (0)      748 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/layer_wise_quant/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    64065 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/layer_wise_quant/modified_pickle.py
+-rw-r--r--   0 root         (0) root         (0)    11304 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/layer_wise_quant/quantize.py
+-rw-r--r--   0 root         (0) root         (0)    12959 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/layer_wise_quant/torch_load.py
+-rw-r--r--   0 root         (0) root         (0)    10151 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/layer_wise_quant/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1920 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/mixed_precision.py
+-rw-r--r--   0 root         (0) root         (0)    23752 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/model_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     7138 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/pattern_detector.py
+-rw-r--r--   0 root         (0) root         (0)     2720 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/symbolic_trace.py
+-rw-r--r--   0 root         (0) root         (0)    12834 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/teq.py
+-rw-r--r--   0 root         (0) root         (0)    50405 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.218004 neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/waq/
+-rw-r--r--   0 root         (0) root         (0)      743 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/waq/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30061 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/waq/auto_alpha.py
+-rw-r--r--   0 root         (0) root         (0)     4118 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/waq/calibration.py
+-rw-r--r--   0 root         (0) root         (0)     9480 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/waq/graph_trace.py
+-rw-r--r--   0 root         (0) root         (0)    26463 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/waq/smooth_quant.py
+-rw-r--r--   0 root         (0) root         (0)    14485 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/waq/utils.py
+-rw-r--r--   0 root         (0) root         (0)    30244 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/weight_only.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.219004 neural_compressor-2.5.1/neural_compressor/algorithm/
+-rw-r--r--   0 root         (0) root         (0)     1131 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/algorithm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6362 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/algorithm/algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     6258 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/algorithm/fast_bias_correction.py
+-rw-r--r--   0 root         (0) root         (0)     3877 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/algorithm/smooth_quant.py
+-rw-r--r--   0 root         (0) root         (0)     6102 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/algorithm/weight_correction.py
+-rw-r--r--   0 root         (0) root         (0)    22341 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/benchmark.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.219004 neural_compressor-2.5.1/neural_compressor/compression/
+-rw-r--r--   0 root         (0) root         (0)      731 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/compression/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19814 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/compression/callbacks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.219004 neural_compressor-2.5.1/neural_compressor/compression/distillation/
+-rw-r--r--   0 root         (0) root         (0)      658 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/compression/distillation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    67415 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/compression/distillation/criterions.py
+-rw-r--r--   0 root         (0) root         (0)     7604 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/compression/distillation/optimizers.py
+-rw-r--r--   0 root         (0) root         (0)     2207 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/compression/distillation/utility.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.220004 neural_compressor-2.5.1/neural_compressor/compression/hpo/
+-rw-r--r--   0 root         (0) root         (0)      758 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/compression/hpo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4293 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/compression/hpo/sa_optimizer.py
+-rw-r--r--   0 root         (0) root         (0)    12510 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/compression/hpo/search_algorithms.py
+-rw-r--r--   0 root         (0) root         (0)     5809 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/compression/hpo/search_space.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.221004 neural_compressor-2.5.1/neural_compressor/compression/pruner/
+-rw-r--r--   0 root         (0) root         (0)     8050 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/compression/pruner/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13557 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/compression/pruner/criteria.py
+-rw-r--r--   0 root         (0) root         (0)    13722 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/compression/pruner/dsnot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.222004 neural_compressor-2.5.1/neural_compressor/compression/pruner/model_slim/
+-rw-r--r--   0 root         (0) root         (0)      750 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/compression/pruner/model_slim/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4999 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/compression/pruner/model_slim/auto_slim.py
+-rw-r--r--   0 root         (0) root         (0)    35992 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/compression/pruner/model_slim/pattern_analyzer.py
+-rw-r--r--   0 root         (0) root         (0)    17780 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/compression/pruner/model_slim/weight_slim.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.222004 neural_compressor-2.5.1/neural_compressor/compression/pruner/patterns/
+-rw-r--r--   0 root         (0) root         (0)     2043 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/compression/pruner/patterns/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30952 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/compression/pruner/patterns/base.py
+-rw-r--r--   0 root         (0) root         (0)     2269 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/compression/pruner/patterns/mha.py
+-rw-r--r--   0 root         (0) root         (0)    19320 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/compression/pruner/patterns/ninm.py
+-rw-r--r--   0 root         (0) root         (0)    35816 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/compression/pruner/patterns/nxm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.224004 neural_compressor-2.5.1/neural_compressor/compression/pruner/pruners/
+-rw-r--r--   0 root         (0) root         (0)     3318 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/compression/pruner/pruners/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10453 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/compression/pruner/pruners/base.py
+-rw-r--r--   0 root         (0) root         (0)     8602 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/compression/pruner/pruners/basic.py
+-rw-r--r--   0 root         (0) root         (0)     6709 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/compression/pruner/pruners/block_mask.py
+-rw-r--r--   0 root         (0) root         (0)    11925 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/compression/pruner/pruners/mha.py
+-rw-r--r--   0 root         (0) root         (0)     2159 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/compression/pruner/pruners/pattern_lock.py
+-rw-r--r--   0 root         (0) root         (0)    14028 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/compression/pruner/pruners/progressive.py
+-rw-r--r--   0 root         (0) root         (0)     8627 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/compression/pruner/pruners/retrain_free.py
+-rw-r--r--   0 root         (0) root         (0)     4492 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/compression/pruner/pruners/sparse_gpt.py
+-rw-r--r--   0 root         (0) root         (0)    11500 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/compression/pruner/pruning.py
+-rw-r--r--   0 root         (0) root         (0)     5080 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/compression/pruner/regs.py
+-rw-r--r--   0 root         (0) root         (0)     6258 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/compression/pruner/schedulers.py
+-rw-r--r--   0 root         (0) root         (0)     3170 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/compression/pruner/tf_criteria.py
+-rw-r--r--   0 root         (0) root         (0)    30386 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/compression/pruner/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.224004 neural_compressor-2.5.1/neural_compressor/compression/pruner/wanda/
+-rw-r--r--   0 root         (0) root         (0)      683 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/compression/pruner/wanda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9216 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/compression/pruner/wanda/prune.py
+-rw-r--r--   0 root         (0) root         (0)     2105 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/compression/pruner/wanda/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2744 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/compression/pruner/wanda/wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.225004 neural_compressor-2.5.1/neural_compressor/conf/
+-rw-r--r--   0 root         (0) root         (0)      631 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/conf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    73546 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/conf/config.py
+-rw-r--r--   0 root         (0) root         (0)     2980 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/conf/dotdict.py
+-rw-r--r--   0 root         (0) root         (0)    52365 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/conf/pythonic_config.py
+-rw-r--r--   0 root         (0) root         (0)    96109 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.225004 neural_compressor-2.5.1/neural_compressor/contrib/
+-rw-r--r--   0 root         (0) root         (0)      712 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/contrib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.226004 neural_compressor-2.5.1/neural_compressor/contrib/strategy/
+-rw-r--r--   0 root         (0) root         (0)      971 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/contrib/strategy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15560 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/contrib/strategy/sigopt.py
+-rw-r--r--   0 root         (0) root         (0)    25177 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/contrib/strategy/tpe.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.226004 neural_compressor-2.5.1/neural_compressor/data/
+-rw-r--r--   0 root         (0) root         (0)     2483 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.227004 neural_compressor-2.5.1/neural_compressor/data/dataloaders/
+-rw-r--r--   0 root         (0) root         (0)      802 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/data/dataloaders/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4978 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/data/dataloaders/base_dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     5995 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/data/dataloaders/dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     6267 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/data/dataloaders/default_dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     4931 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/data/dataloaders/fetcher.py
+-rw-r--r--   0 root         (0) root         (0)     1745 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/data/dataloaders/mxnet_dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     3770 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/data/dataloaders/onnxrt_dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     2585 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/data/dataloaders/pytorch_dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     5117 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/data/dataloaders/sampler.py
+-rw-r--r--   0 root         (0) root         (0)    15359 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/data/dataloaders/tensorflow_dataloader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.228004 neural_compressor-2.5.1/neural_compressor/data/datasets/
+-rw-r--r--   0 root         (0) root         (0)     1240 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/data/datasets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19357 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/data/datasets/bert_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    12572 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/data/datasets/coco_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    42400 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/data/datasets/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     6680 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/data/datasets/dummy_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    13357 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/data/datasets/dummy_dataset_v2.py
+-rw-r--r--   0 root         (0) root         (0)     9362 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/data/datasets/imagenet_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     3672 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/data/datasets/style_transfer_dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.229004 neural_compressor-2.5.1/neural_compressor/data/filters/
+-rw-r--r--   0 root         (0) root         (0)     1130 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/data/filters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1935 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/data/filters/coco_filter.py
+-rw-r--r--   0 root         (0) root         (0)     5858 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/data/filters/filter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.229004 neural_compressor-2.5.1/neural_compressor/data/transforms/
+-rw-r--r--   0 root         (0) root         (0)     2079 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/data/transforms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2023 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/data/transforms/coco_transform.py
+-rw-r--r--   0 root         (0) root         (0)    18418 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/data/transforms/imagenet_transform.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/data/transforms/postprocess.py
+-rw-r--r--   0 root         (0) root         (0)    12107 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/data/transforms/tokenization.py
+-rw-r--r--   0 root         (0) root         (0)   105024 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/data/transforms/transform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.231004 neural_compressor-2.5.1/neural_compressor/experimental/
+-rw-r--r--   0 root         (0) root         (0)     1367 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30418 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/benchmark.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.232004 neural_compressor-2.5.1/neural_compressor/experimental/common/
+-rw-r--r--   0 root         (0) root         (0)     1033 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    47431 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/common/criterion.py
+-rw-r--r--   0 root         (0) root         (0)     5261 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/common/dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     1583 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/common/metric.py
+-rw-r--r--   0 root         (0) root         (0)     2728 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/common/model.py
+-rw-r--r--   0 root         (0) root         (0)     6799 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/common/optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/common/postprocess.py
+-rw-r--r--   0 root         (0) root         (0)     2295 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/common/torch_utils.py
+-rw-r--r--   0 root         (0) root         (0)    24785 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/component.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.232004 neural_compressor-2.5.1/neural_compressor/experimental/compression/
+-rw-r--r--   0 root         (0) root         (0)      664 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/compression/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.232004 neural_compressor-2.5.1/neural_compressor/experimental/contrib/
+-rw-r--r--   0 root         (0) root         (0)      712 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/contrib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.233004 neural_compressor-2.5.1/neural_compressor/experimental/contrib/strategy/
+-rw-r--r--   0 root         (0) root         (0)      970 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/contrib/strategy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14083 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/contrib/strategy/sigopt.py
+-rw-r--r--   0 root         (0) root         (0)    25050 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/contrib/strategy/tpe.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.233004 neural_compressor-2.5.1/neural_compressor/experimental/data/
+-rw-r--r--   0 root         (0) root         (0)     1270 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.234004 neural_compressor-2.5.1/neural_compressor/experimental/data/dataloaders/
+-rw-r--r--   0 root         (0) root         (0)      836 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/data/dataloaders/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5020 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/data/dataloaders/base_dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     1410 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/data/dataloaders/dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     6284 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/data/dataloaders/default_dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     4987 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/data/dataloaders/fetcher.py
+-rw-r--r--   0 root         (0) root         (0)     1787 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/data/dataloaders/mxnet_dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     3819 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/data/dataloaders/onnxrt_dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     2606 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/data/dataloaders/pytorch_dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     5180 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/data/dataloaders/sampler.py
+-rw-r--r--   0 root         (0) root         (0)    15349 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/data/dataloaders/tensorflow_dataloader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.236004 neural_compressor-2.5.1/neural_compressor/experimental/data/datasets/
+-rw-r--r--   0 root         (0) root         (0)     1127 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/data/datasets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19191 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/data/datasets/bert_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    12492 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/data/datasets/coco_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    41844 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/data/datasets/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     6660 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/data/datasets/dummy_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    13317 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/data/datasets/dummy_dataset_v2.py
+-rw-r--r--   0 root         (0) root         (0)     9242 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/data/datasets/imagenet_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     3652 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/data/datasets/style_transfer_dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.236004 neural_compressor-2.5.1/neural_compressor/experimental/data/filters/
+-rw-r--r--   0 root         (0) root         (0)     1044 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/data/filters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1895 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/data/filters/coco_filter.py
+-rw-r--r--   0 root         (0) root         (0)     5697 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/data/filters/filter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.237004 neural_compressor-2.5.1/neural_compressor/experimental/data/transforms/
+-rw-r--r--   0 root         (0) root         (0)     1208 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/data/transforms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17438 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/data/transforms/imagenet_transform.py
+-rw-r--r--   0 root         (0) root         (0)    12107 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/data/transforms/tokenization.py
+-rw-r--r--   0 root         (0) root         (0)   105074 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/data/transforms/transform.py
+-rw-r--r--   0 root         (0) root         (0)    21663 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/distillation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.237004 neural_compressor-2.5.1/neural_compressor/experimental/export/
+-rw-r--r--   0 root         (0) root         (0)      832 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/export/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3089 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/export/qlinear2qdq.py
+-rw-r--r--   0 root         (0) root         (0)     4806 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/export/tf2onnx.py
+-rw-r--r--   0 root         (0) root         (0)    16037 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/export/torch2onnx.py
+-rw-r--r--   0 root         (0) root         (0)    20023 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/graph_optimization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.238004 neural_compressor-2.5.1/neural_compressor/experimental/metric/
+-rw-r--r--   0 root         (0) root         (0)     1067 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/metric/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4977 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/metric/bleu.py
+-rw-r--r--   0 root         (0) root         (0)     5146 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/metric/bleu_util.py
+-rw-r--r--   0 root         (0) root         (0)     2188 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/metric/coco_label_map.py
+-rw-r--r--   0 root         (0) root         (0)    31804 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/metric/coco_tools.py
+-rw-r--r--   0 root         (0) root         (0)     4358 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/metric/evaluate_squad.py
+-rw-r--r--   0 root         (0) root         (0)     5323 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/metric/f1.py
+-rw-r--r--   0 root         (0) root         (0)    57242 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/metric/metric.py
+-rw-r--r--   0 root         (0) root         (0)    10161 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/mixed_precision.py
+-rw-r--r--   0 root         (0) root         (0)    15510 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/model_conversion.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.239004 neural_compressor-2.5.1/neural_compressor/experimental/nas/
+-rw-r--r--   0 root         (0) root         (0)      729 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/nas/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5755 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/nas/basic_nas.py
+-rw-r--r--   0 root         (0) root         (0)     4237 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/nas/dynas.py
+-rw-r--r--   0 root         (0) root         (0)    15265 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/nas/nas.py
+-rw-r--r--   0 root         (0) root         (0)     2913 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/nas/nas_utils.py
+-rw-r--r--   0 root         (0) root         (0)     6010 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/nas/search_algorithms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.240004 neural_compressor-2.5.1/neural_compressor/experimental/pruner_legacy/
+-rw-r--r--   0 root         (0) root         (0)      994 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/pruner_legacy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11431 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/pruner_legacy/gradient_sensitivity.py
+-rw-r--r--   0 root         (0) root         (0)     2740 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/pruner_legacy/group_lasso.py
+-rw-r--r--   0 root         (0) root         (0)     4579 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/pruner_legacy/magnitude.py
+-rw-r--r--   0 root         (0) root         (0)     2219 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/pruner_legacy/pattern_lock.py
+-rw-r--r--   0 root         (0) root         (0)     4795 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/pruner_legacy/pruner.py
+-rw-r--r--   0 root         (0) root         (0)    21661 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/pruning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.240004 neural_compressor-2.5.1/neural_compressor/experimental/pruning_recipes/
+-rw-r--r--   0 root         (0) root         (0)      738 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/pruning_recipes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.241004 neural_compressor-2.5.1/neural_compressor/experimental/pruning_recipes/patterns/
+-rw-r--r--   0 root         (0) root         (0)     1018 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/pruning_recipes/patterns/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3799 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/pruning_recipes/patterns/pattern.py
+-rw-r--r--   0 root         (0) root         (0)     3006 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/pruning_recipes/patterns/tile_pattern.py
+-rw-r--r--   0 root         (0) root         (0)    22247 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/pruning_v2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.241004 neural_compressor-2.5.1/neural_compressor/experimental/pytorch_pruner/
+-rw-r--r--   0 root         (0) root         (0)      661 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/pytorch_pruner/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      682 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/pytorch_pruner/logger.py
+-rw-r--r--   0 root         (0) root         (0)    25049 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/pytorch_pruner/patterns.py
+-rw-r--r--   0 root         (0) root         (0)     9243 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/pytorch_pruner/prune_utils.py
+-rw-r--r--   0 root         (0) root         (0)    12507 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/pytorch_pruner/pruner.py
+-rw-r--r--   0 root         (0) root         (0)     6414 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/pytorch_pruner/pruning.py
+-rw-r--r--   0 root         (0) root         (0)     5554 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/pytorch_pruner/scheduler.py
+-rw-r--r--   0 root         (0) root         (0)    22801 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/quantization.py
+-rw-r--r--   0 root         (0) root         (0)    18339 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.243004 neural_compressor-2.5.1/neural_compressor/experimental/strategy/
+-rw-r--r--   0 root         (0) root         (0)     1022 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/strategy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7684 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/strategy/auto_mixed_precision.py
+-rw-r--r--   0 root         (0) root         (0)     9809 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/strategy/basic.py
+-rw-r--r--   0 root         (0) root         (0)    15351 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/strategy/bayesian.py
+-rw-r--r--   0 root         (0) root         (0)     2156 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/strategy/exhaustive.py
+-rw-r--r--   0 root         (0) root         (0)    10626 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/strategy/mse.py
+-rw-r--r--   0 root         (0) root         (0)    11339 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/strategy/mse_v2.py
+-rw-r--r--   0 root         (0) root         (0)     2508 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/strategy/random.py
+-rw-r--r--   0 root         (0) root         (0)    65514 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/strategy/strategy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.244005 neural_compressor-2.5.1/neural_compressor/experimental/strategy/utils/
+-rw-r--r--   0 root         (0) root         (0)      905 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/strategy/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1393 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/strategy/utils/constant.py
+-rw-r--r--   0 root         (0) root         (0)    22145 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/strategy/utils/tuning_sampler.py
+-rw-r--r--   0 root         (0) root         (0)    30511 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/strategy/utils/tuning_space.py
+-rw-r--r--   0 root         (0) root         (0)     3836 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/strategy/utils/tuning_structs.py
+-rw-r--r--   0 root         (0) root         (0)     1903 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/experimental/strategy/utils/utility.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.245005 neural_compressor-2.5.1/neural_compressor/metric/
+-rw-r--r--   0 root         (0) root         (0)     1325 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/metric/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4862 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/metric/bleu.py
+-rw-r--r--   0 root         (0) root         (0)     5058 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/metric/bleu_util.py
+-rw-r--r--   0 root         (0) root         (0)     2188 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/metric/coco_label_map.py
+-rw-r--r--   0 root         (0) root         (0)    31581 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/metric/coco_tools.py
+-rw-r--r--   0 root         (0) root         (0)     4215 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/metric/evaluate_squad.py
+-rw-r--r--   0 root         (0) root         (0)     5234 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/metric/f1.py
+-rw-r--r--   0 root         (0) root         (0)    59780 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/metric/metric.py
+-rw-r--r--   0 root         (0) root         (0)     8282 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/mix_precision.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.246005 neural_compressor-2.5.1/neural_compressor/model/
+-rw-r--r--   0 root         (0) root         (0)      797 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2095 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/model/base_model.py
+-rw-r--r--   0 root         (0) root         (0)     4376 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/model/keras_model.py
+-rw-r--r--   0 root         (0) root         (0)    11417 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/model/model.py
+-rw-r--r--   0 root         (0) root         (0)     2471 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/model/mxnet_model.py
+-rw-r--r--   0 root         (0) root         (0)     5879 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/model/nets_factory.py
+-rw-r--r--   0 root         (0) root         (0)    50294 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/model/onnx_model.py
+-rw-r--r--   0 root         (0) root         (0)    58843 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/model/tensorflow_model.py
+-rw-r--r--   0 root         (0) root         (0)    28046 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/model/torch_model.py
+-rw-r--r--   0 root         (0) root         (0)    21840 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/objective.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.246005 neural_compressor-2.5.1/neural_compressor/profiling/
+-rw-r--r--   0 root         (0) root         (0)      663 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/profiling/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.247005 neural_compressor-2.5.1/neural_compressor/profiling/parser/
+-rw-r--r--   0 root         (0) root         (0)      621 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/profiling/parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1766 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/profiling/parser/factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.247005 neural_compressor-2.5.1/neural_compressor/profiling/parser/onnx_parser/
+-rw-r--r--   0 root         (0) root         (0)      621 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/profiling/parser/onnx_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1295 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/profiling/parser/onnx_parser/factory.py
+-rw-r--r--   0 root         (0) root         (0)     2943 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/profiling/parser/onnx_parser/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2202 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/profiling/parser/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2198 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/profiling/parser/result.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.248005 neural_compressor-2.5.1/neural_compressor/profiling/parser/tensorflow_parser/
+-rw-r--r--   0 root         (0) root         (0)      621 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/profiling/parser/tensorflow_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1329 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/profiling/parser/tensorflow_parser/factory.py
+-rw-r--r--   0 root         (0) root         (0)     4346 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/profiling/parser/tensorflow_parser/parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.248005 neural_compressor-2.5.1/neural_compressor/profiling/profiler/
+-rw-r--r--   0 root         (0) root         (0)      621 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/profiling/profiler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2076 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/profiling/profiler/factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.248005 neural_compressor-2.5.1/neural_compressor/profiling/profiler/onnxrt_profiler/
+-rw-r--r--   0 root         (0) root         (0)      621 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/profiling/profiler/onnxrt_profiler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1525 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/profiling/profiler/onnxrt_profiler/factory.py
+-rw-r--r--   0 root         (0) root         (0)     3310 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/profiling/profiler/onnxrt_profiler/profiler.py
+-rw-r--r--   0 root         (0) root         (0)     1284 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/profiling/profiler/onnxrt_profiler/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1052 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/profiling/profiler/profiler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.249005 neural_compressor-2.5.1/neural_compressor/profiling/profiler/tensorflow_profiler/
+-rw-r--r--   0 root         (0) root         (0)      621 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/profiling/profiler/tensorflow_profiler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1945 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/profiling/profiler/tensorflow_profiler/factory.py
+-rw-r--r--   0 root         (0) root         (0)     5417 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/profiling/profiler/tensorflow_profiler/profiler.py
+-rw-r--r--   0 root         (0) root         (0)     2682 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/profiling/profiler/tensorflow_profiler/utils.py
+-rw-r--r--   0 root         (0) root         (0)    12315 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/quantization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.251005 neural_compressor-2.5.1/neural_compressor/strategy/
+-rw-r--r--   0 root         (0) root         (0)     1014 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/strategy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6214 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/strategy/auto.py
+-rw-r--r--   0 root         (0) root         (0)    11697 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/strategy/auto_mixed_precision.py
+-rw-r--r--   0 root         (0) root         (0)    22059 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/strategy/basic.py
+-rw-r--r--   0 root         (0) root         (0)    16611 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/strategy/bayesian.py
+-rw-r--r--   0 root         (0) root         (0)    11127 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/strategy/conservative.py
+-rw-r--r--   0 root         (0) root         (0)     2079 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/strategy/exhaustive.py
+-rw-r--r--   0 root         (0) root         (0)     5584 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/strategy/hawq_v2.py
+-rw-r--r--   0 root         (0) root         (0)    11845 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/strategy/mse.py
+-rw-r--r--   0 root         (0) root         (0)    10617 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/strategy/mse_v2.py
+-rw-r--r--   0 root         (0) root         (0)     2348 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/strategy/random.py
+-rw-r--r--   0 root         (0) root         (0)   101604 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/strategy/strategy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.252005 neural_compressor-2.5.1/neural_compressor/strategy/utils/
+-rw-r--r--   0 root         (0) root         (0)      905 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/strategy/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2243 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/strategy/utils/constant.py
+-rw-r--r--   0 root         (0) root         (0)    28718 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/strategy/utils/tuning_sampler.py
+-rw-r--r--   0 root         (0) root         (0)    32978 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/strategy/utils/tuning_space.py
+-rw-r--r--   0 root         (0) root         (0)     4130 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/strategy/utils/tuning_structs.py
+-rw-r--r--   0 root         (0) root         (0)     4676 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/strategy/utils/utility.py
+-rw-r--r--   0 root         (0) root         (0)    21463 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/training.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.253005 neural_compressor-2.5.1/neural_compressor/utils/
+-rw-r--r--   0 root         (0) root         (0)     1057 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2783 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/utils/collect_layer_histogram.py
+-rw-r--r--   0 root         (0) root         (0)     2917 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/utils/constant.py
+-rw-r--r--   0 root         (0) root         (0)     9390 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/utils/create_obj_from_config.py
+-rw-r--r--   0 root         (0) root         (0)     5751 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/utils/kl_divergence.py
+-rw-r--r--   0 root         (0) root         (0)    15257 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/utils/load_huggingface.py
+-rw-r--r--   0 root         (0) root         (0)     4594 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/utils/logger.py
+-rw-r--r--   0 root         (0) root         (0)     6117 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/utils/neural_insights_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1231 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/utils/options.py
+-rw-r--r--   0 root         (0) root         (0)    23214 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/utils/pytorch.py
+-rw-r--r--   0 root         (0) root         (0)    36312 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/utils/utility.py
+-rw-r--r--   0 root         (0) root         (0)     2640 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/utils/weights_details.py
+-rw-r--r--   0 root         (0) root         (0)      765 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/neural_compressor/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:33:46.253005 neural_compressor-2.5.1/neural_compressor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15595 2024-04-03 13:33:46.000000 neural_compressor-2.5.1/neural_compressor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    29656 2024-04-03 13:33:46.000000 neural_compressor-2.5.1/neural_compressor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 13:33:46.000000 neural_compressor-2.5.1/neural_compressor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      387 2024-04-03 13:33:46.000000 neural_compressor-2.5.1/neural_compressor.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-04-03 13:33:46.000000 neural_compressor-2.5.1/neural_compressor.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2418 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      102 2024-04-03 13:33:46.255005 neural_compressor-2.5.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8675 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/setup.py
+-rw-r--r--   0 root         (0) root         (0)    95740 2024-04-03 13:33:19.000000 neural_compressor-2.5.1/third-party-programs.txt
```

### Comparing `neural_compressor-2.5/LICENSE` & `neural_compressor-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/PKG-INFO` & `neural_compressor-2.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neural_compressor
-Version: 2.5
+Version: 2.5.1
 Summary: Repository of Intel® Neural Compressor
 Home-page: https://github.com/intel/neural-compressor
 Author: Intel AIPT Team
 Author-email: feng.tian@intel.com, haihao.shen@intel.com, suyue.chen@intel.com
 License: Apache 2.0
 Keywords: quantization,auto-tuning,post-training static quantization,post-training dynamic quantization,quantization-aware training
 Classifier: Intended Audience :: Science/Research
@@ -26,19 +26,19 @@
 Requires-Dist: pycocotools; sys_platform != "win32" or python_version > "3.8"
 Requires-Dist: pycocotools-windows; sys_platform == "win32" and python_version <= "3.8"
 Requires-Dist: pyyaml
 Requires-Dist: requests
 Requires-Dist: schema
 Requires-Dist: scikit-learn
 Provides-Extra: pt
-Requires-Dist: neural_compressor_3x_pt==2.5; extra == "pt"
+Requires-Dist: neural_compressor_3x_pt==2.5.1; extra == "pt"
 Provides-Extra: tf
-Requires-Dist: neural_compressor_3x_tf==2.5; extra == "tf"
+Requires-Dist: neural_compressor_3x_tf==2.5.1; extra == "tf"
 Provides-Extra: ort
-Requires-Dist: neural_compressor_3x_ort==2.5; extra == "ort"
+Requires-Dist: neural_compressor_3x_ort==2.5.1; extra == "ort"
 
 <div align="center">
 
 Intel® Neural Compressor
 ===========================
 <h3> An open-source Python library supporting popular model compression techniques on all mainstream deep learning frameworks (TensorFlow, PyTorch, ONNX Runtime, and MXNet)</h3>
```

### Comparing `neural_compressor-2.5/README.md` & `neural_compressor-2.5.1/README.md`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/__init__.py` & `neural_compressor-2.5.1/neural_coder/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/__main__.py` & `neural_compressor-2.5.1/neural_coder/__main__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/__init__.py` & `neural_compressor-2.5.1/neural_coder/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/intel_extension_for_transformers.yaml` & `neural_compressor-2.5.1/neural_coder/backends/intel_extension_for_transformers.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/keras_inc.yaml` & `neural_compressor-2.5.1/neural_coder/backends/keras_inc.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/nano_bf16.yaml` & `neural_compressor-2.5.1/neural_coder/backends/nano_bf16.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/nano_bf16_channels_last.yaml` & `neural_compressor-2.5.1/neural_coder/backends/nano_bf16_channels_last.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/nano_bf16_ipex.yaml` & `neural_compressor-2.5.1/neural_coder/backends/nano_bf16_ipex.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/nano_bf16_ipex_channels_last.yaml` & `neural_compressor-2.5.1/neural_coder/backends/nano_bf16_ipex_channels_last.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/nano_fp32_channels_last.yaml` & `neural_compressor-2.5.1/neural_coder/backends/nano_fp32_channels_last.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/nano_fp32_ipex.yaml` & `neural_compressor-2.5.1/neural_coder/backends/nano_fp32_ipex.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/nano_fp32_ipex_channels_last.yaml` & `neural_compressor-2.5.1/neural_coder/backends/nano_fp32_ipex_channels_last.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/nano_gpu_to_cpu.yaml` & `neural_compressor-2.5.1/neural_coder/backends/nano_gpu_to_cpu.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/nano_int8.yaml` & `neural_compressor-2.5.1/neural_coder/backends/nano_int8.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/nano_jit_bf16.yaml` & `neural_compressor-2.5.1/neural_coder/backends/nano_jit_bf16.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/nano_jit_bf16_channels_last.yaml` & `neural_compressor-2.5.1/neural_coder/backends/nano_jit_bf16_channels_last.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/nano_jit_bf16_ipex.yaml` & `neural_compressor-2.5.1/neural_coder/backends/nano_jit_bf16_ipex.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/nano_jit_bf16_ipex_channels_last.yaml` & `neural_compressor-2.5.1/neural_coder/backends/nano_jit_bf16_ipex_channels_last.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/nano_jit_fp32.yaml` & `neural_compressor-2.5.1/neural_coder/backends/nano_jit_fp32.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/nano_jit_fp32_channels_last.yaml` & `neural_compressor-2.5.1/neural_coder/backends/nano_jit_fp32_channels_last.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/nano_jit_fp32_ipex.yaml` & `neural_compressor-2.5.1/neural_coder/backends/nano_jit_fp32_ipex.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/nano_jit_fp32_ipex_channels_last.yaml` & `neural_compressor-2.5.1/neural_coder/backends/nano_jit_fp32_ipex_channels_last.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/nano_onnxruntime_fp32.yaml` & `neural_compressor-2.5.1/neural_coder/backends/nano_onnxruntime_fp32.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/nano_onnxruntime_int8_qlinear.yaml` & `neural_compressor-2.5.1/neural_coder/backends/nano_onnxruntime_int8_qlinear.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/nano_openvino_fp32.yaml` & `neural_compressor-2.5.1/neural_coder/backends/nano_openvino_fp32.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/nano_openvino_int8.yaml` & `neural_compressor-2.5.1/neural_coder/backends/nano_openvino_int8.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/onnx_inc_dynamic_quant.yaml` & `neural_compressor-2.5.1/neural_coder/backends/onnx_inc_dynamic_quant.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/onnx_inc_static_quant_qdq.yaml` & `neural_compressor-2.5.1/neural_coder/backends/onnx_inc_static_quant_qdq.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/onnx_inc_static_quant_qlinear.yaml` & `neural_compressor-2.5.1/neural_coder/backends/onnx_inc_static_quant_qlinear.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/pytorch_aliblade.yaml` & `neural_compressor-2.5.1/neural_coder/backends/pytorch_aliblade.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/pytorch_benchmark.yaml` & `neural_compressor-2.5.1/neural_coder/backends/pytorch_benchmark.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/pytorch_channels_last.yaml` & `neural_compressor-2.5.1/neural_coder/backends/pytorch_channels_last.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/pytorch_inc_bf16.yaml` & `neural_compressor-2.5.1/neural_coder/backends/pytorch_inc_bf16.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/pytorch_inc_dynamic_quant.yaml` & `neural_compressor-2.5.1/neural_coder/backends/pytorch_inc_dynamic_quant.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/pytorch_inc_dynamic_quant_fp8.yaml` & `neural_compressor-2.5.1/neural_coder/backends/pytorch_inc_dynamic_quant_fp8.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/pytorch_inc_huggingface_optimum_dynamic.yaml` & `neural_compressor-2.5.1/neural_coder/backends/pytorch_inc_huggingface_optimum_dynamic.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/pytorch_inc_huggingface_optimum_static.yaml` & `neural_compressor-2.5.1/neural_coder/backends/pytorch_inc_huggingface_optimum_static.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/pytorch_inc_static_quant_fx.yaml` & `neural_compressor-2.5.1/neural_coder/backends/pytorch_inc_static_quant_fx.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/pytorch_inc_static_quant_fx_fp8.yaml` & `neural_compressor-2.5.1/neural_coder/backends/pytorch_inc_static_quant_fx_fp8.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/pytorch_inc_static_quant_ipex.yaml` & `neural_compressor-2.5.1/neural_coder/backends/pytorch_inc_static_quant_ipex.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/pytorch_inc_static_quant_ipex_xpu.yaml` & `neural_compressor-2.5.1/neural_coder/backends/pytorch_inc_static_quant_ipex_xpu.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/pytorch_ipex_bf16.yaml` & `neural_compressor-2.5.1/neural_coder/backends/pytorch_ipex_bf16.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/pytorch_ipex_fp32.yaml` & `neural_compressor-2.5.1/neural_coder/backends/pytorch_ipex_fp32.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/pytorch_ipex_int8_dynamic_quant.yaml` & `neural_compressor-2.5.1/neural_coder/backends/pytorch_ipex_int8_dynamic_quant.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/pytorch_ipex_int8_static_quant.yaml` & `neural_compressor-2.5.1/neural_coder/backends/pytorch_ipex_int8_static_quant.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/pytorch_jit_script.yaml` & `neural_compressor-2.5.1/neural_coder/backends/pytorch_jit_script.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/pytorch_jit_script_ofi.yaml` & `neural_compressor-2.5.1/neural_coder/backends/pytorch_jit_script_ofi.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/pytorch_jit_trace.yaml` & `neural_compressor-2.5.1/neural_coder/backends/pytorch_jit_trace.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/pytorch_jit_trace_ofi.yaml` & `neural_compressor-2.5.1/neural_coder/backends/pytorch_jit_trace_ofi.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/pytorch_mixed_precision_cpu.yaml` & `neural_compressor-2.5.1/neural_coder/backends/pytorch_mixed_precision_cpu.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/pytorch_mixed_precision_cuda.yaml` & `neural_compressor-2.5.1/neural_coder/backends/pytorch_mixed_precision_cuda.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/pytorch_mixed_precision_intel_gpu.yaml` & `neural_compressor-2.5.1/neural_coder/backends/pytorch_mixed_precision_intel_gpu.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/pytorch_torchdynamo_jit_script.yaml` & `neural_compressor-2.5.1/neural_coder/backends/pytorch_torchdynamo_jit_script.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/pytorch_torchdynamo_jit_script_ofi.yaml` & `neural_compressor-2.5.1/neural_coder/backends/pytorch_torchdynamo_jit_script_ofi.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/pytorch_torchdynamo_jit_trace.yaml` & `neural_compressor-2.5.1/neural_coder/backends/pytorch_torchdynamo_jit_trace.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/pytorch_torchdynamo_jit_trace_ofi.yaml` & `neural_compressor-2.5.1/neural_coder/backends/pytorch_torchdynamo_jit_trace_ofi.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/backends/template.yaml` & `neural_compressor-2.5.1/neural_coder/backends/template.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/coders/__init__.py` & `neural_compressor-2.5.1/neural_coder/coders/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/coders/autoinc/__init__.py` & `neural_compressor-2.5.1/neural_coder/coders/autoinc/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/coders/autoinc/autoinc_harness.py` & `neural_compressor-2.5.1/neural_coder/coders/autoinc/autoinc_harness.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/coders/autoinc/calib_dataloader.py` & `neural_compressor-2.5.1/neural_coder/coders/autoinc/calib_dataloader.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/coders/autoinc/domain.py` & `neural_compressor-2.5.1/neural_coder/coders/autoinc/domain.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/coders/autoinc/eval_func.py` & `neural_compressor-2.5.1/neural_coder/coders/autoinc/eval_func.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/coders/pytorch/__init__.py` & `neural_compressor-2.5.1/neural_coder/coders/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/coders/pytorch/batch_size.py` & `neural_compressor-2.5.1/neural_coder/coders/pytorch/batch_size.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/coders/pytorch/change_trainer_to_nlptrainer.py` & `neural_compressor-2.5.1/neural_coder/coders/pytorch/change_trainer_to_nlptrainer.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/coders/pytorch/cuda_to_cpu.py` & `neural_compressor-2.5.1/neural_coder/coders/pytorch/cuda_to_cpu.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/coders/pytorch/dummy_dataloader.py` & `neural_compressor-2.5.1/neural_coder/coders/pytorch/dummy_dataloader.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/coders/pytorch/harness.py` & `neural_compressor-2.5.1/neural_coder/coders/pytorch/harness.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/coders/pytorch/lightning.py` & `neural_compressor-2.5.1/neural_coder/coders/pytorch/lightning.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/coders/pytorch/reclaim_inference_transformers_trainer.py` & `neural_compressor-2.5.1/neural_coder/coders/pytorch/reclaim_inference_transformers_trainer.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/coders/pytorch/reclaim_inputs.py` & `neural_compressor-2.5.1/neural_coder/coders/pytorch/reclaim_inputs.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/coders/tensorflow/__init__.py` & `neural_compressor-2.5.1/neural_coder/coders/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/coders/tensorflow/amp.py` & `neural_compressor-2.5.1/neural_coder/coders/tensorflow/amp.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/coders/tensorflow/inc.py` & `neural_compressor-2.5.1/neural_coder/coders/tensorflow/inc.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/coders/transform.py` & `neural_compressor-2.5.1/neural_coder/coders/transform.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/globals.py` & `neural_compressor-2.5.1/neural_coder/globals.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/graphers/__init__.py` & `neural_compressor-2.5.1/neural_coder/graphers/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/graphers/code_line.py` & `neural_compressor-2.5.1/neural_coder/graphers/code_line.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/graphers/function.py` & `neural_compressor-2.5.1/neural_coder/graphers/function.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/graphers/model.py` & `neural_compressor-2.5.1/neural_coder/graphers/model.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/graphers/preloads/__init__.py` & `neural_compressor-2.5.1/neural_coder/graphers/preloads/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/graphers/preloads/transformers.yaml` & `neural_compressor-2.5.1/neural_coder/graphers/preloads/transformers.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/interface.py` & `neural_compressor-2.5.1/neural_coder/interface.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/launcher.py` & `neural_compressor-2.5.1/neural_coder/launcher.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/utils/__init__.py` & `neural_compressor-2.5.1/neural_coder/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/utils/common.py` & `neural_compressor-2.5.1/neural_coder/utils/common.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/utils/cpu_info.py` & `neural_compressor-2.5.1/neural_coder/utils/cpu_info.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/utils/device.py` & `neural_compressor-2.5.1/neural_coder/utils/device.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/utils/handle_user_input.py` & `neural_compressor-2.5.1/neural_coder/utils/handle_user_input.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/utils/line_operation.py` & `neural_compressor-2.5.1/neural_coder/utils/line_operation.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/utils/numa_launcher.py` & `neural_compressor-2.5.1/neural_coder/utils/numa_launcher.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/utils/pdf_report.py` & `neural_compressor-2.5.1/neural_coder/utils/pdf_report.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_coder/version.py` & `neural_compressor-2.5.1/neural_coder/version.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/__init__.py` & `neural_compressor-2.5.1/neural_compressor/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/__init__.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/adaptor.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/adaptor.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/keras.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/keras.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/keras.yaml` & `neural_compressor-2.5.1/neural_compressor/adaptor/keras.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/keras_utils/__init__.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/keras_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/keras_utils/conv2d.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/keras_utils/conv2d.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/keras_utils/dense.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/keras_utils/dense.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/keras_utils/depthwise_conv2d.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/keras_utils/depthwise_conv2d.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/keras_utils/pool2d.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/keras_utils/pool2d.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/keras_utils/quantizer.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/keras_utils/quantizer.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/keras_utils/separable_conv2d.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/keras_utils/separable_conv2d.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/mxnet.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/mxnet.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/mxnet.yaml` & `neural_compressor-2.5.1/neural_compressor/adaptor/mxnet.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/mxnet_utils/__init__.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/mxnet_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/mxnet_utils/util.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/mxnet_utils/util.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/onnxrt.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/onnxrt.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/onnxrt.yaml` & `neural_compressor-2.5.1/neural_compressor/adaptor/onnxrt.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/onnxrt_cuda.yaml` & `neural_compressor-2.5.1/neural_compressor/adaptor/onnxrt_cuda.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/onnxrt_dml.yaml` & `neural_compressor-2.5.1/neural_compressor/adaptor/onnxrt_dml.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/onnxrt_dnnl.yaml` & `neural_compressor-2.5.1/neural_compressor/adaptor/onnxrt_dnnl.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/onnxrt_trt.yaml` & `neural_compressor-2.5.1/neural_compressor/adaptor/onnxrt_trt.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/ox_utils/__init__.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/ox_utils/calibration.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/calibration.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/ox_utils/calibrator.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/calibrator.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/ox_utils/operators/__init__.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/ox_utils/operators/activation.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/operators/activation.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/ox_utils/operators/argmax.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/operators/argmax.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/ox_utils/operators/attention.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/operators/attention.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/ox_utils/operators/binary_op.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/operators/binary_op.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/ox_utils/operators/concat.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/operators/concat.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/ox_utils/operators/conv.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/operators/conv.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/ox_utils/operators/direct_q8.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/operators/direct_q8.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/ox_utils/operators/embed_layernorm.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/operators/embed_layernorm.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/ox_utils/operators/gather.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/operators/gather.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/ox_utils/operators/gavgpool.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/operators/gavgpool.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/ox_utils/operators/gemm.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/operators/gemm.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/ox_utils/operators/lstm.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/operators/lstm.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/ox_utils/operators/matmul.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/operators/matmul.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/ox_utils/operators/maxpool.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/operators/maxpool.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/ox_utils/operators/norm.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/operators/norm.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/ox_utils/operators/ops.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/operators/ops.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/ox_utils/operators/pad.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/operators/pad.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/ox_utils/operators/pooling.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/operators/pooling.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/ox_utils/operators/reduce.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/operators/reduce.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/ox_utils/operators/resize.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/operators/resize.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/ox_utils/operators/split.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/operators/split.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/ox_utils/operators/unary_op.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/operators/unary_op.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/ox_utils/quantizer.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/quantizer.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/ox_utils/smooth_quant.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/smooth_quant.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/ox_utils/util.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/util.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/ox_utils/weight_only.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/ox_utils/weight_only.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/pytorch.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/pytorch.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/pytorch_cpu.yaml` & `neural_compressor-2.5.1/neural_compressor/adaptor/pytorch_cpu.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/pytorch_gpu.yaml` & `neural_compressor-2.5.1/neural_compressor/adaptor/pytorch_gpu.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/pytorch_ipex.yaml` & `neural_compressor-2.5.1/neural_compressor/adaptor/pytorch_ipex.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/query.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/query.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tensorflow.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tensorflow.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tensorflow.yaml` & `neural_compressor-2.5.1/neural_compressor/adaptor/tensorflow.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tensorflow_itex.yaml` & `neural_compressor-2.5.1/neural_compressor/adaptor/tensorflow_itex.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/__init__.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_converter.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_converter.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_converter_without_calib.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_converter_without_calib.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/__init__.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/bf16/__init__.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/bf16/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/bf16/bf16_convert.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/bf16/bf16_convert.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/bf16/dequantize_cast_optimizer.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/bf16/dequantize_cast_optimizer.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/__init__.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/convert_add_to_biasadd.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/convert_add_to_biasadd.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/convert_layout.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/convert_layout.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/convert_leakyrelu.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/convert_leakyrelu.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/convert_nan_to_random.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/convert_nan_to_random.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/convert_placeholder_to_const.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/convert_placeholder_to_const.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/dilated_contraction.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/dilated_contraction.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/dummy_biasadd.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/dummy_biasadd.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/expanddims_optimizer.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/expanddims_optimizer.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fetch_weight_from_reshape.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fetch_weight_from_reshape.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fold_batch_norm.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fold_batch_norm.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fold_constant.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fold_constant.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_biasadd_add.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_biasadd_add.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_column_wise_mul.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_column_wise_mul.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_conv_with_math.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_conv_with_math.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_decomposed_bn.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_decomposed_bn.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_decomposed_in.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_decomposed_in.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_gelu.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_gelu.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_layer_norm.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_layer_norm.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_pad_with_conv.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_pad_with_conv.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_pad_with_fp32_conv.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_pad_with_fp32_conv.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_reshape_transpose.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_reshape_transpose.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/graph_cse_optimizer.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/graph_cse_optimizer.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/grappler_pass.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/grappler_pass.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/insert_print_node.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/insert_print_node.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/move_squeeze_after_relu.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/move_squeeze_after_relu.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/pre_optimize.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/pre_optimize.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/remove_training_nodes.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/remove_training_nodes.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/rename_batch_norm.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/rename_batch_norm.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/split_shared_input.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/split_shared_input.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/strip_equivalent_nodes.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/strip_equivalent_nodes.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/strip_unused_nodes.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/strip_unused_nodes.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/switch_optimizer.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/switch_optimizer.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/graph_base.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/graph_base.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/__init__.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/freeze_fake_quant.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/freeze_fake_quant.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/freeze_value.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/freeze_value.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/freeze_value_without_calib.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/freeze_value_without_calib.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/fuse_conv_redundant_dequantize.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/fuse_conv_redundant_dequantize.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/fuse_conv_requantize.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/fuse_conv_requantize.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/fuse_matmul_redundant_dequantize.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/fuse_matmul_redundant_dequantize.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/fuse_matmul_requantize.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/fuse_matmul_requantize.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/meta_op_optimizer.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/meta_op_optimizer.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/post_hostconst_converter.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/post_hostconst_converter.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/post_quantized_op_cse.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/post_quantized_op_cse.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/rnn_convert.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/rnn_convert.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/scale_propagation.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/scale_propagation.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/onnx/__init__.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/onnx/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/onnx/onnx_graph.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/onnx/onnx_graph.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/onnx/onnx_node.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/onnx/onnx_node.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/onnx/onnx_schema.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/onnx/onnx_schema.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/onnx/tf2onnx_utils.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/onnx/tf2onnx_utils.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/qdq/__init__.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/qdq/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/qdq/insert_qdq_pattern.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/qdq/insert_qdq_pattern.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/qdq/merge_duplicated_qdq.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/qdq/merge_duplicated_qdq.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_rewriter/qdq/share_qdq_y_pattern.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_rewriter/qdq/share_qdq_y_pattern.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/graph_util.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/graph_util.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/__init__.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/qat/__init__.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/qat/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/qat/fake_quantize.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/qat/fake_quantize.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_config.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_config.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_helper.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_helper.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_layers/__init__.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_layers/optimize_layer.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_layers/optimize_layer.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_layers/quantize_layer_add.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_layers/quantize_layer_add.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_layers/quantize_layer_base.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_layers/quantize_layer_base.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_layers/quantize_layer_bn.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_layers/quantize_layer_bn.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_wrapper.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_wrapper.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/__init__.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_bn.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_bn.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_concatv2.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_concatv2.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_conv.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_conv.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_deconv.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_deconv.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_in.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_in.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_matmul.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_matmul.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_pooling.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_pooling.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/optimize_qdq.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/optimize_qdq.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_base.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_base.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_bn.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_bn.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_concatv2.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_concatv2.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_conv.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_conv.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_for_intel_cpu.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_for_intel_cpu.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_matmul.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_matmul.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_pooling.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_pooling.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/quantize_graph_common.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/quantize_graph_common.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/smooth_quant_calibration.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/smooth_quant_calibration.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/smooth_quant_scaler.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/smooth_quant_scaler.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/tf2onnx_converter.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/tf2onnx_converter.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/transform_graph/__init__.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/transform_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/transform_graph/bias_correction.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/transform_graph/bias_correction.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/transform_graph/graph_transform_base.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/transform_graph/graph_transform_base.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/transform_graph/insert_logging.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/transform_graph/insert_logging.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/transform_graph/rerange_quantized_concat.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/transform_graph/rerange_quantized_concat.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/tf_utils/util.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/tf_utils/util.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/torch_utils/__init__.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/torch_utils/auto_round.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/auto_round.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/torch_utils/autoround/__init__.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/autoround/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/torch_utils/autoround/autoround.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/autoround/autoround.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/torch_utils/autoround/export.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/autoround/export.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/torch_utils/autoround/model_wrapper.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/autoround/model_wrapper.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/torch_utils/autoround/sign_sgd.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/autoround/sign_sgd.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/torch_utils/awq.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/awq.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/torch_utils/bf16_convert.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/bf16_convert.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/torch_utils/gptq.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/gptq.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/torch_utils/hawq_metric.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/hawq_metric.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/torch_utils/layer_wise_quant/__init__.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/layer_wise_quant/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/torch_utils/layer_wise_quant/modified_pickle.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/layer_wise_quant/modified_pickle.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/torch_utils/layer_wise_quant/quantize.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/layer_wise_quant/quantize.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/torch_utils/layer_wise_quant/torch_load.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/layer_wise_quant/torch_load.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/torch_utils/layer_wise_quant/utils.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/layer_wise_quant/utils.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/torch_utils/mixed_precision.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/torch_utils/model_wrapper.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/model_wrapper.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/torch_utils/pattern_detector.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/pattern_detector.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/torch_utils/symbolic_trace.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/symbolic_trace.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/torch_utils/teq.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/teq.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/torch_utils/util.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/util.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/torch_utils/waq/__init__.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/waq/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/torch_utils/waq/auto_alpha.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/waq/auto_alpha.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/torch_utils/waq/calibration.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/waq/calibration.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/torch_utils/waq/graph_trace.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/waq/graph_trace.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/torch_utils/waq/smooth_quant.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/waq/smooth_quant.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/torch_utils/waq/utils.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/waq/utils.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/adaptor/torch_utils/weight_only.py` & `neural_compressor-2.5.1/neural_compressor/adaptor/torch_utils/weight_only.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,15 +172,15 @@
     else:
         scale = wmax / maxq
     scale.unsqueeze_(dim=-1)
     weight.div_(scale)
     weight.round_()
     weight.clamp_(minq, maxq)
     if return_int:
-        return weight, scale.type(torch.float), None
+        return weight, scale, None
     return weight.mul_(scale)
 
 
 def qdq_weight_actor(weight, num_bits, scheme, quantile=1.0, data_type="int", return_int=False, full_range=False):
     """Quant and dequant tensor per channel.
 
     Args:
@@ -234,37 +234,42 @@
             return_int=return_int,
             full_range=full_range,
             data_type=data_type,
         )
 
     orig_shape = weight.shape
     if weight.shape[1] % group_size == 0:
+        orig_weight = weight
         weight = weight.reshape(-1, group_size)
         if return_int:
             weight, scale, zp = qdq_weight_actor(
                 weight,
                 num_bits,
                 scheme=scheme,
                 quantile=quantile,
                 return_int=True,
                 full_range=full_range,
                 data_type=data_type,
             )
             weight = weight.reshape(orig_shape)
+            orig_weight.copy_(weight)
             scale = scale.reshape(orig_shape[0], -1)
             if zp is not None:
                 zp = zp.reshape(orig_shape[0], -1)
-            return weight, scale, zp
+            return orig_weight, scale, zp
         else:
             qdq_weight_actor(
                 weight, num_bits, scheme=scheme, data_type=data_type, quantile=quantile, full_range=full_range
             )
-            return weight.reshape(orig_shape)
+            weight = weight.reshape(orig_shape)
+            orig_weight.copy_(weight)
+            return orig_weight
     else:
         split_index = weight.shape[1] // group_size * group_size
+        orig_weight = weight
         weight1 = weight[:, :split_index]
         weight1 = weight1.reshape(-1, group_size)
         if return_int:
             weight1, scale1, zp1 = qdq_weight_actor(
                 weight1,
                 num_bits,
                 scheme=scheme,
@@ -273,42 +278,42 @@
                 return_int=True,
                 full_range=full_range,
             )
             scale1 = scale1.reshape(orig_shape[0], -1)
             if zp1 is not None:
                 zp1 = zp1.reshape(orig_shape[0], -1)
         else:
-            weight1 = qdq_weight_actor(
+            qdq_weight_actor(
                 weight1, num_bits, scheme=scheme, quantile=quantile, data_type=data_type, full_range=full_range
             )
         weight1 = weight1.reshape(orig_shape[0], split_index)
         weight2 = weight[:, split_index:]
         if return_int:
             weight2, scale2, zp2 = qdq_weight_actor(
                 weight2,
                 num_bits,
                 scheme=scheme,
                 data_type=data_type,
                 quantile=quantile,
                 return_int=True,
                 full_range=full_range,
             )
-            weight.copy_(torch.cat([weight1, weight2], dim=1))
+            orig_weight.copy_(torch.cat([weight1, weight2], dim=1))
             scale = torch.cat([scale1, scale2], dim=1)
             if zp2 is not None:
                 zp = torch.cat([zp1, zp2], dim=1)
             else:
                 zp = None
-            return weight, scale, zp
+            return orig_weight, scale, zp
         else:
             weight2 = qdq_weight_actor(
                 weight2, num_bits, scheme=scheme, data_type=data_type, quantile=quantile, full_range=full_range
             )
-            weight.copy_(torch.cat([weight1, weight2], dim=1))
-            return weight
+            orig_weight.copy_(torch.cat([weight1, weight2], dim=1))
+            return orig_weight
 
 
 def search_clip(m, num_bits=4, group_size=32, scheme="asym", data_type="int", enable_full_range=False):
     """Search best clip range of each linears in current block.
 
     Args:
         m (torch.nn.Module): torch module.
@@ -394,24 +399,24 @@
         group_dim (int, optional):   0 means splitting output channel,
                                      1 means splitting input channel. Defaults to 1.
 
     Returns:
         model: fake quantized torch module
     """
     assert isinstance(model, torch.nn.Module), "only support torch module"
-    supported_layers = ["Linear"]
+    supported_layers = (torch.nn.Linear,)
     if return_int:
         compression_dtype = kwargs.get("compression_dtype", torch.int32)
         compression_dim = kwargs.get("compression_dim", 1)
         scale_dtype = kwargs.get("scale_dtype", torch.float32)
         device = kwargs.get("device", "cpu")
         use_optimum_format = kwargs.get("use_optimum_format", True)
     with torch.no_grad():
         for name, m in model.named_modules():
-            if m.__class__.__name__ not in supported_layers:
+            if not isinstance(m, supported_layers):
                 continue
             orig_dtype = next(m.parameters()).dtype
             if orig_dtype != torch.float:
                 m = m.float()
             if name in weight_config:  # pragma: no cover
                 num_bits = weight_config[name]["bits"]
                 group_size = weight_config[name]["group_size"]
```

### Comparing `neural_compressor-2.5/neural_compressor/algorithm/__init__.py` & `neural_compressor-2.5.1/neural_compressor/algorithm/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/algorithm/algorithm.py` & `neural_compressor-2.5.1/neural_compressor/algorithm/algorithm.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/algorithm/fast_bias_correction.py` & `neural_compressor-2.5.1/neural_compressor/algorithm/fast_bias_correction.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/algorithm/smooth_quant.py` & `neural_compressor-2.5.1/neural_compressor/algorithm/smooth_quant.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/algorithm/weight_correction.py` & `neural_compressor-2.5.1/neural_compressor/algorithm/weight_correction.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/benchmark.py` & `neural_compressor-2.5.1/neural_compressor/benchmark.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/compression/__init__.py` & `neural_compressor-2.5.1/neural_compressor/compression/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/compression/callbacks.py` & `neural_compressor-2.5.1/neural_compressor/compression/callbacks.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/compression/distillation/__init__.py` & `neural_compressor-2.5.1/neural_compressor/compression/distillation/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/compression/distillation/criterions.py` & `neural_compressor-2.5.1/neural_compressor/compression/distillation/criterions.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/compression/distillation/optimizers.py` & `neural_compressor-2.5.1/neural_compressor/compression/distillation/optimizers.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/compression/distillation/utility.py` & `neural_compressor-2.5.1/neural_compressor/compression/distillation/utility.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/compression/hpo/__init__.py` & `neural_compressor-2.5.1/neural_compressor/compression/hpo/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/compression/hpo/sa_optimizer.py` & `neural_compressor-2.5.1/neural_compressor/compression/hpo/sa_optimizer.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/compression/hpo/search_algorithms.py` & `neural_compressor-2.5.1/neural_compressor/compression/hpo/search_algorithms.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/compression/hpo/search_space.py` & `neural_compressor-2.5.1/neural_compressor/compression/hpo/search_space.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/compression/pruner/__init__.py` & `neural_compressor-2.5.1/neural_compressor/compression/pruner/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/compression/pruner/criteria.py` & `neural_compressor-2.5.1/neural_compressor/compression/pruner/criteria.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/compression/pruner/dsnot.py` & `neural_compressor-2.5.1/neural_compressor/compression/pruner/dsnot.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/compression/pruner/model_slim/__init__.py` & `neural_compressor-2.5.1/neural_compressor/compression/pruner/model_slim/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/compression/pruner/model_slim/auto_slim.py` & `neural_compressor-2.5.1/neural_compressor/compression/pruner/model_slim/auto_slim.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/compression/pruner/model_slim/pattern_analyzer.py` & `neural_compressor-2.5.1/neural_compressor/compression/pruner/model_slim/pattern_analyzer.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/compression/pruner/model_slim/weight_slim.py` & `neural_compressor-2.5.1/neural_compressor/compression/pruner/model_slim/weight_slim.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/compression/pruner/patterns/__init__.py` & `neural_compressor-2.5.1/neural_compressor/compression/pruner/patterns/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/compression/pruner/patterns/base.py` & `neural_compressor-2.5.1/neural_compressor/compression/pruner/patterns/base.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/compression/pruner/patterns/mha.py` & `neural_compressor-2.5.1/neural_compressor/compression/pruner/patterns/mha.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/compression/pruner/patterns/ninm.py` & `neural_compressor-2.5.1/neural_compressor/compression/pruner/patterns/ninm.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/compression/pruner/patterns/nxm.py` & `neural_compressor-2.5.1/neural_compressor/compression/pruner/patterns/nxm.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/compression/pruner/pruners/__init__.py` & `neural_compressor-2.5.1/neural_compressor/compression/pruner/pruners/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/compression/pruner/pruners/base.py` & `neural_compressor-2.5.1/neural_compressor/compression/pruner/pruners/base.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/compression/pruner/pruners/basic.py` & `neural_compressor-2.5.1/neural_compressor/compression/pruner/pruners/basic.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/compression/pruner/pruners/block_mask.py` & `neural_compressor-2.5.1/neural_compressor/compression/pruner/pruners/block_mask.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/compression/pruner/pruners/mha.py` & `neural_compressor-2.5.1/neural_compressor/compression/pruner/pruners/mha.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/compression/pruner/pruners/pattern_lock.py` & `neural_compressor-2.5.1/neural_compressor/compression/pruner/pruners/pattern_lock.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/compression/pruner/pruners/progressive.py` & `neural_compressor-2.5.1/neural_compressor/compression/pruner/pruners/progressive.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/compression/pruner/pruners/retrain_free.py` & `neural_compressor-2.5.1/neural_compressor/compression/pruner/pruners/retrain_free.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/compression/pruner/pruners/sparse_gpt.py` & `neural_compressor-2.5.1/neural_compressor/compression/pruner/pruners/sparse_gpt.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/compression/pruner/pruning.py` & `neural_compressor-2.5.1/neural_compressor/compression/pruner/pruning.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/compression/pruner/regs.py` & `neural_compressor-2.5.1/neural_compressor/compression/pruner/regs.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/compression/pruner/schedulers.py` & `neural_compressor-2.5.1/neural_compressor/compression/pruner/schedulers.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/compression/pruner/tf_criteria.py` & `neural_compressor-2.5.1/neural_compressor/compression/pruner/tf_criteria.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/compression/pruner/utils.py` & `neural_compressor-2.5.1/neural_compressor/compression/pruner/utils.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/compression/pruner/wanda/__init__.py` & `neural_compressor-2.5.1/neural_compressor/compression/pruner/wanda/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/compression/pruner/wanda/prune.py` & `neural_compressor-2.5.1/neural_compressor/compression/pruner/wanda/prune.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/compression/pruner/wanda/utils.py` & `neural_compressor-2.5.1/neural_compressor/compression/pruner/wanda/utils.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/compression/pruner/wanda/wrapper.py` & `neural_compressor-2.5.1/neural_compressor/compression/pruner/wanda/wrapper.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/conf/__init__.py` & `neural_compressor-2.5.1/neural_compressor/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/conf/config.py` & `neural_compressor-2.5.1/neural_compressor/conf/config.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/conf/dotdict.py` & `neural_compressor-2.5.1/neural_compressor/conf/dotdict.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/conf/pythonic_config.py` & `neural_compressor-2.5.1/neural_compressor/conf/pythonic_config.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/config.py` & `neural_compressor-2.5.1/neural_compressor/config.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/contrib/__init__.py` & `neural_compressor-2.5.1/neural_compressor/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/contrib/strategy/__init__.py` & `neural_compressor-2.5.1/neural_compressor/contrib/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/contrib/strategy/sigopt.py` & `neural_compressor-2.5.1/neural_compressor/contrib/strategy/sigopt.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/contrib/strategy/tpe.py` & `neural_compressor-2.5.1/neural_compressor/contrib/strategy/tpe.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/data/__init__.py` & `neural_compressor-2.5.1/neural_compressor/data/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/data/dataloaders/__init__.py` & `neural_compressor-2.5.1/neural_compressor/data/dataloaders/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/data/dataloaders/base_dataloader.py` & `neural_compressor-2.5.1/neural_compressor/data/dataloaders/base_dataloader.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/data/dataloaders/dataloader.py` & `neural_compressor-2.5.1/neural_compressor/data/dataloaders/dataloader.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/data/dataloaders/default_dataloader.py` & `neural_compressor-2.5.1/neural_compressor/data/dataloaders/default_dataloader.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/data/dataloaders/fetcher.py` & `neural_compressor-2.5.1/neural_compressor/data/dataloaders/fetcher.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/data/dataloaders/mxnet_dataloader.py` & `neural_compressor-2.5.1/neural_compressor/data/dataloaders/mxnet_dataloader.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/data/dataloaders/onnxrt_dataloader.py` & `neural_compressor-2.5.1/neural_compressor/data/dataloaders/onnxrt_dataloader.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/data/dataloaders/pytorch_dataloader.py` & `neural_compressor-2.5.1/neural_compressor/data/dataloaders/pytorch_dataloader.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/data/dataloaders/sampler.py` & `neural_compressor-2.5.1/neural_compressor/data/dataloaders/sampler.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/data/dataloaders/tensorflow_dataloader.py` & `neural_compressor-2.5.1/neural_compressor/data/dataloaders/tensorflow_dataloader.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/data/datasets/__init__.py` & `neural_compressor-2.5.1/neural_compressor/data/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/data/datasets/bert_dataset.py` & `neural_compressor-2.5.1/neural_compressor/data/datasets/bert_dataset.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/data/datasets/coco_dataset.py` & `neural_compressor-2.5.1/neural_compressor/data/datasets/coco_dataset.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/data/datasets/dataset.py` & `neural_compressor-2.5.1/neural_compressor/data/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/data/datasets/dummy_dataset.py` & `neural_compressor-2.5.1/neural_compressor/data/datasets/dummy_dataset.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/data/datasets/dummy_dataset_v2.py` & `neural_compressor-2.5.1/neural_compressor/data/datasets/dummy_dataset_v2.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/data/datasets/imagenet_dataset.py` & `neural_compressor-2.5.1/neural_compressor/data/datasets/imagenet_dataset.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/data/datasets/style_transfer_dataset.py` & `neural_compressor-2.5.1/neural_compressor/data/datasets/style_transfer_dataset.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/data/filters/__init__.py` & `neural_compressor-2.5.1/neural_compressor/data/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/data/filters/coco_filter.py` & `neural_compressor-2.5.1/neural_compressor/data/filters/coco_filter.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/data/filters/filter.py` & `neural_compressor-2.5.1/neural_compressor/data/filters/filter.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/data/transforms/__init__.py` & `neural_compressor-2.5.1/neural_compressor/data/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/data/transforms/coco_transform.py` & `neural_compressor-2.5.1/neural_compressor/data/transforms/coco_transform.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/data/transforms/imagenet_transform.py` & `neural_compressor-2.5.1/neural_compressor/data/transforms/imagenet_transform.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/data/transforms/postprocess.py` & `neural_compressor-2.5.1/neural_compressor/data/transforms/postprocess.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/data/transforms/tokenization.py` & `neural_compressor-2.5.1/neural_compressor/data/transforms/tokenization.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/data/transforms/transform.py` & `neural_compressor-2.5.1/neural_compressor/data/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/__init__.py` & `neural_compressor-2.5.1/neural_compressor/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/benchmark.py` & `neural_compressor-2.5.1/neural_compressor/experimental/benchmark.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/common/__init__.py` & `neural_compressor-2.5.1/neural_compressor/experimental/common/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/common/criterion.py` & `neural_compressor-2.5.1/neural_compressor/experimental/common/criterion.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/common/dataloader.py` & `neural_compressor-2.5.1/neural_compressor/experimental/common/dataloader.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/common/metric.py` & `neural_compressor-2.5.1/neural_compressor/experimental/common/metric.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/common/model.py` & `neural_compressor-2.5.1/neural_compressor/experimental/common/model.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/common/optimizer.py` & `neural_compressor-2.5.1/neural_compressor/experimental/common/optimizer.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/common/postprocess.py` & `neural_compressor-2.5.1/neural_compressor/experimental/common/postprocess.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/common/torch_utils.py` & `neural_compressor-2.5.1/neural_compressor/experimental/common/torch_utils.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/component.py` & `neural_compressor-2.5.1/neural_compressor/experimental/component.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/compression/__init__.py` & `neural_compressor-2.5.1/neural_compressor/experimental/compression/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/contrib/__init__.py` & `neural_compressor-2.5.1/neural_compressor/experimental/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/contrib/strategy/__init__.py` & `neural_compressor-2.5.1/neural_compressor/experimental/contrib/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/contrib/strategy/sigopt.py` & `neural_compressor-2.5.1/neural_compressor/experimental/contrib/strategy/sigopt.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/contrib/strategy/tpe.py` & `neural_compressor-2.5.1/neural_compressor/experimental/contrib/strategy/tpe.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/data/__init__.py` & `neural_compressor-2.5.1/neural_compressor/experimental/data/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/data/dataloaders/__init__.py` & `neural_compressor-2.5.1/neural_compressor/experimental/data/dataloaders/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/data/dataloaders/base_dataloader.py` & `neural_compressor-2.5.1/neural_compressor/experimental/data/dataloaders/base_dataloader.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/data/dataloaders/dataloader.py` & `neural_compressor-2.5.1/neural_compressor/experimental/data/dataloaders/dataloader.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/data/dataloaders/default_dataloader.py` & `neural_compressor-2.5.1/neural_compressor/experimental/data/dataloaders/default_dataloader.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/data/dataloaders/fetcher.py` & `neural_compressor-2.5.1/neural_compressor/experimental/data/dataloaders/fetcher.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/data/dataloaders/mxnet_dataloader.py` & `neural_compressor-2.5.1/neural_compressor/experimental/data/dataloaders/mxnet_dataloader.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/data/dataloaders/onnxrt_dataloader.py` & `neural_compressor-2.5.1/neural_compressor/experimental/data/dataloaders/onnxrt_dataloader.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/data/dataloaders/pytorch_dataloader.py` & `neural_compressor-2.5.1/neural_compressor/experimental/data/dataloaders/pytorch_dataloader.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/data/dataloaders/sampler.py` & `neural_compressor-2.5.1/neural_compressor/experimental/data/dataloaders/sampler.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/data/dataloaders/tensorflow_dataloader.py` & `neural_compressor-2.5.1/neural_compressor/experimental/data/dataloaders/tensorflow_dataloader.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/data/datasets/__init__.py` & `neural_compressor-2.5.1/neural_compressor/experimental/data/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/data/datasets/bert_dataset.py` & `neural_compressor-2.5.1/neural_compressor/experimental/data/datasets/bert_dataset.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/data/datasets/coco_dataset.py` & `neural_compressor-2.5.1/neural_compressor/experimental/data/datasets/coco_dataset.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/data/datasets/dataset.py` & `neural_compressor-2.5.1/neural_compressor/experimental/data/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/data/datasets/dummy_dataset.py` & `neural_compressor-2.5.1/neural_compressor/experimental/data/datasets/dummy_dataset.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/data/datasets/dummy_dataset_v2.py` & `neural_compressor-2.5.1/neural_compressor/experimental/data/datasets/dummy_dataset_v2.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/data/datasets/imagenet_dataset.py` & `neural_compressor-2.5.1/neural_compressor/experimental/data/datasets/imagenet_dataset.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/data/datasets/style_transfer_dataset.py` & `neural_compressor-2.5.1/neural_compressor/experimental/data/datasets/style_transfer_dataset.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/data/filters/__init__.py` & `neural_compressor-2.5.1/neural_compressor/experimental/data/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/data/filters/coco_filter.py` & `neural_compressor-2.5.1/neural_compressor/experimental/data/filters/coco_filter.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/data/filters/filter.py` & `neural_compressor-2.5.1/neural_compressor/experimental/data/filters/filter.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/data/transforms/__init__.py` & `neural_compressor-2.5.1/neural_compressor/experimental/data/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/data/transforms/imagenet_transform.py` & `neural_compressor-2.5.1/neural_compressor/experimental/data/transforms/imagenet_transform.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/data/transforms/tokenization.py` & `neural_compressor-2.5.1/neural_compressor/experimental/data/transforms/tokenization.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/data/transforms/transform.py` & `neural_compressor-2.5.1/neural_compressor/experimental/data/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/distillation.py` & `neural_compressor-2.5.1/neural_compressor/experimental/distillation.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/export/__init__.py` & `neural_compressor-2.5.1/neural_compressor/experimental/export/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/export/qlinear2qdq.py` & `neural_compressor-2.5.1/neural_compressor/experimental/export/qlinear2qdq.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/export/tf2onnx.py` & `neural_compressor-2.5.1/neural_compressor/experimental/export/tf2onnx.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/export/torch2onnx.py` & `neural_compressor-2.5.1/neural_compressor/experimental/export/torch2onnx.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/graph_optimization.py` & `neural_compressor-2.5.1/neural_compressor/experimental/graph_optimization.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/metric/__init__.py` & `neural_compressor-2.5.1/neural_compressor/experimental/metric/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/metric/bleu.py` & `neural_compressor-2.5.1/neural_compressor/experimental/metric/bleu.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/metric/bleu_util.py` & `neural_compressor-2.5.1/neural_compressor/experimental/metric/bleu_util.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/metric/coco_label_map.py` & `neural_compressor-2.5.1/neural_compressor/experimental/metric/coco_label_map.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/metric/coco_tools.py` & `neural_compressor-2.5.1/neural_compressor/experimental/metric/coco_tools.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/metric/evaluate_squad.py` & `neural_compressor-2.5.1/neural_compressor/experimental/metric/evaluate_squad.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/metric/f1.py` & `neural_compressor-2.5.1/neural_compressor/experimental/metric/f1.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/metric/metric.py` & `neural_compressor-2.5.1/neural_compressor/experimental/metric/metric.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/mixed_precision.py` & `neural_compressor-2.5.1/neural_compressor/experimental/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/model_conversion.py` & `neural_compressor-2.5.1/neural_compressor/experimental/model_conversion.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/nas/__init__.py` & `neural_compressor-2.5.1/neural_compressor/experimental/nas/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/nas/basic_nas.py` & `neural_compressor-2.5.1/neural_compressor/experimental/nas/basic_nas.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/nas/dynas.py` & `neural_compressor-2.5.1/neural_compressor/experimental/nas/dynas.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/nas/nas.py` & `neural_compressor-2.5.1/neural_compressor/experimental/nas/nas.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/nas/nas_utils.py` & `neural_compressor-2.5.1/neural_compressor/experimental/nas/nas_utils.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/nas/search_algorithms.py` & `neural_compressor-2.5.1/neural_compressor/experimental/nas/search_algorithms.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/pruner_legacy/__init__.py` & `neural_compressor-2.5.1/neural_compressor/experimental/pruner_legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/pruner_legacy/gradient_sensitivity.py` & `neural_compressor-2.5.1/neural_compressor/experimental/pruner_legacy/gradient_sensitivity.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/pruner_legacy/group_lasso.py` & `neural_compressor-2.5.1/neural_compressor/experimental/pruner_legacy/group_lasso.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/pruner_legacy/magnitude.py` & `neural_compressor-2.5.1/neural_compressor/experimental/pruner_legacy/magnitude.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/pruner_legacy/pattern_lock.py` & `neural_compressor-2.5.1/neural_compressor/experimental/pruner_legacy/pattern_lock.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/pruner_legacy/pruner.py` & `neural_compressor-2.5.1/neural_compressor/experimental/pruner_legacy/pruner.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/pruning.py` & `neural_compressor-2.5.1/neural_compressor/experimental/pruning.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/pruning_recipes/__init__.py` & `neural_compressor-2.5.1/neural_compressor/experimental/pruning_recipes/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/pruning_recipes/patterns/__init__.py` & `neural_compressor-2.5.1/neural_compressor/experimental/pruning_recipes/patterns/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/pruning_recipes/patterns/pattern.py` & `neural_compressor-2.5.1/neural_compressor/experimental/pruning_recipes/patterns/pattern.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/pruning_recipes/patterns/tile_pattern.py` & `neural_compressor-2.5.1/neural_compressor/experimental/pruning_recipes/patterns/tile_pattern.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/pruning_v2.py` & `neural_compressor-2.5.1/neural_compressor/experimental/pruning_v2.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/pytorch_pruner/__init__.py` & `neural_compressor-2.5.1/neural_compressor/experimental/pytorch_pruner/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/pytorch_pruner/logger.py` & `neural_compressor-2.5.1/neural_compressor/experimental/pytorch_pruner/logger.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/pytorch_pruner/patterns.py` & `neural_compressor-2.5.1/neural_compressor/experimental/pytorch_pruner/patterns.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/pytorch_pruner/prune_utils.py` & `neural_compressor-2.5.1/neural_compressor/experimental/pytorch_pruner/prune_utils.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/pytorch_pruner/pruner.py` & `neural_compressor-2.5.1/neural_compressor/experimental/pytorch_pruner/pruner.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/pytorch_pruner/pruning.py` & `neural_compressor-2.5.1/neural_compressor/experimental/pytorch_pruner/pruning.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/pytorch_pruner/scheduler.py` & `neural_compressor-2.5.1/neural_compressor/experimental/pytorch_pruner/scheduler.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/quantization.py` & `neural_compressor-2.5.1/neural_compressor/experimental/quantization.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/scheduler.py` & `neural_compressor-2.5.1/neural_compressor/experimental/scheduler.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/strategy/__init__.py` & `neural_compressor-2.5.1/neural_compressor/experimental/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/strategy/auto_mixed_precision.py` & `neural_compressor-2.5.1/neural_compressor/experimental/strategy/auto_mixed_precision.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/strategy/basic.py` & `neural_compressor-2.5.1/neural_compressor/experimental/strategy/basic.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/strategy/bayesian.py` & `neural_compressor-2.5.1/neural_compressor/experimental/strategy/bayesian.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/strategy/exhaustive.py` & `neural_compressor-2.5.1/neural_compressor/experimental/strategy/exhaustive.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/strategy/mse.py` & `neural_compressor-2.5.1/neural_compressor/experimental/strategy/mse.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/strategy/mse_v2.py` & `neural_compressor-2.5.1/neural_compressor/experimental/strategy/mse_v2.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/strategy/random.py` & `neural_compressor-2.5.1/neural_compressor/experimental/strategy/random.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/strategy/strategy.py` & `neural_compressor-2.5.1/neural_compressor/experimental/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/strategy/utils/__init__.py` & `neural_compressor-2.5.1/neural_compressor/experimental/strategy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/strategy/utils/constant.py` & `neural_compressor-2.5.1/neural_compressor/experimental/strategy/utils/constant.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/strategy/utils/tuning_sampler.py` & `neural_compressor-2.5.1/neural_compressor/experimental/strategy/utils/tuning_sampler.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/strategy/utils/tuning_space.py` & `neural_compressor-2.5.1/neural_compressor/experimental/strategy/utils/tuning_space.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/strategy/utils/tuning_structs.py` & `neural_compressor-2.5.1/neural_compressor/experimental/strategy/utils/tuning_structs.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/experimental/strategy/utils/utility.py` & `neural_compressor-2.5.1/neural_compressor/experimental/strategy/utils/utility.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/metric/__init__.py` & `neural_compressor-2.5.1/neural_compressor/metric/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/metric/bleu.py` & `neural_compressor-2.5.1/neural_compressor/metric/bleu.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/metric/bleu_util.py` & `neural_compressor-2.5.1/neural_compressor/metric/bleu_util.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/metric/coco_label_map.py` & `neural_compressor-2.5.1/neural_compressor/metric/coco_label_map.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/metric/coco_tools.py` & `neural_compressor-2.5.1/neural_compressor/metric/coco_tools.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/metric/evaluate_squad.py` & `neural_compressor-2.5.1/neural_compressor/metric/evaluate_squad.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/metric/f1.py` & `neural_compressor-2.5.1/neural_compressor/metric/f1.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/metric/metric.py` & `neural_compressor-2.5.1/neural_compressor/metric/metric.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/mix_precision.py` & `neural_compressor-2.5.1/neural_compressor/mix_precision.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/model/__init__.py` & `neural_compressor-2.5.1/neural_compressor/model/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/model/base_model.py` & `neural_compressor-2.5.1/neural_compressor/model/base_model.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/model/keras_model.py` & `neural_compressor-2.5.1/neural_compressor/model/keras_model.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/model/model.py` & `neural_compressor-2.5.1/neural_compressor/model/model.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/model/mxnet_model.py` & `neural_compressor-2.5.1/neural_compressor/model/mxnet_model.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/model/nets_factory.py` & `neural_compressor-2.5.1/neural_compressor/model/nets_factory.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/model/onnx_model.py` & `neural_compressor-2.5.1/neural_compressor/model/onnx_model.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/model/tensorflow_model.py` & `neural_compressor-2.5.1/neural_compressor/model/tensorflow_model.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/model/torch_model.py` & `neural_compressor-2.5.1/neural_compressor/model/torch_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -494,15 +494,14 @@
         if gptq_config_path is not None:
             with open(gptq_config_path, "r") as f:
                 gptq_config = json.load(f)
         else:
             gptq_config = self.gptq_config if hasattr(self, "gptq_config") else {}
 
         autoround_config = self.autoround_config if hasattr(self, "autoround_config") else {}
-
         if gptq_config:
             for k, v in weight_config.items():
                 logger.debug(f"Compressing {k} on device {device}")
                 if v["dtype"] == "fp32":
                     continue
                 else:
                     dtype = v["dtype"]
@@ -555,26 +554,61 @@
                     scale_dtype=scale_dtype,
                     device=device,
                     use_optimum_format=use_optimum_format,
                 )
                 new_module.pack(int_weight, gptq_scale, gptq_zp, m.bias, gptq_perm)
                 set_module(self.model, k, new_module)
         elif autoround_config:
-            from auto_round.export.export_to_itrex.export import pack_model  # pylint: disable=E0401
+            if device == "xpu":
+                for k, v in weight_config.items():
+                    logger.debug(f"Compressing {k} on device {device}")
+                    if v["dtype"] == "fp32":
+                        continue
+                    else:
+                        dtype = v["dtype"]
+                        num_bits = v["bits"]
+                        group_size = v["group_size"]
+                        scheme = v["scheme"]
+                    m = fetch_module(self.model, k)
+                    autoround_conf = autoround_config[k]
+                    fp32_weight = m.weight.data
+                    autoround_scale = torch.tensor(autoround_conf["scale"], dtype=torch.float32)
+                    autoround_zp = None if scheme == "sym" else torch.tensor(autoround_conf["zero"], dtype=torch.int32)
+                    int_weight = quant_weight_w_scale(fp32_weight, autoround_scale, autoround_zp, group_size)
+                    int_weight = int_weight.type(torch.int32)
+                    new_module = WeightOnlyLinear(
+                        m.in_features,
+                        m.out_features,
+                        num_bits,
+                        group_size,
+                        dtype=dtype,
+                        zp=autoround_zp is not None,
+                        bias=m.bias is not None,
+                        g_idx=None,
+                        compression_dtype=compression_dtype,
+                        compression_dim=compression_dim,
+                        scale_dtype=scale_dtype,
+                        device=device,
+                        use_optimum_format=use_optimum_format,
+                    )
+                    new_module.pack(int_weight, autoround_scale, autoround_zp, m.bias, None)
+                    set_module(self.model, k, new_module)
+            else:
+                from auto_round.export.export_to_itrex.export import pack_model  # pylint: disable=E0401
 
-            self.model = pack_model(
-                self.model,
-                weight_config=autoround_config,
-                enable_full_range=enable_full_range,
-                compression_dtype=compression_dtype,
-                compression_dim=compression_dim,
-                device=device,
-                use_optimum_format=use_optimum_format,
-                inplace=True,
-            )
+                self.model = pack_model(
+                    self.model,
+                    weight_config=autoround_config,
+                    enable_full_range=enable_full_range,
+                    compression_dtype=compression_dtype,
+                    compression_dim=compression_dim,
+                    device=device,
+                    use_optimum_format=use_optimum_format,
+                    inplace=True,
+                )
         else:
             for k, v in weight_config.items():
                 logger.debug(f"Compressing {k} on device {device}")
                 if v["dtype"] == "fp32":
                     continue
                 else:
                     dtype = v["dtype"]
```

### Comparing `neural_compressor-2.5/neural_compressor/objective.py` & `neural_compressor-2.5.1/neural_compressor/objective.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/profiling/__init__.py` & `neural_compressor-2.5.1/neural_compressor/profiling/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/profiling/parser/__init__.py` & `neural_compressor-2.5.1/neural_compressor/profiling/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/profiling/parser/factory.py` & `neural_compressor-2.5.1/neural_compressor/profiling/parser/factory.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/profiling/parser/onnx_parser/__init__.py` & `neural_compressor-2.5.1/neural_compressor/profiling/parser/onnx_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/profiling/parser/onnx_parser/factory.py` & `neural_compressor-2.5.1/neural_compressor/profiling/parser/onnx_parser/factory.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/profiling/parser/onnx_parser/parser.py` & `neural_compressor-2.5.1/neural_compressor/profiling/parser/onnx_parser/parser.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/profiling/parser/parser.py` & `neural_compressor-2.5.1/neural_compressor/profiling/parser/parser.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/profiling/parser/result.py` & `neural_compressor-2.5.1/neural_compressor/profiling/parser/result.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/profiling/parser/tensorflow_parser/__init__.py` & `neural_compressor-2.5.1/neural_compressor/profiling/parser/tensorflow_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/profiling/parser/tensorflow_parser/factory.py` & `neural_compressor-2.5.1/neural_compressor/profiling/parser/tensorflow_parser/factory.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/profiling/parser/tensorflow_parser/parser.py` & `neural_compressor-2.5.1/neural_compressor/profiling/parser/tensorflow_parser/parser.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/profiling/profiler/__init__.py` & `neural_compressor-2.5.1/neural_compressor/profiling/profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/profiling/profiler/factory.py` & `neural_compressor-2.5.1/neural_compressor/profiling/profiler/factory.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/profiling/profiler/onnxrt_profiler/__init__.py` & `neural_compressor-2.5.1/neural_compressor/profiling/profiler/onnxrt_profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/profiling/profiler/onnxrt_profiler/factory.py` & `neural_compressor-2.5.1/neural_compressor/profiling/profiler/onnxrt_profiler/factory.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/profiling/profiler/onnxrt_profiler/profiler.py` & `neural_compressor-2.5.1/neural_compressor/profiling/profiler/onnxrt_profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/profiling/profiler/onnxrt_profiler/utils.py` & `neural_compressor-2.5.1/neural_compressor/profiling/profiler/onnxrt_profiler/utils.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/profiling/profiler/profiler.py` & `neural_compressor-2.5.1/neural_compressor/profiling/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/profiling/profiler/tensorflow_profiler/__init__.py` & `neural_compressor-2.5.1/neural_compressor/profiling/profiler/tensorflow_profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/profiling/profiler/tensorflow_profiler/factory.py` & `neural_compressor-2.5.1/neural_compressor/profiling/profiler/tensorflow_profiler/factory.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/profiling/profiler/tensorflow_profiler/profiler.py` & `neural_compressor-2.5.1/neural_compressor/profiling/profiler/tensorflow_profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/profiling/profiler/tensorflow_profiler/utils.py` & `neural_compressor-2.5.1/neural_compressor/profiling/profiler/tensorflow_profiler/utils.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/quantization.py` & `neural_compressor-2.5.1/neural_compressor/quantization.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/strategy/__init__.py` & `neural_compressor-2.5.1/neural_compressor/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/strategy/auto.py` & `neural_compressor-2.5.1/neural_compressor/strategy/auto.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/strategy/auto_mixed_precision.py` & `neural_compressor-2.5.1/neural_compressor/strategy/auto_mixed_precision.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/strategy/basic.py` & `neural_compressor-2.5.1/neural_compressor/strategy/basic.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/strategy/bayesian.py` & `neural_compressor-2.5.1/neural_compressor/strategy/bayesian.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/strategy/conservative.py` & `neural_compressor-2.5.1/neural_compressor/strategy/conservative.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/strategy/exhaustive.py` & `neural_compressor-2.5.1/neural_compressor/strategy/exhaustive.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/strategy/hawq_v2.py` & `neural_compressor-2.5.1/neural_compressor/strategy/hawq_v2.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/strategy/mse.py` & `neural_compressor-2.5.1/neural_compressor/strategy/mse.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/strategy/mse_v2.py` & `neural_compressor-2.5.1/neural_compressor/strategy/mse_v2.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/strategy/random.py` & `neural_compressor-2.5.1/neural_compressor/strategy/random.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/strategy/strategy.py` & `neural_compressor-2.5.1/neural_compressor/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/strategy/utils/__init__.py` & `neural_compressor-2.5.1/neural_compressor/strategy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/strategy/utils/constant.py` & `neural_compressor-2.5.1/neural_compressor/strategy/utils/constant.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/strategy/utils/tuning_sampler.py` & `neural_compressor-2.5.1/neural_compressor/strategy/utils/tuning_sampler.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/strategy/utils/tuning_space.py` & `neural_compressor-2.5.1/neural_compressor/strategy/utils/tuning_space.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/strategy/utils/tuning_structs.py` & `neural_compressor-2.5.1/neural_compressor/strategy/utils/tuning_structs.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/strategy/utils/utility.py` & `neural_compressor-2.5.1/neural_compressor/strategy/utils/utility.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/training.py` & `neural_compressor-2.5.1/neural_compressor/training.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/utils/__init__.py` & `neural_compressor-2.5.1/neural_compressor/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/utils/collect_layer_histogram.py` & `neural_compressor-2.5.1/neural_compressor/utils/collect_layer_histogram.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/utils/constant.py` & `neural_compressor-2.5.1/neural_compressor/utils/constant.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/utils/create_obj_from_config.py` & `neural_compressor-2.5.1/neural_compressor/utils/create_obj_from_config.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/utils/kl_divergence.py` & `neural_compressor-2.5.1/neural_compressor/utils/kl_divergence.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/utils/load_huggingface.py` & `neural_compressor-2.5.1/neural_compressor/utils/load_huggingface.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/utils/logger.py` & `neural_compressor-2.5.1/neural_compressor/utils/logger.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/utils/neural_insights_utils.py` & `neural_compressor-2.5.1/neural_compressor/utils/neural_insights_utils.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/utils/options.py` & `neural_compressor-2.5.1/neural_compressor/utils/options.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/utils/pytorch.py` & `neural_compressor-2.5.1/neural_compressor/utils/pytorch.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/utils/utility.py` & `neural_compressor-2.5.1/neural_compressor/utils/utility.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/utils/weights_details.py` & `neural_compressor-2.5.1/neural_compressor/utils/weights_details.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/neural_compressor/version.py` & `neural_compressor-2.5.1/neural_compressor/version.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Intel® Neural Compressor: An open-source Python library supporting popular model compression techniques."""
-__version__ = "2.5"
+__version__ = "2.5.1"
```

### Comparing `neural_compressor-2.5/neural_compressor.egg-info/PKG-INFO` & `neural_compressor-2.5.1/neural_compressor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neural_compressor
-Version: 2.5
+Version: 2.5.1
 Summary: Repository of Intel® Neural Compressor
 Home-page: https://github.com/intel/neural-compressor
 Author: Intel AIPT Team
 Author-email: feng.tian@intel.com, haihao.shen@intel.com, suyue.chen@intel.com
 License: Apache 2.0
 Keywords: quantization,auto-tuning,post-training static quantization,post-training dynamic quantization,quantization-aware training
 Classifier: Intended Audience :: Science/Research
@@ -26,19 +26,19 @@
 Requires-Dist: pycocotools; sys_platform != "win32" or python_version > "3.8"
 Requires-Dist: pycocotools-windows; sys_platform == "win32" and python_version <= "3.8"
 Requires-Dist: pyyaml
 Requires-Dist: requests
 Requires-Dist: schema
 Requires-Dist: scikit-learn
 Provides-Extra: pt
-Requires-Dist: neural_compressor_3x_pt==2.5; extra == "pt"
+Requires-Dist: neural_compressor_3x_pt==2.5.1; extra == "pt"
 Provides-Extra: tf
-Requires-Dist: neural_compressor_3x_tf==2.5; extra == "tf"
+Requires-Dist: neural_compressor_3x_tf==2.5.1; extra == "tf"
 Provides-Extra: ort
-Requires-Dist: neural_compressor_3x_ort==2.5; extra == "ort"
+Requires-Dist: neural_compressor_3x_ort==2.5.1; extra == "ort"
 
 <div align="center">
 
 Intel® Neural Compressor
 ===========================
 <h3> An open-source Python library supporting popular model compression techniques on all mainstream deep learning frameworks (TensorFlow, PyTorch, ONNX Runtime, and MXNet)</h3>
```

### Comparing `neural_compressor-2.5/neural_compressor.egg-info/SOURCES.txt` & `neural_compressor-2.5.1/neural_compressor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/pyproject.toml` & `neural_compressor-2.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/setup.py` & `neural_compressor-2.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.5/third-party-programs.txt` & `neural_compressor-2.5.1/third-party-programs.txt`

 * *Files identical despite different names*

