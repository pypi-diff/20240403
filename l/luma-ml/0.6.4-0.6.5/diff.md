# Comparing `tmp/luma-ml-0.6.4.tar.gz` & `tmp/luma-ml-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luma-ml-0.6.4.tar", last modified: Sun Mar 17 12:06:12 2024, max compression
+gzip compressed data, was "luma-ml-0.6.5.tar", last modified: Wed Apr  3 19:59:41 2024, max compression
```

## Comparing `luma-ml-0.6.4.tar` & `luma-ml-0.6.5.tar`

### file list

```diff
@@ -1,83 +1,84 @@
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-03-17 12:06:12.760366 luma-ml-0.6.4/
--rw-r--r--   0 chanlee    (501) staff       (20)    35149 2023-11-07 13:17:31.000000 luma-ml-0.6.4/LICENSE
--rw-r--r--   0 chanlee    (501) staff       (20)     5327 2024-03-17 12:06:12.759958 luma-ml-0.6.4/PKG-INFO
--rw-r--r--   0 chanlee    (501) staff       (20)     4834 2024-03-17 12:04:43.000000 luma-ml-0.6.4/README.md
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-03-17 12:06:12.735648 luma-ml-0.6.4/luma/
--rw-r--r--   0 chanlee    (501) staff       (20)     9535 2024-03-17 08:54:43.000000 luma-ml-0.6.4/luma/__import__.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1500 2024-03-16 19:58:45.000000 luma-ml-0.6.4/luma/__init__.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-03-17 12:06:12.738228 luma-ml-0.6.4/luma/classifier/
--rw-r--r--   0 chanlee    (501) staff       (20)    12559 2024-03-16 18:36:55.000000 luma-ml-0.6.4/luma/classifier/discriminant.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7202 2024-03-16 18:33:06.000000 luma-ml-0.6.4/luma/classifier/logistic.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5648 2024-03-16 18:34:12.000000 luma-ml-0.6.4/luma/classifier/naive_bayes.py
--rw-r--r--   0 chanlee    (501) staff       (20)     8788 2024-03-16 19:00:55.000000 luma-ml-0.6.4/luma/classifier/neighbors.py
--rw-r--r--   0 chanlee    (501) staff       (20)     8415 2024-03-16 18:42:33.000000 luma-ml-0.6.4/luma/classifier/svm.py
--rw-r--r--   0 chanlee    (501) staff       (20)     9583 2024-03-16 19:02:44.000000 luma-ml-0.6.4/luma/classifier/tree.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-03-17 12:06:12.740945 luma-ml-0.6.4/luma/clustering/
--rw-r--r--   0 chanlee    (501) staff       (20)    17184 2024-03-01 06:54:16.000000 luma-ml-0.6.4/luma/clustering/affinity.py
--rw-r--r--   0 chanlee    (501) staff       (20)    17357 2024-03-01 19:12:33.000000 luma-ml-0.6.4/luma/clustering/density.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7853 2024-03-04 18:19:25.000000 luma-ml-0.6.4/luma/clustering/hierarchy.py
--rw-r--r--   0 chanlee    (501) staff       (20)    17087 2024-03-02 19:12:27.000000 luma-ml-0.6.4/luma/clustering/kmeans.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7861 2024-03-03 05:12:07.000000 luma-ml-0.6.4/luma/clustering/mixture.py
--rw-r--r--   0 chanlee    (501) staff       (20)    11321 2024-03-05 16:26:06.000000 luma-ml-0.6.4/luma/clustering/spectral.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-03-17 12:06:12.742224 luma-ml-0.6.4/luma/core/
--rw-r--r--   0 chanlee    (501) staff       (20)     4550 2024-03-06 17:56:44.000000 luma-ml-0.6.4/luma/core/base.py
--rw-r--r--   0 chanlee    (501) staff       (20)      382 2024-03-06 17:32:06.000000 luma-ml-0.6.4/luma/core/main.py
--rw-r--r--   0 chanlee    (501) staff       (20)     9768 2024-03-11 20:04:11.000000 luma-ml-0.6.4/luma/core/super.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-03-17 12:06:12.744639 luma-ml-0.6.4/luma/ensemble/
--rw-r--r--   0 chanlee    (501) staff       (20)     9674 2024-03-16 19:38:38.000000 luma-ml-0.6.4/luma/ensemble/bagging.py
--rw-r--r--   0 chanlee    (501) staff       (20)    18833 2024-03-11 17:51:41.000000 luma-ml-0.6.4/luma/ensemble/boost.py
--rw-r--r--   0 chanlee    (501) staff       (20)     9349 2024-03-12 16:39:11.000000 luma-ml-0.6.4/luma/ensemble/forest.py
--rw-r--r--   0 chanlee    (501) staff       (20)    13692 2024-03-17 12:03:05.000000 luma-ml-0.6.4/luma/ensemble/stack.py
--rw-r--r--   0 chanlee    (501) staff       (20)     6709 2024-03-12 18:56:37.000000 luma-ml-0.6.4/luma/ensemble/vote.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-03-17 12:06:12.745286 luma-ml-0.6.4/luma/interface/
--rw-r--r--   0 chanlee    (501) staff       (20)     1084 2024-03-17 09:38:32.000000 luma-ml-0.6.4/luma/interface/exception.py
--rw-r--r--   0 chanlee    (501) staff       (20)    11400 2024-03-16 18:58:58.000000 luma-ml-0.6.4/luma/interface/util.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-03-17 12:06:12.747088 luma-ml-0.6.4/luma/metric/
--rw-r--r--   0 chanlee    (501) staff       (20)     1498 2024-03-06 18:27:41.000000 luma-ml-0.6.4/luma/metric/classification.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5714 2024-03-02 17:01:12.000000 luma-ml-0.6.4/luma/metric/clustering.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1574 2024-03-06 19:23:58.000000 luma-ml-0.6.4/luma/metric/distance.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1296 2024-01-29 14:18:31.000000 luma-ml-0.6.4/luma/metric/regression.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-03-17 12:06:12.747409 luma-ml-0.6.4/luma/migrate/
--rw-r--r--   0 chanlee    (501) staff       (20)     2121 2024-01-29 14:18:33.000000 luma-ml-0.6.4/luma/migrate/port.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-03-17 12:06:12.748939 luma-ml-0.6.4/luma/model_selection/
--rw-r--r--   0 chanlee    (501) staff       (20)     3443 2024-03-16 19:36:15.000000 luma-ml-0.6.4/luma/model_selection/cv.py
--rw-r--r--   0 chanlee    (501) staff       (20)     8039 2024-03-16 11:16:35.000000 luma-ml-0.6.4/luma/model_selection/fold.py
--rw-r--r--   0 chanlee    (501) staff       (20)    11908 2024-03-16 11:34:05.000000 luma-ml-0.6.4/luma/model_selection/search.py
--rw-r--r--   0 chanlee    (501) staff       (20)     3604 2024-03-16 16:03:41.000000 luma-ml-0.6.4/luma/model_selection/split.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-03-17 12:06:12.750507 luma-ml-0.6.4/luma/neural/
--rw-r--r--   0 chanlee    (501) staff       (20)     1895 2024-02-17 17:07:59.000000 luma-ml-0.6.4/luma/neural/activation.py
--rw-r--r--   0 chanlee    (501) staff       (20)    10598 2024-02-20 16:49:48.000000 luma-ml-0.6.4/luma/neural/multi_layer.py
--rw-r--r--   0 chanlee    (501) staff       (20)     6753 2024-02-22 18:06:34.000000 luma-ml-0.6.4/luma/neural/optimizer.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7837 2024-02-11 07:35:09.000000 luma-ml-0.6.4/luma/neural/single.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-03-17 12:06:12.751025 luma-ml-0.6.4/luma/pipe/
--rw-r--r--   0 chanlee    (501) staff       (20)     7314 2024-02-09 18:47:36.000000 luma-ml-0.6.4/luma/pipe/pipeline.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-03-17 12:06:12.752309 luma-ml-0.6.4/luma/preprocessing/
--rw-r--r--   0 chanlee    (501) staff       (20)     5259 2024-02-04 10:29:25.000000 luma-ml-0.6.4/luma/preprocessing/encoder.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5269 2024-01-29 14:19:14.000000 luma-ml-0.6.4/luma/preprocessing/imputer.py
--rw-r--r--   0 chanlee    (501) staff       (20)     3571 2024-01-29 20:01:54.000000 luma-ml-0.6.4/luma/preprocessing/outlier.py
--rw-r--r--   0 chanlee    (501) staff       (20)     2544 2024-02-11 08:01:10.000000 luma-ml-0.6.4/luma/preprocessing/scaler.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-03-17 12:06:12.754075 luma-ml-0.6.4/luma/reduction/
--rw-r--r--   0 chanlee    (501) staff       (20)    18134 2024-03-16 18:52:48.000000 luma-ml-0.6.4/luma/reduction/linear.py
--rw-r--r--   0 chanlee    (501) staff       (20)    37652 2024-02-04 10:30:27.000000 luma-ml-0.6.4/luma/reduction/manifold.py
--rw-r--r--   0 chanlee    (501) staff       (20)    16081 2024-03-16 16:02:52.000000 luma-ml-0.6.4/luma/reduction/selection.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-03-17 12:06:12.757348 luma-ml-0.6.4/luma/regressor/
--rw-r--r--   0 chanlee    (501) staff       (20)    17648 2024-01-29 14:20:17.000000 luma-ml-0.6.4/luma/regressor/general.py
--rw-r--r--   0 chanlee    (501) staff       (20)    11479 2024-02-11 13:26:41.000000 luma-ml-0.6.4/luma/regressor/linear.py
--rw-r--r--   0 chanlee    (501) staff       (20)     6292 2024-02-04 10:30:42.000000 luma-ml-0.6.4/luma/regressor/neighbors.py
--rw-r--r--   0 chanlee    (501) staff       (20)     2764 2024-01-31 17:09:28.000000 luma-ml-0.6.4/luma/regressor/poly.py
--rw-r--r--   0 chanlee    (501) staff       (20)    10332 2024-01-29 14:20:25.000000 luma-ml-0.6.4/luma/regressor/robust.py
--rw-r--r--   0 chanlee    (501) staff       (20)     6882 2024-02-11 13:27:20.000000 luma-ml-0.6.4/luma/regressor/svm.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7229 2024-03-11 18:23:55.000000 luma-ml-0.6.4/luma/regressor/tree.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-03-17 12:06:12.758139 luma-ml-0.6.4/luma/visual/
--rw-r--r--   0 chanlee    (501) staff       (20)     3115 2024-01-29 14:20:24.000000 luma-ml-0.6.4/luma/visual/eda.py
--rw-r--r--   0 chanlee    (501) staff       (20)    30298 2024-03-16 16:03:28.000000 luma-ml-0.6.4/luma/visual/evaluation.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-03-17 12:06:12.759329 luma-ml-0.6.4/luma_ml.egg-info/
--rw-r--r--   0 chanlee    (501) staff       (20)     5327 2024-03-17 12:06:12.000000 luma-ml-0.6.4/luma_ml.egg-info/PKG-INFO
--rw-r--r--   0 chanlee    (501) staff       (20)     1571 2024-03-17 12:06:12.000000 luma-ml-0.6.4/luma_ml.egg-info/SOURCES.txt
--rw-r--r--   0 chanlee    (501) staff       (20)        1 2024-03-17 12:06:12.000000 luma-ml-0.6.4/luma_ml.egg-info/dependency_links.txt
--rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-03-17 12:06:12.000000 luma-ml-0.6.4/luma_ml.egg-info/requires.txt
--rw-r--r--   0 chanlee    (501) staff       (20)       17 2024-03-17 12:06:12.000000 luma-ml-0.6.4/luma_ml.egg-info/top_level.txt
--rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-03-17 12:06:12.760489 luma-ml-0.6.4/setup.cfg
--rw-r--r--   0 chanlee    (501) staff       (20)      840 2024-03-17 12:04:51.000000 luma-ml-0.6.4/setup.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-03-17 12:06:12.759467 luma-ml-0.6.4/test/
--rw-r--r--   0 chanlee    (501) staff       (20)      104 2024-03-16 17:52:05.000000 luma-ml-0.6.4/test/__local__.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-03 19:59:41.797733 luma-ml-0.6.5/
+-rw-r--r--   0 chanlee    (501) staff       (20)    35149 2023-11-07 13:17:31.000000 luma-ml-0.6.5/LICENSE
+-rw-r--r--   0 chanlee    (501) staff       (20)     5558 2024-04-03 19:59:41.797466 luma-ml-0.6.5/PKG-INFO
+-rw-r--r--   0 chanlee    (501) staff       (20)     5065 2024-04-03 19:59:24.000000 luma-ml-0.6.5/README.md
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-03 19:59:41.777717 luma-ml-0.6.5/luma/
+-rw-r--r--   0 chanlee    (501) staff       (20)     9621 2024-04-03 12:19:39.000000 luma-ml-0.6.5/luma/__import__.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1501 2024-03-17 16:24:24.000000 luma-ml-0.6.5/luma/__init__.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-03 19:59:41.779895 luma-ml-0.6.5/luma/classifier/
+-rw-r--r--   0 chanlee    (501) staff       (20)    12289 2024-04-03 15:07:50.000000 luma-ml-0.6.5/luma/classifier/discriminant.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7650 2024-04-03 15:41:30.000000 luma-ml-0.6.5/luma/classifier/logistic.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5566 2024-04-03 15:52:03.000000 luma-ml-0.6.5/luma/classifier/naive_bayes.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     8976 2024-04-03 16:03:41.000000 luma-ml-0.6.5/luma/classifier/neighbors.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     8838 2024-04-03 17:17:16.000000 luma-ml-0.6.5/luma/classifier/svm.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     9562 2024-04-03 17:24:32.000000 luma-ml-0.6.5/luma/classifier/tree.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-03 19:59:41.782068 luma-ml-0.6.5/luma/clustering/
+-rw-r--r--   0 chanlee    (501) staff       (20)    17317 2024-04-03 17:28:35.000000 luma-ml-0.6.5/luma/clustering/affinity.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    17423 2024-04-03 17:49:28.000000 luma-ml-0.6.5/luma/clustering/density.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7701 2024-04-03 17:55:23.000000 luma-ml-0.6.5/luma/clustering/hierarchy.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    17775 2024-04-03 17:56:01.000000 luma-ml-0.6.5/luma/clustering/kmeans.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     8022 2024-04-03 17:57:13.000000 luma-ml-0.6.5/luma/clustering/mixture.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    11490 2024-04-03 18:01:29.000000 luma-ml-0.6.5/luma/clustering/spectral.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-03 19:59:41.783030 luma-ml-0.6.5/luma/core/
+-rw-r--r--   0 chanlee    (501) staff       (20)     5174 2024-04-03 19:14:20.000000 luma-ml-0.6.5/luma/core/base.py
+-rw-r--r--   0 chanlee    (501) staff       (20)      393 2024-03-17 16:24:24.000000 luma-ml-0.6.5/luma/core/main.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    10135 2024-04-03 19:09:33.000000 luma-ml-0.6.5/luma/core/super.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-03 19:59:41.784758 luma-ml-0.6.5/luma/ensemble/
+-rw-r--r--   0 chanlee    (501) staff       (20)     9738 2024-04-03 18:04:08.000000 luma-ml-0.6.5/luma/ensemble/bagging.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    19296 2024-04-03 18:09:25.000000 luma-ml-0.6.5/luma/ensemble/boost.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     9678 2024-04-03 18:09:26.000000 luma-ml-0.6.5/luma/ensemble/forest.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    13574 2024-04-03 18:11:50.000000 luma-ml-0.6.5/luma/ensemble/stack.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     6500 2024-03-17 16:24:24.000000 luma-ml-0.6.5/luma/ensemble/vote.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-03 19:59:41.785410 luma-ml-0.6.5/luma/interface/
+-rw-r--r--   0 chanlee    (501) staff       (20)     1294 2024-04-03 15:51:54.000000 luma-ml-0.6.5/luma/interface/exception.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    14307 2024-04-03 17:28:18.000000 luma-ml-0.6.5/luma/interface/util.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-03 19:59:41.786529 luma-ml-0.6.5/luma/metric/
+-rw-r--r--   0 chanlee    (501) staff       (20)     1471 2024-03-17 17:44:55.000000 luma-ml-0.6.5/luma/metric/classification.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5709 2024-03-17 18:40:44.000000 luma-ml-0.6.5/luma/metric/clustering.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1551 2024-03-19 13:36:06.000000 luma-ml-0.6.5/luma/metric/distance.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1646 2024-03-19 16:59:18.000000 luma-ml-0.6.5/luma/metric/regression.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-03 19:59:41.786822 luma-ml-0.6.5/luma/migrate/
+-rw-r--r--   0 chanlee    (501) staff       (20)     3425 2024-04-03 18:12:20.000000 luma-ml-0.6.5/luma/migrate/port.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-03 19:59:41.788262 luma-ml-0.6.5/luma/model_selection/
+-rw-r--r--   0 chanlee    (501) staff       (20)     3357 2024-04-03 18:17:54.000000 luma-ml-0.6.5/luma/model_selection/cv.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7964 2024-04-03 18:17:54.000000 luma-ml-0.6.5/luma/model_selection/fold.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    11720 2024-04-03 18:17:54.000000 luma-ml-0.6.5/luma/model_selection/search.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     3570 2024-04-03 18:17:54.000000 luma-ml-0.6.5/luma/model_selection/split.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-03 19:59:41.789524 luma-ml-0.6.5/luma/neural/
+-rw-r--r--   0 chanlee    (501) staff       (20)     1909 2024-03-29 20:03:35.000000 luma-ml-0.6.5/luma/neural/activation.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    10709 2024-04-03 18:19:49.000000 luma-ml-0.6.5/luma/neural/multi_layer.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7118 2024-04-03 18:24:38.000000 luma-ml-0.6.5/luma/neural/optimizer.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     8237 2024-04-03 18:26:58.000000 luma-ml-0.6.5/luma/neural/single.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-03 19:59:41.789830 luma-ml-0.6.5/luma/pipe/
+-rw-r--r--   0 chanlee    (501) staff       (20)     7279 2024-04-03 18:27:03.000000 luma-ml-0.6.5/luma/pipe/pipeline.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-03 19:59:41.791108 luma-ml-0.6.5/luma/preprocessing/
+-rw-r--r--   0 chanlee    (501) staff       (20)     5332 2024-04-03 18:29:25.000000 luma-ml-0.6.5/luma/preprocessing/encoder.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5556 2024-04-03 18:33:19.000000 luma-ml-0.6.5/luma/preprocessing/imputer.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     3553 2024-04-03 18:34:45.000000 luma-ml-0.6.5/luma/preprocessing/outlier.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     2551 2024-04-03 18:34:48.000000 luma-ml-0.6.5/luma/preprocessing/scaler.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-03 19:59:41.791947 luma-ml-0.6.5/luma/reduction/
+-rw-r--r--   0 chanlee    (501) staff       (20)    18473 2024-04-03 18:41:38.000000 luma-ml-0.6.5/luma/reduction/linear.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    39231 2024-04-03 19:59:39.000000 luma-ml-0.6.5/luma/reduction/manifold.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    15454 2024-03-17 16:24:24.000000 luma-ml-0.6.5/luma/reduction/selection.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-03 19:59:41.794577 luma-ml-0.6.5/luma/regressor/
+-rw-r--r--   0 chanlee    (501) staff       (20)    17451 2024-03-29 20:03:41.000000 luma-ml-0.6.5/luma/regressor/general.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    11186 2024-04-03 11:16:13.000000 luma-ml-0.6.5/luma/regressor/linear.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     6205 2024-03-17 16:24:24.000000 luma-ml-0.6.5/luma/regressor/neighbors.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     2720 2024-03-17 16:24:24.000000 luma-ml-0.6.5/luma/regressor/poly.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    10094 2024-03-17 16:24:24.000000 luma-ml-0.6.5/luma/regressor/robust.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     6764 2024-04-03 11:16:13.000000 luma-ml-0.6.5/luma/regressor/svm.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     6861 2024-03-17 16:24:24.000000 luma-ml-0.6.5/luma/regressor/tree.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-03 19:59:41.795203 luma-ml-0.6.5/luma/visual/
+-rw-r--r--   0 chanlee    (501) staff       (20)     2971 2024-03-17 16:24:24.000000 luma-ml-0.6.5/luma/visual/eda.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    29242 2024-03-29 17:27:43.000000 luma-ml-0.6.5/luma/visual/evaluation.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-03 19:59:41.796358 luma-ml-0.6.5/luma_ml.egg-info/
+-rw-r--r--   0 chanlee    (501) staff       (20)     5558 2024-04-03 19:59:41.000000 luma-ml-0.6.5/luma_ml.egg-info/PKG-INFO
+-rw-r--r--   0 chanlee    (501) staff       (20)     1585 2024-04-03 19:59:41.000000 luma-ml-0.6.5/luma_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)        1 2024-04-03 19:59:41.000000 luma-ml-0.6.5/luma_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-04-03 19:59:41.000000 luma-ml-0.6.5/luma_ml.egg-info/requires.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)       17 2024-04-03 19:59:41.000000 luma-ml-0.6.5/luma_ml.egg-info/top_level.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-04-03 19:59:41.797798 luma-ml-0.6.5/setup.cfg
+-rw-r--r--   0 chanlee    (501) staff       (20)      795 2024-04-03 19:59:30.000000 luma-ml-0.6.5/setup.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-03 19:59:41.796860 luma-ml-0.6.5/test/
+-rw-r--r--   0 chanlee    (501) staff       (20)      105 2024-03-30 12:09:50.000000 luma-ml-0.6.5/test/__local__.py
+-rw-r--r--   0 chanlee    (501) staff       (20)      807 2024-04-03 19:42:17.000000 luma-ml-0.6.5/test/_docs.py
```

### Comparing `luma-ml-0.6.4/LICENSE` & `luma-ml-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.4/PKG-INFO` & `luma-ml-0.6.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luma-ml
-Version: 0.6.4
+Version: 0.6.5
 Summary: A Comprehensive Python Module for Machine Learning and Data Science
 Home-page: https://github.com/ChanLumerico/LUMA
 Author: ChanLumerico
 Author-email: greensox284@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -18,16 +18,18 @@
         <a href="https://lumerico284.notion.site/LUMA-a467e4a9e885498f87b49c952d0abecd?pvs=74">
             <img src="https://github.com/ChanLumerico/luma/raw/main/others/luma.png" alt="logo" width="75" height="75">
         </a>
         <h1 class="main-title">LUMA</h1>
         <p class="subtitle">A Comprehensive Python Module for Machine Learning and Data Science</p>
         <img alt="pypi-version" src="https://img.shields.io/pypi/v/luma-ml?logo=python&logoColor=white&color=blue">
         <img alt="pypi-downloads" src="https://img.shields.io/pypi/dm/luma-ml">
-        <img src="https://img.shields.io/badge/total downloads-4.0k-red">
+        <img src="https://img.shields.io/badge/total downloads-4.3k-red">
         <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/ChanLumerico/luma?color=yellow">
+        <img alt="Code Style" src="https://img.shields.io/badge/code%20style-black-000000.svg">
+        <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/ChanLumerico/luma?color=purple">
         <div class="module">
             <h3 class="module-header">Submodules</h3>
             <table>
                 <tr>
                     <th>Name</th>
                     <th>Description</th>
                 </tr>
@@ -102,19 +104,19 @@
         </div>
         <h2></h2>
         <div class="others">
             <h3 class="others-header">Others</h3>
             <table>
                 <tr>
                     <td>Latest Version</td>
-                    <td>0.6.4</td>
+                    <td>0.6.5</td>
                 </tr>
                 <tr>
                     <td>Lines of Code</td>
-                    <td>~14K</td>
+                    <td>~15.7K</td>
                 </tr>
                 <tr>
                     <td>Requirement</td>
                     <td>Python 3.10 or later</td>
                 </tr>
                 <tr>
                     <td>Dependencies</td>
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: luma-ml Version: 0.6.4 Summary: A Comprehensive
+Metadata-Version: 2.1 Name: luma-ml Version: 0.6.5 Summary: A Comprehensive
 Python Module for Machine Learning and Data Science Home-page: https://
 github.com/ChanLumerico/LUMA Author: ChanLumerico Author-email:
 greensox284@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE
 _[_l_o_g_o_]
 ************ LLUUMMAA ************
 A Comprehensive Python Module for Machine Learning and Data Science
 [pypi-version][pypi-downloads][https://img.shields.io/badge/total downloads-
-4.0k-red][GitHub last commit]
+4.3k-red][GitHub last commit][Code Style][GitHub code size in bytes]
 ******** SSuubbmmoodduulleess ********
 NNaammee                 DDeessccrriippttiioonn
 luma.classifier      Toolkit for classification models including various
                      algorithms.
 luma.clustering      Focuses on unsupervised learning and clustering
                      algorithms.
 luma.core            Foundational backbone providing essential data structures
@@ -31,12 +31,12 @@
 luma.reduction       Dimensionality reduction techniques for high-dimensional
                      datasets.
 luma.regressor       Comprehensive range of regression algorithms.
 luma.visual          Tools for model visualization and data plotting.
 ******** SSttrruuccttuurree ********
 [structure]
 ******** OOtthheerrss ********
-Latest Version 0.6.4
-Lines of Code  ~14K
+Latest Version 0.6.5
+Lines of Code  ~15.7K
 Requirement    Python 3.10 or later
 Dependencies   NumPy, SciPy, Pandas, Matplotlib, Seaborn
 Documentation  _L_U_M_A_ _N_o_t_i_o_n_ _D_o_c_u_m_e_n_t
```

### Comparing `luma-ml-0.6.4/README.md` & `luma-ml-0.6.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,18 @@
         <a href="https://lumerico284.notion.site/LUMA-a467e4a9e885498f87b49c952d0abecd?pvs=74">
             <img src="https://github.com/ChanLumerico/luma/raw/main/others/luma.png" alt="logo" width="75" height="75">
         </a>
         <h1 class="main-title">LUMA</h1>
         <p class="subtitle">A Comprehensive Python Module for Machine Learning and Data Science</p>
         <img alt="pypi-version" src="https://img.shields.io/pypi/v/luma-ml?logo=python&logoColor=white&color=blue">
         <img alt="pypi-downloads" src="https://img.shields.io/pypi/dm/luma-ml">
-        <img src="https://img.shields.io/badge/total downloads-4.0k-red">
+        <img src="https://img.shields.io/badge/total downloads-4.3k-red">
         <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/ChanLumerico/luma?color=yellow">
+        <img alt="Code Style" src="https://img.shields.io/badge/code%20style-black-000000.svg">
+        <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/ChanLumerico/luma?color=purple">
         <div class="module">
             <h3 class="module-header">Submodules</h3>
             <table>
                 <tr>
                     <th>Name</th>
                     <th>Description</th>
                 </tr>
@@ -88,19 +90,19 @@
         </div>
         <h2></h2>
         <div class="others">
             <h3 class="others-header">Others</h3>
             <table>
                 <tr>
                     <td>Latest Version</td>
-                    <td>0.6.4</td>
+                    <td>0.6.5</td>
                 </tr>
                 <tr>
                     <td>Lines of Code</td>
-                    <td>~14K</td>
+                    <td>~15.7K</td>
                 </tr>
                 <tr>
                     <td>Requirement</td>
                     <td>Python 3.10 or later</td>
                 </tr>
                 <tr>
                     <td>Dependencies</td>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 _[_l_o_g_o_]
 ************ LLUUMMAA ************
 A Comprehensive Python Module for Machine Learning and Data Science
 [pypi-version][pypi-downloads][https://img.shields.io/badge/total downloads-
-4.0k-red][GitHub last commit]
+4.3k-red][GitHub last commit][Code Style][GitHub code size in bytes]
 ******** SSuubbmmoodduulleess ********
 NNaammee                 DDeessccrriippttiioonn
 luma.classifier      Toolkit for classification models including various
                      algorithms.
 luma.clustering      Focuses on unsupervised learning and clustering
                      algorithms.
 luma.core            Foundational backbone providing essential data structures
@@ -24,12 +24,12 @@
 luma.reduction       Dimensionality reduction techniques for high-dimensional
                      datasets.
 luma.regressor       Comprehensive range of regression algorithms.
 luma.visual          Tools for model visualization and data plotting.
 ******** SSttrruuccttuurree ********
 [structure]
 ******** OOtthheerrss ********
-Latest Version 0.6.4
-Lines of Code  ~14K
+Latest Version 0.6.5
+Lines of Code  ~15.7K
 Requirement    Python 3.10 or later
 Dependencies   NumPy, SciPy, Pandas, Matplotlib, Seaborn
 Documentation  _L_U_M_A_ _N_o_t_i_o_n_ _D_o_c_u_m_e_n_t
```

### Comparing `luma-ml-0.6.4/luma/__import__.py` & `luma-ml-0.6.5/luma/__import__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,57 @@
 from luma.core.main import Luma
 from luma.core.base import ModelBase, ParadigmBase, MetricBase, VisualBase
 from luma.core.super import Estimator, Transformer, Optimizer, Evaluator, Visualizer
 from luma.core.super import Supervised, Unsupervised, Distance
 
 from luma.interface.exception import NotFittedError, NotConvergedError
-from luma.interface.exception import UnsupportedParameterError, ModelExtensionError
-from luma.interface.util import Matrix, Vector, Scalar, DecisionTreeNode, NearestNeighbors
+from luma.interface.exception import (
+    UnsupportedParameterError,
+    ModelExtensionError,
+    InvalidRangeError,
+)
+from luma.interface.util import (
+    Matrix,
+    Vector,
+    Scalar,
+    DecisionTreeNode,
+    NearestNeighbors,
+)
 from luma.interface.util import SilhouetteUtil, DBUtil, KernelUtil, ActivationUtil
-from luma.interface.util import Clone
+from luma.interface.util import Clone, ParamRange
 
-from luma.classifier.discriminant import LDAClassifier, QDAClassifier, RDAClassifier, KDAClassifier
+from luma.classifier.discriminant import (
+    LDAClassifier,
+    QDAClassifier,
+    RDAClassifier,
+    KDAClassifier,
+)
 from luma.classifier.logistic import LogisticRegressor, SoftmaxRegressor
 from luma.classifier.naive_bayes import GaussianNaiveBayes, BernoulliNaiveBayes
 from luma.classifier.svm import SVC, KernelSVC
 from luma.classifier.tree import DecisionTreeClassifier
-from luma.classifier.neighbors import KNNClassifier, AdaptiveKNNClassifier, WeightedKNNClassifier
-
-from luma.clustering.kmeans import KMeansClustering, KMeansClusteringPlus, KMediansClustering
+from luma.classifier.neighbors import (
+    KNNClassifier,
+    AdaptiveKNNClassifier,
+    WeightedKNNClassifier,
+)
+
+from luma.clustering.kmeans import (
+    KMeansClustering,
+    KMeansClusteringPlus,
+    KMediansClustering,
+)
 from luma.clustering.kmeans import KMedoidsClustering, MiniBatchKMeansClustering
 from luma.clustering.kmeans import FuzzyCMeansClustering
 from luma.clustering.hierarchy import AgglomerativeClustering, DivisiveClustering
 from luma.clustering.spectral import SpectralClustering, NormalizedSpectralClustering
-from luma.clustering.spectral import HierarchicalSpectralClustering, AdaptiveSpectralClustering
+from luma.clustering.spectral import (
+    HierarchicalSpectralClustering,
+    AdaptiveSpectralClustering,
+)
 from luma.clustering.density import DBSCAN, OPTICS, DENCLUE, MeanShiftClustering
 from luma.clustering.affinity import AffinityPropagation, AdaptiveAffinityPropagation
 from luma.clustering.affinity import KernelAffinityPropagation
 from luma.clustering.mixture import GaussianMixture, MultinomialMixture
 
 from luma.ensemble.forest import RandomForestClassifier, RandomForestRegressor
 from luma.ensemble.vote import VotingClassifier, VotingRegressor
@@ -36,24 +62,30 @@
 
 from luma.neural.activation import ReLU, LeakyReLU, ELU, Tanh, Sigmoid, Softmax
 from luma.neural.optimizer import SGDOptimizer, MomentumOptimizer, RMSPropOptimizer
 from luma.neural.single import PerceptronClassifier, PerceptronRegressor
 from luma.neural.multi_layer import MLPClassifier
 
 from luma.metric.classification import Accuracy, Precision, Recall, F1Score, Specificity
-from luma.metric.regression import MeanAbsoluteError, MeanSquaredError, RootMeanSquaredError
-from luma.metric.regression import MeanAbsolutePercentageError, RSquaredScore
+from luma.metric.regression import (
+    MeanAbsoluteError,
+    MeanSquaredError,
+    RootMeanSquaredError,
+    MeanAbsolutePercentageError,
+    RSquaredScore,
+    AdjustedRSquaredScore,
+)
 from luma.metric.clustering import SilhouetteCoefficient, DaviesBouldin, Inertia
 from luma.metric.distance import Euclidean, Manhattan, Chebyshev, Minkowski
 from luma.metric.distance import CosineSimilarity, Correlation, Mahalanobis
 
 from luma.model_selection.split import TrainTestSplit
 from luma.model_selection.search import GridSearchCV, RandomizedSearchCV
 from luma.model_selection.cv import CrossValidator
-from luma.model_selection.fold import KFold, StratifiedKFold 
+from luma.model_selection.fold import KFold, StratifiedKFold
 
 from luma.preprocessing.scaler import StandardScaler, MinMaxScaler
 from luma.preprocessing.encoder import OneHotEncoder, LabelEncoder, OrdinalEncoder
 from luma.preprocessing.encoder import LabelBinarizer
 from luma.preprocessing.imputer import SimpleImputer, KNNImputer, HotDeckImputer
 from luma.preprocessing.outlier import LocalOutlierFactor
 
@@ -62,168 +94,188 @@
 from luma.reduction.manifold import TSNE, SammonMapping, LaplacianEigenmap
 from luma.reduction.manifold import MDS, MetricMDS, LandmarkMDS
 from luma.reduction.manifold import LLE, ModifiedLLE, HessianLLE, LTSA
 from luma.reduction.manifold import Isomap, ConformalIsomap
 from luma.reduction.selection import SBS, SFS, RFE
 
 from luma.regressor.linear import LinearRegressor, LassoRegressor, RidgeRegressor
-from luma.regressor.linear import ElasticNetRegressor, KernelRidgeRegressor, BayesianRidgeRegressor
+from luma.regressor.linear import (
+    ElasticNetRegressor,
+    KernelRidgeRegressor,
+    BayesianRidgeRegressor,
+)
 from luma.regressor.poly import PolynomialRegressor
 from luma.regressor.general import PoissonRegressor
 from luma.regressor.general import NegativeBinomialRegressor
 from luma.regressor.general import GammaRegressor
 from luma.regressor.general import BetaRegressor
 from luma.regressor.general import InverseGaussianRegressor
 from luma.regressor.svm import SVR, KernelSVR
 from luma.regressor.tree import DecisionTreeRegressor
-from luma.regressor.neighbors import KNNRegressor, AdaptiveKNNRegressor, WeightedKNNRegressor
+from luma.regressor.neighbors import (
+    KNNRegressor,
+    AdaptiveKNNRegressor,
+    WeightedKNNRegressor,
+)
 from luma.regressor.robust import RANSAC, MLESAC
 
 from luma.pipe.pipeline import Pipeline
 
-from luma.visual.eda import CorrelationBar, CorrelationHeatMap, JointPlot, MissingProportion
-from luma.visual.evaluation import DecisionRegion, ClusterPlot, ROCCurve, PrecisionRecallCurve
+from luma.visual.eda import (
+    CorrelationBar,
+    CorrelationHeatMap,
+    JointPlot,
+    MissingProportion,
+)
+from luma.visual.evaluation import (
+    DecisionRegion,
+    ClusterPlot,
+    ROCCurve,
+    PrecisionRecallCurve,
+)
 from luma.visual.evaluation import ConfusionMatrix, ResidualPlot, LearningCurve
 from luma.visual.evaluation import ValidationCurve, ValidationHeatmap, InertiaPlot
 
 from luma.migrate.port import ModelPorter
 
 
-if __name__ == '__main__':
-    
+if __name__ == "__main__":
+
     # ------------------- [ luma.core ] ------------------------
     Luma
-    
+
     ModelBase, ParadigmBase, MetricBase, VisualBase
-    
+
     Estimator, Transformer, Optimizer, Evaluator, Visualizer,
     Supervised, Unsupervised, Distance
-    
+
     # ----------------- [ luma.interface ] ---------------------
     NotFittedError, NotConvergedError,
-    UnsupportedParameterError, ModelExtensionError
-    
+    UnsupportedParameterError, ModelExtensionError,
+    InvalidRangeError
+
     Matrix, Vector, Scalar, DecisionTreeNode, NearestNeighbors,
     SilhouetteUtil, DBUtil, KernelUtil, ActivationUtil,
-    Clone
-    
+    Clone, ParamRange
+
     # ----------------- [ luma.classifier ] --------------------
     LDAClassifier, QDAClassifier, RDAClassifier, KDAClassifier
-    
+
     LogisticRegressor, SoftmaxRegressor
-    
+
     GaussianNaiveBayes, BernoulliNaiveBayes
-    
+
     SVC, KernelSVC
-    
+
     DecisionTreeClassifier
-    
+
     KNNClassifier, AdaptiveKNNClassifier, WeightedKNNClassifier
-    
+
     # ----------------- [ luma.clustering ] --------------------
     KMeansClustering, KMeansClusteringPlus, KMediansClustering,
     KMedoidsClustering, MiniBatchKMeansClustering,
     FuzzyCMeansClustering
-    
+
     AgglomerativeClustering, DivisiveClustering
-    
+
     SpectralClustering, NormalizedSpectralClustering,
     HierarchicalSpectralClustering, AdaptiveSpectralClustering
-    
+
     DBSCAN, OPTICS, DENCLUE, MeanShiftClustering
-    
+
     AffinityPropagation, AdaptiveAffinityPropagation,
     KernelAffinityPropagation
-    
+
     GaussianMixture, MultinomialMixture
-    
+
     # ------------------ [ luma.ensemble ] ---------------------
     RandomForestClassifier, RandomForestRegressor
-    
+
     VotingClassifier, VotingRegressor
-    
+
     BaggingClassifier, BaggingRegressor
-    
+
     AdaBoostClassifier, AdaBoostRegressor,
     GradientBoostingClassifier, GradientBoostingRegressor
-    
+
     StackingClassifier, StackingRegressor
-    
+
     # ------------------- [ luma.neural ] ----------------------
     PerceptronClassifier, PerceptronRegressor
-    
+
     MLPClassifier
-    
+
     ReLU, LeakyReLU, ELU, Tanh, Sigmoid, Softmax
-    
+
     SGDOptimizer, MomentumOptimizer, RMSPropOptimizer
-    
+
     # ------------------- [ luma.metric ] ----------------------
     Accuracy, Precision, Recall, F1Score, Specificity
-    
+
     MeanAbsoluteError, MeanSquaredError, RootMeanSquaredError,
-    MeanAbsolutePercentageError, RSquaredScore
-    
+    MeanAbsolutePercentageError, RSquaredScore,
+    AdjustedRSquaredScore
+
     SilhouetteCoefficient, DaviesBouldin, Inertia
-    
+
     Euclidean, Manhattan, Chebyshev, Minkowski,
     CosineSimilarity, Correlation, Mahalanobis
-    
+
     # --------------- [ luma.module_selection ] ----------------
     TrainTestSplit
-    
+
     GridSearchCV, RandomizedSearchCV
-    
+
     CrossValidator
-    
+
     KFold, StratifiedKFold
-    
+
     # ---------------- [ luma.preprocessing ] ------------------
     StandardScaler, MinMaxScaler
-    
+
     OneHotEncoder, LabelEncoder, OrdinalEncoder, LabelBinarizer
-    
+
     SimpleImputer, KNNImputer, HotDeckImputer
-    
+
     LocalOutlierFactor
-    
+
     # ----------------- [ luma.reduction ] ---------------------
     PCA, KernelPCA, LDA, KDA, CCA, TruncatedSVD, FactorAnalysis
-    
+
     TSNE, SammonMapping, LaplacianEigenmap,
     MDS, MetricMDS, LandmarkMDS,
     LLE, ModifiedLLE, HessianLLE, LTSA,
     Isomap, ConformalIsomap
-    
+
     SBS, SFS, RFE
-    
+
     # ----------------- [ luma.regressor ] ---------------------
-    LinearRegressor, RidgeRegressor, LassoRegressor, 
+    LinearRegressor, RidgeRegressor, LassoRegressor,
     ElasticNetRegressor, KernelRidgeRegressor,
     BayesianRidgeRegressor
-    
+
     PolynomialRegressor
-    
+
     PoissonRegressor, NegativeBinomialRegressor, GammaRegressor,
     BetaRegressor, InverseGaussianRegressor
-    
+
     SVR, KernelSVR
-    
+
     DecisionTreeRegressor
-    
+
     KNNRegressor, AdaptiveKNNRegressor, WeightedKNNRegressor
-    
+
     RANSAC, MLESAC
-    
+
     # -------------------- [ luma.pipe ] -----------------------
     Pipeline
-    
+
     # ------------------- [ luma.visual ] ----------------------
     CorrelationBar, CorrelationHeatMap, JointPlot,
     MissingProportion
-    
-    DecisionRegion, ClusterPlot, ROCCurve, PrecisionRecallCurve, 
+
+    DecisionRegion, ClusterPlot, ROCCurve, PrecisionRecallCurve,
     ConfusionMatrix, ResidualPlot, LearningCurve,
     ValidationCurve, ValidationHeatmap, InertiaPlot
-    
+
     # ------------------ [ luma.migrate ] ----------------------
     ModelPorter
```

### Comparing `luma-ml-0.6.4/luma/__init__.py` & `luma-ml-0.6.5/luma/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -44,8 +44,8 @@
 Whether you're interested in fixing bugs, adding new features, or improving documentation, 
 your help is appreciated.
 
 License
 -------
 Luma is released under the GPL-3.0 License. See `LICENSE` file for more details.
 
-"""
+"""
```

### Comparing `luma-ml-0.6.4/luma/classifier/discriminant.py` & `luma-ml-0.6.5/luma/classifier/discriminant.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,348 +4,346 @@
 
 from luma.core.super import Estimator, Evaluator, Supervised
 from luma.interface.util import Matrix, Scalar, Vector, KernelUtil
 from luma.interface.exception import NotFittedError
 from luma.metric.classification import Accuracy
 
 
-__all__ = (
-    'LDAClassifier',
-    'QDAClassifier',
-    'RDAClassifier',
-    'KDAClassifier'
-)
+__all__ = ("LDAClassifier", "QDAClassifier", "RDAClassifier", "KDAClassifier")
 
 
 class LDAClassifier(Estimator, Supervised):
-    
     """
-    Linear Discriminant Analysis (LDA) is a statistical technique used for 
-    dimensionality reduction and classification. It projects data onto a 
-    lower-dimensional space with the goal of maximizing class separability. 
-    LDA assumes that different classes generate data based on Gaussian 
-    distributions with the same covariance matrix but different mean vectors. 
-    It finds linear combinations of features that best separate the classes, 
+    Linear Discriminant Analysis (LDA) is a statistical technique used for
+    dimensionality reduction and classification. It projects data onto a
+    lower-dimensional space with the goal of maximizing class separability.
+    LDA assumes that different classes generate data based on Gaussian
+    distributions with the same covariance matrix but different mean vectors.
+    It finds linear combinations of features that best separate the classes,
     facilitating classification or visualization of complex data.
-    
+
     Notes
     -----
-    * To use LDA for dimensionality reduction, refer to 
+    * To use LDA for dimensionality reduction, refer to
         `luma.reduction.linear.LDA`
     """
-    
+
     def __init__(self) -> None:
-        self.means = None,
-        self.priors = None,
+        self.means = (None,)
+        self.priors = (None,)
         self.covs = None
         self._fitted = False
-    
-    def fit(self, X: Matrix, y: Vector) -> 'LDAClassifier':
+
+    def fit(self, X: Matrix, y: Vector) -> "LDAClassifier":
         m, n = X.shape
         class_labels = np.unique(y)
         n_classes = len(class_labels)
-        
+
         self.means = np.zeros((n_classes, n))
         self.priors = np.zeros(n_classes)
         self.covs = np.zeros((n, n))
 
         for i, cl in enumerate(class_labels):
             X_class = X[y == cl]
             self.means[i] = X_class.mean(axis=0)
             self.priors[i] = X_class.shape[0] / m
             self.covs += np.cov(X_class, rowvar=False) * (X_class.shape[0] - 1)
-        
-        self.covs /= (X.shape[0] - n_classes)
+
+        self.covs /= X.shape[0] - n_classes
         self.cov_inv = np.linalg.inv(self.covs)
 
         self.coef_ = np.dot(self.cov_inv, self.means.T).T
         self.intercept_ = -0.5 * np.diag(np.dot(self.means, self.coef_.T))
         self.intercept_ += np.log(self.priors)
-        
+
         self._fitted = True
         return self
-    
+
     def predict(self, X: Matrix) -> Vector:
-        if not self._fitted: raise not NotFittedError(self)
+        if not self._fitted:
+            raise not NotFittedError(self)
         scores = np.dot(X, self.coef_.T) + self.intercept_
-        
+
         return np.argmax(scores, axis=1)
-    
+
     def predict_proba(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         scores = np.dot(X, self.coef_.T) + self.intercept_
-        
+
         return softmax(scores, axis=1)
-    
-    def score(self, X: Matrix, y: Matrix, 
-              metric: Evaluator = Accuracy) -> float:
+
+    def score(self, X: Matrix, y: Matrix, metric: Evaluator = Accuracy) -> float:
         X_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=X_pred)
 
 
 class QDAClassifier(Estimator, Supervised):
-    
     """
-    Quadratic Discriminant Analysis (QDA) is a classification technique 
-    that assumes data from each class follows a Gaussian distribution 
-    with class-specific covariance matrices. It calculates the probability 
-    of a given sample belonging to each class based on a quadratic decision 
-    boundary determined by these distributions. Unlike Linear Discriminant 
-    Analysis (LDA), QDA allows for the modeling of nonlinear relationships 
-    due to the class-specific covariances. It is well-suited for datasets 
+    Quadratic Discriminant Analysis (QDA) is a classification technique
+    that assumes data from each class follows a Gaussian distribution
+    with class-specific covariance matrices. It calculates the probability
+    of a given sample belonging to each class based on a quadratic decision
+    boundary determined by these distributions. Unlike Linear Discriminant
+    Analysis (LDA), QDA allows for the modeling of nonlinear relationships
+    due to the class-specific covariances. It is well-suited for datasets
     where classes exhibit different levels of variance.
     """
-    
+
     def __init__(self) -> None:
         self.means = None
         self.covs = None
         self.priors = None
         self.classes = None
         self._fitted = False
-    
-    def fit(self, X: Matrix, y: Vector) -> 'QDAClassifier':
+
+    def fit(self, X: Matrix, y: Vector) -> "QDAClassifier":
         m, n = X.shape
         self.classes = np.unique(y)
         n_classes = len(self.classes)
-        
+
         self.means = np.zeros((n_classes, n))
         self.covs = np.zeros((n_classes, n, n))
         self.priors = np.zeros(n_classes)
-        
+
         for i, cl in enumerate(self.classes):
             X_cls = X[y == cl]
             self.means[i] = np.mean(X_cls, axis=0)
             self.covs[i] = np.cov(X_cls, rowvar=False)
             self.priors[i] = X_cls.shape[0] / m
-        
+
         self._fitted = True
         return self
 
     def predict(self, X: Matrix) -> Vector:
-        if not self._fitted: raise not NotFittedError(self)
+        if not self._fitted:
+            raise not NotFittedError(self)
         y_pred = [self._predict_sample(x) for x in X]
         return Vector(y_pred)
-    
+
     def _predict_sample(self, x: Vector) -> Scalar:
         discs = np.zeros(len(self.classes))
         for i in range(len(self.classes)):
             diff = x - self.means[i]
             cov_inv = np.linalg.inv(self.covs[i])
             cov_det = np.linalg.det(self.covs[i])
-            
+
             disc = np.log(cov_det) + diff.T.dot(cov_inv).dot(diff)
             disc *= -0.5
             disc += np.log(self.priors[i])
             discs[i] = disc
-        
+
         return self.classes[np.argmax(discs)]
-    
+
     def predict_proba(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         log_probs = np.array([self._log_proba_sample(x) for x in X])
-        
+
         return softmax(log_probs, axis=1)
-    
+
     def _log_proba_sample(self, x: Vector) -> Vector:
         log_probs = np.zeros(len(self.classes))
         for i, _ in enumerate(self.classes):
             mvn = multivariate_normal(mean=self.means[i], cov=self.covs[i])
             log_probs[i] = mvn.logpdf(x) + np.log(self.priors[i])
-        
+
         return log_probs
-    
-    def score(self, X: Matrix, y: Matrix, 
-              metric: Evaluator = Accuracy) -> float:
+
+    def score(self, X: Matrix, y: Matrix, metric: Evaluator = Accuracy) -> float:
         X_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=X_pred)
 
 
 class RDAClassifier(Estimator, Supervised):
-    
     """
-    Regularized Discriminant Analysis (RDA) combines the features of 
-    Linear Discriminant Analysis (LDA) and Quadratic Discriminant Analysis 
-    (QDA) by introducing regularization to the covariance matrices. It 
-    adjusts the covariance estimates with a blend between the pooled 
-    covariance (LDA approach) and class-specific covariances (QDA approach), 
-    enhancing classification performance. RDA is particularly effective in 
-    scenarios with high-dimensional data or when the number of samples is 
-    limited. The method employs regularization parameters to balance bias 
+    Regularized Discriminant Analysis (RDA) combines the features of
+    Linear Discriminant Analysis (LDA) and Quadratic Discriminant Analysis
+    (QDA) by introducing regularization to the covariance matrices. It
+    adjusts the covariance estimates with a blend between the pooled
+    covariance (LDA approach) and class-specific covariances (QDA approach),
+    enhancing classification performance. RDA is particularly effective in
+    scenarios with high-dimensional data or when the number of samples is
+    limited. The method employs regularization parameters to balance bias
     and variance, aiming to optimize model accuracy.
-    
+
     Parameters
     ----------
     `alpha` : Balancing parameter between the class-specific covariance matrices
     (0 for LDA-like, 1 for QDA-like approach)
     `gamma` : Shrinkage applied to the covariance matrices
     (0 for large shrinkage, i.e. max regularization)
-    
+
     """
-    
-    def __init__(self, 
-                 alpha: float = 0.5,
-                 gamma: float = 0.5) -> None:
+
+    def __init__(self, alpha: float = 0.5, gamma: float = 0.5) -> None:
         self.alpha = alpha
         self.gamma = gamma
         self.classes = None
         self.means = None
         self.priors = None
         self.covs = None
         self._fitted = False
-    
-    def fit(self, X: Matrix, y: Vector) -> 'RDAClassifier':
+
+        self.set_param_ranges({"alpha": ("0,+1", None), "gamma": ("0<,+inf", None)})
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix, y: Vector) -> "RDAClassifier":
         m, n = X.shape
         self.classes = np.unique(y)
         n_classes = len(self.classes)
-        
+
         self.means = np.zeros((n_classes, n))
         self.pooled_cov = np.zeros((n, n))
         self.covs = np.zeros((n_classes, n, n))
         self.priors = np.zeros(n_classes)
-        
+
         for i, cl in enumerate(self.classes):
             X_cls = X[y == cl]
             self.means[i] = np.mean(X_cls, axis=0)
             self.priors[i] = X_cls.shape[0] / m
             class_cov = np.cov(X_cls, rowvar=False)
             self.pooled_cov += class_cov * (X_cls.shape[0] - 1)
-        
-        self.pooled_cov /= (m - n_classes)
-        
+
+        self.pooled_cov /= m - n_classes
+
         for i in range(n_classes):
             X_cls = X[y == self.classes[i]]
             class_cov = np.cov(X_cls, rowvar=False)
             self.covs[i] = self.alpha * class_cov
-            self.covs[i] += (1 - self.alpha) *  self.pooled_cov
-            
+            self.covs[i] += (1 - self.alpha) * self.pooled_cov
+
             self.covs[i] = self.gamma * self.covs[i]
             self.covs[i] += (1 - self.gamma) * np.eye(n) * np.trace(self.covs[i])
             self.covs[i] /= n
-        
+
         self._fitted = True
         return self
-    
+
     def predict(self, X: Matrix) -> Vector:
-        if not self._fitted: raise not NotFittedError(self)
+        if not self._fitted:
+            raise not NotFittedError(self)
         return Vector([self._predict_sample(x) for x in X])
 
     def _predict_sample(self, x: Vector) -> Scalar:
         discs = np.zeros(len(self.classes))
         for i in range(len(self.classes)):
             diff = x - self.means[i]
             cov_inv = np.linalg.inv(self.covs[i])
             cov_det = np.linalg.det(self.covs[i])
-            
+
             disc = np.log(cov_det) + diff.T.dot(cov_inv).dot(diff)
             disc *= -0.5
             disc += np.log(self.priors[i])
             discs[i] = disc
-        
+
         return self.classes[np.argmax(discs)]
-    
+
     def predict_proba(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         log_probs = np.array([self._log_proba_sample(x) for x in X])
-        
+
         return softmax(log_probs, axis=1)
-    
+
     def _log_proba_sample(self, x: Vector) -> Vector:
         log_probs = np.zeros(len(self.classes))
         for i, _ in enumerate(self.classes):
             mvn = multivariate_normal(mean=self.means[i], cov=self.covs[i])
             log_probs[i] = mvn.logpdf(x) + np.log(self.priors[i])
-        
+
         return log_probs
-    
-    def score(self, X: Matrix, y: Matrix, 
-              metric: Evaluator = Accuracy) -> float:
+
+    def score(self, X: Matrix, y: Matrix, metric: Evaluator = Accuracy) -> float:
         X_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=X_pred)
 
 
 class KDAClassifier(Estimator, Supervised):
-    
     """
-    A Kernel Discriminant Analysis (KDA) classifier is an extension of 
-    traditional discriminant analysis methods that incorporates kernel 
-    techniques to perform classification tasks in a transformed, 
-    high-dimensional feature space. By applying a kernel function, it 
-    enables the classifier to find nonlinear boundaries between classes, 
-    enhancing its ability to handle complex patterns that are not linearly 
-    separable. The KDA classifier operates by projecting input data into 
-    a space where classes are maximally distant from each other, using 
-    the calculated projections to classify new instances based on their 
+    A Kernel Discriminant Analysis (KDA) classifier is an extension of
+    traditional discriminant analysis methods that incorporates kernel
+    techniques to perform classification tasks in a transformed,
+    high-dimensional feature space. By applying a kernel function, it
+    enables the classifier to find nonlinear boundaries between classes,
+    enhancing its ability to handle complex patterns that are not linearly
+    separable. The KDA classifier operates by projecting input data into
+    a space where classes are maximally distant from each other, using
+    the calculated projections to classify new instances based on their
     proximity to class centroids.
-    
+
     Parameters
     ----------
     `deg` : Polynomial degree of `poly` kernel
     `gamma` : Shape parameter of `rbf`, `sigmoid`, `laplacian`
     `coef` : Additional coefficient of `poly`, `sigmoid`
     `kernel` : Type of kernel functions
-    
+
     Notes
     -----
-    * To use KDA for dimensionality reduction, refer to 
+    * To use KDA for dimensionality reduction, refer to
         `luma.reduction.linear.KDA`
-    
+
     """
-    
-    def __init__(self, 
-                 deg: int = 2,
-                 gamma: float = 1.0,
-                 alpha: float = 1.0,
-                 coef: int = 0.0,
-                 kernel: KernelUtil.func_type = 'rbf') -> None:
+
+    def __init__(
+        self,
+        deg: int = 2,
+        gamma: float = 1.0,
+        coef: int = 0.0,
+        kernel: KernelUtil.FuncType = "rbf",
+    ) -> None:
         self.deg = deg
-        self.alpha = alpha
         self.gamma = gamma
         self.coef = coef
         self.kernel = kernel
         self.X_ = None
         self._fitted = False
-        
+
         self.kernel_params = {
-            'deg': self.deg,
-            'alpha': self.alpha,
-            'gamma': self.gamma,
-            'coef': self.coef
+            "deg": self.deg,
+            "alpha": self.alpha,
+            "gamma": self.gamma,
+            "coef": self.coef,
         }
-    
-    def fit(self, X: Matrix, y: Vector) -> 'KDAClassifier':
+
+        self.set_param_ranges({"deg": ("0,+inf", int), "gamma": ("0<,+inf", None)})
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix, y: Vector) -> "KDAClassifier":
         m, _ = X.shape
         self._X = X
         self.classes = np.unique(y)
         self.n_classes = len(self.classes)
-        
+
         self.ku_ = KernelUtil(self.kernel, **self.kernel_params)
         self.class_means = np.zeros((self.n_classes, m))
-        
+
         self.K = self.ku_.kernel_func(X)
         for i, cl in enumerate(self.classes):
             self.class_means[i] = np.mean(self.K[y == cl], axis=0)
-        
+
         self._fitted = False
         return self
-    
+
     def _project(self, X: Matrix) -> Vector:
         K = self.ku_.kernel_func(X, self._X)
         proj = np.dot(K, self.class_means.T)
         return proj
-    
+
     def predict(self, X: Matrix) -> Vector:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         proj = self._project(X)
-        
+
         return self.classes[np.argmax(proj, axis=1)]
-    
+
     def predict_proba(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         proj = self._project(X)
-        
+
         return softmax(proj, axis=1)
-    
-    def score(self, X: Matrix, y: Matrix, 
-              metric: Evaluator = Accuracy) -> float:
+
+    def score(self, X: Matrix, y: Matrix, metric: Evaluator = Accuracy) -> float:
         X_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=X_pred)
-
```

### Comparing `luma-ml-0.6.4/luma/classifier/logistic.py` & `luma-ml-0.6.5/luma/classifier/logistic.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,194 +3,220 @@
 
 from luma.interface.util import Matrix
 from luma.metric.classification import Accuracy
 from luma.interface.exception import NotFittedError, UnsupportedParameterError
 from luma.core.super import Estimator, Evaluator, Supervised
 
 
-__all__ = (
-    'LogisticRegressor', 
-    'SoftmaxRegressor'
-)
+__all__ = ("LogisticRegressor", "SoftmaxRegressor")
 
 
 class LogisticRegressor(Estimator, Supervised):
-    
     """
-    Logistic regression is a statistical model used for binary classification, 
+    Logistic regression is a statistical model used for binary classification,
     which means it's employed to predict one of two possible outcomes.
-    It does this by modeling the relationship between one or more 
+    It does this by modeling the relationship between one or more
     input variables and the probability of the binary outcome.
-    
+
     Parameters
     ----------
     `learning_rate` : Step size of the gradient descent update
     `max_iter` : Number of iteration
     `l1_ratio` : Balancing parameter of `elastic-net`
     `alpha` : Regularization strength
     `regularization` : Regularization type (e.g. `l1`, `l2`, `elastic-net`)
-    
+
     """
-    
-    def __init__(self, 
-                 learning_rate : float = 0.01, 
-                 max_iter: int = 100, 
-                 l1_ratio: float = 0.5, 
-                 alpha: float = 0.01, 
-                 regularization: Literal['l1', 'l2', 'elastic-net'] = None,
-                 verbose: bool = False):
+
+    def __init__(
+        self,
+        learning_rate: float = 0.01,
+        max_iter: int = 100,
+        l1_ratio: float = 0.5,
+        alpha: float = 0.01,
+        regularization: Literal["l1", "l2", "elastic-net"] = None,
+        verbose: bool = False,
+    ):
         self.learning_rate = learning_rate
         self.max_iter = max_iter
         self.l1_ratio = l1_ratio
         self.regularization = regularization
         self.alpha = alpha
         self.verbose = verbose
         self._fitted = False
 
+        self.set_param_ranges(
+            {
+                "learning_rate": ("0<,+inf", None),
+                "max_iter": ("0<,+inf", int),
+                "l1_ratio": ("0,1", None),
+                "alpha": ("0,+inf", None),
+            }
+        )
+        self.check_param_ranges()
+
     def sigmoid(self, z: Matrix) -> Matrix:
         return 1 / (1 + np.exp(-z))
 
-    def fit(self, X: Matrix, y: Matrix) -> 'LogisticRegressor':
+    def fit(self, X: Matrix, y: Matrix) -> "LogisticRegressor":
         X = np.insert(X, 0, 1, axis=1)
         m, n = X.shape
         self.theta = np.zeros(n)
 
         for i in range(self.max_iter):
             z = np.dot(X, self.theta)
             h = self.sigmoid(z)
             gradient = np.dot(X.T, (h - y)) * self.learning_rate
             gradient += self.alpha * self._regularization_term() / m
             gradient[0] -= self.alpha * self._regularization_term()[0]
             self.theta -= gradient
-            
-            if self.verbose and i % 10 == 0: 
-                print(f'[LogisticReg] iteration: {i}/{self.max_iter}', end='')
-                print(f' - gradient-norm: {np.linalg.norm(gradient)}')
-        
+
+            if self.verbose and i % 10 == 0:
+                print(f"[LogisticReg] iteration: {i}/{self.max_iter}", end="")
+                print(f" - gradient-norm: {np.linalg.norm(gradient)}")
+
         self._fitted = True
         return self
 
     def _regularization_term(self) -> Matrix:
-        if self.regularization == 'l1': return np.sign(self.theta)
-        elif self.regularization == 'l2': return self.theta
-        elif self.regularization == 'elastic-net':
+        if self.regularization == "l1":
+            return np.sign(self.theta)
+        elif self.regularization == "l2":
+            return self.theta
+        elif self.regularization == "elastic-net":
             l1_term = np.sign(self.theta)
             l2_term = 2 * self.theta
             return (1 - self.l1_ratio) * l2_term + self.l1_ratio * l1_term
-        elif self.regularization is None: return np.zeros_like(self.theta)
-        else: raise UnsupportedParameterError(self.regularization)
+        elif self.regularization is None:
+            return np.zeros_like(self.theta)
+        else:
+            raise UnsupportedParameterError(self.regularization)
 
     def predict(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         X = np.insert(X, 0, 1, axis=1)
         z = np.dot(X, self.theta)
         h = self.sigmoid(z)
         predictions = (h >= 0.5).astype(int)
         return predictions
-    
+
     def predict_proba(self, X: Matrix) -> Matrix:
         X = np.insert(X, 0, 1, axis=1)
         z = np.dot(X, self.theta)
         h = self.sigmoid(z)
         return h
-    
-    def score(self, X: Matrix, y: Matrix, 
-              metric: Evaluator = Accuracy) -> float:
+
+    def score(self, X: Matrix, y: Matrix, metric: Evaluator = Accuracy) -> float:
         X_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=X_pred)
 
 
 class SoftmaxRegressor(Estimator, Supervised):
-    
     """
-    Softmax regression, also known as multinomial logistic regression, 
-    is a supervised machine learning technique used for classification tasks. 
-    It's an extension of logistic regression, 
+    Softmax regression, also known as multinomial logistic regression,
+    is a supervised machine learning technique used for classification tasks.
+    It's an extension of logistic regression,
     but it can handle multiple classes (more than two).
-    
+
     Parameters
     ----------
     `learning_rate` : Step size of the gradient descent update
     `max_iter` : Number of iteration
-    `l1_ratio` : Balancing parameter of `elastic-net` 
+    `l1_ratio` : Balancing parameter of `elastic-net`
     `alpha` : Regularization strength
     `regularization` : Regularization type (e.g. `l1`, `l2`, `elastic-net`)
-    
+
     """
-    
-    def __init__(self,
-                 learning_rate: float = 0.01,
-                 max_iter: int = 100,
-                 l1_ratio: float = 0.5,
-                 alpha: float = 0.01,
-                 regularization: Literal['l1', 'l2', 'elastic-net'] = None,
-                 verbose: bool = False) -> None:
+
+    def __init__(
+        self,
+        learning_rate: float = 0.01,
+        max_iter: int = 100,
+        l1_ratio: float = 0.5,
+        alpha: float = 0.01,
+        regularization: Literal["l1", "l2", "elastic-net"] = None,
+        verbose: bool = False,
+    ) -> None:
         self.learning_rate = learning_rate
         self.max_iter = max_iter
         self.l1_ratio = l1_ratio
         self.alpha = alpha
         self.regularization = regularization
         self.verbose = verbose
         self._fitted = False
-    
+
+        self.set_param_ranges(
+            {
+                "learning_rate": ("0<,+inf", None),
+                "max_iter": ("0<,+inf", int),
+                "l1_ratio": ("0,1", None),
+                "alpha": ("0,+inf", None),
+            }
+        )
+        self.check_param_ranges()
+
     def softmax(self, z: Matrix) -> Matrix:
         exp_z = np.exp(z - np.max(z, axis=1, keepdims=True))
         return exp_z / exp_z.sum(axis=1, keepdims=True)
 
-    def fit(self, X: Matrix, y: Matrix) -> 'SoftmaxRegressor':
+    def fit(self, X: Matrix, y: Matrix) -> "SoftmaxRegressor":
         X = np.insert(X, 0, 1, axis=1)
         m, n = X.shape
         num_classes = len(np.unique(y))
         self.theta = np.zeros((n, num_classes))
-        
+
         for i in range(self.max_iter):
             z = np.dot(X, self.theta)
             h = self.softmax(z)
             gradient = np.dot(X.T, (h - self._one_hot_encode(y)))
             gradient *= self.learning_rate
             gradient += self.alpha * self._regularization_term() / m
             gradient[0] -= self.alpha * self._regularization_term()[0]
             self.theta -= gradient
-            
-            if self.verbose and i % 10 == 0: 
-                print(f'[SoftmaxReg] iteration: {i}/{self.max_iter}', end='')
-                print(f' - gradient-norm: {np.linalg.norm(gradient)}')
-        
+
+            if self.verbose and i % 10 == 0:
+                print(f"[SoftmaxReg] iteration: {i}/{self.max_iter}", end="")
+                print(f" - gradient-norm: {np.linalg.norm(gradient)}")
+
         self._fitted = True
         return self
-    
+
     def _one_hot_encode(self, y: Matrix) -> Matrix:
         num_classes = self.theta.shape[1]
         one_hot = np.zeros((len(y), num_classes))
         for i in range(len(y)):
             one_hot[i, y[i]] = 1
         return one_hot
-    
+
     def _regularization_term(self) -> Matrix:
-        if self.regularization == 'l1': return np.sign(self.theta)
-        elif self.regularization == 'l2': return self.theta
-        elif self.regularization == 'elastic-net':
+        if self.regularization == "l1":
+            return np.sign(self.theta)
+        elif self.regularization == "l2":
+            return self.theta
+        elif self.regularization == "elastic-net":
             l1_term = np.sign(self.theta)
             l2_term = 2 * self.theta
             return (1 - self.l1_ratio) * l2_term + self.l1_ratio * l1_term
-        elif self.regularization is None: return np.zeros_like(self.theta)
-        else: raise UnsupportedParameterError(self.regularization)
-    
+        elif self.regularization is None:
+            return np.zeros_like(self.theta)
+        else:
+            raise UnsupportedParameterError(self.regularization)
+
     def predict(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         X = np.insert(X, 0, 1, axis=1)
         z = np.dot(X, self.theta)
         h = self.softmax(z)
         predictions = np.argmax(h, axis=1)
         return predictions
-    
+
     def predict_proba(self, X: Matrix) -> Matrix:
         X = np.insert(X, 0, 1, axis=1)
         z = np.dot(X, self.theta)
         h = self.softmax(z)
         return h
-    
-    def score(self, X: Matrix, y: Matrix, 
-              metric: Evaluator = Accuracy) -> float:
+
+    def score(self, X: Matrix, y: Matrix, metric: Evaluator = Accuracy) -> float:
         X_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=X_pred)
-
```

### Comparing `luma-ml-0.6.4/luma/classifier/naive_bayes.py` & `luma-ml-0.6.5/luma/classifier/naive_bayes.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,53 +3,48 @@
 
 from luma.interface.util import Matrix, Vector
 from luma.interface.exception import NotFittedError
 from luma.core.super import Estimator, Evaluator, Supervised
 from luma.metric.classification import Accuracy
 
 
-__all__ = (
-    'GaussianNaiveBayes', 
-    'BernoulliNaiveBayes'
-)
+__all__ = ("GaussianNaiveBayes", "BernoulliNaiveBayes")
 
 
 class GaussianNaiveBayes(Estimator, Supervised):
-    
     """
-    Gaussian Naive Bayes is a probabilistic classification algorithm. 
-    It's based on Bayes' theorem and makes an assumption 
+    Gaussian Naive Bayes is a probabilistic classification algorithm.
+    It's based on Bayes' theorem and makes an assumption
     that the features follow a Gaussian distribution.
     """
 
     def __init__(self) -> None:
         self._fitted = False
-    
-    def fit(self, X: Matrix, y: Matrix) -> 'GaussianNaiveBayes':
+
+    def fit(self, X: Matrix, y: Matrix) -> "GaussianNaiveBayes":
         self.classes = np.unique(y)
         self.parameters = []
         self.priors = []
         self.X_train = X
         self.y_train = y
-        
+
         shared_cov_matrix = np.zeros((X.shape[1], X.shape[1]))
         for c in self.classes:
             X_c = X[y == c]
             cov_matrix = np.diag(X_c.var(axis=0))
             shared_cov_matrix += cov_matrix
             self.parameters.append([X_c.mean(axis=0), cov_matrix])
-        
+
         for params in self.parameters:
             params[1] = shared_cov_matrix / len(self.classes)
-        
+
         self._fitted = True
         return self
-        
-    def _calculate_likelihood(self, x: Matrix, mean: Matrix, 
-                              cov: Matrix) -> float:
+
+    def _calculate_likelihood(self, x: Matrix, mean: Matrix, cov: Matrix) -> float:
         dim = len(mean)
         dev = x - mean
         cov_inv = np.linalg.inv(cov)
         exponent = -0.5 * np.dot(dev, np.dot(cov_inv, dev))
         norm_term = 1 / np.sqrt((2 * np.pi) ** dim * np.linalg.det(cov))
         return norm_term * np.exp(exponent)
 
@@ -62,96 +57,100 @@
             prior = self._calculate_prior(c)
             likelihood = self._calculate_likelihood(x, *self.parameters[i])
             posterior = prior * likelihood
             posteriors.append(posterior)
         return self.classes[np.argmax(posteriors)]
 
     def predict(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         return Matrix([self._classify_sample(x) for x in X])
 
     def predict_proba(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         probabilities = []
         for x in X:
             posteriors = []
             for i, c in enumerate(self.classes):
                 prior = self._calculate_prior(c)
                 likelihood = self._calculate_likelihood(x, *self.parameters[i])
-                
+
                 posterior = prior * likelihood
                 posteriors.append(posterior)
-            
+
             posteriors = Vector(posteriors)
-            probabilities.append(posteriors / np.sum(posteriors))  
-                
+            probabilities.append(posteriors / np.sum(posteriors))
+
         return Matrix(probabilities)
-    
-    def score(self, X: Matrix, y: Matrix, 
-              metric: Evaluator = Accuracy) -> float:
+
+    def score(self, X: Matrix, y: Matrix, metric: Evaluator = Accuracy) -> float:
         X_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=X_pred)
 
 
 class BernoulliNaiveBayes(Estimator, Supervised):
-    
     """
-    Bernoulli Naive Bayes is a classification algorithm based on 
-    Bayes' theorem, which assumes that the features are binary 
-    (i.e., they are either present or absent) and that they are 
+    Bernoulli Naive Bayes is a classification algorithm based on
+    Bayes' theorem, which assumes that the features are binary
+    (i.e., they are either present or absent) and that they are
     conditionally independent given the class label.
     """
-    
+
     def __init__(self) -> None:
         self._fitted = False
-    
-    def fit(self, X: Matrix, y: Matrix) -> 'BernoulliNaiveBayes':
+
+    def fit(self, X: Matrix, y: Matrix) -> "BernoulliNaiveBayes":
         self.classes = np.unique(y)
         self.class_probs = np.zeros(len(self.classes))
         self.feature_probs = np.zeros((len(self.classes), X.shape[1]))
 
         for i, c in enumerate(self.classes):
             X_cls = X[y == c]
             self.class_probs[i] = len(X_cls) / len(y)
             self.feature_probs[i] = (X_cls.sum(axis=0) + 1) / (len(X_cls) + 2)
-        
+
         self._fitted = True
         return self
 
     def predict(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         predictions = []
         for x in X:
             class_scores = np.zeros(len(self.classes))
             for i, _ in enumerate(self.classes):
                 class_scores[i] = np.log(self.class_probs[i])
                 for j, feature in enumerate(x):
-                    if feature == 1: class_scores[i] += np.log(self.feature_probs[i, j])
-                    else: class_scores[i] += np.log(1 - self.feature_probs[i, j])
+                    if feature == 1:
+                        class_scores[i] += np.log(self.feature_probs[i, j])
+                    else:
+                        class_scores[i] += np.log(1 - self.feature_probs[i, j])
 
             predicted_class = self.classes[np.argmax(class_scores)]
             predictions.append(predicted_class)
-        
+
         return Matrix(predictions)
-    
+
     def predict_proba(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         probas = []
         for x in X:
             class_probs = np.zeros(len(self.classes))
-            
+
             for i, _ in enumerate(self.classes):
                 class_probs[i] = np.log(self.class_probs[i])
                 for j, feature in enumerate(x):
-                    if feature == 1: class_probs[i] += np.log(self.feature_probs[i, j])
-                    else: class_probs[i] += np.log(1 - self.feature_probs[i, j])
+                    if feature == 1:
+                        class_probs[i] += np.log(self.feature_probs[i, j])
+                    else:
+                        class_probs[i] += np.log(1 - self.feature_probs[i, j])
 
             exp_class_probs = np.exp(class_probs - np.max(class_probs))
             probas.append(exp_class_probs / exp_class_probs.sum())
-        
+
         return Matrix(probas)
-    
-    def score(self, X: Matrix, y: Matrix, 
-              metric: Evaluator = Accuracy) -> float:
+
+    def score(self, X: Matrix, y: Matrix, metric: Evaluator = Accuracy) -> float:
         X_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=X_pred)
-
```

### Comparing `luma-ml-0.6.4/luma/classifier/neighbors.py` & `luma-ml-0.6.5/luma/classifier/neighbors.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,238 +4,252 @@
 from luma.interface.util import Matrix
 from luma.core.super import Estimator, Supervised, Evaluator
 from luma.interface.util import NearestNeighbors
 from luma.interface.exception import NotFittedError
 from luma.metric.classification import Accuracy
 
 
-__all__ = (
-    'KNNClassifier', 
-    'AdaptiveKNNClassifier', 
-    'WeightedKNNClassifier'
-)
+__all__ = ("KNNClassifier", "AdaptiveKNNClassifier", "WeightedKNNClassifier")
 
 
 class KNNClassifier(Estimator, Supervised):
-    
     """
-    The K-Nearest Neighbors (KNN) classifier is a simple and intuitive 
-    machine learning algorithm that classifies a new data point based on 
-    the majority class among its closest neighbors. It operates by 
-    calculating the distance (such as Euclidean distance) between the 
-    new point and all points in the training set, identifying the 'k' 
-    nearest neighbors, and then performing a majority vote among these 
+    The K-Nearest Neighbors (KNN) classifier is a simple and intuitive
+    machine learning algorithm that classifies a new data point based on
+    the majority class among its closest neighbors. It operates by
+    calculating the distance (such as Euclidean distance) between the
+    new point and all points in the training set, identifying the 'k'
+    nearest neighbors, and then performing a majority vote among these
     neighbors to determine the class label.
-    
+
     Parameters
     ----------
     `n_neighbors` : Number of neighbors to be considered close
-    
+
     """
-    
+
     def __init__(self, n_neighbors: int = 5):
         self.n_neighbors = n_neighbors
         self._neighbors = None
         self._y = None
         self._fitted = False
 
-    def fit(self, X: Matrix, y: Matrix) -> 'KNNClassifier':
+        self.set_param_ranges({"n_neighbors": ("0,+inf", int)})
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix, y: Matrix) -> "KNNClassifier":
         self._neighbors = NearestNeighbors(X, self.n_neighbors)
         self._y = y
         self._fitted = True
         return self
 
     def predict(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         predictions = []
-        
+
         for x in X:
             distances = np.linalg.norm(self._neighbors.data - x, axis=1)
-            nearest_neighbor_ids = np.argsort(distances)[:self.n_neighbors]
+            nearest_neighbor_ids = np.argsort(distances)[: self.n_neighbors]
             nearest_neighbor_labels = self._y[nearest_neighbor_ids]
-            
+
             most_common_label = np.bincount(nearest_neighbor_labels).argmax()
             predictions.append(most_common_label)
 
         return Matrix(predictions)
-    
+
     def predict_proba(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         proba = []
-        
+
         for x in X:
             distances = np.linalg.norm(self._neighbors.data - x, axis=1)
-            nearest_neighbor_ids = np.argsort(distances)[:self.n_neighbors]
+            nearest_neighbor_ids = np.argsort(distances)[: self.n_neighbors]
             nearest_neighbor_labels = self._y[nearest_neighbor_ids]
-            
-            class_votes = np.bincount(nearest_neighbor_labels, 
-                                      minlength=np.max(self._y) + 1)
-            
+
+            class_votes = np.bincount(
+                nearest_neighbor_labels, minlength=np.max(self._y) + 1
+            )
+
             class_probabilities = class_votes / self.n_neighbors
             proba.append(class_probabilities)
-        
+
         return Matrix(proba)
 
-    def score(self, X: Matrix, y: Matrix, 
-              metric: Evaluator = Accuracy) -> float:
+    def score(self, X: Matrix, y: Matrix, metric: Evaluator = Accuracy) -> float:
         X_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=X_pred)
 
 
 class AdaptiveKNNClassifier(Estimator, Supervised):
-    
     """
-    The Adaptive K-Nearest Neighbors (AdaKNN) Classifier is an extension 
-    of the conventional KNN algorithm for classification. It classifies a 
-    new data point based on the majority class among its neighbors, where 
-    the number of neighbors (k) is adaptively determined based on the local 
-    density of the training data. This adaptive approach allows the algorithm 
-    to be more flexible and effective, especially in datasets with varying 
+    The Adaptive K-Nearest Neighbors (AdaKNN) Classifier is an extension
+    of the conventional KNN algorithm for classification. It classifies a
+    new data point based on the majority class among its neighbors, where
+    the number of neighbors (k) is adaptively determined based on the local
+    density of the training data. This adaptive approach allows the algorithm
+    to be more flexible and effective, especially in datasets with varying
     densities.
-    
+
     Parameters
     ----------
     `n_density` : Number of nearest neighbors to estimate the local density
     `min_neighbors` : Minimum number of neighbors to be considered for averaging
     `max_neighbors` : Maximum number of neighbors to be considered
-    
+
     """
-    
-    def __init__(self, 
-                 n_density: int = 10, 
-                 min_neighbors: int = 5, 
-                 max_neighbors: int = 20):
+
+    def __init__(
+        self, n_density: int = 10, min_neighbors: int = 5, max_neighbors: int = 20
+    ):
         self.n_density = n_density
         self.min_neighbors = min_neighbors
         self.max_neighbors = max_neighbors
         self._X = None
         self._y = None
         self._fitted = False
 
-    def fit(self, X: Matrix, y: Matrix) -> 'AdaptiveKNNClassifier':
+        self.set_param_ranges(
+            {
+                "n_density": ("0<,+int", int),
+                "min_neighbors": ("0<,+int", int),
+                "max_neighbors": ("0<,+int", int),
+            }
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix, y: Matrix) -> "AdaptiveKNNClassifier":
         self._X = X
         self._y = y
-        
+
         self.dist_matrix = distance_matrix(X, X)
         self.local_density = np.sort(self.dist_matrix, axis=1)
         self.local_density = self.local_density[:, self.n_density]
-        
-        self.k_values = np.clip(np.ceil(self.max_neighbors / self.local_density), 
-                           self.min_neighbors, self.max_neighbors).astype(int)
-        
+
+        self.k_values = np.clip(
+            np.ceil(self.max_neighbors / self.local_density),
+            self.min_neighbors,
+            self.max_neighbors,
+        ).astype(int)
+
         self._fitted = True
         return self
 
     def predict(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         dist_matrix = distance_matrix(X, self._X)
-        
+
         predictions = []
         for point_distances in dist_matrix:
             nearest_indices = np.argsort(point_distances)
             votes = np.zeros(len(np.unique(self._y)))
 
             for idx, _ in enumerate(point_distances[nearest_indices]):
-                if idx >= self.k_values[nearest_indices[idx]]: break
+                if idx >= self.k_values[nearest_indices[idx]]:
+                    break
                 votes[self._y[nearest_indices[idx]]] += 1
 
             most_common = np.argmax(votes)
             predictions.append(most_common)
 
         return Matrix(predictions)
-    
+
     def predict_proba(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         dist_matrix = distance_matrix(X, self._X)
-        
+
         proba_predictions = []
         for i, point_distances in enumerate(dist_matrix):
             nearest_indices = np.argsort(point_distances)
             k_value = min(self.k_values[i], len(nearest_indices))
             nearest_indices = nearest_indices[:k_value]
-            
+
             votes = np.zeros(np.max(self._y) + 1)
             for idx in nearest_indices:
                 votes[self._y[idx]] += 1
-            
+
             class_probabilities = votes / votes.sum()
             proba_predictions.append(class_probabilities)
 
         return Matrix(proba_predictions)
 
-    def score(self, X: Matrix, y: Matrix, 
-              metric: Evaluator = Accuracy) -> float:
+    def score(self, X: Matrix, y: Matrix, metric: Evaluator = Accuracy) -> float:
         X_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=X_pred)
 
 
 class WeightedKNNClassifier(Estimator, Supervised):
-    
     """
-    The Weighted KNN Classifier is a variation of the k-Nearest Neighbors algorithm 
-    where neighbors contribute to the classification decision based on their distance 
-    from the query point. Closer neighbors have more influence as they are assigned 
-    higher weights, typically using inverse distance weighting. This approach enhances 
+    The Weighted KNN Classifier is a variation of the k-Nearest Neighbors algorithm
+    where neighbors contribute to the classification decision based on their distance
+    from the query point. Closer neighbors have more influence as they are assigned
+    higher weights, typically using inverse distance weighting. This approach enhances
     prediction accuracy, especially in unevenly distributed datasets.
-    
+
     Parameters
     ----------
     `n_neighbors` : Number of neighbors to be considered close
-    
+
     """
-    
+
     def __init__(self, n_neighbors: int = 5):
         self.n_neighbors = n_neighbors
         self._X = None
         self._y = None
         self._fitted = False
 
-    def fit(self, X: Matrix, y: Matrix) -> 'WeightedKNNClassifier':
+        self.set_param_ranges({"n_neighbors": ("0,+inf", int)})
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix, y: Matrix) -> "WeightedKNNClassifier":
         self._X = X
         self._y = y
-        
+
         self._fitted = True
         return self
 
     def predict(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         predictions = np.zeros(X.shape[0])
 
         for i, x in enumerate(X):
             distances = np.linalg.norm(self._X - x, axis=1)
-            nearest_neighbors = np.argsort(distances)[:self.n_neighbors]
+            nearest_neighbors = np.argsort(distances)[: self.n_neighbors]
 
             weights = 1 / (distances[nearest_neighbors] + 1e-5)
             weighted_votes = np.zeros(np.unique(self._y).shape[0])
             for idx, neighbor in enumerate(nearest_neighbors):
                 weighted_votes[self._y[neighbor]] += weights[idx]
 
             predictions[i] = np.argmax(weighted_votes)
 
         return predictions.astype(int)
-    
+
     def predict_proba(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         proba_predictions = []
-        
+
         for x in X:
             distances = np.linalg.norm(self._X - x, axis=1)
-            nearest_neighbor_indices = np.argsort(distances)[:self.n_neighbors]
-            
+            nearest_neighbor_indices = np.argsort(distances)[: self.n_neighbors]
+
             weights = 1 / (distances[nearest_neighbor_indices] + 1e-5)
             all_classes = np.unique(self._y)
             weighted_votes = np.zeros(len(all_classes))
-            
+
             for i, cl in enumerate(all_classes):
                 class_weights = weights[self._y[nearest_neighbor_indices] == cl]
                 weighted_votes[i] = np.sum(class_weights)
-            
+
             class_probabilities = weighted_votes / np.sum(weighted_votes)
             proba_predictions.append(class_probabilities)
-        
+
         return Matrix(proba_predictions)
-    
-    def score(self, X: Matrix, y: Matrix, 
-              metric: Evaluator = Accuracy) -> float:
+
+    def score(self, X: Matrix, y: Matrix, metric: Evaluator = Accuracy) -> float:
         X_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=X_pred)
-
```

### Comparing `luma-ml-0.6.4/luma/classifier/svm.py` & `luma-ml-0.6.5/luma/classifier/svm.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,234 +2,258 @@
 
 from luma.interface.util import Matrix, KernelUtil
 from luma.interface.exception import NotFittedError
 from luma.core.super import Estimator, Evaluator, Supervised
 from luma.metric.classification import Accuracy
 
 
-__all__ = (
-    'SVC', 
-    'KernelSVC'
-)
+__all__ = ("SVC", "KernelSVC")
 
 
 class SVC(Estimator, Supervised):
-    
     """
-    Support Vector Classifier (SVC) is a supervised machine learning 
-    algorithm mainly used for classification tasks. It operates by 
-    determining a hyperplane that best separates different classes in 
-    the input data, aiming to maximize the margin between the hyperplane 
+    Support Vector Classifier (SVC) is a supervised machine learning
+    algorithm mainly used for classification tasks. It operates by
+    determining a hyperplane that best separates different classes in
+    the input data, aiming to maximize the margin between the hyperplane
     and the nearest data points from each class.
-    
+
     Parameters
     ----------
     `C` : Regularization parameter
     `batch_size` : Size of a single batch
     `learning_rate` : Step-size of gradient descent update
     `max_iter` : Number of iteration
-    
+
     """
-    
-    def __init__(self, 
-                 C: float = 1.0, 
-                 batch_size: int = 100, 
-                 learning_rate: float = 0.001, 
-                 max_iter: int = 1000, 
-                 verbose: bool = False) -> None:
+
+    def __init__(
+        self,
+        C: float = 1.0,
+        batch_size: int = 100,
+        learning_rate: float = 0.001,
+        max_iter: int = 1000,
+        verbose: bool = False,
+    ) -> None:
         self.C = C
         self.batch_size = batch_size
         self.learning_rate = learning_rate
         self.max_iter = max_iter
         self.verbose = verbose
         self._fitted = False
-        
-    def fit(self, X: Matrix, y: Matrix) -> 'SVC':
+
+        self.set_param_ranges(
+            {
+                "C": ("0,+inf", None),
+                "batch_size": ("0<,+int", int),
+                "learning_rate": ("0<,+inf", None),
+                "max_iter": ("0,+inf", int),
+            }
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix, y: Matrix) -> "SVC":
         classes = np.unique(y)
         self.models = []
         for cl in classes:
             binary_y = np.where(y == cl, 1, -1)
             self._binary_fit(X, binary_y, cl)
             if self.verbose:
-                print(f'[SVC] Finished OvR fit for class {cl}\n')
-        
+                print(f"[SVC] Finished OvR fit for class {cl}\n")
+
         self._fitted = True
         return self
 
     def _binary_fit(self, X: Matrix, y: Matrix, label: int) -> None:
         m, n = X.shape
         id = np.arange(m)
         np.random.shuffle(id)
 
         bias = 0.0
         weight = np.zeros(n)
-        
+
         for i in range(self.max_iter):
             for batch_point in range(0, m, self.batch_size):
                 gradient_w, gradient_b = 0, 0
                 for j in range(batch_point, batch_point + self.batch_size):
-                    if j >= m: continue
+                    if j >= m:
+                        continue
                     idx = id[j]
                     disc = y[idx] * (np.dot(weight, X[idx].T) + bias)
                     if disc <= 1:
                         gradient_w += self.C * y[idx] * X[idx]
                         gradient_b += self.C * y[idx]
 
                 weight -= self.learning_rate * weight
                 weight += self.learning_rate * gradient_w
                 bias += self.learning_rate * gradient_b
 
             if self.verbose and i % 100 == 0 and i:
-                print(f'[SVC] Finished iteration {i}/{self.max_iter}', end=' ')
-                print(f'with weight-norm of {np.linalg.norm(weight)}')
+                print(f"[SVC] Finished iteration {i}/{self.max_iter}", end=" ")
+                print(f"with weight-norm of {np.linalg.norm(weight)}")
 
         self.models.append((label, weight.copy(), bias))
-    
+
     def predict(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         scores = np.zeros((X.shape[0], len(self.models)))
 
         for i, (_, weight, bias) in enumerate(self.models):
             pred = np.dot(X, weight) + bias
             scores[:, i] = pred
-        
+
         return np.argmax(scores, axis=1)
 
-    def score(self, X: Matrix, y: Matrix, 
-              metric: Evaluator = Accuracy) -> float:
+    def score(self, X: Matrix, y: Matrix, metric: Evaluator = Accuracy) -> float:
         X_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=X_pred)
 
 
 class KernelSVC(Estimator, Supervised):
-    
     """
     Kernel Support Vector Classification (SVC) with batch-based learning.
     This approach processes the training data in batches, making it suitable
     for large datasets that cannot fit into memory at once.
-    
+
     Parameters
     ----------
     `C` : Regularization parameter
     `deg` : Polynomial Degree for `poly` kernel
     `gamma` : Shape parameter of Gaussian curve for `rbf` kernel
     `coef` : Coefficient for `poly`, `sigmoid` kernel
     `learning_rate` : Step-size for gradient descent update
     `max_iter` : Number of iteration
     `batch_size`: Size of the batch for batch-based learning
     `kernel` : Type of kernel (e.g., `linear`, `poly`, `rbf`, `sigmoid`)
-    
+
     """
-    
-    def __init__(self,
-                 C: float = 1.0,
-                 deg: int = 3,
-                 gamma: float = 1.0,
-                 coef: float = 1.0,
-                 learning_rate: float = 0.001,
-                 max_iter: int = 1000,
-                 batch_size: int = 100, 
-                 kernel: KernelUtil.func_type = 'rbf',
-                 verbose: bool = False) -> None:
+
+    def __init__(
+        self,
+        C: float = 1.0,
+        deg: int = 3,
+        gamma: float = 1.0,
+        coef: float = 1.0,
+        learning_rate: float = 0.001,
+        max_iter: int = 1000,
+        batch_size: int = 100,
+        kernel: KernelUtil.FuncType = "rbf",
+        verbose: bool = False,
+    ) -> None:
         self.C = C
         self.deg = deg
         self.gamma = gamma
         self.coef = coef
         self.learning_rate = learning_rate
         self.max_iter = max_iter
         self.batch_size = batch_size
         self.kernel = kernel
         self.verbose = verbose
         self._kernel_func = None
         self._fitted = False
-    
-    def fit(self, X: Matrix, y: Matrix) -> 'KernelSVC':
+
+        self.set_param_ranges(
+            {
+                "C": ("0,+inf", None),
+                "batch_size": ("0<,+int", int),
+                "learning_rate": ("0<,+inf", None),
+                "max_iter": ("0,+inf", int),
+                "deg": ("0,+inf", int),
+                "gamma": ("0,+inf", None),
+            }
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix, y: Matrix) -> "KernelSVC":
         classes = np.unique(y)
         self.models = []
         self._set_kernel_func()
-        
+
         for cl in classes:
             binary_y = np.where(y == cl, 1, -1)
             self._binary_fit(X, binary_y, cl)
             if self.verbose:
-                print(f'[KernelSVC] Finished OvR fit for class {cl}')
-        
+                print(f"[KernelSVC] Finished OvR fit for class {cl}")
+
         self._X = X
         self._y = y
         self._fitted = True
         return self
 
     def _binary_fit(self, X: Matrix, y: Matrix, label: int) -> None:
         m, _ = X.shape
         self.alpha = np.zeros(m)
         self.bias = 0
-        
+
         batch_size = min(self.batch_size, m)
         for i in range(self.max_iter):
             for start in range(0, m, batch_size):
                 end = start + batch_size
                 X_batch = X[start:end]
                 y_batch = y[start:end]
-                
-                y_mul_kernel = np.outer(y_batch, y_batch) \
-                    * self._kernel_func(X_batch, X_batch)
-                
+
+                y_mul_kernel = np.outer(y_batch, y_batch) * self._kernel_func(
+                    X_batch, X_batch
+                )
+
                 gradient = np.ones(y_batch.shape[0])
                 gradient -= y_mul_kernel.dot(self.alpha[start:end])
-                
+
                 self.alpha[start:end] += self.learning_rate * gradient
                 self.alpha[start:end] = np.clip(self.alpha[start:end], 0, self.C)
-            
+
             if self.verbose and i % 100 == 0:
-                print(f'[KernelSVC] Finished iteration {i}/{self.max_iter}',
-                      f'with alpha-norm: {np.linalg.norm(self.alpha)}')
-        
+                print(
+                    f"[KernelSVC] Finished iteration {i}/{self.max_iter}",
+                    f"with alpha-norm: {np.linalg.norm(self.alpha)}",
+                )
+
         self._update_bias(X, y)
         self.models.append((label, X, y, self.alpha.copy(), self.bias))
 
     def _update_bias(self, X: Matrix, y: Matrix) -> None:
         alpha_idx = np.where((self.alpha > 0) & (self.alpha < self.C))[0]
         bias_list = []
         for idx in alpha_idx:
             _append = y[idx] - (self.alpha * y).dot(self._kernel_func(X, X[idx]))
             bias_list.append(_append)
-        
+
         self.bias = np.mean(bias_list) if bias_list else 0
-    
+
     def _linear_kernel(self, xi: Matrix, xj: Matrix) -> Matrix:
         return xi.dot(xj.T)
 
     def _poly_kernel(self, xi: Matrix, xj: Matrix) -> Matrix:
         return (self.coef + xi.dot(xj.T)) ** self.deg
 
     def _rbf_kernel(self, xi: Matrix, xj: Matrix) -> Matrix:
         norm = np.linalg.norm(xi[:, np.newaxis] - xj[np.newaxis, :], axis=2)
-        return np.exp(-self.gamma * norm ** 2)
+        return np.exp(-self.gamma * norm**2)
 
     def _sigmoid_kernel(self, xi: Matrix, xj: Matrix) -> Matrix:
         return np.tanh(2 * xi.dot(xj.T) + self.coef)
 
     def _set_kernel_func(self) -> None:
-        if self.kernel in ('linear', 'lin'): 
+        if self.kernel in ("linear", "lin"):
             self._kernel_func = self._linear_kernel
-        elif self.kernel in ('poly', 'polynomial'): 
+        elif self.kernel in ("poly", "polynomial"):
             self._kernel_func = self._poly_kernel
-        elif self.kernel in ('rbf', 'gaussian', 'Gaussian'): 
+        elif self.kernel in ("rbf", "gaussian", "Gaussian"):
             self._kernel_func = self._rbf_kernel
-        elif self.kernel in ('sigmoid', 'tanh'): 
+        elif self.kernel in ("sigmoid", "tanh"):
             self._kernel_func = self._sigmoid_kernel
 
     def predict(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         scores = np.zeros((X.shape[0], len(self.models)))
 
         for i, (_, _X, _y, alpha, bias) in enumerate(self.models):
             pred = (alpha * _y).dot(self._kernel_func(_X, X)) + bias
             scores[:, i] = pred
 
         return np.argmax(scores, axis=1)
-    
-    def score(self, X: Matrix, y: Matrix, 
-              metric: Evaluator = Accuracy) -> float:
+
+    def score(self, X: Matrix, y: Matrix, metric: Evaluator = Accuracy) -> float:
         X_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=X_pred)
-
```

### Comparing `luma-ml-0.6.4/luma/classifier/tree.py` & `luma-ml-0.6.5/luma/classifier/tree.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,236 +4,256 @@
 from luma.interface.util import Matrix, Vector
 from luma.interface.exception import NotFittedError, UnsupportedParameterError
 from luma.core.super import Estimator, Evaluator, Supervised
 from luma.interface.util import DecisionTreeNode
 from luma.metric.classification import Accuracy
 
 
-__all__ = (
-    'DecisionTreeClassifier'
-)
+__all__ = "DecisionTreeClassifier"
 
 
 class DecisionTreeClassifier(Estimator, Supervised):
-    
     """
-    A Decision Tree Classifier is a machine learning algorithm that 
-    classifies data by making decisions based on asking a series of 
-    questions. It splits the dataset into branches at each node, 
-    based on feature values, aiming to increase homogeneity in each 
-    branch. The process continues recursively until it reaches a 
-    leaf node, where the final decision or classification is made. 
-    This model is intuitive and can easily handle categorical and 
+    A Decision Tree Classifier is a machine learning algorithm that
+    classifies data by making decisions based on asking a series of
+    questions. It splits the dataset into branches at each node,
+    based on feature values, aiming to increase homogeneity in each
+    branch. The process continues recursively until it reaches a
+    leaf node, where the final decision or classification is made.
+    This model is intuitive and can easily handle categorical and
     numerical data.
-    
+
     Parameters
     ----------
     `max_depth` : Maximum depth of the tree
     `criterion` : Function used to measure the quality of a split
     `min_samples_split` : Minimum samples required to split a node
     `min_samples_leaf` : Minimum samples required to be at a leaf node
     `max_features` : Number of features to consider
     `min_impurity_decrease` : Minimum decrement of impurity for a split
     `max_leaf_nodes` : Maximum amount of leaf nodes
     `random_state` : The randomness seed of the estimator
-    
+
     """
-    
-    def __init__(self, 
-                 max_depth: int = 10, 
-                 criterion: Literal['gini', 'entropy'] = 'gini', 
-                 min_samples_split: int = 2,
-                 min_samples_leaf: int = 1, 
-                 max_features: int = None, 
-                 min_impurity_decrease: float = 0.0,
-                 max_leaf_nodes: int = None, 
-                 random_state: int = None) -> None:
+
+    def __init__(
+        self,
+        max_depth: int = 10,
+        criterion: Literal["gini", "entropy"] = "gini",
+        min_samples_split: int = 2,
+        min_samples_leaf: int = 1,
+        max_features: int = None,
+        min_impurity_decrease: float = 0.0,
+        max_leaf_nodes: int = None,
+        random_state: int = None,
+    ) -> None:
         self.max_depth = max_depth
         self.criterion = criterion
         self.min_samples_split = min_samples_split
         self.min_samples_leaf = min_samples_leaf
         self.max_features = max_features
         self.min_impurity_decrease = min_impurity_decrease
         self.max_leaf_nodes = max_leaf_nodes
         self.random_state = random_state
         self.root = None
         self.classes_ = None
         self._fitted = False
-        
+
+        self.set_param_ranges(
+            {
+                "max_depth": ("0<,+inf", int),
+                "min_samples_split": ("0,+inf", int),
+                "min_samples_leaf": ("0,+inf", int),
+                "min_impurity_decrease": ("0,+inf", None),
+                "max_leaf_nodes": ("0<,+inf", int),
+            }
+        )
+        self.check_param_ranges()
         np.random.seed(random_state)
-    
-    def fit(self, 
-            X: Matrix, 
-            y: Vector,
-            sample_weights: Vector = None) -> 'DecisionTreeClassifier':
-        if sample_weights is None: sample_weights = np.ones(len(y))
+
+    def fit(
+        self, X: Matrix, y: Vector, sample_weights: Vector = None
+    ) -> "DecisionTreeClassifier":
+        if sample_weights is None:
+            sample_weights = np.ones(len(y))
         sample_weights = Vector(sample_weights)
-        
+
         self.classes_ = np.unique(y)
         self.root = self._build_tree(X, y, 0, sample_weights)
         self._fitted = True
         return self
 
     def _stopping_criteria(self, y: Vector, depth: int) -> bool:
-        if len(np.unique(y)) == 1: return True
-        if depth == self.max_depth: return True
-        if len(y) < self.min_samples_split: return True
+        if len(np.unique(y)) == 1:
+            return True
+        if depth == self.max_depth:
+            return True
+        if len(y) < self.min_samples_split:
+            return True
         return False
-    
-    def _build_tree(self, 
-                    X: Matrix, 
-                    y: Vector, 
-                    depth: int, 
-                    sample_weights: Vector) -> DecisionTreeNode:
+
+    def _build_tree(
+        self, X: Matrix, y: Vector, depth: int, sample_weights: Vector
+    ) -> DecisionTreeNode:
         if self._stopping_criteria(y, depth):
             leaf_value = self._calculate_leaf_value(y, sample_weights)
             return DecisionTreeNode(value=leaf_value)
-        
+
         feature_index, threshold = self._best_split(X, y, sample_weights)
         if feature_index is None:
             leaf_value = self._calculate_leaf_value(y, sample_weights)
             return DecisionTreeNode(value=leaf_value)
 
         left_indices = X[:, feature_index] <= threshold
         right_indices = X[:, feature_index] > threshold
-        
+
         X_left, X_right = X[left_indices], X[right_indices]
         y_left, y_right = y[left_indices], y[right_indices]
-        
+
         weights_left = sample_weights[left_indices]
         weights_right = sample_weights[right_indices]
-        
+
         left_subtree = self._build_tree(X_left, y_left, depth + 1, weights_left)
         right_subtree = self._build_tree(X_right, y_right, depth + 1, weights_right)
 
-        return DecisionTreeNode(feature_index=feature_index, 
-                                threshold=threshold, 
-                                left=left_subtree, 
-                                right=right_subtree)
+        return DecisionTreeNode(
+            feature_index=feature_index,
+            threshold=threshold,
+            left=left_subtree,
+            right=right_subtree,
+        )
 
     def _calculate_leaf_value(self, y: Vector, sample_weights: Vector) -> dict:
         classes, counts = np.unique(y, return_counts=True)
         weighted_counts = np.zeros_like(counts, dtype=np.float64)
-        
+
         for i, cl in enumerate(classes):
             weighted_counts[i] = sample_weights[y == cl].sum()
-        
+
         return dict(zip(classes, weighted_counts))
 
-    def _best_split(self, 
-                    X: Matrix, 
-                    y: Vector, 
-                    sample_weights: Vector) -> Tuple[int, float]:
+    def _best_split(
+        self, X: Matrix, y: Vector, sample_weights: Vector
+    ) -> Tuple[int, float]:
         best_gain = 0
         best_feature, best_threshold = None, None
         current_impurity = self._calculate_impurity(y, sample_weights)
 
         for feature_index in range(X.shape[1]):
             thresholds = np.unique(X[:, feature_index])
             for threshold in thresholds:
                 left_indices = X[:, feature_index] <= threshold
                 right_indices = X[:, feature_index] > threshold
-                
-                if np.sum(left_indices) < self.min_samples_split or \
-                    np.sum(right_indices) < self.min_samples_split:
+
+                if (
+                    np.sum(left_indices) < self.min_samples_split
+                    or np.sum(right_indices) < self.min_samples_split
+                ):
                     continue
-                
+
                 gain = self._calculate_gain(
                     y, sample_weights, left_indices, right_indices, current_impurity
                 )
                 if gain > best_gain:
                     best_gain = gain
                     best_feature = feature_index
                     best_threshold = threshold
 
         return best_feature, best_threshold
 
     def _calculate_impurity(self, y: Vector, sample_weights: Vector) -> float:
-        if self.criterion == 'gini':
+        if self.criterion == "gini":
             return self._calculate_gini(y, sample_weights)
-        elif self.criterion == 'entropy':
+        elif self.criterion == "entropy":
             return self._calculate_entropy(y, sample_weights)
         else:
             raise UnsupportedParameterError(self.criterion)
 
     def _calculate_gini(self, y: Vector, sample_weights: Vector) -> float:
         total_weight = np.sum(sample_weights)
         _, counts = np.unique(y, return_counts=True)
         weighted_counts = np.zeros_like(counts, dtype=np.float64)
-        
+
         for i, cl in enumerate(np.unique(y)):
             weighted_counts[i] = np.sum(sample_weights[y == cl])
-        
+
         prob = weighted_counts / total_weight
-        gini = 1 - np.sum(prob ** 2)
-        
+        gini = 1 - np.sum(prob**2)
+
         return gini
 
     def _calculate_entropy(self, y: Vector, sample_weights: Vector) -> float:
         total_weight = np.sum(sample_weights)
         _, counts = np.unique(y, return_counts=True)
         weighted_counts = np.zeros_like(counts, dtype=np.float64)
-        
+
         for i, cl in enumerate(np.unique(y)):
             weighted_counts[i] = np.sum(sample_weights[y == cl])
-        
+
         prob = weighted_counts / total_weight
         entropy = -np.sum(prob * np.log2(prob + np.finfo(float).eps))
-        
+
         return entropy
 
-    def _calculate_gain(self, 
-                        y: Vector, 
-                        sample_weights: Vector, 
-                        left_indices: Vector, 
-                        right_indices: Vector, 
-                        current_impurity: float) -> float:
+    def _calculate_gain(
+        self,
+        y: Vector,
+        sample_weights: Vector,
+        left_indices: Vector,
+        right_indices: Vector,
+        current_impurity: float,
+    ) -> float:
         left_weight = np.sum(sample_weights[left_indices])
         right_weight = np.sum(sample_weights[right_indices])
         total_weight = left_weight + right_weight
-        
+
         weights_left = sample_weights[left_indices]
         weights_right = sample_weights[right_indices]
 
         left_impurity = self._calculate_impurity(y[left_indices], weights_left)
         right_impurity = self._calculate_impurity(y[right_indices], weights_right)
 
         weighted_impurity = (left_weight / total_weight) * left_impurity
         weighted_impurity += (right_weight / total_weight) * right_impurity
         gain = current_impurity - weighted_impurity
-        
+
         return gain
 
     def predict(self, X: Matrix) -> Vector:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         preds = [self._predict_single(self.root, x) for x in X]
-        
+
         return Vector(preds)
 
     def _predict_single(self, node: DecisionTreeNode, x: Vector) -> int:
         while node.value is None:
-            if x[node.feature_index] <= node.threshold: node = node.left
-            else: node = node.right
-        
+            if x[node.feature_index] <= node.threshold:
+                node = node.left
+            else:
+                node = node.right
+
         return max(node.value, key=node.value.get)
-    
+
     def predict_proba(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         proba_preds = [self._predict_proba_single(self.root, x) for x in X]
-        
+
         return Matrix(proba_preds)
 
     def _predict_proba_single(self, node: DecisionTreeNode, x: Vector) -> Vector:
         while node.value is None:
-            if x[node.feature_index] <= node.threshold: node = node.left
-            else: node = node.right
-        
+            if x[node.feature_index] <= node.threshold:
+                node = node.left
+            else:
+                node = node.right
+
         total_samples = sum(node.value.values())
         cl_probs = {cl: count / total_samples for cl, count in node.value.items()}
-        
+
         probabilities = Matrix([cl_probs.get(cl, 0.0) for cl in self.classes_])
         return probabilities
 
     def score(self, X: Matrix, y: Vector, metric: Evaluator = Accuracy) -> float:
         preds = self.predict(X)
         return metric.score(y_true=y, y_pred=preds)
-
```

### Comparing `luma-ml-0.6.4/luma/clustering/affinity.py` & `luma-ml-0.6.5/luma/clustering/affinity.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,456 +4,498 @@
 from luma.interface.util import Matrix, Vector, Scalar, KernelUtil
 from luma.core.super import Estimator, Evaluator, Unsupervised
 from luma.interface.exception import NotFittedError, UnsupportedParameterError
 from luma.metric.clustering import SilhouetteCoefficient
 
 
 __all__ = (
-    'AffinityPropagation',
-    'AdaptiveAffinityPropagation',
-    'KernelAffinityPropagation'
+    "AffinityPropagation",
+    "AdaptiveAffinityPropagation",
+    "KernelAffinityPropagation",
 )
 
 
 class AffinityPropagation(Estimator, Unsupervised):
-    
     """
-    Affinity Propagation is a clustering algorithm that identifies exemplars 
-    among data points, effectively determining cluster centers. It works by 
-    exchanging messages between pairs of data points until a set of exemplars 
-    and corresponding clusters emerges. The algorithm doesn't require the 
-    number of clusters to be specified in advance. Affinity Propagation is 
-    particularly useful for problems where the optimal number of clusters 
+    Affinity Propagation is a clustering algorithm that identifies exemplars
+    among data points, effectively determining cluster centers. It works by
+    exchanging messages between pairs of data points until a set of exemplars
+    and corresponding clusters emerges. The algorithm doesn't require the
+    number of clusters to be specified in advance. Affinity Propagation is
+    particularly useful for problems where the optimal number of clusters
     is unknown or hard to estimate.
-    
+
     Parameters
     ----------
     `max_iter` : Maximum iterations for message exchange
     `damping` : Balancing factor for ensuring numerical stability and convergence
     `tol` : Early-stopping threshold
     `preference` : Parameter which determines the selectivity of choosing exemplars
-    
+
     * Self-Similarity Setting:
-        The preference value represents the "self-similarity" of each data point. 
-        It is the value on the diagonal of the similarity matrix, which influences 
+        The preference value represents the "self-similarity" of each data point.
+        It is the value on the diagonal of the similarity matrix, which influences
         how likely a data point is to be chosen as an exemplar (a cluster center).
-    
+
     * Influencing Cluster Count:
-        A higher preference value suggests a greater likelihood for a data point to 
-        become an exemplar, potentially leading to more clusters. Conversely, a lower 
-        preference value tends to produce fewer clusters, as fewer points are strong 
+        A higher preference value suggests a greater likelihood for a data point to
+        become an exemplar, potentially leading to more clusters. Conversely, a lower
+        preference value tends to produce fewer clusters, as fewer points are strong
         candidates for being exemplars.
-    
+
     * Default Setting:
-        If not explicitly set, the preference is often chosen automatically based on 
-        the input data. Common practices include setting it to the median or mean of 
+        If not explicitly set, the preference is often chosen automatically based on
+        the input data. Common practices include setting it to the median or mean of
         the similarity values.
-    
+
     """
-    
-    def __init__(self, 
-                 max_iter: int = 100,
-                 damping: float = 0.7,
-                 preference: Scalar | Vector | Literal['median', 'min'] = 'median',
-                 tol: float = None,
-                 verbose: bool = False) -> None:
+
+    def __init__(
+        self,
+        max_iter: int = 100,
+        damping: float = 0.7,
+        preference: Scalar | Vector | Literal["median", "min"] = "median",
+        tol: float = None,
+        verbose: bool = False,
+    ) -> None:
         self.max_iter = max_iter
         self.damping = damping
         self.preference = preference
         self.tol = tol
         self.verbose = verbose
         self._X = None
         self._fitted = False
-    
-    def fit(self, X: Matrix) -> 'AffinityPropagation':
+
+        self.set_param_ranges({"max_iter": ("0<,+inf", int), "damping": ("0,1", None)})
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix) -> "AffinityPropagation":
         self._X = X
         m, _ = X.shape
-        
+
         S = self._compute_similarity(X)
         S = self._assign_preference(S)
         S += 1e-12 * np.random.normal(size=(m, m)) * (np.max(S) - np.min(S))
-        
+
         R = np.zeros_like(S)
         A = np.zeros_like(S)
-        
+
         for iter in range(self.max_iter):
-            E_old = R + A         
+            E_old = R + A
             R = self._compute_responsibility(S, R, A)
-            A = self._compute_availability(R, A)         
+            A = self._compute_availability(R, A)
             E_new = R + A
 
             if self.tol is not None and np.allclose(E_old, E_new, atol=self.tol):
-                if not self.verbose: break
+                if not self.verbose:
+                    break
                 print(f"[AP] Early convergence at iteration {iter}/{self.max_iter}")
                 break
-            
+
             if self.verbose and iter % 10 == 0 and iter:
-                print(f"[AP] Finished iteration {iter}/{self.max_iter}",
-                      f"with delta-E: {np.linalg.norm(E_new - E_old)}")
-        
+                print(
+                    f"[AP] Finished iteration {iter}/{self.max_iter}",
+                    f"with delta-E: {np.linalg.norm(E_new - E_old)}",
+                )
+
         E = R + A
         self._clusters = np.argmax(E, axis=1)
         self.exemplars = np.unique(self._clusters)
         self.centers = X[self.exemplars]
-        
+
         replace = dict(zip(self.exemplars, range(len(self.exemplars))))
         new_ = np.arange(0, max(self._clusters) + 1)
         new_[list(replace.keys())] = list(replace.values())
-        
+
         self._clusters = new_[self._clusters]
         self._fitted = True
         return self
-    
+
     def _compute_similarity(self, X: Matrix) -> Matrix:
-        first_ = np.sum(X ** 2, axis=-1).reshape(-1, 1)
-        second_ = np.sum(X ** 2, axis=-1)
+        first_ = np.sum(X**2, axis=-1).reshape(-1, 1)
+        second_ = np.sum(X**2, axis=-1)
         third_ = -2 * np.dot(X, X.T)
-        
+
         return -1 * (first_ + second_ + third_)
 
     def _assign_preference(self, S: Matrix) -> Matrix:
         indices = np.where(~np.eye(S.shape[0], dtype=bool))
-        
-        if self.preference == 'median': pref = np.median(S[indices])
-        elif self.preference == 'min': pref = np.min(S[indices])
-        
-        elif isinstance(self.preference, (np.ndarray, float, int)): 
+
+        if self.preference == "median":
+            pref = np.median(S[indices])
+        elif self.preference == "min":
+            pref = np.min(S[indices])
+
+        elif isinstance(self.preference, (np.ndarray, float, int)):
             pref = self.preference
         else:
             raise UnsupportedParameterError(self.preference)
 
         np.fill_diagonal(S, pref)
         return S
-    
+
     def _compute_responsibility(self, S: Matrix, R: Matrix, A: Matrix) -> Matrix:
         max_ = A + S
         np.fill_diagonal(max_, -np.inf)
-        
+
         row_indices = np.arange(max_.shape[0])
         max_indices = np.argmax(max_, axis=1)
-        
+
         row_max = max_[row_indices, max_indices]
         max_[row_indices, max_indices] = -np.inf
-        
+
         row_max_ = max_[row_indices, np.argmax(max_, axis=1)]
         max_AS = np.zeros_like(S) + row_max.reshape(-1, 1)
         max_AS[row_indices, max_indices] = row_max_
-        
+
         return (1 - self.damping) * (S - max_AS) + self.damping * R
-    
+
     def _compute_availability(self, R: Matrix, A: Matrix) -> Matrix:
         R = R.copy()
         diag = np.diag(R).copy()
-        
+
         np.fill_diagonal(R, 0)
         R = np.where(R < 0, 0, R)
-        
+
         sum_vectors = np.sum(R, axis=0)
         A_new = np.minimum(0, diag + sum_vectors - R)
         np.fill_diagonal(A_new, np.sum(R, axis=0))
-        
+
         return (1 - self.damping) * A_new + self.damping * A
 
     @property
     def labels(self) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         return self._clusters
-    
+
     def predict(self) -> None:
         raise Warning(f"{type(self).__name__} does not support prediction!")
-    
+
     def score(self, metric: Evaluator = SilhouetteCoefficient) -> float:
         return metric.score(self._X, self.labels)
 
 
 class AdaptiveAffinityPropagation(Estimator, Unsupervised):
-    
     """
-    Adaptive Affinity Propagation (AAP) is a clustering algorithm that 
-    dynamically adjusts the preference parameter during the clustering 
-    process. It iteratively refines cluster exemplars based on the exchange 
-    of responsibility and availability messages between data points. The 
-    adaptation of preferences allows AAP to be more flexible in identifying 
-    an appropriate number of clusters, especially in complex or ambiguous 
-    datasets. This approach enhances the standard Affinity Propagation 
-    algorithm by offering potentially improved clustering accuracy 
+    Adaptive Affinity Propagation (AAP) is a clustering algorithm that
+    dynamically adjusts the preference parameter during the clustering
+    process. It iteratively refines cluster exemplars based on the exchange
+    of responsibility and availability messages between data points. The
+    adaptation of preferences allows AAP to be more flexible in identifying
+    an appropriate number of clusters, especially in complex or ambiguous
+    datasets. This approach enhances the standard Affinity Propagation
+    algorithm by offering potentially improved clustering accuracy
     and adaptability.
-    
+
     Parameters
     ----------
     `max_iter` : Maximum iterations for message exchange
     `damping` : Balancing factor for ensuring numerical stability and convergence
     `tol` : Early-stopping threshold
     `lambda_param` : Preference updating factor
     `preference` : Parameter which determines the selectivity of choosing exemplars
     (more details in `AffinityPropagation`)
-    
+
     """
-    
-    def __init__(self, 
-                 max_iter: int = 100,
-                 damping: float = 0.7,
-                 preference: Scalar | Vector | Literal['median', 'min'] = 'median',
-                 lambda_param: float = 0.5,
-                 tol: float = None,
-                 verbose: bool = False) -> None:
+
+    def __init__(
+        self,
+        max_iter: int = 100,
+        damping: float = 0.7,
+        preference: Scalar | Vector | Literal["median", "min"] = "median",
+        lambda_param: float = 0.5,
+        tol: float = None,
+        verbose: bool = False,
+    ) -> None:
         self.max_iter = max_iter
         self.damping = damping
         self.preference = preference
         self.tol = tol
         self.lambda_param = lambda_param
         self.verbose = verbose
         self._X = None
         self._fitted = False
-    
-    def fit(self, X: Matrix) -> 'AdaptiveAffinityPropagation':
+
+        self.set_param_ranges(
+            {
+                "max_iter": ("0<,+inf", int),
+                "damping": ("0,1", None),
+                "lambda_param": ("0,+inf", None),
+            }
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix) -> "AdaptiveAffinityPropagation":
         self._X = X
         m, _ = X.shape
-        
+
         S = self._compute_similarity(X)
         S = self._assign_preference(S)
         S += 1e-12 * np.random.normal(size=(m, m)) * (np.max(S) - np.min(S))
-        
+
         R = np.zeros_like(S)
         A = np.zeros_like(S)
 
         for iter in range(self.max_iter):
-            E_old = R + A         
+            E_old = R + A
             R = self._compute_responsibility(S, R, A)
-            A = self._compute_availability(R, A)         
+            A = self._compute_availability(R, A)
             E_new = R + A
 
             diag_R = np.diag(R)
             diag_A = np.diag(A)
             self._update_preferences(S, diag_R + diag_A)
 
             if self.tol is not None and np.allclose(E_old, E_new, atol=self.tol):
-                if not self.verbose: break
+                if not self.verbose:
+                    break
                 print(f"[AAP] Early convergence at iteration {iter}/{self.max_iter}")
                 break
-            
+
             if self.verbose and iter % 10 == 0 and iter:
-                print(f"[AAP] Finished iteration {iter}/{self.max_iter}",
-                      f"with delta-E: {np.linalg.norm(E_new - E_old)}")
-        
+                print(
+                    f"[AAP] Finished iteration {iter}/{self.max_iter}",
+                    f"with delta-E: {np.linalg.norm(E_new - E_old)}",
+                )
+
         E = R + A
         self._clusters = np.argmax(E, axis=1)
         self.exemplars = np.unique(self._clusters)
         self.centers = X[self.exemplars]
-        
+
         replace = dict(zip(self.exemplars, range(len(self.exemplars))))
         new_ = np.arange(0, max(self._clusters) + 1)
         new_[list(replace.keys())] = list(replace.values())
-        
+
         self._clusters = new_[self._clusters]
         self._fitted = True
         return self
 
     def _compute_similarity(self, X: Matrix) -> Matrix:
-        first_ = np.sum(X ** 2, axis=-1).reshape(-1, 1)
-        second_ = np.sum(X ** 2, axis=-1)
+        first_ = np.sum(X**2, axis=-1).reshape(-1, 1)
+        second_ = np.sum(X**2, axis=-1)
         third_ = -2 * np.dot(X, X.T)
-        
+
         return -1 * (first_ + second_ + third_)
 
     def _assign_preference(self, S: Matrix) -> Matrix:
         indices = np.where(~np.eye(S.shape[0], dtype=bool))
-        
-        if self.preference == 'median': pref = np.median(S[indices])
-        elif self.preference == 'min': pref = np.min(S[indices])
-        
-        elif isinstance(self.preference, (np.ndarray, float, int)): 
+
+        if self.preference == "median":
+            pref = np.median(S[indices])
+        elif self.preference == "min":
+            pref = np.min(S[indices])
+
+        elif isinstance(self.preference, (np.ndarray, float, int)):
             pref = self.preference
         else:
             raise UnsupportedParameterError(self.preference)
 
         np.fill_diagonal(S, pref)
         return S
-    
+
     def _compute_responsibility(self, S: Matrix, R: Matrix, A: Matrix) -> Matrix:
         max_ = A + S
         np.fill_diagonal(max_, -np.inf)
-        
+
         row_indices = np.arange(max_.shape[0])
         max_indices = np.argmax(max_, axis=1)
-        
+
         row_max = max_[row_indices, max_indices]
         max_[row_indices, max_indices] = -np.inf
-        
+
         row_max_ = max_[row_indices, np.argmax(max_, axis=1)]
         max_AS = np.zeros_like(S) + row_max.reshape(-1, 1)
         max_AS[row_indices, max_indices] = row_max_
-        
+
         return (1 - self.damping) * (S - max_AS) + self.damping * R
-    
+
     def _compute_availability(self, R: Matrix, A: Matrix) -> Matrix:
         R = R.copy()
         diag = np.diag(R).copy()
-        
+
         np.fill_diagonal(R, 0)
         R = np.where(R < 0, 0, R)
-        
+
         sum_vectors = np.sum(R, axis=0)
         A_new = np.minimum(0, diag + sum_vectors - R)
         np.fill_diagonal(A_new, np.sum(R, axis=0))
-        
+
         return (1 - self.damping) * A_new + self.damping * A
-    
+
     def _update_preferences(self, S: Matrix, delta: Vector) -> None:
-        if not isinstance(self.preference, (int, float)): return
+        if not isinstance(self.preference, (int, float)):
+            return
         self.preference += self.lambda_param * delta
         np.fill_diagonal(S, self.preference)
 
     @property
     def labels(self) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         return self._clusters
-    
+
     def predict(self) -> None:
         raise Warning(f"{type(self).__name__} does not support prediction!")
-    
+
     def score(self, metric: Evaluator = SilhouetteCoefficient) -> float:
         return metric.score(self._X, self.labels)
 
 
 class KernelAffinityPropagation(Estimator, Unsupervised):
-    
     """
-    Kernel-based Affinity Propagation (KAP) employs kernel functions 
-    to transform data into a higher-dimensional space, enabling effective 
-    clustering of complex, non-linear datasets. This approach enhances 
-    the standard Affinity Propagation by uncovering intricate cluster 
-    structures in transformed feature spaces, suitable for non-linearly 
+    Kernel-based Affinity Propagation (KAP) employs kernel functions
+    to transform data into a higher-dimensional space, enabling effective
+    clustering of complex, non-linear datasets. This approach enhances
+    the standard Affinity Propagation by uncovering intricate cluster
+    structures in transformed feature spaces, suitable for non-linearly
     separable data.
-    
+
     Parameters
     ----------
     `max_iter` : Maximum iterations for message exchange
     `damping` : Balancing factor for ensuring numerical stability and convergence
     `preference` : Parameter which determines the selectivity of choosing exemplars
     `tol` : Early-stopping threshold
     `kernel`: Kernel method (`rbf`, `sigmoid`, `laplacian` are supported)
     `gamma` : Scaling factor for kernel function
-    
+
     """
-    
-    def __init__(self, 
-                 max_iter: int = 100,
-                 damping: float = 0.7,
-                 preference: Scalar | Vector | Literal['median', 'min'] = 'median',
-                 tol: float = None,
-                 kernel: KernelUtil.func_type = 'rbf',
-                 gamma: float = 1.0,
-                 verbose: bool = False) -> None:
+
+    def __init__(
+        self,
+        max_iter: int = 100,
+        damping: float = 0.7,
+        preference: Scalar | Vector | Literal["median", "min"] = "median",
+        tol: float = None,
+        kernel: KernelUtil.FuncType = "rbf",
+        gamma: float = 1.0,
+        verbose: bool = False,
+    ) -> None:
         self.max_iter = max_iter
         self.damping = damping
         self.preference = preference
         self.tol = tol
         self.kernel = kernel
         self.gamma = gamma
         self.verbose = verbose
         self._X = None
         self._fitted = False
 
-    def fit(self, X: Matrix) -> 'KernelAffinityPropagation':
+        self.set_param_ranges(
+            {
+                "max_iter": ("0<,+inf", int),
+                "damping": ("0,1", None),
+                "gamma": ("0<,+inf", None),
+            }
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix) -> "KernelAffinityPropagation":
         self._X = X
         m, _ = X.shape
 
         kernel_func = KernelUtil(self.kernel, gamma=self.gamma).kernel_func
         X_trans = kernel_func(X)
-        
+
         S = self._compute_similarity(X_trans)
         S = self._assign_preference(S)
         S += 1e-12 * np.random.normal(size=(m, m)) * (np.max(S) - np.min(S))
-        
+
         R = np.zeros_like(S)
         A = np.zeros_like(S)
-        
+
         for iter in range(self.max_iter):
-            E_old = R + A         
+            E_old = R + A
             R = self._compute_responsibility(S, R, A)
-            A = self._compute_availability(R, A)         
+            A = self._compute_availability(R, A)
             E_new = R + A
 
             if self.tol is not None and np.allclose(E_old, E_new, atol=self.tol):
-                if not self.verbose: break
+                if not self.verbose:
+                    break
                 print(f"[KAP] Early convergence at iteration {iter}/{self.max_iter}")
                 break
-            
+
             if self.verbose and iter % 10 == 0 and iter:
-                print(f"[KAP] Finished iteration {iter}/{self.max_iter}",
-                      f"with delta-E: {np.linalg.norm(E_new - E_old)}")
-        
+                print(
+                    f"[KAP] Finished iteration {iter}/{self.max_iter}",
+                    f"with delta-E: {np.linalg.norm(E_new - E_old)}",
+                )
+
         E = R + A
         self._clusters = np.argmax(E, axis=1)
         self.exemplars = np.unique(self._clusters)
         self.centers = X[self.exemplars]
-        
+
         replace = dict(zip(self.exemplars, range(len(self.exemplars))))
         new_ = np.arange(0, max(self._clusters) + 1)
         new_[list(replace.keys())] = list(replace.values())
-        
+
         self._clusters = new_[self._clusters]
         self._fitted = True
         return self
-    
+
     def _compute_similarity(self, X: Matrix) -> Matrix:
-        first_ = np.sum(X ** 2, axis=-1).reshape(-1, 1)
-        second_ = np.sum(X ** 2, axis=-1)
+        first_ = np.sum(X**2, axis=-1).reshape(-1, 1)
+        second_ = np.sum(X**2, axis=-1)
         third_ = -2 * np.dot(X, X.T)
-        
+
         return -1 * (first_ + second_ + third_)
 
     def _assign_preference(self, S: Matrix) -> Matrix:
         indices = np.where(~np.eye(S.shape[0], dtype=bool))
-        
-        if self.preference == 'median': pref = np.median(S[indices])
-        elif self.preference == 'min': pref = np.min(S[indices])
-        
-        elif isinstance(self.preference, (np.ndarray, float, int)): 
+
+        if self.preference == "median":
+            pref = np.median(S[indices])
+        elif self.preference == "min":
+            pref = np.min(S[indices])
+
+        elif isinstance(self.preference, (np.ndarray, float, int)):
             pref = self.preference
         else:
             raise UnsupportedParameterError(self.preference)
 
         np.fill_diagonal(S, pref)
         return S
-    
+
     def _compute_responsibility(self, S: Matrix, R: Matrix, A: Matrix) -> Matrix:
         max_ = A + S
         np.fill_diagonal(max_, -np.inf)
-        
+
         row_indices = np.arange(max_.shape[0])
         max_indices = np.argmax(max_, axis=1)
-        
+
         row_max = max_[row_indices, max_indices]
         max_[row_indices, max_indices] = -np.inf
-        
+
         row_max_ = max_[row_indices, np.argmax(max_, axis=1)]
         max_AS = np.zeros_like(S) + row_max.reshape(-1, 1)
         max_AS[row_indices, max_indices] = row_max_
-        
+
         return (1 - self.damping) * (S - max_AS) + self.damping * R
-    
+
     def _compute_availability(self, R: Matrix, A: Matrix) -> Matrix:
         R = R.copy()
         diag = np.diag(R).copy()
-        
+
         np.fill_diagonal(R, 0)
         R = np.where(R < 0, 0, R)
-        
+
         sum_vectors = np.sum(R, axis=0)
         A_new = np.minimum(0, diag + sum_vectors - R)
         np.fill_diagonal(A_new, np.sum(R, axis=0))
-        
+
         return (1 - self.damping) * A_new + self.damping * A
 
     @property
     def labels(self) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         return self._clusters
-    
+
     def predict(self) -> None:
         raise Warning(f"{type(self).__name__} does not support prediction!")
-    
+
     def score(self, metric: Evaluator = SilhouetteCoefficient) -> float:
         return metric.score(self._X, self.labels)
-
```

### Comparing `luma-ml-0.6.4/luma/clustering/density.py` & `luma-ml-0.6.5/luma/clustering/density.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,479 +8,517 @@
 from luma.interface.exception import NotFittedError, NotConvergedError
 from luma.interface.exception import UnsupportedParameterError
 
 from luma.metric.distance import Euclidean, Minkowski
 from luma.metric.clustering import SilhouetteCoefficient
 
 
-__all__ = (
-    'DBSCAN',
-    'OPTICS',
-    'DENCLUE',
-    'MeanShiftClustering'
-)
+__all__ = ("DBSCAN", "OPTICS", "DENCLUE", "MeanShiftClustering")
 
 
 class DBSCAN(Estimator, Unsupervised):
-    
     """
-    DBSCAN, short for Density-Based Spatial Clustering of Applications 
-    with Noise, is a clustering algorithm that groups points in a dataset 
-    by their proximity and density. It identifies clusters as areas of high 
-    point density, separated by regions of low density. Points in sparse 
-    regions are classified as noise. DBSCAN is particularly effective at 
+    DBSCAN, short for Density-Based Spatial Clustering of Applications
+    with Noise, is a clustering algorithm that groups points in a dataset
+    by their proximity and density. It identifies clusters as areas of high
+    point density, separated by regions of low density. Points in sparse
+    regions are classified as noise. DBSCAN is particularly effective at
     discovering clusters of arbitrary shapes and dealing with outliers.
-    
+
     Parameters
     ----------
     `epsilon` : Radius of a neighborhood hypersphere
     `min_points` : Minimum required points to form a cluster
-    
+
     """
-    
-    def __init__(self, 
-                 epsilon: float = 0.1, 
-                 min_points: int = 5,
-                 metric: Literal['euclidean', 'minkowski'] = 'euclidean') -> None:
+
+    def __init__(
+        self,
+        epsilon: float = 0.1,
+        min_points: int = 5,
+        metric: Literal["euclidean", "minkowski"] = "euclidean",
+    ) -> None:
         self.epsilon = epsilon
         self.min_points = min_points
         self.metric = metric
         self._X = None
         self._fitted = False
-        
+
         self.metric_func = None
-        if self.metric == 'euclidean': self.metric_func = Euclidean
-        elif self.metric == 'minkowski': self.metric_func = Minkowski
-        else: raise UnsupportedParameterError(self.metric)
-        
-    def fit(self, X: Matrix) -> 'DBSCAN':
+        if self.metric == "euclidean":
+            self.metric_func = Euclidean
+        elif self.metric == "minkowski":
+            self.metric_func = Minkowski
+        else:
+            raise UnsupportedParameterError(self.metric)
+
+        self.set_param_ranges(
+            {"epsilon": ("0<,+inf", None), "min_points": ("0<,+inf", int)}
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix) -> "DBSCAN":
         self._X = X
         clusters = [0] * X.shape[0]
         curPt = 0
-        
+
         for i in range(X.shape[0]):
-            if clusters[i]: continue
+            if clusters[i]:
+                continue
             neighbors = self._generate_neighbors(X, idx=i)
             if len(neighbors) < self.min_points:
                 clusters[i] = -1
             else:
                 curPt += 1
                 self._expand_cluster(X, neighbors, clusters, i, curPt)
-        
+
         self._cluster_labels = clusters
         self._fitted = True
         return self
-    
+
     def _generate_neighbors(self, X: Matrix, idx: int) -> Matrix:
         neighbors = []
         for i in range(X.shape[0]):
             if self.metric_func.compute(X[idx], X[i]) < self.epsilon:
                 neighbors.append(i)
 
         return Matrix(neighbors)
 
-    def _expand_cluster(self, X: Matrix, neighbors: Matrix, clusters: Matrix, 
-                        idx: int, current: int) -> None:
+    def _expand_cluster(
+        self, X: Matrix, neighbors: Matrix, clusters: Matrix, idx: int, current: int
+    ) -> None:
         i = 0
         clusters[idx] = current
-        
+
         while i < len(neighbors):
             next = neighbors[i]
             if clusters[next] == -1:
                 clusters[next] = current
-                
+
             elif clusters[next] == 0:
                 clusters[next] = current
                 next_neighbors = self._generate_neighbors(X, idx=next)
-                
+
                 if len(next_neighbors) > self.min_points:
                     neighbors = np.concatenate([neighbors, next_neighbors], axis=0)
-            
+
             i += 1
-    
+
     @property
     def labels(self) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         return Matrix(self._cluster_labels)
-    
+
     def predict(self) -> None:
         raise Warning(f"{type(self).__name__} does not support prediction!")
-    
+
     def score(self, metric: Evaluator = SilhouetteCoefficient) -> float:
         return metric.score(self._X, self.labels)
 
 
 class OPTICS(Estimator, Unsupervised):
-    
     """
-    OPTICS (Ordering Points To Identify the Clustering Structure) is an 
-    unsupervised learning algorithm for identifying cluster structures 
-    in spatial  It creates an ordered list of points based on 
-    core-distance and reachability-distance, allowing it to find 
-    clusters of varying density. Unlike algorithms like DBSCAN, it 
-    doesn't require a global density threshold, making it versatile 
-    for complex datasets. The result is often visualized as a 
-    reachability plot, revealing the data's clustering hierarchy and 
+    OPTICS (Ordering Points To Identify the Clustering Structure) is an
+    unsupervised learning algorithm for identifying cluster structures
+    in spatial  It creates an ordered list of points based on
+    core-distance and reachability-distance, allowing it to find
+    clusters of varying density. Unlike algorithms like DBSCAN, it
+    doesn't require a global density threshold, making it versatile
+    for complex datasets. The result is often visualized as a
+    reachability plot, revealing the data's clustering hierarchy and
     density variations.
-    
+
     Parameters
     ----------
     `epsilon` : Radius of neighborhood hypersphere
     `min_points` : Minimum nuber of points to form a cluster
     `threshold` : Threshold for filtering samples with large reachabilities
-    
+
     """
-    
-    def __init__(self, 
-                 epsilon: float = 1.0,
-                 min_points: int = 5,
-                 threshold: float = 1.5,
-                 verbose: bool = False) -> None:
+
+    def __init__(
+        self,
+        epsilon: float = 1.0,
+        min_points: int = 5,
+        threshold: float = 1.5,
+        verbose: bool = False,
+    ) -> None:
         self.epsilon = epsilon
         self.min_points = min_points
         self.threshold = threshold
         self.verbose = verbose
         self._X = None
         self._fitted = False
-    
-    def fit(self, X: Matrix) -> 'OPTICS':
+
+        self.set_param_ranges(
+            {
+                "epsilon": ("0<,+inf", None),
+                "min_points": ("0<,+inf", int),
+                "threshold": ("0,+inf", None),
+            }
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix) -> "OPTICS":
         self._X = X
         m, _ = X.shape
-        
+
         self.processed = np.full(m, False, dtype=bool)
         self.reachability = np.full(m, np.inf)
         self.ordered_points = []
-        
+
         for i in range(m):
             if self.verbose and i % 50 == 0 and i:
-                print(f"[OPTICS] Finished for point {i}/{m}",
-                      f"with reachability {self.reachability[i]}")
-            
-            if self.processed[i]: continue
+                print(
+                    f"[OPTICS] Finished for point {i}/{m}",
+                    f"with reachability {self.reachability[i]}",
+                )
+
+            if self.processed[i]:
+                continue
             seeds = []
             point_neighbors = self._neighbors(X, i)
             core_dist = self._core_distance(point_neighbors)
-            
+
             self.processed[i] = True
             self.ordered_points.append(i)
-            
+
             if not np.isinf(core_dist):
                 self._update(X, core_dist, i, seeds)
                 seeds.sort(key=lambda x: x[1])
-                
+
                 while seeds:
                     next_, _ = seeds.pop(0)
                     self.processed[next_] = True
                     self.ordered_points.append(next_)
                     next_neighbors = self._neighbors(X, next_)
                     core_dist = self._core_distance(next_neighbors)
-                    
+
                     if not np.isinf(core_dist):
                         self._update(X, core_dist, next_, seeds)
-        
+
         self._fitted = True
         return self
-    
+
     def _core_distance(self, neighbors: Matrix) -> Matrix | Scalar:
         if len(neighbors) >= self.min_points:
             return sorted(neighbors)[self.min_points - 1]
         return np.inf
-    
+
     def _neighbors(self, X: Matrix, idx: int) -> Matrix:
         distances = cdist([X[idx]], X)[0]
         return distances[distances <= self.epsilon]
-    
-    def _update(self, X: Matrix, core_dist: Scalar, 
-                idx: int, seeds: list) -> None:
+
+    def _update(self, X: Matrix, core_dist: Scalar, idx: int, seeds: list) -> None:
         distances = cdist([X[idx]], X)[0]
         for i, dist in enumerate(distances):
             if dist <= self.epsilon and not self.processed[i]:
                 new_reach_dist = max(core_dist, dist)
-                
+
                 if np.isinf(self.reachability[i]):
                     self.reachability[i] = new_reach_dist
                     seeds.append((i, new_reach_dist))
                 elif new_reach_dist < self.reachability[i]:
                     self.reachability[i] = new_reach_dist
-    
-    def plot_reachability(self, 
-                          ax: Optional[plt.Axes] = None, 
-                          color: str = 'royalblue',
-                          show: bool = False) -> plt.Axes:
+
+    def plot_reachability(
+        self,
+        ax: Optional[plt.Axes] = None,
+        color: str = "royalblue",
+        show: bool = False,
+    ) -> plt.Axes:
         m = range(len(self.ordered_points))
         vals = self.reachability[self.ordered_points]
-        
-        if ax is None: 
+
+        if ax is None:
             _, ax = plt.subplots()
             show = True
-        
+
         ax.plot(m, vals, color=color)
         ax.fill_between(m, vals, color=color, alpha=0.5)
-        
-        ax.set_title('Reachability Plot')
+
+        ax.set_title("Reachability Plot")
         ax.set_xlim(m[0], m[-1])
-        
-        ax.set_xlabel('Order of Points')
-        ax.set_ylabel('Reachability Distance')
+
+        ax.set_xlabel("Order of Points")
+        ax.set_ylabel("Reachability Distance")
         ax.figure.tight_layout()
-        
-        if show: plt.show()
+
+        if show:
+            plt.show()
         return ax
-    
+
     @property
     def labels(self) -> Vector:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         cluster_labels = np.full_like(self.reachability, -1, dtype=int)
         current_ = 0
-        
+
         for point in self.ordered_points:
             if self.reachability[point] <= self.threshold:
                 cluster_labels[point] = current_
-            else: current_ += 1
-        
+            else:
+                current_ += 1
+
         unique_labels = np.unique(cluster_labels[cluster_labels != -1])
         mapping = {original: new for new, original in enumerate(unique_labels)}
         labels = [mapping[label] if label != -1 else -1 for label in cluster_labels]
-        
+
         return Vector(labels)
-    
+
     def predict(self) -> None:
         raise Warning(f"{type(self).__name__} does not support prediction!")
-    
+
     def score(self, metric: Evaluator = SilhouetteCoefficient) -> float:
         return metric.score(self._X, self.labels)
 
 
 class DENCLUE(Estimator, Unsupervised):
-    
     """
-    DENCLUE (Density-Based Clustering) is a machine learning algorithm 
-    for identifying clusters in large datasets. It uses mathematical 
-    functions, typically Gaussian kernels, to estimate data density. 
-    Cluster centers are determined by the peaks of these density functions. 
-    The algorithm excels in handling clusters of arbitrary shapes and noise, 
+    DENCLUE (Density-Based Clustering) is a machine learning algorithm
+    for identifying clusters in large datasets. It uses mathematical
+    functions, typically Gaussian kernels, to estimate data density.
+    Cluster centers are determined by the peaks of these density functions.
+    The algorithm excels in handling clusters of arbitrary shapes and noise,
     but is sensitive to parameter settings.
-    
+
     Parameters
     ----------
     `h` : Smoothing parameter of local density estimation
     `tol` : Threshold for early convergence
     `max_climb` : Maximum number of climbing process for finding local maxima
     `min_density` : Minimum local densities to be considered
     `sample_weight` : Custom individual weights for sample data
-    
+
     Reference
     ---------
-    Hinneburg, A., & Gabriel, H. H. (2007, September). Denclue 2.0: Fast 
-    clustering based on kernel density estimation. In International symposium 
-    on intelligent data analysis (pp. 70-80). Berlin, Heidelberg: Springer 
+    Hinneburg, A., & Gabriel, H. H. (2007, September). Denclue 2.0: Fast
+    clustering based on kernel density estimation. In International symposium
+    on intelligent data analysis (pp. 70-80). Berlin, Heidelberg: Springer
     Berlin Heidelberg.
-    
+
     """
-    
-    def __init__(self, 
-                 h: float | Literal['auto'] = 'auto', 
-                 tol: float = 1e-3, 
-                 max_climb: int = 100,
-                 min_density: float = 0.0, 
-                 sample_weight: Vector = None) -> None:
+
+    def __init__(
+        self,
+        h: float | Literal["auto"] = "auto",
+        tol: float = 1e-3,
+        max_climb: int = 100,
+        min_density: float = 0.0,
+        sample_weight: Vector = None,
+    ) -> None:
         self.h = h
         self.tol = tol
         self.max_climb = max_climb
         self.min_density = min_density
         self.sample_weight = sample_weight
         self._X = None
         self._fitted = False
 
-    def fit(self, X: Matrix) -> 'DENCLUE':
+        self.set_param_ranges(
+            {"max_climb": ("0<,+inf", int), "min_density": ("0,+inf", None)}
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix) -> "DENCLUE":
         self._m, self._n = X.shape
-        
+
         attractors: Vector = np.zeros((self._m, self._n))
         rad: Vector = np.zeros((self._m, 1))
         density: Vector = np.zeros((self._m, 1))
-        
-        if self.h == 'auto': self.h = np.std(X) / 5
+
+        if self.h == "auto":
+            self.h = np.std(X) / 5
         if self.sample_weight is None:
             self.sample_weight = np.ones((self._m, 1))
-        
+
         labels = -np.ones(X.shape[0])
         for i in range(self._m):
             attractors[i], density[i], rad[i] = self._climb_hill(X[i], X)
-        
+
         adj_list = [[] for _ in range(self._m)]
         for i in range(self._m):
             for j in range(i + 1, self._m):
                 diff = np.linalg.norm(attractors[i] - attractors[j])
                 if diff <= rad[i] + rad[j]:
                     adj_list[i].append(j)
                     adj_list[j].append(i)
-        
+
         num_clusters = 0
         for cl in self._find_connected_components(adj_list):
             max_instance = max(cl, key=lambda x: density[x])
             max_density = density[max_instance]
-            
+
             if max_density >= self.min_density:
-                labels[cl] = num_clusters            
+                labels[cl] = num_clusters
             num_clusters += 1
 
         self.labels = labels
         self._fitted = True
         return self
-    
+
     def _climb_hill(self, x: Vector, X: Matrix) -> Tuple[Vector, float, float]:
         error, prob = 99.0, 0.0
         x1 = np.copy(x)
-        
+
         iters = 0
         r_new, r_old, r_2old = 0.0, 0.0, 0.0
         while True:
             r_3old, r_2old, r_old = r_2old, r_old, r_new
             x0 = np.copy(x1)
             x1, density = self._step(x0, X)
-            
+
             error, prob = density - prob, density
             r_new = np.linalg.norm(x1 - x0)
             radius = r_3old + r_2old + r_old + r_new
-            
+
             iters += 1
-            if iters > 3 and error < self.tol: break
-            if iters == self.max_climb: 
+            if iters > 3 and error < self.tol:
+                break
+            if iters == self.max_climb:
                 raise NotConvergedError(self)
-            
+
         return x1, prob, radius
 
     def _step(self, x: Vector, X: Matrix) -> Tuple[Vector, float]:
         sup_weight = 0.0
         x1 = np.zeros((1, self._n))
-        
+
         for j in range(self._m):
             kernel = self._kernel_func(x, X[j], self._n)
-            kernel = kernel * self.sample_weight[j] / (self.h ** self._n)
-            
+            kernel = kernel * self.sample_weight[j] / (self.h**self._n)
+
             sup_weight = sup_weight + kernel
             x1 = x1 + (kernel * X[j])
-            
+
         x1 = x1 / sup_weight
         density = sup_weight / np.sum(self.sample_weight)
-        
+
         return x1, density
 
     def _kernel_func(self, xi: Vector, xj: Vector, deg: int):
-        kernel = np.exp(-(np.linalg.norm(xi - xj) / self.h) ** 2 / 2)
+        kernel = np.exp(-((np.linalg.norm(xi - xj) / self.h) ** 2) / 2)
         kernel /= (2 * np.pi) ** (deg / 2)
-        
+
         return kernel
 
     def _find_connected_components(self, adj_list: List[list]) -> list:
         def __dfs(node: int) -> Vector:
             stack, path = [node], []
             while stack:
                 vertex = stack.pop()
                 if not visited[vertex]:
                     visited[vertex] = True
                     path.append(vertex)
                     stack.extend(set(adj_list[vertex]) - set(path))
-            
+
             return Matrix(path)
 
         clusters = []
         visited = [False] * self._m
         for node in range(self._m):
-            if visited[node]: continue
+            if visited[node]:
+                continue
             cluster = __dfs(node)
             clusters.append(cluster)
-    
+
         return clusters
-    
+
     @property
     def labels(self):
         return self._labels
 
     @labels.setter
     def labels(self, value):
         self._labels = value
 
     def predict(self) -> None:
         raise Warning(f"{type(self).__name__} does not support prediction!")
-    
+
     def score(self, metric: Evaluator = SilhouetteCoefficient) -> float:
         return metric.score(self._X, self.labels)
 
 
 class MeanShiftClustering(Estimator, Unsupervised):
-    
     """
-    Mean Shift is a non-parametric, iterative clustering algorithm 
-    that identifies clusters in a dataset by updating candidate cluster 
-    centers to the mean of points within a given region (bandwidth). 
-    The process repeats until convergence, where centers no longer 
-    significantly shift. It automatically determines the number of 
-    clusters based on the data distribution. Mean Shift is especially 
+    Mean Shift is a non-parametric, iterative clustering algorithm
+    that identifies clusters in a dataset by updating candidate cluster
+    centers to the mean of points within a given region (bandwidth).
+    The process repeats until convergence, where centers no longer
+    significantly shift. It automatically determines the number of
+    clusters based on the data distribution. Mean Shift is especially
     effective in discovering clusters of arbitrary shapes and sizes.
-    
+
     Parameters
     ----------
     `bandwidth` : Window size for kernel density estimation
     `max_iter` : Maximum iteration
     `tol` : Tolerence threshold for early convergence
-    
+
     """
-    
-    def __init__(self, 
-                 bandwidth: float = 2.0, 
-                 max_iter: int = 300, 
-                 tol: float = 1e-3,
-                 verbose: bool = False) -> None:
+
+    def __init__(
+        self,
+        bandwidth: float = 2.0,
+        max_iter: int = 300,
+        tol: float = 1e-3,
+        verbose: bool = False,
+    ) -> None:
         self.bandwidth = bandwidth
         self.max_iter = max_iter
         self.tol = tol
         self.verbose = verbose
         self._X = None
         self._fitted = False
 
-    def fit(self, X: Matrix) -> 'MeanShiftClustering':
+        self.set_param_ranges(
+            {"bandwidth": ("0<,+inf", None), "max_iter": ("0<,+inf", int)}
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix) -> "MeanShiftClustering":
         self._X = X
         m, _ = X.shape
-        
+
         centers = np.copy(X)
         for iter in range(self.max_iter):
             new_centers = []
             for i in range(m):
                 points = X[np.linalg.norm(X - centers[i], axis=1) < self.bandwidth]
                 new_center = points.mean(axis=0)
                 new_centers.append(new_center)
             new_centers = Matrix(new_centers)
-            
+
             diff = np.linalg.norm(new_centers - centers)
             if self.verbose and iter % 10 == 0 and iter:
-                print(f'[MeanShift] iteration: {iter}/{self.max_iter}', end='')
-                print(f' with delta-centers-norm {diff}')
-            
+                print(f"[MeanShift] iteration: {iter}/{self.max_iter}", end="")
+                print(f" with delta-centers-norm {diff}")
+
             if diff < self.tol:
                 if self.verbose:
-                    print(f'[MeanShift] Early-convergence occurred at', end='')
-                    print(f' iteration {iter}/{self.max_iter}')
+                    print(f"[MeanShift] Early-convergence occurred at", end="")
+                    print(f" iteration {iter}/{self.max_iter}")
                 break
             centers = new_centers
-            
+
         self.centers = centers
         self._fitted = True
         return self
 
     @property
     def labels(self) -> Vector:
         return self.predict(self._X)
-    
+
     def predict(self, X: Matrix) -> Vector:
         norm_ = np.linalg.norm(X[:, np.newaxis] - self.centers, axis=2)
         cluster_labels = np.argmin(norm_, axis=1)
 
         unique_labels = np.unique(cluster_labels[cluster_labels != -1])
         mapping = {original: new for new, original in enumerate(unique_labels)}
         labels = [mapping[label] if label != -1 else -1 for label in cluster_labels]
-        
+
         return Vector(labels)
-    
+
     def score(self, metric: Evaluator = SilhouetteCoefficient) -> float:
         return metric.score(self._X, self.labels)
-
```

### Comparing `luma-ml-0.6.4/luma/clustering/hierarchy.py` & `luma-ml-0.6.5/luma/clustering/hierarchy.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,80 +7,81 @@
 from luma.interface.util import Matrix
 from luma.core.super import Estimator, Evaluator, Unsupervised
 from luma.interface.exception import NotFittedError, UnsupportedParameterError
 from luma.clustering.kmeans import KMeansClusteringPlus
 from luma.metric.clustering import SilhouetteCoefficient
 
 
-__all__ = (
-    'AgglomerativeClustering', 
-    'DivisiveClustering'
-)
+__all__ = ("AgglomerativeClustering", "DivisiveClustering")
 
 
 class AgglomerativeClustering(Estimator, Unsupervised):
-    
     """
-    Agglomerative clustering is a hierarchical clustering technique that starts 
-    by treating each data point as a single cluster. It iteratively merges the 
-    closest pairs of clusters based on a chosen distance metric. This process 
-    continues until a specified number of clusters is reached or all points 
+    Agglomerative clustering is a hierarchical clustering technique that starts
+    by treating each data point as a single cluster. It iteratively merges the
+    closest pairs of clusters based on a chosen distance metric. This process
+    continues until a specified number of clusters is reached or all points
     are merged into a single cluster.
-    
+
     Parameters
     ----------
     `n_clusters` : Number of clusters to estimate
     `linkage` : Linkage method (e.g. `single`, `complete`, `average`, `ward`)
-    
+
     Methods
     -------
     Plot hierarchical dendrogram:
     ```py
-    def plot_dendrogram(self, 
-                        ax: Optional[plt.Axes] = None, 
-                        hide_indices: bool = True, 
+    def plot_dendrogram(self,
+                        ax: Optional[plt.Axes] = None,
+                        hide_indices: bool = True,
                         show: bool = False) -> plt.Axes
     ```
     Examples
     --------
     >>> agg = AgglomerativeClustering()
     >>> agg.fit(X, y)
     >>> lables = agg.labels # Get assigned labels
-    
+
     """
-    
-    def __init__(self, 
-                 n_clusters: int = 2, 
-                 linkage: Literal['single', 'complete', 'average'] = 'single'):
+
+    def __init__(
+        self,
+        n_clusters: int = 2,
+        linkage: Literal["single", "complete", "average"] = "single",
+    ):
         self.n_clusters = n_clusters
         self.linkage = linkage
         self._X = None
         self._fitted = False
 
-    def fit(self, X: Matrix) -> 'AgglomerativeClustering':
+        self.set_param_ranges({"n_clusters": ("0<,+inf", int)})
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix) -> "AgglomerativeClustering":
         self._X = X
         n_samples = X.shape[0]
-        dist_matrix = squareform(pdist(X, metric='euclidean'))
+        dist_matrix = squareform(pdist(X, metric="euclidean"))
         clusters = {i: [i] for i in range(n_samples)}
-        
+
         while len(clusters) > self.n_clusters:
             closest_pair, _ = self._find_closest_clusters(dist_matrix, clusters)
 
             self._merge_clusters(clusters, closest_pair)
             self._update_distance_matrix(dist_matrix, closest_pair, clusters)
 
         self.clusters = clusters
         self._n = n_samples
-        
+
         self._fitted = True
         return self
 
-    def _find_closest_clusters(self, 
-                               dist_matrix: Matrix, 
-                               clusters: dict) -> Tuple[tuple, float]:
+    def _find_closest_clusters(
+        self, dist_matrix: Matrix, clusters: dict
+    ) -> Tuple[tuple, float]:
         min_dist = np.inf
         closest_pair = (None, None)
 
         for i in clusters:
             for j in clusters:
                 if i != j and dist_matrix[i, j] < min_dist:
                     min_dist = dist_matrix[i, j]
@@ -89,142 +90,146 @@
         return closest_pair, min_dist
 
     def _merge_clusters(self, clusters: Matrix, pair: tuple) -> None:
         i, j = pair
         clusters[i].extend(clusters[j])
         del clusters[j]
 
-    def _update_distance_matrix(self, 
-                                dist_matrix: Matrix, 
-                                pair: tuple, 
-                                clusters: dict) -> None:
+    def _update_distance_matrix(
+        self, dist_matrix: Matrix, pair: tuple, clusters: dict
+    ) -> None:
         i, j = pair
         for k in clusters:
-            if k == i: continue
+            if k == i:
+                continue
             value = None
-            if self.linkage == 'single':
+            if self.linkage == "single":
                 value = min(dist_matrix[i, k], dist_matrix[j, k])
-            elif self.linkage == 'complete':
+            elif self.linkage == "complete":
                 value = max(dist_matrix[i, k], dist_matrix[j, k])
-            elif self.linkage == 'average':
+            elif self.linkage == "average":
                 value = np.mean([dist_matrix[i, k], dist_matrix[j, k]])
             else:
                 raise UnsupportedParameterError(self.linkage)
-            
+
             dist_matrix[i, k] = dist_matrix[k, i] = value
         dist_matrix[i, i] = np.inf
 
     def _assign_labels(self, clusters: dict, n_samples: int) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
-        
+        if not self._fitted:
+            raise NotFittedError(self)
+
         labels = np.zeros(n_samples, dtype=int)
         for cluster_id, cluster_samples in enumerate(clusters.values()):
             for sample in cluster_samples:
                 labels[sample] = cluster_id
-        
+
         return labels
-    
-    def plot_dendrogram(self, 
-                        ax: Optional[plt.Axes] = None,
-                        hide_indices: bool = True,
-                        show: bool = False) -> plt.Axes:
+
+    def plot_dendrogram(
+        self,
+        ax: Optional[plt.Axes] = None,
+        hide_indices: bool = True,
+        show: bool = False,
+    ) -> plt.Axes:
         if ax is None:
             _, ax = plt.subplots()
             show = True
-        
+
         m = self._X.shape[0]
-        labels = [''] * m if hide_indices else list(range(m))
+        labels = [""] * m if hide_indices else list(range(m))
         Z = linkage(self._X, method=self.linkage)
         dendrogram(Z, labels=labels)
-        
-        ax.set_xlabel('Samples')
-        ax.set_ylabel('Distance')
-        ax.set_title('Dendrogram')
+
+        ax.set_xlabel("Samples")
+        ax.set_ylabel("Distance")
+        ax.set_title("Dendrogram")
         ax.figure.tight_layout()
-        
-        if show: plt.show()
+
+        if show:
+            plt.show()
         return ax
-    
+
     @property
     def labels(self) -> Matrix:
         return self._assign_labels(self.clusters, self._n)
 
     def predict(self) -> None:
         raise Warning(f"{type(self).__name__} does not support prediction!")
-    
+
     def score(self, metric: Evaluator = SilhouetteCoefficient) -> float:
         return metric.score(self._X, self.labels)
 
 
 class DivisiveClustering(Estimator, Unsupervised):
-    
     """
-    Divisive clustering is a "top-down" approach in hierarchical clustering, 
-    starting with all data points in one large cluster. It iteratively splits 
-    clusters into smaller ones based on similarity measures, typically using 
-    algorithms like K-means for splitting. The process continues until a 
-    specified number of clusters is reached or other stopping criteria are met. 
-    This method is particularly effective for datasets with well-defined, 
+    Divisive clustering is a "top-down" approach in hierarchical clustering,
+    starting with all data points in one large cluster. It iteratively splits
+    clusters into smaller ones based on similarity measures, typically using
+    algorithms like K-means for splitting. The process continues until a
+    specified number of clusters is reached or other stopping criteria are met.
+    This method is particularly effective for datasets with well-defined,
     separate clusters.
-    
+
     Parameters
     ----------
     `n_clusters` : Number of clusters to estimate
-    
+
     Examples
     --------
     >>> div = DivisiveClustering()
     >>> div.fit(X)
     >>> labels = div.labels # Get assigned labels
-    
+
     """
-    
-    def __init__(self, 
-                 n_clusters: int = 2):
+
+    def __init__(self, n_clusters: int = 2):
         self.n_clusters = n_clusters
         self.clusters = []
         self._X = None
         self._fitted = False
 
-    def fit(self, X: Matrix) -> 'DivisiveClustering':
+        self.set_param_ranges({"n_clusters": ("0<,+inf", int)})
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix) -> "DivisiveClustering":
         initial_cluster = [0] * X.shape[0]
         self._X = X
         self.clusters.append(initial_cluster)
         self._recursive_split(X)
-        
+
         self._fitted = True
         return self
 
     def _recursive_split(self, X: Matrix, depth: int = 0) -> None:
-        if depth == self.n_clusters - 1: return
-        
+        if depth == self.n_clusters - 1:
+            return
+
         max_cluster_idx = self._find_largest_cluster()
-        split_idx = [i for i, v in enumerate(self.clusters[-1]) 
-                            if v == max_cluster_idx]
+        split_idx = [i for i, v in enumerate(self.clusters[-1]) if v == max_cluster_idx]
 
         if len(split_idx) > 1:
             kmeans = KMeansClusteringPlus(n_clusters=2).fit(X[split_idx])
             new_labels = kmeans.predict(X[split_idx])
 
             new_cluster = self.clusters[-1].copy()
             new_cluster_id = max(new_cluster) + 1
             for idx, label in zip(split_idx, new_labels):
-                new_cluster[idx] = new_cluster_id \
-                    if label == 1 else max_cluster_idx
+                new_cluster[idx] = new_cluster_id if label == 1 else max_cluster_idx
 
             self.clusters.append(new_cluster)
             self._recursive_split(X, depth + 1)
 
     def _find_largest_cluster(self) -> Matrix:
         return np.argmax(np.bincount(self.clusters[-1]))
 
     @property
     def labels(self) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         return Matrix(self.clusters[-1])
-    
+
     def predict(self) -> None:
         raise Warning(f"{type(self).__name__} does not support prediction!")
-    
+
     def score(self, metric: Evaluator = SilhouetteCoefficient) -> float:
         return metric.score(self._X, self.labels)
-
```

### Comparing `luma-ml-0.6.4/luma/clustering/kmeans.py` & `luma-ml-0.6.5/luma/clustering/kmeans.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,408 +3,460 @@
 from luma.interface.util import Matrix, Vector
 from luma.interface.exception import NotFittedError
 from luma.core.super import Estimator, Evaluator, Unsupervised
 from luma.metric.clustering import SilhouetteCoefficient
 
 
 __all__ = (
-    'KMeansClustering', 
-    'KMeansClusteringPlus', 
-    'KMediansClustering', 
-    'KMedoidsClustering',
-    'MiniBatchKMeansClustering',
-    'FuzzyCMeansClustering'
+    "KMeansClustering",
+    "KMeansClusteringPlus",
+    "KMediansClustering",
+    "KMedoidsClustering",
+    "MiniBatchKMeansClustering",
+    "FuzzyCMeansClustering",
 )
 
 
 class KMeansClustering(Estimator, Unsupervised):
-    
     """
-    K-means clustering is a machine learning algorithm that  groups similar data 
-    points into clusters. It works by iteratively assigning data points to the 
-    nearest cluster center (centroid) and updating the centroids based on 
-    the assigned data points. This process continues 
+    K-means clustering is a machine learning algorithm that  groups similar data
+    points into clusters. It works by iteratively assigning data points to the
+    nearest cluster center (centroid) and updating the centroids based on
+    the assigned data points. This process continues
     until convergence.
-    
+
     Parameters
     ----------
     `n_clusters` : Number of clusters
     `max_iter` : Number of iteration
-    
+
     """
-    
-    def __init__(self, 
-                 n_clusters: int = None, 
-                 max_iter: int = 100, 
-                 verbose: bool = False) -> None:
+
+    def __init__(
+        self, n_clusters: int = None, max_iter: int = 100, verbose: bool = False
+    ) -> None:
         self.n_clusters = n_clusters
         self.max_iter = max_iter
         self.verbose = verbose
         self._X = None
         self._fitted = False
-    
-    def fit(self, X: Matrix) -> 'KMeansClustering':
+
+        self.set_param_ranges(
+            {"n_clusters": ("0<,+inf", int), "max_iter": ("0<,+inf", int)}
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix) -> "KMeansClustering":
         init_indices = np.random.choice(X.shape[0], self.n_clusters, replace=False)
         self.centroids = X[init_indices]
         self._X = X
-        
+
         for i in range(self.max_iter):
             distances = np.linalg.norm(X[:, np.newaxis] - self.centroids, axis=2)
             labels = np.argmin(distances, axis=1)
-            
-            new_centroids = [X[labels == i].mean(axis=0) for i in range(self.n_clusters)]
-            if np.all(Matrix(new_centroids) == self.centroids): 
-                if self.verbose: print(f'[K-Means] Ealry convergence at itertaion {i}')
+
+            new_centroids = [
+                X[labels == i].mean(axis=0) for i in range(self.n_clusters)
+            ]
+            if np.all(Matrix(new_centroids) == self.centroids):
+                if self.verbose:
+                    print(f"[K-Means] Ealry convergence at itertaion {i}")
                 break
-            
-            if self.verbose and i % 10 == 0: 
-                diff_norm = np.linalg.norm(Matrix(new_centroids) - Matrix(self.centroids))
-                print(f'[K-Means] iteration: {i}/{self.max_iter}', end='')
-                print(f' - delta-centroid norm: {diff_norm}')
+
+            if self.verbose and i % 10 == 0:
+                diff_norm = np.linalg.norm(
+                    Matrix(new_centroids) - Matrix(self.centroids)
+                )
+                print(f"[K-Means] iteration: {i}/{self.max_iter}", end="")
+                print(f" - delta-centroid norm: {diff_norm}")
             self.centroids = new_centroids
-            
+
         self.centroids = Matrix(self.centroids)
         self._fitted = True
         return self
-    
+
     def predict(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         distances = np.linalg.norm(X[:, np.newaxis] - self.centroids, axis=2)
         labels = np.argmin(distances, axis=1)
         return labels
-    
+
     @property
     def labels(self) -> Matrix:
         return self.predict(self._X)
-    
+
     def score(self, X: Matrix, metric: Evaluator = SilhouetteCoefficient) -> float:
         X_pred = self.predict(X)
         return metric.score(X, X_pred)
 
 
 class KMeansClusteringPlus(Estimator, Unsupervised):
-    
     """
-    K-means++ is an improved version of the original K-means clustering algorithm, 
-    designed to address some of its shortcomings and produce more robust and 
-    efficient clustering results. K-means++ was introduced by David Arthur and 
-    Sergei Vassilvitskii in a 2007 research paper titled "k-means++: 
+    K-means++ is an improved version of the original K-means clustering algorithm,
+    designed to address some of its shortcomings and produce more robust and
+    efficient clustering results. K-means++ was introduced by David Arthur and
+    Sergei Vassilvitskii in a 2007 research paper titled "k-means++:
     The Advantages of Careful Seeding."
-    
+
     Parameters
     ----------
     `n_clusters` : Number of clusters
     `max_iter` : Number of iteration
-    
+
     """
-    
-    def __init__(self, 
-                 n_clusters: int = None, 
-                 max_iter: int = 100,
-                 verbose: bool = False) -> None:
+
+    def __init__(
+        self, n_clusters: int = None, max_iter: int = 100, verbose: bool = False
+    ) -> None:
         self.n_clusters = n_clusters
         self.max_iter = max_iter
         self.verbose = verbose
         self._X = None
         self._fitted = False
 
+        self.set_param_ranges(
+            {"n_clusters": ("0<,+inf", int), "max_iter": ("0<,+inf", int)}
+        )
+        self.check_param_ranges()
+
     def _initialize_centroids(self, X: Matrix) -> None:
         self.centroids = [X[np.random.choice(X.shape[0])]]
         for _ in range(1, self.n_clusters):
-            distances = [min([np.linalg.norm(x - c) ** 2 for c in self.centroids]) for x in X]
+            distances = [
+                min([np.linalg.norm(x - c) ** 2 for c in self.centroids]) for x in X
+            ]
             distances = Matrix(distances)
-            
+
             probs = distances / distances.sum()
             next_centroid = np.random.choice(X.shape[0], p=probs)
             self.centroids.append(X[next_centroid])
-        
-    def fit(self, X: Matrix) -> 'KMeansClusteringPlus':
+
+    def fit(self, X: Matrix) -> "KMeansClusteringPlus":
         self._X = X
         self._initialize_centroids(X)
-        
+
         for _ in range(self.max_iter):
             distances = np.linalg.norm(X[:, np.newaxis] - self.centroids, axis=2)
             labels = np.argmin(distances, axis=1)
-            
+
             for i in range(self.n_clusters):
                 cluster_points = X[labels == i]
-                if len(cluster_points) == 0: continue
+                if len(cluster_points) == 0:
+                    continue
                 self.centroids[i] = np.mean(cluster_points, axis=0)
-            
-            if self.verbose and i % 10 == 0: 
-                print(f'[K-Means++] iteration: {i}/{self.max_iter}', end='')
-        
+
+            if self.verbose and i % 10 == 0:
+                print(f"[K-Means++] iteration: {i}/{self.max_iter}", end="")
+
         self.centroids = Matrix(self.centroids)
         self._fitted = True
         return self
-    
+
     def predict(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         distances = np.linalg.norm(X[:, np.newaxis] - self.centroids, axis=2)
         labels = np.argmin(distances, axis=1)
         return labels
-    
+
     @property
     def labels(self) -> Matrix:
         return self.predict(self._X)
-    
+
     def score(self, X: Matrix, metric: Evaluator = SilhouetteCoefficient) -> float:
         X_pred = self.predict(X)
         return metric.score(X, X_pred)
 
 
 class KMediansClustering(Estimator, Unsupervised):
-    
     """
-    K-median clustering is a data clustering method that divides a dataset into 
-    K clusters with each cluster having a median point as its representative. 
-    It uses distance metrics like Manhattan or Euclidean distance to minimize 
-    the sum of distances between data points and their cluster medians, 
+    K-median clustering is a data clustering method that divides a dataset into
+    K clusters with each cluster having a median point as its representative.
+    It uses distance metrics like Manhattan or Euclidean distance to minimize
+    the sum of distances between data points and their cluster medians,
     making it less sensitive to outliers and adaptable to non-Euclidean data.
-    
+
     Parameters
     ----------
     `n_clusters` : Number of clusters
     `max_iter` : Number of iteration
-    
+
     """
-    
-    def __init__(self, 
-                 n_clusters: int = None, 
-                 max_iter: int = 100,
-                 verbose: bool = False) -> None:
+
+    def __init__(
+        self, n_clusters: int = None, max_iter: int = 100, verbose: bool = False
+    ) -> None:
         self.n_clusters = n_clusters
         self.max_iter = max_iter
         self.verbose = verbose
         self._X = None
         self._fitted = False
-        
-    def fit(self, X: Matrix) -> 'KMediansClustering':
+
+        self.set_param_ranges(
+            {"n_clusters": ("0<,+inf", int), "max_iter": ("0<,+inf", int)}
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix) -> "KMediansClustering":
         self._X = X
         self.medians = X[np.random.choice(X.shape[0], self.n_clusters, replace=False)]
-        
+
         for i in range(self.max_iter):
             distances = np.abs(X[:, np.newaxis] - self.medians)
             labels = np.argmin(distances.sum(axis=2), axis=1)
 
-            new_medians = [np.median(X[labels == i], axis=0) for i in range(self.n_clusters)]
+            new_medians = [
+                np.median(X[labels == i], axis=0) for i in range(self.n_clusters)
+            ]
             new_medians = Matrix(new_medians)
-            
-            if np.all(Matrix(new_medians) == self.medians): 
-                if self.verbose: print(f'[K-Medians] Ealry convergence at itertaion {i}')
+
+            if np.all(Matrix(new_medians) == self.medians):
+                if self.verbose:
+                    print(f"[K-Medians] Ealry convergence at itertaion {i}")
                 break
-            
-            if self.verbose and i % 10 == 0: 
+
+            if self.verbose and i % 10 == 0:
                 diff_norm = np.linalg.norm(Matrix(new_medians) - Matrix(self.medians))
-                print(f'[K-Medians] iteration: {i}/{self.max_iter}', end='')
-                print(f' - delta-centroid norm: {diff_norm}')
-            
+                print(f"[K-Medians] iteration: {i}/{self.max_iter}", end="")
+                print(f" - delta-centroid norm: {diff_norm}")
+
             self.medians = new_medians
-        
+
         self._fitted = True
         return self
-    
+
     def predict(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         distances = np.abs(X[:, np.newaxis] - self.medians)
         labels = np.argmin(distances.sum(axis=2), axis=1)
         return labels
-    
+
     @property
     def labels(self) -> Matrix:
         return self.predict(self._X)
-    
+
     def score(self, X: Matrix, metric: Evaluator = SilhouetteCoefficient) -> float:
         X_pred = self.predict(X)
         return metric.score(X, X_pred)
 
 
 class KMedoidsClustering(Estimator, Unsupervised):
-    
     """
-    K-Medoids is a clustering algorithm similar to K-Means, but it uses actual 
-    data points as cluster centers (medoids) instead of centroids. It minimizes 
-    the sum of dissimilarities between points labeled to be in a cluster and a 
-    point designated as the medoid of that cluster. During each iteration, it 
-    reassigns points to the closest medoid and updates medoids based on the 
-    current cluster assignments. K-Medoids is more robust to noise and outliers 
+    K-Medoids is a clustering algorithm similar to K-Means, but it uses actual
+    data points as cluster centers (medoids) instead of centroids. It minimizes
+    the sum of dissimilarities between points labeled to be in a cluster and a
+    point designated as the medoid of that cluster. During each iteration, it
+    reassigns points to the closest medoid and updates medoids based on the
+    current cluster assignments. K-Medoids is more robust to noise and outliers
     compared to K-Means.
-    
+
     Parameters
     ----------
     `n_clusters` : Number of clusters to estimate
     `max_iter` : Maximum iteration for PAM (Partitioning Around Medoids) algorithm
     `random_state` : Seed for randomized initialization of medoids
-    
+
     """
-    
-    def __init__(self, 
-                 n_clusters: int, 
-                 max_iter: int = 300, 
-                 random_state: int = None,
-                 verbose: bool = False) -> None:
+
+    def __init__(
+        self,
+        n_clusters: int,
+        max_iter: int = 300,
+        random_state: int = None,
+        verbose: bool = False,
+    ) -> None:
         self.n_clusters = n_clusters
         self.max_iter = max_iter
         self.random_state = random_state
         self.medoids = None
         self.verbose = verbose
         self._X = None
         self._fitted = False
 
-    def fit(self, X: Matrix) -> 'KMedoidsClustering': 
+        self.set_param_ranges(
+            {"n_clusters": ("0<,+inf", int), "max_iter": ("0<,+inf", int)}
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix) -> "KMedoidsClustering":
         self._X = X
         m, _ = X.shape
         np.random.seed(self.random_state)
         initial_indices = np.random.choice(m, self.n_clusters, replace=False)
         self.medoids = X[initial_indices]
-        
+
         for i in range(self.max_iter):
             labels = self._closest_medoid(X, self.medoids)
-            new_medoids = Matrix([X[labels == n_clusters].mean(axis=0) 
-                                  for n_clusters in range(self.n_clusters)])
+            new_medoids = Matrix(
+                [
+                    X[labels == n_clusters].mean(axis=0)
+                    for n_clusters in range(self.n_clusters)
+                ]
+            )
 
             if self.verbose and i % 10 == 0 and i:
-                print(f'[K-Medoids] iteration: {i}/{self.max_iter}', end='')
-                print(f' with medoids-norm {np.linalg.norm(self.medoids)}')
-            
-            if np.all(new_medoids == self.medoids): 
+                print(f"[K-Medoids] iteration: {i}/{self.max_iter}", end="")
+                print(f" with medoids-norm {np.linalg.norm(self.medoids)}")
+
+            if np.all(new_medoids == self.medoids):
                 if self.verbose:
-                    print(f'[K-Medoids] Early-convergence at iteration')
-                    print(f'{i}/{self.max_iter}')
+                    print(f"[K-Medoids] Early-convergence at iteration")
+                    print(f"{i}/{self.max_iter}")
                 break
-            
+
             self.medoids = new_medoids
-        
+
         self._fitted = True
         return self
 
     def _closest_medoid(self, X: Matrix, medoids: Matrix) -> Matrix:
         distances = np.zeros((X.shape[0], self.n_clusters))
         for idx, medoid in enumerate(medoids):
             distances[:, idx] = np.linalg.norm(X - medoid, axis=1)
-        
+
         return np.argmin(distances, axis=1)
-    
+
     @property
     def labels(self) -> Vector:
         return self._closest_medoid(self._X, self.medoids)
-    
+
     def predict(self, X: Matrix) -> Vector:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         return self._closest_medoid(X, self.medoids)
-    
+
     def score(self, X: Matrix, metric: Evaluator = SilhouetteCoefficient) -> float:
         X_pred = self.predict(X)
         return metric.score(X, X_pred)
 
 
 class MiniBatchKMeansClustering(Estimator, Unsupervised):
-    
     """
-    Mini-Batch K-Means is an efficient variation of the traditional K-Means 
-    clustering algorithm, designed to handle large datasets more effectively. 
-    It operates by randomly selecting small subsets of the dataset (mini-batches) 
-    and using these subsets, rather than the entire dataset, to update the 
-    cluster centroids in each iteration. This approach significantly reduces 
-    the computational cost and memory requirements, making it well-suited 
+    Mini-Batch K-Means is an efficient variation of the traditional K-Means
+    clustering algorithm, designed to handle large datasets more effectively.
+    It operates by randomly selecting small subsets of the dataset (mini-batches)
+    and using these subsets, rather than the entire dataset, to update the
+    cluster centroids in each iteration. This approach significantly reduces
+    the computational cost and memory requirements, making it well-suited
     for big data applications.
-    
+
     Parameters
     ----------
     `n_clusters` : Number of clusters to estimate
     `batch_size` : Size of a single mini-batch
     `max_iter` : Maximum amount of iteration
-    
+
     """
-    
-    def __init__(self, 
-                 n_clusters: int = None, 
-                 batch_size: int = 100, 
-                 max_iter: int = 100):
+
+    def __init__(
+        self, n_clusters: int = None, batch_size: int = 100, max_iter: int = 100
+    ) -> None:
         self.n_clusters = n_clusters
         self.batch_size = batch_size
         self.max_iter = max_iter
         self.centroids = None
         self._X = None
         self._fitted = False
 
-    def fit(self, X: Matrix) -> 'MiniBatchKMeansClustering':
+        self.set_param_ranges(
+            {
+                "n_clusters": ("0<,+inf", int),
+                "max_iter": ("0<,+inf", int),
+                "batch_size": ("0<,+inf", int),
+            }
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix) -> "MiniBatchKMeansClustering":
         m, _ = X.shape
         self._X = X
-        
+
         rand_idx = np.random.choice(m, self.n_clusters, replace=False)
         self.centroids = X[rand_idx]
 
         for _ in range(self.max_iter):
             batch_idx = np.random.choice(m, self.batch_size, replace=False)
             batch = X[batch_idx]
-            
+
             distances = np.linalg.norm(batch[:, np.newaxis] - self.centroids, axis=2)
             closest_cluster_idx = np.argmin(distances, axis=1)
-            
+
             for i in range(self.n_clusters):
                 cluster_points = batch[closest_cluster_idx == i]
                 if len(cluster_points) > 0:
                     self.centroids[i] = np.mean(cluster_points, axis=0)
-        
+
         self._fitted = True
         return self
 
     def predict(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         distances = np.linalg.norm(X[:, np.newaxis] - self.centroids, axis=2)
         return np.argmin(distances, axis=1)
-    
+
     @property
     def labels(self) -> Matrix:
         return self.predict(self._X)
 
     def score(self, X: Matrix, metric: Evaluator = SilhouetteCoefficient) -> float:
         X_pred = self.predict(X)
         return metric.score(X, X_pred)
 
 
 class FuzzyCMeansClustering(Estimator, Unsupervised):
-    
     """
-    Fuzzy C-Means (FCM) is a clustering algorithm where each data point can 
-    belong to multiple clusters with varying degrees of membership. It 
-    iteratively updates cluster centroids and membership levels based on the 
-    distance of points to centroids, weighted by their membership. The 
-    algorithm is suitable for data with overlapping or unclear boundaries 
-    between clusters. FKM provides a soft partitioning of the data, allowing 
+    Fuzzy C-Means (FCM) is a clustering algorithm where each data point can
+    belong to multiple clusters with varying degrees of membership. It
+    iteratively updates cluster centroids and membership levels based on the
+    distance of points to centroids, weighted by their membership. The
+    algorithm is suitable for data with overlapping or unclear boundaries
+    between clusters. FKM provides a soft partitioning of the data, allowing
     more flexible cluster assignments compared to hard clustering methods.
-    
+
     Parameters
     ----------
     `n_clusters` : Number of clusters to estimate
     `max_iter` : Maximum iteration
     `m`: Fuzziness parameter (larger makes labels softer)
     `tol` : Threshold for early convergence
     `random_state` : Seed for randomized initialization of centers
-    
+
     """
-    
-    def __init__(self, 
-                 n_clusters: int, 
-                 max_iter: int = 100, 
-                 m: float = 2.0, 
-                 tol: float = 1e-5,
-                 random_state: int = None,
-                 verbose: bool = False) -> None:
+
+    def __init__(
+        self,
+        n_clusters: int,
+        max_iter: int = 100,
+        m: float = 2.0,
+        tol: float = 1e-5,
+        random_state: int = None,
+        verbose: bool = False,
+    ) -> None:
         self.n_clusters = n_clusters
         self.max_iter = max_iter
         self.m = m
         self.tol = tol
         self.random_state = random_state
         self.verbose = verbose
         self._X = None
         self._fitted = False
 
-    def fit(self, X: Matrix) -> 'FuzzyCMeansClustering':
+        self.set_param_ranges(
+            {
+                "n_clusters": ("0<,+inf", int),
+                "max_iter": ("0<,+inf", int),
+                "m": ("0,+inf", None),
+            }
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix) -> "FuzzyCMeansClustering":
         self._X = X
         m, _ = X.shape
 
         np.random.seed(self.random_state)
         self.centers = X[np.random.choice(m, self.n_clusters, replace=False)]
         self.membership = np.zeros((m, self.n_clusters))
 
@@ -415,49 +467,49 @@
                     self.membership[i, j] = 1 / sum_term if sum_term != 0 else 0
 
             prev_centers = np.copy(self.centers)
             for j in range(self.n_clusters):
                 num_ = sum([self.membership[i, j] ** self.m * X[i] for i in range(m)])
                 denom_ = sum([self.membership[i, j] ** self.m for i in range(m)])
                 self.centers[j] = num_ / denom_ if denom_ else 0
-            
+
             diff = np.linalg.norm(self.centers - prev_centers)
             if self.verbose and iter % 10 == 0 and iter:
-                print(f'[FKM] iteration: {iter}/{self.max_iter}', end='')
-                print(f' with delta-center-norm: {diff}')
+                print(f"[FKM] iteration: {iter}/{self.max_iter}", end="")
+                print(f" with delta-center-norm: {diff}")
 
-            if diff < self.tol: 
+            if diff < self.tol:
                 if self.verbose:
-                    print(f'[FKM] Early-convergnece at iteration', end='')
-                    print(f' {iter}/{self.max_iter}')
+                    print(f"[FKM] Early-convergnece at iteration", end="")
+                    print(f" {iter}/{self.max_iter}")
                 break
-        
+
         self._fitted = True
         return self
-    
+
     def _sum(self, X: Matrix, i: int, j: int) -> Matrix:
         sum_term = 0
         for k in range(self.n_clusters):
             distance_ratio = np.linalg.norm(X[i] - self.centers[j])
-            distance_ratio /= (np.linalg.norm(X[i] - self.centers[k]) + self.tol)
-            sum_term += (distance_ratio ** (2 / (self.m - 1)))
-        
+            distance_ratio /= np.linalg.norm(X[i] - self.centers[k]) + self.tol
+            sum_term += distance_ratio ** (2 / (self.m - 1))
+
         return sum_term
 
     @property
     def labels(self) -> Vector:
         return self.predict(self._X)
 
     def predict(self, X: Matrix) -> Vector:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         m, _ = X.shape
         predictions = np.zeros(m)
         for i in range(m):
             distances = [np.linalg.norm(X[i] - center) for center in self.centers]
             predictions[i] = np.argmin(distances)
-        
+
         return predictions
 
     def score(self, X: Matrix, metric: Evaluator = SilhouetteCoefficient) -> float:
         X_pred = self.predict(X)
         return metric.score(X, X_pred)
-
```

### Comparing `luma-ml-0.6.4/luma/clustering/mixture.py` & `luma-ml-0.6.5/luma/clustering/mixture.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,158 +2,174 @@
 
 from luma.core.super import Estimator, Evaluator, Unsupervised
 from luma.interface.util import Matrix, Vector
 from luma.metric.clustering import SilhouetteCoefficient
 from luma.interface.exception import NotFittedError
 
 
-__all__ = (
-    'GaussianMixture',
-    'MultinomialMixture'
-)
+__all__ = ("GaussianMixture", "MultinomialMixture")
 
 
 class GaussianMixture(Estimator, Unsupervised):
-    
     """
-    A Gaussian Mixture Model (GMM) is a probabilistic model for representing 
-    an ensemble of multiple Gaussian distributions within a dataset. It is 
-    used in clustering by assuming each cluster follows a different Gaussian 
-    distribution. GMM provides soft clustering, assigning probabilities to 
-    each data point for belonging to each cluster. The model parameters are 
+    A Gaussian Mixture Model (GMM) is a probabilistic model for representing
+    an ensemble of multiple Gaussian distributions within a dataset. It is
+    used in clustering by assuming each cluster follows a different Gaussian
+    distribution. GMM provides soft clustering, assigning probabilities to
+    each data point for belonging to each cluster. The model parameters are
     estimated using the Expectation-Maximization algorithm.
-    
+
     Parameters
     ----------
     `n_clusters` : Number of clusters to estimate
     `max_iter` : Maximum amount of iteration
     `tol` : Tolerance for early convergence
     `random_state` : Seed for random permutation
-    
+
     """
-    
-    def __init__(self, 
-                 n_clusters : int,
-                 max_iter: int = 100,
-                 tol: float = 1e-5,
-                 random_state: int = None,
-                 verbose: bool = False) -> None:
+
+    def __init__(
+        self,
+        n_clusters: int,
+        max_iter: int = 100,
+        tol: float = 1e-5,
+        random_state: int = None,
+        verbose: bool = False,
+    ) -> None:
         self.n_clusters = n_clusters
         self.max_iter = max_iter
         self.tol = tol
         self.random_state = random_state
         self.verbose = verbose
         self._X = None
         self._fitted = False
-    
-    def fit(self, X: Matrix) -> 'GaussianMixture':
+
+        self.set_param_ranges(
+            {
+                "n_clusters": ("0<,+inf", int),
+                "max_iter": ("0<,+inf", int),
+            }
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix) -> "GaussianMixture":
         self._X = X
         self._initialize_params(X)
         for i in range(self.max_iter):
             R = self._E_step(X)
             means_old = self.means.copy()
-            
+
             self._M_step(X, R)
             norm_ = np.linalg.norm(self.means - means_old)
-            
+
             if self.verbose and i % 20 and i:
-                print(f'[GMM] Finished iteration {i}/{self.max_iter}', end='')
-                print(f' with delta-means-norm: {norm_}')
-            
+                print(f"[GMM] Finished iteration {i}/{self.max_iter}", end="")
+                print(f" with delta-means-norm: {norm_}")
+
             if norm_ < self.tol:
                 if self.verbose:
-                    print(f'[GMM] Early-convergence at iteration', end='')
-                    print(f' {i}/{self.max_iter}')
+                    print(f"[GMM] Early-convergence at iteration", end="")
+                    print(f" {i}/{self.max_iter}")
                 break
-        
+
         self._fitted = True
         return self
-    
+
     def _initialize_params(self, X: Matrix) -> None:
         m, _ = X.shape
         np.random.seed(self.random_state)
-        random_indices = np.random.permutation(m)[:self.n_clusters]
-        
+        random_indices = np.random.permutation(m)[: self.n_clusters]
+
         self.means = X[random_indices]
         self.covs = Matrix([np.cov(X.T) for _ in range(self.n_clusters)])
         self.weights = np.full(self.n_clusters, 1 / self.n_clusters)
-    
+
     def _E_step(self, X: Matrix) -> Matrix:
         m, n = X.shape
         resp = np.zeros((m, self.n_clusters))
-        
+
         for i in range(self.n_clusters):
             cov_inv = np.linalg.inv(self.covs[i])
             diff = X - self.means[i]
             exp_term = np.exp(-0.5 * np.sum(diff.dot(cov_inv) * diff, axis=1))
             coeff = 1 / np.sqrt(np.linalg.det(self.covs[i]) * (2 * np.pi) ** n)
             resp[:, i] = self.weights[i] * coeff * exp_term
-        
+
         resp /= resp.sum(axis=1, keepdims=True)
         return resp
-    
+
     def _M_step(self, X: Matrix, R: Matrix) -> None:
         self.weights = R.mean(axis=0)
         self.means = R.T.dot(X) / np.sum(R, axis=0)[:, np.newaxis]
         for i in range(self.n_clusters):
             diff = X - self.means[i]
             self.covs[i] = (R[:, i, np.newaxis] * diff).T.dot(diff) / R[:, i].sum()
-    
+
     @property
     def labels(self) -> Vector:
         return self.predict(self._X)
-    
+
     def predict(self, X: Matrix) -> Vector:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         R = self._E_step(X)
         return np.argmax(R, axis=1)
-    
+
     def predict_proba(self, X: Matrix) -> Vector:
         return self._E_step(X)
-    
+
     def score(self, X: Matrix, metric: Evaluator = SilhouetteCoefficient) -> float:
         X_pred = self.predict(X)
         return metric.score(X, X_pred)
 
 
 class MultinomialMixture(Estimator, Unsupervised):
-    
     """
-    Multinomial Mixture Models (MMM) cluster categorical data using a mixture 
-    of multinomial distributions. Each cluster is modeled with a distinct 
-    multinomial distribution, representing the probability of each category 
-    within that cluster. The Expectation-Maximization (EM) algorithm is 
-    typically used to estimate model parameters, including cluster 
-    probabilities and multinomial parameters. MMM is commonly applied in text 
-    analysis and other scenarios involving discrete data, like document 
+    Multinomial Mixture Models (MMM) cluster categorical data using a mixture
+    of multinomial distributions. Each cluster is modeled with a distinct
+    multinomial distribution, representing the probability of each category
+    within that cluster. The Expectation-Maximization (EM) algorithm is
+    typically used to estimate model parameters, including cluster
+    probabilities and multinomial parameters. MMM is commonly applied in text
+    analysis and other scenarios involving discrete data, like document
     clustering or topic modeling.
 
     Parameters
     ----------
     `n_clusters` : Number of clusters to estimate
     `max_iter` : Maximum amount of iteration
     `tol` : Tolerance for early convergence
-    
+
     """
 
-    def __init__(self, 
-                 n_clusters: int, 
-                 max_iter: int = 100, 
-                 tol: float = 1e-5, 
-                 verbose: bool = False):
+    def __init__(
+        self,
+        n_clusters: int,
+        max_iter: int = 100,
+        tol: float = 1e-5,
+        verbose: bool = False,
+    ):
         self.n_clusters = n_clusters
         self.max_iter = max_iter
         self.tol = tol
         self.verbose = verbose
         self.pi = None
         self.theta = None
         self.X_ = None
         self._fitted = False
 
-    def fit(self, X: Matrix) -> 'MultinomialMixture':
+        self.set_param_ranges(
+            {
+                "n_clusters": ("0<,+inf", int),
+                "max_iter": ("0<,+inf", int),
+            }
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix) -> "MultinomialMixture":
         self.X_ = X
         self._initialize_parameters(X)
         logL = None
 
         for i in range(self.max_iter):
             resp = self._E_step(X)
             self._M_step(X, resp)
@@ -161,29 +177,28 @@
             log_prob_cluster = np.log(self.theta) @ X.T
             log_prob_cluster += np.log(self.pi[:, np.newaxis])
             log_prob_samples = self._logsumexp(log_prob_cluster, axis=0)
             current_logL = np.sum(log_prob_samples)
 
             if logL is not None and np.abs(current_logL - logL) < self.tol:
                 if self.verbose:
-                    print(f'EM converged at iteration {i+1}',
-                          f'with log-likelihood: {current_logL}')
+                    print(
+                        f"EM converged at iteration {i+1}",
+                        f"with log-likelihood: {current_logL}",
+                    )
                 break
-            
+
             logL = current_logL
             if self.verbose and (i + 1) % 10 == 0:
-                print(f'Iteration {i+1}, log-likelihood: {logL}')
+                print(f"Iteration {i+1}, log-likelihood: {logL}")
 
         self._fitted = True
         return self
-    
-    def _logsumexp(self, 
-                   a: Matrix, 
-                   axis: int = None, 
-                   keepdims: bool = False) -> Matrix:
+
+    def _logsumexp(self, a: Matrix, axis: int = None, keepdims: bool = False) -> Matrix:
         a_max = np.max(a, axis=axis, keepdims=True)
         tmp = np.exp(a - a_max)
         s = np.sum(tmp, axis=axis, keepdims=keepdims)
         out = np.log(s)
         if not keepdims:
             a_max = np.squeeze(a_max, axis=axis)
         out += a_max
@@ -193,33 +208,32 @@
         _, n = X.shape
         self.pi = np.ones(self.n_clusters) / self.n_clusters
         self.theta = np.random.dirichlet(alpha=np.ones(n), size=self.n_clusters)
 
     def _E_step(self, X: Matrix) -> Matrix:
         log_prob = np.log(self.theta) @ X.T + np.log(self.pi[:, np.newaxis])
         log_resp = log_prob - self._logsumexp(log_prob, axis=0, keepdims=True)
-        
+
         return np.exp(log_resp).T
 
     def _M_step(self, X: Matrix, resp: Matrix) -> None:
         nk = resp.sum(axis=0) + 10 * np.finfo(resp.dtype).eps
         self.pi = nk / nk.sum()
         self.theta = (resp.T @ X) / nk[:, np.newaxis]
 
     @property
     def labels(self) -> Vector:
         return self.predict(self.X_)
 
     def predict(self, X: Matrix) -> Vector:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         resp = self._E_step(X)
         return np.argmax(resp, axis=1)
 
     def fit_predict(self, X: Matrix) -> Vector:
         self.fit(X)
         return self.predict(X)
 
-    def score(self, X: Matrix, 
-              metric: Evaluator = SilhouetteCoefficient) -> float:
+    def score(self, X: Matrix, metric: Evaluator = SilhouetteCoefficient) -> float:
         X_pred = self.predict(X)
         return metric.score(X, X_pred)
-
```

### Comparing `luma-ml-0.6.4/luma/clustering/spectral.py` & `luma-ml-0.6.5/luma/clustering/spectral.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,312 +9,329 @@
 from luma.interface.util import Matrix
 from luma.core.super import Estimator, Evaluator, Unsupervised
 from luma.interface.exception import NotFittedError, UnsupportedParameterError
 from luma.metric.clustering import SilhouetteCoefficient
 
 
 __all__ = (
-    'SpectralClustering', 
-    'NormalizedSpectralClustering',
-    'HierarchicalSpectralClustering',
-    'AdaptiveSpectralClustering'
+    "SpectralClustering",
+    "NormalizedSpectralClustering",
+    "HierarchicalSpectralClustering",
+    "AdaptiveSpectralClustering",
 )
 
 
 class SpectralClustering(Estimator, Unsupervised):
-    
     """
-    Spectral clustering transforms data into a new space using the 
-    eigenvectors of its graph Laplacian, revealing cluster structure. 
-    It constructs a similarity graph from the data, capturing complex 
-    relationships between points. The algorithm then applies 
-    dimensionality reduction followed by a traditional clustering 
-    method, like K-means, in this transformed space. This approach 
-    is effective for identifying clusters with irregular shapes 
+    Spectral clustering transforms data into a new space using the
+    eigenvectors of its graph Laplacian, revealing cluster structure.
+    It constructs a similarity graph from the data, capturing complex
+    relationships between points. The algorithm then applies
+    dimensionality reduction followed by a traditional clustering
+    method, like K-means, in this transformed space. This approach
+    is effective for identifying clusters with irregular shapes
     and non-linearly separable data.
-    
+
     Parameters
     ----------
     `n_clusters` : Number of clusters to estimate
     `gamma` : Scaling factor for Gaussian kernel
-    
+
     Examples
     --------
     >>> sp = SpectralClustering()
     >>> sp.fit(X, y)
     >>> lables = sp.labels # Get assigned labels
-    
+
     """
-    
-    def __init__(self, 
-                 n_clusters: int, 
-                 gamma: float = 1.0):
+
+    def __init__(self, n_clusters: int, gamma: float = 1.0):
         self.n_clusters = n_clusters
         self.gamma = gamma
         self._X = None
         self._fitted = False
-    
-    def fit(self, X: Matrix) -> 'SpectralClustering':
+
+        self.set_param_ranges(
+            {"n_clusters": ("0<,+inf", int), "gamma": ("0<,+inf", None)}
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix) -> "SpectralClustering":
         self._X = X
         W = self._similarity_matrix(X)
         L = self._laplacian(W)
-        
+
         _, eigenvecs = eigh(L)
-        V = eigenvecs[:, :self.n_clusters]
+        V = eigenvecs[:, : self.n_clusters]
         kmeans = KMeansClusteringPlus(n_clusters=self.n_clusters)
         self.kmeans = kmeans.fit(V)
-        
+
         self._fitted = True
         return self
 
     def _similarity_matrix(self, X: Matrix) -> Matrix:
-        sq_dists = pdist(X, 'sqeuclidean')
+        sq_dists = pdist(X, "sqeuclidean")
         mat_sq_dists = squareform(sq_dists)
         return np.exp(-self.gamma * mat_sq_dists)
 
     def _laplacian(self, W: Matrix) -> Matrix:
         D = np.diag(np.sum(W, axis=1))
         return D - W
 
     @property
     def labels(self) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         return self.kmeans.labels
-    
+
     def predict(self) -> None:
         raise Warning(f"{type(self).__name__} does not support prediction!")
-    
+
     def score(self, metric: Evaluator = SilhouetteCoefficient) -> float:
         return metric.score(self._X, self.labels)
 
 
 class NormalizedSpectralClustering(Estimator, Unsupervised):
-    
     """
-    Normalized spectral clustering is a technique that begins by constructing 
-    a similarity matrix from the data, often using a Gaussian kernel. The graph 
-    Laplacian matrix, derived from this similarity matrix, is then normalized 
-    to enhance the distinctiveness of clusters. Eigenvalue decomposition is 
-    applied to this normalized Laplacian, and the resulting eigenvectors are 
-    used to transform the data into a new space. Finally, a clustering algorithm, 
-    such as k-means, is applied in this transformed space, effectively revealing 
+    Normalized spectral clustering is a technique that begins by constructing
+    a similarity matrix from the data, often using a Gaussian kernel. The graph
+    Laplacian matrix, derived from this similarity matrix, is then normalized
+    to enhance the distinctiveness of clusters. Eigenvalue decomposition is
+    applied to this normalized Laplacian, and the resulting eigenvectors are
+    used to transform the data into a new space. Finally, a clustering algorithm,
+    such as k-means, is applied in this transformed space, effectively revealing
     clusters that are not easily distinguishable in the original space.
-    
+
     Parameters
     ----------
     `n_clusters` : Number of clusters to estimate
     `gamma` : Scaling factor for Gaussian kernel
     `strategy` : Normalization strategy (e.g. `symmetric`, `random-walk`)
-    
+
     """
-    
-    def __init__(self, 
-                 n_clusters: int,
-                 gamma: float = 1.0,
-                 strategy: Literal['symmetric', 
-                                   'random-walk'] = 'symmetric') -> None:
+
+    def __init__(
+        self,
+        n_clusters: int,
+        gamma: float = 1.0,
+        strategy: Literal["symmetric", "random-walk"] = "symmetric",
+    ) -> None:
         self.n_clusters = n_clusters
         self.gamma = gamma
         self.strategy = strategy
         self._X = None
         self._fitted = False
-    
-    def fit(self, X: Matrix) -> 'NormalizedSpectralClustering':
+
+        self.set_param_ranges(
+            {"n_clusters": ("0<,+inf", int), "gamma": ("0<,+inf", None)}
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix) -> "NormalizedSpectralClustering":
         self._X = X
         W = self._similarity_matrix(X)
         L_norm = self._normalize_laplacian(W)
-        
+
         _, eigvecs = eigh(L_norm)
-        V = eigvecs[:, :self.n_clusters]
+        V = eigvecs[:, : self.n_clusters]
         kmeans = KMeansClusteringPlus(n_clusters=self.n_clusters)
         self.kmeans = kmeans.fit(V)
-        
+
         self._fitted = True
         return self
-    
+
     def _similarity_matrix(self, X: Matrix) -> Matrix:
-        sq_dists = pdist(X, 'sqeuclidean')
+        sq_dists = pdist(X, "sqeuclidean")
         mat_sq_dists = squareform(sq_dists)
         return np.exp(-self.gamma * mat_sq_dists)
-    
+
     def _normalize_laplacian(self, W: Matrix) -> Matrix:
         D = np.diag(np.sum(W, axis=1))
         D_inv = np.diag(1 / np.diag(D))
         D_inv_sqrt = np.diag(1 / np.sqrt(np.diag(D)))
-        
-        if self.strategy == 'symmetric':
+
+        if self.strategy == "symmetric":
             L_norm = np.eye(*D.shape) - D_inv_sqrt.dot(W).dot(D_inv_sqrt)
-        elif self.strategy == 'random-walk':
+        elif self.strategy == "random-walk":
             L_norm = np.eye(*D.shape) - D_inv.dot(W)
         else:
             raise UnsupportedParameterError(self.strategy)
 
         return L_norm
-    
+
     @property
     def labels(self) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         return self.kmeans.labels
 
     def predict(self) -> None:
         raise Warning(f"{type(self).__name__} does not support prediction!")
-    
+
     def score(self, metric: Evaluator = SilhouetteCoefficient) -> float:
         return metric.score(self._X, self.labels)
 
 
 class HierarchicalSpectralClustering(Estimator, Unsupervised):
-    
     """
-    Hierarchical spectral clustering starts by applying spectral clustering 
-    to transform data into a space where clusters are more linearly separable. 
-    This involves constructing a similarity matrix, computing the Laplacian, 
-    and performing eigenvalue decomposition. The transformed data is then 
-    clustered using hierarchical methods, either agglomerative (building 
-    clusters by merging smaller ones) or divisive (splitting larger clusters 
-    into smaller ones). This approach reveals multi-level structures in the 
+    Hierarchical spectral clustering starts by applying spectral clustering
+    to transform data into a space where clusters are more linearly separable.
+    This involves constructing a similarity matrix, computing the Laplacian,
+    and performing eigenvalue decomposition. The transformed data is then
+    clustered using hierarchical methods, either agglomerative (building
+    clusters by merging smaller ones) or divisive (splitting larger clusters
+    into smaller ones). This approach reveals multi-level structures in the
     data, uncovering both broad and fine-grained clustering patterns.
-    
+
     Parameters
     ----------
     `n_clusters` : Number of clusters to estimate
     `method` : Method for hierarchical clustering
     (e.g. `agglomerative`, `divisive`)
     `linkage` : Linkage method for `agglomerative` clustering
     (e.g. `single`, `complete`, `average`, `ward`)
     `gamma` : Scaling factor for Gaussian kernel
-    
+
     """
-    
-    def __init__(self, 
-                 n_clusters: int, 
-                 method: Literal['agglomerative', 'divisive'],
-                 linkage: Literal['single', 'complete', 'average'] = 'single',
-                 gamma: float = 1.0,):
+
+    def __init__(
+        self,
+        n_clusters: int,
+        method: Literal["agglomerative", "divisive"],
+        linkage: Literal["single", "complete", "average"] = "single",
+        gamma: float = 1.0,
+    ):
         self.n_clusters = n_clusters
         self.method = method
         self.linkage = linkage
         self.gamma = gamma
         self._hierarchy_model = None
         self._X = None
         self._fitted = False
-    
-    def fit(self, X: Matrix) -> 'HierarchicalSpectralClustering':
+
+        self.set_param_ranges(
+            {"n_clusters": ("0<,+inf", int), "gamma": ("0<,+inf", None)}
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix) -> "HierarchicalSpectralClustering":
         self._X = X
         W = self._similarity_matrix(X)
         L = self._laplacian(W)
-        
+
         _, eigenvecs = eigh(L)
-        V = eigenvecs[:, :self.n_clusters]
-        
-        if self.method == 'agglomerative':
+        V = eigenvecs[:, : self.n_clusters]
+
+        if self.method == "agglomerative":
             self._hierarchy_model = AgglomerativeClustering()
-        elif self.method == 'divisive':
+        elif self.method == "divisive":
             self._hierarchy_model = DivisiveClustering()
         else:
             raise UnsupportedParameterError(self.method)
-        
+
         self._hierarchy_model.n_clusters = self.n_clusters
-        if hasattr(self._hierarchy_model, 'linkage'):
+        if hasattr(self._hierarchy_model, "linkage"):
             self._hierarchy_model.linkage = self.linkage
-        
+
         self._hierarchy_model.fit(V)
-        
+
         self._fitted = True
         return self
 
     def _similarity_matrix(self, X: Matrix) -> Matrix:
-        sq_dists = pdist(X, 'sqeuclidean')
+        sq_dists = pdist(X, "sqeuclidean")
         mat_sq_dists = squareform(sq_dists)
         return np.exp(-self.gamma * mat_sq_dists)
 
     def _laplacian(self, W: Matrix) -> Matrix:
         D = np.diag(np.sum(W, axis=1))
         return D - W
-    
-    def plot_dendrogram(self,
-                        ax: Optional[plt.Axes],
-                        hide_indices: bool = True, 
-                        show: bool = False) -> plt.Axes:
-        if not self.method == 'agglomerative':
+
+    def plot_dendrogram(
+        self, ax: Optional[plt.Axes], hide_indices: bool = True, show: bool = False
+    ) -> plt.Axes:
+        if not self.method == "agglomerative":
             raise UnsupportedParameterError(self.method)
-        
+
         return self._hierarchy_model.plot_dendrogram(ax, hide_indices, show)
 
     @property
     def labels(self) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         return self._hierarchy_model.labels
-    
+
     def predict(self) -> None:
         raise Warning(f"{type(self).__name__} does not support prediction!")
-    
+
     def score(self, metric: Evaluator = SilhouetteCoefficient) -> float:
         return metric.score(self._X, self.labels)
 
 
 class AdaptiveSpectralClustering(Estimator, Unsupervised):
-    
     """
-    Adaptive Spectral Clustering automatically determines the number of clusters 
-    and scale parameters directly from the data, reducing the need for manual 
-    tuning. It constructs a similarity matrix, typically using a Gaussian kernel 
-    with an adaptively chosen scale. Eigenvalue decomposition on the Laplacian of 
-    this matrix reveals the data's structure, and the eigen-gap heuristic is 
+    Adaptive Spectral Clustering automatically determines the number of clusters
+    and scale parameters directly from the data, reducing the need for manual
+    tuning. It constructs a similarity matrix, typically using a Gaussian kernel
+    with an adaptively chosen scale. Eigenvalue decomposition on the Laplacian of
+    this matrix reveals the data's structure, and the eigen-gap heuristic is
     employed to select the optimal number of clusters.
-    
+
     Parameters
     ----------
     `gamma` : Scaling factor for Gaussian kernel
     `max_clusters` : Upper-bound of the number of clusters to estimate
-    
+
     """
-    
-    def __init__(self, 
-                 gamma: float = 1.0,
-                 max_clusters: int = 10) -> None:
+
+    def __init__(self, gamma: float = 1.0, max_clusters: int = 10) -> None:
         self.gamma = gamma
         self.max_clusters = max_clusters
         self._X = None
         self._fitted = False
-    
-    def fit(self, X: Matrix) -> 'AdaptiveSpectralClustering':
+
+        self.set_param_ranges(
+            {"max_clusters": ("0<,+inf", int), "gamma": ("0<,+inf", None)}
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix) -> "AdaptiveSpectralClustering":
         self._X = X
         W = self._similarity_matrix(X)
         L = self._laplacian(W)
-        
+
         eigvals, eigvecs = eigh(L)
         self.n_clusters = self._optimal_clusters(eigvals)
-        
-        V = eigvecs[:, :self.n_clusters]
+
+        V = eigvecs[:, : self.n_clusters]
         kmeans = KMeansClusteringPlus(n_clusters=self.n_clusters)
         self.kmeans = kmeans.fit(V)
-        
+
         self.W = W
         self.L = L
         self._fitted = True
         return self
 
     def _similarity_matrix(self, X: Matrix) -> Matrix:
-        sq_dists = pdist(X, metric='sqeuclidean')
+        sq_dists = pdist(X, metric="sqeuclidean")
         mat_sq_dists = squareform(sq_dists)
         return np.exp(-self.gamma * mat_sq_dists)
-    
+
     def _laplacian(self, W: Matrix) -> Matrix:
         D = np.diag(np.sum(W, axis=0))
         return D - W
-    
+
     def _optimal_clusters(self, eigvals: Matrix) -> Matrix:
         eigval_diff = np.diff(eigvals)
-        return np.argmax(eigval_diff[:self.max_clusters]) + 1
-    
+        return np.argmax(eigval_diff[: self.max_clusters]) + 1
+
     @property
     def labels(self) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         return self.kmeans.labels
-    
+
     def predict(self) -> None:
         raise Warning(f"{type(self).__name__} does not support prediction!")
 
     def score(self, metric: Evaluator = SilhouetteCoefficient) -> float:
         return metric.score(self._X, self.labels)
-
```

### Comparing `luma-ml-0.6.4/luma/core/base.py` & `luma-ml-0.6.5/luma/core/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,143 +1,155 @@
-from typing import Any
+from typing import Any, Dict
 
 from luma.core.main import Luma
+from luma.interface.util import ParamRange
 
 
-__all__ = (
-    'ModelBase',
-    'ParadigmBase',
-    'MetricBase',
-    'VisualBase'
-)
+__all__ = ("ModelBase", "ParadigmBase", "MetricBase", "VisualBase")
 
 
 class ModelBase(Luma):
-    
     """
-    The ModelBase class serves as a superclass for core machine learning components 
-    involved in modeling and data transformation. It provides a foundational base 
-    for classes like Estimator and Transformer, encapsulating shared functionalities 
-    and properties essential for building, preparing, and processing machine 
-    learning models. This class is intended to streamline the development of 
-    machine learning pipelines by offering a unified interface for both model 
+    The ModelBase class serves as a superclass for core machine learning components
+    involved in modeling and data transformation. It provides a foundational base
+    for classes like Estimator and Transformer, encapsulating shared functionalities
+    and properties essential for building, preparing, and processing machine
+    learning models. This class is intended to streamline the development of
+    machine learning pipelines by offering a unified interface for both model
     creation and data preprocessing tasks.
-    
+
     Methods
     -------
     Train an estimator or a transformer for further use:
     ```py
         def fit(self, **kwargs) -> Any
     ```
-    
+
     Set the parameters of an estimator or a transformer:
     ```py
         def set_params(self, **kwargs) -> None
     ```
     This method iterates over the given keyword arguments and sets the
-    attributes of the instance accordingly. 
-    If an attribute corresponding to a given keyword does not exist, 
+    attributes of the instance accordingly.
+    If an attribute corresponding to a given keyword does not exist,
     a message is printed indicating that the attribute was not found.
-    
+
+    Notes
+    -----
+    Upon the call of `set_params`, the method `check_param_ranges` is
+    automatically called after resetting the parameters.
+
     Inheritances
     ------------
     `Estimator`, `Transformer`, `Optimizer`
-    
+
     """
-    
+
     def __validate__(self) -> None:
         return super().__validate__()
-    
+
     def __alloc__(self, *args, **kwargs) -> None:
         return super().__alloc__(*args, **kwargs)
-    
+
     def __dealloc__(self) -> None:
         return super().__dealloc__()
-    
-    def fit(self, **kwargs) -> Any: kwargs
-    
+
+    def fit(self, **kwargs) -> Any:
+        kwargs
+
     def set_params(self, **kwargs) -> None:
         for key, val in kwargs.items():
             if hasattr(self, key):
                 setattr(self, key, val)
             else:
                 print(f"'{type(self).__name__}' has no attribute '{key}'")
+        self.check_param_ranges()
+
+    def set_param_ranges(self, range_dict: Dict[str, tuple]) -> None:
+        self._param_range_dict = {
+            name_: ParamRange(range_, type_)
+            for name_, (range_, type_) in range_dict.items()
+        }
+
+    def check_param_ranges(self) -> None:
+        if not hasattr(self, "_param_range_dict"):
+            return
+        for name, val in self.__dict__.items():
+            if name not in self._param_range_dict:
+                continue
+            self._param_range_dict[name].check(param_name=name, param_value=val)
 
 
 class ParadigmBase(Luma):
-    
     """
-    The ParadigmBase class is a superclass for different learning paradigms in 
-    machine learning, such as Supervised and Unsupervised learning. This class 
-    offers a common base for various types of learning approaches, providing a 
-    standardized interface and shared properties relevant to different learning 
-    methodologies. It helps in categorizing and organizing machine learning 
-    models based on their learning strategy, facilitating the development and 
+    The ParadigmBase class is a superclass for different learning paradigms in
+    machine learning, such as Supervised and Unsupervised learning. This class
+    offers a common base for various types of learning approaches, providing a
+    standardized interface and shared properties relevant to different learning
+    methodologies. It helps in categorizing and organizing machine learning
+    models based on their learning strategy, facilitating the development and
     usage of models tailored to specific types of data and tasks.
-    
+
     Inheritances
     ------------
     `Supervised`, `Unsupervised`
 
     """
-    
+
     def __validate__(self) -> None:
         return super().__validate__()
-    
+
     def __alloc__(self, *args, **kwargs) -> None:
         return super().__alloc__(*args, **kwargs)
-    
+
     def __dealloc__(self) -> None:
         return super().__dealloc__()
 
 
 class MetricBase(Luma):
-    
     """
-    The MetricBase class serves as a superclass for evaluation metrics measures 
-    used in machine learning. It focuses on quantitative measures to assess model 
-    performance and compute similarities or differences. This class provides a 
-    unified base for various types of evaluation methods and other metric calculations, 
-    which are essential for effectively measuring and comparing the efficacy of 
+    The MetricBase class serves as a superclass for evaluation metrics measures
+    used in machine learning. It focuses on quantitative measures to assess model
+    performance and compute similarities or differences. This class provides a
+    unified base for various types of evaluation methods and other metric calculations,
+    which are essential for effectively measuring and comparing the efficacy of
     machine learning models and for analyzing data characteristics.
-    
+
     Inheritances
     ------------
     `Evaluator`, `Distance`
-    
+
     """
-    
+
     def __validate__(self) -> None:
         return super().__validate__()
-    
+
     def __alloc__(self, *args, **kwargs) -> None:
         return super().__alloc__(*args, **kwargs)
-    
+
     def __dealloc__(self) -> None:
         return super().__dealloc__()
 
 
 class VisualBase(Luma):
-    
     """
-    The VisualBase class is a superclass for visualization tools in machine 
-    learning. This class offers a common framework for visualizing different 
-    aspects of machine learning models, datasets, and analysis results. It plays 
-    a crucial role in simplifying the interpretation and understanding of complex 
-    machine learning processes, helping users to gain insights into model behavior, 
+    The VisualBase class is a superclass for visualization tools in machine
+    learning. This class offers a common framework for visualizing different
+    aspects of machine learning models, datasets, and analysis results. It plays
+    a crucial role in simplifying the interpretation and understanding of complex
+    machine learning processes, helping users to gain insights into model behavior,
     data patterns, and performance metrics through intuitive visual representations.
-    
+
     Inheritances
     ------------
     `Visualizer`
-    
+
     """
-    
+
     def __validate__(self) -> None:
         return super().__validate__()
-    
+
     def __alloc__(self, *args, **kwargs) -> None:
         return super().__alloc__(*args, **kwargs)
-    
+
     def __dealloc__(self) -> None:
         return super().__dealloc__()
-
```

### Comparing `luma-ml-0.6.4/luma/core/super.py` & `luma-ml-0.6.5/luma/core/super.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,338 +1,346 @@
-from typing import Any
-from abc import (ABCMeta, 
-                 abstractmethod, 
-                 abstractstaticmethod)
+from typing import Any, Dict
+from abc import ABCMeta, abstractmethod, abstractstaticmethod
 
 from luma.core.base import *
 
 
 __all__ = (
-    'Estimator', 
-    'Transformer', 
-    'Optimizer',
-    'Evaluator', 
-    'Visualizer', 
-    'Supervised', 
-    'Unsupervised', 
-    'Distance'
+    "Estimator",
+    "Transformer",
+    "Optimizer",
+    "Evaluator",
+    "Visualizer",
+    "Supervised",
+    "Unsupervised",
+    "Distance",
 )
 
 
 class Estimator(ModelBase, metaclass=ABCMeta):
-    
     """
-    An estimator is a mathematical model or algorithm 
-    used to make predictions or estimates based on data. 
-    It takes input data and learns from it to generate output predictions, 
-    typically for tasks like classification or regression. 
-    Estimators can be as simple as linear regression or as complex as 
-    deep neural networks, and their goal is to capture patterns and 
+    An estimator is a mathematical model or algorithm
+    used to make predictions or estimates based on data.
+    It takes input data and learns from it to generate output predictions,
+    typically for tasks like classification or regression.
+    Estimators can be as simple as linear regression or as complex as
+    deep neural networks, and their goal is to capture patterns and
     relationships within the data to make accurate predictions on new, unseen data.
-    
+
     Methods
     -------
     For training:
-    ```py 
+    ```py
         @abstractmethod
         def fit(self, *args) -> Estimator
     ```
-    
+
     For prediction:
     ```py
         @abstractmethod
         def predict(self, *args) -> Vector
     ```
-    
+
     For scoring
     ```py
         @abstractmethod
         def score(self, *args) -> float
     ```
-    
+
     For setting parameters when tuning
     ```py
         def set_params(self, *args) -> None
     ```
     """
-    
+
     class Meta:
-        
         """
         An inner class of `Estimator` for meta-estimator.
-        
-        A meta-estimator is a type of estimator in machine learning that 
-        combines or extends other estimators to improve performance or 
+
+        A meta-estimator is a type of estimator in machine learning that
+        combines or extends other estimators to improve performance or
         functionality, such as ensemble methods or pipelines.
         """
-    
+
     class TimeSeries:
-        
         """
         An inner class of `Estimator` dedicated to time series analysis.
-        
-        Time series analysis encompasses methods for analyzing time series 
-        data to extract meaningful statistics and characteristics. The 
-        `TimeSeries` class is specialized for handling and modeling 
-        time-dependent data, with a focus on identifying patterns, forecasting 
-        future values, and analyzing temporal dynamics. It serves as a base 
-        for models designed to work with ordered, time-stamped data, providing 
+
+        Time series analysis encompasses methods for analyzing time series
+        data to extract meaningful statistics and characteristics. The
+        `TimeSeries` class is specialized for handling and modeling
+        time-dependent data, with a focus on identifying patterns, forecasting
+        future values, and analyzing temporal dynamics. It serves as a base
+        for models designed to work with ordered, time-stamped data, providing
         functionalities tailored to the unique needs of time series forecasting.
-        
+
         Notes
         -----
-        - Classes under `TimeSeries` are specifically designed for time 
-          series data and may not be directly compatible with classes 
-          under `Meta`, which are aimed at enhancing or combining 
-          estimators for improved performance or functionality. When 
-          integrating `TimeSeries` models with `Meta` estimators, 
-          special consideration is needed to ensure compatibility and 
+        - Classes under `TimeSeries` are specifically designed for time
+          series data and may not be directly compatible with classes
+          under `Meta`, which are aimed at enhancing or combining
+          estimators for improved performance or functionality. When
+          integrating `TimeSeries` models with `Meta` estimators,
+          special consideration is needed to ensure compatibility and
           effective integration.
-        
+
         """
-    
+
     @abstractmethod
-    def fit(self, *args) -> 'Estimator': ...
-    
+    def fit(self, *args) -> "Estimator": ...
+
     @abstractmethod
     def predict(self, *args) -> Any: ...
-    
+
     @abstractmethod
     def score(self, *args) -> float: ...
-    
+
     def set_params(self, **kwargs) -> None:
         return super().set_params(**kwargs)
 
+    def set_param_ranges(self, range_dict: Dict[str, tuple]) -> None:
+        return super().set_param_ranges(range_dict)
+
+    def check_param_ranges(self) -> None:
+        return super().check_param_ranges()
+
 
 class Transformer(ModelBase, metaclass=ABCMeta):
-    
     """
-    A transformer (preprocessor) is a component or set of operations used to 
-    prepare and clean raw data before it is fed into a machine learning model. 
-    Preprocessing tasks can include data normalization, handling missing values, 
-    feature scaling, one-hot encoding, and more. 
-    The goal of a preprocessor is to make the data suitable for the specific 
-    machine learning algorithm being used, enhancing the model's performance 
-    by ensuring the data is in the right format and is free from inconsistencies 
+    A transformer (preprocessor) is a component or set of operations used to
+    prepare and clean raw data before it is fed into a machine learning model.
+    Preprocessing tasks can include data normalization, handling missing values,
+    feature scaling, one-hot encoding, and more.
+    The goal of a preprocessor is to make the data suitable for the specific
+    machine learning algorithm being used, enhancing the model's performance
+    by ensuring the data is in the right format and is free from inconsistencies
     or noise.
-    
+
     Methods
     -------
     For fitting:
     ```py
         @abstractmethod
         def fit(self, *args) -> Transformer
     ```
-    
+
     For transformation:
     ```py
         @abstractmethod
         def transform(self, *args) -> Matrix
     ```
-    
+
     For fitting and transformation at once:
     ```py
         @abstractmethod
         def fit_transform(self, *args) -> Matrix
     ```
-    
+
     For setting parameters when tuning:
     ```py
         def set_params(self, *args) -> None
     ```
     """
-    
-    class Feature: 
-        
+
+    class Feature:
         """
-        An inner class of `Transformer` dedicated to the processing and 
+        An inner class of `Transformer` dedicated to the processing and
         handling of feature data in a dataset.
-        
+
         Default class for uninherited models.
-        
+
         * `fit` method only gets parameter: `X`
-        
+
             ```py
             def fit(self, X: Matrix) -> Transformer
             ```
         * `transform` method only gets `X` and returns transformed `X`
-        
+
             ```py
             def transform(self, X: Matrix) -> Matrix
             ```
         """
-        
+
     class Target:
-        
         """
-        An inner class of `Transformer` dedicated to the processing and 
+        An inner class of `Transformer` dedicated to the processing and
         handling of target data in a dataset.
-        
+
         * `fit` method only gets parameter: `y`
 
             ```py
             def fit(self, y: Vector) -> Transformer
             ```
         * `transform` method only gets `y` and returns transformed `y`
-        
+
             ```py
             def transform(self, y: Vector) -> Matrix | Vector
             ```
         """
-         
-    class Both: 
-        
+
+    class Both:
         """
-        An inner class of `Transformer` dedicated to the processing and 
+        An inner class of `Transformer` dedicated to the processing and
         handling of both feature and target data in a dataset.
-        
+
         * `fit` method gets two parameters: `X`, `y`
-        
+
             ```py
             def fit(self, X: Matrix, y: Vector) -> Transformer
             ```
             To ignore `y`, replace with placeholder `_`:
             ```py
             def fit(self, X: Matrix, _ = None) -> Transformer
             ```
         * `transform` method gets `X` and `y` and returns transformed `X` and `y`
-        
+
             ```py
             def transform(self, X: Matrix, y: Vector) -> Tuple[Matrix, Matrix | Vector]
             ```
         """
-    
+
     @abstractmethod
-    def fit(self, *args) -> 'Transformer': ...
-    
+    def fit(self, *args) -> "Transformer": ...
+
     @abstractmethod
     def transform(self, *args) -> Any: ...
-    
+
     @abstractmethod
     def fit_transform(self, *args) -> Any: ...
-    
+
     def set_params(self, **kwargs) -> None:
         return super().set_params(**kwargs)
 
+    def set_param_ranges(self, range_dict: Dict[str, tuple]) -> None:
+        return super().set_param_ranges(range_dict)
+
+    def check_param_ranges(self) -> None:
+        return super().check_param_ranges()
+
 
 class Optimizer(ModelBase, metaclass=ABCMeta):
-    
     """
-    The Optimizer class serves as a superclass for optimization techniques in 
-    the luma module, focusing on hyperparameter tuning and model optimization. 
-    This class inherits from ModelBase, indicating its role in enhancing and 
-    fine-tuning machine learning models. It provides an abstract base for 
-    different optimization strategies, offering a standardized interface for 
-    systematically exploring and evaluating different combinations of model 
+    The Optimizer class serves as a superclass for optimization techniques in
+    the luma module, focusing on hyperparameter tuning and model optimization.
+    This class inherits from ModelBase, indicating its role in enhancing and
+    fine-tuning machine learning models. It provides an abstract base for
+    different optimization strategies, offering a standardized interface for
+    systematically exploring and evaluating different combinations of model
     parameters.
-    
+
     Properties
     ----------
     Get the best(optimized) estimator or transformer:
     ```py
         @property
         def best_model(self) -> Estimator | Transformer
-    
+
     """
-    
+
     @property
     def best_model(self) -> Estimator | Transformer: ...
+    
+    def fit(self, **kwargs) -> Any:
+        return super().fit(**kwargs)
+
+    def set_params(self, **kwargs) -> None:
+        return super().set_params(**kwargs)
+
+    def set_param_ranges(self, range_dict: Dict[str, tuple]) -> None:
+        return super().set_param_ranges(range_dict)
+
+    def check_param_ranges(self) -> None:
+        return super().check_param_ranges()
 
 
 class Evaluator(MetricBase, metaclass=ABCMeta):
-    
     """
-    Evaluators, a.k.a. metrics are quantitative measures used to assess the performance 
-    and effectiveness of a machine learning model. These metrics provide insights into 
-    how well a model is performing on a particular task, 
-    such as classification or regression. 
-    
+    Evaluators, a.k.a. metrics are quantitative measures used to assess the performance
+    and effectiveness of a machine learning model. These metrics provide insights into
+    how well a model is performing on a particular task,
+    such as classification or regression.
+
     Methods
     -------
     For scoring:
     ```py
         @abstractstaticmethod
         def score(*args) -> float
     ```
     """
-    
+
     @abstractstaticmethod
     def score(*args) -> float: ...
 
 
 class Visualizer(VisualBase, metaclass=ABCMeta):
-    
     """
-    A visualizer is a tool that helps visualize and understand various aspects 
-    of machine learning models, datasets, and the results the analysis. 
-    Visualizers play a crucial role in simplifying the interpretation of complex 
+    A visualizer is a tool that helps visualize and understand various aspects
+    of machine learning models, datasets, and the results the analysis.
+    Visualizers play a crucial role in simplifying the interpretation of complex
     machine learning processes and results.
-    
+
     Methods
     -------
     For plotting:
     ```py
         @abstractmethod
         def plot(self, *args) -> None
     ```
     """
-    
+
     @abstractmethod
     def plot(self, *args) -> None: ...
 
 
 class Supervised(ParadigmBase):
-    
     """
-    Supervised learning is a type of machine learning where the algorithm learns 
-    to make predictions or decisions by training on a labeled dataset. 
-    In this approach, the algorithm is provided with input data and corresponding 
-    target labels, and it learns to map the inputs to the correct outputs. 
+    Supervised learning is a type of machine learning where the algorithm learns
+    to make predictions or decisions by training on a labeled dataset.
+    In this approach, the algorithm is provided with input data and corresponding
+    target labels, and it learns to map the inputs to the correct outputs.
     """
-    
+
     def __init__(self, *args) -> None: ...
 
 
 class Unsupervised(ParadigmBase):
-    
     """
-    Unsupervised learning is a machine learning paradigm where the algorithm 
-    is given input data without explicit target labels. Instead of making predictions, 
-    the algorithm's goal is to discover hidden patterns, structures, 
+    Unsupervised learning is a machine learning paradigm where the algorithm
+    is given input data without explicit target labels. Instead of making predictions,
+    the algorithm's goal is to discover hidden patterns, structures,
     or relationships within the data.
-    
+
     Default class for uninherited models.
-    
+
     Properties
     ----------
     Get assigned labels:
     ```py
         @property
         def labels(self) -> Vector
     ```
     """
-    
+
     def __init__(self, *args) -> None: ...
-    
+
     @property
-    def labels(self) -> Any:...
+    def labels(self) -> Any: ...
 
 
 class Distance(MetricBase, metaclass=ABCMeta):
-    
     """
-    In mathematics and machine learning, distance is a measure of how much "separation" 
-    or "difference" there is between two points, objects, or distributions. Different 
+    In mathematics and machine learning, distance is a measure of how much "separation"
+    or "difference" there is between two points, objects, or distributions. Different
     types of distances serve various purposes, and they are used in different contexts.
-    
+
     Methods
     -------
     For computing the distance:
     ```py
         @abstractstaticmethod
         def compute(*args) -> float
     ```
     """
-    
+
     @abstractstaticmethod
     def compute(*args) -> float: ...
-
```

### Comparing `luma-ml-0.6.4/luma/ensemble/bagging.py` & `luma-ml-0.6.5/luma/ensemble/bagging.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,237 +6,260 @@
 from luma.interface.exception import NotFittedError
 from luma.classifier.tree import DecisionTreeClassifier
 from luma.regressor.tree import DecisionTreeRegressor
 from luma.metric.classification import Accuracy
 from luma.metric.regression import MeanSquaredError
 
 
-__all__ = (
-    'BaggingClassifier',
-    'BaggingRegressor'
-)
+__all__ = ("BaggingClassifier", "BaggingRegressor")
 
 
 class BaggingClassifier(Estimator, Estimator.Meta, Supervised):
-    
     """
-    A Bagging Classifier is an ensemble learning technique that trains 
-    multiple base models, typically decision trees, on random subsets 
-    of the original dataset. Each model is trained on a bootstrap sample 
-    (random sample with replacement) of the data, potentially using a 
-    random subset of features. The final prediction is made by aggregating 
-    the predictions of all models, typically through voting for 
-    classification or averaging for regression. This approach reduces 
+    A Bagging Classifier is an ensemble learning technique that trains
+    multiple base models, typically decision trees, on random subsets
+    of the original dataset. Each model is trained on a bootstrap sample
+    (random sample with replacement) of the data, potentially using a
+    random subset of features. The final prediction is made by aggregating
+    the predictions of all models, typically through voting for
+    classification or averaging for regression. This approach reduces
     variance, improves model stability, and can prevent overfitting.
-    
+
     Parameters
     ----------
     `base_estimator` : Base estimator for training multiple models
     (Default `DecisionTreeClassifier`)
     `n_estimators` : Number of base estimators to fit
     `max_samples` : Maximum number of data to sample (`0~1` proportion)
     `max_features` : Maximum number of features to sample (`0~1` proporton)
     `bootstrap` : Whether to bootstrap data samples
     `bootstrap_feature`: Whether to bootstrap features
     `random_state` : Seed for random sampling
     `**kwargs` : Additional parameters for base estimator (i.e. `max_depth`)
-    
+
     Examples
     --------
     >>> bag = BaggingClassifier(base_estimator=AnyEstimator(),
                                 n_estimators=100,
                                 max_samples=1.0,
                                 max_features=1.0,
                                 bootstrap=True,
                                 bootstrap_feature=False)
     >>> bag.fit(X, y)
     >>> y_pred = bag.predict(X)
     >>> est = bag[i] # Get i-th base estimator from `bag`
-    
+
     """
-    
-    def __init__(self, 
-                 base_estimator: Estimator = DecisionTreeClassifier(),
-                 n_estimators: int = 50,
-                 max_samples: float | int = 1.0,
-                 max_features: float | int = 1.0,
-                 bootstrap: bool = True,
-                 bootstrap_feature: bool = False,
-                 random_state: int = None,
-                 verbose: bool = False,
-                 **kwargs: Dict[str, Any]) -> None:
+
+    def __init__(
+        self,
+        base_estimator: Estimator = DecisionTreeClassifier(),
+        n_estimators: int = 50,
+        max_samples: float | int = 1.0,
+        max_features: float | int = 1.0,
+        bootstrap: bool = True,
+        bootstrap_feature: bool = False,
+        random_state: int = None,
+        verbose: bool = False,
+        **kwargs: Dict[str, Any],
+    ) -> None:
         self.base_estimator = base_estimator
         self.n_estimators = n_estimators
         self.max_samples = max_samples
         self.max_features = max_features
         self.bootstrap = bootstrap
         self.bootstrap_feature = bootstrap_feature
         self.random_state = random_state
         self.verbose = verbose
         self._base_estimator_params = kwargs
         self._fitted = False
-    
-    def fit(self, X: Matrix, y: Vector) -> 'BaggingClassifier':
+
+        self.set_param_ranges({"n_estimators": ("0<,+inf", int)})
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix, y: Vector) -> "BaggingClassifier":
         np.random.seed(self.random_state)
         self.base_estimator.set_params(**self._base_estimator_params)
         self.estimators_ = []
-        
+
         m, n = X.shape
-        if self.max_samples <= 1.0: max_samples = int(m * self.max_samples)
-        else: max_samples = self.max_samples
-        
-        if self.max_features <= 1.0: max_features = int(n * self.max_features)
-        else: max_features = self.max_features
-        
+        if self.max_samples <= 1.0:
+            max_samples = int(m * self.max_samples)
+        else:
+            max_samples = self.max_samples
+
+        if self.max_features <= 1.0:
+            max_features = int(n * self.max_features)
+        else:
+            max_features = self.max_features
+
         for i in range(self.n_estimators):
             s_indices = np.random.choice(m, max_samples, self.bootstrap)
             f_indices = np.random.choice(n, max_features, self.bootstrap_feature)
-            
+
             X_sample = X[s_indices][:, f_indices]
             y_sample = y[s_indices]
-            
+
             estimator = Clone(self.base_estimator).get
             estimator.fit(X_sample, y_sample)
             self.estimators_.append((estimator, f_indices))
-            
+
             if self.verbose:
-                print(f'[Bagging] Finished fitting',
-                      f'{type(self.base_estimator).__name__}',
-                      f'{i + 1}/{self.n_estimators}')
-        
+                print(
+                    f"[Bagging] Finished fitting",
+                    f"{type(self.base_estimator).__name__}",
+                    f"{i + 1}/{self.n_estimators}",
+                )
+
         self._fitted = True
         return self
-    
+
     def predict(self, X: Matrix) -> Vector:
-        if not self._fitted: raise NotFittedError(self)
-        
+        if not self._fitted:
+            raise NotFittedError(self)
+
         predictions = []
         for i, (estimator, f_indices) in enumerate(self.estimators_):
             predictions.append(estimator.predict(X[:, f_indices]))
             if self.verbose:
-                print(f'[Bagging] Finished prediction of',
-                      f'{type(self.base_estimator).__name__}',
-                      f'{i + 1}/{self.n_estimators}')
-        
+                print(
+                    f"[Bagging] Finished prediction of",
+                    f"{type(self.base_estimator).__name__}",
+                    f"{i + 1}/{self.n_estimators}",
+                )
+
         majority_vote = np.apply_along_axis(
             lambda x: np.bincount(x, minlength=len(np.unique(x))).argmax(),
             axis=0,
-            arr=predictions
+            arr=predictions,
         )
         return majority_vote
-    
+
     def score(self, X: Matrix, y: Vector, metric: Evaluator = Accuracy) -> float:
         X_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=X_pred)
-    
+
     def __getitem__(self, index: int) -> Estimator:
         return self.estimators_[index]
 
 
 class BaggingRegressor(Estimator, Estimator.Meta, Supervised):
-    
     """
-    A Bagging Regressor is an ensemble meta-estimator that fits base 
-    regressors each on random subsets of the original dataset and then 
-    averages their predictions to form the final prediction. It aims to 
-    improve the stability and accuracy of machine learning algorithms, 
+    A Bagging Regressor is an ensemble meta-estimator that fits base
+    regressors each on random subsets of the original dataset and then
+    averages their predictions to form the final prediction. It aims to
+    improve the stability and accuracy of machine learning algorithms,
     especially overfitting in decision trees or other similar models.
-    
+
     Parameters
     ----------
     `base_estimator` : Base estimator for training multiple models
     (Default `DecisionTreeRegressor`)
     `n_estimators` : Number of base estimators to fit
     `max_samples` : Maximum number of data to sample (`0~1` proportion)
     `max_features` : Maximum number of features to sample (`0~1` proporton)
     `bootstrap` : Whether to bootstrap data samples
     `bootstrap_feature`: Whether to bootstrap features
     `random_state` : Seed for random sampling
     `**kwargs` : Additional parameters for base estimator (i.e. `max_depth`)
-    
+
     Examples
     --------
     >>> bag = BaggingRegressor(base_estimator=AnyEstimator(),
                                n_estimators=100,
                                max_samples=1.0,
                                max_features=1.0,
                                bootstrap=True,
                                bootstrap_feature=False)
     >>> bag.fit(X, y)
     >>> y_pred = bag.predict(X)
     >>> est = bag[i] # Get i-th base estimator from `bag`
-    
+
     """
-    
-    def __init__(self, 
-                 base_estimator: Estimator = DecisionTreeRegressor(),
-                 n_estimators: int = 50,
-                 max_samples: float | int = 1.0,
-                 max_features: float | int = 1.0,
-                 bootstrap: bool = True,
-                 bootstrap_feature: bool = False,
-                 random_state: int = None,
-                 verbose: bool = False,
-                 **kwargs: Dict[str, Any]) -> None:
+
+    def __init__(
+        self,
+        base_estimator: Estimator = DecisionTreeRegressor(),
+        n_estimators: int = 50,
+        max_samples: float | int = 1.0,
+        max_features: float | int = 1.0,
+        bootstrap: bool = True,
+        bootstrap_feature: bool = False,
+        random_state: int = None,
+        verbose: bool = False,
+        **kwargs: Dict[str, Any],
+    ) -> None:
         self.base_estimator = base_estimator
         self.n_estimators = n_estimators
         self.max_samples = max_samples
         self.max_features = max_features
         self.bootstrap = bootstrap
         self.bootstrap_feature = bootstrap_feature
         self.random_state = random_state
         self.verbose = verbose
         self._base_estimator_params = kwargs
         self._fitted = False
-    
-    def fit(self, X: Matrix, y: Vector) -> 'BaggingRegressor':
+
+        self.set_param_ranges({"n_estimators": ("0<,+inf", int)})
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix, y: Vector) -> "BaggingRegressor":
         np.random.seed(self.random_state)
         self.base_estimator.set_params(**self._base_estimator_params)
         self.estimators_ = []
-        
+
         m, n = X.shape
-        if self.max_samples <= 1.0: max_samples = int(m * self.max_samples)
-        else: max_samples = self.max_samples
-        
-        if self.max_features <= 1.0: max_features = int(n * self.max_features)
-        else: max_features = self.max_features
-        
+        if self.max_samples <= 1.0:
+            max_samples = int(m * self.max_samples)
+        else:
+            max_samples = self.max_samples
+
+        if self.max_features <= 1.0:
+            max_features = int(n * self.max_features)
+        else:
+            max_features = self.max_features
+
         for i in range(self.n_estimators):
             s_indices = np.random.choice(m, max_samples, self.bootstrap)
             f_indices = np.random.choice(n, max_features, self.bootstrap_feature)
-            
+
             X_sample = X[s_indices][:, f_indices]
             y_sample = y[s_indices]
-            
+
             estimator = Clone(self.base_estimator).get
             estimator.fit(X_sample, y_sample)
             self.estimators_.append((estimator, f_indices))
-            
+
             if self.verbose:
-                print(f'[Bagging] Finished fitting',
-                      f'{type(self.base_estimator).__name__}',
-                      f'{i + 1}/{self.n_estimators}')
-        
+                print(
+                    f"[Bagging] Finished fitting",
+                    f"{type(self.base_estimator).__name__}",
+                    f"{i + 1}/{self.n_estimators}",
+                )
+
         self._fitted = True
         return self
-    
+
     def predict(self, X: Matrix) -> Vector:
-        if not self._fitted: raise NotFittedError(self)
-        
+        if not self._fitted:
+            raise NotFittedError(self)
+
         predictions = []
         for i, (estimator, f_indices) in enumerate(self.estimators_):
             predictions.append(estimator.predict(X[:, f_indices]))
             if self.verbose:
-                print(f'[Bagging] Finished prediction of',
-                      f'{type(self.base_estimator).__name__}',
-                      f'{i + 1}/{self.n_estimators}')
-        
+                print(
+                    f"[Bagging] Finished prediction of",
+                    f"{type(self.base_estimator).__name__}",
+                    f"{i + 1}/{self.n_estimators}",
+                )
+
         return np.mean(predictions, axis=0)
-    
-    def score(self, X: Matrix, y: Vector, 
-              metric: Evaluator = MeanSquaredError) -> float:
+
+    def score(
+        self, X: Matrix, y: Vector, metric: Evaluator = MeanSquaredError
+    ) -> float:
         X_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=X_pred)
-    
+
     def __getitem__(self, index: int) -> Estimator:
         return self.estimators_[index]
-
```

### Comparing `luma-ml-0.6.4/luma/ensemble/boost.py` & `luma-ml-0.6.5/luma/ensemble/boost.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,147 +9,159 @@
 from luma.regressor.tree import DecisionTreeRegressor
 from luma.preprocessing.encoder import LabelBinarizer
 from luma.metric.classification import Accuracy
 from luma.metric.regression import MeanSquaredError
 
 
 __all__ = (
-    'AdaBoostClassifier',
-    'AdaBoostRegressor',
-    'GradientBoostingClassifier',
-    'GradientBoostingRegressor'
+    "AdaBoostClassifier",
+    "AdaBoostRegressor",
+    "GradientBoostingClassifier",
+    "GradientBoostingRegressor",
 )
 
 
 class AdaBoostClassifier(Estimator, Estimator.Meta, Supervised):
-    
     """
-    The AdaBoost classifier is an ensemble method that combines multiple 
-    weak learners, typically decision trees, to form a strong classifier. 
-    During training, it iteratively adjusts the weights of misclassified 
-    instances, making them more likely to be correctly predicted in subsequent 
-    rounds. Each weak learner's contribution to the final prediction is 
-    weighted based on its accuracy. AdaBoost is adaptive in the sense that 
-    subsequent weak learners are tweaked in favor of instances that previous 
-    learners misclassified. The final model makes preds based on the 
+    The AdaBoost classifier is an ensemble method that combines multiple
+    weak learners, typically decision trees, to form a strong classifier.
+    During training, it iteratively adjusts the weights of misclassified
+    instances, making them more likely to be correctly predicted in subsequent
+    rounds. Each weak learner's contribution to the final prediction is
+    weighted based on its accuracy. AdaBoost is adaptive in the sense that
+    subsequent weak learners are tweaked in favor of instances that previous
+    learners misclassified. The final model makes preds based on the
     weighted majority vote of its weak learners.
-    
+
     Parameters
     ----------
     `base_estimator` : Base est for training multiple models
     (Default `DecisionTreeClassifier`)
     `n_estimators` : Number of base estimators to fit
     `learning_rate` : Step size of class weights(`alpha`) update
     `**kwargs` : Additional parameters for base est (i.e. `max_depth`)
-    
+
     Examples
     --------
     >>> ada_est = AdaBoostClassifier(learning_rate=1.0, ...)
     >>> ada_est.fit(X, y)
-    
+
     >>> y_pred = ada_est.predict(X)
     >>> est = ada_est[i] # Get i-th est from `ada_est`
-    
+
     """
-    
-    def __init__(self, 
-                 base_estimator: Estimator = DecisionTreeClassifier(),
-                 n_estimators: int = 50, 
-                 learning_rate: float = 1.0,
-                 verbose: bool = False,
-                 **kwargs: Dict[str, Any]) -> None:
+
+    def __init__(
+        self,
+        base_estimator: Estimator = DecisionTreeClassifier(),
+        n_estimators: int = 50,
+        learning_rate: float = 1.0,
+        verbose: bool = False,
+        **kwargs: Dict[str, Any],
+    ) -> None:
         self.base_estimator = base_estimator
         self.n_estimators = n_estimators
         self.learning_rate = learning_rate
         self.verbose = verbose
         self.classes_ = None
         self.estimators_: List[Estimator] = []
         self.estimator_weights_: List[float] = []
         self.estimator_errors_: List[float] = []
         self._base_estimator_params = kwargs
         self._fitted = False
 
-    def fit(self, X: Matrix, y: Matrix) -> 'AdaBoostClassifier':
+        self.set_param_ranges(
+            {"n_estimators": ("0<,+inf", int), "learning_rate": ("0<,+inf", None)}
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix, y: Matrix) -> "AdaBoostClassifier":
         self.classes_ = np.unique(y)
-        
+
         m, _ = X.shape
         n_classes = len(self.classes_)
         sample_weights = np.ones(m)
-        
+
         lb = LabelBinarizer().fit(self.classes_)
         y_bin = lb.transform(y)
 
         for i in range(self.n_estimators):
             est = Clone(self.base_estimator).get
-            if hasattr(est, 'max_depth'): est.max_depth = 3
-            
+            if hasattr(est, "max_depth"):
+                est.max_depth = 3
+
             est.set_params(**self._base_estimator_params)
             est.fit(X, y, sample_weights=sample_weights)
             y_pred = est.predict(X)
             y_pred_bin = lb.transform(y_pred)
 
             error_vect = np.sum(y_bin != y_pred_bin, axis=1) / (n_classes - 1)
             error = np.sum(sample_weights * error_vect) / np.sum(sample_weights)
             error = max(error, 1e-10)
-            if error >= (n_classes - 1) / n_classes: continue
+            if error >= (n_classes - 1) / n_classes:
+                continue
 
             alpha = self.learning_rate * np.log((1 - error) / error)
             sample_weights *= np.exp(alpha * error_vect)
             sample_weights /= np.sum(sample_weights)
 
             self.estimators_.append(est)
             self.estimator_weights_.append(alpha)
             self.estimator_errors_.append(error)
-            
+
             if self.verbose:
-                print(f'[AdaBoost] Finished fitting {type(est).__name__}',
-                      f'{i + 1}/{self.n_estimators} with',
-                      f'error: {error}, alpha: {alpha}')
+                print(
+                    f"[AdaBoost] Finished fitting {type(est).__name__}",
+                    f"{i + 1}/{self.n_estimators} with",
+                    f"error: {error}, alpha: {alpha}",
+                )
 
         self._fitted = True
         return self
 
     def predict(self, X: Matrix) -> Vector:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         m, _ = X.shape
         est_preds = Matrix([est.predict(X) for est in self.estimators_])
         weighted_preds = np.zeros((m, len(self.classes_)))
-        
+
         for i, est_pred in enumerate(est_preds):
             for j in range(m):
                 cl = np.where(self.classes_ == est_pred[j])[0][0]
                 weighted_preds[j, cl] += self.estimator_weights_[i]
-            
+
             if self.verbose:
-                print(f'[AdaBoost] Finished prediction of',
-                      f'{type(self.base_estimator).__name__}',
-                      f'{i + 1}/{self.n_estimators}')
-        
+                print(
+                    f"[AdaBoost] Finished prediction of",
+                    f"{type(self.base_estimator).__name__}",
+                    f"{i + 1}/{self.n_estimators}",
+                )
+
         return self.classes_[np.argmax(weighted_preds, axis=1)]
 
     def score(self, X: Matrix, y: Vector, metric: Evaluator = Accuracy) -> float:
         X_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=X_pred)
 
     def __getitem__(self, index: int) -> Estimator:
         return self.estimators_[index]
 
 
 class AdaBoostRegressor(Estimator, Estimator.Meta, Supervised):
-    
     """
-    The AdaBoost regressor is an ensemble method that combines multiple 
-    weak learners, typically decision trees, to form a strong regressor. 
-    During training, it focuses on reducing the errors of the ensemble by 
-    adjusting the sample weights and fitting each weak learner to the 
-    residual errors of the previous learners. The final output is a 
-    combination of the weak learners' outputs, weighted by their individual 
-    contributions to the ensemble's performance, which aims to produce 
+    The AdaBoost regressor is an ensemble method that combines multiple
+    weak learners, typically decision trees, to form a strong regressor.
+    During training, it focuses on reducing the errors of the ensemble by
+    adjusting the sample weights and fitting each weak learner to the
+    residual errors of the previous learners. The final output is a
+    combination of the weak learners' outputs, weighted by their individual
+    contributions to the ensemble's performance, which aims to produce
     a more accurate regression model.
-    
+
     Parameters
     ----------
     `base_estimator` : Base est for training multiple models
     (Default `DecisionTreeRegressor`)
     `n_estimators` : Number of base estimators to fit
     `learning_rate` : Step size of class weights(`alpha`) update
     `loss` : Type of loss function (e.g. `linear`, `square`, `exp`)
@@ -160,318 +172,362 @@
     >>> ada_reg = AdaBoostRegressor(learning_rate=1.0, ...)
     >>> ada_reg.fit(X_train, y_train)
 
     >>> y_pred = ada_reg.predict(X_test)
     >>> est = ada_reg[i] # Get the i-th est from the `ada_reg`
 
     """
-    
-    def __init__(self, 
-                 base_estimator: Estimator = DecisionTreeRegressor(),
-                 n_estimators: int = 50,
-                 learning_rate: float = 1.0,
-                 loss: Literal['linear', 'square', 'exp'] = 'linear', 
-                 verbose: bool = False,
-                 **kwargs: Dict[str, Any]) -> None:
+
+    def __init__(
+        self,
+        base_estimator: Estimator = DecisionTreeRegressor(),
+        n_estimators: int = 50,
+        learning_rate: float = 1.0,
+        loss: Literal["linear", "square", "exp"] = "linear",
+        verbose: bool = False,
+        **kwargs: Dict[str, Any],
+    ) -> None:
         self.base_estimator = base_estimator
         self.n_estimators = n_estimators
         self.learning_rate = learning_rate
         self.loss = loss
         self.verbose = verbose
         self.estimators_: List[Estimator] = []
         self.estimator_weights_: List[float] = []
         self.estimator_errors_: List[float] = []
         self._base_estimator_params = kwargs
         self._fitted = False
-    
-    def fit(self, X: Matrix, y: Vector) -> 'AdaBoostRegressor':
+
+        self.set_param_ranges(
+            {"n_estimators": ("0<,+inf", int), "learning_rate": ("0<,+inf", None)}
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix, y: Vector) -> "AdaBoostRegressor":
         m, _ = X.shape
         sample_weights = np.ones(m)
-        
+
         for i in range(self.n_estimators):
             est = Clone(self.base_estimator).get
-            if hasattr(est, 'max_depth'): est.max_depth = 3
-            
+            if hasattr(est, "max_depth"):
+                est.max_depth = 3
+
             est.set_params(**self._base_estimator_params)
             est.fit(X, y, sample_weights=sample_weights)
             y_pred = est.predict(X)
-            
+
             loss, error = self._get_loss(y, y_pred, sample_weights)
-            if error == 0 or error >= 1.0: continue
-            
+            if error == 0 or error >= 1.0:
+                continue
+
             eps = 1e-10
             error = np.maximum(error, eps)
             alpha = self.learning_rate * np.log((1 - error) / error) / 2
-            
+
             sample_weights *= np.power((1 - error) / error, 1 - loss)
             sample_weights /= np.sum(sample_weights)
-            
+
             self.estimators_.append(est)
             self.estimator_weights_.append(alpha)
             self.estimator_errors_.append(error)
-            
+
             if self.verbose:
-                print(f'[AdaBoost] Finished fitting {type(est).__name__}',
-                      f'{i + 1}/{self.n_estimators} with',
-                      f'error: {error}, alpha: {alpha}')
-        
+                print(
+                    f"[AdaBoost] Finished fitting {type(est).__name__}",
+                    f"{i + 1}/{self.n_estimators} with",
+                    f"error: {error}, alpha: {alpha}",
+                )
+
         self._fitted = True
         return self
-    
-    def _get_loss(self, 
-                  y_true: Vector, 
-                  y_pred: Vector, 
-                  sample_weights: Vector) -> Tuple[Vector, float]:
-        if self.loss == 'linear':
+
+    def _get_loss(
+        self, y_true: Vector, y_pred: Vector, sample_weights: Vector
+    ) -> Tuple[Vector, float]:
+        if self.loss == "linear":
             loss = np.abs(y_true - y_pred)
-        elif self.loss == 'square':
+        elif self.loss == "square":
             loss = (y_true - y_pred) ** 2
-        elif self.loss == 'exp':
+        elif self.loss == "exp":
             loss = 1 - np.exp(-np.abs(y_true - y_pred))
         else:
             raise UnsupportedParameterError(self.loss)
-        
+
         weighted_error = np.sum(sample_weights * loss) / np.sum(sample_weights)
         return loss, weighted_error
 
     def predict(self, X: Matrix) -> Vector:
         preds = np.zeros(X.shape[0])
-        for i, (est, weight) in enumerate(zip(self.estimators_, 
-                                              self.estimator_weights_)):
+        for i, (est, weight) in enumerate(
+            zip(self.estimators_, self.estimator_weights_)
+        ):
             preds += weight * est.predict(X)
             if self.verbose:
-                print(f'[AdaBoost] Finished prediction of',
-                      f'{type(self.base_estimator).__name__}',
-                      f'{i + 1}/{self.n_estimators}')
-        
+                print(
+                    f"[AdaBoost] Finished prediction of",
+                    f"{type(self.base_estimator).__name__}",
+                    f"{i + 1}/{self.n_estimators}",
+                )
+
         return preds
-    
-    def score(self, X: Matrix, y: Vector, 
-              metric: Evaluator = MeanSquaredError) -> float:
+
+    def score(
+        self, X: Matrix, y: Vector, metric: Evaluator = MeanSquaredError
+    ) -> float:
         X_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=X_pred)
 
     def __getitem__(self, index: int) -> Estimator:
         return self.estimators_[index]
 
 
 class GradientBoostingClassifier(Estimator, Estimator.Meta, Supervised):
-    
     """
-    Gradient Boosting Classifier (GBC) is an ensemble learning method that 
-    builds a series of decision trees in a sequential manner, where each tree 
-    tries to correct the errors of its predecessor. It combines weak learners 
-    (typically decision trees) to create a strong predictive model. GBC 
-    focuses on minimizing a loss function, improving model preds 
-    iteratively by fitting new models to the residual errors made by previous 
-    ones. It introduces randomness and prevents overfitting through techniques 
-    like subsampling and feature selection. GBC is versatile, effective for a 
-    wide range of classification and regression tasks, and performs well on 
+    Gradient Boosting Classifier (GBC) is an ensemble learning method that
+    builds a series of decision trees in a sequential manner, where each tree
+    tries to correct the errors of its predecessor. It combines weak learners
+    (typically decision trees) to create a strong predictive model. GBC
+    focuses on minimizing a loss function, improving model preds
+    iteratively by fitting new models to the residual errors made by previous
+    ones. It introduces randomness and prevents overfitting through techniques
+    like subsampling and feature selection. GBC is versatile, effective for a
+    wide range of classification and regression tasks, and performs well on
     both linear and non-linear problems.
-    
+
     Parameters
     ----------
     `base_estimator` : Base est for training multiple models
     (Default `DecisionTreeRegressor`)
     `n_estimators` : Number of boosting stages to be run
     `learning_rate` : Shrinking factor of the contribution of each est
     `subsample` : Fraction of samples to be used for fitting each est
     `**kwargs` : Additional parameters for base est (i.e. `max_depth`)
-    
+
     Notes
     -----
-    - Upon using `__getitem__`, it returns a list of base estimators 
+    - Upon using `__getitem__`, it returns a list of base estimators
     of the passed class index:
-    
+
         ```py
         gb_model = GradientBoostingClassifier(...)
         ...
         gb_model[1] # List of estimators of the class '1'
         gb_model[2][0] # First estimator of the class '2'
         ```
     """
-    
-    def __init__(self, 
-                 base_estimator: Estimator = DecisionTreeRegressor(), 
-                 n_estimators: int = 50, 
-                 learning_rate: float = 0.01, 
-                 subsample: float = 1.0, 
-                 verbose: bool = False,
-                 **kwargs: Dict[str, Any]) -> None:
+
+    def __init__(
+        self,
+        base_estimator: Estimator = DecisionTreeRegressor(),
+        n_estimators: int = 50,
+        learning_rate: float = 0.01,
+        subsample: float = 1.0,
+        verbose: bool = False,
+        **kwargs: Dict[str, Any],
+    ) -> None:
         self.base_estimator = base_estimator
         self.n_estimators = n_estimators
         self.learning_rate = learning_rate
         self.subsample = subsample
         self.verbose = verbose
         self.estimators_: List[list] = None
         self.classes_ = None
         self.n_classes_ = None
         self._base_estimator_params = kwargs
         self._fitted = False
 
-    def fit(self, X: Matrix, y: Vector) -> 'GradientBoostingClassifier':
+        self.set_param_ranges(
+            {
+                "n_estimators": ("0<,+inf", int),
+                "learning_rate": ("0<,+inf", None),
+                "subsample": ("0,1", None),
+            }
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix, y: Vector) -> "GradientBoostingClassifier":
         self._initialize(y)
         m, _ = X.shape
         Fm = np.zeros((m, self.n_classes_)) + self.initial_preds_
-        
+
         for cl in range(self.n_classes_):
             y_c = (y == self.classes_[cl]).astype(float)
             for i in range(self.n_estimators):
                 sample_indices = np.random.choice(
                     np.arange(m), size=int(self.subsample * m), replace=False
                 )
                 X_sample, y_sample = X[sample_indices], y_c[sample_indices]
-                
+
                 p = softmax(Fm[sample_indices], axis=1)
                 residuals = y_sample - p[:, cl]
-                
+
                 est: Estimator = self.estimators_[cl][i]
-                if hasattr(est, 'max_depth'): est.max_depth = 3
-                
+                if hasattr(est, "max_depth"):
+                    est.max_depth = 3
+
                 est.set_params(**self._base_estimator_params)
                 est.fit(X_sample, residuals)
                 update = est.predict(X)
                 Fm[:, cl] += self.learning_rate * update
-                
+
                 if self.verbose:
-                    print(f'[GBC] Finished fitting {type(est).__name__}', 
-                          f'{i + 1}/{self.n_estimators} for class {cl}')
-        
+                    print(
+                        f"[GBC] Finished fitting {type(est).__name__}",
+                        f"{i + 1}/{self.n_estimators} for class {cl}",
+                    )
+
         self._fitted = True
         return self
-    
+
     def _initialize(self, y: Vector) -> None:
         self.classes_ = np.unique(y)
         self.n_classes_ = len(self.classes_)
         self.initial_preds_ = np.zeros(self.n_classes_)
         self.estimators_ = [
-            [Clone(self.base_estimator).get for _ in range(self.n_estimators)] 
+            [Clone(self.base_estimator).get for _ in range(self.n_estimators)]
             for _ in range(self.n_classes_)
         ]
 
     def predict_proba(self, X: Matrix) -> Vector:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         m, _ = X.shape
         Fm = np.zeros((m, self.n_classes_)) + self.initial_preds_
         for cl in range(self.n_classes_):
             for est in self.estimators_[cl]:
                 Fm[:, cl] += self.learning_rate * est.predict(X)
-        
+
         probs = softmax(Fm, axis=1)
         return probs
 
     def predict(self, X: Matrix) -> Vector:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         proba = self.predict_proba(X)
-        
+
         return self.classes_[np.argmax(proba, axis=1)]
-    
+
     def score(self, X: Matrix, y: Vector, metric: Evaluator = Accuracy) -> float:
         X_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=X_pred)
-    
+
     def __getitem__(self, index: int) -> List[Estimator]:
         return self.estimators_[index]
 
 
 class GradientBoostingRegressor(Estimator, Estimator.Meta, Supervised):
-    
     """
-    Gradient Boosting Regressor (GBR) is an ensemble learning method for 
-    regression tasks. It builds a series of decision trees in a sequential 
-    manner, where each tree tries to correct the errors of its predecessor 
-    by fitting to the residual errors. It combines weak learners to create 
-    a strong predictive model and minimizes a loss function, often mean 
+    Gradient Boosting Regressor (GBR) is an ensemble learning method for
+    regression tasks. It builds a series of decision trees in a sequential
+    manner, where each tree tries to correct the errors of its predecessor
+    by fitting to the residual errors. It combines weak learners to create
+    a strong predictive model and minimizes a loss function, often mean
     squared error, iteratively.
-    
+
     Parameters
     ----------
-    `base_estimator` : Base est for training multiple models 
+    `base_estimator` : Base est for training multiple models
     (Default `DecisionTreeRegressor`)
     `n_estimators` : Number of boosting stages to be run
     `learning_rate` : Rate of contribution of each est
     `subsample` : Fraction of samples to be used for fitting each est
     `loss` : Type of loss function (Default `mse`)
     `delta` : Balancing factor between `mse` and `mae`
     `verbose` : Whether to output progress messages
-    `**kwargs` : Additional parameters for the base est 
+    `**kwargs` : Additional parameters for the base est
     (i.e. `max_depth`)
-    
+
     """
-    
-    def __init__(self, 
-                 base_estimator: Estimator = DecisionTreeRegressor(), 
-                 n_estimators: int = 50, 
-                 learning_rate: float = 0.01, 
-                 subsample: float = 1.0, 
-                 loss: Literal['mse', 'mae', 'huber'] = 'mse', 
-                 delta: float = 1.0, 
-                 verbose: bool = False, 
-                 **kwargs: Dict[str, Any]) -> None:
+
+    def __init__(
+        self,
+        base_estimator: Estimator = DecisionTreeRegressor(),
+        n_estimators: int = 50,
+        learning_rate: float = 0.01,
+        subsample: float = 1.0,
+        loss: Literal["mse", "mae", "huber"] = "mse",
+        delta: float = 1.0,
+        verbose: bool = False,
+        **kwargs: Dict[str, Any],
+    ) -> None:
         self.base_estimator = base_estimator
         self.n_estimators = n_estimators
         self.learning_rate = learning_rate
         self.subsample = subsample
         self.loss = loss
         self.delta = delta
         self.verbose = verbose
         self.estimators_ = []
         self._base_estimator_params = kwargs
         self._fitted = False
 
-    def fit(self, X: Matrix, y: Vector) -> 'GradientBoostingRegressor':
+        self.set_param_ranges(
+            {
+                "n_estimators": ("0<,+inf", int),
+                "learning_rate": ("0<,+inf", None),
+                "subsample": ("0,1", None),
+                "delta": ("0,1", None),
+            }
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix, y: Vector) -> "GradientBoostingRegressor":
         self.init_pred_ = self._initial_prediction(y)
         self.estimators_ = []
         m, _ = X.shape
         Fm = np.mean(y)
-        
+
         for i in range(self.n_estimators):
             residuals = self._loss_derivative(y, Fm)
             est = Clone(self.base_estimator).get
             est.set_params(**self._base_estimator_params)
-            
+
             sample_indices = np.random.choice(
                 np.arange(m), size=int(self.subsample * m), replace=False
             )
             X_sample, y_sample = X[sample_indices], residuals[sample_indices]
-            
+
             est.fit(X_sample, y_sample)
             self.estimators_.append(est)
             Fm += self.learning_rate * est.predict(X)
-            
+
             if self.verbose:
-                print(f'Finished fitting est {i+1}/{self.n_estimators}')
-                
+                print(f"Finished fitting est {i+1}/{self.n_estimators}")
+
         self._fitted = True
         return self
-    
+
     def _initial_prediction(self, y: Vector) -> Vector:
-        if self.loss in ('mse', 'huber'): return np.mean(y)
-        elif self.loss == 'mae': return np.median(y)
-        else: 
+        if self.loss in ("mse", "huber"):
+            return np.mean(y)
+        elif self.loss == "mae":
+            return np.median(y)
+        else:
             raise UnsupportedParameterError(self.loss)
 
     def _loss_derivative(self, y_true: Vector, y_pred: Vector) -> Vector:
-        if self.loss == 'mse': return -(y_true - y_pred)
-        elif self.loss == 'mae': return np.sign(y_true - y_pred)
-        elif self.loss == 'huber':
+        if self.loss == "mse":
+            return -(y_true - y_pred)
+        elif self.loss == "mae":
+            return np.sign(y_true - y_pred)
+        elif self.loss == "huber":
             diff = y_true - y_pred
             is_small_error = np.abs(diff) <= self.delta
             return np.where(is_small_error, -diff, -self.delta * np.sign(diff))
         else:
             raise UnsupportedParameterError(self.loss)
-    
+
     def predict(self, X: Matrix) -> Vector:
-        if not self._fitted: raise NotFittedError(self)
-        preds = sum(self.learning_rate * est.predict(X) 
-                    for est in self.estimators_)
-        
+        if not self._fitted:
+            raise NotFittedError(self)
+        preds = sum(self.learning_rate * est.predict(X) for est in self.estimators_)
+
         return self.init_pred_ + preds
-    
-    def score(self, X: Matrix, y: Vector, 
-              metric: Evaluator = MeanSquaredError) -> float:
+
+    def score(
+        self, X: Matrix, y: Vector, metric: Evaluator = MeanSquaredError
+    ) -> float:
         X_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=X_pred)
-    
+
     def __getitem__(self, index: int) -> Estimator:
         return self.estimators_[index]
-
```

### Comparing `luma-ml-0.6.4/luma/ensemble/forest.py` & `luma-ml-0.6.5/luma/ensemble/forest.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,57 +7,55 @@
 from luma.regressor.tree import DecisionTreeRegressor
 from luma.core.super import Estimator, Evaluator, Supervised
 from luma.interface.exception import NotFittedError, UnsupportedParameterError
 from luma.metric.classification import Accuracy
 from luma.metric.regression import MeanSquaredError
 
 
-__all__ = (
-    'RandomForestClassifier', 
-    'RandomForestRegressor'
-)
+__all__ = ("RandomForestClassifier", "RandomForestRegressor")
 
 
 class RandomForestClassifier(Estimator, Estimator.Meta, Supervised):
-    
     """
-    A Random Forest Classifier is an ensemble learning method in machine learning, 
-    widely used for both classification and regression tasks. It operates by 
-    constructing a multitude of decision trees during the training phase and 
+    A Random Forest Classifier is an ensemble learning method in machine learning,
+    widely used for both classification and regression tasks. It operates by
+    constructing a multitude of decision trees during the training phase and
     outputs the mode of the classes for classification.
-    
+
     Parameters
     ----------
     `n_trees` : Number of trees in the forest
     `max_depth` :  Maximum depth of each trees
     `criterion` : Function used to measure the quality of a split
     `min_samples_split` : Minimum samples required to split a node
     `min_samples_leaf` : Minimum samples required to be at a leaf node
     `max_features` : Number of features to consider
     `min_impurity_decrease` : Minimum decrement of impurity for a split
     `max_leaf_nodes` : Maximum amount of leaf nodes
     `bootstrap` : Whether to bootstrap the samples of dataset
     `bootstrap_feature` : Whether to bootstrap the features of each data
     `n_features` : Number of features to be sampled when bootstrapping features
-    
+
     """
-    
-    def __init__(self, 
-                 n_trees: int = 10, 
-                 max_depth: int = 100,
-                 criterion: Literal['gini', 'entropy'] = 'gini', 
-                 min_samples_split: int = 2,
-                 min_samples_leaf: int = 1, 
-                 max_features: int = None, 
-                 min_impurity_decrease: float = 0.0, 
-                 max_leaf_nodes: int = None, 
-                 bootstrap: bool = True,
-                 bootstrap_feature: bool = False,
-                 n_features: int | Literal['auto'] = 'auto',
-                 verbose: bool = False) -> None:
+
+    def __init__(
+        self,
+        n_trees: int = 10,
+        max_depth: int = 100,
+        criterion: Literal["gini", "entropy"] = "gini",
+        min_samples_split: int = 2,
+        min_samples_leaf: int = 1,
+        max_features: int = None,
+        min_impurity_decrease: float = 0.0,
+        max_leaf_nodes: int = None,
+        bootstrap: bool = True,
+        bootstrap_feature: bool = False,
+        n_features: int | Literal["auto"] = "auto",
+        verbose: bool = False,
+    ) -> None:
         self.n_trees = n_trees
         self.max_depth = max_depth
         self.criterion = criterion
         self.min_samples_split = min_samples_split
         self.min_samples_leaf = min_samples_leaf
         self.max_features = max_features
         self.min_impurity_decrease = min_impurity_decrease
@@ -65,107 +63,118 @@
         self.n_features = n_features
         self.bootstrap = bootstrap
         self.bootstrap_feature = bootstrap_feature
         self.verbose = verbose
         self.trees = None
         self._fitted = False
 
-    def fit(self, 
-            X: Matrix, 
-            y: Matrix, 
-            sample_weights: Vector = None) -> 'RandomForestClassifier':
+        self.set_param_ranges(
+            {
+                "n_trees": ("0<,+inf", int),
+                "max_depth": ("0<,+inf", int),
+                "min_samples_split": ("0<,+inf", int),
+                "max_samples_leaf": ("0<,+inf", int),
+                "min_impurity_decrease": ("0,+inf", None),
+            }
+        )
+        self.check_param_ranges()
+
+    def fit(
+        self, X: Matrix, y: Matrix, sample_weights: Vector = None
+    ) -> "RandomForestClassifier":
         m, n = X.shape
-        if self.n_features == 'auto': 
-            self.n_features = int(n ** 0.5)
+        if self.n_features == "auto":
+            self.n_features = int(n**0.5)
         else:
             if isinstance(self.n_features, str):
                 raise UnsupportedParameterError(self.n_features)
-        
+
         _tree_params = {
-            'max_depth': self.max_depth,
-            'criterion': self.criterion,
-            'min_samples_split': self.min_samples_split,
-            'min_samples_leaf': self.min_samples_leaf,
-            'max_features': self.max_features,
-            'min_impurity_decrease': self.min_impurity_decrease,
-            'max_leaf_nodes': self.max_leaf_nodes
+            "max_depth": self.max_depth,
+            "criterion": self.criterion,
+            "min_samples_split": self.min_samples_split,
+            "min_samples_leaf": self.min_samples_leaf,
+            "max_features": self.max_features,
+            "min_impurity_decrease": self.min_impurity_decrease,
+            "max_leaf_nodes": self.max_leaf_nodes,
         }
-        
+
         self.trees = [DecisionTreeClassifier() for _ in range(self.n_trees)]
         for i, tree in enumerate(self.trees, start=1):
             X_sample, y_sample = X, y
             if self.bootstrap:
                 bootstrap_data = np.random.choice(m, m, replace=True)
                 X_sample = X_sample[bootstrap_data]
                 y_sample = y_sample[bootstrap_data]
             if self.bootstrap_feature:
                 bootstrap_feature = np.random.choice(n, self.n_features, replace=True)
                 X_sample = X_sample[:, bootstrap_feature]
-            
+
             tree.set_params(**_tree_params)
             tree.fit(X_sample, y_sample, sample_weights=sample_weights)
-            
+
             if self.verbose:
-                print(f'[RandomForest] Finished fitting tree {i}/{self.n_trees}')
-        
+                print(f"[RandomForest] Finished fitting tree {i}/{self.n_trees}")
+
         self._fitted = True
         return self
 
     def predict(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         preds = Matrix([tree.predict(X) for tree in self.trees])
         majority, _ = mode(preds, axis=0)
-        
+
         return majority.flatten()
-    
-    def score(self, X: Matrix, y: Matrix, 
-              metric: Evaluator = Accuracy) -> float:
+
+    def score(self, X: Matrix, y: Matrix, metric: Evaluator = Accuracy) -> float:
         X_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=X_pred)
-    
+
     def __gettiem__(self, index: int) -> DecisionTreeClassifier:
         return self.trees[index]
 
 
 class RandomForestRegressor(Estimator, Estimator.Meta, Supervised):
-    
     """
-    A Random Forest Regressor is an ensemble learning algorithm for regression 
-    tasks. It builds multiple decision trees during training, each on a random 
-    subset of features and bootstrapped data. The final prediction is the average 
+    A Random Forest Regressor is an ensemble learning algorithm for regression
+    tasks. It builds multiple decision trees during training, each on a random
+    subset of features and bootstrapped data. The final prediction is the average
     of individual tree predictions, providing a robust and accurate result.
-    
+
     Parameters
     ----------
     `n_trees` : Number of trees in the forest
     `max_depth` :  Maximum depth of each trees
     `min_samples_split` : Minimum samples required to split a node
     `min_samples_leaf` : Minimum samples required to be at a leaf node
     `max_features` : Number of features to consider
     `min_variance_decrease` : Minimum decrement of variance for a split
     `max_leaf_nodes` : Maximum amount of leaf nodes
     `bootstrap` : Whether to bootstrap the samples of dataset
     `bootstrap_feature` : Whether to bootstrap the features of each data
     `n_features` : Number of features to be sampled when bootstrapping features
-    
+
     """
-    
-    def __init__(self, 
-                 n_trees: int = 10, 
-                 max_depth: int = 10, 
-                 min_samples_split: int = 2,
-                 min_samples_leaf: int = 1, 
-                 max_features: int = None, 
-                 min_variance_decrease: float = 0.0,
-                 max_leaf_nodes: int = None,
-                 bootstrap: bool = True,
-                 bootstrap_feature: bool = False,
-                 n_features: int | Literal['auto'] = 'auto',
-                 sample_weights: Vector = None,
-                 verbose: bool = False) -> None:
+
+    def __init__(
+        self,
+        n_trees: int = 10,
+        max_depth: int = 10,
+        min_samples_split: int = 2,
+        min_samples_leaf: int = 1,
+        max_features: int = None,
+        min_variance_decrease: float = 0.0,
+        max_leaf_nodes: int = None,
+        bootstrap: bool = True,
+        bootstrap_feature: bool = False,
+        n_features: int | Literal["auto"] = "auto",
+        sample_weights: Vector = None,
+        verbose: bool = False,
+    ) -> None:
         self.n_trees = n_trees
         self.max_depth = max_depth
         self.min_samples_split = min_samples_split
         self.min_samples_leaf = min_samples_leaf
         self.max_features = max_features
         self.min_variance_decrease = min_variance_decrease
         self.max_leaf_nodes = max_leaf_nodes
@@ -173,59 +182,71 @@
         self.bootstrap = bootstrap
         self.bootstrap_feature = bootstrap_feature
         self.sample_weights = sample_weights
         self.verbose = verbose
         self.trees = None
         self._fitted = False
 
-    def fit(self, X: Matrix, y: Matrix) -> 'RandomForestRegressor':
+        self.set_param_ranges(
+            {
+                "n_trees": ("0<,+inf", int),
+                "max_depth": ("0<,+inf", int),
+                "min_samples_split": ("0<,+inf", int),
+                "max_samples_leaf": ("0<,+inf", int),
+                "min_variance_decrease": ("0,+inf", None),
+            }
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix, y: Matrix) -> "RandomForestRegressor":
         m, n = X.shape
-        if self.n_features == 'auto': 
-            self.n_features = int(n ** 0.5)
+        if self.n_features == "auto":
+            self.n_features = int(n**0.5)
         else:
             if isinstance(self.n_features, str):
                 raise UnsupportedParameterError(self.n_features)
-        
+
         _tree_params = {
-            'max_depth': self.max_depth,
-            'min_samples_split': self.min_samples_split,
-            'min_samples_leaf': self.min_samples_leaf,
-            'max_features': self.max_features,
-            'min_variance_decrease': self.min_variance_decrease,
-            'max_leaf_nodes': self.max_leaf_nodes
+            "max_depth": self.max_depth,
+            "min_samples_split": self.min_samples_split,
+            "min_samples_leaf": self.min_samples_leaf,
+            "max_features": self.max_features,
+            "min_variance_decrease": self.min_variance_decrease,
+            "max_leaf_nodes": self.max_leaf_nodes,
         }
-        
+
         self.trees = [DecisionTreeRegressor() for _ in range(self.n_trees)]
         for i, tree in enumerate(self.trees, start=1):
             X_sample, y_sample = X, y
             if self.bootstrap:
                 bootstrap_data = np.random.choice(m, m, replace=True)
                 X_sample = X_sample[bootstrap_data]
                 y_sample = y_sample[bootstrap_data]
             if self.bootstrap_feature:
                 bootstrap_feature = np.random.choice(n, self.n_features, replace=True)
                 X_sample = X_sample[:, bootstrap_feature]
-            
+
             tree.set_params(**_tree_params)
             tree.fit(X_sample, y_sample, sample_weights=self.sample_weights)
-            
+
             if self.verbose:
-                print(f'[RandomForest] Finished fitting tree {i}/{self.n_trees}')
-        
+                print(f"[RandomForest] Finished fitting tree {i}/{self.n_trees}")
+
         self._fitted = True
         return self
 
     def predict(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         preds = Matrix([tree.predict(X) for tree in self.trees])
         average_predictions = np.mean(preds, axis=0)
-        
+
         return average_predictions
-    
-    def score(self, X: Matrix, y: Matrix, 
-              metric: Evaluator = MeanSquaredError) -> float:
+
+    def score(
+        self, X: Matrix, y: Matrix, metric: Evaluator = MeanSquaredError
+    ) -> float:
         X_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=X_pred)
-    
+
     def __gettiem__(self, index: int) -> DecisionTreeClassifier:
         return self.trees[index]
-
```

### Comparing `luma-ml-0.6.4/luma/ensemble/stack.py` & `luma-ml-0.6.5/luma/reduction/selection.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,361 +1,464 @@
-from typing import Any, List, Dict, Literal
+from itertools import combinations
+from typing import Tuple
 import numpy as np
 
-from luma.core.super import Estimator, Transformer, Evaluator, Supervised
+from luma.core.super import Estimator, Evaluator, Transformer, Supervised
+from luma.interface.util import Matrix, Vector, Clone
 from luma.interface.exception import NotFittedError, UnsupportedParameterError
-from luma.interface.util import Matrix, Vector
-from luma.classifier.logistic import SoftmaxRegressor
-from luma.regressor.linear import LinearRegressor
-from luma.metric.classification import Accuracy
-from luma.metric.regression import MeanSquaredError
+from luma.model_selection.split import TrainTestSplit
+from luma.model_selection.cv import CrossValidator
 from luma.model_selection.fold import FoldType, KFold
 
 
-__all__ = (
-    'StackingClassifier',
-    'StackingRegressor'
-)
+__all__ = ("SBS", "SFS", "RFE")
 
 
-class StackingClassifier(Estimator, Transformer, Supervised):
-    
+class SBS(Transformer, Transformer.Feature, Supervised):
     """
-    A stacking classifier is a machine learning model that combines multiple 
-    classification models into a single predictive model by stacking the output 
-    of individual classifiers as input to a final classifier. This final 
-    classifier, often called a meta-classifier, is trained to make a final 
-    prediction based on the outputs of the base classifiers. Stacking aims to 
-    leverage the strengths of each base model to improve overall prediction 
-    accuracy.
-    
+    Sequential Backward Selection (SBS) is a feature selection technique
+    used in machine learning. It starts with all features and iteratively
+    removes the least significant feature at each step_size. The goal is to
+    reduce dimensionality while maintaining or improving model performance.
+    The process continues until the desired number of features is reached
+    or performance criteria are met.
+
     Parameters
     ----------
-    `estimators` : List of base estimators
-    `final_estimator` : Final meta-estimator (Default `SoftmaxRegressor`)
-    `pass_original` : Whether to pass the original data to final estimator
-    `drop_threshold` : Omitting threshold for base estimators
-    (`None` not to omit any estimators)
-    `metric` : Scoring metric
-    `method` : Methods called for each base estimator
-    `cv` : Number of folds for cross-validation
+    `estimator` : An estimator to fit and evaluate
+    `n_features` : Number of features to select (`0~1` value for proportion)
+    `metric` : Scoring metric for selecting features
+    `test_size` : Proportional size of the validation set
+    `cv` : K-fold size for cross validation (`0` to disable CV)
+    `shuffle` : Whether to shuffle the dataset
+    `stratify` : Whether to perform stratified split
     `fold_type` : Fold type (Default `KFold`)
-    `shuffle` : Whether to shuffle the dataset when cross-validating
-    `random_state` : Seed for random splitting
-    `**kwargs` : Additional parameters for final estimator
-    (i.e. `learning_rate`)
-    
+    `random_state` : Seed for splitting the data
+
     Notes
     -----
-    `StackingClassifier` can also be utilized as `Transformer`.
-    
-    - The method `transform` returns class labels or probabilities by each 
-        base estimator as a stacked form:
-    
-        ```py
-        def transform(self, X: Matrix) -> Matrix
-        ```
-    
-    Each base estimators can be accessed via indexing of its instance:
-    >>> estimator = stack[0]
-    
+    * An instance of the estimator must be passed to `estimator`
+    * For `metric`, both class or instance are possible
+
     Examples
     --------
-    ```py
-    stack = StackingClassifier(estimators=[...],
-                               final_estimator=SoftmaxRegressor(),
-                               method='label',
-                               cv=5,
-                               fold_type=KFold)
-    stack.fit(X, y)
-    X_new = stack.transform(X)
-    y_pred = stack.predict(X)
-    ```
+    >>> sbs = SBS(estimator=AnyEstimator(),
+                  n_features=0.25,
+                  metric=AnyEvaluator,
+                  test_size=0.2,
+                  cv=5,
+                  random_state=None)
+    >>> sbs.fit(X, y)
+    >>> Z = sbs.transform(X)
+
     """
 
-    def __init__(self, 
-                 estimators: List[Estimator],
-                 final_estimator: Estimator = SoftmaxRegressor(), 
-                 pass_original: bool = False,
-                 drop_threshold: float = None, 
-                 metric: Evaluator = Accuracy,
-                 method: Literal['label', 'prob'] = 'label',
-                 cv: int = 5,
-                 fold_type: FoldType = KFold, 
-                 shuffle: bool = True,
-                 random_state: int = None,
-                 verbose: bool = False, 
-                 **kwargs: Dict[str, Any]) -> None:
-        self.estimators = estimators
-        self.final_estimator = final_estimator
-        self.pass_original = pass_original
-        self.drop_threshold = drop_threshold
+    def __init__(
+        self,
+        estimator: Estimator = None,
+        n_features: int | float = 1,
+        metric: Evaluator = None,
+        test_size: float = 0.2,
+        cv: int = 5,
+        shuffle: bool = True,
+        stratify: bool = False,
+        fold_type: FoldType = KFold,
+        random_state: int = None,
+        verbose: bool = False,
+    ) -> None:
+        self.estimator = estimator
+        self.n_features = n_features
         self.metric = metric
-        self.method = method
+        self.test_size = test_size
         self.cv = cv
-        self.fold_type = fold_type
         self.shuffle = shuffle
+        self.stratify = stratify
+        self.fold_type = fold_type
         self.random_state = random_state
         self.verbose = verbose
-        self._final_estimator_params = kwargs
-        self._base_estimators: List[Estimator] = []
         self._fitted = False
-        
-        if self.method not in ('label', 'prob'):
-            raise UnsupportedParameterError(self.method)
-
-    def fit(self, X: Matrix, y: Vector) -> 'StackingClassifier':
-        m, _ = X.shape
-        self.n_classes = len(np.unique(y))
-        
-        fold = self.fold_type(X, y,
-                              n_folds=self.cv,
-                              shuffle=self.shuffle,
-                              random_state=self.random_state)
-        
-        if self.method == 'label': X_new = np.zeros((m, len(self.estimators)))
-        else: X_new = np.zeros((m, len(self.estimators) * self.n_classes))
-        
-        for i, est in enumerate(self.estimators):
-            if self.method == 'label': preds = np.zeros(m)
-            else: preds = np.zeros((m, self.n_classes))
-            
-            for train_indices, test_indices in fold.split:
-                X_train, y_train = X[train_indices], y[train_indices]
-                X_test = X[test_indices]
-                
-                est.fit(X_train, y_train)
-                if self.method == 'label': pred = est.predict(X_test)
+
+    def fit(self, X: Matrix, y: Vector) -> "SBS":
+        _, n = X.shape
+        self.estimator = Clone(self.estimator).get
+
+        if 0 < self.n_features < 1:
+            self.n_features = np.ceil(n * self.n_features).astype(int)
+        elif self.n_features <= 0 or self.n_features > n:
+            raise UnsupportedParameterError(self.n_features)
+
+        if self.cv:
+            cv_model = CrossValidator(
+                estimator=self.estimator,
+                metric=self.metric,
+                cv=self.cv,
+                shuffle=self.shuffle,
+                fold_type=self.fold_type,
+                random_state=self.random_state,
+            )
+        else:
+            Xy_split = TrainTestSplit(
+                X,
+                y,
+                test_size=self.test_size,
+                shuffle=self.shuffle,
+                stratify=self.stratify,
+                random_state=self.random_state,
+            ).get
+            X_train, X_test, y_train, y_test = Xy_split
+
+        self.indices = tuple(range(n))
+        self.subsets = [self.indices]
+
+        if self.cv:
+            _, score = cv_model.score(X, y)
+        else:
+            score = self._calculate_score(
+                X_train, X_test, y_train, y_test, indices=self.indices
+            )
+        self.scores = [score]
+
+        iter = 1
+        while n > self.n_features:
+            scores = []
+            subsets = []
+            for p in combinations(self.indices, n - 1):
+                if self.cv:
+                    _, score = cv_model.score(X[:, p], y)
                 else:
-                    if not hasattr(est, 'predict_proba'):
-                        raise ValueError(f"{type(est).__name__}" + 
-                                         " does not support 'predict_proba'!")
-                    pred = est.predict_proba(X_test)
-                
-                preds[test_indices] = pred
-            
-            score = est.score(X, y, metric=self.metric)
-            if self.drop_threshold is not None and score < self.drop_threshold:
-                if self.verbose:
-                    print(f'[StackingClassifier] {type(est).__name__}',
-                          f'dropped for low score: {score}')
-                continue
-            
-            if self.method == 'label': X_new[:, i] = preds
-            else: X_new[:, i * self.n_classes:(i + 1) * self.n_classes] = preds
-            
-            self._base_estimators.append(est)
+                    score = self._calculate_score(
+                        X_train, X_test, y_train, y_test, indices=p
+                    )
+                scores.append(score)
+                subsets.append(p)
+
+            best = np.argmax(scores)
+            self.indices = subsets[best]
+            self.subsets.append(self.indices)
+            self.scores.append(scores[best])
+
             if self.verbose:
-                print(f'[StackingClassifier] Finished CV fitting',
-                      f'for {type(est).__name__} with score: {score}')
-        
-        if self.pass_original:
-            X_new = np.hstack((X, X_new))
-        
-        self.final_estimator.set_params(**self._final_estimator_params)
-        self.final_estimator.fit(X_new, y)
-        
+                print(
+                    f"[SBS] Feature added: {self.indices[-1]}",
+                    f"with score: {scores[best]}",
+                )
+
+            n -= 1
+            iter += 1
+
+        self.n_score = self.scores[-1]
         if self.verbose:
-            print(f'[StackingClassifier] Finished fitting for',
-                  f'{type(self.final_estimator).__name__}(final)')
-        
+            print(f"[SBS] Selection finished with final features: {self.indices}")
+
         self._fitted = True
         return self
 
-    def predict(self, X: Matrix) -> Vector:
-        if not self._fitted: raise NotFittedError(self)
-        X_new = self.transform(X)
-        
-        return self.final_estimator.predict(X_new)
-
-    def predict_proba(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
-        if self.method == 'label':
-            raise UnsupportedParameterError(self.method)
-        
-        X_new = self.transform(X)
-        if hasattr(self.final_estimator, 'predict_proba'):
-            return self.final_estimator.predict_proba(X_new)
-        else:
-            raise ValueError(f"{type(self.final_estimator).__name__}" + 
-                             " does not support 'predict_proba'!")
-    
+    def _calculate_score(
+        self,
+        X_train: Matrix,
+        X_test: Matrix,
+        y_train: Matrix,
+        y_test: Matrix,
+        indices: Tuple,
+    ) -> float:
+        self.estimator.fit(X_train[:, indices], y_train)
+        y_pred = self.estimator.predict(X_test[:, indices])
+
+        return self.metric.score(y_true=y_test, y_pred=y_pred)
+
     def transform(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
-        m, _ = X.shape
-        
-        if self.method == 'label':
-            X_new = np.zeros((m, len(self._base_estimators)))
-            for i, est in enumerate(self._base_estimators):
-                X_new[:, i] = est.predict(X)
-        else:
-            X_new = np.zeros((m, len(self._base_estimators) * self.n_classes))
-            for i, est in enumerate(self._base_estimators):
-                if hasattr(est, 'predict_proba'): 
-                    preds = est.predict_proba(X)
-                    X_new[:, i * self.n_classes:(i + 1) * self.n_classes] = preds
-                else: 
-                    raise ValueError(f"{type(est).__name__}" + 
-                                    " does not support 'predict_proba'!")
-        if self.pass_original:
-            X_new = np.hstack((X, X_new))
-        
-        return X_new
+        if not self._fitted:
+            raise NotFittedError(self)
+        return X[:, self.indices]
 
     def fit_transform(self, X: Matrix, y: Vector) -> Matrix:
         self.fit(X, y)
         return self.transform(X)
-    
-    def score(self, X: Matrix, y: Vector, metric: Evaluator = Accuracy) -> float:
-        X_pred = self.predict(X)
-        return metric.score(y_true=y, y_pred=X_pred)
-
-    def __getitem__(self, index: int) -> Estimator:
-        return self._base_estimators[index]
 
 
-class StackingRegressor(Estimator, Transformer, Supervised):
-    
+class SFS(Transformer, Transformer.Feature, Supervised):
     """
-    A stacking regressor is a machine learning model that combines multiple 
-    regression models into a single predictive model by stacking the output 
-    of individual regressors as input to a final regressor. This final 
-    regressor, often called a meta-regressor, is trained to make a final 
-    prediction based on the outputs of the base regressors. Stacking aims to 
-    leverage the strengths of each base model to improve overall prediction 
-    accuracy.
-    
+    Sequential Forward Selection (SFS) is a feature selection technique
+    used in machine learning. It starts with no features and iteratively
+    adds the most significant feature at each step. The goal is to
+    reduce dimensionality while maintaining or improving model performance.
+    The process continues until the desired number of features is reached
+    or performance criteria are met.
+
     Parameters
     ----------
-    `estimators` : List of base estimators
-    `final_estimator` : Final meta-estimator (Default `LinearRegressor`)
-    `pass_original` : Whether to pass the original data to final estimator
-    `cv` : Number of folds for cross-validation
+    `estimator` : An estimator to fit and evaluate
+    `n_features` : Number of features to select (`0~1` value for proportion)
+    `metric` : Scoring metric for selecting features
+    `test_size` : Proportional size of the validation set
+    `cv` : K-fold size for cross validation (`0` to disable CV)
+    `shuffle` : Whether to shuffle the dataset
+    `stratify` : Whether to perform stratified split
     `fold_type` : Fold type (Default `KFold`)
-    `metric` : Scoring metric
-    `shuffle` : Whether to shuffle the dataset when cross-validating
-    `random_state` : Seed for random splitting
-    `**kwargs` : Additional parameters for final estimator
-    (i.e. `learning_rate`)
-    
+    `random_state` : Seed for splitting the data
+
     Notes
     -----
-    `StackingRegressor` can also be utilized as `Transformer`.
-    
-    - The method `transform` returns class labels or probabilities by each 
-        base estimator as a stacked form:
-    
-        ```py
-        def transform(self, X: Matrix) -> Matrix
-        ```
-    
-    Each base estimators can be accessed via indexing of its instance:
-    >>> estimator = stack[0]
-    
+    * An instance of the estimator must be passed to `estimator`
+    * Do not use the estimator for `SFS` if it is supposed to be the
+        main estimator for the model
+    * For `metric`, both class or instance are possible
+
     Examples
     --------
-    ```py
-    stack = StackingRegressor(estimators=[...],
-                              final_estimator=LinearRegressor(),
-                              cv=5,
-                              fold_type=KFold)
-    stack.fit(X, y)
-    X_new = stack.transform(X)
-    y_pred = stack.predict(X)
-    ```
+    >>> sfs = SFS(estimator=AnyEstimator(),
+                  n_features=0.25,
+                  metric=AnyEvaluator,
+                  test_size=0.2,
+                  cv=5,
+                  random_state=None)
+    >>> sfs.fit(X, y)
+    >>> Z = sbs.transform(X)
+
     """
-    
-    def __init__(self, 
-                 estimators: List[Estimator],
-                 final_estimator: Estimator = LinearRegressor(), 
-                 pass_original: bool = False,
-                 cv: int = 5,
-                 fold_type: FoldType = KFold, 
-                 metric: Evaluator = MeanSquaredError,
-                 shuffle: bool = True,
-                 random_state: int = None,
-                 verbose: bool = False, 
-                 **kwargs: Dict[str, Any]) -> None:
-        self.estimators = estimators
-        self.final_estimator = final_estimator
-        self.pass_original = pass_original
-        self.cv = cv
-        self.fold_type = fold_type
+
+    def __init__(
+        self,
+        estimator: Estimator = None,
+        n_features: int | float = 1,
+        metric: Evaluator = None,
+        test_size: float = 0.2,
+        cv: int = 5,
+        shuffle: bool = True,
+        stratify: bool = False,
+        fold_type: FoldType = KFold,
+        random_state: int = None,
+        verbose: bool = False,
+    ) -> None:
+        self.estimator = estimator
+        self.n_features = n_features
         self.metric = metric
+        self.test_size = test_size
+        self.cv = cv
         self.shuffle = shuffle
+        self.stratify = stratify
+        self.fold_type = fold_type
         self.random_state = random_state
         self.verbose = verbose
-        self._final_estimator_params = kwargs
-        self._base_estimators: List[Estimator] = []
         self._fitted = False
 
-    def fit(self, X: Matrix, y: Vector) -> 'StackingClassifier':
-        m, _ = X.shape
-        self.n_classes = len(np.unique(y))
-        
-        fold = self.fold_type(X, y,
-                              n_folds=self.cv,
-                              shuffle=self.shuffle,
-                              random_state=self.random_state)
-        
-        X_new = np.zeros((m, len(self.estimators)))
-        for i, est in enumerate(self.estimators):
-            preds = np.zeros(m)
-            for train_indices, test_indices in fold.split:
-                X_train, y_train = X[train_indices], y[train_indices]
-                X_test = X[test_indices]
-                
-                est.fit(X_train, y_train)
-                pred = est.predict(X_test)
-                preds[test_indices] = pred
-            
-            score = est.score(X, y, metric=self.metric)
-            X_new[:, i] = preds
-            
-            self._base_estimators.append(est)
+    def fit(self, X: Matrix, y: Vector) -> "SFS":
+        _, n = X.shape
+        self.estimator = Clone(self.estimator).get
+
+        if isinstance(self.n_features, float) and 0 < self.n_features < 1:
+            self.n_features = np.ceil(n * self.n_features).astype(int)
+        elif self.n_features <= 0 or self.n_features > n:
+            raise UnsupportedParameterError(self.n_features)
+
+        if self.cv:
+            cv_model = CrossValidator(
+                estimator=self.estimator,
+                metric=self.metric,
+                cv=self.cv,
+                shuffle=self.shuffle,
+                fold_type=self.fold_type,
+                random_state=self.random_state,
+            )
+        else:
+            Xy_split = TrainTestSplit(
+                X,
+                y,
+                test_size=self.test_size,
+                shuffle=self.shuffle,
+                stratify=self.stratify,
+                random_state=self.random_state,
+            ).get
+            X_train, X_test, y_train, y_test = Xy_split
+
+        self.indices = ()
+        self.subsets = [self.indices]
+        score = -np.inf
+        self.scores = [score]
+
+        while len(self.indices) < self.n_features:
+            scores = []
+            subsets = []
+            for p in combinations(range(n), len(self.indices) + 1):
+                if set(self.indices).issubset(set(p)):
+                    if self.cv:
+                        _, score = cv_model.score(X[:, p], y)
+                    else:
+                        score = self._calculate_score(
+                            X_train, X_test, y_train, y_test, indices=p
+                        )
+                    scores.append(score)
+                    subsets.append(p)
+
+            best = np.argmax(scores)
+            self.indices = subsets[best]
+            self.subsets.append(self.indices)
+            self.scores.append(scores[best])
+
             if self.verbose:
-                print(f'[StackingRegressor] Finished CV fitting',
-                      f'for {type(est).__name__} with score: {score}')
-        
-        if self.pass_original:
-            X_new = np.hstack((X, X_new))
-        
-        self.final_estimator.set_params(**self._final_estimator_params)
-        self.final_estimator.fit(X_new, y)
-        
+                print(
+                    f"[SFS] Feature added: {self.indices[-1]}",
+                    f"with score: {scores[best]}",
+                )
+
+        self.n_score = self.scores[-1]
         if self.verbose:
-            print(f'[StackingRegressor] Finished fitting for',
-                  f'{type(self.final_estimator).__name__}(final)')
-        
+            print(f"[SFS] Selection finished with final features: {self.indices}")
+
         self._fitted = True
         return self
 
-    def predict(self, X: Matrix) -> Vector:
-        if not self._fitted: raise NotFittedError(self)
-        X_new = self.transform(X)
-        
-        return self.final_estimator.predict(X_new)
-    
+    def _calculate_score(
+        self,
+        X_train: Matrix,
+        X_test: Matrix,
+        y_train: Matrix,
+        y_test: Matrix,
+        indices: Tuple,
+    ) -> float:
+        self.estimator.fit(X_train[:, indices], y_train)
+        y_pred = self.estimator.predict(X_test[:, indices])
+
+        return self.metric.score(y_true=y_test, y_pred=y_pred)
+
     def transform(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
-        m, _ = X.shape
-        X_new = np.zeros((m, len(self._base_estimators)))
-        for i, est in enumerate(self._base_estimators):
-            X_new[:, i] = est.predict(X)
-            
-        if self.pass_original: 
-            X_new = np.hstack((X, X_new))
-        
-        return X_new
+        if not self._fitted:
+            raise NotFittedError(self)
+        return X[:, self.indices]
 
     def fit_transform(self, X: Matrix, y: Vector) -> Matrix:
         self.fit(X, y)
         return self.transform(X)
-    
-    def score(self, X: Matrix, y: Vector, 
-              metric: Evaluator = MeanSquaredError) -> float:
-        X_pred = self.predict(X)
-        return metric.score(y_true=y, y_pred=X_pred)
 
-    def __getitem__(self, index: int) -> Estimator:
-        return self._base_estimators[index]
 
+class RFE(Transformer, Transformer.Feature, Supervised):
+    """
+    Recursive Feature Elimination (RFE) is a feature selection method
+    used in machine learning. It works by recursively removing the least
+    important features based on a given model's feature importance or
+    coefficients. RFE starts with all features and eliminates a specified
+    number or fraction of features at each step. The process continues
+    until the desired number of features is reached. This method helps in
+    enhancing model performance and interpretability by reducing complexity.
+
+    Parameters
+    ----------
+    `estimator` : An estimator to fit and evaluate
+    `n_features` : Number of features to select (`0~1` value for proportion)
+    `metric` : Scoring metric for selecting features
+    `step_size` : Number of features to eliminate in each step
+    `cv` : K-fold size for cross validation (`0` to disable CV)
+    `shuffle` : Whether to shuffle the dataset
+    `fold_type` : Fold type (Default `KFold`)
+    `random_state` : Seed for splitting the data
+
+    Notes
+    -----
+    * An instance of the estimator must be passed to `estimator`
+    * Do not use the estimator for `RFE` if it is supposed to be the
+        main estimator for the model
+    * For `metric`, both class or instance are possible
+
+    Examples
+    --------
+    >>> rfe = RFE(estimator=AnyEstimator(),
+                  n_features=0.25,
+                  metric=AnyEvaluator,
+                  step_size=1,
+                  cv=5,
+                  random_state=None)
+    >>> rfe.fit(X, y)
+    >>> Z = rfe.transform(X)
+
+    """
+
+    def __init__(
+        self,
+        estimator: Estimator = None,
+        n_features: int | float = 1,
+        metric: Evaluator = None,
+        step_size: int = 1,
+        cv: int = 5,
+        shuffle: bool = True,
+        fold_type: FoldType = KFold,
+        random_state: int = None,
+        verbose: bool = False,
+    ) -> None:
+        self.estimator = estimator
+        self.n_features = n_features
+        self.metric = metric
+        self.step_size = step_size
+        self.cv = cv
+        self.shuffle = shuffle
+        self.fold_type = fold_type
+        self.random_state = random_state
+        self.verbose = verbose
+        self._fitted = False
+
+    def fit(self, X: Matrix, y: Vector) -> "RFE":
+        _, n = X.shape
+        self.estimator = Clone(self.estimator).get
+
+        if 0 < self.n_features < 1:
+            self.n_features = np.floor(n * self.n_features).astype(int)
+        elif self.n_features <= 0 or self.n_features > n:
+            raise UnsupportedParameterError(self.n_features)
+
+        self.cv_model = CrossValidator(
+            estimator=self.estimator,
+            metric=self.metric,
+            cv=self.cv,
+            shuffle=self.shuffle,
+            fold_type=self.fold_type,
+            random_state=self.random_state,
+        )
+
+        self.support = np.ones(n, dtype=bool)
+        self.ranking = np.ones(n, dtype=int)
+
+        while np.sum(self.support) > self.n_features:
+            scores = self._calculate_score(X, y)
+            indices = np.argsort(scores)[::-1][: self.step_size]
+            self.support[indices] = False
+            self.ranking[indices] += 1
+
+            if self.verbose:
+                print(
+                    f"[RFE] Removed {self.step_size} features,",
+                    f"remaining features: {np.sum(self.support)}",
+                    f"with best-score: {scores[:self.step_size]}",
+                )
+
+        features = tuple(i for i, sup in enumerate(self.support) if sup)
+        if self.verbose:
+            print(f"[RFE] Elimination finished with final features: {features}")
+
+        self._fitted = True
+        return self
+
+    def _calculate_score(self, X: Matrix, y: Vector) -> Vector[float]:
+        scores = np.zeros(X.shape[1])
+        for i in range(X.shape[1]):
+            if not self.support[i]:
+                continue
+            indices = self.support.copy()
+            indices[i] = False
+
+            if self.cv:
+                _, score = self.cv_model.score(X[:, indices], y)
+            else:
+                self.estimator.fit(X[:, indices], y)
+                y_pred = self.estimator.predict(X[:, indices])
+                score = self.metric.score(y_true=y, y_pred=y_pred)
+
+            scores[i] = score
+
+        return scores
+
+    def transform(self, X: Matrix) -> Matrix:
+        if not self._fitted:
+            raise NotFittedError(self)
+        return X[:, self.support]
+
+    def fit_transform(self, X: Matrix, y: Vector) -> Matrix:
+        self.fit(X, y)
+        return self.transform(X)
```

### Comparing `luma-ml-0.6.4/luma/ensemble/vote.py` & `luma-ml-0.6.5/luma/ensemble/vote.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,179 +5,180 @@
 from luma.interface.util import Matrix, Vector, Scalar, Clone
 from luma.interface.exception import NotFittedError, UnsupportedParameterError
 from luma.metric.classification import Accuracy
 from luma.metric.regression import MeanSquaredError
 from luma.preprocessing.encoder import LabelEncoder
 
 
-__all__ = (
-    'VotingClassifier',
-    'VotingRegressor'
-)
+__all__ = ("VotingClassifier", "VotingRegressor")
 
 
 class VotingClassifier(Estimator, Estimator.Meta, Supervised):
-    
     """
-    A Voting Classifier is an ensemble machine learning model that combines 
-    predictions from multiple base models. It uses a voting mechanism, either 
-    'hard' (majority rule) or 'soft' (weighted probabilities), to determine 
-    the final output. This approach can increase prediction accuracy and 
-    robustness by leveraging the strengths of diverse models. It's 
-    particularly useful when individual models have different error patterns. 
-    The Voting Classifier is widely used in classification tasks to improve 
+    A Voting Classifier is an ensemble machine learning model that combines
+    predictions from multiple base models. It uses a voting mechanism, either
+    'hard' (majority rule) or 'soft' (weighted probabilities), to determine
+    the final output. This approach can increase prediction accuracy and
+    robustness by leveraging the strengths of diverse models. It's
+    particularly useful when individual models have different error patterns.
+    The Voting Classifier is widely used in classification tasks to improve
     performance over single models.
-    
+
     Parameters
     ----------
     `estimators` : List of estimators to vote
     `voting` : Voting criterion
     (`label` to vote the most frequent and `prob` to vote the most probable)
     `weights` : Weights for each classifier on voting
     (`None` for uniform weights)
-    
+
     Examples
     --------
-    >>> vot = VotingClassifier(estimators=[AnyClassifier(), ...], 
+    >>> vot = VotingClassifier(estimators=[AnyClassifier(), ...],
                                voting='label',
                                weights=[0.25, 0.5, ...])
     >>> vot.fit(X, y)
     >>> pred = vot.predict(X)
     >>> clf = vot[i] # Get i-th classifier from `vot`
-    
+
     """
-    
-    def __init__(self,
-                 estimators: List[Estimator] = None,
-                 voting: Literal['label', 'prob'] = 'label',
-                 weights: Vector[Scalar] = None,
-                 verbose: bool = False) -> None:
+
+    def __init__(
+        self,
+        estimators: List[Estimator] = None,
+        voting: Literal["label", "prob"] = "label",
+        weights: Vector[Scalar] = None,
+        verbose: bool = False,
+    ) -> None:
         self.estimators = estimators
         self.voting = voting
         self.weights = weights
         self.verbose = verbose
         self._fitted = False
-    
-    def fit(self, X: Matrix, y: Vector) -> 'VotingClassifier':
-        if self.voting not in ('label', 'prob'):
+
+    def fit(self, X: Matrix, y: Vector) -> "VotingClassifier":
+        if self.voting not in ("label", "prob"):
             raise UnsupportedParameterError(self.voting)
-        
+
         if self.weights and len(self.weights) != len(self.estimators):
             raise ValueError(f"Size mismatch between 'weights' and 'estimators'!")
-        
+
         self.le = LabelEncoder()
         self.le.fit(y)
-        
+
         self.classes = self.le.classes
         self.estimators_ = []
-        
+
         for est in self.estimators:
             fitted_est = Clone(est).get
-            if hasattr(fitted_est, 'verbose'):
+            if hasattr(fitted_est, "verbose"):
                 fitted_est.verbose = self.verbose
-            
+
             fitted_est.fit(X, self.le.transform(y))
             self.estimators_.append(fitted_est)
-        
+
         self._fitted = True
         return self
-    
+
     def predict(self, X: Matrix) -> Vector:
-        if not self._fitted: raise NotFittedError(self)
-        
-        if self.voting == 'label':
+        if not self._fitted:
+            raise NotFittedError(self)
+
+        if self.voting == "label":
             preds = np.asarray([est.predict(X) for est in self.estimators_]).T
             majority_vote = np.apply_along_axis(
                 lambda x: np.argmax(np.bincount(x, weights=self.weights)),
                 axis=1,
-                arr=preds
+                arr=preds,
             )
         else:
             majority_vote = np.argmax(self.predict_proba(X), axis=1)
-        
+
         majority_vote = self.le.inverse_transform(majority_vote)
         return majority_vote
-    
+
     def predict_proba(self, X: Matrix) -> Matrix:
         probas = []
         for est in self.estimators_:
-            if not hasattr(est, 'predict_proba'):
+            if not hasattr(est, "predict_proba"):
                 raise ValueError(f"'{type(est)}' does not support 'predict_proba'")
             probas.append(est.predict_proba(X))
-        
+
         return np.average(probas, axis=0, weights=self.weights)
 
     def score(self, X: Matrix, y: Vector, metric: Evaluator = Accuracy) -> float:
         X_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=X_pred)
 
     def __getitem__(self, index: int) -> Estimator:
         return self.estimators_[index]
 
 
 class VotingRegressor(Estimator, Estimator.Meta, Supervised):
-    
     """
-    A Voting Regressor is an ensemble machine learning model that combines 
-    predictions from multiple base regression models. It uses a voting mechanism, 
-    where the final output is the average of the predictions from all models. 
-    This approach can increase prediction accuracy and robustness by leveraging 
-    the strengths of diverse models. It's particularly useful when individual 
-    models have different error patterns. The Voting Regressor is widely used in 
+    A Voting Regressor is an ensemble machine learning model that combines
+    predictions from multiple base regression models. It uses a voting mechanism,
+    where the final output is the average of the predictions from all models.
+    This approach can increase prediction accuracy and robustness by leveraging
+    the strengths of diverse models. It's particularly useful when individual
+    models have different error patterns. The Voting Regressor is widely used in
     regression tasks to improve performance over single models.
-    
+
     Parameters
     ----------
     `estimators` : List of regressors to vote
     `weights` : Weights for each regressor on voting
     (`None` for uniform weights)
-    
+
     Examples
     --------
-    >>> vot = VotingRegressor(estimators=[AnyRegressor(), ...], 
+    >>> vot = VotingRegressor(estimators=[AnyRegressor(), ...],
                               weights=[0.25, 0.5, ...])
     >>> vot.fit(X, y)
     >>> pred = vot.predict(X)
     >>> reg = vot[i] # Get i-th regressor from `vot`
-    
+
     """
-    
-    def __init__(self,
-                 estimators: List[Estimator] = None,
-                 weights: Vector[Scalar] = None,
-                 verbose: bool = False) -> None:
+
+    def __init__(
+        self,
+        estimators: List[Estimator] = None,
+        weights: Vector[Scalar] = None,
+        verbose: bool = False,
+    ) -> None:
         self.estimators = estimators
         self.weights = weights
         self.verbose = verbose
         self._fitted = False
-    
-    def fit(self, X: Matrix, y: Vector) -> 'VotingRegressor':
+
+    def fit(self, X: Matrix, y: Vector) -> "VotingRegressor":
         if self.weights and len(self.weights) != len(self.estimators):
             raise ValueError(f"Size mismatch between 'weights' and 'estimators'!")
-        
+
         self.estimators_ = []
         for est in self.estimators:
             fitted_est = Clone(est).get
-            if hasattr(fitted_est, 'verbose'):
+            if hasattr(fitted_est, "verbose"):
                 fitted_est.verbose = self.verbose
-            
+
             fitted_est.fit(X, y)
             self.estimators_.append(fitted_est)
-        
+
         self._fitted = True
         return self
-    
+
     def predict(self, X: Matrix) -> Vector:
-        if not self._fitted: raise NotFittedError(self)
-        
+        if not self._fitted:
+            raise NotFittedError(self)
+
         predictions = np.asarray([est.predict(X) for est in self.estimators_])
         avg_predictions = np.average(predictions, axis=0, weights=self.weights)
         return avg_predictions
 
-    def score(self, X: Matrix, y: Vector, 
-              metric: Evaluator = MeanSquaredError) -> float:
+    def score(
+        self, X: Matrix, y: Vector, metric: Evaluator = MeanSquaredError
+    ) -> float:
         X_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=X_pred)
 
     def __getitem__(self, index: int) -> Estimator:
         return self.estimators_[index]
-
```

### Comparing `luma-ml-0.6.4/luma/interface/util.py` & `luma-ml-0.6.5/luma/interface/util.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,400 +1,519 @@
-from typing import Any, Callable, Literal
+from typing import Any, AnyStr, Callable, Literal, Type, TypeGuard
 import numpy as np
 
-from luma.core.super import Estimator, Transformer
-from luma.interface.exception import UnsupportedParameterError
+from luma.interface.exception import UnsupportedParameterError, InvalidRangeError
 from luma.neural import activation
 
 
 __all__ = (
-    'Matrix', 
-    'Vector', 
-    'Scalar', 
-    'DecisionTreeNode', 
-    'NearestNeighbors', 
-    'SilhouetteUtil', 
-    'DBUtil',
-    'KernelUtil',
-    'ActivationUtil', 
-    'Clone'
+    "Matrix",
+    "Vector",
+    "Scalar",
+    "DecisionTreeNode",
+    "NearestNeighbors",
+    "SilhouetteUtil",
+    "DBUtil",
+    "KernelUtil",
+    "ActivationUtil",
+    "Clone",
+    "ParamRange",
 )
 
 
 class Matrix(np.ndarray):
-
     """
     Internal class that extends `numpy.ndarray`.
 
-    This class provides a way to create matrix objects that have 
-    all the capabilities of numpy arrays with the potential for 
-    additional functionalities and readability.s
-    
+    This class provides a way to create matrix objects that have
+    all the capabilities of numpy arrays with the potential for
+    additional functionalities and readability.
+
     Example
     -------
     >>> m = Matrix([1, 2, 3])
     >>> isinstance(m, numpy.ndarray) # True
-    
+
     """
-    
-    def __new__(cls, array_like: Any) -> 'Matrix':
-        if isinstance(array_like, list): obj = np.array(array_like)
-        else: obj = array_like    
+
+    def __new__(cls, array_like: Any) -> "Matrix":
+        if isinstance(array_like, (list, np.matrix)):
+            obj = np.array(array_like)
+        else:
+            obj = array_like
         return obj
 
     def __array_finalize__(self, obj: np.ndarray | None) -> None:
-        if obj is None: return
+        if obj is None:
+            return
 
 
 class Vector(Matrix):
-    
     """
     Internal class for vector that extends `Matrix`.
-    
+
     This class represents a single row/column vector with its
     type of `numpy.ndarray` or `Matrix`.
-    
+
     """
-    
-    def __new__(cls, array_like: Any) -> 'Vector':
-        if isinstance(array_like, list): obj = Matrix(array_like)
-        else: obj = array_like    
+
+    def __new__(cls, array_like: Any) -> "Vector":
+        if isinstance(array_like, list):
+            obj = Matrix(array_like)
+        else:
+            obj = array_like
         return obj
 
 
 class Scalar:
-    
     """
     A placeholder class for scalar type.
-    
+
     This class encompasses `int` and `float`.
     """
-    
-    def __new__(cls, value: int | float) -> 'Scalar':
+
+    def __new__(cls, value: int | float) -> "Scalar":
         return float(value)
 
 
 class DecisionTreeNode:
-    
     """
     Internal class for node used in tree-based models.
-    
+
     Parameters
     ----------
     `feature_index` : Feature of node
     `threshold` : Threshold for split point
     `left` : Left-child node
     `right` : Right-child node
     `value` : Most popular label of leaf node
-    
+
     """
-    
-    def __init__(self,
-                 feature_index: int = None,
-                 threshold: float = None,
-                 left: 'DecisionTreeNode' = None,
-                 right: 'DecisionTreeNode' = None,
-                 value: Any = None) -> None:
+
+    def __init__(
+        self,
+        feature_index: int = None,
+        threshold: float = None,
+        left: "DecisionTreeNode" = None,
+        right: "DecisionTreeNode" = None,
+        value: Any = None,
+    ) -> None:
         self.feature_index = feature_index
         self.threshold = threshold
         self.left = left
         self.right = right
         self.value = value
 
     @property
     def isLeaf(self) -> bool:
         return self.value is not None
 
 
 class NearestNeighbors:
-    
     """
     Internal class for computing nearest neighbors of given data.
-    
+
     Parameters
     ----------
     `data` : Data to be handled
     `n_neighbors` : Number of nearest neighbors
-    
+
     """
-    
-    def __init__(self,
-                 data: Matrix,
-                 n_neighbors: int) -> None:
+
+    def __init__(self, data: Matrix, n_neighbors: int) -> None:
         self.data = data
         self.n_neighbors = n_neighbors
         self._size = data.shape[0]
-    
+
     @property
     def index_matrix(self) -> Matrix:
         data = self.data
         dist = np.linalg.norm(data[:, np.newaxis, :] - data, axis=2)
         sorted_indices = np.argsort(dist, axis=1)
-        return sorted_indices[:, 1:self.n_neighbors + 1]
-    
+        return sorted_indices[:, 1 : self.n_neighbors + 1]
+
     @property
     def adjacent_matrix(self) -> Matrix:
         indices = self.index_matrix
         adj_mat = np.zeros((self._size, self._size))
         for i in range(self._size):
             adj_mat[i, indices[i]] = 1
-        
+
         return adj_mat.astype(int)
 
 
 class SilhouetteUtil:
-    
     """
-    Internal class for computing various distances used in 
+    Internal class for computing various distances used in
     Silhouette Coefficient calculation.
-    
+
     Parameters
     ----------
     `idx` : Index of a single data point
     `cluster` : Current cluster number
     `labels` : Labels assigned by clustering estimator
     `distances` : Square-form distance matrix of the data
-    
+
     """
-    
-    def __init__(self, 
-                 idx: int,
-                 cluster: int,
-                 labels: Matrix,
-                 distances: Matrix) -> None:
+
+    def __init__(
+        self, idx: int, cluster: int, labels: Matrix, distances: Matrix
+    ) -> None:
         self.idx = idx
         self.cluster = cluster
         self.labels = labels
         self.distances = distances
 
     @property
     def avg_dist_others(self) -> Matrix:
         others = set(self.labels) - {self.cluster}
-        sub_avg = [np.mean(self.distances[self.idx][self.labels == other]) 
-                   for other in others]
+        sub_avg = [
+            np.mean(self.distances[self.idx][self.labels == other]) for other in others
+        ]
 
         return np.mean(sub_avg)
 
     @property
     def avg_dist_within(self) -> Matrix | int:
         within_cluster = self.distances[self.idx][self.labels == self.cluster]
-        if len(within_cluster) <= 1: return 0
+        if len(within_cluster) <= 1:
+            return 0
         return np.mean([dist for dist in within_cluster if dist != 0])
 
 
 class DBUtil:
-    
     """
     Internal class for supporting Davies-Bouldin Index (DBI) computation.
-    
+
     Parameters
     ----------
     `data` : Original data
     `labels` : Labels assigned by clustering estimator
-    
+
     """
-    
-    def __init__(self,
-                 data: Matrix, 
-                 labels: Matrix) -> None:
+
+    def __init__(self, data: Matrix, labels: Matrix) -> None:
         self.data = data
         self.labels = labels
-    
+
     @property
     def cluster_centroids(self) -> Matrix:
         unique_labels = np.unique(self.labels)
-        centroids = [self.data[self.labels == label].mean(axis=0) 
-                     for label in unique_labels]
+        centroids = [
+            self.data[self.labels == label].mean(axis=0) for label in unique_labels
+        ]
         return Matrix(centroids)
 
     @property
     def within_cluster_scatter(self) -> Matrix:
         centroids = self.cluster_centroids
         scatter = np.zeros(len(centroids))
-        
+
         for i, centroid in enumerate(centroids):
             cluster_points = self.data[self.labels == i]
-            diff_sq =  (cluster_points - centroid) ** 2
+            diff_sq = (cluster_points - centroid) ** 2
             scatter[i] = np.mean(np.sqrt(np.sum(diff_sq, axis=1)))
-            
+
         return scatter
 
     @property
     def separation(self) -> Matrix:
         centroids = self.cluster_centroids
         n_clusters = len(centroids)
         separation = np.zeros((n_clusters, n_clusters))
-        
+
         for i in range(n_clusters):
             for j in range(n_clusters):
-                if i == j: continue
+                if i == j:
+                    continue
                 diff_sq = (centroids[i] - centroids[j]) ** 2
                 separation[i, j] = np.sqrt(np.sum(diff_sq))
-                    
+
         return separation
 
 
 class KernelUtil:
-    
     """
     Internal class for kernel methods(tricks).
-    
+
     This class facilitates transferring kernel type strings
     into actual specific kernel function.
-    
+
     Example
     -------
     >>> util = KernelUtil(kernel='rbf', **params)
     >>> util.kernel_func
     KernelUtil.rbf_kernel: Callable[[Matrix, Matrix | None], Matrix]
-    
+
     """
-    
-    func_type = Literal['lin' ,'linear',
-                        'poly', 'polynoimal',
-                        'rbf', 'gaussian', 'Gaussian',
-                        'tanh', 'sigmoid',
-                        'lap', 'laplacian']
-    
-    def __init__(self, 
-                 kernel: str,
-                 alpha: float = 1.0,
-                 gamma: float = 1.0,
-                 coef: float = 0.0,
-                 deg: int = 2) -> None:
+
+    FuncType = Literal[
+        "lin",
+        "linear",
+        "poly",
+        "polynoimal",
+        "rbf",
+        "gaussian",
+        "Gaussian",
+        "tanh",
+        "sigmoid",
+        "lap",
+        "laplacian",
+    ]
+
+    def __init__(
+        self,
+        kernel: str,
+        alpha: float = 1.0,
+        gamma: float = 1.0,
+        coef: float = 0.0,
+        deg: int = 2,
+    ) -> None:
         self.kernel = kernel
         self.alpha = alpha
         self.gamma = gamma
         self.coef = coef
         self.deg = deg
-    
+
     def linear_kernel(self, Xi: Matrix, Xj: Matrix = None) -> Matrix:
-        if Xj is None: Xj = Xi.copy()
+        if Xj is None:
+            Xj = Xi.copy()
         return np.dot(Xi, Xj.T)
-    
+
     def polynomial_kernel(self, Xi: Matrix, Xj: Matrix = None) -> Matrix:
-        if Xj is None: Xj = Xi.copy()
+        if Xj is None:
+            Xj = Xi.copy()
         return (self.gamma * np.dot(Xi, Xj.T) + self.coef) ** self.deg
-    
+
     def rbf_kernel(self, Xi: Matrix, Xj: Matrix = None) -> Matrix:
-        if Xj is None: Xj = Xi.copy()
-        _left = np.sum(Xi ** 2, axis=1).reshape(-1, 1)
-        _right = np.sum(Xj ** 2, axis=1) - 2 * np.dot(Xi, Xj.T)
-        
+        if Xj is None:
+            Xj = Xi.copy()
+        _left = np.sum(Xi**2, axis=1).reshape(-1, 1)
+        _right = np.sum(Xj**2, axis=1) - 2 * np.dot(Xi, Xj.T)
+
         return np.exp(-self.gamma * (_left + _right))
-    
+
     def sigmoid_kernel(self, Xi: Matrix, Xj: Matrix = None) -> Matrix:
-        if Xj is None: Xj = Xi.copy()
+        if Xj is None:
+            Xj = Xi.copy()
         return np.tanh(self.gamma * np.dot(Xi, Xj.T) + self.coef)
-    
+
     def laplacian_kernel(self, Xi: Matrix, Xj: Matrix = None) -> Matrix:
-        if Xj is None: Xj = Xi.copy()
+        if Xj is None:
+            Xj = Xi.copy()
         manhattan_dists = np.sum(np.abs(Xi[:, np.newaxis] - Xj), axis=2)
-        
+
         return np.exp(-self.gamma * manhattan_dists)
-    
+
     @property
     def kernel_func(self) -> Callable[[Matrix, Matrix | None], Matrix]:
-        if self.kernel in ('linear', 'lin'):
+        if self.kernel in ("linear", "lin"):
             return self.linear_kernel
-        elif self.kernel in ('poly', 'polynomial'):
+        elif self.kernel in ("poly", "polynomial"):
             return self.polynomial_kernel
-        elif self.kernel in ('rbf', 'gaussian', 'Gaussian'):
+        elif self.kernel in ("rbf", "gaussian", "Gaussian"):
             return self.rbf_kernel
-        elif self.kernel in ('sigmoid', 'tanh'):
+        elif self.kernel in ("sigmoid", "tanh"):
             return self.sigmoid_kernel
-        elif self.kernel in ('laplacian', 'lap'):
+        elif self.kernel in ("laplacian", "lap"):
             return self.laplacian_kernel
         else:
             raise UnsupportedParameterError(self.kernel)
 
 
 class ActivationUtil:
-    
     """
     Internal class for activaiton functions used in neural networks.
-    
+
     Properties
     ----------
     For getting an activation function class:
         ```py
         @property
         def activation_type(self) -> type
         ```
-    
+
     Examples
     --------
     >>> act = ActivationUtil(activation='relu')
     >>> relu = act.activation_type
     ReLU()
-    
+
     """
-    
-    func_type = Literal['relu', 'ReLU',
-                        'leaky-relu', 'leaky-ReLU',
-                        'elu', 'ELU', 
-                        'tanh', 
-                        'sigmoid', 'sig',
-                        'softmax']
-    
+
+    FuncType = Literal[
+        "relu",
+        "ReLU",
+        "leaky-relu",
+        "leaky-ReLU",
+        "elu",
+        "ELU",
+        "tanh",
+        "sigmoid",
+        "sig",
+        "softmax",
+    ]
+
     def __init__(self, activation: str) -> None:
         self.activation = activation
-    
+
     @property
     def activation_type(self) -> type:
-        if self.activation in ('relu', 'ReLU'): 
+        if self.activation in ("relu", "ReLU"):
             return activation.ReLU
-        elif self.activation in ('leaky-relu', 'leaky-ReLU'): 
+        elif self.activation in ("leaky-relu", "leaky-ReLU"):
             return activation.LeakyReLU
-        elif self.activation in ('elu', 'ELU'): 
+        elif self.activation in ("elu", "ELU"):
             return activation.ELU
-        elif self.activation in ('tanh'): 
+        elif self.activation in ("tanh"):
             return activation.Tanh
-        elif self.activation in ('sigmoid', 'sig'): 
+        elif self.activation in ("sigmoid", "sig"):
             return activation.Sigmoid
-        elif self.activation in ('softmax'):
+        elif self.activation in ("softmax"):
             return activation.Softmax
 
 
 class Clone:
-    
     """
     A utility class for cloning LUMA models.
 
-    This class creates a copy of a given LUMA model, 
-    which can be either an Estimator or a Transformer. 
-    The clone includes all parameters of the original model. 
-    Optionally, the trained state of the model can also be copied 
+    This class creates a copy of a given LUMA model,
+    which can be either an Estimator or a Transformer.
+    The clone includes all parameters of the original model.
+    Optionally, the trained state of the model can also be copied
     if applicable.
 
     Parameters
     ----------
     `model` : The model to be cloned
     `pass_fitted` : Whether to copy the fitted state of the original model
-    
+
     Examples
     --------
     >>> original_model = AnyModel(...)
     >>> cloned_model = Clone(model=original_model, pass_fitted=True).get
 
     """
-    
-    def __init__(self,
-                 model: Estimator | Transformer = None,
-                 pass_fitted: bool = False) -> None:
+
+    def __init__(self, model: object = None, pass_fitted: bool = False) -> None:
         self.model = model
         self.pass_fitted = pass_fitted
-    
+
     @property
-    def get(self) -> Estimator | Transformer:
+    def get(self) -> object:
         model_cls = type(self.model)
         new_model = model_cls()
-        
+
         for param, val in self.model.__dict__.items():
-            try: new_model.set_params(**{param: val})
-            except: continue
-        
-        if hasattr(self.model, '_fitted') and self.pass_fitted:
+            try:
+                new_model.set_params(**{param: val})
+            except:
+                continue
+
+        if hasattr(self.model, "_fitted") and self.pass_fitted:
             new_model._fitted = self.model._fitted
-        
+
         return new_model
 
+
+class ParamRange:
+    """
+    A utility class for setting and checking the range of a specific parameter.
+
+    This class provides a user-friendly functionality which checks whether
+    a certain parameter value falls within its preferred numerical range
+    depending on its algorithm.
+
+    Parameters
+    ----------
+    `param_range` : An interval of a parameter (customizable)
+    `param_type` : Data type of a parameter to be forced to have
+    (`None` for both `int` and `float` types)
+
+    Method
+    ------
+    To check its validity:
+    ```py
+    def check(self, param_value: Any) -> None
+    ```
+    Raises
+    ------
+    - `InvalidRangeError` :
+        When the parameter does not fall in its preferred range
+    - `UnsupportedParameterError` :
+        When the parameter is not numeric or has wrong numeric type
+
+    Examples
+    --------
+    ```py
+    class SomeModel:
+        def __init__(self, a: int) -> None:
+            self.a = a
+            a_range = ParamRange(param_range="0,+inf", param_type=int)
+            a_range.check(param_value=self.a)
+    ```
+    Notes
+    -----
+    - When setting a custom range for `param_range`, it must follow the form of
+        "lower_bound,upper_bound". (i.e. `-inf,20`, `-5,5`)
+    - For open intervals, add '<' inside the range. (i.e. `0<,+inf`, `0<,<10`)
+    """
+
+    Ranges = Literal["-inf,+inf", "-inf,0", "-1,0", "-1,1", "0,1", "0,+inf"]
+
+    def __init__(
+        self, param_range: Ranges | AnyStr, param_type: Type[Scalar] = None
+    ) -> None:
+        self.param_range = param_range
+
+        if param_type is None:
+            self.param_type = int | float
+        else:
+            if not ParamRange.validate_type(param_type):
+                raise UnsupportedParameterError(param_type)
+            self.param_type = param_type
+
+    @classmethod
+    def validate_type(cls, param_type) -> TypeGuard[Scalar]:
+        return param_type in (int, float)
+
+    def check(self, param_name: str, param_value: Any) -> None:
+        if param_value is None:
+            return
+        self._type_check(param_value)
+        if not self.condition(param_value):
+            raise InvalidRangeError(param_value, param_name, self.param_range)
+
+    def _type_check(self, param_value: Any) -> None:
+        if not isinstance(param_value, self.param_type):
+            raise UnsupportedParameterError(param_value)
+
+    @property
+    def condition(self) -> Callable[[Scalar], bool]:
+        try:
+            left, right = self.param_range.split(",")
+        except:
+            raise UnsupportedParameterError(self.param_range)
+
+        lower_open, upper_open = False, False
+        if left[-1] == "<":
+            lower_open = True
+            lower = np.float64(left[:-1])
+        else:
+            lower = np.float64(left)
+
+        if right[0] == "<":
+            upper_open = True
+            upper = np.float64(right[1:])
+        else:
+            upper = np.float64(right)
+
+        if lower_open and not upper_open:
+            return lambda x: lower < x <= upper
+        elif lower_open and upper_open:
+            return lambda x: lower < x < upper
+        elif not lower_open and upper_open:
+            return lambda x: lower <= x < upper
+        elif not lower_open and not upper_open:
+            return lambda x: lower <= x <= upper
+        else:
+            NotImplemented
```

### Comparing `luma-ml-0.6.4/luma/metric/classification.py` & `luma-ml-0.6.5/luma/metric/classification.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,14 @@
 import numpy as np
 
 from luma.interface.util import Matrix
 from luma.core.super import Evaluator
 
 
-__all__ = (
-    'Accuracy', 
-    'Precision', 
-    'Recall', 
-    'F1Score', 
-    'Specificity'
-)
+__all__ = ("Accuracy", "Precision", "Recall", "F1Score", "Specificity")
 
 
 class Accuracy(Evaluator):
     @staticmethod
     def score(y_true: Matrix, y_pred: Matrix) -> float:
         return np.mean(y_true == y_pred)
 
@@ -45,8 +39,7 @@
 
 class Specificity(Evaluator):
     @staticmethod
     def score(y_true: Matrix, y_pred: Matrix) -> float:
         true_negatives = np.sum((y_true == 0) & (y_pred == 0))
         false_positives = np.sum((y_true == 0) & (y_pred == 1))
         return true_negatives / (true_negatives + false_positives)
-
```

### Comparing `luma-ml-0.6.4/luma/metric/clustering.py` & `luma-ml-0.6.5/luma/metric/clustering.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,172 +3,175 @@
 import matplotlib.pyplot as plt
 import numpy as np
 
 from luma.core.super import Evaluator, Visualizer
 from luma.interface.util import Matrix, SilhouetteUtil, DBUtil
 
 
-__all__ = (
-    'SilhouetteCoefficient', 
-    'DaviesBouldin',
-    'Inertia'
-)
+__all__ = ("SilhouetteCoefficient", "DaviesBouldin", "Inertia")
 
 
 class SilhouetteCoefficient(Evaluator, Visualizer):
-    
     """
-    The Silhouette Coefficient is a measure used to evaluate the quality of 
-    clusters in a dataset. It calculates how similar each data point is to its 
-    own cluster compared to other clusters. The coefficient ranges from -1 
-    (poorly clustered) to +1 (well clustered), with values near 0 indicating 
-    overlapping clusters. High average scores across a dataset suggest clear, 
+    The Silhouette Coefficient is a measure used to evaluate the quality of
+    clusters in a dataset. It calculates how similar each data point is to its
+    own cluster compared to other clusters. The coefficient ranges from -1
+    (poorly clustered) to +1 (well clustered), with values near 0 indicating
+    overlapping clusters. High average scores across a dataset suggest clear,
     well-separated clusters.
-    
+
     Parameters
     ----------
     `data` : Original data
     `labels` : Labels assigned by clustering estimator
-    
+
     Examples
     --------
     With Instantiation
     ```py
         sil = SilhouetteCoefficient(data, labels)
         score = sil.score(data, labels) # compute() is a static method
         sil.plot(...)
     ```
-    
+
     Without Instantiation
     ```py
         score = SilhouetteCoefficient.score(data, labels)
         SilhouetteCoefficient.plot(...) # Error; plot() is an instance method
     ```
-    
+
     """
-    
+
     def __init__(self, data: Matrix, labels: Matrix) -> None:
         self.data = data
         self.labels = labels
         self.dist = squareform(pdist(self.data))
-    
+
     @staticmethod
     def score(data: Matrix, labels: Matrix) -> Matrix[float]:
         scores = []
         dist = squareform(pdist(data))
         for idx, label in enumerate(labels):
             util = SilhouetteUtil(idx, label, labels, dist)
             a = util.avg_dist_within
             b = util.avg_dist_others
             score = (b - a) / max(a, b) if max(a, b) != 0 else 0
             scores.append(score)
 
         return np.mean(scores)
-    
+
     def _individual_silhouette(self) -> Matrix:
         silhouette_values = []
         for idx, label in enumerate(self.labels):
             util = SilhouetteUtil(idx, label, self.labels, self.dist)
             a = util.avg_dist_within
             b = util.avg_dist_others
             score = (b - a) / max(a, b) if max(a, b) != 0 else 0
             silhouette_values.append(score)
-        
+
         return Matrix(silhouette_values)
 
     def plot(self, ax: Optional[plt.Axes] = None, show: bool = False) -> plt.Axes:
-        if ax is None: _, ax = plt.subplots()
+        if ax is None:
+            _, ax = plt.subplots()
+            show = True
+
         sample_silhouette = self._individual_silhouette()
         y_lower = 10
-        
+
         for i in range(len(np.unique(self.labels))):
             values = sample_silhouette[self.labels == i]
             values.sort()
 
             size_cluster_i = values.shape[0]
             y_upper = y_lower + size_cluster_i
 
             color = plt.cm.nipy_spectral(float(i) / len(set(self.labels)))
-            ax.fill_betweenx(np.arange(y_lower, y_upper), 0, values,
-                            facecolor=color, edgecolor=color, alpha=0.7)
+            ax.fill_betweenx(
+                np.arange(y_lower, y_upper),
+                0,
+                values,
+                facecolor=color,
+                edgecolor=color,
+                alpha=0.7,
+            )
             y_lower = y_upper + 10
-        
+
         ax.set_title("Silhouette Coefficient Plot")
         ax.set_xlabel("Silhouette coefficient values")
         ax.set_ylabel("Cluster label")
-        ax.axvline(x=self.score(self.data, self.labels), 
-                   color="red", linestyle="--")
-        
+        ax.axvline(x=self.score(self.data, self.labels), color="red", linestyle="--")
+
         ax.set_yticks([])
         ax.set_xticks(np.arange(0.0, 1.2, 0.1))
         plt.tight_layout()
 
-        if show: plt.show()
+        if show:
+            plt.show()
         return ax
 
 
 class DaviesBouldin(Evaluator):
-    
     """
-    The Davies-Bouldin Index (DBI) is a metric for evaluating clustering 
-    algorithms. It compares the average distance within clusters to the 
-    distance between clusters. Lower DBI values indicate better clustering, 
+    The Davies-Bouldin Index (DBI) is a metric for evaluating clustering
+    algorithms. It compares the average distance within clusters to the
+    distance between clusters. Lower DBI values indicate better clustering,
     with compact and well-separated clusters.
-    
+
     Parameters
     ----------
     `data` : Original data
     `labels` : Labels assigned by clustering estimator
-    
+
     """
-    
+
     @staticmethod
     def score(data: Matrix, labels: Matrix) -> float:
         util = DBUtil(data=data, labels=labels)
         centroids = util.cluster_centroids
         scatter = util.within_cluster_scatter
         separation = util.separation
 
         n_clusters = len(centroids)
         db_values = np.zeros(n_clusters)
 
         for i in range(n_clusters):
             max_ratio = 0
             for j in range(n_clusters):
-                if i == j: continue
+                if i == j:
+                    continue
                 ratio = (scatter[i] + scatter[j]) / separation[i, j]
-                if ratio > max_ratio: max_ratio = ratio
-            
+                if ratio > max_ratio:
+                    max_ratio = ratio
+
             db_values[i] = max_ratio
         db_index = np.mean(db_values)
-        
+
         return db_index
 
 
 class Inertia(Evaluator):
-    
     """
-    Inertia in clustering quantifies the compactness of clusters by measuring 
-    the sum of squared distances between data points and their respective 
-    cluster centroids. It serves as a key metric to evaluate the quality of 
-    cluster assignments in algorithms like K-means. A lower inertia value 
-    indicates more cohesive clusters, where data points are closer to their 
-    centroids. However, minimizing inertia excessively can lead to overfitting, 
+    Inertia in clustering quantifies the compactness of clusters by measuring
+    the sum of squared distances between data points and their respective
+    cluster centroids. It serves as a key metric to evaluate the quality of
+    cluster assignments in algorithms like K-means. A lower inertia value
+    indicates more cohesive clusters, where data points are closer to their
+    centroids. However, minimizing inertia excessively can lead to overfitting,
     with a large number of clusters.
-    
+
     Parameters
     ----------
     `data` : Original data
     `centroids`: Centroids(or medoids for certain algorithm)
-    
+
     """
-    
+
     @staticmethod
     def score(data: Matrix, centroids: Matrix) -> float:
         sq_dist = (data[:, np.newaxis, :] - centroids[np.newaxis, :, :]) ** 2
         dist = np.sqrt(sq_dist.sum(axis=2))
-        
+
         closest = np.argmin(dist, axis=1)
         inertia = sum((dist[i, closest[i]] ** 2) for i in range(len(data)))
 
         return inertia
-
```

### Comparing `luma-ml-0.6.4/luma/metric/distance.py` & `luma-ml-0.6.5/luma/metric/distance.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-from typing import *
 import numpy as np
 
 from luma.interface.util import Matrix
 from luma.core.super import Distance
 
 
 __all__ = (
-    'Euclidean', 
-    'Manhattan', 
-    'Chebyshev', 
-    'Minkowski', 
-    'CosineSimilarity', 
-    'Correlation', 
-    'Mahalanobis'
+    "Euclidean",
+    "Manhattan",
+    "Chebyshev",
+    "Minkowski",
+    "CosineSimilarity",
+    "Correlation",
+    "Mahalanobis",
 )
 
 
 class Euclidean(Distance):
     @staticmethod
     def compute(x: Matrix, y: Matrix) -> float:
         return np.linalg.norm(x - y)
@@ -33,15 +32,16 @@
     def compute(x: Matrix, y: Matrix) -> float:
         return np.max(np.abs(x - y))
 
 
 class Minkowski(Distance):
     @staticmethod
     def compute(x: Matrix, y: Matrix, p: int | float) -> float:
-        if p is None: raise ValueError('[Minkowski] Empty p-value!'); return
+        if p is None:
+            raise ValueError("[Minkowski] Empty p-value!")
         return np.power(np.sum(np.abs(x - y) ** p), 1 / p)
 
 
 class CosineSimilarity(Distance):
     @staticmethod
     def compute(x: Matrix, y: Matrix) -> float:
         return 1 - (np.dot(x, y) / (np.linalg.norm(x) * np.linalg.norm(y)))
@@ -57,8 +57,7 @@
 class Mahalanobis(Distance):
     @staticmethod
     def compute(x: Matrix, y: Matrix, cov: Matrix) -> float:
         diff = x - y
         inv_covariance_matrix = np.linalg.inv(cov)
         mahalanobis_distance = np.sqrt(diff.T @ inv_covariance_matrix @ diff)
         return mahalanobis_distance
-
```

### Comparing `luma-ml-0.6.4/luma/metric/regression.py` & `luma-ml-0.6.5/luma/metric/regression.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 import numpy as np
 
 from luma.interface.util import Matrix
 from luma.core.super import Evaluator
 
 
 __all__ = (
-    'MeanAbsoluteError', 
-    'MeanSquaredError', 
-    'RootMeanSquaredError',
-    'MeanAbsolutePercentageError', 
-    'RSquaredScore'
+    "MeanAbsoluteError",
+    "MeanSquaredError",
+    "RootMeanSquaredError",
+    "MeanAbsolutePercentageError",
+    "RSquaredScore",
+    "AdjustedRSquaredScore",
 )
 
 
 class MeanAbsoluteError(Evaluator):
     @staticmethod
     def score(y_true: Matrix, y_pred: Matrix) -> float:
         return np.mean(np.abs(y_true - y_pred))
@@ -38,12 +39,23 @@
         return np.mean(np.abs((y_true - y_pred) / y_true)) * 100
 
 
 class RSquaredScore(Evaluator):
     @staticmethod
     def score(y_true: Matrix, y_pred: Matrix) -> float:
         y_bar = np.mean(y_true)
-        total_sum_of_squares = np.sum((y_true - y_bar) ** 2)
-        residual_sum_of_squares = np.sum((y_true - y_pred) ** 2)
-        r2 = 1 - (residual_sum_of_squares / total_sum_of_squares)
+        sst = np.sum((y_true - y_bar) ** 2)
+        ssr = np.sum((y_true - y_pred) ** 2)
+        r2 = 1 - (ssr / sst)
         return r2
 
+
+class AdjustedRSquaredScore(Evaluator):
+    @staticmethod
+    def score(y_true: Matrix, y_pred: Matrix, n_predictors: int) -> float:
+        m = len(y_true)
+        y_bar = np.mean(y_true)
+        sst = np.sum((y_true - y_bar) ** 2)
+        ssr = np.sum((y_true - y_pred) ** 2)
+        r2 = 1 - (ssr / sst)
+        r2_adj = 1 - ((1 - r2) * (m - 1) / (m - n_predictors - 1))
+        return r2_adj
```

### Comparing `luma-ml-0.6.4/luma/model_selection/cv.py` & `luma-ml-0.6.5/luma/model_selection/cv.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,94 +2,96 @@
 import numpy as np
 
 from luma.core.super import Estimator, Evaluator
 from luma.interface.util import Matrix, Vector
 from luma.model_selection.fold import FoldType, KFold
 
 
-__all__ = (
-    'CrossValidator'
-)
+__all__ = "CrossValidator"
 
 
 class CrossValidator(Evaluator):
-    
     """
-    Cross-validation is a technique in machine learning for assessing how 
-    a model generalizes to an independent dataset. It involves dividing 
-    the data into several parts, training the model on some parts and 
-    testing it on others. This process is repeated multiple times with 
-    different partitions, providing a robust estimate of the model's 
-    performance. It's especially useful in scenarios with limited data, 
-    ensuring that all available data is effectively utilized for both 
+    Cross-validation is a technique in machine learning for assessing how
+    a model generalizes to an independent dataset. It involves dividing
+    the data into several parts, training the model on some parts and
+    testing it on others. This process is repeated multiple times with
+    different partitions, providing a robust estimate of the model's
+    performance. It's especially useful in scenarios with limited data,
+    ensuring that all available data is effectively utilized for both
     training and validation.
-    
+
     Parameters
     ----------
     `estimator` : An estimator to validate
     `metric` : Evaluation metric for validation
     `cv` : Number of folds in splitting data
     `fold_type` : Fold type (Default `KFold`)
     `shuffle` : Whether to shuffle the dataset
     `random_state` : Seed for random sampling upon splitting data
-    
+
     Attributes
     ----------
     `train_scores_` : List of training scores for each fold
     `test_scores_` : List of test(validation) scores for each fold
-    
+
     Methods
     -------
     For getting mean train score and mean test score respectvely:
     ```py
         def score(self, X: Matrix, y: Vector) -> Tuple[float, float]
     ```
     """
-    
-    def __init__(self,
-                 estimator: Estimator,
-                 metric: Evaluator,
-                 cv: int = 5,
-                 fold_type: FoldType = KFold,
-                 shuffle: bool = True,
-                 random_state: int = None,
-                 verbose: bool = False) -> None:
+
+    def __init__(
+        self,
+        estimator: Estimator,
+        metric: Evaluator,
+        cv: int = 5,
+        fold_type: FoldType = KFold,
+        shuffle: bool = True,
+        random_state: int = None,
+        verbose: bool = False,
+    ) -> None:
         self.estimator = estimator
         self.metric = metric
         self.cv = cv
         self.fold_type = fold_type
         self.shuffle = shuffle
         self.random_state = random_state
         self.verbose = verbose
         self.train_scores_ = []
         self.test_scores_ = []
-    
+
+        self.set_param_ranges({"cv": ("0,+inf", int)})
+        self.check_param_ranges()
+
     def _fit(self, X: Matrix, y: Vector) -> None:
-        fold = self.fold_type(X, y,
-                              n_folds=self.cv,
-                              shuffle=self.shuffle,
-                              random_state=self.random_state)
-        
+        fold = self.fold_type(
+            X, y, n_folds=self.cv, shuffle=self.shuffle, random_state=self.random_state
+        )
+
         for i, (train_indices, test_indices) in enumerate(fold.split):
             X_train, y_train = X[train_indices], y[train_indices]
             X_test, y_test = X[test_indices], y[test_indices]
-            
+
             self.estimator.fit(X_train, y_train)
-            if self.metric: 
+            if self.metric:
                 train_score = self.estimator.score(X_train, y_train, self.metric)
                 test_score = self.estimator.score(X_test, y_test, self.metric)
-            else: 
+            else:
                 train_score = self.estimator.score(X_train, y_train)
                 test_score = self.estimator.score(X_test, y_test)
-            
+
             self.train_scores_.append(train_score)
             self.test_scores_.append(test_score)
-            
+
             if self.verbose:
-                print(f'[CV] fold {i + 1} -',
-                      f'train-score: {train_score:.3f},',
-                      f'test-score: {test_score:.3f}')
-        
+                print(
+                    f"[CV] fold {i + 1} -",
+                    f"train-score: {train_score:.3f},",
+                    f"test-score: {test_score:.3f}",
+                )
+
     def score(self, X: Matrix, y: Vector) -> Tuple[float, float]:
         self._fit(X, y)
         return np.mean(self.train_scores_), np.mean(self.test_scores_)
-
```

### Comparing `luma-ml-0.6.4/luma/model_selection/fold.py` & `luma-ml-0.6.5/luma/model_selection/fold.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,109 +1,108 @@
 from collections import Counter, defaultdict
 from itertools import chain
 from typing import Generator, Tuple, Union
 import numpy as np
 
 from luma.interface.util import Matrix, Vector
 
-FoldType = Union['KFold', 'StratifiedKFold', 'GroupKFold']
+FoldType = Union["KFold", "StratifiedKFold", "GroupKFold"]
 
 
-__all__ = (
-    'KFold',
-    'StratifiedKFold',
-    'GroupKFold'
-)
+__all__ = ("KFold", "StratifiedKFold", "GroupKFold")
 
 
 class KFold:
-    
     """
-    K-Fold cross-validation is a model evaluation method that divides 
-    the dataset into `k` equal or nearly equal sized folds. In each 
-    of `k` iterations, one fold is used as the test set, and the 
-    remaining `k-1` folds are combined to form the training set. This 
-    process ensures that every data point gets to be in the test set 
-    exactly once and in the training set `k-1` times. It's widely used 
-    to assess the performance of a model with limited data, providing 
+    K-Fold cross-validation is a model evaluation method that divides
+    the dataset into `k` equal or nearly equal sized folds. In each
+    of `k` iterations, one fold is used as the test set, and the
+    remaining `k-1` folds are combined to form the training set. This
+    process ensures that every data point gets to be in the test set
+    exactly once and in the training set `k-1` times. It's widely used
+    to assess the performance of a model with limited data, providing
     a robust estimate of its generalization capability.
-    
+
     Parameters
     ----------
     `X` : Input data
     `y` : Target data
     `n_folds` : Number of folds
     `shuffle` : Whether to shuffle the dataset
     `random_state` : Seed for random shuffling
-    
+
     Properties
     ----------
     ```py
     @property
     def split(self)
     ```
     This returns a generator with the type:
     ```py
     Generator[Tuple[Vector, Vector], None, None]
     ```
     yielding train indices and test indices.
-    
+
     Examples
     --------
     Usage of the generator returned by the property `split`:
-    
+
     ```py
     kfold = KFold(X, y, n_folds=5, shuffle=True)
-    
+
     for train_indices, test_indices in kfold.split:
         X_train, y_train = X[train_indices], y[train_indices]
         ...
     ```
     """
-    
-    def __init__(self,
-                 X: Matrix, 
-                 y: Vector,
-                 n_folds: int = 5,
-                 shuffle: bool = True,
-                 random_state: int = None) -> None:
+
+    def __init__(
+        self,
+        X: Matrix,
+        y: Vector,
+        n_folds: int = 5,
+        shuffle: bool = True,
+        random_state: int = None,
+    ) -> None:
         self.X = X
         self.y = y
         self.shuffle = shuffle
         self.random_state = random_state
         self.n_folds = n_folds
-    
+
+        self.set_param_ranges({"n_folds": ("0,+inf", int)})
+        self.check_param_ranges()
+
     @property
     def split(self) -> Generator[Tuple[Vector, Vector], None, None]:
         np.random.seed(self.random_state)
         m, _ = self.X.shape
         fold_size = m // self.n_folds
 
         indices = np.arange(m)
         if self.shuffle:
             np.random.shuffle(indices)
-        
+
         for i in range(self.n_folds):
             start = i * fold_size
             end = start + fold_size if i < self.n_folds - 1 else m
-            
+
             test_indices = indices[start:end]
             train_indices = np.concatenate((indices[:start], indices[end:]))
-            
+
             yield train_indices, test_indices
 
 
 class StratifiedKFold:
-    
     """
-    Stratified K-Fold cross-validation is a model evaluation method similar 
-    to KFold but it divides the dataset in a way that preserves the 
-    percentage of samples for each class. This is especially useful for 
-    handling imbalances in the dataset. It ensures each fold is a good 
-    representative of the whole by maintaining the same class distribution 
+    Stratified K-Fold cross-validation is a model evaluation method similar
+    to KFold but it divides the dataset in a way that preserves the
+    percentage of samples for each class. This is especially useful for
+    handling imbalances in the dataset. It ensures each fold is a good
+    representative of the whole by maintaining the same class distribution
     in each fold as in the complete dataset.
 
     Parameters
     ----------
     `X` : Input data
     `y` : Target data
     `n_folds` : Number of folds
@@ -117,149 +116,157 @@
     def split(self)
     ```
     This returns a generator with the type:
     ```py
     Generator[Tuple[Vector, Vector], None, None]
     ```
     yielding train indices and test indices.
-    
+
     Examples
     --------
     Usage of the generator returned by the property `split`:
-    
+
     ```py
     kfold = StratifiedKFold(X, y, n_folds=5, shuffle=True)
-    
+
     for train_indices, test_indices in kfold.split:
         X_train, y_train = X[train_indices], y[train_indices]
         ...
     ```
     """
-    
-    def __init__(self, 
-                 X: Matrix, 
-                 y: Vector, 
-                 n_folds: int = 5, 
-                 shuffle: bool = True, 
-                 random_state: int = None) -> None:
+
+    def __init__(
+        self,
+        X: Matrix,
+        y: Vector,
+        n_folds: int = 5,
+        shuffle: bool = True,
+        random_state: int = None,
+    ) -> None:
         self.X = X
         self.y = y
         self.n_folds = n_folds
         self.shuffle = shuffle
         self.random_state = random_state
-    
+
+        self.set_param_ranges({"n_folds": ("0,+inf", int)})
+        self.check_param_ranges()
+
     @property
     def split(self) -> Generator[Tuple[Vector, Vector], None, None]:
         np.random.seed(self.random_state)
-        
+
         indices_per_class = defaultdict(list)
         for idx, class_ in enumerate(self.y):
             indices_per_class[class_].append(idx)
-        
+
         if self.shuffle:
             for indices in indices_per_class.values():
                 np.random.shuffle(indices)
-        
+
         folds = defaultdict(list)
         for class_, indices in indices_per_class.items():
             fold_size = len(indices) // self.n_folds
             for i in range(self.n_folds):
                 start = i * fold_size
                 end = start + fold_size if i < self.n_folds - 1 else len(indices)
                 folds[i].extend(indices[start:end])
-        
+
         if self.shuffle:
             for fold_indices in folds.values():
                 np.random.shuffle(fold_indices)
-        
+
         for i in range(self.n_folds):
             test_indices = folds[i]
-            train_indices = list(chain.from_iterable(
-                folds[j] for j in range(self.n_folds) if j != i
-            ))
-            
+            train_indices = list(
+                chain.from_iterable(folds[j] for j in range(self.n_folds) if j != i)
+            )
+
             yield Vector(train_indices), Vector(test_indices)
 
 
 class GroupKFold:
-    
     """
-    Group K-Fold cross-validation provides train/test indices to split data into 
-    train/test sets. Each set contains group samples that are entirely in the set 
-    of training or test. This cross-validation object is a variation of KFold 
-    that ensures samples from the same group are not split between training and 
+    Group K-Fold cross-validation provides train/test indices to split data into
+    train/test sets. Each set contains group samples that are entirely in the set
+    of training or test. This cross-validation object is a variation of KFold
+    that ensures samples from the same group are not split between training and
     testing sets.
-    
+
     Parameters
     ----------
     `X` : Input data
     `y` : Target data
     `groups` : Array of group labels for the samples
     `n_folds` : Number of folds. Must be at least 2.
     `shuffle` : Whether to shuffle the dataset
     `random_state` : Seed for random shuffling
-    
+
     Properties
     ----------
     ```py
     @property
     def split(self)
     ```
     This returns a generator with the type:
     ```py
     Generator[Tuple[Vector, Vector], None, None]
     ```
     yielding train indices and test indices.
-    
+
     Examples
     --------
     Usage of the generator returned by the property `split`:
-    
+
     ```py
     kfold = GroupKFold(X, y, n_folds=5, shuffle=True)
-    
+
     for train_indices, test_indices in kfold.split:
         X_train, y_train = X[train_indices], y[train_indices]
         ...
     ```
     """
 
-    def __init__(self,
-                 X: Matrix, 
-                 y: Vector,
-                 groups: Vector,
-                 n_folds: int = 5,
-                 shuffle: bool = True,
-                 random_state: int = None) -> None:
+    def __init__(
+        self,
+        X: Matrix,
+        y: Vector,
+        groups: Vector,
+        n_folds: int = 5,
+        shuffle: bool = True,
+        random_state: int = None,
+    ) -> None:
         self.X = X
         self.y = y
         self.groups = groups
         self.n_folds = n_folds
         self.shuffle = shuffle
         self.random_state = random_state
-    
+
+        self.set_param_ranges({"n_folds": ("0,+inf", int)})
+        self.check_param_ranges()
+
     @property
     def split(self) -> Generator[Tuple[Vector, Vector], None, None]:
         np.random.seed(self.random_state)
         _, groups_indices = np.unique(self.groups, return_inverse=True)
-        
+
         group_counts = Counter(groups_indices)
         group_indices = defaultdict(list)
         for idx, group_idx in enumerate(groups_indices):
             group_indices[group_idx].append(idx)
-        
+
         sorted_groups = sorted(group_counts, key=group_counts.get, reverse=True)
-        
+
         if self.shuffle:
             np.random.shuffle(sorted_groups)
-        
+
         folds = [[] for _ in range(self.n_folds)]
         for group in sorted_groups:
             smallest = min(range(self.n_folds), key=lambda x: len(folds[x]))
             folds[smallest].extend(group_indices[group])
-        
+
         for i in range(self.n_folds):
             test_indices = folds[i]
             train_indices = list(set(range(len(self.X))) - set(test_indices))
-            
-            yield Vector(train_indices), Vector(test_indices)
 
+            yield Vector(train_indices), Vector(test_indices)
```

### Comparing `luma-ml-0.6.4/luma/model_selection/search.py` & `luma-ml-0.6.5/luma/model_selection/search.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,179 +5,188 @@
 
 from luma.interface.util import Matrix, Vector
 from luma.core.super import Estimator, Evaluator, Optimizer
 from luma.interface.exception import NotFittedError
 from luma.model_selection.cv import CrossValidator
 from luma.model_selection.fold import FoldType, KFold
 
-DT = TypeVar('DT', bound=rv_continuous | rv_discrete)
+DT = TypeVar("DT", bound=rv_continuous | rv_discrete)
 
 
-__all__ = (
-    'GridSearchCV',
-    'RandomizedSearchCV'
-)
+__all__ = ("GridSearchCV", "RandomizedSearchCV")
 
 
 class GridSearchCV(Optimizer):
-    
     """
-    Grid seach with cross validation(CV) is a method used to tune hyperparameters 
-    of a model by searching through a specified parameter grid. It evaluates all 
-    combinations of parameter values to find the best combination. This process 
-    is performed using cross-validation to ensure model performance is not biased 
-    to a specific data split. The result is the optimal set of parameters that 
+    Grid seach with cross validation(CV) is a method used to tune hyperparameters
+    of a model by searching through a specified parameter grid. It evaluates all
+    combinations of parameter values to find the best combination. This process
+    is performed using cross-validation to ensure model performance is not biased
+    to a specific data split. The result is the optimal set of parameters that
     yield the best model performance according to a chosen metric.
-    
+
     Parameters
     ----------
     `estimator` : An estimator to fit and evaluate
     `param_grid` : Parameter grid for repetitive search
     `cv` : K-fold size for cross validation
     `metric` : Scoring metric for evaluation
     `maximize` : Whether to optimize in a way of maximizing certain metric
     `shuffle` : Whether to shuffle the dataset
     `fold_type` : Fold type (Default `KFold`)
     `refit` : Whether to re-fit the estimator with the best parameters found
     `random_state` : Seed for random sampling for cross validation
-    
+
     Properties
     ----------
     Get the best(optimized) estimator:
         ```py
         @property
         def best_model(self) -> Estimator
         ```
-    
+
     Notes
     -----
     * An instance of the estimator must be passed to `estimator`
     * For `metric`, both class or instance are possible
     * Only `Pipeline` is allowed for meta estimator
-    
+
     Examples
     --------
-    >>> param_grid = {'param_1': [...], 
+    >>> param_grid = {'param_1': [...],
                       'param_2': [...],
                       ...,
                       AnyStr: List[Any]}
-    
+
     >>> grid = GridSearchCV(estimator=AnyEstimator(),
                             param_grid=param_grid,
                             cv=5,
                             metric=AnyEvaluator,
                             refit=True,
                             random_state=None)
     >>> grid.fit(X, y)
     >>> score = grid.best_score
     >>> model = grid.best_model
-    
+
     """
-    
-    def __init__(self, 
-                 estimator: Estimator, 
-                 param_grid: dict, 
-                 cv: int = 5, 
-                 metric: Evaluator = None,
-                 maximize: bool = True, 
-                 refit: bool = True, 
-                 shuffle: bool = True,
-                 fold_type: FoldType = KFold, 
-                 random_state: int = None,
-                 verbose: bool = False) -> None:
+
+    def __init__(
+        self,
+        estimator: Estimator,
+        param_grid: dict,
+        cv: int = 5,
+        metric: Evaluator = None,
+        maximize: bool = True,
+        refit: bool = True,
+        shuffle: bool = True,
+        fold_type: FoldType = KFold,
+        random_state: int = None,
+        verbose: bool = False,
+    ) -> None:
         self.estimator = estimator
         self.param_grid = param_grid
         self.cv = cv
         self.metric = metric
         self.maximize = maximize
         self.refit = refit
         self.shuffle = shuffle
         self.fold_type = fold_type
         self.random_state = random_state
         self.verbose = verbose
         self.scores_ = []
         self._fitted = False
 
+        self.set_param_ranges({"cv": ("0,+inf", int)})
+        self.check_param_ranges()
+
     def fit(self, X: Matrix, y: Vector) -> Estimator:
         best_score = None
         best_params = None
         param_combinations = self._get_param_combinations()
         max_iter = len(param_combinations)
-        
+
         if self.verbose:
-            print(f'Fitting {self.cv} folds for {max_iter} candidates,',
-                  f'totalling {self.cv * max_iter} fits.\n')
-        
-        for i, params in enumerate(param_combinations, start=1): 
+            print(
+                f"Fitting {self.cv} folds for {max_iter} candidates,",
+                f"totalling {self.cv * max_iter} fits.\n",
+            )
+
+        for i, params in enumerate(param_combinations, start=1):
             self._set_params(params)
-            cv_model = CrossValidator(estimator=self.estimator,
-                                      metric=self.metric,
-                                      cv=self.cv,
-                                      shuffle=self.shuffle,
-                                      fold_type=self.fold_type,
-                                      random_state=self.random_state,
-                                      verbose=self.verbose)
-            
+            cv_model = CrossValidator(
+                estimator=self.estimator,
+                metric=self.metric,
+                cv=self.cv,
+                shuffle=self.shuffle,
+                fold_type=self.fold_type,
+                random_state=self.random_state,
+                verbose=self.verbose,
+            )
+
             _, mean_score = cv_model.score(X, y)
             self.scores_.append((params, mean_score))
-            
+
             if self.verbose:
-                params_f = {k: f'{v:.4f}' if isinstance(v, float) else v 
-                            for k, v in params.items()}
-                print(f'[GridSearchCV] candidate {i}/{max_iter} {params_f}',
-                      f'- score:{mean_score:.3f}')
-            
+                params_f = {
+                    k: f"{v:.4f}" if isinstance(v, float) else v
+                    for k, v in params.items()
+                }
+                print(
+                    f"[GridSearchCV] candidate {i}/{max_iter} {params_f}",
+                    f"- score:{mean_score:.3f}",
+                )
+
             if self.maximize:
                 if best_score is None or mean_score > best_score:
                     best_score = mean_score
                     best_params = params
             else:
                 if best_score is None or mean_score < best_score:
                     best_score = mean_score
                     best_params = params
 
         self.best_score = best_score
         self.best_params = best_params
-        
+
         if self.verbose:
-            print(f'\n[GridSearchCV] Best params: {self.best_params}')
-            print(f'[GridSearchCV] Best score: {self.best_score}')
-        
+            print(f"\n[GridSearchCV] Best params: {self.best_params}")
+            print(f"[GridSearchCV] Best score: {self.best_score}")
+
         if self.refit:
             self.estimator = type(self.estimator)()
             self._set_params(best_params)
             self.estimator.fit(X, y)
-        
+
         self._fitted = True
         return self.best_model
-    
+
     def _get_param_combinations(self) -> List[Dict[str, Any]]:
         keys, values = zip(*self.param_grid.items())
         param_combinations = Matrix(np.meshgrid(*values)).T.reshape(-1, len(keys))
         param_combinations = [dict(zip(keys, v)) for v in param_combinations]
         return param_combinations
-    
+
     def _set_params(self, params: dict) -> None:
         self.estimator.set_params(**params)
-    
+
     @property
     def best_model(self) -> Estimator:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         return self.estimator
 
 
 class RandomizedSearchCV(Optimizer):
-    
     """
-    Randomized search with cross-validation (CV) is a method used to tune 
-    hyperparameters of a model by searching through a specified parameter 
-    distribution. It randomly samples combinations of parameter values to find 
-    the best combination. This process is performed using cross-validation to 
-    ensure model performance is not biased to a specific data split. The result 
-    is the optimal set of parameters that yield the best model performance 
+    Randomized search with cross-validation (CV) is a method used to tune
+    hyperparameters of a model by searching through a specified parameter
+    distribution. It randomly samples combinations of parameter values to find
+    the best combination. This process is performed using cross-validation to
+    ensure model performance is not biased to a specific data split. The result
+    is the optimal set of parameters that yield the best model performance
     according to a chosen metric.
 
     Parameters
     ----------
     `estimator` : An estimator to fit and evaluate
     `param_dist` : Parameter distributions for random search
     `max_iter` : Number of parameter settings that are sampled
@@ -185,139 +194,154 @@
     `metric` : Scoring metric for evaluation
     `maximize` : Whether to optimize in a way of maximizing certain metric
     `refit` : Whether to re-fit the estimator with the best parameters found
     `shuffle` : Whether to shuffle the dataset
     `fold_type` : Fold type (Default `KFold`)
     `random_state` : Seed for random sampling for cross-validation and random search
     `verbose` : Whether to print progress messages
-    
+
     Properties
     ----------
     Get the best(optimized) estimator:
         ```py
         @property
         def best_model(self) -> Estimator
         ```
-    
+
     Notes
     -----
     * An instance of the estimator must be passed to `estimator`
     * For `metric`, both class or instance are possible
     * Only `Pipeline` is allowed for meta estimator
     * Type `DT` is a generic type for `scipy`'s distribution types
         (e.g. `rv_continuous`, `rv_discrete`)
-    
+
     Examples
     --------
-    >>> param_dist = {'param_1': [...], 
+    >>> param_dist = {'param_1': [...],
                       'param_2': [...],
                       ...,
                       AnyStr: Vector | DT }
 
     >>> rand = RandomizedSearchCV(estimator=AnyEstimator(),
                                   param_dist=param_dist,
                                   max_iter=100,
                                   cv=5,
                                   metric=AnyEvaluator,
                                   refit=True,
                                   random_state=None)
     >>> rand.fit(X, y)
     >>> score = rand.best_score
     >>> model = rand.best_model
-    
+
     """
-    
-    def __init__(self,
-                 estimator: Estimator,
-                 param_dist: Dict[str, Vector | DT],
-                 max_iter: int = 100,
-                 cv: int = 5,
-                 metric: Evaluator = None,
-                 maximize: bool = True, 
-                 refit: bool = True,
-                 shuffle: bool = True,
-                 fold_type: FoldType = KFold,
-                 random_state: int = None,
-                 verbose: bool = False) -> None:
+
+    def __init__(
+        self,
+        estimator: Estimator,
+        param_dist: Dict[str, Vector | DT],
+        max_iter: int = 100,
+        cv: int = 5,
+        metric: Evaluator = None,
+        maximize: bool = True,
+        refit: bool = True,
+        shuffle: bool = True,
+        fold_type: FoldType = KFold,
+        random_state: int = None,
+        verbose: bool = False,
+    ) -> None:
         self.estimator = estimator
         self.param_dist = param_dist
         self.max_iter = max_iter
         self.cv = cv
         self.metric = metric
         self.maximize = maximize
         self.refit = refit
         self.shuffle = shuffle
         self.fold_type = fold_type
         self.random_state = random_state
         self.verbose = verbose
         self.scores_ = []
         self._fitted = False
-    
+
+        self.set_param_ranges({"cv": ("0,+inf", int), "max_iter": ("0<,+inf", int)})
+        self.check_param_ranges()
+
     def fit(self, X: Matrix, y: Vector) -> Estimator:
         best_score = None
         best_params = None
-        
+
         if self.verbose:
-            print(f'Fitting {self.cv} folds for {self.max_iter} candidates,',
-                  f'toatlling {self.cv * self.max_iter} fits.\n')
-        
+            print(
+                f"Fitting {self.cv} folds for {self.max_iter} candidates,",
+                f"toatlling {self.cv * self.max_iter} fits.\n",
+            )
+
         for i in range(self.max_iter):
             params = self._sample_params()
             self._set_params(params)
-            
-            cv_model = CrossValidator(estimator=self.estimator,
-                                      metric=self.metric,
-                                      cv=self.cv,
-                                      shuffle=self.shuffle,
-                                      fold_type=self.fold_type,
-                                      random_state=self.random_state,
-                                      verbose=self.verbose)
+
+            cv_model = CrossValidator(
+                estimator=self.estimator,
+                metric=self.metric,
+                cv=self.cv,
+                shuffle=self.shuffle,
+                fold_type=self.fold_type,
+                random_state=self.random_state,
+                verbose=self.verbose,
+            )
 
             _, mean_score = cv_model.score(X, y)
             self.scores_.append((params, mean_score))
-            
+
             if self.verbose:
-                params_f = {k: f'{v:.4f}' if isinstance(v, float) else v 
-                            for k, v in params.items()}
-                print(f'[RandomSearchCV] candidate {i + 1}/{self.max_iter}',
-                      f'{params_f} - score: {mean_score:.3f}')
-            
+                params_f = {
+                    k: f"{v:.4f}" if isinstance(v, float) else v
+                    for k, v in params.items()
+                }
+                print(
+                    f"[RandomSearchCV] candidate {i + 1}/{self.max_iter}",
+                    f"{params_f} - score: {mean_score:.3f}",
+                )
+
             if self.maximize:
                 if best_score is None or mean_score > best_score:
                     best_score = mean_score
                     best_params = params
             else:
                 if best_score is None or mean_score < best_score:
                     best_score = mean_score
                     best_params = params
-        
+
         self.best_score = best_score
         self.best_params = best_params
-        
+
         if self.verbose:
-            print(f'\n[RandomSearchCV] Best params: {self.best_params}')
-            print(f'[RandomSearchCV] Best score: {self.best_score}')
-        
+            print(f"\n[RandomSearchCV] Best params: {self.best_params}")
+            print(f"[RandomSearchCV] Best score: {self.best_score}")
+
         if self.refit:
             self.estimator = type(self.estimator)()
             self._set_params(best_params)
             self.estimator.fit(X, y)
-        
+
         self._fitted = True
         return self.best_model
 
     def _set_params(self, params: dict) -> None:
         self.estimator.set_params(**params)
-        
+
     def _sample_params(self) -> Dict[str, Any]:
         params = {}
         for key, dist in self.param_dist.items():
-            if hasattr(dist, 'rvs'): params[key] = dist.rvs()
-            else: params[key] = random.choice(dist)
-        
+            if hasattr(dist, "rvs"):
+                params[key] = dist.rvs()
+            else:
+                params[key] = random.choice(dist)
+
         return params
 
     @property
     def best_model(self) -> Estimator:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         return self.estimator
-
```

### Comparing `luma-ml-0.6.4/luma/model_selection/split.py` & `luma-ml-0.6.5/luma/model_selection/split.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,115 +1,118 @@
 from typing import Tuple
 import numpy as np
 
 from luma.interface.util import Matrix, Vector
 
 
-__all__ = (
-    'TrainTestSplit'
-)
+__all__ = "TrainTestSplit"
 
 
 class TrainTestSplit:
-    
     """
     Splits the original dataset into the train set and the test set.
-    
+
     Parameters
     ----------
     `X` : Feature data
     `y` : Target data (as a 1-D `Vector`)
     `test_size` : Proportional size of the test set (e.g. `0.2`, `0.3`)
     `shuffle` : Whether to shuffle the dataset
     `stratify` : Whether to perform stratified split (Default `False`)
     `random_state` : Seed for random sampling for split
-    
+
     Properties
     ----------
     `get` : Returns the split data as a 4-tuple
-    
+
     Examples
     --------
     ```py
     X_train, X_test, y_train, y_test = TrainTestSplit(X, y, ...).get
     ```
     """
-    
-    def __init__(self, 
-                 X: Matrix,
-                 y: Vector,
-                 test_size: int | float = 0.3,
-                 shuffle: bool = True,
-                 stratify: bool = False,
-                 random_state: int = None) -> None:
+
+    def __init__(
+        self,
+        X: Matrix,
+        y: Vector,
+        test_size: int | float = 0.3,
+        shuffle: bool = True,
+        stratify: bool = False,
+        random_state: int = None,
+    ) -> None:
         self.X = X
         self.y = y
         self.test_size = test_size
         self.shuffle = shuffle
         self.stratify = stratify
         self.random_state = random_state
-    
+
+        self.set_param_ranges({"test_size": ("0<,+inf", int)})
+        self.check_param_ranges()
+
     @property
     def get(self) -> Tuple[Matrix, Matrix, Vector, Vector]:
         if self.X.shape[0] != self.y.shape[0]:
             raise ValueError("Sample size mismatch between 'X' and 'y'!")
-        
-        if self.stratify: return self._stratified_split()
-        else: return self._split()
-    
+
+        if self.stratify:
+            return self._stratified_split()
+        else:
+            return self._split()
+
     def _split(self) -> Tuple[Matrix, Matrix, Vector, Vector]:
         num_samples = self.X.shape[0]
         indices = np.arange(num_samples)
-        
+
         if isinstance(self.test_size, float):
             num_test_samples = int(self.test_size * num_samples)
         else:
             num_test_samples = self.test_size
-        
+
         if self.random_state is not None:
             np.random.seed(self.random_state)
         if self.shuffle:
             np.random.shuffle(indices)
 
         test_indices = indices[:num_test_samples]
         train_indices = indices[num_test_samples:]
 
         X_train = self.X[train_indices]
         X_test = self.X[test_indices]
         y_train = self.y[train_indices]
         y_test = self.y[test_indices]
 
         return X_train, X_test, y_train, y_test
-    
+
     def _stratified_split(self) -> Tuple[Matrix, Matrix, Vector, Vector]:
         if isinstance(self.test_size, float):
             test_size_func = lambda u: int(self.test_size * len(u))
         else:
             total_size = len(self.y)
             proportion = self.test_size / total_size
             test_size_func = lambda u: int(proportion * len(u))
-        
+
         unique_classes, y_indices = np.unique(self.y, return_inverse=True)
         train_indices, test_indices = [], []
-        
+
         for class_index in unique_classes:
-            class_mask = (y_indices == class_index)
+            class_mask = y_indices == class_index
             class_indices = np.where(class_mask)[0]
-            
+
             if self.shuffle:
                 np.random.shuffle(class_indices)
-            
+
             num_test_samples = test_size_func(class_indices)
             test_indices.extend(class_indices[:num_test_samples])
             train_indices.extend(class_indices[num_test_samples:])
-        
+
         if self.shuffle:
             np.random.shuffle(train_indices)
             np.random.shuffle(test_indices)
 
         X_train = self.X[train_indices]
         X_test = self.X[test_indices]
         y_train = self.y[train_indices]
         y_test = self.y[test_indices]
 
         return X_train, X_test, y_train, y_test
-
```

### Comparing `luma-ml-0.6.4/luma/neural/activation.py` & `luma-ml-0.6.5/luma/neural/activation.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 import numpy as np
 
 
-__all__ = (
-    'ReLU',
-    'LeakyReLU',
-    'ELU',
-    'Tanh', 
-    'Sigmoid',
-    'Softmax'
-)
+__all__ = ("ReLU", "LeakyReLU", "ELU", "Tanh", "Sigmoid", "Softmax")
+
+
+class _Matrix:
+    pass
 
-class _Matrix: pass
 
 Matrix = _Matrix
 
 
 class ReLU:
     def func(self, X: Matrix) -> Matrix:
         return np.maximum(0, X)
-    
+
     def derivative(self, X: Matrix) -> Matrix:
         return (X > 0).astype(float)
 
 
 class LeakyReLU:
     def __init__(self, alpha=0.01):
         self.alpha = alpha
@@ -66,17 +62,18 @@
         exps = np.exp(X - np.max(X, axis=1, keepdims=True))
         return exps / np.sum(exps, axis=1, keepdims=True)
 
     def derivative(self, X: Matrix) -> Matrix:
         m, n = X.shape
         soft_out = self.func(X)
         jacobian = np.zeros((m, n, n))
-        
+
         for i in range(len(soft_out)):
             for j in range(len(soft_out[i])):
                 for k in range(len(soft_out[i])):
-                    if j == k: val = soft_out[i, j] * (1 - soft_out[i, j])
-                    else: val = -soft_out[i, j] * soft_out[i, k]
+                    if j == k:
+                        val = soft_out[i, j] * (1 - soft_out[i, j])
+                    else:
+                        val = -soft_out[i, j] * soft_out[i, k]
                     jacobian[i, j, k] = val
 
         return jacobian
-
```

### Comparing `luma-ml-0.6.4/luma/neural/multi_layer.py` & `luma-ml-0.6.5/luma/neural/multi_layer.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,31 +5,28 @@
 from luma.interface.util import Matrix, Vector, ActivationUtil
 from luma.interface.exception import NotFittedError
 from luma.metric.classification import Accuracy
 from luma.neural.activation import Softmax
 from luma.neural.optimizer import SGDOptimizer
 
 
-__all__ = (
-    'MLPClassifier'
-)
+__all__ = "MLPClassifier"
 
 
 class MLPClassifier(Estimator, Supervised):
-    
     """
-    An MLP (Multilayer Perceptron) is a type of neural network composed 
-    of one input layer, one or more hidden layers, and one output layer, 
-    with fully connected neurons. Each neuron uses a nonlinear activation 
-    function to allow the network to capture complex patterns in the data. 
-    MLPs are trained using backpropagation, where the network learns by 
-    adjusting weights to minimize the difference between its predictions 
-    and the actual data. They are widely used for classification, regression, 
+    An MLP (Multilayer Perceptron) is a type of neural network composed
+    of one input layer, one or more hidden layers, and one output layer,
+    with fully connected neurons. Each neuron uses a nonlinear activation
+    function to allow the network to capture complex patterns in the data.
+    MLPs are trained using backpropagation, where the network learns by
+    adjusting weights to minimize the difference between its predictions
+    and the actual data. They are widely used for classification, regression,
     and other predictive tasks in machine learning.
-    
+
     Parameters
     ----------
     `input_size` : Number of neurons in the input layer
     `hidden_sizes` : List of numbers of neurons in the hidden layers
     (an `int` for a single hidden layer)
     `output_size` : Number of neurons in the output layer
     `max_epoch` :  Maximum number of epochs
@@ -40,17 +37,17 @@
     `lambda_` : L2 regularization strength
     `dropout_rate` : Dropout rate for each layer
     `activation` : Activation function for hidden layers
     (default `ReLU`)
     `optimizer` : An optimizing method for reducing the training loss
     (default `SGDOptimizer`)
     `random_state` : Seed for various random sampling processes
-    `verbose` : Whether to log procedural details 
+    `verbose` : Whether to log procedural details
     (an `int` to log for every specific amount of epochs, default 100)
-    
+
     Properties
     ----------
     For getting weights and biases:
     ```py
         (property) weights: List[Matrix]
         (property) biases: List[Vector]
     ```
@@ -65,32 +62,34 @@
         ```py
         def dump(self, padding: int = 4) -> None
         ```
     Notes
     -----
     * An instance of an `Optimizer` must be passed to `optimizer`
     * Optimizers of `luma.neural.optimizer` are only accepted
-    
+
     """
-    
-    def __init__(self, 
-                 input_size: int,
-                 hidden_sizes: List[int] | int,
-                 output_size: int,
-                 max_epoch: int = 1000,
-                 batch_size: int = 100,
-                 learning_rate: float = 0.001,
-                 momentum: float = 0.9, 
-                 decay_rate: float = 0.9, 
-                 lambda_: float = 0.01,
-                 dropout_rate: float = 0.1,
-                 activation: ActivationUtil.func_type = 'relu',
-                 optimizer: Optimizer = SGDOptimizer(),
-                 random_state: int = None,
-                 verbose: bool | int = False) -> None:
+
+    def __init__(
+        self,
+        input_size: int,
+        hidden_sizes: List[int] | int,
+        output_size: int,
+        max_epoch: int = 1000,
+        batch_size: int = 100,
+        learning_rate: float = 0.001,
+        momentum: float = 0.9,
+        decay_rate: float = 0.9,
+        lambda_: float = 0.01,
+        dropout_rate: float = 0.1,
+        activation: ActivationUtil.FuncType = "relu",
+        optimizer: Optimizer = SGDOptimizer(),
+        random_state: int = None,
+        verbose: bool | int = False,
+    ) -> None:
         self.input_size = input_size
         self.hidden_sizes = hidden_sizes
         self.output_size = output_size
         self.max_epoch = max_epoch
         self.batch_size = batch_size
         self.learning_rate = learning_rate
         self.momentum = momentum
@@ -100,181 +99,196 @@
         self.activation = activation
         self.optimizer = optimizer
         self.random_state = random_state
         self.verbose = verbose
         self.batch_losses_ = []
         self.epoch_losses_ = []
         self._fitted = False
-    
-    def fit(self, X: Matrix, y: Vector) -> 'MLPClassifier':
+
+        self.set_param_ranges(
+            {
+                "input_size": ("0<,+inf", int),
+                "output_size": ("0<,+inf", int),
+                "max_epoch": ("0<,+inf", int),
+                "batch_size": ("0<,+inf", int),
+                "learning_rate": ("0<,+inf", None),
+                "momentum": ("0,1", None),
+                "decay_rate": ("0,1", None),
+                "lambda_": ("0,+inf", None),
+                "dropout_rate": ("0,1", None),
+            }
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix, y: Vector) -> "MLPClassifier":
         if isinstance(self.hidden_sizes, int):
             self.hidden_sizes = [self.hidden_sizes]
-        
-        self.layer_sizes = [
-            self.input_size, 
-            *self.hidden_sizes, 
-            self.output_size
-        ]
+
+        self.layer_sizes = [self.input_size, *self.hidden_sizes, self.output_size]
         self.n_layers = len(self.layer_sizes) - 1
         self.weights = []
         self.biases = []
-        
+
         act = ActivationUtil(self.activation)
         self.act_ = act.activation_type()
         self.softmax_ = Softmax()
         self.rs_ = np.random.RandomState(self.random_state)
-        
+
         optimizer_params = {
-            'learning_rate': self.learning_rate,
-            'momentum': self.momentum,
-            'decay_rate': self.decay_rate
+            "learning_rate": self.learning_rate,
+            "momentum": self.momentum,
+            "decay_rate": self.decay_rate,
         }
         for param, val in optimizer_params.items():
             if hasattr(self.optimizer, param):
                 setattr(self.optimizer, param, val)
-        
+
         for i in range(self.n_layers):
-            weight_mat = self.rs_.randn(self.layer_sizes[i], 
-                                        self.layer_sizes[i + 1])
+            weight_mat = self.rs_.randn(self.layer_sizes[i], self.layer_sizes[i + 1])
             self.weights.append(weight_mat * 0.01)
             self.biases.append(np.zeros((1, self.layer_sizes[i + 1])))
-        
+
         m, _ = X.shape
         y = self._one_hot_encode(y)
         for epoch in range(self.max_epoch):
             indices = np.arange(m)
             self.rs_.shuffle(indices)
             X_shuffled = X[indices]
             y_shuffled = y[indices]
-            
+
             for start in range(0, m, self.batch_size):
                 end = min(start + self.batch_size, m)
                 X_batch = X_shuffled[start:end]
                 y_batch = y_shuffled[start:end]
-                
+
                 y_pred_batch = self._forward_pass(X_batch, is_train=True)
                 self._backpropagation(X_batch, y_batch)
-                
+
                 batch_loss = self._compute_loss(y_batch, y_pred_batch)
                 self.batch_losses_.append(batch_loss)
-            
-            epoch_loss = np.mean(self.batch_losses_[-(m // self.batch_size):])
+
+            epoch_loss = np.mean(self.batch_losses_[-(m // self.batch_size) :])
             self.epoch_losses_.append(epoch_loss)
             if self.verbose:
-                if isinstance(self.verbose, bool): step = 100
-                elif isinstance(self.verbose, int): step = self.verbose
+                if isinstance(self.verbose, bool):
+                    step = 100
+                elif isinstance(self.verbose, int):
+                    step = self.verbose
                 if epoch % step == 0:
                     print(f"[MLPClassifier] Epoch {epoch}, Loss: {epoch_loss}")
-        
+
         self._fitted = True
         return self
-    
+
     def _one_hot_encode(self, y: Vector) -> Matrix:
         m = y.shape[0]
         n_classes = len(np.unique(y))
         one_hot = np.zeros((m, n_classes))
         one_hot[np.arange(m), y] = 1
         return one_hot
-    
+
     def _compute_loss(self, y_true: Matrix, y_pred: Matrix) -> float:
         m, _ = y_true.shape
         log_L = -np.log(y_pred[range(m), y_true.argmax(axis=1)] + 1e-8)
         cross_entropy = np.sum(log_L) / m
-        
-        l2_reg = (self.lambda_ / (2 * m))
+
+        l2_reg = self.lambda_ / (2 * m)
         l2_reg *= np.sum([np.square(w).sum() for w in self.weights])
         return cross_entropy + l2_reg
-    
+
     def _forward_pass(self, X: Matrix, is_train: bool = False) -> Matrix:
         a = X
         for i in range(self.n_layers - 1):
             z = np.dot(a, self.weights[i]) + self.biases[i]
             a = self.act_.func(z)
             if is_train:
                 mask = self.rs_.binomial(1, 1 - self.dropout_rate, a.shape)
                 mask = mask.astype(float) / (1 - self.dropout_rate)
                 a *= mask
-        
+
         z = np.dot(a, self.weights[-1]) + self.biases[-1]
         a = self.softmax_.func(z)
         return a
-    
+
     def _backpropagation(self, X: Matrix, y: Matrix) -> None:
         m, _ = X.shape
         as_, zs_ = [X], []
         a = X
         for i in range(self.n_layers - 1):
             z = np.dot(a, self.weights[i]) + self.biases[i]
             a = self.act_.func(z)
             as_.append(a)
             zs_.append(z)
-        
+
         z = np.dot(a, self.weights[-1]) + self.biases[-1]
         a = self.softmax_.func(z)
         as_.append(a)
         zs_.append(z)
-        
+
         delta = a - y
         grad_weights, grad_biases = [], []
-        
+
         dW = np.dot(as_[-2].T, delta)
         dW += (self.lambda_ / m) * self.weights[-1]
         db = np.sum(delta, axis=0, keepdims=True) / m
         grad_weights.append(dW)
         grad_biases.append(db)
-        
+
         for i in range(self.n_layers - 2, -1, -1):
             delta = np.dot(delta, self.weights[i + 1].T)
             delta *= self.act_.derivative(as_[i + 1])
-            
+
             dW = np.dot(as_[i].T, delta)
             dW += (self.lambda_ / m) * self.weights[i]
             db = np.sum(delta, axis=0, keepdims=True) / m
-            
+
             grad_weights.insert(0, dW)
             grad_biases.insert(0, db)
-        
+
         self.weights, self.biases = self.optimizer.update(
             self.weights, self.biases, grad_weights, grad_biases
         )
-    
+
     def predict(self, X: Matrix) -> Vector:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         y_pred = self._forward_pass(X)
         return np.argmax(y_pred, axis=1)
-    
+
     def predict_proba(self, X: Matrix) -> Vector:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         return self._forward_pass(X)
-    
-    def score(self, X: Matrix, y: Matrix, 
-              metric: Evaluator = Accuracy) -> float:
+
+    def score(self, X: Matrix, y: Matrix, metric: Evaluator = Accuracy) -> float:
         X_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=X_pred)
-    
+
     def dump(self, padding: int = 4) -> None:
         lines = []
         lines.append("MLP Classifier Configuration")
         lines.append(f"Input Size: {self.input_size:,}")
-        
+
         total_params = 0
         layers = self.layer_sizes
         for i, (in_, out_) in enumerate(zip(layers[:-1], layers[1:])):
             params_W = in_ * out_
             params_b = out_
             params_ = params_W + params_b
             total_params += params_
-            
+
             type_ = "Hidden" if i < len(self.layer_sizes) - 2 else "Output"
-            lines.append(f"Layer {i + 1} ({type_}): {in_:,} -> {out_:,}, " + 
-                         f"Parameters: {params_W:,} + {params_b:,} = {params_:,}")
-        
+            lines.append(
+                f"Layer {i + 1} ({type_}): {in_:,} -> {out_:,}, "
+                + f"Parameters: {params_W:,} + {params_b:,} = {params_:,}"
+            )
+
         lines.append(f"Output Size: {self.output_size:,}")
         lines.append(f"Total Parameters: {total_params:,}")
         lines.append(f"Activation Function: {type(self.act_).__name__}")
         lines.append(f"Optimizer: {type(self.optimizer).__name__}")
         box_width = max(len(line) for line in lines) + 2 * padding
         print("+" + "-" * (box_width - 2) + "+")
-        
-        for line in lines: print("|" + line.center(box_width - 2) + "|")
-        print("+" + "-" * (box_width - 2) + "+")
 
+        for line in lines:
+            print("|" + line.center(box_width - 2) + "|")
+        print("+" + "-" * (box_width - 2) + "+")
```

### Comparing `luma-ml-0.6.4/luma/neural/optimizer.py` & `luma-ml-0.6.5/luma/neural/optimizer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,168 +1,203 @@
 from typing import Tuple, List
 import numpy as np
 
 from luma.core.super import Optimizer
 from luma.interface.util import Matrix
 
 
-__all__ = (
-    'SGDOptimizer',
-    'MomentumOptimizer',
-    'RMSPropOptimizer',
-    'AdamOptimizer'
-)
+__all__ = ("SGDOptimizer", "MomentumOptimizer", "RMSPropOptimizer", "AdamOptimizer")
 
 
 class SGDOptimizer(Optimizer):
     def __init__(self, learning_rate: float = 0.01) -> None:
         self.learning_rate = learning_rate
-    
-    def update(self, 
-               weights: List[Matrix], 
-               biases: List[Matrix], 
-               grad_weights: List[Matrix], 
-               grad_biases: List[Matrix]) -> Tuple[List[Matrix]]:
+
+        self.set_param_ranges({"learning_rate": ("0<,+inf", None)})
+        self.check_param_ranges()
+
+    def update(
+        self,
+        weights: List[Matrix],
+        biases: List[Matrix],
+        grad_weights: List[Matrix],
+        grad_biases: List[Matrix],
+    ) -> Tuple[List[Matrix]]:
         updated_weights = []
         for w, grad_w in zip(weights, grad_weights):
             new_weight = w - self.learning_rate * grad_w
             updated_weights.append(new_weight)
-        
+
         updated_biases = []
         for b, grad_b in zip(biases, grad_biases):
             new_bias = b - self.learning_rate * grad_b
             updated_biases.append(new_bias)
-        
+
         return updated_weights, updated_biases
 
 
 class MomentumOptimizer(Optimizer):
-    def __init__(self, 
-                 learning_rate: float = 0.01, 
-                 momentum: float = 0.9) -> None:
+    def __init__(self, learning_rate: float = 0.01, momentum: float = 0.9) -> None:
         self.learning_rate = learning_rate
         self.momentum = momentum
         self.vel_weights = None
         self.vel_biases = None
 
-    def update(self, 
-               weights: List[Matrix], 
-               biases: List[Matrix], 
-               grad_weights: List[Matrix], 
-               grad_biases: List[Matrix]) -> Tuple[List[Matrix]]:
+        self.set_param_ranges(
+            {"learning_rate": ("0<,+inf", None), "momentum": ("0,1", None)}
+        )
+        self.check_param_ranges()
+
+    def update(
+        self,
+        weights: List[Matrix],
+        biases: List[Matrix],
+        grad_weights: List[Matrix],
+        grad_biases: List[Matrix],
+    ) -> Tuple[List[Matrix]]:
         if self.vel_weights is None:
             self.vel_weights = [np.zeros_like(w) for w in weights]
         if self.vel_biases is None:
             self.vel_biases = [np.zeros_like(b) for b in biases]
-        
+
         updated_weights = []
         for w, v_w, grad_w in zip(weights, self.vel_weights, grad_weights):
             v_w = self.momentum * v_w - self.learning_rate * grad_w
             updated_weights.append(w + v_w)
 
         updated_biases = []
         for b, v_b, grad_b in zip(biases, self.vel_biases, grad_biases):
             v_b = self.momentum * v_b - self.learning_rate * grad_b
             updated_biases.append(b + v_b)
-        
-        self.vel_weights = [self.momentum * v_w - self.learning_rate * grad_w 
-                            for v_w, grad_w in zip(self.vel_weights, grad_weights)]
-        
-        self.vel_biases = [self.momentum * v_b - self.learning_rate * grad_b 
-                           for v_b, grad_b in zip(self.vel_biases, grad_biases)]
+
+        self.vel_weights = [
+            self.momentum * v_w - self.learning_rate * grad_w
+            for v_w, grad_w in zip(self.vel_weights, grad_weights)
+        ]
+
+        self.vel_biases = [
+            self.momentum * v_b - self.learning_rate * grad_b
+            for v_b, grad_b in zip(self.vel_biases, grad_biases)
+        ]
 
         return updated_weights, updated_biases
 
 
 class RMSPropOptimizer(Optimizer):
-    def __init__(self,
-                 learning_rate: float = 0.01,
-                 decay_rate: float = 0.9) -> None:
+    def __init__(self, learning_rate: float = 0.01, decay_rate: float = 0.9) -> None:
         self.learning_rate = learning_rate
         self.decay_rate = decay_rate
         self.sq_grad_weights = None
         self.sq_grad_biases = None
-    
-    def update(self,
-               weights: List[Matrix],
-               biases: List[Matrix],
-               grad_weights: List[Matrix],
-               grad_biases: List[Matrix]) -> Tuple[List[Matrix]]:
+
+        self.set_param_ranges(
+            {"learning_rate": ("0<,+inf", None), "decay_rate": ("0,1", None)}
+        )
+        self.check_param_ranges()
+
+    def update(
+        self,
+        weights: List[Matrix],
+        biases: List[Matrix],
+        grad_weights: List[Matrix],
+        grad_biases: List[Matrix],
+    ) -> Tuple[List[Matrix]]:
         if self.sq_grad_weights is None:
             self.sq_grad_weights = [np.zeros_like(w) for w in weights]
         if self.sq_grad_biases is None:
             self.sq_grad_biases = [np.zeros_like(b) for b in biases]
-        
+
         updated_weights = []
         for w, sq_g_w, grad_w in zip(weights, self.sq_grad_weights, grad_weights):
             sq_g_w *= self.decay_rate
             sq_g_w += (1 - self.decay_rate) * np.square(grad_w)
             w -= self.learning_rate * grad_w / (np.sqrt(sq_g_w) + 1e-8)
             updated_weights.append(w)
-        
+
         updated_biases = []
         for b, sq_g_b, grad_b in zip(biases, self.sq_grad_biases, grad_biases):
             sq_g_b *= self.decay_rate
             sq_g_b += (1 - self.decay_rate) * np.square(grad_b)
             b -= self.learning_rate * grad_b / (np.sqrt(sq_g_b) + 1e-8)
             updated_biases.append(b)
-        
+
         self.sq_grad_weights = [
-            self.decay_rate * sq_g_w + (1 - self.decay_rate) * np.square(grad_w) 
+            self.decay_rate * sq_g_w + (1 - self.decay_rate) * np.square(grad_w)
             for sq_g_w, grad_w in zip(self.sq_grad_weights, grad_weights)
         ]
         self.sq_grad_biases = [
-            self.decay_rate * sq_g_b + (1 - self.decay_rate) * np.square(grad_b) 
+            self.decay_rate * sq_g_b + (1 - self.decay_rate) * np.square(grad_b)
             for sq_g_b, grad_b in zip(self.sq_grad_biases, grad_biases)
         ]
-        
+
         return updated_weights, updated_biases
 
 
-class AdamOptimizer:
-    def __init__(self, 
-                 learning_rate: float = 0.001, 
-                 beta_1: float = 0.9, 
-                 beta_2: float = 0.999,
-                 epsilon: float = 1e-8):
+class AdamOptimizer(Optimizer):
+    def __init__(
+        self,
+        learning_rate: float = 0.001,
+        beta_1: float = 0.9,
+        beta_2: float = 0.999,
+        epsilon: float = 1e-8,
+    ):
         self.learning_rate = learning_rate
         self.beta_1 = beta_1
         self.beta_2 = beta_2
         self.epsilon = epsilon
-        self.m_weights = None  # First moment vector for weights
-        self.v_weights = None  # Second moment vector for weights
-        self.m_biases = None   # First moment vector for biases
-        self.v_biases = None   # Second moment vector for biases
-        self.t = 0  # Initialization of the timestep
-
-    def update(self, 
-               weights: Matrix, 
-               biases: Matrix, 
-               grad_weights: Matrix, 
-               grad_biases: Matrix) -> Tuple[Matrix, Matrix]:
+        self.m_weights = None
+        self.v_weights = None
+        self.m_biases = None
+        self.v_biases = None
+        self.t = 0
+
+        self.set_param_ranges(
+            {
+                "learning_rate": ("0<,+inf", None),
+                "beta_1": ("0,1", None),
+                "beta_2": ("0,1", None),
+            }
+        )
+        self.check_param_ranges()
+
+    def update(
+        self, weights: Matrix, biases: Matrix, grad_weights: Matrix, grad_biases: Matrix
+    ) -> Tuple[Matrix, Matrix]:
         if self.m_weights is None:
             self.m_weights = [np.zeros_like(w) for w in weights]
             self.v_weights = [np.zeros_like(w) for w in weights]
         if self.m_biases is None:
             self.m_biases = [np.zeros_like(b) for b in biases]
             self.v_biases = [np.zeros_like(b) for b in biases]
-        
+
         self.t += 1
         updated_weights, updated_biases = [], []
-        
-        # Update parameters
+
         for i in range(len(weights)):
-            self.m_weights[i] = self.beta_1 * self.m_weights[i] + (1 - self.beta_1) * grad_weights[i]
-            self.v_weights[i] = self.beta_2 * self.v_weights[i] + (1 - self.beta_2) * np.square(grad_weights[i])
-            m_hat_w = self.m_weights[i] / (1 - self.beta_1 ** self.t)
-            v_hat_w = self.v_weights[i] / (1 - self.beta_2 ** self.t)
-            updated_weights.append(weights[i] - self.learning_rate * m_hat_w / (np.sqrt(v_hat_w) + self.epsilon))
+            self.m_weights[i] = (
+                self.beta_1 * self.m_weights[i] + (1 - self.beta_1) * grad_weights[i]
+            )
+            self.v_weights[i] = self.beta_2 * self.v_weights[i] + (
+                1 - self.beta_2
+            ) * np.square(grad_weights[i])
+            m_hat_w = self.m_weights[i] / (1 - self.beta_1**self.t)
+            v_hat_w = self.v_weights[i] / (1 - self.beta_2**self.t)
+            updated_weights.append(
+                weights[i]
+                - self.learning_rate * m_hat_w / (np.sqrt(v_hat_w) + self.epsilon)
+            )
 
         for i in range(len(biases)):
-            self.m_biases[i] = self.beta_1 * self.m_biases[i] + (1 - self.beta_1) * grad_biases[i]
-            self.v_biases[i] = self.beta_2 * self.v_biases[i] + (1 - self.beta_2) * np.square(grad_biases[i])
-            m_hat_b = self.m_biases[i] / (1 - self.beta_1 ** self.t)
-            v_hat_b = self.v_biases[i] / (1 - self.beta_2 ** self.t)
-            updated_biases.append(biases[i] - self.learning_rate * m_hat_b / (np.sqrt(v_hat_b) + self.epsilon))
+            self.m_biases[i] = (
+                self.beta_1 * self.m_biases[i] + (1 - self.beta_1) * grad_biases[i]
+            )
+            self.v_biases[i] = self.beta_2 * self.v_biases[i] + (
+                1 - self.beta_2
+            ) * np.square(grad_biases[i])
+            m_hat_b = self.m_biases[i] / (1 - self.beta_1**self.t)
+            v_hat_b = self.v_biases[i] / (1 - self.beta_2**self.t)
+            updated_biases.append(
+                biases[i]
+                - self.learning_rate * m_hat_b / (np.sqrt(v_hat_b) + self.epsilon)
+            )
 
         return updated_weights, updated_biases
-
```

### Comparing `luma-ml-0.6.4/luma/neural/single.py` & `luma-ml-0.6.5/luma/neural/single.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,206 +5,230 @@
 from luma.interface.exception import NotFittedError, UnsupportedParameterError
 from luma.interface.util import Matrix, Vector
 from luma.preprocessing.encoder import LabelBinarizer
 from luma.metric.classification import Accuracy
 from luma.metric.regression import MeanSquaredError
 
 
-__all__ = (
-    'PerceptronClassifier',
-    'PerceptronRegressor'
-)
+__all__ = ("PerceptronClassifier", "PerceptronRegressor")
 
 
 class PerceptronClassifier(Estimator, Supervised):
-    
     """
-    A perceptron classifier is a simple linear binary classifier used in 
-    machine learning. It makes predictions based on a linear combination of 
-    input features and weights, followed by an activation function. The 
-    perceptron updates its weights during training, aiming to correctly 
-    classify training examples. It iteratively adjusts weights based on the 
-    difference between predicted and actual outcomes. The perceptron's 
-    simplicity makes it foundational in understanding more complex neural 
+    A perceptron classifier is a simple linear binary classifier used in
+    machine learning. It makes predictions based on a linear combination of
+    input features and weights, followed by an activation function. The
+    perceptron updates its weights during training, aiming to correctly
+    classify training examples. It iteratively adjusts weights based on the
+    difference between predicted and actual outcomes. The perceptron's
+    simplicity makes it foundational in understanding more complex neural
     networks.
-    
+
     Parameters
     ----------
     `learning_rate` : Step size for updating weights
     `max_iter` : Maximum iteration
     `regularization` : Regularizing methods (e.g. `l1`, `l2`, `elastic-net`)
     `alpha` : Regularization strength
     `l1_ratio` : Ratio of `l1` (Only use when `elastic-net` regularization)
     `random_state` : Seed for random shuffling during SGD
-    
-    """    
-    
-    def __init__(self, 
-                 learning_rate: float = 0.01,
-                 max_iter: int = 1000,
-                 regularization: Literal['l1', 'l2', 'elastic-net'] = None,
-                 alpha: float = 0.0001,
-                 l1_ratio: float = 0.5,
-                 random_state: int = None,
-                 verbose: bool = False) -> None:
+
+    """
+
+    def __init__(
+        self,
+        learning_rate: float = 0.01,
+        max_iter: int = 1000,
+        regularization: Literal["l1", "l2", "elastic-net"] = None,
+        alpha: float = 0.0001,
+        l1_ratio: float = 0.5,
+        random_state: int = None,
+        verbose: bool = False,
+    ) -> None:
         self.learning_rate = learning_rate
         self.max_iter = max_iter
         self.regularization = regularization
         self.alpha = alpha
         self.l1_ratio = l1_ratio
         self.random_state = random_state
         self.verbose = verbose
         self.weights_ = None
         self._fitted = False
-    
-    def fit(self, X: Matrix, y: Vector) -> 'PerceptronClassifier':
+
+        self.set_param_ranges(
+            {
+                "learning_rate": ("0<,+inf", None),
+                "max_iter": ("0<,+inf", int),
+                "alpha": ("0,+inf", None),
+                "l1_ratio": ("0,1", None),
+            }
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix, y: Vector) -> "PerceptronClassifier":
         m, n = X.shape
         np.random.seed(self.random_state)
         n_classes = len(np.unique(y))
-        
+
         X = self._add_bias(X)
         y_binary = LabelBinarizer().fit_transform(y)
         self.weights_ = np.random.uniform(-0.01, 0.01, (n_classes, n + 1))
-        
+
         for i in range(self.max_iter):
             indices = np.arange(m)
             np.random.shuffle(indices)
             X, y_binary = X[indices], y_binary[indices]
-            
+
             for xi, yi in zip(X, y_binary):
                 linear_output = np.dot(self.weights_, xi)
                 y_pred = self._softmax(linear_output)
-                
+
                 self.weights_ += self.learning_rate * np.outer(yi - y_pred, xi)
                 if self.regularization:
                     self._regularize_weights()
 
             if self.verbose and i % 10 == 0:
-                print(f'[Perceptron] Iteration {i}/{self.max_iter}',
-                      f'with weight-norm: {np.linalg.norm(self.weights_)}')
-        
+                print(
+                    f"[Perceptron] Iteration {i}/{self.max_iter}",
+                    f"with weight-norm: {np.linalg.norm(self.weights_)}",
+                )
+
         self._fitted = True
         return self
-    
+
     def _add_bias(self, X: Matrix) -> Matrix:
         return np.insert(X, 0, 1, axis=1)
-    
+
     def _softmax(self, X: Matrix) -> Matrix:
         X = X.reshape(-1, X.shape[-1])
         exp = np.exp(X - np.max(X, axis=1, keepdims=True))
-        
+
         return exp / np.sum(exp, axis=1, keepdims=True)
-    
+
     def _regularize_weights(self) -> None:
-        if self.regularization == 'l1':
+        if self.regularization == "l1":
             self.weights_ -= self.alpha * np.sign(self.weights_)
-        elif self.regularization == 'l2':
+        elif self.regularization == "l2":
             self.weights_ -= self.alpha * self.weights_
-        elif self.regularization == 'elastic-net':
+        elif self.regularization == "elastic-net":
             l1_term = self.l1_ratio * np.sign(self.weights_)
             l2_term = (1 - self.l1_ratio) * self.weights_
             self.weights_ -= self.alpha * (l1_term + l2_term)
         else:
             UnsupportedParameterError(self.regularization)
-    
+
     def predict(self, X: Matrix) -> Vector:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         X = self._add_bias(X)
         linear_output = np.dot(X, self.weights_.T)
         y_pred = self._softmax(linear_output)
-        
+
         return np.argmax(y_pred, axis=1)
-    
-    def score(self, X: Matrix, y: Matrix, 
-              metric: Evaluator = Accuracy) -> float:
+
+    def score(self, X: Matrix, y: Matrix, metric: Evaluator = Accuracy) -> float:
         X_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=X_pred)
 
 
 class PerceptronRegressor(Estimator, Supervised):
-
     """
     Perceptron Regressor is a simple linear model used for regression tasks.
     It makes predictions based on a linear combination of input features and
     weights. The Perceptron Regressor updates its weights during training to
     minimize the difference between predicted and actual continuous outcomes.
     This model provides a basic understanding of linear regression in the
     context of neural networks.
-    
+
     Parameters
     ----------
     `learning_rate` : Step size for updating weights
     `max_iter` : Maximum iteration
     `random_state` : Seed for random shuffling during SGD
-    
+
     """
 
-    def __init__(self, 
-                 learning_rate: float = 0.01,
-                 max_iter: int = 1000,
-                 regularization: Literal['l1', 'l2', 'elastic-net'] = None,
-                 alpha: float = 0.0001,
-                 l1_ratio: float = 0.5,
-                 random_state: int = None,
-                 verbose: bool = False) -> None:
+    def __init__(
+        self,
+        learning_rate: float = 0.01,
+        max_iter: int = 1000,
+        regularization: Literal["l1", "l2", "elastic-net"] = None,
+        alpha: float = 0.0001,
+        l1_ratio: float = 0.5,
+        random_state: int = None,
+        verbose: bool = False,
+    ) -> None:
         self.learning_rate = learning_rate
         self.max_iter = max_iter
         self.regularization = regularization
         self.alpha = alpha
         self.l1_ratio = l1_ratio
         self.random_state = random_state
         self.verbose = verbose
         self.weights_ = None
         self._fitted = False
 
-    def fit(self, X: Matrix, y: Vector) -> 'PerceptronRegressor':
+        self.set_param_ranges(
+            {
+                "learning_rate": ("0<,+inf", None),
+                "max_iter": ("0<,+inf", int),
+                "alpha": ("0,+inf", None),
+                "l1_ratio": ("0,1", None),
+            }
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix, y: Vector) -> "PerceptronRegressor":
         m, n = X.shape
         np.random.seed(self.random_state)
 
         X = self._add_bias(X)
         self.weights_ = np.random.uniform(-0.01, 0.01, n + 1)
 
         for i in range(self.max_iter):
             indices = np.arange(m)
             np.random.shuffle(indices)
             X, y = X[indices], y[indices]
 
             for xi, yi in zip(X, y):
                 y_pred = np.dot(self.weights_, xi)
                 error = yi - y_pred
-                
+
                 self.weights_ += self.learning_rate * error * xi
                 if self.regularization:
                     self._regularize_weights()
 
             if self.verbose and i % 10 == 0:
-                print(f'[Perceptron] Iteration {i}/{self.max_iter}',
-                      f'with weight-norm: {np.linalg.norm(self.weights_)}')
+                print(
+                    f"[Perceptron] Iteration {i}/{self.max_iter}",
+                    f"with weight-norm: {np.linalg.norm(self.weights_)}",
+                )
 
         self._fitted = True
         return self
 
     def _add_bias(self, X: Matrix) -> Matrix:
         return np.insert(X, 0, 1, axis=1)
-    
+
     def _regularize_weights(self) -> None:
-        if self.regularization == 'l1':
+        if self.regularization == "l1":
             self.weights_ -= self.alpha * np.sign(self.weights_)
-        elif self.regularization == 'l2':
+        elif self.regularization == "l2":
             self.weights_ -= self.alpha * self.weights_
-        elif self.regularization == 'elastic-net':
+        elif self.regularization == "elastic-net":
             l1_term = self.l1_ratio * np.sign(self.weights_)
             l2_term = (1 - self.l1_ratio) * self.weights_
             self.weights_ -= self.alpha * (l1_term + l2_term)
         else:
             UnsupportedParameterError(self.regularization)
 
     def predict(self, X: Matrix) -> Vector:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         X = self._add_bias(X)
         return np.dot(X, self.weights_)
 
-    def score(self, X: Matrix, y: Vector, 
-              metric: Evaluator = MeanSquaredError) -> float:
+    def score(
+        self, X: Matrix, y: Vector, metric: Evaluator = MeanSquaredError
+    ) -> float:
         y_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=y_pred)
-
```

### Comparing `luma-ml-0.6.4/luma/pipe/pipeline.py` & `luma-ml-0.6.5/luma/pipe/pipeline.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,43 +3,40 @@
 from luma.core.super import Estimator, Transformer, Evaluator
 from luma.core.super import Supervised
 from luma.interface.util import Matrix
 from luma.interface.exception import NotFittedError, UnsupportedParameterError
 from luma.metric.classification import Accuracy
 from luma.metric.regression import MeanSquaredError
 
-MT = TypeVar('MT', bound=Estimator | Transformer)
+MT = TypeVar("MT", bound=Estimator | Transformer)
 
 
-__all__ = (
-    'Pipeline'
-)
+__all__ = "Pipeline"
 
 
 class Pipeline(Estimator, Estimator.Meta):
-    
     """
-    A pipeline is a sequence of steps to process data and build a model. 
-    It includes data collection and preprocessing, model selection and training, 
-    evaluation, and deployment. This systematic approach ensures efficiency 
-    and accuracy in model development. Pipelines are often automated for 
+    A pipeline is a sequence of steps to process data and build a model.
+    It includes data collection and preprocessing, model selection and training,
+    evaluation, and deployment. This systematic approach ensures efficiency
+    and accuracy in model development. Pipelines are often automated for
     scalability and reproducibility in real-world applications.
-    
+
     Parameters
     ----------
     `models` : List of models \n
     You can assign labels to each model by encapsulating the label and the model
     inside a tuple. \n
     Otherwise, the name of the model is automatically assigned by default.
-    
+
     `param_dict` : Dictionary of parameters for each models \n
     You must specify the name(or label) of the model and its parameter name
     in the key of the dictionary. \n
     e.g. `{'model_name__param_name': value}`
-    
+
     Examples
     --------
     >>> pipe = Pipeline(
             models=[
                 ('trans_1', Transformer()),
                 ('trans_2', Transformer()),
                 ...,
@@ -50,169 +47,182 @@
                 'trans_2__param': List[Any],
                 ...,
                 'est__param': List[Any]
             }
         )
     >>> pipe.fit(X_train, y_train)
     >>> y_pred = pipe.predict(X_test)
-    
+
     Properties
     ----------
     Getting list of transformers:
         ```py
         @property
         def transformers(self) -> List[Transformer]
         ```
-    
+
     Getting final estimator:
         ```py
         @property
         def estimator(self) -> Estimator
         ```
-    
+
     Getting transformed data:
         ```py
         @property
         def transformed_data(self) -> Tuple[Matrix, Matrix]
         ```
-    
+
     Notes
     -----
     * To use `Pipeline` with visual methods of `luma.visual`, make sure to
     transform data using `pipe.transform()` if the pipeline sequence contains
     transformers
-    
+
     * More than one estimator might cause procedural failure
     * Not all the models are compatible with `Pipeline`
     * Type `MT` is a generic type for `Estimator` and `Transformer`
-    
+
     """
-    
-    def __init__(self,
-                 models: List[Tuple[str, MT]] | List[MT],
-                 param_dict: Dict[str, Any] = dict(),
-                 verbose: bool = False) -> None:
+
+    def __init__(
+        self,
+        models: List[Tuple[str, MT]] | List[MT],
+        param_dict: Dict[str, Any] = dict(),
+        verbose: bool = False,
+    ) -> None:
         self.models: Dict[MT] = dict()
         self.param_dict = param_dict
         self.verbose = verbose
         self._X: Matrix
         self._y: Matrix
         self._fitted = False
-        
+
         for model in models:
             if isinstance(model, tuple):
                 _name, _model = model
                 self.models[_name] = _model
-            else: self.models[type(model).__name__] = model
-        
+            else:
+                self.models[type(model).__name__] = model
+
         self.set_params(param_dict)
-    
-    def fit(self, X: Matrix, y: Matrix) -> 'Pipeline':
+
+    def fit(self, X: Matrix, y: Matrix) -> "Pipeline":
         self._X, self._y = self.fit_transform(X, y)
         model = self.estimator
-        if hasattr(model, 'verbose'):
+        if hasattr(model, "verbose"):
             model.verbose = self.verbose
-        
+
         data = [self._X]
-        if isinstance(model, Supervised): data.append(self._y)
+        if isinstance(model, Supervised):
+            data.append(self._y)
         model.fit(*data)
-        
+
         self._fitted = True
         return self
-        
+
     def transform(self, X: Matrix, y: Matrix) -> Tuple[Matrix, Matrix]:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         X_trans, y_trans = X, y
         for model in self.transformers:
             if isinstance(model, Transformer.Target):
                 y_trans = model.transform(y_trans)
             elif isinstance(model, Transformer.Both):
                 X_trans, y_trans = model.transform(X_trans, y_trans)
             else:
                 X_trans = model.transform(X_trans)
 
         return X_trans, y_trans
-    
+
     def predict(self, X: Matrix, transform: bool = True):
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         for model in self.transformers:
-            if not transform: break
+            if not transform:
+                break
             if isinstance(model, Transformer.Target | Transformer.Both):
                 continue
-            
+
             X = model.transform(X)
-        
+
         return self.estimator.predict(X)
-    
+
     def fit_transform(self, X: Matrix, y: Matrix) -> Tuple[Matrix, Matrix]:
         X_trans, y_trans = X, y
         for model in self.transformers:
             data = [X_trans]
-            if hasattr(model, 'verbose'):
+            if hasattr(model, "verbose"):
                 model.verbose = self.verbose
-            
+
             if isinstance(model, Supervised):
                 data.append(y_trans)
             if isinstance(model, Transformer.Target):
                 y_trans = model.fit_transform(y_trans)
             elif isinstance(model, Transformer.Both):
                 X_trans, y_trans = model.fit_transform(*data)
             else:
                 X_trans = model.fit_transform(*data)
 
         return X_trans, y_trans
-    
+
     def fit_predict(self, X: Matrix, y: Matrix) -> Matrix:
         self.fit(X, y)
         return self.predict(X)
-    
+
     def set_params(self, param_dict: Dict[str, Any]) -> None:
         for param_name, value in param_dict.items():
-            try: _name, _param = param_name.split('__')
-            except: raise UnsupportedParameterError(param_name)
+            try:
+                _name, _param = param_name.split("__")
+            except:
+                raise UnsupportedParameterError(param_name)
             self.models[_name].set_params(**{_param: value})
-    
-    def score(self, X: Matrix, y: Matrix, 
-              metric: Evaluator | Literal['default'] = 'default') -> float:
+
+    def score(
+        self, X: Matrix, y: Matrix, metric: Evaluator | Literal["default"] = "default"
+    ) -> float:
         model = self.estimator
-        pkg = model.__module__.split('.')[1]
-        if metric == 'default':
-            if pkg == 'classifier': metric = Accuracy
-            elif pkg == 'regressor': metric = MeanSquaredError
-        
+        pkg = model.__module__.split(".")[1]
+        if metric == "default":
+            if pkg == "classifier":
+                metric = Accuracy
+            elif pkg == "regressor":
+                metric = MeanSquaredError
+
         X_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=X_pred)
-    
+
     def dump(self) -> None:
         print(f"Configuration of a pipeline:")
         for name, model in self.models.items():
             print(f"\n[{type(model).__name__} as '{name}']")
             for attr in model.__dict__.items():
-                print(*attr, sep=': ')
-    
+                print(*attr, sep=": ")
+
     @property
     def transformers(self) -> List[Transformer]:
         _trans = []
         for model in self.models.values():
             if isinstance(model, Transformer):
                 _trans.append(model)
 
         return _trans
 
     @property
     def estimator(self) -> Estimator:
         for model in self.models.values():
             if isinstance(model, Estimator):
                 return model
-    
+
     @property
     def transformed_data(self) -> Tuple[Matrix, Matrix]:
         return self._X, self._y
-    
+
     def __getitem__(self, index: int) -> MT:
         for i, model in enumerate(self.models.values()):
-            if index == i: return model
-        else: raise IndexError('Model index out of bounds!')
-    
+            if index == i:
+                return model
+        else:
+            raise IndexError("Model index out of bounds!")
+
     def __setitem__(self, label: str, model: MT):
         self.models[label] = model
-
```

### Comparing `luma-ml-0.6.4/luma/preprocessing/encoder.py` & `luma-ml-0.6.5/luma/preprocessing/encoder.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,156 +2,161 @@
 import numpy as np
 
 from luma.core.super import Transformer
 from luma.interface.util import Matrix, Vector
 from luma.interface.exception import NotFittedError, UnsupportedParameterError
 
 
-__all__ = (
-    'OneHotEncoder', 
-    'LabelEncoder', 
-    'OrdinalEncoder',
-    'LabelBinarizer'
-)
+__all__ = ("OneHotEncoder", "LabelEncoder", "OrdinalEncoder", "LabelBinarizer")
 
 
 class OneHotEncoder(Transformer, Transformer.Feature):
     def __init__(self, features: list = None):
         self.categories = None
         self.features = features
         self._fitted = False
 
-    def fit(self, X: Matrix) -> 'OneHotEncoder':
+    def fit(self, X: Matrix) -> "OneHotEncoder":
         if self.features is None:
             self.features = range(X.shape[1])
 
         self.categories = [np.unique(X[:, col]) for col in self.features]
         self._fitted = True
         return self
 
     def transform(self, X: Matrix) -> Matrix[int]:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
 
         X_out = []
         for i, col in enumerate(X.T):
             if i in self.features:
                 categories = self.categories[self.features.index(i)]
                 label_to_index = {label: idx for idx, label in enumerate(categories)}
                 matrix = np.zeros((len(X), len(categories)))
 
                 for j, item in enumerate(col):
-                    if item in label_to_index: matrix[j, label_to_index[item]] = 1
-                    elif item is np.nan: continue
-                    else: raise ValueError(f"Unknown label {item} found in column {i}")
+                    if item in label_to_index:
+                        matrix[j, label_to_index[item]] = 1
+                    elif item is np.nan:
+                        continue
+                    else:
+                        raise ValueError(f"Unknown label {item} found in column {i}")
                 X_out.append(matrix)
-                
-            else: X_out.append(X[:, i].reshape(-1, 1))
+
+            else:
+                X_out.append(X[:, i].reshape(-1, 1))
 
         return np.hstack(X_out).astype(int)
 
     def fit_transform(self, X: Matrix) -> Matrix[int]:
         self.fit(X)
         return self.transform(X)
 
 
 class LabelEncoder(Transformer, Transformer.Target):
     def __init__(self):
         self.classes = None
         self._fitted = False
 
-    def fit(self, y: Matrix) -> 'LabelEncoder':
+    def fit(self, y: Matrix) -> "LabelEncoder":
         self.classes = np.unique(y)
         self._fitted = True
         return self
 
     def transform(self, y: Matrix) -> Matrix[int]:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         class_to_index = {k: v for v, k in enumerate(self.classes)}
-        
+
         X_transformed = Matrix([class_to_index.get(y_, -1) for y_ in y])
         if -1 in X_transformed:
             raise ValueError("Unknown label found in input data.")
 
         return X_transformed
-    
+
     def inverse_transform(self, y: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         index_to_class = {v: k for k, v in enumerate(self.classes)}
-        
+
         X_inversed = Matrix([index_to_class.get(y_, None) for y_ in y])
         if None in X_inversed:
             raise ValueError("Unknown index found in input data.")
 
         return X_inversed
 
     def fit_transform(self, y: Matrix) -> Matrix[int]:
         self.fit(y)
         return self.transform(y)
 
 
 class OrdinalEncoder(Transformer, Transformer.Feature):
-    def __init__(self, 
-                 strategy: Literal['occur', 'alpha'] = 'occur'):
+    def __init__(self, strategy: Literal["occur", "alpha"] = "occur"):
         self.categories = None
         self.strategy = strategy
         self._fitted = False
 
-    def fit(self, X: Matrix) -> 'OrdinalEncoder':
-        if self.strategy == 'occur':
+    def fit(self, X: Matrix) -> "OrdinalEncoder":
+        if self.strategy == "occur":
             self.categories = [np.unique(col, return_index=True)[0] for col in X.T]
-        elif self.strategy == 'alpha':
+        elif self.strategy == "alpha":
             self.categories = [np.sort(np.unique(col)) for col in X.T]
-        else: raise UnsupportedParameterError(self.strategy)
+        else:
+            raise UnsupportedParameterError(self.strategy)
 
         self._fitted = True
         return self
 
     def transform(self, X: Matrix) -> Matrix[int]:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         X_out = np.zeros(X.shape, dtype=int)
-        
+
         for i, categories in enumerate(self.categories):
-            category_to_index = {category: index 
-                                 for index, category in enumerate(categories)}
+            category_to_index = {
+                category: index for index, category in enumerate(categories)
+            }
             for j, item in enumerate(X[:, i]):
                 if item in category_to_index:
                     X_out[j, i] = category_to_index[item]
-                else: raise ValueError(f"Unknown label {item} found in column {i}")
+                else:
+                    raise ValueError(f"Unknown label {item} found in column {i}")
 
         return X_out
 
     def fit_transform(self, X: Matrix) -> Matrix[int]:
         self.fit(X)
         return self.transform(X)
 
 
 class LabelBinarizer(Transformer, Transformer.Target):
     def __init__(self, negative_target: bool = False) -> None:
         self.negative_target = negative_target
         self.classes_ = None
         self._fitted = False
 
-    def fit(self, y: Vector) -> 'LabelBinarizer':
+    def fit(self, y: Vector) -> "LabelBinarizer":
         self.classes_ = np.unique(y)
         self._fitted = True
         return self
 
     def transform(self, y: Vector) -> Vector:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         if self.negative_target:
             binarized = np.full((len(y), len(self.classes_)), -1)
         else:
             binarized = np.full((len(y), len(self.classes_)), 0)
-        
+
         for i, label in enumerate(y):
             class_index = np.where(self.classes_ == label)[0][0]
             binarized[i, class_index] = 1
-        
+
         return binarized
-    
+
     def fit_transform(self, y: Vector) -> Vector:
         self.fit(y)
         return self.transform(y)
 
     def inverse_transform(self, y: Vector) -> Vector:
         return self.classes_[np.argmax(y, axis=1)]
-
```

### Comparing `luma-ml-0.6.4/luma/preprocessing/imputer.py` & `luma-ml-0.6.5/luma/preprocessing/imputer.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,129 +5,141 @@
 import pandas as pd
 
 from luma.interface.util import Matrix
 from luma.core.super import Transformer
 from luma.interface.exception import NotFittedError, UnsupportedParameterError
 
 
-__all__ = (
-    'SimpleImputer', 
-    'KNNImputer', 
-    'HotDeckImputer'
-)
+__all__ = ("SimpleImputer", "KNNImputer", "HotDeckImputer")
 
 
 class SimpleImputer(Transformer, Transformer.Feature):
-    def __init__(self, 
-                 strategy: Literal['mean', 'median', 'mode'] = 'mean'):
+    def __init__(self, strategy: Literal["mean", "median", "mode"] = "mean"):
         self.strategy = strategy
         self.statistics = None
         self._fitted = False
 
-    def fit(self, X: Matrix) -> 'SimpleImputer':
-        if self.strategy == 'mean':
+    def fit(self, X: Matrix) -> "SimpleImputer":
+        if self.strategy == "mean":
             self.statistics = np.nanmean(X, axis=0)
-        elif self.strategy == 'median':
+        elif self.strategy == "median":
             self.statistics = np.nanmedian(X, axis=0)
-        elif self.strategy == 'mode':
+        elif self.strategy == "mode":
             self.statistics = []
-            
+
             for x_col in X.T:
                 if np.issubdtype(x_col.dtype, np.number):
-                    column_mode, _ = mode(x_col, nan_policy='omit')
-                    self.statistics.append(column_mode if column_mode.size > 0 else np.nan)
+                    column_mode, _ = mode(x_col, nan_policy="omit")
+                    self.statistics.append(
+                        column_mode if column_mode.size > 0 else np.nan
+                    )
                 else:
-                    unique, counts = np.unique(x_col[~pd.isnull(x_col)], return_counts=True)
-                    if unique.size > 0: self.statistics.append(unique[np.argmax(counts)])
-                    else: self.statistics.append(np.nan)
-        
-        else: raise UnsupportedParameterError(self.strategy)
-        
+                    unique, counts = np.unique(
+                        x_col[~pd.isnull(x_col)], return_counts=True
+                    )
+                    if unique.size > 0:
+                        self.statistics.append(unique[np.argmax(counts)])
+                    else:
+                        self.statistics.append(np.nan)
+
+        else:
+            raise UnsupportedParameterError(self.strategy)
+
         self._fitted = True
         return self
 
     def transform(self, X: Matrix) -> Matrix:
-        if not self._fitted: NotFittedError(self)
+        if not self._fitted:
+            NotFittedError(self)
         X_imp = X.copy()
         for i, stat in enumerate(self.statistics):
             if np.issubdtype(X_imp[:, i].dtype, np.number):
                 X_imp[:, i] = X_imp[:, i].astype(float)
                 mask = np.isnan(X_imp[:, i])
                 X_imp[mask, i] = stat
             else:
-                mask = pd.isnull(X_imp[:, i]) | (X_imp[:, i] == 'nan')
+                mask = pd.isnull(X_imp[:, i]) | (X_imp[:, i] == "nan")
                 X_imp[mask, i] = stat
-        
+
         X_ret = np.zeros_like(X_imp, dtype=object)
         for i in range(X_imp.shape[1]):
-            try: X_ret[:, i] = X_imp[:, i].astype(float)
-            except: X_ret[:, i] = X_imp[:, i]
-        
+            try:
+                X_ret[:, i] = X_imp[:, i].astype(float)
+            except:
+                X_ret[:, i] = X_imp[:, i]
+
         return X_ret
 
     def fit_transform(self, X: Matrix) -> Matrix:
         self.fit(X)
         return self.transform(X)
 
 
 class KNNImputer(Transformer, Transformer.Feature):
     def __init__(self, n_neighbors: int = 5):
         self.n_neighbors = n_neighbors
         self.distances = None
         self._fitted = False
 
-    def fit(self, X: Matrix) -> 'KNNImputer':
+        self.set_param_ranges({"n_neighbors": ("0<,+inf", int)})
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix) -> "KNNImputer":
         if np.isnan(X).any():
             self.distances = self._compute_distances(X)
-        
+
         self._fitted = True
         return self
 
     def transform(self, X: Matrix) -> Matrix:
-        if not self._fitted: NotFittedError(self)
+        if not self._fitted:
+            NotFittedError(self)
         X_imp = X.copy()
-        
+
         for i, row in enumerate(X):
             nan_indices = np.where(np.isnan(row))[0]
             for x_col in nan_indices:
                 neighbor_indices = np.argsort(self.distances[i])
                 neighbor_values = []
-                
+
                 for neighbor_index in neighbor_indices:
                     if not np.isnan(X[neighbor_index, x_col]) and neighbor_index != i:
                         neighbor_values.append(X[neighbor_index, x_col])
-                        if len(neighbor_values) == self.n_neighbors: break
+                        if len(neighbor_values) == self.n_neighbors:
+                            break
 
-                if neighbor_values: X_imp[i, x_col] = np.mean(neighbor_values)
-                else: X_imp[i, x_col] = np.nanmean(X[:, x_col])
+                if neighbor_values:
+                    X_imp[i, x_col] = np.mean(neighbor_values)
+                else:
+                    X_imp[i, x_col] = np.nanmean(X[:, x_col])
 
         return X_imp
 
     def fit_transform(self, X: Matrix) -> Matrix:
         self.fit(X)
         return self.transform(X)
 
     def _compute_distances(self, X: Matrix) -> Matrix:
         nan_replacement = np.nanmax(X) + 1
         data_without_nan = np.where(np.isnan(X), nan_replacement, X)
-        distances = cdist(data_without_nan, data_without_nan, metric='euclidean')
-        
+        distances = cdist(data_without_nan, data_without_nan, metric="euclidean")
+
         return distances
 
 
 class HotDeckImputer(Transformer, Transformer.Feature):
     def __init__(self):
         self._X = None
         self._similar_rows = None
         self._fitted = False
 
-    def fit(self, X: Matrix) -> 'HotDeckImputer':
+    def fit(self, X: Matrix) -> "HotDeckImputer":
         self._X = X
         self._similar_rows = [self._find_similar_row(row) for row in self._X]
-        
+
         self._fitted = True
         return self
 
     def _find_similar_row(self, row: Matrix) -> Matrix:
         min_diff = np.inf
         similar_row = None
 
@@ -141,15 +153,16 @@
         return similar_row
 
     def transform(self, X: Matrix) -> Matrix:
         imputed_data = X.copy()
         for i, row in enumerate(imputed_data):
             if np.any(np.isnan(row)) and self._similar_rows[i] is not None:
                 missing_indices = np.where(np.isnan(row))[0]
-                imputed_data[i, missing_indices] = self._similar_rows[i][missing_indices]
+                imputed_data[i, missing_indices] = self._similar_rows[i][
+                    missing_indices
+                ]
 
         return imputed_data
 
     def fit_transform(self, X: Matrix) -> Matrix:
         self.fit(X)
         return self.transform(X)
-
```

### Comparing `luma-ml-0.6.4/luma/preprocessing/outlier.py` & `luma-ml-0.6.5/luma/preprocessing/outlier.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,103 +3,105 @@
 import numpy as np
 
 from luma.core.super import Transformer, Supervised
 from luma.interface.util import Matrix, Vector
 from luma.interface.exception import NotFittedError
 
 
-__all__ = (
-    'LocalOutlierFactor'
-)
+__all__ = "LocalOutlierFactor"
 
 
 class LocalOutlierFactor(Transformer, Transformer.Both, Supervised):
-    
     """
-    The Local Outlier Factor (LOF) algorithm identifies outliers by comparing 
-    the local density of a data point with the densities of its neighbors. 
-    Points with significantly lower density than their neighbors are considered 
-    outliers. LOF scores greater than 1 indicate potential outliers. It is 
-    effective in datasets with varying densities and does not require a prior 
+    The Local Outlier Factor (LOF) algorithm identifies outliers by comparing
+    the local density of a data point with the densities of its neighbors.
+    Points with significantly lower density than their neighbors are considered
+    outliers. LOF scores greater than 1 indicate potential outliers. It is
+    effective in datasets with varying densities and does not require a prior
     assumption about the data distribution.
-    
+
     Parameters
     ----------
     `n_neighbors` : Number of neighbors to estimate the local densities
-    
+
     Examples
     --------
     >>> lof = LocalOutlierFactor()
     >>> lof.fit(X)
-    
+
     Getting LOF Scores
     >>> lof_scores = lof.get_scores(X)
-    
+
     Filtering Dataset
     >>> X_, y_ = lof.filter(X, y) # or lof.transform(X, y)
-    
+
     """
-    
-    def __init__(self, 
-                 n_neighbors: int = 10,
-                 threshold: float = 1.5):
+
+    def __init__(self, n_neighbors: int = 10, threshold: float = 1.5):
         self.n_neighbors = n_neighbors
         self.threshold = threshold
         self.lrd_ = None
         self.neighbors_ = None
         self._fitted = False
-    
-    def fit(self, X: Matrix, _ = None) -> 'LocalOutlierFactor':
+
+        self.set_param_ranges(
+            {"n_neighbors": ("0<,+inf", int), "threshold": ("0,+inf", None)}
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix, _=None) -> "LocalOutlierFactor":
         n_samples = len(X)
         self.lrd_ = np.zeros(n_samples)
         self.neighbors_ = []
 
         for i in range(n_samples):
             distances = cdist([X[i]], X)[0]
-            neighbors_idx = np.argsort(distances)[1:self.n_neighbors + 1]
+            neighbors_idx = np.argsort(distances)[1 : self.n_neighbors + 1]
             neighbors = X[neighbors_idx]
 
             self.lrd_[i] = self._local_reachability_density(X[i], neighbors)
             self.neighbors_.append(neighbors_idx)
 
         self._fitted = True
         return self
 
     def _k_distance(self, x: Matrix, neighbors: Matrix) -> Matrix:
-        sorted_ = np.sort(cdist([x], neighbors)[0]) 
+        sorted_ = np.sort(cdist([x], neighbors)[0])
         return sorted_[self.n_neighbors - 1]
 
-    def _reachability_distance(self, x: Matrix, 
-                               neighbor: Matrix, 
-                               neighbors: Matrix) -> Matrix:
+    def _reachability_distance(
+        self, x: Matrix, neighbor: Matrix, neighbors: Matrix
+    ) -> Matrix:
         k_dist_neighbor = self._k_distance(neighbor, neighbors)
         return max(k_dist_neighbor, np.linalg.norm(x - neighbor))
 
-    def _local_reachability_density(self, x: Matrix, 
-                                    neighbors: Matrix) -> Matrix:
-        reach_distances = [self._reachability_distance(x, neighbor, neighbors) 
-                           for neighbor in neighbors]
-        return 1 / (np.sum(reach_distances) / len(neighbors) 
-                    if len(neighbors) > 0 else 1)
+    def _local_reachability_density(self, x: Matrix, neighbors: Matrix) -> Matrix:
+        reach_distances = [
+            self._reachability_distance(x, neighbor, neighbors)
+            for neighbor in neighbors
+        ]
+        return 1 / (
+            np.sum(reach_distances) / len(neighbors) if len(neighbors) > 0 else 1
+        )
 
     def get_scores(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         lof = np.zeros(len(X))
         for i in range(len(X)):
             lrd_sum = sum(self.lrd_[idx] for idx in self.neighbors_[i])
             lof[i] = lrd_sum / (self.n_neighbors * self.lrd_[i])
 
         return lof
-    
+
     def filter(self, X: Matrix, y: Matrix) -> Tuple[Matrix, Vector]:
         lof_scores = self.get_scores(X)
         condition = lof_scores < self.threshold
-        
+
         return X[condition], y[condition]
-    
+
     def transform(self, X: Matrix, y: Vector) -> Tuple[Matrix, Vector]:
         return self.filter(X, y)
-    
+
     def fit_transform(self, X: Matrix, y: Vector) -> Tuple[Matrix, Vector]:
         self.fit(X)
         return self.transform(X, y)
-
```

### Comparing `luma-ml-0.6.4/luma/preprocessing/scaler.py` & `luma-ml-0.6.5/luma/preprocessing/scaler.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,87 +1,85 @@
 import numpy as np
 
 from luma.interface.util import Matrix
 from luma.core.super import Transformer
 from luma.interface.exception import NotFittedError
 
 
-__all__ = (
-    'StandardScaler', 
-    'MinMaxScaler'
-)
+__all__ = ("StandardScaler", "MinMaxScaler")
 
 
 class StandardScaler(Transformer):
-    
     """
-    Standard scaling is a data preprocessing technique to transform 
+    Standard scaling is a data preprocessing technique to transform
     the data so that it has a mean of 0 and a standard deviation of 1.
     """
-    
+
     def __init__(self) -> None:
         self.mean = None
         self.std = None
         self._fitted = False
 
-    def fit(self, X: Matrix) -> 'StandardScaler':
+    def fit(self, X: Matrix) -> "StandardScaler":
         self.mean = np.mean(X, axis=0)
         self.std = np.std(X, axis=0, ddof=1)
         self._fitted = True
         return self
 
     def transform(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         epsilon = 1e-8
         return (X - self.mean) / (self.std + epsilon)
 
     def fit_transform(self, X: Matrix) -> Matrix:
         self.fit(X)
         return self.transform(X)
 
     def inverse_transform(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         return (X * self.std) + self.mean
 
 
 class MinMaxScaler(Transformer, Transformer.Feature):
-    
     """
     MinMax scaling (also known as Min-Max normalization)
-    to rescale features to a specific range, typically between 0 and 1. 
-    The purpose of MinMax scaling is to transform the features in a way 
+    to rescale features to a specific range, typically between 0 and 1.
+    The purpose of MinMax scaling is to transform the features in a way
     that they fall within a specific interval.
-    
+
     Parameters
     ----------
     `feature_range` : Range to be scaled
-    
+
     """
-    
+
     def __init__(self, feature_range: tuple = (0, 1)) -> None:
         self.feature_range = feature_range
         self.min = None
         self.max = None
         self._fitted = False
 
-    def fit(self, X: Matrix) -> 'MinMaxScaler':
+    def fit(self, X: Matrix) -> "MinMaxScaler":
         self.min = np.min(X, axis=0)
         self.max = np.max(X, axis=0)
         self._fitted = True
         return self
 
     def transform(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         min_val, max_val = self.feature_range
         scaled = (X - self.min) / (self.max - self.min) * (max_val - min_val)
         return scaled + min_val
 
     def fit_transform(self, X: Matrix) -> Matrix:
         self.fit(X)
         return self.transform(X)
 
     def inverse_transform(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         min_val, max_val = self.feature_range
         original = (X - min_val) / (max_val - min_val) * (self.max - self.min)
         return original + self.min
-
```

### Comparing `luma-ml-0.6.4/luma/reduction/linear.py` & `luma-ml-0.6.5/luma/reduction/linear.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,527 +1,568 @@
 from typing import Tuple
 from scipy.linalg import svd, eigh
 import numpy as np
 
 from luma.interface.util import Matrix, Vector, KernelUtil
 from luma.core.super import Transformer, Unsupervised, Supervised
-from luma.interface.exception import (NotFittedError,
-                                      NotConvergedError,
-                                      UnsupportedParameterError)
+from luma.interface.exception import (
+    NotFittedError,
+    NotConvergedError,
+    UnsupportedParameterError,
+)
 
 
-__all__ = (
-    'PCA', 
-    'LDA', 
-    'KDA', 
-    'CCA', 
-    'KernelPCA', 
-    'TruncatedSVD', 
-    'FactorAnalysis'
-)
+__all__ = ("PCA", "LDA", "KDA", "CCA", "KernelPCA", "TruncatedSVD", "FactorAnalysis")
 
 
 class PCA(Transformer, Unsupervised):
-    
     """
-    PCA, or Principal Component Analysis, is a dimensionality 
-    reduction technique. It's primarily used to simplify complex 
+    PCA, or Principal Component Analysis, is a dimensionality
+    reduction technique. It's primarily used to simplify complex
     data while retaining the most important information.
-    
+
     Parameters
     ----------
     `n_components` : Number of principal components
-    
+
     """
-    
+
     def __init__(self, n_components: int = None) -> None:
         self.n_components = n_components
         self._fitted = False
 
-    def fit(self, X: Matrix) -> 'PCA':
+        self.set_param_ranges({"n_components": ("0<,+inf", int)})
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix) -> "PCA":
         self.mean = np.mean(X, axis=0)
         X_centered = X - self.mean
         covariance_matrix = np.cov(X_centered, rowvar=False)
         eigenvalues, eigenvectors = np.linalg.eigh(covariance_matrix)
 
         sorted_indices = np.argsort(eigenvalues)[::-1]
         eigenvalues = eigenvalues[sorted_indices]
         eigenvectors = eigenvectors[:, sorted_indices]
 
         if self.n_components is not None:
-            self.eigenvalues = eigenvalues[:self.n_components]
-            self.eigenvectors = eigenvectors[:, :self.n_components]
+            self.eigenvalues = eigenvalues[: self.n_components]
+            self.eigenvectors = eigenvectors[:, : self.n_components]
         else:
             self.eigenvalues = eigenvalues
             self.eigenvectors = eigenvectors
-        
+
         self._fitted = True
         return self
 
     def transform(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         X_centered = X - self.mean
         return np.dot(X_centered, self.eigenvectors)
 
     def fit_transform(self, X: Matrix) -> Matrix:
         self.fit(X)
         return self.transform(X)
 
 
 class KernelPCA(Transformer, Unsupervised):
-    
     """
-    Kernel PCA is a dimensionality reduction technique that extends 
-    Principal Component Analysis (PCA) to capture complex, nonlinear 
-    relationships in data by using a kernel function to transform 
-    the data into a higher-dimensional space where nonlinear patterns 
+    Kernel PCA is a dimensionality reduction technique that extends
+    Principal Component Analysis (PCA) to capture complex, nonlinear
+    relationships in data by using a kernel function to transform
+    the data into a higher-dimensional space where nonlinear patterns
     can be better captured.
-    
+
     Parameters
     ----------
     `n_components` : Number of principal components
     `deg` : Polynomial degree of `poly` kernel
     `gamma` : Shape parameter of `rbf`, `sigmoid`, `laplacian`
     `coef` : Additional coefficient of `poly`, `sigmoid`
     `kernel` : Type of kernel functions
     (e.g. `linear`, `poly`, `rbf`, `sigmoid`, `laplacian`)
-    
+
     """
-    
-    def __init__(self, 
-                 n_components: int = None,
-                 deg: int = 3,
-                 gamma: float = 15.0,
-                 coef: float = 1.0,
-                 kernel: KernelUtil.func_type = 'rbf') -> None:
+
+    def __init__(
+        self,
+        n_components: int = None,
+        deg: int = 3,
+        gamma: float = 1.0,
+        coef: float = 1.0,
+        kernel: KernelUtil.FuncType = "rbf",
+    ) -> None:
         self.n_components = n_components
         self.deg = deg
         self.gamma = gamma
         self.coef = coef
         self.kernel = kernel
         self.X = None
         self._fitted = False
-    
-    def fit(self, X: Matrix) -> 'KernelPCA':
+
+        self.set_param_ranges(
+            {
+                "n_components": ("0<,+inf", int),
+                "deg": ("0,+inf", int),
+                "gamma": ("0<,+inf", None),
+            }
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix) -> "KernelPCA":
         self.X = X
         self._select_kernel_function()
         N = X.shape[0]
         self.K = self._compute_kernel_matrix(X, X)
-        
+
         one_n = np.ones((N, N)) / N
         self.K_centered = self.K - one_n.dot(self.K) - self.K.dot(one_n)
         self.K_centered += one_n.dot(self.K).dot(one_n)
-        
+
         self.eigvals, self.eigvecs = eigh(self.K_centered)
         self.eigvals, self.eigvecs = self.eigvals[::-1], self.eigvecs[:, ::-1]
 
         self._fitted = True
         return self
-    
+
     def transform(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
-        
+        if not self._fitted:
+            raise NotFittedError(self)
+
         K_new = self._compute_kernel_matrix(X, self.X)
         N = self.K.shape[0]
         one_N = np.ones((N, N)) / N
         one_new = np.ones((K_new.shape[0], N)) / N
-        
+
         K_new_centered = K_new - one_new.dot(self.K)
         K_new_centered += one_new.dot(one_N.dot(self.K))
         K_new_centered -= K_new.dot(one_N.mean(axis=0))
-        
-        proj = K_new_centered.dot(self.eigvecs[:, :self.n_components])
+
+        proj = K_new_centered.dot(self.eigvecs[:, : self.n_components])
         return proj
-    
+
     def fit_transform(self, X: Matrix) -> Matrix:
         self.fit(X)
         return self.transform(X)
-    
+
     def _compute_kernel_matrix(self, X: Matrix, Y: Matrix) -> Matrix:
         N, M = X.shape[0], Y.shape[0]
         K = np.zeros((N, M))
         for i in range(N):
             for j in range(M):
                 K[i, j] = self.kernel_func(X[i], Y[j])
         return K
-    
+
     def _select_kernel_function(self):
-        if self.kernel == 'linear': self.kernel_func = self._linear
-        elif self.kernel == 'poly': self.kernel_func = self._poly
-        elif self.kernel == 'rbf': self.kernel_func = self._rbf
-        elif self.kernel == 'sigmoid': self.kernel_func = self._sigmoid
-        elif self.kernel == 'laplacian': self.kernel_func = self._laplacian
-        else: raise UnsupportedParameterError(self.kernel)
-    
+        if self.kernel == "linear":
+            self.kernel_func = self._linear
+        elif self.kernel == "poly":
+            self.kernel_func = self._poly
+        elif self.kernel == "rbf":
+            self.kernel_func = self._rbf
+        elif self.kernel == "sigmoid":
+            self.kernel_func = self._sigmoid
+        elif self.kernel == "laplacian":
+            self.kernel_func = self._laplacian
+        else:
+            raise UnsupportedParameterError(self.kernel)
+
     def _linear(self, x: Vector, y: Vector) -> float:
         return np.dot(x, y)
-    
+
     def _poly(self, x: Vector, y: Vector) -> float:
         return (np.dot(x, y) + self.coef) ** self.deg
-    
+
     def _rbf(self, x: Vector, y: Vector) -> float:
         return np.exp(-self.gamma * np.linalg.norm(x - y) ** 2)
-    
+
     def _sigmoid(self, x: Vector, y: Vector) -> float:
         return np.tanh(self.gamma * np.dot(x, y) + self.coef)
-    
+
     def _laplacian(self, x: Vector, y: Vector) -> float:
         return np.exp(-self.gamma * np.linalg.norm(x - y))
 
 
 class LDA(Transformer, Supervised):
-    
     """
-    Linear Discriminant Analysis (LDA) is a dimensionality reduction 
-    and classification technique. It's primarily employed for dimensionality 
-    reduction and feature extraction while also considering class 
+    Linear Discriminant Analysis (LDA) is a dimensionality reduction
+    and classification technique. It's primarily employed for dimensionality
+    reduction and feature extraction while also considering class
     information for classification tasks.
-    
+
     Parameters
     ----------
     `n_components` : Number of linear discriminants
-    
+
     Notes
     -----
-    * To use LDA for classification, refer to 
+    * To use LDA for classification, refer to
         `luma.classifier.discriminant.LDAClassifier`
-    
+
     """
-    
+
     def __init__(self, n_components: int = None) -> None:
         self.n_components = n_components
         self._fitted = False
 
-    def fit(self, X: Matrix, y: Matrix) -> 'LDA':
+        self.set_param_ranges({"n_components": ("0<,+inf", int)})
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix, y: Matrix) -> "LDA":
         self.classes = np.unique(y)
         self.class_means = [np.mean(X[y == c], axis=0) for c in self.classes]
 
         within_class_scatter = np.zeros((X.shape[1], X.shape[1]))
         for c in self.classes:
             X_c = X[y == c]
             mean_diff = X_c - self.class_means[c]
             within_class_scatter += np.dot(mean_diff.T, mean_diff)
-            
+
         between_class_scatter = np.zeros((X.shape[1], X.shape[1]))
         for c in self.classes:
             n = X[y == c].shape[0]
             mean_diff = self.class_means[c] - np.mean(X)
             between_class_scatter += n * np.outer(mean_diff, mean_diff)
-            
-        eigenvalues, eigenvectors = np.linalg.eigh(np.linalg.inv(within_class_scatter)
-                                                   .dot(between_class_scatter))
+
+        eigenvalues, eigenvectors = np.linalg.eigh(
+            np.linalg.inv(within_class_scatter).dot(between_class_scatter)
+        )
 
         sorted_indices = np.argsort(eigenvalues)[::-1]
         eigenvalues = eigenvalues[sorted_indices]
         eigenvectors = eigenvectors[:, sorted_indices]
 
         if self.n_components is not None:
-            self.eigenvalues = eigenvalues[:self.n_components]
-            self.eigenvectors = eigenvectors[:, :self.n_components]
+            self.eigenvalues = eigenvalues[: self.n_components]
+            self.eigenvectors = eigenvectors[:, : self.n_components]
         else:
             self.eigenvalues = eigenvalues
             self.eigenvectors = eigenvectors
-        
+
         self._fitted = True
         return self
 
     def transform(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         return np.dot(X, self.eigenvectors)
 
     def fit_transform(self, X: Matrix, y: Matrix) -> Matrix:
         self.fit(X, y)
         return self.transform(X)
 
 
 class TruncatedSVD(Transformer, Unsupervised):
-    
     """
-    runcated Singular Value Decomposition (TruncatedSVD) is a linear dimensionality 
-    reduction method that simplifies large datasets by preserving the most relevant 
-    information. It achieves this by decomposing a matrix into three components 
-    using singular value decomposition (SVD) and retaining only a specified number 
+    runcated Singular Value Decomposition (TruncatedSVD) is a linear dimensionality
+    reduction method that simplifies large datasets by preserving the most relevant
+    information. It achieves this by decomposing a matrix into three components
+    using singular value decomposition (SVD) and retaining only a specified number
     of important components.
-    
+
     Parameters
     ----------
     `n_components` : Dimensionality of low-space
-    
+
     """
-    
+
     def __init__(self, n_components: int = None) -> None:
         self.n_components = n_components
         self._fitted = False
-    
-    def fit(self, X: Matrix) -> 'TruncatedSVD':
+
+        self.set_param_ranges({"n_components": ("0<,+inf", int)})
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix) -> "TruncatedSVD":
         mean = np.mean(X, axis=0)
         X_centered = X - mean
         U, S, VT = np.linalg.svd(X_centered, full_matrices=False)
-        
-        self.U = U[:, :self.n_components]
-        self.S = np.diag(S[:self.n_components])
-        self.VT = VT[:self.n_components, :]
+
+        self.U = U[:, : self.n_components]
+        self.S = np.diag(S[: self.n_components])
+        self.VT = VT[: self.n_components, :]
         self._fitted = True
         return self
-    
+
     def transform(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         mean = np.mean(X, axis=0)
         X_centered = X - mean
         return np.dot(X_centered, self.VT.T)
-    
+
     def fit_transform(self, X: Matrix) -> Matrix:
         self.fit(X)
         return self.transform(X)
 
 
 class FactorAnalysis(Transformer, Unsupervised):
-    
     """
-    Factor Analysis is a statistical method used to uncover latent factors 
-    influencing observed variables. It assumes that observed variables share 
-    common variance due to these unobservable factors, expressed through 
-    factor loadings. The technique helps simplify data interpretation by 
+    Factor Analysis is a statistical method used to uncover latent factors
+    influencing observed variables. It assumes that observed variables share
+    common variance due to these unobservable factors, expressed through
+    factor loadings. The technique helps simplify data interpretation by
     revealing the underlying structure of the dataset.
-    
+
     Parameters
     ----------
     `n_components` : Dimensionality of low-space
     `max_iter` : Number of iterations
     `tol` : Threshold for convergence
     `noise_variance` : Initial variances for noise of each features
-    
+
     """
-    
-    def __init__(self,
-                 n_components: int = None,
-                 max_iter: int = 1000,
-                 tol: float = 1e-5,
-                 noise_variance: Matrix | list = None,
-                 verbose: bool = False) -> None:
+
+    def __init__(
+        self,
+        n_components: int = None,
+        max_iter: int = 1000,
+        tol: float = 1e-5,
+        noise_variance: Matrix | list = None,
+        verbose: bool = False,
+    ) -> None:
         self.n_components = n_components
         self.max_iter = max_iter
         self.tol = tol
         self.noise_variance = noise_variance
         self.verbose = verbose
         self._fitted = False
 
-    def fit(self, X: Matrix) -> 'FactorAnalysis':
+        self.set_param_ranges(
+            {"n_components": ("0<,+inf", int), "max_iter": ("0<,+inf", int)}
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix) -> "FactorAnalysis":
         m, n = X.shape
         self.mean = X.mean(axis=0)
         X -= self.mean
-        
+
         logL_const = n * np.log(2 * np.pi) * self.n_components
         variance = X.var(axis=0)
         psi = np.ones(n)
         if self.noise_variance:
             psi = Matrix(self.noise_variance)
-        
+
         logLikelihood = []
         prev_logL = -np.inf
         for i in range(self.max_iter):
             sqrt_psi = np.sqrt(psi) + 1e-12
-            _, _S, _VT = svd(X / (sqrt_psi * m ** 0.5), full_matrices=False)
-            S, VT = _S[:self.n_components], _VT[:self.n_components]
+            _, _S, _VT = svd(X / (sqrt_psi * m**0.5), full_matrices=False)
+            S, VT = _S[: self.n_components], _VT[: self.n_components]
             unexp_var = np.linalg.norm(S) ** 2
-            
+
             S **= 2
             W = np.sqrt(np.maximum(S - 1.0, 0.0))[:, np.newaxis] * VT
             W *= sqrt_psi
-            
+
             logL = np.sum(np.log(S)) + np.sum(np.log(psi))
             logL += logL_const + unexp_var
             logL *= -0.5 * m
             logLikelihood.append(logL)
-            
+
             abs_diff = abs(logL - prev_logL)
-            if abs_diff < self.tol: 
+            if abs_diff < self.tol:
                 if self.verbose:
-                    print(f'[FA] Ealry Convergence at iteration {i}/{self.max_iter}', end=' ')
-                    print(f'with delta-logL of {abs_diff}')
+                    print(
+                        f"[FA] Ealry Convergence at iteration {i}/{self.max_iter}",
+                        end=" ",
+                    )
+                    print(f"with delta-logL of {abs_diff}")
                 break
-            prev_logL = logL            
-            psi = np.maximum(variance - np.sum(W ** 2, axis=0), 1e-12)
-            
+            prev_logL = logL
+            psi = np.maximum(variance - np.sum(W**2, axis=0), 1e-12)
+
             if self.verbose and i % 100 == 0 and i:
-                print(f'[FA] Iteration {i}/{self.max_iter} finished', end=' ')
-                print(f'with delta-logL of {abs_diff}')
-                
-        else: NotConvergedError(self)
-        
+                print(f"[FA] Iteration {i}/{self.max_iter} finished", end=" ")
+                print(f"with delta-logL of {abs_diff}")
+
+        else:
+            NotConvergedError(self)
+
         self.W = W
         self._fitted = True
         return self
-    
+
     def transform(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         Ih = np.eye(len(self.W))
         W_psi = self.W / self.noise_variance if self.noise_variance else self.W
         cov = np.linalg.inv(Ih + W_psi.dot(self.W.T))
         return np.dot((X - self.mean).dot(W_psi.T), cov)
-    
+
     def fit_transform(self, X: Matrix) -> Matrix:
         self.fit(X)
         return self.transform(X)
 
 
 class KDA(Transformer, Supervised):
-    
     """
-    Kernel Discriminant Analysis (KDA) is a machine learning technique for 
-    dimensionality reduction and classification that extends Linear 
-    Discriminant Analysis (LDA) to nonlinear feature spaces using kernel 
-    methods. It projects data into a lower-dimensional space where classes 
-    are more separable by maximizing the ratio of between-class variance 
-    to within-class variance. KDA utilizes kernel functions to implicitly 
-    map input data to a high-dimensional space without explicitly computing 
+    Kernel Discriminant Analysis (KDA) is a machine learning technique for
+    dimensionality reduction and classification that extends Linear
+    Discriminant Analysis (LDA) to nonlinear feature spaces using kernel
+    methods. It projects data into a lower-dimensional space where classes
+    are more separable by maximizing the ratio of between-class variance
+    to within-class variance. KDA utilizes kernel functions to implicitly
+    map input data to a high-dimensional space without explicitly computing
     the coordinates in that space.
-    
+
     Parameters
     ----------
     `n_components` : Dimensionality of low-space
     `deg` : Polynomial degree of `poly` kernel
     `gamma` : Shape parameter of `rbf`, `sigmoid`, `laplacian`
     `coef` : Additional coefficient of `poly`, `sigmoid`
     `kernel` : Type of kernel functions
-    
+
     Notes
     -----
-    * To use KDA for classification, refer to 
+    * To use KDA for classification, refer to
         `luma.classifier.discriminant.KDAClassifier`
-    
+
     """
-    
-    def __init__(self, 
-                 n_components: int = None, 
-                 deg: int = 2,
-                 alpha: float = 1.0,
-                 gamma: float = 1.0,
-                 coef: int = 0.0,
-                 kernel: KernelUtil.func_type = 'rbf') -> None:
+
+    def __init__(
+        self,
+        n_components: int = None,
+        deg: int = 2,
+        gamma: float = 1.0,
+        coef: int = 0.0,
+        kernel: KernelUtil.FuncType = "rbf",
+    ) -> None:
         self.n_components = n_components
         self.deg = deg
-        self.alpha = alpha
         self.gamma = gamma
         self.coef = coef
         self.kernel = kernel
         self.X_ = None
         self._fitted = False
-        
+
         self.kernel_params = {
-            'deg': self.deg,
-            'alpha': self.alpha,
-            'gamma': self.gamma,
-            'coef': self.coef
+            "deg": self.deg,
+            "gamma": self.gamma,
+            "coef": self.coef,
         }
-    
-    def fit(self, X: Matrix, y: Vector) -> 'KDA':
+
+        self.set_param_ranges(
+            {
+                "n_components": ("0<,+inf", int),
+                "deg": ("0,+inf", int),
+                "gamma": ("0<,+inf", None),
+            }
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix, y: Vector) -> "KDA":
         m, _ = X.shape
         self.X_ = X
         self.classes = np.unique(y)
         self.ku_ = KernelUtil(self.kernel, **self.kernel_params)
-        
+
         K = self.ku_.kernel_func(X)
         M = np.mean(K, axis=0)
         Sw = np.zeros((m, m))
         Sb = np.zeros((m, m))
-        
+
         for i in self.classes:
             Xi = K[y == i]
             Mi = np.mean(Xi, axis=0)
             Ni = Xi.shape[0]
-            
+
             Sw += np.dot((Xi - Mi).T, Xi - Mi)
             Sb += Ni * np.outer(Mi - M, Mi - M)
-        
+
         eigvals, eigvecs = np.linalg.eigh(np.linalg.pinv(Sw).dot(Sb))
         indices = np.argsort(eigvals)[::-1]
-        self.eigvecs = eigvecs[:, indices[:self.n_components]]
-        
+        self.eigvecs = eigvecs[:, indices[: self.n_components]]
+
         self._fitted = True
         return self
-    
+
     def transform(self, X: Matrix) -> Vector:
         K = self.ku_.kernel_func(X, self.X_)
         return K.dot(self.eigvecs)
-    
+
     def fit_transform(self, X: Matrix, y: Vector) -> Vector:
         self.fit(X, y)
         return self.transform(X)
 
 
 class CCA(Transformer, Unsupervised):
-    
     """
-    Canonical Correlation Analysis (CCA) is a multivariate statistical method 
-    that finds linear combinations of two sets of variables with the highest 
-    correlation. It aims to uncover the underlying correlation structure 
-    between the two variable sets. CCA is an unsupervised technique, often 
-    used for exploring the relationships in complex data. The result is pairs 
-    of canonical variables (or components) that represent the maximal 
+    Canonical Correlation Analysis (CCA) is a multivariate statistical method
+    that finds linear combinations of two sets of variables with the highest
+    correlation. It aims to uncover the underlying correlation structure
+    between the two variable sets. CCA is an unsupervised technique, often
+    used for exploring the relationships in complex data. The result is pairs
+    of canonical variables (or components) that represent the maximal
     correlations between the sets.
-    
+
     Parameters
     ----------
     `n_components` : Dimensionality of low-space
-    
+
     Notes
     -----
-    * `CCA` requires two distinct datasets `X` and `Y`, 
+    * `CCA` requires two distinct datasets `X` and `Y`,
         in which `Y` is not a target variable
-    * Due to its uniqueness in its parameters, 
+    * Due to its uniqueness in its parameters,
         `CCA` may not be compatible with several meta estimators
     * `transform()` and `fit_transform()` returns a 2-tuple of `Matrix`
-        
+
         ```py
         def transform(self, X: Matrix, Y: Matrix) -> Tuple[Matrix, Matrix]
         ```
     """
-    
+
     def __init__(self, n_components: int = None) -> None:
         self.n_components = n_components
         self.correlations_ = None
         self._fitted = False
-    
-    def fit(self, X: Matrix, Y: Matrix) -> 'CCA':
+
+        self.set_param_ranges({"n_components": ("0<,+inf", int)})
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix, Y: Matrix) -> "CCA":
         _, n = X.shape
         X -= X.mean(axis=0)
         Y -= Y.mean(axis=0)
-        
+
         Cxx = np.cov(X.T)
         Cyy = np.cov(Y.T)
         Cxy = np.cov(X.T, Y.T)[:n, n:]
-        
+
         inv_Cxx = np.linalg.pinv(Cxx)
         inv_Cyy = np.linalg.pinv(Cyy)
         eigvals, x_weights = np.linalg.eig(inv_Cxx @ Cxy @ inv_Cyy @ Cxy.T)
-        
+
         indices = eigvals.argsort()[::-1]
-        self.x_weights = x_weights[:, indices][:, :self.n_components]
-        self.y_weights = inv_Cyy @ Cxy.T @ self.x_weights 
-        self.y_weights /= eigvals[indices][:self.n_components]
-        
+        self.x_weights = x_weights[:, indices][:, : self.n_components]
+        self.y_weights = inv_Cyy @ Cxy.T @ self.x_weights
+        self.y_weights /= eigvals[indices][: self.n_components]
+
         self.x_scores = X.dot(self.x_weights)
         self.y_scores = Y.dot(self.y_weights)
-        
-        self.correlations_ = [np.corrcoef(self.x_scores[:, i], 
-                                          self.y_scores[:, i])[0, 1]
-                              for i in range(self.n_components)]
-        
+
+        self.correlations_ = [
+            np.corrcoef(self.x_scores[:, i], self.y_scores[:, i])[0, 1]
+            for i in range(self.n_components)
+        ]
+
         self.x_loadings = Cxy.dot(self.y_weights)
         self.y_loadings = Cxy.T.dot(self.x_weights)
-        
+
         self._fitted = True
         return self
-    
+
     def transform(self, X: Matrix, Y: Matrix) -> Tuple[Matrix, Matrix]:
         X -= X.mean(axis=0)
         Y -= Y.mean(axis=0)
         X_trans = X.dot(self.x_weights)
         Y_trans = Y.dot(self.y_weights)
-        
+
         return X_trans, Y_trans
-    
+
     def fit_transform(self, X: Matrix, Y: Matrix) -> Tuple[Matrix, Matrix]:
         self.fit(X, Y)
         return self.transform(X, Y)
-
```

### Comparing `luma-ml-0.6.4/luma/reduction/manifold.py` & `luma-ml-0.6.5/luma/reduction/manifold.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,478 +11,556 @@
 from luma.core.super import Transformer, Unsupervised
 from luma.interface.exception import NotFittedError, UnsupportedParameterError
 from luma.clustering.kmeans import *
 from luma.metric.distance import *
 
 
 __all__ = (
-    'TSNE', 
-    'MDS', 
-    'MetricMDS', 
-    'LandmarkMDS', 
-    'LLE',
-    'ModifiedLLE', 
-    'HessianLLE', 
-    'SammonMapping', 
-    'LaplacianEigenmap',
-    'Isomap', 
-    'ConformalIsomap', 
-    'LTSA'
+    "TSNE",
+    "MDS",
+    "MetricMDS",
+    "LandmarkMDS",
+    "LLE",
+    "ModifiedLLE",
+    "HessianLLE",
+    "SammonMapping",
+    "LaplacianEigenmap",
+    "Isomap",
+    "ConformalIsomap",
+    "LTSA",
 )
 
 
 class TSNE(Transformer, Unsupervised):
-    
     """
-    t-SNE, which stands for t-distributed Stochastic Neighbor Embedding, 
-    is a machine learning technique commonly used for data visualization 
+    t-SNE, which stands for t-distributed Stochastic Neighbor Embedding,
+    is a machine learning technique commonly used for data visualization
     and dimensionality reduction.
-    
+
     Parameters
     ----------
     `n_components` : Dimensionality of lower spcae
     `max_iter` : Number of iteration
     `learning_rate` : Updating factor of embedding optimization
     `perplexity` : Perplexity parameter of Gaussian kernel
     `verbose` : Provided details of each iteration when set `True`
-    
+
     """
-    
-    def __init__(self, 
-                 n_components: int = None, 
-                 max_iter: int = 1000, 
-                 learning_rate: int = 300, 
-                 perplexity: int = 30,
-                 verbose: bool = False) -> None:
+
+    def __init__(
+        self,
+        n_components: int = None,
+        max_iter: int = 1000,
+        learning_rate: int = 300,
+        perplexity: int = 30,
+        verbose: bool = False,
+    ) -> None:
         self.n_components = n_components
         self.max_iter = max_iter
         self.learning_rate = learning_rate
         self.perplexity = perplexity
         self.verbose = verbose
         self._fitted = False
-        
-    def fit(self, X: Matrix) -> 'TSNE':
+
+        self.set_param_ranges(
+            {
+                "n_components": ("0<,+inf", int),
+                "max_iter": ("0<,+inf", int),
+                "learning_rate": ("0<,+inf", int),
+                "perplexity": ("0<,+inf", int),
+            }
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix) -> "TSNE":
         size = X.shape[0]
         P = self._P_joint_probabilities(X)
         y = np.random.normal(0.0, 1e-4, (size, self.n_components))
         Y = [y, y]
 
         for i in range(1, self.max_iter + 1):
             Q = self._Q_joint_probabilities(Y[-1])
             gradient = self._compute_gradient(P, Q, Y[-1])
             y = Y[-1] - self.learning_rate * gradient
             y += self._momentum(i) * (Y[-1] - Y[-2])
             Y.append(y)
-            
-            if i % 10 == 0: Q = np.maximum(Q, 1e-12)
-            if self.verbose and i % 50 == 0: 
-                print(f'[t-SNE] main iteration: {i}/{self.max_iter}', end='')
-                print(f' - gradient-norm: {np.linalg.norm(gradient)}')
-            
+
+            if i % 10 == 0:
+                Q = np.maximum(Q, 1e-12)
+            if self.verbose and i % 50 == 0:
+                print(f"[t-SNE] main iteration: {i}/{self.max_iter}", end="")
+                print(f" - gradient-norm: {np.linalg.norm(gradient)}")
+
         self.y = y
         self._fitted = True
         return self
-    
+
     def transform(self) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         return self.y
-    
+
     def fit_transform(self, X: Matrix) -> Matrix:
         self.fit(X)
         return self.transform()
-    
+
     def _P_conditional(self, distances: Matrix, sigmas: Matrix) -> Matrix:
-        exponent = np.exp(-distances / (2 * np.square(sigmas.reshape((-1,1)))))
+        exponent = np.exp(-distances / (2 * np.square(sigmas.reshape((-1, 1)))))
         np.fill_diagonal(exponent, 0.0)
         exponent += 1e-8
-        
-        return exponent / exponent.sum(axis=1).reshape([-1,1])
-    
+
+        return exponent / exponent.sum(axis=1).reshape([-1, 1])
+
     def _P_joint_probabilities(self, X: Matrix) -> Matrix:
         size = X.shape[0]
         distances = self._compute_pairwise_dist(X)
         sigmas = self._find_sigma_vector(distances)
         conditional_prob = self._P_conditional(distances, sigmas)
-        
+
         return (conditional_prob + conditional_prob.T) / (2.0 * size)
-    
+
     def _Q_joint_probabilities(self, y: Matrix) -> Matrix:
         distances = self._compute_pairwise_dist(y)
         nominator = 1 / (1 + distances)
         np.fill_diagonal(nominator, 0.0)
-        
+
         return nominator / np.sum(np.sum(nominator))
-    
+
     def _find_sigma_vector(self, distances: Matrix) -> Matrix:
         N = distances.shape[0]
         opt_sigmas = np.zeros(N)
-        
+
         for i in range(N):
             func = lambda sig: self._compute_perplexity(
-                self._P_conditional(distances[i:i + 1, :], Matrix([sig])))
-            
+                self._P_conditional(distances[i : i + 1, :], Matrix([sig]))
+            )
+
             opt_sigmas[i] = self._binary_search(func)
-            if self.verbose and i % 50 == 0: 
-                print(f'[t-SNE] sigma iteration: {i}/{N}', end='')
-                print(f' - sigma-norm: {np.linalg.norm(opt_sigmas[i])}')
-            
-        if self.verbose: print('-' * 70)
+            if self.verbose and i % 50 == 0:
+                print(f"[t-SNE] sigma iteration: {i}/{N}", end="")
+                print(f" - sigma-norm: {np.linalg.norm(opt_sigmas[i])}")
+
+        if self.verbose:
+            print("-" * 70)
         return opt_sigmas
-    
-    def _binary_search(self, func: Callable, 
-                       tol: float = 1e-10, max_iter: int = 1000, 
-                       low: float = 1e-10, high: float = 1e3) -> Matrix:
+
+    def _binary_search(
+        self,
+        func: Callable,
+        tol: float = 1e-10,
+        max_iter: int = 1000,
+        low: float = 1e-10,
+        high: float = 1e3,
+    ) -> Matrix:
         for _ in range(max_iter):
             guess = (high + low) / 2.0
             val = func(guess)
-            if val > self.perplexity: high = guess
-            else: low = guess
-            if np.abs(val - self.perplexity) <= tol: 
+            if val > self.perplexity:
+                high = guess
+            else:
+                low = guess
+            if np.abs(val - self.perplexity) <= tol:
                 return guess
         return guess
-    
+
     def _compute_pairwise_dist(self, X: Matrix) -> Matrix:
         return np.sum((X[None, :] - X[:, None]) ** 2, axis=2)
-    
+
     def _compute_gradient(self, P: Matrix, Q: Matrix, y: Matrix) -> Matrix:
         pq_diff = P - Q
         y_diff = np.expand_dims(y, axis=1) - np.expand_dims(y, axis=0)
         distances = self._compute_pairwise_dist(y)
         aux = 1 / (1 + distances)
-        
-        return 4 * (np.expand_dims(pq_diff, 2) * y_diff * np.expand_dims(aux, 2)).sum(axis=1)
-    
+
+        return 4 * (np.expand_dims(pq_diff, 2) * y_diff * np.expand_dims(aux, 2)).sum(
+            axis=1
+        )
+
     def _compute_perplexity(self, cond_matrix: Matrix) -> Matrix:
         entropy = -np.sum(cond_matrix * np.log2(cond_matrix), axis=1)
-        return 2 ** entropy
-    
+        return 2**entropy
+
     def _momentum(self, iteration: int):
         return 0.5 if iteration < 250 else 0.8
 
 
 class MDS(Transformer, Unsupervised):
-    
     """
-    Multidimensional Scaling (MDS) is a data analysis technique that visualizes 
-    high-dimensional data in a lower-dimensional space while preserving the 
-    relationships between data points. It uses a distance matrix to find a 
-    lower-dimensional representation, making it easier to understand and 
+    Multidimensional Scaling (MDS) is a data analysis technique that visualizes
+    high-dimensional data in a lower-dimensional space while preserving the
+    relationships between data points. It uses a distance matrix to find a
+    lower-dimensional representation, making it easier to understand and
     explore data patterns.
-    
+
     Parameters
     ----------
     `n_components` : Dimensionality of low-space
-    
+
     """
-    
+
     def __init__(self, n_components: int = None) -> None:
         self.n_components = n_components
         self._fitted = False
-    
-    def fit(self, X: Matrix) -> 'MDS':
+
+        self.set_param_ranges({"n_components": ("0<,+inf", int)})
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix) -> "MDS":
         D = self._compute_dissimilarity(X)
         n = D.shape[0]
         H = np.eye(n) - np.ones((n, n)) / n
         B = -0.5 * H.dot(D).dot(H)
-        
+
         eigvals, eigvecs = np.linalg.eigh(B)
         sorted_indices = np.argsort(eigvals)[::-1]
         self.eigvals = eigvals[sorted_indices]
         self.eigvecs = eigvecs[:, sorted_indices]
-        
-        self.eigvals = self.eigvals[:self.n_components]
-        self.eigvecs = self.eigvecs[:, :self.n_components]
+
+        self.eigvals = self.eigvals[: self.n_components]
+        self.eigvecs = self.eigvecs[:, : self.n_components]
         self._fitted = True
         self.stress = self._compute_stress(D)
         return self
-    
+
     def transform(self) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         sqrt_eigvals = np.diag(np.sqrt(np.maximum(self.eigvals, 0)))
         return self.eigvecs.dot(sqrt_eigvals)
-    
+
     def fit_transform(self, X) -> Any:
         self.fit(X)
         return self.transform()
-    
+
     def _compute_dissimilarity(self, X: Matrix) -> Matrix:
-        return squareform(pdist(X, metric='euclidean'))
+        return squareform(pdist(X, metric="euclidean"))
 
     def _compute_stress(self, D: Matrix) -> float:
         Z = self.transform()
         stress = np.sum((D - self._compute_dissimilarity(Z)) ** 2)
-        stress /= np.sum(D ** 2)
+        stress /= np.sum(D**2)
         stress = np.sqrt(stress)
         return stress
 
 
 class MetricMDS(Transformer, Unsupervised):
-    
     """
-    Metric Multidimensional Scaling (MDS) is a data analysis method that focuses 
+    Metric Multidimensional Scaling (MDS) is a data analysis method that focuses
     on accurately preserving the original pairwise distances or dissimilarities
-    between objects in a high-dimensional space when projecting them onto a 
-    lower-dimensional space. 
-    
+    between objects in a high-dimensional space when projecting them onto a
+    lower-dimensional space.
+
     Parameter
     ---------
     `n_components` : Dimensionality of low-space
-    `metric` : Distance metric 
+    `metric` : Distance metric
     (e.g. `euclidean`, `manhattan`, `chebyshev`, `minkowski`,
     `cos_similarity`, `correation`, `mahalanobis`)
     `p` : Power factor for `minkowski`
-    
+
     """
-    
-    def __init__(self,
-                 n_components: int = None,
-                 p: float | int = None,
-                 metric: Literal['euclidean', 'manhattan', 'chebyshev',
-                                 'minkowski', 'cos_similarity', 'correlation',
-                                 'mahalanobis'] = 'euclidean') -> None:
+
+    def __init__(
+        self,
+        n_components: int = None,
+        p: float | int = None,
+        metric: Literal[
+            "euclidean",
+            "manhattan",
+            "chebyshev",
+            "minkowski",
+            "cos_similarity",
+            "correlation",
+            "mahalanobis",
+        ] = "euclidean",
+    ) -> None:
         self.n_components = n_components
         self.metric = metric
         self.p = p
         self._fitted = False
 
-    def fit(self, X: Matrix) -> 'MetricMDS':
+        self.set_param_ranges(
+            {"n_components": ("0<,+inf", int), "p": ("0<,+inf", None)}
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix) -> "MetricMDS":
         D = self._compute_dissimilarity(X)
         n = D.shape[0]
         H = np.eye(n) - np.ones((n, n)) / n
         B = -0.5 * H.dot(D).dot(H)
-        
+
         eigvals, eigvecs = np.linalg.eigh(B)
         sorted_indices = np.argsort(eigvals)[::-1]
         self.eigvals = eigvals[sorted_indices]
         self.eigvecs = eigvecs[:, sorted_indices]
-        
-        self.eigvals = self.eigvals[:self.n_components]
-        self.eigvecs = self.eigvecs[:, :self.n_components]
+
+        self.eigvals = self.eigvals[: self.n_components]
+        self.eigvecs = self.eigvecs[:, : self.n_components]
         self._fitted = True
         self.stress = self._compute_stress(D)
         return self
-    
+
     def transform(self) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         sqrt_eigvals = np.diag(np.sqrt(np.maximum(self.eigvals, 0)))
         return self.eigvecs.dot(sqrt_eigvals)
-    
+
     def fit_transform(self, X) -> Any:
         self.fit(X)
         return self.transform()
-    
+
     def _compute_dissimilarity(self, X: Matrix) -> Matrix:
         m, _ = X.shape
         cov = np.cov(X, rowvar=False)
         D = np.ones((m, m))
         for i in range(m):
             for j in range(i + 1, m):
                 join = (X[i], X[j])
-                if self.metric == 'euclidean': d = Euclidean.compute(*join)
-                elif self.metric == 'manhattan': d = Manhattan.compute(*join)
-                elif self.metric == 'chebyshev': d = Chebyshev.compute(*join)
-                elif self.metric == 'minkowski': d = Minkowski.compute(*join, self.p)
-                elif self.metric == 'cos_similarity': d = CosineSimilarity.compute(*join)
-                elif self.metric == 'correlation': d = Correlation.compute(*join)
-                elif self.metric == 'mahalanobis': d = Mahalanobis.compute(*join, cov)
-                else: raise ValueError(f'[mMDS] Invalid distance metric: {self.metric}')
+                if self.metric == "euclidean":
+                    d = Euclidean.compute(*join)
+                elif self.metric == "manhattan":
+                    d = Manhattan.compute(*join)
+                elif self.metric == "chebyshev":
+                    d = Chebyshev.compute(*join)
+                elif self.metric == "minkowski":
+                    d = Minkowski.compute(*join, self.p)
+                elif self.metric == "cos_similarity":
+                    d = CosineSimilarity.compute(*join)
+                elif self.metric == "correlation":
+                    d = Correlation.compute(*join)
+                elif self.metric == "mahalanobis":
+                    d = Mahalanobis.compute(*join, cov)
+                else:
+                    raise ValueError(f"[mMDS] Invalid distance metric: {self.metric}")
                 D[i, j] = D[j, i] = d
-        
+
         return D
 
     def _compute_stress(self, D: Matrix) -> float:
         Z = self.transform()
         stress = np.sum((D - self._compute_dissimilarity(Z)) ** 2)
-        stress /= np.sum(D ** 2)
+        stress /= np.sum(D**2)
         stress = np.sqrt(stress)
         return stress
 
 
 class LandmarkMDS(Transformer, Unsupervised):
-    
     """
-    Landmark Multi-Dimensional Scaling (LMDS) is a dimensionality reduction method 
-    that selects a subset of "landmark" points to efficiently approximate the 
-    lower-dimensional representation of a dataset while preserving pairwise distances. 
-    It simplifies the computation by focusing on distances between data points and 
+    Landmark Multi-Dimensional Scaling (LMDS) is a dimensionality reduction method
+    that selects a subset of "landmark" points to efficiently approximate the
+    lower-dimensional representation of a dataset while preserving pairwise distances.
+    It simplifies the computation by focusing on distances between data points and
     landmarks, making it suitable for large datasets.
-    
+
     Parameters
     ----------
     `n_components` : Dimensionality of low-space
     `n_landmarks` : Number of landmarks
     `method` : Algorithm for landmark initialization
     (e.g. `random`, `kmeans`, `kmeans++`, `kmedians`)
-    
+
     """
-    
-    def __init__(self, 
-                 n_components: int = None, 
-                 n_landmarks: int = 10,
-                 method: Literal['random', 'kmeans', 'kmeans++', 'kmedians'] = 'random',
-                 verbose: bool = False) -> None:
+
+    def __init__(
+        self,
+        n_components: int = None,
+        n_landmarks: int = 10,
+        method: Literal["random", "kmeans", "kmeans++", "kmedians"] = "random",
+        verbose: bool = False,
+    ) -> None:
         self.n_components = n_components
         self.n_landmarks = n_landmarks
         self.method = method
         self.verbose = verbose
         self._fitted = False
-    
-    def fit(self, X: Matrix) -> 'LandmarkMDS':
+
+        self.set_param_ranges(
+            {"n_components": ("0<,+inf", int), "n_landmarks": ("0<,+inf", int)}
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix) -> "LandmarkMDS":
         self.landmarks = self._initialize_landmarks(X)
         D = self._compute_dissimilarity(self.landmarks)
         n = D.shape[0]
         H = np.eye(n) - np.ones((n, n)) / n
         B = -0.5 * H.dot(D).dot(H)
-        
+
         eigvals, eigvecs = np.linalg.eigh(B)
         sorted_indices = np.argsort(eigvals)[::-1]
         self.eigvals = eigvals[sorted_indices]
         self.eigvecs = eigvecs[:, sorted_indices]
-        
+
         self.eigvals = self.eigvals[self.n_components]
-        self.eigvecs = self.eigvecs[:, :self.n_components]
-        
+        self.eigvecs = self.eigvecs[:, : self.n_components]
+
         D_mean = np.mean(D, axis=0)
         D_xland = np.sum((X[:, np.newaxis, :] - self.landmarks) ** 2, axis=2)
         self.mean_diff = D_mean - D_xland
         self._fitted = True
         return self
-    
+
     def _initialize_landmarks(self, X: Matrix) -> Matrix:
         m, _ = X.shape
-        if self.method == 'random':
-            if self.verbose: print(f'[LMDS] Initializing landmarks with random choice')
+        if self.method == "random":
+            if self.verbose:
+                print(f"[LMDS] Initializing landmarks with random choice")
             landmark = X[np.random.choice(m, self.n_landmarks, replace=False)]
-            
-        elif self.method == 'kmeans':
-            if self.verbose: print(f'[LMDS] Initializing landmarks with K-Means centroids')
+
+        elif self.method == "kmeans":
+            if self.verbose:
+                print(f"[LMDS] Initializing landmarks with K-Means centroids")
             kmeans = KMeansClustering(n_clusters=self.n_landmarks, verbose=self.verbose)
             kmeans.fit(X)
             landmark = kmeans.centroids
-        
-        elif self.method == 'kmeans++':
-            if self.verbose: print(f'[LMDS] Initializing landmarks with K-Means++ centroids')
-            kmeanspp = KMeansClusteringPlus(n_clusters=self.n_landmarks, verbose=self.verbose)
+
+        elif self.method == "kmeans++":
+            if self.verbose:
+                print(f"[LMDS] Initializing landmarks with K-Means++ centroids")
+            kmeanspp = KMeansClusteringPlus(
+                n_clusters=self.n_landmarks, verbose=self.verbose
+            )
             kmeanspp.fit(X)
             landmark = kmeanspp.centroids
-        
-        elif self.method == 'kmedians':
-            if self.verbose: print(f'[LMDS] Initializing landmarks with K-Medians medians')
-            kmedians = KMediansClustering(n_clusters=self.n_landmarks, verbose=self.verbose)
+
+        elif self.method == "kmedians":
+            if self.verbose:
+                print(f"[LMDS] Initializing landmarks with K-Medians medians")
+            kmedians = KMediansClustering(
+                n_clusters=self.n_landmarks, verbose=self.verbose
+            )
             kmedians.fit(X)
             landmark = kmedians.medians
-            
-        else: raise UnsupportedParameterError(self.method)
+
+        else:
+            raise UnsupportedParameterError(self.method)
         return landmark
-    
+
     def _compute_dissimilarity(self, X: Matrix) -> Matrix:
-        return squareform(pdist(X, metric='euclidean'))
-    
+        return squareform(pdist(X, metric="euclidean"))
+
     def transform(self) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         L_sharp = self.eigvecs / np.sqrt(self.eigvals)
         return 0.5 * self.mean_diff.dot(L_sharp)
-    
+
     def fit_transform(self, X: Matrix) -> Matrix:
         self.fit(X)
         return self.transform()
 
 
 class LLE(Transformer, Unsupervised):
-    
     """
-    Locally Linear Embedding (LLE) is a dimensionality reduction technique that aims 
-    to find a lower-dimensional representation of data while preserving the local 
-    relationships between data points. It works by approximating each data point 
-    as a linear combination of its nearest neighbors, revealing the underlying 
-    structure of the data in a lower-dimensional space. 
-    
+    Locally Linear Embedding (LLE) is a dimensionality reduction technique that aims
+    to find a lower-dimensional representation of data while preserving the local
+    relationships between data points. It works by approximating each data point
+    as a linear combination of its nearest neighbors, revealing the underlying
+    structure of the data in a lower-dimensional space.
+
     Parameters
     ----------
     `n_neighbors` : Number of neighbors to be considered 'close'
     `n_components` : Dimensionality of low-space
-    
+
     """
-    
-    def __init__(self, 
-                 n_components: int = None, 
-                 n_neighbors: int = 5, 
-                 verbose: bool = False) -> None:
+
+    def __init__(
+        self, n_components: int = None, n_neighbors: int = 5, verbose: bool = False
+    ) -> None:
         self.n_neighbors = n_neighbors
         self.n_components = n_components
         self.verbose = verbose
         self._fitted = False
-    
-    def fit(self, X: Matrix) -> 'LLE':
+
+        self.set_param_ranges(
+            {"n_components": ("0<,+inf", int), "n_neighbors": ("0<,+inf", int)}
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix) -> "LLE":
         m, _ = X.shape
         distances = np.zeros((m, m))
         for i in range(m):
             for j in range(m):
                 distances[i, j] = np.linalg.norm(X[i] - X[j])
 
         W = np.zeros((m, m))
-        neighbors = np.argsort(distances, axis=1)[:, 1:self.n_neighbors + 1]
+        neighbors = np.argsort(distances, axis=1)[:, 1 : self.n_neighbors + 1]
         for i in range(m):
             Xi = X[neighbors[i]] - X[i]
             Z = np.dot(Xi, Xi.T)
             Z += np.pi * 1e-3 * np.identity(self.n_neighbors)
-            
+
             w = np.linalg.solve(Z, np.ones(self.n_neighbors))
             w /= np.sum(w)
             W[i, neighbors[i]] = w
-            
+
             if self.verbose and i % 100 == 0:
-                print(f'[LLE] Optimized weight for instance {i}/{m}', end='')
-                print(f' - weight-norm: {np.linalg.norm(w)}')
-            
+                print(f"[LLE] Optimized weight for instance {i}/{m}", end="")
+                print(f" - weight-norm: {np.linalg.norm(w)}")
+
         M = np.identity(m) - W
         self.eigvals, self.eigvecs = np.linalg.eig(np.dot(M.T, M))
         self._fitted = True
         return self
-        
+
     def transform(self) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
-        indices = np.argsort(self.eigvals)[1:self.n_components + 1]
+        if not self._fitted:
+            raise NotFittedError(self)
+        indices = np.argsort(self.eigvals)[1 : self.n_components + 1]
         return self.eigvecs[:, indices]
-    
+
     def fit_transform(self, X: Matrix) -> Matrix:
         self.fit(X)
         return self.transform()
 
 
 class ModifiedLLE(Transformer, Unsupervised):
-    
     """
-    Modified Locally Linear Embedding (MLLE) is a dimensionality reduction technique 
-    that extends the LLE method by introducing regularization for improved stability. 
-    MLLE aims to find a lower-dimensional representation of data while preserving the 
-    local relationships between data points. It works by approximating each data 
-    point as a linear combination of its nearest neighbors, revealing the underlying 
-    structure of the data in a lower-dimensional space. 
+    Modified Locally Linear Embedding (MLLE) is a dimensionality reduction technique
+    that extends the LLE method by introducing regularization for improved stability.
+    MLLE aims to find a lower-dimensional representation of data while preserving the
+    local relationships between data points. It works by approximating each data
+    point as a linear combination of its nearest neighbors, revealing the underlying
+    structure of the data in a lower-dimensional space.
 
     Parameters
     ----------
     `n_neighbors` : Number of neighbors to be considered 'close'
     `n_components` : Dimensionality of the lower-dimensional space
     `regularization` : Regularization parameter for stability
-    
+
     """
 
-    def __init__(self, 
-                 n_neighbors: int = 5, 
-                 n_components: int = None, 
-                 regularization: float = 1e-3, 
-                 verbose: bool = False) -> None:
+    def __init__(
+        self,
+        n_neighbors: int = 5,
+        n_components: int = None,
+        regularization: float = 1e-3,
+        verbose: bool = False,
+    ) -> None:
         self.n_neighbors = n_neighbors
         self.n_components = n_components
         self.regularization = regularization
         self.verbose = verbose
         self._fitted = False
 
-    def fit(self, X: Matrix) -> 'ModifiedLLE':
+        self.set_param_ranges(
+            {
+                "n_components": ("0<,+inf", int),
+                "n_neighbors": ("0<,+inf", int),
+                "regularization": ("0,+inf", None),
+            }
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix) -> "ModifiedLLE":
         m, _ = X.shape
         distances = np.zeros((m, m))
         for i in range(m):
             for j in range(m):
                 distances[i, j] = np.linalg.norm(X[i] - X[j])
 
         W = np.zeros((m, m))
@@ -493,521 +571,576 @@
             Z += self.regularization * np.identity(self.n_neighbors)
 
             w = np.linalg.solve(Z, np.ones(self.n_neighbors))
             w /= np.sum(w)
             W[i, neighbors[i]] = w
 
             if self.verbose and i % 100 == 0:
-                print(f'[ModifiedLLE] Optimized weight for instance {i}/{m}', end='')
-                print(f' - weight-norm: {np.linalg.norm(w)}')
+                print(f"[ModifiedLLE] Optimized weight for instance {i}/{m}", end="")
+                print(f" - weight-norm: {np.linalg.norm(w)}")
 
         M = np.identity(m) - W
         self.eigvals, self.eigvecs = np.linalg.eig(np.dot(M.T, M))
         self._fitted = True
         return self
 
     def transform(self) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         indices = np.argsort(self.eigvals)[1 : self.n_components + 1]
         return self.eigvecs[:, indices]
 
     def fit_transform(self, X: Matrix) -> Matrix:
         self.fit(X)
         return self.transform()
 
 
 class HessianLLE(Transformer, Unsupervised):
-    
     """
-    Hessian Locally Linear Embedding (Hessian LLE) is a dimensionality reduction 
-    technique that extends Locally Linear Embedding (LLE). It aims to reduce the 
-    dimensionality of high-dimensional data while preserving local linear relationships 
+    Hessian Locally Linear Embedding (Hessian LLE) is a dimensionality reduction
+    technique that extends Locally Linear Embedding (LLE). It aims to reduce the
+    dimensionality of high-dimensional data while preserving local linear relationships
     and capturing the curvature of these relationships using the Hessian matrix.
-    
+
     Parameters
     ----------
     `n_neighbors` : Number of neighbors to be considered 'close'
     `n_components` : Dimensionality of the lower-dimensional space
     `regularization` : Regularization parameter for stability
-    
+
     """
-    
-    def __init__(self, 
-                 n_neighbors: int = 5, 
-                 n_components: int = None,
-                 regularization: float = 1e-5,
-                 verbose: bool = False) -> None:
+
+    def __init__(
+        self,
+        n_neighbors: int = 5,
+        n_components: int = None,
+        regularization: float = 1e-5,
+        verbose: bool = False,
+    ) -> None:
         self.n_neighbors = n_neighbors
         self.n_components = n_components
         self.regularization = regularization
         self.verbose = verbose
         self._fitted = False
-    
-    def fit(self, X: Matrix) -> 'HessianLLE':
+
+        self.set_param_ranges(
+            {
+                "n_components": ("0<,+inf", int),
+                "n_neighbors": ("0<,+inf", int),
+                "regularization": ("0,+inf", None),
+            }
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix) -> "HessianLLE":
         m, _ = X.shape
         dp = self.n_components * (self.n_components + 1) // 2
-        
+
         if self.n_neighbors <= self.n_components + dp:
             self.n_neighbors = self.n_components * (self.n_components + 3)
             self.n_neighbors /= 2
-            print(f"[HessianLLE] n_neighbors set to {self.n_neighbors}",
-                  "due to Hessian condition mismatch.")
-        
+            print(
+                f"[HessianLLE] n_neighbors set to {self.n_neighbors}",
+                "due to Hessian condition mismatch.",
+            )
+
         index_mat = self._construct_graph(X)
         W = np.zeros((dp * m, m))
         Yi = np.empty((self.n_neighbors, self.n_components + dp + 1))
         Yi[:, 0] = 1
         for i in range(m):
             neighbors = index_mat[i]
             Gi = X[neighbors]
             Gi -= Gi.mean(axis=0)
-            
+
             U, _, _ = np.linalg.svd(Gi, full_matrices=0)
-            Yi[:, 1:self.n_components + 1] = U[:, :self.n_components]
+            Yi[:, 1 : self.n_components + 1] = U[:, : self.n_components]
             j = self.n_components + 1
             for k in range(self.n_components):
-                Yi[:, j:self.n_components + j - k] = \
-                    U[:, k:k + 1] * U[:, k:self.n_components]
+                Yi[:, j : self.n_components + j - k] = (
+                    U[:, k : k + 1] * U[:, k : self.n_components]
+                )
                 j += self.n_components - k
-            
+
             Q, R = np.linalg.qr(Yi)
-            w = Matrix(Q[:, self.n_components + 1:])
+            w = Matrix(Q[:, self.n_components + 1 :])
             S = w.sum(axis=0)
             S[np.where(np.abs(S) < self.regularization)] = 1.0
             w /= S
-            
+
             xn, yn = np.meshgrid(neighbors, neighbors)
             W[xn, yn] += w.dot(w.T)
-            
+
             if self.verbose and i % 100 == 0:
-                print(f'[HessianLLE] Optimized weight for instance {i}/{m}', end='')
-                print(f' - weight-norm: {np.linalg.norm(w)}')
-        
+                print(f"[HessianLLE] Optimized weight for instance {i}/{m}", end="")
+                print(f" - weight-norm: {np.linalg.norm(w)}")
+
         _, sig, VT = np.linalg.svd(W, full_matrices=0)
-        indices = np.argsort(sig)[1:self.n_components + 1]
+        indices = np.argsort(sig)[1 : self.n_components + 1]
         Y = VT[indices, :] * np.sqrt(m)
-        
+
         _, sig, VT = np.linalg.svd(Y, full_matrices=0)
         S = np.matrix(np.diag(sig ** (-1)))
         R = VT.T * S * VT
         self.Y, self.R = Y, R
         self._fitted = True
         return self
-    
+
     def transform(self) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         return Matrix(self.Y * self.R).T
-    
+
     def fit_transform(self, X: Matrix) -> Matrix:
         self.fit(X)
         return self.transform()
-    
+
     def _construct_graph(self, X: Matrix) -> Matrix:
         m, _ = X.shape
         kd_tree = KDTree(X.copy())
         index_mat = np.ones((m, self.n_neighbors), dtype=int)
         for i in range(m):
             _, neighbors = kd_tree.query(X[i], k=self.n_neighbors + 1, p=2)
             neighbors = neighbors.tolist()
             neighbors.remove(i)
             index_mat[i] = Matrix([neighbors])
-        
+
         return index_mat
 
 
 class SammonMapping(Transformer, Unsupervised):
-    
     """
-    Sammon mapping is a dimensionality reduction algorithm designed to transform 
-    high-dimensional data into a lower-dimensional space. Sammon mapping focuses 
-    on preserving the pairwise distances or dissimilarities between data points, 
+    Sammon mapping is a dimensionality reduction algorithm designed to transform
+    high-dimensional data into a lower-dimensional space. Sammon mapping focuses
+    on preserving the pairwise distances or dissimilarities between data points,
     making it well-suited for capturing non-linear relationships in the data.
-    
+
     Parameters
     ----------
     `n_components` : Dimensionality of low-space
     `max_iter` : Number of iteration
     `max_halves` : Number of halving of step-size
     `tol` : Threshold for early-stopping
     `initialize` : Methodology for embedding-space initialization
-    
+
     """
-    
-    def __init__(self,
-                 n_components: int = None,
-                 max_iter: int = 100,
-                 max_halves: int = 20,
-                 tol: float = 1e-5,
-                 initialize: Literal['pca'] | None = 'pca',
-                 verbose: bool = False) -> None:
+
+    def __init__(
+        self,
+        n_components: int = None,
+        max_iter: int = 100,
+        max_halves: int = 20,
+        tol: float = 1e-5,
+        initialize: Literal["pca"] | None = "pca",
+        verbose: bool = False,
+    ) -> None:
         self.n_components = n_components
         self.max_iter = max_iter
         self.max_halves = max_halves
         self.tol = tol
         self.initialize = initialize
         self.verbose = verbose
         self._fitted = False
-    
-    def fit(self, X: Matrix) -> 'SammonMapping':
+
+        self.set_param_ranges(
+            {
+                "n_components": ("0<,+inf", int),
+                "max_iter": ("0<,+inf", int),
+                "max_halves": ("0<,+inf", int),
+            }
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix) -> "SammonMapping":
         m, _ = X.shape
         X_dist = cdist(X, X)
         scale = 0.5 / X_dist.sum()
-        
+
         Y = np.random.normal(0, 1, (m, self.n_components))
-        if self.initialize == 'pca':
+        if self.initialize == "pca":
             Y = PCA(n_components=self.n_components).fit_transform(X)
             if self.verbose:
-                print('[SammonMap] Finished PCA initialization')
-        
+                print("[SammonMap] Finished PCA initialization")
+
         ones = np.ones((m, self.n_components))
         X_dist += np.eye(m)
         X_dist_inv = 1 / X_dist
         self._remove_inf(X_dist_inv, X_dist_inv)
-        
+
         Y_dist = cdist(Y, Y) + np.eye(m)
         Y_dist_inv = 1 / Y_dist
-        
+
         self._fill_diagnoal(X_dist, 1)
         self._fill_diagnoal(Y_dist, 1)
         self._fill_diagnoal(X_dist_inv, 0)
         self._fill_diagnoal(Y_dist_inv, 0)
-        
+
         self._remove_inf(matrix=X_dist_inv, filter=X_dist_inv)
         self._remove_inf(matrix=Y_dist_inv, filter=X_dist_inv)
         self._remove_inf(matrix=X_dist_inv, filter=Y_dist_inv)
         self._remove_inf(matrix=Y_dist_inv, filter=Y_dist_inv)
-        
+
         E = np.sum(((X_dist - Y_dist) ** 2) * X_dist_inv)
         for i in range(self.max_iter):
             delta = Y_dist_inv - X_dist_inv
             delta_one = delta.dot(ones)
-            
+
             gradient = np.dot(delta, Y) - (Y * delta_one)
-            hessian = np.dot(Y_dist_inv ** 3, Y ** 2) - delta_one
-            hessian -= np.dot(2, Y) * np.dot(Y_dist_inv ** 3, Y)
-            hessian += Y ** 2 * np.dot(Y_dist_inv ** 3, ones)
-            
-            step = -gradient.flatten(order='F') / np.abs(hessian.flatten(order='F'))
+            hessian = np.dot(Y_dist_inv**3, Y**2) - delta_one
+            hessian -= np.dot(2, Y) * np.dot(Y_dist_inv**3, Y)
+            hessian += Y**2 * np.dot(Y_dist_inv**3, ones)
+
+            step = -gradient.flatten(order="F") / np.abs(hessian.flatten(order="F"))
             Y_old = Y
-            
+
             for j in range(self.max_halves):
                 step_reshape = step.reshape(2, round(len(step) / 2)).T
                 y = Y_old + step_reshape
-                
+
                 dist = cdist(Y, y) + np.eye(m)
                 dist_inv = 1 / dist
                 self._remove_inf(matrix=dist_inv, filter=dist_inv)
-                
+
                 delta = X_dist - dist
-                E_new = np.sum((delta ** 2) * X_dist_inv)
-                if E_new < E: break
-                else: step = np.dot(0.5, step)
-            
+                E_new = np.sum((delta**2) * X_dist_inv)
+                if E_new < E:
+                    break
+                else:
+                    step = np.dot(0.5, step)
+
             if j == self.max_halves:
-                print(f'[SammonMap] Warning: max halves reached.', end='')
-                print(' Optimization may not converge!')
-            
+                print(f"[SammonMap] Warning: max halves reached.", end="")
+                print(" Optimization may not converge!")
+
             if np.abs((E - E_new) / E) < self.tol:
-                print(f'[SammonMap] Early convergence at iteration {i}/{self.max_iter}')
+                print(f"[SammonMap] Early convergence at iteration {i}/{self.max_iter}")
                 break
-            
+
             if self.verbose and i % 10 == 0:
-                print(f'[SammonMap] Iteration: {i}/{self.max_iter}', end='')
-                print(f' - relative delta-error: {np.abs((E - E_new) / E)}')
-            
+                print(f"[SammonMap] Iteration: {i}/{self.max_iter}", end="")
+                print(f" - relative delta-error: {np.abs((E - E_new) / E)}")
+
             E = E_new
         self.error = E * scale
         self.Y = y
-        
-        if self.verbose: print(f'[SammonMap] Final error: {self.error}')
+
+        if self.verbose:
+            print(f"[SammonMap] Final error: {self.error}")
         self._fitted = True
         return self
-    
+
     def _fill_diagnoal(self, matrix: Matrix, value: float) -> None:
         np.fill_diagonal(matrix, value)
-    
+
     def _remove_inf(self, matrix: Matrix, filter: Matrix) -> None:
         matrix[np.isinf(filter)] = 0
-    
+
     def transform(self) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         return self.Y
-    
+
     def fit_transform(self, X: Matrix) -> Matrix:
         self.fit(X)
         return self.transform()
 
 
 class LaplacianEigenmap(Transformer, Unsupervised):
-    
     """
-    Laplacian Eigenmap is a dimensionality reduction technique that 
-    transforms high-dimensional data into a lower-dimensional space while 
-    preserving local relationships. It constructs a weighted graph based 
-    on pairwise similarities between data points, computes the Laplacian 
-    matrix from the graph, and performs eigenvalue decomposition to 
+    Laplacian Eigenmap is a dimensionality reduction technique that
+    transforms high-dimensional data into a lower-dimensional space while
+    preserving local relationships. It constructs a weighted graph based
+    on pairwise similarities between data points, computes the Laplacian
+    matrix from the graph, and performs eigenvalue decomposition to
     obtain eigenvectors.
-    
+
     Parameters
     ----------
     `n_components` : Dimensionality of the lower-dimensional space
     `sigma` : Width parameter for Gaussian kernel in affinity calculation
-    
+
     """
 
     def __init__(self, n_components: int = None, sigma: float = 1.0) -> None:
         self.n_components = n_components
         self.sigma = sigma
         self.embedding = None
         self._fitted = False
-    
-    def fit(self, X: Matrix) -> 'LaplacianEigenmap':
+
+        self.set_param_ranges(
+            {"n_components": ("0<,+inf", int), "sigma": ("0<,+inf", None)}
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix) -> "LaplacianEigenmap":
         pairwise = cdist(X, X)
-        weights = np.exp(-pairwise / (2 * self.sigma ** 2))
+        weights = np.exp(-pairwise / (2 * self.sigma**2))
         np.fill_diagonal(weights, 0)
-        
+
         laplacian = self._compute_laplacian(weights)
         normalized_laplacian = self._normalize_laplacian(weights, laplacian)
-        
+
         eigvals, eigvecs = np.linalg.eigh(normalized_laplacian)
         sorted_indices = np.argsort(eigvals)
         eigvals = eigvals[sorted_indices]
         eigvecs = eigvecs[:, sorted_indices]
-        self.embedding = eigvecs[:, :self.n_components]
+        self.embedding = eigvecs[:, : self.n_components]
         self._fitted = True
         return self
 
     def _compute_laplacian(self, W: Matrix) -> Matrix:
         return np.diag(np.sum(W, axis=1)) - W
-    
+
     def _normalize_laplacian(self, W: Matrix, L: Matrix) -> Matrix:
         D_sqrt_inv = np.linalg.inv(np.sqrt(np.diag(np.sum(W, axis=1))))
         return D_sqrt_inv.dot(L).dot(D_sqrt_inv)
-    
+
     def transform(self) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         return self.embedding
-    
+
     def fit_transform(self, X: Matrix) -> Matrix:
         self.fit(X)
         return self.transform()
 
 
 class Isomap(Transformer, Unsupervised):
-    
     """
-    Isomap, or Isometric Mapping, is a nonlinear dimensionality reduction technique 
-    employed in machine learning. It focuses on preserving the geodesic distances 
-    between data points in high-dimensional datasets. By constructing a neighborhood 
-    graph and calculating pairwise geodesic distances, Isomap transforms the data 
-    into a lower-dimensional space, offering insights into complex, nonlinear 
+    Isomap, or Isometric Mapping, is a nonlinear dimensionality reduction technique
+    employed in machine learning. It focuses on preserving the geodesic distances
+    between data points in high-dimensional datasets. By constructing a neighborhood
+    graph and calculating pairwise geodesic distances, Isomap transforms the data
+    into a lower-dimensional space, offering insights into complex, nonlinear
     relationships within the dataset.
-    
+
     Parameters
     ----------
     `n_components` : Dimensionality of low-space
     `epsilon` : Boundary radius of the neighbor hypersphere
     `algorithm` : Shortest path finding algorithm
     (e.g. `dijkstra`, `floyd`)
     `metric` : Distance metric
     (e.g. `euclidean`, `cityblock`, `chebyshev`, `cosine`, `correlation`)
-    
+
     """
-    
-    def __init__(self, 
-                 n_components: int = None, 
-                 epsilon: float = 5.0,
-                 algorithm: Literal['dijkstra', 'floyd'] = 'dijkstra',
-                 metric: Literal['euclidean', 'cityblock', 'chebyshev',
-                                 'cosine', 'correlation'] = 'euclidean') -> None:
+
+    def __init__(
+        self,
+        n_components: int = None,
+        epsilon: float = 5.0,
+        algorithm: Literal["dijkstra", "floyd"] = "dijkstra",
+        metric: Literal[
+            "euclidean", "cityblock", "chebyshev", "cosine", "correlation"
+        ] = "euclidean",
+    ) -> None:
         self.n_components = n_components
         self.epsilon = epsilon
         self.algorithm = algorithm
         self.metric = metric
         self._fitted = False
-    
-    def fit(self, X: Matrix) -> 'Isomap':
+
+        self.set_param_ranges(
+            {"n_components": ("0<,+inf", int), "epsilon": ("0<,+inf", None)}
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix) -> "Isomap":
         self.adj = self._make_adjacency(X)
-        if np.isinf(self.adj).any(): 
-            print(f'[Isomap] Too narrow bin size with epsilon of {self.epsilon}!')
+        if np.isinf(self.adj).any():
+            print(f"[Isomap] Too narrow bin size with epsilon of {self.epsilon}!")
             return
-        
+
         m, _ = self.adj.shape
         H = np.eye(m) - (1 / m) * np.ones((m, m))
-        C = -0.5 / m * H.dot(self.adj ** 2).dot(H)
-        
+        C = -0.5 / m * H.dot(self.adj**2).dot(H)
+
         eigvals, eigvecs = eigh(C)
         indices = eigvals.argsort()[::-1]
         eigvals, eigvecs = eigvals[indices], eigvecs[:, indices]
-        self.eigvals = eigvals[:self.n_components]
-        self.eigvecs = eigvecs[:, :self.n_components]
+        self.eigvals = eigvals[: self.n_components]
+        self.eigvecs = eigvecs[:, : self.n_components]
         self._fitted = True
         return self
 
     def _make_adjacency(self, X: Matrix) -> Matrix:
         m, _ = X.shape
         distance = cdist(X, X, metric=self.metric)
         adjacency = np.zeros((m, m)) + np.inf
         bin = distance < self.epsilon
         adjacency[bin] = distance[bin]
-        
-        if self.algorithm == 'dijkstra':
-            path_mat = shortest_path(adjacency, directed=False, method='D')
-        elif self.algorithm == 'floyd':
-            path_mat = shortest_path(adjacency, directed=False, method='FW')
-        else: raise UnsupportedParameterError(self.algorithm)
+
+        if self.algorithm == "dijkstra":
+            path_mat = shortest_path(adjacency, directed=False, method="D")
+        elif self.algorithm == "floyd":
+            path_mat = shortest_path(adjacency, directed=False, method="FW")
+        else:
+            raise UnsupportedParameterError(self.algorithm)
         return path_mat
 
     def transform(self) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         return self.eigvecs.dot(np.diag(np.sqrt(self.eigvals)))
-    
+
     def fit_transform(self, X: Matrix) -> Matrix:
         self.fit(X)
         return self.transform()
 
 
 class ConformalIsomap(Transformer, Unsupervised):
-    
     """
-    Conformal Isomap (C-Isomap) is a variation of the Isomap algorithm that 
-    prioritizes preserving infinitesimal angles (conformality) by adjusting 
-    geodesic distances to reflect scale information. Unlike traditional Isomap, 
-    which focuses on preserving full isometry, C-Isomap is well-suited for 
+    Conformal Isomap (C-Isomap) is a variation of the Isomap algorithm that
+    prioritizes preserving infinitesimal angles (conformality) by adjusting
+    geodesic distances to reflect scale information. Unlike traditional Isomap,
+    which focuses on preserving full isometry, C-Isomap is well-suited for
     datasets with varying local scales or non-uniform structures.
-    
+
     Parameters
     ----------
     `n_components` : Dimensionality of low-space
     `epsilon` : Boundary radius of the neighbor hypersphere
     `algorithm` : Shortest path finding algorithm
     (e.g. `dijkstra`, `floyd`)
-    
+
     """
-    
-    def __init__(self,
-                 n_components: int = None,
-                 epsilon: float = 5.0,
-                 algorithm: Literal['dijkstra', 'floyd'] = 'dijkstra') -> None:
+
+    def __init__(
+        self,
+        n_components: int = None,
+        epsilon: float = 5.0,
+        algorithm: Literal["dijkstra", "floyd"] = "dijkstra",
+    ) -> None:
         self.n_components = n_components
         self.epsilon = epsilon
         self.algorithm = algorithm
         self._fitted = False
-    
-    def fit(self, X: Matrix) -> 'ConformalIsomap':
+        
+        self.set_param_ranges(
+            {"n_components": ("0<,+inf", int), "epsilon": ("0<,+inf", None)}
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix) -> "ConformalIsomap":
         self.adj = self._make_adjacency(X)
         if np.isinf(self.adj).any():
-            print(f'[C-Isomap] Too narrow bin size with epsilon of {self.epsilon}!')
+            print(f"[C-Isomap] Too narrow bin size with epsilon of {self.epsilon}!")
             return
-        
+
         m, _ = self.adj.shape
         H = np.eye(m) - (1 / m) * np.ones((m, m))
-        C = -0.5 / m * H.dot(self.adj ** 2).dot(H)
-        
+        C = -0.5 / m * H.dot(self.adj**2).dot(H)
+
         eigvals, eigvecs = eigh(C)
         indices = eigvals.argsort()[::-1]
         eigvals, eigvecs = eigvals[indices], eigvecs[:, indices]
-        self.eigvals = eigvals[:self.n_components]
-        self.eigvecs = eigvecs[:, :self.n_components]
+        self.eigvals = eigvals[: self.n_components]
+        self.eigvecs = eigvecs[:, : self.n_components]
         self._fitted = True
         return self
-    
+
     def _make_adjacency(self, X: Matrix) -> Matrix:
         m, _ = X.shape
-        distance = cdist(X, X, metric='euclidean')
+        distance = cdist(X, X, metric="euclidean")
         adjacency = np.zeros((m, m)) + np.inf
         bin = distance < self.epsilon
         adjacency[bin] = distance[bin]
-        
+
         masked = np.ma.masked_array(adjacency, mask=np.isinf(adjacency))
         masked_mean = np.ma.mean(masked, axis=0)
         for i in range(m):
             for j in range(m):
                 adjacency[i, j] /= np.sqrt(masked_mean[i] * masked_mean[j])
 
-        if self.algorithm == 'dijkstra':
-            path_mat = shortest_path(adjacency, directed=False, method='D')
-        elif self.algorithm == 'floyd':
-            path_mat = shortest_path(adjacency, directed=False, method='FW')
-        else: raise UnsupportedParameterError(self.algorithm)
+        if self.algorithm == "dijkstra":
+            path_mat = shortest_path(adjacency, directed=False, method="D")
+        elif self.algorithm == "floyd":
+            path_mat = shortest_path(adjacency, directed=False, method="FW")
+        else:
+            raise UnsupportedParameterError(self.algorithm)
         return path_mat
-    
+
     def transform(self) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         return self.eigvecs.dot(np.diag(np.sqrt(self.eigvals)))
-    
+
     def fit_transform(self, X: Matrix) -> Matrix:
         self.fit(X)
         return self.transform()
 
 
 class LTSA(Transformer, Unsupervised):
-    
     """
-    Local Tangent Space Alignment (LTSA) is a dimensionality reduction technique 
-    that aims to preserve the local geometry of data points in a manifold. 
-    It works by approximating the tangent space at each data point and aligning 
-    these local tangent spaces. This helps to capture the intrinsic structure 
-    of the data, particularly in cases where the global geometry might be 
-    complex or non-linear. 
-    
+    Local Tangent Space Alignment (LTSA) is a dimensionality reduction technique
+    that aims to preserve the local geometry of data points in a manifold.
+    It works by approximating the tangent space at each data point and aligning
+    these local tangent spaces. This helps to capture the intrinsic structure
+    of the data, particularly in cases where the global geometry might be
+    complex or non-linear.
+
     Parameters
     ----------
     `n_components` : Dimensionality of low-space
     `n_neighbors` : Number of neighbors
-    
+
     """
-    
-    def __init__(self,
-                 n_components: int = None,
-                 n_neighbors: int = 10) -> None:
+
+    def __init__(self, n_components: int = None, n_neighbors: int = 10) -> None:
         self.n_components = n_components
         self.n_neighbors = n_neighbors
         self._fitted = False
-    
-    def fit(self, X: Matrix) -> 'LTSA':
+        
+        self.set_param_ranges(
+            {"n_components": ("0<,+inf", int), "n_neighbors": ("0<,+inf", int)}
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix) -> "LTSA":
         m, n = X.shape
         self.neighbors, self.neighbor_indices = self._compute_neighborhood(X)
         M = np.zeros((m, m))
         use_svd = self.n_neighbors > n
-        
+
         for i in range(m):
             Xi = self.neighbors[i]
             Xi -= np.mean(self.neighbors[i], axis=0)
             if use_svd:
                 v = svd(Xi, full_matrices=True)[0]
             else:
                 Ci = Xi.dot(Xi.T)
                 v = eigh(Ci)[1][:, ::-1]
-            
+
             Gi = np.zeros((self.n_neighbors, self.n_components + 1))
-            Gi[:, 1:] = v[:, :self.n_components]
+            Gi[:, 1:] = v[:, : self.n_components]
             Gi[:, 0] = 1 / np.sqrt(self.n_neighbors)
-            
-            neighbors_x, neighbors_y = np.meshgrid(self.neighbor_indices[i], 
-                                                   self.neighbor_indices[i])
+
+            neighbors_x, neighbors_y = np.meshgrid(
+                self.neighbor_indices[i], self.neighbor_indices[i]
+            )
             M[neighbors_x, neighbors_y] -= Gi.dot(Gi.T)
             M[self.neighbor_indices[i], self.neighbor_indices[i]] += 1
-        
+
         self._M = M
         self._fitted = True
         return self
-    
+
     def _compute_neighborhood(self, X: Matrix) -> Matrix:
-        distances = cdist(X, X, metric='euclidean')
-        indices = np.argsort(distances, axis=1)[:, :self.n_neighbors]
+        distances = cdist(X, X, metric="euclidean")
+        indices = np.argsort(distances, axis=1)[:, : self.n_neighbors]
         return X[indices], indices
-    
+
     def _find_null_space(self, M: Matrix) -> Matrix:
-        eigvals, eigvecs = eigh(M, subset_by_index=(1, self.n_components), 
-                                overwrite_a=True)
+        eigvals, eigvecs = eigh(
+            M, subset_by_index=(1, self.n_components), overwrite_a=True
+        )
         indices = np.argsort(np.abs(eigvals))
         return eigvecs[:, indices]
-    
+
     def transform(self) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         return self._find_null_space(self._M)
-    
+
     def fit_transform(self, X: Matrix) -> Matrix:
         self.fit(X)
         return self.transform()
-
```

### Comparing `luma-ml-0.6.4/luma/regressor/general.py` & `luma-ml-0.6.5/luma/regressor/general.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,436 +5,481 @@
 from luma.interface.util import Matrix
 from luma.interface.exception import NotFittedError, UnsupportedParameterError
 from luma.core.super import Estimator, Evaluator, Supervised
 from luma.metric.regression import MeanSquaredError
 
 
 __all__ = (
-    'PoissonRegressor', 
-    'NegativeBinomialRegressor', 
-    'GammaRegressor',
-    'BetaRegressor', 
-    'InverseGaussianRegressor'
+    "PoissonRegressor",
+    "NegativeBinomialRegressor",
+    "GammaRegressor",
+    "BetaRegressor",
+    "InverseGaussianRegressor",
 )
 
 
 class PoissonRegressor(Estimator, Supervised):
-    
     """
-    Poisson regression is a model for predicting count or frequency data. 
-    It models the relationship between features and counts, with a focus 
-    on count data that follows a Poisson distribution. The model uses 
-    the natural logarithm of expected counts as a link function and is 
+    Poisson regression is a model for predicting count or frequency data.
+    It models the relationship between features and counts, with a focus
+    on count data that follows a Poisson distribution. The model uses
+    the natural logarithm of expected counts as a link function and is
     trained to minimize the negative log-likelihood.
-    
+
     Parameters
     ----------
     `learning_rate` : Step size of the gradient descent update
     `max_iter` : Number of iteration
-    `l1_ratio` : Balancing parameter of `elastic-net` 
+    `l1_ratio` : Balancing parameter of `elastic-net`
     `alpha` : Regularization strength
     `regularization` : Regularization type (e.g. `l1`, `l2`, `elastic-net`)
-    
+
     """
-    
-    def __init__(self,
-                 learning_rate: float = 0.01,
-                 max_iter: int = 100,
-                 l1_ratio: float = 0.5,
-                 alpha: float = 0.01,
-                 regularization: Literal['l1', 'l2','elastic-net'] = None,
-                 verbose: bool = False) -> None:
+
+    def __init__(
+        self,
+        learning_rate: float = 0.01,
+        max_iter: int = 100,
+        l1_ratio: float = 0.5,
+        alpha: float = 0.01,
+        regularization: Literal["l1", "l2", "elastic-net"] = None,
+        verbose: bool = False,
+    ) -> None:
         self.learning_rate = learning_rate
         self.max_iter = max_iter
         self.regularization = regularization
         self.l1_ratio = l1_ratio
         self.alpha = alpha
         self.verbose = verbose
         self._fitted = False
-    
+
     def link_funciton(self, X: Matrix) -> Matrix:
         return np.exp(np.dot(X, self.weights))
-    
-    def fit(self, X: Matrix, y: Matrix) -> 'PoissonRegressor':
+
+    def fit(self, X: Matrix, y: Matrix) -> "PoissonRegressor":
         X = np.column_stack((np.ones(X.shape[0]), X))
         m, n = X.shape
         self.weights = np.zeros(n)
-        
+
         for i in range(self.max_iter):
             predictions = self.link_funciton(X)
             gradient = np.dot(X.T, y - predictions) * self.learning_rate
             gradient /= m
-            
+
             if self.regularization:
                 regularization_term = self._regularization_term()
                 gradient -= self.alpha * regularization_term / m
-            
+
             if self.verbose and i % 10 == 0:
-                print(f'[PoissonReg] iteration: {i}/{self.max_iter}', end='')
-                print(f' - gradient-norm: {np.linalg.norm(gradient)}')
-            
+                print(f"[PoissonReg] iteration: {i}/{self.max_iter}", end="")
+                print(f" - gradient-norm: {np.linalg.norm(gradient)}")
+
             self.weights += gradient
         self._fitted = True
         return self
-    
+
     def _regularization_term(self) -> Matrix:
-        if self.regularization == 'l1': return np.sign(self.weights)
-        elif self.regularization == 'l2': return self.weights
-        elif self.regularization == 'elastic-net':
+        if self.regularization == "l1":
+            return np.sign(self.weights)
+        elif self.regularization == "l2":
+            return self.weights
+        elif self.regularization == "elastic-net":
             l1_term = np.sign(self.weights)
             l2_term = 2 * self.weights
             return (1 - self.l1_ratio) * l2_term + self.l1_ratio * l1_term
-        elif self.regularization is None: return np.zeros_like(self.weights)
-        else: raise UnsupportedParameterError(self.regularization)
-    
+        elif self.regularization is None:
+            return np.zeros_like(self.weights)
+        else:
+            raise UnsupportedParameterError(self.regularization)
+
     def predict(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         X = np.column_stack((np.ones(X.shape[0]), X))
         predictions = self.link_funciton(X)
         return predictions
-    
-    def score(self, X: Matrix, y: Matrix, 
-              metric: Evaluator = MeanSquaredError) -> float:
+
+    def score(
+        self, X: Matrix, y: Matrix, metric: Evaluator = MeanSquaredError
+    ) -> float:
         X_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=X_pred)
 
 
 class NegativeBinomialRegressor(Estimator, Supervised):
-    
     """
-    Negative Binomial Regression is a statistical method used to 
-    model count data, like the number of events or occurrences, 
-    when the data shows overdispersion (variance is greater than mean) 
-    compared to the Poisson distribution. It estimates how predictors 
+    Negative Binomial Regression is a statistical method used to
+    model count data, like the number of events or occurrences,
+    when the data shows overdispersion (variance is greater than mean)
+    compared to the Poisson distribution. It estimates how predictors
     influence the count while allowing for flexible variance modeling.
-    
+
     Parameters
     ----------
     `learning_rate` : Step size of the gradient descent update
     `max_iter` : Number of iteration
     `alpha` : Regularization strength
-    `l1_ratio` : Balancing parameter of `elastic-net` 
+    `l1_ratio` : Balancing parameter of `elastic-net`
     `phi` : Dispersion parameter
     `regularization` : Regularization type (e.g. `l1`, `l2`, `elastic-net`)
-    
+
     """
-    
-    def __init__(self,
-                 learning_rate: float = 0.01,
-                 max_iter: int = 100,
-                 alpha: float = 0.01,
-                 l1_ratio: float = 0.5,
-                 phi: float = 1.0,
-                 regularization: Literal['l1', 'l2', 'elastic-net'] = None,
-                 verbose: bool = False) -> None:
+
+    def __init__(
+        self,
+        learning_rate: float = 0.01,
+        max_iter: int = 100,
+        alpha: float = 0.01,
+        l1_ratio: float = 0.5,
+        phi: float = 1.0,
+        regularization: Literal["l1", "l2", "elastic-net"] = None,
+        verbose: bool = False,
+    ) -> None:
         self.learning_rate = learning_rate
         self.max_iter = max_iter
         self.alpha = alpha
         self.l1_ratio = l1_ratio
         self.phi = phi
         self.regularization = regularization
         self.verbose = verbose
         self._fitted = False
-    
+
     def link_function(self, X: Matrix) -> Matrix:
         return np.log(1 + np.exp(np.dot(X, self.weights)))
-    
-    def fit(self, X: Matrix, y: Matrix) -> 'NegativeBinomialRegressor':
-        X = np.column_stack((np.ones(X.shape[0]),  X))
+
+    def fit(self, X: Matrix, y: Matrix) -> "NegativeBinomialRegressor":
+        X = np.column_stack((np.ones(X.shape[0]), X))
         m, n = X.shape
         self.weights = np.zeros(n)
-        
+
         for i in range(self.max_iter):
             mu = self.link_function(X)
             gradient = (y - mu) / (self.phi * (1 + mu / self.phi))
             gradient = np.dot(X.T, gradient) * self.learning_rate
             gradient /= m
-            
+
             if self.regularization:
                 regularization_term = self._regularization_term()
                 gradient -= self.alpha * regularization_term / m
-            
+
             if self.verbose and i % 10 == 0:
-                print(f'[NegBinReg] iteration: {i}/{self.max_iter}', end='')
-                print(f' - gradient-norm: {np.linalg.norm(gradient)}')
-            
+                print(f"[NegBinReg] iteration: {i}/{self.max_iter}", end="")
+                print(f" - gradient-norm: {np.linalg.norm(gradient)}")
+
             self.weights += gradient
         self._fitted = True
         return self
-    
+
     def _regularization_term(self) -> Matrix:
-        if self.regularization == 'l1': return np.sign(self.weights)
-        elif self.regularization == 'l2': return self.weights
-        elif self.regularization == 'elastic-net':
+        if self.regularization == "l1":
+            return np.sign(self.weights)
+        elif self.regularization == "l2":
+            return self.weights
+        elif self.regularization == "elastic-net":
             l1_term = np.sign(self.weights)
             l2_term = 2 * self.weights
             return (1 - self.l1_ratio) * l2_term + self.l1_ratio * l1_term
-        elif self.regularization is None: return np.zeros_like(self.weights)
-        else: raise UnsupportedParameterError(self.regularization)
-    
+        elif self.regularization is None:
+            return np.zeros_like(self.weights)
+        else:
+            raise UnsupportedParameterError(self.regularization)
+
     def predict(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         X = np.column_stack((np.ones(X.shape[0]), X))
         mu = self.link_function(X)
         return mu
-    
-    def score(self, X: Matrix, y: Matrix, 
-              metric: Evaluator = MeanSquaredError) -> float:
+
+    def score(
+        self, X: Matrix, y: Matrix, metric: Evaluator = MeanSquaredError
+    ) -> float:
         X_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=X_pred)
 
 
 class GammaRegressor(Estimator, Supervised):
-    
     """
-    Gamma regression is a statistical method for analyzing 
-    data with skewed, positively skewed distributions and where 
-    the variance increases with the mean. It models the 
-    relationship between variables using the gamma distribution, 
-    making it suitable for situations where traditional 
+    Gamma regression is a statistical method for analyzing
+    data with skewed, positively skewed distributions and where
+    the variance increases with the mean. It models the
+    relationship between variables using the gamma distribution,
+    making it suitable for situations where traditional
     linear regression doesn't apply.
-    
+
     Parameters
     ----------
     `alpha` : Shape parameter of gamma distribution
     `beta` : Scale parameter of gamma distribution
     `learning_rate` : Step size of the gradient descent update
     `max_iter` : Number of iteration
     `reg_strength` : Regularization strength
-    `l1_ratio` : Balancing parameter of `elastic-net` 
+    `l1_ratio` : Balancing parameter of `elastic-net`
     `regularization` : Regularization type (e.g. `l1`, `l2`, `elastic-net`)
-    
+
     """
-    
-    def __init__(self,
-                 alpha: float = 1.0,
-                 beta: float = 1.0,
-                 learning_rate: float = 0.01,
-                 max_iter: int = 100,
-                 reg_strength: float = 0.01,
-                 l1_ratio: float = 0.5,
-                 regularization: Literal['l1', 'l2', 'elastic-net'] = None,
-                 verbose: bool = False) -> None:
+
+    def __init__(
+        self,
+        alpha: float = 1.0,
+        beta: float = 1.0,
+        learning_rate: float = 0.01,
+        max_iter: int = 100,
+        reg_strength: float = 0.01,
+        l1_ratio: float = 0.5,
+        regularization: Literal["l1", "l2", "elastic-net"] = None,
+        verbose: bool = False,
+    ) -> None:
         self.alpha = alpha
         self.beta = beta
         self.learning_rate = learning_rate
         self.max_iter = max_iter
         self.reg_strength = reg_strength
         self.l1_ratio = l1_ratio
         self.regularization = regularization
         self.verbose = verbose
         self._fitted = False
-    
-    def fit(self, X: Matrix, y: Matrix) -> 'GammaRegressor':
+
+    def fit(self, X: Matrix, y: Matrix) -> "GammaRegressor":
         X = np.column_stack((np.ones(X.shape[0]), X))
         m, n = X.shape
         self.alpha = np.ones(n) * self.alpha
         self.beta = np.ones(n) * self.beta
-        
+
         for i in range(self.max_iter):
             gradient = (self.alpha - 1) / self.alpha - psi(self.alpha)
             gradient += np.log(self.beta) - (y / self.beta)
-            
+
             self.alpha += self.learning_rate * np.mean(gradient * X, axis=0) / m
-            self.beta += self.learning_rate / m * \
-                np.mean((self.alpha / self.beta ** 2 - y / self.beta) * X, axis=0)
-            
+            self.beta += (
+                self.learning_rate
+                / m
+                * np.mean((self.alpha / self.beta**2 - y / self.beta) * X, axis=0)
+            )
+
             if self.regularization:
-                self.alpha -= self.reg_strength * self._regularization_term(self.alpha) / m
-                self.beta -= self.reg_strength * self._regularization_term(self.beta) / m
-            
+                self.alpha -= (
+                    self.reg_strength * self._regularization_term(self.alpha) / m
+                )
+                self.beta -= (
+                    self.reg_strength * self._regularization_term(self.beta) / m
+                )
+
             if self.verbose and i % 10 == 0:
-                print(f'[GammaReg] iteration: {i}/{self.max_iter}', end='')
-                print(f' - gradient-norm: {np.linalg.norm(gradient)}')
-        
+                print(f"[GammaReg] iteration: {i}/{self.max_iter}", end="")
+                print(f" - gradient-norm: {np.linalg.norm(gradient)}")
+
         self._fitted = True
         return self
-    
+
     def _regularization_term(self, weights: Matrix) -> Matrix:
-        if self.regularization == 'l1': return np.sign(weights)
-        elif self.regularization == 'l2': return self.weights
-        elif self.regularization == 'elastic-net':
+        if self.regularization == "l1":
+            return np.sign(weights)
+        elif self.regularization == "l2":
+            return self.weights
+        elif self.regularization == "elastic-net":
             l1_term = np.sign(weights)
             l2_term = 2 * weights
             return (1 - self.l1_ratio) * l2_term + self.l1_ratio * l1_term
-        elif self.regularization is None: return np.zeros_like(weights)
-        else: raise UnsupportedParameterError(self.regularization)
+        elif self.regularization is None:
+            return np.zeros_like(weights)
+        else:
+            raise UnsupportedParameterError(self.regularization)
 
     def predict(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         X = np.column_stack((np.ones(X.shape[0]), X))
         return np.dot(X, self.alpha / self.beta)
-    
-    def score(self, X: Matrix, y: Matrix, 
-              metric: Evaluator = MeanSquaredError) -> float:
+
+    def score(
+        self, X: Matrix, y: Matrix, metric: Evaluator = MeanSquaredError
+    ) -> float:
         X_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=X_pred)
 
 
 class BetaRegressor(Estimator, Supervised):
-    
     """
-    Beta regression is a statistical model used in machine learning to 
-    analyze and predict data that follows a bounded interval between 
-    0 and 1, such as proportions, probabilities, or percentages. 
-    It's particularly useful for modeling data with heteroscedasticity, 
+    Beta regression is a statistical model used in machine learning to
+    analyze and predict data that follows a bounded interval between
+    0 and 1, such as proportions, probabilities, or percentages.
+    It's particularly useful for modeling data with heteroscedasticity,
     where the spread of the data varies across different input values.
-    
+
     Parameters
     ----------
     `alpha`, `beta` : Shape parameters of beta function
     `learning_rate` : Step size of the gradient descent update
     `max_iter` : Number of iteration
     `reg_strength` : Regularization strength
     `l1_ratio` : Balacing parameter of `elastic-net`
     `regularization` : Regularization type (e.g. `l1`, `l2`, `elastic-net`)
-    
+
     """
 
-    def __init__(self,
-                 alpha: float = 1.0,
-                 beta: float = 1.0,
-                 learning_rate: float = 0.01,
-                 max_iter: int = 100,
-                 reg_strength: float = 0.01,
-                 l1_ratio: float = 0.5,
-                 regularization: Literal['l1', 'l2', 'elastic-net'] = None,
-                 verbose: bool = False) -> None:
+    def __init__(
+        self,
+        alpha: float = 1.0,
+        beta: float = 1.0,
+        learning_rate: float = 0.01,
+        max_iter: int = 100,
+        reg_strength: float = 0.01,
+        l1_ratio: float = 0.5,
+        regularization: Literal["l1", "l2", "elastic-net"] = None,
+        verbose: bool = False,
+    ) -> None:
         self.alpha = alpha
         self.beta = beta
         self.learning_rate = learning_rate
         self.max_iter = max_iter
         self.reg_strength = reg_strength
         self.l1_ratio = l1_ratio
         self.regularization = regularization
         self.verbose = verbose
         self._fitted = False
-    
-    def fit(self, X: Matrix, y: Matrix) -> 'BetaRegressor':
+
+    def fit(self, X: Matrix, y: Matrix) -> "BetaRegressor":
         X = np.column_stack((np.ones(X.shape[0]), X))
         m, n = X.shape
         self.alpha = np.ones(n) * self.alpha
         self.beta = np.ones(n) * self.beta
-        
+
         for i in range(self.max_iter):
             gradient_alpha = psi(self.alpha) - psi(self.alpha + self.beta)
             gradient_alpha += np.log(self.beta) - np.log(1 - y)
             gradient_beta = psi(self.beta) - psi(self.alpha + self.beta)
             gradient_beta += np.log(self.alpha) - np.log(y)
-            
+
             self.alpha -= self.learning_rate * np.mean(gradient_alpha * X, axis=0) / m
             self.beta -= self.learning_rate * np.mean(gradient_beta * X, axis=0) / m
-            
+
             if self.regularization:
-                self.alpha -= self.reg_strength * self._regularization_term(self.alpha) / m
-                self.beta -= self.reg_strength * self._regularization_term(self.beta) / m
-            
+                self.alpha -= (
+                    self.reg_strength * self._regularization_term(self.alpha) / m
+                )
+                self.beta -= (
+                    self.reg_strength * self._regularization_term(self.beta) / m
+                )
+
             if self.verbose and i % 10 == 0:
                 gradient_norm = np.linalg.norm(gradient_alpha + gradient_beta)
-                print(f'[BetaReg] iteration: {i}/{self.max_iter}', end='')
-                print(f' - gradient-norm: {gradient_norm}')
-        
+                print(f"[BetaReg] iteration: {i}/{self.max_iter}", end="")
+                print(f" - gradient-norm: {gradient_norm}")
+
         self._fitted = True
         return self
-    
+
     def _regularization_term(self, weights: Matrix) -> Matrix:
-        if self.regularization == 'l1': return np.sign(weights)
-        elif self.regularization == 'l2': return self.weights
-        elif self.regularization == 'elastic-net':
+        if self.regularization == "l1":
+            return np.sign(weights)
+        elif self.regularization == "l2":
+            return self.weights
+        elif self.regularization == "elastic-net":
             l1_term = np.sign(weights)
             l2_term = 2 * weights
             return (1 - self.l1_ratio) * l2_term + self.l1_ratio * l1_term
-        elif self.regularization is None: return np.zeros_like(weights)
-        else: raise UnsupportedParameterError(self.regularization)
-    
+        elif self.regularization is None:
+            return np.zeros_like(weights)
+        else:
+            raise UnsupportedParameterError(self.regularization)
+
     def predict(self, X: Matrix) -> float:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         X = np.column_stack((np.ones(X.shape[0]), X))
         return np.dot(X, self.alpha / (self.alpha + self.beta))
-    
-    def score(self, X: Matrix, y: Matrix, 
-              metric: Evaluator = MeanSquaredError) -> float:
+
+    def score(
+        self, X: Matrix, y: Matrix, metric: Evaluator = MeanSquaredError
+    ) -> float:
         X_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=X_pred)
 
 
 class InverseGaussianRegressor(Estimator, Supervised):
-    
     """
-    Inverse Gaussian regression is a statistical technique applied in 
-    machine learning to model relationships between predictor variables 
-    and continuous response variables when the response data exhibits 
+    Inverse Gaussian regression is a statistical technique applied in
+    machine learning to model relationships between predictor variables
+    and continuous response variables when the response data exhibits
     a skewed or non-normally distributed pattern.
-    
+
     Parameters
     ----------
     `learning_rate` : Step size of the gradient descent update
     `max_iter` : Number of iteration
     `phi` : Shape parameter of inverse Gaussian density
     `l1_ratio` : Balacing parameter of `elastic-net`
     `alpha` : Regularization strength
     `regularization` : Regularization type (e.g. `l1`, `l2`, `elastic-net`)
-    
+
     """
-    
-    def __init__(self,
-                 learning_rate: float = 0.01,
-                 max_iter: int = 100,
-                 phi: float = 1.0,
-                 l1_ratio: float = 0.5,
-                 alpha: float = 0.01,
-                 regularization: Literal['l1', 'l2', 'elastic-net'] = None,
-                 verbose: bool = False) -> None:
+
+    def __init__(
+        self,
+        learning_rate: float = 0.01,
+        max_iter: int = 100,
+        phi: float = 1.0,
+        l1_ratio: float = 0.5,
+        alpha: float = 0.01,
+        regularization: Literal["l1", "l2", "elastic-net"] = None,
+        verbose: bool = False,
+    ) -> None:
         self.learning_rate = learning_rate
         self.max_iter = max_iter
         self.phi = phi
         self.l1_ratio = l1_ratio
         self.alpha = alpha
         self.regularization = regularization
         self.verbose = verbose
         self._fitted = False
-    
-    def fit(self, X: Matrix, y: Matrix) -> 'InverseGaussianRegressor':
+
+    def fit(self, X: Matrix, y: Matrix) -> "InverseGaussianRegressor":
         X = np.column_stack((np.ones(X.shape[0]), X))
         m, n = X.shape
         self.weights = np.ones(n)
-        
+
         for i in range(self.max_iter):
             error = y - np.dot(X, self.weights)
-            
-            gradient = np.dot(X.T, (error * self.phi) / (2 * self.weights * y ** 2))
-            gradient += 0.5 * error ** 2 / (2 * self.weights * y)
+
+            gradient = np.dot(X.T, (error * self.phi) / (2 * self.weights * y**2))
+            gradient += 0.5 * error**2 / (2 * self.weights * y)
             gradient -= 0.5 * (self.phi / self.weights)
             gradient *= self.learning_rate / m
-            
+
             if self.regularization:
                 regularization_term = self._regularization_term()
                 gradient += self.alpha * regularization_term / m
-                
+
             if self.verbose and i % 10 == 0:
-                print(f'[InvGaussianReg] iteration: {i}/{self.max_iter}', end='')
-                print(f' - gradient-norm: {np.linalg.norm(gradient)}')
-            
+                print(f"[InvGaussianReg] iteration: {i}/{self.max_iter}", end="")
+                print(f" - gradient-norm: {np.linalg.norm(gradient)}")
+
             self.weights -= gradient
         self._fitted = True
         return self
-    
+
     def _regularization_term(self):
-        if self.regularization == 'l1': return np.sign(self.weights)
-        elif self.regularization == 'l2': return self.weights
-        elif self.regularization == 'elastic-net':
+        if self.regularization == "l1":
+            return np.sign(self.weights)
+        elif self.regularization == "l2":
+            return self.weights
+        elif self.regularization == "elastic-net":
             l1_term = np.sign(self.weights)
             l2_term = 2 * self.weights
             return (1 - self.l1_ratio) * l2_term + self.l1_ratio * l1_term
-        elif self.regularization is None: return np.zeros_like(self.weights)
-        else: raise UnsupportedParameterError(self.regularization)
-    
+        elif self.regularization is None:
+            return np.zeros_like(self.weights)
+        else:
+            raise UnsupportedParameterError(self.regularization)
+
     def predict(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         X = np.column_stack((np.ones(X.shape[0]), X))
         return 1 / (self.phi * X) * np.dot(X, self.weights)
-    
-    def score(self, X: Matrix, y: Matrix, 
-              metric: Evaluator = MeanSquaredError) -> float:
+
+    def score(
+        self, X: Matrix, y: Matrix, metric: Evaluator = MeanSquaredError
+    ) -> float:
         X_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=X_pred)
-
```

### Comparing `luma-ml-0.6.4/luma/regressor/linear.py` & `luma-ml-0.6.5/luma/regressor/linear.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,330 +3,344 @@
 from luma.interface.util import Matrix, Vector, KernelUtil
 from luma.interface.exception import NotFittedError
 from luma.core.super import Estimator, Evaluator, Supervised
 from luma.metric.regression import MeanSquaredError
 
 
 __all__ = (
-    'LinearRegressor', 
-    'RidgeRegressor', 
-    'LassoRegressor', 
-    'ElasticNetRegressor',
-    'KernelRidgeRegressor',
-    'BayesianRidgeRegressor'
+    "LinearRegressor",
+    "RidgeRegressor",
+    "LassoRegressor",
+    "ElasticNetRegressor",
+    "KernelRidgeRegressor",
+    "BayesianRidgeRegressor",
 )
 
 
 class RidgeRegressor(Estimator, Supervised):
-    
     """
-    Ridge regression is a linear regression technique used to 
-    prevent overfitting in predictive models. 
-    It adds a penalty term called "L2 regularization" to help 
-    reduce the complexity of the model and prevent it from 
+    Ridge regression is a linear regression technique used to
+    prevent overfitting in predictive models.
+    It adds a penalty term called "L2 regularization" to help
+    reduce the complexity of the model and prevent it from
     fitting noise in the data.
-    
+
     Parameters
     ----------
     `alpha` : L2-regularization strength
-    
+
     """
-    
+
     def __init__(self, alpha: float = 1.0) -> None:
         self.alpha = alpha
         self._fitted = False
 
-    def fit(self, X: Matrix, y: Matrix) -> 'RidgeRegressor':
+    def fit(self, X: Matrix, y: Matrix) -> "RidgeRegressor":
         X = np.column_stack((np.ones(X.shape[0]), X))
         identity_matrix = np.identity(X.shape[1])
         self.coef_ = np.linalg.inv(X.T.dot(X) + self.alpha * identity_matrix)
         self.coef_ = self.coef_.dot(X.T).dot(y)
         self._fitted = True
         return self
 
     def predict(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         X = np.column_stack((np.ones(X.shape[0]), X))
         return X.dot(self.coef_)
-    
-    def score(self, X: Matrix, y: Matrix, 
-              metric: Evaluator = MeanSquaredError) -> float:
+
+    def score(
+        self, X: Matrix, y: Matrix, metric: Evaluator = MeanSquaredError
+    ) -> float:
         X_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=X_pred)
 
 
 class LassoRegressor(Estimator, Supervised):
-    
     """
-    Lasso regression is a linear regression technique used for 
-    feature selection and regularization. It adds a penalty term, 
-    called "L1 regularization," to the standard linear regression 
-    objective function. Lasso encourages some of the model's 
-    coef_ to become exactly zero, effectively eliminating 
+    Lasso regression is a linear regression technique used for
+    feature selection and regularization. It adds a penalty term,
+    called "L1 regularization," to the standard linear regression
+    objective function. Lasso encourages some of the model's
+    coef_ to become exactly zero, effectively eliminating
     certain features from the model.
-    
+
     Parameters
     ----------
     `alpha` : L1-regularization strength
     `max_iter` : Number of iteration
     `learning_rate` : Step size of the gradient descent update
-    
+
     """
-    
-    def __init__(self, 
-                 alpha: float = 1.0, 
-                 max_iter: int = 100, 
-                 learning_rate: float = 0.01, 
-                 verbose: bool = False) -> None:
+
+    def __init__(
+        self,
+        alpha: float = 1.0,
+        max_iter: int = 100,
+        learning_rate: float = 0.01,
+        verbose: bool = False,
+    ) -> None:
         self.alpha = alpha
         self.max_iter = max_iter
         self.learning_rate = learning_rate
         self.verbose = verbose
         self._fitted = False
 
     def _soft_threshold(self, x: Matrix, threshold: float) -> Matrix:
         return np.sign(x) * np.maximum(0, np.abs(x) - threshold)
 
-    def fit(self, X: Matrix, y: Matrix) -> 'LassoRegressor':
+    def fit(self, X: Matrix, y: Matrix) -> "LassoRegressor":
         X = np.column_stack((np.ones(X.shape[0]), X))
         self.coef_ = np.zeros(X.shape[1])
-        
+
         for i in range(self.max_iter):
             coefficients_prev = self.coef_.copy()
             y_pred = X.dot(self.coef_)
             gradient = -(X.T.dot(y - y_pred)) * self.learning_rate
             self.coef_ = self.coef_ - (1.0 / X.shape[0]) * gradient
             self.coef_ = self._soft_threshold(self.coef_, self.alpha / X.shape[0])
-            
+
             if self.verbose and i % 10 == 0:
-                print(f'[LassoReg] iteration: {i}/{self.max_iter}', end='')
-                print(f' - delta-coeff norm: {np.linalg.norm(self.coef_ - coefficients_prev)}')
-        
+                print(f"[LassoReg] iteration: {i}/{self.max_iter}", end="")
+                print(
+                    f" - delta-coeff norm: {np.linalg.norm(self.coef_ - coefficients_prev)}"
+                )
+
         self._fitted = True
         return self
 
     def predict(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         X = np.column_stack((np.ones(X.shape[0]), X))
         return X.dot(self.coef_)
-    
-    def score(self, X: Matrix, y: Matrix, 
-              metric: Evaluator = MeanSquaredError) -> float:
+
+    def score(
+        self, X: Matrix, y: Matrix, metric: Evaluator = MeanSquaredError
+    ) -> float:
         X_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=X_pred)
 
 
 class ElasticNetRegressor(Estimator, Supervised):
-    
     """
-    Elastic-Net regression is a linear regression technique 
-    that combines both L1 (Lasso) and L2 (Ridge) regularization methods. 
-    It adds a combination of L1 and L2 penalty terms to the 
+    Elastic-Net regression is a linear regression technique
+    that combines both L1 (Lasso) and L2 (Ridge) regularization methods.
+    It adds a combination of L1 and L2 penalty terms to the
     standard linear regression objective function.
-    
+
     Parameters
     ----------
     `alpha` : Regularization strength
     `l1_ratio` : Balancing parameter between `l1` and `l2`
     `max_iter` : Number of iteration
     `learning_rate` : Step size of the gradient descent update
-    
+
     """
-    
-    def __init__(self, 
-                 alpha: float = 1.0, 
-                 l1_ratio: float = 0.5, 
-                 max_iter: int = 100, 
-                 learning_rate: float = 0.01,
-                 verbose: bool = False) -> None:
+
+    def __init__(
+        self,
+        alpha: float = 1.0,
+        l1_ratio: float = 0.5,
+        max_iter: int = 100,
+        learning_rate: float = 0.01,
+        verbose: bool = False,
+    ) -> None:
         self.alpha = alpha
         self.l1_ratio = l1_ratio
         self.max_iter = max_iter
         self.learning_rate = learning_rate
         self.verbose = verbose
         self.coef_ = None
         self._fitted = False
-        
+
     def _soft_threshold(self, x: Matrix, alpha: float) -> Matrix:
         return np.sign(x) * np.maximum(np.abs(x) - alpha, 0)
 
-    def fit(self, X: Matrix, y: Matrix) -> 'ElasticNetRegressor':
+    def fit(self, X: Matrix, y: Matrix) -> "ElasticNetRegressor":
         N, p = X.shape
         self.coef_ = np.zeros(p)
 
         for i in range(self.max_iter):
             y_pred = X.dot(self.coef_)
             gradient = -(1 / N) * X.T.dot(y - y_pred)
             lefthand = self.coef_ - self.learning_rate * gradient
             righthand = self.alpha * self.l1_ratio
-            
+
             self.coef_ = self._soft_threshold(lefthand, righthand)
             self.coef_ /= 1 + self.alpha * (1 - self.l1_ratio)
-            
-            if self.verbose and i % 10 == 0: 
-                print(f'[ElasticReg] iteration: {i}/{self.max_iter}')
-        
+
+            if self.verbose and i % 10 == 0:
+                print(f"[ElasticReg] iteration: {i}/{self.max_iter}")
+
         self._fitted = True
         return self
 
     def predict(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
-        if self.coef_ is None: raise ValueError()
+        if not self._fitted:
+            raise NotFittedError(self)
+        if self.coef_ is None:
+            raise ValueError()
         return X.dot(self.coef_)
-    
-    def score(self, X: Matrix, y: Matrix, 
-              metric: Evaluator = MeanSquaredError) -> float:
+
+    def score(
+        self, X: Matrix, y: Matrix, metric: Evaluator = MeanSquaredError
+    ) -> float:
         X_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=X_pred)
 
 
 class LinearRegressor(Estimator, Supervised):
-    
     """
-    An Ordinary Least Squares (OLS) Linear Regressor is a statistical method 
-    used in linear regression analysis. It estimates the coef_ of the 
-    linear equation, minimizing the sum of the squared differences between 
-    observed and predicted values. This results in a line of best fit through 
-    the data points in multidimensional space. OLS is widely used for its 
+    An Ordinary Least Squares (OLS) Linear Regressor is a statistical method
+    used in linear regression analysis. It estimates the coef_ of the
+    linear equation, minimizing the sum of the squared differences between
+    observed and predicted values. This results in a line of best fit through
+    the data points in multidimensional space. OLS is widely used for its
     simplicity and efficiency in modeling linear relationships.
     """
-    
+
     def __init__(self):
         self.coef_ = None
         self._fitted = False
 
-    def fit(self, X: Matrix, y: Matrix) -> 'LinearRegressor':
+    def fit(self, X: Matrix, y: Matrix) -> "LinearRegressor":
         X = np.hstack([np.ones((X.shape[0], 1)), X])
         X_T = np.transpose(X)
         self.coef_ = np.linalg.inv(X_T.dot(X)).dot(X_T).dot(y)
-        
+
         self._fitted = True
         return self
 
     def predict(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         X = np.hstack([np.ones((X.shape[0], 1)), X])
-        
+
         return X.dot(self.coef_)
-    
-    def score(self, X: Matrix, y: Matrix, 
-              metric: Evaluator = MeanSquaredError) -> float:
+
+    def score(
+        self, X: Matrix, y: Matrix, metric: Evaluator = MeanSquaredError
+    ) -> float:
         X_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=X_pred)
 
 
 class KernelRidgeRegressor(Estimator, Supervised):
-    
     """
-    Kernel Ridge Regression (KRR) combines ridge regression's linear coefficient 
-    penalization with kernel methods to handle non-linear data. By using a kernel 
-    function, KRR maps input data into a higher-dimensional feature space. In this 
-    transformed space, it minimizes the regularized loss function to find linear 
-    relationships. KRR excels in capturing complex, non-linear patterns in data, 
+    Kernel Ridge Regression (KRR) combines ridge regression's linear coefficient
+    penalization with kernel methods to handle non-linear data. By using a kernel
+    function, KRR maps input data into a higher-dimensional feature space. In this
+    transformed space, it minimizes the regularized loss function to find linear
+    relationships. KRR excels in capturing complex, non-linear patterns in data,
     making it versatile for various regression tasks.
-    
+
     Parameters
     ----------
     `alpha` : Regularization strength
     `deg` : Degree for `poly` kernel
     `gamma` : Scaling factor for `tanh`, `rbf`, and `laplacian` kernels
     `coef` : Base coefficient for `linear` and `poly` kernels
     `kernel` : Kernel functions
-    
+
     """
-    
-    def __init__(self, 
-                 alpha: float = 1.0,
-                 deg: int = 2,
-                 gamma: float = 1.0,
-                 coef: float = 1.0,
-                 kernel: KernelUtil.func_type = 'rbf') -> None:
+
+    def __init__(
+        self,
+        alpha: float = 1.0,
+        deg: int = 2,
+        gamma: float = 1.0,
+        coef: float = 1.0,
+        kernel: KernelUtil.FuncType = "rbf",
+    ) -> None:
         self.alpha = alpha
         self.deg = deg
         self.gamma = gamma
         self.coef = coef
         self.kernel = kernel
         self._X = None
         self._fitted = False
-        
+
         self.kernel_params = {
-            'alpha': self.alpha,
-            'gamma': self.gamma,
-            'deg': self.deg,
-            'coef': self.coef
+            "alpha": self.alpha,
+            "gamma": self.gamma,
+            "deg": self.deg,
+            "coef": self.coef,
         }
-    
-    def fit(self, X: Matrix, y: Vector) -> 'KernelRidgeRegressor':
+
+    def fit(self, X: Matrix, y: Vector) -> "KernelRidgeRegressor":
         m, _ = X.shape
         self._X = X
         self.ku_ = KernelUtil(self.kernel, **self.kernel_params)
-        
+
         K = self.ku_.kernel_func(X)
         self.alpha_mat = np.eye(m) * self.alpha
         self.dual_coef = np.linalg.inv(K + self.alpha_mat).dot(y)
-    
+
         self._fitted = True
         return self
-    
+
     def predict(self, X: Matrix) -> Vector:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         K = self.ku_.kernel_func(X, self._X)
-        
+
         return K.dot(self.dual_coef)
-    
-    def score(self, X: Matrix, y: Matrix, 
-              metric: Evaluator = MeanSquaredError) -> float:
+
+    def score(
+        self, X: Matrix, y: Matrix, metric: Evaluator = MeanSquaredError
+    ) -> float:
         X_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=X_pred)
 
 
 class BayesianRidgeRegressor(Estimator, Supervised):
-    
     """
-    Bayesian Ridge Regression applies Bayesian methods to linear models, 
-    estimating parameters with uncertainty. It automates regularization, 
-    balancing data fit and model simplicity. The approach provides both 
-    point estimates and confidence measures. It's effective for predictive 
+    Bayesian Ridge Regression applies Bayesian methods to linear models,
+    estimating parameters with uncertainty. It automates regularization,
+    balancing data fit and model simplicity. The approach provides both
+    point estimates and confidence measures. It's effective for predictive
     modeling with inherent uncertainty.
-    
+
     Parameters
     ----------
     `alpha_init` : Initial value for the precision of the distribution of noise
     `lambda_init` : Initial value for the precision of the distribution of weights
-    
+
     """
-    
-    def __init__(self, 
-                 alpha_init: float = None,
-                 lambda_init: float = None) -> None:
+
+    def __init__(self, alpha_init: float = None, lambda_init: float = None) -> None:
         self.alpha_init = alpha_init
         self.lambda_init = lambda_init
         self._fitted = False
-    
-    def fit(self, X: Matrix, y: Vector) -> 'BayesianRidgeRegressor':
-        if self.alpha_init is None: self.alpha_init = 1 / np.var(y)
-        if self.lambda_init is None: self.lambda_init = 1.0
-        
+
+    def fit(self, X: Matrix, y: Vector) -> "BayesianRidgeRegressor":
+        if self.alpha_init is None:
+            self.alpha_init = 1 / np.var(y)
+        if self.lambda_init is None:
+            self.lambda_init = 1.0
+
         m, n = X.shape
         X = np.column_stack((np.ones(m), X))
         A = np.eye(n + 1) * self.alpha_init
-        
+
         sigma_inv = A + self.lambda_init * X.T.dot(X)
         sigma = np.linalg.inv(sigma_inv)
         mu = self.lambda_init * sigma.dot(X.T).dot(y)
-        
+
         self.coef_ = mu
         self.sigma_ = sigma
-        
+
         self._fitted = True
         return self
-    
+
     def predict(self, X: Matrix) -> Vector:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         X = np.column_stack((np.ones(X.shape[0]), X))
         return X.dot(self.coef_)
-    
-    def score(self, X: Matrix, y: Matrix, 
-              metric: Evaluator = MeanSquaredError) -> float:
+
+    def score(
+        self, X: Matrix, y: Matrix, metric: Evaluator = MeanSquaredError
+    ) -> float:
         X_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=X_pred)
-
```

### Comparing `luma-ml-0.6.4/luma/regressor/neighbors.py` & `luma-ml-0.6.5/luma/regressor/neighbors.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,173 +4,173 @@
 from luma.interface.util import Matrix
 from luma.core.super import Estimator, Supervised, Evaluator
 from luma.interface.util import NearestNeighbors
 from luma.interface.exception import NotFittedError
 from luma.metric.regression import MeanSquaredError
 
 
-__all__ = (
-    'KNNRegressor', 
-    'AdaptiveKNNRegressor', 
-    'WeightedKNNRegressor'
-)
+__all__ = ("KNNRegressor", "AdaptiveKNNRegressor", "WeightedKNNRegressor")
 
 
 class KNNRegressor(Estimator, Supervised):
-     
     """
-    The K-Nearest Neighbors (KNN) regressor is a straightforward and 
-    intuitive machine learning algorithm that predicts the value of 
-    a new data point based on the average values of its closest 
-    neighbors. It functions by calculating the distance (such as 
-    Euclidean distance) between the new point and all points in the 
-    training set, determining the 'k' nearest neighbors, and then 
-    averaging the values of these neighbors to predict the continuous 
+    The K-Nearest Neighbors (KNN) regressor is a straightforward and
+    intuitive machine learning algorithm that predicts the value of
+    a new data point based on the average values of its closest
+    neighbors. It functions by calculating the distance (such as
+    Euclidean distance) between the new point and all points in the
+    training set, determining the 'k' nearest neighbors, and then
+    averaging the values of these neighbors to predict the continuous
     output.
-    
+
     Parameters
     ----------
     `n_neighbors` : Number of neighbors to be considered close
-    
+
     """
-    
+
     def __init__(self, n_neighbors: int = 5):
         self.n_neighbors = n_neighbors
         self._neighbors = None
         self._y = None
         self._fitted = False
 
-    def fit(self, X: Matrix, y: Matrix) -> 'KNNRegressor':
+    def fit(self, X: Matrix, y: Matrix) -> "KNNRegressor":
         self._neighbors = NearestNeighbors(X, self.n_neighbors)
         self._y = y
         self._fitted = True
         return self
 
     def predict(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         predictions = []
 
         for point in X:
             distances = np.linalg.norm(self._neighbors.data - point, axis=1)
-            nearest_neighbor_ids = np.argsort(distances)[:self.n_neighbors]
+            nearest_neighbor_ids = np.argsort(distances)[: self.n_neighbors]
             nearest_neighbor_values = self._y[nearest_neighbor_ids]
             average_value = np.mean(nearest_neighbor_values)
             predictions.append(average_value)
 
         return Matrix(predictions)
-    
-    def score(self, X: Matrix, y: Matrix, 
-              metric: Evaluator = MeanSquaredError) -> float:
+
+    def score(
+        self, X: Matrix, y: Matrix, metric: Evaluator = MeanSquaredError
+    ) -> float:
         X_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=X_pred)
 
 
 class AdaptiveKNNRegressor(Estimator, Supervised):
-    
     """
-    The Adaptive K-Nearest Neighbors (AdaKNN) Regressor is an enhanced version 
-    of the traditional KNN algorithm for regression. It predicts the value of a 
-    new data point based on the average values of its neighbors, where the 
-    number of neighbors (k) is adaptively determined based on the local density 
-    of the training data. This method allows the algorithm to be more flexible 
+    The Adaptive K-Nearest Neighbors (AdaKNN) Regressor is an enhanced version
+    of the traditional KNN algorithm for regression. It predicts the value of a
+    new data point based on the average values of its neighbors, where the
+    number of neighbors (k) is adaptively determined based on the local density
+    of the training data. This method allows the algorithm to be more flexible
     and effective, particularly in datasets with varying densities.
 
     Parameters
     ----------
     `n_density` : Number of nearest neighbors to estimate the local density
     `min_neighbors` : Minimum number of neighbors to be considered for averaging
     `max_neighbors` : Maximum number of neighbors to be considered
 
     """
-    
-    def __init__(self, 
-                 n_density: int = 10, 
-                 min_neighbors: int = 5, 
-                 max_neighbors: int = 20):
+
+    def __init__(
+        self, n_density: int = 10, min_neighbors: int = 5, max_neighbors: int = 20
+    ):
         self.n_density = n_density
         self.min_neighbors = min_neighbors
         self.max_neighbors = max_neighbors
         self._X = None
         self._y = None
         self._fitted = False
 
-    def fit(self, X: Matrix, y: Matrix) -> 'AdaptiveKNNRegressor':
+    def fit(self, X: Matrix, y: Matrix) -> "AdaptiveKNNRegressor":
         self._X = X
         self._y = y
         self.dist_matrix = distance_matrix(X, X)
         self.local_density = np.sort(self.dist_matrix, axis=1)
         self.local_density = self.local_density[:, self.n_density]
-        
+
         self._fitted = True
         return self
 
     def predict(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         dist_matrix = distance_matrix(X, self._X)
-        k_values = np.clip(np.ceil(self.max_neighbors / self.local_density), 
-                           self.min_neighbors, self.max_neighbors).astype(int)
-        
+        k_values = np.clip(
+            np.ceil(self.max_neighbors / self.local_density),
+            self.min_neighbors,
+            self.max_neighbors,
+        ).astype(int)
+
         predictions = []
         for point_distances in dist_matrix:
             nearest_indices = np.argsort(point_distances)
             adaptive_neighbors = min(len(nearest_indices), k_values[nearest_indices[0]])
             nearest_indices = nearest_indices[:adaptive_neighbors]
 
             average_value = np.mean(self._y[nearest_indices])
             predictions.append(average_value)
 
         return Matrix(predictions)
 
-    def score(self, X: Matrix, y: Matrix, 
-              metric: Evaluator = MeanSquaredError) -> float:
+    def score(
+        self, X: Matrix, y: Matrix, metric: Evaluator = MeanSquaredError
+    ) -> float:
         X_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=X_pred)
 
 
 class WeightedKNNRegressor(Estimator, Supervised):
-    
     """
     The Weighted KNN Regressor is an adaptation of the k-Nearest Neighbors algorithm
     tailored for regression tasks, where neighbors influence the predicted value
     based on their distance from the query point. Closer neighbors exert greater
     influence due to higher weights, commonly calculated using inverse distance weighting.
     This method improves prediction precision, particularly in datasets with
     irregular distributions.
-    
+
     Parameters
     ----------
     `n_neighbors` : Number of neighbors to be considered close
-    
+
     """
-    
+
     def __init__(self, n_neighbors: int = 5):
         self.n_neighbors = n_neighbors
         self._X = None
         self._y = None
         self._fitted = False
 
-    def fit(self, X: Matrix, y: Matrix) -> 'WeightedKNNRegressor':
+    def fit(self, X: Matrix, y: Matrix) -> "WeightedKNNRegressor":
         self._X = X
         self._y = y
-        
+
         self._fitted = True
         return self
 
     def predict(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise not NotFittedError(self)
+        if not self._fitted:
+            raise not NotFittedError(self)
         predictions = np.zeros(X.shape[0])
         for i, x in enumerate(X):
             distances = np.linalg.norm(self._X - x, axis=1)
-            nearest_neighbors = np.argsort(distances)[:self.n_neighbors]
+            nearest_neighbors = np.argsort(distances)[: self.n_neighbors]
 
             weights = 1 / (distances[nearest_neighbors] + 1e-5)
             weighted_sum = np.dot(weights, self._y[nearest_neighbors])
             total_weight = np.sum(weights)
             predictions[i] = weighted_sum / total_weight
 
         return predictions
 
-    def score(self, X: Matrix, y: Matrix, 
-              metric: Evaluator = MeanSquaredError) -> float:
+    def score(
+        self, X: Matrix, y: Matrix, metric: Evaluator = MeanSquaredError
+    ) -> float:
         X_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=X_pred)
-
```

### Comparing `luma-ml-0.6.4/luma/regressor/poly.py` & `luma-ml-0.6.5/luma/regressor/poly.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,76 +3,76 @@
 
 from luma.interface.util import Matrix
 from luma.interface.exception import NotFittedError
 from luma.core.super import Estimator, Evaluator
 from luma.metric.regression import MeanSquaredError
 
 
-__all__ = (
-    'PolynomialRegressor'
-)
+__all__ = "PolynomialRegressor"
 
 
 class PolynomialRegressor(Estimator):
-    
     """
     Polynomial regression is a type of regression analysis used
-    in statistics and machine learning to model the relationship between 
+    in statistics and machine learning to model the relationship between
     a dependent variable and one or more independent variables.
-    
+
     Parameters
     ----------
     `deg` : Degree of a polynomial function
     `alpha` : Regularization strength
     `l1_ratio` : Balancing parameter between `l1` and `l2`
     `regularization` : Regularization type (e.g. `l1`, `l2`, `elastic-net`)
-    
+
     """
-    
-    def __init__(self, 
-                 deg: int = 2,
-                 alpha: float = 0.01,
-                 l1_ratio: float = 0.5,
-                 regularization: Literal['l1', 'l2', 'elastic-net'] = None) -> None:
+
+    def __init__(
+        self,
+        deg: int = 2,
+        alpha: float = 0.01,
+        l1_ratio: float = 0.5,
+        regularization: Literal["l1", "l2", "elastic-net"] = None,
+    ) -> None:
         self.deg = deg
         self.alpha = alpha
         self.l1_ratio = l1_ratio
         self.regularization = regularization
         self._fitted = False
 
     def _generate_polynomial_features(self, X):
         X_poly = X.copy()
         for d in range(2, self.deg + 1):
-            X_poly = np.hstack((X_poly, X ** d))
+            X_poly = np.hstack((X_poly, X**d))
         return X_poly
 
-    def fit(self, X: Matrix, y: Matrix) -> 'PolynomialRegressor':
+    def fit(self, X: Matrix, y: Matrix) -> "PolynomialRegressor":
         X_poly = self._generate_polynomial_features(X)
         reg_matrix = self._regularization_matrix(X_poly.shape[1])
         augmented_matrix = np.vstack([X_poly, np.sqrt(self.alpha) * reg_matrix])
         augmented_target = np.hstack([y, np.zeros(X_poly.shape[1])])
         self.coef_ = np.linalg.lstsq(augmented_matrix, augmented_target, rcond=None)[0]
         self._fitted = True
         return self
 
     def _regularization_matrix(self, n: int) -> Matrix:
-        if self.regularization == 'l2':
+        if self.regularization == "l2":
             return self.alpha * np.eye(n)
-        elif self.regularization == 'l1':
+        elif self.regularization == "l1":
             return self.alpha * np.sign(np.random.randn(n, n))
-        elif self.regularization == 'elastic-net':
+        elif self.regularization == "elastic-net":
             l1_mat = self.alpha * self.l1_ratio * np.sign(np.random.randn(n, n))
             l2_mat = self.alpha * (1 - self.l1_ratio) * np.eye(n)
             return l1_mat + l2_mat
         else:
             return np.zeros((n, n))
-    
+
     def predict(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         X_poly = self._generate_polynomial_features(X)
         return np.dot(X_poly, self.coef_)
 
-    def score(self, X: Matrix, y: Matrix, 
-              metric: Evaluator = MeanSquaredError) -> float:
+    def score(
+        self, X: Matrix, y: Matrix, metric: Evaluator = MeanSquaredError
+    ) -> float:
         X_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=X_pred)
-
```

### Comparing `luma-ml-0.6.4/luma/regressor/robust.py` & `luma-ml-0.6.5/luma/regressor/robust.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,276 +4,290 @@
 from luma.core.super import Estimator, Evaluator, Supervised
 from luma.interface.util import Matrix, Vector
 from luma.interface.exception import NotFittedError
 from luma.metric.regression import MeanSquaredError
 from luma.regressor.linear import LinearRegressor
 
 
-__all__ = (
-    'RANSAC',
-    'MLESAC'
-)
+__all__ = ("RANSAC", "MLESAC")
 
 
 class RANSAC(Estimator, Supervised):
-    
     """
-    RANSAC (Random Sample Consensus) is an iterative algorithm used for robust 
-    estimation of parameters from a set of data containing outliers. It works by 
-    randomly selecting a subset of the original data and fitting a model to this 
-    subset. The algorithm then tests all other data points against this model, 
-    classifying them as inliers or outliers based on a predefined threshold. 
-    This process is repeated multiple times, each time selecting a different 
-    subset. The best model is chosen based on the maximum number of inliers 
+    RANSAC (Random Sample Consensus) is an iterative algorithm used for robust
+    estimation of parameters from a set of data containing outliers. It works by
+    randomly selecting a subset of the original data and fitting a model to this
+    subset. The algorithm then tests all other data points against this model,
+    classifying them as inliers or outliers based on a predefined threshold.
+    This process is repeated multiple times, each time selecting a different
+    subset. The best model is chosen based on the maximum number of inliers
     it includes.
-    
+
     Parameters
     ----------
     `estimator` : Regression estimator (Default `LinearRegressor()`)
     `min_points` : Mininum sample size for each random sample
     `max_iter` : Maximum iteration
     `min_inliers` : Minimum number of inliers for a model to be considered valid
     `threshold` : Maximum distance a point can have to be considered an inlier
     `random_state` : Seed for random sampling the data
-    
+
     Properties
     ----------
     Get best estimator:
     ```py
         @property
         def best_estimator(self) -> Estimator
     ```
     """
-    
-    def __init__(self, 
-                 estimator: Estimator = LinearRegressor(),
-                 min_points: int | float = 2,
-                 max_iter: int = 1000,
-                 min_inliers: int | float = 0.5,
-                 threshold: float = None,
-                 random_state: int = None,
-                 verbose: bool = False) -> None:
+
+    def __init__(
+        self,
+        estimator: Estimator = LinearRegressor(),
+        min_points: int | float = 2,
+        max_iter: int = 1000,
+        min_inliers: int | float = 0.5,
+        threshold: float = None,
+        random_state: int = None,
+        verbose: bool = False,
+    ) -> None:
         self.estimator = estimator
         self.min_points = min_points
         self.max_iter = max_iter
         self.min_inliers = min_inliers
         self.threshold = threshold
         self.random_state = random_state
         self.verbose = verbose
         self.inliers_ = None
         self._fitted = False
-    
-    def fit(self, X: Matrix, y: Vector) -> 'RANSAC':
+
+    def fit(self, X: Matrix, y: Vector) -> "RANSAC":
         m, _ = X.shape
         best_err = np.inf
         best_indices = None
-        
+
         np.random.seed(self.random_state)
         Xy = np.hstack((X, y.reshape(-1, 1)))
-        
-        if self.min_points < 1: self.min_points = np.ceil(m * self.min_points)
-        if self.min_inliers < 1: self.min_inliers = np.ceil(m * self.min_inliers)
-        if self.threshold is None: self.threshold = self._mean_absdev(y)
-        
+
+        if self.min_points < 1:
+            self.min_points = np.ceil(m * self.min_points)
+        if self.min_inliers < 1:
+            self.min_inliers = np.ceil(m * self.min_inliers)
+        if self.threshold is None:
+            self.threshold = self._mean_absdev(y)
+
         for i in range(self.max_iter):
             hypo_indices, test_indices = self._random_partition(X)
             hypo_inliers = Xy[hypo_indices]
             test_points = Xy[test_indices]
-            
+
             self.estimator.fit(hypo_inliers[:, :-1], hypo_inliers[:, -1])
             test_err = self._error(test_points[:, :-1], test_points[:, -1])
-            
+
             true_indices = test_indices[test_err < self.threshold]
             true_inliers = Xy[true_indices]
-            
+
             if len(true_inliers) > self.min_inliers:
                 Xy_better = np.concatenate((hypo_inliers, true_inliers))
-                
+
                 self.estimator.fit(Xy_better[:, :-1], Xy_better[:, -1])
                 better_err = self._error(Xy_better[:, :-1], Xy_better[:, -1])
                 this_err = np.mean(better_err)
-                
+
                 if this_err < best_err:
                     best_err = this_err
                     best_indices = np.concatenate((hypo_indices, true_indices))
-            
+
             if self.verbose and i % 100 == 0:
-                print(f'[RANSAC] Iteration {i}/{self.max_iter}',
-                      f'with current best-error: {best_err}')
-        
+                print(
+                    f"[RANSAC] Iteration {i}/{self.max_iter}",
+                    f"with current best-error: {best_err}",
+                )
+
         self.inliers_ = Xy[best_indices, :-1]
         self._fitted = True
         return self
-    
+
     def _random_partition(self, X: Matrix) -> Tuple[Vector, Vector]:
         all_indices = np.arange(X.shape[0])
         np.random.shuffle(all_indices)
-        indices_l = all_indices[:self.min_points]
-        indices_r = all_indices[self.min_points:]
-        
+        indices_l = all_indices[: self.min_points]
+        indices_r = all_indices[self.min_points :]
+
         return indices_l, indices_r
 
     def _error(self, X: Matrix, y: Vector) -> Vector:
         y_pred = self.estimator.predict(X)
         return np.abs(y - y_pred)
-    
+
     def _mean_absdev(self, y: Vector) -> float:
         y_median = np.median(y)
         abs_dev = np.abs(y - y_median)
         mad = np.median(abs_dev)
         return mad
-    
+
     @property
     def best_estimator(self) -> Estimator:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         return self.estimator
-    
+
     def predict(self, X: Matrix) -> Vector:
         best = self.best_estimator
         return best.predict(X)
 
-    def score(self, X: Matrix, y: Matrix, 
-              metric: Evaluator = MeanSquaredError) -> float:
+    def score(
+        self, X: Matrix, y: Matrix, metric: Evaluator = MeanSquaredError
+    ) -> float:
         X_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=X_pred)
 
 
 class MLESAC(Estimator, Supervised):
-    
     """
-    MLESAC (Maximum Likelihood Estimation SAmple Consensus) is an iterative algorithm 
-    used for robust estimation of parameters from a set of data containing outliers. 
-    Unlike RANSAC which focuses on maximizing the number of inliers, MLESAC seeks 
-    to maximize the likelihood of the model given the data, considering both the 
+    MLESAC (Maximum Likelihood Estimation SAmple Consensus) is an iterative algorithm
+    used for robust estimation of parameters from a set of data containing outliers.
+    Unlike RANSAC which focuses on maximizing the number of inliers, MLESAC seeks
+    to maximize the likelihood of the model given the data, considering both the
     number of inliers and the quality of the fit.
-    
+
     Parameters
     ----------
     `estimator` : Regression estimator (Default `LinearRegressor()`)
     `min_points` : Minimum sample size for each random sample
     `max_iter` : Maximum number of iterations
     `min_inliers` : Minimum number of inliers for a model to be considered valid
     `threshold` : Maximum distance a point can have to be considered an inlier
     `random_state` : Seed for random sampling the data
-    
+
     Properties
     ----------
     Get best estimator:
     ```py
         @property
         def best_estimator(self) -> Estimator
     ```
-    
+
     Notes
     -----
     * `MLESAC` assumes that inliers follow a multivariate Gaussian model
-    
+
     """
-    
-    def __init__(self, 
-                 estimator: Estimator = LinearRegressor(),
-                 min_points: int | float = 2,
-                 max_iter: int = 1000,
-                 min_inliers: int | float = 0.5,
-                 threshold: float = None,
-                 random_state: int = None,
-                 verbose: bool = False) -> None:
+
+    def __init__(
+        self,
+        estimator: Estimator = LinearRegressor(),
+        min_points: int | float = 2,
+        max_iter: int = 1000,
+        min_inliers: int | float = 0.5,
+        threshold: float = None,
+        random_state: int = None,
+        verbose: bool = False,
+    ) -> None:
         self.estimator = estimator
         self.min_points = min_points
         self.max_iter = max_iter
         self.min_inliers = min_inliers
         self.threshold = threshold
         self.random_state = random_state
         self.verbose = verbose
         self.inliers_ = None
         self._fitted = False
-    
-    def fit(self, X: Matrix, y: Vector) -> 'MLESAC':
+
+    def fit(self, X: Matrix, y: Vector) -> "MLESAC":
         m, _ = X.shape
         best_likelihood = -np.inf
         best_indices = None
-        
+
         np.random.seed(self.random_state)
         Xy = np.hstack((X, y.reshape(-1, 1)))
-        
-        if self.min_points < 1: self.min_points = np.ceil(m * self.min_points)
-        if self.min_inliers < 1: self.min_inliers = np.ceil(m * self.min_inliers)
-        if self.threshold is None: self.threshold = self._mean_absdev(y)
-        
+
+        if self.min_points < 1:
+            self.min_points = np.ceil(m * self.min_points)
+        if self.min_inliers < 1:
+            self.min_inliers = np.ceil(m * self.min_inliers)
+        if self.threshold is None:
+            self.threshold = self._mean_absdev(y)
+
         for i in range(self.max_iter):
             hypo_indices, test_indices = self._random_partition(X)
             hypo_inliers = Xy[hypo_indices]
             test_points = Xy[test_indices]
-            
+
             self.estimator.fit(hypo_inliers[:, :-1], hypo_inliers[:, -1])
             test_err = self._error(test_points[:, :-1], test_points[:, -1])
-            
+
             true_indices = test_indices[test_err < self.threshold]
             true_inliers = Xy[true_indices]
-            
+
             if len(true_inliers) >= self.min_inliers:
                 Xy_better = np.concatenate((hypo_inliers, true_inliers))
-                
+
                 self.estimator.fit(Xy_better[:, :-1], Xy_better[:, -1])
                 better_err = self._error(Xy_better[:, :-1], Xy_better[:, -1])
                 likelihood = self._calculate_likelihood(better_err)
-                
+
                 if likelihood > best_likelihood:
                     best_likelihood = likelihood
                     best_indices = np.concatenate((hypo_indices, true_indices))
 
             if self.verbose and i % 100 == 0:
-                print(f'[MLESAC] Iteration {i}/{self.max_iter}',
-                      f'with current best-likelihood: {best_likelihood}')
+                print(
+                    f"[MLESAC] Iteration {i}/{self.max_iter}",
+                    f"with current best-likelihood: {best_likelihood}",
+                )
 
         self.inliers_ = Xy[best_indices, :-1]
         self._fitted = True
         return self
-    
+
     def _random_partition(self, X: Matrix) -> Tuple[Vector, Vector]:
         all_indices = np.arange(X.shape[0])
         np.random.shuffle(all_indices)
-        indices_l = all_indices[:self.min_points]
-        indices_r = all_indices[self.min_points:]
-        
+        indices_l = all_indices[: self.min_points]
+        indices_r = all_indices[self.min_points :]
+
         return indices_l, indices_r
 
     def _error(self, X: Matrix, y: Vector) -> Vector:
         y_pred = self.estimator.predict(X)
         return np.abs(y - y_pred)
-    
+
     def _mean_absdev(self, y: Vector) -> float:
         y_median = np.median(y)
         abs_dev = np.abs(y - y_median)
         mad = np.median(abs_dev)
         return mad
-    
+
     def _calculate_likelihood(self, error: Vector) -> float:
-        if error.ndim == 1: error = error[:, np.newaxis]
+        if error.ndim == 1:
+            error = error[:, np.newaxis]
         m, n = error.shape
         cov_matrix = np.cov(error, rowvar=False)
-        
-        if n == 1: cov_matrix = cov_matrix.reshape(1, 1)
+
+        if n == 1:
+            cov_matrix = cov_matrix.reshape(1, 1)
         det_cov_matrix = np.linalg.det(cov_matrix)
         inv_cov_matrix = np.linalg.inv(cov_matrix)
 
         likelihood = -m * n * np.log(2 * np.pi) / 2
         likelihood -= m * np.log(det_cov_matrix) / 2
         for error in error:
             likelihood -= 0.5 * np.dot(error, np.dot(inv_cov_matrix, error))
 
         return likelihood
-    
+
     @property
     def best_estimator(self) -> Estimator:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         return self.estimator
-    
+
     def predict(self, X: Matrix) -> Vector:
         best = self.best_estimator
         return best.predict(X)
 
-    def score(self, X: Matrix, y: Matrix, 
-              metric: Evaluator = MeanSquaredError) -> float:
+    def score(
+        self, X: Matrix, y: Matrix, metric: Evaluator = MeanSquaredError
+    ) -> float:
         X_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=X_pred)
-
```

### Comparing `luma-ml-0.6.4/luma/regressor/svm.py` & `luma-ml-0.6.5/luma/regressor/svm.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,186 +2,194 @@
 
 from luma.interface.util import Matrix, KernelUtil
 from luma.interface.exception import NotFittedError, UnsupportedParameterError
 from luma.core.super import Estimator, Evaluator, Supervised
 from luma.metric.regression import MeanSquaredError
 
 
-__all__ = (
-    'SVR', 
-    'KernelSVR'
-)
+__all__ = ("SVR", "KernelSVR")
 
 
 class SVR(Estimator, Supervised):
-    
     """
-    Support Vector Regressor (SVR) is a supervised machine learning 
-    algorithm used for regression tasks. It operates by determining a 
-    hyperplane that best fits the input data, aiming to minimize the 
+    Support Vector Regressor (SVR) is a supervised machine learning
+    algorithm used for regression tasks. It operates by determining a
+    hyperplane that best fits the input data, aiming to minimize the
     difference between the predicted and actual values.
-    
+
     Parameters
     ----------
     `C` : Regularization parameter
     `epsilon` : Epsilon-tube in the training loss function
     `batch_size` : Size of a single batch
     `learning_rate` : Step-size of gradient descent update
     `max_iter` : Number of iteration
-    
+
     """
-    
-    def __init__(self, 
-                 C: float = 1.0, 
-                 epsilon: float = 0.1,
-                 batch_size: int = 100, 
-                 learning_rate: float = 0.001, 
-                 max_iter: int = 1000, 
-                 verbose: bool = False) -> None:
+
+    def __init__(
+        self,
+        C: float = 1.0,
+        epsilon: float = 0.1,
+        batch_size: int = 100,
+        learning_rate: float = 0.001,
+        max_iter: int = 1000,
+        verbose: bool = False,
+    ) -> None:
         self.C = C
         self.epsilon = epsilon
         self.batch_size = batch_size
         self.learning_rate = learning_rate
         self.max_iter = max_iter
         self.verbose = verbose
         self._fitted = False
 
-    def fit(self, X: Matrix, y: Matrix) -> 'SVR':
+    def fit(self, X: Matrix, y: Matrix) -> "SVR":
         m, n = X.shape
         id = np.arange(m)
         np.random.shuffle(id)
 
         self.bias = 0.0
         self.weight = np.zeros(n)
-        
+
         for i in range(self.max_iter):
             for batch_point in range(0, m, self.batch_size):
                 gradient_w, gradient_b = 0, 0
                 for j in range(batch_point, batch_point + self.batch_size):
-                    if j >= m: continue
+                    if j >= m:
+                        continue
                     idx = id[j]
                     pred = np.dot(self.weight, X[idx].T) + self.bias
                     loss = pred - y[idx]
-                    
+
                     if np.abs(loss) > self.epsilon:
                         gradient_w += self.C * np.sign(loss) * X[idx]
                         gradient_b += self.C * np.sign(loss)
 
                 self.weight -= self.learning_rate * self.weight
                 self.weight -= self.learning_rate * gradient_w
                 self.bias -= self.learning_rate * gradient_b
 
             if self.verbose and i % 100 == 0 and i:
-                print(f'[SVR] Finished iteration {i}/{self.max_iter}', end=' ')
-                print(f'with weight-norm of {np.linalg.norm(self.weight)}')
+                print(f"[SVR] Finished iteration {i}/{self.max_iter}", end=" ")
+                print(f"with weight-norm of {np.linalg.norm(self.weight)}")
 
         self._fitted = True
         return self
-    
+
     def predict(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         return np.dot(X, self.weight) + self.bias
 
-    def score(self, X: Matrix, y: Matrix, 
-              metric: Evaluator = MeanSquaredError) -> float:
+    def score(
+        self, X: Matrix, y: Matrix, metric: Evaluator = MeanSquaredError
+    ) -> float:
         X_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=X_pred)
 
 
 class KernelSVR(Estimator, Supervised):
-    
     """
-    Kernel Support Vector Regression (KernelSVR) is an extension of the 
-    Support Vector Regression (SVR) algorithm that enables regression on 
+    Kernel Support Vector Regression (KernelSVR) is an extension of the
+    Support Vector Regression (SVR) algorithm that enables regression on
     non-linearly related data by mapping it into a higher-dimensional space
-    using a kernel function. The kernel function allows the algorithm to 
+    using a kernel function. The kernel function allows the algorithm to
     establish a flexible and non-linear regression model in the transformed space.
 
     Parameters
     ----------
     `C` : Regularization parameter
     `deg` : Polynomial Degree for `poly` kernel
     `gamma` : Shape parameter of Gaussian curve for `rbf` kernel
     `coef` : Coefficient for `poly`, `sigmoid` kernel
     `learning_rate` : Step-size for gradient descent update
     `max_iter` : Number of iteration
     `kernel` : Type of kernel (e.g., `linear`, `poly`, `rbf`, `sigmoid`)
 
     """
-    
-    def __init__(self,
-                 C: float = 1.0,
-                 deg: int = 3,
-                 gamma: float = 1.0,
-                 coef: float = 1.0,
-                 learning_rate: float = 0.001,
-                 max_iter: int = 1000,
-                 kernel: KernelUtil.func_type = 'rbf',
-                 verbose: bool = False) -> None:
+
+    def __init__(
+        self,
+        C: float = 1.0,
+        deg: int = 3,
+        gamma: float = 1.0,
+        coef: float = 1.0,
+        learning_rate: float = 0.001,
+        max_iter: int = 1000,
+        kernel: KernelUtil.FuncType = "rbf",
+        verbose: bool = False,
+    ) -> None:
         self.C = C
         self.deg = deg
         self.gamma = gamma
         self.coef = coef
         self.learning_rate = learning_rate
         self.max_iter = max_iter
         self.kernel = kernel
         self.verbose = verbose
         self._kernel_func = None
         self._fitted = False
 
-    def fit(self, X: Matrix, y: Matrix) -> 'KernelSVR':
+    def fit(self, X: Matrix, y: Matrix) -> "KernelSVR":
         m, _ = X.shape
         self._set_kernel_func()
         self.alpha = np.random.random(m)
         self.bias = 0
-        
+
         y_mul_kernel = np.outer(y, y) * self._kernel_func(X, X)
         for i in range(self.max_iter):
             gradient = np.ones(m) - y_mul_kernel.dot(self.alpha)
             self.alpha += self.learning_rate * gradient
             self.alpha = np.clip(self.alpha, 0, self.C)
-            
+
             if self.verbose and i % 100 == 0 and i:
-                print(f'[KernelSVR] Finished iteration {i}/{self.max_iter}', end=' ')
-                print(f'with alpha-norm: {np.linalg.norm(self.alpha)}')
-        
+                print(f"[KernelSVR] Finished iteration {i}/{self.max_iter}", end=" ")
+                print(f"with alpha-norm: {np.linalg.norm(self.alpha)}")
+
         alpha_idx = np.where((self.alpha > 0) & (self.alpha < self.C))[0]
         bias_list = []
         for idx in alpha_idx:
             _append = y[idx] - (self.alpha * y).dot(self._kernel_func(X, X[idx]))
             bias_list.append(_append)
         self.bias = np.mean(bias_list)
-        
+
         self._X = X
         self._y = y
         self._fitted = True
         return self
-    
+
     def _linear_kernel(self, xi: Matrix, xj: Matrix) -> Matrix:
         return xi.dot(xj.T)
 
     def _poly_kernel(self, xi: Matrix, xj: Matrix) -> Matrix:
         return (self.coef + xi.dot(xj.T)) ** self.deg
 
     def _rbf_kernel(self, xi: Matrix, xj: Matrix) -> Matrix:
         norm = np.linalg.norm(xi[:, np.newaxis] - xj[np.newaxis, :], axis=2)
-        return np.exp(-self.gamma * norm ** 2)
+        return np.exp(-self.gamma * norm**2)
 
     def _sigmoid_kernel(self, xi: Matrix, xj: Matrix) -> Matrix:
         return np.tanh(2 * xi.dot(xj.T) + self.coef)
 
     def _set_kernel_func(self) -> None:
-        if self.kernel == 'linear': self._kernel_func = self._linear_kernel
-        elif self.kernel == 'poly': self._kernel_func = self._poly_kernel
-        elif self.kernel == 'rbf': self._kernel_func = self._rbf_kernel
-        elif self.kernel == 'sigmoid': self._kernel_func = self._sigmoid_kernel
-        else: raise UnsupportedParameterError(self.kernel)
+        if self.kernel == "linear":
+            self._kernel_func = self._linear_kernel
+        elif self.kernel == "poly":
+            self._kernel_func = self._poly_kernel
+        elif self.kernel == "rbf":
+            self._kernel_func = self._rbf_kernel
+        elif self.kernel == "sigmoid":
+            self._kernel_func = self._sigmoid_kernel
+        else:
+            raise UnsupportedParameterError(self.kernel)
 
     def predict(self, X: Matrix) -> Matrix:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         return (self.alpha * self._y).dot(self._kernel_func(self._X, X)) + self.bias
-    
-    def score(self, X: Matrix, y: Matrix, 
-              metric: Evaluator = MeanSquaredError) -> float:
+
+    def score(
+        self, X: Matrix, y: Matrix, metric: Evaluator = MeanSquaredError
+    ) -> float:
         X_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=X_pred)
-
```

### Comparing `luma-ml-0.6.4/luma/regressor/tree.py` & `luma-ml-0.6.5/luma/regressor/tree.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,172 +4,185 @@
 from luma.interface.util import Matrix, Vector
 from luma.interface.exception import NotFittedError
 from luma.core.super import Estimator, Evaluator, Supervised
 from luma.interface.util import DecisionTreeNode
 from luma.metric.regression import MeanSquaredError
 
 
-__all__ = (
-    'DecisionTreeRegressor',
-)
+__all__ = ("DecisionTreeRegressor",)
 
 
 class DecisionTreeRegressor(Estimator, Supervised):
-    
     """
-    A Decision Tree Regressor is a machine learning algorithm used for 
-    predicting continuous values, unlike its counterpart, the Decision 
-    Tree Classifier, which is used for predicting categorical outcomes. 
-    The regressor works by splitting the data into distinct regions based 
-    on feature values. At each node of the tree, it chooses the split 
-    that minimizes the variance (or another specified criterion) of the 
+    A Decision Tree Regressor is a machine learning algorithm used for
+    predicting continuous values, unlike its counterpart, the Decision
+    Tree Classifier, which is used for predicting categorical outcomes.
+    The regressor works by splitting the data into distinct regions based
+    on feature values. At each node of the tree, it chooses the split
+    that minimizes the variance (or another specified criterion) of the
     target variable within the regions created by the split.
-    
+
     Parameters
     ----------
     `max_depth` : Maximum depth of the tree
     `criterion` : Function used to measure the quality of a split
     `min_samples_split` : Minimum samples required to split a node
     `min_samples_leaf` : Minimum samples required to be at a leaf node
     `max_features` : Number of features to consider
     `min_variance_decrease` : Minimum decrement of variance for a split
     `max_leaf_nodes` : Maximum amount of leaf nodes
     `random_state` : The randomness seed of the estimator
-    
+
     """
-    
-    def __init__(self, 
-                 max_depth: int = 10, 
-                 min_samples_split: int = 2,
-                 min_samples_leaf: int = 1, 
-                 max_features: int = None, 
-                 min_variance_decrease: float = 0.0,
-                 max_leaf_nodes: int = None,
-                 random_state: int = None) -> None:
+
+    def __init__(
+        self,
+        max_depth: int = 10,
+        min_samples_split: int = 2,
+        min_samples_leaf: int = 1,
+        max_features: int = None,
+        min_variance_decrease: float = 0.0,
+        max_leaf_nodes: int = None,
+        random_state: int = None,
+    ) -> None:
         self.max_depth = max_depth
         self.min_samples_split = min_samples_split
         self.min_samples_leaf = min_samples_leaf
         self.max_features = max_features
         self.min_variance_decrease = min_variance_decrease
         self.max_leaf_nodes = max_leaf_nodes
         self.random_state = random_state
         self.root = None
         self._fitted = False
-    
-    def fit(self, 
-            X: Matrix, 
-            y: Vector, 
-            sample_weights: Vector = None) -> 'DecisionTreeRegressor':
-        if sample_weights is None: sample_weights = np.ones(len(y))
+
+    def fit(
+        self, X: Matrix, y: Vector, sample_weights: Vector = None
+    ) -> "DecisionTreeRegressor":
+        if sample_weights is None:
+            sample_weights = np.ones(len(y))
         sample_weights = Vector(sample_weights)
         np.random.seed(self.random_state)
-        
+
         self.root = self._build_tree(X, y, 0, sample_weights)
         self._fitted = True
         return self
-    
+
     def _stopping_criteria(self, y: Vector, depth: int) -> bool:
-        if len(y) <= self.min_samples_split: return True
-        if depth == self.max_depth: return True
+        if len(y) <= self.min_samples_split:
+            return True
+        if depth == self.max_depth:
+            return True
         return False
-    
-    def _build_tree(self, 
-                    X: Matrix, 
-                    y: Vector, 
-                    depth: int, 
-                    sample_weights: Vector) -> DecisionTreeNode:
+
+    def _build_tree(
+        self, X: Matrix, y: Vector, depth: int, sample_weights: Vector
+    ) -> DecisionTreeNode:
         if self._stopping_criteria(y, depth):
             return DecisionTreeNode(value=np.average(y, weights=sample_weights))
-        
+
         split_idx, split_threshold = self._best_split(X, y, sample_weights)
         if split_idx is None:
             return DecisionTreeNode(value=np.average(y, weights=sample_weights))
-        
+
         left = X[:, split_idx] <= split_threshold
         right = X[:, split_idx] > split_threshold
-        
+
         X_left, X_right = X[left], X[right]
         y_left, y_right = y[left], y[right]
-        
+
         weights_left, weights_right = sample_weights[left], sample_weights[right]
-        
-        if np.sum(weights_left) < self.min_samples_leaf or \
-            np.sum(weights_right) < self.min_samples_leaf:
+
+        if (
+            np.sum(weights_left) < self.min_samples_leaf
+            or np.sum(weights_right) < self.min_samples_leaf
+        ):
             return DecisionTreeNode(value=np.average(y, weights=sample_weights))
-        
+
         left_subtree = self._build_tree(X_left, y_left, depth + 1, weights_left)
         right_subtree = self._build_tree(X_right, y_right, depth + 1, weights_right)
-        
-        return DecisionTreeNode(feature_index=split_idx, 
-                                threshold=split_threshold, 
-                                left=left_subtree, 
-                                right=right_subtree)
-
-    def _calculate_var_reduction(self, 
-                                 y: Vector, 
-                                 y_left: Vector, 
-                                 y_right: Vector, 
-                                 sample_weights: Vector, 
-                                 weights_left: Vector, 
-                                 weights_right: Vector) -> float:
+
+        return DecisionTreeNode(
+            feature_index=split_idx,
+            threshold=split_threshold,
+            left=left_subtree,
+            right=right_subtree,
+        )
+
+    def _calculate_var_reduction(
+        self,
+        y: Vector,
+        y_left: Vector,
+        y_right: Vector,
+        sample_weights: Vector,
+        weights_left: Vector,
+        weights_right: Vector,
+    ) -> float:
         total_weight = np.sum(sample_weights)
         y_avg = np.average(y, weights=sample_weights)
         weighted_total_var = np.average((y - y_avg) ** 2, weights=sample_weights)
-        
+
         y_left_avg = np.average(y_left, weights=weights_left)
         y_right_avg = np.average(y_right, weights=weights_right)
-        
+
         left_var = np.average((y_left - y_left_avg) ** 2, weights=weights_left)
         right_var = np.average((y_right - y_right_avg) ** 2, weights=weights_right)
-        
+
         weighted_var_red = weighted_total_var
         weighted_var_red -= (np.sum(weights_left) / total_weight) * left_var
         weighted_var_red -= (np.sum(weights_right) / total_weight) * right_var
-        
+
         return weighted_var_red
 
-    def _best_split(self, 
-                    X: Matrix, 
-                    y: Vector, 
-                    sample_weights: Vector) -> Tuple[int, float]:
+    def _best_split(
+        self, X: Matrix, y: Vector, sample_weights: Vector
+    ) -> Tuple[int, float]:
         best_reduction = -np.inf
         split_idx, split_threshold = None, None
-        
+
         for feature_index in range(X.shape[1]):
             thresholds = np.unique(X[:, feature_index])
             for threshold in thresholds:
                 left = X[:, feature_index] <= threshold
                 right = X[:, feature_index] > threshold
-                
-                if np.sum(sample_weights[left]) < self.min_samples_split or \
-                    np.sum(sample_weights[right]) < self.min_samples_split:
+
+                if (
+                    np.sum(sample_weights[left]) < self.min_samples_split
+                    or np.sum(sample_weights[right]) < self.min_samples_split
+                ):
                     continue
-                
+
                 reduction = self._calculate_var_reduction(
-                    y, y[left], y[right], sample_weights, 
-                    sample_weights[left], sample_weights[right]
+                    y,
+                    y[left],
+                    y[right],
+                    sample_weights,
+                    sample_weights[left],
+                    sample_weights[right],
                 )
-                
-                if reduction > best_reduction and \
-                    reduction >= self.min_variance_decrease:
+
+                if (
+                    reduction > best_reduction
+                    and reduction >= self.min_variance_decrease
+                ):
                     best_reduction = reduction
                     split_idx, split_threshold = feature_index, threshold
-        
+
         return split_idx, split_threshold
-    
+
     def _predict_single(self, node: DecisionTreeNode, x: Vector) -> float:
-        if node.value is not None: 
+        if node.value is not None:
             return node.value
-        if x[node.feature_index] <= node.threshold: 
+        if x[node.feature_index] <= node.threshold:
             return self._predict_single(node.left, x)
-        
+
         return self._predict_single(node.right, x)
 
     def predict(self, X: Matrix) -> Vector:
-        if not self._fitted: raise NotFittedError(self)
+        if not self._fitted:
+            raise NotFittedError(self)
         return np.array([self._predict_single(self.root, x) for x in X])
 
-    def score(self, X: Matrix, y: Vector, 
-              metric: Evaluator = MeanSquaredError) -> float:
+    def score(
+        self, X: Matrix, y: Vector, metric: Evaluator = MeanSquaredError
+    ) -> float:
         predictions = self.predict(X)
         return metric.score(y, predictions)
-
```

### Comparing `luma-ml-0.6.4/luma/visual/eda.py` & `luma-ml-0.6.5/luma/visual/eda.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,104 +2,100 @@
 import matplotlib.pyplot as plt
 import seaborn as sns
 import pandas as pd
 
 from luma.core.super import Visualizer
 
 
-__all__ = (
-    'CorrelationHeatMap', 
-    'CorrelationBar', 
-    'JointPlot', 
-    'MissingProportion'
-)
+__all__ = ("CorrelationHeatMap", "CorrelationBar", "JointPlot", "MissingProportion")
 
 
 class CorrelationHeatMap(Visualizer):
     def __init__(self, data: pd.DataFrame) -> None:
         self.data = data
         self.corr = data.corr()
-    
-    def plot(self, 
-             ax: Optional[plt.Axes] = None, 
-             colorMap: str = 'rocket', 
-             annotate: bool = True, 
-             colorBar: bool = True,
-             show: bool = False) -> plt.Axes:
+
+    def plot(
+        self,
+        ax: Optional[plt.Axes] = None,
+        colorMap: str = "rocket",
+        annotate: bool = True,
+        colorBar: bool = True,
+        show: bool = False,
+    ) -> plt.Axes:
         if ax is None:
             n_features = self.data.shape[1]
             size = n_features / 2 if n_features < 20 else 10
             _, ax = plt.subplots(figsize=(size + 1, size))
 
-        sns.heatmap(self.corr, 
-                    ax=ax, 
-                    cmap=colorMap, 
-                    annot=annotate, 
-                    cbar=colorBar, 
-                    fmt='0.2f')
-        
-        ax.set_title('Correlation Heat Map')
+        sns.heatmap(
+            self.corr, ax=ax, cmap=colorMap, annot=annotate, cbar=colorBar, fmt="0.2f"
+        )
+
+        ax.set_title("Correlation Heat Map")
         ax.figure.tight_layout()
-        
-        if show: plt.show()
+
+        if show:
+            plt.show()
         return ax
 
 
 class CorrelationBar(Visualizer):
     def __init__(self, data: pd.DataFrame, target: str) -> None:
         self.data = data
         self.target = target
-    
-    def plot(self, 
-             ax: Optional[plt.Axes] = None, 
-             show: bool = False) -> plt.Axes:
-        if ax is None: _, ax = plt.subplots()
-        corr_bar = [abs(self.data[col].corr(self.data[self.target])) for col in self.data]
+
+    def plot(self, ax: Optional[plt.Axes] = None, show: bool = False) -> plt.Axes:
+        if ax is None:
+            _, ax = plt.subplots()
+        corr_bar = [
+            abs(self.data[col].corr(self.data[self.target])) for col in self.data
+        ]
         sns.barplot(x=self.data.columns, y=corr_bar, hue=self.data.columns, ax=ax)
-        
+
         ax.set_xticklabels(ax.get_xticklabels(), rotation=45)
-        ax.set_title(f'Correlations with {self.target}')
-        ax.set_xlabel('Features')
-        ax.set_ylabel('Correlation')
+        ax.set_title(f"Correlations with {self.target}")
+        ax.set_xlabel("Features")
+        ax.set_ylabel("Correlation")
         ax.figure.tight_layout()
 
-        if show: plt.show()
+        if show:
+            plt.show()
         return ax
 
 
 class JointPlot(Visualizer):
     def __init__(self, data: pd.DataFrame, x: str, y: str) -> None:
         self.data = data
         self.x = x
         self.y = y
 
-    def plot(self, color: str = 'tab:blue') -> None:    
-        sns.jointplot(data=self.data, x=self.x, y=self.y, kind='reg', color=color)
-        plt.title(f'{self.x} vs. {self.y}')
+    def plot(self, color: str = "tab:blue") -> None:
+        sns.jointplot(data=self.data, x=self.x, y=self.y, kind="reg", color=color)
+        plt.title(f"{self.x} vs. {self.y}")
         plt.tight_layout()
         plt.show()
 
 
 class MissingProportion(Visualizer):
     def __init__(self, data: pd.DataFrame):
         self.data = data
 
     def nan_proportions(self) -> pd.DataFrame:
         nan_props = self.data.isna().mean()
         return nan_props
 
-    def plot(self, 
-             ax: Optional[plt.Axes] = None,
-             show: bool = False) -> plt.Axes:
-        if ax is None: _, ax = plt.subplots()
+    def plot(self, ax: Optional[plt.Axes] = None, show: bool = False) -> plt.Axes:
+        if ax is None:
+            _, ax = plt.subplots()
         nan_props = self.nan_proportions()
         sns.barplot(x=nan_props.index, y=nan_props.values, hue=self.data.columns, ax=ax)
-        
+
         ax.set_xticklabels(ax.get_xticklabels(), rotation=45)
-        ax.set_xlabel('Columns')
-        ax.set_ylabel('Proportion')
-        ax.set_title('Missing Value Proportions')
+        ax.set_xlabel("Columns")
+        ax.set_ylabel("Proportion")
+        ax.set_title("Missing Value Proportions")
         ax.figure.tight_layout()
-        
-        if show: plt.show()
-        return ax
 
+        if show:
+            plt.show()
+        return ax
```

### Comparing `luma-ml-0.6.4/luma/visual/evaluation.py` & `luma-ml-0.6.5/luma/visual/evaluation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,876 +1,967 @@
 from itertools import product
 from typing import Any, Dict, List, Literal, Optional, Tuple
-from matplotlib.colors import ListedColormap 
+from matplotlib.colors import ListedColormap
 import matplotlib.pyplot as plt
 import numpy as np
 
 from luma.interface.util import Matrix, Vector
 from luma.core.super import Evaluator, Visualizer, Estimator
 from luma.model_selection.split import TrainTestSplit
 from luma.preprocessing.encoder import LabelBinarizer
 from luma.metric.classification import Accuracy, Precision, Recall, Specificity
 from luma.model_selection.cv import CrossValidator
 from luma.model_selection.fold import FoldType, KFold
 
 
 __all__ = (
-    'DecisionRegion', 
-    'ClusterPlot',
-    'ROCCurve',
-    'PrecisionRecallCurve',
-    'ConfusionMatrix',
-    'ResidualPlot',
-    'LearningCurve',
-    'ValidationCurve',
-    'ValidationHeatmap',
-    'InertiaPlot'
+    "DecisionRegion",
+    "ClusterPlot",
+    "ROCCurve",
+    "PrecisionRecallCurve",
+    "ConfusionMatrix",
+    "ResidualPlot",
+    "LearningCurve",
+    "ValidationCurve",
+    "ValidationHeatmap",
+    "InertiaPlot",
 )
 
 
 class DecisionRegion(Visualizer):
-    def __init__(self, 
-                 estimator: Estimator,
-                 X: Matrix, 
-                 y: Optional[Matrix] = None, 
-                 title: str | Literal['auto'] = 'auto', 
-                 xlabel: str = r'$x_1$', 
-                 ylabel: str = r'$x_2$',
-                 cmap: ListedColormap = 'rainbow',
-                 alpha: float = 0.4) -> None:
+    def __init__(
+        self,
+        estimator: Estimator,
+        X: Matrix,
+        y: Optional[Matrix] = None,
+        title: str | Literal["auto"] = "auto",
+        xlabel: str = r"$x_1$",
+        ylabel: str = r"$x_2$",
+        cmap: ListedColormap = "rainbow",
+        alpha: float = 0.4,
+    ) -> None:
         self.estimator = estimator
         self.X = X
         self.y = y
         self.title = title
         self.xlabel = xlabel
         self.ylabel = ylabel
         self.cmap = cmap
         self.alpha = alpha
-        
-        if self.title == 'auto':
+
+        if self.title == "auto":
             self.title = type(self.estimator).__name__
 
-        if self.y is None and hasattr(self.estimator, 'labels'):
+        if self.y is None and hasattr(self.estimator, "labels"):
             self.y = self.estimator.labels
 
-    def plot(self, 
-             ax: Optional[plt.Axes] = None, 
-             size: float = 250, 
-             scale: float = 10.0, 
-             show: bool = False) -> plt.Axes:
+    def plot(
+        self,
+        ax: Optional[plt.Axes] = None,
+        size: float = 250,
+        scale: float = 10.0,
+        show: bool = False,
+    ) -> plt.Axes:
         x1_min, x1_max = self.X[:, 0].min(), self.X[:, 0].max()
         x2_min, x2_max = self.X[:, 1].min(), self.X[:, 1].max()
         delta_1, delta_2 = (x1_max - x1_min) / size, (x2_max - x2_min) / size
-        
+
         x1_min, x1_max = x1_min - delta_1 * scale, x1_max + delta_1 * scale
         x2_min, x2_max = x2_min - delta_2 * scale, x2_max + delta_2 * scale
-        xx1, xx2 = np.meshgrid(np.arange(x1_min, x1_max, delta_1), 
-                               np.arange(x2_min, x2_max, delta_2))
-        
+        xx1, xx2 = np.meshgrid(
+            np.arange(x1_min, x1_max, delta_1), np.arange(x2_min, x2_max, delta_2)
+        )
+
         Z = self.estimator.predict(Matrix([xx1.ravel(), xx2.ravel()]).T)
         Z = Z.reshape(xx1.shape)
-        
-        if ax is None: 
+
+        if ax is None:
             _, ax = plt.subplots()
             show = True
-        
-        ax.contourf(xx1, xx2, Z, 
-                    alpha=self.alpha, 
-                    cmap=self.cmap, 
-                    levels=len(np.unique(self.y)))
-        
+
+        ax.contourf(
+            xx1, xx2, Z, alpha=self.alpha, cmap=self.cmap, levels=len(np.unique(self.y))
+        )
+
         ax.set_xlim(xx1.min(), xx1.max())
         ax.set_ylim(xx2.min(), xx2.max())
 
-        ax.scatter(self.X[:, 0], self.X[:, 1], 
-                   c=self.y, 
-                   cmap=self.cmap, 
-                   alpha=0.8, 
-                   edgecolors='black')
-        
+        ax.scatter(
+            self.X[:, 0],
+            self.X[:, 1],
+            c=self.y,
+            cmap=self.cmap,
+            alpha=0.8,
+            edgecolors="black",
+        )
+
         ax.set_xlabel(self.xlabel)
         ax.set_ylabel(self.ylabel)
         ax.set_title(self.title)
         ax.figure.tight_layout()
-        
-        if show: plt.show()
+
+        if show:
+            plt.show()
         return ax
 
 
 class ClusterPlot(Visualizer):
-    def __init__(self,
-                 estimator: Estimator,
-                 X: Matrix,
-                 title: str | Literal['auto'] = 'auto',
-                 xlabel: str = r'$x_1$',
-                 ylabel: str = r'$x_2$',
-                 cmap: ListedColormap = 'rainbow',
-                 alpha: float = 0.8) -> None:
+    def __init__(
+        self,
+        estimator: Estimator,
+        X: Matrix,
+        title: str | Literal["auto"] = "auto",
+        xlabel: str = r"$x_1$",
+        ylabel: str = r"$x_2$",
+        cmap: ListedColormap = "rainbow",
+        alpha: float = 0.8,
+    ) -> None:
         self.estimator = estimator
         self.X = X
         self.title = title
         self.xlabel = xlabel
         self.ylabel = ylabel
         self.cmap = cmap
         self.alpha = alpha
         self.labels = self.estimator.labels
-        
-        if self.title == 'auto':
+
+        if self.title == "auto":
             self.title = type(self.estimator).__name__
-    
-    def plot(self, 
-             ax: Optional[plt.Axes] = None, 
-             show: bool = False) -> plt.Axes:
-        if ax is None: 
+
+    def plot(self, ax: Optional[plt.Axes] = None, show: bool = False) -> plt.Axes:
+        if ax is None:
             _, ax = plt.subplots()
             show = True
-        
-        ax.scatter(self.X[self.labels == -1, 0], 
-                   self.X[self.labels == -1, 1],
-                   marker='x',
-                   c='black', 
-                   label='Noise')
-        
-        ax.scatter(self.X[self.labels != -1, 0], 
-                   self.X[self.labels != -1, 1], 
-                   marker='o',
-                   c=self.labels[self.labels != -1],
-                   cmap=self.cmap,
-                   alpha=self.alpha,
-                   edgecolors='black')
-        
+
+        ax.scatter(
+            self.X[self.labels == -1, 0],
+            self.X[self.labels == -1, 1],
+            marker="x",
+            c="black",
+            label="Noise",
+        )
+
+        ax.scatter(
+            self.X[self.labels != -1, 0],
+            self.X[self.labels != -1, 1],
+            marker="o",
+            c=self.labels[self.labels != -1],
+            cmap=self.cmap,
+            alpha=self.alpha,
+            edgecolors="black",
+        )
+
         ax.set_title(self.title)
         ax.set_xlabel(self.xlabel)
         ax.set_ylabel(self.ylabel)
-        
-        if len(self.X[self.labels == -1]): ax.legend()
+
+        if len(self.X[self.labels == -1]):
+            ax.legend()
         ax.figure.tight_layout()
-        
-        if show: plt.show()
+
+        if show:
+            plt.show()
         return ax
 
 
 class ROCCurve(Visualizer):
-    def __init__(self,
-                 y_true: Vector,
-                 y_scores: Matrix) -> None:
+    def __init__(self, y_true: Vector, y_scores: Matrix) -> None:
         self.y_true = y_true
         self.y_scores = y_scores
         self.n_classes = y_scores.shape[1]
-    
-    def plot(self, 
-             ax: Optional[plt.Axes] = None, 
-             show: bool = False) -> plt.Axes:
-        if ax is None: 
+
+    def plot(self, ax: Optional[plt.Axes] = None, show: bool = False) -> plt.Axes:
+        if ax is None:
             _, ax = plt.subplots()
             show = True
-        
+
         y_binary = LabelBinarizer().fit_transform(self.y_true)
-        
+
         fprs, tprs = [], []
         for cl in range(self.n_classes):
             fpr, tpr = self._fpr_tpr(y_binary[:, cl], self.y_scores[:, cl])
             fprs.append(fpr)
             tprs.append(tpr)
-            
+
             auc = self._auc(fpr, tpr)
-            ax.plot(fpr, tpr, 
-                    linewidth=2,
-                    label=f'ROC Curve {cl} (area = {auc:.2f})')
-        
+            ax.plot(fpr, tpr, linewidth=2, label=f"ROC Curve {cl} (area = {auc:.2f})")
+
         mean_fpr, mean_tpr = np.mean(fprs, axis=0), np.mean(tprs, axis=0)
         mean_auc = self._auc(mean_fpr, mean_tpr)
-        
-        ax.plot(mean_fpr, mean_tpr,
-                color='dimgray', 
-                linewidth=2,
-                linestyle='--', 
-                label=f'Mean ROC (area = {mean_auc:.2f})')
-        
-        ax.plot([0, 1], [0, 1], 
-                color='darkgray', 
-                linestyle=':', 
-                label='Random Guessing')
-        
+
+        ax.plot(
+            mean_fpr,
+            mean_tpr,
+            color="dimgray",
+            linewidth=2,
+            linestyle="--",
+            label=f"Mean ROC (area = {mean_auc:.2f})",
+        )
+
+        ax.plot(
+            [0, 1], [0, 1], color="darkgray", linestyle=":", label="Random Guessing"
+        )
+
         ax.set_xlim([-0.05, 1.05])
         ax.set_ylim([-0.05, 1.05])
-        ax.set_xlabel('False Positive Rate')
-        
-        ax.set_ylabel('True Positive Rate')
-        ax.set_title('ROC Curve')
+        ax.set_xlabel("False Positive Rate")
+
+        ax.set_ylabel("True Positive Rate")
+        ax.set_title("ROC Curve")
         ax.legend(loc="lower right")
         ax.figure.tight_layout()
-        
-        if show: plt.show()
+
+        if show:
+            plt.show()
         return ax
-    
+
     def _fpr_tpr(self, y_true: Vector, y_score: Vector) -> Tuple[Vector, Vector]:
         thresholds = np.sort(y_score)[::-1]
         fpr, tpr = [], []
         for threshold in thresholds:
             y_pred = y_score >= threshold
             tpr.append(Recall.score(y_true, y_pred))
             fpr.append(1 - Specificity.score(y_true, y_pred))
-        
+
         return Vector(fpr), Vector(tpr)
-    
+
     def _auc(self, fpr: Vector, tpr: Vector) -> float:
         auc = 0
         for i in range(1, len(fpr)):
             auc += (fpr[i] - fpr[i - 1]) * (tpr[i] + tpr[i - 1]) / 2
         return auc
 
 
 class PrecisionRecallCurve(Visualizer):
-    def __init__(self,
-                 y_true: Vector,
-                 y_scores: Matrix) -> None:
+    def __init__(self, y_true: Vector, y_scores: Matrix) -> None:
         self.y_true = y_true
         self.y_scores = y_scores
         self.n_classes = y_scores.shape[1]
 
-    def plot(self,
-             ax: Optional[plt.Axes] = None,
-             show: bool = False) -> plt.Axes:
-        if ax is None: 
+    def plot(self, ax: Optional[plt.Axes] = None, show: bool = False) -> plt.Axes:
+        if ax is None:
             _, ax = plt.subplots()
             show = True
-        
+
         y_binary = LabelBinarizer().fit_transform(self.y_true)
         pres, recs = [], []
         for cl in range(self.n_classes):
             pre, rec = self._pre_rec(y_binary[:, cl], self.y_scores[:, cl])
             pres.append(pre)
             recs.append(rec)
 
             ap = self._average_precision(pre, rec)
-            ax.plot(rec, pre,
-                    linewidth=2,
-                    label=f'PR Curve {cl} (AP = {ap:.2f})')
+            ax.plot(rec, pre, linewidth=2, label=f"PR Curve {cl} (AP = {ap:.2f})")
 
         mean_pre, mean_rec = np.mean(pres, axis=0), np.mean(recs, axis=0)
         mean_ap = self._average_precision(mean_pre, mean_rec)
 
-        ax.plot(mean_rec, mean_pre,
-                color='dimgray',
-                linewidth=2,
-                linestyle='--',
-                label=f'Mean PR (AP = {mean_ap:.2f})')
-        
-        ax.plot([1, 0], [0, 1], 
-                color='darkgray', 
-                linestyle=':', 
-                label='Random Guessing')
+        ax.plot(
+            mean_rec,
+            mean_pre,
+            color="dimgray",
+            linewidth=2,
+            linestyle="--",
+            label=f"Mean PR (AP = {mean_ap:.2f})",
+        )
+
+        ax.plot(
+            [1, 0], [0, 1], color="darkgray", linestyle=":", label="Random Guessing"
+        )
 
         ax.set_xlim([-0.05, 1.05])
         ax.set_ylim([-0.05, 1.05])
-        ax.set_xlabel('Recall')
-        ax.set_ylabel('Precision')
-        ax.set_title('Precision-Recall Curve')
+        ax.set_xlabel("Recall")
+        ax.set_ylabel("Precision")
+        ax.set_title("Precision-Recall Curve")
         ax.legend(loc="lower left")
         ax.figure.tight_layout()
-        
-        if show: plt.show()
+
+        if show:
+            plt.show()
         return ax
-    
+
     def _pre_rec(self, y_true: Vector, y_score: Vector) -> Tuple[Vector, Vector]:
         thresholds = np.sort(y_score)[::-1]
         pre, rec = [], []
         for threshold in thresholds:
             y_pred = y_score >= threshold
             pre.append(Precision.score(y_true, y_pred))
             rec.append(Recall.score(y_true, y_pred))
 
         return Vector(pre), Vector(rec)
-    
+
     def _average_precision(self, pre: Vector, rec: Vector) -> float:
         ap = 0
         for i in range(1, len(rec)):
             ap += (rec[i] - rec[i - 1]) * pre[i]
         return ap
 
 
 class ConfusionMatrix(Visualizer):
-    def __init__(self, 
-                 y_true: Vector, 
-                 y_pred: Vector, 
-                 labels: List[str] | None = None,
-                 cmap: ListedColormap = 'Blues') -> None:
+    def __init__(
+        self,
+        y_true: Vector,
+        y_pred: Vector,
+        labels: List[str] | None = None,
+        title: str | Literal["auto"] = "auto",
+        cmap: ListedColormap = "Blues",
+    ) -> None:
         self.cmap = cmap
         self.conf_matrix = self._confusion_matrix(y_true, y_pred)
         self.labels = labels
-        
+        self.title = title
+
         if labels is None:
             self.labels = np.arange(len(np.unique(y_true)))
 
     def plot(self, ax: Optional[plt.Axes] = None, show: bool = False) -> plt.Axes:
-        if ax is None: 
+        if ax is None:
             _, ax = plt.subplots()
             show = True
-        
-        cax = ax.imshow(self.conf_matrix, interpolation='nearest', cmap=self.cmap)
-        ax.set_title('Confusion Matrix')
+
+        cax = ax.imshow(self.conf_matrix, interpolation="nearest", cmap=self.cmap)
+        if self.title == "auto":
+            ax.set_title("Confusion Matrix")
+        else:
+            ax.set_title(self.title)
+
         plt.colorbar(cax, ax=ax)
 
         tick_marks = np.arange(len(self.labels))
         ax.set_xticks(tick_marks)
         ax.set_xticklabels(self.labels, rotation=45)
         ax.set_yticks(tick_marks)
         ax.set_yticklabels(self.labels)
 
-        thresh = self.conf_matrix.max() / 2.
+        thresh = self.conf_matrix.max() / 2.0
         for i, j in np.ndindex(self.conf_matrix.shape):
-            ax.text(j, i, format(self.conf_matrix[i, j], 'd'),
-                    horizontalalignment="center",
-                    color="white" if self.conf_matrix[i, j] > thresh else "black")
-
-        ax.set_ylabel('True label')
-        ax.set_xlabel('Predicted label')
-        ax.set_aspect('equal', adjustable='box')
+            ax.text(
+                j,
+                i,
+                format(self.conf_matrix[i, j], "d"),
+                horizontalalignment="center",
+                color="white" if self.conf_matrix[i, j] > thresh else "black",
+            )
+
+        ax.set_ylabel("True label")
+        ax.set_xlabel("Predicted label")
+        ax.set_aspect("equal", adjustable="box")
         ax.figure.tight_layout()
-        
-        if show: plt.show()
+
+        if show:
+            plt.show()
         return ax
-    
+
     def _confusion_matrix(self, y_true: Vector, y_pred: Vector) -> Matrix:
         unique_labels = np.unique(np.concatenate((y_true, y_pred)))
         matrix = np.zeros((len(unique_labels), len(unique_labels)), dtype=int)
         for true, pred in zip(y_true, y_pred):
             matrix[true, pred] += 1
-        
+
         return matrix
 
 
 class ResidualPlot(Visualizer):
-    def __init__(self, 
-                 estimator: Estimator,
-                 X: Matrix,
-                 y: Vector,
-                 alpha: float = 0.8,
-                 cmap: ListedColormap = 'RdYlBu') -> None:
+    def __init__(
+        self,
+        estimator: Estimator,
+        X: Matrix,
+        y: Vector,
+        alpha: float = 0.8,
+        cmap: ListedColormap = "RdYlBu",
+    ) -> None:
         self.estimator = estimator
         self.X = X
         self.y = y
         self.alpha = alpha
         self.cmap = cmap
-    
-    def plot(self, 
-             ax: Optional[plt.Axes] = None,
-             show: bool = False) -> plt.Axes:
-        if ax is None: 
+
+    def plot(self, ax: Optional[plt.Axes] = None, show: bool = False) -> plt.Axes:
+        if ax is None:
             _, ax = plt.subplots()
             show = True
-        
+
         resid = self._calculate_residuals()
-        cax = ax.scatter(self.estimator.predict(self.X), 
-                         resid, 
-                         c=resid, 
-                         s=20, 
-                         cmap=self.cmap, 
-                         alpha=self.alpha)
-
-        ax.axhline(y=0, c='black', 
-                   lw=2, label='Perfect Fit')
-        
-        ax.axhline(y=resid.mean(), c='gray', ls='--', 
-                   lw=2, label='Average Residual')
-        
-        ax.set_xlabel('Predicted Values')
-        ax.set_ylabel('Residuals')
-        ax.set_title(f'Residual Plot of {type(self.estimator).__name__}')
-        
+        cax = ax.scatter(
+            self.estimator.predict(self.X),
+            resid,
+            c=resid,
+            s=20,
+            cmap=self.cmap,
+            alpha=self.alpha,
+        )
+
+        ax.axhline(y=0, c="black", lw=2, label="Perfect Fit")
+
+        ax.axhline(y=resid.mean(), c="gray", ls="--", lw=2, label="Average Residual")
+
+        ax.set_xlabel("Predicted Values")
+        ax.set_ylabel("Residuals")
+        ax.set_title(f"Residual Plot of {type(self.estimator).__name__}")
+
         ax.figure.colorbar(cax)
         ax.legend()
         ax.figure.tight_layout()
-        
-        if show: plt.show()
+
+        if show:
+            plt.show()
         return ax
 
     def _calculate_residuals(self) -> Vector:
-        if not self.estimator._fitted: 
+        if not self.estimator._fitted:
             self.estimator.fit(self.X, self.y)
-        
+
         predictions = self.estimator.predict(self.X)
         residuals = self.y - predictions
         return residuals
 
 
 class LearningCurve(Visualizer):
-    
     """
-    A learning curve in machine learning is a graph that compares the performance 
-    of a model on training and validation data over a series of training iterations. 
-    It helps to diagnose problems like overfitting or underfitting by showing how 
-    the model's error changes as it learns. A steep learning curve indicates rapid 
+    A learning curve in machine learning is a graph that compares the performance
+    of a model on training and validation data over a series of training iterations.
+    It helps to diagnose problems like overfitting or underfitting by showing how
+    the model's error changes as it learns. A steep learning curve indicates rapid
     learning, while a plateau suggests no further learning. The ideal curve shows
-    decreasing error on both training and validation datasets, converging to a 
+    decreasing error on both training and validation datasets, converging to a
     low level.
-    
+
     Parameters
     ----------
     `estimator` : An estimator to evaluate
     `X` : Feature data for training
     `y`: Target data for training
     `train_sizes` : List of fractional values for each dataset size
     `test_size` : Proportional value for validation set size
     `cv` : Number of times for cross-validation
     `shuffle` : Whether to shuffle the dataset
     `stratify` : Whether to perform stratified split
     `fold_type` : Fold type (Default `KFold`)
     `metric` : Evaluation metric for scoring
     `random_state` : Seed for random sampling upon splitting samples
-    
+
     """
-    
-    def __init__(self, 
-                 estimator: Estimator, 
-                 X: Matrix, 
-                 y: Vector, 
-                 train_sizes: Vector = None, 
-                 test_size: float = 0.3,
-                 cv: int = 5,
-                 shuffle: bool = True,
-                 stratify: bool = False,
-                 fold_type: FoldType = KFold,
-                 metric: Evaluator = Accuracy,
-                 random_state: int = None,
-                 verbose: bool = False):
+
+    def __init__(
+        self,
+        estimator: Estimator,
+        X: Matrix,
+        y: Vector,
+        train_sizes: Vector = None,
+        test_size: float = 0.3,
+        cv: int = 5,
+        shuffle: bool = True,
+        stratify: bool = False,
+        fold_type: FoldType = KFold,
+        metric: Evaluator = Accuracy,
+        random_state: int = None,
+        verbose: bool = False,
+    ):
         self.estimator = estimator
         self.X = X
         self.y = y
         self.train_sizes = train_sizes
         self.test_size = test_size
         self.cv = cv
         self.shuffle = shuffle
         self.stratify = stratify
         self.fold_type = fold_type
         self.metric = metric
         self.random_state = random_state
         self.verbose = verbose
-        
+
         if train_sizes is None:
             self.train_sizes = np.linspace(0.1, 1.0, 5)
-    
+
     def _evaluate(self) -> None:
         m, _ = self.X.shape
         self.train_scores, self.test_scores = [], []
-        
+
         for train_size in self.train_sizes:
             n_samples = int(train_size * m)
-            
+
             X_train, X_val, y_train, y_val = TrainTestSplit(
                 self.X,
                 self.y,
                 test_size=n_samples,
                 shuffle=self.shuffle,
                 stratify=self.stratify,
-                random_state=self.random_state
+                random_state=self.random_state,
             ).get
-            
+
             if n_samples == len(self.X):
                 X_train = X_val = self.X
                 y_train = y_val = self.y
-            
+
             self.estimator.fit(X_train, y_train)
             cv_param = (
                 self.estimator,
                 self.metric,
                 self.cv,
                 self.fold_type,
                 self.shuffle,
                 self.random_state,
-                self.verbose
+                self.verbose,
             )
-            
+
             if self.verbose:
-                print(f'Starting CV for training set with {self.cv} folds')
-            
+                print(f"Starting CV for training set with {self.cv} folds")
+
             cv_train = CrossValidator(*cv_param)
             cv_train._fit(X_train, y_train)
             self.train_scores.append(cv_train.test_scores_)
-            
+
             if self.verbose:
-                print(f'Starting CV for validation set with {self.cv} folds')
-            
+                print(f"Starting CV for validation set with {self.cv} folds")
+
             cv_test = CrossValidator(*cv_param)
             cv_test._fit(X_val, y_val)
             self.test_scores.append(cv_test.test_scores_)
-            
+
             if self.verbose:
-                print(f'[LearningCurve] Finished evaluating for',
-                      f'{n_samples} samples')
-        
+                print(
+                    f"[LearningCurve] Finished evaluating for", f"{n_samples} samples"
+                )
+
         self.train_scores = Matrix(self.train_scores)
         self.test_scores = Matrix(self.test_scores)
-    
-    def plot(self, 
-             ax: Optional[plt.Axes] = None, 
-             show: bool = False) -> plt.Axes:
+
+    def plot(self, ax: Optional[plt.Axes] = None, show: bool = False) -> plt.Axes:
         self._evaluate()
         self.train_sizes = (self.train_sizes * self.X.shape[0]).astype(int)
         metric_name = self.metric.__name__
-        
+
         train_mean = self.train_scores.mean(axis=1)
         train_std = self.train_scores.std(axis=1)
         test_mean = self.test_scores.mean(axis=1)
         test_std = self.test_scores.std(axis=1)
-        
-        if ax is None: 
+
+        if ax is None:
             _, ax = plt.subplots()
             show = True
-        
-        ax.plot(self.train_sizes, train_mean,
-                'o-', color="royalblue", label=f"Training {metric_name}")
-        ax.plot(self.train_sizes, test_mean,
-                'o--', color="seagreen", label=f"Validation {metric_name}")
-
-        ax.fill_between(self.train_sizes, 
-                        train_mean + train_std, 
-                        train_mean - train_std, 
-                        color='royalblue', 
-                        alpha=0.2)
-        
-        ax.fill_between(self.train_sizes, 
-                        test_mean + test_std, 
-                        test_mean - test_std, 
-                        color='seagreen', 
-                        alpha=0.2)
+
+        ax.plot(
+            self.train_sizes,
+            train_mean,
+            "o-",
+            color="royalblue",
+            label=f"Training {metric_name}",
+        )
+        ax.plot(
+            self.train_sizes,
+            test_mean,
+            "o--",
+            color="seagreen",
+            label=f"Validation {metric_name}",
+        )
+
+        ax.fill_between(
+            self.train_sizes,
+            train_mean + train_std,
+            train_mean - train_std,
+            color="royalblue",
+            alpha=0.2,
+        )
+
+        ax.fill_between(
+            self.train_sizes,
+            test_mean + test_std,
+            test_mean - test_std,
+            color="seagreen",
+            alpha=0.2,
+        )
 
         ax.set_title(f"Learning Curve")
         ax.set_xlabel("Number of Training Examples")
         ax.set_ylabel(metric_name)
         ax.set_ylim(0.0, 1.1)
         ax.legend()
         ax.grid()
         ax.figure.tight_layout()
-        
-        if show: plt.show()
+
+        if show:
+            plt.show()
         return ax
 
 
 class ValidationCurve(Visualizer):
-    
     """
     A validation curve in machine learning is a graph that compares the performance
-    of a model on training and validation data over a range of values for a specific 
+    of a model on training and validation data over a range of values for a specific
     hyperparameter. It helps to diagnose the best hyperparameter setting by showing
     how the model's error changes as the value of the hyperparameter changes.
-    
+
     Parameters
     ----------
     `estimator` : An estimator to evaluate
     `X` : Feature data for training
     `y`: Target data for training
     `param_name` : Name of the hyperparameter to be varied
     `param_range` : Range of values for the hyperparameter
     `cv` : Number of times for cross-validation
     `shuffle` : Whether to shuffle the dataset
     `fold_type` : Fold type (Default `KFold`)
     `metric` : Evaluation metric for scoring
     `random_state` : Seed for random sampling upon splitting samples
-    
+
     """
-    
-    def __init__(self, 
-                 estimator: Estimator, 
-                 X: Matrix, 
-                 y: Vector, 
-                 param_name: str, 
-                 param_range: Vector, 
-                 cv: int = 5, 
-                 shuffle: bool = True,
-                 fold_type: FoldType = KFold,
-                 metric: Evaluator = Accuracy, 
-                 random_state: int = None,
-                 verbose: bool = False):
+
+    def __init__(
+        self,
+        estimator: Estimator,
+        X: Matrix,
+        y: Vector,
+        param_name: str,
+        param_range: Vector,
+        cv: int = 5,
+        shuffle: bool = True,
+        fold_type: FoldType = KFold,
+        metric: Evaluator = Accuracy,
+        random_state: int = None,
+        verbose: bool = False,
+    ):
         self.estimator = estimator
         self.X = X
         self.y = y
         self.param_name = param_name
         self.param_range = param_range
         self.cv = cv
         self.shuffle = shuffle
         self.fold_type = fold_type
         self.metric = metric
         self.random_state = random_state
         self.verbose = verbose
-    
+
     def _evaluate(self) -> None:
         self.train_scores, self.test_scores = [], []
         for param_value in self.param_range:
             setattr(self.estimator, self.param_name, param_value)
-            
-            cv_model = CrossValidator(estimator=self.estimator,
-                                      metric=self.metric,
-                                      cv=self.cv,
-                                      shuffle=self.shuffle,
-                                      fold_type=self.fold_type,
-                                      random_state=self.random_state,
-                                      verbose=self.verbose)
-            
+
+            cv_model = CrossValidator(
+                estimator=self.estimator,
+                metric=self.metric,
+                cv=self.cv,
+                shuffle=self.shuffle,
+                fold_type=self.fold_type,
+                random_state=self.random_state,
+                verbose=self.verbose,
+            )
+
             cv_model._fit(self.X, self.y)
             self.train_scores.append(cv_model.train_scores_)
             self.test_scores.append(cv_model.test_scores_)
 
             if self.verbose:
-                print(f'[ValidationCurve] Finished evaluating for',
-                      f'{self.param_name}={param_value}')
-        
+                print(
+                    f"[ValidationCurve] Finished evaluating for",
+                    f"{self.param_name}={param_value}",
+                )
+
         self.train_scores = Matrix(self.train_scores)
         self.test_scores = Matrix(self.test_scores)
 
-    def plot(self, 
-             ax: Optional[plt.Axes] = None, 
-             xscale: str = None,
-             show: bool = False) -> plt.Axes:
+    def plot(
+        self, ax: Optional[plt.Axes] = None, xscale: str = None, show: bool = False
+    ) -> plt.Axes:
         self._evaluate()
         metric_name = self.metric.__name__
 
         train_mean = self.train_scores.mean(axis=1)
         train_std = self.train_scores.std(axis=1)
         test_mean = self.test_scores.mean(axis=1)
         test_std = self.test_scores.std(axis=1)
-        
-        if ax is None: 
+
+        if ax is None:
             _, ax = plt.subplots()
             show = True
-        
-        ax.plot(self.param_range, train_mean,
-                'o-', color="royalblue", label=f"Training {metric_name}")
-        ax.plot(self.param_range, test_mean,
-                'o--', color="seagreen", label=f"Validation {metric_name}")
-        
-        ax.fill_between(self.param_range, 
-                        train_mean + train_std, 
-                        train_mean - train_std, 
-                        color='royalblue', 
-                        alpha=0.2)
-        
-        ax.fill_between(self.param_range, 
-                        test_mean + test_std, 
-                        test_mean - test_std, 
-                        color='seagreen', 
-                        alpha=0.2)
-        
+
+        ax.plot(
+            self.param_range,
+            train_mean,
+            "o-",
+            color="royalblue",
+            label=f"Training {metric_name}",
+        )
+        ax.plot(
+            self.param_range,
+            test_mean,
+            "o--",
+            color="seagreen",
+            label=f"Validation {metric_name}",
+        )
+
+        ax.fill_between(
+            self.param_range,
+            train_mean + train_std,
+            train_mean - train_std,
+            color="royalblue",
+            alpha=0.2,
+        )
+
+        ax.fill_between(
+            self.param_range,
+            test_mean + test_std,
+            test_mean - test_std,
+            color="seagreen",
+            alpha=0.2,
+        )
+
         ax.set_title(f"Validation Curve for '{self.param_name}'")
         ax.set_xlabel(self.param_name)
         ax.set_ylabel(metric_name)
-        
-        ax.set_xscale(xscale if xscale else 'linear')
+
+        ax.set_xscale(xscale if xscale else "linear")
         ax.set_ylim(0.0, 1.1)
         ax.legend()
         ax.grid()
         ax.figure.tight_layout()
-        
-        if show: plt.show()
+
+        if show:
+            plt.show()
         return ax
 
 
 class ValidationHeatmap(Visualizer):
-    
     """
-    A validation heatmap in machine learning is a graphical representation that 
-    illustrates the performance of a model on a validation dataset for different 
-    combinations of two hyperparameters. Each cell in the heatmap corresponds to a 
-    specific combination of the hyperparameters' values, and the color intensity 
-    represents the performance metric score. This visualization is useful for 
-    identifying the interaction between two hyperparameters and selecting the best 
+    A validation heatmap in machine learning is a graphical representation that
+    illustrates the performance of a model on a validation dataset for different
+    combinations of two hyperparameters. Each cell in the heatmap corresponds to a
+    specific combination of the hyperparameters' values, and the color intensity
+    represents the performance metric score. This visualization is useful for
+    identifying the interaction between two hyperparameters and selecting the best
     combination for model tuning.
 
     Parameters
     ----------
     `estimator` : An estimator to evaluate
     `X` : Feature data for training
     `y` : Target data for training
     `param_dict` : Dictionary with two hyperparameters and their respective ranges
     `cv` : Number of times for cross-validation
     `shuffle` : Whether to shuffle the dataset
     `fold_type` : Fold type (Default `KFold`)
     `metric` : Evaluation metric for scoring
     `random_state` : Seed for random sampling upon splitting samples
-    
+
     """
-    
-    def __init__(self, 
-                 estimator: Estimator, 
-                 X: Matrix, 
-                 y: Vector, 
-                 param_dict: Dict[str, Any],
-                 cv: int = 5, 
-                 shuffle: bool = True,
-                 fold_type: FoldType = KFold,
-                 metric: Evaluator = Accuracy, 
-                 random_state: int = None,
-                 verbose: bool = False) -> None:
+
+    def __init__(
+        self,
+        estimator: Estimator,
+        X: Matrix,
+        y: Vector,
+        param_dict: Dict[str, Any],
+        cv: int = 5,
+        shuffle: bool = True,
+        fold_type: FoldType = KFold,
+        metric: Evaluator = Accuracy,
+        random_state: int = None,
+        verbose: bool = False,
+    ) -> None:
         self.estimator = estimator
         self.X = X
         self.y = y
         self.param_dict = param_dict
         self.cv = cv
         self.shuffle = shuffle
         self.fold_type = fold_type
         self.metric = metric
         self.random_state = random_state
         self.verbose = verbose
-        
+
         self.names_ = list(self.param_dict.keys())
-        
-        self.sizes_ = (len(self.param_dict[self.names_[0]]), 
-                       len(self.param_dict[self.names_[1]]))
-        
-        self.values_ = (self.param_dict[self.names_[0]],
-                        self.param_dict[self.names_[1]])
-        
+
+        self.sizes_ = (
+            len(self.param_dict[self.names_[0]]),
+            len(self.param_dict[self.names_[1]]),
+        )
+
+        self.values_ = (
+            self.param_dict[self.names_[0]],
+            self.param_dict[self.names_[1]],
+        )
+
         self.scores = np.zeros(self.sizes_)
-    
+
     def _evaluate(self) -> None:
         param_combs = list(product(*self.param_dict.values()))
         max_iter = len(param_combs)
-        
+
         if self.verbose:
-            print(f'Fitting {self.cv} folds for {max_iter} candidates,',
-                  f'totalling {self.cv * max_iter} fits.\n')
+            print(
+                f"Fitting {self.cv} folds for {max_iter} candidates,",
+                f"totalling {self.cv * max_iter} fits.\n",
+            )
 
         for idx, params in enumerate(param_combs):
             param_values = dict(zip(self.names_, params))
             self.estimator.set_params(**param_values)
 
-            cv_model = CrossValidator(estimator=self.estimator,
-                                      metric=self.metric,
-                                      cv=self.cv,
-                                      shuffle=self.shuffle,
-                                      fold_type=self.fold_type,
-                                      random_state=self.random_state,
-                                      verbose=False)
-            
+            cv_model = CrossValidator(
+                estimator=self.estimator,
+                metric=self.metric,
+                cv=self.cv,
+                shuffle=self.shuffle,
+                fold_type=self.fold_type,
+                random_state=self.random_state,
+                verbose=False,
+            )
+
             _, score = cv_model.score(self.X, self.y)
             i, j = idx // self.sizes_[1], idx % self.sizes_[1]
             self.scores[i, j] = score
-            
+
             if self.verbose:
-                print(f'[ValidationHeatmap] candidate {idx + 1}/{max_iter}',
-                      f'{param_values} - score: {score:.3f}')
-    
-    def plot(self, 
-             ax: Optional[plt.Axes] = None, 
-             cmap: ListedColormap = 'RdYlGn',
-             log_xticks: bool = True,
-             log_yticks: bool = True,
-             annotate: bool = True,
-             show: bool = False) -> plt.Axes:
-        if ax is None: 
+                print(
+                    f"[ValidationHeatmap] candidate {idx + 1}/{max_iter}",
+                    f"{param_values} - score: {score:.3f}",
+                )
+
+    def plot(
+        self,
+        ax: Optional[plt.Axes] = None,
+        cmap: ListedColormap = "RdYlGn",
+        log_xticks: bool = True,
+        log_yticks: bool = True,
+        annotate: bool = True,
+        show: bool = False,
+    ) -> plt.Axes:
+        if ax is None:
             _, ax = plt.subplots()
             show = True
-        
+
         cax = ax.imshow(self.scores, cmap=cmap)
         ax.figure.colorbar(cax)
-        
+
         self._evaluate()
         if annotate:
             for i in range(self.sizes_[0]):
                 for j in range(self.sizes_[1]):
                     score = self.scores[i, j]
-                    ax.text(j, i, f'{score:.2f}', 
-                            ha='center', 
-                            va='center', 
-                            color='white',
-                            alpha=0.7)
-        
+                    ax.text(
+                        j,
+                        i,
+                        f"{score:.2f}",
+                        ha="center",
+                        va="center",
+                        color="white",
+                        alpha=0.7,
+                    )
+
         ax.set_xticks(range(self.sizes_[0]), np.round(self.values_[0], 2))
         ax.set_yticks(range(self.sizes_[1]), np.round(self.values_[1], 2))
-        
+
         if log_xticks:
-            ax.set_xticklabels([r'$10^{' + f'{np.log10(n):.1f}' + r'}$' 
-                                for n in self.values_[0]])
+            ax.set_xticklabels(
+                [r"$10^{" + f"{np.log10(n):.1f}" + r"}$" for n in self.values_[0]]
+            )
         if log_yticks:
-            ax.set_yticklabels([r'$10^{' + f'{np.log10(n):.1f}' + r'}$' 
-                                for n in self.values_[1]])
-        
+            ax.set_yticklabels(
+                [r"$10^{" + f"{np.log10(n):.1f}" + r"}$" for n in self.values_[1]]
+            )
+
         ax.set_xlabel(self.names_[1])
         ax.set_ylabel(self.names_[0])
-        
+
         ax.set_title("Validation Heatmap")
         ax.figure.tight_layout()
-        
-        if show: plt.show()
+
+        if show:
+            plt.show()
         return ax
 
 
 class InertiaPlot(Visualizer):
-    
     """
-    An inertia plot in clustering visualizes the inertia against the number of 
-    clusters, helping to determine the optimal number of clusters by identifying 
-    the "elbow" point where the rate of decrease in inertia sharply changes. 
-    It reflects how well clusters are compact and separated, with lower inertia 
-    indicating better clustering. The plot aids in applying the elbow method for 
-    selecting a reasonable number of clusters in algorithms like K-means. The 
-    goal is to choose the number of clusters where inertia begins to decrease 
+    An inertia plot in clustering visualizes the inertia against the number of
+    clusters, helping to determine the optimal number of clusters by identifying
+    the "elbow" point where the rate of decrease in inertia sharply changes.
+    It reflects how well clusters are compact and separated, with lower inertia
+    indicating better clustering. The plot aids in applying the elbow method for
+    selecting a reasonable number of clusters in algorithms like K-means. The
+    goal is to choose the number of clusters where inertia begins to decrease
     more slowly.
-    
+
     Parameters
     ----------
     `inertia_list` : List of inertia values for various cluster sizes
     `n_clusters_list` : List of the number of clusters
-    
+
     Examples
     --------
     ```py
     inertia_list = []
     for i in range(2, 10):
         km = KMeansClustering(n_clusters=i)
         km.fit(data)
-        
+
         inr = Inertia.score(data, km.centroids)
         inertia_list.append(inr)
-    
+
     inr_plot = InertiaPlot(inertia_list=inertia_list,
                            n_clusters_list=list(range(2, 10)))
     inr_plot.plot()
     >>> plt.Axes
     ```
     """
-    
-    def __init__(self, 
-                 inertia_list: List[float],
-                 n_clusters_list: List[int]) -> None:
+
+    def __init__(self, inertia_list: List[float], n_clusters_list: List[int]) -> None:
         self.inertia_list = inertia_list
         self.n_clusters_list = n_clusters_list
-    
+
     def _derivate_inertia(self) -> Vector:
         deriv = [0.0]
         for i in range(1, len(self.n_clusters_list) - 1):
             df = (self.inertia_list[i - 1] - self.inertia_list[i + 1]) / 2
             deriv.append(df)
-        
+
         deriv.append(0.0)
         return np.abs(deriv)
-    
-    def plot(self, 
-             ax: Optional[plt.Axes] = None,
-             marker: str = 'o', 
-             linestyle: str = '-', 
-             show: bool = False) -> None:
+
+    def plot(
+        self,
+        ax: Optional[plt.Axes] = None,
+        marker: str = "o",
+        linestyle: str = "-",
+        show: bool = False,
+    ) -> None:
         if ax is None:
             _, ax = plt.subplots()
             show = True
-        
-        ax.plot(self.n_clusters_list, self.inertia_list, 
-                marker=marker,
-                linestyle=linestyle,
-                label='Inertia')
-        
-        ax.plot(self.n_clusters_list, self._derivate_inertia(),
-                marker=marker,
-                linestyle=linestyle,
-                label='Absolute Derivative')
-        
-        ax.set_title('Inertia Plot')
-        ax.set_xlabel('Number of Clusters')
-        ax.set_ylabel('Inertia / Deriv. of Inertia')
+
+        ax.plot(
+            self.n_clusters_list,
+            self.inertia_list,
+            marker=marker,
+            linestyle=linestyle,
+            label="Inertia",
+        )
+
+        ax.plot(
+            self.n_clusters_list,
+            self._derivate_inertia(),
+            marker=marker,
+            linestyle=linestyle,
+            label="Absolute Derivative",
+        )
+
+        best_idx = np.argmax(self._derivate_inertia())
+        best_n_clusters = self.n_clusters_list[best_idx]
+        ax.axvspan(
+            best_n_clusters - 0.25,
+            best_n_clusters + 0.25,
+            color="orange",
+            alpha=0.2,
+            label="Best Number of Clusters",
+        )
+
+        ax.set_title("Inertia Plot")
+        ax.set_xlabel("Number of Clusters")
+        ax.set_ylabel("Inertia / Deriv. of Inertia")
         ax.legend()
         ax.grid()
         ax.figure.tight_layout()
-        
-        if show: plt.show()
-        return ax
 
+        if show:
+            plt.show()
+        return ax
```

### Comparing `luma-ml-0.6.4/luma_ml.egg-info/PKG-INFO` & `luma-ml-0.6.5/luma_ml.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luma-ml
-Version: 0.6.4
+Version: 0.6.5
 Summary: A Comprehensive Python Module for Machine Learning and Data Science
 Home-page: https://github.com/ChanLumerico/LUMA
 Author: ChanLumerico
 Author-email: greensox284@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -18,16 +18,18 @@
         <a href="https://lumerico284.notion.site/LUMA-a467e4a9e885498f87b49c952d0abecd?pvs=74">
             <img src="https://github.com/ChanLumerico/luma/raw/main/others/luma.png" alt="logo" width="75" height="75">
         </a>
         <h1 class="main-title">LUMA</h1>
         <p class="subtitle">A Comprehensive Python Module for Machine Learning and Data Science</p>
         <img alt="pypi-version" src="https://img.shields.io/pypi/v/luma-ml?logo=python&logoColor=white&color=blue">
         <img alt="pypi-downloads" src="https://img.shields.io/pypi/dm/luma-ml">
-        <img src="https://img.shields.io/badge/total downloads-4.0k-red">
+        <img src="https://img.shields.io/badge/total downloads-4.3k-red">
         <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/ChanLumerico/luma?color=yellow">
+        <img alt="Code Style" src="https://img.shields.io/badge/code%20style-black-000000.svg">
+        <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/ChanLumerico/luma?color=purple">
         <div class="module">
             <h3 class="module-header">Submodules</h3>
             <table>
                 <tr>
                     <th>Name</th>
                     <th>Description</th>
                 </tr>
@@ -102,19 +104,19 @@
         </div>
         <h2></h2>
         <div class="others">
             <h3 class="others-header">Others</h3>
             <table>
                 <tr>
                     <td>Latest Version</td>
-                    <td>0.6.4</td>
+                    <td>0.6.5</td>
                 </tr>
                 <tr>
                     <td>Lines of Code</td>
-                    <td>~14K</td>
+                    <td>~15.7K</td>
                 </tr>
                 <tr>
                     <td>Requirement</td>
                     <td>Python 3.10 or later</td>
                 </tr>
                 <tr>
                     <td>Dependencies</td>
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: luma-ml Version: 0.6.4 Summary: A Comprehensive
+Metadata-Version: 2.1 Name: luma-ml Version: 0.6.5 Summary: A Comprehensive
 Python Module for Machine Learning and Data Science Home-page: https://
 github.com/ChanLumerico/LUMA Author: ChanLumerico Author-email:
 greensox284@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE
 _[_l_o_g_o_]
 ************ LLUUMMAA ************
 A Comprehensive Python Module for Machine Learning and Data Science
 [pypi-version][pypi-downloads][https://img.shields.io/badge/total downloads-
-4.0k-red][GitHub last commit]
+4.3k-red][GitHub last commit][Code Style][GitHub code size in bytes]
 ******** SSuubbmmoodduulleess ********
 NNaammee                 DDeessccrriippttiioonn
 luma.classifier      Toolkit for classification models including various
                      algorithms.
 luma.clustering      Focuses on unsupervised learning and clustering
                      algorithms.
 luma.core            Foundational backbone providing essential data structures
@@ -31,12 +31,12 @@
 luma.reduction       Dimensionality reduction techniques for high-dimensional
                      datasets.
 luma.regressor       Comprehensive range of regression algorithms.
 luma.visual          Tools for model visualization and data plotting.
 ******** SSttrruuccttuurree ********
 [structure]
 ******** OOtthheerrss ********
-Latest Version 0.6.4
-Lines of Code  ~14K
+Latest Version 0.6.5
+Lines of Code  ~15.7K
 Requirement    Python 3.10 or later
 Dependencies   NumPy, SciPy, Pandas, Matplotlib, Seaborn
 Documentation  _L_U_M_A_ _N_o_t_i_o_n_ _D_o_c_u_m_e_n_t
```

### Comparing `luma-ml-0.6.4/luma_ml.egg-info/SOURCES.txt` & `luma-ml-0.6.5/luma_ml.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -56,8 +56,9 @@
 luma/visual/eda.py
 luma/visual/evaluation.py
 luma_ml.egg-info/PKG-INFO
 luma_ml.egg-info/SOURCES.txt
 luma_ml.egg-info/dependency_links.txt
 luma_ml.egg-info/requires.txt
 luma_ml.egg-info/top_level.txt
-test/__local__.py
+test/__local__.py
+test/_docs.py
```

### Comparing `luma-ml-0.6.4/setup.py` & `luma-ml-0.6.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,29 +2,23 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="luma-ml",
-    version='0.6.4',
+    version="0.6.5",
     author="ChanLumerico",
     author_email="greensox284@gmail.com",
     description="A Comprehensive Python Module for Machine Learning and Data Science",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ChanLumerico/LUMA",
     packages=setuptools.find_namespace_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.10',
-    install_requires=[
-        'numpy',
-        'scipy',
-        'pandas',
-        'matplotlib',
-        'seaborn'
-    ]
+    python_requires=">=3.10",
+    install_requires=["numpy", "scipy", "pandas", "matplotlib", "seaborn"],
 )
```

