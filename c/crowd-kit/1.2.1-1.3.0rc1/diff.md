# Comparing `tmp/crowd-kit-1.2.1.tar.gz` & `tmp/crowd-kit-1.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crowd-kit-1.2.1.tar", last modified: Fri Mar 31 09:19:46 2023, max compression
+gzip compressed data, was "crowd-kit-1.3.0rc1.tar", last modified: Wed Apr  3 09:17:49 2024, max compression
```

## Comparing `crowd-kit-1.2.1.tar` & `crowd-kit-1.3.0rc1.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:19:46.113967 crowd-kit-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-03-31 09:19:46.113967 crowd-kit-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:19:46.077967 crowd-kit-1.2.1/crowd_kit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-03-31 09:19:46.000000 crowd-kit-1.2.1/crowd_kit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-03-31 09:19:46.000000 crowd-kit-1.2.1/crowd_kit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 09:19:46.000000 crowd-kit-1.2.1/crowd_kit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-31 09:19:46.000000 crowd-kit-1.2.1/crowd_kit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-31 09:19:46.000000 crowd-kit-1.2.1/crowd_kit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 09:16:39.000000 crowd-kit-1.2.1/crowd_kit.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:19:46.077967 crowd-kit-1.2.1/crowdkit/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:19:46.077967 crowd-kit-1.2.1/crowdkit/aggregation/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/aggregation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:19:46.081967 crowd-kit-1.2.1/crowdkit/aggregation/base/
--rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/aggregation/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/aggregation/base/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:19:46.089967 crowd-kit-1.2.1/crowdkit/aggregation/classification/
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/aggregation/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17741 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/aggregation/classification/dawid_skene.py
--rw-r--r--   0 runner    (1001) docker     (123)    15642 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/aggregation/classification/glad.py
--rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/aggregation/classification/gold_majority_vote.py
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/aggregation/classification/kos.py
--rw-r--r--   0 runner    (1001) docker     (123)    13918 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/aggregation/classification/m_msr.py
--rw-r--r--   0 runner    (1001) docker     (123)    17803 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/aggregation/classification/mace.py
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/aggregation/classification/majority_vote.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/aggregation/classification/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/aggregation/classification/wawa.py
--rw-r--r--   0 runner    (1001) docker     (123)     6789 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/aggregation/classification/zero_based_skill.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:19:46.089967 crowd-kit-1.2.1/crowdkit/aggregation/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/aggregation/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/aggregation/embeddings/closest_to_average.py
--rw-r--r--   0 runner    (1001) docker     (123)    17315 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/aggregation/embeddings/hrrasa.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/aggregation/embeddings/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8530 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/aggregation/embeddings/rasa.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:19:46.093967 crowd-kit-1.2.1/crowdkit/aggregation/image_segmentation/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/aggregation/image_segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/aggregation/image_segmentation/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/aggregation/image_segmentation/segmentation_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/aggregation/image_segmentation/segmentation_majority_vote.py
--rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/aggregation/image_segmentation/segmentation_rasa.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:19:46.093967 crowd-kit-1.2.1/crowdkit/aggregation/multilabel/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/aggregation/multilabel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/aggregation/multilabel/binary_relevance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:19:46.097967 crowd-kit-1.2.1/crowdkit/aggregation/pairwise/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/aggregation/pairwise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/aggregation/pairwise/bradley_terry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/aggregation/pairwise/noisy_bt.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/aggregation/pairwise/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/aggregation/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:19:46.101967 crowd-kit-1.2.1/crowdkit/aggregation/texts/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/aggregation/texts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/aggregation/texts/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/aggregation/texts/rover.py
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/aggregation/texts/text_hrrasa.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/aggregation/texts/text_rasa.py
--rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/aggregation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:19:46.105967 crowd-kit-1.2.1/crowdkit/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/datasets/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/datasets/_loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/datasets/load_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/datasets/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:19:46.109967 crowd-kit-1.2.1/crowdkit/learning/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/learning/conal.py
--rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/learning/crowd_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/learning/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/learning/text_summarization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/learning/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:19:46.109967 crowd-kit-1.2.1/crowdkit/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:19:46.109967 crowd-kit-1.2.1/crowdkit/metrics/data/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/metrics/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10083 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/metrics/data/_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/metrics/data/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:19:46.113967 crowd-kit-1.2.1/crowdkit/metrics/workers/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/metrics/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/metrics/workers/accuracy_on_aggregates.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/metrics/workers/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:19:46.113967 crowd-kit-1.2.1/crowdkit/postprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/postprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/postprocessing/entropy_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/postprocessing/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/crowdkit/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-03-31 09:19:46.117967 crowd-kit-1.2.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       61 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:19:46.113967 crowd-kit-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-03-31 09:16:26.000000 crowd-kit-1.2.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:17:49.253433 crowd-kit-1.3.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9608 2024-04-03 09:17:49.253433 crowd-kit-1.3.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:17:49.253433 crowd-kit-1.3.0rc1/crowd_kit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9608 2024-04-03 09:17:49.000000 crowd-kit-1.3.0rc1/crowd_kit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-03 09:17:49.000000 crowd-kit-1.3.0rc1/crowd_kit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 09:17:49.000000 crowd-kit-1.3.0rc1/crowd_kit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-03 09:17:49.000000 crowd-kit-1.3.0rc1/crowd_kit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 09:17:49.000000 crowd-kit-1.3.0rc1/crowd_kit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 09:07:49.000000 crowd-kit-1.3.0rc1/crowd_kit.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:17:49.241433 crowd-kit-1.3.0rc1/crowdkit/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:17:49.241433 crowd-kit-1.3.0rc1/crowdkit/aggregation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:17:49.245433 crowd-kit-1.3.0rc1/crowdkit/aggregation/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/base/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:17:49.245433 crowd-kit-1.3.0rc1/crowdkit/aggregation/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15945 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/classification/dawid_skene.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16746 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/classification/glad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7368 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/classification/gold_majority_vote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/classification/kos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13828 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/classification/m_msr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17697 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/classification/mace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6139 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/classification/majority_vote.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/classification/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/classification/wawa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/classification/zero_based_skill.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:17:49.245433 crowd-kit-1.3.0rc1/crowdkit/aggregation/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5843 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/embeddings/closest_to_average.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17967 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/embeddings/hrrasa.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/embeddings/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     8770 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/embeddings/rasa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:17:49.245433 crowd-kit-1.3.0rc1/crowdkit/aggregation/image_segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/image_segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/image_segmentation/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9098 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/image_segmentation/segmentation_em.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/image_segmentation/segmentation_majority_vote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/image_segmentation/segmentation_rasa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:17:49.245433 crowd-kit-1.3.0rc1/crowdkit/aggregation/multilabel/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/multilabel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/multilabel/binary_relevance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:17:49.249433 crowd-kit-1.3.0rc1/crowdkit/aggregation/pairwise/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/pairwise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5118 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/pairwise/bradley_terry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8719 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/pairwise/noisy_bt.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/pairwise/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:17:49.249433 crowd-kit-1.3.0rc1/crowdkit/aggregation/texts/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/texts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/texts/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9549 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/texts/rover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/texts/text_hrrasa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/texts/text_rasa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8681 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:17:49.249433 crowd-kit-1.3.0rc1/crowdkit/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/datasets/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14474 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/datasets/_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/datasets/load_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/datasets/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:17:49.249433 crowd-kit-1.3.0rc1/crowdkit/learning/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/learning/conal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6317 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/learning/crowd_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/learning/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/learning/text_summarization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/learning/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:17:49.249433 crowd-kit-1.3.0rc1/crowdkit/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:17:49.249433 crowd-kit-1.3.0rc1/crowdkit/metrics/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/metrics/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10237 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/metrics/data/_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/metrics/data/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:17:49.249433 crowd-kit-1.3.0rc1/crowdkit/metrics/workers/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/metrics/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/metrics/workers/accuracy_on_aggregates.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/metrics/workers/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:17:49.253433 crowd-kit-1.3.0rc1/crowdkit/postprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/postprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/postprocessing/entropy_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/postprocessing/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 09:17:49.253433 crowd-kit-1.3.0rc1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       62 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:17:49.253433 crowd-kit-1.3.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/tests/test_utils.py
```

### Comparing `crowd-kit-1.2.1/CONTRIBUTING.md` & `crowd-kit-1.3.0rc1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `crowd-kit-1.2.1/LICENSE` & `crowd-kit-1.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `crowd-kit-1.2.1/PKG-INFO` & `crowd-kit-1.3.0rc1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,69 +1,38 @@
-Metadata-Version: 2.1
-Name: crowd-kit
-Version: 1.2.1
-Summary: Computational Quality Control for Crowdsourcing
-Home-page: https://github.com/Toloka/crowd-kit
-Author: Toloka
-License: Apache 2.0
-Project-URL: Bug Tracker, https://github.com/Toloka/crowd-kit/issues
-Project-URL: Documentation, https://toloka.ai/en/docs/crowd-kit/
-Project-URL: API Reference, https://toloka.ai/en/docs/crowd-kit/
-Project-URL: Source Code, https://github.com/Toloka/crowd-kit
-Project-URL: Release Notes, https://github.com/Toloka/crowd-kit/blob/main/CHANGELOG.md
-Keywords: crowdsourcing,quality control,answer aggregation
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Software Development
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: learning
-License-File: LICENSE
-License-File: AUTHORS
-
 # Crowd-Kit: Computational Quality Control for Crowdsourcing
 
 [![Crowd-Kit](https://tlk.s3.yandex.net/crowd-kit/Crowd-Kit-GitHub.png)](https://github.com/Toloka/crowd-kit)
 
+[![PyPI Version][pypi_badge]][pypi_link]
 [![GitHub Tests][github_tests_badge]][github_tests_link]
 [![Codecov][codecov_badge]][codecov_link]
 [![Documentation][docs_badge]][docs_link]
 
-[github_tests_badge]: https://github.com/Toloka/crowdlib/workflows/Tests/badge.svg?branch=main
-[github_tests_link]: https://github.com/Toloka/crowdlib/actions?query=workflow:Tests
+[pypi_badge]: https://badge.fury.io/py/crowd-kit.svg
+[pypi_link]: https://pypi.python.org/pypi/crowd-kit
+[github_tests_badge]: https://github.com/Toloka/crowd-kit/actions/workflows/tests.yml/badge.svg?branch=main
+[github_tests_link]: https://github.com/Toloka/crowd-kit/actions/workflows/tests.yml
 [codecov_badge]: https://codecov.io/gh/Toloka/crowd-kit/branch/main/graph/badge.svg
 [codecov_link]: https://codecov.io/gh/Toloka/crowd-kit
-[docs_badge]: https://img.shields.io/badge/docs-toloka.ai-1E2126
-[docs_link]: https://toloka.ai/en/docs/crowd-kit/
+[docs_badge]: https://readthedocs.org/projects/crowd-kit/badge/
+[docs_link]: https://crowd-kit.readthedocs.io/
 
 **Crowd-Kit** is a powerful Python library that implements commonly-used aggregation methods for crowdsourced annotation and offers the relevant metrics and datasets. We strive to implement functionality that simplifies working with crowdsourced data.
 
 Currently, Crowd-Kit contains:
 
 * implementations of commonly-used aggregation methods for categorical, pairwise, textual, and segmentation responses;
 * metrics of uncertainty, consistency, and agreement with aggregate;
 * loaders for popular crowdsourced datasets.
 
 Also, the `learning` subpackage contains PyTorch implementations of deep learning from crowds methods and advanced aggregation algorithms.
 
 ## Installing
 
-To install Crowd-Kit, run the following command: `pip install crowd-kit`. If you also want to use the `learning` subpackage, type `pip instal crowd-kit[learning]`.
+To install Crowd-Kit, run the following command: `pip install crowd-kit`. If you also want to use the `learning` subpackage, type `pip install crowd-kit[learning]`.
 
 If you are interested in contributing to Crowd-Kit, use [Pipenv](https://pipenv.pypa.io/en/latest/) to install the library with its dependencies: `pipenv install --dev`. We use [pytest](https://docs.pytest.org/en/7.1.x/) for testing.
 
 ## Getting Started
 
 This example shows how to use Crowd-Kit for categorical aggregation using the classical Dawid-Skene algorithm.
 
@@ -161,15 +130,14 @@
   eprinttype = {arxiv},
   eprintclass = {cs.HC},
   url       = {https://arxiv.org/abs/2109.08584},
   language  = {english},
 }
 ```
 
-## Questions and Bug Reports
+## Support and Contributions
 
-* To report a bug, post an issue on the [Toloka/bugreport](https://github.com/Toloka/crowdlib/issues) page.
-* To find answers to common questions or start a new discussion, join our English-speaking [Slack community](https://toloka.ai/community).
+Please use [GitHub Issues](https://github.com/Toloka/crowd-kit/issues) to seek support and submit feature requests. We accept contributions to Crowd-Kit via GitHub as according to our guidelines in [CONTRIBUTING.md](CONTRIBUTING.md).
 
 ## License
 
-&copy; Crowd-Kit team authors, 2020&ndash;2023. Licensed under the Apache License, Version 2.0. See LICENSE file for more details.
+&copy; Crowd-Kit team authors, 2020&ndash;2024. Licensed under the Apache License, Version 2.0. See LICENSE file for more details.
```

### Comparing `crowd-kit-1.2.1/crowd_kit.egg-info/PKG-INFO` & `crowd-kit-1.3.0rc1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,69 +1,102 @@
 Metadata-Version: 2.1
 Name: crowd-kit
-Version: 1.2.1
+Version: 1.3.0rc1
 Summary: Computational Quality Control for Crowdsourcing
-Home-page: https://github.com/Toloka/crowd-kit
 Author: Toloka
 License: Apache 2.0
+Project-URL: Homepage, https://github.com/Toloka/crowd-kit
 Project-URL: Bug Tracker, https://github.com/Toloka/crowd-kit/issues
 Project-URL: Documentation, https://toloka.ai/en/docs/crowd-kit/
 Project-URL: API Reference, https://toloka.ai/en/docs/crowd-kit/
 Project-URL: Source Code, https://github.com/Toloka/crowd-kit
 Project-URL: Release Notes, https://github.com/Toloka/crowd-kit/blob/main/CHANGELOG.md
 Keywords: crowdsourcing,quality control,answer aggregation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: learning
 License-File: LICENSE
 License-File: AUTHORS
+Requires-Dist: attrs
+Requires-Dist: nltk
+Requires-Dist: numpy
+Requires-Dist: pandas>=1.1.0
+Requires-Dist: pyarrow
+Requires-Dist: scikit-learn
+Requires-Dist: tqdm
+Requires-Dist: transformers
+Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: build; extra == "dev"
+Requires-Dist: codecov; extra == "dev"
+Requires-Dist: flake8; extra == "dev"
+Requires-Dist: ipywidgets; extra == "dev"
+Requires-Dist: isort; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: nbqa; extra == "dev"
+Requires-Dist: notebook; extra == "dev"
+Requires-Dist: pandas-stubs; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pyupgrade; extra == "dev"
+Requires-Dist: twine; extra == "dev"
+Requires-Dist: types-tqdm; extra == "dev"
+Provides-Extra: docs
+Requires-Dist: mkdocs-material; extra == "docs"
+Requires-Dist: mkdocstrings-python; extra == "docs"
+Provides-Extra: learning
+Requires-Dist: torch>=1.6.0; extra == "learning"
+Requires-Dist: transformers>=4.0.0; extra == "learning"
 
 # Crowd-Kit: Computational Quality Control for Crowdsourcing
 
 [![Crowd-Kit](https://tlk.s3.yandex.net/crowd-kit/Crowd-Kit-GitHub.png)](https://github.com/Toloka/crowd-kit)
 
+[![PyPI Version][pypi_badge]][pypi_link]
 [![GitHub Tests][github_tests_badge]][github_tests_link]
 [![Codecov][codecov_badge]][codecov_link]
 [![Documentation][docs_badge]][docs_link]
 
-[github_tests_badge]: https://github.com/Toloka/crowdlib/workflows/Tests/badge.svg?branch=main
-[github_tests_link]: https://github.com/Toloka/crowdlib/actions?query=workflow:Tests
+[pypi_badge]: https://badge.fury.io/py/crowd-kit.svg
+[pypi_link]: https://pypi.python.org/pypi/crowd-kit
+[github_tests_badge]: https://github.com/Toloka/crowd-kit/actions/workflows/tests.yml/badge.svg?branch=main
+[github_tests_link]: https://github.com/Toloka/crowd-kit/actions/workflows/tests.yml
 [codecov_badge]: https://codecov.io/gh/Toloka/crowd-kit/branch/main/graph/badge.svg
 [codecov_link]: https://codecov.io/gh/Toloka/crowd-kit
-[docs_badge]: https://img.shields.io/badge/docs-toloka.ai-1E2126
-[docs_link]: https://toloka.ai/en/docs/crowd-kit/
+[docs_badge]: https://readthedocs.org/projects/crowd-kit/badge/
+[docs_link]: https://crowd-kit.readthedocs.io/
 
 **Crowd-Kit** is a powerful Python library that implements commonly-used aggregation methods for crowdsourced annotation and offers the relevant metrics and datasets. We strive to implement functionality that simplifies working with crowdsourced data.
 
 Currently, Crowd-Kit contains:
 
 * implementations of commonly-used aggregation methods for categorical, pairwise, textual, and segmentation responses;
 * metrics of uncertainty, consistency, and agreement with aggregate;
 * loaders for popular crowdsourced datasets.
 
 Also, the `learning` subpackage contains PyTorch implementations of deep learning from crowds methods and advanced aggregation algorithms.
 
 ## Installing
 
-To install Crowd-Kit, run the following command: `pip install crowd-kit`. If you also want to use the `learning` subpackage, type `pip instal crowd-kit[learning]`.
+To install Crowd-Kit, run the following command: `pip install crowd-kit`. If you also want to use the `learning` subpackage, type `pip install crowd-kit[learning]`.
 
 If you are interested in contributing to Crowd-Kit, use [Pipenv](https://pipenv.pypa.io/en/latest/) to install the library with its dependencies: `pipenv install --dev`. We use [pytest](https://docs.pytest.org/en/7.1.x/) for testing.
 
 ## Getting Started
 
 This example shows how to use Crowd-Kit for categorical aggregation using the classical Dawid-Skene algorithm.
 
@@ -161,15 +194,14 @@
   eprinttype = {arxiv},
   eprintclass = {cs.HC},
   url       = {https://arxiv.org/abs/2109.08584},
   language  = {english},
 }
 ```
 
-## Questions and Bug Reports
+## Support and Contributions
 
-* To report a bug, post an issue on the [Toloka/bugreport](https://github.com/Toloka/crowdlib/issues) page.
-* To find answers to common questions or start a new discussion, join our English-speaking [Slack community](https://toloka.ai/community).
+Please use [GitHub Issues](https://github.com/Toloka/crowd-kit/issues) to seek support and submit feature requests. We accept contributions to Crowd-Kit via GitHub as according to our guidelines in [CONTRIBUTING.md](CONTRIBUTING.md).
 
 ## License
 
-&copy; Crowd-Kit team authors, 2020&ndash;2023. Licensed under the Apache License, Version 2.0. See LICENSE file for more details.
+&copy; Crowd-Kit team authors, 2020&ndash;2024. Licensed under the Apache License, Version 2.0. See LICENSE file for more details.
```

### Comparing `crowd-kit-1.2.1/crowd_kit.egg-info/SOURCES.txt` & `crowd-kit-1.3.0rc1/crowd_kit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 AUTHORS
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-setup.cfg
 setup.py
 crowd_kit.egg-info/PKG-INFO
 crowd_kit.egg-info/SOURCES.txt
 crowd_kit.egg-info/dependency_links.txt
 crowd_kit.egg-info/requires.txt
 crowd_kit.egg-info/top_level.txt
 crowd_kit.egg-info/zip-safe
```

### Comparing `crowd-kit-1.2.1/crowdkit/aggregation/base/__init__.py` & `crowd-kit-1.3.0rc1/crowdkit/aggregation/base/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 __all__ = [
-    'BaseClassificationAggregator',
-    'BaseImageSegmentationAggregator',
-    'BaseEmbeddingsAggregator',
-    'BaseTextsAggregator',
-    'BasePairwiseAggregator',
+    "BaseClassificationAggregator",
+    "BaseImageSegmentationAggregator",
+    "BaseEmbeddingsAggregator",
+    "BaseTextsAggregator",
+    "BasePairwiseAggregator",
 ]
 
-from typing import Optional
+from typing import Any, Optional
 
 import attr
 import pandas as pd
 
 from ..utils import named_series_attrib
 
 
 @attr.s
 class BaseClassificationAggregator:
     """This is a base class for all classification aggregators
 
     Attributes:
         labels_ (typing.Optional[pandas.core.series.Series]): Tasks' labels.
             A pandas.Series indexed by `task` such that `labels.loc[task]`
-            is the tasks's most likely true label.
+            is the task's most likely true label.
     """
 
-    labels_: Optional[pd.Series] = named_series_attrib(name='agg_label')
+    labels_: Optional["pd.Series[Any]"] = named_series_attrib(name="agg_label")
 
-    def fit(self, data: pd.DataFrame) -> 'BaseClassificationAggregator':
+    def fit(self, data: pd.DataFrame) -> "BaseClassificationAggregator":
         """Args:
             data (DataFrame): Workers' labeling results.
                 A pandas.DataFrame containing `task`, `worker` and `label` columns.
 
         Returns:
             BaseClassificationAggregator: self.
         """
         raise NotImplementedError()
 
-    def fit_predict(self, data: pd.DataFrame) -> pd.Series:
+    def fit_predict(self, data: pd.DataFrame) -> "pd.Series[Any]":
         """Args:
             data (DataFrame): Workers' labeling results.
                 A pandas.DataFrame containing `task`, `worker` and `label` columns.
         Returns:
             Series: Tasks' labels.
                 A pandas.Series indexed by `task` such that `labels.loc[task]`
                 is the tasks's most likely true label.
@@ -54,27 +54,27 @@
 
     Attributes:
         segmentations_ (Series): Tasks' segmentations.
             A pandas.Series indexed by `task` such that `labels.loc[task]`
             is the tasks's aggregated segmentation.
     """
 
-    segmentations_: pd.Series = named_series_attrib(name='agg_segmentation')
+    segmentations_: "pd.Series[Any]" = named_series_attrib(name="agg_segmentation")
 
-    def fit(self, data: pd.DataFrame) -> 'BaseImageSegmentationAggregator':
+    def fit(self, data: pd.DataFrame) -> "BaseImageSegmentationAggregator":
         """Args:
             data (DataFrame): Workers' segmentations.
                 A pandas.DataFrame containing `worker`, `task` and `segmentation` columns'.
 
         Returns:
             BaseImageSegmentationAggregator: self.
         """
         raise NotImplementedError()
 
-    def fit_predict(self, data: pd.DataFrame) -> pd.Series:
+    def fit_predict(self, data: pd.DataFrame) -> "pd.Series[Any]":
         """Args:
             data (DataFrame): Workers' segmentations.
                 A pandas.DataFrame containing `worker`, `task` and `segmentation` columns'.
 
         Returns:
             Series: Tasks' segmentations.
                 A pandas.Series indexed by `task` such that `labels.loc[task]`
@@ -89,15 +89,15 @@
     Attributes:
         embeddings_and_outputs_ (DataFrame): Tasks' embeddings and outputs.
             A pandas.DataFrame indexed by `task` with `embedding` and `output` columns.
     """
 
     embeddings_and_outputs_: pd.DataFrame = attr.ib(init=False)
 
-    def fit(self, data: pd.DataFrame) -> 'BaseEmbeddingsAggregator':
+    def fit(self, data: pd.DataFrame) -> "BaseEmbeddingsAggregator":
         """Args:
             data (DataFrame): Workers' outputs with their embeddings.
                 A pandas.DataFrame containing `task`, `worker`, `output` and `embedding` columns.
         Returns:
             BaseEmbeddingsAggregator: self.
         """
         raise NotImplementedError()
@@ -118,26 +118,26 @@
     """This is a base class for all texts aggregators
     Attributes:
         texts_ (Series): Tasks' texts.
             A pandas.Series indexed by `task` such that `result.loc[task, text]`
             is the task's text.
     """
 
-    texts_: pd.Series = named_series_attrib(name='agg_text')
+    texts_: "pd.Series[Any]" = named_series_attrib(name="agg_text")
 
-    def fit(self, data: pd.DataFrame) -> 'BaseTextsAggregator':
+    def fit(self, data: pd.DataFrame) -> "BaseTextsAggregator":
         """Args:
             data (DataFrame): Workers' text outputs.
                 A pandas.DataFrame containing `task`, `worker` and `text` columns.
         Returns:
             BaseTextsAggregator: self.
         """
         raise NotImplementedError()
 
-    def fit_predict(self, data: pd.DataFrame) -> pd.Series:
+    def fit_predict(self, data: pd.DataFrame) -> "pd.Series[Any]":
         """Args:
             data (DataFrame): Workers' text outputs.
                 A pandas.DataFrame containing `task`, `worker` and `text` columns.
         Returns:
             Series: Tasks' texts.
                 A pandas.Series indexed by `task` such that `result.loc[task, text]`
                 is the task's text.
@@ -149,31 +149,31 @@
 class BasePairwiseAggregator:
     """This is a base class for all pairwise comparison aggregators
     Attributes:
         scores_ (Series): 'Labels' scores.
             A pandas.Series index by labels and holding corresponding label's scores
     """
 
-    scores_: pd.Series = named_series_attrib(name='agg_score')
+    scores_: "pd.Series[Any]" = named_series_attrib(name="agg_score")
 
-    def fit(self, data: pd.DataFrame) -> 'BasePairwiseAggregator':
+    def fit(self, data: pd.DataFrame) -> "BasePairwiseAggregator":
         """Args:
             data (DataFrame): Workers' pairwise comparison results.
                 A pandas.DataFrame containing `worker`, `left`, `right`, and `label` columns'.
                 For each row `label` must be equal to either `left` column or `right` column.
 
         Returns:
             BasePairwiseAggregator: self.
         """
         raise NotImplementedError()
 
-    def fit_predict(self, data: pd.DataFrame) -> pd.Series:
+    def fit_predict(self, data: pd.DataFrame) -> "pd.Series[Any]":
         """Args:
-                    data (DataFrame): Workers' pairwise comparison results.
-                        A pandas.DataFrame containing `worker`, `left`, `right`, and `label` columns'.
-                        For each row `label` must be equal to either `left` column or `right` column.
-
-                Returns:
-                    Series: 'Labels' scores.
-                        A pandas.Series index by labels and holding corresponding label's scores
-                """
+            data (DataFrame): Workers' pairwise comparison results.
+                A pandas.DataFrame containing `worker`, `left`, `right`, and `label` columns'.
+                For each row `label` must be equal to either `left` column or `right` column.
+
+        Returns:
+            Series: 'Labels' scores.
+                A pandas.Series index by labels and holding corresponding label's scores
+        """
         raise NotImplementedError()
```

### Comparing `crowd-kit-1.2.1/crowdkit/aggregation/classification/dawid_skene.py` & `crowd-kit-1.3.0rc1/crowdkit/aggregation/classification/dawid_skene.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-__all__ = [
-    'DawidSkene',
-    'OneCoinDawidSkene'
-]
+__all__ = ["DawidSkene", "OneCoinDawidSkene"]
 
-from typing import List, Optional
+from typing import Any, List, Optional, cast
 
 import attr
 import numpy as np
 import pandas as pd
 
-from .majority_vote import MajorityVote
 from ..base import BaseClassificationAggregator
 from ..utils import get_most_probable_labels, named_series_attrib
+from .majority_vote import MajorityVote
 
 _EPS = np.float_power(10, -10)
 
 
 @attr.s
 class DawidSkene(BaseClassificationAggregator):
     r"""The **Dawid-Skene** aggregation model is a probabilistic model that parametrizes the expertise level of workers with confusion matrices.
@@ -43,122 +40,132 @@
     2. **M-step**. Estimates the workers' error probability matrix using the specified workers' responses and the true task label probabilities.
 
     A. Philip Dawid and Allan M. Skene. Maximum Likelihood Estimation of Observer Error-Rates Using the EM Algorithm.
     *Journal of the Royal Statistical Society. Series C (Applied Statistics), Vol. 28*, 1 (1979), 20–28.
 
     <https://doi.org/10.2307/2346806>
 
-    Args:
-        n_iter: The maximum number of EM iterations.
-        tol: The tolerance stopping criterion for iterative methods with a variable number of steps.
-            The algorithm converges when the loss change is less than the `tol` parameter.
-
     Examples:
         >>> from crowdkit.aggregation import DawidSkene
         >>> from crowdkit.datasets import load_dataset
         >>> df, gt = load_dataset('relevance-2')
         >>> ds = DawidSkene(100)
         >>> result = ds.fit_predict(df)
-
-    Attributes:
-        labels_ (Optional[pd.Series]): The task labels.
-            The `pandas.Series` data is indexed by `task` so that `labels.loc[task]` is the most likely true label of tasks.
-
-        probas_ (Optional[pandas.core.frame.DataFrame]): The probability distributions of task labels.
-            The `pandas.DataFrame` data is indexed by `task` so that `result.loc[task, label]` is the probability that the `task` true label is equal to `label`.
-            Each probability is in the range from 0 to 1, all task probabilities must sum up to 1.
-
-        priors_ (Optional[pd.Series]): The prior label distribution.
-            The `pandas.Series` data is indexed by `label` and contains the probability of the corresponding label
-            occurrence. Each probability is in the range from 0 to 1,
-            all probabilities must sum up to 1.
-
-        errors_ (Optional[pandas.core.frame.DataFrame]): The workers' error matrices.
-            The `pandas.DataFrame` data is indexed by `worker` and `label` with a column for every
-            `label_id` found in `data` so that `result.loc[worker, observed_label, true_label]` is the probability
-            that `worker` produces `observed_label`, given that the task true label is `true_label`.
-
-        loss_history_ (List[float]): A list of loss values during training.
     """
 
     n_iter: int = attr.ib(default=100)
+    """The maximum number of EM iterations."""
+
     tol: float = attr.ib(default=1e-5)
+    """The tolerance stopping criterion for iterative methods with a variable number of steps.
+    The algorithm converges when the loss change is less than the `tol` parameter."""
 
     probas_: Optional[pd.DataFrame] = attr.ib(init=False)
-    priors_: Optional[pd.Series] = named_series_attrib(name='prior')
-    # labels_
+    """The probability distributions of task labels.
+    The `pandas.Series` data is indexed by `task` so that `labels.loc[task]` is the most likely true label of tasks."""
+
+    priors_: Optional["pd.Series[Any]"] = named_series_attrib(name="prior")
+    """The prior label distribution.
+    The `pandas.DataFrame` data is indexed by `task` so that `result.loc[task, label]` is the probability that
+    the `task` true label is equal to `label`. Each probability is in the range from 0 to 1, all task probabilities
+    must sum up to 1."""
+
     errors_: Optional[pd.DataFrame] = attr.ib(init=False)
+    """The workers' error matrices. The `pandas.DataFrame` data is indexed by `worker` and `label` with a column
+    for every `label_id` found in `data` so that `result.loc[worker, observed_label, true_label]` is the probability
+    that `worker` produces `observed_label`, given that the task true label is `true_label`."""
+
     loss_history_: List[float] = attr.ib(init=False)
+    """ A list of loss values during training."""
 
     @staticmethod
     def _m_step(data: pd.DataFrame, probas: pd.DataFrame) -> pd.DataFrame:
         """Performs M-step of the Dawid-Skene algorithm.
 
         Estimates the workers' error probability matrix using the specified workers' responses and the true task label probabilities.
         """
-        joined = data.join(probas, on='task')
-        joined.drop(columns=['task'], inplace=True)
+        joined = data.join(probas, on="task")
+        joined.drop(columns=["task"], inplace=True)
 
-        errors = joined.groupby(['worker', 'label'], sort=False).sum()
+        errors = joined.groupby(["worker", "label"], sort=False).sum()
         errors.clip(lower=_EPS, inplace=True)
-        errors /= errors.groupby('worker', sort=False).sum()
+        errors /= errors.groupby("worker", sort=False).sum()
 
         return errors
 
     @staticmethod
-    def _e_step(data: pd.DataFrame, priors: pd.Series, errors: pd.DataFrame) -> pd.DataFrame:
+    def _e_step(
+        data: pd.DataFrame, priors: "pd.Series[Any]", errors: pd.DataFrame
+    ) -> pd.DataFrame:
         """
         Performs E-step of the Dawid-Skene algorithm.
 
         Estimates the true task label probabilities using the specified workers' responses,
         the prior label probabilities, and the workers' error probability matrix.
         """
 
         # We have to multiply lots of probabilities and such products are known to converge
         # to zero exponentially fast. To avoid floating-point precision problems we work with
         # logs of original values
-        joined = data.join(np.log2(errors), on=['worker', 'label'])
-        joined.drop(columns=['worker', 'label'], inplace=True)
-        log_likelihoods = np.log2(priors) + joined.groupby('task', sort=False).sum()
-        log_likelihoods.rename_axis('label', axis=1, inplace=True)
+        joined = data.join(np.log2(errors), on=["worker", "label"])  # type: ignore
+        joined.drop(columns=["worker", "label"], inplace=True)
+        log_likelihoods = np.log2(priors) + joined.groupby("task", sort=False).sum()
+        log_likelihoods.rename_axis("label", axis=1, inplace=True)
 
         # Exponentiating log_likelihoods 'as is' may still get us beyond our precision.
         # So we shift every row of log_likelihoods by a constant (which is equivalent to
         # multiplying likelihoods rows by a constant) so that max log_likelihood in each
         # row is equal to 0. This trick ensures proper scaling after exponentiating and
         # does not affect the result of E-step
-        scaled_likelihoods = np.exp2(log_likelihoods.sub(log_likelihoods.max(axis=1), axis=0))
-        return scaled_likelihoods.div(scaled_likelihoods.sum(axis=1), axis=0)
-
-    def _evidence_lower_bound(self, data: pd.DataFrame, probas: pd.DataFrame, priors: pd.Series, errors: pd.DataFrame) -> float:
+        scaled_likelihoods = np.exp2(
+            log_likelihoods.sub(log_likelihoods.max(axis=1), axis=0)
+        )
+        scaled_likelihoods = scaled_likelihoods.div(
+            scaled_likelihoods.sum(axis=1), axis=0
+        )
+        # Convert columns types to label type
+        scaled_likelihoods.columns = pd.Index(
+            scaled_likelihoods.columns, name="label", dtype=data.label.dtype
+        )
+        return cast(pd.DataFrame, scaled_likelihoods)
+
+    def _evidence_lower_bound(
+        self,
+        data: pd.DataFrame,
+        probas: pd.DataFrame,
+        priors: "pd.Series[Any]",
+        errors: pd.DataFrame,
+    ) -> float:
         # calculate joint probability log-likelihood expectation over probas
-        joined = data.join(np.log(errors), on=['worker', 'label'])
+        joined = data.join(np.log(errors), on=["worker", "label"])  # type: ignore
 
         # escape boolean index/column names to prevent confusion between indexing by boolean array and iterable of names
-        joined = joined.rename(columns={True: 'True', False: 'False'}, copy=False)
-        priors = priors.rename(index={True: 'True', False: 'False'}, copy=False)
+        joined = joined.rename(columns={True: "True", False: "False"}, copy=False)
+        priors = priors.rename(index={True: "True", False: "False"}, copy=False)
 
-        joined.loc[:, priors.index] = joined.loc[:, priors.index].add(np.log(priors))
+        joined.loc[:, priors.index] = joined.loc[:, priors.index].add(np.log(priors))  # type: ignore
 
-        joined.set_index(['task', 'worker'], inplace=True)
-        joint_expectation = (probas.rename(columns={True: 'True', False: 'False'}) * joined).sum().sum()
+        joined.set_index(["task", "worker"], inplace=True)
+        joint_expectation = (
+            (probas.rename(columns={True: "True", False: "False"}) * joined).sum().sum()
+        )
 
         entropy = -(np.log(probas) * probas).sum().sum()
         return float(joint_expectation + entropy)
 
-    def fit(self, data: pd.DataFrame) -> 'DawidSkene':
+    def fit(self, data: pd.DataFrame) -> "DawidSkene":
         """Fits the model to the training data with the EM algorithm.
         Args:
             data (DataFrame): The training dataset of workers' labeling results
                 which is represented as the `pandas.DataFrame` data containing `task`, `worker`, and `label` columns.
         Returns:
             DawidSkene: self.
         """
 
-        data = data[['task', 'worker', 'label']]
+        data = data[["task", "worker", "label"]]
 
         # Early exit
         if not data.size:
             self.probas_ = pd.DataFrame()
             self.priors_ = pd.Series(dtype=float)
             self.errors_ = pd.DataFrame()
             self.labels_ = pd.Series(dtype=float)
@@ -172,22 +179,26 @@
         self.loss_history_ = []
 
         # Updating proba and errors n_iter times
         for _ in range(self.n_iter):
             probas = self._e_step(data, priors, errors)
             priors = probas.mean()
             errors = self._m_step(data, probas)
-            new_loss = self._evidence_lower_bound(data, probas, priors, errors) / len(data)
+            new_loss = self._evidence_lower_bound(data, probas, priors, errors) / len(
+                data
+            )
             self.loss_history_.append(new_loss)
 
             if new_loss - loss < self.tol:
                 break
             loss = new_loss
 
-        probas.columns = pd.Index(probas.columns, name='label', dtype=probas.columns.dtype)
+        probas.columns = pd.Index(
+            probas.columns, name="label", dtype=probas.columns.dtype
+        )
         # Saving results
         self.probas_ = probas
         self.priors_ = priors
         self.errors_ = errors
         self.labels_ = get_most_probable_labels(probas)
 
         return self
@@ -196,48 +207,54 @@
         """Fits the model to the training data and returns probability distributions of labels for each task.
         Args:
             data (DataFrame): The training dataset of workers' labeling results
                 which is represented as the `pandas.DataFrame` data containing `task`, `worker`, and `label` columns.
         Returns:
             DataFrame: Probability distributions of task labels.
                 The `pandas.DataFrame` data is indexed by `task` so that `result.loc[task, label]` is the probability that the `task` true label is equal to `label`.
-                Each probability is in he range from 0 to 1, all task probabilities must sum up to 1.
+                Each probability is in the range from 0 to 1, all task probabilities must sum up to 1.
         """
 
-        return self.fit(data).probas_
+        self.fit(data)
+        assert self.probas_ is not None, "no probas_"
+        return self.probas_
 
-    def fit_predict(self, data: pd.DataFrame) -> pd.Series:
+    def fit_predict(self, data: pd.DataFrame) -> "pd.Series[Any]":
         """Fits the model to the training data and returns the aggregated results.
         Args:
             data (DataFrame): The training dataset of workers' labeling results
                 which is represented as the `pandas.DataFrame` data containing `task`, `worker`, and `label` columns.
         Returns:
             Series: Task labels. The `pandas.Series` data is indexed by `task` so that `labels.loc[task]` is the most likely true label of tasks.
         """
 
-        return self.fit(data).labels_
+        self.fit(data)
+        assert self.labels_ is not None, "no labels_"
+        return self.labels_
 
 
 @attr.s
 class OneCoinDawidSkene(DawidSkene):
-    r"""The **one-coin Dawid-Skene** aggregation model works exactly the same as the original Dawid-Skene model based on the EM algorithm, except for calculating the workers' errors
+    r"""The **one-coin Dawid-Skene** aggregation model works exactly the same as the original Dawid-Skene model
+    based on the EM algorithm, except for calculating the workers' errors
     at the M-step of the algorithm.
 
     For the one-coin model, a worker confusion (error) matrix is parameterized by a single parameter $s_w$:
     $$
     e^w_{j,z_j}  = \begin{cases}
         s_{w} & y^w_j = z_j \\
         \frac{1 - s_{w}}{K - 1} & y^w_j \neq z_j
     \end{cases}
     $$
     where $e^w$ is a worker confusion (error) matrix of size $K \times K$ in case of the $K$ class classification,
     $z_j$ be a true task label, $y^w_j$ is a worker
     response to the task $j$, and $s_w$ is a worker skill (accuracy).
 
-    In other words, the worker $w$ uses a single coin flip to decide their assignment. No matter what the true label is, the worker has the $s_w$ probability to assign the correct label, and
+    In other words, the worker $w$ uses a single coin flip to decide their assignment. No matter what the true label is,
+    the worker has the $s_w$ probability to assign the correct label, and
     has the $1 − s_w$ probability to randomly assign an incorrect label. For the one-coin model, it
     suffices to estimate $s_w$ for every worker $w$ and estimate $y^w_j$ for every task $j$. Because of its
     simplicity, the one-coin model is easier to estimate and enjoys better convergence properties.
 
     Parameters $p$, $e^w$, and latent variables $z$ are optimized with the Expectation-Maximization algorithm:
     1. **E-step**. Estimates the true task label probabilities using the specified workers' responses,
     the prior label probabilities, and the workers' error probability matrix.
@@ -245,102 +262,73 @@
     Then estimates the workers' error probability matrix by assigning user skills to error matrix row by row.
 
     Y. Zhang, X. Chen, D. Zhou, and M. I. Jordan. Spectral methods meet EM: A provably optimal algorithm for crowdsourcing.
     *Journal of Machine Learning Research. Vol. 17*, (2016), 1-44.
 
     <https://doi.org/10.48550/arXiv.1406.3824>
 
-    Args:
-        n_iter: The maximum number of EM iterations.
-        tol: The tolerance stopping criterion for iterative methods with a variable number of steps.
-            The algorithm converges when the loss change is less than the `tol` parameter.
-
     Examples:
         >>> from crowdkit.aggregation import OneCoinDawidSkene
         >>> from crowdkit.datasets import load_dataset
         >>> df, gt = load_dataset('relevance-2')
         >>> hds = OneCoinDawidSkene(100)
         >>> result = hds.fit_predict(df)
-
-    Attributes:
-        labels_ (Optional[pd.Series]): The task labels.
-            The `pandas.Series` data is indexed by `task` so that `labels.loc[task]` is the most likely true label of tasks.
-
-        probas_ (Optional[pandas.core.frame.DataFrame]): The probability distributions of task labels.
-            The `pandas.DataFrame` data is indexed by `task` so that `result.loc[task, label]` is the probability that the `task` true label is equal to `label`.
-            Each probability is in the range from 0 to 1, all task probabilities must sum up to 1.
-
-        priors_ (Optional[pd.Series]): The prior label distribution.
-            The `pandas.Series` data is indexed by `label` and contains the probability of the corresponding label
-            occurrence. Each probability is in the range from 0 to 1, all probabilities must sum up to 1.
-
-        errors_ (Optional[pandas.core.frame.DataFrame]): The workers' error matrices.
-            The `pandas.DataFrame` data is indexed by `worker` and `label` with a column for every
-            `label_id` found in `data` so that `result.loc[worker, observed_label, true_label]` is the probability
-            that `worker` produces `observed_label`, given that the task true label is `true_label`.
-
-        skills_ (Optional[pd.Series]): The workers' skills. The `pandas.Series` data is indexed by `worker` and has the corresponding worker skill.
-
-        loss_history_ (List[float]): A list of loss values during training.
     """
 
-    n_iter: int = attr.ib(default=100)
-    tol: float = attr.ib(default=1e-5)
-
-    probas_: Optional[pd.DataFrame] = attr.ib(init=False)
-    priors_: Optional[pd.Series] = named_series_attrib(name='prior')
-    errors_: Optional[pd.DataFrame] = attr.ib(init=False)
-    skills_: Optional[pd.Series] = attr.ib(init=False)
-    loss_history_: List[float] = attr.ib(init=False)
-
     @staticmethod
-    def _assign_skills(row: pd.Series, skills: pd.DataFrame) -> pd.DataFrame:
+    def _assign_skills(row: "pd.Series[Any]", skills: pd.DataFrame) -> pd.DataFrame:
         """
         Assigns user skills to error matrix row by row.
         """
         num_categories = len(row)
         for column_name, _ in row.items():
-            if column_name == row.name[1]:
-                row[column_name] = skills[row.name[0]]
+            if column_name == row.name[1]:  # type: ignore
+                row[column_name] = skills[row.name[0]]  # type: ignore
             else:
-                row[column_name] = (1 - skills[row.name[0]]) / (num_categories - 1)
-        return row
+                row[column_name] = (1 - skills[row.name[0]]) / (num_categories - 1)  # type: ignore
+        return row  # type: ignore
 
     @staticmethod
-    def _process_skills_to_errors(data: pd.DataFrame, probas: pd.DataFrame, skills: pd.Series) -> pd.DataFrame:
+    def _process_skills_to_errors(
+        data: pd.DataFrame, probas: pd.DataFrame, skills: "pd.Series[Any]"
+    ) -> pd.DataFrame:
         errors = DawidSkene._m_step(data, probas)
 
-        errors = errors.apply(OneCoinDawidSkene._assign_skills, args=(skills,), axis=1)
+        errors = errors.apply(OneCoinDawidSkene._assign_skills, args=(skills,), axis=1)  # type: ignore
         errors.clip(lower=_EPS, upper=1 - _EPS, inplace=True)
 
         return errors
 
     @staticmethod
-    def _m_step(data: pd.DataFrame, probas: pd.DataFrame) -> pd.Series:
+    def _m_step(data: pd.DataFrame, probas: pd.DataFrame) -> "pd.Series[Any]":  # type: ignore
         """Performs M-step of Homogeneous Dawid-Skene algorithm.
 
         Calculates a worker skill as their accuracy according to the label probability.
         """
         skilled_data = data.copy()
-        idx_cols, cols = pd.factorize(data['label'])
-        idx_rows, rows = pd.factorize(data['task'])
-        skilled_data['skill'] = probas.reindex(rows, axis=0).reindex(cols, axis=1).to_numpy()[idx_rows, idx_cols]
-        skills = skilled_data.groupby(['worker'], sort=False)['skill'].mean()
+        idx_cols, cols = pd.factorize(data["label"])
+        idx_rows, rows = pd.factorize(data["task"])
+        skilled_data["skill"] = (
+            probas.reindex(rows, axis=0)
+            .reindex(cols, axis=1)
+            .to_numpy()[idx_rows, idx_cols]
+        )
+        skills = skilled_data.groupby(["worker"], sort=False)["skill"].mean()
         return skills
 
-    def fit(self, data: pd.DataFrame) -> 'OneCoinDawidSkene':
+    def fit(self, data: pd.DataFrame) -> "OneCoinDawidSkene":
         """Fits the model to the training data with the EM algorithm.
         Args:
             data (DataFrame): The training dataset of workers' labeling results
                 which is represented as the `pandas.DataFrame` data containing `task`, `worker`, and `label` columns.
         Returns:
             DawidSkene: self.
         """
 
-        data = data[['task', 'worker', 'label']]
+        data = data[["task", "worker", "label"]]
 
         # Early exit
         if not data.size:
             self.probas_ = pd.DataFrame()
             self.priors_ = pd.Series(dtype=float)
             self.errors_ = pd.DataFrame()
             self.labels_ = pd.Series(dtype=float)
@@ -356,15 +344,17 @@
 
         # Updating proba and errors n_iter times
         for _ in range(self.n_iter):
             probas = self._e_step(data, priors, errors)
             priors = probas.mean()
             skills = self._m_step(data, probas)
             errors = self._process_skills_to_errors(data, probas, skills)
-            new_loss = self._evidence_lower_bound(data, probas, priors, errors) / len(data)
+            new_loss = self._evidence_lower_bound(data, probas, priors, errors) / len(
+                data
+            )
             self.loss_history_.append(new_loss)
 
             if new_loss - loss < self.tol:
                 break
             loss = new_loss
 
         # Saving results
```

### Comparing `crowd-kit-1.2.1/crowdkit/aggregation/classification/glad.py` & `crowd-kit-1.3.0rc1/crowdkit/aggregation/classification/glad.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-__all__ = ['GLAD']
+__all__ = ["GLAD"]
 
-from typing import Optional, Tuple, List, cast, Any
+from typing import Any, Iterator, List, Optional, Tuple, cast
 
 import attr
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
 import scipy
 import scipy.stats
 from scipy.optimize import minimize
-from tqdm.auto import tqdm
+from tqdm.auto import tqdm, trange
 
 # logsumexp was moved to scipy.special in 0.19.0rc1 version of scipy
 try:
     from scipy.special import logsumexp
 except ImportError:
     from scipy.misc.common import logsumexp
 
@@ -29,15 +29,14 @@
     $\alpha_i \in (-\infty, +\infty)$ be a worker ability parameter, $\beta_j \in (0, +\infty)$ be
     an inverse task difficulty, $z_j$ be a latent variable representing the true task label, and $y^i_j$
     be a worker response that we observe. The relationships between these variables and parameters according
     to GLAD are represented by the following latent label model:
 
     ![GLAD latent label model](https://tlk.s3.yandex.net/crowd-kit/docs/glad_llm.png)
 
-
     The prior probability of $z_j$ being equal to $c$ is
     $$
     \operatorname{Pr}(z_j = c) = p[c],
     $$
     and the probability distribution of the worker responses with the true label $c$ follows the
     single coin Dawid-Skene model where the true label probability is a sigmoid function of the product of the
     worker ability and the inverse task difficulty:
@@ -50,261 +49,309 @@
     $$
 
     Parameters $p$, $\alpha$, $\beta$, and latent variables $z$ are optimized with the Expectation-Minimization algorithm:
     1. **E-step**. Estimates the true task label probabilities using the alpha parameters of workers' abilities,
         the prior label probabilities, and the beta parameters of task difficulty.
     2. **M-step**. Optimizes the alpha and beta parameters using the conjugate gradient method.
 
-
     J. Whitehill, P. Ruvolo, T. Wu, J. Bergsma, and J. Movellan.
     Whose Vote Should Count More: Optimal Integration of Labels from Labelers of Unknown Expertise.
     *Proceedings of the 22nd International Conference on Neural Information Processing Systems*, 2009
 
     <https://proceedings.neurips.cc/paper/2009/file/f899139df5e1059396431415e770c6dd-Paper.pdf>
 
-
-    Args:
-        n_iter: The maximum number of EM iterations.
-        tol: The tolerance stopping criterion for iterative methods with a variable number of steps.
-            The algorithm converges when the loss change is less than the `tol` parameter.
-        silent: Specifies if the progress bar will be shown (false) or not (true).
-        labels_priors: The prior label probabilities.
-        alphas_priors_mean: The prior mean value of the alpha parameters.
-        betas_priors_mean: The prior mean value of the beta parameters.
-        m_step_max_iter: The maximum number of iterations of the conjugate gradient method in the M-step.
-        m_step_tol: The tolerance stopping criterion of the conjugate gradient method in the M-step.
-
     Examples:
         >>> from crowdkit.aggregation import GLAD
         >>> from crowdkit.datasets import load_dataset
         >>> df, gt = load_dataset('relevance-2')
         >>> glad = GLAD()
         >>> result = glad.fit_predict(df)
+    """
+
+    n_iter: int = attr.ib(default=100)
+    """The maximum number of EM iterations."""
 
-    Attributes:
-        labels_ (typing.Optional[pandas.core.series.Series]): The task labels. The `pandas.Series` data is indexed by `task`
-            so that `labels.loc[task]` is the most likely true label of tasks.
+    tol: float = attr.ib(default=1e-5)
+    """The tolerance stopping criterion for iterative methods with a variable number of steps.
+    The algorithm converges when the loss change is less than the `tol` parameter."""
 
-        probas_ (typing.Optional[pandas.core.frame.DataFrame]): The probability distributions of task labels.
-            The `pandas.DataFrame` data is indexed by `task` so that `result.loc[task, label]` is the probability that the `task` true label is equal to `label`.
-            Each probability is in the range from 0 to 1, all task probabilities must sum up to 1.
+    silent: bool = attr.ib(default=True)
+    """Specifies if the progress bar will be shown (false) or not (true)."""
 
-        alphas_ (Series): The alpha parameters of workers' abilities. The `pandas.Series` data is indexed by `worker`
-            that contains the estimated alpha parameters.
+    labels_priors: Optional["pd.Series[Any]"] = attr.ib(default=None)
+    """The prior label probabilities."""
 
-        betas_ (Series): The beta parameters of task difficulty. The `pandas.Series` data is indexed by `task`
-            that contains the estimated beta parameters.
+    alphas_priors_mean: Optional["pd.Series[Any]"] = attr.ib(default=None)
+    """The prior mean value of the alpha parameters."""
 
-        loss_history_ (List[float]): A list of loss values during training.
-    """
+    betas_priors_mean: Optional["pd.Series[Any]"] = attr.ib(default=None)
+    """The prior mean value of the beta parameters."""
 
-    n_iter: int = attr.ib(default=100)
-    tol: float = attr.ib(default=1e-5)
-    silent: bool = attr.ib(default=True)
-    labels_priors: Optional[pd.Series] = attr.ib(default=None)
-    alphas_priors_mean: Optional[pd.Series] = attr.ib(default=None)
-    betas_priors_mean: Optional[pd.Series] = attr.ib(default=None)
     m_step_max_iter: int = attr.ib(default=25)
+    """The maximum number of iterations of the conjugate gradient method in the M-step."""
+
     m_step_tol: float = attr.ib(default=1e-2)
+    """The tolerance stopping criterion of the conjugate gradient method in the M-step."""
 
-    # Available after fit
-    # labels_
     probas_: Optional[pd.DataFrame] = attr.ib(init=False)
-    alphas_: pd.Series = named_series_attrib(name='alpha')
-    betas_: pd.Series = named_series_attrib(name='beta')
+    """The probability distributions of task labels.
+    The data frame is indexed by `task` so that `result.loc[task, label]` is the probability that the `task`
+    true label is equal to `label`. Each probability is in the range from 0 to 1, all task probabilities
+    must sum up to 1."""
+
+    alphas_: "pd.Series[Any]" = named_series_attrib(name="alpha")
+    """The alpha parameters of workers' abilities.
+    The `pandas.Series` data is indexed by `worker` that contains the estimated alpha parameters."""
+
+    betas_: "pd.Series[Any]" = named_series_attrib(name="beta")
+    """The beta parameters of task difficulty.
+    The `pandas.Series` data is indexed by `task` that contains the estimated beta parameters."""
+
     loss_history_: List[float] = attr.ib(init=False)
+    """A list of loss values during training."""
 
     def _join_all(
-            self,
-            data: pd.DataFrame,
-            alphas: pd.Series,
-            betas: pd.Series,
-            priors: pd.Series
+        self,
+        data: pd.DataFrame,
+        alphas: "pd.Series[Any]",
+        betas: "pd.Series[Any]",
+        priors: "pd.Series[Any]",
     ) -> pd.DataFrame:
-        """Makes a data frame with format `(task, worker, label, variable) -> (alpha, beta, posterior, delta)`
-        """
+        """Makes a data frame with format `(task, worker, label, variable) -> (alpha, beta, posterior, delta)`"""
         labels = list(priors.index)
-        data = data.set_index('task')
+        data = data.set_index("task")
         data[labels] = 0
         data.reset_index(inplace=True)
-        data = data.melt(id_vars=['task', 'worker', 'label'], value_vars=labels, value_name='posterior')
-        data = data.set_index('variable')
+        data = data.melt(
+            id_vars=["task", "worker", "label"],
+            value_vars=labels,
+            value_name="posterior",
+        )
+        data = data.set_index("variable")
         data.reset_index(inplace=True)
-        data.set_index('task', inplace=True)
-        data['beta'] = betas
-        data = data.reset_index().set_index('worker')
-        data['alpha'] = alphas
+        data.set_index("task", inplace=True)
+        data["beta"] = betas
+        data = data.reset_index().set_index("worker")
+        data["alpha"] = alphas
         data.reset_index(inplace=True)
-        data['delta'] = data['label'] == data['variable']
+        data["delta"] = data["label"] == data["variable"]
         return data
 
     def _e_step(self, data: pd.DataFrame) -> pd.DataFrame:
         """
         Performs E-step of GLAD algorithm.
 
         Estimates the true task label probabilities using the alpha parameters of workers' abilities,
         the prior label probabilities, and the beta parameters of task difficulty.
         """
-        alpha_beta = data['alpha'] * np.exp(data['beta'])
+        alpha_beta = data["alpha"] * np.exp(data["beta"])
         log_sigma = -self._softplus(-alpha_beta)
         log_one_minus_sigma = -self._softplus(alpha_beta)
-        data['posterior'] = data['delta'] * log_sigma + \
-                            (1 - data['delta']) * (log_one_minus_sigma - np.log(len(self.prior_labels_) - 1))
+        data["posterior"] = data["delta"] * log_sigma + (1 - data["delta"]) * (
+            log_one_minus_sigma - np.log(len(self.prior_labels_) - 1)
+        )
         # sum up by workers
-        probas = data.groupby(['task', 'variable']).sum(numeric_only=True)['posterior']
+        probas = data.groupby(["task", "variable"]).sum(numeric_only=True)["posterior"]
         # add priors to every label
-        probas = probas.add(np.log(cast(pd.Series, self.priors_)), level=1)
+        probas = probas.add(np.log(cast("pd.Series[Any]", self.priors_)), level=1)
         # exponentiate and normalize
-        probas = probas.groupby(['task']).transform(self._softmax)
+        probas = probas.groupby(["task"]).transform(self._softmax)
         # put posterior in data['posterior']
-        probas.name = 'posterior'
-        data = pd.merge(data.drop('posterior', axis=1), probas, on=['task', 'variable'], copy=False)
+        probas.name = "posterior"
+        data = pd.merge(
+            data.drop("posterior", axis=1), probas, on=["task", "variable"], copy=False
+        )
 
         self.probas_ = probas.unstack()
         return data
 
-    def _gradient_Q(self, data: pd.DataFrame) -> Tuple[npt.NDArray[Any], npt.NDArray[Any]]:
-        """Computes gradient of loss function
-        """
+    def _gradient_Q(
+        self, data: pd.DataFrame
+    ) -> Tuple["pd.Series[Any]", "pd.Series[Any]"]:
+        """Computes gradient of loss function"""
 
-        sigma = scipy.special.expit(data['alpha'] * np.exp(data['beta']))
+        sigma = scipy.special.expit(data["alpha"] * np.exp(data["beta"]))
         # multiply by exponent of beta because of beta -> exp(beta) reparameterization
-        data['dQb'] = data['posterior'] * (data['delta'] - sigma) * data['alpha'] * np.exp(data['beta'])
-        dQbeta = data.groupby('task').sum(numeric_only=True)['dQb']
+        data["dQb"] = (
+            data["posterior"]
+            * (data["delta"] - sigma)
+            * data["alpha"]
+            * np.exp(data["beta"])
+        )
+        dQbeta = data.groupby("task").sum(numeric_only=True)["dQb"]
+
         # gradient of priors on betas
-        dQbeta -= (self.betas_ - self.betas_priors_mean_)
+        assert self.betas_ is not None, "betas_ is None"
+        assert self.betas_priors_mean_ is not None, "betas_priors_mean_ is None"
+        dQbeta -= self.betas_ - self.betas_priors_mean_
 
-        data['dQa'] = data['posterior'] * (data['delta'] - sigma) * np.exp(data['beta'])
-        dQalpha = data.groupby('worker').sum(numeric_only=True)['dQa']
+        data["dQa"] = data["posterior"] * (data["delta"] - sigma) * np.exp(data["beta"])
+        dQalpha = data.groupby("worker").sum(numeric_only=True)["dQa"]
         # gradient of priors on alphas
-        dQalpha -= (self.alphas_ - self.alphas_priors_mean_)
+        assert self.alphas_ is not None, "alphas_ is None"
+        assert self.alphas_priors_mean_ is not None, "alphas_priors_mean_ is None"
+        dQalpha -= self.alphas_ - self.alphas_priors_mean_
         return dQalpha, dQbeta
 
     def _compute_Q(self, data: pd.DataFrame) -> float:
-        """Computes loss function
-        """
+        """Computes loss function"""
 
-        alpha_beta = data['alpha'] * np.exp(data['beta'])
+        alpha_beta = data["alpha"] * np.exp(data["beta"])
         log_sigma = -self._softplus(-alpha_beta)
         log_one_minus_sigma = -self._softplus(alpha_beta)
-        data['task_expectation'] = data['posterior'] * \
-                                   (data['delta'] * log_sigma +
-                                    (1 - data['delta']) * (log_one_minus_sigma - np.log(len(self.prior_labels_) - 1)))
-        Q = data['task_expectation'].sum()
+        data["task_expectation"] = data["posterior"] * (
+            data["delta"] * log_sigma
+            + (1 - data["delta"])
+            * (log_one_minus_sigma - np.log(len(self.prior_labels_) - 1))
+        )
+        Q = data["task_expectation"].sum()
 
         # priors on alphas and betas
+        assert self.alphas_ is not None, "alphas_ is None"
+        assert self.alphas_priors_mean_ is not None, "alphas_priors_mean_ is None"
+        assert self.betas_ is not None, "betas_ is None"
+        assert self.betas_priors_mean_ is not None, "betas_priors_mean_ is None"
         Q += np.log(scipy.stats.norm.pdf(self.alphas_ - self.alphas_priors_mean_)).sum()
         Q += np.log(scipy.stats.norm.pdf(self.betas_ - self.betas_priors_mean_)).sum()
         if np.isnan(Q):
             return -np.inf
         return float(Q)
 
     def _optimize_f(self, x: npt.NDArray[Any]) -> float:
-        """Computes loss by parameters represented by numpy array
-        """
+        """Computes loss by parameters represented by numpy array"""
         alpha, beta = self._get_alphas_betas_by_point(x)
         self._update_alphas_betas(alpha, beta)
         return -self._compute_Q(self._current_data)
 
     def _optimize_df(self, x: npt.NDArray[Any]) -> npt.NDArray[Any]:
-        """Computes loss gradient by parameters represented by numpy array
-        """
+        """Computes loss gradient by parameters represented by numpy array"""
         alpha, beta = self._get_alphas_betas_by_point(x)
         self._update_alphas_betas(alpha, beta)
         dQalpha, dQbeta = self._gradient_Q(self._current_data)
 
         minus_grad = np.zeros_like(x)
-        minus_grad[:len(self.workers_)] = -dQalpha[self.workers_].values
-        minus_grad[len(self.workers_):] = -dQbeta[self.tasks_].values
+        minus_grad[: len(self.workers_)] = -dQalpha[self.workers_].values  # type: ignore
+        minus_grad[len(self.workers_) :] = -dQbeta[self.tasks_].values  # type: ignore
         return minus_grad
 
-    def _update_alphas_betas(self, alphas: pd.Series, betas: pd.Series) -> None:
+    def _update_alphas_betas(
+        self, alphas: "pd.Series[Any]", betas: "pd.Series[Any]"
+    ) -> None:
         self.alphas_ = alphas
         self.betas_ = betas
-        self._current_data.set_index('worker', inplace=True)
-        self._current_data['alpha'] = alphas
+        self._current_data.set_index("worker", inplace=True)
+        self._current_data["alpha"] = alphas
         self._current_data.reset_index(inplace=True)
-        self._current_data.set_index('task', inplace=True)
-        self._current_data['beta'] = betas
+        self._current_data.set_index("task", inplace=True)
+        self._current_data["beta"] = betas
         self._current_data.reset_index(inplace=True)
 
-    def _get_alphas_betas_by_point(self, x: npt.NDArray[Any]) -> Tuple[pd.Series, pd.Series]:
-        alphas = pd.Series(x[:len(self.workers_)], index=self.workers_, name='alpha')
-        alphas.index.name = 'worker'
-        betas = pd.Series(x[len(self.workers_):], index=self.tasks_, name='beta')
-        betas.index.name = 'task'
+    def _get_alphas_betas_by_point(
+        self, x: npt.NDArray[Any]
+    ) -> Tuple["pd.Series[Any]", "pd.Series[Any]"]:
+        alphas = pd.Series(x[: len(self.workers_)], index=self.workers_, name="alpha")  # type: ignore
+        alphas.index.name = "worker"
+        betas = pd.Series(x[len(self.workers_) :], index=self.tasks_, name="beta")  # type: ignore
+        betas.index.name = "task"
         return alphas, betas
 
     def _m_step(self, data: pd.DataFrame) -> pd.DataFrame:
-        """Optimizes the alpha and beta parameters using the conjugate gradient method.
-        """
-        x_0 = np.concatenate([self.alphas_.values, self.betas_.values])  # type: ignore
+        """Optimizes the alpha and beta parameters using the conjugate gradient method."""
+        x_0 = np.concatenate([self.alphas_.values, self.betas_.values])
         self._current_data = data
-        res = minimize(self._optimize_f, x_0, method='CG', jac=self._optimize_df, tol=self.m_step_tol,
-                       options={'disp': False, 'maxiter': self.m_step_max_iter})
+        res = minimize(
+            self._optimize_f,
+            x_0,
+            method="CG",
+            jac=self._optimize_df,
+            tol=self.m_step_tol,
+            options={"disp": False, "maxiter": self.m_step_max_iter},
+        )
         self.alphas_, self.betas_ = self._get_alphas_betas_by_point(res.x)
         self._update_alphas_betas(self.alphas_, self.betas_)
         return self._current_data
 
     def _init(self, data: pd.DataFrame) -> None:
-        self.alphas_ = pd.Series(1.0, index=pd.unique(data.worker))
-        self.betas_ = pd.Series(1.0, index=pd.unique(data.task))
-        self.tasks_ = pd.unique(data['task'])
-        self.workers_ = pd.unique(data['worker'])
+        self.alphas_ = pd.Series(1.0, index=pd.unique(data.worker))  # type: ignore
+        self.betas_ = pd.Series(1.0, index=pd.unique(data.task))  # type: ignore
+        self.tasks_ = pd.unique(data["task"])
+        self.workers_ = pd.unique(data["worker"])
         self.priors_ = self.labels_priors
         if self.priors_ is None:
-            self.prior_labels_ = pd.unique(data['label'])
-            self.priors_ = pd.Series(1. / len(self.prior_labels_), index=self.prior_labels_)
+            self.prior_labels_ = pd.unique(data["label"])
+            self.priors_ = pd.Series(
+                1.0 / len(self.prior_labels_), index=self.prior_labels_  # type: ignore
+            )
+        else:
+            self.prior_labels_ = self.priors_.index  # type: ignore
         self.alphas_priors_mean_ = self.alphas_priors_mean
         if self.alphas_priors_mean_ is None:
-            self.alphas_priors_mean_ = pd.Series(1., index=self.alphas_.index)
+            self.alphas_priors_mean_ = pd.Series(1.0, index=self.alphas_.index)
         self.betas_priors_mean_ = self.betas_priors_mean
         if self.betas_priors_mean_ is None:
-            self.betas_priors_mean_ = pd.Series(1., index=self.betas_.index)
+            self.betas_priors_mean_ = pd.Series(1.0, index=self.betas_.index)
 
     @staticmethod
-    def _softplus(x: pd.Series, limit: int = 30) -> npt.NDArray[Any]:
+    def _softplus(x: "pd.Series[Any]", limit: int = 30) -> npt.NDArray[Any]:
         """log(1 + exp(x)) stable version
 
         For x > 30 or x < -30 error is less than 1e-13
         """
         positive_mask = x > limit
         negative_mask = x < -limit
         mask = positive_mask | negative_mask
-        return cast(npt.NDArray[Any], np.log1p(np.exp(x * (1 - mask))) * (1 - mask) + x * positive_mask)
+        return cast(
+            npt.NDArray[Any],
+            np.log1p(np.exp(x * (1 - mask))) * (1 - mask) + x * positive_mask,
+        )
 
     # backport for scipy < 1.12.0
     @staticmethod
     def _softmax(x: npt.NDArray[Any]) -> npt.NDArray[Any]:
         return cast(npt.NDArray[Any], np.exp(x - logsumexp(x, keepdims=True)))
 
-    def fit(self, data: pd.DataFrame) -> 'GLAD':
+    def fit(self, data: pd.DataFrame) -> "GLAD":
         """Fits the model to the training data with the EM algorithm.
 
         Args:
             data (DataFrame): The training dataset of workers' labeling results
                 which is represented as the `pandas.DataFrame` data containing `task`, `worker`, and `label` columns.
 
         Returns:
             GLAD: self.
         """
 
         # Initialization
-        data = data.filter(['task', 'worker', 'label'])
+        data = data.filter(["task", "worker", "label"])
         self._init(data)
+
+        assert self.alphas_ is not None, "no alphas_"
+        assert self.betas_ is not None, "no betas_"
+        assert self.priors_ is not None, "no priors_"
+
         data = self._join_all(data, self.alphas_, self.betas_, self.priors_)
         data = self._e_step(data)
         Q = self._compute_Q(data)
 
         self.loss_history_ = []
-        iterations_range = tqdm(range(self.n_iter)) if not self.silent else range(self.n_iter)
-        for _ in iterations_range:
+
+        def iteration_progress() -> Tuple[Iterator[int], Optional["tqdm[int]"]]:
+            if self.silent:
+                return iter(range(self.n_iter)), None
+            else:
+                trange_ = trange(self.n_iter, desc="Iterations")
+                return iter(trange_), trange_
+
+        iterator, pbar = iteration_progress()
+
+        for _ in iterator:
             last_Q = Q
             if not self.silent:
-                iterations_range.set_description(f'Q = {round(Q, 4)}')
+                assert isinstance(pbar, tqdm)
+                pbar.set_description(f"Q = {round(Q, 4)}")
 
             # E-step
             data = self._e_step(data)
 
             # M-step
             data = self._m_step(data)
 
@@ -323,25 +370,29 @@
         Args:
             data (DataFrame): The training dataset of workers' labeling results
                 which is represented as the `pandas.DataFrame` data containing `task`, `worker`, and `label` columns.
 
         Returns:
             DataFrame: Probability distributions of task labels.
                 The `pandas.DataFrame` data is indexed by `task` so that `result.loc[task, label]` is the probability that the `task` true label is equal to `label`.
-                Each probability is in he range from 0 to 1, all task probabilities must sum up to 1.
+                Each probability is in the range from 0 to 1, all task probabilities must sum up to 1.
         """
 
-        return self.fit(data).probas_
+        self.fit(data)
+        assert self.probas_ is not None, "no probas_"
+        return self.probas_
 
-    def fit_predict(self, data: pd.DataFrame) -> pd.Series:
+    def fit_predict(self, data: pd.DataFrame) -> "pd.Series[Any]":
         """Fits the model to the training data and returns the aggregated results.
 
         Args:
             data (DataFrame): The training dataset of workers' labeling results
                 which is represented as the `pandas.DataFrame` data containing `task`, `worker`, and `label` columns.
 
         Returns:
             Series: Task labels. The `pandas.Series` data is indexed by `task`
                 so that `labels.loc[task]` is the most likely true label of tasks.
         """
 
-        return self.fit(data).labels_
+        self.fit(data)
+        assert self.labels_ is not None, "no labels_"
+        return self.labels_
```

### Comparing `crowd-kit-1.2.1/crowdkit/aggregation/classification/gold_majority_vote.py` & `crowd-kit-1.3.0rc1/crowdkit/aggregation/classification/gold_majority_vote.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-__all__ = ['GoldMajorityVote']
+__all__ = ["GoldMajorityVote"]
 
-from typing import Optional
+from typing import Any, Optional
 
 import attr
 import pandas as pd
 from sklearn.utils.validation import check_is_fitted
 
-from .majority_vote import MajorityVote
 from ..base import BaseClassificationAggregator
 from ..utils import get_accuracy, named_series_attrib
+from .majority_vote import MajorityVote
 
 
 @attr.s
 class GoldMajorityVote(BaseClassificationAggregator):
     r"""The **Gold Majority Vote** model is used when a golden dataset (ground truth) exists for some tasks.
     It calculates the probability of a correct label for each worker based on the golden set.
     After that, the sum of the probabilities of each label is calculated for each task.
@@ -54,75 +54,79 @@
         probas_ (typing.Optional[pandas.core.frame.DataFrame]): The probability distributions of task labels.
             The `pandas.DataFrame` data is indexed by `task` so that `result.loc[task, label]`
             is the probability that the `task` true label is equal to `label`. Each
             probability is in the range from 0 to 1, all task probabilities must sum up to 1.
     """
 
     # Available after fit
-    skills_: Optional[pd.Series] = named_series_attrib(name='skill')
+    skills_: Optional["pd.Series[Any]"] = named_series_attrib(name="skill")
 
     # Available after predict or predict_proba
     # labels_
     probas_: Optional[pd.DataFrame] = attr.ib(init=False)
 
-    def _apply(self, data: pd.DataFrame) -> 'GoldMajorityVote':
-        check_is_fitted(self, attributes='skills_')
+    def _apply(self, data: pd.DataFrame) -> "GoldMajorityVote":
+        check_is_fitted(self, attributes="skills_")
         mv = MajorityVote().fit(data, self.skills_)
         self.labels_ = mv.labels_
         self.probas_ = mv.probas_
         return self
 
-    def fit(self, data: pd.DataFrame, true_labels: pd.Series) -> 'GoldMajorityVote':  # type: ignore
+    def fit(self, data: pd.DataFrame, true_labels: "pd.Series[Any]") -> "GoldMajorityVote":  # type: ignore
         """Fits the model to the training data.
 
         Args:
             data (DataFrame): The training dataset of workers' labeling results
                 which is represented as the `pandas.DataFrame` data containing `task`, `worker`, and `label` columns.
 
             true_labels (Series): The ground truth labels of tasks. The `pandas.Series` data is indexed by `task`
                 so that `labels.loc[task]` is the task ground truth label.
 
         Returns:
             GoldMajorityVote: self.
         """
 
-        data = data[['task', 'worker', 'label']]
-        self.skills_ = get_accuracy(data, true_labels=true_labels, by='worker')
+        data = data[["task", "worker", "label"]]
+        self.skills_ = get_accuracy(data, true_labels=true_labels, by="worker")
         return self
 
-    def predict(self, data: pd.DataFrame) -> pd.Series:
+    def predict(self, data: pd.DataFrame) -> "pd.Series[Any]":
         """Predicts the true labels of tasks when the model is fitted.
 
         Args:
             data (DataFrame): The training dataset of workers' labeling results
                 which is represented as the `pandas.DataFrame` data containing `task`, `worker`, and `label` columns.
 
         Returns:
             Series: The task labels. The `pandas.Series` data is indexed by `task`
                 so that `labels.loc[task]` is the most likely true label of tasks.
         """
 
-        return self._apply(data).labels_
+        self._apply(data)
+        assert self.labels_ is not None, "no labels_"
+        return self.labels_
 
     def predict_proba(self, data: pd.DataFrame) -> pd.DataFrame:
         """Returns probability distributions of labels for each task when the model is fitted.
 
         Args:
             data (DataFrame): The training dataset of workers' labeling results
                 which is represented as the `pandas.DataFrame` data containing `task`, `worker`, and `label` columns.
 
         Returns:
             DataFrame: Probability distributions of task labels.
                 The `pandas.DataFrame` data is indexed by `task` so that `result.loc[task, label]` is the probability that the `task` true label is equal to `label`.
-                Each probability is in he range from 0 to 1, all task probabilities must sum up to 1.
+                Each probability is in the range from 0 to 1, all task probabilities must sum up to 1.
         """
 
-        return self._apply(data).probas_
+        self._apply(data)
+        assert self.probas_ is not None, "no probas_"
+        return self.probas_
 
-    def fit_predict(self, data: pd.DataFrame, true_labels: pd.Series) -> pd.Series:  # type: ignore
+    def fit_predict(self, data: pd.DataFrame, true_labels: "pd.Series[Any]") -> "pd.Series[Any]":  # type: ignore
         """Fits the model to the training data and returns the aggregated results.
         Args:
             data (DataFrame): The training dataset of workers' labeling results
                 which is represented as the `pandas.DataFrame` data containing `task`, `worker`, and `label` columns.
 
             true_labels (Series): The ground truth labels of tasks. The `pandas.Series` data is indexed by `task`
                 so that `labels.loc[task]` is the task ground truth label.
@@ -130,24 +134,26 @@
         Returns:
             Series: The task labels. The `pandas.Series` data is indexed by `task`
                 so that `labels.loc[task]` is the most likely true label of tasks.
         """
 
         return self.fit(data, true_labels).predict(data)
 
-    def fit_predict_proba(self, data: pd.DataFrame, true_labels: pd.Series) -> pd.DataFrame:
+    def fit_predict_proba(
+        self, data: pd.DataFrame, true_labels: "pd.Series[Any]"
+    ) -> pd.DataFrame:
         """Fits the model to the training data and returns probability distributions of labels for each task.
 
         Args:
             data (DataFrame): The training dataset of workers' labeling results
                 which is represented as the `pandas.DataFrame` data containing `task`, `worker`, and `label` columns.
 
-            true_labels (Series): The ground truth labels of tasks. The `pandas.Series` daata is indexed by `task`
+            true_labels (Series): The ground truth labels of tasks. The `pandas.Series` data is indexed by `task`
                 so that `labels.loc[task]` is the task ground truth label.
 
         Returns:
             DataFrame: Probability distributions of task labels.
                 The `pandas.DataFrame` data is indexed by `task` so that `result.loc[task, label]` is the probability that the `task` true label is equal to `label`.
-                Each probability is in he range from 0 to 1, all task probabilities must sum up to 1.
+                Each probability is in the range from 0 to 1, all task probabilities must sum up to 1.
         """
 
         return self.fit(data, true_labels).predict_proba(data)
```

### Comparing `crowd-kit-1.2.1/crowdkit/aggregation/classification/kos.py` & `crowd-kit-1.3.0rc1/crowdkit/aggregation/classification/kos.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-__all__ = [
-    'KOS'
-]
+__all__ = ["KOS"]
+
+from typing import Any, cast
 
 import attr
 import numpy as np
 import pandas as pd
 
 from ..base import BaseClassificationAggregator
 
@@ -30,89 +30,97 @@
     $$
 
     David R. Karger, Sewoong Oh, and Devavrat Shah. Budget-Optimal Task Allocation for Reliable Crowdsourcing Systems.
     *Operations Research 62.1 (2014)*, 1-38.
 
     <https://arxiv.org/abs/1110.3564>
 
-    Args:
-        n_iter: The maximum number of iterations.
-        random_state: The state of the random number generator.
-
     Examples:
         >>> from crowdkit.aggregation import KOS
         >>> from crowdkit.datasets import load_dataset
         >>> df, gt = load_dataset('relevance-2')
         >>> ds = KOS(10)
         >>> result = ds.fit_predict(df)
-
-    Attributes:
-        labels_ (Optional[pd.Series]): The task labels. The `pandas.Series` data is indexed by `task`
-            so that `labels.loc[task]` is the most likely true label of tasks.
-
     """
 
     n_iter: int = attr.ib(default=100)
+    """The maximum number of iterations."""
+
     random_state: int = attr.ib(default=0)
+    """The state of the random number generator."""
 
-    def fit(self, data: pd.DataFrame) -> 'KOS':
+    def fit(self, data: pd.DataFrame) -> "KOS":
         """Fits the model to the training data.
         Args:
             data (DataFrame): The training dataset of workers' labeling results
                 which is represented as the `pandas.DataFrame` data containing `task`, `worker`, and `label` columns.
 
         Returns:
             KOS: self.
         """
 
         np.random.seed(self.random_state)
 
         # Early exit
         if not data.size:
-            self.labels_ = pd.Series([], dtype='O')
+            self.labels_ = pd.Series([], dtype="O")
             return self
 
         # Initialization
         kos_data = data.copy()
         labels = kos_data.label.unique()
         if len(labels) != 2:
-            raise ValueError('KOS aggregation method is for binary classification only.')
+            raise ValueError(
+                "KOS aggregation method is for binary classification only."
+            )
         mapping = {labels[0]: 1, labels[1]: -1}
         kos_data.label = kos_data.label.apply(lambda x: mapping[x])
-        kos_data['reliabilities'] = np.random.normal(loc=1, scale=1, size=len(kos_data))
+        kos_data["reliabilities"] = np.random.normal(loc=1, scale=1, size=len(kos_data))
 
         # Updating reliabilities
         for _ in range(self.n_iter):
             # Update inferred labels for (task, worker)
-            kos_data['multiplied'] = kos_data.label * kos_data.reliabilities
-            kos_data['summed'] = list(kos_data.groupby('task')['multiplied'].sum()[kos_data.task])
+            kos_data["multiplied"] = kos_data.label * kos_data.reliabilities
+            kos_data["summed"] = list(
+                kos_data.groupby("task")["multiplied"].sum()[kos_data.task]
+            )
             # Early exit to prevent NaN
-            if (np.abs(kos_data['summed']) > _MAX).any():
+            if (np.abs(kos_data["summed"]) > _MAX).any():
                 break
-            kos_data['inferred'] = (kos_data['summed'] - kos_data['multiplied']).astype(float)
+            kos_data["inferred"] = (kos_data["summed"] - kos_data["multiplied"]).astype(
+                float
+            )
 
             # Update reliabilities for (task, worker)
-            kos_data['multiplied'] = kos_data.label * kos_data.inferred
-            kos_data['summed'] = list(kos_data.groupby('worker')['multiplied'].sum()[kos_data.worker])
+            kos_data["multiplied"] = kos_data.label * kos_data.inferred
+            kos_data["summed"] = list(
+                kos_data.groupby("worker")["multiplied"].sum()[kos_data.worker]
+            )
             # Early exit to prevent NaN
-            if (np.abs(kos_data['summed']) > _MAX).any():
+            if (np.abs(kos_data["summed"]) > _MAX).any():
                 break
-            kos_data['reliabilities'] = (kos_data.summed - kos_data.multiplied).astype('float')
+            kos_data["reliabilities"] = (kos_data.summed - kos_data.multiplied).astype(
+                "float"
+            )
 
-        kos_data['inferred'] = kos_data.label * kos_data.reliabilities
-        inferred_labels = np.sign(kos_data.groupby('task')['inferred'].sum())
+        kos_data["inferred"] = kos_data.label * kos_data.reliabilities
+        inferred_labels = np.sign(kos_data.groupby("task")["inferred"].sum())
         back_mapping = {v: k for k, v in mapping.items()}
-        self.labels_ = inferred_labels.apply(lambda x: back_mapping[x])
+        self.labels_ = cast(
+            "pd.Series[Any]", inferred_labels.apply(lambda x: back_mapping[x])
+        )
         return self
 
-    def fit_predict(self, data: pd.DataFrame) -> pd.DataFrame:
+    def fit_predict(self, data: pd.DataFrame) -> "pd.Series[Any]":
         """Fits the model to the training data and returns the aggregated results.
         Args:
             data (DataFrame): The training dataset of workers' labeling results
                 which is represented as the `pandas.DataFrame` data containing `task`, `worker`, and `label` columns.
 
         Returns:
             Series: The task labels. The `pandas.Series` data is indexed by `task`
                 so that `labels.loc[task]` is the most likely true label of tasks.
         """
 
-        return self.fit(data).labels_
+        self.fit(data)
+        assert self.labels_ is not None, "no labels_"
+        return self.labels_
```

### Comparing `crowd-kit-1.2.1/crowdkit/aggregation/classification/m_msr.py` & `crowd-kit-1.3.0rc1/crowdkit/aggregation/classification/m_msr.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-__all__ = ['MMSR']
+__all__ = ["MMSR"]
 
-from typing import Optional, List, Any, Dict
+from typing import Any, Dict, List, Optional
 
 import attr
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
 import scipy.sparse.linalg as sla
 import scipy.stats as sps
 
-from .majority_vote import MajorityVote
 from ..base import BaseClassificationAggregator
 from ..utils import named_series_attrib
+from .majority_vote import MajorityVote
 
 
 @attr.s
 class MMSR(BaseClassificationAggregator):
     r"""The **Matrix Mean-Subsequence-Reduced Algorithm** (M-MSR) model assumes that workers have different expertise levels and are represented
     as a vector of "skills" $s$ which entries $s_i$ show the probability
     that the worker $i$ will answer the given task correctly. Having that, we can estimate the probability of each worker via solving a rank-one matrix completion problem as follows:
@@ -23,133 +23,136 @@
     \mathbb{E}\left[\frac{M}{M-1}\widetilde{C}-\frac{1}{M-1}\boldsymbol{1}\boldsymbol{1}^T\right]
      = \boldsymbol{s}\boldsymbol{s}^T,
     $$
     where $M$ is the total number of classes, $\widetilde{C}$ is a covariance matrix between
     workers, and $\boldsymbol{1}\boldsymbol{1}^T$ is the all-ones matrix which has the same
     size as $\widetilde{C}$.
 
-
     Thus, the problem of estimating the skill level vector $s$ becomes equivalent to the
     rank-one matrix completion problem. The M-MSR algorithm is an iterative algorithm for the *robust*
     rank-one matrix completion, so its result is an estimator of the vector $s$.
     And the aggregation is weighted majority voting with weights equal to
     $\log \frac{(M-1)s_i}{1-s_i}$.
 
     Q. Ma and Alex Olshevsky. Adversarial Crowdsourcing Through Robust Rank-One Matrix Completion.
     *34th Conference on Neural Information Processing Systems (NeurIPS 2020)*
 
     <https://arxiv.org/abs/2010.12181>
 
-    Args:
-        n_iter: The maximum number of iterations.
-        tol: The tolerance stopping criterion for iterative methods with a variable number of steps.
-            The algorithm converges when the loss change is less than the `tol` parameter.
-        random_state: The seed number for the random initialization.
-        _observation_matrix: The matrix representing which workers give responses to which tasks.
-        _covariation_matrix: The matrix representing the covariance between workers.
-        _n_common_tasks: The matrix representing workers with tasks in common.
-        _n_workers: The number of workers.
-        _n_tasks: The number of tasks that are assigned to workers.
-        _n_labels: The number of possible labels for a series of classification tasks.
-        _labels_mapping: The mapping of labels and integer values.
-        _workers_mapping: The mapping of workers and integer values.
-        _tasks_mapping: The mapping of tasks and integer values.
-
     Examples:
         >>> from crowdkit.aggregation import MMSR
         >>> from crowdkit.datasets import load_dataset
         >>> df, gt = load_dataset('relevance-2')
         >>> mmsr = MMSR()
         >>> result = mmsr.fit_predict(df)
-    Attributes:
-        labels_ (typing.Optional[pandas.core.series.Series]): The task labels. The `pandas.Series` data is indexed by `task`
-            so that `labels.loc[task]` is the most likely true label of tasks.
-
-        skills_ (typing.Optional[pandas.core.series.Series]): The workers' skills. The `pandas.Series` data is indexed by `worker`
-            and has the corresponding worker skill.
-
-        scores_ (typing.Optional[pandas.core.frame.DataFrame]): The task label scores. The `pandas.DataFrame` data is indexed by `task`
-            so that `result.loc[task, label]` is a score of `label` for `task`.
-
-        loss_history_ (List[float]): A list of loss values during training.
     """
 
     n_iter: int = attr.ib(default=10000)
+    """The maximum number of iterations."""
+
     tol: float = attr.ib(default=1e-10)
+    """The tolerance stopping criterion for iterative methods with a variable number of steps. The algorithm converges when the loss change is less than the `tol` parameter."""
+
     random_state: Optional[int] = attr.ib(default=0)
+    """The seed number for the random initialization."""
+
     _observation_matrix: npt.NDArray[Any] = attr.ib(factory=lambda: np.array([]))
+    """The matrix representing which workers give responses to which tasks."""
+
     _covariation_matrix: npt.NDArray[Any] = attr.ib(factory=lambda: np.array([]))
+    """The matrix representing the covariance between workers."""
+
     _n_common_tasks: npt.NDArray[Any] = attr.ib(factory=lambda: np.array([]))
+    """The matrix representing workers with tasks in common."""
+
     _n_workers: int = attr.ib(default=0)
+    """The number of workers."""
+
     _n_tasks: int = attr.ib(default=0)
+    """The number of tasks that are assigned to workers."""
+
     _n_labels: int = attr.ib(default=0)
+    """The number of possible labels for a series of classification tasks."""
+
     _labels_mapping: Dict[Any, int] = attr.ib(factory=dict)
+    """The mapping of labels and integer values."""
+
     _workers_mapping: Dict[Any, int] = attr.ib(factory=dict)
+    """The mapping of workers and integer values."""
+
     _tasks_mapping: Dict[Any, int] = attr.ib(factory=dict)
+    """The mapping of tasks and integer values."""
 
     # Available after fit
-    skills_: Optional[pd.Series] = named_series_attrib(name='skill')
+    skills_: Optional["pd.Series[Any]"] = named_series_attrib(name="skill")
+    """The task labels.
+    The `pandas.Series` data is indexed by `task` so that `labels.loc[task]` is the most likely true label of tasks."""
 
-    # Available after predict or predict_score
-    # labels_
     scores_: Optional[pd.DataFrame] = attr.ib(init=False)
+    """The task label scores.
+    The `pandas.DataFrame` data is indexed by `task` so that `result.loc[task, label]` is a score of `label` for `task`."""
 
     loss_history_: List[float] = attr.ib(init=False)
+    """A list of loss values during training."""
 
-    def _apply(self, data: pd.DataFrame) -> 'MMSR':
+    def _apply(self, data: pd.DataFrame) -> "MMSR":
         mv = MajorityVote().fit(data, skills=self.skills_)
         self.labels_ = mv.labels_
         self.scores_ = mv.probas_
         return self
 
-    def fit(self, data: pd.DataFrame) -> 'MMSR':
+    def fit(self, data: pd.DataFrame) -> "MMSR":
         """Fits the model to the training data.
 
         Args:
             data (DataFrame): The training dataset of workers' labeling results
                 which is represented as the `pandas.DataFrame` data containing `task`, `worker`, and `label` columns.
 
         Returns:
             MMSR: self.
         """
 
-        data = data[['task', 'worker', 'label']]
+        data = data[["task", "worker", "label"]]
         self._construnct_covariation_matrix(data)
         self._m_msr()
         return self
 
-    def predict(self, data: pd.DataFrame) -> pd.Series:
+    def predict(self, data: pd.DataFrame) -> "pd.Series[Any]":
         """Predicts the true labels of tasks when the model is fitted.
 
         Args:
             data (DataFrame): The training dataset of workers' labeling results
                 which is represented as the `pandas.DataFrame` data containing `task`, `worker`, and `label` columns.
 
         Returns:
             Series: The task labels. The `pandas.Series` data is indexed by `task`
                 so that `labels.loc[task]` is the most likely true label of tasks.
         """
 
-        return self._apply(data).labels_
+        self._apply(data)
+        assert self.labels_ is not None, "no labels_"
+        return self.labels_
 
     def predict_score(self, data: pd.DataFrame) -> pd.DataFrame:
         """Returns the total sum of weights for each label when the model is fitted.
 
         Args:
             data (DataFrame): The training dataset of workers' labeling results
                 which is represented as the `pandas.DataFrame` data containing `task`, `worker`, and `label` columns.
 
         Returns:
             DataFrame: The task label scores. The `pandas.DataFrame` data is indexed by `task`
                 so that `result.loc[task, label]` is a score of `label` for `task`.
         """
 
-        return self._apply(data).scores_
+        self._apply(data)
+        assert self.scores_ is not None, "no scores_"
+        return self.scores_
 
-    def fit_predict(self, data: pd.DataFrame) -> pd.Series:
+    def fit_predict(self, data: pd.DataFrame) -> "pd.Series[Any]":
         """Fits the model to the training data and returns the aggregated results.
 
         Args:
             data (DataFrame): The training dataset of workers' labeling results
                 which is represented as the `pandas.DataFrame` data containing `task`, `worker`, and `label` columns.
 
         Returns:
@@ -178,95 +181,116 @@
         n, m = self._covariation_matrix.shape
         u = sps.uniform.rvs(size=(n, 1), random_state=self.random_state)
         v = sps.uniform.rvs(size=(m, 1), random_state=self.random_state)
         observed_entries = np.abs(np.sign(self._n_common_tasks)) == 1
         X = np.abs(self._covariation_matrix)
         self.loss_history_ = []
         for _ in range(self.n_iter):
-            v_prev = np.copy(v)  # type: ignore
-            u_prev = np.copy(u)  # type: ignore
+            v_prev = np.copy(v)
+            u_prev = np.copy(u)
             for j in range(n):
                 target_v = X[:, j].reshape(-1, 1)
                 target_v = target_v[observed_entries[:, j]] / u[observed_entries[:, j]]
 
-                y = self._remove_largest_and_smallest_F_value(target_v, F_param, v[j][0], self._n_tasks)
+                y = self._remove_largest_and_smallest_F_value(
+                    target_v, F_param, v[j][0], self._n_tasks
+                )
                 if len(y) == 0:
                     v[j] = v[j]
                 else:
                     v[j][0] = y.mean()
 
             for i in range(m):
                 target_u = X[i, :].reshape(-1, 1)
                 target_u = target_u[observed_entries[i, :]] / v[observed_entries[i, :]]
-                y = self._remove_largest_and_smallest_F_value(target_u, F_param, u[i][0], self._n_tasks)
+                y = self._remove_largest_and_smallest_F_value(
+                    target_u, F_param, u[i][0], self._n_tasks
+                )
                 if len(y) == 0:
                     u[i] = u[i]
                 else:
                     u[i][0] = y.mean()
 
-            loss = np.linalg.norm(u @ v.T - u_prev @ v_prev.T, ord='fro')  # type: ignore
+            loss = np.linalg.norm(u @ v.T - u_prev @ v_prev.T, ord="fro")
             self.loss_history_.append(float(loss))
             if loss < self.tol:
                 break
 
-        k = np.sqrt(np.linalg.norm(u) / np.linalg.norm(v))  # type: ignore
+        k = np.sqrt(np.linalg.norm(u) / np.linalg.norm(v))
         x_track_1 = u / k
         x_track_2 = self._sign_determination_valid(self._covariation_matrix, x_track_1)
-        x_track_3 = np.minimum(x_track_2, 1 - 1. / np.sqrt(self._n_tasks))
-        x_MSR = np.maximum(x_track_3, -1 / (self._n_labels - 1) + 1. / np.sqrt(self._n_tasks))
-
-        workers_probas = x_MSR * (self._n_labels - 1) / (self._n_labels) + 1 / self._n_labels
+        x_track_3 = np.minimum(x_track_2, 1 - 1.0 / np.sqrt(self._n_tasks))
+        x_MSR = np.maximum(
+            x_track_3, -1 / (self._n_labels - 1) + 1.0 / np.sqrt(self._n_tasks)
+        )
+
+        workers_probas = (
+            x_MSR * (self._n_labels - 1) / (self._n_labels) + 1 / self._n_labels
+        )
         workers_probas = workers_probas.ravel()
         skills = np.log(workers_probas * (self._n_labels - 1) / (1 - workers_probas))
 
         self.skills_ = self._get_skills_from_array(skills)
 
-    def _get_skills_from_array(self, array: npt.NDArray[Any]) -> pd.Series:
-        inverse_workers_mapping = {ind: worker for worker, ind in self._workers_mapping.items()}
+    def _get_skills_from_array(self, array: npt.NDArray[Any]) -> "pd.Series[Any]":
+        inverse_workers_mapping = {
+            ind: worker for worker, ind in self._workers_mapping.items()
+        }
         index = [inverse_workers_mapping[i] for i in range(len(array))]
-        return pd.Series(array, index=pd.Index(index, name='worker'))
+        return pd.Series(array, index=pd.Index(index, name="worker"))
 
     @staticmethod
-    def _sign_determination_valid(C: npt.NDArray[Any], s_abs: npt.NDArray[Any]) -> npt.NDArray[Any]:
+    def _sign_determination_valid(
+        C: npt.NDArray[Any], s_abs: npt.NDArray[Any]
+    ) -> npt.NDArray[Any]:
         S = np.sign(C)
         n = len(s_abs)
 
         valid_idx = np.where(np.sum(C, axis=1) != 0)[0]
         S_valid = S[valid_idx[:, None], valid_idx]
         k = S_valid.shape[0]
-        upper_idx = np.triu(np.ones(shape=(k, k)))  # type: ignore
+        upper_idx = np.triu(np.ones(shape=(k, k)))
         S_valid_upper = S_valid * upper_idx
         new_node_end_I, new_node_end_J = np.where(S_valid_upper == 1)
         S_valid[S_valid == 1] = 0
         I = np.eye(k)
         S_valid_new = I[new_node_end_I, :] + I[new_node_end_J, :]
         m = S_valid_new.shape[0]
-        A = np.vstack((np.hstack((np.abs(S_valid), S_valid_new.T)), np.hstack((S_valid_new, np.zeros(shape=(m, m))))))
+        A = np.vstack(
+            (
+                np.hstack((np.abs(S_valid), S_valid_new.T)),
+                np.hstack((S_valid_new, np.zeros(shape=(m, m)))),
+            )
+        )
         n_new = A.shape[0]
-        W = (1. / np.sum(A, axis=1)).reshape(-1, 1) @ np.ones(shape=(1, n_new)) * A
-        D, V = sla.eigs(W + np.eye(n_new), 1, which='SM')
+        W = (1.0 / np.sum(A, axis=1)).reshape(-1, 1) @ np.ones(shape=(1, n_new)) * A
+        D, V = sla.eigs(W + np.eye(n_new), 1, which="SM")
         V = V.real
         sign_vector = np.sign(V)
         s_sign = np.zeros(shape=(n, 1))
-        s_sign[valid_idx] = np.sign(np.sum(sign_vector[:k])) * s_abs[valid_idx] * sign_vector[:k]
+        s_sign[valid_idx] = (
+            np.sign(np.sum(sign_vector[:k])) * s_abs[valid_idx] * sign_vector[:k]
+        )
         return s_sign
 
     @staticmethod
-    def _remove_largest_and_smallest_F_value(x: npt.NDArray[Any], F: int, a: float, n_tasks: int) -> npt.NDArray[Any]:
+    def _remove_largest_and_smallest_F_value(
+        x: npt.NDArray[Any], F: int, a: float, n_tasks: int
+    ) -> npt.NDArray[Any]:
         y = np.sort(x, axis=0)
         if np.sum(y < a) < F:
             y = y[y[:, 0] >= a]
         else:
             y = y[F:]
 
         m = y.shape[0]
         if np.sum(y > a) < F:
             y = y[y[:, 0] <= a]
         else:
-            y = np.concatenate((y[:m - F], y[m:]), axis=0)  # type: ignore
+            y = np.concatenate((y[: m - F], y[m:]), axis=0)
         if len(y) == 1 and y[0][0] == 0:
             y[0][0] = 1 / np.sqrt(n_tasks)
         return y
 
     def _construnct_covariation_matrix(self, answers: pd.DataFrame) -> None:
         labels = pd.unique(answers.label)
         self._n_labels = len(labels)
@@ -278,26 +302,37 @@
 
         tasks = pd.unique(answers.task)
         self._n_tasks = len(tasks)
         self._tasks_mapping = {tasks[idx]: idx for idx in range(self._n_tasks)}
 
         self._observation_matrix = np.zeros(shape=(self._n_workers, self._n_tasks))
         for i, row in answers.iterrows():
-            self._observation_matrix[self._workers_mapping[row['worker']]][self._tasks_mapping[row['task']]] = \
-                self._labels_mapping[row['label']]
-
-        self._n_common_tasks = np.sign(self._observation_matrix) @ np.sign(self._observation_matrix).T
-        self._n_common_tasks -= np.diag(np.diag(self._n_common_tasks))  # type: ignore
-        self._sparsity = np.min(np.sign(self._n_common_tasks).sum(axis=0))  # type: ignore
+            self._observation_matrix[self._workers_mapping[row["worker"]]][
+                self._tasks_mapping[row["task"]]
+            ] = self._labels_mapping[row["label"]]
+
+        self._n_common_tasks = (
+            np.sign(self._observation_matrix) @ np.sign(self._observation_matrix).T
+        )
+        self._n_common_tasks -= np.diag(np.diag(self._n_common_tasks))
+        self._sparsity = np.min(np.sign(self._n_common_tasks).sum(axis=0))
 
         # Can we rewrite it in matrix operations?
         self._covariation_matrix = np.zeros(shape=(self._n_workers, self._n_workers))
         for i in range(self._n_workers):
             for j in range(self._n_workers):
                 if self._n_common_tasks[i][j]:
-                    valid_idx = np.sign(self._observation_matrix[i]) * np.sign(self._observation_matrix[j])
-                    self._covariation_matrix[i][j] = np.sum(
-                        (self._observation_matrix[i] == self._observation_matrix[j]) * valid_idx) / \
-                                                     self._n_common_tasks[i][j]
+                    valid_idx = np.sign(self._observation_matrix[i]) * np.sign(
+                        self._observation_matrix[j]
+                    )
+                    self._covariation_matrix[i][j] = (
+                        np.sum(
+                            (self._observation_matrix[i] == self._observation_matrix[j])
+                            * valid_idx
+                        )
+                        / self._n_common_tasks[i][j]
+                    )
 
         self._covariation_matrix *= self._n_labels / (self._n_labels - 1)
-        self._covariation_matrix -= np.ones(shape=(self._n_workers, self._n_workers)) / (self._n_labels - 1)
+        self._covariation_matrix -= np.ones(
+            shape=(self._n_workers, self._n_workers)
+        ) / (self._n_labels - 1)
```

### Comparing `crowd-kit-1.2.1/crowdkit/aggregation/classification/mace.py` & `crowd-kit-1.3.0rc1/crowdkit/aggregation/classification/mace.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,53 +1,56 @@
-__all__ = ['MACE']
+__all__ = ["MACE"]
+
+from typing import Any, Iterator, List, Optional, Tuple, Union
 
-from typing import Any, List, Optional, Tuple
 import attr
 import numpy as np
-from numpy.typing import NDArray
 import pandas as pd
 import scipy.stats as sps
+from numpy.typing import NDArray
 from scipy.special import digamma
-from tqdm.auto import trange
+from tqdm.auto import tqdm, trange
 
 from ..base import BaseClassificationAggregator
 
 
 def normalize(x: NDArray[np.float64], smoothing: float) -> NDArray[np.float64]:
     """Normalizes the rows of the matrix using the smoothing parameter.
 
     Args:
         x (np.ndarray): The array to normalize.
         smoothing (float): The smoothing parameter.
 
     Returns:
         np.ndarray: Normalized array
     """
-    norm = (x + smoothing).sum(axis=1)  # type: ignore
-    return np.divide(  # type: ignore
+    norm = (x + smoothing).sum(axis=1)
+    return np.divide(
         x + smoothing,
         norm[:, np.newaxis],
         out=np.zeros_like(x),
         where=~np.isclose(norm[:, np.newaxis], np.zeros_like(norm[:, np.newaxis])),
     )
 
 
-def variational_normalize(x: NDArray[np.float64], hparams: NDArray[np.float64]) -> NDArray[np.float64]:
+def variational_normalize(
+    x: NDArray[np.float64], hparams: NDArray[np.float64]
+) -> NDArray[np.float64]:
     """Normalizes the rows of the matrix using the MACE priors.
 
     Args:
         x (np.ndarray): The array to normalize.
         hparams (np.ndarray): The prior parameters.
 
     Returns:
         np.ndarray: Normalized array
     """
-    norm = (x + hparams).sum(axis=1)  # type: ignore
+    norm = (x + hparams).sum(axis=1)
     norm = np.exp(digamma(norm))
-    return np.divide(  # type: ignore
+    return np.divide(
         np.exp(digamma(x + hparams)),
         norm[:, np.newaxis],
         out=np.zeros_like(x),
         where=~np.isclose(norm[:, np.newaxis], np.zeros_like(norm[:, np.newaxis])),
     )
 
 
@@ -87,98 +90,106 @@
     3. **Variational M-step**. Employs Variational-Bayes (VB) training with symmetric Beta priors on $\theta_j$ and symmetric Dirichlet priors on the strategy parameters $\xi_j.
 
     D. Hovy, T. Berg-Kirkpatrick, A. Vaswani and E. Hovy. Learning Whom to Trust with MACE.
     In *Proceedings of NAACL-HLT*, Atlanta, GA, USA (2013), 1120–1130.
 
     <https://aclanthology.org/N13-1132.pdf>
 
-    Args:
-        n_restarts (int): The number of optimization runs of the algorithms. The final parameters are those that gave the best log likelihood.
-            If one run takes too long, this parameter can be set to 1. Default: 10.
-        n_iter (int): The maximum number of EM iterations for each optimization run. Default: 50.
-        method (str): The method which is used for the M-step. Either 'vb' or 'em'. 'vb' means optimization with Variational Bayes using priors.
-            'em' means standard Expectation-Maximization algorithm. Default: 'vb'.
-        smoothing (float): The smoothing parameter for the normalization. Default: 0.1.
-        default_noise (float): The default noise parameter for the initialization. Default: 0.5.
-        alpha (float): The prior parameter for the Beta distribution on $\theta_j$. Default: 0.5.
-        beta (float): The prior parameter for the Beta distribution on $\theta_j$. Default: 0.5.
-        random_state (int): The state of the random number generator. Default: 0.
-        verbose (int): Specifies if the progress will be printed or not: 0 — no progress bar, 1 — only for restarts,
-            2 — for both restarts and optimization. Default: 0.
-
     Examples:
         >>> from crowdkit.aggregation import MACE
         >>> from crowdkit.datasets import load_dataset
         >>> df, gt = load_dataset('relevance-2')
         >>> mace = MACE()
         >>> result = mace.fit_predict(df)
-
-    Attributes:
-        labels_ (Optional[pd.Series]): The task labels. The `pandas.Series` data is indexed by `task`
-            so that `labels.loc[task]` is the most likely true label of tasks.
-
-        probas_ (Optional[pandas.core.frame.DataFrame]): The probability distributions of task labels.
-            The `pandas.DataFrame` data is indexed by `task` so that `result.loc[task, label]` is the probability that the `task` true label is equal to `label`.
-            Each probability is in the range from 0 to 1, all task probabilities must sum up to 1.
-
-        spamming_ (np.ndarray): The posterior distribution of workers' spamming states.
-
-        thetas_ (np.ndarray): The posterior distribution of workers' spamming labels.
-
-        theta_priors_ (Optional[np.ndarray]): The prior parameters for the Beta distribution on $\theta_j$.
-
-        strategy_priors_ (Optional[np.ndarray]): The prior parameters for the Diriclet distribution on $\xi_j$.
     """
 
     n_restarts: int = attr.ib(default=10)
+    """The number of optimization runs of the algorithms.
+    The final parameters are those that gave the best log likelihood.
+    If one run takes too long, this parameter can be set to 1."""
+
     n_iter: int = attr.ib(default=50)
+    """The maximum number of EM iterations for each optimization run."""
+
     method: str = attr.ib(default="vb")
+    """The method which is used for the M-step. Either 'vb' or 'em'.
+    'vb' means optimization with Variational Bayes using priors.
+    'em' means standard Expectation-Maximization algorithm."""
+
     smoothing: float = attr.ib(default=0.1)
+    """The smoothing parameter for the normalization."""
+
     default_noise: float = attr.ib(default=0.5)
+    """The default noise parameter for the initialization."""
+
     alpha: float = attr.ib(default=0.5)
+    """The prior parameter for the Beta distribution on $\theta_j$."""
+
     beta: float = attr.ib(default=0.5)
+    """The prior parameter for the Beta distribution on $\theta_j$."""
+
     random_state: int = attr.ib(default=0)
+    """The state of the random number generator."""
+
     verbose: int = attr.ib(default=0)
+    """Specifies if the progress will be printed or not:
+    0 — no progress bar, 1 — only for restarts, 2 — for both restarts and optimization."""
 
     spamming_: NDArray[np.float64] = attr.ib(init=False)
+    """The posterior distribution of workers' spamming states."""
+
     thetas_: NDArray[np.float64] = attr.ib(init=False)
+    """The posterior distribution of workers' spamming labels."""
+
     theta_priors_: Optional[NDArray[np.float64]] = attr.ib(init=False)
+    r"""The prior parameters for the Beta distribution on $\theta_j$."""
+
     strategy_priors_: Optional[NDArray[np.float64]] = attr.ib(init=False)
+    r"""The prior parameters for the Diriclet distribution on $\xi_j$."""
+
     smoothing_: float = attr.ib(init=False)
+    """The smoothing parameter."""
+
     probas_: Optional[pd.DataFrame] = attr.ib(init=False)
+    """The probability distributions of task labels.
+    The `pandas.DataFrame` data is indexed by `task` so that `result.loc[task, label]` is the probability that
+    the `task` true label is equal to `label`. Each probability is in the range from 0 to 1,
+    all task probabilities must sum up to 1."""
 
-    def fit(self, data: pd.DataFrame) -> 'MACE':
+    def fit(self, data: pd.DataFrame) -> "MACE":
         """Fits the model to the training data.
 
         Args:
             data (DataFrame): The training dataset of workers' labeling results
                 which is represented as the `pandas.DataFrame` data containing `task`, `worker`, and `label` columns.
 
         Returns:
             MACE: The fitted MACE model.
         """
 
-        workers, worker_names = pd.factorize(data['worker'])
-        labels, label_names = pd.factorize(data['label'])
-        tasks, task_names = pd.factorize(data['task'])
+        workers, worker_names = pd.factorize(data["worker"])
+        labels, label_names = pd.factorize(data["label"])
+        tasks, task_names = pd.factorize(data["task"])
 
         n_workers = len(worker_names)
         n_labels = len(label_names)
 
         self.smoothing_ = 0.01 / n_labels
 
         annotation = data.copy(deep=True)
 
         best_log_marginal_likelihood = -np.inf
-        restarts_progress = (
-            trange(self.n_restarts) if self.verbose > 0 else range(self.n_restarts)
-        )
-        if self.verbose > 0:
-            restarts_progress.set_description('Restarts')
-        for _ in restarts_progress:
+
+        def restarts_progress() -> Iterator[int]:
+            if self.verbose > 0:
+                yield from trange(self.n_restarts, desc="Restarts")
+            else:
+                yield from range(self.n_restarts)
+
+        for _ in restarts_progress():
             self._initialize(n_workers, n_labels)
             (
                 log_marginal_likelihood,
                 gold_label_marginals,
                 strategy_expected_counts,
                 knowing_expected_counts,
             ) = self._e_step(
@@ -186,19 +197,26 @@
                 task_names,
                 worker_names,
                 label_names,
                 tasks,
                 workers,
                 labels,
             )
-            iter_progress = (
-                trange(self.n_iter) if self.verbose > 1 else range(self.n_iter)
-            )
-            for _ in iter_progress:
-                if self.method == 'vb':
+
+            def iteration_progress() -> Tuple[Iterator[int], Optional["tqdm[int]"]]:
+                if self.verbose > 1:
+                    trange_ = trange(self.n_iter, desc="Iterations")
+                    return iter(trange_), trange_
+                else:
+                    return iter(range(self.n_iter)), None
+
+            iterator, pbar = iteration_progress()
+
+            for _ in iterator:
+                if self.method == "vb":
                     self._variational_m_step(
                         knowing_expected_counts, strategy_expected_counts
                     )
                 else:
                     self._m_step(knowing_expected_counts, strategy_expected_counts)
                 (
                     log_marginal_likelihood,
@@ -211,62 +229,67 @@
                     worker_names,
                     label_names,
                     tasks,
                     workers,
                     labels,
                 )
                 if self.verbose > 1:
-                    iter_progress.set_postfix(
-                        {'log_marginal_likelihood': round(log_marginal_likelihood, 5)}
+                    assert isinstance(pbar, tqdm)
+                    pbar.set_postfix(
+                        {"log_marginal_likelihood": round(log_marginal_likelihood, 5)}
                     )
             if log_marginal_likelihood > best_log_marginal_likelihood:
                 best_log_marginal_likelihood = log_marginal_likelihood
                 best_thetas = self.thetas_.copy()
                 best_spamming = self.spamming_.copy()
 
         self.thetas_ = best_thetas
         self.spamming_ = best_spamming
         _, gold_label_marginals, _, _ = self._e_step(
             annotation, task_names, worker_names, label_names, tasks, workers, labels
         )
 
         self.probas_ = decode_distribution(gold_label_marginals)
-        self.labels_ = self.probas_.idxmax(axis='columns')
-        self.labels_.index.name = 'task'
+        self.labels_ = self.probas_.idxmax(axis="columns")
+        self.labels_.index.name = "task"
 
         return self
 
-    def fit_predict(self, data: pd.DataFrame) -> pd.Series:
+    def fit_predict(self, data: pd.DataFrame) -> "pd.Series[Any]":
         """
         Fits the model to the training data and returns the aggregated results.
 
         Args:
             data (DataFrame): The training dataset of workers' labeling results
                 which is represented as the `pandas.DataFrame` data containing `task`, `worker`, and `label` columns.
 
         Returns:
             Series: Task labels. The `pandas.Series` data is indexed by `task`
                 so that `labels.loc[task]` is the most likely true label of tasks.
         """
-        return self.fit(data).labels_
+        self.fit(data)
+        assert self.labels_ is not None, "no labels_"
+        return self.labels_
 
     def fit_predict_proba(self, data: pd.DataFrame) -> pd.DataFrame:
         """
         Fits the model to the training data and returns probability distributions of labels for each task.
 
         Args:
             data (DataFrame): The training dataset of workers' labeling results
                 which is represented as the `pandas.DataFrame` data containing `task`, `worker`, and `label` columns.
 
         Returns:
             DataFrame: Probability distributions of task labels.
                 The `pandas.DataFrame` data is indexed by `task` so that `result.loc[task, label]` is the probability that the `task` true label is equal to `label`.
-                Each probability is in he range from 0 to 1, all task probabilities must sum up to 1.
+                Each probability is in the range from 0 to 1, all task probabilities must sum up to 1.
         """
-        return self.fit(data).probas_
+        self.fit(data)
+        assert self.probas_ is not None, "no probas_"
+        return self.probas_
 
     def _initialize(self, n_workers: int, n_labels: int) -> None:
         """Initializes the MACE parameters.
 
         Args:
             n_workers (int): The number of workers.
             n_labels (int): The number of labels.
@@ -276,34 +299,33 @@
         """
 
         self.spamming_ = sps.uniform(1, 1 + self.default_noise).rvs(
             size=(n_workers, 2),
             random_state=self.random_state,
         )
         self.thetas_ = sps.uniform(1, 1 + self.default_noise).rvs(
-            size=(n_workers, n_labels),
-            random_state=self.random_state
+            size=(n_workers, n_labels), random_state=self.random_state
         )
 
         self.spamming_ = self.spamming_ / self.spamming_.sum(axis=1, keepdims=True)
         self.thetas_ = self.thetas_ / self.thetas_.sum(axis=1, keepdims=True)
 
-        if self.method == 'vb':
+        if self.method == "vb":
             self.theta_priors_ = np.empty((n_workers, 2))
             self.theta_priors_[:, 0] = self.alpha
             self.theta_priors_[:, 1] = self.beta
 
             self.strategy_priors_ = np.ones((n_workers, n_labels)) * 10.0
 
     def _e_step(
         self,
         annotation: pd.DataFrame,
-        task_names: List[Any],
-        worker_names: List[Any],
-        label_names: List[Any],
+        task_names: Union[List[Any], "pd.Index[Any]"],
+        worker_names: Union[List[Any], "pd.Index[Any]"],
+        label_names: Union[List[Any], "pd.Index[Any]"],
         tasks: NDArray[np.int64],
         workers: NDArray[np.int64],
         labels: NDArray[np.int64],
     ) -> Tuple[float, pd.DataFrame, pd.DataFrame, pd.DataFrame]:
         """Performs E-step of the MACE algorithm.
 
         Args:
@@ -324,70 +346,73 @@
             index=task_names,
             columns=label_names,
         )
 
         knowing_expected_counts = pd.DataFrame(
             np.zeros((len(worker_names), 2)),
             index=worker_names,
-            columns=['knowing_expected_count_0', 'knowing_expected_count_1'],
+            columns=["knowing_expected_count_0", "knowing_expected_count_1"],
         )
 
         for label_idx, label in enumerate(label_names):
-            annotation['gold_marginal'] = self.spamming_[workers, 0] * self.thetas_[
+            annotation["gold_marginal"] = self.spamming_[workers, 0] * self.thetas_[
                 workers, labels
             ] + self.spamming_[workers, 1] * (label_idx == labels)
-            gold_label_marginals[label] = annotation.groupby('task').prod(numeric_only=True)[
-                'gold_marginal'
-            ] / len(label_names)
+            gold_label_marginals[label] = annotation.groupby("task").prod(
+                numeric_only=True
+            )["gold_marginal"] / len(label_names)
 
         instance_marginals = gold_label_marginals.sum(axis=1)
         log_marginal_likelihood = np.log(instance_marginals + 1e-8).sum()
 
-        annotation['strategy_marginal'] = 0.0
+        annotation["strategy_marginal"] = 0.0
         for label in range(len(label_names)):
-            annotation['strategy_marginal'] += gold_label_marginals.values[
+            annotation["strategy_marginal"] += gold_label_marginals.values[
                 tasks, label
             ] / (
                 self.spamming_[workers, 0] * self.thetas_[workers, labels]
                 + self.spamming_[workers, 1] * (labels == label)
             )
 
-        annotation['strategy_marginal'] = (
-            annotation['strategy_marginal']
+        annotation["strategy_marginal"] = (
+            annotation["strategy_marginal"]
             * self.spamming_[workers, 0]
             * self.thetas_[workers, labels]
         )
 
-        annotation.set_index('task', inplace=True)
-        annotation['instance_marginal'] = instance_marginals
+        annotation.set_index("task", inplace=True)
+        annotation["instance_marginal"] = instance_marginals
         annotation.reset_index(inplace=True)
 
-        annotation['strategy_marginal'] = (
-            annotation['strategy_marginal'] / annotation['instance_marginal']
+        annotation["strategy_marginal"] = (
+            annotation["strategy_marginal"] / annotation["instance_marginal"]
         )
 
         strategy_expected_counts = (
-            annotation.groupby(['worker', 'label']).sum(numeric_only=True)['strategy_marginal'].unstack().fillna(0.0)
+            annotation.groupby(["worker", "label"])
+            .sum(numeric_only=True)["strategy_marginal"]
+            .unstack()
+            .fillna(0.0)
         )
 
-        knowing_expected_counts['knowing_expected_count_0'] = annotation.groupby(
-            'worker'
-        ).sum(numeric_only=True)['strategy_marginal']
+        knowing_expected_counts["knowing_expected_count_0"] = annotation.groupby(
+            "worker"
+        ).sum(numeric_only=True)["strategy_marginal"]
 
-        annotation['knowing_expected_counts'] = (
+        annotation["knowing_expected_counts"] = (
             gold_label_marginals.values[tasks, labels].ravel()
             * self.spamming_[workers, 1]
             / (
                 self.spamming_[workers, 0] * self.thetas_[workers, labels]
                 + self.spamming_[workers, 1]
             )
         ) / instance_marginals.values[tasks]
-        knowing_expected_counts['knowing_expected_count_1'] = annotation.groupby(
-            'worker'
-        ).sum(numeric_only=True)['knowing_expected_counts']
+        knowing_expected_counts["knowing_expected_count_1"] = annotation.groupby(
+            "worker"
+        ).sum(numeric_only=True)["knowing_expected_counts"]
 
         return (
             log_marginal_likelihood,
             gold_label_marginals,
             strategy_expected_counts,
             knowing_expected_counts,
         )
```

### Comparing `crowd-kit-1.2.1/crowdkit/aggregation/classification/majority_vote.py` & `crowd-kit-1.3.0rc1/crowdkit/aggregation/classification/majority_vote.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,22 @@
-__all__ = ['MajorityVote']
+__all__ = ["MajorityVote"]
 
-from typing import Optional
+from typing import Any, Optional
 
 import attr
 import pandas as pd
 
 from ..base import BaseClassificationAggregator
-from ..utils import normalize_rows, get_most_probable_labels, get_accuracy, add_skills_to_data, named_series_attrib
+from ..utils import (
+    add_skills_to_data,
+    get_accuracy,
+    get_most_probable_labels,
+    named_series_attrib,
+    normalize_rows,
+)
 
 
 @attr.s
 class MajorityVote(BaseClassificationAggregator):
     r"""The **Majority Vote** aggregation algorithm is a straightforward approach for categorical aggregation: for each task,
     it outputs a label with the largest number of responses. Additionaly, the Majority Vote
     can be used when different weights are assigned to workers' votes. In this case, the
@@ -20,17 +26,14 @@
     {% note info %}
 
      If two or more labels have the largest number of votes, the resulting
      label will be the same for all tasks that have the same set of labels with the same number of votes.
 
      {% endnote %}
 
-    Args:
-        default_skill: Default worker weight value.
-
     Examples:
         Basic Majority Vote:
         >>> from crowdkit.aggregation import MajorityVote
         >>> from crowdkit.datasets import load_dataset
         >>> df, gt = load_dataset('relevance-2')
         >>> result = MajorityVote().fit_predict(df)
 
@@ -45,98 +48,103 @@
         >>>         ['t2', 'p1', 1],
         >>>         ['t2', 'p2', 0],
         >>>         ['t2', 'p3', 1],
         >>>     ],
         >>>     columns=['task', 'worker', 'label']
         >>> )
         >>> skills = pd.Series({'p1': 0.5, 'p2': 0.7, 'p3': 0.4})
-        >>> result = MajorityVote.fit_predict(df, skills)
-
-    Attributes:
-        labels_ (typing.Optional[pandas.core.series.Series]): The task labels. The `pandas.Series` data is indexed by `task`
-            so that `labels.loc[task]` is the most likely true label of tasks.
-
-        skills_ (typing.Optional[pandas.core.series.Series]): The workers' skills. The `pandas.Series` data is indexed by `worker`
-            and has the corresponding worker skill.
-
-        probas_ (typing.Optional[pandas.core.frame.DataFrame]): The probability distributions of task labels.
-            The `pandas.DataFrame` data is indexed by `task` so that `result.loc[task, label]` is the probability that the `task` true label is equal to `label`.
-            Each probability is in the range from 0 to 1, all task probabilities must sum up to 1.
-
-        on_missing_skill (str): A value which specifies how to handle assignments performed by workers with an unknown skill.
-
-            Possible values:
-                    * "error" — raises an exception if there is at least one assignment performed by a worker with an unknown skill;
-                    * "ignore" — drops assignments performed by workers with an unknown skill during prediction. Raises an exception if there are no
-                    assignments with a known skill for any task;
-                    * value — the default value will be used if a skill is missing.
+        >>> result = MajorityVote().fit_predict(df, skills)
     """
 
-    # TODO: remove skills_
-    skills_: Optional[pd.Series] = named_series_attrib(name='skill')
-    probas_: Optional[pd.DataFrame] = attr.ib(init=False)
-    # labels_
-    on_missing_skill: str = attr.ib(default='error')
     default_skill: Optional[float] = attr.ib(default=None)
+    """Default worker weight value."""
+
+    skills_: Optional["pd.Series[Any]"] = named_series_attrib(name="skill")
+    """The workers' skills. The `pandas.Series` data is indexed by `worker` and has the corresponding worker skill."""
 
-    def fit(self, data: pd.DataFrame, skills: pd.Series = None) -> 'MajorityVote':
+    probas_: Optional[pd.DataFrame] = attr.ib(init=False)
+    """The probability distributions of task labels. The `pandas.DataFrame` data is indexed by `task`
+    so that `result.loc[task, label]` is the probability that the `task` true label is equal to `label`.
+    Each probability is in the range from 0 to 1, all task probabilities must sum up to 1."""
+
+    on_missing_skill: str = attr.ib(default="error")
+    """A value which specifies how to handle assignments performed by workers with an unknown skill.
+
+    Possible values:
+    * `error`: raises an exception if there is at least one assignment performed by a worker with an unknown skill;
+    * `ignore`: drops assignments performed by workers with an unknown skill during prediction,
+    raises an exception if there are no assignments with a known skill for any task;
+    * `value`: the default value will be used if a skill is missing."""
+
+    def fit(
+        self, data: pd.DataFrame, skills: Optional["pd.Series[Any]"] = None
+    ) -> "MajorityVote":
         """Fits the model to the training data.
 
         Args:
             data (DataFrame): The training dataset of workers' labeling results
                 which is represented as the `pandas.DataFrame` data containing `task`, `worker`, and `label` columns.
 
-            skills (Series): The workers' skills. The `pandas.Series` data is indexed by `worker
+            skills (Series): The workers' skills. The `pandas.Series` data is indexed by `worker`
                 and has the corresponding worker skill.
 
         Returns:
             MajorityVote: self.
         """
 
-        data = data[['task', 'worker', 'label']]
+        data = data[["task", "worker", "label"]]
 
         if skills is None:
-            scores = data[['task', 'label']].value_counts()
+            scores = data[["task", "label"]].value_counts()
         else:
-            data = add_skills_to_data(data, skills, self.on_missing_skill, self.default_skill)
-            scores = data.groupby(['task', 'label'])['skill'].sum()
+            data = add_skills_to_data(
+                data, skills, self.on_missing_skill, self.default_skill
+            )
+            scores = data.groupby(["task", "label"])["skill"].sum()
 
-        self.probas_ = normalize_rows(scores.unstack('label', fill_value=0))
+        self.probas_ = normalize_rows(scores.unstack("label", fill_value=0))
         self.labels_ = get_most_probable_labels(self.probas_)
-        self.skills_ = get_accuracy(data, self.labels_, by='worker')
+        self.skills_ = get_accuracy(data, self.labels_, by="worker")
 
         return self
 
-    def fit_predict_proba(self, data: pd.DataFrame, skills: Optional[pd.Series] = None) -> pd.DataFrame:
+    def fit_predict_proba(
+        self, data: pd.DataFrame, skills: Optional["pd.Series[Any]"] = None
+    ) -> pd.DataFrame:
         """Fits the model to the training data and returns probability distributions of labels for each task.
 
         Args:
             data (DataFrame): The training dataset of workers' labeling results
                 which is represented as the `pandas.DataFrame` data containing `task`, `worker`, and `label` columns.
 
             skills (Series): The workers' skills. The `pandas.Series` data is indexed by `worker`
                 and has the corresponding worker skill.
 
         Returns:
             DataFrame: The probability distributions of task labels.
                 The `pandas.DataFrame` data is indexed by `task` so that `result.loc[task, label]` is the probability that the `task` true label is equal to `label`.
                 Each probability is in the range from 0 to 1, all task probabilities must sum up to 1.
         """
-
-        return self.fit(data, skills).probas_
-
-    def fit_predict(self, data: pd.DataFrame, skills: pd.Series = None) -> pd.Series:
+        self.fit(data, skills)
+        assert self.probas_ is not None, "no probas_"
+        return self.probas_
+
+    def fit_predict(
+        self, data: pd.DataFrame, skills: Optional["pd.Series[Any]"] = None
+    ) -> "pd.Series[Any]":
         """Fits the model to the training data and returns the aggregated results.
 
-         Args:
-            data (DataFrame): The training dataset of workers' labeling results
-                which is represented as the `pandas.DataFrame` data containing `task`, `worker`, and `label` columns.
+        Args:
+           data (DataFrame): The training dataset of workers' labeling results
+               which is represented as the `pandas.DataFrame` data containing `task`, `worker`, and `label` columns.
 
-            skills (Series): The workers' skills. The `pandas.Series` data is indexed by `worker`
-                and has the corresponding worker skill.
+           skills (Series): The workers' skills. The `pandas.Series` data is indexed by `worker`
+               and has the corresponding worker skill.
 
-         Returns:
-            Series: The task labels. The `pandas.Series` data is indexed by `task`
-                so that `labels.loc[task]` is the most likely true label of tasks.
-         """
+        Returns:
+           Series: The task labels. The `pandas.Series` data is indexed by `task`
+               so that `labels.loc[task]` is the most likely true label of tasks.
+        """
 
-        return self.fit(data, skills).labels_
+        self.fit(data, skills)
+        assert self.labels_ is not None, "no labels_"
+        return self.labels_
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `crowd-kit-1.2.1/crowdkit/aggregation/classification/wawa.py` & `crowd-kit-1.3.0rc1/crowdkit/aggregation/classification/wawa.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,104 +1,103 @@
-__all__ = ['Wawa']
+__all__ = ["Wawa"]
 
-from typing import Optional
+from typing import Any, Optional
 
 import attr
 import pandas as pd
 from sklearn.utils.validation import check_is_fitted
 
-from .majority_vote import MajorityVote
 from ..base import BaseClassificationAggregator
 from ..utils import get_accuracy, named_series_attrib
+from .majority_vote import MajorityVote
 
 
 @attr.s
 class Wawa(BaseClassificationAggregator):
     r"""The **Worker Agreement with Aggregate** (Wawa) algorithm consists of three steps:
-        1. calculates the majority vote label;
-        2. estimates workers' skills as a fraction of responses that are equal to the majority vote;
-        3. calculates the weigthed majority vote based on skills from the previous step.
-
-        Examples:
-            >>> from crowdkit.aggregation import Wawa
-            >>> from crowdkit.datasets import load_dataset
-            >>> df, gt = load_dataset('relevance-2')
-            >>> result = Wawa().fit_predict(df)
-
-        Attributes:
-            labels_ (typing.Optional[pandas.core.series.Series]): The task labels. The `pandas.Series` data is indexed by `task`
-                so that `labels.loc[task]` is the most likely true label of tasks.
-
-            skills_ (typing.Optional[pandas.core.series.Series]): The workers' skills. The `pandas.Series` data is indexed by `worker`
-                and has the corresponding worker skill.
-
-            probas_ (typing.Optional[pandas.core.frame.DataFrame]): The probability distributions of task labels.
-                The `pandas.DataFrame` data is indexed by `task` so that `result.loc[task, label]` is the probability that the `task` true label is equal to `label`.
-                Each probability is in the range from 0 to 1, all task probabilities must sum up to 1.
-        """
+    1. calculates the majority vote label;
+    2. estimates workers' skills as a fraction of responses that are equal to the majority vote;
+    3. calculates the weigthed majority vote based on skills from the previous step.
+
+    Examples:
+        >>> from crowdkit.aggregation import Wawa
+        >>> from crowdkit.datasets import load_dataset
+        >>> df, gt = load_dataset('relevance-2')
+        >>> result = Wawa().fit_predict(df)
+    """
+
+    skills_: Optional["pd.Series[Any]"] = named_series_attrib(name="skill")
+    """The workers' skills.
+    The `pandas.Series` data is indexed by `worker` and has the corresponding worker skill."""
 
-    skills_: Optional[pd.Series] = named_series_attrib(name='skill')
     probas_: Optional[pd.DataFrame] = attr.ib(init=False)
+    """The probability distributions of task labels.
+    The `pandas.DataFrame` data is indexed by `task` so that `result.loc[task, label]` is the probability that
+    the `task` true label is equal to `label`. Each probability is in the range from 0 to 1,
+    all task probabilities must sum up to 1."""
 
-    # labels_
-
-    def _apply(self, data: pd.DataFrame) -> 'Wawa':
-        check_is_fitted(self, attributes='skills_')
+    def _apply(self, data: pd.DataFrame) -> "Wawa":
+        check_is_fitted(self, attributes="skills_")
         mv = MajorityVote().fit(data, skills=self.skills_)
         self.probas_ = mv.probas_
         self.labels_ = mv.labels_
         return self
 
-    def fit(self, data: pd.DataFrame) -> 'Wawa':
+    def fit(self, data: pd.DataFrame) -> "Wawa":
         """Fits the model to the training data.
 
         Args:
             data (DataFrame): The training dataset of workers' labeling results
                 which is represented as the `pandas.DataFrame` data containing `task`, `worker`, and `label` columns.
 
         Returns:
             Wawa: self.
         """
 
         # TODO: support weights?
-        data = data[['task', 'worker', 'label']]
+        data = data[["task", "worker", "label"]]
         mv = MajorityVote().fit(data)
-        self.skills_ = get_accuracy(data, true_labels=mv.labels_, by='worker')
+        assert mv.labels_ is not None, "no labels_"
+        self.skills_ = get_accuracy(data, true_labels=mv.labels_, by="worker")
         return self
 
-    def predict(self, data: pd.DataFrame) -> pd.Series:
+    def predict(self, data: pd.DataFrame) -> "pd.Series[Any]":
         """Predicts the true labels of tasks when the model is fitted.
 
         Args:
             data (DataFrame): The training dataset of workers' labeling results
                 which is represented as the `pandas.DataFrame` data containing `task`, `worker`, and `label` columns.
 
         Returns:
             Series: The task labels. The `pandas.Series` data is indexed by `task`
                 so that `labels.loc[task]` is the most likely true label of tasks.
         """
 
-        return self._apply(data).labels_
+        self._apply(data)
+        assert self.labels_ is not None, "no labels_"
+        return self.labels_
 
     def predict_proba(self, data: pd.DataFrame) -> pd.DataFrame:
         """Returns probability distributions of labels for each task when the model is fitted.
 
         Args:
             data (DataFrame): The training dataset of workers' labeling results
                 which is represented as the `pandas.DataFrame` data containing `task`, `worker`, and `label` columns.
 
         Returns:
             DataFrame: Probability distributions of task labels.
                 The `pandas.DataFrame` data is indexed by `task` so that `result.loc[task, label]` is the probability that the `task` true label is equal to `label`.
-                Each probability is in he range from 0 to 1, all task probabilities must sum up to 1.
+                Each probability is in the range from 0 to 1, all task probabilities must sum up to 1.
         """
 
-        return self._apply(data).probas_
+        self._apply(data)
+        assert self.probas_ is not None, "no probas_"
+        return self.probas_
 
-    def fit_predict(self, data: pd.DataFrame) -> pd.Series:
+    def fit_predict(self, data: pd.DataFrame) -> "pd.Series[Any]":
         """Fits the model to the training data and returns the aggregated results.
 
         Args:
             data (DataFrame): The training dataset of workers' labeling results
                 which is represented as the `pandas.DataFrame` data containing `task`, `worker`, and `label` columns.
 
         Returns:
@@ -114,11 +113,11 @@
         Args:
             data (DataFrame): The training dataset of workers' labeling results
                 which is represented as the `pandas.DataFrame` data containing `task`, `worker`, and `label` columns.
 
         Returns:
             DataFrame: Probability distributions of task labels.
                 The `pandas.DataFrame` data is indexed by `task` so that `result.loc[task, label]` is the probability that the `task` true label is equal to `label`.
-                Each probability is in he range from 0 to 1, all task probabilities must sum up to 1.
+                Each probability is in the range from 0 to 1, all task probabilities must sum up to 1.
         """
 
         return self.fit(data).predict_proba(data)
```

### Comparing `crowd-kit-1.2.1/crowdkit/aggregation/classification/zero_based_skill.py` & `crowd-kit-1.3.0rc1/crowdkit/aggregation/classification/zero_based_skill.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-__all__ = ['ZeroBasedSkill']
+__all__ = ["ZeroBasedSkill"]
 
-from typing import Optional
+from typing import Any, Optional
 
 import attr
 import pandas as pd
 from sklearn.utils.validation import check_is_fitted
 
-from .majority_vote import MajorityVote
 from ..base import BaseClassificationAggregator
 from ..utils import get_accuracy, named_series_attrib
+from .majority_vote import MajorityVote
 
 
 @attr.attrs(auto_attribs=True)
 class ZeroBasedSkill(BaseClassificationAggregator):
     r"""The **Zero-Based Skill** (ZBS) aggregation model performs weighted majority voting on tasks. After processing a pool of tasks,
     it re-estimates the workers' skills with a gradient descend step to optimize
     the mean squared error of the current skills and the fraction of responses that
@@ -23,135 +23,136 @@
     {% note info %}
 
     It is necessary that all workers in the dataset that is sent to `predict` exist in responses to
     the dataset that was sent to `fit`.
 
     {% endnote %}
 
-    Args:
-        n_iter: The maximum number of iterations.
-        lr_init: The initial learning rate.
-        lr_steps_to_reduce: The number of steps required to reduce the learning rate.
-        lr_reduce_factor: The factor by which the learning rate will be multiplied every `lr_steps_to_reduce` step.
-        eps: The convergence threshold.
-
     Examples:
         >>> from crowdkit.aggregation import ZeroBasedSkill
         >>> from crowdkit.datasets import load_dataset
         >>> df, gt = load_dataset('relevance-2')
         >>> result = ZeroBasedSkill().fit_predict(df)
-
-    Attributes:
-        skills_ (typing.Optional[pandas.core.series.Series]): The workers' skills. The `pandas.Series` data is indexed by `worker`
-            and has the corresponding worker skill.
-
-        labels_ (typing.Optional[pandas.core.series.Series]): The task labels. The `pandas.Series` data is indexed by `task`
-            so that `labels.loc[task]` is the most likely true label of tasks.
-
-        probas_ (typing.Optional[pandas.core.frame.DataFrame]): The probability distributions of task labels.
-            The `pandas.DataFrame` data is indexed by `task` so that `result.loc[task, label]` is the probability that the `task` true label is equal to `label`.
-            Each probability is in the range from 0 to 1, all task probabilities must sum up to 1.
     """
 
     n_iter: int = 100
+    """The maximum number of iterations."""
+
     lr_init: float = 1.0
+    """The initial learning rate."""
+
     lr_steps_to_reduce: int = 20
+    """The number of steps required to reduce the learning rate."""
+
     lr_reduce_factor: float = 0.5
+    """The factor by which the learning rate will be multiplied every `lr_steps_to_reduce` step."""
+
     eps: float = 1e-5
+    """The convergence threshold."""
 
-    # Available after fit
-    skills_: Optional[pd.Series] = named_series_attrib(name='skill')
+    skills_: Optional["pd.Series[Any]"] = named_series_attrib(name="skill")
+    """The workers' skills.
+    The `pandas.Series` data is indexed by `worker` and has the corresponding worker skill."""
 
-    # Available after predict or predict_proba
-    # labels_
     probas_: Optional[pd.DataFrame] = attr.ib(init=False)
+    """The probability distributions of task labels.
+    The `pandas.DataFrame` data is indexed by `task` so that `result.loc[task, label]` is the probability that
+    the `task` true label is equal to `label`. Each probability is in the range from 0 to 1,
+    all task probabilities must sum up to 1."""
 
-    def _init_skills(self, data: pd.DataFrame) -> pd.Series:
+    def _init_skills(self, data: pd.DataFrame) -> "pd.Series[Any]":
         skill_value = 1 / data.label.unique().size + self.eps
-        skill_index = pd.Index(data.worker.unique(), name='worker')
+        skill_index = pd.Index(data.worker.unique(), name="worker")
         return pd.Series(skill_value, index=skill_index)
 
-    def _apply(self, data: pd.DataFrame) -> 'ZeroBasedSkill':
-        check_is_fitted(self, attributes='skills_')
+    def _apply(self, data: pd.DataFrame) -> "ZeroBasedSkill":
+        check_is_fitted(self, attributes="skills_")
         mv = MajorityVote().fit(data, self.skills_)
         self.labels_ = mv.labels_
         self.probas_ = mv.probas_
         return self
 
-    def fit(self, data: pd.DataFrame) -> 'ZeroBasedSkill':
+    def fit(self, data: pd.DataFrame) -> "ZeroBasedSkill":
         """Fits the model to the training data.
 
         Args:
             data (DataFrame): The training dataset of workers' labeling results
                 which is represented as the `pandas.DataFrame` data containing `task`, `worker`, and `label` columns.
 
         Returns:
             ZeroBasedSkill: self.
         """
 
         # Initialization
-        data = data[['task', 'worker', 'label']]
+        data = data[["task", "worker", "label"]]
         skills = self._init_skills(data)
         mv = MajorityVote()
 
         # Updating skills and re-fitting majority vote n_iter times
         learning_rate = self.lr_init
         for iteration in range(1, self.n_iter + 1):
             if iteration % self.lr_steps_to_reduce == 0:
                 learning_rate *= self.lr_reduce_factor
             mv.fit(data, skills=skills)
-            skills = skills + learning_rate * (get_accuracy(data, mv.labels_, by='worker') - skills)
+            assert mv.labels_ is not None, "no labels_"
+            skills = skills + learning_rate * (
+                get_accuracy(data, mv.labels_, by="worker") - skills
+            )
 
         # Saving results
         self.skills_ = skills
 
         return self
 
-    def predict(self, data: pd.DataFrame) -> pd.Series:
+    def predict(self, data: pd.DataFrame) -> "pd.Series[Any]":
         """Predicts the true labels of tasks when the model is fitted.
 
         Args:
             data (DataFrame): The training dataset of workers' labeling results
                 which is represented as the `pandas.DataFrame` data containing `task`, `worker`, and `label` columns.
 
         Returns:
             Series: The task labels. The `pandas.Series` data is indexed by `task`
                 so that `labels.loc[task]` is the most likely true label of tasks.
         """
 
-        return self._apply(data).labels_
+        self._apply(data)
+        assert self.labels_ is not None, "no labels_"
+        return self.labels_
 
     def predict_proba(self, data: pd.DataFrame) -> pd.DataFrame:
         """Returns probability distributions of labels for each task when the model is fitted.
 
         Args:
             data (DataFrame): The training dataset of workers' labeling results
                 which is represented as the `pandas.DataFrame` data containing `task`, `worker`, and `label` columns.
 
         Returns:
             DataFrame: The probability distributions of task labels.
                 The `pandas.DataFrame` data is indexed by `task` so that `result.loc[task, label]` is the probability that the `task` true label is equal to `label`.
                 Each probability is in the range from 0 to 1, all task probabilities must sum up to 1.
         """
 
-        return self._apply(data).probas_
+        self._apply(data)
+        assert self.probas_ is not None, "no probas_"
+        return self.probas_
 
-    def fit_predict(self, data: pd.DataFrame) -> pd.Series:
+    def fit_predict(self, data: pd.DataFrame) -> "pd.Series[Any]":
         """Fits the model to the training data and returns the aggregated results.
         Args:
             data (DataFrame): The training dataset of workers' labeling results
                 which is represented as the `pandas.DataFrame` data containing `task`, `worker`, and `label` columns.
         Returns:
             Series: The task labels. The `pandas.Series` data is indexed by `task`
                 so that `labels.loc[task]` is the most likely true label of tasks.
         """
 
         return self.fit(data).predict(data)
 
-    def fit_predict_proba(self, data: pd.DataFrame) -> pd.Series:
+    def fit_predict_proba(self, data: pd.DataFrame) -> pd.DataFrame:
         """Fits the model to the training data and returns the aggregated results.
         Args:
             data (DataFrame): The training dataset of workers' labeling results
                 which is represented as the `pandas.DataFrame` data containing `task`, `worker`, and `label` columns.
         Returns:
             Series: The task labels. The `pandas.Series` data is indexed by `task`
                 so that `labels.loc[task]` is the most likely true label of tasks.
```

### Comparing `crowd-kit-1.2.1/crowdkit/aggregation/embeddings/closest_to_average.py` & `crowd-kit-1.3.0rc1/crowdkit/aggregation/embeddings/closest_to_average.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-__all__ = ['ClosestToAverage']
+__all__ = ["ClosestToAverage"]
 
-from typing import Callable, Optional, Any
+from typing import Any, Callable, Optional
 
 import attr
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
 
 from ..base import BaseEmbeddingsAggregator
@@ -14,35 +14,32 @@
 class ClosestToAverage(BaseEmbeddingsAggregator):
     """The **Closest to Average** aggregation model chooses the output with the embedding that's closest to the average embedding.
 
     This method takes a `DataFrame` containing four columns: `task`, `worker`, `output`, and `embedding`.
     Here the `embedding` is a vector containing a representation of the `output` which might be any
     type of data such as text, images, NumPy arrays, etc. As a result, the method returns the output which
     embedding is the closest one to the average embedding of the task responses.
-
-    Args:
-        distance: A callable that takes two NumPy arrays (the task embedding and the aggregated embedding) and returns a single `float` number — the distance
-            between these two vectors.
-
-    Attributes:
-        embeddings_and_outputs_ (DataFrame): The task embeddings and outputs.
-            The `pandas.DataFrame` data is indexed by `task` and has the `embedding` and `output` columns.
-
-        scores_ (DataFrame): The task label scores.
-            The `pandas.DataFrame` data is indexed by `task` so that `result.loc[task, label]`
-            is a score of `label` for `task`.
     """
 
-    # embeddings_and_outputs_
-    scores_: pd.DataFrame
-
     distance: Callable[[npt.NDArray[Any], npt.NDArray[Any]], float] = attr.ib()
+    """A callable that takes two NumPy arrays (the task embedding and the aggregated embedding)
+    and returns a single `float` number: the distance between these two vectors."""
+
+    embeddings_and_outputs_: pd.DataFrame = attr.ib(init=False)
+    """The task embeddings and outputs. The `pandas.DataFrame` data is indexed by `task` and has the `embedding` and `output` columns."""
+
+    scores_: pd.DataFrame = attr.ib(init=False)
+    """The task label scores. The `pandas.DataFrame` data is indexed by `task` so that `result.loc[task, label]` is a score of `label` for `task`."""
 
-    def fit(self, data: pd.DataFrame, aggregated_embeddings: Optional[pd.Series] = None,
-            true_embeddings: pd.Series = None) -> 'ClosestToAverage':
+    def fit(
+        self,
+        data: pd.DataFrame,
+        aggregated_embeddings: Optional["pd.Series[Any]"] = None,
+        true_embeddings: Optional["pd.Series[Any]"] = None,
+    ) -> "ClosestToAverage":
         """Fits the model to the training data.
 
         Args:
             data (DataFrame): The workers' outputs with their embeddings.
                 The `pandas.DataFrame` data contains the `task`, `worker`, `output`, and `embedding` columns.
             aggregated_embeddings (Series): The task aggregated embeddings.
                 The `pandas.Series` data is indexed by `task` and contains the corresponding aggregated embeddings.
@@ -52,44 +49,52 @@
 
         Returns:
             ClosestToAverage: self.
         """
 
         if true_embeddings is not None and not true_embeddings.index.is_unique:
             raise ValueError(
-                'Incorrect data in true_embeddings: multiple true embeddings for a single task are not supported.'
+                "Incorrect data in true_embeddings: multiple true embeddings for a single task are not supported."
             )
 
-        data = data[['task', 'worker', 'output', 'embedding']]
+        data = data[["task", "worker", "output", "embedding"]]
         if aggregated_embeddings is None:
-            group = data.groupby('task')
+            group = data.groupby("task")
             # we don't use .mean() because it does not work with np.array in older pandas versions
             avg_embeddings = group.embedding.apply(np.sum) / group.worker.count()
-            avg_embeddings.update(true_embeddings)
+            avg_embeddings.update(true_embeddings)  # type: ignore
         else:
             avg_embeddings = aggregated_embeddings
 
         # Calculating distances (scores)
-        data = data.join(avg_embeddings.rename('avg_embedding'), on='task')
+        data = data.join(avg_embeddings.rename("avg_embedding"), on="task")
         # TODO: native Python functions are slow
-        data['score'] = data.apply(lambda row: self.distance(row.embedding, row.avg_embedding), axis=1)
+        data["score"] = data.apply(
+            lambda row: self.distance(row.embedding, row.avg_embedding), axis=1
+        )
 
         # Selecting best scores and outputs
-        scores = data[['task', 'output', 'score', 'embedding']]
+        scores = data[["task", "output", "score", "embedding"]]
         # TODO: process cases when we actually have an answer in true_embeddings
         # TODO: to do that we must make true_embeddings a DataFrame with `output` column
-        embeddings_and_outputs = scores[['task', 'output', 'embedding']].loc[scores.groupby('task')['score'].idxmin()]
+        embeddings_and_outputs = scores[["task", "output", "embedding"]].loc[
+            scores.groupby("task")["score"].idxmin()
+        ]
 
         #
-        self.scores_ = scores.set_index('task')
-        self.embeddings_and_outputs_ = embeddings_and_outputs.set_index('task')
+        self.scores_ = scores.set_index("task")
+        self.embeddings_and_outputs_ = embeddings_and_outputs.set_index("task")
 
         return self
 
-    def fit_predict_scores(self, data: pd.DataFrame, aggregated_embeddings: pd.Series = None) -> pd.DataFrame:
+    def fit_predict_scores(
+        self,
+        data: pd.DataFrame,
+        aggregated_embeddings: Optional["pd.Series[Any]"] = None,
+    ) -> pd.DataFrame:
         """Fits the model to the training data and returns the estimated scores.
 
         Args:
             data (DataFrame): The workers' outputs with their embeddings.
                 The `pandas.DataFrame` data contains the `task`, `worker`, `output`, and `embedding` columns.
             aggregated_embeddings (Series): The task aggregated embeddings.
                 The `pandas.Series` data is indexed by `task` and contains the corresponding aggregated embeddings.
@@ -98,15 +103,19 @@
             DataFrame: The task label scores.
                 The `pandas.DataFrame` data is indexed by `task` so that `result.loc[task, label]`
                 is a score of `label` for `task`.
         """
 
         return self.fit(data, aggregated_embeddings).scores_
 
-    def fit_predict(self, data: pd.DataFrame, aggregated_embeddings: Optional[pd.Series] = None) -> pd.DataFrame:
+    def fit_predict(
+        self,
+        data: pd.DataFrame,
+        aggregated_embeddings: Optional["pd.Series[Any]"] = None,
+    ) -> pd.DataFrame:
         """
         Fits the model to the training data and returns the aggregated outputs.
 
         Args:
             data (DataFrame): The workers' outputs with their embeddings.
                 The `pandas.DataFrame` data contains the `task`, `worker`, `output`, and `embedding` columns.
             aggregated_embeddings (Series): The task aggregated embeddings.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `crowd-kit-1.2.1/crowdkit/aggregation/embeddings/hrrasa.py` & `crowd-kit-1.3.0rc1/crowdkit/aggregation/embeddings/hrrasa.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 __all__ = [
-    'glue_similarity',
-    'HRRASA',
+    "glue_similarity",
+    "HRRASA",
 ]
 
 from functools import partial
-from typing import Any, Tuple, List, Optional, Callable, Generator
+from typing import Any, Callable, Generator, List, Optional, Tuple
 
 import attr
 import nltk.translate.gleu_score as gleu
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
 import scipy.stats as sps
 from scipy.spatial import distance
 
-from .closest_to_average import ClosestToAverage
 from ..base import BaseClassificationAggregator
+from .closest_to_average import ClosestToAverage
 
 _EPS = 1e-5
 
 
 def glue_similarity(hyp: str, ref: List[List[str]]) -> float:
     return float(gleu.sentence_gleu([hyp.split()], ref))
 
@@ -67,29 +67,14 @@
 
     Jiyi Li. Crowdsourced Text Sequence Aggregation based on Hybrid Reliability and Representation.
     In *Proceedings of the 43rd International ACM SIGIR Conference on Research and Development
     in Information Retrieval (SIGIR '20)*, China (July 25–30, 2020), 1761-1764.
 
     <https://doi.org/10.1145/3397271.3401239>
 
-    Args:
-        n_iter: The maximum number of iterations.
-        tol: The tolerance stopping criterion for iterative methods with a variable number of steps.
-            The algorithm converges when the loss change is less than the `tol` parameter.
-        lambda_emb: The weight of reliability calculated on embeddings.
-        lambda_out: The weight of reliability calculated on outputs.
-        alpha: The significance level of the chi-squared distribution quantiles in the $\beta$ parameter formula.
-        calculate_ranks: Specifies if the additional `ranks_` attribute will be calculated (true) or not (false).
-        _output_similarity: The similarity measure $sim$ of the `output` data. By default, it is equal to the GLEU similarity.
-
-    Attributes:
-        embeddings_and_outputs_ (DataFrame): The task embeddings and outputs.
-            The `pandas.DataFrame` data is indexed by `task` and has the `embedding` and `output` columns.
-        loss_history_ (List[float]): A list of loss values during training.
-
     Examples:
         >>> import numpy as np
         >>> import pandas as pd
         >>> from crowdkit.aggregation import HRRASA
         >>> df = pd.DataFrame(
         >>>     [
         >>>         ['t1', 'p1', 'a', np.array([1.0, 0.0])],
@@ -98,24 +83,47 @@
         >>>     ],
         >>>     columns=['task', 'worker', 'output', 'embedding']
         >>> )
         >>> result = HRRASA().fit_predict(df)
     """
 
     n_iter: int = attr.ib(default=100)
+    """The maximum number of iterations."""
+
     tol: float = attr.ib(default=1e-9)
+    """The tolerance stopping criterion for iterative methods with a variable number of steps.
+    The algorithm converges when the loss change is less than the `tol` parameter."""
+
     lambda_emb: float = attr.ib(default=0.5)
+    """The weight of reliability calculated on embeddings."""
+
     lambda_out: float = attr.ib(default=0.5)
+    """The weight of reliability calculated on outputs."""
+
     alpha: float = attr.ib(default=0.05)
+    """The significance level of the chi-squared distribution quantiles in the $\beta$ parameter formula."""
+
     calculate_ranks: bool = attr.ib(default=False)
-    _output_similarity: Callable[[str, List[List[str]]], float] = attr.ib(default=glue_similarity)
-    # embeddings_and_outputs_
+    """Specifies if the additional `ranks_` attribute will be calculated (true) or not (false)."""
+
+    _output_similarity: Callable[[str, List[List[str]]], float] = attr.ib(
+        default=glue_similarity
+    )
+    """The similarity measure $sim$ of the `output` data. By default, it is equal to the GLEU similarity."""
+
+    embeddings_and_outputs_: pd.DataFrame = attr.ib(init=False)
+    """The task embeddings and outputs.
+    The `pandas.DataFrame` data is indexed by `task` and has the `embedding` and `output` columns."""
+
     loss_history_: List[float] = attr.ib(init=False)
+    """A list of loss values during training."""
 
-    def fit(self, data: pd.DataFrame, true_embeddings: pd.Series = None) -> 'HRRASA':
+    def fit(
+        self, data: pd.DataFrame, true_embeddings: Optional["pd.Series[Any]"] = None
+    ) -> "HRRASA":
         """Fits the model to the training data.
 
         Args:
             data (DataFrame): The workers' outputs with their embeddings.
                 The `pandas.DataFrame` data contains the `task`, `worker`, `output`, and `embedding` columns.
             true_embeddings (Series): The embeddings of the true task responses.
                 The `pandas.Series` data is indexed by `task` and contains the corresponding embeddings.
@@ -123,37 +131,45 @@
 
         Returns:
             HRRASA: self.
         """
 
         if true_embeddings is not None and not true_embeddings.index.is_unique:
             raise ValueError(
-                'Incorrect data in true_embeddings: multiple true embeddings for a single task are not supported.'
+                "Incorrect data in true_embeddings: multiple true embeddings for a single task are not supported."
             )
 
-        data = data[['task', 'worker', 'embedding', 'output']]
+        data = data[["task", "worker", "embedding", "output"]]
         data, single_overlap_tasks = self._filter_single_overlap(data)
         data = self._get_local_skills(data)
 
-        prior_skills = data.worker.value_counts().apply(partial(sps.chi2.isf, self.alpha / 2))
+        prior_skills = data.worker.value_counts().apply(
+            partial(sps.chi2.isf, self.alpha / 2)
+        )
         skills = pd.Series(1.0, index=data.worker.unique())
         weights = self._calc_weights(data, skills)
-        aggregated_embeddings = self._aggregate_embeddings(data, weights, true_embeddings)
+        aggregated_embeddings = self._aggregate_embeddings(
+            data, weights, true_embeddings
+        )
         self.loss_history_ = []
         last_aggregated = None
 
         if len(data) > 0:
             for _ in range(self.n_iter):
-                aggregated_embeddings = self._aggregate_embeddings(data, weights, true_embeddings)
+                aggregated_embeddings = self._aggregate_embeddings(
+                    data, weights, true_embeddings
+                )
                 skills = self._update_skills(data, aggregated_embeddings, prior_skills)
                 weights = self._calc_weights(data, skills)
 
                 if last_aggregated is not None:
                     delta = aggregated_embeddings - last_aggregated
-                    loss = (delta * delta).sum().sum() / (aggregated_embeddings * aggregated_embeddings).sum().sum()
+                    loss = (delta * delta).sum().sum() / (
+                        aggregated_embeddings * aggregated_embeddings
+                    ).sum().sum()
                     self.loss_history_.append(loss)
                     if loss < self.tol:
                         break
                 last_aggregated = aggregated_embeddings
 
         self.prior_skills_ = prior_skills
         self.skills_ = skills
@@ -162,15 +178,17 @@
         if self.calculate_ranks:
             self.ranks_ = self._rank_outputs(data, skills)
 
         if len(single_overlap_tasks) > 0:
             self._fill_single_overlap_tasks_info(single_overlap_tasks)
         return self
 
-    def fit_predict_scores(self, data: pd.DataFrame, true_embeddings: pd.Series = None) -> pd.DataFrame:
+    def fit_predict_scores(
+        self, data: pd.DataFrame, true_embeddings: Optional["pd.Series[Any]"] = None
+    ) -> pd.DataFrame:
         """Fits the model to the training data and returns the estimated scores.
 
         Args:
             data (DataFrame): The workers' outputs with their embeddings.
                 The `pandas.DataFrame` data contains the `task`, `worker`, `output`, and `embedding` columns.
             true_embeddings (Series): The embeddings of the true task responses.
                 The `pandas.Series` data is indexed by `task` and contains the corresponding embeddings.
@@ -180,174 +198,228 @@
             DataFrame: The task label scores.
                 The `pandas.DataFrame` data is indexed by `task` so that `result.loc[task, label]`
                 is a score of `label` for `task`.
         """
 
         return self.fit(data, true_embeddings)._apply(data, true_embeddings).scores_
 
-    def fit_predict(self, data: pd.DataFrame, true_embeddings: Optional[pd.Series] = None) -> pd.DataFrame:
+    def fit_predict(  # type: ignore
+        self, data: pd.DataFrame, true_embeddings: Optional["pd.Series[Any]"] = None
+    ) -> pd.DataFrame:
         """Fits the model to the training data and returns the aggregated outputs.
 
         Args:
             data (DataFrame): The workers' outputs with their embeddings.
                 The `pandas.DataFrame` data contains the `task`, `worker`, `output`, and `embedding` columns.
             true_embeddings (Series): The embeddings of the true task responses.
                 The `pandas.Series` data is indexed by `task` and contains the corresponding embeddings.
                 The multiple true embeddings are not supported for a single task.
 
         Returns:
             DataFrame: The task embeddings and outputs.
                 The `pandas.DataFrame` data is indexed by `task` and has the `embedding` and `output` columns.
         """
 
-        return self.fit(data, true_embeddings)._apply(data, true_embeddings).embeddings_and_outputs_
+        return (
+            self.fit(data, true_embeddings)
+            ._apply(data, true_embeddings)
+            .embeddings_and_outputs_
+        )
 
     @staticmethod
-    def _cosine_distance(embedding: npt.NDArray[Any], avg_embedding: npt.NDArray[Any]) -> float:
+    def _cosine_distance(
+        embedding: npt.NDArray[Any], avg_embedding: npt.NDArray[Any]
+    ) -> float:
         if not embedding.any() or not avg_embedding.any():
-            return float('inf')
+            return float("inf")
         return float(distance.cosine(embedding, avg_embedding))
 
-    def _apply(self, data: pd.DataFrame, true_embeddings: pd.Series = None) -> 'HRRASA':
+    def _apply(
+        self, data: pd.DataFrame, true_embeddings: Optional["pd.Series[Any]"] = None
+    ) -> "HRRASA":
         cta = ClosestToAverage(distance=self._cosine_distance)
-        cta.fit(data, aggregated_embeddings=self.aggregated_embeddings_, true_embeddings=true_embeddings)
+        cta.fit(
+            data,
+            aggregated_embeddings=self.aggregated_embeddings_,
+            true_embeddings=true_embeddings,
+        )
         self.scores_ = cta.scores_
         self.embeddings_and_outputs_ = cta.embeddings_and_outputs_
         return self
 
     @staticmethod
-    def _aggregate_embeddings(data: pd.DataFrame, weights: pd.DataFrame,
-                              true_embeddings: Optional[pd.Series] = None) -> pd.Series:
+    def _aggregate_embeddings(
+        data: pd.DataFrame,
+        weights: pd.DataFrame,
+        true_embeddings: Optional["pd.Series[Any]"] = None,
+    ) -> "pd.Series[Any]":
         """Calculates the weighted average of embeddings for each task."""
-        data = data.join(weights, on=['task', 'worker'])
-        data['weighted_embedding'] = data.weight * data.embedding
-        group = data.groupby('task', group_keys=False)
-        aggregated_embeddings = pd.Series((group.weighted_embedding.apply(np.sum) / group.weight.sum()),
-                                          dtype=np.float64)
+        data = data.join(weights, on=["task", "worker"])
+        data["weighted_embedding"] = data.weight * data.embedding
+        group = data.groupby("task", group_keys=False)
+        aggregated_embeddings = pd.Series(
+            (group.weighted_embedding.apply(np.sum) / group.weight.sum()),
+            dtype=np.float64,
+        )
         if true_embeddings is None:
             true_embeddings = pd.Series([], dtype=np.float64)
         aggregated_embeddings.update(true_embeddings)
         return aggregated_embeddings
 
     def _distance_from_aggregated(self, answers: pd.DataFrame) -> pd.DataFrame:
-        """Calculates the square of Euclidian distance from the aggregated embedding for each answer.
-        """
-        with_task_aggregate = answers.set_index('task')
-        with_task_aggregate['task_aggregate'] = self.aggregated_embeddings_
-        with_task_aggregate['distance'] = with_task_aggregate.apply(
-            lambda row: np.sum((row['embedding'] - row['task_aggregate']) ** 2), axis=1)
-        with_task_aggregate['distance'] = with_task_aggregate['distance'].replace({0.0: 1e-5})  # avoid division by zero
+        """Calculates the square of Euclidian distance from the aggregated embedding for each answer."""
+        with_task_aggregate = answers.set_index("task")
+        with_task_aggregate["task_aggregate"] = self.aggregated_embeddings_
+        with_task_aggregate["distance"] = with_task_aggregate.apply(
+            lambda row: np.sum((row["embedding"] - row["task_aggregate"]) ** 2), axis=1
+        )
+        with_task_aggregate["distance"] = with_task_aggregate["distance"].replace(
+            {0.0: 1e-5}
+        )  # avoid division by zero
         return with_task_aggregate.reset_index()
 
-    def _rank_outputs(self, data: pd.DataFrame, skills: pd.Series) -> pd.DataFrame:
-        """Returns the ranking score for each record in the `data` data frame.
-        """
+    def _rank_outputs(
+        self, data: pd.DataFrame, skills: "pd.Series[Any]"
+    ) -> pd.DataFrame:
+        """Returns the ranking score for each record in the `data` data frame."""
 
         if not data.size:
-            return pd.DataFrame(columns=['task', 'output', 'rank'])
+            return pd.DataFrame(columns=["task", "output", "rank"])
 
         data = self._distance_from_aggregated(data)
-        data['norms_prod'] = data.apply(lambda row: np.sum(row['embedding'] ** 2) * np.sum(row['task_aggregate'] ** 2),
-                                        axis=1)
-        data['rank'] = skills * np.exp(-data.distance / data.norms_prod) + data.local_skill
-        return data[['task', 'output', 'rank']]
+        data["norms_prod"] = data.apply(
+            lambda row: np.sum(row["embedding"] ** 2)
+            * np.sum(row["task_aggregate"] ** 2),
+            axis=1,
+        )
+        data["rank"] = (
+            skills * np.exp(-data.distance / data.norms_prod) + data.local_skill
+        )
+        return data[["task", "output", "rank"]]
 
     @staticmethod
-    def _calc_weights(data: pd.DataFrame, worker_skills: pd.Series) -> pd.DataFrame:
-        """Calculates the weight for every embedding according to its local and global skills.
-        """
-        data = data.set_index('worker')
-        data['worker_skill'] = worker_skills
+    def _calc_weights(
+        data: pd.DataFrame, worker_skills: "pd.Series[Any]"
+    ) -> pd.DataFrame:
+        """Calculates the weight for every embedding according to its local and global skills."""
+        data = data.set_index("worker")
+        data["worker_skill"] = worker_skills
         data = data.reset_index()
-        data['weight'] = data['worker_skill'] * data['local_skill']
-        return data[['task', 'worker', 'weight']].set_index(['task', 'worker'])
+        data["weight"] = data["worker_skill"] * data["local_skill"]
+        return data[["task", "worker", "weight"]].set_index(["task", "worker"])
 
     @staticmethod
-    def _update_skills(data: pd.DataFrame, aggregated_embeddings: pd.Series, prior_skills: pd.Series) -> pd.Series:
+    def _update_skills(
+        data: pd.DataFrame,
+        aggregated_embeddings: "pd.Series[Any]",
+        prior_skills: "pd.Series[Any]",
+    ) -> "pd.Series[Any]":
         """Estimates the global reliabilities by aggregated embeddings."""
-        data = data.join(aggregated_embeddings.rename('aggregated_embedding'), on='task')
-        data['distance'] = ((data.embedding - data.aggregated_embedding) ** 2).apply(np.sum)
-        data['distance'] = data['distance'] / data['local_skill']
-        total_distances = data.groupby('worker').distance.apply(np.sum)
+        data = data.join(
+            aggregated_embeddings.rename("aggregated_embedding"), on="task"
+        )
+        data["distance"] = ((data.embedding - data.aggregated_embedding) ** 2).apply(
+            np.sum
+        )
+        data["distance"] = data["distance"] / data["local_skill"]
+        total_distances = data.groupby("worker").distance.apply(np.sum)
         total_distances.clip(lower=_EPS, inplace=True)
         return prior_skills / total_distances
 
     def _get_local_skills(self, data: pd.DataFrame) -> pd.DataFrame:
-        """Computes the local (relative) skills for each task answer.
-        """
+        """Computes the local (relative) skills for each task answer."""
         index = []
         local_skills = []
         processed_pairs = set()
-        for task, task_answers in data.groupby('task'):
+        for task, task_answers in data.groupby("task"):
             for worker, skill in self._local_skills_on_task(task_answers):
                 if (task, worker) not in processed_pairs:
                     local_skills.append(skill)
                     index.append((task, worker))
                     processed_pairs.add((task, worker))
-        data = data.set_index(['task', 'worker'])
-        local_skills = pd.Series(local_skills, index=pd.MultiIndex.from_tuples(index, names=['task', 'worker']),
-                                 dtype=float)
-        data['local_skill'] = local_skills
+        data = data.set_index(["task", "worker"])
+        local_skills = pd.Series(  # type: ignore
+            local_skills,
+            index=pd.MultiIndex.from_tuples(index, names=["task", "worker"]),
+            dtype=float,
+        )
+        data["local_skill"] = local_skills
         return data.reset_index()
 
-    def _local_skills_on_task(self, task_answers: pd.DataFrame) -> Generator[Tuple[Any, float], None, None]:
+    def _local_skills_on_task(
+        self, task_answers: pd.DataFrame
+    ) -> Generator[Tuple[Any, float], None, None]:
         overlap = len(task_answers)
 
         for _, cur_row in task_answers.iterrows():
-            worker = cur_row['worker']
+            worker = cur_row["worker"]
             emb_sum = 0.0
             seq_sum = 0.0
-            emb = cur_row['embedding']
-            seq = cur_row['output']
-            emb_norm = np.sum(emb ** 2)
+            emb = cur_row["embedding"]
+            seq = cur_row["output"]
+            emb_norm = np.sum(emb**2)
             for __, other_row in task_answers.iterrows():
-                if other_row['worker'] == worker:
+                if other_row["worker"] == worker:
                     continue
-                other_emb = other_row['embedding']
-                other_seq = other_row['output']
+                other_emb = other_row["embedding"]
+                other_seq = other_row["output"]
 
                 # embeddings similarity
                 diff_norm = np.sum((emb - other_emb) ** 2)
-                other_norm = np.sum(other_emb ** 2)
+                other_norm = np.sum(other_emb**2)
                 emb_sum += np.exp(-diff_norm / (emb_norm * other_norm))
 
                 # sequence similarity
                 seq_sum += self._output_similarity(seq, other_seq)
-            emb_sum /= (overlap - 1)
-            seq_sum /= (overlap - 1)
+            emb_sum /= overlap - 1
+            seq_sum /= overlap - 1
 
             yield worker, self.lambda_emb * emb_sum + self.lambda_out * seq_sum
 
-    def _filter_single_overlap(self, data: pd.DataFrame) -> Tuple[pd.DataFrame, pd.DataFrame]:
-        """Filter skills, embeddings, weights, and ranks for single overlap tasks that couldn't be processed by HRRASA.
-        """
+    def _filter_single_overlap(
+        self, data: pd.DataFrame
+    ) -> Tuple[pd.DataFrame, pd.DataFrame]:
+        """Filter skills, embeddings, weights, and ranks for single overlap tasks that couldn't be processed by HRRASA."""
 
         single_overlap_task_ids = []
-        for task, task_answers in data.groupby('task'):
+        for task, task_answers in data.groupby("task"):
             if len(task_answers) == 1:
                 single_overlap_task_ids.append(task)
-        data = data.set_index('task')
-        return data.drop(single_overlap_task_ids).reset_index(), data.loc[single_overlap_task_ids].reset_index()
-
-    def _fill_single_overlap_tasks_info(self, single_overlap_tasks: pd.DataFrame) -> None:
-        """Fill skills, embeddings, weights, and ranks for single overlap tasks.
-        """
+        data = data.set_index("task")
+        return (
+            data.drop(single_overlap_task_ids).reset_index(),
+            data.loc[single_overlap_task_ids].reset_index(),
+        )
+
+    def _fill_single_overlap_tasks_info(
+        self, single_overlap_tasks: pd.DataFrame
+    ) -> None:
+        """Fill skills, embeddings, weights, and ranks for single overlap tasks."""
 
         workers_to_append = []
         aggregated_embeddings_to_append = {}
         weights_to_append = []
         ranks_to_append = []
         for row in single_overlap_tasks.itertuples():
             if row.worker not in self.prior_skills_:
                 workers_to_append.append(row.worker)
             if row.task not in self.aggregated_embeddings_:
                 aggregated_embeddings_to_append[row.task] = row.embedding
-                weights_to_append.append({'task': row.task, 'worker': row.worker, 'weight': np.nan})
-                ranks_to_append.append({'task': row.task, 'output': row.output, 'rank': np.nan})
-
-        self.prior_skills_ = pd.concat([self.prior_skills_, pd.Series(np.nan, index=workers_to_append)])
-        self.skills_ = pd.concat([self.skills_, pd.Series(np.nan, index=workers_to_append)])
+                weights_to_append.append(
+                    {"task": row.task, "worker": row.worker, "weight": np.nan}
+                )
+                ranks_to_append.append(
+                    {"task": row.task, "output": row.output, "rank": np.nan}
+                )
+
+        self.prior_skills_ = pd.concat(
+            [self.prior_skills_, pd.Series(np.nan, index=workers_to_append)]
+        )
+        self.skills_ = pd.concat(
+            [self.skills_, pd.Series(np.nan, index=workers_to_append)]
+        )
         self.aggregated_embeddings_ = pd.concat(
-            [self.aggregated_embeddings_, pd.Series(aggregated_embeddings_to_append)])
+            [self.aggregated_embeddings_, pd.Series(aggregated_embeddings_to_append)]
+        )
         self.weights_ = pd.concat([self.weights_, pd.DataFrame(weights_to_append)])
-        if hasattr(self, 'ranks_'):
-            self.ranks_ = self.ranks_.append(pd.DataFrame(ranks_to_append))
+        if hasattr(self, "ranks_"):
+            self.ranks_ = self.ranks_.append(pd.DataFrame(ranks_to_append))  # type: ignore
```

### Comparing `crowd-kit-1.2.1/crowdkit/aggregation/embeddings/rasa.py` & `crowd-kit-1.3.0rc1/crowdkit/aggregation/embeddings/rasa.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 __all__ = [
-    'RASA',
+    "RASA",
 ]
 
-from typing import Any, List
 from functools import partial
+from typing import Any, List, Optional
 
 import attr
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
 import scipy.stats as sps
 from scipy.spatial import distance
 
-from .closest_to_average import ClosestToAverage
 from ..base import BaseEmbeddingsAggregator
+from .closest_to_average import ClosestToAverage
 
 _EPS = 1e-5
 
 
 @attr.s
 class RASA(BaseEmbeddingsAggregator):
     r"""The **Reliability Aware Sequence Aggregation** (RASA) algorithm consists of three steps.
@@ -35,125 +35,151 @@
     the closest one to $\hat{e}_i$.
 
     Jiyi Li, Fumiyo Fukumoto. A Dataset of Crowdsourced Word Sequences: Collections and Answer Aggregation for Ground Truth Creation.
     In *Proceedings of the First Workshop on Aggregating and Analysing Crowdsourced Annotations for NLP*,
     Hong Kong, China (November 3, 2019), 24–28.
     <https://doi.org/10.18653/v1/D19-5904>
 
-    Args:
-        n_iter: The maximum number of iterations.
-        tol: The tolerance stopping criterion for iterative methods with a variable number of steps.
-            The algorithm converges when the loss change is less than the `tol` parameter.
-        alpha: The significance level of the chi-squared distribution quantiles in the $\beta$ parameter formula.
-
     Examples:
         >>> import numpy as np
         >>> import pandas as pd
         >>> from crowdkit.aggregation import RASA
         >>> df = pd.DataFrame(
         >>>     [
         >>>         ['t1', 'p1', 'a', np.array([1.0, 0.0])],
         >>>         ['t1', 'p2', 'a', np.array([1.0, 0.0])],
         >>>         ['t1', 'p3', 'b', np.array([0.0, 1.0])]
         >>>     ],
         >>>     columns=['task', 'worker', 'output', 'embedding']
         >>> )
         >>> result = RASA().fit_predict(df)
-
-    Attributes:
-        embeddings_and_outputs_ (DataFrame): The task embeddings and outputs.
-            The `pandas.DataFrame` data is indexed by `task` and has the `embedding` and `output` columns.
-        loss_history_ (List[float]): A list of loss values during training.
     """
 
     n_iter: int = attr.ib(default=100)
+    """The maximum number of iterations."""
+
     tol: float = attr.ib(default=1e-9)
+    """The tolerance stopping criterion for iterative methods with a variable number of steps. The algorithm converges when the loss change is less than the `tol` parameter."""
+
     alpha: float = attr.ib(default=0.05)
-    # embeddings_and_outputs_
+    """The significance level of the chi-squared distribution quantiles in the $\beta$ parameter formula."""
+
     loss_history_: List[float] = attr.ib(init=False)
+    """A list of loss values during training."""
 
     @staticmethod
-    def _aggregate_embeddings(data: pd.DataFrame, skills: pd.Series,
-                              true_embeddings: pd.Series = None) -> pd.Series:
+    def _aggregate_embeddings(
+        data: pd.DataFrame,
+        skills: "pd.Series[Any]",
+        true_embeddings: Optional["pd.Series[Any]"] = None,
+    ) -> "pd.Series[Any]":
         """Calculates the weighted average of embeddings for each task."""
-        data = data.join(skills.rename('skill'), on='worker')
-        data['weighted_embedding'] = data.skill * data.embedding
-        group = data.groupby('task')
-        aggregated_embeddings = (group.weighted_embedding.apply(np.sum) / group.skill.sum())
+        data = data.join(skills.rename("skill"), on="worker")
+        data["weighted_embedding"] = data.skill * data.embedding
+        group = data.groupby("task")
+        aggregated_embeddings = (
+            group.weighted_embedding.apply(np.sum) / group.skill.sum()
+        )
+        if true_embeddings is None:
+            true_embeddings = pd.Series([], dtype=np.float64)
         aggregated_embeddings.update(true_embeddings)
         return aggregated_embeddings
 
     @staticmethod
-    def _update_skills(data: pd.DataFrame, aggregated_embeddings: pd.Series,
-                       prior_skills: pd.Series) -> pd.Series:
+    def _update_skills(
+        data: pd.DataFrame,
+        aggregated_embeddings: "pd.Series[Any]",
+        prior_skills: "pd.Series[Any]",
+    ) -> "pd.Series[Any]":
         """Estimates the global reliabilities by aggregated embeddings."""
-        data = data.join(aggregated_embeddings.rename('aggregated_embedding'), on='task')
-        data['distance'] = ((data.embedding - data.aggregated_embedding) ** 2).apply(np.sum)
-        total_distances = data.groupby('worker').distance.apply(np.sum)
+        data = data.join(
+            aggregated_embeddings.rename("aggregated_embedding"), on="task"
+        )
+        data["distance"] = ((data.embedding - data.aggregated_embedding) ** 2).apply(
+            np.sum
+        )
+        total_distances = data.groupby("worker").distance.apply(np.sum)
         total_distances.clip(lower=_EPS, inplace=True)
         return prior_skills / total_distances
 
     @staticmethod
-    def _cosine_distance(embedding: npt.NDArray[Any], avg_embedding: npt.NDArray[Any]) -> float:
+    def _cosine_distance(
+        embedding: npt.NDArray[Any], avg_embedding: npt.NDArray[Any]
+    ) -> float:
         if not embedding.any() or not avg_embedding.any():
-            return float('inf')
+            return float("inf")
         return float(distance.cosine(embedding, avg_embedding))
 
-    def _apply(self, data: pd.DataFrame, true_embeddings: pd.Series = None) -> 'RASA':
+    def _apply(
+        self, data: pd.DataFrame, true_embeddings: Optional["pd.Series[Any]"] = None
+    ) -> "RASA":
         cta = ClosestToAverage(distance=self._cosine_distance)
-        cta.fit(data, aggregated_embeddings=self.aggregated_embeddings_, true_embeddings=true_embeddings)
+        cta.fit(
+            data,
+            aggregated_embeddings=self.aggregated_embeddings_,
+            true_embeddings=true_embeddings,
+        )
         self.scores_ = cta.scores_
         self.embeddings_and_outputs_ = cta.embeddings_and_outputs_
         return self
 
-    def fit(self, data: pd.DataFrame, true_embeddings: pd.Series = None) -> 'RASA':
+    def fit(
+        self, data: pd.DataFrame, true_embeddings: Optional["pd.Series[Any]"] = None
+    ) -> "RASA":
         """Fits the model to the training data.
 
         Args:
             data (DataFrame): The workers' outputs with their embeddings.
                 The `pandas.DataFrame` data contains the `task`, `worker`, `output`, and `embedding` columns.
             true_embeddings (Series): The embeddings of the true task responses.
                 The `pandas.Series` data is indexed by `task` and contains the corresponding embeddings.
                 The multiple true embeddings are not supported for a single task.
 
         Returns:
             RASA: self.
         """
 
-        data = data[['task', 'worker', 'embedding']]
+        data = data[["task", "worker", "embedding"]]
 
         if true_embeddings is not None and not true_embeddings.index.is_unique:
             raise ValueError(
-                'Incorrect data in true_embeddings: multiple true embeddings for a single task are not supported.'
+                "Incorrect data in true_embeddings: multiple true embeddings for a single task are not supported."
             )
 
         # What we call skills here is called reliabilities in the paper
-        prior_skills = data.worker.value_counts().apply(partial(sps.chi2.isf, self.alpha / 2))
+        prior_skills = data.worker.value_counts().apply(
+            partial(sps.chi2.isf, self.alpha / 2)
+        )
         skills = pd.Series(1.0, index=data.worker.unique())
         aggregated_embeddings = None
         last_aggregated = None
 
         for _ in range(self.n_iter):
-            aggregated_embeddings = self._aggregate_embeddings(data, skills, true_embeddings)
+            aggregated_embeddings = self._aggregate_embeddings(
+                data, skills, true_embeddings
+            )
             skills = self._update_skills(data, aggregated_embeddings, prior_skills)
 
             if last_aggregated is not None:
                 delta = aggregated_embeddings - last_aggregated
-                loss = (delta * delta).sum().sum() / (aggregated_embeddings * aggregated_embeddings).sum().sum()
+                loss = (delta * delta).sum().sum() / (
+                    aggregated_embeddings * aggregated_embeddings
+                ).sum().sum()
                 if loss < self.tol:
                     break
             last_aggregated = aggregated_embeddings
 
         self.prior_skills_ = prior_skills
         self.skills_ = skills
         self.aggregated_embeddings_ = aggregated_embeddings
         return self
 
-    def fit_predict_scores(self, data: pd.DataFrame,
-                           true_embeddings: pd.Series = None) -> pd.DataFrame:
+    def fit_predict_scores(
+        self, data: pd.DataFrame, true_embeddings: Optional["pd.Series[Any]"] = None
+    ) -> pd.DataFrame:
         """Fits the model to the training data and returns the estimated scores.
 
         Args:
             data (DataFrame): The workers' outputs with their embeddings.
                 The `pandas.DataFrame` data contains the `task`, `worker`, `output`, and `embedding` columns.
             true_embeddings (Series): The embeddings of the true task responses.
                 The `pandas.Series` data is indexed by `task` and contains the corresponding embeddings.
@@ -163,23 +189,29 @@
             DataFrame: The task label scores.
                 The `pandas.DataFrame` data is indexed by `task` so that `result.loc[task, label]`
                 is a score of `label` for `task`.
         """
 
         return self.fit(data, true_embeddings)._apply(data, true_embeddings).scores_
 
-    def fit_predict(self, data: pd.DataFrame, true_embeddings: pd.Series = None) -> pd.DataFrame:
+    def fit_predict(
+        self, data: pd.DataFrame, true_embeddings: Optional["pd.Series[Any]"] = None
+    ) -> pd.DataFrame:
         """Fits the model to the training data and returns the aggregated outputs.
 
         Args:
             data (DataFrame): The workers' outputs with their embeddings.
                 The `pandas.DataFrame` data contains the `task`, `worker`, `output`, and `embedding` columns.
             true_embeddings (Series): The embeddings of the true task responses.
                 The `pandas.Series` data is indexed by `task` and contains the corresponding embeddings.
                 The multiple true embeddings are not supported for a single task.
 
         Returns:
             DataFrame: The task embeddings and outputs.
                 The `pandas.DataFrame` data is indexed by `task` and has the `embedding` and `output` columns.
         """
 
-        return self.fit(data, true_embeddings)._apply(data, true_embeddings).embeddings_and_outputs_
+        return (
+            self.fit(data, true_embeddings)
+            ._apply(data, true_embeddings)
+            .embeddings_and_outputs_
+        )
```

### Comparing `crowd-kit-1.2.1/crowdkit/aggregation/image_segmentation/segmentation_em.py` & `crowd-kit-1.3.0rc1/crowdkit/aggregation/image_segmentation/segmentation_em.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,177 +1,230 @@
-__all__ = ['SegmentationEM']
+__all__ = ["SegmentationEM"]
 
-from typing import List, Union, Any, cast
+from typing import Any, List, Union, cast
 
 import attr
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
 
 from ..base import BaseImageSegmentationAggregator
 
 
 @attr.s
 class SegmentationEM(BaseImageSegmentationAggregator):
-    """The EM algorithm for the image segmentation task.
+    r"""The **Segmentation EM-algorithm** performs a categorical
+    aggregation task for each pixel: should it be included in the resulting aggregate or not.
+    This task is solved by the single-coin Dawid-Skene algorithm.
+    Each worker has a latent parameter `skill` that shows the probability of this worker to answer correctly.
 
-    This method performs a categorical aggregation task for each pixel: should
-    it be included to the resulting aggregate or no. This task is solved by
-    the single coin Dawid-Skene algorithm. Each worker has a latent parameter
-    "skill" that shows the probability of this worker to answer correctly.
-    Skills and true pixels' labels are optimized by the Expectation-Maximization
-    algorithm.
-
-
-    Doris Jung-Lin Lee. 2018.
-    Quality Evaluation Methods for Crowdsourced Image Segmentation
-    <https://ilpubs.stanford.edu:8090/1161/1/main.pdf>
+    Skills and true pixel labels are optimized by the Expectation-Maximization algorithm:
+    1. **E-step**. Estimates the posterior probabilities using the specified workers' segmentations, the prior probabilities for each pixel,
+    and the workers' error probability vector.
+    2. **M-step**. Estimates the probability of a worker answering correctly using the specified workers' segmentations and the posterior probabilities for each pixel.
 
-    Args:
-        n_iter: A number of EM iterations.
+
+    D. Jung-Lin Lee, A. Das Sarma and A. Parameswaran. Aggregating Crowdsourced Image Segmentations.
+    *CEUR Workshop Proceedings. Vol. 2173*, (2018), 1-44.
+
+    <https://ceur-ws.org/Vol-2173/paper10.pdf>
 
     Examples:
         >>> import numpy as np
         >>> import pandas as pd
         >>> from crowdkit.aggregation import SegmentationEM
         >>> df = pd.DataFrame(
         >>>     [
         >>>         ['t1', 'p1', np.array([[1, 0], [1, 1]])],
         >>>         ['t1', 'p2', np.array([[0, 1], [1, 1]])],
         >>>         ['t1', 'p3', np.array([[0, 1], [1, 1]])]
         >>>     ],
         >>>     columns=['task', 'worker', 'segmentation']
         >>> )
         >>> result = SegmentationEM().fit_predict(df)
-
-    Attributes:
-        segmentations_ (Series): Tasks' segmentations.
-            A pandas.Series indexed by `task` such that `labels.loc[task]`
-            is the tasks's aggregated segmentation.
     """
 
     n_iter: int = attr.ib(default=10)
+    """The maximum number of EM iterations."""
+
     tol: float = attr.ib(default=1e-5)
+    """The tolerance stopping criterion for iterative methods with a variable number of steps.
+    The algorithm converges when the loss change is less than the `tol` parameter."""
+
     eps: float = 1e-15
-    # segmentations_
+    """The convergence threshold."""
+
+    segmentation_region_size_: int = attr.ib(init=False)
+    """Segmentation region size."""
+
+    segmentations_sizes_: npt.NDArray[Any] = attr.ib(init=False)
+    """Sizes of image segmentations."""
+
+    priors_: Union[float, npt.NDArray[Any]] = attr.ib(init=False)
+    """The prior probabilities for each pixel to be included in the resulting aggregate.
+    Each probability is in the range from 0 to 1, all probabilities must sum up to 1."""
+
+    posteriors_: npt.NDArray[Any] = attr.ib(init=False)
+    """The posterior probabilities for each pixel to be included in the resulting aggregate.
+    Each probability is in the range from 0 to 1, all probabilities must sum up to 1."""
+
+    errors_: npt.NDArray[Any] = attr.ib(init=False)
+    """The workers' error probability vector."""
+
     loss_history_: List[float] = attr.ib(init=False)
+    """A list of loss values during training."""
 
     @staticmethod
     def _e_step(
-            segmentations: pd.Series,
-            errors: npt.NDArray[Any],
-            priors: Union[float, npt.NDArray[Any]],
+        segmentations: npt.NDArray[Any],
+        errors: npt.NDArray[Any],
+        priors: Union[float, npt.NDArray[Any]],
     ) -> npt.NDArray[Any]:
         """
-        Perform E-step of algorithm.
-        Given workers' segmentations and error vector and priors
-        for each pixel calculates posteriori probabilities.
+        Performs E-step of the algorithm.
+        Estimates the posterior probabilities using the specified workers' segmentations, the prior probabilities for each pixel,
+        and the workers' error probability vector.
         """
 
-        weighted_seg = np.multiply(errors, segmentations.T.astype(float)).T + \
-                       np.multiply((1 - errors), (1 - segmentations).T.astype(float)).T
+        weighted_seg = (
+            np.multiply(errors, segmentations.T.astype(float)).T
+            + np.multiply((1 - errors), (1 - segmentations).T.astype(float)).T
+        )
 
-        with np.errstate(divide='ignore'):
+        with np.errstate(divide="ignore"):
             pos_log_prob = np.log(priors) + np.log(weighted_seg).sum(axis=0)
             neg_log_prob = np.log(1 - priors) + np.log(1 - weighted_seg).sum(axis=0)
 
-            with np.errstate(invalid='ignore'):
+            with np.errstate(invalid="ignore"):
                 # division by the denominator in the Bayes formula
-                posteriors: npt.NDArray[Any] = np.nan_to_num(np.exp(pos_log_prob) /  # type: ignore
-                                                                   (np.exp(pos_log_prob) + np.exp(neg_log_prob)),
-                                                                   nan=0)
+                posteriors: npt.NDArray[Any] = np.nan_to_num(
+                    np.exp(pos_log_prob)
+                    / (np.exp(pos_log_prob) + np.exp(neg_log_prob)),
+                    nan=0,
+                )
 
         return posteriors
 
     @staticmethod
-    def _m_step(segmentations: pd.Series, posteriors: npt.NDArray[Any],
-                segmentation_region_size: int, segmentations_sizes: npt.NDArray[Any]) -> npt.NDArray[Any]:
+    def _m_step(
+        segmentations: npt.NDArray[Any],
+        posteriors: npt.NDArray[Any],
+        segmentation_region_size: int,
+        segmentations_sizes: npt.NDArray[Any],
+    ) -> npt.NDArray[Any]:
         """
-        Perform M-step of algorithm.
-        Given a priori probabilities for each pixel and the segmentation of the workers,
-        it estimates worker's errors probabilities vector.
+        Performs M-step of the algorithm.
+        Estimates the probability of a worker answering correctly using the specified workers' segmentations and the posterior probabilities for each pixel.
         """
 
-        mean_errors_expectation: npt.NDArray[Any] = (segmentations_sizes + posteriors.sum() -
-                                                     2 * (segmentations * posteriors).
-                                                     sum(axis=(1, 2))) / segmentation_region_size
+        mean_errors_expectation: npt.NDArray[Any] = (
+            segmentations_sizes
+            + posteriors.sum()
+            - 2 * (segmentations * posteriors).sum(axis=(1, 2))
+        ) / segmentation_region_size
 
         # return probability of worker marking pixel correctly
         return 1 - mean_errors_expectation
 
-    def _evidence_lower_bound(self, segmentations: pd.Series,
-                              priors: Union[float, npt.NDArray[Any]],
-                              posteriors: npt.NDArray[Any],
-                              errors: npt.NDArray[Any]) -> float:
-        weighted_seg = (np.multiply(errors, segmentations.T.astype(float)).T +
-                        np.multiply((1 - errors), (1 - segmentations).T.astype(float)).T)
+    def _evidence_lower_bound(
+        self,
+        segmentations: npt.NDArray[Any],
+        priors: Union[float, npt.NDArray[Any]],
+        posteriors: npt.NDArray[Any],
+        errors: npt.NDArray[Any],
+    ) -> float:
+        weighted_seg = (
+            np.multiply(errors, segmentations.T.astype(float)).T
+            + np.multiply((1 - errors), (1 - segmentations).T.astype(float)).T
+        )
 
         # we handle log(0) * 0 == 0 case with nan_to_num so warnings are irrelevant here
-        with np.errstate(divide='ignore', invalid='ignore'):
-            log_likelihood_expectation: float = np.nan_to_num(  # type: ignore
-                (np.log(weighted_seg) + np.log(priors)[None, ...]) * posteriors, nan=0).sum() + np.nan_to_num(  # type: ignore
-                (np.log(1 - weighted_seg) + np.log(1 - priors)[None, ...]) * (1 - posteriors), nan=0).sum()
+        with np.errstate(divide="ignore", invalid="ignore"):
+            log_likelihood_expectation: float = (
+                np.nan_to_num(
+                    (np.log(weighted_seg) + np.log(priors)[None, ...]) * posteriors,
+                    nan=0,
+                ).sum()
+                + np.nan_to_num(
+                    (np.log(1 - weighted_seg) + np.log(1 - priors)[None, ...])
+                    * (1 - posteriors),
+                    nan=0,
+                ).sum()
+            )
+
+            return log_likelihood_expectation - float(
+                np.nan_to_num(np.log(posteriors) * posteriors, nan=0).sum()
+            )
 
-            return log_likelihood_expectation - float(np.nan_to_num(np.log(posteriors) * posteriors, nan=0).sum())  # type: ignore
-
-    def _aggregate_one(self, segmentations: pd.Series) -> npt.NDArray[np.bool_]:
+    def _aggregate_one(self, segmentations: "pd.Series[Any]") -> npt.NDArray[np.bool_]:
         """
-        Performs an expectation maximization algorithm for a single image.
+        Performs the Expectation-Maximization algorithm for a single image.
         """
         priors = sum(segmentations) / len(segmentations)
-        segmentations = np.stack(segmentations.values)
-        segmentation_region_size = segmentations.any(axis=0).sum()
+        segmentations_np: npt.NDArray[Any] = np.stack(segmentations.values)  # type: ignore
+        segmentation_region_size = segmentations_np.any(axis=0).sum()
 
         if segmentation_region_size == 0:
-            return np.zeros_like(segmentations[0])
+            return np.zeros_like(segmentations_np[0])
 
-        segmentations_sizes = segmentations.sum(axis=(1, 2))
+        segmentations_sizes = segmentations_np.sum(axis=(1, 2))
         # initialize with errors assuming that ground truth segmentation is majority vote
-        errors = self._m_step(segmentations, np.round(priors), segmentation_region_size, segmentations_sizes)  # type: ignore
+        errors = self._m_step(
+            segmentations_np,
+            np.round(priors),
+            segmentation_region_size,
+            segmentations_sizes,
+        )
         loss = -np.inf
         self.loss_history_ = []
         for _ in range(self.n_iter):
-            posteriors = self._e_step(segmentations, errors, priors)
+            posteriors = self._e_step(segmentations_np, errors, priors)
             posteriors[posteriors < self.eps] = 0
-            errors = self._m_step(segmentations, posteriors, segmentation_region_size, segmentations_sizes)
+            errors = self._m_step(
+                segmentations_np,
+                posteriors,
+                segmentation_region_size,
+                segmentations_sizes,
+            )
             new_loss = self._evidence_lower_bound(
-                segmentations, priors, posteriors, errors) / (len(segmentations) * segmentations[0].size)
+                segmentations_np, priors, posteriors, errors
+            ) / (len(segmentations_np) * segmentations_np[0].size)
             priors = posteriors
             self.loss_history_.append(new_loss)
             if new_loss - loss < self.tol:
                 break
             loss = new_loss
 
         return cast(npt.NDArray[np.bool_], priors > 0.5)
 
-    def fit(self, data: pd.DataFrame) -> 'SegmentationEM':
-        """Fit the model.
+    def fit(self, data: pd.DataFrame) -> "SegmentationEM":
+        """Fits the model to the training data with the EM algorithm.
 
         Args:
-            data (DataFrame): Workers' segmentations.
-                A pandas.DataFrame containing `worker`, `task` and `segmentation` columns'.
+            data (DataFrame): The training dataset of workers' segmentations
+                which is represented as the `pandas.DataFrame` data containing `task`, `worker`, and `segmentation` columns.
 
         Returns:
             SegmentationEM: self.
         """
 
-        data = data[['task', 'worker', 'segmentation']]
+        data = data[["task", "worker", "segmentation"]]
 
-        self.segmentations_ = data.groupby('task').segmentation.apply(
-            lambda segmentations: self._aggregate_one(segmentations)  # using lambda for python 3.7 compatibility
+        self.segmentations_ = data.groupby("task").segmentation.apply(
+            lambda segmentations: self._aggregate_one(
+                segmentations
+            )  # using lambda for python 3.7 compatibility
         )
         return self
 
-    def fit_predict(self, data: pd.DataFrame) -> pd.Series:
-        """Fit the model and return the aggregated segmentations.
+    def fit_predict(self, data: pd.DataFrame) -> "pd.Series[Any]":
+        """Fits the model to the training data and returns the aggregated segmentations.
 
         Args:
-            data (DataFrame): Workers' segmentations.
-                A pandas.DataFrame containing `worker`, `task` and `segmentation` columns'.
+            data (DataFrame): The training dataset of workers' segmentations
+                which is represented as the `pandas.DataFrame` data containing `task`, `worker`, and `segmentation` columns.
 
         Returns:
-            Series: Tasks' segmentations.
-                A pandas.Series indexed by `task` such that `labels.loc[task]`
-                is the tasks's aggregated segmentation.
+            Series: Task segmentations. The `pandas.Series` data is indexed by `task` so that `segmentations.loc[task]` is the task aggregated segmentation.
         """
 
         return self.fit(data).segmentations_
```

### Comparing `crowd-kit-1.2.1/crowdkit/aggregation/image_segmentation/segmentation_majority_vote.py` & `crowd-kit-1.3.0rc1/crowdkit/aggregation/image_segmentation/segmentation_majority_vote.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,86 +1,112 @@
-__all__ = ['SegmentationMajorityVote']
+__all__ = ["SegmentationMajorityVote"]
 
-from typing import Optional
+from typing import Any, Optional
 
 import attr
 import numpy as np
 import pandas as pd
 
 from ..base import BaseImageSegmentationAggregator
-from ..utils import add_skills_to_data
+from ..utils import add_skills_to_data, named_series_attrib
 
 
 @attr.s
 class SegmentationMajorityVote(BaseImageSegmentationAggregator):
-    """Segmentation Majority Vote - chooses a pixel if more than half of workers voted.
+    r"""The **Segmentation Majority Vote** algorithm chooses a pixel if and only if the pixel has "yes" votes
+    from at least half of all workers.
 
-    This method implements a straightforward approach to the image segmentations aggregation:
-    it assumes that if pixel is not inside in the worker's segmentation, this vote counts
-    as 0, otherwise, as 1. Next, the `SegmentationEM` aggregates these categorical values
-    for each pixel by the Majority Vote.
+    This method implements a straightforward approach to the image segmentation aggregation:
+    it assumes that if a pixel is not inside the worker's segmentation, this vote is considered to be equal to 0.
+    Otherwise, it is equal to 1. Then the `SegmentationEM` algorithm aggregates these categorical values
+    for each pixel by the Majority Vote algorithm.
 
-    The method also supports weighted majority voting if `skills` were provided to `fit` method.
+    The method also supports the weighted majority voting if the `skills` parameter is provided for the `fit` method.
 
-    Doris Jung-Lin Lee. 2018.
-    Quality Evaluation Methods for Crowdsourced Image Segmentation
-    <https://ilpubs.stanford.edu:8090/1161/1/main.pdf>
+    D. Jung-Lin Lee, A. Das Sarma and A. Parameswaran. Aggregating Crowdsourced Image Segmentations.
+    *CEUR Workshop Proceedings. Vol. 2173*, (2018), 1-44.
 
-    Args:
-        default_skill: A default skill value for missing skills.
+    <https://ceur-ws.org/Vol-2173/paper10.pdf>
 
     Examples:
         >>> import numpy as np
         >>> import pandas as pd
         >>> from crowdkit.aggregation import SegmentationMajorityVote
         >>> df = pd.DataFrame(
         >>>     [
         >>>         ['t1', 'p1', np.array([[1, 0], [1, 1]])],
         >>>         ['t1', 'p2', np.array([[0, 1], [1, 1]])],
         >>>         ['t1', 'p3', np.array([[0, 1], [1, 1]])]
         >>>     ],
         >>>     columns=['task', 'worker', 'segmentation']
         >>> )
         >>> result = SegmentationMajorityVote().fit_predict(df)
-
-    Attributes:
-        segmentations_ (Series): Tasks' segmentations.
-            A pandas.Series indexed by `task` such that `labels.loc[task]`
-            is the tasks's aggregated segmentation.
-
-        on_missing_skill (str): How to handle assignments done by workers with unknown skill.
-            Possible values:
-                    * "error" — raise an exception if there is at least one assignment done by user with unknown skill;
-                    * "ignore" — drop assignments with unknown skill values during prediction. Raise an exception if there is no
-                    assignments with known skill for any task;
-                    * value — default value will be used if skill is missing.
     """
 
-    # segmentations_
-
-    on_missing_skill: str = attr.ib(default='error')
     default_skill: Optional[float] = attr.ib(default=None)
+    """Default worker weight value."""
+
+    on_missing_skill: str = attr.ib(default="error")
+    """A value which specifies how to handle assignments performed by workers with an unknown skill.
 
-    def fit(self, data: pd.DataFrame, skills: pd.Series = None) -> 'SegmentationMajorityVote':
+    Possible values:
+    * `error`: raises an exception if there is at least one assignment performed by a worker with an unknown skill;
+    * `ignore`: drops assignments performed by workers with an unknown skill during prediction,
+    raises an exception if there are no assignments with a known skill for any task;
+    * `value`: the default value will be used if a skill is missing."""
+
+    skills_: Optional["pd.Series[Any]"] = named_series_attrib(name="skill")
+    """The workers' skills. The `pandas.Series` data is indexed by `worker` and has the corresponding worker skill."""
+
+    def fit(
+        self, data: pd.DataFrame, skills: Optional["pd.Series[Any]"] = None
+    ) -> "SegmentationMajorityVote":
         """
-        Fit the model.
+        Fits the model to the training data.
+
+        Args:
+            data (DataFrame): The training dataset of workers' segmentations
+                which is represented as the `pandas.DataFrame` data containing `task`, `worker`, and `segmentation` columns.
+
+            skills (Series): The workers' skills. The `pandas.Series` data is indexed by `worker`
+                and has the corresponding worker skill.
+
+        Returns:
+            SegmentationMajorityVote: self.
         """
 
-        data = data[['task', 'worker', 'segmentation']]
+        data = data[["task", "worker", "segmentation"]]
 
         if skills is None:
-            data['skill'] = 1
+            data["skill"] = 1
         else:
-            data = add_skills_to_data(data, skills, self.on_missing_skill, self.default_skill)
-
-        data['pixel_scores'] = data.segmentation * data.skill
-        group = data.groupby('task')
-
-        self.segmentations_ = (2 * group.pixel_scores.apply(np.sum) - group.skill.apply(np.sum)).apply(lambda x: x >= 0)
+            data = add_skills_to_data(
+                data, skills, self.on_missing_skill, self.default_skill
+            )
+
+        data["pixel_scores"] = data.segmentation * data.skill
+        group = data.groupby("task")
+
+        self.segmentations_ = (
+            2 * group.pixel_scores.apply(np.sum) - group.skill.apply(np.sum)
+        ).apply(lambda x: x >= 0)
         return self
 
-    def fit_predict(self, data: pd.DataFrame, skills: Optional[pd.Series] = None) -> pd.Series:
+    def fit_predict(
+        self, data: pd.DataFrame, skills: Optional["pd.Series[Any]"] = None
+    ) -> "pd.Series[Any]":
         """
-        Fit the model and return the aggregated segmentations.
+        Fits the model to the training data and returns the aggregated segmentations.
+
+        Args:
+            data (DataFrame): The training dataset of workers' segmentations
+                which is represented as the `pandas.DataFrame` data containing `task`, `worker`, and `segmentation` columns.
+
+            skills (Series): The workers' skills. The `pandas.Series` data is indexed by `worker`
+                and has the corresponding worker skill.
+
+        Returns:
+            Series: Task segmentations. The `pandas.Series` data is indexed by `task`
+                so that `segmentations.loc[task]` is the task aggregated segmentation.
         """
 
         return self.fit(data, skills).segmentations_
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `crowd-kit-1.2.1/crowdkit/aggregation/multilabel/binary_relevance.py` & `crowd-kit-1.3.0rc1/crowdkit/aggregation/multilabel/binary_relevance.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-__all__ = ['BinaryRelevance']
+__all__ = ["BinaryRelevance"]
 
-from typing import Dict, List, Union, Any
+from typing import Any, Dict, List, Union, cast
 
 import attr
 import pandas as pd
 from sklearn.preprocessing import MultiLabelBinarizer
-from ..classification import MajorityVote
 
 from ..base import BaseClassificationAggregator
+from ..classification import MajorityVote
 from ..utils import clone_aggregator
 
 
 @attr.s
 class BinaryRelevance(BaseClassificationAggregator):
     r"""Simple aggregation algorithm for multi-label classification.
 
@@ -23,18 +23,14 @@
 
     If this method is used for single-label classification, the output of the BinaryRelevance method may differ
     from the output of the basic aggregator used for its intended purpose, since each class generates a binary
     classification task, and therefore it is considered separately. For example, some objects may not have labels.
 
     {% endnote %}
 
-    Args:
-        base_aggregator: Aggregator instance that will be used for each binary classification. All class parameters
-         will be copied, except for the results of previous fit.
-
     Examples:
         >>> import pandas as pd
         >>> from crowdkit.aggregation import BinaryRelevance, DawidSkene
         >>> df = pd.DataFrame(
         >>>     [
         >>>         ['t1', 'w1', ['house', 'tree']],
         >>>         ['t1', 'w2', ['house']],
@@ -42,80 +38,79 @@
         >>>         ['t2', 'w1', ['car']],
         >>>         ['t2', 'w2', ['car', 'human']],
         >>>         ['t2', 'w3', ['train']]
         >>>     ]
         >>> )
         >>> df.columns = ['task', 'worker', 'label']
         >>> result = BinaryRelevance(DawidSkene(n_iter=10)).fit_predict(df)
-
-    Attributes:
-        labels_ (typing.Optional[pandas.core.series.Series]): Tasks' labels.
-            A pandas.Series indexed by `task` such that `labels.loc[task]`
-            is the tasks' aggregated labels.
-
-        aggregators_ (dict[str, BaseClassificationAggregator]): Labels' aggregators matched to classes.
-            A dictionary that matches aggregators to classes.
-            The key is the class found in the source data,
-            and the value is the aggregator used for this class.
-            The set of keys is all the classes that are in the input data.
     """
-    base_aggregator: BaseClassificationAggregator = attr.ib(
-        # validator=attr.validators.instance_of(BaseClassificationAggregator),
-        default=MajorityVote())
+
+    base_aggregator: BaseClassificationAggregator = attr.ib(default=MajorityVote())
+    """Aggregator instance that will be used for each binary classification.
+    All class parameters will be copied, except for the results of previous fit."""
+
     aggregators_: Dict[str, BaseClassificationAggregator] = dict()
+    """Label aggregators matched to classes. A dictionary that matches aggregators to classes.
+    The key is the class found in the source data, and the value is the aggregator used for this class.
+    The set of keys is all the classes that are in the input data."""
 
     @base_aggregator.validator
-    def _any_name_except_a_name_of_an_attribute(self, attribute: Any, value: Any) -> None:
-        assert issubclass(value.__class__, BaseClassificationAggregator), \
-            "Aggregator argument should be a classification aggregator"
+    def _any_name_except_a_name_of_an_attribute(
+        self, attribute: Any, value: Any
+    ) -> None:
+        assert issubclass(
+            value.__class__, BaseClassificationAggregator
+        ), "Aggregator argument should be a classification aggregator"
 
-    def fit(self, data: pd.DataFrame) -> 'BinaryRelevance':
+    def fit(self, data: pd.DataFrame) -> "BinaryRelevance":
         """Fit the aggregators.
 
         Args:
             data (DataFrame): Workers' labeling results.
                 A pandas.DataFrame containing `task`, `worker` and `label` columns.
                 'label' column should contain list of labels, e.g. ['tree', 'house', 'car']
 
         Returns:
             BinaryRelevance: self.
         """
 
-        data = data[['task', 'worker', 'label']]
+        data = data[["task", "worker", "label"]]
         mlb = MultiLabelBinarizer()
-        binarized_labels = mlb.fit_transform(data['label'])
+        binarized_labels = mlb.fit_transform(data["label"])
         task_to_labels: Dict[Union[str, float], List[Union[str, float]]] = dict()
 
         for i, label in enumerate(mlb.classes_):
-            single_label_df = data[['task', 'worker']]
-            single_label_df['label'] = binarized_labels[:, i]
+            single_label_df = data[["task", "worker"]]
+            single_label_df["label"] = binarized_labels[:, i]
 
             label_aggregator = clone_aggregator(self.base_aggregator)
             label_aggregator.fit_predict(single_label_df)
             self.aggregators_[label] = label_aggregator
             if label_aggregator.labels_ is not None:  # for mypy correct work
                 for task, label_value in label_aggregator.labels_.items():
                     if task not in task_to_labels:
-                        task_to_labels[task] = list()
+                        task_to_labels[cast(Union[str, float], task)] = list()
                     if label_value:
-                        task_to_labels[task].append(label)
+                        task_to_labels[cast(Union[str, float], task)].append(label)
         if not task_to_labels:
             self.labels_ = pd.Series(task_to_labels, dtype=float)
         else:
             self.labels_ = pd.Series(task_to_labels)
         if len(self.labels_):
-            self.labels_.index.name = 'task'
+            self.labels_.index.name = "task"
         return self
 
-    def fit_predict(self, data: pd.DataFrame) -> pd.Series:
+    def fit_predict(self, data: pd.DataFrame) -> "pd.Series[Any]":
         """Fit the model and return aggregated results.
 
-         Args:
-             data (DataFrame): Workers' labeling results.
-                 A pandas.DataFrame containing `task`, `worker` and `label` columns.
-
-         Returns:
-             Series: Tasks' labels.
-                 A pandas.Series indexed by `task` such that `labels.loc[task]`
-                 is a list with the task's aggregated labels.
-         """
-        return self.fit(data).labels_
+        Args:
+            data (DataFrame): Workers' labeling results.
+                A pandas.DataFrame containing `task`, `worker` and `label` columns.
+
+        Returns:
+            Series: Tasks' labels.
+                A pandas.Series indexed by `task` such that `labels.loc[task]`
+                is a list with the task's aggregated labels.
+        """
+        self.fit(data)
+        assert self.labels_ is not None, "no labels_ produced"
+        return self.labels_
```

### Comparing `crowd-kit-1.2.1/crowdkit/aggregation/pairwise/bradley_terry.py` & `crowd-kit-1.3.0rc1/crowdkit/aggregation/pairwise/bradley_terry.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-__all__ = ['BradleyTerry']
+__all__ = ["BradleyTerry"]
 
-from typing import Tuple, List
+from typing import Any, List, Tuple
 
 import attr
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
 
 from ..base import BasePairwiseAggregator
 
-_EPS = np.float_power(10, -10)
-
 
 @attr.s
 class BradleyTerry(BasePairwiseAggregator):
     r"""Bradley-Terry model for pairwise comparisons.
 
     The model implements the classic algorithm for aggregating pairwise comparisons.
     The algorithm constructs an items' ranking based on pairwise comparisons. Given
@@ -40,17 +38,14 @@
     MM algorithms for generalized Bradley-Terry models
     *Ann. Statist.*, Vol. 32, 1 (2004): 384–406.
 
     Bradley, R. A. and Terry, M. E.
     Rank analysis of incomplete block designs. I. The method of paired comparisons.
     *Biometrika*, Vol. 39 (1952): 324–345.
 
-    Args:
-        n_iter: A number of optimization iterations.
-
     Examples:
         The Bradley-Terry model needs the data to be a `DataFrame` containing columns
         `left`, `right`, and `label`. `left` and `right` contain identifiers of left and
         right items respectively, `label` contains identifiers of items that won these
         comparisons.
 
         >>> import pandas as pd
@@ -58,26 +53,27 @@
         >>> df = pd.DataFrame(
         >>>     [
         >>>         ['item1', 'item2', 'item1'],
         >>>         ['item2', 'item3', 'item2']
         >>>     ],
         >>>     columns=['left', 'right', 'label']
         >>> )
-
-    Attributes:
-        scores_ (Series): 'Labels' scores.
-            A pandas.Series index by labels and holding corresponding label's scores
     """
 
     n_iter: int = attr.ib()
+    """A number of optimization iterations."""
+
     tol: float = attr.ib(default=1e-5)
-    # scores_
+    """The tolerance stopping criterion for iterative methods with a variable number of steps.
+    The algorithm converges when the loss change is less than the `tol` parameter."""
+
     loss_history_: List[float] = attr.ib(init=False)
+    """A list of loss values during training."""
 
-    def fit(self, data: pd.DataFrame) -> 'BradleyTerry':
+    def fit(self, data: pd.DataFrame) -> "BradleyTerry":
         """Args:
             data (DataFrame): Workers' pairwise comparison results.
                 A pandas.DataFrame containing `worker`, `left`, `right`, and `label` columns'.
                 For each row `label` must be equal to either `left` column or `right` column.
 
         Returns:
             BradleyTerry: self.
@@ -100,15 +96,15 @@
         p_new = p.copy() / p.sum()
 
         p_old = None
 
         self.loss_history_ = []
 
         for _ in range(self.n_iter):
-            P: npt.NDArray[np.float_] = np.broadcast_to(p, M.shape)  # type: ignore
+            P: npt.NDArray[np.float_] = np.broadcast_to(p, M.shape)
 
             Z[active] = T[active] / (P[active] + P.T[active])
 
             p_new[:] = w
             p_new /= Z.sum(axis=0)
             p_new /= p_new.sum()
             p[:] = p_new
@@ -121,35 +117,37 @@
 
             p_old = p_new
 
         self.scores_ = pd.Series(p_new, index=unique_labels)
 
         return self
 
-    def fit_predict(self, data: pd.DataFrame) -> pd.Series:
+    def fit_predict(self, data: pd.DataFrame) -> "pd.Series[Any]":
         """Args:
             data (DataFrame): Workers' pairwise comparison results.
                 A pandas.DataFrame containing `worker`, `left`, `right`, and `label` columns'.
                 For each row `label` must be equal to either `left` column or `right` column.
 
         Returns:
             Series: 'Labels' scores.
                 A pandas.Series index by labels and holding corresponding label's scores
         """
         return self.fit(data).scores_
 
     @staticmethod
-    def _build_win_matrix(data: pd.DataFrame) -> Tuple[npt.NDArray[np.int_], npt.NDArray[np.int_]]:
-        data = data[['left', 'right', 'label']]
+    def _build_win_matrix(
+        data: pd.DataFrame,
+    ) -> Tuple[npt.NDArray[np.int_], npt.NDArray[np.int_]]:
+        data = data[["left", "right", "label"]]
 
-        unique_labels, np_data = np.unique(data.values, return_inverse=True)  # type: ignore
+        unique_labels, np_data = np.unique(data.values, return_inverse=True)
         np_data = np_data.reshape(data.shape)
 
         left_wins = np_data[np_data[:, 0] == np_data[:, 2], :2].T
         right_wins = np_data[np_data[:, 1] == np_data[:, 2], 1::-1].T
 
-        win_matrix = np.zeros((unique_labels.size, unique_labels.size), dtype='int')
+        win_matrix = np.zeros((unique_labels.size, unique_labels.size), dtype="int")
 
         np.add.at(win_matrix, tuple(left_wins), 1)
         np.add.at(win_matrix, tuple(right_wins), 1)
 
         return win_matrix, unique_labels
```

### Comparing `crowd-kit-1.2.1/crowdkit/aggregation/pairwise/noisy_bt.py` & `crowd-kit-1.3.0rc1/crowdkit/aggregation/pairwise/noisy_bt.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__all__ = ['NoisyBradleyTerry']
+__all__ = ["NoisyBradleyTerry"]
 
 from typing import Any
 
 import attr
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
@@ -13,22 +13,22 @@
 from ..utils import factorize, named_series_attrib
 
 
 @attr.s
 class NoisyBradleyTerry(BasePairwiseAggregator):
     r"""Bradley-Terry model for pairwise comparisons with additional parameters.
 
-    This model is a modification of the [Bradley-Terry model](crowdkit.aggregation.pairwise.bradley_terry.BradleyTerry.md)
-    with parameters for workers' skills (reliability) and biases.
+    This model is a modification of the BradleyTerry model with parameters
+    for workers' skills (reliability) and biases.
 
     Examples:
         The following example shows how to aggregate results of comparisons **grouped by some column**.
         In the example the two questions `q1` and `q2` are used to group the labeled data.
         Temporary data structure is created and the model is applied to it.
-        The results are splitted in two arrays, and each array contains scores for one of the initial groups.
+        The results are split into two arrays, and each array contains scores for one of the initial groups.
 
         >>> import pandas as pd
         >>> from crowdkit.aggregation import NoisyBradleyTerry
         >>> data = pd.DataFrame(
         >>>     [
         >>>         ['q1', 'w1', 'a', 'b', 'a'],
         >>>         ['q1', 'w2', 'a', 'b', 'b'],
@@ -45,105 +45,184 @@
         >>> for col in 'left', 'right', 'label':
         >>>     data[col] = list(zip(data['question'], data[col]))
         >>> result = NoisyBradleyTerry(n_iter=10).fit_predict(data)
         >>> # Separate results
         >>> result.index = pd.MultiIndex.from_tuples(result.index, names=['question', 'label'])
         >>> print(result['q1'])      # Scores for all items in the q1 question
         >>> print(result['q2']['b']) # Score for the item b in the q2 question
-
-    Attributes:
-        scores_ (Series): 'Labels' scores.
-            A pandas.Series index by labels and holding corresponding label's scores
-        skills_ (Series): workers' skills.
-            A pandas.Series index by workers and holding corresponding worker's skill
-        biases_ (Series): Predicted biases for each worker. Indicates the probability of a worker to choose the left item..
-            A series of workers' biases indexed by workers
     """
+
     n_iter: int = attr.ib(default=100)
+    """A number of optimization iterations."""
+
     tol: float = attr.ib(default=1e-5)
+    """The tolerance stopping criterion for iterative methods with a variable number of steps.
+    The algorithm converges when the loss change is less than the `tol` parameter."""
+
     regularization_ratio: float = attr.ib(default=1e-5)
+    """The regularization ratio."""
+
     random_state: int = attr.ib(default=0)
-    skills_: pd.Series = named_series_attrib(name='skill')
-    biases_: pd.Series = named_series_attrib(name='bias')
+    """The state of the random number generator."""
+
+    skills_: "pd.Series[Any]" = named_series_attrib(name="skill")
+    """A pandas.Series index by workers and holding corresponding worker's skill"""
 
-    # scores_
+    biases_: "pd.Series[Any]" = named_series_attrib(name="bias")
+    """Predicted biases for each worker. Indicates the probability of a worker to choose the left item.
+    A series of worker biases indexed by workers."""
 
-    def fit(self, data: pd.DataFrame) -> 'NoisyBradleyTerry':
+    def fit(self, data: pd.DataFrame) -> "NoisyBradleyTerry":
         """Args:
             data (DataFrame): Workers' pairwise comparison results.
                 A pandas.DataFrame containing `worker`, `left`, `right`, and `label` columns'.
                 For each row `label` must be equal to either `left` column or `right` column.
 
         Returns:
             NoisyBradleyTerry: self.
         """
 
-        unique_labels, np_data = factorize(data[['left', 'right', 'label']].values)
-        unique_workers, np_workers = factorize(data.worker.values)
+        unique_labels, np_data = factorize(data[["left", "right", "label"]].values)
+        unique_workers, np_workers = factorize(data.worker.values)  # type: ignore
         np.random.seed(self.random_state)
         x_0 = np.random.rand(1 + unique_labels.size + 2 * unique_workers.size)
         np_data += 1
 
-        x = minimize(self._compute_log_likelihood, x_0, jac=self._compute_gradient,
-                     args=(np_data, np_workers, unique_labels.size, unique_workers.size, self.regularization_ratio),
-                     method='L-BFGS-B', options={'maxiter': self.n_iter, 'ftol': np.float32(self.tol)})
+        x = minimize(
+            self._compute_log_likelihood,
+            x_0,
+            jac=self._compute_gradient,
+            args=(
+                np_data,
+                np_workers,
+                unique_labels.size,
+                unique_workers.size,
+                self.regularization_ratio,
+            ),
+            method="L-BFGS-B",
+            options={"maxiter": self.n_iter, "ftol": np.float32(self.tol)},
+        )
 
         biases_begin = unique_labels.size + 1
         workers_begin = biases_begin + unique_workers.size
 
-        self.scores_ = pd.Series(expit(x.x[1:biases_begin]), index=pd.Index(unique_labels, name='label'), name='score')
-        self.biases_ = pd.Series(expit(x.x[biases_begin:workers_begin]), index=unique_workers)
+        self.scores_ = pd.Series(
+            expit(x.x[1:biases_begin]),
+            index=pd.Index(unique_labels, name="label"),
+            name="score",
+        )
+        self.biases_ = pd.Series(
+            expit(x.x[biases_begin:workers_begin]), index=unique_workers
+        )
         self.skills_ = pd.Series(expit(x.x[workers_begin:]), index=unique_workers)
 
         return self
 
-    def fit_predict(self, data: pd.DataFrame) -> pd.Series:
+    def fit_predict(self, data: pd.DataFrame) -> "pd.Series[Any]":
         """Args:
             data (DataFrame): Workers' pairwise comparison results.
                 A pandas.DataFrame containing `worker`, `left`, `right`, and `label` columns'.
                 For each row `label` must be equal to either `left` column or `right` column.
 
         Returns:
             Series: 'Labels' scores.
                 A pandas.Series index by labels and holding corresponding label's scores
         """
         return self.fit(data).scores_
 
     @staticmethod
-    def _compute_log_likelihood(x: npt.NDArray[Any], np_data: npt.NDArray[Any],
-                                np_workers: npt.NDArray[Any], labels: int, workers: int,
-                                regularization_ratio: float) -> float:
+    def _compute_log_likelihood(
+        x: npt.NDArray[Any],
+        np_data: npt.NDArray[Any],
+        np_workers: npt.NDArray[Any],
+        labels: int,
+        workers: int,
+        regularization_ratio: float,
+    ) -> float:
         s_i = x[np_data[:, 0]]
         s_j = x[np_data[:, 1]]
         y = np.zeros_like(np_data[:, 2])
         y[np_data[:, 0] == np_data[:, 2]] = 1
         y[np_data[:, 0] != np_data[:, 2]] = -1
         q = x[1 + np_workers + labels]
         gamma = x[1 + np_workers + labels + workers]
 
-        total = np.sum(np.log(expit(gamma) * expit(y * (s_i - s_j)) + (1 - expit(gamma)) * expit(y * q)))
-        reg = np.sum(np.log(expit(x[0] - x[1:labels + 1]))) + np.sum(np.log(expit(x[1:labels + 1] - x[0])))
+        total = np.sum(
+            np.log(
+                expit(gamma) * expit(y * (s_i - s_j))
+                + (1 - expit(gamma)) * expit(y * q)
+            )
+        )
+        reg = np.sum(np.log(expit(x[0] - x[1 : labels + 1]))) + np.sum(
+            np.log(expit(x[1 : labels + 1] - x[0]))
+        )
 
         return float(-total + regularization_ratio * reg)
 
     @staticmethod
-    def _compute_gradient(x: npt.NDArray[Any], np_data: npt.NDArray[Any],
-                          np_workers: npt.NDArray[Any], labels: int, workers: int,
-                          regularization_ratio: float) -> npt.NDArray[Any]:
+    def _compute_gradient(
+        x: npt.NDArray[Any],
+        np_data: npt.NDArray[Any],
+        np_workers: npt.NDArray[Any],
+        labels: int,
+        workers: int,
+        regularization_ratio: float,
+    ) -> npt.NDArray[Any]:
         gradient = np.zeros_like(x)
 
         for worker_idx, (left_idx, right_idx, label) in zip(np_workers, np_data):
             s_i = x[left_idx]
             s_j = x[right_idx]
             y = 1 if label == left_idx else -1
             q = x[1 + labels + worker_idx]
             gamma = x[1 + labels + workers + worker_idx]
 
             # We'll use autograd in the future
-            gradient[left_idx] += (y * np.exp(y * (-(s_i - s_j)))) / ((np.exp(-gamma) + 1) * (np.exp(y * (-(s_i - s_j))) + 1) ** 2 * (1 / ((np.exp(-gamma) + 1) * (np.exp(y * (-(s_i - s_j))) + 1)) + (1 - 1 / (np.exp(-gamma) + 1)) / (np.exp(-q * y) + 1)))  # noqa
-            gradient[right_idx] += -(y * (np.exp(q * y) + 1) * np.exp(y * (s_i - s_j) + gamma)) / ((np.exp(y * (s_i - s_j)) + 1) * (np.exp(y * (s_i - s_j) + gamma + q * y) + np.exp(y * (s_i - s_j) + gamma) + np.exp(y * (s_i - s_j) + q * y) + np.exp(q * y)))  # noqa
-            gradient[labels + worker_idx] = (y * np.exp(q * y) * (np.exp(s_i * y) + np.exp(s_j * y))) / ((np.exp(q * y) + 1) * (np.exp(y * (s_i + q) + gamma) + np.exp(s_i * y + gamma) + np.exp(y * (s_i + q)) + np.exp(y * (s_j + q))))  # noqa #dq
-            gradient[labels + workers + worker_idx] = (np.exp(gamma) * (np.exp(s_i * y) - np.exp(y * (s_j + q)))) / ((np.exp(gamma) + 1) * (np.exp(y * (s_i + q) + gamma) + np.exp(s_i * y + gamma) + np.exp(y * (s_i + q)) + np.exp(y * (s_j + q))))  # noqa #dgamma
-
-        gradient[1:labels + 1] -= regularization_ratio * np.tanh((x[1:labels + 1] - x[0]) / 2.)
-        gradient[0] += regularization_ratio * np.sum(np.tanh((x[1:labels + 1] - x[0]) / 2.))
+            gradient[left_idx] += (y * np.exp(y * (-(s_i - s_j)))) / (
+                (np.exp(-gamma) + 1)
+                * (np.exp(y * (-(s_i - s_j))) + 1) ** 2
+                * (
+                    1 / ((np.exp(-gamma) + 1) * (np.exp(y * (-(s_i - s_j))) + 1))
+                    + (1 - 1 / (np.exp(-gamma) + 1)) / (np.exp(-q * y) + 1)
+                )
+            )  # noqa
+            gradient[right_idx] += -(
+                y * (np.exp(q * y) + 1) * np.exp(y * (s_i - s_j) + gamma)
+            ) / (
+                (np.exp(y * (s_i - s_j)) + 1)
+                * (
+                    np.exp(y * (s_i - s_j) + gamma + q * y)
+                    + np.exp(y * (s_i - s_j) + gamma)
+                    + np.exp(y * (s_i - s_j) + q * y)
+                    + np.exp(q * y)
+                )
+            )  # noqa
+            gradient[labels + worker_idx] = (
+                y * np.exp(q * y) * (np.exp(s_i * y) + np.exp(s_j * y))
+            ) / (
+                (np.exp(q * y) + 1)
+                * (
+                    np.exp(y * (s_i + q) + gamma)
+                    + np.exp(s_i * y + gamma)
+                    + np.exp(y * (s_i + q))
+                    + np.exp(y * (s_j + q))
+                )
+            )  # noqa #dq
+            gradient[labels + workers + worker_idx] = (
+                np.exp(gamma) * (np.exp(s_i * y) - np.exp(y * (s_j + q)))
+            ) / (
+                (np.exp(gamma) + 1)
+                * (
+                    np.exp(y * (s_i + q) + gamma)
+                    + np.exp(s_i * y + gamma)
+                    + np.exp(y * (s_i + q))
+                    + np.exp(y * (s_j + q))
+                )
+            )  # noqa #dgamma
+
+        gradient[1 : labels + 1] -= regularization_ratio * np.tanh(
+            (x[1 : labels + 1] - x[0]) / 2.0
+        )
+        gradient[0] += regularization_ratio * np.sum(
+            np.tanh((x[1 : labels + 1] - x[0]) / 2.0)
+        )
         return -gradient
```

### Comparing `crowd-kit-1.2.1/crowdkit/aggregation/texts/rover.py` & `crowd-kit-1.3.0rc1/crowdkit/aggregation/texts/rover.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 __all__ = [
-    'ROVER',
+    "ROVER",
 ]
 
 from copy import deepcopy
 from enum import Enum, unique
-from typing import List, Callable, Dict, Optional, Tuple, cast
+from typing import Any, Callable, Dict, Hashable, Iterator, List, Optional, Tuple, cast
 
 import attr
 import numpy as np
 import pandas as pd
 from tqdm.auto import tqdm
 
 from ..base import BaseTextsAggregator
 
 
 @unique
 class AlignmentAction(Enum):
-    DELETION = 'DELETION'
-    SUBSTITUTION = 'SUBSTITUTION'
-    INSERTION = 'INSERTION'
-    CORRECT = 'CORRECT'
+    DELETION = "DELETION"
+    SUBSTITUTION = "SUBSTITUTION"
+    INSERTION = "INSERTION"
+    CORRECT = "CORRECT"
 
 
 @attr.s
 class AlignmentEdge:
     value: str = attr.ib()
     sources_count: Optional[int] = attr.ib()
 
@@ -38,71 +38,78 @@
     Finally, the aggregated sequence is the result of majority voting on each edge of the WTN.
 
     J. G. Fiscus,
     "A post-processing system to yield reduced word error rates: Recognizer Output Voting Error Reduction (ROVER),"
     *1997 IEEE Workshop on Automatic Speech Recognition and Understanding Proceedings*, 1997, pp. 347-354.
     <https://doi.org/10.1109/ASRU.1997.659110>
 
-    Args:
-        tokenizer: A callable that takes a string and returns a list of tokens.
-        detokenizer: A callable that takes a list of tokens and returns a string.
-        silent: If false, show a progress bar.
-
     Examples:
-        >>> from crowdkit.aggregation import load_dataset
+        >>> from crowdkit.datasets import load_dataset
         >>> from crowdkit.aggregation import ROVER
         >>> df, gt = load_dataset('crowdspeech-test-clean')
         >>> df['text'] = df['text'].str.lower()
         >>> tokenizer = lambda s: s.split(' ')
         >>> detokenizer = lambda tokens: ' '.join(tokens)
         >>> result = ROVER(tokenizer, detokenizer).fit_predict(df)
 
     Attributes:
         texts_ (Series): Tasks' texts.
-            A pandas.Series indexed by `task` such that `result.loc[task, text]`
-            is the task's text.
+            A pandas.Series indexed by `task` such that `result.loc[task, text]` is the task's text.
     """
 
     tokenizer: Callable[[str], List[str]] = attr.ib()
+    """A callable that takes a string and returns a list of tokens."""
+
     detokenizer: Callable[[List[str]], str] = attr.ib()
+    """A callable that takes a list of tokens and returns a string."""
+
     silent: bool = attr.ib(default=True)
+    """If false, show a progress bar."""
 
     # Available after fit
     # texts_
 
-    def fit(self, data: pd.DataFrame) -> 'ROVER':
+    def fit(self, data: pd.DataFrame) -> "ROVER":
         """Fits the model. The aggregated results are saved to the `texts_` attribute.
 
         Args:
             data (DataFrame): Workers' text outputs.
                 A pandas.DataFrame containing `task`, `worker` and `text` columns.
 
         Returns:
             ROVER: self.
         """
 
+        def grouped_tasks() -> Iterator[Tuple[Hashable, pd.DataFrame]]:
+            grouped = data.groupby("task")
+
+            if self.silent:
+                yield from grouped
+            else:
+                yield from tqdm(grouped)
+
         result = {}
-        grouped_tasks = data.groupby('task') if self.silent else tqdm(data.groupby('task'))
-        for task, df in grouped_tasks:
-            hypotheses = [self.tokenizer(text) for i, text in enumerate(df['text'])]
+
+        for task, df in grouped_tasks():
+            hypotheses = [self.tokenizer(text) for i, text in enumerate(df["text"])]
 
             edges = self._build_word_transition_network(hypotheses)
             rover_result = self._get_result(edges)
 
-            text = self.detokenizer([value for value in rover_result if value != ''])
+            text = self.detokenizer([value for value in rover_result if value != ""])
 
             result[task] = text
 
-        texts = pd.Series(result, name='text')
-        texts.index.name = 'task'
+        texts = pd.Series(result, name="text")
+        texts.index.name = "task"
         self.texts_ = texts
 
         return self
 
-    def fit_predict(self, data: pd.DataFrame) -> pd.Series:
+    def fit_predict(self, data: pd.DataFrame) -> "pd.Series[Any]":
         """Fit the model and return the aggregated texts.
 
         Args:
             data (DataFrame): Workers' text outputs.
                 A pandas.DataFrame containing `task`, `worker` and `text` columns.
 
         Returns:
@@ -110,31 +117,35 @@
                 A pandas.Series indexed by `task` such that `result.loc[task, text]`
                 is the task's text.
         """
 
         self.fit(data)
         return self.texts_
 
-    def _build_word_transition_network(self, hypotheses: List[List[str]]) -> List[Dict[str, AlignmentEdge]]:
-        edges = [{edge.value: edge} for edge in self._get_edges_for_words(hypotheses[0])]
+    def _build_word_transition_network(
+        self, hypotheses: List[List[str]]
+    ) -> List[Dict[str, AlignmentEdge]]:
+        edges = [
+            {edge.value: edge} for edge in self._get_edges_for_words(hypotheses[0])
+        ]
 
         for sources_count, hyp in enumerate(hypotheses[1:], start=1):
             edges = self._align(edges, self._get_edges_for_words(hyp), sources_count)
 
         return edges
 
     @staticmethod
     def _get_edges_for_words(words: List[str]) -> List[AlignmentEdge]:
         return [AlignmentEdge(word, 1) for word in words]
 
     @staticmethod
     def _align(
-            ref_edges_sets: List[Dict[str, AlignmentEdge]],
-            hyp_edges: List[AlignmentEdge],
-            sources_count: int
+        ref_edges_sets: List[Dict[str, AlignmentEdge]],
+        hyp_edges: List[AlignmentEdge],
+        sources_count: int,
     ) -> List[Dict[str, AlignmentEdge]]:
         """Sequence alignment algorithm implementation.
 
         Aligns a sequence of sets of tokens (edges) with a sequence of tokens using dynamic programming algorithm. Look
         for section 2.1 in <https://doi.org/10.1109/ASRU.1997.659110> for implementation details. Penalty for
         insert/deletion or mismatch is 1.
 
@@ -144,104 +155,123 @@
            sources_count: Number of previously aligned sequences.
         """
 
         distance = np.zeros((len(hyp_edges) + 1, len(ref_edges_sets) + 1))
         distance[:, 0] = np.arange(len(hyp_edges) + 1)
         distance[0, :] = np.arange(len(ref_edges_sets) + 1)
 
-        memoization: List[List[Optional[Tuple[AlignmentAction, Dict[str, AlignmentEdge], AlignmentEdge]]]] = [
-            [None] * (len(ref_edges_sets) + 1) for _ in range(len(hyp_edges) + 1)
-        ]
+        memoization: List[
+            List[
+                Optional[
+                    Tuple[AlignmentAction, Dict[str, AlignmentEdge], AlignmentEdge]
+                ]
+            ]
+        ] = [[None] * (len(ref_edges_sets) + 1) for _ in range(len(hyp_edges) + 1)]
 
         for i, hyp_edge in enumerate(hyp_edges, start=1):
             memoization[i][0] = (
                 AlignmentAction.INSERTION,
-                {'': AlignmentEdge('', sources_count)},
+                {"": AlignmentEdge("", sources_count)},
                 hyp_edge,
             )
         for i, ref_edges in enumerate(ref_edges_sets, start=1):
             memoization[0][i] = (
                 AlignmentAction.DELETION,
                 ref_edges,
-                AlignmentEdge('', 1),
+                AlignmentEdge("", 1),
             )
 
         # find alignment minimal cost using dynamic programming algorithm
         for i, hyp_edge in enumerate(hyp_edges, start=1):
             hyp_word = hyp_edge and hyp_edge.value
             for j, ref_edges in enumerate(ref_edges_sets, start=1):
                 ref_words_set = ref_edges.keys()
                 is_hyp_word_in_ref = hyp_word in ref_words_set
 
                 options = []
 
                 if is_hyp_word_in_ref:
-                    options.append((
-                        distance[i - 1, j - 1],
+                    options.append(
                         (
-                            AlignmentAction.CORRECT,
-                            ref_edges,
-                            hyp_edge,
+                            distance[i - 1, j - 1],
+                            (
+                                AlignmentAction.CORRECT,
+                                ref_edges,
+                                hyp_edge,
+                            ),
                         )
-                    ))
+                    )
                 else:
-                    options.append((
-                        distance[i - 1, j - 1] + 1,
+                    options.append(
                         (
-                            AlignmentAction.SUBSTITUTION,
-                            ref_edges,
-                            hyp_edge,
+                            distance[i - 1, j - 1] + 1,
+                            (
+                                AlignmentAction.SUBSTITUTION,
+                                ref_edges,
+                                hyp_edge,
+                            ),
                         )
-                    ))
-                options.append((
-                    distance[i, j - 1] + ('' not in ref_edges),
+                    )
+                options.append(
                     (
-                        AlignmentAction.DELETION,
-                        ref_edges,
-                        AlignmentEdge('', 1),
+                        distance[i, j - 1] + ("" not in ref_edges),
+                        (
+                            AlignmentAction.DELETION,
+                            ref_edges,
+                            AlignmentEdge("", 1),
+                        ),
                     )
-                ))
-                options.append((
-                    distance[i - 1, j] + 1,
+                )
+                options.append(
                     (
-                        AlignmentAction.INSERTION,
-                        {'': AlignmentEdge('', sources_count)},
-                        hyp_edge,
+                        distance[i - 1, j] + 1,
+                        (
+                            AlignmentAction.INSERTION,
+                            {"": AlignmentEdge("", sources_count)},
+                            hyp_edge,
+                        ),
                     )
-                ))
+                )
 
-                distance[i, j], memoization[i][j] = min(options, key=lambda t: t[0])  # type: ignore
+                distance[i, j], memoization[i][j] = min(options, key=lambda t: t[0])
 
         alignment = []
         i = len(hyp_edges)
         j = len(ref_edges_sets)
 
         # reconstruct answer from dp array
         while i != 0 or j != 0:
-            action, ref_edges, hyp_edge = cast(Tuple[AlignmentAction, Dict[str, AlignmentEdge], AlignmentEdge],
-                                               memoization[i][j])
+            action, ref_edges, hyp_edge = cast(
+                Tuple[AlignmentAction, Dict[str, AlignmentEdge], AlignmentEdge],
+                memoization[i][j],
+            )
             joined_edges = deepcopy(ref_edges)
             hyp_edge_word = hyp_edge.value
             if hyp_edge_word not in joined_edges:
                 joined_edges[hyp_edge_word] = hyp_edge
             else:
                 # if word is already in set increment sources count for future score calculation
                 joined_edges[hyp_edge_word].sources_count += 1  # type: ignore
             alignment.append(joined_edges)
-            if action == AlignmentAction.CORRECT or action == AlignmentAction.SUBSTITUTION:
+            if (
+                action == AlignmentAction.CORRECT
+                or action == AlignmentAction.SUBSTITUTION
+            ):
                 i -= 1
                 j -= 1
             elif action == AlignmentAction.INSERTION:
                 i -= 1
             # action == AlignmentAction.DELETION
             else:
                 j -= 1
 
         return alignment[::-1]
 
     @staticmethod
     def _get_result(edges: List[Dict[str, AlignmentEdge]]) -> List[str]:
         result = []
         for edges_set in edges:
-            _, _, value = max((x.sources_count, len(x.value), x.value) for x in edges_set.values())
+            _, _, value = max(
+                (x.sources_count, len(x.value), x.value) for x in edges_set.values()
+            )
             result.append(value)
         return result
```

### Comparing `crowd-kit-1.2.1/crowdkit/aggregation/texts/text_hrrasa.py` & `crowd-kit-1.3.0rc1/crowdkit/aggregation/texts/text_hrrasa.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-__all__ = ['TextHRRASA']
+__all__ = ["TextHRRASA"]
 
-from typing import Callable, List, Any
+from typing import Any, Callable, List
 
 import numpy.typing as npt
 import pandas as pd
 
 from ..base import BaseTextsAggregator
 from ..embeddings.hrrasa import HRRASA, glue_similarity
 
@@ -39,28 +39,42 @@
     # texts_
 
     @property
     def loss_history_(self) -> List[float]:
         return self._hrrasa.loss_history_
 
     def __init__(
-            self,
-            encoder: Callable[[str], npt.ArrayLike],
-            n_iter: int = 100, tol: float = 1e-5, lambda_emb: float = 0.5, lambda_out: float = 0.5,
-            alpha: float = 0.05, calculate_ranks: bool = False,
-            output_similarity: Callable[[str, List[List[str]]], float] = glue_similarity
+        self,
+        encoder: Callable[[str], npt.ArrayLike],
+        n_iter: int = 100,
+        tol: float = 1e-5,
+        lambda_emb: float = 0.5,
+        lambda_out: float = 0.5,
+        alpha: float = 0.05,
+        calculate_ranks: bool = False,
+        output_similarity: Callable[[str, List[List[str]]], float] = glue_similarity,
     ) -> None:
         super().__init__()
         self.encoder = encoder
-        self._hrrasa = HRRASA(n_iter, tol, lambda_emb, lambda_out, alpha, calculate_ranks, output_similarity)
+        self._hrrasa = HRRASA(
+            n_iter,
+            tol,
+            lambda_emb,
+            lambda_out,
+            alpha,
+            calculate_ranks,
+            output_similarity,
+        )
 
     def __getattr__(self, name: str) -> Any:
         return getattr(self._hrrasa, name)
 
-    def fit_predict_scores(self, data: pd.DataFrame, true_objects: pd.Series = None) -> pd.DataFrame:
+    def fit_predict_scores(
+        self, data: pd.DataFrame, true_objects: "pd.Series[Any]"
+    ) -> pd.DataFrame:
         """Fit the model and return scores.
 
         Args:
             data (DataFrame): Workers' responses.
                 A pandas.DataFrame containing `task`, `worker` and `text` columns.
             true_objects (Series): Tasks' ground truth texts.
                 A pandas.Series indexed by `task` such that `labels.loc[task]`
@@ -68,17 +82,21 @@
 
         Returns:
             DataFrame: Tasks' label scores.
                 A pandas.DataFrame indexed by `task` such that `result.loc[task, label]`
                 is the score of `label` for `task`.
         """
 
-        return self._hrrasa.fit_predict_scores(self._encode_data(data), self._encode_true_objects(true_objects))
-
-    def fit_predict(self, data: pd.DataFrame, true_objects: pd.Series = None) -> pd.Series:
+        return self._hrrasa.fit_predict_scores(
+            self._encode_data(data), self._encode_true_objects(true_objects)
+        )
+
+    def fit_predict(  # type: ignore
+        self, data: pd.DataFrame, true_objects: "pd.Series[Any]"
+    ) -> "pd.Series[Any]":
         """Fit the model and return aggregated texts.
 
         Args:
             data (DataFrame): Workers' responses.
                 A pandas.DataFrame containing `task`, `worker` and `text` columns.
             true_objects (Series): Tasks' ground truth texts.
                 A pandas.Series indexed by `task` such that `labels.loc[task]`
@@ -86,18 +104,24 @@
 
         Returns:
             Series: Tasks' texts.
                 A pandas.Series indexed by `task` such that `result.loc[task, text]`
                 is the task's text.
         """
 
-        hrrasa_results = self._hrrasa.fit_predict(self._encode_data(data), self._encode_true_objects(true_objects))
-        self.texts_ = hrrasa_results.reset_index()[['task', 'output']].rename(columns={'output': 'text'}).set_index('task')
+        hrrasa_results = self._hrrasa.fit_predict(
+            self._encode_data(data), self._encode_true_objects(true_objects)
+        )
+        self.texts_ = (
+            hrrasa_results.reset_index()[["task", "output"]]  # type: ignore
+            .rename(columns={"output": "text"})
+            .set_index("task")
+        )
         return self.texts_
 
     def _encode_data(self, data: pd.DataFrame) -> pd.DataFrame:
-        data = data[['task', 'worker', 'text']].rename(columns={'text': 'output'})
-        data['embedding'] = data.output.apply(self.encoder)
+        data = data[["task", "worker", "text"]].rename(columns={"text": "output"})
+        data["embedding"] = data.output.apply(self.encoder)  # type: ignore
         return data
 
-    def _encode_true_objects(self, true_objects: pd.Series) -> pd.Series:
-        return true_objects and true_objects.apply(self.encoder)
+    def _encode_true_objects(self, true_objects: "pd.Series[Any]") -> "pd.Series[Any]":
+        return true_objects and true_objects.apply(self.encoder)  # type: ignore
```

### Comparing `crowd-kit-1.2.1/crowdkit/aggregation/texts/text_rasa.py` & `crowd-kit-1.3.0rc1/crowdkit/aggregation/texts/text_rasa.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-__all__ = ['TextRASA']
+__all__ = ["TextRASA"]
 
-from typing import Callable, Optional, Any, List
+from typing import Any, Callable, List
 
 import numpy.typing as npt
 import pandas as pd
 
 from ..base import BaseTextsAggregator
 from ..embeddings.rasa import RASA
 
@@ -34,24 +34,31 @@
 
     # texts_
 
     @property
     def loss_history_(self) -> List[float]:
         return self._rasa.loss_history_
 
-    def __init__(self, encoder: Callable[[str], npt.NDArray[Any]],
-                 n_iter: int = 100, tol: float = 1e-5, alpha: float = 0.05):
+    def __init__(
+        self,
+        encoder: Callable[[str], npt.NDArray[Any]],
+        n_iter: int = 100,
+        tol: float = 1e-5,
+        alpha: float = 0.05,
+    ):
         super().__init__()
         self.encoder = encoder
         self._rasa = RASA(n_iter, tol, alpha)
 
     def __getattr__(self, name: str) -> Any:
         return getattr(self._rasa, name)
 
-    def fit(self, data: pd.DataFrame, true_objects: Optional[pd.Series] = None) -> 'TextRASA':
+    def fit(  # type: ignore
+        self, data: pd.DataFrame, true_objects: "pd.Series[Any]"
+    ) -> "TextRASA":
         """Fit the model.
         Args:
             data (DataFrame): Workers' outputs.
                 A pandas.DataFrame containing `task`, `worker` and `output` columns.
             true_objects (Series): Tasks' ground truth labels.
                 A pandas.Series indexed by `task` such that `labels.loc[task]`
                 is the tasks's ground truth label.
@@ -59,15 +66,17 @@
         Returns:
             TextRASA: self.
         """
 
         self._rasa.fit(self._encode_data(data), self._encode_true_objects(true_objects))
         return self
 
-    def fit_predict_scores(self, data: pd.DataFrame, true_objects: Optional[pd.Series] = None) -> pd.DataFrame:
+    def fit_predict_scores(
+        self, data: pd.DataFrame, true_objects: "pd.Series[Any]"
+    ) -> pd.DataFrame:
         """Fit the model and return scores.
 
         Args:
             data (DataFrame): Workers' responses.
                 A pandas.DataFrame containing `task`, `worker` and `output` columns.
             true_objects (Series): Tasks' ground truth texts.
                 A pandas.Series indexed by `task` such that `labels.loc[task]`
@@ -75,17 +84,21 @@
 
         Returns:
             DataFrame: Tasks' label scores.
                 A pandas.DataFrame indexed by `task` such that `result.loc[task, label]`
                 is the score of `label` for `task`.
         """
 
-        return self._rasa.fit_predict_scores(self._encode_data(data), self._encode_true_objects(true_objects))
-
-    def fit_predict(self, data: pd.DataFrame, true_objects: Optional[pd.Series] = None) -> pd.Series:
+        return self._rasa.fit_predict_scores(
+            self._encode_data(data), self._encode_true_objects(true_objects)
+        )
+
+    def fit_predict(  # type: ignore
+        self, data: pd.DataFrame, true_objects: "pd.Series[Any]"
+    ) -> "pd.Series[Any]":
         """Fit the model and return aggregated texts.
 
         Args:
             data (DataFrame): Workers' responses.
                 A pandas.DataFrame containing `task`, `worker` and `output` columns.
             true_objects (Series): Tasks' ground truth texts.
                 A pandas.Series indexed by `task` such that `labels.loc[task]`
@@ -93,18 +106,24 @@
 
         Returns:
             Series: Tasks' texts.
                 A pandas.Series indexed by `task` such that `result.loc[task, text]`
                 is the task's text.
         """
 
-        rasa_results = self._rasa.fit_predict(self._encode_data(data), self._encode_true_objects(true_objects))
-        self.texts_ = rasa_results.reset_index()[['task', 'output']].rename(columns={'output': 'text'}).set_index('task')
+        rasa_results = self._rasa.fit_predict(
+            self._encode_data(data), self._encode_true_objects(true_objects)
+        )
+        self.texts_ = (
+            rasa_results.reset_index()[["task", "output"]]  # type: ignore
+            .rename(columns={"output": "text"})
+            .set_index("task")
+        )
         return self.texts_
 
     def _encode_data(self, data: pd.DataFrame) -> pd.DataFrame:
-        data = data[['task', 'worker', 'text']].rename(columns={'text': 'output'})
-        data['embedding'] = data.output.apply(self.encoder)
+        data = data[["task", "worker", "text"]].rename(columns={"text": "output"})
+        data["embedding"] = data.output.apply(self.encoder)  # type: ignore
         return data
 
-    def _encode_true_objects(self, true_objects: pd.Series) -> pd.Series:
-        return true_objects and true_objects.apply(self.encoder)
+    def _encode_true_objects(self, true_objects: "pd.Series[Any]") -> "pd.Series[Any]":
+        return true_objects and true_objects.apply(self.encoder)  # type: ignore
```

### Comparing `crowd-kit-1.2.1/crowdkit/aggregation/utils.py` & `crowd-kit-1.3.0rc1/crowdkit/aggregation/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,93 +1,105 @@
+"""
+Helper routines for aggregation.
+"""
+
 __all__ = [
-    'evaluate_in',
-    'evaluate_equal',
-    'evaluate',
-    'factorize',
-    'get_most_probable_labels',
-    'normalize_rows',
-    'manage_data',
-    'get_accuracy',
-    'add_skills_to_data',
-    'named_series_attrib',
-    'clone_aggregator',
+    "evaluate_in",
+    "evaluate_equal",
+    "evaluate",
+    "factorize",
+    "get_most_probable_labels",
+    "normalize_rows",
+    "manage_data",
+    "get_accuracy",
+    "add_skills_to_data",
+    "named_series_attrib",
+    "clone_aggregator",
 ]
 
-from typing import Tuple, Union, Callable, Optional, Any
+from typing import Any, Callable, Optional, Tuple, Union
 
 import attr
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
+
 from . import base
 
 
-def clone_aggregator(aggregator: 'base.BaseClassificationAggregator') -> 'base.BaseClassificationAggregator':
-    """ Construct a new unfitted aggregator with the same parameters.
+def clone_aggregator(
+    aggregator: "base.BaseClassificationAggregator",
+) -> "base.BaseClassificationAggregator":
+    """Construct a new unfitted aggregator with the same parameters.
     Args:
         aggregator (BaseClassificationAggregator): aggregator instance to be cloned
 
     Returns:
         BaseClassificationAggregator: cloned aggregator's instance. Its params are same to input,
             except for the results of previous fit (private attributes).
     """
-    assert isinstance(aggregator, base.BaseClassificationAggregator), \
-        'Can\'t clone object that is not inherit BaseClassificationAggregator'
+    assert isinstance(
+        aggregator, base.BaseClassificationAggregator
+    ), "Can't clone object that is not inherit BaseClassificationAggregator"
     aggregator_class = aggregator.__class__
     new_object_params = dict()
     for attr_name in aggregator.__dict__:
         # if attribute is not private
-        if not (attr_name.startswith('_') or attr_name.endswith('_')):
+        if not (attr_name.startswith("_") or attr_name.endswith("_")):
             new_object_params[attr_name] = getattr(aggregator, attr_name)
     new_object = aggregator_class(**new_object_params)
     return new_object
 
 
 def _argmax_random_ties(array: npt.NDArray[Any]) -> int:
-    # Returns the index of the maximum element
-    # If there are several such elements, it returns a random one
+    """Returns the index of the maximum element. If there are several such elements, it returns a random one."""
     return int(np.random.choice(np.flatnonzero(array == array.max())))
 
 
-def evaluate_in(row: pd.Series) -> int:
-    return int(row['label_pred'] in row['label_true'])
+def evaluate_in(row: "pd.Series[Any]") -> int:
+    return int(row["label_pred"] in row["label_true"])
 
 
-def evaluate_equal(row: pd.Series) -> int:
-    return int(row['label_pred'] == row['label_true'])
+def evaluate_equal(row: "pd.Series[Any]") -> int:
+    return int(row["label_pred"] == row["label_true"])
 
 
-def evaluate(df_true: pd.DataFrame, df_pred: pd.DataFrame,
-             evaluate_func: Callable[[pd.Series], int] = evaluate_in) -> Union[str, float]:
-    df = df_true.merge(df_pred, on='task', suffixes=('_true', '_pred'))
+def evaluate(
+    df_true: pd.DataFrame,
+    df_pred: pd.DataFrame,
+    evaluate_func: Callable[["pd.Series[Any]"], int] = evaluate_in,
+) -> Union[str, float]:
+    df = df_true.merge(df_pred, on="task", suffixes=("_true", "_pred"))
 
-    assert len(df_true) == len(df), f'Dataset length mismatch, expected {len(df_true):d}, got {len(df):d}'
+    assert len(df_true) == len(
+        df
+    ), f"Dataset length mismatch, expected {len(df_true)}, got {len(df)}"
 
-    df['evaluation'] = df.apply(evaluate_func, axis=1)
-    return float(df['evaluation'].mean())
+    df["evaluation"] = df.apply(evaluate_func, axis=1)
+    return float(df["evaluation"].mean())
 
 
 def factorize(data: npt.NDArray[Any]) -> Tuple[npt.NDArray[Any], npt.NDArray[Any]]:
-    unique_values, coded = np.unique(data, return_inverse=True)  # type: ignore
+    unique_values, coded = np.unique(data, return_inverse=True)
     return unique_values, coded.reshape(data.shape)
 
 
-def get_most_probable_labels(proba: pd.DataFrame) -> pd.Series:
+def get_most_probable_labels(proba: pd.DataFrame) -> "pd.Series[Any]":
     """Returns most probable labels
 
     Args:
         proba (DataFrame): Tasks' label probability distributions.
             A pandas.DataFrame indexed by `task` such that `result.loc[task, label]`
             is the probability of `task`'s true label to be equal to `label`. Each
             probability is between 0 and 1, all task's probabilities should sum up to 1
     """
     # patch for pandas<=1.1.5
     if not proba.size:
-        return pd.Series([], dtype='O')
-    return proba.idxmax(axis='columns')
+        return pd.Series([], dtype="O")
+    return proba.idxmax(axis="columns")
 
 
 def normalize_rows(scores: pd.DataFrame) -> pd.DataFrame:
     """Scales values so that every raw sums to 1
 
     Args:
         scores (DataFrame): Tasks' label scores.
@@ -99,121 +111,137 @@
             A pandas.DataFrame indexed by `task` such that `result.loc[task, label]`
             is the probability of `task`'s true label to be equal to `label`. Each
             probability is between 0 and 1, all task's probabilities should sum up to 1
     """
     return scores.div(scores.sum(axis=1), axis=0)
 
 
-def manage_data(data: pd.DataFrame, weights: Optional[pd.Series] = None,
-                skills: pd.Series = None) -> pd.DataFrame:
+def manage_data(
+    data: pd.DataFrame,
+    weights: Optional["pd.Series[Any]"] = None,
+    skills: Optional["pd.Series[Any]"] = None,
+) -> pd.DataFrame:
     """
     Args:
         data (DataFrame): Workers' labeling results.
             A pandas.DataFrame containing `task`, `worker` and `label` columns.
         skills (Series): workers' skills.
             A pandas.Series index by workers and holding corresponding worker's skill
     """
-    data = data[['task', 'worker', 'label']]
+    data = data[["task", "worker", "label"]]
 
     if weights is None:
-        data['weight'] = 1
+        data["weight"] = 1
     else:
-        data = data.join(weights.rename('weight'), on='task')
+        data = data.join(weights.rename("weight"), on="task")
 
     if skills is None:
-        data['skill'] = 1
+        data["skill"] = 1
     else:
-        data = data.join(skills.rename('skill'), on='task')
+        data = data.join(skills.rename("skill"), on="task")
 
     return data
 
 
-def get_accuracy(data: pd.DataFrame, true_labels: pd.Series, by: Optional[str] = None) -> pd.Series:
+def get_accuracy(
+    data: pd.DataFrame, true_labels: "pd.Series[Any]", by: Optional[str] = None
+) -> "pd.Series[Any]":
     """
     Args:
         data (DataFrame): Workers' labeling results.
             A pandas.DataFrame containing `task`, `worker` and `label` columns.
         true_labels (Series): Tasks' ground truth labels.
             A pandas.Series indexed by `task` such that `labels.loc[task]`
             is the tasks's ground truth label.
 
     Returns:
         Series: workers' skills.
             A pandas.Series index by workers and holding corresponding worker's skill
     """
-    if 'weight' in data.columns:
-        data = data[['task', 'worker', 'label', 'weight']]
+    if "weight" in data.columns:
+        data = data[["task", "worker", "label", "weight"]]
     else:
-        data = data[['task', 'worker', 'label']]
+        data = data[["task", "worker", "label"]]
 
     if data.empty:
-        data['true_label'] = []
+        data["true_label"] = []
     else:
-        data = data.join(pd.Series(true_labels, name='true_label'), on='task')
+        data = data.join(pd.Series(true_labels, name="true_label"), on="task")
 
     data = data[data.true_label.notna()]
 
-    if 'weight' not in data.columns:
-        data['weight'] = 1
-    data.eval('score = weight * (label == true_label)', inplace=True)
-
-    data = data.sort_values('score').drop_duplicates(['task', 'worker', 'label'], keep='last')
+    if "weight" not in data.columns:
+        data["weight"] = 1
+    data.eval("score = weight * (label == true_label)", inplace=True)
+
+    data = data.sort_values("score").drop_duplicates(
+        ["task", "worker", "label"], keep="last"
+    )
 
     if by is not None:
-        data = data.groupby(by)
-
-    return data.score.sum() / data.weight.sum()
+        group = data.groupby(by)
+        return group.score.sum() / group.weight.sum()
+    else:
+        return data.score.sum() / data.weight.sum()  # type: ignore
 
 
-def named_series_attrib(name: str) -> pd.Series:
+def named_series_attrib(name: str) -> "pd.Series[Any]":
     """Attrs attribute with converter and setter which preserves specified attribute name"""
 
-    def converter(series: pd.Series) -> pd.Series:
+    def converter(series: "pd.Series[Any]") -> "pd.Series[Any]":
         series.name = name
         return series
 
     return attr.ib(init=False, converter=converter, on_setattr=attr.setters.convert)
 
 
-def add_skills_to_data(data: pd.DataFrame, skills: pd.Series, on_missing_skill: str,
-                       default_skill: Optional[float]) -> pd.DataFrame:
+def add_skills_to_data(
+    data: pd.DataFrame,
+    skills: "pd.Series[Any]",
+    on_missing_skill: str,
+    default_skill: Optional[float],
+) -> pd.DataFrame:
     """
     Args:
         skills (Series): workers' skills.
             A pandas.Series index by workers and holding corresponding worker's skill
         on_missing_skill (str): How to handle assignments done by workers with unknown skill.
             Possible values:
                     * "error" — raise an exception if there is at least one assignment done by user with unknown skill;
                     * "ignore" — drop assignments with unknown skill values during prediction. Raise an exception if there is no
                     assignments with known skill for any task;
                     * value — default value will be used if skill is missing.
     """
-    data = data.join(skills.rename('skill'), on='worker')
+    data = data.join(skills.rename("skill"), on="worker")
 
-    if on_missing_skill != 'value' and default_skill is not None:
+    if on_missing_skill != "value" and default_skill is not None:
         raise ValueError('default_skill is used but on_missing_skill is not "value"')
 
-    if on_missing_skill == 'error':
-        missing_skills_count = data['skill'].isna().sum()
+    if on_missing_skill == "error":
+        missing_skills_count = data["skill"].isna().sum()
         if missing_skills_count > 0:
             raise ValueError(
                 f"Skill value is missing in {missing_skills_count} assignments. Specify skills for every"
                 f"used worker or use different 'on_unknown_skill' value."
             )
-    elif on_missing_skill == 'ignore':
-        data.set_index('task', inplace=True)
+    elif on_missing_skill == "ignore":
+        data.set_index("task", inplace=True)
         index_before_drop = data.index
         data.dropna(inplace=True)
         dropped_tasks_count = len(index_before_drop.difference(data.index))
         if dropped_tasks_count > 0:
             raise ValueError(
                 f"{dropped_tasks_count} tasks has no workers with known skills. Provide at least one worker with known"
                 f"skill for every task or use different 'on_unknown_skill' value."
             )
         data.reset_index(inplace=True)
-    elif on_missing_skill == 'value':
+    elif on_missing_skill == "value":
         if default_skill is None:
-            raise ValueError('Default skill value must be specified when using on_missing_skill="value"')
-        data.loc[data['skill'].isna(), 'skill'] = default_skill
+            raise ValueError(
+                'Default skill value must be specified when using on_missing_skill="value"'
+            )
+        data.loc[data["skill"].isna(), "skill"] = default_skill
     else:
-        raise ValueError(f'Unknown option {on_missing_skill!r} of "on_missing_skill" argument.')
+        raise ValueError(
+            f'Unknown option {on_missing_skill!r} of "on_missing_skill" argument.'
+        )
     return data
```

### Comparing `crowd-kit-1.2.1/crowdkit/datasets/_base.py` & `crowd-kit-1.3.0rc1/crowdkit/datasets/_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os.path
 import tempfile
 from hashlib import md5
-from os import environ, makedirs, listdir, rename
-from os.path import exists, expanduser, join, splitext, basename
+from os import environ, listdir, makedirs, rename
+from os.path import basename, exists, expanduser, join, splitext
 from shutil import unpack_archive
-from typing import Optional, AnyStr, cast
+from typing import AnyStr, Optional, cast
 from urllib.request import urlretrieve
 
 
 def get_data_dir(data_dir: Optional[AnyStr] = None) -> AnyStr:
     """Return the path of the crowd-kit data dir.
 
     This folder is used by some large dataset loaders to avoid downloading the
@@ -22,15 +22,17 @@
 
     Parameters:
         data_dir: str, default=None
             The path to crowd-kit data directory. If `None`, the default path
             is `~/crowdkit_data`.
     """
     if data_dir is None:
-        data_dir = cast(AnyStr, environ.get('CROWDKIT_DATA', join('~', 'crowdkit_data')))
+        data_dir = cast(
+            AnyStr, environ.get("CROWDKIT_DATA", join("~", "crowdkit_data"))
+        )
         data_dir = expanduser(data_dir)
 
     if not exists(data_dir):
         makedirs(data_dir)
 
     return data_dir
 
@@ -38,27 +40,28 @@
 def fetch_remote(url: str, checksum_url: str, path: str, data_dir: str) -> None:
     """Helper function to download a remote dataset into path
     Fetch a dataset pointed by remote's url, save into path using remote's
     filename and ensure its integrity based on the MD5 Checksum of the
     downloaded file.
     Parameters:
         url: str
-        checksum: str
+        checksum_url: str
         path: str, path to save a zip file
         data_dir: path to crowd-kit data directory
     """
     urlretrieve(url, path)
-    fetched_checksum = md5(open(path, 'rb').read()).hexdigest()
+    fetched_checksum = md5(open(path, "rb").read()).hexdigest()
     with tempfile.TemporaryDirectory() as tmpdir:
-        checksum_path = os.path.join(tmpdir, 'checksum.md5')
+        checksum_path = os.path.join(tmpdir, "checksum.md5")
         urlretrieve(checksum_url, checksum_path)
         with open(checksum_path) as f:
             checksum = f.read().strip()
     if checksum != fetched_checksum:
         raise IOError(
-            f"{path} has an MD5 checksum ({fetched_checksum}) differing from expected ({checksum}), file may be corrupted.")
+            f"{path} has an MD5 checksum ({fetched_checksum}) differing from expected ({checksum}), file may be corrupted."
+        )
     listed_data_dir = listdir(data_dir)
-    print(f'Unpacking {basename(path)}')
+    print(f"Unpacking {basename(path)}")
     unpack_archive(path, data_dir)
     data_dir_diff = set(listdir(data_dir)) - set(listed_data_dir)
     unpacked_folder_name = data_dir_diff.pop()
     rename(join(data_dir, unpacked_folder_name), splitext(path)[0])
```

### Comparing `crowd-kit-1.2.1/crowdkit/datasets/_loaders.py` & `crowd-kit-1.3.0rc1/crowdkit/datasets/_loaders.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,231 +1,348 @@
 from os.path import exists, join
-from typing import Optional, Tuple, Dict, Callable, Union
+from typing import Any, Callable, Dict, Optional, Tuple, Union
 
+import numpy as np
 import pandas as pd
 
-from ._base import get_data_dir, fetch_remote
+from ._base import fetch_remote, get_data_dir
 
 
-def _load_dataset(data_name: str, data_dir: Optional[str], data_url: str, checksum_url: str) -> str:
+def _load_dataset(
+    data_name: str, data_dir: Optional[str], data_url: str, checksum_url: str
+) -> str:
     data_root = get_data_dir(data_dir)
     full_data_path = join(data_root, data_name)
 
     if not exists(full_data_path):
-        print(f'Downloading {data_name} from remote')
-        fetch_remote(data_url, checksum_url, full_data_path + '.zip', data_root)
+        print(f"Downloading {data_name} from remote")
+        fetch_remote(data_url, checksum_url, full_data_path + ".zip", data_root)
 
     return full_data_path
 
 
-def load_relevance2(data_dir: Optional[str] = None) -> Tuple[pd.DataFrame, pd.Series]:
-    data_name = 'relevance-2'
-    data_url = 'https://tlk.s3.yandex.net/dataset/crowd-kit/relevance-2.zip'
-    checksum_url = 'https://tlk.s3.yandex.net/dataset/crowd-kit/relevance-2.md5'
-
-    def load_dataframes(data_path: str) -> Tuple[pd.DataFrame, pd.Series]:
-        labels = pd.read_csv(join(data_path, 'crowd_labels.csv')).rename(columns={'performer': 'worker'})
-        true_labels = pd.read_csv(join(data_path, 'gt.csv')).set_index('task')['label'].rename('true_label')
+def _load_ms_coco_dataframes(data_path: str) -> Tuple[pd.DataFrame, "pd.Series[Any]"]:
+    labels = np.load(join(data_path, "crowd_labels.npz"))
+    rows = []
+    for key in labels.files:
+        task, worker = key.split("\t")
+        rows.append([int(task), worker, labels[key]])
+    labels = pd.DataFrame(rows, columns=["task", "worker", "segmentation"])
+
+    true_labels = np.load(join(data_path, "gt.npz"))
+    true_labels = {int(key): true_labels[key] for key in true_labels.files}
+    true_labels = pd.Series(
+        true_labels,
+        name="true_segmentation",
+        index=pd.Index(true_labels.keys(), name="task"),
+    )
+
+    return labels, true_labels
+
+
+def load_relevance2(
+    data_dir: Optional[str] = None,
+) -> Tuple[pd.DataFrame, "pd.Series[Any]"]:
+    data_name = "relevance-2"
+    data_url = "https://tlk.s3.yandex.net/dataset/crowd-kit/relevance-2.zip"
+    checksum_url = "https://tlk.s3.yandex.net/dataset/crowd-kit/relevance-2.md5"
+
+    def load_dataframes(data_path: str) -> Tuple[pd.DataFrame, "pd.Series[Any]"]:
+        labels = pd.read_csv(join(data_path, "crowd_labels.csv")).rename(
+            columns={"performer": "worker"}
+        )
+        true_labels = (
+            pd.read_csv(join(data_path, "gt.csv"))
+            .set_index("task")["label"]
+            .rename("true_label")
+        )
 
         return labels, true_labels
 
     full_data_path = _load_dataset(data_name, data_dir, data_url, checksum_url)
 
     return load_dataframes(full_data_path)
 
 
-def load_relevance5(data_dir: Optional[str] = None) -> Tuple[pd.DataFrame, pd.Series]:
-    data_name = 'relevance-5'
-    data_url = 'https://tlk.s3.yandex.net/dataset/crowd-kit/relevance-5.zip'
-    checksum_url = 'https://tlk.s3.yandex.net/dataset/crowd-kit/relevance-5.md5'
-
-    def load_dataframes(data_path: str) -> Tuple[pd.DataFrame, pd.Series]:
-        labels = pd.read_csv(join(data_path, 'crowd_labels.csv')).rename(columns={'performer': 'worker'})
-        true_labels = pd.read_csv(join(data_path, 'gt.csv')).set_index('task')['label'].rename('true_label')
+def load_relevance5(
+    data_dir: Optional[str] = None,
+) -> Tuple[pd.DataFrame, "pd.Series[Any]"]:
+    data_name = "relevance-5"
+    data_url = "https://tlk.s3.yandex.net/dataset/crowd-kit/relevance-5.zip"
+    checksum_url = "https://tlk.s3.yandex.net/dataset/crowd-kit/relevance-5.md5"
+
+    def load_dataframes(data_path: str) -> Tuple[pd.DataFrame, "pd.Series[Any]"]:
+        labels = pd.read_csv(join(data_path, "crowd_labels.csv")).rename(
+            columns={"performer": "worker"}
+        )
+        true_labels = (
+            pd.read_csv(join(data_path, "gt.csv"))
+            .set_index("task")["label"]
+            .rename("true_label")
+        )
 
         return labels, true_labels
 
     full_data_path = _load_dataset(data_name, data_dir, data_url, checksum_url)
 
     return load_dataframes(full_data_path)
 
 
-def load_mscoco(data_dir: Optional[str] = None) -> Tuple[pd.DataFrame, pd.Series]:
-    data_name = 'mscoco'
-    data_url = 'https://tlk.s3.yandex.net/dataset/crowd-kit/mscoco.zip'
-    checksum_url = 'https://tlk.s3.yandex.net/dataset/crowd-kit/mscoco.md5'
-
-    def load_dataframes(data_path: str) -> Tuple[pd.DataFrame, pd.Series]:
-        labels = pd.read_pickle(join(data_path, 'crowd_labels.zip')).rename(columns={'performer': 'worker'})
-        true_labels = pd.read_pickle(join(data_path, 'gt.zip')).set_index('task')['true_segmentation']
+def load_netease_crowd(
+    data_dir: Optional[str] = None,
+) -> Tuple[pd.DataFrame, "pd.Series[Any]"]:
+    data_name = "netease_crowd"
+    data_url = (
+        "https://huggingface.co/datasets/"
+        "liuhyuu/NetEaseCrowd/resolve/58cab8743581a2647dcc86590a5a2aaf5429fa8c/NetEaseCrowd.zip"
+    )
+    checksum_url = (
+        "https://huggingface.co/datasets/"
+        "liuhyuu/NetEaseCrowd/resolve/58cab8743581a2647dcc86590a5a2aaf5429fa8c/NetEaseCrowd.md5"
+    )
+
+    def load_dataframes(data_path: str) -> Tuple[pd.DataFrame, "pd.Series[Any]"]:
+        labels = pd.read_csv(
+            join(data_path, "crowd_labels.csv"),
+            usecols=("workerId", "taskId", "answer"),
+        ).rename(columns={"workerId": "worker", "taskId": "task", "answer": "label"})
+        true_labels = (
+            pd.read_csv(join(data_path, "gt.csv"))
+            .rename(columns={"taskId": "task"})
+            .set_index("task")["truth"]
+            .rename("true_label")
+        )
 
         return labels, true_labels
 
     full_data_path = _load_dataset(data_name, data_dir, data_url, checksum_url)
 
     return load_dataframes(full_data_path)
 
 
-def load_mscoco_small(data_dir: Optional[str] = None) -> Tuple[pd.DataFrame, pd.Series]:
-    data_name = 'mscoco_small'
-    data_url = 'https://tlk.s3.yandex.net/dataset/crowd-kit/mscoco_small.zip'
-    checksum_url = 'https://tlk.s3.yandex.net/dataset/crowd-kit/mscoco_small.md5'
-
-    def load_dataframes(data_path: str) -> Tuple[pd.DataFrame, pd.Series]:
-        labels = pd.read_pickle(join(data_path, 'crowd_labels.zip')).rename(columns={'performer': 'worker'})
-        true_labels = pd.read_pickle(join(data_path, 'gt.zip'))
+def load_mscoco(
+    data_dir: Optional[str] = None,
+) -> Tuple[pd.DataFrame, "pd.Series[Any]"]:
+    data_name = "mscoco"
+    data_url = "https://huggingface.co/datasets/toloka/crowdkit-datasets/resolve/af2c00549cc026eaea80c18c54a686d98a58fd6e/mscoco.zip"
+    checksum_url = "https://huggingface.co/datasets/toloka/crowdkit-datasets/resolve/79d5468d12d233153c0fdcee0dd61b98980ff7a4/mscoco.md5"
 
-        return labels, true_labels
+    full_data_path = _load_dataset(data_name, data_dir, data_url, checksum_url)
+
+    return _load_ms_coco_dataframes(full_data_path)
+
+
+def load_mscoco_small(
+    data_dir: Optional[str] = None,
+) -> Tuple[pd.DataFrame, "pd.Series[Any]"]:
+    data_name = "mscoco_small"
+    data_url = "https://huggingface.co/datasets/toloka/crowdkit-datasets/resolve/0e0cac7f51869d4b20d83842c578ca3d013af7b7/mscoco_small.zip"
+    checksum_url = "https://huggingface.co/datasets/toloka/crowdkit-datasets/resolve/bb48658b78db95845ff2a8d3db3e533a493ab819/mscoco_small.md5"
 
     full_data_path = _load_dataset(data_name, data_dir, data_url, checksum_url)
 
-    return load_dataframes(full_data_path)
+    return _load_ms_coco_dataframes(full_data_path)
 
 
-def load_crowdspeech_dataframes(data_path: str) -> Tuple[pd.DataFrame, pd.Series]:
-    labels = pd.read_csv(join(data_path, 'crowd_labels.csv')).rename(columns={'output': 'text', 'performer': 'worker'})
-    true_labels = pd.read_csv(join(data_path, 'gt.csv')).set_index('task')['output'].rename('true_label')
+def load_crowdspeech_dataframes(
+    data_path: str,
+) -> Tuple[pd.DataFrame, "pd.Series[Any]"]:
+    labels = pd.read_csv(join(data_path, "crowd_labels.csv")).rename(
+        columns={"output": "text", "performer": "worker"}
+    )
+    true_labels = (
+        pd.read_csv(join(data_path, "gt.csv"))
+        .set_index("task")["output"]
+        .rename("true_label")
+    )
 
     return labels, true_labels
 
 
-def load_crowdspeech_dev_clean(data_dir: Optional[str] = None) -> Tuple[pd.DataFrame, pd.Series]:
-    data_name = 'crowdspeech-dev-clean'
-    data_url = 'https://tlk.s3.yandex.net/dataset/crowd-kit/crowdspeech-dev-clean.zip'
-    checksum_url = 'https://tlk.s3.yandex.net/dataset/crowd-kit/crowdspeech-dev-clean.md5'
+def load_crowdspeech_dev_clean(
+    data_dir: Optional[str] = None,
+) -> Tuple[pd.DataFrame, "pd.Series[Any]"]:
+    data_name = "crowdspeech-dev-clean"
+    data_url = "https://tlk.s3.yandex.net/dataset/crowd-kit/crowdspeech-dev-clean.zip"
+    checksum_url = (
+        "https://tlk.s3.yandex.net/dataset/crowd-kit/crowdspeech-dev-clean.md5"
+    )
 
     full_data_path = _load_dataset(data_name, data_dir, data_url, checksum_url)
     return load_crowdspeech_dataframes(full_data_path)
 
 
-def load_crowdspeech_dev_other(data_dir: Optional[str] = None) -> Tuple[pd.DataFrame, pd.Series]:
-    data_name = 'crowdspeech-dev-other'
-    data_url = 'https://tlk.s3.yandex.net/dataset/crowd-kit/crowdspeech-dev-other.zip'
-    checksum_url = 'https://tlk.s3.yandex.net/dataset/crowd-kit/crowdspeech-dev-other.md5'
+def load_crowdspeech_dev_other(
+    data_dir: Optional[str] = None,
+) -> Tuple[pd.DataFrame, "pd.Series[Any]"]:
+    data_name = "crowdspeech-dev-other"
+    data_url = "https://tlk.s3.yandex.net/dataset/crowd-kit/crowdspeech-dev-other.zip"
+    checksum_url = (
+        "https://tlk.s3.yandex.net/dataset/crowd-kit/crowdspeech-dev-other.md5"
+    )
 
     full_data_path = _load_dataset(data_name, data_dir, data_url, checksum_url)
     return load_crowdspeech_dataframes(full_data_path)
 
 
-def load_crowdspeech_test_clean(data_dir: Optional[str] = None) -> Tuple[pd.DataFrame, pd.Series]:
-    data_name = 'crowdspeech-test-clean'
-    data_url = 'https://tlk.s3.yandex.net/dataset/crowd-kit/crowdspeech-test-clean.zip'
-    checksum_url = 'https://tlk.s3.yandex.net/dataset/crowd-kit/crowdspeech-test-clean.md5'
+def load_crowdspeech_test_clean(
+    data_dir: Optional[str] = None,
+) -> Tuple[pd.DataFrame, "pd.Series[Any]"]:
+    data_name = "crowdspeech-test-clean"
+    data_url = "https://tlk.s3.yandex.net/dataset/crowd-kit/crowdspeech-test-clean.zip"
+    checksum_url = (
+        "https://tlk.s3.yandex.net/dataset/crowd-kit/crowdspeech-test-clean.md5"
+    )
 
     full_data_path = _load_dataset(data_name, data_dir, data_url, checksum_url)
     return load_crowdspeech_dataframes(full_data_path)
 
 
-def load_crowdspeech_test_other(data_dir: Optional[str] = None) -> Tuple[pd.DataFrame, pd.Series]:
-    data_name = 'crowdspeech-test-other'
-    data_url = 'https://tlk.s3.yandex.net/dataset/crowd-kit/crowdspeech-test-other.zip'
-    checksum_url = 'https://tlk.s3.yandex.net/dataset/crowd-kit/crowdspeech-test-other.md5'
+def load_crowdspeech_test_other(
+    data_dir: Optional[str] = None,
+) -> Tuple[pd.DataFrame, "pd.Series[Any]"]:
+    data_name = "crowdspeech-test-other"
+    data_url = "https://tlk.s3.yandex.net/dataset/crowd-kit/crowdspeech-test-other.zip"
+    checksum_url = (
+        "https://tlk.s3.yandex.net/dataset/crowd-kit/crowdspeech-test-other.md5"
+    )
 
     full_data_path = _load_dataset(data_name, data_dir, data_url, checksum_url)
     return load_crowdspeech_dataframes(full_data_path)
 
 
-def load_imdb_wiki_sbs(data_dir: Optional[str] = None) -> Tuple[pd.DataFrame, pd.Series]:
-    data_name = 'imdb-wiki-sbs'
-    data_url = 'https://tlk.s3.yandex.net/dataset/crowd-kit/imdb-wiki-sbs.zip'
-    checksum_url = 'https://tlk.s3.yandex.net/dataset/crowd-kit/imdb-wiki-sbs.md5'
-
-    def load_dataframes(data_path: str) -> Tuple[pd.DataFrame, pd.Series]:
-        labels = pd.read_csv(join(data_path, 'crowd_labels.csv')).rename(columns={'performer': 'worker'})
-        labels.loc[labels['label'] == 'left', 'label'] = labels['left'].copy()
-        labels.loc[labels['label'] == 'right', 'label'] = labels['right'].copy()
-
-        true_labels = pd.read_csv(join(data_path, 'gt.csv')).set_index('label')['score'].rename('true_label')
+def load_imdb_wiki_sbs(
+    data_dir: Optional[str] = None,
+) -> Tuple[pd.DataFrame, "pd.Series[Any]"]:
+    data_name = "imdb-wiki-sbs"
+    data_url = "https://tlk.s3.yandex.net/dataset/crowd-kit/imdb-wiki-sbs.zip"
+    checksum_url = "https://tlk.s3.yandex.net/dataset/crowd-kit/imdb-wiki-sbs.md5"
+
+    def load_dataframes(data_path: str) -> Tuple[pd.DataFrame, "pd.Series[Any]"]:
+        labels = pd.read_csv(join(data_path, "crowd_labels.csv")).rename(
+            columns={"performer": "worker"}
+        )
+        labels.loc[labels["label"] == "left", "label"] = labels["left"].copy()
+        labels.loc[labels["label"] == "right", "label"] = labels["right"].copy()
+
+        true_labels = (
+            pd.read_csv(join(data_path, "gt.csv"))
+            .set_index("label")["score"]
+            .rename("true_label")
+        )
 
         return labels, true_labels
 
     full_data_path = _load_dataset(data_name, data_dir, data_url, checksum_url)
 
     return load_dataframes(full_data_path)
 
 
-def load_nist_trec_relevance(data_dir: Optional[str] = None) -> Tuple[pd.DataFrame, pd.Series]:
-    data_name = 'nist-trec-relevance'
-    data_url = 'https://tlk.s3.yandex.net/dataset/crowd-kit/relevance.zip'
-    checksum_url = 'https://tlk.s3.yandex.net/dataset/crowd-kit/relevance.md5'
-
-    def load_dataframes(data_path: str) -> Tuple[pd.DataFrame, pd.Series]:
-        labels = pd.read_csv(join(data_path, 'crowd_labels.csv')).rename(columns={'performer': 'worker'})
-        true_labels = pd.read_csv(join(data_path, 'gt.csv')).set_index('task')['label'].rename('true_label')
+def load_nist_trec_relevance(
+    data_dir: Optional[str] = None,
+) -> Tuple[pd.DataFrame, "pd.Series[Any]"]:
+    data_name = "nist-trec-relevance"
+    data_url = "https://tlk.s3.yandex.net/dataset/crowd-kit/relevance.zip"
+    checksum_url = "https://tlk.s3.yandex.net/dataset/crowd-kit/relevance.md5"
+
+    def load_dataframes(data_path: str) -> Tuple[pd.DataFrame, "pd.Series[Any]"]:
+        labels = pd.read_csv(join(data_path, "crowd_labels.csv")).rename(
+            columns={"performer": "worker"}
+        )
+        true_labels = (
+            pd.read_csv(join(data_path, "gt.csv"))
+            .set_index("task")["label"]
+            .rename("true_label")
+        )
 
         return labels, true_labels
 
     full_data_path = _load_dataset(data_name, data_dir, data_url, checksum_url)
 
     return load_dataframes(full_data_path)
 
 
-DATA_LOADERS: Dict[str, Dict[str, Union[str, Callable[[Optional[str]], Tuple[pd.DataFrame, pd.Series]]]]] = {
-    'relevance-2': {
-        'loader': load_relevance2,
-        'description': 'This dataset, designed for evaluating answer aggregation methods in crowdsourcing, '
-        'contains around 0.5 million anonymized crowdsourced labels collected in the Relevance 2 Gradations project'
-        ' in 2016 at Yandex. In this project, query-document pairs are provided with binary labels: relevant or non-relevant.'
-    },
-    'relevance-5': {
-        'loader': load_relevance5,
-        'description': 'This dataset was designed for evaluating answer aggregation methods in crowdsourcing. '
-        'It contains around 1 million anonymized crowdsourced labels collected in the Relevance 5 Gradations project'
-        ' in 2016 at Yandex. In this project, query-document pairs are labeled on a scale of 1 to 5. from least relevant'
-        ' to most relevant.'
-    },
-    'mscoco': {
-        'loader': load_mscoco,
-        'description': 'A sample of 2,000 images segmentations from MSCOCO dataset (https://cocodataset.org, licensed '
-        'under Creative Commons Attribution 4.0 International Public License.) annotated on Toloka by 911 peformers. '
-        'For each image, 9 workers submitted segmentations.'
-    },
-    'mscoco_small': {
-        'loader': load_mscoco_small,
-        'description': 'A sample of 100 images segmentations from MSCOCO dataset (https://cocodataset.org, licensed '
-        'under Creative Commons Attribution 4.0 International Public License.) annotated on Toloka by 96 workers. '
-        'For each image, 9 workers submitted segmentations.'
-    },
-    'crowdspeech-dev-clean': {
-        'loader': load_crowdspeech_dev_clean,
-        'description': 'This dataset is a publicly available large-scale dataset of crowdsourced audio transcriptions. '
-        'It contains annotations for more than 20 hours of English speech from more than 1,000 crowd workers. '
-        'This dataset corresponds to LibriSpeech (https://www.openslr.org/12,  licensed under CC BY 4.0) '
-        'dev-clean dataset'
-    },
-    'crowdspeech-test-clean': {
-        'loader': load_crowdspeech_test_clean,
-        'description': 'This dataset is a publicly available large-scale dataset of crowdsourced audio transcriptions. '
-        'It contains annotations for more than 20 hours of English speech from more than 1,000 crowd workers. '
-        'This dataset corresponds to LibriSpeech (https://www.openslr.org/12, licensed under CC BY 4.0) '
-        'test-clean dataset'
-    },
-    'crowdspeech-dev-other': {
-        'loader': load_crowdspeech_dev_other,
-        'description': 'This dataset is a publicly available large-scale dataset of crowdsourced audio transcriptions. '
-        'It contains annotations for more than 20 hours of English speech from more than 1,000 crowd workers. '
-        'This dataset corresponds to LibriSpeech (https://www.openslr.org/12, licensed under CC BY 4.0) '
-        'dev-clean dataset'
-    },
-    'crowdspeech-test-other': {
-        'loader': load_crowdspeech_test_other,
-        'description': 'This dataset is a publicly available large-scale dataset of crowdsourced audio transcriptions. '
-        'It contains annotations for more than 20 hours of English speech from more than 1,000 crowd workers. '
-        'This dataset corresponds to LibriSpeech (https://www.openslr.org/12, licensed under CC BY 4.0) '
-        'test-clean dataset'
-    },
-    'imdb-wiki-sbs': {
-        'loader': load_imdb_wiki_sbs,
-        'description': 'A sample of 2,497 images from the IMDB-WIKI dataset '
-        '(https://data.vision.ee.ethz.ch/cvl/rrothe/imdb-wiki/) annotated on Toloka. This dataset contains images of '
-        'people with reliable ground-truth age assigned to every image. The annotation allowed us to obtain 84,543 '
-        'comparisons by 2,085 workers.'
-    },
-    'nist-trec-relevance': {
-        'loader': load_nist_trec_relevance,
-        'description': 'A dataset of English Web pages from the ClueWeb09 for English search queries which relevance '
-        'were judged using crowdsourcing. This dataset was collected during NIST TREC Relevance Feedback Track 2010 '
-        '(C.Buckley, M.Lease, and M.D.Smucker. Overview of the trec 2010 relevance feedback track (notebook). In The '
-        'Nineteenth TREC Notebook, 2010.). There are 20,232 total (topic, document) examples (noisily) judged by 766 '
-        'workers, who produced a total of 98,453 judgments. 3277 of the examples have prior "gold" labels by NIST.'
-    }
+DATA_LOADERS: Dict[
+    str,
+    Dict[
+        str,
+        Union[str, Callable[[Optional[str]], Tuple[pd.DataFrame, "pd.Series[Any]"]]],
+    ],
+] = {
+    "relevance-2": {
+        "loader": load_relevance2,
+        "description": "This dataset, designed for evaluating answer aggregation methods in crowdsourcing, "
+        "contains around 0.5 million anonymized crowdsourced labels collected in the Relevance 2 Gradations project"
+        " in 2016 at Yandex. In this project, query-document pairs are provided with binary labels: relevant or non-relevant.",
+    },
+    "relevance-5": {
+        "loader": load_relevance5,
+        "description": "This dataset was designed for evaluating answer aggregation methods in crowdsourcing. "
+        "It contains around 1 million anonymized crowdsourced labels collected in the Relevance 5 Gradations project"
+        " in 2016 at Yandex. In this project, query-document pairs are labeled on a scale of 1 to 5. from least relevant"
+        " to most relevant.",
+    },
+    "netease_crowd": {
+        "loader": load_netease_crowd,
+        "description": "NetEaseCrowd(https://github.com/fuxiAIlab/NetEaseCrowd-Dataset) "
+        "is a large-scale crowdsourcing annotation dataset based on a mature Chinese data "
+        "crowdsourcing platform of NetEase Inc.. NetEaseCrowd dataset contains about 2,400 workers, "
+        "1,000,000 tasks, and 6,000,000 annotations between them, "
+        "where the annotations are collected in about 6 months. "
+        "This dataset is licensed under CC BY-SA 4.0",
+    },
+    "mscoco": {
+        "loader": load_mscoco,
+        "description": "A sample of 2,000 images segmentations from MSCOCO dataset (https://cocodataset.org, licensed "
+        "under Creative Commons Attribution 4.0 International Public License.) annotated on Toloka by 911 performers. "
+        "For each image, 9 workers submitted segmentations.",
+    },
+    "mscoco_small": {
+        "loader": load_mscoco_small,
+        "description": "A sample of 100 images segmentations from MSCOCO dataset (https://cocodataset.org, licensed "
+        "under Creative Commons Attribution 4.0 International Public License.) annotated on Toloka by 96 workers. "
+        "For each image, 9 workers submitted segmentations.",
+    },
+    "crowdspeech-dev-clean": {
+        "loader": load_crowdspeech_dev_clean,
+        "description": "This dataset is a publicly available large-scale dataset of crowdsourced audio transcriptions. "
+        "It contains annotations for more than 20 hours of English speech from more than 1,000 crowd workers. "
+        "This dataset corresponds to LibriSpeech (https://www.openslr.org/12,  licensed under CC BY 4.0) "
+        "dev-clean dataset",
+    },
+    "crowdspeech-test-clean": {
+        "loader": load_crowdspeech_test_clean,
+        "description": "This dataset is a publicly available large-scale dataset of crowdsourced audio transcriptions. "
+        "It contains annotations for more than 20 hours of English speech from more than 1,000 crowd workers. "
+        "This dataset corresponds to LibriSpeech (https://www.openslr.org/12, licensed under CC BY 4.0) "
+        "test-clean dataset",
+    },
+    "crowdspeech-dev-other": {
+        "loader": load_crowdspeech_dev_other,
+        "description": "This dataset is a publicly available large-scale dataset of crowdsourced audio transcriptions. "
+        "It contains annotations for more than 20 hours of English speech from more than 1,000 crowd workers. "
+        "This dataset corresponds to LibriSpeech (https://www.openslr.org/12, licensed under CC BY 4.0) "
+        "dev-clean dataset",
+    },
+    "crowdspeech-test-other": {
+        "loader": load_crowdspeech_test_other,
+        "description": "This dataset is a publicly available large-scale dataset of crowdsourced audio transcriptions. "
+        "It contains annotations for more than 20 hours of English speech from more than 1,000 crowd workers. "
+        "This dataset corresponds to LibriSpeech (https://www.openslr.org/12, licensed under CC BY 4.0) "
+        "test-clean dataset",
+    },
+    "imdb-wiki-sbs": {
+        "loader": load_imdb_wiki_sbs,
+        "description": "A sample of 2,497 images from the IMDB-WIKI dataset "
+        "(https://data.vision.ee.ethz.ch/cvl/rrothe/imdb-wiki/) annotated on Toloka. This dataset contains images of "
+        "people with reliable ground-truth age assigned to every image. The annotation allowed us to obtain 84,543 "
+        "comparisons by 2,085 workers.",
+    },
+    "nist-trec-relevance": {
+        "loader": load_nist_trec_relevance,
+        "description": "A dataset of English Web pages from the ClueWeb09 for English search queries which relevance "
+        "were judged using crowdsourcing. This dataset was collected during NIST TREC Relevance Feedback Track 2010 "
+        "(C.Buckley, M.Lease, and M.D.Smucker. Overview of the trec 2010 relevance feedback track (notebook). In The "
+        "Nineteenth TREC Notebook, 2010.). There are 20,232 total (topic, document) examples (noisily) judged by 766 "
+        'workers, who produced a total of 98,453 judgments. 3277 of the examples have prior "gold" labels by NIST.',
+    },
 }
```

### Comparing `crowd-kit-1.2.1/crowdkit/datasets/load_dataset.py` & `crowd-kit-1.3.0rc1/crowdkit/datasets/load_dataset.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 __all__ = [
-    'load_dataset',
-    'get_datasets_list',
+    "load_dataset",
+    "get_datasets_list",
 ]
 
-from typing import Optional, List, Tuple, Callable, Dict, cast
+from typing import Any, Callable, Dict, List, Optional, Tuple, cast
 
 import pandas as pd
 
 from ._loaders import DATA_LOADERS
 
 
-def load_dataset(dataset: str, data_dir: Optional[str] = None) -> Tuple[pd.DataFrame, pd.Series]:
+def load_dataset(
+    dataset: str, data_dir: Optional[str] = None
+) -> Tuple[pd.DataFrame, "pd.Series[Any]"]:
     """Downloads a dataset from remote and loads it into Pandas objects.
     If a dataset is already downloaded, loads it from cache.
 
     Parameters:
         dataset: str, a dataset name
         data_dir: Optional[str]
             Path to folder where to store downloaded dataset. If `None`, `~/crowdkit_data` is used.
             `default=None`. Alternatively, it can be set by the 'CROWDKIT_DATA' environment variable.
     Returns:
         data: Tuple[pd.DataFrame, pd.Series], a tuple of workers answers and ground truth labels.
     """
 
     if dataset not in DATA_LOADERS:
-        raise ValueError('This dataset does not exist')
+        raise ValueError("This dataset does not exist")
 
-    return cast(Dict[str, Callable[[Optional[str]], Tuple[pd.DataFrame, pd.Series]]],
-                DATA_LOADERS[dataset])['loader'](data_dir)
+    return cast(
+        Dict[str, Callable[[Optional[str]], Tuple[pd.DataFrame, "pd.Series[Any]"]]],
+        DATA_LOADERS[dataset],
+    )["loader"](data_dir)
 
 
 def get_datasets_list() -> List[Tuple[str, str]]:
     """Returns a list of available datasets in format [(name, description)]."""
-    return cast(List[Tuple[str, str]],
-                [(dataset, info['description']) for dataset, info in DATA_LOADERS.items()])
+    return cast(
+        List[Tuple[str, str]],
+        [(dataset, info["description"]) for dataset, info in DATA_LOADERS.items()],
+    )
```

### Comparing `crowd-kit-1.2.1/crowdkit/learning/conal.py` & `crowd-kit-1.3.0rc1/crowdkit/learning/conal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Adapted from:
 # https://github.com/zdchu/CoNAL/blob/main/conal.py
 __all__ = [
-    'CoNAL',
+    "CoNAL",
 ]
 
 from typing import Optional, Tuple, Union
-from numpy.typing import NDArray
 
 import numpy as np
 import torch
 import torch.nn.functional as F
+from numpy.typing import NDArray
 from torch import nn
 
 from crowdkit.learning.utils import differentiable_ds
 
 
 def _identity_init(shape: Union[Tuple[int, int], Tuple[int, int, int]]) -> torch.Tensor:
     """
@@ -32,15 +32,15 @@
                 out[r, i, i] = 2.0
     elif len(shape) == 2:
         for i in range(shape[1]):
             out[i, i] = 2.0
     return torch.Tensor(out)
 
 
-class CoNAL(nn.Module):  # type: ignore
+class CoNAL(nn.Module):
     """
     Common Noise Adaptation Layers (CoNAL). This method introduces two types of confusions: worker-specific and
     global. Each is parameterized by a confusion matrix. The ratio of the two confusions is determined by the
     common noise adaptation layer. The common noise adaptation layer is a trainable function that takes the
     instance embedding and the worker ID as input and outputs a scalar value between 0 and 1.
 
     Zhendong Chu, Jing Ma, and Hongning Wang. Learning from Crowds by Modeling Common Confusions.
```

### Comparing `crowd-kit-1.2.1/crowdkit/learning/crowd_layer.py` & `crowd-kit-1.3.0rc1/crowdkit/learning/crowd_layer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __all__ = [
-    'CrowdLayer',
+    "CrowdLayer",
 ]
 
 from typing import Optional
 
 import torch
 from torch import nn
 
@@ -81,15 +81,15 @@
 
     Returns:
         torch.Tensor: Tensor of shape (batch_size, input_dim)
     """
     return scale[workers] * outputs + bias[workers]
 
 
-class CrowdLayer(nn.Module):  # type: ignore
+class CrowdLayer(nn.Module):
     """
     CrowdLayer module for classification tasks.
 
     This method applies a worker-specific transformation of the logits. There are four types of transformations:
     - MW: Multiplication on the worker's confusion matrix.
     - VW: Element-wise multiplication with the worker's weight vector.
     - VB: Element-wise addition with the worker's bias vector.
@@ -128,15 +128,17 @@
         """
         super(CrowdLayer, self).__init__()
         self.conn_type = conn_type
 
         self.n_workers = n_workers
         if conn_type == "mw":
             self.weight = nn.Parameter(
-                batch_identity_matrices(n_workers, num_labels, dtype=dtype, device=device)
+                batch_identity_matrices(
+                    n_workers, num_labels, dtype=dtype, device=device
+                )
             )
         elif conn_type == "vw":
             self.weight = nn.Parameter(
                 torch.ones(n_workers, num_labels, dtype=dtype, device=device)
             )
         elif conn_type == "vb":
             self.weight = nn.Parameter(
```

### Comparing `crowd-kit-1.2.1/crowdkit/learning/text_summarization.py` & `crowd-kit-1.3.0rc1/crowdkit/learning/text_summarization.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 __all__ = [
-    'TextSummarization',
+    "TextSummarization",
 ]
 
 import itertools
-from typing import Optional, cast
+from typing import Any, Iterable, Optional, Union, cast
 
 import attr
 import numpy as np
 import pandas as pd
-from transformers import PreTrainedTokenizer, PreTrainedModel  # type: ignore
+from transformers import PreTrainedModel, PreTrainedTokenizer
 
 from crowdkit.aggregation.base import BaseTextsAggregator
 
 
 @attr.s
 class TextSummarization(BaseTextsAggregator):
     """Text Aggregation through Summarization
@@ -31,88 +31,91 @@
     <https://ceur-ws.org/Vol-2932/short1.pdf>
 
     S. Pletenev,
     "Noisy Text Sequences Aggregation as a Summarization Subtask,"
     Proceedings of the 2nd Crowd Science Workshop: Trust, Ethics, and Excellence in Crowdsourced Data Management at Scale, 2021, pp. 15-20.
     <https://ceur-ws.org/Vol-2932/short2.pdf>
 
-    Args:
-        tokenizer: [Pre-trained tokenizer](https://huggingface.co/transformers/main_classes/tokenizer.html#pretrainedtokenizer).
-        model: [Pre-trained model](https://huggingface.co/transformers/main_classes/model.html#pretrainedmodel) for text summarization.
-        concat_token: Token used for the workers' texts concatenation.
-            Default value: ` | `.
-        num_beams: Number of beams for beam search. 1 means no beam search.
-            Default value: `16`.
-        n_permutations: Number of input permutations to use. If `None`, use a single permutation according to the input's order.
-            Default value: `None`.
-        permutation_aggregator: Text aggregation method to use for aggregating outputs of multiple input permutations if `use_permutations` flag is set.
-            Default value: `None`.
-        device: Device to use such as `cpu` or `cuda`.
-            Default value: `cpu`.
-    Example:
+    Examples:
         >>> import torch
         >>> from transformers import AutoModelForSeq2SeqLM, AutoTokenizer, AutoConfig
         >>> from crowdkit.learning import TextSummarization
         >>> device = 'cuda' if torch.cuda.is_available() else 'cpu'
         >>> mname = "toloka/t5-large-for-text-aggregation"
         >>> tokenizer = AutoTokenizer.from_pretrained(mname)
         >>> model = AutoModelForSeq2SeqLM.from_pretrained(mname)
         >>> agg = TextSummarization(tokenizer, model, device=device)
         >>> result = agg.fit_predict(df)
         ...
-    Attributes:
-        texts_ (Series): Tasks' texts.
-            A pandas.Series indexed by `task` such that `result.loc[task, text]`
-            is the task's text.
     """
+
     tokenizer: PreTrainedTokenizer = attr.ib()
+    """[Pre-trained tokenizer](https://huggingface.co/transformers/main_classes/tokenizer.html#pretrainedtokenizer)."""
+
     model: PreTrainedModel = attr.ib()
-    concat_token: str = attr.ib(default=' | ')
+    """[Pre-trained model](https://huggingface.co/transformers/main_classes/model.html#pretrainedmodel) for text summarization."""
+
+    concat_token: str = attr.ib(default=" | ")
+    """Token used for the workers' texts concatenation."""
+
     num_beams: int = attr.ib(default=16)
+    """Number of beams for beam search. 1 means no beam search."""
+
     n_permutations: Optional[int] = attr.ib(default=None)
+    """Number of input permutations to use. If `None`, use a single permutation according to the input's order."""
+
     permutation_aggregator: Optional[BaseTextsAggregator] = attr.ib(default=None)
-    device: str = attr.ib(default='cpu')
+    """Text aggregation method to use for aggregating outputs of multiple input permutations if `use_permutations` flag is set."""
 
-    # texts_
+    device: str = attr.ib(default="cpu")
+    """Device to use such as `cpu` or `cuda`."""
 
-    def fit_predict(self, data: pd.DataFrame) -> pd.Series:
+    def fit_predict(self, data: pd.DataFrame) -> "pd.Series[Any]":
         """Run the aggregation and return the aggregated texts.
         Args:
             data (DataFrame): Workers' text outputs.
                 A pandas.DataFrame containing `task`, `worker` and `text` columns.
         Returns:
             Series: Tasks' texts.
                 A pandas.Series indexed by `task` such that `result.loc[task, text]`
                 is the task's text.
         """
 
-        data = data[['task', 'worker', 'text']]
+        data = data[["task", "worker", "text"]]
 
-        self.model = self.model.to(self.device)  # type: ignore
-        self.texts_ = data.groupby('task')['text'].apply(self._aggregate_one)
+        self.model = self.model.to(self.device)
+        self.texts_ = data.groupby("task")["text"].apply(self._aggregate_one)
         return self.texts_
 
-    def _aggregate_one(self, outputs: pd.Series) -> str:
+    def _aggregate_one(self, outputs: "pd.Series[Any]") -> str:
         if not self.n_permutations:
             return self._generate_output(outputs)
 
         generated_outputs = []
 
         # TODO: generate only `n_permutations` permutations
         permutations = list(itertools.permutations(outputs))
-        permutations_idx = np.random.choice(len(permutations), size=self.n_permutations, replace=False)
+        permutations_idx = np.random.choice(
+            len(permutations), size=self.n_permutations, replace=False
+        )
         permutations = [permutations[i] for i in permutations_idx]
         for permutation in permutations:
             generated_outputs.append(self._generate_output(permutation))
 
-        data = pd.DataFrame({'task': [''] * len(generated_outputs), 'text': generated_outputs})
+        data = pd.DataFrame(
+            {"task": [""] * len(generated_outputs), "text": generated_outputs}
+        )
 
         if self.permutation_aggregator is not None:
-            return cast(str, self.permutation_aggregator.fit_predict(data)[''])
+            return cast(str, self.permutation_aggregator.fit_predict(data)[""])
 
         return cast(str, data.text.mode())
 
-    def _generate_output(self, permutation: pd.Series) -> str:
+    def _generate_output(
+        self, permutation: Union[Iterable[Any], "pd.Series[Any]"]
+    ) -> str:
         input_text = self.concat_token.join(permutation)
-        input_ids = self.tokenizer.encode(input_text, return_tensors='pt').to(self.device)
-        outputs = self.model.generate(input_ids, num_beams=self.num_beams)  # type: ignore
+        input_ids = self.tokenizer.encode(input_text, return_tensors="pt").to(
+            self.device
+        )
+        outputs = self.model.generate(input_ids, num_beams=self.num_beams)
         return cast(str, self.tokenizer.decode(outputs[0], skip_special_tokens=True))
```

### Comparing `crowd-kit-1.2.1/crowdkit/learning/utils.py` & `crowd-kit-1.3.0rc1/crowdkit/learning/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 __all__ = [
-    'differentiable_ds',
-    'batch_identity_matrices',
+    "differentiable_ds",
+    "batch_identity_matrices",
 ]
 
+from typing import Optional
+
 import torch
 import torch.nn.functional as F
-from typing import Optional
 
 
-def differentiable_ds(outputs: torch.Tensor, confusion_matrices: torch.Tensor) -> torch.Tensor:
+def differentiable_ds(
+    outputs: torch.Tensor, confusion_matrices: torch.Tensor
+) -> torch.Tensor:
     """
     Differentiable Dawid-Skene logit transformation.
     Args:
         outputs (torch.Tensor): Tensor of shape (batch_size, input_dim)
         confusion_matrices (torch.Tensor): Tensor of shape (batch_size, input_dim, input_dim)
 
     Returns:
@@ -25,18 +28,19 @@
             normalized_matrices,
             F.softmax(outputs, dim=-1).unsqueeze(-1),
         ).squeeze()
     )
 
 
 def batch_identity_matrices(
-        batch_size: int,
-        dim_size: int,
-        device: Optional[torch.device] = None,
-        dtype: Optional[torch.dtype] = None) -> torch.Tensor:
+    batch_size: int,
+    dim_size: int,
+    device: Optional[torch.device] = None,
+    dtype: Optional[torch.dtype] = None,
+) -> torch.Tensor:
     """
     Creates a batch of identity matrices.
     Args:
         batch_size (int): Batch size.
         dim_size (int): Dimension size.
         device (torch.device): Device to place the matrices on.
         dtype (torch.dtype): Data type of the matrices.
```

### Comparing `crowd-kit-1.2.1/crowdkit/metrics/data/_classification.py` & `crowd-kit-1.3.0rc1/crowdkit/metrics/data/_classification.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,116 +1,120 @@
 __all__ = [
-    'consistency',
-    'uncertainty',
-    'alpha_krippendorff',
+    "consistency",
+    "uncertainty",
+    "alpha_krippendorff",
 ]
 
-from typing import Any, Callable, Hashable, List, Optional, Tuple, Union
+from typing import Any, Callable, Hashable, List, Optional, Tuple, Union, cast
 
 import numpy as np
 import pandas as pd
 from nltk.metrics.agreement import AnnotationTask
 from nltk.metrics.distance import binary_distance
 from scipy.stats import entropy
 
 from crowdkit.aggregation import MajorityVote
 from crowdkit.aggregation.base import BaseClassificationAggregator
 
 
 def _check_answers(answers: pd.DataFrame) -> None:
     if not isinstance(answers, pd.DataFrame):
-        raise TypeError('Working only with pandas DataFrame')
-    assert 'task' in answers, 'There is no "task" column in answers'
-    assert 'worker' in answers, 'There is no "worker" column in answers'
-    assert 'label' in answers, 'There is no "label" column in answers'
+        raise TypeError("Working only with pandas DataFrame")
+    assert "task" in answers, 'There is no "task" column in answers'
+    assert "worker" in answers, 'There is no "worker" column in answers'
+    assert "label" in answers, 'There is no "label" column in answers'
 
 
-def _label_probability(row: pd.Series, label: Any, n_labels: int) -> float:
+def _label_probability(row: "pd.Series[Any]", label: Any, n_labels: int) -> float:
     """Numerator in the Bayes formula"""
-    if row['label'] == label:
-        return float(row['skill'])
+    if row["label"] == label:
+        return float(row["skill"])
     else:
-        return (1. - float(row['skill'])) / (n_labels - 1)
+        return (1.0 - float(row["skill"])) / (n_labels - 1)
 
 
-def _task_consistency(row: pd.Series) -> float:
+def _task_consistency(row: "pd.Series[Any]") -> float:
     """Posterior probability for a single task"""
-    if row['denominator'] != 0:
-        return float(row[row['aggregated_label']]) / float(row['denominator'])
+    if row["denominator"] != 0:
+        return float(row[row["aggregated_label"]]) / float(row["denominator"])
     else:
-        return 0.
+        return 0.0
 
 
 def consistency(
-        answers: pd.DataFrame,
-        workers_skills: Optional[pd.Series] = None,
-        aggregator: BaseClassificationAggregator = MajorityVote(),
-        by_task: bool = False
-) -> Union[float, pd.Series]:
+    answers: pd.DataFrame,
+    workers_skills: Optional["pd.Series[Any]"] = None,
+    aggregator: BaseClassificationAggregator = MajorityVote(),
+    by_task: bool = False,
+) -> Union[float, "pd.Series[Any]"]:
     """
     Consistency metric: posterior probability of aggregated label given workers skills
-    calculated using standard Dawid-Skene model.
+    calculated using the standard Dawid-Skene model.
 
     Args:
         answers (pandas.DataFrame): A data frame containing `task`, `worker` and `label` columns.
         workers_skills (Optional[pandas.Series]): workers skills e.g. golden set skills. If not provided,
             uses aggregator's `workers_skills` attribute.
         aggregator (aggregation.base.BaseClassificationAggregator): aggregation method, default: MajorityVote
         by_task (bool): if set, returns consistencies for every task in provided data frame.
 
     Returns:
         Union[float, pd.Series]
     """
     _check_answers(answers)
     aggregated = aggregator.fit_predict(answers)
     if workers_skills is None:
-        if hasattr(aggregator, 'skills_'):
-            workers_skills = aggregator.skills_  # type: ignore
+        if hasattr(aggregator, "skills_"):
+            workers_skills = aggregator.skills_
         else:
-            raise AssertionError('This aggregator is not supported. Please, provide workers skills.')
+            raise AssertionError(
+                "This aggregator is not supported. Please, provide workers skills."
+            )
 
     answers = answers.copy(deep=False)
-    answers.set_index('task', inplace=True)
-    answers = answers.reset_index().set_index('worker')
-    answers['skill'] = workers_skills
+    answers.set_index("task", inplace=True)
+    answers = answers.reset_index().set_index("worker")
+    answers["skill"] = workers_skills
     answers.reset_index(inplace=True)
 
     labels = pd.unique(answers.label)
     for label in labels:
-        answers[label] = answers.apply(lambda row: _label_probability(row, label, len(labels)), axis=1)
-
-    labels_proba = answers.groupby('task').prod(numeric_only=True)
-    labels_proba['aggregated_label'] = aggregated
-    labels_proba['denominator'] = labels_proba[list(labels)].sum(axis=1)
+        answers[label] = answers.apply(
+            lambda row: _label_probability(row, label, len(labels)), axis=1
+        )
+
+    labels_proba = answers.groupby("task").prod(numeric_only=True)
+    labels_proba["aggregated_label"] = aggregated
+    labels_proba["denominator"] = labels_proba[list(labels)].sum(axis=1)
 
     consistencies = labels_proba.apply(_task_consistency, axis=1)
 
     if by_task:
         return consistencies
     else:
         return consistencies.mean()
 
 
-def _task_uncertainty(row: pd.Series, labels: List[Hashable]) -> float:
-    if row['denominator'] == 0:
+def _task_uncertainty(row: "pd.Series[Any]", labels: List[str]) -> float:
+    if row["denominator"] == 0:
         row[labels] = 1 / len(labels)
     else:
-        row[labels] /= row['denominator']
+        row[labels] /= row["denominator"]
     softmax = row[labels]
     log_softmax = np.log(row[list(labels)])
     return float(-np.sum(softmax * log_softmax))
 
 
 def uncertainty(
-        answers: pd.DataFrame,
-        workers_skills: Optional[pd.Series] = None,
-        aggregator: Optional[BaseClassificationAggregator] = None,
-        compute_by: str = 'task',
-        aggregate: bool = True
-) -> Union[float, pd.Series]:
+    answers: pd.DataFrame,
+    workers_skills: Optional["pd.Series[Any]"] = None,
+    aggregator: Optional[BaseClassificationAggregator] = None,
+    compute_by: str = "task",
+    aggregate: bool = True,
+) -> Union[float, "pd.Series[Any]"]:
     r"""Label uncertainty metric: entropy of labels probability distribution.
     Computed as Shannon's Entropy with label probabilities computed either for tasks or workers:
     $$H(L) = -\sum_{label_i \in L} p(label_i) \cdot \log(p(label_i))$$
 
     Args:
         answers: A data frame containing `task`, `worker` and `label` columns.
         workers_skills: workers skills e.g. golden set skills. If not provided,
@@ -179,40 +183,52 @@
         workers_skills (typing.Optional[pandas.core.series.Series]): workers' skills.
             A pandas.Series index by workers and holding corresponding worker's skill
     """
     _check_answers(answers)
 
     if workers_skills is None and aggregator is not None:
         aggregator.fit(answers)
-        if hasattr(aggregator, 'skills_'):
-            workers_skills = aggregator.skills_  # type: ignore
+        if hasattr(aggregator, "skills_"):
+            workers_skills = aggregator.skills_
         else:
-            raise AssertionError('This aggregator is not supported. Please, provide workers skills.')
+            raise AssertionError(
+                "This aggregator is not supported. Please, provide workers skills."
+            )
 
     answers = answers.copy(deep=False)
-    answers = answers.set_index('worker')
-    answers['skill'] = workers_skills if workers_skills is not None else 1
-    if answers['skill'].isnull().any():
+    answers = answers.set_index("worker")
+    answers["skill"] = workers_skills if workers_skills is not None else 1
+    if answers["skill"].isnull().any():
         missing_workers = set(answers[answers.skill.isnull()].index.tolist())
-        raise AssertionError(f'Did not provide skills for workers: {missing_workers}.'
-                             f'Please provide workers skills.')
+        raise AssertionError(
+            f"Did not provide skills for workers: {missing_workers}."
+            f"Please provide workers skills."
+        )
     answers.reset_index(inplace=True)
     labels = pd.unique(answers.label)
     for label in labels:
-        answers[label] = answers.apply(lambda row: _label_probability(row, label, len(labels)), axis=1)
+        answers[label] = answers.apply(
+            lambda row: _label_probability(row, label, len(labels)), axis=1
+        )
 
     labels_proba = answers.groupby(compute_by).sum(numeric_only=True)
-    uncertainties = labels_proba.apply(lambda row: entropy(row[labels] / (sum(row[labels]) + 1e-6)), axis=1)
+    uncertainties = labels_proba.apply(
+        lambda row: entropy(row[labels] / (sum(row[labels]) + 1e-6)), axis=1
+    )
+
     if aggregate:
-        return uncertainties.mean()
-    return uncertainties
+        return cast(float, uncertainties.mean())
+
+    return cast("pd.Series[Any]", uncertainties)
 
 
-def alpha_krippendorff(answers: pd.DataFrame,
-                       distance: Callable[[Hashable, Hashable], float] = binary_distance) -> float:
+def alpha_krippendorff(
+    answers: pd.DataFrame,
+    distance: Callable[[Hashable, Hashable], float] = binary_distance,
+) -> float:
     """Inter-annotator agreement coefficient (Krippendorff 1980).
 
     Amount that annotators agreed on label assignments beyond what is expected by chance.
     The value of alpha should be interpreted as follows.
         alpha >= 0.8 indicates a reliable annotation,
         alpha >= 0.667 allows making tentative conclusions only,
         while the lower values suggest the unreliable annotation.
@@ -246,9 +262,11 @@
         >>>     {'task': 'Y', 'worker': 'B', 'label': 'No'},
         >>>     {'task': 'Z', 'worker': 'A', 'label': 'Yes'},
         >>>     {'task': 'Z', 'worker': 'B', 'label': 'No'},
         >>> ]))
         0.4444444444444444
     """
     _check_answers(answers)
-    data: List[Tuple[Any, Hashable, Hashable]] = answers[['worker', 'task', 'label']].values.tolist()
+    data: List[Tuple[Any, Hashable, Hashable]] = answers[
+        ["worker", "task", "label"]
+    ].values.tolist()
     return float(AnnotationTask(data, distance).alpha())
```

### Comparing `crowd-kit-1.2.1/crowdkit/metrics/workers/accuracy_on_aggregates.py` & `crowd-kit-1.3.0rc1/crowdkit/metrics/workers/accuracy_on_aggregates.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 __all__ = [
-    'accuracy_on_aggregates',
+    "accuracy_on_aggregates",
 ]
 
-from typing import Optional, Union
+from typing import Any, Optional, Union
 
 import pandas as pd
 
 from crowdkit.aggregation import MajorityVote
 from crowdkit.aggregation.base import BaseClassificationAggregator
 from crowdkit.aggregation.utils import get_accuracy
 
 
 def accuracy_on_aggregates(
-        answers: pd.DataFrame,
-        aggregator: Optional[BaseClassificationAggregator] = MajorityVote(),
-        aggregates: Optional[pd.Series] = None,
-        by: Optional[str] = None
-) -> Union[float, pd.Series]:
+    answers: pd.DataFrame,
+    aggregator: Optional[BaseClassificationAggregator] = MajorityVote(),
+    aggregates: Optional["pd.Series[Any]"] = None,
+    by: Optional[str] = None,
+) -> Union[float, "pd.Series[Any]"]:
     """
     Accuracy on aggregates: a fraction of worker's answers that match the aggregated one.
 
     Args:
         answers: a data frame containing `task`, `worker` and `label` columns.
         aggregator: aggregation algorithm. default: MajorityVote
         aggregates: aggregated answers for provided tasks.
         by: if set, returns accuracies for every worker in provided data frame. Otherwise,
             returns an average accuracy of all workers.
 
         Returns:
             Union[float, pd.Series]
     """
     if aggregates is None and aggregator is None:
-        raise AssertionError('One of aggregator or aggregates should be not None')
+        raise AssertionError("One of aggregator or aggregates should be not None")
 
     if aggregates is None:
         aggregates = aggregator.fit_predict(answers)  # type: ignore
 
     return get_accuracy(answers, aggregates, by=by)
```

### Comparing `crowd-kit-1.2.1/crowdkit/postprocessing/entropy_threshold.py` & `crowd-kit-1.3.0rc1/crowdkit/postprocessing/entropy_threshold.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 __all__ = [
-    'entropy_threshold',
+    "entropy_threshold",
 ]
 
 import warnings
-from typing import Optional, cast
+from typing import Any, Optional, cast
 
 import numpy as np
 import pandas as pd
 
 from ..metrics.data import uncertainty
 
 
 def entropy_threshold(
-        answers: pd.DataFrame,
-        workers_skills: Optional[pd.Series] = None,
-        percentile: int = 10,
-        min_answers: int = 2,
+    answers: pd.DataFrame,
+    workers_skills: Optional["pd.Series[Any]"] = None,
+    percentile: int = 10,
+    min_answers: int = 2,
 ) -> pd.DataFrame:
     """Entropy thresholding postprocessing: filters out all answers by workers,
     whos' entropy (uncertanity) of answers is below specified percentile.
 
     This heuristic detects answers of workers that answer the same way too often, e.g. when "speed-running" by only
     clicking one button.
 
@@ -54,31 +54,38 @@
     Args:
         answers (DataFrame): Workers' labeling results.
             A pandas.DataFrame containing `task`, `worker` and `label` columns.
         workers_skills (typing.Optional[pandas.core.series.Series]): workers' skills.
             A pandas.Series index by workers and holding corresponding worker's skill
     """
 
-    answers_per_worker = answers.groupby('worker')['label'].count()
+    answers_per_worker = answers.groupby("worker")["label"].count()
     answers_per_worker = answers_per_worker[answers_per_worker >= min_answers]
 
     answers_for_filtration = answers[answers.worker.isin(answers_per_worker.index)]
 
-    uncertainties = cast(pd.Series, uncertainty(
-        answers_for_filtration,
-        workers_skills,
-        compute_by='worker',
-        aggregate=False,
-    ))
+    uncertainties = cast(
+        "pd.Series[Any]",
+        uncertainty(
+            answers_for_filtration,
+            workers_skills,
+            compute_by="worker",
+            aggregate=False,
+        ),
+    )
 
-    cutoff = np.percentile(uncertainties, percentile)  # type: ignore
+    cutoff = np.percentile(uncertainties, percentile)
 
     removed_workers = uncertainties[uncertainties <= cutoff].index
 
     filtered_answers = answers.copy(deep=False)
-    filtered_answers = filtered_answers[~filtered_answers['worker'].isin(removed_workers)]
+    filtered_answers = filtered_answers[
+        ~filtered_answers["worker"].isin(removed_workers)
+    ]
 
     if filtered_answers.shape[0] <= answers.shape[0] // 2:
-        warnings.warn('Removed >= 1/2 of answers with entropy_threshold. This might lead to poor annotation quality. '
-                      'Try decreasing percentile or min_answers.')
+        warnings.warn(
+            "Removed >= 1/2 of answers with entropy_threshold. This might lead to poor annotation quality. "
+            "Try decreasing percentile or min_answers."
+        )
 
     return filtered_answers
```

### Comparing `crowd-kit-1.2.1/tests/test_utils.py` & `crowd-kit-1.3.0rc1/tests/test_utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,91 +1,99 @@
 import pandas as pd
-
-from crowdkit.aggregation.utils import get_most_probable_labels, get_accuracy, normalize_rows
 from pandas.testing import assert_frame_equal, assert_series_equal
 
+from crowdkit.aggregation.utils import (
+    get_accuracy,
+    get_most_probable_labels,
+    normalize_rows,
+)
+
 
 def test_get_most_probable_labels() -> None:
     proba = pd.DataFrame(
         [
             [0.9, 0.1, 0.0],
             [0.3, 0.5, 0.2],
             [0.1, 0.2, 0.7],
             [0.5, 0.4, 0.1],
         ],
-        columns=['a', 'b', 'c'],
-        index=['w', 'x', 'y', 'z'],
+        columns=["a", "b", "c"],
+        index=["w", "x", "y", "z"],
     )
 
     most_probable_labels = pd.Series(
-        ['a', 'b', 'c', 'a'],
-        index=['w', 'x', 'y', 'z'],
+        ["a", "b", "c", "a"],
+        index=["w", "x", "y", "z"],
     )
 
     assert_series_equal(get_most_probable_labels(proba), most_probable_labels)
 
 
 def test_normalize_rows() -> None:
     scores = pd.DataFrame(
         [
             [4.5, 0.5, 0.0],
             [0.6, 1.0, 0.4],
             [0.3, 0.6, 2.1],
             [3.5, 2.8, 0.7],
         ],
-        columns=['a', 'b', 'c'],
-        index=['w', 'x', 'y', 'z'],
+        columns=["a", "b", "c"],
+        index=["w", "x", "y", "z"],
     )
 
     proba = pd.DataFrame(
         [
             [0.9, 0.1, 0.0],
             [0.3, 0.5, 0.2],
             [0.1, 0.2, 0.7],
             [0.5, 0.4, 0.1],
         ],
-        columns=['a', 'b', 'c'],
-        index=['w', 'x', 'y', 'z'],
+        columns=["a", "b", "c"],
+        index=["w", "x", "y", "z"],
     )
 
     assert_frame_equal(normalize_rows(scores), proba)
 
 
 def test_get_accuracy() -> None:
-    true_labels = pd.Series({'t1': 'c', 't2': 'b'})
+    true_labels = pd.Series({"t1": "c", "t2": "b"})
     data = pd.DataFrame(
         [
-            ['t1', 'p1', 'a', 1],
-            ['t1', 'p2', 'a', 1],
-            ['t1', 'p3', 'c', 3],
-            ['t2', 'p1', 'b', 2],
-            ['t2', 'p4', 'b', 1],
-            ['t2', 'p3', 'c', 1],
+            ["t1", "p1", "a", 1],
+            ["t1", "p2", "a", 1],
+            ["t1", "p3", "c", 3],
+            ["t2", "p1", "b", 2],
+            ["t2", "p4", "b", 1],
+            ["t2", "p3", "c", 1],
         ],
-        columns=['task', 'worker', 'label', 'weight']
+        columns=["task", "worker", "label", "weight"],
     )
 
     # With weights
     assert get_accuracy(data, true_labels) == 6 / 9
 
-    skills = pd.Series([3/5, 3/4], index=pd.Index(['t1', 't2'], name='task'))
-    assert_series_equal(get_accuracy(data, true_labels, by='task'), skills)
+    skills = pd.Series([3 / 5, 3 / 4], index=pd.Index(["t1", "t2"], name="task"))
+    assert_series_equal(get_accuracy(data, true_labels, by="task"), skills)
 
-    skills = pd.Series([2/3, 0, 3/4, 1], index=pd.Index(['p1', 'p2', 'p3', 'p4'], name='worker'))
-    assert_series_equal(get_accuracy(data, true_labels, by='worker'), skills)
+    skills = pd.Series(
+        [2 / 3, 0, 3 / 4, 1], index=pd.Index(["p1", "p2", "p3", "p4"], name="worker")
+    )
+    assert_series_equal(get_accuracy(data, true_labels, by="worker"), skills)
 
-    skills = pd.Series([3/4, 3/5], index=pd.Index(['b', 'c'], name='true_label'))
-    assert_series_equal(get_accuracy(data, true_labels, by='true_label'), skills)
+    skills = pd.Series([3 / 4, 3 / 5], index=pd.Index(["b", "c"], name="true_label"))
+    assert_series_equal(get_accuracy(data, true_labels, by="true_label"), skills)
 
     # Without weights
-    data = data[['task', 'worker', 'label']]
+    data = data[["task", "worker", "label"]]
 
     assert get_accuracy(data, true_labels) == 1 / 2
 
-    skills = pd.Series([1/3, 2/3], index=pd.Index(['t1', 't2'], name='task'))
-    assert_series_equal(get_accuracy(data, true_labels, by='task'), skills)
+    skills = pd.Series([1 / 3, 2 / 3], index=pd.Index(["t1", "t2"], name="task"))
+    assert_series_equal(get_accuracy(data, true_labels, by="task"), skills)
 
-    skills = pd.Series([1/2, 0, 1/2, 1], index=pd.Index(['p1', 'p2', 'p3', 'p4'], name='worker'))
-    assert_series_equal(get_accuracy(data, true_labels, by='worker'), skills)
+    skills = pd.Series(
+        [1 / 2, 0, 1 / 2, 1], index=pd.Index(["p1", "p2", "p3", "p4"], name="worker")
+    )
+    assert_series_equal(get_accuracy(data, true_labels, by="worker"), skills)
 
-    skills = pd.Series([2/3, 1/3], index=pd.Index(['b', 'c'], name='true_label'))
-    assert_series_equal(get_accuracy(data, true_labels, by='true_label'), skills)
+    skills = pd.Series([2 / 3, 1 / 3], index=pd.Index(["b", "c"], name="true_label"))
+    assert_series_equal(get_accuracy(data, true_labels, by="true_label"), skills)
```

