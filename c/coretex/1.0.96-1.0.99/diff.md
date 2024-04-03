# Comparing `tmp/coretex-1.0.96.tar.gz` & `tmp/coretex-1.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coretex-1.0.96.tar", last modified: Wed Mar 27 04:38:39 2024, max compression
+gzip compressed data, was "coretex-1.0.99.tar", last modified: Fri Mar 29 04:41:15 2024, max compression
```

## Comparing `coretex-1.0.96.tar` & `coretex-1.0.99.tar`

### file list

```diff
@@ -1,273 +1,273 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.813193 coretex-1.0.96/
--rw-r--r--   0 runner    (1001) docker     (127)    31740 2024-03-27 04:38:34.000000 coretex-1.0.96/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-03-27 04:38:39.813193 coretex-1.0.96/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-03-27 04:38:34.000000 coretex-1.0.96/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.773193 coretex-1.0.96/coretex/
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.777193 coretex-1.0.96/coretex/_task/
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/_task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/_task/base_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/_task/current_task_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/_task/initialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.777193 coretex-1.0.96/coretex/_task/local/
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/_task/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/_task/local/arg_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/_task/local/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/_task/local/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/_task/local/task_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.777193 coretex-1.0.96/coretex/_task/logging/
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/_task/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/_task/logging/output_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/_task/logging/upload_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.777193 coretex-1.0.96/coretex/_task/remote/
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/_task/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/_task/remote/remote.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.777193 coretex-1.0.96/coretex/_task/worker/
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/_task/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/_task/worker/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/_task/worker/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/_task/worker/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/_task/worker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.777193 coretex-1.0.96/coretex/bioinformatics/
--rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/bioinformatics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.781193 coretex-1.0.96/coretex/bioinformatics/ctx_qiime2/
--rw-r--r--   0 runner    (1001) docker     (127)    22820 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/bioinformatics/ctx_qiime2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/bioinformatics/ctx_qiime2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.781193 coretex-1.0.96/coretex/bioinformatics/sequence_alignment/
--rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/bioinformatics/sequence_alignment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/bioinformatics/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7971 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.781193 coretex-1.0.96/coretex/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.781193 coretex-1.0.96/coretex/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/cli/commands/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/cli/commands/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/cli/commands/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/cli/commands/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.781193 coretex-1.0.96/coretex/cli/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/cli/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/cli/modules/config_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/cli/modules/cron.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/cli/modules/intercept.py
--rw-r--r--   0 runner    (1001) docker     (127)    11656 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/cli/modules/node.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/cli/modules/node_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/cli/modules/project_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/cli/modules/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/cli/modules/update.py
--rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/cli/modules/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/cli/modules/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.781193 coretex-1.0.96/coretex/cli/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/cli/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/cli/resources/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/cli/resources/update_script_template.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.785193 coretex-1.0.96/coretex/codable/
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/codable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8281 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/codable/codable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/codable/descriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.785193 coretex-1.0.96/coretex/entities/
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.785193 coretex-1.0.96/coretex/entities/annotation/
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/annotation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.785193 coretex-1.0.96/coretex/entities/annotation/image/
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/annotation/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/annotation/image/bbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     7629 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/annotation/image/classes_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/annotation/image/coretex_format.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.785193 coretex-1.0.96/coretex/entities/conversion/
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/conversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/conversion/base_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/conversion/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/conversion/converter_processor_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.785193 coretex-1.0.96/coretex/entities/conversion/converters/
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/conversion/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/conversion/converters/city_scape_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/conversion/converters/coco_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/conversion/converters/create_ml_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/conversion/converters/human_segmentation_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/conversion/converters/label_me_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.789193 coretex-1.0.96/coretex/entities/conversion/converters/pascal/
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/conversion/converters/pascal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11973 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/conversion/converters/pascal/instance_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/conversion/converters/pascal/pascal_2012_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/conversion/converters/pascal/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/conversion/converters/voc_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/conversion/converters/yolo_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.789193 coretex-1.0.96/coretex/entities/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/dataset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.789193 coretex-1.0.96/coretex/entities/dataset/computer_vision_dataset/
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/dataset/computer_vision_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/dataset/computer_vision_dataset/computer_vision_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/dataset/computer_vision_dataset/local_computer_vision_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.789193 coretex-1.0.96/coretex/entities/dataset/custom_dataset/
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/dataset/custom_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/dataset/custom_dataset/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/dataset/custom_dataset/custom_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/dataset/custom_dataset/local_custom_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/dataset/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.793193 coretex-1.0.96/coretex/entities/dataset/image_dataset/
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/dataset/image_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/dataset/image_dataset/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/dataset/image_dataset/image_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/dataset/image_dataset/local_image_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     8157 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/dataset/image_dataset/synthetic_image_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.793193 coretex-1.0.96/coretex/entities/dataset/image_segmentation_dataset/
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/dataset/image_segmentation_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/dataset/image_segmentation_dataset/image_segmentation_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/dataset/image_segmentation_dataset/local_image_segmentation_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/dataset/local_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     8484 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/dataset/network_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.793193 coretex-1.0.96/coretex/entities/dataset/sequence_dataset/
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/dataset/sequence_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/dataset/sequence_dataset/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/dataset/sequence_dataset/local_sequence_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/dataset/sequence_dataset/sequence_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/dataset/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/dataset/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.793193 coretex-1.0.96/coretex/entities/model/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9430 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/model/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.793193 coretex-1.0.96/coretex/entities/project/
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/project/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/project/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/project/project_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/project/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.793193 coretex-1.0.96/coretex/entities/sample/
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/sample/any_local_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.797193 coretex-1.0.96/coretex/entities/sample/computer_vision_sample/
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/sample/computer_vision_sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/sample/computer_vision_sample/computer_vision_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/sample/computer_vision_sample/local_computer_vision_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.797193 coretex-1.0.96/coretex/entities/sample/custom_sample/
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/sample/custom_sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/sample/custom_sample/custom_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/sample/custom_sample/custom_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/sample/custom_sample/local_custom_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.797193 coretex-1.0.96/coretex/entities/sample/image_sample/
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/sample/image_sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/sample/image_sample/image_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/sample/image_sample/image_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/sample/image_sample/image_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/sample/image_sample/local_image_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.797193 coretex-1.0.96/coretex/entities/sample/image_segmentation_sample/
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/sample/image_segmentation_sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/sample/image_segmentation_sample/image_segmentation_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/sample/image_segmentation_sample/local_image_segmentation_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/sample/local_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/sample/network_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/sample/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.797193 coretex-1.0.96/coretex/entities/sample/sequence_sample/
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/sample/sequence_sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6123 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/sample/sequence_sample/local_sequence_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/sample/sequence_sample/sequence_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/sample/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.801193 coretex-1.0.96/coretex/entities/secret/
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/secret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/secret/aws_secret.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/secret/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/secret/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/secret/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.801193 coretex-1.0.96/coretex/entities/task_run/
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/task_run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/task_run/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/task_run/execution_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.801193 coretex-1.0.96/coretex/entities/task_run/log/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/task_run/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/task_run/log/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/task_run/log/severity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.801193 coretex-1.0.96/coretex/entities/task_run/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/task_run/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/task_run/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/task_run/metrics/metric_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/task_run/metrics/metric_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.805193 coretex-1.0.96/coretex/entities/task_run/metrics/predefined_metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/task_run/metrics/predefined_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/task_run/metrics/predefined_metrics/cpu_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/task_run/metrics/predefined_metrics/disk_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/task_run/metrics/predefined_metrics/disk_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/task_run/metrics/predefined_metrics/download_speed.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/task_run/metrics/predefined_metrics/gpu_temperature.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/task_run/metrics/predefined_metrics/gpu_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/task_run/metrics/predefined_metrics/ram_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/task_run/metrics/predefined_metrics/swap_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/task_run/metrics/predefined_metrics/upload_speed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.805193 coretex-1.0.96/coretex/entities/task_run/parameter/
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/task_run/parameter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/task_run/parameter/base_list_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/task_run/parameter/base_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/task_run/parameter/parameter_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/task_run/parameter/parameter_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.809193 coretex-1.0.96/coretex/entities/task_run/parameter/parameters/
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/task_run/parameter/parameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/task_run/parameter/parameters/bool_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/task_run/parameter/parameters/dataset_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/task_run/parameter/parameters/enum_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/task_run/parameter/parameters/float_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/task_run/parameter/parameters/imu_vectors_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/task_run/parameter/parameters/int_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/task_run/parameter/parameters/list_dataset_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/task_run/parameter/parameters/list_enum_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/task_run/parameter/parameters/list_float_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/task_run/parameter/parameters/list_int_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/task_run/parameter/parameters/list_model_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/task_run/parameter/parameters/list_str_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/task_run/parameter/parameters/model_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/task_run/parameter/parameters/range_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/task_run/parameter/parameters/str_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/task_run/parameter/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/task_run/status.py
--rw-r--r--   0 runner    (1001) docker     (127)    21477 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/task_run/task_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/entities/task_run/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/folder_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.809193 coretex-1.0.96/coretex/logging/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/logging/formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/logging/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.809193 coretex-1.0.96/coretex/networking/
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/networking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/networking/chunk_upload_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/networking/file_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/networking/network_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    19921 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/networking/network_manager_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8232 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/networking/network_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/networking/network_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/networking/request_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/networking/user_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/networking/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.813193 coretex-1.0.96/coretex/nlp/
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/nlp/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/nlp/token.py
--rw-r--r--   0 runner    (1001) docker     (127)     8052 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/nlp/transcriber.py
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/nlp/transcription.py
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/nlp/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.813193 coretex-1.0.96/coretex/threading/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/threading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/threading/threaded_data_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.813193 coretex-1.0.96/coretex/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/utils/date.py
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/utils/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/utils/hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/utils/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/utils/number.py
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-03-27 04:38:34.000000 coretex-1.0.96/coretex/utils/process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:38:39.813193 coretex-1.0.96/coretex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-03-27 04:38:39.000000 coretex-1.0.96/coretex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9811 2024-03-27 04:38:39.000000 coretex-1.0.96/coretex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 04:38:39.000000 coretex-1.0.96/coretex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-27 04:38:39.000000 coretex-1.0.96/coretex.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-27 04:38:39.000000 coretex-1.0.96/coretex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-27 04:38:39.000000 coretex-1.0.96/coretex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-03-27 04:38:34.000000 coretex-1.0.96/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 04:38:39.813193 coretex-1.0.96/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.441880 coretex-1.0.99/
+-rw-r--r--   0 runner    (1001) docker     (127)    31740 2024-03-29 04:41:08.000000 coretex-1.0.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-03-29 04:41:15.441880 coretex-1.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-03-29 04:41:08.000000 coretex-1.0.99/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.409880 coretex-1.0.99/coretex/
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.409880 coretex-1.0.99/coretex/_task/
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/_task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/_task/base_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/_task/current_task_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/_task/initialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.409880 coretex-1.0.99/coretex/_task/local/
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/_task/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/_task/local/arg_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/_task/local/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/_task/local/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/_task/local/task_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.409880 coretex-1.0.99/coretex/_task/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/_task/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/_task/logging/output_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/_task/logging/upload_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.409880 coretex-1.0.99/coretex/_task/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/_task/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/_task/remote/remote.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.413880 coretex-1.0.99/coretex/_task/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/_task/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/_task/worker/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/_task/worker/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/_task/worker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/_task/worker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.413880 coretex-1.0.99/coretex/bioinformatics/
+-rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/bioinformatics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.413880 coretex-1.0.99/coretex/bioinformatics/ctx_qiime2/
+-rw-r--r--   0 runner    (1001) docker     (127)    22820 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/bioinformatics/ctx_qiime2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/bioinformatics/ctx_qiime2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.413880 coretex-1.0.99/coretex/bioinformatics/sequence_alignment/
+-rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/bioinformatics/sequence_alignment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/bioinformatics/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7971 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.413880 coretex-1.0.99/coretex/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.413880 coretex-1.0.99/coretex/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/cli/commands/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/cli/commands/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/cli/commands/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/cli/commands/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.417880 coretex-1.0.99/coretex/cli/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/cli/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/cli/modules/config_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/cli/modules/cron.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/cli/modules/intercept.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11656 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/cli/modules/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/cli/modules/node_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/cli/modules/project_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/cli/modules/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/cli/modules/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/cli/modules/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/cli/modules/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.417880 coretex-1.0.99/coretex/cli/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/cli/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/cli/resources/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/cli/resources/update_script_template.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.417880 coretex-1.0.99/coretex/codable/
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/codable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8281 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/codable/codable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/codable/descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.417880 coretex-1.0.99/coretex/entities/
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.417880 coretex-1.0.99/coretex/entities/annotation/
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/annotation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.417880 coretex-1.0.99/coretex/entities/annotation/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/annotation/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/annotation/image/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7629 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/annotation/image/classes_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/annotation/image/coretex_format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.417880 coretex-1.0.99/coretex/entities/conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/conversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/conversion/base_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/conversion/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/conversion/converter_processor_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.417880 coretex-1.0.99/coretex/entities/conversion/converters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/conversion/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/conversion/converters/city_scape_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/conversion/converters/coco_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/conversion/converters/create_ml_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/conversion/converters/human_segmentation_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/conversion/converters/label_me_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.421880 coretex-1.0.99/coretex/entities/conversion/converters/pascal/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/conversion/converters/pascal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11973 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/conversion/converters/pascal/instance_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/conversion/converters/pascal/pascal_2012_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/conversion/converters/pascal/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/conversion/converters/voc_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/conversion/converters/yolo_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.421880 coretex-1.0.99/coretex/entities/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/dataset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.421880 coretex-1.0.99/coretex/entities/dataset/computer_vision_dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/dataset/computer_vision_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/dataset/computer_vision_dataset/computer_vision_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/dataset/computer_vision_dataset/local_computer_vision_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.421880 coretex-1.0.99/coretex/entities/dataset/custom_dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/dataset/custom_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/dataset/custom_dataset/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/dataset/custom_dataset/custom_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/dataset/custom_dataset/local_custom_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/dataset/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.421880 coretex-1.0.99/coretex/entities/dataset/image_dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/dataset/image_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/dataset/image_dataset/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/dataset/image_dataset/image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/dataset/image_dataset/local_image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8157 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/dataset/image_dataset/synthetic_image_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.425880 coretex-1.0.99/coretex/entities/dataset/image_segmentation_dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/dataset/image_segmentation_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/dataset/image_segmentation_dataset/image_segmentation_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/dataset/image_segmentation_dataset/local_image_segmentation_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/dataset/local_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8484 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/dataset/network_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.425880 coretex-1.0.99/coretex/entities/dataset/sequence_dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/dataset/sequence_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/dataset/sequence_dataset/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/dataset/sequence_dataset/local_sequence_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/dataset/sequence_dataset/sequence_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/dataset/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/dataset/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.425880 coretex-1.0.99/coretex/entities/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9430 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/model/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.425880 coretex-1.0.99/coretex/entities/project/
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/project/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/project/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/project/project_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/project/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.425880 coretex-1.0.99/coretex/entities/sample/
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/sample/any_local_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.425880 coretex-1.0.99/coretex/entities/sample/computer_vision_sample/
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/sample/computer_vision_sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/sample/computer_vision_sample/computer_vision_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/sample/computer_vision_sample/local_computer_vision_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.425880 coretex-1.0.99/coretex/entities/sample/custom_sample/
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/sample/custom_sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/sample/custom_sample/custom_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/sample/custom_sample/custom_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/sample/custom_sample/local_custom_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.429880 coretex-1.0.99/coretex/entities/sample/image_sample/
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/sample/image_sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/sample/image_sample/image_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/sample/image_sample/image_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/sample/image_sample/image_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/sample/image_sample/local_image_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.429880 coretex-1.0.99/coretex/entities/sample/image_segmentation_sample/
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/sample/image_segmentation_sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/sample/image_segmentation_sample/image_segmentation_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/sample/image_segmentation_sample/local_image_segmentation_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/sample/local_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/sample/network_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/sample/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.429880 coretex-1.0.99/coretex/entities/sample/sequence_sample/
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/sample/sequence_sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6123 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/sample/sequence_sample/local_sequence_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/sample/sequence_sample/sequence_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/sample/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.429880 coretex-1.0.99/coretex/entities/secret/
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/secret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/secret/aws_secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/secret/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/secret/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/secret/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.429880 coretex-1.0.99/coretex/entities/task_run/
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/task_run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/task_run/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/task_run/execution_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.429880 coretex-1.0.99/coretex/entities/task_run/log/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/task_run/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/task_run/log/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/task_run/log/severity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.433880 coretex-1.0.99/coretex/entities/task_run/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/task_run/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/task_run/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/task_run/metrics/metric_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/task_run/metrics/metric_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.433880 coretex-1.0.99/coretex/entities/task_run/metrics/predefined_metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/task_run/metrics/predefined_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/task_run/metrics/predefined_metrics/cpu_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/task_run/metrics/predefined_metrics/disk_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/task_run/metrics/predefined_metrics/disk_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/task_run/metrics/predefined_metrics/download_speed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/task_run/metrics/predefined_metrics/gpu_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/task_run/metrics/predefined_metrics/gpu_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/task_run/metrics/predefined_metrics/ram_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/task_run/metrics/predefined_metrics/swap_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/task_run/metrics/predefined_metrics/upload_speed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.433880 coretex-1.0.99/coretex/entities/task_run/parameter/
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/task_run/parameter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/task_run/parameter/base_list_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/task_run/parameter/base_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/task_run/parameter/parameter_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/task_run/parameter/parameter_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.437880 coretex-1.0.99/coretex/entities/task_run/parameter/parameters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/task_run/parameter/parameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/task_run/parameter/parameters/bool_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/task_run/parameter/parameters/dataset_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/task_run/parameter/parameters/enum_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/task_run/parameter/parameters/float_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/task_run/parameter/parameters/imu_vectors_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/task_run/parameter/parameters/int_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/task_run/parameter/parameters/list_dataset_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/task_run/parameter/parameters/list_enum_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/task_run/parameter/parameters/list_float_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/task_run/parameter/parameters/list_int_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/task_run/parameter/parameters/list_model_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/task_run/parameter/parameters/list_str_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/task_run/parameter/parameters/model_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/task_run/parameter/parameters/range_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/task_run/parameter/parameters/str_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/task_run/parameter/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/task_run/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21477 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/task_run/task_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/entities/task_run/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/folder_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.437880 coretex-1.0.99/coretex/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/logging/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/logging/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.437880 coretex-1.0.99/coretex/networking/
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/networking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/networking/chunk_upload_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/networking/file_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/networking/network_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20550 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/networking/network_manager_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8232 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/networking/network_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/networking/network_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/networking/request_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/networking/user_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/networking/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.441880 coretex-1.0.99/coretex/nlp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/nlp/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/nlp/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8052 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/nlp/transcriber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/nlp/transcription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/nlp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.441880 coretex-1.0.99/coretex/threading/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/threading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/threading/threaded_data_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.441880 coretex-1.0.99/coretex/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/utils/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/utils/hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/utils/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/utils/number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-03-29 04:41:08.000000 coretex-1.0.99/coretex/utils/process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:41:15.441880 coretex-1.0.99/coretex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-03-29 04:41:15.000000 coretex-1.0.99/coretex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9811 2024-03-29 04:41:15.000000 coretex-1.0.99/coretex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 04:41:15.000000 coretex-1.0.99/coretex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-29 04:41:15.000000 coretex-1.0.99/coretex.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-29 04:41:15.000000 coretex-1.0.99/coretex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-29 04:41:15.000000 coretex-1.0.99/coretex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-03-29 04:41:08.000000 coretex-1.0.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 04:41:15.441880 coretex-1.0.99/setup.cfg
```

### Comparing `coretex-1.0.96/LICENSE` & `coretex-1.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/PKG-INFO` & `coretex-1.0.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coretex
-Version: 1.0.96
+Version: 1.0.99
 Summary: A package for AI experiment tracking, infrastructure and dataset management using Coretex.ai platform.
 Author-email: Duško Mirković <dmirkovic@coretex.ai>
 Maintainer-email: Duško Mirković <dmirkovic@coretex.ai>, Igor Perić <igor@coretex.ai>, Jovica Zarić <jzaric@coretex.ai>, Darko Zarić <dzaric@coretex.ai>, Bogdan Tintor <btintor@coretex.ai>, Alex Maslennikov <alex@coretex.ai>
 Project-URL: Homepage, https://coretex.ai
 Project-URL: Documentation, https://docs.coretex.ai/
 Project-URL: Python API, https://coretexpylib.coretex.ai/
 Project-URL: Source, https://github.com/coretex-ai/coretexpylib
```

### Comparing `coretex-1.0.96/README.md` & `coretex-1.0.99/README.md`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/__init__.py` & `coretex-1.0.99/coretex/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/_logger.py` & `coretex-1.0.99/coretex/_logger.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/_task/__init__.py` & `coretex-1.0.99/coretex/_task/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/_task/base_callback.py` & `coretex-1.0.99/coretex/_task/base_callback.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/_task/current_task_run.py` & `coretex-1.0.99/coretex/_task/current_task_run.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/_task/initialization.py` & `coretex-1.0.99/coretex/_task/initialization.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/_task/local/__init__.py` & `coretex-1.0.99/coretex/_task/local/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/_task/local/arg_parser.py` & `coretex-1.0.99/coretex/_task/local/arg_parser.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/_task/local/callback.py` & `coretex-1.0.99/coretex/_task/local/callback.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/_task/local/local.py` & `coretex-1.0.99/coretex/_task/local/local.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/_task/local/task_config.py` & `coretex-1.0.99/coretex/_task/local/task_config.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/_task/logging/__init__.py` & `coretex-1.0.99/coretex/_task/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/_task/logging/output_interceptor.py` & `coretex-1.0.99/coretex/_task/logging/output_interceptor.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/_task/logging/upload_worker.py` & `coretex-1.0.99/coretex/_task/logging/upload_worker.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/_task/remote/__init__.py` & `coretex-1.0.99/coretex/_task/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/_task/remote/remote.py` & `coretex-1.0.99/coretex/_task/remote/remote.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/_task/worker/__init__.py` & `coretex-1.0.99/coretex/_task/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/_task/worker/artifacts.py` & `coretex-1.0.99/coretex/_task/worker/artifacts.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/_task/worker/metrics.py` & `coretex-1.0.99/coretex/_task/worker/metrics.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/_task/worker/utils.py` & `coretex-1.0.99/coretex/_task/worker/utils.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/_task/worker/worker.py` & `coretex-1.0.99/coretex/_task/worker/worker.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/bioinformatics/__init__.py` & `coretex-1.0.99/coretex/bioinformatics/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/bioinformatics/ctx_qiime2/__init__.py` & `coretex-1.0.99/coretex/bioinformatics/ctx_qiime2/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/bioinformatics/ctx_qiime2/utils.py` & `coretex-1.0.99/coretex/bioinformatics/ctx_qiime2/utils.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/bioinformatics/sequence_alignment/__init__.py` & `coretex-1.0.99/coretex/bioinformatics/sequence_alignment/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/cache.py` & `coretex-1.0.99/coretex/cache.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/cli/__init__.py` & `coretex-1.0.99/coretex/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/cli/commands/__init__.py` & `coretex-1.0.99/coretex/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/cli/commands/login.py` & `coretex-1.0.99/coretex/cli/commands/login.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/cli/commands/model.py` & `coretex-1.0.99/coretex/cli/commands/model.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/cli/commands/node.py` & `coretex-1.0.99/coretex/cli/commands/node.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/cli/commands/project.py` & `coretex-1.0.99/coretex/cli/commands/project.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/cli/main.py` & `coretex-1.0.99/coretex/cli/main.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/cli/modules/__init__.py` & `coretex-1.0.99/coretex/cli/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/cli/modules/config_defaults.py` & `coretex-1.0.99/coretex/cli/modules/config_defaults.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/cli/modules/cron.py` & `coretex-1.0.99/coretex/cli/modules/cron.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/cli/modules/intercept.py` & `coretex-1.0.99/coretex/cli/modules/intercept.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/cli/modules/node.py` & `coretex-1.0.99/coretex/cli/modules/node.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/cli/modules/node_mode.py` & `coretex-1.0.99/coretex/cli/modules/node_mode.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/cli/modules/project_utils.py` & `coretex-1.0.99/coretex/cli/modules/project_utils.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/cli/modules/ui.py` & `coretex-1.0.99/coretex/cli/modules/ui.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/cli/modules/update.py` & `coretex-1.0.99/coretex/cli/modules/update.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/cli/modules/user.py` & `coretex-1.0.99/coretex/cli/modules/user.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/cli/modules/utils.py` & `coretex-1.0.99/coretex/cli/modules/utils.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/cli/resources/__init__.py` & `coretex-1.0.99/coretex/cli/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/cli/resources/resources.py` & `coretex-1.0.99/coretex/cli/resources/resources.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/cli/resources/update_script_template.sh` & `coretex-1.0.99/coretex/cli/resources/update_script_template.sh`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/codable/__init__.py` & `coretex-1.0.99/coretex/codable/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/codable/codable.py` & `coretex-1.0.99/coretex/codable/codable.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/codable/descriptor.py` & `coretex-1.0.99/coretex/codable/descriptor.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/configuration.py` & `coretex-1.0.99/coretex/configuration.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/__init__.py` & `coretex-1.0.99/coretex/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/annotation/__init__.py` & `coretex-1.0.99/coretex/entities/annotation/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/annotation/image/__init__.py` & `coretex-1.0.99/coretex/entities/annotation/image/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/annotation/image/bbox.py` & `coretex-1.0.99/coretex/entities/annotation/image/bbox.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/annotation/image/classes_format.py` & `coretex-1.0.99/coretex/entities/annotation/image/classes_format.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/annotation/image/coretex_format.py` & `coretex-1.0.99/coretex/entities/annotation/image/coretex_format.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/conversion/__init__.py` & `coretex-1.0.99/coretex/entities/conversion/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/conversion/base_converter.py` & `coretex-1.0.99/coretex/entities/conversion/base_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/conversion/converter.py` & `coretex-1.0.99/coretex/entities/conversion/converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/conversion/converter_processor_factory.py` & `coretex-1.0.99/coretex/entities/conversion/converter_processor_factory.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/conversion/converters/__init__.py` & `coretex-1.0.99/coretex/entities/conversion/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/conversion/converters/city_scape_converter.py` & `coretex-1.0.99/coretex/entities/conversion/converters/city_scape_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/conversion/converters/coco_converter.py` & `coretex-1.0.99/coretex/entities/conversion/converters/coco_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/conversion/converters/create_ml_converter.py` & `coretex-1.0.99/coretex/entities/conversion/converters/create_ml_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/conversion/converters/human_segmentation_converter.py` & `coretex-1.0.99/coretex/entities/conversion/converters/human_segmentation_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/conversion/converters/label_me_converter.py` & `coretex-1.0.99/coretex/entities/conversion/converters/label_me_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/conversion/converters/pascal/__init__.py` & `coretex-1.0.99/coretex/entities/conversion/converters/pascal/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/conversion/converters/pascal/instance_extractor.py` & `coretex-1.0.99/coretex/entities/conversion/converters/pascal/instance_extractor.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/conversion/converters/pascal/pascal_2012_converter.py` & `coretex-1.0.99/coretex/entities/conversion/converters/pascal/pascal_2012_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/conversion/converters/pascal/shared.py` & `coretex-1.0.99/coretex/entities/conversion/converters/pascal/shared.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/conversion/converters/voc_converter.py` & `coretex-1.0.99/coretex/entities/conversion/converters/voc_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/conversion/converters/yolo_converter.py` & `coretex-1.0.99/coretex/entities/conversion/converters/yolo_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/dataset/__init__.py` & `coretex-1.0.99/coretex/entities/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/dataset/computer_vision_dataset/__init__.py` & `coretex-1.0.99/coretex/entities/dataset/computer_vision_dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/dataset/computer_vision_dataset/computer_vision_dataset.py` & `coretex-1.0.99/coretex/entities/dataset/computer_vision_dataset/computer_vision_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/dataset/computer_vision_dataset/local_computer_vision_dataset.py` & `coretex-1.0.99/coretex/entities/dataset/computer_vision_dataset/local_computer_vision_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/dataset/custom_dataset/__init__.py` & `coretex-1.0.99/coretex/entities/dataset/custom_dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/dataset/custom_dataset/base.py` & `coretex-1.0.99/coretex/entities/dataset/custom_dataset/base.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/dataset/custom_dataset/custom_dataset.py` & `coretex-1.0.99/coretex/entities/dataset/custom_dataset/custom_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/dataset/custom_dataset/local_custom_dataset.py` & `coretex-1.0.99/coretex/entities/dataset/custom_dataset/local_custom_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/dataset/dataset.py` & `coretex-1.0.99/coretex/entities/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/dataset/image_dataset/__init__.py` & `coretex-1.0.99/coretex/entities/dataset/image_dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/dataset/image_dataset/base.py` & `coretex-1.0.99/coretex/entities/dataset/image_dataset/base.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/dataset/image_dataset/image_dataset.py` & `coretex-1.0.99/coretex/entities/dataset/image_dataset/image_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/dataset/image_dataset/local_image_dataset.py` & `coretex-1.0.99/coretex/entities/dataset/image_dataset/local_image_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/dataset/image_dataset/synthetic_image_generator.py` & `coretex-1.0.99/coretex/entities/dataset/image_dataset/synthetic_image_generator.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/dataset/image_segmentation_dataset/__init__.py` & `coretex-1.0.99/coretex/entities/dataset/image_segmentation_dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/dataset/image_segmentation_dataset/image_segmentation_dataset.py` & `coretex-1.0.99/coretex/entities/dataset/image_segmentation_dataset/image_segmentation_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/dataset/image_segmentation_dataset/local_image_segmentation_dataset.py` & `coretex-1.0.99/coretex/entities/dataset/image_segmentation_dataset/local_image_segmentation_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/dataset/local_dataset.py` & `coretex-1.0.99/coretex/entities/dataset/local_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/dataset/network_dataset.py` & `coretex-1.0.99/coretex/entities/dataset/network_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/dataset/sequence_dataset/__init__.py` & `coretex-1.0.99/coretex/entities/dataset/sequence_dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/dataset/sequence_dataset/base.py` & `coretex-1.0.99/coretex/entities/dataset/sequence_dataset/base.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/dataset/sequence_dataset/local_sequence_dataset.py` & `coretex-1.0.99/coretex/entities/dataset/sequence_dataset/local_sequence_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/dataset/sequence_dataset/sequence_dataset.py` & `coretex-1.0.99/coretex/entities/dataset/sequence_dataset/sequence_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/dataset/state.py` & `coretex-1.0.99/coretex/entities/dataset/state.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/dataset/utils.py` & `coretex-1.0.99/coretex/entities/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/model/__init__.py` & `coretex-1.0.99/coretex/entities/model/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/model/model.py` & `coretex-1.0.99/coretex/entities/model/model.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/project/__init__.py` & `coretex-1.0.99/coretex/entities/project/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/project/base.py` & `coretex-1.0.99/coretex/entities/project/base.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/project/project.py` & `coretex-1.0.99/coretex/entities/project/project.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/project/project_type.py` & `coretex-1.0.99/coretex/entities/project/project_type.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/project/task.py` & `coretex-1.0.99/coretex/entities/project/task.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/sample/__init__.py` & `coretex-1.0.99/coretex/entities/sample/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/sample/any_local_sample.py` & `coretex-1.0.99/coretex/entities/sample/any_local_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/sample/computer_vision_sample/__init__.py` & `coretex-1.0.99/coretex/entities/sample/computer_vision_sample/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/sample/computer_vision_sample/computer_vision_sample.py` & `coretex-1.0.99/coretex/entities/sample/computer_vision_sample/computer_vision_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/sample/computer_vision_sample/local_computer_vision_sample.py` & `coretex-1.0.99/coretex/entities/sample/computer_vision_sample/local_computer_vision_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/sample/custom_sample/__init__.py` & `coretex-1.0.99/coretex/entities/sample/custom_sample/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/sample/custom_sample/custom_sample.py` & `coretex-1.0.99/coretex/entities/sample/custom_sample/custom_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/sample/custom_sample/custom_sample_data.py` & `coretex-1.0.99/coretex/entities/sample/custom_sample/custom_sample_data.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/sample/custom_sample/local_custom_sample.py` & `coretex-1.0.99/coretex/entities/sample/custom_sample/local_custom_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/sample/image_sample/__init__.py` & `coretex-1.0.99/coretex/entities/sample/image_sample/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/sample/image_sample/image_format.py` & `coretex-1.0.99/coretex/entities/sample/image_sample/image_format.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/sample/image_sample/image_sample.py` & `coretex-1.0.99/coretex/entities/sample/image_sample/image_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/sample/image_sample/image_sample_data.py` & `coretex-1.0.99/coretex/entities/sample/image_sample/image_sample_data.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/sample/image_sample/local_image_sample.py` & `coretex-1.0.99/coretex/entities/sample/image_sample/local_image_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/sample/image_segmentation_sample/__init__.py` & `coretex-1.0.99/coretex/entities/sample/image_segmentation_sample/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/sample/image_segmentation_sample/image_segmentation_sample.py` & `coretex-1.0.99/coretex/entities/sample/image_segmentation_sample/image_segmentation_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/sample/image_segmentation_sample/local_image_segmentation_sample.py` & `coretex-1.0.99/coretex/entities/sample/image_segmentation_sample/local_image_segmentation_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/sample/local_sample.py` & `coretex-1.0.99/coretex/entities/sample/local_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/sample/network_sample.py` & `coretex-1.0.99/coretex/entities/sample/network_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/sample/sample.py` & `coretex-1.0.99/coretex/entities/sample/sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/sample/sequence_sample/__init__.py` & `coretex-1.0.99/coretex/entities/sample/sequence_sample/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/sample/sequence_sample/local_sequence_sample.py` & `coretex-1.0.99/coretex/entities/sample/sequence_sample/local_sequence_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/sample/sequence_sample/sequence_sample.py` & `coretex-1.0.99/coretex/entities/sample/sequence_sample/sequence_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/sample/utils.py` & `coretex-1.0.99/coretex/entities/sample/utils.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/secret/__init__.py` & `coretex-1.0.99/coretex/entities/secret/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/secret/aws_secret.py` & `coretex-1.0.99/coretex/entities/secret/aws_secret.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/secret/credentials.py` & `coretex-1.0.99/coretex/entities/secret/credentials.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/secret/secret.py` & `coretex-1.0.99/coretex/entities/secret/secret.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/secret/utils.py` & `coretex-1.0.99/coretex/entities/secret/utils.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/task_run/__init__.py` & `coretex-1.0.99/coretex/entities/task_run/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/task_run/artifact.py` & `coretex-1.0.99/coretex/entities/task_run/artifact.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/task_run/execution_type.py` & `coretex-1.0.99/coretex/entities/task_run/execution_type.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/task_run/log/__init__.py` & `coretex-1.0.99/coretex/entities/task_run/log/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/task_run/log/log.py` & `coretex-1.0.99/coretex/entities/task_run/log/log.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/task_run/log/severity.py` & `coretex-1.0.99/coretex/entities/task_run/log/severity.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/task_run/metrics/__init__.py` & `coretex-1.0.99/coretex/entities/task_run/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/task_run/metrics/metric.py` & `coretex-1.0.99/coretex/entities/task_run/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/task_run/metrics/metric_factory.py` & `coretex-1.0.99/coretex/entities/task_run/metrics/metric_factory.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/task_run/metrics/metric_type.py` & `coretex-1.0.99/coretex/entities/task_run/metrics/metric_type.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/task_run/metrics/predefined_metrics/__init__.py` & `coretex-1.0.99/coretex/entities/task_run/metrics/predefined_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/task_run/metrics/predefined_metrics/cpu_usage.py` & `coretex-1.0.99/coretex/entities/task_run/metrics/predefined_metrics/cpu_usage.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/task_run/metrics/predefined_metrics/disk_read.py` & `coretex-1.0.99/coretex/entities/task_run/metrics/predefined_metrics/disk_read.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/task_run/metrics/predefined_metrics/disk_write.py` & `coretex-1.0.99/coretex/entities/task_run/metrics/predefined_metrics/disk_write.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/task_run/metrics/predefined_metrics/download_speed.py` & `coretex-1.0.99/coretex/entities/task_run/metrics/predefined_metrics/download_speed.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/task_run/metrics/predefined_metrics/gpu_temperature.py` & `coretex-1.0.99/coretex/entities/task_run/metrics/predefined_metrics/gpu_temperature.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/task_run/metrics/predefined_metrics/gpu_usage.py` & `coretex-1.0.99/coretex/entities/task_run/metrics/predefined_metrics/gpu_usage.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/task_run/metrics/predefined_metrics/ram_usage.py` & `coretex-1.0.99/coretex/entities/task_run/metrics/predefined_metrics/ram_usage.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/task_run/metrics/predefined_metrics/swap_usage.py` & `coretex-1.0.99/coretex/entities/task_run/metrics/predefined_metrics/swap_usage.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/task_run/metrics/predefined_metrics/upload_speed.py` & `coretex-1.0.99/coretex/entities/task_run/metrics/predefined_metrics/upload_speed.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/task_run/parameter/__init__.py` & `coretex-1.0.99/coretex/entities/task_run/parameter/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/task_run/parameter/base_list_parameter.py` & `coretex-1.0.99/coretex/entities/task_run/parameter/base_list_parameter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/task_run/parameter/base_parameter.py` & `coretex-1.0.99/coretex/entities/task_run/parameter/base_parameter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/task_run/parameter/parameter_factory.py` & `coretex-1.0.99/coretex/entities/task_run/parameter/parameter_factory.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/task_run/parameter/parameter_type.py` & `coretex-1.0.99/coretex/entities/task_run/parameter/parameter_type.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/task_run/parameter/parameters/__init__.py` & `coretex-1.0.99/coretex/entities/task_run/parameter/parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/task_run/parameter/parameters/bool_parameter.py` & `coretex-1.0.99/coretex/entities/task_run/parameter/parameters/bool_parameter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/task_run/parameter/parameters/dataset_parameter.py` & `coretex-1.0.99/coretex/entities/task_run/parameter/parameters/dataset_parameter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/task_run/parameter/parameters/enum_parameter.py` & `coretex-1.0.99/coretex/entities/task_run/parameter/parameters/enum_parameter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/task_run/parameter/parameters/float_parameter.py` & `coretex-1.0.99/coretex/entities/task_run/parameter/parameters/float_parameter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/task_run/parameter/parameters/imu_vectors_parameter.py` & `coretex-1.0.99/coretex/entities/task_run/parameter/parameters/imu_vectors_parameter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/task_run/parameter/parameters/int_parameter.py` & `coretex-1.0.99/coretex/entities/task_run/parameter/parameters/int_parameter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/task_run/parameter/parameters/list_dataset_parameter.py` & `coretex-1.0.99/coretex/entities/task_run/parameter/parameters/list_dataset_parameter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/task_run/parameter/parameters/list_enum_parameter.py` & `coretex-1.0.99/coretex/entities/task_run/parameter/parameters/list_enum_parameter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/task_run/parameter/parameters/list_float_parameter.py` & `coretex-1.0.99/coretex/entities/task_run/parameter/parameters/list_float_parameter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/task_run/parameter/parameters/list_int_parameter.py` & `coretex-1.0.99/coretex/entities/task_run/parameter/parameters/list_int_parameter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/task_run/parameter/parameters/list_model_parameter.py` & `coretex-1.0.99/coretex/entities/task_run/parameter/parameters/list_model_parameter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/task_run/parameter/parameters/list_str_parameter.py` & `coretex-1.0.99/coretex/entities/task_run/parameter/parameters/list_str_parameter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/task_run/parameter/parameters/model_parameter.py` & `coretex-1.0.99/coretex/entities/task_run/parameter/parameters/model_parameter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/task_run/parameter/parameters/range_parameter.py` & `coretex-1.0.99/coretex/entities/task_run/parameter/parameters/range_parameter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/task_run/parameter/parameters/str_parameter.py` & `coretex-1.0.99/coretex/entities/task_run/parameter/parameters/str_parameter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/task_run/parameter/utils.py` & `coretex-1.0.99/coretex/entities/task_run/parameter/utils.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/task_run/status.py` & `coretex-1.0.99/coretex/entities/task_run/status.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/task_run/task_run.py` & `coretex-1.0.99/coretex/entities/task_run/task_run.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/entities/task_run/utils.py` & `coretex-1.0.99/coretex/entities/task_run/utils.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/folder_manager.py` & `coretex-1.0.99/coretex/folder_manager.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/functions.py` & `coretex-1.0.99/coretex/functions.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/logging/__init__.py` & `coretex-1.0.99/coretex/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/logging/formatter.py` & `coretex-1.0.99/coretex/logging/formatter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/logging/logging.py` & `coretex-1.0.99/coretex/logging/logging.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/networking/__init__.py` & `coretex-1.0.99/coretex/networking/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/networking/chunk_upload_session.py` & `coretex-1.0.99/coretex/networking/chunk_upload_session.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/networking/file_data.py` & `coretex-1.0.99/coretex/networking/file_data.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/networking/network_manager.py` & `coretex-1.0.99/coretex/networking/network_manager.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/networking/network_manager_base.py` & `coretex-1.0.99/coretex/networking/network_manager_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,31 +30,34 @@
 import time
 
 import requests
 import requests.adapters
 
 from .utils import RequestBodyType, RequestFormType, logFilesData, logRequestFailure
 from .request_type import RequestType
-from .network_response import NetworkResponse
+from .network_response import NetworkResponse, NetworkRequestError
 from .file_data import FileData
 
 
+REQUEST_TIMEOUT = 5
 MAX_RETRY_COUNT = 5
 LOGIN_ENDPOINT = "user/login"
 REFRESH_ENDPOINT = "user/refresh"
 API_TOKEN_HEADER = "api-token"
 API_TOKEN_KEY = "token"
 REFRESH_TOKEN_KEY = "refresh_token"
 
 RETRY_STATUS_CODES = [
     HTTPStatus.TOO_MANY_REQUESTS,
     HTTPStatus.INTERNAL_SERVER_ERROR,
     HTTPStatus.SERVICE_UNAVAILABLE
 ]
 
+TimeoutType = Optional[Union[int, Tuple[int, int]]]
+
 
 def getDelayBeforeRetry(retryCount: int) -> int:
     # retryCount starts from 0 so we add +1/+2 to start/end
     # to make it have proper delay
 
     start = (retryCount + 1) ** 2
     end   = (retryCount + 2) ** 2
@@ -172,14 +175,15 @@
         endpoint: str,
         requestType: RequestType,
         headers: Optional[Dict[str, str]] = None,
         query: Optional[Dict[str, Any]] = None,
         body: Optional[RequestBodyType] = None,
         files: Optional[RequestFormType] = None,
         auth: Optional[Tuple[str, str]] = None,
+        timeout: Optional[TimeoutType] = REQUEST_TIMEOUT,
         stream: bool = False,
         retryCount: int = 0
     ) -> NetworkResponse:
 
         """
             Sends an HTTP request with provided parameters
             This method is used as a base for all other networkManager methods
@@ -238,14 +242,15 @@
         try:
             rawResponse = self._session.request(
                 requestType.value,
                 url,
                 params = query,
                 data = data,
                 auth = auth,
+                timeout = timeout,
                 files = files,
                 headers = headers
             )
 
             response = NetworkResponse(rawResponse, endpoint)
             if response.hasFailed():
                 logRequestFailure(endpoint, response)
@@ -257,25 +262,25 @@
                 # If we hit rate limiter sleep before retrying the request
                 if response.statusCode == HTTPStatus.TOO_MANY_REQUESTS:
                     delay = getDelayBeforeRetry(retryCount)
                     logging.getLogger("coretexpylib").debug(f">> [Coretex] Waiting for {delay} seconds before retrying failed \"{endpoint}\" request")
 
                     time.sleep(delay)
 
-                return self.request(endpoint, requestType, headers, query, body, files, auth, stream, retryCount + 1)
+                return self.request(endpoint, requestType, headers, query, body, files, auth, timeout, stream, retryCount + 1)
 
             return response
         except BaseException as exception:
             logging.getLogger("coretexpylib").debug(f">> [Coretex] Request failed. Reason \"{exception}\"", exc_info = exception)
 
             if self.shouldRetry(retryCount, None):
                 if self._apiToken is not None:
                     headers[API_TOKEN_HEADER] = self._apiToken
 
-                return self.request(endpoint, requestType, headers, query, body, files, auth, stream, retryCount + 1)
+                return self.request(endpoint, requestType, headers, query, body, files, auth, timeout, stream, retryCount + 1)
 
             raise RequestFailedError(endpoint, requestType)
 
     def post(self, endpoint: str, params: Optional[RequestBodyType] = None) -> NetworkResponse:
         """
             Sends post HTTP request
 
@@ -403,15 +408,25 @@
 
         with ExitStack() as stack:
             filesData = [file.prepareForUpload(stack) for file in files]
 
             headers = self._headers("multipart/form-data")
             del headers["Content-Type"]
 
-            return self.request(endpoint, RequestType.post, headers, body = params, files = filesData)
+            timeout: TimeoutType
+            if len(files) == 0:
+                timeout = REQUEST_TIMEOUT
+            else:
+                response = self.request(endpoint, RequestType.options, timeout = REQUEST_TIMEOUT)
+                if response.hasFailed():
+                    raise NetworkRequestError(response, "Could not establish a connection with the server")
+
+                timeout = None
+
+            return self.request(endpoint, RequestType.post, headers, body = params, files = filesData, timeout = timeout)
 
         # mypy is complaining about missing return statement but this code is unreachable
         # see: https://github.com/python/mypy/issues/7726
         raise RuntimeError("Unreachable")
 
     def authenticate(self, username: str, password: str, storeCredentials: bool = True) -> NetworkResponse:
         """
```

### Comparing `coretex-1.0.96/coretex/networking/network_object.py` & `coretex-1.0.99/coretex/networking/network_object.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/networking/network_response.py` & `coretex-1.0.99/coretex/networking/network_response.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/networking/request_type.py` & `coretex-1.0.99/coretex/networking/request_type.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,8 +23,9 @@
     """
         Represents request types supported by NetworkManager
     """
 
     get = "GET"
     post = "POST"
     put = "PUT"
-    delete = 'DELETE'
+    delete = "DELETE"
+    options = "OPTIONS"
```

### Comparing `coretex-1.0.96/coretex/networking/user_data.py` & `coretex-1.0.99/coretex/networking/user_data.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/networking/utils.py` & `coretex-1.0.99/coretex/networking/utils.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/nlp/__init__.py` & `coretex-1.0.99/coretex/nlp/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/nlp/text.py` & `coretex-1.0.99/coretex/nlp/text.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/nlp/token.py` & `coretex-1.0.99/coretex/nlp/token.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/nlp/transcriber.py` & `coretex-1.0.99/coretex/nlp/transcriber.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/nlp/transcription.py` & `coretex-1.0.99/coretex/nlp/transcription.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/nlp/utils.py` & `coretex-1.0.99/coretex/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/statistics.py` & `coretex-1.0.99/coretex/statistics.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/threading/__init__.py` & `coretex-1.0.99/coretex/threading/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/threading/threaded_data_processor.py` & `coretex-1.0.99/coretex/threading/threaded_data_processor.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/utils/__init__.py` & `coretex-1.0.99/coretex/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/utils/date.py` & `coretex-1.0.99/coretex/utils/date.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/utils/docker.py` & `coretex-1.0.99/coretex/utils/docker.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/utils/file.py` & `coretex-1.0.99/coretex/utils/file.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/utils/hash.py` & `coretex-1.0.99/coretex/utils/hash.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/utils/image.py` & `coretex-1.0.99/coretex/utils/image.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/utils/logs.py` & `coretex-1.0.99/coretex/utils/logs.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/utils/number.py` & `coretex-1.0.99/coretex/utils/number.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex/utils/process.py` & `coretex-1.0.99/coretex/utils/process.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/coretex.egg-info/PKG-INFO` & `coretex-1.0.99/coretex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coretex
-Version: 1.0.96
+Version: 1.0.99
 Summary: A package for AI experiment tracking, infrastructure and dataset management using Coretex.ai platform.
 Author-email: Duško Mirković <dmirkovic@coretex.ai>
 Maintainer-email: Duško Mirković <dmirkovic@coretex.ai>, Igor Perić <igor@coretex.ai>, Jovica Zarić <jzaric@coretex.ai>, Darko Zarić <dzaric@coretex.ai>, Bogdan Tintor <btintor@coretex.ai>, Alex Maslennikov <alex@coretex.ai>
 Project-URL: Homepage, https://coretex.ai
 Project-URL: Documentation, https://docs.coretex.ai/
 Project-URL: Python API, https://coretexpylib.coretex.ai/
 Project-URL: Source, https://github.com/coretex-ai/coretexpylib
```

### Comparing `coretex-1.0.96/coretex.egg-info/SOURCES.txt` & `coretex-1.0.99/coretex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coretex-1.0.96/pyproject.toml` & `coretex-1.0.99/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "coretex"
-version = "1.0.96"
+version = "1.0.99"
 authors = [
   { name="Duško Mirković", email="dmirkovic@coretex.ai" }
 ]
 maintainers = [
   { name="Duško Mirković", email="dmirkovic@coretex.ai" },
   { name="Igor Perić", email="igor@coretex.ai" },
   { name="Jovica Zarić", email="jzaric@coretex.ai" },
```

