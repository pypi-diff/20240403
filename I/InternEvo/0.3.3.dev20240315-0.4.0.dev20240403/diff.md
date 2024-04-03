# Comparing `tmp/InternEvo-0.3.3.dev20240315.tar.gz` & `tmp/InternEvo-0.4.0.dev20240403.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "InternEvo-0.3.3.dev20240315.tar", last modified: Fri Mar 15 02:41:08 2024, max compression
+gzip compressed data, was "InternEvo-0.4.0.dev20240403.tar", last modified: Wed Apr  3 14:30:19 2024, max compression
```

## Comparing `InternEvo-0.3.3.dev20240315.tar` & `InternEvo-0.4.0.dev20240403.tar`

### file list

```diff
@@ -1,135 +1,161 @@
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 02:39:36.781574 InternEvo-0.3.3.dev20240315/
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 02:39:35.816577 InternEvo-0.3.3.dev20240315/InternEvo.egg-info/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5332 2024-03-15 02:41:07.000000 InternEvo-0.3.3.dev20240315/InternEvo.egg-info/PKG-INFO
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3501 2024-03-15 02:41:07.000000 InternEvo-0.3.3.dev20240315/InternEvo.egg-info/SOURCES.txt
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        1 2024-03-15 02:41:07.000000 InternEvo-0.3.3.dev20240315/InternEvo.egg-info/dependency_links.txt
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       15 2024-03-15 02:41:07.000000 InternEvo-0.3.3.dev20240315/InternEvo.egg-info/top_level.txt
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    13656 2024-01-17 04:37:11.000000 InternEvo-0.3.3.dev20240315/LICENSE
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5332 2024-03-15 02:41:08.947112 InternEvo-0.3.3.dev20240315/PKG-INFO
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4730 2024-01-22 07:03:00.000000 InternEvo-0.3.3.dev20240315/README.md
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 02:39:35.822439 InternEvo-0.3.3.dev20240315/internlm/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      267 2024-01-30 08:18:33.000000 InternEvo-0.3.3.dev20240315/internlm/__init__.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 02:39:35.838471 InternEvo-0.3.3.dev20240315/internlm/apis/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-17 04:36:06.000000 InternEvo-0.3.3.dev20240315/internlm/apis/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    37532 2024-01-18 05:06:05.000000 InternEvo-0.3.3.dev20240315/internlm/apis/inference.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 02:39:35.877508 InternEvo-0.3.3.dev20240315/internlm/core/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      158 2024-01-17 04:37:12.000000 InternEvo-0.3.3.dev20240315/internlm/core/__init__.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 02:39:35.919666 InternEvo-0.3.3.dev20240315/internlm/core/communication/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      884 2024-01-17 04:37:12.000000 InternEvo-0.3.3.dev20240315/internlm/core/communication/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    23658 2024-03-14 12:46:21.000000 InternEvo-0.3.3.dev20240315/internlm/core/communication/isp.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    22550 2024-01-30 08:18:33.000000 InternEvo-0.3.3.dev20240315/internlm/core/communication/p2p.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10184 2024-03-14 12:46:21.000000 InternEvo-0.3.3.dev20240315/internlm/core/communication/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 02:39:35.949120 InternEvo-0.3.3.dev20240315/internlm/core/context/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1220 2024-03-12 11:35:05.000000 InternEvo-0.3.3.dev20240315/internlm/core/context/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    27372 2024-03-12 11:35:05.000000 InternEvo-0.3.3.dev20240315/internlm/core/context/parallel_context.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    38371 2024-03-12 11:35:05.000000 InternEvo-0.3.3.dev20240315/internlm/core/context/process_group_initializer.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4011 2024-01-30 08:18:33.000000 InternEvo-0.3.3.dev20240315/internlm/core/context/random.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7447 2024-03-14 12:46:21.000000 InternEvo-0.3.3.dev20240315/internlm/core/engine.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3080 2024-01-30 08:18:33.000000 InternEvo-0.3.3.dev20240315/internlm/core/gradient_handler.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7990 2024-02-06 04:29:21.000000 InternEvo-0.3.3.dev20240315/internlm/core/naive_amp.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 02:39:35.979333 InternEvo-0.3.3.dev20240315/internlm/core/scheduler/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      303 2024-02-06 04:29:21.000000 InternEvo-0.3.3.dev20240315/internlm/core/scheduler/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5258 2024-02-06 04:29:21.000000 InternEvo-0.3.3.dev20240315/internlm/core/scheduler/base_scheduler.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     8618 2024-02-06 04:29:21.000000 InternEvo-0.3.3.dev20240315/internlm/core/scheduler/no_pipeline_scheduler.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    63524 2024-03-04 06:50:16.000000 InternEvo-0.3.3.dev20240315/internlm/core/scheduler/pipeline_scheduler.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7598 2024-01-18 05:06:05.000000 InternEvo-0.3.3.dev20240315/internlm/core/trainer.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 02:39:36.247924 InternEvo-0.3.3.dev20240315/internlm/data/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      404 2024-03-14 12:46:21.000000 InternEvo-0.3.3.dev20240315/internlm/data/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    15158 2024-03-14 12:46:21.000000 InternEvo-0.3.3.dev20240315/internlm/data/batch_sampler.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3767 2024-03-14 12:46:21.000000 InternEvo-0.3.3.dev20240315/internlm/data/collaters.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1704 2024-03-14 12:46:21.000000 InternEvo-0.3.3.dev20240315/internlm/data/dataset.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1238 2024-03-14 12:46:21.000000 InternEvo-0.3.3.dev20240315/internlm/data/dummy_dataset.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    17060 2024-03-14 12:46:21.000000 InternEvo-0.3.3.dev20240315/internlm/data/packed_dataset.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3740 2024-03-14 12:46:21.000000 InternEvo-0.3.3.dev20240315/internlm/data/single_dataset.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1873 2024-01-18 05:06:05.000000 InternEvo-0.3.3.dev20240315/internlm/data/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 02:39:36.273130 InternEvo-0.3.3.dev20240315/internlm/initialize/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      368 2024-01-18 05:06:05.000000 InternEvo-0.3.3.dev20240315/internlm/initialize/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1793 2024-01-17 04:37:12.000000 InternEvo-0.3.3.dev20240315/internlm/initialize/initialize_tensor.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5908 2024-03-14 12:46:21.000000 InternEvo-0.3.3.dev20240315/internlm/initialize/initialize_trainer.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    26316 2024-03-15 02:20:29.000000 InternEvo-0.3.3.dev20240315/internlm/initialize/launch.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 02:39:36.290549 InternEvo-0.3.3.dev20240315/internlm/initialize/legacy/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-17 04:36:06.000000 InternEvo-0.3.3.dev20240315/internlm/initialize/legacy/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1589 2024-01-17 04:37:12.000000 InternEvo-0.3.3.dev20240315/internlm/initialize/legacy/launch.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 02:39:36.379000 InternEvo-0.3.3.dev20240315/internlm/model/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      963 2024-03-14 12:46:21.000000 InternEvo-0.3.3.dev20240315/internlm/model/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    25277 2024-03-14 12:46:21.000000 InternEvo-0.3.3.dev20240315/internlm/model/embedding.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    22840 2024-03-14 12:46:21.000000 InternEvo-0.3.3.dev20240315/internlm/model/linear.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2161 2024-03-14 12:46:21.000000 InternEvo-0.3.3.dev20240315/internlm/model/loss.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    14649 2024-03-08 11:41:31.000000 InternEvo-0.3.3.dev20240315/internlm/model/metrics.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    24020 2024-03-14 12:46:21.000000 InternEvo-0.3.3.dev20240315/internlm/model/modeling_internlm.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    54863 2024-03-14 12:46:21.000000 InternEvo-0.3.3.dev20240315/internlm/model/modeling_internlm2.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    54790 2024-03-14 12:46:21.000000 InternEvo-0.3.3.dev20240315/internlm/model/modeling_llama.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    26089 2024-03-14 12:46:21.000000 InternEvo-0.3.3.dev20240315/internlm/model/modeling_moe.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4291 2024-03-14 12:46:21.000000 InternEvo-0.3.3.dev20240315/internlm/model/moe.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    32110 2024-03-14 12:46:21.000000 InternEvo-0.3.3.dev20240315/internlm/model/multi_head_attention.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1500 2024-03-14 12:46:21.000000 InternEvo-0.3.3.dev20240315/internlm/model/norm.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    23195 2024-03-14 12:46:21.000000 InternEvo-0.3.3.dev20240315/internlm/model/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 02:39:36.413322 InternEvo-0.3.3.dev20240315/internlm/moe/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      635 2024-03-15 02:20:29.000000 InternEvo-0.3.3.dev20240315/internlm/moe/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1146 2024-03-14 12:46:21.000000 InternEvo-0.3.3.dev20240315/internlm/moe/base_moe.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2762 2024-03-14 12:46:21.000000 InternEvo-0.3.3.dev20240315/internlm/moe/experts.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    17695 2024-03-15 02:20:29.000000 InternEvo-0.3.3.dev20240315/internlm/moe/gshard_moe.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 02:39:36.449326 InternEvo-0.3.3.dev20240315/internlm/moe/megablock/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 02:18:56.000000 InternEvo-0.3.3.dev20240315/internlm/moe/megablock/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     8679 2024-03-15 02:20:29.000000 InternEvo-0.3.3.dev20240315/internlm/moe/megablock/megablock_dmoe.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    13623 2024-03-15 02:20:29.000000 InternEvo-0.3.3.dev20240315/internlm/moe/megablock/megablock_moe.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2528 2024-03-15 02:20:29.000000 InternEvo-0.3.3.dev20240315/internlm/moe/megablock/mlp.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11795 2024-03-15 02:20:29.000000 InternEvo-0.3.3.dev20240315/internlm/moe/megablock/utils.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2021 2024-03-14 12:46:21.000000 InternEvo-0.3.3.dev20240315/internlm/moe/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 02:39:36.475891 InternEvo-0.3.3.dev20240315/internlm/monitor/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      307 2024-01-17 04:37:12.000000 InternEvo-0.3.3.dev20240315/internlm/monitor/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4156 2024-01-18 05:06:05.000000 InternEvo-0.3.3.dev20240315/internlm/monitor/alert.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10581 2024-01-18 05:06:05.000000 InternEvo-0.3.3.dev20240315/internlm/monitor/monitor.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1068 2024-01-18 05:06:05.000000 InternEvo-0.3.3.dev20240315/internlm/monitor/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 02:39:36.502446 InternEvo-0.3.3.dev20240315/internlm/solver/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      282 2024-03-14 12:46:21.000000 InternEvo-0.3.3.dev20240315/internlm/solver/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      988 2024-03-14 12:46:21.000000 InternEvo-0.3.3.dev20240315/internlm/solver/beta2_scheduler.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5940 2024-03-14 12:46:21.000000 InternEvo-0.3.3.dev20240315/internlm/solver/lr_scheduler.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 02:39:36.547693 InternEvo-0.3.3.dev20240315/internlm/solver/optimizer/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      252 2024-01-18 05:06:05.000000 InternEvo-0.3.3.dev20240315/internlm/solver/optimizer/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1080 2024-01-18 05:06:05.000000 InternEvo-0.3.3.dev20240315/internlm/solver/optimizer/base_optimizer.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     9190 2024-01-18 05:06:05.000000 InternEvo-0.3.3.dev20240315/internlm/solver/optimizer/fsdp_optimizer.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    54124 2024-03-12 11:35:06.000000 InternEvo-0.3.3.dev20240315/internlm/solver/optimizer/hybrid_zero_optim.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11132 2024-02-06 04:29:22.000000 InternEvo-0.3.3.dev20240315/internlm/solver/optimizer/store.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    32014 2024-03-15 02:20:29.000000 InternEvo-0.3.3.dev20240315/internlm/solver/optimizer/utils.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1280 2024-01-17 04:37:12.000000 InternEvo-0.3.3.dev20240315/internlm/solver/pipeline_utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 02:39:36.568312 InternEvo-0.3.3.dev20240315/internlm/train/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      766 2024-03-14 12:46:21.000000 InternEvo-0.3.3.dev20240315/internlm/train/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    30746 2024-03-15 02:20:29.000000 InternEvo-0.3.3.dev20240315/internlm/train/training_internlm.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3454 2024-03-12 11:35:06.000000 InternEvo-0.3.3.dev20240315/internlm/train/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 02:39:36.667969 InternEvo-0.3.3.dev20240315/internlm/utils/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-17 04:36:06.000000 InternEvo-0.3.3.dev20240315/internlm/utils/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     9915 2024-03-14 12:46:21.000000 InternEvo-0.3.3.dev20240315/internlm/utils/checkpoint.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     8576 2024-02-06 04:29:22.000000 InternEvo-0.3.3.dev20240315/internlm/utils/common.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     8407 2024-03-14 12:46:21.000000 InternEvo-0.3.3.dev20240315/internlm/utils/evaluation.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    12678 2024-03-14 12:46:21.000000 InternEvo-0.3.3.dev20240315/internlm/utils/gputest.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3082 2024-01-17 04:37:13.000000 InternEvo-0.3.3.dev20240315/internlm/utils/logger.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4068 2024-01-30 08:18:33.000000 InternEvo-0.3.3.dev20240315/internlm/utils/megatron_timers.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    57349 2024-03-14 12:46:21.000000 InternEvo-0.3.3.dev20240315/internlm/utils/model_checkpoint.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5893 2024-03-15 02:20:29.000000 InternEvo-0.3.3.dev20240315/internlm/utils/parallel.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2423 2024-01-18 05:06:05.000000 InternEvo-0.3.3.dev20240315/internlm/utils/registry.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    24600 2024-01-18 05:06:05.000000 InternEvo-0.3.3.dev20240315/internlm/utils/simple_memory_profiler.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    46135 2024-03-04 06:50:17.000000 InternEvo-0.3.3.dev20240315/internlm/utils/storage_manager.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3107 2024-03-14 12:46:21.000000 InternEvo-0.3.3.dev20240315/internlm/utils/timeout.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      709 2024-02-07 12:02:59.000000 InternEvo-0.3.3.dev20240315/internlm/utils/utils.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6995 2024-01-30 08:18:33.000000 InternEvo-0.3.3.dev20240315/internlm/utils/writer.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       38 2024-03-15 02:41:08.951843 InternEvo-0.3.3.dev20240315/setup.cfg
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1103 2024-01-25 12:12:30.000000 InternEvo-0.3.3.dev20240315/setup.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 02:39:36.678041 InternEvo-0.3.3.dev20240315/tests/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-17 04:36:06.000000 InternEvo-0.3.3.dev20240315/tests/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4349 2024-03-14 12:46:21.000000 InternEvo-0.3.3.dev20240315/tests/common_fixture.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 02:39:36.699075 InternEvo-0.3.3.dev20240315/tests/test_core/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-18 05:04:59.000000 InternEvo-0.3.3.dev20240315/tests/test_core/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5231 2024-03-14 12:46:21.000000 InternEvo-0.3.3.dev20240315/tests/test_core/test_pipeline.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6751 2024-02-06 04:29:22.000000 InternEvo-0.3.3.dev20240315/tests/test_core/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 02:39:36.771529 InternEvo-0.3.3.dev20240315/tests/test_training/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5678 2024-01-18 05:06:05.000000 InternEvo-0.3.3.dev20240315/tests/test_training/7B_check_acc.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6319 2024-02-06 04:29:22.000000 InternEvo-0.3.3.dev20240315/tests/test_training/7B_check_init.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-18 05:04:59.000000 InternEvo-0.3.3.dev20240315/tests/test_training/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7626 2024-03-14 12:46:21.000000 InternEvo-0.3.3.dev20240315/tests/test_training/test_forward_output_no_fa.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10078 2024-03-14 12:46:21.000000 InternEvo-0.3.3.dev20240315/tests/test_training/test_load_ckpt_loss.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    12833 2024-03-14 12:46:21.000000 InternEvo-0.3.3.dev20240315/tests/test_training/test_loss.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3706 2024-03-14 12:46:21.000000 InternEvo-0.3.3.dev20240315/tests/test_training/test_no_fa_train_temp.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6330 2024-03-14 12:46:21.000000 InternEvo-0.3.3.dev20240315/tests/test_training/test_norm_weight.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    12500 2024-03-14 12:46:21.000000 InternEvo-0.3.3.dev20240315/tests/test_training/test_swap_nb_loss_and_gradnorm.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    14297 2024-03-14 12:46:21.000000 InternEvo-0.3.3.dev20240315/tests/test_training/train_CI.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:37.723194 InternEvo-0.4.0.dev20240403/
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:36.816954 InternEvo-0.4.0.dev20240403/InternEvo.egg-info/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5332 2024-04-03 14:30:17.000000 InternEvo-0.4.0.dev20240403/InternEvo.egg-info/PKG-INFO
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4317 2024-04-03 14:30:17.000000 InternEvo-0.4.0.dev20240403/InternEvo.egg-info/SOURCES.txt
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        1 2024-04-03 14:30:17.000000 InternEvo-0.4.0.dev20240403/InternEvo.egg-info/dependency_links.txt
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       15 2024-04-03 14:30:17.000000 InternEvo-0.4.0.dev20240403/InternEvo.egg-info/top_level.txt
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    13656 2024-01-25 08:28:54.000000 InternEvo-0.4.0.dev20240403/LICENSE
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5332 2024-04-03 14:30:19.044910 InternEvo-0.4.0.dev20240403/PKG-INFO
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4730 2024-01-25 08:28:54.000000 InternEvo-0.4.0.dev20240403/README.md
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:36.824243 InternEvo-0.4.0.dev20240403/internlm/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      267 2024-01-30 08:18:31.000000 InternEvo-0.4.0.dev20240403/internlm/__init__.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:36.867718 InternEvo-0.4.0.dev20240403/internlm/accelerator/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      147 2024-03-26 14:50:22.000000 InternEvo-0.4.0.dev20240403/internlm/accelerator/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4017 2024-04-02 03:03:24.000000 InternEvo-0.4.0.dev20240403/internlm/accelerator/abstract_accelerator.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11010 2024-03-28 03:16:50.000000 InternEvo-0.4.0.dev20240403/internlm/accelerator/cuda_accelerator.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11446 2024-04-02 03:03:24.000000 InternEvo-0.4.0.dev20240403/internlm/accelerator/dipu_accelerator.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10866 2024-03-28 03:16:50.000000 InternEvo-0.4.0.dev20240403/internlm/accelerator/npu_accelerator.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:36.880860 InternEvo-0.4.0.dev20240403/internlm/apis/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.4.0.dev20240403/internlm/apis/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    37532 2024-01-25 08:28:55.000000 InternEvo-0.4.0.dev20240403/internlm/apis/inference.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:36.926106 InternEvo-0.4.0.dev20240403/internlm/checkpoint/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       83 2024-03-15 18:58:58.000000 InternEvo-0.4.0.dev20240403/internlm/checkpoint/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    27404 2024-03-26 14:50:22.000000 InternEvo-0.4.0.dev20240403/internlm/checkpoint/checkpoint_manager.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20076 2024-03-26 14:50:22.000000 InternEvo-0.4.0.dev20240403/internlm/checkpoint/components.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     8723 2024-03-26 14:50:23.000000 InternEvo-0.4.0.dev20240403/internlm/checkpoint/load_funcs.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2504 2024-04-03 02:12:20.000000 InternEvo-0.4.0.dev20240403/internlm/checkpoint/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:36.967895 InternEvo-0.4.0.dev20240403/internlm/core/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      158 2024-01-25 08:28:55.000000 InternEvo-0.4.0.dev20240403/internlm/core/__init__.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:36.998938 InternEvo-0.4.0.dev20240403/internlm/core/communication/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      884 2024-01-25 08:28:55.000000 InternEvo-0.4.0.dev20240403/internlm/core/communication/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    23944 2024-04-02 03:03:24.000000 InternEvo-0.4.0.dev20240403/internlm/core/communication/isp.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    22670 2024-03-26 14:50:23.000000 InternEvo-0.4.0.dev20240403/internlm/core/communication/p2p.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10352 2024-04-03 02:12:20.000000 InternEvo-0.4.0.dev20240403/internlm/core/communication/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:37.032423 InternEvo-0.4.0.dev20240403/internlm/core/context/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1220 2024-03-18 08:30:10.000000 InternEvo-0.4.0.dev20240403/internlm/core/context/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    27076 2024-03-27 02:26:43.000000 InternEvo-0.4.0.dev20240403/internlm/core/context/parallel_context.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    38371 2024-03-18 08:30:10.000000 InternEvo-0.4.0.dev20240403/internlm/core/context/process_group_initializer.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4295 2024-04-03 12:26:56.000000 InternEvo-0.4.0.dev20240403/internlm/core/context/random.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7458 2024-03-15 18:58:58.000000 InternEvo-0.4.0.dev20240403/internlm/core/engine.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3113 2024-03-28 03:16:50.000000 InternEvo-0.4.0.dev20240403/internlm/core/gradient_handler.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     8195 2024-04-01 03:27:51.000000 InternEvo-0.4.0.dev20240403/internlm/core/naive_amp.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:37.059207 InternEvo-0.4.0.dev20240403/internlm/core/scheduler/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      303 2024-02-08 03:13:39.000000 InternEvo-0.4.0.dev20240403/internlm/core/scheduler/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5258 2024-03-22 07:04:00.000000 InternEvo-0.4.0.dev20240403/internlm/core/scheduler/base_scheduler.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     9071 2024-04-01 03:27:51.000000 InternEvo-0.4.0.dev20240403/internlm/core/scheduler/no_pipeline_scheduler.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    64105 2024-04-01 03:27:51.000000 InternEvo-0.4.0.dev20240403/internlm/core/scheduler/pipeline_scheduler.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7598 2024-01-25 08:28:55.000000 InternEvo-0.4.0.dev20240403/internlm/core/trainer.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:37.090006 InternEvo-0.4.0.dev20240403/internlm/data/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      209 2024-03-15 18:58:58.000000 InternEvo-0.4.0.dev20240403/internlm/data/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5819 2024-03-26 10:32:52.000000 InternEvo-0.4.0.dev20240403/internlm/data/build_dataloader.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:37.138904 InternEvo-0.4.0.dev20240403/internlm/data/tokenized/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      418 2024-03-22 07:04:00.000000 InternEvo-0.4.0.dev20240403/internlm/data/tokenized/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    15158 2024-03-15 18:58:58.000000 InternEvo-0.4.0.dev20240403/internlm/data/tokenized/batch_sampler.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3767 2024-03-25 08:46:10.000000 InternEvo-0.4.0.dev20240403/internlm/data/tokenized/collaters.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1714 2024-03-15 18:58:58.000000 InternEvo-0.4.0.dev20240403/internlm/data/tokenized/dataset.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1406 2024-03-26 10:32:52.000000 InternEvo-0.4.0.dev20240403/internlm/data/tokenized/dummy_dataset.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    18135 2024-03-26 10:32:52.000000 InternEvo-0.4.0.dev20240403/internlm/data/tokenized/packed_dataset.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3740 2024-03-15 18:58:58.000000 InternEvo-0.4.0.dev20240403/internlm/data/tokenized/single_dataset.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      454 2024-03-15 18:58:58.000000 InternEvo-0.4.0.dev20240403/internlm/data/train_state.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1919 2024-04-01 03:27:51.000000 InternEvo-0.4.0.dev20240403/internlm/data/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:37.156319 InternEvo-0.4.0.dev20240403/internlm/eval/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       86 2024-03-15 18:58:58.000000 InternEvo-0.4.0.dev20240403/internlm/eval/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5552 2024-04-01 03:27:51.000000 InternEvo-0.4.0.dev20240403/internlm/eval/evaluation.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:37.183331 InternEvo-0.4.0.dev20240403/internlm/initialize/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      368 2024-01-25 08:28:55.000000 InternEvo-0.4.0.dev20240403/internlm/initialize/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1793 2024-01-25 08:28:55.000000 InternEvo-0.4.0.dev20240403/internlm/initialize/initialize_tensor.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5922 2024-03-26 10:32:52.000000 InternEvo-0.4.0.dev20240403/internlm/initialize/initialize_trainer.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    27669 2024-04-03 12:26:56.000000 InternEvo-0.4.0.dev20240403/internlm/initialize/launch.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:37.199228 InternEvo-0.4.0.dev20240403/internlm/initialize/legacy/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.4.0.dev20240403/internlm/initialize/legacy/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1592 2024-04-01 03:27:51.000000 InternEvo-0.4.0.dev20240403/internlm/initialize/legacy/launch.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:37.250254 InternEvo-0.4.0.dev20240403/internlm/model/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1011 2024-03-25 08:46:10.000000 InternEvo-0.4.0.dev20240403/internlm/model/__init__.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:37.265555 InternEvo-0.4.0.dev20240403/internlm/model/losses/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       73 2024-03-15 18:58:58.000000 InternEvo-0.4.0.dev20240403/internlm/model/losses/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2275 2024-04-03 02:12:20.000000 InternEvo-0.4.0.dev20240403/internlm/model/losses/ce_loss.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    16750 2024-04-03 03:05:29.000000 InternEvo-0.4.0.dev20240403/internlm/model/metrics.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    24429 2024-04-03 02:12:20.000000 InternEvo-0.4.0.dev20240403/internlm/model/modeling_internlm.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    55789 2024-04-03 02:12:20.000000 InternEvo-0.4.0.dev20240403/internlm/model/modeling_internlm2.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    53658 2024-04-03 02:12:20.000000 InternEvo-0.4.0.dev20240403/internlm/model/modeling_llama.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    26623 2024-04-03 02:12:20.000000 InternEvo-0.4.0.dev20240403/internlm/model/modeling_moe.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:37.297343 InternEvo-0.4.0.dev20240403/internlm/model/modules/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 18:57:26.000000 InternEvo-0.4.0.dev20240403/internlm/model/modules/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20285 2024-04-03 02:12:20.000000 InternEvo-0.4.0.dev20240403/internlm/model/modules/embedding.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     9883 2024-04-01 07:02:19.000000 InternEvo-0.4.0.dev20240403/internlm/model/modules/mlp.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    40988 2024-04-03 02:12:20.000000 InternEvo-0.4.0.dev20240403/internlm/model/modules/multi_head_attention.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:37.335707 InternEvo-0.4.0.dev20240403/internlm/model/moe/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      678 2024-03-15 18:58:58.000000 InternEvo-0.4.0.dev20240403/internlm/model/moe/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1198 2024-03-28 03:16:50.000000 InternEvo-0.4.0.dev20240403/internlm/model/moe/base_layer.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2762 2024-03-18 08:30:10.000000 InternEvo-0.4.0.dev20240403/internlm/model/moe/experts.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    17698 2024-04-02 09:15:26.000000 InternEvo-0.4.0.dev20240403/internlm/model/moe/gshard_layer.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:37.371323 InternEvo-0.4.0.dev20240403/internlm/model/moe/megablock/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 18:57:26.000000 InternEvo-0.4.0.dev20240403/internlm/model/moe/megablock/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     8705 2024-03-15 18:58:58.000000 InternEvo-0.4.0.dev20240403/internlm/model/moe/megablock/megablock_dmoe.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    13643 2024-03-15 18:58:58.000000 InternEvo-0.4.0.dev20240403/internlm/model/moe/megablock/megablock_moe.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2555 2024-03-15 18:58:58.000000 InternEvo-0.4.0.dev20240403/internlm/model/moe/megablock/mlp.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11986 2024-03-26 14:50:23.000000 InternEvo-0.4.0.dev20240403/internlm/model/moe/megablock/utils.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4494 2024-04-01 03:27:51.000000 InternEvo-0.4.0.dev20240403/internlm/model/moe/moe.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2021 2024-03-18 08:30:10.000000 InternEvo-0.4.0.dev20240403/internlm/model/moe/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:37.392015 InternEvo-0.4.0.dev20240403/internlm/model/ops/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 18:57:26.000000 InternEvo-0.4.0.dev20240403/internlm/model/ops/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    16010 2024-03-28 02:19:14.000000 InternEvo-0.4.0.dev20240403/internlm/model/ops/linear.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1500 2024-03-15 18:58:59.000000 InternEvo-0.4.0.dev20240403/internlm/model/ops/norm.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    26403 2024-04-03 02:12:20.000000 InternEvo-0.4.0.dev20240403/internlm/model/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:37.423565 InternEvo-0.4.0.dev20240403/internlm/monitor/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      193 2024-04-03 12:26:56.000000 InternEvo-0.4.0.dev20240403/internlm/monitor/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1479 2024-04-03 12:26:56.000000 InternEvo-0.4.0.dev20240403/internlm/monitor/alert.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10213 2024-04-03 12:26:56.000000 InternEvo-0.4.0.dev20240403/internlm/monitor/monitor.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      776 2024-04-03 12:26:56.000000 InternEvo-0.4.0.dev20240403/internlm/monitor/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:37.444280 InternEvo-0.4.0.dev20240403/internlm/solver/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      252 2024-03-15 18:58:59.000000 InternEvo-0.4.0.dev20240403/internlm/solver/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10095 2024-04-03 12:26:56.000000 InternEvo-0.4.0.dev20240403/internlm/solver/activation_checkpoint.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:37.485173 InternEvo-0.4.0.dev20240403/internlm/solver/optimizer/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      252 2024-03-22 07:04:01.000000 InternEvo-0.4.0.dev20240403/internlm/solver/optimizer/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1080 2024-01-25 08:28:55.000000 InternEvo-0.4.0.dev20240403/internlm/solver/optimizer/base_optimizer.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     9173 2024-03-22 08:39:35.000000 InternEvo-0.4.0.dev20240403/internlm/solver/optimizer/fsdp_optimizer.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    42555 2024-04-02 03:03:24.000000 InternEvo-0.4.0.dev20240403/internlm/solver/optimizer/hybrid_zero_optim.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10132 2024-03-22 08:39:35.000000 InternEvo-0.4.0.dev20240403/internlm/solver/optimizer/store.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20351 2024-04-02 03:03:24.000000 InternEvo-0.4.0.dev20240403/internlm/solver/optimizer/utils.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1280 2024-01-25 08:28:55.000000 InternEvo-0.4.0.dev20240403/internlm/solver/pipeline_utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:37.509032 InternEvo-0.4.0.dev20240403/internlm/solver/schedulers/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      272 2024-03-15 18:58:59.000000 InternEvo-0.4.0.dev20240403/internlm/solver/schedulers/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      844 2024-03-26 03:26:29.000000 InternEvo-0.4.0.dev20240403/internlm/solver/schedulers/beta2_scheduler.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5940 2024-03-15 18:58:59.000000 InternEvo-0.4.0.dev20240403/internlm/solver/schedulers/lr_scheduler.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:37.529815 InternEvo-0.4.0.dev20240403/internlm/train/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      635 2024-03-15 18:58:59.000000 InternEvo-0.4.0.dev20240403/internlm/train/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    24865 2024-04-03 12:26:56.000000 InternEvo-0.4.0.dev20240403/internlm/train/pipeline.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3454 2024-03-25 08:46:10.000000 InternEvo-0.4.0.dev20240403/internlm/train/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:37.610026 InternEvo-0.4.0.dev20240403/internlm/utils/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.4.0.dev20240403/internlm/utils/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     8886 2024-04-02 03:03:24.000000 InternEvo-0.4.0.dev20240403/internlm/utils/common.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6321 2024-04-02 07:54:06.000000 InternEvo-0.4.0.dev20240403/internlm/utils/gputest.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1353 2024-04-03 12:26:56.000000 InternEvo-0.4.0.dev20240403/internlm/utils/logger.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4156 2024-03-26 14:51:38.000000 InternEvo-0.4.0.dev20240403/internlm/utils/megatron_timers.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4038 2024-04-03 02:12:20.000000 InternEvo-0.4.0.dev20240403/internlm/utils/parallel.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2423 2024-01-25 08:28:55.000000 InternEvo-0.4.0.dev20240403/internlm/utils/registry.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    24734 2024-03-26 03:26:29.000000 InternEvo-0.4.0.dev20240403/internlm/utils/simple_memory_profiler.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    46133 2024-04-01 03:27:51.000000 InternEvo-0.4.0.dev20240403/internlm/utils/storage_manager.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3126 2024-03-15 18:58:59.000000 InternEvo-0.4.0.dev20240403/internlm/utils/timeout.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      709 2024-02-07 12:02:58.000000 InternEvo-0.4.0.dev20240403/internlm/utils/utils.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7117 2024-03-28 03:16:51.000000 InternEvo-0.4.0.dev20240403/internlm/utils/writer.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       38 2024-04-03 14:30:19.047881 InternEvo-0.4.0.dev20240403/setup.cfg
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1103 2024-01-25 12:12:29.000000 InternEvo-0.4.0.dev20240403/setup.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:37.619324 InternEvo-0.4.0.dev20240403/tests/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.4.0.dev20240403/tests/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4510 2024-03-26 15:01:25.000000 InternEvo-0.4.0.dev20240403/tests/common_fixture.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:37.642253 InternEvo-0.4.0.dev20240403/tests/test_core/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.4.0.dev20240403/tests/test_core/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5875 2024-04-03 02:12:20.000000 InternEvo-0.4.0.dev20240403/tests/test_core/test_pipeline.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6978 2024-03-26 15:01:25.000000 InternEvo-0.4.0.dev20240403/tests/test_core/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:37.712084 InternEvo-0.4.0.dev20240403/tests/test_training/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5750 2024-04-01 03:27:51.000000 InternEvo-0.4.0.dev20240403/tests/test_training/7B_check_acc.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6360 2024-04-01 03:27:51.000000 InternEvo-0.4.0.dev20240403/tests/test_training/7B_check_init.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:46.000000 InternEvo-0.4.0.dev20240403/tests/test_training/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7939 2024-04-03 02:12:20.000000 InternEvo-0.4.0.dev20240403/tests/test_training/test_forward_output_no_fa.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11734 2024-04-03 02:12:20.000000 InternEvo-0.4.0.dev20240403/tests/test_training/test_load_ckpt_loss.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    12904 2024-04-01 04:38:33.000000 InternEvo-0.4.0.dev20240403/tests/test_training/test_loss.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3845 2024-03-27 06:23:57.000000 InternEvo-0.4.0.dev20240403/tests/test_training/test_no_fa_train_temp.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6521 2024-03-27 06:23:57.000000 InternEvo-0.4.0.dev20240403/tests/test_training/test_norm_weight.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    12591 2024-04-03 02:12:20.000000 InternEvo-0.4.0.dev20240403/tests/test_training/test_swap_nb_loss_and_gradnorm.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    13964 2024-04-03 12:26:56.000000 InternEvo-0.4.0.dev20240403/tests/test_training/train_CI.py
```

### Comparing `InternEvo-0.3.3.dev20240315/InternEvo.egg-info/PKG-INFO` & `InternEvo-0.4.0.dev20240403/InternEvo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: InternEvo
-Version: 0.3.3.dev20240315
+Version: 0.4.0.dev20240403
 Summary: an open-sourced lightweight training framework aims to support model pre-training without the need for extensive dependencies
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: InternEvo Version: 0.3.3.dev20240315 Summary: an
+Metadata-Version: 2.1 Name: InternEvo Version: 0.4.0.dev20240403 Summary: an
 open-sourced lightweight training framework aims to support model pre-training
 without the need for extensive dependencies Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Education Classifier: Intended Audience :: Science/Research
 Description-Content-Type: text/markdown License-File: LICENSE # InternEvo
```

### Comparing `InternEvo-0.3.3.dev20240315/LICENSE` & `InternEvo-0.4.0.dev20240403/LICENSE`

 * *Files identical despite different names*

### Comparing `InternEvo-0.3.3.dev20240315/PKG-INFO` & `InternEvo-0.4.0.dev20240403/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: InternEvo
-Version: 0.3.3.dev20240315
+Version: 0.4.0.dev20240403
 Summary: an open-sourced lightweight training framework aims to support model pre-training without the need for extensive dependencies
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: InternEvo Version: 0.3.3.dev20240315 Summary: an
+Metadata-Version: 2.1 Name: InternEvo Version: 0.4.0.dev20240403 Summary: an
 open-sourced lightweight training framework aims to support model pre-training
 without the need for extensive dependencies Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Education Classifier: Intended Audience :: Science/Research
 Description-Content-Type: text/markdown License-File: LICENSE # InternEvo
```

### Comparing `InternEvo-0.3.3.dev20240315/README.md` & `InternEvo-0.4.0.dev20240403/README.md`

 * *Files identical despite different names*

### Comparing `InternEvo-0.3.3.dev20240315/internlm/apis/inference.py` & `InternEvo-0.4.0.dev20240403/internlm/apis/inference.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.3.3.dev20240315/internlm/core/communication/__init__.py` & `InternEvo-0.4.0.dev20240403/internlm/core/communication/__init__.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.3.3.dev20240315/internlm/core/communication/isp.py` & `InternEvo-0.4.0.dev20240403/internlm/core/communication/isp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,43 @@
 #!/usr/bin/env python
 # -*- encoding: utf-8 -*-
 
-from dataclasses import dataclass
 from functools import partial
 from typing import Any, Callable, Dict, List, Union
 
 import torch
 from torch import distributed as dist
 from torch import nn
 
 from internlm.core.context import global_context as gpc
 from internlm.core.naive_amp import NaiveAMPModel
-from internlm.model.linear import ISPLinear
+from internlm.model.ops.linear import ISPLinear
 from internlm.model.utils import all_gather_raw, reduce_scatter_raw
-from internlm.utils.common import SchedulerHook
+from internlm.utils.common import SchedulerHook, get_current_device
 
 
-@dataclass
 class ISPCommModelConfig:
     """
     model config for isp communicator.
     """
 
-    dtype: torch.dtype = torch.half
-    device: torch.device = torch.device("cuda")
-    activation_checkpointing: float = 0.0
-    module_shapes: Dict[str, torch.Size] = None
+    def __init__(
+        self,
+        dtype: torch.dtype = torch.half,
+        device: torch.device = None,
+        activation_checkpointing: float = 0.0,
+        module_shapes: Dict[str, torch.Size] = None,
+    ) -> None:
+        self.dtype = dtype
+        if device is None:
+            self.device = get_current_device()
+        else:
+            self.device = device
+        self.activation_checkpointing = activation_checkpointing
+        self.module_shapes = module_shapes
 
 
 class MemoryPool:
     """
     memory pool for isp communication.
     """
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/core/communication/p2p.py` & `InternEvo-0.4.0.dev20240403/internlm/core/communication/p2p.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 import operator
 from functools import reduce
 from typing import List, Tuple, Union
 
 import torch
 import torch.distributed as dist
 
+from internlm.accelerator import get_accelerator
 from internlm.core.context import ParallelMode
 from internlm.core.context import global_context as gpc
 from internlm.utils.common import get_current_device
 
 from .utils import gather_split_1d_tensor, split_tensor_into_1d_equal_chunks
 
 TensorShape = Union[torch.Size, List[int], Tuple[int]]
+internlm_accelerator = get_accelerator()
 
 
 def _get_tensor_shape(tensor_shape: TensorShape, chunk_tensor: bool = False) -> Tuple[TensorShape, bool]:
     """get the exact tensor shape when communicating and return whether the tensor is a chunk
 
     Args:
         tensor_shape (:class:`torch.Size`): shape of tensor
@@ -167,15 +169,15 @@
         filling_ops_queue(object_send_next, dist.isend, next_rank, ops)
 
     if len(ops) > 0:
         reqs = dist.batch_isend_irecv(ops)
         for req in reqs:
             req.wait()
     # To protect against race condition when using batch_isend_irecv().
-    torch.cuda.synchronize()
+    internlm_accelerator.synchronize()
 
     if recv_prev and recv_prev_split:
         if isinstance(tensor_recv_prev, torch.Tensor):
             tensor_recv_prev = gather_split_1d_tensor(tensor_recv_prev).view(recv_prev_shape).requires_grad_()
         else:
             for index in range(len(tensor_recv_prev)):
                 tensor_recv_prev[index] = (
@@ -467,15 +469,15 @@
     # return and do other things
     yield
 
     # check communication completed
     for req in reqs:
         req.wait()
     # To protect against race condition when using batch_isend_irecv()
-    torch.cuda.synchronize()
+    internlm_accelerator.synchronize()
 
     # Process received data
     if recv_prev_shape is not None and recv_prev_split:
         if isinstance(tensor_recv_prev, torch.Tensor):
             tensor_recv_prev = gather_split_1d_tensor(tensor_recv_prev).view(recv_prev_shape).requires_grad_()
         else:
             for index in range(len(tensor_recv_prev)):
@@ -527,15 +529,15 @@
     # return and do other things
     yield
 
     # check communication completed
     for req in reqs:
         req.wait()
     # To protect against race condition when using batch_isend_irecv()
-    torch.cuda.synchronize()
+    internlm_accelerator.synchronize()
 
     # Process received data
     if recv_next_shape is not None and recv_next_split:
         if isinstance(tensor_recv_next, torch.Tensor):
             tensor_recv_next = gather_split_1d_tensor(tensor_recv_next).view(recv_next_shape).requires_grad_()
         else:
             for index in range(len(tensor_recv_next)):
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/core/communication/utils.py` & `InternEvo-0.4.0.dev20240403/internlm/core/communication/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # adopted from https://github.com/hpcaitech/ColossalAI/blob/main/colossalai/communication
 
 from collections import OrderedDict
 from typing import Dict, List, Tuple, Union
 
 import torch
 import torch.distributed as dist
-from flash_attn.modules.embedding import ParallelGPT2Embeddings
 from torch import nn
 
 from internlm.core.communication.isp import ISPCommunicator
 from internlm.core.context import ParallelMode
 from internlm.core.context import global_context as gpc
 from internlm.core.naive_amp import NaiveAMPModel
-from internlm.model.embedding import Embedding1D
-from internlm.model.linear import BaseScaleColumnParallelLinear
+from internlm.model.modules.embedding import Embedding1D
+from internlm.model.ops.linear import BaseScaleColumnParallelLinear
 from internlm.utils.common import get_current_device
 
 TensorShape = Union[torch.Size, List[int], Tuple[int]]
 
 
 def send_meta_helper(obj, next_rank, tensor_kwargs):
     send_shape = torch.tensor(obj.size(), **tensor_kwargs)
@@ -104,15 +103,15 @@
     Returns:
         :class:`torch.Tensor`: The split tensor
     """
     partition_size = torch.numel(tensor) // gpc.get_world_size(ParallelMode.TENSOR)
     start_index = partition_size * gpc.get_local_rank(ParallelMode.TENSOR)
     end_index = start_index + partition_size
     if new_buffer:
-        data = torch.empty(partition_size, dtype=tensor.dtype, device=torch.cuda.current_device(), requires_grad=False)
+        data = torch.empty(partition_size, dtype=tensor.dtype, device=get_current_device(), requires_grad=False)
         data.copy_(tensor.view(-1)[start_index:end_index])
     else:
         data = tensor.view(-1)[start_index:end_index]
     return data
 
 
 def gather_split_1d_tensor(tensor: torch.Tensor) -> torch.Tensor:
@@ -122,15 +121,15 @@
         tensor (:class:`torch.Tensor`): Tensor to be gathered after communication.
     Returns:
         :class:`torch.Tensor`: The gathered tensor.
     """
     world_size = gpc.get_world_size(ParallelMode.TENSOR)
     numel = torch.numel(tensor)
     numel_gathered = world_size * numel
-    gathered = torch.empty(numel_gathered, dtype=tensor.dtype, device=torch.cuda.current_device(), requires_grad=False)
+    gathered = torch.empty(numel_gathered, dtype=tensor.dtype, device=get_current_device(), requires_grad=False)
     chunks = [gathered[i * numel : (i + 1) * numel] for i in range(world_size)]
     dist.all_gather(chunks, tensor, group=gpc.get_group(ParallelMode.TENSOR))
     return gathered
 
 
 class ParamAsyncBcastHandler:
     """
@@ -213,17 +212,22 @@
         for block, _ in self._block_to_rank.items():
             # TODO: remove special handling for embedding and head layers,
             # instead implement support for weight parallelism of embedding and head layers within the ISP.
 
             # NOTE: Although the layernorm layer does not have explicit processing,
             # both ISPCommunicator and ParamAsyncBcastHandler handle transformer blocks as granularity,
             # so everything is fine.
-            if isp_communicator is None or isinstance(
-                block, (Embedding1D, ParallelGPT2Embeddings, BaseScaleColumnParallelLinear)
-            ):
+
+            embedding_head_cls = (Embedding1D, BaseScaleColumnParallelLinear)
+            if gpc.config.use_cuda_flash_attn:
+                from flash_attn.modules.embedding import ParallelGPT2Embeddings
+
+                embedding_head_cls = (Embedding1D, ParallelGPT2Embeddings, BaseScaleColumnParallelLinear)
+
+            if isp_communicator is None or isinstance(block, embedding_head_cls):
                 block.register_forward_pre_hook(_pre_forward_hook)
         if isp_communicator:
             isp_communicator.register_prerequisite_for_forward_prefetch_hooks(_pre_forward_hook)
 
     def get_rank_by_param(self, param) -> int:
         return self._param_to_rank[param]
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/core/context/__init__.py` & `InternEvo-0.4.0.dev20240403/internlm/core/context/__init__.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.3.3.dev20240315/internlm/core/context/parallel_context.py` & `InternEvo-0.4.0.dev20240403/internlm/core/context/parallel_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 
 # adopted from https://github.com/hpcaitech/ColossalAI/blob/main/colossalai/context
 
 import inspect
 import random
 import socket
 import sys
-from collections import Counter
 from importlib.machinery import SourceFileLoader
 from pathlib import Path
 from typing import Union
 
 import numpy as np
 import torch
 import torch.distributed as dist
 
+from internlm.accelerator import get_accelerator
 from internlm.utils.common import SingletonMeta
 from internlm.utils.logger import get_logger
 from internlm.utils.timeout import LLM_NCCL_TIMEOUT
 
 from . import process_group_initializer as pgroup_initializer
 from .process_group_initializer import ParallelMode
 from .random import add_seed, get_seeds, set_mode
@@ -29,14 +29,15 @@
 IS_TENSOR_DATA_PARALLEL = "is_tensor_data_parallel"
 # for mtp/msp/fsp, with optimizer split in zero1 group
 IS_TENSOR_ZERO_PARALLEL = "is_tensor_zero_parallel"
 IS_WEIGHT_ZERO_PARALLEL = "is_weight_zero_parallel"
 IS_TENSOR_EXPERT_DATA_PARALLEL = "is_tensor_expert_data_parallel"
 
 logger = get_logger(__file__)
+internlm_accelerator = get_accelerator()
 
 
 class Config(dict):
     """This is a wrapper class for dict objects so that values of which can be
     accessed as attributes.
 
     Args:
@@ -192,21 +193,14 @@
         if isinstance(config, str):
             self._config = Config.from_file(config)
         elif isinstance(config, dict):
             self._config = Config(config)
         else:
             raise TypeError("Invalid type for config, only dictionary or string is supported")
 
-    def detect_num_processes_on_current_node(self):
-        hostname = socket.gethostname()
-        hostname_list = [None for _ in range(self.get_world_size(ParallelMode.GLOBAL))]
-        dist.all_gather_object(hostname_list, hostname, group=self.get_group(ParallelMode.GLOBAL))
-        counter = Counter(hostname_list)
-        self.num_processes_on_current_node = counter[hostname]
-
     @staticmethod
     def _check_parallel_mode(parallel_mode: ParallelMode):
         assert isinstance(
             parallel_mode, ParallelMode
         ), f"expected the argument parallel_mode to be of enum ParallelMode, but got {type(parallel_mode)}"
 
     def get_global_rank(self):
@@ -608,33 +602,33 @@
         """Sets distributed processes to be bound to devices.
 
         Args:
            device_ordinal (int, optional): the device id to be bound to
         """
         global_rank = self.get_global_rank()
         if device_ordinal is None:
-            devices_per_node = torch.cuda.device_count()
+            devices_per_node = internlm_accelerator.device_count()
             device_ordinal = global_rank % devices_per_node
 
-        torch.cuda.set_device(device_ordinal)
+        internlm_accelerator.set_device(device_ordinal)
         logger.info(f"process rank {global_rank} is bound to host:{socket.gethostname()} device: {device_ordinal}")
 
     def set_seed(self, seed: int, dpseed_with_tpoffset: bool = False):
         """Sets seeds for all random libraries.
 
         Args:
             seed (int): seed for random states
         """
         pipeline_offset = self._local_ranks.get(ParallelMode.PIPELINE, 0)
         global_rank = self.get_global_rank()
 
         random.seed(seed)
         np.random.seed(seed)
         torch.manual_seed(seed)
-        assert torch.cuda.is_available()
+        assert internlm_accelerator.is_available()
 
         # data parallel seed are kept the same in the same pipeline stage
         dp_seed = seed
         if dpseed_with_tpoffset:
             dp_seed = seed + pipeline_offset * 1024
         add_seed(ParallelMode.DATA, dp_seed)
         add_seed(ParallelMode.WEIGHT_DATA, dp_seed)
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/core/context/process_group_initializer.py` & `InternEvo-0.4.0.dev20240403/internlm/core/context/process_group_initializer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.3.3.dev20240315/internlm/core/context/random.py` & `InternEvo-0.4.0.dev20240403/internlm/core/context/random.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 #!/usr/bin/env python
 # -*- encoding: utf-8 -*-
 # adopted from https://github.com/hpcaitech/ColossalAI/blob/main/colossalai/context
 
 from contextlib import contextmanager
 
-import torch
-import torch.cuda
 from torch import Tensor
 
+from internlm.accelerator import get_accelerator
+
 from .process_group_initializer import ParallelMode
 
+internlm_accelerator = get_accelerator()
+
 
 class SeedManager:
     """This class is a manager of all random seeds involved in the system."""
 
     def __init__(self):
         self._current_mode = None
         self._seeds = {}
@@ -32,37 +34,37 @@
         return self._seed_states
 
     def set_state(self, parallel_mode: ParallelMode, state: Tensor):
         """Sets the state of the seed manager for `parallel_mode`."""
         assert parallel_mode in self._seed_states, f"{parallel_mode} not found in seed manager"
         self._seed_states[parallel_mode] = state
 
-    def set_mode(self, parallel_mode: ParallelMode):
+    def set_mode(self, parallel_mode: ParallelMode, update_rng_current_mode: bool = True):
         """Sets the current mode of the seed manager."""
-        if self.current_mode:
+        if update_rng_current_mode and self.current_mode:
             # save state for current mode
-            self._seed_states[self._current_mode] = torch.cuda.get_rng_state()
+            self._seed_states[self._current_mode] = internlm_accelerator.get_rng_state()
 
         # set new state for new mode
         self._current_mode = parallel_mode
-        torch.cuda.set_rng_state(self._seed_states[parallel_mode])
+        internlm_accelerator.set_rng_state(self._seed_states[parallel_mode])
 
     def add_seed(self, parallel_mode: ParallelMode, seed: int, overwrite: bool = False):
         """Adds a seed to the seed manager for `parallel_mode`."""
         assert isinstance(parallel_mode, ParallelMode), "Invalid ParallelMode"
         if not overwrite:
             assert parallel_mode not in self._seed_states, f"Seed for {parallel_mode} exists"
         elif parallel_mode in self._seed_states:
             print(f"Warning: {parallel_mode} seed overwritten.", flush=True)
 
-        current_state = torch.cuda.get_rng_state()
-        torch.cuda.manual_seed(seed)
-        self._seed_states[parallel_mode] = torch.cuda.get_rng_state()
+        current_state = internlm_accelerator.get_rng_state()
+        internlm_accelerator.manual_seed(seed)
+        self._seed_states[parallel_mode] = internlm_accelerator.get_rng_state()
         self._seeds[parallel_mode] = seed
-        torch.cuda.set_rng_state(current_state)
+        internlm_accelerator.set_rng_state(current_state)
 
     def reset(self):
         self._current_mode = None
         self._seeds = {}
         self._seed_states = {}
 
 
@@ -101,27 +103,27 @@
 
 
 def add_seed(parallel_mode: ParallelMode, seed: int, overwrite: bool = False):
     """Adds a seed to the seed manager for `parallel_mode`."""
     _SEED_MANAGER.add_seed(parallel_mode, seed, overwrite)
 
 
-def set_mode(parallel_mode: ParallelMode):
+def set_mode(parallel_mode: ParallelMode, update_rng_current_mode: bool = True):
     """Sets the current mode of the seed manager."""
-    _SEED_MANAGER.set_mode(parallel_mode)
+    _SEED_MANAGER.set_mode(parallel_mode, update_rng_current_mode=update_rng_current_mode)
 
 
 def set_seed_states(parallel_mode: ParallelMode, state: Tensor):
     """Sets the state of the seed manager for `parallel_mode`."""
     _SEED_MANAGER.set_state(parallel_mode, state)
 
 
 def sync_states():
     current_mode = get_current_mode()
-    current_states = torch.cuda.get_rng_state()
+    current_states = internlm_accelerator.get_rng_state()
     set_seed_states(current_mode, current_states)
 
 
 @contextmanager
 def seed(parallel_mode: ParallelMode):
     """A context for seed switch"""
     current_mode = _SEED_MANAGER.current_mode
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/core/engine.py` & `InternEvo-0.4.0.dev20240403/internlm/core/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 import torch
 from torch.nn import Module
 from torch.nn.modules.loss import _Loss
 from torch.optim.lr_scheduler import _LRScheduler
 
 from internlm.core.gradient_handler import BaseGradientHandler
-from internlm.solver.beta2_scheduler import Beta2Scheduler
 from internlm.solver.optimizer.hybrid_zero_optim import BaseOptimizer
+from internlm.solver.schedulers.beta2_scheduler import Beta2Scheduler
 from internlm.utils.common import get_batch_size, move_to_device
 
 
 class Engine:
     """
     The Engine class is responsible for managing the training and evaluation process of a neural network model.
     It handles the forward and backward passes, parameter updates, gradient handling, and mode switching between
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/core/gradient_handler.py` & `InternEvo-0.4.0.dev20240403/internlm/core/gradient_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/usr/bin/env python
 # -*- encoding: utf-8 -*-
 
 from abc import ABC, abstractmethod
 from collections import defaultdict
 
-import torch
 import torch.distributed as dist
 from torch._utils import _flatten_dense_tensors, _unflatten_dense_tensors
 
 from internlm.core.context import global_context as gpc
+from internlm.utils.common import get_current_device
 
 
 class BaseGradientHandler(ABC):
     """A basic helper class to handle all-reduce operations of gradients across different parallel groups
     before optimization.
 
     Args:
@@ -66,11 +66,11 @@
             # For each bucket, all-reduce and copy all-reduced grads.
             for group, group_buckets in buckets.items():
                 for tp, bucket in group_buckets.items():
                     grads = [
                         param.colo_attr.grad_payload if hasattr(param, "colo_attr") else param.grad.data
                         for param in bucket
                     ]
-                    coalesced = _flatten_dense_tensors(grads).to(torch.cuda.current_device())
+                    coalesced = _flatten_dense_tensors(grads).to(get_current_device())
                     dist.all_reduce(coalesced, op=dist.ReduceOp.SUM, group=group)
                     for buf, synced in zip(grads, _unflatten_dense_tensors(coalesced, grads)):
                         buf.copy_(synced)
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/core/naive_amp.py` & `InternEvo-0.4.0.dev20240403/internlm/core/naive_amp.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,17 +8,20 @@
 
 import torch
 import torch.distributed as dist
 from torch import Tensor, nn
 from torch._utils import _flatten_dense_tensors, _unflatten_dense_tensors
 from torch.distributed import ReduceOp
 
+from internlm.accelerator import AcceleratorType, get_accelerator
 from internlm.core.context import ParallelMode
 from internlm.core.context.parallel_context import global_context as gpc
 
+internlm_accelerator = get_accelerator()
+
 
 def set_fp32_attr_to_module(module: nn.Module):
     setattr(module, "is_fp32_module", True)
 
 
 def module_has_fp32_attr(module: nn.Module):
     return hasattr(module, "is_fp32_module") and getattr(module, "is_fp32_module")
@@ -170,15 +173,15 @@
         def _pre_forward_hook_for_fp32(model: nn.Module, inputs: tuple):  # pylint: disable=W0613
             assert isinstance(inputs, tuple)
             return tuple(map(to_dtype, inputs))
 
         def _post_forward_hook_for_fp32(
             model: nn.Module, inputs: tuple, outputs: Union[tuple, Tensor]
         ):  # pylint: disable=W0613
-            assert isinstance(inputs, Union[tuple, Tensor])
+            assert isinstance(inputs, (tuple, Tensor))
             if isinstance(outputs, tuple):
                 return tuple(map(to_dtype, outputs, [self.dtype] * len(outputs)))
             else:
                 return to_dtype(outputs, self.dtype)
 
         # just want to share same for loop for ModuleList and Module
         if isinstance(self.model, nn.ModuleList):
@@ -195,10 +198,11 @@
         for sub_module in modules:
             if module_has_fp32_attr(sub_module):
                 sub_module.to(fp32_dtype)
                 sub_module.register_forward_pre_hook(partial(_pre_forward_hook_for_fp32))
                 sub_module.register_forward_hook(partial(_post_forward_hook_for_fp32))
             if gpc.config.get("output_tf32", False) and module_is_output(sub_module):
                 sub_module.to(fp32_dtype)
-                torch.backends.cudnn.allow_tf32 = True
-                torch.backends.cuda.matmul.allow_tf32 = True
+                if internlm_accelerator.get_accelerator_backend() == AcceleratorType.GPU:
+                    torch.backends.cudnn.allow_tf32 = True
+                    torch.backends.cuda.matmul.allow_tf32 = True
                 sub_module.register_forward_pre_hook(partial(_pre_forward_hook_for_fp32))
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/core/scheduler/base_scheduler.py` & `InternEvo-0.4.0.dev20240403/internlm/core/scheduler/base_scheduler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.3.3.dev20240315/internlm/core/scheduler/no_pipeline_scheduler.py` & `InternEvo-0.4.0.dev20240403/internlm/core/scheduler/no_pipeline_scheduler.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,20 @@
 
 import torch
 import torch.distributed as dist
 
 from internlm.core.context import ParallelMode
 from internlm.core.context import global_context as gpc
 from internlm.core.engine import Engine
-from internlm.utils.common import SchedulerHook, conditional_context
+from internlm.utils.common import (
+    SchedulerHook,
+    check_data_is_packed,
+    conditional_context,
+    get_current_device,
+)
 from internlm.utils.logger import get_logger
 from internlm.utils.timeout import llm_timeout
 
 from .base_scheduler import BaseScheduler
 
 logger = get_logger(__file__)
 
@@ -70,20 +75,22 @@
         """Loads a batch of data and label for gradient accumulation.
 
         Args:
             data (Any): The data to be loaded.
             label (Any): The label to be loaded.
         """
 
-        _data, _label = self._load_micro_batch(data=data, label=label, offset=self._grad_accum_offset, bsz_stride=1)
-        self._grad_accum_offset += 1
+        _data, _label = self._load_micro_batch(
+            data=data, label=label, offset=self._grad_accum_offset, bsz_stride=self._bsz_stride
+        )
+        self._grad_accum_offset += self._bsz_stride
 
         if self.data_process_func:
             _data["input_ids"] = self.data_process_func(_data["input_ids"], _data["cu_seqlens"])
-            _label = self.data_process_func(_label, _data["cu_seqlens"])
+            _label = self.data_process_func(_label, _data["cu_seqlens"], padding_v=-100)
             _data.pop("cu_seqlens")
             _data.pop("indexes")
 
         return _data, _label
 
     def _train_one_batch(
         self,
@@ -123,15 +130,15 @@
             if return_loss:
                 self._call_hooks("before_criterion", output, label)
                 loss = self._call_engine_criterion(engine, output, label)
                 self._call_hooks("after_criterion", loss)
                 moe_loss = (
                     sum(moe_losses) * gpc.config.loss.moe_loss_coeff
                     if hasattr(gpc.config.model, "num_experts") and gpc.config.model.num_experts > 1
-                    else torch.tensor(0.0, device=torch.cuda.current_device(), dtype=gpc.config.model.get("dtype"))
+                    else torch.tensor(0.0, device=get_current_device(), dtype=gpc.config.model.get("dtype"))
                 )
                 # the moe_loss is computed among the "tensor" group if sequence parallel is enabled,
                 # so we need to do allreduce
                 if gpc.config.parallel.sequence_parallel:
                     dist.all_reduce(moe_loss, op=dist.ReduceOp.AVG, group=gpc.get_group(ParallelMode.TENSOR))
                 moe_loss /= scale_loss
                 loss /= scale_loss
@@ -175,17 +182,25 @@
         Returns:
             Tuple[:class:`torch.Tensor`]: A tuple of (output, label, loss), loss and label could be None.
         """
         assert (
             forward_only or return_loss
         ), "The argument 'return_loss' has to be True when 'forward_only' is False, but got False."
 
-        batch_data, actual_batch_size = engine.load_batch(data_iter)  # actual_batch_size is micro_num
+        # actual_batch_size is micro_num when training,
+        # actual_batch_size is micro_num * micro_bsz when evaluating
+        batch_data, actual_batch_size = engine.load_batch(data_iter)
+
+        if check_data_is_packed(batch_data):
+            micro_num = actual_batch_size
+        else:
+            micro_num = actual_batch_size // gpc.config.data["micro_bsz"]
 
-        self._grad_accum_size = actual_batch_size  # Rampup or variable bsz size.
+        self._grad_accum_size = micro_num  # Rampup or variable bsz size.
+        self._bsz_stride = actual_batch_size // self._grad_accum_size
 
         data, label = batch_data
 
         loss = 0 if return_loss else None
         moe_loss = 0 if return_loss else None
         outputs = []
         labels = []
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/core/scheduler/pipeline_scheduler.py` & `InternEvo-0.4.0.dev20240403/internlm/core/scheduler/pipeline_scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- encoding: utf-8 -*-
 
 # adopted from https://github.com/hpcaitech/ColossalAI/blob/main/colossalai/engine
 
 from contextlib import contextmanager
 from typing import Callable, List, Optional, Tuple, Union
 
-import torch.cuda
+import torch
 import torch.distributed as dist
 
 import internlm.core.communication as comm
 from internlm.core.context import ParallelMode
 from internlm.core.context import global_context as gpc
 from internlm.core.engine import Engine
 from internlm.core.naive_amp import NaiveAMPModel
@@ -32,33 +32,43 @@
     if hasattr(gpc.config, "TENSOR_SHAPE"):
         return gpc.config.TENSOR_SHAPE
 
     if not gpc.is_initialized(ParallelMode.PIPELINE):
         return None
 
     if hasattr(gpc.config, "SEQ_LEN") and hasattr(gpc.config.data, "micro_bsz") and hasattr(gpc.config, "HIDDEN_SIZE"):
-        if gpc.config.model.use_flash_attn:
+        if gpc.config.data.use_packed_dataset and gpc.is_evaluating is False:
             if gpc.config.parallel.sequence_parallel:
                 sequence_world_size = gpc.get_world_size(ParallelMode.TENSOR)
                 tensor_shape = (
+                    1,
                     gpc.config.data["seq_len"] * gpc.config.data["micro_bsz"] // sequence_world_size,
                     gpc.config.model["hidden_size"],
                 )
             else:
                 tensor_shape = (
+                    1,
                     gpc.config.data["seq_len"] * gpc.config.data["micro_bsz"],
                     gpc.config.model["hidden_size"],
                 )
         else:
-            tensor_shape = (
-                gpc.config.data["micro_bsz"],
-                gpc.config.data["seq_len"],
-                gpc.config.model["hidden_size"],
-            )
-        return tensor_shape
+            if gpc.config.parallel.sequence_parallel:
+                sequence_world_size = gpc.get_world_size(ParallelMode.TENSOR)
+                tensor_shape = (
+                    gpc.config.data["micro_bsz"],
+                    gpc.config.data["seq_len"] // sequence_world_size,
+                    gpc.config.model["hidden_size"],
+                )
+            else:
+                tensor_shape = (
+                    gpc.config.data["micro_bsz"],
+                    gpc.config.data["seq_len"],
+                    gpc.config.model["hidden_size"],
+                )
+        return torch.Size(tensor_shape)
     else:
         return None
 
 
 def pack_return_tensors(return_tensors):
     output, label = tuple(zip(*return_tensors))
     if isinstance(output[0], torch.Tensor):
@@ -210,15 +220,17 @@
         micro_batch_data, micro_batch_label = self._load_micro_batch(
             data=self.batch_data, label=self.batch_label, offset=self.microbatch_offset, bsz_stride=self.bsz_stride
         )
         if self.data_process_func:
             micro_batch_data["input_ids"] = self.data_process_func(
                 micro_batch_data["input_ids"], micro_batch_data["cu_seqlens"]
             )
-            micro_batch_label = self.data_process_func(micro_batch_label, micro_batch_data["cu_seqlens"])
+            micro_batch_label = self.data_process_func(
+                micro_batch_label, micro_batch_data["cu_seqlens"], padding_v=-100
+            )
 
             micro_batch_data.pop("cu_seqlens")
             micro_batch_data.pop("indexes")
 
         micro_batch_data["label"] = micro_batch_label
         self.microbatch_offset += self.bsz_stride
 
@@ -302,15 +314,15 @@
                 loss_reduced = loss / self.num_microbatches
                 accum_loss.add_(loss_reduced.detach())
                 output_obj = loss_reduced
 
         moe_loss = (
             sum(moe_losses) * gpc.config.loss.moe_loss_coeff
             if hasattr(gpc.config.model, "num_experts") and gpc.config.model.num_experts > 1
-            else torch.tensor(0.0, device=torch.cuda.current_device(), dtype=gpc.config.model.get("dtype"))
+            else torch.tensor(0.0, device=get_current_device(), dtype=gpc.config.model.get("dtype"))
         )
         # the moe_loss is computed among the "tensor" group if sequence parallel is enabled, so we need to do allreduce
         if gpc.config.parallel.sequence_parallel:
             dist.all_reduce(moe_loss, op=dist.ReduceOp.AVG, group=gpc.get_group(ParallelMode.TENSOR))
         moe_loss /= self.num_microbatches
         accum_moe_loss.add_(moe_loss.detach())
 
@@ -728,15 +740,15 @@
             scatter_gather_tensors (bool, optional):
                 If set to `True`, communication will be reduced over pipeline when using 1D tensor parallelization.
             scheduler_hooks (List[SchedulerHook], optional): List of scheduler hooks. Default is None.
             communication_overlap (bool, optional): Whether to enable communication overlap. Default is False.
         """
         assert (
             num_microbatches % gpc.get_world_size(ParallelMode.PIPELINE) == 0
-        ), "num_microbatches must be an integer multiple of pipeline parallel world size"
+        ), f"num_microbatches: {num_microbatches} must be an integer multiple of pipeline parallel world size"
 
         assert (
             isinstance(num_chunks, int) and num_chunks > 0
         ), f"expected num_chunks to be an integer and larger than 0, but got {num_chunks}"
 
         super().__init__(
             num_microbatches,
@@ -808,15 +820,17 @@
             offset=self.microbatch_offset[model_chunk_id],
             bsz_stride=self.bsz_stride,
         )
         if self.data_process_func:
             micro_batch_data["input_ids"] = self.data_process_func(
                 micro_batch_data["input_ids"], micro_batch_data["cu_seqlens"]
             )
-            micro_batch_label = self.data_process_func(micro_batch_label, micro_batch_data["cu_seqlens"])
+            micro_batch_label = self.data_process_func(
+                micro_batch_label, micro_batch_data["cu_seqlens"], padding_v=-100
+            )
 
             micro_batch_data.pop("cu_seqlens")
             micro_batch_data.pop("indexes")
 
         micro_batch_data["label"] = micro_batch_label
         self.microbatch_offset[model_chunk_id] += self.bsz_stride
         return move_to_device(micro_batch_data)
@@ -865,15 +879,15 @@
                 loss_reduced = loss / self.num_microbatches
                 self._accum_loss.add_(loss_reduced.detach())
                 output_obj = loss_reduced
 
         moe_loss = (
             sum(moe_losses) * gpc.config.loss.moe_loss_coeff
             if hasattr(gpc.config.model, "num_experts") and gpc.config.model.num_experts > 1
-            else torch.tensor(0.0, device=torch.cuda.current_device(), dtype=gpc.config.model.get("dtype"))
+            else torch.tensor(0.0, device=get_current_device(), dtype=gpc.config.model.get("dtype"))
         )
         # the moe_loss is computed among the "tensor" group if sequence parallel is enabled, so we need to do allreduce
         if gpc.config.parallel.sequence_parallel:
             dist.all_reduce(moe_loss, op=dist.ReduceOp.AVG, group=gpc.get_group(ParallelMode.TENSOR))
         moe_loss /= self.num_microbatches
 
         if self._accum_moe_loss is not None:
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/core/trainer.py` & `InternEvo-0.4.0.dev20240403/internlm/core/trainer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.3.3.dev20240315/internlm/data/batch_sampler.py` & `InternEvo-0.4.0.dev20240403/internlm/data/tokenized/batch_sampler.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -103,82 +103,14 @@
 
         Args:
             epoch (int): Epoch number.
         """
         self.epoch = epoch
 
 
-def get_dpsampler_dataloader(
-    dataset,
-    shuffle=False,
-    seed=1024,
-    add_sampler=True,
-    drop_last=False,
-    pin_memory=False,
-    num_workers=0,
-    **kwargs,
-):
-    r"""Set up a deterministic dataloader (also configure seed workers, samplers and whether shuffle or not)
-
-    Note:
-        When pipeline parallel is enabled, shuffle cannot be True as it will result in mismatch between input data
-        on the 1st stage and label on the last stage.
-
-    Args:
-        dataset (:class:`torch.utils.data.Dataset`): The dataset to be loaded.
-        shuffle (bool, optional): Whether to shuffle the dataset. Defaults to False.
-        seed (int, optional): Random worker seed for sampling, defaults to 1024.
-        add_sampler: Whether to add ``DistributedDataParallelSampler`` to the dataset. Defaults to True.
-        drop_last (bool, optional): Set to True to drop the last incomplete batch, if the dataset size
-            is not divisible by the batch size. If False and the size of dataset is not divisible by
-            the batch size, then the last batch will be smaller, defaults to False.
-        pin_memory (bool, optional): Whether to pin memory address in CPU memory. Defaults to False.
-        num_workers (int, optional): Number of worker threads for this dataloader. Defaults to 0.
-        kwargs (dict): optional parameters for ``torch.utils.data.DataLoader``, more details could be found in
-                `DataLoader <https://pytorch.org/docs/stable/_modules/torch/utils/data/dataloader.html#DataLoader>`_.
-
-    Returns:
-        :class:`torch.utils.data.DataLoader`: A DataLoader used for training or testing.
-    """
-    _kwargs = kwargs.copy()
-
-    if add_sampler and gpc.is_using_parallel_mode(ParallelMode.DATA):
-        sampler = DataParallelSampler(dataset, shuffle=shuffle, drop_last=drop_last)
-    else:
-        sampler = None
-
-    # Deterministic dataloader
-    def seed_worker():
-        worker_seed = seed
-        np.random.seed(worker_seed)
-        torch.manual_seed(worker_seed)
-        random.seed(worker_seed)
-
-    if sampler is None:
-        return DataLoader(
-            dataset,
-            worker_init_fn=seed_worker,
-            shuffle=shuffle,
-            drop_last=drop_last,
-            pin_memory=pin_memory,
-            num_workers=num_workers,
-            **_kwargs,
-        )
-    else:
-        return DataLoader(
-            dataset,
-            sampler=sampler,
-            worker_init_fn=seed_worker,
-            drop_last=drop_last,
-            pin_memory=pin_memory,
-            num_workers=num_workers,
-            **_kwargs,
-        )
-
-
 class StaticBatchSampler:
     """
     A static batch sampler that generates batches with a fixed micro-batch size.
 
     Args:
         num_samples (int): The total number of samples in the dataset.
         batch_size (int): The batch size for the current rank. Defaults to 192.
@@ -349,7 +281,75 @@
             drop_last=True,
             data_rank=self.data_rank,
             data_world_size=self.data_world_size,
         )
 
         copy_sampler.load_state_dict(self.state_dict())
         return copy_sampler
+
+
+def get_dpsampler_dataloader(
+    dataset,
+    shuffle=False,
+    seed=1024,
+    add_sampler=True,
+    drop_last=False,
+    pin_memory=False,
+    num_workers=0,
+    **kwargs,
+):
+    r"""Set up a deterministic dataloader (also configure seed workers, samplers and whether shuffle or not)
+
+    Note:
+        When pipeline parallel is enabled, shuffle cannot be True as it will result in mismatch between input data
+        on the 1st stage and label on the last stage.
+
+    Args:
+        dataset (:class:`torch.utils.data.Dataset`): The dataset to be loaded.
+        shuffle (bool, optional): Whether to shuffle the dataset. Defaults to False.
+        seed (int, optional): Random worker seed for sampling, defaults to 1024.
+        add_sampler: Whether to add ``DistributedDataParallelSampler`` to the dataset. Defaults to True.
+        drop_last (bool, optional): Set to True to drop the last incomplete batch, if the dataset size
+            is not divisible by the batch size. If False and the size of dataset is not divisible by
+            the batch size, then the last batch will be smaller, defaults to False.
+        pin_memory (bool, optional): Whether to pin memory address in CPU memory. Defaults to False.
+        num_workers (int, optional): Number of worker threads for this dataloader. Defaults to 0.
+        kwargs (dict): optional parameters for ``torch.utils.data.DataLoader``, more details could be found in
+                `DataLoader <https://pytorch.org/docs/stable/_modules/torch/utils/data/dataloader.html#DataLoader>`_.
+
+    Returns:
+        :class:`torch.utils.data.DataLoader`: A DataLoader used for training or testing.
+    """
+    _kwargs = kwargs.copy()
+
+    if add_sampler and gpc.is_using_parallel_mode(ParallelMode.DATA):
+        sampler = DataParallelSampler(dataset, shuffle=shuffle, drop_last=drop_last)
+    else:
+        sampler = None
+
+    # Deterministic dataloader
+    def seed_worker():
+        worker_seed = seed
+        np.random.seed(worker_seed)
+        torch.manual_seed(worker_seed)
+        random.seed(worker_seed)
+
+    if sampler is None:
+        return DataLoader(
+            dataset,
+            worker_init_fn=seed_worker,
+            shuffle=shuffle,
+            drop_last=drop_last,
+            pin_memory=pin_memory,
+            num_workers=num_workers,
+            **_kwargs,
+        )
+    else:
+        return DataLoader(
+            dataset,
+            sampler=sampler,
+            worker_init_fn=seed_worker,
+            drop_last=drop_last,
+            pin_memory=pin_memory,
+            num_workers=num_workers,
+            **_kwargs,
+        )
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/data/collaters.py` & `InternEvo-0.4.0.dev20240403/internlm/data/tokenized/collaters.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.3.3.dev20240315/internlm/data/dataset.py` & `InternEvo-0.4.0.dev20240403/internlm/data/tokenized/dataset.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from typing import Dict
 
 from torch.utils.data import ConcatDataset
 
-from internlm.data.single_dataset import JsonlDataset
+from internlm.data.tokenized.single_dataset import JsonlDataset
 
 
 def get_dataset_dict(folder, split="valid") -> Dict:
     """
     Return a dictionary of Datasets from a folder containing data files for validation.
 
     Args:
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/data/dummy_dataset.py` & `InternEvo-0.4.0.dev20240403/internlm/data/tokenized/dummy_dataset.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,23 +11,28 @@
 
     Args:
         num_samples (int): The number of samples to generate.
         max_len (int): The maximum length of each sample.
 
     """
 
-    def __init__(self, num_samples=10000, max_len=1024) -> None:
+    def __init__(self, num_samples=10000, max_len=1024, fixed_seqlen: bool = False) -> None:
         super().__init__()
         rng = np.random.RandomState(1999)
         max_num = rng.randint(1, 30, size=(num_samples,))
         rep_num = rng.randint(10, 200, size=(num_samples,))
         data = []
         lengths = []
         for n, r in zip(max_num, rep_num):
             d = list(range(n)) * r
+            if fixed_seqlen:
+                while len(d) < max_len:
+                    r *= 2
+                    d = list(range(n)) * r
+
             d = [n, r] + d
             d = d[:max_len]
             data.append(d)
             lengths.append(len(d))
         self.data = data
         self.max_len = max_len
         self.lengths = np.array(lengths, dtype=int)
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/data/packed_dataset.py` & `InternEvo-0.4.0.dev20240403/internlm/data/tokenized/packed_dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 import os
 from copy import deepcopy
 from typing import Dict
 
 import numpy as np
 import torch
 import torch.distributed as dist
-from torch.utils.data import ConcatDataset
+from torch.utils.data import ConcatDataset, Dataset
 from tqdm import tqdm
 
 from internlm.core.context import global_context as gpc
-from internlm.data.single_dataset import JsonlDataset
+from internlm.data.tokenized.single_dataset import JsonlDataset
 from internlm.data.utils import get_dataset_type_id, get_dataset_type_ids_map
 from internlm.utils.logger import get_logger
 
 DEFAULT_SEED = 1024
 logger = get_logger(__file__)
 
 
-class PackedDataset(torch.utils.data.Dataset):
+class PackedDataset(Dataset):
     """
     The class PackedDataset takes in a dataset and aggregates samples of different
     lengths together based on the packed_length.
 
     Args:
         dataset: The original dataset to pack.
         max_length_per_sample: The maximum length of each original sample. Default is 2048.
@@ -46,164 +46,27 @@
         self.dataset = dataset
         self.max_length_per_sample = max_length_per_sample
         self.lengths = getattr(self.dataset, "lengths")
         self.packed_length = packed_length
         # Force a seed to be fixed to prevent problems caused by the seed not being restored when restarting
 
         self.seed = DEFAULT_SEED
-        self.sample_indices, self.len_samples_shuffled, self.acm_len_samples = self.accu_sample_len(seed=self.seed)
-        self.num_tokens = sum(self.lengths)
-
-    def get_dataset_name(self):
-        return self.dataset.get_dataset_name()
-
-    def accu_sample_len(self, seed=None):
-        """accumulative length of samples"""
-        if seed is not None:
-            rng = np.random.RandomState(seed)
-        else:
-            rng = np.random.RandomState(self.seed - 1)
-
-        sample_indices = np.arange(len(self.lengths))
-        rng.shuffle(sample_indices)
-        len_samples_shuffled = list(map(self.lengths.__getitem__, sample_indices))
-        acm_len_samples = list(it.accumulate(len_samples_shuffled, operator.add))
-        return sample_indices, len_samples_shuffled, acm_len_samples
-
-    def __len__(self):
-        # Line 405 of document_to_sequence.py in metaseq is directly spliced,
-        # without additional consideration of sos or eos
-        n_packs = self.num_tokens // self.packed_length
-        return n_packs
-
-    def cal_map(self, carriage_idx: int = 0):
-        assert carriage_idx >= 0
-        length_train = (carriage_idx + 1) * self.packed_length
-        post_pos = np.searchsorted(self.acm_len_samples, length_train, side="left")
-        return post_pos
-
-    def mapping(self, pack_idx: int = 0):
-        # pack_idx is zero-based
-        pre_pos, pre_token_id = 0, 0
-        if pack_idx > 0:
-            pre_pos = self.cal_map(pack_idx - 1)
-            pre_token_id = self.len_samples_shuffled[pre_pos] - (
-                self.acm_len_samples[pre_pos] - (pack_idx) * self.packed_length
-            )
-            if pre_token_id == self.len_samples_shuffled[pre_pos]:
-                pre_pos += 1
-                pre_token_id = 0
-
-        pos = self.cal_map(pack_idx)
-        token_id = self.len_samples_shuffled[pos] - (self.acm_len_samples[pos] - (pack_idx + 1) * self.packed_length)
-        return pre_pos, pre_token_id, pos, token_id
-
-    def build_pack(self, pre_pos: int, pre_token_id: int, pos: int, token_id: int):
-        pack, cu_seqlens, indexes, labels, type_ids = [], [0], [], [], []
-
-        while pre_pos < pos:
-            sample_idx = self.sample_indices[pre_pos]
-            sample = self.dataset[sample_idx]
-            chunk = sample["tokens"][pre_token_id:]
-            pack.extend(chunk)
-            _labels = deepcopy(chunk)
-            _labels = list(_labels[1:]) + [-100]
-            assert len(_labels) == len(chunk), (_labels, chunk)
-            labels.extend(_labels)
-            type_ids.extend([sample.get("type_id", 0)] * len(chunk))
-            num_new_samples, tokens_left = divmod(len(chunk), self.max_length_per_sample)
-            for _ in range(num_new_samples):
-                cu_seqlens.append(cu_seqlens[-1] + self.max_length_per_sample)
-                indexes.extend(list(range(self.max_length_per_sample)))
-            if tokens_left > 0:
-                cu_seqlens.append(cu_seqlens[-1] + tokens_left)
-                indexes.extend(list(range(tokens_left)))
-            pre_pos = pre_pos + 1
-            pre_token_id = 0
-
-        sample_idx = self.sample_indices[pos]
-        sample = self.dataset[sample_idx]
-        chunk = sample["tokens"][pre_token_id:token_id]  # fragement of a sample
-        pack.extend(chunk)
-        _labels = deepcopy(chunk)
-        if token_id == len(sample["tokens"]):
-            _labels = list(_labels[1:]) + [-100]
-        else:
-            if token_id > len(sample["tokens"]):
-                print(f"token_id {token_id}, len of sample {len(sample['tokens'])}")
-            _labels = list(_labels[1:]) + [sample["tokens"][token_id]]
-        assert len(_labels) == len(chunk), (_labels, chunk)
-        labels.extend(_labels)
-        type_ids.extend([sample.get("type_id", 0)] * len(chunk))
-        num_new_samples, tokens_left = divmod(len(chunk), self.max_length_per_sample)
-        for _ in range(num_new_samples):
-            cu_seqlens.append(cu_seqlens[-1] + self.max_length_per_sample)
-            indexes.extend(list(range(self.max_length_per_sample)))
-        if tokens_left > 0:
-            cu_seqlens.append(cu_seqlens[-1] + tokens_left)
-            indexes.extend(list(range(tokens_left)))
-
-        out = {"tokens": pack, "cu_seqlens": cu_seqlens, "indexes": indexes, "labels": labels, "type_ids": type_ids}
-        return out
-
-    def cal_pos_unpack(self, index):
-        if index == 0:
-            pre_pos = 0
-        else:
-            pre_pos = index * gpc.config.data["micro_bsz"]
-
-        pos = (index + 1) * gpc.config.data["micro_bsz"]
-        return pre_pos, pos
-
-    def build_unpack(self, index):
-
-        pre_pos, pos = self.cal_pos_unpack(index)
-
-        pack, cu_seqlens, indexes, labels, type_ids = [], [0], [], [], []
-
-        while pre_pos < pos and pre_pos < len(self.dataset):
-            sample_idx = self.sample_indices[pre_pos]
-            sample = self.dataset[sample_idx]
-            length = min(len(sample["tokens"]), self.max_length_per_sample)
-            chunk = sample["tokens"][0:length]
-            pack.extend(chunk)
-            _labels = deepcopy(chunk)
-            _labels = list(_labels[1:]) + [-100]
-            assert len(_labels) == len(chunk), (_labels, chunk)
-            labels.extend(_labels)
-            type_ids.extend([sample.get("type_id", 0)] * len(chunk))
-            cu_seqlens.append(cu_seqlens[-1] + len(chunk))
-            indexes.extend(list(range(length)))
-            pre_pos = pre_pos + 1
-
-        if cu_seqlens[-1] != self.packed_length:
-            pack = pack + [0] * (self.packed_length - cu_seqlens[-1])
-            labels = labels + [-100] * (self.packed_length - cu_seqlens[-1])
-            type_ids = type_ids + [0] * (self.packed_length - cu_seqlens[-1])
-            indexes.extend(list(range(self.packed_length - cu_seqlens[-1])))
-            cu_seqlens.append(self.packed_length)
-
-        assert len(pack) == self.packed_length
-
-        out = {"tokens": pack, "cu_seqlens": cu_seqlens, "indexes": indexes, "labels": labels, "type_ids": type_ids}
-        return out
 
     def __getitem__(self, item: int) -> Dict:
         """Given the index, it returns a dict as
         {
          'tokens': List[int],
          'cu_seqlens': List[int],
          'indexes': List[int], # denotes positional vector as 'tokens'
          'labels': List[int], # corresponds to 'tokens' and shifted yet, -100 means skipping prediction
         }
         """
 
-        if gpc.config.model.use_flash_attn:
-            pos_before, token_id_before, pos_after, token_id_after = self.mapping(item)
-            return self.build_pack(pos_before, token_id_before, pos_after, token_id_after)
+        if gpc.config is None or gpc.config.model is None or gpc.config.data.use_packed_dataset:
+            return self.build_pack(item)
 
         return self.build_unpack(item)
 
 
 class PackedDatasetWithoutCuSeqlen(torch.utils.data.Dataset):
     """
     A dataset wrapper that aggregates samples with different lengths based on packed_length.
@@ -336,22 +199,208 @@
             "cu_seqlens": [i * self.max_length_per_sample for i in range(self.bsz + 1)],
             "indexes": list(range(self.max_length_per_sample)) * self.bsz,
             "labels": pack_labels,
             "type_ids": type_ids,
         }
 
 
+class PackedDatasetWithCut(PackedDataset):
+    """
+    The class PackedDataset takes in a dataset and aggregates samples of different
+    lengths together based on the packed_length using cut mode.
+
+
+    max_length_per_sample = 3
+    packed_length = 5
+    [1, 2]
+    [3, 4]
+    [5, 6, 7]
+    [8, 9, 10, 11, 12, 13]
+
+    --->
+    [1, 2, 3, 4, 5]
+    [6, 7, 8, 9, 10]
+    [11, 12, 13, 0, 0]
+
+    Args:
+        dataset: The original dataset to pack.
+        max_length_per_sample: The maximum length of each original sample. Default is 2048.
+        packed_length: The length of each packed sample. Default is 4096.
+    """
+
+    def __init__(
+        self,
+        dataset,
+        max_length_per_sample: int = 2048,
+        packed_length: int = 4096,
+    ):
+        super().__init__(dataset, max_length_per_sample, packed_length)
+        self.sample_indices, self.len_samples_shuffled, self.acm_len_samples = self.accu_sample_len(seed=self.seed)
+        self.num_tokens = sum(self.lengths)
+
+    def get_dataset_name(self):
+        return self.dataset.get_dataset_name()
+
+    def accu_sample_len(self, seed=None):
+        """accumulative length of samples"""
+        if seed is not None:
+            rng = np.random.RandomState(seed)
+        else:
+            rng = np.random.RandomState(self.seed - 1)
+
+        sample_indices = np.arange(len(self.lengths))
+        rng.shuffle(sample_indices)
+        len_samples_shuffled = list(map(self.lengths.__getitem__, sample_indices))
+        acm_len_samples = list(it.accumulate(len_samples_shuffled, operator.add))
+        return sample_indices, len_samples_shuffled, acm_len_samples
+
+    def __len__(self):
+        # Line 405 of document_to_sequence.py in metaseq is directly spliced,
+        # without additional consideration of sos or eos
+        n_packs = self.num_tokens // self.packed_length
+        return n_packs
+
+    def cal_map(self, carriage_idx: int = 0):
+        assert carriage_idx >= 0
+        length_train = (carriage_idx + 1) * self.packed_length
+        post_pos = np.searchsorted(self.acm_len_samples, length_train, side="left")
+        return post_pos
+
+    def mapping(self, pack_idx: int = 0):
+        # pack_idx is zero-based
+        pre_pos, pre_token_id = 0, 0
+        if pack_idx > 0:
+            pre_pos = self.cal_map(pack_idx - 1)
+            pre_token_id = self.len_samples_shuffled[pre_pos] - (
+                self.acm_len_samples[pre_pos] - (pack_idx) * self.packed_length
+            )
+            if pre_token_id == self.len_samples_shuffled[pre_pos]:
+                pre_pos += 1
+                pre_token_id = 0
+
+        pos = self.cal_map(pack_idx)
+        token_id = self.len_samples_shuffled[pos] - (self.acm_len_samples[pos] - (pack_idx + 1) * self.packed_length)
+        return pre_pos, pre_token_id, pos, token_id
+
+    def build_pack(self, item):
+        pre_pos, pre_token_id, pos, token_id = self.mapping(item)
+        pack, cu_seqlens, indexes, labels, type_ids = [], [0], [], [], []
+
+        while pre_pos < pos:
+            sample_idx = self.sample_indices[pre_pos]
+            sample = self.dataset[sample_idx]
+            chunk = sample["tokens"][pre_token_id:]
+            pack.extend(chunk)
+            _labels = deepcopy(chunk)
+            _labels = list(_labels[1:]) + [-100]
+            assert len(_labels) == len(chunk), (_labels, chunk)
+            labels.extend(_labels)
+            type_ids.extend([sample.get("type_id", 0)] * len(chunk))
+            num_new_samples, tokens_left = divmod(len(chunk), self.max_length_per_sample)
+            for _ in range(num_new_samples):
+                cu_seqlens.append(cu_seqlens[-1] + self.max_length_per_sample)
+                indexes.extend(list(range(self.max_length_per_sample)))
+            if tokens_left > 0:
+                cu_seqlens.append(cu_seqlens[-1] + tokens_left)
+                indexes.extend(list(range(tokens_left)))
+            pre_pos = pre_pos + 1
+            pre_token_id = 0
+
+        sample_idx = self.sample_indices[pos]
+        sample = self.dataset[sample_idx]
+        chunk = sample["tokens"][pre_token_id:token_id]  # fragement of a sample
+        pack.extend(chunk)
+        _labels = deepcopy(chunk)
+        if token_id == len(sample["tokens"]):
+            _labels = list(_labels[1:]) + [-100]
+        else:
+            if token_id > len(sample["tokens"]):
+                print(f"token_id {token_id}, len of sample {len(sample['tokens'])}")
+            _labels = list(_labels[1:]) + [sample["tokens"][token_id]]
+        assert len(_labels) == len(chunk), (_labels, chunk)
+        labels.extend(_labels)
+        type_ids.extend([sample.get("type_id", 0)] * len(chunk))
+        num_new_samples, tokens_left = divmod(len(chunk), self.max_length_per_sample)
+        for _ in range(num_new_samples):
+            cu_seqlens.append(cu_seqlens[-1] + self.max_length_per_sample)
+            indexes.extend(list(range(self.max_length_per_sample)))
+        if tokens_left > 0:
+            cu_seqlens.append(cu_seqlens[-1] + tokens_left)
+            indexes.extend(list(range(tokens_left)))
+
+        out = {"tokens": pack, "cu_seqlens": cu_seqlens, "indexes": indexes, "labels": labels, "type_ids": type_ids}
+        return out
+
+    def cal_pos_unpack(self, index):
+        if index == 0:
+            pre_pos = 0
+        else:
+            pre_pos = index * gpc.config.data["micro_bsz"]
+
+        pos = (index + 1) * gpc.config.data["micro_bsz"]
+        return pre_pos, pos
+
+    def build_unpack(self, index):
+        """
+        max_length_per_sample = 3
+        packed_length = 6
+        micro_bsz = 2
+        [1, 2]
+        [3, 4]
+        [5, 6, 7]
+        [8, 9, 10, 11, 12, 13]
+        [14, 15, 16, 17]
+
+        --->
+        [1, 2, 3, 4, 0, 0]
+        [5, 6, 7, 8, 9, 10]
+        [14, 15, 16, 0, 0, 0]
+
+        """
+
+        pre_pos, pos = self.cal_pos_unpack(index)
+
+        pack, cu_seqlens, indexes, labels, type_ids = [], [0], [], [], []
+
+        while pre_pos < pos and pre_pos < len(self.dataset):
+            sample_idx = self.sample_indices[pre_pos]
+            sample = self.dataset[sample_idx]
+            length = min(len(sample["tokens"]), self.max_length_per_sample)
+            chunk = sample["tokens"][0:length]
+            pack.extend(chunk)
+            _labels = deepcopy(chunk)
+            _labels = list(_labels[1:]) + [-100]
+            assert len(_labels) == len(chunk), (_labels, chunk)
+            labels.extend(_labels)
+            type_ids.extend([sample.get("type_id", 0)] * len(chunk))
+            cu_seqlens.append(cu_seqlens[-1] + len(chunk))
+            indexes.extend(list(range(length)))
+            pre_pos = pre_pos + 1
+
+        if cu_seqlens[-1] != self.packed_length:
+            pack = pack + [0] * (self.packed_length - cu_seqlens[-1])
+            labels = labels + [0] * (self.packed_length - cu_seqlens[-1])
+            type_ids = type_ids + [0] * (self.packed_length - cu_seqlens[-1])
+            indexes.extend(list(range(self.packed_length - cu_seqlens[-1])))
+            cu_seqlens.append(self.packed_length)
+
+        assert len(pack) == self.packed_length
+
+        out = {"tokens": pack, "cu_seqlens": cu_seqlens, "indexes": indexes, "labels": labels, "type_ids": type_ids}
+        return out
+
+
 def get_packed_dataset_without_short_length(
     folder,
     max_length_per_sample=2048,
     packed_length=4096,
     show_progress=False,
     min_length=50,
     min_length_dict=None,
-    pack_into_one_sample=False,
+    pack_sample_into_one=False,
 ):
     """
     Given a folder, combine all the .bin files into a single large dataset.
     And filter out short samples with length less than 'min_length'.
 
     Each .bin file is treated as a separate dataset.
 
@@ -408,18 +457,18 @@
                 if hasattr(ds, "old_length"):
                     delete_samples += ds.old_length - len(ds)
                 if len(ds) == 0:
                     if gpc.is_rank_for_log():
                         logger.info(f"None of the data in `{fp}` is longer than {min_length}")
                     continue
 
-                if pack_into_one_sample:
+                if pack_sample_into_one:
                     ds = PackedDatasetWithoutCuSeqlen(ds, max_length_per_sample, packed_length)
                 else:
-                    ds = PackedDataset(ds, max_length_per_sample, packed_length)
+                    ds = PackedDatasetWithCut(ds, max_length_per_sample, packed_length)
 
                 num_token_in_folder += len(ds) * packed_length
                 datasets.append(ds)
 
     dataset = ConcatDataset(datasets=datasets)
     if gpc.is_rank_for_log():
         logger.info(
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/data/single_dataset.py` & `InternEvo-0.4.0.dev20240403/internlm/data/tokenized/single_dataset.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.3.3.dev20240315/internlm/data/utils.py` & `InternEvo-0.4.0.dev20240403/internlm/data/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,36 +20,38 @@
     for key, idx in dataset_type_ids_map.items():
         if re.search(rf"/[z_]*{key}/", path):
             match_idxes.append(idx)
     assert len(match_idxes) == 1, f"{path}, match_idxes should be 1, but got {match_idxes} from {dataset_type_ids_map}"
     return match_idxes[0]
 
 
-def unpack_data(input_ids, cu_seqlens, is_type_ids: bool = False):
+def unpack_data(input_ids, cu_seqlens, is_type_ids: bool = False, padding_v: int = 0):
     """
     input_ids: if input_ids is not type_ids, the shape is (1, packed_length)
                else the shape is (micro_num, packed_length)
     is_type_ids: whether the input_ids is type_ids
 
     Return:
     output: if input_ids is not type ids, the shape is (micro_bsz, max_length)
             else the shape is (micro_num, micro_bsz, max_length)
     """
     bsz = input_ids.shape[0]
 
-    num_sequence = gpc.config.data["micro_bsz"]
+    num_seq = gpc.config.data["micro_bsz"]
+    seq_len_ = gpc.config.data.seq_len
+    dtype_ = input_ids.dtype
 
-    outputs = torch.zeros(bsz, num_sequence, gpc.config.data.seq_len, device=input_ids.device, dtype=input_ids.dtype)
+    outputs = torch.empty(bsz, num_seq, seq_len_, device=input_ids.device, dtype=dtype_).fill_(padding_v)
 
     for i in range(bsz):
-        output = torch.zeros(num_sequence, gpc.config.data.seq_len, device=input_ids.device, dtype=input_ids.dtype)
+        output = torch.empty(num_seq, seq_len_, device=input_ids.device, dtype=dtype_).fill_(padding_v)
         cu_seqlens_slice = cu_seqlens[i]
-        for j in range(num_sequence):
-            seq_length = cu_seqlens_slice[j + 1] - cu_seqlens_slice[j]
-            output[j, 0:seq_length] = input_ids[0, cu_seqlens_slice[j] : cu_seqlens_slice[j + 1]]
+        for j in range(num_seq):
+            length = cu_seqlens_slice[j + 1] - cu_seqlens_slice[j]
+            output[j, 0:length] = input_ids[i, cu_seqlens_slice[j] : cu_seqlens_slice[j + 1]]
         outputs[i] = output
 
     # if the input_ids is not type_ids, we need squeeze the first dimension if it is 1.
     if bsz == 1 and not is_type_ids:
         outputs = outputs.squeeze(0)
 
     return outputs
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/initialize/initialize_tensor.py` & `InternEvo-0.4.0.dev20240403/internlm/initialize/initialize_tensor.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.3.3.dev20240315/internlm/initialize/initialize_trainer.py` & `InternEvo-0.4.0.dev20240403/internlm/initialize/initialize_trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,16 +19,16 @@
     InterleavedPipelineScheduler,
     NonPipelineScheduler,
     PipelineScheduler,
 )
 from internlm.core.scheduler.pipeline_scheduler import get_tensor_shape
 from internlm.core.trainer import Trainer
 from internlm.data.utils import unpack_data
-from internlm.solver.beta2_scheduler import Beta2Scheduler
 from internlm.solver.optimizer.hybrid_zero_optim import BaseOptimizer
+from internlm.solver.schedulers.beta2_scheduler import Beta2Scheduler
 from internlm.utils.common import SchedulerHook, get_current_device
 
 
 def initialize_trainer(
     model: nn.Module,
     optimizer: Optimizer,
     criterion: Optional[_Loss] = None,
@@ -75,15 +75,15 @@
     for config in gradient_handler_cfg:
         if isinstance(config, dict) and config.get("type") == "PipelineSharedModuleGradientHandler":
             handler = PipelineSharedModuleGradientHandler(model=model, optimizer=optimizer)
             gradient_handlers.append(handler)
 
     # initialize scheduler for trainer
     scheduler = None
-    if gpc.config.model.use_flash_attn:
+    if gpc.config.data.use_packed_dataset:
         data_fn = None
     else:
         data_fn = unpack_data
     if gpc.is_using_parallel_mode(ParallelMode.PIPELINE):
         gpc.config.NUM_MICRO_BATCHES = gpc.config.data.micro_num
         tensor_shape = get_tensor_shape()
         use_interleaved = (
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/initialize/launch.py` & `InternEvo-0.4.0.dev20240403/internlm/initialize/launch.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,19 +5,22 @@
 import gc
 import os
 from pathlib import Path
 from typing import Dict, Union
 
 import torch
 
+from internlm.accelerator import AcceleratorType, get_accelerator
 from internlm.core.context import Config
 from internlm.core.context import global_context as gpc
 from internlm.core.context.process_group_initializer import ParallelMode
-from internlm.moe.megablock.utils import check_megablock_installed, check_stk_installed
-from internlm.monitor import initialize_light_monitor
+from internlm.model.moe.megablock.utils import (
+    check_megablock_installed,
+    check_stk_installed,
+)
 from internlm.utils.common import get_master_node
 from internlm.utils.gputest import warmup_process_group
 from internlm.utils.logger import get_logger
 from internlm.utils.timeout import llm_timeout
 
 # check package
 try:
@@ -26,14 +29,15 @@
     from pynvml.smi import nvidia_smi
 except (AttributeError, ImportError):
     get_numa = False
 else:
     get_numa = True
 
 logger = get_logger(__file__)
+internlm_accelerator = get_accelerator()
 
 
 def get_default_parser():
     """Reads user command line and uses an argument parser to parse the input arguments.
     Input arguments include configuration, host, port, world size, local rank, backend for torch.distributed.
 
     Returns:
@@ -115,14 +119,17 @@
     assert data.micro_bsz is not None, "'micro_bsz' must be given a value"
 
     if "packed_length" in data and gpc.is_rank_for_log():
         logger.warning("packed_length would be ignored and will be setted as seq_len * micro_bsz.")
 
     data._add_item("packed_length", data.seq_len * data.micro_bsz)
 
+    if "type" not in data:
+        data._add_item("type", "tokenized")
+
     if "micro_num" not in data:
         data._add_item("micro_num", 1)
 
     if "gradient_accumulation" not in data:
         data._add_item("gradient_accumulation", data.micro_num)
         if gpc.is_rank_for_log():
             logger.info(f"gradient_accumulation size will be setted to {data.micro_num}.")
@@ -154,14 +161,20 @@
         data._add_item("empty_cache_and_diag_interval", 50)
 
     if "diag_outlier_ratio" not in data:
         data._add_item("diag_outlier_ratio", 1.1)
 
     data.diag_outlier_ratio = max(1, data.diag_outlier_ratio)
 
+    if "use_packed_dataset" not in data:
+        data._add_item("use_packed_dataset", True)
+
+    if "fixed_random_dataset_seqlen" not in data:
+        data._add_item("fixed_random_dataset_seqlen", True)
+
     if gpc.is_rank_for_log():
         logger.info("+" * 15 + " Data Info " + "+" * 15)  # pylint: disable=W1201
         logger.info(f"seq_len: {data.seq_len}")
         logger.info(f"micro_num: {data.micro_num}")
         logger.info(f"micro_bsz: {data.micro_bsz}")
         logger.info(f"packed_length: {data.packed_length}")
         logger.info(f"pack_sample_into_one: {data.pack_sample_into_one}")
@@ -304,35 +317,51 @@
         logger.info("+" * 15 + " beta2_scheduler Info " + "+" * 15)  # pylint: disable=W1201
         logger.info(f"beta2_scheduler: {gpc.config.beta2_scheduler}")
 
     # process the model config
     if "use_flash_attn" not in gpc.config.model:
         gpc.config.model._add_item("use_flash_attn", True)
 
+    gpc.config["use_cuda_flash_attn"] = False
+    if gpc.config.model.use_flash_attn and (
+        internlm_accelerator.get_accelerator_backend() in [AcceleratorType.GPU, AcceleratorType.DIPU]
+    ):
+        gpc.config["use_cuda_flash_attn"] = True
+
+    old_parallel_output = gpc.config.model.get("parallel_output", None)
+    # Try to change user setting
+    if not gpc.config.use_cuda_flash_attn:
+        gpc.config.model.update({"parallel_output": False})
+        if old_parallel_output is True and gpc.is_rank_for_log():
+            logger.warning(
+                "'parallel_output' is converted from 'True' to 'False'."
+                "Because 'parallel_output' only support by FlashCrossEntropyLoss."
+                "Please make sure you are using flash attention in cuda device."
+            )
+
     if "MoE" in gpc.config.get("model_type", "INTERNLM"):
         if "num_experts" not in model:
             model._add_item("num_experts", 1)
         if "moe_use_residual" not in model:
             model._add_item("moe_use_residual", False)
         if "moe_type" not in model:
             model._add_item("moe_type", "GShard")
         # check dependency
         if gpc.config.model.moe_type == "MegaBlock":
             check_megablock_installed()
         if gpc.config.model.moe_type == "MegaBlock-D":
             check_megablock_installed()
             check_stk_installed()
 
+    if "mlp_layer_fusion" not in model:
+        model._add_item("mlp_layer_fusion", False)
+
     # process the parallel config
     if "sequence_parallel" not in gpc.config.parallel:
         gpc.config.parallel._add_item("sequence_parallel", False)
-    else:
-        assert not (
-            gpc.config.parallel.sequence_parallel is True and gpc.config.model.use_flash_attn is False
-        ), "sequence parallel does not support use_flash_attn=False"
 
     # set default value for tensor parallel
     if isinstance(gpc.config.parallel["tensor"], int):
         gpc.config.parallel["tensor"] = dict(size=gpc.config.parallel["tensor"], mode="mtp")
     if gpc.config.parallel["tensor"].get("mode", None) is None:
         gpc.config.parallel["tensor"]["mode"] = "mtp"
     if gpc.config.parallel["tensor"]["mode"] == "isp":
@@ -343,14 +372,29 @@
     assert gpc.config.parallel["tensor"].get("mode", None) in [
         "mtp",
         "msp",
         "fsp",
         "isp",
     ], "invalid tensor parallel mode, only ['mtp', 'msp', 'fsp', 'isp'] is supported"
 
+    # for NPU accelerator supports: 1）FA-True + Packed-True 2) FA-False + Packed-False
+    # for DIPU accelerator supports: 1）FA-True + Packed-False 2) FA-False + Packed-False
+    # for GPU accelerator supports: 1）FA-True + Packed-True 2) FA-False + Packed-False
+    if gpc.config.parallel["tensor"]["mode"] == "isp" and internlm_accelerator.get_accelerator_backend() in [
+        AcceleratorType.NPU,
+        AcceleratorType.DIPU,
+    ]:
+        assert (
+            gpc.config.data.use_packed_dataset is False
+        ), "only unpacked data is supported when tensor parallel mode is isp and accelerator type is NPU or DIPU"
+    else:
+        assert (
+            gpc.config.model.use_flash_attn == gpc.config.data.use_packed_dataset
+        ), "use_packed_dataset should be set same value as use_flash_attn"
+
     # adapt to old version's sequence parallel config
     if gpc.config.parallel["tensor"].get("mode", None) in ["msp", "fsp", "isp"]:
         gpc.config.parallel.sequence_parallel = True
 
     # set default value for weight parallel
     if gpc.config.parallel["weight"].get("overlap", None) is None:
         gpc.config.parallel["weight"]["overlap"] = False
@@ -463,21 +507,18 @@
     # init default process group
     gpc.init_global_dist(rank, world_size, backend, host, port)
 
     # init process groups for different parallel modes from config
     gpc.init_parallel_groups()
 
     # set cuda device
-    if torch.cuda.is_available():
+    if internlm_accelerator.is_available():
         # if local rank is not given, calculate automatically
         gpc.set_device(local_rank)
 
-    # set the number of processes running on the same node
-    gpc.detect_num_processes_on_current_node()
-
     gpc.set_seed(seed)
 
     warmup_process_group()
 
     if gpc.is_rank_for_log():
         logger.info(
             f"Distributed environment is initialized, "
@@ -567,55 +608,45 @@
 @llm_timeout(func_name="initialize_distributed_env")
 def initialize_distributed_env(
     config: str,
     launcher: str = "slurm",
     master_port: int = 8888,
     seed: int = 1024,
     args_check=True,
+    backend: str = "nccl",
 ):
     """
     Initialize distributed environment for distributed training.
 
     Args:
         config (str): Config file path.
         launcher (str): Launcher for launching distributed environment, can be slurm or torch. "slurm" by default.
         master_port (str): The master port for distributed training. 8888 by default.
         seed (int, optional): Specified random seed for every process. 1024 by default.
     """
+    backend = internlm_accelerator._communication_backend_name
 
     # close automatic garbage collection
     gc.disable()
 
-    torch.cuda.empty_cache()
-
     if launcher == "torch":
-        launch_from_torch(config=config, seed=seed)
+        launch_from_torch(config=config, seed=seed, backend=backend)
     elif launcher == "slurm":
         launch_from_slurm(
             config=config,
             host=get_master_node(),
             port=master_port,
             seed=seed,
         )
     else:
         assert launcher in ["slurm", "torch"], "launcher only support slurm or torch"
 
     if args_check:
         args_sanity_check()
 
-    # init light monitor client
-    if gpc.config.get("monitor") and gpc.config.monitor.get("alert"):
-        alert_config = gpc.config.monitor.alert
-        if alert_config.enable_feishu_alert:
-            light_monitor_address = alert_config.light_monitor_address
-            if light_monitor_address:
-                initialize_light_monitor(light_monitor_address)
-            elif gpc.is_rank_for_log():
-                logger.warning("monitor address is none, monitor could not be used!")
-
 
 def get_config_value(config, key, defalut):
     try:
         value = config[key]
     except KeyError:
         value = defalut
     return value
@@ -643,15 +674,15 @@
         if total_GPU_per_node % numa_node_num != 0:
             return
         # return while the number of processes is smaller than one node GPUs num
         if world_size < total_GPU_per_node:
             return
 
         if local_rank is None:
-            devices_per_node = torch.cuda.device_count()
+            devices_per_node = internlm_accelerator.device_count()
             local_rank = global_rank % devices_per_node
 
         # compute numa id for each locak rank
         per_numa = total_GPU_per_node // numa_node_num
         numa_id = local_rank // per_numa
 
         # bind numa node
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/initialize/legacy/launch.py` & `InternEvo-0.4.0.dev20240403/internlm/initialize/legacy/launch.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,20 +21,20 @@
     load_model_only_folder = get_config_value(ckpt_config, "load_model_only_folder", None)
 
     if load_model_only_folder is not None:
         assert (
             load_ckpt_folder is None
         ), "Detect 'load_ckpt_folder' and 'load_model_only_folder' set at the same time, \
 # and 'load_given_ckpt' is True, so internlm will load from 'load_ckpt_folder'"
-        return dict(path=load_model_only_folder, content=("model",), ckpt_type="internlm")
+        return dict(path=load_model_only_folder, content=("model",), ckpt_type="internevo")
     else:
         load_optimizer = get_config_value(ckpt_config, "load_optimizer", True)
 
         if isinstance(load_ckpt_folder, str):
             if load_optimizer:
-                return dict(path=load_ckpt_folder, content=("model", "sampler", "optimizer"), ckpt_type="internlm")
+                return dict(path=load_ckpt_folder, content=("model", "sampler", "optimizer"), ckpt_type="internevo")
             else:
-                return dict(path=load_ckpt_folder, content=("model", "sampler"), ckpt_type="internlm")
+                return dict(path=load_ckpt_folder, content=("model", "sampler"), ckpt_type="internevo")
         elif load_ckpt_folder is None:
             return None
         else:
             assert f"Unsupport data type:'{type(load_ckpt_folder)}' for config.ckpt arg: 'load_ckpt_folder'"
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/model/__init__.py` & `InternEvo-0.4.0.dev20240403/internlm/model/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 #!/usr/bin/env python
 # -*- encoding: utf-8 -*-
 
-from .embedding import Embedding1D, RotaryEmbedding
-from .linear import FeedForward, RewardModelLinear, ScaleColumnParallelLinear
 from .metrics import AccPerplex
 from .modeling_internlm import build_model_with_cfg
 from .modeling_internlm2 import build_model_with_cfg as build_model_with_cfg2
 from .modeling_llama import build_model_with_cfg as build_model_with_llama_cfg
 from .modeling_moe import build_model_with_moe_cfg
-from .moe import MoE
-from .multi_head_attention import MHA, DistributedAttention
+from .modules.embedding import Embedding1D, RotaryEmbedding
+from .modules.mlp import FeedForward
+from .modules.multi_head_attention import MHA, DistributedAttention
+from .moe.moe import MoE
+from .ops.linear import RewardModelLinear, ScaleColumnParallelLinear
 from .utils import gather_forward_split_backward
 
 __all__ = [
     "Embedding1D",
     "FeedForward",
     "MoE",
     "RotaryEmbedding",
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/model/embedding.py` & `InternEvo-0.4.0.dev20240403/internlm/model/modules/embedding.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 #!/usr/bin/env python
 # -*- encoding: utf-8 -*-
 
-from typing import Optional, Tuple, Union
+from typing import Tuple
 
 import torch
 import torch.nn.functional as F
-from einops import rearrange, repeat
+from einops import rearrange
 from torch import Tensor, nn
 
+from internlm.accelerator import AcceleratorType, get_accelerator
 from internlm.core.context import ParallelMode
 from internlm.core.context import global_context as gpc
 
-from .utils import gather_forward_split_backward, split_forward_gather_backward
+from ..utils import gather_forward_split_backward, split_forward_gather_backward
+
+try:
+    import rotary_emb
+except (ModuleNotFoundError, ImportError):
+    pass
+
+internlm_accelerator = get_accelerator()
 
 
 class Embedding1D(nn.Module):
     """
     1D Embedding.
 
     Args:
@@ -56,357 +64,210 @@
 
         if gpc.config.parallel.sequence_parallel:
             output = split_forward_gather_backward(output, ParallelMode.TENSOR, dim=1)
 
         return output
 
 
-def rotate_half(x, interleaved=False):
-    if not interleaved:
-        x1, x2 = x.chunk(2, dim=-1)
-        return torch.cat((-x2, x1), dim=-1)
-    else:
-        x1, x2 = x[..., ::2], x[..., 1::2]
-        return rearrange(torch.stack((-x2, x1), dim=-1), "... d two -> ... (d two)", two=2)
-
-
-def apply_rotary_emb_torch(x, cos, sin, interleaved=False):
-    """
-    x: (batch_size, seqlen, nheads, headdim) or (total, nheads, headdim)
-    cos, sin: (seqlen, rotary_dim / 2) or (batch_size, seqlen, rotary_dim / 2)
-    """
-    ro_dim = cos.shape[-1] * 2
-    assert ro_dim <= x.shape[-1]
-    cos = repeat(cos, "... d -> ... 1 (2 d)" if not interleaved else "... d -> ... 1 (d 2)")
-    sin = repeat(sin, "... d -> ... 1 (2 d)" if not interleaved else "... d -> ... 1 (d 2)")
-    return torch.cat(
-        [x[..., :ro_dim] * cos + rotate_half(x[..., :ro_dim], interleaved) * sin, x[..., ro_dim:]],
-        dim=-1,
-    )
-
-
-def apply_rotary_torch(
-    x,
-    cos,
-    sin,
-    interleaved=False,
-    seqlen_offsets: Union[int, torch.Tensor] = 0,
-    cu_seqlens: Optional[torch.Tensor] = None,
+def _torch_apply_rotary_func(
+    x1: torch.Tensor,
+    x2: torch.Tensor,
+    cos: torch.Tensor,
+    sin: torch.Tensor,
+    out1: torch.Tensor,
+    out2: torch.Tensor,
+    conj: bool = False,
 ):
-    x_pt = x.detach().clone().requires_grad_()
-
-    is_varlen = cu_seqlens is not None
-    if not is_varlen:
-        seqlen = x.shape[1]
-        if isinstance(seqlen_offsets, torch.Tensor):
-            batch_size = seqlen_offsets.shape[0]
-            arange = rearrange(torch.arange(seqlen, device=cos.device), "s -> 1 s")
-            idx = rearrange(seqlen_offsets, "b -> b 1") + arange
-            cos_pt = rearrange(cos[idx.flatten()], "(b s) d -> b s d", b=batch_size)
-            sin_pt = rearrange(sin[idx.flatten()], "(b s) d -> b s d", b=batch_size)
-        else:
-            cos_pt = cos[seqlen_offsets : seqlen_offsets + seqlen]
-            sin_pt = sin[seqlen_offsets : seqlen_offsets + seqlen]
-    else:
-        cos_pt = cos
-        sin_pt = sin
-
-    output = apply_rotary_emb_torch(x_pt, cos_pt, sin_pt, interleaved)
-    return output
-
-
-def apply_rotary_packed_torch(x1, x2, cos, sin, conj):
     assert x1.device == x2.device == cos.device == sin.device, "All inputs must be on the same device"
     assert x1.dtype == x2.dtype == cos.dtype == sin.dtype, "All inputs must have the same dtype"
     assert x1.size() == x2.size(), "Input x1 and x2 must have the same sizes"
     assert cos.size() == sin.size(), "Input cos and sin must have the same sizes"
 
+    x1, x2, cos, sin = x1.float(), x2.float(), cos.float(), sin.float()
+
     if conj:
-        out1 = x1 * cos + x2 * sin
-        out2 = -x1 * sin + x2 * cos
+        out1.copy_(x1 * cos + x2 * sin)
+        out2.copy_(-x1 * sin + x2 * cos)
     else:
-        out1 = x1 * cos - x2 * sin
-        out2 = x1 * sin + x2 * cos
+        out1.copy_(x1 * cos - x2 * sin)
+        out2.copy_(x1 * sin + x2 * cos)
 
     return out1, out2
 
 
-class ApplyRotaryEmb(torch.autograd.Function):
-    """
-    ApplyRotaryEmb
-    """
-
-    @staticmethod
-    def forward(
-        ctx,
-        x,
-        cos,
-        sin,
-        interleaved=False,
-        inplace=False,
-        seqlen_offsets: Union[int, torch.Tensor] = 0,
-        cu_seqlens: Optional[torch.Tensor] = None,
-        max_seqlen: Optional[int] = None,
-    ):
-        if gpc.config.model.use_flash_attn:
-            from flash_attn.ops.triton.rotary import apply_rotary
-
-            out = apply_rotary(
-                x,
-                cos,
-                sin,
-                seqlen_offsets=seqlen_offsets,
-                cu_seqlens=cu_seqlens,
-                max_seqlen=max_seqlen,
-                interleaved=interleaved,
-                inplace=inplace,
-            )
-        else:
-            out = apply_rotary_torch(x, cos, sin, interleaved, seqlen_offsets, cu_seqlens)
-        if isinstance(seqlen_offsets, int):
-            ctx.save_for_backward(cos, sin, cu_seqlens)  # Can't save int with save_for_backward
-            ctx.seqlen_offsets = seqlen_offsets
-        else:
-            ctx.save_for_backward(cos, sin, cu_seqlens, seqlen_offsets)
-            ctx.seqlen_offsets = None
-        ctx.interleaved = interleaved
-        ctx.inplace = inplace
-        ctx.cu_seqlens = cu_seqlens
-        ctx.max_seqlen = max_seqlen
-        return out if not inplace else x
-
-    @staticmethod
-    def backward(ctx, do):
-        seqlen_offsets = ctx.seqlen_offsets
-        if seqlen_offsets is None:
-            cos, sin, cu_seqlens, seqlen_offsets = ctx.saved_tensors
-        else:
-            cos, sin, cu_seqlens = ctx.saved_tensors
-        # TD [2023-09-02]: For some reason Triton (2.0.0.post1) errors with
-        # "[CUDA]: invalid device context", and cloning makes it work. Idk why. Triton 2.1.0 works.
-        if not ctx.interleaved and not ctx.inplace:
-            do = do.clone()
-        if gpc.config.model.use_flash_attn:
-            from flash_attn.ops.triton.rotary import apply_rotary
-
-            dx = apply_rotary(
-                do,
-                cos,
-                sin,
-                seqlen_offsets=seqlen_offsets,
-                cu_seqlens=cu_seqlens,
-                max_seqlen=ctx.max_seqlen,
-                interleaved=ctx.interleaved,
-                inplace=ctx.inplace,
-                conjugate=True,
-            )
-        else:
-            dx = apply_rotary_torch(do, cos, sin, ctx.interleaved, seqlen_offsets, cu_seqlens)
-        return dx, None, None, None, None, None, None, None
-
-
-apply_rotary_emb = ApplyRotaryEmb.apply
+def get_rotary_func():
+    if gpc.config.use_cuda_flash_attn:
+        return rotary_emb.apply_rotary
+    else:
+        return _torch_apply_rotary_func
 
 
-class ApplyRotaryEmbQKV_(torch.autograd.Function):
+class ApplyRotaryEmb(torch.autograd.Function):
     """
-    ApplyRotaryEmbQKV_
+    ApplyRotaryEmb
     """
 
     @staticmethod
-    def forward(
-        ctx,
-        qkv,
-        cos,
-        sin,
-        cos_k=None,
-        sin_k=None,
-        interleaved=False,
-        seqlen_offsets: Union[int, torch.Tensor] = 0,
-    ):
+    def forward(ctx, x, cos, sin, interleaved=False):
         """
-            qkv: (batch_size, seqlen, 3, nheads, headdim)
+            x: (batch_size, seqlen, nheads, headdim)
             cos, sin: (seqlen, rotary_dim / 2)
-            cos_k, sin_k: (seqlen, rotary_dim / 2), optional
+            interleaved: if True, rotate pairs of even and odd dimensions (GPT-J style) instead
+                of 1st half and 2nd half (GPT-NeoX style).
         rotary_dim must be <= headdim
-        Apply rotary embedding *inplace* to the first rotary_dim of q and k.
+        Apply rotary embedding to the first rotary_dim of x.
         """
-        three = qkv.shape[2]
-        assert three == 3
-
-        if gpc.config.model.use_flash_attn:
-            from flash_attn.ops.triton.rotary import apply_rotary
+        _, seqlen, _, headdim = x.shape
+        rotary_seqlen, rotary_dim = cos.shape
+        rotary_dim *= 2
+        assert rotary_dim <= headdim
+        assert seqlen <= rotary_seqlen
+        assert sin.shape == (rotary_seqlen, rotary_dim // 2)
+        x_ro = x[..., :rotary_dim]
+        x1, x2 = x_ro.chunk(2, dim=-1) if not interleaved else (x_ro[..., ::2], x_ro[..., 1::2])
+        out = torch.empty_like(x)
+        out_ro = out[..., :rotary_dim]
+        o1, o2 = out_ro.chunk(2, dim=-1) if not interleaved else (out_ro[..., ::2], out_ro[..., 1::2])
+
+        get_rotary_func()(
+            x1,
+            x2,
+            rearrange(cos[:seqlen], "s d -> s 1 d"),
+            rearrange(sin[:seqlen], "s d -> s 1 d"),
+            o1,
+            o2,
+            False,
+        )
 
-        if cos_k is None and sin_k is None and qkv.is_contiguous():
-            # Call 1 kernel instead of 2 kernels
-            # We need qkv to be contiguous so that when we reshape to combine (3, nheads)
-            # dimensions, we get the same tensor
-            qk = rearrange(qkv[:, :, :2], "b s t h d -> b s (t h) d")
-            if gpc.config.model.use_flash_attn:
-                apply_rotary(qk, cos, sin, seqlen_offsets, interleaved=interleaved, inplace=True)
-            else:
-                qk = apply_rotary_torch(qk, cos, sin, interleaved, seqlen_offsets)
-        else:
-            cos_k = cos if cos_k is None else cos_k
-            sin_k = sin if sin_k is None else sin_k
-            q, k = qkv[:, :, 0], qkv[:, :, 1]
-            if gpc.config.model.use_flash_attn:
-                apply_rotary(q, cos, sin, seqlen_offsets, interleaved=interleaved, inplace=True)
-                apply_rotary(k, cos_k, sin_k, seqlen_offsets, interleaved=interleaved, inplace=True)
-            else:
-                q = apply_rotary_torch(q, cos, sin, interleaved, seqlen_offsets)
-                k = apply_rotary_torch(k, cos_k, sin_k, interleaved, seqlen_offsets)
-            ctx.save_for_backward(cos, sin, cos_k, sin_k)
-        if isinstance(seqlen_offsets, int):
-            ctx.save_for_backward(cos, sin, cos_k, sin_k)
-            ctx.seqlen_offsets = seqlen_offsets
-        else:
-            ctx.save_for_backward(cos, sin, cos_k, sin_k, seqlen_offsets)
-            ctx.seqlen_offsets = None
+        if rotary_dim < headdim:
+            out[..., rotary_dim:].copy_(x[..., rotary_dim:])
+        ctx.save_for_backward(cos, sin)
         ctx.interleaved = interleaved
-        return qkv
+        return out
 
     @staticmethod
-    def backward(ctx, dqkv):
-        seqlen_offsets = ctx.seqlen_offsets
-        if seqlen_offsets is None:
-            cos, sin, cos_k, sin_k, seqlen_offsets = ctx.saved_tensors
-        else:
-            cos, sin, cos_k, sin_k = ctx.saved_tensors
+    def backward(ctx, do):
+        cos, sin = ctx.saved_tensors
+        _, seqlen, _, headdim = do.shape
+        rotary_dim = cos.shape[-1]
+        rotary_dim *= 2
+        do_ro = do[..., :rotary_dim]
+        do1, do2 = do_ro.chunk(2, dim=-1) if not ctx.interleaved else (do_ro[..., ::2], do_ro[..., 1::2])
+        dx = torch.empty_like(do)
+        dx_ro = dx[..., :rotary_dim]
+        dx1, dx2 = dx_ro.chunk(2, dim=-1) if not ctx.interleaved else (dx_ro[..., ::2], dx_ro[..., 1::2])
+
+        get_rotary_func()(
+            do1,
+            do2,
+            rearrange(cos[:seqlen], "s d -> s 1 d"),
+            rearrange(sin[:seqlen], "s d -> s 1 d"),
+            dx1,
+            dx2,
+            True,
+        )
+        if rotary_dim < headdim:
+            dx[..., rotary_dim:].copy_(do[..., rotary_dim:])
+        return dx, None, None, None, None
 
-        if gpc.config.model.use_flash_attn:
-            from flash_attn.ops.triton.rotary import apply_rotary
-
-        if cos_k is None and sin_k is None and dqkv.is_contiguous():
-            # Call 1 kernel instead of 2 kernels
-            # We need dqkv to be contiguous so that when we reshape to combine (3, nheads)
-            # dimensions, we get the same tensor
-            dqk = rearrange(dqkv[:, :, :2], "b s t h d -> b s (t h) d")
-            if gpc.config.model.use_flash_attn:
-                apply_rotary(
-                    dqk,
-                    cos,
-                    sin,
-                    seqlen_offsets=seqlen_offsets,
-                    interleaved=ctx.interleaved,
-                    inplace=True,
-                    conjugate=True,
-                )
-            else:
-                dqk = apply_rotary_torch(dqk, cos, sin, ctx.interleaved, seqlen_offsets)
-        else:
-            cos_k = cos if cos_k is None else cos_k
-            sin_k = sin if sin_k is None else sin_k
-            dq, dk = dqkv[:, :, 0], dqkv[:, :, 1]
-            if gpc.config.model.use_flash_attn:
-                apply_rotary(
-                    dq,
-                    cos,
-                    sin,
-                    seqlen_offsets,
-                    interleaved=ctx.interleaved,
-                    inplace=True,
-                    conjugate=True,
-                )
-                apply_rotary(
-                    dk,
-                    cos_k,
-                    sin_k,
-                    seqlen_offsets,
-                    interleaved=ctx.interleaved,
-                    inplace=True,
-                    conjugate=True,
-                )
-            else:
-                dq = apply_rotary_torch(dq, cos, sin, ctx.interleaved, seqlen_offsets)
-                dk = apply_rotary_torch(dk, cos_k, sin_k, ctx.interleaved, seqlen_offsets)
-        return dqkv, None, None, None, None, None, None
 
+if AcceleratorType.DIPU == internlm_accelerator.get_accelerator_backend():
+    from deeplink_ext.internlm_ops.rotary.deeplink import DeeplinkApplyRotaryEmb
 
-apply_rotary_emb_qkv_ = ApplyRotaryEmbQKV_.apply
+    apply_rotary_emb = DeeplinkApplyRotaryEmb.apply
+else:
+    apply_rotary_emb = ApplyRotaryEmb.apply
 
 
-class ApplyRotaryEmbPackedQKV_(torch.autograd.Function):
+class ApplyRotaryEmbQKV_(torch.autograd.Function):
     """
-    ApplyRotaryEmbPackedQKV_
-
-    Currently, packed qkv calculation is not supported in flash attention,
-    a CUDA memory access error may occur in rotary_kernel function. Therefore,
-    we need this class here, still using the implemention of flash attention v1.0.
+    ApplyRotaryEmbQKV_
     """
 
     @staticmethod
-    def forward(ctx, qkv, cos, sin, cos_k=None, sin_k=None):
+    def forward(ctx, qkv, cos, sin, cos_k=None, sin_k=None, interleaved=False):
         """
-            qkv: (total, 3, nheads, headdim)
+            qkv: (total, 3, nheads, headdim) / (batch_size, seqlen, 3, nheads, headdim)
             cos, sin: (seqlen, rotary_dim / 2)
             cos_k, sin_k: (seqlen, rotary_dim / 2), optional
+            interleaved: if True, rotate pairs of even and odd dimensions (GPT-J style) instead of
+                1st half and 2nd half (GPT-NeoX style).
         rotary_dim must be <= headdim
         Apply rotary embedding *inplace* to the first rotary_dim of q and k.
         """
-        _, three, _, headdim = qkv.shape
+        # len(qkv.shape) == 4 means the format of qkv is (total, 3, nheads, headdim) which is packed,
+        # otherwise the format of qkv is (batch_size, seqlen, 3, nheads, headdim) which is unpacked.
+        # We handle both packed qkv and unpacked qkv scenario in this class.
+        three = qkv.shape[1] if len(qkv.shape) == 4 else qkv.shape[2]
         assert three == 3
+        seqlen = None if len(qkv.shape) == 4 else qkv.shape[1]
         rotary_seqlen, rotary_dim = cos.shape
+        if len(qkv.shape) != 4:
+            assert seqlen <= rotary_seqlen
+        headdim = qkv.shape[-1]
         rotary_dim *= 2
         assert rotary_dim <= headdim
         cos_k = cos if cos_k is None else cos_k
         sin_k = sin if sin_k is None else sin_k
         assert sin.shape == cos_k.shape == sin_k.shape == (rotary_seqlen, rotary_dim // 2)
-        q1, q2 = qkv[:, 0, :, :rotary_dim].chunk(2, dim=-1)
-        if gpc.config.model.use_flash_attn:
-            import rotary_emb
+        q_ro = qkv[:, 0, :, :rotary_dim] if len(qkv.shape) == 4 else qkv[:, :, 0, :, :rotary_dim]
+        q1, q2 = q_ro.chunk(2, dim=-1) if not interleaved else (q_ro[..., ::2], q_ro[..., 1::2])
+        re_cos = rearrange(cos, "s d -> s 1 d") if len(qkv.shape) == 4 else rearrange(cos[:seqlen], "s d -> s 1 d")
+        re_sin = rearrange(sin, "s d -> s 1 d") if len(qkv.shape) == 4 else rearrange(sin[:seqlen], "s d -> s 1 d")
+
+        get_rotary_func()(q1, q2, re_cos, re_sin, q1, q2, False)
+
+        k_ro = qkv[:, 1, :, :rotary_dim] if len(qkv.shape) == 4 else qkv[:, :, 1, :, :rotary_dim]
+        k1, k2 = k_ro.chunk(2, dim=-1) if not interleaved else (k_ro[..., ::2], k_ro[..., 1::2])
+        re_cos_k = (
+            rearrange(cos_k, "s d -> s 1 d") if len(qkv.shape) == 4 else rearrange(cos_k[:seqlen], "s d -> s 1 d")
+        )
+        re_sin_k = (
+            rearrange(sin_k, "s d -> s 1 d") if len(qkv.shape) == 4 else rearrange(sin_k[:seqlen], "s d -> s 1 d")
+        )
+
+        get_rotary_func()(k1, k2, re_cos_k, re_sin_k, k1, k2, False)
 
-            rotary_emb.apply_rotary(
-                q1, q2, rearrange(cos, "s d -> s 1 d"), rearrange(sin, "s d -> s 1 d"), q1, q2, False
-            )
-        else:
-            q1, q2 = apply_rotary_packed_torch(
-                q1, q2, rearrange(cos, "s d -> s 1 d"), rearrange(sin, "s d -> s 1 d"), False
-            )
-        k1, k2 = qkv[:, 1, :, :rotary_dim].chunk(2, dim=-1)
-        if gpc.config.model.use_flash_attn:
-            rotary_emb.apply_rotary(
-                k1, k2, rearrange(cos_k, "s d -> s 1 d"), rearrange(sin_k, "s d -> s 1 d"), k1, k2, False
-            )
-        else:
-            k1, k2 = apply_rotary_packed_torch(
-                k1, k2, rearrange(cos_k, "s d -> s 1 d"), rearrange(sin_k, "s d -> s 1 d"), False
-            )
         ctx.save_for_backward(cos, sin, cos_k, sin_k)
+        ctx.interleaved = interleaved
         return qkv
 
     @staticmethod
     def backward(ctx, dqkv):
         cos, sin, cos_k, sin_k = ctx.saved_tensors
+        seqlen = None if len(dqkv.shape) == 4 else dqkv.shape[1]
         rotary_dim = cos.shape[-1]
         rotary_dim *= 2
-        dq1, dq2 = dqkv[:, 0, :, :rotary_dim].chunk(2, dim=-1)
-        if gpc.config.model.use_flash_attn:
-            import rotary_emb
+        dq_ro = dqkv[:, 0, :, :rotary_dim] if len(dqkv.shape) == 4 else dqkv[:, :, 0, :, :rotary_dim]
+        dq1, dq2 = dq_ro.chunk(2, dim=-1) if not ctx.interleaved else (dq_ro[..., ::2], dq_ro[..., 1::2])
+        re_cos = rearrange(cos, "s d -> s 1 d") if len(dqkv.shape) == 4 else rearrange(cos[:seqlen], "s d -> s 1 d")
+        re_sin = rearrange(sin, "s d -> s 1 d") if len(dqkv.shape) == 4 else rearrange(sin[:seqlen], "s d -> s 1 d")
+
+        get_rotary_func()(dq1, dq2, re_cos, re_sin, dq1, dq2, True)
+
+        dk_ro = dqkv[:, 1, :, :rotary_dim] if len(dqkv.shape) == 4 else dqkv[:, :, 1, :, :rotary_dim]
+        dk1, dk2 = dk_ro.chunk(2, dim=-1) if not ctx.interleaved else (dk_ro[..., ::2], dk_ro[..., 1::2])
+        re_cos_k = (
+            rearrange(cos_k, "s d -> s 1 d") if len(dqkv.shape) == 4 else rearrange(cos_k[:seqlen], "s d -> s 1 d")
+        )
+        re_sin_k = (
+            rearrange(sin_k, "s d -> s 1 d") if len(dqkv.shape) == 4 else rearrange(sin_k[:seqlen], "s d -> s 1 d")
+        )
+
+        get_rotary_func()(dk1, dk2, re_cos_k, re_sin_k, dk1, dk2, True)
+
+        return dqkv, None, None, None, None, None
 
-            rotary_emb.apply_rotary(
-                dq1, dq2, rearrange(cos, "s d -> s 1 d"), rearrange(sin, "s d -> s 1 d"), dq1, dq2, True
-            )
-        else:
-            dq1, dq2 = apply_rotary_packed_torch(
-                dq1, dq2, rearrange(cos, "s d -> s 1 d"), rearrange(sin, "s d -> s 1 d"), True
-            )
-        dk1, dk2 = dqkv[:, 1, :, :rotary_dim].chunk(2, dim=-1)
-        if gpc.config.model.use_flash_attn:
-            rotary_emb.apply_rotary(
-                dk1, dk2, rearrange(cos_k, "s d -> s 1 d"), rearrange(sin_k, "s d -> s 1 d"), dk1, dk2, True
-            )
-        else:
-            dk1, dk2 = apply_rotary_packed_torch(
-                dk1, dk2, rearrange(cos_k, "s d -> s 1 d"), rearrange(sin_k, "s d -> s 1 d"), True
-            )
-        return dqkv, None, None, None, None
 
+if AcceleratorType.DIPU == internlm_accelerator.get_accelerator_backend():
+    from deeplink_ext.internlm_ops.rotary.deeplink import DeeplinkApplyRotaryEmbQKV_
 
-apply_rotary_emb_packed_qkv_ = ApplyRotaryEmbPackedQKV_.apply
+    apply_rotary_emb_qkv_ = DeeplinkApplyRotaryEmbQKV_.apply
+else:
+    apply_rotary_emb_qkv_ = ApplyRotaryEmbQKV_.apply
 
 
 class RotaryEmbedding(torch.nn.Module):
     """
     The rotary position embeddings from RoFormer_ (Su et. al).
     A crucial insight from the method is that the query and keys are
     transformed by rotation matrices which depend on the relative positions.
@@ -478,17 +339,17 @@
             return self._eval_forward(qkv, seqlen_offset=kwargs.get("inference_params", None).sequence_len_offset)
         else:
             return self._eval_forward(qkv)
 
     def _forward(self, qkv: torch.Tensor, indexes=0) -> Tuple[torch.Tensor, torch.Tensor]:
         self._update_cos_sin_cache(qkv, indexes)
         if self.scale is None:
-            return apply_rotary_emb_packed_qkv_(qkv, self._cos_cached[indexes], self._sin_cached[indexes])
+            return apply_rotary_emb_qkv_(qkv, self._cos_cached[indexes], self._sin_cached[indexes])
         else:
-            return apply_rotary_emb_packed_qkv_(
+            return apply_rotary_emb_qkv_(
                 qkv,
                 self._cos_cached[indexes],
                 self._sin_cached[indexes],
                 self._cos_k_cached[indexes],
                 self._sin_k_cached[indexes],
             )
 
@@ -505,23 +366,18 @@
                 qkv,
                 self._cos_cached[seqlen_offset:],
                 self._sin_cached[seqlen_offset:],
                 self._cos_k_cached[seqlen_offset:],
                 self._sin_k_cached[seqlen_offset:],
             )
 
-    def _single_forward(
-        self, x, indexes=0, cu_seqlens: Optional[torch.Tensor] = None, max_seqlen: Optional[int] = None
-    ):
+    def _single_forward(self, x, indexes=0):
         assert self.scale is None
         self._update_cos_sin_cache(x, indexes)
-        x = x[None, ...]
-        ret = apply_rotary_emb(
-            x, self._cos_cached[indexes], self._sin_cached[indexes], False, False, 0, cu_seqlens, max_seqlen
-        ).squeeze(0)
+        ret = apply_rotary_emb(x, self._cos_cached[indexes], self._sin_cached[indexes])
         return ret
 
     def _single_eval_forward(self, x, seqlen_offset=0):
         assert self.scale is None
         self._update_cos_sin_cache(x, seqlen_offset + x.shape[1])
         return apply_rotary_emb(x, self._cos_cached[seqlen_offset:], self._sin_cached[seqlen_offset:])
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/model/linear.py` & `InternEvo-0.4.0.dev20240403/internlm/model/ops/linear.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 #!/usr/bin/env python
 # -*- encoding: utf-8 -*-
 
-from typing import Callable, Optional
+from typing import Optional
 
 import torch
 from torch import nn
 from torch.distributed import ProcessGroup
 
 from internlm.core.context import ParallelMode
 from internlm.core.context import global_context as gpc
 from internlm.model.utils import (
-    Silu,
     all_reduce,
     fused_dense_func,
     isp_fused_dense_func,
     megatron_fused_dense_func,
     reduce_scatter,
 )
 from internlm.utils.logger import get_logger
@@ -59,15 +58,15 @@
 
 
 class ScaleColumnParallelLinear(BaseScaleColumnParallelLinear):
     """
     ScaleColumnParallelLinear in flash implementation.
     """
 
-    def forward(self, input, gather_dim=0, tp_mode: str = "mtp"):  # pylint: disable=W0622
+    def forward(self, input, gather_dim=1, tp_mode: str = "mtp"):  # pylint: disable=W0622
         # If self.sequence_parallel is True, we're doing Tensor Parallel with sequence parallelism:
         # we do an all_gather of x before doing the matmul.
         # If not, then the input is already gathered.
         if self.weight_scale != 1:
             weight = self.weight * self.weight_scale + (1 - self.weight_scale) * self.weight.detach()
         else:
             weight = self.weight
@@ -79,15 +78,15 @@
             self.bias,
             process_group=self.process_group,
             sequence_parallel=gpc.config.parallel.sequence_parallel,
             gather_dim=gather_dim,
         )
 
 
-class InternLM2ScaleColumnParallelLinear(BaseScaleColumnParallelLinear):
+class ScaleColumnParallelLinearWithNormHead(BaseScaleColumnParallelLinear):
     """
     ScaleColumnParallelLinear for InternLM2.
 
     Args:
         in_features (int): size of each input sample
         out_features (int): size of each output sample
         process_group (Optional[torch.distributed.ProcessGroup]): The group of the current device for `parallel_mode`.
@@ -118,15 +117,15 @@
 
         self.norm_head = norm_head
         if self.norm_head:
             logger.info("Notice that norm head is enabled to normalize head weight.")
         self.first_eval_flag = True
         self.tmp_weight = None
 
-    def forward(self, input, gather_dim=0, tp_mode: str = "mtp"):  # pylint: disable=W0622
+    def forward(self, input, gather_dim=1, tp_mode: str = "mtp"):  # pylint: disable=W0622
         if self.weight_scale != 1:
             weight = self.weight * self.weight_scale + (1 - self.weight_scale) * self.weight.detach()
         else:
             weight = self.weight
         if self.norm_head:
             if self.training:
                 if not self.first_eval_flag:
@@ -240,15 +239,15 @@
         mod = multiple % world_size
         # The first @mod ranks get @div + 1 copies, the rest get @div copies
         local_multiple = div + int(torch.distributed.get_rank(process_group) < mod)
         super().__init__(in_features, local_multiple * multiple_of, bias=bias, device=device, dtype=dtype)
         self.process_group = process_group
         self.sequence_parallel = sequence_parallel
 
-    def forward(self, x, gather_dim=0):
+    def forward(self, x, gather_dim=1):
         # If self.sequence_parallel is True, we're doing Tensor Parallel with sequence parallelism:
         # we do an all_gather of x before doing the matmul.
         # If not, then the input is already gathered.
         return fused_dense_func(
             x,
             self.weight,
             self.bias,
@@ -259,15 +258,15 @@
 
 
 class MegatronColumnParallelLinearTorch(ColumnParallelLinearTorch):
     """
     MegatronColumnParallelLinearTorch
     """
 
-    def forward(self, x, gather_dim=0):
+    def forward(self, x, gather_dim=1):
         # If self.sequence_parallel is True, we're doing Tensor Parallel with sequence parallelism:
         # we do an all_gather of x before doing the matmul.
         # If not, then the input is already gathered.
         return megatron_fused_dense_func(
             x,
             self.weight,
             self.bias,
@@ -322,188 +321,41 @@
             bias=bias and rank == 0,
             device=device,
             dtype=dtype,
         )
         self.process_group = process_group
         self.sequence_parallel = sequence_parallel
 
-    def forward(self, x):
+    def forward(self, x, reduce_dim=1):
         """
         We're doing Tensor Parallel with sequence parallelism: we do the matmul and then
         a reduce_scatter of the result.
         """
         out = fused_dense_func(x, self.weight, self.bias)
-        reduce_fn = reduce_scatter if self.sequence_parallel else all_reduce
-        return reduce_fn(out, self.process_group)
+        if self.sequence_parallel:
+            return reduce_scatter(out, self.process_group, reduce_dim)
+        else:
+            return all_reduce(out, self.process_group)
 
 
 class MegatronRowParallelLinearTorch(RowParallelLinearTorch):
     """
     MegatronRowParallelLinearTorch.
     """
 
-    def forward(self, x):
+    def forward(self, x, reduce_dim=1):
         """
         We're doing Tensor Parallel with sequence parallelism: we do the matmul and then
         a reduce_scatter of the result.
         """
         out = megatron_fused_dense_func(x, self.weight, self.bias)
-        reduce_fn = reduce_scatter if self.sequence_parallel else all_reduce
-        return reduce_fn(out, self.process_group)
-
-
-class BaseFeedForward(nn.Module):
-    """
-    Base FeedForward in flash implementation.
-
-    Args:
-        in_features (int): size of each input sample
-        hidden_features (int): size of hidden state of FFN
-        out_features (int): size of each output sample
-        process_group (Optional[torch.distributed.ProcessGroup]): The group of the current device for `parallel_mode`.
-        bias (bool): Whether the bias is needed for linears. True by default. But it is typically set to False
-                    in the config.
-        device (Optional[Union[str, torch.device]]): The device will be used.
-        dtype (Optional[torch.dtype]): The type of data.
-        multiple_of (int): For efficient training. Reset the size of hidden feature. 256 by default.
-        column_cls (Optional[Callable]): The column parallel class for w1 and w3. None by default.
-        row_cls (Optional[Callable]): The row parallel class for w2. None by default.
-    """
-
-    def __init__(
-        self,
-        in_features: int,
-        hidden_features: int,
-        out_features: int = None,
-        process_group: Optional[torch.distributed.ProcessGroup] = None,
-        bias: bool = True,
-        device: Optional[torch.device] = None,
-        dtype: Optional[torch.dtype] = None,
-        multiple_of: int = 256,
-        column_cls: Optional[Callable] = None,
-        row_cls: Optional[Callable] = None,
-    ):
-        super().__init__()
-        hidden_features = multiple_of * ((hidden_features + multiple_of - 1) // multiple_of)
-
-        self.w1 = column_cls(
-            in_features,
-            hidden_features,
-            process_group,
-            bias,
-            sequence_parallel=gpc.config.parallel.sequence_parallel,
-            device=device,
-            dtype=dtype,
-        )
-        self.w2 = row_cls(
-            hidden_features,
-            out_features,
-            process_group,
-            bias=bias,
-            sequence_parallel=gpc.config.parallel.sequence_parallel,
-            device=device,
-            dtype=dtype,
-        )
-        self.w3 = column_cls(
-            in_features,
-            hidden_features,
-            process_group,
-            bias,
-            sequence_parallel=gpc.config.parallel.sequence_parallel,
-            device=device,
-            dtype=dtype,
-        )
-
-    def forward(self, x):
-        w1_o = self.w1(x)
-        w3_o = self.w3(x)
-        out = self.w2(Silu(w1_o, w3_o))
-        return out
-
-
-class FeedForward(BaseFeedForward):
-    """
-    FeedForward in flash implementation.
-
-    Args:
-        in_features (int): size of each input sample
-        hidden_features (int): size of hidden state of FFN
-        out_features (int): size of each output sample
-        process_group (Optional[torch.distributed.ProcessGroup]): The group of the current device for `parallel_mode`.
-        bias (bool): Whether the bias is needed for linears. True by default. But it is typically set to False
-                    in the config.
-        device (Optional[Union[str, torch.device]]): The device will be used.
-        dtype (Optional[torch.dtype]): The type of data.
-        multiple_of (int): For efficient training. Reset the size of hidden feature. 256 by default.
-    """
-
-    def __init__(
-        self,
-        in_features: int,
-        hidden_features: int,
-        out_features: int = None,
-        process_group: Optional[torch.distributed.ProcessGroup] = None,
-        bias: bool = True,
-        device: Optional[torch.device] = None,
-        dtype: Optional[torch.dtype] = None,
-        multiple_of: int = 256,
-    ):
-        super().__init__(
-            in_features,
-            hidden_features,
-            out_features,
-            process_group,
-            bias,
-            device,
-            dtype,
-            multiple_of,
-            ColumnParallelLinearTorch,
-            RowParallelLinearTorch,
-        )
-
-
-class MegatronFeedForward(BaseFeedForward):
-    """
-    FeedForward in megatron implementation.
-
-    Args:
-        in_features (int): size of each input sample
-        hidden_features (int): size of hidden state of FFN
-        out_features (int): size of each output sample
-        process_group (Optional[torch.distributed.ProcessGroup]): The group of the current device for `parallel_mode`.
-        bias (bool): Whether the bias is needed for linears. True by default. But it is typically set to False
-                    in the config.
-        device (Optional[Union[str, torch.device]]): The device will be used.
-        dtype (Optional[torch.dtype]): The type of data.
-        multiple_of (int): For efficient training. Reset the size of hidden feature. 256 by default.
-    """
-
-    def __init__(
-        self,
-        in_features: int,
-        hidden_features: int,
-        out_features: int = None,
-        process_group: Optional[torch.distributed.ProcessGroup] = None,
-        bias: bool = True,
-        device: Optional[torch.device] = None,
-        dtype: Optional[torch.dtype] = None,
-        multiple_of: int = 256,
-    ):
-        super().__init__(
-            in_features,
-            hidden_features,
-            out_features,
-            process_group,
-            bias,
-            device,
-            dtype,
-            multiple_of,
-            MegatronColumnParallelLinearTorch,
-            MegatronRowParallelLinearTorch,
-        )
+        if self.sequence_parallel:
+            return reduce_scatter(out, self.process_group, reduce_dim)
+        else:
+            return all_reduce(out, self.process_group)
 
 
 class ISPLinear(ColumnParallelLinearTorch):
     """
     Linear class for isp tensor parallel mode.
     """
 
@@ -522,65 +374,14 @@
             self.weight,
             module=self,
             communicator=self.__communicator,
             bias=self.bias,
         )
 
 
-class ISPFeedForward(BaseFeedForward):
-    """
-    FeedForward in ISP.
-
-    Args:
-        in_features (int): size of each input sample
-        hidden_features (int): size of hidden state of FFN
-        out_features (int): size of each output sample
-        process_group (Optional[torch.distributed.ProcessGroup]): The group of the current device for `parallel_mode`.
-        bias (bool): Whether the bias is needed for linears. True by default. But it is typically set to False
-                    in the config.
-        device (Optional[Union[str, torch.device]]): The device will be used.
-        dtype (Optional[torch.dtype]): The type of data.
-        multiple_of (int): For efficient training. Reset the size of hidden feature. 256 by default.
-    """
-
-    def __init__(
-        self,
-        in_features: int,
-        hidden_features: int,
-        out_features: int = None,
-        process_group: Optional[torch.distributed.ProcessGroup] = None,
-        bias: bool = True,
-        device: Optional[torch.device] = None,
-        dtype: Optional[torch.dtype] = None,
-        multiple_of: int = 256,
-    ):
-        super().__init__(
-            in_features,
-            hidden_features,
-            out_features,
-            process_group,
-            bias,
-            device,
-            dtype,
-            multiple_of,
-            ISPLinear,
-            ISPLinear,
-        )
-
-
-def get_mlp_cls(tp_mode: str):
-    if tp_mode in ["mtp", "fsp"]:
-        mlp_cls = FeedForward
-    elif tp_mode == "msp":
-        mlp_cls = MegatronFeedForward
-    else:
-        mlp_cls = ISPFeedForward
-    return mlp_cls
-
-
 def get_linear_cls(tp_mode: str, parallel_mode: str):
     if parallel_mode == "column":
         if tp_mode in ["mtp", "fsp"]:
             cls = ColumnParallelLinearTorch
         elif tp_mode == "msp":
             cls = MegatronColumnParallelLinearTorch
         else:
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/model/loss.py` & `InternEvo-0.4.0.dev20240403/internlm/model/losses/ce_loss.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,26 +19,27 @@
             if label_smoothing != 0:
                 if gpc.is_rank_for_log():
                     print(f"use label_smoothing: {label_smoothing}")
         else:
             label_smoothing = 0
         self.label_smoothing = label_smoothing
 
-        if gpc.config.model.use_flash_attn and parallel_output:
+        if gpc.config.use_cuda_flash_attn and parallel_output:
             from flash_attn.losses.cross_entropy import (
                 CrossEntropyLoss as FlashCrossEntropyLoss,
             )
 
             self.loss_fn = FlashCrossEntropyLoss(
                 reduction="mean",
                 inplace_backward=True,
                 process_group=gpc.get_group(ParallelMode.TENSOR),
                 label_smoothing=label_smoothing,
             )  # The loss in this place is bound to the gather_output initialized by VocabParallelClassifier1D
         else:
+            assert parallel_output is False, "parallel_output should be False when using nn.CrossEntropyLoss func"
             # Here, the output will gather output is set in the model, so use ordinary loss
             self.loss_fn = nn.CrossEntropyLoss(reduction="mean", label_smoothing=label_smoothing)
 
     def forward(self, *args):
         if len(args) == 3:
             # residual is to match prenorm
             logits, _, labels = args
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/model/metrics.py` & `InternEvo-0.4.0.dev20240403/internlm/model/metrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,60 @@
 from typing import Callable, List, Optional
 
 import torch
 from torch import nn
-from torch_scatter import scatter
 
+from internlm.accelerator import AcceleratorType, get_accelerator
 from internlm.core.context import ParallelMode
 from internlm.core.context import global_context as gpc
-from internlm.utils.common import SchedulerHook
+from internlm.utils.common import SchedulerHook, get_current_device
 from internlm.utils.megatron_timers import megatron_timer as timer
 
+try:
+    from torch_scatter import scatter as cuda_scatter
+except (ModuleNotFoundError, ImportError):
+    pass
+
+internlm_accelerator = get_accelerator()
+
+
+def broadcast(src: torch.Tensor, other: torch.Tensor, dim: int):
+    if dim < 0:
+        dim = other.dim() + dim
+    if src.dim() == 1:
+        for _ in range(0, dim):
+            src = src.unsqueeze(0)
+    for _ in range(src.dim(), other.dim()):
+        src = src.unsqueeze(-1)
+    src = src.expand(other.size())
+    return src
+
+
+def vanilla_scatter(
+    src: torch.Tensor,
+    index: torch.Tensor,
+    dim: int = -1,
+    out: Optional[torch.Tensor] = None,
+    dim_size: Optional[int] = None,
+    reduce=None,  # pylint: disable=W0613
+) -> torch.Tensor:
+    index = broadcast(index, src, dim)
+    if out is None:
+        size = list(src.size())
+        if dim_size is not None:
+            size[dim] = dim_size
+        elif index.numel() == 0:
+            size[dim] = 0
+        else:
+            size[dim] = int(index.max()) + 1
+        out = torch.zeros(size, dtype=src.dtype, device=src.device)
+        return out.scatter_add_(dim, index, src)
+    else:
+        return out.scatter_add_(dim, index, src)
+
 
 class AccPerplex:
     """
     AccPerplex module for calculating model's accuracy and perplexity metrics.
 
     Args:
         device: The GPU device.
@@ -44,23 +86,31 @@
             self.dataset_types = dataset_types
             self.total_type_count = len(dataset_types)
             self.ds_right = torch.zeros(self.total_type_count, dtype=torch.long, device=device)
             self.ds_tokens = torch.zeros(self.total_type_count, dtype=torch.long, device=device)
 
         self.loss_with_type_id = LossWithTypeId(device, dp_pg, dataset_types)
 
+        if internlm_accelerator.get_accelerator_backend() in [AcceleratorType.GPU, AcceleratorType.DIPU]:
+            self.scatter_sum = cuda_scatter
+        else:
+            self.scatter_sum = vanilla_scatter
+
     def set_current_type_ids(self, type_ids: torch.Tensor):
         self.batch_shift = 0
-        self.type_ids = type_ids.cuda()
+        self.type_ids = type_ids.to(get_current_device())
+
+    def set_cu_seqlens(self, cu_seqlens: List):
+        self.cu_seqlens = cu_seqlens
 
     def __call__(self, logits, labels):
         return self.update(logits, labels, type_ids=self.type_ids)
 
     def update(self, logits, labels, type_ids=None):
-        if gpc.config.model.use_flash_attn:
+        if gpc.config.data.use_packed_dataset:
             micro_bsz = labels.size(0)
         else:
             micro_bsz = 1
         if type_ids is not None:
             type_ids = type_ids[self.batch_shift * micro_bsz : (self.batch_shift + 1) * micro_bsz].view(-1)
             self.batch_shift += 1
         self.loss_with_type_id.update(logits, labels, type_ids)
@@ -87,31 +137,33 @@
             logits_global = logits_max == torch.max(shift_logits, dim=-1)[0]
 
             corrects = torch.logical_and(
                 (shift_labels == (shift_logits.argmax(dim=-1) + pred_shift)), logits_global
             ).long()
             mask = shift_labels.ne(-100).long()
             if hasattr(self, "total_type_count"):
-                ds_acc = scatter(corrects, type_ids, dim=0, reduce="sum")
-                token_num_type = scatter(mask, type_ids, dim=0, reduce="sum")
+                ds_acc = self.scatter_sum(corrects, type_ids, dim=0, reduce="sum")
+                token_num_type = self.scatter_sum(mask, type_ids, dim=0, reduce="sum")
                 if len(ds_acc) < self.total_type_count:
                     ds_acc = torch.cat([ds_acc, ds_acc.new_zeros(self.total_type_count - len(ds_acc))])
                     token_num_type = torch.cat(
                         [token_num_type, token_num_type.new_zeros(self.total_type_count - len(token_num_type))]
                     )
                 self.ds_tokens += token_num_type
                 sync_tensor = ds_acc
                 torch.distributed.all_reduce(sync_tensor, op=torch.distributed.ReduceOp.SUM, group=self.tp_pg)
                 self.ds_right += sync_tensor.view(-1)
 
             acc = corrects.sum()
             torch.distributed.all_reduce(acc, op=torch.distributed.ReduceOp.SUM, group=self.tp_pg)
+            # The synchronization here is to prevent unpredictable HANG when the NPU is running.
+            if internlm_accelerator.get_accelerator_backend() in [AcceleratorType.NPU, AcceleratorType.DIPU]:
+                internlm_accelerator.current_stream().synchronize()
             self.right += acc  # Masked_fill is not needed here because -100 is not available anyway
             self.total += mask.sum()
-
             # Subtract the maximum value.
             shift_logits = shift_logits.sub(logits_max.unsqueeze(dim=-1))
 
             # Get the partition's vocab indecies
             partition_vocab_size = shift_logits.size()[-1]
             vocab_start_index = partition_vocab_size * self.tp_local_rank
             vocab_end_index = vocab_start_index + partition_vocab_size
@@ -206,44 +258,50 @@
 
         if dataset_types is not None:
             self.dataset_types = dataset_types
             self.total_type_count = len(dataset_types)
             self.ds_loss = torch.zeros(self.total_type_count, dtype=torch.float, device=device)
             self.ds_token_num = torch.zeros(self.total_type_count, dtype=torch.float, device=device)
 
-        if gpc.config.model.use_flash_attn:
+        if gpc.config.use_cuda_flash_attn and AcceleratorType.GPU == get_accelerator():
             from flash_attn.losses.cross_entropy import (
                 CrossEntropyLoss as FlashCrossEntropyLoss,
             )
 
             self.loss_fn = FlashCrossEntropyLoss(
                 reduction="none", inplace_backward=True, process_group=gpc.get_group(ParallelMode.TENSOR)
             )
         else:
             self.loss_fn = nn.CrossEntropyLoss(reduction="none")
 
+        if internlm_accelerator.get_accelerator_backend() in [AcceleratorType.GPU, AcceleratorType.DIPU]:
+            self.scatter_sum = cuda_scatter
+        else:
+            self.scatter_sum = vanilla_scatter
+
     def update(self, logits, labels, type_ids=None):
         with torch.no_grad():
             if isinstance(logits, (list, tuple)):
                 logits = logits[0]
             logits = logits.contiguous().view(-1, logits.size(-1))
             labels = labels.contiguous().view(-1)
+
             loss_list = self.loss_fn(logits, labels)
 
             cond = labels != -100
             real_loss_list = loss_list[cond]
             self.loss += real_loss_list.sum()
             self.token_num += real_loss_list.numel()
 
             if hasattr(self, "total_type_count"):
                 type_ids = type_ids.contiguous().view(-1).to(self.device)
                 real_type_ids = type_ids[cond]
 
-                loss_list_type = scatter(real_loss_list, real_type_ids, dim=0, reduce="sum")
-                token_num_type = scatter(torch.ones_like(real_loss_list), real_type_ids, dim=0, reduce="sum")
+                loss_list_type = self.scatter_sum(real_loss_list, real_type_ids, dim=0, reduce="sum")
+                token_num_type = self.scatter_sum(torch.ones_like(real_loss_list), real_type_ids, dim=0, reduce="sum")
 
                 if len(loss_list_type) < self.total_type_count:
                     loss_list_type = torch.cat(
                         [loss_list_type, loss_list_type.new_zeros(self.total_type_count - len(loss_list_type))]
                     )
                     token_num_type = torch.cat(
                         [token_num_type, token_num_type.new_zeros(self.total_type_count - len(token_num_type))]
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/model/modeling_internlm.py` & `InternEvo-0.4.0.dev20240403/internlm/model/modeling_internlm.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,29 +7,26 @@
 import torch
 from torch import nn
 
 from internlm.core.context import ParallelMode
 from internlm.core.context.parallel_context import global_context as gpc
 from internlm.core.naive_amp import set_output_attr_to_module
 from internlm.initialize.initialize_tensor import normal_, scaled_init_method_normal
-from internlm.model.embedding import Embedding1D
-from internlm.model.linear import (
-    RewardModelLinear,
-    ScaleColumnParallelLinear,
-    get_mlp_cls,
-)
-from internlm.model.multi_head_attention import MHA
+from internlm.model.modules.embedding import Embedding1D
+from internlm.model.modules.mlp import get_mlp_cls
+from internlm.model.modules.multi_head_attention import MHA
+from internlm.model.ops.linear import RewardModelLinear, ScaleColumnParallelLinear
 from internlm.model.utils import (
     gather_forward_split_backward,
     split_forward_gather_backward,
     try_import_RMSNorm,
 )
+from internlm.solver.activation_checkpoint import activation_checkpoint
 from internlm.solver.pipeline_utils import partition_uniform
-from internlm.utils.checkpoint import activation_checkpoint
-from internlm.utils.common import filter_kwargs
+from internlm.utils.common import filter_kwargs, get_current_device
 from internlm.utils.logger import get_logger
 from internlm.utils.registry import MODEL_INITIALIZER
 
 MODEL_TYPE = "INTERNLM"
 
 logger = get_logger(__file__)
 RMSNorm = try_import_RMSNorm()
@@ -74,14 +71,16 @@
         norm_type: str = "rmsnorm",
         dropout_selective_checkpoint: bool = True,
         use_scaled_init: bool = True,
         use_swiglu: bool = True,
         use_flash_attn: bool = True,
         tp_mode: str = "mtp",
         rope_base: int = 10000,
+        mlp_layer_fusion: bool = False,
+        multiple_of: int = 256,
     ):
         super().__init__()
         self.checkpoint = checkpoint
         # dropout selective checkpoint can only be enabled when checkpoint is disabled.
         self.dropout_selective_checkpoint = dropout_selective_checkpoint is True and checkpoint is False
         self.layer_idx = layer_idx
         self.use_flash_attn = use_flash_attn
@@ -124,16 +123,20 @@
                 hidden_size,
                 int(hidden_size * mlp_ratio),
                 out_features=hidden_size,
                 process_group=gpc.get_group(parallel_mode),
                 bias=False,
                 device=device,
                 dtype=dtype,
+                mlp_layer_fusion=mlp_layer_fusion,
+                sequence_parallel=gpc.config.parallel.sequence_parallel,
+                multiple_of=multiple_of,
             )
         else:
+            assert gpc.config.use_cuda_flash_attn is True
             from flash_attn.modules.mlp import ParallelFusedMLP
 
             self.mlp = ParallelFusedMLP(
                 hidden_size,
                 int(hidden_size * mlp_ratio),
                 out_features=hidden_size,
                 activation="gelu_approx",
@@ -169,15 +172,16 @@
             for name, param in self.mlp.named_parameters():
                 if param.ndim == 1 and "bias" in name:
                     param.data.zero_()
                 elif self.use_swiglu:
                     if self.use_scaled_init and "w2" in name:
                         scaled_init_method_normal(sigma=0.006, num_layers=self.layer_idx + 1)(param.data)
                     else:
-                        normal_(std=0.006 if "w1" in name or "w2" in name else 0.0015)(param.data)
+                        # candidate: w1, w3, fused_w1_w3
+                        normal_(std=0.006 if "w1" in name or "w3" in name else 0.0015)(param.data)
                 else:
                     if self.use_scaled_init and "fc1" not in name:
                         scaled_init_method_normal(sigma=0.006, num_layers=self.layer_idx + 1)(param.data)
                     else:
                         normal_(std=0.006 if "fc1" in name else 0.0015)(param.data)
 
     def forward(self, hidden_states, cu_seqlens=None, indexes=None, inference_params=None, max_seqlen=None):
@@ -295,28 +299,30 @@
         norm_type: str = "rmsnorm",
         is_reward: bool = False,
         dropout_selective_checkpoint: bool = True,
         use_scaled_init: bool = True,
         use_swiglu: bool = True,
         use_flash_attn: bool = True,
         rope_base: int = 10000,
+        mlp_layer_fusion: bool = False,
+        multiple_of: int = 256,
     ):
         super().__init__()
 
         checkpoint_layer_num = int(num_layers * checkpoint)
         self.tp_mode = "mtp"
         if isinstance(gpc.config.parallel["tensor"], dict):
             self.tp_mode = gpc.config.parallel["tensor"].get("mode", "mtp")
 
         if is_reward:
             head_cls = RewardModelLinear
         else:
             head_cls = ScaleColumnParallelLinear
         if first:
-            if embed_split_hidden or not use_flash_attn:
+            if embed_split_hidden or not gpc.config.use_cuda_flash_attn:
                 self.embedding = Embedding1D(num_embeddings=vocab_size, embedding_dim=hidden_size)
             else:
                 from flash_attn.modules.embedding import ParallelGPT2Embeddings
 
                 self.embedding = ParallelGPT2Embeddings(
                     embed_dim=hidden_size,
                     vocab_size=vocab_size,
@@ -350,14 +356,16 @@
                     norm_type=norm_type,
                     dropout_selective_checkpoint=dropout_selective_checkpoint,
                     use_scaled_init=use_scaled_init,
                     use_swiglu=use_swiglu,
                     use_flash_attn=use_flash_attn,
                     tp_mode=self.tp_mode,
                     rope_base=rope_base,
+                    mlp_layer_fusion=mlp_layer_fusion,
+                    multiple_of=multiple_of,
                 )
                 for lid in range(num_layers)
             ]
         )
         if last:
             if norm_type == "rmsnorm":
                 self.norm = RMSNorm(hidden_size, eps=layer_norm_epsilon)
@@ -382,22 +390,21 @@
         # attention_mask: compute attention on the places where the value is 1
         if hasattr(self, "embedding"):
             hidden_states = self.embedding(input_ids)
             if self.embed_grad_scale != 1:
                 hidden_states = (
                     self.embed_grad_scale * hidden_states + (1 - self.embed_grad_scale) * hidden_states.detach()
                 )
+
         if isinstance(cu_seqlens, list):
             assert len(cu_seqlens) == 1
             cu_seqlens = cu_seqlens[0].to(hidden_states.device)
 
         if cu_seqlens is not None:
             cu_seqlens = cu_seqlens.squeeze(0)
-            hidden_states = hidden_states.squeeze(0)  # If cu_seqlens is passed in，it indicated a packed state，
-            # the batch dimension with a size of 1 should be directly squeezed off.
 
         if indexes is not None:
             assert len(indexes) == 1
             # The indexes are used to indicate the actual position IDs of each token in the packed input.
             indexes = indexes[0]
             # if the sequence parallel mode is 'isp', the indexes should also be split in sequence dimension.
             if gpc.config.parallel.sequence_parallel and self.tp_mode == "isp":
@@ -413,35 +420,32 @@
                 inference_params=inference_params,
                 max_seqlen=max_seqlen,
             )
 
         if hasattr(self, "norm"):
             hidden_states = self.norm(hidden_states.float())
         if hasattr(self, "head"):
-            # Evaluation
-            if hidden_states.ndim == 3:
-                hidden_states = self.head(hidden_states, gather_dim=1, tp_mode=self.tp_mode)
-            else:  # Training
-                hidden_states = self.head(hidden_states, gather_dim=0, tp_mode=self.tp_mode)
+            hidden_states = self.head(hidden_states, gather_dim=1, tp_mode=self.tp_mode)
 
-        if not self.parallel_output:
+        if not self.parallel_output and gpc.is_pipeline_last_stage():
             hidden_states = gather_forward_split_backward(hidden_states, ParallelMode.TENSOR, dim=-1)
         return hidden_states
 
 
-def _build_generic_model_1d(num_layers, num_chunks, device=torch.device("cuda"), **kwargs):
+def _build_generic_model_1d(num_layers, num_chunks, **kwargs):
     """
     build generic model 1d
 
     Args:
         num_layers (int): The number of layer.
         num_chunks (int): The number of partitions in pipeline parallel.
-        device (Optional[Union[str, torch.device]]): The device will be used. torch.device("cuda") by default.
+        device (Optional[Union[str, torch.device]]): The device will be used. internlm_accelerator.device() by default.
 
     """
+    device = get_current_device()
     pipeline_size = gpc.get_world_size(ParallelMode.PIPELINE)
     pipeline_rank = gpc.get_local_rank(ParallelMode.PIPELINE)
 
     all_parts = partition_uniform(num_layers, pipeline_size, num_chunks)
     parts = all_parts[pipeline_rank]
     if gpc.is_rank_for_log():
         logger.info(f"The layer sharding is {all_parts}.")
@@ -490,14 +494,16 @@
     layer_norm_epsilon=1e-5,
     is_reward=False,
     dropout_selective_checkpoint=True,
     use_scaled_init: bool = True,
     use_swiglu: bool = True,
     use_flash_attn: bool = True,
     rope_base: int = 10000,
+    mlp_layer_fusion: bool = False,
+    multiple_of: int = 256,
 ):
     """
     Build model with config.
 
     Args:
         num_chunks (int): The number of partitions in pipeline parallel. 1 by default.
         checkpoint (bool): Whether to use checkpointing to save VRAM. False by default.
@@ -547,10 +553,12 @@
         layer_norm_epsilon=layer_norm_epsilon,
         is_reward=is_reward,
         dropout_selective_checkpoint=dropout_selective_checkpoint,
         use_scaled_init=use_scaled_init,
         use_swiglu=use_swiglu,
         use_flash_attn=use_flash_attn,
         rope_base=rope_base,
+        mlp_layer_fusion=mlp_layer_fusion,
+        multiple_of=multiple_of,
     )
 
     return _build_generic_model_1d(num_layers=num_layers, num_chunks=num_chunks, **cfg)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/model/modeling_internlm2.py` & `InternEvo-0.4.0.dev20240403/internlm/model/modeling_internlm2.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,54 +3,56 @@
 from typing import Optional
 
 import torch
 import torch.nn.functional as F
 from einops import rearrange
 from torch import nn
 
+from internlm.accelerator import AcceleratorType, get_accelerator
 from internlm.core.context import ParallelMode
 from internlm.core.context.parallel_context import global_context as gpc
 from internlm.initialize.initialize_tensor import (
     normal_,
     scaled_init_method_normal,
     scaled_init_method_uniform,
     uniform_,
 )
-from internlm.model.embedding import (
+from internlm.model.modules.embedding import (
     DynamicNTKScalingRotaryEmbedding,
     Embedding1D,
     RotaryEmbedding,
 )
-from internlm.model.linear import (
-    InternLM2ScaleColumnParallelLinear,
+from internlm.model.modules.mlp import get_mlp_cls
+from internlm.model.modules.multi_head_attention import (
+    _update_kv_cache,
+    get_gqa_attn_cls,
+)
+from internlm.model.ops.linear import (
     RewardModelLinear,
+    ScaleColumnParallelLinearWithNormHead,
     get_linear_cls,
-    get_mlp_cls,
-)
-from internlm.model.multi_head_attention import (
-    CrossAttention,
-    DistributedAttention,
-    SelfAttention,
-    _update_kv_cache,
 )
 from internlm.model.utils import (
     gather_forward_split_backward,
+    pack_output_after_attn,
     split_forward_gather_backward,
     try_import_RMSNorm,
+    unpack_qkv_before_attn,
 )
+from internlm.solver.activation_checkpoint import activation_checkpoint
 from internlm.solver.pipeline_utils import partition_uniform
-from internlm.utils.checkpoint import activation_checkpoint
-from internlm.utils.common import filter_kwargs
+from internlm.utils.common import filter_kwargs, get_current_device
 from internlm.utils.logger import get_logger
 from internlm.utils.registry import MODEL_INITIALIZER
 
 MODEL_TYPE = "INTERNLM2_PUBLIC"
 
 logger = get_logger(__file__)
 RMSNorm = try_import_RMSNorm()
+internlm_accelerator = get_accelerator()
 
 
 class MHA(nn.Module):
     """
     Multi-head self-attention and cross-attention.
 
     Args:
@@ -147,33 +149,21 @@
             embed_dim + 2 * self.kv_dim,
             process_group,
             bias=bias,
             sequence_parallel=sequence_parallel,
             **factory_kwargs,
         )
 
-        if use_flash_attn:
-            from flash_attn import flash_attn_varlen_kvpacked_func
-            from flash_attn.modules.mha import FlashCrossAttention, FlashSelfAttention
-
-        inner_attn_cls = FlashSelfAttention if use_flash_attn else SelfAttention
-        inner_cross_attn_cls = FlashCrossAttention if use_flash_attn else CrossAttention
-        self.inner_attn = inner_attn_cls(causal=causal, softmax_scale=softmax_scale, attention_dropout=dropout)
-        self.inner_cross_attn = inner_cross_attn_cls(
-            causal=causal, softmax_scale=softmax_scale, attention_dropout=dropout
+        self.inner_attn, self.inner_cross_attn = get_gqa_attn_cls(
+            use_flash_attn, self.tp_mode, causal, softmax_scale, dropout, sequence_process_group
         )
-
         self.inner_cross_attn_causal = causal
         self.inner_cross_attn_softmax_scale = softmax_scale
         self.inner_cross_attn_dropout = dropout
 
-        self.attn = flash_attn_varlen_kvpacked_func if use_flash_attn else SelfAttention
-        if self.tp_mode == "isp":
-            self.attn = DistributedAttention(self.attn, sequence_process_group=sequence_process_group)
-
         wo_cls = get_linear_cls(self.tp_mode, "row")
         self.wo = wo_cls(
             embed_dim,
             embed_dim,
             process_group,
             bias=bias,
             sequence_parallel=sequence_parallel,
@@ -216,18 +206,18 @@
                 k = self.rotary_emb._single_eval_forward(k)
             kv = torch.concat([k.unsqueeze(2), v.unsqueeze(2)], dim=2)
             if self.dtype is torch.float32 and self.use_flash_attn:
                 if q.dtype not in [torch.float16, torch.bfloat16]:
                     q = q.to(torch.bfloat16)
                 if kv.dtype not in [torch.float16, torch.bfloat16]:
                     kv = kv.to(torch.bfloat16)
-                with torch.cuda.amp.autocast(dtype=torch.bfloat16):
-                    context = self.inner_cross_attn(q, kv).to(self.dtype)
+                with internlm_accelerator.amp.autocast(dtype=torch.bfloat16):
+                    context = self.inner_cross_attn(q=q, kv=kv).to(self.dtype)
             else:
-                context = self.inner_cross_attn(q, kv)
+                context = self.inner_cross_attn(q=q, kv=kv)
 
         else:
             assert self.rotary_emb_dim > 0
             if hasattr(inference_params, "attention_mask") and inference_params.attention_mask is not None:
                 empties = inference_params.attention_mask[..., -1].sum(dim=-1)
                 moved_q = q.clone()
                 moved_k = k.clone()
@@ -293,15 +283,15 @@
 
             # When using FP16, there is a high probability of NAN in the KV.
             # Since NAN cannot be removed by multiplying with and 0, it needs
             # to be removed manually here.
             kv = torch.where(torch.isnan(kv), 0, kv)
 
             if hasattr(inference_params, "attention_mask") and inference_params.attention_mask is not None:
-                assert self.use_flash_attn is True
+                assert gpc.config.use_cuda_flash_attn is True
                 from flash_attn import flash_attn_varlen_kvpacked_func
 
                 if inference_params.sequence_len_offset == 0:  # First entrance, attnmask (bs*seqlen*seqlen)
                     attn_mask = inference_params.attention_mask[:, None, ...]
                     attn_mask = torch.logical_or(
                         torch.ones_like(attn_mask, dtype=torch.bool).triu(diagonal=1), attn_mask
                     )
@@ -321,15 +311,15 @@
                         -1, kv.shape[-3], kv.shape[-2], kv.shape[-1]
                     )
                     if self.dtype is torch.float32:
                         if total_q.dtype not in [torch.float16, torch.bfloat16]:
                             total_q = total_q.to(torch.bfloat16)
                         if total_kv.dtype not in [torch.float16, torch.bfloat16]:
                             total_kv = total_kv.to(torch.bfloat16)
-                        with torch.cuda.amp.autocast(dtype=torch.bfloat16):
+                        with internlm_accelerator.amp.autocast(dtype=torch.bfloat16):
                             output = flash_attn_varlen_kvpacked_func(
                                 q=total_q,
                                 kv=total_kv,
                                 cu_seqlens_q=cu_seqlens,
                                 cu_seqlens_k=cu_seqlens,
                                 max_seqlen_q=max_seqlen_q,
                                 max_seqlen_k=max_seqlen_k,
@@ -382,18 +372,18 @@
                     )
             else:
                 if self.dtype is torch.float32 and self.use_flash_attn:
                     if q.dtype not in [torch.float16, torch.bfloat16]:
                         q = q.to(torch.bfloat16)
                     if kv.dtype not in [torch.float16, torch.bfloat16]:
                         kv = kv.to(torch.bfloat16)
-                    with torch.cuda.amp.autocast(dtype=torch.bfloat16):
-                        context = self.inner_cross_attn(q, kv, causal=True).to(self.dtype)
+                    with internlm_accelerator.amp.autocast(dtype=torch.bfloat16):
+                        context = self.inner_cross_attn(q=q, kv=kv, causal=True).to(self.dtype)
                 else:
-                    context = self.inner_cross_attn(q, kv, causal=True)
+                    context = self.inner_cross_attn(q=q, kv=kv, causal=True)
 
         if seqlen is None:
             context = rearrange(context, "b s h d -> b s (h d)")
         else:
             context = rearrange(context, "b s h d -> (b s) (h d)")
 
         out = self.wo(context)
@@ -407,66 +397,82 @@
                 split x during sequence parallel, we split the batch * seqlen dimension
                 (in case batch is small).
         """
         assert self.use_flash_attn is True
 
         qkv = self.wqkv(x)
 
-        qkv = rearrange(qkv, "t (h gs d) -> t h gs d", gs=self.q_per_kv + 2, d=self.head_dim)
+        qkv = rearrange(qkv, "b t (h gs d) -> b t h gs d", gs=self.q_per_kv + 2, d=self.head_dim)
 
         q, k, v = (qkv[..., : self.q_per_kv, :], qkv[..., -2, :], qkv[..., -1, :])
 
-        q = rearrange(q, "t h gs d -> t (h gs) d")
+        q = rearrange(q, "b t h gs d -> b t (h gs) d")
 
         # qkv shift
         # the rotary embedding in flash attention module in performed by separating the front and back parts, while
         # most of others are done by odd-even methods.
         if not self.rot_embed_HF_impl:
             q = torch.cat([q[..., ::2], q[..., 1::2]], dim=-1)
             k = torch.cat([k[..., ::2], k[..., 1::2]], dim=-1)
 
         indexes = kwargs.pop("indexes")
+
         q = self.rotary_emb._single_forward(q, indexes=indexes)
         k = self.rotary_emb._single_forward(k, indexes=indexes)
 
         if inference_params is None:
-            kv = torch.concat([k.unsqueeze(1), v.unsqueeze(1)], dim=1)
+            kv = torch.concat([k.unsqueeze(2), v.unsqueeze(2)], dim=2)
+            # for packed data, batch dimension with a size of 1 should be directly squeezed off.
+            if internlm_accelerator.get_accelerator_backend() == AcceleratorType.GPU:
+                q = q.squeeze(0)
+                kv = kv.squeeze(0)
+            # since torch_npu only supports fa with no packed data currently, qkv should be unpacked
+            elif internlm_accelerator.get_accelerator_backend() in [AcceleratorType.NPU, AcceleratorType.DIPU]:
+                q = unpack_qkv_before_attn(q, kwargs["cu_seqlens"])
+                kv = unpack_qkv_before_attn(kv, kwargs["cu_seqlens"])
+
             if self.dtype is torch.float32:
                 if q.dtype not in [torch.float16, torch.bfloat16]:
                     q = q.to(torch.bfloat16)
                 if kv.dtype not in [torch.float16, torch.bfloat16]:
                     kv = kv.to(torch.bfloat16)
-                with torch.cuda.amp.autocast(dtype=torch.bfloat16):
-                    context = self.attn(
+                with internlm_accelerator.amp.autocast(dtype=torch.bfloat16):
+                    context = self.inner_attn(
                         q=q,
                         kv=kv,
                         cu_seqlens_q=kwargs["cu_seqlens"],
                         cu_seqlens_k=kwargs["cu_seqlens"],
                         max_seqlen_q=kwargs["max_seqlen"],
                         max_seqlen_k=kwargs["max_seqlen"],
                         dropout_p=self.inner_cross_attn_dropout,
                         softmax_scale=self.inner_cross_attn_softmax_scale,
                         causal=self.inner_cross_attn_causal,
                     ).to(self.dtype)
             else:
-                context = self.attn(
+                context = self.inner_attn(
                     q=q,
                     kv=kv,
                     cu_seqlens_q=kwargs["cu_seqlens"],
                     cu_seqlens_k=kwargs["cu_seqlens"],
                     max_seqlen_q=kwargs["max_seqlen"],
                     max_seqlen_k=kwargs["max_seqlen"],
                     dropout_p=self.inner_cross_attn_dropout,
                     softmax_scale=self.inner_cross_attn_softmax_scale,
                     causal=self.inner_cross_attn_causal,
                 )
         else:
             raise RuntimeError("Not support this right now")
 
-        context = rearrange(context, "b h d -> b (h d)")  # recover shape
+        if internlm_accelerator.get_accelerator_backend() == AcceleratorType.GPU:
+            context = rearrange(context, "s h d -> s (h d)")  # recover the shape
+            context = context.unsqueeze(0)  # restore bsz dimension
+        elif internlm_accelerator.get_accelerator_backend() in [AcceleratorType.NPU, AcceleratorType.DIPU]:
+            context = rearrange(context, "b s h d -> b s (h d)")  # recover the shape
+            context = pack_output_after_attn(context, kwargs["cu_seqlens"])
+
         out = self.wo(context)
         return out
 
 
 class PackedFlashLlamaLayer1D(nn.Module):
     """
     InternLM2 layer.
@@ -526,14 +532,16 @@
         tp_mode: str = "mtp",
         attn_wqkv_init_std: float = 0.02,
         attn_other_init_std: float = 0.02,
         ffn_uplayer_init_std: float = 0.02,
         ffn_other_init_std: float = 0.02,
         init_type: str = "normal",
         rope_base: int = 10000,
+        mlp_layer_fusion: bool = False,
+        multiple_of: int = 256,
     ):
         super().__init__()
         self.checkpoint = checkpoint
         # dropout selective checkpoint can only be enabled when checkpoint is disabled.
         self.dropout_selective_checkpoint = dropout_selective_checkpoint is True and checkpoint is False
         self.layer_idx = layer_idx
         self.use_flash_attn = use_flash_attn
@@ -577,15 +585,15 @@
         self.dropout1 = nn.Dropout(drop_rate)
         if norm_type == "rmsnorm":
             self.attention_norm = RMSNorm(hidden_size, eps=layer_norm_epsilon)
             self.ffn_norm = RMSNorm(hidden_size, eps=layer_norm_epsilon)
         else:
             self.attention_norm = nn.LayerNorm(hidden_size, eps=layer_norm_epsilon)
             self.ffn_norm = nn.LayerNorm(hidden_size, eps=layer_norm_epsilon)
-        if self.fused_dropout_add_ln and self.use_flash_attn:
+        if self.fused_dropout_add_ln and gpc.config.use_cuda_flash_attn:
             from flash_attn.ops.layer_norm import dropout_add_layer_norm
 
             assert dropout_add_layer_norm is not None, "dropout_add_ln is not installed"
             assert isinstance(self.attention_norm, nn.LayerNorm) and isinstance(self.dropout1, nn.Dropout)
 
         sequence_parallel = gpc.config.parallel.get("sequence_parallel", False)
         if use_swiglu or not gpc.config.model.use_flash_attn:
@@ -594,14 +602,17 @@
                 hidden_size,
                 int(hidden_size * mlp_ratio),
                 out_features=hidden_size,
                 process_group=gpc.get_group(parallel_mode),
                 bias=False,
                 device=device,
                 dtype=dtype,
+                mlp_layer_fusion=mlp_layer_fusion,
+                sequence_parallel=sequence_parallel,
+                multiple_of=multiple_of,
             )
         else:
             from flash_attn.modules.mlp import ParallelFusedMLP
 
             self.feed_forward = ParallelFusedMLP(
                 hidden_size,
                 int(hidden_size * mlp_ratio),
@@ -645,14 +656,15 @@
                     self.init_func(std=self.attn_other_init_std)(param.data)
 
             for name, param in self.feed_forward.named_parameters():
                 if self.use_swiglu:
                     if self.use_scaled_init and "w2" in name:
                         self.scaled_init_func(sigma=self.ffn_other_init_std, num_layers=self.layer_idx + 1)(param.data)
                     else:
+                        # candidate: w1, w3, fused_w1_w3
                         self.init_func(
                             std=self.ffn_uplayer_init_std if "w1" in name or "w3" in name else self.ffn_other_init_std
                         )(param.data)
                 else:
                     if self.use_scaled_init and "fc1" not in name:
                         self.scaled_init_func(sigma=self.ffn_other_init_std, num_layers=self.layer_idx + 1)(param.data)
                     else:
@@ -834,14 +846,16 @@
         ffn_uplayer_init_std: float = 0.02,
         ffn_other_init_std: float = 0.02,
         out_head_init_std: float = 0.02,
         init_type: str = "normal",
         rope_base: int = 10000,
         norm_head: bool = False,
         tp_mode: str = "mtp",
+        mlp_layer_fusion: bool = False,
+        multiple_of: int = 256,
     ):
         super().__init__()
 
         self.use_flash_attn = use_flash_attn
 
         if checkpoint_fraction <= 0:
             checkpoint = False
@@ -852,15 +866,15 @@
         self.tp_mode = tp_mode
         if isinstance(gpc.config.parallel["tensor"], dict):
             self.tp_mode = gpc.config.parallel["tensor"].get("mode", "mtp")
 
         if is_reward:
             head_cls = RewardModelLinear
         else:
-            head_cls = InternLM2ScaleColumnParallelLinear
+            head_cls = ScaleColumnParallelLinearWithNormHead
 
         sequence_parallel = gpc.config.parallel.get("sequence_parallel", False)
 
         if first:
             if embed_split_hidden or not gpc.config.model.use_flash_attn:
                 self.tok_embeddings = Embedding1D(num_embeddings=vocab_size, embedding_dim=hidden_size)
             else:
@@ -913,30 +927,32 @@
                     attn_wqkv_init_std=attn_wqkv_init_std,
                     attn_other_init_std=attn_other_init_std,
                     ffn_uplayer_init_std=ffn_uplayer_init_std,
                     ffn_other_init_std=ffn_other_init_std,
                     init_type=init_type,
                     tp_mode=self.tp_mode,
                     rope_base=rope_base,
+                    mlp_layer_fusion=mlp_layer_fusion,
+                    multiple_of=multiple_of,
                 )
                 for lid in range(num_layers)
             ]
         )
 
         if last:
             if not apply_post_layer_norm:
                 if norm_type == "rmsnorm":
                     self.norm = RMSNorm(hidden_size, eps=layer_norm_epsilon)
                 else:
                     self.norm = nn.LayerNorm(hidden_size, eps=layer_norm_epsilon)
 
-            if norm_head and not issubclass(head_cls, InternLM2ScaleColumnParallelLinear):
+            if norm_head and not issubclass(head_cls, ScaleColumnParallelLinearWithNormHead):
                 raise TypeError(
                     "Parameter ``norm_head`` should only be True when head_cls is "
-                    f"``InternLM2ScaleColumnParallelLinear``, instead of {head_cls}."
+                    f"``ScaleColumnParallelLinearWithNormHead``, instead of {head_cls}."
                 )
             self.output = head_cls(  # pylint: disable=E1123
                 in_features=hidden_size,
                 out_features=gpc.get_world_size(ParallelMode.TENSOR) if is_reward else vocab_size,
                 process_group=gpc.get_group(ParallelMode.TENSOR),
                 bias=False,
                 device=device,
@@ -962,16 +978,14 @@
                 )
         if isinstance(cu_seqlens, list):
             assert len(cu_seqlens) == 1
             cu_seqlens = cu_seqlens[0].to(hidden_states.device)
 
         if cu_seqlens is not None:
             cu_seqlens = cu_seqlens.squeeze(0)
-            hidden_states = hidden_states.squeeze(0)  # If cu_seqlens is passed in，it indicated a packed state，
-            # the batch dimension with a size of 1 should be directly squeezed off.
 
         if indexes is not None:
             assert len(indexes) == 1
             # The indexes are used to indicate the actual position IDs of each token in the packed input.
             indexes = indexes[0]
             # if the sequence parallel mode is 'isp', the indexes should also be split in sequence dimension.
             if gpc.config.parallel.sequence_parallel and self.tp_mode == "isp":
@@ -988,36 +1002,33 @@
                 inference_params=inference_params,
                 max_seqlen=max_seqlen,
             )
 
         if hasattr(self, "norm"):
             hidden_states = self.norm(hidden_states.float())
         if hasattr(self, "output"):
-            # Evaluation
-            if gpc.is_evaluating is True:
-                hidden_states = self.output(hidden_states, gather_dim=1, tp_mode=self.tp_mode)
-            else:  # Training
-                hidden_states = self.output(hidden_states, gather_dim=0, tp_mode=self.tp_mode)
+            hidden_states = self.output(hidden_states, gather_dim=1, tp_mode=self.tp_mode)
 
-        if not self.parallel_output:
+        if not self.parallel_output and gpc.is_pipeline_last_stage():
             hidden_states = gather_forward_split_backward(hidden_states, ParallelMode.TENSOR, dim=-1)
 
         return hidden_states
 
 
-def _build_generic_model_1d(num_layers, num_chunks, device=torch.device("cuda"), **kwargs):
+def _build_generic_model_1d(num_layers, num_chunks, **kwargs):
     """
     build generic model 1d
 
     Args:
         num_layers (int): The number of layer.
         num_chunks (int): The number of partitions in pipeline parallel.
-        device (Optional[Union[str, torch.device]]): The device will be used. torch.device("cuda") by default.
+        device (Optional[Union[str, torch.device]]): The device will be used. internlm_accelerator.device() by default.
 
     """
+    device = get_current_device()
     pipeline_size = gpc.get_world_size(ParallelMode.PIPELINE)
     pipeline_rank = gpc.get_local_rank(ParallelMode.PIPELINE)
 
     all_parts = partition_uniform(num_layers, pipeline_size, num_chunks)
     parts = all_parts[pipeline_rank]
     if gpc.is_rank_for_log():
         logger.info(f"The layer sharding is {all_parts}.")
@@ -1081,14 +1092,16 @@
     ffn_other_init_std: float = 0.02,
     out_head_init_std: float = 0.02,
     init_type: str = "normal",
     rope_base: int = 10000,
     norm_head: bool = False,
     max_position_embeddings=2048,
     use_dynamic_ntk_rope=False,
+    mlp_layer_fusion: bool = False,
+    multiple_of: int = 256,
 ):
     """
     Builde model with config
 
     Args:
         num_chunks (int): The number of partitions in pipeline parallel. 1 by default.
         checkpoint (bool): Whether to use checkpointing to save VRAM. False by default.
@@ -1161,10 +1174,12 @@
         ffn_other_init_std=ffn_other_init_std,
         out_head_init_std=out_head_init_std,
         init_type=init_type,
         rope_base=rope_base,
         norm_head=norm_head,
         max_position_embeddings=max_position_embeddings,
         use_dynamic_ntk_rope=use_dynamic_ntk_rope,
+        mlp_layer_fusion=mlp_layer_fusion,
+        multiple_of=multiple_of,
     )
 
     return _build_generic_model_1d(num_layers=num_layers, num_chunks=num_chunks, **cfg)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/model/modeling_llama.py` & `InternEvo-0.4.0.dev20240403/internlm/model/modeling_llama.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,51 +2,53 @@
 from typing import Optional
 
 import torch
 import torch.nn.functional as F
 from einops import rearrange
 from torch import nn
 
+from internlm.accelerator import AcceleratorType, get_accelerator
 from internlm.core.context import ParallelMode
 from internlm.core.context.parallel_context import global_context as gpc
 from internlm.core.naive_amp import set_output_attr_to_module
 from internlm.initialize.initialize_tensor import (
     normal_,
     scaled_init_method_normal,
     scaled_init_method_uniform,
     uniform_,
 )
-from internlm.model.embedding import Embedding1D, RotaryEmbedding
-from internlm.model.linear import (
+from internlm.model.modules.embedding import Embedding1D, RotaryEmbedding
+from internlm.model.modules.mlp import get_mlp_cls
+from internlm.model.modules.multi_head_attention import (
+    _update_kv_cache,
+    get_gqa_attn_cls,
+)
+from internlm.model.ops.linear import (
     RewardModelLinear,
     ScaleColumnParallelLinear,
     get_linear_cls,
-    get_mlp_cls,
-)
-from internlm.model.multi_head_attention import (
-    CrossAttention,
-    DistributedAttention,
-    SelfAttention,
-    _update_kv_cache,
 )
 from internlm.model.utils import (
     gather_forward_split_backward,
+    pack_output_after_attn,
     split_forward_gather_backward,
     try_import_RMSNorm,
+    unpack_qkv_before_attn,
 )
+from internlm.solver.activation_checkpoint import activation_checkpoint
 from internlm.solver.pipeline_utils import partition_uniform
-from internlm.utils.checkpoint import activation_checkpoint
-from internlm.utils.common import filter_kwargs
+from internlm.utils.common import filter_kwargs, get_current_device
 from internlm.utils.logger import get_logger
 from internlm.utils.registry import MODEL_INITIALIZER
 
 MODEL_TYPE = "LLAMA2"
 
 logger = get_logger(__file__)
 RMSNorm = try_import_RMSNorm()
+internlm_accelerator = get_accelerator()
 
 
 class MHA(nn.Module):
     """
     Multi-head self-attention and cross-attention.
 
     Args:
@@ -142,33 +144,21 @@
             self.kv_dim,
             process_group,
             bias=bias,
             sequence_parallel=sequence_parallel,
             **factory_kwargs,
         )
 
-        if use_flash_attn:
-            from flash_attn import flash_attn_varlen_kvpacked_func
-            from flash_attn.modules.mha import FlashCrossAttention, FlashSelfAttention
-
-        inner_attn_cls = FlashSelfAttention if use_flash_attn else SelfAttention
-        inner_cross_attn_cls = FlashCrossAttention if use_flash_attn else CrossAttention
-        self.inner_attn = inner_attn_cls(causal=causal, softmax_scale=softmax_scale, attention_dropout=dropout)
-        self.inner_cross_attn = inner_cross_attn_cls(
-            causal=causal, softmax_scale=softmax_scale, attention_dropout=dropout
+        self.inner_attn, self.inner_cross_attn = get_gqa_attn_cls(
+            use_flash_attn, self.tp_mode, causal, softmax_scale, dropout, sequence_process_group
         )
-
         self.inner_cross_attn_causal = causal
         self.inner_cross_attn_softmax_scale = softmax_scale
         self.inner_cross_attn_dropout = dropout
 
-        self.attn = flash_attn_varlen_kvpacked_func if use_flash_attn else SelfAttention
-        if self.tp_mode == "isp":
-            self.attn = DistributedAttention(self.attn, sequence_process_group=sequence_process_group)
-
         # output projection always have the bias (for now)
         out_proj_cls = get_linear_cls(self.tp_mode, "row")
         self.wo = out_proj_cls(
             embed_dim,
             embed_dim,
             process_group,
             bias=bias,
@@ -210,18 +200,18 @@
                 k = self.rotary_emb._single_eval_forward(k)
             kv = torch.concat([k.unsqueeze(2), v.unsqueeze(2)], dim=2)
             if self.dtype is torch.float32 and self.use_flash_attn:
                 if q.dtype not in [torch.float16, torch.bfloat16]:
                     q = q.to(torch.bfloat16)
                 if kv.dtype not in [torch.float16, torch.bfloat16]:
                     kv = kv.to(torch.bfloat16)
-                with torch.cuda.amp.autocast(dtype=torch.bfloat16):
-                    context = self.inner_cross_attn(q, kv).to(self.dtype)
+                with internlm_accelerator.amp.autocast(dtype=torch.bfloat16):
+                    context = self.inner_cross_attn(q=q, kv=kv).to(self.dtype)
             else:
-                context = self.inner_cross_attn(q, kv)
+                context = self.inner_cross_attn(q=q, kv=kv)
 
         else:
             assert self.rotary_emb_dim > 0
             if hasattr(inference_params, "attention_mask") and inference_params.attention_mask is not None:
                 empties = inference_params.attention_mask[..., -1].sum(dim=-1)
                 moved_q = q.clone()
                 moved_k = k.clone()
@@ -287,15 +277,15 @@
 
             # When using FP16, there is a high probability of NAN in the KV.
             # Since NAN cannot be removed by multiplying with and 0, it needs
             # to be removed manually here.
             kv = torch.where(torch.isnan(kv), 0, kv)
 
             if hasattr(inference_params, "attention_mask") and inference_params.attention_mask is not None:
-                assert self.use_flash_attn is True
+                assert gpc.config.use_cuda_flash_attn is True
                 from flash_attn.flash_attn_interface import FlashAttnVarlenKVPackedFunc
 
                 if inference_params.sequence_len_offset == 0:  # First entrance, attnmask (bs*seqlen*seqlen)
                     attn_mask = inference_params.attention_mask[:, None, ...]
                     attn_mask = torch.logical_or(
                         torch.ones_like(attn_mask, dtype=torch.bool).triu(diagonal=1), attn_mask
                     )
@@ -316,15 +306,15 @@
                     )
 
                     if self.dtype is torch.float32:
                         if total_q.dtype not in [torch.float16, torch.bfloat16]:
                             total_q = total_q.to(torch.bfloat16)
                         if total_kv.dtype not in [torch.float16, torch.bfloat16]:
                             total_kv = total_kv.to(torch.bfloat16)
-                        with torch.cuda.amp.autocast(dtype=torch.bfloat16):
+                        with internlm_accelerator.amp.autocast(dtype=torch.bfloat16):
                             output = FlashAttnVarlenKVPackedFunc.apply(
                                 total_q,
                                 total_kv,
                                 cu_seqlens,
                                 cu_seqlens,
                                 max_seqlen_q,
                                 max_seqlen_k,
@@ -381,18 +371,18 @@
                     )
             else:
                 if self.dtype is torch.float32 and self.use_flash_attn:
                     if q.dtype not in [torch.float16, torch.bfloat16]:
                         q = q.to(torch.bfloat16)
                     if kv.dtype not in [torch.float16, torch.bfloat16]:
                         kv = kv.to(torch.bfloat16)
-                    with torch.cuda.amp.autocast(dtype=torch.bfloat16):
-                        context = self.inner_cross_attn(q, kv, causal=True).to(self.dtype)
+                    with internlm_accelerator.amp.autocast(dtype=torch.bfloat16):
+                        context = self.inner_cross_attn(q=q, kv=kv, causal=True).to(self.dtype)
                 else:
-                    context = self.inner_cross_attn(q, kv, causal=True)
+                    context = self.inner_cross_attn(q=q, kv=kv, causal=True)
         if seqlen is None:
             context = rearrange(context, "b s h d -> b s (h d)")
         else:
             context = rearrange(context, "b s h d -> (b s) (h d)")
         out = self.wo(context)
         return out
 
@@ -404,63 +394,80 @@
             x: (batch, seqlen, hidden_dim) (where hidden_dim = num heads * head dim) if seqlen=None.
                 If seqlen is not None, x is (batch * seqlen, hidden_dim). This is so that when we
                 split x during sequence parallel, we split the batch * seqlen dimension
                 (in case batch is small).
         """
         assert self.use_flash_attn is True
         q, k, v = self.wq(x), self.wk(x), self.wv(x)
-        q = rearrange(q, "t (h d) -> t h d", d=self.head_dim)
-        k = rearrange(k, "t (h d) -> t h d", d=self.head_dim)
-        v = rearrange(v, "t (h d) -> t h d", d=self.head_dim)
+        q = rearrange(q, "b t (h d) -> b t h d", d=self.head_dim)
+        k = rearrange(k, "b t (h d) -> b t h d", d=self.head_dim)
+        v = rearrange(v, "b t (h d) -> b t h d", d=self.head_dim)
 
         # qkv shift
         # the rotary embedding in flash attention module in performed by separating the front and back parts, while
         # most of others are done by odd-even methods.
         if not self.rot_embed_HF_impl:
             q = torch.cat([q[..., ::2], q[..., 1::2]], dim=-1)
             k = torch.cat([k[..., ::2], k[..., 1::2]], dim=-1)
 
         indexes = kwargs.pop("indexes")
+
         q = self.rotary_emb._single_forward(q, indexes=indexes)
         k = self.rotary_emb._single_forward(k, indexes=indexes)
 
         if inference_params is None:
-            kv = torch.concat([k.unsqueeze(1), v.unsqueeze(1)], dim=1)
+            kv = torch.concat([k.unsqueeze(2), v.unsqueeze(2)], dim=2)
+            # for packed data, batch dimension with a size of 1 should be directly squeezed off.
+            if internlm_accelerator.get_accelerator_backend() == AcceleratorType.GPU:
+                q = q.squeeze(0)
+                kv = kv.squeeze(0)
+            # since torch_npu only supports fa with no packed data currently, qkv should be unpacked
+            elif internlm_accelerator.get_accelerator_backend() in [AcceleratorType.NPU, AcceleratorType.DIPU]:
+                q = unpack_qkv_before_attn(q, kwargs["cu_seqlens"])
+                kv = unpack_qkv_before_attn(kv, kwargs["cu_seqlens"])
+
             if self.dtype is torch.float32:
                 if q.dtype not in [torch.float16, torch.bfloat16]:
                     q = q.to(torch.bfloat16)
                 if kv.dtype not in [torch.float16, torch.bfloat16]:
                     kv = kv.to(torch.bfloat16)
-                with torch.cuda.amp.autocast(dtype=torch.bfloat16):
-                    context = self.attn(
+                with internlm_accelerator.amp.autocast(dtype=torch.bfloat16):
+                    context = self.inner_attn(
                         q=q,
                         kv=kv,
                         cu_seqlens_q=kwargs["cu_seqlens"],
                         cu_seqlens_k=kwargs["cu_seqlens"],
                         max_seqlen_q=kwargs["max_seqlen"],
                         max_seqlen_k=kwargs["max_seqlen"],
                         dropout_p=self.inner_cross_attn_dropout,
                         softmax_scale=self.inner_cross_attn_softmax_scale,
                         causal=self.inner_cross_attn_causal,
                     ).to(self.dtype)
             else:
-                context = self.attn(
+                context = self.inner_attn(
                     q=q,
                     kv=kv,
                     cu_seqlens_q=kwargs["cu_seqlens"],
                     cu_seqlens_k=kwargs["cu_seqlens"],
                     max_seqlen_q=kwargs["max_seqlen"],
                     max_seqlen_k=kwargs["max_seqlen"],
                     dropout_p=self.inner_cross_attn_dropout,
                     softmax_scale=self.inner_cross_attn_softmax_scale,
                     causal=self.inner_cross_attn_causal,
                 )
         else:
             raise RuntimeError("Not support this right now")
-        context = rearrange(context, "b h d -> b (h d)")  # recover shape
+
+        if internlm_accelerator.get_accelerator_backend() == AcceleratorType.GPU:
+            context = rearrange(context, "s h d -> s (h d)")  # recover the shape
+            context = context.unsqueeze(0)  # restore bsz dimension
+        elif internlm_accelerator.get_accelerator_backend() in [AcceleratorType.NPU, AcceleratorType.DIPU]:
+            context = rearrange(context, "b s h d -> b s (h d)")  # recover the shape
+            context = pack_output_after_attn(context, kwargs["cu_seqlens"])
+
         out = self.wo(context)
         return out
 
 
 class PackedFlashLlamaLayer1D(nn.Module):
     """
     1D Packed Flash Llama Layer.
@@ -516,14 +523,16 @@
         attn_wqkv_init_std: float = 0.02,
         attn_other_init_std: float = 0.02,
         ffn_uplayer_init_std: float = 0.02,
         ffn_other_init_std: float = 0.02,
         init_type: str = "normal",
         rope_base: int = 10000,
         tp_mode: str = "mtp",
+        mlp_layer_fusion: bool = False,
+        multiple_of: int = 256,
     ):
         super().__init__()
         self.checkpoint = checkpoint
         # dropout selective checkpoint can only be enabled when checkpoint is disabled.
         self.dropout_selective_checkpoint = dropout_selective_checkpoint is True and checkpoint is False
         self.layer_idx = layer_idx
         self.use_flash_attn = use_flash_attn
@@ -563,31 +572,34 @@
         self.dropout1 = nn.Dropout(drop_rate)
         if norm_type == "rmsnorm":
             self.attention_norm = RMSNorm(hidden_size, eps=layer_norm_epsilon)
             self.ffn_norm = RMSNorm(hidden_size, eps=layer_norm_epsilon)
         else:
             self.attention_norm = nn.LayerNorm(hidden_size, eps=layer_norm_epsilon)
             self.ffn_norm = nn.LayerNorm(hidden_size, eps=layer_norm_epsilon)
-        if self.fused_dropout_add_ln and self.use_flash_attn:
+        if self.fused_dropout_add_ln and gpc.config.use_cuda_flash_attn:
             from flash_attn.ops.layer_norm import dropout_add_layer_norm
 
             assert dropout_add_layer_norm is not None, "dropout_add_ln is not installed"
             assert isinstance(self.attention_norm, nn.LayerNorm) and isinstance(self.dropout1, nn.Dropout)
 
         sequence_parallel = gpc.config.parallel.get("sequence_parallel", False)
-        if use_swiglu or not gpc.config.model.use_flash_attn:
+        if use_swiglu or not gpc.config.use_cuda_flash_attn:
             mlp_cls = get_mlp_cls(self.tp_mode)
             self.feed_forward = mlp_cls(
                 hidden_size,
                 int(hidden_size * mlp_ratio),
                 out_features=hidden_size,
                 process_group=gpc.get_group(parallel_mode),
                 bias=False,
                 device=device,
                 dtype=dtype,
+                mlp_layer_fusion=mlp_layer_fusion,
+                sequence_parallel=gpc.config.parallel.sequence_parallel,
+                multiple_of=multiple_of,
             )
         else:
             from flash_attn.modules.mlp import ParallelFusedMLP
 
             self.feed_forward = ParallelFusedMLP(
                 hidden_size,
                 int(hidden_size * mlp_ratio),
@@ -631,14 +643,15 @@
                     self.init_func(std=self.attn_other_init_std)(param.data)
 
             for name, param in self.feed_forward.named_parameters():
                 if self.use_swiglu:
                     if self.use_scaled_init and "w2" in name:
                         self.scaled_init_func(sigma=self.ffn_other_init_std, num_layers=self.layer_idx + 1)(param.data)
                     else:
+                        # candidate: w1, w3, fused_w1_w3
                         self.init_func(
                             std=self.ffn_uplayer_init_std if "w1" in name or "w3" in name else self.ffn_other_init_std
                         )(param.data)
                 else:
                     if self.use_scaled_init and "fc1" not in name:
                         self.scaled_init_func(sigma=self.ffn_other_init_std, num_layers=self.layer_idx + 1)(param.data)
                     else:
@@ -769,15 +782,14 @@
         attn_wqkv_init_std (float): std used to init attn_wqkv weight. 0.02 by default,
         attn_other_init_std (float): std used to init attn_other weight. 0.02 by default,
         ffn_uplayer_init_std (float): std used to init w1, w2 weight in ffn when using glu
             otherwise init fc1 weight in ffn. 0.02 by default,
         ffn_other_init_std (float): std used to init ffn_other weight. 0.02 by default,
         out_head_init_std (float): std used to init output lmhead weight. 0.02 by default,
         init_type (str): Initialization type. Use uniform or normal. "normal" by default,
-        extra_pred_tokens (int): The number of extra output head for multi-token-prediction. 0 by default.
         rope_base (int): The value of `base` for rotary position embeddings. 10000 by default.
     """
 
     def __init__(
         self,
         num_layers: int = 12,
         hidden_size: int = 768,
@@ -811,16 +823,17 @@
         embedding_init_std: float = 0.02,
         attn_wqkv_init_std: float = 0.02,
         attn_other_init_std: float = 0.02,
         ffn_uplayer_init_std: float = 0.02,
         ffn_other_init_std: float = 0.02,
         out_head_init_std: float = 0.02,
         init_type: str = "normal",
-        extra_pred_tokens: int = 0,
         rope_base: int = 10000,
+        mlp_layer_fusion: bool = False,
+        multiple_of: int = 256,
     ):
         super().__init__()
 
         self.use_flash_attn = use_flash_attn
         if checkpoint_fraction <= 0:
             checkpoint = False
         if not checkpoint:
@@ -833,15 +846,15 @@
 
         if is_reward:
             head_cls = RewardModelLinear
         else:
             head_cls = ScaleColumnParallelLinear
 
         if first:
-            if embed_split_hidden or not gpc.config.model.use_flash_attn:
+            if embed_split_hidden or not gpc.config.use_cuda_flash_attn:
                 self.tok_embeddings = Embedding1D(num_embeddings=vocab_size, embedding_dim=hidden_size)
             else:
                 from flash_attn.modules.embedding import ParallelGPT2Embeddings
 
                 self.tok_embeddings = ParallelGPT2Embeddings(
                     embed_dim=hidden_size,
                     vocab_size=vocab_size,
@@ -886,14 +899,16 @@
                     attn_wqkv_init_std=attn_wqkv_init_std,
                     attn_other_init_std=attn_other_init_std,
                     ffn_uplayer_init_std=ffn_uplayer_init_std,
                     ffn_other_init_std=ffn_other_init_std,
                     init_type=init_type,
                     rope_base=rope_base,
                     tp_mode=self.tp_mode,
+                    mlp_layer_fusion=mlp_layer_fusion,
+                    multiple_of=multiple_of,
                 )
                 for lid in range(num_layers)
             ]
         )
 
         if last:
             if not apply_post_layer_norm:
@@ -914,37 +929,14 @@
             set_output_attr_to_module(self.output)
             for _, param in self.output.named_parameters():
                 if init_type == "normal":
                     normal_(std=out_head_init_std)(param)
                 else:
                     uniform_(std=out_head_init_std)(param)
 
-            if extra_pred_tokens > 0:
-                self.extra_pred_tokens = extra_pred_tokens
-                assert not is_reward, "extra_pred_tokens > 0 means using multi token prediction, not implement for RLHF"
-                self.extra_outputs = nn.ModuleList(
-                    [
-                        head_cls(
-                            in_features=hidden_size,
-                            out_features=vocab_size,
-                            process_group=gpc.get_group(ParallelMode.TENSOR),
-                            bias=False,
-                            device=device,
-                            dtype=dtype,
-                            weight_scale=embed_grad_scale,
-                        )
-                        for _ in range(self.extra_pred_tokens)
-                    ]
-                )
-                for _, param in self.extra_outputs.named_parameters():
-                    if init_type == "normal":
-                        normal_(std=out_head_init_std)(param)
-                    else:
-                        uniform_(std=out_head_init_std)(param)
-
         self.parallel_output = parallel_output
 
     def forward(self, hidden_states=None, cu_seqlens=None, input_ids=None, indexes=None, inference_params=None):
         # attention_mask: compute attention on the places where the value is 1
         if hasattr(self, "tok_embeddings"):
             hidden_states = self.tok_embeddings(input_ids)
             if self.embed_grad_scale != 1:
@@ -953,16 +945,14 @@
                 )
         if isinstance(cu_seqlens, list):
             assert len(cu_seqlens) == 1
             cu_seqlens = cu_seqlens[0].to(hidden_states.device)
 
         if cu_seqlens is not None:
             cu_seqlens = cu_seqlens.squeeze(0)
-            hidden_states = hidden_states.squeeze(0)  # If cu_seqlens is passed in，it indicated a packed state，
-            # the batch dimension with a size of 1 should be directly squeezed off.
 
         if indexes is not None:
             assert len(indexes) == 1
             # The indexes are used to indicate the actual position IDs of each token in the packed input.
             indexes = indexes[0]
             # if the sequence parallel mode is 'isp', the indexes should also be split in sequence dimension.
             if gpc.config.parallel.sequence_parallel and self.tp_mode == "isp":
@@ -978,49 +968,35 @@
                 indexes=indexes,
                 inference_params=inference_params,
                 max_seqlen=max_seqlen,
             )
 
         if hasattr(self, "norm"):
             hidden_states = self.norm(hidden_states.float())
-        if hasattr(self, "extra_pred_tokens") and self.extra_pred_tokens > 0:
-            extra_hidden_states_list = [self.extra_outputs[i](hidden_states) for i in range(self.extra_pred_tokens)]
-        else:
-            extra_hidden_states_list = None
+
         if hasattr(self, "output"):
-            # Evaluation
-            if gpc.is_evaluating is True:
-                hidden_states = self.output(hidden_states, gather_dim=1, tp_mode=self.tp_mode)
-            else:  # Training
-                hidden_states = self.output(hidden_states, gather_dim=0, tp_mode=self.tp_mode)
+            hidden_states = self.output(hidden_states, gather_dim=1, tp_mode=self.tp_mode)
 
-        if not self.parallel_output:
+        if not self.parallel_output and gpc.is_pipeline_last_stage():
             hidden_states = gather_forward_split_backward(hidden_states, ParallelMode.TENSOR, dim=-1)
-            if extra_hidden_states_list is not None:
-                extra_hidden_states_list = [
-                    gather_forward_split_backward(extra_hidden_states, ParallelMode.TENSOR, dim=-1)
-                    for extra_hidden_states in extra_hidden_states_list
-                ]
-
-        if extra_hidden_states_list is not None:
-            return (hidden_states, extra_hidden_states_list)
 
         return hidden_states
 
 
-def _build_generic_model_1d(num_layers, num_chunks, device=torch.device("cuda"), **kwargs):
+def _build_generic_model_1d(num_layers, num_chunks, **kwargs):
     """
     build generic model 1d
 
     Args:
         num_layers (int): The number of layer.
         num_chunks (int): The number of partitions in pipeline parallel.
-        device (Optional[Union[str, torch.device]]): The device will be used. torch.device("cuda") by default.
+        device (Optional[Union[str, torch.device]]): The device will be used. internlm_accelerator.device() by default.
 
     """
+    device = get_current_device()
     pipeline_size = gpc.get_world_size(ParallelMode.PIPELINE)
     pipeline_rank = gpc.get_local_rank(ParallelMode.PIPELINE)
 
     all_parts = partition_uniform(num_layers, pipeline_size, num_chunks)
     parts = all_parts[pipeline_rank]
     if gpc.is_rank_for_log():
         logger.info(f"The layer sharding is {all_parts}.")
@@ -1080,16 +1056,17 @@
     embedding_init_std: float = 0.02,
     attn_wqkv_init_std: float = 0.02,
     attn_other_init_std: float = 0.02,
     ffn_uplayer_init_std: float = 0.02,
     ffn_other_init_std: float = 0.02,
     out_head_init_std: float = 0.02,
     init_type: str = "normal",
-    extra_pred_tokens: int = 0,
     rope_base: int = 10000,
+    mlp_layer_fusion: bool = False,
+    multiple_of: int = 256,
 ):
     """
     Builde model with config
 
     Args:
         num_chunks (int): The number of partitions in pipeline parallel. 1 by default.
         checkpoint (bool): Whether to use checkpointing to save VRAM. False by default.
@@ -1120,15 +1097,14 @@
         attn_wqkv_init_std (float): std used to init attn_wqkv weight. 0.02 by default,
         attn_other_init_std (float): std used to init attn_other weight. 0.02 by default,
         ffn_uplayer_init_std (float): std used to init w1, w2 weight in ffn when using glu
             otherwise init fc1 weight in ffn. 0.02 by default,
         ffn_other_init_std (float): std used to init ffn_other weight. 0.02 by default,
         out_head_init_std (float): std used to init output lmhead weight. 0.02 by default,
         init_type (str): Initialization type. Use uniform or normal. "normal" by default,
-        extra_pred_tokens (int): The number of extra output head for multi-token-prediction. 0 by default.
         rope_base (int): The value of `base` for rotary position embeddings. 10000 by default.
     """
     if deepnorm:
         raise AssertionError("deepnorm will not be supported in future versions." "Use early versions if necessary.")
 
     cfg = dict(
         hidden_size=hidden_size,
@@ -1157,12 +1133,13 @@
         embedding_init_std=embedding_init_std,
         attn_wqkv_init_std=attn_wqkv_init_std,
         attn_other_init_std=attn_other_init_std,
         ffn_uplayer_init_std=ffn_uplayer_init_std,
         ffn_other_init_std=ffn_other_init_std,
         out_head_init_std=out_head_init_std,
         init_type=init_type,
-        extra_pred_tokens=extra_pred_tokens,
         rope_base=rope_base,
+        mlp_layer_fusion=mlp_layer_fusion,
+        multiple_of=multiple_of,
     )
 
     return _build_generic_model_1d(num_layers=num_layers, num_chunks=num_chunks, **cfg)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/model/modeling_moe.py` & `InternEvo-0.4.0.dev20240403/internlm/model/modeling_moe.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,30 +7,27 @@
 import torch
 from torch import nn
 
 from internlm.core.context import ParallelMode
 from internlm.core.context.parallel_context import global_context as gpc
 from internlm.core.naive_amp import set_fp32_attr_to_module
 from internlm.initialize.initialize_tensor import normal_, scaled_init_method_normal
-from internlm.model.embedding import Embedding1D
-from internlm.model.linear import (
-    RewardModelLinear,
-    ScaleColumnParallelLinear,
-    get_mlp_cls,
-)
+from internlm.model.modules.embedding import Embedding1D
+from internlm.model.modules.mlp import get_mlp_cls
+from internlm.model.modules.multi_head_attention import MHA
 from internlm.model.moe import MoE
-from internlm.model.multi_head_attention import MHA
+from internlm.model.ops.linear import RewardModelLinear, ScaleColumnParallelLinear
 from internlm.model.utils import (
     gather_forward_split_backward,
     split_forward_gather_backward,
     try_import_RMSNorm,
 )
+from internlm.solver.activation_checkpoint import activation_checkpoint
 from internlm.solver.pipeline_utils import partition_uniform
-from internlm.utils.checkpoint import activation_checkpoint
-from internlm.utils.common import filter_kwargs
+from internlm.utils.common import filter_kwargs, get_current_device
 from internlm.utils.logger import get_logger
 from internlm.utils.registry import MODEL_INITIALIZER
 
 MODEL_TYPE = "INTERNLM_MoE"
 
 logger = get_logger(__file__)
 RMSNorm = try_import_RMSNorm()
@@ -78,14 +75,16 @@
         norm_type: str = "rmsnorm",
         dropout_selective_checkpoint: bool = True,
         use_scaled_init: bool = True,
         use_swiglu: bool = True,
         use_flash_attn: bool = True,
         num_experts: int = 1,
         tp_mode: str = "mtp",
+        mlp_layer_fusion: bool = False,
+        multiple_of: int = 256,
     ):
         super().__init__()
         self.checkpoint = checkpoint
         # dropout selective checkpoint can only be enabled when checkpoint is disabled.
         self.dropout_selective_checkpoint = dropout_selective_checkpoint is True and checkpoint is False
         self.layer_idx = layer_idx
         self.use_flash_attn = use_flash_attn
@@ -119,24 +118,27 @@
         else:
             self.norm1 = nn.LayerNorm(hidden_size, eps=layer_norm_epsilon)
             self.norm2 = nn.LayerNorm(hidden_size, eps=layer_norm_epsilon)
 
         self.num_experts = num_experts
         ep_size = gpc.get_world_size(ParallelMode.EXPERT)
         if num_experts <= 1:  # dense, not MoE
-            if use_swiglu or not use_flash_attn:
+            if use_swiglu or not gpc.config.use_cuda_flash_attn:
                 mlp_cls = get_mlp_cls(self.tp_mode)
                 self.mlp = mlp_cls(
                     hidden_size,
                     int(hidden_size * mlp_ratio),
                     out_features=hidden_size,
                     process_group=gpc.get_group(parallel_mode),
                     bias=False,
                     device=device,
                     dtype=dtype,
+                    mlp_layer_fusion=mlp_layer_fusion,
+                    sequence_parallel=gpc.config.parallel.sequence_parallel,
+                    multiple_of=multiple_of,
                 )
             else:
                 from flash_attn.modules.mlp import ParallelFusedMLP
 
                 self.mlp = ParallelFusedMLP(
                     hidden_size,
                     int(hidden_size * mlp_ratio),
@@ -149,17 +151,21 @@
                     checkpoint_lvl=0,
                     heuristic="auto",
                     device=device,
                     dtype=dtype,
                 )
         else:
             # replace mlp by MoE module. The expert in MoE is a FeedForward module.
+            mlp_cls = get_mlp_cls(self.tp_mode)
             self.mlp = MoE(
-                hidden_size=hidden_size,
+                hidden_size,
+                int(hidden_size * mlp_ratio),
+                out_features=hidden_size,
                 num_experts=num_experts,
+                ep_cls=mlp_cls,
                 ep_group=gpc.get_group(ParallelMode.EXPERT),
                 ep_size=ep_size,
                 device=device,
                 dtype=dtype,
             )
             set_fp32_attr_to_module(self.mlp.moe_layer.gate)
 
@@ -185,15 +191,16 @@
             for name, param in self.mlp.named_parameters():
                 if param.ndim == 1 and "bias" in name:
                     param.data.zero_()
                 elif self.use_swiglu:
                     if self.use_scaled_init and "w2" in name:
                         scaled_init_method_normal(sigma=0.006, num_layers=self.layer_idx + 1)(param.data)
                     else:
-                        normal_(std=0.006 if "w1" in name or "w2" in name else 0.0015)(param.data)
+                        # candidate: w1, w3, fused_w1_w3
+                        normal_(std=0.006 if "w1" in name or "w3" in name else 0.0015)(param.data)
                 else:
                     if self.use_scaled_init and "fc1" not in name:
                         scaled_init_method_normal(sigma=0.006, num_layers=self.layer_idx + 1)(param.data)
                     else:
                         normal_(std=0.006 if "fc1" in name else 0.0015)(param.data)
 
     def forward(self, hidden_states, cu_seqlens=None, indexes=None, inference_params=None, max_seqlen=None):
@@ -318,29 +325,31 @@
         norm_type: str = "rmsnorm",
         is_reward: bool = False,
         dropout_selective_checkpoint: bool = True,
         use_scaled_init: bool = True,
         use_swiglu: bool = True,
         use_flash_attn: bool = True,
         num_experts: bool = 1,
+        mlp_layer_fusion: bool = False,
+        multiple_of: int = 256,
     ):
         super().__init__()
 
         checkpoint_layer_num = int(num_layers * checkpoint)
         self.tp_mode = "mtp"
         if isinstance(gpc.config.parallel["tensor"], dict):
             self.tp_mode = gpc.config.parallel["tensor"].get("mode", "mtp")
 
         if is_reward:
             head_cls = RewardModelLinear
         else:
             head_cls = ScaleColumnParallelLinear
 
         if first:
-            if embed_split_hidden or not use_flash_attn:
+            if embed_split_hidden or not gpc.config.use_cuda_flash_attn:
                 self.embedding = Embedding1D(num_embeddings=vocab_size, embedding_dim=hidden_size)
             else:
                 from flash_attn.modules.embedding import ParallelGPT2Embeddings
 
                 self.embedding = ParallelGPT2Embeddings(
                     embed_dim=hidden_size,
                     vocab_size=vocab_size,
@@ -373,14 +382,16 @@
                     norm_type=norm_type,
                     dropout_selective_checkpoint=dropout_selective_checkpoint,
                     use_scaled_init=use_scaled_init,
                     use_swiglu=use_swiglu,
                     use_flash_attn=use_flash_attn,
                     num_experts=num_experts,
                     tp_mode=self.tp_mode,
+                    mlp_layer_fusion=mlp_layer_fusion,
+                    multiple_of=multiple_of,
                 )
                 for lid in range(num_layers)
             ]
         )
         if last:
             if norm_type == "rmsnorm":
                 self.norm = RMSNorm(hidden_size, eps=layer_norm_epsilon)
@@ -411,16 +422,14 @@
                 )
         if isinstance(cu_seqlens, list):
             assert len(cu_seqlens) == 1
             cu_seqlens = cu_seqlens[0].to(hidden_states.device)
 
         if cu_seqlens is not None:
             cu_seqlens = cu_seqlens.squeeze(0)
-            hidden_states = hidden_states.squeeze(0)  # If cu_seqlens is passed in，it indicated a packed state，
-            # the batch dimension with a size of 1 should be directly squeezed off.
 
         if indexes is not None:
             assert len(indexes) == 1
             # The indexes are used to indicate the actual position IDs of each token in the packed input.
             indexes = indexes[0]
             # if the sequence parallel mode is 'isp', the indexes should also be split in sequence dimension.
             if gpc.config.parallel.sequence_parallel and self.tp_mode == "isp":
@@ -438,35 +447,32 @@
                 max_seqlen=max_seqlen,
             )
             moe_losses.append(mos_loss)
 
         if hasattr(self, "norm"):
             hidden_states = self.norm(hidden_states.float())
         if hasattr(self, "head"):
-            # Evaluation
-            if hidden_states.ndim == 3:
-                hidden_states = self.head(hidden_states, gather_dim=1, tp_mode=self.tp_mode)
-            else:  # Training
-                hidden_states = self.head(hidden_states, gather_dim=0, tp_mode=self.tp_mode)
+            hidden_states = self.head(hidden_states, gather_dim=1, tp_mode=self.tp_mode)
 
-        if not self.parallel_output:
+        if not self.parallel_output and gpc.is_pipeline_last_stage():
             hidden_states = gather_forward_split_backward(hidden_states, ParallelMode.TENSOR, dim=-1)
         return hidden_states, moe_losses
 
 
-def _build_generic_model_1d(num_layers, num_chunks, device=torch.device("cuda"), **kwargs):
+def _build_generic_model_1d(num_layers, num_chunks, **kwargs):
     """
     build generic model 1d
 
     Args:
         num_layers (int): The number of layer.
         num_chunks (int): The number of partitions in pipeline parallel.
-        device (Optional[Union[str, torch.device]]): The device will be used. torch.device("cuda") by default.
+        device (Optional[Union[str, torch.device]]): The device will be used. internlm_accelerator.device() by default.
 
     """
+    device = get_current_device()
     pipeline_size = gpc.get_world_size(ParallelMode.PIPELINE)
     pipeline_rank = gpc.get_local_rank(ParallelMode.PIPELINE)
 
     all_parts = partition_uniform(num_layers, pipeline_size, num_chunks)
     parts = all_parts[pipeline_rank]
     if gpc.is_rank_for_log():
         logger.info(f"The layer sharding is {all_parts}.")
@@ -517,14 +523,16 @@
     dropout_selective_checkpoint=True,
     use_scaled_init: bool = True,
     use_swiglu: bool = True,
     use_flash_attn: bool = True,
     num_experts: int = 1,
     moe_use_residual: bool = False,  # pylint: disable=W0613
     moe_type: str = None,  # pylint: disable=W0613
+    mlp_layer_fusion: bool = False,
+    multiple_of: int = 256,
 ):
     """
     Build model with config.
 
     Args:
         num_chunks (int): The number of partitions in pipeline parallel. 1 by default.
         checkpoint (bool): Whether to use checkpointing to save VRAM. False by default.
@@ -576,10 +584,12 @@
         layer_norm_epsilon=layer_norm_epsilon,
         is_reward=is_reward,
         dropout_selective_checkpoint=dropout_selective_checkpoint,
         use_scaled_init=use_scaled_init,
         use_swiglu=use_swiglu,
         use_flash_attn=use_flash_attn,
         num_experts=num_experts,
+        mlp_layer_fusion=mlp_layer_fusion,
+        multiple_of=multiple_of,
     )
 
     return _build_generic_model_1d(num_layers=num_layers, num_chunks=num_chunks, **cfg)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/model/moe.py` & `InternEvo-0.4.0.dev20240403/internlm/model/moe/moe.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+from typing import Callable, Optional
+
 import torch
 
-import internlm.moe  # noqa # pylint: disable=W0611
 from internlm.core.context import ParallelMode
 from internlm.core.context import global_context as gpc
-from internlm.model.linear import FeedForward
 from internlm.utils.logger import get_logger
 from internlm.utils.registry import MODEL_INITIALIZER
 
 # global llm logger
 logger = get_logger(__file__)
 
 
@@ -31,51 +31,58 @@
         moe_use_residual (bool, optional): default=False, make this MoE layer a Residual MoE
                                           (https://arxiv.org/abs/2201.05596) layer.
         residual_mlp (torch.nn.Module, optional): default=None, the torch module that defines the residual MLP.
     """
 
     def __init__(
         self,
-        hidden_size,
-        num_experts=1,
-        ep_group=None,
+        in_features: int,
+        hidden_features: int,
+        out_features: int,
+        ep_cls: Optional[Callable],
+        ep_group: Optional[torch.distributed.ProcessGroup],
+        num_experts: int = 1,
         ep_size=1,
+        use_residual: bool = False,
         device=None,
         dtype=None,
     ):
 
         super().__init__()
 
         if not hasattr(gpc.config, "moe"):
             gpc.config.moe = dict()
 
         self.moe_layer = MODEL_INITIALIZER.get_module(module_name=gpc.config.model.moe_type)(
-            hidden_size=hidden_size,
+            in_features=in_features,
+            hidden_features=hidden_features,
+            out_features=out_features,
             num_experts=num_experts,
+            ep_cls=ep_cls,
             ep_group=ep_group,
             ep_size=ep_size,
             device=device,
             dtype=dtype,
             **(gpc.config.moe)
         )
 
         # residual network, see https://arxiv.org/pdf/2201.05596.pdf, seems useful for convergence
-        self.use_residual = gpc.config.model.moe_use_residual
+        self.use_residual = use_residual
         if self.use_residual:
-            self.residual_mlp = FeedForward(
-                hidden_size,
-                int(hidden_size * gpc.config.model.mlp_ratio),
-                out_features=hidden_size,
+            self.residual_mlp = ep_cls(
+                in_features=in_features,
+                hidden_features=hidden_features,
+                out_features=out_features,
                 process_group=gpc.get_group(ParallelMode.TENSOR),
                 bias=False,
                 device=device,
                 dtype=dtype,
             )
             # coefficient is used for weighted sum of the output of expert and residual mlp
-            self.coefficient = torch.nn.Linear(hidden_size, 2)
+            self.coefficient = torch.nn.Linear(in_features, 2)
 
     def forward(self, hidden_states, used_token=None):
         """MoE forward
 
         Arguments:
             hidden_states (Tensor): input to the layer
             used_token (Tensor, optional): default: None, mask only used tokens
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/model/multi_head_attention.py` & `InternEvo-0.4.0.dev20240403/internlm/model/modules/multi_head_attention.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,17 +8,201 @@
 import torch
 import torch.distributed as dist
 import torch.nn.functional as F
 from einops import rearrange, repeat
 from torch import Tensor, nn
 from torch.nn import Module
 
+from internlm.accelerator import AcceleratorType, get_accelerator
 from internlm.core.context import global_context as gpc
-from internlm.model.embedding import DynamicNTKScalingRotaryEmbedding, RotaryEmbedding
-from internlm.model.linear import get_linear_cls
+from internlm.model.modules.embedding import (
+    DynamicNTKScalingRotaryEmbedding,
+    RotaryEmbedding,
+)
+from internlm.model.ops.linear import get_linear_cls
+from internlm.model.utils import pack_output_after_attn, unpack_qkv_before_attn
+from internlm.utils.common import get_current_device
+
+internlm_accelerator = get_accelerator()
+
+try:
+    import torch_npu
+except (ImportError, ModuleNotFoundError):
+    pass
+
+
+def get_gqa_attn_cls(use_flash_attn, tp_mode, causal, softmax_scale, dropout, sequence_process_group):
+    if use_flash_attn:
+        device_backend = internlm_accelerator.get_accelerator_backend()
+        if device_backend == AcceleratorType.GPU:
+            from flash_attn import flash_attn_varlen_kvpacked_func
+            from flash_attn.modules.mha import FlashCrossAttention
+
+            inner_attn, inner_cross_attn_cls = flash_attn_varlen_kvpacked_func, FlashCrossAttention
+        elif device_backend == AcceleratorType.NPU:
+            from internlm.model.modules.multi_head_attention import (
+                AscendFlashSelfAttention,
+            )
+
+            inner_attn_cls, inner_cross_attn_cls = AscendFlashSelfAttention, AscendFlashSelfAttention
+            inner_attn = inner_attn_cls(causal=causal, softmax_scale=softmax_scale, attention_dropout=dropout)
+        elif device_backend == AcceleratorType.DIPU:
+            from deeplink_ext.internlm_ops.mha import (
+                DeepLinkCrossAttention,
+                DeepLinkSelfAttention,
+            )
+
+            inner_attn_cls, inner_cross_attn_cls = DeepLinkSelfAttention, DeepLinkCrossAttention
+            inner_attn = inner_attn_cls(causal=causal, softmax_scale=softmax_scale, attention_dropout=dropout)
+        else:
+            raise NotImplementedError(f"Unsupport device type: {device_backend} for flash attention")
+    else:
+        inner_attn_cls, inner_cross_attn_cls = SelfAttention, CrossAttention
+        inner_attn = inner_attn_cls(causal=causal, softmax_scale=softmax_scale, attention_dropout=dropout)
+
+    inner_cross_attn = inner_cross_attn_cls(causal=causal, softmax_scale=softmax_scale, attention_dropout=dropout)
+
+    if tp_mode == "isp":
+        inner_attn = DistributedAttention(inner_attn, sequence_process_group=sequence_process_group)
+        inner_cross_attn = DistributedAttention(inner_cross_attn, sequence_process_group=sequence_process_group)
+
+    return inner_attn, inner_cross_attn
+
+
+class AscendFlashSelfAttention(torch.nn.Module):
+    """Implement the scaled dot product attention with softmax.
+    Arguments
+    ---------
+        softmax_scale: The temperature to use for the softmax attention.
+                      (default: 1/sqrt(d_keys) where d_keys is computed at
+                      runtime)
+        attention_dropout: The dropout rate to apply to the attention
+                           (default: 0.0)
+    """
+
+    def __init__(
+        self,
+        causal: bool = True,
+        softmax_scale: float = None,
+        attention_dropout: float = 0.0,
+    ):
+        super().__init__()
+        assert rearrange is not None, "Please install einops first, e.g., with pip install einops"
+        self.causal = causal
+        self.softmax_scale = softmax_scale
+        self.shape_order = "BSND"
+        self.dropout_p = attention_dropout
+
+        if self.causal:
+            self.sparse_mode = 0
+            self.next_tockens = 0
+        else:
+            assert False, "Ascend flash attention unsupport causal=False now!"
+
+    def forward(
+        self,
+        qkv=None,
+        q=None,
+        k=None,
+        v=None,
+        kv=None,
+        cu_seqlens_q=None,  # pylint: disable=W0613
+        cu_seqlens_k=None,  # pylint: disable=W0613
+        max_seqlen_q=None,  # pylint: disable=W0613
+        max_seqlen_k=None,  # pylint: disable=W0613
+        dropout_p=0.0,
+        softmax_scale=None,
+        causal=False,
+        window_size=(-1, -1),  # pylint: disable=W0613
+        alibi_slopes=None,  # pylint: disable=W0613
+        deterministic=False,
+        return_attn_probs=False,  # pylint: disable=W0613
+        attention_mask=None,
+    ):
+        if qkv is not None:
+            assert (q, k, v, kv) == (None, None, None, None)
+            q = qkv[:, :, 0]
+            k = qkv[:, :, 1]
+            v = qkv[:, :, 2]
+        else:
+            assert q is not None
+            if kv is not None:
+                assert (k, v) == (None, None)
+                k = kv[:, :, 0]
+                v = kv[:, :, 1]
+            else:
+                assert k is not None and v is not None
+
+        if causal:
+            assert causal == self.causal
+        if dropout_p:
+            assert dropout_p == self.dropout_p
+        if softmax_scale:
+            assert softmax_scale == self.softmax_scale
+
+        return self._forward(q, k, v, deterministic=deterministic, attention_mask=attention_mask)
+
+    def _forward(
+        self,
+        q,
+        k,
+        v,
+        deterministic: bool = False,
+        attention_mask: Tensor = None,
+        actual_seq_qlen: Tensor = None,  # pylint: disable=W0613
+        actual_seq_kvlen: Tensor = None,  # pylint: disable=W0613
+    ):
+        """Implements the multihead softmax attention.
+        Arguments
+        ---------
+            q, k, v: The tensor containing the query, key, and value. (B, S, H, D)
+        """
+        assert q.dtype in (torch.bfloat16, torch.float16)
+
+        if len(q.shape) == 5:
+            q = q.squeeze(dim=2)
+            k = k.squeeze(dim=2)
+            v = v.squeeze(dim=2)
+
+        B, S, N, D = q.shape[0], q.shape[1], q.shape[2], q.shape[3]  # noqa: F841  # pylint: disable=W0612
+
+        if self.shape_order == "BSH":
+            q, k, v = [rearrange(x, "b s h d -> b s (h d)") for x in [q, k, v]]
+        elif self.shape_order == "SBH":
+            q, k, v = [rearrange(x, "b s h d -> s b (h d)") for x in [q, k, v]]
+        elif self.shape_order != "BSND":
+            raise ValueError("Invalid shape-order: {}, shape-order must be SBH or BSH or BSND".format(self.shape_order))
+
+        if attention_mask is None:
+            attention_mask = torch.triu(torch.ones(S, S, device=get_current_device()), 1).bool()
+
+        output = torch_npu.npu_fusion_attention(
+            query=q,
+            key=k,
+            value=v,
+            head_num=N,
+            input_layout="BSND",
+            pse=None,
+            atten_mask=attention_mask,
+            scale=self.softmax_scale,
+            sparse_mode=self.sparse_mode,
+            pre_tockens=k.shape[1],  # Used for sparse calculations, representing the left boundary of the slides window
+            next_tockens=self.next_tockens,
+            keep_prob=1 - self.dropout_p,
+            inner_precise=0 if not deterministic else 2,
+        )[0]
+
+        if self.shape_order == "BSH":
+            output = rearrange(output, "b s (h d) -> b s h d", h=N)
+        elif self.shape_order == "SBH":
+            output = rearrange(output, "s b (h d) -> b s h d", h=N)
+        elif self.shape_order != "BSND":
+            raise ValueError("Invalid shape-order: {}, shape-order must be SBH or BSH or BSND".format(self.shape_order))
+
+        return output
 
 
 # adpated from https://github.com/microsoft/DeepSpeed/blob/master/deepspeed/sequence/layer.py
 class _SeqAllToAll(torch.autograd.Function):
     "sequence alltoall"
 
     @staticmethod
@@ -76,15 +260,15 @@
         self._scatter_gather_idx["kv"] = [2, 0]  # kv shape: [sequence, 2, head, head_dim]
         self._scatter_gather_idx["q"] = [1, 0]  # q/k/v shape: [sequence, head, head_dim]
         self._scatter_gather_idx["output"] = [0, 1]  # output shape: [sequence, head, head_dim]
 
     def forward(
         self, qkv: Tensor = None, kv: Tensor = None, q: Tensor = None, k: Tensor = None, v: Tensor = None, **kwargs: Any
     ) -> Tensor:
-        if gpc.is_evaluating is True:
+        if gpc.is_evaluating is True or gpc.config.data.use_packed_dataset is False:
             # when conducting evaluation, the scatter and gather index should add 1.
             eval_scatter_gather_idx = {key: [x + 1 for x in value] for key, value in self._scatter_gather_idx.items()}
             return self._forward(qkv=qkv, kv=kv, q=q, k=k, v=v, scatter_gather=eval_scatter_gather_idx, **kwargs)
         else:
             return self._forward(qkv=qkv, kv=kv, q=q, k=k, v=v, scatter_gather=self._scatter_gather_idx, **kwargs)
 
     def _forward(
@@ -109,24 +293,24 @@
 
         Returns:
             * output (Tensor): context output
         """
 
         if qkv is not None:
             qkv = _SeqAllToAll.apply(self.spg, qkv, scatter_gather["qkv"][0], scatter_gather["qkv"][1])
-            context_layer = self.local_attn(qkv, **kwargs)
+            context_layer = self.local_attn(qkv=qkv, **kwargs)
         elif kv is not None:
             q = _SeqAllToAll.apply(self.spg, q, scatter_gather["q"][0], scatter_gather["q"][1])
             kv = _SeqAllToAll.apply(self.spg, kv, scatter_gather["kv"][0], scatter_gather["kv"][1])
-            context_layer = self.local_attn(q, kv, **kwargs)
+            context_layer = self.local_attn(q=q, kv=kv, **kwargs)
         else:
             q = _SeqAllToAll.apply(self.spg, q, scatter_gather["q"][0], scatter_gather["q"][1])
             k = _SeqAllToAll.apply(self.spg, k, scatter_gather["q"][0], scatter_gather["q"][1])
             v = _SeqAllToAll.apply(self.spg, v, scatter_gather["q"][0], scatter_gather["q"][1])
-            context_layer = self.local_attn(q, k, v, **kwargs)
+            context_layer = self.local_attn(q=q, k=k, v=v, **kwargs)
         output = _SeqAllToAll.apply(self.spg, context_layer, scatter_gather["output"][0], scatter_gather["output"][1])
 
         # out e.g., [s/p::h]
         return output
 
 
 class SelfAttention(nn.Module):
@@ -369,21 +553,35 @@
             process_group,
             bias=True,
             sequence_parallel=gpc.config.parallel.sequence_parallel,
             **factory_kwargs,
         )  # according to https://spaces.ac.cn/archives/9577
 
         if gpc.config.model.use_flash_attn:
-            from flash_attn.modules.mha import FlashCrossAttention, FlashSelfAttention
+            if internlm_accelerator.get_accelerator_backend() == AcceleratorType.GPU:
+                from flash_attn.modules.mha import (
+                    FlashCrossAttention,
+                    FlashSelfAttention,
+                )
+            elif internlm_accelerator.get_accelerator_backend() == AcceleratorType.NPU:
+                FlashCrossAttention, FlashSelfAttention = AscendFlashSelfAttention, AscendFlashSelfAttention
+            elif internlm_accelerator.get_accelerator_backend() == AcceleratorType.DIPU:
+                from deeplink_ext.internlm_ops.mha import (
+                    DeepLinkCrossAttention,
+                    DeepLinkSelfAttention,
+                )
+
+                FlashCrossAttention, FlashSelfAttention = DeepLinkCrossAttention, DeepLinkSelfAttention
 
             inner_attn_cls = FlashSelfAttention
             inner_cross_attn_cls = FlashCrossAttention
         else:
             inner_attn_cls = SelfAttention
             inner_cross_attn_cls = CrossAttention
+
         self.inner_attn = inner_attn_cls(causal=causal, softmax_scale=softmax_scale, attention_dropout=dropout)
         self.inner_cross_attn = inner_cross_attn_cls(
             causal=causal, softmax_scale=softmax_scale, attention_dropout=dropout
         )
         if self.tp_mode == "isp":
             self.inner_attn = DistributedAttention(self.inner_attn, sequence_process_group=sequence_process_group)
             self.inner_cross_attn = DistributedAttention(
@@ -422,20 +620,20 @@
         else:
             qkv = rearrange(qkv, "(b s) (three h d) -> b s three h d", s=seqlen, three=3, d=self.head_dim)
 
         if inference_params is None:
             kwargs["inference_params"] = inference_params
             qkv = self.rotary_emb(qkv, **kwargs)
             if gpc.config.model.dtype is torch.float32 and gpc.config.model.use_flash_attn:
-                with torch.cuda.amp.autocast(dtype=torch.bfloat16):
+                with internlm_accelerator.amp.autocast(dtype=torch.bfloat16):
                     if qkv.dtype not in [torch.float16, torch.bfloat16]:
                         qkv = qkv.to(torch.bfloat16)
-                    context = self.inner_attn(qkv).to(x.dtype)
+                    context = self.inner_attn(qkv=qkv).to(x.dtype)
             else:
-                context = self.inner_attn(qkv)
+                context = self.inner_attn(qkv=qkv)
 
         else:
             if self.use_dynamic_ntk_rope:
                 q = qkv[:, :, 0]
                 assert self.layer_idx is not None, "Generation requires layer_idx in the constructor"
                 kv = _update_kv_cache(qkv[:, :, 1:], inference_params, self.layer_idx)
                 if inference_params.sequence_len_offset != 0:
@@ -547,21 +745,21 @@
                     max_seqlen_k = attn_mask4flsh.shape[-1]
                     total_q = q.masked_select(attn_mask4flsh.view(bsz, -1, 1, 1)).view(-1, q.shape[-2], q.shape[-1])
                     total_kv = kv.masked_select(attn_mask4flsh.view(bsz, -1, 1, 1, 1)).view(
                         -1, kv.shape[-3], kv.shape[-2], kv.shape[-1]
                     )
 
                     if gpc.config.model.dtype is torch.float32 and gpc.config.model.use_flash_attn:
-                        with torch.cuda.amp.autocast(dtype=torch.bfloat16):
+                        with internlm_accelerator.amp.autocast(dtype=torch.bfloat16):
                             if total_q.dtype not in [torch.float16, torch.bfloat16]:
                                 total_q = total_q.to(torch.bfloat16)
                             if total_kv.dtype not in [torch.float16, torch.bfloat16]:
                                 total_kv = total_kv.to(torch.bfloat16)
 
-                    if gpc.config.model.use_flash_attn:
+                    if gpc.config.use_cuda_flash_attn:
                         try:
                             from flash_attn.flash_attn_interface import (
                                 flash_attn_unpadded_func,
                             )
                         except ImportError:
                             try:
                                 from flash_attn.flash_attn_interface import (
@@ -629,27 +827,46 @@
         """
         Arguments:
             x: (batch, seqlen, hidden_dim) (where hidden_dim = num heads * head dim) if seqlen=None.
                 If seqlen is not None, x is (batch * seqlen, hidden_dim). This is so that when we
                 split x during sequence parallel, we split the batch * seqlen dimension
                 (in case batch is small).
         """
-        qkv = self.Wqkv(x)  # total x hsz'
-        qkv = rearrange(qkv, "t (three h d) -> t three h d", three=3, d=self.head_dim)  # total x 3 x n_head x d
+        qkv = self.Wqkv(x)  # bsz x total x hsz
+        qkv = rearrange(
+            qkv, "b t (three h d) -> b t three h d", three=3, d=self.head_dim
+        )  # bsz x total x 3 x n_head x d
         qkv = self.rotary_emb(qkv, **kwargs)
+
         kwargs.pop("indexes")
+
+        # for packed data, batch dimension with a size of 1 should be directly squeezed off.
+        if internlm_accelerator.get_accelerator_backend() == AcceleratorType.GPU:
+            qkv = qkv.squeeze(0)
+        # since torch_npu only supports fa with no packed data currently, qkv should be unpacked
+        elif internlm_accelerator.get_accelerator_backend() in [AcceleratorType.NPU, AcceleratorType.DIPU]:
+            qkv = unpack_qkv_before_attn(qkv, kwargs["cu_seqlens"])
+            kwargs.pop("cu_seqlens")
+            kwargs.pop("max_seqlen")
+
         if inference_params is None:
             if gpc.config.model.dtype is torch.float32 and gpc.config.model.use_flash_attn:
-                with torch.cuda.amp.autocast(dtype=torch.bfloat16):
+                with internlm_accelerator.amp.autocast(dtype=torch.bfloat16):
                     if qkv.dtype not in [torch.float16, torch.bfloat16]:
                         qkv = qkv.to(torch.bfloat16)
-                    context = self.inner_attn(qkv, **kwargs).to(x.dtype)
+                    context = self.inner_attn(qkv=qkv, **kwargs).to(x.dtype)
             else:
-                context = self.inner_attn(qkv, **kwargs)
+                context = self.inner_attn(qkv=qkv, **kwargs)
 
         else:
             raise RuntimeError("Not support this right now")
 
-        context = rearrange(context, "b h d -> b (h d)")  # recover the shape
+        if internlm_accelerator.get_accelerator_backend() == AcceleratorType.GPU:
+            context = rearrange(context, "s h d -> s (h d)")  # recover the shape
+            context = context.unsqueeze(0)  # restore bsz dimension
+        elif internlm_accelerator.get_accelerator_backend() in [AcceleratorType.NPU, AcceleratorType.DIPU]:
+            context = rearrange(context, "b s h d -> b s (h d)")  # recover the shape
+            context = pack_output_after_attn(context, kwargs["cu_seqlens"])
+
         out = self.out_proj(context)
 
         return out
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/model/norm.py` & `InternEvo-0.4.0.dev20240403/internlm/model/ops/norm.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.3.3.dev20240315/internlm/model/utils.py` & `InternEvo-0.4.0.dev20240403/internlm/model/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,43 +3,56 @@
 
 from typing import Callable, Optional
 
 import torch
 import torch.distributed as dist
 import torch.nn.functional as F
 from torch import Tensor
-from torch.cuda.amp import custom_bwd, custom_fwd
 from torch.distributed import ProcessGroup
+from torch.nn.utils.rnn import pad_sequence
 
+from internlm.accelerator import AcceleratorType, get_accelerator
 from internlm.core.context import global_context as gpc
 from internlm.utils.logger import get_logger
 
+try:
+    import fused_dense_lib as fused_dense_cuda
+except (ModuleNotFoundError, ImportError):
+    print("Import fused_dense_lib failed!")
+
+internlm_accelerator = get_accelerator()
+
+custom_bwd = internlm_accelerator.return_custom_bwd()
+custom_fwd = internlm_accelerator.return_custom_fwd()
+
 logger = get_logger(__file__)
 
 
 # Raw operation, does not support autograd, but does support async
 def all_reduce_raw(input_: Tensor, process_group: ProcessGroup, async_op: bool = False):
     input_ = input_.contiguous()
     handle = torch.distributed.all_reduce(input_, group=process_group, async_op=async_op)
     return input_, handle
 
 
 class ReduceScatterFunc(torch.autograd.Function):
     """Reduce scatter the input from the sequence parallel region and concatenate."""
 
     @staticmethod
-    def forward(ctx, input_: Tensor, process_group: ProcessGroup) -> Tensor:
+    def forward(ctx, input_: Tensor, process_group: ProcessGroup, reduce_dim: int = 0) -> Tensor:
         ctx.process_group = process_group
-        output, _ = reduce_scatter_raw(input_, process_group)
+        ctx.reduce_dim = reduce_dim
+        output, _ = reduce_scatter_raw(input_, process_group, reduce_dim=reduce_dim)
         return output
 
     @staticmethod
     def backward(ctx, grad_output: Tensor):
-        grad_input, _ = all_gather_raw(grad_output, ctx.process_group)
-        return grad_input, None
+        gather_dim = ctx.reduce_dim
+        grad_input, _ = all_gather_raw(grad_output, ctx.process_group, gather_dim=gather_dim)
+        return grad_input, None, None
 
 
 # Supports autograd, but does not support async
 reduce_scatter = ReduceScatterFunc.apply
 
 
 class AllReduceFunc(torch.autograd.Function):
@@ -181,29 +194,31 @@
 
 
 def reduce_scatter_raw(
     input_: Tensor,
     process_group: ProcessGroup,
     op=dist.ReduceOp.SUM,
     async_op: bool = False,
+    reduce_dim: int = 0,
     memory_pool_allocator: Callable = None,
 ):
     world_size = dist.get_world_size(process_group)
-    assert input_.shape[0] % world_size == 0
+    assert input_.shape[reduce_dim] % world_size == 0
 
     if world_size <= 1:
         return input_, None
 
+    shape_list = list(input_.shape)
+    shape_list[reduce_dim] = shape_list[reduce_dim] // world_size
+
     if memory_pool_allocator is not None:
-        size = (input_.shape[0] // world_size, *input_.shape[1:])
-        output = memory_pool_allocator(size)
+        output = memory_pool_allocator(tuple(shape_list))
     else:
         output = torch.empty(
-            input_.shape[0] // world_size,
-            *input_.shape[1:],
+            shape_list,
             dtype=input_.dtype,
             device=input_.device,
         ).contiguous()
 
     handle = dist.reduce_scatter_tensor(output, input_.contiguous(), op=op, group=process_group, async_op=async_op)
     return output, handle
 
@@ -277,18 +292,16 @@
         if ctx.return_residual:
             (grad_input,) = args
             grad_input = grad_input.contiguous()
         process_group = ctx.process_group
         sequence_parallel = ctx.sequence_parallel
         gather_dim = ctx.gather_dim
 
-        if gpc.config.model.use_flash_attn:
-            import fused_dense_lib as fused_dense_cuda
-
-        if gpc.config.model.use_flash_attn and ctx.is_using_cuda:
+        if gpc.config.use_cuda_flash_attn and AcceleratorType.GPU == get_accelerator().get_accelerator_backend():
+            assert ctx.is_using_cuda, "CUDA Flash Attention only support GPU device"
             backward_func = fused_dense_cuda.linear_bias_wgrad
         else:
             backward_func = linear_bias_wgrad_torch
 
         if ctx.compute_weight_gradient:
             x, weight = ctx.saved_tensors
             if process_group is not None and sequence_parallel:
@@ -308,16 +321,20 @@
                 grad_input = torch.addmm(
                     grad_input.reshape(batch_dim, grad_input.shape[-1]),
                     grad_output,
                     weight,
                 )
             grad_input = grad_input.reshape(*batch_shape, grad_input.shape[-1])
             if process_group is not None:
-                reduce_fn = reduce_scatter_raw if sequence_parallel else all_reduce_raw
-                grad_input, handle_grad_input = reduce_fn(grad_input, process_group, async_op=True)
+                if sequence_parallel:
+                    grad_input, handle_grad_input = reduce_scatter_raw(
+                        grad_input, process_group, async_op=True, reduce_dim=1
+                    )
+                else:
+                    grad_input, handle_grad_input = all_reduce_raw(grad_input, process_group, async_op=True)
         else:
             grad_input = None
         if ctx.needs_input_grad[1]:
             assert ctx.compute_weight_gradient
             if process_group is not None and sequence_parallel and handle_x is not None:
                 handle_x.wait()
             grad_weight, grad_bias = backward_func(
@@ -396,18 +413,16 @@
         grad_output = grad_output.contiguous()
         if ctx.return_residual:
             (grad_input,) = args
             grad_input = grad_input.contiguous()
         process_group = ctx.process_group
         sequence_parallel = ctx.sequence_parallel
 
-        if gpc.config.model.use_flash_attn:
-            import fused_dense_lib as fused_dense_cuda
-
-        if gpc.config.model.use_flash_attn and ctx.is_using_cuda:
+        if gpc.config.use_cuda_flash_attn and AcceleratorType.GPU == get_accelerator().get_accelerator_backend():
+            assert ctx.is_using_cuda, "CUDA Flash Attention only support GPU device"
             backward_func = fused_dense_cuda.linear_bias_wgrad
         else:
             backward_func = linear_bias_wgrad_torch
 
         if ctx.compute_weight_gradient:
             total_x, weight = ctx.saved_tensors
         else:
@@ -423,16 +438,20 @@
                 grad_input = torch.addmm(
                     grad_input.reshape(batch_dim, grad_input.shape[-1]),
                     grad_output,
                     weight,
                 )
             grad_input = grad_input.reshape(*batch_shape, grad_input.shape[-1])
             if process_group is not None:
-                reduce_fn = reduce_scatter_raw if sequence_parallel else all_reduce_raw
-                grad_input, handle_grad_input = reduce_fn(grad_input, process_group, async_op=True)
+                if sequence_parallel:
+                    grad_input, handle_grad_input = reduce_scatter_raw(
+                        grad_input, process_group, async_op=True, reduce_dim=1
+                    )
+                else:
+                    grad_input, handle_grad_input = all_reduce_raw(grad_input, process_group, async_op=True)
         else:
             grad_input = None
         if ctx.needs_input_grad[1]:
             assert ctx.compute_weight_gradient
             grad_weight, grad_bias = backward_func(
                 total_x.reshape(batch_dim, total_x.shape[-1]),
                 grad_output,
@@ -499,18 +518,16 @@
 
     @staticmethod
     @custom_bwd
     def backward(ctx, grad_output, *args):
         module = ctx.module
         communicator = ctx.communicator
 
-        if gpc.config.model.use_flash_attn:
-            import fused_dense_lib as fused_dense_cuda
-
-        if gpc.config.model.use_flash_attn and ctx.is_using_cuda:
+        if gpc.config.use_cuda_flash_attn and AcceleratorType.GPU == get_accelerator().get_accelerator_backend():
+            assert ctx.is_using_cuda, "CUDA Flash Attention only support GPU device"
             backward_func = fused_dense_cuda.linear_bias_wgrad
         else:
             backward_func = linear_bias_wgrad_torch
 
         grad_output = grad_output.contiguous()
         if ctx.return_residual:
             (grad_input,) = args
@@ -577,15 +594,17 @@
     process_group: Optional[ProcessGroup] = None,
     sequence_parallel: bool = True,
     gather_dim: int = 0,
 ):
     dtype_eligible = x.dtype in [torch.float16, torch.bfloat16] or (
         x.dtype == torch.float32 and torch.is_autocast_enabled()
     )
-    is_using_cuda = x.is_cuda and weight.is_cuda and (bias is None or bias.is_cuda) and dtype_eligible
+    is_using_cuda = (
+        internlm_accelerator.get_accelerator_backend() in [AcceleratorType.GPU, AcceleratorType.DIPU]
+    ) and dtype_eligible
     return FusedDenseFunc.apply(
         x,
         weight,
         bias,
         return_residual,
         process_group,
         sequence_parallel,
@@ -602,15 +621,17 @@
     process_group: Optional[ProcessGroup] = None,
     sequence_parallel: bool = True,
     gather_dim: int = 0,
 ):
     dtype_eligible = x.dtype in [torch.float16, torch.bfloat16] or (
         x.dtype == torch.float32 and torch.is_autocast_enabled()
     )
-    is_using_cuda = x.is_cuda and weight.is_cuda and (bias is None or bias.is_cuda) and dtype_eligible
+    is_using_cuda = (
+        internlm_accelerator.get_accelerator_backend() in [AcceleratorType.GPU, AcceleratorType.DIPU]
+    ) and dtype_eligible
     return MegatronFusedDenseFunc.apply(
         x,
         weight,
         bias,
         return_residual,
         process_group,
         sequence_parallel,
@@ -626,15 +647,17 @@
     communicator,
     bias: Optional[Tensor] = None,
     return_residual: bool = False,
 ):
     dtype_eligible = x.dtype in [torch.float16, torch.bfloat16] or (
         x.dtype == torch.float32 and torch.is_autocast_enabled()
     )
-    is_using_cuda = x.is_cuda and weight.is_cuda and (bias is None or bias.is_cuda) and dtype_eligible
+    is_using_cuda = (
+        internlm_accelerator.get_accelerator_backend() in [AcceleratorType.GPU, AcceleratorType.DIPU]
+    ) and dtype_eligible
     return ISPFusedDenseFunc.apply(
         x,
         weight,
         bias,
         module,
         communicator,
         return_residual,
@@ -644,20 +667,28 @@
 
 def try_import_RMSNorm():
     """
     Try import MixFusedRMSNorm from apex, if failed, return our RMSNorm
 
     """
     try:
-        from apex.normalization.fused_layer_norm import MixedFusedRMSNorm as RMSNorm
+        device_backend = internlm_accelerator.get_accelerator_backend()
+        if device_backend == AcceleratorType.DIPU:
+            from deeplink_ext.internlm_ops.rms_norm import (
+                DeepLinkRMSNormWithNormalizedShape as RMSNorm,
+            )
 
-        return RMSNorm
-    except ModuleNotFoundError:
+            return RMSNorm
+        else:
+            from apex.normalization.fused_layer_norm import MixedFusedRMSNorm as RMSNorm
+
+            return RMSNorm
+    except (ModuleNotFoundError, ImportError):
         logger.warning("The torch implementation for MixFusedRMSNorm is slower than apex. Please note this!")
-        from internlm.model.norm import RMSNormTorch as RMSNorm
+        from internlm.model.ops.norm import RMSNormTorch as RMSNorm
 
         return RMSNorm
 
 
 def is_moe_param(param: torch.Tensor) -> bool:
     if hasattr(param, "is_expert") and param.is_expert:
         return True
@@ -665,7 +696,56 @@
 
 
 def Silu(w1_o, w2_o):
     return F.silu(w1_o) * w2_o
 
 
 Silu = torch.jit.script(Silu)
+
+
+def unpack_qkv_before_attn(cur_input=None, cu_seqlens=None, padding_v: int = 0):
+    """
+    qkv: the shape is (1, packed_length, three, head_num, head_dim)
+    kv: the shape is (1, packed_length, two, head_num, head_dim)
+    q/k/v: the shape is (1, packed_length, head_num, head_dim)
+
+    Return:
+    output: the shape is (micro_bsz, seq_len, three, head_num, head_dim) for qkv
+                        (micro_bsz, seq_len, two, head_num, head_dim) for kv
+                        (micro_bsz, seq_len, head_num, head_dim) for q/k/v
+    """
+    if cu_seqlens is None or cur_input is None:
+        raise ValueError("cu_seqlens and cur_input must be provided.")
+
+    assert cur_input.shape[0] == 1
+    cur_input = cur_input.squeeze(0)
+
+    sequences = []
+    for i in range(len(cu_seqlens) - 1):
+        sequences.append(cur_input[cu_seqlens[i] : cu_seqlens[i + 1]])
+
+    padded_sequences = pad_sequence(sequences, batch_first=True, padding_value=padding_v)
+
+    return padded_sequences
+
+
+def pack_output_after_attn(cur_input=None, cu_seqlens=None, padding_v: int = 0):
+    """
+    cur_input: the shape is (micro_bsz, seq_len, hidden_size)
+
+    Return:
+    output: the shape is (1, packed_length, hidden_size)
+    """
+    if cu_seqlens is None or cur_input is None:
+        raise ValueError("cu_seqlens and cur_input must be provided.")
+
+    packed_len_ = gpc.config.data.micro_bsz * gpc.config.data.seq_len
+    output_shape = list(cur_input.shape)
+    output_shape[0] = 1
+    output_shape[1] = packed_len_
+
+    output = torch.full(output_shape, fill_value=padding_v, device=cur_input.device, dtype=cur_input.dtype)
+    for i in range(len(cu_seqlens) - 1):
+        length = cu_seqlens[i + 1] - cu_seqlens[i]
+        output[0, cu_seqlens[i] : cu_seqlens[i + 1]] = cur_input[i, 0:length]
+
+    return output
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/moe/__init__.py` & `InternEvo-0.4.0.dev20240403/internlm/model/moe/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-from .gshard_moe import GShardMOELayer
+from .gshard_layer import GShardMOELayer
+from .moe import MoE
+
+__all__ = ["MoE", "GShardMOELayer"]
 
-__all__ = ["GShardMOELayer"]
 
 try:
     from megablocks import ops  # noqa # pylint: disable=W0611
 except ModuleNotFoundError:
     pass
 else:
-    from internlm.moe.megablock.megablock_moe import (  # noqa # pylint: disable=W0611
+    from internlm.model.moe.megablock.megablock_moe import (  # noqa # pylint: disable=W0611
         MegaBlockMoE,
     )
 
     __all__ += "MegaBlockMoE"
 
 try:
     import stk  # noqa # pylint: disable=W0611
     from megablocks import ops  # noqa # pylint: disable=W0611
 except ModuleNotFoundError:
     pass
 else:
-    from internlm.moe.megablock.megablock_dmoe import (  # noqa # pylint: disable=W0611
+    from internlm.model.moe.megablock.megablock_dmoe import (  # noqa # pylint: disable=W0611
         MegaBlockdMoE,
     )
 
     __all__ += "MegaBlockdMoE"
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/moe/base_moe.py` & `InternEvo-0.4.0.dev20240403/internlm/model/moe/base_layer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from typing import TYPE_CHECKING, Union
 
 import torch
 from torch import Tensor
 from torch.nn import Module, ModuleList
 
 from internlm.core.context import global_context as gpc
-from internlm.moe.experts import Experts
+from internlm.model.moe.experts import Experts
+from internlm.utils.common import get_current_device
 
 if TYPE_CHECKING:
     Base = Module[Tensor]
 else:
     Base = Module
 
 
@@ -27,9 +28,9 @@
         if expert_group_name not in gpc.expert_parallel_group_names:
             gpc.expert_parallel_group_names.append(expert_group_name)
         self.gate = gate
         self.experts = Experts(experts, num_local_experts, expert_group_name)
         self.ep_group = ep_group
         self.ep_size = ep_size
         self.num_local_experts = num_local_experts
-        self.l_aux = torch.tensor(0.0, device=torch.cuda.current_device(), dtype=gpc.config.model.get("dtype"))
+        self.l_aux = torch.tensor(0.0, device=get_current_device(), dtype=gpc.config.model.get("dtype"))
         self.exp_counts = None
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/moe/experts.py` & `InternEvo-0.4.0.dev20240403/internlm/model/moe/experts.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.3.3.dev20240315/internlm/moe/gshard_moe.py` & `InternEvo-0.4.0.dev20240403/internlm/model/moe/gshard_layer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """
 The file has been adapted from the following files:
 https://github.com/microsoft/DeepSpeed/blob/master/deepspeed/moe/experts.py
  Git commit hash: f3943cf9109226ed3ecf2d5dbb639a11cd925555
  We retain the following license from the original files:
 """
+
 from typing import Callable, Dict, Optional, Tuple
 
 import torch
 import torch.distributed as dist
 import torch.nn.functional as F
 from torch import Tensor
 from torch.nn import Module
 
 from internlm.core.context import ParallelMode
 from internlm.core.context import global_context as gpc
-from internlm.model.linear import FeedForward
 from internlm.utils.logger import get_logger
 from internlm.utils.megatron_timers import megatron_timer as timer
 from internlm.utils.registry import MODEL_INITIALIZER
 
-from .base_moe import BaseMoELayer
+from .base_layer import BaseMoELayer
 from .utils import all_to_all
 
 # global llm logger
 logger = get_logger(__file__)
 
 uniform_map: Dict[torch.device, Callable] = {}
 gumbel_map: Dict[torch.device, Callable] = {}
@@ -381,16 +381,19 @@
             gate network
         expert (torch.nn.Module):
             expert network
     """
 
     def __init__(
         self,
-        hidden_size: int,
+        in_features: int,
+        hidden_features: int,
+        out_features: int,
         num_experts: int,
+        ep_cls: Optional[Callable],
         ep_group: Optional[torch.distributed.ProcessGroup],
         ep_size: int,
         top_k: int = 1,
         capacity_factor: float = 1.0,
         eval_capacity_factor: float = 1.0,
         min_capacity: int = 4,
         noisy_gate_policy: str = None,
@@ -403,30 +406,30 @@
             "Unsupported noisy_gate_policy: " + noisy_gate_policy
         )
         assert (
             num_experts % ep_size == 0
         ), f"Number of experts ({num_experts}) should be divisible by expert parallel size ({ep_size})"
         super().__init__(
             TopKGate(
-                hidden_size,
+                in_features,
                 num_experts,
                 top_k,
                 capacity_factor,
                 eval_capacity_factor,
                 min_capacity,
                 noisy_gate_policy,
                 drop_tokens,
                 use_rts,
             ),
             torch.nn.ModuleList(
                 [
-                    FeedForward(
-                        hidden_size,
-                        int(hidden_size * gpc.config.model.mlp_ratio),
-                        out_features=hidden_size,
+                    ep_cls(
+                        in_features,
+                        hidden_features,
+                        out_features,
                         process_group=gpc.get_group(ParallelMode.TENSOR),
                         bias=False,
                         device=device,
                         dtype=dtype,
                     )
                     for _ in range(num_experts // ep_size)
                 ]
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/moe/megablock/megablock_dmoe.py` & `InternEvo-0.4.0.dev20240403/internlm/model/moe/megablock/megablock_dmoe.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import numpy as np
 import stk
 import torch
 from megablocks import ops
 
 from internlm.core.context import ParallelMode
 from internlm.core.context import global_context as gpc
-from internlm.moe.base_moe import BaseMoELayer
-from internlm.moe.megablock.megablock_moe import MegaBlockMoE
-from internlm.moe.megablock.mlp import MegaBlockGroupedFeedForward
-from internlm.moe.megablock.utils import promote_scalar
+from internlm.model.moe.base_layer import BaseMoELayer
+from internlm.model.moe.megablock.megablock_moe import MegaBlockMoE
+from internlm.model.moe.megablock.mlp import MegaBlockGroupedFeedForward
+from internlm.model.moe.megablock.utils import promote_scalar
 from internlm.utils.registry import MODEL_INITIALIZER
 
 
 @MODEL_INITIALIZER.register_module(module_name="MegaBlock-D")
 class MegaBlockdMoE(MegaBlockMoE):
     """
     Built on the paper and library Megablocks as described in
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/moe/megablock/megablock_moe.py` & `InternEvo-0.4.0.dev20240403/internlm/model/moe/megablock/megablock_moe.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import numpy as np
 import torch
 import torch.nn.functional as F
 from megablocks import ops
 
 from internlm.core.context import ParallelMode
 from internlm.core.context import global_context as gpc
-from internlm.moe.base_moe import BaseMoELayer
-from internlm.moe.megablock.mlp import MegaBlockFeedForward
-from internlm.moe.utils import all_to_all
+from internlm.model.moe.base_layer import BaseMoELayer
+from internlm.model.moe.megablock.mlp import MegaBlockFeedForward
+from internlm.model.moe.utils import all_to_all
 from internlm.utils.registry import MODEL_INITIALIZER
 
 
 @MODEL_INITIALIZER.register_module(module_name="MegaBlock")
 class MegaBlockMoE(BaseMoELayer):
     """
     Built on the paper and library Megablocks as described in
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/moe/megablock/mlp.py` & `InternEvo-0.4.0.dev20240403/internlm/model/moe/megablock/mlp.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import torch
 from torch import nn
 
 from internlm.core.context import ParallelMode
 from internlm.core.context import global_context as gpc
+from internlm.model.moe.megablock.utils import (
+    act_fn,
+    dsd_nn,
+    sdd_nt,
+    tensor_parallel_bmm,
+)
 from internlm.model.utils import Silu
-from internlm.moe.megablock.utils import act_fn, dsd_nn, sdd_nt, tensor_parallel_bmm
 
 
 class MegaBlockFeedForward(nn.Module):
     """
     Feed forward using megablock kernel
     """
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/moe/megablock/utils.py` & `InternEvo-0.4.0.dev20240403/internlm/model/moe/megablock/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 import sys
 
 import torch
 
+from internlm.accelerator import get_accelerator
 from internlm.model.utils import Silu
 
 try:
     import stk
 except ImportError:
     pass
 
+internlm_accelerator = get_accelerator()
+
 
 class TensorParallelBmm(torch.autograd.Function):
     """
     Tensor parallel sdd
     """
 
     @staticmethod
-    @torch.cuda.amp.custom_fwd
+    @internlm_accelerator.amp.custom_fwd
     def forward(ctx, x, w, group=None):
         # [m, k] x [n, k] = [m, n]
         if not x.is_contiguous() or not w.is_contiguous():
             raise ValueError("Expected contiguous 'x' and 'w'.")
 
         ctx.group = group
         ctx.save_for_backward(
             x,
             w,
         )
 
         return torch.bmm(x, w)
 
     @staticmethod
-    @torch.cuda.amp.custom_bwd
+    @internlm_accelerator.amp.custom_bwd
     def backward(ctx, grad):
         x, w = ctx.saved_tensors[:2]
 
         dx = None
         if ctx.needs_input_grad[0]:
             dx = torch.bmm(grad, w.transpose(-2, -1))
         if ctx.group is not None:
@@ -115,15 +118,15 @@
 
 class WeightParallelSddNt(torch.autograd.Function):
     """
     Weight parallel sdd
     """
 
     @staticmethod
-    @torch.cuda.amp.custom_fwd
+    @internlm_accelerator.amp.custom_fwd
     def forward(ctx, x, w, topo, group):
         # [m, k] x [n, k] = [m, n]
         if not x.is_contiguous() or not w.is_contiguous():
             raise ValueError("Expected contiguous 'x' and 'w'.")
 
         ctx.group = group
         ctx.shape = topo.shape
@@ -139,15 +142,15 @@
         )
 
         # TODO(tgale): Support prefetching forward weights.
         parallel_w, _ = _gather_weights(w, group)
         return stk.ops.sdd(x, parallel_w.t(), topo).data
 
     @staticmethod
-    @torch.cuda.amp.custom_bwd
+    @internlm_accelerator.amp.custom_bwd
     def backward(ctx, grad):
         x, w = ctx.saved_tensors[:2]
         grad = stk.Matrix(ctx.shape, grad, *ctx.saved_tensors[2:])
 
         # Start the weight gather asynchronously to overlap with the
         # weight gradient computation.
         parallel_w, handle = _gather_weights(w, ctx.group, async_op=True)
@@ -172,15 +175,15 @@
 
 class WeightParallelDsdNn(torch.autograd.Function):
     """
     Weight parallel dsd
     """
 
     @staticmethod
-    @torch.cuda.amp.custom_fwd
+    @internlm_accelerator.amp.custom_fwd
     def forward(
         ctx, shape, data, row_indices, column_indices, offsets, column_indices_t, offsets_t, block_offsets_t, w, group
     ):
         # [m, k] x [k, n] = [m, n]
         if not data.is_contiguous() or not w.is_contiguous():
             raise ValueError("Expected contiguous 'data' and 'w'.")
 
@@ -192,15 +195,15 @@
         x = stk.Matrix(shape, data, row_indices, column_indices, offsets, column_indices_t, offsets_t, block_offsets_t)
 
         # TODO(tgale): Support prefetching forward weights.
         parallel_w, _ = _gather_weights(w, group)
         return stk.ops.dsd(x, parallel_w)
 
     @staticmethod
-    @torch.cuda.amp.custom_bwd
+    @internlm_accelerator.amp.custom_bwd
     def backward(ctx, grad):
         x = stk.Matrix(ctx.shape, *ctx.saved_tensors[:-1])
         w = ctx.saved_tensors[-1]
 
         # Start the weight gather asynchronously to overlap with the
         # weight gradient computation.
         parallel_w, handle = _gather_weights(w, ctx.group, async_op=True)
@@ -225,15 +228,15 @@
 
 class TensorParallelSddNt(torch.autograd.Function):
     """
     Tensor parallel sdd
     """
 
     @staticmethod
-    @torch.cuda.amp.custom_fwd
+    @internlm_accelerator.amp.custom_fwd
     def forward(ctx, x, w, topo, group):
         # [m, k] x [n, k] = [m, n]
         if not x.is_contiguous() or not w.is_contiguous():
             raise ValueError("Expected contiguous 'x' and 'w'.")
 
         ctx.group = group
         ctx.shape = topo.shape
@@ -247,15 +250,15 @@
             topo.offsets_t,
             topo.block_offsets_t,
         )
 
         return stk.ops.sdd(x, w.t(), topo).data
 
     @staticmethod
-    @torch.cuda.amp.custom_bwd
+    @internlm_accelerator.amp.custom_bwd
     def backward(ctx, grad):
         x, w = ctx.saved_tensors[:2]
         grad = stk.Matrix(ctx.shape, grad, *ctx.saved_tensors[2:])
 
         dw = None
         if ctx.needs_input_grad[1]:
             dw = stk.ops.dsd(grad.t(), x)
@@ -275,15 +278,15 @@
 
 class TensorParallelDsdNn(torch.autograd.Function):
     """
     Tensor parallel dsd
     """
 
     @staticmethod
-    @torch.cuda.amp.custom_fwd
+    @internlm_accelerator.amp.custom_fwd
     def forward(
         ctx, shape, data, row_indices, column_indices, offsets, column_indices_t, offsets_t, block_offsets_t, w, group
     ):
         # [m, k] x [k, n] = [m, n]
         if not data.is_contiguous() or not w.is_contiguous():
             raise ValueError("Expected contiguous 'data' and 'w'.")
 
@@ -296,15 +299,15 @@
 
         out = stk.ops.dsd(x, w)
         torch.distributed.all_reduce(out, group=group)
 
         return out
 
     @staticmethod
-    @torch.cuda.amp.custom_bwd
+    @internlm_accelerator.amp.custom_bwd
     def backward(ctx, grad):
         x = stk.Matrix(ctx.shape, *ctx.saved_tensors[:-1])
         w = ctx.saved_tensors[-1]
 
         dw = None
         if ctx.needs_input_grad[-2]:
             dw = stk.ops.dsd(x.t(), grad)
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/moe/utils.py` & `InternEvo-0.4.0.dev20240403/internlm/model/moe/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.3.3.dev20240315/internlm/monitor/alert.py` & `InternEvo-0.4.0.dev20240403/tests/test_training/test_no_fa_train_temp.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,136 +1,132 @@
-import json
-import math
-import os
-import re
-import time
-from typing import Dict
+import multiprocessing as mp
 
-import requests
+import pytest
 
+import internlm
+from internlm.accelerator import get_accelerator
+from internlm.core.context import ParallelMode
 from internlm.core.context import global_context as gpc
+from internlm.data import build_train_loader_with_data_type
+from internlm.model.losses import FlashGPTLMLoss
+from internlm.model.metrics import AccPerplex
+from internlm.train import (
+    get_scheduler_hooks,
+    initialize_isp_communicator,
+    initialize_model,
+    initialize_optimizer,
+)
 from internlm.utils.logger import get_logger
+from tests.common_fixture import (
+    build_environment,
+    config_7B,
+    find_free_port,
+    get_current_device,
+    load_new_batch,
+    seed_all,
+)
 
 logger = get_logger(__file__)
+internlm_accelerator = get_accelerator()
 
-
-def initialize_light_monitor(monitor_address: str = None):
-    """
-    Initialize the lightweight monitoring module.
-
-    Args:
-        monitor_address (str, optional): The address of the monitor. Defaults to 'MONITOR_SERVER' environment.
-
-    Raises:
-        Exception: If any exceptions occur during initialization, they will be caught and logged as warnings.
-
-    Example:
-        Initialize the monitoring module with the default address
-        ``initialize_light_monitor()``
-    """
-    try:
-        from uniscale_monitoring import init_monitor
-
-        init_monitor(monitor_address, is_root_rank=gpc.is_rank_for_log())
-    except Exception as e:
-        logger.warning(f"init monitor meet error: {e}")
-
-
-def send_heartbeat(msg_type: str, msg: Dict):
-    """
-    Send a heartbeat message to a monitoring server.
-
-    Args:
-        msg_type (str): The type of heartbeat message, e.g., "train_metrics", "init_time", "stage_time".
-        msg (Dict): A dictionary containing message data to be included in the heartbeat.
-
-    Example:
-        Sending a heartbeat message for training metrics
-        ``send_heartbeat("train_metrics", {"loss": 0.1, "accuracy": 0.95})``
-
-        Sending a heartbeat message for initialization time
-        ``send_heartbeat("init_time", {"import_time": 0.25})``
-
-        Sending a heartbeat message for stage time
-        ``send_heartbeat("stage_time", {"fwd_time": 2.3, "bwd_time": 6.2})``
-    """
-
-    def nan2none(v):
-        if isinstance(v, float) and math.isnan(v):
-            return None
-        return v
-
-    try:
-        from uniscale_monitoring import send_meta
-
-        data = {}
-        for k, v in msg.items():
-            if isinstance(v, Dict):
-                for k1, v1 in v.items():
-                    new_k = f"{k}_{k1}".split(" ")[0]
-                    new_k = re.sub(r"[^a-zA-Z0-9_]", "_", new_k)
-                    data[new_k] = nan2none(v1)
-            else:
-                new_k = k.split(" ")[0]
-                new_k = re.sub(r"[^a-zA-Z0-9_]", "_", new_k)
-                data[new_k] = nan2none(v)
-
-        if os.getenv("CLUSTER_NAME"):
-            data.update({"cluster": os.getenv("CLUSTER_NAME")})
-        if msg_type == "train_metrics":
-            data.update({"msg_type": "train_metrics"})
-        elif msg_type == "init_time":
-            data.update({"msg_type": "init_time"})
-        elif msg_type == "stage_time":
-            data.update({"msg_type": "stage_time"})
-        send_meta(data, timeout=0.1)
-    except Exception as e:
-        logger.warning(f"send heartbeat meet error: {e}")
-
-
-def send_feishu_msg_with_webhook(webhook: str, title: str, message: str):
-    """
-    Use Feishu robot to send messages with the given webhook.
-
-    Args:
-        webhook (str): The webhook to be used to send message.
-        title (str): The message title.
-        message (str): The message body.
-
-    Returns:
-        The response from the request. Or catch the exception and return None.
-
-    Raises:
-        Exception: An exception rasied by the HTTP post request.
-
-    """
-
-    headers = {"Content-Type": "application/json;charset=utf-8"}
-    msg_body = {
-        "timestamp": int(time.time()),
-        "msg_type": "post",
-        "content": {
-            "post": {
-                "zh_cn": {
-                    "title": title,
-                    "content": [
-                        [
-                            {
-                                "tag": "text",
-                                "text": message,
-                            },
-                        ],
-                    ],
-                },
-            },
-        },
-    }
-
-    try:
-        res = requests.post(webhook, data=json.dumps(msg_body), headers=headers, timeout=30)
-        res = res.json()
-        print(f"Feishu webhook response: {res}")
-    except Exception as err:  # pylint: disable=W0703
-        print(f"HTTP Post error: {err}")
-        res = None
-
-    return res
+# init config
+config = config_7B
+total_steps = 5
+config.data.total_steps = total_steps
+config.lr_scheduler.total_steps = total_steps
+config.model.use_flash_attn = False
+config.parallel.pipeline = dict(size=2, interleaved_overlap=True)
+
+
+def train_check(args):
+    # init
+    rank, world_size, free_port, mode, num_chunks = args
+    config.model.num_chunks = num_chunks
+    config.parallel.tensor = dict(size=2, mode=f"{mode}")
+    if mode == "isp":
+        config.parallel.weight = dict(size=4, overlap=True, memory_pool=True)
+
+    build_environment(rank, world_size, free_port, config)
+
+    # set seed
+    seed_all(1024)
+
+    # initialize model
+    model = initialize_model()
+
+    # initialize isp communicator
+    isp_communicator = initialize_isp_communicator(model)
+
+    # initialize loss function
+    criterion = FlashGPTLMLoss(parallel_output=True, label_smoothing=gpc.config.loss.label_smoothing)
+
+    optimizer, beta2_scheduler, lr_scheduler = initialize_optimizer(model, isp_communicator)
+
+    train_dl, dataset_types = build_train_loader_with_data_type()
+
+    metric = AccPerplex(
+        device=get_current_device(),
+        tp_pg=gpc.get_group(ParallelMode.TENSOR),
+        dp_pg=gpc.get_group(ParallelMode.DATA),
+        dataset_types=dataset_types,
+    )
+
+    trainer, train_dl, _, _ = internlm.initialize_trainer(
+        model=model,
+        optimizer=optimizer,
+        criterion=criterion,
+        train_dataloader=train_dl,
+        lr_scheduler=lr_scheduler,
+        beta2_scheduler=beta2_scheduler,
+        scheduler_hooks=get_scheduler_hooks(metric, optimizer, isp_communicator),
+    )
+
+    # transfer the train data loader into train data iterator
+    trainer.train()
+
+    train_iter = iter(train_dl)
+
+    for batch_count in range(total_steps):
+        if gpc.is_rank_for_log():
+            print(f"{mode}: {batch_count}", flush=True)
+
+        # load batch data
+        batch, train_iter = load_new_batch(train_dl=train_dl, train_iter=train_iter)
+
+        # zero the grads of parameters
+        trainer.zero_grad()
+
+        # process data
+        if batch[0].get("type_ids", None) is not None:
+            metric.set_current_type_ids(type_ids=batch[0].pop("type_ids", None))
+
+        # zero the grads of parameters
+        _, _, _ = trainer.execute_schedule(
+            batch,
+            forward_only=False,
+            return_loss=True,
+            return_output_label=False,
+        )
+
+        if isp_communicator and isp_communicator.enable_memory_pool:
+            isp_communicator.memory_pool.reset_lazy_pools()
+
+        trainer.step()
+        internlm_accelerator.reset_peak_memory_stats()
+
+
+mode_list = ["mtp"]
+num_chunks = [1, 2]
+
+
+@pytest.mark.parametrize("mode", mode_list)
+@pytest.mark.parametrize("num_chunks", num_chunks)
+def test_train(mode, num_chunks):
+    free_port = find_free_port()
+    ctx = mp.get_context("spawn")
+    with ctx.Pool(processes=8) as pool:
+        pool.map(
+            train_check,
+            [[rank, 8, free_port, mode, num_chunks] for rank in range(8)],
+        )
+        pool.close()
+        pool.join()
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/monitor/monitor.py` & `InternEvo-0.4.0.dev20240403/internlm/monitor/monitor.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from contextlib import contextmanager
 from threading import Thread
 
 from internlm.core.context import global_context as gpc
 from internlm.monitor.alert import send_feishu_msg_with_webhook
 from internlm.utils.common import SingletonMeta
 
-from .utils import get_job_key, set_env_var, try_import_send_exception
+from .utils import get_job_key, set_env_var
 
 
 def send_alert_message(address: str = None, title: str = None, message: str = None):
     """
     Send alert messages to the given Feishu webhook address in log rank.
 
     Args:
@@ -130,15 +130,14 @@
     Monitor Manager for managing monitor thread and monitoring training status.
     """
 
     def __init__(self, loss_spike_limit: float = 1.5) -> None:
         self.monitor_thread = None
         self.loss_spike_limit = loss_spike_limit
         self.last_step_loss = -1
-        self.send_exception = try_import_send_exception()
         self.alert_file_path = None
         self.enable_alert = False
         self.light_monitor_address = None
 
     def monitor_loss_spike(self, alert_address: str = None, step_count: int = 0, cur_step_loss: float = 0.0):
         """Check loss value, if loss spike occurs, send alert message to Feishu."""
         if self.enable_alert:
@@ -179,16 +178,14 @@
         """Catch and format exception information, send alert message to Feishu."""
         if self.enable_alert:
             filtered_trace = excp_info.split("\n")[-10:]
             format_trace = ""
             for line in filtered_trace:
                 format_trace += "\n" + line
 
-            if self.send_exception and self.light_monitor_address:
-                self.send_exception(format_trace, gpc.get_global_rank())
             message = f"Catch Exception from {socket.gethostname()} with rank id {gpc.get_global_rank()}:{format_trace}"
             if self.alert_file_path:
                 if self.exception_should_be_alert(format_trace, alert_address):
                     send_feishu_msg_with_webhook(
                         webhook=alert_address,
                         title=get_job_key(),
                         message=message,
@@ -200,16 +197,14 @@
         """Catch SIGTERM signal, and send alert message to Feishu."""
 
         def sigterm_handler(sys_signal, frame):
             if self.enable_alert:
                 print("receive frame: ", frame)
                 print("receive signal: ", sys_signal)
                 message = f"Process received signal {signal} and exited."
-                if self.send_exception and self.light_monitor_address:
-                    self.send_exception(message, gpc.get_global_rank())
                 send_alert_message(
                     address=alert_address,
                     message=message,
                 )
 
         signal.signal(signal.SIGTERM, sigterm_handler)
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/solver/beta2_scheduler.py` & `InternEvo-0.4.0.dev20240403/internlm/solver/schedulers/beta2_scheduler.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,17 +10,14 @@
     """
 
     def __init__(self, optimizer: torch.optim.Adam, init_beta2, c=0.8, cur_iter=-1):
         self.cur_iter = 0 if cur_iter == -1 else cur_iter
         self.init_beta2 = init_beta2
         self.c = c
         self.optimizer = optimizer
-        assert isinstance(
-            optimizer, (torch.optim.Adam, torch.optim.AdamW)
-        ), "should use Adam optimzier, which has beta2"
 
     def step(self, cur_iter=None):
         if cur_iter is None:
             self.cur_iter += 1
         else:
             self.cur_iter = cur_iter
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/solver/lr_scheduler.py` & `InternEvo-0.4.0.dev20240403/internlm/solver/schedulers/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.3.3.dev20240315/internlm/solver/optimizer/base_optimizer.py` & `InternEvo-0.4.0.dev20240403/internlm/solver/optimizer/base_optimizer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.3.3.dev20240315/internlm/solver/optimizer/fsdp_optimizer.py` & `InternEvo-0.4.0.dev20240403/internlm/solver/optimizer/fsdp_optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     def _compute_norm_with_fsdp_flatten(self, group_id):
         params = [p for p in self._fp16_param_groups[group_id] if p.untyped_storage().size() != 0]
         gradients = [p.grad for p in params if p.untyped_storage().size() != 0]
 
         norm_group = 0
         if len(params) <= 0 or len(gradients) <= 0:
             return norm_group
-        norm_group = compute_norm(gradients=gradients, parameters=params, last_stage=True)
+        norm_group = compute_norm(gradients=gradients, parameters=params)
 
         return norm_group
 
     def zero_grad(self):
         for _, param_group in self._fp16_param_groups.items():
             for param in param_group:
                 param.grad = None
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/solver/optimizer/hybrid_zero_optim.py` & `InternEvo-0.4.0.dev20240403/internlm/solver/optimizer/hybrid_zero_optim.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,18 +6,20 @@
 from itertools import product
 from typing import List, Optional
 
 import torch
 import torch.distributed as dist
 from torch.optim import Optimizer
 
+from internlm.accelerator import get_accelerator
 from internlm.core.communication.utils import ParamAsyncBcastHandler
-from internlm.core.context import IS_REPLICA_ZERO_PARALLEL, Config, ParallelMode
+from internlm.core.context import Config, ParallelMode
 from internlm.core.context import global_context as gpc
 from internlm.core.context.parallel_context import (
+    IS_REPLICA_ZERO_PARALLEL,
     IS_TENSOR_DATA_PARALLEL,
     IS_TENSOR_EXPERT_DATA_PARALLEL,
     IS_TENSOR_ZERO_PARALLEL,
     IS_WEIGHT_ZERO_PARALLEL,
 )
 from internlm.monitor import send_alert_message
 from internlm.solver.optimizer.store import (
@@ -39,25 +41,19 @@
 from internlm.utils.common import get_current_device
 from internlm.utils.logger import get_logger
 from internlm.utils.megatron_timers import megatron_timer as timer
 from internlm.utils.parallel import is_using_isp, is_using_sequence_parallel
 from internlm.utils.timeout import llm_timeout
 
 from .base_optimizer import BaseOptimizer
-from .utils import (
-    compute_layer_norm,
-    compute_layer_zero_grad_count,
-    compute_norm,
-    compute_param_norm,
-    compute_vocab_grad_norm,
-    compute_zero_grad_count,
-)
+from .utils import compute_norm
 
 inf = math.inf
 logger = get_logger(__file__)
+internlm_accelerator = get_accelerator()
 
 
 class HybridZeroOptimizer(BaseOptimizer):
     """
     Hybrid Zero Optimizer.
     """
 
@@ -119,15 +115,15 @@
             min_scale=min_scale,
             growth_factor=growth_factor,
             backoff_factor=backoff_factor,
             growth_interval=growth_interval,
             hysteresis=hysteresis,
             max_scale=max_scale,
         )
-        self._found_overflow = torch.cuda.FloatTensor([0], device=get_current_device())
+        self._found_overflow = torch.tensor([0], device=get_current_device(), dtype=torch.float32)
 
         # gradient clipping
         self._clip_grad_norm = clip_grad_norm
 
         # need to record the rank in which parameter groups are not assigned parameters.
         self.param_group_has_params = []
         self.param_group_no_params_ranks = []
@@ -192,24 +188,26 @@
                     self._param_store.add_fp16_param_list_by_rank_group(rank, group_id, params)
                     for param in params:
                         setattr(param, "group_id", group_id)
                         self._param_store.set_param_to_rank(param, rank)
 
             # move to cpu to make room to create the flat tensor
             for param in group_params:
+                if param.requires_grad is False:
+                    continue
                 param.data = param.data.cpu()
 
             # flatten the reordered tensors
             for rank in range(self._zero_world_size[group_id]):
                 # No flat fp16 buffer is allocated if the process has no parameters.
                 if rank not in self.param_group_no_params_ranks[group_id]:
                     tensor_list = self._param_store.get_fp16_params_by_rank_group(rank, group_id)
                     with torch.no_grad():
                         flat_tensor = flatten(tensor_list)
-                    flat_tensor = flat_tensor.data.cuda()
+                    flat_tensor = flat_tensor.data.to(get_current_device())
                     self._param_store.add_flat_fp16_param_by_rank_group(rank, group_id, flat_tensor)
                     sync_param(flat_tensor=flat_tensor, tensor_list=tensor_list)
 
             # create a copy of fp32 weights of the parameters for which this rank is responsible
             # No flat fp32 buffer is allocated if the process has no parameters.
             if self.param_group_has_params[group_id]:
                 fp16_flat_current_rank = self._param_store.get_flat_fp16_param_by_rank_group(
@@ -260,14 +258,17 @@
         params_per_rank = [[] for _ in range(self._zero_world_size[group_id])]
         numel_per_rank = [0 for _ in range(self._zero_world_size[group_id])]
         self.params_per_rank_id_dict.append([[] for _ in range(self._zero_world_size[group_id])])
         param_list = param_group["params"]
 
         sorted_params = sorted(param_list, key=lambda x: x.numel(), reverse=True)
         for i, param in enumerate(sorted_params):
+            if param.requires_grad is False:
+                continue
+
             global_id = str(i)
             for j in range(len(param.size())):
                 global_id = "_".join([global_id, str(param.size()[j])])
             if self._overlap_sync_param:
                 rank_to_go = self._param_bcast_sync_handler.get_rank_by_param(param)
             else:
                 rank_to_go = numel_per_rank.index(min(numel_per_rank))
@@ -434,15 +435,15 @@
         # check if the bucket is full
         # if full, will reduce the grads already in the bucket
         # after reduction, the bucket will be empty
         group_id = getattr(param, "group_id")
         current_bucket = self._bucket_store[group_id]
 
         if current_bucket.num_elements_in_bucket(reduce_rank) + param_size > self._reduce_bucket_size:
-            self._reduce_grads_stored_in_bucket(current_bucket, reduce_rank, last_bucket=False)
+            self._reduce_grads_stored_in_bucket(current_bucket, reduce_rank)
 
         # the param must not be reduced to ensure correctness
         is_param_reduced = self._param_store.is_param_reduced(param)
         if is_param_reduced:
             msg = (
                 f"Parameter of size ({param.size()}) has already been reduced, "
                 + "duplicate reduction will lead to arithmetic incorrectness"
@@ -452,15 +453,15 @@
         # the param must have grad for reduction
         assert param.grad is not None, f"Parameter of size ({param.size()}) has None grad, cannot be reduced"
 
         current_bucket.add_num_elements_in_bucket(param_size, reduce_rank)
         current_bucket.add_grad(param.grad, reduce_rank)
         current_bucket.add_param(param, reduce_rank)
 
-    def _reduce_grads_stored_in_bucket(self, current_bucket, reduce_rank=None, last_bucket=False):
+    def _reduce_grads_stored_in_bucket(self, current_bucket, reduce_rank=None):
         # reduce grads
         self._reduce_grads_by_rank(
             reduce_rank=reduce_rank,
             grads=current_bucket.get_grad(reduce_rank=reduce_rank),
             bucket_size=current_bucket.num_elements_in_bucket(reduce_rank),
             group_id=current_bucket.get_param_group_id(),
             dp_parallel_mode=current_bucket.get_dp_parallel_mode(),
@@ -480,15 +481,15 @@
                 )
                 raise RuntimeError(msg)
 
             # update the flag
             self._param_store.set_param_reduction_state(param, True)
 
             if self.belongs_to_current_rank(param):
-                self._param_store.add_reduced_param_for_compute_norm(param, last_bucket)
+                self._param_store.add_reduced_param_for_compute_norm(param)
             else:
                 self._param_store.add_previous_reduced_param(param)
 
         current_bucket.reset_by_rank(reduce_rank)
 
     def _reduce_grads_by_rank(self, reduce_rank, grads, bucket_size, group_id, dp_parallel_mode):
         grad_buckets_by_dtype = split_half_float_double(grads)
@@ -595,56 +596,47 @@
 
     def backward(self, loss, retain_graph=False):
         loss = self.loss_scale * loss
         loss.backward(retain_graph=retain_graph)
 
         # Gradients may not be fully synchronized here.
 
-    def _compute_norm_with_stage(
-        self,
-        group_id: int = 0,
-        last_bucket: bool = False,
-        last_stage: bool = False,
-        previous_norm=None,
-    ):
+    def _compute_norm(self, group_id: int = 0):
         # compute norm for gradients that have been reduced
-        params, grads = self._param_store.get_reduced_param_for_compute_norm(group_id=group_id, last_bucket=last_bucket)
+        params, grads = self._param_store.get_reduced_param_for_compute_norm(group_id=group_id)
         params_is_padding = False
         if len(params) == 0:
             params_is_padding = True
             dtype = self.param_groups[group_id]["dtype"]
             grads = [self.padding_grad.to(dtype)]
             params = [self.padding_tensor.to(dtype)]
 
-            if self.optim.param_groups[group_id]["name"] in ("default", "fp32"):
+            if self.optim.param_groups[group_id]["name"] == "default":
                 for param in params:
                     if self.use_isp:
                         setattr(param, IS_WEIGHT_ZERO_PARALLEL, True)
                     else:
                         setattr(param, IS_TENSOR_ZERO_PARALLEL, True)
+            elif self.optim.param_groups[group_id]["name"] == "fp32":
+                for param in params:
+                    setattr(param, IS_REPLICA_ZERO_PARALLEL, True)
             elif self.optim.param_groups[group_id]["name"] == "embed_head":
                 # should be isp mode
                 for param in params:
                     setattr(param, IS_TENSOR_DATA_PARALLEL, True)
             elif self._is_moe_group(self.optim.param_groups[group_id]):
                 for param in params:
                     setattr(param, IS_TENSOR_EXPERT_DATA_PARALLEL, True)
             else:
                 raise NotImplementedError("unrecognized parameter group.")
 
         norm = 0
         if self._clip_grad_norm > 0:
             # this norm is before scaling, it will be very large
-            norm = compute_norm(
-                gradients=grads,
-                parameters=params,
-                last_stage=last_stage,
-                previous_norm=previous_norm,
-                zero_mode=self._broadcast_parallel_mode[group_id],
-            )
+            norm = compute_norm(gradients=grads, parameters=params, zero_mode=self._broadcast_parallel_mode[group_id])
 
         if params_is_padding:
             for param in params:
                 if hasattr(param, IS_REPLICA_ZERO_PARALLEL):
                     delattr(param, IS_REPLICA_ZERO_PARALLEL)
                 if hasattr(param, IS_TENSOR_DATA_PARALLEL):
                     delattr(param, IS_TENSOR_DATA_PARALLEL)
@@ -653,173 +645,14 @@
                 if hasattr(param, IS_WEIGHT_ZERO_PARALLEL):
                     delattr(param, IS_WEIGHT_ZERO_PARALLEL)
                 if hasattr(param, IS_TENSOR_EXPERT_DATA_PARALLEL):
                     delattr(param, IS_TENSOR_EXPERT_DATA_PARALLEL)
 
         return norm
 
-    def _compute_param_norm_stage(
-        self, group_id: int = 0, last_bucket: bool = False, last_stage: bool = False, previous_param_norms=None
-    ):
-        # compute norm for gradients that have been reduced
-        params, grads = self._param_store.get_reduced_param_for_compute_norm(group_id=group_id, last_bucket=last_bucket)
-        params_is_padding = False
-        total_param_norms = {}
-        if len(params) == 0:
-            params_is_padding = True
-            dtype = self.param_groups[group_id]["dtype"]
-            grads = [self.padding_grad.to(dtype)]
-            params = [self.padding_tensor.to(dtype)]
-
-            if self.optim.param_groups[group_id]["name"] in ("default", "fp32"):
-                for param in params:
-                    if self.use_isp:
-                        setattr(param, IS_WEIGHT_ZERO_PARALLEL, True)
-                    else:
-                        setattr(param, IS_TENSOR_ZERO_PARALLEL, True)
-            elif self.optim.param_groups[group_id]["name"] == "embed_head":
-                # should be isp mode
-                for param in params:
-                    setattr(param, IS_TENSOR_DATA_PARALLEL, True)
-            elif self._is_moe_group(self.optim.param_groups[group_id]):
-                for param in params:
-                    setattr(param, IS_TENSOR_EXPERT_DATA_PARALLEL, True)
-            else:
-                raise NotImplementedError("unrecognized parameter group.")
-
-        if self._clip_grad_norm > 0:
-            total_param_norms = compute_param_norm(
-                grads,
-                params,
-                last_stage=last_stage,
-                previous_param_norms=previous_param_norms,
-                zero_mode=self._broadcast_parallel_mode[group_id],
-            )
-
-        if params_is_padding:
-            for param in params:
-                if hasattr(param, IS_REPLICA_ZERO_PARALLEL):
-                    delattr(param, IS_REPLICA_ZERO_PARALLEL)
-                if hasattr(param, IS_TENSOR_DATA_PARALLEL):
-                    delattr(param, IS_TENSOR_DATA_PARALLEL)
-                if hasattr(param, IS_TENSOR_ZERO_PARALLEL):
-                    delattr(param, IS_TENSOR_ZERO_PARALLEL)
-                if hasattr(param, IS_WEIGHT_ZERO_PARALLEL):
-                    delattr(param, IS_WEIGHT_ZERO_PARALLEL)
-                if hasattr(param, IS_TENSOR_EXPERT_DATA_PARALLEL):
-                    delattr(param, IS_TENSOR_EXPERT_DATA_PARALLEL)
-
-        return total_param_norms
-
-    def _compute_vocab_grad_norm_stage(
-        self, group_id: int = 0, last_bucket: bool = False, last_stage: bool = False, previous_vocab_grad_norm=None
-    ):
-        params, grads = self._param_store.get_reduced_param_for_compute_norm(group_id=group_id, last_bucket=last_bucket)
-        params_is_padding = False
-        if len(params) == 0:
-            params_is_padding = True
-            dtype = self.param_groups[group_id]["dtype"]
-            grads = [self.padding_grad.to(dtype)]
-            params = [self.padding_tensor.to(dtype)]
-
-            if self.optim.param_groups[group_id]["name"] in ("default", "fp32"):
-                for param in params:
-                    if self.use_isp:
-                        setattr(param, IS_WEIGHT_ZERO_PARALLEL, True)
-                    else:
-                        setattr(param, IS_TENSOR_ZERO_PARALLEL, True)
-            elif self.optim.param_groups[group_id]["name"] == "embed_head":
-                # should be isp mode
-                for param in params:
-                    setattr(param, IS_TENSOR_DATA_PARALLEL, True)
-            elif self._is_moe_group(self.optim.param_groups[group_id]):
-                for param in params:
-                    setattr(param, IS_TENSOR_EXPERT_DATA_PARALLEL, True)
-            else:
-                raise NotImplementedError("unrecognized parameter group.")
-
-        vocab_grad_norm = None
-
-        if self._clip_grad_norm > 0:
-            vocab_grad_norm = compute_vocab_grad_norm(
-                grads,
-                params,
-                last_stage=last_stage,
-                previous_vocab_grad_norm=previous_vocab_grad_norm,
-                zero_mode=self._broadcast_parallel_mode[group_id],
-            )
-
-        if params_is_padding:
-            for param in params:
-                if hasattr(param, IS_REPLICA_ZERO_PARALLEL):
-                    delattr(param, IS_REPLICA_ZERO_PARALLEL)
-                if hasattr(param, IS_TENSOR_DATA_PARALLEL):
-                    delattr(param, IS_TENSOR_DATA_PARALLEL)
-                if hasattr(param, IS_TENSOR_ZERO_PARALLEL):
-                    delattr(param, IS_TENSOR_ZERO_PARALLEL)
-                if hasattr(param, IS_WEIGHT_ZERO_PARALLEL):
-                    delattr(param, IS_WEIGHT_ZERO_PARALLEL)
-                if hasattr(param, IS_TENSOR_EXPERT_DATA_PARALLEL):
-                    delattr(param, IS_TENSOR_EXPERT_DATA_PARALLEL)
-
-        return vocab_grad_norm
-
-    def _count_zero_grads_stage(
-        self, group_id: int = 0, last_bucket: bool = False, last_stage: bool = False, previous_zero_grad_count=None
-    ):
-        params, grads = self._param_store.get_reduced_param_for_compute_norm(group_id=group_id, last_bucket=last_bucket)
-        params_is_padding = False
-        total_zero_grad_count = {}
-
-        if len(params) == 0:
-            params_is_padding = True
-            dtype = self.param_groups[group_id]["dtype"]
-            grads = [self.padding_grad.to(dtype)]
-            params = [self.padding_tensor.to(dtype)]
-
-            if self.optim.param_groups[group_id]["name"] in ("default", "fp32"):
-                for param in params:
-                    if self.use_isp:
-                        setattr(param, IS_WEIGHT_ZERO_PARALLEL, True)
-                    else:
-                        setattr(param, IS_TENSOR_ZERO_PARALLEL, True)
-            elif self.optim.param_groups[group_id]["name"] == "embed_head":
-                # should be isp mode
-                for param in params:
-                    setattr(param, IS_TENSOR_DATA_PARALLEL, True)
-            elif self._is_moe_group(self.optim.param_groups[group_id]):
-                for param in params:
-                    setattr(param, IS_TENSOR_EXPERT_DATA_PARALLEL, True)
-            else:
-                raise NotImplementedError("unrecognized parameter group.")
-
-        if self._clip_grad_norm > 0:
-            total_zero_grad_count = compute_zero_grad_count(
-                grads,
-                params,
-                last_stage=last_stage,
-                previous_zero_grad_count=previous_zero_grad_count,
-                zero_mode=self._broadcast_parallel_mode[group_id],
-            )
-
-        if params_is_padding:
-            for param in params:
-                if hasattr(param, IS_REPLICA_ZERO_PARALLEL):
-                    delattr(param, IS_REPLICA_ZERO_PARALLEL)
-                if hasattr(param, IS_TENSOR_DATA_PARALLEL):
-                    delattr(param, IS_TENSOR_DATA_PARALLEL)
-                if hasattr(param, IS_TENSOR_ZERO_PARALLEL):
-                    delattr(param, IS_TENSOR_ZERO_PARALLEL)
-                if hasattr(param, IS_WEIGHT_ZERO_PARALLEL):
-                    delattr(param, IS_WEIGHT_ZERO_PARALLEL)
-                if hasattr(param, IS_TENSOR_EXPERT_DATA_PARALLEL):
-                    delattr(param, IS_TENSOR_EXPERT_DATA_PARALLEL)
-
-        return total_zero_grad_count
-
     @llm_timeout(func_name="optim_step")
     def step(self, closure=None):
         """Performs a single optimization step.
 
         Args:
             closure (Callable, optional): A closure that reevaluates the model
                 and returns the loss.
@@ -835,109 +668,36 @@
                 for param in self._fp16_param_groups[group_id]:
                     # we should not reduce the param in moe
                     if param.grad is not None:
                         self._store_and_try_reduce_grads_by_bucket(param)
 
         # we need to reduce the gradients left in the communication bucket
         for group_id in range(self.num_param_groups):
-            self._reduce_grads_stored_in_bucket(self._bucket_store[group_id], reduce_rank=None, last_bucket=True)
+            self._reduce_grads_stored_in_bucket(self._bucket_store[group_id], reduce_rank=None)
 
-        # compute norm for gradients in the before bucket
-        grad_profiling_config = gpc.config.get("grad_profiling", {})
-        groups_norms = []
-        groups_param_norms = []
-        group_param_zero_grad_count = []
-        group_vocab_norms = []
-        batch_count = gpc.config.get("batch_count")
-        interval_steps = grad_profiling_config.get("interval_steps", 1)
-        is_profiling = batch_count % interval_steps == 0 if batch_count is not None else False
-        for group_id in range(self.num_param_groups):
-            groups_norms.append(self._compute_norm_with_stage(group_id=group_id))
-            if is_profiling:
-                if grad_profiling_config.get("grad_norm_profiling", False):
-                    groups_param_norms.append(self._compute_param_norm_stage(group_id=group_id))
-                if grad_profiling_config.get("zero_grad_profiling", False):
-                    group_param_zero_grad_count.append(self._count_zero_grads_stage(group_id=group_id))
-                if grad_profiling_config.get("vocab_grad_norm_profiling", False):
-                    group_vocab_norms.append(self._compute_vocab_grad_norm_stage(group_id=group_id))
-
-        # clear reduced grads
-        # grads in the last bucket is reduced
+        # wait grads reduced and clear reduced grads
         for bucket in self._bucket_in_progress:
             bucket.commu_handle.wait()
             bucket.unflatten_and_copy()
             bucket.empty()
         self._bucket_in_progress = []
         self._param_store.clear_grads_of_previous_reduced_params()
+
         # compute norm for gradients in the last bucket
         total_norms = {}
-        total_param_grad_norms = {}
-        total_layer_grad_norms = {}
-        total_param_zero_grad_count = {}
-        total_layer_zero_grad_count = {}
-        total_vocab_grad_norms = {}
         for group_id in range(self.num_param_groups):
             group_name = self.param_groups[group_id]["name"] if "name" in self.param_groups[group_id] else "default"
             group_name = f"{group_id}_{group_name}"
-            total_norms[group_name] = self._compute_norm_with_stage(
-                group_id=group_id,
-                last_bucket=True,
-                last_stage=True,
-                previous_norm=groups_norms[group_id],
-            )
-            if is_profiling:
-                if grad_profiling_config.get("grad_norm_profiling", False):
-                    param_norms = self._compute_param_norm_stage(
-                        group_id=group_id,
-                        last_bucket=True,
-                        last_stage=True,
-                        previous_param_norms=groups_param_norms[group_id],
-                    )
-                    total_layer_grad_norms[group_name], total_param_grad_norms[group_name] = compute_layer_norm(
-                        param_norms=param_norms, loss_scale=self.loss_scale.item()
-                    )
-                if grad_profiling_config.get("zero_grad_profiling", False):
-                    zero_grad_count = self._count_zero_grads_stage(
-                        group_id=group_id,
-                        last_bucket=True,
-                        last_stage=True,
-                        previous_zero_grad_count=group_param_zero_grad_count[group_id],
-                    )
-                    (
-                        total_layer_zero_grad_count[group_name],
-                        total_param_zero_grad_count[group_name],
-                    ) = compute_layer_zero_grad_count(zero_grad_count)
-                if grad_profiling_config.get("vocab_grad_norm_profiling", False):
-                    vocab_grad_norms = self._compute_vocab_grad_norm_stage(
-                        group_id=group_id,
-                        last_bucket=True,
-                        last_stage=True,
-                        previous_vocab_grad_norm=group_vocab_norms[group_id],
-                    )
-                    inf_mask = vocab_grad_norms == -1
-                    nan_mask = vocab_grad_norms == -2
-                    vocab_grad_norms = vocab_grad_norms**0.5 / self.loss_scale.item()
-                    vocab_grad_norms[inf_mask] = -1
-                    vocab_grad_norms[nan_mask] = -2
-                    total_vocab_grad_norms[group_name] = vocab_grad_norms.to("cpu")
+            total_norms[group_name] = self._compute_norm(group_id=group_id)
 
         timer("sync_grad").start()
         self._sync_grad()
         timer("sync_grad").stop()
 
         state, global_norms = self._step(closure=closure, norms=total_norms)
-        if is_profiling:
-            if grad_profiling_config.get("grad_norm_profiling", False):
-                global_norms["layer_grad_norm"] = total_layer_grad_norms
-                global_norms["param_grad_norm"] = total_param_grad_norms
-            if grad_profiling_config.get("zero_grad_profiling", False):
-                global_norms["layer_zero_grad"] = total_layer_zero_grad_count
-                global_norms["param_zero_grad"] = total_param_zero_grad_count
-            if grad_profiling_config.get("vocab_grad_norm_profiling", False):
-                global_norms["vocab_grad_norm"] = total_vocab_grad_norms
 
         return state, global_norms
 
     def _step(self, closure=None, norms=None):
         assert closure is None, "closure is not supported by step()"
 
         # check for overflow
@@ -1036,15 +796,15 @@
             for group_id in range(len(self._fp16_param_groups)):
                 if self.param_group_has_params[group_id]:
                     fp16_param = self._param_store.get_flat_fp16_param_by_rank_group(
                         rank=self._zero_local_rank[group_id], group_id=group_id
                     )
                     fp32_param = self._fp32_flat_param_groups_of_current_rank[group_id]
                     fp16_param.data.copy_(fp32_param)
-        torch.cuda.synchronize()
+        internlm_accelerator.synchronize()
         self.broadcast_params()
 
         timer("step").stop()
 
         # update gradients may not be needed here, because the sync_params function is used in initialization,
         # so synchronization is maintained
         for group_name, global_norm in global_norm_groups.items():
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/solver/optimizer/store.py` & `InternEvo-0.4.0.dev20240403/internlm/solver/optimizer/store.py`

 * *Files 8% similar despite different names*

```diff
@@ -159,18 +159,16 @@
         self._rank_groupid_to_fp16_param_list = dict()
         self._rank_group_id_to_flat_fp16_param = dict()
 
         # param reduction data structures
         self._is_param_reduced = dict()
         self._reduced_param = []
 
-        self._former_bucket_reduced_param = {}
-        self._last_bucket_reduced_param = {}
-        self._former_bucket_reduced_grad = {}
-        self._last_bucket_reduced_grad = {}
+        self._bucket_reduced_param = {}
+        self._bucket_reduced_grad = {}
 
     def set_param_to_rank(self, tensor: Tensor, rank: int) -> None:
         """
         Set the mapping between parameter to rank, each parameter should be owned by a rank.
 
         :param tensor: A :class:`torch.Tensor` object
         :type tensor: torch.Tensor
@@ -223,52 +221,34 @@
 
     def reset_previous_reduced_params(self):
         self._reduced_param = []
 
     def add_previous_reduced_param(self, tensor):
         self._reduced_param.append(tensor)
 
-    def add_reduced_param_for_compute_norm(self, param, last_bucket=False):
+    def add_reduced_param_for_compute_norm(self, param):
         group_id = getattr(param, "group_id")
-        if last_bucket:
-            if group_id not in self._last_bucket_reduced_param:
-                self._last_bucket_reduced_param[group_id] = []
-                self._last_bucket_reduced_grad[group_id] = []
-
-            self._last_bucket_reduced_param[group_id].append(param)
-            self._last_bucket_reduced_grad[group_id].append(param.grad)
-        else:
-            if group_id not in self._former_bucket_reduced_param:
-                self._former_bucket_reduced_param[group_id] = []
-                self._former_bucket_reduced_grad[group_id] = []
-
-            self._former_bucket_reduced_param[group_id].append(param)
-            self._former_bucket_reduced_grad[group_id].append(param.grad)
-
-    def get_reduced_param_for_compute_norm(self, group_id=0, last_bucket=False):
-        if not last_bucket:
-            if group_id not in self._former_bucket_reduced_param:
-                return [], []
-            return (
-                self._former_bucket_reduced_param[group_id],
-                self._former_bucket_reduced_grad[group_id],
-            )
-        else:
-            if group_id not in self._last_bucket_reduced_param:
-                return [], []
-            return (
-                self._last_bucket_reduced_param[group_id],
-                self._last_bucket_reduced_grad[group_id],
-            )
+        if group_id not in self._bucket_reduced_param:
+            self._bucket_reduced_param[group_id] = []
+            self._bucket_reduced_grad[group_id] = []
+
+        self._bucket_reduced_param[group_id].append(param)
+        self._bucket_reduced_grad[group_id].append(param.grad)
+
+    def get_reduced_param_for_compute_norm(self, group_id=0):
+        if group_id not in self._bucket_reduced_param:
+            return [], []
+        return (
+            self._bucket_reduced_param[group_id],
+            self._bucket_reduced_grad[group_id],
+        )
 
     def reset_reduced_data_for_compute_norm(self):
-        self._former_bucket_reduced_param = {}
-        self._last_bucket_reduced_param = {}
-        self._former_bucket_reduced_grad = {}
-        self._last_bucket_reduced_grad = {}
+        self._bucket_reduced_param = {}
+        self._bucket_reduced_grad = {}
 
     def clear_grads_of_previous_reduced_params(self):
         if len(self._reduced_param) > 0:
             for param in self._reduced_param:
                 param.grad = None
             self.reset_previous_reduced_params()
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/solver/pipeline_utils.py` & `InternEvo-0.4.0.dev20240403/internlm/solver/pipeline_utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.3.3.dev20240315/internlm/train/__init__.py` & `InternEvo-0.4.0.dev20240403/internlm/train/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,21 @@
-from .training_internlm import (
+from .pipeline import (
     get_scheduler_hooks,
-    get_train_data_loader,
-    get_validation_data_loader,
     initialize_isp_communicator,
     initialize_llm_profile,
     initialize_model,
     initialize_optimizer,
     load_new_batch,
     record_current_batch_training_metrics,
     set_fp32_attr_for_model,
     set_parallel_attr_for_param_groups,
     wrap_FSDP_model,
 )
 
 __all__ = [
-    "get_train_data_loader",
-    "get_validation_data_loader",
     "initialize_llm_profile",
     "initialize_model",
     "initialize_isp_communicator",
     "initialize_optimizer",
     "load_new_batch",
     "record_current_batch_training_metrics",
     "wrap_FSDP_model",
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/train/training_internlm.py` & `InternEvo-0.4.0.dev20240403/internlm/train/pipeline.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 #!/usr/bin/env python
 # -*- encoding: utf-8 -*-
 
 import functools
-import os
-import pickle
 import time
-from functools import partial
 from typing import Callable, Iterable, List, Optional, Union
 
 import torch
-import torch.distributed as dist
 from torch import nn
 from torch.distributed.fsdp import FullyShardedDataParallel as FSDP
 from torch.distributed.fsdp.fully_sharded_data_parallel import (
     BackwardPrefetch,
     ShardingStrategy,
 )
 from torch.distributed.fsdp.wrap import transformer_auto_wrap_policy
-from torch.utils.data import ConcatDataset, DataLoader
+from torch.utils.data import DataLoader
 
+from internlm.accelerator import AcceleratorType, get_accelerator
 from internlm.core.communication.isp import (
     ISPCommModelConfig,
     ISPCommunicator,
     ISPCommunicatorSchedulerHook,
 )
 from internlm.core.communication.utils import ParamAsyncBcastHandler
 from internlm.core.context import (
@@ -33,69 +30,63 @@
     IS_WEIGHT_ZERO_PARALLEL,
     ParallelMode,
 )
 from internlm.core.context import global_context as gpc
 from internlm.core.context.random import set_mode
 from internlm.core.naive_amp import NaiveAMPModel, set_fp32_attr_to_module
 from internlm.core.trainer import TrainState
-from internlm.data.batch_sampler import StaticBatchSampler, get_dpsampler_dataloader
-from internlm.data.collaters import jsonl_ds_collate_fn, packed_collate_fn
-from internlm.data.dataset import get_dataset_dict
-from internlm.data.dummy_dataset import RandomDataset
-from internlm.data.packed_dataset import (
-    PackedDataset,
-    PackedDatasetWithoutCuSeqlen,
-    get_packed_dataset_without_short_length,
+from internlm.data.utils import unpack_data
+from internlm.model.metrics import SchedulerMetricHook
+from internlm.model.modules.embedding import Embedding1D
+from internlm.model.modules.mlp import FeedForward
+from internlm.model.modules.multi_head_attention import MHA
+from internlm.model.moe.megablock.mlp import (
+    MegaBlockFeedForward,
+    MegaBlockGroupedFeedForward,
 )
-from internlm.data.utils import get_dataset_type_ids_map, unpack_data
-from internlm.model.embedding import Embedding1D
-from internlm.model.linear import (
+from internlm.model.moe.moe import MoE
+from internlm.model.ops.linear import (
     BaseScaleColumnParallelLinear,
     ColumnParallelLinearTorch,
-    FeedForward,
     ISPLinear,
     RewardModelLinear,
     RowParallelLinearTorch,
     ScaleColumnParallelLinear,
 )
-from internlm.model.metrics import SchedulerMetricHook
-from internlm.model.moe import MoE
-from internlm.model.multi_head_attention import MHA
 from internlm.model.utils import is_moe_param, try_import_RMSNorm
-from internlm.moe.megablock.mlp import MegaBlockFeedForward, MegaBlockGroupedFeedForward
-from internlm.monitor import send_heartbeat, set_env_var
+from internlm.monitor import set_env_var
 from internlm.monitor.monitor import monitor_manager as mm
-from internlm.solver.beta2_scheduler import Beta2Scheduler
-from internlm.solver.lr_scheduler import FineTuneCosineAnnealingWarmupLR
 from internlm.solver.optimizer import FSDPadaptOptimizer, HybridZeroOptimizer
+from internlm.solver.schedulers.beta2_scheduler import Beta2Scheduler
+from internlm.solver.schedulers.lr_scheduler import FineTuneCosineAnnealingWarmupLR
 from internlm.train.utils import create_param_groups
-from internlm.utils.common import (
-    DummyProfile,
-    SchedulerHook,
-    get_current_device,
-    launch_time,
-)
+from internlm.utils.common import DummyProfile, SchedulerHook, get_current_device
 from internlm.utils.logger import get_logger
 from internlm.utils.megatron_timers import megatron_timer as timer
 from internlm.utils.parallel import (
     is_replica_zero_parallel_parameter,
     is_tensor_data_parallel_parameter,
     is_tensor_expert_data_parallel_parameter,
     is_tensor_zero_parallel_parameter,
     is_using_isp,
     is_weight_zero_parallel_parameter,
-    set_model_params_layer_name,
     sync_model_param,
     sync_model_replica_param_group,
 )
 from internlm.utils.registry import MODEL_INITIALIZER
 from internlm.utils.timeout import llm_timeout
 
+try:
+    import torch_npu
+except (ImportError, ModuleNotFoundError):
+    pass
+
 RMSNorm = try_import_RMSNorm()
 logger = get_logger(__file__)
+internlm_accelerator = get_accelerator()
 
 
 def set_fp32_attr_for_model(model: Union[nn.Module, nn.ModuleList]):
     if not isinstance(model, nn.ModuleList):
         model = [model]
 
     for _chunk in model:
@@ -112,19 +103,19 @@
                 setattr(param, IS_REPLICA_ZERO_PARALLEL, True)
 
         if isinstance(module, MoE):
             for param in module.moe_layer.gate.parameters():
                 setattr(param, IS_REPLICA_ZERO_PARALLEL, True)
 
         # embedding and head
-        if gpc.config.model.use_flash_attn:
+        if gpc.config.use_cuda_flash_attn:
             from flash_attn.modules.embedding import ParallelGPT2Embeddings
 
         if isinstance(module, (Embedding1D, BaseScaleColumnParallelLinear)) or (
-            gpc.config.model.use_flash_attn and isinstance(module, ParallelGPT2Embeddings)
+            gpc.config.use_cuda_flash_attn and isinstance(module, ParallelGPT2Embeddings)
         ):
             for param in module.parameters():
                 if gpc.is_initialized(ParallelMode.TENSOR) and is_using_isp():
                     setattr(param, IS_TENSOR_DATA_PARALLEL, True)
                 elif gpc.is_initialized(ParallelMode.TENSOR) and not is_using_isp():
                     setattr(param, IS_TENSOR_ZERO_PARALLEL, True)
 
@@ -295,50 +286,71 @@
 
     Args:
         model (:class:`torch.nn.Module`): Your model instance to be trained or evaluated.
 
     Returns:
         A tuple of (optimizer, beta2_scheduler, lr_scheduler).
     """
-    grad_profiling_config = gpc.config.get("grad_profiling", {})
-    if (
-        grad_profiling_config.get("grad_norm_profiling", False)
-        or grad_profiling_config.get("zero_grad_profiling", False)
-        or grad_profiling_config.get("vocab_grad_norm_profiling", False)
-    ):
-        # set the layer name as an attribute of the model parameters
-        set_model_params_layer_name(model)
-
-    if gpc.config.hybrid_zero_optimizer.overlap_sync_param:
-        param_bcast_sync_handler = ParamAsyncBcastHandler(ParallelMode.ZERO1, model, isp_communicator)
-    else:
-        param_bcast_sync_handler = None
 
     adam_cfg = gpc.config.adam
+    zero_cfg = gpc.config.hybrid_zero_optimizer
+    grad_scal_cfg = gpc.config.grad_scaler
+
     params = create_param_groups(model, adam_cfg.weight_decay)
-    naive_optimizer = torch.optim.AdamW(
+    adam_extra_kwargs = {}
+    # set fused=True to avoid nan grad norm when model size is larger and use_fp32_norm=True
+
+    # TODO(caikun): add DIPU backend adamw
+    if internlm_accelerator.get_accelerator_backend() == AcceleratorType.NPU:
+        internlm_adamw = torch_npu.optim.NpuFusedAdamW
+    else:
+        internlm_adamw = torch.optim.AdamW
+        if torch.__version__ >= "2.1.0" and internlm_accelerator.get_accelerator_backend() == AcceleratorType.GPU:
+            adam_extra_kwargs["fused"] = True
+
+    naive_optimizer = internlm_adamw(
         params=params,
         lr=adam_cfg.lr,
         betas=(adam_cfg.adam_beta1, adam_cfg.adam_beta2),
         eps=adam_cfg.adam_eps,
+        **adam_extra_kwargs,
     )
 
+    if (
+        zero_cfg.overlap_sync_grad
+        and gpc.is_using_parallel_mode(ParallelMode.PIPELINE)
+        and gpc.is_pipeline_first_stage() is False
+    ):
+        # When pipeline parallelism is enabled, we prefer to only enable optimizer
+        # gradient communication overlap in the first stage, to avoid amplifying
+        # the communication overhead stage by stage in cases where the optimizer
+        # communication overhead is greater than the compute overhead.
+        # For pipeline stages except the first, even if overlap is not enabled,
+        # their gradient synchronization overhead can be well hidden by
+        # the inherent bubbles of pipeline parallelism.
+        zero_cfg.overlap_sync_grad = False
+
+    if zero_cfg.overlap_sync_param:
+        param_bcast_sync_handler = ParamAsyncBcastHandler(ParallelMode.ZERO1, model, isp_communicator)
+    else:
+        param_bcast_sync_handler = None
+
     if not gpc.config.parallel.zero1.fsdp:
         optimizer = HybridZeroOptimizer(
             naive_optimizer,
-            grad_scal_cfg=gpc.config.grad_scaler,
-            zero_cfg=gpc.config.hybrid_zero_optimizer,
+            grad_scal_cfg=grad_scal_cfg,
+            zero_cfg=zero_cfg,
             param_bcast_sync_handler=param_bcast_sync_handler,
             isp_communicator=isp_communicator,
         )
     else:
         optimizer = FSDPadaptOptimizer(
             naive_optimizer,
-            grad_scal_cfg=gpc.config.grad_scaler,
-            zero_cfg=gpc.config.hybrid_zero_optimizer,
+            grad_scal_cfg=grad_scal_cfg,
+            zero_cfg=zero_cfg,
         )
 
     beta2_scheduler = Beta2Scheduler(optimizer=naive_optimizer, **gpc.config.beta2_scheduler)
 
     lr_scheduler = FineTuneCosineAnnealingWarmupLR(optimizer, **gpc.config.lr_scheduler)
 
     return optimizer, beta2_scheduler, lr_scheduler
@@ -362,143 +374,14 @@
 
     if isp_communicator is not None and gpc.config.parallel["weight"].get("overlap", False):
         scheduler_hooks.append(ISPCommunicatorSchedulerHook(isp_communicator, zero_optim))
 
     return scheduler_hooks
 
 
-@llm_timeout(func_name="get_train_data_loader")
-def get_train_data_loader(num_worker: int = 0, dataset_generate_func: Optional[Callable] = None):
-    """
-    Generate and return the training data loader.
-
-    Args:
-        num_worker (:class:`int`): number of subprocesses used for dataloader.
-        dataset_generate_func (:class:`Callable`, optional): generate function for dataset.
-
-    Returns:
-        A tuple of (train_dl, dataset_types).
-    """
-
-    # Get the dataset types
-    data_cfg = gpc.config.data
-    train_folder = data_cfg.train_folder
-    dataset_types = list(get_dataset_type_ids_map(train_folder).keys())
-
-    if dataset_generate_func is not None:
-        train_ds, train_sampler, train_collate_fn = dataset_generate_func()
-    else:
-        if train_folder is None:
-            dataset_types = ["en", "cn", "code"]
-            train_ds = RandomDataset(num_samples=1000000, max_len=data_cfg.seq_len)
-            if data_cfg.pack_sample_into_one:
-                train_ds = PackedDatasetWithoutCuSeqlen(
-                    train_ds, max_length_per_sample=data_cfg.seq_len, packed_length=data_cfg.packed_length
-                )
-            else:
-                train_ds = PackedDataset(
-                    train_ds, max_length_per_sample=data_cfg.seq_len, packed_length=data_cfg.packed_length
-                )
-        else:
-            train_ds = get_packed_dataset_without_short_length(
-                folder=data_cfg.train_folder,
-                packed_length=data_cfg.packed_length,
-                max_length_per_sample=data_cfg.seq_len,
-                show_progress=dist.get_rank() == 0,
-                min_length=data_cfg.min_length,
-                min_length_dict=data_cfg.get("min_length_dict", {}),
-                pack_into_one_sample=data_cfg.pack_sample_into_one,
-            )
-        train_sampler = StaticBatchSampler(
-            train_ds.datasets if isinstance(train_ds, ConcatDataset) else [train_ds],
-            batch_size=data_cfg.micro_num,
-            rampup_batch_size=data_cfg.rampup_batch_size,
-            micro_bsz=data_cfg.micro_bsz,
-            seed=1024,
-            drop_last=True,
-            data_rank=gpc.get_local_rank(ParallelMode.DATA),
-            data_world_size=gpc.get_world_size(ParallelMode.DATA),
-        )
-        train_collate_fn = partial(packed_collate_fn, packed_length=data_cfg.packed_length)
-
-    # Create the training data loader
-    train_dl = DataLoader(
-        dataset=train_ds,
-        batch_sampler=train_sampler,
-        num_workers=num_worker,
-        pin_memory=True,
-        collate_fn=train_collate_fn,
-        persistent_workers=num_worker > 0,
-    )
-
-    return train_dl, dataset_types
-
-
-@llm_timeout(func_name="get_validation_data_loader")
-def get_validation_data_loader(
-    num_worker: int = 0, dataset_generate_func: Callable = None, val_collate_fn=None, dataloader_func=None
-):
-    """Generate and return the validation data loader."""
-
-    data_cfg = gpc.config.data
-
-    if not data_cfg.valid_folder:
-        val_ds = RandomDataset(num_samples=gpc.get_world_size(ParallelMode.DATA) * 500, max_len=data_cfg.seq_len)
-    else:
-        if dataset_generate_func is not None:
-            assert val_collate_fn and dataloader_func is not None
-            val_ds = dataset_generate_func()
-        else:
-            val_ds = get_dataset_dict(folder=data_cfg.valid_folder, split="")
-
-    if not isinstance(val_ds, dict):
-        val_ds = {"val": val_ds}
-
-    if val_collate_fn is None or not data_cfg.valid_folder:
-        val_collate_fn = partial(jsonl_ds_collate_fn, max_length_per_sample=data_cfg.seq_len)
-
-    val_dls = {}
-    for val_name, ds in val_ds.items():
-        if dataloader_func and data_cfg.valid_folder is not None:
-            val_dls[val_name] = dataloader_func(dataset=ds, collate_fn=val_collate_fn)
-            if gpc.is_rank_for_log():
-                logger.info(
-                    f"load validation dataset {val_name} with valid batch size {str(data_cfg.valid_micro_num)} and "
-                    f"{ds.size} Byte samples."
-                )
-        else:
-            # making the batch_size of validate larger can speed up the evaluation, but it should not be too large,
-            # otherwise too much data may be dropped
-            batch_size = min(
-                data_cfg.valid_micro_num * data_cfg.micro_bsz, len(ds) // gpc.get_world_size(ParallelMode.DATA)
-            )
-            batch_size = batch_size // data_cfg.micro_bsz * data_cfg.micro_bsz
-
-            if batch_size == 0 and gpc.is_rank_for_log():
-                logger.info(f"skip validate {val_name}.")
-                continue
-
-            val_dls[val_name] = get_dpsampler_dataloader(
-                ds,
-                shuffle=False,
-                num_workers=num_worker,
-                batch_size=batch_size,
-                collate_fn=val_collate_fn,
-                drop_last=True,
-            )  # drop_last=True, otherwise it may cause problems in the last batch
-
-            if gpc.is_rank_for_log():
-                logger.info(
-                    f"load validation dataset {val_name} with valid batch size {str(batch_size)} and "
-                    f"samples {str(len(val_dls[val_name]))}."
-                )
-
-    return val_dls
-
-
 @llm_timeout(func_name="load_new_batch")
 def load_new_batch(train_dl: DataLoader, train_iter: Iterable, train_state: TrainState):
     """
     Load and return the new batch data based on training data loader.
 
     Args:
         train_dl (torch.utils.data.DataLoader): Dataloader for training.
@@ -514,48 +397,71 @@
         if hasattr(train_state, "batch_sampler_iter"):
             next(train_state.batch_sampler_iter)
     except StopIteration:
         train_iter = iter(train_dl)
         batch = next(train_iter)
         train_state.num_consumed_samples_in_epoch = 0
         if hasattr(train_state, "batch_sampler"):
+            train_state.batch_sampler.batch_count = 0
+            train_state.batch_sampler.num_consumed_samples_in_epoch = 0
             train_state.batch_sampler_iter = iter(train_state.batch_sampler)
             next(train_state.batch_sampler_iter)
     timer("batch-gen").stop()
 
     if batch[0].get("type_ids", None) is not None:
-        # if use_flash_attn is False, we need to unpack type_ids
-        if not gpc.config.model.use_flash_attn:
+        # if use_packed_dataset is False, we need to unpack type_ids
+        if not gpc.config.data.use_packed_dataset:
             batch[0]["type_ids"] = unpack_data(batch[0]["type_ids"], batch[0]["cu_seqlens"], is_type_ids=True)
 
     return batch, train_iter
 
 
 def initialize_llm_profile(profiling: bool = False, start_time: str = None):
     """Initialize and return the profiler context manager instance."""
 
     if profiling and gpc.get_local_rank(ParallelMode.DATA) == 0 and gpc.get_local_rank(ParallelMode.TENSOR) == 0:
-        llm_profile = torch.profiler.profile
-        logger.info(f"Do profiling in rank {gpc.get_global_rank()}!")
+        schedule_config = {"wait": 1, "warmup": 1, "active": 1, "repeat": 1, "skip_first": 3}
+        trace_path = (
+            f"RUN/{gpc.config.JOB_NAME}/{start_time}/traces/rank{gpc.get_global_rank()}_"
+            f"dp{gpc.get_local_rank(ParallelMode.DATA)}_"
+            f"wp{gpc.get_local_rank(ParallelMode.WEIGHT)}_"
+            f"tp{gpc.get_local_rank(ParallelMode.TENSOR)}"
+        )
+        if internlm_accelerator.get_accelerator_backend() == AcceleratorType.NPU:
+            experimental_config = torch_npu.profiler._ExperimentalConfig(
+                aic_metrics=torch_npu.profiler.AiCMetrics.PipeUtilization,
+                profiler_level=torch_npu.profiler.ProfilerLevel.Level1,
+                l2_cache=False,
+            )
+            llm_profile = torch_npu.profiler.profile(
+                activities=[torch_npu.profiler.ProfilerActivity.CPU, torch_npu.profiler.ProfilerActivity.NPU],
+                schedule=torch_npu.profiler.schedule(**schedule_config),
+                on_trace_ready=torch_npu.profiler.tensorboard_trace_handler(trace_path),
+                record_shapes=True,
+                profile_memory=True,
+                with_stack=False,
+                with_flops=False,
+                with_modules=False,
+                experimental_config=experimental_config,
+            )
+            logger.info(f"Do profiling for NPU on rank {gpc.get_global_rank()}!")
+        else:
+            llm_profile = torch.profiler.profile(
+                activities=[torch.profiler.ProfilerActivity.CPU, torch.profiler.ProfilerActivity.CUDA],
+                schedule=torch.profiler.schedule(**schedule_config),
+                on_trace_ready=torch.profiler.tensorboard_trace_handler(trace_path),
+                with_stack=True,
+                with_modules=True,
+                profile_memory=True,
+            )
+            logger.info(f"Do profiling for GPU on rank {gpc.get_global_rank()}!")
     else:
-        llm_profile = DummyProfile
+        llm_profile = DummyProfile()
 
-    return llm_profile(
-        activities=[torch.profiler.ProfilerActivity.CPU, torch.profiler.ProfilerActivity.CUDA],
-        schedule=torch.profiler.schedule(skip_first=5, wait=1, warmup=1, active=1, repeat=1),
-        on_trace_ready=torch.profiler.tensorboard_trace_handler(
-            f"RUN/{gpc.config.JOB_NAME}/{start_time}/traces/rank{gpc.get_global_rank()}_"
-            + f"dp{gpc.get_local_rank(ParallelMode.DATA)}_"
-            + f"wp{gpc.get_local_rank(ParallelMode.WEIGHT)}_"
-            + f"tp{gpc.get_local_rank(ParallelMode.TENSOR)}",
-        ),
-        with_stack=True,
-        with_modules=True,
-        profile_memory=True,
-    )
+    return llm_profile
 
 
 @llm_timeout(func_name="record_current_batch_training_metrics")
 def record_current_batch_training_metrics(
     get_tflops_func,
     logger,
     writer,
@@ -679,61 +585,22 @@
 
         fwd_bwd_time = round(timer("fwd-bwd").elapsed(), 2)
         infos["fwd_bwd_time"] = fwd_bwd_time
 
         for key, value in acc_perplex.items():
             infos[key] = value
 
-        grad_profiling_config = gpc.config.get("grad_profiling", {})
-        interval_steps = grad_profiling_config.get("interval_steps", 1)
-        if batch_count % interval_steps == 0:
-            layer_metrics = [metric for metric in ["layer_grad_norm", "layer_zero_grad"] if metric in grad_norm]
-            param_metrics = [metric for metric in ["param_grad_norm", "param_zero_grad"] if metric in grad_norm]
-            layer_names = grad_profiling_config.get("layers", [])
-            for metric_name in layer_metrics:
-                metric = grad_norm.get(metric_name)
-                for group_name, layer_group in metric.items():
-                    title = f"{metric_name}/{group_name}"
-                    metrics = {k: v for k, v in layer_group.items() if not layer_names or k in layer_names}
-                    if metrics:
-                        writer.add_scalars(key=title, value=metrics, step=train_state.step_count)
-                del grad_norm[metric_name]
-            for metric_name in param_metrics:
-                metric = grad_norm.get(metric_name)
-                for group_name, layer_group in metric.items():
-                    for param_name, param_group in layer_group.items():
-                        title = f"{param_name}/{group_name}_{metric_name}"
-                        metrics = {k: v for k, v in param_group.items() if not layer_names or k in layer_names}
-                        if metrics:
-                            writer.add_scalars(key=title, value=metrics, step=train_state.step_count)
-                del grad_norm[metric_name]
-            if grad_profiling_config.get("vocab_grad_norm_profiling", False):
-                local_save_path = f"RUN/{gpc.config.JOB_NAME}/{launch_time()}/grad_norm"
-                os.makedirs(local_save_path, exist_ok=True)
-                local_save_file = f"{local_save_path}/vocab_grad_norm.pt"
-                vocab_grad_norms = grad_norm.get("vocab_grad_norm")
-                if vocab_grad_norms:
-                    try:
-                        with open(local_save_file, "ab+") as vocab_f:
-                            pickle.dump((train_state.step_count, vocab_grad_norms), vocab_f)
-                    except IOError as e:
-                        logger.warning(f"Error saving vocab_grad_norm: {e}")
-                del grad_norm["vocab_grad_norm"]
-
         line = ""
         for key, value in infos.items():
             line += f"{key}={value} "
             if isinstance(value, dict):
                 writer.add_scalars(key=key, value=value, step=train_state.step_count)
             else:
                 writer.add_scalar(key=key, value=value, step=train_state.step_count)
 
-        if gpc.config.monitor.alert.get("light_monitor_address", None) and batch_count % 50 == 0:
-            send_heartbeat("train_metrics", infos)
-
         if update_panel:
             # metrics shown with dashboard panels
             panel_metrics = {
                 "step": batch_count,
                 "lr": lr,
                 "num_consumed_tokens": train_state.num_consumed_tokens,
                 "loss": loss.item() - moe_loss.item() if moe_loss is not None else loss.item(),
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/train/utils.py` & `InternEvo-0.4.0.dev20240403/internlm/train/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.3.3.dev20240315/internlm/utils/checkpoint.py` & `InternEvo-0.4.0.dev20240403/internlm/solver/activation_checkpoint.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,23 +2,26 @@
 # -*- encoding: utf-8 -*-
 
 import weakref
 
 import torch
 from torch.utils.checkpoint import check_backward_validity, detach_variable
 
+from internlm.accelerator import get_accelerator
 from internlm.core.context.random import (
     get_current_mode,
     get_states,
     set_mode,
     set_seed_states,
     sync_states,
 )
 
-from .common import get_current_device
+from ..utils.common import get_current_device
+
+internlm_accelerator = get_accelerator()
 
 
 def copy_to_device(obj, device):
     if torch.is_tensor(obj):
         # Notice:
         # When in no_grad context, requires_gard is False after movement
         ret = obj.to(device).detach()
@@ -108,36 +111,36 @@
         bwd_seed_states = get_states(copy=True)
         bwd_current_mode = get_current_mode()
 
         # set the states to what it used to be
         torch.set_rng_state(ctx.fwd_cpu_rng_state)
         for parallel_mode, state in ctx.fwd_seed_states.items():
             set_seed_states(parallel_mode, state)
-        set_mode(ctx.fwd_current_mode)
+        set_mode(ctx.fwd_current_mode, update_rng_current_mode=False)
         if ctx.activation_offload:
             tensors = copy_to_device(tensors, ctx.device)
 
         # Fill in inputs with appropriate saved tensors.
         for i, idx in enumerate(tensor_indices):
             inputs[idx] = tensors[i]
         detached_inputs = detach_variable(tuple(inputs))
         if ctx.had_autocast_in_fwd:
-            with torch.enable_grad(), torch.cuda.amp.autocast():
+            with torch.enable_grad(), internlm_accelerator.amp.autocast():
                 outputs = ctx.run_function(*detached_inputs)
         else:
             with torch.enable_grad():
                 outputs = ctx.run_function(*detached_inputs)
 
         if isinstance(outputs, torch.Tensor):
             outputs = (outputs,)
         # recover the rng states
         torch.set_rng_state(bwd_cpu_rng_state)
         for parallel_mode, state in bwd_seed_states.items():
             set_seed_states(parallel_mode, state)
-        set_mode(bwd_current_mode)
+        set_mode(bwd_current_mode, update_rng_current_mode=False)
 
         # run backward() with only tensor that requires grad
         outputs_with_grad = []
         args_with_grad = []
         for i in range(len(outputs)):
             if torch.is_tensor(outputs[i]) and outputs[i].requires_grad:
                 outputs_with_grad.append(outputs[i])
@@ -231,15 +234,15 @@
             if activation_offload:
                 for arg in args:
                     if torch.is_tensor(arg):
                         arg = arg.to(device=device)
 
             # rerun forward, the inner_pack will store all the activations in storage
             if has_autocast_in_fwd:
-                with torch.enable_grad(), torch.cuda.amp.autocast(), torch.autograd.graph.saved_tensors_hooks(
+                with torch.enable_grad(), internlm_accelerator.amp.autocast(), torch.autograd.graph.saved_tensors_hooks(
                     inner_pack, inner_unpack
                 ):
                     function(*args)
             else:
                 with torch.enable_grad(), torch.autograd.graph.saved_tensors_hooks(inner_pack, inner_unpack):
                     function(*args)
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/utils/common.py` & `InternEvo-0.4.0.dev20240403/internlm/utils/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,18 +10,20 @@
 from datetime import datetime
 from typing import Union
 
 import numpy as np
 import torch
 
 import internlm
+from internlm.accelerator import AcceleratorType, get_accelerator
 from internlm.utils.logger import get_logger
 
 CURRENT_TIME = None
 logger = get_logger(__file__)
+internlm_accelerator = get_accelerator()
 
 
 def parse_args():
     parser = internlm.get_default_parser()
     args = parser.parse_args()
 
     return args
@@ -34,37 +36,39 @@
         raise RuntimeError("get_master_node can only used in Slurm launch!")
     result = subprocess.check_output('scontrol show hostnames "$SLURM_JOB_NODELIST" | head -n 1', shell=True)
     result = result.decode("utf8").strip()
     return result
 
 
 def move_norm_to_cuda(norm: Union[float, torch.Tensor]) -> Union[float, torch.Tensor]:
-    if torch.is_tensor(norm) and norm.device.type != "cuda":
-        norm = norm.to(torch.cuda.current_device())
+    if torch.is_tensor(norm) and norm.device.type != internlm_accelerator.get_backend_name():
+        norm = norm.to(get_current_device())
     return norm
 
 
 def _move_tensor(element):
     if not torch.is_tensor(element):
         # we expecte the data type if a list of dictionaries
-        for item in element:
+        for idx, item in enumerate(element):
             if isinstance(item, dict):
                 for key, value in item.items():
-                    assert not value.is_cuda, "elements are already on devices."
+                    assert value.device.type == "cpu"
                     item[key] = value.to(get_current_device()).detach()
             elif isinstance(item, list):
                 for index, value in enumerate(item):
-                    assert not value.is_cuda, "elements are already on devices."
+                    assert value.device.type == "cpu"
                     item[index] = value.to(get_current_device()).detach()
             elif torch.is_tensor(item):
-                if not item.is_cuda:
-                    item = item.to(get_current_device()).detach()
+                if item.device.type == "cpu":
+                    element[idx] = item.to(get_current_device()).detach()
+            else:
+                assert False, f"{type(item)}, {item}"
     else:
         assert torch.is_tensor(element), f"element should be of type tensor, but got {type(element)}"
-        if not element.is_cuda:
+        if element.device.type == "cpu":
             element = element.to(get_current_device()).detach()
     return element
 
 
 def move_to_device(data):
     if isinstance(data, torch.Tensor):
         data = data.to(get_current_device())
@@ -83,25 +87,25 @@
     return data
 
 
 def get_tensor_norm(norm: Union[float, torch.Tensor], move_to_cuda) -> torch.Tensor:
     if isinstance(norm, float):
         norm = torch.Tensor([norm])
     if move_to_cuda:
-        norm = norm.to(torch.cuda.current_device())
+        norm = norm.to(get_current_device())
     return norm
 
 
 def get_current_device() -> torch.device:
     """
     Returns currently selected device (gpu/cpu).
     If cuda available, return gpu, otherwise return cpu.
     """
-    if torch.cuda.is_available():
-        return torch.device(f"cuda:{torch.cuda.current_device()}")
+    if internlm_accelerator.is_available():
+        return torch.device(f"{internlm_accelerator.current_device_name()}")
     else:
         return torch.device("cpu")
 
 
 def get_batch_size(data):
     if isinstance(data, torch.Tensor):
         return data.size(0)
@@ -140,17 +144,17 @@
     """Set random seed for reproducability."""
     # It is recommended to use this only when inference.
     if seed is not None:
         assert seed > 0
         random.seed(seed)
         np.random.seed(seed)
         torch.manual_seed(seed)
-        torch.cuda.manual_seed(seed)
+        internlm_accelerator.manual_seed(seed)
         # if you are using multi-GPU.
-        torch.cuda.manual_seed_all(seed)
+        internlm_accelerator.manual_seed_all(seed)
 
 
 @contextmanager
 def conditional_context(context_manager, enable=True):
     if enable:
         with context_manager:
             yield
@@ -231,19 +235,19 @@
     ) * num_layers + 6 * global_batch_size * seq_len * hidden_size * vocab_size
 
     tflops = flops_per_iteration / (elapsed_time_per_iter * global_world_size * (10**12))
     return tflops
 
 
 def enable_pytorch_expandable_segments():
-    if torch.__version__ >= "2.1.0":
+    if torch.__version__ >= "2.1.0" and AcceleratorType.GPU == internlm_accelerator.get_accelerator_backend():
         _alloc_setting = "expandable_segments:True"
         if os.getenv("PYTORCH_CUDA_ALLOC_CONF", None) is not None:
             _alloc_setting = os.getenv("PYTORCH_CUDA_ALLOC_CONF") + "," + _alloc_setting
-        torch.cuda.memory._set_allocator_settings(_alloc_setting)
+        internlm_accelerator.memory._set_allocator_settings(_alloc_setting)
     else:
         logger.warning("To support the 'expandable_segments' configuration, please upgrade torch to version 2.1.0.")
 
 
 class DummyProfile:
     """
     Dummy Profile.
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/utils/evaluation.py` & `InternEvo-0.4.0.dev20240403/internlm/eval/evaluation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,164 +1,113 @@
 from contextlib import contextmanager
 
 import torch
 import torch.distributed as dist
 from tqdm import tqdm
 
+from internlm.accelerator import get_accelerator
 from internlm.core.context import ParallelMode
 from internlm.core.context import global_context as gpc
+from internlm.core.scheduler.pipeline_scheduler import get_tensor_shape
 from internlm.model.metrics import AccPerplex, SchedulerMetricHook
+from internlm.utils.common import get_current_device
 
-
-@contextmanager
-def switch_evaluation_no_pipeline_scheduler(trainer, grad_accum_size, metric_hook_list):
-    if not gpc.is_using_parallel_mode(ParallelMode.PIPELINE):
-        prev_data_process_func = trainer.schedule.data_process_func
-        prev_grad_accum_size = trainer.schedule._grad_accum_size
-        prev_metric_hooks = trainer.schedule._hooks
-        try:
-            trainer.schedule.data_process_func = None
-            trainer.schedule._grad_accum_size = grad_accum_size
-            trainer.schedule._hooks = metric_hook_list
-            yield
-        finally:
-            trainer.schedule.data_process_func = prev_data_process_func
-            trainer.schedule._grad_accum_size = prev_grad_accum_size
-            trainer.schedule._hooks = prev_metric_hooks
+internlm_accelerator = get_accelerator()
 
 
 @contextmanager
-def switch_evaluation_pipeline_scheduler(trainer, num_microbatches, tensor_shape, metric_hook_list):
+def switch_evaluation_pipeline_scheduler(trainer):
     if gpc.is_using_parallel_mode(ParallelMode.PIPELINE):
-        pre_data_process_func = trainer.schedule.data_process_func
-        prev_num_microbatches = trainer.schedule.num_microbatches
         prev_tensor_shape = trainer.schedule.tensor_shape
-        prev_metric_hooks = trainer.schedule._hooks
         try:
-            trainer.schedule.data_process_func = None
-            trainer.schedule.num_microbatches = num_microbatches
-            trainer.schedule.tensor_shape = tensor_shape
-            trainer.schedule._hooks = metric_hook_list
+            trainer.schedule.tensor_shape = get_tensor_shape()
             yield
         finally:
-            trainer.schedule.data_process_func = pre_data_process_func
-            trainer.schedule.num_microbatches = prev_num_microbatches
             trainer.schedule.tensor_shape = prev_tensor_shape
-            trainer.schedule._hooks = prev_metric_hooks
 
 
 @contextmanager
-def switch_evaluation_mode():
-    prev_seq = gpc.config.parallel.sequence_parallel
+def switch_evaluation_mode(trainer, metric_hook_list):
     prev_eval = gpc.is_evaluating
+    pre_data_process_func = trainer.schedule.data_process_func
+    prev_metric_hooks = trainer.schedule._hooks
     try:
         gpc.is_evaluating = True
-
-        # when training x.shape is torch.Size([1024, 4096]), linear all gather in dim=0(sequence dim)
-        # but evaluation x.shape is torch.Size([1, 1024, 4096]), gather in dim=0 is error.
-        if gpc.config.parallel["tensor"]["mode"] == "isp":
-            gpc.config.parallel.sequence_parallel = True
-        else:
-            gpc.config.parallel.sequence_parallel = False
+        trainer.schedule.data_process_func = None
+        trainer.schedule._hooks = metric_hook_list
 
         yield
     finally:
-        gpc.config.parallel.sequence_parallel = prev_seq
         gpc.is_evaluating = prev_eval
+        trainer.schedule.data_process_func = pre_data_process_func
+        trainer.schedule._hooks = prev_metric_hooks
 
 
 def evaluate_on_val_dls(
     trainer,
     val_dls,
     writer,
     logger,
     step_count,
     update_panel: bool = False,
     streaming: bool = False,
 ):
-    with switch_evaluation_mode():
-        torch.cuda.empty_cache()
+    val_metric = AccPerplex(
+        device=get_current_device(),
+        tp_pg=gpc.get_group(ParallelMode.TENSOR),
+        dp_pg=gpc.get_group(ParallelMode.DATA),
+    )
+    val_sche_metric_hook = SchedulerMetricHook(metric=val_metric)
+
+    with switch_evaluation_mode(trainer, metric_hook_list=[val_sche_metric_hook]):
+        internlm_accelerator.empty_cache()
         trainer.eval()
         verbose = gpc.is_rank_for_log()
         data_cfg = gpc.config.data
 
         for val_name, val_dl in val_dls.items():
             if not streaming and len(val_dl) == 0 and verbose:
                 logger.info(f"Validation dataset: {val_name} is empty")
                 continue
 
-            val_metric = AccPerplex(
-                device=torch.cuda.current_device(),
-                tp_pg=gpc.get_group(ParallelMode.TENSOR),
-                dp_pg=gpc.get_group(ParallelMode.DATA),
-            )
-            val_sche_metric_hook = SchedulerMetricHook(metric=val_metric)
-
             val_loss = 0
             val_idx = -1
             for val_idx, batch in tqdm(
                 enumerate(val_dl),
                 desc="Val.",
                 total=len(val_dl) if not streaming else None,
                 position=1,
                 disable=not verbose,
                 leave=False,
             ):
                 moe_loss = None
                 with torch.inference_mode():
-                    if gpc.is_using_parallel_mode(ParallelMode.PIPELINE):
-                        total_val_bsz = len(batch[1])
-                        assert total_val_bsz % data_cfg.micro_bsz == 0
-                        num_microbatches = total_val_bsz // data_cfg.micro_bsz
-                        if gpc.config.parallel.sequence_parallel:
-                            sequence_world_size = gpc.get_world_size(ParallelMode.TENSOR)
-                            tensor_shape = torch.Size(
-                                [
-                                    data_cfg.micro_bsz,
-                                    batch[0]["input_ids"].shape[1] // sequence_world_size,
-                                    gpc.config.HIDDEN_SIZE,
-                                ]
-                            )
-                        else:
-                            tensor_shape = torch.Size(
-                                [data_cfg.micro_bsz, batch[0]["input_ids"].shape[1], gpc.config.HIDDEN_SIZE]
-                            )
+                    total_val_bsz = len(batch[1])
+                    assert total_val_bsz % data_cfg.micro_bsz == 0
 
-                        with switch_evaluation_pipeline_scheduler(
-                            trainer=trainer,
-                            num_microbatches=num_microbatches,
-                            tensor_shape=tensor_shape,
-                            metric_hook_list=[val_sche_metric_hook],
-                        ):
+                    if gpc.is_using_parallel_mode(ParallelMode.PIPELINE):
+                        with switch_evaluation_pipeline_scheduler(trainer=trainer):
                             # Compatible for non-moe
                             if hasattr(gpc.config.model, "num_experts"):
                                 _, _, loss, moe_loss = trainer.execute_schedule(
                                     batch, forward_only=True, return_loss=True, return_output_label=False
                                 )
                             else:
                                 _, _, loss = trainer.execute_schedule(
                                     batch, forward_only=True, return_loss=True, return_output_label=False
                                 )
                     else:
-                        total_val_bsz = len(batch[1])
-                        assert total_val_bsz % data_cfg.micro_bsz == 0
-                        grad_accum_size = total_val_bsz // data_cfg.micro_bsz
-                        with switch_evaluation_no_pipeline_scheduler(
-                            trainer=trainer,
-                            grad_accum_size=grad_accum_size,
-                            metric_hook_list=[val_sche_metric_hook],
-                        ):
-                            if hasattr(gpc.config.model, "num_experts"):
-                                _, _, loss, moe_loss = trainer.execute_schedule(
-                                    batch, forward_only=True, return_loss=True, return_output_label=False
-                                )
-                            else:
-                                _, _, loss = trainer.execute_schedule(
-                                    batch, forward_only=True, return_loss=True, return_output_label=False
-                                )
+                        if hasattr(gpc.config.model, "num_experts"):
+                            _, _, loss, moe_loss = trainer.execute_schedule(
+                                batch, forward_only=True, return_loss=True, return_output_label=False
+                            )
+                        else:
+                            _, _, loss = trainer.execute_schedule(
+                                batch, forward_only=True, return_loss=True, return_output_label=False
+                            )
                 if verbose:
                     val_loss += loss.item() - moe_loss.item() if moe_loss is not None else loss.item()
 
             assert val_idx != -1
             dist.barrier()
 
             val_res = val_metric.get_metric()
@@ -186,9 +135,9 @@
                     )
                 else:
                     logger.info(
                         f"Validation on {val_name}: " + " ".join([f"{key}={value}" for key, value in infos.items()])
                     )
 
         trainer.train()
-        torch.cuda.empty_cache()
+        internlm_accelerator.empty_cache()
         dist.barrier()
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/utils/megatron_timers.py` & `InternEvo-0.4.0.dev20240403/internlm/utils/megatron_timers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 #!/usr/bin/env python
 # -*- encoding: utf-8 -*-
 
 import time
 
-import torch
+from internlm.accelerator import get_accelerator
+
+internlm_accelerator = get_accelerator()
 
 
 class _Timer:
     """Timer."""
 
     def __init__(self, name):
         self.name_ = name
         self.elapsed_ = 0.0
         self.started_ = False
         self.start_time = time.time()
-        self.stream = torch.cuda.current_stream()
+        self.stream = internlm_accelerator.current_stream()
 
     def start(self, reset_all=True):
         """Start the timer."""
         # need to reset all timers in a new batch
         if self.name_ == "one-batch" and reset_all is True:
             megatron_timer.reset()
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/utils/parallel.py` & `InternEvo-0.4.0.dev20240403/internlm/utils/parallel.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 #!/usr/bin/env python
 # -*- encoding: utf-8 -*-
 
 import torch.distributed as dist
-from torch import nn
 
 from internlm.core.context import (
     IS_REPLICA_ZERO_PARALLEL,
     IS_TENSOR_DATA_PARALLEL,
     IS_TENSOR_EXPERT_DATA_PARALLEL,
     IS_TENSOR_ZERO_PARALLEL,
     IS_WEIGHT_ZERO_PARALLEL,
     ParallelMode,
 )
 from internlm.core.context import global_context as gpc
-from internlm.core.naive_amp import NaiveAMPModel
 from internlm.model.utils import try_import_RMSNorm
-from internlm.solver.pipeline_utils import partition_uniform
 
 RMSNorm = try_import_RMSNorm()
 
 
 def is_using_sequence_parallel():
     return (
         isinstance(gpc.config.parallel["tensor"], dict)
@@ -116,41 +113,7 @@
         fn_prefix = ""
 
     log_file_name = (
         f"{fn_prefix}dp={gpc.get_local_rank(ParallelMode.DATA)}_"
         f"tp={gpc.get_local_rank(ParallelMode.TENSOR)}_pp={gpc.get_local_rank(ParallelMode.PIPELINE)}"
     )
     return log_file_name
-
-
-def set_model_params_layer_name(model):
-    r"""Set the layer name as an attribute of the model parameters.
-    Args:
-        model (:class:`torch.nn.Module`): A pyTorch model on whose parameters you check the consistency.
-    """
-    pipeline_size = gpc.get_world_size(ParallelMode.PIPELINE)
-    pipeline_rank = gpc.get_local_rank(ParallelMode.PIPELINE)
-    all_parts = partition_uniform(gpc.config.model.num_layers, pipeline_size, gpc.config.model.num_chunks)
-    parts = all_parts[pipeline_rank]
-
-    if not isinstance(model, nn.ModuleList):
-        model = [model]
-
-    for chunk_idx, _chunk in enumerate(model):
-        if isinstance(_chunk, NaiveAMPModel):
-            _chunk = _chunk.model
-        chunk_start = parts[chunk_idx][0]
-        # Create a unique layer name based on the block's class name and index
-        for _, children in _chunk.named_children():
-            if isinstance(children, nn.ModuleList):
-                for idx, block in enumerate(children):
-                    for param_name, param in block.named_parameters():
-                        layer_name = f"{block.__class__.__name__}Block{idx + chunk_start}"
-                        layer_param_name = f"{layer_name}-{param_name}"
-                        param.__setattr__("layer_name", layer_name)
-                        param.__setattr__("param_name", layer_param_name)
-            else:
-                for param_name, param in children.named_parameters():
-                    layer_name = f"{children.__class__.__name__}"
-                    layer_param_name = f"{layer_name}-{param_name}"
-                    param.__setattr__("layer_name", layer_name)
-                    param.__setattr__("param_name", f"{layer_name}-{param_name}")
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/utils/registry.py` & `InternEvo-0.4.0.dev20240403/internlm/utils/registry.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.3.3.dev20240315/internlm/utils/simple_memory_profiler.py` & `InternEvo-0.4.0.dev20240403/internlm/utils/simple_memory_profiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
 import time
 from collections import OrderedDict
 from functools import partial, reduce
 from typing import Any, Dict, List, Tuple
 
-import pyecharts
 import torch
 
 from internlm.core.naive_amp import NaiveAMPModel
+from internlm.utils.common import get_current_device
 
 mb = 1024 * 1024
 
 
 class SimpleMemState:
     """
     A class to represent the memory state of a model layer.
@@ -359,14 +359,16 @@
                 {"name": "os_state", "value": self._os_state_mem_state.total_mem // mb},
                 {"name": "activation", "value": self._activation_mem_max // mb},
             ]
 
             self._render_sunburst_chart(summary_sunburst_data, "summary_sunburst")
 
     def _render_sunburst_chart(self, data: Any, name: str) -> None:
+        import pyecharts
+
         pyecharts.charts.Sunburst(init_opts=pyecharts.options.InitOpts(width="1000px", height="1000px")).add(
             name,
             data_pair=data,
             highlight_policy="ancestor",
             radius=[0, "95%"],
             levels=[
                 {},
@@ -643,27 +645,27 @@
 
     # num_chunks config
     _num_chunks = 1
 
     # init model and optimizer
     if _num_chunks > 1:
         _chunks = [SimpleModel(skip_layer2=idx % 2 == 0) for idx in range(_num_chunks)]
-        _model = torch.nn.ModuleList(_chunks).cuda()
+        _model = torch.nn.ModuleList(_chunks).to(get_current_device())
     else:
-        _model: torch.nn.Module = SimpleModel().cuda()
+        _model: torch.nn.Module = SimpleModel().to(get_current_device())
     _optimizer = torch.optim.Adam(_model.parameters())
 
     # init profiler
     profiler = SimpleMemoryProfiler(_model, _optimizer, "./test_simple_memory_profiler", total_steps=1)
 
     _optimizer.zero_grad()
 
     # inputs
-    x1 = torch.randn((128, 5120)).cuda()
-    x2 = torch.randn((128, 5120)).cuda()
+    x1 = torch.randn((128, 5120)).to(get_current_device())
+    x2 = torch.randn((128, 5120)).to(get_current_device())
     # forward
     out1 = _simple_schedule(_num_chunks, _model, x1)
     out2 = _simple_schedule(_num_chunks, _model, x2)
     # backward
     out1.mean().backward()
     out2.mean().backward()
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/utils/storage_manager.py` & `InternEvo-0.4.0.dev20240403/internlm/utils/storage_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 #!/usr/bin/env python
 # -*- encoding: utf-8 -*-
 
 import multiprocessing
+import os
 
-import dill
+if "USE_DILL_PICKLE" in os.environ:
+    import dill
 
-dill.Pickler.dumps, dill.Pickler.loads = dill.dumps, dill.loads
-multiprocessing.reduction.ForkingPickler = dill.Pickler
-multiprocessing.reduction.dump = dill.dump
+    dill.Pickler.dumps, dill.Pickler.loads = dill.dumps, dill.loads
+    multiprocessing.reduction.ForkingPickler = dill.Pickler
+    multiprocessing.reduction.dump = dill.dump
 
 import asyncio  # noqa: E402  #pylint: disable=wrong-import-position
 import concurrent.futures  # noqa: E402  #pylint: disable=wrong-import-position
 import hashlib  # noqa: E402  #pylint: disable=wrong-import-position
 import io  # noqa: E402  #pylint: disable=wrong-import-position
-import os  # noqa: E402  #pylint: disable=wrong-import-position
 import pickle  # noqa: E402  #pylint: disable=wrong-import-position
 import re  # noqa: E402  #pylint: disable=wrong-import-position
 import socket  # noqa: E402  #pylint: disable=wrong-import-position
 import stat  # noqa: E402  #pylint: disable=wrong-import-position
 from asyncio import (  # noqa: E402  #pylint: disable=wrong-import-position
     InvalidStateError,
 )
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/utils/timeout.py` & `InternEvo-0.4.0.dev20240403/internlm/utils/timeout.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,16 +40,16 @@
 
 timeout_threshold_dict = {
     "initialize_distributed_env": 240,
     "nopp_forward_backward_step": 360,
     "initialize_model": 60,
     "initialize_optimizer": 60,
     "optim_step": 60,
-    "get_train_data_loader": 600,
-    "get_validation_data_loader": 120,
+    "build_train_loader_with_data_type": 600,
+    "build_valid_loader_with_data_type": 120,
     "load_new_batch": 20,
     "record_current_batch_training_metrics": 10,
     "save_checkpoint": 1200,
     "interleaved_forward_backward_step": 600,
     "nointerleaved_forward_backward_step": 600,
 }
```

### Comparing `InternEvo-0.3.3.dev20240315/internlm/utils/utils.py` & `InternEvo-0.4.0.dev20240403/internlm/utils/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.3.3.dev20240315/internlm/utils/writer.py` & `InternEvo-0.4.0.dev20240403/internlm/utils/writer.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,19 @@
 import sys
 import traceback
 from functools import partial
 
 import torch
 from torch.utils.tensorboard import SummaryWriter
 
+from internlm.accelerator import get_accelerator
 from internlm.core.context import global_context as gpc
 
+internlm_accelerator = get_accelerator()
+
 
 def tb_save_run_info(writer, config_lines, global_step=0):
     writer.add_text(tag="cmd", text_string=" ".join(sys.argv[:]), global_step=global_step)
     lines = []
     for line in config_lines:
         if line.strip().startswith("#"):
             continue
@@ -74,15 +77,16 @@
             writer=writer,
             config_lines=config,
             global_step=step_count,
         )
 
     writer.add_text(
         tag=f"mapping_{tb_log_file_name}",
-        text_string=f"file_path={tb_logdir} hostname={socket.gethostname()} device={torch.cuda.current_device()}",
+        text_string=f"file_path={tb_logdir} hostname={socket.gethostname()} \
+                    device={internlm_accelerator.get_device_id()}",
         global_step=step_count,
     )
     writer.add_scaler = partial(writer.add_scalar, new_style=True)
 
     return writer, tb_logdir
```

### Comparing `InternEvo-0.3.3.dev20240315/setup.py` & `InternEvo-0.4.0.dev20240403/setup.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.3.3.dev20240315/tests/common_fixture.py` & `InternEvo-0.4.0.dev20240403/tests/common_fixture.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,28 +2,32 @@
 import random
 import socket
 
 import numpy as np
 import torch
 
 import internlm
+from internlm.accelerator import get_accelerator
 from internlm.core.context import global_context as gpc
 from internlm.core.context.parallel_context import Config
 from internlm.data.utils import unpack_data
 from internlm.initialize.launch import args_sanity_check
 
+internlm_accelerator = get_accelerator()
+
 config_7B = Config(
     dict(
         parallel=dict(
             zero1=dict(size=-1),
             tensor=dict(size=1, mode="mtp"),
             pipeline=dict(size=1, interleaved_overlap=True),
             weight=dict(size=1, overlap=True, memory_pool=True),
         ),
         data=dict(
+            type="tokenized",
             seq_len=2048,
             micro_num=4,
             micro_bsz=2,
             pack_sample_into_one=False,
             min_length=50,
             total_steps=10,
             valid_micro_num=4,
@@ -109,27 +113,27 @@
 
 def build_environment(rank, world_size, free_port, config):
     os.environ["RANK"] = str(rank)
     os.environ["LOCAL_RANK"] = str(rank)
     os.environ["WORLD_SIZE"] = str(world_size)
     os.environ["MASTER_ADDR"] = "localhost"
     os.environ["MASTER_PORT"] = str(free_port)
-    torch.cuda.empty_cache()
+    internlm_accelerator.empty_cache()
     # launcher="torch"
     internlm.launch_from_torch(config=config, seed=1024)
     args_sanity_check()
 
 
 def seed_all(seed, cuda_deterministic=False):
     random.seed(seed)
     np.random.seed(seed)
     torch.manual_seed(seed)
-    if torch.cuda.is_available():
-        torch.cuda.manual_seed(seed)
-        torch.cuda.manual_seed_all(seed)
+    if internlm_accelerator.is_available():
+        internlm_accelerator.manual_seed(seed)
+        internlm_accelerator.manual_seed_all(seed)
     if cuda_deterministic:  # slower, more reproducible
         torch.backends.cudnn.deterministic = True
         torch.backends.cudnn.benchmark = False
     else:
         torch.backends.cudnn.deterministic = False
         torch.backends.cudnn.benchmark = True
```

### Comparing `InternEvo-0.3.3.dev20240315/tests/test_core/test_pipeline.py` & `InternEvo-0.4.0.dev20240403/tests/test_core/test_pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import multiprocessing as mp
 
 import pytest
 import torch
 
+from internlm.accelerator import AcceleratorType, get_accelerator
 from internlm.core.context import ParallelMode
 from internlm.core.context import global_context as gpc
 from internlm.core.context.parallel_context import Config
+from internlm.utils.common import get_current_device
 from tests.test_core.utils import (
     MlpModel,
     MyLoss,
     build_environment,
     init_model_and_optim,
     loose_close,
     seed_all,
@@ -21,15 +23,23 @@
         parallel=dict(
             zero1=dict(size=1, fsdp=False),
             tensor=dict(size=1, mode="mtp"),
             pipeline=dict(size=8, interleaved_overlap=True),
             weight=dict(size=1, overlap=True, memory_pool=True),
         ),
         model_type="INTERNLM",
-        data=dict(seq_len=8, micro_num=16, micro_bsz=1, pack_sample_into_one=False, min_length=0, total_steps=9999),
+        data=dict(
+            type="tokenized",
+            seq_len=8,
+            micro_num=16,
+            micro_bsz=1,
+            pack_sample_into_one=False,
+            min_length=0,
+            total_steps=9999,
+        ),
         model=dict(
             dtype=torch.bfloat16,
             num_chunks=2,
             use_flash_attn=True,
         ),
         resume_tb_folder="",
         tensorboard_folder="",
@@ -68,28 +78,29 @@
         lr_scheduler=dict(
             total_steps=100,
             init_steps=0,
             warmup_ratio=0.01,
             eta_min=1e-5,
             last_epoch=-1,
         ),
+        use_cuda_flash_attn=True,
     )
 )
 
 
 def exam_pipeline_parallel(args):
     # init
     rank, world_size, micro_num, num_chunks, interleaved_overlap = args
     config.data.micro_num = micro_num
     config.model.num_chunks = num_chunks
     config.parallel.pipeline.interleaved_overlap = interleaved_overlap
 
     build_environment(rank, world_size, config)
 
-    device = torch.device(f"cuda:{rank}")
+    device = get_current_device()
     dtype = config.model["dtype"]
     seq_len = gpc.config.data.seq_len
 
     # set seed
     seed_all(1024)
 
     engine, scheduler = init_model_and_optim(32, num_chunks, dtype, micro_num, interleaved_overlap, tensor_shape=[1, 8])
@@ -121,19 +132,30 @@
     # engine.step()
 
     # torch related
     if gpc.is_last_rank(ParallelMode.PIPELINE):
         torch_xs = torch.tensor(x_list).to(device).to(torch.float32)
         torch_ys = torch.tensor(y_list).to(device).to(torch.float32)
         torch_model = MlpModel(0, 32, "torch").to(device)
-        torch_optimizer = torch.optim.AdamW(
+        adam_extra_kwargs = {}
+        if get_accelerator().get_accelerator_backend() == AcceleratorType.NPU:
+            import torch_npu
+
+            internlm_adamw = torch_npu.optim.NpuFusedAdamW
+        else:
+            internlm_adamw = torch.optim.AdamW
+            if torch.__version__ >= "2.1.0":
+                adam_extra_kwargs["fused"] = True
+
+        torch_optimizer = internlm_adamw(
             params=[{"params": torch_model.parameters(), "weight_decay": config.adam.weight_decay}],
             lr=config.adam.lr,
             betas=(config.adam.adam_beta1, config.adam.adam_beta2),
             eps=config.adam.adam_eps,
+            **adam_extra_kwargs,
         )
 
         # check only forward logits
         first_output = output_list[0]
         for i in range(1, 10):
             assert torch.equal(first_output, output_list[i])
```

### Comparing `InternEvo-0.3.3.dev20240315/tests/test_core/utils.py` & `InternEvo-0.4.0.dev20240403/tests/test_core/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,22 +2,30 @@
 
 import numpy as np
 import torch
 from torch import nn
 from torch.testing import assert_close
 
 import internlm
+from internlm.accelerator import get_accelerator
 from internlm.core.context import ParallelMode
 from internlm.core.context import global_context as gpc
 from internlm.core.engine import Engine
 from internlm.core.gradient_handler import PipelineSharedModuleGradientHandler
-from internlm.core.scheduler import InterleavedPipelineScheduler, NonPipelineScheduler, PipelineScheduler
+from internlm.core.scheduler import (
+    InterleavedPipelineScheduler,
+    NonPipelineScheduler,
+    PipelineScheduler,
+)
 from internlm.model.metrics import SchedulerMetricHook
 from internlm.solver.pipeline_utils import partition_uniform
 from internlm.train import initialize_optimizer
+from internlm.utils.common import get_current_device
+
+internlm_accelerator = get_accelerator()
 
 
 class MlpModel(nn.Module):
     """
     Custom model
     """
 
@@ -29,15 +37,15 @@
         self.embedding = embedding
 
     def forward(
         self, hidden_states=None, cu_seqlens=None, input_ids=None, indexes=None, inference_params=None
     ):  # pylint: disable=W0613
         if self.model_type != "torch" and self.part[0] != 0:
             input_ids = hidden_states
-
+        
         # Simulate Embedding.
         if self.embedding:
             if len(input_ids.shape) == 2:
                 input_ids = input_ids.view(-1, 8)
             elif len(input_ids.shape) == 3:
                 input_ids = input_ids.view(input_ids.shape(0), -1, 8)
 
@@ -142,15 +150,15 @@
     import os
 
     os.environ["RANK"] = str(rank)
     os.environ["LOCAL_RANK"] = str(rank)
     os.environ["WORLD_SIZE"] = str(world_size)
     os.environ["MASTER_ADDR"] = "127.0.0.1"
     os.environ["MASTER_PORT"] = "33333"
-    torch.cuda.empty_cache()
+    internlm_accelerator.empty_cache()
     # launcher="torch"
     internlm.launch_from_torch(config=config, seed=1024)
 
 
 def loose_close(a, b, dtype: torch.dtype = torch.float32):
     if dtype is torch.float32:
         rtol = 1.3e-6
@@ -166,17 +174,17 @@
     assert_close(a, b, rtol=rtol, atol=atol)
 
 
 def seed_all(seed, cuda_deterministic=False):
     random.seed(seed)
     np.random.seed(seed)
     torch.manual_seed(seed)
-    if torch.cuda.is_available():
-        torch.cuda.manual_seed(seed)
-        torch.cuda.manual_seed_all(seed)
+    if internlm_accelerator.is_available():
+        internlm_accelerator.manual_seed(seed)
+        internlm_accelerator.manual_seed_all(seed)
     if cuda_deterministic:  # slower, more reproducible
         torch.backends.cudnn.deterministic = True
         torch.backends.cudnn.benchmark = False
     else:
         torch.backends.cudnn.deterministic = False
         torch.backends.cudnn.benchmark = True
 
@@ -188,15 +196,15 @@
     all_parts = partition_uniform(num_layers, pipeline_size, num_chunks)
     parts = all_parts[pipeline_rank]
     if gpc.is_rank_for_log():
         print(f"The layer sharding is {all_parts}.", flush=True)
 
     models = []
     for start, end in parts:
-        models.append(MlpModel(start, end, embedding=embedding).cuda())
+        models.append(MlpModel(start, end, embedding=embedding).to(get_current_device()))
     torch.distributed.barrier()
     if len(models) == 1:
         model = models[0]
     else:
         model = nn.ModuleList(models)
 
     return model
```

### Comparing `InternEvo-0.3.3.dev20240315/tests/test_training/7B_check_acc.py` & `InternEvo-0.4.0.dev20240403/tests/test_training/7B_check_acc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+import os
+
 JOB_NAME = "7b_train"
 DO_ALERT = False
 
 SEQ_LEN = 2048
 HIDDEN_SIZE = 4096
 NUM_ATTENTION_HEAD = 32
 MLP_RATIO = 8 / 3
 NUM_LAYER = 32
 VOCAB_SIZE = 103168
 
-MODEL_ONLY_FOLDER = "/mnt/petrelfs/share/quailty_assurance/7B_model_weights_ckpt/init"
+MODEL_ONLY_FOLDER = os.path.join(os.environ["share_path"], "quailty_assurance/7B_model_weights_ckpt/init")
 # Ckpt folder format:
 # fs: 'local:/mnt/nfs/XXX'
 # SAVE_CKPT_FOLDER = "local:llm_ckpts_0925_9"
 # LOAD_CKPT_FOLDER = "local:llm_ckpts/49"
 
 # boto3 Ckpt folder format:
 # import os
@@ -26,15 +28,15 @@
     # save_ckpt_folder=SAVE_CKPT_FOLDER,  # Path to save training ckpt.
     # load_ckpt_folder= dict(path=MODEL_ONLY_FOLDER, content=["model"], ckpt_type="normal"),
     # load_ckpt_folder="local:llm_ckpts/",
     # # 'load_ckpt_info' setting guide:
     # # 1. the 'path' indicate ckpt path,
     # # 2. the 'content‘ means what states will be loaded, support: "model", "sampler", "optimizer", "scheduler", "all"
     # # 3. the ’ckpt_type‘ means the type of checkpoint to be loaded, now only 'normal' type is supported.
-    load_ckpt_info=dict(path=MODEL_ONLY_FOLDER, content=("model",), ckpt_type="internlm"),
+    load_ckpt_info=dict(path=MODEL_ONLY_FOLDER, content=("model",), ckpt_type="internevo"),
     # checkpoint_every=CHECKPOINT_EVERY,
     # async_upload=True,  # async ckpt upload. (only work for boto3 ckpt)
     # async_upload_tmp_folder="/dev/shm/internlm_tmp_ckpt/",  # path for temporarily files during asynchronous upload.
     # oss_snapshot_freq=int(CHECKPOINT_EVERY / 2),  # snapshot ckpt save frequency.
 )
 
 TRAIN_FOLDER = "/path/to/dataset"
@@ -80,15 +82,15 @@
     # the number of overflows before decreasing loss scale, defaults to 2
     hysteresis=2,
 )
 
 hybrid_zero_optimizer = dict(
     # Enable low_level_optimzer overlap_communication
     overlap_sync_grad=True,
-    overlap_sync_param=True,
+    overlap_sync_param=False,
     # bucket size for nccl communication params
     reduce_bucket_size=512 * 1024 * 1024,
     # grad clipping
     clip_grad_norm=1.0,
 )
 
 loss = dict(
@@ -144,18 +146,18 @@
         For smaller models, it is usually a better choice to split the parameters within nodes with a setting <= 8.
 pipeline parallel (dict):
     1. size: int, the size of pipeline parallel.
     2. interleaved_overlap: bool, enable/disable communication overlap when using interleaved pipeline scheduler.
 tensor parallel: tensor parallel size, usually the number of GPUs per node.
 """
 parallel = dict(
-    zero1=dict(size=8, fsdp=False),
-    tensor=1,
+    zero1=dict(size=8),
+    tensor=dict(size=1, mode="mtp"),
     pipeline=dict(size=1, interleaved_overlap=True),
-    sequence_parallel=False,
+    weight=dict(size=1, overlap=True, memory_pool=True),
 )
 
 cudnn_deterministic = False
 cudnn_benchmark = False
 
 monitor = dict(
     # feishu alert configs
```

### Comparing `InternEvo-0.3.3.dev20240315/tests/test_training/7B_check_init.py` & `InternEvo-0.4.0.dev20240403/tests/test_training/7B_check_init.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     # the number of overflows before decreasing loss scale, defaults to 2
     hysteresis=2,
 )
 
 hybrid_zero_optimizer = dict(
     # Enable low_level_optimzer overlap_communication
     overlap_sync_grad=True,
-    overlap_sync_param=True,
+    overlap_sync_param=False,
     # bucket size for nccl communication params
     reduce_bucket_size=512 * 1024 * 1024,
     # grad clipping
     clip_grad_norm=1.0,
 )
 
 loss = dict(
@@ -153,18 +153,18 @@
         For smaller models, it is usually a better choice to split the parameters within nodes with a setting <= 8.
 pipeline parallel (dict):
     1. size: int, the size of pipeline parallel.
     2. interleaved_overlap: bool, enable/disable communication overlap when using interleaved pipeline scheduler.
 tensor parallel: tensor parallel size, usually the number of GPUs per node.
 """
 parallel = dict(
-    zero1=dict(size=1, fsdp=False),
-    tensor=4,
+    zero1=dict(size=-1),
+    tensor=dict(size=2, mode="mtp"),
     pipeline=dict(size=2, interleaved_overlap=True),
-    sequence_parallel=False,
+    weight=dict(size=1, overlap=True, memory_pool=True),
 )
 
 cudnn_deterministic = False
 cudnn_benchmark = False
 
 monitor = dict(
     # feishu alert configs
```

### Comparing `InternEvo-0.3.3.dev20240315/tests/test_training/test_forward_output_no_fa.py` & `InternEvo-0.4.0.dev20240403/tests/test_training/test_forward_output_no_fa.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,53 +4,59 @@
 import socket
 
 import numpy as np
 import pytest
 import torch
 
 import internlm
+from internlm.accelerator import get_accelerator
 from internlm.core.context import ParallelMode
 from internlm.core.context import global_context as gpc
 from internlm.core.context.parallel_context import Config
+from internlm.data import build_train_loader_with_data_type
 from internlm.initialize.launch import args_sanity_check
-from internlm.model.loss import FlashGPTLMLoss
+from internlm.model.losses import FlashGPTLMLoss
 from internlm.model.metrics import AccPerplex, SchedulerMetricHook
-from internlm.train import get_train_data_loader, initialize_model, initialize_optimizer
+from internlm.train import initialize_model, initialize_optimizer
+from internlm.utils.common import get_current_device
 from internlm.utils.logger import get_logger
 
 logger = get_logger(__file__)
+internlm_accelerator = get_accelerator()
 
 TOTAL_STEPS = 1
 config = Config(
     dict(
         parallel=dict(
             zero1=dict(size=-1),
             tensor=dict(size=1, mode="mtp"),
             pipeline=dict(size=1, interleaved_overlap=True),
             weight=dict(size=1, overlap=True, memory_pool=True),
         ),
         data=dict(
+            type="tokenized",
             seq_len=2048,
             micro_num=4,
             micro_bsz=2,
             pack_sample_into_one=False,
             min_length=50,
             total_steps=TOTAL_STEPS,
             valid_micro_num=4,
             valid_every=300,
             rampup_batch_size=None,
             diag_outlier_ratio=1.1,
+            use_packed_dataset=False,
         ),
         model=dict(
             checkpoint=True,
             num_attention_heads=32,
             embed_split_hidden=True,
             vocab_size=103168,
             embed_grad_scale=1,
-            parallel_output=True,
+            parallel_output=False,
             hidden_size=4096,
             num_layers=32,
             mlp_ratio=8 / 3,
             apply_post_layer_norm=False,
             dtype="torch.bfloat16",
             norm_type="rmsnorm",
             layer_norm_epsilon=1e-5,
@@ -100,14 +106,15 @@
         ckpt=dict(
             enable_save_ckpt=False,
             auto_resume=False,
         ),
         loss=dict(
             label_smoothing=0,
         ),
+        use_cuda_flash_attn=True,
     )
 )
 
 
 def find_free_port():
     with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
         s.bind(("", 0))
@@ -116,27 +123,27 @@
 
 def build_environment(rank, world_size, free_port, config):
     os.environ["RANK"] = str(rank)
     os.environ["LOCAL_RANK"] = str(rank)
     os.environ["WORLD_SIZE"] = str(world_size)
     os.environ["MASTER_ADDR"] = "localhost"
     os.environ["MASTER_PORT"] = str(free_port)
-    torch.cuda.empty_cache()
+    internlm_accelerator.empty_cache()
     # launcher="torch"
     internlm.launch_from_torch(config=config, seed=1024)
     args_sanity_check()
 
 
 def seed_all(seed, cuda_deterministic=False):
     random.seed(seed)
     np.random.seed(seed)
     torch.manual_seed(seed)
-    if torch.cuda.is_available():
-        torch.cuda.manual_seed(seed)
-        torch.cuda.manual_seed_all(seed)
+    if internlm_accelerator.is_available():
+        internlm_accelerator.manual_seed(seed)
+        internlm_accelerator.manual_seed_all(seed)
     if cuda_deterministic:  # slower, more reproducible
         torch.backends.cudnn.deterministic = True
         torch.backends.cudnn.benchmark = False
     else:
         torch.backends.cudnn.deterministic = False
         torch.backends.cudnn.benchmark = True
 
@@ -158,22 +165,22 @@
     # set seed
     seed_all(1024)
 
     # initialize model
     model = initialize_model()
 
     # initialize loss function
-    criterion = FlashGPTLMLoss(parallel_output=True, label_smoothing=gpc.config.loss.label_smoothing)
+    criterion = FlashGPTLMLoss(parallel_output=False, label_smoothing=gpc.config.loss.label_smoothing)
 
     optimizer, beta2_scheduler, lr_scheduler = initialize_optimizer(model=model)
 
-    train_dl, dataset_types = get_train_data_loader(num_worker=0)
+    train_dl, dataset_types = build_train_loader_with_data_type()
 
     metric = AccPerplex(
-        device=torch.cuda.current_device(),
+        device=get_current_device(),
         tp_pg=gpc.get_group(ParallelMode.TENSOR),
         dp_pg=gpc.get_group(ParallelMode.DATA),
         dataset_types=dataset_types,
     )
 
     scheduler_hooks = [
         SchedulerMetricHook(
@@ -226,15 +233,15 @@
             max_diff, index_max_diff = (tensor1 - tensor2).abs().max(dim=0)
             max_diff = max_diff.item()
             index_max_diff = index_max_diff.item()
             rtol = max_diff / abs(tensor2[index_max_diff])
             logger.info(
                 f"The relative error is {rtol}. Between {tensor1[index_max_diff]} and {tensor2[index_max_diff]}"
             )
-            assert rtol < 1e-5, f"The relative error is {rtol}"
+            assert False, f"The relative error is {rtol}"
 
 
 def test_output():
     free_port = find_free_port()
     ctx = mp.get_context("spawn")
     with ctx.Pool(processes=8) as pool:
         pool.map(
```

### Comparing `InternEvo-0.3.3.dev20240315/tests/test_training/test_load_ckpt_loss.py` & `InternEvo-0.4.0.dev20240403/tests/test_training/test_load_ckpt_loss.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,67 @@
 import multiprocessing as mp
-import os
-import random
-import shutil
-import socket
-
-import numpy as np
-import pytest
-import torch
-import torch.distributed as dist
-
-import internlm
-from internlm.core.context import ParallelMode
-from internlm.core.context import global_context as gpc
-from internlm.core.context.parallel_context import Config
-from internlm.core.trainer import TrainState
-from internlm.initialize.launch import args_sanity_check
-from internlm.model.loss import FlashGPTLMLoss
-from internlm.model.metrics import AccPerplex, SchedulerMetricHook
-from internlm.train import (
-    get_train_data_loader,
+
+from internlm.accelerator import get_accelerator
+
+backup_ForkingPickler = mp.reduction.ForkingPickler
+backup_dump = mp.reduction.dump
+import os  # noqa: E402  #pylint: disable=wrong-import-position
+import random  # noqa: E402  #pylint: disable=wrong-import-position
+import shutil  # noqa: E402  #pylint: disable=wrong-import-position
+import socket  # noqa: E402  #pylint: disable=wrong-import-position
+
+import numpy as np  # noqa: E402  #pylint: disable=wrong-import-position
+import pytest  # noqa: E402  #pylint: disable=wrong-import-position
+import torch  # noqa: E402  #pylint: disable=wrong-import-position
+import torch.distributed as dist  # noqa: E402  #pylint: disable=wrong-import-position
+
+import internlm  # noqa: E402  #pylint: disable=wrong-import-position
+from internlm.checkpoint import (  # noqa: E402  #pylint: disable=wrong-import-position
+    CheckpointManager,
+)
+from internlm.core.context import (  # noqa: E402  #pylint: disable=wrong-import-position
+    ParallelMode,
+)
+from internlm.core.context import (  # noqa: E402  #pylint: disable=wrong-import-position
+    global_context as gpc,
+)
+from internlm.core.context.parallel_context import (  # noqa: E402  #pylint: disable=wrong-import-position
+    Config,
+)
+from internlm.core.trainer import (  # noqa: E402  #pylint: disable=wrong-import-position
+    TrainState,
+)
+from internlm.data import (  # noqa: E402  #pylint: disable=wrong-import-position
+    build_train_loader_with_data_type,
+)
+from internlm.initialize.launch import (  # noqa: E402  #pylint: disable=wrong-import-position
+    args_sanity_check,
+)
+from internlm.model.losses import (  # noqa: E402  #pylint: disable=wrong-import-position
+    FlashGPTLMLoss,
+)
+from internlm.model.metrics import (  # noqa: E402  #pylint: disable=wrong-import-position
+    AccPerplex,
+    SchedulerMetricHook,
+)
+from internlm.train import (  # noqa: E402  #pylint: disable=wrong-import-position
     initialize_model,
     initialize_optimizer,
     load_new_batch,
 )
-from internlm.utils.common import launch_time
-from internlm.utils.logger import get_logger
-from internlm.utils.model_checkpoint import CheckpointManager
+from internlm.utils.common import (  # noqa: E402  #pylint: disable=wrong-import-position
+    get_current_device,
+    launch_time,
+)
+from internlm.utils.logger import (  # noqa: E402  #pylint: disable=wrong-import-position
+    get_logger,
+)
 
 logger = get_logger(__file__)
+internlm_accelerator = get_accelerator()
 
 TOTAL_STEPS = 10
 temp_folder = "temp_ckpt_for_check_loss"
 config = Config(
     dict(
         parallel=dict(
             zero1=dict(size=-1, fsdp=False),
@@ -52,14 +82,15 @@
             diag_outlier_ratio=1.1,
             train_folder=os.path.join(
                 os.environ["share_path"], "quailty_assurance/0623_scratch_tokenized_filtered/train"
             ),
             valid_folder=os.path.join(
                 os.environ["share_path"], "quailty_assurance/0623_scratch_tokenized_filtered/val"
             ),
+            num_worker=0,
         ),
         model=dict(
             checkpoint=False,
             num_attention_heads=16,
             embed_split_hidden=True,
             vocab_size=103168,
             embed_grad_scale=1,
@@ -119,14 +150,15 @@
             save_ckpt_folder=f"local:{temp_folder}/",
             auto_resume=False,
             checkpoint_every=5,
         ),
         loss=dict(
             label_smoothing=0,
         ),
+        use_cuda_flash_attn=True,
     )
 )
 
 
 def find_free_port():
     with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
         s.bind(("", 0))
@@ -135,27 +167,27 @@
 
 def build_environment(rank, world_size, free_port, config):
     os.environ["RANK"] = str(rank)
     os.environ["LOCAL_RANK"] = str(rank)
     os.environ["WORLD_SIZE"] = str(world_size)
     os.environ["MASTER_ADDR"] = "localhost"
     os.environ["MASTER_PORT"] = str(free_port)
-    torch.cuda.empty_cache()
+    internlm_accelerator.empty_cache()
     # launcher="torch"
     internlm.launch_from_torch(config=config, seed=1024)
     args_sanity_check()
 
 
 def seed_all(seed, cuda_deterministic=False):
     random.seed(seed)
     np.random.seed(seed)
     torch.manual_seed(seed)
-    if torch.cuda.is_available():
-        torch.cuda.manual_seed(seed)
-        torch.cuda.manual_seed_all(seed)
+    if internlm_accelerator.is_available():
+        internlm_accelerator.manual_seed(seed)
+        internlm_accelerator.manual_seed_all(seed)
     if cuda_deterministic:  # slower, more reproducible
         torch.backends.cudnn.deterministic = True
         torch.backends.cudnn.benchmark = False
     else:
         torch.backends.cudnn.deterministic = False
         torch.backends.cudnn.benchmark = True
 
@@ -165,15 +197,15 @@
     rank, world_size, train_round, free_port = args
     build_environment(rank, world_size, free_port, config)
     total_steps = 6
 
     if train_round == 1:
         gpc.config.ckpt.enable_save_ckpt = False
         gpc.config.ckpt._add_item(
-            "load_ckpt_info", dict(path=f"local:{temp_folder}/5/", content=("all",), ckpt_type="internlm")
+            "load_ckpt_info", dict(path=f"local:{temp_folder}/5/", content=("all",), ckpt_type="internevo")
         )
     else:
         assert (
             os.path.exists(temp_folder) is False
         ), f"Error: ckpt temp folder '{temp_folder}' already exists, please check it."
 
     # set seed
@@ -188,15 +220,15 @@
     # initialize model
     model = initialize_model()
 
     # initialize loss function
     criterion = FlashGPTLMLoss(parallel_output=True, label_smoothing=gpc.config.loss.label_smoothing)
 
     # initialize the train and validation data loader
-    train_dl, dataset_types = get_train_data_loader(num_worker=0)
+    train_dl, dataset_types = build_train_loader_with_data_type()
 
     train_state = TrainState(gpc.config, train_dl.batch_sampler)
 
     optimizer, beta2_scheduler, lr_scheduler = initialize_optimizer(model=model)
 
     ckpt_manager = CheckpointManager(
         ckpt_config=gpc.config.ckpt,
@@ -209,15 +241,15 @@
         feishu_address=gpc.config.monitor.alert.feishu_alert_address,
     )
 
     ckpt_manager.try_resume_training(train_state, current_time)
 
     # initialize metric for calculating accuracy and perplexity
     metric = AccPerplex(
-        device=torch.cuda.current_device(),
+        device=get_current_device(),
         tp_pg=gpc.get_group(ParallelMode.TENSOR),
         dp_pg=gpc.get_group(ParallelMode.DATA),
         dataset_types=dataset_types,
     )
 
     # initialize trainer
     scheduler_hooks = [
@@ -277,24 +309,26 @@
             train_state.inf_nan_skip_batches += 1  # record the amount of updating parameters unsuccessfully.
             if -1 in grad_norm_groups.values() and gpc.is_rank_for_log():  # -1 encodes a specific failure case
                 logger.warning(f"Warning: skip parameter update at step {batch_count}.")
 
         ckpt_manager.try_save_checkpoint(train_state)
 
     ckpt_manager.wait_async_upload_finish()
-    torch.cuda.empty_cache()
+    internlm_accelerator.empty_cache()
     dist.barrier()
 
     if gpc.is_rank_for_log():
         if train_round == 1:
             shutil.rmtree(temp_folder)
         return loss.item(), batch
 
 
 def test_loss():
+    mp.reduction.ForkingPickler = backup_ForkingPickler
+    mp.reduction.dump = backup_dump
     results = []
     free_port = find_free_port()
     ctx = mp.get_context("spawn")
     for train_round in range(2):
         with ctx.Pool(processes=8) as pool:
             result = pool.map(
                 train_model,
```

### Comparing `InternEvo-0.3.3.dev20240315/tests/test_training/test_loss.py` & `InternEvo-0.4.0.dev20240403/tests/test_training/test_loss.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 import math
 import os
 
 import pytest
-import torch
 import torch.distributed as dist
 
 import internlm
+from internlm.checkpoint import CheckpointManager
 from internlm.core.context import ParallelMode
 from internlm.core.context import global_context as gpc
 from internlm.core.trainer import TrainState
+from internlm.data import build_train_loader_with_data_type
 from internlm.initialize import initialize_distributed_env
-from internlm.model.loss import FlashGPTLMLoss
+from internlm.model.losses import FlashGPTLMLoss
 from internlm.model.metrics import AccPerplex
 from internlm.train import (
-    get_train_data_loader,
+    get_scheduler_hooks,
+    initialize_isp_communicator,
     initialize_model,
     initialize_optimizer,
-    initialize_isp_communicator,
     load_new_batch,
-    get_scheduler_hooks,
 )
-from internlm.utils.common import BatchSkipper, launch_time
+from internlm.utils.common import BatchSkipper, get_current_device, launch_time
 from internlm.utils.gputest import empty_cache_and_diag
 from internlm.utils.megatron_timers import megatron_timer as timer
-from internlm.utils.model_checkpoint import CheckpointManager
 
 CONFIG_FILE_PATH = os.getenv("CONFIG_FILE_PATH", "./configs/7B_sft.py")
 TOTAL_STEPS = 10
 LOSS_SPIKE_LIMIT = 1.5
 LOSS_DEVIATION_LIMIT = 0.2
 # dp_size = 4
 BASELINE_LOSS_LIST = [
-    11.680583953857422, 
-    7.83256721496582, 
-    6.745327949523926, 
-    6.187380790710449, 
-    5.421087265014648, 
-    5.3960981369018555, 
-    5.090664863586426, 
-    4.77808952331543, 
-    4.6484055519104, 
-    4.634660720825195
+    11.63298511505127,
+    7.826552391052246,
+    6.727715969085693,
+    6.182102680206299,
+    5.395875930786133,
+    5.394404411315918,
+    5.053983688354492,
+    4.741974353790283,
+    4.629222869873047,
+    4.6164231300354,
 ]
+
 cur_loss_list = []
 
 
 def train(
     dp_size: int = 1,
     tp_size: int = 1,
     wp_size: int = 1,
@@ -87,14 +87,15 @@
         assert gpc.config.parallel.get(
             "sequence_parallel", False
         ), "sequence_parallel must be True when enable_sp is True"
     assert gpc.config.parallel["tensor"]["mode"] == tp_mode
 
     # init setting
     gpc.config.data.total_steps = TOTAL_STEPS
+    gpc.config.data.fixed_random_dataset_seqlen = False
     gpc.config.lr_scheduler.total_steps = TOTAL_STEPS
     gpc.config.model_type = model_type
     total_steps = gpc.config.data.total_steps
     skip_batches = gpc.config.data.skip_batches
     label_smoothing = gpc.config.loss.label_smoothing
 
     # update ckpt config
@@ -118,15 +119,15 @@
     # initialize isp communicator
     isp_communicator = initialize_isp_communicator(model)
 
     # initialize loss function
     criterion = FlashGPTLMLoss(parallel_output=True, label_smoothing=label_smoothing)
 
     # initialize the train data loader
-    train_dl, dataset_types = get_train_data_loader(num_worker=4)
+    train_dl, dataset_types = build_train_loader_with_data_type()
 
     # initialize and resume train state
     train_state = TrainState(gpc.config, train_dl.batch_sampler)
 
     optimizer, beta2_scheduler, lr_scheduler = initialize_optimizer(model, isp_communicator)
 
     with open(CONFIG_FILE_PATH, "r") as f:
@@ -143,15 +144,15 @@
     )
 
     # Loading other persistent training states.
     ckpt_manager.try_resume_training(train_state, current_time)
 
     # initialize metric for calculating accuracy and perplexity
     metric = AccPerplex(
-        device=torch.cuda.current_device(),
+        device=get_current_device(),
         tp_pg=gpc.get_group(ParallelMode.TENSOR),
         dp_pg=gpc.get_group(ParallelMode.DATA),
         dataset_types=dataset_types,
     )
 
     # initialize trainer
     trainer, train_dl, _, _ = internlm.initialize_trainer(
@@ -396,8 +397,7 @@
 @pytest.mark.training_internlm2
 def test_training_internlm2():
     # update config file
     global CONFIG_FILE_PATH
     CONFIG_FILE_PATH = "./configs/7B_internlm2.py"
 
     train(dp_size=8, model_type="INTERNLM2_PUBLIC")
-
```

### Comparing `InternEvo-0.3.3.dev20240315/tests/test_training/test_norm_weight.py` & `InternEvo-0.4.0.dev20240403/tests/test_training/test_norm_weight.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,36 +2,39 @@
 import multiprocessing as mp
 import os
 
 import pytest
 import torch
 
 import internlm
+from internlm.accelerator import get_accelerator
 from internlm.core.context import ParallelMode
 from internlm.core.context import global_context as gpc
-from internlm.model.loss import FlashGPTLMLoss
+from internlm.data import build_train_loader_with_data_type
+from internlm.model.losses import FlashGPTLMLoss
 from internlm.model.metrics import AccPerplex
 from internlm.train import (
     get_scheduler_hooks,
-    get_train_data_loader,
     initialize_isp_communicator,
     initialize_model,
     initialize_optimizer,
 )
+from internlm.utils.common import get_current_device
 from internlm.utils.logger import get_logger
 from tests.common_fixture import (
     build_environment,
     config_7B,
     find_free_port,
     load_new_batch,
     seed_all,
 )
 
 logger = get_logger(__file__)
 config = config_7B
+internlm_accelerator = get_accelerator()
 
 
 def compute_rotol(tensor1, tensor2):
     torch.set_printoptions(precision=10)
     max_diff, index_max_diff = (tensor1 - tensor2).abs().max(dim=0)
     max_diff = max_diff.item()
     index_max_diff = index_max_diff.item()
@@ -74,18 +77,18 @@
     isp_communicator = initialize_isp_communicator(model)
 
     # initialize loss function
     criterion = FlashGPTLMLoss(parallel_output=True, label_smoothing=gpc.config.loss.label_smoothing)
 
     optimizer, beta2_scheduler, lr_scheduler = initialize_optimizer(model, isp_communicator)
 
-    train_dl, dataset_types = get_train_data_loader(num_worker=0)
+    train_dl, dataset_types = build_train_loader_with_data_type()
 
     metric = AccPerplex(
-        device=torch.cuda.current_device(),
+        device=get_current_device(),
         tp_pg=gpc.get_group(ParallelMode.TENSOR),
         dp_pg=gpc.get_group(ParallelMode.DATA),
         dataset_types=dataset_types,
     )
 
     trainer, train_dl, _, _ = internlm.initialize_trainer(
         model=model,
@@ -100,15 +103,15 @@
     # transfer the train data loader into train data iterator
     trainer.train()
 
     train_iter = iter(train_dl)
 
     for batch_count in range(total_steps):
         if batch_count % 100 == 0:
-            torch.cuda.empty_cache()
+            internlm_accelerator.empty_cache()
             gc.collect()
 
         # load batch data
         batch, train_iter = load_new_batch(train_dl=train_dl, train_iter=train_iter)
 
         # zero the grads of parameters
         trainer.zero_grad()
@@ -126,15 +129,15 @@
         )
 
         if isp_communicator and isp_communicator.enable_memory_pool:
             isp_communicator.memory_pool.reset_lazy_pools()
 
         trainer.step()
 
-        torch.cuda.reset_peak_memory_stats()
+        internlm_accelerator.reset_peak_memory_stats()
 
     blocks_norm1_list = []
     blocks_norm2_list = []
 
     for block in model.model.blocks:
         blocks_norm1_list.append(block.norm1.weight.detach().to("cpu"))
         blocks_norm2_list.append(block.norm2.weight.detach().to("cpu"))
```

### Comparing `InternEvo-0.3.3.dev20240315/tests/test_training/test_swap_nb_loss_and_gradnorm.py` & `InternEvo-0.4.0.dev20240403/tests/test_training/test_swap_nb_loss_and_gradnorm.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,41 +6,44 @@
 import numpy as np
 import pytest
 import torch
 import torch.distributed as dist
 from tqdm import tqdm
 
 import internlm
+from internlm.accelerator import get_accelerator
 from internlm.core.context import ParallelMode
 from internlm.core.context import global_context as gpc
 from internlm.core.context.parallel_context import Config
+from internlm.data import (
+    build_train_loader_with_data_type,
+    build_valid_loader_with_data_type,
+)
+from internlm.eval.evaluation import switch_evaluation_mode
 from internlm.initialize.launch import args_sanity_check
-from internlm.model.loss import FlashGPTLMLoss
+from internlm.model.losses import FlashGPTLMLoss
 from internlm.model.metrics import AccPerplex, SchedulerMetricHook
-from internlm.train import (
-    get_train_data_loader,
-    get_validation_data_loader,
-    initialize_model,
-    initialize_optimizer,
-)
-from internlm.utils.evaluation import switch_evaluation_no_pipeline_scheduler
+from internlm.train import initialize_model, initialize_optimizer
+from internlm.utils.common import get_current_device
 from internlm.utils.logger import get_logger
 
 logger = get_logger(__file__)
+internlm_accelerator = get_accelerator()
 
 TOTAL_STEPS = 300
 config = Config(
     dict(
         parallel=dict(
             zero1=dict(size=-1),
             tensor=dict(size=1, mode="mtp"),
             pipeline=dict(size=1, interleaved_overlap=True),
             weight=dict(size=1, overlap=True, memory_pool=True),
         ),
         data=dict(
+            type="tokenized",
             seq_len=2048,
             micro_num=4,
             micro_bsz=2,
             pack_sample_into_one=False,
             min_length=50,
             total_steps=TOTAL_STEPS,
             valid_micro_num=4,
@@ -113,60 +116,61 @@
             enable_save_ckpt=False,
             auto_resume=False,
         ),
         loss=dict(
             label_smoothing=0,
         ),
         cudnn_deterministic=True,
+        use_cuda_flash_attn=True,
     )
 )
 
 
 def build_environment(rank, world_size, config):
     os.environ["RANK"] = str(rank)
     os.environ["LOCAL_RANK"] = str(rank)
     os.environ["WORLD_SIZE"] = str(world_size)
     os.environ["MASTER_ADDR"] = "127.0.0.1"
     os.environ["MASTER_PORT"] = "33333"
-    torch.cuda.empty_cache()
+    internlm_accelerator.empty_cache()
     # launcher="torch"
     internlm.launch_from_torch(config=config, seed=1024)
     args_sanity_check()
 
 
 def seed_all(seed, cuda_deterministic=False):
     random.seed(seed)
     np.random.seed(seed)
     torch.manual_seed(seed)
-    if torch.cuda.is_available():
-        torch.cuda.manual_seed(seed)
-        torch.cuda.manual_seed_all(seed)
+    if internlm_accelerator.is_available():
+        internlm_accelerator.manual_seed(seed)
+        internlm_accelerator.manual_seed_all(seed)
     if cuda_deterministic:  # slower, more reproducible
         torch.backends.cudnn.deterministic = True
         torch.backends.cudnn.benchmark = False
     else:
         torch.backends.cudnn.deterministic = False
         torch.backends.cudnn.benchmark = True
 
 
 def evaluate_on_val_dls(
     trainer,
     val_dls,
 ):
-    torch.cuda.empty_cache()
+    internlm_accelerator.empty_cache()
     trainer.eval()
     verbose = gpc.is_rank_for_log()
     data_cfg = gpc.config.data
 
     for _, val_dl in val_dls.items():
         if len(val_dl) == 0 and verbose:
             continue
 
         val_metric = AccPerplex(
-            device=torch.cuda.current_device(),
+            device=get_current_device(),
             tp_pg=gpc.get_group(ParallelMode.TENSOR),
             dp_pg=gpc.get_group(ParallelMode.DATA),
         )
         val_sche_metric_hook = SchedulerMetricHook(metric=val_metric)
 
         val_loss = 0
         val_idx = -1
@@ -177,35 +181,30 @@
             position=1,
             disable=not verbose,
             leave=False,
         ):
             with torch.inference_mode():
                 total_val_bsz = len(batch[1])
                 assert total_val_bsz % data_cfg.micro_bsz == 0
-                grad_accum_size = total_val_bsz // data_cfg.micro_bsz
-                with switch_evaluation_no_pipeline_scheduler(
-                    trainer=trainer,
-                    grad_accum_size=grad_accum_size,
-                    metric_hook_list=[val_sche_metric_hook],
-                ):
+                with switch_evaluation_mode(trainer=trainer, metric_hook_list=[val_sche_metric_hook]):
                     _, _, loss = trainer.execute_schedule(
                         batch, forward_only=True, return_loss=True, return_output_label=False
                     )
 
             if verbose:
                 val_loss += loss.item()
 
         assert val_idx != -1
         dist.barrier()
 
         if verbose and len(val_dl) != 0:
             val_loss = val_loss / (val_idx + 1 + 1e-6)
 
     trainer.train()
-    torch.cuda.empty_cache()
+    internlm_accelerator.empty_cache()
     dist.barrier()
     return val_loss
 
 
 def compute_trimmed_mean(value_list):
     trim = int(0.05 * len(value_list))
     trimmed_list = value_list[trim:-trim]
@@ -269,22 +268,22 @@
     # initialize model
     model = initialize_model()
 
     # initialize loss function
     criterion = FlashGPTLMLoss(parallel_output=True, label_smoothing=gpc.config.loss.label_smoothing)
 
     # initialize the train and validation data loader
-    train_dl, dataset_types = get_train_data_loader(num_worker=0)
-    val_dls = get_validation_data_loader()
+    train_dl, dataset_types = build_train_loader_with_data_type()
+    val_dls = build_valid_loader_with_data_type()
 
     optimizer, beta2_scheduler, lr_scheduler = initialize_optimizer(model=model)
 
     # initialize metric for calculating accuracy and perplexity
     metric = AccPerplex(
-        device=torch.cuda.current_device(),
+        device=get_current_device(),
         tp_pg=gpc.get_group(ParallelMode.TENSOR),
         dp_pg=gpc.get_group(ParallelMode.DATA),
         dataset_types=dataset_types,
     )
 
     # initialize trainer
     scheduler_hooks = [
@@ -365,15 +364,15 @@
             val_result = evaluate_on_val_dls(
                 trainer=trainer,
                 val_dls=val_dls,
             )
             if val_result != 0:
                 val_list.append(val_result)
 
-    torch.cuda.empty_cache()
+    internlm_accelerator.empty_cache()
     dist.barrier()
 
     if gpc.is_rank_for_log():
         check_grad_norm(grad_norm_list)
 
     return rank, loss_list, val_list
```

### Comparing `InternEvo-0.3.3.dev20240315/tests/test_training/train_CI.py` & `InternEvo-0.4.0.dev20240403/tests/test_training/train_CI.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,76 +13,63 @@
 import torch.distributed as dist
 
 script_dir = os.path.dirname(os.path.abspath(__file__))
 project_root = os.path.abspath(os.path.join(script_dir, "../../"))
 sys.path.append(project_root)
 
 import internlm  # noqa: E402
+from internlm.checkpoint import CheckpointManager  # noqa: E402
 from internlm.core.context import ParallelMode  # noqa: E402
 from internlm.core.context import global_context as gpc  # noqa: E402
 from internlm.core.trainer import TrainState  # noqa: E402
+from internlm.data import (  # noqa: E402
+    build_train_loader_with_data_type,
+    build_valid_loader_with_data_type,
+)
+from internlm.eval.evaluation import evaluate_on_val_dls  # noqa: E402
 from internlm.initialize import initialize_distributed_env  # noqa: E402
-from internlm.model.loss import FlashGPTLMLoss  # noqa: E402
+from internlm.model.losses import FlashGPTLMLoss  # noqa: E402
 from internlm.model.metrics import AccPerplex, SchedulerMetricHook  # noqa: E402
 from internlm.monitor import (  # noqa: E402
     initialize_monitor_manager,
     send_alert_message,
 )
 from internlm.monitor.monitor import monitor_manager as mm  # noqa: E402
 from internlm.train import (  # noqa: E402
-    get_train_data_loader,
-    get_validation_data_loader,
     initialize_llm_profile,
     initialize_model,
     initialize_optimizer,
     record_current_batch_training_metrics,
 )
 from internlm.utils.common import (  # noqa: E402
     BatchSkipper,
+    get_current_device,
     get_megatron_flops,
     launch_time,
     parse_args,
 )
-from internlm.utils.evaluation import evaluate_on_val_dls  # noqa: E402
 from internlm.utils.gputest import empty_cache_and_diag  # noqa: E402
-from internlm.utils.logger import get_logger, initialize_uniscale_logger  # noqa: E402
+from internlm.utils.logger import get_logger  # noqa: E402
 from internlm.utils.megatron_timers import megatron_timer as timer  # noqa: E402
-from internlm.utils.model_checkpoint import CheckpointManager  # noqa: E402
 from internlm.utils.parallel import get_parallel_log_file_name  # noqa: E402
 from internlm.utils.simple_memory_profiler import SimpleMemoryProfiler  # noqa: E402
 from internlm.utils.writer import Writer  # noqa: E402
 
 # global llm logger
 logger = get_logger(__file__)
 
 
-def initialize_llm_logger(start_time: str):
-    """
-    Initialize customed uniscale logger.
-
-    Args:
-        start_time (str): The launch time of current training job.
-
-    Returns: The instance of uniscale logger.
-    """
-
-    uniscale_logger = initialize_uniscale_logger(
-        job_name=gpc.config.JOB_NAME, launch_time=start_time, file_name=get_parallel_log_file_name()
-    )
-    if uniscale_logger is not None:
-        global logger
-        logger = uniscale_logger
-
-    return uniscale_logger
-
-
 def check_model_weights(model, ckpt_path, total_equal=False):
     model1_dict = torch.load(ckpt_path, map_location="cuda")
     model2_dict = model.state_dict()
 
+    for key in model2_dict.keys():
+        if key not in model1_dict:
+            assert False, f"Error: The key {key} for current model dose not exist in standard ckpt!"
+
     for key in model1_dict.keys():
         if key in model2_dict:
             tensor1 = model1_dict[key]
             tensor2 = model2_dict[key]
             if total_equal:
                 assert torch.equal(tensor1, tensor2), "model weights are not equal"
             else:
@@ -116,29 +103,26 @@
 
     # get and broadcast current time
     current_time = launch_time()
     objs = [current_time]
     dist.broadcast_object_list(objs, src=0)
     current_time = objs[0]
 
-    # initialize customed llm logger
-    uniscale_logger = initialize_llm_logger(start_time=current_time)
-
     # initialize model
     model = initialize_model()
 
     with open(args.config, "r") as f:
         config_lines = f.readlines()
 
     # initialize loss function
     criterion = FlashGPTLMLoss(parallel_output=True, label_smoothing=label_smoothing)
 
     # initialize the train and validation data loader
-    train_dl, dataset_types = get_train_data_loader(num_worker=4)
-    val_dls = get_validation_data_loader()
+    train_dl, dataset_types = build_train_loader_with_data_type()
+    val_dls = build_valid_loader_with_data_type()
 
     # initialize and resume train state
     train_state = TrainState(gpc.config, train_dl.batch_sampler)
 
     optimizer, beta2_scheduler, lr_scheduler = initialize_optimizer(model=model)
 
     ckpt_manager = CheckpointManager(
@@ -166,15 +150,15 @@
         config=config_lines,
         logger=logger,
         enable_tb=gpc.config.enable_tb,
     )
 
     # initialize metric for calculating accuracy and perplexity
     metric = AccPerplex(
-        device=torch.cuda.current_device(),
+        device=get_current_device(),
         tp_pg=gpc.get_group(ParallelMode.TENSOR),
         dp_pg=gpc.get_group(ParallelMode.DATA),
         dataset_types=dataset_types,
     )
 
     # initialize trainer
     scheduler_hooks = [
@@ -218,17 +202,19 @@
 
     # transfer the train data loader into train data iterator
     # train_iter = iter(train_dl)
 
     # check model init weights
     if hasattr(gpc.config, "CHECK_INIT") and gpc.config.CHECK_INIT == 1:
         ckpt_name = (
-            f"model_tp{gpc.get_local_rank(ParallelMode.TENSOR)}_pp{gpc.get_local_rank(ParallelMode.PIPELINE)}.pt"
+            f"model_dp{gpc.get_local_rank(ParallelMode.DATA)}"
+            f"_tp{gpc.get_local_rank(ParallelMode.TENSOR)}"
+            f"_pp{gpc.get_local_rank(ParallelMode.PIPELINE)}.pt"
         )
-        ckpt_path = os.path.join(os.environ["share_path"], "quailty_assurance/7B_init_8_tp=4_pp=2_ckpt", ckpt_name)
+        ckpt_path = os.path.join(os.environ["share_path"], "quailty_assurance/7B_init_dp=2_tp=2_pp=2_ckpt", ckpt_name)
         check_model_weights(model, ckpt_path, total_equal=True)
 
     with initialize_llm_profile(profiling=args.profiling, start_time=current_time) as prof:
         # start iterating the train data and begin training
         for batch_count in range(train_state.batch_count, total_steps):
             empty_cache_and_diag(batch_count, interval=gpc.config.data.empty_cache_and_diag_interval)
             start_time = time.time()
@@ -313,32 +299,32 @@
                 beta2_scheduler=beta2_scheduler,
                 trainer=trainer,
                 start_time=start_time,
                 loss=loss,
                 moe_loss=moe_loss,
                 grad_norm=grad_norm_groups,
                 metric=metric,
-                update_panel=uniscale_logger is not None,
+                update_panel=False,
             )
 
             timer("one-batch").stop()
 
             # evaluate on validation data loaders
             if valid_every > 0 and train_state.step_count % valid_every == 0:
                 evaluate_on_val_dls(
                     trainer=trainer,
                     val_dls=val_dls,
                     writer=writer,
                     logger=logger,
                     step_count=train_state.step_count,
-                    update_panel=uniscale_logger is not None,
+                    update_panel=False,
                 )
 
             # check model weights
-            if batch_count > 0 and batch_count % 100 == 0:
+            if gpc.is_rank_for_log() and batch_count > 0 and batch_count % 100 == 0:
                 ckpt_path = os.path.join(
                     os.environ["share_path"],
                     "quailty_assurance/7B_model_weights_ckpt",
                     str(batch_count),
                     "model_tp0_pp0.pt",
                 )
                 check_model_weights(model, ckpt_path)
```

