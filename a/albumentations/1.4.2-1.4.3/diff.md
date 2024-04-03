# Comparing `tmp/albumentations-1.4.2.tar.gz` & `tmp/albumentations-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "albumentations-1.4.2.tar", last modified: Tue Mar 19 00:00:13 2024, max compression
+gzip compressed data, was "albumentations-1.4.3.tar", last modified: Wed Apr  3 01:50:59 2024, max compression
```

## Comparing `albumentations-1.4.2.tar` & `albumentations-1.4.3.tar`

### file list

```diff
@@ -1,91 +1,76 @@
-drwxr-xr-x   0 vladimiriglovikov   (501) staff       (20)        0 2024-03-19 00:00:13.677005 albumentations-1.4.2/
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     1114 2024-03-13 14:21:41.000000 albumentations-1.4.2/LICENSE
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)      176 2024-02-12 19:09:55.000000 albumentations-1.4.2/MANIFEST.in
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)    36767 2024-03-19 00:00:13.676610 albumentations-1.4.2/PKG-INFO
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)    35010 2024-03-18 21:47:51.000000 albumentations-1.4.2/README.md
-drwxr-xr-x   0 vladimiriglovikov   (501) staff       (20)        0 2024-03-19 00:00:13.645430 albumentations-1.4.2/albumentations/
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)      159 2024-03-18 23:08:19.000000 albumentations-1.4.2/albumentations/__init__.py
-drwxr-xr-x   0 vladimiriglovikov   (501) staff       (20)        0 2024-03-19 00:00:13.650445 albumentations-1.4.2/albumentations/augmentations/
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)      695 2024-03-13 14:21:41.000000 albumentations-1.4.2/albumentations/augmentations/__init__.py
-drwxr-xr-x   0 vladimiriglovikov   (501) staff       (20)        0 2024-03-19 00:00:13.651775 albumentations-1.4.2/albumentations/augmentations/blur/
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)       52 2024-03-07 04:07:43.000000 albumentations-1.4.2/albumentations/augmentations/blur/__init__.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     3770 2024-03-13 14:21:41.000000 albumentations-1.4.2/albumentations/augmentations/blur/functional.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)    20466 2024-03-18 21:47:51.000000 albumentations-1.4.2/albumentations/augmentations/blur/transforms.py
-drwxr-xr-x   0 vladimiriglovikov   (501) staff       (20)        0 2024-03-19 00:00:13.652935 albumentations-1.4.2/albumentations/augmentations/crops/
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)       52 2024-02-12 19:09:55.000000 albumentations-1.4.2/albumentations/augmentations/crops/__init__.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)    10110 2024-03-13 14:21:41.000000 albumentations-1.4.2/albumentations/augmentations/crops/functional.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)    41842 2024-03-13 14:21:41.000000 albumentations-1.4.2/albumentations/augmentations/crops/transforms.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)    10151 2024-03-13 14:21:41.000000 albumentations-1.4.2/albumentations/augmentations/domain_adaptation.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     6311 2024-03-13 14:21:41.000000 albumentations-1.4.2/albumentations/augmentations/domain_adaptation_functional.py
-drwxr-xr-x   0 vladimiriglovikov   (501) staff       (20)        0 2024-03-19 00:00:13.655142 albumentations-1.4.2/albumentations/augmentations/dropout/
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)      143 2024-03-13 14:21:41.000000 albumentations-1.4.2/albumentations/augmentations/dropout/__init__.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     2329 2024-03-13 14:21:41.000000 albumentations-1.4.2/albumentations/augmentations/dropout/channel_dropout.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     6899 2024-03-13 14:21:41.000000 albumentations-1.4.2/albumentations/augmentations/dropout/coarse_dropout.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     1218 2024-03-13 14:21:41.000000 albumentations-1.4.2/albumentations/augmentations/dropout/functional.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     8644 2024-03-13 14:21:41.000000 albumentations-1.4.2/albumentations/augmentations/dropout/grid_dropout.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     3519 2024-03-13 14:21:41.000000 albumentations-1.4.2/albumentations/augmentations/dropout/mask_dropout.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     8596 2024-03-13 14:21:41.000000 albumentations-1.4.2/albumentations/augmentations/dropout/xy_masking.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)    44916 2024-03-18 21:47:51.000000 albumentations-1.4.2/albumentations/augmentations/functional.py
-drwxr-xr-x   0 vladimiriglovikov   (501) staff       (20)        0 2024-03-19 00:00:13.656795 albumentations-1.4.2/albumentations/augmentations/geometric/
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)       96 2024-03-13 00:00:34.000000 albumentations-1.4.2/albumentations/augmentations/geometric/__init__.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)    39909 2024-03-13 14:21:41.000000 albumentations-1.4.2/albumentations/augmentations/geometric/functional.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     8251 2024-03-13 14:21:41.000000 albumentations-1.4.2/albumentations/augmentations/geometric/resize.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)    13823 2024-03-13 14:21:41.000000 albumentations-1.4.2/albumentations/augmentations/geometric/rotate.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)    68133 2024-03-13 14:21:41.000000 albumentations-1.4.2/albumentations/augmentations/geometric/transforms.py
-drwxr-xr-x   0 vladimiriglovikov   (501) staff       (20)        0 2024-03-19 00:00:13.658139 albumentations-1.4.2/albumentations/augmentations/mixing/
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)       52 2024-03-13 14:21:41.000000 albumentations-1.4.2/albumentations/augmentations/mixing/__init__.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)      349 2024-03-13 14:21:41.000000 albumentations-1.4.2/albumentations/augmentations/mixing/functional.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)    10427 2024-03-13 14:23:02.000000 albumentations-1.4.2/albumentations/augmentations/mixing/transforms.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)   105489 2024-03-18 21:47:51.000000 albumentations-1.4.2/albumentations/augmentations/transforms.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     6985 2024-03-13 14:21:41.000000 albumentations-1.4.2/albumentations/augmentations/utils.py
-drwxr-xr-x   0 vladimiriglovikov   (501) staff       (20)        0 2024-03-19 00:00:13.660442 albumentations-1.4.2/albumentations/core/
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)        0 2024-02-12 19:09:55.000000 albumentations-1.4.2/albumentations/core/__init__.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)    20398 2024-03-13 14:21:41.000000 albumentations-1.4.2/albumentations/core/bbox_utils.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)    21759 2024-03-13 14:21:41.000000 albumentations-1.4.2/albumentations/core/composition.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     9100 2024-03-13 14:21:41.000000 albumentations-1.4.2/albumentations/core/keypoints_utils.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)    12736 2024-03-13 14:21:41.000000 albumentations-1.4.2/albumentations/core/serialization.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)    14314 2024-03-13 14:21:41.000000 albumentations-1.4.2/albumentations/core/transforms_interface.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     1499 2024-03-18 21:47:51.000000 albumentations-1.4.2/albumentations/core/types.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     4939 2024-03-13 14:21:41.000000 albumentations-1.4.2/albumentations/core/utils.py
-drwxr-xr-x   0 vladimiriglovikov   (501) staff       (20)        0 2024-03-19 00:00:13.665846 albumentations-1.4.2/albumentations/pytorch/
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)       26 2024-03-08 01:27:39.000000 albumentations-1.4.2/albumentations/pytorch/__init__.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     2103 2024-03-13 14:21:41.000000 albumentations-1.4.2/albumentations/pytorch/transforms.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     3799 2024-03-13 14:23:02.000000 albumentations-1.4.2/albumentations/random_utils.py
-drwxr-xr-x   0 vladimiriglovikov   (501) staff       (20)        0 2024-03-19 00:00:13.676258 albumentations-1.4.2/albumentations.egg-info/
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)    36767 2024-03-19 00:00:13.000000 albumentations-1.4.2/albumentations.egg-info/PKG-INFO
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     2676 2024-03-19 00:00:13.000000 albumentations-1.4.2/albumentations.egg-info/SOURCES.txt
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)        1 2024-03-19 00:00:13.000000 albumentations-1.4.2/albumentations.egg-info/dependency_links.txt
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)      131 2024-03-19 00:00:13.000000 albumentations-1.4.2/albumentations.egg-info/requires.txt
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)       15 2024-03-19 00:00:13.000000 albumentations-1.4.2/albumentations.egg-info/top_level.txt
-drwxr-xr-x   0 vladimiriglovikov   (501) staff       (20)        0 2024-03-19 00:00:13.667273 albumentations-1.4.2/benchmark/
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)      349 2024-02-12 19:09:55.000000 albumentations-1.4.2/benchmark/Dockerfile
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     1039 2024-03-13 14:21:41.000000 albumentations-1.4.2/benchmark/README.md
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)    27306 2024-03-16 00:29:30.000000 albumentations-1.4.2/benchmark/benchmark.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)      140 2024-03-16 00:29:30.000000 albumentations-1.4.2/benchmark/requirements.txt
-drwxr-xr-x   0 vladimiriglovikov   (501) staff       (20)        0 2024-03-19 00:00:13.667521 albumentations-1.4.2/docs/
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)      592 2024-03-07 04:08:36.000000 albumentations-1.4.2/docs/index.md
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     2542 2024-03-18 23:33:44.000000 albumentations-1.4.2/pyproject.toml
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)       38 2024-03-19 00:00:13.677069 albumentations-1.4.2/setup.cfg
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     3460 2024-03-18 23:58:15.000000 albumentations-1.4.2/setup.py
-drwxr-xr-x   0 vladimiriglovikov   (501) staff       (20)        0 2024-03-19 00:00:13.674417 albumentations-1.4.2/tests/
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)        0 2024-02-12 19:09:55.000000 albumentations-1.4.2/tests/__init__.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     1474 2024-03-13 14:21:41.000000 albumentations-1.4.2/tests/conftest.py
-drwxr-xr-x   0 vladimiriglovikov   (501) staff       (20)        0 2024-03-19 00:00:13.675781 albumentations-1.4.2/tests/files/
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)    14644 2024-02-16 21:31:06.000000 albumentations-1.4.2/tests/files/transform_serialization_v2_with_totensor.json
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)    14523 2024-02-16 21:31:06.000000 albumentations-1.4.2/tests/files/transform_serialization_v2_without_totensor.json
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)    16220 2024-02-16 21:31:06.000000 albumentations-1.4.2/tests/files/transform_v1.1.0_with_totensor.json
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)    16042 2024-02-16 21:31:06.000000 albumentations-1.4.2/tests/files/transform_v1.1.0_without_totensor.json
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)    39987 2024-03-18 21:47:51.000000 albumentations-1.4.2/tests/test_augmentations.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)    11658 2024-02-12 19:09:55.000000 albumentations-1.4.2/tests/test_bbox.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)    15589 2024-02-15 21:36:19.000000 albumentations-1.4.2/tests/test_core.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)    46127 2024-03-13 14:23:02.000000 albumentations-1.4.2/tests/test_functional.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     1863 2024-03-13 14:21:41.000000 albumentations-1.4.2/tests/test_functional_cutout.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     2261 2024-03-13 14:21:41.000000 albumentations-1.4.2/tests/test_functional_mixing.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)    12548 2024-03-13 14:21:41.000000 albumentations-1.4.2/tests/test_keypoint.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     8393 2024-03-13 14:23:02.000000 albumentations-1.4.2/tests/test_mixing.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     6237 2024-03-13 14:21:41.000000 albumentations-1.4.2/tests/test_pytorch.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     1028 2024-03-13 14:23:02.000000 albumentations-1.4.2/tests/test_random.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)    36680 2024-03-18 21:47:51.000000 albumentations-1.4.2/tests/test_serialization.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     8291 2024-03-13 14:21:41.000000 albumentations-1.4.2/tests/test_targets.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)    49987 2024-03-18 21:47:51.000000 albumentations-1.4.2/tests/test_transforms.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     4818 2024-03-13 14:21:41.000000 albumentations-1.4.2/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:50:59.672591 albumentations-1.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-03 01:50:48.000000 albumentations-1.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-03 01:50:48.000000 albumentations-1.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    37024 2024-04-03 01:50:59.672591 albumentations-1.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    35267 2024-04-03 01:50:48.000000 albumentations-1.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:50:59.660591 albumentations-1.4.3/albumentations/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:50:59.664591 albumentations-1.4.3/albumentations/augmentations/
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:50:59.664591 albumentations-1.4.3/albumentations/augmentations/blur/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/blur/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/blur/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20466 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/blur/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:50:59.664591 albumentations-1.4.3/albumentations/augmentations/crops/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/crops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10110 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/crops/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44695 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/crops/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14384 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/domain_adaptation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/domain_adaptation_functional.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:50:59.664591 albumentations-1.4.3/albumentations/augmentations/dropout/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/dropout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/dropout/channel_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6899 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/dropout/coarse_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/dropout/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8644 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/dropout/grid_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/dropout/mask_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8596 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/dropout/xy_masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45479 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/functional.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:50:59.664591 albumentations-1.4.3/albumentations/augmentations/geometric/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/geometric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39909 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/geometric/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8251 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/geometric/resize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13823 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/geometric/rotate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68133 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/geometric/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:50:59.664591 albumentations-1.4.3/albumentations/augmentations/mixing/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/mixing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/mixing/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10427 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/mixing/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)   108319 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:50:59.668591 albumentations-1.4.3/albumentations/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20398 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/core/bbox_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21759 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/core/composition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9100 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/core/keypoints_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12736 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/core/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14314 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/core/transforms_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:50:59.668591 albumentations-1.4.3/albumentations/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/pytorch/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/random_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:50:59.672591 albumentations-1.4.3/albumentations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    37024 2024-04-03 01:50:59.000000 albumentations-1.4.3/albumentations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-03 01:50:59.000000 albumentations-1.4.3/albumentations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 01:50:59.000000 albumentations-1.4.3/albumentations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-03 01:50:59.000000 albumentations-1.4.3/albumentations.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-03 01:50:59.000000 albumentations-1.4.3/albumentations.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-04-03 01:50:48.000000 albumentations-1.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 01:50:59.672591 albumentations-1.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-03 01:50:48.000000 albumentations-1.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:50:59.672591 albumentations-1.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    39987 2024-04-03 01:50:48.000000 albumentations-1.4.3/tests/test_augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11658 2024-04-03 01:50:48.000000 albumentations-1.4.3/tests/test_bbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15589 2024-04-03 01:50:48.000000 albumentations-1.4.3/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46127 2024-04-03 01:50:48.000000 albumentations-1.4.3/tests/test_functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-03 01:50:48.000000 albumentations-1.4.3/tests/test_functional_cutout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-03 01:50:48.000000 albumentations-1.4.3/tests/test_functional_mixing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12548 2024-04-03 01:50:48.000000 albumentations-1.4.3/tests/test_keypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-04-03 01:50:48.000000 albumentations-1.4.3/tests/test_mixing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-04-03 01:50:48.000000 albumentations-1.4.3/tests/test_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-03 01:50:48.000000 albumentations-1.4.3/tests/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36764 2024-04-03 01:50:48.000000 albumentations-1.4.3/tests/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8112 2024-04-03 01:50:48.000000 albumentations-1.4.3/tests/test_targets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53341 2024-04-03 01:50:48.000000 albumentations-1.4.3/tests/test_transforms.py
```

### Comparing `albumentations-1.4.2/LICENSE` & `albumentations-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.2/PKG-INFO` & `albumentations-1.4.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,2298 +1,2205 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 616c 6275  : 2.1.Name: albu
-00000020: 6d65 6e74 6174 696f 6e73 0a56 6572 7369  mentations.Versi
-00000030: 6f6e 3a20 312e 342e 320a 5375 6d6d 6172  on: 1.4.2.Summar
-00000040: 793a 2041 6e20 6566 6669 6369 656e 7420  y: An efficient 
-00000050: 6c69 6272 6172 7920 666f 7220 696d 6167  library for imag
-00000060: 6520 6175 676d 656e 7461 7469 6f6e 2c20  e augmentation, 
-00000070: 7072 6f76 6964 696e 6720 6578 7465 6e73  providing extens
-00000080: 6976 6520 7472 616e 7366 6f72 6d61 7469  ive transformati
-00000090: 6f6e 7320 746f 2073 7570 706f 7274 206d  ons to support m
-000000a0: 6163 6869 6e65 206c 6561 726e 696e 6720  achine learning 
-000000b0: 616e 6420 636f 6d70 7574 6572 2076 6973  and computer vis
-000000c0: 696f 6e20 7461 736b 732e 0a48 6f6d 652d  ion tasks..Home-
-000000d0: 7061 6765 3a20 6874 7470 733a 2f2f 616c  page: https://al
-000000e0: 6275 6d65 6e74 6174 696f 6e73 2e61 690a  bumentations.ai.
-000000f0: 4175 7468 6f72 3a20 566c 6164 696d 6972  Author: Vladimir
-00000100: 2049 2e20 4967 6c6f 7669 6b6f 762c 204d   I. Iglovikov, M
-00000110: 696b 6861 696c 2044 7275 7a68 696e 696e  ikhail Druzhinin
-00000120: 2c20 416c 6578 2050 6172 696e 6f76 2c20  , Alex Parinov, 
-00000130: 416c 6578 616e 6465 7220 4275 736c 6165  Alexander Buslae
-00000140: 762c 2045 7567 656e 6520 4b68 7665 6463  v, Eugene Khvedc
-00000150: 6865 6e79 610a 4c69 6365 6e73 653a 204d  henya.License: M
-00000160: 4954 0a4b 6579 776f 7264 733a 2069 6d61  IT.Keywords: ima
-00000170: 6765 2061 7567 6d65 6e74 6174 696f 6e2c  ge augmentation,
-00000180: 6461 7461 2061 7567 6d65 6e74 6174 696f  data augmentatio
-00000190: 6e2c 636f 6d70 7574 6572 2076 6973 696f  n,computer visio
-000001a0: 6e2c 6465 6570 206c 6561 726e 696e 672c  n,deep learning,
-000001b0: 6d61 6368 696e 6520 6c65 6172 6e69 6e67  machine learning
-000001c0: 2c69 6d61 6765 2070 726f 6365 7373 696e  ,image processin
-000001d0: 672c 6172 7469 6669 6369 616c 2069 6e74  g,artificial int
-000001e0: 656c 6c69 6765 6e63 652c 6175 676d 656e  elligence,augmen
-000001f0: 7461 7469 6f6e 206c 6962 7261 7279 2c69  tation library,i
-00000200: 6d61 6765 2074 7261 6e73 666f 726d 6174  mage transformat
-00000210: 696f 6e2c 7669 7369 6f6e 2061 7567 6d65  ion,vision augme
-00000220: 6e74 6174 696f 6e0a 436c 6173 7369 6669  ntation.Classifi
-00000230: 6572 3a20 4465 7665 6c6f 706d 656e 7420  er: Development 
-00000240: 5374 6174 7573 203a 3a20 3520 2d20 5072  Status :: 5 - Pr
-00000250: 6f64 7563 7469 6f6e 2f53 7461 626c 650a  oduction/Stable.
-00000260: 436c 6173 7369 6669 6572 3a20 496e 7465  Classifier: Inte
-00000270: 6e64 6564 2041 7564 6965 6e63 6520 3a3a  nded Audience ::
-00000280: 2044 6576 656c 6f70 6572 730a 436c 6173   Developers.Clas
-00000290: 7369 6669 6572 3a20 496e 7465 6e64 6564  sifier: Intended
-000002a0: 2041 7564 6965 6e63 6520 3a3a 2053 6369   Audience :: Sci
-000002b0: 656e 6365 2f52 6573 6561 7263 680a 436c  ence/Research.Cl
-000002c0: 6173 7369 6669 6572 3a20 4c69 6365 6e73  assifier: Licens
-000002d0: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
-000002e0: 6420 3a3a 204d 4954 204c 6963 656e 7365  d :: MIT License
-000002f0: 0a43 6c61 7373 6966 6965 723a 204f 7065  .Classifier: Ope
-00000300: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
-00000310: 204f 5320 496e 6465 7065 6e64 656e 740a   OS Independent.
-00000320: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
-00000330: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000340: 203a 3a20 5079 7468 6f6e 0a43 6c61 7373   :: Python.Class
-00000350: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-00000360: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000370: 7974 686f 6e20 3a3a 2033 0a43 6c61 7373  ython :: 3.Class
-00000380: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-00000390: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-000003a0: 7974 686f 6e20 3a3a 2033 2e38 0a43 6c61  ython :: 3.8.Cla
-000003b0: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-000003c0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-000003d0: 2050 7974 686f 6e20 3a3a 2033 2e39 0a43   Python :: 3.9.C
-000003e0: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
-000003f0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000400: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
-00000410: 300a 436c 6173 7369 6669 6572 3a20 5072  0.Classifier: Pr
-00000420: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000430: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000440: 332e 3131 0a43 6c61 7373 6966 6965 723a  3.11.Classifier:
-00000450: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
-00000460: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000470: 3a3a 2033 2e31 320a 436c 6173 7369 6669  :: 3.12.Classifi
-00000480: 6572 3a20 546f 7069 6320 3a3a 2053 6f66  er: Topic :: Sof
-00000490: 7477 6172 6520 4465 7665 6c6f 706d 656e  tware Developmen
-000004a0: 7420 3a3a 204c 6962 7261 7269 6573 0a43  t :: Libraries.C
-000004b0: 6c61 7373 6966 6965 723a 2054 6f70 6963  lassifier: Topic
-000004c0: 203a 3a20 536f 6674 7761 7265 2044 6576   :: Software Dev
-000004d0: 656c 6f70 6d65 6e74 203a 3a20 4c69 6272  elopment :: Libr
-000004e0: 6172 6965 7320 3a3a 2050 7974 686f 6e20  aries :: Python 
-000004f0: 4d6f 6475 6c65 730a 436c 6173 7369 6669  Modules.Classifi
-00000500: 6572 3a20 546f 7069 6320 3a3a 2053 6369  er: Topic :: Sci
-00000510: 656e 7469 6669 632f 456e 6769 6e65 6572  entific/Engineer
-00000520: 696e 6720 3a3a 2041 7274 6966 6963 6961  ing :: Artificia
-00000530: 6c20 496e 7465 6c6c 6967 656e 6365 0a43  l Intelligence.C
-00000540: 6c61 7373 6966 6965 723a 2054 6f70 6963  lassifier: Topic
-00000550: 203a 3a20 5363 6965 6e74 6966 6963 2f45   :: Scientific/E
-00000560: 6e67 696e 6565 7269 6e67 203a 3a20 496d  ngineering :: Im
-00000570: 6167 6520 5072 6f63 6573 7369 6e67 0a43  age Processing.C
-00000580: 6c61 7373 6966 6965 723a 2054 7970 696e  lassifier: Typin
-00000590: 6720 3a3a 2054 7970 6564 0a52 6571 7569  g :: Typed.Requi
-000005a0: 7265 732d 5079 7468 6f6e 3a20 3e3d 332e  res-Python: >=3.
-000005b0: 380a 4465 7363 7269 7074 696f 6e2d 436f  8.Description-Co
-000005c0: 6e74 656e 742d 5479 7065 3a20 7465 7874  ntent-Type: text
-000005d0: 2f6d 6172 6b64 6f77 6e0a 4c69 6365 6e73  /markdown.Licens
-000005e0: 652d 4669 6c65 3a20 4c49 4345 4e53 450a  e-File: LICENSE.
-000005f0: 5265 7175 6972 6573 2d44 6973 743a 206e  Requires-Dist: n
-00000600: 756d 7079 3e3d 312e 3234 2e34 0a52 6571  umpy>=1.24.4.Req
-00000610: 7569 7265 732d 4469 7374 3a20 7363 6970  uires-Dist: scip
-00000620: 793e 3d31 2e31 302e 300a 5265 7175 6972  y>=1.10.0.Requir
-00000630: 6573 2d44 6973 743a 2073 6369 6b69 742d  es-Dist: scikit-
-00000640: 696d 6167 653e 3d30 2e32 312e 300a 5265  image>=0.21.0.Re
-00000650: 7175 6972 6573 2d44 6973 743a 2050 7959  quires-Dist: PyY
-00000660: 414d 4c0a 5265 7175 6972 6573 2d44 6973  AML.Requires-Dis
-00000670: 743a 2074 7970 696e 672d 6578 7465 6e73  t: typing-extens
-00000680: 696f 6e73 3e3d 342e 392e 300a 5265 7175  ions>=4.9.0.Requ
-00000690: 6972 6573 2d44 6973 743a 2073 6369 6b69  ires-Dist: sciki
-000006a0: 742d 6c65 6172 6e3e 3d31 2e33 2e32 0a52  t-learn>=1.3.2.R
-000006b0: 6571 7569 7265 732d 4469 7374 3a20 6f70  equires-Dist: op
-000006c0: 656e 6376 2d70 7974 686f 6e2d 6865 6164  encv-python-head
-000006d0: 6c65 7373 3e3d 342e 392e 300a 0a23 2041  less>=4.9.0..# A
-000006e0: 6c62 756d 656e 7461 7469 6f6e 730a 0a5b  lbumentations..[
-000006f0: 215b 5079 5049 2076 6572 7369 6f6e 5d28  ![PyPI version](
-00000700: 6874 7470 733a 2f2f 6261 6467 652e 6675  https://badge.fu
-00000710: 7279 2e69 6f2f 7079 2f61 6c62 756d 656e  ry.io/py/albumen
-00000720: 7461 7469 6f6e 732e 7376 6729 5d28 6874  tations.svg)](ht
-00000730: 7470 733a 2f2f 6261 6467 652e 6675 7279  tps://badge.fury
-00000740: 2e69 6f2f 7079 2f61 6c62 756d 656e 7461  .io/py/albumenta
-00000750: 7469 6f6e 7329 0a21 5b43 495d 2868 7474  tions).![CI](htt
-00000760: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000770: 616c 6275 6d65 6e74 6174 696f 6e73 2d74  albumentations-t
-00000780: 6561 6d2f 616c 6275 6d65 6e74 6174 696f  eam/albumentatio
-00000790: 6e73 2f77 6f72 6b66 6c6f 7773 2f43 492f  ns/workflows/CI/
-000007a0: 6261 6467 652e 7376 6729 0a5b 215b 4c69  badge.svg).[![Li
-000007b0: 6365 6e73 653a 204d 4954 5d28 6874 7470  cense: MIT](http
-000007c0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-000007d0: 696f 2f62 6164 6765 2f4c 6963 656e 7365  io/badge/License
-000007e0: 2d4d 4954 2d62 7269 6768 7467 7265 656e  -MIT-brightgreen
-000007f0: 2e73 7667 295d 2868 7474 7073 3a2f 2f6f  .svg)](https://o
-00000800: 7065 6e73 6f75 7263 652e 6f72 672f 6c69  pensource.org/li
-00000810: 6365 6e73 6573 2f4d 4954 290a 5b21 5b52  censes/MIT).[![R
-00000820: 7566 665d 2868 7474 7073 3a2f 2f69 6d67  uff](https://img
-00000830: 2e73 6869 656c 6473 2e69 6f2f 656e 6470  .shields.io/endp
-00000840: 6f69 6e74 3f75 726c 3d68 7474 7073 3a2f  oint?url=https:/
-00000850: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
-00000860: 6f6e 7465 6e74 2e63 6f6d 2f61 7374 7261  ontent.com/astra
-00000870: 6c2d 7368 2f72 7566 662f 6d61 696e 2f61  l-sh/ruff/main/a
-00000880: 7373 6574 732f 6261 6467 652f 7632 2e6a  ssets/badge/v2.j
-00000890: 736f 6e29 5d28 6874 7470 733a 2f2f 6769  son)](https://gi
-000008a0: 7468 7562 2e63 6f6d 2f61 7374 7261 6c2d  thub.com/astral-
-000008b0: 7368 2f72 7566 6629 0a0a 5b44 6973 636f  sh/ruff)..[Disco
-000008c0: 7264 5d28 6874 7470 733a 2f2f 6469 7363  rd](https://disc
-000008d0: 6f72 642e 6767 2f41 4b50 7272 4459 4e41  ord.gg/AKPrrDYNA
-000008e0: 7429 207c 205b 5477 6974 7465 725d 2868  t) | [Twitter](h
-000008f0: 7474 7073 3a2f 2f74 7769 7474 6572 2e63  ttps://twitter.c
-00000900: 6f6d 2f61 6c62 756d 656e 7461 7469 6f6e  om/albumentation
-00000910: 7329 207c 205b 446f 6373 5d28 6874 7470  s) | [Docs](http
-00000920: 733a 2f2f 616c 6275 6d65 6e74 6174 696f  s://albumentatio
-00000930: 6e73 2e61 692f 646f 6373 2f29 0a0a 416c  ns.ai/docs/)..Al
-00000940: 6275 6d65 6e74 6174 696f 6e73 2069 7320  bumentations is 
-00000950: 6120 5079 7468 6f6e 206c 6962 7261 7279  a Python library
-00000960: 2066 6f72 2069 6d61 6765 2061 7567 6d65   for image augme
-00000970: 6e74 6174 696f 6e2e 2049 6d61 6765 2061  ntation. Image a
-00000980: 7567 6d65 6e74 6174 696f 6e20 6973 2075  ugmentation is u
-00000990: 7365 6420 696e 2064 6565 7020 6c65 6172  sed in deep lear
-000009a0: 6e69 6e67 2061 6e64 2063 6f6d 7075 7465  ning and compute
-000009b0: 7220 7669 7369 6f6e 2074 6173 6b73 2074  r vision tasks t
-000009c0: 6f20 696e 6372 6561 7365 2074 6865 2071  o increase the q
-000009d0: 7561 6c69 7479 206f 6620 7472 6169 6e65  uality of traine
-000009e0: 6420 6d6f 6465 6c73 2e20 5468 6520 7075  d models. The pu
-000009f0: 7270 6f73 6520 6f66 2069 6d61 6765 2061  rpose of image a
-00000a00: 7567 6d65 6e74 6174 696f 6e20 6973 2074  ugmentation is t
-00000a10: 6f20 6372 6561 7465 206e 6577 2074 7261  o create new tra
-00000a20: 696e 696e 6720 7361 6d70 6c65 7320 6672  ining samples fr
-00000a30: 6f6d 2074 6865 2065 7869 7374 696e 6720  om the existing 
-00000a40: 6461 7461 2e0a 0a48 6572 6520 6973 2061  data...Here is a
-00000a50: 6e20 6578 616d 706c 6520 6f66 2068 6f77  n example of how
-00000a60: 2079 6f75 2063 616e 2061 7070 6c79 2073   you can apply s
-00000a70: 6f6d 6520 5b70 6978 656c 2d6c 6576 656c  ome [pixel-level
-00000a80: 5d28 2370 6978 656c 2d6c 6576 656c 2d74  ](#pixel-level-t
-00000a90: 7261 6e73 666f 726d 7329 2061 7567 6d65  ransforms) augme
-00000aa0: 6e74 6174 696f 6e73 2066 726f 6d20 416c  ntations from Al
-00000ab0: 6275 6d65 6e74 6174 696f 6e73 2074 6f20  bumentations to 
-00000ac0: 6372 6561 7465 206e 6577 2069 6d61 6765  create new image
-00000ad0: 7320 6672 6f6d 2074 6865 206f 7269 6769  s from the origi
-00000ae0: 6e61 6c20 6f6e 653a 0a21 5b70 6172 726f  nal one:.![parro
-00000af0: 745d 2868 7474 7073 3a2f 2f68 6162 7261  t](https://habra
-00000b00: 7374 6f72 6167 652e 6f72 672f 7765 6274  storage.org/webt
-00000b10: 2f62 642f 6e65 2f72 762f 6264 6e65 7276  /bd/ne/rv/bdnerv
-00000b20: 3563 746b 7564 6d73 617a 6e68 7734 6372  5ctkudmsaznhw4cr
-00000b30: 7364 6669 772e 6a70 6567 290a 0a23 2320  sdfiw.jpeg)..## 
-00000b40: 5768 7920 416c 6275 6d65 6e74 6174 696f  Why Albumentatio
-00000b50: 6e73 0a0a 2d20 416c 6275 6d65 6e74 6174  ns..- Albumentat
-00000b60: 696f 6e73 202a 2a5b 7375 7070 6f72 7473  ions **[supports
-00000b70: 2061 6c6c 2063 6f6d 6d6f 6e20 636f 6d70   all common comp
-00000b80: 7574 6572 2076 6973 696f 6e20 7461 736b  uter vision task
-00000b90: 735d 2823 692d 7761 6e74 2d74 6f2d 7573  s](#i-want-to-us
-00000ba0: 652d 616c 6275 6d65 6e74 6174 696f 6e73  e-albumentations
-00000bb0: 2d66 6f72 2d74 6865 2d73 7065 6369 6669  -for-the-specifi
-00000bc0: 632d 7461 736b 2d73 7563 682d 6173 2d63  c-task-such-as-c
-00000bd0: 6c61 7373 6966 6963 6174 696f 6e2d 6f72  lassification-or
-00000be0: 2d73 6567 6d65 6e74 6174 696f 6e29 2a2a  -segmentation)**
-00000bf0: 2073 7563 6820 6173 2063 6c61 7373 6966   such as classif
-00000c00: 6963 6174 696f 6e2c 2073 656d 616e 7469  ication, semanti
-00000c10: 6320 7365 676d 656e 7461 7469 6f6e 2c20  c segmentation, 
-00000c20: 696e 7374 616e 6365 2073 6567 6d65 6e74  instance segment
-00000c30: 6174 696f 6e2c 206f 626a 6563 7420 6465  ation, object de
-00000c40: 7465 6374 696f 6e2c 2061 6e64 2070 6f73  tection, and pos
-00000c50: 6520 6573 7469 6d61 7469 6f6e 2e0a 2d20  e estimation..- 
-00000c60: 5468 6520 6c69 6272 6172 7920 7072 6f76  The library prov
-00000c70: 6964 6573 202a 2a5b 6120 7369 6d70 6c65  ides **[a simple
-00000c80: 2075 6e69 6669 6564 2041 5049 5d28 2361   unified API](#a
-00000c90: 2d73 696d 706c 652d 6578 616d 706c 6529  -simple-example)
-00000ca0: 2a2a 2074 6f20 776f 726b 2077 6974 6820  ** to work with 
-00000cb0: 616c 6c20 6461 7461 2074 7970 6573 3a20  all data types: 
-00000cc0: 696d 6167 6573 2028 5242 472d 696d 6167  images (RBG-imag
-00000cd0: 6573 2c20 6772 6179 7363 616c 6520 696d  es, grayscale im
-00000ce0: 6167 6573 2c20 6d75 6c74 6973 7065 6374  ages, multispect
-00000cf0: 7261 6c20 696d 6167 6573 292c 2073 6567  ral images), seg
-00000d00: 6d65 6e74 6174 696f 6e20 6d61 736b 732c  mentation masks,
-00000d10: 2062 6f75 6e64 696e 6720 626f 7865 732c   bounding boxes,
-00000d20: 2061 6e64 206b 6579 706f 696e 7473 2e0a   and keypoints..
-00000d30: 2d20 5468 6520 6c69 6272 6172 7920 636f  - The library co
-00000d40: 6e74 6169 6e73 202a 2a5b 6d6f 7265 2074  ntains **[more t
-00000d50: 6861 6e20 3730 2064 6966 6665 7265 6e74  han 70 different
-00000d60: 2061 7567 6d65 6e74 6174 696f 6e73 5d28   augmentations](
-00000d70: 236c 6973 742d 6f66 2d61 7567 6d65 6e74  #list-of-augment
-00000d80: 6174 696f 6e73 292a 2a20 746f 2067 656e  ations)** to gen
-00000d90: 6572 6174 6520 6e65 7720 7472 6169 6e69  erate new traini
-00000da0: 6e67 2073 616d 706c 6573 2066 726f 6d20  ng samples from 
-00000db0: 7468 6520 6578 6973 7469 6e67 2064 6174  the existing dat
-00000dc0: 612e 0a2d 2041 6c62 756d 656e 7461 7469  a..- Albumentati
-00000dd0: 6f6e 7320 6973 205b 2a2a 6661 7374 2a2a  ons is [**fast**
-00000de0: 5d28 2362 656e 6368 6d61 726b 696e 672d  ](#benchmarking-
-00000df0: 7265 7375 6c74 7329 2e20 5765 2062 656e  results). We ben
-00000e00: 6368 6d61 726b 2065 6163 6820 6e65 7720  chmark each new 
-00000e10: 7265 6c65 6173 6520 746f 2065 6e73 7572  release to ensur
-00000e20: 6520 7468 6174 2061 7567 6d65 6e74 6174  e that augmentat
-00000e30: 696f 6e73 2070 726f 7669 6465 206d 6178  ions provide max
-00000e40: 696d 756d 2073 7065 6564 2e0a 2d20 4974  imum speed..- It
-00000e50: 202a 2a5b 776f 726b 7320 7769 7468 2070   **[works with p
-00000e60: 6f70 756c 6172 2064 6565 7020 6c65 6172  opular deep lear
-00000e70: 6e69 6e67 2066 7261 6d65 776f 726b 735d  ning frameworks]
-00000e80: 2823 692d 7761 6e74 2d74 6f2d 6b6e 6f77  (#i-want-to-know
-00000e90: 2d68 6f77 2d74 6f2d 7573 652d 616c 6275  -how-to-use-albu
-00000ea0: 6d65 6e74 6174 696f 6e73 2d77 6974 682d  mentations-with-
-00000eb0: 6465 6570 2d6c 6561 726e 696e 672d 6672  deep-learning-fr
-00000ec0: 616d 6577 6f72 6b73 292a 2a20 7375 6368  ameworks)** such
-00000ed0: 2061 7320 5079 546f 7263 6820 616e 6420   as PyTorch and 
-00000ee0: 5465 6e73 6f72 466c 6f77 2e20 4279 2074  TensorFlow. By t
-00000ef0: 6865 2077 6179 2c20 416c 6275 6d65 6e74  he way, Albument
-00000f00: 6174 696f 6e73 2069 7320 6120 7061 7274  ations is a part
-00000f10: 206f 6620 7468 6520 5b50 7954 6f72 6368   of the [PyTorch
-00000f20: 2065 636f 7379 7374 656d 5d28 6874 7470   ecosystem](http
-00000f30: 733a 2f2f 7079 746f 7263 682e 6f72 672f  s://pytorch.org/
-00000f40: 6563 6f73 7973 7465 6d2f 292e 0a2d 205b  ecosystem/)..- [
-00000f50: 2a2a 5772 6974 7465 6e20 6279 2065 7870  **Written by exp
-00000f60: 6572 7473 2a2a 5d28 2361 7574 686f 7273  erts**](#authors
-00000f70: 292e 2054 6865 2061 7574 686f 7273 2068  ). The authors h
-00000f80: 6176 6520 6578 7065 7269 656e 6365 2062  ave experience b
-00000f90: 6f74 6820 776f 726b 696e 6720 6f6e 2070  oth working on p
-00000fa0: 726f 6475 6374 696f 6e20 636f 6d70 7574  roduction comput
-00000fb0: 6572 2076 6973 696f 6e20 7379 7374 656d  er vision system
-00000fc0: 7320 616e 6420 7061 7274 6963 6970 6174  s and participat
-00000fd0: 696e 6720 696e 2063 6f6d 7065 7469 7469  ing in competiti
-00000fe0: 7665 206d 6163 6869 6e65 206c 6561 726e  ve machine learn
-00000ff0: 696e 672e 204d 616e 7920 636f 7265 2074  ing. Many core t
-00001000: 6561 6d20 6d65 6d62 6572 7320 6172 6520  eam members are 
-00001010: 4b61 6767 6c65 204d 6173 7465 7273 2061  Kaggle Masters a
-00001020: 6e64 2047 7261 6e64 6d61 7374 6572 732e  nd Grandmasters.
-00001030: 0a2d 2054 6865 206c 6962 7261 7279 2069  .- The library i
-00001040: 7320 5b2a 2a77 6964 656c 7920 7573 6564  s [**widely used
-00001050: 2a2a 5d28 2377 686f 2d69 732d 7573 696e  **](#who-is-usin
-00001060: 672d 616c 6275 6d65 6e74 6174 696f 6e73  g-albumentations
-00001070: 2920 696e 2069 6e64 7573 7472 792c 2064  ) in industry, d
-00001080: 6565 7020 6c65 6172 6e69 6e67 2072 6573  eep learning res
-00001090: 6561 7263 682c 206d 6163 6869 6e65 206c  earch, machine l
-000010a0: 6561 726e 696e 6720 636f 6d70 6574 6974  earning competit
-000010b0: 696f 6e73 2c20 616e 6420 6f70 656e 2073  ions, and open s
-000010c0: 6f75 7263 6520 7072 6f6a 6563 7473 2e0a  ource projects..
-000010d0: 0a23 2320 5370 6f6e 736f 7273 0a0a 3c61  .## Sponsors..<a
-000010e0: 2068 7265 663d 2268 7474 7073 3a2f 2f72   href="https://r
-000010f0: 6f62 6f66 6c6f 772e 636f 6d2f 2220 7461  oboflow.com/" ta
-00001100: 7267 6574 3d22 5f62 6c61 6e6b 223e 3c69  rget="_blank"><i
-00001110: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-00001120: 6176 6174 6172 732e 6769 7468 7562 7573  avatars.githubus
-00001130: 6572 636f 6e74 656e 742e 636f 6d2f 752f  ercontent.com/u/
-00001140: 3533 3130 3431 3138 3f73 3d32 3030 2676  53104118?s=200&v
-00001150: 3d34 2220 7769 6474 683d 2231 3030 222f  =4" width="100"/
-00001160: 3e3c 2f61 3e0a 0a23 2320 5461 626c 6520  ></a>..## Table 
-00001170: 6f66 2063 6f6e 7465 6e74 730a 0a2d 205b  of contents..- [
-00001180: 416c 6275 6d65 6e74 6174 696f 6e73 5d28  Albumentations](
-00001190: 2361 6c62 756d 656e 7461 7469 6f6e 7329  #albumentations)
-000011a0: 0a20 202d 205b 5768 7920 416c 6275 6d65  .  - [Why Albume
-000011b0: 6e74 6174 696f 6e73 5d28 2377 6879 2d61  ntations](#why-a
-000011c0: 6c62 756d 656e 7461 7469 6f6e 7329 0a20  lbumentations). 
-000011d0: 202d 205b 5370 6f6e 736f 7273 5d28 2373   - [Sponsors](#s
-000011e0: 706f 6e73 6f72 7329 0a20 202d 205b 5461  ponsors).  - [Ta
-000011f0: 626c 6520 6f66 2063 6f6e 7465 6e74 735d  ble of contents]
-00001200: 2823 7461 626c 652d 6f66 2d63 6f6e 7465  (#table-of-conte
-00001210: 6e74 7329 0a20 202d 205b 4175 7468 6f72  nts).  - [Author
-00001220: 735d 2823 6175 7468 6f72 7329 0a20 202d  s](#authors).  -
-00001230: 205b 496e 7374 616c 6c61 7469 6f6e 5d28   [Installation](
-00001240: 2369 6e73 7461 6c6c 6174 696f 6e29 0a20  #installation). 
-00001250: 202d 205b 446f 6375 6d65 6e74 6174 696f   - [Documentatio
-00001260: 6e5d 2823 646f 6375 6d65 6e74 6174 696f  n](#documentatio
-00001270: 6e29 0a20 202d 205b 4120 7369 6d70 6c65  n).  - [A simple
-00001280: 2065 7861 6d70 6c65 5d28 2361 2d73 696d   example](#a-sim
-00001290: 706c 652d 6578 616d 706c 6529 0a20 202d  ple-example).  -
-000012a0: 205b 4765 7474 696e 6720 7374 6172 7465   [Getting starte
-000012b0: 645d 2823 6765 7474 696e 672d 7374 6172  d](#getting-star
-000012c0: 7465 6429 0a20 2020 202d 205b 4920 616d  ted).    - [I am
-000012d0: 206e 6577 2074 6f20 696d 6167 6520 6175   new to image au
-000012e0: 676d 656e 7461 7469 6f6e 5d28 2369 2d61  gmentation](#i-a
-000012f0: 6d2d 6e65 772d 746f 2d69 6d61 6765 2d61  m-new-to-image-a
-00001300: 7567 6d65 6e74 6174 696f 6e29 0a20 2020  ugmentation).   
-00001310: 202d 205b 4920 7761 6e74 2074 6f20 7573   - [I want to us
-00001320: 6520 416c 6275 6d65 6e74 6174 696f 6e73  e Albumentations
-00001330: 2066 6f72 2074 6865 2073 7065 6369 6669   for the specifi
-00001340: 6320 7461 736b 2073 7563 6820 6173 2063  c task such as c
-00001350: 6c61 7373 6966 6963 6174 696f 6e20 6f72  lassification or
-00001360: 2073 6567 6d65 6e74 6174 696f 6e5d 2823   segmentation](#
-00001370: 692d 7761 6e74 2d74 6f2d 7573 652d 616c  i-want-to-use-al
-00001380: 6275 6d65 6e74 6174 696f 6e73 2d66 6f72  bumentations-for
-00001390: 2d74 6865 2d73 7065 6369 6669 632d 7461  -the-specific-ta
-000013a0: 736b 2d73 7563 682d 6173 2d63 6c61 7373  sk-such-as-class
-000013b0: 6966 6963 6174 696f 6e2d 6f72 2d73 6567  ification-or-seg
-000013c0: 6d65 6e74 6174 696f 6e29 0a20 2020 202d  mentation).    -
-000013d0: 205b 4920 7761 6e74 2074 6f20 6b6e 6f77   [I want to know
-000013e0: 2068 6f77 2074 6f20 7573 6520 416c 6275   how to use Albu
-000013f0: 6d65 6e74 6174 696f 6e73 2077 6974 6820  mentations with 
-00001400: 6465 6570 206c 6561 726e 696e 6720 6672  deep learning fr
-00001410: 616d 6577 6f72 6b73 5d28 2369 2d77 616e  ameworks](#i-wan
-00001420: 742d 746f 2d6b 6e6f 772d 686f 772d 746f  t-to-know-how-to
-00001430: 2d75 7365 2d61 6c62 756d 656e 7461 7469  -use-albumentati
-00001440: 6f6e 732d 7769 7468 2d64 6565 702d 6c65  ons-with-deep-le
-00001450: 6172 6e69 6e67 2d66 7261 6d65 776f 726b  arning-framework
-00001460: 7329 0a20 2020 202d 205b 4920 7761 6e74  s).    - [I want
-00001470: 2074 6f20 6578 706c 6f72 6520 6175 676d   to explore augm
-00001480: 656e 7461 7469 6f6e 7320 616e 6420 7365  entations and se
-00001490: 6520 416c 6275 6d65 6e74 6174 696f 6e73  e Albumentations
-000014a0: 2069 6e20 6163 7469 6f6e 5d28 2369 2d77   in action](#i-w
-000014b0: 616e 742d 746f 2d65 7870 6c6f 7265 2d61  ant-to-explore-a
-000014c0: 7567 6d65 6e74 6174 696f 6e73 2d61 6e64  ugmentations-and
-000014d0: 2d73 6565 2d61 6c62 756d 656e 7461 7469  -see-albumentati
-000014e0: 6f6e 732d 696e 2d61 6374 696f 6e29 0a20  ons-in-action). 
-000014f0: 202d 205b 5768 6f20 6973 2075 7369 6e67   - [Who is using
-00001500: 2041 6c62 756d 656e 7461 7469 6f6e 735d   Albumentations]
-00001510: 2823 7768 6f2d 6973 2d75 7369 6e67 2d61  (#who-is-using-a
-00001520: 6c62 756d 656e 7461 7469 6f6e 7329 0a20  lbumentations). 
-00001530: 2020 202d 205b 5365 6520 616c 736f 5d28     - [See also](
-00001540: 2373 6565 2d61 6c73 6f29 0a20 202d 205b  #see-also).  - [
-00001550: 4c69 7374 206f 6620 6175 676d 656e 7461  List of augmenta
-00001560: 7469 6f6e 735d 2823 6c69 7374 2d6f 662d  tions](#list-of-
-00001570: 6175 676d 656e 7461 7469 6f6e 7329 0a20  augmentations). 
-00001580: 2020 202d 205b 5069 7865 6c2d 6c65 7665     - [Pixel-leve
-00001590: 6c20 7472 616e 7366 6f72 6d73 5d28 2370  l transforms](#p
-000015a0: 6978 656c 2d6c 6576 656c 2d74 7261 6e73  ixel-level-trans
-000015b0: 666f 726d 7329 0a20 2020 202d 205b 5370  forms).    - [Sp
-000015c0: 6174 6961 6c2d 6c65 7665 6c20 7472 616e  atial-level tran
-000015d0: 7366 6f72 6d73 5d28 2373 7061 7469 616c  sforms](#spatial
-000015e0: 2d6c 6576 656c 2d74 7261 6e73 666f 726d  -level-transform
-000015f0: 7329 0a20 2020 202d 205b 4d69 7869 6e67  s).    - [Mixing
-00001600: 2d6c 6576 656c 2074 7261 6e73 666f 726d  -level transform
-00001610: 735d 2823 6d69 7869 6e67 2d6c 6576 656c  s](#mixing-level
-00001620: 2d74 7261 6e73 666f 726d 7329 0a20 202d  -transforms).  -
-00001630: 205b 4120 6665 7720 6d6f 7265 2065 7861   [A few more exa
-00001640: 6d70 6c65 7320 6f66 202a 2a61 7567 6d65  mples of **augme
-00001650: 6e74 6174 696f 6e73 2a2a 5d28 2361 2d66  ntations**](#a-f
-00001660: 6577 2d6d 6f72 652d 6578 616d 706c 6573  ew-more-examples
-00001670: 2d6f 662d 6175 676d 656e 7461 7469 6f6e  -of-augmentation
-00001680: 7329 0a20 2020 202d 205b 5365 6d61 6e74  s).    - [Semant
-00001690: 6963 2073 6567 6d65 6e74 6174 696f 6e20  ic segmentation 
-000016a0: 6f6e 2074 6865 2049 6e72 6961 2064 6174  on the Inria dat
-000016b0: 6173 6574 5d28 2373 656d 616e 7469 632d  aset](#semantic-
-000016c0: 7365 676d 656e 7461 7469 6f6e 2d6f 6e2d  segmentation-on-
-000016d0: 7468 652d 696e 7269 612d 6461 7461 7365  the-inria-datase
-000016e0: 7429 0a20 2020 202d 205b 4d65 6469 6361  t).    - [Medica
-000016f0: 6c20 696d 6167 696e 675d 2823 6d65 6469  l imaging](#medi
-00001700: 6361 6c2d 696d 6167 696e 6729 0a20 2020  cal-imaging).   
-00001710: 202d 205b 4f62 6a65 6374 2064 6574 6563   - [Object detec
-00001720: 7469 6f6e 2061 6e64 2073 656d 616e 7469  tion and semanti
-00001730: 6320 7365 676d 656e 7461 7469 6f6e 206f  c segmentation o
-00001740: 6e20 7468 6520 4d61 7069 6c6c 6172 7920  n the Mapillary 
-00001750: 5669 7374 6173 2064 6174 6173 6574 5d28  Vistas dataset](
-00001760: 236f 626a 6563 742d 6465 7465 6374 696f  #object-detectio
-00001770: 6e2d 616e 642d 7365 6d61 6e74 6963 2d73  n-and-semantic-s
-00001780: 6567 6d65 6e74 6174 696f 6e2d 6f6e 2d74  egmentation-on-t
-00001790: 6865 2d6d 6170 696c 6c61 7279 2d76 6973  he-mapillary-vis
-000017a0: 7461 732d 6461 7461 7365 7429 0a20 2020  tas-dataset).   
-000017b0: 202d 205b 4b65 7970 6f69 6e74 7320 6175   - [Keypoints au
-000017c0: 676d 656e 7461 7469 6f6e 5d28 236b 6579  gmentation](#key
-000017d0: 706f 696e 7473 2d61 7567 6d65 6e74 6174  points-augmentat
-000017e0: 696f 6e29 0a20 202d 205b 4265 6e63 686d  ion).  - [Benchm
-000017f0: 6172 6b69 6e67 2072 6573 756c 7473 5d28  arking results](
-00001800: 2362 656e 6368 6d61 726b 696e 672d 7265  #benchmarking-re
-00001810: 7375 6c74 7329 0a20 202d 205b 436f 6e74  sults).  - [Cont
-00001820: 7269 6275 7469 6e67 5d28 2363 6f6e 7472  ributing](#contr
-00001830: 6962 7574 696e 6729 0a20 202d 205b 436f  ibuting).  - [Co
-00001840: 6d6d 756e 6974 7920 616e 6420 5375 7070  mmunity and Supp
-00001850: 6f72 745d 2823 636f 6d6d 756e 6974 792d  ort](#community-
-00001860: 616e 642d 7375 7070 6f72 7429 0a20 202d  and-support).  -
-00001870: 205b 436f 6d6d 656e 7473 5d28 2363 6f6d   [Comments](#com
-00001880: 6d65 6e74 7329 0a20 202d 205b 4369 7469  ments).  - [Citi
-00001890: 6e67 5d28 2363 6974 696e 6729 0a0a 2323  ng](#citing)..##
-000018a0: 2041 7574 686f 7273 0a0a 5b2a 2a56 6c61   Authors..[**Vla
-000018b0: 6469 6d69 7220 492e 2049 676c 6f76 696b  dimir I. Iglovik
-000018c0: 6f76 2a2a 5d28 6874 7470 733a 2f2f 7777  ov**](https://ww
-000018d0: 772e 6c69 6e6b 6564 696e 2e63 6f6d 2f69  w.linkedin.com/i
-000018e0: 6e2f 6967 6c6f 7669 6b6f 762f 2920 7c20  n/iglovikov/) | 
-000018f0: 5b4b 6167 676c 6520 4772 616e 646d 6173  [Kaggle Grandmas
-00001900: 7465 725d 2868 7474 7073 3a2f 2f77 7777  ter](https://www
-00001910: 2e6b 6167 676c 652e 636f 6d2f 6967 6c6f  .kaggle.com/iglo
-00001920: 7669 6b6f 7629 0a0a 5b2a 2a4d 696b 6861  vikov)..[**Mikha
-00001930: 696c 2044 7275 7a68 696e 696e 2a2a 5d28  il Druzhinin**](
-00001940: 6874 7470 733a 2f2f 7777 772e 6c69 6e6b  https://www.link
-00001950: 6564 696e 2e63 6f6d 2f69 6e2f 6d69 6b68  edin.com/in/mikh
-00001960: 6169 6c2d 6472 757a 6869 6e69 6e2d 3534  ail-druzhinin-54
-00001970: 3832 3239 3130 302f 2920 7c20 5b4b 6167  8229100/) | [Kag
-00001980: 676c 6520 4578 7065 7274 5d28 6874 7470  gle Expert](http
-00001990: 733a 2f2f 7777 772e 6b61 6767 6c65 2e63  s://www.kaggle.c
-000019a0: 6f6d 2f64 6970 6574 6d29 0a0a 5b2a 2a41  om/dipetm)..[**A
-000019b0: 6c65 7820 5061 7269 6e6f 762a 2a5d 2868  lex Parinov**](h
-000019c0: 7474 7073 3a2f 2f77 7777 2e6c 696e 6b65  ttps://www.linke
-000019d0: 6469 6e2e 636f 6d2f 696e 2f61 6c65 782d  din.com/in/alex-
-000019e0: 7061 7269 6e6f 762f 2920 7c20 5b4b 6167  parinov/) | [Kag
-000019f0: 676c 6520 4d61 7374 6572 5d28 6874 7470  gle Master](http
-00001a00: 733a 2f2f 7777 772e 6b61 6767 6c65 2e63  s://www.kaggle.c
-00001a10: 6f6d 2f63 7265 6166 7a29 0a0a 5b2a 2a41  om/creafz)..[**A
-00001a20: 6c65 7861 6e64 6572 2042 7573 6c61 6576  lexander Buslaev
-00001a30: 2a2a 20e2 8094 2043 6f6d 7075 7465 7220  ** ... Computer 
-00001a40: 5669 7369 6f6e 2045 6e67 696e 6565 7220  Vision Engineer 
-00001a50: 6174 204d 6170 626f 785d 2868 7474 7073  at Mapbox](https
-00001a60: 3a2f 2f77 7777 2e6c 696e 6b65 6469 6e2e  ://www.linkedin.
-00001a70: 636f 6d2f 696e 2f61 6c2d 6275 736c 6165  com/in/al-buslae
-00001a80: 762f 2920 7c20 5b4b 6167 676c 6520 4d61  v/) | [Kaggle Ma
-00001a90: 7374 6572 5d28 6874 7470 733a 2f2f 7777  ster](https://ww
-00001aa0: 772e 6b61 6767 6c65 2e63 6f6d 2f61 6c62  w.kaggle.com/alb
-00001ab0: 7573 6c61 6576 290a 0a5b 2a2a 4576 6567  uslaev)..[**Eveg
-00001ac0: 656e 6520 4b68 7665 6463 6865 6e79 612a  ene Khvedchenya*
-00001ad0: 2a20 e280 9420 436f 6d70 7574 6572 2056  * ... Computer V
-00001ae0: 6973 696f 6e20 5265 7365 6172 6368 2045  ision Research E
-00001af0: 6e67 696e 6565 7220 6174 2050 69c3 b161  ngineer at Pi..a
-00001b00: 7461 2046 6172 6d73 5d28 6874 7470 733a  ta Farms](https:
-00001b10: 2f2f 7777 772e 6c69 6e6b 6564 696e 2e63  //www.linkedin.c
-00001b20: 6f6d 2f69 6e2f 6376 7461 6c6b 732f 2920  om/in/cvtalks/) 
-00001b30: 7c20 5b4b 6167 676c 6520 4772 616e 646d  | [Kaggle Grandm
-00001b40: 6173 7465 725d 2868 7474 7073 3a2f 2f77  aster](https://w
-00001b50: 7777 2e6b 6167 676c 652e 636f 6d2f 626c  ww.kaggle.com/bl
-00001b60: 6f6f 6461 7865 290a 0a23 2320 496e 7374  oodaxe)..## Inst
-00001b70: 616c 6c61 7469 6f6e 0a0a 416c 6275 6d65  allation..Albume
-00001b80: 6e74 6174 696f 6e73 2072 6571 7569 7265  ntations require
-00001b90: 7320 5079 7468 6f6e 2033 2e38 206f 7220  s Python 3.8 or 
-00001ba0: 6869 6768 6572 2e20 546f 2069 6e73 7461  higher. To insta
-00001bb0: 6c6c 2074 6865 206c 6174 6573 7420 7665  ll the latest ve
-00001bc0: 7273 696f 6e20 6672 6f6d 2050 7950 493a  rsion from PyPI:
-00001bd0: 0a0a 6060 6062 6173 680a 7069 7020 696e  ..```bash.pip in
-00001be0: 7374 616c 6c20 2d55 2061 6c62 756d 656e  stall -U albumen
-00001bf0: 7461 7469 6f6e 730a 6060 600a 0a4f 7468  tations.```..Oth
-00001c00: 6572 2069 6e73 7461 6c6c 6174 696f 6e20  er installation 
-00001c10: 6f70 7469 6f6e 7320 6172 6520 6465 7363  options are desc
-00001c20: 7269 6265 6420 696e 2074 6865 205b 646f  ribed in the [do
-00001c30: 6375 6d65 6e74 6174 696f 6e5d 2868 7474  cumentation](htt
-00001c40: 7073 3a2f 2f61 6c62 756d 656e 7461 7469  ps://albumentati
-00001c50: 6f6e 732e 6169 2f64 6f63 732f 6765 7474  ons.ai/docs/gett
-00001c60: 696e 675f 7374 6172 7465 642f 696e 7374  ing_started/inst
-00001c70: 616c 6c61 7469 6f6e 2f29 2e0a 0a23 2320  allation/)...## 
-00001c80: 446f 6375 6d65 6e74 6174 696f 6e0a 0a54  Documentation..T
-00001c90: 6865 2066 756c 6c20 646f 6375 6d65 6e74  he full document
-00001ca0: 6174 696f 6e20 6973 2061 7661 696c 6162  ation is availab
-00001cb0: 6c65 2061 7420 2a2a 5b68 7474 7073 3a2f  le at **[https:/
-00001cc0: 2f61 6c62 756d 656e 7461 7469 6f6e 732e  /albumentations.
-00001cd0: 6169 2f64 6f63 732f 5d28 6874 7470 733a  ai/docs/](https:
-00001ce0: 2f2f 616c 6275 6d65 6e74 6174 696f 6e73  //albumentations
-00001cf0: 2e61 692f 646f 6373 2f29 2a2a 2e0a 0a23  .ai/docs/)**...#
-00001d00: 2320 4120 7369 6d70 6c65 2065 7861 6d70  # A simple examp
-00001d10: 6c65 0a0a 6060 6070 7974 686f 6e0a 696d  le..```python.im
-00001d20: 706f 7274 2061 6c62 756d 656e 7461 7469  port albumentati
-00001d30: 6f6e 7320 6173 2041 0a69 6d70 6f72 7420  ons as A.import 
-00001d40: 6376 320a 0a23 2044 6563 6c61 7265 2061  cv2..# Declare a
-00001d50: 6e20 6175 676d 656e 7461 7469 6f6e 2070  n augmentation p
-00001d60: 6970 656c 696e 650a 7472 616e 7366 6f72  ipeline.transfor
-00001d70: 6d20 3d20 412e 436f 6d70 6f73 6528 5b0a  m = A.Compose([.
-00001d80: 2020 2020 412e 5261 6e64 6f6d 4372 6f70      A.RandomCrop
-00001d90: 2877 6964 7468 3d32 3536 2c20 6865 6967  (width=256, heig
-00001da0: 6874 3d32 3536 292c 0a20 2020 2041 2e48  ht=256),.    A.H
-00001db0: 6f72 697a 6f6e 7461 6c46 6c69 7028 703d  orizontalFlip(p=
-00001dc0: 302e 3529 2c0a 2020 2020 412e 5261 6e64  0.5),.    A.Rand
-00001dd0: 6f6d 4272 6967 6874 6e65 7373 436f 6e74  omBrightnessCont
-00001de0: 7261 7374 2870 3d30 2e32 292c 0a5d 290a  rast(p=0.2),.]).
-00001df0: 0a23 2052 6561 6420 616e 2069 6d61 6765  .# Read an image
-00001e00: 2077 6974 6820 4f70 656e 4356 2061 6e64   with OpenCV and
-00001e10: 2063 6f6e 7665 7274 2069 7420 746f 2074   convert it to t
-00001e20: 6865 2052 4742 2063 6f6c 6f72 7370 6163  he RGB colorspac
-00001e30: 650a 696d 6167 6520 3d20 6376 322e 696d  e.image = cv2.im
-00001e40: 7265 6164 2822 696d 6167 652e 6a70 6722  read("image.jpg"
-00001e50: 290a 696d 6167 6520 3d20 6376 322e 6376  ).image = cv2.cv
-00001e60: 7443 6f6c 6f72 2869 6d61 6765 2c20 6376  tColor(image, cv
-00001e70: 322e 434f 4c4f 525f 4247 5232 5247 4229  2.COLOR_BGR2RGB)
-00001e80: 0a0a 2320 4175 676d 656e 7420 616e 2069  ..# Augment an i
-00001e90: 6d61 6765 0a74 7261 6e73 666f 726d 6564  mage.transformed
-00001ea0: 203d 2074 7261 6e73 666f 726d 2869 6d61   = transform(ima
-00001eb0: 6765 3d69 6d61 6765 290a 7472 616e 7366  ge=image).transf
-00001ec0: 6f72 6d65 645f 696d 6167 6520 3d20 7472  ormed_image = tr
-00001ed0: 616e 7366 6f72 6d65 645b 2269 6d61 6765  ansformed["image
-00001ee0: 225d 0a60 6060 0a0a 2323 2047 6574 7469  "].```..## Getti
-00001ef0: 6e67 2073 7461 7274 6564 0a0a 2323 2320  ng started..### 
-00001f00: 4920 616d 206e 6577 2074 6f20 696d 6167  I am new to imag
-00001f10: 6520 6175 676d 656e 7461 7469 6f6e 0a0a  e augmentation..
-00001f20: 506c 6561 7365 2073 7461 7274 2077 6974  Please start wit
-00001f30: 6820 7468 6520 5b69 6e74 726f 6475 6374  h the [introduct
-00001f40: 696f 6e20 6172 7469 636c 6573 5d28 6874  ion articles](ht
-00001f50: 7470 733a 2f2f 616c 6275 6d65 6e74 6174  tps://albumentat
-00001f60: 696f 6e73 2e61 692f 646f 6373 2f23 696e  ions.ai/docs/#in
-00001f70: 7472 6f64 7563 7469 6f6e 2d74 6f2d 696d  troduction-to-im
-00001f80: 6167 652d 6175 676d 656e 7461 7469 6f6e  age-augmentation
-00001f90: 2920 6162 6f75 7420 7768 7920 696d 6167  ) about why imag
-00001fa0: 6520 6175 676d 656e 7461 7469 6f6e 2069  e augmentation i
-00001fb0: 7320 696d 706f 7274 616e 7420 616e 6420  s important and 
-00001fc0: 686f 7720 6974 2068 656c 7073 2074 6f20  how it helps to 
-00001fd0: 6275 696c 6420 6265 7474 6572 206d 6f64  build better mod
-00001fe0: 656c 732e 0a0a 2323 2320 4920 7761 6e74  els...### I want
-00001ff0: 2074 6f20 7573 6520 416c 6275 6d65 6e74   to use Albument
-00002000: 6174 696f 6e73 2066 6f72 2074 6865 2073  ations for the s
-00002010: 7065 6369 6669 6320 7461 736b 2073 7563  pecific task suc
-00002020: 6820 6173 2063 6c61 7373 6966 6963 6174  h as classificat
-00002030: 696f 6e20 6f72 2073 6567 6d65 6e74 6174  ion or segmentat
-00002040: 696f 6e0a 0a49 6620 796f 7520 7761 6e74  ion..If you want
-00002050: 2074 6f20 7573 6520 416c 6275 6d65 6e74   to use Albument
-00002060: 6174 696f 6e73 2066 6f72 2061 2073 7065  ations for a spe
-00002070: 6369 6669 6320 7461 736b 2073 7563 6820  cific task such 
-00002080: 6173 2063 6c61 7373 6966 6963 6174 696f  as classificatio
-00002090: 6e2c 2073 6567 6d65 6e74 6174 696f 6e2c  n, segmentation,
-000020a0: 206f 7220 6f62 6a65 6374 2064 6574 6563   or object detec
-000020b0: 7469 6f6e 2c20 7265 6665 7220 746f 2074  tion, refer to t
-000020c0: 6865 205b 7365 7420 6f66 2061 7274 6963  he [set of artic
-000020d0: 6c65 735d 2868 7474 7073 3a2f 2f61 6c62  les](https://alb
-000020e0: 756d 656e 7461 7469 6f6e 732e 6169 2f64  umentations.ai/d
-000020f0: 6f63 732f 2367 6574 7469 6e67 2d73 7461  ocs/#getting-sta
-00002100: 7274 6564 2d77 6974 682d 616c 6275 6d65  rted-with-albume
-00002110: 6e74 6174 696f 6e73 2920 7468 6174 2068  ntations) that h
-00002120: 6173 2061 6e20 696e 2d64 6570 7468 2064  as an in-depth d
-00002130: 6573 6372 6970 7469 6f6e 206f 6620 7468  escription of th
-00002140: 6973 2074 6173 6b2e 2057 6520 616c 736f  is task. We also
-00002150: 2068 6176 6520 6120 5b6c 6973 7420 6f66   have a [list of
-00002160: 2065 7861 6d70 6c65 735d 2868 7474 7073   examples](https
-00002170: 3a2f 2f61 6c62 756d 656e 7461 7469 6f6e  ://albumentation
-00002180: 732e 6169 2f64 6f63 732f 6578 616d 706c  s.ai/docs/exampl
-00002190: 6573 2f29 206f 6e20 6170 706c 7969 6e67  es/) on applying
-000021a0: 2041 6c62 756d 656e 7461 7469 6f6e 7320   Albumentations 
-000021b0: 666f 7220 6469 6666 6572 656e 7420 7573  for different us
-000021c0: 6520 6361 7365 732e 0a0a 2323 2320 4920  e cases...### I 
-000021d0: 7761 6e74 2074 6f20 6b6e 6f77 2068 6f77  want to know how
-000021e0: 2074 6f20 7573 6520 416c 6275 6d65 6e74   to use Albument
-000021f0: 6174 696f 6e73 2077 6974 6820 6465 6570  ations with deep
-00002200: 206c 6561 726e 696e 6720 6672 616d 6577   learning framew
-00002210: 6f72 6b73 0a0a 5765 2068 6176 6520 5b65  orks..We have [e
-00002220: 7861 6d70 6c65 7320 6f66 2075 7369 6e67  xamples of using
-00002230: 2041 6c62 756d 656e 7461 7469 6f6e 735d   Albumentations]
-00002240: 2868 7474 7073 3a2f 2f61 6c62 756d 656e  (https://albumen
-00002250: 7461 7469 6f6e 732e 6169 2f64 6f63 732f  tations.ai/docs/
-00002260: 2365 7861 6d70 6c65 732d 6f66 2d68 6f77  #examples-of-how
-00002270: 2d74 6f2d 7573 652d 616c 6275 6d65 6e74  -to-use-albument
-00002280: 6174 696f 6e73 2d77 6974 682d 6469 6666  ations-with-diff
-00002290: 6572 656e 742d 6465 6570 2d6c 6561 726e  erent-deep-learn
-000022a0: 696e 672d 6672 616d 6577 6f72 6b73 2920  ing-frameworks) 
-000022b0: 616c 6f6e 6720 7769 7468 2050 7954 6f72  along with PyTor
-000022c0: 6368 2061 6e64 2054 656e 736f 7246 6c6f  ch and TensorFlo
-000022d0: 772e 0a0a 2323 2320 4920 7761 6e74 2074  w...### I want t
-000022e0: 6f20 6578 706c 6f72 6520 6175 676d 656e  o explore augmen
-000022f0: 7461 7469 6f6e 7320 616e 6420 7365 6520  tations and see 
-00002300: 416c 6275 6d65 6e74 6174 696f 6e73 2069  Albumentations i
-00002310: 6e20 6163 7469 6f6e 0a0a 4368 6563 6b20  n action..Check 
-00002320: 7468 6520 5b6f 6e6c 696e 6520 6465 6d6f  the [online demo
-00002330: 206f 6620 7468 6520 6c69 6272 6172 795d   of the library]
-00002340: 2868 7474 7073 3a2f 2f61 6c62 756d 656e  (https://albumen
-00002350: 7461 7469 6f6e 732d 6465 6d6f 2e68 6572  tations-demo.her
-00002360: 6f6b 7561 7070 2e63 6f6d 2f29 2e20 5769  okuapp.com/). Wi
-00002370: 7468 2069 742c 2079 6f75 2063 616e 2061  th it, you can a
-00002380: 7070 6c79 2061 7567 6d65 6e74 6174 696f  pply augmentatio
-00002390: 6e73 2074 6f20 6469 6666 6572 656e 7420  ns to different 
-000023a0: 696d 6167 6573 2061 6e64 2073 6565 2074  images and see t
-000023b0: 6865 2072 6573 756c 742e 2041 6c73 6f2c  he result. Also,
-000023c0: 2077 6520 6861 7665 2061 205b 6c69 7374   we have a [list
-000023d0: 206f 6620 616c 6c20 6176 6169 6c61 626c   of all availabl
-000023e0: 6520 6175 676d 656e 7461 7469 6f6e 7320  e augmentations 
-000023f0: 616e 6420 7468 6569 7220 7461 7267 6574  and their target
-00002400: 735d 2823 6c69 7374 2d6f 662d 6175 676d  s](#list-of-augm
-00002410: 656e 7461 7469 6f6e 7329 2e0a 0a23 2320  entations)...## 
-00002420: 5768 6f20 6973 2075 7369 6e67 2041 6c62  Who is using Alb
-00002430: 756d 656e 7461 7469 6f6e 730a 0a3c 6120  umentations..<a 
-00002440: 6872 6566 3d22 6874 7470 733a 2f2f 7777  href="https://ww
-00002450: 772e 6170 706c 652e 636f 6d2f 2220 7461  w.apple.com/" ta
-00002460: 7267 6574 3d22 5f62 6c61 6e6b 223e 3c69  rget="_blank"><i
-00002470: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-00002480: 7261 772e 6769 7468 7562 7573 6572 636f  raw.githubuserco
-00002490: 6e74 656e 742e 636f 6d2f 616c 6275 6d65  ntent.com/albume
-000024a0: 6e74 6174 696f 6e73 2d74 6561 6d2f 616c  ntations-team/al
-000024b0: 6275 6d65 6e74 6174 696f 6e73 2e61 692f  bumentations.ai/
-000024c0: 6d61 696e 2f68 746d 6c2f 6173 7365 7473  main/html/assets
-000024d0: 2f69 6d67 2f69 6e64 7573 7472 792f 6170  /img/industry/ap
-000024e0: 706c 652e 6a70 6567 2220 7769 6474 683d  ple.jpeg" width=
-000024f0: 2231 3030 222f 3e3c 2f61 3e0a 3c61 2068  "100"/></a>.<a h
-00002500: 7265 663d 2268 7474 7073 3a2f 2f72 6573  ref="https://res
-00002510: 6561 7263 682e 676f 6f67 6c65 2f22 2074  earch.google/" t
-00002520: 6172 6765 743d 225f 626c 616e 6b22 3e3c  arget="_blank"><
-00002530: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-00002540: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
-00002550: 6f6e 7465 6e74 2e63 6f6d 2f61 6c62 756d  ontent.com/album
-00002560: 656e 7461 7469 6f6e 732d 7465 616d 2f61  entations-team/a
-00002570: 6c62 756d 656e 7461 7469 6f6e 732e 6169  lbumentations.ai
-00002580: 2f6d 6169 6e2f 6874 6d6c 2f61 7373 6574  /main/html/asset
-00002590: 732f 696d 672f 696e 6475 7374 7279 2f67  s/img/industry/g
-000025a0: 6f6f 676c 652e 706e 6722 2077 6964 7468  oogle.png" width
-000025b0: 3d22 3130 3022 2f3e 3c2f 613e 0a3c 6120  ="100"/></a>.<a 
-000025c0: 6872 6566 3d22 6874 7470 733a 2f2f 6f70  href="https://op
-000025d0: 656e 736f 7572 6365 2e66 622e 636f 6d2f  ensource.fb.com/
-000025e0: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
-000025f0: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
-00002600: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
-00002610: 6572 636f 6e74 656e 742e 636f 6d2f 616c  ercontent.com/al
-00002620: 6275 6d65 6e74 6174 696f 6e73 2d74 6561  bumentations-tea
-00002630: 6d2f 616c 6275 6d65 6e74 6174 696f 6e73  m/albumentations
-00002640: 2e61 692f 6d61 696e 2f68 746d 6c2f 6173  .ai/main/html/as
-00002650: 7365 7473 2f69 6d67 2f69 6e64 7573 7472  sets/img/industr
-00002660: 792f 6d65 7461 5f72 6573 6561 7263 682e  y/meta_research.
-00002670: 706e 6722 2077 6964 7468 3d22 3130 3022  png" width="100"
-00002680: 2f3e 3c2f 613e 0a3c 6120 6872 6566 3d22  /></a>.<a href="
-00002690: 6874 7470 733a 202f 2f77 7777 2e6e 7669  https: //www.nvi
-000026a0: 6469 612e 636f 6d2f 656e 2d75 732f 7265  dia.com/en-us/re
-000026b0: 7365 6172 6368 2f22 2074 6172 6765 743d  search/" target=
-000026c0: 225f 626c 616e 6b22 3e3c 696d 6720 7372  "_blank"><img sr
-000026d0: 633d 2268 7474 7073 3a2f 2f72 6177 2e67  c="https://raw.g
-000026e0: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
-000026f0: 2e63 6f6d 2f61 6c62 756d 656e 7461 7469  .com/albumentati
-00002700: 6f6e 732d 7465 616d 2f61 6c62 756d 656e  ons-team/albumen
-00002710: 7461 7469 6f6e 732e 6169 2f6d 6169 6e2f  tations.ai/main/
-00002720: 6874 6d6c 2f61 7373 6574 732f 696d 672f  html/assets/img/
-00002730: 696e 6475 7374 7279 2f6e 7669 6469 615f  industry/nvidia_
-00002740: 7265 7365 6172 6368 2e6a 7065 6722 2077  research.jpeg" w
-00002750: 6964 7468 3d22 3130 3022 2f3e 3c2f 613e  idth="100"/></a>
-00002760: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
-00002770: 2f2f 7777 772e 616d 617a 6f6e 2e73 6369  //www.amazon.sci
-00002780: 656e 6365 2f22 2074 6172 6765 743d 225f  ence/" target="_
-00002790: 626c 616e 6b22 3e3c 696d 6720 7372 633d  blank"><img src=
-000027a0: 2268 7474 7073 3a2f 2f72 6177 2e67 6974  "https://raw.git
-000027b0: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
-000027c0: 6f6d 2f61 6c62 756d 656e 7461 7469 6f6e  om/albumentation
-000027d0: 732d 7465 616d 2f61 6c62 756d 656e 7461  s-team/albumenta
-000027e0: 7469 6f6e 732e 6169 2f6d 6169 6e2f 6874  tions.ai/main/ht
-000027f0: 6d6c 2f61 7373 6574 732f 696d 672f 696e  ml/assets/img/in
-00002800: 6475 7374 7279 2f61 6d61 7a6f 6e5f 7363  dustry/amazon_sc
-00002810: 6965 6e63 652e 706e 6722 2077 6964 7468  ience.png" width
-00002820: 3d22 3130 3022 2f3e 3c2f 613e 0a3c 6120  ="100"/></a>.<a 
-00002830: 6872 6566 3d22 6874 7470 733a 2f2f 6f70  href="https://op
-00002840: 656e 736f 7572 6365 2e6d 6963 726f 736f  ensource.microso
-00002850: 6674 2e63 6f6d 2f22 2074 6172 6765 743d  ft.com/" target=
-00002860: 225f 626c 616e 6b22 3e3c 696d 6720 7372  "_blank"><img sr
-00002870: 633d 2268 7474 7073 3a2f 2f72 6177 2e67  c="https://raw.g
-00002880: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
-00002890: 2e63 6f6d 2f61 6c62 756d 656e 7461 7469  .com/albumentati
-000028a0: 6f6e 732d 7465 616d 2f61 6c62 756d 656e  ons-team/albumen
-000028b0: 7461 7469 6f6e 732e 6169 2f6d 6169 6e2f  tations.ai/main/
-000028c0: 6874 6d6c 2f61 7373 6574 732f 696d 672f  html/assets/img/
-000028d0: 696e 6475 7374 7279 2f6d 6963 726f 736f  industry/microso
-000028e0: 6674 2e70 6e67 2220 7769 6474 683d 2231  ft.png" width="1
-000028f0: 3030 222f 3e3c 2f61 3e0a 3c61 2068 7265  00"/></a>.<a hre
-00002900: 663d 2268 7474 7073 3a2f 2f65 6e67 696e  f="https://engin
-00002910: 6565 7269 6e67 2e73 616c 6573 666f 7263  eering.salesforc
-00002920: 652e 636f 6d2f 6f70 656e 2d73 6f75 7263  e.com/open-sourc
-00002930: 652f 2220 7461 7267 6574 3d22 5f62 6c61  e/" target="_bla
-00002940: 6e6b 223e 3c69 6d67 2073 7263 3d22 6874  nk"><img src="ht
-00002950: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
-00002960: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
-00002970: 616c 6275 6d65 6e74 6174 696f 6e73 2d74  albumentations-t
-00002980: 6561 6d2f 616c 6275 6d65 6e74 6174 696f  eam/albumentatio
-00002990: 6e73 2e61 692f 6d61 696e 2f68 746d 6c2f  ns.ai/main/html/
-000029a0: 6173 7365 7473 2f69 6d67 2f69 6e64 7573  assets/img/indus
-000029b0: 7472 792f 7361 6c65 7366 6f72 6365 5f6f  try/salesforce_o
-000029c0: 7065 6e5f 736f 7572 6365 2e70 6e67 2220  pen_source.png" 
-000029d0: 7769 6474 683d 2231 3030 222f 3e3c 2f61  width="100"/></a
-000029e0: 3e0a 3c61 2068 7265 663d 2268 7474 7073  >.<a href="https
-000029f0: 3a2f 2f73 7461 6269 6c69 7479 2e61 692f  ://stability.ai/
-00002a00: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
-00002a10: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
-00002a20: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
-00002a30: 6572 636f 6e74 656e 742e 636f 6d2f 616c  ercontent.com/al
-00002a40: 6275 6d65 6e74 6174 696f 6e73 2d74 6561  bumentations-tea
-00002a50: 6d2f 616c 6275 6d65 6e74 6174 696f 6e73  m/albumentations
-00002a60: 2e61 692f 6d61 696e 2f68 746d 6c2f 6173  .ai/main/html/as
-00002a70: 7365 7473 2f69 6d67 2f69 6e64 7573 7472  sets/img/industr
-00002a80: 792f 7374 6162 696c 6974 792e 706e 6722  y/stability.png"
-00002a90: 2077 6964 7468 3d22 3130 3022 2f3e 3c2f   width="100"/></
-00002aa0: 613e 0a3c 6120 6872 6566 3d22 6874 7470  a>.<a href="http
-00002ab0: 733a 2f2f 7777 772e 6962 6d2e 636f 6d2f  s://www.ibm.com/
-00002ac0: 6f70 656e 736f 7572 6365 2f22 2074 6172  opensource/" tar
-00002ad0: 6765 743d 225f 626c 616e 6b22 3e3c 696d  get="_blank"><im
-00002ae0: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
-00002af0: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-00002b00: 7465 6e74 2e63 6f6d 2f61 6c62 756d 656e  tent.com/albumen
-00002b10: 7461 7469 6f6e 732d 7465 616d 2f61 6c62  tations-team/alb
-00002b20: 756d 656e 7461 7469 6f6e 732e 6169 2f6d  umentations.ai/m
-00002b30: 6169 6e2f 6874 6d6c 2f61 7373 6574 732f  ain/html/assets/
-00002b40: 696d 672f 696e 6475 7374 7279 2f69 626d  img/industry/ibm
-00002b50: 2e6a 7065 6722 2077 6964 7468 3d22 3130  .jpeg" width="10
-00002b60: 3022 2f3e 3c2f 613e 0a3c 6120 6872 6566  0"/></a>.<a href
-00002b70: 3d22 6874 7470 733a 2f2f 6875 6767 696e  ="https://huggin
-00002b80: 6766 6163 652e 636f 2f22 2074 6172 6765  gface.co/" targe
-00002b90: 743d 225f 626c 616e 6b22 3e3c 696d 6720  t="_blank"><img 
-00002ba0: 7372 633d 2268 7474 7073 3a2f 2f72 6177  src="https://raw
-00002bb0: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
-00002bc0: 6e74 2e63 6f6d 2f61 6c62 756d 656e 7461  nt.com/albumenta
-00002bd0: 7469 6f6e 732d 7465 616d 2f61 6c62 756d  tions-team/album
-00002be0: 656e 7461 7469 6f6e 732e 6169 2f6d 6169  entations.ai/mai
-00002bf0: 6e2f 6874 6d6c 2f61 7373 6574 732f 696d  n/html/assets/im
-00002c00: 672f 696e 6475 7374 7279 2f68 7567 6769  g/industry/huggi
-00002c10: 6e67 5f66 6163 652e 706e 6722 2077 6964  ng_face.png" wid
-00002c20: 7468 3d22 3130 3022 2f3e 3c2f 613e 0a3c  th="100"/></a>.<
-00002c30: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00002c40: 7777 772e 736f 6e79 2e63 6f6d 2f65 6e2f  www.sony.com/en/
-00002c50: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
-00002c60: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
-00002c70: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
-00002c80: 6572 636f 6e74 656e 742e 636f 6d2f 616c  ercontent.com/al
-00002c90: 6275 6d65 6e74 6174 696f 6e73 2d74 6561  bumentations-tea
-00002ca0: 6d2f 616c 6275 6d65 6e74 6174 696f 6e73  m/albumentations
-00002cb0: 2e61 692f 6d61 696e 2f68 746d 6c2f 6173  .ai/main/html/as
-00002cc0: 7365 7473 2f69 6d67 2f69 6e64 7573 7472  sets/img/industr
-00002cd0: 792f 736f 6e79 2e70 6e67 2220 7769 6474  y/sony.png" widt
-00002ce0: 683d 2231 3030 222f 3e3c 2f61 3e0a 3c61  h="100"/></a>.<a
-00002cf0: 2068 7265 663d 2268 7474 7073 3a2f 2f6f   href="https://o
-00002d00: 7065 6e73 6f75 7263 652e 616c 6962 6162  pensource.alibab
-00002d10: 612e 636f 6d2f 2220 7461 7267 6574 3d22  a.com/" target="
-00002d20: 5f62 6c61 6e6b 223e 3c69 6d67 2073 7263  _blank"><img src
-00002d30: 3d22 6874 7470 733a 2f2f 7261 772e 6769  ="https://raw.gi
-00002d40: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
-00002d50: 636f 6d2f 616c 6275 6d65 6e74 6174 696f  com/albumentatio
-00002d60: 6e73 2d74 6561 6d2f 616c 6275 6d65 6e74  ns-team/albument
-00002d70: 6174 696f 6e73 2e61 692f 6d61 696e 2f68  ations.ai/main/h
-00002d80: 746d 6c2f 6173 7365 7473 2f69 6d67 2f69  tml/assets/img/i
-00002d90: 6e64 7573 7472 792f 616c 6962 6162 612e  ndustry/alibaba.
-00002da0: 706e 6722 2077 6964 7468 3d22 3130 3022  png" width="100"
-00002db0: 2f3e 3c2f 613e 0a3c 6120 6872 6566 3d22  /></a>.<a href="
-00002dc0: 6874 7470 733a 2f2f 6f70 656e 736f 7572  https://opensour
-00002dd0: 6365 2e74 656e 6365 6e74 2e63 6f6d 2f22  ce.tencent.com/"
-00002de0: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
-00002df0: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
-00002e00: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
-00002e10: 7263 6f6e 7465 6e74 2e63 6f6d 2f61 6c62  rcontent.com/alb
-00002e20: 756d 656e 7461 7469 6f6e 732d 7465 616d  umentations-team
-00002e30: 2f61 6c62 756d 656e 7461 7469 6f6e 732e  /albumentations.
-00002e40: 6169 2f6d 6169 6e2f 6874 6d6c 2f61 7373  ai/main/html/ass
-00002e50: 6574 732f 696d 672f 696e 6475 7374 7279  ets/img/industry
-00002e60: 2f74 656e 6365 6e74 2e70 6e67 2220 7769  /tencent.png" wi
-00002e70: 6474 683d 2231 3030 222f 3e3c 2f61 3e0a  dth="100"/></a>.
-00002e80: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00002e90: 2f68 326f 2e61 692f 2220 7461 7267 6574  /h2o.ai/" target
-00002ea0: 3d22 5f62 6c61 6e6b 223e 3c69 6d67 2073  ="_blank"><img s
-00002eb0: 7263 3d22 6874 7470 733a 2f2f 7261 772e  rc="https://raw.
-00002ec0: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
-00002ed0: 742e 636f 6d2f 616c 6275 6d65 6e74 6174  t.com/albumentat
-00002ee0: 696f 6e73 2d74 6561 6d2f 616c 6275 6d65  ions-team/albume
-00002ef0: 6e74 6174 696f 6e73 2e61 692f 6d61 696e  ntations.ai/main
-00002f00: 2f68 746d 6c2f 6173 7365 7473 2f69 6d67  /html/assets/img
-00002f10: 2f69 6e64 7573 7472 792f 6832 6f5f 6169  /industry/h2o_ai
-00002f20: 2e70 6e67 2220 7769 6474 683d 2231 3030  .png" width="100
-00002f30: 222f 3e3c 2f61 3e0a 0a23 2323 2053 6565  "/></a>..### See
-00002f40: 2061 6c73 6f0a 0a2d 205b 4120 6c69 7374   also..- [A list
-00002f50: 206f 6620 7061 7065 7273 2074 6861 7420   of papers that 
-00002f60: 6369 7465 2041 6c62 756d 656e 7461 7469  cite Albumentati
-00002f70: 6f6e 735d 2868 7474 7073 3a2f 2f73 6368  ons](https://sch
-00002f80: 6f6c 6172 2e67 6f6f 676c 652e 636f 6d2f  olar.google.com/
-00002f90: 6369 7461 7469 6f6e 733f 7669 6577 5f6f  citations?view_o
-00002fa0: 703d 7669 6577 5f63 6974 6174 696f 6e26  p=view_citation&
-00002fb0: 6369 7461 7469 6f6e 5f66 6f72 5f76 6965  citation_for_vie
-00002fc0: 773d 766b 6a68 3958 3041 4141 414a 3a72  w=vkjh9X0AAAAJ:r
-00002fd0: 3042 706e 745a 714a 4734 4329 2e0a 2d20  0BpntZqJG4C)..- 
-00002fe0: 5b41 206c 6973 7420 6f66 2074 6561 6d73  [A list of teams
-00002ff0: 2074 6861 7420 7765 7265 2075 7369 6e67   that were using
-00003000: 2041 6c62 756d 656e 7461 7469 6f6e 7320   Albumentations 
-00003010: 616e 6420 746f 6f6b 2068 6967 6820 706c  and took high pl
-00003020: 6163 6573 2069 6e20 6d61 6368 696e 6520  aces in machine 
-00003030: 6c65 6172 6e69 6e67 2063 6f6d 7065 7469  learning competi
-00003040: 7469 6f6e 735d 2868 7474 7073 3a2f 2f61  tions](https://a
-00003050: 6c62 756d 656e 7461 7469 6f6e 732e 6169  lbumentations.ai
-00003060: 2f77 686f 735f 7573 696e 6723 636f 6d70  /whos_using#comp
-00003070: 6574 6974 696f 6e73 292e 0a2d 205b 4f70  etitions)..- [Op
-00003080: 656e 2073 6f75 7263 6520 7072 6f6a 6563  en source projec
-00003090: 7473 2074 6861 7420 7573 6520 416c 6275  ts that use Albu
-000030a0: 6d65 6e74 6174 696f 6e73 5d28 6874 7470  mentations](http
-000030b0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f61  s://github.com/a
-000030c0: 6c62 756d 656e 7461 7469 6f6e 732d 7465  lbumentations-te
-000030d0: 616d 2f61 6c62 756d 656e 7461 7469 6f6e  am/albumentation
-000030e0: 732f 6e65 7477 6f72 6b2f 6465 7065 6e64  s/network/depend
-000030f0: 656e 7473 3f64 6570 656e 6465 6e74 5f74  ents?dependent_t
-00003100: 7970 653d 5041 434b 4147 4529 2e0a 0a23  ype=PACKAGE)...#
-00003110: 2320 4c69 7374 206f 6620 6175 676d 656e  # List of augmen
-00003120: 7461 7469 6f6e 730a 0a23 2323 2050 6978  tations..### Pix
-00003130: 656c 2d6c 6576 656c 2074 7261 6e73 666f  el-level transfo
-00003140: 726d 730a 0a50 6978 656c 2d6c 6576 656c  rms..Pixel-level
-00003150: 2074 7261 6e73 666f 726d 7320 7769 6c6c   transforms will
-00003160: 2063 6861 6e67 6520 6a75 7374 2061 6e20   change just an 
-00003170: 696e 7075 7420 696d 6167 6520 616e 6420  input image and 
-00003180: 7769 6c6c 206c 6561 7665 2061 6e79 2061  will leave any a
-00003190: 6464 6974 696f 6e61 6c20 7461 7267 6574  dditional target
-000031a0: 7320 7375 6368 2061 7320 6d61 736b 732c  s such as masks,
-000031b0: 2062 6f75 6e64 696e 6720 626f 7865 732c   bounding boxes,
-000031c0: 2061 6e64 206b 6579 706f 696e 7473 2075   and keypoints u
-000031d0: 6e63 6861 6e67 6564 2e20 5468 6520 6c69  nchanged. The li
-000031e0: 7374 206f 6620 7069 7865 6c2d 6c65 7665  st of pixel-leve
-000031f0: 6c20 7472 616e 7366 6f72 6d73 3a0a 0a2d  l transforms:..-
-00003200: 205b 4164 7661 6e63 6564 426c 7572 5d28   [AdvancedBlur](
-00003210: 6874 7470 733a 2f2f 616c 6275 6d65 6e74  https://albument
-00003220: 6174 696f 6e73 2e61 692f 646f 6373 2f61  ations.ai/docs/a
-00003230: 7069 5f72 6566 6572 656e 6365 2f61 7567  pi_reference/aug
-00003240: 6d65 6e74 6174 696f 6e73 2f62 6c75 722f  mentations/blur/
-00003250: 7472 616e 7366 6f72 6d73 2f23 616c 6275  transforms/#albu
-00003260: 6d65 6e74 6174 696f 6e73 2e61 7567 6d65  mentations.augme
-00003270: 6e74 6174 696f 6e73 2e62 6c75 722e 7472  ntations.blur.tr
-00003280: 616e 7366 6f72 6d73 2e41 6476 616e 6365  ansforms.Advance
-00003290: 6442 6c75 7229 0a2d 205b 426c 7572 5d28  dBlur).- [Blur](
-000032a0: 6874 7470 733a 2f2f 616c 6275 6d65 6e74  https://albument
-000032b0: 6174 696f 6e73 2e61 692f 646f 6373 2f61  ations.ai/docs/a
-000032c0: 7069 5f72 6566 6572 656e 6365 2f61 7567  pi_reference/aug
-000032d0: 6d65 6e74 6174 696f 6e73 2f62 6c75 722f  mentations/blur/
-000032e0: 7472 616e 7366 6f72 6d73 2f23 616c 6275  transforms/#albu
-000032f0: 6d65 6e74 6174 696f 6e73 2e61 7567 6d65  mentations.augme
-00003300: 6e74 6174 696f 6e73 2e62 6c75 722e 7472  ntations.blur.tr
-00003310: 616e 7366 6f72 6d73 2e42 6c75 7229 0a2d  ansforms.Blur).-
-00003320: 205b 434c 4148 455d 2868 7474 7073 3a2f   [CLAHE](https:/
-00003330: 2f61 6c62 756d 656e 7461 7469 6f6e 732e  /albumentations.
-00003340: 6169 2f64 6f63 732f 6170 695f 7265 6665  ai/docs/api_refe
-00003350: 7265 6e63 652f 6175 676d 656e 7461 7469  rence/augmentati
-00003360: 6f6e 732f 7472 616e 7366 6f72 6d73 2f23  ons/transforms/#
-00003370: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
-00003380: 7567 6d65 6e74 6174 696f 6e73 2e74 7261  ugmentations.tra
-00003390: 6e73 666f 726d 732e 434c 4148 4529 0a2d  nsforms.CLAHE).-
-000033a0: 205b 4368 616e 6e65 6c44 726f 706f 7574   [ChannelDropout
-000033b0: 5d28 6874 7470 733a 2f2f 616c 6275 6d65  ](https://albume
-000033c0: 6e74 6174 696f 6e73 2e61 692f 646f 6373  ntations.ai/docs
-000033d0: 2f61 7069 5f72 6566 6572 656e 6365 2f61  /api_reference/a
-000033e0: 7567 6d65 6e74 6174 696f 6e73 2f64 726f  ugmentations/dro
-000033f0: 706f 7574 2f63 6861 6e6e 656c 5f64 726f  pout/channel_dro
-00003400: 706f 7574 2f23 616c 6275 6d65 6e74 6174  pout/#albumentat
-00003410: 696f 6e73 2e61 7567 6d65 6e74 6174 696f  ions.augmentatio
-00003420: 6e73 2e64 726f 706f 7574 2e63 6861 6e6e  ns.dropout.chann
-00003430: 656c 5f64 726f 706f 7574 2e43 6861 6e6e  el_dropout.Chann
-00003440: 656c 4472 6f70 6f75 7429 0a2d 205b 4368  elDropout).- [Ch
-00003450: 616e 6e65 6c53 6875 6666 6c65 5d28 6874  annelShuffle](ht
-00003460: 7470 733a 2f2f 616c 6275 6d65 6e74 6174  tps://albumentat
-00003470: 696f 6e73 2e61 692f 646f 6373 2f61 7069  ions.ai/docs/api
-00003480: 5f72 6566 6572 656e 6365 2f61 7567 6d65  _reference/augme
-00003490: 6e74 6174 696f 6e73 2f74 7261 6e73 666f  ntations/transfo
-000034a0: 726d 732f 2361 6c62 756d 656e 7461 7469  rms/#albumentati
-000034b0: 6f6e 732e 6175 676d 656e 7461 7469 6f6e  ons.augmentation
-000034c0: 732e 7472 616e 7366 6f72 6d73 2e43 6861  s.transforms.Cha
-000034d0: 6e6e 656c 5368 7566 666c 6529 0a2d 205b  nnelShuffle).- [
-000034e0: 4368 726f 6d61 7469 6341 6265 7272 6174  ChromaticAberrat
-000034f0: 696f 6e5d 2868 7474 7073 3a2f 2f61 6c62  ion](https://alb
-00003500: 756d 656e 7461 7469 6f6e 732e 6169 2f64  umentations.ai/d
-00003510: 6f63 732f 6170 695f 7265 6665 7265 6e63  ocs/api_referenc
-00003520: 652f 6175 676d 656e 7461 7469 6f6e 732f  e/augmentations/
-00003530: 7472 616e 7366 6f72 6d73 2f23 616c 6275  transforms/#albu
-00003540: 6d65 6e74 6174 696f 6e73 2e61 7567 6d65  mentations.augme
-00003550: 6e74 6174 696f 6e73 2e74 7261 6e73 666f  ntations.transfo
-00003560: 726d 732e 4368 726f 6d61 7469 6341 6265  rms.ChromaticAbe
-00003570: 7272 6174 696f 6e29 0a2d 205b 436f 6c6f  rration).- [Colo
-00003580: 724a 6974 7465 725d 2868 7474 7073 3a2f  rJitter](https:/
+00000000: 2320 416c 6275 6d65 6e74 6174 696f 6e73  # Albumentations
+00000010: 0a0a 5b21 5b50 7950 4920 7665 7273 696f  ..[![PyPI versio
+00000020: 6e5d 2868 7474 7073 3a2f 2f62 6164 6765  n](https://badge
+00000030: 2e66 7572 792e 696f 2f70 792f 616c 6275  .fury.io/py/albu
+00000040: 6d65 6e74 6174 696f 6e73 2e73 7667 295d  mentations.svg)]
+00000050: 2868 7474 7073 3a2f 2f62 6164 6765 2e66  (https://badge.f
+00000060: 7572 792e 696f 2f70 792f 616c 6275 6d65  ury.io/py/albume
+00000070: 6e74 6174 696f 6e73 290a 215b 4349 5d28  ntations).![CI](
+00000080: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000090: 6f6d 2f61 6c62 756d 656e 7461 7469 6f6e  om/albumentation
+000000a0: 732d 7465 616d 2f61 6c62 756d 656e 7461  s-team/albumenta
+000000b0: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
+000000c0: 4349 2f62 6164 6765 2e73 7667 290a 5b21  CI/badge.svg).[!
+000000d0: 5b4c 6963 656e 7365 3a20 4d49 545d 2868  [License: MIT](h
+000000e0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+000000f0: 6473 2e69 6f2f 6261 6467 652f 4c69 6365  ds.io/badge/Lice
+00000100: 6e73 652d 4d49 542d 6272 6967 6874 6772  nse-MIT-brightgr
+00000110: 6565 6e2e 7376 6729 5d28 6874 7470 733a  een.svg)](https:
+00000120: 2f2f 6f70 656e 736f 7572 6365 2e6f 7267  //opensource.org
+00000130: 2f6c 6963 656e 7365 732f 4d49 5429 0a5b  /licenses/MIT).[
+00000140: 215b 5275 6666 5d28 6874 7470 733a 2f2f  ![Ruff](https://
+00000150: 696d 672e 7368 6965 6c64 732e 696f 2f65  img.shields.io/e
+00000160: 6e64 706f 696e 743f 7572 6c3d 6874 7470  ndpoint?url=http
+00000170: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+00000180: 6572 636f 6e74 656e 742e 636f 6d2f 6173  ercontent.com/as
+00000190: 7472 616c 2d73 682f 7275 6666 2f6d 6169  tral-sh/ruff/mai
+000001a0: 6e2f 6173 7365 7473 2f62 6164 6765 2f76  n/assets/badge/v
+000001b0: 322e 6a73 6f6e 295d 2868 7474 7073 3a2f  2.json)](https:/
+000001c0: 2f67 6974 6875 622e 636f 6d2f 6173 7472  /github.com/astr
+000001d0: 616c 2d73 682f 7275 6666 290a 0a5b 446f  al-sh/ruff)..[Do
+000001e0: 6373 5d28 6874 7470 733a 2f2f 616c 6275  cs](https://albu
+000001f0: 6d65 6e74 6174 696f 6e73 2e61 692f 646f  mentations.ai/do
+00000200: 6373 2f29 207c 205b 4469 7363 6f72 645d  cs/) | [Discord]
+00000210: 2868 7474 7073 3a2f 2f64 6973 636f 7264  (https://discord
+00000220: 2e67 672f 414b 5072 7244 594e 4174 2920  .gg/AKPrrDYNAt) 
+00000230: 7c20 5b54 7769 7474 6572 5d28 6874 7470  | [Twitter](http
+00000240: 733a 2f2f 7477 6974 7465 722e 636f 6d2f  s://twitter.com/
+00000250: 616c 6275 6d65 6e74 6174 696f 6e73 2920  albumentations) 
+00000260: 7c20 5b4c 696e 6b65 6449 6e5d 2868 7474  | [LinkedIn](htt
+00000270: 7073 3a2f 2f77 7777 2e6c 696e 6b65 6469  ps://www.linkedi
+00000280: 6e2e 636f 6d2f 636f 6d70 616e 792f 3130  n.com/company/10
+00000290: 3035 3034 3437 352f 290a 0a41 6c62 756d  0504475/)..Album
+000002a0: 656e 7461 7469 6f6e 7320 6973 2061 2050  entations is a P
+000002b0: 7974 686f 6e20 6c69 6272 6172 7920 666f  ython library fo
+000002c0: 7220 696d 6167 6520 6175 676d 656e 7461  r image augmenta
+000002d0: 7469 6f6e 2e20 496d 6167 6520 6175 676d  tion. Image augm
+000002e0: 656e 7461 7469 6f6e 2069 7320 7573 6564  entation is used
+000002f0: 2069 6e20 6465 6570 206c 6561 726e 696e   in deep learnin
+00000300: 6720 616e 6420 636f 6d70 7574 6572 2076  g and computer v
+00000310: 6973 696f 6e20 7461 736b 7320 746f 2069  ision tasks to i
+00000320: 6e63 7265 6173 6520 7468 6520 7175 616c  ncrease the qual
+00000330: 6974 7920 6f66 2074 7261 696e 6564 206d  ity of trained m
+00000340: 6f64 656c 732e 2054 6865 2070 7572 706f  odels. The purpo
+00000350: 7365 206f 6620 696d 6167 6520 6175 676d  se of image augm
+00000360: 656e 7461 7469 6f6e 2069 7320 746f 2063  entation is to c
+00000370: 7265 6174 6520 6e65 7720 7472 6169 6e69  reate new traini
+00000380: 6e67 2073 616d 706c 6573 2066 726f 6d20  ng samples from 
+00000390: 7468 6520 6578 6973 7469 6e67 2064 6174  the existing dat
+000003a0: 612e 0a0a 4865 7265 2069 7320 616e 2065  a...Here is an e
+000003b0: 7861 6d70 6c65 206f 6620 686f 7720 796f  xample of how yo
+000003c0: 7520 6361 6e20 6170 706c 7920 736f 6d65  u can apply some
+000003d0: 205b 7069 7865 6c2d 6c65 7665 6c5d 2823   [pixel-level](#
+000003e0: 7069 7865 6c2d 6c65 7665 6c2d 7472 616e  pixel-level-tran
+000003f0: 7366 6f72 6d73 2920 6175 676d 656e 7461  sforms) augmenta
+00000400: 7469 6f6e 7320 6672 6f6d 2041 6c62 756d  tions from Album
+00000410: 656e 7461 7469 6f6e 7320 746f 2063 7265  entations to cre
+00000420: 6174 6520 6e65 7720 696d 6167 6573 2066  ate new images f
+00000430: 726f 6d20 7468 6520 6f72 6967 696e 616c  rom the original
+00000440: 206f 6e65 3a0a 215b 7061 7272 6f74 5d28   one:.![parrot](
+00000450: 6874 7470 733a 2f2f 6861 6272 6173 746f  https://habrasto
+00000460: 7261 6765 2e6f 7267 2f77 6562 742f 6264  rage.org/webt/bd
+00000470: 2f6e 652f 7276 2f62 646e 6572 7635 6374  /ne/rv/bdnerv5ct
+00000480: 6b75 646d 7361 7a6e 6877 3463 7273 6466  kudmsaznhw4crsdf
+00000490: 6977 2e6a 7065 6729 0a0a 2323 2057 6879  iw.jpeg)..## Why
+000004a0: 2041 6c62 756d 656e 7461 7469 6f6e 730a   Albumentations.
+000004b0: 0a2d 2041 6c62 756d 656e 7461 7469 6f6e  .- Albumentation
+000004c0: 7320 2a2a 5b73 7570 706f 7274 7320 616c  s **[supports al
+000004d0: 6c20 636f 6d6d 6f6e 2063 6f6d 7075 7465  l common compute
+000004e0: 7220 7669 7369 6f6e 2074 6173 6b73 5d28  r vision tasks](
+000004f0: 2369 2d77 616e 742d 746f 2d75 7365 2d61  #i-want-to-use-a
+00000500: 6c62 756d 656e 7461 7469 6f6e 732d 666f  lbumentations-fo
+00000510: 722d 7468 652d 7370 6563 6966 6963 2d74  r-the-specific-t
+00000520: 6173 6b2d 7375 6368 2d61 732d 636c 6173  ask-such-as-clas
+00000530: 7369 6669 6361 7469 6f6e 2d6f 722d 7365  sification-or-se
+00000540: 676d 656e 7461 7469 6f6e 292a 2a20 7375  gmentation)** su
+00000550: 6368 2061 7320 636c 6173 7369 6669 6361  ch as classifica
+00000560: 7469 6f6e 2c20 7365 6d61 6e74 6963 2073  tion, semantic s
+00000570: 6567 6d65 6e74 6174 696f 6e2c 2069 6e73  egmentation, ins
+00000580: 7461 6e63 6520 7365 676d 656e 7461 7469  tance segmentati
+00000590: 6f6e 2c20 6f62 6a65 6374 2064 6574 6563  on, object detec
+000005a0: 7469 6f6e 2c20 616e 6420 706f 7365 2065  tion, and pose e
+000005b0: 7374 696d 6174 696f 6e2e 0a2d 2054 6865  stimation..- The
+000005c0: 206c 6962 7261 7279 2070 726f 7669 6465   library provide
+000005d0: 7320 2a2a 5b61 2073 696d 706c 6520 756e  s **[a simple un
+000005e0: 6966 6965 6420 4150 495d 2823 612d 7369  ified API](#a-si
+000005f0: 6d70 6c65 2d65 7861 6d70 6c65 292a 2a20  mple-example)** 
+00000600: 746f 2077 6f72 6b20 7769 7468 2061 6c6c  to work with all
+00000610: 2064 6174 6120 7479 7065 733a 2069 6d61   data types: ima
+00000620: 6765 7320 2852 4247 2d69 6d61 6765 732c  ges (RBG-images,
+00000630: 2067 7261 7973 6361 6c65 2069 6d61 6765   grayscale image
+00000640: 732c 206d 756c 7469 7370 6563 7472 616c  s, multispectral
+00000650: 2069 6d61 6765 7329 2c20 7365 676d 656e   images), segmen
+00000660: 7461 7469 6f6e 206d 6173 6b73 2c20 626f  tation masks, bo
+00000670: 756e 6469 6e67 2062 6f78 6573 2c20 616e  unding boxes, an
+00000680: 6420 6b65 7970 6f69 6e74 732e 0a2d 2054  d keypoints..- T
+00000690: 6865 206c 6962 7261 7279 2063 6f6e 7461  he library conta
+000006a0: 696e 7320 2a2a 5b6d 6f72 6520 7468 616e  ins **[more than
+000006b0: 2037 3020 6469 6666 6572 656e 7420 6175   70 different au
+000006c0: 676d 656e 7461 7469 6f6e 735d 2823 6c69  gmentations](#li
+000006d0: 7374 2d6f 662d 6175 676d 656e 7461 7469  st-of-augmentati
+000006e0: 6f6e 7329 2a2a 2074 6f20 6765 6e65 7261  ons)** to genera
+000006f0: 7465 206e 6577 2074 7261 696e 696e 6720  te new training 
+00000700: 7361 6d70 6c65 7320 6672 6f6d 2074 6865  samples from the
+00000710: 2065 7869 7374 696e 6720 6461 7461 2e0a   existing data..
+00000720: 2d20 416c 6275 6d65 6e74 6174 696f 6e73  - Albumentations
+00000730: 2069 7320 5b2a 2a66 6173 742a 2a5d 2823   is [**fast**](#
+00000740: 6265 6e63 686d 6172 6b69 6e67 2d72 6573  benchmarking-res
+00000750: 756c 7473 292e 2057 6520 6265 6e63 686d  ults). We benchm
+00000760: 6172 6b20 6561 6368 206e 6577 2072 656c  ark each new rel
+00000770: 6561 7365 2074 6f20 656e 7375 7265 2074  ease to ensure t
+00000780: 6861 7420 6175 676d 656e 7461 7469 6f6e  hat augmentation
+00000790: 7320 7072 6f76 6964 6520 6d61 7869 6d75  s provide maximu
+000007a0: 6d20 7370 6565 642e 0a2d 2049 7420 2a2a  m speed..- It **
+000007b0: 5b77 6f72 6b73 2077 6974 6820 706f 7075  [works with popu
+000007c0: 6c61 7220 6465 6570 206c 6561 726e 696e  lar deep learnin
+000007d0: 6720 6672 616d 6577 6f72 6b73 5d28 2369  g frameworks](#i
+000007e0: 2d77 616e 742d 746f 2d6b 6e6f 772d 686f  -want-to-know-ho
+000007f0: 772d 746f 2d75 7365 2d61 6c62 756d 656e  w-to-use-albumen
+00000800: 7461 7469 6f6e 732d 7769 7468 2d64 6565  tations-with-dee
+00000810: 702d 6c65 6172 6e69 6e67 2d66 7261 6d65  p-learning-frame
+00000820: 776f 726b 7329 2a2a 2073 7563 6820 6173  works)** such as
+00000830: 2050 7954 6f72 6368 2061 6e64 2054 656e   PyTorch and Ten
+00000840: 736f 7246 6c6f 772e 2042 7920 7468 6520  sorFlow. By the 
+00000850: 7761 792c 2041 6c62 756d 656e 7461 7469  way, Albumentati
+00000860: 6f6e 7320 6973 2061 2070 6172 7420 6f66  ons is a part of
+00000870: 2074 6865 205b 5079 546f 7263 6820 6563   the [PyTorch ec
+00000880: 6f73 7973 7465 6d5d 2868 7474 7073 3a2f  osystem](https:/
+00000890: 2f70 7974 6f72 6368 2e6f 7267 2f65 636f  /pytorch.org/eco
+000008a0: 7379 7374 656d 2f29 2e0a 2d20 5b2a 2a57  system/)..- [**W
+000008b0: 7269 7474 656e 2062 7920 6578 7065 7274  ritten by expert
+000008c0: 732a 2a5d 2823 6175 7468 6f72 7329 2e20  s**](#authors). 
+000008d0: 5468 6520 6175 7468 6f72 7320 6861 7665  The authors have
+000008e0: 2065 7870 6572 6965 6e63 6520 626f 7468   experience both
+000008f0: 2077 6f72 6b69 6e67 206f 6e20 7072 6f64   working on prod
+00000900: 7563 7469 6f6e 2063 6f6d 7075 7465 7220  uction computer 
+00000910: 7669 7369 6f6e 2073 7973 7465 6d73 2061  vision systems a
+00000920: 6e64 2070 6172 7469 6369 7061 7469 6e67  nd participating
+00000930: 2069 6e20 636f 6d70 6574 6974 6976 6520   in competitive 
+00000940: 6d61 6368 696e 6520 6c65 6172 6e69 6e67  machine learning
+00000950: 2e20 4d61 6e79 2063 6f72 6520 7465 616d  . Many core team
+00000960: 206d 656d 6265 7273 2061 7265 204b 6167   members are Kag
+00000970: 676c 6520 4d61 7374 6572 7320 616e 6420  gle Masters and 
+00000980: 4772 616e 646d 6173 7465 7273 2e0a 2d20  Grandmasters..- 
+00000990: 5468 6520 6c69 6272 6172 7920 6973 205b  The library is [
+000009a0: 2a2a 7769 6465 6c79 2075 7365 642a 2a5d  **widely used**]
+000009b0: 2823 7768 6f2d 6973 2d75 7369 6e67 2d61  (#who-is-using-a
+000009c0: 6c62 756d 656e 7461 7469 6f6e 7329 2069  lbumentations) i
+000009d0: 6e20 696e 6475 7374 7279 2c20 6465 6570  n industry, deep
+000009e0: 206c 6561 726e 696e 6720 7265 7365 6172   learning resear
+000009f0: 6368 2c20 6d61 6368 696e 6520 6c65 6172  ch, machine lear
+00000a00: 6e69 6e67 2063 6f6d 7065 7469 7469 6f6e  ning competition
+00000a10: 732c 2061 6e64 206f 7065 6e20 736f 7572  s, and open sour
+00000a20: 6365 2070 726f 6a65 6374 732e 0a0a 2323  ce projects...##
+00000a30: 2053 706f 6e73 6f72 730a 0a3c 6120 6872   Sponsors..<a hr
+00000a40: 6566 3d22 6874 7470 733a 2f2f 726f 626f  ef="https://robo
+00000a50: 666c 6f77 2e63 6f6d 2f22 2074 6172 6765  flow.com/" targe
+00000a60: 743d 225f 626c 616e 6b22 3e3c 696d 6720  t="_blank"><img 
+00000a70: 7372 633d 2268 7474 7073 3a2f 2f61 7661  src="https://ava
+00000a80: 7461 7273 2e67 6974 6875 6275 7365 7263  tars.githubuserc
+00000a90: 6f6e 7465 6e74 2e63 6f6d 2f75 2f35 3331  ontent.com/u/531
+00000aa0: 3034 3131 383f 733d 3230 3026 763d 3422  04118?s=200&v=4"
+00000ab0: 2077 6964 7468 3d22 3130 3022 2f3e 3c2f   width="100"/></
+00000ac0: 613e 0a0a 2323 2054 6162 6c65 206f 6620  a>..## Table of 
+00000ad0: 636f 6e74 656e 7473 0a0a 2d20 5b41 6c62  contents..- [Alb
+00000ae0: 756d 656e 7461 7469 6f6e 735d 2823 616c  umentations](#al
+00000af0: 6275 6d65 6e74 6174 696f 6e73 290a 2020  bumentations).  
+00000b00: 2d20 5b57 6879 2041 6c62 756d 656e 7461  - [Why Albumenta
+00000b10: 7469 6f6e 735d 2823 7768 792d 616c 6275  tions](#why-albu
+00000b20: 6d65 6e74 6174 696f 6e73 290a 2020 2d20  mentations).  - 
+00000b30: 5b53 706f 6e73 6f72 735d 2823 7370 6f6e  [Sponsors](#spon
+00000b40: 736f 7273 290a 2020 2d20 5b54 6162 6c65  sors).  - [Table
+00000b50: 206f 6620 636f 6e74 656e 7473 5d28 2374   of contents](#t
+00000b60: 6162 6c65 2d6f 662d 636f 6e74 656e 7473  able-of-contents
+00000b70: 290a 2020 2d20 5b41 7574 686f 7273 5d28  ).  - [Authors](
+00000b80: 2361 7574 686f 7273 290a 2020 2d20 5b49  #authors).  - [I
+00000b90: 6e73 7461 6c6c 6174 696f 6e5d 2823 696e  nstallation](#in
+00000ba0: 7374 616c 6c61 7469 6f6e 290a 2020 2d20  stallation).  - 
+00000bb0: 5b44 6f63 756d 656e 7461 7469 6f6e 5d28  [Documentation](
+00000bc0: 2364 6f63 756d 656e 7461 7469 6f6e 290a  #documentation).
+00000bd0: 2020 2d20 5b41 2073 696d 706c 6520 6578    - [A simple ex
+00000be0: 616d 706c 655d 2823 612d 7369 6d70 6c65  ample](#a-simple
+00000bf0: 2d65 7861 6d70 6c65 290a 2020 2d20 5b47  -example).  - [G
+00000c00: 6574 7469 6e67 2073 7461 7274 6564 5d28  etting started](
+00000c10: 2367 6574 7469 6e67 2d73 7461 7274 6564  #getting-started
+00000c20: 290a 2020 2020 2d20 5b49 2061 6d20 6e65  ).    - [I am ne
+00000c30: 7720 746f 2069 6d61 6765 2061 7567 6d65  w to image augme
+00000c40: 6e74 6174 696f 6e5d 2823 692d 616d 2d6e  ntation](#i-am-n
+00000c50: 6577 2d74 6f2d 696d 6167 652d 6175 676d  ew-to-image-augm
+00000c60: 656e 7461 7469 6f6e 290a 2020 2020 2d20  entation).    - 
+00000c70: 5b49 2077 616e 7420 746f 2075 7365 2041  [I want to use A
+00000c80: 6c62 756d 656e 7461 7469 6f6e 7320 666f  lbumentations fo
+00000c90: 7220 7468 6520 7370 6563 6966 6963 2074  r the specific t
+00000ca0: 6173 6b20 7375 6368 2061 7320 636c 6173  ask such as clas
+00000cb0: 7369 6669 6361 7469 6f6e 206f 7220 7365  sification or se
+00000cc0: 676d 656e 7461 7469 6f6e 5d28 2369 2d77  gmentation](#i-w
+00000cd0: 616e 742d 746f 2d75 7365 2d61 6c62 756d  ant-to-use-album
+00000ce0: 656e 7461 7469 6f6e 732d 666f 722d 7468  entations-for-th
+00000cf0: 652d 7370 6563 6966 6963 2d74 6173 6b2d  e-specific-task-
+00000d00: 7375 6368 2d61 732d 636c 6173 7369 6669  such-as-classifi
+00000d10: 6361 7469 6f6e 2d6f 722d 7365 676d 656e  cation-or-segmen
+00000d20: 7461 7469 6f6e 290a 2020 2020 2d20 5b49  tation).    - [I
+00000d30: 2077 616e 7420 746f 206b 6e6f 7720 686f   want to know ho
+00000d40: 7720 746f 2075 7365 2041 6c62 756d 656e  w to use Albumen
+00000d50: 7461 7469 6f6e 7320 7769 7468 2064 6565  tations with dee
+00000d60: 7020 6c65 6172 6e69 6e67 2066 7261 6d65  p learning frame
+00000d70: 776f 726b 735d 2823 692d 7761 6e74 2d74  works](#i-want-t
+00000d80: 6f2d 6b6e 6f77 2d68 6f77 2d74 6f2d 7573  o-know-how-to-us
+00000d90: 652d 616c 6275 6d65 6e74 6174 696f 6e73  e-albumentations
+00000da0: 2d77 6974 682d 6465 6570 2d6c 6561 726e  -with-deep-learn
+00000db0: 696e 672d 6672 616d 6577 6f72 6b73 290a  ing-frameworks).
+00000dc0: 2020 2020 2d20 5b49 2077 616e 7420 746f      - [I want to
+00000dd0: 2065 7870 6c6f 7265 2061 7567 6d65 6e74   explore augment
+00000de0: 6174 696f 6e73 2061 6e64 2073 6565 2041  ations and see A
+00000df0: 6c62 756d 656e 7461 7469 6f6e 7320 696e  lbumentations in
+00000e00: 2061 6374 696f 6e5d 2823 692d 7761 6e74   action](#i-want
+00000e10: 2d74 6f2d 6578 706c 6f72 652d 6175 676d  -to-explore-augm
+00000e20: 656e 7461 7469 6f6e 732d 616e 642d 7365  entations-and-se
+00000e30: 652d 616c 6275 6d65 6e74 6174 696f 6e73  e-albumentations
+00000e40: 2d69 6e2d 6163 7469 6f6e 290a 2020 2d20  -in-action).  - 
+00000e50: 5b57 686f 2069 7320 7573 696e 6720 416c  [Who is using Al
+00000e60: 6275 6d65 6e74 6174 696f 6e73 5d28 2377  bumentations](#w
+00000e70: 686f 2d69 732d 7573 696e 672d 616c 6275  ho-is-using-albu
+00000e80: 6d65 6e74 6174 696f 6e73 290a 2020 2020  mentations).    
+00000e90: 2d20 5b53 6565 2061 6c73 6f5d 2823 7365  - [See also](#se
+00000ea0: 652d 616c 736f 290a 2020 2d20 5b4c 6973  e-also).  - [Lis
+00000eb0: 7420 6f66 2061 7567 6d65 6e74 6174 696f  t of augmentatio
+00000ec0: 6e73 5d28 236c 6973 742d 6f66 2d61 7567  ns](#list-of-aug
+00000ed0: 6d65 6e74 6174 696f 6e73 290a 2020 2020  mentations).    
+00000ee0: 2d20 5b50 6978 656c 2d6c 6576 656c 2074  - [Pixel-level t
+00000ef0: 7261 6e73 666f 726d 735d 2823 7069 7865  ransforms](#pixe
+00000f00: 6c2d 6c65 7665 6c2d 7472 616e 7366 6f72  l-level-transfor
+00000f10: 6d73 290a 2020 2020 2d20 5b53 7061 7469  ms).    - [Spati
+00000f20: 616c 2d6c 6576 656c 2074 7261 6e73 666f  al-level transfo
+00000f30: 726d 735d 2823 7370 6174 6961 6c2d 6c65  rms](#spatial-le
+00000f40: 7665 6c2d 7472 616e 7366 6f72 6d73 290a  vel-transforms).
+00000f50: 2020 2020 2d20 5b4d 6978 696e 672d 6c65      - [Mixing-le
+00000f60: 7665 6c20 7472 616e 7366 6f72 6d73 5d28  vel transforms](
+00000f70: 236d 6978 696e 672d 6c65 7665 6c2d 7472  #mixing-level-tr
+00000f80: 616e 7366 6f72 6d73 290a 2020 2d20 5b41  ansforms).  - [A
+00000f90: 2066 6577 206d 6f72 6520 6578 616d 706c   few more exampl
+00000fa0: 6573 206f 6620 2a2a 6175 676d 656e 7461  es of **augmenta
+00000fb0: 7469 6f6e 732a 2a5d 2823 612d 6665 772d  tions**](#a-few-
+00000fc0: 6d6f 7265 2d65 7861 6d70 6c65 732d 6f66  more-examples-of
+00000fd0: 2d61 7567 6d65 6e74 6174 696f 6e73 290a  -augmentations).
+00000fe0: 2020 2020 2d20 5b53 656d 616e 7469 6320      - [Semantic 
+00000ff0: 7365 676d 656e 7461 7469 6f6e 206f 6e20  segmentation on 
+00001000: 7468 6520 496e 7269 6120 6461 7461 7365  the Inria datase
+00001010: 745d 2823 7365 6d61 6e74 6963 2d73 6567  t](#semantic-seg
+00001020: 6d65 6e74 6174 696f 6e2d 6f6e 2d74 6865  mentation-on-the
+00001030: 2d69 6e72 6961 2d64 6174 6173 6574 290a  -inria-dataset).
+00001040: 2020 2020 2d20 5b4d 6564 6963 616c 2069      - [Medical i
+00001050: 6d61 6769 6e67 5d28 236d 6564 6963 616c  maging](#medical
+00001060: 2d69 6d61 6769 6e67 290a 2020 2020 2d20  -imaging).    - 
+00001070: 5b4f 626a 6563 7420 6465 7465 6374 696f  [Object detectio
+00001080: 6e20 616e 6420 7365 6d61 6e74 6963 2073  n and semantic s
+00001090: 6567 6d65 6e74 6174 696f 6e20 6f6e 2074  egmentation on t
+000010a0: 6865 204d 6170 696c 6c61 7279 2056 6973  he Mapillary Vis
+000010b0: 7461 7320 6461 7461 7365 745d 2823 6f62  tas dataset](#ob
+000010c0: 6a65 6374 2d64 6574 6563 7469 6f6e 2d61  ject-detection-a
+000010d0: 6e64 2d73 656d 616e 7469 632d 7365 676d  nd-semantic-segm
+000010e0: 656e 7461 7469 6f6e 2d6f 6e2d 7468 652d  entation-on-the-
+000010f0: 6d61 7069 6c6c 6172 792d 7669 7374 6173  mapillary-vistas
+00001100: 2d64 6174 6173 6574 290a 2020 2020 2d20  -dataset).    - 
+00001110: 5b4b 6579 706f 696e 7473 2061 7567 6d65  [Keypoints augme
+00001120: 6e74 6174 696f 6e5d 2823 6b65 7970 6f69  ntation](#keypoi
+00001130: 6e74 732d 6175 676d 656e 7461 7469 6f6e  nts-augmentation
+00001140: 290a 2020 2d20 5b42 656e 6368 6d61 726b  ).  - [Benchmark
+00001150: 696e 6720 7265 7375 6c74 735d 2823 6265  ing results](#be
+00001160: 6e63 686d 6172 6b69 6e67 2d72 6573 756c  nchmarking-resul
+00001170: 7473 290a 2020 2d20 5b43 6f6e 7472 6962  ts).  - [Contrib
+00001180: 7574 696e 675d 2823 636f 6e74 7269 6275  uting](#contribu
+00001190: 7469 6e67 290a 2020 2d20 5b43 6f6d 6d75  ting).  - [Commu
+000011a0: 6e69 7479 2061 6e64 2053 7570 706f 7274  nity and Support
+000011b0: 5d28 2363 6f6d 6d75 6e69 7479 2d61 6e64  ](#community-and
+000011c0: 2d73 7570 706f 7274 290a 2020 2d20 5b43  -support).  - [C
+000011d0: 6f6d 6d65 6e74 735d 2823 636f 6d6d 656e  omments](#commen
+000011e0: 7473 290a 2020 2d20 5b43 6974 696e 675d  ts).  - [Citing]
+000011f0: 2823 6369 7469 6e67 290a 0a23 2320 4175  (#citing)..## Au
+00001200: 7468 6f72 730a 0a5b 2a2a 566c 6164 696d  thors..[**Vladim
+00001210: 6972 2049 2e20 4967 6c6f 7669 6b6f 762a  ir I. Iglovikov*
+00001220: 2a5d 2868 7474 7073 3a2f 2f77 7777 2e6c  *](https://www.l
+00001230: 696e 6b65 6469 6e2e 636f 6d2f 696e 2f69  inkedin.com/in/i
+00001240: 676c 6f76 696b 6f76 2f29 207c 205b 4b61  glovikov/) | [Ka
+00001250: 6767 6c65 2047 7261 6e64 6d61 7374 6572  ggle Grandmaster
+00001260: 5d28 6874 7470 733a 2f2f 7777 772e 6b61  ](https://www.ka
+00001270: 6767 6c65 2e63 6f6d 2f69 676c 6f76 696b  ggle.com/iglovik
+00001280: 6f76 290a 0a5b 2a2a 4d69 6b68 6169 6c20  ov)..[**Mikhail 
+00001290: 4472 757a 6869 6e69 6e2a 2a5d 2868 7474  Druzhinin**](htt
+000012a0: 7073 3a2f 2f77 7777 2e6c 696e 6b65 6469  ps://www.linkedi
+000012b0: 6e2e 636f 6d2f 696e 2f6d 696b 6861 696c  n.com/in/mikhail
+000012c0: 2d64 7275 7a68 696e 696e 2d35 3438 3232  -druzhinin-54822
+000012d0: 3931 3030 2f29 207c 205b 4b61 6767 6c65  9100/) | [Kaggle
+000012e0: 2045 7870 6572 745d 2868 7474 7073 3a2f   Expert](https:/
+000012f0: 2f77 7777 2e6b 6167 676c 652e 636f 6d2f  /www.kaggle.com/
+00001300: 6469 7065 746d 290a 0a5b 2a2a 416c 6578  dipetm)..[**Alex
+00001310: 2050 6172 696e 6f76 2a2a 5d28 6874 7470   Parinov**](http
+00001320: 733a 2f2f 7777 772e 6c69 6e6b 6564 696e  s://www.linkedin
+00001330: 2e63 6f6d 2f69 6e2f 616c 6578 2d70 6172  .com/in/alex-par
+00001340: 696e 6f76 2f29 207c 205b 4b61 6767 6c65  inov/) | [Kaggle
+00001350: 204d 6173 7465 725d 2868 7474 7073 3a2f   Master](https:/
+00001360: 2f77 7777 2e6b 6167 676c 652e 636f 6d2f  /www.kaggle.com/
+00001370: 6372 6561 667a 290a 0a5b 2a2a 416c 6578  creafz)..[**Alex
+00001380: 616e 6465 7220 4275 736c 6165 762a 2a20  ander Buslaev** 
+00001390: e280 9420 436f 6d70 7574 6572 2056 6973  ... Computer Vis
+000013a0: 696f 6e20 456e 6769 6e65 6572 2061 7420  ion Engineer at 
+000013b0: 4d61 7062 6f78 5d28 6874 7470 733a 2f2f  Mapbox](https://
+000013c0: 7777 772e 6c69 6e6b 6564 696e 2e63 6f6d  www.linkedin.com
+000013d0: 2f69 6e2f 616c 2d62 7573 6c61 6576 2f29  /in/al-buslaev/)
+000013e0: 207c 205b 4b61 6767 6c65 204d 6173 7465   | [Kaggle Maste
+000013f0: 725d 2868 7474 7073 3a2f 2f77 7777 2e6b  r](https://www.k
+00001400: 6167 676c 652e 636f 6d2f 616c 6275 736c  aggle.com/albusl
+00001410: 6165 7629 0a0a 5b2a 2a45 7665 6765 6e65  aev)..[**Evegene
+00001420: 204b 6876 6564 6368 656e 7961 2a2a 20e2   Khvedchenya** .
+00001430: 8094 2043 6f6d 7075 7465 7220 5669 7369  .. Computer Visi
+00001440: 6f6e 2052 6573 6561 7263 6820 456e 6769  on Research Engi
+00001450: 6e65 6572 2061 7420 5069 c3b1 6174 6120  neer at Pi..ata 
+00001460: 4661 726d 735d 2868 7474 7073 3a2f 2f77  Farms](https://w
+00001470: 7777 2e6c 696e 6b65 6469 6e2e 636f 6d2f  ww.linkedin.com/
+00001480: 696e 2f63 7674 616c 6b73 2f29 207c 205b  in/cvtalks/) | [
+00001490: 4b61 6767 6c65 2047 7261 6e64 6d61 7374  Kaggle Grandmast
+000014a0: 6572 5d28 6874 7470 733a 2f2f 7777 772e  er](https://www.
+000014b0: 6b61 6767 6c65 2e63 6f6d 2f62 6c6f 6f64  kaggle.com/blood
+000014c0: 6178 6529 0a0a 2323 2049 6e73 7461 6c6c  axe)..## Install
+000014d0: 6174 696f 6e0a 0a41 6c62 756d 656e 7461  ation..Albumenta
+000014e0: 7469 6f6e 7320 7265 7175 6972 6573 2050  tions requires P
+000014f0: 7974 686f 6e20 332e 3820 6f72 2068 6967  ython 3.8 or hig
+00001500: 6865 722e 2054 6f20 696e 7374 616c 6c20  her. To install 
+00001510: 7468 6520 6c61 7465 7374 2076 6572 7369  the latest versi
+00001520: 6f6e 2066 726f 6d20 5079 5049 3a0a 0a60  on from PyPI:..`
+00001530: 6060 6261 7368 0a70 6970 2069 6e73 7461  ``bash.pip insta
+00001540: 6c6c 202d 5520 616c 6275 6d65 6e74 6174  ll -U albumentat
+00001550: 696f 6e73 0a60 6060 0a0a 4f74 6865 7220  ions.```..Other 
+00001560: 696e 7374 616c 6c61 7469 6f6e 206f 7074  installation opt
+00001570: 696f 6e73 2061 7265 2064 6573 6372 6962  ions are describ
+00001580: 6564 2069 6e20 7468 6520 5b64 6f63 756d  ed in the [docum
+00001590: 656e 7461 7469 6f6e 5d28 6874 7470 733a  entation](https:
+000015a0: 2f2f 616c 6275 6d65 6e74 6174 696f 6e73  //albumentations
+000015b0: 2e61 692f 646f 6373 2f67 6574 7469 6e67  .ai/docs/getting
+000015c0: 5f73 7461 7274 6564 2f69 6e73 7461 6c6c  _started/install
+000015d0: 6174 696f 6e2f 292e 0a0a 2323 2044 6f63  ation/)...## Doc
+000015e0: 756d 656e 7461 7469 6f6e 0a0a 5468 6520  umentation..The 
+000015f0: 6675 6c6c 2064 6f63 756d 656e 7461 7469  full documentati
+00001600: 6f6e 2069 7320 6176 6169 6c61 626c 6520  on is available 
+00001610: 6174 202a 2a5b 6874 7470 733a 2f2f 616c  at **[https://al
+00001620: 6275 6d65 6e74 6174 696f 6e73 2e61 692f  bumentations.ai/
+00001630: 646f 6373 2f5d 2868 7474 7073 3a2f 2f61  docs/](https://a
+00001640: 6c62 756d 656e 7461 7469 6f6e 732e 6169  lbumentations.ai
+00001650: 2f64 6f63 732f 292a 2a2e 0a0a 2323 2041  /docs/)**...## A
+00001660: 2073 696d 706c 6520 6578 616d 706c 650a   simple example.
+00001670: 0a60 6060 7079 7468 6f6e 0a69 6d70 6f72  .```python.impor
+00001680: 7420 616c 6275 6d65 6e74 6174 696f 6e73  t albumentations
+00001690: 2061 7320 410a 696d 706f 7274 2063 7632   as A.import cv2
+000016a0: 0a0a 2320 4465 636c 6172 6520 616e 2061  ..# Declare an a
+000016b0: 7567 6d65 6e74 6174 696f 6e20 7069 7065  ugmentation pipe
+000016c0: 6c69 6e65 0a74 7261 6e73 666f 726d 203d  line.transform =
+000016d0: 2041 2e43 6f6d 706f 7365 285b 0a20 2020   A.Compose([.   
+000016e0: 2041 2e52 616e 646f 6d43 726f 7028 7769   A.RandomCrop(wi
+000016f0: 6474 683d 3235 362c 2068 6569 6768 743d  dth=256, height=
+00001700: 3235 3629 2c0a 2020 2020 412e 486f 7269  256),.    A.Hori
+00001710: 7a6f 6e74 616c 466c 6970 2870 3d30 2e35  zontalFlip(p=0.5
+00001720: 292c 0a20 2020 2041 2e52 616e 646f 6d42  ),.    A.RandomB
+00001730: 7269 6768 746e 6573 7343 6f6e 7472 6173  rightnessContras
+00001740: 7428 703d 302e 3229 2c0a 5d29 0a0a 2320  t(p=0.2),.])..# 
+00001750: 5265 6164 2061 6e20 696d 6167 6520 7769  Read an image wi
+00001760: 7468 204f 7065 6e43 5620 616e 6420 636f  th OpenCV and co
+00001770: 6e76 6572 7420 6974 2074 6f20 7468 6520  nvert it to the 
+00001780: 5247 4220 636f 6c6f 7273 7061 6365 0a69  RGB colorspace.i
+00001790: 6d61 6765 203d 2063 7632 2e69 6d72 6561  mage = cv2.imrea
+000017a0: 6428 2269 6d61 6765 2e6a 7067 2229 0a69  d("image.jpg").i
+000017b0: 6d61 6765 203d 2063 7632 2e63 7674 436f  mage = cv2.cvtCo
+000017c0: 6c6f 7228 696d 6167 652c 2063 7632 2e43  lor(image, cv2.C
+000017d0: 4f4c 4f52 5f42 4752 3252 4742 290a 0a23  OLOR_BGR2RGB)..#
+000017e0: 2041 7567 6d65 6e74 2061 6e20 696d 6167   Augment an imag
+000017f0: 650a 7472 616e 7366 6f72 6d65 6420 3d20  e.transformed = 
+00001800: 7472 616e 7366 6f72 6d28 696d 6167 653d  transform(image=
+00001810: 696d 6167 6529 0a74 7261 6e73 666f 726d  image).transform
+00001820: 6564 5f69 6d61 6765 203d 2074 7261 6e73  ed_image = trans
+00001830: 666f 726d 6564 5b22 696d 6167 6522 5d0a  formed["image"].
+00001840: 6060 600a 0a23 2320 4765 7474 696e 6720  ```..## Getting 
+00001850: 7374 6172 7465 640a 0a23 2323 2049 2061  started..### I a
+00001860: 6d20 6e65 7720 746f 2069 6d61 6765 2061  m new to image a
+00001870: 7567 6d65 6e74 6174 696f 6e0a 0a50 6c65  ugmentation..Ple
+00001880: 6173 6520 7374 6172 7420 7769 7468 2074  ase start with t
+00001890: 6865 205b 696e 7472 6f64 7563 7469 6f6e  he [introduction
+000018a0: 2061 7274 6963 6c65 735d 2868 7474 7073   articles](https
+000018b0: 3a2f 2f61 6c62 756d 656e 7461 7469 6f6e  ://albumentation
+000018c0: 732e 6169 2f64 6f63 732f 2369 6e74 726f  s.ai/docs/#intro
+000018d0: 6475 6374 696f 6e2d 746f 2d69 6d61 6765  duction-to-image
+000018e0: 2d61 7567 6d65 6e74 6174 696f 6e29 2061  -augmentation) a
+000018f0: 626f 7574 2077 6879 2069 6d61 6765 2061  bout why image a
+00001900: 7567 6d65 6e74 6174 696f 6e20 6973 2069  ugmentation is i
+00001910: 6d70 6f72 7461 6e74 2061 6e64 2068 6f77  mportant and how
+00001920: 2069 7420 6865 6c70 7320 746f 2062 7569   it helps to bui
+00001930: 6c64 2062 6574 7465 7220 6d6f 6465 6c73  ld better models
+00001940: 2e0a 0a23 2323 2049 2077 616e 7420 746f  ...### I want to
+00001950: 2075 7365 2041 6c62 756d 656e 7461 7469   use Albumentati
+00001960: 6f6e 7320 666f 7220 7468 6520 7370 6563  ons for the spec
+00001970: 6966 6963 2074 6173 6b20 7375 6368 2061  ific task such a
+00001980: 7320 636c 6173 7369 6669 6361 7469 6f6e  s classification
+00001990: 206f 7220 7365 676d 656e 7461 7469 6f6e   or segmentation
+000019a0: 0a0a 4966 2079 6f75 2077 616e 7420 746f  ..If you want to
+000019b0: 2075 7365 2041 6c62 756d 656e 7461 7469   use Albumentati
+000019c0: 6f6e 7320 666f 7220 6120 7370 6563 6966  ons for a specif
+000019d0: 6963 2074 6173 6b20 7375 6368 2061 7320  ic task such as 
+000019e0: 636c 6173 7369 6669 6361 7469 6f6e 2c20  classification, 
+000019f0: 7365 676d 656e 7461 7469 6f6e 2c20 6f72  segmentation, or
+00001a00: 206f 626a 6563 7420 6465 7465 6374 696f   object detectio
+00001a10: 6e2c 2072 6566 6572 2074 6f20 7468 6520  n, refer to the 
+00001a20: 5b73 6574 206f 6620 6172 7469 636c 6573  [set of articles
+00001a30: 5d28 6874 7470 733a 2f2f 616c 6275 6d65  ](https://albume
+00001a40: 6e74 6174 696f 6e73 2e61 692f 646f 6373  ntations.ai/docs
+00001a50: 2f23 6765 7474 696e 672d 7374 6172 7465  /#getting-starte
+00001a60: 642d 7769 7468 2d61 6c62 756d 656e 7461  d-with-albumenta
+00001a70: 7469 6f6e 7329 2074 6861 7420 6861 7320  tions) that has 
+00001a80: 616e 2069 6e2d 6465 7074 6820 6465 7363  an in-depth desc
+00001a90: 7269 7074 696f 6e20 6f66 2074 6869 7320  ription of this 
+00001aa0: 7461 736b 2e20 5765 2061 6c73 6f20 6861  task. We also ha
+00001ab0: 7665 2061 205b 6c69 7374 206f 6620 6578  ve a [list of ex
+00001ac0: 616d 706c 6573 5d28 6874 7470 733a 2f2f  amples](https://
+00001ad0: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
+00001ae0: 692f 646f 6373 2f65 7861 6d70 6c65 732f  i/docs/examples/
+00001af0: 2920 6f6e 2061 7070 6c79 696e 6720 416c  ) on applying Al
+00001b00: 6275 6d65 6e74 6174 696f 6e73 2066 6f72  bumentations for
+00001b10: 2064 6966 6665 7265 6e74 2075 7365 2063   different use c
+00001b20: 6173 6573 2e0a 0a23 2323 2049 2077 616e  ases...### I wan
+00001b30: 7420 746f 206b 6e6f 7720 686f 7720 746f  t to know how to
+00001b40: 2075 7365 2041 6c62 756d 656e 7461 7469   use Albumentati
+00001b50: 6f6e 7320 7769 7468 2064 6565 7020 6c65  ons with deep le
+00001b60: 6172 6e69 6e67 2066 7261 6d65 776f 726b  arning framework
+00001b70: 730a 0a57 6520 6861 7665 205b 6578 616d  s..We have [exam
+00001b80: 706c 6573 206f 6620 7573 696e 6720 416c  ples of using Al
+00001b90: 6275 6d65 6e74 6174 696f 6e73 5d28 6874  bumentations](ht
+00001ba0: 7470 733a 2f2f 616c 6275 6d65 6e74 6174  tps://albumentat
+00001bb0: 696f 6e73 2e61 692f 646f 6373 2f23 6578  ions.ai/docs/#ex
+00001bc0: 616d 706c 6573 2d6f 662d 686f 772d 746f  amples-of-how-to
+00001bd0: 2d75 7365 2d61 6c62 756d 656e 7461 7469  -use-albumentati
+00001be0: 6f6e 732d 7769 7468 2d64 6966 6665 7265  ons-with-differe
+00001bf0: 6e74 2d64 6565 702d 6c65 6172 6e69 6e67  nt-deep-learning
+00001c00: 2d66 7261 6d65 776f 726b 7329 2061 6c6f  -frameworks) alo
+00001c10: 6e67 2077 6974 6820 5079 546f 7263 6820  ng with PyTorch 
+00001c20: 616e 6420 5465 6e73 6f72 466c 6f77 2e0a  and TensorFlow..
+00001c30: 0a23 2323 2049 2077 616e 7420 746f 2065  .### I want to e
+00001c40: 7870 6c6f 7265 2061 7567 6d65 6e74 6174  xplore augmentat
+00001c50: 696f 6e73 2061 6e64 2073 6565 2041 6c62  ions and see Alb
+00001c60: 756d 656e 7461 7469 6f6e 7320 696e 2061  umentations in a
+00001c70: 6374 696f 6e0a 0a43 6865 636b 2074 6865  ction..Check the
+00001c80: 205b 6f6e 6c69 6e65 2064 656d 6f20 6f66   [online demo of
+00001c90: 2074 6865 206c 6962 7261 7279 5d28 6874   the library](ht
+00001ca0: 7470 733a 2f2f 616c 6275 6d65 6e74 6174  tps://albumentat
+00001cb0: 696f 6e73 2d64 656d 6f2e 6865 726f 6b75  ions-demo.heroku
+00001cc0: 6170 702e 636f 6d2f 292e 2057 6974 6820  app.com/). With 
+00001cd0: 6974 2c20 796f 7520 6361 6e20 6170 706c  it, you can appl
+00001ce0: 7920 6175 676d 656e 7461 7469 6f6e 7320  y augmentations 
+00001cf0: 746f 2064 6966 6665 7265 6e74 2069 6d61  to different ima
+00001d00: 6765 7320 616e 6420 7365 6520 7468 6520  ges and see the 
+00001d10: 7265 7375 6c74 2e20 416c 736f 2c20 7765  result. Also, we
+00001d20: 2068 6176 6520 6120 5b6c 6973 7420 6f66   have a [list of
+00001d30: 2061 6c6c 2061 7661 696c 6162 6c65 2061   all available a
+00001d40: 7567 6d65 6e74 6174 696f 6e73 2061 6e64  ugmentations and
+00001d50: 2074 6865 6972 2074 6172 6765 7473 5d28   their targets](
+00001d60: 236c 6973 742d 6f66 2d61 7567 6d65 6e74  #list-of-augment
+00001d70: 6174 696f 6e73 292e 0a0a 2323 2057 686f  ations)...## Who
+00001d80: 2069 7320 7573 696e 6720 416c 6275 6d65   is using Albume
+00001d90: 6e74 6174 696f 6e73 0a0a 3c61 2068 7265  ntations..<a hre
+00001da0: 663d 2268 7474 7073 3a2f 2f77 7777 2e61  f="https://www.a
+00001db0: 7070 6c65 2e63 6f6d 2f22 2074 6172 6765  pple.com/" targe
+00001dc0: 743d 225f 626c 616e 6b22 3e3c 696d 6720  t="_blank"><img 
+00001dd0: 7372 633d 2268 7474 7073 3a2f 2f72 6177  src="https://raw
+00001de0: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
+00001df0: 6e74 2e63 6f6d 2f61 6c62 756d 656e 7461  nt.com/albumenta
+00001e00: 7469 6f6e 732d 7465 616d 2f61 6c62 756d  tions-team/album
+00001e10: 656e 7461 7469 6f6e 732e 6169 2f6d 6169  entations.ai/mai
+00001e20: 6e2f 6874 6d6c 2f61 7373 6574 732f 696d  n/html/assets/im
+00001e30: 672f 696e 6475 7374 7279 2f61 7070 6c65  g/industry/apple
+00001e40: 2e6a 7065 6722 2077 6964 7468 3d22 3130  .jpeg" width="10
+00001e50: 3022 2f3e 3c2f 613e 0a3c 6120 6872 6566  0"/></a>.<a href
+00001e60: 3d22 6874 7470 733a 2f2f 7265 7365 6172  ="https://resear
+00001e70: 6368 2e67 6f6f 676c 652f 2220 7461 7267  ch.google/" targ
+00001e80: 6574 3d22 5f62 6c61 6e6b 223e 3c69 6d67  et="_blank"><img
+00001e90: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
+00001ea0: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
+00001eb0: 656e 742e 636f 6d2f 616c 6275 6d65 6e74  ent.com/albument
+00001ec0: 6174 696f 6e73 2d74 6561 6d2f 616c 6275  ations-team/albu
+00001ed0: 6d65 6e74 6174 696f 6e73 2e61 692f 6d61  mentations.ai/ma
+00001ee0: 696e 2f68 746d 6c2f 6173 7365 7473 2f69  in/html/assets/i
+00001ef0: 6d67 2f69 6e64 7573 7472 792f 676f 6f67  mg/industry/goog
+00001f00: 6c65 2e70 6e67 2220 7769 6474 683d 2231  le.png" width="1
+00001f10: 3030 222f 3e3c 2f61 3e0a 3c61 2068 7265  00"/></a>.<a hre
+00001f20: 663d 2268 7474 7073 3a2f 2f6f 7065 6e73  f="https://opens
+00001f30: 6f75 7263 652e 6662 2e63 6f6d 2f22 2074  ource.fb.com/" t
+00001f40: 6172 6765 743d 225f 626c 616e 6b22 3e3c  arget="_blank"><
+00001f50: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00001f60: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
+00001f70: 6f6e 7465 6e74 2e63 6f6d 2f61 6c62 756d  ontent.com/album
+00001f80: 656e 7461 7469 6f6e 732d 7465 616d 2f61  entations-team/a
+00001f90: 6c62 756d 656e 7461 7469 6f6e 732e 6169  lbumentations.ai
+00001fa0: 2f6d 6169 6e2f 6874 6d6c 2f61 7373 6574  /main/html/asset
+00001fb0: 732f 696d 672f 696e 6475 7374 7279 2f6d  s/img/industry/m
+00001fc0: 6574 615f 7265 7365 6172 6368 2e70 6e67  eta_research.png
+00001fd0: 2220 7769 6474 683d 2231 3030 222f 3e3c  " width="100"/><
+00001fe0: 2f61 3e0a 3c61 2068 7265 663d 2268 7474  /a>.<a href="htt
+00001ff0: 7073 3a20 2f2f 7777 772e 6e76 6964 6961  ps: //www.nvidia
+00002000: 2e63 6f6d 2f65 6e2d 7573 2f72 6573 6561  .com/en-us/resea
+00002010: 7263 682f 2220 7461 7267 6574 3d22 5f62  rch/" target="_b
+00002020: 6c61 6e6b 223e 3c69 6d67 2073 7263 3d22  lank"><img src="
+00002030: 6874 7470 733a 2f2f 7261 772e 6769 7468  https://raw.gith
+00002040: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
+00002050: 6d2f 616c 6275 6d65 6e74 6174 696f 6e73  m/albumentations
+00002060: 2d74 6561 6d2f 616c 6275 6d65 6e74 6174  -team/albumentat
+00002070: 696f 6e73 2e61 692f 6d61 696e 2f68 746d  ions.ai/main/htm
+00002080: 6c2f 6173 7365 7473 2f69 6d67 2f69 6e64  l/assets/img/ind
+00002090: 7573 7472 792f 6e76 6964 6961 5f72 6573  ustry/nvidia_res
+000020a0: 6561 7263 682e 6a70 6567 2220 7769 6474  earch.jpeg" widt
+000020b0: 683d 2231 3030 222f 3e3c 2f61 3e0a 3c61  h="100"/></a>.<a
+000020c0: 2068 7265 663d 2268 7474 7073 3a2f 2f77   href="https://w
+000020d0: 7777 2e61 6d61 7a6f 6e2e 7363 6965 6e63  ww.amazon.scienc
+000020e0: 652f 2220 7461 7267 6574 3d22 5f62 6c61  e/" target="_bla
+000020f0: 6e6b 223e 3c69 6d67 2073 7263 3d22 6874  nk"><img src="ht
+00002100: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
+00002110: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+00002120: 616c 6275 6d65 6e74 6174 696f 6e73 2d74  albumentations-t
+00002130: 6561 6d2f 616c 6275 6d65 6e74 6174 696f  eam/albumentatio
+00002140: 6e73 2e61 692f 6d61 696e 2f68 746d 6c2f  ns.ai/main/html/
+00002150: 6173 7365 7473 2f69 6d67 2f69 6e64 7573  assets/img/indus
+00002160: 7472 792f 616d 617a 6f6e 5f73 6369 656e  try/amazon_scien
+00002170: 6365 2e70 6e67 2220 7769 6474 683d 2231  ce.png" width="1
+00002180: 3030 222f 3e3c 2f61 3e0a 3c61 2068 7265  00"/></a>.<a hre
+00002190: 663d 2268 7474 7073 3a2f 2f6f 7065 6e73  f="https://opens
+000021a0: 6f75 7263 652e 6d69 6372 6f73 6f66 742e  ource.microsoft.
+000021b0: 636f 6d2f 2220 7461 7267 6574 3d22 5f62  com/" target="_b
+000021c0: 6c61 6e6b 223e 3c69 6d67 2073 7263 3d22  lank"><img src="
+000021d0: 6874 7470 733a 2f2f 7261 772e 6769 7468  https://raw.gith
+000021e0: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
+000021f0: 6d2f 616c 6275 6d65 6e74 6174 696f 6e73  m/albumentations
+00002200: 2d74 6561 6d2f 616c 6275 6d65 6e74 6174  -team/albumentat
+00002210: 696f 6e73 2e61 692f 6d61 696e 2f68 746d  ions.ai/main/htm
+00002220: 6c2f 6173 7365 7473 2f69 6d67 2f69 6e64  l/assets/img/ind
+00002230: 7573 7472 792f 6d69 6372 6f73 6f66 742e  ustry/microsoft.
+00002240: 706e 6722 2077 6964 7468 3d22 3130 3022  png" width="100"
+00002250: 2f3e 3c2f 613e 0a3c 6120 6872 6566 3d22  /></a>.<a href="
+00002260: 6874 7470 733a 2f2f 656e 6769 6e65 6572  https://engineer
+00002270: 696e 672e 7361 6c65 7366 6f72 6365 2e63  ing.salesforce.c
+00002280: 6f6d 2f6f 7065 6e2d 736f 7572 6365 2f22  om/open-source/"
+00002290: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
+000022a0: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
+000022b0: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
+000022c0: 7263 6f6e 7465 6e74 2e63 6f6d 2f61 6c62  rcontent.com/alb
+000022d0: 756d 656e 7461 7469 6f6e 732d 7465 616d  umentations-team
+000022e0: 2f61 6c62 756d 656e 7461 7469 6f6e 732e  /albumentations.
+000022f0: 6169 2f6d 6169 6e2f 6874 6d6c 2f61 7373  ai/main/html/ass
+00002300: 6574 732f 696d 672f 696e 6475 7374 7279  ets/img/industry
+00002310: 2f73 616c 6573 666f 7263 655f 6f70 656e  /salesforce_open
+00002320: 5f73 6f75 7263 652e 706e 6722 2077 6964  _source.png" wid
+00002330: 7468 3d22 3130 3022 2f3e 3c2f 613e 0a3c  th="100"/></a>.<
+00002340: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00002350: 7374 6162 696c 6974 792e 6169 2f22 2074  stability.ai/" t
+00002360: 6172 6765 743d 225f 626c 616e 6b22 3e3c  arget="_blank"><
+00002370: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00002380: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
+00002390: 6f6e 7465 6e74 2e63 6f6d 2f61 6c62 756d  ontent.com/album
+000023a0: 656e 7461 7469 6f6e 732d 7465 616d 2f61  entations-team/a
+000023b0: 6c62 756d 656e 7461 7469 6f6e 732e 6169  lbumentations.ai
+000023c0: 2f6d 6169 6e2f 6874 6d6c 2f61 7373 6574  /main/html/asset
+000023d0: 732f 696d 672f 696e 6475 7374 7279 2f73  s/img/industry/s
+000023e0: 7461 6269 6c69 7479 2e70 6e67 2220 7769  tability.png" wi
+000023f0: 6474 683d 2231 3030 222f 3e3c 2f61 3e0a  dth="100"/></a>.
+00002400: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00002410: 2f77 7777 2e69 626d 2e63 6f6d 2f6f 7065  /www.ibm.com/ope
+00002420: 6e73 6f75 7263 652f 2220 7461 7267 6574  nsource/" target
+00002430: 3d22 5f62 6c61 6e6b 223e 3c69 6d67 2073  ="_blank"><img s
+00002440: 7263 3d22 6874 7470 733a 2f2f 7261 772e  rc="https://raw.
+00002450: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+00002460: 742e 636f 6d2f 616c 6275 6d65 6e74 6174  t.com/albumentat
+00002470: 696f 6e73 2d74 6561 6d2f 616c 6275 6d65  ions-team/albume
+00002480: 6e74 6174 696f 6e73 2e61 692f 6d61 696e  ntations.ai/main
+00002490: 2f68 746d 6c2f 6173 7365 7473 2f69 6d67  /html/assets/img
+000024a0: 2f69 6e64 7573 7472 792f 6962 6d2e 6a70  /industry/ibm.jp
+000024b0: 6567 2220 7769 6474 683d 2231 3030 222f  eg" width="100"/
+000024c0: 3e3c 2f61 3e0a 3c61 2068 7265 663d 2268  ></a>.<a href="h
+000024d0: 7474 7073 3a2f 2f68 7567 6769 6e67 6661  ttps://huggingfa
+000024e0: 6365 2e63 6f2f 2220 7461 7267 6574 3d22  ce.co/" target="
+000024f0: 5f62 6c61 6e6b 223e 3c69 6d67 2073 7263  _blank"><img src
+00002500: 3d22 6874 7470 733a 2f2f 7261 772e 6769  ="https://raw.gi
+00002510: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
+00002520: 636f 6d2f 616c 6275 6d65 6e74 6174 696f  com/albumentatio
+00002530: 6e73 2d74 6561 6d2f 616c 6275 6d65 6e74  ns-team/albument
+00002540: 6174 696f 6e73 2e61 692f 6d61 696e 2f68  ations.ai/main/h
+00002550: 746d 6c2f 6173 7365 7473 2f69 6d67 2f69  tml/assets/img/i
+00002560: 6e64 7573 7472 792f 6875 6767 696e 675f  ndustry/hugging_
+00002570: 6661 6365 2e70 6e67 2220 7769 6474 683d  face.png" width=
+00002580: 2231 3030 222f 3e3c 2f61 3e0a 3c61 2068  "100"/></a>.<a h
+00002590: 7265 663d 2268 7474 7073 3a2f 2f77 7777  ref="https://www
+000025a0: 2e73 6f6e 792e 636f 6d2f 656e 2f22 2074  .sony.com/en/" t
+000025b0: 6172 6765 743d 225f 626c 616e 6b22 3e3c  arget="_blank"><
+000025c0: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+000025d0: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
+000025e0: 6f6e 7465 6e74 2e63 6f6d 2f61 6c62 756d  ontent.com/album
+000025f0: 656e 7461 7469 6f6e 732d 7465 616d 2f61  entations-team/a
+00002600: 6c62 756d 656e 7461 7469 6f6e 732e 6169  lbumentations.ai
+00002610: 2f6d 6169 6e2f 6874 6d6c 2f61 7373 6574  /main/html/asset
+00002620: 732f 696d 672f 696e 6475 7374 7279 2f73  s/img/industry/s
+00002630: 6f6e 792e 706e 6722 2077 6964 7468 3d22  ony.png" width="
+00002640: 3130 3022 2f3e 3c2f 613e 0a3c 6120 6872  100"/></a>.<a hr
+00002650: 6566 3d22 6874 7470 733a 2f2f 6f70 656e  ef="https://open
+00002660: 736f 7572 6365 2e61 6c69 6261 6261 2e63  source.alibaba.c
+00002670: 6f6d 2f22 2074 6172 6765 743d 225f 626c  om/" target="_bl
+00002680: 616e 6b22 3e3c 696d 6720 7372 633d 2268  ank"><img src="h
+00002690: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
+000026a0: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+000026b0: 2f61 6c62 756d 656e 7461 7469 6f6e 732d  /albumentations-
+000026c0: 7465 616d 2f61 6c62 756d 656e 7461 7469  team/albumentati
+000026d0: 6f6e 732e 6169 2f6d 6169 6e2f 6874 6d6c  ons.ai/main/html
+000026e0: 2f61 7373 6574 732f 696d 672f 696e 6475  /assets/img/indu
+000026f0: 7374 7279 2f61 6c69 6261 6261 2e70 6e67  stry/alibaba.png
+00002700: 2220 7769 6474 683d 2231 3030 222f 3e3c  " width="100"/><
+00002710: 2f61 3e0a 3c61 2068 7265 663d 2268 7474  /a>.<a href="htt
+00002720: 7073 3a2f 2f6f 7065 6e73 6f75 7263 652e  ps://opensource.
+00002730: 7465 6e63 656e 742e 636f 6d2f 2220 7461  tencent.com/" ta
+00002740: 7267 6574 3d22 5f62 6c61 6e6b 223e 3c69  rget="_blank"><i
+00002750: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00002760: 7261 772e 6769 7468 7562 7573 6572 636f  raw.githubuserco
+00002770: 6e74 656e 742e 636f 6d2f 616c 6275 6d65  ntent.com/albume
+00002780: 6e74 6174 696f 6e73 2d74 6561 6d2f 616c  ntations-team/al
+00002790: 6275 6d65 6e74 6174 696f 6e73 2e61 692f  bumentations.ai/
+000027a0: 6d61 696e 2f68 746d 6c2f 6173 7365 7473  main/html/assets
+000027b0: 2f69 6d67 2f69 6e64 7573 7472 792f 7465  /img/industry/te
+000027c0: 6e63 656e 742e 706e 6722 2077 6964 7468  ncent.png" width
+000027d0: 3d22 3130 3022 2f3e 3c2f 613e 0a3c 6120  ="100"/></a>.<a 
+000027e0: 6872 6566 3d22 6874 7470 733a 2f2f 6832  href="https://h2
+000027f0: 6f2e 6169 2f22 2074 6172 6765 743d 225f  o.ai/" target="_
+00002800: 626c 616e 6b22 3e3c 696d 6720 7372 633d  blank"><img src=
+00002810: 2268 7474 7073 3a2f 2f72 6177 2e67 6974  "https://raw.git
+00002820: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+00002830: 6f6d 2f61 6c62 756d 656e 7461 7469 6f6e  om/albumentation
+00002840: 732d 7465 616d 2f61 6c62 756d 656e 7461  s-team/albumenta
+00002850: 7469 6f6e 732e 6169 2f6d 6169 6e2f 6874  tions.ai/main/ht
+00002860: 6d6c 2f61 7373 6574 732f 696d 672f 696e  ml/assets/img/in
+00002870: 6475 7374 7279 2f68 326f 5f61 692e 706e  dustry/h2o_ai.pn
+00002880: 6722 2077 6964 7468 3d22 3130 3022 2f3e  g" width="100"/>
+00002890: 3c2f 613e 0a0a 2323 2320 5365 6520 616c  </a>..### See al
+000028a0: 736f 0a0a 2d20 5b41 206c 6973 7420 6f66  so..- [A list of
+000028b0: 2070 6170 6572 7320 7468 6174 2063 6974   papers that cit
+000028c0: 6520 416c 6275 6d65 6e74 6174 696f 6e73  e Albumentations
+000028d0: 5d28 6874 7470 733a 2f2f 7363 686f 6c61  ](https://schola
+000028e0: 722e 676f 6f67 6c65 2e63 6f6d 2f63 6974  r.google.com/cit
+000028f0: 6174 696f 6e73 3f76 6965 775f 6f70 3d76  ations?view_op=v
+00002900: 6965 775f 6369 7461 7469 6f6e 2663 6974  iew_citation&cit
+00002910: 6174 696f 6e5f 666f 725f 7669 6577 3d76  ation_for_view=v
+00002920: 6b6a 6839 5830 4141 4141 4a3a 7230 4270  kjh9X0AAAAJ:r0Bp
+00002930: 6e74 5a71 4a47 3443 292e 0a2d 205b 4120  ntZqJG4C)..- [A 
+00002940: 6c69 7374 206f 6620 7465 616d 7320 7468  list of teams th
+00002950: 6174 2077 6572 6520 7573 696e 6720 416c  at were using Al
+00002960: 6275 6d65 6e74 6174 696f 6e73 2061 6e64  bumentations and
+00002970: 2074 6f6f 6b20 6869 6768 2070 6c61 6365   took high place
+00002980: 7320 696e 206d 6163 6869 6e65 206c 6561  s in machine lea
+00002990: 726e 696e 6720 636f 6d70 6574 6974 696f  rning competitio
+000029a0: 6e73 5d28 6874 7470 733a 2f2f 616c 6275  ns](https://albu
+000029b0: 6d65 6e74 6174 696f 6e73 2e61 692f 7768  mentations.ai/wh
+000029c0: 6f73 5f75 7369 6e67 2363 6f6d 7065 7469  os_using#competi
+000029d0: 7469 6f6e 7329 2e0a 2d20 5b4f 7065 6e20  tions)..- [Open 
+000029e0: 736f 7572 6365 2070 726f 6a65 6374 7320  source projects 
+000029f0: 7468 6174 2075 7365 2041 6c62 756d 656e  that use Albumen
+00002a00: 7461 7469 6f6e 735d 2868 7474 7073 3a2f  tations](https:/
+00002a10: 2f67 6974 6875 622e 636f 6d2f 616c 6275  /github.com/albu
+00002a20: 6d65 6e74 6174 696f 6e73 2d74 6561 6d2f  mentations-team/
+00002a30: 616c 6275 6d65 6e74 6174 696f 6e73 2f6e  albumentations/n
+00002a40: 6574 776f 726b 2f64 6570 656e 6465 6e74  etwork/dependent
+00002a50: 733f 6465 7065 6e64 656e 745f 7479 7065  s?dependent_type
+00002a60: 3d50 4143 4b41 4745 292e 0a0a 2323 204c  =PACKAGE)...## L
+00002a70: 6973 7420 6f66 2061 7567 6d65 6e74 6174  ist of augmentat
+00002a80: 696f 6e73 0a0a 2323 2320 5069 7865 6c2d  ions..### Pixel-
+00002a90: 6c65 7665 6c20 7472 616e 7366 6f72 6d73  level transforms
+00002aa0: 0a0a 5069 7865 6c2d 6c65 7665 6c20 7472  ..Pixel-level tr
+00002ab0: 616e 7366 6f72 6d73 2077 696c 6c20 6368  ansforms will ch
+00002ac0: 616e 6765 206a 7573 7420 616e 2069 6e70  ange just an inp
+00002ad0: 7574 2069 6d61 6765 2061 6e64 2077 696c  ut image and wil
+00002ae0: 6c20 6c65 6176 6520 616e 7920 6164 6469  l leave any addi
+00002af0: 7469 6f6e 616c 2074 6172 6765 7473 2073  tional targets s
+00002b00: 7563 6820 6173 206d 6173 6b73 2c20 626f  uch as masks, bo
+00002b10: 756e 6469 6e67 2062 6f78 6573 2c20 616e  unding boxes, an
+00002b20: 6420 6b65 7970 6f69 6e74 7320 756e 6368  d keypoints unch
+00002b30: 616e 6765 642e 2054 6865 206c 6973 7420  anged. The list 
+00002b40: 6f66 2070 6978 656c 2d6c 6576 656c 2074  of pixel-level t
+00002b50: 7261 6e73 666f 726d 733a 0a0a 2d20 5b41  ransforms:..- [A
+00002b60: 6476 616e 6365 6442 6c75 725d 2868 7474  dvancedBlur](htt
+00002b70: 7073 3a2f 2f61 6c62 756d 656e 7461 7469  ps://albumentati
+00002b80: 6f6e 732e 6169 2f64 6f63 732f 6170 695f  ons.ai/docs/api_
+00002b90: 7265 6665 7265 6e63 652f 6175 676d 656e  reference/augmen
+00002ba0: 7461 7469 6f6e 732f 626c 7572 2f74 7261  tations/blur/tra
+00002bb0: 6e73 666f 726d 732f 2361 6c62 756d 656e  nsforms/#albumen
+00002bc0: 7461 7469 6f6e 732e 6175 676d 656e 7461  tations.augmenta
+00002bd0: 7469 6f6e 732e 626c 7572 2e74 7261 6e73  tions.blur.trans
+00002be0: 666f 726d 732e 4164 7661 6e63 6564 426c  forms.AdvancedBl
+00002bf0: 7572 290a 2d20 5b42 6c75 725d 2868 7474  ur).- [Blur](htt
+00002c00: 7073 3a2f 2f61 6c62 756d 656e 7461 7469  ps://albumentati
+00002c10: 6f6e 732e 6169 2f64 6f63 732f 6170 695f  ons.ai/docs/api_
+00002c20: 7265 6665 7265 6e63 652f 6175 676d 656e  reference/augmen
+00002c30: 7461 7469 6f6e 732f 626c 7572 2f74 7261  tations/blur/tra
+00002c40: 6e73 666f 726d 732f 2361 6c62 756d 656e  nsforms/#albumen
+00002c50: 7461 7469 6f6e 732e 6175 676d 656e 7461  tations.augmenta
+00002c60: 7469 6f6e 732e 626c 7572 2e74 7261 6e73  tions.blur.trans
+00002c70: 666f 726d 732e 426c 7572 290a 2d20 5b43  forms.Blur).- [C
+00002c80: 4c41 4845 5d28 6874 7470 733a 2f2f 616c  LAHE](https://al
+00002c90: 6275 6d65 6e74 6174 696f 6e73 2e61 692f  bumentations.ai/
+00002ca0: 646f 6373 2f61 7069 5f72 6566 6572 656e  docs/api_referen
+00002cb0: 6365 2f61 7567 6d65 6e74 6174 696f 6e73  ce/augmentations
+00002cc0: 2f74 7261 6e73 666f 726d 732f 2361 6c62  /transforms/#alb
+00002cd0: 756d 656e 7461 7469 6f6e 732e 6175 676d  umentations.augm
+00002ce0: 656e 7461 7469 6f6e 732e 7472 616e 7366  entations.transf
+00002cf0: 6f72 6d73 2e43 4c41 4845 290a 2d20 5b43  orms.CLAHE).- [C
+00002d00: 6861 6e6e 656c 4472 6f70 6f75 745d 2868  hannelDropout](h
+00002d10: 7474 7073 3a2f 2f61 6c62 756d 656e 7461  ttps://albumenta
+00002d20: 7469 6f6e 732e 6169 2f64 6f63 732f 6170  tions.ai/docs/ap
+00002d30: 695f 7265 6665 7265 6e63 652f 6175 676d  i_reference/augm
+00002d40: 656e 7461 7469 6f6e 732f 6472 6f70 6f75  entations/dropou
+00002d50: 742f 6368 616e 6e65 6c5f 6472 6f70 6f75  t/channel_dropou
+00002d60: 742f 2361 6c62 756d 656e 7461 7469 6f6e  t/#albumentation
+00002d70: 732e 6175 676d 656e 7461 7469 6f6e 732e  s.augmentations.
+00002d80: 6472 6f70 6f75 742e 6368 616e 6e65 6c5f  dropout.channel_
+00002d90: 6472 6f70 6f75 742e 4368 616e 6e65 6c44  dropout.ChannelD
+00002da0: 726f 706f 7574 290a 2d20 5b43 6861 6e6e  ropout).- [Chann
+00002db0: 656c 5368 7566 666c 655d 2868 7474 7073  elShuffle](https
+00002dc0: 3a2f 2f61 6c62 756d 656e 7461 7469 6f6e  ://albumentation
+00002dd0: 732e 6169 2f64 6f63 732f 6170 695f 7265  s.ai/docs/api_re
+00002de0: 6665 7265 6e63 652f 6175 676d 656e 7461  ference/augmenta
+00002df0: 7469 6f6e 732f 7472 616e 7366 6f72 6d73  tions/transforms
+00002e00: 2f23 616c 6275 6d65 6e74 6174 696f 6e73  /#albumentations
+00002e10: 2e61 7567 6d65 6e74 6174 696f 6e73 2e74  .augmentations.t
+00002e20: 7261 6e73 666f 726d 732e 4368 616e 6e65  ransforms.Channe
+00002e30: 6c53 6875 6666 6c65 290a 2d20 5b43 6872  lShuffle).- [Chr
+00002e40: 6f6d 6174 6963 4162 6572 7261 7469 6f6e  omaticAberration
+00002e50: 5d28 6874 7470 733a 2f2f 616c 6275 6d65  ](https://albume
+00002e60: 6e74 6174 696f 6e73 2e61 692f 646f 6373  ntations.ai/docs
+00002e70: 2f61 7069 5f72 6566 6572 656e 6365 2f61  /api_reference/a
+00002e80: 7567 6d65 6e74 6174 696f 6e73 2f74 7261  ugmentations/tra
+00002e90: 6e73 666f 726d 732f 2361 6c62 756d 656e  nsforms/#albumen
+00002ea0: 7461 7469 6f6e 732e 6175 676d 656e 7461  tations.augmenta
+00002eb0: 7469 6f6e 732e 7472 616e 7366 6f72 6d73  tions.transforms
+00002ec0: 2e43 6872 6f6d 6174 6963 4162 6572 7261  .ChromaticAberra
+00002ed0: 7469 6f6e 290a 2d20 5b43 6f6c 6f72 4a69  tion).- [ColorJi
+00002ee0: 7474 6572 5d28 6874 7470 733a 2f2f 616c  tter](https://al
+00002ef0: 6275 6d65 6e74 6174 696f 6e73 2e61 692f  bumentations.ai/
+00002f00: 646f 6373 2f61 7069 5f72 6566 6572 656e  docs/api_referen
+00002f10: 6365 2f61 7567 6d65 6e74 6174 696f 6e73  ce/augmentations
+00002f20: 2f74 7261 6e73 666f 726d 732f 2361 6c62  /transforms/#alb
+00002f30: 756d 656e 7461 7469 6f6e 732e 6175 676d  umentations.augm
+00002f40: 656e 7461 7469 6f6e 732e 7472 616e 7366  entations.transf
+00002f50: 6f72 6d73 2e43 6f6c 6f72 4a69 7474 6572  orms.ColorJitter
+00002f60: 290a 2d20 5b44 6566 6f63 7573 5d28 6874  ).- [Defocus](ht
+00002f70: 7470 733a 2f2f 616c 6275 6d65 6e74 6174  tps://albumentat
+00002f80: 696f 6e73 2e61 692f 646f 6373 2f61 7069  ions.ai/docs/api
+00002f90: 5f72 6566 6572 656e 6365 2f61 7567 6d65  _reference/augme
+00002fa0: 6e74 6174 696f 6e73 2f62 6c75 722f 7472  ntations/blur/tr
+00002fb0: 616e 7366 6f72 6d73 2f23 616c 6275 6d65  ansforms/#albume
+00002fc0: 6e74 6174 696f 6e73 2e61 7567 6d65 6e74  ntations.augment
+00002fd0: 6174 696f 6e73 2e62 6c75 722e 7472 616e  ations.blur.tran
+00002fe0: 7366 6f72 6d73 2e44 6566 6f63 7573 290a  sforms.Defocus).
+00002ff0: 2d20 5b44 6f77 6e73 6361 6c65 5d28 6874  - [Downscale](ht
+00003000: 7470 733a 2f2f 616c 6275 6d65 6e74 6174  tps://albumentat
+00003010: 696f 6e73 2e61 692f 646f 6373 2f61 7069  ions.ai/docs/api
+00003020: 5f72 6566 6572 656e 6365 2f61 7567 6d65  _reference/augme
+00003030: 6e74 6174 696f 6e73 2f74 7261 6e73 666f  ntations/transfo
+00003040: 726d 732f 2361 6c62 756d 656e 7461 7469  rms/#albumentati
+00003050: 6f6e 732e 6175 676d 656e 7461 7469 6f6e  ons.augmentation
+00003060: 732e 7472 616e 7366 6f72 6d73 2e44 6f77  s.transforms.Dow
+00003070: 6e73 6361 6c65 290a 2d20 5b45 6d62 6f73  nscale).- [Embos
+00003080: 735d 2868 7474 7073 3a2f 2f61 6c62 756d  s](https://album
+00003090: 656e 7461 7469 6f6e 732e 6169 2f64 6f63  entations.ai/doc
+000030a0: 732f 6170 695f 7265 6665 7265 6e63 652f  s/api_reference/
+000030b0: 6175 676d 656e 7461 7469 6f6e 732f 7472  augmentations/tr
+000030c0: 616e 7366 6f72 6d73 2f23 616c 6275 6d65  ansforms/#albume
+000030d0: 6e74 6174 696f 6e73 2e61 7567 6d65 6e74  ntations.augment
+000030e0: 6174 696f 6e73 2e74 7261 6e73 666f 726d  ations.transform
+000030f0: 732e 456d 626f 7373 290a 2d20 5b45 7175  s.Emboss).- [Equ
+00003100: 616c 697a 655d 2868 7474 7073 3a2f 2f61  alize](https://a
+00003110: 6c62 756d 656e 7461 7469 6f6e 732e 6169  lbumentations.ai
+00003120: 2f64 6f63 732f 6170 695f 7265 6665 7265  /docs/api_refere
+00003130: 6e63 652f 6175 676d 656e 7461 7469 6f6e  nce/augmentation
+00003140: 732f 7472 616e 7366 6f72 6d73 2f23 616c  s/transforms/#al
+00003150: 6275 6d65 6e74 6174 696f 6e73 2e61 7567  bumentations.aug
+00003160: 6d65 6e74 6174 696f 6e73 2e74 7261 6e73  mentations.trans
+00003170: 666f 726d 732e 4571 7561 6c69 7a65 290a  forms.Equalize).
+00003180: 2d20 5b46 4441 5d28 6874 7470 733a 2f2f  - [FDA](https://
+00003190: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
+000031a0: 692f 646f 6373 2f61 7069 5f72 6566 6572  i/docs/api_refer
+000031b0: 656e 6365 2f61 7567 6d65 6e74 6174 696f  ence/augmentatio
+000031c0: 6e73 2f64 6f6d 6169 6e5f 6164 6170 7461  ns/domain_adapta
+000031d0: 7469 6f6e 2f23 616c 6275 6d65 6e74 6174  tion/#albumentat
+000031e0: 696f 6e73 2e61 7567 6d65 6e74 6174 696f  ions.augmentatio
+000031f0: 6e73 2e64 6f6d 6169 6e5f 6164 6170 7461  ns.domain_adapta
+00003200: 7469 6f6e 2e46 4441 290a 2d20 5b46 616e  tion.FDA).- [Fan
+00003210: 6379 5043 415d 2868 7474 7073 3a2f 2f61  cyPCA](https://a
+00003220: 6c62 756d 656e 7461 7469 6f6e 732e 6169  lbumentations.ai
+00003230: 2f64 6f63 732f 6170 695f 7265 6665 7265  /docs/api_refere
+00003240: 6e63 652f 6175 676d 656e 7461 7469 6f6e  nce/augmentation
+00003250: 732f 7472 616e 7366 6f72 6d73 2f23 616c  s/transforms/#al
+00003260: 6275 6d65 6e74 6174 696f 6e73 2e61 7567  bumentations.aug
+00003270: 6d65 6e74 6174 696f 6e73 2e74 7261 6e73  mentations.trans
+00003280: 666f 726d 732e 4661 6e63 7950 4341 290a  forms.FancyPCA).
+00003290: 2d20 5b46 726f 6d46 6c6f 6174 5d28 6874  - [FromFloat](ht
+000032a0: 7470 733a 2f2f 616c 6275 6d65 6e74 6174  tps://albumentat
+000032b0: 696f 6e73 2e61 692f 646f 6373 2f61 7069  ions.ai/docs/api
+000032c0: 5f72 6566 6572 656e 6365 2f61 7567 6d65  _reference/augme
+000032d0: 6e74 6174 696f 6e73 2f74 7261 6e73 666f  ntations/transfo
+000032e0: 726d 732f 2361 6c62 756d 656e 7461 7469  rms/#albumentati
+000032f0: 6f6e 732e 6175 676d 656e 7461 7469 6f6e  ons.augmentation
+00003300: 732e 7472 616e 7366 6f72 6d73 2e46 726f  s.transforms.Fro
+00003310: 6d46 6c6f 6174 290a 2d20 5b47 6175 7373  mFloat).- [Gauss
+00003320: 4e6f 6973 655d 2868 7474 7073 3a2f 2f61  Noise](https://a
+00003330: 6c62 756d 656e 7461 7469 6f6e 732e 6169  lbumentations.ai
+00003340: 2f64 6f63 732f 6170 695f 7265 6665 7265  /docs/api_refere
+00003350: 6e63 652f 6175 676d 656e 7461 7469 6f6e  nce/augmentation
+00003360: 732f 7472 616e 7366 6f72 6d73 2f23 616c  s/transforms/#al
+00003370: 6275 6d65 6e74 6174 696f 6e73 2e61 7567  bumentations.aug
+00003380: 6d65 6e74 6174 696f 6e73 2e74 7261 6e73  mentations.trans
+00003390: 666f 726d 732e 4761 7573 734e 6f69 7365  forms.GaussNoise
+000033a0: 290a 2d20 5b47 6175 7373 6961 6e42 6c75  ).- [GaussianBlu
+000033b0: 725d 2868 7474 7073 3a2f 2f61 6c62 756d  r](https://album
+000033c0: 656e 7461 7469 6f6e 732e 6169 2f64 6f63  entations.ai/doc
+000033d0: 732f 6170 695f 7265 6665 7265 6e63 652f  s/api_reference/
+000033e0: 6175 676d 656e 7461 7469 6f6e 732f 626c  augmentations/bl
+000033f0: 7572 2f74 7261 6e73 666f 726d 732f 2361  ur/transforms/#a
+00003400: 6c62 756d 656e 7461 7469 6f6e 732e 6175  lbumentations.au
+00003410: 676d 656e 7461 7469 6f6e 732e 626c 7572  gmentations.blur
+00003420: 2e74 7261 6e73 666f 726d 732e 4761 7573  .transforms.Gaus
+00003430: 7369 616e 426c 7572 290a 2d20 5b47 6c61  sianBlur).- [Gla
+00003440: 7373 426c 7572 5d28 6874 7470 733a 2f2f  ssBlur](https://
+00003450: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
+00003460: 692f 646f 6373 2f61 7069 5f72 6566 6572  i/docs/api_refer
+00003470: 656e 6365 2f61 7567 6d65 6e74 6174 696f  ence/augmentatio
+00003480: 6e73 2f62 6c75 722f 7472 616e 7366 6f72  ns/blur/transfor
+00003490: 6d73 2f23 616c 6275 6d65 6e74 6174 696f  ms/#albumentatio
+000034a0: 6e73 2e61 7567 6d65 6e74 6174 696f 6e73  ns.augmentations
+000034b0: 2e62 6c75 722e 7472 616e 7366 6f72 6d73  .blur.transforms
+000034c0: 2e47 6c61 7373 426c 7572 290a 2d20 5b48  .GlassBlur).- [H
+000034d0: 6973 746f 6772 616d 4d61 7463 6869 6e67  istogramMatching
+000034e0: 5d28 6874 7470 733a 2f2f 616c 6275 6d65  ](https://albume
+000034f0: 6e74 6174 696f 6e73 2e61 692f 646f 6373  ntations.ai/docs
+00003500: 2f61 7069 5f72 6566 6572 656e 6365 2f61  /api_reference/a
+00003510: 7567 6d65 6e74 6174 696f 6e73 2f64 6f6d  ugmentations/dom
+00003520: 6169 6e5f 6164 6170 7461 7469 6f6e 2f23  ain_adaptation/#
+00003530: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
+00003540: 7567 6d65 6e74 6174 696f 6e73 2e64 6f6d  ugmentations.dom
+00003550: 6169 6e5f 6164 6170 7461 7469 6f6e 2e48  ain_adaptation.H
+00003560: 6973 746f 6772 616d 4d61 7463 6869 6e67  istogramMatching
+00003570: 290a 2d20 5b48 7565 5361 7475 7261 7469  ).- [HueSaturati
+00003580: 6f6e 5661 6c75 655d 2868 7474 7073 3a2f  onValue](https:/
 00003590: 2f61 6c62 756d 656e 7461 7469 6f6e 732e  /albumentations.
 000035a0: 6169 2f64 6f63 732f 6170 695f 7265 6665  ai/docs/api_refe
 000035b0: 7265 6e63 652f 6175 676d 656e 7461 7469  rence/augmentati
 000035c0: 6f6e 732f 7472 616e 7366 6f72 6d73 2f23  ons/transforms/#
 000035d0: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
 000035e0: 7567 6d65 6e74 6174 696f 6e73 2e74 7261  ugmentations.tra
-000035f0: 6e73 666f 726d 732e 436f 6c6f 724a 6974  nsforms.ColorJit
-00003600: 7465 7229 0a2d 205b 4465 666f 6375 735d  ter).- [Defocus]
-00003610: 2868 7474 7073 3a2f 2f61 6c62 756d 656e  (https://albumen
-00003620: 7461 7469 6f6e 732e 6169 2f64 6f63 732f  tations.ai/docs/
-00003630: 6170 695f 7265 6665 7265 6e63 652f 6175  api_reference/au
-00003640: 676d 656e 7461 7469 6f6e 732f 626c 7572  gmentations/blur
-00003650: 2f74 7261 6e73 666f 726d 732f 2361 6c62  /transforms/#alb
-00003660: 756d 656e 7461 7469 6f6e 732e 6175 676d  umentations.augm
-00003670: 656e 7461 7469 6f6e 732e 626c 7572 2e74  entations.blur.t
-00003680: 7261 6e73 666f 726d 732e 4465 666f 6375  ransforms.Defocu
-00003690: 7329 0a2d 205b 446f 776e 7363 616c 655d  s).- [Downscale]
-000036a0: 2868 7474 7073 3a2f 2f61 6c62 756d 656e  (https://albumen
-000036b0: 7461 7469 6f6e 732e 6169 2f64 6f63 732f  tations.ai/docs/
-000036c0: 6170 695f 7265 6665 7265 6e63 652f 6175  api_reference/au
-000036d0: 676d 656e 7461 7469 6f6e 732f 7472 616e  gmentations/tran
-000036e0: 7366 6f72 6d73 2f23 616c 6275 6d65 6e74  sforms/#albument
-000036f0: 6174 696f 6e73 2e61 7567 6d65 6e74 6174  ations.augmentat
-00003700: 696f 6e73 2e74 7261 6e73 666f 726d 732e  ions.transforms.
-00003710: 446f 776e 7363 616c 6529 0a2d 205b 456d  Downscale).- [Em
-00003720: 626f 7373 5d28 6874 7470 733a 2f2f 616c  boss](https://al
-00003730: 6275 6d65 6e74 6174 696f 6e73 2e61 692f  bumentations.ai/
-00003740: 646f 6373 2f61 7069 5f72 6566 6572 656e  docs/api_referen
-00003750: 6365 2f61 7567 6d65 6e74 6174 696f 6e73  ce/augmentations
-00003760: 2f74 7261 6e73 666f 726d 732f 2361 6c62  /transforms/#alb
-00003770: 756d 656e 7461 7469 6f6e 732e 6175 676d  umentations.augm
-00003780: 656e 7461 7469 6f6e 732e 7472 616e 7366  entations.transf
-00003790: 6f72 6d73 2e45 6d62 6f73 7329 0a2d 205b  orms.Emboss).- [
-000037a0: 4571 7561 6c69 7a65 5d28 6874 7470 733a  Equalize](https:
-000037b0: 2f2f 616c 6275 6d65 6e74 6174 696f 6e73  //albumentations
-000037c0: 2e61 692f 646f 6373 2f61 7069 5f72 6566  .ai/docs/api_ref
-000037d0: 6572 656e 6365 2f61 7567 6d65 6e74 6174  erence/augmentat
-000037e0: 696f 6e73 2f74 7261 6e73 666f 726d 732f  ions/transforms/
-000037f0: 2361 6c62 756d 656e 7461 7469 6f6e 732e  #albumentations.
-00003800: 6175 676d 656e 7461 7469 6f6e 732e 7472  augmentations.tr
-00003810: 616e 7366 6f72 6d73 2e45 7175 616c 697a  ansforms.Equaliz
-00003820: 6529 0a2d 205b 4644 415d 2868 7474 7073  e).- [FDA](https
-00003830: 3a2f 2f61 6c62 756d 656e 7461 7469 6f6e  ://albumentation
-00003840: 732e 6169 2f64 6f63 732f 6170 695f 7265  s.ai/docs/api_re
-00003850: 6665 7265 6e63 652f 6175 676d 656e 7461  ference/augmenta
-00003860: 7469 6f6e 732f 646f 6d61 696e 5f61 6461  tions/domain_ada
-00003870: 7074 6174 696f 6e2f 2361 6c62 756d 656e  ptation/#albumen
-00003880: 7461 7469 6f6e 732e 6175 676d 656e 7461  tations.augmenta
-00003890: 7469 6f6e 732e 646f 6d61 696e 5f61 6461  tions.domain_ada
-000038a0: 7074 6174 696f 6e2e 4644 4129 0a2d 205b  ptation.FDA).- [
-000038b0: 4661 6e63 7950 4341 5d28 6874 7470 733a  FancyPCA](https:
-000038c0: 2f2f 616c 6275 6d65 6e74 6174 696f 6e73  //albumentations
-000038d0: 2e61 692f 646f 6373 2f61 7069 5f72 6566  .ai/docs/api_ref
-000038e0: 6572 656e 6365 2f61 7567 6d65 6e74 6174  erence/augmentat
-000038f0: 696f 6e73 2f74 7261 6e73 666f 726d 732f  ions/transforms/
-00003900: 2361 6c62 756d 656e 7461 7469 6f6e 732e  #albumentations.
-00003910: 6175 676d 656e 7461 7469 6f6e 732e 7472  augmentations.tr
-00003920: 616e 7366 6f72 6d73 2e46 616e 6379 5043  ansforms.FancyPC
-00003930: 4129 0a2d 205b 4672 6f6d 466c 6f61 745d  A).- [FromFloat]
-00003940: 2868 7474 7073 3a2f 2f61 6c62 756d 656e  (https://albumen
-00003950: 7461 7469 6f6e 732e 6169 2f64 6f63 732f  tations.ai/docs/
-00003960: 6170 695f 7265 6665 7265 6e63 652f 6175  api_reference/au
-00003970: 676d 656e 7461 7469 6f6e 732f 7472 616e  gmentations/tran
-00003980: 7366 6f72 6d73 2f23 616c 6275 6d65 6e74  sforms/#albument
-00003990: 6174 696f 6e73 2e61 7567 6d65 6e74 6174  ations.augmentat
-000039a0: 696f 6e73 2e74 7261 6e73 666f 726d 732e  ions.transforms.
-000039b0: 4672 6f6d 466c 6f61 7429 0a2d 205b 4761  FromFloat).- [Ga
-000039c0: 7573 734e 6f69 7365 5d28 6874 7470 733a  ussNoise](https:
-000039d0: 2f2f 616c 6275 6d65 6e74 6174 696f 6e73  //albumentations
-000039e0: 2e61 692f 646f 6373 2f61 7069 5f72 6566  .ai/docs/api_ref
-000039f0: 6572 656e 6365 2f61 7567 6d65 6e74 6174  erence/augmentat
-00003a00: 696f 6e73 2f74 7261 6e73 666f 726d 732f  ions/transforms/
-00003a10: 2361 6c62 756d 656e 7461 7469 6f6e 732e  #albumentations.
-00003a20: 6175 676d 656e 7461 7469 6f6e 732e 7472  augmentations.tr
-00003a30: 616e 7366 6f72 6d73 2e47 6175 7373 4e6f  ansforms.GaussNo
-00003a40: 6973 6529 0a2d 205b 4761 7573 7369 616e  ise).- [Gaussian
-00003a50: 426c 7572 5d28 6874 7470 733a 2f2f 616c  Blur](https://al
-00003a60: 6275 6d65 6e74 6174 696f 6e73 2e61 692f  bumentations.ai/
-00003a70: 646f 6373 2f61 7069 5f72 6566 6572 656e  docs/api_referen
-00003a80: 6365 2f61 7567 6d65 6e74 6174 696f 6e73  ce/augmentations
-00003a90: 2f62 6c75 722f 7472 616e 7366 6f72 6d73  /blur/transforms
-00003aa0: 2f23 616c 6275 6d65 6e74 6174 696f 6e73  /#albumentations
-00003ab0: 2e61 7567 6d65 6e74 6174 696f 6e73 2e62  .augmentations.b
-00003ac0: 6c75 722e 7472 616e 7366 6f72 6d73 2e47  lur.transforms.G
-00003ad0: 6175 7373 6961 6e42 6c75 7229 0a2d 205b  aussianBlur).- [
-00003ae0: 476c 6173 7342 6c75 725d 2868 7474 7073  GlassBlur](https
-00003af0: 3a2f 2f61 6c62 756d 656e 7461 7469 6f6e  ://albumentation
-00003b00: 732e 6169 2f64 6f63 732f 6170 695f 7265  s.ai/docs/api_re
-00003b10: 6665 7265 6e63 652f 6175 676d 656e 7461  ference/augmenta
-00003b20: 7469 6f6e 732f 626c 7572 2f74 7261 6e73  tions/blur/trans
-00003b30: 666f 726d 732f 2361 6c62 756d 656e 7461  forms/#albumenta
-00003b40: 7469 6f6e 732e 6175 676d 656e 7461 7469  tions.augmentati
-00003b50: 6f6e 732e 626c 7572 2e74 7261 6e73 666f  ons.blur.transfo
-00003b60: 726d 732e 476c 6173 7342 6c75 7229 0a2d  rms.GlassBlur).-
-00003b70: 205b 4869 7374 6f67 7261 6d4d 6174 6368   [HistogramMatch
-00003b80: 696e 675d 2868 7474 7073 3a2f 2f61 6c62  ing](https://alb
-00003b90: 756d 656e 7461 7469 6f6e 732e 6169 2f64  umentations.ai/d
-00003ba0: 6f63 732f 6170 695f 7265 6665 7265 6e63  ocs/api_referenc
-00003bb0: 652f 6175 676d 656e 7461 7469 6f6e 732f  e/augmentations/
-00003bc0: 646f 6d61 696e 5f61 6461 7074 6174 696f  domain_adaptatio
-00003bd0: 6e2f 2361 6c62 756d 656e 7461 7469 6f6e  n/#albumentation
-00003be0: 732e 6175 676d 656e 7461 7469 6f6e 732e  s.augmentations.
-00003bf0: 646f 6d61 696e 5f61 6461 7074 6174 696f  domain_adaptatio
-00003c00: 6e2e 4869 7374 6f67 7261 6d4d 6174 6368  n.HistogramMatch
-00003c10: 696e 6729 0a2d 205b 4875 6553 6174 7572  ing).- [HueSatur
-00003c20: 6174 696f 6e56 616c 7565 5d28 6874 7470  ationValue](http
-00003c30: 733a 2f2f 616c 6275 6d65 6e74 6174 696f  s://albumentatio
-00003c40: 6e73 2e61 692f 646f 6373 2f61 7069 5f72  ns.ai/docs/api_r
-00003c50: 6566 6572 656e 6365 2f61 7567 6d65 6e74  eference/augment
-00003c60: 6174 696f 6e73 2f74 7261 6e73 666f 726d  ations/transform
-00003c70: 732f 2361 6c62 756d 656e 7461 7469 6f6e  s/#albumentation
-00003c80: 732e 6175 676d 656e 7461 7469 6f6e 732e  s.augmentations.
-00003c90: 7472 616e 7366 6f72 6d73 2e48 7565 5361  transforms.HueSa
-00003ca0: 7475 7261 7469 6f6e 5661 6c75 6529 0a2d  turationValue).-
-00003cb0: 205b 4953 4f4e 6f69 7365 5d28 6874 7470   [ISONoise](http
-00003cc0: 733a 2f2f 616c 6275 6d65 6e74 6174 696f  s://albumentatio
-00003cd0: 6e73 2e61 692f 646f 6373 2f61 7069 5f72  ns.ai/docs/api_r
-00003ce0: 6566 6572 656e 6365 2f61 7567 6d65 6e74  eference/augment
-00003cf0: 6174 696f 6e73 2f74 7261 6e73 666f 726d  ations/transform
-00003d00: 732f 2361 6c62 756d 656e 7461 7469 6f6e  s/#albumentation
-00003d10: 732e 6175 676d 656e 7461 7469 6f6e 732e  s.augmentations.
-00003d20: 7472 616e 7366 6f72 6d73 2e49 534f 4e6f  transforms.ISONo
-00003d30: 6973 6529 0a2d 205b 496d 6167 6543 6f6d  ise).- [ImageCom
-00003d40: 7072 6573 7369 6f6e 5d28 6874 7470 733a  pression](https:
-00003d50: 2f2f 616c 6275 6d65 6e74 6174 696f 6e73  //albumentations
-00003d60: 2e61 692f 646f 6373 2f61 7069 5f72 6566  .ai/docs/api_ref
-00003d70: 6572 656e 6365 2f61 7567 6d65 6e74 6174  erence/augmentat
-00003d80: 696f 6e73 2f74 7261 6e73 666f 726d 732f  ions/transforms/
-00003d90: 2361 6c62 756d 656e 7461 7469 6f6e 732e  #albumentations.
-00003da0: 6175 676d 656e 7461 7469 6f6e 732e 7472  augmentations.tr
-00003db0: 616e 7366 6f72 6d73 2e49 6d61 6765 436f  ansforms.ImageCo
-00003dc0: 6d70 7265 7373 696f 6e29 0a2d 205b 496e  mpression).- [In
-00003dd0: 7665 7274 496d 675d 2868 7474 7073 3a2f  vertImg](https:/
-00003de0: 2f61 6c62 756d 656e 7461 7469 6f6e 732e  /albumentations.
-00003df0: 6169 2f64 6f63 732f 6170 695f 7265 6665  ai/docs/api_refe
-00003e00: 7265 6e63 652f 6175 676d 656e 7461 7469  rence/augmentati
-00003e10: 6f6e 732f 7472 616e 7366 6f72 6d73 2f23  ons/transforms/#
-00003e20: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
-00003e30: 7567 6d65 6e74 6174 696f 6e73 2e74 7261  ugmentations.tra
-00003e40: 6e73 666f 726d 732e 496e 7665 7274 496d  nsforms.InvertIm
-00003e50: 6729 0a2d 205b 4d65 6469 616e 426c 7572  g).- [MedianBlur
-00003e60: 5d28 6874 7470 733a 2f2f 616c 6275 6d65  ](https://albume
-00003e70: 6e74 6174 696f 6e73 2e61 692f 646f 6373  ntations.ai/docs
-00003e80: 2f61 7069 5f72 6566 6572 656e 6365 2f61  /api_reference/a
-00003e90: 7567 6d65 6e74 6174 696f 6e73 2f62 6c75  ugmentations/blu
-00003ea0: 722f 7472 616e 7366 6f72 6d73 2f23 616c  r/transforms/#al
-00003eb0: 6275 6d65 6e74 6174 696f 6e73 2e61 7567  bumentations.aug
-00003ec0: 6d65 6e74 6174 696f 6e73 2e62 6c75 722e  mentations.blur.
-00003ed0: 7472 616e 7366 6f72 6d73 2e4d 6564 6961  transforms.Media
-00003ee0: 6e42 6c75 7229 0a2d 205b 4d6f 7469 6f6e  nBlur).- [Motion
-00003ef0: 426c 7572 5d28 6874 7470 733a 2f2f 616c  Blur](https://al
-00003f00: 6275 6d65 6e74 6174 696f 6e73 2e61 692f  bumentations.ai/
-00003f10: 646f 6373 2f61 7069 5f72 6566 6572 656e  docs/api_referen
-00003f20: 6365 2f61 7567 6d65 6e74 6174 696f 6e73  ce/augmentations
-00003f30: 2f62 6c75 722f 7472 616e 7366 6f72 6d73  /blur/transforms
-00003f40: 2f23 616c 6275 6d65 6e74 6174 696f 6e73  /#albumentations
-00003f50: 2e61 7567 6d65 6e74 6174 696f 6e73 2e62  .augmentations.b
-00003f60: 6c75 722e 7472 616e 7366 6f72 6d73 2e4d  lur.transforms.M
-00003f70: 6f74 696f 6e42 6c75 7229 0a2d 205b 4d75  otionBlur).- [Mu
-00003f80: 6c74 6970 6c69 6361 7469 7665 4e6f 6973  ltiplicativeNois
-00003f90: 655d 2868 7474 7073 3a2f 2f61 6c62 756d  e](https://album
-00003fa0: 656e 7461 7469 6f6e 732e 6169 2f64 6f63  entations.ai/doc
-00003fb0: 732f 6170 695f 7265 6665 7265 6e63 652f  s/api_reference/
-00003fc0: 6175 676d 656e 7461 7469 6f6e 732f 7472  augmentations/tr
-00003fd0: 616e 7366 6f72 6d73 2f23 616c 6275 6d65  ansforms/#albume
-00003fe0: 6e74 6174 696f 6e73 2e61 7567 6d65 6e74  ntations.augment
-00003ff0: 6174 696f 6e73 2e74 7261 6e73 666f 726d  ations.transform
-00004000: 732e 4d75 6c74 6970 6c69 6361 7469 7665  s.Multiplicative
-00004010: 4e6f 6973 6529 0a2d 205b 4e6f 726d 616c  Noise).- [Normal
-00004020: 697a 655d 2868 7474 7073 3a2f 2f61 6c62  ize](https://alb
-00004030: 756d 656e 7461 7469 6f6e 732e 6169 2f64  umentations.ai/d
-00004040: 6f63 732f 6170 695f 7265 6665 7265 6e63  ocs/api_referenc
-00004050: 652f 6175 676d 656e 7461 7469 6f6e 732f  e/augmentations/
-00004060: 7472 616e 7366 6f72 6d73 2f23 616c 6275  transforms/#albu
-00004070: 6d65 6e74 6174 696f 6e73 2e61 7567 6d65  mentations.augme
-00004080: 6e74 6174 696f 6e73 2e74 7261 6e73 666f  ntations.transfo
-00004090: 726d 732e 4e6f 726d 616c 697a 6529 0a2d  rms.Normalize).-
-000040a0: 205b 5069 7865 6c44 6973 7472 6962 7574   [PixelDistribut
-000040b0: 696f 6e41 6461 7074 6174 696f 6e5d 2868  ionAdaptation](h
-000040c0: 7474 7073 3a2f 2f61 6c62 756d 656e 7461  ttps://albumenta
-000040d0: 7469 6f6e 732e 6169 2f64 6f63 732f 6170  tions.ai/docs/ap
-000040e0: 695f 7265 6665 7265 6e63 652f 6175 676d  i_reference/augm
-000040f0: 656e 7461 7469 6f6e 732f 646f 6d61 696e  entations/domain
-00004100: 5f61 6461 7074 6174 696f 6e2f 2361 6c62  _adaptation/#alb
-00004110: 756d 656e 7461 7469 6f6e 732e 6175 676d  umentations.augm
-00004120: 656e 7461 7469 6f6e 732e 646f 6d61 696e  entations.domain
-00004130: 5f61 6461 7074 6174 696f 6e2e 5069 7865  _adaptation.Pixe
-00004140: 6c44 6973 7472 6962 7574 696f 6e41 6461  lDistributionAda
-00004150: 7074 6174 696f 6e29 0a2d 205b 506f 7374  ptation).- [Post
-00004160: 6572 697a 655d 2868 7474 7073 3a2f 2f61  erize](https://a
-00004170: 6c62 756d 656e 7461 7469 6f6e 732e 6169  lbumentations.ai
-00004180: 2f64 6f63 732f 6170 695f 7265 6665 7265  /docs/api_refere
-00004190: 6e63 652f 6175 676d 656e 7461 7469 6f6e  nce/augmentation
-000041a0: 732f 7472 616e 7366 6f72 6d73 2f23 616c  s/transforms/#al
-000041b0: 6275 6d65 6e74 6174 696f 6e73 2e61 7567  bumentations.aug
-000041c0: 6d65 6e74 6174 696f 6e73 2e74 7261 6e73  mentations.trans
-000041d0: 666f 726d 732e 506f 7374 6572 697a 6529  forms.Posterize)
-000041e0: 0a2d 205b 5247 4253 6869 6674 5d28 6874  .- [RGBShift](ht
-000041f0: 7470 733a 2f2f 616c 6275 6d65 6e74 6174  tps://albumentat
-00004200: 696f 6e73 2e61 692f 646f 6373 2f61 7069  ions.ai/docs/api
-00004210: 5f72 6566 6572 656e 6365 2f61 7567 6d65  _reference/augme
-00004220: 6e74 6174 696f 6e73 2f74 7261 6e73 666f  ntations/transfo
-00004230: 726d 732f 2361 6c62 756d 656e 7461 7469  rms/#albumentati
-00004240: 6f6e 732e 6175 676d 656e 7461 7469 6f6e  ons.augmentation
-00004250: 732e 7472 616e 7366 6f72 6d73 2e52 4742  s.transforms.RGB
-00004260: 5368 6966 7429 0a2d 205b 5261 6e64 6f6d  Shift).- [Random
-00004270: 4272 6967 6874 6e65 7373 436f 6e74 7261  BrightnessContra
-00004280: 7374 5d28 6874 7470 733a 2f2f 616c 6275  st](https://albu
-00004290: 6d65 6e74 6174 696f 6e73 2e61 692f 646f  mentations.ai/do
-000042a0: 6373 2f61 7069 5f72 6566 6572 656e 6365  cs/api_reference
-000042b0: 2f61 7567 6d65 6e74 6174 696f 6e73 2f74  /augmentations/t
-000042c0: 7261 6e73 666f 726d 732f 2361 6c62 756d  ransforms/#album
-000042d0: 656e 7461 7469 6f6e 732e 6175 676d 656e  entations.augmen
-000042e0: 7461 7469 6f6e 732e 7472 616e 7366 6f72  tations.transfor
-000042f0: 6d73 2e52 616e 646f 6d42 7269 6768 746e  ms.RandomBrightn
-00004300: 6573 7343 6f6e 7472 6173 7429 0a2d 205b  essContrast).- [
-00004310: 5261 6e64 6f6d 466f 675d 2868 7474 7073  RandomFog](https
-00004320: 3a2f 2f61 6c62 756d 656e 7461 7469 6f6e  ://albumentation
-00004330: 732e 6169 2f64 6f63 732f 6170 695f 7265  s.ai/docs/api_re
-00004340: 6665 7265 6e63 652f 6175 676d 656e 7461  ference/augmenta
-00004350: 7469 6f6e 732f 7472 616e 7366 6f72 6d73  tions/transforms
-00004360: 2f23 616c 6275 6d65 6e74 6174 696f 6e73  /#albumentations
-00004370: 2e61 7567 6d65 6e74 6174 696f 6e73 2e74  .augmentations.t
-00004380: 7261 6e73 666f 726d 732e 5261 6e64 6f6d  ransforms.Random
-00004390: 466f 6729 0a2d 205b 5261 6e64 6f6d 4761  Fog).- [RandomGa
-000043a0: 6d6d 615d 2868 7474 7073 3a2f 2f61 6c62  mma](https://alb
-000043b0: 756d 656e 7461 7469 6f6e 732e 6169 2f64  umentations.ai/d
-000043c0: 6f63 732f 6170 695f 7265 6665 7265 6e63  ocs/api_referenc
-000043d0: 652f 6175 676d 656e 7461 7469 6f6e 732f  e/augmentations/
-000043e0: 7472 616e 7366 6f72 6d73 2f23 616c 6275  transforms/#albu
-000043f0: 6d65 6e74 6174 696f 6e73 2e61 7567 6d65  mentations.augme
-00004400: 6e74 6174 696f 6e73 2e74 7261 6e73 666f  ntations.transfo
-00004410: 726d 732e 5261 6e64 6f6d 4761 6d6d 6129  rms.RandomGamma)
-00004420: 0a2d 205b 5261 6e64 6f6d 4772 6176 656c  .- [RandomGravel
-00004430: 5d28 6874 7470 733a 2f2f 616c 6275 6d65  ](https://albume
-00004440: 6e74 6174 696f 6e73 2e61 692f 646f 6373  ntations.ai/docs
-00004450: 2f61 7069 5f72 6566 6572 656e 6365 2f61  /api_reference/a
-00004460: 7567 6d65 6e74 6174 696f 6e73 2f74 7261  ugmentations/tra
-00004470: 6e73 666f 726d 732f 2361 6c62 756d 656e  nsforms/#albumen
-00004480: 7461 7469 6f6e 732e 6175 676d 656e 7461  tations.augmenta
-00004490: 7469 6f6e 732e 7472 616e 7366 6f72 6d73  tions.transforms
-000044a0: 2e52 616e 646f 6d47 7261 7665 6c29 0a2d  .RandomGravel).-
-000044b0: 205b 5261 6e64 6f6d 5261 696e 5d28 6874   [RandomRain](ht
-000044c0: 7470 733a 2f2f 616c 6275 6d65 6e74 6174  tps://albumentat
-000044d0: 696f 6e73 2e61 692f 646f 6373 2f61 7069  ions.ai/docs/api
-000044e0: 5f72 6566 6572 656e 6365 2f61 7567 6d65  _reference/augme
-000044f0: 6e74 6174 696f 6e73 2f74 7261 6e73 666f  ntations/transfo
-00004500: 726d 732f 2361 6c62 756d 656e 7461 7469  rms/#albumentati
-00004510: 6f6e 732e 6175 676d 656e 7461 7469 6f6e  ons.augmentation
-00004520: 732e 7472 616e 7366 6f72 6d73 2e52 616e  s.transforms.Ran
-00004530: 646f 6d52 6169 6e29 0a2d 205b 5261 6e64  domRain).- [Rand
-00004540: 6f6d 5368 6164 6f77 5d28 6874 7470 733a  omShadow](https:
-00004550: 2f2f 616c 6275 6d65 6e74 6174 696f 6e73  //albumentations
-00004560: 2e61 692f 646f 6373 2f61 7069 5f72 6566  .ai/docs/api_ref
-00004570: 6572 656e 6365 2f61 7567 6d65 6e74 6174  erence/augmentat
-00004580: 696f 6e73 2f74 7261 6e73 666f 726d 732f  ions/transforms/
-00004590: 2361 6c62 756d 656e 7461 7469 6f6e 732e  #albumentations.
-000045a0: 6175 676d 656e 7461 7469 6f6e 732e 7472  augmentations.tr
-000045b0: 616e 7366 6f72 6d73 2e52 616e 646f 6d53  ansforms.RandomS
-000045c0: 6861 646f 7729 0a2d 205b 5261 6e64 6f6d  hadow).- [Random
-000045d0: 536e 6f77 5d28 6874 7470 733a 2f2f 616c  Snow](https://al
-000045e0: 6275 6d65 6e74 6174 696f 6e73 2e61 692f  bumentations.ai/
-000045f0: 646f 6373 2f61 7069 5f72 6566 6572 656e  docs/api_referen
-00004600: 6365 2f61 7567 6d65 6e74 6174 696f 6e73  ce/augmentations
-00004610: 2f74 7261 6e73 666f 726d 732f 2361 6c62  /transforms/#alb
-00004620: 756d 656e 7461 7469 6f6e 732e 6175 676d  umentations.augm
-00004630: 656e 7461 7469 6f6e 732e 7472 616e 7366  entations.transf
-00004640: 6f72 6d73 2e52 616e 646f 6d53 6e6f 7729  orms.RandomSnow)
-00004650: 0a2d 205b 5261 6e64 6f6d 5375 6e46 6c61  .- [RandomSunFla
-00004660: 7265 5d28 6874 7470 733a 2f2f 616c 6275  re](https://albu
-00004670: 6d65 6e74 6174 696f 6e73 2e61 692f 646f  mentations.ai/do
-00004680: 6373 2f61 7069 5f72 6566 6572 656e 6365  cs/api_reference
-00004690: 2f61 7567 6d65 6e74 6174 696f 6e73 2f74  /augmentations/t
-000046a0: 7261 6e73 666f 726d 732f 2361 6c62 756d  ransforms/#album
-000046b0: 656e 7461 7469 6f6e 732e 6175 676d 656e  entations.augmen
-000046c0: 7461 7469 6f6e 732e 7472 616e 7366 6f72  tations.transfor
-000046d0: 6d73 2e52 616e 646f 6d53 756e 466c 6172  ms.RandomSunFlar
-000046e0: 6529 0a2d 205b 5261 6e64 6f6d 546f 6e65  e).- [RandomTone
-000046f0: 4375 7276 655d 2868 7474 7073 3a2f 2f61  Curve](https://a
-00004700: 6c62 756d 656e 7461 7469 6f6e 732e 6169  lbumentations.ai
-00004710: 2f64 6f63 732f 6170 695f 7265 6665 7265  /docs/api_refere
-00004720: 6e63 652f 6175 676d 656e 7461 7469 6f6e  nce/augmentation
-00004730: 732f 7472 616e 7366 6f72 6d73 2f23 616c  s/transforms/#al
-00004740: 6275 6d65 6e74 6174 696f 6e73 2e61 7567  bumentations.aug
-00004750: 6d65 6e74 6174 696f 6e73 2e74 7261 6e73  mentations.trans
-00004760: 666f 726d 732e 5261 6e64 6f6d 546f 6e65  forms.RandomTone
-00004770: 4375 7276 6529 0a2d 205b 5269 6e67 696e  Curve).- [Ringin
-00004780: 674f 7665 7273 686f 6f74 5d28 6874 7470  gOvershoot](http
-00004790: 733a 2f2f 616c 6275 6d65 6e74 6174 696f  s://albumentatio
-000047a0: 6e73 2e61 692f 646f 6373 2f61 7069 5f72  ns.ai/docs/api_r
-000047b0: 6566 6572 656e 6365 2f61 7567 6d65 6e74  eference/augment
-000047c0: 6174 696f 6e73 2f74 7261 6e73 666f 726d  ations/transform
-000047d0: 732f 2361 6c62 756d 656e 7461 7469 6f6e  s/#albumentation
-000047e0: 732e 6175 676d 656e 7461 7469 6f6e 732e  s.augmentations.
-000047f0: 7472 616e 7366 6f72 6d73 2e52 696e 6769  transforms.Ringi
-00004800: 6e67 4f76 6572 7368 6f6f 7429 0a2d 205b  ngOvershoot).- [
-00004810: 5368 6172 7065 6e5d 2868 7474 7073 3a2f  Sharpen](https:/
-00004820: 2f61 6c62 756d 656e 7461 7469 6f6e 732e  /albumentations.
-00004830: 6169 2f64 6f63 732f 6170 695f 7265 6665  ai/docs/api_refe
-00004840: 7265 6e63 652f 6175 676d 656e 7461 7469  rence/augmentati
-00004850: 6f6e 732f 7472 616e 7366 6f72 6d73 2f23  ons/transforms/#
-00004860: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
-00004870: 7567 6d65 6e74 6174 696f 6e73 2e74 7261  ugmentations.tra
-00004880: 6e73 666f 726d 732e 5368 6172 7065 6e29  nsforms.Sharpen)
-00004890: 0a2d 205b 536f 6c61 7269 7a65 5d28 6874  .- [Solarize](ht
-000048a0: 7470 733a 2f2f 616c 6275 6d65 6e74 6174  tps://albumentat
-000048b0: 696f 6e73 2e61 692f 646f 6373 2f61 7069  ions.ai/docs/api
-000048c0: 5f72 6566 6572 656e 6365 2f61 7567 6d65  _reference/augme
-000048d0: 6e74 6174 696f 6e73 2f74 7261 6e73 666f  ntations/transfo
-000048e0: 726d 732f 2361 6c62 756d 656e 7461 7469  rms/#albumentati
-000048f0: 6f6e 732e 6175 676d 656e 7461 7469 6f6e  ons.augmentation
-00004900: 732e 7472 616e 7366 6f72 6d73 2e53 6f6c  s.transforms.Sol
-00004910: 6172 697a 6529 0a2d 205b 5370 6174 7465  arize).- [Spatte
-00004920: 725d 2868 7474 7073 3a2f 2f61 6c62 756d  r](https://album
-00004930: 656e 7461 7469 6f6e 732e 6169 2f64 6f63  entations.ai/doc
-00004940: 732f 6170 695f 7265 6665 7265 6e63 652f  s/api_reference/
-00004950: 6175 676d 656e 7461 7469 6f6e 732f 7472  augmentations/tr
-00004960: 616e 7366 6f72 6d73 2f23 616c 6275 6d65  ansforms/#albume
-00004970: 6e74 6174 696f 6e73 2e61 7567 6d65 6e74  ntations.augment
-00004980: 6174 696f 6e73 2e74 7261 6e73 666f 726d  ations.transform
-00004990: 732e 5370 6174 7465 7229 0a2d 205b 5375  s.Spatter).- [Su
-000049a0: 7065 7270 6978 656c 735d 2868 7474 7073  perpixels](https
-000049b0: 3a2f 2f61 6c62 756d 656e 7461 7469 6f6e  ://albumentation
-000049c0: 732e 6169 2f64 6f63 732f 6170 695f 7265  s.ai/docs/api_re
-000049d0: 6665 7265 6e63 652f 6175 676d 656e 7461  ference/augmenta
-000049e0: 7469 6f6e 732f 7472 616e 7366 6f72 6d73  tions/transforms
-000049f0: 2f23 616c 6275 6d65 6e74 6174 696f 6e73  /#albumentations
-00004a00: 2e61 7567 6d65 6e74 6174 696f 6e73 2e74  .augmentations.t
-00004a10: 7261 6e73 666f 726d 732e 5375 7065 7270  ransforms.Superp
-00004a20: 6978 656c 7329 0a2d 205b 5465 6d70 6c61  ixels).- [Templa
-00004a30: 7465 5472 616e 7366 6f72 6d5d 2868 7474  teTransform](htt
-00004a40: 7073 3a2f 2f61 6c62 756d 656e 7461 7469  ps://albumentati
-00004a50: 6f6e 732e 6169 2f64 6f63 732f 6170 695f  ons.ai/docs/api_
-00004a60: 7265 6665 7265 6e63 652f 6175 676d 656e  reference/augmen
-00004a70: 7461 7469 6f6e 732f 7472 616e 7366 6f72  tations/transfor
-00004a80: 6d73 2f23 616c 6275 6d65 6e74 6174 696f  ms/#albumentatio
-00004a90: 6e73 2e61 7567 6d65 6e74 6174 696f 6e73  ns.augmentations
-00004aa0: 2e74 7261 6e73 666f 726d 732e 5465 6d70  .transforms.Temp
-00004ab0: 6c61 7465 5472 616e 7366 6f72 6d29 0a2d  lateTransform).-
-00004ac0: 205b 546f 466c 6f61 745d 2868 7474 7073   [ToFloat](https
-00004ad0: 3a2f 2f61 6c62 756d 656e 7461 7469 6f6e  ://albumentation
-00004ae0: 732e 6169 2f64 6f63 732f 6170 695f 7265  s.ai/docs/api_re
-00004af0: 6665 7265 6e63 652f 6175 676d 656e 7461  ference/augmenta
-00004b00: 7469 6f6e 732f 7472 616e 7366 6f72 6d73  tions/transforms
-00004b10: 2f23 616c 6275 6d65 6e74 6174 696f 6e73  /#albumentations
-00004b20: 2e61 7567 6d65 6e74 6174 696f 6e73 2e74  .augmentations.t
-00004b30: 7261 6e73 666f 726d 732e 546f 466c 6f61  ransforms.ToFloa
-00004b40: 7429 0a2d 205b 546f 4772 6179 5d28 6874  t).- [ToGray](ht
-00004b50: 7470 733a 2f2f 616c 6275 6d65 6e74 6174  tps://albumentat
-00004b60: 696f 6e73 2e61 692f 646f 6373 2f61 7069  ions.ai/docs/api
-00004b70: 5f72 6566 6572 656e 6365 2f61 7567 6d65  _reference/augme
-00004b80: 6e74 6174 696f 6e73 2f74 7261 6e73 666f  ntations/transfo
-00004b90: 726d 732f 2361 6c62 756d 656e 7461 7469  rms/#albumentati
-00004ba0: 6f6e 732e 6175 676d 656e 7461 7469 6f6e  ons.augmentation
-00004bb0: 732e 7472 616e 7366 6f72 6d73 2e54 6f47  s.transforms.ToG
-00004bc0: 7261 7929 0a2d 205b 546f 5247 425d 2868  ray).- [ToRGB](h
-00004bd0: 7474 7073 3a2f 2f61 6c62 756d 656e 7461  ttps://albumenta
-00004be0: 7469 6f6e 732e 6169 2f64 6f63 732f 6170  tions.ai/docs/ap
-00004bf0: 695f 7265 6665 7265 6e63 652f 6175 676d  i_reference/augm
-00004c00: 656e 7461 7469 6f6e 732f 7472 616e 7366  entations/transf
-00004c10: 6f72 6d73 2f23 616c 6275 6d65 6e74 6174  orms/#albumentat
-00004c20: 696f 6e73 2e61 7567 6d65 6e74 6174 696f  ions.augmentatio
-00004c30: 6e73 2e74 7261 6e73 666f 726d 732e 546f  ns.transforms.To
-00004c40: 5247 4229 0a2d 205b 546f 5365 7069 615d  RGB).- [ToSepia]
-00004c50: 2868 7474 7073 3a2f 2f61 6c62 756d 656e  (https://albumen
-00004c60: 7461 7469 6f6e 732e 6169 2f64 6f63 732f  tations.ai/docs/
-00004c70: 6170 695f 7265 6665 7265 6e63 652f 6175  api_reference/au
-00004c80: 676d 656e 7461 7469 6f6e 732f 7472 616e  gmentations/tran
-00004c90: 7366 6f72 6d73 2f23 616c 6275 6d65 6e74  sforms/#albument
-00004ca0: 6174 696f 6e73 2e61 7567 6d65 6e74 6174  ations.augmentat
-00004cb0: 696f 6e73 2e74 7261 6e73 666f 726d 732e  ions.transforms.
-00004cc0: 546f 5365 7069 6129 0a2d 205b 556e 7368  ToSepia).- [Unsh
-00004cd0: 6172 704d 6173 6b5d 2868 7474 7073 3a2f  arpMask](https:/
-00004ce0: 2f61 6c62 756d 656e 7461 7469 6f6e 732e  /albumentations.
-00004cf0: 6169 2f64 6f63 732f 6170 695f 7265 6665  ai/docs/api_refe
-00004d00: 7265 6e63 652f 6175 676d 656e 7461 7469  rence/augmentati
-00004d10: 6f6e 732f 7472 616e 7366 6f72 6d73 2f23  ons/transforms/#
-00004d20: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
-00004d30: 7567 6d65 6e74 6174 696f 6e73 2e74 7261  ugmentations.tra
-00004d40: 6e73 666f 726d 732e 556e 7368 6172 704d  nsforms.UnsharpM
-00004d50: 6173 6b29 0a2d 205b 5a6f 6f6d 426c 7572  ask).- [ZoomBlur
-00004d60: 5d28 6874 7470 733a 2f2f 616c 6275 6d65  ](https://albume
-00004d70: 6e74 6174 696f 6e73 2e61 692f 646f 6373  ntations.ai/docs
-00004d80: 2f61 7069 5f72 6566 6572 656e 6365 2f61  /api_reference/a
-00004d90: 7567 6d65 6e74 6174 696f 6e73 2f62 6c75  ugmentations/blu
-00004da0: 722f 7472 616e 7366 6f72 6d73 2f23 616c  r/transforms/#al
-00004db0: 6275 6d65 6e74 6174 696f 6e73 2e61 7567  bumentations.aug
-00004dc0: 6d65 6e74 6174 696f 6e73 2e62 6c75 722e  mentations.blur.
-00004dd0: 7472 616e 7366 6f72 6d73 2e5a 6f6f 6d42  transforms.ZoomB
-00004de0: 6c75 7229 0a0a 2323 2320 5370 6174 6961  lur)..### Spatia
-00004df0: 6c2d 6c65 7665 6c20 7472 616e 7366 6f72  l-level transfor
-00004e00: 6d73 0a0a 5370 6174 6961 6c2d 6c65 7665  ms..Spatial-leve
-00004e10: 6c20 7472 616e 7366 6f72 6d73 2077 696c  l transforms wil
-00004e20: 6c20 7369 6d75 6c74 616e 656f 7573 6c79  l simultaneously
-00004e30: 2063 6861 6e67 6520 626f 7468 2061 6e20   change both an 
-00004e40: 696e 7075 7420 696d 6167 6520 6173 2077  input image as w
-00004e50: 656c 6c20 6173 2061 6464 6974 696f 6e61  ell as additiona
-00004e60: 6c20 7461 7267 6574 7320 7375 6368 2061  l targets such a
-00004e70: 7320 6d61 736b 732c 2062 6f75 6e64 696e  s masks, boundin
-00004e80: 6720 626f 7865 732c 2061 6e64 206b 6579  g boxes, and key
-00004e90: 706f 696e 7473 2e20 5468 6520 666f 6c6c  points. The foll
-00004ea0: 6f77 696e 6720 7461 626c 6520 7368 6f77  owing table show
-00004eb0: 7320 7768 6963 6820 6164 6469 7469 6f6e  s which addition
-00004ec0: 616c 2074 6172 6765 7473 2061 7265 2073  al targets are s
-00004ed0: 7570 706f 7274 6564 2062 7920 6561 6368  upported by each
-00004ee0: 2074 7261 6e73 666f 726d 2e0a 0a7c 2054   transform...| T
-00004ef0: 7261 6e73 666f 726d 2020 2020 2020 2020  ransform        
-00004f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f90: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00004fa0: 2049 6d61 6765 207c 204d 6173 6b20 7c20   Image | Mask | 
-00004fb0: 4242 6f78 6573 207c 204b 6579 706f 696e  BBoxes | Keypoin
-00004fc0: 7473 207c 0a7c 202d 2d2d 2d2d 2d2d 2d2d  ts |.| ---------
-00004fd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004fe0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004ff0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005000: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005010: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005020: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005030: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005040: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005050: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005060: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005070: 2d2d 2d2d 2d2d 207c 203a 2d2d 2d3a 207c  ------ | :---: |
-00005080: 203a 2d2d 3a20 7c20 3a2d 2d2d 2d3a 207c   :--: | :----: |
-00005090: 203a 2d2d 2d2d 2d2d 2d3a 207c 0a7c 205b   :-------: |.| [
-000050a0: 4166 6669 6e65 5d28 6874 7470 733a 2f2f  Affine](https://
-000050b0: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
-000050c0: 692f 646f 6373 2f61 7069 5f72 6566 6572  i/docs/api_refer
-000050d0: 656e 6365 2f61 7567 6d65 6e74 6174 696f  ence/augmentatio
-000050e0: 6e73 2f67 656f 6d65 7472 6963 2f74 7261  ns/geometric/tra
-000050f0: 6e73 666f 726d 732f 2361 6c62 756d 656e  nsforms/#albumen
-00005100: 7461 7469 6f6e 732e 6175 676d 656e 7461  tations.augmenta
-00005110: 7469 6f6e 732e 6765 6f6d 6574 7269 632e  tions.geometric.
-00005120: 7472 616e 7366 6f72 6d73 2e41 6666 696e  transforms.Affin
-00005130: 6529 2020 2020 2020 2020 2020 2020 2020  e)              
-00005140: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00005150: 20e2 9c93 2020 2020 207c 20e2 9c93 2020   ...     | ...  
-00005160: 2020 7c20 e29c 9320 2020 2020 207c 20e2    | ...      | .
-00005170: 9c93 2020 2020 2020 2020 207c 0a7c 205b  ..         |.| [
-00005180: 4242 6f78 5361 6665 5261 6e64 6f6d 4372  BBoxSafeRandomCr
-00005190: 6f70 5d28 6874 7470 733a 2f2f 616c 6275  op](https://albu
-000051a0: 6d65 6e74 6174 696f 6e73 2e61 692f 646f  mentations.ai/do
-000051b0: 6373 2f61 7069 5f72 6566 6572 656e 6365  cs/api_reference
-000051c0: 2f61 7567 6d65 6e74 6174 696f 6e73 2f63  /augmentations/c
-000051d0: 726f 7073 2f74 7261 6e73 666f 726d 732f  rops/transforms/
-000051e0: 2361 6c62 756d 656e 7461 7469 6f6e 732e  #albumentations.
-000051f0: 6175 676d 656e 7461 7469 6f6e 732e 6372  augmentations.cr
-00005200: 6f70 732e 7472 616e 7366 6f72 6d73 2e42  ops.transforms.B
-00005210: 426f 7853 6166 6552 616e 646f 6d43 726f  BoxSafeRandomCro
-00005220: 7029 2020 2020 2020 2020 2020 2020 207c  p)             |
-00005230: 20e2 9c93 2020 2020 207c 20e2 9c93 2020   ...     | ...  
-00005240: 2020 7c20 e29c 9320 2020 2020 207c 2020    | ...      |  
-00005250: 2020 2020 2020 2020 207c 0a7c 205b 4365           |.| [Ce
-00005260: 6e74 6572 4372 6f70 5d28 6874 7470 733a  nterCrop](https:
-00005270: 2f2f 616c 6275 6d65 6e74 6174 696f 6e73  //albumentations
-00005280: 2e61 692f 646f 6373 2f61 7069 5f72 6566  .ai/docs/api_ref
-00005290: 6572 656e 6365 2f61 7567 6d65 6e74 6174  erence/augmentat
-000052a0: 696f 6e73 2f63 726f 7073 2f74 7261 6e73  ions/crops/trans
-000052b0: 666f 726d 732f 2361 6c62 756d 656e 7461  forms/#albumenta
-000052c0: 7469 6f6e 732e 6175 676d 656e 7461 7469  tions.augmentati
-000052d0: 6f6e 732e 6372 6f70 732e 7472 616e 7366  ons.crops.transf
-000052e0: 6f72 6d73 2e43 656e 7465 7243 726f 7029  orms.CenterCrop)
-000052f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005300: 2020 2020 2020 2020 2020 2020 207c 20e2               | .
-00005310: 9c93 2020 2020 207c 20e2 9c93 2020 2020  ..     | ...    
-00005320: 7c20 e29c 9320 2020 2020 207c 20e2 9c93  | ...      | ...
-00005330: 2020 2020 2020 2020 207c 0a7c 205b 436f           |.| [Co
-00005340: 6172 7365 4472 6f70 6f75 745d 2868 7474  arseDropout](htt
-00005350: 7073 3a2f 2f61 6c62 756d 656e 7461 7469  ps://albumentati
-00005360: 6f6e 732e 6169 2f64 6f63 732f 6170 695f  ons.ai/docs/api_
-00005370: 7265 6665 7265 6e63 652f 6175 676d 656e  reference/augmen
-00005380: 7461 7469 6f6e 732f 6472 6f70 6f75 742f  tations/dropout/
-00005390: 636f 6172 7365 5f64 726f 706f 7574 2f23  coarse_dropout/#
-000053a0: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
-000053b0: 7567 6d65 6e74 6174 696f 6e73 2e64 726f  ugmentations.dro
-000053c0: 706f 7574 2e63 6f61 7273 655f 6472 6f70  pout.coarse_drop
-000053d0: 6f75 742e 436f 6172 7365 4472 6f70 6f75  out.CoarseDropou
-000053e0: 7429 2020 2020 2020 2020 2020 207c 20e2  t)           | .
-000053f0: 9c93 2020 2020 207c 20e2 9c93 2020 2020  ..     | ...    
-00005400: 7c20 2020 2020 2020 207c 20e2 9c93 2020  |        | ...  
-00005410: 2020 2020 2020 207c 0a7c 205b 4372 6f70         |.| [Crop
-00005420: 5d28 6874 7470 733a 2f2f 616c 6275 6d65  ](https://albume
-00005430: 6e74 6174 696f 6e73 2e61 692f 646f 6373  ntations.ai/docs
-00005440: 2f61 7069 5f72 6566 6572 656e 6365 2f61  /api_reference/a
-00005450: 7567 6d65 6e74 6174 696f 6e73 2f63 726f  ugmentations/cro
-00005460: 7073 2f74 7261 6e73 666f 726d 732f 2361  ps/transforms/#a
-00005470: 6c62 756d 656e 7461 7469 6f6e 732e 6175  lbumentations.au
-00005480: 676d 656e 7461 7469 6f6e 732e 6372 6f70  gmentations.crop
-00005490: 732e 7472 616e 7366 6f72 6d73 2e43 726f  s.transforms.Cro
-000054a0: 7029 2020 2020 2020 2020 2020 2020 2020  p)              
-000054b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000054c0: 2020 2020 2020 2020 2020 207c 20e2 9c93             | ...
-000054d0: 2020 2020 207c 20e2 9c93 2020 2020 7c20       | ...    | 
-000054e0: e29c 9320 2020 2020 207c 20e2 9c93 2020  ...      | ...  
-000054f0: 2020 2020 2020 207c 0a7c 205b 4372 6f70         |.| [Crop
-00005500: 416e 6450 6164 5d28 6874 7470 733a 2f2f  AndPad](https://
-00005510: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
-00005520: 692f 646f 6373 2f61 7069 5f72 6566 6572  i/docs/api_refer
-00005530: 656e 6365 2f61 7567 6d65 6e74 6174 696f  ence/augmentatio
-00005540: 6e73 2f63 726f 7073 2f74 7261 6e73 666f  ns/crops/transfo
-00005550: 726d 732f 2361 6c62 756d 656e 7461 7469  rms/#albumentati
-00005560: 6f6e 732e 6175 676d 656e 7461 7469 6f6e  ons.augmentation
-00005570: 732e 6372 6f70 732e 7472 616e 7366 6f72  s.crops.transfor
-00005580: 6d73 2e43 726f 7041 6e64 5061 6429 2020  ms.CropAndPad)  
-00005590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000055a0: 2020 2020 2020 2020 2020 207c 20e2 9c93             | ...
-000055b0: 2020 2020 207c 20e2 9c93 2020 2020 7c20       | ...    | 
-000055c0: e29c 9320 2020 2020 207c 20e2 9c93 2020  ...      | ...  
-000055d0: 2020 2020 2020 207c 0a7c 205b 4372 6f70         |.| [Crop
-000055e0: 4e6f 6e45 6d70 7479 4d61 736b 4966 4578  NonEmptyMaskIfEx
-000055f0: 6973 7473 5d28 6874 7470 733a 2f2f 616c  ists](https://al
-00005600: 6275 6d65 6e74 6174 696f 6e73 2e61 692f  bumentations.ai/
-00005610: 646f 6373 2f61 7069 5f72 6566 6572 656e  docs/api_referen
-00005620: 6365 2f61 7567 6d65 6e74 6174 696f 6e73  ce/augmentations
-00005630: 2f63 726f 7073 2f74 7261 6e73 666f 726d  /crops/transform
-00005640: 732f 2361 6c62 756d 656e 7461 7469 6f6e  s/#albumentation
-00005650: 732e 6175 676d 656e 7461 7469 6f6e 732e  s.augmentations.
-00005660: 6372 6f70 732e 7472 616e 7366 6f72 6d73  crops.transforms
-00005670: 2e43 726f 704e 6f6e 456d 7074 794d 6173  .CropNonEmptyMas
-00005680: 6b49 6645 7869 7374 7329 207c 20e2 9c93  kIfExists) | ...
-00005690: 2020 2020 207c 20e2 9c93 2020 2020 7c20       | ...    | 
-000056a0: e29c 9320 2020 2020 207c 20e2 9c93 2020  ...      | ...  
-000056b0: 2020 2020 2020 207c 0a7c 205b 456c 6173         |.| [Elas
-000056c0: 7469 6354 7261 6e73 666f 726d 5d28 6874  ticTransform](ht
-000056d0: 7470 733a 2f2f 616c 6275 6d65 6e74 6174  tps://albumentat
-000056e0: 696f 6e73 2e61 692f 646f 6373 2f61 7069  ions.ai/docs/api
-000056f0: 5f72 6566 6572 656e 6365 2f61 7567 6d65  _reference/augme
-00005700: 6e74 6174 696f 6e73 2f67 656f 6d65 7472  ntations/geometr
-00005710: 6963 2f74 7261 6e73 666f 726d 732f 2361  ic/transforms/#a
-00005720: 6c62 756d 656e 7461 7469 6f6e 732e 6175  lbumentations.au
-00005730: 676d 656e 7461 7469 6f6e 732e 6765 6f6d  gmentations.geom
-00005740: 6574 7269 632e 7472 616e 7366 6f72 6d73  etric.transforms
-00005750: 2e45 6c61 7374 6963 5472 616e 7366 6f72  .ElasticTransfor
-00005760: 6d29 2020 2020 2020 2020 207c 20e2 9c93  m)         | ...
-00005770: 2020 2020 207c 20e2 9c93 2020 2020 7c20       | ...    | 
-00005780: e29c 9320 2020 2020 207c 2020 2020 2020  ...      |      
-00005790: 2020 2020 207c 0a7c 205b 466c 6970 5d28       |.| [Flip](
-000057a0: 6874 7470 733a 2f2f 616c 6275 6d65 6e74  https://albument
-000057b0: 6174 696f 6e73 2e61 692f 646f 6373 2f61  ations.ai/docs/a
-000057c0: 7069 5f72 6566 6572 656e 6365 2f61 7567  pi_reference/aug
-000057d0: 6d65 6e74 6174 696f 6e73 2f67 656f 6d65  mentations/geome
-000057e0: 7472 6963 2f74 7261 6e73 666f 726d 732f  tric/transforms/
-000057f0: 2361 6c62 756d 656e 7461 7469 6f6e 732e  #albumentations.
-00005800: 6175 676d 656e 7461 7469 6f6e 732e 6765  augmentations.ge
-00005810: 6f6d 6574 7269 632e 7472 616e 7366 6f72  ometric.transfor
-00005820: 6d73 2e46 6c69 7029 2020 2020 2020 2020  ms.Flip)        
-00005830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005840: 2020 2020 2020 2020 207c 20e2 9c93 2020           | ...  
-00005850: 2020 207c 20e2 9c93 2020 2020 7c20 e29c     | ...    | ..
-00005860: 9320 2020 2020 207c 20e2 9c93 2020 2020  .      | ...    
-00005870: 2020 2020 207c 0a7c 205b 4772 6964 4469       |.| [GridDi
-00005880: 7374 6f72 7469 6f6e 5d28 6874 7470 733a  stortion](https:
-00005890: 2f2f 616c 6275 6d65 6e74 6174 696f 6e73  //albumentations
-000058a0: 2e61 692f 646f 6373 2f61 7069 5f72 6566  .ai/docs/api_ref
-000058b0: 6572 656e 6365 2f61 7567 6d65 6e74 6174  erence/augmentat
-000058c0: 696f 6e73 2f67 656f 6d65 7472 6963 2f74  ions/geometric/t
-000058d0: 7261 6e73 666f 726d 732f 2361 6c62 756d  ransforms/#album
-000058e0: 656e 7461 7469 6f6e 732e 6175 676d 656e  entations.augmen
-000058f0: 7461 7469 6f6e 732e 6765 6f6d 6574 7269  tations.geometri
-00005900: 632e 7472 616e 7366 6f72 6d73 2e47 7269  c.transforms.Gri
-00005910: 6444 6973 746f 7274 696f 6e29 2020 2020  dDistortion)    
-00005920: 2020 2020 2020 2020 207c 20e2 9c93 2020           | ...  
-00005930: 2020 207c 20e2 9c93 2020 2020 7c20 e29c     | ...    | ..
-00005940: 9320 2020 2020 207c 2020 2020 2020 2020  .      |        
-00005950: 2020 207c 0a7c 205b 4772 6964 4472 6f70     |.| [GridDrop
-00005960: 6f75 745d 2868 7474 7073 3a2f 2f61 6c62  out](https://alb
-00005970: 756d 656e 7461 7469 6f6e 732e 6169 2f64  umentations.ai/d
-00005980: 6f63 732f 6170 695f 7265 6665 7265 6e63  ocs/api_referenc
-00005990: 652f 6175 676d 656e 7461 7469 6f6e 732f  e/augmentations/
-000059a0: 6472 6f70 6f75 742f 6772 6964 5f64 726f  dropout/grid_dro
-000059b0: 706f 7574 2f23 616c 6275 6d65 6e74 6174  pout/#albumentat
-000059c0: 696f 6e73 2e61 7567 6d65 6e74 6174 696f  ions.augmentatio
-000059d0: 6e73 2e64 726f 706f 7574 2e67 7269 645f  ns.dropout.grid_
-000059e0: 6472 6f70 6f75 742e 4772 6964 4472 6f70  dropout.GridDrop
-000059f0: 6f75 7429 2020 2020 2020 2020 2020 2020  out)            
-00005a00: 2020 2020 2020 207c 20e2 9c93 2020 2020         | ...    
-00005a10: 207c 20e2 9c93 2020 2020 7c20 2020 2020   | ...    |     
-00005a20: 2020 207c 2020 2020 2020 2020 2020 207c     |           |
-00005a30: 0a7c 205b 486f 7269 7a6f 6e74 616c 466c  .| [HorizontalFl
-00005a40: 6970 5d28 6874 7470 733a 2f2f 616c 6275  ip](https://albu
-00005a50: 6d65 6e74 6174 696f 6e73 2e61 692f 646f  mentations.ai/do
-00005a60: 6373 2f61 7069 5f72 6566 6572 656e 6365  cs/api_reference
-00005a70: 2f61 7567 6d65 6e74 6174 696f 6e73 2f67  /augmentations/g
-00005a80: 656f 6d65 7472 6963 2f74 7261 6e73 666f  eometric/transfo
-00005a90: 726d 732f 2361 6c62 756d 656e 7461 7469  rms/#albumentati
-00005aa0: 6f6e 732e 6175 676d 656e 7461 7469 6f6e  ons.augmentation
-00005ab0: 732e 6765 6f6d 6574 7269 632e 7472 616e  s.geometric.tran
-00005ac0: 7366 6f72 6d73 2e48 6f72 697a 6f6e 7461  sforms.Horizonta
-00005ad0: 6c46 6c69 7029 2020 2020 2020 2020 2020  lFlip)          
-00005ae0: 2020 207c 20e2 9c93 2020 2020 207c 20e2     | ...     | .
-00005af0: 9c93 2020 2020 7c20 e29c 9320 2020 2020  ..    | ...     
-00005b00: 207c 20e2 9c93 2020 2020 2020 2020 207c   | ...         |
-00005b10: 0a7c 205b 4c61 6d62 6461 5d28 6874 7470  .| [Lambda](http
-00005b20: 733a 2f2f 616c 6275 6d65 6e74 6174 696f  s://albumentatio
-00005b30: 6e73 2e61 692f 646f 6373 2f61 7069 5f72  ns.ai/docs/api_r
-00005b40: 6566 6572 656e 6365 2f61 7567 6d65 6e74  eference/augment
-00005b50: 6174 696f 6e73 2f74 7261 6e73 666f 726d  ations/transform
-00005b60: 732f 2361 6c62 756d 656e 7461 7469 6f6e  s/#albumentation
-00005b70: 732e 6175 676d 656e 7461 7469 6f6e 732e  s.augmentations.
-00005b80: 7472 616e 7366 6f72 6d73 2e4c 616d 6264  transforms.Lambd
-00005b90: 6129 2020 2020 2020 2020 2020 2020 2020  a)              
-00005ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005bc0: 2020 207c 20e2 9c93 2020 2020 207c 20e2     | ...     | .
-00005bd0: 9c93 2020 2020 7c20 e29c 9320 2020 2020  ..    | ...     
-00005be0: 207c 20e2 9c93 2020 2020 2020 2020 207c   | ...         |
-00005bf0: 0a7c 205b 4c6f 6e67 6573 744d 6178 5369  .| [LongestMaxSi
-00005c00: 7a65 5d28 6874 7470 733a 2f2f 616c 6275  ze](https://albu
-00005c10: 6d65 6e74 6174 696f 6e73 2e61 692f 646f  mentations.ai/do
-00005c20: 6373 2f61 7069 5f72 6566 6572 656e 6365  cs/api_reference
-00005c30: 2f61 7567 6d65 6e74 6174 696f 6e73 2f67  /augmentations/g
-00005c40: 656f 6d65 7472 6963 2f72 6573 697a 652f  eometric/resize/
-00005c50: 2361 6c62 756d 656e 7461 7469 6f6e 732e  #albumentations.
-00005c60: 6175 676d 656e 7461 7469 6f6e 732e 6765  augmentations.ge
-00005c70: 6f6d 6574 7269 632e 7265 7369 7a65 2e4c  ometric.resize.L
-00005c80: 6f6e 6765 7374 4d61 7853 697a 6529 2020  ongestMaxSize)  
-00005c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ca0: 2020 207c 20e2 9c93 2020 2020 207c 20e2     | ...     | .
-00005cb0: 9c93 2020 2020 7c20 e29c 9320 2020 2020  ..    | ...     
-00005cc0: 207c 20e2 9c93 2020 2020 2020 2020 207c   | ...         |
-00005cd0: 0a7c 205b 4d61 736b 4472 6f70 6f75 745d  .| [MaskDropout]
-00005ce0: 2868 7474 7073 3a2f 2f61 6c62 756d 656e  (https://albumen
-00005cf0: 7461 7469 6f6e 732e 6169 2f64 6f63 732f  tations.ai/docs/
-00005d00: 6170 695f 7265 6665 7265 6e63 652f 6175  api_reference/au
-00005d10: 676d 656e 7461 7469 6f6e 732f 6472 6f70  gmentations/drop
-00005d20: 6f75 742f 6d61 736b 5f64 726f 706f 7574  out/mask_dropout
-00005d30: 2f23 616c 6275 6d65 6e74 6174 696f 6e73  /#albumentations
-00005d40: 2e61 7567 6d65 6e74 6174 696f 6e73 2e64  .augmentations.d
-00005d50: 726f 706f 7574 2e6d 6173 6b5f 6472 6f70  ropout.mask_drop
-00005d60: 6f75 742e 4d61 736b 4472 6f70 6f75 7429  out.MaskDropout)
-00005d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d80: 2020 207c 20e2 9c93 2020 2020 207c 20e2     | ...     | .
-00005d90: 9c93 2020 2020 7c20 2020 2020 2020 207c  ..    |        |
-00005da0: 2020 2020 2020 2020 2020 207c 0a7c 205b             |.| [
-00005db0: 4e6f 4f70 5d28 6874 7470 733a 2f2f 616c  NoOp](https://al
-00005dc0: 6275 6d65 6e74 6174 696f 6e73 2e61 692f  bumentations.ai/
-00005dd0: 646f 6373 2f61 7069 5f72 6566 6572 656e  docs/api_referen
-00005de0: 6365 2f63 6f72 652f 7472 616e 7366 6f72  ce/core/transfor
-00005df0: 6d73 5f69 6e74 6572 6661 6365 2f23 616c  ms_interface/#al
-00005e00: 6275 6d65 6e74 6174 696f 6e73 2e63 6f72  bumentations.cor
-00005e10: 652e 7472 616e 7366 6f72 6d73 5f69 6e74  e.transforms_int
-00005e20: 6572 6661 6365 2e4e 6f4f 7029 2020 2020  erface.NoOp)    
-00005e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e50: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00005e60: 20e2 9c93 2020 2020 207c 20e2 9c93 2020   ...     | ...  
-00005e70: 2020 7c20 e29c 9320 2020 2020 207c 20e2    | ...      | .
-00005e80: 9c93 2020 2020 2020 2020 207c 0a7c 205b  ..         |.| [
-00005e90: 4f70 7469 6361 6c44 6973 746f 7274 696f  OpticalDistortio
-00005ea0: 6e5d 2868 7474 7073 3a2f 2f61 6c62 756d  n](https://album
-00005eb0: 656e 7461 7469 6f6e 732e 6169 2f64 6f63  entations.ai/doc
-00005ec0: 732f 6170 695f 7265 6665 7265 6e63 652f  s/api_reference/
-00005ed0: 6175 676d 656e 7461 7469 6f6e 732f 6765  augmentations/ge
-00005ee0: 6f6d 6574 7269 632f 7472 616e 7366 6f72  ometric/transfor
-00005ef0: 6d73 2f23 616c 6275 6d65 6e74 6174 696f  ms/#albumentatio
-00005f00: 6e73 2e61 7567 6d65 6e74 6174 696f 6e73  ns.augmentations
-00005f10: 2e67 656f 6d65 7472 6963 2e74 7261 6e73  .geometric.trans
-00005f20: 666f 726d 732e 4f70 7469 6361 6c44 6973  forms.OpticalDis
-00005f30: 746f 7274 696f 6e29 2020 2020 2020 207c  tortion)       |
-00005f40: 20e2 9c93 2020 2020 207c 20e2 9c93 2020   ...     | ...  
-00005f50: 2020 7c20 e29c 9320 2020 2020 207c 2020    | ...      |  
-00005f60: 2020 2020 2020 2020 207c 0a7c 205b 5061           |.| [Pa
-00005f70: 6449 664e 6565 6465 645d 2868 7474 7073  dIfNeeded](https
-00005f80: 3a2f 2f61 6c62 756d 656e 7461 7469 6f6e  ://albumentation
-00005f90: 732e 6169 2f64 6f63 732f 6170 695f 7265  s.ai/docs/api_re
-00005fa0: 6665 7265 6e63 652f 6175 676d 656e 7461  ference/augmenta
-00005fb0: 7469 6f6e 732f 6765 6f6d 6574 7269 632f  tions/geometric/
-00005fc0: 7472 616e 7366 6f72 6d73 2f23 616c 6275  transforms/#albu
-00005fd0: 6d65 6e74 6174 696f 6e73 2e61 7567 6d65  mentations.augme
-00005fe0: 6e74 6174 696f 6e73 2e67 656f 6d65 7472  ntations.geometr
-00005ff0: 6963 2e74 7261 6e73 666f 726d 732e 5061  ic.transforms.Pa
-00006000: 6449 664e 6565 6465 6429 2020 2020 2020  dIfNeeded)      
-00006010: 2020 2020 2020 2020 2020 2020 207c 20e2               | .
-00006020: 9c93 2020 2020 207c 20e2 9c93 2020 2020  ..     | ...    
-00006030: 7c20 e29c 9320 2020 2020 207c 20e2 9c93  | ...      | ...
-00006040: 2020 2020 2020 2020 207c 0a7c 205b 5065           |.| [Pe
-00006050: 7273 7065 6374 6976 655d 2868 7474 7073  rspective](https
-00006060: 3a2f 2f61 6c62 756d 656e 7461 7469 6f6e  ://albumentation
-00006070: 732e 6169 2f64 6f63 732f 6170 695f 7265  s.ai/docs/api_re
-00006080: 6665 7265 6e63 652f 6175 676d 656e 7461  ference/augmenta
-00006090: 7469 6f6e 732f 6765 6f6d 6574 7269 632f  tions/geometric/
-000060a0: 7472 616e 7366 6f72 6d73 2f23 616c 6275  transforms/#albu
-000060b0: 6d65 6e74 6174 696f 6e73 2e61 7567 6d65  mentations.augme
-000060c0: 6e74 6174 696f 6e73 2e67 656f 6d65 7472  ntations.geometr
-000060d0: 6963 2e74 7261 6e73 666f 726d 732e 5065  ic.transforms.Pe
-000060e0: 7273 7065 6374 6976 6529 2020 2020 2020  rspective)      
-000060f0: 2020 2020 2020 2020 2020 2020 207c 20e2               | .
-00006100: 9c93 2020 2020 207c 20e2 9c93 2020 2020  ..     | ...    
-00006110: 7c20 e29c 9320 2020 2020 207c 20e2 9c93  | ...      | ...
-00006120: 2020 2020 2020 2020 207c 0a7c 205b 5069           |.| [Pi
-00006130: 6563 6577 6973 6541 6666 696e 655d 2868  ecewiseAffine](h
-00006140: 7474 7073 3a2f 2f61 6c62 756d 656e 7461  ttps://albumenta
-00006150: 7469 6f6e 732e 6169 2f64 6f63 732f 6170  tions.ai/docs/ap
-00006160: 695f 7265 6665 7265 6e63 652f 6175 676d  i_reference/augm
-00006170: 656e 7461 7469 6f6e 732f 6765 6f6d 6574  entations/geomet
-00006180: 7269 632f 7472 616e 7366 6f72 6d73 2f23  ric/transforms/#
-00006190: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
-000061a0: 7567 6d65 6e74 6174 696f 6e73 2e67 656f  ugmentations.geo
-000061b0: 6d65 7472 6963 2e74 7261 6e73 666f 726d  metric.transform
-000061c0: 732e 5069 6563 6577 6973 6541 6666 696e  s.PiecewiseAffin
-000061d0: 6529 2020 2020 2020 2020 2020 207c 20e2  e)           | .
-000061e0: 9c93 2020 2020 207c 20e2 9c93 2020 2020  ..     | ...    
-000061f0: 7c20 e29c 9320 2020 2020 207c 20e2 9c93  | ...      | ...
-00006200: 2020 2020 2020 2020 207c 0a7c 205b 5069           |.| [Pi
-00006210: 7865 6c44 726f 706f 7574 5d28 6874 7470  xelDropout](http
-00006220: 733a 2f2f 616c 6275 6d65 6e74 6174 696f  s://albumentatio
-00006230: 6e73 2e61 692f 646f 6373 2f61 7069 5f72  ns.ai/docs/api_r
-00006240: 6566 6572 656e 6365 2f61 7567 6d65 6e74  eference/augment
-00006250: 6174 696f 6e73 2f74 7261 6e73 666f 726d  ations/transform
-00006260: 732f 2361 6c62 756d 656e 7461 7469 6f6e  s/#albumentation
-00006270: 732e 6175 676d 656e 7461 7469 6f6e 732e  s.augmentations.
-00006280: 7472 616e 7366 6f72 6d73 2e50 6978 656c  transforms.Pixel
-00006290: 4472 6f70 6f75 7429 2020 2020 2020 2020  Dropout)        
-000062a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062b0: 2020 2020 2020 2020 2020 2020 207c 20e2               | .
-000062c0: 9c93 2020 2020 207c 20e2 9c93 2020 2020  ..     | ...    
-000062d0: 7c20 2020 2020 2020 207c 2020 2020 2020  |        |      
-000062e0: 2020 2020 207c 0a7c 205b 5261 6e64 6f6d       |.| [Random
-000062f0: 4372 6f70 5d28 6874 7470 733a 2f2f 616c  Crop](https://al
-00006300: 6275 6d65 6e74 6174 696f 6e73 2e61 692f  bumentations.ai/
-00006310: 646f 6373 2f61 7069 5f72 6566 6572 656e  docs/api_referen
-00006320: 6365 2f61 7567 6d65 6e74 6174 696f 6e73  ce/augmentations
-00006330: 2f63 726f 7073 2f74 7261 6e73 666f 726d  /crops/transform
-00006340: 732f 2361 6c62 756d 656e 7461 7469 6f6e  s/#albumentation
-00006350: 732e 6175 676d 656e 7461 7469 6f6e 732e  s.augmentations.
-00006360: 6372 6f70 732e 7472 616e 7366 6f72 6d73  crops.transforms
-00006370: 2e52 616e 646f 6d43 726f 7029 2020 2020  .RandomCrop)    
-00006380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006390: 2020 2020 2020 2020 207c 20e2 9c93 2020           | ...  
-000063a0: 2020 207c 20e2 9c93 2020 2020 7c20 e29c     | ...    | ..
-000063b0: 9320 2020 2020 207c 20e2 9c93 2020 2020  .      | ...    
-000063c0: 2020 2020 207c 0a7c 205b 5261 6e64 6f6d       |.| [Random
-000063d0: 4372 6f70 4672 6f6d 426f 7264 6572 735d  CropFromBorders]
-000063e0: 2868 7474 7073 3a2f 2f61 6c62 756d 656e  (https://albumen
-000063f0: 7461 7469 6f6e 732e 6169 2f64 6f63 732f  tations.ai/docs/
-00006400: 6170 695f 7265 6665 7265 6e63 652f 6175  api_reference/au
-00006410: 676d 656e 7461 7469 6f6e 732f 6372 6f70  gmentations/crop
-00006420: 732f 7472 616e 7366 6f72 6d73 2f23 616c  s/transforms/#al
-00006430: 6275 6d65 6e74 6174 696f 6e73 2e61 7567  bumentations.aug
-00006440: 6d65 6e74 6174 696f 6e73 2e63 726f 7073  mentations.crops
-00006450: 2e74 7261 6e73 666f 726d 732e 5261 6e64  .transforms.Rand
-00006460: 6f6d 4372 6f70 4672 6f6d 426f 7264 6572  omCropFromBorder
-00006470: 7329 2020 2020 2020 207c 20e2 9c93 2020  s)       | ...  
-00006480: 2020 207c 20e2 9c93 2020 2020 7c20 e29c     | ...    | ..
-00006490: 9320 2020 2020 207c 20e2 9c93 2020 2020  .      | ...    
-000064a0: 2020 2020 207c 0a7c 205b 5261 6e64 6f6d       |.| [Random
-000064b0: 4372 6f70 4e65 6172 4242 6f78 5d28 6874  CropNearBBox](ht
-000064c0: 7470 733a 2f2f 616c 6275 6d65 6e74 6174  tps://albumentat
-000064d0: 696f 6e73 2e61 692f 646f 6373 2f61 7069  ions.ai/docs/api
-000064e0: 5f72 6566 6572 656e 6365 2f61 7567 6d65  _reference/augme
-000064f0: 6e74 6174 696f 6e73 2f63 726f 7073 2f74  ntations/crops/t
-00006500: 7261 6e73 666f 726d 732f 2361 6c62 756d  ransforms/#album
-00006510: 656e 7461 7469 6f6e 732e 6175 676d 656e  entations.augmen
-00006520: 7461 7469 6f6e 732e 6372 6f70 732e 7472  tations.crops.tr
-00006530: 616e 7366 6f72 6d73 2e52 616e 646f 6d43  ansforms.RandomC
-00006540: 726f 704e 6561 7242 426f 7829 2020 2020  ropNearBBox)    
-00006550: 2020 2020 2020 2020 207c 20e2 9c93 2020           | ...  
-00006560: 2020 207c 20e2 9c93 2020 2020 7c20 e29c     | ...    | ..
-00006570: 9320 2020 2020 207c 20e2 9c93 2020 2020  .      | ...    
-00006580: 2020 2020 207c 0a7c 205b 5261 6e64 6f6d       |.| [Random
-00006590: 4772 6964 5368 7566 666c 655d 2868 7474  GridShuffle](htt
-000065a0: 7073 3a2f 2f61 6c62 756d 656e 7461 7469  ps://albumentati
-000065b0: 6f6e 732e 6169 2f64 6f63 732f 6170 695f  ons.ai/docs/api_
-000065c0: 7265 6665 7265 6e63 652f 6175 676d 656e  reference/augmen
-000065d0: 7461 7469 6f6e 732f 7472 616e 7366 6f72  tations/transfor
-000065e0: 6d73 2f23 616c 6275 6d65 6e74 6174 696f  ms/#albumentatio
-000065f0: 6e73 2e61 7567 6d65 6e74 6174 696f 6e73  ns.augmentations
-00006600: 2e74 7261 6e73 666f 726d 732e 5261 6e64  .transforms.Rand
-00006610: 6f6d 4772 6964 5368 7566 666c 6529 2020  omGridShuffle)  
-00006620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006630: 2020 2020 2020 2020 207c 20e2 9c93 2020           | ...  
-00006640: 2020 207c 20e2 9c93 2020 2020 7c20 2020     | ...    |   
-00006650: 2020 2020 207c 20e2 9c93 2020 2020 2020       | ...      
-00006660: 2020 207c 0a7c 205b 5261 6e64 6f6d 5265     |.| [RandomRe
-00006670: 7369 7a65 6443 726f 705d 2868 7474 7073  sizedCrop](https
-00006680: 3a2f 2f61 6c62 756d 656e 7461 7469 6f6e  ://albumentation
-00006690: 732e 6169 2f64 6f63 732f 6170 695f 7265  s.ai/docs/api_re
-000066a0: 6665 7265 6e63 652f 6175 676d 656e 7461  ference/augmenta
-000066b0: 7469 6f6e 732f 6372 6f70 732f 7472 616e  tions/crops/tran
-000066c0: 7366 6f72 6d73 2f23 616c 6275 6d65 6e74  sforms/#albument
-000066d0: 6174 696f 6e73 2e61 7567 6d65 6e74 6174  ations.augmentat
-000066e0: 696f 6e73 2e63 726f 7073 2e74 7261 6e73  ions.crops.trans
-000066f0: 666f 726d 732e 5261 6e64 6f6d 5265 7369  forms.RandomResi
-00006700: 7a65 6443 726f 7029 2020 2020 2020 2020  zedCrop)        
-00006710: 2020 2020 2020 207c 20e2 9c93 2020 2020         | ...    
-00006720: 207c 20e2 9c93 2020 2020 7c20 e29c 9320   | ...    | ... 
-00006730: 2020 2020 207c 20e2 9c93 2020 2020 2020       | ...      
-00006740: 2020 207c 0a7c 205b 5261 6e64 6f6d 526f     |.| [RandomRo
-00006750: 7461 7465 3930 5d28 6874 7470 733a 2f2f  tate90](https://
-00006760: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
-00006770: 692f 646f 6373 2f61 7069 5f72 6566 6572  i/docs/api_refer
-00006780: 656e 6365 2f61 7567 6d65 6e74 6174 696f  ence/augmentatio
-00006790: 6e73 2f67 656f 6d65 7472 6963 2f72 6f74  ns/geometric/rot
-000067a0: 6174 652f 2361 6c62 756d 656e 7461 7469  ate/#albumentati
-000067b0: 6f6e 732e 6175 676d 656e 7461 7469 6f6e  ons.augmentation
-000067c0: 732e 6765 6f6d 6574 7269 632e 726f 7461  s.geometric.rota
-000067d0: 7465 2e52 616e 646f 6d52 6f74 6174 6539  te.RandomRotate9
-000067e0: 3029 2020 2020 2020 2020 2020 2020 2020  0)              
-000067f0: 2020 2020 2020 207c 20e2 9c93 2020 2020         | ...    
-00006800: 207c 20e2 9c93 2020 2020 7c20 e29c 9320   | ...    | ... 
-00006810: 2020 2020 207c 20e2 9c93 2020 2020 2020       | ...      
-00006820: 2020 207c 0a7c 205b 5261 6e64 6f6d 5363     |.| [RandomSc
-00006830: 616c 655d 2868 7474 7073 3a2f 2f61 6c62  ale](https://alb
-00006840: 756d 656e 7461 7469 6f6e 732e 6169 2f64  umentations.ai/d
-00006850: 6f63 732f 6170 695f 7265 6665 7265 6e63  ocs/api_referenc
-00006860: 652f 6175 676d 656e 7461 7469 6f6e 732f  e/augmentations/
-00006870: 6765 6f6d 6574 7269 632f 7265 7369 7a65  geometric/resize
-00006880: 2f23 616c 6275 6d65 6e74 6174 696f 6e73  /#albumentations
-00006890: 2e61 7567 6d65 6e74 6174 696f 6e73 2e67  .augmentations.g
-000068a0: 656f 6d65 7472 6963 2e72 6573 697a 652e  eometric.resize.
-000068b0: 5261 6e64 6f6d 5363 616c 6529 2020 2020  RandomScale)    
-000068c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068d0: 2020 2020 2020 207c 20e2 9c93 2020 2020         | ...    
-000068e0: 207c 20e2 9c93 2020 2020 7c20 e29c 9320   | ...    | ... 
-000068f0: 2020 2020 207c 20e2 9c93 2020 2020 2020       | ...      
-00006900: 2020 207c 0a7c 205b 5261 6e64 6f6d 5369     |.| [RandomSi
-00006910: 7a65 6442 426f 7853 6166 6543 726f 705d  zedBBoxSafeCrop]
-00006920: 2868 7474 7073 3a2f 2f61 6c62 756d 656e  (https://albumen
-00006930: 7461 7469 6f6e 732e 6169 2f64 6f63 732f  tations.ai/docs/
-00006940: 6170 695f 7265 6665 7265 6e63 652f 6175  api_reference/au
-00006950: 676d 656e 7461 7469 6f6e 732f 6372 6f70  gmentations/crop
-00006960: 732f 7472 616e 7366 6f72 6d73 2f23 616c  s/transforms/#al
-00006970: 6275 6d65 6e74 6174 696f 6e73 2e61 7567  bumentations.aug
-00006980: 6d65 6e74 6174 696f 6e73 2e63 726f 7073  mentations.crops
-00006990: 2e74 7261 6e73 666f 726d 732e 5261 6e64  .transforms.Rand
-000069a0: 6f6d 5369 7a65 6442 426f 7853 6166 6543  omSizedBBoxSafeC
-000069b0: 726f 7029 2020 207c 20e2 9c93 2020 2020  rop)   | ...    
-000069c0: 207c 20e2 9c93 2020 2020 7c20 e29c 9320   | ...    | ... 
-000069d0: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-000069e0: 207c 0a7c 205b 5261 6e64 6f6d 5369 7a65   |.| [RandomSize
-000069f0: 6443 726f 705d 2868 7474 7073 3a2f 2f61  dCrop](https://a
-00006a00: 6c62 756d 656e 7461 7469 6f6e 732e 6169  lbumentations.ai
-00006a10: 2f64 6f63 732f 6170 695f 7265 6665 7265  /docs/api_refere
-00006a20: 6e63 652f 6175 676d 656e 7461 7469 6f6e  nce/augmentation
-00006a30: 732f 6372 6f70 732f 7472 616e 7366 6f72  s/crops/transfor
-00006a40: 6d73 2f23 616c 6275 6d65 6e74 6174 696f  ms/#albumentatio
-00006a50: 6e73 2e61 7567 6d65 6e74 6174 696f 6e73  ns.augmentations
-00006a60: 2e63 726f 7073 2e74 7261 6e73 666f 726d  .crops.transform
-00006a70: 732e 5261 6e64 6f6d 5369 7a65 6443 726f  s.RandomSizedCro
-00006a80: 7029 2020 2020 2020 2020 2020 2020 2020  p)              
-00006a90: 2020 2020 207c 20e2 9c93 2020 2020 207c       | ...     |
-00006aa0: 20e2 9c93 2020 2020 7c20 e29c 9320 2020   ...    | ...   
-00006ab0: 2020 207c 20e2 9c93 2020 2020 2020 2020     | ...        
-00006ac0: 207c 0a7c 205b 5265 7369 7a65 5d28 6874   |.| [Resize](ht
-00006ad0: 7470 733a 2f2f 616c 6275 6d65 6e74 6174  tps://albumentat
-00006ae0: 696f 6e73 2e61 692f 646f 6373 2f61 7069  ions.ai/docs/api
-00006af0: 5f72 6566 6572 656e 6365 2f61 7567 6d65  _reference/augme
-00006b00: 6e74 6174 696f 6e73 2f67 656f 6d65 7472  ntations/geometr
-00006b10: 6963 2f72 6573 697a 652f 2361 6c62 756d  ic/resize/#album
-00006b20: 656e 7461 7469 6f6e 732e 6175 676d 656e  entations.augmen
-00006b30: 7461 7469 6f6e 732e 6765 6f6d 6574 7269  tations.geometri
-00006b40: 632e 7265 7369 7a65 2e52 6573 697a 6529  c.resize.Resize)
-00006b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b70: 2020 2020 207c 20e2 9c93 2020 2020 207c       | ...     |
-00006b80: 20e2 9c93 2020 2020 7c20 e29c 9320 2020   ...    | ...   
-00006b90: 2020 207c 20e2 9c93 2020 2020 2020 2020     | ...        
-00006ba0: 207c 0a7c 205b 526f 7461 7465 5d28 6874   |.| [Rotate](ht
-00006bb0: 7470 733a 2f2f 616c 6275 6d65 6e74 6174  tps://albumentat
-00006bc0: 696f 6e73 2e61 692f 646f 6373 2f61 7069  ions.ai/docs/api
-00006bd0: 5f72 6566 6572 656e 6365 2f61 7567 6d65  _reference/augme
-00006be0: 6e74 6174 696f 6e73 2f67 656f 6d65 7472  ntations/geometr
-00006bf0: 6963 2f72 6f74 6174 652f 2361 6c62 756d  ic/rotate/#album
-00006c00: 656e 7461 7469 6f6e 732e 6175 676d 656e  entations.augmen
-00006c10: 7461 7469 6f6e 732e 6765 6f6d 6574 7269  tations.geometri
-00006c20: 632e 726f 7461 7465 2e52 6f74 6174 6529  c.rotate.Rotate)
-00006c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c50: 2020 2020 207c 20e2 9c93 2020 2020 207c       | ...     |
-00006c60: 20e2 9c93 2020 2020 7c20 e29c 9320 2020   ...    | ...   
-00006c70: 2020 207c 20e2 9c93 2020 2020 2020 2020     | ...        
-00006c80: 207c 0a7c 205b 5361 6665 526f 7461 7465   |.| [SafeRotate
-00006c90: 5d28 6874 7470 733a 2f2f 616c 6275 6d65  ](https://albume
-00006ca0: 6e74 6174 696f 6e73 2e61 692f 646f 6373  ntations.ai/docs
-00006cb0: 2f61 7069 5f72 6566 6572 656e 6365 2f61  /api_reference/a
-00006cc0: 7567 6d65 6e74 6174 696f 6e73 2f67 656f  ugmentations/geo
-00006cd0: 6d65 7472 6963 2f72 6f74 6174 652f 2361  metric/rotate/#a
-00006ce0: 6c62 756d 656e 7461 7469 6f6e 732e 6175  lbumentations.au
-00006cf0: 676d 656e 7461 7469 6f6e 732e 6765 6f6d  gmentations.geom
-00006d00: 6574 7269 632e 726f 7461 7465 2e53 6166  etric.rotate.Saf
-00006d10: 6552 6f74 6174 6529 2020 2020 2020 2020  eRotate)        
-00006d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d30: 2020 2020 207c 20e2 9c93 2020 2020 207c       | ...     |
-00006d40: 20e2 9c93 2020 2020 7c20 e29c 9320 2020   ...    | ...   
-00006d50: 2020 207c 20e2 9c93 2020 2020 2020 2020     | ...        
-00006d60: 207c 0a7c 205b 5368 6966 7453 6361 6c65   |.| [ShiftScale
-00006d70: 526f 7461 7465 5d28 6874 7470 733a 2f2f  Rotate](https://
-00006d80: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
-00006d90: 692f 646f 6373 2f61 7069 5f72 6566 6572  i/docs/api_refer
-00006da0: 656e 6365 2f61 7567 6d65 6e74 6174 696f  ence/augmentatio
-00006db0: 6e73 2f67 656f 6d65 7472 6963 2f74 7261  ns/geometric/tra
-00006dc0: 6e73 666f 726d 732f 2361 6c62 756d 656e  nsforms/#albumen
-00006dd0: 7461 7469 6f6e 732e 6175 676d 656e 7461  tations.augmenta
-00006de0: 7469 6f6e 732e 6765 6f6d 6574 7269 632e  tions.geometric.
-00006df0: 7472 616e 7366 6f72 6d73 2e53 6869 6674  transforms.Shift
-00006e00: 5363 616c 6552 6f74 6174 6529 2020 2020  ScaleRotate)    
-00006e10: 2020 2020 207c 20e2 9c93 2020 2020 207c       | ...     |
-00006e20: 20e2 9c93 2020 2020 7c20 e29c 9320 2020   ...    | ...   
-00006e30: 2020 207c 20e2 9c93 2020 2020 2020 2020     | ...        
-00006e40: 207c 0a7c 205b 536d 616c 6c65 7374 4d61   |.| [SmallestMa
-00006e50: 7853 697a 655d 2868 7474 7073 3a2f 2f61  xSize](https://a
-00006e60: 6c62 756d 656e 7461 7469 6f6e 732e 6169  lbumentations.ai
-00006e70: 2f64 6f63 732f 6170 695f 7265 6665 7265  /docs/api_refere
-00006e80: 6e63 652f 6175 676d 656e 7461 7469 6f6e  nce/augmentation
-00006e90: 732f 6765 6f6d 6574 7269 632f 7265 7369  s/geometric/resi
-00006ea0: 7a65 2f23 616c 6275 6d65 6e74 6174 696f  ze/#albumentatio
-00006eb0: 6e73 2e61 7567 6d65 6e74 6174 696f 6e73  ns.augmentations
-00006ec0: 2e67 656f 6d65 7472 6963 2e72 6573 697a  .geometric.resiz
-00006ed0: 652e 536d 616c 6c65 7374 4d61 7853 697a  e.SmallestMaxSiz
-00006ee0: 6529 2020 2020 2020 2020 2020 2020 2020  e)              
-00006ef0: 2020 2020 207c 20e2 9c93 2020 2020 207c       | ...     |
-00006f00: 20e2 9c93 2020 2020 7c20 e29c 9320 2020   ...    | ...   
-00006f10: 2020 207c 20e2 9c93 2020 2020 2020 2020     | ...        
-00006f20: 207c 0a7c 205b 5472 616e 7370 6f73 655d   |.| [Transpose]
-00006f30: 2868 7474 7073 3a2f 2f61 6c62 756d 656e  (https://albumen
-00006f40: 7461 7469 6f6e 732e 6169 2f64 6f63 732f  tations.ai/docs/
-00006f50: 6170 695f 7265 6665 7265 6e63 652f 6175  api_reference/au
-00006f60: 676d 656e 7461 7469 6f6e 732f 6765 6f6d  gmentations/geom
-00006f70: 6574 7269 632f 7472 616e 7366 6f72 6d73  etric/transforms
-00006f80: 2f23 616c 6275 6d65 6e74 6174 696f 6e73  /#albumentations
-00006f90: 2e61 7567 6d65 6e74 6174 696f 6e73 2e67  .augmentations.g
-00006fa0: 656f 6d65 7472 6963 2e74 7261 6e73 666f  eometric.transfo
-00006fb0: 726d 732e 5472 616e 7370 6f73 6529 2020  rms.Transpose)  
-00006fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006fd0: 2020 2020 207c 20e2 9c93 2020 2020 207c       | ...     |
-00006fe0: 20e2 9c93 2020 2020 7c20 e29c 9320 2020   ...    | ...   
-00006ff0: 2020 207c 20e2 9c93 2020 2020 2020 2020     | ...        
-00007000: 207c 0a7c 205b 5665 7274 6963 616c 466c   |.| [VerticalFl
-00007010: 6970 5d28 6874 7470 733a 2f2f 616c 6275  ip](https://albu
-00007020: 6d65 6e74 6174 696f 6e73 2e61 692f 646f  mentations.ai/do
-00007030: 6373 2f61 7069 5f72 6566 6572 656e 6365  cs/api_reference
-00007040: 2f61 7567 6d65 6e74 6174 696f 6e73 2f67  /augmentations/g
-00007050: 656f 6d65 7472 6963 2f74 7261 6e73 666f  eometric/transfo
-00007060: 726d 732f 2361 6c62 756d 656e 7461 7469  rms/#albumentati
-00007070: 6f6e 732e 6175 676d 656e 7461 7469 6f6e  ons.augmentation
-00007080: 732e 6765 6f6d 6574 7269 632e 7472 616e  s.geometric.tran
-00007090: 7366 6f72 6d73 2e56 6572 7469 6361 6c46  sforms.VerticalF
-000070a0: 6c69 7029 2020 2020 2020 2020 2020 2020  lip)            
-000070b0: 2020 2020 207c 20e2 9c93 2020 2020 207c       | ...     |
-000070c0: 20e2 9c93 2020 2020 7c20 e29c 9320 2020   ...    | ...   
-000070d0: 2020 207c 20e2 9c93 2020 2020 2020 2020     | ...        
-000070e0: 207c 0a7c 205b 5859 4d61 736b 696e 675d   |.| [XYMasking]
-000070f0: 2868 7474 7073 3a2f 2f61 6c62 756d 656e  (https://albumen
-00007100: 7461 7469 6f6e 732e 6169 2f64 6f63 732f  tations.ai/docs/
-00007110: 6170 695f 7265 6665 7265 6e63 652f 6175  api_reference/au
-00007120: 676d 656e 7461 7469 6f6e 732f 6472 6f70  gmentations/drop
-00007130: 6f75 742f 7879 5f6d 6173 6b69 6e67 2f23  out/xy_masking/#
-00007140: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
-00007150: 7567 6d65 6e74 6174 696f 6e73 2e64 726f  ugmentations.dro
-00007160: 706f 7574 2e78 795f 6d61 736b 696e 672e  pout.xy_masking.
-00007170: 5859 4d61 736b 696e 6729 2020 2020 2020  XYMasking)      
-00007180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007190: 2020 2020 207c 20e2 9c93 2020 2020 207c       | ...     |
-000071a0: 20e2 9c93 2020 2020 7c20 2020 2020 2020   ...    |       
-000071b0: 207c 20e2 9c93 2020 2020 2020 2020 207c   | ...         |
-000071c0: 0a0a 2323 2320 4d69 7869 6e67 2d6c 6576  ..### Mixing-lev
-000071d0: 656c 2074 7261 6e73 666f 726d 730a 0a54  el transforms..T
-000071e0: 7261 6e73 666f 726d 7320 7468 6174 206d  ransforms that m
-000071f0: 6978 2073 6576 6572 616c 2069 6d61 6765  ix several image
-00007200: 7320 696e 746f 206f 6e65 0a0a 7c20 5472  s into one..| Tr
-00007210: 616e 7366 6f72 6d20 2020 2020 2020 2020  ansform         
-00007220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007290: 2020 2020 2020 2020 2020 7c20 496d 6167            | Imag
-000072a0: 6520 7c20 4d61 736b 207c 2042 426f 7865  e | Mask | BBoxe
-000072b0: 7320 7c20 4b65 7970 6f69 6e74 7320 7c20  s | Keypoints | 
-000072c0: 476c 6f62 616c 204c 6162 656c 207c 0a7c  Global Label |.|
-000072d0: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
-000072e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000072f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007300: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007310: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007320: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007330: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007340: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007350: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c 203a  ------------ | :
-00007360: 2d2d 2d3a 207c 203a 2d2d 3a20 7c20 3a2d  ---: | :--: | :-
-00007370: 2d2d 2d3a 207c 203a 2d2d 2d2d 2d2d 2d3a  ---: | :-------:
-00007380: 207c 203a 2d2d 2d2d 2d2d 2d2d 2d2d 3a20   | :----------: 
-00007390: 7c0a 7c20 5b4d 6978 5570 5d28 6874 7470  |.| [MixUp](http
-000073a0: 733a 2f2f 616c 6275 6d65 6e74 6174 696f  s://albumentatio
-000073b0: 6e73 2e61 692f 646f 6373 2f61 7069 5f72  ns.ai/docs/api_r
-000073c0: 6566 6572 656e 6365 2f61 7567 6d65 6e74  eference/augment
-000073d0: 6174 696f 6e73 2f6d 6978 696e 672f 7472  ations/mixing/tr
-000073e0: 616e 7366 6f72 6d73 2f23 616c 6275 6d65  ansforms/#albume
-000073f0: 6e74 6174 696f 6e73 2e61 7567 6d65 6e74  ntations.augment
-00007400: 6174 696f 6e73 2e6d 6978 696e 672e 7472  ations.mixing.tr
-00007410: 616e 7366 6f72 6d73 2e4d 6978 5570 2920  ansforms.MixUp) 
-00007420: 7c20 e29c 9320 2020 2020 7c20 e29c 9320  | ...     | ... 
-00007430: 2020 207c 2020 2020 2020 2020 7c20 2020     |        |   
-00007440: 2020 2020 2020 2020 7c20 e29c 9320 2020          | ...   
-00007450: 2020 2020 2020 2020 207c 0a0a 2323 2041           |..## A
-00007460: 2066 6577 206d 6f72 6520 6578 616d 706c   few more exampl
-00007470: 6573 206f 6620 2a2a 6175 676d 656e 7461  es of **augmenta
-00007480: 7469 6f6e 732a 2a0a 0a23 2323 2053 656d  tions**..### Sem
-00007490: 616e 7469 6320 7365 676d 656e 7461 7469  antic segmentati
-000074a0: 6f6e 206f 6e20 7468 6520 496e 7269 6120  on on the Inria 
-000074b0: 6461 7461 7365 740a 0a21 5b69 6e72 6961  dataset..![inria
-000074c0: 5d28 6874 7470 733a 2f2f 6861 6272 6173  ](https://habras
-000074d0: 746f 7261 6765 2e6f 7267 2f77 6562 742f  torage.org/webt/
-000074e0: 7375 2f77 612f 6e70 2f73 7577 616e 7065  su/wa/np/suwanpe
-000074f0: 6f36 7777 3777 7077 746f 6274 727a 645f  o6ww7wpwtobtrzd_
-00007500: 6367 3230 2e6a 7065 6729 0a0a 2323 2320  cg20.jpeg)..### 
-00007510: 4d65 6469 6361 6c20 696d 6167 696e 670a  Medical imaging.
-00007520: 0a21 5b6d 6564 6963 616c 5d28 6874 7470  .![medical](http
-00007530: 733a 2f2f 6861 6272 6173 746f 7261 6765  s://habrastorage
-00007540: 2e6f 7267 2f77 6562 742f 3169 2f66 692f  .org/webt/1i/fi/
-00007550: 777a 2f31 6966 6977 7a79 306c 7865 7463  wz/1ifiwzy0lxetc
-00007560: 346e 776a 7673 732d 3731 6e6b 7730 2e6a  4nwjvss-71nkw0.j
-00007570: 7065 6729 0a0a 2323 2320 4f62 6a65 6374  peg)..### Object
-00007580: 2064 6574 6563 7469 6f6e 2061 6e64 2073   detection and s
-00007590: 656d 616e 7469 6320 7365 676d 656e 7461  emantic segmenta
-000075a0: 7469 6f6e 206f 6e20 7468 6520 4d61 7069  tion on the Mapi
-000075b0: 6c6c 6172 7920 5669 7374 6173 2064 6174  llary Vistas dat
-000075c0: 6173 6574 0a0a 215b 7669 7374 6173 5d28  aset..![vistas](
-000075d0: 6874 7470 733a 2f2f 6861 6272 6173 746f  https://habrasto
-000075e0: 7261 6765 2e6f 7267 2f77 6562 742f 727a  rage.org/webt/rz
-000075f0: 2f2d 682f 336a 2f72 7a2d 6833 6a61 6c62  /-h/3j/rz-h3jalb
-00007600: 7869 6338 6f5f 6668 7563 7879 7374 7334  xic8o_fhucxysts4
-00007610: 7463 2e6a 7065 6729 0a0a 2323 2320 4b65  tc.jpeg)..### Ke
-00007620: 7970 6f69 6e74 7320 6175 676d 656e 7461  ypoints augmenta
-00007630: 7469 6f6e 0a0a 3c69 6d67 2073 7263 3d22  tion..<img src="
-00007640: 6874 7470 733a 2f2f 6861 6272 6173 746f  https://habrasto
-00007650: 7261 6765 2e6f 7267 2f77 6562 742f 652d  rage.org/webt/e-
-00007660: 2f36 6b2f 7a2d 2f65 2d36 6b7a 2d66 7567  /6k/z-/e-6kz-fug
-00007670: 7032 6865 616b 336a 7a6e 7333 6263 2d72  p2heak3jzns3bc-r
-00007680: 386f 2e6a 7065 6722 2077 6964 7468 3d31  8o.jpeg" width=1
-00007690: 3030 253e 0a0a 0a23 2320 4265 6e63 686d  00%>...## Benchm
-000076a0: 6172 6b69 6e67 2072 6573 756c 7473 0a0a  arking results..
-000076b0: 546f 2072 756e 2074 6865 2062 656e 6368  To run the bench
-000076c0: 6d61 726b 2079 6f75 7273 656c 662c 2066  mark yourself, f
-000076d0: 6f6c 6c6f 7720 7468 6520 696e 7374 7275  ollow the instru
-000076e0: 6374 696f 6e73 2069 6e20 5b62 656e 6368  ctions in [bench
-000076f0: 6d61 726b 2f52 4541 444d 452e 6d64 5d28  mark/README.md](
-00007700: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00007710: 6f6d 2f61 6c62 756d 656e 7461 7469 6f6e  om/albumentation
-00007720: 732d 7465 616d 2f61 6c62 756d 656e 7461  s-team/albumenta
-00007730: 7469 6f6e 732f 626c 6f62 2f6d 6173 7465  tions/blob/maste
-00007740: 722f 6265 6e63 686d 6172 6b2f 5245 4144  r/benchmark/READ
-00007750: 4d45 2e6d 6429 0a0a 5265 7375 6c74 7320  ME.md)..Results 
-00007760: 666f 7220 7275 6e6e 696e 6720 7468 6520  for running the 
-00007770: 6265 6e63 686d 6172 6b20 6f6e 2074 6865  benchmark on the
-00007780: 2066 6972 7374 2032 3030 3020 696d 6167   first 2000 imag
-00007790: 6573 2066 726f 6d20 7468 6520 496d 6167  es from the Imag
-000077a0: 654e 6574 2076 616c 6964 6174 696f 6e20  eNet validation 
-000077b0: 7365 7420 7573 696e 6720 616e 2041 4d44  set using an AMD
-000077c0: 2052 797a 656e 2054 6872 6561 6472 6970   Ryzen Threadrip
-000077d0: 7065 7220 3339 3730 5820 4350 552e 0a41  per 3970X CPU..A
-000077e0: 6c6c 206f 7574 7075 7473 2061 7265 2063  ll outputs are c
-000077f0: 6f6e 7665 7274 6564 2074 6f20 6120 636f  onverted to a co
-00007800: 6e74 6967 756f 7573 204e 756d 5079 2061  ntiguous NumPy a
-00007810: 7272 6179 2077 6974 6820 7468 6520 6e70  rray with the np
-00007820: 2e75 696e 7438 2064 6174 6120 7479 7065  .uint8 data type
-00007830: 2e0a 5468 6520 7461 626c 6520 7368 6f77  ..The table show
-00007840: 7320 686f 7720 6d61 6e79 2069 6d61 6765  s how many image
-00007850: 7320 7065 7220 7365 636f 6e64 2063 616e  s per second can
-00007860: 2062 6520 7072 6f63 6573 7365 6420 6f6e   be processed on
-00007870: 2061 2073 696e 676c 6520 636f 7265 3b20   a single core; 
-00007880: 6869 6768 6572 2069 7320 6265 7474 6572  higher is better
-00007890: 2e0a 0a0a 7c20 2020 2020 2020 2020 2020  ....|           
-000078a0: 2020 2020 2020 2020 2020 207c 616c 6275             |albu
-000078b0: 6d65 6e74 6174 696f 6e73 3c62 723e 3c73  mentations<br><s
-000078c0: 6d61 6c6c 3e31 2e34 2e30 3c2f 736d 616c  mall>1.4.0</smal
-000078d0: 6c3e 7c69 6d67 6175 673c 6272 3e3c 736d  l>|imgaug<br><sm
-000078e0: 616c 6c3e 302e 342e 303c 2f73 6d61 6c6c  all>0.4.0</small
-000078f0: 3e7c 746f 7263 6876 6973 696f 6e3c 6272  >|torchvision<br
-00007900: 3e3c 736d 616c 6c3e 302e 3137 2e30 3c2f  ><small>0.17.0</
-00007910: 736d 616c 6c3e 7c6b 6572 6173 3c62 723e  small>|keras<br>
-00007920: 3c73 6d61 6c6c 3e32 2e31 352e 303c 2f73  <small>2.15.0</s
-00007930: 6d61 6c6c 3e7c 6175 676d 656e 746f 723c  mall>|augmentor<
-00007940: 6272 3e3c 736d 616c 6c3e 302e 322e 3132  br><small>0.2.12
-00007950: 3c2f 736d 616c 6c3e 7c73 6f6c 743c 6272  </small>|solt<br
-00007960: 3e3c 736d 616c 6c3e 302e 312e 393c 2f73  ><small>0.1.9</s
-00007970: 6d61 6c6c 3e7c 0a7c 2d2d 2d2d 2d2d 2d2d  mall>|.|--------
-00007980: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d  --------------|-
-00007990: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000079a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000079b0: 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d  -----|----------
-000079c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000079d0: 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----|-----------
-000079e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000079f0: 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d  ---------|------
-00007a00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007a10: 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d  --------|-------
-00007a20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007a30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d  -----------|----
-00007a40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007a50: 2d2d 2d2d 2d2d 2d2d 7c0a 7c48 6f72 697a  --------|.|Horiz
-00007a60: 6f6e 7461 6c46 6c69 7020 2020 2020 2020  ontalFlip       
-00007a70: 207c 2a2a 3134 3831 362a 2a20 2020 2020   |**14816**     
+000035f0: 6e73 666f 726d 732e 4875 6553 6174 7572  nsforms.HueSatur
+00003600: 6174 696f 6e56 616c 7565 290a 2d20 5b49  ationValue).- [I
+00003610: 534f 4e6f 6973 655d 2868 7474 7073 3a2f  SONoise](https:/
+00003620: 2f61 6c62 756d 656e 7461 7469 6f6e 732e  /albumentations.
+00003630: 6169 2f64 6f63 732f 6170 695f 7265 6665  ai/docs/api_refe
+00003640: 7265 6e63 652f 6175 676d 656e 7461 7469  rence/augmentati
+00003650: 6f6e 732f 7472 616e 7366 6f72 6d73 2f23  ons/transforms/#
+00003660: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
+00003670: 7567 6d65 6e74 6174 696f 6e73 2e74 7261  ugmentations.tra
+00003680: 6e73 666f 726d 732e 4953 4f4e 6f69 7365  nsforms.ISONoise
+00003690: 290a 2d20 5b49 6d61 6765 436f 6d70 7265  ).- [ImageCompre
+000036a0: 7373 696f 6e5d 2868 7474 7073 3a2f 2f61  ssion](https://a
+000036b0: 6c62 756d 656e 7461 7469 6f6e 732e 6169  lbumentations.ai
+000036c0: 2f64 6f63 732f 6170 695f 7265 6665 7265  /docs/api_refere
+000036d0: 6e63 652f 6175 676d 656e 7461 7469 6f6e  nce/augmentation
+000036e0: 732f 7472 616e 7366 6f72 6d73 2f23 616c  s/transforms/#al
+000036f0: 6275 6d65 6e74 6174 696f 6e73 2e61 7567  bumentations.aug
+00003700: 6d65 6e74 6174 696f 6e73 2e74 7261 6e73  mentations.trans
+00003710: 666f 726d 732e 496d 6167 6543 6f6d 7072  forms.ImageCompr
+00003720: 6573 7369 6f6e 290a 2d20 5b49 6e76 6572  ession).- [Inver
+00003730: 7449 6d67 5d28 6874 7470 733a 2f2f 616c  tImg](https://al
+00003740: 6275 6d65 6e74 6174 696f 6e73 2e61 692f  bumentations.ai/
+00003750: 646f 6373 2f61 7069 5f72 6566 6572 656e  docs/api_referen
+00003760: 6365 2f61 7567 6d65 6e74 6174 696f 6e73  ce/augmentations
+00003770: 2f74 7261 6e73 666f 726d 732f 2361 6c62  /transforms/#alb
+00003780: 756d 656e 7461 7469 6f6e 732e 6175 676d  umentations.augm
+00003790: 656e 7461 7469 6f6e 732e 7472 616e 7366  entations.transf
+000037a0: 6f72 6d73 2e49 6e76 6572 7449 6d67 290a  orms.InvertImg).
+000037b0: 2d20 5b4d 6564 6961 6e42 6c75 725d 2868  - [MedianBlur](h
+000037c0: 7474 7073 3a2f 2f61 6c62 756d 656e 7461  ttps://albumenta
+000037d0: 7469 6f6e 732e 6169 2f64 6f63 732f 6170  tions.ai/docs/ap
+000037e0: 695f 7265 6665 7265 6e63 652f 6175 676d  i_reference/augm
+000037f0: 656e 7461 7469 6f6e 732f 626c 7572 2f74  entations/blur/t
+00003800: 7261 6e73 666f 726d 732f 2361 6c62 756d  ransforms/#album
+00003810: 656e 7461 7469 6f6e 732e 6175 676d 656e  entations.augmen
+00003820: 7461 7469 6f6e 732e 626c 7572 2e74 7261  tations.blur.tra
+00003830: 6e73 666f 726d 732e 4d65 6469 616e 426c  nsforms.MedianBl
+00003840: 7572 290a 2d20 5b4d 6f74 696f 6e42 6c75  ur).- [MotionBlu
+00003850: 725d 2868 7474 7073 3a2f 2f61 6c62 756d  r](https://album
+00003860: 656e 7461 7469 6f6e 732e 6169 2f64 6f63  entations.ai/doc
+00003870: 732f 6170 695f 7265 6665 7265 6e63 652f  s/api_reference/
+00003880: 6175 676d 656e 7461 7469 6f6e 732f 626c  augmentations/bl
+00003890: 7572 2f74 7261 6e73 666f 726d 732f 2361  ur/transforms/#a
+000038a0: 6c62 756d 656e 7461 7469 6f6e 732e 6175  lbumentations.au
+000038b0: 676d 656e 7461 7469 6f6e 732e 626c 7572  gmentations.blur
+000038c0: 2e74 7261 6e73 666f 726d 732e 4d6f 7469  .transforms.Moti
+000038d0: 6f6e 426c 7572 290a 2d20 5b4d 756c 7469  onBlur).- [Multi
+000038e0: 706c 6963 6174 6976 654e 6f69 7365 5d28  plicativeNoise](
+000038f0: 6874 7470 733a 2f2f 616c 6275 6d65 6e74  https://albument
+00003900: 6174 696f 6e73 2e61 692f 646f 6373 2f61  ations.ai/docs/a
+00003910: 7069 5f72 6566 6572 656e 6365 2f61 7567  pi_reference/aug
+00003920: 6d65 6e74 6174 696f 6e73 2f74 7261 6e73  mentations/trans
+00003930: 666f 726d 732f 2361 6c62 756d 656e 7461  forms/#albumenta
+00003940: 7469 6f6e 732e 6175 676d 656e 7461 7469  tions.augmentati
+00003950: 6f6e 732e 7472 616e 7366 6f72 6d73 2e4d  ons.transforms.M
+00003960: 756c 7469 706c 6963 6174 6976 654e 6f69  ultiplicativeNoi
+00003970: 7365 290a 2d20 5b4e 6f72 6d61 6c69 7a65  se).- [Normalize
+00003980: 5d28 6874 7470 733a 2f2f 616c 6275 6d65  ](https://albume
+00003990: 6e74 6174 696f 6e73 2e61 692f 646f 6373  ntations.ai/docs
+000039a0: 2f61 7069 5f72 6566 6572 656e 6365 2f61  /api_reference/a
+000039b0: 7567 6d65 6e74 6174 696f 6e73 2f74 7261  ugmentations/tra
+000039c0: 6e73 666f 726d 732f 2361 6c62 756d 656e  nsforms/#albumen
+000039d0: 7461 7469 6f6e 732e 6175 676d 656e 7461  tations.augmenta
+000039e0: 7469 6f6e 732e 7472 616e 7366 6f72 6d73  tions.transforms
+000039f0: 2e4e 6f72 6d61 6c69 7a65 290a 2d20 5b50  .Normalize).- [P
+00003a00: 6978 656c 4469 7374 7269 6275 7469 6f6e  ixelDistribution
+00003a10: 4164 6170 7461 7469 6f6e 5d28 6874 7470  Adaptation](http
+00003a20: 733a 2f2f 616c 6275 6d65 6e74 6174 696f  s://albumentatio
+00003a30: 6e73 2e61 692f 646f 6373 2f61 7069 5f72  ns.ai/docs/api_r
+00003a40: 6566 6572 656e 6365 2f61 7567 6d65 6e74  eference/augment
+00003a50: 6174 696f 6e73 2f64 6f6d 6169 6e5f 6164  ations/domain_ad
+00003a60: 6170 7461 7469 6f6e 2f23 616c 6275 6d65  aptation/#albume
+00003a70: 6e74 6174 696f 6e73 2e61 7567 6d65 6e74  ntations.augment
+00003a80: 6174 696f 6e73 2e64 6f6d 6169 6e5f 6164  ations.domain_ad
+00003a90: 6170 7461 7469 6f6e 2e50 6978 656c 4469  aptation.PixelDi
+00003aa0: 7374 7269 6275 7469 6f6e 4164 6170 7461  stributionAdapta
+00003ab0: 7469 6f6e 290a 2d20 5b50 6f73 7465 7269  tion).- [Posteri
+00003ac0: 7a65 5d28 6874 7470 733a 2f2f 616c 6275  ze](https://albu
+00003ad0: 6d65 6e74 6174 696f 6e73 2e61 692f 646f  mentations.ai/do
+00003ae0: 6373 2f61 7069 5f72 6566 6572 656e 6365  cs/api_reference
+00003af0: 2f61 7567 6d65 6e74 6174 696f 6e73 2f74  /augmentations/t
+00003b00: 7261 6e73 666f 726d 732f 2361 6c62 756d  ransforms/#album
+00003b10: 656e 7461 7469 6f6e 732e 6175 676d 656e  entations.augmen
+00003b20: 7461 7469 6f6e 732e 7472 616e 7366 6f72  tations.transfor
+00003b30: 6d73 2e50 6f73 7465 7269 7a65 290a 2d20  ms.Posterize).- 
+00003b40: 5b52 4742 5368 6966 745d 2868 7474 7073  [RGBShift](https
+00003b50: 3a2f 2f61 6c62 756d 656e 7461 7469 6f6e  ://albumentation
+00003b60: 732e 6169 2f64 6f63 732f 6170 695f 7265  s.ai/docs/api_re
+00003b70: 6665 7265 6e63 652f 6175 676d 656e 7461  ference/augmenta
+00003b80: 7469 6f6e 732f 7472 616e 7366 6f72 6d73  tions/transforms
+00003b90: 2f23 616c 6275 6d65 6e74 6174 696f 6e73  /#albumentations
+00003ba0: 2e61 7567 6d65 6e74 6174 696f 6e73 2e74  .augmentations.t
+00003bb0: 7261 6e73 666f 726d 732e 5247 4253 6869  ransforms.RGBShi
+00003bc0: 6674 290a 2d20 5b52 616e 646f 6d42 7269  ft).- [RandomBri
+00003bd0: 6768 746e 6573 7343 6f6e 7472 6173 745d  ghtnessContrast]
+00003be0: 2868 7474 7073 3a2f 2f61 6c62 756d 656e  (https://albumen
+00003bf0: 7461 7469 6f6e 732e 6169 2f64 6f63 732f  tations.ai/docs/
+00003c00: 6170 695f 7265 6665 7265 6e63 652f 6175  api_reference/au
+00003c10: 676d 656e 7461 7469 6f6e 732f 7472 616e  gmentations/tran
+00003c20: 7366 6f72 6d73 2f23 616c 6275 6d65 6e74  sforms/#albument
+00003c30: 6174 696f 6e73 2e61 7567 6d65 6e74 6174  ations.augmentat
+00003c40: 696f 6e73 2e74 7261 6e73 666f 726d 732e  ions.transforms.
+00003c50: 5261 6e64 6f6d 4272 6967 6874 6e65 7373  RandomBrightness
+00003c60: 436f 6e74 7261 7374 290a 2d20 5b52 616e  Contrast).- [Ran
+00003c70: 646f 6d46 6f67 5d28 6874 7470 733a 2f2f  domFog](https://
+00003c80: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
+00003c90: 692f 646f 6373 2f61 7069 5f72 6566 6572  i/docs/api_refer
+00003ca0: 656e 6365 2f61 7567 6d65 6e74 6174 696f  ence/augmentatio
+00003cb0: 6e73 2f74 7261 6e73 666f 726d 732f 2361  ns/transforms/#a
+00003cc0: 6c62 756d 656e 7461 7469 6f6e 732e 6175  lbumentations.au
+00003cd0: 676d 656e 7461 7469 6f6e 732e 7472 616e  gmentations.tran
+00003ce0: 7366 6f72 6d73 2e52 616e 646f 6d46 6f67  sforms.RandomFog
+00003cf0: 290a 2d20 5b52 616e 646f 6d47 616d 6d61  ).- [RandomGamma
+00003d00: 5d28 6874 7470 733a 2f2f 616c 6275 6d65  ](https://albume
+00003d10: 6e74 6174 696f 6e73 2e61 692f 646f 6373  ntations.ai/docs
+00003d20: 2f61 7069 5f72 6566 6572 656e 6365 2f61  /api_reference/a
+00003d30: 7567 6d65 6e74 6174 696f 6e73 2f74 7261  ugmentations/tra
+00003d40: 6e73 666f 726d 732f 2361 6c62 756d 656e  nsforms/#albumen
+00003d50: 7461 7469 6f6e 732e 6175 676d 656e 7461  tations.augmenta
+00003d60: 7469 6f6e 732e 7472 616e 7366 6f72 6d73  tions.transforms
+00003d70: 2e52 616e 646f 6d47 616d 6d61 290a 2d20  .RandomGamma).- 
+00003d80: 5b52 616e 646f 6d47 7261 7665 6c5d 2868  [RandomGravel](h
+00003d90: 7474 7073 3a2f 2f61 6c62 756d 656e 7461  ttps://albumenta
+00003da0: 7469 6f6e 732e 6169 2f64 6f63 732f 6170  tions.ai/docs/ap
+00003db0: 695f 7265 6665 7265 6e63 652f 6175 676d  i_reference/augm
+00003dc0: 656e 7461 7469 6f6e 732f 7472 616e 7366  entations/transf
+00003dd0: 6f72 6d73 2f23 616c 6275 6d65 6e74 6174  orms/#albumentat
+00003de0: 696f 6e73 2e61 7567 6d65 6e74 6174 696f  ions.augmentatio
+00003df0: 6e73 2e74 7261 6e73 666f 726d 732e 5261  ns.transforms.Ra
+00003e00: 6e64 6f6d 4772 6176 656c 290a 2d20 5b52  ndomGravel).- [R
+00003e10: 616e 646f 6d52 6169 6e5d 2868 7474 7073  andomRain](https
+00003e20: 3a2f 2f61 6c62 756d 656e 7461 7469 6f6e  ://albumentation
+00003e30: 732e 6169 2f64 6f63 732f 6170 695f 7265  s.ai/docs/api_re
+00003e40: 6665 7265 6e63 652f 6175 676d 656e 7461  ference/augmenta
+00003e50: 7469 6f6e 732f 7472 616e 7366 6f72 6d73  tions/transforms
+00003e60: 2f23 616c 6275 6d65 6e74 6174 696f 6e73  /#albumentations
+00003e70: 2e61 7567 6d65 6e74 6174 696f 6e73 2e74  .augmentations.t
+00003e80: 7261 6e73 666f 726d 732e 5261 6e64 6f6d  ransforms.Random
+00003e90: 5261 696e 290a 2d20 5b52 616e 646f 6d53  Rain).- [RandomS
+00003ea0: 6861 646f 775d 2868 7474 7073 3a2f 2f61  hadow](https://a
+00003eb0: 6c62 756d 656e 7461 7469 6f6e 732e 6169  lbumentations.ai
+00003ec0: 2f64 6f63 732f 6170 695f 7265 6665 7265  /docs/api_refere
+00003ed0: 6e63 652f 6175 676d 656e 7461 7469 6f6e  nce/augmentation
+00003ee0: 732f 7472 616e 7366 6f72 6d73 2f23 616c  s/transforms/#al
+00003ef0: 6275 6d65 6e74 6174 696f 6e73 2e61 7567  bumentations.aug
+00003f00: 6d65 6e74 6174 696f 6e73 2e74 7261 6e73  mentations.trans
+00003f10: 666f 726d 732e 5261 6e64 6f6d 5368 6164  forms.RandomShad
+00003f20: 6f77 290a 2d20 5b52 616e 646f 6d53 6e6f  ow).- [RandomSno
+00003f30: 775d 2868 7474 7073 3a2f 2f61 6c62 756d  w](https://album
+00003f40: 656e 7461 7469 6f6e 732e 6169 2f64 6f63  entations.ai/doc
+00003f50: 732f 6170 695f 7265 6665 7265 6e63 652f  s/api_reference/
+00003f60: 6175 676d 656e 7461 7469 6f6e 732f 7472  augmentations/tr
+00003f70: 616e 7366 6f72 6d73 2f23 616c 6275 6d65  ansforms/#albume
+00003f80: 6e74 6174 696f 6e73 2e61 7567 6d65 6e74  ntations.augment
+00003f90: 6174 696f 6e73 2e74 7261 6e73 666f 726d  ations.transform
+00003fa0: 732e 5261 6e64 6f6d 536e 6f77 290a 2d20  s.RandomSnow).- 
+00003fb0: 5b52 616e 646f 6d53 756e 466c 6172 655d  [RandomSunFlare]
+00003fc0: 2868 7474 7073 3a2f 2f61 6c62 756d 656e  (https://albumen
+00003fd0: 7461 7469 6f6e 732e 6169 2f64 6f63 732f  tations.ai/docs/
+00003fe0: 6170 695f 7265 6665 7265 6e63 652f 6175  api_reference/au
+00003ff0: 676d 656e 7461 7469 6f6e 732f 7472 616e  gmentations/tran
+00004000: 7366 6f72 6d73 2f23 616c 6275 6d65 6e74  sforms/#albument
+00004010: 6174 696f 6e73 2e61 7567 6d65 6e74 6174  ations.augmentat
+00004020: 696f 6e73 2e74 7261 6e73 666f 726d 732e  ions.transforms.
+00004030: 5261 6e64 6f6d 5375 6e46 6c61 7265 290a  RandomSunFlare).
+00004040: 2d20 5b52 616e 646f 6d54 6f6e 6543 7572  - [RandomToneCur
+00004050: 7665 5d28 6874 7470 733a 2f2f 616c 6275  ve](https://albu
+00004060: 6d65 6e74 6174 696f 6e73 2e61 692f 646f  mentations.ai/do
+00004070: 6373 2f61 7069 5f72 6566 6572 656e 6365  cs/api_reference
+00004080: 2f61 7567 6d65 6e74 6174 696f 6e73 2f74  /augmentations/t
+00004090: 7261 6e73 666f 726d 732f 2361 6c62 756d  ransforms/#album
+000040a0: 656e 7461 7469 6f6e 732e 6175 676d 656e  entations.augmen
+000040b0: 7461 7469 6f6e 732e 7472 616e 7366 6f72  tations.transfor
+000040c0: 6d73 2e52 616e 646f 6d54 6f6e 6543 7572  ms.RandomToneCur
+000040d0: 7665 290a 2d20 5b52 696e 6769 6e67 4f76  ve).- [RingingOv
+000040e0: 6572 7368 6f6f 745d 2868 7474 7073 3a2f  ershoot](https:/
+000040f0: 2f61 6c62 756d 656e 7461 7469 6f6e 732e  /albumentations.
+00004100: 6169 2f64 6f63 732f 6170 695f 7265 6665  ai/docs/api_refe
+00004110: 7265 6e63 652f 6175 676d 656e 7461 7469  rence/augmentati
+00004120: 6f6e 732f 7472 616e 7366 6f72 6d73 2f23  ons/transforms/#
+00004130: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
+00004140: 7567 6d65 6e74 6174 696f 6e73 2e74 7261  ugmentations.tra
+00004150: 6e73 666f 726d 732e 5269 6e67 696e 674f  nsforms.RingingO
+00004160: 7665 7273 686f 6f74 290a 2d20 5b53 6861  vershoot).- [Sha
+00004170: 7270 656e 5d28 6874 7470 733a 2f2f 616c  rpen](https://al
+00004180: 6275 6d65 6e74 6174 696f 6e73 2e61 692f  bumentations.ai/
+00004190: 646f 6373 2f61 7069 5f72 6566 6572 656e  docs/api_referen
+000041a0: 6365 2f61 7567 6d65 6e74 6174 696f 6e73  ce/augmentations
+000041b0: 2f74 7261 6e73 666f 726d 732f 2361 6c62  /transforms/#alb
+000041c0: 756d 656e 7461 7469 6f6e 732e 6175 676d  umentations.augm
+000041d0: 656e 7461 7469 6f6e 732e 7472 616e 7366  entations.transf
+000041e0: 6f72 6d73 2e53 6861 7270 656e 290a 2d20  orms.Sharpen).- 
+000041f0: 5b53 6f6c 6172 697a 655d 2868 7474 7073  [Solarize](https
+00004200: 3a2f 2f61 6c62 756d 656e 7461 7469 6f6e  ://albumentation
+00004210: 732e 6169 2f64 6f63 732f 6170 695f 7265  s.ai/docs/api_re
+00004220: 6665 7265 6e63 652f 6175 676d 656e 7461  ference/augmenta
+00004230: 7469 6f6e 732f 7472 616e 7366 6f72 6d73  tions/transforms
+00004240: 2f23 616c 6275 6d65 6e74 6174 696f 6e73  /#albumentations
+00004250: 2e61 7567 6d65 6e74 6174 696f 6e73 2e74  .augmentations.t
+00004260: 7261 6e73 666f 726d 732e 536f 6c61 7269  ransforms.Solari
+00004270: 7a65 290a 2d20 5b53 7061 7474 6572 5d28  ze).- [Spatter](
+00004280: 6874 7470 733a 2f2f 616c 6275 6d65 6e74  https://albument
+00004290: 6174 696f 6e73 2e61 692f 646f 6373 2f61  ations.ai/docs/a
+000042a0: 7069 5f72 6566 6572 656e 6365 2f61 7567  pi_reference/aug
+000042b0: 6d65 6e74 6174 696f 6e73 2f74 7261 6e73  mentations/trans
+000042c0: 666f 726d 732f 2361 6c62 756d 656e 7461  forms/#albumenta
+000042d0: 7469 6f6e 732e 6175 676d 656e 7461 7469  tions.augmentati
+000042e0: 6f6e 732e 7472 616e 7366 6f72 6d73 2e53  ons.transforms.S
+000042f0: 7061 7474 6572 290a 2d20 5b53 7570 6572  patter).- [Super
+00004300: 7069 7865 6c73 5d28 6874 7470 733a 2f2f  pixels](https://
+00004310: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
+00004320: 692f 646f 6373 2f61 7069 5f72 6566 6572  i/docs/api_refer
+00004330: 656e 6365 2f61 7567 6d65 6e74 6174 696f  ence/augmentatio
+00004340: 6e73 2f74 7261 6e73 666f 726d 732f 2361  ns/transforms/#a
+00004350: 6c62 756d 656e 7461 7469 6f6e 732e 6175  lbumentations.au
+00004360: 676d 656e 7461 7469 6f6e 732e 7472 616e  gmentations.tran
+00004370: 7366 6f72 6d73 2e53 7570 6572 7069 7865  sforms.Superpixe
+00004380: 6c73 290a 2d20 5b54 656d 706c 6174 6554  ls).- [TemplateT
+00004390: 7261 6e73 666f 726d 5d28 6874 7470 733a  ransform](https:
+000043a0: 2f2f 616c 6275 6d65 6e74 6174 696f 6e73  //albumentations
+000043b0: 2e61 692f 646f 6373 2f61 7069 5f72 6566  .ai/docs/api_ref
+000043c0: 6572 656e 6365 2f61 7567 6d65 6e74 6174  erence/augmentat
+000043d0: 696f 6e73 2f74 7261 6e73 666f 726d 732f  ions/transforms/
+000043e0: 2361 6c62 756d 656e 7461 7469 6f6e 732e  #albumentations.
+000043f0: 6175 676d 656e 7461 7469 6f6e 732e 7472  augmentations.tr
+00004400: 616e 7366 6f72 6d73 2e54 656d 706c 6174  ansforms.Templat
+00004410: 6554 7261 6e73 666f 726d 290a 2d20 5b54  eTransform).- [T
+00004420: 6f46 6c6f 6174 5d28 6874 7470 733a 2f2f  oFloat](https://
+00004430: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
+00004440: 692f 646f 6373 2f61 7069 5f72 6566 6572  i/docs/api_refer
+00004450: 656e 6365 2f61 7567 6d65 6e74 6174 696f  ence/augmentatio
+00004460: 6e73 2f74 7261 6e73 666f 726d 732f 2361  ns/transforms/#a
+00004470: 6c62 756d 656e 7461 7469 6f6e 732e 6175  lbumentations.au
+00004480: 676d 656e 7461 7469 6f6e 732e 7472 616e  gmentations.tran
+00004490: 7366 6f72 6d73 2e54 6f46 6c6f 6174 290a  sforms.ToFloat).
+000044a0: 2d20 5b54 6f47 7261 795d 2868 7474 7073  - [ToGray](https
+000044b0: 3a2f 2f61 6c62 756d 656e 7461 7469 6f6e  ://albumentation
+000044c0: 732e 6169 2f64 6f63 732f 6170 695f 7265  s.ai/docs/api_re
+000044d0: 6665 7265 6e63 652f 6175 676d 656e 7461  ference/augmenta
+000044e0: 7469 6f6e 732f 7472 616e 7366 6f72 6d73  tions/transforms
+000044f0: 2f23 616c 6275 6d65 6e74 6174 696f 6e73  /#albumentations
+00004500: 2e61 7567 6d65 6e74 6174 696f 6e73 2e74  .augmentations.t
+00004510: 7261 6e73 666f 726d 732e 546f 4772 6179  ransforms.ToGray
+00004520: 290a 2d20 5b54 6f52 4742 5d28 6874 7470  ).- [ToRGB](http
+00004530: 733a 2f2f 616c 6275 6d65 6e74 6174 696f  s://albumentatio
+00004540: 6e73 2e61 692f 646f 6373 2f61 7069 5f72  ns.ai/docs/api_r
+00004550: 6566 6572 656e 6365 2f61 7567 6d65 6e74  eference/augment
+00004560: 6174 696f 6e73 2f74 7261 6e73 666f 726d  ations/transform
+00004570: 732f 2361 6c62 756d 656e 7461 7469 6f6e  s/#albumentation
+00004580: 732e 6175 676d 656e 7461 7469 6f6e 732e  s.augmentations.
+00004590: 7472 616e 7366 6f72 6d73 2e54 6f52 4742  transforms.ToRGB
+000045a0: 290a 2d20 5b54 6f53 6570 6961 5d28 6874  ).- [ToSepia](ht
+000045b0: 7470 733a 2f2f 616c 6275 6d65 6e74 6174  tps://albumentat
+000045c0: 696f 6e73 2e61 692f 646f 6373 2f61 7069  ions.ai/docs/api
+000045d0: 5f72 6566 6572 656e 6365 2f61 7567 6d65  _reference/augme
+000045e0: 6e74 6174 696f 6e73 2f74 7261 6e73 666f  ntations/transfo
+000045f0: 726d 732f 2361 6c62 756d 656e 7461 7469  rms/#albumentati
+00004600: 6f6e 732e 6175 676d 656e 7461 7469 6f6e  ons.augmentation
+00004610: 732e 7472 616e 7366 6f72 6d73 2e54 6f53  s.transforms.ToS
+00004620: 6570 6961 290a 2d20 5b55 6e73 6861 7270  epia).- [Unsharp
+00004630: 4d61 736b 5d28 6874 7470 733a 2f2f 616c  Mask](https://al
+00004640: 6275 6d65 6e74 6174 696f 6e73 2e61 692f  bumentations.ai/
+00004650: 646f 6373 2f61 7069 5f72 6566 6572 656e  docs/api_referen
+00004660: 6365 2f61 7567 6d65 6e74 6174 696f 6e73  ce/augmentations
+00004670: 2f74 7261 6e73 666f 726d 732f 2361 6c62  /transforms/#alb
+00004680: 756d 656e 7461 7469 6f6e 732e 6175 676d  umentations.augm
+00004690: 656e 7461 7469 6f6e 732e 7472 616e 7366  entations.transf
+000046a0: 6f72 6d73 2e55 6e73 6861 7270 4d61 736b  orms.UnsharpMask
+000046b0: 290a 2d20 5b5a 6f6f 6d42 6c75 725d 2868  ).- [ZoomBlur](h
+000046c0: 7474 7073 3a2f 2f61 6c62 756d 656e 7461  ttps://albumenta
+000046d0: 7469 6f6e 732e 6169 2f64 6f63 732f 6170  tions.ai/docs/ap
+000046e0: 695f 7265 6665 7265 6e63 652f 6175 676d  i_reference/augm
+000046f0: 656e 7461 7469 6f6e 732f 626c 7572 2f74  entations/blur/t
+00004700: 7261 6e73 666f 726d 732f 2361 6c62 756d  ransforms/#album
+00004710: 656e 7461 7469 6f6e 732e 6175 676d 656e  entations.augmen
+00004720: 7461 7469 6f6e 732e 626c 7572 2e74 7261  tations.blur.tra
+00004730: 6e73 666f 726d 732e 5a6f 6f6d 426c 7572  nsforms.ZoomBlur
+00004740: 290a 0a23 2323 2053 7061 7469 616c 2d6c  )..### Spatial-l
+00004750: 6576 656c 2074 7261 6e73 666f 726d 730a  evel transforms.
+00004760: 0a53 7061 7469 616c 2d6c 6576 656c 2074  .Spatial-level t
+00004770: 7261 6e73 666f 726d 7320 7769 6c6c 2073  ransforms will s
+00004780: 696d 756c 7461 6e65 6f75 736c 7920 6368  imultaneously ch
+00004790: 616e 6765 2062 6f74 6820 616e 2069 6e70  ange both an inp
+000047a0: 7574 2069 6d61 6765 2061 7320 7765 6c6c  ut image as well
+000047b0: 2061 7320 6164 6469 7469 6f6e 616c 2074   as additional t
+000047c0: 6172 6765 7473 2073 7563 6820 6173 206d  argets such as m
+000047d0: 6173 6b73 2c20 626f 756e 6469 6e67 2062  asks, bounding b
+000047e0: 6f78 6573 2c20 616e 6420 6b65 7970 6f69  oxes, and keypoi
+000047f0: 6e74 732e 2054 6865 2066 6f6c 6c6f 7769  nts. The followi
+00004800: 6e67 2074 6162 6c65 2073 686f 7773 2077  ng table shows w
+00004810: 6869 6368 2061 6464 6974 696f 6e61 6c20  hich additional 
+00004820: 7461 7267 6574 7320 6172 6520 7375 7070  targets are supp
+00004830: 6f72 7465 6420 6279 2065 6163 6820 7472  orted by each tr
+00004840: 616e 7366 6f72 6d2e 0a0a 7c20 5472 616e  ansform...| Tran
+00004850: 7366 6f72 6d20 2020 2020 2020 2020 2020  sform           
+00004860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000048a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000048b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000048c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000048d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000048e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000048f0: 2020 2020 2020 2020 2020 2020 7c20 496d              | Im
+00004900: 6167 6520 7c20 4d61 736b 207c 2042 426f  age | Mask | BBo
+00004910: 7865 7320 7c20 4b65 7970 6f69 6e74 7320  xes | Keypoints 
+00004920: 7c0a 7c20 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |.| ------------
+00004930: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004940: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004950: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004960: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004970: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004980: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004990: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000049a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000049b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000049c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000049d0: 2d2d 2d20 7c20 3a2d 2d2d 3a20 7c20 3a2d  --- | :---: | :-
+000049e0: 2d3a 207c 203a 2d2d 2d2d 3a20 7c20 3a2d  -: | :----: | :-
+000049f0: 2d2d 2d2d 2d2d 3a20 7c0a 7c20 5b41 6666  ------: |.| [Aff
+00004a00: 696e 655d 2868 7474 7073 3a2f 2f61 6c62  ine](https://alb
+00004a10: 756d 656e 7461 7469 6f6e 732e 6169 2f64  umentations.ai/d
+00004a20: 6f63 732f 6170 695f 7265 6665 7265 6e63  ocs/api_referenc
+00004a30: 652f 6175 676d 656e 7461 7469 6f6e 732f  e/augmentations/
+00004a40: 6765 6f6d 6574 7269 632f 7472 616e 7366  geometric/transf
+00004a50: 6f72 6d73 2f23 616c 6275 6d65 6e74 6174  orms/#albumentat
+00004a60: 696f 6e73 2e61 7567 6d65 6e74 6174 696f  ions.augmentatio
+00004a70: 6e73 2e67 656f 6d65 7472 6963 2e74 7261  ns.geometric.tra
+00004a80: 6e73 666f 726d 732e 4166 6669 6e65 2920  nsforms.Affine) 
+00004a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004aa0: 2020 2020 2020 2020 2020 2020 7c20 e29c              | ..
+00004ab0: 9320 2020 2020 7c20 e29c 9320 2020 207c  .     | ...    |
+00004ac0: 20e2 9c93 2020 2020 2020 7c20 e29c 9320   ...      | ... 
+00004ad0: 2020 2020 2020 2020 7c0a 7c20 5b42 426f          |.| [BBo
+00004ae0: 7853 6166 6552 616e 646f 6d43 726f 705d  xSafeRandomCrop]
+00004af0: 2868 7474 7073 3a2f 2f61 6c62 756d 656e  (https://albumen
+00004b00: 7461 7469 6f6e 732e 6169 2f64 6f63 732f  tations.ai/docs/
+00004b10: 6170 695f 7265 6665 7265 6e63 652f 6175  api_reference/au
+00004b20: 676d 656e 7461 7469 6f6e 732f 6372 6f70  gmentations/crop
+00004b30: 732f 7472 616e 7366 6f72 6d73 2f23 616c  s/transforms/#al
+00004b40: 6275 6d65 6e74 6174 696f 6e73 2e61 7567  bumentations.aug
+00004b50: 6d65 6e74 6174 696f 6e73 2e63 726f 7073  mentations.crops
+00004b60: 2e74 7261 6e73 666f 726d 732e 4242 6f78  .transforms.BBox
+00004b70: 5361 6665 5261 6e64 6f6d 4372 6f70 2920  SafeRandomCrop) 
+00004b80: 2020 2020 2020 2020 2020 2020 7c20 e29c              | ..
+00004b90: 9320 2020 2020 7c20 e29c 9320 2020 207c  .     | ...    |
+00004ba0: 20e2 9c93 2020 2020 2020 7c20 2020 2020   ...      |     
+00004bb0: 2020 2020 2020 7c0a 7c20 5b43 656e 7465        |.| [Cente
+00004bc0: 7243 726f 705d 2868 7474 7073 3a2f 2f61  rCrop](https://a
+00004bd0: 6c62 756d 656e 7461 7469 6f6e 732e 6169  lbumentations.ai
+00004be0: 2f64 6f63 732f 6170 695f 7265 6665 7265  /docs/api_refere
+00004bf0: 6e63 652f 6175 676d 656e 7461 7469 6f6e  nce/augmentation
+00004c00: 732f 6372 6f70 732f 7472 616e 7366 6f72  s/crops/transfor
+00004c10: 6d73 2f23 616c 6275 6d65 6e74 6174 696f  ms/#albumentatio
+00004c20: 6e73 2e61 7567 6d65 6e74 6174 696f 6e73  ns.augmentations
+00004c30: 2e63 726f 7073 2e74 7261 6e73 666f 726d  .crops.transform
+00004c40: 732e 4365 6e74 6572 4372 6f70 2920 2020  s.CenterCrop)   
+00004c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c60: 2020 2020 2020 2020 2020 7c20 e29c 9320            | ... 
+00004c70: 2020 2020 7c20 e29c 9320 2020 207c 20e2      | ...    | .
+00004c80: 9c93 2020 2020 2020 7c20 e29c 9320 2020  ..      | ...   
+00004c90: 2020 2020 2020 7c0a 7c20 5b43 6f61 7273        |.| [Coars
+00004ca0: 6544 726f 706f 7574 5d28 6874 7470 733a  eDropout](https:
+00004cb0: 2f2f 616c 6275 6d65 6e74 6174 696f 6e73  //albumentations
+00004cc0: 2e61 692f 646f 6373 2f61 7069 5f72 6566  .ai/docs/api_ref
+00004cd0: 6572 656e 6365 2f61 7567 6d65 6e74 6174  erence/augmentat
+00004ce0: 696f 6e73 2f64 726f 706f 7574 2f63 6f61  ions/dropout/coa
+00004cf0: 7273 655f 6472 6f70 6f75 742f 2361 6c62  rse_dropout/#alb
+00004d00: 756d 656e 7461 7469 6f6e 732e 6175 676d  umentations.augm
+00004d10: 656e 7461 7469 6f6e 732e 6472 6f70 6f75  entations.dropou
+00004d20: 742e 636f 6172 7365 5f64 726f 706f 7574  t.coarse_dropout
+00004d30: 2e43 6f61 7273 6544 726f 706f 7574 2920  .CoarseDropout) 
+00004d40: 2020 2020 2020 2020 2020 7c20 e29c 9320            | ... 
+00004d50: 2020 2020 7c20 e29c 9320 2020 207c 2020      | ...    |  
+00004d60: 2020 2020 2020 7c20 e29c 9320 2020 2020        | ...     
+00004d70: 2020 2020 7c0a 7c20 5b43 726f 705d 2868      |.| [Crop](h
+00004d80: 7474 7073 3a2f 2f61 6c62 756d 656e 7461  ttps://albumenta
+00004d90: 7469 6f6e 732e 6169 2f64 6f63 732f 6170  tions.ai/docs/ap
+00004da0: 695f 7265 6665 7265 6e63 652f 6175 676d  i_reference/augm
+00004db0: 656e 7461 7469 6f6e 732f 6372 6f70 732f  entations/crops/
+00004dc0: 7472 616e 7366 6f72 6d73 2f23 616c 6275  transforms/#albu
+00004dd0: 6d65 6e74 6174 696f 6e73 2e61 7567 6d65  mentations.augme
+00004de0: 6e74 6174 696f 6e73 2e63 726f 7073 2e74  ntations.crops.t
+00004df0: 7261 6e73 666f 726d 732e 4372 6f70 2920  ransforms.Crop) 
+00004e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e20: 2020 2020 2020 2020 7c20 e29c 9320 2020          | ...   
+00004e30: 2020 7c20 e29c 9320 2020 207c 20e2 9c93    | ...    | ...
+00004e40: 2020 2020 2020 7c20 e29c 9320 2020 2020        | ...     
+00004e50: 2020 2020 7c0a 7c20 5b43 726f 7041 6e64      |.| [CropAnd
+00004e60: 5061 645d 2868 7474 7073 3a2f 2f61 6c62  Pad](https://alb
+00004e70: 756d 656e 7461 7469 6f6e 732e 6169 2f64  umentations.ai/d
+00004e80: 6f63 732f 6170 695f 7265 6665 7265 6e63  ocs/api_referenc
+00004e90: 652f 6175 676d 656e 7461 7469 6f6e 732f  e/augmentations/
+00004ea0: 6372 6f70 732f 7472 616e 7366 6f72 6d73  crops/transforms
+00004eb0: 2f23 616c 6275 6d65 6e74 6174 696f 6e73  /#albumentations
+00004ec0: 2e61 7567 6d65 6e74 6174 696f 6e73 2e63  .augmentations.c
+00004ed0: 726f 7073 2e74 7261 6e73 666f 726d 732e  rops.transforms.
+00004ee0: 4372 6f70 416e 6450 6164 2920 2020 2020  CropAndPad)     
+00004ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004f00: 2020 2020 2020 2020 7c20 e29c 9320 2020          | ...   
+00004f10: 2020 7c20 e29c 9320 2020 207c 20e2 9c93    | ...    | ...
+00004f20: 2020 2020 2020 7c20 e29c 9320 2020 2020        | ...     
+00004f30: 2020 2020 7c0a 7c20 5b43 726f 704e 6f6e      |.| [CropNon
+00004f40: 456d 7074 794d 6173 6b49 6645 7869 7374  EmptyMaskIfExist
+00004f50: 735d 2868 7474 7073 3a2f 2f61 6c62 756d  s](https://album
+00004f60: 656e 7461 7469 6f6e 732e 6169 2f64 6f63  entations.ai/doc
+00004f70: 732f 6170 695f 7265 6665 7265 6e63 652f  s/api_reference/
+00004f80: 6175 676d 656e 7461 7469 6f6e 732f 6372  augmentations/cr
+00004f90: 6f70 732f 7472 616e 7366 6f72 6d73 2f23  ops/transforms/#
+00004fa0: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
+00004fb0: 7567 6d65 6e74 6174 696f 6e73 2e63 726f  ugmentations.cro
+00004fc0: 7073 2e74 7261 6e73 666f 726d 732e 4372  ps.transforms.Cr
+00004fd0: 6f70 4e6f 6e45 6d70 7479 4d61 736b 4966  opNonEmptyMaskIf
+00004fe0: 4578 6973 7473 2920 7c20 e29c 9320 2020  Exists) | ...   
+00004ff0: 2020 7c20 e29c 9320 2020 207c 20e2 9c93    | ...    | ...
+00005000: 2020 2020 2020 7c20 e29c 9320 2020 2020        | ...     
+00005010: 2020 2020 7c0a 7c20 5b45 6c61 7374 6963      |.| [Elastic
+00005020: 5472 616e 7366 6f72 6d5d 2868 7474 7073  Transform](https
+00005030: 3a2f 2f61 6c62 756d 656e 7461 7469 6f6e  ://albumentation
+00005040: 732e 6169 2f64 6f63 732f 6170 695f 7265  s.ai/docs/api_re
+00005050: 6665 7265 6e63 652f 6175 676d 656e 7461  ference/augmenta
+00005060: 7469 6f6e 732f 6765 6f6d 6574 7269 632f  tions/geometric/
+00005070: 7472 616e 7366 6f72 6d73 2f23 616c 6275  transforms/#albu
+00005080: 6d65 6e74 6174 696f 6e73 2e61 7567 6d65  mentations.augme
+00005090: 6e74 6174 696f 6e73 2e67 656f 6d65 7472  ntations.geometr
+000050a0: 6963 2e74 7261 6e73 666f 726d 732e 456c  ic.transforms.El
+000050b0: 6173 7469 6354 7261 6e73 666f 726d 2920  asticTransform) 
+000050c0: 2020 2020 2020 2020 7c20 e29c 9320 2020          | ...   
+000050d0: 2020 7c20 e29c 9320 2020 207c 20e2 9c93    | ...    | ...
+000050e0: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
+000050f0: 2020 7c0a 7c20 5b46 6c69 705d 2868 7474    |.| [Flip](htt
+00005100: 7073 3a2f 2f61 6c62 756d 656e 7461 7469  ps://albumentati
+00005110: 6f6e 732e 6169 2f64 6f63 732f 6170 695f  ons.ai/docs/api_
+00005120: 7265 6665 7265 6e63 652f 6175 676d 656e  reference/augmen
+00005130: 7461 7469 6f6e 732f 6765 6f6d 6574 7269  tations/geometri
+00005140: 632f 7472 616e 7366 6f72 6d73 2f23 616c  c/transforms/#al
+00005150: 6275 6d65 6e74 6174 696f 6e73 2e61 7567  bumentations.aug
+00005160: 6d65 6e74 6174 696f 6e73 2e67 656f 6d65  mentations.geome
+00005170: 7472 6963 2e74 7261 6e73 666f 726d 732e  tric.transforms.
+00005180: 466c 6970 2920 2020 2020 2020 2020 2020  Flip)           
+00005190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000051a0: 2020 2020 2020 7c20 e29c 9320 2020 2020        | ...     
+000051b0: 7c20 e29c 9320 2020 207c 20e2 9c93 2020  | ...    | ...  
+000051c0: 2020 2020 7c20 e29c 9320 2020 2020 2020      | ...       
+000051d0: 2020 7c0a 7c20 5b47 7269 6444 6973 746f    |.| [GridDisto
+000051e0: 7274 696f 6e5d 2868 7474 7073 3a2f 2f61  rtion](https://a
+000051f0: 6c62 756d 656e 7461 7469 6f6e 732e 6169  lbumentations.ai
+00005200: 2f64 6f63 732f 6170 695f 7265 6665 7265  /docs/api_refere
+00005210: 6e63 652f 6175 676d 656e 7461 7469 6f6e  nce/augmentation
+00005220: 732f 6765 6f6d 6574 7269 632f 7472 616e  s/geometric/tran
+00005230: 7366 6f72 6d73 2f23 616c 6275 6d65 6e74  sforms/#albument
+00005240: 6174 696f 6e73 2e61 7567 6d65 6e74 6174  ations.augmentat
+00005250: 696f 6e73 2e67 656f 6d65 7472 6963 2e74  ions.geometric.t
+00005260: 7261 6e73 666f 726d 732e 4772 6964 4469  ransforms.GridDi
+00005270: 7374 6f72 7469 6f6e 2920 2020 2020 2020  stortion)       
+00005280: 2020 2020 2020 7c20 e29c 9320 2020 2020        | ...     
+00005290: 7c20 e29c 9320 2020 207c 20e2 9c93 2020  | ...    | ...  
+000052a0: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
+000052b0: 7c0a 7c20 5b47 7269 6444 726f 706f 7574  |.| [GridDropout
+000052c0: 5d28 6874 7470 733a 2f2f 616c 6275 6d65  ](https://albume
+000052d0: 6e74 6174 696f 6e73 2e61 692f 646f 6373  ntations.ai/docs
+000052e0: 2f61 7069 5f72 6566 6572 656e 6365 2f61  /api_reference/a
+000052f0: 7567 6d65 6e74 6174 696f 6e73 2f64 726f  ugmentations/dro
+00005300: 706f 7574 2f67 7269 645f 6472 6f70 6f75  pout/grid_dropou
+00005310: 742f 2361 6c62 756d 656e 7461 7469 6f6e  t/#albumentation
+00005320: 732e 6175 676d 656e 7461 7469 6f6e 732e  s.augmentations.
+00005330: 6472 6f70 6f75 742e 6772 6964 5f64 726f  dropout.grid_dro
+00005340: 706f 7574 2e47 7269 6444 726f 706f 7574  pout.GridDropout
+00005350: 2920 2020 2020 2020 2020 2020 2020 2020  )               
+00005360: 2020 2020 7c20 e29c 9320 2020 2020 7c20      | ...     | 
+00005370: e29c 9320 2020 207c 2020 2020 2020 2020  ...    |        
+00005380: 7c20 2020 2020 2020 2020 2020 7c0a 7c20  |           |.| 
+00005390: 5b48 6f72 697a 6f6e 7461 6c46 6c69 705d  [HorizontalFlip]
+000053a0: 2868 7474 7073 3a2f 2f61 6c62 756d 656e  (https://albumen
+000053b0: 7461 7469 6f6e 732e 6169 2f64 6f63 732f  tations.ai/docs/
+000053c0: 6170 695f 7265 6665 7265 6e63 652f 6175  api_reference/au
+000053d0: 676d 656e 7461 7469 6f6e 732f 6765 6f6d  gmentations/geom
+000053e0: 6574 7269 632f 7472 616e 7366 6f72 6d73  etric/transforms
+000053f0: 2f23 616c 6275 6d65 6e74 6174 696f 6e73  /#albumentations
+00005400: 2e61 7567 6d65 6e74 6174 696f 6e73 2e67  .augmentations.g
+00005410: 656f 6d65 7472 6963 2e74 7261 6e73 666f  eometric.transfo
+00005420: 726d 732e 486f 7269 7a6f 6e74 616c 466c  rms.HorizontalFl
+00005430: 6970 2920 2020 2020 2020 2020 2020 2020  ip)             
+00005440: 7c20 e29c 9320 2020 2020 7c20 e29c 9320  | ...     | ... 
+00005450: 2020 207c 20e2 9c93 2020 2020 2020 7c20     | ...      | 
+00005460: e29c 9320 2020 2020 2020 2020 7c0a 7c20  ...         |.| 
+00005470: 5b4c 616d 6264 615d 2868 7474 7073 3a2f  [Lambda](https:/
+00005480: 2f61 6c62 756d 656e 7461 7469 6f6e 732e  /albumentations.
+00005490: 6169 2f64 6f63 732f 6170 695f 7265 6665  ai/docs/api_refe
+000054a0: 7265 6e63 652f 6175 676d 656e 7461 7469  rence/augmentati
+000054b0: 6f6e 732f 7472 616e 7366 6f72 6d73 2f23  ons/transforms/#
+000054c0: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
+000054d0: 7567 6d65 6e74 6174 696f 6e73 2e74 7261  ugmentations.tra
+000054e0: 6e73 666f 726d 732e 4c61 6d62 6461 2920  nsforms.Lambda) 
+000054f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005520: 7c20 e29c 9320 2020 2020 7c20 e29c 9320  | ...     | ... 
+00005530: 2020 207c 20e2 9c93 2020 2020 2020 7c20     | ...      | 
+00005540: e29c 9320 2020 2020 2020 2020 7c0a 7c20  ...         |.| 
+00005550: 5b4c 6f6e 6765 7374 4d61 7853 697a 655d  [LongestMaxSize]
+00005560: 2868 7474 7073 3a2f 2f61 6c62 756d 656e  (https://albumen
+00005570: 7461 7469 6f6e 732e 6169 2f64 6f63 732f  tations.ai/docs/
+00005580: 6170 695f 7265 6665 7265 6e63 652f 6175  api_reference/au
+00005590: 676d 656e 7461 7469 6f6e 732f 6765 6f6d  gmentations/geom
+000055a0: 6574 7269 632f 7265 7369 7a65 2f23 616c  etric/resize/#al
+000055b0: 6275 6d65 6e74 6174 696f 6e73 2e61 7567  bumentations.aug
+000055c0: 6d65 6e74 6174 696f 6e73 2e67 656f 6d65  mentations.geome
+000055d0: 7472 6963 2e72 6573 697a 652e 4c6f 6e67  tric.resize.Long
+000055e0: 6573 744d 6178 5369 7a65 2920 2020 2020  estMaxSize)     
+000055f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005600: 7c20 e29c 9320 2020 2020 7c20 e29c 9320  | ...     | ... 
+00005610: 2020 207c 20e2 9c93 2020 2020 2020 7c20     | ...      | 
+00005620: e29c 9320 2020 2020 2020 2020 7c0a 7c20  ...         |.| 
+00005630: 5b4d 6173 6b44 726f 706f 7574 5d28 6874  [MaskDropout](ht
+00005640: 7470 733a 2f2f 616c 6275 6d65 6e74 6174  tps://albumentat
+00005650: 696f 6e73 2e61 692f 646f 6373 2f61 7069  ions.ai/docs/api
+00005660: 5f72 6566 6572 656e 6365 2f61 7567 6d65  _reference/augme
+00005670: 6e74 6174 696f 6e73 2f64 726f 706f 7574  ntations/dropout
+00005680: 2f6d 6173 6b5f 6472 6f70 6f75 742f 2361  /mask_dropout/#a
+00005690: 6c62 756d 656e 7461 7469 6f6e 732e 6175  lbumentations.au
+000056a0: 676d 656e 7461 7469 6f6e 732e 6472 6f70  gmentations.drop
+000056b0: 6f75 742e 6d61 736b 5f64 726f 706f 7574  out.mask_dropout
+000056c0: 2e4d 6173 6b44 726f 706f 7574 2920 2020  .MaskDropout)   
+000056d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000056e0: 7c20 e29c 9320 2020 2020 7c20 e29c 9320  | ...     | ... 
+000056f0: 2020 207c 2020 2020 2020 2020 7c20 2020     |        |   
+00005700: 2020 2020 2020 2020 7c0a 7c20 5b4d 6f72          |.| [Mor
+00005710: 7068 6f6c 6f67 6963 616c 5d28 6874 7470  phological](http
+00005720: 733a 2f2f 616c 6275 6d65 6e74 6174 696f  s://albumentatio
+00005730: 6e73 2e61 692f 646f 6373 2f61 7069 5f72  ns.ai/docs/api_r
+00005740: 6566 6572 656e 6365 2f61 7567 6d65 6e74  eference/augment
+00005750: 6174 696f 6e73 2f74 7261 6e73 666f 726d  ations/transform
+00005760: 732f 2361 6c62 756d 656e 7461 7469 6f6e  s/#albumentation
+00005770: 732e 6175 676d 656e 7461 7469 6f6e 732e  s.augmentations.
+00005780: 7472 616e 7366 6f72 6d73 2e4d 6f72 7068  transforms.Morph
+00005790: 6f6c 6f67 6963 616c 2920 2020 2020 2020  ological)       
+000057a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000057b0: 2020 2020 2020 2020 2020 2020 7c20 e29c              | ..
+000057c0: 9320 2020 2020 7c20 e29c 9320 2020 207c  .     | ...    |
+000057d0: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
+000057e0: 2020 2020 7c0a 7c20 5b4e 6f4f 705d 2868      |.| [NoOp](h
+000057f0: 7474 7073 3a2f 2f61 6c62 756d 656e 7461  ttps://albumenta
+00005800: 7469 6f6e 732e 6169 2f64 6f63 732f 6170  tions.ai/docs/ap
+00005810: 695f 7265 6665 7265 6e63 652f 636f 7265  i_reference/core
+00005820: 2f74 7261 6e73 666f 726d 735f 696e 7465  /transforms_inte
+00005830: 7266 6163 652f 2361 6c62 756d 656e 7461  rface/#albumenta
+00005840: 7469 6f6e 732e 636f 7265 2e74 7261 6e73  tions.core.trans
+00005850: 666f 726d 735f 696e 7465 7266 6163 652e  forms_interface.
+00005860: 4e6f 4f70 2920 2020 2020 2020 2020 2020  NoOp)           
+00005870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005890: 2020 2020 2020 2020 7c20 e29c 9320 2020          | ...   
+000058a0: 2020 7c20 e29c 9320 2020 207c 20e2 9c93    | ...    | ...
+000058b0: 2020 2020 2020 7c20 e29c 9320 2020 2020        | ...     
+000058c0: 2020 2020 7c0a 7c20 5b4f 7074 6963 616c      |.| [Optical
+000058d0: 4469 7374 6f72 7469 6f6e 5d28 6874 7470  Distortion](http
+000058e0: 733a 2f2f 616c 6275 6d65 6e74 6174 696f  s://albumentatio
+000058f0: 6e73 2e61 692f 646f 6373 2f61 7069 5f72  ns.ai/docs/api_r
+00005900: 6566 6572 656e 6365 2f61 7567 6d65 6e74  eference/augment
+00005910: 6174 696f 6e73 2f67 656f 6d65 7472 6963  ations/geometric
+00005920: 2f74 7261 6e73 666f 726d 732f 2361 6c62  /transforms/#alb
+00005930: 756d 656e 7461 7469 6f6e 732e 6175 676d  umentations.augm
+00005940: 656e 7461 7469 6f6e 732e 6765 6f6d 6574  entations.geomet
+00005950: 7269 632e 7472 616e 7366 6f72 6d73 2e4f  ric.transforms.O
+00005960: 7074 6963 616c 4469 7374 6f72 7469 6f6e  pticalDistortion
+00005970: 2920 2020 2020 2020 7c20 e29c 9320 2020  )       | ...   
+00005980: 2020 7c20 e29c 9320 2020 207c 20e2 9c93    | ...    | ...
+00005990: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
+000059a0: 2020 7c0a 7c20 5b50 6164 4966 4e65 6564    |.| [PadIfNeed
+000059b0: 6564 5d28 6874 7470 733a 2f2f 616c 6275  ed](https://albu
+000059c0: 6d65 6e74 6174 696f 6e73 2e61 692f 646f  mentations.ai/do
+000059d0: 6373 2f61 7069 5f72 6566 6572 656e 6365  cs/api_reference
+000059e0: 2f61 7567 6d65 6e74 6174 696f 6e73 2f67  /augmentations/g
+000059f0: 656f 6d65 7472 6963 2f74 7261 6e73 666f  eometric/transfo
+00005a00: 726d 732f 2361 6c62 756d 656e 7461 7469  rms/#albumentati
+00005a10: 6f6e 732e 6175 676d 656e 7461 7469 6f6e  ons.augmentation
+00005a20: 732e 6765 6f6d 6574 7269 632e 7472 616e  s.geometric.tran
+00005a30: 7366 6f72 6d73 2e50 6164 4966 4e65 6564  sforms.PadIfNeed
+00005a40: 6564 2920 2020 2020 2020 2020 2020 2020  ed)             
+00005a50: 2020 2020 2020 7c20 e29c 9320 2020 2020        | ...     
+00005a60: 7c20 e29c 9320 2020 207c 20e2 9c93 2020  | ...    | ...  
+00005a70: 2020 2020 7c20 e29c 9320 2020 2020 2020      | ...       
+00005a80: 2020 7c0a 7c20 5b50 6572 7370 6563 7469    |.| [Perspecti
+00005a90: 7665 5d28 6874 7470 733a 2f2f 616c 6275  ve](https://albu
+00005aa0: 6d65 6e74 6174 696f 6e73 2e61 692f 646f  mentations.ai/do
+00005ab0: 6373 2f61 7069 5f72 6566 6572 656e 6365  cs/api_reference
+00005ac0: 2f61 7567 6d65 6e74 6174 696f 6e73 2f67  /augmentations/g
+00005ad0: 656f 6d65 7472 6963 2f74 7261 6e73 666f  eometric/transfo
+00005ae0: 726d 732f 2361 6c62 756d 656e 7461 7469  rms/#albumentati
+00005af0: 6f6e 732e 6175 676d 656e 7461 7469 6f6e  ons.augmentation
+00005b00: 732e 6765 6f6d 6574 7269 632e 7472 616e  s.geometric.tran
+00005b10: 7366 6f72 6d73 2e50 6572 7370 6563 7469  sforms.Perspecti
+00005b20: 7665 2920 2020 2020 2020 2020 2020 2020  ve)             
+00005b30: 2020 2020 2020 7c20 e29c 9320 2020 2020        | ...     
+00005b40: 7c20 e29c 9320 2020 207c 20e2 9c93 2020  | ...    | ...  
+00005b50: 2020 2020 7c20 e29c 9320 2020 2020 2020      | ...       
+00005b60: 2020 7c0a 7c20 5b50 6965 6365 7769 7365    |.| [Piecewise
+00005b70: 4166 6669 6e65 5d28 6874 7470 733a 2f2f  Affine](https://
+00005b80: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
+00005b90: 692f 646f 6373 2f61 7069 5f72 6566 6572  i/docs/api_refer
+00005ba0: 656e 6365 2f61 7567 6d65 6e74 6174 696f  ence/augmentatio
+00005bb0: 6e73 2f67 656f 6d65 7472 6963 2f74 7261  ns/geometric/tra
+00005bc0: 6e73 666f 726d 732f 2361 6c62 756d 656e  nsforms/#albumen
+00005bd0: 7461 7469 6f6e 732e 6175 676d 656e 7461  tations.augmenta
+00005be0: 7469 6f6e 732e 6765 6f6d 6574 7269 632e  tions.geometric.
+00005bf0: 7472 616e 7366 6f72 6d73 2e50 6965 6365  transforms.Piece
+00005c00: 7769 7365 4166 6669 6e65 2920 2020 2020  wiseAffine)     
+00005c10: 2020 2020 2020 7c20 e29c 9320 2020 2020        | ...     
+00005c20: 7c20 e29c 9320 2020 207c 20e2 9c93 2020  | ...    | ...  
+00005c30: 2020 2020 7c20 e29c 9320 2020 2020 2020      | ...       
+00005c40: 2020 7c0a 7c20 5b50 6978 656c 4472 6f70    |.| [PixelDrop
+00005c50: 6f75 745d 2868 7474 7073 3a2f 2f61 6c62  out](https://alb
+00005c60: 756d 656e 7461 7469 6f6e 732e 6169 2f64  umentations.ai/d
+00005c70: 6f63 732f 6170 695f 7265 6665 7265 6e63  ocs/api_referenc
+00005c80: 652f 6175 676d 656e 7461 7469 6f6e 732f  e/augmentations/
+00005c90: 7472 616e 7366 6f72 6d73 2f23 616c 6275  transforms/#albu
+00005ca0: 6d65 6e74 6174 696f 6e73 2e61 7567 6d65  mentations.augme
+00005cb0: 6e74 6174 696f 6e73 2e74 7261 6e73 666f  ntations.transfo
+00005cc0: 726d 732e 5069 7865 6c44 726f 706f 7574  rms.PixelDropout
+00005cd0: 2920 2020 2020 2020 2020 2020 2020 2020  )               
+00005ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005cf0: 2020 2020 2020 7c20 e29c 9320 2020 2020        | ...     
+00005d00: 7c20 e29c 9320 2020 207c 2020 2020 2020  | ...    |      
+00005d10: 2020 7c20 2020 2020 2020 2020 2020 7c0a    |           |.
+00005d20: 7c20 5b52 616e 646f 6d43 726f 705d 2868  | [RandomCrop](h
+00005d30: 7474 7073 3a2f 2f61 6c62 756d 656e 7461  ttps://albumenta
+00005d40: 7469 6f6e 732e 6169 2f64 6f63 732f 6170  tions.ai/docs/ap
+00005d50: 695f 7265 6665 7265 6e63 652f 6175 676d  i_reference/augm
+00005d60: 656e 7461 7469 6f6e 732f 6372 6f70 732f  entations/crops/
+00005d70: 7472 616e 7366 6f72 6d73 2f23 616c 6275  transforms/#albu
+00005d80: 6d65 6e74 6174 696f 6e73 2e61 7567 6d65  mentations.augme
+00005d90: 6e74 6174 696f 6e73 2e63 726f 7073 2e74  ntations.crops.t
+00005da0: 7261 6e73 666f 726d 732e 5261 6e64 6f6d  ransforms.Random
+00005db0: 4372 6f70 2920 2020 2020 2020 2020 2020  Crop)           
+00005dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005dd0: 2020 7c20 e29c 9320 2020 2020 7c20 e29c    | ...     | ..
+00005de0: 9320 2020 207c 20e2 9c93 2020 2020 2020  .    | ...      
+00005df0: 7c20 e29c 9320 2020 2020 2020 2020 7c0a  | ...         |.
+00005e00: 7c20 5b52 616e 646f 6d43 726f 7046 726f  | [RandomCropFro
+00005e10: 6d42 6f72 6465 7273 5d28 6874 7470 733a  mBorders](https:
+00005e20: 2f2f 616c 6275 6d65 6e74 6174 696f 6e73  //albumentations
+00005e30: 2e61 692f 646f 6373 2f61 7069 5f72 6566  .ai/docs/api_ref
+00005e40: 6572 656e 6365 2f61 7567 6d65 6e74 6174  erence/augmentat
+00005e50: 696f 6e73 2f63 726f 7073 2f74 7261 6e73  ions/crops/trans
+00005e60: 666f 726d 732f 2361 6c62 756d 656e 7461  forms/#albumenta
+00005e70: 7469 6f6e 732e 6175 676d 656e 7461 7469  tions.augmentati
+00005e80: 6f6e 732e 6372 6f70 732e 7472 616e 7366  ons.crops.transf
+00005e90: 6f72 6d73 2e52 616e 646f 6d43 726f 7046  orms.RandomCropF
+00005ea0: 726f 6d42 6f72 6465 7273 2920 2020 2020  romBorders)     
+00005eb0: 2020 7c20 e29c 9320 2020 2020 7c20 e29c    | ...     | ..
+00005ec0: 9320 2020 207c 20e2 9c93 2020 2020 2020  .    | ...      
+00005ed0: 7c20 e29c 9320 2020 2020 2020 2020 7c0a  | ...         |.
+00005ee0: 7c20 5b52 616e 646f 6d47 7269 6453 6875  | [RandomGridShu
+00005ef0: 6666 6c65 5d28 6874 7470 733a 2f2f 616c  ffle](https://al
+00005f00: 6275 6d65 6e74 6174 696f 6e73 2e61 692f  bumentations.ai/
+00005f10: 646f 6373 2f61 7069 5f72 6566 6572 656e  docs/api_referen
+00005f20: 6365 2f61 7567 6d65 6e74 6174 696f 6e73  ce/augmentations
+00005f30: 2f74 7261 6e73 666f 726d 732f 2361 6c62  /transforms/#alb
+00005f40: 756d 656e 7461 7469 6f6e 732e 6175 676d  umentations.augm
+00005f50: 656e 7461 7469 6f6e 732e 7472 616e 7366  entations.transf
+00005f60: 6f72 6d73 2e52 616e 646f 6d47 7269 6453  orms.RandomGridS
+00005f70: 6875 6666 6c65 2920 2020 2020 2020 2020  huffle)         
+00005f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f90: 2020 7c20 e29c 9320 2020 2020 7c20 e29c    | ...     | ..
+00005fa0: 9320 2020 207c 2020 2020 2020 2020 7c20  .    |        | 
+00005fb0: e29c 9320 2020 2020 2020 2020 7c0a 7c20  ...         |.| 
+00005fc0: 5b52 616e 646f 6d52 6573 697a 6564 4372  [RandomResizedCr
+00005fd0: 6f70 5d28 6874 7470 733a 2f2f 616c 6275  op](https://albu
+00005fe0: 6d65 6e74 6174 696f 6e73 2e61 692f 646f  mentations.ai/do
+00005ff0: 6373 2f61 7069 5f72 6566 6572 656e 6365  cs/api_reference
+00006000: 2f61 7567 6d65 6e74 6174 696f 6e73 2f63  /augmentations/c
+00006010: 726f 7073 2f74 7261 6e73 666f 726d 732f  rops/transforms/
+00006020: 2361 6c62 756d 656e 7461 7469 6f6e 732e  #albumentations.
+00006030: 6175 676d 656e 7461 7469 6f6e 732e 6372  augmentations.cr
+00006040: 6f70 732e 7472 616e 7366 6f72 6d73 2e52  ops.transforms.R
+00006050: 616e 646f 6d52 6573 697a 6564 4372 6f70  andomResizedCrop
+00006060: 2920 2020 2020 2020 2020 2020 2020 2020  )               
+00006070: 7c20 e29c 9320 2020 2020 7c20 e29c 9320  | ...     | ... 
+00006080: 2020 207c 20e2 9c93 2020 2020 2020 7c20     | ...      | 
+00006090: e29c 9320 2020 2020 2020 2020 7c0a 7c20  ...         |.| 
+000060a0: 5b52 616e 646f 6d52 6f74 6174 6539 305d  [RandomRotate90]
+000060b0: 2868 7474 7073 3a2f 2f61 6c62 756d 656e  (https://albumen
+000060c0: 7461 7469 6f6e 732e 6169 2f64 6f63 732f  tations.ai/docs/
+000060d0: 6170 695f 7265 6665 7265 6e63 652f 6175  api_reference/au
+000060e0: 676d 656e 7461 7469 6f6e 732f 6765 6f6d  gmentations/geom
+000060f0: 6574 7269 632f 726f 7461 7465 2f23 616c  etric/rotate/#al
+00006100: 6275 6d65 6e74 6174 696f 6e73 2e61 7567  bumentations.aug
+00006110: 6d65 6e74 6174 696f 6e73 2e67 656f 6d65  mentations.geome
+00006120: 7472 6963 2e72 6f74 6174 652e 5261 6e64  tric.rotate.Rand
+00006130: 6f6d 526f 7461 7465 3930 2920 2020 2020  omRotate90)     
+00006140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006150: 7c20 e29c 9320 2020 2020 7c20 e29c 9320  | ...     | ... 
+00006160: 2020 207c 20e2 9c93 2020 2020 2020 7c20     | ...      | 
+00006170: e29c 9320 2020 2020 2020 2020 7c0a 7c20  ...         |.| 
+00006180: 5b52 616e 646f 6d53 6361 6c65 5d28 6874  [RandomScale](ht
+00006190: 7470 733a 2f2f 616c 6275 6d65 6e74 6174  tps://albumentat
+000061a0: 696f 6e73 2e61 692f 646f 6373 2f61 7069  ions.ai/docs/api
+000061b0: 5f72 6566 6572 656e 6365 2f61 7567 6d65  _reference/augme
+000061c0: 6e74 6174 696f 6e73 2f67 656f 6d65 7472  ntations/geometr
+000061d0: 6963 2f72 6573 697a 652f 2361 6c62 756d  ic/resize/#album
+000061e0: 656e 7461 7469 6f6e 732e 6175 676d 656e  entations.augmen
+000061f0: 7461 7469 6f6e 732e 6765 6f6d 6574 7269  tations.geometri
+00006200: 632e 7265 7369 7a65 2e52 616e 646f 6d53  c.resize.RandomS
+00006210: 6361 6c65 2920 2020 2020 2020 2020 2020  cale)           
+00006220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006230: 7c20 e29c 9320 2020 2020 7c20 e29c 9320  | ...     | ... 
+00006240: 2020 207c 20e2 9c93 2020 2020 2020 7c20     | ...      | 
+00006250: e29c 9320 2020 2020 2020 2020 7c0a 7c20  ...         |.| 
+00006260: 5b52 616e 646f 6d53 697a 6564 4242 6f78  [RandomSizedBBox
+00006270: 5361 6665 4372 6f70 5d28 6874 7470 733a  SafeCrop](https:
+00006280: 2f2f 616c 6275 6d65 6e74 6174 696f 6e73  //albumentations
+00006290: 2e61 692f 646f 6373 2f61 7069 5f72 6566  .ai/docs/api_ref
+000062a0: 6572 656e 6365 2f61 7567 6d65 6e74 6174  erence/augmentat
+000062b0: 696f 6e73 2f63 726f 7073 2f74 7261 6e73  ions/crops/trans
+000062c0: 666f 726d 732f 2361 6c62 756d 656e 7461  forms/#albumenta
+000062d0: 7469 6f6e 732e 6175 676d 656e 7461 7469  tions.augmentati
+000062e0: 6f6e 732e 6372 6f70 732e 7472 616e 7366  ons.crops.transf
+000062f0: 6f72 6d73 2e52 616e 646f 6d53 697a 6564  orms.RandomSized
+00006300: 4242 6f78 5361 6665 4372 6f70 2920 2020  BBoxSafeCrop)   
+00006310: 7c20 e29c 9320 2020 2020 7c20 e29c 9320  | ...     | ... 
+00006320: 2020 207c 20e2 9c93 2020 2020 2020 7c20     | ...      | 
+00006330: 2020 2020 2020 2020 2020 7c0a 7c20 5b52            |.| [R
+00006340: 616e 646f 6d53 697a 6564 4372 6f70 5d28  andomSizedCrop](
+00006350: 6874 7470 733a 2f2f 616c 6275 6d65 6e74  https://albument
+00006360: 6174 696f 6e73 2e61 692f 646f 6373 2f61  ations.ai/docs/a
+00006370: 7069 5f72 6566 6572 656e 6365 2f61 7567  pi_reference/aug
+00006380: 6d65 6e74 6174 696f 6e73 2f63 726f 7073  mentations/crops
+00006390: 2f74 7261 6e73 666f 726d 732f 2361 6c62  /transforms/#alb
+000063a0: 756d 656e 7461 7469 6f6e 732e 6175 676d  umentations.augm
+000063b0: 656e 7461 7469 6f6e 732e 6372 6f70 732e  entations.crops.
+000063c0: 7472 616e 7366 6f72 6d73 2e52 616e 646f  transforms.Rando
+000063d0: 6d53 697a 6564 4372 6f70 2920 2020 2020  mSizedCrop)     
+000063e0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+000063f0: e29c 9320 2020 2020 7c20 e29c 9320 2020  ...     | ...   
+00006400: 207c 20e2 9c93 2020 2020 2020 7c20 e29c   | ...      | ..
+00006410: 9320 2020 2020 2020 2020 7c0a 7c20 5b52  .         |.| [R
+00006420: 6573 697a 655d 2868 7474 7073 3a2f 2f61  esize](https://a
+00006430: 6c62 756d 656e 7461 7469 6f6e 732e 6169  lbumentations.ai
+00006440: 2f64 6f63 732f 6170 695f 7265 6665 7265  /docs/api_refere
+00006450: 6e63 652f 6175 676d 656e 7461 7469 6f6e  nce/augmentation
+00006460: 732f 6765 6f6d 6574 7269 632f 7265 7369  s/geometric/resi
+00006470: 7a65 2f23 616c 6275 6d65 6e74 6174 696f  ze/#albumentatio
+00006480: 6e73 2e61 7567 6d65 6e74 6174 696f 6e73  ns.augmentations
+00006490: 2e67 656f 6d65 7472 6963 2e72 6573 697a  .geometric.resiz
+000064a0: 652e 5265 7369 7a65 2920 2020 2020 2020  e.Resize)       
+000064b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000064c0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+000064d0: e29c 9320 2020 2020 7c20 e29c 9320 2020  ...     | ...   
+000064e0: 207c 20e2 9c93 2020 2020 2020 7c20 e29c   | ...      | ..
+000064f0: 9320 2020 2020 2020 2020 7c0a 7c20 5b52  .         |.| [R
+00006500: 6f74 6174 655d 2868 7474 7073 3a2f 2f61  otate](https://a
+00006510: 6c62 756d 656e 7461 7469 6f6e 732e 6169  lbumentations.ai
+00006520: 2f64 6f63 732f 6170 695f 7265 6665 7265  /docs/api_refere
+00006530: 6e63 652f 6175 676d 656e 7461 7469 6f6e  nce/augmentation
+00006540: 732f 6765 6f6d 6574 7269 632f 726f 7461  s/geometric/rota
+00006550: 7465 2f23 616c 6275 6d65 6e74 6174 696f  te/#albumentatio
+00006560: 6e73 2e61 7567 6d65 6e74 6174 696f 6e73  ns.augmentations
+00006570: 2e67 656f 6d65 7472 6963 2e72 6f74 6174  .geometric.rotat
+00006580: 652e 526f 7461 7465 2920 2020 2020 2020  e.Rotate)       
+00006590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000065a0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+000065b0: e29c 9320 2020 2020 7c20 e29c 9320 2020  ...     | ...   
+000065c0: 207c 20e2 9c93 2020 2020 2020 7c20 e29c   | ...      | ..
+000065d0: 9320 2020 2020 2020 2020 7c0a 7c20 5b53  .         |.| [S
+000065e0: 6166 6552 6f74 6174 655d 2868 7474 7073  afeRotate](https
+000065f0: 3a2f 2f61 6c62 756d 656e 7461 7469 6f6e  ://albumentation
+00006600: 732e 6169 2f64 6f63 732f 6170 695f 7265  s.ai/docs/api_re
+00006610: 6665 7265 6e63 652f 6175 676d 656e 7461  ference/augmenta
+00006620: 7469 6f6e 732f 6765 6f6d 6574 7269 632f  tions/geometric/
+00006630: 726f 7461 7465 2f23 616c 6275 6d65 6e74  rotate/#albument
+00006640: 6174 696f 6e73 2e61 7567 6d65 6e74 6174  ations.augmentat
+00006650: 696f 6e73 2e67 656f 6d65 7472 6963 2e72  ions.geometric.r
+00006660: 6f74 6174 652e 5361 6665 526f 7461 7465  otate.SafeRotate
+00006670: 2920 2020 2020 2020 2020 2020 2020 2020  )               
+00006680: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+00006690: e29c 9320 2020 2020 7c20 e29c 9320 2020  ...     | ...   
+000066a0: 207c 20e2 9c93 2020 2020 2020 7c20 e29c   | ...      | ..
+000066b0: 9320 2020 2020 2020 2020 7c0a 7c20 5b53  .         |.| [S
+000066c0: 6869 6674 5363 616c 6552 6f74 6174 655d  hiftScaleRotate]
+000066d0: 2868 7474 7073 3a2f 2f61 6c62 756d 656e  (https://albumen
+000066e0: 7461 7469 6f6e 732e 6169 2f64 6f63 732f  tations.ai/docs/
+000066f0: 6170 695f 7265 6665 7265 6e63 652f 6175  api_reference/au
+00006700: 676d 656e 7461 7469 6f6e 732f 6765 6f6d  gmentations/geom
+00006710: 6574 7269 632f 7472 616e 7366 6f72 6d73  etric/transforms
+00006720: 2f23 616c 6275 6d65 6e74 6174 696f 6e73  /#albumentations
+00006730: 2e61 7567 6d65 6e74 6174 696f 6e73 2e67  .augmentations.g
+00006740: 656f 6d65 7472 6963 2e74 7261 6e73 666f  eometric.transfo
+00006750: 726d 732e 5368 6966 7453 6361 6c65 526f  rms.ShiftScaleRo
+00006760: 7461 7465 2920 2020 2020 2020 2020 7c20  tate)         | 
+00006770: e29c 9320 2020 2020 7c20 e29c 9320 2020  ...     | ...   
+00006780: 207c 20e2 9c93 2020 2020 2020 7c20 e29c   | ...      | ..
+00006790: 9320 2020 2020 2020 2020 7c0a 7c20 5b53  .         |.| [S
+000067a0: 6d61 6c6c 6573 744d 6178 5369 7a65 5d28  mallestMaxSize](
+000067b0: 6874 7470 733a 2f2f 616c 6275 6d65 6e74  https://albument
+000067c0: 6174 696f 6e73 2e61 692f 646f 6373 2f61  ations.ai/docs/a
+000067d0: 7069 5f72 6566 6572 656e 6365 2f61 7567  pi_reference/aug
+000067e0: 6d65 6e74 6174 696f 6e73 2f67 656f 6d65  mentations/geome
+000067f0: 7472 6963 2f72 6573 697a 652f 2361 6c62  tric/resize/#alb
+00006800: 756d 656e 7461 7469 6f6e 732e 6175 676d  umentations.augm
+00006810: 656e 7461 7469 6f6e 732e 6765 6f6d 6574  entations.geomet
+00006820: 7269 632e 7265 7369 7a65 2e53 6d61 6c6c  ric.resize.Small
+00006830: 6573 744d 6178 5369 7a65 2920 2020 2020  estMaxSize)     
+00006840: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+00006850: e29c 9320 2020 2020 7c20 e29c 9320 2020  ...     | ...   
+00006860: 207c 20e2 9c93 2020 2020 2020 7c20 e29c   | ...      | ..
+00006870: 9320 2020 2020 2020 2020 7c0a 7c20 5b54  .         |.| [T
+00006880: 7261 6e73 706f 7365 5d28 6874 7470 733a  ranspose](https:
+00006890: 2f2f 616c 6275 6d65 6e74 6174 696f 6e73  //albumentations
+000068a0: 2e61 692f 646f 6373 2f61 7069 5f72 6566  .ai/docs/api_ref
+000068b0: 6572 656e 6365 2f61 7567 6d65 6e74 6174  erence/augmentat
+000068c0: 696f 6e73 2f67 656f 6d65 7472 6963 2f74  ions/geometric/t
+000068d0: 7261 6e73 666f 726d 732f 2361 6c62 756d  ransforms/#album
+000068e0: 656e 7461 7469 6f6e 732e 6175 676d 656e  entations.augmen
+000068f0: 7461 7469 6f6e 732e 6765 6f6d 6574 7269  tations.geometri
+00006900: 632e 7472 616e 7366 6f72 6d73 2e54 7261  c.transforms.Tra
+00006910: 6e73 706f 7365 2920 2020 2020 2020 2020  nspose)         
+00006920: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+00006930: e29c 9320 2020 2020 7c20 e29c 9320 2020  ...     | ...   
+00006940: 207c 20e2 9c93 2020 2020 2020 7c20 e29c   | ...      | ..
+00006950: 9320 2020 2020 2020 2020 7c0a 7c20 5b56  .         |.| [V
+00006960: 6572 7469 6361 6c46 6c69 705d 2868 7474  erticalFlip](htt
+00006970: 7073 3a2f 2f61 6c62 756d 656e 7461 7469  ps://albumentati
+00006980: 6f6e 732e 6169 2f64 6f63 732f 6170 695f  ons.ai/docs/api_
+00006990: 7265 6665 7265 6e63 652f 6175 676d 656e  reference/augmen
+000069a0: 7461 7469 6f6e 732f 6765 6f6d 6574 7269  tations/geometri
+000069b0: 632f 7472 616e 7366 6f72 6d73 2f23 616c  c/transforms/#al
+000069c0: 6275 6d65 6e74 6174 696f 6e73 2e61 7567  bumentations.aug
+000069d0: 6d65 6e74 6174 696f 6e73 2e67 656f 6d65  mentations.geome
+000069e0: 7472 6963 2e74 7261 6e73 666f 726d 732e  tric.transforms.
+000069f0: 5665 7274 6963 616c 466c 6970 2920 2020  VerticalFlip)   
+00006a00: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+00006a10: e29c 9320 2020 2020 7c20 e29c 9320 2020  ...     | ...   
+00006a20: 207c 20e2 9c93 2020 2020 2020 7c20 e29c   | ...      | ..
+00006a30: 9320 2020 2020 2020 2020 7c0a 7c20 5b58  .         |.| [X
+00006a40: 594d 6173 6b69 6e67 5d28 6874 7470 733a  YMasking](https:
+00006a50: 2f2f 616c 6275 6d65 6e74 6174 696f 6e73  //albumentations
+00006a60: 2e61 692f 646f 6373 2f61 7069 5f72 6566  .ai/docs/api_ref
+00006a70: 6572 656e 6365 2f61 7567 6d65 6e74 6174  erence/augmentat
+00006a80: 696f 6e73 2f64 726f 706f 7574 2f78 795f  ions/dropout/xy_
+00006a90: 6d61 736b 696e 672f 2361 6c62 756d 656e  masking/#albumen
+00006aa0: 7461 7469 6f6e 732e 6175 676d 656e 7461  tations.augmenta
+00006ab0: 7469 6f6e 732e 6472 6f70 6f75 742e 7879  tions.dropout.xy
+00006ac0: 5f6d 6173 6b69 6e67 2e58 594d 6173 6b69  _masking.XYMaski
+00006ad0: 6e67 2920 2020 2020 2020 2020 2020 2020  ng)             
+00006ae0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+00006af0: e29c 9320 2020 2020 7c20 e29c 9320 2020  ...     | ...   
+00006b00: 207c 2020 2020 2020 2020 7c20 e29c 9320   |        | ... 
+00006b10: 2020 2020 2020 2020 7c0a 0a23 2323 204d          |..### M
+00006b20: 6978 696e 672d 6c65 7665 6c20 7472 616e  ixing-level tran
+00006b30: 7366 6f72 6d73 0a0a 5472 616e 7366 6f72  sforms..Transfor
+00006b40: 6d73 2074 6861 7420 6d69 7820 7365 7665  ms that mix seve
+00006b50: 7261 6c20 696d 6167 6573 2069 6e74 6f20  ral images into 
+00006b60: 6f6e 650a 0a7c 2054 7261 6e73 666f 726d  one..| Transform
+00006b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006bf0: 2020 207c 2049 6d61 6765 207c 204d 6173     | Image | Mas
+00006c00: 6b20 7c20 4242 6f78 6573 207c 204b 6579  k | BBoxes | Key
+00006c10: 706f 696e 7473 207c 2047 6c6f 6261 6c20  points | Global 
+00006c20: 4c61 6265 6c20 7c0a 7c20 2d2d 2d2d 2d2d  Label |.| ------
+00006c30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006c40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006c50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006c60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006c70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006c80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006c90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006ca0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006cb0: 2d2d 2d2d 2d20 7c20 3a2d 2d2d 3a20 7c20  ----- | :---: | 
+00006cc0: 3a2d 2d3a 207c 203a 2d2d 2d2d 3a20 7c20  :--: | :----: | 
+00006cd0: 3a2d 2d2d 2d2d 2d2d 3a20 7c20 3a2d 2d2d  :-------: | :---
+00006ce0: 2d2d 2d2d 2d2d 2d3a 207c 0a7c 205b 4d69  -------: |.| [Mi
+00006cf0: 7855 705d 2868 7474 7073 3a2f 2f61 6c62  xUp](https://alb
+00006d00: 756d 656e 7461 7469 6f6e 732e 6169 2f64  umentations.ai/d
+00006d10: 6f63 732f 6170 695f 7265 6665 7265 6e63  ocs/api_referenc
+00006d20: 652f 6175 676d 656e 7461 7469 6f6e 732f  e/augmentations/
+00006d30: 6d69 7869 6e67 2f74 7261 6e73 666f 726d  mixing/transform
+00006d40: 732f 2361 6c62 756d 656e 7461 7469 6f6e  s/#albumentation
+00006d50: 732e 6175 676d 656e 7461 7469 6f6e 732e  s.augmentations.
+00006d60: 6d69 7869 6e67 2e74 7261 6e73 666f 726d  mixing.transform
+00006d70: 732e 4d69 7855 7029 207c 20e2 9c93 2020  s.MixUp) | ...  
+00006d80: 2020 207c 20e2 9c93 2020 2020 7c20 2020     | ...    |   
+00006d90: 2020 2020 207c 2020 2020 2020 2020 2020       |          
+00006da0: 207c 20e2 9c93 2020 2020 2020 2020 2020   | ...          
+00006db0: 2020 7c0a 0a23 2320 4120 6665 7720 6d6f    |..## A few mo
+00006dc0: 7265 2065 7861 6d70 6c65 7320 6f66 202a  re examples of *
+00006dd0: 2a61 7567 6d65 6e74 6174 696f 6e73 2a2a  *augmentations**
+00006de0: 0a0a 2323 2320 5365 6d61 6e74 6963 2073  ..### Semantic s
+00006df0: 6567 6d65 6e74 6174 696f 6e20 6f6e 2074  egmentation on t
+00006e00: 6865 2049 6e72 6961 2064 6174 6173 6574  he Inria dataset
+00006e10: 0a0a 215b 696e 7269 615d 2868 7474 7073  ..![inria](https
+00006e20: 3a2f 2f68 6162 7261 7374 6f72 6167 652e  ://habrastorage.
+00006e30: 6f72 672f 7765 6274 2f73 752f 7761 2f6e  org/webt/su/wa/n
+00006e40: 702f 7375 7761 6e70 656f 3677 7737 7770  p/suwanpeo6ww7wp
+00006e50: 7774 6f62 7472 7a64 5f63 6732 302e 6a70  wtobtrzd_cg20.jp
+00006e60: 6567 290a 0a23 2323 204d 6564 6963 616c  eg)..### Medical
+00006e70: 2069 6d61 6769 6e67 0a0a 215b 6d65 6469   imaging..![medi
+00006e80: 6361 6c5d 2868 7474 7073 3a2f 2f68 6162  cal](https://hab
+00006e90: 7261 7374 6f72 6167 652e 6f72 672f 7765  rastorage.org/we
+00006ea0: 6274 2f31 692f 6669 2f77 7a2f 3169 6669  bt/1i/fi/wz/1ifi
+00006eb0: 777a 7930 6c78 6574 6334 6e77 6a76 7373  wzy0lxetc4nwjvss
+00006ec0: 2d37 316e 6b77 302e 6a70 6567 290a 0a23  -71nkw0.jpeg)..#
+00006ed0: 2323 204f 626a 6563 7420 6465 7465 6374  ## Object detect
+00006ee0: 696f 6e20 616e 6420 7365 6d61 6e74 6963  ion and semantic
+00006ef0: 2073 6567 6d65 6e74 6174 696f 6e20 6f6e   segmentation on
+00006f00: 2074 6865 204d 6170 696c 6c61 7279 2056   the Mapillary V
+00006f10: 6973 7461 7320 6461 7461 7365 740a 0a21  istas dataset..!
+00006f20: 5b76 6973 7461 735d 2868 7474 7073 3a2f  [vistas](https:/
+00006f30: 2f68 6162 7261 7374 6f72 6167 652e 6f72  /habrastorage.or
+00006f40: 672f 7765 6274 2f72 7a2f 2d68 2f33 6a2f  g/webt/rz/-h/3j/
+00006f50: 727a 2d68 336a 616c 6278 6963 386f 5f66  rz-h3jalbxic8o_f
+00006f60: 6875 6378 7973 7473 3474 632e 6a70 6567  hucxysts4tc.jpeg
+00006f70: 290a 0a23 2323 204b 6579 706f 696e 7473  )..### Keypoints
+00006f80: 2061 7567 6d65 6e74 6174 696f 6e0a 0a3c   augmentation..<
+00006f90: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00006fa0: 2f68 6162 7261 7374 6f72 6167 652e 6f72  /habrastorage.or
+00006fb0: 672f 7765 6274 2f65 2d2f 366b 2f7a 2d2f  g/webt/e-/6k/z-/
+00006fc0: 652d 366b 7a2d 6675 6770 3268 6561 6b33  e-6kz-fugp2heak3
+00006fd0: 6a7a 6e73 3362 632d 7238 6f2e 6a70 6567  jzns3bc-r8o.jpeg
+00006fe0: 2220 7769 6474 683d 3130 3025 3e0a 0a23  " width=100%>..#
+00006ff0: 2320 4265 6e63 686d 6172 6b69 6e67 2072  # Benchmarking r
+00007000: 6573 756c 7473 0a0a 546f 2072 756e 2074  esults..To run t
+00007010: 6865 2062 656e 6368 6d61 726b 2079 6f75  he benchmark you
+00007020: 7273 656c 662c 2066 6f6c 6c6f 7720 7468  rself, follow th
+00007030: 6520 696e 7374 7275 6374 696f 6e73 2069  e instructions i
+00007040: 6e20 5b62 656e 6368 6d61 726b 2f52 4541  n [benchmark/REA
+00007050: 444d 452e 6d64 5d28 6874 7470 733a 2f2f  DME.md](https://
+00007060: 6769 7468 7562 2e63 6f6d 2f61 6c62 756d  github.com/album
+00007070: 656e 7461 7469 6f6e 732d 7465 616d 2f61  entations-team/a
+00007080: 6c62 756d 656e 7461 7469 6f6e 732f 626c  lbumentations/bl
+00007090: 6f62 2f6d 6173 7465 722f 6265 6e63 686d  ob/master/benchm
+000070a0: 6172 6b2f 5245 4144 4d45 2e6d 6429 0a0a  ark/README.md)..
+000070b0: 5265 7375 6c74 7320 666f 7220 7275 6e6e  Results for runn
+000070c0: 696e 6720 7468 6520 6265 6e63 686d 6172  ing the benchmar
+000070d0: 6b20 6f6e 2074 6865 2066 6972 7374 2032  k on the first 2
+000070e0: 3030 3020 696d 6167 6573 2066 726f 6d20  000 images from 
+000070f0: 7468 6520 496d 6167 654e 6574 2076 616c  the ImageNet val
+00007100: 6964 6174 696f 6e20 7365 7420 7573 696e  idation set usin
+00007110: 6720 616e 2041 4d44 2052 797a 656e 2054  g an AMD Ryzen T
+00007120: 6872 6561 6472 6970 7065 7220 3339 3730  hreadripper 3970
+00007130: 5820 4350 552e 0a54 6865 2074 6162 6c65  X CPU..The table
+00007140: 2073 686f 7773 2068 6f77 206d 616e 7920   shows how many 
+00007150: 696d 6167 6573 2070 6572 2073 6563 6f6e  images per secon
+00007160: 6420 6361 6e20 6265 2070 726f 6365 7373  d can be process
+00007170: 6564 206f 6e20 6120 7369 6e67 6c65 2063  ed on a single c
+00007180: 6f72 653b 2068 6967 6865 7220 6973 2062  ore; higher is b
+00007190: 6574 7465 722e 0a0a 7c20 4c69 6272 6172  etter...| Librar
+000071a0: 7920 7c20 5665 7273 696f 6e20 7c0a 7c2d  y | Version |.|-
+000071b0: 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d  --------|-------
+000071c0: 2d2d 7c0a 7c20 5079 7468 6f6e 207c 2033  --|.| Python | 3
+000071d0: 2e31 302e 3133 2028 6d61 696e 2c20 5365  .10.13 (main, Se
+000071e0: 7020 3131 2032 3032 332c 2031 333a 3434  p 11 2023, 13:44
+000071f0: 3a33 3529 205b 4743 4320 3131 2e32 2e30  :35) [GCC 11.2.0
+00007200: 5d20 7c0a 7c20 616c 6275 6d65 6e74 6174  ] |.| albumentat
+00007210: 696f 6e73 207c 2031 2e34 2e31 207c 0a7c  ions | 1.4.1 |.|
+00007220: 2069 6d67 6175 6720 7c20 302e 342e 3020   imgaug | 0.4.0 
+00007230: 7c0a 7c20 746f 7263 6876 6973 696f 6e20  |.| torchvision 
+00007240: 7c20 302e 3137 2e31 2b72 6f63 6d35 2e37  | 0.17.1+rocm5.7
+00007250: 207c 0a7c 206e 756d 7079 207c 2031 2e32   |.| numpy | 1.2
+00007260: 362e 3420 7c0a 7c20 6f70 656e 6376 2d70  6.4 |.| opencv-p
+00007270: 7974 686f 6e2d 6865 6164 6c65 7373 207c  ython-headless |
+00007280: 2034 2e39 2e30 2e38 3020 7c0a 7c20 7363   4.9.0.80 |.| sc
+00007290: 696b 6974 2d69 6d61 6765 207c 2030 2e32  ikit-image | 0.2
+000072a0: 322e 3020 7c0a 7c20 7363 6970 7920 7c20  2.0 |.| scipy | 
+000072b0: 312e 3132 2e30 207c 0a7c 2070 696c 6c6f  1.12.0 |.| pillo
+000072c0: 7720 7c20 3130 2e32 2e30 207c 0a7c 206b  w | 10.2.0 |.| k
+000072d0: 6f72 6e69 6120 7c20 302e 372e 3220 7c0a  ornia | 0.7.2 |.
+000072e0: 7c20 6175 676c 7920 7c20 312e 302e 3020  | augly | 1.0.0 
+000072f0: 7c0a 0a7c 2020 2020 2020 2020 2020 2020  |..|            
+00007300: 2020 2020 207c 616c 6275 6d65 6e74 6174       |albumentat
+00007310: 696f 6e73 3c62 723e 3c73 6d61 6c6c 3e31  ions<br><small>1
+00007320: 2e34 2e30 3c2f 736d 616c 6c3e 7c74 6f72  .4.0</small>|tor
+00007330: 6368 7669 7369 6f6e 3c62 723e 3c73 6d61  chvision<br><sma
+00007340: 6c6c 3e30 2e31 372e 312b 726f 636d 352e  ll>0.17.1+rocm5.
+00007350: 373c 2f73 6d61 6c6c 3e7c 6b6f 726e 6961  7</small>|kornia
+00007360: 3c62 723e 3c73 6d61 6c6c 3e30 2e37 2e32  <br><small>0.7.2
+00007370: 3c2f 736d 616c 6c3e 7c61 7567 6c79 3c62  </small>|augly<b
+00007380: 723e 3c73 6d61 6c6c 3e31 2e30 2e30 3c2f  r><small>1.0.0</
+00007390: 736d 616c 6c3e 7c69 6d67 6175 673c 6272  small>|imgaug<br
+000073a0: 3e3c 736d 616c 6c3e 302e 342e 303c 2f73  ><small>0.4.0</s
+000073b0: 6d61 6c6c 3e7c 0a7c 2d2d 2d2d 2d2d 2d2d  mall>|.|--------
+000073c0: 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d  ---------|------
+000073d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000073e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000073f0: 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |---------------
+00007400: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007410: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d  -------------|--
+00007420: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007430: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d  ------------|---
+00007440: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007450: 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d  ----------|-----
+00007460: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007470: 2d2d 2d2d 2d2d 2d2d 2d7c 0a7c 486f 7269  ---------|.|Hori
+00007480: 7a6f 6e74 616c 466c 6970 2020 207c 2a2a  zontalFlip   |**
+00007490: 3938 3433 20c2 b120 3231 3335 2a2a 2020  9843 .. 2135**  
+000074a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000074b0: 2020 2020 207c 3234 3336 20c2 b120 3239       |2436 .. 29
+000074c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000074d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000074e0: 2020 207c 3130 3134 20c2 b120 3320 2020     |1014 .. 3   
+000074f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007500: 2020 207c 3336 3633 20c2 b120 3138 2020     |3663 .. 18  
+00007510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007520: 2020 7c34 3838 3420 c2b1 2035 3120 2020    |4884 .. 51   
+00007530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007540: 2020 7c0a 7c56 6572 7469 6361 6c46 6c69    |.|VerticalFli
+00007550: 7020 2020 2020 7c2a 2a39 3839 3820 c2b1  p     |**9898 ..
+00007560: 2031 382a 2a20 2020 2020 2020 2020 2020   18**           
+00007570: 2020 2020 2020 2020 2020 2020 2020 7c32                |2
+00007580: 3537 3020 c2b1 2033 3720 2020 2020 2020  570 .. 37       
+00007590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000075a0: 2020 2020 2020 2020 2020 2020 7c31 3032              |102
+000075b0: 3420 c2b1 2034 2020 2020 2020 2020 2020  4 .. 4          
+000075c0: 2020 2020 2020 2020 2020 2020 7c35 3332              |532
+000075d0: 3520 c2b1 2031 3320 2020 2020 2020 2020  5 .. 13         
+000075e0: 2020 2020 2020 2020 2020 207c 3836 3833             |8683
+000075f0: 20c2 b120 3520 2020 2020 2020 2020 2020   .. 5           
+00007600: 2020 2020 2020 2020 2020 207c 0a7c 526f             |.|Ro
+00007610: 7461 7465 2020 2020 2020 2020 2020 207c  tate           |
+00007620: 3631 3020 c2b1 2034 2020 2020 2020 2020  610 .. 4        
+00007630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007640: 2020 2020 2020 207c 3135 3320 c2b1 2032         |153 .. 2
+00007650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007670: 2020 2020 207c 3230 3420 c2b1 2031 2020       |204 .. 1  
+00007680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007690: 2020 2020 207c 2a2a 3632 3620 c2b1 2033       |**626 .. 3
+000076a0: 2a2a 2020 2020 2020 2020 2020 2020 2020  **              
+000076b0: 2020 2020 7c34 3939 20c2 b120 3520 2020      |499 .. 5   
+000076c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000076d0: 2020 2020 7c0a 7c41 6666 696e 6520 2020      |.|Affine   
+000076e0: 2020 2020 2020 2020 7c2a 2a31 3730 3520          |**1705 
+000076f0: c2b1 2036 372a 2a20 2020 2020 2020 2020  .. 67**         
+00007700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007710: 7c31 3539 20c2 b120 3120 2020 2020 2020  |159 .. 1       
+00007720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007730: 2020 2020 2020 2020 2020 2020 2020 7c32                |2
+00007740: 3030 20c2 b120 3120 2020 2020 2020 2020  00 .. 1         
+00007750: 2020 2020 2020 2020 2020 2020 2020 7c2d                |-
+00007760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007770: 2020 2020 2020 2020 2020 2020 7c36 3633              |663
+00007780: 20c2 b120 3234 2020 2020 2020 2020 2020   .. 24          
+00007790: 2020 2020 2020 2020 2020 2020 7c0a 7c45              |.|E
+000077a0: 7175 616c 697a 6520 2020 2020 2020 2020  qualize         
+000077b0: 7c2a 2a31 3036 3120 c2b1 2031 342a 2a20  |**1061 .. 14** 
+000077c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000077d0: 2020 2020 2020 2020 7c33 3337 20c2 b120          |337 .. 
+000077e0: 3120 2020 2020 2020 2020 2020 2020 2020  1               
+000077f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007800: 2020 2020 2020 7c37 3720 c2b1 2031 2020        |77 .. 1  
+00007810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007820: 2020 2020 2020 7c2d 2020 2020 2020 2020        |-        
+00007830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007840: 2020 2020 7c38 3435 20c2 b120 3333 2020      |845 .. 33  
+00007850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007860: 2020 2020 7c0a 7c52 616e 646f 6d43 726f      |.|RandomCro
+00007870: 7036 3420 2020 2020 7c2a 2a32 3033 3139  p64     |**20319
+00007880: 3720 c2b1 2032 3130 352a 2a20 2020 2020  7 .. 2105**     
+00007890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000078a0: 7c31 3539 3331 20c2 b120 3237 2020 2020  |15931 .. 27    
+000078b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000078c0: 2020 2020 2020 2020 2020 2020 2020 7c38                |8
+000078d0: 3337 20c2 b120 3220 2020 2020 2020 2020  37 .. 2         
+000078e0: 2020 2020 2020 2020 2020 2020 2020 7c32                |2
+000078f0: 3138 3538 20c2 b120 3336 3220 2020 2020  1858 .. 362     
+00007900: 2020 2020 2020 2020 2020 2020 207c 3536               |56
+00007910: 3831 20c2 b120 3936 2020 2020 2020 2020  81 .. 96        
+00007920: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+00007930: 5261 6e64 6f6d 5265 7369 7a65 6443 726f  RandomResizedCro
+00007940: 707c 2a2a 3239 3938 20c2 b120 3330 2a2a  p|**2998 .. 30**
+00007950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007960: 2020 2020 2020 2020 207c 3131 3630 20c2           |1160 .
+00007970: b120 3420 2020 2020 2020 2020 2020 2020  . 4             
+00007980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007990: 2020 2020 2020 207c 3139 3020 c2b1 2031         |190 .. 1
+000079a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000079b0: 2020 2020 2020 207c 2d20 2020 2020 2020         |-       
+000079c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000079d0: 2020 2020 207c 2d20 2020 2020 2020 2020       |-         
+000079e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000079f0: 2020 2020 7c0a 7c53 6869 6674 5247 4220      |.|ShiftRGB 
+00007a00: 2020 2020 2020 2020 7c31 3430 3020 c2b1          |1400 ..
+00007a10: 2033 2020 2020 2020 2020 2020 2020 2020   3              
+00007a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a30: 7c2d 2020 2020 2020 2020 2020 2020 2020  |-              
+00007a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a50: 2020 2020 2020 2020 2020 2020 207c 3433               |43
+00007a60: 3520 c2b1 2031 2020 2020 2020 2020 2020  5 .. 1          
+00007a70: 2020 2020 2020 2020 2020 2020 207c 2d20               |- 
 00007a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a90: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-00007aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ab0: 2020 2035 3938 327c 2020 2020 2020 2020     5982|        
-00007ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ad0: 2020 2020 2020 2020 3332 3838 7c20 2020          3288|   
+00007a90: 2020 2020 2020 2020 2020 207c 2a2a 3135             |**15
+00007aa0: 3238 20c2 b120 362a 2a20 2020 2020 2020  28 .. 6**       
+00007ab0: 2020 2020 2020 2020 2020 207c 0a7c 5265             |.|Re
+00007ac0: 7369 7a65 2020 2020 2020 2020 2020 207c  size           |
+00007ad0: 2a2a 3235 3831 20c2 b120 332a 2a20 2020  **2581 .. 3**   
 00007ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007af0: 2020 2020 2020 2032 3137 327c 2020 2020         2172|    
-00007b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b10: 2020 2020 2020 2020 2020 3239 3432 7c20            2942| 
-00007b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b30: 2020 2020 2020 2038 3630 317c 0a7c 5665         8601|.|Ve
-00007b40: 7274 6963 616c 466c 6970 2020 2020 2020  rticalFlip      
-00007b50: 2020 2020 7c2a 2a31 3230 3332 2a2a 2020      |**12032**  
-00007b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b70: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-00007b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b90: 2020 2020 2020 3635 3839 7c20 2020 2020        6589|     
-00007ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007bb0: 2020 2020 2020 2020 2020 2033 3839 347c             3894|
-00007bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007bd0: 2020 2020 2020 2020 2020 3138 3433 7c20            1843| 
-00007be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007bf0: 2020 2020 2020 2020 2020 2020 2033 3539               359
-00007c00: 317c 2020 2020 2020 2020 2020 2020 2020  1|              
-00007c10: 2020 2020 2020 2020 2020 3737 3939 7c0a            7799|.
-00007c20: 7c52 6f74 6174 6520 2020 2020 2020 2020  |Rotate         
-00007c30: 2020 2020 2020 207c 2a2a 3630 302a 2a20         |**600** 
-00007c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c50: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00007c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c70: 2020 2020 2020 2020 2020 3530 357c 2020            505|  
-00007c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c90: 2020 2020 2020 2020 2020 2020 2020 2032                 2
-00007ca0: 3535 7c20 2020 2020 2020 2020 2020 2020  55|             
-00007cb0: 2020 2020 2020 2020 2020 2020 2020 2032                 2
-00007cc0: 317c 2020 2020 2020 2020 2020 2020 2020  1|              
-00007cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ce0: 2020 3933 7c20 2020 2020 2020 2020 2020    93|           
-00007cf0: 2020 2020 2020 2020 2020 2020 2020 3535                55
-00007d00: 337c 0a7c 5368 6966 7453 6361 6c65 526f  3|.|ShiftScaleRo
-00007d10: 7461 7465 2020 2020 2020 7c2a 2a39 3332  tate      |**932
-00007d20: 2a2a 2020 2020 2020 2020 2020 2020 2020  **              
-00007d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d40: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-00007d50: 2020 2020 2020 2020 2020 2020 2036 3835               685
-00007d60: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-00007d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d80: 2020 3232 347c 2d20 2020 2020 2020 2020    224|-         
-00007d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007da0: 2020 2020 7c2d 2020 2020 2020 2020 2020      |-          
-00007db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007dc0: 2020 2020 2020 207c 2d20 2020 2020 2020         |-       
-00007dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007de0: 2020 2020 7c0a 7c42 7269 6768 746e 6573      |.|Brightnes
-00007df0: 7343 6f6e 7472 6173 7420 2020 207c 2a2a  sContrast    |**
-00007e00: 3437 3337 2a2a 2020 2020 2020 2020 2020  4737**          
-00007e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e20: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
-00007e30: 2020 2020 2020 2020 2020 2020 2020 2031                 1
-00007e40: 3432 347c 2020 2020 2020 2020 2020 2020  424|            
+00007af0: 2020 2020 2020 207c 3132 3339 20c2 b120         |1239 .. 
+00007b00: 3120 2020 2020 2020 2020 2020 2020 2020  1               
+00007b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b20: 2020 2020 207c 3139 3720 c2b1 2031 2020       |197 .. 1  
+00007b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b40: 2020 2020 207c 3433 3120 c2b1 2031 2020       |431 .. 1  
+00007b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b60: 2020 2020 7c31 3732 3820 c2b1 2031 2020      |1728 .. 1  
+00007b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b80: 2020 2020 7c0a 7c52 616e 646f 6d47 616d      |.|RandomGam
+00007b90: 6d61 2020 2020 2020 7c2a 2a34 3535 3620  ma      |**4556 
+00007ba0: c2b1 2033 2a2a 2020 2020 2020 2020 2020  .. 3**          
+00007bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007bc0: 7c32 3330 20c2 b120 3120 2020 2020 2020  |230 .. 1       
+00007bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007be0: 2020 2020 2020 2020 2020 2020 2020 7c32                |2
+00007bf0: 3035 20c2 b120 3120 2020 2020 2020 2020  05 .. 1         
+00007c00: 2020 2020 2020 2020 2020 2020 2020 7c2d                |-
+00007c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c20: 2020 2020 2020 2020 2020 2020 7c32 3238              |228
+00007c30: 3220 c2b1 2031 3130 2020 2020 2020 2020  2 .. 110        
+00007c40: 2020 2020 2020 2020 2020 2020 7c0a 7c47              |.|G
+00007c50: 7261 7973 6361 6c65 2020 2020 2020 2020  rayscale        
+00007c60: 7c2a 2a37 3233 3420 c2b1 2034 2a2a 2020  |**7234 .. 4**  
+00007c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c80: 2020 2020 2020 2020 7c31 3533 3920 c2b1          |1539 ..
+00007c90: 2037 2020 2020 2020 2020 2020 2020 2020   7              
+00007ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007cb0: 2020 2020 2020 7c34 3434 20c2 b120 3320        |444 .. 3 
+00007cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007cd0: 2020 2020 2020 7c32 3630 3620 c2b1 2032        |2606 .. 2
+00007ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007cf0: 2020 2020 207c 3931 3820 c2b1 2034 3220       |918 .. 42 
+00007d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d10: 2020 2020 207c 0a7c 436f 6c6f 724a 6974       |.|ColorJit
+00007d20: 7465 7220 2020 2020 207c 2a2a 3435 3220  ter      |**452 
+00007d30: c2b1 2034 332a 2a20 2020 2020 2020 2020  .. 43**         
+00007d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d50: 207c 3531 20c2 b120 3120 2020 2020 2020   |51 .. 1       
+00007d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d70: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00007d80: 3530 20c2 b120 3120 2020 2020 2020 2020  50 .. 1         
+00007d90: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00007da0: 3232 3120 c2b1 2031 2020 2020 2020 2020  221 .. 1        
+00007db0: 2020 2020 2020 2020 2020 2020 2020 7c2d                |-
+00007dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007dd0: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+00007de0: 5261 6e64 6f6d 5065 7273 7065 6374 6976  RandomPerspectiv
+00007df0: 657c 2a2a 3436 3520 c2b1 2031 2a2a 2020  e|**465 .. 1**  
+00007e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007e10: 2020 2020 2020 2020 207c 3132 3120 c2b1           |121 ..
+00007e20: 2031 2020 2020 2020 2020 2020 2020 2020   1              
+00007e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007e40: 2020 2020 2020 207c 3131 3520 c2b1 2031         |115 .. 1
 00007e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e60: 2020 2020 2032 3537 7c20 2020 2020 2020       257|       
+00007e60: 2020 2020 2020 207c 2d20 2020 2020 2020         |-       
 00007e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e80: 2020 2020 3532 337c 2020 2020 2020 2020      523|        
+00007e80: 2020 2020 207c 3433 3320 c2b1 2031 3620       |433 .. 16 
 00007e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ea0: 2020 2020 2020 2032 3537 7c20 2020 2020         257|     
-00007eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ec0: 2020 2032 3036 347c 0a7c 5368 6966 7452     2064|.|ShiftR
-00007ed0: 4742 2020 2020 2020 2020 2020 2020 2020  GB              
-00007ee0: 7c2a 2a34 3735 382a 2a20 2020 2020 2020  |**4758**       
+00007ea0: 2020 2020 207c 0a7c 4761 7573 7369 616e       |.|Gaussian
+00007eb0: 426c 7572 2020 2020 207c 2a2a 3233 3135  Blur     |**2315
+00007ec0: 20c2 b120 392a 2a20 2020 2020 2020 2020   .. 9**         
+00007ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ee0: 207c 3130 3620 c2b1 2032 2020 2020 2020   |106 .. 2      
 00007ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f00: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-00007f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f20: 2020 3234 3739 7c2d 2020 2020 2020 2020    2479|-        
-00007f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f40: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-00007f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f60: 2020 2020 2020 2032 3531 7c2d 2020 2020         251|-    
-00007f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f80: 2020 2020 2020 2020 2020 2020 207c 2d20               |- 
+00007f00: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00007f10: 3732 20c2 b120 3120 2020 2020 2020 2020  72 .. 1         
+00007f20: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00007f30: 3136 3120 c2b1 2031 2020 2020 2020 2020  161 .. 1        
+00007f40: 2020 2020 2020 2020 2020 2020 2020 7c31                |1
+00007f50: 3231 3320 c2b1 2033 2020 2020 2020 2020  213 .. 3        
+00007f60: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+00007f70: 7c4d 6564 6961 6e42 6c75 7220 2020 2020  |MedianBlur     
+00007f80: 2020 7c2a 2a33 3731 3120 c2b1 2032 2a2a    |**3711 .. 2**
 00007f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007fa0: 2020 2020 2020 2020 2020 7c0a 7c53 6869            |.|Shi
-00007fb0: 6674 4853 5620 2020 2020 2020 2020 2020  ftHSV           
-00007fc0: 2020 207c 2a2a 3837 382a 2a20 2020 2020     |**878**     
-00007fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007fe0: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-00007ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008000: 2020 2020 2020 3339 357c 2020 2020 2020        395|      
-00008010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008020: 2020 2020 2020 2020 2020 2020 3935 7c20              95| 
-00008030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008040: 2020 2020 2020 2020 2020 3131 327c 2d20            112|- 
-00008050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007fa0: 2020 2020 2020 2020 2020 7c2d 2020 2020            |-    
+00007fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007fd0: 2020 2020 2020 207c 3220 c2b1 2031 2020         |2 .. 1  
+00007fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ff0: 2020 2020 2020 207c 2d20 2020 2020 2020         |-       
+00008000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008010: 2020 2020 207c 3536 3620 c2b1 2033 2020       |566 .. 3  
+00008020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008030: 2020 2020 207c 0a7c 4d6f 7469 6f6e 426c       |.|MotionBl
+00008040: 7572 2020 2020 2020 207c 2a2a 3237 3633  ur       |**2763
+00008050: 20c2 b120 3235 2a2a 2020 2020 2020 2020   .. 25**        
 00008060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008070: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-00008080: 2020 2020 2020 2020 2020 3235 317c 0a7c            251|.|
-00008090: 5261 6e64 6f6d 4761 6d6d 6120 2020 2020  RandomGamma     
-000080a0: 2020 2020 2020 7c2a 2a34 3837 312a 2a20        |**4871** 
-000080b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000080c0: 2020 2020 2020 2020 2020 2020 207c 2d20               |- 
-000080d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000080e0: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-000080f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008100: 2020 2020 2020 2020 2020 2020 2031 3530               150
-00008110: 397c 2020 2020 2020 2020 2020 2020 2020  9|              
-00008120: 2020 2020 2020 2020 2020 2020 2032 3836               286
-00008130: 7c2d 2020 2020 2020 2020 2020 2020 2020  |-              
-00008140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008150: 2020 207c 2020 2020 2020 2020 2020 2020     |            
-00008160: 2020 2020 2020 2020 2020 2020 3135 3430              1540
-00008170: 7c0a 7c47 7261 7973 6361 6c65 2020 2020  |.|Grayscale    
-00008180: 2020 2020 2020 2020 207c 2a2a 3737 3930           |**7790
-00008190: 2a2a 2020 2020 2020 2020 2020 2020 2020  **              
-000081a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000081b0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-000081c0: 2020 2020 2020 2020 2020 2031 3137 397c             1179|
-000081d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000081e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000081f0: 3133 3838 7c20 2020 2020 2020 2020 2020  1388|           
-00008200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008210: 3639 387c 2020 2020 2020 2020 2020 2020  698|            
-00008220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008230: 2020 3235 3637 7c20 2020 2020 2020 2020    2567|         
-00008240: 2020 2020 2020 2020 2020 2020 2020 2032                 2
-00008250: 3733 377c 0a7c 5261 6e64 6f6d 4372 6f70  737|.|RandomCrop
-00008260: 3634 2020 2020 2020 2020 2020 7c2a 2a32  64          |**2
-00008270: 3031 3239 382a 2a20 2020 2020 2020 2020  01298**         
-00008280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008290: 2020 207c 2020 2020 2020 2020 2020 2020     |            
-000082a0: 2020 2020 2020 2020 2020 2020 2020 3630                60
-000082b0: 3133 7c20 2020 2020 2020 2020 2020 2020  13|             
-000082c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000082d0: 2020 3634 3332 307c 2020 2020 2020 2020    64320|        
+00008070: 207c 2d20 2020 2020 2020 2020 2020 2020   |-             
+00008080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008090: 2020 2020 2020 2020 2020 2020 2020 7c31                |1
+000080a0: 3031 20c2 b120 3420 2020 2020 2020 2020  01 .. 4         
+000080b0: 2020 2020 2020 2020 2020 2020 2020 7c2d                |-
+000080c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000080d0: 2020 2020 2020 2020 2020 2020 7c35 3038              |508
+000080e0: 20c2 b120 3220 2020 2020 2020 2020 2020   .. 2           
+000080f0: 2020 2020 2020 2020 2020 2020 7c0a 7c50              |.|P
+00008100: 6f73 7465 7269 7a65 2020 2020 2020 2020  osterize        
+00008110: 7c2a 2a34 3233 3820 c2b1 2035 312a 2a20  |**4238 .. 51** 
+00008120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008130: 2020 2020 2020 2020 7c32 3538 3120 c2b1          |2581 ..
+00008140: 2032 3020 2020 2020 2020 2020 2020 2020   20             
+00008150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008160: 2020 2020 2020 7c32 3834 20c2 b120 3420        |284 .. 4 
+00008170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008180: 2020 2020 2020 7c2d 2020 2020 2020 2020        |-        
+00008190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000081a0: 2020 2020 7c31 3839 3320 c2b1 2039 2020      |1893 .. 9  
+000081b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000081c0: 2020 2020 7c0a 7c4a 7065 6743 6f6d 7072      |.|JpegCompr
+000081d0: 6573 7369 6f6e 2020 7c32 3038 20c2 b120  ession  |208 .. 
+000081e0: 3120 2020 2020 2020 2020 2020 2020 2020  1               
+000081f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008200: 7c2d 2020 2020 2020 2020 2020 2020 2020  |-              
+00008210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008220: 2020 2020 2020 2020 2020 2020 207c 2d20               |- 
+00008230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008240: 2020 2020 2020 2020 2020 2020 7c2a 2a36              |**6
+00008250: 3932 20c2 b120 342a 2a20 2020 2020 2020  92 .. 4**       
+00008260: 2020 2020 2020 2020 2020 207c 3433 3520             |435 
+00008270: c2b1 2031 2020 2020 2020 2020 2020 2020  .. 1            
+00008280: 2020 2020 2020 2020 2020 207c 0a7c 4761             |.|Ga
+00008290: 7573 7369 616e 4e6f 6973 6520 2020 207c  ussianNoise    |
+000082a0: 3634 20c2 b120 3920 2020 2020 2020 2020  64 .. 9         
+000082b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000082c0: 2020 2020 2020 207c 2d20 2020 2020 2020         |-       
+000082d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000082e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000082f0: 2020 3130 3131 7c20 2020 2020 2020 2020    1011|         
+000082f0: 2020 2020 7c2d 2020 2020 2020 2020 2020      |-          
 00008300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008310: 2020 2020 3631 3837 307c 2020 2020 2020      61870|      
+00008310: 2020 207c 3637 20c2 b120 3120 2020 2020     |67 .. 1     
 00008320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008330: 2032 3632 3630 7c0a 7c50 6164 546f 5369   26260|.|PadToSi
-00008340: 7a65 3531 3220 2020 2020 2020 2020 207c  ze512          |
-00008350: 2a2a 3831 3536 2a2a 2020 2020 2020 2020  **8156**        
-00008360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008370: 2020 2020 2020 7c2d 2020 2020 2020 2020        |-        
-00008380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008390: 2020 2020 207c 2020 2020 2020 2020 2020       |          
+00008330: 2020 7c2a 2a32 3132 20c2 b120 3136 2a2a    |**212 .. 16**
+00008340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008350: 2020 7c0a 7c45 6c61 7374 6963 2020 2020    |.|Elastic    
+00008360: 2020 2020 2020 7c2a 2a31 3239 20c2 b120        |**129 .. 
+00008370: 312a 2a20 2020 2020 2020 2020 2020 2020  1**             
+00008380: 2020 2020 2020 2020 2020 2020 2020 7c33                |3
+00008390: 20c2 b120 3120 2020 2020 2020 2020 2020   .. 1           
 000083a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000083b0: 2020 2020 2020 3130 3531 7c2d 2020 2020        1051|-    
-000083c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000083d0: 2020 2020 2020 2020 207c 2d20 2020 2020           |-     
+000083b0: 2020 2020 2020 2020 2020 2020 7c31 20c2              |1 .
+000083c0: b120 3120 2020 2020 2020 2020 2020 2020  . 1             
+000083d0: 2020 2020 2020 2020 2020 2020 7c2d 2020              |-  
 000083e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000083f0: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-00008400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008410: 2020 2020 2035 3835 317c 0a7c 5265 7369       5851|.|Resi
-00008420: 7a65 3531 3220 2020 2020 2020 2020 2020  ze512           
-00008430: 2020 7c2a 2a32 3636 372a 2a20 2020 2020    |**2667**     
-00008440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008450: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-00008460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008470: 2020 2020 3137 3737 7c20 2020 2020 2020      1777|       
-00008480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008490: 2020 2020 2020 2020 2020 3430 377c 2020            407|  
-000084a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000084b0: 2020 2020 2020 2020 2035 3137 7c20 2020           517|   
-000084c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000084d0: 2020 2020 2020 2020 2020 2020 3430 397c              409|
-000084e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000084f0: 2020 2020 2020 2020 3234 3530 7c0a 7c52          2450|.|R
-00008500: 616e 646f 6d53 697a 6564 4372 6f70 5f36  andomSizedCrop_6
-00008510: 345f 3531 327c 2a2a 3532 3234 2a2a 2020  4_512|**5224**  
-00008520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008530: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-00008540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008550: 2020 2020 2020 2032 3137 307c 2020 2020         2170|    
-00008560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008570: 2020 2020 2020 2020 2020 2020 2036 3638               668
-00008580: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-00008590: 2020 2020 2020 2020 2020 2020 3337 387c              378|
-000085a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000085b0: 2020 2020 2020 2020 2020 2020 2020 2036                 6
-000085c0: 3730 7c20 2020 2020 2020 2020 2020 2020  70|             
-000085d0: 2020 2020 2020 2020 2020 2034 3132 307c             4120|
-000085e0: 0a7c 4571 7561 6c69 7a65 2020 2020 2020  .|Equalize      
-000085f0: 2020 2020 2020 2020 7c2a 2a31 3039 342a          |**1094*
-00008600: 2a20 2020 2020 2020 2020 2020 2020 2020  *               
-00008610: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00008620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008630: 2020 2020 2020 2020 2020 2035 3631 7c2d             561|-
-00008640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008660: 2020 207c 2d20 2020 2020 2020 2020 2020     |-           
-00008670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008680: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-00008690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000086a0: 2020 3938 347c 2d20 2020 2020 2020 2020    984|-         
-000086b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000086c0: 2020 7c0a 7c4d 756c 7469 706c 7920 2020    |.|Multiply   
-000086d0: 2020 2020 2020 2020 2020 207c 2a2a 3436             |**46
-000086e0: 3830 2a2a 2020 2020 2020 2020 2020 2020  80**            
-000086f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008700: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-00008710: 2020 2020 2020 2020 2020 2020 2032 3632               262
-00008720: 337c 2d20 2020 2020 2020 2020 2020 2020  3|-             
-00008730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008740: 2020 2020 2020 7c2d 2020 2020 2020 2020        |-        
-00008750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008760: 2020 2020 207c 2d20 2020 2020 2020 2020       |-         
-00008770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008780: 2020 2020 2020 2020 7c2d 2020 2020 2020          |-      
-00008790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000087a0: 2020 2020 207c 0a7c 4d75 6c74 6970 6c79       |.|Multiply
-000087b0: 456c 656d 656e 7477 6973 6520 2020 7c2a  Elementwise   |*
-000087c0: 2a34 3533 322a 2a20 2020 2020 2020 2020  *4532**         
-000087d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000087e0: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-000087f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008800: 3130 3037 7c2d 2020 2020 2020 2020 2020  1007|-          
-00008810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008820: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-00008830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008840: 2020 2020 2034 3533 7c2d 2020 2020 2020       453|-      
-00008850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008860: 2020 2020 2020 2020 2020 207c 2d20 2020             |-   
-00008870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008880: 2020 2020 2020 2020 7c0a 7c43 6f6c 6f72          |.|Color
-00008890: 4a69 7474 6572 2020 2020 2020 2020 2020  Jitter          
-000088a0: 207c 2a2a 3534 342a 2a20 2020 2020 2020   |**544**       
-000088b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000088c0: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-000088d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000088e0: 2020 2020 3130 387c 2020 2020 2020 2020      108|        
-000088f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008900: 2020 2020 2020 2020 2020 3834 7c20 2020            84|   
-00008910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008920: 2020 2020 2020 2020 3131 367c 2d20 2020          116|-   
-00008930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008940: 2020 2020 2020 2020 2020 2020 2020 7c2d                |-
-00008950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008960: 2020 2020 2020 2020 2020 207c 0a0a 5079             |..Py
-00008970: 7468 6f6e 2061 6e64 206c 6962 7261 7279  thon and library
-00008980: 2076 6572 7369 6f6e 733a 2050 7974 686f   versions: Pytho
-00008990: 6e20 332e 3130 2e31 332c 206e 756d 7079  n 3.10.13, numpy
-000089a0: 2031 2e32 362e 342c 2070 696c 6c6f 772d   1.26.4, pillow-
-000089b0: 7369 6d64 2031 302e 322e 302c 206f 7065  simd 10.2.0, ope
-000089c0: 6e63 762d 7079 7468 6f6e 2034 2e39 2e30  ncv-python 4.9.0
-000089d0: 2e38 302c 2073 6369 6b69 742d 696d 6167  .80, scikit-imag
-000089e0: 6520 302e 3232 2e30 2c20 7363 6970 7920  e 0.22.0, scipy 
-000089f0: 312e 3132 2e30 2e0a 0a23 2320 436f 6e74  1.12.0...## Cont
-00008a00: 7269 6275 7469 6e67 0a0a 546f 2063 7265  ributing..To cre
-00008a10: 6174 6520 6120 7075 6c6c 2072 6571 7565  ate a pull reque
-00008a20: 7374 2074 6f20 7468 6520 7265 706f 7369  st to the reposi
-00008a30: 746f 7279 2c20 666f 6c6c 6f77 2074 6865  tory, follow the
-00008a40: 2064 6f63 756d 656e 7461 7469 6f6e 2061   documentation a
-00008a50: 7420 5b43 4f4e 5452 4942 5554 494e 472e  t [CONTRIBUTING.
-00008a60: 6d64 5d28 434f 4e54 5249 4255 5449 4e47  md](CONTRIBUTING
-00008a70: 2e6d 6429 0a0a 215b 6874 7470 733a 2f2f  .md)..![https://
-00008a80: 6769 7468 7562 2e63 6f6d 2f61 6c62 7565  github.com/albue
-00008a90: 6d6e 7461 7469 6f6e 732d 7465 616d 2f61  mntations-team/a
-00008aa0: 6c62 756d 656e 7461 7469 6f6e 2f67 7261  lbumentation/gra
-00008ab0: 7068 732f 636f 6e74 7269 6275 746f 7273  phs/contributors
-00008ac0: 5d28 6874 7470 733a 2f2f 636f 6e74 7269  ](https://contri
-00008ad0: 622e 726f 636b 732f 696d 6167 653f 7265  b.rocks/image?re
-00008ae0: 706f 3d61 6c62 756d 656e 7461 7469 6f6e  po=albumentation
-00008af0: 732d 7465 616d 2f61 6c62 756d 656e 7461  s-team/albumenta
-00008b00: 7469 6f6e 7329 0a0a 2323 2043 6f6d 6d75  tions)..## Commu
-00008b10: 6e69 7479 2061 6e64 2053 7570 706f 7274  nity and Support
-00008b20: 0a0a 2d20 5b54 7769 7474 6572 5d28 6874  ..- [Twitter](ht
-00008b30: 7470 733a 2f2f 7477 6974 7465 722e 636f  tps://twitter.co
-00008b40: 6d2f 616c 6275 6d65 6e74 6174 696f 6e73  m/albumentations
-00008b50: 290a 2d20 5b44 6973 636f 7264 5d28 6874  ).- [Discord](ht
-00008b60: 7470 733a 2f2f 6469 7363 6f72 642e 6767  tps://discord.gg
-00008b70: 2f41 4b50 7272 4459 4e41 7429 0a0a 2323  /AKPrrDYNAt)..##
-00008b80: 2043 6f6d 6d65 6e74 730a 0a49 6e20 736f   Comments..In so
-00008b90: 6d65 2073 7973 7465 6d73 2c20 696e 2074  me systems, in t
-00008ba0: 6865 206d 756c 7469 706c 6520 4750 5520  he multiple GPU 
-00008bb0: 7265 6769 6d65 2c20 5079 546f 7263 6820  regime, PyTorch 
-00008bc0: 6d61 7920 6465 6164 6c6f 636b 2074 6865  may deadlock the
-00008bd0: 2044 6174 614c 6f61 6465 7220 6966 204f   DataLoader if O
-00008be0: 7065 6e43 5620 7761 7320 636f 6d70 696c  penCV was compil
-00008bf0: 6564 2077 6974 6820 4f70 656e 434c 206f  ed with OpenCL o
-00008c00: 7074 696d 697a 6174 696f 6e73 2e20 4164  ptimizations. Ad
-00008c10: 6469 6e67 2074 6865 2066 6f6c 6c6f 7769  ding the followi
-00008c20: 6e67 2074 776f 206c 696e 6573 2062 6566  ng two lines bef
-00008c30: 6f72 6520 7468 6520 6c69 6272 6172 7920  ore the library 
-00008c40: 696d 706f 7274 206d 6179 2068 656c 702e  import may help.
-00008c50: 2046 6f72 206d 6f72 6520 6465 7461 696c   For more detail
-00008c60: 7320 5b68 7474 7073 3a2f 2f67 6974 6875  s [https://githu
-00008c70: 622e 636f 6d2f 7079 746f 7263 682f 7079  b.com/pytorch/py
-00008c80: 746f 7263 682f 6973 7375 6573 2f31 3335  torch/issues/135
-00008c90: 355d 2868 7474 7073 3a2f 2f67 6974 6875  5](https://githu
-00008ca0: 622e 636f 6d2f 7079 746f 7263 682f 7079  b.com/pytorch/py
-00008cb0: 746f 7263 682f 6973 7375 6573 2f31 3335  torch/issues/135
-00008cc0: 3529 0a0a 6060 6070 7974 686f 6e0a 6376  5)..```python.cv
-00008cd0: 322e 7365 744e 756d 5468 7265 6164 7328  2.setNumThreads(
-00008ce0: 3029 0a63 7632 2e6f 636c 2e73 6574 5573  0).cv2.ocl.setUs
-00008cf0: 654f 7065 6e43 4c28 4661 6c73 6529 0a60  eOpenCL(False).`
-00008d00: 6060 0a0a 2323 2043 6974 696e 670a 0a49  ``..## Citing..I
-00008d10: 6620 796f 7520 6669 6e64 2074 6869 7320  f you find this 
-00008d20: 6c69 6272 6172 7920 7573 6566 756c 2066  library useful f
-00008d30: 6f72 2079 6f75 7220 7265 7365 6172 6368  or your research
-00008d40: 2c20 706c 6561 7365 2063 6f6e 7369 6465  , please conside
-00008d50: 7220 6369 7469 6e67 205b 416c 6275 6d65  r citing [Albume
-00008d60: 6e74 6174 696f 6e73 3a20 4661 7374 2061  ntations: Fast a
-00008d70: 6e64 2046 6c65 7869 626c 6520 496d 6167  nd Flexible Imag
-00008d80: 6520 4175 676d 656e 7461 7469 6f6e 735d  e Augmentations]
-00008d90: 2868 7474 7073 3a2f 2f77 7777 2e6d 6470  (https://www.mdp
-00008da0: 692e 636f 6d2f 3230 3738 2d32 3438 392f  i.com/2078-2489/
-00008db0: 3131 2f32 2f31 3235 293a 0a0a 6060 6062  11/2/125):..```b
-00008dc0: 6962 7465 780a 4041 7274 6963 6c65 7b69  ibtex.@Article{i
-00008dd0: 6e66 6f31 3130 3230 3132 352c 0a20 2020  nfo11020125,.   
-00008de0: 2041 5554 484f 5220 3d20 7b42 7573 6c61   AUTHOR = {Busla
-00008df0: 6576 2c20 416c 6578 616e 6465 7220 616e  ev, Alexander an
-00008e00: 6420 4967 6c6f 7669 6b6f 762c 2056 6c61  d Iglovikov, Vla
-00008e10: 6469 6d69 7220 492e 2061 6e64 204b 6876  dimir I. and Khv
-00008e20: 6564 6368 656e 7961 2c20 4575 6765 6e65  edchenya, Eugene
-00008e30: 2061 6e64 2050 6172 696e 6f76 2c20 416c   and Parinov, Al
-00008e40: 6578 2061 6e64 2044 7275 7a68 696e 696e  ex and Druzhinin
-00008e50: 2c20 4d69 6b68 6169 6c20 616e 6420 4b61  , Mikhail and Ka
-00008e60: 6c69 6e69 6e2c 2041 6c65 7861 6e64 7220  linin, Alexandr 
-00008e70: 412e 7d2c 0a20 2020 2054 4954 4c45 203d  A.},.    TITLE =
-00008e80: 207b 416c 6275 6d65 6e74 6174 696f 6e73   {Albumentations
-00008e90: 3a20 4661 7374 2061 6e64 2046 6c65 7869  : Fast and Flexi
-00008ea0: 626c 6520 496d 6167 6520 4175 676d 656e  ble Image Augmen
-00008eb0: 7461 7469 6f6e 737d 2c0a 2020 2020 4a4f  tations},.    JO
-00008ec0: 5552 4e41 4c20 3d20 7b49 6e66 6f72 6d61  URNAL = {Informa
-00008ed0: 7469 6f6e 7d2c 0a20 2020 2056 4f4c 554d  tion},.    VOLUM
-00008ee0: 4520 3d20 7b31 317d 2c0a 2020 2020 5945  E = {11},.    YE
-00008ef0: 4152 203d 207b 3230 3230 7d2c 0a20 2020  AR = {2020},.   
-00008f00: 204e 554d 4245 5220 3d20 7b32 7d2c 0a20   NUMBER = {2},. 
-00008f10: 2020 2041 5254 4943 4c45 2d4e 554d 4245     ARTICLE-NUMBE
-00008f20: 5220 3d20 7b31 3235 7d2c 0a20 2020 2055  R = {125},.    U
-00008f30: 524c 203d 207b 6874 7470 733a 2f2f 7777  RL = {https://ww
-00008f40: 772e 6d64 7069 2e63 6f6d 2f32 3037 382d  w.mdpi.com/2078-
-00008f50: 3234 3839 2f31 312f 322f 3132 357d 2c0a  2489/11/2/125},.
-00008f60: 2020 2020 4953 534e 203d 207b 3230 3738      ISSN = {2078
-00008f70: 2d32 3438 397d 2c0a 2020 2020 444f 4920  -2489},.    DOI 
-00008f80: 3d20 7b31 302e 3333 3930 2f69 6e66 6f31  = {10.3390/info1
-00008f90: 3130 3230 3132 357d 0a7d 0a60 6060 0a    1020125}.}.```.
+000083f0: 2020 2020 2020 2020 2020 7c31 3238 20c2            |128 .
+00008400: b120 3120 2020 2020 2020 2020 2020 2020  . 1             
+00008410: 2020 2020 2020 2020 2020 7c0a 0a23 2320            |..## 
+00008420: 436f 6e74 7269 6275 7469 6e67 0a0a 546f  Contributing..To
+00008430: 2063 7265 6174 6520 6120 7075 6c6c 2072   create a pull r
+00008440: 6571 7565 7374 2074 6f20 7468 6520 7265  equest to the re
+00008450: 706f 7369 746f 7279 2c20 666f 6c6c 6f77  pository, follow
+00008460: 2074 6865 2064 6f63 756d 656e 7461 7469   the documentati
+00008470: 6f6e 2061 7420 5b43 4f4e 5452 4942 5554  on at [CONTRIBUT
+00008480: 494e 472e 6d64 5d28 434f 4e54 5249 4255  ING.md](CONTRIBU
+00008490: 5449 4e47 2e6d 6429 0a0a 215b 6874 7470  TING.md)..![http
+000084a0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f61  s://github.com/a
+000084b0: 6c62 7565 6d6e 7461 7469 6f6e 732d 7465  lbuemntations-te
+000084c0: 616d 2f61 6c62 756d 656e 7461 7469 6f6e  am/albumentation
+000084d0: 2f67 7261 7068 732f 636f 6e74 7269 6275  /graphs/contribu
+000084e0: 746f 7273 5d28 6874 7470 733a 2f2f 636f  tors](https://co
+000084f0: 6e74 7269 622e 726f 636b 732f 696d 6167  ntrib.rocks/imag
+00008500: 653f 7265 706f 3d61 6c62 756d 656e 7461  e?repo=albumenta
+00008510: 7469 6f6e 732d 7465 616d 2f61 6c62 756d  tions-team/album
+00008520: 656e 7461 7469 6f6e 7329 0a0a 2323 2043  entations)..## C
+00008530: 6f6d 6d75 6e69 7479 2061 6e64 2053 7570  ommunity and Sup
+00008540: 706f 7274 0a0a 2d20 5b54 7769 7474 6572  port..- [Twitter
+00008550: 5d28 6874 7470 733a 2f2f 7477 6974 7465  ](https://twitte
+00008560: 722e 636f 6d2f 616c 6275 6d65 6e74 6174  r.com/albumentat
+00008570: 696f 6e73 290a 2d20 5b44 6973 636f 7264  ions).- [Discord
+00008580: 5d28 6874 7470 733a 2f2f 6469 7363 6f72  ](https://discor
+00008590: 642e 6767 2f41 4b50 7272 4459 4e41 7429  d.gg/AKPrrDYNAt)
+000085a0: 0a0a 2323 2043 6f6d 6d65 6e74 730a 0a49  ..## Comments..I
+000085b0: 6e20 736f 6d65 2073 7973 7465 6d73 2c20  n some systems, 
+000085c0: 696e 2074 6865 206d 756c 7469 706c 6520  in the multiple 
+000085d0: 4750 5520 7265 6769 6d65 2c20 5079 546f  GPU regime, PyTo
+000085e0: 7263 6820 6d61 7920 6465 6164 6c6f 636b  rch may deadlock
+000085f0: 2074 6865 2044 6174 614c 6f61 6465 7220   the DataLoader 
+00008600: 6966 204f 7065 6e43 5620 7761 7320 636f  if OpenCV was co
+00008610: 6d70 696c 6564 2077 6974 6820 4f70 656e  mpiled with Open
+00008620: 434c 206f 7074 696d 697a 6174 696f 6e73  CL optimizations
+00008630: 2e20 4164 6469 6e67 2074 6865 2066 6f6c  . Adding the fol
+00008640: 6c6f 7769 6e67 2074 776f 206c 696e 6573  lowing two lines
+00008650: 2062 6566 6f72 6520 7468 6520 6c69 6272   before the libr
+00008660: 6172 7920 696d 706f 7274 206d 6179 2068  ary import may h
+00008670: 656c 702e 2046 6f72 206d 6f72 6520 6465  elp. For more de
+00008680: 7461 696c 7320 5b68 7474 7073 3a2f 2f67  tails [https://g
+00008690: 6974 6875 622e 636f 6d2f 7079 746f 7263  ithub.com/pytorc
+000086a0: 682f 7079 746f 7263 682f 6973 7375 6573  h/pytorch/issues
+000086b0: 2f31 3335 355d 2868 7474 7073 3a2f 2f67  /1355](https://g
+000086c0: 6974 6875 622e 636f 6d2f 7079 746f 7263  ithub.com/pytorc
+000086d0: 682f 7079 746f 7263 682f 6973 7375 6573  h/pytorch/issues
+000086e0: 2f31 3335 3529 0a0a 6060 6070 7974 686f  /1355)..```pytho
+000086f0: 6e0a 6376 322e 7365 744e 756d 5468 7265  n.cv2.setNumThre
+00008700: 6164 7328 3029 0a63 7632 2e6f 636c 2e73  ads(0).cv2.ocl.s
+00008710: 6574 5573 654f 7065 6e43 4c28 4661 6c73  etUseOpenCL(Fals
+00008720: 6529 0a60 6060 0a0a 2323 2043 6974 696e  e).```..## Citin
+00008730: 670a 0a49 6620 796f 7520 6669 6e64 2074  g..If you find t
+00008740: 6869 7320 6c69 6272 6172 7920 7573 6566  his library usef
+00008750: 756c 2066 6f72 2079 6f75 7220 7265 7365  ul for your rese
+00008760: 6172 6368 2c20 706c 6561 7365 2063 6f6e  arch, please con
+00008770: 7369 6465 7220 6369 7469 6e67 205b 416c  sider citing [Al
+00008780: 6275 6d65 6e74 6174 696f 6e73 3a20 4661  bumentations: Fa
+00008790: 7374 2061 6e64 2046 6c65 7869 626c 6520  st and Flexible 
+000087a0: 496d 6167 6520 4175 676d 656e 7461 7469  Image Augmentati
+000087b0: 6f6e 735d 2868 7474 7073 3a2f 2f77 7777  ons](https://www
+000087c0: 2e6d 6470 692e 636f 6d2f 3230 3738 2d32  .mdpi.com/2078-2
+000087d0: 3438 392f 3131 2f32 2f31 3235 293a 0a0a  489/11/2/125):..
+000087e0: 6060 6062 6962 7465 780a 4041 7274 6963  ```bibtex.@Artic
+000087f0: 6c65 7b69 6e66 6f31 3130 3230 3132 352c  le{info11020125,
+00008800: 0a20 2020 2041 5554 484f 5220 3d20 7b42  .    AUTHOR = {B
+00008810: 7573 6c61 6576 2c20 416c 6578 616e 6465  uslaev, Alexande
+00008820: 7220 616e 6420 4967 6c6f 7669 6b6f 762c  r and Iglovikov,
+00008830: 2056 6c61 6469 6d69 7220 492e 2061 6e64   Vladimir I. and
+00008840: 204b 6876 6564 6368 656e 7961 2c20 4575   Khvedchenya, Eu
+00008850: 6765 6e65 2061 6e64 2050 6172 696e 6f76  gene and Parinov
+00008860: 2c20 416c 6578 2061 6e64 2044 7275 7a68  , Alex and Druzh
+00008870: 696e 696e 2c20 4d69 6b68 6169 6c20 616e  inin, Mikhail an
+00008880: 6420 4b61 6c69 6e69 6e2c 2041 6c65 7861  d Kalinin, Alexa
+00008890: 6e64 7220 412e 7d2c 0a20 2020 2054 4954  ndr A.},.    TIT
+000088a0: 4c45 203d 207b 416c 6275 6d65 6e74 6174  LE = {Albumentat
+000088b0: 696f 6e73 3a20 4661 7374 2061 6e64 2046  ions: Fast and F
+000088c0: 6c65 7869 626c 6520 496d 6167 6520 4175  lexible Image Au
+000088d0: 676d 656e 7461 7469 6f6e 737d 2c0a 2020  gmentations},.  
+000088e0: 2020 4a4f 5552 4e41 4c20 3d20 7b49 6e66    JOURNAL = {Inf
+000088f0: 6f72 6d61 7469 6f6e 7d2c 0a20 2020 2056  ormation},.    V
+00008900: 4f4c 554d 4520 3d20 7b31 317d 2c0a 2020  OLUME = {11},.  
+00008910: 2020 5945 4152 203d 207b 3230 3230 7d2c    YEAR = {2020},
+00008920: 0a20 2020 204e 554d 4245 5220 3d20 7b32  .    NUMBER = {2
+00008930: 7d2c 0a20 2020 2041 5254 4943 4c45 2d4e  },.    ARTICLE-N
+00008940: 554d 4245 5220 3d20 7b31 3235 7d2c 0a20  UMBER = {125},. 
+00008950: 2020 2055 524c 203d 207b 6874 7470 733a     URL = {https:
+00008960: 2f2f 7777 772e 6d64 7069 2e63 6f6d 2f32  //www.mdpi.com/2
+00008970: 3037 382d 3234 3839 2f31 312f 322f 3132  078-2489/11/2/12
+00008980: 357d 2c0a 2020 2020 4953 534e 203d 207b  5},.    ISSN = {
+00008990: 3230 3738 2d32 3438 397d 2c0a 2020 2020  2078-2489},.    
+000089a0: 444f 4920 3d20 7b31 302e 3333 3930 2f69  DOI = {10.3390/i
+000089b0: 6e66 6f31 3130 3230 3132 357d 0a7d 0a60  nfo11020125}.}.`
+000089c0: 6060 0a                                  ``.
```

### Comparing `albumentations-1.4.2/README.md` & `albumentations-1.4.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,2189 +1,2314 @@
-00000000: 2320 416c 6275 6d65 6e74 6174 696f 6e73  # Albumentations
-00000010: 0a0a 5b21 5b50 7950 4920 7665 7273 696f  ..[![PyPI versio
-00000020: 6e5d 2868 7474 7073 3a2f 2f62 6164 6765  n](https://badge
-00000030: 2e66 7572 792e 696f 2f70 792f 616c 6275  .fury.io/py/albu
-00000040: 6d65 6e74 6174 696f 6e73 2e73 7667 295d  mentations.svg)]
-00000050: 2868 7474 7073 3a2f 2f62 6164 6765 2e66  (https://badge.f
-00000060: 7572 792e 696f 2f70 792f 616c 6275 6d65  ury.io/py/albume
-00000070: 6e74 6174 696f 6e73 290a 215b 4349 5d28  ntations).![CI](
-00000080: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000090: 6f6d 2f61 6c62 756d 656e 7461 7469 6f6e  om/albumentation
-000000a0: 732d 7465 616d 2f61 6c62 756d 656e 7461  s-team/albumenta
-000000b0: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
-000000c0: 4349 2f62 6164 6765 2e73 7667 290a 5b21  CI/badge.svg).[!
-000000d0: 5b4c 6963 656e 7365 3a20 4d49 545d 2868  [License: MIT](h
-000000e0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-000000f0: 6473 2e69 6f2f 6261 6467 652f 4c69 6365  ds.io/badge/Lice
-00000100: 6e73 652d 4d49 542d 6272 6967 6874 6772  nse-MIT-brightgr
-00000110: 6565 6e2e 7376 6729 5d28 6874 7470 733a  een.svg)](https:
-00000120: 2f2f 6f70 656e 736f 7572 6365 2e6f 7267  //opensource.org
-00000130: 2f6c 6963 656e 7365 732f 4d49 5429 0a5b  /licenses/MIT).[
-00000140: 215b 5275 6666 5d28 6874 7470 733a 2f2f  ![Ruff](https://
-00000150: 696d 672e 7368 6965 6c64 732e 696f 2f65  img.shields.io/e
-00000160: 6e64 706f 696e 743f 7572 6c3d 6874 7470  ndpoint?url=http
-00000170: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
-00000180: 6572 636f 6e74 656e 742e 636f 6d2f 6173  ercontent.com/as
-00000190: 7472 616c 2d73 682f 7275 6666 2f6d 6169  tral-sh/ruff/mai
-000001a0: 6e2f 6173 7365 7473 2f62 6164 6765 2f76  n/assets/badge/v
-000001b0: 322e 6a73 6f6e 295d 2868 7474 7073 3a2f  2.json)](https:/
-000001c0: 2f67 6974 6875 622e 636f 6d2f 6173 7472  /github.com/astr
-000001d0: 616c 2d73 682f 7275 6666 290a 0a5b 4469  al-sh/ruff)..[Di
-000001e0: 7363 6f72 645d 2868 7474 7073 3a2f 2f64  scord](https://d
-000001f0: 6973 636f 7264 2e67 672f 414b 5072 7244  iscord.gg/AKPrrD
-00000200: 594e 4174 2920 7c20 5b54 7769 7474 6572  YNAt) | [Twitter
-00000210: 5d28 6874 7470 733a 2f2f 7477 6974 7465  ](https://twitte
-00000220: 722e 636f 6d2f 616c 6275 6d65 6e74 6174  r.com/albumentat
-00000230: 696f 6e73 2920 7c20 5b44 6f63 735d 2868  ions) | [Docs](h
-00000240: 7474 7073 3a2f 2f61 6c62 756d 656e 7461  ttps://albumenta
-00000250: 7469 6f6e 732e 6169 2f64 6f63 732f 290a  tions.ai/docs/).
-00000260: 0a41 6c62 756d 656e 7461 7469 6f6e 7320  .Albumentations 
-00000270: 6973 2061 2050 7974 686f 6e20 6c69 6272  is a Python libr
-00000280: 6172 7920 666f 7220 696d 6167 6520 6175  ary for image au
-00000290: 676d 656e 7461 7469 6f6e 2e20 496d 6167  gmentation. Imag
-000002a0: 6520 6175 676d 656e 7461 7469 6f6e 2069  e augmentation i
-000002b0: 7320 7573 6564 2069 6e20 6465 6570 206c  s used in deep l
-000002c0: 6561 726e 696e 6720 616e 6420 636f 6d70  earning and comp
-000002d0: 7574 6572 2076 6973 696f 6e20 7461 736b  uter vision task
-000002e0: 7320 746f 2069 6e63 7265 6173 6520 7468  s to increase th
-000002f0: 6520 7175 616c 6974 7920 6f66 2074 7261  e quality of tra
-00000300: 696e 6564 206d 6f64 656c 732e 2054 6865  ined models. The
-00000310: 2070 7572 706f 7365 206f 6620 696d 6167   purpose of imag
-00000320: 6520 6175 676d 656e 7461 7469 6f6e 2069  e augmentation i
-00000330: 7320 746f 2063 7265 6174 6520 6e65 7720  s to create new 
-00000340: 7472 6169 6e69 6e67 2073 616d 706c 6573  training samples
-00000350: 2066 726f 6d20 7468 6520 6578 6973 7469   from the existi
-00000360: 6e67 2064 6174 612e 0a0a 4865 7265 2069  ng data...Here i
-00000370: 7320 616e 2065 7861 6d70 6c65 206f 6620  s an example of 
-00000380: 686f 7720 796f 7520 6361 6e20 6170 706c  how you can appl
-00000390: 7920 736f 6d65 205b 7069 7865 6c2d 6c65  y some [pixel-le
-000003a0: 7665 6c5d 2823 7069 7865 6c2d 6c65 7665  vel](#pixel-leve
-000003b0: 6c2d 7472 616e 7366 6f72 6d73 2920 6175  l-transforms) au
-000003c0: 676d 656e 7461 7469 6f6e 7320 6672 6f6d  gmentations from
-000003d0: 2041 6c62 756d 656e 7461 7469 6f6e 7320   Albumentations 
-000003e0: 746f 2063 7265 6174 6520 6e65 7720 696d  to create new im
-000003f0: 6167 6573 2066 726f 6d20 7468 6520 6f72  ages from the or
-00000400: 6967 696e 616c 206f 6e65 3a0a 215b 7061  iginal one:.![pa
-00000410: 7272 6f74 5d28 6874 7470 733a 2f2f 6861  rrot](https://ha
-00000420: 6272 6173 746f 7261 6765 2e6f 7267 2f77  brastorage.org/w
-00000430: 6562 742f 6264 2f6e 652f 7276 2f62 646e  ebt/bd/ne/rv/bdn
-00000440: 6572 7635 6374 6b75 646d 7361 7a6e 6877  erv5ctkudmsaznhw
-00000450: 3463 7273 6466 6977 2e6a 7065 6729 0a0a  4crsdfiw.jpeg)..
-00000460: 2323 2057 6879 2041 6c62 756d 656e 7461  ## Why Albumenta
-00000470: 7469 6f6e 730a 0a2d 2041 6c62 756d 656e  tions..- Albumen
-00000480: 7461 7469 6f6e 7320 2a2a 5b73 7570 706f  tations **[suppo
-00000490: 7274 7320 616c 6c20 636f 6d6d 6f6e 2063  rts all common c
-000004a0: 6f6d 7075 7465 7220 7669 7369 6f6e 2074  omputer vision t
-000004b0: 6173 6b73 5d28 2369 2d77 616e 742d 746f  asks](#i-want-to
-000004c0: 2d75 7365 2d61 6c62 756d 656e 7461 7469  -use-albumentati
-000004d0: 6f6e 732d 666f 722d 7468 652d 7370 6563  ons-for-the-spec
-000004e0: 6966 6963 2d74 6173 6b2d 7375 6368 2d61  ific-task-such-a
-000004f0: 732d 636c 6173 7369 6669 6361 7469 6f6e  s-classification
-00000500: 2d6f 722d 7365 676d 656e 7461 7469 6f6e  -or-segmentation
-00000510: 292a 2a20 7375 6368 2061 7320 636c 6173  )** such as clas
-00000520: 7369 6669 6361 7469 6f6e 2c20 7365 6d61  sification, sema
-00000530: 6e74 6963 2073 6567 6d65 6e74 6174 696f  ntic segmentatio
-00000540: 6e2c 2069 6e73 7461 6e63 6520 7365 676d  n, instance segm
-00000550: 656e 7461 7469 6f6e 2c20 6f62 6a65 6374  entation, object
-00000560: 2064 6574 6563 7469 6f6e 2c20 616e 6420   detection, and 
-00000570: 706f 7365 2065 7374 696d 6174 696f 6e2e  pose estimation.
-00000580: 0a2d 2054 6865 206c 6962 7261 7279 2070  .- The library p
-00000590: 726f 7669 6465 7320 2a2a 5b61 2073 696d  rovides **[a sim
-000005a0: 706c 6520 756e 6966 6965 6420 4150 495d  ple unified API]
-000005b0: 2823 612d 7369 6d70 6c65 2d65 7861 6d70  (#a-simple-examp
-000005c0: 6c65 292a 2a20 746f 2077 6f72 6b20 7769  le)** to work wi
-000005d0: 7468 2061 6c6c 2064 6174 6120 7479 7065  th all data type
-000005e0: 733a 2069 6d61 6765 7320 2852 4247 2d69  s: images (RBG-i
-000005f0: 6d61 6765 732c 2067 7261 7973 6361 6c65  mages, grayscale
-00000600: 2069 6d61 6765 732c 206d 756c 7469 7370   images, multisp
-00000610: 6563 7472 616c 2069 6d61 6765 7329 2c20  ectral images), 
-00000620: 7365 676d 656e 7461 7469 6f6e 206d 6173  segmentation mas
-00000630: 6b73 2c20 626f 756e 6469 6e67 2062 6f78  ks, bounding box
-00000640: 6573 2c20 616e 6420 6b65 7970 6f69 6e74  es, and keypoint
-00000650: 732e 0a2d 2054 6865 206c 6962 7261 7279  s..- The library
-00000660: 2063 6f6e 7461 696e 7320 2a2a 5b6d 6f72   contains **[mor
-00000670: 6520 7468 616e 2037 3020 6469 6666 6572  e than 70 differ
-00000680: 656e 7420 6175 676d 656e 7461 7469 6f6e  ent augmentation
-00000690: 735d 2823 6c69 7374 2d6f 662d 6175 676d  s](#list-of-augm
-000006a0: 656e 7461 7469 6f6e 7329 2a2a 2074 6f20  entations)** to 
-000006b0: 6765 6e65 7261 7465 206e 6577 2074 7261  generate new tra
-000006c0: 696e 696e 6720 7361 6d70 6c65 7320 6672  ining samples fr
-000006d0: 6f6d 2074 6865 2065 7869 7374 696e 6720  om the existing 
-000006e0: 6461 7461 2e0a 2d20 416c 6275 6d65 6e74  data..- Albument
-000006f0: 6174 696f 6e73 2069 7320 5b2a 2a66 6173  ations is [**fas
-00000700: 742a 2a5d 2823 6265 6e63 686d 6172 6b69  t**](#benchmarki
-00000710: 6e67 2d72 6573 756c 7473 292e 2057 6520  ng-results). We 
-00000720: 6265 6e63 686d 6172 6b20 6561 6368 206e  benchmark each n
-00000730: 6577 2072 656c 6561 7365 2074 6f20 656e  ew release to en
-00000740: 7375 7265 2074 6861 7420 6175 676d 656e  sure that augmen
-00000750: 7461 7469 6f6e 7320 7072 6f76 6964 6520  tations provide 
-00000760: 6d61 7869 6d75 6d20 7370 6565 642e 0a2d  maximum speed..-
-00000770: 2049 7420 2a2a 5b77 6f72 6b73 2077 6974   It **[works wit
-00000780: 6820 706f 7075 6c61 7220 6465 6570 206c  h popular deep l
-00000790: 6561 726e 696e 6720 6672 616d 6577 6f72  earning framewor
-000007a0: 6b73 5d28 2369 2d77 616e 742d 746f 2d6b  ks](#i-want-to-k
-000007b0: 6e6f 772d 686f 772d 746f 2d75 7365 2d61  now-how-to-use-a
-000007c0: 6c62 756d 656e 7461 7469 6f6e 732d 7769  lbumentations-wi
-000007d0: 7468 2d64 6565 702d 6c65 6172 6e69 6e67  th-deep-learning
-000007e0: 2d66 7261 6d65 776f 726b 7329 2a2a 2073  -frameworks)** s
-000007f0: 7563 6820 6173 2050 7954 6f72 6368 2061  uch as PyTorch a
-00000800: 6e64 2054 656e 736f 7246 6c6f 772e 2042  nd TensorFlow. B
-00000810: 7920 7468 6520 7761 792c 2041 6c62 756d  y the way, Album
-00000820: 656e 7461 7469 6f6e 7320 6973 2061 2070  entations is a p
-00000830: 6172 7420 6f66 2074 6865 205b 5079 546f  art of the [PyTo
-00000840: 7263 6820 6563 6f73 7973 7465 6d5d 2868  rch ecosystem](h
-00000850: 7474 7073 3a2f 2f70 7974 6f72 6368 2e6f  ttps://pytorch.o
-00000860: 7267 2f65 636f 7379 7374 656d 2f29 2e0a  rg/ecosystem/)..
-00000870: 2d20 5b2a 2a57 7269 7474 656e 2062 7920  - [**Written by 
-00000880: 6578 7065 7274 732a 2a5d 2823 6175 7468  experts**](#auth
-00000890: 6f72 7329 2e20 5468 6520 6175 7468 6f72  ors). The author
-000008a0: 7320 6861 7665 2065 7870 6572 6965 6e63  s have experienc
-000008b0: 6520 626f 7468 2077 6f72 6b69 6e67 206f  e both working o
-000008c0: 6e20 7072 6f64 7563 7469 6f6e 2063 6f6d  n production com
-000008d0: 7075 7465 7220 7669 7369 6f6e 2073 7973  puter vision sys
-000008e0: 7465 6d73 2061 6e64 2070 6172 7469 6369  tems and partici
-000008f0: 7061 7469 6e67 2069 6e20 636f 6d70 6574  pating in compet
-00000900: 6974 6976 6520 6d61 6368 696e 6520 6c65  itive machine le
-00000910: 6172 6e69 6e67 2e20 4d61 6e79 2063 6f72  arning. Many cor
-00000920: 6520 7465 616d 206d 656d 6265 7273 2061  e team members a
-00000930: 7265 204b 6167 676c 6520 4d61 7374 6572  re Kaggle Master
-00000940: 7320 616e 6420 4772 616e 646d 6173 7465  s and Grandmaste
-00000950: 7273 2e0a 2d20 5468 6520 6c69 6272 6172  rs..- The librar
-00000960: 7920 6973 205b 2a2a 7769 6465 6c79 2075  y is [**widely u
-00000970: 7365 642a 2a5d 2823 7768 6f2d 6973 2d75  sed**](#who-is-u
-00000980: 7369 6e67 2d61 6c62 756d 656e 7461 7469  sing-albumentati
-00000990: 6f6e 7329 2069 6e20 696e 6475 7374 7279  ons) in industry
-000009a0: 2c20 6465 6570 206c 6561 726e 696e 6720  , deep learning 
-000009b0: 7265 7365 6172 6368 2c20 6d61 6368 696e  research, machin
-000009c0: 6520 6c65 6172 6e69 6e67 2063 6f6d 7065  e learning compe
-000009d0: 7469 7469 6f6e 732c 2061 6e64 206f 7065  titions, and ope
-000009e0: 6e20 736f 7572 6365 2070 726f 6a65 6374  n source project
-000009f0: 732e 0a0a 2323 2053 706f 6e73 6f72 730a  s...## Sponsors.
-00000a00: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
-00000a10: 2f2f 726f 626f 666c 6f77 2e63 6f6d 2f22  //roboflow.com/"
-00000a20: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
-00000a30: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
-00000a40: 3a2f 2f61 7661 7461 7273 2e67 6974 6875  ://avatars.githu
-00000a50: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
-00000a60: 2f75 2f35 3331 3034 3131 383f 733d 3230  /u/53104118?s=20
-00000a70: 3026 763d 3422 2077 6964 7468 3d22 3130  0&v=4" width="10
-00000a80: 3022 2f3e 3c2f 613e 0a0a 2323 2054 6162  0"/></a>..## Tab
-00000a90: 6c65 206f 6620 636f 6e74 656e 7473 0a0a  le of contents..
-00000aa0: 2d20 5b41 6c62 756d 656e 7461 7469 6f6e  - [Albumentation
-00000ab0: 735d 2823 616c 6275 6d65 6e74 6174 696f  s](#albumentatio
-00000ac0: 6e73 290a 2020 2d20 5b57 6879 2041 6c62  ns).  - [Why Alb
-00000ad0: 756d 656e 7461 7469 6f6e 735d 2823 7768  umentations](#wh
-00000ae0: 792d 616c 6275 6d65 6e74 6174 696f 6e73  y-albumentations
-00000af0: 290a 2020 2d20 5b53 706f 6e73 6f72 735d  ).  - [Sponsors]
-00000b00: 2823 7370 6f6e 736f 7273 290a 2020 2d20  (#sponsors).  - 
-00000b10: 5b54 6162 6c65 206f 6620 636f 6e74 656e  [Table of conten
-00000b20: 7473 5d28 2374 6162 6c65 2d6f 662d 636f  ts](#table-of-co
-00000b30: 6e74 656e 7473 290a 2020 2d20 5b41 7574  ntents).  - [Aut
-00000b40: 686f 7273 5d28 2361 7574 686f 7273 290a  hors](#authors).
-00000b50: 2020 2d20 5b49 6e73 7461 6c6c 6174 696f    - [Installatio
-00000b60: 6e5d 2823 696e 7374 616c 6c61 7469 6f6e  n](#installation
-00000b70: 290a 2020 2d20 5b44 6f63 756d 656e 7461  ).  - [Documenta
-00000b80: 7469 6f6e 5d28 2364 6f63 756d 656e 7461  tion](#documenta
-00000b90: 7469 6f6e 290a 2020 2d20 5b41 2073 696d  tion).  - [A sim
-00000ba0: 706c 6520 6578 616d 706c 655d 2823 612d  ple example](#a-
-00000bb0: 7369 6d70 6c65 2d65 7861 6d70 6c65 290a  simple-example).
-00000bc0: 2020 2d20 5b47 6574 7469 6e67 2073 7461    - [Getting sta
-00000bd0: 7274 6564 5d28 2367 6574 7469 6e67 2d73  rted](#getting-s
-00000be0: 7461 7274 6564 290a 2020 2020 2d20 5b49  tarted).    - [I
-00000bf0: 2061 6d20 6e65 7720 746f 2069 6d61 6765   am new to image
-00000c00: 2061 7567 6d65 6e74 6174 696f 6e5d 2823   augmentation](#
-00000c10: 692d 616d 2d6e 6577 2d74 6f2d 696d 6167  i-am-new-to-imag
-00000c20: 652d 6175 676d 656e 7461 7469 6f6e 290a  e-augmentation).
-00000c30: 2020 2020 2d20 5b49 2077 616e 7420 746f      - [I want to
-00000c40: 2075 7365 2041 6c62 756d 656e 7461 7469   use Albumentati
-00000c50: 6f6e 7320 666f 7220 7468 6520 7370 6563  ons for the spec
-00000c60: 6966 6963 2074 6173 6b20 7375 6368 2061  ific task such a
-00000c70: 7320 636c 6173 7369 6669 6361 7469 6f6e  s classification
-00000c80: 206f 7220 7365 676d 656e 7461 7469 6f6e   or segmentation
-00000c90: 5d28 2369 2d77 616e 742d 746f 2d75 7365  ](#i-want-to-use
-00000ca0: 2d61 6c62 756d 656e 7461 7469 6f6e 732d  -albumentations-
-00000cb0: 666f 722d 7468 652d 7370 6563 6966 6963  for-the-specific
-00000cc0: 2d74 6173 6b2d 7375 6368 2d61 732d 636c  -task-such-as-cl
-00000cd0: 6173 7369 6669 6361 7469 6f6e 2d6f 722d  assification-or-
-00000ce0: 7365 676d 656e 7461 7469 6f6e 290a 2020  segmentation).  
-00000cf0: 2020 2d20 5b49 2077 616e 7420 746f 206b    - [I want to k
-00000d00: 6e6f 7720 686f 7720 746f 2075 7365 2041  now how to use A
-00000d10: 6c62 756d 656e 7461 7469 6f6e 7320 7769  lbumentations wi
-00000d20: 7468 2064 6565 7020 6c65 6172 6e69 6e67  th deep learning
-00000d30: 2066 7261 6d65 776f 726b 735d 2823 692d   frameworks](#i-
-00000d40: 7761 6e74 2d74 6f2d 6b6e 6f77 2d68 6f77  want-to-know-how
-00000d50: 2d74 6f2d 7573 652d 616c 6275 6d65 6e74  -to-use-albument
-00000d60: 6174 696f 6e73 2d77 6974 682d 6465 6570  ations-with-deep
-00000d70: 2d6c 6561 726e 696e 672d 6672 616d 6577  -learning-framew
-00000d80: 6f72 6b73 290a 2020 2020 2d20 5b49 2077  orks).    - [I w
-00000d90: 616e 7420 746f 2065 7870 6c6f 7265 2061  ant to explore a
-00000da0: 7567 6d65 6e74 6174 696f 6e73 2061 6e64  ugmentations and
-00000db0: 2073 6565 2041 6c62 756d 656e 7461 7469   see Albumentati
-00000dc0: 6f6e 7320 696e 2061 6374 696f 6e5d 2823  ons in action](#
-00000dd0: 692d 7761 6e74 2d74 6f2d 6578 706c 6f72  i-want-to-explor
-00000de0: 652d 6175 676d 656e 7461 7469 6f6e 732d  e-augmentations-
-00000df0: 616e 642d 7365 652d 616c 6275 6d65 6e74  and-see-albument
-00000e00: 6174 696f 6e73 2d69 6e2d 6163 7469 6f6e  ations-in-action
-00000e10: 290a 2020 2d20 5b57 686f 2069 7320 7573  ).  - [Who is us
-00000e20: 696e 6720 416c 6275 6d65 6e74 6174 696f  ing Albumentatio
-00000e30: 6e73 5d28 2377 686f 2d69 732d 7573 696e  ns](#who-is-usin
-00000e40: 672d 616c 6275 6d65 6e74 6174 696f 6e73  g-albumentations
-00000e50: 290a 2020 2020 2d20 5b53 6565 2061 6c73  ).    - [See als
-00000e60: 6f5d 2823 7365 652d 616c 736f 290a 2020  o](#see-also).  
-00000e70: 2d20 5b4c 6973 7420 6f66 2061 7567 6d65  - [List of augme
-00000e80: 6e74 6174 696f 6e73 5d28 236c 6973 742d  ntations](#list-
-00000e90: 6f66 2d61 7567 6d65 6e74 6174 696f 6e73  of-augmentations
-00000ea0: 290a 2020 2020 2d20 5b50 6978 656c 2d6c  ).    - [Pixel-l
-00000eb0: 6576 656c 2074 7261 6e73 666f 726d 735d  evel transforms]
-00000ec0: 2823 7069 7865 6c2d 6c65 7665 6c2d 7472  (#pixel-level-tr
-00000ed0: 616e 7366 6f72 6d73 290a 2020 2020 2d20  ansforms).    - 
-00000ee0: 5b53 7061 7469 616c 2d6c 6576 656c 2074  [Spatial-level t
-00000ef0: 7261 6e73 666f 726d 735d 2823 7370 6174  ransforms](#spat
-00000f00: 6961 6c2d 6c65 7665 6c2d 7472 616e 7366  ial-level-transf
-00000f10: 6f72 6d73 290a 2020 2020 2d20 5b4d 6978  orms).    - [Mix
-00000f20: 696e 672d 6c65 7665 6c20 7472 616e 7366  ing-level transf
-00000f30: 6f72 6d73 5d28 236d 6978 696e 672d 6c65  orms](#mixing-le
-00000f40: 7665 6c2d 7472 616e 7366 6f72 6d73 290a  vel-transforms).
-00000f50: 2020 2d20 5b41 2066 6577 206d 6f72 6520    - [A few more 
-00000f60: 6578 616d 706c 6573 206f 6620 2a2a 6175  examples of **au
-00000f70: 676d 656e 7461 7469 6f6e 732a 2a5d 2823  gmentations**](#
-00000f80: 612d 6665 772d 6d6f 7265 2d65 7861 6d70  a-few-more-examp
-00000f90: 6c65 732d 6f66 2d61 7567 6d65 6e74 6174  les-of-augmentat
-00000fa0: 696f 6e73 290a 2020 2020 2d20 5b53 656d  ions).    - [Sem
-00000fb0: 616e 7469 6320 7365 676d 656e 7461 7469  antic segmentati
-00000fc0: 6f6e 206f 6e20 7468 6520 496e 7269 6120  on on the Inria 
-00000fd0: 6461 7461 7365 745d 2823 7365 6d61 6e74  dataset](#semant
-00000fe0: 6963 2d73 6567 6d65 6e74 6174 696f 6e2d  ic-segmentation-
-00000ff0: 6f6e 2d74 6865 2d69 6e72 6961 2d64 6174  on-the-inria-dat
-00001000: 6173 6574 290a 2020 2020 2d20 5b4d 6564  aset).    - [Med
-00001010: 6963 616c 2069 6d61 6769 6e67 5d28 236d  ical imaging](#m
-00001020: 6564 6963 616c 2d69 6d61 6769 6e67 290a  edical-imaging).
-00001030: 2020 2020 2d20 5b4f 626a 6563 7420 6465      - [Object de
-00001040: 7465 6374 696f 6e20 616e 6420 7365 6d61  tection and sema
-00001050: 6e74 6963 2073 6567 6d65 6e74 6174 696f  ntic segmentatio
-00001060: 6e20 6f6e 2074 6865 204d 6170 696c 6c61  n on the Mapilla
-00001070: 7279 2056 6973 7461 7320 6461 7461 7365  ry Vistas datase
-00001080: 745d 2823 6f62 6a65 6374 2d64 6574 6563  t](#object-detec
-00001090: 7469 6f6e 2d61 6e64 2d73 656d 616e 7469  tion-and-semanti
-000010a0: 632d 7365 676d 656e 7461 7469 6f6e 2d6f  c-segmentation-o
-000010b0: 6e2d 7468 652d 6d61 7069 6c6c 6172 792d  n-the-mapillary-
-000010c0: 7669 7374 6173 2d64 6174 6173 6574 290a  vistas-dataset).
-000010d0: 2020 2020 2d20 5b4b 6579 706f 696e 7473      - [Keypoints
-000010e0: 2061 7567 6d65 6e74 6174 696f 6e5d 2823   augmentation](#
-000010f0: 6b65 7970 6f69 6e74 732d 6175 676d 656e  keypoints-augmen
-00001100: 7461 7469 6f6e 290a 2020 2d20 5b42 656e  tation).  - [Ben
-00001110: 6368 6d61 726b 696e 6720 7265 7375 6c74  chmarking result
-00001120: 735d 2823 6265 6e63 686d 6172 6b69 6e67  s](#benchmarking
-00001130: 2d72 6573 756c 7473 290a 2020 2d20 5b43  -results).  - [C
-00001140: 6f6e 7472 6962 7574 696e 675d 2823 636f  ontributing](#co
-00001150: 6e74 7269 6275 7469 6e67 290a 2020 2d20  ntributing).  - 
-00001160: 5b43 6f6d 6d75 6e69 7479 2061 6e64 2053  [Community and S
-00001170: 7570 706f 7274 5d28 2363 6f6d 6d75 6e69  upport](#communi
-00001180: 7479 2d61 6e64 2d73 7570 706f 7274 290a  ty-and-support).
-00001190: 2020 2d20 5b43 6f6d 6d65 6e74 735d 2823    - [Comments](#
-000011a0: 636f 6d6d 656e 7473 290a 2020 2d20 5b43  comments).  - [C
-000011b0: 6974 696e 675d 2823 6369 7469 6e67 290a  iting](#citing).
-000011c0: 0a23 2320 4175 7468 6f72 730a 0a5b 2a2a  .## Authors..[**
-000011d0: 566c 6164 696d 6972 2049 2e20 4967 6c6f  Vladimir I. Iglo
-000011e0: 7669 6b6f 762a 2a5d 2868 7474 7073 3a2f  vikov**](https:/
-000011f0: 2f77 7777 2e6c 696e 6b65 6469 6e2e 636f  /www.linkedin.co
-00001200: 6d2f 696e 2f69 676c 6f76 696b 6f76 2f29  m/in/iglovikov/)
-00001210: 207c 205b 4b61 6767 6c65 2047 7261 6e64   | [Kaggle Grand
-00001220: 6d61 7374 6572 5d28 6874 7470 733a 2f2f  master](https://
-00001230: 7777 772e 6b61 6767 6c65 2e63 6f6d 2f69  www.kaggle.com/i
-00001240: 676c 6f76 696b 6f76 290a 0a5b 2a2a 4d69  glovikov)..[**Mi
-00001250: 6b68 6169 6c20 4472 757a 6869 6e69 6e2a  khail Druzhinin*
-00001260: 2a5d 2868 7474 7073 3a2f 2f77 7777 2e6c  *](https://www.l
-00001270: 696e 6b65 6469 6e2e 636f 6d2f 696e 2f6d  inkedin.com/in/m
-00001280: 696b 6861 696c 2d64 7275 7a68 696e 696e  ikhail-druzhinin
-00001290: 2d35 3438 3232 3931 3030 2f29 207c 205b  -548229100/) | [
-000012a0: 4b61 6767 6c65 2045 7870 6572 745d 2868  Kaggle Expert](h
-000012b0: 7474 7073 3a2f 2f77 7777 2e6b 6167 676c  ttps://www.kaggl
-000012c0: 652e 636f 6d2f 6469 7065 746d 290a 0a5b  e.com/dipetm)..[
-000012d0: 2a2a 416c 6578 2050 6172 696e 6f76 2a2a  **Alex Parinov**
-000012e0: 5d28 6874 7470 733a 2f2f 7777 772e 6c69  ](https://www.li
-000012f0: 6e6b 6564 696e 2e63 6f6d 2f69 6e2f 616c  nkedin.com/in/al
-00001300: 6578 2d70 6172 696e 6f76 2f29 207c 205b  ex-parinov/) | [
-00001310: 4b61 6767 6c65 204d 6173 7465 725d 2868  Kaggle Master](h
-00001320: 7474 7073 3a2f 2f77 7777 2e6b 6167 676c  ttps://www.kaggl
-00001330: 652e 636f 6d2f 6372 6561 667a 290a 0a5b  e.com/creafz)..[
-00001340: 2a2a 416c 6578 616e 6465 7220 4275 736c  **Alexander Busl
-00001350: 6165 762a 2a20 e280 9420 436f 6d70 7574  aev** ... Comput
-00001360: 6572 2056 6973 696f 6e20 456e 6769 6e65  er Vision Engine
-00001370: 6572 2061 7420 4d61 7062 6f78 5d28 6874  er at Mapbox](ht
-00001380: 7470 733a 2f2f 7777 772e 6c69 6e6b 6564  tps://www.linked
-00001390: 696e 2e63 6f6d 2f69 6e2f 616c 2d62 7573  in.com/in/al-bus
-000013a0: 6c61 6576 2f29 207c 205b 4b61 6767 6c65  laev/) | [Kaggle
-000013b0: 204d 6173 7465 725d 2868 7474 7073 3a2f   Master](https:/
-000013c0: 2f77 7777 2e6b 6167 676c 652e 636f 6d2f  /www.kaggle.com/
-000013d0: 616c 6275 736c 6165 7629 0a0a 5b2a 2a45  albuslaev)..[**E
-000013e0: 7665 6765 6e65 204b 6876 6564 6368 656e  vegene Khvedchen
-000013f0: 7961 2a2a 20e2 8094 2043 6f6d 7075 7465  ya** ... Compute
-00001400: 7220 5669 7369 6f6e 2052 6573 6561 7263  r Vision Researc
-00001410: 6820 456e 6769 6e65 6572 2061 7420 5069  h Engineer at Pi
-00001420: c3b1 6174 6120 4661 726d 735d 2868 7474  ..ata Farms](htt
-00001430: 7073 3a2f 2f77 7777 2e6c 696e 6b65 6469  ps://www.linkedi
-00001440: 6e2e 636f 6d2f 696e 2f63 7674 616c 6b73  n.com/in/cvtalks
-00001450: 2f29 207c 205b 4b61 6767 6c65 2047 7261  /) | [Kaggle Gra
-00001460: 6e64 6d61 7374 6572 5d28 6874 7470 733a  ndmaster](https:
-00001470: 2f2f 7777 772e 6b61 6767 6c65 2e63 6f6d  //www.kaggle.com
-00001480: 2f62 6c6f 6f64 6178 6529 0a0a 2323 2049  /bloodaxe)..## I
-00001490: 6e73 7461 6c6c 6174 696f 6e0a 0a41 6c62  nstallation..Alb
-000014a0: 756d 656e 7461 7469 6f6e 7320 7265 7175  umentations requ
-000014b0: 6972 6573 2050 7974 686f 6e20 332e 3820  ires Python 3.8 
-000014c0: 6f72 2068 6967 6865 722e 2054 6f20 696e  or higher. To in
-000014d0: 7374 616c 6c20 7468 6520 6c61 7465 7374  stall the latest
-000014e0: 2076 6572 7369 6f6e 2066 726f 6d20 5079   version from Py
-000014f0: 5049 3a0a 0a60 6060 6261 7368 0a70 6970  PI:..```bash.pip
-00001500: 2069 6e73 7461 6c6c 202d 5520 616c 6275   install -U albu
-00001510: 6d65 6e74 6174 696f 6e73 0a60 6060 0a0a  mentations.```..
-00001520: 4f74 6865 7220 696e 7374 616c 6c61 7469  Other installati
-00001530: 6f6e 206f 7074 696f 6e73 2061 7265 2064  on options are d
-00001540: 6573 6372 6962 6564 2069 6e20 7468 6520  escribed in the 
-00001550: 5b64 6f63 756d 656e 7461 7469 6f6e 5d28  [documentation](
-00001560: 6874 7470 733a 2f2f 616c 6275 6d65 6e74  https://albument
-00001570: 6174 696f 6e73 2e61 692f 646f 6373 2f67  ations.ai/docs/g
-00001580: 6574 7469 6e67 5f73 7461 7274 6564 2f69  etting_started/i
-00001590: 6e73 7461 6c6c 6174 696f 6e2f 292e 0a0a  nstallation/)...
-000015a0: 2323 2044 6f63 756d 656e 7461 7469 6f6e  ## Documentation
-000015b0: 0a0a 5468 6520 6675 6c6c 2064 6f63 756d  ..The full docum
-000015c0: 656e 7461 7469 6f6e 2069 7320 6176 6169  entation is avai
-000015d0: 6c61 626c 6520 6174 202a 2a5b 6874 7470  lable at **[http
-000015e0: 733a 2f2f 616c 6275 6d65 6e74 6174 696f  s://albumentatio
-000015f0: 6e73 2e61 692f 646f 6373 2f5d 2868 7474  ns.ai/docs/](htt
-00001600: 7073 3a2f 2f61 6c62 756d 656e 7461 7469  ps://albumentati
-00001610: 6f6e 732e 6169 2f64 6f63 732f 292a 2a2e  ons.ai/docs/)**.
-00001620: 0a0a 2323 2041 2073 696d 706c 6520 6578  ..## A simple ex
-00001630: 616d 706c 650a 0a60 6060 7079 7468 6f6e  ample..```python
-00001640: 0a69 6d70 6f72 7420 616c 6275 6d65 6e74  .import albument
-00001650: 6174 696f 6e73 2061 7320 410a 696d 706f  ations as A.impo
-00001660: 7274 2063 7632 0a0a 2320 4465 636c 6172  rt cv2..# Declar
-00001670: 6520 616e 2061 7567 6d65 6e74 6174 696f  e an augmentatio
-00001680: 6e20 7069 7065 6c69 6e65 0a74 7261 6e73  n pipeline.trans
-00001690: 666f 726d 203d 2041 2e43 6f6d 706f 7365  form = A.Compose
-000016a0: 285b 0a20 2020 2041 2e52 616e 646f 6d43  ([.    A.RandomC
-000016b0: 726f 7028 7769 6474 683d 3235 362c 2068  rop(width=256, h
-000016c0: 6569 6768 743d 3235 3629 2c0a 2020 2020  eight=256),.    
-000016d0: 412e 486f 7269 7a6f 6e74 616c 466c 6970  A.HorizontalFlip
-000016e0: 2870 3d30 2e35 292c 0a20 2020 2041 2e52  (p=0.5),.    A.R
-000016f0: 616e 646f 6d42 7269 6768 746e 6573 7343  andomBrightnessC
-00001700: 6f6e 7472 6173 7428 703d 302e 3229 2c0a  ontrast(p=0.2),.
-00001710: 5d29 0a0a 2320 5265 6164 2061 6e20 696d  ])..# Read an im
-00001720: 6167 6520 7769 7468 204f 7065 6e43 5620  age with OpenCV 
-00001730: 616e 6420 636f 6e76 6572 7420 6974 2074  and convert it t
-00001740: 6f20 7468 6520 5247 4220 636f 6c6f 7273  o the RGB colors
-00001750: 7061 6365 0a69 6d61 6765 203d 2063 7632  pace.image = cv2
-00001760: 2e69 6d72 6561 6428 2269 6d61 6765 2e6a  .imread("image.j
-00001770: 7067 2229 0a69 6d61 6765 203d 2063 7632  pg").image = cv2
-00001780: 2e63 7674 436f 6c6f 7228 696d 6167 652c  .cvtColor(image,
-00001790: 2063 7632 2e43 4f4c 4f52 5f42 4752 3252   cv2.COLOR_BGR2R
-000017a0: 4742 290a 0a23 2041 7567 6d65 6e74 2061  GB)..# Augment a
-000017b0: 6e20 696d 6167 650a 7472 616e 7366 6f72  n image.transfor
-000017c0: 6d65 6420 3d20 7472 616e 7366 6f72 6d28  med = transform(
-000017d0: 696d 6167 653d 696d 6167 6529 0a74 7261  image=image).tra
-000017e0: 6e73 666f 726d 6564 5f69 6d61 6765 203d  nsformed_image =
-000017f0: 2074 7261 6e73 666f 726d 6564 5b22 696d   transformed["im
-00001800: 6167 6522 5d0a 6060 600a 0a23 2320 4765  age"].```..## Ge
-00001810: 7474 696e 6720 7374 6172 7465 640a 0a23  tting started..#
-00001820: 2323 2049 2061 6d20 6e65 7720 746f 2069  ## I am new to i
-00001830: 6d61 6765 2061 7567 6d65 6e74 6174 696f  mage augmentatio
-00001840: 6e0a 0a50 6c65 6173 6520 7374 6172 7420  n..Please start 
-00001850: 7769 7468 2074 6865 205b 696e 7472 6f64  with the [introd
-00001860: 7563 7469 6f6e 2061 7274 6963 6c65 735d  uction articles]
-00001870: 2868 7474 7073 3a2f 2f61 6c62 756d 656e  (https://albumen
-00001880: 7461 7469 6f6e 732e 6169 2f64 6f63 732f  tations.ai/docs/
-00001890: 2369 6e74 726f 6475 6374 696f 6e2d 746f  #introduction-to
-000018a0: 2d69 6d61 6765 2d61 7567 6d65 6e74 6174  -image-augmentat
-000018b0: 696f 6e29 2061 626f 7574 2077 6879 2069  ion) about why i
-000018c0: 6d61 6765 2061 7567 6d65 6e74 6174 696f  mage augmentatio
-000018d0: 6e20 6973 2069 6d70 6f72 7461 6e74 2061  n is important a
-000018e0: 6e64 2068 6f77 2069 7420 6865 6c70 7320  nd how it helps 
-000018f0: 746f 2062 7569 6c64 2062 6574 7465 7220  to build better 
-00001900: 6d6f 6465 6c73 2e0a 0a23 2323 2049 2077  models...### I w
-00001910: 616e 7420 746f 2075 7365 2041 6c62 756d  ant to use Album
-00001920: 656e 7461 7469 6f6e 7320 666f 7220 7468  entations for th
-00001930: 6520 7370 6563 6966 6963 2074 6173 6b20  e specific task 
-00001940: 7375 6368 2061 7320 636c 6173 7369 6669  such as classifi
-00001950: 6361 7469 6f6e 206f 7220 7365 676d 656e  cation or segmen
-00001960: 7461 7469 6f6e 0a0a 4966 2079 6f75 2077  tation..If you w
-00001970: 616e 7420 746f 2075 7365 2041 6c62 756d  ant to use Album
-00001980: 656e 7461 7469 6f6e 7320 666f 7220 6120  entations for a 
-00001990: 7370 6563 6966 6963 2074 6173 6b20 7375  specific task su
-000019a0: 6368 2061 7320 636c 6173 7369 6669 6361  ch as classifica
-000019b0: 7469 6f6e 2c20 7365 676d 656e 7461 7469  tion, segmentati
-000019c0: 6f6e 2c20 6f72 206f 626a 6563 7420 6465  on, or object de
-000019d0: 7465 6374 696f 6e2c 2072 6566 6572 2074  tection, refer t
-000019e0: 6f20 7468 6520 5b73 6574 206f 6620 6172  o the [set of ar
-000019f0: 7469 636c 6573 5d28 6874 7470 733a 2f2f  ticles](https://
-00001a00: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
-00001a10: 692f 646f 6373 2f23 6765 7474 696e 672d  i/docs/#getting-
-00001a20: 7374 6172 7465 642d 7769 7468 2d61 6c62  started-with-alb
-00001a30: 756d 656e 7461 7469 6f6e 7329 2074 6861  umentations) tha
-00001a40: 7420 6861 7320 616e 2069 6e2d 6465 7074  t has an in-dept
-00001a50: 6820 6465 7363 7269 7074 696f 6e20 6f66  h description of
-00001a60: 2074 6869 7320 7461 736b 2e20 5765 2061   this task. We a
-00001a70: 6c73 6f20 6861 7665 2061 205b 6c69 7374  lso have a [list
-00001a80: 206f 6620 6578 616d 706c 6573 5d28 6874   of examples](ht
-00001a90: 7470 733a 2f2f 616c 6275 6d65 6e74 6174  tps://albumentat
-00001aa0: 696f 6e73 2e61 692f 646f 6373 2f65 7861  ions.ai/docs/exa
-00001ab0: 6d70 6c65 732f 2920 6f6e 2061 7070 6c79  mples/) on apply
-00001ac0: 696e 6720 416c 6275 6d65 6e74 6174 696f  ing Albumentatio
-00001ad0: 6e73 2066 6f72 2064 6966 6665 7265 6e74  ns for different
-00001ae0: 2075 7365 2063 6173 6573 2e0a 0a23 2323   use cases...###
-00001af0: 2049 2077 616e 7420 746f 206b 6e6f 7720   I want to know 
-00001b00: 686f 7720 746f 2075 7365 2041 6c62 756d  how to use Album
-00001b10: 656e 7461 7469 6f6e 7320 7769 7468 2064  entations with d
-00001b20: 6565 7020 6c65 6172 6e69 6e67 2066 7261  eep learning fra
-00001b30: 6d65 776f 726b 730a 0a57 6520 6861 7665  meworks..We have
-00001b40: 205b 6578 616d 706c 6573 206f 6620 7573   [examples of us
-00001b50: 696e 6720 416c 6275 6d65 6e74 6174 696f  ing Albumentatio
-00001b60: 6e73 5d28 6874 7470 733a 2f2f 616c 6275  ns](https://albu
-00001b70: 6d65 6e74 6174 696f 6e73 2e61 692f 646f  mentations.ai/do
-00001b80: 6373 2f23 6578 616d 706c 6573 2d6f 662d  cs/#examples-of-
-00001b90: 686f 772d 746f 2d75 7365 2d61 6c62 756d  how-to-use-album
-00001ba0: 656e 7461 7469 6f6e 732d 7769 7468 2d64  entations-with-d
-00001bb0: 6966 6665 7265 6e74 2d64 6565 702d 6c65  ifferent-deep-le
-00001bc0: 6172 6e69 6e67 2d66 7261 6d65 776f 726b  arning-framework
-00001bd0: 7329 2061 6c6f 6e67 2077 6974 6820 5079  s) along with Py
-00001be0: 546f 7263 6820 616e 6420 5465 6e73 6f72  Torch and Tensor
-00001bf0: 466c 6f77 2e0a 0a23 2323 2049 2077 616e  Flow...### I wan
-00001c00: 7420 746f 2065 7870 6c6f 7265 2061 7567  t to explore aug
-00001c10: 6d65 6e74 6174 696f 6e73 2061 6e64 2073  mentations and s
-00001c20: 6565 2041 6c62 756d 656e 7461 7469 6f6e  ee Albumentation
-00001c30: 7320 696e 2061 6374 696f 6e0a 0a43 6865  s in action..Che
-00001c40: 636b 2074 6865 205b 6f6e 6c69 6e65 2064  ck the [online d
-00001c50: 656d 6f20 6f66 2074 6865 206c 6962 7261  emo of the libra
-00001c60: 7279 5d28 6874 7470 733a 2f2f 616c 6275  ry](https://albu
-00001c70: 6d65 6e74 6174 696f 6e73 2d64 656d 6f2e  mentations-demo.
-00001c80: 6865 726f 6b75 6170 702e 636f 6d2f 292e  herokuapp.com/).
-00001c90: 2057 6974 6820 6974 2c20 796f 7520 6361   With it, you ca
-00001ca0: 6e20 6170 706c 7920 6175 676d 656e 7461  n apply augmenta
-00001cb0: 7469 6f6e 7320 746f 2064 6966 6665 7265  tions to differe
-00001cc0: 6e74 2069 6d61 6765 7320 616e 6420 7365  nt images and se
-00001cd0: 6520 7468 6520 7265 7375 6c74 2e20 416c  e the result. Al
-00001ce0: 736f 2c20 7765 2068 6176 6520 6120 5b6c  so, we have a [l
-00001cf0: 6973 7420 6f66 2061 6c6c 2061 7661 696c  ist of all avail
-00001d00: 6162 6c65 2061 7567 6d65 6e74 6174 696f  able augmentatio
-00001d10: 6e73 2061 6e64 2074 6865 6972 2074 6172  ns and their tar
-00001d20: 6765 7473 5d28 236c 6973 742d 6f66 2d61  gets](#list-of-a
-00001d30: 7567 6d65 6e74 6174 696f 6e73 292e 0a0a  ugmentations)...
-00001d40: 2323 2057 686f 2069 7320 7573 696e 6720  ## Who is using 
-00001d50: 416c 6275 6d65 6e74 6174 696f 6e73 0a0a  Albumentations..
-00001d60: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00001d70: 2f77 7777 2e61 7070 6c65 2e63 6f6d 2f22  /www.apple.com/"
-00001d80: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
-00001d90: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
-00001da0: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
-00001db0: 7263 6f6e 7465 6e74 2e63 6f6d 2f61 6c62  rcontent.com/alb
-00001dc0: 756d 656e 7461 7469 6f6e 732d 7465 616d  umentations-team
-00001dd0: 2f61 6c62 756d 656e 7461 7469 6f6e 732e  /albumentations.
-00001de0: 6169 2f6d 6169 6e2f 6874 6d6c 2f61 7373  ai/main/html/ass
-00001df0: 6574 732f 696d 672f 696e 6475 7374 7279  ets/img/industry
-00001e00: 2f61 7070 6c65 2e6a 7065 6722 2077 6964  /apple.jpeg" wid
-00001e10: 7468 3d22 3130 3022 2f3e 3c2f 613e 0a3c  th="100"/></a>.<
-00001e20: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00001e30: 7265 7365 6172 6368 2e67 6f6f 676c 652f  research.google/
-00001e40: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
-00001e50: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
-00001e60: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
-00001e70: 6572 636f 6e74 656e 742e 636f 6d2f 616c  ercontent.com/al
-00001e80: 6275 6d65 6e74 6174 696f 6e73 2d74 6561  bumentations-tea
-00001e90: 6d2f 616c 6275 6d65 6e74 6174 696f 6e73  m/albumentations
-00001ea0: 2e61 692f 6d61 696e 2f68 746d 6c2f 6173  .ai/main/html/as
-00001eb0: 7365 7473 2f69 6d67 2f69 6e64 7573 7472  sets/img/industr
-00001ec0: 792f 676f 6f67 6c65 2e70 6e67 2220 7769  y/google.png" wi
-00001ed0: 6474 683d 2231 3030 222f 3e3c 2f61 3e0a  dth="100"/></a>.
-00001ee0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00001ef0: 2f6f 7065 6e73 6f75 7263 652e 6662 2e63  /opensource.fb.c
-00001f00: 6f6d 2f22 2074 6172 6765 743d 225f 626c  om/" target="_bl
-00001f10: 616e 6b22 3e3c 696d 6720 7372 633d 2268  ank"><img src="h
-00001f20: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
-00001f30: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
-00001f40: 2f61 6c62 756d 656e 7461 7469 6f6e 732d  /albumentations-
-00001f50: 7465 616d 2f61 6c62 756d 656e 7461 7469  team/albumentati
-00001f60: 6f6e 732e 6169 2f6d 6169 6e2f 6874 6d6c  ons.ai/main/html
-00001f70: 2f61 7373 6574 732f 696d 672f 696e 6475  /assets/img/indu
-00001f80: 7374 7279 2f6d 6574 615f 7265 7365 6172  stry/meta_resear
-00001f90: 6368 2e70 6e67 2220 7769 6474 683d 2231  ch.png" width="1
-00001fa0: 3030 222f 3e3c 2f61 3e0a 3c61 2068 7265  00"/></a>.<a hre
-00001fb0: 663d 2268 7474 7073 3a20 2f2f 7777 772e  f="https: //www.
-00001fc0: 6e76 6964 6961 2e63 6f6d 2f65 6e2d 7573  nvidia.com/en-us
-00001fd0: 2f72 6573 6561 7263 682f 2220 7461 7267  /research/" targ
-00001fe0: 6574 3d22 5f62 6c61 6e6b 223e 3c69 6d67  et="_blank"><img
-00001ff0: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
-00002000: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
-00002010: 656e 742e 636f 6d2f 616c 6275 6d65 6e74  ent.com/albument
-00002020: 6174 696f 6e73 2d74 6561 6d2f 616c 6275  ations-team/albu
-00002030: 6d65 6e74 6174 696f 6e73 2e61 692f 6d61  mentations.ai/ma
-00002040: 696e 2f68 746d 6c2f 6173 7365 7473 2f69  in/html/assets/i
-00002050: 6d67 2f69 6e64 7573 7472 792f 6e76 6964  mg/industry/nvid
-00002060: 6961 5f72 6573 6561 7263 682e 6a70 6567  ia_research.jpeg
-00002070: 2220 7769 6474 683d 2231 3030 222f 3e3c  " width="100"/><
-00002080: 2f61 3e0a 3c61 2068 7265 663d 2268 7474  /a>.<a href="htt
-00002090: 7073 3a2f 2f77 7777 2e61 6d61 7a6f 6e2e  ps://www.amazon.
-000020a0: 7363 6965 6e63 652f 2220 7461 7267 6574  science/" target
-000020b0: 3d22 5f62 6c61 6e6b 223e 3c69 6d67 2073  ="_blank"><img s
-000020c0: 7263 3d22 6874 7470 733a 2f2f 7261 772e  rc="https://raw.
-000020d0: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
-000020e0: 742e 636f 6d2f 616c 6275 6d65 6e74 6174  t.com/albumentat
-000020f0: 696f 6e73 2d74 6561 6d2f 616c 6275 6d65  ions-team/albume
-00002100: 6e74 6174 696f 6e73 2e61 692f 6d61 696e  ntations.ai/main
-00002110: 2f68 746d 6c2f 6173 7365 7473 2f69 6d67  /html/assets/img
-00002120: 2f69 6e64 7573 7472 792f 616d 617a 6f6e  /industry/amazon
-00002130: 5f73 6369 656e 6365 2e70 6e67 2220 7769  _science.png" wi
-00002140: 6474 683d 2231 3030 222f 3e3c 2f61 3e0a  dth="100"/></a>.
-00002150: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00002160: 2f6f 7065 6e73 6f75 7263 652e 6d69 6372  /opensource.micr
-00002170: 6f73 6f66 742e 636f 6d2f 2220 7461 7267  osoft.com/" targ
-00002180: 6574 3d22 5f62 6c61 6e6b 223e 3c69 6d67  et="_blank"><img
-00002190: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
-000021a0: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
-000021b0: 656e 742e 636f 6d2f 616c 6275 6d65 6e74  ent.com/albument
-000021c0: 6174 696f 6e73 2d74 6561 6d2f 616c 6275  ations-team/albu
-000021d0: 6d65 6e74 6174 696f 6e73 2e61 692f 6d61  mentations.ai/ma
-000021e0: 696e 2f68 746d 6c2f 6173 7365 7473 2f69  in/html/assets/i
-000021f0: 6d67 2f69 6e64 7573 7472 792f 6d69 6372  mg/industry/micr
-00002200: 6f73 6f66 742e 706e 6722 2077 6964 7468  osoft.png" width
-00002210: 3d22 3130 3022 2f3e 3c2f 613e 0a3c 6120  ="100"/></a>.<a 
-00002220: 6872 6566 3d22 6874 7470 733a 2f2f 656e  href="https://en
-00002230: 6769 6e65 6572 696e 672e 7361 6c65 7366  gineering.salesf
-00002240: 6f72 6365 2e63 6f6d 2f6f 7065 6e2d 736f  orce.com/open-so
-00002250: 7572 6365 2f22 2074 6172 6765 743d 225f  urce/" target="_
-00002260: 626c 616e 6b22 3e3c 696d 6720 7372 633d  blank"><img src=
-00002270: 2268 7474 7073 3a2f 2f72 6177 2e67 6974  "https://raw.git
-00002280: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
-00002290: 6f6d 2f61 6c62 756d 656e 7461 7469 6f6e  om/albumentation
-000022a0: 732d 7465 616d 2f61 6c62 756d 656e 7461  s-team/albumenta
-000022b0: 7469 6f6e 732e 6169 2f6d 6169 6e2f 6874  tions.ai/main/ht
-000022c0: 6d6c 2f61 7373 6574 732f 696d 672f 696e  ml/assets/img/in
-000022d0: 6475 7374 7279 2f73 616c 6573 666f 7263  dustry/salesforc
-000022e0: 655f 6f70 656e 5f73 6f75 7263 652e 706e  e_open_source.pn
-000022f0: 6722 2077 6964 7468 3d22 3130 3022 2f3e  g" width="100"/>
-00002300: 3c2f 613e 0a3c 6120 6872 6566 3d22 6874  </a>.<a href="ht
-00002310: 7470 733a 2f2f 7374 6162 696c 6974 792e  tps://stability.
-00002320: 6169 2f22 2074 6172 6765 743d 225f 626c  ai/" target="_bl
-00002330: 616e 6b22 3e3c 696d 6720 7372 633d 2268  ank"><img src="h
-00002340: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
-00002350: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
-00002360: 2f61 6c62 756d 656e 7461 7469 6f6e 732d  /albumentations-
-00002370: 7465 616d 2f61 6c62 756d 656e 7461 7469  team/albumentati
-00002380: 6f6e 732e 6169 2f6d 6169 6e2f 6874 6d6c  ons.ai/main/html
-00002390: 2f61 7373 6574 732f 696d 672f 696e 6475  /assets/img/indu
-000023a0: 7374 7279 2f73 7461 6269 6c69 7479 2e70  stry/stability.p
-000023b0: 6e67 2220 7769 6474 683d 2231 3030 222f  ng" width="100"/
-000023c0: 3e3c 2f61 3e0a 3c61 2068 7265 663d 2268  ></a>.<a href="h
-000023d0: 7474 7073 3a2f 2f77 7777 2e69 626d 2e63  ttps://www.ibm.c
-000023e0: 6f6d 2f6f 7065 6e73 6f75 7263 652f 2220  om/opensource/" 
-000023f0: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
-00002400: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00002410: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
-00002420: 636f 6e74 656e 742e 636f 6d2f 616c 6275  content.com/albu
-00002430: 6d65 6e74 6174 696f 6e73 2d74 6561 6d2f  mentations-team/
-00002440: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
-00002450: 692f 6d61 696e 2f68 746d 6c2f 6173 7365  i/main/html/asse
-00002460: 7473 2f69 6d67 2f69 6e64 7573 7472 792f  ts/img/industry/
-00002470: 6962 6d2e 6a70 6567 2220 7769 6474 683d  ibm.jpeg" width=
-00002480: 2231 3030 222f 3e3c 2f61 3e0a 3c61 2068  "100"/></a>.<a h
-00002490: 7265 663d 2268 7474 7073 3a2f 2f68 7567  ref="https://hug
-000024a0: 6769 6e67 6661 6365 2e63 6f2f 2220 7461  gingface.co/" ta
-000024b0: 7267 6574 3d22 5f62 6c61 6e6b 223e 3c69  rget="_blank"><i
-000024c0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-000024d0: 7261 772e 6769 7468 7562 7573 6572 636f  raw.githubuserco
-000024e0: 6e74 656e 742e 636f 6d2f 616c 6275 6d65  ntent.com/albume
-000024f0: 6e74 6174 696f 6e73 2d74 6561 6d2f 616c  ntations-team/al
-00002500: 6275 6d65 6e74 6174 696f 6e73 2e61 692f  bumentations.ai/
-00002510: 6d61 696e 2f68 746d 6c2f 6173 7365 7473  main/html/assets
-00002520: 2f69 6d67 2f69 6e64 7573 7472 792f 6875  /img/industry/hu
-00002530: 6767 696e 675f 6661 6365 2e70 6e67 2220  gging_face.png" 
-00002540: 7769 6474 683d 2231 3030 222f 3e3c 2f61  width="100"/></a
-00002550: 3e0a 3c61 2068 7265 663d 2268 7474 7073  >.<a href="https
-00002560: 3a2f 2f77 7777 2e73 6f6e 792e 636f 6d2f  ://www.sony.com/
-00002570: 656e 2f22 2074 6172 6765 743d 225f 626c  en/" target="_bl
-00002580: 616e 6b22 3e3c 696d 6720 7372 633d 2268  ank"><img src="h
-00002590: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
-000025a0: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
-000025b0: 2f61 6c62 756d 656e 7461 7469 6f6e 732d  /albumentations-
-000025c0: 7465 616d 2f61 6c62 756d 656e 7461 7469  team/albumentati
-000025d0: 6f6e 732e 6169 2f6d 6169 6e2f 6874 6d6c  ons.ai/main/html
-000025e0: 2f61 7373 6574 732f 696d 672f 696e 6475  /assets/img/indu
-000025f0: 7374 7279 2f73 6f6e 792e 706e 6722 2077  stry/sony.png" w
-00002600: 6964 7468 3d22 3130 3022 2f3e 3c2f 613e  idth="100"/></a>
-00002610: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
-00002620: 2f2f 6f70 656e 736f 7572 6365 2e61 6c69  //opensource.ali
-00002630: 6261 6261 2e63 6f6d 2f22 2074 6172 6765  baba.com/" targe
-00002640: 743d 225f 626c 616e 6b22 3e3c 696d 6720  t="_blank"><img 
-00002650: 7372 633d 2268 7474 7073 3a2f 2f72 6177  src="https://raw
-00002660: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
-00002670: 6e74 2e63 6f6d 2f61 6c62 756d 656e 7461  nt.com/albumenta
-00002680: 7469 6f6e 732d 7465 616d 2f61 6c62 756d  tions-team/album
-00002690: 656e 7461 7469 6f6e 732e 6169 2f6d 6169  entations.ai/mai
-000026a0: 6e2f 6874 6d6c 2f61 7373 6574 732f 696d  n/html/assets/im
-000026b0: 672f 696e 6475 7374 7279 2f61 6c69 6261  g/industry/aliba
-000026c0: 6261 2e70 6e67 2220 7769 6474 683d 2231  ba.png" width="1
-000026d0: 3030 222f 3e3c 2f61 3e0a 3c61 2068 7265  00"/></a>.<a hre
-000026e0: 663d 2268 7474 7073 3a2f 2f6f 7065 6e73  f="https://opens
-000026f0: 6f75 7263 652e 7465 6e63 656e 742e 636f  ource.tencent.co
-00002700: 6d2f 2220 7461 7267 6574 3d22 5f62 6c61  m/" target="_bla
-00002710: 6e6b 223e 3c69 6d67 2073 7263 3d22 6874  nk"><img src="ht
-00002720: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
-00002730: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
-00002740: 616c 6275 6d65 6e74 6174 696f 6e73 2d74  albumentations-t
-00002750: 6561 6d2f 616c 6275 6d65 6e74 6174 696f  eam/albumentatio
-00002760: 6e73 2e61 692f 6d61 696e 2f68 746d 6c2f  ns.ai/main/html/
-00002770: 6173 7365 7473 2f69 6d67 2f69 6e64 7573  assets/img/indus
-00002780: 7472 792f 7465 6e63 656e 742e 706e 6722  try/tencent.png"
-00002790: 2077 6964 7468 3d22 3130 3022 2f3e 3c2f   width="100"/></
-000027a0: 613e 0a3c 6120 6872 6566 3d22 6874 7470  a>.<a href="http
-000027b0: 733a 2f2f 6832 6f2e 6169 2f22 2074 6172  s://h2o.ai/" tar
-000027c0: 6765 743d 225f 626c 616e 6b22 3e3c 696d  get="_blank"><im
-000027d0: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
-000027e0: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-000027f0: 7465 6e74 2e63 6f6d 2f61 6c62 756d 656e  tent.com/albumen
-00002800: 7461 7469 6f6e 732d 7465 616d 2f61 6c62  tations-team/alb
-00002810: 756d 656e 7461 7469 6f6e 732e 6169 2f6d  umentations.ai/m
-00002820: 6169 6e2f 6874 6d6c 2f61 7373 6574 732f  ain/html/assets/
-00002830: 696d 672f 696e 6475 7374 7279 2f68 326f  img/industry/h2o
-00002840: 5f61 692e 706e 6722 2077 6964 7468 3d22  _ai.png" width="
-00002850: 3130 3022 2f3e 3c2f 613e 0a0a 2323 2320  100"/></a>..### 
-00002860: 5365 6520 616c 736f 0a0a 2d20 5b41 206c  See also..- [A l
-00002870: 6973 7420 6f66 2070 6170 6572 7320 7468  ist of papers th
-00002880: 6174 2063 6974 6520 416c 6275 6d65 6e74  at cite Albument
-00002890: 6174 696f 6e73 5d28 6874 7470 733a 2f2f  ations](https://
-000028a0: 7363 686f 6c61 722e 676f 6f67 6c65 2e63  scholar.google.c
-000028b0: 6f6d 2f63 6974 6174 696f 6e73 3f76 6965  om/citations?vie
-000028c0: 775f 6f70 3d76 6965 775f 6369 7461 7469  w_op=view_citati
-000028d0: 6f6e 2663 6974 6174 696f 6e5f 666f 725f  on&citation_for_
-000028e0: 7669 6577 3d76 6b6a 6839 5830 4141 4141  view=vkjh9X0AAAA
-000028f0: 4a3a 7230 4270 6e74 5a71 4a47 3443 292e  J:r0BpntZqJG4C).
-00002900: 0a2d 205b 4120 6c69 7374 206f 6620 7465  .- [A list of te
-00002910: 616d 7320 7468 6174 2077 6572 6520 7573  ams that were us
-00002920: 696e 6720 416c 6275 6d65 6e74 6174 696f  ing Albumentatio
-00002930: 6e73 2061 6e64 2074 6f6f 6b20 6869 6768  ns and took high
-00002940: 2070 6c61 6365 7320 696e 206d 6163 6869   places in machi
-00002950: 6e65 206c 6561 726e 696e 6720 636f 6d70  ne learning comp
-00002960: 6574 6974 696f 6e73 5d28 6874 7470 733a  etitions](https:
-00002970: 2f2f 616c 6275 6d65 6e74 6174 696f 6e73  //albumentations
-00002980: 2e61 692f 7768 6f73 5f75 7369 6e67 2363  .ai/whos_using#c
-00002990: 6f6d 7065 7469 7469 6f6e 7329 2e0a 2d20  ompetitions)..- 
-000029a0: 5b4f 7065 6e20 736f 7572 6365 2070 726f  [Open source pro
-000029b0: 6a65 6374 7320 7468 6174 2075 7365 2041  jects that use A
-000029c0: 6c62 756d 656e 7461 7469 6f6e 735d 2868  lbumentations](h
-000029d0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000029e0: 6d2f 616c 6275 6d65 6e74 6174 696f 6e73  m/albumentations
-000029f0: 2d74 6561 6d2f 616c 6275 6d65 6e74 6174  -team/albumentat
-00002a00: 696f 6e73 2f6e 6574 776f 726b 2f64 6570  ions/network/dep
-00002a10: 656e 6465 6e74 733f 6465 7065 6e64 656e  endents?dependen
-00002a20: 745f 7479 7065 3d50 4143 4b41 4745 292e  t_type=PACKAGE).
-00002a30: 0a0a 2323 204c 6973 7420 6f66 2061 7567  ..## List of aug
-00002a40: 6d65 6e74 6174 696f 6e73 0a0a 2323 2320  mentations..### 
-00002a50: 5069 7865 6c2d 6c65 7665 6c20 7472 616e  Pixel-level tran
-00002a60: 7366 6f72 6d73 0a0a 5069 7865 6c2d 6c65  sforms..Pixel-le
-00002a70: 7665 6c20 7472 616e 7366 6f72 6d73 2077  vel transforms w
-00002a80: 696c 6c20 6368 616e 6765 206a 7573 7420  ill change just 
-00002a90: 616e 2069 6e70 7574 2069 6d61 6765 2061  an input image a
-00002aa0: 6e64 2077 696c 6c20 6c65 6176 6520 616e  nd will leave an
-00002ab0: 7920 6164 6469 7469 6f6e 616c 2074 6172  y additional tar
-00002ac0: 6765 7473 2073 7563 6820 6173 206d 6173  gets such as mas
-00002ad0: 6b73 2c20 626f 756e 6469 6e67 2062 6f78  ks, bounding box
-00002ae0: 6573 2c20 616e 6420 6b65 7970 6f69 6e74  es, and keypoint
-00002af0: 7320 756e 6368 616e 6765 642e 2054 6865  s unchanged. The
-00002b00: 206c 6973 7420 6f66 2070 6978 656c 2d6c   list of pixel-l
-00002b10: 6576 656c 2074 7261 6e73 666f 726d 733a  evel transforms:
-00002b20: 0a0a 2d20 5b41 6476 616e 6365 6442 6c75  ..- [AdvancedBlu
-00002b30: 725d 2868 7474 7073 3a2f 2f61 6c62 756d  r](https://album
-00002b40: 656e 7461 7469 6f6e 732e 6169 2f64 6f63  entations.ai/doc
-00002b50: 732f 6170 695f 7265 6665 7265 6e63 652f  s/api_reference/
-00002b60: 6175 676d 656e 7461 7469 6f6e 732f 626c  augmentations/bl
-00002b70: 7572 2f74 7261 6e73 666f 726d 732f 2361  ur/transforms/#a
-00002b80: 6c62 756d 656e 7461 7469 6f6e 732e 6175  lbumentations.au
-00002b90: 676d 656e 7461 7469 6f6e 732e 626c 7572  gmentations.blur
-00002ba0: 2e74 7261 6e73 666f 726d 732e 4164 7661  .transforms.Adva
-00002bb0: 6e63 6564 426c 7572 290a 2d20 5b42 6c75  ncedBlur).- [Blu
-00002bc0: 725d 2868 7474 7073 3a2f 2f61 6c62 756d  r](https://album
-00002bd0: 656e 7461 7469 6f6e 732e 6169 2f64 6f63  entations.ai/doc
-00002be0: 732f 6170 695f 7265 6665 7265 6e63 652f  s/api_reference/
-00002bf0: 6175 676d 656e 7461 7469 6f6e 732f 626c  augmentations/bl
-00002c00: 7572 2f74 7261 6e73 666f 726d 732f 2361  ur/transforms/#a
-00002c10: 6c62 756d 656e 7461 7469 6f6e 732e 6175  lbumentations.au
-00002c20: 676d 656e 7461 7469 6f6e 732e 626c 7572  gmentations.blur
-00002c30: 2e74 7261 6e73 666f 726d 732e 426c 7572  .transforms.Blur
-00002c40: 290a 2d20 5b43 4c41 4845 5d28 6874 7470  ).- [CLAHE](http
-00002c50: 733a 2f2f 616c 6275 6d65 6e74 6174 696f  s://albumentatio
-00002c60: 6e73 2e61 692f 646f 6373 2f61 7069 5f72  ns.ai/docs/api_r
-00002c70: 6566 6572 656e 6365 2f61 7567 6d65 6e74  eference/augment
-00002c80: 6174 696f 6e73 2f74 7261 6e73 666f 726d  ations/transform
-00002c90: 732f 2361 6c62 756d 656e 7461 7469 6f6e  s/#albumentation
-00002ca0: 732e 6175 676d 656e 7461 7469 6f6e 732e  s.augmentations.
-00002cb0: 7472 616e 7366 6f72 6d73 2e43 4c41 4845  transforms.CLAHE
-00002cc0: 290a 2d20 5b43 6861 6e6e 656c 4472 6f70  ).- [ChannelDrop
-00002cd0: 6f75 745d 2868 7474 7073 3a2f 2f61 6c62  out](https://alb
-00002ce0: 756d 656e 7461 7469 6f6e 732e 6169 2f64  umentations.ai/d
-00002cf0: 6f63 732f 6170 695f 7265 6665 7265 6e63  ocs/api_referenc
-00002d00: 652f 6175 676d 656e 7461 7469 6f6e 732f  e/augmentations/
-00002d10: 6472 6f70 6f75 742f 6368 616e 6e65 6c5f  dropout/channel_
-00002d20: 6472 6f70 6f75 742f 2361 6c62 756d 656e  dropout/#albumen
-00002d30: 7461 7469 6f6e 732e 6175 676d 656e 7461  tations.augmenta
-00002d40: 7469 6f6e 732e 6472 6f70 6f75 742e 6368  tions.dropout.ch
-00002d50: 616e 6e65 6c5f 6472 6f70 6f75 742e 4368  annel_dropout.Ch
-00002d60: 616e 6e65 6c44 726f 706f 7574 290a 2d20  annelDropout).- 
-00002d70: 5b43 6861 6e6e 656c 5368 7566 666c 655d  [ChannelShuffle]
-00002d80: 2868 7474 7073 3a2f 2f61 6c62 756d 656e  (https://albumen
-00002d90: 7461 7469 6f6e 732e 6169 2f64 6f63 732f  tations.ai/docs/
-00002da0: 6170 695f 7265 6665 7265 6e63 652f 6175  api_reference/au
-00002db0: 676d 656e 7461 7469 6f6e 732f 7472 616e  gmentations/tran
-00002dc0: 7366 6f72 6d73 2f23 616c 6275 6d65 6e74  sforms/#albument
-00002dd0: 6174 696f 6e73 2e61 7567 6d65 6e74 6174  ations.augmentat
-00002de0: 696f 6e73 2e74 7261 6e73 666f 726d 732e  ions.transforms.
-00002df0: 4368 616e 6e65 6c53 6875 6666 6c65 290a  ChannelShuffle).
-00002e00: 2d20 5b43 6872 6f6d 6174 6963 4162 6572  - [ChromaticAber
-00002e10: 7261 7469 6f6e 5d28 6874 7470 733a 2f2f  ration](https://
-00002e20: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
-00002e30: 692f 646f 6373 2f61 7069 5f72 6566 6572  i/docs/api_refer
-00002e40: 656e 6365 2f61 7567 6d65 6e74 6174 696f  ence/augmentatio
-00002e50: 6e73 2f74 7261 6e73 666f 726d 732f 2361  ns/transforms/#a
-00002e60: 6c62 756d 656e 7461 7469 6f6e 732e 6175  lbumentations.au
-00002e70: 676d 656e 7461 7469 6f6e 732e 7472 616e  gmentations.tran
-00002e80: 7366 6f72 6d73 2e43 6872 6f6d 6174 6963  sforms.Chromatic
-00002e90: 4162 6572 7261 7469 6f6e 290a 2d20 5b43  Aberration).- [C
-00002ea0: 6f6c 6f72 4a69 7474 6572 5d28 6874 7470  olorJitter](http
-00002eb0: 733a 2f2f 616c 6275 6d65 6e74 6174 696f  s://albumentatio
-00002ec0: 6e73 2e61 692f 646f 6373 2f61 7069 5f72  ns.ai/docs/api_r
-00002ed0: 6566 6572 656e 6365 2f61 7567 6d65 6e74  eference/augment
-00002ee0: 6174 696f 6e73 2f74 7261 6e73 666f 726d  ations/transform
-00002ef0: 732f 2361 6c62 756d 656e 7461 7469 6f6e  s/#albumentation
-00002f00: 732e 6175 676d 656e 7461 7469 6f6e 732e  s.augmentations.
-00002f10: 7472 616e 7366 6f72 6d73 2e43 6f6c 6f72  transforms.Color
-00002f20: 4a69 7474 6572 290a 2d20 5b44 6566 6f63  Jitter).- [Defoc
-00002f30: 7573 5d28 6874 7470 733a 2f2f 616c 6275  us](https://albu
-00002f40: 6d65 6e74 6174 696f 6e73 2e61 692f 646f  mentations.ai/do
-00002f50: 6373 2f61 7069 5f72 6566 6572 656e 6365  cs/api_reference
-00002f60: 2f61 7567 6d65 6e74 6174 696f 6e73 2f62  /augmentations/b
-00002f70: 6c75 722f 7472 616e 7366 6f72 6d73 2f23  lur/transforms/#
-00002f80: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
-00002f90: 7567 6d65 6e74 6174 696f 6e73 2e62 6c75  ugmentations.blu
-00002fa0: 722e 7472 616e 7366 6f72 6d73 2e44 6566  r.transforms.Def
-00002fb0: 6f63 7573 290a 2d20 5b44 6f77 6e73 6361  ocus).- [Downsca
-00002fc0: 6c65 5d28 6874 7470 733a 2f2f 616c 6275  le](https://albu
-00002fd0: 6d65 6e74 6174 696f 6e73 2e61 692f 646f  mentations.ai/do
-00002fe0: 6373 2f61 7069 5f72 6566 6572 656e 6365  cs/api_reference
-00002ff0: 2f61 7567 6d65 6e74 6174 696f 6e73 2f74  /augmentations/t
-00003000: 7261 6e73 666f 726d 732f 2361 6c62 756d  ransforms/#album
-00003010: 656e 7461 7469 6f6e 732e 6175 676d 656e  entations.augmen
-00003020: 7461 7469 6f6e 732e 7472 616e 7366 6f72  tations.transfor
-00003030: 6d73 2e44 6f77 6e73 6361 6c65 290a 2d20  ms.Downscale).- 
-00003040: 5b45 6d62 6f73 735d 2868 7474 7073 3a2f  [Emboss](https:/
-00003050: 2f61 6c62 756d 656e 7461 7469 6f6e 732e  /albumentations.
-00003060: 6169 2f64 6f63 732f 6170 695f 7265 6665  ai/docs/api_refe
-00003070: 7265 6e63 652f 6175 676d 656e 7461 7469  rence/augmentati
-00003080: 6f6e 732f 7472 616e 7366 6f72 6d73 2f23  ons/transforms/#
-00003090: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
-000030a0: 7567 6d65 6e74 6174 696f 6e73 2e74 7261  ugmentations.tra
-000030b0: 6e73 666f 726d 732e 456d 626f 7373 290a  nsforms.Emboss).
-000030c0: 2d20 5b45 7175 616c 697a 655d 2868 7474  - [Equalize](htt
-000030d0: 7073 3a2f 2f61 6c62 756d 656e 7461 7469  ps://albumentati
-000030e0: 6f6e 732e 6169 2f64 6f63 732f 6170 695f  ons.ai/docs/api_
-000030f0: 7265 6665 7265 6e63 652f 6175 676d 656e  reference/augmen
-00003100: 7461 7469 6f6e 732f 7472 616e 7366 6f72  tations/transfor
-00003110: 6d73 2f23 616c 6275 6d65 6e74 6174 696f  ms/#albumentatio
-00003120: 6e73 2e61 7567 6d65 6e74 6174 696f 6e73  ns.augmentations
-00003130: 2e74 7261 6e73 666f 726d 732e 4571 7561  .transforms.Equa
-00003140: 6c69 7a65 290a 2d20 5b46 4441 5d28 6874  lize).- [FDA](ht
-00003150: 7470 733a 2f2f 616c 6275 6d65 6e74 6174  tps://albumentat
-00003160: 696f 6e73 2e61 692f 646f 6373 2f61 7069  ions.ai/docs/api
-00003170: 5f72 6566 6572 656e 6365 2f61 7567 6d65  _reference/augme
-00003180: 6e74 6174 696f 6e73 2f64 6f6d 6169 6e5f  ntations/domain_
-00003190: 6164 6170 7461 7469 6f6e 2f23 616c 6275  adaptation/#albu
-000031a0: 6d65 6e74 6174 696f 6e73 2e61 7567 6d65  mentations.augme
-000031b0: 6e74 6174 696f 6e73 2e64 6f6d 6169 6e5f  ntations.domain_
-000031c0: 6164 6170 7461 7469 6f6e 2e46 4441 290a  adaptation.FDA).
-000031d0: 2d20 5b46 616e 6379 5043 415d 2868 7474  - [FancyPCA](htt
-000031e0: 7073 3a2f 2f61 6c62 756d 656e 7461 7469  ps://albumentati
-000031f0: 6f6e 732e 6169 2f64 6f63 732f 6170 695f  ons.ai/docs/api_
-00003200: 7265 6665 7265 6e63 652f 6175 676d 656e  reference/augmen
-00003210: 7461 7469 6f6e 732f 7472 616e 7366 6f72  tations/transfor
-00003220: 6d73 2f23 616c 6275 6d65 6e74 6174 696f  ms/#albumentatio
-00003230: 6e73 2e61 7567 6d65 6e74 6174 696f 6e73  ns.augmentations
-00003240: 2e74 7261 6e73 666f 726d 732e 4661 6e63  .transforms.Fanc
-00003250: 7950 4341 290a 2d20 5b46 726f 6d46 6c6f  yPCA).- [FromFlo
-00003260: 6174 5d28 6874 7470 733a 2f2f 616c 6275  at](https://albu
-00003270: 6d65 6e74 6174 696f 6e73 2e61 692f 646f  mentations.ai/do
-00003280: 6373 2f61 7069 5f72 6566 6572 656e 6365  cs/api_reference
-00003290: 2f61 7567 6d65 6e74 6174 696f 6e73 2f74  /augmentations/t
-000032a0: 7261 6e73 666f 726d 732f 2361 6c62 756d  ransforms/#album
-000032b0: 656e 7461 7469 6f6e 732e 6175 676d 656e  entations.augmen
-000032c0: 7461 7469 6f6e 732e 7472 616e 7366 6f72  tations.transfor
-000032d0: 6d73 2e46 726f 6d46 6c6f 6174 290a 2d20  ms.FromFloat).- 
-000032e0: 5b47 6175 7373 4e6f 6973 655d 2868 7474  [GaussNoise](htt
-000032f0: 7073 3a2f 2f61 6c62 756d 656e 7461 7469  ps://albumentati
-00003300: 6f6e 732e 6169 2f64 6f63 732f 6170 695f  ons.ai/docs/api_
-00003310: 7265 6665 7265 6e63 652f 6175 676d 656e  reference/augmen
-00003320: 7461 7469 6f6e 732f 7472 616e 7366 6f72  tations/transfor
-00003330: 6d73 2f23 616c 6275 6d65 6e74 6174 696f  ms/#albumentatio
-00003340: 6e73 2e61 7567 6d65 6e74 6174 696f 6e73  ns.augmentations
-00003350: 2e74 7261 6e73 666f 726d 732e 4761 7573  .transforms.Gaus
-00003360: 734e 6f69 7365 290a 2d20 5b47 6175 7373  sNoise).- [Gauss
-00003370: 6961 6e42 6c75 725d 2868 7474 7073 3a2f  ianBlur](https:/
-00003380: 2f61 6c62 756d 656e 7461 7469 6f6e 732e  /albumentations.
-00003390: 6169 2f64 6f63 732f 6170 695f 7265 6665  ai/docs/api_refe
-000033a0: 7265 6e63 652f 6175 676d 656e 7461 7469  rence/augmentati
-000033b0: 6f6e 732f 626c 7572 2f74 7261 6e73 666f  ons/blur/transfo
-000033c0: 726d 732f 2361 6c62 756d 656e 7461 7469  rms/#albumentati
-000033d0: 6f6e 732e 6175 676d 656e 7461 7469 6f6e  ons.augmentation
-000033e0: 732e 626c 7572 2e74 7261 6e73 666f 726d  s.blur.transform
-000033f0: 732e 4761 7573 7369 616e 426c 7572 290a  s.GaussianBlur).
-00003400: 2d20 5b47 6c61 7373 426c 7572 5d28 6874  - [GlassBlur](ht
-00003410: 7470 733a 2f2f 616c 6275 6d65 6e74 6174  tps://albumentat
-00003420: 696f 6e73 2e61 692f 646f 6373 2f61 7069  ions.ai/docs/api
-00003430: 5f72 6566 6572 656e 6365 2f61 7567 6d65  _reference/augme
-00003440: 6e74 6174 696f 6e73 2f62 6c75 722f 7472  ntations/blur/tr
-00003450: 616e 7366 6f72 6d73 2f23 616c 6275 6d65  ansforms/#albume
-00003460: 6e74 6174 696f 6e73 2e61 7567 6d65 6e74  ntations.augment
-00003470: 6174 696f 6e73 2e62 6c75 722e 7472 616e  ations.blur.tran
-00003480: 7366 6f72 6d73 2e47 6c61 7373 426c 7572  sforms.GlassBlur
-00003490: 290a 2d20 5b48 6973 746f 6772 616d 4d61  ).- [HistogramMa
-000034a0: 7463 6869 6e67 5d28 6874 7470 733a 2f2f  tching](https://
-000034b0: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
-000034c0: 692f 646f 6373 2f61 7069 5f72 6566 6572  i/docs/api_refer
-000034d0: 656e 6365 2f61 7567 6d65 6e74 6174 696f  ence/augmentatio
-000034e0: 6e73 2f64 6f6d 6169 6e5f 6164 6170 7461  ns/domain_adapta
-000034f0: 7469 6f6e 2f23 616c 6275 6d65 6e74 6174  tion/#albumentat
-00003500: 696f 6e73 2e61 7567 6d65 6e74 6174 696f  ions.augmentatio
-00003510: 6e73 2e64 6f6d 6169 6e5f 6164 6170 7461  ns.domain_adapta
-00003520: 7469 6f6e 2e48 6973 746f 6772 616d 4d61  tion.HistogramMa
-00003530: 7463 6869 6e67 290a 2d20 5b48 7565 5361  tching).- [HueSa
-00003540: 7475 7261 7469 6f6e 5661 6c75 655d 2868  turationValue](h
-00003550: 7474 7073 3a2f 2f61 6c62 756d 656e 7461  ttps://albumenta
-00003560: 7469 6f6e 732e 6169 2f64 6f63 732f 6170  tions.ai/docs/ap
-00003570: 695f 7265 6665 7265 6e63 652f 6175 676d  i_reference/augm
-00003580: 656e 7461 7469 6f6e 732f 7472 616e 7366  entations/transf
-00003590: 6f72 6d73 2f23 616c 6275 6d65 6e74 6174  orms/#albumentat
-000035a0: 696f 6e73 2e61 7567 6d65 6e74 6174 696f  ions.augmentatio
-000035b0: 6e73 2e74 7261 6e73 666f 726d 732e 4875  ns.transforms.Hu
-000035c0: 6553 6174 7572 6174 696f 6e56 616c 7565  eSaturationValue
-000035d0: 290a 2d20 5b49 534f 4e6f 6973 655d 2868  ).- [ISONoise](h
-000035e0: 7474 7073 3a2f 2f61 6c62 756d 656e 7461  ttps://albumenta
-000035f0: 7469 6f6e 732e 6169 2f64 6f63 732f 6170  tions.ai/docs/ap
-00003600: 695f 7265 6665 7265 6e63 652f 6175 676d  i_reference/augm
-00003610: 656e 7461 7469 6f6e 732f 7472 616e 7366  entations/transf
-00003620: 6f72 6d73 2f23 616c 6275 6d65 6e74 6174  orms/#albumentat
-00003630: 696f 6e73 2e61 7567 6d65 6e74 6174 696f  ions.augmentatio
-00003640: 6e73 2e74 7261 6e73 666f 726d 732e 4953  ns.transforms.IS
-00003650: 4f4e 6f69 7365 290a 2d20 5b49 6d61 6765  ONoise).- [Image
-00003660: 436f 6d70 7265 7373 696f 6e5d 2868 7474  Compression](htt
-00003670: 7073 3a2f 2f61 6c62 756d 656e 7461 7469  ps://albumentati
-00003680: 6f6e 732e 6169 2f64 6f63 732f 6170 695f  ons.ai/docs/api_
-00003690: 7265 6665 7265 6e63 652f 6175 676d 656e  reference/augmen
-000036a0: 7461 7469 6f6e 732f 7472 616e 7366 6f72  tations/transfor
-000036b0: 6d73 2f23 616c 6275 6d65 6e74 6174 696f  ms/#albumentatio
-000036c0: 6e73 2e61 7567 6d65 6e74 6174 696f 6e73  ns.augmentations
-000036d0: 2e74 7261 6e73 666f 726d 732e 496d 6167  .transforms.Imag
-000036e0: 6543 6f6d 7072 6573 7369 6f6e 290a 2d20  eCompression).- 
-000036f0: 5b49 6e76 6572 7449 6d67 5d28 6874 7470  [InvertImg](http
-00003700: 733a 2f2f 616c 6275 6d65 6e74 6174 696f  s://albumentatio
-00003710: 6e73 2e61 692f 646f 6373 2f61 7069 5f72  ns.ai/docs/api_r
-00003720: 6566 6572 656e 6365 2f61 7567 6d65 6e74  eference/augment
-00003730: 6174 696f 6e73 2f74 7261 6e73 666f 726d  ations/transform
-00003740: 732f 2361 6c62 756d 656e 7461 7469 6f6e  s/#albumentation
-00003750: 732e 6175 676d 656e 7461 7469 6f6e 732e  s.augmentations.
-00003760: 7472 616e 7366 6f72 6d73 2e49 6e76 6572  transforms.Inver
-00003770: 7449 6d67 290a 2d20 5b4d 6564 6961 6e42  tImg).- [MedianB
-00003780: 6c75 725d 2868 7474 7073 3a2f 2f61 6c62  lur](https://alb
-00003790: 756d 656e 7461 7469 6f6e 732e 6169 2f64  umentations.ai/d
-000037a0: 6f63 732f 6170 695f 7265 6665 7265 6e63  ocs/api_referenc
-000037b0: 652f 6175 676d 656e 7461 7469 6f6e 732f  e/augmentations/
-000037c0: 626c 7572 2f74 7261 6e73 666f 726d 732f  blur/transforms/
-000037d0: 2361 6c62 756d 656e 7461 7469 6f6e 732e  #albumentations.
-000037e0: 6175 676d 656e 7461 7469 6f6e 732e 626c  augmentations.bl
-000037f0: 7572 2e74 7261 6e73 666f 726d 732e 4d65  ur.transforms.Me
-00003800: 6469 616e 426c 7572 290a 2d20 5b4d 6f74  dianBlur).- [Mot
-00003810: 696f 6e42 6c75 725d 2868 7474 7073 3a2f  ionBlur](https:/
-00003820: 2f61 6c62 756d 656e 7461 7469 6f6e 732e  /albumentations.
-00003830: 6169 2f64 6f63 732f 6170 695f 7265 6665  ai/docs/api_refe
-00003840: 7265 6e63 652f 6175 676d 656e 7461 7469  rence/augmentati
-00003850: 6f6e 732f 626c 7572 2f74 7261 6e73 666f  ons/blur/transfo
-00003860: 726d 732f 2361 6c62 756d 656e 7461 7469  rms/#albumentati
-00003870: 6f6e 732e 6175 676d 656e 7461 7469 6f6e  ons.augmentation
-00003880: 732e 626c 7572 2e74 7261 6e73 666f 726d  s.blur.transform
-00003890: 732e 4d6f 7469 6f6e 426c 7572 290a 2d20  s.MotionBlur).- 
-000038a0: 5b4d 756c 7469 706c 6963 6174 6976 654e  [MultiplicativeN
-000038b0: 6f69 7365 5d28 6874 7470 733a 2f2f 616c  oise](https://al
-000038c0: 6275 6d65 6e74 6174 696f 6e73 2e61 692f  bumentations.ai/
-000038d0: 646f 6373 2f61 7069 5f72 6566 6572 656e  docs/api_referen
-000038e0: 6365 2f61 7567 6d65 6e74 6174 696f 6e73  ce/augmentations
-000038f0: 2f74 7261 6e73 666f 726d 732f 2361 6c62  /transforms/#alb
-00003900: 756d 656e 7461 7469 6f6e 732e 6175 676d  umentations.augm
-00003910: 656e 7461 7469 6f6e 732e 7472 616e 7366  entations.transf
-00003920: 6f72 6d73 2e4d 756c 7469 706c 6963 6174  orms.Multiplicat
-00003930: 6976 654e 6f69 7365 290a 2d20 5b4e 6f72  iveNoise).- [Nor
-00003940: 6d61 6c69 7a65 5d28 6874 7470 733a 2f2f  malize](https://
-00003950: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
-00003960: 692f 646f 6373 2f61 7069 5f72 6566 6572  i/docs/api_refer
-00003970: 656e 6365 2f61 7567 6d65 6e74 6174 696f  ence/augmentatio
-00003980: 6e73 2f74 7261 6e73 666f 726d 732f 2361  ns/transforms/#a
-00003990: 6c62 756d 656e 7461 7469 6f6e 732e 6175  lbumentations.au
-000039a0: 676d 656e 7461 7469 6f6e 732e 7472 616e  gmentations.tran
-000039b0: 7366 6f72 6d73 2e4e 6f72 6d61 6c69 7a65  sforms.Normalize
-000039c0: 290a 2d20 5b50 6978 656c 4469 7374 7269  ).- [PixelDistri
-000039d0: 6275 7469 6f6e 4164 6170 7461 7469 6f6e  butionAdaptation
-000039e0: 5d28 6874 7470 733a 2f2f 616c 6275 6d65  ](https://albume
-000039f0: 6e74 6174 696f 6e73 2e61 692f 646f 6373  ntations.ai/docs
-00003a00: 2f61 7069 5f72 6566 6572 656e 6365 2f61  /api_reference/a
-00003a10: 7567 6d65 6e74 6174 696f 6e73 2f64 6f6d  ugmentations/dom
-00003a20: 6169 6e5f 6164 6170 7461 7469 6f6e 2f23  ain_adaptation/#
-00003a30: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
-00003a40: 7567 6d65 6e74 6174 696f 6e73 2e64 6f6d  ugmentations.dom
-00003a50: 6169 6e5f 6164 6170 7461 7469 6f6e 2e50  ain_adaptation.P
-00003a60: 6978 656c 4469 7374 7269 6275 7469 6f6e  ixelDistribution
-00003a70: 4164 6170 7461 7469 6f6e 290a 2d20 5b50  Adaptation).- [P
-00003a80: 6f73 7465 7269 7a65 5d28 6874 7470 733a  osterize](https:
-00003a90: 2f2f 616c 6275 6d65 6e74 6174 696f 6e73  //albumentations
-00003aa0: 2e61 692f 646f 6373 2f61 7069 5f72 6566  .ai/docs/api_ref
-00003ab0: 6572 656e 6365 2f61 7567 6d65 6e74 6174  erence/augmentat
-00003ac0: 696f 6e73 2f74 7261 6e73 666f 726d 732f  ions/transforms/
-00003ad0: 2361 6c62 756d 656e 7461 7469 6f6e 732e  #albumentations.
-00003ae0: 6175 676d 656e 7461 7469 6f6e 732e 7472  augmentations.tr
-00003af0: 616e 7366 6f72 6d73 2e50 6f73 7465 7269  ansforms.Posteri
-00003b00: 7a65 290a 2d20 5b52 4742 5368 6966 745d  ze).- [RGBShift]
-00003b10: 2868 7474 7073 3a2f 2f61 6c62 756d 656e  (https://albumen
-00003b20: 7461 7469 6f6e 732e 6169 2f64 6f63 732f  tations.ai/docs/
-00003b30: 6170 695f 7265 6665 7265 6e63 652f 6175  api_reference/au
-00003b40: 676d 656e 7461 7469 6f6e 732f 7472 616e  gmentations/tran
-00003b50: 7366 6f72 6d73 2f23 616c 6275 6d65 6e74  sforms/#albument
-00003b60: 6174 696f 6e73 2e61 7567 6d65 6e74 6174  ations.augmentat
-00003b70: 696f 6e73 2e74 7261 6e73 666f 726d 732e  ions.transforms.
-00003b80: 5247 4253 6869 6674 290a 2d20 5b52 616e  RGBShift).- [Ran
-00003b90: 646f 6d42 7269 6768 746e 6573 7343 6f6e  domBrightnessCon
-00003ba0: 7472 6173 745d 2868 7474 7073 3a2f 2f61  trast](https://a
-00003bb0: 6c62 756d 656e 7461 7469 6f6e 732e 6169  lbumentations.ai
-00003bc0: 2f64 6f63 732f 6170 695f 7265 6665 7265  /docs/api_refere
-00003bd0: 6e63 652f 6175 676d 656e 7461 7469 6f6e  nce/augmentation
-00003be0: 732f 7472 616e 7366 6f72 6d73 2f23 616c  s/transforms/#al
-00003bf0: 6275 6d65 6e74 6174 696f 6e73 2e61 7567  bumentations.aug
-00003c00: 6d65 6e74 6174 696f 6e73 2e74 7261 6e73  mentations.trans
-00003c10: 666f 726d 732e 5261 6e64 6f6d 4272 6967  forms.RandomBrig
-00003c20: 6874 6e65 7373 436f 6e74 7261 7374 290a  htnessContrast).
-00003c30: 2d20 5b52 616e 646f 6d46 6f67 5d28 6874  - [RandomFog](ht
-00003c40: 7470 733a 2f2f 616c 6275 6d65 6e74 6174  tps://albumentat
-00003c50: 696f 6e73 2e61 692f 646f 6373 2f61 7069  ions.ai/docs/api
-00003c60: 5f72 6566 6572 656e 6365 2f61 7567 6d65  _reference/augme
-00003c70: 6e74 6174 696f 6e73 2f74 7261 6e73 666f  ntations/transfo
-00003c80: 726d 732f 2361 6c62 756d 656e 7461 7469  rms/#albumentati
-00003c90: 6f6e 732e 6175 676d 656e 7461 7469 6f6e  ons.augmentation
-00003ca0: 732e 7472 616e 7366 6f72 6d73 2e52 616e  s.transforms.Ran
-00003cb0: 646f 6d46 6f67 290a 2d20 5b52 616e 646f  domFog).- [Rando
-00003cc0: 6d47 616d 6d61 5d28 6874 7470 733a 2f2f  mGamma](https://
-00003cd0: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
-00003ce0: 692f 646f 6373 2f61 7069 5f72 6566 6572  i/docs/api_refer
-00003cf0: 656e 6365 2f61 7567 6d65 6e74 6174 696f  ence/augmentatio
-00003d00: 6e73 2f74 7261 6e73 666f 726d 732f 2361  ns/transforms/#a
-00003d10: 6c62 756d 656e 7461 7469 6f6e 732e 6175  lbumentations.au
-00003d20: 676d 656e 7461 7469 6f6e 732e 7472 616e  gmentations.tran
-00003d30: 7366 6f72 6d73 2e52 616e 646f 6d47 616d  sforms.RandomGam
-00003d40: 6d61 290a 2d20 5b52 616e 646f 6d47 7261  ma).- [RandomGra
-00003d50: 7665 6c5d 2868 7474 7073 3a2f 2f61 6c62  vel](https://alb
-00003d60: 756d 656e 7461 7469 6f6e 732e 6169 2f64  umentations.ai/d
-00003d70: 6f63 732f 6170 695f 7265 6665 7265 6e63  ocs/api_referenc
-00003d80: 652f 6175 676d 656e 7461 7469 6f6e 732f  e/augmentations/
-00003d90: 7472 616e 7366 6f72 6d73 2f23 616c 6275  transforms/#albu
-00003da0: 6d65 6e74 6174 696f 6e73 2e61 7567 6d65  mentations.augme
-00003db0: 6e74 6174 696f 6e73 2e74 7261 6e73 666f  ntations.transfo
-00003dc0: 726d 732e 5261 6e64 6f6d 4772 6176 656c  rms.RandomGravel
-00003dd0: 290a 2d20 5b52 616e 646f 6d52 6169 6e5d  ).- [RandomRain]
-00003de0: 2868 7474 7073 3a2f 2f61 6c62 756d 656e  (https://albumen
-00003df0: 7461 7469 6f6e 732e 6169 2f64 6f63 732f  tations.ai/docs/
-00003e00: 6170 695f 7265 6665 7265 6e63 652f 6175  api_reference/au
-00003e10: 676d 656e 7461 7469 6f6e 732f 7472 616e  gmentations/tran
-00003e20: 7366 6f72 6d73 2f23 616c 6275 6d65 6e74  sforms/#albument
-00003e30: 6174 696f 6e73 2e61 7567 6d65 6e74 6174  ations.augmentat
-00003e40: 696f 6e73 2e74 7261 6e73 666f 726d 732e  ions.transforms.
-00003e50: 5261 6e64 6f6d 5261 696e 290a 2d20 5b52  RandomRain).- [R
-00003e60: 616e 646f 6d53 6861 646f 775d 2868 7474  andomShadow](htt
-00003e70: 7073 3a2f 2f61 6c62 756d 656e 7461 7469  ps://albumentati
-00003e80: 6f6e 732e 6169 2f64 6f63 732f 6170 695f  ons.ai/docs/api_
-00003e90: 7265 6665 7265 6e63 652f 6175 676d 656e  reference/augmen
-00003ea0: 7461 7469 6f6e 732f 7472 616e 7366 6f72  tations/transfor
-00003eb0: 6d73 2f23 616c 6275 6d65 6e74 6174 696f  ms/#albumentatio
-00003ec0: 6e73 2e61 7567 6d65 6e74 6174 696f 6e73  ns.augmentations
-00003ed0: 2e74 7261 6e73 666f 726d 732e 5261 6e64  .transforms.Rand
-00003ee0: 6f6d 5368 6164 6f77 290a 2d20 5b52 616e  omShadow).- [Ran
-00003ef0: 646f 6d53 6e6f 775d 2868 7474 7073 3a2f  domSnow](https:/
-00003f00: 2f61 6c62 756d 656e 7461 7469 6f6e 732e  /albumentations.
-00003f10: 6169 2f64 6f63 732f 6170 695f 7265 6665  ai/docs/api_refe
-00003f20: 7265 6e63 652f 6175 676d 656e 7461 7469  rence/augmentati
-00003f30: 6f6e 732f 7472 616e 7366 6f72 6d73 2f23  ons/transforms/#
-00003f40: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
-00003f50: 7567 6d65 6e74 6174 696f 6e73 2e74 7261  ugmentations.tra
-00003f60: 6e73 666f 726d 732e 5261 6e64 6f6d 536e  nsforms.RandomSn
-00003f70: 6f77 290a 2d20 5b52 616e 646f 6d53 756e  ow).- [RandomSun
-00003f80: 466c 6172 655d 2868 7474 7073 3a2f 2f61  Flare](https://a
-00003f90: 6c62 756d 656e 7461 7469 6f6e 732e 6169  lbumentations.ai
-00003fa0: 2f64 6f63 732f 6170 695f 7265 6665 7265  /docs/api_refere
-00003fb0: 6e63 652f 6175 676d 656e 7461 7469 6f6e  nce/augmentation
-00003fc0: 732f 7472 616e 7366 6f72 6d73 2f23 616c  s/transforms/#al
-00003fd0: 6275 6d65 6e74 6174 696f 6e73 2e61 7567  bumentations.aug
-00003fe0: 6d65 6e74 6174 696f 6e73 2e74 7261 6e73  mentations.trans
-00003ff0: 666f 726d 732e 5261 6e64 6f6d 5375 6e46  forms.RandomSunF
-00004000: 6c61 7265 290a 2d20 5b52 616e 646f 6d54  lare).- [RandomT
-00004010: 6f6e 6543 7572 7665 5d28 6874 7470 733a  oneCurve](https:
-00004020: 2f2f 616c 6275 6d65 6e74 6174 696f 6e73  //albumentations
-00004030: 2e61 692f 646f 6373 2f61 7069 5f72 6566  .ai/docs/api_ref
-00004040: 6572 656e 6365 2f61 7567 6d65 6e74 6174  erence/augmentat
-00004050: 696f 6e73 2f74 7261 6e73 666f 726d 732f  ions/transforms/
-00004060: 2361 6c62 756d 656e 7461 7469 6f6e 732e  #albumentations.
-00004070: 6175 676d 656e 7461 7469 6f6e 732e 7472  augmentations.tr
-00004080: 616e 7366 6f72 6d73 2e52 616e 646f 6d54  ansforms.RandomT
-00004090: 6f6e 6543 7572 7665 290a 2d20 5b52 696e  oneCurve).- [Rin
-000040a0: 6769 6e67 4f76 6572 7368 6f6f 745d 2868  gingOvershoot](h
-000040b0: 7474 7073 3a2f 2f61 6c62 756d 656e 7461  ttps://albumenta
-000040c0: 7469 6f6e 732e 6169 2f64 6f63 732f 6170  tions.ai/docs/ap
-000040d0: 695f 7265 6665 7265 6e63 652f 6175 676d  i_reference/augm
-000040e0: 656e 7461 7469 6f6e 732f 7472 616e 7366  entations/transf
-000040f0: 6f72 6d73 2f23 616c 6275 6d65 6e74 6174  orms/#albumentat
-00004100: 696f 6e73 2e61 7567 6d65 6e74 6174 696f  ions.augmentatio
-00004110: 6e73 2e74 7261 6e73 666f 726d 732e 5269  ns.transforms.Ri
-00004120: 6e67 696e 674f 7665 7273 686f 6f74 290a  ngingOvershoot).
-00004130: 2d20 5b53 6861 7270 656e 5d28 6874 7470  - [Sharpen](http
-00004140: 733a 2f2f 616c 6275 6d65 6e74 6174 696f  s://albumentatio
-00004150: 6e73 2e61 692f 646f 6373 2f61 7069 5f72  ns.ai/docs/api_r
-00004160: 6566 6572 656e 6365 2f61 7567 6d65 6e74  eference/augment
-00004170: 6174 696f 6e73 2f74 7261 6e73 666f 726d  ations/transform
-00004180: 732f 2361 6c62 756d 656e 7461 7469 6f6e  s/#albumentation
-00004190: 732e 6175 676d 656e 7461 7469 6f6e 732e  s.augmentations.
-000041a0: 7472 616e 7366 6f72 6d73 2e53 6861 7270  transforms.Sharp
-000041b0: 656e 290a 2d20 5b53 6f6c 6172 697a 655d  en).- [Solarize]
-000041c0: 2868 7474 7073 3a2f 2f61 6c62 756d 656e  (https://albumen
-000041d0: 7461 7469 6f6e 732e 6169 2f64 6f63 732f  tations.ai/docs/
-000041e0: 6170 695f 7265 6665 7265 6e63 652f 6175  api_reference/au
-000041f0: 676d 656e 7461 7469 6f6e 732f 7472 616e  gmentations/tran
-00004200: 7366 6f72 6d73 2f23 616c 6275 6d65 6e74  sforms/#albument
-00004210: 6174 696f 6e73 2e61 7567 6d65 6e74 6174  ations.augmentat
-00004220: 696f 6e73 2e74 7261 6e73 666f 726d 732e  ions.transforms.
-00004230: 536f 6c61 7269 7a65 290a 2d20 5b53 7061  Solarize).- [Spa
-00004240: 7474 6572 5d28 6874 7470 733a 2f2f 616c  tter](https://al
-00004250: 6275 6d65 6e74 6174 696f 6e73 2e61 692f  bumentations.ai/
-00004260: 646f 6373 2f61 7069 5f72 6566 6572 656e  docs/api_referen
-00004270: 6365 2f61 7567 6d65 6e74 6174 696f 6e73  ce/augmentations
-00004280: 2f74 7261 6e73 666f 726d 732f 2361 6c62  /transforms/#alb
-00004290: 756d 656e 7461 7469 6f6e 732e 6175 676d  umentations.augm
-000042a0: 656e 7461 7469 6f6e 732e 7472 616e 7366  entations.transf
-000042b0: 6f72 6d73 2e53 7061 7474 6572 290a 2d20  orms.Spatter).- 
-000042c0: 5b53 7570 6572 7069 7865 6c73 5d28 6874  [Superpixels](ht
-000042d0: 7470 733a 2f2f 616c 6275 6d65 6e74 6174  tps://albumentat
-000042e0: 696f 6e73 2e61 692f 646f 6373 2f61 7069  ions.ai/docs/api
-000042f0: 5f72 6566 6572 656e 6365 2f61 7567 6d65  _reference/augme
-00004300: 6e74 6174 696f 6e73 2f74 7261 6e73 666f  ntations/transfo
-00004310: 726d 732f 2361 6c62 756d 656e 7461 7469  rms/#albumentati
-00004320: 6f6e 732e 6175 676d 656e 7461 7469 6f6e  ons.augmentation
-00004330: 732e 7472 616e 7366 6f72 6d73 2e53 7570  s.transforms.Sup
-00004340: 6572 7069 7865 6c73 290a 2d20 5b54 656d  erpixels).- [Tem
-00004350: 706c 6174 6554 7261 6e73 666f 726d 5d28  plateTransform](
-00004360: 6874 7470 733a 2f2f 616c 6275 6d65 6e74  https://albument
-00004370: 6174 696f 6e73 2e61 692f 646f 6373 2f61  ations.ai/docs/a
-00004380: 7069 5f72 6566 6572 656e 6365 2f61 7567  pi_reference/aug
-00004390: 6d65 6e74 6174 696f 6e73 2f74 7261 6e73  mentations/trans
-000043a0: 666f 726d 732f 2361 6c62 756d 656e 7461  forms/#albumenta
-000043b0: 7469 6f6e 732e 6175 676d 656e 7461 7469  tions.augmentati
-000043c0: 6f6e 732e 7472 616e 7366 6f72 6d73 2e54  ons.transforms.T
-000043d0: 656d 706c 6174 6554 7261 6e73 666f 726d  emplateTransform
-000043e0: 290a 2d20 5b54 6f46 6c6f 6174 5d28 6874  ).- [ToFloat](ht
-000043f0: 7470 733a 2f2f 616c 6275 6d65 6e74 6174  tps://albumentat
-00004400: 696f 6e73 2e61 692f 646f 6373 2f61 7069  ions.ai/docs/api
-00004410: 5f72 6566 6572 656e 6365 2f61 7567 6d65  _reference/augme
-00004420: 6e74 6174 696f 6e73 2f74 7261 6e73 666f  ntations/transfo
-00004430: 726d 732f 2361 6c62 756d 656e 7461 7469  rms/#albumentati
-00004440: 6f6e 732e 6175 676d 656e 7461 7469 6f6e  ons.augmentation
-00004450: 732e 7472 616e 7366 6f72 6d73 2e54 6f46  s.transforms.ToF
-00004460: 6c6f 6174 290a 2d20 5b54 6f47 7261 795d  loat).- [ToGray]
-00004470: 2868 7474 7073 3a2f 2f61 6c62 756d 656e  (https://albumen
-00004480: 7461 7469 6f6e 732e 6169 2f64 6f63 732f  tations.ai/docs/
-00004490: 6170 695f 7265 6665 7265 6e63 652f 6175  api_reference/au
-000044a0: 676d 656e 7461 7469 6f6e 732f 7472 616e  gmentations/tran
-000044b0: 7366 6f72 6d73 2f23 616c 6275 6d65 6e74  sforms/#albument
-000044c0: 6174 696f 6e73 2e61 7567 6d65 6e74 6174  ations.augmentat
-000044d0: 696f 6e73 2e74 7261 6e73 666f 726d 732e  ions.transforms.
-000044e0: 546f 4772 6179 290a 2d20 5b54 6f52 4742  ToGray).- [ToRGB
-000044f0: 5d28 6874 7470 733a 2f2f 616c 6275 6d65  ](https://albume
-00004500: 6e74 6174 696f 6e73 2e61 692f 646f 6373  ntations.ai/docs
-00004510: 2f61 7069 5f72 6566 6572 656e 6365 2f61  /api_reference/a
-00004520: 7567 6d65 6e74 6174 696f 6e73 2f74 7261  ugmentations/tra
-00004530: 6e73 666f 726d 732f 2361 6c62 756d 656e  nsforms/#albumen
-00004540: 7461 7469 6f6e 732e 6175 676d 656e 7461  tations.augmenta
-00004550: 7469 6f6e 732e 7472 616e 7366 6f72 6d73  tions.transforms
-00004560: 2e54 6f52 4742 290a 2d20 5b54 6f53 6570  .ToRGB).- [ToSep
-00004570: 6961 5d28 6874 7470 733a 2f2f 616c 6275  ia](https://albu
-00004580: 6d65 6e74 6174 696f 6e73 2e61 692f 646f  mentations.ai/do
-00004590: 6373 2f61 7069 5f72 6566 6572 656e 6365  cs/api_reference
-000045a0: 2f61 7567 6d65 6e74 6174 696f 6e73 2f74  /augmentations/t
-000045b0: 7261 6e73 666f 726d 732f 2361 6c62 756d  ransforms/#album
-000045c0: 656e 7461 7469 6f6e 732e 6175 676d 656e  entations.augmen
-000045d0: 7461 7469 6f6e 732e 7472 616e 7366 6f72  tations.transfor
-000045e0: 6d73 2e54 6f53 6570 6961 290a 2d20 5b55  ms.ToSepia).- [U
-000045f0: 6e73 6861 7270 4d61 736b 5d28 6874 7470  nsharpMask](http
-00004600: 733a 2f2f 616c 6275 6d65 6e74 6174 696f  s://albumentatio
-00004610: 6e73 2e61 692f 646f 6373 2f61 7069 5f72  ns.ai/docs/api_r
-00004620: 6566 6572 656e 6365 2f61 7567 6d65 6e74  eference/augment
-00004630: 6174 696f 6e73 2f74 7261 6e73 666f 726d  ations/transform
-00004640: 732f 2361 6c62 756d 656e 7461 7469 6f6e  s/#albumentation
-00004650: 732e 6175 676d 656e 7461 7469 6f6e 732e  s.augmentations.
-00004660: 7472 616e 7366 6f72 6d73 2e55 6e73 6861  transforms.Unsha
-00004670: 7270 4d61 736b 290a 2d20 5b5a 6f6f 6d42  rpMask).- [ZoomB
-00004680: 6c75 725d 2868 7474 7073 3a2f 2f61 6c62  lur](https://alb
-00004690: 756d 656e 7461 7469 6f6e 732e 6169 2f64  umentations.ai/d
-000046a0: 6f63 732f 6170 695f 7265 6665 7265 6e63  ocs/api_referenc
-000046b0: 652f 6175 676d 656e 7461 7469 6f6e 732f  e/augmentations/
-000046c0: 626c 7572 2f74 7261 6e73 666f 726d 732f  blur/transforms/
-000046d0: 2361 6c62 756d 656e 7461 7469 6f6e 732e  #albumentations.
-000046e0: 6175 676d 656e 7461 7469 6f6e 732e 626c  augmentations.bl
-000046f0: 7572 2e74 7261 6e73 666f 726d 732e 5a6f  ur.transforms.Zo
-00004700: 6f6d 426c 7572 290a 0a23 2323 2053 7061  omBlur)..### Spa
-00004710: 7469 616c 2d6c 6576 656c 2074 7261 6e73  tial-level trans
-00004720: 666f 726d 730a 0a53 7061 7469 616c 2d6c  forms..Spatial-l
-00004730: 6576 656c 2074 7261 6e73 666f 726d 7320  evel transforms 
-00004740: 7769 6c6c 2073 696d 756c 7461 6e65 6f75  will simultaneou
-00004750: 736c 7920 6368 616e 6765 2062 6f74 6820  sly change both 
-00004760: 616e 2069 6e70 7574 2069 6d61 6765 2061  an input image a
-00004770: 7320 7765 6c6c 2061 7320 6164 6469 7469  s well as additi
-00004780: 6f6e 616c 2074 6172 6765 7473 2073 7563  onal targets suc
-00004790: 6820 6173 206d 6173 6b73 2c20 626f 756e  h as masks, boun
-000047a0: 6469 6e67 2062 6f78 6573 2c20 616e 6420  ding boxes, and 
-000047b0: 6b65 7970 6f69 6e74 732e 2054 6865 2066  keypoints. The f
-000047c0: 6f6c 6c6f 7769 6e67 2074 6162 6c65 2073  ollowing table s
-000047d0: 686f 7773 2077 6869 6368 2061 6464 6974  hows which addit
-000047e0: 696f 6e61 6c20 7461 7267 6574 7320 6172  ional targets ar
-000047f0: 6520 7375 7070 6f72 7465 6420 6279 2065  e supported by e
-00004800: 6163 6820 7472 616e 7366 6f72 6d2e 0a0a  ach transform...
-00004810: 7c20 5472 616e 7366 6f72 6d20 2020 2020  | Transform     
-00004820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000048a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000048b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000048c0: 2020 7c20 496d 6167 6520 7c20 4d61 736b    | Image | Mask
-000048d0: 207c 2042 426f 7865 7320 7c20 4b65 7970   | BBoxes | Keyp
-000048e0: 6f69 6e74 7320 7c0a 7c20 2d2d 2d2d 2d2d  oints |.| ------
-000048f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004900: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004910: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004920: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004930: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004940: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004950: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004960: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004970: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004980: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004990: 2d2d 2d2d 2d2d 2d2d 2d20 7c20 3a2d 2d2d  --------- | :---
-000049a0: 3a20 7c20 3a2d 2d3a 207c 203a 2d2d 2d2d  : | :--: | :----
-000049b0: 3a20 7c20 3a2d 2d2d 2d2d 2d2d 3a20 7c0a  : | :-------: |.
-000049c0: 7c20 5b41 6666 696e 655d 2868 7474 7073  | [Affine](https
-000049d0: 3a2f 2f61 6c62 756d 656e 7461 7469 6f6e  ://albumentation
-000049e0: 732e 6169 2f64 6f63 732f 6170 695f 7265  s.ai/docs/api_re
-000049f0: 6665 7265 6e63 652f 6175 676d 656e 7461  ference/augmenta
-00004a00: 7469 6f6e 732f 6765 6f6d 6574 7269 632f  tions/geometric/
-00004a10: 7472 616e 7366 6f72 6d73 2f23 616c 6275  transforms/#albu
-00004a20: 6d65 6e74 6174 696f 6e73 2e61 7567 6d65  mentations.augme
-00004a30: 6e74 6174 696f 6e73 2e67 656f 6d65 7472  ntations.geometr
-00004a40: 6963 2e74 7261 6e73 666f 726d 732e 4166  ic.transforms.Af
-00004a50: 6669 6e65 2920 2020 2020 2020 2020 2020  fine)           
-00004a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a70: 2020 7c20 e29c 9320 2020 2020 7c20 e29c    | ...     | ..
-00004a80: 9320 2020 207c 20e2 9c93 2020 2020 2020  .    | ...      
-00004a90: 7c20 e29c 9320 2020 2020 2020 2020 7c0a  | ...         |.
-00004aa0: 7c20 5b42 426f 7853 6166 6552 616e 646f  | [BBoxSafeRando
-00004ab0: 6d43 726f 705d 2868 7474 7073 3a2f 2f61  mCrop](https://a
-00004ac0: 6c62 756d 656e 7461 7469 6f6e 732e 6169  lbumentations.ai
-00004ad0: 2f64 6f63 732f 6170 695f 7265 6665 7265  /docs/api_refere
-00004ae0: 6e63 652f 6175 676d 656e 7461 7469 6f6e  nce/augmentation
-00004af0: 732f 6372 6f70 732f 7472 616e 7366 6f72  s/crops/transfor
-00004b00: 6d73 2f23 616c 6275 6d65 6e74 6174 696f  ms/#albumentatio
-00004b10: 6e73 2e61 7567 6d65 6e74 6174 696f 6e73  ns.augmentations
-00004b20: 2e63 726f 7073 2e74 7261 6e73 666f 726d  .crops.transform
-00004b30: 732e 4242 6f78 5361 6665 5261 6e64 6f6d  s.BBoxSafeRandom
-00004b40: 4372 6f70 2920 2020 2020 2020 2020 2020  Crop)           
-00004b50: 2020 7c20 e29c 9320 2020 2020 7c20 e29c    | ...     | ..
-00004b60: 9320 2020 207c 20e2 9c93 2020 2020 2020  .    | ...      
-00004b70: 7c20 2020 2020 2020 2020 2020 7c0a 7c20  |           |.| 
-00004b80: 5b43 656e 7465 7243 726f 705d 2868 7474  [CenterCrop](htt
-00004b90: 7073 3a2f 2f61 6c62 756d 656e 7461 7469  ps://albumentati
-00004ba0: 6f6e 732e 6169 2f64 6f63 732f 6170 695f  ons.ai/docs/api_
-00004bb0: 7265 6665 7265 6e63 652f 6175 676d 656e  reference/augmen
-00004bc0: 7461 7469 6f6e 732f 6372 6f70 732f 7472  tations/crops/tr
-00004bd0: 616e 7366 6f72 6d73 2f23 616c 6275 6d65  ansforms/#albume
-00004be0: 6e74 6174 696f 6e73 2e61 7567 6d65 6e74  ntations.augment
-00004bf0: 6174 696f 6e73 2e63 726f 7073 2e74 7261  ations.crops.tra
-00004c00: 6e73 666f 726d 732e 4365 6e74 6572 4372  nsforms.CenterCr
-00004c10: 6f70 2920 2020 2020 2020 2020 2020 2020  op)             
-00004c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c30: 7c20 e29c 9320 2020 2020 7c20 e29c 9320  | ...     | ... 
-00004c40: 2020 207c 20e2 9c93 2020 2020 2020 7c20     | ...      | 
-00004c50: e29c 9320 2020 2020 2020 2020 7c0a 7c20  ...         |.| 
-00004c60: 5b43 6f61 7273 6544 726f 706f 7574 5d28  [CoarseDropout](
-00004c70: 6874 7470 733a 2f2f 616c 6275 6d65 6e74  https://albument
-00004c80: 6174 696f 6e73 2e61 692f 646f 6373 2f61  ations.ai/docs/a
-00004c90: 7069 5f72 6566 6572 656e 6365 2f61 7567  pi_reference/aug
-00004ca0: 6d65 6e74 6174 696f 6e73 2f64 726f 706f  mentations/dropo
-00004cb0: 7574 2f63 6f61 7273 655f 6472 6f70 6f75  ut/coarse_dropou
-00004cc0: 742f 2361 6c62 756d 656e 7461 7469 6f6e  t/#albumentation
-00004cd0: 732e 6175 676d 656e 7461 7469 6f6e 732e  s.augmentations.
-00004ce0: 6472 6f70 6f75 742e 636f 6172 7365 5f64  dropout.coarse_d
-00004cf0: 726f 706f 7574 2e43 6f61 7273 6544 726f  ropout.CoarseDro
-00004d00: 706f 7574 2920 2020 2020 2020 2020 2020  pout)           
-00004d10: 7c20 e29c 9320 2020 2020 7c20 e29c 9320  | ...     | ... 
-00004d20: 2020 207c 2020 2020 2020 2020 7c20 e29c     |        | ..
-00004d30: 9320 2020 2020 2020 2020 7c0a 7c20 5b43  .         |.| [C
-00004d40: 726f 705d 2868 7474 7073 3a2f 2f61 6c62  rop](https://alb
-00004d50: 756d 656e 7461 7469 6f6e 732e 6169 2f64  umentations.ai/d
-00004d60: 6f63 732f 6170 695f 7265 6665 7265 6e63  ocs/api_referenc
-00004d70: 652f 6175 676d 656e 7461 7469 6f6e 732f  e/augmentations/
-00004d80: 6372 6f70 732f 7472 616e 7366 6f72 6d73  crops/transforms
-00004d90: 2f23 616c 6275 6d65 6e74 6174 696f 6e73  /#albumentations
-00004da0: 2e61 7567 6d65 6e74 6174 696f 6e73 2e63  .augmentations.c
-00004db0: 726f 7073 2e74 7261 6e73 666f 726d 732e  rops.transforms.
-00004dc0: 4372 6f70 2920 2020 2020 2020 2020 2020  Crop)           
-00004dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004de0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00004df0: e29c 9320 2020 2020 7c20 e29c 9320 2020  ...     | ...   
-00004e00: 207c 20e2 9c93 2020 2020 2020 7c20 e29c   | ...      | ..
-00004e10: 9320 2020 2020 2020 2020 7c0a 7c20 5b43  .         |.| [C
-00004e20: 726f 7041 6e64 5061 645d 2868 7474 7073  ropAndPad](https
-00004e30: 3a2f 2f61 6c62 756d 656e 7461 7469 6f6e  ://albumentation
-00004e40: 732e 6169 2f64 6f63 732f 6170 695f 7265  s.ai/docs/api_re
-00004e50: 6665 7265 6e63 652f 6175 676d 656e 7461  ference/augmenta
-00004e60: 7469 6f6e 732f 6372 6f70 732f 7472 616e  tions/crops/tran
-00004e70: 7366 6f72 6d73 2f23 616c 6275 6d65 6e74  sforms/#albument
-00004e80: 6174 696f 6e73 2e61 7567 6d65 6e74 6174  ations.augmentat
-00004e90: 696f 6e73 2e63 726f 7073 2e74 7261 6e73  ions.crops.trans
-00004ea0: 666f 726d 732e 4372 6f70 416e 6450 6164  forms.CropAndPad
-00004eb0: 2920 2020 2020 2020 2020 2020 2020 2020  )               
-00004ec0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00004ed0: e29c 9320 2020 2020 7c20 e29c 9320 2020  ...     | ...   
-00004ee0: 207c 20e2 9c93 2020 2020 2020 7c20 e29c   | ...      | ..
-00004ef0: 9320 2020 2020 2020 2020 7c0a 7c20 5b43  .         |.| [C
-00004f00: 726f 704e 6f6e 456d 7074 794d 6173 6b49  ropNonEmptyMaskI
-00004f10: 6645 7869 7374 735d 2868 7474 7073 3a2f  fExists](https:/
-00004f20: 2f61 6c62 756d 656e 7461 7469 6f6e 732e  /albumentations.
-00004f30: 6169 2f64 6f63 732f 6170 695f 7265 6665  ai/docs/api_refe
-00004f40: 7265 6e63 652f 6175 676d 656e 7461 7469  rence/augmentati
-00004f50: 6f6e 732f 6372 6f70 732f 7472 616e 7366  ons/crops/transf
-00004f60: 6f72 6d73 2f23 616c 6275 6d65 6e74 6174  orms/#albumentat
-00004f70: 696f 6e73 2e61 7567 6d65 6e74 6174 696f  ions.augmentatio
-00004f80: 6e73 2e63 726f 7073 2e74 7261 6e73 666f  ns.crops.transfo
-00004f90: 726d 732e 4372 6f70 4e6f 6e45 6d70 7479  rms.CropNonEmpty
-00004fa0: 4d61 736b 4966 4578 6973 7473 2920 7c20  MaskIfExists) | 
-00004fb0: e29c 9320 2020 2020 7c20 e29c 9320 2020  ...     | ...   
-00004fc0: 207c 20e2 9c93 2020 2020 2020 7c20 e29c   | ...      | ..
-00004fd0: 9320 2020 2020 2020 2020 7c0a 7c20 5b45  .         |.| [E
-00004fe0: 6c61 7374 6963 5472 616e 7366 6f72 6d5d  lasticTransform]
-00004ff0: 2868 7474 7073 3a2f 2f61 6c62 756d 656e  (https://albumen
-00005000: 7461 7469 6f6e 732e 6169 2f64 6f63 732f  tations.ai/docs/
-00005010: 6170 695f 7265 6665 7265 6e63 652f 6175  api_reference/au
-00005020: 676d 656e 7461 7469 6f6e 732f 6765 6f6d  gmentations/geom
-00005030: 6574 7269 632f 7472 616e 7366 6f72 6d73  etric/transforms
-00005040: 2f23 616c 6275 6d65 6e74 6174 696f 6e73  /#albumentations
-00005050: 2e61 7567 6d65 6e74 6174 696f 6e73 2e67  .augmentations.g
-00005060: 656f 6d65 7472 6963 2e74 7261 6e73 666f  eometric.transfo
-00005070: 726d 732e 456c 6173 7469 6354 7261 6e73  rms.ElasticTrans
-00005080: 666f 726d 2920 2020 2020 2020 2020 7c20  form)         | 
-00005090: e29c 9320 2020 2020 7c20 e29c 9320 2020  ...     | ...   
-000050a0: 207c 20e2 9c93 2020 2020 2020 7c20 2020   | ...      |   
-000050b0: 2020 2020 2020 2020 7c0a 7c20 5b46 6c69          |.| [Fli
-000050c0: 705d 2868 7474 7073 3a2f 2f61 6c62 756d  p](https://album
-000050d0: 656e 7461 7469 6f6e 732e 6169 2f64 6f63  entations.ai/doc
-000050e0: 732f 6170 695f 7265 6665 7265 6e63 652f  s/api_reference/
-000050f0: 6175 676d 656e 7461 7469 6f6e 732f 6765  augmentations/ge
-00005100: 6f6d 6574 7269 632f 7472 616e 7366 6f72  ometric/transfor
-00005110: 6d73 2f23 616c 6275 6d65 6e74 6174 696f  ms/#albumentatio
-00005120: 6e73 2e61 7567 6d65 6e74 6174 696f 6e73  ns.augmentations
-00005130: 2e67 656f 6d65 7472 6963 2e74 7261 6e73  .geometric.trans
-00005140: 666f 726d 732e 466c 6970 2920 2020 2020  forms.Flip)     
-00005150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005160: 2020 2020 2020 2020 2020 2020 7c20 e29c              | ..
-00005170: 9320 2020 2020 7c20 e29c 9320 2020 207c  .     | ...    |
-00005180: 20e2 9c93 2020 2020 2020 7c20 e29c 9320   ...      | ... 
-00005190: 2020 2020 2020 2020 7c0a 7c20 5b47 7269          |.| [Gri
-000051a0: 6444 6973 746f 7274 696f 6e5d 2868 7474  dDistortion](htt
-000051b0: 7073 3a2f 2f61 6c62 756d 656e 7461 7469  ps://albumentati
-000051c0: 6f6e 732e 6169 2f64 6f63 732f 6170 695f  ons.ai/docs/api_
-000051d0: 7265 6665 7265 6e63 652f 6175 676d 656e  reference/augmen
-000051e0: 7461 7469 6f6e 732f 6765 6f6d 6574 7269  tations/geometri
-000051f0: 632f 7472 616e 7366 6f72 6d73 2f23 616c  c/transforms/#al
-00005200: 6275 6d65 6e74 6174 696f 6e73 2e61 7567  bumentations.aug
-00005210: 6d65 6e74 6174 696f 6e73 2e67 656f 6d65  mentations.geome
-00005220: 7472 6963 2e74 7261 6e73 666f 726d 732e  tric.transforms.
-00005230: 4772 6964 4469 7374 6f72 7469 6f6e 2920  GridDistortion) 
-00005240: 2020 2020 2020 2020 2020 2020 7c20 e29c              | ..
-00005250: 9320 2020 2020 7c20 e29c 9320 2020 207c  .     | ...    |
-00005260: 20e2 9c93 2020 2020 2020 7c20 2020 2020   ...      |     
-00005270: 2020 2020 2020 7c0a 7c20 5b47 7269 6444        |.| [GridD
-00005280: 726f 706f 7574 5d28 6874 7470 733a 2f2f  ropout](https://
-00005290: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
-000052a0: 692f 646f 6373 2f61 7069 5f72 6566 6572  i/docs/api_refer
-000052b0: 656e 6365 2f61 7567 6d65 6e74 6174 696f  ence/augmentatio
-000052c0: 6e73 2f64 726f 706f 7574 2f67 7269 645f  ns/dropout/grid_
-000052d0: 6472 6f70 6f75 742f 2361 6c62 756d 656e  dropout/#albumen
-000052e0: 7461 7469 6f6e 732e 6175 676d 656e 7461  tations.augmenta
-000052f0: 7469 6f6e 732e 6472 6f70 6f75 742e 6772  tions.dropout.gr
-00005300: 6964 5f64 726f 706f 7574 2e47 7269 6444  id_dropout.GridD
-00005310: 726f 706f 7574 2920 2020 2020 2020 2020  ropout)         
-00005320: 2020 2020 2020 2020 2020 7c20 e29c 9320            | ... 
-00005330: 2020 2020 7c20 e29c 9320 2020 207c 2020      | ...    |  
-00005340: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-00005350: 2020 7c0a 7c20 5b48 6f72 697a 6f6e 7461    |.| [Horizonta
-00005360: 6c46 6c69 705d 2868 7474 7073 3a2f 2f61  lFlip](https://a
-00005370: 6c62 756d 656e 7461 7469 6f6e 732e 6169  lbumentations.ai
-00005380: 2f64 6f63 732f 6170 695f 7265 6665 7265  /docs/api_refere
-00005390: 6e63 652f 6175 676d 656e 7461 7469 6f6e  nce/augmentation
-000053a0: 732f 6765 6f6d 6574 7269 632f 7472 616e  s/geometric/tran
-000053b0: 7366 6f72 6d73 2f23 616c 6275 6d65 6e74  sforms/#albument
-000053c0: 6174 696f 6e73 2e61 7567 6d65 6e74 6174  ations.augmentat
-000053d0: 696f 6e73 2e67 656f 6d65 7472 6963 2e74  ions.geometric.t
-000053e0: 7261 6e73 666f 726d 732e 486f 7269 7a6f  ransforms.Horizo
-000053f0: 6e74 616c 466c 6970 2920 2020 2020 2020  ntalFlip)       
-00005400: 2020 2020 2020 7c20 e29c 9320 2020 2020        | ...     
-00005410: 7c20 e29c 9320 2020 207c 20e2 9c93 2020  | ...    | ...  
-00005420: 2020 2020 7c20 e29c 9320 2020 2020 2020      | ...       
-00005430: 2020 7c0a 7c20 5b4c 616d 6264 615d 2868    |.| [Lambda](h
-00005440: 7474 7073 3a2f 2f61 6c62 756d 656e 7461  ttps://albumenta
-00005450: 7469 6f6e 732e 6169 2f64 6f63 732f 6170  tions.ai/docs/ap
-00005460: 695f 7265 6665 7265 6e63 652f 6175 676d  i_reference/augm
-00005470: 656e 7461 7469 6f6e 732f 7472 616e 7366  entations/transf
-00005480: 6f72 6d73 2f23 616c 6275 6d65 6e74 6174  orms/#albumentat
-00005490: 696f 6e73 2e61 7567 6d65 6e74 6174 696f  ions.augmentatio
-000054a0: 6e73 2e74 7261 6e73 666f 726d 732e 4c61  ns.transforms.La
-000054b0: 6d62 6461 2920 2020 2020 2020 2020 2020  mbda)           
-000054c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000054d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000054e0: 2020 2020 2020 7c20 e29c 9320 2020 2020        | ...     
-000054f0: 7c20 e29c 9320 2020 207c 20e2 9c93 2020  | ...    | ...  
-00005500: 2020 2020 7c20 e29c 9320 2020 2020 2020      | ...       
-00005510: 2020 7c0a 7c20 5b4c 6f6e 6765 7374 4d61    |.| [LongestMa
-00005520: 7853 697a 655d 2868 7474 7073 3a2f 2f61  xSize](https://a
-00005530: 6c62 756d 656e 7461 7469 6f6e 732e 6169  lbumentations.ai
-00005540: 2f64 6f63 732f 6170 695f 7265 6665 7265  /docs/api_refere
-00005550: 6e63 652f 6175 676d 656e 7461 7469 6f6e  nce/augmentation
-00005560: 732f 6765 6f6d 6574 7269 632f 7265 7369  s/geometric/resi
-00005570: 7a65 2f23 616c 6275 6d65 6e74 6174 696f  ze/#albumentatio
-00005580: 6e73 2e61 7567 6d65 6e74 6174 696f 6e73  ns.augmentations
-00005590: 2e67 656f 6d65 7472 6963 2e72 6573 697a  .geometric.resiz
-000055a0: 652e 4c6f 6e67 6573 744d 6178 5369 7a65  e.LongestMaxSize
-000055b0: 2920 2020 2020 2020 2020 2020 2020 2020  )               
-000055c0: 2020 2020 2020 7c20 e29c 9320 2020 2020        | ...     
-000055d0: 7c20 e29c 9320 2020 207c 20e2 9c93 2020  | ...    | ...  
-000055e0: 2020 2020 7c20 e29c 9320 2020 2020 2020      | ...       
-000055f0: 2020 7c0a 7c20 5b4d 6173 6b44 726f 706f    |.| [MaskDropo
-00005600: 7574 5d28 6874 7470 733a 2f2f 616c 6275  ut](https://albu
-00005610: 6d65 6e74 6174 696f 6e73 2e61 692f 646f  mentations.ai/do
-00005620: 6373 2f61 7069 5f72 6566 6572 656e 6365  cs/api_reference
-00005630: 2f61 7567 6d65 6e74 6174 696f 6e73 2f64  /augmentations/d
-00005640: 726f 706f 7574 2f6d 6173 6b5f 6472 6f70  ropout/mask_drop
-00005650: 6f75 742f 2361 6c62 756d 656e 7461 7469  out/#albumentati
-00005660: 6f6e 732e 6175 676d 656e 7461 7469 6f6e  ons.augmentation
-00005670: 732e 6472 6f70 6f75 742e 6d61 736b 5f64  s.dropout.mask_d
-00005680: 726f 706f 7574 2e4d 6173 6b44 726f 706f  ropout.MaskDropo
-00005690: 7574 2920 2020 2020 2020 2020 2020 2020  ut)             
-000056a0: 2020 2020 2020 7c20 e29c 9320 2020 2020        | ...     
-000056b0: 7c20 e29c 9320 2020 207c 2020 2020 2020  | ...    |      
-000056c0: 2020 7c20 2020 2020 2020 2020 2020 7c0a    |           |.
-000056d0: 7c20 5b4e 6f4f 705d 2868 7474 7073 3a2f  | [NoOp](https:/
-000056e0: 2f61 6c62 756d 656e 7461 7469 6f6e 732e  /albumentations.
-000056f0: 6169 2f64 6f63 732f 6170 695f 7265 6665  ai/docs/api_refe
-00005700: 7265 6e63 652f 636f 7265 2f74 7261 6e73  rence/core/trans
-00005710: 666f 726d 735f 696e 7465 7266 6163 652f  forms_interface/
-00005720: 2361 6c62 756d 656e 7461 7469 6f6e 732e  #albumentations.
-00005730: 636f 7265 2e74 7261 6e73 666f 726d 735f  core.transforms_
-00005740: 696e 7465 7266 6163 652e 4e6f 4f70 2920  interface.NoOp) 
-00005750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005780: 2020 7c20 e29c 9320 2020 2020 7c20 e29c    | ...     | ..
-00005790: 9320 2020 207c 20e2 9c93 2020 2020 2020  .    | ...      
-000057a0: 7c20 e29c 9320 2020 2020 2020 2020 7c0a  | ...         |.
-000057b0: 7c20 5b4f 7074 6963 616c 4469 7374 6f72  | [OpticalDistor
-000057c0: 7469 6f6e 5d28 6874 7470 733a 2f2f 616c  tion](https://al
-000057d0: 6275 6d65 6e74 6174 696f 6e73 2e61 692f  bumentations.ai/
-000057e0: 646f 6373 2f61 7069 5f72 6566 6572 656e  docs/api_referen
-000057f0: 6365 2f61 7567 6d65 6e74 6174 696f 6e73  ce/augmentations
-00005800: 2f67 656f 6d65 7472 6963 2f74 7261 6e73  /geometric/trans
-00005810: 666f 726d 732f 2361 6c62 756d 656e 7461  forms/#albumenta
-00005820: 7469 6f6e 732e 6175 676d 656e 7461 7469  tions.augmentati
-00005830: 6f6e 732e 6765 6f6d 6574 7269 632e 7472  ons.geometric.tr
-00005840: 616e 7366 6f72 6d73 2e4f 7074 6963 616c  ansforms.Optical
-00005850: 4469 7374 6f72 7469 6f6e 2920 2020 2020  Distortion)     
-00005860: 2020 7c20 e29c 9320 2020 2020 7c20 e29c    | ...     | ..
-00005870: 9320 2020 207c 20e2 9c93 2020 2020 2020  .    | ...      
-00005880: 7c20 2020 2020 2020 2020 2020 7c0a 7c20  |           |.| 
-00005890: 5b50 6164 4966 4e65 6564 6564 5d28 6874  [PadIfNeeded](ht
-000058a0: 7470 733a 2f2f 616c 6275 6d65 6e74 6174  tps://albumentat
-000058b0: 696f 6e73 2e61 692f 646f 6373 2f61 7069  ions.ai/docs/api
-000058c0: 5f72 6566 6572 656e 6365 2f61 7567 6d65  _reference/augme
-000058d0: 6e74 6174 696f 6e73 2f67 656f 6d65 7472  ntations/geometr
-000058e0: 6963 2f74 7261 6e73 666f 726d 732f 2361  ic/transforms/#a
-000058f0: 6c62 756d 656e 7461 7469 6f6e 732e 6175  lbumentations.au
-00005900: 676d 656e 7461 7469 6f6e 732e 6765 6f6d  gmentations.geom
-00005910: 6574 7269 632e 7472 616e 7366 6f72 6d73  etric.transforms
-00005920: 2e50 6164 4966 4e65 6564 6564 2920 2020  .PadIfNeeded)   
-00005930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005940: 7c20 e29c 9320 2020 2020 7c20 e29c 9320  | ...     | ... 
-00005950: 2020 207c 20e2 9c93 2020 2020 2020 7c20     | ...      | 
-00005960: e29c 9320 2020 2020 2020 2020 7c0a 7c20  ...         |.| 
-00005970: 5b50 6572 7370 6563 7469 7665 5d28 6874  [Perspective](ht
-00005980: 7470 733a 2f2f 616c 6275 6d65 6e74 6174  tps://albumentat
-00005990: 696f 6e73 2e61 692f 646f 6373 2f61 7069  ions.ai/docs/api
-000059a0: 5f72 6566 6572 656e 6365 2f61 7567 6d65  _reference/augme
-000059b0: 6e74 6174 696f 6e73 2f67 656f 6d65 7472  ntations/geometr
-000059c0: 6963 2f74 7261 6e73 666f 726d 732f 2361  ic/transforms/#a
-000059d0: 6c62 756d 656e 7461 7469 6f6e 732e 6175  lbumentations.au
-000059e0: 676d 656e 7461 7469 6f6e 732e 6765 6f6d  gmentations.geom
-000059f0: 6574 7269 632e 7472 616e 7366 6f72 6d73  etric.transforms
-00005a00: 2e50 6572 7370 6563 7469 7665 2920 2020  .Perspective)   
-00005a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a20: 7c20 e29c 9320 2020 2020 7c20 e29c 9320  | ...     | ... 
-00005a30: 2020 207c 20e2 9c93 2020 2020 2020 7c20     | ...      | 
-00005a40: e29c 9320 2020 2020 2020 2020 7c0a 7c20  ...         |.| 
-00005a50: 5b50 6965 6365 7769 7365 4166 6669 6e65  [PiecewiseAffine
-00005a60: 5d28 6874 7470 733a 2f2f 616c 6275 6d65  ](https://albume
-00005a70: 6e74 6174 696f 6e73 2e61 692f 646f 6373  ntations.ai/docs
-00005a80: 2f61 7069 5f72 6566 6572 656e 6365 2f61  /api_reference/a
-00005a90: 7567 6d65 6e74 6174 696f 6e73 2f67 656f  ugmentations/geo
-00005aa0: 6d65 7472 6963 2f74 7261 6e73 666f 726d  metric/transform
-00005ab0: 732f 2361 6c62 756d 656e 7461 7469 6f6e  s/#albumentation
-00005ac0: 732e 6175 676d 656e 7461 7469 6f6e 732e  s.augmentations.
-00005ad0: 6765 6f6d 6574 7269 632e 7472 616e 7366  geometric.transf
-00005ae0: 6f72 6d73 2e50 6965 6365 7769 7365 4166  orms.PiecewiseAf
-00005af0: 6669 6e65 2920 2020 2020 2020 2020 2020  fine)           
-00005b00: 7c20 e29c 9320 2020 2020 7c20 e29c 9320  | ...     | ... 
-00005b10: 2020 207c 20e2 9c93 2020 2020 2020 7c20     | ...      | 
-00005b20: e29c 9320 2020 2020 2020 2020 7c0a 7c20  ...         |.| 
-00005b30: 5b50 6978 656c 4472 6f70 6f75 745d 2868  [PixelDropout](h
-00005b40: 7474 7073 3a2f 2f61 6c62 756d 656e 7461  ttps://albumenta
-00005b50: 7469 6f6e 732e 6169 2f64 6f63 732f 6170  tions.ai/docs/ap
-00005b60: 695f 7265 6665 7265 6e63 652f 6175 676d  i_reference/augm
-00005b70: 656e 7461 7469 6f6e 732f 7472 616e 7366  entations/transf
-00005b80: 6f72 6d73 2f23 616c 6275 6d65 6e74 6174  orms/#albumentat
-00005b90: 696f 6e73 2e61 7567 6d65 6e74 6174 696f  ions.augmentatio
-00005ba0: 6e73 2e74 7261 6e73 666f 726d 732e 5069  ns.transforms.Pi
-00005bb0: 7865 6c44 726f 706f 7574 2920 2020 2020  xelDropout)     
-00005bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 616c 6275  : 2.1.Name: albu
+00000020: 6d65 6e74 6174 696f 6e73 0a56 6572 7369  mentations.Versi
+00000030: 6f6e 3a20 312e 342e 330a 5375 6d6d 6172  on: 1.4.3.Summar
+00000040: 793a 2041 6e20 6566 6669 6369 656e 7420  y: An efficient 
+00000050: 6c69 6272 6172 7920 666f 7220 696d 6167  library for imag
+00000060: 6520 6175 676d 656e 7461 7469 6f6e 2c20  e augmentation, 
+00000070: 7072 6f76 6964 696e 6720 6578 7465 6e73  providing extens
+00000080: 6976 6520 7472 616e 7366 6f72 6d61 7469  ive transformati
+00000090: 6f6e 7320 746f 2073 7570 706f 7274 206d  ons to support m
+000000a0: 6163 6869 6e65 206c 6561 726e 696e 6720  achine learning 
+000000b0: 616e 6420 636f 6d70 7574 6572 2076 6973  and computer vis
+000000c0: 696f 6e20 7461 736b 732e 0a48 6f6d 652d  ion tasks..Home-
+000000d0: 7061 6765 3a20 6874 7470 733a 2f2f 616c  page: https://al
+000000e0: 6275 6d65 6e74 6174 696f 6e73 2e61 690a  bumentations.ai.
+000000f0: 4175 7468 6f72 3a20 566c 6164 696d 6972  Author: Vladimir
+00000100: 2049 2e20 4967 6c6f 7669 6b6f 762c 204d   I. Iglovikov, M
+00000110: 696b 6861 696c 2044 7275 7a68 696e 696e  ikhail Druzhinin
+00000120: 2c20 416c 6578 2050 6172 696e 6f76 2c20  , Alex Parinov, 
+00000130: 416c 6578 616e 6465 7220 4275 736c 6165  Alexander Buslae
+00000140: 762c 2045 7567 656e 6520 4b68 7665 6463  v, Eugene Khvedc
+00000150: 6865 6e79 610a 4c69 6365 6e73 653a 204d  henya.License: M
+00000160: 4954 0a4b 6579 776f 7264 733a 2069 6d61  IT.Keywords: ima
+00000170: 6765 2061 7567 6d65 6e74 6174 696f 6e2c  ge augmentation,
+00000180: 6461 7461 2061 7567 6d65 6e74 6174 696f  data augmentatio
+00000190: 6e2c 636f 6d70 7574 6572 2076 6973 696f  n,computer visio
+000001a0: 6e2c 6465 6570 206c 6561 726e 696e 672c  n,deep learning,
+000001b0: 6d61 6368 696e 6520 6c65 6172 6e69 6e67  machine learning
+000001c0: 2c69 6d61 6765 2070 726f 6365 7373 696e  ,image processin
+000001d0: 672c 6172 7469 6669 6369 616c 2069 6e74  g,artificial int
+000001e0: 656c 6c69 6765 6e63 652c 6175 676d 656e  elligence,augmen
+000001f0: 7461 7469 6f6e 206c 6962 7261 7279 2c69  tation library,i
+00000200: 6d61 6765 2074 7261 6e73 666f 726d 6174  mage transformat
+00000210: 696f 6e2c 7669 7369 6f6e 2061 7567 6d65  ion,vision augme
+00000220: 6e74 6174 696f 6e0a 436c 6173 7369 6669  ntation.Classifi
+00000230: 6572 3a20 4465 7665 6c6f 706d 656e 7420  er: Development 
+00000240: 5374 6174 7573 203a 3a20 3520 2d20 5072  Status :: 5 - Pr
+00000250: 6f64 7563 7469 6f6e 2f53 7461 626c 650a  oduction/Stable.
+00000260: 436c 6173 7369 6669 6572 3a20 496e 7465  Classifier: Inte
+00000270: 6e64 6564 2041 7564 6965 6e63 6520 3a3a  nded Audience ::
+00000280: 2044 6576 656c 6f70 6572 730a 436c 6173   Developers.Clas
+00000290: 7369 6669 6572 3a20 496e 7465 6e64 6564  sifier: Intended
+000002a0: 2041 7564 6965 6e63 6520 3a3a 2053 6369   Audience :: Sci
+000002b0: 656e 6365 2f52 6573 6561 7263 680a 436c  ence/Research.Cl
+000002c0: 6173 7369 6669 6572 3a20 4c69 6365 6e73  assifier: Licens
+000002d0: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
+000002e0: 6420 3a3a 204d 4954 204c 6963 656e 7365  d :: MIT License
+000002f0: 0a43 6c61 7373 6966 6965 723a 204f 7065  .Classifier: Ope
+00000300: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
+00000310: 204f 5320 496e 6465 7065 6e64 656e 740a   OS Independent.
+00000320: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+00000330: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000340: 203a 3a20 5079 7468 6f6e 0a43 6c61 7373   :: Python.Class
+00000350: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+00000360: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000370: 7974 686f 6e20 3a3a 2033 0a43 6c61 7373  ython :: 3.Class
+00000380: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+00000390: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+000003a0: 7974 686f 6e20 3a3a 2033 2e38 0a43 6c61  ython :: 3.8.Cla
+000003b0: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+000003c0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+000003d0: 2050 7974 686f 6e20 3a3a 2033 2e39 0a43   Python :: 3.9.C
+000003e0: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
+000003f0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000400: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
+00000410: 300a 436c 6173 7369 6669 6572 3a20 5072  0.Classifier: Pr
+00000420: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000430: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000440: 332e 3131 0a43 6c61 7373 6966 6965 723a  3.11.Classifier:
+00000450: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+00000460: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000470: 3a3a 2033 2e31 320a 436c 6173 7369 6669  :: 3.12.Classifi
+00000480: 6572 3a20 546f 7069 6320 3a3a 2053 6f66  er: Topic :: Sof
+00000490: 7477 6172 6520 4465 7665 6c6f 706d 656e  tware Developmen
+000004a0: 7420 3a3a 204c 6962 7261 7269 6573 0a43  t :: Libraries.C
+000004b0: 6c61 7373 6966 6965 723a 2054 6f70 6963  lassifier: Topic
+000004c0: 203a 3a20 536f 6674 7761 7265 2044 6576   :: Software Dev
+000004d0: 656c 6f70 6d65 6e74 203a 3a20 4c69 6272  elopment :: Libr
+000004e0: 6172 6965 7320 3a3a 2050 7974 686f 6e20  aries :: Python 
+000004f0: 4d6f 6475 6c65 730a 436c 6173 7369 6669  Modules.Classifi
+00000500: 6572 3a20 546f 7069 6320 3a3a 2053 6369  er: Topic :: Sci
+00000510: 656e 7469 6669 632f 456e 6769 6e65 6572  entific/Engineer
+00000520: 696e 6720 3a3a 2041 7274 6966 6963 6961  ing :: Artificia
+00000530: 6c20 496e 7465 6c6c 6967 656e 6365 0a43  l Intelligence.C
+00000540: 6c61 7373 6966 6965 723a 2054 6f70 6963  lassifier: Topic
+00000550: 203a 3a20 5363 6965 6e74 6966 6963 2f45   :: Scientific/E
+00000560: 6e67 696e 6565 7269 6e67 203a 3a20 496d  ngineering :: Im
+00000570: 6167 6520 5072 6f63 6573 7369 6e67 0a43  age Processing.C
+00000580: 6c61 7373 6966 6965 723a 2054 7970 696e  lassifier: Typin
+00000590: 6720 3a3a 2054 7970 6564 0a52 6571 7569  g :: Typed.Requi
+000005a0: 7265 732d 5079 7468 6f6e 3a20 3e3d 332e  res-Python: >=3.
+000005b0: 380a 4465 7363 7269 7074 696f 6e2d 436f  8.Description-Co
+000005c0: 6e74 656e 742d 5479 7065 3a20 7465 7874  ntent-Type: text
+000005d0: 2f6d 6172 6b64 6f77 6e0a 4c69 6365 6e73  /markdown.Licens
+000005e0: 652d 4669 6c65 3a20 4c49 4345 4e53 450a  e-File: LICENSE.
+000005f0: 5265 7175 6972 6573 2d44 6973 743a 206e  Requires-Dist: n
+00000600: 756d 7079 3e3d 312e 3234 2e34 0a52 6571  umpy>=1.24.4.Req
+00000610: 7569 7265 732d 4469 7374 3a20 7363 6970  uires-Dist: scip
+00000620: 793e 3d31 2e31 302e 300a 5265 7175 6972  y>=1.10.0.Requir
+00000630: 6573 2d44 6973 743a 2073 6369 6b69 742d  es-Dist: scikit-
+00000640: 696d 6167 653e 3d30 2e32 312e 300a 5265  image>=0.21.0.Re
+00000650: 7175 6972 6573 2d44 6973 743a 2050 7959  quires-Dist: PyY
+00000660: 414d 4c0a 5265 7175 6972 6573 2d44 6973  AML.Requires-Dis
+00000670: 743a 2074 7970 696e 672d 6578 7465 6e73  t: typing-extens
+00000680: 696f 6e73 3e3d 342e 392e 300a 5265 7175  ions>=4.9.0.Requ
+00000690: 6972 6573 2d44 6973 743a 2073 6369 6b69  ires-Dist: sciki
+000006a0: 742d 6c65 6172 6e3e 3d31 2e33 2e32 0a52  t-learn>=1.3.2.R
+000006b0: 6571 7569 7265 732d 4469 7374 3a20 6f70  equires-Dist: op
+000006c0: 656e 6376 2d70 7974 686f 6e2d 6865 6164  encv-python-head
+000006d0: 6c65 7373 3e3d 342e 392e 300a 0a23 2041  less>=4.9.0..# A
+000006e0: 6c62 756d 656e 7461 7469 6f6e 730a 0a5b  lbumentations..[
+000006f0: 215b 5079 5049 2076 6572 7369 6f6e 5d28  ![PyPI version](
+00000700: 6874 7470 733a 2f2f 6261 6467 652e 6675  https://badge.fu
+00000710: 7279 2e69 6f2f 7079 2f61 6c62 756d 656e  ry.io/py/albumen
+00000720: 7461 7469 6f6e 732e 7376 6729 5d28 6874  tations.svg)](ht
+00000730: 7470 733a 2f2f 6261 6467 652e 6675 7279  tps://badge.fury
+00000740: 2e69 6f2f 7079 2f61 6c62 756d 656e 7461  .io/py/albumenta
+00000750: 7469 6f6e 7329 0a21 5b43 495d 2868 7474  tions).![CI](htt
+00000760: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000770: 616c 6275 6d65 6e74 6174 696f 6e73 2d74  albumentations-t
+00000780: 6561 6d2f 616c 6275 6d65 6e74 6174 696f  eam/albumentatio
+00000790: 6e73 2f77 6f72 6b66 6c6f 7773 2f43 492f  ns/workflows/CI/
+000007a0: 6261 6467 652e 7376 6729 0a5b 215b 4c69  badge.svg).[![Li
+000007b0: 6365 6e73 653a 204d 4954 5d28 6874 7470  cense: MIT](http
+000007c0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+000007d0: 696f 2f62 6164 6765 2f4c 6963 656e 7365  io/badge/License
+000007e0: 2d4d 4954 2d62 7269 6768 7467 7265 656e  -MIT-brightgreen
+000007f0: 2e73 7667 295d 2868 7474 7073 3a2f 2f6f  .svg)](https://o
+00000800: 7065 6e73 6f75 7263 652e 6f72 672f 6c69  pensource.org/li
+00000810: 6365 6e73 6573 2f4d 4954 290a 5b21 5b52  censes/MIT).[![R
+00000820: 7566 665d 2868 7474 7073 3a2f 2f69 6d67  uff](https://img
+00000830: 2e73 6869 656c 6473 2e69 6f2f 656e 6470  .shields.io/endp
+00000840: 6f69 6e74 3f75 726c 3d68 7474 7073 3a2f  oint?url=https:/
+00000850: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
+00000860: 6f6e 7465 6e74 2e63 6f6d 2f61 7374 7261  ontent.com/astra
+00000870: 6c2d 7368 2f72 7566 662f 6d61 696e 2f61  l-sh/ruff/main/a
+00000880: 7373 6574 732f 6261 6467 652f 7632 2e6a  ssets/badge/v2.j
+00000890: 736f 6e29 5d28 6874 7470 733a 2f2f 6769  son)](https://gi
+000008a0: 7468 7562 2e63 6f6d 2f61 7374 7261 6c2d  thub.com/astral-
+000008b0: 7368 2f72 7566 6629 0a0a 5b44 6f63 735d  sh/ruff)..[Docs]
+000008c0: 2868 7474 7073 3a2f 2f61 6c62 756d 656e  (https://albumen
+000008d0: 7461 7469 6f6e 732e 6169 2f64 6f63 732f  tations.ai/docs/
+000008e0: 2920 7c20 5b44 6973 636f 7264 5d28 6874  ) | [Discord](ht
+000008f0: 7470 733a 2f2f 6469 7363 6f72 642e 6767  tps://discord.gg
+00000900: 2f41 4b50 7272 4459 4e41 7429 207c 205b  /AKPrrDYNAt) | [
+00000910: 5477 6974 7465 725d 2868 7474 7073 3a2f  Twitter](https:/
+00000920: 2f74 7769 7474 6572 2e63 6f6d 2f61 6c62  /twitter.com/alb
+00000930: 756d 656e 7461 7469 6f6e 7329 207c 205b  umentations) | [
+00000940: 4c69 6e6b 6564 496e 5d28 6874 7470 733a  LinkedIn](https:
+00000950: 2f2f 7777 772e 6c69 6e6b 6564 696e 2e63  //www.linkedin.c
+00000960: 6f6d 2f63 6f6d 7061 6e79 2f31 3030 3530  om/company/10050
+00000970: 3434 3735 2f29 0a0a 416c 6275 6d65 6e74  4475/)..Albument
+00000980: 6174 696f 6e73 2069 7320 6120 5079 7468  ations is a Pyth
+00000990: 6f6e 206c 6962 7261 7279 2066 6f72 2069  on library for i
+000009a0: 6d61 6765 2061 7567 6d65 6e74 6174 696f  mage augmentatio
+000009b0: 6e2e 2049 6d61 6765 2061 7567 6d65 6e74  n. Image augment
+000009c0: 6174 696f 6e20 6973 2075 7365 6420 696e  ation is used in
+000009d0: 2064 6565 7020 6c65 6172 6e69 6e67 2061   deep learning a
+000009e0: 6e64 2063 6f6d 7075 7465 7220 7669 7369  nd computer visi
+000009f0: 6f6e 2074 6173 6b73 2074 6f20 696e 6372  on tasks to incr
+00000a00: 6561 7365 2074 6865 2071 7561 6c69 7479  ease the quality
+00000a10: 206f 6620 7472 6169 6e65 6420 6d6f 6465   of trained mode
+00000a20: 6c73 2e20 5468 6520 7075 7270 6f73 6520  ls. The purpose 
+00000a30: 6f66 2069 6d61 6765 2061 7567 6d65 6e74  of image augment
+00000a40: 6174 696f 6e20 6973 2074 6f20 6372 6561  ation is to crea
+00000a50: 7465 206e 6577 2074 7261 696e 696e 6720  te new training 
+00000a60: 7361 6d70 6c65 7320 6672 6f6d 2074 6865  samples from the
+00000a70: 2065 7869 7374 696e 6720 6461 7461 2e0a   existing data..
+00000a80: 0a48 6572 6520 6973 2061 6e20 6578 616d  .Here is an exam
+00000a90: 706c 6520 6f66 2068 6f77 2079 6f75 2063  ple of how you c
+00000aa0: 616e 2061 7070 6c79 2073 6f6d 6520 5b70  an apply some [p
+00000ab0: 6978 656c 2d6c 6576 656c 5d28 2370 6978  ixel-level](#pix
+00000ac0: 656c 2d6c 6576 656c 2d74 7261 6e73 666f  el-level-transfo
+00000ad0: 726d 7329 2061 7567 6d65 6e74 6174 696f  rms) augmentatio
+00000ae0: 6e73 2066 726f 6d20 416c 6275 6d65 6e74  ns from Albument
+00000af0: 6174 696f 6e73 2074 6f20 6372 6561 7465  ations to create
+00000b00: 206e 6577 2069 6d61 6765 7320 6672 6f6d   new images from
+00000b10: 2074 6865 206f 7269 6769 6e61 6c20 6f6e   the original on
+00000b20: 653a 0a21 5b70 6172 726f 745d 2868 7474  e:.![parrot](htt
+00000b30: 7073 3a2f 2f68 6162 7261 7374 6f72 6167  ps://habrastorag
+00000b40: 652e 6f72 672f 7765 6274 2f62 642f 6e65  e.org/webt/bd/ne
+00000b50: 2f72 762f 6264 6e65 7276 3563 746b 7564  /rv/bdnerv5ctkud
+00000b60: 6d73 617a 6e68 7734 6372 7364 6669 772e  msaznhw4crsdfiw.
+00000b70: 6a70 6567 290a 0a23 2320 5768 7920 416c  jpeg)..## Why Al
+00000b80: 6275 6d65 6e74 6174 696f 6e73 0a0a 2d20  bumentations..- 
+00000b90: 416c 6275 6d65 6e74 6174 696f 6e73 202a  Albumentations *
+00000ba0: 2a5b 7375 7070 6f72 7473 2061 6c6c 2063  *[supports all c
+00000bb0: 6f6d 6d6f 6e20 636f 6d70 7574 6572 2076  ommon computer v
+00000bc0: 6973 696f 6e20 7461 736b 735d 2823 692d  ision tasks](#i-
+00000bd0: 7761 6e74 2d74 6f2d 7573 652d 616c 6275  want-to-use-albu
+00000be0: 6d65 6e74 6174 696f 6e73 2d66 6f72 2d74  mentations-for-t
+00000bf0: 6865 2d73 7065 6369 6669 632d 7461 736b  he-specific-task
+00000c00: 2d73 7563 682d 6173 2d63 6c61 7373 6966  -such-as-classif
+00000c10: 6963 6174 696f 6e2d 6f72 2d73 6567 6d65  ication-or-segme
+00000c20: 6e74 6174 696f 6e29 2a2a 2073 7563 6820  ntation)** such 
+00000c30: 6173 2063 6c61 7373 6966 6963 6174 696f  as classificatio
+00000c40: 6e2c 2073 656d 616e 7469 6320 7365 676d  n, semantic segm
+00000c50: 656e 7461 7469 6f6e 2c20 696e 7374 616e  entation, instan
+00000c60: 6365 2073 6567 6d65 6e74 6174 696f 6e2c  ce segmentation,
+00000c70: 206f 626a 6563 7420 6465 7465 6374 696f   object detectio
+00000c80: 6e2c 2061 6e64 2070 6f73 6520 6573 7469  n, and pose esti
+00000c90: 6d61 7469 6f6e 2e0a 2d20 5468 6520 6c69  mation..- The li
+00000ca0: 6272 6172 7920 7072 6f76 6964 6573 202a  brary provides *
+00000cb0: 2a5b 6120 7369 6d70 6c65 2075 6e69 6669  *[a simple unifi
+00000cc0: 6564 2041 5049 5d28 2361 2d73 696d 706c  ed API](#a-simpl
+00000cd0: 652d 6578 616d 706c 6529 2a2a 2074 6f20  e-example)** to 
+00000ce0: 776f 726b 2077 6974 6820 616c 6c20 6461  work with all da
+00000cf0: 7461 2074 7970 6573 3a20 696d 6167 6573  ta types: images
+00000d00: 2028 5242 472d 696d 6167 6573 2c20 6772   (RBG-images, gr
+00000d10: 6179 7363 616c 6520 696d 6167 6573 2c20  ayscale images, 
+00000d20: 6d75 6c74 6973 7065 6374 7261 6c20 696d  multispectral im
+00000d30: 6167 6573 292c 2073 6567 6d65 6e74 6174  ages), segmentat
+00000d40: 696f 6e20 6d61 736b 732c 2062 6f75 6e64  ion masks, bound
+00000d50: 696e 6720 626f 7865 732c 2061 6e64 206b  ing boxes, and k
+00000d60: 6579 706f 696e 7473 2e0a 2d20 5468 6520  eypoints..- The 
+00000d70: 6c69 6272 6172 7920 636f 6e74 6169 6e73  library contains
+00000d80: 202a 2a5b 6d6f 7265 2074 6861 6e20 3730   **[more than 70
+00000d90: 2064 6966 6665 7265 6e74 2061 7567 6d65   different augme
+00000da0: 6e74 6174 696f 6e73 5d28 236c 6973 742d  ntations](#list-
+00000db0: 6f66 2d61 7567 6d65 6e74 6174 696f 6e73  of-augmentations
+00000dc0: 292a 2a20 746f 2067 656e 6572 6174 6520  )** to generate 
+00000dd0: 6e65 7720 7472 6169 6e69 6e67 2073 616d  new training sam
+00000de0: 706c 6573 2066 726f 6d20 7468 6520 6578  ples from the ex
+00000df0: 6973 7469 6e67 2064 6174 612e 0a2d 2041  isting data..- A
+00000e00: 6c62 756d 656e 7461 7469 6f6e 7320 6973  lbumentations is
+00000e10: 205b 2a2a 6661 7374 2a2a 5d28 2362 656e   [**fast**](#ben
+00000e20: 6368 6d61 726b 696e 672d 7265 7375 6c74  chmarking-result
+00000e30: 7329 2e20 5765 2062 656e 6368 6d61 726b  s). We benchmark
+00000e40: 2065 6163 6820 6e65 7720 7265 6c65 6173   each new releas
+00000e50: 6520 746f 2065 6e73 7572 6520 7468 6174  e to ensure that
+00000e60: 2061 7567 6d65 6e74 6174 696f 6e73 2070   augmentations p
+00000e70: 726f 7669 6465 206d 6178 696d 756d 2073  rovide maximum s
+00000e80: 7065 6564 2e0a 2d20 4974 202a 2a5b 776f  peed..- It **[wo
+00000e90: 726b 7320 7769 7468 2070 6f70 756c 6172  rks with popular
+00000ea0: 2064 6565 7020 6c65 6172 6e69 6e67 2066   deep learning f
+00000eb0: 7261 6d65 776f 726b 735d 2823 692d 7761  rameworks](#i-wa
+00000ec0: 6e74 2d74 6f2d 6b6e 6f77 2d68 6f77 2d74  nt-to-know-how-t
+00000ed0: 6f2d 7573 652d 616c 6275 6d65 6e74 6174  o-use-albumentat
+00000ee0: 696f 6e73 2d77 6974 682d 6465 6570 2d6c  ions-with-deep-l
+00000ef0: 6561 726e 696e 672d 6672 616d 6577 6f72  earning-framewor
+00000f00: 6b73 292a 2a20 7375 6368 2061 7320 5079  ks)** such as Py
+00000f10: 546f 7263 6820 616e 6420 5465 6e73 6f72  Torch and Tensor
+00000f20: 466c 6f77 2e20 4279 2074 6865 2077 6179  Flow. By the way
+00000f30: 2c20 416c 6275 6d65 6e74 6174 696f 6e73  , Albumentations
+00000f40: 2069 7320 6120 7061 7274 206f 6620 7468   is a part of th
+00000f50: 6520 5b50 7954 6f72 6368 2065 636f 7379  e [PyTorch ecosy
+00000f60: 7374 656d 5d28 6874 7470 733a 2f2f 7079  stem](https://py
+00000f70: 746f 7263 682e 6f72 672f 6563 6f73 7973  torch.org/ecosys
+00000f80: 7465 6d2f 292e 0a2d 205b 2a2a 5772 6974  tem/)..- [**Writ
+00000f90: 7465 6e20 6279 2065 7870 6572 7473 2a2a  ten by experts**
+00000fa0: 5d28 2361 7574 686f 7273 292e 2054 6865  ](#authors). The
+00000fb0: 2061 7574 686f 7273 2068 6176 6520 6578   authors have ex
+00000fc0: 7065 7269 656e 6365 2062 6f74 6820 776f  perience both wo
+00000fd0: 726b 696e 6720 6f6e 2070 726f 6475 6374  rking on product
+00000fe0: 696f 6e20 636f 6d70 7574 6572 2076 6973  ion computer vis
+00000ff0: 696f 6e20 7379 7374 656d 7320 616e 6420  ion systems and 
+00001000: 7061 7274 6963 6970 6174 696e 6720 696e  participating in
+00001010: 2063 6f6d 7065 7469 7469 7665 206d 6163   competitive mac
+00001020: 6869 6e65 206c 6561 726e 696e 672e 204d  hine learning. M
+00001030: 616e 7920 636f 7265 2074 6561 6d20 6d65  any core team me
+00001040: 6d62 6572 7320 6172 6520 4b61 6767 6c65  mbers are Kaggle
+00001050: 204d 6173 7465 7273 2061 6e64 2047 7261   Masters and Gra
+00001060: 6e64 6d61 7374 6572 732e 0a2d 2054 6865  ndmasters..- The
+00001070: 206c 6962 7261 7279 2069 7320 5b2a 2a77   library is [**w
+00001080: 6964 656c 7920 7573 6564 2a2a 5d28 2377  idely used**](#w
+00001090: 686f 2d69 732d 7573 696e 672d 616c 6275  ho-is-using-albu
+000010a0: 6d65 6e74 6174 696f 6e73 2920 696e 2069  mentations) in i
+000010b0: 6e64 7573 7472 792c 2064 6565 7020 6c65  ndustry, deep le
+000010c0: 6172 6e69 6e67 2072 6573 6561 7263 682c  arning research,
+000010d0: 206d 6163 6869 6e65 206c 6561 726e 696e   machine learnin
+000010e0: 6720 636f 6d70 6574 6974 696f 6e73 2c20  g competitions, 
+000010f0: 616e 6420 6f70 656e 2073 6f75 7263 6520  and open source 
+00001100: 7072 6f6a 6563 7473 2e0a 0a23 2320 5370  projects...## Sp
+00001110: 6f6e 736f 7273 0a0a 3c61 2068 7265 663d  onsors..<a href=
+00001120: 2268 7474 7073 3a2f 2f72 6f62 6f66 6c6f  "https://roboflo
+00001130: 772e 636f 6d2f 2220 7461 7267 6574 3d22  w.com/" target="
+00001140: 5f62 6c61 6e6b 223e 3c69 6d67 2073 7263  _blank"><img src
+00001150: 3d22 6874 7470 733a 2f2f 6176 6174 6172  ="https://avatar
+00001160: 732e 6769 7468 7562 7573 6572 636f 6e74  s.githubusercont
+00001170: 656e 742e 636f 6d2f 752f 3533 3130 3431  ent.com/u/531041
+00001180: 3138 3f73 3d32 3030 2676 3d34 2220 7769  18?s=200&v=4" wi
+00001190: 6474 683d 2231 3030 222f 3e3c 2f61 3e0a  dth="100"/></a>.
+000011a0: 0a23 2320 5461 626c 6520 6f66 2063 6f6e  .## Table of con
+000011b0: 7465 6e74 730a 0a2d 205b 416c 6275 6d65  tents..- [Albume
+000011c0: 6e74 6174 696f 6e73 5d28 2361 6c62 756d  ntations](#album
+000011d0: 656e 7461 7469 6f6e 7329 0a20 202d 205b  entations).  - [
+000011e0: 5768 7920 416c 6275 6d65 6e74 6174 696f  Why Albumentatio
+000011f0: 6e73 5d28 2377 6879 2d61 6c62 756d 656e  ns](#why-albumen
+00001200: 7461 7469 6f6e 7329 0a20 202d 205b 5370  tations).  - [Sp
+00001210: 6f6e 736f 7273 5d28 2373 706f 6e73 6f72  onsors](#sponsor
+00001220: 7329 0a20 202d 205b 5461 626c 6520 6f66  s).  - [Table of
+00001230: 2063 6f6e 7465 6e74 735d 2823 7461 626c   contents](#tabl
+00001240: 652d 6f66 2d63 6f6e 7465 6e74 7329 0a20  e-of-contents). 
+00001250: 202d 205b 4175 7468 6f72 735d 2823 6175   - [Authors](#au
+00001260: 7468 6f72 7329 0a20 202d 205b 496e 7374  thors).  - [Inst
+00001270: 616c 6c61 7469 6f6e 5d28 2369 6e73 7461  allation](#insta
+00001280: 6c6c 6174 696f 6e29 0a20 202d 205b 446f  llation).  - [Do
+00001290: 6375 6d65 6e74 6174 696f 6e5d 2823 646f  cumentation](#do
+000012a0: 6375 6d65 6e74 6174 696f 6e29 0a20 202d  cumentation).  -
+000012b0: 205b 4120 7369 6d70 6c65 2065 7861 6d70   [A simple examp
+000012c0: 6c65 5d28 2361 2d73 696d 706c 652d 6578  le](#a-simple-ex
+000012d0: 616d 706c 6529 0a20 202d 205b 4765 7474  ample).  - [Gett
+000012e0: 696e 6720 7374 6172 7465 645d 2823 6765  ing started](#ge
+000012f0: 7474 696e 672d 7374 6172 7465 6429 0a20  tting-started). 
+00001300: 2020 202d 205b 4920 616d 206e 6577 2074     - [I am new t
+00001310: 6f20 696d 6167 6520 6175 676d 656e 7461  o image augmenta
+00001320: 7469 6f6e 5d28 2369 2d61 6d2d 6e65 772d  tion](#i-am-new-
+00001330: 746f 2d69 6d61 6765 2d61 7567 6d65 6e74  to-image-augment
+00001340: 6174 696f 6e29 0a20 2020 202d 205b 4920  ation).    - [I 
+00001350: 7761 6e74 2074 6f20 7573 6520 416c 6275  want to use Albu
+00001360: 6d65 6e74 6174 696f 6e73 2066 6f72 2074  mentations for t
+00001370: 6865 2073 7065 6369 6669 6320 7461 736b  he specific task
+00001380: 2073 7563 6820 6173 2063 6c61 7373 6966   such as classif
+00001390: 6963 6174 696f 6e20 6f72 2073 6567 6d65  ication or segme
+000013a0: 6e74 6174 696f 6e5d 2823 692d 7761 6e74  ntation](#i-want
+000013b0: 2d74 6f2d 7573 652d 616c 6275 6d65 6e74  -to-use-albument
+000013c0: 6174 696f 6e73 2d66 6f72 2d74 6865 2d73  ations-for-the-s
+000013d0: 7065 6369 6669 632d 7461 736b 2d73 7563  pecific-task-suc
+000013e0: 682d 6173 2d63 6c61 7373 6966 6963 6174  h-as-classificat
+000013f0: 696f 6e2d 6f72 2d73 6567 6d65 6e74 6174  ion-or-segmentat
+00001400: 696f 6e29 0a20 2020 202d 205b 4920 7761  ion).    - [I wa
+00001410: 6e74 2074 6f20 6b6e 6f77 2068 6f77 2074  nt to know how t
+00001420: 6f20 7573 6520 416c 6275 6d65 6e74 6174  o use Albumentat
+00001430: 696f 6e73 2077 6974 6820 6465 6570 206c  ions with deep l
+00001440: 6561 726e 696e 6720 6672 616d 6577 6f72  earning framewor
+00001450: 6b73 5d28 2369 2d77 616e 742d 746f 2d6b  ks](#i-want-to-k
+00001460: 6e6f 772d 686f 772d 746f 2d75 7365 2d61  now-how-to-use-a
+00001470: 6c62 756d 656e 7461 7469 6f6e 732d 7769  lbumentations-wi
+00001480: 7468 2d64 6565 702d 6c65 6172 6e69 6e67  th-deep-learning
+00001490: 2d66 7261 6d65 776f 726b 7329 0a20 2020  -frameworks).   
+000014a0: 202d 205b 4920 7761 6e74 2074 6f20 6578   - [I want to ex
+000014b0: 706c 6f72 6520 6175 676d 656e 7461 7469  plore augmentati
+000014c0: 6f6e 7320 616e 6420 7365 6520 416c 6275  ons and see Albu
+000014d0: 6d65 6e74 6174 696f 6e73 2069 6e20 6163  mentations in ac
+000014e0: 7469 6f6e 5d28 2369 2d77 616e 742d 746f  tion](#i-want-to
+000014f0: 2d65 7870 6c6f 7265 2d61 7567 6d65 6e74  -explore-augment
+00001500: 6174 696f 6e73 2d61 6e64 2d73 6565 2d61  ations-and-see-a
+00001510: 6c62 756d 656e 7461 7469 6f6e 732d 696e  lbumentations-in
+00001520: 2d61 6374 696f 6e29 0a20 202d 205b 5768  -action).  - [Wh
+00001530: 6f20 6973 2075 7369 6e67 2041 6c62 756d  o is using Album
+00001540: 656e 7461 7469 6f6e 735d 2823 7768 6f2d  entations](#who-
+00001550: 6973 2d75 7369 6e67 2d61 6c62 756d 656e  is-using-albumen
+00001560: 7461 7469 6f6e 7329 0a20 2020 202d 205b  tations).    - [
+00001570: 5365 6520 616c 736f 5d28 2373 6565 2d61  See also](#see-a
+00001580: 6c73 6f29 0a20 202d 205b 4c69 7374 206f  lso).  - [List o
+00001590: 6620 6175 676d 656e 7461 7469 6f6e 735d  f augmentations]
+000015a0: 2823 6c69 7374 2d6f 662d 6175 676d 656e  (#list-of-augmen
+000015b0: 7461 7469 6f6e 7329 0a20 2020 202d 205b  tations).    - [
+000015c0: 5069 7865 6c2d 6c65 7665 6c20 7472 616e  Pixel-level tran
+000015d0: 7366 6f72 6d73 5d28 2370 6978 656c 2d6c  sforms](#pixel-l
+000015e0: 6576 656c 2d74 7261 6e73 666f 726d 7329  evel-transforms)
+000015f0: 0a20 2020 202d 205b 5370 6174 6961 6c2d  .    - [Spatial-
+00001600: 6c65 7665 6c20 7472 616e 7366 6f72 6d73  level transforms
+00001610: 5d28 2373 7061 7469 616c 2d6c 6576 656c  ](#spatial-level
+00001620: 2d74 7261 6e73 666f 726d 7329 0a20 2020  -transforms).   
+00001630: 202d 205b 4d69 7869 6e67 2d6c 6576 656c   - [Mixing-level
+00001640: 2074 7261 6e73 666f 726d 735d 2823 6d69   transforms](#mi
+00001650: 7869 6e67 2d6c 6576 656c 2d74 7261 6e73  xing-level-trans
+00001660: 666f 726d 7329 0a20 202d 205b 4120 6665  forms).  - [A fe
+00001670: 7720 6d6f 7265 2065 7861 6d70 6c65 7320  w more examples 
+00001680: 6f66 202a 2a61 7567 6d65 6e74 6174 696f  of **augmentatio
+00001690: 6e73 2a2a 5d28 2361 2d66 6577 2d6d 6f72  ns**](#a-few-mor
+000016a0: 652d 6578 616d 706c 6573 2d6f 662d 6175  e-examples-of-au
+000016b0: 676d 656e 7461 7469 6f6e 7329 0a20 2020  gmentations).   
+000016c0: 202d 205b 5365 6d61 6e74 6963 2073 6567   - [Semantic seg
+000016d0: 6d65 6e74 6174 696f 6e20 6f6e 2074 6865  mentation on the
+000016e0: 2049 6e72 6961 2064 6174 6173 6574 5d28   Inria dataset](
+000016f0: 2373 656d 616e 7469 632d 7365 676d 656e  #semantic-segmen
+00001700: 7461 7469 6f6e 2d6f 6e2d 7468 652d 696e  tation-on-the-in
+00001710: 7269 612d 6461 7461 7365 7429 0a20 2020  ria-dataset).   
+00001720: 202d 205b 4d65 6469 6361 6c20 696d 6167   - [Medical imag
+00001730: 696e 675d 2823 6d65 6469 6361 6c2d 696d  ing](#medical-im
+00001740: 6167 696e 6729 0a20 2020 202d 205b 4f62  aging).    - [Ob
+00001750: 6a65 6374 2064 6574 6563 7469 6f6e 2061  ject detection a
+00001760: 6e64 2073 656d 616e 7469 6320 7365 676d  nd semantic segm
+00001770: 656e 7461 7469 6f6e 206f 6e20 7468 6520  entation on the 
+00001780: 4d61 7069 6c6c 6172 7920 5669 7374 6173  Mapillary Vistas
+00001790: 2064 6174 6173 6574 5d28 236f 626a 6563   dataset](#objec
+000017a0: 742d 6465 7465 6374 696f 6e2d 616e 642d  t-detection-and-
+000017b0: 7365 6d61 6e74 6963 2d73 6567 6d65 6e74  semantic-segment
+000017c0: 6174 696f 6e2d 6f6e 2d74 6865 2d6d 6170  ation-on-the-map
+000017d0: 696c 6c61 7279 2d76 6973 7461 732d 6461  illary-vistas-da
+000017e0: 7461 7365 7429 0a20 2020 202d 205b 4b65  taset).    - [Ke
+000017f0: 7970 6f69 6e74 7320 6175 676d 656e 7461  ypoints augmenta
+00001800: 7469 6f6e 5d28 236b 6579 706f 696e 7473  tion](#keypoints
+00001810: 2d61 7567 6d65 6e74 6174 696f 6e29 0a20  -augmentation). 
+00001820: 202d 205b 4265 6e63 686d 6172 6b69 6e67   - [Benchmarking
+00001830: 2072 6573 756c 7473 5d28 2362 656e 6368   results](#bench
+00001840: 6d61 726b 696e 672d 7265 7375 6c74 7329  marking-results)
+00001850: 0a20 202d 205b 436f 6e74 7269 6275 7469  .  - [Contributi
+00001860: 6e67 5d28 2363 6f6e 7472 6962 7574 696e  ng](#contributin
+00001870: 6729 0a20 202d 205b 436f 6d6d 756e 6974  g).  - [Communit
+00001880: 7920 616e 6420 5375 7070 6f72 745d 2823  y and Support](#
+00001890: 636f 6d6d 756e 6974 792d 616e 642d 7375  community-and-su
+000018a0: 7070 6f72 7429 0a20 202d 205b 436f 6d6d  pport).  - [Comm
+000018b0: 656e 7473 5d28 2363 6f6d 6d65 6e74 7329  ents](#comments)
+000018c0: 0a20 202d 205b 4369 7469 6e67 5d28 2363  .  - [Citing](#c
+000018d0: 6974 696e 6729 0a0a 2323 2041 7574 686f  iting)..## Autho
+000018e0: 7273 0a0a 5b2a 2a56 6c61 6469 6d69 7220  rs..[**Vladimir 
+000018f0: 492e 2049 676c 6f76 696b 6f76 2a2a 5d28  I. Iglovikov**](
+00001900: 6874 7470 733a 2f2f 7777 772e 6c69 6e6b  https://www.link
+00001910: 6564 696e 2e63 6f6d 2f69 6e2f 6967 6c6f  edin.com/in/iglo
+00001920: 7669 6b6f 762f 2920 7c20 5b4b 6167 676c  vikov/) | [Kaggl
+00001930: 6520 4772 616e 646d 6173 7465 725d 2868  e Grandmaster](h
+00001940: 7474 7073 3a2f 2f77 7777 2e6b 6167 676c  ttps://www.kaggl
+00001950: 652e 636f 6d2f 6967 6c6f 7669 6b6f 7629  e.com/iglovikov)
+00001960: 0a0a 5b2a 2a4d 696b 6861 696c 2044 7275  ..[**Mikhail Dru
+00001970: 7a68 696e 696e 2a2a 5d28 6874 7470 733a  zhinin**](https:
+00001980: 2f2f 7777 772e 6c69 6e6b 6564 696e 2e63  //www.linkedin.c
+00001990: 6f6d 2f69 6e2f 6d69 6b68 6169 6c2d 6472  om/in/mikhail-dr
+000019a0: 757a 6869 6e69 6e2d 3534 3832 3239 3130  uzhinin-54822910
+000019b0: 302f 2920 7c20 5b4b 6167 676c 6520 4578  0/) | [Kaggle Ex
+000019c0: 7065 7274 5d28 6874 7470 733a 2f2f 7777  pert](https://ww
+000019d0: 772e 6b61 6767 6c65 2e63 6f6d 2f64 6970  w.kaggle.com/dip
+000019e0: 6574 6d29 0a0a 5b2a 2a41 6c65 7820 5061  etm)..[**Alex Pa
+000019f0: 7269 6e6f 762a 2a5d 2868 7474 7073 3a2f  rinov**](https:/
+00001a00: 2f77 7777 2e6c 696e 6b65 6469 6e2e 636f  /www.linkedin.co
+00001a10: 6d2f 696e 2f61 6c65 782d 7061 7269 6e6f  m/in/alex-parino
+00001a20: 762f 2920 7c20 5b4b 6167 676c 6520 4d61  v/) | [Kaggle Ma
+00001a30: 7374 6572 5d28 6874 7470 733a 2f2f 7777  ster](https://ww
+00001a40: 772e 6b61 6767 6c65 2e63 6f6d 2f63 7265  w.kaggle.com/cre
+00001a50: 6166 7a29 0a0a 5b2a 2a41 6c65 7861 6e64  afz)..[**Alexand
+00001a60: 6572 2042 7573 6c61 6576 2a2a 20e2 8094  er Buslaev** ...
+00001a70: 2043 6f6d 7075 7465 7220 5669 7369 6f6e   Computer Vision
+00001a80: 2045 6e67 696e 6565 7220 6174 204d 6170   Engineer at Map
+00001a90: 626f 785d 2868 7474 7073 3a2f 2f77 7777  box](https://www
+00001aa0: 2e6c 696e 6b65 6469 6e2e 636f 6d2f 696e  .linkedin.com/in
+00001ab0: 2f61 6c2d 6275 736c 6165 762f 2920 7c20  /al-buslaev/) | 
+00001ac0: 5b4b 6167 676c 6520 4d61 7374 6572 5d28  [Kaggle Master](
+00001ad0: 6874 7470 733a 2f2f 7777 772e 6b61 6767  https://www.kagg
+00001ae0: 6c65 2e63 6f6d 2f61 6c62 7573 6c61 6576  le.com/albuslaev
+00001af0: 290a 0a5b 2a2a 4576 6567 656e 6520 4b68  )..[**Evegene Kh
+00001b00: 7665 6463 6865 6e79 612a 2a20 e280 9420  vedchenya** ... 
+00001b10: 436f 6d70 7574 6572 2056 6973 696f 6e20  Computer Vision 
+00001b20: 5265 7365 6172 6368 2045 6e67 696e 6565  Research Enginee
+00001b30: 7220 6174 2050 69c3 b161 7461 2046 6172  r at Pi..ata Far
+00001b40: 6d73 5d28 6874 7470 733a 2f2f 7777 772e  ms](https://www.
+00001b50: 6c69 6e6b 6564 696e 2e63 6f6d 2f69 6e2f  linkedin.com/in/
+00001b60: 6376 7461 6c6b 732f 2920 7c20 5b4b 6167  cvtalks/) | [Kag
+00001b70: 676c 6520 4772 616e 646d 6173 7465 725d  gle Grandmaster]
+00001b80: 2868 7474 7073 3a2f 2f77 7777 2e6b 6167  (https://www.kag
+00001b90: 676c 652e 636f 6d2f 626c 6f6f 6461 7865  gle.com/bloodaxe
+00001ba0: 290a 0a23 2320 496e 7374 616c 6c61 7469  )..## Installati
+00001bb0: 6f6e 0a0a 416c 6275 6d65 6e74 6174 696f  on..Albumentatio
+00001bc0: 6e73 2072 6571 7569 7265 7320 5079 7468  ns requires Pyth
+00001bd0: 6f6e 2033 2e38 206f 7220 6869 6768 6572  on 3.8 or higher
+00001be0: 2e20 546f 2069 6e73 7461 6c6c 2074 6865  . To install the
+00001bf0: 206c 6174 6573 7420 7665 7273 696f 6e20   latest version 
+00001c00: 6672 6f6d 2050 7950 493a 0a0a 6060 6062  from PyPI:..```b
+00001c10: 6173 680a 7069 7020 696e 7374 616c 6c20  ash.pip install 
+00001c20: 2d55 2061 6c62 756d 656e 7461 7469 6f6e  -U albumentation
+00001c30: 730a 6060 600a 0a4f 7468 6572 2069 6e73  s.```..Other ins
+00001c40: 7461 6c6c 6174 696f 6e20 6f70 7469 6f6e  tallation option
+00001c50: 7320 6172 6520 6465 7363 7269 6265 6420  s are described 
+00001c60: 696e 2074 6865 205b 646f 6375 6d65 6e74  in the [document
+00001c70: 6174 696f 6e5d 2868 7474 7073 3a2f 2f61  ation](https://a
+00001c80: 6c62 756d 656e 7461 7469 6f6e 732e 6169  lbumentations.ai
+00001c90: 2f64 6f63 732f 6765 7474 696e 675f 7374  /docs/getting_st
+00001ca0: 6172 7465 642f 696e 7374 616c 6c61 7469  arted/installati
+00001cb0: 6f6e 2f29 2e0a 0a23 2320 446f 6375 6d65  on/)...## Docume
+00001cc0: 6e74 6174 696f 6e0a 0a54 6865 2066 756c  ntation..The ful
+00001cd0: 6c20 646f 6375 6d65 6e74 6174 696f 6e20  l documentation 
+00001ce0: 6973 2061 7661 696c 6162 6c65 2061 7420  is available at 
+00001cf0: 2a2a 5b68 7474 7073 3a2f 2f61 6c62 756d  **[https://album
+00001d00: 656e 7461 7469 6f6e 732e 6169 2f64 6f63  entations.ai/doc
+00001d10: 732f 5d28 6874 7470 733a 2f2f 616c 6275  s/](https://albu
+00001d20: 6d65 6e74 6174 696f 6e73 2e61 692f 646f  mentations.ai/do
+00001d30: 6373 2f29 2a2a 2e0a 0a23 2320 4120 7369  cs/)**...## A si
+00001d40: 6d70 6c65 2065 7861 6d70 6c65 0a0a 6060  mple example..``
+00001d50: 6070 7974 686f 6e0a 696d 706f 7274 2061  `python.import a
+00001d60: 6c62 756d 656e 7461 7469 6f6e 7320 6173  lbumentations as
+00001d70: 2041 0a69 6d70 6f72 7420 6376 320a 0a23   A.import cv2..#
+00001d80: 2044 6563 6c61 7265 2061 6e20 6175 676d   Declare an augm
+00001d90: 656e 7461 7469 6f6e 2070 6970 656c 696e  entation pipelin
+00001da0: 650a 7472 616e 7366 6f72 6d20 3d20 412e  e.transform = A.
+00001db0: 436f 6d70 6f73 6528 5b0a 2020 2020 412e  Compose([.    A.
+00001dc0: 5261 6e64 6f6d 4372 6f70 2877 6964 7468  RandomCrop(width
+00001dd0: 3d32 3536 2c20 6865 6967 6874 3d32 3536  =256, height=256
+00001de0: 292c 0a20 2020 2041 2e48 6f72 697a 6f6e  ),.    A.Horizon
+00001df0: 7461 6c46 6c69 7028 703d 302e 3529 2c0a  talFlip(p=0.5),.
+00001e00: 2020 2020 412e 5261 6e64 6f6d 4272 6967      A.RandomBrig
+00001e10: 6874 6e65 7373 436f 6e74 7261 7374 2870  htnessContrast(p
+00001e20: 3d30 2e32 292c 0a5d 290a 0a23 2052 6561  =0.2),.])..# Rea
+00001e30: 6420 616e 2069 6d61 6765 2077 6974 6820  d an image with 
+00001e40: 4f70 656e 4356 2061 6e64 2063 6f6e 7665  OpenCV and conve
+00001e50: 7274 2069 7420 746f 2074 6865 2052 4742  rt it to the RGB
+00001e60: 2063 6f6c 6f72 7370 6163 650a 696d 6167   colorspace.imag
+00001e70: 6520 3d20 6376 322e 696d 7265 6164 2822  e = cv2.imread("
+00001e80: 696d 6167 652e 6a70 6722 290a 696d 6167  image.jpg").imag
+00001e90: 6520 3d20 6376 322e 6376 7443 6f6c 6f72  e = cv2.cvtColor
+00001ea0: 2869 6d61 6765 2c20 6376 322e 434f 4c4f  (image, cv2.COLO
+00001eb0: 525f 4247 5232 5247 4229 0a0a 2320 4175  R_BGR2RGB)..# Au
+00001ec0: 676d 656e 7420 616e 2069 6d61 6765 0a74  gment an image.t
+00001ed0: 7261 6e73 666f 726d 6564 203d 2074 7261  ransformed = tra
+00001ee0: 6e73 666f 726d 2869 6d61 6765 3d69 6d61  nsform(image=ima
+00001ef0: 6765 290a 7472 616e 7366 6f72 6d65 645f  ge).transformed_
+00001f00: 696d 6167 6520 3d20 7472 616e 7366 6f72  image = transfor
+00001f10: 6d65 645b 2269 6d61 6765 225d 0a60 6060  med["image"].```
+00001f20: 0a0a 2323 2047 6574 7469 6e67 2073 7461  ..## Getting sta
+00001f30: 7274 6564 0a0a 2323 2320 4920 616d 206e  rted..### I am n
+00001f40: 6577 2074 6f20 696d 6167 6520 6175 676d  ew to image augm
+00001f50: 656e 7461 7469 6f6e 0a0a 506c 6561 7365  entation..Please
+00001f60: 2073 7461 7274 2077 6974 6820 7468 6520   start with the 
+00001f70: 5b69 6e74 726f 6475 6374 696f 6e20 6172  [introduction ar
+00001f80: 7469 636c 6573 5d28 6874 7470 733a 2f2f  ticles](https://
+00001f90: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
+00001fa0: 692f 646f 6373 2f23 696e 7472 6f64 7563  i/docs/#introduc
+00001fb0: 7469 6f6e 2d74 6f2d 696d 6167 652d 6175  tion-to-image-au
+00001fc0: 676d 656e 7461 7469 6f6e 2920 6162 6f75  gmentation) abou
+00001fd0: 7420 7768 7920 696d 6167 6520 6175 676d  t why image augm
+00001fe0: 656e 7461 7469 6f6e 2069 7320 696d 706f  entation is impo
+00001ff0: 7274 616e 7420 616e 6420 686f 7720 6974  rtant and how it
+00002000: 2068 656c 7073 2074 6f20 6275 696c 6420   helps to build 
+00002010: 6265 7474 6572 206d 6f64 656c 732e 0a0a  better models...
+00002020: 2323 2320 4920 7761 6e74 2074 6f20 7573  ### I want to us
+00002030: 6520 416c 6275 6d65 6e74 6174 696f 6e73  e Albumentations
+00002040: 2066 6f72 2074 6865 2073 7065 6369 6669   for the specifi
+00002050: 6320 7461 736b 2073 7563 6820 6173 2063  c task such as c
+00002060: 6c61 7373 6966 6963 6174 696f 6e20 6f72  lassification or
+00002070: 2073 6567 6d65 6e74 6174 696f 6e0a 0a49   segmentation..I
+00002080: 6620 796f 7520 7761 6e74 2074 6f20 7573  f you want to us
+00002090: 6520 416c 6275 6d65 6e74 6174 696f 6e73  e Albumentations
+000020a0: 2066 6f72 2061 2073 7065 6369 6669 6320   for a specific 
+000020b0: 7461 736b 2073 7563 6820 6173 2063 6c61  task such as cla
+000020c0: 7373 6966 6963 6174 696f 6e2c 2073 6567  ssification, seg
+000020d0: 6d65 6e74 6174 696f 6e2c 206f 7220 6f62  mentation, or ob
+000020e0: 6a65 6374 2064 6574 6563 7469 6f6e 2c20  ject detection, 
+000020f0: 7265 6665 7220 746f 2074 6865 205b 7365  refer to the [se
+00002100: 7420 6f66 2061 7274 6963 6c65 735d 2868  t of articles](h
+00002110: 7474 7073 3a2f 2f61 6c62 756d 656e 7461  ttps://albumenta
+00002120: 7469 6f6e 732e 6169 2f64 6f63 732f 2367  tions.ai/docs/#g
+00002130: 6574 7469 6e67 2d73 7461 7274 6564 2d77  etting-started-w
+00002140: 6974 682d 616c 6275 6d65 6e74 6174 696f  ith-albumentatio
+00002150: 6e73 2920 7468 6174 2068 6173 2061 6e20  ns) that has an 
+00002160: 696e 2d64 6570 7468 2064 6573 6372 6970  in-depth descrip
+00002170: 7469 6f6e 206f 6620 7468 6973 2074 6173  tion of this tas
+00002180: 6b2e 2057 6520 616c 736f 2068 6176 6520  k. We also have 
+00002190: 6120 5b6c 6973 7420 6f66 2065 7861 6d70  a [list of examp
+000021a0: 6c65 735d 2868 7474 7073 3a2f 2f61 6c62  les](https://alb
+000021b0: 756d 656e 7461 7469 6f6e 732e 6169 2f64  umentations.ai/d
+000021c0: 6f63 732f 6578 616d 706c 6573 2f29 206f  ocs/examples/) o
+000021d0: 6e20 6170 706c 7969 6e67 2041 6c62 756d  n applying Album
+000021e0: 656e 7461 7469 6f6e 7320 666f 7220 6469  entations for di
+000021f0: 6666 6572 656e 7420 7573 6520 6361 7365  fferent use case
+00002200: 732e 0a0a 2323 2320 4920 7761 6e74 2074  s...### I want t
+00002210: 6f20 6b6e 6f77 2068 6f77 2074 6f20 7573  o know how to us
+00002220: 6520 416c 6275 6d65 6e74 6174 696f 6e73  e Albumentations
+00002230: 2077 6974 6820 6465 6570 206c 6561 726e   with deep learn
+00002240: 696e 6720 6672 616d 6577 6f72 6b73 0a0a  ing frameworks..
+00002250: 5765 2068 6176 6520 5b65 7861 6d70 6c65  We have [example
+00002260: 7320 6f66 2075 7369 6e67 2041 6c62 756d  s of using Album
+00002270: 656e 7461 7469 6f6e 735d 2868 7474 7073  entations](https
+00002280: 3a2f 2f61 6c62 756d 656e 7461 7469 6f6e  ://albumentation
+00002290: 732e 6169 2f64 6f63 732f 2365 7861 6d70  s.ai/docs/#examp
+000022a0: 6c65 732d 6f66 2d68 6f77 2d74 6f2d 7573  les-of-how-to-us
+000022b0: 652d 616c 6275 6d65 6e74 6174 696f 6e73  e-albumentations
+000022c0: 2d77 6974 682d 6469 6666 6572 656e 742d  -with-different-
+000022d0: 6465 6570 2d6c 6561 726e 696e 672d 6672  deep-learning-fr
+000022e0: 616d 6577 6f72 6b73 2920 616c 6f6e 6720  ameworks) along 
+000022f0: 7769 7468 2050 7954 6f72 6368 2061 6e64  with PyTorch and
+00002300: 2054 656e 736f 7246 6c6f 772e 0a0a 2323   TensorFlow...##
+00002310: 2320 4920 7761 6e74 2074 6f20 6578 706c  # I want to expl
+00002320: 6f72 6520 6175 676d 656e 7461 7469 6f6e  ore augmentation
+00002330: 7320 616e 6420 7365 6520 416c 6275 6d65  s and see Albume
+00002340: 6e74 6174 696f 6e73 2069 6e20 6163 7469  ntations in acti
+00002350: 6f6e 0a0a 4368 6563 6b20 7468 6520 5b6f  on..Check the [o
+00002360: 6e6c 696e 6520 6465 6d6f 206f 6620 7468  nline demo of th
+00002370: 6520 6c69 6272 6172 795d 2868 7474 7073  e library](https
+00002380: 3a2f 2f61 6c62 756d 656e 7461 7469 6f6e  ://albumentation
+00002390: 732d 6465 6d6f 2e68 6572 6f6b 7561 7070  s-demo.herokuapp
+000023a0: 2e63 6f6d 2f29 2e20 5769 7468 2069 742c  .com/). With it,
+000023b0: 2079 6f75 2063 616e 2061 7070 6c79 2061   you can apply a
+000023c0: 7567 6d65 6e74 6174 696f 6e73 2074 6f20  ugmentations to 
+000023d0: 6469 6666 6572 656e 7420 696d 6167 6573  different images
+000023e0: 2061 6e64 2073 6565 2074 6865 2072 6573   and see the res
+000023f0: 756c 742e 2041 6c73 6f2c 2077 6520 6861  ult. Also, we ha
+00002400: 7665 2061 205b 6c69 7374 206f 6620 616c  ve a [list of al
+00002410: 6c20 6176 6169 6c61 626c 6520 6175 676d  l available augm
+00002420: 656e 7461 7469 6f6e 7320 616e 6420 7468  entations and th
+00002430: 6569 7220 7461 7267 6574 735d 2823 6c69  eir targets](#li
+00002440: 7374 2d6f 662d 6175 676d 656e 7461 7469  st-of-augmentati
+00002450: 6f6e 7329 2e0a 0a23 2320 5768 6f20 6973  ons)...## Who is
+00002460: 2075 7369 6e67 2041 6c62 756d 656e 7461   using Albumenta
+00002470: 7469 6f6e 730a 0a3c 6120 6872 6566 3d22  tions..<a href="
+00002480: 6874 7470 733a 2f2f 7777 772e 6170 706c  https://www.appl
+00002490: 652e 636f 6d2f 2220 7461 7267 6574 3d22  e.com/" target="
+000024a0: 5f62 6c61 6e6b 223e 3c69 6d67 2073 7263  _blank"><img src
+000024b0: 3d22 6874 7470 733a 2f2f 7261 772e 6769  ="https://raw.gi
+000024c0: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
+000024d0: 636f 6d2f 616c 6275 6d65 6e74 6174 696f  com/albumentatio
+000024e0: 6e73 2d74 6561 6d2f 616c 6275 6d65 6e74  ns-team/albument
+000024f0: 6174 696f 6e73 2e61 692f 6d61 696e 2f68  ations.ai/main/h
+00002500: 746d 6c2f 6173 7365 7473 2f69 6d67 2f69  tml/assets/img/i
+00002510: 6e64 7573 7472 792f 6170 706c 652e 6a70  ndustry/apple.jp
+00002520: 6567 2220 7769 6474 683d 2231 3030 222f  eg" width="100"/
+00002530: 3e3c 2f61 3e0a 3c61 2068 7265 663d 2268  ></a>.<a href="h
+00002540: 7474 7073 3a2f 2f72 6573 6561 7263 682e  ttps://research.
+00002550: 676f 6f67 6c65 2f22 2074 6172 6765 743d  google/" target=
+00002560: 225f 626c 616e 6b22 3e3c 696d 6720 7372  "_blank"><img sr
+00002570: 633d 2268 7474 7073 3a2f 2f72 6177 2e67  c="https://raw.g
+00002580: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+00002590: 2e63 6f6d 2f61 6c62 756d 656e 7461 7469  .com/albumentati
+000025a0: 6f6e 732d 7465 616d 2f61 6c62 756d 656e  ons-team/albumen
+000025b0: 7461 7469 6f6e 732e 6169 2f6d 6169 6e2f  tations.ai/main/
+000025c0: 6874 6d6c 2f61 7373 6574 732f 696d 672f  html/assets/img/
+000025d0: 696e 6475 7374 7279 2f67 6f6f 676c 652e  industry/google.
+000025e0: 706e 6722 2077 6964 7468 3d22 3130 3022  png" width="100"
+000025f0: 2f3e 3c2f 613e 0a3c 6120 6872 6566 3d22  /></a>.<a href="
+00002600: 6874 7470 733a 2f2f 6f70 656e 736f 7572  https://opensour
+00002610: 6365 2e66 622e 636f 6d2f 2220 7461 7267  ce.fb.com/" targ
+00002620: 6574 3d22 5f62 6c61 6e6b 223e 3c69 6d67  et="_blank"><img
+00002630: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
+00002640: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
+00002650: 656e 742e 636f 6d2f 616c 6275 6d65 6e74  ent.com/albument
+00002660: 6174 696f 6e73 2d74 6561 6d2f 616c 6275  ations-team/albu
+00002670: 6d65 6e74 6174 696f 6e73 2e61 692f 6d61  mentations.ai/ma
+00002680: 696e 2f68 746d 6c2f 6173 7365 7473 2f69  in/html/assets/i
+00002690: 6d67 2f69 6e64 7573 7472 792f 6d65 7461  mg/industry/meta
+000026a0: 5f72 6573 6561 7263 682e 706e 6722 2077  _research.png" w
+000026b0: 6964 7468 3d22 3130 3022 2f3e 3c2f 613e  idth="100"/></a>
+000026c0: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
+000026d0: 202f 2f77 7777 2e6e 7669 6469 612e 636f   //www.nvidia.co
+000026e0: 6d2f 656e 2d75 732f 7265 7365 6172 6368  m/en-us/research
+000026f0: 2f22 2074 6172 6765 743d 225f 626c 616e  /" target="_blan
+00002700: 6b22 3e3c 696d 6720 7372 633d 2268 7474  k"><img src="htt
+00002710: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
+00002720: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f61  sercontent.com/a
+00002730: 6c62 756d 656e 7461 7469 6f6e 732d 7465  lbumentations-te
+00002740: 616d 2f61 6c62 756d 656e 7461 7469 6f6e  am/albumentation
+00002750: 732e 6169 2f6d 6169 6e2f 6874 6d6c 2f61  s.ai/main/html/a
+00002760: 7373 6574 732f 696d 672f 696e 6475 7374  ssets/img/indust
+00002770: 7279 2f6e 7669 6469 615f 7265 7365 6172  ry/nvidia_resear
+00002780: 6368 2e6a 7065 6722 2077 6964 7468 3d22  ch.jpeg" width="
+00002790: 3130 3022 2f3e 3c2f 613e 0a3c 6120 6872  100"/></a>.<a hr
+000027a0: 6566 3d22 6874 7470 733a 2f2f 7777 772e  ef="https://www.
+000027b0: 616d 617a 6f6e 2e73 6369 656e 6365 2f22  amazon.science/"
+000027c0: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
+000027d0: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
+000027e0: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
+000027f0: 7263 6f6e 7465 6e74 2e63 6f6d 2f61 6c62  rcontent.com/alb
+00002800: 756d 656e 7461 7469 6f6e 732d 7465 616d  umentations-team
+00002810: 2f61 6c62 756d 656e 7461 7469 6f6e 732e  /albumentations.
+00002820: 6169 2f6d 6169 6e2f 6874 6d6c 2f61 7373  ai/main/html/ass
+00002830: 6574 732f 696d 672f 696e 6475 7374 7279  ets/img/industry
+00002840: 2f61 6d61 7a6f 6e5f 7363 6965 6e63 652e  /amazon_science.
+00002850: 706e 6722 2077 6964 7468 3d22 3130 3022  png" width="100"
+00002860: 2f3e 3c2f 613e 0a3c 6120 6872 6566 3d22  /></a>.<a href="
+00002870: 6874 7470 733a 2f2f 6f70 656e 736f 7572  https://opensour
+00002880: 6365 2e6d 6963 726f 736f 6674 2e63 6f6d  ce.microsoft.com
+00002890: 2f22 2074 6172 6765 743d 225f 626c 616e  /" target="_blan
+000028a0: 6b22 3e3c 696d 6720 7372 633d 2268 7474  k"><img src="htt
+000028b0: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
+000028c0: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f61  sercontent.com/a
+000028d0: 6c62 756d 656e 7461 7469 6f6e 732d 7465  lbumentations-te
+000028e0: 616d 2f61 6c62 756d 656e 7461 7469 6f6e  am/albumentation
+000028f0: 732e 6169 2f6d 6169 6e2f 6874 6d6c 2f61  s.ai/main/html/a
+00002900: 7373 6574 732f 696d 672f 696e 6475 7374  ssets/img/indust
+00002910: 7279 2f6d 6963 726f 736f 6674 2e70 6e67  ry/microsoft.png
+00002920: 2220 7769 6474 683d 2231 3030 222f 3e3c  " width="100"/><
+00002930: 2f61 3e0a 3c61 2068 7265 663d 2268 7474  /a>.<a href="htt
+00002940: 7073 3a2f 2f65 6e67 696e 6565 7269 6e67  ps://engineering
+00002950: 2e73 616c 6573 666f 7263 652e 636f 6d2f  .salesforce.com/
+00002960: 6f70 656e 2d73 6f75 7263 652f 2220 7461  open-source/" ta
+00002970: 7267 6574 3d22 5f62 6c61 6e6b 223e 3c69  rget="_blank"><i
+00002980: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00002990: 7261 772e 6769 7468 7562 7573 6572 636f  raw.githubuserco
+000029a0: 6e74 656e 742e 636f 6d2f 616c 6275 6d65  ntent.com/albume
+000029b0: 6e74 6174 696f 6e73 2d74 6561 6d2f 616c  ntations-team/al
+000029c0: 6275 6d65 6e74 6174 696f 6e73 2e61 692f  bumentations.ai/
+000029d0: 6d61 696e 2f68 746d 6c2f 6173 7365 7473  main/html/assets
+000029e0: 2f69 6d67 2f69 6e64 7573 7472 792f 7361  /img/industry/sa
+000029f0: 6c65 7366 6f72 6365 5f6f 7065 6e5f 736f  lesforce_open_so
+00002a00: 7572 6365 2e70 6e67 2220 7769 6474 683d  urce.png" width=
+00002a10: 2231 3030 222f 3e3c 2f61 3e0a 3c61 2068  "100"/></a>.<a h
+00002a20: 7265 663d 2268 7474 7073 3a2f 2f73 7461  ref="https://sta
+00002a30: 6269 6c69 7479 2e61 692f 2220 7461 7267  bility.ai/" targ
+00002a40: 6574 3d22 5f62 6c61 6e6b 223e 3c69 6d67  et="_blank"><img
+00002a50: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
+00002a60: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
+00002a70: 656e 742e 636f 6d2f 616c 6275 6d65 6e74  ent.com/albument
+00002a80: 6174 696f 6e73 2d74 6561 6d2f 616c 6275  ations-team/albu
+00002a90: 6d65 6e74 6174 696f 6e73 2e61 692f 6d61  mentations.ai/ma
+00002aa0: 696e 2f68 746d 6c2f 6173 7365 7473 2f69  in/html/assets/i
+00002ab0: 6d67 2f69 6e64 7573 7472 792f 7374 6162  mg/industry/stab
+00002ac0: 696c 6974 792e 706e 6722 2077 6964 7468  ility.png" width
+00002ad0: 3d22 3130 3022 2f3e 3c2f 613e 0a3c 6120  ="100"/></a>.<a 
+00002ae0: 6872 6566 3d22 6874 7470 733a 2f2f 7777  href="https://ww
+00002af0: 772e 6962 6d2e 636f 6d2f 6f70 656e 736f  w.ibm.com/openso
+00002b00: 7572 6365 2f22 2074 6172 6765 743d 225f  urce/" target="_
+00002b10: 626c 616e 6b22 3e3c 696d 6720 7372 633d  blank"><img src=
+00002b20: 2268 7474 7073 3a2f 2f72 6177 2e67 6974  "https://raw.git
+00002b30: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+00002b40: 6f6d 2f61 6c62 756d 656e 7461 7469 6f6e  om/albumentation
+00002b50: 732d 7465 616d 2f61 6c62 756d 656e 7461  s-team/albumenta
+00002b60: 7469 6f6e 732e 6169 2f6d 6169 6e2f 6874  tions.ai/main/ht
+00002b70: 6d6c 2f61 7373 6574 732f 696d 672f 696e  ml/assets/img/in
+00002b80: 6475 7374 7279 2f69 626d 2e6a 7065 6722  dustry/ibm.jpeg"
+00002b90: 2077 6964 7468 3d22 3130 3022 2f3e 3c2f   width="100"/></
+00002ba0: 613e 0a3c 6120 6872 6566 3d22 6874 7470  a>.<a href="http
+00002bb0: 733a 2f2f 6875 6767 696e 6766 6163 652e  s://huggingface.
+00002bc0: 636f 2f22 2074 6172 6765 743d 225f 626c  co/" target="_bl
+00002bd0: 616e 6b22 3e3c 696d 6720 7372 633d 2268  ank"><img src="h
+00002be0: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
+00002bf0: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+00002c00: 2f61 6c62 756d 656e 7461 7469 6f6e 732d  /albumentations-
+00002c10: 7465 616d 2f61 6c62 756d 656e 7461 7469  team/albumentati
+00002c20: 6f6e 732e 6169 2f6d 6169 6e2f 6874 6d6c  ons.ai/main/html
+00002c30: 2f61 7373 6574 732f 696d 672f 696e 6475  /assets/img/indu
+00002c40: 7374 7279 2f68 7567 6769 6e67 5f66 6163  stry/hugging_fac
+00002c50: 652e 706e 6722 2077 6964 7468 3d22 3130  e.png" width="10
+00002c60: 3022 2f3e 3c2f 613e 0a3c 6120 6872 6566  0"/></a>.<a href
+00002c70: 3d22 6874 7470 733a 2f2f 7777 772e 736f  ="https://www.so
+00002c80: 6e79 2e63 6f6d 2f65 6e2f 2220 7461 7267  ny.com/en/" targ
+00002c90: 6574 3d22 5f62 6c61 6e6b 223e 3c69 6d67  et="_blank"><img
+00002ca0: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
+00002cb0: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
+00002cc0: 656e 742e 636f 6d2f 616c 6275 6d65 6e74  ent.com/albument
+00002cd0: 6174 696f 6e73 2d74 6561 6d2f 616c 6275  ations-team/albu
+00002ce0: 6d65 6e74 6174 696f 6e73 2e61 692f 6d61  mentations.ai/ma
+00002cf0: 696e 2f68 746d 6c2f 6173 7365 7473 2f69  in/html/assets/i
+00002d00: 6d67 2f69 6e64 7573 7472 792f 736f 6e79  mg/industry/sony
+00002d10: 2e70 6e67 2220 7769 6474 683d 2231 3030  .png" width="100
+00002d20: 222f 3e3c 2f61 3e0a 3c61 2068 7265 663d  "/></a>.<a href=
+00002d30: 2268 7474 7073 3a2f 2f6f 7065 6e73 6f75  "https://opensou
+00002d40: 7263 652e 616c 6962 6162 612e 636f 6d2f  rce.alibaba.com/
+00002d50: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
+00002d60: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
+00002d70: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+00002d80: 6572 636f 6e74 656e 742e 636f 6d2f 616c  ercontent.com/al
+00002d90: 6275 6d65 6e74 6174 696f 6e73 2d74 6561  bumentations-tea
+00002da0: 6d2f 616c 6275 6d65 6e74 6174 696f 6e73  m/albumentations
+00002db0: 2e61 692f 6d61 696e 2f68 746d 6c2f 6173  .ai/main/html/as
+00002dc0: 7365 7473 2f69 6d67 2f69 6e64 7573 7472  sets/img/industr
+00002dd0: 792f 616c 6962 6162 612e 706e 6722 2077  y/alibaba.png" w
+00002de0: 6964 7468 3d22 3130 3022 2f3e 3c2f 613e  idth="100"/></a>
+00002df0: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
+00002e00: 2f2f 6f70 656e 736f 7572 6365 2e74 656e  //opensource.ten
+00002e10: 6365 6e74 2e63 6f6d 2f22 2074 6172 6765  cent.com/" targe
+00002e20: 743d 225f 626c 616e 6b22 3e3c 696d 6720  t="_blank"><img 
+00002e30: 7372 633d 2268 7474 7073 3a2f 2f72 6177  src="https://raw
+00002e40: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
+00002e50: 6e74 2e63 6f6d 2f61 6c62 756d 656e 7461  nt.com/albumenta
+00002e60: 7469 6f6e 732d 7465 616d 2f61 6c62 756d  tions-team/album
+00002e70: 656e 7461 7469 6f6e 732e 6169 2f6d 6169  entations.ai/mai
+00002e80: 6e2f 6874 6d6c 2f61 7373 6574 732f 696d  n/html/assets/im
+00002e90: 672f 696e 6475 7374 7279 2f74 656e 6365  g/industry/tence
+00002ea0: 6e74 2e70 6e67 2220 7769 6474 683d 2231  nt.png" width="1
+00002eb0: 3030 222f 3e3c 2f61 3e0a 3c61 2068 7265  00"/></a>.<a hre
+00002ec0: 663d 2268 7474 7073 3a2f 2f68 326f 2e61  f="https://h2o.a
+00002ed0: 692f 2220 7461 7267 6574 3d22 5f62 6c61  i/" target="_bla
+00002ee0: 6e6b 223e 3c69 6d67 2073 7263 3d22 6874  nk"><img src="ht
+00002ef0: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
+00002f00: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+00002f10: 616c 6275 6d65 6e74 6174 696f 6e73 2d74  albumentations-t
+00002f20: 6561 6d2f 616c 6275 6d65 6e74 6174 696f  eam/albumentatio
+00002f30: 6e73 2e61 692f 6d61 696e 2f68 746d 6c2f  ns.ai/main/html/
+00002f40: 6173 7365 7473 2f69 6d67 2f69 6e64 7573  assets/img/indus
+00002f50: 7472 792f 6832 6f5f 6169 2e70 6e67 2220  try/h2o_ai.png" 
+00002f60: 7769 6474 683d 2231 3030 222f 3e3c 2f61  width="100"/></a
+00002f70: 3e0a 0a23 2323 2053 6565 2061 6c73 6f0a  >..### See also.
+00002f80: 0a2d 205b 4120 6c69 7374 206f 6620 7061  .- [A list of pa
+00002f90: 7065 7273 2074 6861 7420 6369 7465 2041  pers that cite A
+00002fa0: 6c62 756d 656e 7461 7469 6f6e 735d 2868  lbumentations](h
+00002fb0: 7474 7073 3a2f 2f73 6368 6f6c 6172 2e67  ttps://scholar.g
+00002fc0: 6f6f 676c 652e 636f 6d2f 6369 7461 7469  oogle.com/citati
+00002fd0: 6f6e 733f 7669 6577 5f6f 703d 7669 6577  ons?view_op=view
+00002fe0: 5f63 6974 6174 696f 6e26 6369 7461 7469  _citation&citati
+00002ff0: 6f6e 5f66 6f72 5f76 6965 773d 766b 6a68  on_for_view=vkjh
+00003000: 3958 3041 4141 414a 3a72 3042 706e 745a  9X0AAAAJ:r0BpntZ
+00003010: 714a 4734 4329 2e0a 2d20 5b41 206c 6973  qJG4C)..- [A lis
+00003020: 7420 6f66 2074 6561 6d73 2074 6861 7420  t of teams that 
+00003030: 7765 7265 2075 7369 6e67 2041 6c62 756d  were using Album
+00003040: 656e 7461 7469 6f6e 7320 616e 6420 746f  entations and to
+00003050: 6f6b 2068 6967 6820 706c 6163 6573 2069  ok high places i
+00003060: 6e20 6d61 6368 696e 6520 6c65 6172 6e69  n machine learni
+00003070: 6e67 2063 6f6d 7065 7469 7469 6f6e 735d  ng competitions]
+00003080: 2868 7474 7073 3a2f 2f61 6c62 756d 656e  (https://albumen
+00003090: 7461 7469 6f6e 732e 6169 2f77 686f 735f  tations.ai/whos_
+000030a0: 7573 696e 6723 636f 6d70 6574 6974 696f  using#competitio
+000030b0: 6e73 292e 0a2d 205b 4f70 656e 2073 6f75  ns)..- [Open sou
+000030c0: 7263 6520 7072 6f6a 6563 7473 2074 6861  rce projects tha
+000030d0: 7420 7573 6520 416c 6275 6d65 6e74 6174  t use Albumentat
+000030e0: 696f 6e73 5d28 6874 7470 733a 2f2f 6769  ions](https://gi
+000030f0: 7468 7562 2e63 6f6d 2f61 6c62 756d 656e  thub.com/albumen
+00003100: 7461 7469 6f6e 732d 7465 616d 2f61 6c62  tations-team/alb
+00003110: 756d 656e 7461 7469 6f6e 732f 6e65 7477  umentations/netw
+00003120: 6f72 6b2f 6465 7065 6e64 656e 7473 3f64  ork/dependents?d
+00003130: 6570 656e 6465 6e74 5f74 7970 653d 5041  ependent_type=PA
+00003140: 434b 4147 4529 2e0a 0a23 2320 4c69 7374  CKAGE)...## List
+00003150: 206f 6620 6175 676d 656e 7461 7469 6f6e   of augmentation
+00003160: 730a 0a23 2323 2050 6978 656c 2d6c 6576  s..### Pixel-lev
+00003170: 656c 2074 7261 6e73 666f 726d 730a 0a50  el transforms..P
+00003180: 6978 656c 2d6c 6576 656c 2074 7261 6e73  ixel-level trans
+00003190: 666f 726d 7320 7769 6c6c 2063 6861 6e67  forms will chang
+000031a0: 6520 6a75 7374 2061 6e20 696e 7075 7420  e just an input 
+000031b0: 696d 6167 6520 616e 6420 7769 6c6c 206c  image and will l
+000031c0: 6561 7665 2061 6e79 2061 6464 6974 696f  eave any additio
+000031d0: 6e61 6c20 7461 7267 6574 7320 7375 6368  nal targets such
+000031e0: 2061 7320 6d61 736b 732c 2062 6f75 6e64   as masks, bound
+000031f0: 696e 6720 626f 7865 732c 2061 6e64 206b  ing boxes, and k
+00003200: 6579 706f 696e 7473 2075 6e63 6861 6e67  eypoints unchang
+00003210: 6564 2e20 5468 6520 6c69 7374 206f 6620  ed. The list of 
+00003220: 7069 7865 6c2d 6c65 7665 6c20 7472 616e  pixel-level tran
+00003230: 7366 6f72 6d73 3a0a 0a2d 205b 4164 7661  sforms:..- [Adva
+00003240: 6e63 6564 426c 7572 5d28 6874 7470 733a  ncedBlur](https:
+00003250: 2f2f 616c 6275 6d65 6e74 6174 696f 6e73  //albumentations
+00003260: 2e61 692f 646f 6373 2f61 7069 5f72 6566  .ai/docs/api_ref
+00003270: 6572 656e 6365 2f61 7567 6d65 6e74 6174  erence/augmentat
+00003280: 696f 6e73 2f62 6c75 722f 7472 616e 7366  ions/blur/transf
+00003290: 6f72 6d73 2f23 616c 6275 6d65 6e74 6174  orms/#albumentat
+000032a0: 696f 6e73 2e61 7567 6d65 6e74 6174 696f  ions.augmentatio
+000032b0: 6e73 2e62 6c75 722e 7472 616e 7366 6f72  ns.blur.transfor
+000032c0: 6d73 2e41 6476 616e 6365 6442 6c75 7229  ms.AdvancedBlur)
+000032d0: 0a2d 205b 426c 7572 5d28 6874 7470 733a  .- [Blur](https:
+000032e0: 2f2f 616c 6275 6d65 6e74 6174 696f 6e73  //albumentations
+000032f0: 2e61 692f 646f 6373 2f61 7069 5f72 6566  .ai/docs/api_ref
+00003300: 6572 656e 6365 2f61 7567 6d65 6e74 6174  erence/augmentat
+00003310: 696f 6e73 2f62 6c75 722f 7472 616e 7366  ions/blur/transf
+00003320: 6f72 6d73 2f23 616c 6275 6d65 6e74 6174  orms/#albumentat
+00003330: 696f 6e73 2e61 7567 6d65 6e74 6174 696f  ions.augmentatio
+00003340: 6e73 2e62 6c75 722e 7472 616e 7366 6f72  ns.blur.transfor
+00003350: 6d73 2e42 6c75 7229 0a2d 205b 434c 4148  ms.Blur).- [CLAH
+00003360: 455d 2868 7474 7073 3a2f 2f61 6c62 756d  E](https://album
+00003370: 656e 7461 7469 6f6e 732e 6169 2f64 6f63  entations.ai/doc
+00003380: 732f 6170 695f 7265 6665 7265 6e63 652f  s/api_reference/
+00003390: 6175 676d 656e 7461 7469 6f6e 732f 7472  augmentations/tr
+000033a0: 616e 7366 6f72 6d73 2f23 616c 6275 6d65  ansforms/#albume
+000033b0: 6e74 6174 696f 6e73 2e61 7567 6d65 6e74  ntations.augment
+000033c0: 6174 696f 6e73 2e74 7261 6e73 666f 726d  ations.transform
+000033d0: 732e 434c 4148 4529 0a2d 205b 4368 616e  s.CLAHE).- [Chan
+000033e0: 6e65 6c44 726f 706f 7574 5d28 6874 7470  nelDropout](http
+000033f0: 733a 2f2f 616c 6275 6d65 6e74 6174 696f  s://albumentatio
+00003400: 6e73 2e61 692f 646f 6373 2f61 7069 5f72  ns.ai/docs/api_r
+00003410: 6566 6572 656e 6365 2f61 7567 6d65 6e74  eference/augment
+00003420: 6174 696f 6e73 2f64 726f 706f 7574 2f63  ations/dropout/c
+00003430: 6861 6e6e 656c 5f64 726f 706f 7574 2f23  hannel_dropout/#
+00003440: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
+00003450: 7567 6d65 6e74 6174 696f 6e73 2e64 726f  ugmentations.dro
+00003460: 706f 7574 2e63 6861 6e6e 656c 5f64 726f  pout.channel_dro
+00003470: 706f 7574 2e43 6861 6e6e 656c 4472 6f70  pout.ChannelDrop
+00003480: 6f75 7429 0a2d 205b 4368 616e 6e65 6c53  out).- [ChannelS
+00003490: 6875 6666 6c65 5d28 6874 7470 733a 2f2f  huffle](https://
+000034a0: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
+000034b0: 692f 646f 6373 2f61 7069 5f72 6566 6572  i/docs/api_refer
+000034c0: 656e 6365 2f61 7567 6d65 6e74 6174 696f  ence/augmentatio
+000034d0: 6e73 2f74 7261 6e73 666f 726d 732f 2361  ns/transforms/#a
+000034e0: 6c62 756d 656e 7461 7469 6f6e 732e 6175  lbumentations.au
+000034f0: 676d 656e 7461 7469 6f6e 732e 7472 616e  gmentations.tran
+00003500: 7366 6f72 6d73 2e43 6861 6e6e 656c 5368  sforms.ChannelSh
+00003510: 7566 666c 6529 0a2d 205b 4368 726f 6d61  uffle).- [Chroma
+00003520: 7469 6341 6265 7272 6174 696f 6e5d 2868  ticAberration](h
+00003530: 7474 7073 3a2f 2f61 6c62 756d 656e 7461  ttps://albumenta
+00003540: 7469 6f6e 732e 6169 2f64 6f63 732f 6170  tions.ai/docs/ap
+00003550: 695f 7265 6665 7265 6e63 652f 6175 676d  i_reference/augm
+00003560: 656e 7461 7469 6f6e 732f 7472 616e 7366  entations/transf
+00003570: 6f72 6d73 2f23 616c 6275 6d65 6e74 6174  orms/#albumentat
+00003580: 696f 6e73 2e61 7567 6d65 6e74 6174 696f  ions.augmentatio
+00003590: 6e73 2e74 7261 6e73 666f 726d 732e 4368  ns.transforms.Ch
+000035a0: 726f 6d61 7469 6341 6265 7272 6174 696f  romaticAberratio
+000035b0: 6e29 0a2d 205b 436f 6c6f 724a 6974 7465  n).- [ColorJitte
+000035c0: 725d 2868 7474 7073 3a2f 2f61 6c62 756d  r](https://album
+000035d0: 656e 7461 7469 6f6e 732e 6169 2f64 6f63  entations.ai/doc
+000035e0: 732f 6170 695f 7265 6665 7265 6e63 652f  s/api_reference/
+000035f0: 6175 676d 656e 7461 7469 6f6e 732f 7472  augmentations/tr
+00003600: 616e 7366 6f72 6d73 2f23 616c 6275 6d65  ansforms/#albume
+00003610: 6e74 6174 696f 6e73 2e61 7567 6d65 6e74  ntations.augment
+00003620: 6174 696f 6e73 2e74 7261 6e73 666f 726d  ations.transform
+00003630: 732e 436f 6c6f 724a 6974 7465 7229 0a2d  s.ColorJitter).-
+00003640: 205b 4465 666f 6375 735d 2868 7474 7073   [Defocus](https
+00003650: 3a2f 2f61 6c62 756d 656e 7461 7469 6f6e  ://albumentation
+00003660: 732e 6169 2f64 6f63 732f 6170 695f 7265  s.ai/docs/api_re
+00003670: 6665 7265 6e63 652f 6175 676d 656e 7461  ference/augmenta
+00003680: 7469 6f6e 732f 626c 7572 2f74 7261 6e73  tions/blur/trans
+00003690: 666f 726d 732f 2361 6c62 756d 656e 7461  forms/#albumenta
+000036a0: 7469 6f6e 732e 6175 676d 656e 7461 7469  tions.augmentati
+000036b0: 6f6e 732e 626c 7572 2e74 7261 6e73 666f  ons.blur.transfo
+000036c0: 726d 732e 4465 666f 6375 7329 0a2d 205b  rms.Defocus).- [
+000036d0: 446f 776e 7363 616c 655d 2868 7474 7073  Downscale](https
+000036e0: 3a2f 2f61 6c62 756d 656e 7461 7469 6f6e  ://albumentation
+000036f0: 732e 6169 2f64 6f63 732f 6170 695f 7265  s.ai/docs/api_re
+00003700: 6665 7265 6e63 652f 6175 676d 656e 7461  ference/augmenta
+00003710: 7469 6f6e 732f 7472 616e 7366 6f72 6d73  tions/transforms
+00003720: 2f23 616c 6275 6d65 6e74 6174 696f 6e73  /#albumentations
+00003730: 2e61 7567 6d65 6e74 6174 696f 6e73 2e74  .augmentations.t
+00003740: 7261 6e73 666f 726d 732e 446f 776e 7363  ransforms.Downsc
+00003750: 616c 6529 0a2d 205b 456d 626f 7373 5d28  ale).- [Emboss](
+00003760: 6874 7470 733a 2f2f 616c 6275 6d65 6e74  https://albument
+00003770: 6174 696f 6e73 2e61 692f 646f 6373 2f61  ations.ai/docs/a
+00003780: 7069 5f72 6566 6572 656e 6365 2f61 7567  pi_reference/aug
+00003790: 6d65 6e74 6174 696f 6e73 2f74 7261 6e73  mentations/trans
+000037a0: 666f 726d 732f 2361 6c62 756d 656e 7461  forms/#albumenta
+000037b0: 7469 6f6e 732e 6175 676d 656e 7461 7469  tions.augmentati
+000037c0: 6f6e 732e 7472 616e 7366 6f72 6d73 2e45  ons.transforms.E
+000037d0: 6d62 6f73 7329 0a2d 205b 4571 7561 6c69  mboss).- [Equali
+000037e0: 7a65 5d28 6874 7470 733a 2f2f 616c 6275  ze](https://albu
+000037f0: 6d65 6e74 6174 696f 6e73 2e61 692f 646f  mentations.ai/do
+00003800: 6373 2f61 7069 5f72 6566 6572 656e 6365  cs/api_reference
+00003810: 2f61 7567 6d65 6e74 6174 696f 6e73 2f74  /augmentations/t
+00003820: 7261 6e73 666f 726d 732f 2361 6c62 756d  ransforms/#album
+00003830: 656e 7461 7469 6f6e 732e 6175 676d 656e  entations.augmen
+00003840: 7461 7469 6f6e 732e 7472 616e 7366 6f72  tations.transfor
+00003850: 6d73 2e45 7175 616c 697a 6529 0a2d 205b  ms.Equalize).- [
+00003860: 4644 415d 2868 7474 7073 3a2f 2f61 6c62  FDA](https://alb
+00003870: 756d 656e 7461 7469 6f6e 732e 6169 2f64  umentations.ai/d
+00003880: 6f63 732f 6170 695f 7265 6665 7265 6e63  ocs/api_referenc
+00003890: 652f 6175 676d 656e 7461 7469 6f6e 732f  e/augmentations/
+000038a0: 646f 6d61 696e 5f61 6461 7074 6174 696f  domain_adaptatio
+000038b0: 6e2f 2361 6c62 756d 656e 7461 7469 6f6e  n/#albumentation
+000038c0: 732e 6175 676d 656e 7461 7469 6f6e 732e  s.augmentations.
+000038d0: 646f 6d61 696e 5f61 6461 7074 6174 696f  domain_adaptatio
+000038e0: 6e2e 4644 4129 0a2d 205b 4661 6e63 7950  n.FDA).- [FancyP
+000038f0: 4341 5d28 6874 7470 733a 2f2f 616c 6275  CA](https://albu
+00003900: 6d65 6e74 6174 696f 6e73 2e61 692f 646f  mentations.ai/do
+00003910: 6373 2f61 7069 5f72 6566 6572 656e 6365  cs/api_reference
+00003920: 2f61 7567 6d65 6e74 6174 696f 6e73 2f74  /augmentations/t
+00003930: 7261 6e73 666f 726d 732f 2361 6c62 756d  ransforms/#album
+00003940: 656e 7461 7469 6f6e 732e 6175 676d 656e  entations.augmen
+00003950: 7461 7469 6f6e 732e 7472 616e 7366 6f72  tations.transfor
+00003960: 6d73 2e46 616e 6379 5043 4129 0a2d 205b  ms.FancyPCA).- [
+00003970: 4672 6f6d 466c 6f61 745d 2868 7474 7073  FromFloat](https
+00003980: 3a2f 2f61 6c62 756d 656e 7461 7469 6f6e  ://albumentation
+00003990: 732e 6169 2f64 6f63 732f 6170 695f 7265  s.ai/docs/api_re
+000039a0: 6665 7265 6e63 652f 6175 676d 656e 7461  ference/augmenta
+000039b0: 7469 6f6e 732f 7472 616e 7366 6f72 6d73  tions/transforms
+000039c0: 2f23 616c 6275 6d65 6e74 6174 696f 6e73  /#albumentations
+000039d0: 2e61 7567 6d65 6e74 6174 696f 6e73 2e74  .augmentations.t
+000039e0: 7261 6e73 666f 726d 732e 4672 6f6d 466c  ransforms.FromFl
+000039f0: 6f61 7429 0a2d 205b 4761 7573 734e 6f69  oat).- [GaussNoi
+00003a00: 7365 5d28 6874 7470 733a 2f2f 616c 6275  se](https://albu
+00003a10: 6d65 6e74 6174 696f 6e73 2e61 692f 646f  mentations.ai/do
+00003a20: 6373 2f61 7069 5f72 6566 6572 656e 6365  cs/api_reference
+00003a30: 2f61 7567 6d65 6e74 6174 696f 6e73 2f74  /augmentations/t
+00003a40: 7261 6e73 666f 726d 732f 2361 6c62 756d  ransforms/#album
+00003a50: 656e 7461 7469 6f6e 732e 6175 676d 656e  entations.augmen
+00003a60: 7461 7469 6f6e 732e 7472 616e 7366 6f72  tations.transfor
+00003a70: 6d73 2e47 6175 7373 4e6f 6973 6529 0a2d  ms.GaussNoise).-
+00003a80: 205b 4761 7573 7369 616e 426c 7572 5d28   [GaussianBlur](
+00003a90: 6874 7470 733a 2f2f 616c 6275 6d65 6e74  https://albument
+00003aa0: 6174 696f 6e73 2e61 692f 646f 6373 2f61  ations.ai/docs/a
+00003ab0: 7069 5f72 6566 6572 656e 6365 2f61 7567  pi_reference/aug
+00003ac0: 6d65 6e74 6174 696f 6e73 2f62 6c75 722f  mentations/blur/
+00003ad0: 7472 616e 7366 6f72 6d73 2f23 616c 6275  transforms/#albu
+00003ae0: 6d65 6e74 6174 696f 6e73 2e61 7567 6d65  mentations.augme
+00003af0: 6e74 6174 696f 6e73 2e62 6c75 722e 7472  ntations.blur.tr
+00003b00: 616e 7366 6f72 6d73 2e47 6175 7373 6961  ansforms.Gaussia
+00003b10: 6e42 6c75 7229 0a2d 205b 476c 6173 7342  nBlur).- [GlassB
+00003b20: 6c75 725d 2868 7474 7073 3a2f 2f61 6c62  lur](https://alb
+00003b30: 756d 656e 7461 7469 6f6e 732e 6169 2f64  umentations.ai/d
+00003b40: 6f63 732f 6170 695f 7265 6665 7265 6e63  ocs/api_referenc
+00003b50: 652f 6175 676d 656e 7461 7469 6f6e 732f  e/augmentations/
+00003b60: 626c 7572 2f74 7261 6e73 666f 726d 732f  blur/transforms/
+00003b70: 2361 6c62 756d 656e 7461 7469 6f6e 732e  #albumentations.
+00003b80: 6175 676d 656e 7461 7469 6f6e 732e 626c  augmentations.bl
+00003b90: 7572 2e74 7261 6e73 666f 726d 732e 476c  ur.transforms.Gl
+00003ba0: 6173 7342 6c75 7229 0a2d 205b 4869 7374  assBlur).- [Hist
+00003bb0: 6f67 7261 6d4d 6174 6368 696e 675d 2868  ogramMatching](h
+00003bc0: 7474 7073 3a2f 2f61 6c62 756d 656e 7461  ttps://albumenta
+00003bd0: 7469 6f6e 732e 6169 2f64 6f63 732f 6170  tions.ai/docs/ap
+00003be0: 695f 7265 6665 7265 6e63 652f 6175 676d  i_reference/augm
+00003bf0: 656e 7461 7469 6f6e 732f 646f 6d61 696e  entations/domain
+00003c00: 5f61 6461 7074 6174 696f 6e2f 2361 6c62  _adaptation/#alb
+00003c10: 756d 656e 7461 7469 6f6e 732e 6175 676d  umentations.augm
+00003c20: 656e 7461 7469 6f6e 732e 646f 6d61 696e  entations.domain
+00003c30: 5f61 6461 7074 6174 696f 6e2e 4869 7374  _adaptation.Hist
+00003c40: 6f67 7261 6d4d 6174 6368 696e 6729 0a2d  ogramMatching).-
+00003c50: 205b 4875 6553 6174 7572 6174 696f 6e56   [HueSaturationV
+00003c60: 616c 7565 5d28 6874 7470 733a 2f2f 616c  alue](https://al
+00003c70: 6275 6d65 6e74 6174 696f 6e73 2e61 692f  bumentations.ai/
+00003c80: 646f 6373 2f61 7069 5f72 6566 6572 656e  docs/api_referen
+00003c90: 6365 2f61 7567 6d65 6e74 6174 696f 6e73  ce/augmentations
+00003ca0: 2f74 7261 6e73 666f 726d 732f 2361 6c62  /transforms/#alb
+00003cb0: 756d 656e 7461 7469 6f6e 732e 6175 676d  umentations.augm
+00003cc0: 656e 7461 7469 6f6e 732e 7472 616e 7366  entations.transf
+00003cd0: 6f72 6d73 2e48 7565 5361 7475 7261 7469  orms.HueSaturati
+00003ce0: 6f6e 5661 6c75 6529 0a2d 205b 4953 4f4e  onValue).- [ISON
+00003cf0: 6f69 7365 5d28 6874 7470 733a 2f2f 616c  oise](https://al
+00003d00: 6275 6d65 6e74 6174 696f 6e73 2e61 692f  bumentations.ai/
+00003d10: 646f 6373 2f61 7069 5f72 6566 6572 656e  docs/api_referen
+00003d20: 6365 2f61 7567 6d65 6e74 6174 696f 6e73  ce/augmentations
+00003d30: 2f74 7261 6e73 666f 726d 732f 2361 6c62  /transforms/#alb
+00003d40: 756d 656e 7461 7469 6f6e 732e 6175 676d  umentations.augm
+00003d50: 656e 7461 7469 6f6e 732e 7472 616e 7366  entations.transf
+00003d60: 6f72 6d73 2e49 534f 4e6f 6973 6529 0a2d  orms.ISONoise).-
+00003d70: 205b 496d 6167 6543 6f6d 7072 6573 7369   [ImageCompressi
+00003d80: 6f6e 5d28 6874 7470 733a 2f2f 616c 6275  on](https://albu
+00003d90: 6d65 6e74 6174 696f 6e73 2e61 692f 646f  mentations.ai/do
+00003da0: 6373 2f61 7069 5f72 6566 6572 656e 6365  cs/api_reference
+00003db0: 2f61 7567 6d65 6e74 6174 696f 6e73 2f74  /augmentations/t
+00003dc0: 7261 6e73 666f 726d 732f 2361 6c62 756d  ransforms/#album
+00003dd0: 656e 7461 7469 6f6e 732e 6175 676d 656e  entations.augmen
+00003de0: 7461 7469 6f6e 732e 7472 616e 7366 6f72  tations.transfor
+00003df0: 6d73 2e49 6d61 6765 436f 6d70 7265 7373  ms.ImageCompress
+00003e00: 696f 6e29 0a2d 205b 496e 7665 7274 496d  ion).- [InvertIm
+00003e10: 675d 2868 7474 7073 3a2f 2f61 6c62 756d  g](https://album
+00003e20: 656e 7461 7469 6f6e 732e 6169 2f64 6f63  entations.ai/doc
+00003e30: 732f 6170 695f 7265 6665 7265 6e63 652f  s/api_reference/
+00003e40: 6175 676d 656e 7461 7469 6f6e 732f 7472  augmentations/tr
+00003e50: 616e 7366 6f72 6d73 2f23 616c 6275 6d65  ansforms/#albume
+00003e60: 6e74 6174 696f 6e73 2e61 7567 6d65 6e74  ntations.augment
+00003e70: 6174 696f 6e73 2e74 7261 6e73 666f 726d  ations.transform
+00003e80: 732e 496e 7665 7274 496d 6729 0a2d 205b  s.InvertImg).- [
+00003e90: 4d65 6469 616e 426c 7572 5d28 6874 7470  MedianBlur](http
+00003ea0: 733a 2f2f 616c 6275 6d65 6e74 6174 696f  s://albumentatio
+00003eb0: 6e73 2e61 692f 646f 6373 2f61 7069 5f72  ns.ai/docs/api_r
+00003ec0: 6566 6572 656e 6365 2f61 7567 6d65 6e74  eference/augment
+00003ed0: 6174 696f 6e73 2f62 6c75 722f 7472 616e  ations/blur/tran
+00003ee0: 7366 6f72 6d73 2f23 616c 6275 6d65 6e74  sforms/#albument
+00003ef0: 6174 696f 6e73 2e61 7567 6d65 6e74 6174  ations.augmentat
+00003f00: 696f 6e73 2e62 6c75 722e 7472 616e 7366  ions.blur.transf
+00003f10: 6f72 6d73 2e4d 6564 6961 6e42 6c75 7229  orms.MedianBlur)
+00003f20: 0a2d 205b 4d6f 7469 6f6e 426c 7572 5d28  .- [MotionBlur](
+00003f30: 6874 7470 733a 2f2f 616c 6275 6d65 6e74  https://albument
+00003f40: 6174 696f 6e73 2e61 692f 646f 6373 2f61  ations.ai/docs/a
+00003f50: 7069 5f72 6566 6572 656e 6365 2f61 7567  pi_reference/aug
+00003f60: 6d65 6e74 6174 696f 6e73 2f62 6c75 722f  mentations/blur/
+00003f70: 7472 616e 7366 6f72 6d73 2f23 616c 6275  transforms/#albu
+00003f80: 6d65 6e74 6174 696f 6e73 2e61 7567 6d65  mentations.augme
+00003f90: 6e74 6174 696f 6e73 2e62 6c75 722e 7472  ntations.blur.tr
+00003fa0: 616e 7366 6f72 6d73 2e4d 6f74 696f 6e42  ansforms.MotionB
+00003fb0: 6c75 7229 0a2d 205b 4d75 6c74 6970 6c69  lur).- [Multipli
+00003fc0: 6361 7469 7665 4e6f 6973 655d 2868 7474  cativeNoise](htt
+00003fd0: 7073 3a2f 2f61 6c62 756d 656e 7461 7469  ps://albumentati
+00003fe0: 6f6e 732e 6169 2f64 6f63 732f 6170 695f  ons.ai/docs/api_
+00003ff0: 7265 6665 7265 6e63 652f 6175 676d 656e  reference/augmen
+00004000: 7461 7469 6f6e 732f 7472 616e 7366 6f72  tations/transfor
+00004010: 6d73 2f23 616c 6275 6d65 6e74 6174 696f  ms/#albumentatio
+00004020: 6e73 2e61 7567 6d65 6e74 6174 696f 6e73  ns.augmentations
+00004030: 2e74 7261 6e73 666f 726d 732e 4d75 6c74  .transforms.Mult
+00004040: 6970 6c69 6361 7469 7665 4e6f 6973 6529  iplicativeNoise)
+00004050: 0a2d 205b 4e6f 726d 616c 697a 655d 2868  .- [Normalize](h
+00004060: 7474 7073 3a2f 2f61 6c62 756d 656e 7461  ttps://albumenta
+00004070: 7469 6f6e 732e 6169 2f64 6f63 732f 6170  tions.ai/docs/ap
+00004080: 695f 7265 6665 7265 6e63 652f 6175 676d  i_reference/augm
+00004090: 656e 7461 7469 6f6e 732f 7472 616e 7366  entations/transf
+000040a0: 6f72 6d73 2f23 616c 6275 6d65 6e74 6174  orms/#albumentat
+000040b0: 696f 6e73 2e61 7567 6d65 6e74 6174 696f  ions.augmentatio
+000040c0: 6e73 2e74 7261 6e73 666f 726d 732e 4e6f  ns.transforms.No
+000040d0: 726d 616c 697a 6529 0a2d 205b 5069 7865  rmalize).- [Pixe
+000040e0: 6c44 6973 7472 6962 7574 696f 6e41 6461  lDistributionAda
+000040f0: 7074 6174 696f 6e5d 2868 7474 7073 3a2f  ptation](https:/
+00004100: 2f61 6c62 756d 656e 7461 7469 6f6e 732e  /albumentations.
+00004110: 6169 2f64 6f63 732f 6170 695f 7265 6665  ai/docs/api_refe
+00004120: 7265 6e63 652f 6175 676d 656e 7461 7469  rence/augmentati
+00004130: 6f6e 732f 646f 6d61 696e 5f61 6461 7074  ons/domain_adapt
+00004140: 6174 696f 6e2f 2361 6c62 756d 656e 7461  ation/#albumenta
+00004150: 7469 6f6e 732e 6175 676d 656e 7461 7469  tions.augmentati
+00004160: 6f6e 732e 646f 6d61 696e 5f61 6461 7074  ons.domain_adapt
+00004170: 6174 696f 6e2e 5069 7865 6c44 6973 7472  ation.PixelDistr
+00004180: 6962 7574 696f 6e41 6461 7074 6174 696f  ibutionAdaptatio
+00004190: 6e29 0a2d 205b 506f 7374 6572 697a 655d  n).- [Posterize]
+000041a0: 2868 7474 7073 3a2f 2f61 6c62 756d 656e  (https://albumen
+000041b0: 7461 7469 6f6e 732e 6169 2f64 6f63 732f  tations.ai/docs/
+000041c0: 6170 695f 7265 6665 7265 6e63 652f 6175  api_reference/au
+000041d0: 676d 656e 7461 7469 6f6e 732f 7472 616e  gmentations/tran
+000041e0: 7366 6f72 6d73 2f23 616c 6275 6d65 6e74  sforms/#albument
+000041f0: 6174 696f 6e73 2e61 7567 6d65 6e74 6174  ations.augmentat
+00004200: 696f 6e73 2e74 7261 6e73 666f 726d 732e  ions.transforms.
+00004210: 506f 7374 6572 697a 6529 0a2d 205b 5247  Posterize).- [RG
+00004220: 4253 6869 6674 5d28 6874 7470 733a 2f2f  BShift](https://
+00004230: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
+00004240: 692f 646f 6373 2f61 7069 5f72 6566 6572  i/docs/api_refer
+00004250: 656e 6365 2f61 7567 6d65 6e74 6174 696f  ence/augmentatio
+00004260: 6e73 2f74 7261 6e73 666f 726d 732f 2361  ns/transforms/#a
+00004270: 6c62 756d 656e 7461 7469 6f6e 732e 6175  lbumentations.au
+00004280: 676d 656e 7461 7469 6f6e 732e 7472 616e  gmentations.tran
+00004290: 7366 6f72 6d73 2e52 4742 5368 6966 7429  sforms.RGBShift)
+000042a0: 0a2d 205b 5261 6e64 6f6d 4272 6967 6874  .- [RandomBright
+000042b0: 6e65 7373 436f 6e74 7261 7374 5d28 6874  nessContrast](ht
+000042c0: 7470 733a 2f2f 616c 6275 6d65 6e74 6174  tps://albumentat
+000042d0: 696f 6e73 2e61 692f 646f 6373 2f61 7069  ions.ai/docs/api
+000042e0: 5f72 6566 6572 656e 6365 2f61 7567 6d65  _reference/augme
+000042f0: 6e74 6174 696f 6e73 2f74 7261 6e73 666f  ntations/transfo
+00004300: 726d 732f 2361 6c62 756d 656e 7461 7469  rms/#albumentati
+00004310: 6f6e 732e 6175 676d 656e 7461 7469 6f6e  ons.augmentation
+00004320: 732e 7472 616e 7366 6f72 6d73 2e52 616e  s.transforms.Ran
+00004330: 646f 6d42 7269 6768 746e 6573 7343 6f6e  domBrightnessCon
+00004340: 7472 6173 7429 0a2d 205b 5261 6e64 6f6d  trast).- [Random
+00004350: 466f 675d 2868 7474 7073 3a2f 2f61 6c62  Fog](https://alb
+00004360: 756d 656e 7461 7469 6f6e 732e 6169 2f64  umentations.ai/d
+00004370: 6f63 732f 6170 695f 7265 6665 7265 6e63  ocs/api_referenc
+00004380: 652f 6175 676d 656e 7461 7469 6f6e 732f  e/augmentations/
+00004390: 7472 616e 7366 6f72 6d73 2f23 616c 6275  transforms/#albu
+000043a0: 6d65 6e74 6174 696f 6e73 2e61 7567 6d65  mentations.augme
+000043b0: 6e74 6174 696f 6e73 2e74 7261 6e73 666f  ntations.transfo
+000043c0: 726d 732e 5261 6e64 6f6d 466f 6729 0a2d  rms.RandomFog).-
+000043d0: 205b 5261 6e64 6f6d 4761 6d6d 615d 2868   [RandomGamma](h
+000043e0: 7474 7073 3a2f 2f61 6c62 756d 656e 7461  ttps://albumenta
+000043f0: 7469 6f6e 732e 6169 2f64 6f63 732f 6170  tions.ai/docs/ap
+00004400: 695f 7265 6665 7265 6e63 652f 6175 676d  i_reference/augm
+00004410: 656e 7461 7469 6f6e 732f 7472 616e 7366  entations/transf
+00004420: 6f72 6d73 2f23 616c 6275 6d65 6e74 6174  orms/#albumentat
+00004430: 696f 6e73 2e61 7567 6d65 6e74 6174 696f  ions.augmentatio
+00004440: 6e73 2e74 7261 6e73 666f 726d 732e 5261  ns.transforms.Ra
+00004450: 6e64 6f6d 4761 6d6d 6129 0a2d 205b 5261  ndomGamma).- [Ra
+00004460: 6e64 6f6d 4772 6176 656c 5d28 6874 7470  ndomGravel](http
+00004470: 733a 2f2f 616c 6275 6d65 6e74 6174 696f  s://albumentatio
+00004480: 6e73 2e61 692f 646f 6373 2f61 7069 5f72  ns.ai/docs/api_r
+00004490: 6566 6572 656e 6365 2f61 7567 6d65 6e74  eference/augment
+000044a0: 6174 696f 6e73 2f74 7261 6e73 666f 726d  ations/transform
+000044b0: 732f 2361 6c62 756d 656e 7461 7469 6f6e  s/#albumentation
+000044c0: 732e 6175 676d 656e 7461 7469 6f6e 732e  s.augmentations.
+000044d0: 7472 616e 7366 6f72 6d73 2e52 616e 646f  transforms.Rando
+000044e0: 6d47 7261 7665 6c29 0a2d 205b 5261 6e64  mGravel).- [Rand
+000044f0: 6f6d 5261 696e 5d28 6874 7470 733a 2f2f  omRain](https://
+00004500: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
+00004510: 692f 646f 6373 2f61 7069 5f72 6566 6572  i/docs/api_refer
+00004520: 656e 6365 2f61 7567 6d65 6e74 6174 696f  ence/augmentatio
+00004530: 6e73 2f74 7261 6e73 666f 726d 732f 2361  ns/transforms/#a
+00004540: 6c62 756d 656e 7461 7469 6f6e 732e 6175  lbumentations.au
+00004550: 676d 656e 7461 7469 6f6e 732e 7472 616e  gmentations.tran
+00004560: 7366 6f72 6d73 2e52 616e 646f 6d52 6169  sforms.RandomRai
+00004570: 6e29 0a2d 205b 5261 6e64 6f6d 5368 6164  n).- [RandomShad
+00004580: 6f77 5d28 6874 7470 733a 2f2f 616c 6275  ow](https://albu
+00004590: 6d65 6e74 6174 696f 6e73 2e61 692f 646f  mentations.ai/do
+000045a0: 6373 2f61 7069 5f72 6566 6572 656e 6365  cs/api_reference
+000045b0: 2f61 7567 6d65 6e74 6174 696f 6e73 2f74  /augmentations/t
+000045c0: 7261 6e73 666f 726d 732f 2361 6c62 756d  ransforms/#album
+000045d0: 656e 7461 7469 6f6e 732e 6175 676d 656e  entations.augmen
+000045e0: 7461 7469 6f6e 732e 7472 616e 7366 6f72  tations.transfor
+000045f0: 6d73 2e52 616e 646f 6d53 6861 646f 7729  ms.RandomShadow)
+00004600: 0a2d 205b 5261 6e64 6f6d 536e 6f77 5d28  .- [RandomSnow](
+00004610: 6874 7470 733a 2f2f 616c 6275 6d65 6e74  https://albument
+00004620: 6174 696f 6e73 2e61 692f 646f 6373 2f61  ations.ai/docs/a
+00004630: 7069 5f72 6566 6572 656e 6365 2f61 7567  pi_reference/aug
+00004640: 6d65 6e74 6174 696f 6e73 2f74 7261 6e73  mentations/trans
+00004650: 666f 726d 732f 2361 6c62 756d 656e 7461  forms/#albumenta
+00004660: 7469 6f6e 732e 6175 676d 656e 7461 7469  tions.augmentati
+00004670: 6f6e 732e 7472 616e 7366 6f72 6d73 2e52  ons.transforms.R
+00004680: 616e 646f 6d53 6e6f 7729 0a2d 205b 5261  andomSnow).- [Ra
+00004690: 6e64 6f6d 5375 6e46 6c61 7265 5d28 6874  ndomSunFlare](ht
+000046a0: 7470 733a 2f2f 616c 6275 6d65 6e74 6174  tps://albumentat
+000046b0: 696f 6e73 2e61 692f 646f 6373 2f61 7069  ions.ai/docs/api
+000046c0: 5f72 6566 6572 656e 6365 2f61 7567 6d65  _reference/augme
+000046d0: 6e74 6174 696f 6e73 2f74 7261 6e73 666f  ntations/transfo
+000046e0: 726d 732f 2361 6c62 756d 656e 7461 7469  rms/#albumentati
+000046f0: 6f6e 732e 6175 676d 656e 7461 7469 6f6e  ons.augmentation
+00004700: 732e 7472 616e 7366 6f72 6d73 2e52 616e  s.transforms.Ran
+00004710: 646f 6d53 756e 466c 6172 6529 0a2d 205b  domSunFlare).- [
+00004720: 5261 6e64 6f6d 546f 6e65 4375 7276 655d  RandomToneCurve]
+00004730: 2868 7474 7073 3a2f 2f61 6c62 756d 656e  (https://albumen
+00004740: 7461 7469 6f6e 732e 6169 2f64 6f63 732f  tations.ai/docs/
+00004750: 6170 695f 7265 6665 7265 6e63 652f 6175  api_reference/au
+00004760: 676d 656e 7461 7469 6f6e 732f 7472 616e  gmentations/tran
+00004770: 7366 6f72 6d73 2f23 616c 6275 6d65 6e74  sforms/#albument
+00004780: 6174 696f 6e73 2e61 7567 6d65 6e74 6174  ations.augmentat
+00004790: 696f 6e73 2e74 7261 6e73 666f 726d 732e  ions.transforms.
+000047a0: 5261 6e64 6f6d 546f 6e65 4375 7276 6529  RandomToneCurve)
+000047b0: 0a2d 205b 5269 6e67 696e 674f 7665 7273  .- [RingingOvers
+000047c0: 686f 6f74 5d28 6874 7470 733a 2f2f 616c  hoot](https://al
+000047d0: 6275 6d65 6e74 6174 696f 6e73 2e61 692f  bumentations.ai/
+000047e0: 646f 6373 2f61 7069 5f72 6566 6572 656e  docs/api_referen
+000047f0: 6365 2f61 7567 6d65 6e74 6174 696f 6e73  ce/augmentations
+00004800: 2f74 7261 6e73 666f 726d 732f 2361 6c62  /transforms/#alb
+00004810: 756d 656e 7461 7469 6f6e 732e 6175 676d  umentations.augm
+00004820: 656e 7461 7469 6f6e 732e 7472 616e 7366  entations.transf
+00004830: 6f72 6d73 2e52 696e 6769 6e67 4f76 6572  orms.RingingOver
+00004840: 7368 6f6f 7429 0a2d 205b 5368 6172 7065  shoot).- [Sharpe
+00004850: 6e5d 2868 7474 7073 3a2f 2f61 6c62 756d  n](https://album
+00004860: 656e 7461 7469 6f6e 732e 6169 2f64 6f63  entations.ai/doc
+00004870: 732f 6170 695f 7265 6665 7265 6e63 652f  s/api_reference/
+00004880: 6175 676d 656e 7461 7469 6f6e 732f 7472  augmentations/tr
+00004890: 616e 7366 6f72 6d73 2f23 616c 6275 6d65  ansforms/#albume
+000048a0: 6e74 6174 696f 6e73 2e61 7567 6d65 6e74  ntations.augment
+000048b0: 6174 696f 6e73 2e74 7261 6e73 666f 726d  ations.transform
+000048c0: 732e 5368 6172 7065 6e29 0a2d 205b 536f  s.Sharpen).- [So
+000048d0: 6c61 7269 7a65 5d28 6874 7470 733a 2f2f  larize](https://
+000048e0: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
+000048f0: 692f 646f 6373 2f61 7069 5f72 6566 6572  i/docs/api_refer
+00004900: 656e 6365 2f61 7567 6d65 6e74 6174 696f  ence/augmentatio
+00004910: 6e73 2f74 7261 6e73 666f 726d 732f 2361  ns/transforms/#a
+00004920: 6c62 756d 656e 7461 7469 6f6e 732e 6175  lbumentations.au
+00004930: 676d 656e 7461 7469 6f6e 732e 7472 616e  gmentations.tran
+00004940: 7366 6f72 6d73 2e53 6f6c 6172 697a 6529  sforms.Solarize)
+00004950: 0a2d 205b 5370 6174 7465 725d 2868 7474  .- [Spatter](htt
+00004960: 7073 3a2f 2f61 6c62 756d 656e 7461 7469  ps://albumentati
+00004970: 6f6e 732e 6169 2f64 6f63 732f 6170 695f  ons.ai/docs/api_
+00004980: 7265 6665 7265 6e63 652f 6175 676d 656e  reference/augmen
+00004990: 7461 7469 6f6e 732f 7472 616e 7366 6f72  tations/transfor
+000049a0: 6d73 2f23 616c 6275 6d65 6e74 6174 696f  ms/#albumentatio
+000049b0: 6e73 2e61 7567 6d65 6e74 6174 696f 6e73  ns.augmentations
+000049c0: 2e74 7261 6e73 666f 726d 732e 5370 6174  .transforms.Spat
+000049d0: 7465 7229 0a2d 205b 5375 7065 7270 6978  ter).- [Superpix
+000049e0: 656c 735d 2868 7474 7073 3a2f 2f61 6c62  els](https://alb
+000049f0: 756d 656e 7461 7469 6f6e 732e 6169 2f64  umentations.ai/d
+00004a00: 6f63 732f 6170 695f 7265 6665 7265 6e63  ocs/api_referenc
+00004a10: 652f 6175 676d 656e 7461 7469 6f6e 732f  e/augmentations/
+00004a20: 7472 616e 7366 6f72 6d73 2f23 616c 6275  transforms/#albu
+00004a30: 6d65 6e74 6174 696f 6e73 2e61 7567 6d65  mentations.augme
+00004a40: 6e74 6174 696f 6e73 2e74 7261 6e73 666f  ntations.transfo
+00004a50: 726d 732e 5375 7065 7270 6978 656c 7329  rms.Superpixels)
+00004a60: 0a2d 205b 5465 6d70 6c61 7465 5472 616e  .- [TemplateTran
+00004a70: 7366 6f72 6d5d 2868 7474 7073 3a2f 2f61  sform](https://a
+00004a80: 6c62 756d 656e 7461 7469 6f6e 732e 6169  lbumentations.ai
+00004a90: 2f64 6f63 732f 6170 695f 7265 6665 7265  /docs/api_refere
+00004aa0: 6e63 652f 6175 676d 656e 7461 7469 6f6e  nce/augmentation
+00004ab0: 732f 7472 616e 7366 6f72 6d73 2f23 616c  s/transforms/#al
+00004ac0: 6275 6d65 6e74 6174 696f 6e73 2e61 7567  bumentations.aug
+00004ad0: 6d65 6e74 6174 696f 6e73 2e74 7261 6e73  mentations.trans
+00004ae0: 666f 726d 732e 5465 6d70 6c61 7465 5472  forms.TemplateTr
+00004af0: 616e 7366 6f72 6d29 0a2d 205b 546f 466c  ansform).- [ToFl
+00004b00: 6f61 745d 2868 7474 7073 3a2f 2f61 6c62  oat](https://alb
+00004b10: 756d 656e 7461 7469 6f6e 732e 6169 2f64  umentations.ai/d
+00004b20: 6f63 732f 6170 695f 7265 6665 7265 6e63  ocs/api_referenc
+00004b30: 652f 6175 676d 656e 7461 7469 6f6e 732f  e/augmentations/
+00004b40: 7472 616e 7366 6f72 6d73 2f23 616c 6275  transforms/#albu
+00004b50: 6d65 6e74 6174 696f 6e73 2e61 7567 6d65  mentations.augme
+00004b60: 6e74 6174 696f 6e73 2e74 7261 6e73 666f  ntations.transfo
+00004b70: 726d 732e 546f 466c 6f61 7429 0a2d 205b  rms.ToFloat).- [
+00004b80: 546f 4772 6179 5d28 6874 7470 733a 2f2f  ToGray](https://
+00004b90: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
+00004ba0: 692f 646f 6373 2f61 7069 5f72 6566 6572  i/docs/api_refer
+00004bb0: 656e 6365 2f61 7567 6d65 6e74 6174 696f  ence/augmentatio
+00004bc0: 6e73 2f74 7261 6e73 666f 726d 732f 2361  ns/transforms/#a
+00004bd0: 6c62 756d 656e 7461 7469 6f6e 732e 6175  lbumentations.au
+00004be0: 676d 656e 7461 7469 6f6e 732e 7472 616e  gmentations.tran
+00004bf0: 7366 6f72 6d73 2e54 6f47 7261 7929 0a2d  sforms.ToGray).-
+00004c00: 205b 546f 5247 425d 2868 7474 7073 3a2f   [ToRGB](https:/
+00004c10: 2f61 6c62 756d 656e 7461 7469 6f6e 732e  /albumentations.
+00004c20: 6169 2f64 6f63 732f 6170 695f 7265 6665  ai/docs/api_refe
+00004c30: 7265 6e63 652f 6175 676d 656e 7461 7469  rence/augmentati
+00004c40: 6f6e 732f 7472 616e 7366 6f72 6d73 2f23  ons/transforms/#
+00004c50: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
+00004c60: 7567 6d65 6e74 6174 696f 6e73 2e74 7261  ugmentations.tra
+00004c70: 6e73 666f 726d 732e 546f 5247 4229 0a2d  nsforms.ToRGB).-
+00004c80: 205b 546f 5365 7069 615d 2868 7474 7073   [ToSepia](https
+00004c90: 3a2f 2f61 6c62 756d 656e 7461 7469 6f6e  ://albumentation
+00004ca0: 732e 6169 2f64 6f63 732f 6170 695f 7265  s.ai/docs/api_re
+00004cb0: 6665 7265 6e63 652f 6175 676d 656e 7461  ference/augmenta
+00004cc0: 7469 6f6e 732f 7472 616e 7366 6f72 6d73  tions/transforms
+00004cd0: 2f23 616c 6275 6d65 6e74 6174 696f 6e73  /#albumentations
+00004ce0: 2e61 7567 6d65 6e74 6174 696f 6e73 2e74  .augmentations.t
+00004cf0: 7261 6e73 666f 726d 732e 546f 5365 7069  ransforms.ToSepi
+00004d00: 6129 0a2d 205b 556e 7368 6172 704d 6173  a).- [UnsharpMas
+00004d10: 6b5d 2868 7474 7073 3a2f 2f61 6c62 756d  k](https://album
+00004d20: 656e 7461 7469 6f6e 732e 6169 2f64 6f63  entations.ai/doc
+00004d30: 732f 6170 695f 7265 6665 7265 6e63 652f  s/api_reference/
+00004d40: 6175 676d 656e 7461 7469 6f6e 732f 7472  augmentations/tr
+00004d50: 616e 7366 6f72 6d73 2f23 616c 6275 6d65  ansforms/#albume
+00004d60: 6e74 6174 696f 6e73 2e61 7567 6d65 6e74  ntations.augment
+00004d70: 6174 696f 6e73 2e74 7261 6e73 666f 726d  ations.transform
+00004d80: 732e 556e 7368 6172 704d 6173 6b29 0a2d  s.UnsharpMask).-
+00004d90: 205b 5a6f 6f6d 426c 7572 5d28 6874 7470   [ZoomBlur](http
+00004da0: 733a 2f2f 616c 6275 6d65 6e74 6174 696f  s://albumentatio
+00004db0: 6e73 2e61 692f 646f 6373 2f61 7069 5f72  ns.ai/docs/api_r
+00004dc0: 6566 6572 656e 6365 2f61 7567 6d65 6e74  eference/augment
+00004dd0: 6174 696f 6e73 2f62 6c75 722f 7472 616e  ations/blur/tran
+00004de0: 7366 6f72 6d73 2f23 616c 6275 6d65 6e74  sforms/#albument
+00004df0: 6174 696f 6e73 2e61 7567 6d65 6e74 6174  ations.augmentat
+00004e00: 696f 6e73 2e62 6c75 722e 7472 616e 7366  ions.blur.transf
+00004e10: 6f72 6d73 2e5a 6f6f 6d42 6c75 7229 0a0a  orms.ZoomBlur)..
+00004e20: 2323 2320 5370 6174 6961 6c2d 6c65 7665  ### Spatial-leve
+00004e30: 6c20 7472 616e 7366 6f72 6d73 0a0a 5370  l transforms..Sp
+00004e40: 6174 6961 6c2d 6c65 7665 6c20 7472 616e  atial-level tran
+00004e50: 7366 6f72 6d73 2077 696c 6c20 7369 6d75  sforms will simu
+00004e60: 6c74 616e 656f 7573 6c79 2063 6861 6e67  ltaneously chang
+00004e70: 6520 626f 7468 2061 6e20 696e 7075 7420  e both an input 
+00004e80: 696d 6167 6520 6173 2077 656c 6c20 6173  image as well as
+00004e90: 2061 6464 6974 696f 6e61 6c20 7461 7267   additional targ
+00004ea0: 6574 7320 7375 6368 2061 7320 6d61 736b  ets such as mask
+00004eb0: 732c 2062 6f75 6e64 696e 6720 626f 7865  s, bounding boxe
+00004ec0: 732c 2061 6e64 206b 6579 706f 696e 7473  s, and keypoints
+00004ed0: 2e20 5468 6520 666f 6c6c 6f77 696e 6720  . The following 
+00004ee0: 7461 626c 6520 7368 6f77 7320 7768 6963  table shows whic
+00004ef0: 6820 6164 6469 7469 6f6e 616c 2074 6172  h additional tar
+00004f00: 6765 7473 2061 7265 2073 7570 706f 7274  gets are support
+00004f10: 6564 2062 7920 6561 6368 2074 7261 6e73  ed by each trans
+00004f20: 666f 726d 2e0a 0a7c 2054 7261 6e73 666f  form...| Transfo
+00004f30: 726d 2020 2020 2020 2020 2020 2020 2020  rm              
+00004f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004fd0: 2020 2020 2020 2020 207c 2049 6d61 6765           | Image
+00004fe0: 207c 204d 6173 6b20 7c20 4242 6f78 6573   | Mask | BBoxes
+00004ff0: 207c 204b 6579 706f 696e 7473 207c 0a7c   | Keypoints |.|
+00005000: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+00005010: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005020: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005030: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005040: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005050: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005060: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005070: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005080: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005090: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000050a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000050b0: 207c 203a 2d2d 2d3a 207c 203a 2d2d 3a20   | :---: | :--: 
+000050c0: 7c20 3a2d 2d2d 2d3a 207c 203a 2d2d 2d2d  | :----: | :----
+000050d0: 2d2d 2d3a 207c 0a7c 205b 4166 6669 6e65  ---: |.| [Affine
+000050e0: 5d28 6874 7470 733a 2f2f 616c 6275 6d65  ](https://albume
+000050f0: 6e74 6174 696f 6e73 2e61 692f 646f 6373  ntations.ai/docs
+00005100: 2f61 7069 5f72 6566 6572 656e 6365 2f61  /api_reference/a
+00005110: 7567 6d65 6e74 6174 696f 6e73 2f67 656f  ugmentations/geo
+00005120: 6d65 7472 6963 2f74 7261 6e73 666f 726d  metric/transform
+00005130: 732f 2361 6c62 756d 656e 7461 7469 6f6e  s/#albumentation
+00005140: 732e 6175 676d 656e 7461 7469 6f6e 732e  s.augmentations.
+00005150: 6765 6f6d 6574 7269 632e 7472 616e 7366  geometric.transf
+00005160: 6f72 6d73 2e41 6666 696e 6529 2020 2020  orms.Affine)    
+00005170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005180: 2020 2020 2020 2020 207c 20e2 9c93 2020           | ...  
+00005190: 2020 207c 20e2 9c93 2020 2020 7c20 e29c     | ...    | ..
+000051a0: 9320 2020 2020 207c 20e2 9c93 2020 2020  .      | ...    
+000051b0: 2020 2020 207c 0a7c 205b 4242 6f78 5361       |.| [BBoxSa
+000051c0: 6665 5261 6e64 6f6d 4372 6f70 5d28 6874  feRandomCrop](ht
+000051d0: 7470 733a 2f2f 616c 6275 6d65 6e74 6174  tps://albumentat
+000051e0: 696f 6e73 2e61 692f 646f 6373 2f61 7069  ions.ai/docs/api
+000051f0: 5f72 6566 6572 656e 6365 2f61 7567 6d65  _reference/augme
+00005200: 6e74 6174 696f 6e73 2f63 726f 7073 2f74  ntations/crops/t
+00005210: 7261 6e73 666f 726d 732f 2361 6c62 756d  ransforms/#album
+00005220: 656e 7461 7469 6f6e 732e 6175 676d 656e  entations.augmen
+00005230: 7461 7469 6f6e 732e 6372 6f70 732e 7472  tations.crops.tr
+00005240: 616e 7366 6f72 6d73 2e42 426f 7853 6166  ansforms.BBoxSaf
+00005250: 6552 616e 646f 6d43 726f 7029 2020 2020  eRandomCrop)    
+00005260: 2020 2020 2020 2020 207c 20e2 9c93 2020           | ...  
+00005270: 2020 207c 20e2 9c93 2020 2020 7c20 e29c     | ...    | ..
+00005280: 9320 2020 2020 207c 2020 2020 2020 2020  .      |        
+00005290: 2020 207c 0a7c 205b 4365 6e74 6572 4372     |.| [CenterCr
+000052a0: 6f70 5d28 6874 7470 733a 2f2f 616c 6275  op](https://albu
+000052b0: 6d65 6e74 6174 696f 6e73 2e61 692f 646f  mentations.ai/do
+000052c0: 6373 2f61 7069 5f72 6566 6572 656e 6365  cs/api_reference
+000052d0: 2f61 7567 6d65 6e74 6174 696f 6e73 2f63  /augmentations/c
+000052e0: 726f 7073 2f74 7261 6e73 666f 726d 732f  rops/transforms/
+000052f0: 2361 6c62 756d 656e 7461 7469 6f6e 732e  #albumentations.
+00005300: 6175 676d 656e 7461 7469 6f6e 732e 6372  augmentations.cr
+00005310: 6f70 732e 7472 616e 7366 6f72 6d73 2e43  ops.transforms.C
+00005320: 656e 7465 7243 726f 7029 2020 2020 2020  enterCrop)      
+00005330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005340: 2020 2020 2020 207c 20e2 9c93 2020 2020         | ...    
+00005350: 207c 20e2 9c93 2020 2020 7c20 e29c 9320   | ...    | ... 
+00005360: 2020 2020 207c 20e2 9c93 2020 2020 2020       | ...      
+00005370: 2020 207c 0a7c 205b 436f 6172 7365 4472     |.| [CoarseDr
+00005380: 6f70 6f75 745d 2868 7474 7073 3a2f 2f61  opout](https://a
+00005390: 6c62 756d 656e 7461 7469 6f6e 732e 6169  lbumentations.ai
+000053a0: 2f64 6f63 732f 6170 695f 7265 6665 7265  /docs/api_refere
+000053b0: 6e63 652f 6175 676d 656e 7461 7469 6f6e  nce/augmentation
+000053c0: 732f 6472 6f70 6f75 742f 636f 6172 7365  s/dropout/coarse
+000053d0: 5f64 726f 706f 7574 2f23 616c 6275 6d65  _dropout/#albume
+000053e0: 6e74 6174 696f 6e73 2e61 7567 6d65 6e74  ntations.augment
+000053f0: 6174 696f 6e73 2e64 726f 706f 7574 2e63  ations.dropout.c
+00005400: 6f61 7273 655f 6472 6f70 6f75 742e 436f  oarse_dropout.Co
+00005410: 6172 7365 4472 6f70 6f75 7429 2020 2020  arseDropout)    
+00005420: 2020 2020 2020 207c 20e2 9c93 2020 2020         | ...    
+00005430: 207c 20e2 9c93 2020 2020 7c20 2020 2020   | ...    |     
+00005440: 2020 207c 20e2 9c93 2020 2020 2020 2020     | ...        
+00005450: 207c 0a7c 205b 4372 6f70 5d28 6874 7470   |.| [Crop](http
+00005460: 733a 2f2f 616c 6275 6d65 6e74 6174 696f  s://albumentatio
+00005470: 6e73 2e61 692f 646f 6373 2f61 7069 5f72  ns.ai/docs/api_r
+00005480: 6566 6572 656e 6365 2f61 7567 6d65 6e74  eference/augment
+00005490: 6174 696f 6e73 2f63 726f 7073 2f74 7261  ations/crops/tra
+000054a0: 6e73 666f 726d 732f 2361 6c62 756d 656e  nsforms/#albumen
+000054b0: 7461 7469 6f6e 732e 6175 676d 656e 7461  tations.augmenta
+000054c0: 7469 6f6e 732e 6372 6f70 732e 7472 616e  tions.crops.tran
+000054d0: 7366 6f72 6d73 2e43 726f 7029 2020 2020  sforms.Crop)    
+000054e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000054f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005500: 2020 2020 207c 20e2 9c93 2020 2020 207c       | ...     |
+00005510: 20e2 9c93 2020 2020 7c20 e29c 9320 2020   ...    | ...   
+00005520: 2020 207c 20e2 9c93 2020 2020 2020 2020     | ...        
+00005530: 207c 0a7c 205b 4372 6f70 416e 6450 6164   |.| [CropAndPad
+00005540: 5d28 6874 7470 733a 2f2f 616c 6275 6d65  ](https://albume
+00005550: 6e74 6174 696f 6e73 2e61 692f 646f 6373  ntations.ai/docs
+00005560: 2f61 7069 5f72 6566 6572 656e 6365 2f61  /api_reference/a
+00005570: 7567 6d65 6e74 6174 696f 6e73 2f63 726f  ugmentations/cro
+00005580: 7073 2f74 7261 6e73 666f 726d 732f 2361  ps/transforms/#a
+00005590: 6c62 756d 656e 7461 7469 6f6e 732e 6175  lbumentations.au
+000055a0: 676d 656e 7461 7469 6f6e 732e 6372 6f70  gmentations.crop
+000055b0: 732e 7472 616e 7366 6f72 6d73 2e43 726f  s.transforms.Cro
+000055c0: 7041 6e64 5061 6429 2020 2020 2020 2020  pAndPad)        
+000055d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000055e0: 2020 2020 207c 20e2 9c93 2020 2020 207c       | ...     |
+000055f0: 20e2 9c93 2020 2020 7c20 e29c 9320 2020   ...    | ...   
+00005600: 2020 207c 20e2 9c93 2020 2020 2020 2020     | ...        
+00005610: 207c 0a7c 205b 4372 6f70 4e6f 6e45 6d70   |.| [CropNonEmp
+00005620: 7479 4d61 736b 4966 4578 6973 7473 5d28  tyMaskIfExists](
+00005630: 6874 7470 733a 2f2f 616c 6275 6d65 6e74  https://albument
+00005640: 6174 696f 6e73 2e61 692f 646f 6373 2f61  ations.ai/docs/a
+00005650: 7069 5f72 6566 6572 656e 6365 2f61 7567  pi_reference/aug
+00005660: 6d65 6e74 6174 696f 6e73 2f63 726f 7073  mentations/crops
+00005670: 2f74 7261 6e73 666f 726d 732f 2361 6c62  /transforms/#alb
+00005680: 756d 656e 7461 7469 6f6e 732e 6175 676d  umentations.augm
+00005690: 656e 7461 7469 6f6e 732e 6372 6f70 732e  entations.crops.
+000056a0: 7472 616e 7366 6f72 6d73 2e43 726f 704e  transforms.CropN
+000056b0: 6f6e 456d 7074 794d 6173 6b49 6645 7869  onEmptyMaskIfExi
+000056c0: 7374 7329 207c 20e2 9c93 2020 2020 207c  sts) | ...     |
+000056d0: 20e2 9c93 2020 2020 7c20 e29c 9320 2020   ...    | ...   
+000056e0: 2020 207c 20e2 9c93 2020 2020 2020 2020     | ...        
+000056f0: 207c 0a7c 205b 456c 6173 7469 6354 7261   |.| [ElasticTra
+00005700: 6e73 666f 726d 5d28 6874 7470 733a 2f2f  nsform](https://
+00005710: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
+00005720: 692f 646f 6373 2f61 7069 5f72 6566 6572  i/docs/api_refer
+00005730: 656e 6365 2f61 7567 6d65 6e74 6174 696f  ence/augmentatio
+00005740: 6e73 2f67 656f 6d65 7472 6963 2f74 7261  ns/geometric/tra
+00005750: 6e73 666f 726d 732f 2361 6c62 756d 656e  nsforms/#albumen
+00005760: 7461 7469 6f6e 732e 6175 676d 656e 7461  tations.augmenta
+00005770: 7469 6f6e 732e 6765 6f6d 6574 7269 632e  tions.geometric.
+00005780: 7472 616e 7366 6f72 6d73 2e45 6c61 7374  transforms.Elast
+00005790: 6963 5472 616e 7366 6f72 6d29 2020 2020  icTransform)    
+000057a0: 2020 2020 207c 20e2 9c93 2020 2020 207c       | ...     |
+000057b0: 20e2 9c93 2020 2020 7c20 e29c 9320 2020   ...    | ...   
+000057c0: 2020 207c 2020 2020 2020 2020 2020 207c     |           |
+000057d0: 0a7c 205b 466c 6970 5d28 6874 7470 733a  .| [Flip](https:
+000057e0: 2f2f 616c 6275 6d65 6e74 6174 696f 6e73  //albumentations
+000057f0: 2e61 692f 646f 6373 2f61 7069 5f72 6566  .ai/docs/api_ref
+00005800: 6572 656e 6365 2f61 7567 6d65 6e74 6174  erence/augmentat
+00005810: 696f 6e73 2f67 656f 6d65 7472 6963 2f74  ions/geometric/t
+00005820: 7261 6e73 666f 726d 732f 2361 6c62 756d  ransforms/#album
+00005830: 656e 7461 7469 6f6e 732e 6175 676d 656e  entations.augmen
+00005840: 7461 7469 6f6e 732e 6765 6f6d 6574 7269  tations.geometri
+00005850: 632e 7472 616e 7366 6f72 6d73 2e46 6c69  c.transforms.Fli
+00005860: 7029 2020 2020 2020 2020 2020 2020 2020  p)              
+00005870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005880: 2020 207c 20e2 9c93 2020 2020 207c 20e2     | ...     | .
+00005890: 9c93 2020 2020 7c20 e29c 9320 2020 2020  ..    | ...     
+000058a0: 207c 20e2 9c93 2020 2020 2020 2020 207c   | ...         |
+000058b0: 0a7c 205b 4772 6964 4469 7374 6f72 7469  .| [GridDistorti
+000058c0: 6f6e 5d28 6874 7470 733a 2f2f 616c 6275  on](https://albu
+000058d0: 6d65 6e74 6174 696f 6e73 2e61 692f 646f  mentations.ai/do
+000058e0: 6373 2f61 7069 5f72 6566 6572 656e 6365  cs/api_reference
+000058f0: 2f61 7567 6d65 6e74 6174 696f 6e73 2f67  /augmentations/g
+00005900: 656f 6d65 7472 6963 2f74 7261 6e73 666f  eometric/transfo
+00005910: 726d 732f 2361 6c62 756d 656e 7461 7469  rms/#albumentati
+00005920: 6f6e 732e 6175 676d 656e 7461 7469 6f6e  ons.augmentation
+00005930: 732e 6765 6f6d 6574 7269 632e 7472 616e  s.geometric.tran
+00005940: 7366 6f72 6d73 2e47 7269 6444 6973 746f  sforms.GridDisto
+00005950: 7274 696f 6e29 2020 2020 2020 2020 2020  rtion)          
+00005960: 2020 207c 20e2 9c93 2020 2020 207c 20e2     | ...     | .
+00005970: 9c93 2020 2020 7c20 e29c 9320 2020 2020  ..    | ...     
+00005980: 207c 2020 2020 2020 2020 2020 207c 0a7c   |           |.|
+00005990: 205b 4772 6964 4472 6f70 6f75 745d 2868   [GridDropout](h
+000059a0: 7474 7073 3a2f 2f61 6c62 756d 656e 7461  ttps://albumenta
+000059b0: 7469 6f6e 732e 6169 2f64 6f63 732f 6170  tions.ai/docs/ap
+000059c0: 695f 7265 6665 7265 6e63 652f 6175 676d  i_reference/augm
+000059d0: 656e 7461 7469 6f6e 732f 6472 6f70 6f75  entations/dropou
+000059e0: 742f 6772 6964 5f64 726f 706f 7574 2f23  t/grid_dropout/#
+000059f0: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
+00005a00: 7567 6d65 6e74 6174 696f 6e73 2e64 726f  ugmentations.dro
+00005a10: 706f 7574 2e67 7269 645f 6472 6f70 6f75  pout.grid_dropou
+00005a20: 742e 4772 6964 4472 6f70 6f75 7429 2020  t.GridDropout)  
+00005a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a40: 207c 20e2 9c93 2020 2020 207c 20e2 9c93   | ...     | ...
+00005a50: 2020 2020 7c20 2020 2020 2020 207c 2020      |        |  
+00005a60: 2020 2020 2020 2020 207c 0a7c 205b 486f           |.| [Ho
+00005a70: 7269 7a6f 6e74 616c 466c 6970 5d28 6874  rizontalFlip](ht
+00005a80: 7470 733a 2f2f 616c 6275 6d65 6e74 6174  tps://albumentat
+00005a90: 696f 6e73 2e61 692f 646f 6373 2f61 7069  ions.ai/docs/api
+00005aa0: 5f72 6566 6572 656e 6365 2f61 7567 6d65  _reference/augme
+00005ab0: 6e74 6174 696f 6e73 2f67 656f 6d65 7472  ntations/geometr
+00005ac0: 6963 2f74 7261 6e73 666f 726d 732f 2361  ic/transforms/#a
+00005ad0: 6c62 756d 656e 7461 7469 6f6e 732e 6175  lbumentations.au
+00005ae0: 676d 656e 7461 7469 6f6e 732e 6765 6f6d  gmentations.geom
+00005af0: 6574 7269 632e 7472 616e 7366 6f72 6d73  etric.transforms
+00005b00: 2e48 6f72 697a 6f6e 7461 6c46 6c69 7029  .HorizontalFlip)
+00005b10: 2020 2020 2020 2020 2020 2020 207c 20e2               | .
+00005b20: 9c93 2020 2020 207c 20e2 9c93 2020 2020  ..     | ...    
+00005b30: 7c20 e29c 9320 2020 2020 207c 20e2 9c93  | ...      | ...
+00005b40: 2020 2020 2020 2020 207c 0a7c 205b 4c61           |.| [La
+00005b50: 6d62 6461 5d28 6874 7470 733a 2f2f 616c  mbda](https://al
+00005b60: 6275 6d65 6e74 6174 696f 6e73 2e61 692f  bumentations.ai/
+00005b70: 646f 6373 2f61 7069 5f72 6566 6572 656e  docs/api_referen
+00005b80: 6365 2f61 7567 6d65 6e74 6174 696f 6e73  ce/augmentations
+00005b90: 2f74 7261 6e73 666f 726d 732f 2361 6c62  /transforms/#alb
+00005ba0: 756d 656e 7461 7469 6f6e 732e 6175 676d  umentations.augm
+00005bb0: 656e 7461 7469 6f6e 732e 7472 616e 7366  entations.transf
+00005bc0: 6f72 6d73 2e4c 616d 6264 6129 2020 2020  orms.Lambda)    
 00005bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005be0: 7c20 e29c 9320 2020 2020 7c20 e29c 9320  | ...     | ... 
-00005bf0: 2020 207c 2020 2020 2020 2020 7c20 2020     |        |   
-00005c00: 2020 2020 2020 2020 7c0a 7c20 5b52 616e          |.| [Ran
-00005c10: 646f 6d43 726f 705d 2868 7474 7073 3a2f  domCrop](https:/
-00005c20: 2f61 6c62 756d 656e 7461 7469 6f6e 732e  /albumentations.
-00005c30: 6169 2f64 6f63 732f 6170 695f 7265 6665  ai/docs/api_refe
-00005c40: 7265 6e63 652f 6175 676d 656e 7461 7469  rence/augmentati
-00005c50: 6f6e 732f 6372 6f70 732f 7472 616e 7366  ons/crops/transf
-00005c60: 6f72 6d73 2f23 616c 6275 6d65 6e74 6174  orms/#albumentat
-00005c70: 696f 6e73 2e61 7567 6d65 6e74 6174 696f  ions.augmentatio
-00005c80: 6e73 2e63 726f 7073 2e74 7261 6e73 666f  ns.crops.transfo
-00005c90: 726d 732e 5261 6e64 6f6d 4372 6f70 2920  rms.RandomCrop) 
-00005ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005cb0: 2020 2020 2020 2020 2020 2020 7c20 e29c              | ..
-00005cc0: 9320 2020 2020 7c20 e29c 9320 2020 207c  .     | ...    |
-00005cd0: 20e2 9c93 2020 2020 2020 7c20 e29c 9320   ...      | ... 
-00005ce0: 2020 2020 2020 2020 7c0a 7c20 5b52 616e          |.| [Ran
-00005cf0: 646f 6d43 726f 7046 726f 6d42 6f72 6465  domCropFromBorde
-00005d00: 7273 5d28 6874 7470 733a 2f2f 616c 6275  rs](https://albu
-00005d10: 6d65 6e74 6174 696f 6e73 2e61 692f 646f  mentations.ai/do
-00005d20: 6373 2f61 7069 5f72 6566 6572 656e 6365  cs/api_reference
-00005d30: 2f61 7567 6d65 6e74 6174 696f 6e73 2f63  /augmentations/c
-00005d40: 726f 7073 2f74 7261 6e73 666f 726d 732f  rops/transforms/
-00005d50: 2361 6c62 756d 656e 7461 7469 6f6e 732e  #albumentations.
-00005d60: 6175 676d 656e 7461 7469 6f6e 732e 6372  augmentations.cr
-00005d70: 6f70 732e 7472 616e 7366 6f72 6d73 2e52  ops.transforms.R
-00005d80: 616e 646f 6d43 726f 7046 726f 6d42 6f72  andomCropFromBor
-00005d90: 6465 7273 2920 2020 2020 2020 7c20 e29c  ders)       | ..
-00005da0: 9320 2020 2020 7c20 e29c 9320 2020 207c  .     | ...    |
-00005db0: 20e2 9c93 2020 2020 2020 7c20 e29c 9320   ...      | ... 
-00005dc0: 2020 2020 2020 2020 7c0a 7c20 5b52 616e          |.| [Ran
-00005dd0: 646f 6d43 726f 704e 6561 7242 426f 785d  domCropNearBBox]
-00005de0: 2868 7474 7073 3a2f 2f61 6c62 756d 656e  (https://albumen
-00005df0: 7461 7469 6f6e 732e 6169 2f64 6f63 732f  tations.ai/docs/
-00005e00: 6170 695f 7265 6665 7265 6e63 652f 6175  api_reference/au
-00005e10: 676d 656e 7461 7469 6f6e 732f 6372 6f70  gmentations/crop
-00005e20: 732f 7472 616e 7366 6f72 6d73 2f23 616c  s/transforms/#al
-00005e30: 6275 6d65 6e74 6174 696f 6e73 2e61 7567  bumentations.aug
-00005e40: 6d65 6e74 6174 696f 6e73 2e63 726f 7073  mentations.crops
-00005e50: 2e74 7261 6e73 666f 726d 732e 5261 6e64  .transforms.Rand
-00005e60: 6f6d 4372 6f70 4e65 6172 4242 6f78 2920  omCropNearBBox) 
-00005e70: 2020 2020 2020 2020 2020 2020 7c20 e29c              | ..
-00005e80: 9320 2020 2020 7c20 e29c 9320 2020 207c  .     | ...    |
-00005e90: 20e2 9c93 2020 2020 2020 7c20 e29c 9320   ...      | ... 
-00005ea0: 2020 2020 2020 2020 7c0a 7c20 5b52 616e          |.| [Ran
-00005eb0: 646f 6d47 7269 6453 6875 6666 6c65 5d28  domGridShuffle](
-00005ec0: 6874 7470 733a 2f2f 616c 6275 6d65 6e74  https://albument
-00005ed0: 6174 696f 6e73 2e61 692f 646f 6373 2f61  ations.ai/docs/a
-00005ee0: 7069 5f72 6566 6572 656e 6365 2f61 7567  pi_reference/aug
-00005ef0: 6d65 6e74 6174 696f 6e73 2f74 7261 6e73  mentations/trans
-00005f00: 666f 726d 732f 2361 6c62 756d 656e 7461  forms/#albumenta
-00005f10: 7469 6f6e 732e 6175 676d 656e 7461 7469  tions.augmentati
-00005f20: 6f6e 732e 7472 616e 7366 6f72 6d73 2e52  ons.transforms.R
-00005f30: 616e 646f 6d47 7269 6453 6875 6666 6c65  andomGridShuffle
-00005f40: 2920 2020 2020 2020 2020 2020 2020 2020  )               
-00005f50: 2020 2020 2020 2020 2020 2020 7c20 e29c              | ..
-00005f60: 9320 2020 2020 7c20 e29c 9320 2020 207c  .     | ...    |
-00005f70: 2020 2020 2020 2020 7c20 e29c 9320 2020          | ...   
-00005f80: 2020 2020 2020 7c0a 7c20 5b52 616e 646f        |.| [Rando
-00005f90: 6d52 6573 697a 6564 4372 6f70 5d28 6874  mResizedCrop](ht
-00005fa0: 7470 733a 2f2f 616c 6275 6d65 6e74 6174  tps://albumentat
-00005fb0: 696f 6e73 2e61 692f 646f 6373 2f61 7069  ions.ai/docs/api
-00005fc0: 5f72 6566 6572 656e 6365 2f61 7567 6d65  _reference/augme
-00005fd0: 6e74 6174 696f 6e73 2f63 726f 7073 2f74  ntations/crops/t
-00005fe0: 7261 6e73 666f 726d 732f 2361 6c62 756d  ransforms/#album
-00005ff0: 656e 7461 7469 6f6e 732e 6175 676d 656e  entations.augmen
-00006000: 7461 7469 6f6e 732e 6372 6f70 732e 7472  tations.crops.tr
-00006010: 616e 7366 6f72 6d73 2e52 616e 646f 6d52  ansforms.RandomR
-00006020: 6573 697a 6564 4372 6f70 2920 2020 2020  esizedCrop)     
-00006030: 2020 2020 2020 2020 2020 7c20 e29c 9320            | ... 
-00006040: 2020 2020 7c20 e29c 9320 2020 207c 20e2      | ...    | .
-00006050: 9c93 2020 2020 2020 7c20 e29c 9320 2020  ..      | ...   
-00006060: 2020 2020 2020 7c0a 7c20 5b52 616e 646f        |.| [Rando
-00006070: 6d52 6f74 6174 6539 305d 2868 7474 7073  mRotate90](https
-00006080: 3a2f 2f61 6c62 756d 656e 7461 7469 6f6e  ://albumentation
-00006090: 732e 6169 2f64 6f63 732f 6170 695f 7265  s.ai/docs/api_re
-000060a0: 6665 7265 6e63 652f 6175 676d 656e 7461  ference/augmenta
-000060b0: 7469 6f6e 732f 6765 6f6d 6574 7269 632f  tions/geometric/
-000060c0: 726f 7461 7465 2f23 616c 6275 6d65 6e74  rotate/#albument
-000060d0: 6174 696f 6e73 2e61 7567 6d65 6e74 6174  ations.augmentat
-000060e0: 696f 6e73 2e67 656f 6d65 7472 6963 2e72  ions.geometric.r
-000060f0: 6f74 6174 652e 5261 6e64 6f6d 526f 7461  otate.RandomRota
-00006100: 7465 3930 2920 2020 2020 2020 2020 2020  te90)           
-00006110: 2020 2020 2020 2020 2020 7c20 e29c 9320            | ... 
-00006120: 2020 2020 7c20 e29c 9320 2020 207c 20e2      | ...    | .
-00006130: 9c93 2020 2020 2020 7c20 e29c 9320 2020  ..      | ...   
-00006140: 2020 2020 2020 7c0a 7c20 5b52 616e 646f        |.| [Rando
-00006150: 6d53 6361 6c65 5d28 6874 7470 733a 2f2f  mScale](https://
-00006160: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
-00006170: 692f 646f 6373 2f61 7069 5f72 6566 6572  i/docs/api_refer
-00006180: 656e 6365 2f61 7567 6d65 6e74 6174 696f  ence/augmentatio
-00006190: 6e73 2f67 656f 6d65 7472 6963 2f72 6573  ns/geometric/res
-000061a0: 697a 652f 2361 6c62 756d 656e 7461 7469  ize/#albumentati
-000061b0: 6f6e 732e 6175 676d 656e 7461 7469 6f6e  ons.augmentation
-000061c0: 732e 6765 6f6d 6574 7269 632e 7265 7369  s.geometric.resi
-000061d0: 7a65 2e52 616e 646f 6d53 6361 6c65 2920  ze.RandomScale) 
-000061e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061f0: 2020 2020 2020 2020 2020 7c20 e29c 9320            | ... 
-00006200: 2020 2020 7c20 e29c 9320 2020 207c 20e2      | ...    | .
-00006210: 9c93 2020 2020 2020 7c20 e29c 9320 2020  ..      | ...   
-00006220: 2020 2020 2020 7c0a 7c20 5b52 616e 646f        |.| [Rando
-00006230: 6d53 697a 6564 4242 6f78 5361 6665 4372  mSizedBBoxSafeCr
-00006240: 6f70 5d28 6874 7470 733a 2f2f 616c 6275  op](https://albu
-00006250: 6d65 6e74 6174 696f 6e73 2e61 692f 646f  mentations.ai/do
-00006260: 6373 2f61 7069 5f72 6566 6572 656e 6365  cs/api_reference
-00006270: 2f61 7567 6d65 6e74 6174 696f 6e73 2f63  /augmentations/c
-00006280: 726f 7073 2f74 7261 6e73 666f 726d 732f  rops/transforms/
-00006290: 2361 6c62 756d 656e 7461 7469 6f6e 732e  #albumentations.
-000062a0: 6175 676d 656e 7461 7469 6f6e 732e 6372  augmentations.cr
-000062b0: 6f70 732e 7472 616e 7366 6f72 6d73 2e52  ops.transforms.R
-000062c0: 616e 646f 6d53 697a 6564 4242 6f78 5361  andomSizedBBoxSa
-000062d0: 6665 4372 6f70 2920 2020 7c20 e29c 9320  feCrop)   | ... 
-000062e0: 2020 2020 7c20 e29c 9320 2020 207c 20e2      | ...    | .
-000062f0: 9c93 2020 2020 2020 7c20 2020 2020 2020  ..      |       
-00006300: 2020 2020 7c0a 7c20 5b52 616e 646f 6d53      |.| [RandomS
-00006310: 697a 6564 4372 6f70 5d28 6874 7470 733a  izedCrop](https:
-00006320: 2f2f 616c 6275 6d65 6e74 6174 696f 6e73  //albumentations
-00006330: 2e61 692f 646f 6373 2f61 7069 5f72 6566  .ai/docs/api_ref
-00006340: 6572 656e 6365 2f61 7567 6d65 6e74 6174  erence/augmentat
-00006350: 696f 6e73 2f63 726f 7073 2f74 7261 6e73  ions/crops/trans
-00006360: 666f 726d 732f 2361 6c62 756d 656e 7461  forms/#albumenta
-00006370: 7469 6f6e 732e 6175 676d 656e 7461 7469  tions.augmentati
-00006380: 6f6e 732e 6372 6f70 732e 7472 616e 7366  ons.crops.transf
-00006390: 6f72 6d73 2e52 616e 646f 6d53 697a 6564  orms.RandomSized
-000063a0: 4372 6f70 2920 2020 2020 2020 2020 2020  Crop)           
-000063b0: 2020 2020 2020 2020 7c20 e29c 9320 2020          | ...   
-000063c0: 2020 7c20 e29c 9320 2020 207c 20e2 9c93    | ...    | ...
-000063d0: 2020 2020 2020 7c20 e29c 9320 2020 2020        | ...     
-000063e0: 2020 2020 7c0a 7c20 5b52 6573 697a 655d      |.| [Resize]
-000063f0: 2868 7474 7073 3a2f 2f61 6c62 756d 656e  (https://albumen
-00006400: 7461 7469 6f6e 732e 6169 2f64 6f63 732f  tations.ai/docs/
-00006410: 6170 695f 7265 6665 7265 6e63 652f 6175  api_reference/au
-00006420: 676d 656e 7461 7469 6f6e 732f 6765 6f6d  gmentations/geom
-00006430: 6574 7269 632f 7265 7369 7a65 2f23 616c  etric/resize/#al
-00006440: 6275 6d65 6e74 6174 696f 6e73 2e61 7567  bumentations.aug
-00006450: 6d65 6e74 6174 696f 6e73 2e67 656f 6d65  mentations.geome
-00006460: 7472 6963 2e72 6573 697a 652e 5265 7369  tric.resize.Resi
-00006470: 7a65 2920 2020 2020 2020 2020 2020 2020  ze)             
-00006480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006490: 2020 2020 2020 2020 7c20 e29c 9320 2020          | ...   
-000064a0: 2020 7c20 e29c 9320 2020 207c 20e2 9c93    | ...    | ...
-000064b0: 2020 2020 2020 7c20 e29c 9320 2020 2020        | ...     
-000064c0: 2020 2020 7c0a 7c20 5b52 6f74 6174 655d      |.| [Rotate]
-000064d0: 2868 7474 7073 3a2f 2f61 6c62 756d 656e  (https://albumen
-000064e0: 7461 7469 6f6e 732e 6169 2f64 6f63 732f  tations.ai/docs/
-000064f0: 6170 695f 7265 6665 7265 6e63 652f 6175  api_reference/au
-00006500: 676d 656e 7461 7469 6f6e 732f 6765 6f6d  gmentations/geom
-00006510: 6574 7269 632f 726f 7461 7465 2f23 616c  etric/rotate/#al
-00006520: 6275 6d65 6e74 6174 696f 6e73 2e61 7567  bumentations.aug
-00006530: 6d65 6e74 6174 696f 6e73 2e67 656f 6d65  mentations.geome
-00006540: 7472 6963 2e72 6f74 6174 652e 526f 7461  tric.rotate.Rota
-00006550: 7465 2920 2020 2020 2020 2020 2020 2020  te)             
-00006560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006570: 2020 2020 2020 2020 7c20 e29c 9320 2020          | ...   
-00006580: 2020 7c20 e29c 9320 2020 207c 20e2 9c93    | ...    | ...
-00006590: 2020 2020 2020 7c20 e29c 9320 2020 2020        | ...     
-000065a0: 2020 2020 7c0a 7c20 5b53 6166 6552 6f74      |.| [SafeRot
-000065b0: 6174 655d 2868 7474 7073 3a2f 2f61 6c62  ate](https://alb
-000065c0: 756d 656e 7461 7469 6f6e 732e 6169 2f64  umentations.ai/d
-000065d0: 6f63 732f 6170 695f 7265 6665 7265 6e63  ocs/api_referenc
-000065e0: 652f 6175 676d 656e 7461 7469 6f6e 732f  e/augmentations/
-000065f0: 6765 6f6d 6574 7269 632f 726f 7461 7465  geometric/rotate
-00006600: 2f23 616c 6275 6d65 6e74 6174 696f 6e73  /#albumentations
-00006610: 2e61 7567 6d65 6e74 6174 696f 6e73 2e67  .augmentations.g
-00006620: 656f 6d65 7472 6963 2e72 6f74 6174 652e  eometric.rotate.
-00006630: 5361 6665 526f 7461 7465 2920 2020 2020  SafeRotate)     
-00006640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006650: 2020 2020 2020 2020 7c20 e29c 9320 2020          | ...   
-00006660: 2020 7c20 e29c 9320 2020 207c 20e2 9c93    | ...    | ...
-00006670: 2020 2020 2020 7c20 e29c 9320 2020 2020        | ...     
-00006680: 2020 2020 7c0a 7c20 5b53 6869 6674 5363      |.| [ShiftSc
-00006690: 616c 6552 6f74 6174 655d 2868 7474 7073  aleRotate](https
-000066a0: 3a2f 2f61 6c62 756d 656e 7461 7469 6f6e  ://albumentation
-000066b0: 732e 6169 2f64 6f63 732f 6170 695f 7265  s.ai/docs/api_re
-000066c0: 6665 7265 6e63 652f 6175 676d 656e 7461  ference/augmenta
-000066d0: 7469 6f6e 732f 6765 6f6d 6574 7269 632f  tions/geometric/
-000066e0: 7472 616e 7366 6f72 6d73 2f23 616c 6275  transforms/#albu
-000066f0: 6d65 6e74 6174 696f 6e73 2e61 7567 6d65  mentations.augme
-00006700: 6e74 6174 696f 6e73 2e67 656f 6d65 7472  ntations.geometr
-00006710: 6963 2e74 7261 6e73 666f 726d 732e 5368  ic.transforms.Sh
-00006720: 6966 7453 6361 6c65 526f 7461 7465 2920  iftScaleRotate) 
-00006730: 2020 2020 2020 2020 7c20 e29c 9320 2020          | ...   
-00006740: 2020 7c20 e29c 9320 2020 207c 20e2 9c93    | ...    | ...
-00006750: 2020 2020 2020 7c20 e29c 9320 2020 2020        | ...     
-00006760: 2020 2020 7c0a 7c20 5b53 6d61 6c6c 6573      |.| [Smalles
-00006770: 744d 6178 5369 7a65 5d28 6874 7470 733a  tMaxSize](https:
-00006780: 2f2f 616c 6275 6d65 6e74 6174 696f 6e73  //albumentations
-00006790: 2e61 692f 646f 6373 2f61 7069 5f72 6566  .ai/docs/api_ref
-000067a0: 6572 656e 6365 2f61 7567 6d65 6e74 6174  erence/augmentat
-000067b0: 696f 6e73 2f67 656f 6d65 7472 6963 2f72  ions/geometric/r
-000067c0: 6573 697a 652f 2361 6c62 756d 656e 7461  esize/#albumenta
-000067d0: 7469 6f6e 732e 6175 676d 656e 7461 7469  tions.augmentati
-000067e0: 6f6e 732e 6765 6f6d 6574 7269 632e 7265  ons.geometric.re
-000067f0: 7369 7a65 2e53 6d61 6c6c 6573 744d 6178  size.SmallestMax
-00006800: 5369 7a65 2920 2020 2020 2020 2020 2020  Size)           
-00006810: 2020 2020 2020 2020 7c20 e29c 9320 2020          | ...   
-00006820: 2020 7c20 e29c 9320 2020 207c 20e2 9c93    | ...    | ...
-00006830: 2020 2020 2020 7c20 e29c 9320 2020 2020        | ...     
-00006840: 2020 2020 7c0a 7c20 5b54 7261 6e73 706f      |.| [Transpo
-00006850: 7365 5d28 6874 7470 733a 2f2f 616c 6275  se](https://albu
-00006860: 6d65 6e74 6174 696f 6e73 2e61 692f 646f  mentations.ai/do
-00006870: 6373 2f61 7069 5f72 6566 6572 656e 6365  cs/api_reference
-00006880: 2f61 7567 6d65 6e74 6174 696f 6e73 2f67  /augmentations/g
-00006890: 656f 6d65 7472 6963 2f74 7261 6e73 666f  eometric/transfo
-000068a0: 726d 732f 2361 6c62 756d 656e 7461 7469  rms/#albumentati
-000068b0: 6f6e 732e 6175 676d 656e 7461 7469 6f6e  ons.augmentation
-000068c0: 732e 6765 6f6d 6574 7269 632e 7472 616e  s.geometric.tran
-000068d0: 7366 6f72 6d73 2e54 7261 6e73 706f 7365  sforms.Transpose
-000068e0: 2920 2020 2020 2020 2020 2020 2020 2020  )               
-000068f0: 2020 2020 2020 2020 7c20 e29c 9320 2020          | ...   
-00006900: 2020 7c20 e29c 9320 2020 207c 20e2 9c93    | ...    | ...
-00006910: 2020 2020 2020 7c20 e29c 9320 2020 2020        | ...     
-00006920: 2020 2020 7c0a 7c20 5b56 6572 7469 6361      |.| [Vertica
-00006930: 6c46 6c69 705d 2868 7474 7073 3a2f 2f61  lFlip](https://a
-00006940: 6c62 756d 656e 7461 7469 6f6e 732e 6169  lbumentations.ai
-00006950: 2f64 6f63 732f 6170 695f 7265 6665 7265  /docs/api_refere
-00006960: 6e63 652f 6175 676d 656e 7461 7469 6f6e  nce/augmentation
-00006970: 732f 6765 6f6d 6574 7269 632f 7472 616e  s/geometric/tran
-00006980: 7366 6f72 6d73 2f23 616c 6275 6d65 6e74  sforms/#albument
-00006990: 6174 696f 6e73 2e61 7567 6d65 6e74 6174  ations.augmentat
-000069a0: 696f 6e73 2e67 656f 6d65 7472 6963 2e74  ions.geometric.t
-000069b0: 7261 6e73 666f 726d 732e 5665 7274 6963  ransforms.Vertic
-000069c0: 616c 466c 6970 2920 2020 2020 2020 2020  alFlip)         
-000069d0: 2020 2020 2020 2020 7c20 e29c 9320 2020          | ...   
-000069e0: 2020 7c20 e29c 9320 2020 207c 20e2 9c93    | ...    | ...
-000069f0: 2020 2020 2020 7c20 e29c 9320 2020 2020        | ...     
-00006a00: 2020 2020 7c0a 7c20 5b58 594d 6173 6b69      |.| [XYMaski
-00006a10: 6e67 5d28 6874 7470 733a 2f2f 616c 6275  ng](https://albu
-00006a20: 6d65 6e74 6174 696f 6e73 2e61 692f 646f  mentations.ai/do
-00006a30: 6373 2f61 7069 5f72 6566 6572 656e 6365  cs/api_reference
-00006a40: 2f61 7567 6d65 6e74 6174 696f 6e73 2f64  /augmentations/d
-00006a50: 726f 706f 7574 2f78 795f 6d61 736b 696e  ropout/xy_maskin
-00006a60: 672f 2361 6c62 756d 656e 7461 7469 6f6e  g/#albumentation
-00006a70: 732e 6175 676d 656e 7461 7469 6f6e 732e  s.augmentations.
-00006a80: 6472 6f70 6f75 742e 7879 5f6d 6173 6b69  dropout.xy_maski
-00006a90: 6e67 2e58 594d 6173 6b69 6e67 2920 2020  ng.XYMasking)   
-00006aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ab0: 2020 2020 2020 2020 7c20 e29c 9320 2020          | ...   
-00006ac0: 2020 7c20 e29c 9320 2020 207c 2020 2020    | ...    |    
-00006ad0: 2020 2020 7c20 e29c 9320 2020 2020 2020      | ...       
-00006ae0: 2020 7c0a 0a23 2323 204d 6978 696e 672d    |..### Mixing-
-00006af0: 6c65 7665 6c20 7472 616e 7366 6f72 6d73  level transforms
-00006b00: 0a0a 5472 616e 7366 6f72 6d73 2074 6861  ..Transforms tha
-00006b10: 7420 6d69 7820 7365 7665 7261 6c20 696d  t mix several im
-00006b20: 6167 6573 2069 6e74 6f20 6f6e 650a 0a7c  ages into one..|
-00006b30: 2054 7261 6e73 666f 726d 2020 2020 2020   Transform      
-00006b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005bf0: 2020 2020 2020 2020 2020 2020 207c 20e2               | .
+00005c00: 9c93 2020 2020 207c 20e2 9c93 2020 2020  ..     | ...    
+00005c10: 7c20 e29c 9320 2020 2020 207c 20e2 9c93  | ...      | ...
+00005c20: 2020 2020 2020 2020 207c 0a7c 205b 4c6f           |.| [Lo
+00005c30: 6e67 6573 744d 6178 5369 7a65 5d28 6874  ngestMaxSize](ht
+00005c40: 7470 733a 2f2f 616c 6275 6d65 6e74 6174  tps://albumentat
+00005c50: 696f 6e73 2e61 692f 646f 6373 2f61 7069  ions.ai/docs/api
+00005c60: 5f72 6566 6572 656e 6365 2f61 7567 6d65  _reference/augme
+00005c70: 6e74 6174 696f 6e73 2f67 656f 6d65 7472  ntations/geometr
+00005c80: 6963 2f72 6573 697a 652f 2361 6c62 756d  ic/resize/#album
+00005c90: 656e 7461 7469 6f6e 732e 6175 676d 656e  entations.augmen
+00005ca0: 7461 7469 6f6e 732e 6765 6f6d 6574 7269  tations.geometri
+00005cb0: 632e 7265 7369 7a65 2e4c 6f6e 6765 7374  c.resize.Longest
+00005cc0: 4d61 7853 697a 6529 2020 2020 2020 2020  MaxSize)        
+00005cd0: 2020 2020 2020 2020 2020 2020 207c 20e2               | .
+00005ce0: 9c93 2020 2020 207c 20e2 9c93 2020 2020  ..     | ...    
+00005cf0: 7c20 e29c 9320 2020 2020 207c 20e2 9c93  | ...      | ...
+00005d00: 2020 2020 2020 2020 207c 0a7c 205b 4d61           |.| [Ma
+00005d10: 736b 4472 6f70 6f75 745d 2868 7474 7073  skDropout](https
+00005d20: 3a2f 2f61 6c62 756d 656e 7461 7469 6f6e  ://albumentation
+00005d30: 732e 6169 2f64 6f63 732f 6170 695f 7265  s.ai/docs/api_re
+00005d40: 6665 7265 6e63 652f 6175 676d 656e 7461  ference/augmenta
+00005d50: 7469 6f6e 732f 6472 6f70 6f75 742f 6d61  tions/dropout/ma
+00005d60: 736b 5f64 726f 706f 7574 2f23 616c 6275  sk_dropout/#albu
+00005d70: 6d65 6e74 6174 696f 6e73 2e61 7567 6d65  mentations.augme
+00005d80: 6e74 6174 696f 6e73 2e64 726f 706f 7574  ntations.dropout
+00005d90: 2e6d 6173 6b5f 6472 6f70 6f75 742e 4d61  .mask_dropout.Ma
+00005da0: 736b 4472 6f70 6f75 7429 2020 2020 2020  skDropout)      
+00005db0: 2020 2020 2020 2020 2020 2020 207c 20e2               | .
+00005dc0: 9c93 2020 2020 207c 20e2 9c93 2020 2020  ..     | ...    
+00005dd0: 7c20 2020 2020 2020 207c 2020 2020 2020  |        |      
+00005de0: 2020 2020 207c 0a7c 205b 4d6f 7270 686f       |.| [Morpho
+00005df0: 6c6f 6769 6361 6c5d 2868 7474 7073 3a2f  logical](https:/
+00005e00: 2f61 6c62 756d 656e 7461 7469 6f6e 732e  /albumentations.
+00005e10: 6169 2f64 6f63 732f 6170 695f 7265 6665  ai/docs/api_refe
+00005e20: 7265 6e63 652f 6175 676d 656e 7461 7469  rence/augmentati
+00005e30: 6f6e 732f 7472 616e 7366 6f72 6d73 2f23  ons/transforms/#
+00005e40: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
+00005e50: 7567 6d65 6e74 6174 696f 6e73 2e74 7261  ugmentations.tra
+00005e60: 6e73 666f 726d 732e 4d6f 7270 686f 6c6f  nsforms.Morpholo
+00005e70: 6769 6361 6c29 2020 2020 2020 2020 2020  gical)          
+00005e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e90: 2020 2020 2020 2020 207c 20e2 9c93 2020           | ...  
+00005ea0: 2020 207c 20e2 9c93 2020 2020 7c20 2020     | ...    |   
+00005eb0: 2020 2020 207c 2020 2020 2020 2020 2020       |          
+00005ec0: 207c 0a7c 205b 4e6f 4f70 5d28 6874 7470   |.| [NoOp](http
+00005ed0: 733a 2f2f 616c 6275 6d65 6e74 6174 696f  s://albumentatio
+00005ee0: 6e73 2e61 692f 646f 6373 2f61 7069 5f72  ns.ai/docs/api_r
+00005ef0: 6566 6572 656e 6365 2f63 6f72 652f 7472  eference/core/tr
+00005f00: 616e 7366 6f72 6d73 5f69 6e74 6572 6661  ansforms_interfa
+00005f10: 6365 2f23 616c 6275 6d65 6e74 6174 696f  ce/#albumentatio
+00005f20: 6e73 2e63 6f72 652e 7472 616e 7366 6f72  ns.core.transfor
+00005f30: 6d73 5f69 6e74 6572 6661 6365 2e4e 6f4f  ms_interface.NoO
+00005f40: 7029 2020 2020 2020 2020 2020 2020 2020  p)              
+00005f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f70: 2020 2020 207c 20e2 9c93 2020 2020 207c       | ...     |
+00005f80: 20e2 9c93 2020 2020 7c20 e29c 9320 2020   ...    | ...   
+00005f90: 2020 207c 20e2 9c93 2020 2020 2020 2020     | ...        
+00005fa0: 207c 0a7c 205b 4f70 7469 6361 6c44 6973   |.| [OpticalDis
+00005fb0: 746f 7274 696f 6e5d 2868 7474 7073 3a2f  tortion](https:/
+00005fc0: 2f61 6c62 756d 656e 7461 7469 6f6e 732e  /albumentations.
+00005fd0: 6169 2f64 6f63 732f 6170 695f 7265 6665  ai/docs/api_refe
+00005fe0: 7265 6e63 652f 6175 676d 656e 7461 7469  rence/augmentati
+00005ff0: 6f6e 732f 6765 6f6d 6574 7269 632f 7472  ons/geometric/tr
+00006000: 616e 7366 6f72 6d73 2f23 616c 6275 6d65  ansforms/#albume
+00006010: 6e74 6174 696f 6e73 2e61 7567 6d65 6e74  ntations.augment
+00006020: 6174 696f 6e73 2e67 656f 6d65 7472 6963  ations.geometric
+00006030: 2e74 7261 6e73 666f 726d 732e 4f70 7469  .transforms.Opti
+00006040: 6361 6c44 6973 746f 7274 696f 6e29 2020  calDistortion)  
+00006050: 2020 2020 207c 20e2 9c93 2020 2020 207c       | ...     |
+00006060: 20e2 9c93 2020 2020 7c20 e29c 9320 2020   ...    | ...   
+00006070: 2020 207c 2020 2020 2020 2020 2020 207c     |           |
+00006080: 0a7c 205b 5061 6449 664e 6565 6465 645d  .| [PadIfNeeded]
+00006090: 2868 7474 7073 3a2f 2f61 6c62 756d 656e  (https://albumen
+000060a0: 7461 7469 6f6e 732e 6169 2f64 6f63 732f  tations.ai/docs/
+000060b0: 6170 695f 7265 6665 7265 6e63 652f 6175  api_reference/au
+000060c0: 676d 656e 7461 7469 6f6e 732f 6765 6f6d  gmentations/geom
+000060d0: 6574 7269 632f 7472 616e 7366 6f72 6d73  etric/transforms
+000060e0: 2f23 616c 6275 6d65 6e74 6174 696f 6e73  /#albumentations
+000060f0: 2e61 7567 6d65 6e74 6174 696f 6e73 2e67  .augmentations.g
+00006100: 656f 6d65 7472 6963 2e74 7261 6e73 666f  eometric.transfo
+00006110: 726d 732e 5061 6449 664e 6565 6465 6429  rms.PadIfNeeded)
+00006120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006130: 2020 207c 20e2 9c93 2020 2020 207c 20e2     | ...     | .
+00006140: 9c93 2020 2020 7c20 e29c 9320 2020 2020  ..    | ...     
+00006150: 207c 20e2 9c93 2020 2020 2020 2020 207c   | ...         |
+00006160: 0a7c 205b 5065 7273 7065 6374 6976 655d  .| [Perspective]
+00006170: 2868 7474 7073 3a2f 2f61 6c62 756d 656e  (https://albumen
+00006180: 7461 7469 6f6e 732e 6169 2f64 6f63 732f  tations.ai/docs/
+00006190: 6170 695f 7265 6665 7265 6e63 652f 6175  api_reference/au
+000061a0: 676d 656e 7461 7469 6f6e 732f 6765 6f6d  gmentations/geom
+000061b0: 6574 7269 632f 7472 616e 7366 6f72 6d73  etric/transforms
+000061c0: 2f23 616c 6275 6d65 6e74 6174 696f 6e73  /#albumentations
+000061d0: 2e61 7567 6d65 6e74 6174 696f 6e73 2e67  .augmentations.g
+000061e0: 656f 6d65 7472 6963 2e74 7261 6e73 666f  eometric.transfo
+000061f0: 726d 732e 5065 7273 7065 6374 6976 6529  rms.Perspective)
+00006200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006210: 2020 207c 20e2 9c93 2020 2020 207c 20e2     | ...     | .
+00006220: 9c93 2020 2020 7c20 e29c 9320 2020 2020  ..    | ...     
+00006230: 207c 20e2 9c93 2020 2020 2020 2020 207c   | ...         |
+00006240: 0a7c 205b 5069 6563 6577 6973 6541 6666  .| [PiecewiseAff
+00006250: 696e 655d 2868 7474 7073 3a2f 2f61 6c62  ine](https://alb
+00006260: 756d 656e 7461 7469 6f6e 732e 6169 2f64  umentations.ai/d
+00006270: 6f63 732f 6170 695f 7265 6665 7265 6e63  ocs/api_referenc
+00006280: 652f 6175 676d 656e 7461 7469 6f6e 732f  e/augmentations/
+00006290: 6765 6f6d 6574 7269 632f 7472 616e 7366  geometric/transf
+000062a0: 6f72 6d73 2f23 616c 6275 6d65 6e74 6174  orms/#albumentat
+000062b0: 696f 6e73 2e61 7567 6d65 6e74 6174 696f  ions.augmentatio
+000062c0: 6e73 2e67 656f 6d65 7472 6963 2e74 7261  ns.geometric.tra
+000062d0: 6e73 666f 726d 732e 5069 6563 6577 6973  nsforms.Piecewis
+000062e0: 6541 6666 696e 6529 2020 2020 2020 2020  eAffine)        
+000062f0: 2020 207c 20e2 9c93 2020 2020 207c 20e2     | ...     | .
+00006300: 9c93 2020 2020 7c20 e29c 9320 2020 2020  ..    | ...     
+00006310: 207c 20e2 9c93 2020 2020 2020 2020 207c   | ...         |
+00006320: 0a7c 205b 5069 7865 6c44 726f 706f 7574  .| [PixelDropout
+00006330: 5d28 6874 7470 733a 2f2f 616c 6275 6d65  ](https://albume
+00006340: 6e74 6174 696f 6e73 2e61 692f 646f 6373  ntations.ai/docs
+00006350: 2f61 7069 5f72 6566 6572 656e 6365 2f61  /api_reference/a
+00006360: 7567 6d65 6e74 6174 696f 6e73 2f74 7261  ugmentations/tra
+00006370: 6e73 666f 726d 732f 2361 6c62 756d 656e  nsforms/#albumen
+00006380: 7461 7469 6f6e 732e 6175 676d 656e 7461  tations.augmenta
+00006390: 7469 6f6e 732e 7472 616e 7366 6f72 6d73  tions.transforms
+000063a0: 2e50 6978 656c 4472 6f70 6f75 7429 2020  .PixelDropout)  
+000063b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063d0: 2020 207c 20e2 9c93 2020 2020 207c 20e2     | ...     | .
+000063e0: 9c93 2020 2020 7c20 2020 2020 2020 207c  ..    |        |
+000063f0: 2020 2020 2020 2020 2020 207c 0a7c 205b             |.| [
+00006400: 5261 6e64 6f6d 4372 6f70 5d28 6874 7470  RandomCrop](http
+00006410: 733a 2f2f 616c 6275 6d65 6e74 6174 696f  s://albumentatio
+00006420: 6e73 2e61 692f 646f 6373 2f61 7069 5f72  ns.ai/docs/api_r
+00006430: 6566 6572 656e 6365 2f61 7567 6d65 6e74  eference/augment
+00006440: 6174 696f 6e73 2f63 726f 7073 2f74 7261  ations/crops/tra
+00006450: 6e73 666f 726d 732f 2361 6c62 756d 656e  nsforms/#albumen
+00006460: 7461 7469 6f6e 732e 6175 676d 656e 7461  tations.augmenta
+00006470: 7469 6f6e 732e 6372 6f70 732e 7472 616e  tions.crops.tran
+00006480: 7366 6f72 6d73 2e52 616e 646f 6d43 726f  sforms.RandomCro
+00006490: 7029 2020 2020 2020 2020 2020 2020 2020  p)              
+000064a0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+000064b0: 20e2 9c93 2020 2020 207c 20e2 9c93 2020   ...     | ...  
+000064c0: 2020 7c20 e29c 9320 2020 2020 207c 20e2    | ...      | .
+000064d0: 9c93 2020 2020 2020 2020 207c 0a7c 205b  ..         |.| [
+000064e0: 5261 6e64 6f6d 4372 6f70 4672 6f6d 426f  RandomCropFromBo
+000064f0: 7264 6572 735d 2868 7474 7073 3a2f 2f61  rders](https://a
+00006500: 6c62 756d 656e 7461 7469 6f6e 732e 6169  lbumentations.ai
+00006510: 2f64 6f63 732f 6170 695f 7265 6665 7265  /docs/api_refere
+00006520: 6e63 652f 6175 676d 656e 7461 7469 6f6e  nce/augmentation
+00006530: 732f 6372 6f70 732f 7472 616e 7366 6f72  s/crops/transfor
+00006540: 6d73 2f23 616c 6275 6d65 6e74 6174 696f  ms/#albumentatio
+00006550: 6e73 2e61 7567 6d65 6e74 6174 696f 6e73  ns.augmentations
+00006560: 2e63 726f 7073 2e74 7261 6e73 666f 726d  .crops.transform
+00006570: 732e 5261 6e64 6f6d 4372 6f70 4672 6f6d  s.RandomCropFrom
+00006580: 426f 7264 6572 7329 2020 2020 2020 207c  Borders)       |
+00006590: 20e2 9c93 2020 2020 207c 20e2 9c93 2020   ...     | ...  
+000065a0: 2020 7c20 e29c 9320 2020 2020 207c 20e2    | ...      | .
+000065b0: 9c93 2020 2020 2020 2020 207c 0a7c 205b  ..         |.| [
+000065c0: 5261 6e64 6f6d 4772 6964 5368 7566 666c  RandomGridShuffl
+000065d0: 655d 2868 7474 7073 3a2f 2f61 6c62 756d  e](https://album
+000065e0: 656e 7461 7469 6f6e 732e 6169 2f64 6f63  entations.ai/doc
+000065f0: 732f 6170 695f 7265 6665 7265 6e63 652f  s/api_reference/
+00006600: 6175 676d 656e 7461 7469 6f6e 732f 7472  augmentations/tr
+00006610: 616e 7366 6f72 6d73 2f23 616c 6275 6d65  ansforms/#albume
+00006620: 6e74 6174 696f 6e73 2e61 7567 6d65 6e74  ntations.augment
+00006630: 6174 696f 6e73 2e74 7261 6e73 666f 726d  ations.transform
+00006640: 732e 5261 6e64 6f6d 4772 6964 5368 7566  s.RandomGridShuf
+00006650: 666c 6529 2020 2020 2020 2020 2020 2020  fle)            
+00006660: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00006670: 20e2 9c93 2020 2020 207c 20e2 9c93 2020   ...     | ...  
+00006680: 2020 7c20 2020 2020 2020 207c 20e2 9c93    |        | ...
+00006690: 2020 2020 2020 2020 207c 0a7c 205b 5261           |.| [Ra
+000066a0: 6e64 6f6d 5265 7369 7a65 6443 726f 705d  ndomResizedCrop]
+000066b0: 2868 7474 7073 3a2f 2f61 6c62 756d 656e  (https://albumen
+000066c0: 7461 7469 6f6e 732e 6169 2f64 6f63 732f  tations.ai/docs/
+000066d0: 6170 695f 7265 6665 7265 6e63 652f 6175  api_reference/au
+000066e0: 676d 656e 7461 7469 6f6e 732f 6372 6f70  gmentations/crop
+000066f0: 732f 7472 616e 7366 6f72 6d73 2f23 616c  s/transforms/#al
+00006700: 6275 6d65 6e74 6174 696f 6e73 2e61 7567  bumentations.aug
+00006710: 6d65 6e74 6174 696f 6e73 2e63 726f 7073  mentations.crops
+00006720: 2e74 7261 6e73 666f 726d 732e 5261 6e64  .transforms.Rand
+00006730: 6f6d 5265 7369 7a65 6443 726f 7029 2020  omResizedCrop)  
+00006740: 2020 2020 2020 2020 2020 2020 207c 20e2               | .
+00006750: 9c93 2020 2020 207c 20e2 9c93 2020 2020  ..     | ...    
+00006760: 7c20 e29c 9320 2020 2020 207c 20e2 9c93  | ...      | ...
+00006770: 2020 2020 2020 2020 207c 0a7c 205b 5261           |.| [Ra
+00006780: 6e64 6f6d 526f 7461 7465 3930 5d28 6874  ndomRotate90](ht
+00006790: 7470 733a 2f2f 616c 6275 6d65 6e74 6174  tps://albumentat
+000067a0: 696f 6e73 2e61 692f 646f 6373 2f61 7069  ions.ai/docs/api
+000067b0: 5f72 6566 6572 656e 6365 2f61 7567 6d65  _reference/augme
+000067c0: 6e74 6174 696f 6e73 2f67 656f 6d65 7472  ntations/geometr
+000067d0: 6963 2f72 6f74 6174 652f 2361 6c62 756d  ic/rotate/#album
+000067e0: 656e 7461 7469 6f6e 732e 6175 676d 656e  entations.augmen
+000067f0: 7461 7469 6f6e 732e 6765 6f6d 6574 7269  tations.geometri
+00006800: 632e 726f 7461 7465 2e52 616e 646f 6d52  c.rotate.RandomR
+00006810: 6f74 6174 6539 3029 2020 2020 2020 2020  otate90)        
+00006820: 2020 2020 2020 2020 2020 2020 207c 20e2               | .
+00006830: 9c93 2020 2020 207c 20e2 9c93 2020 2020  ..     | ...    
+00006840: 7c20 e29c 9320 2020 2020 207c 20e2 9c93  | ...      | ...
+00006850: 2020 2020 2020 2020 207c 0a7c 205b 5261           |.| [Ra
+00006860: 6e64 6f6d 5363 616c 655d 2868 7474 7073  ndomScale](https
+00006870: 3a2f 2f61 6c62 756d 656e 7461 7469 6f6e  ://albumentation
+00006880: 732e 6169 2f64 6f63 732f 6170 695f 7265  s.ai/docs/api_re
+00006890: 6665 7265 6e63 652f 6175 676d 656e 7461  ference/augmenta
+000068a0: 7469 6f6e 732f 6765 6f6d 6574 7269 632f  tions/geometric/
+000068b0: 7265 7369 7a65 2f23 616c 6275 6d65 6e74  resize/#albument
+000068c0: 6174 696f 6e73 2e61 7567 6d65 6e74 6174  ations.augmentat
+000068d0: 696f 6e73 2e67 656f 6d65 7472 6963 2e72  ions.geometric.r
+000068e0: 6573 697a 652e 5261 6e64 6f6d 5363 616c  esize.RandomScal
+000068f0: 6529 2020 2020 2020 2020 2020 2020 2020  e)              
+00006900: 2020 2020 2020 2020 2020 2020 207c 20e2               | .
+00006910: 9c93 2020 2020 207c 20e2 9c93 2020 2020  ..     | ...    
+00006920: 7c20 e29c 9320 2020 2020 207c 20e2 9c93  | ...      | ...
+00006930: 2020 2020 2020 2020 207c 0a7c 205b 5261           |.| [Ra
+00006940: 6e64 6f6d 5369 7a65 6442 426f 7853 6166  ndomSizedBBoxSaf
+00006950: 6543 726f 705d 2868 7474 7073 3a2f 2f61  eCrop](https://a
+00006960: 6c62 756d 656e 7461 7469 6f6e 732e 6169  lbumentations.ai
+00006970: 2f64 6f63 732f 6170 695f 7265 6665 7265  /docs/api_refere
+00006980: 6e63 652f 6175 676d 656e 7461 7469 6f6e  nce/augmentation
+00006990: 732f 6372 6f70 732f 7472 616e 7366 6f72  s/crops/transfor
+000069a0: 6d73 2f23 616c 6275 6d65 6e74 6174 696f  ms/#albumentatio
+000069b0: 6e73 2e61 7567 6d65 6e74 6174 696f 6e73  ns.augmentations
+000069c0: 2e63 726f 7073 2e74 7261 6e73 666f 726d  .crops.transform
+000069d0: 732e 5261 6e64 6f6d 5369 7a65 6442 426f  s.RandomSizedBBo
+000069e0: 7853 6166 6543 726f 7029 2020 207c 20e2  xSafeCrop)   | .
+000069f0: 9c93 2020 2020 207c 20e2 9c93 2020 2020  ..     | ...    
+00006a00: 7c20 e29c 9320 2020 2020 207c 2020 2020  | ...      |    
+00006a10: 2020 2020 2020 207c 0a7c 205b 5261 6e64         |.| [Rand
+00006a20: 6f6d 5369 7a65 6443 726f 705d 2868 7474  omSizedCrop](htt
+00006a30: 7073 3a2f 2f61 6c62 756d 656e 7461 7469  ps://albumentati
+00006a40: 6f6e 732e 6169 2f64 6f63 732f 6170 695f  ons.ai/docs/api_
+00006a50: 7265 6665 7265 6e63 652f 6175 676d 656e  reference/augmen
+00006a60: 7461 7469 6f6e 732f 6372 6f70 732f 7472  tations/crops/tr
+00006a70: 616e 7366 6f72 6d73 2f23 616c 6275 6d65  ansforms/#albume
+00006a80: 6e74 6174 696f 6e73 2e61 7567 6d65 6e74  ntations.augment
+00006a90: 6174 696f 6e73 2e63 726f 7073 2e74 7261  ations.crops.tra
+00006aa0: 6e73 666f 726d 732e 5261 6e64 6f6d 5369  nsforms.RandomSi
+00006ab0: 7a65 6443 726f 7029 2020 2020 2020 2020  zedCrop)        
+00006ac0: 2020 2020 2020 2020 2020 207c 20e2 9c93             | ...
+00006ad0: 2020 2020 207c 20e2 9c93 2020 2020 7c20       | ...    | 
+00006ae0: e29c 9320 2020 2020 207c 20e2 9c93 2020  ...      | ...  
+00006af0: 2020 2020 2020 207c 0a7c 205b 5265 7369         |.| [Resi
+00006b00: 7a65 5d28 6874 7470 733a 2f2f 616c 6275  ze](https://albu
+00006b10: 6d65 6e74 6174 696f 6e73 2e61 692f 646f  mentations.ai/do
+00006b20: 6373 2f61 7069 5f72 6566 6572 656e 6365  cs/api_reference
+00006b30: 2f61 7567 6d65 6e74 6174 696f 6e73 2f67  /augmentations/g
+00006b40: 656f 6d65 7472 6963 2f72 6573 697a 652f  eometric/resize/
+00006b50: 2361 6c62 756d 656e 7461 7469 6f6e 732e  #albumentations.
+00006b60: 6175 676d 656e 7461 7469 6f6e 732e 6765  augmentations.ge
+00006b70: 6f6d 6574 7269 632e 7265 7369 7a65 2e52  ometric.resize.R
+00006b80: 6573 697a 6529 2020 2020 2020 2020 2020  esize)          
 00006b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006bb0: 2020 2020 2020 2020 2020 2020 207c 2049               | I
-00006bc0: 6d61 6765 207c 204d 6173 6b20 7c20 4242  mage | Mask | BB
-00006bd0: 6f78 6573 207c 204b 6579 706f 696e 7473  oxes | Keypoints
-00006be0: 207c 2047 6c6f 6261 6c20 4c61 6265 6c20   | Global Label 
-00006bf0: 7c0a 7c20 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |.| ------------
-00006c00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006c10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006c20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006c30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006c40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006c50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006c60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006c70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d20  --------------- 
-00006c80: 7c20 3a2d 2d2d 3a20 7c20 3a2d 2d3a 207c  | :---: | :--: |
-00006c90: 203a 2d2d 2d2d 3a20 7c20 3a2d 2d2d 2d2d   :----: | :-----
-00006ca0: 2d2d 3a20 7c20 3a2d 2d2d 2d2d 2d2d 2d2d  --: | :---------
-00006cb0: 2d3a 207c 0a7c 205b 4d69 7855 705d 2868  -: |.| [MixUp](h
-00006cc0: 7474 7073 3a2f 2f61 6c62 756d 656e 7461  ttps://albumenta
-00006cd0: 7469 6f6e 732e 6169 2f64 6f63 732f 6170  tions.ai/docs/ap
-00006ce0: 695f 7265 6665 7265 6e63 652f 6175 676d  i_reference/augm
-00006cf0: 656e 7461 7469 6f6e 732f 6d69 7869 6e67  entations/mixing
-00006d00: 2f74 7261 6e73 666f 726d 732f 2361 6c62  /transforms/#alb
-00006d10: 756d 656e 7461 7469 6f6e 732e 6175 676d  umentations.augm
-00006d20: 656e 7461 7469 6f6e 732e 6d69 7869 6e67  entations.mixing
-00006d30: 2e74 7261 6e73 666f 726d 732e 4d69 7855  .transforms.MixU
-00006d40: 7029 207c 20e2 9c93 2020 2020 207c 20e2  p) | ...     | .
-00006d50: 9c93 2020 2020 7c20 2020 2020 2020 207c  ..    |        |
+00006ba0: 2020 2020 2020 2020 2020 207c 20e2 9c93             | ...
+00006bb0: 2020 2020 207c 20e2 9c93 2020 2020 7c20       | ...    | 
+00006bc0: e29c 9320 2020 2020 207c 20e2 9c93 2020  ...      | ...  
+00006bd0: 2020 2020 2020 207c 0a7c 205b 526f 7461         |.| [Rota
+00006be0: 7465 5d28 6874 7470 733a 2f2f 616c 6275  te](https://albu
+00006bf0: 6d65 6e74 6174 696f 6e73 2e61 692f 646f  mentations.ai/do
+00006c00: 6373 2f61 7069 5f72 6566 6572 656e 6365  cs/api_reference
+00006c10: 2f61 7567 6d65 6e74 6174 696f 6e73 2f67  /augmentations/g
+00006c20: 656f 6d65 7472 6963 2f72 6f74 6174 652f  eometric/rotate/
+00006c30: 2361 6c62 756d 656e 7461 7469 6f6e 732e  #albumentations.
+00006c40: 6175 676d 656e 7461 7469 6f6e 732e 6765  augmentations.ge
+00006c50: 6f6d 6574 7269 632e 726f 7461 7465 2e52  ometric.rotate.R
+00006c60: 6f74 6174 6529 2020 2020 2020 2020 2020  otate)          
+00006c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c80: 2020 2020 2020 2020 2020 207c 20e2 9c93             | ...
+00006c90: 2020 2020 207c 20e2 9c93 2020 2020 7c20       | ...    | 
+00006ca0: e29c 9320 2020 2020 207c 20e2 9c93 2020  ...      | ...  
+00006cb0: 2020 2020 2020 207c 0a7c 205b 5361 6665         |.| [Safe
+00006cc0: 526f 7461 7465 5d28 6874 7470 733a 2f2f  Rotate](https://
+00006cd0: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
+00006ce0: 692f 646f 6373 2f61 7069 5f72 6566 6572  i/docs/api_refer
+00006cf0: 656e 6365 2f61 7567 6d65 6e74 6174 696f  ence/augmentatio
+00006d00: 6e73 2f67 656f 6d65 7472 6963 2f72 6f74  ns/geometric/rot
+00006d10: 6174 652f 2361 6c62 756d 656e 7461 7469  ate/#albumentati
+00006d20: 6f6e 732e 6175 676d 656e 7461 7469 6f6e  ons.augmentation
+00006d30: 732e 6765 6f6d 6574 7269 632e 726f 7461  s.geometric.rota
+00006d40: 7465 2e53 6166 6552 6f74 6174 6529 2020  te.SafeRotate)  
+00006d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006d60: 2020 2020 2020 2020 2020 207c 20e2 9c93             | ...
-00006d70: 2020 2020 2020 2020 2020 2020 7c0a 0a23              |..#
-00006d80: 2320 4120 6665 7720 6d6f 7265 2065 7861  # A few more exa
-00006d90: 6d70 6c65 7320 6f66 202a 2a61 7567 6d65  mples of **augme
-00006da0: 6e74 6174 696f 6e73 2a2a 0a0a 2323 2320  ntations**..### 
-00006db0: 5365 6d61 6e74 6963 2073 6567 6d65 6e74  Semantic segment
-00006dc0: 6174 696f 6e20 6f6e 2074 6865 2049 6e72  ation on the Inr
-00006dd0: 6961 2064 6174 6173 6574 0a0a 215b 696e  ia dataset..![in
-00006de0: 7269 615d 2868 7474 7073 3a2f 2f68 6162  ria](https://hab
-00006df0: 7261 7374 6f72 6167 652e 6f72 672f 7765  rastorage.org/we
-00006e00: 6274 2f73 752f 7761 2f6e 702f 7375 7761  bt/su/wa/np/suwa
-00006e10: 6e70 656f 3677 7737 7770 7774 6f62 7472  npeo6ww7wpwtobtr
-00006e20: 7a64 5f63 6732 302e 6a70 6567 290a 0a23  zd_cg20.jpeg)..#
-00006e30: 2323 204d 6564 6963 616c 2069 6d61 6769  ## Medical imagi
-00006e40: 6e67 0a0a 215b 6d65 6469 6361 6c5d 2868  ng..![medical](h
-00006e50: 7474 7073 3a2f 2f68 6162 7261 7374 6f72  ttps://habrastor
-00006e60: 6167 652e 6f72 672f 7765 6274 2f31 692f  age.org/webt/1i/
-00006e70: 6669 2f77 7a2f 3169 6669 777a 7930 6c78  fi/wz/1ifiwzy0lx
-00006e80: 6574 6334 6e77 6a76 7373 2d37 316e 6b77  etc4nwjvss-71nkw
-00006e90: 302e 6a70 6567 290a 0a23 2323 204f 626a  0.jpeg)..### Obj
-00006ea0: 6563 7420 6465 7465 6374 696f 6e20 616e  ect detection an
-00006eb0: 6420 7365 6d61 6e74 6963 2073 6567 6d65  d semantic segme
-00006ec0: 6e74 6174 696f 6e20 6f6e 2074 6865 204d  ntation on the M
-00006ed0: 6170 696c 6c61 7279 2056 6973 7461 7320  apillary Vistas 
-00006ee0: 6461 7461 7365 740a 0a21 5b76 6973 7461  dataset..![vista
-00006ef0: 735d 2868 7474 7073 3a2f 2f68 6162 7261  s](https://habra
-00006f00: 7374 6f72 6167 652e 6f72 672f 7765 6274  storage.org/webt
-00006f10: 2f72 7a2f 2d68 2f33 6a2f 727a 2d68 336a  /rz/-h/3j/rz-h3j
-00006f20: 616c 6278 6963 386f 5f66 6875 6378 7973  albxic8o_fhucxys
-00006f30: 7473 3474 632e 6a70 6567 290a 0a23 2323  ts4tc.jpeg)..###
-00006f40: 204b 6579 706f 696e 7473 2061 7567 6d65   Keypoints augme
-00006f50: 6e74 6174 696f 6e0a 0a3c 696d 6720 7372  ntation..<img sr
-00006f60: 633d 2268 7474 7073 3a2f 2f68 6162 7261  c="https://habra
-00006f70: 7374 6f72 6167 652e 6f72 672f 7765 6274  storage.org/webt
-00006f80: 2f65 2d2f 366b 2f7a 2d2f 652d 366b 7a2d  /e-/6k/z-/e-6kz-
-00006f90: 6675 6770 3268 6561 6b33 6a7a 6e73 3362  fugp2heak3jzns3b
-00006fa0: 632d 7238 6f2e 6a70 6567 2220 7769 6474  c-r8o.jpeg" widt
-00006fb0: 683d 3130 3025 3e0a 0a0a 2323 2042 656e  h=100%>...## Ben
-00006fc0: 6368 6d61 726b 696e 6720 7265 7375 6c74  chmarking result
-00006fd0: 730a 0a54 6f20 7275 6e20 7468 6520 6265  s..To run the be
-00006fe0: 6e63 686d 6172 6b20 796f 7572 7365 6c66  nchmark yourself
-00006ff0: 2c20 666f 6c6c 6f77 2074 6865 2069 6e73  , follow the ins
-00007000: 7472 7563 7469 6f6e 7320 696e 205b 6265  tructions in [be
-00007010: 6e63 686d 6172 6b2f 5245 4144 4d45 2e6d  nchmark/README.m
-00007020: 645d 2868 7474 7073 3a2f 2f67 6974 6875  d](https://githu
-00007030: 622e 636f 6d2f 616c 6275 6d65 6e74 6174  b.com/albumentat
-00007040: 696f 6e73 2d74 6561 6d2f 616c 6275 6d65  ions-team/albume
-00007050: 6e74 6174 696f 6e73 2f62 6c6f 622f 6d61  ntations/blob/ma
-00007060: 7374 6572 2f62 656e 6368 6d61 726b 2f52  ster/benchmark/R
-00007070: 4541 444d 452e 6d64 290a 0a52 6573 756c  EADME.md)..Resul
-00007080: 7473 2066 6f72 2072 756e 6e69 6e67 2074  ts for running t
-00007090: 6865 2062 656e 6368 6d61 726b 206f 6e20  he benchmark on 
-000070a0: 7468 6520 6669 7273 7420 3230 3030 2069  the first 2000 i
-000070b0: 6d61 6765 7320 6672 6f6d 2074 6865 2049  mages from the I
-000070c0: 6d61 6765 4e65 7420 7661 6c69 6461 7469  mageNet validati
-000070d0: 6f6e 2073 6574 2075 7369 6e67 2061 6e20  on set using an 
-000070e0: 414d 4420 5279 7a65 6e20 5468 7265 6164  AMD Ryzen Thread
-000070f0: 7269 7070 6572 2033 3937 3058 2043 5055  ripper 3970X CPU
-00007100: 2e0a 416c 6c20 6f75 7470 7574 7320 6172  ..All outputs ar
-00007110: 6520 636f 6e76 6572 7465 6420 746f 2061  e converted to a
-00007120: 2063 6f6e 7469 6775 6f75 7320 4e75 6d50   contiguous NumP
-00007130: 7920 6172 7261 7920 7769 7468 2074 6865  y array with the
-00007140: 206e 702e 7569 6e74 3820 6461 7461 2074   np.uint8 data t
-00007150: 7970 652e 0a54 6865 2074 6162 6c65 2073  ype..The table s
-00007160: 686f 7773 2068 6f77 206d 616e 7920 696d  hows how many im
-00007170: 6167 6573 2070 6572 2073 6563 6f6e 6420  ages per second 
-00007180: 6361 6e20 6265 2070 726f 6365 7373 6564  can be processed
-00007190: 206f 6e20 6120 7369 6e67 6c65 2063 6f72   on a single cor
-000071a0: 653b 2068 6967 6865 7220 6973 2062 6574  e; higher is bet
-000071b0: 7465 722e 0a0a 0a7c 2020 2020 2020 2020  ter....|        
-000071c0: 2020 2020 2020 2020 2020 2020 2020 7c61                |a
-000071d0: 6c62 756d 656e 7461 7469 6f6e 733c 6272  lbumentations<br
-000071e0: 3e3c 736d 616c 6c3e 312e 342e 303c 2f73  ><small>1.4.0</s
-000071f0: 6d61 6c6c 3e7c 696d 6761 7567 3c62 723e  mall>|imgaug<br>
-00007200: 3c73 6d61 6c6c 3e30 2e34 2e30 3c2f 736d  <small>0.4.0</sm
-00007210: 616c 6c3e 7c74 6f72 6368 7669 7369 6f6e  all>|torchvision
-00007220: 3c62 723e 3c73 6d61 6c6c 3e30 2e31 372e  <br><small>0.17.
-00007230: 303c 2f73 6d61 6c6c 3e7c 6b65 7261 733c  0</small>|keras<
-00007240: 6272 3e3c 736d 616c 6c3e 322e 3135 2e30  br><small>2.15.0
-00007250: 3c2f 736d 616c 6c3e 7c61 7567 6d65 6e74  </small>|augment
-00007260: 6f72 3c62 723e 3c73 6d61 6c6c 3e30 2e32  or<br><small>0.2
-00007270: 2e31 323c 2f73 6d61 6c6c 3e7c 736f 6c74  .12</small>|solt
-00007280: 3c62 723e 3c73 6d61 6c6c 3e30 2e31 2e39  <br><small>0.1.9
-00007290: 3c2f 736d 616c 6c3e 7c0a 7c2d 2d2d 2d2d  </small>|.|-----
-000072a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000072b0: 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -|--------------
-000072c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000072d0: 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d  --------|-------
-000072e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000072f0: 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d  -------|--------
-00007300: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007310: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d  ------------|---
+00006d70: 2020 2020 207c 20e2 9c93 2020 2020 7c20       | ...    | 
+00006d80: e29c 9320 2020 2020 207c 20e2 9c93 2020  ...      | ...  
+00006d90: 2020 2020 2020 207c 0a7c 205b 5368 6966         |.| [Shif
+00006da0: 7453 6361 6c65 526f 7461 7465 5d28 6874  tScaleRotate](ht
+00006db0: 7470 733a 2f2f 616c 6275 6d65 6e74 6174  tps://albumentat
+00006dc0: 696f 6e73 2e61 692f 646f 6373 2f61 7069  ions.ai/docs/api
+00006dd0: 5f72 6566 6572 656e 6365 2f61 7567 6d65  _reference/augme
+00006de0: 6e74 6174 696f 6e73 2f67 656f 6d65 7472  ntations/geometr
+00006df0: 6963 2f74 7261 6e73 666f 726d 732f 2361  ic/transforms/#a
+00006e00: 6c62 756d 656e 7461 7469 6f6e 732e 6175  lbumentations.au
+00006e10: 676d 656e 7461 7469 6f6e 732e 6765 6f6d  gmentations.geom
+00006e20: 6574 7269 632e 7472 616e 7366 6f72 6d73  etric.transforms
+00006e30: 2e53 6869 6674 5363 616c 6552 6f74 6174  .ShiftScaleRotat
+00006e40: 6529 2020 2020 2020 2020 207c 20e2 9c93  e)         | ...
+00006e50: 2020 2020 207c 20e2 9c93 2020 2020 7c20       | ...    | 
+00006e60: e29c 9320 2020 2020 207c 20e2 9c93 2020  ...      | ...  
+00006e70: 2020 2020 2020 207c 0a7c 205b 536d 616c         |.| [Smal
+00006e80: 6c65 7374 4d61 7853 697a 655d 2868 7474  lestMaxSize](htt
+00006e90: 7073 3a2f 2f61 6c62 756d 656e 7461 7469  ps://albumentati
+00006ea0: 6f6e 732e 6169 2f64 6f63 732f 6170 695f  ons.ai/docs/api_
+00006eb0: 7265 6665 7265 6e63 652f 6175 676d 656e  reference/augmen
+00006ec0: 7461 7469 6f6e 732f 6765 6f6d 6574 7269  tations/geometri
+00006ed0: 632f 7265 7369 7a65 2f23 616c 6275 6d65  c/resize/#albume
+00006ee0: 6e74 6174 696f 6e73 2e61 7567 6d65 6e74  ntations.augment
+00006ef0: 6174 696f 6e73 2e67 656f 6d65 7472 6963  ations.geometric
+00006f00: 2e72 6573 697a 652e 536d 616c 6c65 7374  .resize.Smallest
+00006f10: 4d61 7853 697a 6529 2020 2020 2020 2020  MaxSize)        
+00006f20: 2020 2020 2020 2020 2020 207c 20e2 9c93             | ...
+00006f30: 2020 2020 207c 20e2 9c93 2020 2020 7c20       | ...    | 
+00006f40: e29c 9320 2020 2020 207c 20e2 9c93 2020  ...      | ...  
+00006f50: 2020 2020 2020 207c 0a7c 205b 5472 616e         |.| [Tran
+00006f60: 7370 6f73 655d 2868 7474 7073 3a2f 2f61  spose](https://a
+00006f70: 6c62 756d 656e 7461 7469 6f6e 732e 6169  lbumentations.ai
+00006f80: 2f64 6f63 732f 6170 695f 7265 6665 7265  /docs/api_refere
+00006f90: 6e63 652f 6175 676d 656e 7461 7469 6f6e  nce/augmentation
+00006fa0: 732f 6765 6f6d 6574 7269 632f 7472 616e  s/geometric/tran
+00006fb0: 7366 6f72 6d73 2f23 616c 6275 6d65 6e74  sforms/#albument
+00006fc0: 6174 696f 6e73 2e61 7567 6d65 6e74 6174  ations.augmentat
+00006fd0: 696f 6e73 2e67 656f 6d65 7472 6963 2e74  ions.geometric.t
+00006fe0: 7261 6e73 666f 726d 732e 5472 616e 7370  ransforms.Transp
+00006ff0: 6f73 6529 2020 2020 2020 2020 2020 2020  ose)            
+00007000: 2020 2020 2020 2020 2020 207c 20e2 9c93             | ...
+00007010: 2020 2020 207c 20e2 9c93 2020 2020 7c20       | ...    | 
+00007020: e29c 9320 2020 2020 207c 20e2 9c93 2020  ...      | ...  
+00007030: 2020 2020 2020 207c 0a7c 205b 5665 7274         |.| [Vert
+00007040: 6963 616c 466c 6970 5d28 6874 7470 733a  icalFlip](https:
+00007050: 2f2f 616c 6275 6d65 6e74 6174 696f 6e73  //albumentations
+00007060: 2e61 692f 646f 6373 2f61 7069 5f72 6566  .ai/docs/api_ref
+00007070: 6572 656e 6365 2f61 7567 6d65 6e74 6174  erence/augmentat
+00007080: 696f 6e73 2f67 656f 6d65 7472 6963 2f74  ions/geometric/t
+00007090: 7261 6e73 666f 726d 732f 2361 6c62 756d  ransforms/#album
+000070a0: 656e 7461 7469 6f6e 732e 6175 676d 656e  entations.augmen
+000070b0: 7461 7469 6f6e 732e 6765 6f6d 6574 7269  tations.geometri
+000070c0: 632e 7472 616e 7366 6f72 6d73 2e56 6572  c.transforms.Ver
+000070d0: 7469 6361 6c46 6c69 7029 2020 2020 2020  ticalFlip)      
+000070e0: 2020 2020 2020 2020 2020 207c 20e2 9c93             | ...
+000070f0: 2020 2020 207c 20e2 9c93 2020 2020 7c20       | ...    | 
+00007100: e29c 9320 2020 2020 207c 20e2 9c93 2020  ...      | ...  
+00007110: 2020 2020 2020 207c 0a7c 205b 5859 4d61         |.| [XYMa
+00007120: 736b 696e 675d 2868 7474 7073 3a2f 2f61  sking](https://a
+00007130: 6c62 756d 656e 7461 7469 6f6e 732e 6169  lbumentations.ai
+00007140: 2f64 6f63 732f 6170 695f 7265 6665 7265  /docs/api_refere
+00007150: 6e63 652f 6175 676d 656e 7461 7469 6f6e  nce/augmentation
+00007160: 732f 6472 6f70 6f75 742f 7879 5f6d 6173  s/dropout/xy_mas
+00007170: 6b69 6e67 2f23 616c 6275 6d65 6e74 6174  king/#albumentat
+00007180: 696f 6e73 2e61 7567 6d65 6e74 6174 696f  ions.augmentatio
+00007190: 6e73 2e64 726f 706f 7574 2e78 795f 6d61  ns.dropout.xy_ma
+000071a0: 736b 696e 672e 5859 4d61 736b 696e 6729  sking.XYMasking)
+000071b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000071c0: 2020 2020 2020 2020 2020 207c 20e2 9c93             | ...
+000071d0: 2020 2020 207c 20e2 9c93 2020 2020 7c20       | ...    | 
+000071e0: 2020 2020 2020 207c 20e2 9c93 2020 2020         | ...    
+000071f0: 2020 2020 207c 0a0a 2323 2320 4d69 7869       |..### Mixi
+00007200: 6e67 2d6c 6576 656c 2074 7261 6e73 666f  ng-level transfo
+00007210: 726d 730a 0a54 7261 6e73 666f 726d 7320  rms..Transforms 
+00007220: 7468 6174 206d 6978 2073 6576 6572 616c  that mix several
+00007230: 2069 6d61 6765 7320 696e 746f 206f 6e65   images into one
+00007240: 0a0a 7c20 5472 616e 7366 6f72 6d20 2020  ..| Transform   
+00007250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000072a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000072b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000072c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000072d0: 7c20 496d 6167 6520 7c20 4d61 736b 207c  | Image | Mask |
+000072e0: 2042 426f 7865 7320 7c20 4b65 7970 6f69   BBoxes | Keypoi
+000072f0: 6e74 7320 7c20 476c 6f62 616c 204c 6162  nts | Global Lab
+00007300: 656c 207c 0a7c 202d 2d2d 2d2d 2d2d 2d2d  el |.| ---------
+00007310: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00007320: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007330: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d  -----------|----
+00007330: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00007340: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007350: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d  --------------|-
+00007350: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00007360: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007370: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 0a7c 486f  -----------|.|Ho
-00007380: 7269 7a6f 6e74 616c 466c 6970 2020 2020  rizontalFlip    
-00007390: 2020 2020 7c2a 2a31 3438 3136 2a2a 2020      |**14816**  
-000073a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000073b0: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-000073c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000073d0: 2020 2020 2020 3539 3832 7c20 2020 2020        5982|     
-000073e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000073f0: 2020 2020 2020 2020 2020 2033 3238 387c             3288|
-00007400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007410: 2020 2020 2020 2020 2020 3231 3732 7c20            2172| 
-00007420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007430: 2020 2020 2020 2020 2020 2020 2032 3934               294
-00007440: 327c 2020 2020 2020 2020 2020 2020 2020  2|              
-00007450: 2020 2020 2020 2020 2020 3836 3031 7c0a            8601|.
-00007460: 7c56 6572 7469 6361 6c46 6c69 7020 2020  |VerticalFlip   
-00007470: 2020 2020 2020 207c 2a2a 3132 3033 322a         |**12032*
-00007480: 2a20 2020 2020 2020 2020 2020 2020 2020  *               
-00007490: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-000074a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000074b0: 2020 2020 2020 2020 2036 3538 397c 2020           6589|  
-000074c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000074d0: 2020 2020 2020 2020 2020 2020 2020 3338                38
-000074e0: 3934 7c20 2020 2020 2020 2020 2020 2020  94|             
-000074f0: 2020 2020 2020 2020 2020 2020 2031 3834               184
-00007500: 337c 2020 2020 2020 2020 2020 2020 2020  3|              
-00007510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007520: 3335 3931 7c20 2020 2020 2020 2020 2020  3591|           
-00007530: 2020 2020 2020 2020 2020 2020 2037 3739               779
-00007540: 397c 0a7c 526f 7461 7465 2020 2020 2020  9|.|Rotate      
-00007550: 2020 2020 2020 2020 2020 7c2a 2a36 3030            |**600
-00007560: 2a2a 2020 2020 2020 2020 2020 2020 2020  **              
-00007570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007580: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-00007590: 2020 2020 2020 2020 2020 2020 2035 3035               505
-000075a0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-000075b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000075c0: 2020 3235 357c 2020 2020 2020 2020 2020    255|          
-000075d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000075e0: 2020 3231 7c20 2020 2020 2020 2020 2020    21|           
-000075f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007600: 2020 2020 2039 337c 2020 2020 2020 2020       93|        
-00007610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007620: 2035 3533 7c0a 7c53 6869 6674 5363 616c   553|.|ShiftScal
-00007630: 6552 6f74 6174 6520 2020 2020 207c 2a2a  eRotate      |**
-00007640: 3933 322a 2a20 2020 2020 2020 2020 2020  932**           
-00007650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007660: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
-00007670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007680: 3638 357c 2020 2020 2020 2020 2020 2020  685|            
-00007690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000076a0: 2020 2020 2032 3234 7c2d 2020 2020 2020       224|-      
-000076b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000076c0: 2020 2020 2020 207c 2d20 2020 2020 2020         |-       
-000076d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000076e0: 2020 2020 2020 2020 2020 7c2d 2020 2020            |-    
-000076f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007700: 2020 2020 2020 207c 0a7c 4272 6967 6874         |.|Bright
-00007710: 6e65 7373 436f 6e74 7261 7374 2020 2020  nessContrast    
-00007720: 7c2a 2a34 3733 372a 2a20 2020 2020 2020  |**4737**       
-00007730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007740: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-00007750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007760: 2020 3134 3234 7c20 2020 2020 2020 2020    1424|         
-00007770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007780: 2020 2020 2020 2020 3235 377c 2020 2020          257|    
-00007790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000077a0: 2020 2020 2020 2035 3233 7c20 2020 2020         523|     
-000077b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000077c0: 2020 2020 2020 2020 2020 3235 377c 2020            257|  
-000077d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000077e0: 2020 2020 2020 3230 3634 7c0a 7c53 6869        2064|.|Shi
-000077f0: 6674 5247 4220 2020 2020 2020 2020 2020  ftRGB           
-00007800: 2020 207c 2a2a 3437 3538 2a2a 2020 2020     |**4758**    
-00007810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007820: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-00007830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007840: 2020 2020 2032 3437 397c 2d20 2020 2020       2479|-     
-00007850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007860: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00007870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007880: 2020 2020 2020 2020 2020 3235 317c 2d20            251|- 
-00007890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078b0: 7c2d 2020 2020 2020 2020 2020 2020 2020  |-              
-000078c0: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
-000078d0: 5368 6966 7448 5356 2020 2020 2020 2020  ShiftHSV        
-000078e0: 2020 2020 2020 7c2a 2a38 3738 2a2a 2020        |**878**  
-000078f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007900: 2020 2020 2020 2020 2020 2020 207c 2020               |  
-00007910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007920: 2020 2020 2020 2020 2033 3935 7c20 2020           395|   
-00007930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007940: 2020 2020 2020 2020 2020 2020 2020 2039                 9
-00007950: 357c 2020 2020 2020 2020 2020 2020 2020  5|              
-00007960: 2020 2020 2020 2020 2020 2020 2031 3132               112
-00007970: 7c2d 2020 2020 2020 2020 2020 2020 2020  |-              
-00007980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007990: 2020 207c 2020 2020 2020 2020 2020 2020     |            
-000079a0: 2020 2020 2020 2020 2020 2020 2032 3531               251
-000079b0: 7c0a 7c52 616e 646f 6d47 616d 6d61 2020  |.|RandomGamma  
-000079c0: 2020 2020 2020 2020 207c 2a2a 3438 3731           |**4871
-000079d0: 2a2a 2020 2020 2020 2020 2020 2020 2020  **              
-000079e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000079f0: 7c2d 2020 2020 2020 2020 2020 2020 2020  |-              
-00007a00: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00007a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a30: 3135 3039 7c20 2020 2020 2020 2020 2020  1509|           
-00007a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a50: 3238 367c 2d20 2020 2020 2020 2020 2020  286|-           
-00007a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a70: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-00007a80: 2020 2020 2020 2020 2020 2020 2020 2031                 1
-00007a90: 3534 307c 0a7c 4772 6179 7363 616c 6520  540|.|Grayscale 
-00007aa0: 2020 2020 2020 2020 2020 2020 7c2a 2a37              |**7
-00007ab0: 3739 302a 2a20 2020 2020 2020 2020 2020  790**           
-00007ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ad0: 2020 207c 2020 2020 2020 2020 2020 2020     |            
-00007ae0: 2020 2020 2020 2020 2020 2020 2020 3131                11
-00007af0: 3739 7c20 2020 2020 2020 2020 2020 2020  79|             
-00007b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b10: 2020 2031 3338 387c 2020 2020 2020 2020     1388|        
-00007b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b30: 2020 2036 3938 7c20 2020 2020 2020 2020     698|         
-00007b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b50: 2020 2020 2032 3536 377c 2020 2020 2020       2567|      
-00007b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b70: 2020 3237 3337 7c0a 7c52 616e 646f 6d43    2737|.|RandomC
-00007b80: 726f 7036 3420 2020 2020 2020 2020 207c  rop64          |
-00007b90: 2a2a 3230 3132 3938 2a2a 2020 2020 2020  **201298**      
+00007370: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007380: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007390: 2d2d 207c 203a 2d2d 2d3a 207c 203a 2d2d  -- | :---: | :--
+000073a0: 3a20 7c20 3a2d 2d2d 2d3a 207c 203a 2d2d  : | :----: | :--
+000073b0: 2d2d 2d2d 2d3a 207c 203a 2d2d 2d2d 2d2d  -----: | :------
+000073c0: 2d2d 2d2d 3a20 7c0a 7c20 5b4d 6978 5570  ----: |.| [MixUp
+000073d0: 5d28 6874 7470 733a 2f2f 616c 6275 6d65  ](https://albume
+000073e0: 6e74 6174 696f 6e73 2e61 692f 646f 6373  ntations.ai/docs
+000073f0: 2f61 7069 5f72 6566 6572 656e 6365 2f61  /api_reference/a
+00007400: 7567 6d65 6e74 6174 696f 6e73 2f6d 6978  ugmentations/mix
+00007410: 696e 672f 7472 616e 7366 6f72 6d73 2f23  ing/transforms/#
+00007420: 616c 6275 6d65 6e74 6174 696f 6e73 2e61  albumentations.a
+00007430: 7567 6d65 6e74 6174 696f 6e73 2e6d 6978  ugmentations.mix
+00007440: 696e 672e 7472 616e 7366 6f72 6d73 2e4d  ing.transforms.M
+00007450: 6978 5570 2920 7c20 e29c 9320 2020 2020  ixUp) | ...     
+00007460: 7c20 e29c 9320 2020 207c 2020 2020 2020  | ...    |      
+00007470: 2020 7c20 2020 2020 2020 2020 2020 7c20    |           | 
+00007480: e29c 9320 2020 2020 2020 2020 2020 207c  ...            |
+00007490: 0a0a 2323 2041 2066 6577 206d 6f72 6520  ..## A few more 
+000074a0: 6578 616d 706c 6573 206f 6620 2a2a 6175  examples of **au
+000074b0: 676d 656e 7461 7469 6f6e 732a 2a0a 0a23  gmentations**..#
+000074c0: 2323 2053 656d 616e 7469 6320 7365 676d  ## Semantic segm
+000074d0: 656e 7461 7469 6f6e 206f 6e20 7468 6520  entation on the 
+000074e0: 496e 7269 6120 6461 7461 7365 740a 0a21  Inria dataset..!
+000074f0: 5b69 6e72 6961 5d28 6874 7470 733a 2f2f  [inria](https://
+00007500: 6861 6272 6173 746f 7261 6765 2e6f 7267  habrastorage.org
+00007510: 2f77 6562 742f 7375 2f77 612f 6e70 2f73  /webt/su/wa/np/s
+00007520: 7577 616e 7065 6f36 7777 3777 7077 746f  uwanpeo6ww7wpwto
+00007530: 6274 727a 645f 6367 3230 2e6a 7065 6729  btrzd_cg20.jpeg)
+00007540: 0a0a 2323 2320 4d65 6469 6361 6c20 696d  ..### Medical im
+00007550: 6167 696e 670a 0a21 5b6d 6564 6963 616c  aging..![medical
+00007560: 5d28 6874 7470 733a 2f2f 6861 6272 6173  ](https://habras
+00007570: 746f 7261 6765 2e6f 7267 2f77 6562 742f  torage.org/webt/
+00007580: 3169 2f66 692f 777a 2f31 6966 6977 7a79  1i/fi/wz/1ifiwzy
+00007590: 306c 7865 7463 346e 776a 7673 732d 3731  0lxetc4nwjvss-71
+000075a0: 6e6b 7730 2e6a 7065 6729 0a0a 2323 2320  nkw0.jpeg)..### 
+000075b0: 4f62 6a65 6374 2064 6574 6563 7469 6f6e  Object detection
+000075c0: 2061 6e64 2073 656d 616e 7469 6320 7365   and semantic se
+000075d0: 676d 656e 7461 7469 6f6e 206f 6e20 7468  gmentation on th
+000075e0: 6520 4d61 7069 6c6c 6172 7920 5669 7374  e Mapillary Vist
+000075f0: 6173 2064 6174 6173 6574 0a0a 215b 7669  as dataset..![vi
+00007600: 7374 6173 5d28 6874 7470 733a 2f2f 6861  stas](https://ha
+00007610: 6272 6173 746f 7261 6765 2e6f 7267 2f77  brastorage.org/w
+00007620: 6562 742f 727a 2f2d 682f 336a 2f72 7a2d  ebt/rz/-h/3j/rz-
+00007630: 6833 6a61 6c62 7869 6338 6f5f 6668 7563  h3jalbxic8o_fhuc
+00007640: 7879 7374 7334 7463 2e6a 7065 6729 0a0a  xysts4tc.jpeg)..
+00007650: 2323 2320 4b65 7970 6f69 6e74 7320 6175  ### Keypoints au
+00007660: 676d 656e 7461 7469 6f6e 0a0a 3c69 6d67  gmentation..<img
+00007670: 2073 7263 3d22 6874 7470 733a 2f2f 6861   src="https://ha
+00007680: 6272 6173 746f 7261 6765 2e6f 7267 2f77  brastorage.org/w
+00007690: 6562 742f 652d 2f36 6b2f 7a2d 2f65 2d36  ebt/e-/6k/z-/e-6
+000076a0: 6b7a 2d66 7567 7032 6865 616b 336a 7a6e  kz-fugp2heak3jzn
+000076b0: 7333 6263 2d72 386f 2e6a 7065 6722 2077  s3bc-r8o.jpeg" w
+000076c0: 6964 7468 3d31 3030 253e 0a0a 2323 2042  idth=100%>..## B
+000076d0: 656e 6368 6d61 726b 696e 6720 7265 7375  enchmarking resu
+000076e0: 6c74 730a 0a54 6f20 7275 6e20 7468 6520  lts..To run the 
+000076f0: 6265 6e63 686d 6172 6b20 796f 7572 7365  benchmark yourse
+00007700: 6c66 2c20 666f 6c6c 6f77 2074 6865 2069  lf, follow the i
+00007710: 6e73 7472 7563 7469 6f6e 7320 696e 205b  nstructions in [
+00007720: 6265 6e63 686d 6172 6b2f 5245 4144 4d45  benchmark/README
+00007730: 2e6d 645d 2868 7474 7073 3a2f 2f67 6974  .md](https://git
+00007740: 6875 622e 636f 6d2f 616c 6275 6d65 6e74  hub.com/albument
+00007750: 6174 696f 6e73 2d74 6561 6d2f 616c 6275  ations-team/albu
+00007760: 6d65 6e74 6174 696f 6e73 2f62 6c6f 622f  mentations/blob/
+00007770: 6d61 7374 6572 2f62 656e 6368 6d61 726b  master/benchmark
+00007780: 2f52 4541 444d 452e 6d64 290a 0a52 6573  /README.md)..Res
+00007790: 756c 7473 2066 6f72 2072 756e 6e69 6e67  ults for running
+000077a0: 2074 6865 2062 656e 6368 6d61 726b 206f   the benchmark o
+000077b0: 6e20 7468 6520 6669 7273 7420 3230 3030  n the first 2000
+000077c0: 2069 6d61 6765 7320 6672 6f6d 2074 6865   images from the
+000077d0: 2049 6d61 6765 4e65 7420 7661 6c69 6461   ImageNet valida
+000077e0: 7469 6f6e 2073 6574 2075 7369 6e67 2061  tion set using a
+000077f0: 6e20 414d 4420 5279 7a65 6e20 5468 7265  n AMD Ryzen Thre
+00007800: 6164 7269 7070 6572 2033 3937 3058 2043  adripper 3970X C
+00007810: 5055 2e0a 5468 6520 7461 626c 6520 7368  PU..The table sh
+00007820: 6f77 7320 686f 7720 6d61 6e79 2069 6d61  ows how many ima
+00007830: 6765 7320 7065 7220 7365 636f 6e64 2063  ges per second c
+00007840: 616e 2062 6520 7072 6f63 6573 7365 6420  an be processed 
+00007850: 6f6e 2061 2073 696e 676c 6520 636f 7265  on a single core
+00007860: 3b20 6869 6768 6572 2069 7320 6265 7474  ; higher is bett
+00007870: 6572 2e0a 0a7c 204c 6962 7261 7279 207c  er...| Library |
+00007880: 2056 6572 7369 6f6e 207c 0a7c 2d2d 2d2d   Version |.|----
+00007890: 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d 2d7c  -----|---------|
+000078a0: 0a7c 2050 7974 686f 6e20 7c20 332e 3130  .| Python | 3.10
+000078b0: 2e31 3320 286d 6169 6e2c 2053 6570 2031  .13 (main, Sep 1
+000078c0: 3120 3230 3233 2c20 3133 3a34 343a 3335  1 2023, 13:44:35
+000078d0: 2920 5b47 4343 2031 312e 322e 305d 207c  ) [GCC 11.2.0] |
+000078e0: 0a7c 2061 6c62 756d 656e 7461 7469 6f6e  .| albumentation
+000078f0: 7320 7c20 312e 342e 3120 7c0a 7c20 696d  s | 1.4.1 |.| im
+00007900: 6761 7567 207c 2030 2e34 2e30 207c 0a7c  gaug | 0.4.0 |.|
+00007910: 2074 6f72 6368 7669 7369 6f6e 207c 2030   torchvision | 0
+00007920: 2e31 372e 312b 726f 636d 352e 3720 7c0a  .17.1+rocm5.7 |.
+00007930: 7c20 6e75 6d70 7920 7c20 312e 3236 2e34  | numpy | 1.26.4
+00007940: 207c 0a7c 206f 7065 6e63 762d 7079 7468   |.| opencv-pyth
+00007950: 6f6e 2d68 6561 646c 6573 7320 7c20 342e  on-headless | 4.
+00007960: 392e 302e 3830 207c 0a7c 2073 6369 6b69  9.0.80 |.| sciki
+00007970: 742d 696d 6167 6520 7c20 302e 3232 2e30  t-image | 0.22.0
+00007980: 207c 0a7c 2073 6369 7079 207c 2031 2e31   |.| scipy | 1.1
+00007990: 322e 3020 7c0a 7c20 7069 6c6c 6f77 207c  2.0 |.| pillow |
+000079a0: 2031 302e 322e 3020 7c0a 7c20 6b6f 726e   10.2.0 |.| korn
+000079b0: 6961 207c 2030 2e37 2e32 207c 0a7c 2061  ia | 0.7.2 |.| a
+000079c0: 7567 6c79 207c 2031 2e30 2e30 207c 0a0a  ugly | 1.0.0 |..
+000079d0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+000079e0: 2020 7c61 6c62 756d 656e 7461 7469 6f6e    |albumentation
+000079f0: 733c 6272 3e3c 736d 616c 6c3e 312e 342e  s<br><small>1.4.
+00007a00: 303c 2f73 6d61 6c6c 3e7c 746f 7263 6876  0</small>|torchv
+00007a10: 6973 696f 6e3c 6272 3e3c 736d 616c 6c3e  ision<br><small>
+00007a20: 302e 3137 2e31 2b72 6f63 6d35 2e37 3c2f  0.17.1+rocm5.7</
+00007a30: 736d 616c 6c3e 7c6b 6f72 6e69 613c 6272  small>|kornia<br
+00007a40: 3e3c 736d 616c 6c3e 302e 372e 323c 2f73  ><small>0.7.2</s
+00007a50: 6d61 6c6c 3e7c 6175 676c 793c 6272 3e3c  mall>|augly<br><
+00007a60: 736d 616c 6c3e 312e 302e 303c 2f73 6d61  small>1.0.0</sma
+00007a70: 6c6c 3e7c 696d 6761 7567 3c62 723e 3c73  ll>|imgaug<br><s
+00007a80: 6d61 6c6c 3e30 2e34 2e30 3c2f 736d 616c  mall>0.4.0</smal
+00007a90: 6c3e 7c0a 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d  l>|.|-----------
+00007aa0: 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d  ------|---------
+00007ab0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007ac0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d  -------------|--
+00007ad0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007ae0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007af0: 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d  ----------|-----
+00007b00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007b10: 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d  ---------|------
+00007b20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007b30: 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d  -------|--------
+00007b40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007b50: 2d2d 2d2d 2d2d 7c0a 7c48 6f72 697a 6f6e  ------|.|Horizon
+00007b60: 7461 6c46 6c69 7020 2020 7c2a 2a39 3834  talFlip   |**984
+00007b70: 3320 c2b1 2032 3133 352a 2a20 2020 2020  3 .. 2135**     
+00007b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b90: 2020 7c32 3433 3620 c2b1 2032 3920 2020    |2436 .. 29   
 00007ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007bb0: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-00007bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007bd0: 2036 3031 337c 2020 2020 2020 2020 2020   6013|          
-00007be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007bf0: 2020 2020 2036 3433 3230 7c20 2020 2020       64320|     
-00007c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c10: 2020 2020 2031 3031 317c 2020 2020 2020       1011|      
-00007c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c30: 2020 2020 2020 2036 3138 3730 7c20 2020         61870|   
-00007c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c50: 2020 2020 3236 3236 307c 0a7c 5061 6454      26260|.|PadT
-00007c60: 6f53 697a 6535 3132 2020 2020 2020 2020  oSize512        
-00007c70: 2020 7c2a 2a38 3135 362a 2a20 2020 2020    |**8156**     
-00007c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c90: 2020 2020 2020 2020 207c 2d20 2020 2020           |-     
-00007ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007cb0: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-00007cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007cd0: 2020 2020 2020 2020 2031 3035 317c 2d20           1051|- 
-00007ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007cf0: 2020 2020 2020 2020 2020 2020 7c2d 2020              |-  
-00007d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d10: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00007d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d30: 2020 2020 2020 2020 3538 3531 7c0a 7c52          5851|.|R
-00007d40: 6573 697a 6535 3132 2020 2020 2020 2020  esize512        
-00007d50: 2020 2020 207c 2a2a 3236 3637 2a2a 2020       |**2667**  
+00007bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007bc0: 7c31 3031 3420 c2b1 2033 2020 2020 2020  |1014 .. 3      
+00007bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007be0: 7c33 3636 3320 c2b1 2031 3820 2020 2020  |3663 .. 18     
+00007bf0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00007c00: 3438 3834 20c2 b120 3531 2020 2020 2020  4884 .. 51      
+00007c10: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00007c20: 0a7c 5665 7274 6963 616c 466c 6970 2020  .|VerticalFlip  
+00007c30: 2020 207c 2a2a 3938 3938 20c2 b120 3138     |**9898 .. 18
+00007c40: 2a2a 2020 2020 2020 2020 2020 2020 2020  **              
+00007c50: 2020 2020 2020 2020 2020 207c 3235 3730             |2570
+00007c60: 20c2 b120 3337 2020 2020 2020 2020 2020   .. 37          
+00007c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c80: 2020 2020 2020 2020 207c 3130 3234 20c2           |1024 .
+00007c90: b120 3420 2020 2020 2020 2020 2020 2020  . 4             
+00007ca0: 2020 2020 2020 2020 207c 3533 3235 20c2           |5325 .
+00007cb0: b120 3133 2020 2020 2020 2020 2020 2020  . 13            
+00007cc0: 2020 2020 2020 2020 7c38 3638 3320 c2b1          |8683 ..
+00007cd0: 2035 2020 2020 2020 2020 2020 2020 2020   5              
+00007ce0: 2020 2020 2020 2020 7c0a 7c52 6f74 6174          |.|Rotat
+00007cf0: 6520 2020 2020 2020 2020 2020 7c36 3130  e           |610
+00007d00: 20c2 b120 3420 2020 2020 2020 2020 2020   .. 4           
+00007d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d20: 2020 2020 7c31 3533 20c2 b120 3220 2020      |153 .. 2   
+00007d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d50: 2020 7c32 3034 20c2 b120 3120 2020 2020    |204 .. 1     
 00007d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d70: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
+00007d70: 2020 7c2a 2a36 3236 20c2 b120 332a 2a20    |**626 .. 3** 
 00007d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d90: 2020 2020 2020 2031 3737 377c 2020 2020         1777|    
+00007d90: 207c 3439 3920 c2b1 2035 2020 2020 2020   |499 .. 5      
 00007da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007db0: 2020 2020 2020 2020 2020 2020 2034 3037               407
-00007dc0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-00007dd0: 2020 2020 2020 2020 2020 2020 3531 377c              517|
-00007de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007df0: 2020 2020 2020 2020 2020 2020 2020 2034                 4
-00007e00: 3039 7c20 2020 2020 2020 2020 2020 2020  09|             
-00007e10: 2020 2020 2020 2020 2020 2032 3435 307c             2450|
-00007e20: 0a7c 5261 6e64 6f6d 5369 7a65 6443 726f  .|RandomSizedCro
-00007e30: 705f 3634 5f35 3132 7c2a 2a35 3232 342a  p_64_512|**5224*
-00007e40: 2a20 2020 2020 2020 2020 2020 2020 2020  *               
-00007e50: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00007e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e70: 2020 2020 2020 2020 2020 3231 3730 7c20            2170| 
-00007e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ea0: 3636 387c 2020 2020 2020 2020 2020 2020  668|            
-00007eb0: 2020 2020 2020 2020 2020 2020 2020 2033                 3
-00007ec0: 3738 7c20 2020 2020 2020 2020 2020 2020  78|             
+00007db0: 207c 0a7c 4166 6669 6e65 2020 2020 2020   |.|Affine      
+00007dc0: 2020 2020 207c 2a2a 3137 3035 20c2 b120       |**1705 .. 
+00007dd0: 3637 2a2a 2020 2020 2020 2020 2020 2020  67**            
+00007de0: 2020 2020 2020 2020 2020 2020 207c 3135               |15
+00007df0: 3920 c2b1 2031 2020 2020 2020 2020 2020  9 .. 1          
+00007e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007e10: 2020 2020 2020 2020 2020 207c 3230 3020             |200 
+00007e20: c2b1 2031 2020 2020 2020 2020 2020 2020  .. 1            
+00007e30: 2020 2020 2020 2020 2020 207c 2d20 2020             |-   
+00007e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007e50: 2020 2020 2020 2020 207c 3636 3320 c2b1           |663 ..
+00007e60: 2032 3420 2020 2020 2020 2020 2020 2020   24             
+00007e70: 2020 2020 2020 2020 207c 0a7c 4571 7561           |.|Equa
+00007e80: 6c69 7a65 2020 2020 2020 2020 207c 2a2a  lize         |**
+00007e90: 3130 3631 20c2 b120 3134 2a2a 2020 2020  1061 .. 14**    
+00007ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007eb0: 2020 2020 207c 3333 3720 c2b1 2031 2020       |337 .. 1  
+00007ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ee0: 2020 3637 307c 2020 2020 2020 2020 2020    670|          
-00007ef0: 2020 2020 2020 2020 2020 2020 2020 3431                41
-00007f00: 3230 7c0a 7c45 7175 616c 697a 6520 2020  20|.|Equalize   
-00007f10: 2020 2020 2020 2020 2020 207c 2a2a 3130             |**10
-00007f20: 3934 2a2a 2020 2020 2020 2020 2020 2020  94**            
+00007ee0: 2020 207c 3737 20c2 b120 3120 2020 2020     |77 .. 1     
+00007ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f00: 2020 207c 2d20 2020 2020 2020 2020 2020     |-           
+00007f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f20: 207c 3834 3520 c2b1 2033 3320 2020 2020   |845 .. 33     
 00007f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f40: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-00007f50: 2020 2020 2020 2020 2020 2020 2020 3536                56
-00007f60: 317c 2d20 2020 2020 2020 2020 2020 2020  1|-             
-00007f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f80: 2020 2020 2020 7c2d 2020 2020 2020 2020        |-        
+00007f40: 207c 0a7c 5261 6e64 6f6d 4372 6f70 3634   |.|RandomCrop64
+00007f50: 2020 2020 207c 2a2a 3230 3331 3937 20c2       |**203197 .
+00007f60: b120 3231 3035 2a2a 2020 2020 2020 2020  . 2105**        
+00007f70: 2020 2020 2020 2020 2020 2020 207c 3135               |15
+00007f80: 3933 3120 c2b1 2032 3720 2020 2020 2020  931 .. 27       
 00007f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007fa0: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-00007fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007fc0: 2020 2020 2039 3834 7c2d 2020 2020 2020       984|-      
-00007fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007fe0: 2020 2020 207c 0a7c 4d75 6c74 6970 6c79       |.|Multiply
-00007ff0: 2020 2020 2020 2020 2020 2020 2020 7c2a                |*
-00008000: 2a34 3638 302a 2a20 2020 2020 2020 2020  *4680**         
-00008010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008020: 2020 2020 207c 2020 2020 2020 2020 2020       |          
+00007fa0: 2020 2020 2020 2020 2020 207c 3833 3720             |837 
+00007fb0: c2b1 2032 2020 2020 2020 2020 2020 2020  .. 2            
+00007fc0: 2020 2020 2020 2020 2020 207c 3231 3835             |2185
+00007fd0: 3820 c2b1 2033 3632 2020 2020 2020 2020  8 .. 362        
+00007fe0: 2020 2020 2020 2020 2020 7c35 3638 3120            |5681 
+00007ff0: c2b1 2039 3620 2020 2020 2020 2020 2020  .. 96           
+00008000: 2020 2020 2020 2020 2020 7c0a 7c52 616e            |.|Ran
+00008010: 646f 6d52 6573 697a 6564 4372 6f70 7c2a  domResizedCrop|*
+00008020: 2a32 3939 3820 c2b1 2033 302a 2a20 2020  *2998 .. 30**   
 00008030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008040: 3236 3233 7c2d 2020 2020 2020 2020 2020  2623|-          
+00008040: 2020 2020 2020 7c31 3136 3020 c2b1 2034        |1160 .. 4
 00008050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008060: 2020 2020 2020 2020 207c 2d20 2020 2020           |-     
-00008070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008080: 2020 2020 2020 2020 7c2d 2020 2020 2020          |-      
-00008090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000080a0: 2020 2020 2020 2020 2020 207c 2d20 2020             |-   
-000080b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000080c0: 2020 2020 2020 2020 7c0a 7c4d 756c 7469          |.|Multi
-000080d0: 706c 7945 6c65 6d65 6e74 7769 7365 2020  plyElementwise  
-000080e0: 207c 2a2a 3435 3332 2a2a 2020 2020 2020   |**4532**      
+00008060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008070: 2020 2020 7c31 3930 20c2 b120 3120 2020      |190 .. 1   
+00008080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008090: 2020 2020 7c2d 2020 2020 2020 2020 2020      |-          
+000080a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000080b0: 2020 7c2d 2020 2020 2020 2020 2020 2020    |-            
+000080c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000080d0: 207c 0a7c 5368 6966 7452 4742 2020 2020   |.|ShiftRGB    
+000080e0: 2020 2020 207c 3134 3030 20c2 b120 3320       |1400 .. 3 
 000080f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008100: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
+00008100: 2020 2020 2020 2020 2020 2020 207c 2d20               |- 
 00008110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008120: 2020 2031 3030 377c 2d20 2020 2020 2020     1007|-       
-00008130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008140: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-00008150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008160: 2020 2020 2020 2020 3435 337c 2d20 2020          453|-   
-00008170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008180: 2020 2020 2020 2020 2020 2020 2020 7c2d                |-
-00008190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000081a0: 2020 2020 2020 2020 2020 207c 0a7c 436f             |.|Co
-000081b0: 6c6f 724a 6974 7465 7220 2020 2020 2020  lorJitter       
-000081c0: 2020 2020 7c2a 2a35 3434 2a2a 2020 2020      |**544**    
-000081d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000081e0: 2020 2020 2020 2020 2020 207c 2020 2020             |    
+00008120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008130: 2020 2020 2020 2020 2020 7c34 3335 20c2            |435 .
+00008140: b120 3120 2020 2020 2020 2020 2020 2020  . 1             
+00008150: 2020 2020 2020 2020 2020 7c2d 2020 2020            |-    
+00008160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008170: 2020 2020 2020 2020 7c2a 2a31 3532 3820          |**1528 
+00008180: c2b1 2036 2a2a 2020 2020 2020 2020 2020  .. 6**          
+00008190: 2020 2020 2020 2020 7c0a 7c52 6573 697a          |.|Resiz
+000081a0: 6520 2020 2020 2020 2020 2020 7c2a 2a32  e           |**2
+000081b0: 3538 3120 c2b1 2033 2a2a 2020 2020 2020  581 .. 3**      
+000081c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000081d0: 2020 2020 7c31 3233 3920 c2b1 2031 2020      |1239 .. 1  
+000081e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000081f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008200: 2020 2020 2020 2031 3038 7c20 2020 2020         108|     
+00008200: 2020 7c31 3937 20c2 b120 3120 2020 2020    |197 .. 1     
 00008210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008220: 2020 2020 2020 2020 2020 2020 2038 347c               84|
+00008220: 2020 7c34 3331 20c2 b120 3120 2020 2020    |431 .. 1     
 00008230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008240: 2020 2020 2020 2020 2020 2031 3136 7c2d             116|-
+00008240: 207c 3137 3238 20c2 b120 3120 2020 2020   |1728 .. 1     
 00008250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008270: 207c 2d20 2020 2020 2020 2020 2020 2020   |-             
-00008280: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-00008290: 0a50 7974 686f 6e20 616e 6420 6c69 6272  .Python and libr
-000082a0: 6172 7920 7665 7273 696f 6e73 3a20 5079  ary versions: Py
-000082b0: 7468 6f6e 2033 2e31 302e 3133 2c20 6e75  thon 3.10.13, nu
-000082c0: 6d70 7920 312e 3236 2e34 2c20 7069 6c6c  mpy 1.26.4, pill
-000082d0: 6f77 2d73 696d 6420 3130 2e32 2e30 2c20  ow-simd 10.2.0, 
-000082e0: 6f70 656e 6376 2d70 7974 686f 6e20 342e  opencv-python 4.
-000082f0: 392e 302e 3830 2c20 7363 696b 6974 2d69  9.0.80, scikit-i
-00008300: 6d61 6765 2030 2e32 322e 302c 2073 6369  mage 0.22.0, sci
-00008310: 7079 2031 2e31 322e 302e 0a0a 2323 2043  py 1.12.0...## C
-00008320: 6f6e 7472 6962 7574 696e 670a 0a54 6f20  ontributing..To 
-00008330: 6372 6561 7465 2061 2070 756c 6c20 7265  create a pull re
-00008340: 7175 6573 7420 746f 2074 6865 2072 6570  quest to the rep
-00008350: 6f73 6974 6f72 792c 2066 6f6c 6c6f 7720  ository, follow 
-00008360: 7468 6520 646f 6375 6d65 6e74 6174 696f  the documentatio
-00008370: 6e20 6174 205b 434f 4e54 5249 4255 5449  n at [CONTRIBUTI
-00008380: 4e47 2e6d 645d 2843 4f4e 5452 4942 5554  NG.md](CONTRIBUT
-00008390: 494e 472e 6d64 290a 0a21 5b68 7474 7073  ING.md)..![https
-000083a0: 3a2f 2f67 6974 6875 622e 636f 6d2f 616c  ://github.com/al
-000083b0: 6275 656d 6e74 6174 696f 6e73 2d74 6561  buemntations-tea
-000083c0: 6d2f 616c 6275 6d65 6e74 6174 696f 6e2f  m/albumentation/
-000083d0: 6772 6170 6873 2f63 6f6e 7472 6962 7574  graphs/contribut
-000083e0: 6f72 735d 2868 7474 7073 3a2f 2f63 6f6e  ors](https://con
-000083f0: 7472 6962 2e72 6f63 6b73 2f69 6d61 6765  trib.rocks/image
-00008400: 3f72 6570 6f3d 616c 6275 6d65 6e74 6174  ?repo=albumentat
-00008410: 696f 6e73 2d74 6561 6d2f 616c 6275 6d65  ions-team/albume
-00008420: 6e74 6174 696f 6e73 290a 0a23 2320 436f  ntations)..## Co
-00008430: 6d6d 756e 6974 7920 616e 6420 5375 7070  mmunity and Supp
-00008440: 6f72 740a 0a2d 205b 5477 6974 7465 725d  ort..- [Twitter]
-00008450: 2868 7474 7073 3a2f 2f74 7769 7474 6572  (https://twitter
-00008460: 2e63 6f6d 2f61 6c62 756d 656e 7461 7469  .com/albumentati
-00008470: 6f6e 7329 0a2d 205b 4469 7363 6f72 645d  ons).- [Discord]
-00008480: 2868 7474 7073 3a2f 2f64 6973 636f 7264  (https://discord
-00008490: 2e67 672f 414b 5072 7244 594e 4174 290a  .gg/AKPrrDYNAt).
-000084a0: 0a23 2320 436f 6d6d 656e 7473 0a0a 496e  .## Comments..In
-000084b0: 2073 6f6d 6520 7379 7374 656d 732c 2069   some systems, i
-000084c0: 6e20 7468 6520 6d75 6c74 6970 6c65 2047  n the multiple G
-000084d0: 5055 2072 6567 696d 652c 2050 7954 6f72  PU regime, PyTor
-000084e0: 6368 206d 6179 2064 6561 646c 6f63 6b20  ch may deadlock 
-000084f0: 7468 6520 4461 7461 4c6f 6164 6572 2069  the DataLoader i
-00008500: 6620 4f70 656e 4356 2077 6173 2063 6f6d  f OpenCV was com
-00008510: 7069 6c65 6420 7769 7468 204f 7065 6e43  piled with OpenC
-00008520: 4c20 6f70 7469 6d69 7a61 7469 6f6e 732e  L optimizations.
-00008530: 2041 6464 696e 6720 7468 6520 666f 6c6c   Adding the foll
-00008540: 6f77 696e 6720 7477 6f20 6c69 6e65 7320  owing two lines 
-00008550: 6265 666f 7265 2074 6865 206c 6962 7261  before the libra
-00008560: 7279 2069 6d70 6f72 7420 6d61 7920 6865  ry import may he
-00008570: 6c70 2e20 466f 7220 6d6f 7265 2064 6574  lp. For more det
-00008580: 6169 6c73 205b 6874 7470 733a 2f2f 6769  ails [https://gi
-00008590: 7468 7562 2e63 6f6d 2f70 7974 6f72 6368  thub.com/pytorch
-000085a0: 2f70 7974 6f72 6368 2f69 7373 7565 732f  /pytorch/issues/
-000085b0: 3133 3535 5d28 6874 7470 733a 2f2f 6769  1355](https://gi
-000085c0: 7468 7562 2e63 6f6d 2f70 7974 6f72 6368  thub.com/pytorch
-000085d0: 2f70 7974 6f72 6368 2f69 7373 7565 732f  /pytorch/issues/
-000085e0: 3133 3535 290a 0a60 6060 7079 7468 6f6e  1355)..```python
-000085f0: 0a63 7632 2e73 6574 4e75 6d54 6872 6561  .cv2.setNumThrea
-00008600: 6473 2830 290a 6376 322e 6f63 6c2e 7365  ds(0).cv2.ocl.se
-00008610: 7455 7365 4f70 656e 434c 2846 616c 7365  tUseOpenCL(False
-00008620: 290a 6060 600a 0a23 2320 4369 7469 6e67  ).```..## Citing
-00008630: 0a0a 4966 2079 6f75 2066 696e 6420 7468  ..If you find th
-00008640: 6973 206c 6962 7261 7279 2075 7365 6675  is library usefu
-00008650: 6c20 666f 7220 796f 7572 2072 6573 6561  l for your resea
-00008660: 7263 682c 2070 6c65 6173 6520 636f 6e73  rch, please cons
-00008670: 6964 6572 2063 6974 696e 6720 5b41 6c62  ider citing [Alb
-00008680: 756d 656e 7461 7469 6f6e 733a 2046 6173  umentations: Fas
-00008690: 7420 616e 6420 466c 6578 6962 6c65 2049  t and Flexible I
-000086a0: 6d61 6765 2041 7567 6d65 6e74 6174 696f  mage Augmentatio
-000086b0: 6e73 5d28 6874 7470 733a 2f2f 7777 772e  ns](https://www.
-000086c0: 6d64 7069 2e63 6f6d 2f32 3037 382d 3234  mdpi.com/2078-24
-000086d0: 3839 2f31 312f 322f 3132 3529 3a0a 0a60  89/11/2/125):..`
-000086e0: 6060 6269 6274 6578 0a40 4172 7469 636c  ``bibtex.@Articl
-000086f0: 657b 696e 666f 3131 3032 3031 3235 2c0a  e{info11020125,.
-00008700: 2020 2020 4155 5448 4f52 203d 207b 4275      AUTHOR = {Bu
-00008710: 736c 6165 762c 2041 6c65 7861 6e64 6572  slaev, Alexander
-00008720: 2061 6e64 2049 676c 6f76 696b 6f76 2c20   and Iglovikov, 
-00008730: 566c 6164 696d 6972 2049 2e20 616e 6420  Vladimir I. and 
-00008740: 4b68 7665 6463 6865 6e79 612c 2045 7567  Khvedchenya, Eug
-00008750: 656e 6520 616e 6420 5061 7269 6e6f 762c  ene and Parinov,
-00008760: 2041 6c65 7820 616e 6420 4472 757a 6869   Alex and Druzhi
-00008770: 6e69 6e2c 204d 696b 6861 696c 2061 6e64  nin, Mikhail and
-00008780: 204b 616c 696e 696e 2c20 416c 6578 616e   Kalinin, Alexan
-00008790: 6472 2041 2e7d 2c0a 2020 2020 5449 544c  dr A.},.    TITL
-000087a0: 4520 3d20 7b41 6c62 756d 656e 7461 7469  E = {Albumentati
-000087b0: 6f6e 733a 2046 6173 7420 616e 6420 466c  ons: Fast and Fl
-000087c0: 6578 6962 6c65 2049 6d61 6765 2041 7567  exible Image Aug
-000087d0: 6d65 6e74 6174 696f 6e73 7d2c 0a20 2020  mentations},.   
-000087e0: 204a 4f55 524e 414c 203d 207b 496e 666f   JOURNAL = {Info
-000087f0: 726d 6174 696f 6e7d 2c0a 2020 2020 564f  rmation},.    VO
-00008800: 4c55 4d45 203d 207b 3131 7d2c 0a20 2020  LUME = {11},.   
-00008810: 2059 4541 5220 3d20 7b32 3032 307d 2c0a   YEAR = {2020},.
-00008820: 2020 2020 4e55 4d42 4552 203d 207b 327d      NUMBER = {2}
-00008830: 2c0a 2020 2020 4152 5449 434c 452d 4e55  ,.    ARTICLE-NU
-00008840: 4d42 4552 203d 207b 3132 357d 2c0a 2020  MBER = {125},.  
-00008850: 2020 5552 4c20 3d20 7b68 7474 7073 3a2f    URL = {https:/
-00008860: 2f77 7777 2e6d 6470 692e 636f 6d2f 3230  /www.mdpi.com/20
-00008870: 3738 2d32 3438 392f 3131 2f32 2f31 3235  78-2489/11/2/125
-00008880: 7d2c 0a20 2020 2049 5353 4e20 3d20 7b32  },.    ISSN = {2
-00008890: 3037 382d 3234 3839 7d2c 0a20 2020 2044  078-2489},.    D
-000088a0: 4f49 203d 207b 3130 2e33 3339 302f 696e  OI = {10.3390/in
-000088b0: 666f 3131 3032 3031 3235 7d0a 7d0a 6060  fo11020125}.}.``
-000088c0: 600a                                     `.
+00008260: 207c 0a7c 5261 6e64 6f6d 4761 6d6d 6120   |.|RandomGamma 
+00008270: 2020 2020 207c 2a2a 3435 3536 20c2 b120       |**4556 .. 
+00008280: 332a 2a20 2020 2020 2020 2020 2020 2020  3**             
+00008290: 2020 2020 2020 2020 2020 2020 207c 3233               |23
+000082a0: 3020 c2b1 2031 2020 2020 2020 2020 2020  0 .. 1          
+000082b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000082c0: 2020 2020 2020 2020 2020 207c 3230 3520             |205 
+000082d0: c2b1 2031 2020 2020 2020 2020 2020 2020  .. 1            
+000082e0: 2020 2020 2020 2020 2020 207c 2d20 2020             |-   
+000082f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008300: 2020 2020 2020 2020 207c 3232 3832 20c2           |2282 .
+00008310: b120 3131 3020 2020 2020 2020 2020 2020  . 110           
+00008320: 2020 2020 2020 2020 207c 0a7c 4772 6179           |.|Gray
+00008330: 7363 616c 6520 2020 2020 2020 207c 2a2a  scale        |**
+00008340: 3732 3334 20c2 b120 342a 2a20 2020 2020  7234 .. 4**     
+00008350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008360: 2020 2020 207c 3135 3339 20c2 b120 3720       |1539 .. 7 
+00008370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008390: 2020 207c 3434 3420 c2b1 2033 2020 2020     |444 .. 3    
+000083a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000083b0: 2020 207c 3236 3036 20c2 b120 3220 2020     |2606 .. 2   
+000083c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000083d0: 2020 7c39 3138 20c2 b120 3432 2020 2020    |918 .. 42    
+000083e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000083f0: 2020 7c0a 7c43 6f6c 6f72 4a69 7474 6572    |.|ColorJitter
+00008400: 2020 2020 2020 7c2a 2a34 3532 20c2 b120        |**452 .. 
+00008410: 3433 2a2a 2020 2020 2020 2020 2020 2020  43**            
+00008420: 2020 2020 2020 2020 2020 2020 2020 7c35                |5
+00008430: 3120 c2b1 2031 2020 2020 2020 2020 2020  1 .. 1          
+00008440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008450: 2020 2020 2020 2020 2020 2020 7c35 3020              |50 
+00008460: c2b1 2031 2020 2020 2020 2020 2020 2020  .. 1            
+00008470: 2020 2020 2020 2020 2020 2020 7c32 3231              |221
+00008480: 20c2 b120 3120 2020 2020 2020 2020 2020   .. 1           
+00008490: 2020 2020 2020 2020 2020 207c 2d20 2020             |-   
+000084a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000084b0: 2020 2020 2020 2020 2020 7c0a 7c52 616e            |.|Ran
+000084c0: 646f 6d50 6572 7370 6563 7469 7665 7c2a  domPerspective|*
+000084d0: 2a34 3635 20c2 b120 312a 2a20 2020 2020  *465 .. 1**     
+000084e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000084f0: 2020 2020 2020 7c31 3231 20c2 b120 3120        |121 .. 1 
+00008500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008520: 2020 2020 7c31 3135 20c2 b120 3120 2020      |115 .. 1   
+00008530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008540: 2020 2020 7c2d 2020 2020 2020 2020 2020      |-          
+00008550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008560: 2020 7c34 3333 20c2 b120 3136 2020 2020    |433 .. 16    
+00008570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008580: 2020 7c0a 7c47 6175 7373 6961 6e42 6c75    |.|GaussianBlu
+00008590: 7220 2020 2020 7c2a 2a32 3331 3520 c2b1  r     |**2315 ..
+000085a0: 2039 2a2a 2020 2020 2020 2020 2020 2020   9**            
+000085b0: 2020 2020 2020 2020 2020 2020 2020 7c31                |1
+000085c0: 3036 20c2 b120 3220 2020 2020 2020 2020  06 .. 2         
+000085d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000085e0: 2020 2020 2020 2020 2020 2020 7c37 3220              |72 
+000085f0: c2b1 2031 2020 2020 2020 2020 2020 2020  .. 1            
+00008600: 2020 2020 2020 2020 2020 2020 7c31 3631              |161
+00008610: 20c2 b120 3120 2020 2020 2020 2020 2020   .. 1           
+00008620: 2020 2020 2020 2020 2020 207c 3132 3133             |1213
+00008630: 20c2 b120 3320 2020 2020 2020 2020 2020   .. 3           
+00008640: 2020 2020 2020 2020 2020 207c 0a7c 4d65             |.|Me
+00008650: 6469 616e 426c 7572 2020 2020 2020 207c  dianBlur       |
+00008660: 2a2a 3337 3131 20c2 b120 322a 2a20 2020  **3711 .. 2**   
+00008670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008680: 2020 2020 2020 207c 2d20 2020 2020 2020         |-       
+00008690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000086a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000086b0: 2020 2020 7c32 20c2 b120 3120 2020 2020      |2 .. 1     
+000086c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000086d0: 2020 2020 7c2d 2020 2020 2020 2020 2020      |-          
+000086e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000086f0: 2020 7c35 3636 20c2 b120 3320 2020 2020    |566 .. 3     
+00008700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008710: 2020 7c0a 7c4d 6f74 696f 6e42 6c75 7220    |.|MotionBlur 
+00008720: 2020 2020 2020 7c2a 2a32 3736 3320 c2b1        |**2763 ..
+00008730: 2032 352a 2a20 2020 2020 2020 2020 2020   25**           
+00008740: 2020 2020 2020 2020 2020 2020 2020 7c2d                |-
+00008750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008770: 2020 2020 2020 2020 2020 207c 3130 3120             |101 
+00008780: c2b1 2034 2020 2020 2020 2020 2020 2020  .. 4            
+00008790: 2020 2020 2020 2020 2020 207c 2d20 2020             |-   
+000087a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000087b0: 2020 2020 2020 2020 207c 3530 3820 c2b1           |508 ..
+000087c0: 2032 2020 2020 2020 2020 2020 2020 2020   2              
+000087d0: 2020 2020 2020 2020 207c 0a7c 506f 7374           |.|Post
+000087e0: 6572 697a 6520 2020 2020 2020 207c 2a2a  erize        |**
+000087f0: 3432 3338 20c2 b120 3531 2a2a 2020 2020  4238 .. 51**    
+00008800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008810: 2020 2020 207c 3235 3831 20c2 b120 3230       |2581 .. 20
+00008820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008840: 2020 207c 3238 3420 c2b1 2034 2020 2020     |284 .. 4    
+00008850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008860: 2020 207c 2d20 2020 2020 2020 2020 2020     |-           
+00008870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008880: 207c 3138 3933 20c2 b120 3920 2020 2020   |1893 .. 9     
+00008890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000088a0: 207c 0a7c 4a70 6567 436f 6d70 7265 7373   |.|JpegCompress
+000088b0: 696f 6e20 207c 3230 3820 c2b1 2031 2020  ion  |208 .. 1  
+000088c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000088d0: 2020 2020 2020 2020 2020 2020 207c 2d20               |- 
+000088e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000088f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008900: 2020 2020 2020 2020 2020 7c2d 2020 2020            |-    
+00008910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008920: 2020 2020 2020 2020 207c 2a2a 3639 3220           |**692 
+00008930: c2b1 2034 2a2a 2020 2020 2020 2020 2020  .. 4**          
+00008940: 2020 2020 2020 2020 7c34 3335 20c2 b120          |435 .. 
+00008950: 3120 2020 2020 2020 2020 2020 2020 2020  1               
+00008960: 2020 2020 2020 2020 7c0a 7c47 6175 7373          |.|Gauss
+00008970: 6961 6e4e 6f69 7365 2020 2020 7c36 3420  ianNoise    |64 
+00008980: c2b1 2039 2020 2020 2020 2020 2020 2020  .. 9            
+00008990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000089a0: 2020 2020 7c2d 2020 2020 2020 2020 2020      |-          
+000089b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000089c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000089d0: 207c 2d20 2020 2020 2020 2020 2020 2020   |-             
+000089e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000089f0: 7c36 3720 c2b1 2031 2020 2020 2020 2020  |67 .. 1        
+00008a00: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00008a10: 2a2a 3231 3220 c2b1 2031 362a 2a20 2020  **212 .. 16**   
+00008a20: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00008a30: 0a7c 456c 6173 7469 6320 2020 2020 2020  .|Elastic       
+00008a40: 2020 207c 2a2a 3132 3920 c2b1 2031 2a2a     |**129 .. 1**
+00008a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a60: 2020 2020 2020 2020 2020 207c 3320 c2b1             |3 ..
+00008a70: 2031 2020 2020 2020 2020 2020 2020 2020   1              
+00008a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a90: 2020 2020 2020 2020 207c 3120 c2b1 2031           |1 .. 1
+00008aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ab0: 2020 2020 2020 2020 207c 2d20 2020 2020           |-     
+00008ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ad0: 2020 2020 2020 207c 3132 3820 c2b1 2031         |128 .. 1
+00008ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008af0: 2020 2020 2020 207c 0a0a 2323 2043 6f6e         |..## Con
+00008b00: 7472 6962 7574 696e 670a 0a54 6f20 6372  tributing..To cr
+00008b10: 6561 7465 2061 2070 756c 6c20 7265 7175  eate a pull requ
+00008b20: 6573 7420 746f 2074 6865 2072 6570 6f73  est to the repos
+00008b30: 6974 6f72 792c 2066 6f6c 6c6f 7720 7468  itory, follow th
+00008b40: 6520 646f 6375 6d65 6e74 6174 696f 6e20  e documentation 
+00008b50: 6174 205b 434f 4e54 5249 4255 5449 4e47  at [CONTRIBUTING
+00008b60: 2e6d 645d 2843 4f4e 5452 4942 5554 494e  .md](CONTRIBUTIN
+00008b70: 472e 6d64 290a 0a21 5b68 7474 7073 3a2f  G.md)..![https:/
+00008b80: 2f67 6974 6875 622e 636f 6d2f 616c 6275  /github.com/albu
+00008b90: 656d 6e74 6174 696f 6e73 2d74 6561 6d2f  emntations-team/
+00008ba0: 616c 6275 6d65 6e74 6174 696f 6e2f 6772  albumentation/gr
+00008bb0: 6170 6873 2f63 6f6e 7472 6962 7574 6f72  aphs/contributor
+00008bc0: 735d 2868 7474 7073 3a2f 2f63 6f6e 7472  s](https://contr
+00008bd0: 6962 2e72 6f63 6b73 2f69 6d61 6765 3f72  ib.rocks/image?r
+00008be0: 6570 6f3d 616c 6275 6d65 6e74 6174 696f  epo=albumentatio
+00008bf0: 6e73 2d74 6561 6d2f 616c 6275 6d65 6e74  ns-team/albument
+00008c00: 6174 696f 6e73 290a 0a23 2320 436f 6d6d  ations)..## Comm
+00008c10: 756e 6974 7920 616e 6420 5375 7070 6f72  unity and Suppor
+00008c20: 740a 0a2d 205b 5477 6974 7465 725d 2868  t..- [Twitter](h
+00008c30: 7474 7073 3a2f 2f74 7769 7474 6572 2e63  ttps://twitter.c
+00008c40: 6f6d 2f61 6c62 756d 656e 7461 7469 6f6e  om/albumentation
+00008c50: 7329 0a2d 205b 4469 7363 6f72 645d 2868  s).- [Discord](h
+00008c60: 7474 7073 3a2f 2f64 6973 636f 7264 2e67  ttps://discord.g
+00008c70: 672f 414b 5072 7244 594e 4174 290a 0a23  g/AKPrrDYNAt)..#
+00008c80: 2320 436f 6d6d 656e 7473 0a0a 496e 2073  # Comments..In s
+00008c90: 6f6d 6520 7379 7374 656d 732c 2069 6e20  ome systems, in 
+00008ca0: 7468 6520 6d75 6c74 6970 6c65 2047 5055  the multiple GPU
+00008cb0: 2072 6567 696d 652c 2050 7954 6f72 6368   regime, PyTorch
+00008cc0: 206d 6179 2064 6561 646c 6f63 6b20 7468   may deadlock th
+00008cd0: 6520 4461 7461 4c6f 6164 6572 2069 6620  e DataLoader if 
+00008ce0: 4f70 656e 4356 2077 6173 2063 6f6d 7069  OpenCV was compi
+00008cf0: 6c65 6420 7769 7468 204f 7065 6e43 4c20  led with OpenCL 
+00008d00: 6f70 7469 6d69 7a61 7469 6f6e 732e 2041  optimizations. A
+00008d10: 6464 696e 6720 7468 6520 666f 6c6c 6f77  dding the follow
+00008d20: 696e 6720 7477 6f20 6c69 6e65 7320 6265  ing two lines be
+00008d30: 666f 7265 2074 6865 206c 6962 7261 7279  fore the library
+00008d40: 2069 6d70 6f72 7420 6d61 7920 6865 6c70   import may help
+00008d50: 2e20 466f 7220 6d6f 7265 2064 6574 6169  . For more detai
+00008d60: 6c73 205b 6874 7470 733a 2f2f 6769 7468  ls [https://gith
+00008d70: 7562 2e63 6f6d 2f70 7974 6f72 6368 2f70  ub.com/pytorch/p
+00008d80: 7974 6f72 6368 2f69 7373 7565 732f 3133  ytorch/issues/13
+00008d90: 3535 5d28 6874 7470 733a 2f2f 6769 7468  55](https://gith
+00008da0: 7562 2e63 6f6d 2f70 7974 6f72 6368 2f70  ub.com/pytorch/p
+00008db0: 7974 6f72 6368 2f69 7373 7565 732f 3133  ytorch/issues/13
+00008dc0: 3535 290a 0a60 6060 7079 7468 6f6e 0a63  55)..```python.c
+00008dd0: 7632 2e73 6574 4e75 6d54 6872 6561 6473  v2.setNumThreads
+00008de0: 2830 290a 6376 322e 6f63 6c2e 7365 7455  (0).cv2.ocl.setU
+00008df0: 7365 4f70 656e 434c 2846 616c 7365 290a  seOpenCL(False).
+00008e00: 6060 600a 0a23 2320 4369 7469 6e67 0a0a  ```..## Citing..
+00008e10: 4966 2079 6f75 2066 696e 6420 7468 6973  If you find this
+00008e20: 206c 6962 7261 7279 2075 7365 6675 6c20   library useful 
+00008e30: 666f 7220 796f 7572 2072 6573 6561 7263  for your researc
+00008e40: 682c 2070 6c65 6173 6520 636f 6e73 6964  h, please consid
+00008e50: 6572 2063 6974 696e 6720 5b41 6c62 756d  er citing [Album
+00008e60: 656e 7461 7469 6f6e 733a 2046 6173 7420  entations: Fast 
+00008e70: 616e 6420 466c 6578 6962 6c65 2049 6d61  and Flexible Ima
+00008e80: 6765 2041 7567 6d65 6e74 6174 696f 6e73  ge Augmentations
+00008e90: 5d28 6874 7470 733a 2f2f 7777 772e 6d64  ](https://www.md
+00008ea0: 7069 2e63 6f6d 2f32 3037 382d 3234 3839  pi.com/2078-2489
+00008eb0: 2f31 312f 322f 3132 3529 3a0a 0a60 6060  /11/2/125):..```
+00008ec0: 6269 6274 6578 0a40 4172 7469 636c 657b  bibtex.@Article{
+00008ed0: 696e 666f 3131 3032 3031 3235 2c0a 2020  info11020125,.  
+00008ee0: 2020 4155 5448 4f52 203d 207b 4275 736c    AUTHOR = {Busl
+00008ef0: 6165 762c 2041 6c65 7861 6e64 6572 2061  aev, Alexander a
+00008f00: 6e64 2049 676c 6f76 696b 6f76 2c20 566c  nd Iglovikov, Vl
+00008f10: 6164 696d 6972 2049 2e20 616e 6420 4b68  adimir I. and Kh
+00008f20: 7665 6463 6865 6e79 612c 2045 7567 656e  vedchenya, Eugen
+00008f30: 6520 616e 6420 5061 7269 6e6f 762c 2041  e and Parinov, A
+00008f40: 6c65 7820 616e 6420 4472 757a 6869 6e69  lex and Druzhini
+00008f50: 6e2c 204d 696b 6861 696c 2061 6e64 204b  n, Mikhail and K
+00008f60: 616c 696e 696e 2c20 416c 6578 616e 6472  alinin, Alexandr
+00008f70: 2041 2e7d 2c0a 2020 2020 5449 544c 4520   A.},.    TITLE 
+00008f80: 3d20 7b41 6c62 756d 656e 7461 7469 6f6e  = {Albumentation
+00008f90: 733a 2046 6173 7420 616e 6420 466c 6578  s: Fast and Flex
+00008fa0: 6962 6c65 2049 6d61 6765 2041 7567 6d65  ible Image Augme
+00008fb0: 6e74 6174 696f 6e73 7d2c 0a20 2020 204a  ntations},.    J
+00008fc0: 4f55 524e 414c 203d 207b 496e 666f 726d  OURNAL = {Inform
+00008fd0: 6174 696f 6e7d 2c0a 2020 2020 564f 4c55  ation},.    VOLU
+00008fe0: 4d45 203d 207b 3131 7d2c 0a20 2020 2059  ME = {11},.    Y
+00008ff0: 4541 5220 3d20 7b32 3032 307d 2c0a 2020  EAR = {2020},.  
+00009000: 2020 4e55 4d42 4552 203d 207b 327d 2c0a    NUMBER = {2},.
+00009010: 2020 2020 4152 5449 434c 452d 4e55 4d42      ARTICLE-NUMB
+00009020: 4552 203d 207b 3132 357d 2c0a 2020 2020  ER = {125},.    
+00009030: 5552 4c20 3d20 7b68 7474 7073 3a2f 2f77  URL = {https://w
+00009040: 7777 2e6d 6470 692e 636f 6d2f 3230 3738  ww.mdpi.com/2078
+00009050: 2d32 3438 392f 3131 2f32 2f31 3235 7d2c  -2489/11/2/125},
+00009060: 0a20 2020 2049 5353 4e20 3d20 7b32 3037  .    ISSN = {207
+00009070: 382d 3234 3839 7d2c 0a20 2020 2044 4f49  8-2489},.    DOI
+00009080: 203d 207b 3130 2e33 3339 302f 696e 666f   = {10.3390/info
+00009090: 3131 3032 3031 3235 7d0a 7d0a 6060 600a  11020125}.}.```.
```

### Comparing `albumentations-1.4.2/albumentations/augmentations/__init__.py` & `albumentations-1.4.3/albumentations/augmentations/__init__.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.2/albumentations/augmentations/blur/functional.py` & `albumentations-1.4.3/albumentations/augmentations/blur/functional.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.2/albumentations/augmentations/blur/transforms.py` & `albumentations-1.4.3/albumentations/augmentations/blur/transforms.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.2/albumentations/augmentations/crops/functional.py` & `albumentations-1.4.3/albumentations/augmentations/crops/functional.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.2/albumentations/augmentations/crops/transforms.py` & `albumentations-1.4.3/albumentations/augmentations/crops/transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -330,20 +330,19 @@
         keypoint = F.keypoint_random_crop(keypoint, crop_height, crop_width, h_start, w_start, rows, cols)
         scale_x = self.width / crop_width
         scale_y = self.height / crop_height
         return FGeometric.keypoint_scale(keypoint, scale_x, scale_y)
 
 
 class RandomSizedCrop(_BaseRandomSizedCrop):
-    """Crop a random part of the input and rescale it to some size.
+    """Crop a random portion of the input and rescale it to a specific size.
 
     Args:
         min_max_height ((int, int)): crop size limits.
-        height (int): height after crop and resize.
-        width (int): width after crop and resize.
+        size (tuple[int]): target size for the output image, i.e. (height, width) after crop and resize
         w2h_ratio (float): aspect ratio of crop.
         interpolation (OpenCV flag): flag that is used to specify the interpolation algorithm. Should be one of:
             cv2.INTER_NEAREST, cv2.INTER_LINEAR, cv2.INTER_CUBIC, cv2.INTER_AREA, cv2.INTER_LANCZOS4.
             Default: cv2.INTER_LINEAR.
         p (float): probability of applying the transform. Default: 1.
 
     Targets:
@@ -351,25 +350,57 @@
 
     Image types:
         uint8, float32
 
     """
 
     _targets = (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS)
+    _size_len = 2
 
     def __init__(
         self,
         min_max_height: Tuple[int, int],
-        height: int,
-        width: int,
+        # NOTE @zetyquickly: when (width, height) are deprecated, make 'size' non optional
+        size: Optional[Union[int, Tuple[int, int]]] = None,
+        width: Optional[int] = None,
+        height: Optional[int] = None,
+        *,
         w2h_ratio: float = 1.0,
         interpolation: int = cv2.INTER_LINEAR,
         always_apply: bool = False,
         p: float = 1.0,
     ):
+        if isinstance(size, tuple):
+            if len(size) != self._size_len:
+                message = "Size must be a tuple of two integers (height, width)."
+                raise ValueError(message)
+            height, width = size
+        elif size is None:
+            if height is None or width is None:
+                message = "If 'size' is not provided, both 'height' and 'width' must be specified."
+                raise ValueError(message)
+            size = (height, width)
+            warn(
+                "Initializing with 'height' and 'width' is deprecated. "
+                "Please use a tuple (height, width) for the 'size' argument.",
+                DeprecationWarning,
+                stacklevel=2,
+            )
+        else:
+            if width is None:
+                message = "When 'size' is an integer, 'width' must be provided."
+                raise ValueError(message)
+            height = size
+            warn(
+                "Initializing with 'size' as an integer and a separate 'width' is deprecated. "
+                "Please use a tuple (height, width) for the 'size' argument.",
+                DeprecationWarning,
+                stacklevel=2,
+            )
+
         super().__init__(height=height, width=width, interpolation=interpolation, always_apply=always_apply, p=p)
 
         self.min_max_height = min_max_height
         self.w2h_ratio = w2h_ratio
 
     def get_params(self) -> Dict[str, Union[int, float]]:
         crop_height = random.randint(self.min_max_height[0], self.min_max_height[1])
@@ -384,16 +415,15 @@
         return "min_max_height", "height", "width", "w2h_ratio", "interpolation"
 
 
 class RandomResizedCrop(_BaseRandomSizedCrop):
     """Torchvision's variant of crop a random part of the input and rescale it to some size.
 
     Args:
-        height (int): height after crop and resize.
-        width (int): width after crop and resize.
+        size (tuple[int]): target size for the output image, i.e. (height, width) after crop and resize
         scale ((float, float)): range of size of the origin size cropped
         ratio ((float, float)): range of aspect ratio of the origin aspect ratio cropped
         interpolation (OpenCV flag): flag that is used to specify the interpolation algorithm. Should be one of:
             cv2.INTER_NEAREST, cv2.INTER_LINEAR, cv2.INTER_CUBIC, cv2.INTER_AREA, cv2.INTER_LANCZOS4.
             Default: cv2.INTER_LINEAR.
         p (float): probability of applying the transform. Default: 1.
 
@@ -402,25 +432,57 @@
 
     Image types:
         uint8, float32
 
     """
 
     _targets = (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS)
+    _size_len = 2
 
     def __init__(
         self,
-        height: int,
-        width: int,
+        # NOTE @zetyquickly: when (width, height) are deprecated, make 'size' non optional
+        size: Optional[Union[int, Tuple[int, int]]] = None,
+        width: Optional[int] = None,
+        height: Optional[int] = None,
+        *,
         scale: Tuple[float, float] = (0.08, 1.0),
         ratio: Tuple[float, float] = (0.75, 1.3333333333333333),
         interpolation: int = cv2.INTER_LINEAR,
         always_apply: bool = False,
         p: float = 1.0,
     ):
+        if isinstance(size, tuple):
+            if len(size) != self._size_len:
+                message = "Size must be a tuple of two integers (height, width)."
+                raise ValueError(message)
+            height, width = size
+        elif size is None:
+            if height is None or width is None:
+                message = "If 'size' is not provided, both 'height' and 'width' must be specified."
+                raise ValueError(message)
+            size = (height, width)
+            warn(
+                "Initializing with 'height' and 'width' is deprecated. "
+                "Please use a tuple (height, width) for the 'size' argument.",
+                DeprecationWarning,
+                stacklevel=2,
+            )
+        else:
+            if width is None:
+                message = "When 'size' is an integer, 'width' must be provided."
+                raise ValueError(message)
+            height = size
+            warn(
+                "Initializing with 'size' as an integer and a separate 'width' is deprecated. "
+                "Please use a tuple (height, width) for the 'size' argument.",
+                DeprecationWarning,
+                stacklevel=2,
+            )
+
         super().__init__(height=height, width=width, interpolation=interpolation, always_apply=always_apply, p=p)
         self.scale = scale
         self.ratio = ratio
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, Union[int, float]]:
         img = params["image"]
         area = img.shape[0] * img.shape[1]
```

### Comparing `albumentations-1.4.2/albumentations/augmentations/domain_adaptation_functional.py` & `albumentations-1.4.3/albumentations/augmentations/domain_adaptation_functional.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 from albumentations.augmentations.utils import (
     clipped,
     get_opencv_dtype_from_numpy,
     preserve_shape,
 )
 
+GRAYSCALE_IMAGE_SHAPE = 2
 NON_GRAY_IMAGE_SHAPE = 3
 RGB_NUM_CHANNELS = 3
 
 __all__ = [
     "fourier_domain_adaptation",
     "apply_histogram",
     "adapt_pixel_distribution",
@@ -96,67 +97,71 @@
     initial_type = img.dtype
     transformer = {"pca": PCA, "standard": StandardScaler, "minmax": MinMaxScaler}[transform_type]()
     adapter = DomainAdapter(transformer=transformer, ref_img=ref)
     result = adapter(img).astype("float32")
     return (img.astype("float32") * (1 - weight) + result * weight).astype(initial_type)
 
 
+def low_freq_mutate(amp_src: np.ndarray, amp_trg: np.ndarray, beta: float) -> np.ndarray:
+    height, width = amp_src.shape[:2]
+    border = int(np.floor(min(height, width) * beta))
+    center_y, center_h = height // 2, width // 2
+    h1, h2 = max(0, center_y - border), min(center_y + border, height - 1)
+    w1, w2 = max(0, center_h - border), min(center_h + border, width - 1)
+    amp_src[h1:h2, w1:w2] = amp_trg[h1:h2, w1:w2]
+    return amp_src
+
+
 @clipped
 @preserve_shape
 def fourier_domain_adaptation(img: np.ndarray, target_img: np.ndarray, beta: float) -> np.ndarray:
-    img = np.squeeze(img)
-    target_img = np.squeeze(target_img)
-    # Ensure input images have the same shape
-    if img.shape != target_img.shape:
-        raise ValueError(
-            f"The source and target images must have the same shape, but got {img.shape} and {target_img.shape} "
-            "respectively."
-        )
-
-    # Convert images to float32 if not already to avoid unnecessary conversions
-    if img.dtype != np.float32:
-        img = img.astype(np.float32)
-    if target_img.dtype != np.float32:
-        target_img = target_img.astype(np.float32)
-
-    # Compute FFT of both source and target images
-    fft_src = np.fft.fft2(img, axes=(0, 1))
-    fft_trg = np.fft.fft2(target_img, axes=(0, 1))
-
-    # Extract amplitude and phase
-    amplitude_src, phase_src = np.abs(fft_src), np.angle(fft_src)
-    amplitude_trg = np.abs(fft_trg)
+    src_img = img.astype(np.float32)
+    trg_img = target_img.astype(np.float32)
 
-    # Compute border for amplitude substitution
-    height, width = img.shape[:2]
-    border = int(np.floor(min(height, width) * beta))
-    center_y, center_x = height // 2, width // 2
+    if len(src_img.shape) == GRAYSCALE_IMAGE_SHAPE:
+        src_img = np.expand_dims(src_img, axis=-1)
+    if len(trg_img.shape) == GRAYSCALE_IMAGE_SHAPE:
+        trg_img = np.expand_dims(trg_img, axis=-1)
+
+    num_channels = src_img.shape[-1]
+
+    # Prepare container for the output image
+    src_in_trg = np.zeros_like(src_img)
 
-    # Define region for amplitude substitution
-    y1, y2 = center_y - border, center_y + border
-    x1, x2 = center_x - border, center_x + border
+    for channel_id in range(num_channels):
+        # Perform FFT on each channel
+        fft_src = np.fft.fft2(src_img[:, :, channel_id])
+        fft_trg = np.fft.fft2(trg_img[:, :, channel_id])
 
-    # Directly mutate the amplitude part of the source with the target in the specified region
-    amplitude_src[y1:y2, x1:x2] = amplitude_trg[y1:y2, x1:x2]
+        # Shift the zero frequency component to the center
+        fft_src_shifted = np.fft.fftshift(fft_src)
+        fft_trg_shifted = np.fft.fftshift(fft_trg)
 
-    # Reconstruct the source image from its mutated amplitude and original phase
-    src_image_transformed = np.fft.ifft2(amplitude_src * np.exp(1j * phase_src), axes=(0, 1))
+        # Extract amplitude and phase
+        amp_src, pha_src = np.abs(fft_src_shifted), np.angle(fft_src_shifted)
+        amp_trg = np.abs(fft_trg_shifted)
 
-    # Return the real part of the transformed image
-    return np.real(src_image_transformed)
+        # Mutate the amplitude part of the source with the target
+
+        mutated_amp = low_freq_mutate(amp_src.copy(), amp_trg, beta)
+
+        # Combine the mutated amplitude with the original phase
+        fft_src_mutated = np.fft.ifftshift(mutated_amp * np.exp(1j * pha_src))
+
+        # Perform inverse FFT
+        src_in_trg_channel = np.fft.ifft2(fft_src_mutated)
+
+        # Store the result in the corresponding channel of the output image
+        src_in_trg[:, :, channel_id] = np.real(src_in_trg_channel)
+
+    return src_in_trg
 
 
 @preserve_shape
 def apply_histogram(img: np.ndarray, reference_image: np.ndarray, blend_ratio: float) -> np.ndarray:
-    # Ensure the data types match
-    if img.dtype != reference_image.dtype:
-        raise RuntimeError(
-            f"Dtype of image and reference image must be the same. Got {img.dtype} and {reference_image.dtype}."
-        )
-
     # Resize reference image only if necessary
     if img.shape[:2] != reference_image.shape[:2]:
         reference_image = cv2.resize(reference_image, dsize=(img.shape[1], img.shape[0]))
 
     img, reference_image = np.squeeze(img), np.squeeze(reference_image)
 
     # Determine if the images are multi-channel based on a predefined condition or shape analysis
```

### Comparing `albumentations-1.4.2/albumentations/augmentations/dropout/channel_dropout.py` & `albumentations-1.4.3/albumentations/augmentations/dropout/channel_dropout.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.2/albumentations/augmentations/dropout/coarse_dropout.py` & `albumentations-1.4.3/albumentations/augmentations/dropout/coarse_dropout.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.2/albumentations/augmentations/dropout/functional.py` & `albumentations-1.4.3/albumentations/augmentations/dropout/functional.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.2/albumentations/augmentations/dropout/grid_dropout.py` & `albumentations-1.4.3/albumentations/augmentations/dropout/grid_dropout.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.2/albumentations/augmentations/dropout/mask_dropout.py` & `albumentations-1.4.3/albumentations/augmentations/dropout/mask_dropout.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.2/albumentations/augmentations/dropout/xy_masking.py` & `albumentations-1.4.3/albumentations/augmentations/dropout/xy_masking.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.2/albumentations/augmentations/functional.py` & `albumentations-1.4.3/albumentations/augmentations/functional.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,16 @@
     "to_float",
     "to_gray",
     "gray_to_rgb",
     "unsharp_mask",
     "MAX_VALUES_BY_DTYPE",
     "split_uniform_grid",
     "chromatic_aberration",
+    "erode",
+    "dilate",
 ]
 
 TWO = 2
 THREE = 3
 FOUR = 4
 EIGHT = 8
 THREE_SIXTY = 360
@@ -1494,7 +1496,26 @@
     return cv2.remap(
         channel,
         map_x,
         map_y,
         interpolation=interpolation,
         borderMode=cv2.BORDER_REPLICATE,
     )
+
+
+@preserve_shape
+def erode(img: np.ndarray, kernel: np.ndarray) -> np.ndarray:
+    return cv2.erode(img, kernel, iterations=1)
+
+
+@preserve_shape
+def dilate(img: np.ndarray, kernel: np.ndarray) -> np.ndarray:
+    return cv2.dilate(img, kernel, iterations=1)
+
+
+def morphology(img: np.ndarray, kernel: np.ndarray, operation: str) -> np.ndarray:
+    if operation == "dilation":
+        return dilate(img, kernel)
+    if operation == "erosion":
+        return erode(img, kernel)
+
+    raise ValueError(f"Unsupported operation: {operation}")
```

### Comparing `albumentations-1.4.2/albumentations/augmentations/geometric/functional.py` & `albumentations-1.4.3/albumentations/augmentations/geometric/functional.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.2/albumentations/augmentations/geometric/resize.py` & `albumentations-1.4.3/albumentations/augmentations/geometric/resize.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.2/albumentations/augmentations/geometric/rotate.py` & `albumentations-1.4.3/albumentations/augmentations/geometric/rotate.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.2/albumentations/augmentations/geometric/transforms.py` & `albumentations-1.4.3/albumentations/augmentations/geometric/transforms.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.2/albumentations/augmentations/mixing/transforms.py` & `albumentations-1.4.3/albumentations/augmentations/mixing/transforms.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.2/albumentations/augmentations/transforms.py` & `albumentations-1.4.3/albumentations/augmentations/transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,26 +10,26 @@
 import cv2
 import numpy as np
 from scipy import special
 from scipy.ndimage import gaussian_filter
 
 from albumentations import random_utils
 from albumentations.augmentations.blur.functional import blur
-from albumentations.augmentations.functional import split_uniform_grid
 from albumentations.augmentations.utils import (
     get_num_channels,
     is_grayscale_image,
     is_rgb_image,
 )
 from albumentations.core.transforms_interface import DualTransform, ImageOnlyTransform, Interpolation, NoOp, to_tuple
 from albumentations.core.types import (
     BoxInternalType,
     ChromaticAberrationMode,
     ImageMode,
     KeypointInternalType,
+    MorphologyMode,
     ScaleFloatType,
     ScaleIntType,
     ScaleType,
     SpatterMode,
     Targets,
     image_modes,
 )
@@ -75,17 +75,18 @@
     "Superpixels",
     "TemplateTransform",
     "RingingOvershoot",
     "UnsharpMask",
     "PixelDropout",
     "Spatter",
     "ChromaticAberration",
+    "Morphological",
 ]
 
-HUNDRED = 100
+MAX_JPEG_QUALITY = 100
 TWENTY = 20
 FIVE = 5
 THREE = 3
 TWO = 2
 
 
 class RandomGridShuffle(DualTransform):
@@ -148,15 +149,15 @@
             "Keypoint not in any tile, returning it unchanged. This is unexpected and should be investigated.",
             RuntimeWarning,
         )
         return keypoint
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, Any]:
         # Generate the original grid
-        original_tiles = split_uniform_grid(params["image"].shape[:2], self.grid)
+        original_tiles = F.split_uniform_grid(params["image"].shape[:2], self.grid)
 
         # Copy the original grid to keep track of the initial positions
         indexed_tiles = np.array(list(enumerate(original_tiles)), dtype=object)
 
         # Shuffle the tiles while keeping track of original indices
         random_utils.shuffle(indexed_tiles)
 
@@ -255,17 +256,17 @@
 
         self.compression_type = ImageCompression.ImageCompressionType(compression_type)
         low_thresh_quality_assert = 0
 
         if self.compression_type == ImageCompression.ImageCompressionType.WEBP:
             low_thresh_quality_assert = 1
 
-        if not low_thresh_quality_assert <= quality_lower <= HUNDRED:
+        if not low_thresh_quality_assert <= quality_lower <= MAX_JPEG_QUALITY:
             raise ValueError(f"Invalid quality_lower. Got: {quality_lower}")
-        if not low_thresh_quality_assert <= quality_upper <= HUNDRED:
+        if not low_thresh_quality_assert <= quality_upper <= MAX_JPEG_QUALITY:
             raise ValueError(f"Invalid quality_upper. Got: {quality_upper}")
 
         self.quality_lower = quality_lower
         self.quality_upper = quality_upper
 
     def apply(self, img: np.ndarray, quality: int = 100, image_type: str = ".jpg", **params: Any) -> np.ndarray:
         if img.ndim != TWO and img.shape[-1] not in (1, 3, 4):
@@ -497,15 +498,15 @@
         if rain_type not in ["drizzle", "heavy", "torrential", None]:
             msg = "raint_type must be one of ({}). Got: {}".format(["drizzle", "heavy", "torrential", None], rain_type)
             raise ValueError(msg)
         if not -TWENTY <= slant_lower <= slant_upper <= TWENTY:
             raise ValueError(f"Invalid combination of slant_lower and slant_upper. Got: {(slant_lower, slant_upper)}")
         if not 1 <= drop_width <= FIVE:
             raise ValueError(f"drop_width must be in range [1, 5]. Got: {drop_width}")
-        if not 0 <= drop_length <= HUNDRED:
+        if not 0 <= drop_length <= MAX_JPEG_QUALITY:
             raise ValueError(f"drop_length must be in range [0, 100]. Got: {drop_length}")
         if not 0 <= brightness_coefficient <= 1:
             raise ValueError(f"brightness_coefficient must be in range [0, 1]. Got: {brightness_coefficient}")
 
         self.slant_lower = slant_lower
         self.slant_upper = slant_upper
 
@@ -2862,7 +2863,77 @@
         # Unmatch the sign of b to a
         if (a < 0 and b < 0) or (a > 0 and b > 0):
             b = -b
         return b
 
     def get_transform_init_args_names(self) -> Tuple[str, str, str, str]:
         return "primary_distortion_limit", "secondary_distortion_limit", "mode", "interpolation"
+
+
+class Morphological(DualTransform):
+    """Apply a morphological operation (dilation or erosion) to an image,
+    with particular value for enhancing document scans.
+
+    Morphological operations modify the structure of the image.
+    Dilation expands the white (foreground) regions in a binary or grayscale image, while erosion shrinks them.
+    These operations are beneficial in document processing, for example:
+    - Dilation helps in closing up gaps within text or making thin lines thicker,
+        enhancing legibility for OCR (Optical Character Recognition).
+    - Erosion can remove small white noise and detach connected objects,
+        making the structure of larger objects more pronounced.
+
+    Args:
+        scale (int or tuple/list of int): Specifies the size of the structuring element (kernel) used for the operation.
+            - If an integer is provided, a square kernel of that size will be used.
+            - If a tuple or list is provided, it should contain two integers representing the minimum
+                and maximum sizes for the dilation kernel.
+        operation (str, optional): The morphological operation to apply. Options are 'dilation' or 'erosion'.
+            Default is 'dilation'.
+        always_apply (bool, optional): Whether to always apply this transformation. Default is False.
+        p (float, optional): The probability of applying this transformation. Default is 0.5.
+
+    Targets:
+        image, mask
+
+    Image types:
+        uint8, float32
+
+    Reference:
+        https://github.com/facebookresearch/nougat
+
+    Example:
+        >>> import albumentations as A
+        >>> transform = A.Compose([
+        >>>     A.Morphological(scale=(2, 3), operation='dilation', p=0.5)
+        >>> ])
+        >>> image = transform(image=image)["image"]
+    """
+
+    _targets = (Targets.IMAGE, Targets.MASK)
+
+    def __init__(
+        self,
+        scale: ScaleIntType = (2, 3),
+        operation: MorphologyMode = "dilation",
+        always_apply: bool = False,
+        p: float = 0.5,
+    ):
+        super().__init__(always_apply, p)
+        self.scale = to_tuple(scale, scale)
+        self.operation = operation
+
+    def apply(self, img: np.ndarray, kernel: Tuple[int, int], **params: Any) -> np.ndarray:
+        return F.morphology(img, kernel, self.operation)
+
+    def apply_to_mask(self, mask: np.ndarray, kernel: Tuple[int, int], **params: Any) -> np.ndarray:
+        return F.morphology(mask, kernel, self.operation)
+
+    def get_params(self) -> Dict[str, float]:
+        kernel = cv2.getStructuringElement(
+            cv2.MORPH_ELLIPSE, tuple(random_utils.randint(self.scale[0], self.scale[1], 2))
+        )
+        return {
+            "kernel": kernel,
+        }
+
+    def get_transform_init_args_names(self) -> Tuple[str, ...]:
+        return ("scale", "operation")
```

### Comparing `albumentations-1.4.2/albumentations/augmentations/utils.py` & `albumentations-1.4.3/albumentations/augmentations/utils.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.2/albumentations/core/bbox_utils.py` & `albumentations-1.4.3/albumentations/core/bbox_utils.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.2/albumentations/core/composition.py` & `albumentations-1.4.3/albumentations/core/composition.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.2/albumentations/core/keypoints_utils.py` & `albumentations-1.4.3/albumentations/core/keypoints_utils.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.2/albumentations/core/serialization.py` & `albumentations-1.4.3/albumentations/core/serialization.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.2/albumentations/core/transforms_interface.py` & `albumentations-1.4.3/albumentations/core/transforms_interface.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.2/albumentations/core/types.py` & `albumentations-1.4.3/albumentations/core/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 image_modes = ["cv", "pil"]
 ImageMode = Literal["cv", "pil"]
 
 
 SpatterMode = Literal["rain", "mud"]
 ChromaticAberrationMode = Literal["green_purple", "red_blue", "random"]
 
+MorphologyMode = Literal["erosion", "dilation"]
+
 
 class ReferenceImage(TypedDict):
     image: Union[str, Path]
     mask: NotRequired[np.ndarray]
     global_label: NotRequired[np.ndarray]
     bbox: NotRequired[BoxType]
     keypoints: NotRequired[KeypointType]
```

### Comparing `albumentations-1.4.2/albumentations/core/utils.py` & `albumentations-1.4.3/albumentations/core/utils.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.2/albumentations/pytorch/transforms.py` & `albumentations-1.4.3/albumentations/pytorch/transforms.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.2/albumentations/random_utils.py` & `albumentations-1.4.3/albumentations/random_utils.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.2/albumentations.egg-info/PKG-INFO` & `albumentations-1.4.3/albumentations.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: albumentations
-Version: 1.4.2
+Version: 1.4.3
 Summary: An efficient library for image augmentation, providing extensive transformations to support machine learning and computer vision tasks.
 Home-page: https://albumentations.ai
 Author: Vladimir I. Iglovikov, Mikhail Druzhinin, Alex Parinov, Alexander Buslaev, Eugene Khvedchenya
 License: MIT
 Keywords: image augmentation,data augmentation,computer vision,deep learning,machine learning,image processing,artificial intelligence,augmentation library,image transformation,vision augmentation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -37,15 +37,15 @@
 # Albumentations
 
 [![PyPI version](https://badge.fury.io/py/albumentations.svg)](https://badge.fury.io/py/albumentations)
 ![CI](https://github.com/albumentations-team/albumentations/workflows/CI/badge.svg)
 [![License: MIT](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://opensource.org/licenses/MIT)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
-[Discord](https://discord.gg/AKPrrDYNAt) | [Twitter](https://twitter.com/albumentations) | [Docs](https://albumentations.ai/docs/)
+[Docs](https://albumentations.ai/docs/) | [Discord](https://discord.gg/AKPrrDYNAt) | [Twitter](https://twitter.com/albumentations) | [LinkedIn](https://www.linkedin.com/company/100504475/)
 
 Albumentations is a Python library for image augmentation. Image augmentation is used in deep learning and computer vision tasks to increase the quality of trained models. The purpose of image augmentation is to create new training samples from the existing data.
 
 Here is an example of how you can apply some [pixel-level](#pixel-level-transforms) augmentations from Albumentations to create new images from the original one:
 ![parrot](https://habrastorage.org/webt/bd/ne/rv/bdnerv5ctkudmsaznhw4crsdfiw.jpeg)
 
 ## Why Albumentations
@@ -257,23 +257,23 @@
 | [Flip](https://albumentations.ai/docs/api_reference/augmentations/geometric/transforms/#albumentations.augmentations.geometric.transforms.Flip)                                 | ✓     | ✓    | ✓      | ✓         |
 | [GridDistortion](https://albumentations.ai/docs/api_reference/augmentations/geometric/transforms/#albumentations.augmentations.geometric.transforms.GridDistortion)             | ✓     | ✓    | ✓      |           |
 | [GridDropout](https://albumentations.ai/docs/api_reference/augmentations/dropout/grid_dropout/#albumentations.augmentations.dropout.grid_dropout.GridDropout)                   | ✓     | ✓    |        |           |
 | [HorizontalFlip](https://albumentations.ai/docs/api_reference/augmentations/geometric/transforms/#albumentations.augmentations.geometric.transforms.HorizontalFlip)             | ✓     | ✓    | ✓      | ✓         |
 | [Lambda](https://albumentations.ai/docs/api_reference/augmentations/transforms/#albumentations.augmentations.transforms.Lambda)                                                 | ✓     | ✓    | ✓      | ✓         |
 | [LongestMaxSize](https://albumentations.ai/docs/api_reference/augmentations/geometric/resize/#albumentations.augmentations.geometric.resize.LongestMaxSize)                     | ✓     | ✓    | ✓      | ✓         |
 | [MaskDropout](https://albumentations.ai/docs/api_reference/augmentations/dropout/mask_dropout/#albumentations.augmentations.dropout.mask_dropout.MaskDropout)                   | ✓     | ✓    |        |           |
+| [Morphological](https://albumentations.ai/docs/api_reference/augmentations/transforms/#albumentations.augmentations.transforms.Morphological)                                   | ✓     | ✓    |        |           |
 | [NoOp](https://albumentations.ai/docs/api_reference/core/transforms_interface/#albumentations.core.transforms_interface.NoOp)                                                   | ✓     | ✓    | ✓      | ✓         |
 | [OpticalDistortion](https://albumentations.ai/docs/api_reference/augmentations/geometric/transforms/#albumentations.augmentations.geometric.transforms.OpticalDistortion)       | ✓     | ✓    | ✓      |           |
 | [PadIfNeeded](https://albumentations.ai/docs/api_reference/augmentations/geometric/transforms/#albumentations.augmentations.geometric.transforms.PadIfNeeded)                   | ✓     | ✓    | ✓      | ✓         |
 | [Perspective](https://albumentations.ai/docs/api_reference/augmentations/geometric/transforms/#albumentations.augmentations.geometric.transforms.Perspective)                   | ✓     | ✓    | ✓      | ✓         |
 | [PiecewiseAffine](https://albumentations.ai/docs/api_reference/augmentations/geometric/transforms/#albumentations.augmentations.geometric.transforms.PiecewiseAffine)           | ✓     | ✓    | ✓      | ✓         |
 | [PixelDropout](https://albumentations.ai/docs/api_reference/augmentations/transforms/#albumentations.augmentations.transforms.PixelDropout)                                     | ✓     | ✓    |        |           |
 | [RandomCrop](https://albumentations.ai/docs/api_reference/augmentations/crops/transforms/#albumentations.augmentations.crops.transforms.RandomCrop)                             | ✓     | ✓    | ✓      | ✓         |
 | [RandomCropFromBorders](https://albumentations.ai/docs/api_reference/augmentations/crops/transforms/#albumentations.augmentations.crops.transforms.RandomCropFromBorders)       | ✓     | ✓    | ✓      | ✓         |
-| [RandomCropNearBBox](https://albumentations.ai/docs/api_reference/augmentations/crops/transforms/#albumentations.augmentations.crops.transforms.RandomCropNearBBox)             | ✓     | ✓    | ✓      | ✓         |
 | [RandomGridShuffle](https://albumentations.ai/docs/api_reference/augmentations/transforms/#albumentations.augmentations.transforms.RandomGridShuffle)                           | ✓     | ✓    |        | ✓         |
 | [RandomResizedCrop](https://albumentations.ai/docs/api_reference/augmentations/crops/transforms/#albumentations.augmentations.crops.transforms.RandomResizedCrop)               | ✓     | ✓    | ✓      | ✓         |
 | [RandomRotate90](https://albumentations.ai/docs/api_reference/augmentations/geometric/rotate/#albumentations.augmentations.geometric.rotate.RandomRotate90)                     | ✓     | ✓    | ✓      | ✓         |
 | [RandomScale](https://albumentations.ai/docs/api_reference/augmentations/geometric/resize/#albumentations.augmentations.geometric.resize.RandomScale)                           | ✓     | ✓    | ✓      | ✓         |
 | [RandomSizedBBoxSafeCrop](https://albumentations.ai/docs/api_reference/augmentations/crops/transforms/#albumentations.augmentations.crops.transforms.RandomSizedBBoxSafeCrop)   | ✓     | ✓    | ✓      |           |
 | [RandomSizedCrop](https://albumentations.ai/docs/api_reference/augmentations/crops/transforms/#albumentations.augmentations.crops.transforms.RandomSizedCrop)                   | ✓     | ✓    | ✓      | ✓         |
 | [Resize](https://albumentations.ai/docs/api_reference/augmentations/geometric/resize/#albumentations.augmentations.geometric.resize.Resize)                                     | ✓     | ✓    | ✓      | ✓         |
@@ -307,45 +307,57 @@
 
 ![vistas](https://habrastorage.org/webt/rz/-h/3j/rz-h3jalbxic8o_fhucxysts4tc.jpeg)
 
 ### Keypoints augmentation
 
 <img src="https://habrastorage.org/webt/e-/6k/z-/e-6kz-fugp2heak3jzns3bc-r8o.jpeg" width=100%>
 
-
 ## Benchmarking results
 
 To run the benchmark yourself, follow the instructions in [benchmark/README.md](https://github.com/albumentations-team/albumentations/blob/master/benchmark/README.md)
 
 Results for running the benchmark on the first 2000 images from the ImageNet validation set using an AMD Ryzen Threadripper 3970X CPU.
-All outputs are converted to a contiguous NumPy array with the np.uint8 data type.
 The table shows how many images per second can be processed on a single core; higher is better.
 
-
-|                      |albumentations<br><small>1.4.0</small>|imgaug<br><small>0.4.0</small>|torchvision<br><small>0.17.0</small>|keras<br><small>2.15.0</small>|augmentor<br><small>0.2.12</small>|solt<br><small>0.1.9</small>|
-|----------------------|--------------------------------------|------------------------------|------------------------------------|------------------------------|----------------------------------|----------------------------|
-|HorizontalFlip        |**14816**                             |                          5982|                                3288|                          2172|                              2942|                        8601|
-|VerticalFlip          |**12032**                             |                          6589|                                3894|                          1843|                              3591|                        7799|
-|Rotate                |**600**                               |                           505|                                 255|                            21|                                93|                         553|
-|ShiftScaleRotate      |**932**                               |                           685|                                 224|-                             |-                                 |-                           |
-|BrightnessContrast    |**4737**                              |                          1424|                                 257|                           523|                               257|                        2064|
-|ShiftRGB              |**4758**                              |                          2479|-                                   |                           251|-                                 |-                           |
-|ShiftHSV              |**878**                               |                           395|                                  95|                           112|-                                 |                         251|
-|RandomGamma           |**4871**                              |-                             |                                1509|                           286|-                                 |                        1540|
-|Grayscale             |**7790**                              |                          1179|                                1388|                           698|                              2567|                        2737|
-|RandomCrop64          |**201298**                            |                          6013|                               64320|                          1011|                             61870|                       26260|
-|PadToSize512          |**8156**                              |-                             |                                1051|-                             |-                                 |                        5851|
-|Resize512             |**2667**                              |                          1777|                                 407|                           517|                               409|                        2450|
-|RandomSizedCrop_64_512|**5224**                              |                          2170|                                 668|                           378|                               670|                        4120|
-|Equalize              |**1094**                              |                           561|-                                   |-                             |                               984|-                           |
-|Multiply              |**4680**                              |                          2623|-                                   |-                             |-                                 |-                           |
-|MultiplyElementwise   |**4532**                              |                          1007|-                                   |                           453|-                                 |-                           |
-|ColorJitter           |**544**                               |                           108|                                  84|                           116|-                                 |-                           |
-
-Python and library versions: Python 3.10.13, numpy 1.26.4, pillow-simd 10.2.0, opencv-python 4.9.0.80, scikit-image 0.22.0, scipy 1.12.0.
+| Library | Version |
+|---------|---------|
+| Python | 3.10.13 (main, Sep 11 2023, 13:44:35) [GCC 11.2.0] |
+| albumentations | 1.4.1 |
+| imgaug | 0.4.0 |
+| torchvision | 0.17.1+rocm5.7 |
+| numpy | 1.26.4 |
+| opencv-python-headless | 4.9.0.80 |
+| scikit-image | 0.22.0 |
+| scipy | 1.12.0 |
+| pillow | 10.2.0 |
+| kornia | 0.7.2 |
+| augly | 1.0.0 |
+
+|                 |albumentations<br><small>1.4.0</small>|torchvision<br><small>0.17.1+rocm5.7</small>|kornia<br><small>0.7.2</small>|augly<br><small>1.0.0</small>|imgaug<br><small>0.4.0</small>|
+|-----------------|--------------------------------------|--------------------------------------------|------------------------------|-----------------------------|------------------------------|
+|HorizontalFlip   |**9843 ± 2135**                       |2436 ± 29                                   |1014 ± 3                      |3663 ± 18                    |4884 ± 51                     |
+|VerticalFlip     |**9898 ± 18**                         |2570 ± 37                                   |1024 ± 4                      |5325 ± 13                    |8683 ± 5                      |
+|Rotate           |610 ± 4                               |153 ± 2                                     |204 ± 1                       |**626 ± 3**                  |499 ± 5                       |
+|Affine           |**1705 ± 67**                         |159 ± 1                                     |200 ± 1                       |-                            |663 ± 24                      |
+|Equalize         |**1061 ± 14**                         |337 ± 1                                     |77 ± 1                        |-                            |845 ± 33                      |
+|RandomCrop64     |**203197 ± 2105**                     |15931 ± 27                                  |837 ± 2                       |21858 ± 362                  |5681 ± 96                     |
+|RandomResizedCrop|**2998 ± 30**                         |1160 ± 4                                    |190 ± 1                       |-                            |-                             |
+|ShiftRGB         |1400 ± 3                              |-                                           |435 ± 1                       |-                            |**1528 ± 6**                  |
+|Resize           |**2581 ± 3**                          |1239 ± 1                                    |197 ± 1                       |431 ± 1                      |1728 ± 1                      |
+|RandomGamma      |**4556 ± 3**                          |230 ± 1                                     |205 ± 1                       |-                            |2282 ± 110                    |
+|Grayscale        |**7234 ± 4**                          |1539 ± 7                                    |444 ± 3                       |2606 ± 2                     |918 ± 42                      |
+|ColorJitter      |**452 ± 43**                          |51 ± 1                                      |50 ± 1                        |221 ± 1                      |-                             |
+|RandomPerspective|**465 ± 1**                           |121 ± 1                                     |115 ± 1                       |-                            |433 ± 16                      |
+|GaussianBlur     |**2315 ± 9**                          |106 ± 2                                     |72 ± 1                        |161 ± 1                      |1213 ± 3                      |
+|MedianBlur       |**3711 ± 2**                          |-                                           |2 ± 1                         |-                            |566 ± 3                       |
+|MotionBlur       |**2763 ± 25**                         |-                                           |101 ± 4                       |-                            |508 ± 2                       |
+|Posterize        |**4238 ± 51**                         |2581 ± 20                                   |284 ± 4                       |-                            |1893 ± 9                      |
+|JpegCompression  |208 ± 1                               |-                                           |-                             |**692 ± 4**                  |435 ± 1                       |
+|GaussianNoise    |64 ± 9                                |-                                           |-                             |67 ± 1                       |**212 ± 16**                  |
+|Elastic          |**129 ± 1**                           |3 ± 1                                       |1 ± 1                         |-                            |128 ± 1                       |
 
 ## Contributing
 
 To create a pull request to the repository, follow the documentation at [CONTRIBUTING.md](CONTRIBUTING.md)
 
 ![https://github.com/albuemntations-team/albumentation/graphs/contributors](https://contrib.rocks/image?repo=albumentations-team/albumentations)
```

### Comparing `albumentations-1.4.2/pyproject.toml` & `albumentations-1.4.3/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,19 @@
 # NOTE: you have to use single-quoted strings in TOML for regular expressions.
 # It's the equivalent of r-strings in Python.  Multiline strings are treated as
 # verbose regular expressions by Black.  Use [ ] to denote a significant space
 # character.
 
-[tool.mypy]
-python_version = "3.8"
-ignore_missing_imports = true
-follow_imports = "silent"
-warn_redundant_casts = true
-warn_unused_ignores = true
-disallow_any_generics = true
-check_untyped_defs = true
-no_implicit_reexport = true
-
-# for strict mypy: (this is the tricky one :-))
-disallow_untyped_defs = true
 
+[build-system]
+build-backend = "setuptools.build_meta"
+requires = [
+  "setuptools",
+  "wheel",
+]
 
 [tool.ruff]
 # Exclude a variety of commonly ignored directories.
 exclude = [
     ".bzr",
     ".direnv",
     ".eggs",
@@ -43,31 +37,127 @@
     "buck-out",
     "build",
     "dist",
     "node_modules",
     "site-packages",
     "venv",
     "tests",
-    "benchmark",
     "setup.py",
-    "tools"
+    "tools",
 ]
 
-# Same as Black.
 line-length = 120
 indent-width = 4
 
 # Assume Python 3.8
 target-version = "py38"
 
 [tool.ruff.lint]
 explicit-preview-rules = true
 
-select = ["F", "E", "W", "C90", "I", "N", "D", "UP", "YTT", "ANN", "ASYNC", "TRIO", "S", "BLE", "FBT", "B", "A", "COM", "CPY", "C4", "DTZ", "T10", "DJ", "EM", "EXE", "ISC", "ICN", "G", "INP", "PIE", "T20", "PYI", "PT", "Q", "RSE", "RET", "SLF", "SLOT", "SIM", "TID", "TCH", "INT", "ARG", "PTH", "TD", "FIX", "ERA", "PD", "PGH", "PL", "TRY", "FLY", "NPY", "PERF", "FURB", "LOG", "RUF"]
-ignore = [ "ANN101", "D107", "ANN401", "ANN204", "ARG002", "S311", "F403", "PLR0913", "FBT001", "FBT002", "ISC001", "COM812", "ANN102", "EM102", "TRY003", "D401", "A002", "PTH123", "B028", "ARG001", "ARG005", "B028", "N812", "FBT003", "B027", "D104", "D100", "D103", "D102", "D415", "D101", "D205", "D105", "D417"]
+select = [
+    "F",
+    "E",
+    "W",
+    "C90",
+    "I",
+    "N",
+    "D",
+    "UP",
+    "YTT",
+    "ANN",
+    "ASYNC",
+    "TRIO",
+    "S",
+    "BLE",
+    "FBT",
+    "B",
+    "A",
+    "COM",
+    "CPY",
+    "C4",
+    "DTZ",
+    "T10",
+    "DJ",
+    "EM",
+    "EXE",
+    "ISC",
+    "ICN",
+    "G",
+    "INP",
+    "PIE",
+    "T20",
+    "PYI",
+    "PT",
+    "Q",
+    "RSE",
+    "RET",
+    "SLF",
+    "SLOT",
+    "SIM",
+    "TID",
+    "TCH",
+    "INT",
+    "ARG",
+    "PTH",
+    "TD",
+    "FIX",
+    "ERA",
+    "PD",
+    "PGH",
+    "PL",
+    "TRY",
+    "FLY",
+    "NPY",
+    "PERF",
+    "FURB",
+    "LOG",
+    "RUF",
+]
+ignore = [
+    "ANN101",
+    "D107",
+    "ANN401",
+    "ANN204",
+    "ARG002",
+    "S311",
+    "F403",
+    "PLR0913",
+    "FBT001",
+    "FBT002",
+    "ISC001",
+    "COM812",
+    "ANN102",
+    "EM102",
+    "TRY003",
+    "D401",
+    "A002",
+    "PTH123",
+    "B028",
+    "ARG001",
+    "ARG005",
+    "B028",
+    "N812",
+    "FBT003",
+    "B027",
+    "D104",
+    "D100",
+    "D103",
+    "D102",
+    "D415",
+    "D101",
+    "D205",
+    "D105",
+    "D417",
+    "PD901",
+    "B023",
+    "N801",
+    "T201",
+    "PERF203",
+]
 
 # Allow fix for all enabled rules (when `--fix`) is provided.
 fixable = ["ALL"]
 unfixable = []
 
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
@@ -83,7 +173,20 @@
 skip-magic-trailing-comma = false
 
 # Like Black, automatically detect the appropriate line ending.
 line-ending = "auto"
 
 [tool.ruff.lint.pydocstyle]
 convention = "google"
+
+[tool.mypy]
+python_version = "3.8"
+ignore_missing_imports = true
+follow_imports = "silent"
+warn_redundant_casts = true
+warn_unused_ignores = true
+disallow_any_generics = true
+check_untyped_defs = true
+no_implicit_reexport = true
+
+# for strict mypy: (this is the tricky one :-))
+disallow_untyped_defs = true
```

### Comparing `albumentations-1.4.2/setup.py` & `albumentations-1.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.2/tests/test_augmentations.py` & `albumentations-1.4.3/tests/test_augmentations.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.2/tests/test_bbox.py` & `albumentations-1.4.3/tests/test_bbox.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.2/tests/test_core.py` & `albumentations-1.4.3/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.2/tests/test_functional.py` & `albumentations-1.4.3/tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.2/tests/test_functional_cutout.py` & `albumentations-1.4.3/tests/test_functional_cutout.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.2/tests/test_functional_mixing.py` & `albumentations-1.4.3/tests/test_functional_mixing.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.2/tests/test_keypoint.py` & `albumentations-1.4.3/tests/test_keypoint.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.2/tests/test_mixing.py` & `albumentations-1.4.3/tests/test_mixing.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.2/tests/test_pytorch.py` & `albumentations-1.4.3/tests/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.2/tests/test_random.py` & `albumentations-1.4.3/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.2/tests/test_serialization.py` & `albumentations-1.4.3/tests/test_serialization.py`

 * *Files 1% similar despite different names*

```diff
@@ -446,14 +446,15 @@
             shift_x=10,
             shift_y=20,
             random_offset=True,
             fill_value=10,
             mask_fill_value=20,
         )
     ],
+    [A.Morphological, {}]
 ]
 
 AUGMENTATION_CLS_EXCEPT = {
     A.FDA,
     A.HistogramMatching,
     A.PixelDistributionAdaptation,
     A.Lambda,
@@ -540,15 +541,16 @@
             A.RandomGridShuffle,
             A.MaskDropout,
             A.OpticalDistortion,
             A.TemplateTransform,
             A.XYMasking,
             A.MixUp,
             A.CropNonEmptyMaskIfExists,
-            A.GridDropout
+            A.GridDropout,
+            A.Morphological
         },
     ),
 )
 @pytest.mark.parametrize("p", [0.5, 1])
 @pytest.mark.parametrize("seed", TEST_SEEDS)
 @pytest.mark.parametrize("always_apply", (False, True))
 def test_augmentations_for_bboxes_serialization(
@@ -603,15 +605,16 @@
             A.GridDistortion,
             A.GridDropout,
             A.MaskDropout,
             A.OpticalDistortion,
             A.RandomSizedBBoxSafeCrop,
             A.BBoxSafeRandomCrop,
             A.TemplateTransform,
-            A.MixUp
+            A.MixUp,
+            A.Morphological
         },
     ),
 )
 @pytest.mark.parametrize("p", [0.5, 1])
 @pytest.mark.parametrize("seed", TEST_SEEDS)
 @pytest.mark.parametrize("always_apply", (False, True))
 def test_augmentations_for_keypoints_serialization(augmentation_cls, params, p, seed, image, keypoints, always_apply):
```

### Comparing `albumentations-1.4.2/tests/test_targets.py` & `albumentations-1.4.3/tests/test_targets.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,32 +59,28 @@
     A.RandomCrop: (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS),
     A.RandomCropFromBorders: (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS),
     A.RandomResizedCrop: (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS),
     A.CropNonEmptyMaskIfExists: (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS),
     A.CoarseDropout: (Targets.IMAGE, Targets.MASK, Targets.KEYPOINTS),
     A.Crop: (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS),
     A.CropAndPad: (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS),
-    A.CropNonEmptyMaskIfExists: (Targets.IMAGE, Targets.MASK),
     A.Flip: (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS),
     A.VerticalFlip: (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS),
     A.HorizontalFlip: (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS),
     A.PadIfNeeded: (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS),
     A.RandomScale: (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS),
     A.XYMasking: (Targets.IMAGE, Targets.MASK, Targets.KEYPOINTS),
     A.NoOp: (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS, Targets.GLOBAL_LABEL),
     A.Resize: (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS),
     A.Rotate: (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS),
     A.RandomRotate90: (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS),
-    A.MaskDropout: (Targets.IMAGE, Targets.MASK),
-    A.PixelDropout: (Targets.IMAGE, Targets.MASK),
     A.Transpose: (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS),
     A.SmallestMaxSize: (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS),
     A.ShiftScaleRotate: (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS),
     A.ElasticTransform: (Targets.IMAGE, Targets.MASK, Targets.BBOXES),
-    A.GridDropout: (Targets.IMAGE, Targets.MASK),
     A.GridDistortion: (Targets.IMAGE, Targets.MASK, Targets.BBOXES),
     A.LongestMaxSize: (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS),
     A.PiecewiseAffine: (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS),
     A.RandomSizedCrop: (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS),
     A.RandomCropFromBorders: (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS),
     A.RandomGridShuffle: (Targets.IMAGE, Targets.MASK, Targets.KEYPOINTS),
     A.OpticalDistortion: (Targets.IMAGE, Targets.MASK, Targets.BBOXES),
@@ -158,13 +154,13 @@
                 "read_fn": lambda x: x,
             },
         },
     ),
 )
 def test_dual(augmentation_cls, params):
     aug = augmentation_cls(p=1, **params)
-    assert set(aug._targets) == set(DUAL_TARGETS[augmentation_cls])
+    assert set(aug._targets) == set(DUAL_TARGETS.get(augmentation_cls, {Targets.IMAGE, Targets.MASK}))
     assert set(aug._targets) <= get_targets_from_methods(augmentation_cls)
 
     targets_from_docstring = {str2target[target] for target in  extract_targets_from_docstring(augmentation_cls)}
 
     assert set(aug._targets) == targets_from_docstring
```

### Comparing `albumentations-1.4.2/tests/test_transforms.py` & `albumentations-1.4.3/tests/test_transforms.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import random
 from functools import partial
 
 import cv2
 import numpy as np
 import pytest
+import warnings
+from torchvision import transforms as torch_transforms
 
 import albumentations as A
 import albumentations.augmentations.functional as F
 import albumentations.augmentations.geometric.functional as FGeometric
 from albumentations.augmentations.blur.functional import gaussian_blur
 
 from .utils import get_dual_transforms, get_image_only_transforms, get_transforms, set_seed
@@ -1349,7 +1351,66 @@
     ],
 )
 def test_spatter_incorrect_color(unsupported_color, mode, message):
     with pytest.raises(ValueError) as exc_info:
         A.Spatter(mode=mode, color=unsupported_color)
 
     assert str(exc_info.value).startswith(message)
+
+@pytest.mark.parametrize("height, width", [(100, 200), (200, 100)])
+@pytest.mark.parametrize("scale", [(0.08, 1.0), (0.5, 1.0)])
+@pytest.mark.parametrize("ratio", [(0.75, 1.33), (1.0, 1.0)])
+def test_random_crop_interfaces_vs_torchvision(height, width, scale, ratio):
+    # NOTE: below will fail when height, width is no longer expected as first two positional arguments
+    transform_albu = A.RandomResizedCrop(height, width, scale=scale, ratio=ratio, p=1)
+    transform_albu_new = A.RandomResizedCrop(size=(height, width), scale=scale, ratio=ratio, p=1)
+
+    image = np.random.randint(0, 256, (224, 224, 3), dtype=np.uint8)
+    transformed_image_albu = transform_albu(image=image)['image']
+    transformed_image_albu_new = transform_albu_new(image=image)['image']
+
+    # PyTorch equivalent operation
+    transform_pt = torch_transforms.RandomResizedCrop(size=(height, width), scale=scale, ratio=ratio)
+    image_pil = torch_transforms.functional.to_pil_image(image)
+    transformed_image_pt = transform_pt(image_pil)
+
+    transformed_image_pt_np = np.array(transformed_image_pt)
+    assert transformed_image_albu.shape == transformed_image_pt_np.shape
+    assert transformed_image_albu_new.shape == transformed_image_pt_np.shape
+
+    # NOTE: below will fail when height, width is no longer expected as second and third positional arguments
+    transform_albu = A.RandomSizedCrop((128, 224), height, width, p=1.0)
+    transform_albu_new = A.RandomSizedCrop(min_max_height=(128, 224), size=(height, width), p=1.0)
+    transformed_image_albu = transform_albu(image=image)['image']
+    transformed_image_albu_new = transform_albu_new(image=image)['image']
+    assert transformed_image_albu.shape == transformed_image_pt_np.shape
+    assert transformed_image_albu_new.shape == transformed_image_pt_np.shape
+
+    # NOTE: below will fail when height, width is no longer expected as first two positional arguments
+    transform_albu = A.RandomResizedCrop(height, width, scale=scale, ratio=ratio, p=1)
+    transform_albu_height_is_size = A.RandomResizedCrop(size=height, width=width, scale=scale, ratio=ratio, p=1)
+
+    image = np.random.randint(0, 256, (224, 224, 3), dtype=np.uint8)
+    transformed_image_albu = transform_albu(image=image)['image']
+    transform_albu_height_is_size = transform_albu_new(image=image)['image']
+    assert transformed_image_albu.shape == transformed_image_pt_np.shape
+    assert transform_albu_height_is_size.shape == transformed_image_pt_np.shape
+
+@pytest.mark.parametrize("size, width, height, expected_warning", [
+    ((100, 200), None, None, None),
+    (None, 200, 100, DeprecationWarning),
+    (100, None, None, ValueError),
+])
+def test_deprecation_warnings(size, width, height, expected_warning):
+    with warnings.catch_warnings(record=True) as w:
+        warnings.simplefilter("always")
+        if expected_warning == ValueError:
+            with pytest.raises(ValueError):
+                A.RandomResizedCrop(size=size, width=width, height=height)
+        else:
+            A.RandomResizedCrop(size=size, width=width, height=height)
+        if expected_warning is DeprecationWarning:
+            assert len(w) == 1
+            assert issubclass(w[-1].category, expected_warning)
+        else:
+            assert not w
+    warnings.resetwarnings()
```

