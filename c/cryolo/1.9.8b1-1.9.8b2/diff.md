# Comparing `tmp/cryolo-1.9.8b1.tar.gz` & `tmp/cryolo-1.9.8b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryolo-1.9.8b1.tar", last modified: Tue Mar 26 15:23:19 2024, max compression
+gzip compressed data, was "cryolo-1.9.8b2.tar", last modified: Wed Apr  3 13:02:06 2024, max compression
```

## Comparing `cryolo-1.9.8b1.tar` & `cryolo-1.9.8b2.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2024-03-26 15:23:19.487782 cryolo-1.9.8b1/
--rw-r--r--   0 twagner  (22293) domain users (32000)    17704 2023-02-09 08:33:23.000000 cryolo-1.9.8b1/.gitignore
--rw-r--r--   0 twagner  (22293) domain users (32000)      605 2022-08-09 07:16:57.000000 cryolo-1.9.8b1/.gitlab-ci.yml
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2024-03-26 15:23:19.475782 cryolo-1.9.8b1/.idea/
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2024-03-26 15:23:19.479781 cryolo-1.9.8b1/.idea/codeStyles/
--rw-r--r--   0 twagner  (22293) domain users (32000)      149 2018-12-11 09:23:01.000000 cryolo-1.9.8b1/.idea/codeStyles/codeStyleConfig.xml
--rw-r--r--   0 twagner  (22293) domain users (32000)      649 2022-08-09 07:16:57.000000 cryolo-1.9.8b1/Dockerfile
--rw-r--r--   0 twagner  (22293) domain users (32000)     6596 2019-09-10 13:28:55.000000 cryolo-1.9.8b1/LICENSE
--rw-r--r--   0 twagner  (22293) domain users (32000)       57 2022-08-09 07:16:57.000000 cryolo-1.9.8b1/MANIFEST.in
--rw-r--r--   0 twagner  (22293) domain users (32000)     1750 2024-03-26 15:23:19.487782 cryolo-1.9.8b1/PKG-INFO
--rw-r--r--   0 twagner  (22293) domain users (32000)      869 2022-08-11 12:21:51.000000 cryolo-1.9.8b1/README.md
--rw-r--r--   0 twagner  (22293) domain users (32000)     6593 2022-08-09 07:16:57.000000 cryolo-1.9.8b1/changelog.txt
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2024-03-26 15:23:19.479781 cryolo-1.9.8b1/cryolo/
--rw-r--r--   0 twagner  (22293) domain users (32000)    28327 2024-03-26 15:04:22.000000 cryolo-1.9.8b1/cryolo/CoordsIO.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     2187 2024-03-26 15:04:22.000000 cryolo-1.9.8b1/cryolo/ExtendedModelCheckpoint.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     3325 2024-03-26 15:04:22.000000 cryolo-1.9.8b1/cryolo/MultiGPUModelCheckpoint.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     3475 2024-03-26 15:04:22.000000 cryolo-1.9.8b1/cryolo/SGDRSchedular.py
--rw-r--r--   0 twagner  (22293) domain users (32000)      162 2024-03-26 15:23:14.000000 cryolo-1.9.8b1/cryolo/__init__.py
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2024-03-26 15:23:19.483782 cryolo-1.9.8b1/cryolo/augmentation/
--rw-r--r--   0 twagner  (22293) domain users (32000)      877 2024-03-26 15:04:22.000000 cryolo-1.9.8b1/cryolo/augmentation/AddConstantAugmentation.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     1436 2024-03-26 15:04:22.000000 cryolo-1.9.8b1/cryolo/augmentation/AdditiveGaussianNoiseAugmentation.py
--rw-r--r--   0 twagner  (22293) domain users (32000)      298 2024-03-26 15:04:22.000000 cryolo-1.9.8b1/cryolo/augmentation/AugmentationMethod.py
--rw-r--r--   0 twagner  (22293) domain users (32000)      895 2024-03-26 15:04:22.000000 cryolo-1.9.8b1/cryolo/augmentation/AverageBlurAugmentation.py
--rw-r--r--   0 twagner  (22293) domain users (32000)      980 2024-03-26 15:04:22.000000 cryolo-1.9.8b1/cryolo/augmentation/ContrastNormalizationAugmentation.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     2128 2024-03-26 15:04:22.000000 cryolo-1.9.8b1/cryolo/augmentation/CustomRotationAugmentation.py
--rw-r--r--   0 twagner  (22293) domain users (32000)      995 2024-03-26 15:04:22.000000 cryolo-1.9.8b1/cryolo/augmentation/DropoutAugmentation.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     1828 2024-03-26 15:04:22.000000 cryolo-1.9.8b1/cryolo/augmentation/FlipAugmentation.py
--rw-r--r--   0 twagner  (22293) domain users (32000)      957 2024-03-26 15:04:22.000000 cryolo-1.9.8b1/cryolo/augmentation/GaussBlurAugmentation.py
--rw-r--r--   0 twagner  (22293) domain users (32000)      851 2024-03-26 15:04:22.000000 cryolo-1.9.8b1/cryolo/augmentation/MultiplyAugmentation.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     1979 2024-03-26 15:04:22.000000 cryolo-1.9.8b1/cryolo/augmentation/Rot90Augmentation.py
--rw-r--r--   0 twagner  (22293) domain users (32000)        0 2022-08-09 07:16:57.000000 cryolo-1.9.8b1/cryolo/augmentation/__init__.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     3567 2024-03-26 15:04:22.000000 cryolo-1.9.8b1/cryolo/augmentation/augmentation.py
--rw-r--r--   0 twagner  (22293) domain users (32000)    20749 2024-03-26 15:04:22.000000 cryolo-1.9.8b1/cryolo/backend.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     1156 2018-07-13 06:29:00.000000 cryolo-1.9.8b1/cryolo/config.json
--rw-r--r--   0 twagner  (22293) domain users (32000)     5662 2024-03-26 15:04:22.000000 cryolo-1.9.8b1/cryolo/config_tools.py
--rw-r--r--   0 twagner  (22293) domain users (32000)    16314 2024-03-26 15:04:22.000000 cryolo-1.9.8b1/cryolo/cryolo_main.py
--rw-r--r--   0 twagner  (22293) domain users (32000)    35754 2024-03-26 15:04:22.000000 cryolo-1.9.8b1/cryolo/eval.py
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2024-03-26 15:23:19.483782 cryolo-1.9.8b1/cryolo/evaluation/
--rw-r--r--   0 twagner  (22293) domain users (32000)        0 2022-08-09 07:16:57.000000 cryolo-1.9.8b1/cryolo/evaluation/__init__.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     1683 2024-03-26 15:04:22.000000 cryolo-1.9.8b1/cryolo/evaluation/boxdataprovider.py
--rw-r--r--   0 twagner  (22293) domain users (32000)      356 2024-03-26 15:04:22.000000 cryolo-1.9.8b1/cryolo/evaluation/metric.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     1021 2024-03-26 15:04:22.000000 cryolo-1.9.8b1/cryolo/evaluation/pathsboxdataprovider.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     1592 2024-03-26 15:04:22.000000 cryolo-1.9.8b1/cryolo/evaluation/pathsfilamentprovider.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     1437 2024-03-26 15:04:22.000000 cryolo-1.9.8b1/cryolo/evaluation/recallprecisionmetric3d.py
--rw-r--r--   0 twagner  (22293) domain users (32000)      699 2024-03-26 15:04:22.000000 cryolo-1.9.8b1/cryolo/evaluation/resultsview.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     6272 2024-03-26 15:04:22.000000 cryolo-1.9.8b1/cryolo/evaluation/tomoevaluation.py
--rw-r--r--   0 twagner  (22293) domain users (32000)    39033 2024-03-26 15:04:22.000000 cryolo-1.9.8b1/cryolo/filament_tracer.py
--rw-r--r--   0 twagner  (22293) domain users (32000)    43372 2024-03-26 15:04:22.000000 cryolo-1.9.8b1/cryolo/frontend.py
--rw-r--r--   0 twagner  (22293) domain users (32000)    16850 2024-03-26 15:04:22.000000 cryolo-1.9.8b1/cryolo/grouping3d.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     5599 2024-03-26 15:04:22.000000 cryolo-1.9.8b1/cryolo/imagereader.py
--rw-r--r--   0 twagner  (22293) domain users (32000)    12487 2024-03-26 15:04:22.000000 cryolo-1.9.8b1/cryolo/lowpass.py
--rw-r--r--   0 twagner  (22293) domain users (32000)    17815 2024-03-26 15:04:22.000000 cryolo-1.9.8b1/cryolo/patchwisebatchgenerator2.py
--rw-r--r--   0 twagner  (22293) domain users (32000)    89603 2024-03-26 15:17:42.000000 cryolo-1.9.8b1/cryolo/predict.py
--rw-r--r--   0 twagner  (22293) domain users (32000)    10518 2024-03-26 15:04:22.000000 cryolo-1.9.8b1/cryolo/preprocessing.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     1440 2020-05-19 10:49:52.000000 cryolo-1.9.8b1/cryolo/test_gooey.py
--rw-r--r--   0 twagner  (22293) domain users (32000)    28161 2024-03-26 15:04:22.000000 cryolo-1.9.8b1/cryolo/train.py
--rw-r--r--   0 twagner  (22293) domain users (32000)    61953 2024-03-26 15:04:22.000000 cryolo-1.9.8b1/cryolo/utils.py
--rw-r--r--   0 twagner  (22293) domain users (32000)      693 2020-11-11 15:27:12.000000 cryolo-1.9.8b1/cryolo/vis_box_3d.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     3960 2024-03-26 15:04:22.000000 cryolo-1.9.8b1/cryolo/warmup_callback.py
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2024-03-26 15:23:19.483782 cryolo-1.9.8b1/cryolo.egg-info/
--rw-r--r--   0 twagner  (22293) domain users (32000)     1750 2024-03-26 15:23:14.000000 cryolo-1.9.8b1/cryolo.egg-info/PKG-INFO
--rw-r--r--   0 twagner  (22293) domain users (32000)     2533 2024-03-26 15:23:19.000000 cryolo-1.9.8b1/cryolo.egg-info/SOURCES.txt
--rw-r--r--   0 twagner  (22293) domain users (32000)        1 2024-03-26 15:23:14.000000 cryolo-1.9.8b1/cryolo.egg-info/dependency_links.txt
--rw-r--r--   0 twagner  (22293) domain users (32000)      250 2024-03-26 15:23:14.000000 cryolo-1.9.8b1/cryolo.egg-info/entry_points.txt
--rw-r--r--   0 twagner  (22293) domain users (32000)      505 2024-03-26 15:23:14.000000 cryolo-1.9.8b1/cryolo.egg-info/requires.txt
--rw-r--r--   0 twagner  (22293) domain users (32000)       13 2024-03-26 15:23:14.000000 cryolo-1.9.8b1/cryolo.egg-info/top_level.txt
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2024-03-26 15:23:19.483782 cryolo-1.9.8b1/icons/
--rw-r--r--   0 twagner  (22293) domain users (32000)    15129 2019-07-30 13:12:26.000000 cryolo-1.9.8b1/icons/config_icon.png
--rw-r--r--   0 twagner  (22293) domain users (32000)   113506 2019-07-30 13:57:17.000000 cryolo-1.9.8b1/icons/program_icon.ico
--rw-r--r--   0 twagner  (22293) domain users (32000)     2628 2019-09-24 13:29:39.000000 cryolo-1.9.8b1/icons/program_icon.png
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2024-03-26 15:23:19.475782 cryolo-1.9.8b1/resources/
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2024-03-26 15:23:19.475782 cryolo-1.9.8b1/resources/test_FolderDataProvider/
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2024-03-26 15:23:19.483782 cryolo-1.9.8b1/resources/test_FolderDataProvider/00_gt/
--rw-r--r--   0 twagner  (22293) domain users (32000)      393 2022-08-09 07:16:59.000000 cryolo-1.9.8b1/resources/test_FolderDataProvider/00_gt/tomo018_10.cbox
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2024-03-26 15:23:19.483782 cryolo-1.9.8b1/resources/test_FolderDataProvider/00_measured/
--rw-r--r--   0 twagner  (22293) domain users (32000)    30847 2022-08-09 07:16:59.000000 cryolo-1.9.8b1/resources/test_FolderDataProvider/00_measured/tomo018_10.cbox
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2024-03-26 15:23:19.483782 cryolo-1.9.8b1/resources/test_FolderDataProvider/01_gt_filament/
--rw-r--r--   0 twagner  (22293) domain users (32000)    83564 2022-08-09 07:16:59.000000 cryolo-1.9.8b1/resources/test_FolderDataProvider/01_gt_filament/SarcDros_ba03_ex01_la03_to01_10.96Apx_lp60.cbox
--rw-r--r--   0 twagner  (22293) domain users (32000)       38 2024-03-26 15:23:19.487782 cryolo-1.9.8b1/setup.cfg
--rw-r--r--   0 twagner  (22293) domain users (32000)     7231 2024-03-26 15:04:22.000000 cryolo-1.9.8b1/setup.py
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2024-03-26 15:23:19.483782 cryolo-1.9.8b1/tests/
--rw-r--r--   0 twagner  (22293) domain users (32000)        0 2022-08-09 07:16:59.000000 cryolo-1.9.8b1/tests/__init__.py
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2024-03-26 15:23:19.487782 cryolo-1.9.8b1/tests/evaluation/
--rw-r--r--   0 twagner  (22293) domain users (32000)        0 2022-08-09 07:16:59.000000 cryolo-1.9.8b1/tests/evaluation/__init__.py
--rw-r--r--   0 twagner  (22293) domain users (32000)      367 2022-08-09 07:16:59.000000 cryolo-1.9.8b1/tests/evaluation/test_BoxDataProvider.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     2462 2022-08-09 07:16:59.000000 cryolo-1.9.8b1/tests/evaluation/test_PathsDataProvider.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     3667 2022-08-09 07:16:59.000000 cryolo-1.9.8b1/tests/evaluation/test_RecallPrecisionMetric3D.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     5708 2024-03-26 15:04:22.000000 cryolo-1.9.8b1/tests/evaluation/test_tomoevaluation.py
--rw-r--r--   0 twagner  (22293) domain users (32000)    10039 2024-03-26 15:04:22.000000 cryolo-1.9.8b1/tests/test_CoordsIO.py
--rw-r--r--   0 twagner  (22293) domain users (32000)    16715 2024-03-26 15:04:22.000000 cryolo-1.9.8b1/tests/test_augmentation.py
--rw-r--r--   0 twagner  (22293) domain users (32000)      374 2022-08-09 07:16:59.000000 cryolo-1.9.8b1/tests/test_eval.py
--rw-r--r--   0 twagner  (22293) domain users (32000)    35400 2024-03-26 15:04:22.000000 cryolo-1.9.8b1/tests/test_filament_tracer.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     3006 2024-03-26 15:04:22.000000 cryolo-1.9.8b1/tests/test_frontend.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     6591 2024-03-26 15:04:22.000000 cryolo-1.9.8b1/tests/test_grouping3d.py
--rw-r--r--   0 twagner  (22293) domain users (32000)      494 2024-03-26 15:04:22.000000 cryolo-1.9.8b1/tests/test_lowpass.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     1885 2022-08-09 07:16:59.000000 cryolo-1.9.8b1/tests/test_predict.py
--rw-r--r--   0 twagner  (22293) domain users (32000)      606 2022-08-09 07:16:59.000000 cryolo-1.9.8b1/tests/test_preprocessing.py
--rw-r--r--   0 twagner  (22293) domain users (32000)    26655 2024-03-26 15:04:22.000000 cryolo-1.9.8b1/tests/test_utils.py
+drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2024-04-03 13:02:06.725680 cryolo-1.9.8b2/
+-rw-r--r--   0 twagner  (22293) domain users (32000)    17704 2023-02-09 08:33:23.000000 cryolo-1.9.8b2/.gitignore
+-rw-r--r--   0 twagner  (22293) domain users (32000)      605 2022-08-09 07:16:57.000000 cryolo-1.9.8b2/.gitlab-ci.yml
+drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2024-04-03 13:02:06.717681 cryolo-1.9.8b2/.idea/
+drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2024-04-03 13:02:06.717681 cryolo-1.9.8b2/.idea/codeStyles/
+-rw-r--r--   0 twagner  (22293) domain users (32000)      149 2018-12-11 09:23:01.000000 cryolo-1.9.8b2/.idea/codeStyles/codeStyleConfig.xml
+-rw-r--r--   0 twagner  (22293) domain users (32000)      649 2022-08-09 07:16:57.000000 cryolo-1.9.8b2/Dockerfile
+-rw-r--r--   0 twagner  (22293) domain users (32000)     6596 2019-09-10 13:28:55.000000 cryolo-1.9.8b2/LICENSE
+-rw-r--r--   0 twagner  (22293) domain users (32000)       57 2022-08-09 07:16:57.000000 cryolo-1.9.8b2/MANIFEST.in
+-rw-r--r--   0 twagner  (22293) domain users (32000)     1750 2024-04-03 13:02:06.725680 cryolo-1.9.8b2/PKG-INFO
+-rw-r--r--   0 twagner  (22293) domain users (32000)      869 2022-08-11 12:21:51.000000 cryolo-1.9.8b2/README.md
+-rw-r--r--   0 twagner  (22293) domain users (32000)     6593 2022-08-09 07:16:57.000000 cryolo-1.9.8b2/changelog.txt
+drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2024-04-03 13:02:06.721680 cryolo-1.9.8b2/cryolo/
+-rw-r--r--   0 twagner  (22293) domain users (32000)    28327 2024-04-03 11:42:40.000000 cryolo-1.9.8b2/cryolo/CoordsIO.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     2187 2024-04-03 11:42:40.000000 cryolo-1.9.8b2/cryolo/ExtendedModelCheckpoint.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     3325 2024-04-03 11:42:40.000000 cryolo-1.9.8b2/cryolo/MultiGPUModelCheckpoint.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     3475 2024-04-03 11:42:40.000000 cryolo-1.9.8b2/cryolo/SGDRSchedular.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)      413 2024-04-03 13:02:01.000000 cryolo-1.9.8b2/cryolo/__init__.py
+drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2024-04-03 13:02:06.721680 cryolo-1.9.8b2/cryolo/augmentation/
+-rw-r--r--   0 twagner  (22293) domain users (32000)      877 2024-04-03 11:42:40.000000 cryolo-1.9.8b2/cryolo/augmentation/AddConstantAugmentation.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     1436 2024-04-03 11:42:40.000000 cryolo-1.9.8b2/cryolo/augmentation/AdditiveGaussianNoiseAugmentation.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)      298 2024-04-03 11:42:40.000000 cryolo-1.9.8b2/cryolo/augmentation/AugmentationMethod.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)      895 2024-04-03 11:42:40.000000 cryolo-1.9.8b2/cryolo/augmentation/AverageBlurAugmentation.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)      980 2024-04-03 11:42:40.000000 cryolo-1.9.8b2/cryolo/augmentation/ContrastNormalizationAugmentation.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     2128 2024-04-03 11:42:40.000000 cryolo-1.9.8b2/cryolo/augmentation/CustomRotationAugmentation.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)      995 2024-04-03 11:42:40.000000 cryolo-1.9.8b2/cryolo/augmentation/DropoutAugmentation.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     1828 2024-04-03 11:42:40.000000 cryolo-1.9.8b2/cryolo/augmentation/FlipAugmentation.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)      957 2024-04-03 11:42:40.000000 cryolo-1.9.8b2/cryolo/augmentation/GaussBlurAugmentation.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)      851 2024-04-03 11:42:40.000000 cryolo-1.9.8b2/cryolo/augmentation/MultiplyAugmentation.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     1979 2024-04-03 11:42:40.000000 cryolo-1.9.8b2/cryolo/augmentation/Rot90Augmentation.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)        0 2022-08-09 07:16:57.000000 cryolo-1.9.8b2/cryolo/augmentation/__init__.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     3567 2024-04-03 11:42:40.000000 cryolo-1.9.8b2/cryolo/augmentation/augmentation.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)    20749 2024-04-03 11:42:40.000000 cryolo-1.9.8b2/cryolo/backend.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     1156 2018-07-13 06:29:00.000000 cryolo-1.9.8b2/cryolo/config.json
+-rw-r--r--   0 twagner  (22293) domain users (32000)     5662 2024-04-03 11:42:40.000000 cryolo-1.9.8b2/cryolo/config_tools.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)    16314 2024-04-03 11:42:40.000000 cryolo-1.9.8b2/cryolo/cryolo_main.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)    35754 2024-04-03 11:42:40.000000 cryolo-1.9.8b2/cryolo/eval.py
+drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2024-04-03 13:02:06.721680 cryolo-1.9.8b2/cryolo/evaluation/
+-rw-r--r--   0 twagner  (22293) domain users (32000)        0 2022-08-09 07:16:57.000000 cryolo-1.9.8b2/cryolo/evaluation/__init__.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     1683 2024-04-03 11:42:40.000000 cryolo-1.9.8b2/cryolo/evaluation/boxdataprovider.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)      356 2024-04-03 11:42:40.000000 cryolo-1.9.8b2/cryolo/evaluation/metric.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     1021 2024-04-03 11:42:40.000000 cryolo-1.9.8b2/cryolo/evaluation/pathsboxdataprovider.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     1592 2024-04-03 11:42:40.000000 cryolo-1.9.8b2/cryolo/evaluation/pathsfilamentprovider.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     1437 2024-04-03 11:42:40.000000 cryolo-1.9.8b2/cryolo/evaluation/recallprecisionmetric3d.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)      699 2024-04-03 11:42:40.000000 cryolo-1.9.8b2/cryolo/evaluation/resultsview.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     6272 2024-04-03 11:42:40.000000 cryolo-1.9.8b2/cryolo/evaluation/tomoevaluation.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)    39033 2024-04-03 11:42:40.000000 cryolo-1.9.8b2/cryolo/filament_tracer.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)    43372 2024-04-03 11:42:40.000000 cryolo-1.9.8b2/cryolo/frontend.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)    16850 2024-04-03 11:42:40.000000 cryolo-1.9.8b2/cryolo/grouping3d.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     5599 2024-04-03 11:42:40.000000 cryolo-1.9.8b2/cryolo/imagereader.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)    12487 2024-04-03 11:42:40.000000 cryolo-1.9.8b2/cryolo/lowpass.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)    17815 2024-04-03 11:42:40.000000 cryolo-1.9.8b2/cryolo/patchwisebatchgenerator2.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)    89603 2024-04-03 12:40:00.000000 cryolo-1.9.8b2/cryolo/predict.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)    10518 2024-04-03 12:40:00.000000 cryolo-1.9.8b2/cryolo/preprocessing.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     1440 2020-05-19 10:49:52.000000 cryolo-1.9.8b2/cryolo/test_gooey.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)    28161 2024-04-03 12:40:00.000000 cryolo-1.9.8b2/cryolo/train.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)    61953 2024-04-03 11:42:40.000000 cryolo-1.9.8b2/cryolo/utils.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)      693 2020-11-11 15:27:12.000000 cryolo-1.9.8b2/cryolo/vis_box_3d.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     3960 2024-04-03 11:42:40.000000 cryolo-1.9.8b2/cryolo/warmup_callback.py
+drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2024-04-03 13:02:06.721680 cryolo-1.9.8b2/cryolo.egg-info/
+-rw-r--r--   0 twagner  (22293) domain users (32000)     1750 2024-04-03 13:02:01.000000 cryolo-1.9.8b2/cryolo.egg-info/PKG-INFO
+-rw-r--r--   0 twagner  (22293) domain users (32000)     2533 2024-04-03 13:02:06.000000 cryolo-1.9.8b2/cryolo.egg-info/SOURCES.txt
+-rw-r--r--   0 twagner  (22293) domain users (32000)        1 2024-04-03 13:02:01.000000 cryolo-1.9.8b2/cryolo.egg-info/dependency_links.txt
+-rw-r--r--   0 twagner  (22293) domain users (32000)      250 2024-04-03 13:02:01.000000 cryolo-1.9.8b2/cryolo.egg-info/entry_points.txt
+-rw-r--r--   0 twagner  (22293) domain users (32000)      505 2024-04-03 13:02:01.000000 cryolo-1.9.8b2/cryolo.egg-info/requires.txt
+-rw-r--r--   0 twagner  (22293) domain users (32000)       13 2024-04-03 13:02:01.000000 cryolo-1.9.8b2/cryolo.egg-info/top_level.txt
+drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2024-04-03 13:02:06.721680 cryolo-1.9.8b2/icons/
+-rw-r--r--   0 twagner  (22293) domain users (32000)    15129 2019-07-30 13:12:26.000000 cryolo-1.9.8b2/icons/config_icon.png
+-rw-r--r--   0 twagner  (22293) domain users (32000)   113506 2019-07-30 13:57:17.000000 cryolo-1.9.8b2/icons/program_icon.ico
+-rw-r--r--   0 twagner  (22293) domain users (32000)     2628 2019-09-24 13:29:39.000000 cryolo-1.9.8b2/icons/program_icon.png
+drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2024-04-03 13:02:06.717681 cryolo-1.9.8b2/resources/
+drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2024-04-03 13:02:06.717681 cryolo-1.9.8b2/resources/test_FolderDataProvider/
+drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2024-04-03 13:02:06.721680 cryolo-1.9.8b2/resources/test_FolderDataProvider/00_gt/
+-rw-r--r--   0 twagner  (22293) domain users (32000)      393 2022-08-09 07:16:59.000000 cryolo-1.9.8b2/resources/test_FolderDataProvider/00_gt/tomo018_10.cbox
+drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2024-04-03 13:02:06.721680 cryolo-1.9.8b2/resources/test_FolderDataProvider/00_measured/
+-rw-r--r--   0 twagner  (22293) domain users (32000)    30847 2022-08-09 07:16:59.000000 cryolo-1.9.8b2/resources/test_FolderDataProvider/00_measured/tomo018_10.cbox
+drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2024-04-03 13:02:06.721680 cryolo-1.9.8b2/resources/test_FolderDataProvider/01_gt_filament/
+-rw-r--r--   0 twagner  (22293) domain users (32000)    83564 2022-08-09 07:16:59.000000 cryolo-1.9.8b2/resources/test_FolderDataProvider/01_gt_filament/SarcDros_ba03_ex01_la03_to01_10.96Apx_lp60.cbox
+-rw-r--r--   0 twagner  (22293) domain users (32000)       38 2024-04-03 13:02:06.725680 cryolo-1.9.8b2/setup.cfg
+-rw-r--r--   0 twagner  (22293) domain users (32000)     7171 2024-04-03 13:01:29.000000 cryolo-1.9.8b2/setup.py
+drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2024-04-03 13:02:06.725680 cryolo-1.9.8b2/tests/
+-rw-r--r--   0 twagner  (22293) domain users (32000)        0 2022-08-09 07:16:59.000000 cryolo-1.9.8b2/tests/__init__.py
+drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2024-04-03 13:02:06.725680 cryolo-1.9.8b2/tests/evaluation/
+-rw-r--r--   0 twagner  (22293) domain users (32000)        0 2022-08-09 07:16:59.000000 cryolo-1.9.8b2/tests/evaluation/__init__.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)      367 2022-08-09 07:16:59.000000 cryolo-1.9.8b2/tests/evaluation/test_BoxDataProvider.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     2462 2022-08-09 07:16:59.000000 cryolo-1.9.8b2/tests/evaluation/test_PathsDataProvider.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     3667 2022-08-09 07:16:59.000000 cryolo-1.9.8b2/tests/evaluation/test_RecallPrecisionMetric3D.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     5708 2024-04-03 11:42:40.000000 cryolo-1.9.8b2/tests/evaluation/test_tomoevaluation.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)    10039 2024-04-03 11:42:40.000000 cryolo-1.9.8b2/tests/test_CoordsIO.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)    16715 2024-04-03 11:42:40.000000 cryolo-1.9.8b2/tests/test_augmentation.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)      374 2022-08-09 07:16:59.000000 cryolo-1.9.8b2/tests/test_eval.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)    35400 2024-04-03 11:42:40.000000 cryolo-1.9.8b2/tests/test_filament_tracer.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     3006 2024-04-03 11:42:40.000000 cryolo-1.9.8b2/tests/test_frontend.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     6591 2024-04-03 11:42:40.000000 cryolo-1.9.8b2/tests/test_grouping3d.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)      494 2024-04-03 11:42:40.000000 cryolo-1.9.8b2/tests/test_lowpass.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     1885 2022-08-09 07:16:59.000000 cryolo-1.9.8b2/tests/test_predict.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)      606 2022-08-09 07:16:59.000000 cryolo-1.9.8b2/tests/test_preprocessing.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)    26655 2024-04-03 11:42:40.000000 cryolo-1.9.8b2/tests/test_utils.py
```

### Comparing `cryolo-1.9.8b1/.gitignore` & `cryolo-1.9.8b2/.gitignore`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/.gitlab-ci.yml` & `cryolo-1.9.8b2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/Dockerfile` & `cryolo-1.9.8b2/Dockerfile`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/LICENSE` & `cryolo-1.9.8b2/LICENSE`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/PKG-INFO` & `cryolo-1.9.8b2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryolo
-Version: 1.9.8b1
+Version: 1.9.8b2
 Summary: Picking procedure for cryo em single particle analysis
 Home-page: https://cryolo.readthedocs.io/en/stable/index.html
 Author: Thorsten Wagner
 Author-email: thorsten.wagner@mpi-dortmund.mpg.de
 License: Other/Proprietary License (all rights reserved)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `cryolo-1.9.8b1/README.md` & `cryolo-1.9.8b2/README.md`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/changelog.txt` & `cryolo-1.9.8b2/changelog.txt`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/cryolo/CoordsIO.py` & `cryolo-1.9.8b2/cryolo/CoordsIO.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/cryolo/ExtendedModelCheckpoint.py` & `cryolo-1.9.8b2/cryolo/ExtendedModelCheckpoint.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/cryolo/MultiGPUModelCheckpoint.py` & `cryolo-1.9.8b2/cryolo/MultiGPUModelCheckpoint.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/cryolo/SGDRSchedular.py` & `cryolo-1.9.8b2/cryolo/SGDRSchedular.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/cryolo/augmentation/AddConstantAugmentation.py` & `cryolo-1.9.8b2/cryolo/augmentation/AddConstantAugmentation.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/cryolo/augmentation/AdditiveGaussianNoiseAugmentation.py` & `cryolo-1.9.8b2/cryolo/augmentation/AdditiveGaussianNoiseAugmentation.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/cryolo/augmentation/AverageBlurAugmentation.py` & `cryolo-1.9.8b2/cryolo/augmentation/AverageBlurAugmentation.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/cryolo/augmentation/ContrastNormalizationAugmentation.py` & `cryolo-1.9.8b2/cryolo/augmentation/ContrastNormalizationAugmentation.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/cryolo/augmentation/CustomRotationAugmentation.py` & `cryolo-1.9.8b2/cryolo/augmentation/CustomRotationAugmentation.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/cryolo/augmentation/DropoutAugmentation.py` & `cryolo-1.9.8b2/cryolo/augmentation/DropoutAugmentation.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/cryolo/augmentation/FlipAugmentation.py` & `cryolo-1.9.8b2/cryolo/augmentation/FlipAugmentation.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/cryolo/augmentation/GaussBlurAugmentation.py` & `cryolo-1.9.8b2/cryolo/augmentation/GaussBlurAugmentation.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/cryolo/augmentation/MultiplyAugmentation.py` & `cryolo-1.9.8b2/cryolo/augmentation/MultiplyAugmentation.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/cryolo/augmentation/Rot90Augmentation.py` & `cryolo-1.9.8b2/cryolo/augmentation/Rot90Augmentation.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/cryolo/augmentation/augmentation.py` & `cryolo-1.9.8b2/cryolo/augmentation/augmentation.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/cryolo/backend.py` & `cryolo-1.9.8b2/cryolo/backend.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/cryolo/config.json` & `cryolo-1.9.8b2/cryolo/config.json`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/cryolo/config_tools.py` & `cryolo-1.9.8b2/cryolo/config_tools.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/cryolo/cryolo_main.py` & `cryolo-1.9.8b2/cryolo/cryolo_main.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/cryolo/eval.py` & `cryolo-1.9.8b2/cryolo/eval.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/cryolo/evaluation/boxdataprovider.py` & `cryolo-1.9.8b2/cryolo/evaluation/boxdataprovider.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/cryolo/evaluation/pathsboxdataprovider.py` & `cryolo-1.9.8b2/cryolo/evaluation/pathsboxdataprovider.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/cryolo/evaluation/pathsfilamentprovider.py` & `cryolo-1.9.8b2/cryolo/evaluation/pathsfilamentprovider.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/cryolo/evaluation/recallprecisionmetric3d.py` & `cryolo-1.9.8b2/cryolo/evaluation/recallprecisionmetric3d.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/cryolo/evaluation/resultsview.py` & `cryolo-1.9.8b2/cryolo/evaluation/resultsview.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/cryolo/evaluation/tomoevaluation.py` & `cryolo-1.9.8b2/cryolo/evaluation/tomoevaluation.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/cryolo/filament_tracer.py` & `cryolo-1.9.8b2/cryolo/filament_tracer.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/cryolo/frontend.py` & `cryolo-1.9.8b2/cryolo/frontend.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/cryolo/grouping3d.py` & `cryolo-1.9.8b2/cryolo/grouping3d.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/cryolo/imagereader.py` & `cryolo-1.9.8b2/cryolo/imagereader.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/cryolo/lowpass.py` & `cryolo-1.9.8b2/cryolo/lowpass.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/cryolo/patchwisebatchgenerator2.py` & `cryolo-1.9.8b2/cryolo/patchwisebatchgenerator2.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/cryolo/predict.py` & `cryolo-1.9.8b2/cryolo/predict.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/cryolo/preprocessing.py` & `cryolo-1.9.8b2/cryolo/preprocessing.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/cryolo/test_gooey.py` & `cryolo-1.9.8b2/cryolo/test_gooey.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/cryolo/train.py` & `cryolo-1.9.8b2/cryolo/train.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/cryolo/utils.py` & `cryolo-1.9.8b2/cryolo/utils.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/cryolo/vis_box_3d.py` & `cryolo-1.9.8b2/cryolo/vis_box_3d.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/cryolo/warmup_callback.py` & `cryolo-1.9.8b2/cryolo/warmup_callback.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/cryolo.egg-info/PKG-INFO` & `cryolo-1.9.8b2/cryolo.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryolo
-Version: 1.9.8b1
+Version: 1.9.8b2
 Summary: Picking procedure for cryo em single particle analysis
 Home-page: https://cryolo.readthedocs.io/en/stable/index.html
 Author: Thorsten Wagner
 Author-email: thorsten.wagner@mpi-dortmund.mpg.de
 License: Other/Proprietary License (all rights reserved)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `cryolo-1.9.8b1/cryolo.egg-info/SOURCES.txt` & `cryolo-1.9.8b2/cryolo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/icons/config_icon.png` & `cryolo-1.9.8b2/icons/config_icon.png`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/icons/program_icon.ico` & `cryolo-1.9.8b2/icons/program_icon.ico`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/icons/program_icon.png` & `cryolo-1.9.8b2/icons/program_icon.png`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/resources/test_FolderDataProvider/00_measured/tomo018_10.cbox` & `cryolo-1.9.8b2/resources/test_FolderDataProvider/00_measured/tomo018_10.cbox`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/resources/test_FolderDataProvider/01_gt_filament/SarcDros_ba03_ex01_la03_to01_10.96Apx_lp60.cbox` & `cryolo-1.9.8b2/resources/test_FolderDataProvider/01_gt_filament/SarcDros_ba03_ex01_la03_to01_10.96Apx_lp60.cbox`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/setup.py` & `cryolo-1.9.8b2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from setuptools import setup
 import os
 import re
 import codecs
 import sys
-import setuptools
-from distutils.command.sdist import sdist
 from setuptools.command.install import install
 # Create new package with python setup.py sdist
 
 
 
 here = os.path.abspath(os.path.dirname(__file__))
```

### Comparing `cryolo-1.9.8b1/tests/evaluation/test_PathsDataProvider.py` & `cryolo-1.9.8b2/tests/evaluation/test_PathsDataProvider.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/tests/evaluation/test_RecallPrecisionMetric3D.py` & `cryolo-1.9.8b2/tests/evaluation/test_RecallPrecisionMetric3D.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/tests/evaluation/test_tomoevaluation.py` & `cryolo-1.9.8b2/tests/evaluation/test_tomoevaluation.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/tests/test_CoordsIO.py` & `cryolo-1.9.8b2/tests/test_CoordsIO.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/tests/test_augmentation.py` & `cryolo-1.9.8b2/tests/test_augmentation.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/tests/test_filament_tracer.py` & `cryolo-1.9.8b2/tests/test_filament_tracer.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/tests/test_frontend.py` & `cryolo-1.9.8b2/tests/test_frontend.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/tests/test_grouping3d.py` & `cryolo-1.9.8b2/tests/test_grouping3d.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/tests/test_predict.py` & `cryolo-1.9.8b2/tests/test_predict.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/tests/test_preprocessing.py` & `cryolo-1.9.8b2/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `cryolo-1.9.8b1/tests/test_utils.py` & `cryolo-1.9.8b2/tests/test_utils.py`

 * *Files identical despite different names*

