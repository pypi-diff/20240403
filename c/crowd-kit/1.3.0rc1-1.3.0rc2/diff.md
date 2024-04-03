# Comparing `tmp/crowd-kit-1.3.0rc1.tar.gz` & `tmp/crowd-kit-1.3.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crowd-kit-1.3.0rc1.tar", last modified: Wed Apr  3 09:17:49 2024, max compression
+gzip compressed data, was "crowd-kit-1.3.0rc2.tar", last modified: Wed Apr  3 11:00:26 2024, max compression
```

## Comparing `crowd-kit-1.3.0rc1.tar` & `crowd-kit-1.3.0rc2.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:17:49.253433 crowd-kit-1.3.0rc1/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9608 2024-04-03 09:17:49.253433 crowd-kit-1.3.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:17:49.253433 crowd-kit-1.3.0rc1/crowd_kit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9608 2024-04-03 09:17:49.000000 crowd-kit-1.3.0rc1/crowd_kit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-03 09:17:49.000000 crowd-kit-1.3.0rc1/crowd_kit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 09:17:49.000000 crowd-kit-1.3.0rc1/crowd_kit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-03 09:17:49.000000 crowd-kit-1.3.0rc1/crowd_kit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 09:17:49.000000 crowd-kit-1.3.0rc1/crowd_kit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 09:07:49.000000 crowd-kit-1.3.0rc1/crowd_kit.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:17:49.241433 crowd-kit-1.3.0rc1/crowdkit/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:17:49.241433 crowd-kit-1.3.0rc1/crowdkit/aggregation/
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:17:49.245433 crowd-kit-1.3.0rc1/crowdkit/aggregation/base/
--rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/base/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:17:49.245433 crowd-kit-1.3.0rc1/crowdkit/aggregation/classification/
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15945 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/classification/dawid_skene.py
--rw-r--r--   0 runner    (1001) docker     (127)    16746 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/classification/glad.py
--rw-r--r--   0 runner    (1001) docker     (127)     7368 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/classification/gold_majority_vote.py
--rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/classification/kos.py
--rw-r--r--   0 runner    (1001) docker     (127)    13828 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/classification/m_msr.py
--rw-r--r--   0 runner    (1001) docker     (127)    17697 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/classification/mace.py
--rw-r--r--   0 runner    (1001) docker     (127)     6139 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/classification/majority_vote.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/classification/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/classification/wawa.py
--rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/classification/zero_based_skill.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:17:49.245433 crowd-kit-1.3.0rc1/crowdkit/aggregation/embeddings/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5843 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/embeddings/closest_to_average.py
--rw-r--r--   0 runner    (1001) docker     (127)    17967 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/embeddings/hrrasa.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/embeddings/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     8770 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/embeddings/rasa.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:17:49.245433 crowd-kit-1.3.0rc1/crowdkit/aggregation/image_segmentation/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/image_segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/image_segmentation/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9098 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/image_segmentation/segmentation_em.py
--rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/image_segmentation/segmentation_majority_vote.py
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/image_segmentation/segmentation_rasa.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:17:49.245433 crowd-kit-1.3.0rc1/crowdkit/aggregation/multilabel/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/multilabel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/multilabel/binary_relevance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:17:49.249433 crowd-kit-1.3.0rc1/crowdkit/aggregation/pairwise/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/pairwise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5118 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/pairwise/bradley_terry.py
--rw-r--r--   0 runner    (1001) docker     (127)     8719 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/pairwise/noisy_bt.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/pairwise/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:17:49.249433 crowd-kit-1.3.0rc1/crowdkit/aggregation/texts/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/texts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/texts/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9549 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/texts/rover.py
--rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/texts/text_hrrasa.py
--rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/texts/text_rasa.py
--rw-r--r--   0 runner    (1001) docker     (127)     8681 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/aggregation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:17:49.249433 crowd-kit-1.3.0rc1/crowdkit/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/datasets/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    14474 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/datasets/_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/datasets/load_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/datasets/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:17:49.249433 crowd-kit-1.3.0rc1/crowdkit/learning/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/learning/conal.py
--rw-r--r--   0 runner    (1001) docker     (127)     6317 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/learning/crowd_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/learning/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/learning/text_summarization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/learning/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:17:49.249433 crowd-kit-1.3.0rc1/crowdkit/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:17:49.249433 crowd-kit-1.3.0rc1/crowdkit/metrics/data/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/metrics/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10237 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/metrics/data/_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/metrics/data/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:17:49.249433 crowd-kit-1.3.0rc1/crowdkit/metrics/workers/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/metrics/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/metrics/workers/accuracy_on_aggregates.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/metrics/workers/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:17:49.253433 crowd-kit-1.3.0rc1/crowdkit/postprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/postprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/postprocessing/entropy_threshold.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/postprocessing/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/crowdkit/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 09:17:49.253433 crowd-kit-1.3.0rc1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       62 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:17:49.253433 crowd-kit-1.3.0rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-03 09:07:38.000000 crowd-kit-1.3.0rc1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:00:26.856519 crowd-kit-1.3.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9608 2024-04-03 11:00:26.856519 crowd-kit-1.3.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:00:26.852518 crowd-kit-1.3.0rc2/crowd_kit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9608 2024-04-03 11:00:26.000000 crowd-kit-1.3.0rc2/crowd_kit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-03 11:00:26.000000 crowd-kit-1.3.0rc2/crowd_kit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 11:00:26.000000 crowd-kit-1.3.0rc2/crowd_kit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-03 11:00:26.000000 crowd-kit-1.3.0rc2/crowd_kit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 11:00:26.000000 crowd-kit-1.3.0rc2/crowd_kit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 10:57:51.000000 crowd-kit-1.3.0rc2/crowd_kit.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:00:26.844518 crowd-kit-1.3.0rc2/crowdkit/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:00:26.844518 crowd-kit-1.3.0rc2/crowdkit/aggregation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/aggregation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:00:26.844518 crowd-kit-1.3.0rc2/crowdkit/aggregation/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/aggregation/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/aggregation/base/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:00:26.848518 crowd-kit-1.3.0rc2/crowdkit/aggregation/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/aggregation/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15945 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/aggregation/classification/dawid_skene.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16746 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/aggregation/classification/glad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7368 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/aggregation/classification/gold_majority_vote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/aggregation/classification/kos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13828 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/aggregation/classification/m_msr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17697 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/aggregation/classification/mace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6139 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/aggregation/classification/majority_vote.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/aggregation/classification/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/aggregation/classification/wawa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/aggregation/classification/zero_based_skill.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:00:26.848518 crowd-kit-1.3.0rc2/crowdkit/aggregation/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/aggregation/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5843 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/aggregation/embeddings/closest_to_average.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17967 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/aggregation/embeddings/hrrasa.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/aggregation/embeddings/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     8770 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/aggregation/embeddings/rasa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:00:26.848518 crowd-kit-1.3.0rc2/crowdkit/aggregation/image_segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/aggregation/image_segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/aggregation/image_segmentation/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9098 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/aggregation/image_segmentation/segmentation_em.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/aggregation/image_segmentation/segmentation_majority_vote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/aggregation/image_segmentation/segmentation_rasa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:00:26.848518 crowd-kit-1.3.0rc2/crowdkit/aggregation/multilabel/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/aggregation/multilabel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/aggregation/multilabel/binary_relevance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:00:26.848518 crowd-kit-1.3.0rc2/crowdkit/aggregation/pairwise/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/aggregation/pairwise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5118 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/aggregation/pairwise/bradley_terry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8719 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/aggregation/pairwise/noisy_bt.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/aggregation/pairwise/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/aggregation/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:00:26.848518 crowd-kit-1.3.0rc2/crowdkit/aggregation/texts/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/aggregation/texts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/aggregation/texts/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9549 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/aggregation/texts/rover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/aggregation/texts/text_hrrasa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/aggregation/texts/text_rasa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8681 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/aggregation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:00:26.852518 crowd-kit-1.3.0rc2/crowdkit/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/datasets/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14474 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/datasets/_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/datasets/load_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/datasets/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:00:26.852518 crowd-kit-1.3.0rc2/crowdkit/learning/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/learning/conal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6317 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/learning/crowd_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/learning/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/learning/text_summarization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/learning/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:00:26.852518 crowd-kit-1.3.0rc2/crowdkit/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:00:26.852518 crowd-kit-1.3.0rc2/crowdkit/metrics/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/metrics/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10237 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/metrics/data/_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/metrics/data/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:00:26.852518 crowd-kit-1.3.0rc2/crowdkit/metrics/workers/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/metrics/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/metrics/workers/accuracy_on_aggregates.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/metrics/workers/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:00:26.852518 crowd-kit-1.3.0rc2/crowdkit/postprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/postprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/postprocessing/entropy_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/postprocessing/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/crowdkit/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 11:00:26.856519 crowd-kit-1.3.0rc2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       62 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:00:26.852518 crowd-kit-1.3.0rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-03 10:57:42.000000 crowd-kit-1.3.0rc2/tests/test_utils.py
```

### Comparing `crowd-kit-1.3.0rc1/CONTRIBUTING.md` & `crowd-kit-1.3.0rc2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `crowd-kit-1.3.0rc1/LICENSE` & `crowd-kit-1.3.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `crowd-kit-1.3.0rc1/PKG-INFO` & `crowd-kit-1.3.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crowd-kit
-Version: 1.3.0rc1
+Version: 1.3.0rc2
 Summary: Computational Quality Control for Crowdsourcing
 Author: Toloka
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/Toloka/crowd-kit
 Project-URL: Bug Tracker, https://github.com/Toloka/crowd-kit/issues
 Project-URL: Documentation, https://toloka.ai/en/docs/crowd-kit/
 Project-URL: API Reference, https://toloka.ai/en/docs/crowd-kit/
```

### Comparing `crowd-kit-1.3.0rc1/README.md` & `crowd-kit-1.3.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `crowd-kit-1.3.0rc1/crowd_kit.egg-info/PKG-INFO` & `crowd-kit-1.3.0rc2/crowd_kit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crowd-kit
-Version: 1.3.0rc1
+Version: 1.3.0rc2
 Summary: Computational Quality Control for Crowdsourcing
 Author: Toloka
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/Toloka/crowd-kit
 Project-URL: Bug Tracker, https://github.com/Toloka/crowd-kit/issues
 Project-URL: Documentation, https://toloka.ai/en/docs/crowd-kit/
 Project-URL: API Reference, https://toloka.ai/en/docs/crowd-kit/
```

### Comparing `crowd-kit-1.3.0rc1/crowd_kit.egg-info/SOURCES.txt` & `crowd-kit-1.3.0rc2/crowd_kit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crowd-kit-1.3.0rc1/crowdkit/aggregation/__init__.py` & `crowd-kit-1.3.0rc2/crowdkit/aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `crowd-kit-1.3.0rc1/crowdkit/aggregation/base/__init__.py` & `crowd-kit-1.3.0rc2/crowdkit/aggregation/base/__init__.py`

 * *Files identical despite different names*

### Comparing `crowd-kit-1.3.0rc1/crowdkit/aggregation/classification/__init__.py` & `crowd-kit-1.3.0rc2/crowdkit/aggregation/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `crowd-kit-1.3.0rc1/crowdkit/aggregation/classification/dawid_skene.py` & `crowd-kit-1.3.0rc2/crowdkit/aggregation/classification/dawid_skene.py`

 * *Files identical despite different names*

### Comparing `crowd-kit-1.3.0rc1/crowdkit/aggregation/classification/glad.py` & `crowd-kit-1.3.0rc2/crowdkit/aggregation/classification/glad.py`

 * *Files identical despite different names*

### Comparing `crowd-kit-1.3.0rc1/crowdkit/aggregation/classification/gold_majority_vote.py` & `crowd-kit-1.3.0rc2/crowdkit/aggregation/classification/gold_majority_vote.py`

 * *Files identical despite different names*

### Comparing `crowd-kit-1.3.0rc1/crowdkit/aggregation/classification/kos.py` & `crowd-kit-1.3.0rc2/crowdkit/aggregation/classification/kos.py`

 * *Files identical despite different names*

### Comparing `crowd-kit-1.3.0rc1/crowdkit/aggregation/classification/m_msr.py` & `crowd-kit-1.3.0rc2/crowdkit/aggregation/classification/m_msr.py`

 * *Files identical despite different names*

### Comparing `crowd-kit-1.3.0rc1/crowdkit/aggregation/classification/mace.py` & `crowd-kit-1.3.0rc2/crowdkit/aggregation/classification/mace.py`

 * *Files identical despite different names*

### Comparing `crowd-kit-1.3.0rc1/crowdkit/aggregation/classification/majority_vote.py` & `crowd-kit-1.3.0rc2/crowdkit/aggregation/classification/majority_vote.py`

 * *Files identical despite different names*

### Comparing `crowd-kit-1.3.0rc1/crowdkit/aggregation/classification/wawa.py` & `crowd-kit-1.3.0rc2/crowdkit/aggregation/classification/wawa.py`

 * *Files identical despite different names*

### Comparing `crowd-kit-1.3.0rc1/crowdkit/aggregation/classification/zero_based_skill.py` & `crowd-kit-1.3.0rc2/crowdkit/aggregation/classification/zero_based_skill.py`

 * *Files identical despite different names*

### Comparing `crowd-kit-1.3.0rc1/crowdkit/aggregation/embeddings/closest_to_average.py` & `crowd-kit-1.3.0rc2/crowdkit/aggregation/embeddings/closest_to_average.py`

 * *Files identical despite different names*

### Comparing `crowd-kit-1.3.0rc1/crowdkit/aggregation/embeddings/hrrasa.py` & `crowd-kit-1.3.0rc2/crowdkit/aggregation/embeddings/hrrasa.py`

 * *Files identical despite different names*

### Comparing `crowd-kit-1.3.0rc1/crowdkit/aggregation/embeddings/rasa.py` & `crowd-kit-1.3.0rc2/crowdkit/aggregation/embeddings/rasa.py`

 * *Files identical despite different names*

### Comparing `crowd-kit-1.3.0rc1/crowdkit/aggregation/image_segmentation/segmentation_em.py` & `crowd-kit-1.3.0rc2/crowdkit/aggregation/image_segmentation/segmentation_em.py`

 * *Files identical despite different names*

### Comparing `crowd-kit-1.3.0rc1/crowdkit/aggregation/image_segmentation/segmentation_majority_vote.py` & `crowd-kit-1.3.0rc2/crowdkit/aggregation/image_segmentation/segmentation_majority_vote.py`

 * *Files identical despite different names*

### Comparing `crowd-kit-1.3.0rc1/crowdkit/aggregation/image_segmentation/segmentation_rasa.py` & `crowd-kit-1.3.0rc2/crowdkit/aggregation/image_segmentation/segmentation_rasa.py`

 * *Files identical despite different names*

### Comparing `crowd-kit-1.3.0rc1/crowdkit/aggregation/multilabel/binary_relevance.py` & `crowd-kit-1.3.0rc2/crowdkit/aggregation/multilabel/binary_relevance.py`

 * *Files identical despite different names*

### Comparing `crowd-kit-1.3.0rc1/crowdkit/aggregation/pairwise/bradley_terry.py` & `crowd-kit-1.3.0rc2/crowdkit/aggregation/pairwise/bradley_terry.py`

 * *Files identical despite different names*

### Comparing `crowd-kit-1.3.0rc1/crowdkit/aggregation/pairwise/noisy_bt.py` & `crowd-kit-1.3.0rc2/crowdkit/aggregation/pairwise/noisy_bt.py`

 * *Files identical despite different names*

### Comparing `crowd-kit-1.3.0rc1/crowdkit/aggregation/texts/rover.py` & `crowd-kit-1.3.0rc2/crowdkit/aggregation/texts/rover.py`

 * *Files identical despite different names*

### Comparing `crowd-kit-1.3.0rc1/crowdkit/aggregation/texts/text_hrrasa.py` & `crowd-kit-1.3.0rc2/crowdkit/aggregation/texts/text_hrrasa.py`

 * *Files identical despite different names*

### Comparing `crowd-kit-1.3.0rc1/crowdkit/aggregation/texts/text_rasa.py` & `crowd-kit-1.3.0rc2/crowdkit/aggregation/texts/text_rasa.py`

 * *Files identical despite different names*

### Comparing `crowd-kit-1.3.0rc1/crowdkit/aggregation/utils.py` & `crowd-kit-1.3.0rc2/crowdkit/aggregation/utils.py`

 * *Files identical despite different names*

### Comparing `crowd-kit-1.3.0rc1/crowdkit/datasets/_base.py` & `crowd-kit-1.3.0rc2/crowdkit/datasets/_base.py`

 * *Files identical despite different names*

### Comparing `crowd-kit-1.3.0rc1/crowdkit/datasets/_loaders.py` & `crowd-kit-1.3.0rc2/crowdkit/datasets/_loaders.py`

 * *Files identical despite different names*

### Comparing `crowd-kit-1.3.0rc1/crowdkit/datasets/load_dataset.py` & `crowd-kit-1.3.0rc2/crowdkit/datasets/load_dataset.py`

 * *Files identical despite different names*

### Comparing `crowd-kit-1.3.0rc1/crowdkit/learning/conal.py` & `crowd-kit-1.3.0rc2/crowdkit/learning/conal.py`

 * *Files identical despite different names*

### Comparing `crowd-kit-1.3.0rc1/crowdkit/learning/crowd_layer.py` & `crowd-kit-1.3.0rc2/crowdkit/learning/crowd_layer.py`

 * *Files identical despite different names*

### Comparing `crowd-kit-1.3.0rc1/crowdkit/learning/text_summarization.py` & `crowd-kit-1.3.0rc2/crowdkit/learning/text_summarization.py`

 * *Files identical despite different names*

### Comparing `crowd-kit-1.3.0rc1/crowdkit/learning/utils.py` & `crowd-kit-1.3.0rc2/crowdkit/learning/utils.py`

 * *Files identical despite different names*

### Comparing `crowd-kit-1.3.0rc1/crowdkit/metrics/data/_classification.py` & `crowd-kit-1.3.0rc2/crowdkit/metrics/data/_classification.py`

 * *Files identical despite different names*

### Comparing `crowd-kit-1.3.0rc1/crowdkit/metrics/workers/accuracy_on_aggregates.py` & `crowd-kit-1.3.0rc2/crowdkit/metrics/workers/accuracy_on_aggregates.py`

 * *Files identical despite different names*

### Comparing `crowd-kit-1.3.0rc1/crowdkit/postprocessing/entropy_threshold.py` & `crowd-kit-1.3.0rc2/crowdkit/postprocessing/entropy_threshold.py`

 * *Files identical despite different names*

### Comparing `crowd-kit-1.3.0rc1/pyproject.toml` & `crowd-kit-1.3.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `crowd-kit-1.3.0rc1/tests/test_utils.py` & `crowd-kit-1.3.0rc2/tests/test_utils.py`

 * *Files identical despite different names*

