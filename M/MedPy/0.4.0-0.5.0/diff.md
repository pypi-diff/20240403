# Comparing `tmp/MedPy-0.4.0.tar.gz` & `tmp/MedPy-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/MedPy-0.4.0.tar", last modified: Thu Feb 14 17:10:41 2019, max compression
+gzip compressed data, was "MedPy-0.5.0.tar", last modified: Wed Apr  3 14:43:39 2024, max compression
```

## Comparing `MedPy-0.4.0.tar` & `MedPy-0.5.0.tar`

### file list

```diff
@@ -1,110 +1,111 @@
-drwxr-xr-x   0 administrator  (1001) administrator  (1001)        0 2019-02-14 17:10:41.000000 MedPy-0.4.0/
-drwxr-xr-x   0 administrator  (1001) administrator  (1001)        0 2019-02-14 17:10:41.000000 MedPy-0.4.0/lib/
-drwxr-xr-x   0 administrator  (1001) administrator  (1001)        0 2019-02-14 17:10:41.000000 MedPy-0.4.0/lib/maxflow/
-drwxr-xr-x   0 administrator  (1001) administrator  (1001)        0 2019-02-14 17:10:41.000000 MedPy-0.4.0/lib/maxflow/src/
--rw-r--r--   0 administrator  (1001) administrator  (1001)      856 2018-11-22 16:25:39.000000 MedPy-0.4.0/lib/maxflow/src/pythongraph.h
--rw-r--r--   0 administrator  (1001) administrator  (1001)     7220 2018-11-22 16:25:39.000000 MedPy-0.4.0/lib/maxflow/src/block.h
--rw-r--r--   0 administrator  (1001) administrator  (1001)    14887 2018-11-22 16:25:39.000000 MedPy-0.4.0/lib/maxflow/src/maxflow.cpp
--rw-r--r--   0 administrator  (1001) administrator  (1001)    20050 2018-11-22 16:25:39.000000 MedPy-0.4.0/lib/maxflow/src/graph.h
--rw-r--r--   0 administrator  (1001) administrator  (1001)      394 2018-11-22 16:25:39.000000 MedPy-0.4.0/lib/maxflow/src/instances.inc
--rw-r--r--   0 administrator  (1001) administrator  (1001)    11266 2018-11-22 16:25:39.000000 MedPy-0.4.0/lib/maxflow/src/wrapper.cpp
--rw-r--r--   0 administrator  (1001) administrator  (1001)     2936 2018-11-22 16:25:39.000000 MedPy-0.4.0/lib/maxflow/src/graph.cpp
-drwxr-xr-x   0 administrator  (1001) administrator  (1001)        0 2019-02-14 17:10:41.000000 MedPy-0.4.0/MedPy.egg-info/
--rw-r--r--   0 administrator  (1001) administrator  (1001)     2497 2019-02-14 17:10:41.000000 MedPy-0.4.0/MedPy.egg-info/SOURCES.txt
--rw-r--r--   0 administrator  (1001) administrator  (1001)        1 2019-02-14 17:10:41.000000 MedPy-0.4.0/MedPy.egg-info/dependency_links.txt
--rw-r--r--   0 administrator  (1001) administrator  (1001)     8332 2019-02-14 17:10:41.000000 MedPy-0.4.0/MedPy.egg-info/PKG-INFO
--rw-r--r--   0 administrator  (1001) administrator  (1001)        6 2019-02-14 17:10:41.000000 MedPy-0.4.0/MedPy.egg-info/top_level.txt
--rw-r--r--   0 administrator  (1001) administrator  (1001)       44 2019-02-14 17:10:41.000000 MedPy-0.4.0/MedPy.egg-info/requires.txt
--rwxr-xr-x   0 administrator  (1001) administrator  (1001)     7340 2019-02-14 17:04:47.000000 MedPy-0.4.0/setup.py
--rw-r--r--   0 administrator  (1001) administrator  (1001)      176 2019-02-14 16:53:45.000000 MedPy-0.4.0/MANIFEST.in
--rw-r--r--   0 administrator  (1001) administrator  (1001)       38 2019-02-14 17:10:41.000000 MedPy-0.4.0/setup.cfg
-drwxr-xr-x   0 administrator  (1001) administrator  (1001)        0 2019-02-14 17:10:41.000000 MedPy-0.4.0/medpy/
-drwxr-xr-x   0 administrator  (1001) administrator  (1001)        0 2019-02-14 17:10:41.000000 MedPy-0.4.0/medpy/metric/
--rw-r--r--   0 administrator  (1001) administrator  (1001)     3651 2018-11-22 16:25:39.000000 MedPy-0.4.0/medpy/metric/__init__.py
--rw-r--r--   0 administrator  (1001) administrator  (1001)    33216 2018-11-22 16:25:39.000000 MedPy-0.4.0/medpy/metric/histogram.py
--rw-r--r--   0 administrator  (1001) administrator  (1001)     4179 2018-11-22 16:25:39.000000 MedPy-0.4.0/medpy/metric/image.py
--rw-r--r--   0 administrator  (1001) administrator  (1001)    44737 2019-01-31 15:32:57.000000 MedPy-0.4.0/medpy/metric/binary.py
-drwxr-xr-x   0 administrator  (1001) administrator  (1001)        0 2019-02-14 17:10:41.000000 MedPy-0.4.0/medpy/graphcut/
--rw-r--r--   0 administrator  (1001) administrator  (1001)     2635 2019-01-31 15:32:57.000000 MedPy-0.4.0/medpy/graphcut/write.py
--rw-r--r--   0 administrator  (1001) administrator  (1001)     7441 2018-11-22 16:25:39.000000 MedPy-0.4.0/medpy/graphcut/__init__.py
--rw-r--r--   0 administrator  (1001) administrator  (1001)    18872 2018-11-22 16:25:39.000000 MedPy-0.4.0/medpy/graphcut/energy_label.py
--rw-r--r--   0 administrator  (1001) administrator  (1001)    16327 2018-11-22 16:25:39.000000 MedPy-0.4.0/medpy/graphcut/generate.py
--rw-r--r--   0 administrator  (1001) administrator  (1001)    27379 2018-11-22 16:25:39.000000 MedPy-0.4.0/medpy/graphcut/energy_voxel.py
--rw-r--r--   0 administrator  (1001) administrator  (1001)    10552 2019-01-31 15:32:57.000000 MedPy-0.4.0/medpy/graphcut/wrapper.py
--rw-r--r--   0 administrator  (1001) administrator  (1001)    19822 2019-01-31 15:32:57.000000 MedPy-0.4.0/medpy/graphcut/graph.py
-drwxr-xr-x   0 administrator  (1001) administrator  (1001)        0 2019-02-14 17:10:41.000000 MedPy-0.4.0/medpy/features/
--rw-r--r--   0 administrator  (1001) administrator  (1001)     6483 2018-11-22 16:25:39.000000 MedPy-0.4.0/medpy/features/__init__.py
--rw-r--r--   0 administrator  (1001) administrator  (1001)    19488 2018-11-22 16:25:39.000000 MedPy-0.4.0/medpy/features/histogram.py
--rw-r--r--   0 administrator  (1001) administrator  (1001)    33408 2018-11-22 16:34:15.000000 MedPy-0.4.0/medpy/features/intensity.py
--rw-r--r--   0 administrator  (1001) administrator  (1001)     6312 2018-11-22 16:25:39.000000 MedPy-0.4.0/medpy/features/utilities.py
--rw-r--r--   0 administrator  (1001) administrator  (1001)    12601 2018-11-22 16:25:39.000000 MedPy-0.4.0/medpy/features/texture.py
-drwxr-xr-x   0 administrator  (1001) administrator  (1001)        0 2019-02-14 17:10:41.000000 MedPy-0.4.0/medpy/filter/
--rw-r--r--   0 administrator  (1001) administrator  (1001)     7547 2018-11-22 16:34:42.000000 MedPy-0.4.0/medpy/filter/noise.py
--rw-r--r--   0 administrator  (1001) administrator  (1001)    24685 2018-11-22 16:25:39.000000 MedPy-0.4.0/medpy/filter/IntensityRangeStandardization.py
--rw-r--r--   0 administrator  (1001) administrator  (1001)     3970 2018-11-22 16:25:39.000000 MedPy-0.4.0/medpy/filter/__init__.py
--rw-r--r--   0 administrator  (1001) administrator  (1001)     5863 2018-11-22 16:25:39.000000 MedPy-0.4.0/medpy/filter/smoothing.py
--rw-r--r--   0 administrator  (1001) administrator  (1001)    19601 2018-11-22 16:34:25.000000 MedPy-0.4.0/medpy/filter/image.py
--rw-r--r--   0 administrator  (1001) administrator  (1001)     4889 2018-11-22 16:25:39.000000 MedPy-0.4.0/medpy/filter/binary.py
--rw-r--r--   0 administrator  (1001) administrator  (1001)     9378 2018-11-22 16:25:39.000000 MedPy-0.4.0/medpy/filter/houghtransform.py
--rw-r--r--   0 administrator  (1001) administrator  (1001)    10864 2018-11-22 16:34:59.000000 MedPy-0.4.0/medpy/filter/utilities.py
--rw-r--r--   0 administrator  (1001) administrator  (1001)     5961 2019-01-31 15:32:57.000000 MedPy-0.4.0/medpy/filter/label.py
-drwxr-xr-x   0 administrator  (1001) administrator  (1001)        0 2019-02-14 17:10:41.000000 MedPy-0.4.0/medpy/io/
--rw-r--r--   0 administrator  (1001) administrator  (1001)     1756 2019-02-14 16:44:00.000000 MedPy-0.4.0/medpy/io/__init__.py
--rw-r--r--   0 administrator  (1001) administrator  (1001)     4315 2019-02-14 16:44:00.000000 MedPy-0.4.0/medpy/io/save.py
--rw-r--r--   0 administrator  (1001) administrator  (1001)    10725 2019-02-14 16:44:00.000000 MedPy-0.4.0/medpy/io/header.py
--rw-r--r--   0 administrator  (1001) administrator  (1001)     4421 2019-02-14 16:44:00.000000 MedPy-0.4.0/medpy/io/load.py
--rw-r--r--   0 administrator  (1001) administrator  (1001)     1001 2018-11-22 16:25:39.000000 MedPy-0.4.0/medpy/__init__.py
-drwxr-xr-x   0 administrator  (1001) administrator  (1001)        0 2019-02-14 17:10:41.000000 MedPy-0.4.0/medpy/core/
--rw-r--r--   0 administrator  (1001) administrator  (1001)     1759 2018-11-22 16:25:39.000000 MedPy-0.4.0/medpy/core/exceptions.py
--rw-r--r--   0 administrator  (1001) administrator  (1001)     1978 2018-11-22 16:25:39.000000 MedPy-0.4.0/medpy/core/__init__.py
--rw-r--r--   0 administrator  (1001) administrator  (1001)     4862 2018-11-22 16:25:39.000000 MedPy-0.4.0/medpy/core/logger.py
-drwxr-xr-x   0 administrator  (1001) administrator  (1001)        0 2019-02-14 17:10:41.000000 MedPy-0.4.0/medpy/utilities/
--rw-r--r--   0 administrator  (1001) administrator  (1001)     7089 2018-11-22 16:25:39.000000 MedPy-0.4.0/medpy/utilities/argparseu.py
--rw-r--r--   0 administrator  (1001) administrator  (1001)     1103 2019-02-14 16:44:00.000000 MedPy-0.4.0/medpy/utilities/__init__.py
--rw-r--r--   0 administrator  (1001) administrator  (1001)     1572 2019-02-14 16:44:00.000000 MedPy-0.4.0/README.md
--rw-r--r--   0 administrator  (1001) administrator  (1001)     5765 2019-02-14 16:44:00.000000 MedPy-0.4.0/README_PYPI.md
--rw-r--r--   0 administrator  (1001) administrator  (1001)    35147 2018-11-22 16:25:39.000000 MedPy-0.4.0/LICENSE.txt
--rw-r--r--   0 administrator  (1001) administrator  (1001)      873 2019-02-14 16:44:00.000000 MedPy-0.4.0/CHANGES.txt
-drwxr-xr-x   0 administrator  (1001) administrator  (1001)        0 2019-02-14 17:10:41.000000 MedPy-0.4.0/bin/
--rwxr-xr-x   0 administrator  (1001) administrator  (1001)     4404 2018-11-22 16:25:39.000000 MedPy-0.4.0/bin/medpy_intersection.py
--rwxr-xr-x   0 administrator  (1001) administrator  (1001)     2932 2018-11-22 16:25:39.000000 MedPy-0.4.0/bin/medpy_create_empty_volume_by_example.py
--rwxr-xr-x   0 administrator  (1001) administrator  (1001)     9015 2019-01-31 15:32:57.000000 MedPy-0.4.0/bin/medpy_graphcut_label_bgreduced.py
--rwxr-xr-x   0 administrator  (1001) administrator  (1001)     5300 2018-11-22 16:25:39.000000 MedPy-0.4.0/bin/medpy_zoom_image.py
--rwxr-xr-x   0 administrator  (1001) administrator  (1001)     5563 2018-11-22 16:25:39.000000 MedPy-0.4.0/bin/medpy_extract_contour.py
--rwxr-xr-x   0 administrator  (1001) administrator  (1001)    10674 2018-11-22 16:25:39.000000 MedPy-0.4.0/bin/medpy_binary_resampling.py
--rwxr-xr-x   0 administrator  (1001) administrator  (1001)     4377 2019-02-14 16:44:00.000000 MedPy-0.4.0/bin/medpy_watershed.py
--rwxr-xr-x   0 administrator  (1001) administrator  (1001)     7347 2019-01-31 15:32:57.000000 MedPy-0.4.0/bin/medpy_graphcut_label.py
--rwxr-xr-x   0 administrator  (1001) administrator  (1001)     3041 2019-02-14 16:44:00.000000 MedPy-0.4.0/bin/medpy_dicom_slices_to_volume.py
--rwxr-xr-x   0 administrator  (1001) administrator  (1001)     8900 2019-01-31 15:32:57.000000 MedPy-0.4.0/bin/medpy_graphcut_label_w_regional.py
--rwxr-xr-x   0 administrator  (1001) administrator  (1001)     4097 2018-11-22 16:25:39.000000 MedPy-0.4.0/bin/medpy_anisotropic_diffusion.py
--rwxr-xr-x   0 administrator  (1001) administrator  (1001)     4564 2019-01-31 15:32:57.000000 MedPy-0.4.0/bin/medpy_join_masks.py
--rwxr-xr-x   0 administrator  (1001) administrator  (1001)     4295 2018-11-22 16:25:39.000000 MedPy-0.4.0/bin/medpy_fit_into_shape.py
--rwxr-xr-x   0 administrator  (1001) administrator  (1001)     3677 2019-01-31 15:32:57.000000 MedPy-0.4.0/bin/medpy_extract_min_max.py
--rwxr-xr-x   0 administrator  (1001) administrator  (1001)     3335 2019-01-31 15:32:57.000000 MedPy-0.4.0/bin/medpy_info.py
--rwxr-xr-x   0 administrator  (1001) administrator  (1001)     4874 2018-11-22 16:25:39.000000 MedPy-0.4.0/bin/medpy_morphology.py
--rwxr-xr-x   0 administrator  (1001) administrator  (1001)     4593 2018-11-22 16:25:39.000000 MedPy-0.4.0/bin/medpy_shrink_image.py
--rwxr-xr-x   0 administrator  (1001) administrator  (1001)     9654 2018-11-22 16:25:39.000000 MedPy-0.4.0/bin/medpy_intensity_range_standardization.py
--rwxr-xr-x   0 administrator  (1001) administrator  (1001)     4395 2019-02-14 16:44:00.000000 MedPy-0.4.0/bin/medpy_label_fit_to_mask.py
--rwxr-xr-x   0 administrator  (1001) administrator  (1001)     6497 2019-01-31 15:32:57.000000 MedPy-0.4.0/bin/medpy_extract_sub_volume_by_example.py
--rwxr-xr-x   0 administrator  (1001) administrator  (1001)     8628 2018-11-22 16:25:39.000000 MedPy-0.4.0/bin/medpy_graphcut_voxel.py
--rwxr-xr-x   0 administrator  (1001) administrator  (1001)     3327 2018-11-22 16:25:39.000000 MedPy-0.4.0/bin/medpy_merge.py
--rwxr-xr-x   0 administrator  (1001) administrator  (1001)     4572 2018-11-22 16:25:39.000000 MedPy-0.4.0/bin/medpy_resample.py
--rwxr-xr-x   0 administrator  (1001) administrator  (1001)     4444 2019-02-14 16:44:00.000000 MedPy-0.4.0/bin/medpy_split_xd_to_xminus1d.py
--rwxr-xr-x   0 administrator  (1001) administrator  (1001)     3675 2019-01-31 15:32:57.000000 MedPy-0.4.0/bin/medpy_diff.py
--rwxr-xr-x   0 administrator  (1001) administrator  (1001)     7024 2018-11-22 16:25:39.000000 MedPy-0.4.0/bin/medpy_apparent_diffusion_coefficient.py
--rwxr-xr-x   0 administrator  (1001) administrator  (1001)     5799 2018-11-22 16:25:39.000000 MedPy-0.4.0/bin/medpy_graphcut_label_wsplit.py
--rwxr-xr-x   0 administrator  (1001) administrator  (1001)     3571 2019-02-14 16:44:00.000000 MedPy-0.4.0/bin/medpy_gradient.py
--rwxr-xr-x   0 administrator  (1001) administrator  (1001)     5753 2018-11-22 16:25:39.000000 MedPy-0.4.0/bin/medpy_extract_sub_volume_auto.py
--rwxr-xr-x   0 administrator  (1001) administrator  (1001)     5903 2019-02-14 16:44:00.000000 MedPy-0.4.0/bin/medpy_label_superimposition.py
--rwxr-xr-x   0 administrator  (1001) administrator  (1001)     8639 2019-01-31 15:32:57.000000 MedPy-0.4.0/bin/medpy_grid.py
--rwxr-xr-x   0 administrator  (1001) administrator  (1001)     5440 2018-11-22 16:25:39.000000 MedPy-0.4.0/bin/medpy_reslice_3d_to_4d.py
--rwxr-xr-x   0 administrator  (1001) administrator  (1001)     3116 2019-01-31 15:32:57.000000 MedPy-0.4.0/bin/medpy_label_count.py
--rwxr-xr-x   0 administrator  (1001) administrator  (1001)     6276 2019-01-31 15:32:57.000000 MedPy-0.4.0/bin/medpy_extract_sub_volume.py
--rwxr-xr-x   0 administrator  (1001) administrator  (1001)     4206 2018-11-22 16:25:39.000000 MedPy-0.4.0/bin/medpy_swap_dimensions.py
--rwxr-xr-x   0 administrator  (1001) administrator  (1001)     2758 2018-11-22 16:25:39.000000 MedPy-0.4.0/bin/medpy_set_pixel_spacing.py
--rwxr-xr-x   0 administrator  (1001) administrator  (1001)     6336 2019-02-14 16:44:00.000000 MedPy-0.4.0/bin/medpy_dicom_to_4D.py
--rwxr-xr-x   0 administrator  (1001) administrator  (1001)     2989 2018-11-22 16:25:39.000000 MedPy-0.4.0/bin/medpy_convert.py
--rwxr-xr-x   0 administrator  (1001) administrator  (1001)     5243 2019-02-14 16:44:00.000000 MedPy-0.4.0/bin/medpy_join_xd_to_xplus1d.py
--rwxr-xr-x   0 administrator  (1001) administrator  (1001)     4970 2019-02-14 16:44:00.000000 MedPy-0.4.0/bin/medpy_stack_sub_volumes.py
--rw-r--r--   0 administrator  (1001) administrator  (1001)      152 2018-11-22 16:25:39.000000 MedPy-0.4.0/requirements-dev.txt
--rw-r--r--   0 administrator  (1001) administrator  (1001)     8332 2019-02-14 17:10:41.000000 MedPy-0.4.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:43:39.456257 MedPy-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-03 14:43:34.000000 MedPy-0.5.0/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-03 14:43:34.000000 MedPy-0.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-03 14:43:34.000000 MedPy-0.5.0/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:43:39.456257 MedPy-0.5.0/MedPy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7512 2024-04-03 14:43:39.000000 MedPy-0.5.0/MedPy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-04-03 14:43:39.000000 MedPy-0.5.0/MedPy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 14:43:39.000000 MedPy-0.5.0/MedPy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-03 14:43:39.000000 MedPy-0.5.0/MedPy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-03 14:43:39.000000 MedPy-0.5.0/MedPy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7512 2024-04-03 14:43:39.456257 MedPy-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-03 14:43:34.000000 MedPy-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-04-03 14:43:34.000000 MedPy-0.5.0/README_PYPI.md
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-03 14:43:34.000000 MedPy-0.5.0/RELEASE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:43:39.448257 MedPy-0.5.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4486 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_anisotropic_diffusion.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7368 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_apparent_diffusion_coefficient.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10766 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_binary_resampling.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3071 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_convert.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2984 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_create_empty_volume_by_example.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3086 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_dicom_slices_to_volume.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6511 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_dicom_to_4D.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3769 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_diff.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6209 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_extract_contour.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3669 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_extract_min_max.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6589 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_extract_sub_volume.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6149 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_extract_sub_volume_auto.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6700 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_extract_sub_volume_by_example.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4225 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_fit_into_shape.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3589 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_gradient.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7371 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_graphcut_label.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9004 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_graphcut_label_bgreduced.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8936 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_graphcut_label_w_regional.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5636 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_graphcut_label_wsplit.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8923 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_graphcut_voxel.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9151 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_grid.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3332 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10440 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_intensity_range_standardization.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4582 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_intersection.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4645 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_join_masks.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5622 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_join_xd_to_xplus1d.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3048 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_label_count.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4521 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_label_fit_to_mask.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6311 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_label_superimposition.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3361 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_merge.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5073 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_morphology.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4721 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_resample.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5650 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_reslice_3d_to_4d.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2771 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_set_pixel_spacing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4676 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_shrink_image.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4587 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_split_xd_to_xminus1d.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5128 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_stack_sub_volumes.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4357 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_swap_dimensions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4492 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_watershed.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5514 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_zoom_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:43:39.436257 MedPy-0.5.0/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:43:39.436257 MedPy-0.5.0/lib/maxflow/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:43:39.448257 MedPy-0.5.0/lib/maxflow/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-03 14:43:34.000000 MedPy-0.5.0/lib/maxflow/src/README
+-rw-r--r--   0 runner    (1001) docker     (127)     7218 2024-04-03 14:43:34.000000 MedPy-0.5.0/lib/maxflow/src/block.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-03 14:43:34.000000 MedPy-0.5.0/lib/maxflow/src/graph.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    20008 2024-04-03 14:43:34.000000 MedPy-0.5.0/lib/maxflow/src/graph.h
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-03 14:43:34.000000 MedPy-0.5.0/lib/maxflow/src/instances.inc
+-rw-r--r--   0 runner    (1001) docker     (127)    14873 2024-04-03 14:43:34.000000 MedPy-0.5.0/lib/maxflow/src/maxflow.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-03 14:43:34.000000 MedPy-0.5.0/lib/maxflow/src/pythongraph.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11263 2024-04-03 14:43:34.000000 MedPy-0.5.0/lib/maxflow/src/wrapper.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:43:39.448257 MedPy-0.5.0/medpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:43:39.448257 MedPy-0.5.0/medpy/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/core/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:43:39.452257 MedPy-0.5.0/medpy/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     7493 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18892 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/features/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34017 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/features/intensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12918 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/features/texture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6138 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/features/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:43:39.452257 MedPy-0.5.0/medpy/filter/
+-rw-r--r--   0 runner    (1001) docker     (127)    24588 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/filter/IntensityRangeStandardization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/filter/binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9622 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/filter/houghtransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19807 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/filter/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/filter/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/filter/noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6120 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/filter/smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11284 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/filter/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:43:39.452257 MedPy-0.5.0/medpy/graphcut/
+-rw-r--r--   0 runner    (1001) docker     (127)     7613 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/graphcut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19015 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/graphcut/energy_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26949 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/graphcut/energy_voxel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16053 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/graphcut/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19756 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/graphcut/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10794 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/graphcut/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/graphcut/write.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:43:39.456257 MedPy-0.5.0/medpy/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/io/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/io/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/io/save.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:43:39.456257 MedPy-0.5.0/medpy/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)     5837 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44679 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/metric/binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32470 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/metric/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/metric/image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:43:39.456257 MedPy-0.5.0/medpy/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7217 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/utilities/argparseu.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 14:43:39.456257 MedPy-0.5.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8243 2024-04-03 14:43:34.000000 MedPy-0.5.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `MedPy-0.4.0/lib/maxflow/src/pythongraph.h` & `MedPy-0.5.0/lib/maxflow/src/pythongraph.h`

 * *Files 0% similar despite different names*

```diff
@@ -17,8 +17,7 @@
 {
 public:
 	Pythongraph(int node_num_max, int edge_num_max) : Graph<captype, tcaptype, flowtype>(node_num_max, edge_num_max, NULL) {};
 	flowtype maxflow() { Graph<captype, tcaptype, flowtype>::maxflow(); };
 	typename Graph<captype, tcaptype, flowtype>::termtype what_segment(int i) { Graph<captype, tcaptype, flowtype>::what_segment(i); };
 };
 #endif
-
```

### Comparing `MedPy-0.4.0/lib/maxflow/src/block.h` & `MedPy-0.5.0/lib/maxflow/src/block.h`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 	}
 
 	delete block;
 
 	...
 
 	DBlock<MyType> *dblock = new DBlock<MyType>(BLOCK_SIZE);
-	
+
 	// adding items
 	for (int i=0; i<sizeof(array); i++)
 	{
 		array[i] = dblock -> New();
 	}
 
 	// deleting items
@@ -261,8 +261,7 @@
 	block_item	*first_free;
 
 	void	(*error_function)(char *);
 };
 
 
 #endif
-
```

### Comparing `MedPy-0.4.0/lib/maxflow/src/maxflow.cpp` & `MedPy-0.5.0/lib/maxflow/src/maxflow.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 	to the end of the second queue and read from
 	the front of the first queue. If the first queue
 	is empty, it is replaced by the second queue
 	(and the second queue becomes empty).
 */
 
 
-template <typename captype, typename tcaptype, typename flowtype> 
+template <typename captype, typename tcaptype, typename flowtype>
 	inline void Graph<captype,tcaptype,flowtype>::set_active(node *i)
 {
 	if (!i->next)
 	{
 		/* it's not in the list yet */
 		if (queue_last[1]) queue_last[1] -> next = i;
 		else               queue_first[1]        = i;
@@ -44,15 +44,15 @@
 }
 
 /*
 	Returns the next active node.
 	If it is connected to the sink, it stays in the list,
 	otherwise it is removed from the list
 */
-template <typename captype, typename tcaptype, typename flowtype> 
+template <typename captype, typename tcaptype, typename flowtype>
 	inline typename Graph<captype,tcaptype,flowtype>::node* Graph<captype,tcaptype,flowtype>::next_active()
 {
 	node *i;
 
 	while ( 1 )
 	{
 		if (!(i=queue_first[0]))
@@ -72,54 +72,54 @@
 		/* a node in the list is active iff it has a parent */
 		if (i->parent) return i;
 	}
 }
 
 /***********************************************************************/
 
-template <typename captype, typename tcaptype, typename flowtype> 
+template <typename captype, typename tcaptype, typename flowtype>
 	inline void Graph<captype,tcaptype,flowtype>::set_orphan_front(node *i)
 {
 	nodeptr *np;
 	i -> parent = ORPHAN;
 	np = nodeptr_block -> New();
 	np -> ptr = i;
 	np -> next = orphan_first;
 	orphan_first = np;
 }
 
-template <typename captype, typename tcaptype, typename flowtype> 
+template <typename captype, typename tcaptype, typename flowtype>
 	inline void Graph<captype,tcaptype,flowtype>::set_orphan_rear(node *i)
 {
 	nodeptr *np;
 	i -> parent = ORPHAN;
 	np = nodeptr_block -> New();
 	np -> ptr = i;
 	if (orphan_last) orphan_last -> next = np;
 	else             orphan_first        = np;
 	orphan_last = np;
 	np -> next = NULL;
 }
 
 /***********************************************************************/
 
-template <typename captype, typename tcaptype, typename flowtype> 
+template <typename captype, typename tcaptype, typename flowtype>
 	inline void Graph<captype,tcaptype,flowtype>::add_to_changed_list(node *i)
 {
 	if (changed_list && !i->is_in_changed_list)
 	{
 		node_id* ptr = changed_list->New();
 		*ptr = (node_id)(i - nodes);
 		i->is_in_changed_list = true;
 	}
 }
 
 /***********************************************************************/
 
-template <typename captype, typename tcaptype, typename flowtype> 
+template <typename captype, typename tcaptype, typename flowtype>
 	void Graph<captype,tcaptype,flowtype>::maxflow_init()
 {
 	node *i;
 
 	queue_first[0] = queue_last[0] = NULL;
 	queue_first[1] = queue_last[1] = NULL;
 	orphan_first = NULL;
@@ -151,15 +151,15 @@
 		else
 		{
 			i -> parent = NULL;
 		}
 	}
 }
 
-template <typename captype, typename tcaptype, typename flowtype> 
+template <typename captype, typename tcaptype, typename flowtype>
 	void Graph<captype,tcaptype,flowtype>::maxflow_reuse_trees_init()
 {
 	node* i;
 	node* j;
 	node* queue = queue_first[1];
 	arc* a;
 	nodeptr* np;
@@ -236,15 +236,15 @@
 		else            process_source_orphan(i);
 	}
 	/* adoption end */
 
 	//test_consistency();
 }
 
-template <typename captype, typename tcaptype, typename flowtype> 
+template <typename captype, typename tcaptype, typename flowtype>
 	void Graph<captype,tcaptype,flowtype>::augment(arc *middle_arc)
 {
 	node *i;
 	arc *a;
 	tcaptype bottleneck;
 
 
@@ -308,15 +308,15 @@
 
 
 	flow += bottleneck;
 }
 
 /***********************************************************************/
 
-template <typename captype, typename tcaptype, typename flowtype> 
+template <typename captype, typename tcaptype, typename flowtype>
 	void Graph<captype,tcaptype,flowtype>::process_source_orphan(node *i)
 {
 	node *j;
 	arc *a0, *a0_min = NULL, *a;
 	int d, d_min = INFINITE_D;
 
 	/* trying to find a new parent */
@@ -385,15 +385,15 @@
 					set_orphan_rear(j); // add j to the end of the adoption list
 				}
 			}
 		}
 	}
 }
 
-template <typename captype, typename tcaptype, typename flowtype> 
+template <typename captype, typename tcaptype, typename flowtype>
 	void Graph<captype,tcaptype,flowtype>::process_sink_orphan(node *i)
 {
 	node *j;
 	arc *a0, *a0_min = NULL, *a;
 	int d, d_min = INFINITE_D;
 
 	/* trying to find a new parent */
@@ -464,15 +464,15 @@
 			}
 		}
 	}
 }
 
 /***********************************************************************/
 
-template <typename captype, typename tcaptype, typename flowtype> 
+template <typename captype, typename tcaptype, typename flowtype>
 	flowtype Graph<captype,tcaptype,flowtype>::maxflow(bool reuse_trees, Block<node_id>* _changed_list)
 {
 	node *i, *j, *current_node = NULL;
 	arc *a;
 	nodeptr *np, *np_next;
 
 	if (!nodeptr_block)
@@ -591,26 +591,26 @@
 		}
 		else current_node = NULL;
 	}
 	// test_consistency();
 
 	if (!reuse_trees || (maxflow_iteration % 64) == 0)
 	{
-		delete nodeptr_block; 
-		nodeptr_block = NULL; 
+		delete nodeptr_block;
+		nodeptr_block = NULL;
 	}
 
 	maxflow_iteration ++;
 	return flow;
 }
 
 /***********************************************************************/
 
 
-template <typename captype, typename tcaptype, typename flowtype> 
+template <typename captype, typename tcaptype, typename flowtype>
 	void Graph<captype,tcaptype,flowtype>::test_consistency(node* current_node)
 {
 	node *i;
 	arc *a;
 	int r;
 	int num1 = 0, num2 = 0;
```

### Comparing `MedPy-0.4.0/lib/maxflow/src/graph.h` & `MedPy-0.5.0/lib/maxflow/src/graph.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 /* graph.h */
 /*
 	This software library implements the maxflow algorithm
 	described in
 
 		"An Experimental Comparison of Min-Cut/Max-Flow Algorithms for Energy Minimization in Vision."
 		Yuri Boykov and Vladimir Kolmogorov.
-		In IEEE Transactions on Pattern Analysis and Machine Intelligence (PAMI), 
+		In IEEE Transactions on Pattern Analysis and Machine Intelligence (PAMI),
 		September 2004
 
 	This algorithm was developed by Yuri Boykov and Vladimir Kolmogorov
 	at Siemens Corporate Research. To make it available for public use,
 	it was later reimplemented by Vladimir Kolmogorov based on open publications.
 
 	If you use this software for research purposes, you should cite
@@ -54,47 +54,47 @@
 template <typename captype, typename tcaptype, typename flowtype> class Graph
 {
 public:
 	typedef enum
 	{
 		SOURCE	= 0,
 		SINK	= 1
-	} termtype; // terminals 
+	} termtype; // terminals
 	typedef int node_id;
 
 	/////////////////////////////////////////////////////////////////////////
 	//                     BASIC INTERFACE FUNCTIONS                       //
     //              (should be enough for most applications)               //
 	/////////////////////////////////////////////////////////////////////////
 
-	// Constructor. 
+	// Constructor.
 	// The first argument gives an estimate of the maximum number of nodes that can be added
 	// to the graph, and the second argument is an estimate of the maximum number of edges.
-	// The last (optional) argument is the pointer to the function which will be called 
-	// if an error occurs; an error message is passed to this function. 
+	// The last (optional) argument is the pointer to the function which will be called
+	// if an error occurs; an error message is passed to this function.
 	// If this argument is omitted, exit(1) will be called.
 	//
-	// IMPORTANT: It is possible to add more nodes to the graph than node_num_max 
-	// (and node_num_max can be zero). However, if the count is exceeded, then 
-	// the internal memory is reallocated (increased by 50%) which is expensive. 
+	// IMPORTANT: It is possible to add more nodes to the graph than node_num_max
+	// (and node_num_max can be zero). However, if the count is exceeded, then
+	// the internal memory is reallocated (increased by 50%) which is expensive.
 	// Also, temporarily the amount of allocated memory would be more than twice than needed.
 	// Similarly for edges.
 	// If you wish to avoid this overhead, you can download version 2.2, where nodes and edges are stored in blocks.
 	Graph(int node_num_max, int edge_num_max, void (*err_function)(char *) = NULL);
 
 	// Destructor
 	~Graph();
 
-	// Adds node(s) to the graph. By default, one node is added (num=1); then first call returns 0, second call returns 1, and so on. 
+	// Adds node(s) to the graph. By default, one node is added (num=1); then first call returns 0, second call returns 1, and so on.
 	// If num>1, then several nodes are added, and node_id of the first one is returned.
-	// IMPORTANT: see note about the constructor 
+	// IMPORTANT: see note about the constructor
 	node_id add_node(int num = 1);
 
 	// Adds a bidirectional edge between 'i' and 'j' with the weights 'cap' and 'rev_cap'.
-	// IMPORTANT: see note about the constructor 
+	// IMPORTANT: see note about the constructor
 	// NOTE: One call to this function adds two arcs (i->j and j->i) to the graph. But in
 	// the sense of the memory allocation passed to the constructor, these count as one
 	// single edge!
 	// NOTE: a repeated call to this function adds an additional edge (i.e. two arcs i->j
 	// and j->i) to the graph. In the sense of the max-flow/min-cut computation, this
 	// works as if the new capacity would have been added to the old one. But in the
 	// sense of memory allocation, this counts as an additional edge!
@@ -151,16 +151,16 @@
 
 public:
 
 	////////////////////////////
 	// 1. Reallocating graph. //
 	////////////////////////////
 
-	// Removes all nodes and edges. 
-	// After that functions add_node() and add_edge() must be called again. 
+	// Removes all nodes and edges.
+	// After that functions add_node() and add_edge() must be called again.
 	//
 	// Advantage compared to deleting Graph and allocating it again:
 	// no calls to delete/new (which could be quite slow).
 	//
 	// If the graph structure stays the same, then an alternative
 	// is to go through all nodes/edges and set new residual capacities
 	// (see functions below).
@@ -191,46 +191,46 @@
 	void get_arc_ends(arc_id a, node_id& i, node_id& j); // returns i,j to that a = i->j
 
 	///////////////////////////////////////////////////
 	// 3. Functions for reading residual capacities. //
 	///////////////////////////////////////////////////
 
 	// returns residual capacity of SOURCE->i minus residual capacity of i->SINK
-	tcaptype get_trcap(node_id i); 
+	tcaptype get_trcap(node_id i);
 	// returns residual capacity of arc a
 	captype get_rcap(arc* a);
 
 	/////////////////////////////////////////////////////////////////
 	// 4. Functions for setting residual capacities.               //
 	//    NOTE: If these functions are used, the value of the flow //
 	//    returned by maxflow() will not be valid!                 //
 	/////////////////////////////////////////////////////////////////
 
-	void set_trcap(node_id i, tcaptype trcap); 
+	void set_trcap(node_id i, tcaptype trcap);
 	void set_rcap(arc* a, captype rcap);
 
 	////////////////////////////////////////////////////////////////////
 	// 5. Functions related to reusing trees & list of changed nodes. //
 	////////////////////////////////////////////////////////////////////
 
 	// If flag reuse_trees is true while calling maxflow(), then search trees
-	// are reused from previous maxflow computation. 
+	// are reused from previous maxflow computation.
 	// In this case before calling maxflow() the user must
 	// specify which parts of the graph have changed by calling mark_node():
 	//   add_tweights(i),set_trcap(i)    => call mark_node(i)
 	//   add_edge(i,j),set_rcap(a)       => call mark_node(i); mark_node(j)
 	//
 	// This option makes sense only if a small part of the graph is changed.
 	// The initialization procedure goes only through marked nodes then.
-	// 
+	//
 	// mark_node(i) can either be called before or after graph modification.
 	// Can be called more than once per node, but calls after the first one
 	// do not have any effect.
-	// 
-	// NOTE: 
+	//
+	// NOTE:
 	//   - This option cannot be used in the first call to maxflow().
 	//   - It is not necessary to call mark_node() if the change is ``not essential'',
 	//     i.e. sign(trcap) is preserved for a node and zero/nonzero status is preserved for an arc.
 	//   - To check that you marked all necessary nodes, you can call maxflow(false) after calling maxflow(true).
 	//     If everything is correct, the two calls must return the same value of flow. (Useful for debugging).
 	void mark_node(node_id i);
 
@@ -258,54 +258,54 @@
 	//				g->remove_from_changed_list(i);
 	//				// do something with node i...
 	//				if (g->what_segment(i) == G::SOURCE) { ... }
 	//			}
 	//			changed_list->Reset();
 	//		}
 	//		delete changed_list;
-	//		
+	//
 	// NOTE:
 	//  - If changed_list option is used, then reuse_trees must be used as well.
 	//  - In the example above, the user may omit calls g->remove_from_changed_list(i) and changed_list->Reset() in a given iteration.
 	//    Then during the next call to maxflow(true, &changed_list) new nodes will be added to changed_list.
 	//  - If the next call to maxflow() does not use option reuse_trees, then calling remove_from_changed_list()
 	//    is not necessary. ("changed_list->Reset()" or "delete changed_list" should still be called, though).
-	void remove_from_changed_list(node_id i) 
-	{ 
-		assert(i>=0 && i<node_num && nodes[i].is_in_changed_list); 
+	void remove_from_changed_list(node_id i)
+	{
+		assert(i>=0 && i<node_num && nodes[i].is_in_changed_list);
 		nodes[i].is_in_changed_list = 0;
 	}
 
 
 
 
 
 
 /////////////////////////////////////////////////////////////////////////
 /////////////////////////////////////////////////////////////////////////
 /////////////////////////////////////////////////////////////////////////
-	
+
 private:
 	// internal variables and functions
 
 	struct node
 	{
 		arc			*first;		// first outcoming arc
 
 		arc			*parent;	// node's parent
 		node		*next;		// pointer to the next active node
 								//   (or to itself if it is the last node in the list)
 		int			TS;			// timestamp showing when DIST was computed
 		int			DIST;		// distance to the terminal
 		int			is_sink : 1;	// flag showing whether the node is in the source or in the sink tree (if parent!=NULL)
 		int			is_marked : 1;	// set by mark_node()
-		int			is_in_changed_list : 1; // set by maxflow if 
+		int			is_in_changed_list : 1; // set by maxflow if
 
 		tcaptype	tr_cap;		// if tr_cap > 0 then tr_cap is residual capacity of the arc SOURCE->node
-								// otherwise         -tr_cap is residual capacity of the arc node->SINK 
+								// otherwise         -tr_cap is residual capacity of the arc node->SINK
 
 	};
 
 	struct arc
 	{
 		node		*head;		// node the arc points to
 		arc			*next;		// next arc with the same originating node
@@ -380,15 +380,15 @@
 
 ///////////////////////////////////////
 // Implementation - inline functions //
 ///////////////////////////////////////
 
 
 
-template <typename captype, typename tcaptype, typename flowtype> 
+template <typename captype, typename tcaptype, typename flowtype>
 	inline typename Graph<captype,tcaptype,flowtype>::node_id Graph<captype,tcaptype,flowtype>::add_node(int num)
 {
 	assert(num > 0);
 
 	if (node_last + num > node_max) reallocate_nodes(num);
 
 	if (num == 1)
@@ -408,27 +408,27 @@
 		node_id i = node_num;
 		node_num += num;
 		node_last += num;
 		return i;
 	}
 }
 
-template <typename captype, typename tcaptype, typename flowtype> 
+template <typename captype, typename tcaptype, typename flowtype>
 	inline void Graph<captype,tcaptype,flowtype>::add_tweights(node_id i, tcaptype cap_source, tcaptype cap_sink)
 {
 	assert(i >= 0 && i < node_num);
 
 	tcaptype delta = nodes[i].tr_cap;
 	if (delta > 0) cap_source += delta;
 	else           cap_sink   -= delta;
 	flow += (cap_source < cap_sink) ? cap_source : cap_sink;
 	nodes[i].tr_cap = cap_source - cap_sink;
 }
 
-template <typename captype, typename tcaptype, typename flowtype> 
+template <typename captype, typename tcaptype, typename flowtype>
 	inline void Graph<captype,tcaptype,flowtype>::add_edge(node_id _i, node_id _j, captype cap, captype rev_cap)
 {
 	assert(_i >= 0 && _i < node_num);
 	assert(_j >= 0 && _j < node_num);
 	assert(_i != _j);
 	assert(cap >= 0);
 	assert(rev_cap >= 0);
@@ -504,77 +504,77 @@
 	{
 		if (a->head == j) return a;
 		a = a->next;
 	}
 	return NULL;
 }
 
-template <typename captype, typename tcaptype, typename flowtype> 
+template <typename captype, typename tcaptype, typename flowtype>
 	inline typename Graph<captype,tcaptype,flowtype>::arc* Graph<captype,tcaptype,flowtype>::get_first_arc()
 {
 	return arcs;
 }
 
-template <typename captype, typename tcaptype, typename flowtype> 
-	inline typename Graph<captype,tcaptype,flowtype>::arc* Graph<captype,tcaptype,flowtype>::get_next_arc(arc* a) 
+template <typename captype, typename tcaptype, typename flowtype>
+	inline typename Graph<captype,tcaptype,flowtype>::arc* Graph<captype,tcaptype,flowtype>::get_next_arc(arc* a)
 {
-	return a + 1; 
+	return a + 1;
 }
 
-template <typename captype, typename tcaptype, typename flowtype> 
+template <typename captype, typename tcaptype, typename flowtype>
 	inline void Graph<captype,tcaptype,flowtype>::get_arc_ends(arc* a, node_id& i, node_id& j)
 {
 	assert(a >= arcs && a < arc_last);
 	i = (node_id) (a->sister->head - nodes);
 	j = (node_id) (a->head - nodes);
 }
 
-template <typename captype, typename tcaptype, typename flowtype> 
+template <typename captype, typename tcaptype, typename flowtype>
 	inline tcaptype Graph<captype,tcaptype,flowtype>::get_trcap(node_id i)
 {
 	assert(i>=0 && i<node_num);
 	return nodes[i].tr_cap;
 }
 
-template <typename captype, typename tcaptype, typename flowtype> 
+template <typename captype, typename tcaptype, typename flowtype>
 	inline captype Graph<captype,tcaptype,flowtype>::get_rcap(arc* a)
 {
 	assert(a >= arcs && a < arc_last);
 	return a->r_cap;
 }
 
-template <typename captype, typename tcaptype, typename flowtype> 
+template <typename captype, typename tcaptype, typename flowtype>
 	inline void Graph<captype,tcaptype,flowtype>::set_trcap(node_id i, tcaptype trcap)
 {
-	assert(i>=0 && i<node_num); 
+	assert(i>=0 && i<node_num);
 	nodes[i].tr_cap = trcap;
 }
 
-template <typename captype, typename tcaptype, typename flowtype> 
+template <typename captype, typename tcaptype, typename flowtype>
 	inline void Graph<captype,tcaptype,flowtype>::set_rcap(arc* a, captype rcap)
 {
 	assert(a >= arcs && a < arc_last);
 	a->r_cap = rcap;
 }
 
 
-template <typename captype, typename tcaptype, typename flowtype> 
+template <typename captype, typename tcaptype, typename flowtype>
 	inline typename Graph<captype,tcaptype,flowtype>::termtype Graph<captype,tcaptype,flowtype>::what_segment(node_id i, termtype default_segm)
 {
 	if (nodes[i].parent)
 	{
 		return (nodes[i].is_sink) ? SINK : SOURCE;
 	}
 	else
 	{
 		return default_segm;
 	}
 }
 
-template <typename captype, typename tcaptype, typename flowtype> 
+template <typename captype, typename tcaptype, typename flowtype>
 	inline void Graph<captype,tcaptype,flowtype>::mark_node(node_id _i)
 {
 	node* i = nodes + _i;
 	if (!i->next)
 	{
 		/* it's not in the list yet */
 		if (queue_last[1]) queue_last[1] -> next = i;
```

### Comparing `MedPy-0.4.0/lib/maxflow/src/wrapper.cpp` & `MedPy-0.5.0/lib/maxflow/src/wrapper.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 BOOST_PYTHON_MEMBER_FUNCTION_OVERLOADS(GraphInt_what_segment_overload, what_segment, 1, 2)
 
 
 // Wrapper functions for different scopes
 void wrap_scopegraphfloat()
 {
 	using namespace boost::python;
-	scope graphFloat = 
+	scope graphFloat =
 		class_<GraphFloat>("GraphFloat", "Graph template intance with float for flowtype, tcaptype and captype. Takes the number of nodes as first and the number of edges as second parameter. Although it is possible to exceed these values later, it is discourage as it leads to bad memory management. The edges i->j and j->i count here as one single edge.", init<int, int>())
         .def("add_node", &GraphFloat::add_node/*, GraphFloat_add_node_overload()*/) // "Add one or more nodes to the graph and returns the id of the first such created node. The total number of added nodes should never exceed the max node number passed to the initializer. Only nodes added with this function can be referenced in methods such as add_edge and add_tweights."
         .def("add_edge", &GraphFloat::add_edge, "Add an edge from i to j with the capacity cap and reversed capacity rev_cap. Node ids start from 0. Repeated calls lead to the addition of multiple arcs and therefore the allocate memory can be exceeded.")
         .def("sum_edge", &GraphFloat::sum_edge, "Add an edge from i to j with the capacity cap and reversed capacity rev_cap. Node ids start from 0. Repeated calls are summed to already existing edge weights. Requires less memory, but is slightly slower.")
         .def("add_tweights", &GraphFloat::add_tweights, "Add a terminal weight from cap_source to i and from i to cap_sink. Can be called multiple times (add to the existing weights).")
         .def("maxflow", &GraphFloat::maxflow/*, GraphFloat_maxflow_overload()*/, "Compute the min-cut/max-flow of the graph and return the maxflow value.")
         .def("what_segment", &GraphFloat::what_segment/*, GraphFloat_what_segment_overload()*/, "Returns the terminal the node i belongs to after executing the min-cut/max-flow. Returns either GraphFloat::SOURCE or GraphFloat::SINK.")
@@ -55,15 +55,15 @@
 		.value("SINK", GraphFloat::SINK)
 		;
 }
 
 void wrap_scopegraphdouble()
 {
 	using namespace boost::python;
-	scope graphDouble = 
+	scope graphDouble =
 		class_<GraphDouble>("GraphDouble", "Graph template intance with double for flowtype, tcaptype and captype. Takes the number of nodes as first and the number of edges as second parameter. Although it is possible to exceed these values later, it is discourage as it leads to bad memory management. The edges i->j and j->i count here as one single edge.", init<int, int>())
         .def("add_node", &GraphDouble::add_node/*, GraphDouble_add_node_overload()*/) // "Add one or more nodes to the graph and returns the id of the first such created node. The total number of added nodes should never exceed the max node number passed to the initializer. Only nodes added with this function can be referenced in methods such as add_edge and add_tweights."
         .def("add_edge", &GraphDouble::add_edge, "Add an edge from i to j with the capacity cap and reversed capacity rev_cap. Node ids start from 0. Repeated calls lead to the addition of multiple arcs and therefore the allocate memory can be exceeded.")
         .def("sum_edge", &GraphDouble::sum_edge, "Add an edge from i to j with the capacity cap and reversed capacity rev_cap. Node ids start from 0. Repeated calls are summed to already existing edge weights. Requires less memory, but is slightly slower.")
         .def("add_tweights", &GraphDouble::add_tweights, "Add a terminal weight from cap_source to i and from i to cap_sink. Can be called multiple times (add to the existing weights).")
         .def("maxflow", &GraphDouble::maxflow/*, GraphDouble_maxflow_overload()*/, "Compute the min-cut/max-flow of the graph and return the maxflow value.")
         .def("what_segment", &GraphDouble::what_segment/*, GraphDouble_what_segment_overload()*/, "Returns the terminal the node i belongs to after executing the min-cut/max-flow. Returns either GraphDouble::SOURCE or GraphDouble::SINK.")
@@ -87,15 +87,15 @@
 		.value("SINK", GraphDouble::SINK)
     	;
 }
 
 void wrap_scopegraphint()
 {
 	using namespace boost::python;
-	scope graphInt = 
+	scope graphInt =
 		class_<GraphInt>("GraphInt", "Graph template intance with int for flowtype, tcaptype and captype. Takes the number of nodes as first and the number of edges as second parameter. Although it is possible to exceed these values later, it is discourage as it leads to bad memory management. The edges i->j and j->i count here as one single edge.", init<int, int>())
 		  .def("add_node", &GraphInt::add_node/*, GraphInt_add_node_overload()*/) // "Add one or more nodes to the graph and returns the id of the first such created node. The total number of added nodes should never exceed the max node number passed to the initializer. Only nodes added with this function can be referenced in methods such as add_edge and add_tweights."
 	      .def("add_edge", &GraphInt::add_edge, "Add an edge from i to j with the capacity cap and reversed capacity rev_cap. Node ids start from 0. Repeated calls lead to the addition of multiple arcs and therefore the allocate memory can be exceeded.")
 	      .def("sum_edge", &GraphInt::sum_edge, "Add an edge from i to j with the capacity cap and reversed capacity rev_cap. Node ids start from 0. Repeated calls are summed to already existing edge weights. Requires less memory, but is slightly slower.")
 		  .def("add_tweights", &GraphInt::add_tweights, "Add a terminal weight from cap_source to i and from i to cap_sink. Can be called multiple times (add to the existing weights).")
 		  .def("maxflow", &GraphInt::maxflow/*, GraphInt_maxflow_overload()*/, "Compute the min-cut/max-flow of the graph and return the maxflow value.")
 		  .def("what_segment", &GraphInt::what_segment/*, GraphInt_what_segment_overload()*/, "Returns the terminal the node i belongs to after executing the min-cut/max-flow. Returns either GraphInt::SOURCE or GraphInt::SINK.")
```

### Comparing `MedPy-0.4.0/lib/maxflow/src/graph.cpp` & `MedPy-0.5.0/lib/maxflow/src/graph.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #include <stdio.h>
 #include <iostream>
 #include <stdlib.h>
 #include <string.h>
 #include "graph.h"
 
 
-template <typename captype, typename tcaptype, typename flowtype> 
+template <typename captype, typename tcaptype, typename flowtype>
 	Graph<captype, tcaptype, flowtype>::Graph(int node_num_max, int edge_num_max, void (*err_function)(char *))
 	: node_num(0),
 	  nodeptr_block(NULL),
 	  error_function(err_function)
 {
 	if (node_num_max < 16) node_num_max = 16;
 	if (edge_num_max < 16) edge_num_max = 16;
@@ -26,44 +26,44 @@
 	arc_last = arcs;
 	arc_max = arcs + 2*edge_num_max;
 
 	maxflow_iteration = 0;
 	flow = 0;
 }
 
-template <typename captype, typename tcaptype, typename flowtype> 
+template <typename captype, typename tcaptype, typename flowtype>
 	Graph<captype,tcaptype,flowtype>::~Graph()
 {
-	if (nodeptr_block) 
-	{ 
-		delete nodeptr_block; 
-		nodeptr_block = NULL; 
+	if (nodeptr_block)
+	{
+		delete nodeptr_block;
+		nodeptr_block = NULL;
 	}
 	free(nodes);
 	free(arcs);
 }
 
-template <typename captype, typename tcaptype, typename flowtype> 
+template <typename captype, typename tcaptype, typename flowtype>
 	void Graph<captype,tcaptype,flowtype>::reset()
 {
 	node_last = nodes;
 	arc_last = arcs;
 	node_num = 0;
 
-	if (nodeptr_block) 
-	{ 
-		delete nodeptr_block; 
-		nodeptr_block = NULL; 
+	if (nodeptr_block)
+	{
+		delete nodeptr_block;
+		nodeptr_block = NULL;
 	}
 
 	maxflow_iteration = 0;
 	flow = 0;
 }
 
-template <typename captype, typename tcaptype, typename flowtype> 
+template <typename captype, typename tcaptype, typename flowtype>
 	void Graph<captype,tcaptype,flowtype>::reallocate_nodes(int num)
 {
 	int node_num_max = (int)(node_max - nodes);
 	node* nodes_old = nodes;
 
 	node_num_max += node_num_max / 2;
 	if (node_num_max < node_num + num) node_num_max = node_num + num;
@@ -79,15 +79,15 @@
 		for (a=arcs; a<arc_last; a++)
 		{
 			a->head = (node*) ((char*)a->head + (((char*) nodes) - ((char*) nodes_old)));
 		}
 	}
 }
 
-template <typename captype, typename tcaptype, typename flowtype> 
+template <typename captype, typename tcaptype, typename flowtype>
 	void Graph<captype,tcaptype,flowtype>::reallocate_arcs()
 {
 	int arc_num_max = (int)(arc_max - arcs);
 	int arc_num = (int)(arc_last - arcs);
 	arc* arcs_old = arcs;
 
 	arc_num_max += arc_num_max / 2; if (arc_num_max & 1) arc_num_max ++;
```

### Comparing `MedPy-0.4.0/MedPy.egg-info/SOURCES.txt` & `MedPy-0.5.0/MedPy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 CHANGES.txt
 LICENSE.txt
 MANIFEST.in
 README.md
 README_PYPI.md
-requirements-dev.txt
+RELEASE.md
 setup.py
 MedPy.egg-info/PKG-INFO
 MedPy.egg-info/SOURCES.txt
 MedPy.egg-info/dependency_links.txt
 MedPy.egg-info/requires.txt
 MedPy.egg-info/top_level.txt
 bin/medpy_anisotropic_diffusion.py
@@ -46,14 +46,15 @@
 bin/medpy_set_pixel_spacing.py
 bin/medpy_shrink_image.py
 bin/medpy_split_xd_to_xminus1d.py
 bin/medpy_stack_sub_volumes.py
 bin/medpy_swap_dimensions.py
 bin/medpy_watershed.py
 bin/medpy_zoom_image.py
+lib/maxflow/src/README
 lib/maxflow/src/block.h
 lib/maxflow/src/graph.cpp
 lib/maxflow/src/graph.h
 lib/maxflow/src/instances.inc
 lib/maxflow/src/maxflow.cpp
 lib/maxflow/src/pythongraph.h
 lib/maxflow/src/wrapper.cpp
```

### Comparing `MedPy-0.4.0/MedPy.egg-info/PKG-INFO` & `MedPy-0.5.0/MedPy.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,195 +1,204 @@
 Metadata-Version: 2.1
 Name: MedPy
-Version: 0.4.0
+Version: 0.5.0
 Summary: Medical image processing in Python
 Home-page: https://github.com/loli/medpy
 Author: Oskar Maier
 Author-email: oskar.maier@gmail.com
 License: LICENSE.txt
-Description: # MedPy
-        
-        [GitHub](https://github.com/loli/medpy/) | [Documentation](http://loli.github.io/medpy/) | [Tutorials](http://loli.github.io/medpy/) | [Issue tracker](https://github.com/loli/medpy/issues) | [Contact](oskar.maier@gmail.com)
-        
-        **MedPy** is a library and script collection for medical image processing in Python, providing basic functionalities for **reading**, **writing** and **manipulating** large images of **arbitrary dimensionality**.
-        Its main contributions are n-dimensional versions of popular **image filters**, a collection of **image feature extractors**, ready to be used with [scikit-learn](http://scikit-learn.org), and an exhaustive n-dimensional **graph-cut** package.
-        
-        * [Installation](#installation)
-        * [Getting started with the library](#getting-started-with-the-library)
-        * [Getting started with the scripts](#getting-started-with-the-scripts)
-        * [Read/write support for medical image formats](#read-write-support-for-medical-image-formats)
-        * [Requirements](#requirements)
-        * [License](#license)
-        
-        ## Installation
-        
-        ```bash
-        sudo apt-get install libboost-python-dev build-essential
-        pip3 install medpy
-        ```
-        
-        **MedPy** requires **Python 3** and officially supports Ubuntu as well as other Debian derivatives.
-        For installation instructions on other operating systems see the [documentation](http://loli.github.io/medpy/).
-        While the library itself is written purely in Python, the **graph-cut** extension comes in C++ and has it's own requirements. More details can be found in the [documentation](http://loli.github.io/medpy/).
-        
-        ### Using Python 2
-        
-        **Python 2** is no longer supported. But you can still use the older releases.
-        
-        ```bash
-        pip install medpy==0.3.0
-        ```
-        
-        ## Getting started with the library
-        
-        If you already have a medical image whose format is support (see the [documentation](http://loli.github.io/medpy/>) for details), then good.
-        Otherwise, navigate to http://www.nitrc.org/projects/inia19, click on the *Download Now* button, unpack and look for the *inia19-t1.nii* file. Open it in your favorite medical image viewer (I personally fancy [itksnap](http://www.itksnap.org)) and beware: the INIA19 primate brain atlas.
-        
-        Load the image
-        
-        ```python
-        from medpy.io import load
-        image_data, image_header = load('/path/to/image.xxx')
-        ```
-        
-        The data is stored in a numpy ndarray, the header is an object containing additional metadata, such as the voxel-spacing. Now lets take a look at some of the image metadata
-        
-        ```python
-        image_data.shape
-        ```
-        
-        `(168, 206, 128)`
-        
-        ```python
-        image_data.dtype
-        ```
-        
-        `dtype(float32)`
-        
-        And the header gives us
-        
-        ```python
-        image_header.get_voxel_spacing()
-        ```
-        
-        `(0.5, 0.5, 0.5)`
-        
-        ```python
-        image_header.get_offset()
-        ```
-        
-        `(0.0, 0.0, 0.0)`
-        
-        Now lets apply one of the **MedPy** filter, more exactly the [Otsu thresholding](https://en.wikipedia.org/wiki/Otsu%27s_method), which can be used for automatic background removal
-        
-        ```python
-        from medpy.filter import otsu
-        threshold = otsu(image_data)
-        output_data = image_data > threshold
-        ```
-        
-        And save the binary image, marking the foreground
-        
-        ```python
-        from medpy.io import save
-        save(output_data, '/path/to/otsu.xxx', image_header)
-        ```
-        
-        After taking a look at it, you might want to dive deeper with the tutorials found in the [documentation](http://loli.github.io/medpy/).
-        
-        ## Getting started with the scripts
-        
-        **MedPy** comes with a range of read-to-use commandline scripts, which are all prefixed by `medpy_`.
-        To try these examples, first get an image as described in the previous section. Now call
-        
-        ```bash
-        medpy_info.py /path/to/image.xxx
-        ```
-        
-        will give you some details about the image. With
-        
-        ```bash
-        medpy_diff.py /path/to/image1.xxx /path/to/image2.xxx
-        ```
-        
-        you can compare two image. And
-        
-        ```bash
-        medpy_anisotropic_diffusion.py /path/to/image.xxx /path/to/output.xxx
-        ```
-        
-        lets you apply an edge preserving anisotropic diffusion filter. For a list of all scripts, see the [documentation](http://loli.github.io/medpy/).
-        
-        ## Read/write support for medical image formats
-        
-        MedPy relies on SimpleITK, which enables the power of ITK for image loading and saving.
-        The supported image file formats should include at least the following. Note that not all might be supported by your machine.
-        
-        **Medical formats:**
-        
-        * ITK MetaImage (.mha/.raw, .mhd)
-        * Neuroimaging Informatics Technology Initiative (NIfTI) (.nia, .nii, .nii.gz, .hdr, .img, .img.gz)
-        * Analyze (plain, SPM99, SPM2) (.hdr/.img, .img.gz)
-        * Digital Imaging and Communications in Medicine (DICOM) (.dcm, .dicom)
-        * Digital Imaging and Communications in Medicine (DICOM) series (<directory>/)
-        * Nearly Raw Raster Data (Nrrd) (.nrrd, .nhdr) 
-        * Medical Imaging NetCDF (MINC) (.mnc, .MNC)
-        * Guys Image Processing Lab (GIPL) (.gipl, .gipl.gz)
-        
-        **Microscopy formats:**
-        
-        * Medical Research Council (MRC) (.mrc, .rec)
-        * Bio-Rad (.pic, .PIC)
-        * LSM (Zeiss) microscopy images (.tif, .TIF, .tiff, .TIFF, .lsm, .LSM)
-        * Stimulate / Signal Data (SDT) (.sdt)
-        
-        **Visualization formats:**
-        
-        * VTK images (.vtk)
-        
-        **Other formats:**
-        
-        * Portable Network Graphics (PNG) (.png, .PNG)
-        * Joint Photographic Experts Group (JPEG) (.jpg, .JPG, .jpeg, .JPEG)
-        * Tagged Image File Format (TIFF) (.tif, .TIF, .tiff, .TIFF)
-        * Windows bitmap (.bmp, .BMP)
-        * Hierarchical Data Format (HDF5) (.h5 , .hdf5 , .he5)
-        * MSX-DOS Screen-x (.ge4, .ge5)
-        
-        ## Requirements
-        
-        MedPy comes with a number of dependencies and optional functionality that can require you to install additional packages.
-        
-        ### Main dependencies
-        
-        * [scipy](http://www.scipy.org)
-        * [numpy](http://www.numpy.org)
-        * [SimpleITK](https://simpleitk.readthedocs.io)
-        
-        ### Optional functionalities
-        
-        * compilation with `max-flow/min-cut` (enables the GraphCut functionalities)
-        
-        ## License
-        
-        MedPy is distributed under the GNU General Public License, a version of which can be found in the LICENSE.txt file.
-        
 Keywords: medical image processing dicom itk insight tool kit MRI CT US graph cut max-flow min-cut
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: C++
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
+Requires-Python: >=3.5, <4
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: scipy>=1.10
+Requires-Dist: numpy>=1.24
+Requires-Dist: SimpleITK>=2.1
+Provides-Extra: dev
+Requires-Dist: pre-commit; extra == "dev"
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: hypothesis; extra == "test"
+Provides-Extra: watershed
+Requires-Dist: scikit-image; extra == "watershed"
+Provides-Extra: doc
+Requires-Dist: sphinx>=1.6; extra == "doc"
+Requires-Dist: numpydoc; extra == "doc"
+Requires-Dist: pydata-sphinx-theme; extra == "doc"
+
+# MedPy
+
+[GitHub](https://github.com/loli/medpy/) | [Documentation](http://loli.github.io/medpy/) | [Tutorials](http://loli.github.io/medpy/) | [Issue tracker](https://github.com/loli/medpy/issues)
+
+**MedPy** is a library and script collection for medical image processing in Python, providing basic functionalities for **reading**, **writing** and **manipulating** large images of **arbitrary dimensionality**.
+Its main contributions are n-dimensional versions of popular **image filters**, a collection of **image feature extractors**, ready to be used with [scikit-learn](http://scikit-learn.org), and an exhaustive n-dimensional **graph-cut** package.
+
+* [Installation](#installation)
+* [Getting started with the library](#getting-started-with-the-library)
+* [Getting started with the scripts](#getting-started-with-the-scripts)
+* [Support of medical image formats](#support-of-medical-image-formats)
+* [Requirements](#requirements)
+* [License](#license)
+
+## Installation
+
+```bash
+sudo apt-get install libboost-python-dev build-essential
+pip3 install medpy
+```
+
+**MedPy** requires **Python 3** and officially supports Ubuntu as well as other Debian derivatives.
+For installation instructions on other operating systems see the [documentation](http://loli.github.io/medpy/).
+While the library itself is written purely in Python, the **graph-cut** extension comes in C++ and has [it's own requirements](http://loli.github.io/medpy/installation/graphcutsupport.html).
+
+## Getting started with the library
+
+If you already have a medical image at hand in [one of the supported formats](http://loli.github.io/medpy/information/imageformats.html), you can use it for this introduction. If not, navigate to http://www.nitrc.org/projects/inia19, click on the *Download Now* button, unpack and look for the *inia19-t1.nii* file. Open it in your favorite medical image viewer (I personally fancy [itksnap](http://www.itksnap.org)) and beware: the INIA19 primate brain atlas.
+
+Load the image
+
+```python
+from medpy.io import load
+image_data, image_header = load('/path/to/image.xxx')
+```
+
+The data is stored in a numpy ndarray, the header is an object containing additional metadata, such as the voxel-spacing. Now lets take a look at some of the image metadata
+
+```python
+image_data.shape
+```
+
+`(168, 206, 128)`
+
+```python
+image_data.dtype
+```
+
+`dtype(float32)`
+
+And the header gives us
+
+```python
+image_header.get_voxel_spacing()
+```
+
+`(0.5, 0.5, 0.5)`
+
+```python
+image_header.get_offset()
+```
+
+`(0.0, 0.0, 0.0)`
+
+Now lets apply one of the **MedPy** filter, more exactly the [Otsu thresholding](https://en.wikipedia.org/wiki/Otsu%27s_method), which can be used for automatic background removal
+
+```python
+from medpy.filter import otsu
+threshold = otsu(image_data)
+output_data = image_data > threshold
+```
+
+And save the binary image, marking the foreground
+
+```python
+from medpy.io import save
+save(output_data, '/path/to/otsu.xxx', image_header)
+```
+
+After taking a look at it, you might want to dive deeper with the tutorials found in the [documentation](http://loli.github.io/medpy/information/commandline_tools_listing.html).
+
+## Getting started with the scripts
+
+**MedPy** comes with a range of read-to-use commandline scripts, which are all prefixed by `medpy_`.
+To try these examples, first get an image as described in the previous section. Now call
+
+```bash
+medpy_info.py /path/to/image.xxx
+```
+
+will give you some details about the image. With
+
+```bash
+medpy_diff.py /path/to/image1.xxx /path/to/image2.xxx
+```
+
+you can compare two image. And
+
+```bash
+medpy_anisotropic_diffusion.py /path/to/image.xxx /path/to/output.xxx
+```
+
+lets you apply an edge preserving anisotropic diffusion filter. For a list of all scripts, see the [documentation](http://loli.github.io/medpy/).
+
+## Support of medical image formats
+
+MedPy relies on SimpleITK, which enables the power of ITK for image loading and saving.
+The supported image file formats should include at least the following. Note that not all might be supported by your machine.
+
+**Medical formats:**
+
+* ITK MetaImage (.mha/.raw, .mhd)
+* Neuroimaging Informatics Technology Initiative (NIfTI) (.nia, .nii, .nii.gz, .hdr, .img, .img.gz)
+* Analyze (plain, SPM99, SPM2) (.hdr/.img, .img.gz)
+* Digital Imaging and Communications in Medicine (DICOM) (.dcm, .dicom)
+* Digital Imaging and Communications in Medicine (DICOM) series (<directory>/)
+* Nearly Raw Raster Data (Nrrd) (.nrrd, .nhdr)
+* Medical Imaging NetCDF (MINC) (.mnc, .MNC)
+* Guys Image Processing Lab (GIPL) (.gipl, .gipl.gz)
+
+**Microscopy formats:**
+
+* Medical Research Council (MRC) (.mrc, .rec)
+* Bio-Rad (.pic, .PIC)
+* LSM (Zeiss) microscopy images (.tif, .TIF, .tiff, .TIFF, .lsm, .LSM)
+* Stimulate / Signal Data (SDT) (.sdt)
+
+**Visualization formats:**
+
+* VTK images (.vtk)
+
+**Other formats:**
+
+* Portable Network Graphics (PNG) (.png, .PNG)
+* Joint Photographic Experts Group (JPEG) (.jpg, .JPG, .jpeg, .JPEG)
+* Tagged Image File Format (TIFF) (.tif, .TIF, .tiff, .TIFF)
+* Windows bitmap (.bmp, .BMP)
+* Hierarchical Data Format (HDF5) (.h5 , .hdf5 , .he5)
+* MSX-DOS Screen-x (.ge4, .ge5)
+
+## Requirements
+
+MedPy comes with a number of dependencies and optional functionality that can require you to install additional packages.
+
+### Main dependencies
+
+* [scipy](http://www.scipy.org)
+* [numpy](http://www.numpy.org)
+* [SimpleITK](https://simpleitk.readthedocs.io)
+
+### Optional functionalities
+
+* compilation with `max-flow/min-cut` (enables the GraphCut functionalities)
+
+## License
+
+MedPy is distributed under the GNU General Public License, a version of which can be found in the LICENSE.txt file.
```

### Comparing `MedPy-0.4.0/setup.py` & `MedPy-0.5.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,198 +5,239 @@
 # https://pypi.python.org/pypi/simplejson/
 
 import os
 import sys
 from ctypes.util import find_library
 from distutils.command.build_ext import build_ext
 from distutils.errors import CCompilerError, DistutilsExecError, DistutilsPlatformError
-from setuptools import setup, Extension, Command
+
+from setuptools import Command, Extension, setup
 
 # CONSTANTS
-IS_PYPY = hasattr(sys, 'pypy_translation_info') # why this?
-PACKAGES= [
-    'medpy',
-    'medpy.core',
-    'medpy.features',
-    'medpy.filter',
-    'medpy.graphcut',
-    'medpy.io',
-    'medpy.metric',
-    'medpy.utilities'
+PACKAGES = [
+    "medpy",
+    "medpy.core",
+    "medpy.features",
+    "medpy.filter",
+    "medpy.graphcut",
+    "medpy.io",
+    "medpy.metric",
+    "medpy.utilities",
 ]
 
+
 #### FUNCTIONS
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
+
+def try_find_library(lib_name):
+    if not find_library(lib_name):
+        return None
+    else:
+        return lib_name
+
+
 ### PREDEFINED MODULES
 # The maxflow graphcut wrapper using boost.python
 
 # Special handling for homebrew Boost Python library
 if sys.platform == "darwin":
     if sys.version_info.major > 2:
-        boost_python_library = 'boost_python' + str(sys.version_info.major)
+        boost_python_library = "boost_python" + str(sys.version_info.major)
     else:
-        boost_python_library = 'boost_python'
+        boost_python_library = "boost_python"
 else:
-    boost_python_library = 'boost_python-py' + str(sys.version_info.major) + str(sys.version_info.minor)
-    if not find_library(boost_python_library):
-        # exact version not find, trying with major fit only as fallback
-        boost_python_library = 'boost_python' + str(sys.version_info.major)
-
-maxflow = Extension('medpy.graphcut.maxflow',
-                    define_macros = [('MAJOR_VERSION', '0'),
-                                     ('MINOR_VERSION', '1')],
-                    sources = ['lib/maxflow/src/maxflow.cpp', 'lib/maxflow/src/wrapper.cpp', 'lib/maxflow/src/graph.cpp'],
-                    libraries = [boost_python_library],
-                    extra_compile_args = ['-O0'])
+    boost_python_library = try_find_library(
+        "boost_python-py" + str(sys.version_info.major) + str(sys.version_info.minor)
+    )
+    if not boost_python_library:
+        boost_python_library = try_find_library(
+            "boost_python-py" + str(sys.version_info.major)
+        )
+    if not boost_python_library:
+        boost_python_library = try_find_library(
+            "boost_python" + str(sys.version_info.major) + str(sys.version_info.minor)
+        )
+    if not boost_python_library:
+        # exact version not found, trying with major fit only as fallback
+        boost_python_library = "boost_python" + str(sys.version_info.major)
+
+maxflow = Extension(
+    "medpy.graphcut.maxflow",
+    define_macros=[("MAJOR_VERSION", "0"), ("MINOR_VERSION", "1")],
+    sources=[
+        "lib/maxflow/src/maxflow.cpp",
+        "lib/maxflow/src/wrapper.cpp",
+        "lib/maxflow/src/graph.cpp",
+    ],
+    libraries=[boost_python_library],
+    extra_compile_args=["-O0"],
+)
 
 ### FUNCTIONALITY FOR CONDITIONAL C++ BUILD
-if sys.platform == 'win32' and sys.version_info > (2, 6):
+if sys.platform == "win32" and sys.version_info > (2, 6):
     # 2.6's distutils.msvc9compiler can raise an IOError when failing to
     # find the compiler
     # It can also raise ValueError http://bugs.python.org/issue7511
-    ext_errors = (CCompilerError, DistutilsExecError, DistutilsPlatformError, IOError, ValueError)
+    ext_errors = (
+        CCompilerError,
+        DistutilsExecError,
+        DistutilsPlatformError,
+        IOError,
+        ValueError,
+    )
 else:
     ext_errors = (CCompilerError, DistutilsExecError, DistutilsPlatformError)
 
+
 class BuildFailed(Exception):
     pass
 
+
 class TestCommand(Command):
     user_options = []
 
     def initialize_options(self):
         pass
 
     def finalize_options(self):
         pass
 
     def run(self):
         raise SystemExit(1)
 
+
 class ve_build_ext(build_ext):
     # This class allows C++ extension building to fail.
     def run(self):
         try:
             build_ext.run(self)
         except DistutilsPlatformError:
             raise BuildFailed()
 
     def build_extension(self, ext):
         try:
             build_ext.build_extension(self, ext)
         except ext_errors:
             raise BuildFailed()
 
+
 ### MAIN SETUP FUNCTION
 def run_setup(with_compilation):
     cmdclass = dict(test=TestCommand)
     if with_compilation:
-        kw = dict(ext_modules = [maxflow],
-                  cmdclass=dict(cmdclass, build_ext=ve_build_ext))
-        ap = ['medpy.graphcut']
+        kw = dict(
+            ext_modules=[maxflow], cmdclass=dict(cmdclass, build_ext=ve_build_ext)
+        )
+        ap = ["medpy.graphcut"]
     else:
         kw = dict(cmdclass=cmdclass)
         ap = []
 
     setup(
-          name='MedPy',
-          version='0.4.0', # major.minor.micro
-          description='Medical image processing in Python',
-          author='Oskar Maier',
-          author_email='oskar.maier@gmail.com',
-          url='https://github.com/loli/medpy',
-          license='LICENSE.txt',
-          keywords='medical image processing dicom itk insight tool kit MRI CT US graph cut max-flow min-cut',
-          long_description=read('README_PYPI.md'),
-          long_description_content_type='text/markdown',
-
-          classifiers=[
-              'Development Status :: 5 - Production/Stable',
-              'Environment :: Console',
-              'Environment :: Other Environment',
-              'Intended Audience :: End Users/Desktop',
-              'Intended Audience :: Developers',
-              'Intended Audience :: Healthcare Industry',
-              'Intended Audience :: Science/Research',
-              'License :: OSI Approved :: GNU General Public License (GPL)',
-              'Operating System :: MacOS :: MacOS X',
-              'Operating System :: Microsoft :: Windows',
-              'Operating System :: POSIX',
-              'Operating System :: Unix',
-              'Programming Language :: Python :: 3.5',
-              'Programming Language :: Python :: 3.6',
-              'Programming Language :: C++',
-              'Topic :: Scientific/Engineering :: Medical Science Apps.',
-              'Topic :: Scientific/Engineering :: Image Recognition'
-          ],
-
-          install_requires=[
-            "scipy >= 1.1.0",
-            "numpy >= 1.11.0",
-            "SimpleITK >= 1.1.0"
-          ],
-
-          packages = PACKAGES + ap,
-
-          scripts=[
-            'bin/medpy_anisotropic_diffusion.py',
-            'bin/medpy_apparent_diffusion_coefficient.py',
-            'bin/medpy_binary_resampling.py',
-            'bin/medpy_convert.py',
-            'bin/medpy_create_empty_volume_by_example.py',
-            'bin/medpy_dicom_slices_to_volume.py',
-            'bin/medpy_dicom_to_4D.py',
-            'bin/medpy_diff.py',
-            'bin/medpy_extract_contour.py',
-            'bin/medpy_extract_min_max.py',
-            'bin/medpy_extract_sub_volume_auto.py',
-            'bin/medpy_extract_sub_volume_by_example.py',
-            'bin/medpy_extract_sub_volume.py',
-            'bin/medpy_fit_into_shape.py',
-            'bin/medpy_gradient.py',
-            'bin/medpy_graphcut_label_bgreduced.py',
-            'bin/medpy_graphcut_label_w_regional.py',
-            'bin/medpy_graphcut_label_wsplit.py',
-            'bin/medpy_graphcut_label.py',
-            'bin/medpy_graphcut_voxel.py',
-            'bin/medpy_grid.py',
-            'bin/medpy_info.py',
-            'bin/medpy_intensity_range_standardization.py',
-            'bin/medpy_intersection.py',
-            'bin/medpy_join_masks.py',
-            'bin/medpy_join_xd_to_xplus1d.py',
-            'bin/medpy_label_count.py',
-            'bin/medpy_label_fit_to_mask.py',
-            'bin/medpy_label_superimposition.py',
-            'bin/medpy_merge.py',
-            'bin/medpy_morphology.py',
-            'bin/medpy_resample.py',
-            'bin/medpy_reslice_3d_to_4d.py',
-            'bin/medpy_set_pixel_spacing.py',
-            'bin/medpy_shrink_image.py',
-            'bin/medpy_split_xd_to_xminus1d.py',
-            'bin/medpy_stack_sub_volumes.py',
-            'bin/medpy_swap_dimensions.py',
-            'bin/medpy_watershed.py',
-            'bin/medpy_zoom_image.py'
-          ],
+        name="MedPy",
+        version="0.5.0",  # major.minor.micro
+        description="Medical image processing in Python",
+        author="Oskar Maier",
+        author_email="oskar.maier@gmail.com",
+        url="https://github.com/loli/medpy",
+        license="LICENSE.txt",
+        keywords="medical image processing dicom itk insight tool kit MRI CT US graph cut max-flow min-cut",
+        long_description=read("README_PYPI.md"),
+        long_description_content_type="text/markdown",
+        classifiers=[
+            "Development Status :: 5 - Production/Stable",
+            "Environment :: Console",
+            "Environment :: Other Environment",
+            "Intended Audience :: End Users/Desktop",
+            "Intended Audience :: Developers",
+            "Intended Audience :: Healthcare Industry",
+            "Intended Audience :: Science/Research",
+            "License :: OSI Approved :: GNU General Public License (GPL)",
+            "Operating System :: MacOS :: MacOS X",
+            "Operating System :: Microsoft :: Windows",
+            "Operating System :: POSIX",
+            "Operating System :: Unix",
+            "Programming Language :: Python :: 3 :: Only",
+            "Programming Language :: Python :: 3.8",
+            "Programming Language :: Python :: 3.9",
+            "Programming Language :: Python :: 3.10",
+            "Programming Language :: Python :: 3.11",
+            "Programming Language :: C++",
+            "Topic :: Scientific/Engineering :: Medical Science Apps.",
+            "Topic :: Scientific/Engineering :: Image Recognition",
+        ],
+        python_requires=">=3.5, <4",
+        install_requires=["scipy >= 1.10", "numpy >= 1.24", "SimpleITK >= 2.1"],
+        extras_require={
+            "dev": ["pre-commit"],  # for development
+            "test": ["pytest", "hypothesis"],  # for testing
+            "watershed": ["scikit-image"],  # for watershed segmentation script
+            "doc": [
+                "sphinx >= 1.6",
+                "numpydoc",
+                "pydata-sphinx-theme",
+            ],  # for documentation generation
+        },
+        packages=PACKAGES + ap,
+        scripts=[
+            "bin/medpy_anisotropic_diffusion.py",
+            "bin/medpy_apparent_diffusion_coefficient.py",
+            "bin/medpy_binary_resampling.py",
+            "bin/medpy_convert.py",
+            "bin/medpy_create_empty_volume_by_example.py",
+            "bin/medpy_dicom_slices_to_volume.py",
+            "bin/medpy_dicom_to_4D.py",
+            "bin/medpy_diff.py",
+            "bin/medpy_extract_contour.py",
+            "bin/medpy_extract_min_max.py",
+            "bin/medpy_extract_sub_volume_auto.py",
+            "bin/medpy_extract_sub_volume_by_example.py",
+            "bin/medpy_extract_sub_volume.py",
+            "bin/medpy_fit_into_shape.py",
+            "bin/medpy_gradient.py",
+            "bin/medpy_graphcut_label_bgreduced.py",
+            "bin/medpy_graphcut_label_w_regional.py",
+            "bin/medpy_graphcut_label_wsplit.py",
+            "bin/medpy_graphcut_label.py",
+            "bin/medpy_graphcut_voxel.py",
+            "bin/medpy_grid.py",
+            "bin/medpy_info.py",
+            "bin/medpy_intensity_range_standardization.py",
+            "bin/medpy_intersection.py",
+            "bin/medpy_join_masks.py",
+            "bin/medpy_join_xd_to_xplus1d.py",
+            "bin/medpy_label_count.py",
+            "bin/medpy_label_fit_to_mask.py",
+            "bin/medpy_label_superimposition.py",
+            "bin/medpy_merge.py",
+            "bin/medpy_morphology.py",
+            "bin/medpy_resample.py",
+            "bin/medpy_reslice_3d_to_4d.py",
+            "bin/medpy_set_pixel_spacing.py",
+            "bin/medpy_shrink_image.py",
+            "bin/medpy_split_xd_to_xminus1d.py",
+            "bin/medpy_stack_sub_volumes.py",
+            "bin/medpy_swap_dimensions.py",
+            "bin/medpy_watershed.py",
+            "bin/medpy_zoom_image.py",
+        ],
+        **kw
+    )
 
-          **kw
-     )
 
 ### INSTALLATION
 try:
-    run_setup(not IS_PYPY)
+    run_setup(with_compilation=True)
 except BuildFailed:
-    BUILD_EXT_WARNING = ("WARNING: The medpy.graphcut.maxflow external C++ package could not be compiled, all graphcut functionality will be disabled. You might be missing Boost.Python or some build essentials like g++.")
-    print(('*' * 75))
+    BUILD_EXT_WARNING = "WARNING: The medpy.graphcut.maxflow external C++ package could not be compiled, all graphcut functionality will be disabled. You might be missing Boost.Python or some build essentials like g++."
+    print(("*" * 75))
     print(BUILD_EXT_WARNING)
     print("Failure information, if any, is above.")
     print("I'm retrying the build without the graphcut C++ module now.")
-    print(('*' * 75))
-    run_setup(False)
-    print(('*' * 75))
+    print(("*" * 75))
+    run_setup(with_compilation=False)
+    print(("*" * 75))
     print(BUILD_EXT_WARNING)
     print("Plain-Python installation succeeded.")
-    print(('*' * 75))
+    print(("*" * 75))
```

### Comparing `MedPy-0.4.0/medpy/metric/histogram.py` & `MedPy-0.5.0/medpy/metric/histogram.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,1252 +1,1311 @@
 # Copyright (C) 2013 Oskar Maier
-# 
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
-# 
+#
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
-# 
+#
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 # author Oskar Maier
 # version r0.1.0
 # since 2011-12-01
 # status Release
 
 # build-in modules
 import math
 
 # third-party modules
-import scipy
+import numpy
 
 # own modules
 
 # code
 # ////////////////////////////// #
 # Bin-by-bin comparison measures #
 # ////////////////////////////// #
 
-def minowski(h1, h2, p = 2): # 46..45..14,11..43..44 / 45 us for p=int(-inf..-24..-1,1..24..inf) / float @array, +20 us @list \w 100 bins
+
+def minowski(
+    h1, h2, p=2
+):  # 46..45..14,11..43..44 / 45 us for p=int(-inf..-24..-1,1..24..inf) / float @array, +20 us @list \w 100 bins
     r"""
     Minowski distance.
-    
+
     With :math:`p=2` equal to the Euclidean distance, with :math:`p=1` equal to the Manhattan distance,
     and the Chebyshev distance implementation represents the case of :math:`p=\pm inf`.
-    
+
     The Minowksi distance between two histograms :math:`H` and :math:`H'` of size :math:`m` is
     defined as:
-    
+
     .. math::
-    
-        d_p(H, H') = \left(\sum_{m=1}^M|H_m - H'_m|^p  
+
+        d_p(H, H') = \left(\sum_{m=1}^M|H_m - H'_m|^p
             \right)^{\frac{1}{p}}
 
     *Attributes:*
-    
+
     - a real metric
-    
+
     *Attributes for normalized histograms:*
-    
+
     - :math:`d(H, H')\in[0, \sqrt[p]{2}]`
     - :math:`d(H, H) = 0`
     - :math:`d(H, H') = d(H', H)`
-    
+
     *Attributes for not-normalized histograms:*
-    
+
     - :math:`d(H, H')\in[0, \infty)`
     - :math:`d(H, H) = 0`
     - :math:`d(H, H') = d(H', H)`
-    
+
     *Attributes for not-equal histograms:*
-    
+
     - not applicable
-    
+
     Parameters
     ----------
     h1 : sequence
         The first histogram.
     h2 : sequence
         The second histogram.
     p : float
         The :math:`p` value in the Minowksi distance formula.
-    
+
     Returns
     -------
     minowski : float
         Minowski distance.
-    
+
     Raises
     ------
     ValueError
         If ``p`` is zero.
     """
     h1, h2 = __prepare_histogram(h1, h2)
-    if 0 == p: raise ValueError('p can not be zero')
+    if 0 == p:
+        raise ValueError("p can not be zero")
     elif int == type(p):
-        if p > 0 and p < 25: return __minowski_low_positive_integer_p(h1, h2, p)
-        elif p < 0 and p > -25: return __minowski_low_negative_integer_p(h1, h2, p)
-    return math.pow(scipy.sum(scipy.power(scipy.absolute(h1 - h2), p)), 1./p)
+        if p > 0 and p < 25:
+            return __minowski_low_positive_integer_p(h1, h2, p)
+        elif p < 0 and p > -25:
+            return __minowski_low_negative_integer_p(h1, h2, p)
+    return math.pow(numpy.sum(numpy.power(numpy.absolute(h1 - h2), p)), 1.0 / p)
 
-def __minowski_low_positive_integer_p(h1, h2, p = 2): # 11..43 us for p = 1..24 \w 100 bins
+
+def __minowski_low_positive_integer_p(
+    h1, h2, p=2
+):  # 11..43 us for p = 1..24 \w 100 bins
     """
     A faster implementation of the Minowski distance for positive integer < 25.
     @note do not use this function directly, but the general @link minowski() method.
     @note the passed histograms must be scipy arrays.
     """
-    mult = scipy.absolute(h1 - h2)
+    mult = numpy.absolute(h1 - h2)
     dif = mult
-    for _ in range(p - 1): dif = scipy.multiply(dif, mult)
-    return math.pow(scipy.sum(dif), 1./p)
+    for _ in range(p - 1):
+        dif = numpy.multiply(dif, mult)
+    return math.pow(numpy.sum(dif), 1.0 / p)
+
 
-def __minowski_low_negative_integer_p(h1, h2, p = 2): # 14..46 us for p = -1..-24 \w 100 bins
+def __minowski_low_negative_integer_p(
+    h1, h2, p=2
+):  # 14..46 us for p = -1..-24 \w 100 bins
     """
     A faster implementation of the Minowski distance for negative integer > -25.
     @note do not use this function directly, but the general @link minowski() method.
     @note the passed histograms must be scipy arrays.
     """
-    mult = scipy.absolute(h1 - h2)
+    mult = numpy.absolute(h1 - h2)
     dif = mult
-    for _ in range(-p + 1): dif = scipy.multiply(dif, mult)
-    return math.pow(scipy.sum(1./dif), 1./p)
+    for _ in range(-p + 1):
+        dif = numpy.multiply(dif, mult)
+    return math.pow(numpy.sum(1.0 / dif), 1.0 / p)
+
 
-def manhattan(h1, h2): # # 7 us @array, 31 us @list \w 100 bins
+def manhattan(h1, h2):  # # 7 us @array, 31 us @list \w 100 bins
     r"""
     Equal to Minowski distance with :math:`p=1`.
-    
+
     See also
     --------
     minowski
     """
     h1, h2 = __prepare_histogram(h1, h2)
-    return scipy.sum(scipy.absolute(h1 - h2))
+    return numpy.sum(numpy.absolute(h1 - h2))
+
 
-def euclidean(h1, h2): # 9 us @array, 33 us @list \w 100 bins
+def euclidean(h1, h2):  # 9 us @array, 33 us @list \w 100 bins
     r"""
     Equal to Minowski distance with :math:`p=2`.
-    
+
     See also
     --------
     minowski
     """
     h1, h2 = __prepare_histogram(h1, h2)
-    return math.sqrt(scipy.sum(scipy.square(scipy.absolute(h1 - h2))))
+    return math.sqrt(numpy.sum(numpy.square(numpy.absolute(h1 - h2))))
+
 
-def chebyshev(h1, h2): # 12 us @array, 36 us @list \w 100 bins
+def chebyshev(h1, h2):  # 12 us @array, 36 us @list \w 100 bins
     r"""
     Chebyshev distance.
-    
+
     Also Tchebychev distance, Maximum or :math:`L_{\infty}` metric; equal to Minowski
     distance with :math:`p=+\infty`. For the case of :math:`p=-\infty`, use `chebyshev_neg`.
-    
+
     The Chebyshev distance between two histograms :math:`H` and :math:`H'` of size :math:`m` is
     defined as:
-    
+
     .. math::
-    
+
         d_{\infty}(H, H') = \max_{m=1}^M|H_m-H'_m|
-    
+
     *Attributes:*
-    
+
     - semimetric (triangle equation satisfied?)
-    
+
     *Attributes for normalized histograms:*
-    
+
     - :math:`d(H, H')\in[0, 1]`
     - :math:`d(H, H) = 0`
     - :math:`d(H, H') = d(H', H)`
-    
+
     *Attributes for not-normalized histograms:*
-    
+
     - :math:`d(H, H')\in[0, \infty)`
     - :math:`d(H, H) = 0`
     - :math:`d(H, H') = d(H', H)`
-    
+
     *Attributes for not-equal histograms:*
-    
+
     - not applicable
-    
+
     Parameters
     ----------
     h1 : sequence
         The first histogram.
     h2 : sequence
         The second histogram.
-    
+
     Returns
     -------
     chebyshev : float
         Chebyshev distance.
-    
+
     See also
     --------
     minowski, chebyshev_neg
     """
     h1, h2 = __prepare_histogram(h1, h2)
-    return max(scipy.absolute(h1 - h2))
+    return max(numpy.absolute(h1 - h2))
 
-def chebyshev_neg(h1, h2): # 12 us @array, 36 us @list \w 100 bins
+
+def chebyshev_neg(h1, h2):  # 12 us @array, 36 us @list \w 100 bins
     r"""
     Chebyshev negative distance.
-    
+
     Also Tchebychev distance, Minimum or :math:`L_{-\infty}` metric; equal to Minowski
     distance with :math:`p=-\infty`. For the case of :math:`p=+\infty`, use `chebyshev`.
-    
+
     The Chebyshev distance between two histograms :math:`H` and :math:`H'` of size :math:`m` is
     defined as:
-    
+
     .. math::
-    
+
         d_{-\infty}(H, H') = \min_{m=1}^M|H_m-H'_m|
-    
+
     *Attributes:*
 
     - semimetric (triangle equation satisfied?)
-    
+
     *Attributes for normalized histograms:*
 
     - :math:`d(H, H')\in[0, 1]`
     - :math:`d(H, H) = 0`
     - :math:`d(H, H') = d(H', H)`
-    
+
     *Attributes for not-normalized histograms:*
 
     - :math:`d(H, H')\in[0, \infty)`
     - :math:`d(H, H) = 0`
     - :math:`d(H, H') = d(H', H)`
-    
+
     *Attributes for not-equal histograms:*
 
     - not applicable
-    
+
     Parameters
     ----------
     h1 : sequence
         The first histogram.
     h2 : sequence
         The second histogram.
-    
+
     Returns
     -------
     chebyshev_neg : float
         Chebyshev negative distance.
-    
+
     See also
     --------
     minowski, chebyshev
     """
     h1, h2 = __prepare_histogram(h1, h2)
-    return min(scipy.absolute(h1 - h2))
+    return min(numpy.absolute(h1 - h2))
 
-def histogram_intersection(h1, h2): # 6 us @array, 30 us @list \w 100 bins
+
+def histogram_intersection(h1, h2):  # 6 us @array, 30 us @list \w 100 bins
     r"""
     Calculate the common part of two histograms.
-    
+
     The histogram intersection between two histograms :math:`H` and :math:`H'` of size :math:`m` is
     defined as:
-    
+
     .. math::
-    
+
         d_{\cap}(H, H') = \sum_{m=1}^M\min(H_m, H'_m)
-    
+
     *Attributes:*
 
     - a real metric
-    
+
     *Attributes for normalized histograms:*
 
     - :math:`d(H, H')\in[0, 1]`
     - :math:`d(H, H) = 1`
     - :math:`d(H, H') = d(H', H)`
-    
+
     *Attributes for not-normalized histograms:*
 
     - not applicable
-    
+
     *Attributes for not-equal histograms:*
 
     - not applicable
-    
+
     Parameters
     ----------
     h1 : sequence
         The first histogram, normalized.
     h2 : sequence
         The second histogram, normalized, same bins as ``h1``.
-    
+
     Returns
     -------
     histogram_intersection : float
         Intersection between the two histograms.
     """
     h1, h2 = __prepare_histogram(h1, h2)
-    return scipy.sum(scipy.minimum(h1, h2))
+    return numpy.sum(numpy.minimum(h1, h2))
+
 
-def histogram_intersection_1(h1, h2): # 7 us @array, 31 us @list \w 100 bins
+def histogram_intersection_1(h1, h2):  # 7 us @array, 31 us @list \w 100 bins
     r"""
     Turns the histogram intersection similarity into a distance measure for normalized,
     positive histograms.
-    
+
     .. math::
-    
+
         d_{\bar{\cos}}(H, H') = 1 - d_{\cap}(H, H')
-    
+
     See `histogram_intersection` for the definition of :math:`d_{\cap}(H, H')`.
-    
+
     *Attributes:*
 
     - semimetric
-    
+
     *Attributes for normalized histograms:*
 
     - :math:`d(H, H')\in[0, 1]`
     - :math:`d(H, H) = 0`
     - :math:`d(H, H') = d(H', H)`
-    
+
     *Attributes for not-normalized histograms:*
 
     - not applicable
-    
+
     *Attributes for not-equal histograms:*
 
     - not applicable
-    
+
     Parameters
     ----------
     h1 : sequence
         The first histogram, normalized.
     h2 : sequence
         The second histogram, normalized, same bins as ``h1``.
-    
+
     Returns
     -------
     histogram_intersection : float
         Intersection between the two histograms.
     """
-    return 1. - histogram_intersection(h1, h2)
+    return 1.0 - histogram_intersection(h1, h2)
 
-def relative_deviation(h1, h2): # 18 us @array, 42 us @list \w 100 bins
+
+def relative_deviation(h1, h2):  # 18 us @array, 42 us @list \w 100 bins
     r"""
     Calculate the deviation between two histograms.
-    
+
     The relative deviation between two histograms :math:`H` and :math:`H'` of size :math:`m` is
     defined as:
-    
+
     .. math::
-    
+
         d_{rd}(H, H') =
             \frac{
                 \sqrt{\sum_{m=1}^M(H_m - H'_m)^2}
               }{
                 \frac{1}{2}
                 \left(
                     \sqrt{\sum_{m=1}^M H_m^2} +
                     \sqrt{\sum_{m=1}^M {H'}_m^2}
                 \right)
               }
-    
+
     *Attributes:*
 
     - semimetric (triangle equation satisfied?)
-    
+
     *Attributes for normalized histograms:*
 
     - :math:`d(H, H')\in[0, \sqrt{2}]`
     - :math:`d(H, H) = 0`
     - :math:`d(H, H') = d(H', H)`
-    
+
     *Attributes for not-normalized histograms:*
 
     - :math:`d(H, H')\in[0, 2]`
     - :math:`d(H, H) = 0`
     - :math:`d(H, H') = d(H', H)`
-    
+
     *Attributes for not-equal histograms:*
 
-    - not applicable    
-    
+    - not applicable
+
     Parameters
     ----------
     h1 : sequence
         The first histogram.
     h2 : sequence
         The second histogram, same bins as ``h1``.
-    
+
     Returns
     -------
     relative_deviation : float
         Relative deviation between the two histograms.
     """
     h1, h2 = __prepare_histogram(h1, h2)
-    numerator = math.sqrt(scipy.sum(scipy.square(h1 - h2)))
-    denominator = (math.sqrt(scipy.sum(scipy.square(h1))) + math.sqrt(scipy.sum(scipy.square(h2)))) / 2.
+    numerator = math.sqrt(numpy.sum(numpy.square(h1 - h2)))
+    denominator = (
+        math.sqrt(numpy.sum(numpy.square(h1))) + math.sqrt(numpy.sum(numpy.square(h2)))
+    ) / 2.0
     return numerator / denominator
 
-def relative_bin_deviation(h1, h2): # 79 us @array, 104 us @list \w 100 bins
+
+def relative_bin_deviation(h1, h2):  # 79 us @array, 104 us @list \w 100 bins
     r"""
     Calculate the bin-wise deviation between two histograms.
-    
+
     The relative bin deviation between two histograms :math:`H` and :math:`H'` of size
     :math:`m` is defined as:
-    
+
     .. math::
-    
+
         d_{rbd}(H, H') = \sum_{m=1}^M
             \frac{
                 \sqrt{(H_m - H'_m)^2}
               }{
                 \frac{1}{2}
                 \left(
                     \sqrt{H_m^2} +
                     \sqrt{{H'}_m^2}
                 \right)
               }
-    
+
     *Attributes:*
 
     - a real metric
-    
+
     *Attributes for normalized histograms:*
 
     - :math:`d(H, H')\in[0, \infty)`
     - :math:`d(H, H) = 0`
     - :math:`d(H, H') = d(H', H)`
-    
+
     *Attributes for not-normalized histograms:*
 
     - :math:`d(H, H')\in[0, \infty)`
     - :math:`d(H, H) = 0`
     - :math:`d(H, H') = d(H', H)`
-    
+
     *Attributes for not-equal histograms:*
 
-    - not applicable 
-    
+    - not applicable
+
     Parameters
     ----------
     h1 : sequence
         The first histogram.
     h2 : sequence
         The second histogram, same bins as ``h1``.
-    
+
     Returns
     -------
     relative_bin_deviation : float
         Relative bin deviation between the two histograms.
     """
     h1, h2 = __prepare_histogram(h1, h2)
-    numerator = scipy.sqrt(scipy.square(h1 - h2))
-    denominator = (scipy.sqrt(scipy.square(h1)) + scipy.sqrt(scipy.square(h2))) / 2.
-    old_err_state = scipy.seterr(invalid='ignore') # divide through zero only occurs when the bin is zero in both histograms, in which case the division is 0/0 and leads to (and should lead to) 0
+    numerator = numpy.sqrt(numpy.square(h1 - h2))
+    denominator = (numpy.sqrt(numpy.square(h1)) + numpy.sqrt(numpy.square(h2))) / 2.0
+    old_err_state = numpy.seterr(
+        invalid="ignore"
+    )  # divide through zero only occurs when the bin is zero in both histograms, in which case the division is 0/0 and leads to (and should lead to) 0
     result = numerator / denominator
-    scipy.seterr(**old_err_state)
-    result[scipy.isnan(result)] = 0 # faster than scipy.nan_to_num, which checks for +inf and -inf also
-    return scipy.sum(result)
+    numpy.seterr(**old_err_state)
+    result[
+        numpy.isnan(result)
+    ] = 0  # faster than numpy.nan_to_num, which checks for +inf and -inf also
+    return numpy.sum(result)
 
-def chi_square(h1, h2): # 23 us @array, 49 us @list \w 100
+
+def chi_square(h1, h2):  # 23 us @array, 49 us @list \w 100
     r"""
     Chi-square distance.
-    
+
     Measure how unlikely it is that one distribution (histogram) was drawn from the
     other. The Chi-square distance between two histograms :math:`H` and :math:`H'` of size
     :math:`m` is defined as:
-    
+
     .. math::
-    
+
         d_{\chi^2}(H, H') = \sum_{m=1}^M
             \frac{
                 (H_m - H'_m)^2
             }{
                 H_m + H'_m
             }
-    
+
     *Attributes:*
 
     - semimetric
-    
+
     *Attributes for normalized histograms:*
 
     - :math:`d(H, H')\in[0, 2]`
     - :math:`d(H, H) = 0`
     - :math:`d(H, H') = d(H', H)`
-    
+
     *Attributes for not-normalized histograms:*
 
     - :math:`d(H, H')\in[0, \infty)`
     - :math:`d(H, H) = 0`
     - :math:`d(H, H') = d(H', H)`
-    
+
     *Attributes for not-equal histograms:*
 
-    - not applicable     
-    
+    - not applicable
+
     Parameters
     ----------
     h1 : sequence
         The first histogram.
     h2 : sequence
         The second histogram.
-    
+
     Returns
     -------
     chi_square : float
         Chi-square distance.
     """
     h1, h2 = __prepare_histogram(h1, h2)
-    old_err_state = scipy.seterr(invalid='ignore') # divide through zero only occurs when the bin is zero in both histograms, in which case the division is 0/0 and leads to (and should lead to) 0
-    result = scipy.square(h1 - h2) / (h1 + h2)
-    scipy.seterr(**old_err_state)
-    result[scipy.isnan(result)] = 0 # faster than scipy.nan_to_num, which checks for +inf and -inf also
-    return scipy.sum(result)
+    old_err_state = numpy.seterr(
+        invalid="ignore"
+    )  # divide through zero only occurs when the bin is zero in both histograms, in which case the division is 0/0 and leads to (and should lead to) 0
+    result = numpy.square(h1 - h2) / (h1 + h2)
+    numpy.seterr(**old_err_state)
+    result[
+        numpy.isnan(result)
+    ] = 0  # faster than numpy.nan_to_num, which checks for +inf and -inf also
+    return numpy.sum(result)
+
 
-    
-def kullback_leibler(h1, h2): # 83 us @array, 109 us @list \w 100 bins
+def kullback_leibler(h1, h2):  # 83 us @array, 109 us @list \w 100 bins
     r"""
     Kullback-Leibler divergence.
-    
+
     Compute how inefficient it would to be code one histogram into another.
     Actually computes :math:`\frac{d_{KL}(h1, h2) + d_{KL}(h2, h1)}{2}` to achieve symmetry.
-    
+
     The Kullback-Leibler divergence between two histograms :math:`H` and :math:`H'` of size
     :math:`m` is defined as:
-    
+
     .. math::
-    
+
         d_{KL}(H, H') = \sum_{m=1}^M H_m\log\frac{H_m}{H'_m}
-    
+
     *Attributes:*
 
     - quasimetric (but made symetric)
-    
+
     *Attributes for normalized histograms:*
 
     - :math:`d(H, H')\in[0, \infty)`
     - :math:`d(H, H) = 0`
     - :math:`d(H, H') = d(H', H)`
-    
+
     *Attributes for not-normalized histograms:*
 
     - not applicable
-    
+
     *Attributes for not-equal histograms:*
 
     - not applicable
-        
+
     Parameters
     ----------
     h1 : sequence
         The first histogram, where h1[i] > 0 for any i such that h2[i] > 0, normalized.
     h2 : sequence
         The second histogram, where h2[i] > 0 for any i such that h1[i] > 0, normalized, same bins as ``h1``.
-    
+
     Returns
     -------
     kullback_leibler : float
         Kullback-Leibler divergence.
 
     """
-    old_err_state = scipy.seterr(divide='raise')
+    old_err_state = numpy.seterr(divide="raise")
     try:
         h1, h2 = __prepare_histogram(h1, h2)
-        result = (__kullback_leibler(h1, h2) + __kullback_leibler(h2, h1)) / 2.
-        scipy.seterr(**old_err_state)
+        result = (__kullback_leibler(h1, h2) + __kullback_leibler(h2, h1)) / 2.0
+        numpy.seterr(**old_err_state)
         return result
     except FloatingPointError:
-        scipy.seterr(**old_err_state)
-        raise ValueError('h1 can only contain zero values where h2 also contains zero values and vice-versa')
-    
-def __kullback_leibler(h1, h2): # 36.3 us
+        numpy.seterr(**old_err_state)
+        raise ValueError(
+            "h1 can only contain zero values where h2 also contains zero values and vice-versa"
+        )
+
+
+def __kullback_leibler(h1, h2):  # 36.3 us
     """
     The actual KL implementation. @see kullback_leibler() for details.
-    Expects the histograms to be of type scipy.ndarray.
+    Expects the histograms to be of type numpy.ndarray.
     """
-    result = h1.astype(scipy.float_)
+    result = h1.astype(float)
     mask = h1 != 0
-    result[mask] = scipy.multiply(h1[mask], scipy.log(h1[mask] / h2[mask]))
-    return scipy.sum(result)
-       
-def jensen_shannon(h1, h2): # 85 us @array, 110 us @list \w 100 bins
+    result[mask] = numpy.multiply(h1[mask], numpy.log(h1[mask] / h2[mask]))
+    return numpy.sum(result)
+
+
+def jensen_shannon(h1, h2):  # 85 us @array, 110 us @list \w 100 bins
     r"""
     Jensen-Shannon divergence.
-    
+
     A symmetric and numerically more stable empirical extension of the Kullback-Leibler
     divergence.
-    
+
     The Jensen Shannon divergence between two histograms :math:`H` and :math:`H'` of size
     :math:`m` is defined as:
-    
+
     .. math::
-    
+
         d_{JSD}(H, H') =
             \frac{1}{2} d_{KL}(H, H^*) +
             \frac{1}{2} d_{KL}(H', H^*)
-    
+
     with :math:`H^*=\frac{1}{2}(H + H')`.
-    
+
     *Attributes:*
 
     - semimetric
-    
+
     *Attributes for normalized histograms:*
 
     - :math:`d(H, H')\in[0, 1]`
     - :math:`d(H, H) = 0`
     - :math:`d(H, H') = d(H', H)`
-    
+
     *Attributes for not-normalized histograms:*
 
     - :math:`d(H, H')\in[0, \infty)`
     - :math:`d(H, H) = 0`
     - :math:`d(H, H') = d(H', H)`
-    
+
     *Attributes for not-equal histograms:*
 
     - not applicable
-    
+
     Parameters
     ----------
     h1 : sequence
         The first histogram.
     h2 : sequence
         The second histogram, same bins as ``h1``.
-    
+
     Returns
     -------
     jensen_shannon : float
-        Jensen-Shannon divergence.    
+        Jensen-Shannon divergence.
 
     """
     h1, h2 = __prepare_histogram(h1, h2)
-    s = (h1 + h2) / 2.
-    return __kullback_leibler(h1, s) / 2. + __kullback_leibler(h2, s) / 2.
-    
-def fidelity_based(h1, h2): # 25 us @array, 51 us @list \w 100 bins
+    s = (h1 + h2) / 2.0
+    return __kullback_leibler(h1, s) / 2.0 + __kullback_leibler(h2, s) / 2.0
+
+
+def fidelity_based(h1, h2):  # 25 us @array, 51 us @list \w 100 bins
     r"""
     Fidelity based distance.
-    
+
     Also Bhattacharyya distance; see also the extensions `noelle_1` to `noelle_5`.
-    
+
     The metric between two histograms :math:`H` and :math:`H'` of size :math:`m` is defined as:
-    
+
     .. math::
-    
+
         d_{F}(H, H') = \sum_{m=1}^M\sqrt{H_m * H'_m}
-    
-    
+
+
     *Attributes:*
 
     - not a metric, a similarity
-    
+
     *Attributes for normalized histograms:*
 
     - :math:`d(H, H')\in[0, 1]`
     - :math:`d(H, H) = 1`
     - :math:`d(H, H') = d(H', H)`
-    
+
     *Attributes for not-normalized histograms:*
 
     - not applicable
-    
+
     *Attributes for not-equal histograms:*
 
     - not applicable
-    
+
     Parameters
     ----------
     h1 : sequence
         The first histogram, normalized.
     h2 : sequence
         The second histogram, normalized, same bins as ``h1``.
-    
+
     Returns
     -------
     fidelity_based : float
         Fidelity based distance.
-    
+
     Notes
     -----
     The fidelity between two histograms :math:`H` and :math:`H'` is the same as the
     cosine between their square roots :math:`\sqrt{H}` and :math:`\sqrt{H'}`.
     """
     h1, h2 = __prepare_histogram(h1, h2)
-    result = scipy.sum(scipy.sqrt(h1 * h2))
-    result = 0 if 0 > result else result # for rounding errors
-    result = 1 if 1 < result else result # for rounding errors
+    result = numpy.sum(numpy.sqrt(h1 * h2))
+    result = 0 if 0 > result else result  # for rounding errors
+    result = 1 if 1 < result else result  # for rounding errors
     return result
 
-def noelle_1(h1, h2): # 26 us @array, 52 us @list \w 100 bins
+
+def noelle_1(h1, h2):  # 26 us @array, 52 us @list \w 100 bins
     r"""
     Extension of `fidelity_based` proposed by [1]_.
-    
+
     .. math::
-    
+
         d_{\bar{F}}(H, H') = 1 - d_{F}(H, H')
-    
+
     See `fidelity_based` for the definition of :math:`d_{F}(H, H')`.
-    
+
     *Attributes:*
 
     - semimetric
-    
+
     *Attributes for normalized histograms:*
 
     - :math:`d(H, H')\in[0, 1]`
     - :math:`d(H, H) = 0`
     - :math:`d(H, H') = d(H', H)`
-    
+
     *Attributes for not-normalized histograms:*
 
     - not applicable
-    
+
     *Attributes for not-equal histograms:*
 
     - not applicable
-    
+
     Parameters
     ----------
     h1 : sequence
         The first histogram, normalized.
     h2 : sequence
         The second histogram, normalized, same bins as ``h1``.
-    
+
     Returns
     -------
     fidelity_based : float
         Fidelity based distance.
-    
+
     References
     ----------
     .. [1] M. Noelle "Distribution Distance Measures Applied to 3-D Object Recognition", 2003
     """
-    return 1. - fidelity_based(h1, h2)
+    return 1.0 - fidelity_based(h1, h2)
 
-def noelle_2(h1, h2): # 26 us @array, 52 us @list \w 100 bins
+
+def noelle_2(h1, h2):  # 26 us @array, 52 us @list \w 100 bins
     r"""
     Extension of `fidelity_based` proposed by [1]_.
-    
+
     .. math::
-        
+
         d_{\sqrt{1-F}}(H, H') = \sqrt{1 - d_{F}(H, H')}
-    
+
     See `fidelity_based` for the definition of :math:`d_{F}(H, H')`.
-    
+
     *Attributes:*
 
     - metric
-    
+
     *Attributes for normalized histograms:*
 
     - :math:`d(H, H')\in[0, 1]`
     - :math:`d(H, H) = 0`
     - :math:`d(H, H') = d(H', H)`
-    
+
     *Attributes for not-normalized histograms:*
 
     - not applicable
-    
+
     *Attributes for not-equal histograms:*
 
     - not applicable
-    
+
     Parameters
     ----------
     h1 : sequence
         The first histogram, normalized.
     h2 : sequence
         The second histogram, normalized, same bins as ``h1``.
-    
+
     Returns
     -------
     fidelity_based : float
         Fidelity based distance.
-    
+
     References
     ----------
     .. [1] M. Noelle "Distribution Distance Measures Applied to 3-D Object Recognition", 2003
     """
-    return math.sqrt(1. - fidelity_based(h1, h2))
+    return math.sqrt(1.0 - fidelity_based(h1, h2))
 
-def noelle_3(h1, h2): # 26 us @array, 52 us @list \w 100 bins
+
+def noelle_3(h1, h2):  # 26 us @array, 52 us @list \w 100 bins
     r"""
     Extension of `fidelity_based` proposed by [1]_.
-    
+
     .. math::
-    
+
         d_{\log(2-F)}(H, H') = \log(2 - d_{F}(H, H'))
-    
+
     See `fidelity_based` for the definition of :math:`d_{F}(H, H')`.
-        
+
     *Attributes:*
 
     - semimetric
-    
+
     *Attributes for normalized histograms:*
 
     - :math:`d(H, H')\in[0, log(2)]`
     - :math:`d(H, H) = 0`
     - :math:`d(H, H') = d(H', H)`
-    
+
     *Attributes for not-normalized histograms:*
 
     - not applicable
-    
+
     *Attributes for not-equal histograms:*
 
     - not applicable
-    
+
     Parameters
     ----------
     h1 : sequence
         The first histogram, normalized.
     h2 : sequence
         The second histogram, normalized, same bins as ``h1``.
-    
+
     Returns
     -------
     fidelity_based : float
         Fidelity based distance.
-    
+
     References
     ----------
     .. [1] M. Noelle "Distribution Distance Measures Applied to 3-D Object Recognition", 2003
     """
     return math.log(2 - fidelity_based(h1, h2))
 
-def noelle_4(h1, h2): # 26 us @array, 52 us @list \w 100 bins
+
+def noelle_4(h1, h2):  # 26 us @array, 52 us @list \w 100 bins
     r"""
     Extension of `fidelity_based` proposed by [1]_.
-    
+
     .. math::
-    
+
         d_{\arccos F}(H, H') = \frac{2}{\pi} \arccos d_{F}(H, H')
-    
+
     See `fidelity_based` for the definition of :math:`d_{F}(H, H')`.
-            
+
     *Attributes:*
 
     - metric
-    
+
     *Attributes for normalized histograms:*
 
     - :math:`d(H, H')\in[0, 1]`
     - :math:`d(H, H) = 0`
     - :math:`d(H, H') = d(H', H)`
-    
+
     *Attributes for not-normalized histograms:*
 
     - not applicable
-    
+
     *Attributes for not-equal histograms:*
 
     - not applicable
-    
+
     Parameters
     ----------
     h1 : sequence
         The first histogram, normalized.
     h2 : sequence
         The second histogram, normalized, same bins as ``h1``.
-    
+
     Returns
     -------
     fidelity_based : float
         Fidelity based distance.
-    
+
     References
     ----------
     .. [1] M. Noelle "Distribution Distance Measures Applied to 3-D Object Recognition", 2003
     """
-    return 2. / math.pi * math.acos(fidelity_based(h1, h2))
+    return 2.0 / math.pi * math.acos(fidelity_based(h1, h2))
+
 
-def noelle_5(h1, h2): # 26 us @array, 52 us @list \w 100 bins
+def noelle_5(h1, h2):  # 26 us @array, 52 us @list \w 100 bins
     r"""
     Extension of `fidelity_based` proposed by [1]_.
-    
+
     .. math::
-    
+
         d_{\sin F}(H, H') = \sqrt{1 -d_{F}^2(H, H')}
-    
+
     See `fidelity_based` for the definition of :math:`d_{F}(H, H')`.
-                
+
     *Attributes:*
 
     - metric
-    
+
     *Attributes for normalized histograms:*
 
     - :math:`d(H, H')\in[0, 1]`
     - :math:`d(H, H) = 0`
     - :math:`d(H, H') = d(H', H)`
-    
+
     *Attributes for not-normalized histograms:*
 
     - not applicable
-    
+
     *Attributes for not-equal histograms:*
 
     - not applicable
-    
+
     Parameters
     ----------
     h1 : sequence
         The first histogram, normalized.
     h2 : sequence
         The second histogram, normalized, same bins as ``h1``.
-    
+
     Returns
     -------
     fidelity_based : float
         Fidelity based distance.
-    
+
     References
     ----------
     .. [1] M. Noelle "Distribution Distance Measures Applied to 3-D Object Recognition", 2003
     """
     return math.sqrt(1 - math.pow(fidelity_based(h1, h2), 2))
 
 
-def cosine_alt(h1, h2): # 17 us @array, 42 us @list \w 100 bins
+def cosine_alt(h1, h2):  # 17 us @array, 42 us @list \w 100 bins
     r"""
     Alternative implementation of the `cosine` distance measure.
-    
+
     Notes
     -----
     Under development.
     """
     h1, h2 = __prepare_histogram(h1, h2)
-    return -1 * float(scipy.sum(h1 * h2)) / (scipy.sum(scipy.power(h1, 2)) * scipy.sum(scipy.power(h2, 2)))
+    return (
+        -1
+        * float(numpy.sum(h1 * h2))
+        / (numpy.sum(numpy.power(h1, 2)) * numpy.sum(numpy.power(h2, 2)))
+    )
 
-def cosine(h1, h2): # 17 us @array, 42 us @list \w 100 bins
+
+def cosine(h1, h2):  # 17 us @array, 42 us @list \w 100 bins
     r"""
     Cosine simmilarity.
-    
+
     Compute the angle between the two histograms in vector space irrespective of their
     length. The cosine similarity between two histograms :math:`H` and :math:`H'` of size
     :math:`m` is defined as:
-    
+
     .. math::
-    
+
         d_{\cos}(H, H') = \cos\alpha = \frac{H * H'}{\|H\| \|H'\|} = \frac{\sum_{m=1}^M H_m*H'_m}{\sqrt{\sum_{m=1}^M H_m^2} * \sqrt{\sum_{m=1}^M {H'}_m^2}}
-    
-    
+
+
     *Attributes:*
 
     - not a metric, a similarity
-    
+
     *Attributes for normalized histograms:*
 
     - :math:`d(H, H')\in[0, 1]`
     - :math:`d(H, H) = 1`
     - :math:`d(H, H') = d(H', H)`
-    
+
     *Attributes for not-normalized histograms:*
 
     - :math:`d(H, H')\in[-1, 1]`
     - :math:`d(H, H) = 1`
     - :math:`d(H, H') = d(H', H)`
-    
+
     *Attributes for not-equal histograms:*
 
-    - not applicable    
-        
+    - not applicable
+
     Parameters
     ----------
     h1 : sequence
         The first histogram.
     h2 : sequence
         The second histogram, same bins as ``h1``.
-    
+
     Returns
     -------
     cosine : float
         Cosine simmilarity.
-        
+
     Notes
     -----
     The resulting similarity ranges from -1 meaning exactly opposite, to 1 meaning
     exactly the same, with 0 usually indicating independence, and in-between values
     indicating intermediate similarity or dissimilarity.
     """
     h1, h2 = __prepare_histogram(h1, h2)
-    return scipy.sum(h1 * h2) / math.sqrt(scipy.sum(scipy.square(h1)) * scipy.sum(scipy.square(h2)))
+    return numpy.sum(h1 * h2) / math.sqrt(
+        numpy.sum(numpy.square(h1)) * numpy.sum(numpy.square(h2))
+    )
 
-def cosine_1(h1, h2): # 18 us @array, 43 us @list \w 100 bins
+
+def cosine_1(h1, h2):  # 18 us @array, 43 us @list \w 100 bins
     r"""
     Cosine simmilarity.
-    
+
     Turns the cosine similarity into a distance measure for normalized, positive
     histograms.
-    
+
     .. math::
-    
+
         d_{\bar{\cos}}(H, H') = 1 - d_{\cos}(H, H')
-    
+
     See `cosine` for the definition of :math:`d_{\cos}(H, H')`.
-    
+
     *Attributes:*
 
     - metric
-    
+
     *Attributes for normalized histograms:*
 
     - :math:`d(H, H')\in[0, 1]`
     - :math:`d(H, H) = 0`
     - :math:`d(H, H') = d(H', H)`
-    
+
     *Attributes for not-normalized histograms:*
 
     - not applicable
-    
+
     *Attributes for not-equal histograms:*
 
     - not applicable
-    
+
     Parameters
     ----------
     h1 : sequence
         The first histogram, normalized.
     h2 : sequence
         The second histogram, normalized, same bins as ``h1``.
-        
+
         Returns
     -------
     cosine : float
         Cosine distance.
     """
-    return 1. - cosine(h1, h2)
+    return 1.0 - cosine(h1, h2)
 
-def cosine_2(h1, h2): # 19 us @array, 44 us @list \w 100 bins
+
+def cosine_2(h1, h2):  # 19 us @array, 44 us @list \w 100 bins
     r"""
     Cosine simmilarity.
-    
+
     Turns the cosine similarity into a distance measure for normalized, positive
     histograms.
-    
+
     .. math::
-    
+
         d_{\bar{\cos}}(H, H') = 1 - \frac{2*\arccos d_{\cos}(H, H')}{pi}
-    
+
     See `cosine` for the definition of :math:`d_{\cos}(H, H')`.
-    
+
     *Attributes:*
 
     - metric
-    
+
     *Attributes for normalized histograms:*
 
     - :math:`d(H, H')\in[0, 1]`
     - :math:`d(H, H) = 0`
     - :math:`d(H, H') = d(H', H)`
-    
+
     *Attributes for not-normalized histograms:*
 
     - not applicable
-    
+
     *Attributes for not-equal histograms:*
 
     - not applicable
-    
+
     Parameters
     ----------
     h1 : sequence
         The first histogram, normalized.
     h2 : sequence
         The second histogram, normalized, same bins as ``h1``.
-        
+
         Returns
     -------
     cosine : float
-        Cosine distance. 
+        Cosine distance.
     """
-    return 1. - (2 * cosine(h1, h2)) / math.pi
+    return 1.0 - (2 * cosine(h1, h2)) / math.pi
+
 
-def correlate(h1, h2): # 31 us @array, 55 us @list \w 100 bins
+def correlate(h1, h2):  # 31 us @array, 55 us @list \w 100 bins
     r"""
     Correlation between two histograms.
-    
+
     The histogram correlation between two histograms :math:`H` and :math:`H'` of size :math:`m`
     is defined as:
-    
+
     .. math::
-    
-        d_{corr}(H, H') = 
+
+        d_{corr}(H, H') =
         \frac{
             \sum_{m=1}^M (H_m-\bar{H}) \cdot (H'_m-\bar{H'})
         }{
             \sqrt{\sum_{m=1}^M (H_m-\bar{H})^2 \cdot \sum_{m=1}^M (H'_m-\bar{H'})^2}
         }
-    
+
     with :math:`\bar{H}` and :math:`\bar{H'}` being the mean values of :math:`H` resp. :math:`H'`
-        
+
     *Attributes:*
 
     - not a metric, a similarity
-    
+
     *Attributes for normalized histograms:*
 
     - :math:`d(H, H')\in[-1, 1]`
     - :math:`d(H, H) = 1`
     - :math:`d(H, H') = d(H', H)`
-    
+
     *Attributes for not-normalized histograms:*
 
     - :math:`d(H, H')\in[-1, 1]`
     - :math:`d(H, H) = 1`
     - :math:`d(H, H') = d(H', H)`
-    
+
     *Attributes for not-equal histograms:*
 
     - not applicable
-    
+
     Parameters
     ----------
     h1 : sequence
         The first histogram.
     h2 : sequence
         The second histogram, same bins as ``h1``.
-    
+
     Returns
     -------
     correlate : float
         Correlation between the histograms.
-        
+
     Notes
     -----
     Returns 0 if one of h1 or h2 contain only zeros.
-    
+
     """
     h1, h2 = __prepare_histogram(h1, h2)
-    h1m = h1 - scipy.sum(h1) / float(h1.size)
-    h2m = h2 - scipy.sum(h2) / float(h2.size)
-    a = scipy.sum(scipy.multiply(h1m, h2m))
-    b = math.sqrt(scipy.sum(scipy.square(h1m)) * scipy.sum(scipy.square(h2m)))
+    h1m = h1 - numpy.sum(h1) / float(h1.size)
+    h2m = h2 - numpy.sum(h2) / float(h2.size)
+    a = numpy.sum(numpy.multiply(h1m, h2m))
+    b = math.sqrt(numpy.sum(numpy.square(h1m)) * numpy.sum(numpy.square(h2m)))
     return 0 if 0 == b else a / b
 
-def correlate_1(h1, h2): # 32 us @array, 56 us @list \w 100 bins
+
+def correlate_1(h1, h2):  # 32 us @array, 56 us @list \w 100 bins
     r"""
     Correlation distance.
-    
+
     Turns the histogram correlation into a distance measure for normalized, positive
     histograms.
-    
+
     .. math::
-    
+
         d_{\bar{corr}}(H, H') = 1-\frac{d_{corr}(H, H')}{2}.
-    
+
     See `correlate` for the definition of :math:`d_{corr}(H, H')`.
-    
+
     *Attributes:*
 
     - semimetric
-    
+
     *Attributes for normalized histograms:*
 
     - :math:`d(H, H')\in[0, 1]`
     - :math:`d(H, H) = 0`
     - :math:`d(H, H') = d(H', H)`
-    
+
     *Attributes for not-normalized histograms:*
 
     - :math:`d(H, H')\in[0, 1]`
     - :math:`d(H, H) = 0`
     - :math:`d(H, H') = d(H', H)`
-    
+
     *Attributes for not-equal histograms:*
 
     - not applicable
-    
+
     Parameters
     ----------
     h1 : sequence
         The first histogram.
     h2 : sequence
         The second histogram, same bins as ``h1``.
-    
+
     Returns
     -------
     correlate : float
         Correlation distnace between the histograms.
-        
+
     Notes
     -----
     Returns 0.5 if one of h1 or h2 contains only zeros.
     """
-    return (1. - correlate(h1, h2))/2.
+    return (1.0 - correlate(h1, h2)) / 2.0
 
 
 # ///////////////////////////// #
 # Cross-bin comparison measures #
 # ///////////////////////////// #
 
+
 def quadratic_forms(h1, h2):
     r"""
     Quadrativ forms metric.
-    
+
     Notes
     -----
     UNDER DEVELOPMENT
-    
+
     This distance measure shows very strange behaviour. The expression
     transpose(h1-h2) * A * (h1-h2) yields egative values that can not be processed by the
     square root. Some examples::
-    
+
         h1        h2                                          transpose(h1-h2) * A * (h1-h2)
         [1, 0] to [0.0, 1.0] :                                -2.0
         [1, 0] to [0.5, 0.5] :                                 0.0
         [1, 0] to [0.6666666666666667, 0.3333333333333333] :   0.111111111111
         [1, 0] to [0.75, 0.25] :                               0.0833333333333
         [1, 0] to [0.8, 0.2] :                                 0.06
         [1, 0] to [0.8333333333333334, 0.16666666666666666] :  0.0444444444444
         [1, 0] to [0.8571428571428572, 0.14285714285714285] :  0.0340136054422
         [1, 0] to [0.875, 0.125] :                             0.0267857142857
         [1, 0] to [0.8888888888888888, 0.1111111111111111] :   0.0216049382716
         [1, 0] to [0.9, 0.1] :                                 0.0177777777778
         [1, 0] to [1, 0]:                                      0.0
-    
+
     It is clearly undesireable to recieve negative values and even worse to get a value
     of zero for other cases than the same histograms.
     """
     h1, h2 = __prepare_histogram(h1, h2)
     A = __quadratic_forms_matrix_euclidean(h1, h2)
-    return math.sqrt((h1-h2).dot(A.dot(h1-h2))) # transpose(h1-h2) * A * (h1-h2)
-    
+    return math.sqrt((h1 - h2).dot(A.dot(h1 - h2)))  # transpose(h1-h2) * A * (h1-h2)
+
+
 def __quadratic_forms_matrix_euclidean(h1, h2):
     r"""
     Compute the bin-similarity matrix for the quadratic form distance measure.
     The matric :math:`A` for two histograms :math:`H` and :math:`H'` of size :math:`m` and
     :math:`n` respectively is defined as
-    
+
     .. math::
-    
+
         A_{m,n} = 1 - \frac{d_2(H_m, {H'}_n)}{d_{max}}
-    
+
     with
-    
+
     .. math::
-    
+
        d_{max} = \max_{m,n}d_2(H_m, {H'}_n)
-    
+
     See also
     --------
     quadratic_forms
     """
-    A = scipy.repeat(h2[:,scipy.newaxis], h1.size, 1) # repeat second array to form a matrix
-    A = scipy.absolute(A - h1) # euclidean distances
+    A = numpy.repeat(
+        h2[:, numpy.newaxis], h1.size, 1
+    )  # repeat second array to form a matrix
+    A = numpy.absolute(A - h1)  # euclidean distances
     return 1 - (A / float(A.max()))
 
 
 # //////////////// #
 # Helper functions #
 # //////////////// #
 
+
 def __prepare_histogram(h1, h2):
-    """Convert the histograms to scipy.ndarrays if required."""
-    h1 = h1 if scipy.ndarray == type(h1) else scipy.asarray(h1)
-    h2 = h2 if scipy.ndarray == type(h2) else scipy.asarray(h2)
+    """Convert the histograms to numpy.ndarrays if required."""
+    h1 = h1 if numpy.ndarray == type(h1) else numpy.asarray(h1)
+    h2 = h2 if numpy.ndarray == type(h2) else numpy.asarray(h2)
     if h1.shape != h2.shape or h1.size != h2.size:
-        raise ValueError('h1 and h2 must be of same shape and size')
+        raise ValueError("h1 and h2 must be of same shape and size")
     return h1, h2
```

### Comparing `MedPy-0.4.0/medpy/metric/image.py` & `MedPy-0.5.0/medpy/metric/image.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Copyright (C) 2013 Oskar Maier
-# 
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
-# 
+#
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
-# 
+#
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 # author Oskar Maier
 # version r0.1.0
 # since 2013-07-09
 # status Release
@@ -22,99 +22,105 @@
 
 # third-party modules
 import numpy
 
 # own modules
 from ..core import ArgumentError
 
+
 # code
 def mutual_information(i1, i2, bins=256):
     r"""
     Computes the mutual information (MI) (a measure of entropy) between two images.
 
     MI is not real metric, but a symmetric and nonnegative similarity measures that
     takes high values for similar images. Negative values are also possible.
-    
+
     Intuitively, mutual information measures the information that ``i1`` and ``i2`` share: it
     measures how much knowing one of these variables reduces uncertainty about the other.
-    
+
     The Entropy is defined as:
-    
+
     .. math::
-    
+
         H(X) = - \sum_i p(g_i) * ln(p(g_i)
 
     with :math:`p(g_i)` being the intensity probability of the images grey value :math:`g_i`.
-    
+
     Assuming two images :math:`R` and :math:`T`, the mutual information is then computed by comparing the
     images entropy values (i.e. a measure how well-structured the common histogram is).
     The distance metric is then calculated as follows:
-    
+
     .. math::
-    
+
         MI(R,T) = H(R) + H(T) - H(R,T) = H(R) - H(R|T) = H(T) - H(T|R)
-    
+
     A maximization of the mutual information is equal to a minimization of the joint
     entropy.
-    
+
     Parameters
     ----------
     i1 : array_like
         The first image.
     i2 : array_like
         The second image.
     bins : integer
         The number of histogram bins (squared for the joined histogram).
-    
+
     Returns
     -------
     mutual_information : float
         The mutual information distance value between the supplied images.
-    
+
     Raises
     ------
     ArgumentError
         If the supplied arrays are of different shape.
     """
     # pre-process function arguments
     i1 = numpy.asarray(i1)
     i2 = numpy.asarray(i2)
-    
+
     # validate function arguments
     if not i1.shape == i2.shape:
-        raise ArgumentError('the two supplied array-like sequences i1 and i2 must be of the same shape')
-    
+        raise ArgumentError(
+            "the two supplied array-like sequences i1 and i2 must be of the same shape"
+        )
+
     # compute i1 and i2 histogram range
     i1_range = __range(i1, bins)
     i2_range = __range(i2, bins)
-    
+
     # compute joined and separated normed histograms
-    i1i2_hist, _, _ = numpy.histogram2d(i1.flatten(), i2.flatten(), bins=bins, range=[i1_range, i2_range]) # Note: histogram2d does not flatten array on its own
+    i1i2_hist, _, _ = numpy.histogram2d(
+        i1.flatten(), i2.flatten(), bins=bins, range=[i1_range, i2_range]
+    )  # Note: histogram2d does not flatten array on its own
     i1_hist, _ = numpy.histogram(i1, bins=bins, range=i1_range)
     i2_hist, _ = numpy.histogram(i2, bins=bins, range=i2_range)
-    
+
     # compute joined and separated entropy
     i1i2_entropy = __entropy(i1i2_hist)
     i1_entropy = __entropy(i1_hist)
     i2_entropy = __entropy(i2_hist)
-    
+
     # compute and return the mutual information distance
     return i1_entropy + i2_entropy - i1i2_entropy
 
+
 def __range(a, bins):
-    '''Compute the histogram range of the values in the array a according to
-    scipy.stats.histogram.'''
+    """Compute the histogram range of the values in the array a according to
+    scipy.stats.histogram."""
     a = numpy.asarray(a)
     a_max = a.max()
     a_min = a.min()
     s = 0.5 * (a_max - a_min) / float(bins - 1)
     return (a_min - s, a_max + s)
- 
+
+
 def __entropy(data):
-    '''Compute entropy of the flattened data set (e.g. a density distribution).'''
+    """Compute entropy of the flattened data set (e.g. a density distribution)."""
     # normalize and convert to float
-    data = data/float(numpy.sum(data))
+    data = data / float(numpy.sum(data))
     # for each grey-value g with a probability p(g) = 0, the entropy is defined as 0, therefore we remove these values and also flatten the histogram
     data = data[numpy.nonzero(data)]
     # compute entropy
-    return -1. * numpy.sum(data * numpy.log2(data))
-    
+    return -1.0 * numpy.sum(data * numpy.log2(data))
```

### Comparing `MedPy-0.4.0/medpy/metric/binary.py` & `MedPy-0.5.0/medpy/metric/binary.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,319 +1,336 @@
 # Copyright (C) 2013 Oskar Maier
-# 
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
-# 
+#
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
-# 
+#
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 # author Oskar Maier
 # version r0.1.1
 # since 2014-03-13
 # status Release
 
 # build-in modules
 
 # third-party modules
 import numpy
-from scipy.ndimage import _ni_support
-from scipy.ndimage.morphology import distance_transform_edt, binary_erosion,\
-    generate_binary_structure
-from scipy.ndimage.measurements import label, find_objects
+from scipy.ndimage import (
+    _ni_support,
+    binary_erosion,
+    distance_transform_edt,
+    find_objects,
+    generate_binary_structure,
+    label,
+)
 from scipy.stats import pearsonr
 
 # own modules
 
+
 # code
 def dc(result, reference):
     r"""
     Dice coefficient
-    
+
     Computes the Dice coefficient (also known as Sorensen index) between the binary
     objects in two images.
-    
+
     The metric is defined as
-    
+
     .. math::
-        
+
         DC=\frac{2|A\cap B|}{|A|+|B|}
-        
+
     , where :math:`A` is the first and :math:`B` the second set of samples (here: binary objects).
-    
+
     Parameters
     ----------
     result : array_like
         Input data containing objects. Can be any type but will be converted
         into binary: background where 0, object everywhere else.
     reference : array_like
         Input data containing objects. Can be any type but will be converted
         into binary: background where 0, object everywhere else.
-    
+
     Returns
     -------
     dc : float
         The Dice coefficient between the object(s) in ```result``` and the
         object(s) in ```reference```. It ranges from 0 (no overlap) to 1 (perfect overlap).
-        
+
     Notes
     -----
     This is a real metric. The binary images can therefore be supplied in any order.
     """
-    result = numpy.atleast_1d(result.astype(numpy.bool))
-    reference = numpy.atleast_1d(reference.astype(numpy.bool))
-    
+    result = numpy.atleast_1d(result.astype(numpy.bool_))
+    reference = numpy.atleast_1d(reference.astype(numpy.bool_))
+
     intersection = numpy.count_nonzero(result & reference)
-    
+
     size_i1 = numpy.count_nonzero(result)
     size_i2 = numpy.count_nonzero(reference)
-    
+
     try:
-        dc = 2. * intersection / float(size_i1 + size_i2)
+        dc = 2.0 * intersection / float(size_i1 + size_i2)
     except ZeroDivisionError:
-        dc = 0.0
-    
+        dc = 1.0
+
     return dc
 
+
 def jc(result, reference):
     """
     Jaccard coefficient
-    
+
     Computes the Jaccard coefficient between the binary objects in two images.
-    
+
     Parameters
     ----------
     result: array_like
             Input data containing objects. Can be any type but will be converted
             into binary: background where 0, object everywhere else.
     reference: array_like
             Input data containing objects. Can be any type but will be converted
             into binary: background where 0, object everywhere else.
 
     Returns
     -------
     jc: float
         The Jaccard coefficient between the object(s) in `result` and the
         object(s) in `reference`. It ranges from 0 (no overlap) to 1 (perfect overlap).
-    
+
     Notes
     -----
     This is a real metric. The binary images can therefore be supplied in any order.
     """
-    result = numpy.atleast_1d(result.astype(numpy.bool))
-    reference = numpy.atleast_1d(reference.astype(numpy.bool))
-    
+    result = numpy.atleast_1d(result.astype(numpy.bool_))
+    reference = numpy.atleast_1d(reference.astype(numpy.bool_))
+
     intersection = numpy.count_nonzero(result & reference)
     union = numpy.count_nonzero(result | reference)
-    
-    jc = float(intersection) / float(union)
-    
+
+    try:
+        jc = float(intersection) / float(union)
+    except ZeroDivisionError:
+        jc = 1.0
+
     return jc
 
+
 def precision(result, reference):
     """
     Precison.
-    
+
     Parameters
     ----------
     result : array_like
         Input data containing objects. Can be any type but will be converted
         into binary: background where 0, object everywhere else.
     reference : array_like
         Input data containing objects. Can be any type but will be converted
         into binary: background where 0, object everywhere else.
-    
+
     Returns
     -------
     precision : float
         The precision between two binary datasets, here mostly binary objects in images,
         which is defined as the fraction of retrieved instances that are relevant. The
         precision is not symmetric.
-    
+
     See also
     --------
     :func:`recall`
-    
+
     Notes
     -----
     Not symmetric. The inverse of the precision is :func:`recall`.
     High precision means that an algorithm returned substantially more relevant results than irrelevant.
-    
+
     References
     ----------
     .. [1] http://en.wikipedia.org/wiki/Precision_and_recall
     .. [2] http://en.wikipedia.org/wiki/Confusion_matrix#Table_of_confusion
     """
-    result = numpy.atleast_1d(result.astype(numpy.bool))
-    reference = numpy.atleast_1d(reference.astype(numpy.bool))
-        
+    result = numpy.atleast_1d(result.astype(numpy.bool_))
+    reference = numpy.atleast_1d(reference.astype(numpy.bool_))
+
     tp = numpy.count_nonzero(result & reference)
     fp = numpy.count_nonzero(result & ~reference)
-    
+
     try:
         precision = tp / float(tp + fp)
     except ZeroDivisionError:
         precision = 0.0
-    
+
     return precision
 
+
 def recall(result, reference):
     """
     Recall.
-    
+
     Parameters
     ----------
     result : array_like
         Input data containing objects. Can be any type but will be converted
         into binary: background where 0, object everywhere else.
     reference : array_like
         Input data containing objects. Can be any type but will be converted
         into binary: background where 0, object everywhere else.
-    
+
     Returns
     -------
     recall : float
         The recall between two binary datasets, here mostly binary objects in images,
         which is defined as the fraction of relevant instances that are retrieved. The
         recall is not symmetric.
-    
+
     See also
     --------
     :func:`precision`
-    
+
     Notes
     -----
     Not symmetric. The inverse of the recall is :func:`precision`.
     High recall means that an algorithm returned most of the relevant results.
-    
+
     References
     ----------
     .. [1] http://en.wikipedia.org/wiki/Precision_and_recall
     .. [2] http://en.wikipedia.org/wiki/Confusion_matrix#Table_of_confusion
     """
-    result = numpy.atleast_1d(result.astype(numpy.bool))
-    reference = numpy.atleast_1d(reference.astype(numpy.bool))
-        
+    result = numpy.atleast_1d(result.astype(numpy.bool_))
+    reference = numpy.atleast_1d(reference.astype(numpy.bool_))
+
     tp = numpy.count_nonzero(result & reference)
     fn = numpy.count_nonzero(~result & reference)
 
     try:
         recall = tp / float(tp + fn)
     except ZeroDivisionError:
         recall = 0.0
-    
+
     return recall
 
+
 def sensitivity(result, reference):
     """
     Sensitivity.
     Same as :func:`recall`, see there for a detailed description.
-    
+
     See also
     --------
-    :func:`specificity` 
+    :func:`specificity`
     """
     return recall(result, reference)
 
+
 def specificity(result, reference):
     """
     Specificity.
-    
+
     Parameters
     ----------
     result : array_like
         Input data containing objects. Can be any type but will be converted
         into binary: background where 0, object everywhere else.
     reference : array_like
         Input data containing objects. Can be any type but will be converted
         into binary: background where 0, object everywhere else.
-    
+
     Returns
     -------
     specificity : float
         The specificity between two binary datasets, here mostly binary objects in images,
         which denotes the fraction of correctly returned negatives. The
         specificity is not symmetric.
-    
+
     See also
     --------
     :func:`sensitivity`
-    
+
     Notes
     -----
     Not symmetric. The completment of the specificity is :func:`sensitivity`.
     High recall means that an algorithm returned most of the irrelevant results.
-    
+
     References
     ----------
     .. [1] https://en.wikipedia.org/wiki/Sensitivity_and_specificity
     .. [2] http://en.wikipedia.org/wiki/Confusion_matrix#Table_of_confusion
     """
-    result = numpy.atleast_1d(result.astype(numpy.bool))
-    reference = numpy.atleast_1d(reference.astype(numpy.bool))
-       
+    result = numpy.atleast_1d(result.astype(numpy.bool_))
+    reference = numpy.atleast_1d(reference.astype(numpy.bool_))
+
     tn = numpy.count_nonzero(~result & ~reference)
     fp = numpy.count_nonzero(result & ~reference)
 
     try:
         specificity = tn / float(tn + fp)
     except ZeroDivisionError:
         specificity = 0.0
-    
+
     return specificity
 
+
 def true_negative_rate(result, reference):
     """
     True negative rate.
     Same as :func:`specificity`, see there for a detailed description.
-    
+
     See also
     --------
-    :func:`true_positive_rate` 
+    :func:`true_positive_rate`
     :func:`positive_predictive_value`
     """
     return specificity(result, reference)
 
+
 def true_positive_rate(result, reference):
     """
     True positive rate.
     Same as :func:`recall` and :func:`sensitivity`, see there for a detailed description.
-    
+
     See also
     --------
-    :func:`positive_predictive_value` 
+    :func:`positive_predictive_value`
     :func:`true_negative_rate`
     """
     return recall(result, reference)
 
+
 def positive_predictive_value(result, reference):
     """
     Positive predictive value.
     Same as :func:`precision`, see there for a detailed description.
-    
+
     See also
     --------
     :func:`true_positive_rate`
     :func:`true_negative_rate`
     """
     return precision(result, reference)
 
+
 def hd(result, reference, voxelspacing=None, connectivity=1):
     """
     Hausdorff Distance.
-    
+
     Computes the (symmetric) Hausdorff Distance (HD) between the binary objects in two
     images. It is defined as the maximum surface distance between the objects.
-    
+
     Parameters
     ----------
     result : array_like
         Input data containing objects. Can be any type but will be converted
         into binary: background where 0, object everywhere else.
     reference : array_like
         Input data containing objects. Can be any type but will be converted
@@ -322,29 +339,29 @@
         The voxelspacing in a distance unit i.e. spacing of elements
         along each dimension. If a sequence, must be of length equal to
         the input rank; if a single number, this is used for all axes. If
         not specified, a grid spacing of unity is implied.
     connectivity : int
         The neighbourhood/connectivity considered when determining the surface
         of the binary objects. This value is passed to
-        `scipy.ndimage.morphology.generate_binary_structure` and should usually be :math:`> 1`.
+        `scipy.ndimage.generate_binary_structure` and should usually be :math:`> 1`.
         Note that the connectivity influences the result in the case of the Hausdorff distance.
-        
+
     Returns
     -------
     hd : float
         The symmetric Hausdorff Distance between the object(s) in ```result``` and the
-        object(s) in ```reference```. The distance unit is the same as for the spacing of 
+        object(s) in ```reference```. The distance unit is the same as for the spacing of
         elements along each dimension, which is usually given in mm.
-        
+
     See also
     --------
     :func:`assd`
     :func:`asd`
-    
+
     Notes
     -----
     This is a real metric. The binary images can therefore be supplied in any order.
     """
     hd1 = __surface_distances(result, reference, voxelspacing, connectivity).max()
     hd2 = __surface_distances(reference, result, voxelspacing, connectivity).max()
     hd = max(hd1, hd2)
@@ -371,22 +388,22 @@
         The voxelspacing in a distance unit i.e. spacing of elements
         along each dimension. If a sequence, must be of length equal to
         the input rank; if a single number, this is used for all axes. If
         not specified, a grid spacing of unity is implied.
     connectivity : int
         The neighbourhood/connectivity considered when determining the surface
         of the binary objects. This value is passed to
-        `scipy.ndimage.morphology.generate_binary_structure` and should usually be :math:`> 1`.
+        `scipy.ndimage.generate_binary_structure` and should usually be :math:`> 1`.
         Note that the connectivity influences the result in the case of the Hausdorff distance.
 
     Returns
     -------
     hd : float
         The symmetric Hausdorff Distance between the object(s) in ```result``` and the
-        object(s) in ```reference```. The distance unit is the same as for the spacing of 
+        object(s) in ```reference```. The distance unit is the same as for the spacing of
         elements along each dimension, which is usually given in mm.
 
     See also
     --------
     :func:`hd`
 
     Notes
@@ -398,18 +415,18 @@
     hd95 = numpy.percentile(numpy.hstack((hd1, hd2)), 95)
     return hd95
 
 
 def assd(result, reference, voxelspacing=None, connectivity=1):
     """
     Average symmetric surface distance.
-    
+
     Computes the average symmetric surface distance (ASD) between the binary objects in
     two images.
-    
+
     Parameters
     ----------
     result : array_like
         Input data containing objects. Can be any type but will be converted
         into binary: background where 0, object everywhere else.
     reference : array_like
         Input data containing objects. Can be any type but will be converted
@@ -418,51 +435,57 @@
         The voxelspacing in a distance unit i.e. spacing of elements
         along each dimension. If a sequence, must be of length equal to
         the input rank; if a single number, this is used for all axes. If
         not specified, a grid spacing of unity is implied.
     connectivity : int
         The neighbourhood/connectivity considered when determining the surface
         of the binary objects. This value is passed to
-        `scipy.ndimage.morphology.generate_binary_structure` and should usually be :math:`> 1`.
+        `scipy.ndimage.generate_binary_structure` and should usually be :math:`> 1`.
         The decision on the connectivity is important, as it can influence the results
-        strongly. If in doubt, leave it as it is.         
-        
+        strongly. If in doubt, leave it as it is.
+
     Returns
     -------
     assd : float
         The average symmetric surface distance between the object(s) in ``result`` and the
-        object(s) in ``reference``. The distance unit is the same as for the spacing of 
+        object(s) in ``reference``. The distance unit is the same as for the spacing of
         elements along each dimension, which is usually given in mm.
-        
+
     See also
     --------
     :func:`asd`
     :func:`hd`
-    
+
     Notes
     -----
-    This is a real metric, obtained by calling and averaging
-    
-    >>> asd(result, reference)
-    
+    This is a real metric, obtained by calling
+
+    >>> __surface_distances(result, reference)
+
     and
-    
-    >>> asd(reference, result)
-    
-    The binary images can therefore be supplied in any order.
+
+    >>> __surface_distances(reference, result)
+
+    and then averaging the two lists. The binary images can therefore be supplied in any order.
     """
-    assd = numpy.mean( (asd(result, reference, voxelspacing, connectivity), asd(reference, result, voxelspacing, connectivity)) )
+    assd = numpy.mean(
+        (
+            __surface_distances(result, reference, voxelspacing, connectivity),
+            __surface_distances(reference, result, voxelspacing, connectivity),
+        )
+    )
     return assd
 
+
 def asd(result, reference, voxelspacing=None, connectivity=1):
     """
     Average surface distance metric.
-    
+
     Computes the average surface distance (ASD) between the binary objects in two images.
-    
+
     Parameters
     ----------
     result : array_like
         Input data containing objects. Can be any type but will be converted
         into binary: background where 0, object everywhere else.
     reference : array_like
         Input data containing objects. Can be any type but will be converted
@@ -471,266 +494,274 @@
         The voxelspacing in a distance unit i.e. spacing of elements
         along each dimension. If a sequence, must be of length equal to
         the input rank; if a single number, this is used for all axes. If
         not specified, a grid spacing of unity is implied.
     connectivity : int
         The neighbourhood/connectivity considered when determining the surface
         of the binary objects. This value is passed to
-        `scipy.ndimage.morphology.generate_binary_structure` and should usually be :math:`> 1`.
+        `scipy.ndimage.generate_binary_structure` and should usually be :math:`> 1`.
         The decision on the connectivity is important, as it can influence the results
         strongly. If in doubt, leave it as it is.
-    
+
     Returns
     -------
     asd : float
         The average surface distance between the object(s) in ``result`` and the
         object(s) in ``reference``. The distance unit is the same as for the spacing
         of elements along each dimension, which is usually given in mm.
-        
+
     See also
     --------
     :func:`assd`
     :func:`hd`
-    
-    
+
+
     Notes
     -----
     This is not a real metric, as it is directed. See `assd` for a real metric of this.
-    
+
     The method is implemented making use of distance images and simple binary morphology
     to achieve high computational speed.
-    
+
     Examples
     --------
     The `connectivity` determines what pixels/voxels are considered the surface of a
     binary object. Take the following binary image showing a cross
-    
-    >>> from scipy.ndimage.morphology import generate_binary_structure
+
+    >>> from scipy.ndimage import generate_binary_structure
     >>> cross = generate_binary_structure(2, 1)
     array([[0, 1, 0],
            [1, 1, 1],
            [0, 1, 0]])
-           
+
     With `connectivity` set to `1` a 4-neighbourhood is considered when determining the
     object surface, resulting in the surface
-    
+
     .. code-block:: python
-    
+
         array([[0, 1, 0],
                [1, 0, 1],
                [0, 1, 0]])
-           
+
     Changing `connectivity` to `2`, a 8-neighbourhood is considered and we get:
-    
+
     .. code-block:: python
-    
+
         array([[0, 1, 0],
                [1, 1, 1],
                [0, 1, 0]])
-           
+
     , as a diagonal connection does no longer qualifies as valid object surface.
-    
+
     This influences the  results `asd` returns. Imagine we want to compute the surface
     distance of our cross to a cube-like object:
-    
+
     >>> cube = generate_binary_structure(2, 1)
     array([[1, 1, 1],
            [1, 1, 1],
            [1, 1, 1]])
-           
+
     , which surface is, independent of the `connectivity` value set, always
-    
+
     .. code-block:: python
-    
+
         array([[1, 1, 1],
                [1, 0, 1],
                [1, 1, 1]])
-           
+
     Using a `connectivity` of `1` we get
-    
+
     >>> asd(cross, cube, connectivity=1)
     0.0
-    
+
     while a value of `2` returns us
-    
+
     >>> asd(cross, cube, connectivity=2)
     0.20000000000000001
-    
+
     due to the center of the cross being considered surface as well.
-    
+
     """
     sds = __surface_distances(result, reference, voxelspacing, connectivity)
     asd = sds.mean()
     return asd
 
+
 def ravd(result, reference):
     """
     Relative absolute volume difference.
-    
+
     Compute the relative absolute volume difference between the (joined) binary objects
     in the two images.
-    
+
     Parameters
     ----------
     result : array_like
         Input data containing objects. Can be any type but will be converted
         into binary: background where 0, object everywhere else.
     reference : array_like
         Input data containing objects. Can be any type but will be converted
         into binary: background where 0, object everywhere else.
-        
+
     Returns
     -------
     ravd : float
         The relative absolute volume difference between the object(s) in ``result``
         and the object(s) in ``reference``. This is a percentage value in the range
         :math:`[-1.0, +inf]` for which a :math:`0` denotes an ideal score.
-        
+
     Raises
     ------
     RuntimeError
         If the reference object is empty.
-        
+
     See also
     --------
     :func:`dc`
     :func:`precision`
     :func:`recall`
-    
+
     Notes
     -----
     This is not a real metric, as it is directed. Negative values denote a smaller
     and positive values a larger volume than the reference.
     This implementation does not check, whether the two supplied arrays are of the same
     size.
-    
+
     Examples
     --------
     Considering the following inputs
-    
+
     >>> import numpy
     >>> arr1 = numpy.asarray([[0,1,0],[1,1,1],[0,1,0]])
     >>> arr1
     array([[0, 1, 0],
            [1, 1, 1],
            [0, 1, 0]])
     >>> arr2 = numpy.asarray([[0,1,0],[1,0,1],[0,1,0]])
     >>> arr2
     array([[0, 1, 0],
            [1, 0, 1],
            [0, 1, 0]])
-           
+
     comparing `arr1` to `arr2` we get
-    
+
     >>> ravd(arr1, arr2)
     -0.2
-    
+
     and reversing the inputs the directivness of the metric becomes evident
-    
+
     >>> ravd(arr2, arr1)
     0.25
-    
+
     It is important to keep in mind that a perfect score of `0` does not mean that the
     binary objects fit exactely, as only the volumes are compared:
-    
+
     >>> arr1 = numpy.asarray([1,0,0])
     >>> arr2 = numpy.asarray([0,0,1])
     >>> ravd(arr1, arr2)
     0.0
-    
+
     """
-    result = numpy.atleast_1d(result.astype(numpy.bool))
-    reference = numpy.atleast_1d(reference.astype(numpy.bool))
-        
+    result = numpy.atleast_1d(result.astype(numpy.bool_))
+    reference = numpy.atleast_1d(reference.astype(numpy.bool_))
+
     vol1 = numpy.count_nonzero(result)
     vol2 = numpy.count_nonzero(reference)
-    
+
     if 0 == vol2:
-        raise RuntimeError('The second supplied array does not contain any binary object.')
-    
+        raise RuntimeError(
+            "The second supplied array does not contain any binary object."
+        )
+
     return (vol1 - vol2) / float(vol2)
 
+
 def volume_correlation(results, references):
     r"""
     Volume correlation.
-    
+
     Computes the linear correlation in binary object volume between the
     contents of the successive binary images supplied. Measured through
-    the Pearson product-moment correlation coefficient. 
-    
+    the Pearson product-moment correlation coefficient.
+
     Parameters
     ----------
     results : sequence of array_like
         Ordered list of input data containing objects. Each array_like will be
         converted into binary: background where 0, object everywhere else.
     references : sequence of array_like
         Ordered list of input data containing objects. Each array_like will be
         converted into binary: background where 0, object everywhere else.
         The order must be the same as for ``results``.
-    
+
     Returns
     -------
     r : float
         The correlation coefficient between -1 and 1.
     p : float
         The two-side p value.
-        
+
     """
-    results = numpy.atleast_2d(numpy.array(results).astype(numpy.bool))
-    references = numpy.atleast_2d(numpy.array(references).astype(numpy.bool))
-    
+    results = numpy.atleast_2d(numpy.array(results).astype(numpy.bool_))
+    references = numpy.atleast_2d(numpy.array(references).astype(numpy.bool_))
+
     results_volumes = [numpy.count_nonzero(r) for r in results]
     references_volumes = [numpy.count_nonzero(r) for r in references]
-    
-    return pearsonr(results_volumes, references_volumes) # returns (Pearson'
+
+    return pearsonr(results_volumes, references_volumes)  # returns (Pearson'
+
 
 def volume_change_correlation(results, references):
     r"""
     Volume change correlation.
-    
+
     Computes the linear correlation of change in binary object volume between
     the contents of the successive binary images supplied. Measured through
-    the Pearson product-moment correlation coefficient. 
-    
+    the Pearson product-moment correlation coefficient.
+
     Parameters
     ----------
     results : sequence of array_like
         Ordered list of input data containing objects. Each array_like will be
         converted into binary: background where 0, object everywhere else.
     references : sequence of array_like
         Ordered list of input data containing objects. Each array_like will be
         converted into binary: background where 0, object everywhere else.
         The order must be the same as for ``results``.
-    
+
     Returns
     -------
     r : float
         The correlation coefficient between -1 and 1.
     p : float
         The two-side p value.
-        
+
     """
-    results = numpy.atleast_2d(numpy.array(results).astype(numpy.bool))
-    references = numpy.atleast_2d(numpy.array(references).astype(numpy.bool))
-    
+    results = numpy.atleast_2d(numpy.array(results).astype(numpy.bool_))
+    references = numpy.atleast_2d(numpy.array(references).astype(numpy.bool_))
+
     results_volumes = numpy.asarray([numpy.count_nonzero(r) for r in results])
     references_volumes = numpy.asarray([numpy.count_nonzero(r) for r in references])
-    
+
     results_volumes_changes = results_volumes[1:] - results_volumes[:-1]
-    references_volumes_changes = references_volumes[1:] - references_volumes[:-1] 
-    
-    return pearsonr(results_volumes_changes, references_volumes_changes) # returns (Pearson's correlation coefficient, 2-tailed p-value)
-    
+    references_volumes_changes = references_volumes[1:] - references_volumes[:-1]
+
+    return pearsonr(
+        results_volumes_changes, references_volumes_changes
+    )  # returns (Pearson's correlation coefficient, 2-tailed p-value)
+
+
 def obj_assd(result, reference, voxelspacing=None, connectivity=1):
     """
     Average symmetric surface distance.
-    
+
     Computes the average symmetric surface distance (ASSD) between the binary objects in
     two images.
-    
+
     Parameters
     ----------
     result : array_like
         Input data containing objects. Can be any type but will be converted
         into binary: background where 0, object everywhere else.
     reference : array_like
         Input data containing objects. Can be any type but will be converted
@@ -740,53 +771,58 @@
         along each dimension. If a sequence, must be of length equal to
         the input rank; if a single number, this is used for all axes. If
         not specified, a grid spacing of unity is implied.
     connectivity : int
         The neighbourhood/connectivity considered when determining what accounts
         for a distinct binary object as well as when determining the surface
         of the binary objects. This value is passed to
-        `scipy.ndimage.morphology.generate_binary_structure` and should usually be :math:`> 1`.
+        `scipy.ndimage.generate_binary_structure` and should usually be :math:`> 1`.
         The decision on the connectivity is important, as it can influence the results
         strongly. If in doubt, leave it as it is.
-        
+
     Returns
     -------
     assd : float
         The average symmetric surface distance between all mutually existing distinct
         binary object(s) in ``result`` and ``reference``. The distance unit is the same as for
         the spacing of elements along each dimension, which is usually given in mm.
-        
+
     See also
     --------
     :func:`obj_asd`
-    
+
     Notes
     -----
-    This is a real metric, obtained by calling and averaging
-    
-    >>> obj_asd(result, reference)
-    
+    This is a real metric, obtained by calling
+
+    >>> __obj_surface_distances(result, reference)
+
     and
-    
-    >>> obj_asd(reference, result)
-    
-    The binary images can therefore be supplied in any order.
+
+    >>> __obj_surface_distances(reference, result)
+
+    and then averaging the two lists. The binary images can therefore be supplied in any order.
     """
-    assd = numpy.mean( (obj_asd(result, reference, voxelspacing, connectivity), obj_asd(reference, result, voxelspacing, connectivity)) )
+    assd = numpy.mean(
+        (
+            __obj_surface_distances(result, reference, voxelspacing, connectivity),
+            __obj_surface_distances(reference, result, voxelspacing, connectivity),
+        )
+    )
     return assd
-    
-    
+
+
 def obj_asd(result, reference, voxelspacing=None, connectivity=1):
     """
     Average surface distance between objects.
-    
+
     First correspondences between distinct binary objects in reference and result are
     established. Then the average surface distance is only computed between corresponding
     objects. Correspondence is defined as unique and at least one voxel overlap.
-    
+
     Parameters
     ----------
     result : array_like
         Input data containing objects. Can be any type but will be converted
         into binary: background where 0, object everywhere else.
     reference : array_like
         Input data containing objects. Can be any type but will be converted
@@ -796,39 +832,39 @@
         along each dimension. If a sequence, must be of length equal to
         the input rank; if a single number, this is used for all axes. If
         not specified, a grid spacing of unity is implied.
     connectivity : int
         The neighbourhood/connectivity considered when determining what accounts
         for a distinct binary object as well as when determining the surface
         of the binary objects. This value is passed to
-        `scipy.ndimage.morphology.generate_binary_structure` and should usually be :math:`> 1`.
+        `scipy.ndimage.generate_binary_structure` and should usually be :math:`> 1`.
         The decision on the connectivity is important, as it can influence the results
         strongly. If in doubt, leave it as it is.
-        
+
     Returns
     -------
     asd : float
         The average surface distance between all mutually existing distinct binary
         object(s) in ``result`` and ``reference``. The distance unit is the same as for the
         spacing of elements along each dimension, which is usually given in mm.
-        
+
     See also
     --------
     :func:`obj_assd`
     :func:`obj_tpr`
     :func:`obj_fpr`
-        
+
     Notes
     -----
     This is not a real metric, as it is directed. See `obj_assd` for a real metric of this.
-    
+
     For the understanding of this metric, both the notions of connectedness and surface
     distance are essential. Please see :func:`obj_tpr` and :func:`obj_fpr` for more
     information on the first and :func:`asd` on the second.
-        
+
     Examples
     --------
     >>> arr1 = numpy.asarray([[1,1,1],[1,1,1],[1,1,1]])
     >>> arr2 = numpy.asarray([[0,1,0],[0,1,0],[0,1,0]])
     >>> arr1
     array([[1, 1, 1],
            [1, 1, 1],
@@ -837,141 +873,134 @@
     array([[0, 1, 0],
            [0, 1, 0],
            [0, 1, 0]])
     >>> obj_asd(arr1, arr2)
     1.5
     >>> obj_asd(arr2, arr1)
     0.333333333333
-    
+
     With the `voxelspacing` parameter, the distances between the voxels can be set for
     each dimension separately:
-    
+
     >>> obj_asd(arr1, arr2, voxelspacing=(1,2))
     1.5
     >>> obj_asd(arr2, arr1, voxelspacing=(1,2))
-    0.333333333333    
-    
+    0.333333333333
+
     More examples depicting the notion of object connectedness:
-    
+
     >>> arr1 = numpy.asarray([[1,0,1],[1,0,0],[0,0,0]])
     >>> arr2 = numpy.asarray([[1,0,1],[1,0,0],[0,0,1]])
     >>> arr1
     array([[1, 0, 1],
            [1, 0, 0],
            [0, 0, 0]])
     >>> arr2
     array([[1, 0, 1],
            [1, 0, 0],
            [0, 0, 1]])
     >>> obj_asd(arr1, arr2)
     0.0
     >>> obj_asd(arr2, arr1)
     0.0
-    
+
     >>> arr1 = numpy.asarray([[1,0,1],[1,0,1],[0,0,1]])
     >>> arr2 = numpy.asarray([[1,0,1],[1,0,0],[0,0,1]])
     >>> arr1
     array([[1, 0, 1],
            [1, 0, 1],
            [0, 0, 1]])
     >>> arr2
     array([[1, 0, 1],
            [1, 0, 0],
            [0, 0, 1]])
     >>> obj_asd(arr1, arr2)
     0.6
     >>> obj_asd(arr2, arr1)
     0.0
-    
+
     Influence of `connectivity` parameter can be seen in the following example, where
     with the (default) connectivity of `1` the first array is considered to contain two
     objects, while with an increase connectivity of `2`, just one large object is
-    detected.  
-    
+    detected.
+
     >>> arr1 = numpy.asarray([[1,0,0],[0,1,1],[0,1,1]])
     >>> arr2 = numpy.asarray([[1,0,0],[0,0,0],[0,0,0]])
     >>> arr1
     array([[1, 0, 0],
            [0, 1, 1],
            [0, 1, 1]])
     >>> arr2
     array([[1, 0, 0],
            [0, 0, 0],
            [0, 0, 0]])
     >>> obj_asd(arr1, arr2)
     0.0
     >>> obj_asd(arr1, arr2, connectivity=2)
     1.742955328
-    
+
     Note that the connectivity also influence the notion of what is considered an object
     surface voxels.
     """
-    sds = list()
-    labelmap1, labelmap2, _a, _b, mapping = __distinct_binary_object_correspondences(result, reference, connectivity)
-    slicers1 = find_objects(labelmap1)
-    slicers2 = find_objects(labelmap2)
-    for lid2, lid1 in list(mapping.items()):
-        window = __combine_windows(slicers1[lid1 - 1], slicers2[lid2 - 1])
-        object1 = labelmap1[window] == lid1
-        object2 = labelmap2[window] == lid2
-        sds.extend(__surface_distances(object1, object2, voxelspacing, connectivity))
+    sds = __obj_surface_distances(result, reference, voxelspacing, connectivity)
     asd = numpy.mean(sds)
     return asd
-    
+
+
 def obj_fpr(result, reference, connectivity=1):
     """
     The false positive rate of distinct binary object detection.
-    
+
     The false positive rates gives a percentage measure of how many distinct binary
     objects in the second array do not exists in the first array. A partial overlap
     (of minimum one voxel) is here considered sufficient.
-    
+
     In cases where two distinct binary object in the second array overlap with a single
     distinct object in the first array, only one is considered to have been detected
     successfully and the other is added to the count of false positives.
-    
+
     Parameters
     ----------
     result : array_like
         Input data containing objects. Can be any type but will be converted
         into binary: background where 0, object everywhere else.
     reference : array_like
         Input data containing objects. Can be any type but will be converted
         into binary: background where 0, object everywhere else.
     connectivity : int
         The neighbourhood/connectivity considered when determining what accounts
         for a distinct binary object. This value is passed to
-        `scipy.ndimage.morphology.generate_binary_structure` and should usually be :math:`> 1`.
+        `scipy.ndimage.generate_binary_structure` and should usually be :math:`> 1`.
         The decision on the connectivity is important, as it can influence the results
         strongly. If in doubt, leave it as it is.
-        
+
     Returns
     -------
     tpr : float
         A percentage measure of how many distinct binary objects in ``results`` have no
         corresponding binary object in ``reference``. It has the range :math:`[0, 1]`, where a :math:`0`
         denotes an ideal score.
-        
+
     Raises
     ------
     RuntimeError
         If the second array is empty.
-    
+
     See also
     --------
     :func:`obj_tpr`
-    
+
     Notes
     -----
     This is not a real metric, as it is directed. Whatever array is considered as
     reference should be passed second. A perfect score of :math:`0` tells that there are no
     distinct binary objects in the second array that do not exists also in the reference
     array, but does not reveal anything about objects in the reference array also
     existing in the second array (use :func:`obj_tpr` for this).
-    
+
     Examples
     --------
     >>> arr2 = numpy.asarray([[1,0,0],[1,0,1],[0,0,1]])
     >>> arr1 = numpy.asarray([[0,0,1],[1,0,1],[0,0,1]])
     >>> arr2
     array([[1, 0, 0],
            [1, 0, 1],
@@ -980,108 +1009,111 @@
     array([[0, 0, 1],
            [1, 0, 1],
            [0, 0, 1]])
     >>> obj_fpr(arr1, arr2)
     0.0
     >>> obj_fpr(arr2, arr1)
     0.0
-    
+
     Example of directedness:
-    
+
     >>> arr2 = numpy.asarray([1,0,1,0,1])
     >>> arr1 = numpy.asarray([1,0,1,0,0])
     >>> obj_fpr(arr1, arr2)
     0.0
     >>> obj_fpr(arr2, arr1)
     0.3333333333333333
-    
+
     Examples of multiple overlap treatment:
-    
+
     >>> arr2 = numpy.asarray([1,0,1,0,1,1,1])
     >>> arr1 = numpy.asarray([1,1,1,0,1,0,1])
     >>> obj_fpr(arr1, arr2)
     0.3333333333333333
     >>> obj_fpr(arr2, arr1)
     0.3333333333333333
-    
+
     >>> arr2 = numpy.asarray([1,0,1,1,1,0,1])
     >>> arr1 = numpy.asarray([1,1,1,0,1,1,1])
     >>> obj_fpr(arr1, arr2)
     0.0
     >>> obj_fpr(arr2, arr1)
     0.3333333333333333
-    
+
     >>> arr2 = numpy.asarray([[1,0,1,0,0],
                               [1,0,0,0,0],
                               [1,0,1,1,1],
                               [0,0,0,0,0],
                               [1,0,1,0,0]])
     >>> arr1 = numpy.asarray([[1,1,1,0,0],
                               [0,0,0,0,0],
                               [1,1,1,0,1],
                               [0,0,0,0,0],
                               [1,1,1,0,0]])
     >>> obj_fpr(arr1, arr2)
     0.0
     >>> obj_fpr(arr2, arr1)
-    0.2    
+    0.2
     """
-    _, _, _, n_obj_reference, mapping = __distinct_binary_object_correspondences(reference, result, connectivity)
+    _, _, _, n_obj_reference, mapping = __distinct_binary_object_correspondences(
+        reference, result, connectivity
+    )
     return (n_obj_reference - len(mapping)) / float(n_obj_reference)
-    
+
+
 def obj_tpr(result, reference, connectivity=1):
     """
     The true positive rate of distinct binary object detection.
-    
+
     The true positive rates gives a percentage measure of how many distinct binary
     objects in the first array also exists in the second array. A partial overlap
     (of minimum one voxel) is here considered sufficient.
-    
+
     In cases where two distinct binary object in the first array overlaps with a single
     distinct object in the second array, only one is considered to have been detected
-    successfully.  
-    
+    successfully.
+
     Parameters
     ----------
     result : array_like
         Input data containing objects. Can be any type but will be converted
         into binary: background where 0, object everywhere else.
     reference : array_like
         Input data containing objects. Can be any type but will be converted
         into binary: background where 0, object everywhere else.
     connectivity : int
         The neighbourhood/connectivity considered when determining what accounts
         for a distinct binary object. This value is passed to
-        `scipy.ndimage.morphology.generate_binary_structure` and should usually be :math:`> 1`.
+        `scipy.ndimage.generate_binary_structure` and should usually be :math:`> 1`.
         The decision on the connectivity is important, as it can influence the results
         strongly. If in doubt, leave it as it is.
-        
+
     Returns
     -------
     tpr : float
         A percentage measure of how many distinct binary objects in ``result`` also exists
         in ``reference``. It has the range :math:`[0, 1]`, where a :math:`1` denotes an ideal score.
-        
+
     Raises
     ------
     RuntimeError
         If the reference object is empty.
-    
+
     See also
     --------
     :func:`obj_fpr`
-    
+
     Notes
     -----
     This is not a real metric, as it is directed. Whatever array is considered as
     reference should be passed second. A perfect score of :math:`1` tells that all distinct
     binary objects in the reference array also exist in the result array, but does not
     reveal anything about additional binary objects in the result array
     (use :func:`obj_fpr` for this).
-    
+
     Examples
     --------
     >>> arr2 = numpy.asarray([[1,0,0],[1,0,1],[0,0,1]])
     >>> arr1 = numpy.asarray([[0,0,1],[1,0,1],[0,0,1]])
     >>> arr2
     array([[1, 0, 0],
            [1, 0, 1],
@@ -1090,146 +1122,192 @@
     array([[0, 0, 1],
            [1, 0, 1],
            [0, 0, 1]])
     >>> obj_tpr(arr1, arr2)
     1.0
     >>> obj_tpr(arr2, arr1)
     1.0
-    
+
     Example of directedness:
-    
+
     >>> arr2 = numpy.asarray([1,0,1,0,1])
     >>> arr1 = numpy.asarray([1,0,1,0,0])
     >>> obj_tpr(arr1, arr2)
     0.6666666666666666
     >>> obj_tpr(arr2, arr1)
     1.0
-    
+
     Examples of multiple overlap treatment:
-    
+
     >>> arr2 = numpy.asarray([1,0,1,0,1,1,1])
     >>> arr1 = numpy.asarray([1,1,1,0,1,0,1])
     >>> obj_tpr(arr1, arr2)
     0.6666666666666666
     >>> obj_tpr(arr2, arr1)
     0.6666666666666666
-    
+
     >>> arr2 = numpy.asarray([1,0,1,1,1,0,1])
     >>> arr1 = numpy.asarray([1,1,1,0,1,1,1])
     >>> obj_tpr(arr1, arr2)
     0.6666666666666666
     >>> obj_tpr(arr2, arr1)
     1.0
-    
+
     >>> arr2 = numpy.asarray([[1,0,1,0,0],
                               [1,0,0,0,0],
                               [1,0,1,1,1],
                               [0,0,0,0,0],
                               [1,0,1,0,0]])
     >>> arr1 = numpy.asarray([[1,1,1,0,0],
                               [0,0,0,0,0],
                               [1,1,1,0,1],
                               [0,0,0,0,0],
                               [1,1,1,0,0]])
     >>> obj_tpr(arr1, arr2)
     0.8
     >>> obj_tpr(arr2, arr1)
-    1.0    
+    1.0
     """
-    _, _, n_obj_result, _, mapping = __distinct_binary_object_correspondences(reference, result, connectivity)
+    _, _, n_obj_result, _, mapping = __distinct_binary_object_correspondences(
+        reference, result, connectivity
+    )
     return len(mapping) / float(n_obj_result)
 
+
 def __distinct_binary_object_correspondences(reference, result, connectivity=1):
     """
     Determines all distinct (where connectivity is defined by the connectivity parameter
     passed to scipy's `generate_binary_structure`) binary objects in both of the input
     parameters and returns a 1to1 mapping from the labelled objects in reference to the
     corresponding (whereas a one-voxel overlap suffices for correspondence) objects in
     result.
-    
+
     All stems from the problem, that the relationship is non-surjective many-to-many.
-    
+
     @return (labelmap1, labelmap2, n_lables1, n_labels2, labelmapping2to1)
     """
-    result = numpy.atleast_1d(result.astype(numpy.bool))
-    reference = numpy.atleast_1d(reference.astype(numpy.bool))
-    
+    result = numpy.atleast_1d(result.astype(numpy.bool_))
+    reference = numpy.atleast_1d(reference.astype(numpy.bool_))
+
     # binary structure
     footprint = generate_binary_structure(result.ndim, connectivity)
-    
+
     # label distinct binary objects
     labelmap1, n_obj_result = label(result, footprint)
     labelmap2, n_obj_reference = label(reference, footprint)
-    
+
     # find all overlaps from labelmap2 to labelmap1; collect one-to-one relationships and store all one-two-many for later processing
-    slicers = find_objects(labelmap2) # get windows of labelled objects
-    mapping = dict() # mappings from labels in labelmap2 to corresponding object labels in labelmap1
-    used_labels = set() # set to collect all already used labels from labelmap2
-    one_to_many = list() # list to collect all one-to-many mappings
-    for l1id, slicer in enumerate(slicers): # iterate over object in labelmap2 and their windows
-        l1id += 1 # labelled objects have ids sarting from 1
-        bobj = (l1id) == labelmap2[slicer] # find binary object corresponding to the label1 id in the segmentation
-        l2ids = numpy.unique(labelmap1[slicer][bobj]) # extract all unique object identifiers at the corresponding positions in the reference (i.e. the mapping)
-        l2ids = l2ids[0 != l2ids] # remove background identifiers (=0)
-        if 1 == len(l2ids): # one-to-one mapping: if target label not already used, add to final list of object-to-object mappings and mark target label as used
+    slicers = find_objects(labelmap2)  # get windows of labelled objects
+    mapping = (
+        dict()
+    )  # mappings from labels in labelmap2 to corresponding object labels in labelmap1
+    used_labels = set()  # set to collect all already used labels from labelmap2
+    one_to_many = list()  # list to collect all one-to-many mappings
+    for l1id, slicer in enumerate(
+        slicers
+    ):  # iterate over object in labelmap2 and their windows
+        l1id += 1  # labelled objects have ids sarting from 1
+        bobj = (l1id) == labelmap2[
+            slicer
+        ]  # find binary object corresponding to the label1 id in the segmentation
+        l2ids = numpy.unique(
+            labelmap1[slicer][bobj]
+        )  # extract all unique object identifiers at the corresponding positions in the reference (i.e. the mapping)
+        l2ids = l2ids[0 != l2ids]  # remove background identifiers (=0)
+        if 1 == len(
+            l2ids
+        ):  # one-to-one mapping: if target label not already used, add to final list of object-to-object mappings and mark target label as used
             l2id = l2ids[0]
             if not l2id in used_labels:
                 mapping[l1id] = l2id
                 used_labels.add(l2id)
-        elif 1 < len(l2ids): # one-to-many mapping: store relationship for later processing
+        elif 1 < len(
+            l2ids
+        ):  # one-to-many mapping: store relationship for later processing
             one_to_many.append((l1id, set(l2ids)))
-            
+
     # process one-to-many mappings, always choosing the one with the least labelmap2 correspondences first
     while True:
-        one_to_many = [(l1id, l2ids - used_labels) for l1id, l2ids in one_to_many] # remove already used ids from all sets
-        one_to_many = [x for x in one_to_many if x[1]] # remove empty sets
-        one_to_many = sorted(one_to_many, key=lambda x: len(x[1])) # sort by set length
+        one_to_many = [
+            (l1id, l2ids - used_labels) for l1id, l2ids in one_to_many
+        ]  # remove already used ids from all sets
+        one_to_many = [x for x in one_to_many if x[1]]  # remove empty sets
+        one_to_many = sorted(one_to_many, key=lambda x: len(x[1]))  # sort by set length
         if 0 == len(one_to_many):
             break
-        l2id = one_to_many[0][1].pop() # select an arbitrary target label id from the shortest set
-        mapping[one_to_many[0][0]] = l2id # add to one-to-one mappings 
-        used_labels.add(l2id) # mark target label as used
-        one_to_many = one_to_many[1:] # delete the processed set from all sets
-    
+        l2id = one_to_many[0][
+            1
+        ].pop()  # select an arbitrary target label id from the shortest set
+        mapping[one_to_many[0][0]] = l2id  # add to one-to-one mappings
+        used_labels.add(l2id)  # mark target label as used
+        one_to_many = one_to_many[1:]  # delete the processed set from all sets
+
     return labelmap1, labelmap2, n_obj_result, n_obj_reference, mapping
-    
+
+
 def __surface_distances(result, reference, voxelspacing=None, connectivity=1):
     """
     The distances between the surface voxel of binary objects in result and their
     nearest partner surface voxel of a binary object in reference.
     """
-    result = numpy.atleast_1d(result.astype(numpy.bool))
-    reference = numpy.atleast_1d(reference.astype(numpy.bool))
+    result = numpy.atleast_1d(result.astype(numpy.bool_))
+    reference = numpy.atleast_1d(reference.astype(numpy.bool_))
     if voxelspacing is not None:
         voxelspacing = _ni_support._normalize_sequence(voxelspacing, result.ndim)
         voxelspacing = numpy.asarray(voxelspacing, dtype=numpy.float64)
         if not voxelspacing.flags.contiguous:
             voxelspacing = voxelspacing.copy()
-            
+
     # binary structure
     footprint = generate_binary_structure(result.ndim, connectivity)
-    
+
     # test for emptiness
-    if 0 == numpy.count_nonzero(result): 
-        raise RuntimeError('The first supplied array does not contain any binary object.')
-    if 0 == numpy.count_nonzero(reference): 
-        raise RuntimeError('The second supplied array does not contain any binary object.')    
-            
+    if 0 == numpy.count_nonzero(result):
+        raise RuntimeError(
+            "The first supplied array does not contain any binary object."
+        )
+    if 0 == numpy.count_nonzero(reference):
+        raise RuntimeError(
+            "The second supplied array does not contain any binary object."
+        )
+
     # extract only 1-pixel border line of objects
     result_border = result ^ binary_erosion(result, structure=footprint, iterations=1)
-    reference_border = reference ^ binary_erosion(reference, structure=footprint, iterations=1)
-    
-    # compute average surface distance        
+    reference_border = reference ^ binary_erosion(
+        reference, structure=footprint, iterations=1
+    )
+
+    # compute average surface distance
     # Note: scipys distance transform is calculated only inside the borders of the
     #       foreground objects, therefore the input has to be reversed
     dt = distance_transform_edt(~reference_border, sampling=voxelspacing)
     sds = dt[result_border]
-    
+
     return sds
 
+
+def __obj_surface_distances(result, reference, voxelspacing=None, connectivity=1):
+    """
+    The distances between the surface voxel between all corresponding binary
+    objects in result and reference. Correspondence is defined as unique and at least one voxel overlap.
+    """
+    sds = list()
+    labelmap1, labelmap2, _a, _b, mapping = __distinct_binary_object_correspondences(
+        result, reference, connectivity
+    )
+    slicers1 = find_objects(labelmap1)
+    slicers2 = find_objects(labelmap2)
+    for lid2, lid1 in list(mapping.items()):
+        window = __combine_windows(slicers1[lid1 - 1], slicers2[lid2 - 1])
+        object1 = labelmap1[window] == lid1
+        object2 = labelmap2[window] == lid2
+        sds.extend(__surface_distances(object1, object2, voxelspacing, connectivity))
+    return sds
+
+
 def __combine_windows(w1, w2):
     """
     Joins two windows (defined by tuple of slices) such that their maximum
     combined extend is covered by the new returned window.
     """
     res = []
     for s1, s2 in zip(w1, w2):
```

### Comparing `MedPy-0.4.0/medpy/graphcut/write.py` & `MedPy-0.5.0/medpy/graphcut/write.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,73 +1,76 @@
 # Copyright (C) 2013 Oskar Maier
-# 
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
-# 
+#
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
-# 
+#
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 # author Oskar Maier
 # version r0.1.0
 # since 2012-02-06
 # status Release
 
 # build-in modules
 
 # third-party modules
 
 # own modules
 
+
 # code
 def graph_to_dimacs(g, f):
     """
     Persists the supplied graph in valid dimacs format into the file.
-    
+
     Parameters
     ----------
     g : `~medpy.graphcut.graph.Graph`
         A graph object to persist.
     f : file
         A file-like object.
     """
     # write comments
-    f.write('c Created by medpy\n')
-    f.write('c Oskar Maier, oskar.maier@googlemail.com\n')
-    f.write('c\n')
-    
+    f.write("c Created by medpy\n")
+    f.write("c Oskar Maier, oskar.maier@googlemail.com\n")
+    f.write("c\n")
+
     # write problem
-    f.write('c problem line\n')
-    f.write('p max {} {}\n'.format(g.get_node_count() + 2, len(g.get_edges()))) # +2 as terminal nodes also count in dimacs format # no-nodes / no-edges
-    
+    f.write("c problem line\n")
+    f.write(
+        "p max {} {}\n".format(g.get_node_count() + 2, len(g.get_edges()))
+    )  # +2 as terminal nodes also count in dimacs format # no-nodes / no-edges
+
     # denote source and sink
-    f.write('c source descriptor\n')
-    f.write('n 1 s\n')
-    f.write('c sink descriptor\n')
-    f.write('n 2 t\n')
-    
+    f.write("c source descriptor\n")
+    f.write("n 1 s\n")
+    f.write("c sink descriptor\n")
+    f.write("n 2 t\n")
+
     # write terminal arcs (t-weights)
-    f.write('c terminal arcs (t-weights)\n')
+    f.write("c terminal arcs (t-weights)\n")
     for node, weight in list(g.get_tweights().items()):
         # Note: the nodes ids of the graph start from 1, but 1 and 2 are reserved for source and sink respectively, therefore add 2
-        if not 0 == weight[0]: # 0 weights are implicit
-            f.write('a 1 {} {}\n'.format(node + 2, weight[0]))
-        if not 0 == weight[1]: # 0 weights are implicit
-            f.write('a {} 2 {}\n'.format(node + 2, weight[1]))
-    
+        if not 0 == weight[0]:  # 0 weights are implicit
+            f.write("a 1 {} {}\n".format(node + 2, weight[0]))
+        if not 0 == weight[1]:  # 0 weights are implicit
+            f.write("a {} 2 {}\n".format(node + 2, weight[1]))
+
     # write inter-node arcs (n-weights)
-    f.write('c inter-node arcs (n-weights)\n')
+    f.write("c inter-node arcs (n-weights)\n")
     for edge, weight in list(g.get_nweights().items()):
-        if not 0 == weight[0]: # 0 weights are implicit
-            f.write('a {} {} {}\n'.format(edge[0] + 2, edge[1] + 2, weight[0]))
+        if not 0 == weight[0]:  # 0 weights are implicit
+            f.write("a {} {} {}\n".format(edge[0] + 2, edge[1] + 2, weight[0]))
         # reversed weights have to follow directly in the next line
-        if not 0 == weight[1]: # 0 weights are implicit
-            f.write('a {} {} {}\n'.format(edge[1] + 2, edge[0] + 2, weight[1]))
-            
+        if not 0 == weight[1]:  # 0 weights are implicit
+            f.write("a {} {} {}\n".format(edge[1] + 2, edge[0] + 2, weight[1]))
+
     # end comment
-    f.write('c end-of-file')
+    f.write("c end-of-file")
```

### Comparing `MedPy-0.4.0/medpy/graphcut/__init__.py` & `MedPy-0.5.0/medpy/graphcut/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,124 +6,124 @@
 
 Provides functionalities to efficiently construct nD graphs from various sources using
 arbitrary energy functions (boundary and regional terms). The graph can then be saved in
 the Dimacs graph standard [5]_ and/or processed (i.e. cut) using 3rd party graph-cut [1]_
 algorithms.
 
 This module makes use of a custom *Boost.Python* [2]_ wrapper written for a modified
-version of Boykov and Kolmogorovs max-flow/min-cut algorithm (v3.01) [4]_ that can be found at [3]_. 
+version of Boykov and Kolmogorovs max-flow/min-cut algorithm (v3.01) [4]_ that can be found at [3]_.
 
 Supports voxel- as well as label/region-based graph-cuts.
 
 See below for examples.
 
 
 Directly generate graphs from image :mod:`medpy.graphcut.generate`
 ==================================================================
 Provides functions to generate graphs efficiently from nD images.
 Use together with an energy term from :mod:`~medpy.graphcut.energy_voxel` respectively :mod:`~medpy.graphcut.energy_label`,
 
 .. module:: medpy.graphcut.generate
 .. autosummary::
     :toctree: generated/
-    
+
     graph_from_voxels
     graph_from_labels
-    
+
 Energy terms for voxel-based graph-cuts :mod:`medpy.graphcut.energy_voxel`
 ==========================================================================
 Run-time optimized energy functions for the graph generation. Voxel based [7]_.
 
 .. module:: medpy.graphcut.energy_voxel
-    
+
 Boundary energy terms
 ---------------------
 .. autosummary::
-    :toctree: generated/    
-    
+    :toctree: generated/
+
     boundary_maximum_linear
     boundary_difference_linear
     boundary_maximum_exponential
     boundary_difference_exponential
     boundary_maximum_division
     boundary_difference_division
     boundary_maximum_power
     boundary_difference_power
-    
+
 Regional energy terms
 ---------------------
 .. autosummary::
     :toctree: generated/
-    
+
     regional_probability_map
-    
+
 Energy terms for label-based graph-cuts :mod:`medpy.graphcut.energy_label`
 ==========================================================================
 Run-time optimized energy functions for the graph generation. Label/Superpixel based [6]_.
 
 .. module:: medpy.graphcut.energy_label
 
 Boundary energy terms
 ---------------------
 .. autosummary::
-    :toctree: generated/    
-    
+    :toctree: generated/
+
     boundary_difference_of_means
     boundary_stawiaski
     boundary_stawiaski_directed
-    
+
 Regional energy terms
 ---------------------
 .. autosummary::
     :toctree: generated/
-    
-    regional_atlas    
+
+    regional_atlas
 
 Persist a graph :mod:`medpy.graphcut.write`
 ===========================================
 Functions to persist a graph in file formats like Dimacs [5]_, which can be read by external graph-cut algorithms.
 
 .. module:: medpy.graphcut.write
 .. autosummary::
     :toctree: generated/
-    
+
     graph_to_dimacs
 
 Graph :mod:`medpy.graphcut.graph`
 =================================
 Graph objects that can be used to generate a custom graph and execute a graph-cut over it.
 
 .. module:: medpy.graphcut.graph
 .. autosummary::
     :toctree: generated/
-    
+
     GCGraph
     Graph
-    
+
 Maxflow :mod:`medpy.graphcut.maxflow`
 =====================================
 C++ wrapper around the max-flow/min-cut implementation of [4]_ using Boost.Python.
 Do not use these directly, but rather the graph objects supplied by :mod:`medpy.graphcut.graph`.
 
 .. module:: medpy.graphcut.maxflow
 .. autosummary::
     :toctree: generated/
-    
+
     GraphDouble
     GraphFloat
     GraphInt
-    
+
 Wrapper :mod:`medpy.graphcut.wrapper`
 =====================================
 Wrappers for executing graph cuts in a memory-friendly way and other convenience functions.
 
 .. module:: medpy.graphcut.wrapper
 .. autosummary::
     :toctree: generated/
-    
+
     split_marker
     graphcut_split
     graphcut_subprocesses
     graphcut_stawiaski
 
 Example of voxel based graph cut
 --------------------------------
@@ -155,17 +155,17 @@
 Executing the graph-cut (depending on the image size, this might take a while).
 
 >>> maxflow = gcgraph.maxflow()
 
 Building the resulting segmentation image, with True values for foreground and False
 values for background voxels.
 
->>> result_image_data = numpy.zeros(image_data.size, dtype=numpy.bool)
+>>> result_image_data = numpy.zeros(image_data.size, dtype=numpy.bool_)
 >>> for idx in range(len(result_image_data)):
-        result_image_data[idx] = 0 if gcgraph.termtype.SINK == gcgraph.what_segment(idx) else 1    
+        result_image_data[idx] = 0 if gcgraph.termtype.SINK == gcgraph.what_segment(idx) else 1
 >>> result_image_data = result_image_data.reshape(image_data.shape)
 
 
 References
 ----------
 .. [1] http://en.wikipedia.org/wiki/Graph_cuts_in_computer_vision
 .. [2] http://www.boost.org/doc/libs/1_55_0/libs/python/doc/
@@ -178,33 +178,45 @@
        Using Graph-cuts and watershed" MICCAI 2008 participation
 .. [7] Kolmogorov, Vladimir, and Ramin Zabin. "What energy functions can be minimized
        via graph cuts?." Pattern Analysis and Machine Intelligence, IEEE Transactions
        on 26.2 (2004): 147-159.
 """
 
 # Copyright (C) 2013 Oskar Maier
-# 
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
-# 
+#
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
-# 
+#
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-# import from compile C++ Python module
-from .maxflow import GraphDouble, GraphFloat, GraphInt # this always triggers an error in Eclipse, but is right
-
-# import all functions/methods/classes into the module
-from .graph import Graph, GCGraph
-from .write import graph_to_dimacs
-from .generate import graph_from_labels, graph_from_voxels
-from . import energy_label
-from . import energy_voxel
 
-# import all sub-modules in the __all__ variable
-__all__ = [s for s in dir() if not s.startswith('_')]
+from . import energy_label as energy_label
+from . import energy_voxel as energy_voxel
+from .generate import graph_from_labels as graph_from_labels
+from .generate import graph_from_voxels as graph_from_voxels
+from .graph import GCGraph as GCGraph
+from .graph import Graph as Graph
+from .maxflow import GraphDouble as GraphDouble  # compiled C++ Python
+from .maxflow import GraphFloat as GraphFloat  # compiled C++ Python
+from .maxflow import GraphInt as GraphInt  # compiled C++ Python
+from .write import graph_to_dimacs as graph_to_dimacs
+
+__all__ = [
+    "GraphDouble",
+    "GraphFloat",
+    "GraphInt",
+    "Graph",
+    "GCGraph",
+    "graph_to_dimacs",
+    "graph_from_labels",
+    "graph_from_voxels",
+    "energy_label",
+    "energy_voxel",
+]
```

### Comparing `MedPy-0.4.0/medpy/graphcut/energy_label.py` & `MedPy-0.5.0/medpy/graphcut/energy_label.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,413 +1,461 @@
 # Copyright (C) 2013 Oskar Maier
-# 
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
-# 
+#
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
-# 
+#
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 # author Oskar Maier
 # version r0.3.0
 # since 2012-01-18
 # status Release
 
 # build-in modules
 import math
 import sys
 
 # third-party modules
-import scipy.ndimage
 import numpy
+import scipy.ndimage
 
 # own modules
 
+
 # code
-def boundary_difference_of_means(graph, label_image, original_image): # label image is not required to hold continuous ids or to start from 1
+def boundary_difference_of_means(
+    graph, label_image, original_image
+):  # label image is not required to hold continuous ids or to start from 1
     r"""
     Boundary term based on the difference of means between adjacent image regions.
-    
+
     An implementation of the boundary term, suitable to be used with the `~medpy.graphcut.generate.graph_from_labels` function.
-    
+
     This simple energy function computes the mean values for all regions. The weights of
     the edges are then determined by the difference in mean values.
-    
+
     The graph weights generated have to be strictly positive and preferably in the
     interval :math:`(0, 1]`. To ensure this, the maximum possible difference in mean values is computed as:
-    
+
     .. math::
-    
+
         \alpha = \|\max \bar{I} - \min \bar{I}\|
-    
+
     , where :math:`\min \bar{I}` constitutes the lowest mean intensity value of all regions in
     the image, while :math:`\max \bar{I}` constitutes the highest mean intensity value With this
     value the weights between a region :math:`x` and its neighbour :math:`y` can be computed:
-    
+
     .. math::
-    
+
         w(x,y) = \max \left( 1 - \frac{\|\bar{I}_x - \bar{I}_y\|}{\alpha}, \epsilon \right)
-    
+
     where :math:`\epsilon` is the smallest floating point step and thus :math:`w(x,y) \in (0, 1]` holds true.
-    
+
     Parameters
     ----------
     graph : GCGraph
         The graph to add the weights to.
     label_image : ndarray
         The label image.
     original_image : ndarray
         The original image.
-    
+
     Notes
     -----
     This function requires the original image to be passed along. That means that
     `~medpy.graphcut.generate.graph_from_labels` has to be called with ``boundary_term_args`` set to the
-    original image. 
-    
-    This function is tested on 2D and 3D images and theoretically works for all dimensionalities. 
+    original image.
+
+    This function is tested on 2D and 3D images and theoretically works for all dimensionalities.
     """
     # convert to arrays if necessary
-    label_image = scipy.asarray(label_image)
-    original_image = scipy.asarray(original_image)
-    
-    if label_image.flags['F_CONTIGUOUS']: # strangely one this one is required to be ctype ordering
-        label_image = scipy.ascontiguousarray(label_image)
-        
+    label_image = numpy.asarray(label_image)
+    original_image = numpy.asarray(original_image)
+
+    if label_image.flags[
+        "F_CONTIGUOUS"
+    ]:  # strangely one this one is required to be ctype ordering
+        label_image = numpy.ascontiguousarray(label_image)
+
     __check_label_image(label_image)
-    
+
     # create a lookup-table that translates from a label id to its position in the sorted unique vector
-    labels_unique = scipy.unique(label_image)
-    
+    labels_unique = numpy.unique(label_image)
+
     # compute the mean intensities of all regions
     # Note: Bug in mean implementation: means over labels is only computed if the indexes are also supplied
-    means = scipy.ndimage.measurements.mean(original_image, labels=label_image, index=labels_unique)
-    
+    means = scipy.ndimage.mean(original_image, labels=label_image, index=labels_unique)
+
     # compute the maximum possible intensity difference
     max_difference = float(abs(min(means) - max(means)))
 
     # create a lookup table that relates region ids to their respective intensity values
     means = dict(list(zip(labels_unique, means)))
 
     # get the adjuncancy of the labels
     edges = __compute_edges(label_image)
-    
+
     # compute the difference of means for each adjunct region and add it as a tuple to the dictionary
-    if 0. == max_difference: # special case when the divider is zero and therefore all values can be assured to equal zero
+    if (
+        0.0 == max_difference
+    ):  # special case when the divider is zero and therefore all values can be assured to equal zero
         for edge in edges:
-            graph.set_nweight(edge[0] - 1, edge[1] - 1, sys.float_info.min, sys.float_info.min)
-    else:    
+            graph.set_nweight(
+                edge[0] - 1, edge[1] - 1, sys.float_info.min, sys.float_info.min
+            )
+    else:
         # compute the difference of means for each adjunct region and add it as a tuple to the dictionary
         for edge in edges:
-            value = max(1. - abs(means[edge[0]] - means[edge[1]]) / max_difference, sys.float_info.min)
+            value = max(
+                1.0 - abs(means[edge[0]] - means[edge[1]]) / max_difference,
+                sys.float_info.min,
+            )
             graph.set_nweight(edge[0] - 1, edge[1] - 1, value, value)
 
 
-def boundary_stawiaski(graph, label_image, gradient_image): # label image is not required to hold continuous ids or to start from 1
+def boundary_stawiaski(
+    graph, label_image, gradient_image
+):  # label image is not required to hold continuous ids or to start from 1
     r"""
     Boundary term based on the sum of border voxel pairs differences.
-     
+
     An implementation of the boundary term in [1]_, suitable to be used with the `~medpy.graphcut.generate.graph_from_labels` function.
-    
+
     Determines for each two supplied regions the voxels forming their border assuming
     :math:`ndim*2`-connectedness (e.g. :math:`3*2=6` for 3D). From the gradient magnitude values of each
     end-point voxel the border-voxel pairs, the highest one is selected and passed to a
     strictly positive and decreasing function :math:`g(x)`, which is defined as:
-    
+
     .. math::
-    
+
         g(x) = \left(\frac{1}{1+|x|}\right)^k
-    
+
     ,where :math:`k=2`. The final weight :math:`w_{i,j}` between two regions :math:`r_i` and
     :math:`r_j` is then determined by the sum of all these neighbour values:
-    
+
     .. math::
-    
+
         w_{i,j} = \sum_{e_{m,n}\in F_{(r_i,r_j)}}g(\max(|I(m)|,|I(n)|))
-    
+
     , where :math:`F_{(r_i,r_j)}` is the set of border voxel-pairs :math:`e_{m,n}` between
     the regions :math:`r_i` and :math:`r_j` and :math:`|I(p)|` the absolute of the gradient
     magnitude at the voxel :math:`p`
-    
+
     This boundary_function works as an edge indicator in the original image. In simpler
     words the weight (and therefore the energy) is obtained by summing the local contrast
     along the boundaries between two regions.
-    
+
     Parameters
     ----------
     graph : GCGraph
         The graph to add the weights to.
     label_image : ndarray
         The label image. Must contain consecutively labelled regions starting from index 1.
     gradient_image : ndarray
         The gradient image.
-    
+
     Notes
     -----
     This function requires the gradient magnitude image of the original image to be passed
     along. That means that `~medpy.graphcut.generate.graph_from_labels` has to be called
     with ``boundary_term_args`` set to the gradient image. This can be obtained e.g. with
     `generic_gradient_magnitude` and `prewitt` from `scipy.ndimage`.
-    
-    This function is tested on 2D and 3D images and theoretically works for all dimensionalities. 
-    
+
+    This function is tested on 2D and 3D images and theoretically works for all dimensionalities.
+
     References
     ----------
     .. [1] Stawiaski J., Decenciere E., Bidlaut F. "Interactive Liver Tumor Segmentation
            Using Graph-cuts and watershed" MICCAI 2008 participation
     """
     # convert to arrays if necessary
-    label_image = scipy.asarray(label_image)
-    gradient_image = scipy.asarray(gradient_image)
-    
-    if label_image.flags['F_CONTIGUOUS']: # strangely, this one is required to be ctype ordering
-        label_image = scipy.ascontiguousarray(label_image)
-        
+    label_image = numpy.asarray(label_image)
+    gradient_image = numpy.asarray(gradient_image)
+
+    if label_image.flags[
+        "F_CONTIGUOUS"
+    ]:  # strangely, this one is required to be ctype ordering
+        label_image = numpy.ascontiguousarray(label_image)
+
     __check_label_image(label_image)
-        
+
     for dim in range(label_image.ndim):
         # prepare slicer for all minus last and all minus first "row"
         slicer_from = [slice(None)] * label_image.ndim
         slicer_to = [slice(None)] * label_image.ndim
         slicer_from[dim] = slice(None, -1)
         slicer_to[dim] = slice(1, None)
         # slice views of keys
-        keys_from = label_image[slicer_from]
-        keys_to = label_image[slicer_to]
+        keys_from = label_image[tuple(slicer_from)]
+        keys_to = label_image[tuple(slicer_to)]
         # determine not equal keys
         valid_edges = keys_from != keys_to
         # determine largest gradient
-        gradient_max = numpy.maximum(numpy.abs(gradient_image[slicer_from]), numpy.abs(gradient_image[slicer_to]))[valid_edges]
+        gradient_max = numpy.maximum(
+            numpy.abs(gradient_image[tuple(slicer_from)]),
+            numpy.abs(gradient_image[tuple(slicer_to)]),
+        )[valid_edges]
         # determine key order
         keys_max = numpy.maximum(keys_from, keys_to)[valid_edges]
         keys_min = numpy.minimum(keys_from, keys_to)[valid_edges]
         # set edges / nweights
         for k1, k2, val in zip(keys_min, keys_max, gradient_max):
-            weight = math.pow(1./(1. + val), 2) # weight contribution of a single pixel
+            weight = math.pow(
+                1.0 / (1.0 + val), 2
+            )  # weight contribution of a single pixel
             weight = max(weight, sys.float_info.min)
-            graph.set_nweight(k1 - 1 , k2 - 1, weight, weight)
+            graph.set_nweight(k1 - 1, k2 - 1, weight, weight)
 
 
-def boundary_stawiaski_directed(graph, label_image, xxx_todo_changeme): # label image is not required to hold continuous ids or to start from 1
+def boundary_stawiaski_directed(
+    graph, label_image, xxx_todo_changeme
+):  # label image is not required to hold continuous ids or to start from 1
     r"""
     Boundary term based on the sum of border voxel pairs differences, directed version.
-    
+
     An implementation of the boundary term in [1]_, suitable to be used with the
     `~medpy.graphcut.generate.graph_from_labels` function.
-    
+
     The basic definition of this term is the same as for `boundary_stawiaski`, but the
     edges of the created graph will be directed.
-    
+
     This boundary_function works as an edge indicator in the original image. In simpler
     words the weight (and therefore the energy) is obtained by summing the local contrast
     along the boundaries between two regions.
-    
+
     When the ``directedness`` parameter is set to zero, the resulting graph will be undirected
     and the behaviour equals `boundary_stawiaski`.
     When it is set to a positive value, light-to-dark transitions are favored i.e. voxels
     with a lower intensity (darker) than the objects tend to be assigned to the object.
     The boundary term is thus changed to:
-    
+
     .. math::
-    
+
           g_{ltd}(x) = \left\{
               \begin{array}{l l}
                 g(x) + \beta & \quad \textrm{if $I_i > I_j$}\\
                 g(x) & \quad \textrm{if $I_i \leq I_j$}\\
               \end{array} \right.
 
     With a negative value for ``directedness``, the opposite effect can be achieved i.e.
     voxels with a higher intensity (lighter) than the objects tend to be assigned to the
     object. The boundary term is thus changed to
-    
+
     .. math::
-    
+
       g_{dtl} = \left\{
           \begin{array}{l l}
             g(x) & \quad \textrm{if $I_i > I_j$}\\
             g(x) + \beta & \quad \textrm{if $I_i \leq I_j$}\\
           \end{array} \right.
 
     Subsequently the :math:`g(x)` in the computation of :math:`w_{i,j}` is substituted by
     :math:`g_{ltd}` resp. :math:`g_{dtl}`. The value :math:`\beta` determines the power of the
     directedness and corresponds to the absolute value of the supplied ``directedness``
     parameter. Experiments showed values between 0.0001 and 0.0003 to be good candidates.
-    
+
     Parameters
     ----------
     graph : GCGraph
         The graph to add the weights to.
     label_image : ndarray
         The label image.  Must contain consecutively labelled regions starting from index 1.
     gradient_image : ndarray
         The gradient image.
     directedness : integer
         The weight of the directedness, a positive number to favour
         light-to-dark and a negative to dark-to-light transitions. See function
         description for more details.
-    
+
     Notes
     -----
     This function requires the gradient magnitude image of the original image to be passed
     along. That means that `~medpy.graphcut.generate.graph_from_labels` has to be called
     with ``boundary_term_args`` set to the gradient image. This can be obtained e.g. with
     `generic_gradient_magnitude` and `prewitt` from `scipy.ndimage`.
-    
+
     This function is tested on 2D and 3D images and theoretically works for all dimensionalities.
-    
+
     References
     ----------
     .. [1] Stawiaski J., Decenciere E., Bidlaut F. "Interactive Liver Tumor Segmentation
-           Using Graph-cuts and watershed" MICCAI 2008 participation    
+           Using Graph-cuts and watershed" MICCAI 2008 participation
     """
     (gradient_image, directedness) = xxx_todo_changeme
-    label_image = scipy.asarray(label_image)
-    gradient_image = scipy.asarray(gradient_image)
-    
-    if label_image.flags['F_CONTIGUOUS']: # strangely one this one is required to be ctype ordering
-        label_image = scipy.ascontiguousarray(label_image)
-        
+    label_image = numpy.asarray(label_image)
+    gradient_image = numpy.asarray(gradient_image)
+
+    if label_image.flags[
+        "F_CONTIGUOUS"
+    ]:  # strangely one this one is required to be ctype ordering
+        label_image = numpy.ascontiguousarray(label_image)
+
     __check_label_image(label_image)
-        
+
     beta = abs(directedness)
-        
-    def addition_directed_ltd(key1, key2, v1, v2, dic): # for light-to-dark # tested
+
+    def addition_directed_ltd(key1, key2, v1, v2, dic):  # for light-to-dark # tested
         "Takes a key defined by two uints, two voxel intensities and a dict to which it adds g(v1, v2)."
-        if not key1 == key2: # do not process voxel pairs which belong to the same region
+        if (
+            not key1 == key2
+        ):  # do not process voxel pairs which belong to the same region
             # The function used to compute the weight contribution of each voxel pair
-            weight = math.pow(1./(1. + max(abs(v1), abs(v2))), 2)
+            weight = math.pow(1.0 / (1.0 + max(abs(v1), abs(v2))), 2)
             # ensure that no value is zero; this can occur due to rounding errors
             weight = max(weight, sys.float_info.min)
             # add weighted values to already existing edge
-            if v1 > v2: graph.set_nweight(key1 - 1, key2 - 1, min(1, weight + beta), weight)
-            else: graph.set_nweight(key1 - 1, key2 - 1, weight, min(1, weight + beta))
-            
-    def addition_directed_dtl(key1, key2, v1, v2): # for dark-to-light # tested
+            if v1 > v2:
+                graph.set_nweight(key1 - 1, key2 - 1, min(1, weight + beta), weight)
+            else:
+                graph.set_nweight(key1 - 1, key2 - 1, weight, min(1, weight + beta))
+
+    def addition_directed_dtl(key1, key2, v1, v2):  # for dark-to-light # tested
         "Takes a key defined by two uints, two voxel intensities and a dict to which it adds g(v1, v2)."
-        if not key1 == key2: # do not process voxel pairs which belong to the same region
+        if (
+            not key1 == key2
+        ):  # do not process voxel pairs which belong to the same region
             # The function used to compute the weight contribution of each voxel pair
-            weight = math.pow(1./(1. + max(abs(v1), abs(v2))), 2)
+            weight = math.pow(1.0 / (1.0 + max(abs(v1), abs(v2))), 2)
             # ensure that no value is zero; this can occur due to rounding errors
             weight = max(weight, sys.float_info.min)
             # add weighted values to already existing edge
-            if v1 > v2: graph.set_nweight(key1 - 1, key2 - 1, weight, min(1, weight + beta))
-            else: graph.set_nweight(key1 - 1, key2 - 1, min(1, weight + beta), weight)
-                                                  
+            if v1 > v2:
+                graph.set_nweight(key1 - 1, key2 - 1, weight, min(1, weight + beta))
+            else:
+                graph.set_nweight(key1 - 1, key2 - 1, min(1, weight + beta), weight)
+
     # pick and vectorize the function to achieve a speedup
     if 0 > directedness:
-        vaddition = scipy.vectorize(addition_directed_dtl)
+        vaddition = numpy.vectorize(addition_directed_dtl)
     else:
-        vaddition = scipy.vectorize(addition_directed_ltd)
-    
+        vaddition = numpy.vectorize(addition_directed_ltd)
+
     # iterate over each dimension
     for dim in range(label_image.ndim):
         slices_x = []
         slices_y = []
         for di in range(label_image.ndim):
             slices_x.append(slice(None, -1 if di == dim else None))
             slices_y.append(slice(1 if di == dim else None, None))
-        vaddition(label_image[slices_x],
-                  label_image[slices_y],
-                  gradient_image[slices_x],
-                  gradient_image[slices_y])
+        vaddition(
+            label_image[tuple(slices_x)],
+            label_image[tuple(slices_y)],
+            gradient_image[tuple(slices_x)],
+            gradient_image[tuple(slices_y)],
+        )
 
-def regional_atlas(graph, label_image, xxx_todo_changeme1): # label image is required to hold continuous ids starting from 1
+
+def regional_atlas(
+    graph, label_image, xxx_todo_changeme1
+):  # label image is required to hold continuous ids starting from 1
     r"""
     Regional term based on a probability atlas.
-    
+
     An implementation of a regional term, suitable to be used with the
     `~medpy.graphcut.generate.graph_from_labels` function.
-    
+
     This regional term introduces statistical probability of a voxel to belong to the
     object to segment. It computes the sum of all statistical atlas voxels under each
     region and uses this value as terminal node weight for the graph cut.
 
     Parameters
     ----------
     graph : GCGraph
         The graph to add the weights to.
     label_image : ndarray
         The label image.
     probability_map : ndarray
         The probability atlas image associated with the object to segment.
     alpha : float
-        The energy terms alpha value, balancing between boundary and regional term. 
-    
+        The energy terms alpha value, balancing between boundary and regional term.
+
     Notes
     -----
     This function requires a probability atlas image of the same shape as the original image
     to be passed along. That means that `~medpy.graphcut.generate.graph_from_labels` has to
     be called with ``regional_term_args`` set to the probability atlas image.
-    
-    This function is tested on 2D and 3D images and theoretically works for all dimensionalities.    
+
+    This function is tested on 2D and 3D images and theoretically works for all dimensionalities.
     """
     (probability_map, alpha) = xxx_todo_changeme1
-    label_image = scipy.asarray(label_image)
-    probability_map = scipy.asarray(probability_map)
+    label_image = numpy.asarray(label_image)
+    probability_map = numpy.asarray(probability_map)
     __check_label_image(label_image)
-    
+
     # finding the objects in the label image (bounding boxes around regions)
     objects = scipy.ndimage.find_objects(label_image)
-    
+
     # iterate over regions and compute the respective sums of atlas values
     for rid in range(1, len(objects) + 1):
-        weight = scipy.sum(probability_map[objects[rid - 1]][label_image[objects[rid - 1]] == rid])
-        graph.set_tweight(rid - 1, alpha * weight, -1. * alpha * weight) # !TODO: rid's inside the graph start from 0 or 1? => seems to start from 0
+        weight = numpy.sum(
+            probability_map[objects[rid - 1]][label_image[objects[rid - 1]] == rid]
+        )
+        graph.set_tweight(
+            rid - 1, alpha * weight, -1.0 * alpha * weight
+        )  # !TODO: rid's inside the graph start from 0 or 1? => seems to start from 0
         # !TODO: I can exclude source and sink nodes from this!
         # !TODO: I only have to do this in the range of the atlas objects!
 
 
 def __compute_edges(label_image):
     """
     Computes the region neighbourhood defined by a star shaped n-dimensional structuring
     element (as returned by scipy.ndimage.generate_binary_structure(ndim, 1)) for the
     supplied region/label image.
     Note The returned set contains neither duplicates, nor self-references
     (i.e. (id_1, id_1)), nor reversed references (e.g. (id_1, id_2) and (id_2, id_1).
-    
+
     @param label_image An image with labeled regions (nD).
     @param return A set with tuples denoting the edge neighbourhood.
     """
     return __compute_edges_nd(label_image)
-    
+
+
 def __compute_edges_nd(label_image):
     """
     Computes the region neighbourhood defined by a star shaped n-dimensional structuring
     element (as returned by scipy.ndimage.generate_binary_structure(ndim, 1)) for the
     supplied region/label image.
     Note The returned set contains neither duplicates, nor self-references
     (i.e. (id_1, id_1)), nor reversed references (e.g. (id_1, id_2) and (id_2, id_1).
-    
+
     @param label_image An image with labeled regions (nD).
     @param return A set with tuples denoting the edge neighbourhood.
     """
     Er = set()
-   
+
     def append(v1, v2):
         if v1 != v2:
             Er.update([(min(v1, v2), max(v1, v2))])
-        
-    vappend = scipy.vectorize(append)
-   
+
+    vappend = numpy.vectorize(append)
+
     for dim in range(label_image.ndim):
         slices_x = []
         slices_y = []
         for di in range(label_image.ndim):
             slices_x.append(slice(None, -1 if di == dim else None))
             slices_y.append(slice(1 if di == dim else None, None))
-        vappend(label_image[slices_x], label_image[slices_y])
-        
+        vappend(label_image[tuple(slices_x)], label_image[tuple(slices_y)])
+
     return Er
 
+
 def __check_label_image(label_image):
     """Check the label image for consistent labelling starting from 1."""
-    encountered_indices = scipy.unique(label_image)
-    expected_indices = scipy.arange(1, label_image.max() + 1)
-    if not encountered_indices.size == expected_indices.size or \
-       not (encountered_indices == expected_indices).all():
-        raise AttributeError('The supplied label image does either not contain any regions or they are not labeled consecutively starting from 1.')
+    encountered_indices = numpy.unique(label_image)
+    expected_indices = numpy.arange(1, label_image.max() + 1)
+    if (
+        not encountered_indices.size == expected_indices.size
+        or not (encountered_indices == expected_indices).all()
+    ):
+        raise AttributeError(
+            "The supplied label image does either not contain any regions or they are not labeled consecutively starting from 1."
+        )
```

### Comparing `MedPy-0.4.0/medpy/graphcut/generate.py` & `MedPy-0.5.0/medpy/graphcut/generate.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,67 +1,70 @@
 # Copyright (C) 2013 Oskar Maier
-# 
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
-# 
+#
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
-# 
+#
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 # author Oskar Maier
 # version r0.3.0
 # since 2012-01-18
 # status Release
 
 # build-in modules
 import inspect
 
 # third-party modules
-import scipy
+import numpy
 
 # own modules
 from ..core import Logger
+from .energy_label import __check_label_image
 from .graph import GCGraph
-from medpy.graphcut.energy_label import __check_label_image
 
-def graph_from_voxels(fg_markers,
-                        bg_markers,
-                        regional_term = False,
-                        boundary_term = False,
-                        regional_term_args = False,
-                        boundary_term_args = False):
+
+def graph_from_voxels(
+    fg_markers,
+    bg_markers,
+    regional_term=False,
+    boundary_term=False,
+    regional_term_args=False,
+    boundary_term_args=False,
+):
     """
     Create a graph-cut ready graph to segment a nD image using the voxel neighbourhood.
-    
+
     Create a `~medpy.graphcut.maxflow.GraphDouble` object for all voxels of an image with a
     :math:`ndim * 2` neighbourhood.
-    
+
     Every voxel of the image is regarded as a node. They are connected to their immediate
     neighbours via arcs. If to voxels are neighbours is determined using
     :math:`ndim*2`-connectedness (e.g. :math:`3*2=6` for 3D). In the next step the arcs weights
     (n-weights) are computed using the supplied ``boundary_term`` function
     (see :mod:`~medpy.graphcut.energy_voxel` for a selection).
-    
+
     Implicitly the graph holds two additional nodes: the source and the sink, so called
     terminal nodes. These are connected with all other nodes through arcs of an initial
     weight (t-weight) of zero.
     All voxels that are under the foreground markers are considered to be tightly bound
     to the source: The t-weight of the arc from source to these nodes is set to a maximum
     value. The same goes for the background markers: The covered voxels receive a maximum
     (`~medpy.graphcut.graph.GCGraph.MAX`) t-weight for their arc towards the sink.
-    
+
     All other t-weights are set using the supplied ``regional_term`` function
     (see :mod:`~medpy.graphcut.energy_voxel` for a selection).
-    
+
     Parameters
     ----------
     fg_markers : ndarray
         The foreground markers as binary array of the same shape as the original image.
     bg_markers : ndarray
         The background markers as binary array of the same shape as the original image.
     regional_term : function
@@ -79,113 +82,134 @@
         supplied function is used to compute the edge weights. It has to have the
         following signature *boundary_term(graph, boundary_term_args)*, and is supposed
         to compute the edges between the graphs nodes and to add them to the supplied
         `~medpy.graphcut.graph.GCGraph` object. Additional parameters can be passed to
         the function via the ``boundary_term_args`` parameter.
     regional_term_args : tuple
         Use this to pass some additional parameters to the ``regional_term`` function.
-    boundary_term_args : tuple    
+    boundary_term_args : tuple
         Use this to pass some additional parameters to the ``boundary_term`` function.
-    
+
     Returns
     -------
     graph : `~medpy.graphcut.maxflow.GraphDouble`
         The created graph, ready to execute the graph-cut.
-    
+
     Raises
     ------
     AttributeError
         If an argument is malformed.
     FunctionError
         If one of the supplied functions returns unexpected results.
-    
+
     Notes
     -----
     If a voxel is marked as both, foreground and background, the background marker
     is given higher priority.
-     
+
     All arcs whose weight is not explicitly set are assumed to carry a weight of zero.
     """
     # prepare logger
     logger = Logger.getInstance()
-    
+
     # prepare result graph
-    logger.debug('Assuming {} nodes and {} edges for image of shape {}'.format(fg_markers.size, __voxel_4conectedness(fg_markers.shape), fg_markers.shape)) 
+    logger.debug(
+        "Assuming {} nodes and {} edges for image of shape {}".format(
+            fg_markers.size, __voxel_4conectedness(fg_markers.shape), fg_markers.shape
+        )
+    )
     graph = GCGraph(fg_markers.size, __voxel_4conectedness(fg_markers.shape))
-    
-    logger.info('Performing attribute tests...')
-    
+
+    logger.info("Performing attribute tests...")
+
     # check, set and convert all supplied parameters
-    fg_markers = scipy.asarray(fg_markers, dtype=scipy.bool_)
-    bg_markers = scipy.asarray(bg_markers, dtype=scipy.bool_)
-    
+    fg_markers = numpy.asarray(fg_markers, dtype=numpy.bool_)
+    bg_markers = numpy.asarray(bg_markers, dtype=numpy.bool_)
+
     # set dummy functions if not supplied
-    if not regional_term: regional_term = __regional_term_voxel
-    if not boundary_term: boundary_term = __boundary_term_voxel
-    
+    if not regional_term:
+        regional_term = __regional_term_voxel
+    if not boundary_term:
+        boundary_term = __boundary_term_voxel
+
     # check supplied functions and their signature
-    if not hasattr(regional_term, '__call__') or not 2 == len(inspect.getargspec(regional_term)[0]):
-        raise AttributeError('regional_term has to be a callable object which takes two parameter.')
-    if not hasattr(boundary_term, '__call__') or not 2 == len(inspect.getargspec(boundary_term)[0]):
-        raise AttributeError('boundary_term has to be a callable object which takes two parameters.')
-
-    logger.debug('#nodes={}, #hardwired-nodes source/sink={}/{}'.format(fg_markers.size,
-                                                                        len(fg_markers.ravel().nonzero()[0]),
-                                                                        len(bg_markers.ravel().nonzero()[0])))
-    
+    if not hasattr(regional_term, "__call__") or not 2 == len(
+        inspect.getfullargspec(regional_term)[0]
+    ):
+        raise AttributeError(
+            "regional_term has to be a callable object which takes two parameter."
+        )
+    if not hasattr(boundary_term, "__call__") or not 2 == len(
+        inspect.getfullargspec(boundary_term)[0]
+    ):
+        raise AttributeError(
+            "boundary_term has to be a callable object which takes two parameters."
+        )
+
+    logger.debug(
+        "#nodes={}, #hardwired-nodes source/sink={}/{}".format(
+            fg_markers.size,
+            len(fg_markers.ravel().nonzero()[0]),
+            len(bg_markers.ravel().nonzero()[0]),
+        )
+    )
+
     # compute the weights of all edges from the source and to the sink i.e.
     # compute the weights of the t_edges Wt
-    logger.info('Computing and adding terminal edge weights...')
+    logger.info("Computing and adding terminal edge weights...")
     regional_term(graph, regional_term_args)
 
     # compute the weights of the edges between the neighbouring nodes i.e.
     # compute the weights of the n_edges Wr
-    logger.info('Computing and adding inter-node edge weights...')
+    logger.info("Computing and adding inter-node edge weights...")
     boundary_term(graph, boundary_term_args)
-    
+
     # collect all voxels that are under the foreground resp. background markers i.e.
     # collect all nodes that are connected to the source resp. sink
-    logger.info('Setting terminal weights for the markers...')
-    if not 0 == scipy.count_nonzero(fg_markers):
+    logger.info("Setting terminal weights for the markers...")
+    if not 0 == numpy.count_nonzero(fg_markers):
         graph.set_source_nodes(fg_markers.ravel().nonzero()[0])
-    if not 0 == scipy.count_nonzero(bg_markers):
-        graph.set_sink_nodes(bg_markers.ravel().nonzero()[0])    
-    
+    if not 0 == numpy.count_nonzero(bg_markers):
+        graph.set_sink_nodes(bg_markers.ravel().nonzero()[0])
+
     return graph.get_graph()
 
-def graph_from_labels(label_image,
-                        fg_markers,
-                        bg_markers,
-                        regional_term = False,
-                        boundary_term = False,
-                        regional_term_args = False,
-                        boundary_term_args = False):
+
+def graph_from_labels(
+    label_image,
+    fg_markers,
+    bg_markers,
+    regional_term=False,
+    boundary_term=False,
+    regional_term_args=False,
+    boundary_term_args=False,
+):
     """
     Create a graph-cut ready graph to segment a nD image using the region neighbourhood.
-    
+
     Create a `~medpy.graphcut.maxflow.GraphDouble` object for all regions of a nD label
     image.
-    
+
     Every region of the label image is regarded as a node. They are connected to their
     immediate neighbours by arcs. If to regions are neighbours is determined using
     :math:`ndim*2`-connectedness (e.g. :math:`3*2=6` for 3D).
     In the next step the arcs weights (n-weights) are computed using the supplied
     ``boundary_term`` function (see :mod:`~medpy.graphcut.energy_voxel` for a selection).
-    
+
     Implicitly the graph holds two additional nodes: the source and the sink, so called
     terminal nodes. These are connected with all other nodes through arcs of an initial
     weight (t-weight) of zero.
     All regions that are under the foreground markers are considered to be tightly bound
-    to the source: The t-weight of the arc from source to these nodes is set to a maximum 
+    to the source: The t-weight of the arc from source to these nodes is set to a maximum
     value. The same goes for the background markers: The covered regions receive a
     maximum (`~medpy.graphcut.graph.GCGraph.MAX`) t-weight for their arc towards the sink.
-    
+
     All other t-weights are set using the supplied ``regional_term`` function
     (see :mod:`~medpy.graphcut.energy_voxel` for a selection).
-    
+
     Parameters
     ----------
     label_image: ndarray
         The label image as an array cwhere each voxel carries the id of the region it
         belongs to. Note that the region labels have to start from 1 and be continuous
         (can be achieved with `~medpy.filter.label.relabel`).
     fg_markers : ndarray
@@ -207,125 +231,153 @@
         supplied function is used to compute the edge weights. It has to have the
         following signature *boundary_term(graph, boundary_term_args)*, and is supposed
         to compute the edges between all adjacent regions of the image and to add them
         to the supplied `~medpy.graphcut.graph.GCGraph` object. Additional parameters
         can be passed to the function via the ``boundary_term_args`` parameter.
     regional_term_args : tuple
         Use this to pass some additional parameters to the ``regional_term`` function.
-    boundary_term_args : tuple    
+    boundary_term_args : tuple
         Use this to pass some additional parameters to the ``boundary_term`` function.
 
     Returns
     -------
     graph : `~medpy.graphcut.maxflow.GraphDouble`
         The created graph, ready to execute the graph-cut.
-    
+
     Raises
     ------
     AttributeError
         If an argument is malformed.
     FunctionError
         If one of the supplied functions returns unexpected results.
-    
+
     Notes
     -----
     If a voxel is marked as both, foreground and background, the background marker
     is given higher priority.
-     
-    All arcs whose weight is not explicitly set are assumed to carry a weight of zero.    
-    """    
+
+    All arcs whose weight is not explicitly set are assumed to carry a weight of zero.
+    """
     # prepare logger
     logger = Logger.getInstance()
-    
-    logger.info('Performing attribute tests...')
-    
+
+    logger.info("Performing attribute tests...")
+
     # check, set and convert all supplied parameters
-    label_image = scipy.asarray(label_image)
-    fg_markers = scipy.asarray(fg_markers, dtype=scipy.bool_)
-    bg_markers = scipy.asarray(bg_markers, dtype=scipy.bool_)
-    
+    label_image = numpy.asarray(label_image)
+    fg_markers = numpy.asarray(fg_markers, dtype=numpy.bool_)
+    bg_markers = numpy.asarray(bg_markers, dtype=numpy.bool_)
+
     __check_label_image(label_image)
-    
+
     # set dummy functions if not supplied
-    if not regional_term: regional_term = __regional_term_label
-    if not boundary_term: boundary_term = __boundary_term_label
-    
+    if not regional_term:
+        regional_term = __regional_term_label
+    if not boundary_term:
+        boundary_term = __boundary_term_label
+
     # check supplied functions and their signature
-    if not hasattr(regional_term, '__call__') or not 3 == len(inspect.getargspec(regional_term)[0]):
-        raise AttributeError('regional_term has to be a callable object which takes three parameters.')
-    if not hasattr(boundary_term, '__call__') or not 3 == len(inspect.getargspec(boundary_term)[0]):
-        raise AttributeError('boundary_term has to be a callable object which takes three parameters.')    
-    
-    logger.info('Determining number of nodes and edges.')
-    
+    if not hasattr(regional_term, "__call__") or not 3 == len(
+        inspect.getargspec(regional_term)[0]
+    ):
+        raise AttributeError(
+            "regional_term has to be a callable object which takes three parameters."
+        )
+    if not hasattr(boundary_term, "__call__") or not 3 == len(
+        inspect.getargspec(boundary_term)[0]
+    ):
+        raise AttributeError(
+            "boundary_term has to be a callable object which takes three parameters."
+        )
+
+    logger.info("Determining number of nodes and edges.")
+
     # compute number of nodes and edges
-    nodes = len(scipy.unique(label_image))
+    nodes = len(numpy.unique(label_image))
     # POSSIBILITY 1: guess the number of edges (in the best situation is faster but requires a little bit more memory. In the worst is slower.)
     edges = 10 * nodes
-    logger.debug('guessed: #nodes={} nodes / #edges={}'.format(nodes, edges))
+    logger.debug("guessed: #nodes={} nodes / #edges={}".format(nodes, edges))
     # POSSIBILITY 2: compute the edges (slow)
-    #edges = len(__compute_edges(label_image))
-    #logger.debug('computed: #nodes={} nodes / #edges={}'.format(nodes, edges))
-        
+    # edges = len(__compute_edges(label_image))
+    # logger.debug('computed: #nodes={} nodes / #edges={}'.format(nodes, edges))
+
     # prepare result graph
     graph = GCGraph(nodes, edges)
-                                        
-    logger.debug('#hardwired-nodes source/sink={}/{}'.format(len(scipy.unique(label_image[fg_markers])),
-                                                             len(scipy.unique(label_image[bg_markers]))))
-                 
-    #logger.info('Extracting the regions bounding boxes...')
+
+    logger.debug(
+        "#hardwired-nodes source/sink={}/{}".format(
+            len(numpy.unique(label_image[fg_markers])),
+            len(numpy.unique(label_image[bg_markers])),
+        )
+    )
+
+    # logger.info('Extracting the regions bounding boxes...')
     # extract the bounding boxes
-    #bounding_boxes = find_objects(label_image)
-        
+    # bounding_boxes = find_objects(label_image)
+
     # compute the weights of all edges from the source and to the sink i.e.
     # compute the weights of the t_edges Wt
-    logger.info('Computing and adding terminal edge weights...')
-    #regions = set(graph.get_nodes()) - set(graph.get_source_nodes()) - set(graph.get_sink_nodes())
-    regional_term(graph, label_image, regional_term_args) # bounding boxes indexed from 0 # old version: regional_term(graph, label_image, regions, bounding_boxes, regional_term_args)
+    logger.info("Computing and adding terminal edge weights...")
+    # regions = set(graph.get_nodes()) - set(graph.get_source_nodes()) - set(graph.get_sink_nodes())
+    regional_term(
+        graph, label_image, regional_term_args
+    )  # bounding boxes indexed from 0 # old version: regional_term(graph, label_image, regions, bounding_boxes, regional_term_args)
 
     # compute the weights of the edges between the neighbouring nodes i.e.
     # compute the weights of the n_edges Wr
-    logger.info('Computing and adding inter-node edge weights...')
+    logger.info("Computing and adding inter-node edge weights...")
     boundary_term(graph, label_image, boundary_term_args)
-    
+
     # collect all regions that are under the foreground resp. background markers i.e.
     # collect all nodes that are connected to the source resp. sink
-    logger.info('Setting terminal weights for the markers...')
-    graph.set_source_nodes(scipy.unique(label_image[fg_markers] - 1)) # requires -1 to adapt to node id system
-    graph.set_sink_nodes(scipy.unique(label_image[bg_markers] - 1))
-    
+    logger.info("Setting terminal weights for the markers...")
+    graph.set_source_nodes(
+        numpy.unique(label_image[fg_markers] - 1)
+    )  # requires -1 to adapt to node id system
+    graph.set_sink_nodes(numpy.unique(label_image[bg_markers] - 1))
+
     return graph.get_graph()
 
+
 def __regional_term_voxel(graph, regional_term_args):
     """Fake regional_term function with the appropriate signature."""
     return {}
 
+
 def __regional_term_label(graph, label_image, regional_term_args):
     """Fake regional_term function with the appropriate signature."""
     return {}
 
+
 def __boundary_term_voxel(graph, boundary_term_args):
     """Fake regional_term function with the appropriate signature."""
     # supplying no boundary term contradicts the whole graph cut idea.
     return {}
 
+
 def __boundary_term_label(graph, label_image, boundary_term_args):
     """Fake regional_term function with the appropriate signature."""
     # supplying no boundary term contradicts the whole graph cut idea.
     return {}
-    
+
+
 def __voxel_4conectedness(shape):
     """
     Returns the number of edges for the supplied image shape assuming 4-connectedness.
-    
+
     The name of the function has historical reasons. Essentially it returns the number
     of edges assuming 4-connectedness only for 2D. For 3D it assumes 6-connectedness,
     etc.
-    
+
     @param shape the shape of the image
     @type shape sequence
     @return the number of edges
     @rtype int
     """
     shape = list(shape)
-    while 1 in shape: shape.remove(1) # empty resp. 1-sized dimensions have to be removed (equal to scipy.squeeze on the array)
-    return int(round(sum([(dim - 1)/float(dim) for dim in shape]) * scipy.prod(shape)))
+    while 1 in shape:
+        shape.remove(
+            1
+        )  # empty resp. 1-sized dimensions have to be removed (equal to numpy.squeeze on the array)
+    return int(
+        round(sum([(dim - 1) / float(dim) for dim in shape]) * numpy.prod(shape))
+    )
```

### Comparing `MedPy-0.4.0/medpy/graphcut/energy_voxel.py` & `MedPy-0.5.0/medpy/graphcut/energy_voxel.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,602 +1,623 @@
 # Copyright (C) 2013 Oskar Maier
-# 
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
-# 
+#
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
-# 
+#
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 # author Oskar Maier
 # version r0.3.0
 # since 2012-03-23
 # status Release
 
+import math
+
 # build-in modules
 import sys
 
 # third-party modules
 import numpy
-import scipy
-import math
 
 # own modules
 
+
 # code
 def regional_probability_map(graph, xxx_todo_changeme):
     r"""
     Regional term based on a probability atlas.
-    
+
     An implementation of a regional term, suitable to be used with the
     `~medpy.graphcut.generate.graph_from_voxels` function.
-    
+
     Takes an image/graph/map as input where each entry contains a probability value for
     the corresponding GC graph node to belong to the foreground object. The probabilities
     must be in the range :math:`[0, 1]`. The reverse weights are assigned to the sink
     (which corresponds to the background).
-    
+
     Parameters
     ----------
     graph : GCGraph
         The graph to add the weights to.
     probability_map : ndarray
         The label image.
     alpha : float
         The energy terms alpha value, balancing between boundary and regional term.
-    
+
     Notes
     -----
     This function requires a probability atlas image of the same shape as the original image
     to be passed along. That means that `~medpy.graphcut.generate.graph_from_labels` has to
     be called with ``regional_term_args`` set to the probability atlas image.
     """
     (probability_map, alpha) = xxx_todo_changeme
-    probability_map = scipy.asarray(probability_map)
-    probabilities = numpy.vstack([(probability_map * alpha).flat,
-                                  ((1 - probability_map) * alpha).flat]).T
+    probability_map = numpy.asarray(probability_map)
+    probabilities = numpy.vstack(
+        [(probability_map * alpha).flat, ((1 - probability_map) * alpha).flat]
+    ).T
     graph.set_tweights_all(probabilities)
 
+
 def boundary_maximum_linear(graph, xxx_todo_changeme1):
     r"""
-    Boundary term processing adjacent voxels maximum value using a linear relationship. 
-    
+    Boundary term processing adjacent voxels maximum value using a linear relationship.
+
     An implementation of a boundary term, suitable to be used with the
     `~medpy.graphcut.generate.graph_from_voxels` function.
-    
+
     The same as `boundary_difference_linear`, but working on the gradient image instead
     of the original. See there for details.
-    
+
     Parameters
     ----------
     graph : GCGraph
         The graph to add the weights to.
     gradient_image : ndarray
         The gradient image.
     spacing : sequence of float or False
         A sequence containing the slice spacing used for weighting the
         computed neighbourhood weight value for different dimensions. If
         `False`, no distance based weighting of the graph edges is performed.
-        
+
     Notes
     -----
     This function requires the gradient image to be passed along. That means that
     `~medpy.graphcut.generate.graph_from_voxels` has to be called with ``boundary_term_args`` set to the
     gradient image.
     """
     (gradient_image, spacing) = xxx_todo_changeme1
-    gradient_image = scipy.asarray(gradient_image)
-    
+    gradient_image = numpy.asarray(gradient_image)
+
     # compute maximum intensity to encounter
     max_intensity = float(numpy.abs(gradient_image).max())
-    
+
     def boundary_term_linear(intensities):
         """
         Implementation of a linear boundary term computation over an array.
         """
         # normalize the intensity distances to the interval (0, 1]
         intensities /= max_intensity
-        #difference_to_neighbour[difference_to_neighbour > 1] = 1 # this line should not be required, but might be due to rounding errors
-        intensities = (1. - intensities) # reverse weights such that high intensity difference lead to small weights and hence more likely to a cut at this edge
-        intensities[intensities == 0.] = sys.float_info.min # required to avoid zero values
+        # difference_to_neighbour[difference_to_neighbour > 1] = 1 # this line should not be required, but might be due to rounding errors
+        intensities = (
+            1.0 - intensities
+        )  # reverse weights such that high intensity difference lead to small weights and hence more likely to a cut at this edge
+        intensities[
+            intensities == 0.0
+        ] = sys.float_info.min  # required to avoid zero values
         return intensities
-    
+
     __skeleton_maximum(graph, gradient_image, boundary_term_linear, spacing)
 
+
 def boundary_difference_linear(graph, xxx_todo_changeme2):
     r"""
-    Boundary term processing adjacent voxels difference value using a linear relationship. 
-    
+    Boundary term processing adjacent voxels difference value using a linear relationship.
+
     An implementation of a regional term, suitable to be used with the
     `~medpy.graphcut.generate.graph_from_voxels` function.
-    
+
     Finds all edges between all neighbours of the image and uses their normalized
     difference in intensity values as edge weight.
-    
+
     The weights are linearly normalized using the maximum possible intensity difference
     of the image. Formally, this value is computed as:
-    
+
     .. math::
-    
+
         \sigma = |max I - \min I|
-    
+
     , where :math:`\min I` constitutes the lowest intensity value in the image, while
     :math:`\max I` constitutes the highest.
-    
+
     The weights between two neighbouring voxels :math:`(p, q)` is then computed as:
-    
+
     .. math::
-    
+
         w(p,q) = 1 - \frac{|I_p - I_q|}{\sigma} + \epsilon
-    
+
     , where :math:`\epsilon` is a infinitively small number and for which
     :math:`w(p, q) \in (0, 1]` holds true.
-    
+
     When the created edge weights should be weighted according to the slice distance,
     provide the list of slice thicknesses via the ``spacing`` parameter. Then all weights
     computed for the corresponding direction are divided by the respective slice
-    thickness. Set this parameter to `False` for equally weighted edges.     
-    
+    thickness. Set this parameter to `False` for equally weighted edges.
+
     Parameters
     ----------
     graph : GCGraph
         The graph to add the weights to.
     original_image : ndarray
         The original image.
     spacing : sequence of float or False
         A sequence containing the slice spacing used for weighting the
         computed neighbourhood weight value for different dimensions. If
         `False`, no distance based weighting of the graph edges is performed.
-        
+
     Notes
     -----
     This function requires the original image to be passed along. That means that
     `~medpy.graphcut.generate.graph_from_voxels` has to be called with ``boundary_term_args`` set to the
     original image.
     """
     (original_image, spacing) = xxx_todo_changeme2
-    original_image = scipy.asarray(original_image)
-    
+    original_image = numpy.asarray(original_image)
+
     # compute maximum (possible) intensity difference
     max_intensity_difference = float(abs(original_image.max() - original_image.min()))
-    
+
     def boundary_term_linear(intensities):
         """
         Implementation of a linear boundary term computation over an array.
         """
         # normalize the intensity distances to the interval (0, 1]
         intensities /= max_intensity_difference
-        #difference_to_neighbour[difference_to_neighbour > 1] = 1 # this line should not be required, but might be due to rounding errors
-        intensities = (1. - intensities) # reverse weights such that high intensity difference lead to small weights and hence more likely to a cut at this edge
-        intensities[intensities == 0.] = sys.float_info.min # required to avoid zero values
+        # difference_to_neighbour[difference_to_neighbour > 1] = 1 # this line should not be required, but might be due to rounding errors
+        intensities = (
+            1.0 - intensities
+        )  # reverse weights such that high intensity difference lead to small weights and hence more likely to a cut at this edge
+        intensities[
+            intensities == 0.0
+        ] = sys.float_info.min  # required to avoid zero values
         return intensities
-    
+
     __skeleton_difference(graph, original_image, boundary_term_linear, spacing)
 
+
 def boundary_maximum_exponential(graph, xxx_todo_changeme3):
     r"""
-    Boundary term processing adjacent voxels maximum value using an exponential relationship. 
-    
+    Boundary term processing adjacent voxels maximum value using an exponential relationship.
+
     An implementation of a boundary term, suitable to be used with the
     `~medpy.graphcut.generate.graph_from_voxels` function.
-    
+
     The same as `boundary_difference_exponential`, but working on the gradient image instead
     of the original. See there for details.
-    
+
     Parameters
     ----------
     graph : GCGraph
         The graph to add the weights to.
     gradient_image : ndarray
         The gradient image.
     sigma : float
         The sigma parameter to use in the boundary term.
     spacing : sequence of float or False
         A sequence containing the slice spacing used for weighting the
         computed neighbourhood weight value for different dimensions. If
         `False`, no distance based weighting of the graph edges is performed.
-        
+
     Notes
     -----
     This function requires the gradient image to be passed along. That means that
     `~medpy.graphcut.generate.graph_from_voxels` has to be called with ``boundary_term_args`` set to the
     gradient image.
     """
     (gradient_image, sigma, spacing) = xxx_todo_changeme3
-    gradient_image = scipy.asarray(gradient_image)
-    
+    gradient_image = numpy.asarray(gradient_image)
+
     def boundary_term_exponential(intensities):
         """
         Implementation of a exponential boundary term computation over an array.
         """
         # apply exp-(x**2/sigma**2)
-        intensities = scipy.power(intensities, 2)
+        intensities = numpy.power(intensities, 2)
         intensities /= math.pow(sigma, 2)
         intensities *= -1
-        intensities = scipy.exp(intensities)
+        intensities = numpy.exp(intensities)
         intensities[intensities <= 0] = sys.float_info.min
         return intensities
-    
-    __skeleton_maximum(graph, gradient_image, boundary_term_exponential, spacing)    
+
+    __skeleton_maximum(graph, gradient_image, boundary_term_exponential, spacing)
+
 
 def boundary_difference_exponential(graph, xxx_todo_changeme4):
     r"""
     Boundary term processing adjacent voxels difference value using an exponential relationship.
-    
+
     An implementation of a boundary term, suitable to be used with the
     `~medpy.graphcut.generate.graph_from_voxels` function.
-    
+
     Finds all edges between all neighbours of the image and uses their difference in
     intensity values as edge weight.
-    
+
     The weights are normalized using an exponential function and a smoothing factor
     :math:`\sigma`. The :math:`\sigma` value has to be supplied manually, since its
     ideal settings differ greatly from application to application.
-    
+
     The weights between two neighbouring voxels :math:`(p, q)` is then computed as
-    
+
     .. math::
-    
+
         w(p,q) = \exp^{-\frac{|I_p - I_q|^2}{\sigma^2}}
-    
+
     , for which :math:`w(p, q) \in (0, 1]` holds true.
-    
+
     When the created edge weights should be weighted according to the slice distance,
     provide the list of slice thicknesses via the ``spacing`` parameter. Then all weights
     computed for the corresponding direction are divided by the respective slice
-    thickness. Set this parameter to `False` for equally weighted edges.     
-    
+    thickness. Set this parameter to `False` for equally weighted edges.
+
     Parameters
     ----------
     graph : GCGraph
         The graph to add the weights to.
     original_image : ndarray
         The original image.
     sigma : float
         The sigma parameter to use in the boundary term.
     spacing : sequence of float or False
         A sequence containing the slice spacing used for weighting the
         computed neighbourhood weight value for different dimensions. If
         `False`, no distance based weighting of the graph edges is performed.
-        
+
     Notes
     -----
     This function requires the original image to be passed along. That means that
     `~medpy.graphcut.generate.graph_from_voxels` has to be called with ``boundary_term_args`` set to the
     original image.
     """
     (original_image, sigma, spacing) = xxx_todo_changeme4
-    original_image = scipy.asarray(original_image)
-    
+    original_image = numpy.asarray(original_image)
+
     def boundary_term_exponential(intensities):
         """
         Implementation of a exponential boundary term computation over an array.
         """
         # apply exp-(x**2/sigma**2)
-        intensities = scipy.power(intensities, 2)
+        intensities = numpy.power(intensities, 2)
         intensities /= math.pow(sigma, 2)
         intensities *= -1
-        intensities = scipy.exp(intensities)
+        intensities = numpy.exp(intensities)
         intensities[intensities <= 0] = sys.float_info.min
         return intensities
-    
+
     __skeleton_difference(graph, original_image, boundary_term_exponential, spacing)
-    
+
+
 def boundary_maximum_division(graph, xxx_todo_changeme5):
     r"""
-    Boundary term processing adjacent voxels maximum value using a division relationship. 
-    
+    Boundary term processing adjacent voxels maximum value using a division relationship.
+
     An implementation of a boundary term, suitable to be used with the
     `~medpy.graphcut.generate.graph_from_voxels` function.
-    
+
     The same as `boundary_difference_division`, but working on the gradient image instead
     of the original. See there for details.
-    
+
     Parameters
     ----------
     graph : GCGraph
         The graph to add the weights to.
     gradient_image : ndarray
         The gradient image.
     sigma : float
         The sigma parameter to use in the boundary term.
     spacing : sequence of float or False
         A sequence containing the slice spacing used for weighting the
         computed neighbourhood weight value for different dimensions. If
         `False`, no distance based weighting of the graph edges is performed.
-        
+
     Notes
     -----
     This function requires the gradient image to be passed along. That means that
     `~medpy.graphcut.generate.graph_from_voxels` has to be called with ``boundary_term_args`` set to the
     gradient image.
     """
     (gradient_image, sigma, spacing) = xxx_todo_changeme5
-    gradient_image = scipy.asarray(gradient_image)
-    
+    gradient_image = numpy.asarray(gradient_image)
+
     def boundary_term_division(intensities):
         """
         Implementation of a exponential boundary term computation over an array.
         """
         # apply 1 / (1  + x/sigma)
         intensities /= sigma
-        intensities = 1. / (intensities + 1)
+        intensities = 1.0 / (intensities + 1)
         intensities[intensities <= 0] = sys.float_info.min
         return intensities
-    
+
     __skeleton_difference(graph, gradient_image, boundary_term_division, spacing)
-    
+
+
 def boundary_difference_division(graph, xxx_todo_changeme6):
     r"""
-    Boundary term processing adjacent voxels difference value using a division relationship. 
-    
+    Boundary term processing adjacent voxels difference value using a division relationship.
+
     An implementation of a boundary term, suitable to be used with the
     `~medpy.graphcut.generate.graph_from_voxels` function.
-    
+
     Finds all edges between all neighbours of the image and uses their difference in
     intensity values as edge weight.
-    
+
     The weights are normalized using an division function and a smoothing factor
     :math:`\sigma`. The :math:`\sigma` value has to be supplied manually, since its ideal settings
     differ greatly from application to application.
-    
+
     The weights between two neighbouring voxels :math:`(p, q)` is then computed as
-    
+
     .. math::
-    
+
         w(p,q) = \frac{1}{1 + \frac{|I_p - I_q|}{\sigma}}
-    
+
     , for which :math:`w(p, q) \in (0, 1]` holds true.
-    
+
     When the created edge weights should be weighted according to the slice distance,
     provide the list of slice thicknesses via the ``spacing`` parameter. Then all weights
     computed for the corresponding direction are divided by the respective slice
-    thickness. Set this parameter to `False` for equally weighted edges.     
-    
+    thickness. Set this parameter to `False` for equally weighted edges.
+
     Parameters
     ----------
     graph : GCGraph
         The graph to add the weights to.
     original_image : ndarray
         The original image.
     sigma : float
         The sigma parameter to use in the boundary term.
     spacing : sequence of float or False
         A sequence containing the slice spacing used for weighting the
         computed neighbourhood weight value for different dimensions. If
         `False`, no distance based weighting of the graph edges is performed.
-        
+
     Notes
     -----
     This function requires the original image to be passed along. That means that
     `~medpy.graphcut.generate.graph_from_voxels` has to be called with ``boundary_term_args`` set to the
     original image.
     """
     (original_image, sigma, spacing) = xxx_todo_changeme6
-    original_image = scipy.asarray(original_image)
-    
+    original_image = numpy.asarray(original_image)
+
     def boundary_term_division(intensities):
         """
         Implementation of a division boundary term computation over an array.
         """
         # apply 1 / (1  + x/sigma)
         intensities /= sigma
-        intensities = 1. / (intensities + 1)
+        intensities = 1.0 / (intensities + 1)
         intensities[intensities <= 0] = sys.float_info.min
         return intensities
-    
+
     __skeleton_difference(graph, original_image, boundary_term_division, spacing)
-    
+
+
 def boundary_maximum_power(graph, xxx_todo_changeme7):
     """
-    Boundary term processing adjacent voxels maximum value using a power relationship. 
-    
+    Boundary term processing adjacent voxels maximum value using a power relationship.
+
     An implementation of a boundary term, suitable to be used with the
     `~medpy.graphcut.generate.graph_from_voxels` function.
-    
+
     The same as `boundary_difference_power`, but working on the gradient image instead
     of the original. See there for details.
-    
+
     Parameters
     ----------
     graph : GCGraph
         The graph to add the weights to.
     gradient_image : ndarray
         The gradient image.
     sigma : float
         The sigma parameter to use in the boundary term.
     spacing : sequence of float or False
         A sequence containing the slice spacing used for weighting the
         computed neighbourhood weight value for different dimensions. If
         `False`, no distance based weighting of the graph edges is performed.
-        
+
     Notes
     -----
     This function requires the gradient image to be passed along. That means that
     `~medpy.graphcut.generate.graph_from_voxels` has to be called with ``boundary_term_args`` set to the
-    gradient image.    
+    gradient image.
     """
     (gradient_image, sigma, spacing) = xxx_todo_changeme7
-    gradient_image = scipy.asarray(gradient_image)
-    
+    gradient_image = numpy.asarray(gradient_image)
+
     def boundary_term_power(intensities):
         """
         Implementation of a power boundary term computation over an array.
         """
         # apply (1 / (1  + x))^sigma
-        intensities = 1. / (intensities + 1)
-        intensities = scipy.power(intensities, sigma)
+        intensities = 1.0 / (intensities + 1)
+        intensities = numpy.power(intensities, sigma)
         intensities[intensities <= 0] = sys.float_info.min
         return intensities
-    
-    __skeleton_maximum(graph, gradient_image, boundary_term_power, spacing)       
-    
-    
+
+    __skeleton_maximum(graph, gradient_image, boundary_term_power, spacing)
+
+
 def boundary_difference_power(graph, xxx_todo_changeme8):
     r"""
-    Boundary term processing adjacent voxels difference value using a power relationship. 
-    
+    Boundary term processing adjacent voxels difference value using a power relationship.
+
     An implementation of a boundary term, suitable to be used with the
     `~medpy.graphcut.generate.graph_from_voxels` function.
-    
+
     Finds all edges between all neighbours of the image and uses their difference in
     intensity values as edge weight.
-    
+
     The weights are normalized using an power function and a smoothing factor
     :math:`\sigma`. The :math:`\sigma` value has to be supplied manually, since its
     ideal settings differ greatly from application to application.
-    
+
     The weights between two neighbouring voxels :math:`(p, q)` is then computed as
-    
+
     .. math::
-    
+
         w(p,q) = \frac{1}{1 + |I_p - I_q|}^\sigma
-    
+
     , for which :math:`w(p, q) \in (0, 1]` holds true.
-    
+
     When the created edge weights should be weighted according to the slice distance,
     provide the list of slice thicknesses via the ``spacing`` parameter. Then all weights
     computed for the corresponding direction are divided by the respective slice
-    thickness. Set this parameter to `False` for equally weighted edges.     
-    
+    thickness. Set this parameter to `False` for equally weighted edges.
+
     Parameters
     ----------
     graph : GCGraph
         The graph to add the weights to.
     original_image : ndarray
         The original image.
     sigma : float
         The sigma parameter to use in the boundary term.
     spacing : sequence of float or False
         A sequence containing the slice spacing used for weighting the
         computed neighbourhood weight value for different dimensions. If
         `False`, no distance based weighting of the graph edges is performed.
-        
+
     Notes
     -----
     This function requires the original image to be passed along. That means that
     `~medpy.graphcut.generate.graph_from_voxels` has to be called with ``boundary_term_args`` set to the
     original image.
     """
     (original_image, sigma, spacing) = xxx_todo_changeme8
-    original_image = scipy.asarray(original_image)
-    
+    original_image = numpy.asarray(original_image)
+
     def boundary_term_power(intensities):
         """
         Implementation of a exponential boundary term computation over an array.
         """
         # apply (1 / (1  + x))^sigma
-        intensities = 1. / (intensities + 1)
-        intensities = scipy.power(intensities, sigma)
+        intensities = 1.0 / (intensities + 1)
+        intensities = numpy.power(intensities, sigma)
         intensities[intensities <= 0] = sys.float_info.min
         return intensities
-    
-    __skeleton_difference(graph, original_image, boundary_term_power, spacing)   
+
+    __skeleton_difference(graph, original_image, boundary_term_power, spacing)
+
 
 def __skeleton_maximum(graph, image, boundary_term, spacing):
     """
     A skeleton for the calculation of maximum intensity based boundary terms.
-    
+
     This function is equivalent to energy_voxel.__skeleton_difference(), but uses the
     maximum intensity rather than the intensity difference of neighbouring voxels. It is
     therefore suitable to be used with the gradient image, rather than the original
     image.
-    
+
     The computation of the edge weights follows
-    
+
     .. math::
-    
+
         w(p,q) = g(max(I_p, I_q))
-    
+
     ,where :math:`g(\cdot)` is the supplied boundary term function.
-    
+
     @param graph An initialized graph.GCGraph object
     @type graph.GCGraph
     @param image The image to compute on
     @type image numpy.ndarray
     @param boundary_term A function to compute the boundary term over an array of
                          maximum intensities
     @type boundary_term function
     @param spacing A sequence containing the slice spacing used for weighting the
                    computed neighbourhood weight value for different dimensions. If
                    False, no distance based weighting of the graph edges is performed.
-    @param spacing sequence | False    
-    
+    @param spacing sequence | False
+
     @see energy_voxel.__skeleton_difference() for more details.
     """
+
     def intensity_maximum(neighbour_one, neighbour_two):
         """
         Takes two voxel arrays constituting neighbours and computes the maximum between
         their intensities.
         """
-        return scipy.maximum(neighbour_one, neighbour_two)
-        
+        return numpy.maximum(neighbour_one, neighbour_two)
+
     __skeleton_base(graph, numpy.abs(image), boundary_term, intensity_maximum, spacing)
-    
+
 
 def __skeleton_difference(graph, image, boundary_term, spacing):
     """
     A skeleton for the calculation of intensity difference based boundary terms.
-    
+
     Iterates over the images dimensions and generates for each an array of absolute
     neighbouring voxel :math:`(p, q)` intensity differences :math:`|I_p, I_q|`. These are
     then passed to the supplied function :math:`g(\cdot)` for for boundary term
     computation. Finally the returned edge weights are added to the graph.
-    
+
     Formally for each edge :math:`(p, q)` of the image, their edge weight is computed as
-    
+
     .. math::
-    
+
         w(p,q) = g(|I_p - I_q|)
-    
+
     ,where :math:`g(\cdot)` is the supplied boundary term function.
-    
+
     The boundary term function has to take an array of intensity differences as only
     parameter and return an array of the same shape containing the edge weights. For the
     implemented function the condition :math:`g(\cdot)\in(0, 1]` must hold true, i.e., it
     has to be strictly positive with :math:`1` as the upper limit.
-    
-    @note the underlying neighbourhood connectivity is 4 for 2D, 6 for 3D, etc. 
-    
+
+    @note the underlying neighbourhood connectivity is 4 for 2D, 6 for 3D, etc.
+
     @note This function is able to work with images of arbitrary dimensions, but was only
     tested for 2D and 3D cases.
-    
+
     @param graph An initialized graph.GCGraph object
     @type graph.GCGraph
     @param image The image to compute on
     @type image numpy.ndarray
     @param boundary_term A function to compute the boundary term over an array of
                          absolute intensity differences
     @type boundary_term function
     @param spacing A sequence containing the slice spacing used for weighting the
                    computed neighbourhood weight value for different dimensions. If
                    False, no distance based weighting of the graph edges is performed.
-    @param spacing sequence | False    
+    @param spacing sequence | False
     """
+
     def intensity_difference(neighbour_one, neighbour_two):
         """
         Takes two voxel arrays constituting neighbours and computes the absolute
         intensity differences.
         """
-        return scipy.absolute(neighbour_one - neighbour_two)
-        
+        return numpy.absolute(neighbour_one - neighbour_two)
+
     __skeleton_base(graph, image, boundary_term, intensity_difference, spacing)
 
+
 def __skeleton_base(graph, image, boundary_term, neighbourhood_function, spacing):
     """
     Base of the skeleton for voxel based boundary term calculation.
-    
+
     This function holds the low level procedures shared by nearly all boundary terms.
-    
+
     @param graph An initialized graph.GCGraph object
     @type graph.GCGraph
     @param image The image containing the voxel intensity values
     @type image numpy.ndarray
     @param boundary_term A function to compute the boundary term over an array of
                            absolute intensity differences
     @type boundary_term function
@@ -605,49 +626,52 @@
                                   returned as a single array of the same shape
     @type neighbourhood_function function
     @param spacing A sequence containing the slice spacing used for weighting the
                    computed neighbourhood weight value for different dimensions. If
                    False, no distance based weighting of the graph edges is performed.
     @param spacing sequence | False
     """
-    image = scipy.asarray(image)
-    image = image.astype(scipy.float_)
+    image = numpy.asarray(image)
+    image = image.astype(float)
 
     # iterate over the image dimensions and for each create the appropriate edges and compute the associated weights
     for dim in range(image.ndim):
         # construct slice-objects for the current dimension
         slices_exclude_last = [slice(None)] * image.ndim
         slices_exclude_last[dim] = slice(-1)
         slices_exclude_first = [slice(None)] * image.ndim
         slices_exclude_first[dim] = slice(1, None)
         # compute difference between all layers in the current dimensions direction
-        neighbourhood_intensity_term = neighbourhood_function(image[slices_exclude_last], image[slices_exclude_first])
+        neighbourhood_intensity_term = neighbourhood_function(
+            image[tuple(slices_exclude_last)], image[tuple(slices_exclude_first)]
+        )
         # apply boundary term
         neighbourhood_intensity_term = boundary_term(neighbourhood_intensity_term)
         # compute key offset for relative key difference
         offset_key = [1 if i == dim else 0 for i in range(image.ndim)]
         offset = __flatten_index(offset_key, image.shape)
         # generate index offset function for index dependent offset
         idx_offset_divider = (image.shape[dim] - 1) * offset
         idx_offset = lambda x: int(x / idx_offset_divider) * offset
-        
+
         # weight the computed distanced in dimension dim by the corresponding slice spacing provided
-        if spacing: neighbourhood_intensity_term /= spacing[dim]
-        
+        if spacing:
+            neighbourhood_intensity_term /= spacing[dim]
+
         for key, value in enumerate(neighbourhood_intensity_term.ravel()):
             # apply index dependent offset
-            key += idx_offset(key) 
+            key += idx_offset(key)
             # add edges and set the weight
-            graph.set_nweight(key, key + offset, value, value)    
-    
+            graph.set_nweight(key, key + offset, value, value)
+
+
 def __flatten_index(pos, shape):
     """
     Takes a three dimensional index (x,y,z) and computes the index required to access the
     same element in the flattened version of the array.
     """
     res = 0
     acc = 1
     for pi, si in zip(reversed(pos), reversed(shape)):
         res += pi * acc
         acc *= si
     return res
-
```

### Comparing `MedPy-0.4.0/medpy/graphcut/wrapper.py` & `MedPy-0.5.0/medpy/graphcut/wrapper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,89 +1,96 @@
 # Copyright (C) 2013 Oskar Maier
-# 
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
-# 
+#
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
-# 
+#
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 # author Oskar Maier
 # version r0.1.0
 # since 2012-06-25
 # status Release
 
+import itertools
 
 # build-in modules
-import multiprocessing
-import itertools
 import math
+import multiprocessing
 
 # third-party modules
-import scipy
+import numpy
+
+from ..core import ArgumentError, Logger
+from ..filter import relabel, relabel_map
 
 # own modules
 from .energy_label import boundary_stawiaski
 from .generate import graph_from_labels
-from ..core.exceptions import ArgumentError
-from ..core.logger import Logger
-from ..filter import relabel, relabel_map
-try:
-    from functools import reduce
-except ImportError:
-    pass
+
 
 # code
-def split_marker(marker, fg_id = 1, bg_id = 2):
+def split_marker(marker, fg_id=1, bg_id=2):
     """
     Splits an integer marker image into two binary image containing the foreground and
     background markers respectively.
     All encountered 1's are hereby treated as foreground, all 2's as background, all 0's
     as neutral marker and all others are ignored.
     This behaviour can be changed by supplying the fg_id and/or bg_id parameters.
-    
+
     Parameters
     ----------
     marker : ndarray
         The marker image.
     fg_id : integer
         The value that should be treated as foreground.
     bg_id : integer
         The value that should be treated as background.
-    
+
     Returns
     -------
     fgmarkers, bgmarkers : nadarray
         The fore- and background markers as boolean images.
     """
-    img_marker = scipy.asarray(marker)
-    
-    img_fgmarker = scipy.zeros(img_marker.shape, scipy.bool_)
+    img_marker = numpy.asarray(marker)
+
+    img_fgmarker = numpy.zeros(img_marker.shape, numpy.bool_)
     img_fgmarker[img_marker == fg_id] = True
-    
-    img_bgmarker = scipy.zeros(img_marker.shape, scipy.bool_)
+
+    img_bgmarker = numpy.zeros(img_marker.shape, numpy.bool_)
     img_bgmarker[img_marker == bg_id] = True
-    
+
     return img_fgmarker, img_bgmarker
 
-def graphcut_split(graphcut_function, regions, gradient, foreground, background, minimal_edge_length = 100, overlap = 10, processes = None):
+
+def graphcut_split(
+    graphcut_function,
+    regions,
+    gradient,
+    foreground,
+    background,
+    minimal_edge_length=100,
+    overlap=10,
+    processes=None,
+):
     """
     Executes a graph cut by splitting the original volume into a number of sub-volumes of
     a minimal edge length. These are then processed in subprocesses.
-    
+
     This can be significantly faster than the traditional graph cuts, but should be
     used with, as it can lead to different results. To minimize this effect, the overlap
     parameter allows control over how much the respective sub-volumes should overlap.
-    
+
     Parameters
     ----------
     graphcut_function : function
         The graph cut to use (e.g. `graphcut_stawiaski`).
     regions : ndarray
         The regions image / label map.
     gradient : ndarray
@@ -95,168 +102,219 @@
     minimal_edge_length : integer
         The minimal edge length of the sub-volumes in voxels.
     overlap : integer
         The overlap (in voxels) between the generated sub-volumes.
     processes : integer or None
         The number of processes to run simultaneously, if not supplied, will be the same
         as the number of processors.
-        
+
     Returns
     -------
     segmentation : ndarray
         The graph-cut segmentation result as boolean array.
     """
     # initialize logger
     logger = Logger.getInstance()
-    
+
     # ensure that input images are scipy arrays
-    img_region = scipy.asarray(regions)
-    img_gradient = scipy.asarray(gradient)
-    img_fg = scipy.asarray(foreground, dtype=scipy.bool_)
-    img_bg = scipy.asarray(background, dtype=scipy.bool_)
-    
+    img_region = numpy.asarray(regions)
+    img_gradient = numpy.asarray(gradient)
+    img_fg = numpy.asarray(foreground, dtype=numpy.bool_)
+    img_bg = numpy.asarray(background, dtype=numpy.bool_)
+
     # ensure correctness of supplied images
-    if not (img_region.shape == img_gradient.shape == img_fg.shape == img_bg.shape): raise ArgumentError('All supplied images must be of the same shape.')    
-    
+    if not (img_region.shape == img_gradient.shape == img_fg.shape == img_bg.shape):
+        raise ArgumentError("All supplied images must be of the same shape.")
+
     # check and eventually enhance input parameters
-    if minimal_edge_length < 10: raise ArgumentError('A minimal edge length smaller than 10 is not supported.')
-    if overlap < 0: raise ArgumentError('A negative overlap is not supported.')
-    if overlap >= minimal_edge_length: raise ArgumentError('The overlap is not allowed to exceed the minimal edge length.')
-    
+    if minimal_edge_length < 10:
+        raise ArgumentError("A minimal edge length smaller than 10 is not supported.")
+    if overlap < 0:
+        raise ArgumentError("A negative overlap is not supported.")
+    if overlap >= minimal_edge_length:
+        raise ArgumentError(
+            "The overlap is not allowed to exceed the minimal edge length."
+        )
+
     # compute how to split the volumes into sub-volumes i.e. determine step-size for each image dimension
     shape = list(img_region.shape)
     steps = [x // minimal_edge_length for x in shape]
-    steps = [1 if 0 == x else x for x in steps] # replace zeros by ones
+    steps = [1 if 0 == x else x for x in steps]  # replace zeros by ones
     stepsizes = [math.ceil(x / y) for x, y in zip(shape, steps)]
-    logger.debug('Using a minimal edge length of {}, a sub-volume size of {} was determined from the shape {}, which means {} sub-volumes.'.format(minimal_edge_length, stepsizes, shape, reduce(lambda x, y: x*y, steps)))
-    
+    logger.debug(
+        "Using a minimal edge length of {}, a sub-volume size of {} was determined from the shape {}, which means {} sub-volumes.".format(
+            minimal_edge_length, stepsizes, shape, reduce(lambda x, y: x * y, steps)
+        )
+    )
+
     # control step-sizes to definitely cover the whole image
     covered_shape = [x * y for x, y in zip(steps, stepsizes)]
     for c, o in zip(covered_shape, shape):
-        if c < o: raise Exception("The computed sub-volumes do not cover the complete image!")
-            
+        if c < o:
+            raise Exception("The computed sub-volumes do not cover the complete image!")
+
     # iterate over the steps and extract subvolumes according to the stepsizes
-    slicer_steps = [list(range(0, int(step * stepsize), int(stepsize))) for step, stepsize in zip(steps, stepsizes)]
-    slicers = [[slice(_from, _from + _offset + overlap) for _from, _offset in zip(slicer_step, stepsizes)] for slicer_step in itertools.product(*slicer_steps)]
-    subvolumes_input = [(img_region[slicer],
-                         img_gradient[slicer],
-                         img_fg[slicer],
-                         img_bg[slicer]) for slicer in slicers]
-    
+    slicer_steps = [
+        list(range(0, int(step * stepsize), int(stepsize)))
+        for step, stepsize in zip(steps, stepsizes)
+    ]
+    slicers = [
+        [
+            slice(_from, _from + _offset + overlap)
+            for _from, _offset in zip(slicer_step, stepsizes)
+        ]
+        for slicer_step in itertools.product(*slicer_steps)
+    ]
+    subvolumes_input = [
+        (
+            img_region[tuple(slicer)],
+            img_gradient[tuple(slicer)],
+            img_fg[tuple(slicer)],
+            img_bg[tuple(slicer)],
+        )
+        for slicer in slicers
+    ]
+
     # execute the graph cuts and collect results
-    subvolumes_output = graphcut_subprocesses(graphcut_function, subvolumes_input, processes)
-    
+    subvolumes_output = graphcut_subprocesses(
+        graphcut_function, subvolumes_input, processes
+    )
+
     # put back data together
-    img_result = scipy.zeros(img_region.shape, dtype=scipy.bool_)
+    img_result = numpy.zeros(img_region.shape, dtype=numpy.bool_)
     for slicer, subvolume in zip(slicers, subvolumes_output):
         sslicer_antioverlap = [slice(None)] * img_result.ndim
-        
+
         # treat overlap area using logical-and (&)
         for dim in range(img_result.ndim):
-            if 0 == slicer[dim].start: continue
+            if 0 == slicer[dim].start:
+                continue
             sslicer_antioverlap[dim] = slice(overlap, None)
             sslicer_overlap = [slice(None)] * img_result.ndim
             sslicer_overlap[dim] = slice(0, overlap)
-            img_result[slicer][sslicer_overlap] = scipy.logical_and(img_result[slicer][sslicer_overlap], subvolume[sslicer_overlap])
-            
+            img_result[tuple(slicer)][tuple(sslicer_overlap)] = numpy.logical_and(
+                img_result[tuple(slicer)][tuple(sslicer_overlap)],
+                subvolume[tuple(sslicer_overlap)],
+            )
+
         # treat remainder through assignment
-        img_result[slicer][sslicer_antioverlap] = subvolume[sslicer_antioverlap]
-    
-    return img_result.astype(scipy.bool_)
-    
+        img_result[tuple(slicer)][tuple(sslicer_antioverlap)] = subvolume[
+            tuple(sslicer_antioverlap)
+        ]
+
+    return img_result.astype(numpy.bool_)
 
-def graphcut_subprocesses(graphcut_function, graphcut_arguments, processes = None):
+
+def graphcut_subprocesses(graphcut_function, graphcut_arguments, processes=None):
     """
     Executes multiple graph cuts in parallel.
     This can result in a significant speed-up.
-    
+
     Parameters
     ----------
     graphcut_function : function
         The graph cut to use (e.g. `graphcut_stawiaski`).
     graphcut_arguments : tuple
         List of arguments to pass to the respective subprocesses resp. the ``graphcut_function``.
     processes : integer or None
         The number of processes to run simultaneously, if not supplied, will be the same
         as the number of processors.
-        
+
     Returns
     -------
     segmentations : tuple of ndarray
         The graph-cut segmentation results as list of boolean arraya.
     """
     # initialize logger
     logger = Logger.getInstance()
-    
+
     # check and eventually enhance input parameters
-    if not processes: processes = multiprocessing.cpu_count()
-    if not int == type(processes) or processes <= 0: raise ArgumentError('The number processes can not be zero or negative.')
-    
-    logger.debug('Executing graph cuts in {} subprocesses.'.format(multiprocessing.cpu_count()))
-    
+    if not processes:
+        processes = multiprocessing.cpu_count()
+    if not int == type(processes) or processes <= 0:
+        raise ArgumentError("The number processes can not be zero or negative.")
+
+    logger.debug(
+        "Executing graph cuts in {} subprocesses.".format(multiprocessing.cpu_count())
+    )
+
     # creates subprocess pool and execute
     pool = multiprocessing.Pool(processes)
     results = pool.map(graphcut_function, graphcut_arguments)
-    
+
     return results
 
 
-def graphcut_stawiaski(regions, gradient = False, foreground = False, background = False):
+def graphcut_stawiaski(regions, gradient=False, foreground=False, background=False):
     """
     Executes a Stawiaski label graph cut.
-    
+
     Parameters
     ----------
     regions : ndarray
         The regions image / label map.
     gradient : ndarray
         The gradient image.
     foreground : ndarray
         The foreground markers.
     background : ndarray
         The background markers.
-        
+
     Returns
     -------
     segmentation : ndarray
         The graph-cut segmentation result as boolean array.
-        
+
     Raises
     ------
     ArgumentError
         When the supplied data is erroneous.
     """
     # initialize logger
     logger = Logger.getInstance()
-    
+
     # unpack images if required
     # !TODO: This is an ugly hack, especially since it can be seen inside the function definition
     # How to overcome this, since I can not use a wrapper function as the whole thing must be pickable
-    if not gradient and not foreground and not background: 
+    if not gradient and not foreground and not background:
         regions, gradient, foreground, background = regions
-    
+
     # ensure that input images are scipy arrays
-    img_region = scipy.asarray(regions)
-    img_gradient = scipy.asarray(gradient)
-    img_fg = scipy.asarray(foreground, dtype=scipy.bool_)
-    img_bg = scipy.asarray(background, dtype=scipy.bool_)
-    
+    img_region = numpy.asarray(regions)
+    img_gradient = numpy.asarray(gradient)
+    img_fg = numpy.asarray(foreground, dtype=numpy.bool_)
+    img_bg = numpy.asarray(background, dtype=numpy.bool_)
+
     # ensure correctness of supplied images
-    if not (img_region.shape == img_gradient.shape == img_fg.shape == img_bg.shape): raise ArgumentError('All supplied images must be of the same shape.')
+    if not (img_region.shape == img_gradient.shape == img_fg.shape == img_bg.shape):
+        raise ArgumentError("All supplied images must be of the same shape.")
 
     # recompute the label ids to start from id = 1
     img_region = relabel(img_region)
-    
+
     # generate graph
-    gcgraph = graph_from_labels(img_region, img_fg, img_bg, boundary_term = boundary_stawiaski, boundary_term_args = (img_gradient))
-    
+    gcgraph = graph_from_labels(
+        img_region,
+        img_fg,
+        img_bg,
+        boundary_term=boundary_stawiaski,
+        boundary_term_args=(img_gradient),
+    )
+
     # execute min-cut
-    maxflow = gcgraph.maxflow() # executes the cut and returns the maxflow value
-    
-    logger.debug('Graph-cut terminated successfully with maxflow of {}.'.format(maxflow))
-    
+    maxflow = gcgraph.maxflow()  # executes the cut and returns the maxflow value
+
+    logger.debug(
+        "Graph-cut terminated successfully with maxflow of {}.".format(maxflow)
+    )
+
     # apply results to the region image
-    mapping = [0] # no regions with id 1 exists in mapping, entry used as padding
-    mapping.extend([0 if gcgraph.termtype.SINK == gcgraph.what_segment(int(x) - 1) else 1 for x in scipy.unique(img_region)])
+    mapping = [0]  # no regions with id 1 exists in mapping, entry used as padding
+    mapping.extend(
+        [
+            0 if gcgraph.termtype.SINK == gcgraph.what_segment(int(x) - 1) else 1
+            for x in numpy.unique(img_region)
+        ]
+    )
     img_results = relabel_map(img_region, mapping)
-    
-    return img_results.astype(scipy.bool_)
+
+    return img_results.astype(numpy.bool_)
```

### Comparing `MedPy-0.4.0/medpy/graphcut/graph.py` & `MedPy-0.5.0/medpy/graphcut/graph.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,551 +1,596 @@
 # Copyright (C) 2013 Oskar Maier
-# 
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
-# 
+#
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
-# 
+#
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 # author Oskar Maier
 # version r0.1.2
 # since 2012-02-06
 # status Release
 
 # build-in modules
 
 # third-party modules
 
 # own modules
-from .maxflow import GraphDouble, GraphFloat
+from .maxflow import GraphDouble
+
 
 # code
 class Graph(object):
     r"""
     Represents a graph suitable for further processing with the graphcut package.
-    
+
     The graph contains nodes, edges (directed) between the nodes (n-edges), edges
     between two terminals (called source and sink) and the nodes (t-edges), and a
-    weight for each edge. 
-    
+    weight for each edge.
+
     Notes
     -----
     The node-ids used by the graph are assumed to start with 1 and be
     continuous. This is not actually checked, except when calling the
     inconsistent() method, so be careful.
     """
-    
+
     # @var __INT_16_BIT The maximum value of signed int 16bit.
     __INT_16_BIT = 32767
     # @var __UINT_16_BIT: The maximum value of unsigned int 16bit.
     __UINT_16_BIT = 65535
     # @var MAX The maximum value a weight can take.
     MAX = __UINT_16_BIT
-    
+
     def __init__(self):
         self.__nodes = 0
         self.__snodes = []
         self.__tnodes = []
         self.__nweights = {}
         self.__tweights = {}
-        
+
     def set_nodes(self, nodes):
         r"""
         Set the number of graph nodes (starting from node-id = 1),
         excluding sink and source.
-        
+
         Parameters
         ----------
         nodes : int
             Number of nodes
         """
         self.__nodes = int(nodes)
-        
+
     def set_source_nodes(self, source_nodes):
         r"""
         Set the source nodes and compute their t-weights.
-        
+
         Parameters
         ----------
         source_nodes : sequence of integers
             Declare the source nodes via their ids.
-        
+
         Notes
         -----
         It does not get checked if one of the supplied source-nodes already has
         a weight assigned (e.g. by passing it to `set_sink_nodes`). This can
         occur when the foreground- and background-markers cover the same region. In this
         case the order of setting the terminal nodes can affect the graph and therefore
         the graph-cut result.
         """
         self.__snodes = list(source_nodes)
-        
+
         # set the source-to-node weights (t-weights)
         for snode in self.__snodes:
-            self.__tweights[snode] = (self.MAX, 0) # (weight-to-source, weight-to-sink)
-            
+            self.__tweights[snode] = (self.MAX, 0)  # (weight-to-source, weight-to-sink)
+
     def set_sink_nodes(self, sink_nodes):
         r"""
         Set the sink nodes and compute their t-weights.
-        
+
         Parameters
         ----------
         sink_nodes : sequence of integers
             Declare the sink nodes via their ids.
-        
+
         Notes
         -----
         It does not get checked if one of the supplied sink-nodes already has
         a weight assigned (e.g. by passing it to set_source_nodes()). This can
         occur when the foreground- and background-markers cover the same region. In this
         case the order of setting the terminal nodes can affect the graph and therefore
         the graph-cut result.
         """
         self.__tnodes = list(sink_nodes)
-        
+
         # set the source-to-node weights (t-weights)
         for tnode in self.__tnodes:
-            self.__tweights[tnode] = (0, self.MAX) # (weight-to-source, weight-to-sink)
-            
+            self.__tweights[tnode] = (0, self.MAX)  # (weight-to-source, weight-to-sink)
+
     def set_nweights(self, nweights):
         r"""
         Sets all n-weights.
-        
+
         Parameters
         ----------
         nweights : dict
             A dictionary with (node-id, node-id) tuples as keys and (weight-a-to-b, weight-b-to-a) as values.
         """
         self.__nweights = nweights
-            
+
     def add_tweights(self, tweights):
         r"""
         Adds t-weights to the current collection of t-weights, overwriting already
         existing ones.
-        
+
         Parameters
         ----------
         tweights : dict
             A dictionary with node_ids as keys and (weight-to-source, weight-to-sink) tuples as values.
-        
+
         Notes
         -----
         The weights for nodes directly connected to either the source or the sink
         are best set using `set_source_nodes` or `set_sink_nodes` to ensure
         consistency of their maximum values.
         """
-        self.__tweights.update(tweights)    
-        
+        self.__tweights.update(tweights)
+
     def get_node_count(self):
         r"""
         Get the number of nodes.
-        
+
         Returns
         -------
         node_count : int
             The number of nodes (excluding sink and source).
         """
         return self.__nodes
-        
+
     def get_nodes(self):
         r"""
         Get the nodes.
-        
+
         Returns
         -------
         nodes : list
             All nodes as an ordered list.
         """
         return list(range(1, self.__nodes + 1))
-    
+
     def get_source_nodes(self):
         r"""
         Get the source nodes.
-        
+
         Returns
         -------
         source_nodes : list
             All nodes that are connected with the source as an unordered list (excluding sink and source).
         """
         return self.__snodes
-    
+
     def get_sink_nodes(self):
         r"""
         Get the sink nodes.
-        
+
         Returns
         -------
         sink_nodes : list
             All nodes that are connected with the sink as an unordered list (excluding sink and source).
         """
         return self.__tnodes
-    
+
     def get_edges(self):
         r"""
         Get the edges.
-        
+
         Returns
         -------
         edges : list
             All edges as ordered list of tuples (i.e. [(node_id1, node_id2), (..), ...].
         """
         return list(self.__nweights.keys())
-        
+
     def get_nweights(self):
         r"""
         Get the nweights.
-        
+
         Returns
         -------
         nweights : dict
             All n-weights (inter-node weights) as {edge-tuple: (weight, weight_reverersed)...} dict.
         """
         return self.__nweights
-        
+
     def get_tweights(self):
         r"""
         Get the tweights.
-        
+
         Returns
         -------
         tweights : dict
             All t-weights (terminal-node weights) as {node_id: (weight-source-node, weight-node-sink), ...} dict.
-        
+
         Notes
         -----
         Returns only the t-weights that have been set so far. For nodes with unset t-weight, no entry is returned.
         """
         return self.__tweights
-    
+
     def inconsistent(self):
         r"""
         Perform some consistency tests on the graph represented by this object
-        
+
         Returns
         -------
         consistent : bool or list
             False if consistent, else a list of inconsistency messages.
-        
+
         Notes
         -----
         This check is very time intensive and should not be executed on huge
         graphs, except for debugging purposes.
         """
         messages = []
         for node in list(self.__tweights.keys()):
-            if not node <= self.__nodes: messages.append("Node {} in t-weights but not in nodes.".format(node))
+            if not node <= self.__nodes:
+                messages.append("Node {} in t-weights but not in nodes.".format(node))
         for node in self.__snodes:
-            if not node <= self.__nodes: messages.append("Node {} in s-nodes but not in nodes.".format(node))
+            if not node <= self.__nodes:
+                messages.append("Node {} in s-nodes but not in nodes.".format(node))
         for node in self.__tnodes:
-            if not node <= self.__nodes: messages.append("Node {} in t-nodes but not in nodes.".format(node))
+            if not node <= self.__nodes:
+                messages.append("Node {} in t-nodes but not in nodes.".format(node))
         for e in list(self.__nweights.keys()):
-            if not e[0] <= self.__nodes: messages.append("Node {} in edge {} but not in nodes.".format(e[0], e))
-            if not e[1] <= self.__nodes: messages.append("Node {} in edge {} but not in nodes.".format(e[1], e))
-            if (e[1], e[0]) in iter(list(self.__nweights.keys())): messages.append("The reversed edges of {} is also in the n-weights.".format(e))
-                
-            
-        if 0 == len(messages): return False
-        else: return messages
-        
+            if not e[0] <= self.__nodes:
+                messages.append("Node {} in edge {} but not in nodes.".format(e[0], e))
+            if not e[1] <= self.__nodes:
+                messages.append("Node {} in edge {} but not in nodes.".format(e[1], e))
+            if (e[1], e[0]) in iter(list(self.__nweights.keys())):
+                messages.append(
+                    "The reversed edges of {} is also in the n-weights.".format(e)
+                )
+
+        if 0 == len(messages):
+            return False
+        else:
+            return messages
+
+
 class GCGraph:
     r"""
     A graph representation that works directly with the maxflow.GraphDouble graph as
     base. It is therefore less flexible as graph.Graph, but leads to lower memory
     requirements.
-    
+
     The graph contains nodes, edges (directed) between the nodes (n-edges), edges
     between two terminals (called source and sink) and the nodes (t-edges), and a
-    weight for each edge. 
-    
+    weight for each edge.
+
     Notes
     -----
     The node-ids used by the graph are assumed to start with 0 and be
     continuous. This is not actually checked, so be careful.
-    
+
     This wrapper tries to catch the most usual exception that can occur in the
     underlying C++ implementation and to convert them into catchable and meaningful
     error messages.
     """
     # @var __INT_16_BIT The maximum value of signed int 16bit.
     __INT_16_BIT = 32767
     # @var __UINT_16_BIT: The maximum value of unsigned int 16bit.
     __UINT_16_BIT = 65535
-    
+
     MAX = __UINT_16_BIT
     """The maximum value a terminal weight can take."""
-    
+
     def __init__(self, nodes, edges):
         r"""
         Initialize.
-        
+
         Parameters
         ----------
         nodes : int
             The number of nodes in the graph.
         edges : int
             The number of edges in the graph.
         """
         self.__graph = GraphDouble(nodes, edges)
         self.__graph.add_node(nodes)
         self.__nodes = nodes
         self.__edges = edges
-        
+
     def set_source_nodes(self, source_nodes):
         r"""
         Set multiple source nodes and compute their t-weights.
-        
+
         Parameters
         ----------
         source_nodes : sequence of integers
             Declare the source nodes via their ids.
-        
+
         Raises
         ------
-        ValueError 
+        ValueError
             If a passed node id does not refer to any node of the graph
             (i.e. it is either higher than the initially set number of
             nodes or lower than zero).
-                          
+
         Notes
         -----
         It does not get checked if one of the supplied source-nodes already has
         a weight assigned (e.g. by passing it to `set_sink_nodes`). This can
         occur when the foreground- and background-markers cover the same region. In this
         case the order of setting the terminal nodes can affect the graph and therefore
         the graph-cut result.
         """
         if max(source_nodes) >= self.__nodes or min(source_nodes) < 0:
-            raise ValueError('Invalid node id of {} or {}. Valid values are 0 to {}.'.format(max(source_nodes), min(source_nodes), self.__nodes - 1))
+            raise ValueError(
+                "Invalid node id of {} or {}. Valid values are 0 to {}.".format(
+                    max(source_nodes), min(source_nodes), self.__nodes - 1
+                )
+            )
         # set the source-to-node weights (t-weights)
         for snode in source_nodes:
-            self.__graph.add_tweights(int(snode), self.MAX, 0) # (weight-to-source, weight-to-sink)
-            
+            self.__graph.add_tweights(
+                int(snode), self.MAX, 0
+            )  # (weight-to-source, weight-to-sink)
+
     def set_sink_nodes(self, sink_nodes):
         r"""
         Set multiple sink nodes and compute their t-weights.
-        
+
         Parameters
         ----------
         sink_nodes : sequence of integers
             Declare the sink nodes via their ids.
-            
+
         Raises
         ------
-        ValueError 
+        ValueError
             If a passed node id does not refer to any node of the graph
             (i.e. it is either higher than the initially set number of
-            nodes or lower than zero).            
-        
+            nodes or lower than zero).
+
         Notes
         -----
         It does not get checked if one of the supplied sink-nodes already has
         a weight assigned (e.g. by passing it to `set_source_nodes`). This can
         occur when the foreground- and background-markers cover the same region. In this
         case the order of setting the terminal nodes can affect the graph and therefore
         the graph-cut result.
         """
         if max(sink_nodes) >= self.__nodes or min(sink_nodes) < 0:
-            raise ValueError('Invalid node id of {} or {}. Valid values are 0 to {}.'.format(max(sink_nodes), min(sink_nodes), self.__nodes - 1))
+            raise ValueError(
+                "Invalid node id of {} or {}. Valid values are 0 to {}.".format(
+                    max(sink_nodes), min(sink_nodes), self.__nodes - 1
+                )
+            )
         # set the node-to-sink weights (t-weights)
         for snode in sink_nodes:
-            self.__graph.add_tweights(int(snode), 0, self.MAX) # (weight-to-source, weight-to-sink)
-            
+            self.__graph.add_tweights(
+                int(snode), 0, self.MAX
+            )  # (weight-to-source, weight-to-sink)
+
     def set_nweight(self, node_from, node_to, weight_there, weight_back):
         r"""
         Set a single n-weight / edge-weight.
-        
+
         Parameters
         ----------
         node_from : int
             Node-id from the first node of the edge.
         node_to : int
             Node-id from the second node of the edge.
         weight_there : float
-            Weight from first to second node (>0). 
+            Weight from first to second node (>0).
         weight_back : float
             Weight from second to first node (>0).
-        
+
         Raises
         ------
         ValueError
             If a passed node id does not refer to any node of the graph
             (i.e. it is either higher than the initially set number of
             nodes or lower than zero).
         ValueError
             If the two node-ids of the edge are the same (graph cut does
             not allow self-edges).
         ValueError
             If one of the passed weights is <= 0.
-            
+
         Notes
         -----
         The object does not check if the number of supplied edges in total exceeds
         the number passed to the init-method. If this is the case, the underlying
         C++ implementation will double the memory, which is very unefficient.
-        
+
         The underlying C++ implementation allows zero weights, but these are highly
         undesirable for inter-node weights and therefore raise an error.
         """
         if node_from >= self.__nodes or node_from < 0:
-            raise ValueError('Invalid node id (node_from) of {}. Valid values are 0 to {}.'.format(node_from, self.__nodes - 1))
+            raise ValueError(
+                "Invalid node id (node_from) of {}. Valid values are 0 to {}.".format(
+                    node_from, self.__nodes - 1
+                )
+            )
         elif node_to >= self.__nodes or node_to < 0:
-            raise ValueError('Invalid node id (node_to) of {}. Valid values are 0 to {}.'.format(node_to, self.__nodes - 1))
+            raise ValueError(
+                "Invalid node id (node_to) of {}. Valid values are 0 to {}.".format(
+                    node_to, self.__nodes - 1
+                )
+            )
         elif node_from == node_to:
-            raise ValueError('The node_from ({}) can not be equal to the node_to ({}) (self-connections are forbidden in graph cuts).'.format(node_from, node_to))
+            raise ValueError(
+                "The node_from ({}) can not be equal to the node_to ({}) (self-connections are forbidden in graph cuts).".format(
+                    node_from, node_to
+                )
+            )
         elif weight_there <= 0 or weight_back <= 0:
-            raise ValueError('Negative or zero weights are not allowed.')
-        self.__graph.sum_edge(int(node_from), int(node_to), float(weight_there), float(weight_back))
-            
+            raise ValueError("Negative or zero weights are not allowed.")
+        self.__graph.sum_edge(
+            int(node_from), int(node_to), float(weight_there), float(weight_back)
+        )
+
     def set_nweights(self, nweights):
         r"""
         Set multiple n-weights / edge-weights.
-        
+
         Parameters
         ----------
         nweights : dict
             A dictionary with (node-id, node-id) tuples as keys and (weight-a-to-b, weight-b-to-a) as values.
-        
+
         Notes
         -----
         The object does not check if the number of supplied edges in total exceeds
         the number passed to the init-method. If this is the case, the underlying
         C++ implementation will double the memory, which is very inefficient.
-              
+
         See `set_nweight` for raised errors.
         """
         for edge, weight in list(nweights.items()):
             self.set_nweight(edge[0], edge[1], weight[0], weight[1])
-            
+
     def set_tweight(self, node, weight_source, weight_sink):
         r"""
         Set a single t-weight / terminal-weight.
-        
+
         Parameters
         ----------
         node : int
             Node-id for which to set the terminal weights.
         weight_source : float
             Weight to source terminal.
         weight_sink : float
             Weight to sink terminal.
-        
+
         Raises
         ------
         ValueError
             If a passed node id does not refer to any node of the graph
             (i.e. it is either higher than the initially set number of
             nodes or lower than zero).
-            
+
         Notes
-        -----        
+        -----
         The object does not check if the number of supplied edges in total exceeds
         the number passed to the init-method. If this is the case, the underlying
         C++ implementation will double the memory, which is very inefficient.
-              
+
         Terminal weights can be zero or negative.
         """
         if node >= self.__nodes or node < 0:
-            raise ValueError('Invalid node id of {}. Valid values are 0 to {}.'.format(node, self.__nodes - 1))
-        self.__graph.add_tweights(int(node), float(weight_source), float(weight_sink)) # (weight-to-source, weight-to-sink)
-            
+            raise ValueError(
+                "Invalid node id of {}. Valid values are 0 to {}.".format(
+                    node, self.__nodes - 1
+                )
+            )
+        self.__graph.add_tweights(
+            int(node), float(weight_source), float(weight_sink)
+        )  # (weight-to-source, weight-to-sink)
+
     def set_tweights(self, tweights):
         r"""
         Set multiple t-weights to the current collection of t-weights, overwriting
         already existing ones.
-        
+
         Parameters
         ----------
         tweights : dict
             A dictionary with node_ids as keys and (weight-to-source, weight-to-sink) tuples as values.
-        
+
         Raises
         ------
         ValueError
             If a passed node id does not refer to any node of the graph
             (i.e. it is either higher than the initially set number of
-            nodes or lower than zero).        
-        
+            nodes or lower than zero).
+
         Notes
         -----
         Since this method overrides already existing t-weights, it is strongly
         recommended to run `set_source_nodes` and `set_sink_nodes` after the
         last call to this method.
-        
+
         The weights for nodes directly connected to either the source or the sink
         are best set using `set_source_nodes` or `set_sink_nodes` to ensure
         consistency of their maximum values.
-        """        
+        """
         for node, weight in list(tweights.items()):
-            self.set_tweight(node, weight[0], weight[1]) # (weight-to-source, weight-to-sink)
-            
+            self.set_tweight(
+                node, weight[0], weight[1]
+            )  # (weight-to-source, weight-to-sink)
+
     def set_tweights_all(self, tweights):
         r"""
         Set all t-weights at once.
-        
+
         Parameters
         ----------
         tweights : iterable
             Containing a pair of numeric values for each of the graphs nodes.
-        
+
         Notes
         -----
         Since this method overrides already existing t-weights, it is strongly
         recommended to run `set_source_nodes` and `set_sink_nodes` after the
         last call to this method.
-        
+
         The weights for nodes directly connected to either the source or the sink
         are best set using `set_source_nodes` or `set_sink_nodes` to ensure
         consistency of their maximum values.
         """
         for node, (twsource, twsink) in enumerate(tweights):
-            self.set_tweight(node, twsource, twsink) # source = FG, sink = BG
-        
+            self.set_tweight(node, twsource, twsink)  # source = FG, sink = BG
+
     def get_graph(self):
         r"""
         Get the C++ graph.
-        
+
         Returns
         -------
         graph : maxflow.GraphDouble
             The underlying maxflow.GraphDouble C++ implementation of the graph.
         """
         return self.__graph
-        
+
     def get_node_count(self):
         r"""
         Get the number of nodes.
-        
+
         Returns
         -------
         node_count : int
             The number of nodes (excluding sink and source).
         """
         return self.__nodes
-        
+
     def get_nodes(self):
         r"""
         Get the nodes.
-        
+
         Returns
         -------
         nodes : list
             All nodes as an ordered list (starting from 0).
         """
         return list(range(0, self.__nodes))
-    
+
     def get_edge_count(self):
         r"""
         Get the number of edges.
-        
+
         Returns
         -------
         edge_count : int
             The number of edges.
         """
         return self.__edges
```

### Comparing `MedPy-0.4.0/medpy/features/__init__.py` & `MedPy-0.5.0/medpy/features/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 =================================================================
 Image feature extraction and manipulation (:mod:`medpy.features`)
 =================================================================
 .. currentmodule:: medpy.features
 
 This package contains various functions for feature extraction and
 manipulation in medical images.
- 
+
 Intensity :mod:`medpy.features.intensity`
 =========================================
 Functions to extracts intensity based features. Ready to be
 manipulated with :mod:`medpy.features.utilities` and used in
 `scikit-learn <http://scikit-learn.org/>`_.
 
 .. module:: medpy.features.intensity
 .. autosummary::
     :toctree: generated/
-    
+
     intensities
     centerdistance
     centerdistance_xdminus1
     indices
     shifted_mean_gauss
     mask_distance
     local_mean_gauss
@@ -32,20 +32,20 @@
 Feature representation
 ----------------------
 Features can be one or more dimensional and are kept in the following
 structures::
 
     ===== | == == =====
     s1    | s2 s3 [...]
-    f1.1  | 
-    f1.2  | 
-    f2.1  | 
-    f3.1  | 
-    f3.2  | 
-    [...] | 
+    f1.1  |
+    f1.2  |
+    f2.1  |
+    f3.1  |
+    f3.2  |
+    [...] |
     ===== | == == =====
 
 , where each column sX denotes a single sample (voxel) and each row
 a features element e.g. f1 is constitutes a 2-dimensional features
 and occupies therefore two rows, while f2 is a single element
 features with a single row. Entries of this array are of type float.
 These feature representation forms are processable by the
@@ -64,33 +64,33 @@
 Utilities :mod:`medpy.feature.utilities`
 ========================================
 A number of utilities to manipulate feature vectors created with `medpy.features.intensity`.
 
 .. module:: medpy.features.utilities
 .. autosummary::
     :toctree: generated/
-    
+
     normalize
     normalize_with_model
     append
     join
-    
+
 Histogram :mod:`medy.features.histogram`
 ========================================
 Functions to create various kinds of fuzzy histograms with the fuzzy_histogram function.
 
 .. module:: medpy.features.histogram
 .. autosummary::
     :toctree: generated/
-    
+
     fuzzy_histogram
     triangular_membership
     trapezoid_membership
     gaussian_membership
-    sigmoidal_difference_membership    
+    sigmoidal_difference_membership
 
 Available membership functions
 ------------------------------
 function (string to pass to `membership` argument of fuzzy_histogram)
 
 * triangular_membership (triangular)
 * trapezoid_membership (trapezoid)
@@ -105,17 +105,17 @@
 fuzzy membership function.
 More clearly the smoothness term determines how much the function reaches into the
 adjunct bins.
 
 An example of the smoothness parameter::
 
                   ____________ ________ ____________ ________ ____________
-                 /          / \        / \       /  \        / \          \ 
-                /          /   \      /   \     /    \      /   \          \ 
-               /          /     \    /     \   /      \    /     \          \ 
+                 /          / \\        / \\       /  \\        / \\          \\
+                /          /   \\      /   \\     /    \\      /   \\          \\
+               /          /     \\    /     \\   /      \\    /     \\          \\
     ---|----------|----------|----------|----------|----------|----------|----------|----
             x-3        x-2        x-1        x          x+1        x+2        x+3
                   |-nbh      |          |crisp bin |          |      +nbh|
 
 The considered value v is associated with the bin x using crisp (i.e. standard)
 histograms. For fuzzy histograms with a smoothness of 2, its membership value for
 the bins x-smoothness (x-2) until x+smoothness (x+2) is computed. While it also
@@ -126,40 +126,73 @@
 Boundary effect / the guarantee parameter
 -----------------------------------------
 Values near the left and right border of the histogram might
 not contribute with a full value of 1 to the histogram, as part of their contribution
 lies outside of the histogram range. To avoid this affect (which can be quite strong
 for histograms with few bins and a height smoothness term), set 'guarantee' to True.
 The histogram size is then selected to be (left_side - smoothness * bin_width till
-right_side + smoothness * bin_width) and therefore neglect all boundary effects.    
+right_side + smoothness * bin_width) and therefore neglect all boundary effects.
 
 Plots of the membership functions can e.g. be found at http://www.atp.ruhr-uni-bochum.de/rt1/syscontrol/node117.html .
-    
+
 """
 
 # Copyright (C) 2013 Oskar Maier
-# 
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
-# 
+#
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
-# 
+#
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-# import all functions/methods/classes into the module
-from .histogram import fuzzy_histogram, triangular_membership, trapezoid_membership, \
-                       gaussian_membership, sigmoidal_difference_membership
-from .intensity import centerdistance, centerdistance_xdminus1, gaussian_gradient_magnitude, \
-                       hemispheric_difference, indices, intensities, local_histogram, local_mean_gauss, \
-                       median, shifted_mean_gauss, mask_distance
-from .utilities import append, join, normalize, normalize_with_model
-
-# import all sub-modules in the __all__ variable
-__all__ = [s for s in dir() if not s.startswith('_')]
-
-
+from .histogram import fuzzy_histogram as fuzzy_histogram
+from .histogram import gaussian_membership as gaussian_membership
+from .histogram import (
+    sigmoidal_difference_membership as sigmoidal_difference_membership,
+)
+from .histogram import trapezoid_membership as trapezoid_membership
+from .histogram import triangular_membership as triangular_membership
+from .intensity import centerdistance as centerdistance
+from .intensity import centerdistance_xdminus1 as centerdistance_xdminus1
+from .intensity import gaussian_gradient_magnitude as gaussian_gradient_magnitude
+from .intensity import hemispheric_difference as hemispheric_difference
+from .intensity import indices as indices
+from .intensity import intensities as intensities
+from .intensity import local_histogram as local_histogram
+from .intensity import local_mean_gauss as local_mean_gauss
+from .intensity import mask_distance as mask_distance
+from .intensity import median as median
+from .intensity import shifted_mean_gauss as shifted_mean_gauss
+from .utilities import append as append
+from .utilities import join as join
+from .utilities import normalize as normalize
+from .utilities import normalize_with_model as normalize_with_model
+
+__all__ = [
+    "fuzzy_histogram",
+    "triangular_membership",
+    "trapezoid_membership",
+    "gaussian_membership",
+    "sigmoidal_difference_membership",
+    "centerdistance",
+    "centerdistance_xdminus1",
+    "gaussian_gradient_magnitude",
+    "hemispheric_difference",
+    "indices",
+    "intensities",
+    "local_histogram",
+    "local_mean_gauss",
+    "median",
+    "shifted_mean_gauss",
+    "mask_distance",
+    "append",
+    "join",
+    "normalize",
+    "normalize_with_model",
+]
```

### Comparing `MedPy-0.4.0/medpy/features/histogram.py` & `MedPy-0.5.0/medpy/features/histogram.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,56 @@
 # Copyright (C) 2013 Oskar Maier
-# 
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
-# 
+#
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
-# 
+#
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 # author Oskar Maier
 # version r0.1.3
 # since 2012-03-01
 # status Release
 
 # build-in modules
 import math
 
 # third-party modules
+import numpy
 import scipy.stats
 
 # own modules
 
 # constants
 # the available membership functions for fuzzy histogram calculation
-__MBS = ['triangular', 'trapezoid', 'gaussian', 'sigmoid']
+__MBS = ["triangular", "trapezoid", "gaussian", "sigmoid"]
+
 
 # code
-def fuzzy_histogram(a, bins=10, range=None, normed=False, membership='triangular', smoothness=None, guarantee=False):
+def fuzzy_histogram(
+    a,
+    bins=10,
+    range=None,
+    normed=False,
+    membership="triangular",
+    smoothness=None,
+    guarantee=False,
+):
     r"""Compute a fuzzy histogram.
     The percentage of a value's membership in a bin is computed using the selected
     membership function. This functions stays as near as possible to the `numpy.histogram`
     behaviour.
-    
+
     Parameters
     ----------
     a : array_like
         Input data; The histogram is computed over the flattened array (with ravel()).
     bins : int
         The number of equal-width bins in the given range (10, by default).
     range : (float, float)
@@ -55,419 +65,444 @@
         description for available options.
     smoothness : float
         The smoothness of the fuzzy function; See package
         description and the membership functions for more details.
     guarantee : bool
         Guarantee that all values contribute equally to the histogram; when this value is
         set, the range term is ignored; see package descriptions for details.
-    
+
     Returns
     -------
     hist : array
         The values of the histogram. See normed and weights for a description of the possible semantics.
     bin_edges : array of dtype float
         Return the bin edges (length(hist)+1).
-    
+
     Notes
     -----
     See package description for more details on the usage.
-    
+
     Examples
     --------
     >>> import numpy as np
     >>> from medpy.features import fuzzy_histogram
     >>> a = np.asarray([1,2,3,3.2,3.4,3.5,7.5,7.6,7.8,8,9,10])
     >>> np.histogram(a, bins=4)
     (array([4, 2, 2, 4]), array([  1.  ,   3.25,   5.5 ,   7.75,  10.  ]))
     >>> fuzzy_histogram(a, bins=4)
     (array([ 3.4       ,  2.04444444,  2.04444444,  3.4       ]), array([  1.  ,   3.25,   5.5 ,   7.75,  10.  ]))
     >>> fuzzy_histogram(a, bins=4, membership='sigmoid')
     (array([ 3.34304743,  2.15613626,  2.15613626,  3.34304743]), array([  1.  ,   3.25,   5.5 ,   7.75,  10.  ]))
-    
+
     """
     # check and prepare parameters
-    a = scipy.asarray(a).ravel()
-    if None == range: range = (a.min(), a.max())
-    if range[1] <= range[0]: raise AttributeError('max must be larger than min in range parameter.')
-    if not int == type(bins): raise AttributeError('bins must an integer.')
-    if bins <= 0: raise AttributeError('bins must greater than zero.')
-    if membership not in __MBS: raise AttributeError('Unknown type: {}. Must be one of {}.'.format(membership, __MBS))
-    if not None == smoothness and smoothness <= 0.0: raise AttributeError('smoothness must be greater than zero.')
-    
+    a = numpy.asarray(a).ravel()
+    if range is None:
+        range = (a.min(), a.max())
+    if range[1] <= range[0]:
+        raise AttributeError("max must be larger than min in range parameter.")
+    if not int == type(bins):
+        raise AttributeError("bins must an integer.")
+    if bins <= 0:
+        raise AttributeError("bins must greater than zero.")
+    if membership not in __MBS:
+        raise AttributeError(
+            "Unknown type: {}. Must be one of {}.".format(membership, __MBS)
+        )
+    if smoothness is not None and smoothness <= 0.0:
+        raise AttributeError("smoothness must be greater than zero.")
+
     # set default smoothness values
-    if None == smoothness:
-        smoothness = 0.25 if 'trapezoid' == membership else 0.5
-    
-    if not guarantee: # compute bin distribution in no guarantee case
+    if smoothness is None:
+        smoothness = 0.25 if "trapezoid" == membership else 0.5
+
+    if not guarantee:  # compute bin distribution in no guarantee case
         binw = (range[1] - range[0]) / float(bins)
-        bins = scipy.asarray([i * binw + range[0] for i in scipy.arange(bins + 1)])
-    else: # compute bin distribution for guarantee case
+        bins = numpy.asarray([i * binw + range[0] for i in numpy.arange(bins + 1)])
+    else:  # compute bin distribution for guarantee case
         bins_core = bins - 2 * int(math.ceil(smoothness))
-        if bins_core <= 0: raise AttributeError('bins to few to guarantee removing boundary effect.')
+        if bins_core <= 0:
+            raise AttributeError("bins to few to guarantee removing boundary effect.")
         binw = (range[1] - range[0]) / float(bins_core)
-        range = (range[0] - int(math.ceil(smoothness)) * binw, range[1] + int(math.ceil(smoothness)) * binw)
-        bins = scipy.asarray([i * binw + range[0] for i in scipy.arange(bins + 1)])
-    
+        range = (
+            range[0] - int(math.ceil(smoothness)) * binw,
+            range[1] + int(math.ceil(smoothness)) * binw,
+        )
+        bins = numpy.asarray([i * binw + range[0] for i in numpy.arange(bins + 1)])
+
     # create membership function (centered at 0)
-    if 'triangular' == membership:
+    if "triangular" == membership:
         membership = triangular_membership(0, binw, smoothness)
-    elif 'trapezoid' == membership:
+    elif "trapezoid" == membership:
         membership = trapezoid_membership(0, binw, smoothness)
-    elif 'gaussian' == membership:
+    elif "gaussian" == membership:
         membership = gaussian_membership(0, binw, smoothness)
-    elif 'sigmoid' == membership:
+    elif "sigmoid" == membership:
         membership = sigmoidal_difference_membership(0, binw, smoothness)
 
     # compute histogram i.e. memberships of values across neighbourhood (determined by smoothness)
     neighbourhood = int(math.ceil(smoothness))
     l = len(bins) - 2
-    histogram = scipy.zeros(l + 1)
+    histogram = numpy.zeros(l + 1)
     m = range[0]
-    for v in a: # for each value
+    for v in a:  # for each value
         idx = min(l, int((v - m) / binw))
-        for i in scipy.arange(max(0, idx - neighbourhood), min(l + 1, idx + neighbourhood + 1)): # for crips bin neighbourhood
+        for i in numpy.arange(
+            max(0, idx - neighbourhood), min(l + 1, idx + neighbourhood + 1)
+        ):  # for crips bin neighbourhood
             start = bins[i]
-            histogram[i] += membership(v - start - 0.5 * binw) # adjust v for evaluation on zero-centered membership function
+            histogram[i] += membership(
+                v - start - 0.5 * binw
+            )  # adjust v for evaluation on zero-centered membership function
 
     # normalize
-    if normed: histogram /= float(sum(histogram))
-    
+    if normed:
+        histogram /= float(sum(histogram))
+
     return histogram, bins
-    
+
+
 # //////////////////// #
 # Membership functions #
 # //////////////////// #
-# see http://www.atp.ruhr-uni-bochum.de/rt1/syscontrol/node117.html for graphs    
+# see http://www.atp.ruhr-uni-bochum.de/rt1/syscontrol/node117.html for graphs
+
 
-def triangular_membership(bin_center, bin_width, smoothness = 0.5):
+def triangular_membership(bin_center, bin_width, smoothness=0.5):
     r"""
     Create a triangular membership function for a fuzzy histogram bin.
-    
+
     Parameters
     ----------
     bin_center : number
         The center of the bin of which to compute the membership function.
     bin_width : number
         The width of a single bin (all expected to be of equal width).
     smoothness : number, optional
         The smoothness of the function; determines the neighbourhood affected.
         See below and `fuzzy_histogram` for a more detailed explanation
-    
+
     Returns
     -------
     triangular_membership : function
         A triangular membership function centered on the bin.
-    
+
     Notes
     -----
     For the triangular function the smoothness factor has to be 0.5. Lower values
     are accepted, but then the function assumes the shape of the trapezium membership
     function. Higher values lead to an exception.
-    
+
     The triangular membership function is defined as
 
     .. math::
-        
+
         \mu_{\triangle}(x) =
           \left\{
             \begin{array}{ll}
               0, & x<a, x>c\\
               \frac{x-a}{b-a}, & a\leq x\leq b \\
               \frac{c-x}{c-b}, & b<x\leq c\\
             \end{array}
           \right.
 
     where :math:`a` is the left border, :math:`c` the right border and :math:`b` the center of the triangular
     function. The height of the triangle is chosen such, that all values contribute with
     exactly one.
-    
+
     The standard triangular function (:math:`smoothness = 0.5`) is displayed in the following
     figure
-    
+
     .. .. image:: images/triangular_01.png
-    
+
     "Triangular functions (1)"
-    
+
     where the bin width is :math:`2` with centers at :math:`-2`, :math:`0` and :math:`2`.
     """
-    if smoothness > 0.5: raise AttributeError('the triangular/trapezium membership functions supports only smoothnesses between 1/10 and 1/2.')
-    if smoothness < 0.5: return trapezoid_membership(bin_center, bin_width, smoothness)
-    
+    if smoothness > 0.5:
+        raise AttributeError(
+            "the triangular/trapezium membership functions supports only smoothnesses between 1/10 and 1/2."
+        )
+    if smoothness < 0.5:
+        return trapezoid_membership(bin_center, bin_width, smoothness)
+
     a = bin_center - bin_width
     b = float(bin_center)
     c = bin_center + bin_width
-    
+
     def fun(x):
-        if x < a or x > c: return 0
-        elif x <= b: return (x-a)/(b-a)
-        else: return (c-x)/(c-b)
+        if x < a or x > c:
+            return 0
+        elif x <= b:
+            return (x - a) / (b - a)
+        else:
+            return (c - x) / (c - b)
+
     return fun
-    
+
+
 def trapezoid_membership(bin_center, bin_width, smoothness):
     r"""Create a trapezium membership function for a fuzzy histogram bin.
-    
+
     Parameters
     ----------
     bin_center : number
         The center of the bin of which to compute the membership function.
     bin_width : number
         The width of a single bin (all expected to be of equal width).
     smoothness : number, optional
         The smoothness of the function; determines the neighbourhood affected.
         See below and `fuzzy_histogram` for a more detailed explanation
-        
+
     Returns
     -------
     trapezoid_membership : function
         A trapezoidal membership function centered on the bin.
-    
+
     Notes
     -----
     For the trapezium function the smoothness factor can be between >0.0 and <0.5.
     Higher values are excepted, but then the function assumes the shape of the triangular
     membership function. A value of 0.0 would make the histogram behave like a crisp one.
-    
+
     The trapezium membership function is defined as
-    
+
     .. math::
-    
+
         \mu_{trapez}(x) =
           \left\{
             \begin{array}{ll}
               0, & x<a, x>d\\
               \frac{x-a}{b-a}, & a\leq x\leq b \\
               1, & b<x<c\\
               \frac{d-x}{d-c}, & c\leq x\leq d\\
             \end{array}
           \right.
-    
+
     where :math:`a` is the left lower border, :math:`b` the left upper border, :math:`c` the right upper border
     and :math:`d` the right lower border of the trapezium.
-    
+
     A smoothness term of 0.1 makes the trapezium function reach by :math:`0.1 * bin\_width` into
     the areas of the adjunct bins, as can be observed in the following figure
-    
+
     .. .. image:: images/trapezium_02.png
-    
+
     "Trapezium functions (1)"
-    
+
     where the bin width is 2 with centers at -2, 0 and 2.
-    
+
     Increasing the smoothness term toward 0.5, the function starts to resemble the
     triangular membership function, which in fact it becomes for any :math:`smoothness >= 0.5`.
-    The behavior can be observed in the following graph with :math:`smoothness=0.4` 
-    
+    The behavior can be observed in the following graph with :math:`smoothness=0.4`
+
     .. .. image:: images/trapezium_01.png
-    
+
     "Trapezium functions (2)"
-    
+
     Lowering the smoothness toward 0.0, on the other hand, leads the trapezium function
     to behave more and more like a crisp histogram membership, which in fact it becomes
     at a smoothness of 0.0. The following figure, where the smoothness term is near zero,
     illustrates this behaviour
-    
+
     .. .. image:: images/trapezium_03.png
-    
+
     "Trapezium functions (3)"
-    
+
     """
     # special case of high smoothness
-    if smoothness < 1./10: raise AttributeError('the triangular/trapezium membership functions supports only smoothnesses between 1/10 and 1/2.')
-    if smoothness >= 0.5: return triangular_membership(bin_center, bin_width, smoothness)
+    if smoothness < 1.0 / 10:
+        raise AttributeError(
+            "the triangular/trapezium membership functions supports only smoothnesses between 1/10 and 1/2."
+        )
+    if smoothness >= 0.5:
+        return triangular_membership(bin_center, bin_width, smoothness)
 
-    a = bin_center - (smoothness + 0.5) * bin_width 
+    a = bin_center - (smoothness + 0.5) * bin_width
     b = bin_center - (0.5 - smoothness) * bin_width
     c = bin_center + (0.5 - smoothness) * bin_width
     d = bin_center + (smoothness + 0.5) * bin_width
-     
+
     def fun(x):
-        if x < a or x > d: return 0
-        elif x <= b: return (x-a)/float(b-a)
-        elif x <= c: return 1
-        else: return (d-x)/float(d-c)
+        if x < a or x > d:
+            return 0
+        elif x <= b:
+            return (x - a) / float(b - a)
+        elif x <= c:
+            return 1
+        else:
+            return (d - x) / float(d - c)
+
     return fun
 
+
 def gaussian_membership(bin_center, bin_width, smoothness):
     r"""Create a gaussian membership function for a fuzzy histogram bin.
-    
+
     Parameters
     ----------
     bin_center : number
         The center of the bin of which to compute the membership function.
     bin_width : number
         The width of a single bin (all expected to be of equal width).
     smoothness : number, optional
         The smoothness of the function; determines the neighbourhood affected.
         See below and `fuzzy_histogram` for a more detailed explanation
-        
+
     Returns
     -------
     gaussian_membership : function
         The cumulative density function of the desired gaussian.
 
     Notes
     -----
     Since the gaussian membership function is infinite, it is
     not actually true that it does not contribute to bins outside of the neighbourhood
     range. But the contribution is so marginal (:math:`eps <= 0.001` per value) that it can be
     safely ignored.
-    
+
     The gaussian membership function is defined as
-    
+
     .. math::
-    
+
         \mu_{gauss}(x) = \frac{1}{\sigma\sqrt{2\pi}} e^{-\frac{(x-\zeta)^2}{2\sigma^2}}
 
     Since the gaussian distributions can not be formed to sum up to one at each point of
     the x-axis, their cumulative density functions (CDF) are used instead. For more
     details on CDF see http://en.wikipedia.org/wiki/Normal_distribution .
-    
+
     The gaussian and therefore the CDF are centered above the requested value instead of
     the bin center. Then the CDF value for the left side of the bin is subtracted from
     the CDF value returned for the right side. The result is the integral under the
     gaussian with :math:`\mu/\zeta = value` with the bin-sides as the integral borders.
-    
+
     This approach might seem a little bit unintuitive, but is the best possible for
     gaussian membership functions. The following graph gives a graphical example of the
     computation of each values bin membership
-    
-    .. .. image:: images/gaussian_01.png 
-    
+
+    .. .. image:: images/gaussian_01.png
+
     "Trapezium functions (1)"
-    
+
     where the bin_width is 1, one bin between each of the x tics (e.g. [-1, 0], [0, 1],
     etc.). The value which membership should be computed is marked by a yellow bar at
     :math:`x = 0.3`. Its membership in each bin is defined by the integral under the gaussian
     centered at the value (i.e. 0.3). The purple area therefore defines its membership in
     the [-2,-1] bin, the red area its membership in the [-1,0] bin, etc.
     Since the gaussian is guaranteed to have an infinite integral of 1, the some of the
     contributions of a value to all bins is one.
 
     For computation the function normalizes all values to a bin_width of 1, which can
     introduce marginal rounding errors.
     """
-    if smoothness > 10 or smoothness < 1./10: raise AttributeError('the gaussian membership function supports only smoothnesses between 1/10 and 5.')
-    
+    if smoothness > 10 or smoothness < 1.0 / 10:
+        raise AttributeError(
+            "the gaussian membership function supports only smoothnesses between 1/10 and 5."
+        )
+
     bin_width = float(bin_width)
     bin_center = bin_center / bin_width
     start = bin_center - 0.5
     end = bin_center + 0.5
     sigma = _gaussian_membership_sigma(smoothness)
 
     def fun(x):
-        return scipy.stats.norm.cdf(end, x / bin_width, sigma) - scipy.stats.norm.cdf(start, x / bin_width, sigma) # x, mu, sigma
-    
+        return scipy.stats.norm.cdf(end, x / bin_width, sigma) - scipy.stats.norm.cdf(
+            start, x / bin_width, sigma
+        )  # x, mu, sigma
+
     return fun
 
-def _gaussian_membership_sigma(smoothness, eps = 0.0005): # 275us @ smothness=10
+
+def _gaussian_membership_sigma(smoothness, eps=0.0005):  # 275us @ smothness=10
     r"""Compute the sigma required for a gaussian, such that in a neighbourhood of
     smoothness the maximum error is 'eps'.
     The error is here the difference between the clipped integral and one.
     """
     error = 0
     deltas = [0.1, 0.01, 0.001, 0.0001]
     sigma = smoothness * 0.3
-    point = -1. * (smoothness + 0.5)
+    point = -1.0 * (smoothness + 0.5)
     for delta in deltas:
         while error < eps:
             sigma += delta
-            error = scipy.stats.norm.cdf(0.5, point, sigma) - scipy.stats.norm.cdf(-0.5, point, sigma) # x, mu, sigma
+            error = scipy.stats.norm.cdf(0.5, point, sigma) - scipy.stats.norm.cdf(
+                -0.5, point, sigma
+            )  # x, mu, sigma
         sigma -= delta
     return sigma
 
+
 def sigmoidal_difference_membership(bin_center, bin_width, smoothness):
     r"""Create the difference of two sigmoids as membership function for a fuzzy histogram bin.
-    
+
     Parameters
     ----------
     bin_center : number
         The center of the bin of which to compute the membership function.
     bin_width : number
         The width of a single bin (all expected to be of equal width).
     smoothness : number, optional
         The smoothness of the function; determines the neighbourhood affected.
         See below and `fuzzy_histogram` for a more detailed explanation
-        
+
     Returns
     -------
     sigmoidal_difference_membership : function
         A sigmoidal difference membership function centered on the bin.
-    
+
     Notes
     -----
     Since the sigmoidal membership function is infinite, it is
     not actually true that it does not contribute to bins outside of the neighbourhood
     range. But the contribution is so marginal (eps <= 0.001 per value) that it can be
     safely ignored.
-    
+
     The sigmoidal membership function is defined as
-    
+
     .. math::
-        
+
         \mu_{sigmoid}(x) = \left[1+e^{-\alpha_1 (x-\zeta_1)}\right]^{-1} - \left[1+e^{-\alpha_2 (x-\zeta_2)}\right]^{-1}
 
     where :math:`\alpha_1 = \alpha_2 = \alpha` is computed throught the smoothness term
     and :math:`\zeta_1` and :math:`\zeta_2` constitute the left resp. right borders of the bin.
-    
+
     The following figure shows three sigmoidal membership functions for bins at the
     centers -2, -0 and 2 with a bin width of 2 and a smoothness of 2:
-    
+
     .. .. image:: images/sigmoid_01.png
-    
+
     "Sigmoidal functions (1)"
-    
+
     The central (green) membership functions extends to its up till the second bin
     (centered around -4) and the same to the right (until the bin centered around +4).
     Therefore all values from -5 to +5 are considered for membership in this bin. Values
     out of this range would only contribute marginally to this bin.
     Furthermore it is inteligable that the sum of all membership functions at each point
     is equal to 1, therefore all values are equally represented (i.e. contribute with 1
     to the overall histogram).
-    
+
     The influence of the smoothness term can be observed in the following figure:
-    
+
     .. .. image:: images/sigmoid_02.png
-    
+
     "Sigmoidal functions (2)"
-    
+
     Here smoothness has been chosen to be 1. The green function therefore extends just
     into the directly adjunct bins to its left and right.
-    
+
     """
-    if smoothness > 10 or smoothness < 1./10: raise AttributeError('the sigmoidal membership function supports only smoothnesses between 1/10 and 10.')
-    
+    if smoothness > 10 or smoothness < 1.0 / 10:
+        raise AttributeError(
+            "the sigmoidal membership function supports only smoothnesses between 1/10 and 10."
+        )
+
     # compute the alpha that will give a contribution to the next bins right and left
-    alpha_nbh1 = 8. / bin_width # experimental value
-    # compute the alpha that results in the desired smoothness level 
+    alpha_nbh1 = 8.0 / bin_width  # experimental value
+    # compute the alpha that results in the desired smoothness level
     alpha = alpha_nbh1 / smoothness
-    
+
     def fun(x):
-        sigmoid1 = 1 + math.exp(-1. * alpha * (x - (bin_center - 0.5 * bin_width)))
-        sigmoid2 = 1 + math.exp(-1. * alpha * (x - (bin_center + 0.5 * bin_width)))
+        sigmoid1 = 1 + math.exp(-1.0 * alpha * (x - (bin_center - 0.5 * bin_width)))
+        sigmoid2 = 1 + math.exp(-1.0 * alpha * (x - (bin_center + 0.5 * bin_width)))
         return math.pow(sigmoid1, -1) - math.pow(sigmoid2, -1)
+
     return fun
-    
-#def generalized_bell_membership(alpha, beta, zeta):
-#    """
-#    Create a generalized bell function as membership function for a fuzzy histogram bin.
-#    
-#    @param alpha controls the width of the plateau
-#    @param beta controls the width of the base
-#    @param zeta the center of the function
-#    
-#    Recommended values are:
-#        - alpha: bin-width/2
-#        - beta: bin-width/2
-#        - zeta: bin center
-#    
-#    The bell membership function is defined as    
-#    \f[
-#     \mu_{bell}(x) = \left[1+\left|\frac{x-\zeta}{\alpha}\right|^{2\beta}\right]^{-1}
-#    \f]
-#    """
-#    def fun(x):
-#        try:
-#            return math.pow(1 + math.pow(abs((x - zeta)/float(alpha)), 2. * beta), -1)
-#        except Exception as e:
-#            print x, zeta, alpha, beta
-#            raise e
-#    return fun
```

### Comparing `MedPy-0.4.0/medpy/features/intensity.py` & `MedPy-0.5.0/medpy/features/intensity.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,423 +1,482 @@
 # Copyright (C) 2013 Oskar Maier
-# 
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
-# 
+#
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
-# 
+#
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 # author Oskar Maier
 # version r0.3.3
 # since 2013-08-24
 # status Release
 
 # build-in modules
 
 # third-party modules
 import numpy
-from scipy.ndimage.filters import gaussian_filter, median_filter
-from scipy.ndimage.filters import gaussian_gradient_magnitude as scipy_gaussian_gradient_magnitude
-from scipy.interpolate.interpolate import interp1d
-from scipy.ndimage.morphology import distance_transform_edt
+from scipy.interpolate import interp1d
+from scipy.ndimage import distance_transform_edt, gaussian_filter
+from scipy.ndimage import (
+    gaussian_gradient_magnitude as scipy_gaussian_gradient_magnitude,
+)
+from scipy.ndimage import median_filter
 from scipy.ndimage._ni_support import _get_output
 
-# own modules
-from .utilities import join
 from ..core import ArgumentError
 from ..filter import sum_filter
 
+# own modules
+from .utilities import join
+
 # constants
 
-def intensities(image, mask = slice(None)):
+
+def intensities(image, mask=slice(None)):
     r"""Takes a simple or multi-spectral image and returns its voxel-wise intensities.
     A multi-spectral image must be supplied as a list or tuple of its spectra.
-    
+
     Optionally a binary mask can be supplied to select the voxels for which the feature
     should be extracted.
-    
+
     Parameters
     ----------
-    image : array_like or list/tuple of array_like 
+    image : array_like or list/tuple of array_like
         A single image or a list/tuple of images (for multi-spectral case).
     mask : array_like
         A binary mask for the image.
-    
+
     Returns
     -------
     intensities : ndarray
         The images intensities.
     """
     return _extract_feature(_extract_intensities, image, mask)
 
-def centerdistance(image, voxelspacing = None, mask = slice(None)):
+
+def centerdistance(image, voxelspacing=None, mask=slice(None)):
     r"""
     Takes a simple or multi-spectral image and returns its voxel-wise center distance in
     mm. A multi-spectral image must be supplied as a list or tuple of its spectra.
-    
+
     Optionally a binary mask can be supplied to select the voxels for which the feature
     should be extracted.
-    
+
     The center distance is the exact euclidean distance in mm of each voxels center to
     the central point of the overal image volume.
-    
+
     Note that this feature is independent of the actual image content, but depends
     solely on its shape. Therefore always a one-dimensional feature is returned, even if
-    a multi-spectral image has been supplied. 
+    a multi-spectral image has been supplied.
 
     Parameters
     ----------
-    image : array_like or list/tuple of array_like 
+    image : array_like or list/tuple of array_like
         A single image or a list/tuple of images (for multi-spectral case).
     voxelspacing : sequence of floats
         The side-length of each voxel.
     mask : array_like
         A binary mask for the image.
 
     Returns
     -------
     centerdistance : ndarray
         The distance of each voxel to the images center.
-        
+
     See Also
     --------
     centerdistance_xdminus1
-    
+
     """
-    if type(image) == tuple or type(image) == list:
+    if type(image) is tuple or type(image) is list:
         image = image[0]
-        
-    return _extract_feature(_extract_centerdistance, image, mask, voxelspacing = voxelspacing)
 
-def centerdistance_xdminus1(image, dim, voxelspacing = None, mask = slice(None)):
+    return _extract_feature(
+        _extract_centerdistance, image, mask, voxelspacing=voxelspacing
+    )
+
+
+def centerdistance_xdminus1(image, dim, voxelspacing=None, mask=slice(None)):
     r"""
     Implementation of `centerdistance` that allows to compute sub-volume wise
     centerdistances.
-    
+
     The same notes as for `centerdistance` apply.
-    
+
     Parameters
     ----------
-    image : array_like or list/tuple of array_like 
+    image : array_like or list/tuple of array_like
         A single image or a list/tuple of images (for multi-spectral case).
     dim : int or sequence of ints
         The dimension or dimensions along which to cut the image into sub-volumes.
     voxelspacing : sequence of floats
         The side-length of each voxel.
     mask : array_like
         A binary mask for the image.
-    
+
     Returns
     -------
     centerdistance_xdminus1 : ndarray
         The distance of each voxel to the images center in the supplied dimensions.
-    
+
     Raises
     ------
     ArgumentError
         If a invalid dim index of number of dim indices were supplied
 
     Examples
     --------
     Considering a 3D medical image we want to compute the axial slice-wise
     centerdistances instead of the ones over the complete image volume. Assuming that
     the third image dimension corresponds to the axial axes of the image, we call
-        
+
     >>> centerdistance_xdminus1(image, 2)
-    
+
     Note that the centerdistance of each slice will be equal.
 
     """
     # pre-process arguments
-    if type(image) == tuple or type(image) == list:
+    if type(image) is tuple or type(image) is list:
         image = image[0]
-    
+
     if type(dim) is int:
         dims = [dim]
     else:
         dims = list(dim)
-        
+
     # check arguments
     if len(dims) >= image.ndim - 1:
-        raise ArgumentError('Applying a sub-volume extraction of depth {} on a image of dimensionality {} would lead to invalid images of dimensionality <= 1.'.format(len(dims), image.ndim))
+        raise ArgumentError(
+            "Applying a sub-volume extraction of depth {} on a image of dimensionality {} would lead to invalid images of dimensionality <= 1.".format(
+                len(dims), image.ndim
+            )
+        )
     for dim in dims:
         if dim >= image.ndim:
-            raise ArgumentError('Invalid dimension index {} supplied for image(s) of shape {}.'.format(dim, image.shape))
-    
+            raise ArgumentError(
+                "Invalid dimension index {} supplied for image(s) of shape {}.".format(
+                    dim, image.shape
+                )
+            )
+
     # extract desired sub-volume
     slicer = [slice(None)] * image.ndim
-    for dim in dims: slicer[dim] = slice(1)
-    subvolume = numpy.squeeze(image[slicer])
-    
+    for dim in dims:
+        slicer[dim] = slice(1)
+    subvolume = numpy.squeeze(image[tuple(slicer)])
+
     # compute centerdistance for sub-volume and reshape to original sub-volume shape (note that normalization and mask are not passed on in this step)
     o = centerdistance(subvolume, voxelspacing).reshape(subvolume.shape)
-    
+
     # re-establish original shape by copying the resulting array multiple times
     for dim in sorted(dims):
         o = numpy.asarray([o] * image.shape[dim])
         o = numpy.rollaxis(o, 0, dim + 1)
-        
+
     # extract intensities / centerdistance values, applying normalization and mask in this step
     return intensities(o, mask)
 
-def indices(image, voxelspacing = None, mask = slice(None)):
+
+def indices(image, voxelspacing=None, mask=slice(None)):
     r"""
     Takes an image and returns the voxels ndim-indices as voxel-wise feature. The voxel
     spacing is taken into account, i.e. the indices are not array indices, but millimeter
     indices.
-    
+
     This is a multi-element feature where each element corresponds to one of the images
     axes, e.g. x, y, z, ...
-    
+
     Parameters
     ----------
-    image : array_like or list/tuple of array_like 
+    image : array_like or list/tuple of array_like
         A single image or a list/tuple of images (for multi-spectral case).
     voxelspacing : sequence of floats
         The side-length of each voxel.
     mask : array_like
-        A binary mask for the image. 
-    
+        A binary mask for the image.
+
     Returns
     -------
     indices : ndarray
         Each voxels ndimensional index.
 
     Notes
     -----
     This feature is independent of the actual image content, but depends
     solely on its shape. Therefore always a one-dimensional feature is returned, even if
     a multi-spectral image has been supplied.
-    
+
     """
-    if type(image) == tuple or type(image) == list:
+    if type(image) is tuple or type(image) is list:
         image = image[0]
-        
+
     if not type(mask) is slice:
-        mask = numpy.array(mask, copy=False, dtype=numpy.bool)
-        
+        mask = numpy.array(mask, copy=False, dtype=numpy.bool_)
+
     if voxelspacing is None:
-        voxelspacing = [1.] * image.ndim
+        voxelspacing = [1.0] * image.ndim
+
+    return join(
+        *[
+            a[mask].ravel() * vs
+            for a, vs in zip(numpy.indices(image.shape), voxelspacing)
+        ]
+    )
 
-    return join(*[a[mask].ravel() * vs for a, vs in zip(numpy.indices(image.shape), voxelspacing)])
-    
-def shifted_mean_gauss(image, offset = None, sigma = 5, voxelspacing = None, mask = slice(None)):
+
+def shifted_mean_gauss(
+    image, offset=None, sigma=5, voxelspacing=None, mask=slice(None)
+):
     r"""
     The approximate mean over a small region at an offset from each voxel.
-    
+
     Functions like `local_mean_gauss`, but instead of computing the average over a small
     patch around the current voxel, the region is centered at an offset away. Can be used
     to use a distant regions average as feature for a voxel.
-    
+
     Parameters
     ----------
-    image : array_like or list/tuple of array_like 
+    image : array_like or list/tuple of array_like
         A single image or a list/tuple of images (for multi-spectral case).
     offset : sequence of ints
         At this offset in voxels of the current position the region is placed.
     sigma : number or sequence of numbers
         Standard deviation for Gaussian kernel. The standard deviations of the
         Gaussian filter are given for each axis as a sequence, or as a single number,
         in which case it is equal for all axes. Note that the voxel spacing of the image
         is taken into account, the given values are treated as mm.
     voxelspacing : sequence of floats
         The side-length of each voxel.
     mask : array_like
-        A binary mask for the image. 
-    
+        A binary mask for the image.
+
     Returns
     -------
     shifted_mean_gauss : ndarray
         The weighted mean intensities over a region at offset away from each voxel.
-    
+
     See also
     --------
     local_mean_gauss
-    
+
     """
-    return _extract_feature(_extract_shifted_mean_gauss, image, mask, offset = offset, sigma = sigma, voxelspacing = voxelspacing)
-    
-def mask_distance(image, voxelspacing = None, mask = slice(None)):
+    return _extract_feature(
+        _extract_shifted_mean_gauss,
+        image,
+        mask,
+        offset=offset,
+        sigma=sigma,
+        voxelspacing=voxelspacing,
+    )
+
+
+def mask_distance(image, voxelspacing=None, mask=slice(None)):
     r"""
     Computes the distance of each point under the mask to the mask border taking the
     voxel-spacing into account.
-    
+
     Note that this feature is independent of the actual image content, but depends
     solely the mask image. Therefore always a one-dimensional feature is returned,
     even if a multi-spectral image has been supplied.
-    
+
     If no mask has been supplied, the distances to the image borders are returned.
 
     Parameters
     ----------
-    image : array_like or list/tuple of array_like 
+    image : array_like or list/tuple of array_like
         A single image or a list/tuple of images (for multi-spectral case).
     voxelspacing : sequence of floats
         The side-length of each voxel.
     mask : array_like
-        A binary mask for the image.     
-    
+        A binary mask for the image.
+
     Returns
     -------
     mask_distance : ndarray
         Each voxels distance to the mask borders.
 
     """
-    if type(image) == tuple or type(image) == list:
+    if type(image) is tuple or type(image) is list:
         image = image[0]
-        
-    return _extract_mask_distance(image, mask = mask, voxelspacing = voxelspacing)
-    
-def local_mean_gauss(image, sigma = 5, voxelspacing = None, mask = slice(None)):
+
+    return _extract_mask_distance(image, mask=mask, voxelspacing=voxelspacing)
+
+
+def local_mean_gauss(image, sigma=5, voxelspacing=None, mask=slice(None)):
     r"""
     Takes a simple or multi-spectral image and returns the approximate mean over a small
     region around each voxel. A multi-spectral image must be supplied as a list or tuple
     of its spectra.
-    
+
     Optionally a binary mask can be supplied to select the voxels for which the feature
     should be extracted.
-    
+
     For this feature a Gaussian smoothing filter is applied to the image / each spectrum
     and then the resulting intensity values returned. Another name for this function
     would be weighted local mean.
-    
+
     Parameters
     ----------
-    image : array_like or list/tuple of array_like 
+    image : array_like or list/tuple of array_like
         A single image or a list/tuple of images (for multi-spectral case).
     sigma : number or sequence of numbers
         Standard deviation for Gaussian kernel. The standard deviations of the
         Gaussian filter are given for each axis as a sequence, or as a single number,
         in which case it is equal for all axes. Note that the voxel spacing of the image
-        is taken into account, the given values are treated as mm.        
+        is taken into account, the given values are treated as mm.
     voxelspacing : sequence of floats
         The side-length of each voxel.
     mask : array_like
-        A binary mask for the image.       
-    
-    
+        A binary mask for the image.
+
+
     Returns
     -------
     local_mean_gauss : ndarray
         The weighted mean intensities over a region around each voxel.
-    
+
     """
-    return _extract_feature(_extract_local_mean_gauss, image, mask, sigma = sigma, voxelspacing = voxelspacing)
+    return _extract_feature(
+        _extract_local_mean_gauss, image, mask, sigma=sigma, voxelspacing=voxelspacing
+    )
+
 
-def gaussian_gradient_magnitude(image, sigma = 5, voxelspacing = None, mask = slice(None)):
+def gaussian_gradient_magnitude(image, sigma=5, voxelspacing=None, mask=slice(None)):
     r"""
     Computes the gradient magnitude (edge-detection) of the supplied image using gaussian
     derivates and returns the intensity values.
-    
+
     Optionally a binary mask can be supplied to select the voxels for which the feature
     should be extracted.
-    
+
     Parameters
     ----------
-    image : array_like or list/tuple of array_like 
+    image : array_like or list/tuple of array_like
         A single image or a list/tuple of images (for multi-spectral case).
     sigma : number or sequence of numbers
         Standard deviation for Gaussian kernel. The standard deviations of the
         Gaussian filter are given for each axis as a sequence, or as a single number,
         in which case it is equal for all axes. Note that the voxel spacing of the image
-        is taken into account, the given values are treated as mm.        
+        is taken into account, the given values are treated as mm.
     voxelspacing : sequence of floats
         The side-length of each voxel.
     mask : array_like
-        A binary mask for the image.          
+        A binary mask for the image.
 
     Returns
     -------
     gaussian_gradient_magnitude : ndarray
         The gaussian gradient magnitude of the supplied image.
-    
+
     """
-    return _extract_feature(_extract_gaussian_gradient_magnitude, image, mask, sigma = sigma, voxelspacing = voxelspacing)
+    return _extract_feature(
+        _extract_gaussian_gradient_magnitude,
+        image,
+        mask,
+        sigma=sigma,
+        voxelspacing=voxelspacing,
+    )
 
-def median(image, size = 5, voxelspacing = None, mask = slice(None)):
+
+def median(image, size=5, voxelspacing=None, mask=slice(None)):
     """
     Computes the multi-dimensional median filter and returns the resulting values per
     voxel.
-    
+
     Optionally a binary mask can be supplied to select the voxels for which the feature
     should be extracted.
-    
+
     Parameters
     ----------
-    image : array_like or list/tuple of array_like 
+    image : array_like or list/tuple of array_like
         A single image or a list/tuple of images (for multi-spectral case).
     size : number or sequence of numbers
         Size of the structuring element. Can be given given for each axis as a sequence,
         or as a single number, in which case it is equal for all axes. Note that the
         voxel spacing of the image is taken into account, the given values are treated
         as mm.
     voxelspacing : sequence of floats
         The side-length of each voxel.
     mask : array_like
         A binary mask for the image.
-        
+
     Returns
     -------
     median : ndarray
         Multi-dimesnional median filtered version of the input images.
-    
-    """
-    return _extract_feature(_extract_median, image, mask, size = size, voxelspacing = voxelspacing)
 
-def local_histogram(image, bins=19, rang="image", cutoffp=(0.0, 100.0), size=None, footprint=None, output=None, mode="ignore", origin=0, mask=slice(None)):
+    """
+    return _extract_feature(
+        _extract_median, image, mask, size=size, voxelspacing=voxelspacing
+    )
+
+
+def local_histogram(
+    image,
+    bins=19,
+    rang="image",
+    cutoffp=(0.0, 100.0),
+    size=None,
+    footprint=None,
+    output=None,
+    mode="ignore",
+    origin=0,
+    mask=slice(None),
+):
     r"""
     Computes multi-dimensional histograms over a region around each voxel.
-    
+
     Supply an image and (optionally) a mask and get the local histogram of local
     neighbourhoods around each voxel. These neighbourhoods are cubic with a sidelength of
     size in voxels or, when a shape instead of an integer is passed to size, of this
     shape.
-    
+
     If not argument is passed to output, the returned array will be of dtype float.
-    
+
     Voxels along the image border are treated as defined by mode. The possible values are
     the same as for scipy.ndimage filter without the ''constant'' mode. Instead "ignore"
     is the default and additional mode, which sets that the area outside of the image are
     ignored when computing the histogram.
-    
+
     When a mask is supplied, the local histogram is extracted only for the voxels where
     the mask is True. But voxels from outside the mask can be incorporated in the
     compuation of the histograms.
-    
+
     The range of the histograms can be set via the rang argument. The 'image' keyword can
     be supplied, to use the same range for all local histograms, extracted from the images
     max and min intensity values. Alternatively, an own range can be supplied in the form
     of a tuple of two numbers. Values outside the range of the histogram are ignored.
-    
+
     Setting a proper range is important, as all voxels that lie outside of the range are
     ignored i.e. do not contribute to the histograms as if they would not exists. Some
     of the local histograms can therefore be constructed from less than the expected
     number of voxels.
-    
+
     Taking the histogram range from the whole image is sensitive to outliers. Supplying
     percentile values to the cutoffp argument, these can be filtered out when computing
     the range. This keyword is ignored if rang is not set to 'image'.
-    
+
     Setting the rang to None causes local ranges to be used i.e. the ranges of the
     histograms are computed only over the local area covered by them and are hence
     not comparable. This behaviour should normally not be taken.
-    
+
     The local histograms are normalized by dividing them through the number of elements
     in the bins.
-    
+
     Parameters
     ----------
-    image : array_like or list/tuple of array_like 
+    image : array_like or list/tuple of array_like
         A single image or a list/tuple of images (for multi-spectral case).
     bins : integer
         The number of histogram bins.
     rang : 'image' or tuple of numbers or None
         The range of the histograms, can be supplied manually, set to 'image' to use
         global or set to None to use local ranges.
     cutoffp : tuple of numbers
@@ -438,54 +497,73 @@
         The ``output`` parameter passes an array in which to store the filter output.
     mode : {'reflect', 'ignore', 'nearest', 'mirror', 'wrap'}
         The ``mode`` parameter determines how the array borders are handled. Default is 'ignore'
     origin : number
         The ``origin`` parameter controls the placement of the filter. Default 0.
     mask : array_like
         A binary mask for the image.
-        
+
     Returns
     -------
     local_histogram : ndarray
         The bin values of the local histograms for each voxel as a multi-dimensional image.
 
-    """    
-    return _extract_feature(_extract_local_histogram, image, mask, bins=bins, rang=rang, cutoffp=cutoffp, size=size, footprint=footprint, output=output, mode=mode, origin=origin)
-
-
-def hemispheric_difference(image, sigma_active = 7, sigma_reference = 7, cut_plane = 0, voxelspacing = None, mask = slice(None)):
+    """
+    return _extract_feature(
+        _extract_local_histogram,
+        image,
+        mask,
+        bins=bins,
+        rang=rang,
+        cutoffp=cutoffp,
+        size=size,
+        footprint=footprint,
+        output=output,
+        mode=mode,
+        origin=origin,
+    )
+
+
+def hemispheric_difference(
+    image,
+    sigma_active=7,
+    sigma_reference=7,
+    cut_plane=0,
+    voxelspacing=None,
+    mask=slice(None),
+):
     r"""
     Computes the hemispheric intensity difference between the brain hemispheres of an brain image.
-    
+
     Cuts the image along the middle of the supplied cut-plane. This results in two
     images, each containing one of the brains hemispheres.
-    
+
     For each of these two, the following steps are applied:
-    
+
     1. One image is marked as active image
     2. The other hemisphere image is marked as reference image
     3. The reference image is fliped along the cut_plane
     4. A gaussian smoothing is applied to the active image with the supplied sigma
     5. A gaussian smoothing is applied to the reference image with the supplied sigma
     6. The reference image is substracted from the active image, resulting in the
        difference image for the active hemisphere
-    
+
     Finally, the two resulting difference images are stitched back together, forming a
     hemispheric difference image of the same size as the original.
-    
+
     Note that the supplied gaussian kernel sizes (sigmas) are sensitive to the images
     voxel spacing.
-    
+
     If the number of slices along the cut-plane is odd, the central slice is
     interpolated from the two hemisphere difference images when stitching them back
     together.
-    
+
     Parameters
     ----------
-    image : array_like or list/tuple of array_like 
+    image : array_like or list/tuple of array_like
         A single image or a list/tuple of images (for multi-spectral case).
     sigma_active : number or sequence of numbers
         Standard deviation for Gaussian kernel of the active image. The standard
         deviations of the Gaussian filter are given for each axis as a sequence, or as a
         single number, in which case it is equal for all axes. Note that the voxel
         spacing of the image is taken into account, the given values are treated
         as mm.
@@ -497,285 +575,375 @@
         as mm.
     cut_plane : integer
         he axes along which to cut. This is usually the coronal plane.
     voxelspacing : sequence of floats
         The side-length of each voxel.
     mask : array_like
         A binary mask for the image.
-        
+
     Returns
     -------
     hemispheric_difference : ndarray
         The intensity differences between the locally smoothed hemispheres of the image.
         The resulting voxel value's magnitude denotes symmetrical its asymmetry. The
         direction is revealed by the sign. That means that the resulting image will be
-        symmetric in absolute values, but differ in sign. 
+        symmetric in absolute values, but differ in sign.
 
     Raises
     ------
     ArgumentError
         If the supplied cut-plane dimension is invalid.
 
-    """   
-    return _extract_feature(_extract_hemispheric_difference, image, mask, sigma_active = sigma_active, sigma_reference = sigma_reference, cut_plane = cut_plane, voxelspacing = voxelspacing)
-
-
-def _extract_hemispheric_difference(image, mask = slice(None), sigma_active = 7, sigma_reference = 7, cut_plane = 0, voxelspacing = None):
+    """
+    return _extract_feature(
+        _extract_hemispheric_difference,
+        image,
+        mask,
+        sigma_active=sigma_active,
+        sigma_reference=sigma_reference,
+        cut_plane=cut_plane,
+        voxelspacing=voxelspacing,
+    )
+
+
+def _extract_hemispheric_difference(
+    image,
+    mask=slice(None),
+    sigma_active=7,
+    sigma_reference=7,
+    cut_plane=0,
+    voxelspacing=None,
+):
     """
     Internal, single-image version of `hemispheric_difference`.
     """
     # constants
-    INTERPOLATION_RANGE = int(10) # how many neighbouring values to take into account when interpolating the medial longitudinal fissure slice
-    
+    INTERPOLATION_RANGE = int(
+        10
+    )  # how many neighbouring values to take into account when interpolating the medial longitudinal fissure slice
+
     # check arguments
     if cut_plane >= image.ndim:
-        raise ArgumentError('The suppliedc cut-plane ({}) is invalid, the image has only {} dimensions.'.format(cut_plane, image.ndim))
-    
+        raise ArgumentError(
+            "The suppliedc cut-plane ({}) is invalid, the image has only {} dimensions.".format(
+                cut_plane, image.ndim
+            )
+        )
+
     # set voxel spacing
     if voxelspacing is None:
-        voxelspacing = [1.] * image.ndim
-    
+        voxelspacing = [1.0] * image.ndim
+
     # compute the (presumed) location of the medial longitudinal fissure, treating also the special of an odd number of slices, in which case a cut into two equal halves is not possible
     medial_longitudinal_fissure = int(image.shape[cut_plane] / 2)
     medial_longitudinal_fissure_excluded = image.shape[cut_plane] % 2
-    
+
     # split the head into a dexter and sinister half along the saggital plane
     # this is assumed to be consistent with a cut of the brain along the medial longitudinal fissure, thus separating it into its hemispheres
     slicer = [slice(None)] * image.ndim
     slicer[cut_plane] = slice(None, medial_longitudinal_fissure)
-    left_hemisphere = image[slicer]
+    left_hemisphere = image[tuple(slicer)]
+
+    slicer[cut_plane] = slice(
+        medial_longitudinal_fissure + medial_longitudinal_fissure_excluded, None
+    )
+    right_hemisphere = image[tuple(slicer)]
 
-    slicer[cut_plane] = slice(medial_longitudinal_fissure + medial_longitudinal_fissure_excluded, None)
-    right_hemisphere = image[slicer]
-    
     # flip right hemisphere image along cut plane
     slicer[cut_plane] = slice(None, None, -1)
-    right_hemisphere = right_hemisphere[slicer]
+    right_hemisphere = right_hemisphere[tuple(slicer)]
 
     # substract once left from right and once right from left hemisphere, including smoothing steps
-    right_hemisphere_difference = _substract_hemispheres(right_hemisphere, left_hemisphere, sigma_active, sigma_reference, voxelspacing)
-    left_hemisphere_difference = _substract_hemispheres(left_hemisphere, right_hemisphere, sigma_active, sigma_reference, voxelspacing)
-    
+    right_hemisphere_difference = _substract_hemispheres(
+        right_hemisphere, left_hemisphere, sigma_active, sigma_reference, voxelspacing
+    )
+    left_hemisphere_difference = _substract_hemispheres(
+        left_hemisphere, right_hemisphere, sigma_active, sigma_reference, voxelspacing
+    )
+
     # re-flip right hemisphere image to original orientation
-    right_hemisphere_difference = right_hemisphere_difference[slicer]
-    
+    right_hemisphere_difference = right_hemisphere_difference[tuple(slicer)]
+
     # estimate the medial longitudinal fissure if required
     if 1 == medial_longitudinal_fissure_excluded:
         left_slicer = [slice(None)] * image.ndim
         right_slicer = [slice(None)] * image.ndim
         left_slicer[cut_plane] = slice(-1 * INTERPOLATION_RANGE, None)
         right_slicer[cut_plane] = slice(None, INTERPOLATION_RANGE)
-        interp_data_left = left_hemisphere_difference[left_slicer]
-        interp_data_right = right_hemisphere_difference[right_slicer]
+        interp_data_left = left_hemisphere_difference[tuple(left_slicer)]
+        interp_data_right = right_hemisphere_difference[tuple(right_slicer)]
         interp_indices_left = list(range(-1 * interp_data_left.shape[cut_plane], 0))
         interp_indices_right = list(range(1, interp_data_right.shape[cut_plane] + 1))
-        interp_data = numpy.concatenate((left_hemisphere_difference[left_slicer], right_hemisphere_difference[right_slicer]), cut_plane)
-        interp_indices = numpy.concatenate((interp_indices_left, interp_indices_right), 0)
-        medial_longitudinal_fissure_estimated = interp1d(interp_indices, interp_data, kind='cubic', axis=cut_plane)(0)
+        interp_data = numpy.concatenate(
+            (
+                left_hemisphere_difference[tuple(left_slicer)],
+                right_hemisphere_difference[tuple(right_slicer)],
+            ),
+            cut_plane,
+        )
+        interp_indices = numpy.concatenate(
+            (interp_indices_left, interp_indices_right), 0
+        )
+        medial_longitudinal_fissure_estimated = interp1d(
+            interp_indices, interp_data, kind="cubic", axis=cut_plane
+        )(0)
         # add singleton dimension
         slicer[cut_plane] = numpy.newaxis
-        medial_longitudinal_fissure_estimated = medial_longitudinal_fissure_estimated[slicer]
+        medial_longitudinal_fissure_estimated = medial_longitudinal_fissure_estimated[
+            tuple(slicer)
+        ]
 
     # stich images back together
     if 1 == medial_longitudinal_fissure_excluded:
-        hemisphere_difference = numpy.concatenate((left_hemisphere_difference, medial_longitudinal_fissure_estimated, right_hemisphere_difference), cut_plane)
+        hemisphere_difference = numpy.concatenate(
+            (
+                left_hemisphere_difference,
+                medial_longitudinal_fissure_estimated,
+                right_hemisphere_difference,
+            ),
+            cut_plane,
+        )
     else:
-        hemisphere_difference = numpy.concatenate((left_hemisphere_difference, right_hemisphere_difference), cut_plane)
+        hemisphere_difference = numpy.concatenate(
+            (left_hemisphere_difference, right_hemisphere_difference), cut_plane
+        )
 
     # extract intensities and return
     return _extract_intensities(hemisphere_difference, mask)
 
-def _extract_local_histogram(image, mask=slice(None), bins=19, rang="image", cutoffp=(0.0, 100.0), size=None, footprint=None, output=None, mode="ignore", origin=0):
+
+def _extract_local_histogram(
+    image,
+    mask=slice(None),
+    bins=19,
+    rang="image",
+    cutoffp=(0.0, 100.0),
+    size=None,
+    footprint=None,
+    output=None,
+    mode="ignore",
+    origin=0,
+):
     """
     Internal, single-image version of @see local_histogram
-    
+
     Note: Values outside of the histograms range are not considered.
     Note: Mode constant is not available, instead a mode "ignore" is provided.
     Note: Default dtype of returned values is float.
     """
     if "constant" == mode:
-        raise RuntimeError('boundary mode not supported')
+        raise RuntimeError("boundary mode not supported")
     elif "ignore" == mode:
         mode = "constant"
-    if 'image' == rang:
+    if "image" == rang:
         rang = tuple(numpy.percentile(image[mask], cutoffp))
     elif not 2 == len(rang):
-        raise RuntimeError('the rang must contain exactly two elements or the string "image"')
-        
+        raise RuntimeError(
+            'the rang must contain exactly two elements or the string "image"'
+        )
+
     _, bin_edges = numpy.histogram([], bins=bins, range=rang)
-    output = _get_output(numpy.float if None == output else output, image, shape = [bins] + list(image.shape))
+    output = _get_output(
+        float if output is None else output, image, shape=[bins] + list(image.shape)
+    )
 
     # threshold the image into the histogram bins represented by the output images first dimension, treat last bin separately, since upper border is inclusive
     for i in range(bins - 1):
         output[i] = (image >= bin_edges[i]) & (image < bin_edges[i + 1])
     output[-1] = (image >= bin_edges[-2]) & (image <= bin_edges[-1])
 
     # apply the sum filter to each dimension, then normalize by dividing through the sum of elements in the bins of each histogram
     for i in range(bins):
-        output[i] = sum_filter(output[i], size=size, footprint=footprint, output=None, mode=mode, cval=0.0, origin=origin)
+        output[i] = sum_filter(
+            output[i],
+            size=size,
+            footprint=footprint,
+            output=None,
+            mode=mode,
+            cval=0.0,
+            origin=origin,
+        )
     divident = numpy.sum(output, 0)
     divident[0 == divident] = 1
     output /= divident
-    
+
     # Notes on modes:
     # mode=constant with a cval outside histogram range for the histogram equals a mode=constant with a cval = 0 for the sum_filter
     # mode=constant with a cval inside  histogram range for the histogram has no equal for the sum_filter (and does not make much sense)
     # mode=X for the histogram equals mode=X for the sum_filter
 
     # treat as multi-spectral image which intensities to extracted
     return _extract_feature(_extract_intensities, [h for h in output], mask)
-    
-def _extract_median(image, mask = slice(None), size = 1, voxelspacing = None):
+
+
+def _extract_median(image, mask=slice(None), size=1, voxelspacing=None):
     """
     Internal, single-image version of `median`.
     """
     # set voxel spacing
     if voxelspacing is None:
-        voxelspacing = [1.] * image.ndim
-        
+        voxelspacing = [1.0] * image.ndim
+
     # determine structure element size in voxel units
     size = _create_structure_array(size, voxelspacing)
-        
+
     return _extract_intensities(median_filter(image, size), mask)
-    
-def _extract_gaussian_gradient_magnitude(image, mask = slice(None), sigma = 1, voxelspacing = None):
+
+
+def _extract_gaussian_gradient_magnitude(
+    image, mask=slice(None), sigma=1, voxelspacing=None
+):
     """
     Internal, single-image version of `gaussian_gradient_magnitude`.
     """
     # set voxel spacing
     if voxelspacing is None:
-        voxelspacing = [1.] * image.ndim
-        
+        voxelspacing = [1.0] * image.ndim
+
     # determine gaussian kernel size in voxel units
     sigma = _create_structure_array(sigma, voxelspacing)
-        
+
     return _extract_intensities(scipy_gaussian_gradient_magnitude(image, sigma), mask)
-    
-def _extract_shifted_mean_gauss(image, mask = slice(None), offset = None, sigma = 1, voxelspacing = None):
+
+
+def _extract_shifted_mean_gauss(
+    image, mask=slice(None), offset=None, sigma=1, voxelspacing=None
+):
     """
     Internal, single-image version of `shifted_mean_gauss`.
-    """    
+    """
     # set voxel spacing
     if voxelspacing is None:
-        voxelspacing = [1.] * image.ndim
+        voxelspacing = [1.0] * image.ndim
     # set offset
     if offset is None:
         offset = [0] * image.ndim
-    
+
     # determine gaussian kernel size in voxel units
     sigma = _create_structure_array(sigma, voxelspacing)
-    
+
     # compute smoothed version of image
     smoothed = gaussian_filter(image, sigma)
-    
+
     shifted = numpy.zeros_like(smoothed)
     in_slicer = []
     out_slicer = []
     for o in offset:
         in_slicer.append(slice(o, None))
         out_slicer.append(slice(None, -1 * o))
-    shifted[out_slicer] = smoothed[in_slicer]
-    
+    shifted[tuple(out_slicer)] = smoothed[tuple(in_slicer)]
+
     return _extract_intensities(shifted, mask)
-    
-def _extract_mask_distance(image, mask = slice(None), voxelspacing = None):
+
+
+def _extract_mask_distance(image, mask=slice(None), voxelspacing=None):
     """
     Internal, single-image version of `mask_distance`.
     """
     if isinstance(mask, slice):
-        mask = numpy.ones(image.shape, numpy.bool)
-    
+        mask = numpy.ones(image.shape, numpy.bool_)
+
     distance_map = distance_transform_edt(mask, sampling=voxelspacing)
-    
+
     return _extract_intensities(distance_map, mask)
-    
-def _extract_local_mean_gauss(image, mask = slice(None), sigma = 1, voxelspacing = None):
+
+
+def _extract_local_mean_gauss(image, mask=slice(None), sigma=1, voxelspacing=None):
     """
     Internal, single-image version of `local_mean_gauss`.
     """
     # set voxel spacing
     if voxelspacing is None:
-        voxelspacing = [1.] * image.ndim
-        
+        voxelspacing = [1.0] * image.ndim
+
     # determine gaussian kernel size in voxel units
     sigma = _create_structure_array(sigma, voxelspacing)
-        
+
     return _extract_intensities(gaussian_filter(image, sigma), mask)
 
 
-def _extract_centerdistance(image, mask = slice(None), voxelspacing = None):
+def _extract_centerdistance(image, mask=slice(None), voxelspacing=None):
     """
     Internal, single-image version of `centerdistance`.
     """
     image = numpy.array(image, copy=False)
-    
+
     if None == voxelspacing:
-        voxelspacing = [1.] * image.ndim
-        
+        voxelspacing = [1.0] * image.ndim
+
     # get image center and an array holding the images indices
-    centers = [(x - 1) / 2. for x in image.shape]
-    indices = numpy.indices(image.shape, dtype=numpy.float)
-    
+    centers = [(x - 1) / 2.0 for x in image.shape]
+    indices = numpy.indices(image.shape, dtype=float)
+
     # shift to center of image and correct spacing to real world coordinates
     for dim_indices, c, vs in zip(indices, centers, voxelspacing):
         dim_indices -= c
         dim_indices *= vs
-        
+
     # compute euclidean distance to image center
     return numpy.sqrt(numpy.sum(numpy.square(indices), 0))[mask].ravel()
-    
 
-def _extract_intensities(image, mask = slice(None)):
+
+def _extract_intensities(image, mask=slice(None)):
     """
     Internal, single-image version of `intensities`.
     """
+    if type(mask) is list and type(mask[0]) is slice:
+        mask = tuple(mask)
     return numpy.array(image, copy=True)[mask].ravel()
 
-def _substract_hemispheres(active, reference, active_sigma, reference_sigma, voxel_spacing):
+
+def _substract_hemispheres(
+    active, reference, active_sigma, reference_sigma, voxel_spacing
+):
     """
     Helper function for `_extract_hemispheric_difference`.
     Smoothes both images and then substracts the reference from the active image.
     """
     active_kernel = _create_structure_array(active_sigma, voxel_spacing)
-    active_smoothed = gaussian_filter(active, sigma = active_kernel)
+    active_smoothed = gaussian_filter(active, sigma=active_kernel)
 
     reference_kernel = _create_structure_array(reference_sigma, voxel_spacing)
-    reference_smoothed = gaussian_filter(reference, sigma = reference_kernel)
+    reference_smoothed = gaussian_filter(reference, sigma=reference_kernel)
 
     return active_smoothed - reference_smoothed
 
+
 def _create_structure_array(structure_array, voxelspacing):
     """
     Convenient function to take a structure array (single number valid for all dimensions
     or a sequence with a distinct number for each dimension) assumed to be in mm and
     returns a structure array (a sequence) adapted to the image space using the supplied
     voxel spacing.
     """
     try:
-        structure_array = [s / float(vs) for s, vs in zip(structure_array, voxelspacing)]
+        structure_array = [
+            s / float(vs) for s, vs in zip(structure_array, voxelspacing)
+        ]
     except TypeError:
         structure_array = [structure_array / float(vs) for vs in voxelspacing]
-    
-    return structure_array    
 
-def _extract_feature(fun, image, mask = slice(None), **kwargs):
+    return structure_array
+
+
+def _extract_feature(fun, image, mask=slice(None), **kwargs):
     """
     Convenient function to cope with multi-spectral images and feature normalization.
-    
+
     Parameters
     ----------
     fun : function
         The feature extraction function to call
-    image : array_like or list/tuple of array_like 
+    image : array_like or list/tuple of array_like
         A single image or a list/tuple of images (for multi-spectral case).
     mask : ndarray
         The binary mask to select the voxels for which to extract the feature
     kwargs : sequence
-        Additional keyword arguments to be passed to the feature extraction function 
+        Additional keyword arguments to be passed to the feature extraction function
     """
     if not type(mask) is slice:
-        mask = numpy.array(mask, copy=False, dtype=numpy.bool)
-    
-    if type(image) == tuple or type(image) == list:
+        mask = numpy.array(mask, copy=False, dtype=numpy.bool_)
+
+    if type(image) is tuple or type(image) is list:
         return join(*[fun(i, mask, **kwargs) for i in image])
     else:
         return fun(image, mask, **kwargs)
```

### Comparing `MedPy-0.4.0/medpy/features/utilities.py` & `MedPy-0.5.0/medpy/features/utilities.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Copyright (C) 2013 Oskar Maier
-# 
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
-# 
+#
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
-# 
+#
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 # author Oskar Maier
 # version r0.1.1
 # since 2013-08-24
 # status Release
@@ -24,184 +24,187 @@
 import numpy
 
 # own modules
 
 # code
 
 
-def normalize(vector, cutoffp = (0, 100), model = False):
+def normalize(vector, cutoffp=(0, 100), model=False):
     r"""
     Returns a feature-wise normalized version of the supplied vector. Normalization is
     achieved to [0,1] over the complete vector using shifting and scaling.
-    
+
     When cut-off percentile (cutoffp) values other than (0, 100) are supplied, the values
     lying before or behind the supplied percentiles are cut-off i.e. shifted to fit the
-    range. 
-    
+    range.
+
     When model is set to True, an additional model describing the normalization is
     returned, that can at a later point be passed to the `normalize_with_model` function
     to normalize other feature vectors accordingly to the one passed.
-    
+
     The vector is expected to have the form samples*features i.e.::
-    
+
             s1    s2    s3    [...]
         f1
         f2
         [...]
-    
+
     Therefore a supplied vector::
-    
+
             s1    s2    s3
         f1   1.5    1    2
         f2    -1    0    1
-    
+
     would result in the returned vector::
-    
+
             s1    s2    s3
         f1 0.50  0.00  1.00
         f2 0.00  0.50  1.00
-    
+
     Parameters
     ----------
     vector : sequence
         A sequence of feature vectors to normalize.
     cutoffp : (float, float)
         Cut-off percentiles.
     model : bool
         Whether to return the learned normalization model.
-    
+
     Returns
     -------
     normalized_feature_vectors : ndarray
         The normalized versions of the input vectors.
     model : tuple, optional
         The learned normalization model.
-    
+
     """
-    vector = numpy.array(vector, dtype=numpy.float)
-    
+    vector = numpy.array(vector, dtype=float)
+
     # add a singleton dimension if required
     if 1 == vector.ndim:
         vector = vector[:, None]
-    
+
     # compute lower and upper range border of each row using the supplied percentiles
     minp, maxp = numpy.percentile(vector, cutoffp, 0)
-    
+
     # shift outliers to fit range
     for i in range(vector.shape[1]):
-        vector[:,i][vector[:,i] < minp[i]] = minp[i]
-        vector[:,i][vector[:,i] > maxp[i]] = maxp[i]
-    
+        vector[:, i][vector[:, i] < minp[i]] = minp[i]
+        vector[:, i][vector[:, i] > maxp[i]] = maxp[i]
+
     # normalize
     minv = vector.min(0)
     vector -= minv
     maxv = vector.max(0)
     vector /= maxv
-    
+
     if not model:
         return vector
     else:
         return vector, (minp, maxp, minv, maxv)
-    
+
+
 def normalize_with_model(vector, model):
     r"""
     Normalize as with `normalize`, but not based on the data of the passed feature
     vector, but rather on a learned model created with `normalize`. Thus formerly
     unseen query data can be normalized according to the training data.
-    
+
     Parameters
     ----------
     vector : sequence
         A sequence of feature vectors to normalize.
     model : tuple
         A normalization model created with `normalize`.
-    
+
     Returns
     -------
     normalize : ndarray
         The normalized versions of the input vectors.
     """
-    vector = numpy.array(vector, dtype=numpy.float)
-    
+    vector = numpy.array(vector, dtype=float)
+
     # unpack model
     minp, maxp, minv, maxv = model
-    
+
     # add a singleton dimension if required
     if 1 == vector.ndim:
         vector = vector[:, None]
-    
+
     # shift outliers to fit range
     for i in range(vector.shape[1]):
-        vector[:,i][vector[:,i] < minp[i]] = minp[i]
-        vector[:,i][vector[:,i] > maxp[i]] = maxp[i]
-        
+        vector[:, i][vector[:, i] < minp[i]] = minp[i]
+        vector[:, i][vector[:, i] > maxp[i]] = maxp[i]
+
     # normalize
     vector -= minv
     vector /= maxv
-    
-    return vector        
+
+    return vector
+
 
 def append(*vectors):
     r"""
     Takes an arbitrary number of vectors containing features and append them
     (horizontally).
-    
+
     E.g. taking a 100 and a 200 sample vector with 7 features each, a 300x7
     vector is returned.
-    
+
     The vectors are expected to have the form samples*features i.e.::
-    
+
             s1    s2    s3    [...]
         f1
         f2
         [...]
-    
+
     Parameters
     ----------
     *vectors : sequences
         A number of vectors with the same number and type of features.
-    
+
     Returns
     -------
     vector : ndarray
         The appended vectors.
     """
     # check supplied arguments
     if len(vectors) < 2:
         return vectors[0]
-    
+
     # process supplied arguments
     vectors = list(vectors)
     for i in range(len(vectors)):
         vectors[i] = numpy.asarray(vectors[i])
         if vectors[i].ndim == 1:
             vectors[i] = numpy.asarray([vectors[i]]).T
 
     return numpy.squeeze(numpy.concatenate(vectors, 0))
-    
+
+
 def join(*vectors):
     r"""
     Takes an arbitrary number of aligned vectors of the same length and combines
     them into a single vector (vertically).
-    
+
     E.g. taking two 100-sample feature vectors of once 5 and once 7 features, a 100x12
-    feature vector is created and returned. 
-    
+    feature vector is created and returned.
+
     The feature vectors are expected to have the form samples*features i.e.::
-    
+
             s1    s2    s3    [...]
         f1
         f2
         [...]
-    
+
     Parameters
     ----------
     *vectors : sequences
         A number of vectors with the same number of samples.
-    
+
     Returns
     -------
     vector : ndarray
         The combined vectors.
     """
     # check supplied arguments
     if len(vectors) < 2:
@@ -209,13 +212,13 @@
 
     # process supplied arguments
     vectors = list(vectors)
     for i in range(len(vectors)):
         vectors[i] = numpy.array(vectors[i], copy=False)
         if vectors[i].ndim == 1:
             vectors[i] = numpy.array([vectors[i]], copy=False).T
-    
+
     # treat single-value cases special (no squeezing)
     if 1 == len(vectors[0]):
         return numpy.concatenate(vectors, 1)
-    
+
     return numpy.squeeze(numpy.concatenate(vectors, 1))
```

### Comparing `MedPy-0.4.0/medpy/features/texture.py` & `MedPy-0.5.0/medpy/features/texture.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,190 +1,213 @@
 # Copyright (C) 2013 Oskar Maier
-# 
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
-# 
+#
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
-# 
+#
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 # author Alexander Ruesch
 # version r0.1.1
 # since 2013-08-24
 # status Release
 
 # build-in modules
 
+from math import factorial
+
 # third-party modules
 import numpy
-from scipy.ndimage.filters import uniform_filter, sobel, maximum_filter, minimum_filter, gaussian_filter
 from scipy import stats
-from math import factorial
+from scipy.ndimage import (
+    gaussian_filter,
+    maximum_filter,
+    minimum_filter,
+    sobel,
+    uniform_filter,
+)
 
 # own modules
 
 # constants
 
-def coarseness(image, voxelspacing = None, mask = slice(None)):
+
+def coarseness(image, voxelspacing=None, mask=slice(None)):
     r"""
     Takes a simple or multi-spectral image and returns the coarseness of the texture.
-    
+
     Step1  At each pixel, compute six averages for the windows of size 2**k x 2**k,
-            k=0,1,...,5, around the pixel. 
-    Step2  At each pixel, compute absolute differences E between the pairs of non 
+            k=0,1,...,5, around the pixel.
+    Step2  At each pixel, compute absolute differences E between the pairs of non
             overlapping averages in every directions.
-    step3  At each pixel, find the value of k that maximises the difference Ek in either 
+    step3  At each pixel, find the value of k that maximises the difference Ek in either
             direction and set the best size Sbest=2**k
     step4  Compute the coarseness feature Fcrs by averaging Sbest over the entire image.
 
     Parameters
     ----------
-    image : array_like or list/tuple of array_like 
+    image : array_like or list/tuple of array_like
         A single image or a list/tuple of images (for multi-spectral case).
     voxelspacing : sequence of floats
         The side-length of each voxel.
     mask : array_like
         A binary mask for the image or a slice object
-        
+
     Returns
     -------
     coarseness : float
         The size of coarseness of the given texture. It is basically the size of
-        repeating elements in the image. 
-        
+        repeating elements in the image.
+
     See Also
     --------
-    
-    
+
+
     """
     # Step1:  At each pixel (x,y), compute six averages for the windows
     # of size 2**k x 2**k, k=0,1,...,5, around the pixel.
 
     image = numpy.asarray(image, dtype=numpy.float32)
-   
-  
+
     # set default mask or apply given mask
     if not type(mask) is slice:
         if not type(mask[0] is slice):
-            mask = numpy.array(mask, copy=False, dtype = numpy.bool)
+            mask = numpy.array(mask, copy=False, dtype=numpy.bool_)
     image = image[mask]
-    
+
     # set default voxel spacing if not suppliec
-    if None == voxelspacing:
-        voxelspacing = tuple([1.] * image.ndim)
-    
+    if voxelspacing is None:
+        voxelspacing = tuple([1.0] * image.ndim)
+
     if len(voxelspacing) != image.ndim:
         print("Voxel spacing and image dimensions do not fit.")
         return None
     # set padding for image border control
-    padSize = numpy.asarray([(numpy.rint((2**5.0) * voxelspacing[jj]),0) for jj in range(image.ndim)]).astype(numpy.int)
-    Apad = numpy.pad(image,pad_width=padSize, mode='reflect')
+    padSize = numpy.asarray(
+        [
+            (int(numpy.rint((2**5.0) * voxelspacing[jj])), 0)
+            for jj in range(image.ndim)
+        ]
+    ).astype(int)
+    Apad = numpy.pad(image, pad_width=padSize, mode="reflect")
 
     # Allocate memory
-    E = numpy.empty((6,image.ndim)+image.shape)
+    E = numpy.empty((6, image.ndim) + image.shape)
 
-    # prepare some slicer 
-    rawSlicer           = [slice(None)] * image.ndim
-    slicerForImageInPad = [slice(padSize[d][0],None)for d in range(image.ndim)]
+    # prepare some slicer
+    rawSlicer = [slice(None)] * image.ndim
+    slicerForImageInPad = [slice(padSize[d][0], None) for d in range(image.ndim)]
 
     for k in range(6):
+        size_vs = tuple(
+            int(numpy.rint((2**k) * voxelspacing[jj])) for jj in range(image.ndim)
+        )
+        A = uniform_filter(Apad, size=size_vs, mode="mirror")
 
-        size_vs = tuple(numpy.rint((2**k) * voxelspacing[jj]) for jj in range(image.ndim))
-        A = uniform_filter(Apad, size = size_vs, mode = 'mirror')
-
-        # Step2: At each pixel, compute absolute differences E(x,y) between 
+        # Step2: At each pixel, compute absolute differences E(x,y) between
         # the pairs of non overlapping averages in the horizontal and vertical directions.
         for d in range(image.ndim):
-            borders = numpy.rint((2**k) * voxelspacing[d])
-            
-            slicerPad_k_d   = slicerForImageInPad[:]
-            slicerPad_k_d[d]= slice((padSize[d][0]-borders if borders < padSize[d][0] else 0),None)
-            A_k_d           = A[slicerPad_k_d]
-
-            AslicerL        = rawSlicer[:]
-            AslicerL[d]     = slice(0, -borders)
-            
-            AslicerR        = rawSlicer[:]
-            AslicerR[d]     = slice(borders, None)
+            borders = int(numpy.rint((2**k) * voxelspacing[d]))
+
+            slicerPad_k_d = slicerForImageInPad[:]
+            slicerPad_k_d[d] = slice(
+                (int(padSize[d][0] - borders) if borders < padSize[d][0] else 0), None
+            )
+            A_k_d = A[tuple(slicerPad_k_d)]
+
+            AslicerL = rawSlicer[:]
+            AslicerL[d] = slice(0, -borders)
+
+            AslicerR = rawSlicer[:]
+            AslicerR[d] = slice(borders, None)
 
-            E[k,d,...] = numpy.abs(A_k_d[AslicerL] - A_k_d[AslicerR])
+            E[k, d, ...] = numpy.abs(A_k_d[tuple(AslicerL)] - A_k_d[tuple(AslicerR)])
 
     # step3: At each pixel, find the value of k that maximises the difference Ek(x,y)
     # in either direction and set the best size Sbest(x,y)=2**k
-    
+
     k_max = E.max(1).argmax(0)
     dim = E.argmax(1)
-    dim_vox_space = numpy.asarray([voxelspacing[dim[k_max.flat[i]].flat[i]] for i in range(k_max.size)]).reshape(k_max.shape) 
+    dim_vox_space = numpy.asarray(
+        [voxelspacing[dim[k_max.flat[i]].flat[i]] for i in range(k_max.size)]
+    ).reshape(k_max.shape)
     S = (2**k_max) * dim_vox_space
 
     # step4: Compute the coarseness feature Fcrs by averaging Sbest(x,y) over the entire image.
     return S.mean()
 
-def contrast(image, mask = slice(None)):
+
+def contrast(image, mask=slice(None)):
     r"""
     Takes a simple or multi-spectral image and returns the contrast of the texture.
-    
+
     Fcon = standard_deviation(gray_value) / (kurtosis(gray_value)**0.25)
-    
+
     Parameters
     ----------
-    image : array_like or list/tuple of array_like 
+    image : array_like or list/tuple of array_like
         A single image or a list/tuple of images (for multi-spectral case).
     mask : array_like
         A binary mask for the image or a slice object
     Returns
     -------
     contrast : float
-        High differences in gray value distribution is represented in a high contrast value. 
-        
+        High differences in gray value distribution is represented in a high contrast value.
+
     See Also
     --------
-    
-    
+
+
     """
     image = numpy.asarray(image)
-    
+
     # set default mask or apply given mask
     if not type(mask) is slice:
         if not type(mask[0] is slice):
-            mask = numpy.array(mask, copy=False, dtype = numpy.bool)
+            mask = numpy.array(mask, copy=False, dtype=numpy.bool_)
+        else:
+            mask = tuple(mask)
     image = image[mask]
-    
+
     standard_deviation = numpy.std(image)
     kurtosis = stats.kurtosis(image, axis=None, bias=True, fisher=False)
-    n = 0.25 # The value n=0.25 is recommended as the best for discriminating the textures.  
-    
-    Fcon = standard_deviation / (kurtosis**n) 
-    
+    n = 0.25  # The value n=0.25 is recommended as the best for discriminating the textures.
+
+    Fcon = standard_deviation / (kurtosis**n)
+
     return Fcon
 
-def directionality(image, min_distance = 4, threshold = 0.1, voxelspacing = None, mask = slice(None)):
+
+def directionality(
+    image, min_distance=4, threshold=0.1, voxelspacing=None, mask=slice(None)
+):
     r"""
     Takes a simple or multi-spectral image and returns the directionality of the image texture.
-    It is just a value representing the strength of directionality, not the specific direction. 
-    
+    It is just a value representing the strength of directionality, not the specific direction.
+
     An edge detection is applied on the image. Then the edge strength and directional angle between
     the image axis are computed. A histogram of the directional angles is than used to calculate a
     qualitative value for directionality in ONE image layer. Note that there are n choose 2 layers
-    in a n dimensional image. 
-    
+    in a n dimensional image.
+
     Warning
     -------
     Experimental. There are still issues with finding the right maxs and mins in histogram and
     predefining the number of bins for the histogram.
 
     Parameters
     ----------
-    image : array_like or list/tuple of array_like 
+    image : array_like or list/tuple of array_like
         A single image or a list/tuple of images (for multi-spectral case).
     voxelspacing : sequence of floats
         The side-length of each voxel.
     mask : array_like
         A binary mask for the image or a slice object
     min_distance : int
         minimal Distance between 2 local minima or maxima in the histogram. Default is 4.
@@ -199,126 +222,146 @@
         Returns the directionality of an image in relation to one special image layer.
         The returned values are sorted like this. The axis are named v,w,x,y,z
         for a five dimensional image:
                                     w   x   y   z   v     x   y   z   v   w
         arctan(delta)| delta =    ---,---,---,---,---,  ---,---,---,---,---
                                     v   w   x   y   z     v   w   x   y   z
         There are always n choose k axis relations; n=image.ndim, k=2 (2 axis in every image layer).
-        
-    
+
+
     See Also
     --------
-    
+
     """
     image = numpy.asarray(image)
     ndim = image.ndim
+    min_distance = int(min_distance)
     # set default mask or apply given mask
     if not type(mask) is slice:
         if not type(mask[0] is slice):
-            mask = numpy.array(mask, copy=False, dtype = numpy.bool)
+            mask = numpy.array(mask, copy=False, dtype=numpy.bool_)
     image = image[mask]
-           
+
     # set default voxel spacing if not suppliec
-    if None == voxelspacing:
-        voxelspacing = tuple([1.] * ndim)
-        
+    if voxelspacing is None:
+        voxelspacing = tuple([1.0] * ndim)
+
     if len(voxelspacing) != ndim:
         print("Voxel spacing and image dimensions do not fit.")
         return None
-   
-   # Calculate amount of combinations: n choose k, normalizing factor r and voxel spacing.    
-    n = (factorial(ndim)/(2*factorial(ndim-2)))
-    pi1_2 = numpy.pi/2.0
-    r=1.0 / (pi1_2**2)
-    vs = [slice(None,None,numpy.rint(ii)) for ii in voxelspacing]
-   
+
+    # Calculate amount of combinations: n choose k, normalizing factor r and voxel spacing.
+    n = factorial(ndim) // (2 * factorial(ndim - 2))
+    pi1_2 = numpy.pi / 2.0
+    r = 1.0 / (pi1_2**2)
+    vs = [slice(None, None, int(numpy.rint(ii))) for ii in voxelspacing]
+
     # Allocate memory, define constants
     Fdir = numpy.empty(n)
 
     # calculate differences by using Sobel-filter. (Maybe other filter kernel like Prewitt will do a better job)
-    E = [sobel(image, axis=ndim-1-i) for i in range(ndim)]
-    
+    E = [sobel(image, axis=ndim - 1 - i) for i in range(ndim)]
+
     # The edge strength e(x,y) is used for thresholding.
     e = sum(E) / float(ndim)
-    border = [numpy.percentile(e, 1),numpy.percentile(e, 99)]
+    border = [numpy.percentile(e, 1), numpy.percentile(e, 99)]
     e[e < border[0]] = 0
     e[e > border[1]] = border[1]
     e -= border[0]
     e /= border[1]
     em = e > threshold
-        
+
     for i in range(n):
-        A = numpy.arctan((E[(i + (ndim+i)/ndim) % ndim][vs]) / (E[i%ndim][vs]+numpy.spacing(1))) # [0 , pi/2]
-        A = A[em[vs]]
-        # Calculate number of bins for the histogram. Watch out, this is just a work around! 
+        A = numpy.arctan(
+            (E[int((i + (ndim + i) / ndim) % ndim)][tuple(vs)])
+            / (E[int(i % ndim)][tuple(vs)] + numpy.spacing(1))
+        )  # [0 , pi/2]
+        A = A[em[tuple(vs)]]
+        # Calculate number of bins for the histogram. Watch out, this is just a work around!
         # @TODO: Write a more stable code to prevent for minimum and maximum repetition when the same value in the Histogram appears multiple times in a row. Example: image = numpy.zeros([10,10]), image[:,::3] = 1
-        bins = numpy.unique(A).size + min_distance        
-        H = numpy.histogram(A, bins = bins, density=True)[0] # [0 , 1]
-        H[H < numpy.percentile(H,1)] = 0.0
+        bins = numpy.unique(A).size + min_distance
+        H = numpy.histogram(A, bins=bins, density=True)[0]  # [0 , 1]
+        H[H < numpy.percentile(H, 1)] = 0.0
         H_peaks, H_valleys, H_range = find_valley_range(H)
         summe = 0.0
         for idx_ap in range(len(H_peaks)):
-            for range_idx in range( H_valleys[idx_ap], H_valleys[idx_ap]+H_range[idx_ap]):
-                a=range_idx % len(H)
-                summe += (((pi1_2*a)/bins - (pi1_2 * H_peaks[idx_ap])/bins) **2) * H[a]
-        Fdir[i] = 1.0 - r * summe 
-        
+            for range_idx in range(
+                numpy.squeeze(H_valleys[idx_ap]),
+                numpy.squeeze(H_valleys[idx_ap] + H_range[idx_ap]),
+            ):
+                a = range_idx % len(H)
+                summe += (
+                    ((pi1_2 * a) / bins - (pi1_2 * H_peaks[idx_ap]) / bins) ** 2
+                ) * H[a]
+        Fdir[i] = 1.0 - r * numpy.squeeze(summe)
+
     return Fdir
 
 
-def local_maxima(vector,min_distance = 4, brd_mode = "wrap"):
+def local_maxima(vector, min_distance=4, brd_mode="wrap"):
     """
     Internal finder for local maxima .
     Returns UNSORTED indices of maxima in input vector.
     """
-    fits = gaussian_filter(numpy.asarray(vector,dtype=numpy.float32),1., mode=brd_mode)
+    fits = gaussian_filter(
+        numpy.asarray(vector, dtype=numpy.float32), 1.0, mode=brd_mode
+    )
     for ii in range(len(fits)):
-        if fits[ii] == fits[ii-1]:
-            fits[ii-1] = 0.0
-    maxfits     = maximum_filter(fits, size=min_distance, mode=brd_mode)
+        if fits[ii] == fits[ii - 1]:
+            fits[ii - 1] = 0.0
+    maxfits = maximum_filter(fits, size=min_distance, mode=brd_mode)
     maxima_mask = fits == maxfits
-    maximum     = numpy.transpose(maxima_mask.nonzero())
+    maximum = numpy.transpose(maxima_mask.nonzero())
     return numpy.asarray(maximum)
 
-def local_minima(vector,min_distance = 4, brd_mode = "wrap"):
+
+def local_minima(vector, min_distance=4, brd_mode="wrap"):
     """
     Internal finder for local minima .
     Returns UNSORTED indices of minima in input vector.
     """
-    fits = gaussian_filter(numpy.asarray(vector,dtype=numpy.float32),1., mode=brd_mode)
+    fits = gaussian_filter(
+        numpy.asarray(vector, dtype=numpy.float32), 1.0, mode=brd_mode
+    )
     for ii in range(len(fits)):
-        if fits[ii] == fits[ii-1]:
-            fits[ii-1] = numpy.pi/2.0
+        if fits[ii] == fits[ii - 1]:
+            fits[ii - 1] = numpy.pi / 2.0
     minfits = minimum_filter(fits, size=min_distance, mode=brd_mode)
     minima_mask = fits == minfits
     minima = numpy.transpose(minima_mask.nonzero())
     return numpy.asarray(minima)
 
-def find_valley_range(vector, min_distance = 4):
+
+def find_valley_range(vector, min_distance=4):
     """
     Internal finder peaks and valley ranges.
     Returns UNSORTED indices of maxima in input vector.
     Returns range of valleys before and after maximum
     """
-    
+
     # http://users.monash.edu.au/~dengs/resource/papers/icme08.pdf
     # find min and max with mode = wrap
     mode = "wrap"
-    minima = local_minima(vector,min_distance,mode)
-    maxima = local_maxima(vector,min_distance,mode)
+    minima = local_minima(vector, min_distance, mode)
+    maxima = local_maxima(vector, min_distance, mode)
 
-    if len(maxima)>len(minima):
+    if len(maxima) > len(minima):
         if vector[maxima[0]] >= vector[maxima[-1]]:
-            maxima=maxima[1:]
+            maxima = maxima[1:]
         else:
-            maxima=maxima[:-1]
-        
-    if len(maxima)==len(minima):
-        valley_range = numpy.asarray([minima[ii+1] - minima[ii] for ii in range(len(minima)-1)] + [len(vector)-minima[-1]+minima[0]])
+            maxima = maxima[:-1]
+
+    if len(maxima) == len(minima):
+        valley_range = numpy.asarray(
+            [minima[ii + 1] - minima[ii] for ii in range(len(minima) - 1)]
+            + [len(vector) - minima[-1] + minima[0]]
+        )
         if minima[0] < maxima[0]:
             minima = numpy.asarray(list(minima) + [minima[0]])
         else:
-            minima = numpy.asarray(list(minima) + [minima[-1]])       
+            minima = numpy.asarray(list(minima) + [minima[-1]])
     else:
-        valley_range = numpy.asarray([minima[ii+1] - minima[ii] for ii in range(len(maxima))])
-    
+        valley_range = numpy.asarray(
+            [minima[ii + 1] - minima[ii] for ii in range(len(maxima))]
+        )
+
     return maxima, minima, valley_range
```

### Comparing `MedPy-0.4.0/medpy/filter/noise.py` & `MedPy-0.5.0/medpy/filter/noise.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,201 +1,213 @@
 # Copyright (C) 2013 Oskar Maier
-# 
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
-# 
+#
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
-# 
+#
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 # author Oskar Maier
 # version r0.1.0
 # since 2014-03-20
 # status Release
 
 # build-in modules
 
 # third-party modules
 import numpy
-from scipy.ndimage import _ni_support
-from scipy.ndimage.filters import convolve1d
+from scipy.ndimage import _ni_support, convolve1d
 
 # own modules
 
+
 # code
 def immerkaer_local(input, size, output=None, mode="reflect", cval=0.0):
     r"""
     Estimate the local noise.
-    
+
     The input image is assumed to have additive zero mean Gaussian noise. The Immerkaer
     noise estimation is applied to the image locally over a N-dimensional cube of
     side-length size. The size of the region should be sufficiently high for a stable
     noise estimation.
-    
+
     Parameters
     ----------
     input : array_like
         Array of which to estimate the noise.
     size : integer
         The local region's side length.
     output : ndarray, optional
         The `output` parameter passes an array in which to store the
-        filter output.        
+        filter output.
     mode : {'reflect', 'constant', 'nearest', 'mirror', 'wrap'}, optional
         The `mode` parameter determines how the array borders are
         handled, where `cval` is the value when mode is equal to
         'constant'. Default is 'reflect'
     cval : scalar, optional
         Value to fill past edges of input if `mode` is 'constant'. Default
-        is 0.0        
-        
+        is 0.0
+
     Returns
     -------
     sigmas : array_like
         Map of the estimated standard deviation of the images Gaussian noise per voxel.
-    
+
     Notes
     -----
     Does not take the voxel spacing into account.
     Works good with medium to strong noise. Tends to underestimate for low noise levels.
-    
+
     See also
     --------
     immerkaer
     """
     output = _ni_support._get_output(output, input)
     footprint = numpy.asarray([1] * size)
-    
+
     # build nd-kernel to acquire square root of sum of squared elements
     kernel = [1, -2, 1]
     for _ in range(input.ndim - 1):
         kernel = numpy.tensordot(kernel, [1, -2, 1], 0)
-    divider = numpy.square(numpy.abs(kernel)).sum() # 36 for 1d, 216 for 3D, etc.
-    
+    divider = numpy.square(numpy.abs(kernel)).sum()  # 36 for 1d, 216 for 3D, etc.
+
     # compute laplace of input
     laplace = separable_convolution(input, [1, -2, 1], numpy.double, mode, cval)
-    
+
     # compute factor
-    factor = numpy.sqrt(numpy.pi / 2.) * 1. / ( numpy.sqrt(divider) * numpy.power(footprint.size, laplace.ndim) )
-    
+    factor = (
+        numpy.sqrt(numpy.pi / 2.0)
+        * 1.0
+        / (numpy.sqrt(divider) * numpy.power(footprint.size, laplace.ndim))
+    )
+
     # locally sum laplacian values
     separable_convolution(numpy.abs(laplace), footprint, output, mode, cval)
-    
+
     output *= factor
-    
+
     return output
 
+
 def immerkaer(input, mode="reflect", cval=0.0):
     r"""
     Estimate the global noise.
-    
+
     The input image is assumed to have additive zero mean Gaussian noise. Using a
     convolution with a Laplacian operator and a subsequent averaging the standard
     deviation sigma of this noise is estimated. This estimation is global i.e. the
     noise is assumed to be globally homogeneous over the image.
-    
+
     Implementation based on [1]_.
-    
-        
+
+
     Immerkaer suggested a Laplacian-based 2D kernel::
-    
+
         [[ 1, -2,  1],
          [-2,  4, -1],
          [ 1, -2, 1]]
 
     , which is separable and can therefore be applied by consecutive convolutions with
     the one dimensional kernel [1, -2, 1].
-    
+
     We generalize from this 1D-kernel to an ND-kernel by applying N consecutive
     convolutions with the 1D-kernel along all N dimensions.
-    
+
     This is equivalent with convolving the image with an ND-kernel constructed by calling
-    
+
     >>> kernel1d = numpy.asarray([1, -2, 1])
     >>> kernel = kernel1d.copy()
     >>> for _ in range(input.ndim):
     >>>     kernel = numpy.tensordot(kernel, kernel1d, 0)
-    
+
     Parameters
     ----------
     input : array_like
         Array of which to estimate the noise.
     mode : {'reflect', 'constant', 'nearest', 'mirror', 'wrap'}, optional
         The `mode` parameter determines how the array borders are
         handled, where `cval` is the value when mode is equal to
         'constant'. Default is 'reflect'
     cval : scalar, optional
         Value to fill past edges of input if `mode` is 'constant'. Default
-        is 0.0        
-        
+        is 0.0
+
     Returns
     -------
     sigma : float
         The estimated standard deviation of the images Gaussian noise.
-        
+
     Notes
     -----
     Does not take the voxel spacing into account.
     Works good with medium to strong noise. Tends to underestimate for low noise levels.
-        
+
     See also
     --------
     immerkaer_local
-    
+
     References
     ----------
     .. [1] John Immerkaer, "Fast Noise Variance Estimation", Computer Vision and Image
            Understanding, Volume 64, Issue 2, September 1996, Pages 300-302, ISSN 1077-3142
     """
     # build nd-kernel to acquire square root of sum of squared elements
     kernel = [1, -2, 1]
     for _ in range(input.ndim - 1):
         kernel = numpy.tensordot(kernel, [1, -2, 1], 0)
-    divider = numpy.square(numpy.abs(kernel)).sum() # 36 for 1d, 216 for 3D, etc.
-    
+    divider = numpy.square(numpy.abs(kernel)).sum()  # 36 for 1d, 216 for 3D, etc.
+
     # compute laplace of input and derive noise sigma
     laplace = separable_convolution(input, [1, -2, 1], None, mode, cval)
-    factor = numpy.sqrt(numpy.pi / 2.) * 1. / ( numpy.sqrt(divider) * numpy.prod(laplace.shape) )
+    factor = (
+        numpy.sqrt(numpy.pi / 2.0)
+        * 1.0
+        / (numpy.sqrt(divider) * numpy.prod(laplace.shape))
+    )
     sigma = factor * numpy.abs(laplace).sum()
-    
+
     return sigma
-    
-def separable_convolution(input, weights, output=None, mode="reflect", cval=0.0, origin=0):
+
+
+def separable_convolution(
+    input, weights, output=None, mode="reflect", cval=0.0, origin=0
+):
     r"""
     Calculate a n-dimensional convolution of a separable kernel to a n-dimensional input.
-    
+
     Achieved by calling convolution1d along the first axis, obtaining an intermediate
     image, on which the next convolution1d along the second axis is called and so on.
-    
+
     Parameters
     ----------
     input : array_like
         Array of which to estimate the noise.
     weights : ndarray
-        One-dimensional sequence of numbers.          
+        One-dimensional sequence of numbers.
     output : array, optional
         The `output` parameter passes an array in which to store the
         filter output.
     mode : {'reflect', 'constant', 'nearest', 'mirror', 'wrap'}, optional
         The `mode` parameter determines how the array borders are
         handled, where `cval` is the value when mode is equal to
         'constant'. Default is 'reflect'
     cval : scalar, optional
         Value to fill past edges of input if `mode` is 'constant'. Default
         is 0.0
     origin : scalar, optional
         The `origin` parameter controls the placement of the filter.
         Default 0.0.
-        
+
     Returns
     -------
     output : ndarray
         Input image convolved with the supplied kernel.
     """
     input = numpy.asarray(input)
     output = _ni_support._get_output(output, input)
@@ -203,9 +215,7 @@
     if len(axes) > 0:
         convolve1d(input, weights, axes[0], output, mode, cval, origin)
         for ii in range(1, len(axes)):
             convolve1d(output, weights, axes[ii], output, mode, cval, origin)
     else:
         output[...] = input[...]
     return output
-    
-
```

### Comparing `MedPy-0.4.0/medpy/filter/IntensityRangeStandardization.py` & `MedPy-0.5.0/medpy/filter/IntensityRangeStandardization.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,90 +1,91 @@
 # Copyright (C) 2013 Oskar Maier
-# 
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
-# 
+#
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
-# 
+#
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 # author Oskar Maier
 # version r0.1.2
 # since 2013-09-04
 # status Release
 
 # build-in modules
 
 # third-party modules
 import numpy
-from scipy.interpolate.interpolate import interp1d
+from scipy.interpolate import interp1d
 
 # path changes
 
 # own modules
 
+
 # code
-class IntensityRangeStandardization (object):
+class IntensityRangeStandardization(object):
     r"""
     Class to standardize intensity ranges between a number of images.
-    
+
     **Short description:**
     Often images containing similar objects or scenes have different intensity ranges
     that make it difficult to compare them manually as well as to process them
     further.
-    
+
     IntensityRangeStandardization offers a way to transform a number of such images
     intensity ranges to a common standard intensity space without any loss of
     information using a multi-segment linear transformation model.
-    
+
     Once learned, this model can be applied to other, formerly unseen images to map
-    them to the same standard intensity space.    
-            
+    them to the same standard intensity space.
+
     **Concept of similar images:**
     IntensityRangeStandardization is limited to similar images. Images containing
     different object or different compositions of objects are not suitable to be
     transformed to a common intensity space (and it would furthermore not make much
     sense).
-    
+
     A typical application of IntensityRangeStandardization are MRI images showing the
     same body region. These often have different intensity ranges, even when acquired
     from the same patient and using the same scanner. For further processing, e.g.
     for training a classifier, they have to be mapped to a common intensity space.
-    
+
     **Failure of the transformation:**
     The method implemented in IntensityRangeStandardization ensures that no
     information is lost i.e. a lossless transformation is performed. This can be
     assured when there exists a one-to-one mapping between the images original
     intensity values and their values mapped to the standard intensity space.
-    
+
     But since the transformation model is trained on, and the standard intensity
     space range selected over the training images, this can not be guaranteed for all
     formerly unseen image. If they differ greatly from the training set images, a
     lossless transformation can not be assured anymore. In this case the transform()
     method will throw an InformationLossException.
-    
+
     Should this happen, the model needs to be re-trained with the original training
     images and additionally the images which caused the failure. Since this will lead
     to a new intensity standard space, all already transformed images have to be
     processed again.
-    
+
     **Setting the training parameters:**
     The method comes with a set of default parameters, that are suitable for most
     cases. But for some special cases, it might be better to set them on your own. Ti
     understand the working of the parameters, it is recommended to read the detailed
     method description first.
-    
+
     **The method depends on three parameters:**
-    
+
     cutoffp, i.e. the cut-off percentiles
         These are used to the define the intensity outliers, both during training and
         image transformation. The default values are usualy a good choice.
         (in [1]_ these are called the minimum and maximum percentile values pc1 and pc2 respectively)
     landmarkp, i.e. the landmark percentiles
         These percentiles define the landmark positions. The more supplied, the more
         exact but less general becomes the model. It is common to supply equally
@@ -93,460 +94,511 @@
     strange, i.e. the standard intensity space range
         These two intensity values define roughly the standard intensity space (or
         common intensity space of the images; or even target intensity space) to
         which each images intensities are mapped. This space can be supplied, but it
         is usually recommended to let the method select it automatically during the
         training process. It is additionally possible to supply only the lower or
         upper range border and set the other to ''auto'', in which case the method
-        chooses the range automatically, but not the position. 
+        chooses the range automatically, but not the position.
         (in [1]_ these are called the minimum and maximum intensities on the standard scale of the IOI s1 resp. s2)
-    
-    
+
+
     **Details of the method:**
     In the following the method is described in some more detail. For even more
     information see [1]_.
-         
+
     Essentially the method is based on a multi-segment linear transformation model. A
     standard intensity space (or common intensity space) is defined by an intensity
     value range ''stdrange''.
     During the training phase, the intensity values at certain cut-off percentiles of
     each image are computed and a single-segment linear mapping from them to the
     standard intensity space range limits created. Then the images intensity values
     at a number of landmark percentiles are extracted and passed to the linear
     mapping to be transfered roughly to the standard intensity space. The mean of all
     these mapped landmark intensities form the model learned.
-      
+
     When presented with an image to transform, these images intensity values are
     extracted at the cut-off percentile as well as at the landmark percentile
     positions. This results in a number of segments. Using these and the
     corresponding standard intensity space range values and learned mean landmark
     values, a multi-segment linear transformation model is created for the image.
     This is then applied to the images intensity values to map them to the standard
     intensity space.
-    
+
     Outliers, i.e. the images intensity values that lie outside of the cut-off
     percentiles, are treated separately. They are transformed like the first resp.
     last segmented of the transformation model. Not that this means the transformed
     images intensity values do not always lie inside the standard intensity space
     range, but are fitted as best as possible inside.
-         
+
     Parameters
     ----------
     cutoffp : (float, float)
         Lower and upper cut-off percentiles to exclude outliers.
     landmarkp : sequence of floats
         List of percentiles serving as model landmarks, must lie
         between the cutoffp values.
     stdrange : string or (float, float)
         The range of the standard intensity space for which a
         transformation is learned; when set to 'auto, automatically
         determined from the training image upon training; it is also
         possible to fix either the upper or the lower border value and
         setting the other to 'auto'.
-        
+
     Examples
     --------
     We have a number of similar images with varying intensity ranges. To make them
     comparable, we would like to transform them to a common intensity space. Thus we
     run:
-    
+
         >>> from medpy.filter import IntensityRangeStandardization
         >>> irs = IntensityRangeStandardization()
         >>> trained_model, transformed_images = irs.train_transform(images)
-        
+
     Let us assume we now obtain another, new image, that we would like to make
     comparable to the others. As long as it does not differ to much from these, we
     can simply call:
-        
+
         >>> transformed_image = irs.transform(new_image)
-        
+
     For many application, not all images are already available at the time of
     execution. It would therefore be good to be able to preserve a once trained
     model. The solution is to just pickle the once trained model:
-    
+
         >>> import pickle
         >>> with open('my_trained_model.pkl', 'wb') as f:
         >>>     pickle.dump(irs, f)
-            
+
     And load it again when required with:
-    
+
         >>> with open('my_trained_model.pkl', 'r') as f:
         >>>     irs = pickle.load(f)
-        
+
     References
     ----------
     .. [1] Nyul, L.G.; Udupa, J.K.; Xuan Zhang, "New variants of a method of MRI scale
        standardization," Medical Imaging, IEEE Transactions on , vol.19, no.2, pp.143-150,
        Feb. 2000
-    """    
-    
+    """
+
     # static member variables
     L2 = [50]
     """1-value landmark points model."""
     L3 = [25, 50, 75]
     """3-value landmark points model."""
     L4 = [10, 20, 30, 40, 50, 60, 70, 80, 90]
     """9-value landmark points model."""
-    
-    def __init__(self, cutoffp = (1, 99), landmarkp = L4, stdrange = 'auto'):
+
+    def __init__(self, cutoffp=(1, 99), landmarkp=L4, stdrange="auto"):
         # check parameters
         if not IntensityRangeStandardization.is_sequence(cutoffp):
-            raise ValueError('cutoffp must be a sequence')
+            raise ValueError("cutoffp must be a sequence")
         if not 2 == len(cutoffp):
-            raise ValueError('cutoffp must be of length 2, not {}'.format(len(cutoffp)))
+            raise ValueError("cutoffp must be of length 2, not {}".format(len(cutoffp)))
         if not IntensityRangeStandardization.are_numbers(cutoffp):
-            raise ValueError('cutoffp elements must be numbers')
-        if not IntensityRangeStandardization.are_in_interval(cutoffp, 0, 100, 'included'):
-            raise ValueError('cutoffp elements must be in [0, 100]')
+            raise ValueError("cutoffp elements must be numbers")
+        if not IntensityRangeStandardization.are_in_interval(
+            cutoffp, 0, 100, "included"
+        ):
+            raise ValueError("cutoffp elements must be in [0, 100]")
         if not cutoffp[1] > cutoffp[0]:
-            raise ValueError('the second element of cutoffp must be larger than the first')
-        
+            raise ValueError(
+                "the second element of cutoffp must be larger than the first"
+            )
+
         if not IntensityRangeStandardization.is_sequence(landmarkp):
-            raise ValueError('landmarkp must be a sequence')
+            raise ValueError("landmarkp must be a sequence")
         if not 1 <= len(landmarkp):
-            raise ValueError('landmarkp must be of length >= 1, not {}'.format(len(landmarkp)))
+            raise ValueError(
+                "landmarkp must be of length >= 1, not {}".format(len(landmarkp))
+            )
         if not IntensityRangeStandardization.are_numbers(landmarkp):
-            raise ValueError('landmarkp elements must be numbers')
-        if not IntensityRangeStandardization.are_in_interval(landmarkp, 0, 100, 'included'):
-            raise ValueError('landmarkp elements must be in [0, 100]')
-        if not IntensityRangeStandardization.are_in_interval(landmarkp, cutoffp[0], cutoffp[1], 'excluded'):
-            raise ValueError('landmarkp elements must be in between the elements of cutoffp')
+            raise ValueError("landmarkp elements must be numbers")
+        if not IntensityRangeStandardization.are_in_interval(
+            landmarkp, 0, 100, "included"
+        ):
+            raise ValueError("landmarkp elements must be in [0, 100]")
+        if not IntensityRangeStandardization.are_in_interval(
+            landmarkp, cutoffp[0], cutoffp[1], "excluded"
+        ):
+            raise ValueError(
+                "landmarkp elements must be in between the elements of cutoffp"
+            )
         if not len(landmarkp) == len(numpy.unique(landmarkp)):
-            raise ValueError('landmarkp elements must be unique')
-        
-        if 'auto' == stdrange:
-            stdrange = ('auto', 'auto')
+            raise ValueError("landmarkp elements must be unique")
+
+        if "auto" == stdrange:
+            stdrange = ("auto", "auto")
         else:
             if not IntensityRangeStandardization.is_sequence(stdrange):
-                raise ValueError('stdrange must be a sequence or \'auto\'')
+                raise ValueError("stdrange must be a sequence or 'auto'")
             if not 2 == len(stdrange):
-                raise ValueError('stdrange must be of length 2, not {}'.format(len(stdrange)))
-            if not 'auto' in stdrange:
+                raise ValueError(
+                    "stdrange must be of length 2, not {}".format(len(stdrange))
+                )
+            if not "auto" in stdrange:
                 if not IntensityRangeStandardization.are_numbers(stdrange):
-                    raise ValueError('stdrange elements must be numbers or \'auto\'')
+                    raise ValueError("stdrange elements must be numbers or 'auto'")
                 if not stdrange[1] > stdrange[0]:
-                    raise ValueError('the second element of stdrange must be larger than the first')
-            elif 'auto' == stdrange[0] and not IntensityRangeStandardization.is_number(stdrange[1]):
-                raise ValueError('stdrange elements must be numbers or \'auto\'')
-            elif 'auto' == stdrange[1] and not IntensityRangeStandardization.is_number(stdrange[0]):
-                raise ValueError('stdrange elements must be numbers or \'auto\'')
-                
-        
+                    raise ValueError(
+                        "the second element of stdrange must be larger than the first"
+                    )
+            elif "auto" == stdrange[0] and not IntensityRangeStandardization.is_number(
+                stdrange[1]
+            ):
+                raise ValueError("stdrange elements must be numbers or 'auto'")
+            elif "auto" == stdrange[1] and not IntensityRangeStandardization.is_number(
+                stdrange[0]
+            ):
+                raise ValueError("stdrange elements must be numbers or 'auto'")
+
         # process parameters
         self.__cutoffp = IntensityRangeStandardization.to_float(cutoffp)
         self.__landmarkp = IntensityRangeStandardization.to_float(sorted(landmarkp))
-        self.__stdrange = ['auto' if 'auto' == x else float(x) for x in stdrange]
-            
+        self.__stdrange = ["auto" if "auto" == x else float(x) for x in stdrange]
+
         # initialize remaining instance parameters
         self.__model = None
         self.__sc_umins = None
         self.__sc_umaxs = None
-        
+
     def train(self, images):
         r"""
         Train a standard intensity space and an associated transformation model.
-        
+
         Note that the passed images should be masked to contain only the foreground.
-        
+
         Parameters
         ----------
         images : sequence of array_likes
             A number of images.
-        
+
         Returns
         -------
         IntensityRangeStandardization : IntensityRangeStandardization
             This instance of IntensityRangeStandardization
         """
         self.__stdrange = self.__compute_stdrange(images)
-        
+
         lim = []
         for idx, i in enumerate(images):
             ci = numpy.array(numpy.percentile(i, self.__cutoffp))
             li = numpy.array(numpy.percentile(i, self.__landmarkp))
             ipf = interp1d(ci, self.__stdrange)
             lim.append(ipf(li))
 
-            # treat single intensity accumulation error            
+            # treat single intensity accumulation error
             if not len(numpy.unique(numpy.concatenate((ci, li)))) == len(ci) + len(li):
-                raise SingleIntensityAccumulationError('Image no.{} shows an unusual single-intensity accumulation that leads to a situation where two percentile values are equal. This situation is usually caused, when the background has not been removed from the image. Another possibility would be to reduce the number of landmark percentiles landmarkp or to change their distribution.'.format(idx))
-            
-        self.__model = [self.__stdrange[0]] + list(numpy.mean(lim, 0)) + [self.__stdrange[1]]
-        self.__sc_umins = [self.__stdrange[0]] + list(numpy.min(lim, 0)) + [self.__stdrange[1]]
-        self.__sc_umaxs = [self.__stdrange[0]] + list(numpy.max(lim, 0)) + [self.__stdrange[1]]
-            
+                raise SingleIntensityAccumulationError(
+                    "Image no.{} shows an unusual single-intensity accumulation that leads to a situation where two percentile values are equal. This situation is usually caused, when the background has not been removed from the image. Another possibility would be to reduce the number of landmark percentiles landmarkp or to change their distribution.".format(
+                        idx
+                    )
+                )
+
+        self.__model = (
+            [self.__stdrange[0]] + list(numpy.mean(lim, 0)) + [self.__stdrange[1]]
+        )
+        self.__sc_umins = (
+            [self.__stdrange[0]] + list(numpy.min(lim, 0)) + [self.__stdrange[1]]
+        )
+        self.__sc_umaxs = (
+            [self.__stdrange[0]] + list(numpy.max(lim, 0)) + [self.__stdrange[1]]
+        )
+
         return self
-        
-    def transform(self, image, surpress_mapping_check = False):
+
+    def transform(self, image, surpress_mapping_check=False):
         r"""
         Transform an images intensity values to the learned standard intensity space.
-        
+
         Note that the passed image should be masked to contain only the foreground.
-        
+
         The transformation is guaranteed to be lossless i.e. a one-to-one mapping between
         old and new intensity values exists. In cases where this does not hold, an error
         is thrown. This can be suppressed by setting ``surpress_mapping_check`` to 'True'.
         Do this only if you know what you are doing.
-        
+
         Parameters
         ----------
         image : array_like
             The image to transform.
         surpress_mapping_check : bool
             Whether to ensure a lossless transformation or not.
-        
+
         Returns
         -------
         image : ndarray
             The transformed image
-        
+
         Raises
-        -------
-        InformationLossException 
+        ------
+        InformationLossException
             If a lossless transformation can not be ensured
         Exception
             If no model has been trained before
         """
         if None == self.__model:
-            raise UntrainedException('Model not trained. Call train() first.')
-        
+            raise UntrainedException("Model not trained. Call train() first.")
+
         image = numpy.asarray(image)
-        
+
         # determine image intensity values at cut-off percentiles & landmark percentiles
-        li = numpy.percentile(image, [self.__cutoffp[0]] + self.__landmarkp + [self.__cutoffp[1]])
-        
-        # treat single intensity accumulation error            
+        li = numpy.percentile(
+            image, [self.__cutoffp[0]] + self.__landmarkp + [self.__cutoffp[1]]
+        )
+
+        # treat single intensity accumulation error
         if not len(numpy.unique(li)) == len(li):
-            raise SingleIntensityAccumulationError('The image shows an unusual single-intensity accumulation that leads to a situation where two percentile values are equal. This situation is usually caused, when the background has not been removed from the image. The only other possibility would be to re-train the model with a reduced number of landmark percentiles landmarkp or a changed distribution.')
-        
-        # create linear mapping models for the percentile segments to the learned standard intensity space  
-        ipf = interp1d(li, self.__model, bounds_error = False)
-        
+            raise SingleIntensityAccumulationError(
+                "The image shows an unusual single-intensity accumulation that leads to a situation where two percentile values are equal. This situation is usually caused, when the background has not been removed from the image. The only other possibility would be to re-train the model with a reduced number of landmark percentiles landmarkp or a changed distribution."
+            )
+
+        # create linear mapping models for the percentile segments to the learned standard intensity space
+        ipf = interp1d(li, self.__model, bounds_error=False)
+
         # transform the input image intensity values
         output = ipf(image)
-        
+
         # treat image intensity values outside of the cut-off percentiles range separately
         llm = IntensityRangeStandardization.linear_model(li[:2], self.__model[:2])
         rlm = IntensityRangeStandardization.linear_model(li[-2:], self.__model[-2:])
-        
+
         output[image < li[0]] = llm(image[image < li[0]])
         output[image > li[-1]] = rlm(image[image > li[-1]])
-        
+
         if not surpress_mapping_check and not self.__check_mapping(li):
-            raise InformationLossException('Image can not be transformed to the learned standard intensity space without loss of information. Please re-train.')
-        
+            raise InformationLossException(
+                "Image can not be transformed to the learned standard intensity space without loss of information. Please re-train."
+            )
+
         return output
-    
-    def train_transform(self, images, surpress_mapping_check = False):
+
+    def train_transform(self, images, surpress_mapping_check=False):
         r"""
         See also
         --------
         train, transform
         """
         ret = self.train(images)
         outputs = [self.transform(i, surpress_mapping_check) for i in images]
         return ret, outputs
-    
+
     @property
     def stdrange(self):
         """Get the set resp. learned standard intensity range."""
         return self.__stdrange
-    
+
     @property
     def cutoffp(self):
         """Get the cut-off percentiles."""
         return self.__cutoffp
-    
+
     @property
     def landmarkp(self):
         """Get the landmark percentiles."""
         return self.__landmarkp
-    
+
     @property
     def model(self):
         """Get the model (the learned percentile values)."""
         return self.__model
-    
+
     def __compute_stdrange(self, images):
         r"""
         Computes a common standard intensity range over a number of images.
-        
+
         Depending on the settings of the internal self.__stdrange variable,
         either (1) the already fixed values are returned, (2) a complete standard
         intensity range is computed from the supplied images, (3) an intensity range
         fixed at the lower end or (4) an intensity range fixed at the upper end is
         returned.
-        
+
         Takes into account the maximum length of each percentile segment over all
         images, then adds a security margin defined by the highest variability among
         all segments over all images.
-        
+
         Be
-        
+
         .. math::
-        
+
             L = (cop_l, lp_1, lp_2, ..., lp_n, cop_u)
-        
+
         the set formed by the two cut-off percentiles :math:`cop_l` and :math:`cop_u` and the
         landmark percentiles :math:`lp_1, ..., lp_n`. The corresponding intensity values of
         an image :math:`i\in I` are then
-        
+
         .. math::
-            
+
             V_i = (v_{i,1}, v_{i,2}, ..., v_{i,n+2})
-        
+
         The distance between each of these intensity values forms a segment along the
         images :math:`i` intensity range denoted as
-        
+
         ..math ::
-            
+
             S_i = (s_{i,1}, s_{i,2}, ..., s_{i, n+1})
-        
+
         The common standard intensity range :math:`sir` over the set of images :math:`I` is
         then defined as
-        
+
         ..math ::
             sir = \sum_{l=1}^{n+1}\max_{i=1}^I s_{i,l} * \max_{l=1}^{n+1} \left(\frac{\max_{i=1}^I s_{i,l}}{\min_{i=1}^I s_{i,l}}\right)
-        
+
         Parameters
         ----------
         images : sequence of array_like
             A number of images.
-            
+
         Returns
         -------
         stdrange : (float, float)
             The borders of the computed standard intensity range.
         """
-        if not 'auto' in self.__stdrange:
+        if not "auto" in self.__stdrange:
             return self.__stdrange
-        
+
         copl, copu = self.__cutoffp
-        
-        # collect cutoff + landmark percentile segments and image mean intensity values 
+
+        # collect cutoff + landmark percentile segments and image mean intensity values
         s = []
         m = []
         for idx, i in enumerate(images):
             li = numpy.percentile(i, [copl] + self.__landmarkp + [copu])
-            
+
             s.append(numpy.asarray(li)[1:] - numpy.asarray(li)[:-1])
             m.append(i.mean())
-            
+
             # treat single intensity accumulation error
             if 0 in s[-1]:
-                raise SingleIntensityAccumulationError('Image no.{} shows an unusual single-intensity accumulation that leads to a situation where two percentile values are equal. This situation is usually caused, when the background has not been removed from the image. Another possibility would be to reduce the number of landmark percentiles landmarkp or to change their distribution.'.format(idx))
-            
+                raise SingleIntensityAccumulationError(
+                    "Image no.{} shows an unusual single-intensity accumulation that leads to a situation where two percentile values are equal. This situation is usually caused, when the background has not been removed from the image. Another possibility would be to reduce the number of landmark percentiles landmarkp or to change their distribution.".format(
+                        idx
+                    )
+                )
+
         # select the maximum and minimum of each percentile segment over all images
         maxs = numpy.max(s, 0)
         mins = numpy.min(s, 0)
-        
+
         # divide them pairwise
-        divs = numpy.divide(numpy.asarray(maxs, dtype=numpy.float), mins) 
-        
+        divs = numpy.divide(numpy.asarray(maxs, dtype=float), mins)
+
         # compute interval range according to generalized theorem 2 of [1]
         intv = numpy.sum(maxs) + numpy.max(divs)
-        
+
         # compute mean intensity value over all images (assuming equal size)
         im = numpy.mean(m)
-        
+
         # return interval with borders according to settings
-        if 'auto' == self.__stdrange[0] and 'auto' == self.__stdrange[1]:
+        if "auto" == self.__stdrange[0] and "auto" == self.__stdrange[1]:
             return im - intv / 2, im + intv / 2
-        elif 'auto' == self.__stdrange[0]:
+        elif "auto" == self.__stdrange[0]:
             return self.__stdrange[1] - intv, self.__stdrange[1]
         else:
             return self.__stdrange[0], self.__stdrange[0] + intv
-        
+
     def __check_mapping(self, landmarks):
         """
         Checks whether the image, from which the supplied landmarks were extracted, can
         be transformed to the learned standard intensity space without loss of
         information.
         """
-        sc_udiff = numpy.asarray(self.__sc_umaxs)[1:] - numpy.asarray(self.__sc_umins)[:-1]
+        sc_udiff = (
+            numpy.asarray(self.__sc_umaxs)[1:] - numpy.asarray(self.__sc_umins)[:-1]
+        )
         l_diff = numpy.asarray(landmarks)[1:] - numpy.asarray(landmarks)[:-1]
         return numpy.all(sc_udiff > numpy.asarray(l_diff))
-        
+
     @staticmethod
     def is_sequence(arg):
         """
         Checks via its hidden attribute whether the passed argument is a sequence (but
         excluding strings).
-        
+
         Credits to Steve R. Hastings a.k.a steveha @ http://stackoverflow.com
         """
-        return (not hasattr(arg, "strip") and
-            hasattr(arg, "__getitem__") or
-            hasattr(arg, "__iter__"))
-        
+        return (
+            not hasattr(arg, "strip")
+            and hasattr(arg, "__getitem__")
+            or hasattr(arg, "__iter__")
+        )
+
     @staticmethod
     def is_number(arg):
         """
         Checks whether the passed argument is a valid number or not.
         """
         import numbers
+
         return isinstance(arg, numbers.Number)
-    
+
     @staticmethod
     def are_numbers(arg):
         """
         Checks whether all elements in a sequence are valid numbers.
         """
         return numpy.all([IntensityRangeStandardization.is_number(x) for x in arg])
-    
+
     @staticmethod
-    def is_in_interval(n, l, r, border = 'included'):
+    def is_in_interval(n, l, r, border="included"):
         """
         Checks whether a number is inside the interval l, r.
         """
-        if 'included' == border:
+        if "included" == border:
             return (n >= l) and (n <= r)
-        elif 'excluded' == border:
+        elif "excluded" == border:
             return (n > l) and (n < r)
         else:
-            raise ValueError('borders must be either \'included\' or \'excluded\'')
-        
+            raise ValueError("borders must be either 'included' or 'excluded'")
+
     @staticmethod
-    def are_in_interval(s, l, r, border = 'included'):
+    def are_in_interval(s, l, r, border="included"):
         """
         Checks whether all number in the sequence s lie inside the interval formed by
         l and r.
         """
-        return numpy.all([IntensityRangeStandardization.is_in_interval(x, l, r, border) for x in s])
-    
+        return numpy.all(
+            [IntensityRangeStandardization.is_in_interval(x, l, r, border) for x in s]
+        )
+
     @staticmethod
     def to_float(s):
         """
         Cast a sequences elements to float numbers.
         """
         return [float(x) for x in s]
-    
+
     @staticmethod
     def linear_model(x, y):
         """
         Returns a linear model transformation function fitted on the two supplied points.
         y = m*x + b
         Note: Assumes that slope > 0, otherwise division through zero might occur.
         """
         x1, x2 = x
         y1, y2 = y
         m = (y2 - y1) / (x2 - x1)
         b = y1 - (m * x1)
         return lambda x: m * x + b
-    
+
+
 class SingleIntensityAccumulationError(Exception):
     """
     Thrown when an image shows an unusual single-intensity peaks which would obstruct
     both, training and transformation.
     """
-    
+
+
 class InformationLossException(Exception):
     """
     Thrown when a transformation can not be guaranteed to be lossless.
     """
+
     pass
-    
+
+
 class UntrainedException(Exception):
     """
     Thrown when a transformation is attempted before training.
     """
+
     pass
```

### Comparing `MedPy-0.4.0/medpy/filter/__init__.py` & `MedPy-0.5.0/medpy/filter/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,136 +2,188 @@
 ===================================================
 Image filter and manipulation (:mod:`medpy.filter`)
 ===================================================
 .. currentmodule:: medpy.filter
 
 This package contains various image filters and image
 manipulation functions.
- 
+
 Smoothing :mod:`medpy.filter.smoothing`
 =======================================
 Image smoothing / noise reduction in grayscale images.
 
 .. module:: medpy.filter.smoothing
 .. autosummary::
     :toctree: generated/
-    
+
     anisotropic_diffusion
     gauss_xminus1d
- 
+
 Binary :mod:`medpy.filter.binary`
 =================================
 Binary image manipulation.
 
 .. module:: medpy.filter.binary
 .. autosummary::
     :toctree: generated/
-    
+
     size_threshold
     largest_connected_component
     bounding_box
 
 Image :mod:`medpy.filter.image`
 =================================
 Grayscale image manipulation.
 
 .. module:: medpy.filter.image
 .. autosummary::
     :toctree: generated/
-    
+
     sls
     ssd
     average_filter
     sum_filter
     local_minima
     otsu
     resample
-    
+
 Label :mod:`medpy.filter.label`
 =================================
 Label map manipulation.
 
 .. module:: medpy.filter.label
 .. autosummary::
     :toctree: generated/
-    
+
     relabel_map
     relabel
     relabel_non_zero
     fit_labels_to_mask
-    
+
 Noise :mod:`medpy.filter.noise`
 ===============================
 Global and local noise estimation in grayscale images.
 
 .. module:: medpy.filter.noise
 .. autosummary::
     :toctree: generated/
-    
+
     immerkaer
     immerkaer_local
     separable_convolution
-    
-    
+
+
 Utilities :mod:`medpy.filter.utilities`
 =======================================
 Utilities to apply filters selectively and create your own ones.
 
 .. module:: medpy.filter.utilities
 .. autosummary::
     :toctree: generated/
-    
+
     xminus1d
     intersection
     pad
-    
+
 Hough transform :mod:`medpy.filter.houghtransform`
 ==================================================
 The hough transform shape detection algorithm.
 
 .. module:: medpy.filter.houghtransform
 .. autosummary::
     :toctree: generated/
-    
+
     ght
     ght_alternative
     template_ellipsoid
     template_sphere
-    
+
 Intensity range standardization :mod:`medpy.filter.IntensityRangeStandardization`
 =================================================================================
 A learning method to align the intensity ranges of images.
 
 .. module:: medpy.filter.IntensityRangeStandardization
 .. autosummary::
     :toctree: generated/
-    
+
     IntensityRangeStandardization
 
 """
 
 # Copyright (C) 2013 Oskar Maier
-# 
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
-# 
+#
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
-# 
+#
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-# if __all__ is not set, only the following, explicit import statements are executed
-from .binary import largest_connected_component, size_threshold, bounding_box
-from .image import sls, ssd, average_filter, sum_filter, otsu, local_minima, resample
-from .smoothing import anisotropic_diffusion, gauss_xminus1d
-from .label import fit_labels_to_mask, relabel, relabel_map, relabel_non_zero
-from .houghtransform import ght, ght_alternative, template_ellipsoid, template_sphere
-from .utilities import pad, intersection, xminus1d
-from .IntensityRangeStandardization import IntensityRangeStandardization, UntrainedException, InformationLossException, SingleIntensityAccumulationError
-
-# import all sub-modules in the __all__ variable
-__all__ = [s for s in dir() if not s.startswith('_')]
+from .binary import bounding_box as bounding_box
+from .binary import largest_connected_component as largest_connected_component
+from .binary import size_threshold as size_threshold
+from .houghtransform import ght as ght
+from .houghtransform import ght_alternative as ght_alternative
+from .houghtransform import template_ellipsoid as template_ellipsoid
+from .houghtransform import template_sphere as template_sphere
+from .image import average_filter as average_filter
+from .image import local_minima as local_minima
+from .image import otsu as otsu
+from .image import resample as resample
+from .image import sls as sls
+from .image import ssd as ssd
+from .image import sum_filter as sum_filter
+from .IntensityRangeStandardization import (
+    InformationLossException as InformationLossException,
+)
+from .IntensityRangeStandardization import (
+    IntensityRangeStandardization as IntensityRangeStandardization,
+)
+from .IntensityRangeStandardization import (
+    SingleIntensityAccumulationError as SingleIntensityAccumulationError,
+)
+from .IntensityRangeStandardization import UntrainedException as UntrainedException
+from .label import fit_labels_to_mask as fit_labels_to_mask
+from .label import relabel as relabel
+from .label import relabel_map as relabel_map
+from .label import relabel_non_zero as relabel_non_zero
+from .smoothing import anisotropic_diffusion as anisotropic_diffusion
+from .smoothing import gauss_xminus1d as gauss_xminus1d
+from .utilities import intersection as intersection
+from .utilities import pad as pad
+from .utilities import xminus1d as xminus1d
+
+__all__ = [
+    "largest_connected_component",
+    "size_threshold",
+    "bounding_box",
+    "sls",
+    "ssd",
+    "average_filter",
+    "sum_filter",
+    "otsu",
+    "local_minima",
+    "resample",
+    "anisotropic_diffusion",
+    "gauss_xminus1d",
+    "fit_labels_to_mask",
+    "relabel",
+    "relabel_map",
+    "relabel_non_zero",
+    "ght",
+    "ght_alternative",
+    "template_ellipsoid",
+    "template_sphere",
+    "pad",
+    "intersection",
+    "xminus1d",
+    "IntensityRangeStandardization",
+    "UntrainedException",
+    "InformationLossException",
+    "SingleIntensityAccumulationError",
+]
```

### Comparing `MedPy-0.4.0/medpy/filter/smoothing.py` & `MedPy-0.5.0/medpy/filter/smoothing.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,28 +18,28 @@
 # since 2013-08-23
 # status Release
 
 # build-in modules
 
 # third-party modules
 import numpy
-from scipy.ndimage.filters import gaussian_filter
-
-# path changes
+from scipy.ndimage import gaussian_filter
 
 # own modules
 from .utilities import xminus1d
 
+# path changes
+
 
 # code
 def gauss_xminus1d(img, sigma, dim=2):
     r"""
     Applies a X-1D gauss to a copy of a XD image, slicing it along dim.
 
-    Essentially uses `scipy.ndimage.filters.gaussian_filter`, but
+    Essentially uses `scipy.ndimage.gaussian_filter`, but
     applies it to a dimension less than the image has.
 
     Parameters
     ----------
     img : array_like
         The image to smooth.
     sigma : integer
@@ -51,18 +51,24 @@
     -------
     gauss_xminus1d : ndarray
         The input image ``img`` smoothed by a gaussian kernel along dimension ``dim``.
     """
     img = numpy.array(img, copy=False)
     return xminus1d(img, gaussian_filter, dim, sigma=sigma)
 
-def anisotropic_diffusion(img, niter=1, kappa=50, gamma=0.1, voxelspacing=None, option=1):
+
+def anisotropic_diffusion(
+    img, niter=1, kappa=50, gamma=0.1, voxelspacing=None, option=1
+):
     r"""
     Edge-preserving, XD Anisotropic diffusion.
 
+    To achieve the best effects, the image should be scaled to
+    values between 0 and 1 beforehand.
+
 
     Parameters
     ----------
     img : array_like
         Input image (will be cast to numpy.float).
     niter : integer
         Number of iterations.
@@ -121,49 +127,59 @@
     .. [2] M.J. Black, G. Sapiro, D. Marimont, D. Heeger
        Robust anisotropic diffusion.
        IEEE Transactions on Image Processing,
        7(3):421-432, March 1998.
     """
     # define conduction gradients functions
     if option == 1:
+
         def condgradient(delta, spacing):
-            return numpy.exp(-(delta/kappa)**2.)/float(spacing)
+            return numpy.exp(-((delta / kappa) ** 2.0)) / float(spacing)
+
     elif option == 2:
+
         def condgradient(delta, spacing):
-            return 1./(1.+(delta/kappa)**2.)/float(spacing)
+            return 1.0 / (1.0 + (delta / kappa) ** 2.0) / float(spacing)
+
     elif option == 3:
         kappa_s = kappa * (2**0.5)
 
         def condgradient(delta, spacing):
-            top = 0.5*((1.-(delta/kappa_s)**2.)**2.)/float(spacing)
+            top = 0.5 * ((1.0 - (delta / kappa_s) ** 2.0) ** 2.0) / float(spacing)
             return numpy.where(numpy.abs(delta) <= kappa_s, top, 0)
 
     # initialize output array
     out = numpy.array(img, dtype=numpy.float32, copy=True)
 
     # set default voxel spacing if not supplied
     if voxelspacing is None:
-        voxelspacing = tuple([1.] * img.ndim)
+        voxelspacing = tuple([1.0] * img.ndim)
 
     # initialize some internal variables
     deltas = [numpy.zeros_like(out) for _ in range(out.ndim)]
 
     for _ in range(niter):
-
         # calculate the diffs
         for i in range(out.ndim):
-            slicer = [slice(None, -1) if j == i else slice(None) for j in range(out.ndim)]
-            deltas[i][slicer] = numpy.diff(out, axis=i)
+            slicer = tuple(
+                [slice(None, -1) if j == i else slice(None) for j in range(out.ndim)]
+            )
+            deltas[i][tuple(slicer)] = numpy.diff(out, axis=i)
 
         # update matrices
-        matrices = [condgradient(delta, spacing) * delta for delta, spacing in zip(deltas, voxelspacing)]
+        matrices = [
+            condgradient(delta, spacing) * delta
+            for delta, spacing in zip(deltas, voxelspacing)
+        ]
 
         # subtract a copy that has been shifted ('Up/North/West' in 3D case) by one
         # pixel. Don't as questions. just do it. trust me.
         for i in range(out.ndim):
-            slicer = [slice(1, None) if j == i else slice(None) for j in range(out.ndim)]
-            matrices[i][slicer] = numpy.diff(matrices[i], axis=i)
+            slicer = tuple(
+                [slice(1, None) if j == i else slice(None) for j in range(out.ndim)]
+            )
+            matrices[i][tuple(slicer)] = numpy.diff(matrices[i], axis=i)
 
         # update the image
         out += gamma * (numpy.sum(matrices, axis=0))
 
     return out
```

### Comparing `MedPy-0.4.0/medpy/filter/image.py` & `MedPy-0.5.0/medpy/filter/image.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,46 +1,59 @@
 # Copyright (C) 2013 Oskar Maier
-# 
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
-# 
+#
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
-# 
+#
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 # author Oskar Maier
 # version r0.3.0
 # since 2013-11-29
 # status Release
 
 # build-in modules
 import itertools
-import numbers
 import math
+import numbers
 
 # third-party modules
 import numpy
-from scipy.ndimage.filters import convolve, gaussian_filter, minimum_filter
+from scipy.ndimage import convolve, gaussian_filter, minimum_filter, zoom
 from scipy.ndimage._ni_support import _get_output
-from scipy.ndimage.interpolation import zoom
 
-# own modules
-from .utilities import pad, __make_footprint
 from ..io import header
 
+# own modules
+from .utilities import __make_footprint, pad
+
+
 # code
-def sls(minuend, subtrahend, metric = "ssd", noise = "global", signed = True,
-        sn_size = None, sn_footprint = None, sn_mode = "reflect", sn_cval = 0.0,
-        pn_size = None, pn_footprint = None, pn_mode = "reflect", pn_cval = 0.0):
+def sls(
+    minuend,
+    subtrahend,
+    metric="ssd",
+    noise="global",
+    signed=True,
+    sn_size=None,
+    sn_footprint=None,
+    sn_mode="reflect",
+    sn_cval=0.0,
+    pn_size=None,
+    pn_footprint=None,
+    pn_mode="reflect",
+    pn_cval=0.0,
+):
     r"""
     Computes the signed local similarity between two images.
 
     Compares a patch around each voxel of the minuend array to a number of patches
     centered at the points of a search neighbourhood in the subtrahend. Thus, creates
     a multi-dimensional measure of patch similarity between the minuend and a
     corresponding search area in the subtrahend.
@@ -102,87 +115,120 @@
     pn_mode : {'reflect', 'constant', 'nearest', 'mirror', 'wrap'}, optional
         The `pn_mode` parameter determines how the array borders are
         handled, where `pn_cval` is the value when mode is equal to
         'constant'. Default is 'reflect'
     pn_cval : scalar, optional
         Value to fill past edges of input if `pn_mode` is 'constant'. Default
         is 0.0
-        
+
     Returns
     -------
     sls : ndarray
         The signed local similarity image between subtrahend and minuend.
 
     References
     ----------
-    
+
     .. [1] Mattias P. Heinrich, Mark Jenkinson, Manav Bhushan, Tahreema Matin, Fergus V. Gleeson, Sir Michael Brady, Julia A. Schnabel
            MIND: Modality independent neighbourhood descriptor for multi-modal deformable registration
            Medical Image Analysis, Volume 16, Issue 7, October 2012, Pages 1423-1435, ISSN 1361-8415
            http://dx.doi.org/10.1016/j.media.2012.05.008
     """
     minuend = numpy.asarray(minuend)
     subtrahend = numpy.asarray(subtrahend)
-    
+
     if numpy.iscomplexobj(minuend):
-        raise TypeError('complex type not supported')
+        raise TypeError("complex type not supported")
     if numpy.iscomplexobj(subtrahend):
-        raise TypeError('complex type not supported')  
-    
+        raise TypeError("complex type not supported")
+
     mshape = [ii for ii in minuend.shape if ii > 0]
     sshape = [ii for ii in subtrahend.shape if ii > 0]
     if not len(mshape) == len(sshape):
         raise RuntimeError("minuend and subtrahend must be of same shape")
     if not numpy.all([sm == ss for sm, ss in zip(mshape, sshape)]):
         raise RuntimeError("minuend and subtrahend must be of same shape")
-    
+
     sn_footprint = __make_footprint(minuend, sn_size, sn_footprint)
     sn_fshape = [ii for ii in sn_footprint.shape if ii > 0]
     if len(sn_fshape) != minuend.ndim:
-        raise RuntimeError('search neighbourhood footprint array has incorrect shape.')
-    
+        raise RuntimeError("search neighbourhood footprint array has incorrect shape.")
+
     #!TODO: Is this required?
     if not sn_footprint.flags.contiguous:
         sn_footprint = sn_footprint.copy()
-    
-    # created a padded copy of the subtrahend, whereas the padding mode is always 'reflect'  
+
+    # created a padded copy of the subtrahend, whereas the padding mode is always 'reflect'
     subtrahend = pad(subtrahend, footprint=sn_footprint, mode=sn_mode, cval=sn_cval)
-    
+
     # compute slicers for position where the search neighbourhood sn_footprint is TRUE
-    slicers = [[slice(x, (x + 1) - d if 0 != (x + 1) - d else None) for x in range(d)] for d in sn_fshape]
-    slicers = [sl for sl, tv in zip(itertools.product(*slicers), sn_footprint.flat) if tv]
-    
+    slicers = [
+        [slice(x, (x + 1) - d if 0 != (x + 1) - d else None) for x in range(d)]
+        for d in sn_fshape
+    ]
+    slicers = [
+        sl for sl, tv in zip(itertools.product(*slicers), sn_footprint.flat) if tv
+    ]
+
     # compute difference images and sign images for search neighbourhood elements
-    ssds = [ssd(minuend, subtrahend[slicer], normalized=True, signed=signed, size=pn_size, footprint=pn_footprint, mode=pn_mode, cval=pn_cval) for slicer in slicers]
+    ssds = [
+        ssd(
+            minuend,
+            subtrahend[tuple(slicer)],
+            normalized=True,
+            signed=signed,
+            size=pn_size,
+            footprint=pn_footprint,
+            mode=pn_mode,
+            cval=pn_cval,
+        )
+        for slicer in slicers
+    ]
     distance = [x[0] for x in ssds]
     distance_sign = [x[1] for x in ssds]
 
     # compute local variance, which constitutes an approximation of local noise, out of patch-distances over the neighbourhood structure
     variance = numpy.average(distance, 0)
-    variance = gaussian_filter(variance, sigma=3) #!TODO: Figure out if a fixed sigma is desirable here... I think that yes
-    if 'global' == noise:
-        variance = variance.sum() / float(numpy.product(variance.shape))
+    variance = gaussian_filter(
+        variance, sigma=3
+    )  #!TODO: Figure out if a fixed sigma is desirable here... I think that yes
+    if "global" == noise:
+        variance = variance.sum() / float(numpy.prod(variance.shape))
     # variance[variance < variance_global / 10.] = variance_global / 10. #!TODO: Should I keep this i.e. regularizing the variance to be at least 10% of the global one?
-    
+
     # compute sls
-    sls = [dist_sign * numpy.exp(-1 * (dist / variance)) for dist_sign, dist in zip(distance_sign, distance)]
-    
+    sls = [
+        dist_sign * numpy.exp(-1 * (dist / variance))
+        for dist_sign, dist in zip(distance_sign, distance)
+    ]
+
     # convert into sls image, swapping dimensions to have varying patches in the last dimension
     return numpy.rollaxis(numpy.asarray(sls), 0, minuend.ndim + 1)
 
-def ssd(minuend, subtrahend, normalized=True, signed=False, size=None, footprint=None, mode="reflect", cval=0.0, origin=0):
+
+def ssd(
+    minuend,
+    subtrahend,
+    normalized=True,
+    signed=False,
+    size=None,
+    footprint=None,
+    mode="reflect",
+    cval=0.0,
+    origin=0,
+):
     r"""
     Computes the sum of squared difference (SSD) between patches of minuend and subtrahend.
-    
+
     Parameters
     ----------
     minuend : array_like
         Input array from which to subtract the subtrahend.
     subtrahend : array_like
-        Input array to subtract from the minuend.    
+        Input array to subtract from the minuend.
     normalized : bool, optional
         Whether the SSD of each patch should be divided through the filter size for
         normalization. Default is 'True'.
     signed : bool, optional
         Whether the accumulative sign of each patch should be returned as well. If
         'True', the second return value is a numpy.sign array, otherwise the scalar '1'.
         Default is 'False'.
@@ -203,35 +249,63 @@
     mode : {'reflect', 'constant', 'nearest', 'mirror', 'wrap'}, optional
         The `mode` parameter determines how the array borders are
         handled, where `cval` is the value when mode is equal to
         'constant'. Default is 'reflect'
     cval : scalar, optional
         Value to fill past edges of input if `mode` is 'constant'. Default
         is 0.0
-        
+
     Returns
     -------
     ssd : ndarray
         The patchwise sum of squared differences between minuend and subtrahend.
     """
     convolution_filter = average_filter if normalized else sum_filter
-    output = numpy.float if normalized else minuend.dtype
-    
+    output = float if normalized else minuend.dtype
+
     if signed:
         difference = minuend - subtrahend
         difference_squared = numpy.square(difference)
-        distance_sign = numpy.sign(convolution_filter(numpy.sign(difference) * difference_squared, size=size, footprint=footprint, mode=mode, cval=cval, origin=origin, output=output))
-        distance = convolution_filter(difference_squared, size=size, footprint=footprint, mode=mode, cval=cval, output=output)
+        distance_sign = numpy.sign(
+            convolution_filter(
+                numpy.sign(difference) * difference_squared,
+                size=size,
+                footprint=footprint,
+                mode=mode,
+                cval=cval,
+                origin=origin,
+                output=output,
+            )
+        )
+        distance = convolution_filter(
+            difference_squared,
+            size=size,
+            footprint=footprint,
+            mode=mode,
+            cval=cval,
+            output=output,
+        )
     else:
-        distance = convolution_filter(numpy.square(minuend - subtrahend), size=size, footprint=footprint, mode=mode, cval=cval, origin=origin, output=output)
+        distance = convolution_filter(
+            numpy.square(minuend - subtrahend),
+            size=size,
+            footprint=footprint,
+            mode=mode,
+            cval=cval,
+            origin=origin,
+            output=output,
+        )
         distance_sign = 1
-    
+
     return distance, distance_sign
 
-def average_filter(input, size=None, footprint=None, output=None, mode="reflect", cval=0.0, origin=0):
+
+def average_filter(
+    input, size=None, footprint=None, output=None, mode="reflect", cval=0.0, origin=0
+):
     r"""
     Calculates a multi-dimensional average filter.
 
     Parameters
     ----------
     input : array-like
         input array to filter
@@ -269,26 +343,29 @@
 
     Notes
     -----
     Convenience implementation employing convolve.
 
     See Also
     --------
-    scipy.ndimage.filters.convolve : Convolve an image with a kernel.
+    scipy.ndimage.convolve : Convolve an image with a kernel.
     """
     footprint = __make_footprint(input, size, footprint)
     filter_size = footprint.sum()
-    
+
     output = _get_output(output, input)
-    sum_filter(input, footprint=footprint, output=output, mode=mode, cval=cval, origin=origin)
-    output /= filter_size
-    return output
+    sum_filter(
+        input, footprint=footprint, output=output, mode=mode, cval=cval, origin=origin
+    )
+    return output / filter_size
 
 
-def sum_filter(input, size=None, footprint=None, output=None, mode="reflect", cval=0.0, origin=0):
+def sum_filter(
+    input, size=None, footprint=None, output=None, mode="reflect", cval=0.0, origin=0
+):
     r"""
     Calculates a multi-dimensional sum filter.
 
     Parameters
     ----------
     input : array-like
         input array to filter
@@ -326,142 +403,149 @@
 
     Notes
     -----
     Convenience implementation employing convolve.
 
     See Also
     --------
-    scipy.ndimage.filters.convolve : Convolve an image with a kernel.
+    scipy.ndimage.convolve : Convolve an image with a kernel.
     """
     footprint = __make_footprint(input, size, footprint)
-    slicer = [slice(None, None, -1)] * footprint.ndim 
-    return convolve(input, footprint[slicer], output, mode, cval, origin)
+    slicer = [slice(None, None, -1)] * footprint.ndim
+    return convolve(input, footprint[tuple(slicer)], output, mode, cval, origin)
 
-def otsu (img, bins=64):
+
+def otsu(img, bins=64):
     r"""
     Otsu's method to find the optimal threshold separating an image into fore- and background.
-    
+
     This rather expensive method iterates over a number of thresholds to separate the
     images histogram into two parts with a minimal intra-class variance.
-    
+
     An increase in the number of bins increases the algorithms specificity at the cost of
     slowing it down.
-    
+
     Parameters
     ----------
     img : array_like
         The image for which to determine the threshold.
     bins : integer
         The number of histogram bins.
-        
+
     Returns
     -------
     otsu : float
         The otsu threshold to separate the input image into fore- and background.
     """
     # cast bins parameter to int
     bins = int(bins)
-    
+
     # cast img parameter to scipy arrax
     img = numpy.asarray(img)
-    
+
     # check supplied parameters
     if bins <= 1:
-        raise AttributeError('At least a number two bins have to be provided.')
-    
+        raise AttributeError("At least a number two bins have to be provided.")
+
     # determine initial threshold and threshold step-length
     steplength = (img.max() - img.min()) / float(bins)
     initial_threshold = img.min() + steplength
-    
+
     # initialize best value variables
     best_bcv = 0
     best_threshold = initial_threshold
-    
+
     # iterate over the thresholds and find highest between class variance
     for threshold in numpy.arange(initial_threshold, img.max(), steplength):
-        mask_fg = (img >= threshold)
-        mask_bg = (img < threshold)
-        
+        mask_fg = img >= threshold
+        mask_bg = img < threshold
+
         wfg = numpy.count_nonzero(mask_fg)
         wbg = numpy.count_nonzero(mask_bg)
-        
-        if 0 == wfg or 0 == wbg: continue
-        
+
+        if 0 == wfg or 0 == wbg:
+            continue
+
         mfg = img[mask_fg].mean()
         mbg = img[mask_bg].mean()
-        
+
         bcv = wfg * wbg * math.pow(mbg - mfg, 2)
-        
+
         if bcv > best_bcv:
             best_bcv = bcv
             best_threshold = threshold
-        
+
     return best_threshold
 
-def local_minima(img, min_distance = 4):
+
+def local_minima(img, min_distance=4):
     r"""
     Returns all local minima from an image.
-    
+
     Parameters
     ----------
     img : array_like
         The image.
     min_distance : integer
         The minimal distance between the minimas in voxels. If it is less, only the lower minima is returned.
-    
+
     Returns
     -------
     indices : sequence
         List of all minima indices.
     values : sequence
         List of all minima values.
     """
     # @TODO: Write a unittest for this.
     fits = numpy.asarray(img)
-    minfits = minimum_filter(fits, size=min_distance) # default mode is reflect
+    minfits = minimum_filter(fits, size=min_distance)  # default mode is reflect
     minima_mask = fits == minfits
     good_indices = numpy.transpose(minima_mask.nonzero())
     good_fits = fits[minima_mask]
     order = good_fits.argsort()
     return good_indices[order], good_fits[order]
 
-def resample(img, hdr, target_spacing, bspline_order=3, mode='constant'):
-        """
-        Re-sample an image to a new voxel-spacing.
-        
-        Parameters
-        ----------
-        img : array_like
-            The image.
-        hdr : object
-            The image header.
-        target_spacing : number or sequence of numbers
-            The target voxel spacing to achieve. If a single number, isotropic spacing is assumed.
-        bspline_order : int
-            The bspline order used for interpolation.
-        mode : str
-            Points outside the boundaries of the input are filled according to the given mode ('constant', 'nearest', 'reflect' or 'wrap'). Default is 'constant'.
-            
-        Warning
-        -------
-        Voxel-spacing of input header will be modified in-place!
-            
-        Returns
-        -------
-        img : ndarray
-            The re-sampled image.
-        hdr : object
-            The image header with the new voxel spacing.
-        """
-        if isinstance(target_spacing, numbers.Number):
-            target_spacing = [target_spacing] * img.ndim
-        
-        # compute zoom values
-        zoom_factors = [old / float(new) for new, old in zip(target_spacing, header.get_pixel_spacing(hdr))]
-    
-        # zoom image
-        img = zoom(img, zoom_factors, order=bspline_order, mode=mode)
-        
-        # set new voxel spacing
-        header.set_pixel_spacing(hdr, target_spacing)
-        
-        return img, hdr
+
+def resample(img, hdr, target_spacing, bspline_order=3, mode="constant"):
+    """
+    Re-sample an image to a new voxel-spacing.
+
+    Parameters
+    ----------
+    img : array_like
+        The image.
+    hdr : object
+        The image header.
+    target_spacing : number or sequence of numbers
+        The target voxel spacing to achieve. If a single number, isotropic spacing is assumed.
+    bspline_order : int
+        The bspline order used for interpolation.
+    mode : str
+        Points outside the boundaries of the input are filled according to the given mode ('constant', 'nearest', 'reflect' or 'wrap'). Default is 'constant'.
+
+    Warnings
+    --------
+    Voxel-spacing of input header will be modified in-place!
+
+    Returns
+    -------
+    img : ndarray
+        The re-sampled image.
+    hdr : object
+        The image header with the new voxel spacing.
+    """
+    if isinstance(target_spacing, numbers.Number):
+        target_spacing = [target_spacing] * img.ndim
+
+    # compute zoom values
+    zoom_factors = [
+        old / float(new)
+        for new, old in zip(target_spacing, header.get_pixel_spacing(hdr))
+    ]
+
+    # zoom image
+    img = zoom(img, zoom_factors, order=bspline_order, mode=mode)
+
+    # set new voxel spacing
+    header.set_pixel_spacing(hdr, target_spacing)
+
+    return img, hdr
```

### Comparing `MedPy-0.4.0/medpy/filter/binary.py` & `MedPy-0.5.0/medpy/filter/binary.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,134 +1,140 @@
 # Copyright (C) 2013 Oskar Maier
-# 
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
-# 
+#
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
-# 
+#
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 # author Oskar Maier
 # version r0.2.1
 # since 2013-10-14
 # status Release
 
 # build-in modules
-from operator import  lt, le, gt, ge, ne, eq
+from operator import eq, ge, gt, le, lt, ne
 
 # third-party modules
-import numpy 
-from scipy.ndimage.measurements import label
+import numpy
+from scipy.ndimage import label
 
 # own modules
 
+
 # code
-def size_threshold(img, thr, comp='lt', structure = None):
+def size_threshold(img, thr, comp="lt", structure=None):
     r"""
     Removes binary objects from an image identified by a size threshold.
-    
+
     The unconnected binary objects in an image are identified and all removed
     whose size compares (e.g. less-than) to a supplied threshold value.
-    
+
     The threshold ``thr`` can be any positive integer value. The comparison operator
     can be one of lt, le, gt, ge, ne or eq. The operators used are the functions of
     the same name supplied by the `operator` module of python.
-    
+
     Parameters
     ----------
     img : array_like
-        An array containing connected objects. Will be cast to type numpy.bool.
+        An array containing connected objects. Will be cast to type `bool`.
     thr : int
         Integer defining the threshold size of the binary objects to remove.
     comp : {'lt', 'le', 'gt', 'ge', 'ne', 'eq'}
         The type of comparison to perform. Use e.g. 'lt' for less-than.
     structure : array of ints, optional
         A structuring element that defines feature connections.
         ``structure`` must be symmetric. If no structuring element is provided,
         one is automatically generated with a squared connectivity equal to
         one. That is, for a 2-D ``input`` array, the default structuring element
         is::
-        
+
             [[0,1,0],
              [1,1,1],
              [0,1,0]]
-    
+
     Returns
     -------
     binary_image : ndarray
         The supplied binary image with all objects removed that positively compare
         to the threshold ``thr`` using the comparison operator defined with ``comp``.
-        
+
     Notes
     -----
     If your voxel size is no isotrop i.e. of side-length 1 for all dimensions, simply
     divide the supplied threshold through the real voxel size.
     """
-    
-    operators = {'lt': lt, 'le': le, 'gt': gt, 'ge': ge, 'eq': eq, 'ne': ne}
-    
-    img = numpy.asarray(img).astype(numpy.bool)
+
+    operators = {"lt": lt, "le": le, "gt": gt, "ge": ge, "eq": eq, "ne": ne}
+
+    img = numpy.asarray(img).astype(numpy.bool_)
     if comp not in operators:
         raise ValueError("comp must be one of {}".format(list(operators.keys())))
     comp = operators[comp]
-    
+
     labeled_array, num_features = label(img, structure)
     for oidx in range(1, num_features + 1):
         omask = labeled_array == oidx
         if comp(numpy.count_nonzero(omask), thr):
             img[omask] = False
-            
+
     return img
 
-def largest_connected_component(img, structure = None):
+
+def largest_connected_component(img, structure=None):
     r"""
     Select the largest connected binary component in an image.
-    
+
     Treats all zero values in the input image as background and all others as foreground.
     The return value is an binary array of equal dimensions as the input array with TRUE
     values where the largest connected component is situated.
-    
+
     Parameters
     ----------
     img : array_like
-        An array containing connected objects. Will be cast to type numpy.bool.
+        An array containing connected objects. Will be cast to type `bool`.
     structure : array_like
         A structuring element that defines the connectivity. Structure must be symmetric.
         If no structuring element is provided, one is automatically generated with a
         squared connectivity equal to one.
-    
+
     Returns
     -------
     binary_image : ndarray
         The supplied binary image with only the largest connected component remaining.
-    """   
+    """
     labeled_array, num_features = label(img, structure)
-    component_sizes = [numpy.count_nonzero(labeled_array == label_idx) for label_idx in range(1, num_features + 1)]
+    component_sizes = [
+        numpy.count_nonzero(labeled_array == label_idx)
+        for label_idx in range(1, num_features + 1)
+    ]
     largest_component_idx = numpy.argmax(component_sizes) + 1
 
-    out = numpy.zeros(img.shape, numpy.bool)  
+    out = numpy.zeros(img.shape, numpy.bool_)
     out[labeled_array == largest_component_idx] = True
     return out
 
+
 def bounding_box(img):
     r"""
     Return the bounding box incorporating all non-zero values in the image.
-    
+
     Parameters
     ----------
     img : array_like
         An array containing non-zero objects.
-        
+
     Returns
     -------
     bbox : a list of slicer objects defining the bounding box
     """
     locations = numpy.argwhere(img)
     mins = locations.min(0)
     maxs = locations.max(0) + 1
-    return [slice(x, y) for x, y in zip(mins, maxs)]
+    return tuple([slice(x, y) for x, y in zip(mins, maxs)])
```

### Comparing `MedPy-0.4.0/medpy/filter/houghtransform.py` & `MedPy-0.5.0/medpy/filter/houghtransform.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Copyright (C) 2013 Oskar Maier
-# 
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
-# 
+#
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
-# 
+#
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 # author Oskar Maier
 # version r0.1.2
 # since 2012-06-07
 # status Release
@@ -23,141 +23,152 @@
 
 # third-party modules
 import numpy
 
 # own modules
 from .utilities import pad
 
+
 # public methods
-def ght_alternative (img, template, indices):
+def ght_alternative(img, template, indices):
     """
     Alternative implementation of the general hough transform, which uses iteration over
     indices rather than broadcasting rules like `ght`.
-    
+
     It is therefore considerably slower, especially for large, multi-dimensional arrays.
     The only application are cases, where the hough transform should only be computed for
     a small number of points (=template centers) in the image. In this case the indices
     of interest can be provided as a list.
-    
+
     Parameters
     ----------
     img : array_like
         The image in which to search for the structure.
     template : array_like
         A boolean array containing the structure to search for.
     indices : sequences
         A sequence of image indices at which to compute the hough transform.
-    
+
     Returns
     -------
     hough_transform : ndarray
         The general hough transformation image.
     """
     # cast template to bool and img to numpy array
     img = numpy.asarray(img)
-    template = numpy.asarray(template).astype(numpy.bool)
-    
+    template = numpy.asarray(template).astype(numpy.bool_)
+
     # check supplied parameters
     if img.ndim != template.ndim:
-        raise AttributeError('The supplied image and template must be of the same dimensionality.')
+        raise AttributeError(
+            "The supplied image and template must be of the same dimensionality."
+        )
     if not numpy.all(numpy.greater_equal(img.shape, template.shape)):
-        raise AttributeError('The supplied template is bigger than the image. This setting makes no sense for a hough transform.')
-    
+        raise AttributeError(
+            "The supplied template is bigger than the image. This setting makes no sense for a hough transform."
+        )
+
     # pad the original image
-    img_padded = pad(img, footprint=template, mode='constant')
-    
+    img_padded = pad(img, footprint=template, mode="constant")
+
     # prepare the hough image
-    if numpy.bool == img.dtype:
+    if numpy.bool_ == img.dtype:
         img_hough = numpy.zeros(img.shape, numpy.int32)
     else:
         img_hough = numpy.zeros(img.shape, img.dtype)
-        
+
     # iterate over the pixels, apply the template center to each of these and save the sum into the hough image
     for idx_hough in indices:
         idx_hough = tuple(idx_hough)
         slices_img_padded = [slice(idx_hough[i], None) for i in range(img_hough.ndim)]
-        img_hough[idx_hough] = sum(img_padded[slices_img_padded][template])     
-        
+        img_hough[idx_hough] = sum(img_padded[tuple(slices_img_padded)][template])
+
     return img_hough
 
+
 def ght(img, template):
     r"""
     Implementation of the general hough transform for all dimensions.
-    
+
     Providing a template, this method searches in the image for structures similar to the
     one depicted by the template. The returned hough image denotes how well the structure
     fit in each index.
-    
+
     The indices of the returned image correspond with the centers of the template. At the
     corresponding locations of the original image the template is applied (like a stamp)
     and the underlying voxel values summed up to form the hough images value. It is
     suggested to normalize the input image before for speaking results.
-    
+
     This function behaves as the general hough transform if a binary image has been
     supplied. In the case of a gray-scale image, the values of the pixels under the
     templates structure are summed up, thus weighting becomes possible.
-    
+
     Parameters
     ----------
     img : array_like
         The image in which to search for the structure.
     template : array_like
         A boolean array containing the structure to search for.
-    
+
     Returns
     -------
     hough_transform : ndarray
         The general hough transformation image.
-        
+
     Notes
     -----
     The center of a structure with odd side-length is simple the arrays middle. When an
     even-sided array has been supplied as template, the middle rounded down is taken as
     the structures center. This means that in the second case the hough image is shifted
     by half a voxel (:math:`ndim * [-0.5]`).
-    """    
+    """
     # cast template to bool and img to numpy array
     img = numpy.asarray(img)
-    template = numpy.asarray(template).astype(numpy.bool)
-    
+    template = numpy.asarray(template).astype(numpy.bool_)
+
     # check supplied parameters
     if img.ndim != template.ndim:
-        raise AttributeError('The supplied image and template must be of the same dimensionality.')
+        raise AttributeError(
+            "The supplied image and template must be of the same dimensionality."
+        )
     if not numpy.all(numpy.greater_equal(img.shape, template.shape)):
-        raise AttributeError('The supplied template is bigger than the image. This setting makes no sense for a hough transform.')    
-    
+        raise AttributeError(
+            "The supplied template is bigger than the image. This setting makes no sense for a hough transform."
+        )
+
     # compute center of template array
     center = (numpy.asarray(template.shape) - 1) // 2
-    
+
     # prepare the hough image
-    if numpy.bool == img.dtype:
+    if numpy.bool_ == img.dtype:
         img_hough = numpy.zeros(img.shape, numpy.int32)
     else:
         img_hough = numpy.zeros(img.shape, img.dtype)
-    
-    # iterate over the templates non-zero positions and sum up the images accordingly shifted 
+
+    # iterate over the templates non-zero positions and sum up the images accordingly shifted
     for idx in numpy.transpose(template.nonzero()):
         slicers_hough = []
         slicers_orig = []
         for i in range(img.ndim):
             pos = -1 * (idx[i] - center[i])
-            if 0 == pos: # no shift
+            if 0 == pos:  # no shift
                 slicers_hough.append(slice(None, None))
                 slicers_orig.append(slice(None, None))
-            elif pos > 0: # right shifted hough
+            elif pos > 0:  # right shifted hough
                 slicers_hough.append(slice(pos, None))
                 slicers_orig.append(slice(None, -1 * pos))
-            else: # left shifted hough
+            else:  # left shifted hough
                 slicers_hough.append(slice(None, pos))
                 slicers_orig.append(slice(-1 * pos, None))
-        img_hough[slicers_hough] += img[slicers_orig]
-        
+        img_hough[tuple(slicers_hough)] += img[tuple(slicers_orig)]
+
     return img_hough
 
-def template_sphere (radius, dimensions):
+
+def template_sphere(radius, dimensions):
     r"""
     Returns a spherical binary structure of a of the supplied radius that can be used as
     template input to the generalized hough transform.
 
     Parameters
     ----------
     radius : integer
@@ -167,61 +178,78 @@
 
     Returns
     -------
     template_sphere : ndarray
         A boolean array containing a sphere.
     """
     if int(dimensions) != dimensions:
-        raise TypeError('The supplied dimension parameter must be of type integer.')
+        raise TypeError("The supplied dimension parameter must be of type integer.")
     dimensions = int(dimensions)
-    
+
     return template_ellipsoid(dimensions * [radius * 2])
 
 
 def template_ellipsoid(shape):
     r"""
     Returns an ellipsoid binary structure of a of the supplied radius that can be used as
     template input to the generalized hough transform.
-    
+
     Parameters
     ----------
     shape : tuple of integers
         The main axes of the ellipsoid in voxel units.
-    
+
     Returns
     -------
     template_sphere : ndarray
         A boolean array containing an ellipsoid.
     """
     # prepare template array
-    template = numpy.zeros([int(x // 2 + (x % 2)) for x in shape], dtype=numpy.bool) # in odd shape cases, this will include the ellipses middle line, otherwise not
+    template = numpy.zeros(
+        [int(x // 2 + (x % 2)) for x in shape], dtype=numpy.bool_
+    )  # in odd shape cases, this will include the ellipses middle line, otherwise not
 
     # get real world offset to compute the ellipsoid membership
     rw_offset = []
     for s in shape:
-        if int(s) % 2 == 0: rw_offset.append(0.5 - (s % 2) / 2.) # number before point is even 
-        else: rw_offset.append(-1 * (s % int(s)) / 2.) # number before point is odd 
+        if int(s) % 2 == 0:
+            rw_offset.append(0.5 - (s % 2) / 2.0)  # number before point is even
+        else:
+            rw_offset.append(-1 * (s % int(s)) / 2.0)  # number before point is odd
 
     # prepare an array containing the squares of the half axes to avoid computing inside the loop
-    shape_pow = numpy.power(numpy.asarray(shape) / 2., 2)
+    shape_pow = numpy.power(numpy.asarray(shape) / 2.0, 2)
 
     # we use the ellipse normal form to find all point in its surface as well as volume
     # e.g. for 2D, all voxels inside the ellipse (or on its surface) with half-axes a and b
     #      follow x^2/a^2 + y^2/b^2 <= 1; for higher dimensions accordingly
     # to not have to iterate over each voxel, we make use of the ellipsoids symmetry
     # and construct just a part of the whole ellipse here
     for idx in numpy.ndindex(template.shape):
-        distance = sum((math.pow(coordinate + rwo, 2) / axes_pow for axes_pow, coordinate, rwo in zip(shape_pow, idx, rw_offset))) # plus once since ndarray is zero based, but real-world coordinates not
-        if distance <= 1: template[idx] = True
-        
+        distance = sum(
+            (
+                math.pow(coordinate + rwo, 2) / axes_pow
+                for axes_pow, coordinate, rwo in zip(shape_pow, idx, rw_offset)
+            )
+        )  # plus once since ndarray is zero based, but real-world coordinates not
+        if distance <= 1:
+            template[idx] = True
+
     # we take now our ellipse part and flip it once along each dimension, concatenating it in each step
     # the slicers are constructed to flip in each step the current dimension i.e. to behave like arr[...,::-1,...]
     for i in range(template.ndim):
-        slicers = [(slice(None, None, -1) if i == j else slice(None)) for j in range(template.ndim)]
-        if 0 == int(shape[i]) % 2: # even case
-            template = numpy.concatenate((template[slicers], template), i)
-        else: # odd case, in which an overlap has to be created
-            slicers_truncate = [(slice(None, -1) if i == j else slice(None)) for j in range(template.ndim)]
-            template = numpy.concatenate((template[slicers][slicers_truncate], template), i)
+        slicers = [
+            (slice(None, None, -1) if i == j else slice(None))
+            for j in range(template.ndim)
+        ]
+        if 0 == int(shape[i]) % 2:  # even case
+            template = numpy.concatenate((template[tuple(slicers)], template), i)
+        else:  # odd case, in which an overlap has to be created
+            slicers_truncate = [
+                (slice(None, -1) if i == j else slice(None))
+                for j in range(template.ndim)
+            ]
+            template = numpy.concatenate(
+                (template[tuple(slicers)][tuple(slicers_truncate)], template), i
+            )
 
     return template
-
```

### Comparing `MedPy-0.4.0/medpy/filter/utilities.py` & `MedPy-0.5.0/medpy/filter/utilities.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Copyright (C) 2013 Oskar Maier
-# 
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
-# 
+#
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
-# 
+#
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 # author Oskar Maier
 # version r0.1.3
 # since 2013-12-03
 # status Release
@@ -23,60 +23,62 @@
 # third-party modules
 import numpy
 from scipy.ndimage import _ni_support
 
 # own modules
 from ..io import header
 
+
 # code
 def xminus1d(img, fun, dim, *args, **kwargs):
     r"""
     Applies the function fun along all X-1D dimensional volumes of the images img
     dimension dim.
-    
+
     E.g. you want to apply a gauss filter to each slice of a 3D MRI brain image,
     simply supply the function as fun, the image as img and the dimension along which
     to iterate as dim.
-    
+
     Parameters
     ----------
     img : ndarray
         The image to apply the function ``fun`` to.
     fun : function
         A image modification function.
     dim : integer
         The dimension along which to apply the function.
-    
+
     Returns
     -------
     output : ndarray
         The result of the operation over the image ``img``.
-    
+
     Notes
     -----
     With ``*args`` and ``**kwargs``, arguments can be passed to the function ``fun``.
     """
     slicer = [slice(None)] * img.ndim
     output = []
     for slid in range(img.shape[dim]):
         slicer[dim] = slice(slid, slid + 1)
-        output.append(fun(numpy.squeeze(img[slicer]), *args, **kwargs))
+        output.append(fun(numpy.squeeze(img[tuple(slicer)]), *args, **kwargs))
     return numpy.rollaxis(numpy.asarray(output), 0, dim + 1)
 
+
 #!TODO: Utilise the numpy.pad function that is available since 1.7.0. The numpy version should go inside this function, since it does not support the supplying of a template/footprint on its own.
 def pad(input, size=None, footprint=None, output=None, mode="reflect", cval=0.0):
     r"""
     Returns a copy of the input, padded by the supplied structuring element.
-    
+
     In the case of odd dimensionality, the structure element will be centered as
     following on the currently processed position::
-    
+
         [[T, Tx, T],
          [T, T , T]]
-         
+
     , where Tx denotes the center of the structure element.
 
     Simulates the behaviour of scipy.ndimage filters.
 
     Parameters
     ----------
     input : array_like
@@ -100,25 +102,25 @@
     mode : {'reflect', 'constant', 'nearest', 'mirror', 'wrap'}, optional
         The `mode` parameter determines how the array borders are
         handled, where `cval` is the value when mode is equal to
         'constant'. Default is 'reflect'.
     cval : scalar, optional
         Value to fill past edges of input if `mode` is 'constant'. Default
         is 0.0
-        
+
     Returns
     -------
     output : ndarray
         The padded version of the input image.
-        
+
     Notes
     -----
     Since version 1.7.0, numpy supplied a pad function `numpy.pad` that provides
     the same functionality and should be preferred.
-    
+
     Raises
     ------
     ValueError
         If the provided footprint/size is more than double the image size.
     """
     input = numpy.asarray(input)
     if footprint is None:
@@ -126,126 +128,185 @@
             raise RuntimeError("no footprint or filter size provided")
         sizes = _ni_support._normalize_sequence(size, input.ndim)
         footprint = numpy.ones(sizes, dtype=bool)
     else:
         footprint = numpy.asarray(footprint, dtype=bool)
     fshape = [ii for ii in footprint.shape if ii > 0]
     if len(fshape) != input.ndim:
-        raise RuntimeError('filter footprint array has incorrect shape.')
-    
-    if numpy.any([x > 2*y for x, y in zip(footprint.shape, input.shape)]):
-        raise ValueError('The size of the padding element is not allowed to be more than double the size of the input array in any dimension.')
+        raise RuntimeError("filter footprint array has incorrect shape.")
 
-    padding_offset = [((s - 1) / 2, s / 2) for s in fshape]
+    if numpy.any([x > 2 * y for x, y in zip(footprint.shape, input.shape)]):
+        raise ValueError(
+            "The size of the padding element is not allowed to be more than double the size of the input array in any dimension."
+        )
+
+    padding_offset = [((s - 1) // 2, s // 2) for s in fshape]
     input_slicer = [slice(l, None if 0 == r else -1 * r) for l, r in padding_offset]
     output_shape = [s + sum(os) for s, os in zip(input.shape, padding_offset)]
     output = _ni_support._get_output(output, input, output_shape)
 
-    if 'constant' == mode:
+    if "constant" == mode:
         output += cval
-        output[input_slicer] = input
+        output[tuple(input_slicer)] = input
         return output
-    elif 'nearest' == mode:
-        output[input_slicer] = input
-        dim_mult_slices = [(d, l, slice(None, l), slice(l, l + 1)) for d, (l, _) in zip(list(range(output.ndim)), padding_offset) if not 0 == l]
-        dim_mult_slices.extend([(d, r, slice(-1 * r, None), slice(-2 * r, -2 * r + 1)) for d, (_, r) in zip(list(range(output.ndim)), padding_offset) if not 0 == r])
+    elif "nearest" == mode:
+        output[tuple(input_slicer)] = input
+        dim_mult_slices = [
+            (d, l, slice(None, l), slice(l, l + 1))
+            for d, (l, _) in zip(list(range(output.ndim)), padding_offset)
+            if not 0 == l
+        ]
+        dim_mult_slices.extend(
+            [
+                (d, r, slice(-1 * r, None), slice(-2 * r, -2 * r + 1))
+                for d, (_, r) in zip(list(range(output.ndim)), padding_offset)
+                if not 0 == r
+            ]
+        )
         for dim, mult, to_slice, from_slice in dim_mult_slices:
-            slicer_to = [to_slice if d == dim else slice(None) for d in range(output.ndim)]
-            slicer_from = [from_slice if d == dim else slice(None) for d in range(output.ndim)]
+            slicer_to = [
+                to_slice if d == dim else slice(None) for d in range(output.ndim)
+            ]
+            slicer_from = [
+                from_slice if d == dim else slice(None) for d in range(output.ndim)
+            ]
             if not 0 == mult:
-                output[slicer_to] = numpy.concatenate([output[slicer_from]] * mult, dim)
+                output[tuple(slicer_to)] = numpy.concatenate(
+                    [output[tuple(slicer_from)]] * mult, dim
+                )
         return output
-    elif 'mirror' == mode:
-        dim_slices = [(d, slice(None, l), slice(l + 1, 2 * l + 1)) for d, (l, _) in zip(list(range(output.ndim)), padding_offset) if not 0 == l]
-        dim_slices.extend([(d, slice(-1 * r, None), slice(-2 * r - 1, -1 * r - 1)) for d, (_, r) in zip(list(range(output.ndim)), padding_offset) if not 0 == r])
+    elif "mirror" == mode:
+        dim_slices = [
+            (d, slice(None, l), slice(l + 1, 2 * l + 1))
+            for d, (l, _) in zip(list(range(output.ndim)), padding_offset)
+            if not 0 == l
+        ]
+        dim_slices.extend(
+            [
+                (d, slice(-1 * r, None), slice(-2 * r - 1, -1 * r - 1))
+                for d, (_, r) in zip(list(range(output.ndim)), padding_offset)
+                if not 0 == r
+            ]
+        )
         reverse_slice = slice(None, None, -1)
-    elif 'reflect' == mode:
-        dim_slices = [(d, slice(None, l), slice(l, 2 * l)) for d, (l, _) in zip(list(range(output.ndim)), padding_offset) if not 0 == l]
-        dim_slices.extend([(d, slice(-1 * r, None), slice(-2 * r, -1 * r)) for d, (_, r) in zip(list(range(output.ndim)), padding_offset) if not 0 == r])
+    elif "reflect" == mode:
+        dim_slices = [
+            (d, slice(None, l), slice(l, 2 * l))
+            for d, (l, _) in zip(list(range(output.ndim)), padding_offset)
+            if not 0 == l
+        ]
+        dim_slices.extend(
+            [
+                (d, slice(-1 * r, None), slice(-2 * r, -1 * r))
+                for d, (_, r) in zip(list(range(output.ndim)), padding_offset)
+                if not 0 == r
+            ]
+        )
         reverse_slice = slice(None, None, -1)
-    elif 'wrap' == mode:
-        dim_slices = [(d, slice(None, l), slice(-1 * (l + r), -1 * r if not 0 == r else None)) for d, (l, r) in zip(list(range(output.ndim)), padding_offset) if not 0 == l]
-        dim_slices.extend([(d, slice(-1 * r, None), slice(l, r + l)) for d, (l, r) in zip(list(range(output.ndim)), padding_offset) if not 0 == r])
+    elif "wrap" == mode:
+        dim_slices = [
+            (d, slice(None, l), slice(-1 * (l + r), -1 * r if not 0 == r else None))
+            for d, (l, r) in zip(list(range(output.ndim)), padding_offset)
+            if not 0 == l
+        ]
+        dim_slices.extend(
+            [
+                (d, slice(-1 * r, None), slice(l, r + l))
+                for d, (l, r) in zip(list(range(output.ndim)), padding_offset)
+                if not 0 == r
+            ]
+        )
         reverse_slice = slice(None)
     else:
-        raise RuntimeError('boundary mode not supported')
-    
-    output[input_slicer] = input
+        raise RuntimeError("boundary mode not supported")
+
+    output[tuple(input_slicer)] = input
     for dim, to_slice, from_slice in dim_slices:
-        slicer_reverse = [reverse_slice if d == dim else slice(None) for d in range(output.ndim)]
+        slicer_reverse = [
+            reverse_slice if d == dim else slice(None) for d in range(output.ndim)
+        ]
         slicer_to = [to_slice if d == dim else slice(None) for d in range(output.ndim)]
-        slicer_from = [from_slice if d == dim else slice(None) for d in range(output.ndim)]
-        output[slicer_to] = output[slicer_from][slicer_reverse]
+        slicer_from = [
+            from_slice if d == dim else slice(None) for d in range(output.ndim)
+        ]
+        output[tuple(slicer_to)] = output[tuple(slicer_from)][tuple(slicer_reverse)]
 
     return output
 
+
 def intersection(i1, h1, i2, h2):
-        r"""
-        Returns the intersecting parts of two images in real world coordinates.
-        Takes both, voxelspacing and image offset into account.
-        
-        Note that the returned new offset might be inaccurate up to 1/2 voxel size for
-        each dimension due to averaging.
-        
-        Parameters
-        ----------
-        i1 : array_like
-        i2 : array_like
-            The two images.
-        h1 : MedPy image header
-        h2 : MedPy image header
-            The corresponding headers.
-            
-        Returns
-        -------
-        v1 : ndarray
-            The intersecting part of ``i1``.
-        v2 : ndarray
-            The intersecting part of ``i2``.
-        offset : tuple of floats
-            The new offset of ``v1`` and ``v2`` in real world coordinates.
-        """
-        
-        # compute image bounding boxes in real-world coordinates
-        os1 = numpy.asarray(header.get_offset(h1))
-        ps1 = numpy.asarray(header.get_pixel_spacing(h1))
-        bb1 = (os1, numpy.asarray(i1.shape) * ps1 + os1)
-        
-        
-        os2 = numpy.asarray(header.get_offset(h2))
-        ps2 = numpy.asarray(header.get_pixel_spacing(h2))
-        bb2 = (os2, numpy.asarray(i2.shape) * ps2 + os2)
-        
-        # compute intersection
-        ib = (numpy.maximum(bb1[0], bb2[0]), numpy.minimum(bb1[1], bb2[1]))
-        
-        # transfer intersection to respective image coordinates image
-        ib1 = [ ((ib[0] - os1) / numpy.asarray(ps1)).astype(numpy.int), ((ib[1] - os1) / numpy.asarray(ps1)).astype(numpy.int) ]
-        ib2 = [ ((ib[0] - os2) / numpy.asarray(ps2)).astype(numpy.int), ((ib[1] - os2) / numpy.asarray(ps2)).astype(numpy.int) ]
-        
-        # ensure that both sub-volumes are of same size (might be affected by rounding errors); only reduction allowed
-        s1 = ib1[1] - ib1[0]
-        s2 = ib2[1] - ib2[0]
-        d1 = s1 - s2
-        d1[d1 > 0] = 0
-        d2 = s2 - s1
-        d2[d2 > 0] = 0
-        ib1[1] -= d1
-        ib2[1] -= d2
-        
-        # compute new image offsets (in real-world coordinates); averaged to account for rounding errors due to world-to-voxel mapping
-        nos1 = ib1[0] * ps1 + os1 # real offset for image 1
-        nos2 = ib2[0] * ps2 + os2 # real offset for image 2
-        nos = numpy.average([nos1, nos2], 0)
-        
-        # build slice lists
-        sl1 = [slice(l, u) for l, u in zip(*ib1)]
-        sl2 = [slice(l, u) for l, u in zip(*ib2)]
-        
-        return i1[sl1], i2[sl2], nos
+    r"""
+    Returns the intersecting parts of two images in real world coordinates.
+    Takes both, voxelspacing and image offset into account.
+
+    Note that the returned new offset might be inaccurate up to 1/2 voxel size for
+    each dimension due to averaging.
+
+    Parameters
+    ----------
+    i1 : array_like
+    i2 : array_like
+        The two images.
+    h1 : MedPy image header
+    h2 : MedPy image header
+        The corresponding headers.
+
+    Returns
+    -------
+    v1 : ndarray
+        The intersecting part of ``i1``.
+    v2 : ndarray
+        The intersecting part of ``i2``.
+    offset : tuple of floats
+        The new offset of ``v1`` and ``v2`` in real world coordinates.
+    """
+
+    # compute image bounding boxes in real-world coordinates
+    os1 = numpy.asarray(header.get_offset(h1))
+    ps1 = numpy.asarray(header.get_pixel_spacing(h1))
+    bb1 = (os1, numpy.asarray(i1.shape) * ps1 + os1)
+
+    os2 = numpy.asarray(header.get_offset(h2))
+    ps2 = numpy.asarray(header.get_pixel_spacing(h2))
+    bb2 = (os2, numpy.asarray(i2.shape) * ps2 + os2)
+
+    # compute intersection
+    ib = (numpy.maximum(bb1[0], bb2[0]), numpy.minimum(bb1[1], bb2[1]))
+
+    # transfer intersection to respective image coordinates image
+    ib1 = [
+        ((ib[0] - os1) / numpy.asarray(ps1)).astype(int),
+        ((ib[1] - os1) / numpy.asarray(ps1)).astype(int),
+    ]
+    ib2 = [
+        ((ib[0] - os2) / numpy.asarray(ps2)).astype(int),
+        ((ib[1] - os2) / numpy.asarray(ps2)).astype(int),
+    ]
+
+    # ensure that both sub-volumes are of same size (might be affected by rounding errors); only reduction allowed
+    s1 = ib1[1] - ib1[0]
+    s2 = ib2[1] - ib2[0]
+    d1 = s1 - s2
+    d1[d1 > 0] = 0
+    d2 = s2 - s1
+    d2[d2 > 0] = 0
+    ib1[1] -= d1
+    ib2[1] -= d2
+
+    # compute new image offsets (in real-world coordinates); averaged to account for rounding errors due to world-to-voxel mapping
+    nos1 = ib1[0] * ps1 + os1  # real offset for image 1
+    nos2 = ib2[0] * ps2 + os2  # real offset for image 2
+    nos = numpy.average([nos1, nos2], 0)
+
+    # build slice lists
+    sl1 = [slice(l, u) for l, u in zip(*ib1)]
+    sl2 = [slice(l, u) for l, u in zip(*ib2)]
+
+    return i1[tuple(sl1)], i2[tuple(sl2)], nos
+
 
 def __make_footprint(input, size, footprint):
     "Creates a standard footprint element ala scipy.ndimage."
     if footprint is None:
         if size is None:
             raise RuntimeError("no footprint or filter size provided")
         sizes = _ni_support._normalize_sequence(size, input.ndim)
```

### Comparing `MedPy-0.4.0/medpy/filter/label.py` & `MedPy-0.5.0/medpy/filter/label.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,193 +1,203 @@
 # Copyright (C) 2013 Oskar Maier
-# 
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
-# 
+#
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
-# 
+#
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 # author Oskar Maier
 # version r0.1.1
 # since 2012-02-07
 # status Development
 
 # build-in modules
 
 # third-party modules
-import scipy
+import numpy
 
 # own modules
-from ..core.exceptions import ArgumentError
+from ..core import ArgumentError
+
 
 # code
 def relabel_map(label_image, mapping, key=lambda x, y: x[y]):
     r"""
     Relabel an image using the supplied mapping.
-    
+
     The ``mapping`` can be any kind of subscriptable object. The respective region id is used
     to access the new value from the ``mapping``. The ``key`` keyword parameter can be used to
     supply another access function. The ``key`` function must have the signature
     key(mapping, region-id) and return the new region-id to assign.
-    
+
     Parameters
     ----------
     label_image : array_like
         A nD label map.
     mapping : dictionary or subscriptable object
         A mapping object.
     key : function
         Can be used to defined the key-access to the ``mapping`` object.
-    
+
     Returns
     -------
     relabel_map : ndarray
         A label map with new region ids.
-    
+
     Raises
     ------
     ArgumentError
         If a region id is missing in the supplied mapping
-    """    
-    label_image = scipy.array(label_image)
-    
+    """
+    label_image = numpy.array(label_image)
+
     def _map(x):
         try:
             return key(mapping, x)
         except Exception as e:
-            raise ArgumentError('No conversion for region id {} found in the supplied mapping. Error: {}'.format(x, e))
-    
-    vmap = scipy.vectorize(_map, otypes=[label_image.dtype])
-         
+            raise ArgumentError(
+                "No conversion for region id {} found in the supplied mapping. Error: {}".format(
+                    x, e
+                )
+            )
+
+    vmap = numpy.vectorize(_map, otypes=[label_image.dtype])
+
     return vmap(label_image)
 
-def relabel(label_image, start = 1):
+
+def relabel(label_image, start=1):
     r"""
     Relabel the regions of a label image.
     Re-processes the labels to make them consecutively and starting from start.
-    
+
     Parameters
     ----------
     label_image : array_like
         A nD label map.
     start : integer
         The id of the first label to assign
-    
+
     Returns
     -------
     relabel_map : ndarray
         The relabelled label map.
-        
+
     See also
     --------
     relabel_non_zero
     """
-    label_image = scipy.asarray(label_image)
+    label_image = numpy.asarray(label_image)
     mapping = {}
     rav = label_image.ravel()
     for i in range(len(rav)):
         if not rav[i] in mapping:
             mapping[rav[i]] = start
             start += 1
         rav[i] = mapping[rav[i]]
     return rav.reshape(label_image.shape)
 
-def relabel_non_zero(label_image, start = 1):
-    r""" 
+
+def relabel_non_zero(label_image, start=1):
+    r"""
     Relabel the regions of a label image.
     Re-processes the labels to make them consecutively and starting from start.
     Keeps all zero (0) labels, as they are considered background.
-    
+
     Parameters
     ----------
     label_image : array_like
         A nD label map.
     start : integer
         The id of the first label to assign
-    
+
     Returns
     -------
     relabel_map : ndarray
         The relabelled label map.
-        
+
     See also
     --------
-    relabel  
+    relabel
     """
-    if start <= 0: raise ArgumentError('The starting value can not be 0 or lower.')
-    
-    l = list(scipy.unique(label_image))
-    if 0 in l: l.remove(0)
+    if start <= 0:
+        raise ArgumentError("The starting value can not be 0 or lower.")
+
+    l = list(numpy.unique(label_image))
+    if 0 in l:
+        l.remove(0)
     mapping = dict()
     mapping[0] = 0
     for key, item in zip(l, list(range(start, len(l) + start))):
         mapping[key] = item
-    
+
     return relabel_map(label_image, mapping)
 
 
 def fit_labels_to_mask(label_image, mask):
     r"""
     Reduces a label images by overlaying it with a binary mask and assign the labels
     either to the mask or to the background. The resulting binary mask is the nearest
     expression the label image can form of the supplied binary mask.
-    
+
     Parameters
     ----------
     label_image : array_like
         A nD label map.
     mask : array_like
         A mask image, i.e., a binary image with False for background and True for foreground.
-        
+
     Returns
     -------
     best_fit : ndarray
         The best fit of the labels to the mask.
-    
+
     Raises
-    ------         
+    ------
     ValueError
         If ``label_image`` and ``mask`` are not of the same shape.
     """
-    label_image = scipy.asarray(label_image)
-    mask = scipy.asarray(mask, dtype=scipy.bool_)
+    label_image = numpy.asarray(label_image)
+    mask = numpy.asarray(mask, dtype=numpy.bool_)
 
     if label_image.shape != mask.shape:
-        raise ValueError('The input images must be of the same shape.')
-    
+        raise ValueError("The input images must be of the same shape.")
+
     # prepare collection dictionaries
-    labels = scipy.unique(label_image)
+    labels = numpy.unique(label_image)
     collection = {}
     for label in labels:
         collection[label] = [0, 0, []]  # size, union, points
-    
+
     # iterate over the label images pixels and collect position, size and union
     for x in range(label_image.shape[0]):
         for y in range(label_image.shape[1]):
             for z in range(label_image.shape[2]):
-                entry = collection[label_image[x,y,z]]
+                entry = collection[label_image[x, y, z]]
                 entry[0] += 1
-                if mask[x,y,z]: entry[1] += 1
-                entry[2].append((x,y,z))
-                
+                if mask[x, y, z]:
+                    entry[1] += 1
+                entry[2].append((x, y, z))
+
     # select labels that are more than half in the mask
     for label in labels:
-        if collection[label][0] / 2. >= collection[label][1]:
+        if collection[label][0] / 2.0 >= collection[label][1]:
             del collection[label]
-                
+
     # image_result = numpy.zeros_like(mask) this is eq. to mask.copy().fill(0), which directly applied does not allow access to the rows and colums: Why?
     image_result = mask.copy()
-    image_result.fill(False)         
+    image_result.fill(False)
 
     # add labels to result mask
     for label, data in list(collection.items()):
         for point in data[2]:
             image_result[point] = True
-            
+
     return image_result
```

### Comparing `MedPy-0.4.0/medpy/io/save.py` & `MedPy-0.5.0/medpy/io/save.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Copyright (C) 2013 Oskar Maier
-# 
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
-# 
+#
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
-# 
+#
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 # author Oskar Maier
 # version r0.2.1
 # since 2012-05-28
 # status Release
@@ -22,41 +22,41 @@
 import os
 
 # third-party modules
 import numpy as np
 import SimpleITK as sitk
 
 # own modules
-from ..core import Logger
-from ..core import ImageSavingError
+from ..core import ImageSavingError, Logger
+
 
 # code
-def save(arr, filename, hdr = False, force = True, use_compression = False):
+def save(arr, filename, hdr=False, force=True, use_compression=False):
     r"""
     Save the image ``arr`` as filename using information encoded in ``hdr``. The target image
     format is determined by the ``filename`` suffix. If the ``force`` parameter is set to true,
     an already existing image is overwritten silently. Otherwise an error is thrown.
-    
+
     The header (``hdr``) object is the one returned by `~medpy.io.load.load` and is used
     opportunistically, possibly loosing some meta-information.
-    
+
     Generally this function does not guarantee, that metadata other than the image shape
     and pixel data type are kept.
-    
+
     MedPy relies on SimpleITK, which enables the power of ITK for image loading and saving.
     The supported image file formats should include at least the following.
 
     Medical formats:
-    
+
     - ITK MetaImage (.mha/.raw, .mhd)
     - Neuroimaging Informatics Technology Initiative (NIfTI) (.nia, .nii, .nii.gz, .hdr, .img, .img.gz)
     - Analyze (plain, SPM99, SPM2) (.hdr/.img, .img.gz)
     - Digital Imaging and Communications in Medicine (DICOM) (.dcm, .dicom)
     - Digital Imaging and Communications in Medicine (DICOM) series (<directory>/)
-    - Nearly Raw Raster Data (Nrrd) (.nrrd, .nhdr) 
+    - Nearly Raw Raster Data (Nrrd) (.nrrd, .nhdr)
     - Medical Imaging NetCDF (MINC) (.mnc, .MNC)
     - Guys Image Processing Lab (GIPL) (.gipl, .gipl.gz)
 
     Microscopy formats:
 
     - Medical Research Council (MRC) (.mrc, .rec)
     - Bio-Rad (.pic, .PIC)
@@ -71,50 +71,54 @@
 
     - Portable Network Graphics (PNG) (.png, .PNG)
     - Joint Photographic Experts Group (JPEG) (.jpg, .JPG, .jpeg, .JPEG)
     - Tagged Image File Format (TIFF) (.tif, .TIF, .tiff, .TIFF)
     - Windows bitmap (.bmp, .BMP)
     - Hierarchical Data Format (HDF5) (.h5 , .hdf5 , .he5)
     - MSX-DOS Screen-x (.ge4, .ge5)
-        
+
     For informations about which image formats, dimensionalities and pixel data types
     your current configuration supports, run `python3 tests/support.py > myformats.log`.
-          
+
     Further information see https://simpleitk.readthedocs.io .
-                
+
     Parameters
     ----------
     arr : array_like
         The image data with order `x,y,z,c`.
     filename : string
         Where to save the image; path and filename including the image suffix.
     hdr : object
         The image header containing the metadata.
     force : bool
         Set to True to overwrite already exiting image silently.
     use_compression : bool
         Use data compression of the target format supports it.
-    
+
     Raises
     ------
     ImageSavingError
         If the image could not be saved due to various reasons
     """
     logger = Logger.getInstance()
-    logger.info('Saving image as {}...'.format(filename))
-    
+    logger.info("Saving image as {}...".format(filename))
+
     # Check image file existance
     if not force and os.path.exists(filename):
-        raise ImageSavingError('The target file {} already exists.'.format(filename))
-    
+        raise ImageSavingError("The target file {} already exists.".format(filename))
+
     # Roll axes from x,y,z,c to z,y,x,c
     if arr.ndim == 4:
         arr = np.moveaxis(arr, -1, 0)
     arr = arr.T
 
+    # treat unsupported dtypes
+    if arr.dtype == bool:
+        arr = arr.astype(np.uint8)
+
     sitkimage = sitk.GetImageFromArray(arr)
-  
+
     # Copy met-data as far as possible
     if hdr:
         hdr.copy_to(sitkimage)
-        
+
     sitk.WriteImage(sitkimage, filename, use_compression)
```

### Comparing `MedPy-0.4.0/medpy/io/header.py` & `MedPy-0.5.0/medpy/io/header.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Copyright (C) 2013 Oskar Maier
-# 
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
-# 
+#
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
-# 
+#
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 # author Oskar Maier
 # version r0.2.3
 # since 2012-06-01
 # status Release
@@ -23,97 +23,109 @@
 
 # third-party modules
 import numpy as np
 
 # own modules
 from ..core import Logger
 
+
 # code
 def get_voxel_spacing(hdr):
     r"""
     Extracts the voxel spacing from an image header.
 
     Notes
     -----
     It is recommended to call `hdr.get_voxel_spacing()` instead
     of this function.
-    
+
     Parameters
     ----------
     hdr : medpy.io.Header
         An image header as returned by `load`.
-    
+
     Returns
     -------
     pixel_spacing : tuple of floats
         The image's pixel spacing.
     """
     return hdr.get_voxel_spacing()
 
+
 def get_pixel_spacing(hdr):
     r"""Depreciated synonym of `~medpy.io.header.get_voxel_spacing`."""
-    warnings.warn('get_pixel_spacing() is depreciated, use set_voxel_spacing() instead', category=DeprecationWarning)
+    warnings.warn(
+        "get_pixel_spacing() is depreciated, use get_voxel_spacing() instead",
+        category=DeprecationWarning,
+    )
     return get_voxel_spacing(hdr)
 
+
 def get_offset(hdr):
     r"""
     Extracts the image offset (akak origin) from an image header.
 
     Notes
     -----
     It is recommended to call `hdr.get_offset()` instead
     of this function.
     It can be assumed that the offset is measured from the center point of
     the first pixel, which SimpleITK promises independent of the file format.
     Some formats do not specify a header field for the offset, thus zeros
     are returned.
-    
+
     Parameters
     ----------
     hdr : medpy.io.Header
         An image header as returned by `load`.
-    
+
     Returns
     -------
     offset : tuple of floats
         The image's offset.
     """
     return hdr.get_offset()
 
+
 def set_voxel_spacing(hdr, spacing):
     r"""
     Sets the voxel spacing in an image header.
-    
+
     Notes
     -----
     It is recommended to call `hdr.set_voxel_spacing()` instead
-    of this function.    
+    of this function.
 
     Parameters
     ----------
     hdr : medpy.io.Header
         An image header as returned by `load`.
     pixel_spacing : tuple of floats
         The desired pixel spacing.
     """
     hdr.set_voxel_spacing(spacing)
 
+
 def set_pixel_spacing(hdr, spacing):
     r"""Depreciated synonym of `~medpy.io.header.set_voxel_spacing`."""
-    warnings.warn('get_pixel_spacing() is depreciated, use set_voxel_spacing() instead', category=DeprecationWarning)
+    warnings.warn(
+        "get_pixel_spacing() is depreciated, use set_voxel_spacing() instead",
+        category=DeprecationWarning,
+    )
     set_voxel_spacing(hdr, spacing)
-   
+
+
 def set_offset(hdr, offset):
     r"""
     Sets the offset (aka origin) in the image header.
-    
+
     Notes
     -----
     It is recommended to call `hdr.set_offset()` instead
-    of this function.    
+    of this function.
     The offset is based on the center of the first voxel.
     See also `get_offset` for more details.
 
     Parameters
     ----------
     hdr : medpy.io.Header
         An image header as returned by `load`.
@@ -122,86 +134,98 @@
     """
     hdr.set_offset(offset)
 
 
 def copy_meta_data(hdr_to, hdr_from):
     r"""
     Copy image meta data (voxel spacing and offset) from one header to another.
-    
+
     Parameters
     ----------
     hdr_to : object
         An image header as returned by `load`.
     hdr_from : object
         An image header as returned by `load`.
     """
-    warnings.warn('copy_meta_data() is depreciated and may be removed in future versions', category=DeprecationWarning)
+    warnings.warn(
+        "copy_meta_data() is depreciated and may be removed in future versions",
+        category=DeprecationWarning,
+    )
     logger = Logger.getInstance()
     try:
         set_pixel_spacing(hdr_to, get_pixel_spacing(hdr_from))
     except AttributeError as e:
-        logger.warning('The voxel spacing could not be set correctly. Signaled error: {}'.format(e))
+        logger.warning(
+            "The voxel spacing could not be set correctly. Signaled error: {}".format(e)
+        )
     try:
         set_offset(hdr_to, get_offset(hdr_from))
     except AttributeError as e:
-        logger.warning('The image offset could not be set correctly. Signaled error: {}'.format(e))
+        logger.warning(
+            "The image offset could not be set correctly. Signaled error: {}".format(e)
+        )
 
 
 class Header:
     r"""
     A medpy header object.
 
     Stores spacing, offset/origin, direction, and possibly further meta information.
     Provide at least one of the parameters. Missing information is extracted from
-    the ``sitkimage`` or, if not supplied, set to a default value. 
+    the ``sitkimage`` or, if not supplied, set to a default value.
 
     Parameters
     ----------
     spacing : tuple of floats
         the image's voxel spacing
-        defaults to a tuple of `1.0`s
+        defaults to a tuple of 1.0s
     offset : tuple of floats
         the image's offset/origin
-        defaults to a tuple of `0.0`s
+        defaults to a tuple of 0.0s
     direction : ndarray
         the image's affine transformation matrix
         must be of square shape
         default to the identity matrix
     sitkimage : sitk.Image
         the simple itk image as loaded
     """
 
     def __init__(self, spacing=None, offset=None, direction=None, sitkimage=None):
-        assert \
-            sitkimage is not None or \
-            spacing is not None or \
-            offset is not None or \
-            direction is not None
+        assert (
+            sitkimage is not None
+            or spacing is not None
+            or offset is not None
+            or direction is not None
+        )
 
         # determin the image's ndim and default data types
         if direction is not None:
             direction = np.asarray(direction)
             ndim = len(direction.shape[0])
         elif offset is not None:
             offset = tuple(offset)
             ndim = len(offset)
         elif spacing is not None:
             spacing = tuple(spacing)
             ndim = len(spacing)
         else:
             ndim = len(sitkimage.GetSpacing())
-        
+
         # set missing information to extracted or default values
         if spacing is None:
-            spacing = sitkimage.GetSpacing() if sitkimage is not None else (1.0, ) * ndim
+            spacing = sitkimage.GetSpacing() if sitkimage is not None else (1.0,) * ndim
         if offset is None:
-            offset = sitkimage.GetOrigin() if sitkimage is not None else (0.0, ) * ndim
+            offset = sitkimage.GetOrigin() if sitkimage is not None else (0.0,) * ndim
         if direction is None:
-            direction = np.asarray(sitkimage.GetDirection()).reshape(ndim, ndim) if sitkimage is not None else np.identity(ndim)
-            
+            direction = (
+                np.asarray(sitkimage.GetDirection()).reshape(ndim, ndim)
+                if sitkimage is not None
+                else np.identity(ndim)
+            )
+
         # assert consistency
         assert len(spacing) == len(offset)
         assert direction.ndim == 2
         assert len(spacing) == direction.shape[0]
         assert direction.shape[0] == direction.shape[1]
 
         # set members
@@ -230,70 +254,72 @@
         """
         if self.sitkimage is not None:
             for k in self.sitkimage.GetMetaDataKeys():
                 sitkimage.SetMetaData(k, self.sitkimage.GetMetaData(k))
 
         ndim = len(sitkimage.GetSize())
         spacing, offset, direction = self.get_info_consistent(ndim)
-            
+
         sitkimage.SetSpacing(spacing)
         sitkimage.SetOrigin(offset)
         sitkimage.SetDirection(tuple(direction.flatten()))
-        
+
         return sitkimage
-        
+
     def get_info_consistent(self, ndim):
         """
         Returns the main meta-data information adapted to the supplied
         image dimensionality.
 
         It will try to resolve inconsistencies and other conflicts,
         altering the information avilable int he most plausible way.
 
         Parameters
         ----------
         ndim : int
             image's dimensionality
-        
+
         Returns
         -------
         spacing : tuple of floats
         offset : tuple of floats
         direction : ndarray
         """
         if ndim > len(self.spacing):
-            spacing = self.spacing + (1.0, ) * (ndim - len(self.spacing))
+            spacing = self.spacing + (1.0,) * (ndim - len(self.spacing))
         else:
             spacing = self.spacing[:ndim]
 
         if ndim > len(self.offset):
-            offset = self.offset + (0.0, ) * (ndim - len(self.offset))
+            offset = self.offset + (0.0,) * (ndim - len(self.offset))
         else:
             offset = self.offset[:ndim]
 
         if ndim > self.direction.shape[0]:
             direction = np.identity(ndim)
-            direction[:self.direction.shape[0], :self.direction.shape[0]] = self.direction
+            direction[
+                : self.direction.shape[0], : self.direction.shape[0]
+            ] = self.direction
         else:
             direction = self.direction[:ndim, :ndim]
-        
+
         return spacing, offset, direction
 
     def set_voxel_spacing(self, spacing):
         """
         Set image's spacing.
 
         Parameters
         ----------
         spacing : tuple of floats
             the new image voxel spacing
             take care that image and spacing dimensionalities match
-        """        
+        """
         self.spacing = tuple(spacing)
-    
+
     def set_offset(self, offset):
         """
         Set image's offset.
 
         Parameters
         ----------
         offset : tuple of floats
@@ -310,26 +336,26 @@
         -------
         direction : tuple of floats
             the image's direction / affine transformation matrix
             must be of square shape
             default to the identity matrix
         """
         self.direction = np.asarray(direction)
-    
+
     def get_voxel_spacing(self):
         """
         Get image's spacing.
-        
+
         Returns
         -------
         spacing : tuple of floats
             the image's spacing
         """
         return self.spacing
-    
+
     def get_offset(self):
         """
         Get image's offset.
 
         Returns
         -------
         offset : tuple of floats
@@ -343,19 +369,19 @@
 
         Returns
         -------
         direction : ndarray
             the image's direction / affine transformation matrix
             of square shape
         """
-        return self.direction    
+        return self.direction
 
     def get_sitkimage(self):
         """
         Get underlying sitk Image object.
-        
+
         Returns
         -------
         image-object : sitk.Image or None
             the underlying sitk image object if set
         """
         return self.sitkimage
```

### Comparing `MedPy-0.4.0/medpy/io/load.py` & `MedPy-0.5.0/medpy/io/load.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Copyright (C) 2013 Oskar Maier
-# 
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
-# 
+#
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
-# 
+#
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 # author Oskar Maier
 # version r0.3.1
 # since 2012-05-28
 # status Release
@@ -21,43 +21,44 @@
 # build-in modules
 import os.path
 
 # third-party modules
 import numpy as np
 import SimpleITK as sitk
 
+from ..core import ImageLoadingError, Logger
+
 # own modules
 from .header import Header
-from ..core import Logger
-from ..core import ImageLoadingError
+
 
 # code
 def load(image):
     r"""
     Loads the ``image`` and returns a ndarray with the image's pixel content as well as
     a header object.
-    
+
     The header can, with restrictions, be used to extract additional meta-information
     about the image (e.g. using the methods in `~medpy.io.Header`). Additionally
     it serves as meta-data container that can be passes to `~medpy.io.save.save` when the
     altered image is saved to the hard drive again. Note that the transfer of meta-data is
     only possible, and even then not guaranteed, when the source and target image formats
     are the same.
-    
+
     MedPy relies on SimpleITK, which enables the power of ITK for image loading and saving.
     The supported image file formats should include at least the following.
 
     Medical formats:
 
     - ITK MetaImage (.mha/.raw, .mhd)
     - Neuroimaging Informatics Technology Initiative (NIfTI) (.nia, .nii, .nii.gz, .hdr, .img, .img.gz)
     - Analyze (plain, SPM99, SPM2) (.hdr/.img, .img.gz)
     - Digital Imaging and Communications in Medicine (DICOM) (.dcm, .dicom)
     - Digital Imaging and Communications in Medicine (DICOM) series (<directory>/)
-    - Nearly Raw Raster Data (Nrrd) (.nrrd, .nhdr) 
+    - Nearly Raw Raster Data (Nrrd) (.nrrd, .nhdr)
     - Medical Imaging NetCDF (MINC) (.mnc, .MNC)
     - Guys Image Processing Lab (GIPL) (.gipl, .gipl.gz)
 
     Microscopy formats:
 
     - Medical Research Council (MRC) (.mrc, .rec)
     - Bio-Rad (.pic, .PIC)
@@ -65,57 +66,61 @@
     - Stimulate / Signal Data (SDT) (.sdt)
 
     Visualization formats:
 
     - VTK images (.vtk)
 
     Other formats:
-    
+
     - Portable Network Graphics (PNG) (.png, .PNG)
     - Joint Photographic Experts Group (JPEG) (.jpg, .JPG, .jpeg, .JPEG)
     - Tagged Image File Format (TIFF) (.tif, .TIF, .tiff, .TIFF)
     - Windows bitmap (.bmp, .BMP)
     - Hierarchical Data Format (HDF5) (.h5 , .hdf5 , .he5)
     - MSX-DOS Screen-x (.ge4, .ge5)
-        
+
     For informations about which image formats, dimensionalities and pixel data types
     your current configuration supports, run `python3 tests/support.py > myformats.log`.
 
     Further information see https://simpleitk.readthedocs.io .
-    
+
     Parameters
     ----------
     image : string
         Path to the image to load.
-    
+
     Returns
     -------
     image_data : ndarray
         The image data as numpy array with order `x,y,z,c`.
     image_header : Header
         The image metadata as :mod:`medpy.io.Header`.
-    
+
     Raises
     ------
     ImageLoadingError
         If the image could not be loaded due to some reason.
     """
     logger = Logger.getInstance()
-    logger.info('Loading image {}...'.format(image))
+    logger.info("Loading image {}...".format(image))
 
     if not os.path.exists(image):
-        raise ImageLoadingError('The supplied image {} does not exist.'.format(image))
+        raise ImageLoadingError("The supplied image {} does not exist.".format(image))
 
     if os.path.isdir(image):
         # !TODO: this does not load the meta-data, find a way to load it from a series, too
-        logger.info('Loading image as DICOM series. If more than one found in folder {} defaulting to first.'.format(image))
+        logger.info(
+            "Loading image as DICOM series. If more than one found in folder {} defaulting to first.".format(
+                image
+            )
+        )
         sitkimage = sitk.ReadImage(sitk.ImageSeriesReader_GetGDCMSeriesFileNames(image))
     else:
         sitkimage = sitk.ReadImage(image)
-        
+
     # Make image array data and header
     header = Header(sitkimage=sitkimage)
     image = sitk.GetArrayFromImage(sitkimage)
 
     # Roll axes from z,y,x,c to x,y,z,c
     if image.ndim == 4:
         image = np.moveaxis(image, -1, 0)
```

### Comparing `MedPy-0.4.0/medpy/__init__.py` & `MedPy-0.5.0/medpy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
-__version__ = '0.3.0'
+__version__ = "0.5.0"
```

### Comparing `MedPy-0.4.0/medpy/core/exceptions.py` & `MedPy-0.5.0/medpy/core/exceptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Copyright (C) 2013 Oskar Maier
-# 
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
-# 
+#
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
-# 
+#
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 # author Oskar Maier
 # version r0.2
 # since 2011-12-11
 # status Development
@@ -22,47 +22,48 @@
 
 # third-party modules
 
 # path changes
 
 # own modules
 
+
 # code
 class ArgumentError(Exception):
-    r"""Thrown by an application when an invalid command line argument has been supplied.
-    """
+    r"""Thrown by an application when an invalid command line argument has been
+    supplied."""
     pass
-    
+
+
 class FunctionError(Exception):
-    r"""Thrown when a supplied function returns unexpected results.
-    """
+    r"""Thrown when a supplied function returns unexpected results."""
     pass
-    
+
+
 class SubprocessError(Exception):
-    r"""Thrown by an application when a subprocess execution failed.
-    """
+    r"""Thrown by an application when a subprocess execution failed."""
     pass
 
+
 class ImageTypeError(Exception):
-    r"""Thrown when trying to load or save an image of unknown type.
-    """
+    r"""Thrown when trying to load or save an image of unknown type."""
     pass
 
+
 class DependencyError(Exception):
-    r"""Thrown when a required module could not be loaded.
-    """
+    r"""Thrown when a required module could not be loaded."""
     pass
 
+
 class ImageLoadingError(Exception):
-    r"""Thrown when a image could not be loaded.
-    """
+    r"""Thrown when a image could not be loaded."""
     pass
 
+
 class ImageSavingError(Exception):
-    r"""Thrown when a image could not be saved.
-    """
+    r"""Thrown when a image could not be saved."""
     pass
 
+
 class MetaDataError(Exception):
-    r"""Thrown when an image meta data failure occurred.
-    """
+    r"""Thrown when an image meta data failure occurred."""
     pass
```

### Comparing `MedPy-0.4.0/medpy/core/logger.py` & `MedPy-0.5.0/medpy/core/logger.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,144 +1,148 @@
 # Copyright (C) 2013 Oskar Maier
-# 
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
-# 
+#
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
-# 
+#
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 # author Oskar Maier
 # version r0.1
 # since 2011-12-12
 # status Release
 
+import logging
+
 # build-in module
 import sys
-import logging
 from logging import Logger as NativeLogger
 
 # third-party modules
 
 # own modules
 
 # constants
 
+
 # code
-class Logger (NativeLogger):
+class Logger(NativeLogger):
     r"""Logger to be used by all applications and classes.
-    
+
     Notes
     -----
     Singleton class i.e. setting the log level changes the output globally.
-    
+
     Examples
     --------
     Initializing the logger
-    
+
     >>> from medpy.core import Logger
     >>> logger = Logger.getInstance()
-    
+
     Error messages are passed to stdout
-    
+
     >>> logger.error('error message')
     15.09.2014 12:40:25 [ERROR   ] error message
     >>> logger.error('critical message')
     15.09.2014 12:40:42 [CRITICAL] critical message
-    
+
     But debug and info messages are suppressed
-    
+
     >>> logger.info('info message')
     >>> logger.debug('debug message')
-    
+
     Unless the log level is set accordingly
-    
+
     >>> import logging
     >>> logger.setLevel(logging.DEBUG)
-    
+
     >>> logger.info('info message')
     15.09.2014 12:43:06 [INFO    ] info message (in <ipython-input-14-a08cad56519d>.<module>:1)
     >>> logger.debug('debug message')
     15.09.2014 12:42:50 [DEBUG   ] debug message (in <ipython-input-13-3bb0c512b560>.<module>:1)
-        
+
     """
-    
-    class LoggerHelper (object):
-        r"""A helper class which performs the actual initialization.
-        """
-        def __call__(self, *args, **kw) :
+
+    class LoggerHelper(object):
+        r"""A helper class which performs the actual initialization."""
+
+        def __call__(self, *args, **kw):
             # If an instance of TestSingleton does not exist,
             # create one and assign it to TestSingleton.instance.
-            if Logger._instance is None :
+            if Logger._instance is None:
                 Logger._instance = Logger()
             # Return TestSingleton.instance, which should contain
             # a reference to the only instance of TestSingleton
             # in the system.
             return Logger._instance
-    
-    r"""Member variable initiating and returning the instance of the class."""    
-    getInstance = LoggerHelper() 
+
+    r"""Member variable initiating and returning the instance of the class."""
+    getInstance = LoggerHelper()
     r"""The member variable holding the actual instance of the class."""
     _instance = None
     r"""Holds the loggers handler for format changes."""
     _handler = None
 
-    def __init__(self, name = 'MedPyLogger', level = 0) :
+    def __init__(self, name="MedPyLogger", level=0):
         # To guarantee that no one created more than one instance of Logger:
-        if not Logger._instance == None :
-            raise RuntimeError('Only one instance of Logger is allowed!')
-        
+        if Logger._instance is not None:
+            raise RuntimeError("Only one instance of Logger is allowed!")
+
         # initialize parent
         NativeLogger.__init__(self, name, level)
-        
+
         # set attributes
         self.setHandler(logging.StreamHandler(sys.stdout))
         self.setLevel(logging.WARNING)
-        
+
     def setHandler(self, hdlr):
         r"""Replace the current handler with a new one.
-        
+
         Parameters
         ----------
         hdlr : logging.Handler
-            A subclass of Handler that should used to handle the logging output. 
-        
+            A subclass of Handler that should used to handle the logging output.
+
         Notes
         -----
         If none should be replaces, but just one added, use the parent classes
         addHandler() method.
         """
-        if None != self._handler:
+        if self._handler is not None:
             self.removeHandler(self._handler)
         self._handler = hdlr
         self.addHandler(self._handler)
-        
+
     def setLevel(self, level):
         r"""Overrides the parent method to adapt the formatting string to the level.
-        
+
         Parameters
         ----------
         level : int
             The new log level to set. See the logging levels in the logging module for details.
-            
+
         Examples
         --------
         >>> import logging
         >>> Logger.setLevel(logging.DEBUG)
         """
         if logging.DEBUG >= level:
-            formatter = logging.Formatter("%(asctime)s [%(levelname)-8s] %(message)s (in %(module)s.%(funcName)s:%(lineno)s)", 
-                                          "%d.%m.%Y %H:%M:%S") 
+            formatter = logging.Formatter(
+                "%(asctime)s [%(levelname)-8s] %(message)s (in %(module)s.%(funcName)s:%(lineno)s)",
+                "%d.%m.%Y %H:%M:%S",
+            )
             self._handler.setFormatter(formatter)
         else:
-            formatter = logging.Formatter("%(asctime)s [%(levelname)-8s] %(message)s", 
-                                          "%d.%m.%Y %H:%M:%S") 
+            formatter = logging.Formatter(
+                "%(asctime)s [%(levelname)-8s] %(message)s", "%d.%m.%Y %H:%M:%S"
+            )
             self._handler.setFormatter(formatter)
-            
+
         NativeLogger.setLevel(self, level)
-
```

### Comparing `MedPy-0.4.0/medpy/utilities/argparseu.py` & `MedPy-0.5.0/medpy/utilities/argparseu.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,104 +1,109 @@
 # Copyright (C) 2013 Oskar Maier
-# 
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
-# 
+#
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
-# 
+#
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 # author Oskar Maier
 # version r0.1.1
 # since 2013-07-02
 # status Release
 
 # build-in modules
 import argparse
-import itertools
 import os
 
 # third-party modules
 
 # own modules
 
+
 # code
 def existingDirectory(string):
     """
     A custom type for the argparse commandline parser.
     Check whether the supplied string points to a valid directory.
-    
+
     Examples
     --------
-    
-    >>> parser.add_argument('argname', type=existingDirectory, help='help')    
+
+    >>> parser.add_argument('argname', type=existingDirectory, help='help')
     """
     if not os.path.isdir(string):
-        argparse.ArgumentTypeError('{} is not a valid directory.'.format(string))
+        argparse.ArgumentTypeError("{} is not a valid directory.".format(string))
     return string
 
+
 def sequenceOfStrings(string):
     """
     A custom type for the argparse commandline parser.
     Accepts colon-separated lists of strings.
-    
+
     Examples
     --------
-    
+
     >>> parser.add_argument('argname', type=sequenceOfStrings, help='help')
     """
-    return string.split(',')
+    return string.split(",")
+
 
 def sequenceOfIntegersGeAscendingStrict(string):
     """
     A custom type for the argparse commandline parser.
     Accepts only colon-separated lists of valid integer values that are greater than or
     equal to 0 and in ascending order.
-    
+
     Examples
     --------
 
     >>> parser.add_argument('argname', type=sequenceOfIntegersGeAscending, help='help')
     """
     return __sequenceAscendingStrict(__sequenceGe(sequenceOfIntegers(string)))
 
+
 def sequenceOfIntegers(string):
     """
     A custom type for the argparse commandline parser.
     Accepts only colon-separated lists of valid integer values.
 
     Examples
     --------
 
     >>> parser.add_argument('argname', type=sequenceOfIntegers, help='help')
 
     """
-    value = list(map(int, string.split(',')))
+    value = list(map(int, string.split(",")))
     return value
 
+
 def sequenceOfIntegersGt(string):
     """
     A custom type for the argparse commandline parser.
     Accepts only colon-separated lists of valid integer values that are greater than 0.
 
     Examples
     --------
 
     >>> parser.add_argument('argname', type=sequenceOfIntegersGt, help='help')
 
     """
     value = sequenceOfIntegers(string)
     return __sequenceGt(value)
 
+
 def sequenceOfIntegersGe(string):
     """
     A custom type for the argparse commandline parser.
     Accepts only colon-separated lists of valid integer values that are greater than or
     equal to 0.
 
     Examples
@@ -106,28 +111,30 @@
 
     >>> parser.add_argument('argname', type=sequenceOfIntegersGe, help='help')
 
     """
     value = sequenceOfIntegers(string)
     return __sequenceGe(value)
 
+
 def sequenceOfIntegersLt(string):
     """
     A custom type for the argparse commandline parser.
     Accepts only colon-separated lists of valid integer values that are less than 0.
 
     Examples
     --------
 
     >>> parser.add_argument('argname', type=sequenceOfIntegersLt, help='help')
 
     """
     value = sequenceOfIntegers(string)
     return __sequenceLt(value)
 
+
 def sequenceOfIntegersLe(string):
     """
     A custom type for the argparse commandline parser.
     Accepts only colon-separated lists of valid integer values that are less than or
     equal to 0.
 
     Examples
@@ -135,42 +142,45 @@
 
     >>> parser.add_argument('argname', type=sequenceOfIntegersLe, help='help')
 
     """
     value = sequenceOfIntegers(string)
     return __sequenceLe(value)
 
+
 def sequenceOfFloats(string):
     """
     A custom type for the argparse commandline parser.
     Accepts only colon-separated lists of valid float values.
 
     Examples
     --------
 
     >>> parser.add_argument('argname', type=sequenceOfFloats, help='help')
 
     """
-    value = list(map(float, string.split(',')))
+    value = list(map(float, string.split(",")))
     return value
 
+
 def sequenceOfFloatsGt(string):
     """
     A custom type for the argparse commandline parser.
     Accepts only colon-separated lists of valid float values that are greater than 0.
 
     Examples
     --------
 
     >>> parser.add_argument('argname', type=sequenceOfFloatsGt, help='help')
 
     """
     value = sequenceOfFloats(string)
     return __sequenceGt(value)
 
+
 def sequenceOfFloatsGe(string):
     """
     A custom type for the argparse commandline parser.
     Accepts only colon-separated lists of valid float values that are greater than or
     equal to 0.
 
     Examples
@@ -178,28 +188,30 @@
 
     >>> parser.add_argument('argname', type=sequenceOfFloatsGe, help='help')
 
     """
     value = sequenceOfFloats(string)
     return __sequenceGe(value)
 
+
 def sequenceOfFloatsLt(string):
     """
     A custom type for the argparse commandline parser.
     Accepts only colon-separated lists of valid float values that are less than 0.
 
     Examples
     --------
 
     >>> parser.add_argument('argname', type=sequenceOfFloatsLt, help='help')
 
     """
     value = sequenceOfFloats(string)
     return __sequenceLt(value)
 
+
 def sequenceOfFloatsLe(string):
     """
     A custom type for the argparse commandline parser.
     Accepts only colon-separated lists of valid float values that are less than or
     equal to 0.
 
     Examples
@@ -207,46 +219,64 @@
 
     >>> parser.add_argument('argname', type=sequenceOfFloatsLe, help='help')
 
     """
     value = sequenceOfFloats(string)
     return __sequenceLe(value)
 
+
 def __sequenceGt(l):
     "Test a sequences values for being greater than 0."
     for e in l:
-        if 0 >= e: raise argparse.ArgumentTypeError('All values have to be greater than 0.')
+        if 0 >= e:
+            raise argparse.ArgumentTypeError("All values have to be greater than 0.")
     return l
 
+
 def __sequenceGe(l):
     "Test a sequences values for being greater than or equal to 0."
     for e in l:
-        if 0 > e: raise argparse.ArgumentTypeError('All values have to be greater than or equal to 0.')
+        if 0 > e:
+            raise argparse.ArgumentTypeError(
+                "All values have to be greater than or equal to 0."
+            )
     return l
 
+
 def __sequenceLt(l):
     "Test a sequences values for being less than 0."
     for e in l:
-        if 0 <= e: raise argparse.ArgumentTypeError('All values have to be less than 0.')
+        if 0 <= e:
+            raise argparse.ArgumentTypeError("All values have to be less than 0.")
     return l
 
+
 def __sequenceLe(l):
     "Test a sequences values for being less than or equal to 0."
     for e in l:
-        if 0 < e: raise argparse.ArgumentTypeError('All values have to be less than or equal to 0.')
+        if 0 < e:
+            raise argparse.ArgumentTypeError(
+                "All values have to be less than or equal to 0."
+            )
     return l
 
+
 def __sequenceAscendingStrict(l):
     "Test a sequences values to be in strictly ascending order."
     it = iter(l)
     next(it)
     if not all(b > a for a, b in zip(l, it)):
-        raise argparse.ArgumentTypeError('All values must be given in strictly ascending order.')
+        raise argparse.ArgumentTypeError(
+            "All values must be given in strictly ascending order."
+        )
     return l
 
+
 def __sequenceDescendingStrict(l):
     "Test a sequences values to be in strictly descending order."
     it = iter(l)
     next(it)
     if not all(b < a for a, b in zip(l, it)):
-        raise argparse.ArgumentTypeError('All values must be given in strictly descending order.')
-    return l
+        raise argparse.ArgumentTypeError(
+            "All values must be given in strictly descending order."
+        )
+    return l
```

### Comparing `MedPy-0.4.0/medpy/utilities/__init__.py` & `MedPy-0.5.0/medpy/utilities/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,22 +11,24 @@
 
 Custom types for the `argparse <https://docs.python.org/3/library/argparse.html>`_ commandline parser
 =====================================================================================================
 
 .. module:: medpy.utilities.argparseu
 .. autosummary::
     :toctree: generated/
-    
+
     sequenceOfIntegers
     sequenceOfIntegersGt
     sequenceOfIntegersGe
     sequenceOfIntegersLt
     sequenceOfIntegersLe
     sequenceOfIntegersGeAscendingStrict
     sequenceOfFloats
     sequenceOfFloatsGt
     sequenceOfFloatsGe
     sequenceOfFloatsLt
     sequenceOfFloatsLe
 
 """
-from . import argparseu
+from . import argparseu as argparseu
+
+__all__ = ["argparseu"]
```

### Comparing `MedPy-0.4.0/README.md` & `MedPy-0.5.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,38 @@
-[![PyPI version fury.io](https://badge.fury.io/py/MedPy.svg)](https://pypi.python.org/pypi/MedPy/)
+[![PyPI version](https://badge.fury.io/py/MedPy.svg)](https://pypi.python.org/pypi/MedPy/)
+[![anaconda version](https://anaconda.org/conda-forge/medpy/badges/version.svg)](https://anaconda.org/conda-forge/medpy)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/MedPy.svg)](https://pypi.python.org/pypi/MedPy/)
 [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![Downloads](https://pepy.tech/badge/medpy/month)](https://pepy.tech/project/medpy)
-![travis auto-build](https://travis-ci.org/loli/medpy.svg?branch=master)
-[![DOI](https://zenodo.org/badge/4295983.svg)](https://zenodo.org/badge/latestdoi/4295983)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.2565940.svg)](https://doi.org/10.5281/zenodo.2565940)
 
-[GitHub](https://github.com/loli/medpy/) | [Documentation](http://loli.github.io/medpy/) | [Tutorials](http://loli.github.io/medpy/) | [Issue tracker](https://github.com/loli/medpy/issues) | [Contact](oskar.maier@gmail.com)
+
+[GitHub](https://github.com/loli/medpy/) | [Documentation](http://loli.github.io/medpy/) | [Tutorials](http://loli.github.io/medpy/) | [Issue tracker](https://github.com/loli/medpy/issues)
 
 # medpy - Medical Image Processing in Python
 
 MedPy is an image processing library and collection of scripts targeted towards medical (i.e. high dimensional) image processing.
 
 ## Stable releases
 
 - Download (stable release): https://pypi.python.org/pypi/medpy
 - HTML documentation and installation instruction (stable release): http://loli.github.io/medpy/
+- Download from [Conda-Forge](https://conda-forge.org): https://anaconda.org/conda-forge/medpy
 
 ## Development version
 
 - Download (development version): https://github.com/loli/medpy
 - HTML documentation and installation instruction (development version): create this from doc/ folder following instructions in contained README file
 
+## Contribute
+
+- Clone `master` branch from [github](https://github.com/loli/medpy)
+- Install [pre-commit](https://pre-commit.com/) hooks or with `[dev,test]` extras
+- Submit your change as a PR request
+
 ## Python 2 version
 
 Python 2 is no longer supported. But you can still use the older releases `<=0.3.0`.
 
 ## Other links
 
 - Issue tracker: https://github.com/loli/medpy/issues
```

### Comparing `MedPy-0.4.0/README_PYPI.md` & `MedPy-0.5.0/README_PYPI.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,35 @@
 # MedPy
 
-[GitHub](https://github.com/loli/medpy/) | [Documentation](http://loli.github.io/medpy/) | [Tutorials](http://loli.github.io/medpy/) | [Issue tracker](https://github.com/loli/medpy/issues) | [Contact](oskar.maier@gmail.com)
+[GitHub](https://github.com/loli/medpy/) | [Documentation](http://loli.github.io/medpy/) | [Tutorials](http://loli.github.io/medpy/) | [Issue tracker](https://github.com/loli/medpy/issues)
 
 **MedPy** is a library and script collection for medical image processing in Python, providing basic functionalities for **reading**, **writing** and **manipulating** large images of **arbitrary dimensionality**.
 Its main contributions are n-dimensional versions of popular **image filters**, a collection of **image feature extractors**, ready to be used with [scikit-learn](http://scikit-learn.org), and an exhaustive n-dimensional **graph-cut** package.
 
 * [Installation](#installation)
 * [Getting started with the library](#getting-started-with-the-library)
 * [Getting started with the scripts](#getting-started-with-the-scripts)
-* [Read/write support for medical image formats](#read-write-support-for-medical-image-formats)
+* [Support of medical image formats](#support-of-medical-image-formats)
 * [Requirements](#requirements)
 * [License](#license)
 
 ## Installation
 
 ```bash
 sudo apt-get install libboost-python-dev build-essential
 pip3 install medpy
 ```
 
 **MedPy** requires **Python 3** and officially supports Ubuntu as well as other Debian derivatives.
 For installation instructions on other operating systems see the [documentation](http://loli.github.io/medpy/).
-While the library itself is written purely in Python, the **graph-cut** extension comes in C++ and has it's own requirements. More details can be found in the [documentation](http://loli.github.io/medpy/).
-
-### Using Python 2
-
-**Python 2** is no longer supported. But you can still use the older releases.
-
-```bash
-pip install medpy==0.3.0
-```
+While the library itself is written purely in Python, the **graph-cut** extension comes in C++ and has [it's own requirements](http://loli.github.io/medpy/installation/graphcutsupport.html).
 
 ## Getting started with the library
 
-If you already have a medical image whose format is support (see the [documentation](http://loli.github.io/medpy/>) for details), then good.
-Otherwise, navigate to http://www.nitrc.org/projects/inia19, click on the *Download Now* button, unpack and look for the *inia19-t1.nii* file. Open it in your favorite medical image viewer (I personally fancy [itksnap](http://www.itksnap.org)) and beware: the INIA19 primate brain atlas.
+If you already have a medical image at hand in [one of the supported formats](http://loli.github.io/medpy/information/imageformats.html), you can use it for this introduction. If not, navigate to http://www.nitrc.org/projects/inia19, click on the *Download Now* button, unpack and look for the *inia19-t1.nii* file. Open it in your favorite medical image viewer (I personally fancy [itksnap](http://www.itksnap.org)) and beware: the INIA19 primate brain atlas.
 
 Load the image
 
 ```python
 from medpy.io import load
 image_data, image_header = load('/path/to/image.xxx')
 ```
@@ -82,15 +73,15 @@
 And save the binary image, marking the foreground
 
 ```python
 from medpy.io import save
 save(output_data, '/path/to/otsu.xxx', image_header)
 ```
 
-After taking a look at it, you might want to dive deeper with the tutorials found in the [documentation](http://loli.github.io/medpy/).
+After taking a look at it, you might want to dive deeper with the tutorials found in the [documentation](http://loli.github.io/medpy/information/commandline_tools_listing.html).
 
 ## Getting started with the scripts
 
 **MedPy** comes with a range of read-to-use commandline scripts, which are all prefixed by `medpy_`.
 To try these examples, first get an image as described in the previous section. Now call
 
 ```bash
@@ -107,27 +98,27 @@
 
 ```bash
 medpy_anisotropic_diffusion.py /path/to/image.xxx /path/to/output.xxx
 ```
 
 lets you apply an edge preserving anisotropic diffusion filter. For a list of all scripts, see the [documentation](http://loli.github.io/medpy/).
 
-## Read/write support for medical image formats
+## Support of medical image formats
 
 MedPy relies on SimpleITK, which enables the power of ITK for image loading and saving.
 The supported image file formats should include at least the following. Note that not all might be supported by your machine.
 
 **Medical formats:**
 
 * ITK MetaImage (.mha/.raw, .mhd)
 * Neuroimaging Informatics Technology Initiative (NIfTI) (.nia, .nii, .nii.gz, .hdr, .img, .img.gz)
 * Analyze (plain, SPM99, SPM2) (.hdr/.img, .img.gz)
 * Digital Imaging and Communications in Medicine (DICOM) (.dcm, .dicom)
 * Digital Imaging and Communications in Medicine (DICOM) series (<directory>/)
-* Nearly Raw Raster Data (Nrrd) (.nrrd, .nhdr) 
+* Nearly Raw Raster Data (Nrrd) (.nrrd, .nhdr)
 * Medical Imaging NetCDF (MINC) (.mnc, .MNC)
 * Guys Image Processing Lab (GIPL) (.gipl, .gipl.gz)
 
 **Microscopy formats:**
 
 * Medical Research Council (MRC) (.mrc, .rec)
 * Bio-Rad (.pic, .PIC)
```

### Comparing `MedPy-0.4.0/LICENSE.txt` & `MedPy-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MedPy-0.4.0/CHANGES.txt` & `MedPy-0.5.0/CHANGES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+v0.5.0, 2024-04-XX -- Addressed all depreciation warnings and incompatabilities
+                      Updated documentation
+                      Updated and fixed tests
+                      Added github workflows as system
+                      Introduced formatting rules and pre-commit to enforce them
+                      Removed dockerfile creation files
 v0.4.0, 2018-02-XX -- Switched to Python 3: finally compatible with modern development environements
                       Switched to simple itk for image loading/saving: read dicom series, more formats, less dependencies, cleaner code, easier to maintain
                       Documentation: installation instructions for Windows and OsX
                       Others: improved filters, cleanup, bugfixes
 v0.3.0, 2017-09-20 -- Extensive cleanup, many new functionalities, updated documentation, notebook tutorials, Python 3 branch
 v0.2.2, 2014-09-18 -- Changes the documentation engine to Sphinx and fixed a number of bugs
 v0.2.1, 2014-08-19 -- ez_setup.py has not been include
```

### Comparing `MedPy-0.4.0/bin/medpy_intersection.py` & `MedPy-0.5.0/bin/medpy_intersection.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 
 """
-Extracts the intersecting parts of two volumes regarding offset and voxel-spacing. 
+Extracts the intersecting parts of two volumes regarding offset and voxel-spacing.
 
 Copyright (C) 2013 Oskar Maier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
@@ -20,94 +20,126 @@
 """
 
 # build-in modules
 import argparse
 import logging
 import os
 
+from medpy.core import Logger
+from medpy.filter.utilities import intersection
+
+# own modules
+from medpy.io import header, load, save
+
 # third-party modules
 
 # path changes
 
-# own modules
-from medpy.io import load, save, header
-from medpy.core import Logger
-from medpy.filter.utilities import intersection
-
 
 # information
 __author__ = "Oskar Maier"
 __version__ = "r0.0.1, 2014-04-25"
 __email__ = "oskar.maier@googlemail.com"
 __status__ = "Development"
 __description__ = """
                   Extracts the intersecting parts of two volumes regarding offset
                   and voxel-spacing.
-                                  
+
                   Copyright (C) 2013 Oskar Maier
                   This program comes with ABSOLUTELY NO WARRANTY; This is free software,
                   and you are welcome to redistribute it under certain conditions; see
-                  the LICENSE file or <http://www.gnu.org/licenses/> for details.   
+                  the LICENSE file or <http://www.gnu.org/licenses/> for details.
                   """
 
+
 # code
 def main():
     # parse cmd arguments
     parser = getParser()
     parser.parse_args()
     args = getArguments(parser)
-    
+
     # prepare logger
     logger = Logger.getInstance()
-    if args.debug: logger.setLevel(logging.DEBUG)
-    elif args.verbose: logger.setLevel(logging.INFO)
-    
+    if args.debug:
+        logger.setLevel(logging.DEBUG)
+    elif args.verbose:
+        logger.setLevel(logging.INFO)
+
     # check if output image exists (will also be performed before saving, but as the smoothing might be very time intensity, a initial check can save frustration)
     if not args.force:
         if os.path.exists(args.output1):
-            raise parser.error('The output image {} already exists.'.format(args.output1))
+            raise parser.error(
+                "The output image {} already exists.".format(args.output1)
+            )
         if os.path.exists(args.output2):
-            raise parser.error('The output image {} already exists.'.format(args.output2))
-    
+            raise parser.error(
+                "The output image {} already exists.".format(args.output2)
+            )
+
     # loading images
     data_input1, header_input1 = load(args.input1)
     data_input2, header_input2 = load(args.input2)
-    logger.debug('Original image sizes are {} and {}.'.format(data_input1.shape, data_input2.shape))
-    
+    logger.debug(
+        "Original image sizes are {} and {}.".format(
+            data_input1.shape, data_input2.shape
+        )
+    )
+
     # compute intersection volumes (punch)
-    logger.info('Computing the intersection.')
-    inters1, inters2, new_offset = intersection(data_input1, header_input1, data_input2, header_input2)
-    logger.debug('Punched images are of sizes {} and {} with new offset {}.'.format(inters1.shape, inters2.shape, new_offset))
-    
+    logger.info("Computing the intersection.")
+    inters1, inters2, new_offset = intersection(
+        data_input1, header_input1, data_input2, header_input2
+    )
+    logger.debug(
+        "Punched images are of sizes {} and {} with new offset {}.".format(
+            inters1.shape, inters2.shape, new_offset
+        )
+    )
+
     # check if any intersection could be found at all
     if 0 == inters1.size:
-        logger.warning('No intersection could be found between the images. Please check their meta-data e.g. with medpy_info')
-    
+        logger.warning(
+            "No intersection could be found between the images. Please check their meta-data e.g. with medpy_info"
+        )
+
     # update header informations
     header.set_offset(header_input1, new_offset)
     header.set_offset(header_input2, new_offset)
-    
+
     # save punched images
     save(inters1, args.output1, header_input1, args.force)
     save(inters2, args.output2, header_input2, args.force)
-    
-    logger.info('Successfully terminated.')
+
+    logger.info("Successfully terminated.")
+
 
 def getArguments(parser):
     "Provides additional validation of the arguments collected by argparse."
     return parser.parse_args()
 
+
 def getParser():
     "Creates and returns the argparse parser object."
     parser = argparse.ArgumentParser(description=__description__)
-    parser.add_argument('input1', help='First source volume.')
-    parser.add_argument('input2', help='Second source volume.')
-    parser.add_argument('output1', help='First target volume.')
-    parser.add_argument('output2', help='Second target volume.')
-    parser.add_argument('-v', dest='verbose', action='store_true', help='Display more information.')
-    parser.add_argument('-d', dest='debug', action='store_true', help='Display debug information.')
-    parser.add_argument('-f', dest='force', action='store_true', help='Silently override existing output images.')
-    
+    parser.add_argument("input1", help="First source volume.")
+    parser.add_argument("input2", help="Second source volume.")
+    parser.add_argument("output1", help="First target volume.")
+    parser.add_argument("output2", help="Second target volume.")
+    parser.add_argument(
+        "-v", dest="verbose", action="store_true", help="Display more information."
+    )
+    parser.add_argument(
+        "-d", dest="debug", action="store_true", help="Display debug information."
+    )
+    parser.add_argument(
+        "-f",
+        dest="force",
+        action="store_true",
+        help="Silently override existing output images.",
+    )
+
     return parser
-    
+
+
 if __name__ == "__main__":
     main()
```

### Comparing `MedPy-0.4.0/bin/medpy_create_empty_volume_by_example.py` & `MedPy-0.5.0/bin/medpy_create_empty_volume_by_example.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,67 +19,83 @@
 along with this program.  If not, see <http://www.gnu.org/licenses/>."""
 
 # build-in modules
 import argparse
 import logging
 
 # third-party modules
-import scipy
-
-# path changes
+import numpy
 
 # own modules
 from medpy.core import Logger
 from medpy.io import load, save
 
+# path changes
+
 
 # information
 __author__ = "Oskar Maier"
 __version__ = "r0.1.0, 2012-08-24"
 __email__ = "oskar.maier@googlemail.com"
 __status__ = "Release"
 __description__ = """
                   Creates an empty volume with the same attributes as the passes example image.
-                
+
                   Copyright (C) 2013 Oskar Maier
                   This program comes with ABSOLUTELY NO WARRANTY; This is free software,
                   and you are welcome to redistribute it under certain conditions; see
-                  the LICENSE file or <http://www.gnu.org/licenses/> for details.    
+                  the LICENSE file or <http://www.gnu.org/licenses/> for details.
                   """
 
+
 # code
 def main():
     args = getArguments(getParser())
-    
+
     # prepare logger
     logger = Logger.getInstance()
-    if args.debug: logger.setLevel(logging.DEBUG)
-    elif args.verbose: logger.setLevel(logging.INFO)
-    
+    if args.debug:
+        logger.setLevel(logging.DEBUG)
+    elif args.verbose:
+        logger.setLevel(logging.INFO)
+
     # loading input image
     input_data, input_header = load(args.example)
-    
+
     # create empty volume with same attributes
-    output_data = scipy.zeros(input_data.shape, dtype=input_data.dtype)
-    
+    output_data = numpy.zeros(input_data.shape, dtype=input_data.dtype)
+
     # save resulting image
     save(output_data, args.output, input_header, args.force)
-        
+
     logger.info("Successfully terminated.")
 
-    
+
 def getArguments(parser):
     "Provides additional validation of the arguments collected by argparse."
     return parser.parse_args()
 
+
 def getParser():
     "Creates and returns the argparse parser object."
-    parser = argparse.ArgumentParser(description=__description__, formatter_class=argparse.RawTextHelpFormatter)
-    parser.add_argument('example', help='The example volume.')
-    parser.add_argument('output', help='Target volume.')
-    parser.add_argument('-v', dest='verbose', action='store_true', help='Display more information.')
-    parser.add_argument('-d', dest='debug', action='store_true', help='Display debug information.')
-    parser.add_argument('-f', dest='force', action='store_true', help='Silently override existing output images.')
+    parser = argparse.ArgumentParser(
+        description=__description__, formatter_class=argparse.RawTextHelpFormatter
+    )
+    parser.add_argument("example", help="The example volume.")
+    parser.add_argument("output", help="Target volume.")
+    parser.add_argument(
+        "-v", dest="verbose", action="store_true", help="Display more information."
+    )
+    parser.add_argument(
+        "-d", dest="debug", action="store_true", help="Display debug information."
+    )
+    parser.add_argument(
+        "-f",
+        dest="force",
+        action="store_true",
+        help="Silently override existing output images.",
+    )
     return parser
 
+
 if __name__ == "__main__":
-    main() 
+    main()
```

### Comparing `MedPy-0.4.0/bin/medpy_graphcut_label_bgreduced.py` & `MedPy-0.5.0/bin/medpy_graphcut_label_bgreduced.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,210 +15,257 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
-# build-in modules
-from argparse import RawTextHelpFormatter
 import argparse
-import logging
 import itertools
+import logging
 import os
 
+# build-in modules
+from argparse import RawTextHelpFormatter
+
 # third-party modules
-import scipy
+import numpy
 from scipy import ndimage
 
-# path changes
+from medpy import filter, graphcut
 
 # own modules
 from medpy.core import ArgumentError, Logger
-from medpy.io import load, save
-from medpy import graphcut
-from medpy import filter
 from medpy.graphcut.wrapper import split_marker
+from medpy.io import load, save
 
+# path changes
 
 
 # information
 __author__ = "Oskar Maier"
 __version__ = "r0.3.4, 2012-03-16"
 __email__ = "oskar.maier@googlemail.com"
 __status__ = "Release"
 __description__ = """
                   !Modified version of original GC label, as reduces the volume sizes
                   using the background markers.
-                  
+
                   Perform a binary graph cut using Boykov's max-flow/min-cut algorithm.
-                  
+
                   This implementation does only compute a boundary term and does not use
                   any regional term. The desired boundary term can be selected via the
                   --boundary argument. Depending on the selected term, an additional
                   image has to be supplied as badditional.
-                  
+
                   In the case of the stawiaski boundary term, this is the gradient image.
                   In the case of the difference of means, it is the original image.
-                  
+
                   Furthermore the algorithm requires the region map of the original
                   image, a binary image with foreground markers and a binary
                   image with background markers.
-                  
+
                   Additionally a filename for the created binary mask marking foreground
                   and background has to be supplied.
-                  
+
                   Note that the input images must be of the same dimensionality,
                   otherwise an exception is thrown.
                   Note to take into account the input images orientation.
                   Note that the quality of the resulting segmentations depends also on
                   the quality of the supplied markers.
-                  
+
                   Copyright (C) 2013 Oskar Maier
                   This program comes with ABSOLUTELY NO WARRANTY; This is free software,
                   and you are welcome to redistribute it under certain conditions; see
-                  the LICENSE file or <http://www.gnu.org/licenses/> for details.   
+                  the LICENSE file or <http://www.gnu.org/licenses/> for details.
                   """
 
+
 # code
 def main():
     # parse cmd arguments
     parser = getParser()
     parser.parse_args()
     args = getArguments(parser)
-    
+
     # prepare logger
     logger = Logger.getInstance()
-    if args.debug: logger.setLevel(logging.DEBUG)
-    elif args.verbose: logger.setLevel(logging.INFO)
-        
+    if args.debug:
+        logger.setLevel(logging.DEBUG)
+    elif args.verbose:
+        logger.setLevel(logging.INFO)
+
     # check if output image exists
     if not args.force:
         if os.path.exists(args.output):
-            logger.warning('The output image {} already exists. Exiting.'.format(args.output))
+            logger.warning(
+                "The output image {} already exists. Exiting.".format(args.output)
+            )
             exit(-1)
 
     # load input images
     region_image_data, reference_header = load(args.region)
     markers_image_data, _ = load(args.markers)
     gradient_image_data, _ = load(args.gradient)
-    
+
     # split marker image into fg and bg images
-    logger.info('Extracting foreground and background markers...')
+    logger.info("Extracting foreground and background markers...")
     fgmarkers_image_data, bgmarkers_image_data = split_marker(markers_image_data)
-       
+
     # check if all images dimensions are the same shape
-    if not (gradient_image_data.shape == region_image_data.shape == fgmarkers_image_data.shape == bgmarkers_image_data.shape):
-        logger.critical('Not all of the supplied images are of the same shape.')
-        raise ArgumentError('Not all of the supplied images are of the same shape.')
-    
+    if not (
+        gradient_image_data.shape
+        == region_image_data.shape
+        == fgmarkers_image_data.shape
+        == bgmarkers_image_data.shape
+    ):
+        logger.critical("Not all of the supplied images are of the same shape.")
+        raise ArgumentError("Not all of the supplied images are of the same shape.")
+
     # collect cut objects
     cut_xy = __get_bg_bounding_pipe(bgmarkers_image_data)
-    
+
     # cut volumes
     old_size = region_image_data.shape
     gradient_image_data = gradient_image_data[cut_xy]
     region_image_data = region_image_data[cut_xy]
     fgmarkers_image_data = fgmarkers_image_data[cut_xy]
     bgmarkers_image_data = bgmarkers_image_data[cut_xy]
-    
+
     # recompute the label ids to start from id = 1
-    logger.info('Relabel input image...')
+    logger.info("Relabel input image...")
     region_image_data = filter.relabel(region_image_data)
 
     # generate graph
-    logger.info('Preparing graph...')
-    gcgraph = graphcut.graph_from_labels(region_image_data,
-                                    fgmarkers_image_data,
-                                    bgmarkers_image_data,
-                                    boundary_term = graphcut.energy_label.boundary_stawiaski,
-                                    boundary_term_args = (gradient_image_data)) # second is directedness of graph , 0)
+    logger.info("Preparing graph...")
+    gcgraph = graphcut.graph_from_labels(
+        region_image_data,
+        fgmarkers_image_data,
+        bgmarkers_image_data,
+        boundary_term=graphcut.energy_label.boundary_stawiaski,
+        boundary_term_args=(gradient_image_data),
+    )  # second is directedness of graph , 0)
 
-    logger.info('Removing images that are not longer required from memory...')
+    logger.info("Removing images that are not longer required from memory...")
     del fgmarkers_image_data
     del bgmarkers_image_data
     del gradient_image_data
-    
+
     # execute min-cut
-    logger.info('Executing min-cut...')
+    logger.info("Executing min-cut...")
     maxflow = gcgraph.maxflow()
-    logger.debug('Maxflow is {}'.format(maxflow))
-    
+    logger.debug("Maxflow is {}".format(maxflow))
+
     # apply results to the region image
-    logger.info('Applying results...')
-    mapping = [0] # no regions with id 1 exists in mapping, entry used as padding
-    mapping.extend([0 if gcgraph.termtype.SINK == gcgraph.what_segment(int(x) - 1) else 1 for x in scipy.unique(region_image_data)])
+    logger.info("Applying results...")
+    mapping = [0]  # no regions with id 1 exists in mapping, entry used as padding
+    mapping.extend(
+        [
+            0 if gcgraph.termtype.SINK == gcgraph.what_segment(int(x) - 1) else 1
+            for x in numpy.unique(region_image_data)
+        ]
+    )
     region_image_data = filter.relabel_map(region_image_data, mapping)
-    
+
     # generating final image by increasing the size again
-    output_image_data = scipy.zeros(old_size, dtype=scipy.bool_)
+    output_image_data = numpy.zeros(old_size, dtype=numpy.bool_)
     output_image_data[cut_xy] = region_image_data
-    
+
     # save resulting mask
     save(output_image_data, args.output, reference_header, args.force)
 
-    logger.info('Successfully terminated.')
+    logger.info("Successfully terminated.")
+
 
 def __get_bg_bounding_pipe(bgmarkers):
     # constants
     xdim = 0
     ydim = 1
-    
+
     # compute biggest bb in direction
     bb = __xd_iterator_pass_on(bgmarkers, (xdim, ydim), __extract_bbox)
-    
+
     slicer = [slice(None)] * bgmarkers.ndim
     slicer[xdim] = bb[0]
     slicer[ydim] = bb[1]
-    
-    return slicer
-    
-    
+
+    return tuple(slicer)
+
+
 def __xd_iterator_pass_on(arr, view, fun):
     """
     Like xd_iterator, but the fun return values are always passed on to the next and only the last returned.
     """
     # create list of iterations
-    iterations = [[None] if dim in view else list(range(arr.shape[dim])) for dim in range(arr.ndim)]
-     
+    iterations = [
+        [None] if dim in view else list(range(arr.shape[dim]))
+        for dim in range(arr.ndim)
+    ]
+
     # iterate, create slicer, execute function and collect results
     passon = None
     for indices in itertools.product(*iterations):
-        slicer = [slice(None) if idx is None else slice(idx, idx + 1) for idx in indices]
-        passon = fun(scipy.squeeze(arr[slicer]), passon)
-        
+        slicer = [
+            slice(None) if idx is None else slice(idx, idx + 1) for idx in indices
+        ]
+        passon = fun(numpy.squeeze(arr[tuple(slicer)]), passon)
+
     return passon
-        
+
+
 def __extract_bbox(arr, bb_old):
     "Extracts the bounding box of an binary objects hole (assuming only one in existence)."
-    hole = ndimage.binary_fill_holes(arr)- arr
-    bb_list = ndimage.find_objects(ndimage.binary_dilation(hole, iterations = 1))
-    if 0 == len(bb_list): return bb_old
-    else: bb = bb_list[0]
-    
-    if not bb_old: return list(bb)
-    
+    hole = ndimage.binary_fill_holes(arr) - arr
+    bb_list = ndimage.find_objects(ndimage.binary_dilation(hole, iterations=1))
+    if 0 == len(bb_list):
+        return bb_old
+    else:
+        bb = bb_list[0]
+
+    if not bb_old:
+        return list(bb)
+
     for i in range(len(bb_old)):
-        bb_old[i] = slice(min(bb_old[i].start, bb[i].start),
-                          max(bb_old[i].stop, bb[i].stop))
-    return bb_old
+        bb_old[i] = slice(
+            min(bb_old[i].start, bb[i].start), max(bb_old[i].stop, bb[i].stop)
+        )
+    return tuple(bb_old)
+
 
 def getArguments(parser):
     "Provides additional validation of the arguments collected by argparse."
     return parser.parse_args()
 
+
 def getParser():
     "Creates and returns the argparse parser object."
-    parser = argparse.ArgumentParser(description=__description__, formatter_class=RawTextHelpFormatter)
+    parser = argparse.ArgumentParser(
+        description=__description__, formatter_class=RawTextHelpFormatter
+    )
+
+    parser.add_argument(
+        "gradient", help="The gradient magnitude image of the image to segment."
+    )
+    parser.add_argument("region", help="The region image of the image to segment.")
+    parser.add_argument(
+        "markers",
+        help="Binary image containing the foreground (=1) and background (=2) markers.",
+    )
+    parser.add_argument("output", help="The output image containing the segmentation.")
+    parser.add_argument(
+        "-f",
+        dest="force",
+        action="store_true",
+        help="Set this flag to silently override files that exist.",
+    )
+    parser.add_argument(
+        "-v", dest="verbose", action="store_true", help="Display more information."
+    )
+    parser.add_argument(
+        "-d", dest="debug", action="store_true", help="Display debug information."
+    )
+
+    return parser
 
-    parser.add_argument('gradient', help='The gradient magnitude image of the image to segment.')
-    parser.add_argument('region', help='The region image of the image to segment.')
-    parser.add_argument('markers', help='Binary image containing the foreground (=1) and background (=2) markers.')
-    parser.add_argument('output', help='The output image containing the segmentation.')
-    parser.add_argument('-f', dest='force', action='store_true', help='Set this flag to silently override files that exist.')
-    parser.add_argument('-v', dest='verbose', action='store_true', help='Display more information.')
-    parser.add_argument('-d', dest='debug', action='store_true', help='Display debug information.')
-    
-    return parser    
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `MedPy-0.4.0/bin/medpy_zoom_image.py` & `MedPy-0.5.0/bin/medpy_zoom_image.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,109 +23,147 @@
 import argparse
 import logging
 import os
 
 # third-party modules
 from scipy.ndimage import interpolation
 
-# path changes
-
 # own modules
 from medpy.core import Logger
-from medpy.io import load, save, header
+from medpy.io import header, load, save
+
+# path changes
 
 
 # information
 __author__ = "Oskar Maier"
 __version__ = "r0.2.1, 2012-06-13"
 __email__ = "oskar.maier@googlemail.com"
 __status__ = "Release"
 __description__ = """
                   Zoom into an image by adding new slices in the z-direction and filling
                   them with interpolated data. Overall "enhancement" new slices will be
                   created between every two original slices.
-                  
+
                   If you want to zoom multiple binary objects in an image without
                   interpolating between their values, use the -o switch.
-                  
+
                   Copyright (C) 2013 Oskar Maier
                   This program comes with ABSOLUTELY NO WARRANTY; This is free software,
                   and you are welcome to redistribute it under certain conditions; see
-                  the LICENSE file or <http://www.gnu.org/licenses/> for details.   
+                  the LICENSE file or <http://www.gnu.org/licenses/> for details.
                   """
 
+
 # code
 def main():
     args = getArguments(getParser())
 
     # prepare logger
     logger = Logger.getInstance()
-    if args.debug: logger.setLevel(logging.DEBUG)
-    elif args.verbose: logger.setLevel(logging.INFO)
-    
+    if args.debug:
+        logger.setLevel(logging.DEBUG)
+    elif args.verbose:
+        logger.setLevel(logging.INFO)
+
     # check if output image exists
     if not args.force and os.path.exists(args.output):
-        logger.warning('The output image {} already exists. Exiting.'.format(args.output))
+        logger.warning(
+            "The output image {} already exists. Exiting.".format(args.output)
+        )
         exit(-1)
-    
+
     # load input data
     input_data, input_header = load(args.input)
-    
+
     # if normal mode, perform the zoom
-    logger.info('Performing normal zoom...')
-    output_data, output_header = zoom(input_data, args.enhancement, args.dimension, hdr=input_header)
+    logger.info("Performing normal zoom...")
+    output_data, output_header = zoom(
+        input_data, args.enhancement, args.dimension, hdr=input_header
+    )
 
     # saving results
     save(output_data, args.output, output_header, args.force)
-    
-def zoom(image, factor, dimension, hdr = False, order = 3):
+
+
+def zoom(image, factor, dimension, hdr=False, order=3):
     """
     Zooms the provided image by the supplied factor in the supplied dimension.
     The factor is an integer determining how many slices should be put between each
     existing pair.
     If an image header (hdr) is supplied, its voxel spacing gets updated.
     Returns the image and the updated header or false.
     """
     # check if supplied dimension is valid
     if dimension >= image.ndim:
-        raise argparse.ArgumentError('The supplied zoom-dimension {} exceeds the image dimensionality of 0 to {}.'.format(dimension, image.ndim - 1))
-    
+        raise argparse.ArgumentError(
+            "The supplied zoom-dimension {} exceeds the image dimensionality of 0 to {}.".format(
+                dimension, image.ndim - 1
+            )
+        )
+
     # get logger
     logger = Logger.getInstance()
 
-    logger.debug('Old shape = {}.'.format(image.shape))
+    logger.debug("Old shape = {}.".format(image.shape))
 
     # perform the zoom
     zoom = [1] * image.ndim
-    zoom[dimension] = (image.shape[dimension] + (image.shape[dimension] - 1) * factor) / float(image.shape[dimension])
-    logger.debug('Reshaping with = {}.'.format(zoom))
+    zoom[dimension] = (
+        image.shape[dimension] + (image.shape[dimension] - 1) * factor
+    ) / float(image.shape[dimension])
+    logger.debug("Reshaping with = {}.".format(zoom))
     image = interpolation.zoom(image, zoom, order=order)
-        
-    logger.debug('New shape = {}.'.format(image.shape))
-    
+
+    logger.debug("New shape = {}.".format(image.shape))
+
     if hdr:
         new_spacing = list(header.get_pixel_spacing(hdr))
         new_spacing[dimension] = new_spacing[dimension] / float(factor + 1)
-        logger.debug('Setting pixel spacing from {} to {}....'.format(header.get_pixel_spacing(hdr), new_spacing))
+        logger.debug(
+            "Setting pixel spacing from {} to {}....".format(
+                header.get_pixel_spacing(hdr), new_spacing
+            )
+        )
         header.set_pixel_spacing(hdr, tuple(new_spacing))
-    
+
     return image, hdr
-    
+
+
 def getArguments(parser):
     "Provides additional validation of the arguments collected by argparse."
     return parser.parse_args()
 
+
 def getParser():
     "Creates and returns the argparse parser object."
-    parser = argparse.ArgumentParser(description=__description__, formatter_class=argparse.RawTextHelpFormatter)
-    parser.add_argument('input', help='Source volume.')
-    parser.add_argument('output', help='Target volume.')
-    parser.add_argument('dimension', type=int, help='The dimension along which to zoom.')
-    parser.add_argument('enhancement', type=int, help='How many slices to put between each original slice.')
-    #parser.add_argument('-o', dest='objects', action='store_true', help='Activate this flag to perform the zoom for any binary object in the image separatly.')
-    parser.add_argument('-v', dest='verbose', action='store_true', help='Display more information.')
-    parser.add_argument('-d', dest='debug', action='store_true', help='Display debug information.')
-    parser.add_argument('-f', dest='force', action='store_true', help='Silently override existing output images.')
+    parser = argparse.ArgumentParser(
+        description=__description__, formatter_class=argparse.RawTextHelpFormatter
+    )
+    parser.add_argument("input", help="Source volume.")
+    parser.add_argument("output", help="Target volume.")
+    parser.add_argument(
+        "dimension", type=int, help="The dimension along which to zoom."
+    )
+    parser.add_argument(
+        "enhancement",
+        type=int,
+        help="How many slices to put between each original slice.",
+    )
+    # parser.add_argument('-o', dest='objects', action='store_true', help='Activate this flag to perform the zoom for any binary object in the image separatly.')
+    parser.add_argument(
+        "-v", dest="verbose", action="store_true", help="Display more information."
+    )
+    parser.add_argument(
+        "-d", dest="debug", action="store_true", help="Display debug information."
+    )
+    parser.add_argument(
+        "-f",
+        dest="force",
+        action="store_true",
+        help="Silently override existing output images.",
+    )
     return parser
 
+
 if __name__ == "__main__":
-    main()     
+    main()
```

### Comparing `MedPy-0.4.0/bin/medpy_extract_contour.py` & `MedPy-0.5.0/bin/medpy_stack_sub_volumes.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 
 """
-Convert a binary volume into a surface contour.
+Stacks a number of volumes into one dimension.
 
 Copyright (C) 2013 Oskar Maier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
@@ -15,115 +15,147 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
-# build-in modules
 import argparse
 import logging
-import math
+
+# build-in modules
+from argparse import RawTextHelpFormatter
 
 # third-party modules
 import numpy
-from scipy.ndimage.morphology import binary_erosion, binary_dilation,\
-    generate_binary_structure
-
-# path changes
 
 # own modules
 from medpy.core import Logger
 from medpy.io import load, save
 
+# path changes
+
 
 # information
 __author__ = "Oskar Maier"
-__version__ = "r0.1.0, 2014-06-04"
+__version__ = "r0.3.1, 2011-03-29"
 __email__ = "oskar.maier@googlemail.com"
 __status__ = "Release"
 __description__ = """
-                  Converts a binary volume into a surface contour. In the case of an even
-                  contour width, the surface of the volume will correspond with the
-                  middle of the contour line. In the case of an odd contour width, the
-                  contour will be shifted by one voxel towards the inside of the volume.
-                  
-                  In the case of 3D volumes, the contours result in shells, which might
-                  not be desired, as they do not visualize well in 2D views. With the
-                  '--dimension' argument, a dimension along which to extract the contours
-                  can be supplied.
-                  
+                  Takes a arbitrary number of medical images that are of equal depth in
+                  all but one dimension. The images are then stacked on top of each other
+                  to produce a single result image. The dimension in which to stack is
+                  supplied by the dimension parameter.
+
+                  Note that the supplied images must be of the same data type.
+                  Note to take into account the input images orientations.
+
                   Copyright (C) 2013 Oskar Maier
                   This program comes with ABSOLUTELY NO WARRANTY; This is free software,
                   and you are welcome to redistribute it under certain conditions; see
-                  the LICENSE file or <http://www.gnu.org/licenses/> for details.   
+                  the LICENSE file or <http://www.gnu.org/licenses/> for details.
                   """
 
+
 # code
 def main():
-    args = getArguments(getParser())
+    # parse cmd arguments
+    parser = getParser()
+    parser.parse_args()
+    args = getArguments(parser)
 
     # prepare logger
     logger = Logger.getInstance()
-    if args.debug: logger.setLevel(logging.DEBUG)
-    elif args.verbose: logger.setLevel(logging.INFO)
-    
-    # load input image
-    data_input, header_input = load(args.input)
-    
-    # treat as binary
-    data_input = data_input.astype(numpy.bool)
-    
+    if args.debug:
+        logger.setLevel(logging.DEBUG)
+    elif args.verbose:
+        logger.setLevel(logging.INFO)
+
+    # load first image as result image
+    logger.info("Loading {}...".format(args.images[0]))
+    result_data, result_header = load(args.images[0])
+
     # check dimension argument
-    if args.dimension and (not args.dimension >= 0 or not args.dimension < data_input.ndim):
-        argparse.ArgumentError(args.dimension, 'Invalid dimension of {} supplied. Image has only {} dimensions.'.format(args.dimension, data_input.ndim))
-        
-    # compute erosion and dilation steps
-    erosions = int(math.ceil(args.width / 2.))
-    dilations = int(math.floor(args.width / 2.))
-    logger.debug("Performing {} erosions and {} dilations to achieve a contour of width {}.".format(erosions, dilations, args.width))
-    
-    # erode, dilate and compute contour
-    if not args.dimension:
-        eroded = binary_erosion(data_input, iterations=erosions) if not 0 == erosions else data_input
-        dilated = binary_dilation(data_input, iterations=dilations) if not 0 == dilations else data_input
-        data_output = dilated - eroded
-    else:
-        slicer = [slice(None)] * data_input.ndim
-        bs_slicer = [slice(None)] * data_input.ndim
-        data_output = numpy.zeros_like(data_input)
-        for sl in range(data_input.shape[args.dimension]):
-            slicer[args.dimension] = slice(sl, sl+1)
-            bs_slicer[args.dimension] = slice(1, 2)
-            bs = generate_binary_structure(data_input.ndim, 1)
-            
-            eroded = binary_erosion(data_input[slicer], structure=bs[bs_slicer], iterations=erosions) if not 0 == erosions else data_input[slicer]
-            dilated = binary_dilation(data_input[slicer], structure=bs[bs_slicer], iterations=dilations) if not 0 == dilations else data_input[slicer]
-            data_output[slicer] = dilated - eroded
-    logger.debug("Contour image contains {} contour voxels.".format(numpy.count_nonzero(data_output)))
-
-    # save resulting volume
-    save(data_output, args.output, header_input, args.force)
-    
-    logger.info("Successfully terminated.")    
-    
+    if args.dimension >= result_data.ndim:
+        raise argparse.ArgumentError(
+            "The supplied stack-dimension {} exceeds the image dimensionality of 0 to {}.".format(
+                args.dimension, result_data.ndim - 1
+            )
+        )
+
+    # reduce the image dimensions
+    if args.zero and result_data.all():
+        result_data = numpy.zeros(result_data.shape, result_data.dtype)
+
+    # iterate over remaining images and concatenate
+    for image_name in args.images[1:]:
+        logger.info("Loading {}...".format(image_name))
+        image_data, _ = load(image_name)
+
+        # change to zero matrix if requested
+        if args.zero and image_data.all():
+            image_data = numpy.zeros(image_data.shape, image_data.dtype)
+
+        # concatenate
+        if args.reversed:
+            result_data = numpy.concatenate((image_data, result_data), args.dimension)
+        else:
+            result_data = numpy.concatenate((result_data, image_data), args.dimension)
+
+    logger.debug("Final image is of shape {}.".format(result_data.shape))
+
+    # save results in same format as input image
+    logger.info("Saving concatenated image as {}...".format(args.output))
+
+    save(result_data, args.output, result_header, args.force)
+
+    logger.info("Successfully terminated.")
+
+
 def getArguments(parser):
     "Provides additional validation of the arguments collected by argparse."
-    args = parser.parse_args()
-    if args.width <= 0:
-        raise argparse.ArgumentError(args.width, 'The contour width must be a positive number.')
-    return args
+    return parser.parse_args()
+
 
 def getParser():
     "Creates and returns the argparse parser object."
-    parser = argparse.ArgumentParser(description=__description__)
-    parser.add_argument('input', help='Source volume.')
-    parser.add_argument('output', help='Target volume.')
-    parser.add_argument('-w', '--width', dest='width', type=int, default=1, help='Width of the contour.')
-    parser.add_argument('--dimension', type=int, help='Extract contours only along this dimension.')
-    parser.add_argument('-v', dest='verbose', action='store_true', help='Display more information.')
-    parser.add_argument('-d', dest='debug', action='store_true', help='Display debug information.')
-    parser.add_argument('-f', dest='force', action='store_true', help='Silently override existing output images.')
-    return parser    
+    parser = argparse.ArgumentParser(
+        description=__description__, formatter_class=RawTextHelpFormatter
+    )
+
+    parser.add_argument(
+        "dimension",
+        type=int,
+        help="The dimension in which direction to stack (starting from 0:x).",
+    )
+    parser.add_argument("output", help="The output image.")
+    parser.add_argument("images", nargs="+", help="The images to concatenate/stack.")
+    parser.add_argument(
+        "-f",
+        dest="force",
+        action="store_true",
+        help="Set this flag to silently override files that exist.",
+    )
+    parser.add_argument(
+        "-v", dest="verbose", action="store_true", help="Display more information."
+    )
+    parser.add_argument(
+        "-d", dest="debug", action="store_true", help="Display debug information."
+    )
+    parser.add_argument(
+        "-z",
+        dest="zero",
+        action="store_true",
+        help="If supplied, all images containing only 1s are treated as empty image.",
+    )
+    parser.add_argument(
+        "-r",
+        dest="reversed",
+        action="store_true",
+        help="Stack in resversed order as how the files are supplied.",
+    )
+
+    return parser
+
 
 if __name__ == "__main__":
-    main()        
+    main()
```

### Comparing `MedPy-0.4.0/bin/medpy_binary_resampling.py` & `MedPy-0.5.0/bin/medpy_binary_resampling.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,30 +15,29 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
+import argparse
+import logging
+
 # build-in modules
 import os
-import logging
-import argparse
 
 # third-party modules
 import numpy
-from scipy.ndimage.interpolation import zoom
-from scipy.ndimage.morphology import distance_transform_edt, binary_erosion
-from scipy.ndimage.measurements import label
+from scipy.ndimage import binary_erosion, distance_transform_edt, label, zoom
 
 # own modules
 from medpy.core import Logger
-from medpy.filter import resample, bounding_box
+from medpy.filter import resample
+from medpy.io import header, load, save
 from medpy.utilities import argparseu
-from medpy.io import load, save, header
 
 # information
 __author__ = "Oskar Maier"
 __version__ = "r0.1.0, 2014-11-25"
 __email__ = "oskar.maier@googlemail.com"
 __status__ = "Release"
 __description__ = """
@@ -54,124 +53,137 @@
 necessary.
 
 Note that the pixel data type of the input image is treated as binary.
 
 Copyright (C) 2013 Oskar Maier
 This program comes with ABSOLUTELY NO WARRANTY; This is free software,
 and you are welcome to redistribute it under certain conditions; see
-the LICENSE file or <http://www.gnu.org/licenses/> for details.   
+the LICENSE file or <http://www.gnu.org/licenses/> for details.
 """
 
+
 # code
 def main():
     parser = getParser()
     args = getArguments(parser)
 
     # prepare logger
     logger = Logger.getInstance()
-    if args.debug: logger.setLevel(logging.DEBUG)
-    elif args.verbose: logger.setLevel(logging.INFO)
-    
+    if args.debug:
+        logger.setLevel(logging.DEBUG)
+    elif args.verbose:
+        logger.setLevel(logging.INFO)
+
     # loading input images
     img, hdr = load(args.input)
-    img = img.astype(numpy.bool)
-    
+    img = img.astype(numpy.bool_)
+
     # check spacing values
     if not len(args.spacing) == img.ndim:
-        parser.error('The image has {} dimensions, but {} spacing parameters have been supplied.'.format(img.ndim, len(args.spacing)))
-        
+        parser.error(
+            "The image has {} dimensions, but {} spacing parameters have been supplied.".format(
+                img.ndim, len(args.spacing)
+            )
+        )
+
     # check if output image exists
     if not args.force:
         if os.path.exists(args.output):
-            parser.error('The output image {} already exists.'.format(args.output)) 
-        
-    logger.debug('target voxel spacing: {}'.format(args.spacing))
-    
+            parser.error("The output image {} already exists.".format(args.output))
+
+    logger.debug("target voxel spacing: {}".format(args.spacing))
+
     # determine number of required complete slices for up-sampling
     vs = header.get_pixel_spacing(hdr)
-    rcss = [int(y // x - 1) for x, y in zip(args.spacing, vs)] # TODO: For option b, remove the - 1; better: no option b, since I am rounding later anyway
-    
+    rcss = [
+        int(y // x - 1) for x, y in zip(args.spacing, vs)
+    ]  # TODO: For option b, remove the - 1; better: no option b, since I am rounding later anyway
+
     # remove negatives and round up to next even number
     rcss = [x if x > 0 else 0 for x in rcss]
     rcss = [x if 0 == x % 2 else x + 1 for x in rcss]
-    logger.debug('intermediate slices to add per dimension: {}'.format(rcss))
-    
+    logger.debug("intermediate slices to add per dimension: {}".format(rcss))
+
     # for each dimension requiring up-sampling, from the highest down, perform shape based slice interpolation
-    logger.info('Adding required slices using shape based interpolation.')
+    logger.info("Adding required slices using shape based interpolation.")
     for dim, rcs in enumerate(rcss):
         if rcs > 0:
-            logger.debug('adding {} intermediate slices to dimension {}'.format(rcs, dim))
+            logger.debug(
+                "adding {} intermediate slices to dimension {}".format(rcs, dim)
+            )
             img = shape_based_slice_interpolation(img, dim, rcs)
-            logger.debug('resulting new image shape: {}'.format(img.shape))
-            
+            logger.debug("resulting new image shape: {}".format(img.shape))
+
     # compute and set new voxel spacing
-    nvs = [x / (y + 1.) for x, y in zip(vs, rcss)]
+    nvs = [x / (y + 1.0) for x, y in zip(vs, rcss)]
     header.set_pixel_spacing(hdr, nvs)
-    logger.debug('intermediate voxel spacing: {}'.format(nvs))
-    
+    logger.debug("intermediate voxel spacing: {}".format(nvs))
+
     # interpolate with nearest neighbour
-    logger.info('Re-sampling the image with a b-spline order of {}.'.format(args.order))
-    img, hdr = resample(img, hdr, args.spacing, args.order, mode='nearest')
-    
+    logger.info("Re-sampling the image with a b-spline order of {}.".format(args.order))
+    img, hdr = resample(img, hdr, args.spacing, args.order, mode="nearest")
+
     # saving the resulting image
     save(img, args.output, hdr, args.force)
-    
+
+
 def shape_based_slice_interpolation(img, dim, nslices):
     """
     Adds `nslices` slices between all slices of the binary image `img` along dimension
     `dim` respecting the original slice values to be situated in the middle of each
     slice. Extrapolation situations are handled by simple repeating.
-    
+
     Interpolation of new slices is performed using shape based interpolation.
-    
+
     Parameters
     ----------
     img : array_like
         A n-dimensional image.
     dim : int
         The dimension along which to add slices.
     nslices : int
         The number of slices to add. Must be an even number.
-    
+
     Returns
     -------
     out : ndarray
         The re-sampled image.
     """
     # check arguments
     if not 0 == nslices % 2:
-        raise ValueError('nslices must be an even number')
-    
+        raise ValueError("nslices must be an even number")
+
     out = None
     slicer = [slice(None)] * img.ndim
     chunk_full_shape = list(img.shape)
     chunk_full_shape[dim] = nslices + 2
-     
+
     for sl1, sl2 in zip(numpy.rollaxis(img, dim)[:-1], numpy.rollaxis(img, dim)[1:]):
         if 0 == numpy.count_nonzero(sl1) and 0 == numpy.count_nonzero(sl2):
-            chunk = numpy.zeros(chunk_full_shape, dtype=numpy.bool)
+            chunk = numpy.zeros(chunk_full_shape, dtype=numpy.bool_)
         else:
             chunk = shape_based_slice_insertation_object_wise(sl1, sl2, dim, nslices)
         if out is None:
             out = numpy.delete(chunk, -1, dim)
         else:
             out = numpy.concatenate((out, numpy.delete(chunk, -1, dim)), dim)
-    
-    slicer[dim] = numpy.newaxis    
-    out = numpy.concatenate((out, sl2[slicer]), dim)
-    
+
+    slicer[dim] = numpy.newaxis
+    out = numpy.concatenate((out, sl2[tuple(slicer)]), dim)
+
     slicer[dim] = slice(0, 1)
     for _ in range(nslices // 2):
-        out = numpy.concatenate((img[slicer], out), dim)
+        out = numpy.concatenate((img[tuple(slicer)], out), dim)
     slicer[dim] = slice(-1, None)
     for _ in range(nslices // 2):
-        out = numpy.concatenate((out, img[slicer]), dim)
-        
+        out = numpy.concatenate((out, img[tuple(slicer)]), dim)
+
     return out
 
+
 def shape_based_slice_insertation_object_wise(sl1, sl2, dim, nslices, order=3):
     """
     Wrapper to apply `shape_based_slice_insertation()` for each binary object
     separately to ensure correct extrapolation behaviour.
     """
     out = None
     sandwich = numpy.concatenate((sl1[numpy.newaxis], sl2[numpy.newaxis]), 0)
@@ -180,94 +192,122 @@
         _sl1, _sl2 = label_image == lid
         _out = shape_based_slice_insertation(_sl1, _sl2, dim, nslices, order=3)
         if out is None:
             out = _out
         else:
             out |= _out
     return out
-    
+
+
 def shape_based_slice_insertation(sl1, sl2, dim, nslices, order=3):
     """
     Insert `nslices` new slices between `sl1` and `sl2` along dimension `dim` using shape
     based binary interpolation.
-    
+
     Extrapolation is handled adding `nslices`/2 step-wise eroded copies of the last slice
     in each direction.
-    
+
     Parameters
     ----------
     sl1 : array_like
         First slice. Treated as binary data.
     sl2 : array_like
         Second slice. Treated as binary data.
     dim : int
         The new dimension along which to add the new slices.
     nslices : int
         The number of slices to add.
     order : int
         The b-spline interpolation order for re-sampling the distance maps.
-        
+
     Returns
     -------
     out : ndarray
         A binary image of size `sl1`.shape() extend by `nslices`+2 along the new
         dimension `dim`. The border slices are the original slices `sl1` and `sl2`.
     """
-    sl1 = sl1.astype(numpy.bool)
-    sl2 = sl2.astype(numpy.bool)
-    
+    sl1 = sl1.astype(numpy.bool_)
+    sl2 = sl2.astype(numpy.bool_)
+
     # extrapolation through erosion
     if 0 == numpy.count_nonzero(sl1):
         slices = [sl1]
         for _ in range(nslices / 2):
             slices.append(numpy.zeros_like(sl1))
         for i in range(1, nslices / 2 + nslices % 2 + 1)[::-1]:
             slices.append(binary_erosion(sl2, iterations=i))
         slices.append(sl2)
         return numpy.rollaxis(numpy.asarray(slices), 0, dim + 1)
-        #return numpy.asarray([sl.T for sl in slices]).T
-    elif 0 ==numpy.count_nonzero(sl2):
+        # return numpy.asarray([sl.T for sl in slices]).T
+    elif 0 == numpy.count_nonzero(sl2):
         slices = [sl1]
         for i in range(1, nslices / 2 + 1):
             slices.append(binary_erosion(sl1, iterations=i))
         for _ in range(0, nslices / 2 + nslices % 2):
             slices.append(numpy.zeros_like(sl2))
         slices.append(sl2)
         return numpy.rollaxis(numpy.asarray(slices), 0, dim + 1)
-        #return numpy.asarray([sl.T for sl in slices]).T
-    
-    # interpolation shape based 
+        # return numpy.asarray([sl.T for sl in slices]).T
+
+    # interpolation shape based
     # note: distance_transform_edt shows strange behaviour for ones-arrays
     dt1 = distance_transform_edt(~sl1) - distance_transform_edt(sl1)
     dt2 = distance_transform_edt(~sl2) - distance_transform_edt(sl2)
-    
+
     slicer = [slice(None)] * dt1.ndim
     slicer = slicer[:dim] + [numpy.newaxis] + slicer[dim:]
-    out = numpy.concatenate((dt1[slicer], dt2[slicer]), axis=dim)
+    out = numpy.concatenate((dt1[tuple(slicer)], dt2[tuple(slicer)]), axis=dim)
     zoom_factors = [1] * dt1.ndim
-    zoom_factors = zoom_factors[:dim] + [(nslices + 2)/2.] + zoom_factors[dim:]
+    zoom_factors = zoom_factors[:dim] + [(nslices + 2) / 2.0] + zoom_factors[dim:]
     out = zoom(out, zoom_factors, order=order)
-    
+
     return out <= 0
-    
+
+
 def getArguments(parser):
     "Provides additional validation of the arguments collected by argparse."
     args = parser.parse_args()
     if args.order < 0 or args.order > 5:
-        parser.error('The order has to be a number between 0 and 5.')   
+        parser.error("The order has to be a number between 0 and 5.")
     return args
 
+
 def getParser():
     "Creates and returns the argparse parser object."
-    parser = argparse.ArgumentParser(formatter_class=argparse.RawDescriptionHelpFormatter, description=__description__)
-    parser.add_argument('input', help='the input image')
-    parser.add_argument('output', help='the output image')
-    parser.add_argument('spacing', type=argparseu.sequenceOfFloatsGt, help='the desired voxel spacing in colon-separated values, e.g. 1.2,1.2,5.0')
-    parser.add_argument('-o', '--order', type=int, default=0, dest='order', help='the bspline order, default is 0 (= nearest neighbour)')
-
-    parser.add_argument('-v', '--verbose', dest='verbose', action='store_true', help='verbose output')
-    parser.add_argument('-d', dest='debug', action='store_true', help='Display debug information.')
-    parser.add_argument('-f', '--force', dest='force', action='store_true', help='overwrite existing files')
+    parser = argparse.ArgumentParser(
+        formatter_class=argparse.RawDescriptionHelpFormatter,
+        description=__description__,
+    )
+    parser.add_argument("input", help="the input image")
+    parser.add_argument("output", help="the output image")
+    parser.add_argument(
+        "spacing",
+        type=argparseu.sequenceOfFloatsGt,
+        help="the desired voxel spacing in colon-separated values, e.g. 1.2,1.2,5.0",
+    )
+    parser.add_argument(
+        "-o",
+        "--order",
+        type=int,
+        default=0,
+        dest="order",
+        help="the bspline order, default is 0 (= nearest neighbour)",
+    )
+
+    parser.add_argument(
+        "-v", "--verbose", dest="verbose", action="store_true", help="verbose output"
+    )
+    parser.add_argument(
+        "-d", dest="debug", action="store_true", help="Display debug information."
+    )
+    parser.add_argument(
+        "-f",
+        "--force",
+        dest="force",
+        action="store_true",
+        help="overwrite existing files",
+    )
     return parser
-    
+
+
 if __name__ == "__main__":
-    main()    
+    main()
```

### Comparing `MedPy-0.4.0/bin/medpy_watershed.py` & `MedPy-0.5.0/bin/medpy_watershed.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,96 +23,124 @@
 # build-in modules
 import argparse
 import logging
 import os
 
 # third-party modules
 import numpy
-from scipy.ndimage.measurements import label
-from skimage.morphology import watershed
+from scipy.ndimage import label
+from skimage.segmentation import watershed
 
-# path changes
+from medpy.core import ArgumentError, Logger
+from medpy.filter import local_minima
 
 # own modules
 from medpy.io import load, save
-from medpy.core import Logger, ArgumentError
-from medpy.filter import local_minima
+
+# path changes
 
 
 # information
 __author__ = "Oskar Maier"
-__version__ = "r0.1.1, 2013-12-11"
+__version__ = "r0.1.2, 2013-12-11"
 __email__ = "oskar.maier@googlemail.com"
 __status__ = "Release"
 __description__ = """
                   Applies the watershed segmentation an image using the supplied
                   parameters.
                   Note that this version does not take the voxel-spacing into account.
-                                  
+
                   Copyright (C) 2013 Oskar Maier
                   This program comes with ABSOLUTELY NO WARRANTY; This is free software,
                   and you are welcome to redistribute it under certain conditions; see
-                  the LICENSE file or <http://www.gnu.org/licenses/> for details.   
+                  the LICENSE file or <http://www.gnu.org/licenses/> for details.
                   """
 
+
 # code
 def main():
     # parse cmd arguments
     parser = getParser()
     parser.parse_args()
     args = getArguments(parser)
-    
+
     # prepare logger
     logger = Logger.getInstance()
-    if args.debug: logger.setLevel(logging.DEBUG)
-    elif args.verbose: logger.setLevel(logging.INFO)
-    
+    if args.debug:
+        logger.setLevel(logging.DEBUG)
+    elif args.verbose:
+        logger.setLevel(logging.INFO)
+
     # check if output image exists (will also be performed before saving, but as the watershed might be very time intensity, a initial check can save frustration)
     if not args.force:
         if os.path.exists(args.output):
-            raise ArgumentError('The output image {} already exists.'.format(args.output))
-    
+            raise ArgumentError(
+                "The output image {} already exists.".format(args.output)
+            )
+
     # loading images
     data_input, header_input = load(args.input)
     if args.mask:
-        mask = load(args.mask)[0].astype(numpy.bool)
+        mask = load(args.mask)[0].astype(numpy.bool_)
     else:
         mask = None
-    
+
     # extract local minima and convert to markers
-    logger.info('Extract local minima with minimum distance of {}...'.format(args.mindist))
+    logger.info(
+        "Extract local minima with minimum distance of {}...".format(args.mindist)
+    )
     lm, _ = local_minima(data_input, args.mindist)
     lm_indices = tuple([numpy.asarray(x) for x in lm.T])
     minima_labels = numpy.zeros(data_input.shape, dtype=numpy.uint64)
     minima_labels[lm_indices] = 1
     if not None == mask:
         minima_labels[~mask] = 0
     minima_labels, _ = label(minima_labels)
-    
+
     # apply the watershed
-    logger.info('Watershedding...')
+    logger.info("Watershedding...")
     data_output = watershed(data_input, minima_labels, mask=mask)
 
     # save file
     save(data_output, args.output, header_input, args.force)
-    
-    logger.info('Successfully terminated.')
+
+    logger.info("Successfully terminated.")
+
 
 def getArguments(parser):
     "Provides additional validation of the arguments collected by argparse."
     return parser.parse_args()
 
+
 def getParser():
     "Creates and returns the argparse parser object."
     parser = argparse.ArgumentParser(description=__description__)
-    parser.add_argument('input', help='Source volume (usually a gradient image).')
-    parser.add_argument('output', help='Target volume.')
-    parser.add_argument('--mindist', type=int, default=2, help='The minimum distance between local minima in voxel units.')
-    parser.add_argument('--mask', help='Optional binary mask image denoting the area over which to compute the watershed.')
-    parser.add_argument('-v', dest='verbose', action='store_true', help='Display more information.')
-    parser.add_argument('-d', dest='debug', action='store_true', help='Display debug information.')
-    parser.add_argument('-f', dest='force', action='store_true', help='Silently override existing output images.')
-    
+    parser.add_argument("input", help="Source volume (usually a gradient image).")
+    parser.add_argument("output", help="Target volume.")
+    parser.add_argument(
+        "--mindist",
+        type=int,
+        default=2,
+        help="The minimum distance between local minima in voxel units.",
+    )
+    parser.add_argument(
+        "--mask",
+        help="Optional binary mask image denoting the area over which to compute the watershed.",
+    )
+    parser.add_argument(
+        "-v", dest="verbose", action="store_true", help="Display more information."
+    )
+    parser.add_argument(
+        "-d", dest="debug", action="store_true", help="Display debug information."
+    )
+    parser.add_argument(
+        "-f",
+        dest="force",
+        action="store_true",
+        help="Silently override existing output images.",
+    )
+
     return parser
-    
+
+
 if __name__ == "__main__":
     main()
```

### Comparing `MedPy-0.4.0/bin/medpy_graphcut_label.py` & `MedPy-0.5.0/bin/medpy_graphcut_label.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,154 +15,198 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
-# build-in modules
-from argparse import RawTextHelpFormatter
 import argparse
 import logging
 import os
 
+# build-in modules
+from argparse import RawTextHelpFormatter
+
 # third-party modules
-import scipy
+import numpy
 
-# path changes
+from medpy import filter, graphcut
 
 # own modules
 from medpy.core import ArgumentError, Logger
-from medpy.io import load, save
-from medpy import graphcut
-from medpy import filter
 from medpy.graphcut.wrapper import split_marker
+from medpy.io import load, save
 
+# path changes
 
 
 # information
 __author__ = "Oskar Maier"
 __version__ = "r0.4.4, 2012-03-16"
 __email__ = "oskar.maier@googlemail.com"
 __status__ = "Release"
 __description__ = """
                   Perform a binary graph cut using Boykov's max-flow/min-cut algorithm.
-                  
+
                   This implementation does only compute a boundary term and does not use
                   any regional term. The desired boundary term can be selected via the
                   --boundary argument. Depending on the selected term, an additional
                   image has to be supplied as badditional.
-                  
+
                   In the case of the stawiaski boundary term, this is the gradient image.
                   In the case of the difference of means, it is the original image.
-                  
+
                   Furthermore the algorithm requires the region map of the original
                   image and an integer image with foreground and background markers.
-                  
+
                   Additionally a filename for the created binary mask marking foreground
                   and background has to be supplied.
-                  
+
                   Note that the input images must be of the same dimensionality,
                   otherwise an exception is thrown.
                   Note to take into account the input images orientation.
                   Note that the quality of the resulting segmentations depends also on
                   the quality of the supplied markers.
-                  
+
                   Copyright (C) 2013 Oskar Maier
                   This program comes with ABSOLUTELY NO WARRANTY; This is free software,
                   and you are welcome to redistribute it under certain conditions; see
-                  the LICENSE file or <http://www.gnu.org/licenses/> for details.   
+                  the LICENSE file or <http://www.gnu.org/licenses/> for details.
                   """
 
+
 # code
 def main():
     # parse cmd arguments
     parser = getParser()
     parser.parse_args()
     args = getArguments(parser)
-    
+
     # prepare logger
     logger = Logger.getInstance()
-    if args.debug: logger.setLevel(logging.DEBUG)
-    elif args.verbose: logger.setLevel(logging.INFO)
-        
+    if args.debug:
+        logger.setLevel(logging.DEBUG)
+    elif args.verbose:
+        logger.setLevel(logging.INFO)
+
     # check if output image exists
     if not args.force:
         if os.path.exists(args.output):
-            logger.warning('The output image {} already exists. Exiting.'.format(args.output))
+            logger.warning(
+                "The output image {} already exists. Exiting.".format(args.output)
+            )
             exit(-1)
-            
+
     # select boundary term
-    if args.boundary == 'stawiaski':
+    if args.boundary == "stawiaski":
         boundary_term = graphcut.energy_label.boundary_stawiaski
-        logger.info('Selected boundary term: stawiaski')
+        logger.info("Selected boundary term: stawiaski")
     else:
         boundary_term = graphcut.energy_label.boundary_difference_of_means
-        logger.info('Selected boundary term: difference of means')
+        logger.info("Selected boundary term: difference of means")
 
     # load input images
     region_image_data, reference_header = load(args.region)
     badditional_image_data, _ = load(args.badditional)
     markers_image_data, _ = load(args.markers)
-    
+
     # split marker image into fg and bg images
     fgmarkers_image_data, bgmarkers_image_data = split_marker(markers_image_data)
-       
+
     # check if all images dimensions are the same
-    if not (badditional_image_data.shape == region_image_data.shape == fgmarkers_image_data.shape == bgmarkers_image_data.shape):
-        logger.critical('Not all of the supplied images are of the same shape.')
-        raise ArgumentError('Not all of the supplied images are of the same shape.')
-       
+    if not (
+        badditional_image_data.shape
+        == region_image_data.shape
+        == fgmarkers_image_data.shape
+        == bgmarkers_image_data.shape
+    ):
+        logger.critical("Not all of the supplied images are of the same shape.")
+        raise ArgumentError("Not all of the supplied images are of the same shape.")
+
     # recompute the label ids to start from id = 1
-    logger.info('Relabel input image...')
+    logger.info("Relabel input image...")
     region_image_data = filter.relabel(region_image_data)
 
     # generate graph
-    logger.info('Preparing graph...')
-    gcgraph = graphcut.graph_from_labels(region_image_data,
-                                    fgmarkers_image_data,
-                                    bgmarkers_image_data,
-                                    boundary_term = boundary_term,
-                                    boundary_term_args = (badditional_image_data)) # second is directedness of graph , 0)
+    logger.info("Preparing graph...")
+    gcgraph = graphcut.graph_from_labels(
+        region_image_data,
+        fgmarkers_image_data,
+        bgmarkers_image_data,
+        boundary_term=boundary_term,
+        boundary_term_args=(badditional_image_data),
+    )  # second is directedness of graph , 0)
 
-    logger.info('Removing images that are not longer required from memory...')
+    logger.info("Removing images that are not longer required from memory...")
     del fgmarkers_image_data
     del bgmarkers_image_data
     del badditional_image_data
-    
+
     # execute min-cut
-    logger.info('Executing min-cut...')
+    logger.info("Executing min-cut...")
     maxflow = gcgraph.maxflow()
-    logger.debug('Maxflow is {}'.format(maxflow))
-    
+    logger.debug("Maxflow is {}".format(maxflow))
+
     # apply results to the region image
-    logger.info('Applying results...')
-    mapping = [0] # no regions with id 1 exists in mapping, entry used as padding
-    mapping.extend([0 if gcgraph.termtype.SINK == gcgraph.what_segment(int(x) - 1) else 1 for x in scipy.unique(region_image_data)])
+    logger.info("Applying results...")
+    mapping = [0]  # no regions with id 1 exists in mapping, entry used as padding
+    mapping.extend(
+        [
+            0 if gcgraph.termtype.SINK == gcgraph.what_segment(int(x) - 1) else 1
+            for x in numpy.unique(region_image_data)
+        ]
+    )
     region_image_data = filter.relabel_map(region_image_data, mapping)
-    
+
     # save resulting mask
-    save(region_image_data.astype(scipy.bool_), args.output, reference_header, args.force)
+    save(
+        region_image_data.astype(numpy.bool_), args.output, reference_header, args.force
+    )
+
+    logger.info("Successfully terminated.")
 
-    logger.info('Successfully terminated.')
 
 def getArguments(parser):
     "Provides additional validation of the arguments collected by argparse."
     return parser.parse_args()
 
+
 def getParser():
     "Creates and returns the argparse parser object."
-    parser = argparse.ArgumentParser(description=__description__, formatter_class=RawTextHelpFormatter)
-    
-    parser.add_argument('badditional', help='The additional image required by the boundary term. See there for details.')
-    parser.add_argument('region', help='The region image of the image to segment.')
-    parser.add_argument('markers', help='Binary image containing the foreground (=1) and background (=2) markers.')
-    parser.add_argument('output', help='The output image containing the segmentation.')
-    parser.add_argument('--boundary', default='stawiaski', help='The boundary term to use. Note that difference of means (means) requires the original image, while stawiaski requires the gradient image of the original image to be passed to badditional.', choices=['means', 'stawiaski'])
-    parser.add_argument('-f', dest='force', action='store_true', help='Set this flag to silently override files that exist.')
-    parser.add_argument('-v', dest='verbose', action='store_true', help='Display more information.')
-    parser.add_argument('-d', dest='debug', action='store_true', help='Display debug information.')
-    
-    return parser    
+    parser = argparse.ArgumentParser(
+        description=__description__, formatter_class=RawTextHelpFormatter
+    )
+
+    parser.add_argument(
+        "badditional",
+        help="The additional image required by the boundary term. See there for details.",
+    )
+    parser.add_argument("region", help="The region image of the image to segment.")
+    parser.add_argument(
+        "markers",
+        help="Binary image containing the foreground (=1) and background (=2) markers.",
+    )
+    parser.add_argument("output", help="The output image containing the segmentation.")
+    parser.add_argument(
+        "--boundary",
+        default="stawiaski",
+        help="The boundary term to use. Note that difference of means (means) requires the original image, while stawiaski requires the gradient image of the original image to be passed to badditional.",
+        choices=["means", "stawiaski"],
+    )
+    parser.add_argument(
+        "-f",
+        dest="force",
+        action="store_true",
+        help="Set this flag to silently override files that exist.",
+    )
+    parser.add_argument(
+        "-v", dest="verbose", action="store_true", help="Display more information."
+    )
+    parser.add_argument(
+        "-d", dest="debug", action="store_true", help="Display debug information."
+    )
+
+    return parser
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `MedPy-0.4.0/bin/medpy_dicom_slices_to_volume.py` & `MedPy-0.5.0/bin/medpy_convert.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,88 +1,107 @@
 #!/usr/bin/env python
 
 """
-Converts a collection of DICOM slices into a proper image volume.
+Convert an image from one format into another.
 
 Copyright (C) 2013 Oskar Maier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>."""
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
 
 # build-in modules
 import argparse
 import logging
 
-# third-party modules
-
-# path changes
-
 # own modules
 from medpy.core import Logger
 from medpy.io import load, save
 
+# third-party modules
+
+# path changes
+
 
 # information
 __author__ = "Oskar Maier"
-__version__ = "r0.2.1, 2012-06-13"
+__version__ = "r0.1.1, 2012-05-25"
 __email__ = "oskar.maier@googlemail.com"
 __status__ = "Release"
 __description__ = """
-                  Converts a collection of DICOM slices (a DICOM series) into a proper
-                  image volume. Note that this operation does not preserve header
-                  information.
-                  
+                  Convert an image from one format into another. The image type is
+                  determined by the file suffixes.
+
                   Copyright (C) 2013 Oskar Maier
                   This program comes with ABSOLUTELY NO WARRANTY; This is free software,
                   and you are welcome to redistribute it under certain conditions; see
-                  the LICENSE file or <http://www.gnu.org/licenses/> for details.   
+                  the LICENSE file or <http://www.gnu.org/licenses/> for details.
                   """
 
+
 # code
 def main():
     args = getArguments(getParser())
 
     # prepare logger
     logger = Logger.getInstance()
-    if args.debug: logger.setLevel(logging.DEBUG)
-    elif args.verbose: logger.setLevel(logging.INFO)
-    
-    img, hdr = load(args.input)
-    
-    if args.spacing:
-        print('{}'.format(hdr.get_voxel_spacing()))
-        return 0
-    
-    logger.debug('Resulting shape is {}.'.format(img.shape))
+    if args.debug:
+        logger.setLevel(logging.DEBUG)
+    elif args.verbose:
+        logger.setLevel(logging.INFO)
+
+    # load input image
+    data_input, header_input = load(args.input)
+
+    # eventually empty data
+    if args.empty:
+        data_input.fill(False)
 
     # save resulting volume
-    save(img, args.output, hdr, args.force)
-    
-    logger.info("Successfully terminated.")    
-    
+    save(data_input, args.output, header_input, args.force)
+
+    logger.info("Successfully terminated.")
+
+
 def getArguments(parser):
     "Provides additional validation of the arguments collected by argparse."
     return parser.parse_args()
 
+
 def getParser():
     "Creates and returns the argparse parser object."
     parser = argparse.ArgumentParser(description=__description__)
-    parser.add_argument('input', help='Source folder.')
-    parser.add_argument('output', help='Target volume.')
-    parser.add_argument('-s', dest='spacing', action='store_true', help='Just print spacing and exit.')
-    parser.add_argument('-v', dest='verbose', action='store_true', help='Display more information.')
-    parser.add_argument('-d', dest='debug', action='store_true', help='Display debug information.')
-    parser.add_argument('-f', dest='force', action='store_true', help='Silently override existing output images.')
-    return parser    
+    parser.add_argument("input", help="Source volume.")
+    parser.add_argument("output", help="Target volume.")
+    parser.add_argument(
+        "-e",
+        dest="empty",
+        action="store_true",
+        help="Instead of copying the voxel data, create an empty copy conserving all meta-data if possible.",
+    )
+    parser.add_argument(
+        "-v", dest="verbose", action="store_true", help="Display more information."
+    )
+    parser.add_argument(
+        "-d", dest="debug", action="store_true", help="Display debug information."
+    )
+    parser.add_argument(
+        "-f",
+        dest="force",
+        action="store_true",
+        help="Silently override existing output images.",
+    )
+    return parser
+
 
 if __name__ == "__main__":
-    main()        
+    main()
```

### Comparing `MedPy-0.4.0/bin/medpy_graphcut_label_w_regional.py` & `MedPy-0.5.0/bin/medpy_graphcut_label_w_regional.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,180 +15,235 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
-# build-in modules
-from argparse import RawTextHelpFormatter
 import argparse
 import logging
 import os
 
+# build-in modules
+from argparse import RawTextHelpFormatter
+
 # third-party modules
-import scipy
+import numpy
 
-# path changes
+from medpy import filter, graphcut
 
 # own modules
 from medpy.core import ArgumentError, Logger
-from medpy.io import load, save
-from medpy import graphcut
-from medpy import filter
 from medpy.graphcut.wrapper import split_marker
+from medpy.io import load, save
 
+# path changes
 
 
 # information
 __author__ = "Oskar Maier"
 __version__ = "d0.2.1, 2012-07-31"
 __email__ = "oskar.maier@googlemail.com"
 __status__ = "Development"
 __description__ = """
                   Perform a binary graph cut using Boykov's max-flow/min-cut algorithm.
-                  
+
                   This implementation does not only compute a boundary term but also a
                   regional term which. The only available implementation up till now is
                   the use of an atalas (i.e. a probability image of float values). The
                   pixel values have to lie between 0 and 1, whereas 1 denounces a sure
                   probability that the object is situated at this position.  The desired
                   boundary term can be selected via the --boundary argument. Depending on
                   the selected term, an additional image has to be supplied as badditional.
-                  
+
                   In the case of the stawiaski boundary term, this is the gradient image.
                   In the case of the difference of means, it is the original image.
-                  
+
                   Furthermore the algorithm requires the region map of the original
                   image and an integer image with foreground and background markers.
-                  
+
                   Additionally a filename for the created binary mask marking foreground
                   and background has to be supplied.
-                  
+
                   Note that the input images must be of the same dimensionality,
                   otherwise an exception is thrown.
                   Note to take into account the input images orientation.
                   Note that the quality of the resulting segmentations depends also on
                   the quality of the supplied markers.
-                  
+
                   Copyright (C) 2013 Oskar Maier
                   This program comes with ABSOLUTELY NO WARRANTY; This is free software,
                   and you are welcome to redistribute it under certain conditions; see
-                  the LICENSE file or <http://www.gnu.org/licenses/> for details.   
+                  the LICENSE file or <http://www.gnu.org/licenses/> for details.
                   """
 
+
 # code
 def main():
     # parse cmd arguments
     parser = getParser()
     parser.parse_args()
     args = getArguments(parser)
-    
+
     # prepare logger
     logger = Logger.getInstance()
-    if args.debug: logger.setLevel(logging.DEBUG)
-    elif args.verbose: logger.setLevel(logging.INFO)
-        
+    if args.debug:
+        logger.setLevel(logging.DEBUG)
+    elif args.verbose:
+        logger.setLevel(logging.INFO)
+
     # check if output image exists
     if not args.force:
         if os.path.exists(args.output):
-            logger.warning('The output image {} already exists. Exiting.'.format(args.output))
+            logger.warning(
+                "The output image {} already exists. Exiting.".format(args.output)
+            )
             exit(-1)
-            
+
     # select boundary term
-    if args.boundary == 'stawiaski':
+    if args.boundary == "stawiaski":
         boundary_term = graphcut.energy_label.boundary_stawiaski
-        logger.info('Selected boundary term: stawiaski')
+        logger.info("Selected boundary term: stawiaski")
     else:
         boundary_term = graphcut.energy_label.boundary_difference_of_means
-        logger.info('Selected boundary term: difference of means')
-        
+        logger.info("Selected boundary term: difference of means")
+
     # select regional term
-    if args.regional == 'atlas':
+    if args.regional == "atlas":
         regional_term = graphcut.energy_label.regional_atlas
     else:
         regional_term = None
 
     # load input images
     region_image_data, reference_header = load(args.region)
     markers_image_data, _ = load(args.markers)
-    
+
     # loading and splitting the marker image
     fgmarkers_image_data, bgmarkers_image_data = split_marker(markers_image_data)
-    
+
     badditional_image_data, _ = load(args.badditional)
-    
-    if 'radditional' in args:
+
+    if "radditional" in args:
         radditional_image_data, _ = load(args.radditional)
     else:
         radditional_image_data = False
-    
-       
+
     # check if all images dimensions are the same
-    if not (badditional_image_data.shape == region_image_data.shape == fgmarkers_image_data.shape == bgmarkers_image_data.shape):
-        logger.critical('Not all of the supplied images are of the same shape.')
-        raise ArgumentError('Not all of the supplied images are of the same shape.')
+    if not (
+        badditional_image_data.shape
+        == region_image_data.shape
+        == fgmarkers_image_data.shape
+        == bgmarkers_image_data.shape
+    ):
+        logger.critical("Not all of the supplied images are of the same shape.")
+        raise ArgumentError("Not all of the supplied images are of the same shape.")
     if not bool == type(radditional_image_data):
         if not (badditional_image_data.shape == radditional_image_data.shape):
-            logger.critical('Not all of the supplied images are of the same shape.')
-            raise ArgumentError('Not all of the supplied images are of the same shape.')
-       
+            logger.critical("Not all of the supplied images are of the same shape.")
+            raise ArgumentError("Not all of the supplied images are of the same shape.")
+
     # recompute the label ids to start from id = 1
-    logger.info('Relabel input image...')
+    logger.info("Relabel input image...")
     region_image_data = filter.relabel(region_image_data)
 
     # generate graph
-    logger.info('Preparing graph...')
-    gcgraph = graphcut.graph_from_labels(region_image_data,
-                                    fgmarkers_image_data,
-                                    bgmarkers_image_data,
-                                    regional_term = regional_term,
-                                    boundary_term = boundary_term,
-                                    regional_term_args = (radditional_image_data, args.alpha),
-                                    boundary_term_args = (badditional_image_data)) # second (optional) parameter is directedness of graph , 0)
+    logger.info("Preparing graph...")
+    gcgraph = graphcut.graph_from_labels(
+        region_image_data,
+        fgmarkers_image_data,
+        bgmarkers_image_data,
+        regional_term=regional_term,
+        boundary_term=boundary_term,
+        regional_term_args=(radditional_image_data, args.alpha),
+        boundary_term_args=(badditional_image_data),
+    )  # second (optional) parameter is directedness of graph , 0)
 
-    logger.info('Removing images that are not longer required from memory...')
+    logger.info("Removing images that are not longer required from memory...")
     del fgmarkers_image_data
     del bgmarkers_image_data
     del radditional_image_data
     del badditional_image_data
-    
+
     # execute min-cut
-    logger.info('Executing min-cut...')
+    logger.info("Executing min-cut...")
     maxflow = gcgraph.maxflow()
-    logger.debug('Maxflow is {}'.format(maxflow))
-    
+    logger.debug("Maxflow is {}".format(maxflow))
+
     # apply results to the region image
-    logger.info('Applying results...')
-    mapping = [0] # no regions with id 1 exists in mapping, entry used as padding
-    mapping.extend([0 if gcgraph.termtype.SINK == gcgraph.what_segment(int(x) - 1) else 1 for x in scipy.unique(region_image_data)])
+    logger.info("Applying results...")
+    mapping = [0]  # no regions with id 1 exists in mapping, entry used as padding
+    mapping.extend(
+        [
+            0 if gcgraph.termtype.SINK == gcgraph.what_segment(int(x) - 1) else 1
+            for x in numpy.unique(region_image_data)
+        ]
+    )
     region_image_data = filter.relabel_map(region_image_data, mapping)
-    
+
     # save resulting mask
-    save(region_image_data.astype(scipy.bool_), args.output, reference_header, args.force)
+    save(
+        region_image_data.astype(numpy.bool_), args.output, reference_header, args.force
+    )
+
+    logger.info("Successfully terminated.")
 
-    logger.info('Successfully terminated.')
 
 def getArguments(parser):
     "Provides additional validation of the arguments collected by argparse."
     return parser.parse_args()
 
+
 def getParser():
     "Creates and returns the argparse parser object."
-    parser = argparse.ArgumentParser(description=__description__, formatter_class=RawTextHelpFormatter)
-    
-    parser.add_argument('badditional', help='The additional image required by the boundary term. See there for details.')
-    parser.add_argument('region', help='The region image of the image to segment.')
-    parser.add_argument('markers', help='Binary image containing the foreground (=1) and background (=2) markers.')
-    parser.add_argument('output', help='The output image containing the segmentation.')
-    parser.add_argument('--boundary', default='stawiaski', help='The boundary term to use. Note that difference of means (means) requires the original image, while stawiaski requires the gradient image of the original image to be passed to badditional.', choices=['means', 'stawiaski'])
-    parser.add_argument('--regional', default='none', help='The regional term to use. Note that the atlas requires to provide an atlas image.', choices=['none', 'atlas'])
-    parser.add_argument('--radditional', help='The additional image required by the regional term. See there for details.')
-    parser.add_argument('--alpha', type=float, help='The weight of the regional term compared to the boundary term.')
-    parser.add_argument('-f', dest='force', action='store_true', help='Set this flag to silently override files that exist.')
-    parser.add_argument('-v', dest='verbose', action='store_true', help='Display more information.')
-    parser.add_argument('-d', dest='debug', action='store_true', help='Display debug information.')
-    
-    return parser    
+    parser = argparse.ArgumentParser(
+        description=__description__, formatter_class=RawTextHelpFormatter
+    )
+
+    parser.add_argument(
+        "badditional",
+        help="The additional image required by the boundary term. See there for details.",
+    )
+    parser.add_argument("region", help="The region image of the image to segment.")
+    parser.add_argument(
+        "markers",
+        help="Binary image containing the foreground (=1) and background (=2) markers.",
+    )
+    parser.add_argument("output", help="The output image containing the segmentation.")
+    parser.add_argument(
+        "--boundary",
+        default="stawiaski",
+        help="The boundary term to use. Note that difference of means (means) requires the original image, while stawiaski requires the gradient image of the original image to be passed to badditional.",
+        choices=["means", "stawiaski"],
+    )
+    parser.add_argument(
+        "--regional",
+        default="none",
+        help="The regional term to use. Note that the atlas requires to provide an atlas image.",
+        choices=["none", "atlas"],
+    )
+    parser.add_argument(
+        "--radditional",
+        help="The additional image required by the regional term. See there for details.",
+    )
+    parser.add_argument(
+        "--alpha",
+        type=float,
+        help="The weight of the regional term compared to the boundary term.",
+    )
+    parser.add_argument(
+        "-f",
+        dest="force",
+        action="store_true",
+        help="Set this flag to silently override files that exist.",
+    )
+    parser.add_argument(
+        "-v", dest="verbose", action="store_true", help="Display more information."
+    )
+    parser.add_argument(
+        "-d", dest="debug", action="store_true", help="Display debug information."
+    )
+
+    return parser
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `MedPy-0.4.0/bin/medpy_anisotropic_diffusion.py` & `MedPy-0.5.0/bin/medpy_anisotropic_diffusion.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,83 +20,131 @@
 """
 
 # build-in modules
 import argparse
 import logging
 import os
 
+from medpy.core import Logger
+from medpy.filter.smoothing import anisotropic_diffusion
+
+# own modules
+from medpy.io import get_pixel_spacing, load, save
+
 # third-party modules
 
 # path changes
 
-# own modules
-from medpy.io import load, save, get_pixel_spacing
-from medpy.core import Logger
-from medpy.filter.smoothing import anisotropic_diffusion
-
 
 # information
 __author__ = "Oskar Maier"
 __version__ = "r0.1.0, 2013-08-24"
 __email__ = "oskar.maier@googlemail.com"
 __status__ = "Release"
 __description__ = """
                   Executes gradient anisotropic diffusion filter over an image.
                   This smoothing algorithm is edges preserving.
-                  
+                  To achieve the best effects, the image should be scaled to
+                  values between 0 and 1 beforehand.
+
                   Note that the images voxel-spacing will be taken into account.
-                                  
+
                   Copyright (C) 2013 Oskar Maier
                   This program comes with ABSOLUTELY NO WARRANTY; This is free software,
                   and you are welcome to redistribute it under certain conditions; see
-                  the LICENSE file or <http://www.gnu.org/licenses/> for details.   
+                  the LICENSE file or <http://www.gnu.org/licenses/> for details.
                   """
 
+
 # code
 def main():
     # parse cmd arguments
     parser = getParser()
     parser.parse_args()
     args = getArguments(parser)
-    
+
     # prepare logger
     logger = Logger.getInstance()
-    if args.debug: logger.setLevel(logging.DEBUG)
-    elif args.verbose: logger.setLevel(logging.INFO)
-    
+    if args.debug:
+        logger.setLevel(logging.DEBUG)
+    elif args.verbose:
+        logger.setLevel(logging.INFO)
+
     # check if output image exists (will also be performed before saving, but as the smoothing might be very time intensity, a initial check can save frustration)
     if not args.force:
         if os.path.exists(args.output):
-            raise parser.error('The output image {} already exists.'.format(args.output))
-    
+            raise parser.error(
+                "The output image {} already exists.".format(args.output)
+            )
+
     # loading image
     data_input, header_input = load(args.input)
-    
+
     # apply the watershed
-    logger.info('Applying anisotropic diffusion with settings: niter={} / kappa={} / gamma={}...'.format(args.iterations, args.kappa, args.gamma))
-    data_output = anisotropic_diffusion(data_input, args.iterations, args.kappa, args.gamma, get_pixel_spacing(header_input))
+    logger.info(
+        "Applying anisotropic diffusion with settings: niter={} / kappa={} / gamma={}...".format(
+            args.iterations, args.kappa, args.gamma
+        )
+    )
+    data_output = anisotropic_diffusion(
+        data_input,
+        args.iterations,
+        args.kappa,
+        args.gamma,
+        get_pixel_spacing(header_input),
+    )
 
     # save file
     save(data_output, args.output, header_input, args.force)
-    
-    logger.info('Successfully terminated.')
+
+    logger.info("Successfully terminated.")
+
 
 def getArguments(parser):
     "Provides additional validation of the arguments collected by argparse."
     return parser.parse_args()
 
+
 def getParser():
     "Creates and returns the argparse parser object."
     parser = argparse.ArgumentParser(description=__description__)
-    parser.add_argument('input', help='Source volume.')
-    parser.add_argument('output', help='Target volume.')
-    parser.add_argument('-i', '--iterations', type=int, default=1, help='The number of smoothing iterations. Strong parameter.')
-    parser.add_argument('-k', '--kappa', type=int, default=50, help='The algorithms kappa parameter. The higher the more edges are smoothed over.')
-    parser.add_argument('-g', '--gamma', type=float, default=0.1, help='The algorithms gamma parameter. The higher, the stronger the plateaus between edges are smeared.')
-    parser.add_argument('-v', dest='verbose', action='store_true', help='Display more information.')
-    parser.add_argument('-d', dest='debug', action='store_true', help='Display debug information.')
-    parser.add_argument('-f', dest='force', action='store_true', help='Silently override existing output images.')
-    
+    parser.add_argument("input", help="Source volume.")
+    parser.add_argument("output", help="Target volume.")
+    parser.add_argument(
+        "-i",
+        "--iterations",
+        type=int,
+        default=1,
+        help="The number of smoothing iterations. Strong parameter.",
+    )
+    parser.add_argument(
+        "-k",
+        "--kappa",
+        type=int,
+        default=50,
+        help="The algorithms kappa parameter. The higher the more edges are smoothed over.",
+    )
+    parser.add_argument(
+        "-g",
+        "--gamma",
+        type=float,
+        default=0.1,
+        help="The algorithms gamma parameter. The higher, the stronger the plateaus between edges are smeared.",
+    )
+    parser.add_argument(
+        "-v", dest="verbose", action="store_true", help="Display more information."
+    )
+    parser.add_argument(
+        "-d", dest="debug", action="store_true", help="Display debug information."
+    )
+    parser.add_argument(
+        "-f",
+        dest="force",
+        action="store_true",
+        help="Silently override existing output images.",
+    )
+
     return parser
-    
+
+
 if __name__ == "__main__":
     main()
```

### Comparing `MedPy-0.4.0/bin/medpy_join_masks.py` & `MedPy-0.5.0/bin/medpy_join_masks.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,102 +14,134 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>."""
 
-# build-in modules
-import sys
 import argparse
 import logging
 
 # third-party modules
 import numpy
 
-# path changes
-
 # own modules
 from medpy.core import Logger
-from medpy.io import load, save, header
+from medpy.io import header, load, save
+
+# build-in modules
+
+
+# path changes
 
 
 # information
 __author__ = "Oskar Maier"
 __version__ = "r0.1.0, 2014-05-15"
 __email__ = "oskar.maier@googlemail.com"
 __status__ = "Release"
 __description__ = """
                   Joins a number of binary images into a single conjunction.
-                  
+
                   The available combinatorial operations are sum, avg, max and min.
                   In the case of max and min, the output volumes are also binary images,
                   in the case of sum they are uint8 and in the case of avg of type float.
-                  
+
                   All input images must be of same shape and voxel spacing.
-                  
+
                   WARNING: Does not consider image offset.
-                  
+
                   Copyright (C) 2013 Oskar Maier
                   This program comes with ABSOLUTELY NO WARRANTY; This is free software,
                   and you are welcome to redistribute it under certain conditions; see
-                  the LICENSE file or <http://www.gnu.org/licenses/> for details.   
+                  the LICENSE file or <http://www.gnu.org/licenses/> for details.
                   """
 
+
 # code
 def main():
     args = getArguments(getParser())
 
     # prepare logger
     logger = Logger.getInstance()
-    if args.debug: logger.setLevel(logging.DEBUG)
-    elif args.verbose: logger.setLevel(logging.INFO)
-    
-    
+    if args.debug:
+        logger.setLevel(logging.DEBUG)
+    elif args.verbose:
+        logger.setLevel(logging.INFO)
+
     # load input images and cast to bool
     images = []
     for input_ in args.inputs:
         t = load(input_)
         images.append((t[0], t[1]))
-    
+
     # check if their shapes and voxel spacings are all equal
     s0 = images[0][0].shape
     if not numpy.all([i[0].shape == s0 for i in images[1:]]):
-        raise argparse.ArgumentError(args.input, 'At least one input image is of a different shape than the others.')
+        raise argparse.ArgumentError(
+            args.input,
+            "At least one input image is of a different shape than the others.",
+        )
     vs0 = header.get_pixel_spacing(images[0][1])
     if not numpy.all([header.get_pixel_spacing(i[1]) == vs0 for i in images[1:]]):
-        raise argparse.ArgumentError(args.input, 'At least one input image has a different voxel spacing than the others.')
-    
+        raise argparse.ArgumentError(
+            args.input,
+            "At least one input image has a different voxel spacing than the others.",
+        )
+
     # execute operation
-    logger.debug('Executing operation {} over {} images.'.format(args.operation, len(images)))
-    if 'max' == args.operation:
+    logger.debug(
+        "Executing operation {} over {} images.".format(args.operation, len(images))
+    )
+    if "max" == args.operation:
         out = numpy.maximum.reduce([t[0] for t in images])
-    elif 'min' == args.operation:
+    elif "min" == args.operation:
         out = numpy.minimum.reduce([t[0] for t in images])
-    elif 'sum' == args.operation:
+    elif "sum" == args.operation:
         out = numpy.sum([t[0] for t in images], 0).astype(numpy.uint8)
-    else: # avg
+    else:  # avg
         out = numpy.average([t[0] for t in images], 0).astype(numpy.float32)
-        
+
     # save output
     save(out, args.output, images[0][1], args.force)
-    
-    logger.info("Successfully terminated.")    
-    
+
+    logger.info("Successfully terminated.")
+
+
 def getArguments(parser):
     "Provides additional validation of the arguments collected by argparse."
     return parser.parse_args()
 
+
 def getParser():
     "Creates and returns the argparse parser object."
-    parser = argparse.ArgumentParser(formatter_class=argparse.RawDescriptionHelpFormatter,
-                                     description=__description__)
-    parser.add_argument('output', help='Target volume.')
-    parser.add_argument('inputs', nargs='+', help='Source volume(s).')
-    parser.add_argument('-o', '--operation', dest='operation', choices=['sum', 'avg', 'max', 'min'], default='avg', help='Combinatorial operation to conduct.')
-    parser.add_argument('-v', dest='verbose', action='store_true', help='Display more information.')
-    parser.add_argument('-d', dest='debug', action='store_true', help='Display debug information.')
-    parser.add_argument('-f', dest='force', action='store_true', help='Silently override existing output images.')
-    return parser    
+    parser = argparse.ArgumentParser(
+        formatter_class=argparse.RawDescriptionHelpFormatter,
+        description=__description__,
+    )
+    parser.add_argument("output", help="Target volume.")
+    parser.add_argument("inputs", nargs="+", help="Source volume(s).")
+    parser.add_argument(
+        "-o",
+        "--operation",
+        dest="operation",
+        choices=["sum", "avg", "max", "min"],
+        default="avg",
+        help="Combinatorial operation to conduct.",
+    )
+    parser.add_argument(
+        "-v", dest="verbose", action="store_true", help="Display more information."
+    )
+    parser.add_argument(
+        "-d", dest="debug", action="store_true", help="Display debug information."
+    )
+    parser.add_argument(
+        "-f",
+        dest="force",
+        action="store_true",
+        help="Silently override existing output images.",
+    )
+    return parser
+
 
 if __name__ == "__main__":
-    main()        
+    main()
```

### Comparing `MedPy-0.4.0/bin/medpy_fit_into_shape.py` & `MedPy-0.5.0/bin/medpy_fit_into_shape.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,30 +15,27 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
+import argparse
+import logging
+
 # build-in modules
 import os
-import logging
-import argparse
 
 # third-party modules
 import numpy
-from scipy.ndimage.interpolation import zoom
-from scipy.ndimage.morphology import distance_transform_edt, binary_erosion
-from scipy.ndimage.measurements import label
 
 # own modules
 from medpy.core import Logger
-from medpy.filter import resample, bounding_box
+from medpy.io import load, save
 from medpy.utilities import argparseu
-from medpy.io import load, save, header
 
 # information
 __author__ = "Oskar Maier"
 __version__ = "r0.1.0, 2014-11-25"
 __email__ = "oskar.maier@googlemail.com"
 __status__ = "Release"
 __description__ = """
@@ -46,74 +43,101 @@
 
 If larger, the original image is placed centered in all dimensions. If smaller,
 it is cut equally at all sides.
 
 Copyright (C) 2013 Oskar Maier
 This program comes with ABSOLUTELY NO WARRANTY; This is free software,
 and you are welcome to redistribute it under certain conditions; see
-the LICENSE file or <http://www.gnu.org/licenses/> for details.   
+the LICENSE file or <http://www.gnu.org/licenses/> for details.
 """
 
+
 # code
 def main():
     parser = getParser()
     args = getArguments(parser)
 
     # prepare logger
     logger = Logger.getInstance()
-    if args.debug: logger.setLevel(logging.DEBUG)
-    elif args.verbose: logger.setLevel(logging.INFO)
-    
+    if args.debug:
+        logger.setLevel(logging.DEBUG)
+    elif args.verbose:
+        logger.setLevel(logging.INFO)
+
     # loading input images
     img, hdr = load(args.input)
-    
+
     # check shape dimensionality
     if not len(args.shape) == img.ndim:
-        parser.error('The image has {} dimensions, but {} shape parameters have been supplied.'.format(img.ndim, len(args.shape)))
-        
+        parser.error(
+            "The image has {} dimensions, but {} shape parameters have been supplied.".format(
+                img.ndim, len(args.shape)
+            )
+        )
+
     # check if output image exists
     if not args.force and os.path.exists(args.output):
-        parser.error('The output image {} already exists.'.format(args.output))         
-    
+        parser.error("The output image {} already exists.".format(args.output))
+
     # compute required cropping and extention
     slicers_cut = []
     slicers_extend = []
     for dim in range(len(img.shape)):
         slicers_cut.append(slice(None))
         slicers_extend.append(slice(None))
         if args.shape[dim] != img.shape[dim]:
             difference = abs(img.shape[dim] - args.shape[dim])
             cutoff_left = difference / 2
             cutoff_right = difference / 2 + difference % 2
             if args.shape[dim] > img.shape[dim]:
                 slicers_extend[-1] = slice(cutoff_left, -1 * cutoff_right)
             else:
                 slicers_cut[-1] = slice(cutoff_left, -1 * cutoff_right)
-            
+
     # crop original image
-    img = img[slicers_cut]
-    
+    img = img[tuple(slicers_cut)]
+
     # create output image and place input image centered
     out = numpy.zeros(args.shape, img.dtype)
-    out[slicers_extend] = img
-    
+    out[tuple(slicers_extend)] = img
+
     # saving the resulting image
     save(out, args.output, hdr, args.force)
-    
+
+
 def getArguments(parser):
     "Provides additional validation of the arguments collected by argparse."
     return parser.parse_args()
 
+
 def getParser():
     "Creates and returns the argparse parser object."
-    parser = argparse.ArgumentParser(formatter_class=argparse.RawDescriptionHelpFormatter, description=__description__)
-    parser.add_argument('input', help='the input image')
-    parser.add_argument('output', help='the output image')
-    parser.add_argument('shape', type=argparseu.sequenceOfIntegersGt, help='the desired shape in colon-separated values, e.g. 255,255,32')
-
-    parser.add_argument('-v', '--verbose', dest='verbose', action='store_true', help='verbose output')
-    parser.add_argument('-d', dest='debug', action='store_true', help='Display debug information.')
-    parser.add_argument('-f', '--force', dest='force', action='store_true', help='overwrite existing files')
+    parser = argparse.ArgumentParser(
+        formatter_class=argparse.RawDescriptionHelpFormatter,
+        description=__description__,
+    )
+    parser.add_argument("input", help="the input image")
+    parser.add_argument("output", help="the output image")
+    parser.add_argument(
+        "shape",
+        type=argparseu.sequenceOfIntegersGt,
+        help="the desired shape in colon-separated values, e.g. 255,255,32",
+    )
+
+    parser.add_argument(
+        "-v", "--verbose", dest="verbose", action="store_true", help="verbose output"
+    )
+    parser.add_argument(
+        "-d", dest="debug", action="store_true", help="Display debug information."
+    )
+    parser.add_argument(
+        "-f",
+        "--force",
+        dest="force",
+        action="store_true",
+        help="overwrite existing files",
+    )
     return parser
-    
+
+
 if __name__ == "__main__":
-    main()    
+    main()
```

### Comparing `MedPy-0.4.0/bin/medpy_extract_min_max.py` & `MedPy-0.5.0/bin/medpy_extract_min_max.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,95 +18,110 @@
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 # build-in modules
 import argparse
 import logging
-import sys
 import os
-
-# third-party modules
-
-# path changes
+import sys
 
 # own modules
 from medpy.core import Logger
 from medpy.io import load
 
+# third-party modules
+
+# path changes
+
 
 # information
 __author__ = "Oskar Maier"
 __version__ = "r0.2, 2011-12-13"
 __email__ = "oskar.maier@googlemail.com"
 __status__ = "Release"
 __description__ = """
                   Extracts and displays the min/max values of a number of images
                   and prints the results to the stdout in csv format.
-                  
+
                   Copyright (C) 2013 Oskar Maier
                   This program comes with ABSOLUTELY NO WARRANTY; This is free software,
                   and you are welcome to redistribute it under certain conditions; see
-                  the LICENSE file or <http://www.gnu.org/licenses/> for details.   
+                  the LICENSE file or <http://www.gnu.org/licenses/> for details.
                   """
 
+
 # code
 def main():
     # parse cmd arguments
     parser = getParser()
     parser.parse_args()
     args = getArguments(parser)
-    
+
     # prepare logger
     logger = Logger.getInstance()
-    if args.debug: logger.setLevel(logging.DEBUG)
-    elif args.verbose: logger.setLevel(logging.INFO)
-    
+    if args.debug:
+        logger.setLevel(logging.DEBUG)
+    elif args.verbose:
+        logger.setLevel(logging.INFO)
+
     # build output file name
-    file_csv_name = args.csv + '.csv'
-    
+    file_csv_name = args.csv + ".csv"
+
     # check if output file exists
     if not args.force:
         if os.path.exists(file_csv_name):
-            logger.warning('The output file {} already exists. Skipping.'.format(file_csv_name))
+            logger.warning(
+                "The output file {} already exists. Skipping.".format(file_csv_name)
+            )
             sys.exit(0)
-        
+
     # write header line
-    print('image;min;max\n')
-    
+    print("image;min;max\n")
+
     # iterate over input images
     for image in args.images:
-        
         # get and prepare image data
-        logger.info('Processing image {}...'.format(image))
+        logger.info("Processing image {}...".format(image))
         image_data, _ = load(image)
-        
+
         # count number of labels and flag a warning if they reach the ushort border
         min_value = image_data.min()
-        max_value = image_data.max() 
-        
+        max_value = image_data.max()
+
         # count number of labels and write
-        print('{};{};{}\n'.format(image.split('/')[-1], min_value, max_value))
-        
+        print("{};{};{}\n".format(image.split("/")[-1], min_value, max_value))
+
         sys.stdout.flush()
-            
-    logger.info('Successfully terminated.')
-      
+
+    logger.info("Successfully terminated.")
+
+
 def getArguments(parser):
     "Provides additional validation of the arguments collected by argparse."
     return parser.parse_args()
 
+
 def getParser():
     "Creates and returns the argparse parser object."
     parser = argparse.ArgumentParser(description=__description__)
 
-    parser.add_argument('csv', help='The file to store the results in (\wo suffix).')
-    parser.add_argument('images', nargs='+', help='One or more images.')
-    parser.add_argument('-v', dest='verbose', action='store_true', help='Display more information.')
-    parser.add_argument('-d', dest='debug', action='store_true', help='Display debug information.')
-    parser.add_argument('-f', dest='force', action='store_true', help='Silently override existing output images.')
-    
-    return parser    
-    
+    parser.add_argument("csv", help="The file to store the results in (\wo suffix).")
+    parser.add_argument("images", nargs="+", help="One or more images.")
+    parser.add_argument(
+        "-v", dest="verbose", action="store_true", help="Display more information."
+    )
+    parser.add_argument(
+        "-d", dest="debug", action="store_true", help="Display debug information."
+    )
+    parser.add_argument(
+        "-f",
+        dest="force",
+        action="store_true",
+        help="Silently override existing output images.",
+    )
+
+    return parser
+
+
 if __name__ == "__main__":
-    main()            
-    
+    main()
```

### Comparing `MedPy-0.4.0/bin/medpy_info.py` & `MedPy-0.5.0/bin/medpy_info.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,83 +19,99 @@
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 # build-in modules
 import argparse
 import logging
 
+from medpy.core import Logger
+
+# own modules
+from medpy.io import get_offset, get_pixel_spacing, load
+
 # third-party modules
 
 # path changes
 
-# own modules
-from medpy.io import load, get_pixel_spacing, get_offset
-from medpy.core import Logger
-
 
 # information
 __author__ = "Oskar Maier"
 __version__ = "r0.2.1, 2012-05-24"
 __email__ = "oskar.maier@googlemail.com"
 __status__ = "Release"
 __description__ = """
                   Prints information about an image volume to the command line.
-                  
+
                   Copyright (C) 2013 Oskar Maier
                   This program comes with ABSOLUTELY NO WARRANTY; This is free software,
                   and you are welcome to redistribute it under certain conditions; see
-                  the LICENSE file or <http://www.gnu.org/licenses/> for details.   
+                  the LICENSE file or <http://www.gnu.org/licenses/> for details.
                   """
 
+
 # code
 def main():
     # parse cmd arguments
     parser = getParser()
     parser.parse_args()
     args = getArguments(parser)
-    
+
     # prepare logger
     logger = Logger.getInstance()
-    if args.debug: logger.setLevel(logging.DEBUG)
-    elif args.verbose: logger.setLevel(logging.INFO)
-    
+    if args.debug:
+        logger.setLevel(logging.DEBUG)
+    elif args.verbose:
+        logger.setLevel(logging.INFO)
+
     # load input image
     input_data, input_header = load(args.input)
-    
+
     # print information about the image
     printInfo(input_data, input_header)
-    
-    logger.info('Successfully terminated.')
-        
+
+    logger.info("Successfully terminated.")
+
+
 def printInfo(data, header):
     # print image information
-    print('\nInformations obtained from image header:')
-    print('header type={}'.format(type(header)))
+    print("\nInformations obtained from image header:")
+    print("header type={}".format(type(header)))
     try:
-        print('voxel spacing={}'.format(get_pixel_spacing(header)))
+        print("voxel spacing={}".format(get_pixel_spacing(header)))
     except AttributeError:
-        print('Failed to retrieve voxel spacing.')
+        print("Failed to retrieve voxel spacing.")
     try:
-        print('offset={}'.format(get_offset(header)))
+        print("offset={}".format(get_offset(header)))
     except AttributeError:
-        print('Failed to retrieve offset.')    
-    
-    print('\nInformations obtained from image array:')
-    print('datatype={},dimensions={},shape={}'.format(data.dtype, data.ndim, data.shape))
-    print('first and last element: {} / {}'.format(data.flatten()[0], data.flatten()[-1]))
-        
+        print("Failed to retrieve offset.")
+
+    print("\nInformations obtained from image array:")
+    print(
+        "datatype={},dimensions={},shape={}".format(data.dtype, data.ndim, data.shape)
+    )
+    print(
+        "first and last element: {} / {}".format(data.flatten()[0], data.flatten()[-1])
+    )
+
+
 def getArguments(parser):
     "Provides additional validation of the arguments collected by argparse."
     return parser.parse_args()
 
+
 def getParser():
     "Creates and returns the argparse parser object."
     parser = argparse.ArgumentParser(description=__description__)
 
-    parser.add_argument('input', help='The image to analyse.')
-    parser.add_argument('-v', dest='verbose', action='store_true', help='Display more information.')
-    parser.add_argument('-d', dest='debug', action='store_true', help='Display debug information.')
-    
-    return parser    
-    
+    parser.add_argument("input", help="The image to analyse.")
+    parser.add_argument(
+        "-v", dest="verbose", action="store_true", help="Display more information."
+    )
+    parser.add_argument(
+        "-d", dest="debug", action="store_true", help="Display debug information."
+    )
+
+    return parser
+
+
 if __name__ == "__main__":
-    main()        
+    main()
```

### Comparing `MedPy-0.4.0/bin/medpy_morphology.py` & `MedPy-0.5.0/bin/medpy_morphology.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,91 +20,136 @@
 """
 
 # build-in modules
 import argparse
 import logging
 
 # third-party modules
-import scipy.ndimage.morphology
-
-# path changes
+import scipy.ndimage
 
 # own modules
 from medpy.core import Logger
 from medpy.io import load, save
 
+# path changes
+
 
 # information
 __author__ = "Oskar Maier"
 __version__ = "r2.0.0, 2011-12-13"
 __email__ = "oskar.maier@googlemail.com"
 __status__ = "Release"
 __description__ = """
                   Executes opening and closing morphological operations over the input image(s).
-                  
+
                   Copyright (C) 2013 Oskar Maier
                   This program comes with ABSOLUTELY NO WARRANTY; This is free software,
                   and you are welcome to redistribute it under certain conditions; see
-                  the LICENSE file or <http://www.gnu.org/licenses/> for details.   
+                  the LICENSE file or <http://www.gnu.org/licenses/> for details.
                   """
 
+
 # code
 def main():
     # parse cmd arguments
     parser = getParser()
     parser.parse_args()
     args = getArguments(parser)
-    
+
     # prepare logger
     logger = Logger.getInstance()
-    if args.debug: logger.setLevel(logging.DEBUG)
-    elif args.verbose: logger.setLevel(logging.INFO)
+    if args.debug:
+        logger.setLevel(logging.DEBUG)
+    elif args.verbose:
+        logger.setLevel(logging.INFO)
 
     # load input image
     image_smoothed_data, image_header = load(args.input)
-        
+
     # perform opening resp. closing
     # in 3D case: size 1 = 6-connectedness, 2 = 12-connectedness, 3 = 18-connectedness, etc.
-    footprint = scipy.ndimage.morphology.generate_binary_structure(image_smoothed_data.ndim, args.size)
-    if 'erosion' == args.type:
-        logger.info('Applying erosion...')
-        image_smoothed_data = scipy.ndimage.morphology.binary_erosion(image_smoothed_data, footprint, iterations=args.iterations)
-    elif 'dilation' == args.type:
-        logger.info('Applying dilation...')
-        image_smoothed_data = scipy.ndimage.morphology.binary_dilation(image_smoothed_data, footprint, iterations=args.iterations)
-    elif 'opening' == args.type:
-        logger.info('Applying opening...')
-        image_smoothed_data = scipy.ndimage.morphology.binary_opening(image_smoothed_data, footprint, iterations=args.iterations)
-    else: # closing
-        logger.info('Applying closing...')
-        image_smoothed_data = scipy.ndimage.morphology.binary_closing(image_smoothed_data, footprint, iterations=args.iterations)
+    footprint = scipy.ndimage.generate_binary_structure(
+        image_smoothed_data.ndim, args.size
+    )
+    if "erosion" == args.type:
+        logger.info("Applying erosion...")
+        image_smoothed_data = scipy.ndimage.binary_erosion(
+            image_smoothed_data, footprint, iterations=args.iterations
+        )
+    elif "dilation" == args.type:
+        logger.info("Applying dilation...")
+        image_smoothed_data = scipy.ndimage.binary_dilation(
+            image_smoothed_data, footprint, iterations=args.iterations
+        )
+    elif "opening" == args.type:
+        logger.info("Applying opening...")
+        image_smoothed_data = scipy.ndimage.binary_opening(
+            image_smoothed_data, footprint, iterations=args.iterations
+        )
+    else:  # closing
+        logger.info("Applying closing...")
+        image_smoothed_data = scipy.ndimage.binary_closing(
+            image_smoothed_data, footprint, iterations=args.iterations
+        )
 
     # apply additional hole closing step
-    logger.info('Closing holes...')
-    image_smoothed_data = scipy.ndimage.morphology.binary_fill_holes(image_smoothed_data)
+    logger.info("Closing holes...")
+    image_smoothed_data = scipy.ndimage.binary_fill_holes(image_smoothed_data)
 
     # save resulting mas
     save(image_smoothed_data, args.output, image_header, args.force)
-            
-    logger.info('Successfully terminated.')
-      
+
+    logger.info("Successfully terminated.")
+
+
 def getArguments(parser):
     "Provides additional validation of the arguments collected by argparse."
     return parser.parse_args()
 
+
 def getParser():
     "Creates and returns the argparse parser object."
     parser = argparse.ArgumentParser(description=__description__)
-    parser.add_argument('input', help='Source volume.')
-    parser.add_argument('output', help='Target volume.')
-    parser.add_argument('-t', '--type', dest='type', choices=['erosion', 'dilation', 'opening', 'closing'], default='erosion', help='The type of the morphological operation.')
-    parser.add_argument('-i', '--iterations', dest='iterations', default=0, type=int, help='The number of iteration to execute. Supply a value of 1 or higher to restrict the effect of the morphological operation. Otherwise it is applied until saturation.')
-    parser.add_argument('-s', '--size', dest='size', default=3, type=int, help='Size of the closing element (>=1). The higher this value, the bigger the wholes that get closed (closing) resp. unconnected elements that are removed (opening). In the 3D case, 1 equals a 6-connectedness, 2 a 12-connectedness, 3 a 18-connectedness, etc.')
-    parser.add_argument('-v', dest='verbose', action='store_true', help='Display more information.')
-    parser.add_argument('-d', dest='debug', action='store_true', help='Display debug information.')
-    parser.add_argument('-f', dest='force', action='store_true', help='Silently override existing output images.')
-    
-    return parser    
-    
+    parser.add_argument("input", help="Source volume.")
+    parser.add_argument("output", help="Target volume.")
+    parser.add_argument(
+        "-t",
+        "--type",
+        dest="type",
+        choices=["erosion", "dilation", "opening", "closing"],
+        default="erosion",
+        help="The type of the morphological operation.",
+    )
+    parser.add_argument(
+        "-i",
+        "--iterations",
+        dest="iterations",
+        default=0,
+        type=int,
+        help="The number of iteration to execute. Supply a value of 1 or higher to restrict the effect of the morphological operation. Otherwise it is applied until saturation.",
+    )
+    parser.add_argument(
+        "-s",
+        "--size",
+        dest="size",
+        default=3,
+        type=int,
+        help="Size of the closing element (>=1). The higher this value, the bigger the wholes that get closed (closing) resp. unconnected elements that are removed (opening). In the 3D case, 1 equals a 6-connectedness, 2 a 12-connectedness, 3 a 18-connectedness, etc.",
+    )
+    parser.add_argument(
+        "-v", dest="verbose", action="store_true", help="Display more information."
+    )
+    parser.add_argument(
+        "-d", dest="debug", action="store_true", help="Display debug information."
+    )
+    parser.add_argument(
+        "-f",
+        dest="force",
+        action="store_true",
+        help="Silently override existing output images.",
+    )
+
+    return parser
+
+
 if __name__ == "__main__":
-    main()            
-    
+    main()
```

### Comparing `MedPy-0.4.0/bin/medpy_shrink_image.py` & `MedPy-0.5.0/bin/medpy_shrink_image.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,105 +20,130 @@
 """
 
 # build-in modules
 import argparse
 import logging
 
 # third-party modules
-import scipy
-
-# path changes
+import numpy
 
 # own modules
 from medpy.core import Logger
-from medpy.io import load, save, header
+from medpy.io import header, load, save
+
+# path changes
 
 
 # information
 __author__ = "Oskar Maier"
 __version__ = "d0.2.0, 2012-06-13"
 __email__ = "oskar.maier@googlemail.com"
 __status__ = "Development"
 __description__ = """
                   Shrinks an image by discarding slices. Reverse operation of zoom_image.py.
                   Reduces the image by keeping one slice, then discarding "discard" slices, then
                   keeping the next and so on.
-                                  
+
                   Copyright (C) 2013 Oskar Maier
                   This program comes with ABSOLUTELY NO WARRANTY; This is free software,
                   and you are welcome to redistribute it under certain conditions; see
                   the LICENSE file or <http://www.gnu.org/licenses/> for details.
     """
 
+
 # code
 def main():
     args = getArguments(getParser())
 
     # prepare logger
     logger = Logger.getInstance()
-    if args.debug: logger.setLevel(logging.DEBUG)
-    elif args.verbose: logger.setLevel(logging.INFO)
-    
+    if args.debug:
+        logger.setLevel(logging.DEBUG)
+    elif args.verbose:
+        logger.setLevel(logging.INFO)
+
     # load input data
     input_data, input_header = load(args.input)
-    
-    logger.debug('Old shape = {}.'.format(input_data.shape))
-    
+
+    logger.debug("Old shape = {}.".format(input_data.shape))
+
     # compute new shape
     new_shape = list(input_data.shape)
     new_shape[args.dimension] = 1 + (new_shape[args.dimension] - 1) / (args.discard + 1)
-    
+
     # prepare output image
-    output_data = scipy.zeros(new_shape, dtype=input_data.dtype)
-    
+    output_data = numpy.zeros(new_shape, dtype=input_data.dtype)
+
     # prepare slicers
     slicer_in = [slice(None)] * input_data.ndim
     slicer_out = [slice(None)] * input_data.ndim
-    
+
     # prepare skip-counter and output image slice counter
     skipc = 0
     slicec = 0
-    
-    logger.debug('Shrinking from {} to {}...'.format(input_data.shape, new_shape))
+
+    logger.debug("Shrinking from {} to {}...".format(input_data.shape, new_shape))
     for idx in range(input_data.shape[args.dimension]):
-        
         if 0 == skipc:
             # transfer slice
             slicer_in[args.dimension] = slice(idx, idx + 1)
-            slicer_out[args.dimension]  = slice(slicec, slicec + 1)
-            output_data[slicer_out] = input_data[slicer_in]
-            
+            slicer_out[args.dimension] = slice(slicec, slicec + 1)
+            output_data[tuple(slicer_out)] = input_data[tuple(slicer_in)]
+
             # resert resp. increase counter
             skipc = args.discard
             slicec += 1
-            
-        else: # skip slice
+
+        else:  # skip slice
             # decrease skip counter
             skipc -= 1
 
-    
     # set new pixel spacing
     new_spacing = list(header.get_pixel_spacing(input_header))
     new_spacing[args.dimension] = new_spacing[args.dimension] * float(args.discard + 1)
-    logger.debug('Setting pixel spacing from {} to {}....'.format(header.get_pixel_spacing(input_header), new_spacing))
+    logger.debug(
+        "Setting pixel spacing from {} to {}....".format(
+            header.get_pixel_spacing(input_header), new_spacing
+        )
+    )
     header.set_pixel_spacing(input_header, tuple(new_spacing))
-    
+
     save(output_data, args.output, input_header, args.force)
-    
+
+
 def getArguments(parser):
     "Provides additional validation of the arguments collected by argparse."
     return parser.parse_args()
 
+
 def getParser():
     "Creates and returns the argparse parser object."
-    parser = argparse.ArgumentParser(description=__description__, formatter_class=argparse.RawTextHelpFormatter)
-    parser.add_argument('input', help='Source volume.')
-    parser.add_argument('output', help='Target volume.')
-    parser.add_argument('dimension', type=int, help='The dimension along which to discard the slices.')
-    parser.add_argument('discard', type=int, help='How many slices to discard between each two slices which are kept.')
-    parser.add_argument('-v', dest='verbose', action='store_true', help='Display more information.')
-    parser.add_argument('-d', dest='debug', action='store_true', help='Display debug information.')
-    parser.add_argument('-f', dest='force', action='store_true', help='Silently override existing output images.')
+    parser = argparse.ArgumentParser(
+        description=__description__, formatter_class=argparse.RawTextHelpFormatter
+    )
+    parser.add_argument("input", help="Source volume.")
+    parser.add_argument("output", help="Target volume.")
+    parser.add_argument(
+        "dimension", type=int, help="The dimension along which to discard the slices."
+    )
+    parser.add_argument(
+        "discard",
+        type=int,
+        help="How many slices to discard between each two slices which are kept.",
+    )
+    parser.add_argument(
+        "-v", dest="verbose", action="store_true", help="Display more information."
+    )
+    parser.add_argument(
+        "-d", dest="debug", action="store_true", help="Display debug information."
+    )
+    parser.add_argument(
+        "-f",
+        dest="force",
+        action="store_true",
+        help="Silently override existing output images.",
+    )
     return parser
 
+
 if __name__ == "__main__":
-    main()     
+    main()
```

### Comparing `MedPy-0.4.0/bin/medpy_intensity_range_standardization.py` & `MedPy-0.5.0/bin/medpy_intensity_range_standardization.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,45 +15,46 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
+import argparse
+import logging
+
 # build-in modules
 import os
 import pickle
-import argparse
-import logging
 
 # third-party modules
 import numpy
 
-# path changes
-
 # own modules
 from medpy.core import Logger
 from medpy.core.exceptions import ArgumentError
+from medpy.filter import IntensityRangeStandardization
 from medpy.io import load, save
 from medpy.utilities.argparseu import sequenceOfIntegersGeAscendingStrict
-from medpy.filter import IntensityRangeStandardization
+
+# path changes
 
 
 # information
 __author__ = "Oskar Maier"
 __version__ = "r0.1.1, 2013-10-11"
 __email__ = "oskar.maier@googlemail.com"
 __status__ = "Release"
 __description__ = """
 Standardizes the intensity range / profile of a number of similar images.
 
 Takes a number of images that display the same scene (most commonly MRI volumes of the
 same body region) and learns an average intensity range model from these. This model can
 then be used to transfer the training image set and other, formerly unseen images, to the
-learned average intensity range. Such prepared, these images display the same intensity 
+learned average intensity range. Such prepared, these images display the same intensity
 profiles for the same structures.
 
 The employed algorithm guarantees a lossless intensity transformation and throws an
 exception, should the model require re-training.
 
 The application requires the supplied images to be stripped of their background. This can
 either be done by setting a threshold value or by supplying a foreground-mask for each
@@ -65,130 +66,226 @@
 Depending on the application, different arguments are require that are reflected by the
 argument grouping.
 
 The implementation is based on:
 [1] Nyul, L.G.; Udupa, J.K.; Xuan Zhang, "New variants of a method of MRI scale
     standardization," Medical Imaging, IEEE Transactions on , vol.19, no.2, pp.143-150,
     Feb. 2000
-    
+
 For more details on the algorithm, see the medpy.filter.IntensityRangeStandardization class.
 
 Copyright (C) 2013 Oskar Maier
 This program comes with ABSOLUTELY NO WARRANTY; This is free software,
 and you are welcome to redistribute it under certain conditions; see
-the LICENSE file or <http://www.gnu.org/licenses/> for details.   
+the LICENSE file or <http://www.gnu.org/licenses/> for details.
                   """
 
+
 # code
 def main():
     args = getArguments(getParser())
 
     # prepare logger
     logger = Logger.getInstance()
-    if args.debug: logger.setLevel(logging.DEBUG)
-    elif args.verbose: logger.setLevel(logging.INFO)
-    
+    if args.debug:
+        logger.setLevel(logging.DEBUG)
+    elif args.verbose:
+        logger.setLevel(logging.INFO)
+
     # loading input images (as image, header pairs)
     images = []
     headers = []
     for image_name in args.images:
         i, h = load(image_name)
         images.append(i)
         headers.append(h)
-    
+
     # loading binary foreground masks if supplied, else create masks from threshold value
     if args.masks:
-        masks = [load(mask_name)[0].astype(numpy.bool) for mask_name in args.masks]
+        masks = [load(mask_name)[0].astype(numpy.bool_) for mask_name in args.masks]
     else:
         masks = [i > args.threshold for i in images]
-    
+
     # if in application mode, load the supplied model and apply it to the images
     if args.lmodel:
-        logger.info('Loading the model and transforming images...')
-        with open(args.lmodel, 'r') as f:
+        logger.info("Loading the model and transforming images...")
+        with open(args.lmodel, "r") as f:
             trained_model = pickle.load(f)
             if not isinstance(trained_model, IntensityRangeStandardization):
-                raise ArgumentError('{} does not seem to be a valid pickled instance of an IntensityRangeStandardization object'.format(args.lmodel))
-            transformed_images = [trained_model.transform(i[m], surpress_mapping_check = args.ignore) for i, m in zip(images, masks)]
-            
+                raise ArgumentError(
+                    "{} does not seem to be a valid pickled instance of an IntensityRangeStandardization object".format(
+                        args.lmodel
+                    )
+                )
+            transformed_images = [
+                trained_model.transform(i[m], surpress_mapping_check=args.ignore)
+                for i, m in zip(images, masks)
+            ]
+
     # in in training mode, train the model, apply it to the images and save it
     else:
-        logger.info('Training the average intensity model...')
+        logger.info("Training the average intensity model...")
         irs = IntensityRangeStandardization()
-        trained_model, transformed_images = irs.train_transform([i[m] for i, m in zip(images, masks)], surpress_mapping_check = args.ignore)
-        logger.info('Saving the trained model as {}...'.format(args.smodel))
-        with open(args.smodel, 'wb') as f:
-                pickle.dump(trained_model, f)
-                
+        trained_model, transformed_images = irs.train_transform(
+            [i[m] for i, m in zip(images, masks)], surpress_mapping_check=args.ignore
+        )
+        logger.info("Saving the trained model as {}...".format(args.smodel))
+        with open(args.smodel, "wb") as f:
+            pickle.dump(trained_model, f)
+
     # save the transformed images
     if args.simages:
-        logger.info('Saving intensity transformed images to {}...'.format(args.simages))
-        for ti, i, m, h, image_name in zip(transformed_images, images, masks, headers, args.images):
+        logger.info("Saving intensity transformed images to {}...".format(args.simages))
+        for ti, i, m, h, image_name in zip(
+            transformed_images, images, masks, headers, args.images
+        ):
             i[m] = ti
-            save(i, '{}/{}'.format(args.simages, image_name.split('/')[-1]), h, args.force)
-    
-    logger.info('Terminated.')
-    
+            save(
+                i,
+                "{}/{}".format(args.simages, image_name.split("/")[-1]),
+                h,
+                args.force,
+            )
+
+    logger.info("Terminated.")
+
 
-    
 def getArguments(parser):
     "Provides additional validation of the arguments collected by argparse."
     args = parser.parse_args()
-    
+
     # check mutual exlusive and reaquired arguments
     if args.lmodel and args.smodel:
-        parser.error('only one of --load-model and --save-model can be supplied, as they decide on whether to apply the application or the training mode')
+        parser.error(
+            "only one of --load-model and --save-model can be supplied, as they decide on whether to apply the application or the training mode"
+        )
     if not args.lmodel and not args.smodel:
-        parser.error('exactly one of --load-model or --save-model has to be supplied')
-    
+        parser.error("exactly one of --load-model or --save-model has to be supplied")
+
     # application mode
     if args.lmodel:
         if not os.path.isfile(args.lmodel):
-            parser.error('the supplied model file {} does not exist'.format(args.lmodel))
+            parser.error(
+                "the supplied model file {} does not exist".format(args.lmodel)
+            )
         if not args.simages:
-            parser.error('--save-images must be supplied when running the application mode')
-    
+            parser.error(
+                "--save-images must be supplied when running the application mode"
+            )
+
     # training mode
     if args.smodel:
-        if not args.landmarkp in ('L2', 'L3', 'L4'):
+        if not args.landmarkp in ("L2", "L3", "L4"):
             args.landmarkp = sequenceOfIntegersGeAscendingStrict(args.landmarkp)
-        if not 'auto' == args.stdspace:
+        if not "auto" == args.stdspace:
             args.stdspace = sequenceOfIntegersGeAscendingStrict(args.stdspace)
         if not args.force and os.path.isfile(args.smodel):
-            parser.error('the target model file {} already exists'.format(args.smodel))
-        
+            parser.error("the target model file {} already exists".format(args.smodel))
+
     # others
     if args.simages:
         if not os.path.isdir(args.simages):
-            parser.error('--save-images must be a valid directory')
+            parser.error("--save-images must be a valid directory")
     if args.masks and len(args.masks) != len(args.images):
-        parser.error('the same number of masks must be passed to --masks as images have been supplied') 
-    
+        parser.error(
+            "the same number of masks must be passed to --masks as images have been supplied"
+        )
+
     return args
 
+
 def getParser():
     "Creates and returns the argparse parser object."
-    parser = argparse.ArgumentParser(description=__description__, formatter_class=argparse.RawDescriptionHelpFormatter)
-    parser.add_argument('images', nargs='+', help='The images used for training (in the learning case) or to transform (in the transformation case)')
-
-    apply_group = parser.add_argument_group('apply an existing model')
-    apply_group.add_argument('--load-model', dest='lmodel', default=False, help='Location of the pickled intensity range model to load. Activated application mode.')
-    
-    train_group = parser.add_argument_group('train a new model and save and/or apply it')
-    train_group.add_argument('--save-model', dest='smodel', default=False, help='Save the trained model under this name as a pickled object (should end in .pkl). Activates training mode.')
-    train_group.add_argument('--cutoffp', dest='cutoffp', type=sequenceOfIntegersGeAscendingStrict, default='1,99', help='Colon-separated lower and upper cut-off percentile values to exclude intensity outliers during the model training.')
-    train_group.add_argument('--landmarkp', dest='landmarkp', default='L4', help='The landmark percentiles, based on which to train the model. Can be L2, L3, L4 or a colon-separated, ordered list of percentiles.')
-    train_group.add_argument('--stdspace', dest='stdspace', default='auto', help='Two colon-separated intensity values to roughly define the average intensity space to learn. In most cases should be left set to \'auto\'')
-    
-    shared_group = parser.add_argument_group('shared arguments')
-    shared_group.add_argument('--save-images', dest='simages', default=False, help='Save the transformed images under this location. Required for the application mode, optional for the learning mode.')
-    shared_group.add_argument('--threshold', type=float, default=0, help='All voxel with an intensity > threshold are considered as foreground. Supply either this or a mask for each image.')
-    shared_group.add_argument('--masks', nargs='+', help='A number of binary foreground mask, one for each image. Alternative to supplying a threshold. Overrides the threshold parameter if supplied.')
-    shared_group.add_argument('--ignore', dest='ignore', action='store_true', help='Ignore possible loss of information during the intensity transformation. Should only be used when you know what you are doing.')
-    
-    parser.add_argument('-v', '--verbose', dest='verbose', action='store_true', help='Verbose output')
-    parser.add_argument('-d', '--debug', dest='debug', action='store_true', help='Display debug information.')
-    parser.add_argument('-f', '--force', dest='force', action='store_true', help='Overwrite existing files (both model and images)')
+    parser = argparse.ArgumentParser(
+        description=__description__,
+        formatter_class=argparse.RawDescriptionHelpFormatter,
+    )
+    parser.add_argument(
+        "images",
+        nargs="+",
+        help="The images used for training (in the learning case) or to transform (in the transformation case)",
+    )
+
+    apply_group = parser.add_argument_group("apply an existing model")
+    apply_group.add_argument(
+        "--load-model",
+        dest="lmodel",
+        default=False,
+        help="Location of the pickled intensity range model to load. Activated application mode.",
+    )
+
+    train_group = parser.add_argument_group(
+        "train a new model and save and/or apply it"
+    )
+    train_group.add_argument(
+        "--save-model",
+        dest="smodel",
+        default=False,
+        help="Save the trained model under this name as a pickled object (should end in .pkl). Activates training mode.",
+    )
+    train_group.add_argument(
+        "--cutoffp",
+        dest="cutoffp",
+        type=sequenceOfIntegersGeAscendingStrict,
+        default="1,99",
+        help="Colon-separated lower and upper cut-off percentile values to exclude intensity outliers during the model training.",
+    )
+    train_group.add_argument(
+        "--landmarkp",
+        dest="landmarkp",
+        default="L4",
+        help="The landmark percentiles, based on which to train the model. Can be L2, L3, L4 or a colon-separated, ordered list of percentiles.",
+    )
+    train_group.add_argument(
+        "--stdspace",
+        dest="stdspace",
+        default="auto",
+        help="Two colon-separated intensity values to roughly define the average intensity space to learn. In most cases should be left set to 'auto'",
+    )
+
+    shared_group = parser.add_argument_group("shared arguments")
+    shared_group.add_argument(
+        "--save-images",
+        dest="simages",
+        default=False,
+        help="Save the transformed images under this location. Required for the application mode, optional for the learning mode.",
+    )
+    shared_group.add_argument(
+        "--threshold",
+        type=float,
+        default=0,
+        help="All voxel with an intensity > threshold are considered as foreground. Supply either this or a mask for each image.",
+    )
+    shared_group.add_argument(
+        "--masks",
+        nargs="+",
+        help="A number of binary foreground mask, one for each image. Alternative to supplying a threshold. Overrides the threshold parameter if supplied.",
+    )
+    shared_group.add_argument(
+        "--ignore",
+        dest="ignore",
+        action="store_true",
+        help="Ignore possible loss of information during the intensity transformation. Should only be used when you know what you are doing.",
+    )
+
+    parser.add_argument(
+        "-v", "--verbose", dest="verbose", action="store_true", help="Verbose output"
+    )
+    parser.add_argument(
+        "-d",
+        "--debug",
+        dest="debug",
+        action="store_true",
+        help="Display debug information.",
+    )
+    parser.add_argument(
+        "-f",
+        "--force",
+        dest="force",
+        action="store_true",
+        help="Overwrite existing files (both model and images)",
+    )
     return parser
-    
+
+
 if __name__ == "__main__":
-    main()        
+    main()
```

### Comparing `MedPy-0.4.0/bin/medpy_label_fit_to_mask.py` & `MedPy-0.5.0/bin/medpy_label_fit_to_mask.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,21 +23,22 @@
 import argparse
 import logging
 import os
 
 # third-party modules
 import numpy
 
-# path changes
-
-# own modules
-from medpy.io import load, save 
 from medpy.core import Logger
 from medpy.filter import fit_labels_to_mask
 
+# own modules
+from medpy.io import load, save
+
+# path changes
+
 
 # information
 __author__ = "Oskar Maier"
 __version__ = "r0.2.0, 2011-12-12"
 __email__ = "oskar.maier@googlemail.com"
 __status__ = "Release"
 __description__ = """
@@ -45,69 +46,94 @@
                   mask and subsequently creating mask out of them.
                   The resulting image is saved in the supplied folder with the same
                   name as the input image, but with a suffix '_reduced' attached.
                   For each region the intersection with the reference mask is computed
                   and if the value exceeds 50% of the total region size, it is marked
                   as mask, otherwise as background. For more details on how the fitting
                   is performed @see filter.fit_labels_to_mask.
-                  
+
                   Copyright (C) 2013 Oskar Maier
                   This program comes with ABSOLUTELY NO WARRANTY; This is free software,
                   and you are welcome to redistribute it under certain conditions; see
-                  the LICENSE file or <http://www.gnu.org/licenses/> for details.   
+                  the LICENSE file or <http://www.gnu.org/licenses/> for details.
                   """
 
+
 # code
 def main():
     # parse cmd arguments
     parser = getParser()
     parser.parse_args()
     args = getArguments(parser)
-    
+
     # prepare logger
     logger = Logger.getInstance()
-    if args.debug: logger.setLevel(logging.DEBUG)
-    elif args.verbose: logger.setLevel(logging.INFO)
-    
+    if args.debug:
+        logger.setLevel(logging.DEBUG)
+    elif args.verbose:
+        logger.setLevel(logging.INFO)
+
     # load input image
-    logger.info('Loading image {}...'.format(args.input))
-    image_labels_data, _ = load(args.image)    
-    
+    logger.info("Loading image {}...".format(args.input))
+    image_labels_data, _ = load(args.image)
+
     # load mask image
-    logger.info('Loading mask {}...'.format(args.mask))
+    logger.info("Loading mask {}...".format(args.mask))
     image_mask_data, image_mask_data_header = load(args.mask)
-    
+
     # check if output image exists
     if not args.force:
         if os.path.exists(args.output):
-            logger.warning('The output image {} already exists. Skipping this image.'.format(args.output))
-    
+            logger.warning(
+                "The output image {} already exists. Skipping this image.".format(
+                    args.output
+                )
+            )
+
     # create a mask from the label image
-    logger.info('Reducing the label image...')
+    logger.info("Reducing the label image...")
     image_reduced_data = fit_labels_to_mask(image_labels_data, image_mask_data)
-    
+
     # save resulting mask
-    logger.info('Saving resulting mask as {} in the same format as input mask, only with data-type int8...'.format(args.output))
-    image_reduced_data = image_reduced_data.astype(numpy.bool, copy=False) # bool sadly not recognized
+    logger.info(
+        "Saving resulting mask as {} in the same format as input mask, only with data-type int8...".format(
+            args.output
+        )
+    )
+    image_reduced_data = image_reduced_data.astype(
+        numpy.bool_, copy=False
+    )  # bool sadly not recognized
     save(image_reduced_data, args.output, image_mask_data_header, args.force)
-    
-    logger.info('Successfully terminated.')
-        
+
+    logger.info("Successfully terminated.")
+
+
 def getArguments(parser):
     "Provides additional validation of the arguments collected by argparse."
     return parser.parse_args()
 
+
 def getParser():
     "Creates and returns the argparse parser object."
     parser = argparse.ArgumentParser(description=__description__)
 
-    parser.add_argument('image', nargs='+', help='The input label image.')
-    parser.add_argument('mask', help='The mask image to which to fit the label images.')
-    parser.add_argument('output', help='The output image.')
-    parser.add_argument('-v', dest='verbose', action='store_true', help='Display more information.')
-    parser.add_argument('-d', dest='debug', action='store_true', help='Display debug information.')
-    parser.add_argument('-f', dest='force', action='store_true', help='Silently override existing output images.')
-    
-    return parser    
-    
+    parser.add_argument("image", nargs="+", help="The input label image.")
+    parser.add_argument("mask", help="The mask image to which to fit the label images.")
+    parser.add_argument("output", help="The output image.")
+    parser.add_argument(
+        "-v", dest="verbose", action="store_true", help="Display more information."
+    )
+    parser.add_argument(
+        "-d", dest="debug", action="store_true", help="Display debug information."
+    )
+    parser.add_argument(
+        "-f",
+        dest="force",
+        action="store_true",
+        help="Silently override existing output images.",
+    )
+
+    return parser
+
+
 if __name__ == "__main__":
-    main()        
+    main()
```

### Comparing `MedPy-0.4.0/bin/medpy_extract_sub_volume_by_example.py` & `MedPy-0.5.0/bin/medpy_extract_sub_volume_by_example.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,143 +15,185 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
-# build-in modules
-from argparse import RawTextHelpFormatter
 import argparse
 import logging
-import sys
 import os
+import sys
+
+# build-in modules
+from argparse import RawTextHelpFormatter
 
 # third-party modules
 import numpy
 
-# path changes
-
 # own modules
 from medpy.core import ArgumentError, Logger
 from medpy.io import load, save
 
+# path changes
+
+
 # information
 __author__ = "Oskar Maier"
 __version__ = "r0.2.0, 2011-12-11"
 __email__ = "oskar.maier@googlemail.com"
 __status__ = "Release"
 __description__ = """
                   Takes a medical image of arbitrary dimensions and a binary mask
                   image of the same dimensions. Extract the exact position of the
                   binary mask in the binary mask image and uses these dimensions
                   for the extraction of a sub-volume that lies inside the dimensions
                   of the medical images.
                   Extracts the sub-volume from the supplied image and saves it.
-                  
+
                   Note that both images must be of the same dimensionality, otherwise an exception is thrown.
                   Note that the input images offset is not taken into account.
                   Note to take into account the input images orientation.
-                  
+
                   This is a convenience script, combining the functionalities of
                   extract_mask_position and extract_sub_volume.
-                  
+
                   Copyright (C) 2013 Oskar Maier
                   This program comes with ABSOLUTELY NO WARRANTY; This is free software,
                   and you are welcome to redistribute it under certain conditions; see
-                  the LICENSE file or <http://www.gnu.org/licenses/> for details.   
+                  the LICENSE file or <http://www.gnu.org/licenses/> for details.
                   """
 
+
 # code
 def main():
     # parse cmd arguments
     parser = getParser()
     parser.parse_args()
     args = getArguments(parser)
-    
+
     # prepare logger
     logger = Logger.getInstance()
-    if args.debug: logger.setLevel(logging.DEBUG)
-    elif args.verbose: logger.setLevel(logging.INFO)
-    
+    if args.debug:
+        logger.setLevel(logging.DEBUG)
+    elif args.verbose:
+        logger.setLevel(logging.INFO)
+
     # load mask
-    logger.info('Loading mask {}...'.format(args.mask))
+    logger.info("Loading mask {}...".format(args.mask))
     mask_image, _ = load(args.mask)
-    
+
     # store mask images shape for later check against the input image
-    mask_image_shape = mask_image.shape 
-    
+    mask_image_shape = mask_image.shape
+
     # extract the position of the foreground object in the mask image
-    logger.info('Extract the position of the foreground object...')
+    logger.info("Extract the position of the foreground object...")
     positions = mask_image.nonzero()
-    positions = [(max(0, positions[i].min() - args.offset), positions[i].max() + 1 + args.offset)
-                    for i in range(len(positions))] # crop negative values
-    logger.debug('Extracted position is {}.'.format(positions))
+    positions = [
+        (max(0, positions[i].min() - args.offset), positions[i].max() + 1 + args.offset)
+        for i in range(len(positions))
+    ]  # crop negative values
+    logger.debug("Extracted position is {}.".format(positions))
 
     # load image
-    logger.info('Loading image {}...'.format(args.image))
+    logger.info("Loading image {}...".format(args.image))
     image_data, image_header = load(args.image)
-    
+
     # check if the mask image and the input image are of the same shape
     if mask_image_shape != image_data.shape:
-        raise ArgumentError('The two input images are of different shape (mask: {} and image: {}).'.format(mask_image_shape, image_data.shape))
-    
-    # execute extraction of the sub-area  
-    logger.info('Extracting sub-volume...')
+        raise ArgumentError(
+            "The two input images are of different shape (mask: {} and image: {}).".format(
+                mask_image_shape, image_data.shape
+            )
+        )
+
+    # execute extraction of the sub-area
+    logger.info("Extracting sub-volume...")
     index = tuple([slice(x[0], x[1]) for x in positions])
     volume = image_data[index]
-    
+
     # check if the output image contains data
     if 0 == len(volume):
-        logger.exception('The extracted sub-volume is of zero-size. This usual means that the mask image contained no foreground object.')
+        logger.exception(
+            "The extracted sub-volume is of zero-size. This usual means that the mask image contained no foreground object."
+        )
         sys.exit(0)
-    
-    logger.debug('Extracted volume is of shape {}.'.format(volume.shape))
-    
+
+    logger.debug("Extracted volume is of shape {}.".format(volume.shape))
+
     # get base origin of the image
-    origin_base = numpy.array([0] * image_data.ndim) # for backwards compatibility
-        
+    origin_base = numpy.array([0] * image_data.ndim)  # for backwards compatibility
+
     # modify the volume offset to imitate numpy behavior (e.g. wrap negative values)
     offset = numpy.array([x[0] for x in positions])
     for i in range(0, len(offset)):
-        if None == offset[i]: offset[i] = 0
-    offset[offset<0] += numpy.array(image_data.shape)[offset<0] # wrap around
-    offset[offset<0] = 0 # set negative to zero
-    
+        if None == offset[i]:
+            offset[i] = 0
+    offset[offset < 0] += numpy.array(image_data.shape)[offset < 0]  # wrap around
+    offset[offset < 0] = 0  # set negative to zero
+
     # calculate final new origin
     origin = origin_base + offset
-    
-    logger.debug('Final origin created as {} + {} = {}.'.format(origin_base, offset, origin))
-    
+
+    logger.debug(
+        "Final origin created as {} + {} = {}.".format(origin_base, offset, origin)
+    )
+
     # save results in same format as input image
-    logger.info('Saving extracted volume...')
+    logger.info("Saving extracted volume...")
     save(volume, args.output, image_header, args.force)
-    
-    logger.info('Successfully terminated.')
 
-    
+    logger.info("Successfully terminated.")
+
+
 def getArguments(parser):
     "Provides additional validation of the arguments collected by argparse."
-    args = parser.parse_args()    
+    args = parser.parse_args()
     # check output image exists if override not forced
     if not args.force:
         if os.path.exists(args.output + args.image[-4:]):
-            raise ArgumentError('The supplied output file {} already exists. Run -f/force flag to override.'.format(args.output))
+            raise ArgumentError(
+                "The supplied output file {} already exists. Run -f/force flag to override.".format(
+                    args.output
+                )
+            )
 
     return args
 
+
 def getParser():
     "Creates and returns the argparse parser object."
-    parser = argparse.ArgumentParser(description=__description__, formatter_class=RawTextHelpFormatter)
-    
-    parser.add_argument('image', help='The input image.')
-    parser.add_argument('output', help='The resulting sub-volume.')
-    parser.add_argument('mask', help='A mask image containing a single foreground object (non-zero).')
-    parser.add_argument('-o', '--offset', dest='offset', default=0, type=int, help='Set an offset by which the extracted sub-volume size should be increased in all directions.')
-    parser.add_argument('-f', dest='force', action='store_true', help='Set this flag to silently override files that exist.')
-    parser.add_argument('-v', dest='verbose', action='store_true', help='Display more information.')
-    parser.add_argument('-d', dest='debug', action='store_true', help='Display debug information.')
-    
-    return parser    
-    
+    parser = argparse.ArgumentParser(
+        description=__description__, formatter_class=RawTextHelpFormatter
+    )
+
+    parser.add_argument("image", help="The input image.")
+    parser.add_argument("output", help="The resulting sub-volume.")
+    parser.add_argument(
+        "mask", help="A mask image containing a single foreground object (non-zero)."
+    )
+    parser.add_argument(
+        "-o",
+        "--offset",
+        dest="offset",
+        default=0,
+        type=int,
+        help="Set an offset by which the extracted sub-volume size should be increased in all directions.",
+    )
+    parser.add_argument(
+        "-f",
+        dest="force",
+        action="store_true",
+        help="Set this flag to silently override files that exist.",
+    )
+    parser.add_argument(
+        "-v", dest="verbose", action="store_true", help="Display more information."
+    )
+    parser.add_argument(
+        "-d", dest="debug", action="store_true", help="Display debug information."
+    )
+
+    return parser
+
+
 if __name__ == "__main__":
-    main()    
+    main()
```

### Comparing `MedPy-0.4.0/bin/medpy_graphcut_voxel.py` & `MedPy-0.5.0/bin/medpy_graphcut_voxel.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,169 +15,239 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
-# build-in modules
-from argparse import RawTextHelpFormatter
 import argparse
 import logging
 import os
 
+# build-in modules
+from argparse import RawTextHelpFormatter
+
 # third-party modules
-import scipy
+import numpy
 
-# path changes
+from medpy import graphcut
 
 # own modules
 from medpy.core import ArgumentError, Logger
-from medpy.io import load, save, header
-from medpy import graphcut
 from medpy.graphcut.wrapper import split_marker
+from medpy.io import header, load, save
 
+# path changes
 
 
 # information
 __author__ = "Oskar Maier"
 __version__ = "r0.3.1, 2012-03-23"
 __email__ = "oskar.maier@googlemail.com"
 __status__ = "Release"
 __description__ = """
                   Perform a binary graph cut using Boykov's max-flow/min-cut algorithm.
-                  
+
                   This implementation does only compute a boundary term and does not use
                   any regional term. The desired boundary term can be selected via the
                   --boundary argument. Depending on the selected term, an additional
                   image has to be supplied as badditional.
-                  
+
                   In the case of the difference of means, it is the original image.
-                  
+
                   Furthermore the algorithm requires a binary image with foreground
                   markers and a binary image with background markers.
-                  
+
                   Additionally a filename for the created binary mask marking foreground
                   and background has to be supplied.
-                  
+
                   Note that the input images must be of the same dimensionality,
                   otherwise an exception is thrown.
                   Note to take into account the input images orientation.
                   Note that the quality of the resulting segmentations depends also on
                   the quality of the supplied markers.
-                  
+
                   Copyright (C) 2013 Oskar Maier
                   This program comes with ABSOLUTELY NO WARRANTY; This is free software,
                   and you are welcome to redistribute it under certain conditions; see
-                  the LICENSE file or <http://www.gnu.org/licenses/> for details.   
+                  the LICENSE file or <http://www.gnu.org/licenses/> for details.
                   """
 
+
 # code
 def main():
     # parse cmd arguments
     parser = getParser()
     parser.parse_args()
     args = getArguments(parser)
-    
+
     # prepare logger
     logger = Logger.getInstance()
-    if args.debug: logger.setLevel(logging.DEBUG)
-    elif args.verbose: logger.setLevel(logging.INFO)
-        
+    if args.debug:
+        logger.setLevel(logging.DEBUG)
+    elif args.verbose:
+        logger.setLevel(logging.INFO)
+
     # check if output image exists
     if not args.force:
         if os.path.exists(args.output):
-            logger.warning('The output image {} already exists. Exiting.'.format(args.output))
+            logger.warning(
+                "The output image {} already exists. Exiting.".format(args.output)
+            )
             exit(-1)
-            
+
     # select boundary term
-    ['diff_linear', 'diff_exp', 'diff_div', 'diff_pow', 'max_linear', 'max_exp', 'max_div', 'max_pow']
-    if 'diff_linear' == args.boundary:
+    [
+        "diff_linear",
+        "diff_exp",
+        "diff_div",
+        "diff_pow",
+        "max_linear",
+        "max_exp",
+        "max_div",
+        "max_pow",
+    ]
+    if "diff_linear" == args.boundary:
         boundary_term = graphcut.energy_voxel.boundary_difference_linear
-        logger.info('Selected boundary term: linear difference of intensities')
-    elif 'diff_exp' == args.boundary:
+        logger.info("Selected boundary term: linear difference of intensities")
+    elif "diff_exp" == args.boundary:
         boundary_term = graphcut.energy_voxel.boundary_difference_exponential
-        logger.info('Selected boundary term: exponential difference of intensities')
-    elif 'diff_div' == args.boundary:
+        logger.info("Selected boundary term: exponential difference of intensities")
+    elif "diff_div" == args.boundary:
         boundary_term = graphcut.energy_voxel.boundary_difference_division
-        logger.info('Selected boundary term: divided difference of intensities')
-    elif 'diff_pow' == args.boundary:
+        logger.info("Selected boundary term: divided difference of intensities")
+    elif "diff_pow" == args.boundary:
         boundary_term = graphcut.energy_voxel.boundary_difference_power
-        logger.info('Selected boundary term: power based / raised difference of intensities')
-    elif 'max_linear' == args.boundary:
+        logger.info(
+            "Selected boundary term: power based / raised difference of intensities"
+        )
+    elif "max_linear" == args.boundary:
         boundary_term = graphcut.energy_voxel.boundary_maximum_linear
-        logger.info('Selected boundary term: linear maximum of intensities')
-    elif 'max_exp' == args.boundary:
+        logger.info("Selected boundary term: linear maximum of intensities")
+    elif "max_exp" == args.boundary:
         boundary_term = graphcut.energy_voxel.boundary_maximum_exponential
-        logger.info('Selected boundary term: exponential maximum of intensities')
-    elif 'max_div' == args.boundary:
+        logger.info("Selected boundary term: exponential maximum of intensities")
+    elif "max_div" == args.boundary:
         boundary_term = graphcut.energy_voxel.boundary_maximum_division
-        logger.info('Selected boundary term: divided maximum of intensities')
-    elif 'max_pow' == args.boundary:
+        logger.info("Selected boundary term: divided maximum of intensities")
+    elif "max_pow" == args.boundary:
         boundary_term = graphcut.energy_voxel.boundary_maximum_power
-        logger.info('Selected boundary term: power based / raised maximum of intensities')
+        logger.info(
+            "Selected boundary term: power based / raised maximum of intensities"
+        )
 
     # load input images
     badditional_image_data, reference_header = load(args.badditional)
     markers_image_data, _ = load(args.markers)
-    
+
     # split marker image into fg and bg images
     fgmarkers_image_data, bgmarkers_image_data = split_marker(markers_image_data)
-       
+
     # check if all images dimensions are the same
-    if not (badditional_image_data.shape == fgmarkers_image_data.shape == bgmarkers_image_data.shape):
-        logger.critical('Not all of the supplied images are of the same shape.')
-        raise ArgumentError('Not all of the supplied images are of the same shape.')
+    if not (
+        badditional_image_data.shape
+        == fgmarkers_image_data.shape
+        == bgmarkers_image_data.shape
+    ):
+        logger.critical("Not all of the supplied images are of the same shape.")
+        raise ArgumentError("Not all of the supplied images are of the same shape.")
 
     # extract spacing if required
     if args.spacing:
         spacing = header.get_pixel_spacing(reference_header)
-        logger.info('Taking spacing of {} into account.'.format(spacing))
+        logger.info("Taking spacing of {} into account.".format(spacing))
     else:
         spacing = False
 
     # generate graph
-    logger.info('Preparing BK_MFMC C++ graph...')
-    gcgraph = graphcut.graph_from_voxels(fgmarkers_image_data,
-                                         bgmarkers_image_data,
-                                         boundary_term = boundary_term,
-                                         boundary_term_args = (badditional_image_data, args.sigma, spacing))
-    
+    logger.info("Preparing BK_MFMC C++ graph...")
+    gcgraph = graphcut.graph_from_voxels(
+        fgmarkers_image_data,
+        bgmarkers_image_data,
+        boundary_term=boundary_term,
+        boundary_term_args=(badditional_image_data, args.sigma, spacing),
+    )
+
     # execute min-cut
-    logger.info('Executing min-cut...')
+    logger.info("Executing min-cut...")
     maxflow = gcgraph.maxflow()
-    logger.debug('Maxflow is {}'.format(maxflow))
-    
+    logger.debug("Maxflow is {}".format(maxflow))
+
     # reshape results to form a valid mask
-    logger.info('Applying results...')
-    result_image_data = scipy.zeros(bgmarkers_image_data.size, dtype=scipy.bool_)
+    logger.info("Applying results...")
+    result_image_data = numpy.zeros(bgmarkers_image_data.size, dtype=numpy.bool_)
     for idx in range(len(result_image_data)):
-        result_image_data[idx] = 0 if gcgraph.termtype.SINK == gcgraph.what_segment(idx) else 1    
+        result_image_data[idx] = (
+            0 if gcgraph.termtype.SINK == gcgraph.what_segment(idx) else 1
+        )
     result_image_data = result_image_data.reshape(bgmarkers_image_data.shape)
-    
-    # save resulting mask    
-    save(result_image_data.astype(scipy.bool_), args.output, reference_header, args.force)
 
-    logger.info('Successfully terminated.')
+    # save resulting mask
+    save(
+        result_image_data.astype(numpy.bool_), args.output, reference_header, args.force
+    )
+
+    logger.info("Successfully terminated.")
+
 
 def getArguments(parser):
     "Provides additional validation of the arguments collected by argparse."
     return parser.parse_args()
 
+
 def getParser():
     "Creates and returns the argparse parser object."
-    parser = argparse.ArgumentParser(description=__description__, formatter_class=RawTextHelpFormatter)
-    
-    parser.add_argument('sigma', type=float, help='The sigma required for the boundary terms.')
-    parser.add_argument('badditional', help='The additional image required by the boundary term. See there for details.')
-    parser.add_argument('markers', help='Image containing the foreground (=1) and background (=2) markers.')
-    parser.add_argument('output', help='The output image containing the segmentation.')
-    parser.add_argument('--boundary', default='diff_exp', help='The boundary term to use. Note that the ones prefixed with diff_ require the original image, while the ones prefixed with max_ require the gradient image.', choices=['diff_linear', 'diff_exp', 'diff_div', 'diff_pow', 'max_linear', 'max_exp', 'max_div', 'max_pow'])
-    parser.add_argument('-s', dest='spacing', action='store_true', help='Set this flag to take the pixel spacing of the image into account. The spacing data will be extracted from the baddtional image.')
-    parser.add_argument('-f', dest='force', action='store_true', help='Set this flag to silently override files that exist.')
-    parser.add_argument('-v', dest='verbose', action='store_true', help='Display more information.')
-    parser.add_argument('-d', dest='debug', action='store_true', help='Display debug information.')
-    
-    return parser    
+    parser = argparse.ArgumentParser(
+        description=__description__, formatter_class=RawTextHelpFormatter
+    )
+
+    parser.add_argument(
+        "sigma", type=float, help="The sigma required for the boundary terms."
+    )
+    parser.add_argument(
+        "badditional",
+        help="The additional image required by the boundary term. See there for details.",
+    )
+    parser.add_argument(
+        "markers",
+        help="Image containing the foreground (=1) and background (=2) markers.",
+    )
+    parser.add_argument("output", help="The output image containing the segmentation.")
+    parser.add_argument(
+        "--boundary",
+        default="diff_exp",
+        help="The boundary term to use. Note that the ones prefixed with diff_ require the original image, while the ones prefixed with max_ require the gradient image.",
+        choices=[
+            "diff_linear",
+            "diff_exp",
+            "diff_div",
+            "diff_pow",
+            "max_linear",
+            "max_exp",
+            "max_div",
+            "max_pow",
+        ],
+    )
+    parser.add_argument(
+        "-s",
+        dest="spacing",
+        action="store_true",
+        help="Set this flag to take the pixel spacing of the image into account. The spacing data will be extracted from the baddtional image.",
+    )
+    parser.add_argument(
+        "-f",
+        dest="force",
+        action="store_true",
+        help="Set this flag to silently override files that exist.",
+    )
+    parser.add_argument(
+        "-v", dest="verbose", action="store_true", help="Display more information."
+    )
+    parser.add_argument(
+        "-d", dest="debug", action="store_true", help="Display debug information."
+    )
+
+    return parser
+
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `MedPy-0.4.0/bin/medpy_merge.py` & `MedPy-0.5.0/bin/medpy_merge.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,76 +19,96 @@
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 # build-in modules
 import argparse
 import logging
 
-# third-party modules
-
-# path changes
-
 # own modules
 from medpy.core import Logger
 from medpy.io import load, save
 
+# third-party modules
+
+# path changes
+
 
 # information
 __author__ = "Oskar Maier"
 __version__ = "r0.1.0, 2012-05-25"
 __email__ = "oskar.maier@googlemail.com"
 __status__ = "Release"
 __description__ = """
                   Merges to images into one.
-                  
+
                   All voxels of the first supplied image that equal False (e.g. zeros),
                   are replaced by the corresponding voxels of the second image.
-                  
+
                   A common use case is the merging of two marker images.
-                  
+
                   Copyright (C) 2013 Oskar Maier
                   This program comes with ABSOLUTELY NO WARRANTY; This is free software,
                   and you are welcome to redistribute it under certain conditions; see
-                  the LICENSE file or <http://www.gnu.org/licenses/> for details.   
+                  the LICENSE file or <http://www.gnu.org/licenses/> for details.
                   """
 
+
 # code
 def main():
     args = getArguments(getParser())
 
     # prepare logger
     logger = Logger.getInstance()
-    if args.debug: logger.setLevel(logging.DEBUG)
-    elif args.verbose: logger.setLevel(logging.INFO)
-    
+    if args.debug:
+        logger.setLevel(logging.DEBUG)
+    elif args.verbose:
+        logger.setLevel(logging.INFO)
+
     # load first input image
     data_input1, header_input1 = load(args.input1)
-    
+
     # load second input image
     data_input2, _ = load(args.input2)
-    
+
     # merge
     data_input1[data_input1 == False] += data_input2[data_input1 == False]
 
     # save resulting volume
     save(data_input1, args.output, header_input1, args.force)
-    
-    logger.info("Successfully terminated.")    
-    
+
+    logger.info("Successfully terminated.")
+
+
 def getArguments(parser):
     "Provides additional validation of the arguments collected by argparse."
     return parser.parse_args()
 
+
 def getParser():
     "Creates and returns the argparse parser object."
     parser = argparse.ArgumentParser(description=__description__)
-    parser.add_argument('input1', help='Source volume one.')
-    parser.add_argument('input2', help='Source volume two.')
-    parser.add_argument('output', help='Target volume.')
-    parser.add_argument('-e', dest='empty', action='store_true', help='Instead of copying the voxel data, create an empty copy conserving all meta-data if possible.')
-    parser.add_argument('-v', dest='verbose', action='store_true', help='Display more information.')
-    parser.add_argument('-d', dest='debug', action='store_true', help='Display debug information.')
-    parser.add_argument('-f', dest='force', action='store_true', help='Silently override existing output images.')
-    return parser    
+    parser.add_argument("input1", help="Source volume one.")
+    parser.add_argument("input2", help="Source volume two.")
+    parser.add_argument("output", help="Target volume.")
+    parser.add_argument(
+        "-e",
+        dest="empty",
+        action="store_true",
+        help="Instead of copying the voxel data, create an empty copy conserving all meta-data if possible.",
+    )
+    parser.add_argument(
+        "-v", dest="verbose", action="store_true", help="Display more information."
+    )
+    parser.add_argument(
+        "-d", dest="debug", action="store_true", help="Display debug information."
+    )
+    parser.add_argument(
+        "-f",
+        dest="force",
+        action="store_true",
+        help="Silently override existing output images.",
+    )
+    return parser
+
 
 if __name__ == "__main__":
-    main()        
+    main()
```

### Comparing `MedPy-0.4.0/bin/medpy_resample.py` & `MedPy-0.5.0/bin/medpy_resample.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,107 +15,141 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
-# build-in modules
-import os
 import argparse
 import logging
 
-# third-party modules
-import scipy.ndimage.interpolation
-
-# path changes
+# build-in modules
+import os
 
 # own modules
 from medpy.core import Logger
-from medpy.io import load, save, header
+from medpy.io import header, load, save
 from medpy.utilities import argparseu
 
+# third-party modules
+
+
+# path changes
+
 
 # information
 __author__ = "Oskar Maier"
 __version__ = "r0.1.1, 2013-07-08"
 __email__ = "oskar.maier@googlemail.com"
 __status__ = "Release"
 __description__ = """
           Resamples an image according to a supplied voxel spacing.
 
           BSpline is used for interpolation. A order between 1 and 5 can be selected.
-          
+
           Note that the pixel data type of the input image is respected, i.e. a integer
           input image leads to an integer output image etc.
 
           Copyright (C) 2013 Oskar Maier
           This program comes with ABSOLUTELY NO WARRANTY; This is free software,
           and you are welcome to redistribute it under certain conditions; see
-          the LICENSE file or <http://www.gnu.org/licenses/> for details.   
+          the LICENSE file or <http://www.gnu.org/licenses/> for details.
                   """
 
+
 # code
 def main():
     parser = getParser()
     args = getArguments(parser)
 
     # prepare logger
     logger = Logger.getInstance()
-    if args.debug: logger.setLevel(logging.DEBUG)
-    elif args.verbose: logger.setLevel(logging.INFO)
-    
+    if args.debug:
+        logger.setLevel(logging.DEBUG)
+    elif args.verbose:
+        logger.setLevel(logging.INFO)
+
     # loading input images
     img, hdr = load(args.input)
 
     # check spacing values
     if not len(args.spacing) == img.ndim:
-        parser.error('The image has {} dimensions, but {} spacing parameters have been supplied.'.format(img.ndim, len(args.spacing)))
-        
+        parser.error(
+            "The image has {} dimensions, but {} spacing parameters have been supplied.".format(
+                img.ndim, len(args.spacing)
+            )
+        )
+
     # check if output image exists
     if not args.force:
         if os.path.exists(args.output):
-            parser.error('The output image {} already exists.'.format(args.output)) 
-        
-    logger.debug('target voxel spacing: {}'.format(args.spacing))
+            parser.error("The output image {} already exists.".format(args.output))
+
+    logger.debug("target voxel spacing: {}".format(args.spacing))
 
     # compute zoom values
-    zoom_factors = [old / float(new) for new, old in zip(args.spacing, header.get_pixel_spacing(hdr))]
-    logger.debug('zoom-factors: {}'.format(zoom_factors))
+    zoom_factors = [
+        old / float(new)
+        for new, old in zip(args.spacing, header.get_pixel_spacing(hdr))
+    ]
+    logger.debug("zoom-factors: {}".format(zoom_factors))
 
     # zoom image
-    img = scipy.ndimage.interpolation.zoom(img, zoom_factors, order=args.order)
-    logger.debug('new image shape: {}'.format(img.shape))
+    img = scipy.ndimage.zoom(img, zoom_factors, order=args.order)
+    logger.debug("new image shape: {}".format(img.shape))
 
     # set new voxel spacing
     header.set_pixel_spacing(hdr, args.spacing)
 
     # saving the resulting image
     save(img, args.output, hdr, args.force)
 
-    
+
 def getArguments(parser):
     "Provides additional validation of the arguments collected by argparse."
     args = parser.parse_args()
     if args.order < 0 or args.order > 5:
-        parser.error('The order has to be a number between 0 and 5.')   
+        parser.error("The order has to be a number between 0 and 5.")
     return args
 
+
 def getParser():
     "Creates and returns the argparse parser object."
     parser = argparse.ArgumentParser(description=__description__)
-    parser.add_argument('input', help='the input image')
-    parser.add_argument('output', help='the output image')
-    parser.add_argument('spacing', type=argparseu.sequenceOfFloatsGt, help='the desired voxel spacing in colon-separated values, e.g. 1.2,1.2,5.0')
-    parser.add_argument('-o', '--order', type=int, default=2, dest='order', help='the bspline order, default is 2;  means nearest neighbours; see also medpy_binary_resampling.py')
-    
-    #group = parser.add_mutually_exclusive_group(required=False)
-    #group.add_argument('--binary', action='store_true', dest='binary', help='enforce binary output image')
-    #group.add_argument('--float', action='store_true', dest='float', help='enforce floating point output image')
-    
-    parser.add_argument('-v', '--verbose', dest='verbose', action='store_true', help='verbose output')
-    parser.add_argument('-d', dest='debug', action='store_true', help='Display debug information.')
-    parser.add_argument('-f', '--force', dest='force', action='store_true', help='overwrite existing files')
+    parser.add_argument("input", help="the input image")
+    parser.add_argument("output", help="the output image")
+    parser.add_argument(
+        "spacing",
+        type=argparseu.sequenceOfFloatsGt,
+        help="the desired voxel spacing in colon-separated values, e.g. 1.2,1.2,5.0",
+    )
+    parser.add_argument(
+        "-o",
+        "--order",
+        type=int,
+        default=2,
+        dest="order",
+        help="the bspline order, default is 2;  means nearest neighbours; see also medpy_binary_resampling.py",
+    )
+
+    # group = parser.add_mutually_exclusive_group(required=False)
+    # group.add_argument('--binary', action='store_true', dest='binary', help='enforce binary output image')
+    # group.add_argument('--float', action='store_true', dest='float', help='enforce floating point output image')
+
+    parser.add_argument(
+        "-v", "--verbose", dest="verbose", action="store_true", help="verbose output"
+    )
+    parser.add_argument(
+        "-d", dest="debug", action="store_true", help="Display debug information."
+    )
+    parser.add_argument(
+        "-f",
+        "--force",
+        dest="force",
+        action="store_true",
+        help="overwrite existing files",
+    )
     return parser
-    
+
+
 if __name__ == "__main__":
-    main()        
+    main()
```

### Comparing `MedPy-0.4.0/bin/medpy_split_xd_to_xminus1d.py` & `MedPy-0.5.0/bin/medpy_split_xd_to_xminus1d.py`

 * *Files 23% similar despite different names*

```diff
@@ -20,95 +20,124 @@
 """
 
 # build-in modules
 import argparse
 import logging
 
 # third-party modules
-import scipy
+import numpy
 
-# path changes
-
-# own modules
-from medpy.io import load, save, header
 from medpy.core import Logger
 from medpy.core.exceptions import ArgumentError
 
+# own modules
+from medpy.io import header, load, save
+
+# path changes
+
 
 # information
 __author__ = "Oskar Maier"
 __version__ = "r0.1.2, 2012-05-25"
 __email__ = "oskar.maier@googlemail.com"
 __status__ = "Release"
 __description__ = """
                   Splits a XD into a number of (X-1)D volumes.
-                  
+
                   One common use case is the creation of manual markers for 4D images.
                   This script allows to split a 4D into a number of either spatial or
                   temporal 3D volumes, for which one then can create the markers. These
                   can be rejoined using the join_xd_to_xplus1d.py script.
-                  
+
                   Copyright (C) 2013 Oskar Maier
                   This program comes with ABSOLUTELY NO WARRANTY; This is free software,
                   and you are welcome to redistribute it under certain conditions; see
-                  the LICENSE file or <http://www.gnu.org/licenses/> for details.   
+                  the LICENSE file or <http://www.gnu.org/licenses/> for details.
                   """
 
+
 # code
 def main():
     # parse cmd arguments
     parser = getParser()
     parser.parse_args()
     args = getArguments(parser)
-    
+
     # prepare logger
     logger = Logger.getInstance()
-    if args.debug: logger.setLevel(logging.DEBUG)
-    elif args.verbose: logger.setLevel(logging.INFO)
-    
+    if args.debug:
+        logger.setLevel(logging.DEBUG)
+    elif args.verbose:
+        logger.setLevel(logging.INFO)
+
     # load input image
     data_input, header_input = load(args.input)
-    
+
     # check if the supplied dimension is valid
     if args.dimension >= data_input.ndim or args.dimension < 0:
-        raise ArgumentError('The supplied cut-dimension {} exceeds the image dimensionality of 0 to {}.'.format(args.dimension, data_input.ndim - 1))
-    
+        raise ArgumentError(
+            "The supplied cut-dimension {} exceeds the image dimensionality of 0 to {}.".format(
+                args.dimension, data_input.ndim - 1
+            )
+        )
+
     # prepare output file string
-    name_output = args.output.replace('{}', '{:03d}')
-    
+    name_output = args.output.replace("{}", "{:03d}")
+
     # compute the new the voxel spacing
     spacing = list(header.get_pixel_spacing(header_input))
     del spacing[args.dimension]
-    
+
     # iterate over the cut dimension
     slices = data_input.ndim * [slice(None)]
     for idx in range(data_input.shape[args.dimension]):
-        # cut the current slice from the original image 
+        # cut the current slice from the original image
         slices[args.dimension] = slice(idx, idx + 1)
-        data_output = scipy.squeeze(data_input[slices])
+        data_output = numpy.squeeze(data_input[tuple(slices)])
         # update the header and set the voxel spacing
         header_input.set_voxel_spacing(spacing)
         # save current slice
         save(data_output, name_output.format(idx), header_input, args.force)
-        
+
     logger.info("Successfully terminated.")
-    
+
+
 def getArguments(parser):
     "Provides additional validation of the arguments collected by argparse."
     args = parser.parse_args()
-    if not '{}' in args.output:
-        raise argparse.ArgumentError(args.output, 'The output argument string must contain the sequence "{}".')
+    if not "{}" in args.output:
+        raise argparse.ArgumentError(
+            args.output, 'The output argument string must contain the sequence "{}".'
+        )
     return args
 
+
 def getParser():
     "Creates and returns the argparse parser object."
     parser = argparse.ArgumentParser(description=__description__)
-    parser.add_argument('input', help='Source volume.')
-    parser.add_argument('output', help='Target volumes. Has to include the sequence "{}" in the place where the volume number should be placed.')
-    parser.add_argument('dimension', type=int, help='The dimension along which to split (starting from 0).')
-    parser.add_argument('-v', dest='verbose', action='store_true', help='Display more information.')
-    parser.add_argument('-d', dest='debug', action='store_true', help='Display debug information.')
-    parser.add_argument('-f', dest='force', action='store_true', help='Silently override existing output images.')
-    return parser    
+    parser.add_argument("input", help="Source volume.")
+    parser.add_argument(
+        "output",
+        help='Target volumes. Has to include the sequence "{}" in the place where the volume number should be placed.',
+    )
+    parser.add_argument(
+        "dimension",
+        type=int,
+        help="The dimension along which to split (starting from 0).",
+    )
+    parser.add_argument(
+        "-v", dest="verbose", action="store_true", help="Display more information."
+    )
+    parser.add_argument(
+        "-d", dest="debug", action="store_true", help="Display debug information."
+    )
+    parser.add_argument(
+        "-f",
+        dest="force",
+        action="store_true",
+        help="Silently override existing output images.",
+    )
+    return parser
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `MedPy-0.4.0/bin/medpy_diff.py` & `MedPy-0.5.0/bin/medpy_diff.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,87 +14,111 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>."""
 
-# build-in modules
-import sys
 import argparse
 import logging
 
-# third-party modules
-import scipy
+# build-in modules
+import sys
+from functools import reduce
 
-# path changes
+# third-party modules
+import numpy
 
 # own modules
 from medpy.core import Logger
 from medpy.io import load
-from functools import reduce
+
+# path changes
 
 
 # information
 __author__ = "Oskar Maier"
 __version__ = "r0.1.0, 2012-05-25"
 __email__ = "oskar.maier@googlemail.com"
 __status__ = "Release"
 __description__ = """
                   Compares the pixel values of two images and gives a measure of the difference.
-                  
+
                   Also compares the dtype and shape.
-                  
+
                   Copyright (C) 2013 Oskar Maier
                   This program comes with ABSOLUTELY NO WARRANTY; This is free software,
                   and you are welcome to redistribute it under certain conditions; see
-                  the LICENSE file or <http://www.gnu.org/licenses/> for details.   
+                  the LICENSE file or <http://www.gnu.org/licenses/> for details.
                   """
 
+
 # code
 def main():
     args = getArguments(getParser())
 
     # prepare logger
     logger = Logger.getInstance()
-    if args.debug: logger.setLevel(logging.DEBUG)
-    elif args.verbose: logger.setLevel(logging.INFO)
-    
+    if args.debug:
+        logger.setLevel(logging.DEBUG)
+    elif args.verbose:
+        logger.setLevel(logging.INFO)
+
     # load input image1
     data_input1, _ = load(args.input1)
-    
+
     # load input image2
     data_input2, _ = load(args.input2)
-    
+
     # compare dtype and shape
-    if not data_input1.dtype == data_input2.dtype: print('Dtype differs: {} to {}'.format(data_input1.dtype, data_input2.dtype))
+    if not data_input1.dtype == data_input2.dtype:
+        print("Dtype differs: {} to {}".format(data_input1.dtype, data_input2.dtype))
     if not data_input1.shape == data_input2.shape:
-        print('Shape differs: {} to {}'.format(data_input1.shape, data_input2.shape))
-        print('The voxel content of images of different shape can not be compared. Exiting.')
+        print("Shape differs: {} to {}".format(data_input1.shape, data_input2.shape))
+        print(
+            "The voxel content of images of different shape can not be compared. Exiting."
+        )
         sys.exit(-1)
-    
+
     # compare image data
-    voxel_total = reduce(lambda x, y: x*y, data_input1.shape)
+    voxel_total = reduce(lambda x, y: x * y, data_input1.shape)
     voxel_difference = len((data_input1 != data_input2).nonzero()[0])
     if not 0 == voxel_difference:
-        print('Voxel differ: {} of {} total voxels'.format(voxel_difference, voxel_total))
-        print('Max difference: {}'.format(scipy.absolute(data_input1 - data_input2).max()))
-    else: print('No other difference.')
-    
-    logger.info("Successfully terminated.")    
-    
+        print(
+            "Voxel differ: {} of {} total voxels".format(voxel_difference, voxel_total)
+        )
+        print(
+            "Max difference: {}".format(numpy.absolute(data_input1 - data_input2).max())
+        )
+    else:
+        print("No other difference.")
+
+    logger.info("Successfully terminated.")
+
+
 def getArguments(parser):
     "Provides additional validation of the arguments collected by argparse."
     return parser.parse_args()
 
+
 def getParser():
     "Creates and returns the argparse parser object."
     parser = argparse.ArgumentParser(description=__description__)
-    parser.add_argument('input1', help='Source volume one.')
-    parser.add_argument('input2', help='Source volume two.')
-    parser.add_argument('-v', dest='verbose', action='store_true', help='Display more information.')
-    parser.add_argument('-d', dest='debug', action='store_true', help='Display debug information.')
-    parser.add_argument('-f', dest='force', action='store_true', help='Silently override existing output images.')
-    return parser    
+    parser.add_argument("input1", help="Source volume one.")
+    parser.add_argument("input2", help="Source volume two.")
+    parser.add_argument(
+        "-v", dest="verbose", action="store_true", help="Display more information."
+    )
+    parser.add_argument(
+        "-d", dest="debug", action="store_true", help="Display debug information."
+    )
+    parser.add_argument(
+        "-f",
+        dest="force",
+        action="store_true",
+        help="Silently override existing output images.",
+    )
+    return parser
+
 
 if __name__ == "__main__":
-    main()        
+    main()
```

### Comparing `MedPy-0.4.0/bin/medpy_apparent_diffusion_coefficient.py` & `MedPy-0.5.0/bin/medpy_apparent_diffusion_coefficient.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,25 +21,24 @@
 
 # build-in modules
 import argparse
 import logging
 
 # third-party modules
 import numpy
-from scipy.ndimage.morphology import binary_fill_holes, binary_dilation,\
-    binary_erosion
-
-# path changes
+from scipy.ndimage import binary_dilation, binary_erosion, binary_fill_holes
 
 # own modules
 from medpy.core import Logger
-from medpy.io import load, save, header
-from medpy.filter import otsu
 from medpy.core.exceptions import ArgumentError
+from medpy.filter import otsu
 from medpy.filter.binary import largest_connected_component
+from medpy.io import header, load, save
+
+# path changes
 
 
 # information
 __author__ = "Oskar Maier"
 __version__ = "r0.1.1, 2013-07-18"
 __email__ = "oskar.maier@googlemail.com"
 __status__ = "Release"
@@ -77,93 +76,143 @@
 Patric Hagmann et al.
 [2] "Understanding the Mathematics Involved in Calculating Apparent
 Diffusion Coefficient Maps" by Michael Yong Park and Jae Young Byun
 
 Copyright (C) 2013 Oskar Maier
 This program comes with ABSOLUTELY NO WARRANTY; This is free software,
 and you are welcome to redistribute it under certain conditions; see
-the LICENSE file or <http://www.gnu.org/licenses/> for details.   
+the LICENSE file or <http://www.gnu.org/licenses/> for details.
                   """
 
+
 # code
 def main():
     args = getArguments(getParser())
 
     # prepare logger
     logger = Logger.getInstance()
-    if args.debug: logger.setLevel(logging.DEBUG)
-    elif args.verbose: logger.setLevel(logging.INFO)
-    
+    if args.debug:
+        logger.setLevel(logging.DEBUG)
+    elif args.verbose:
+        logger.setLevel(logging.INFO)
+
     # loading input images
     b0img, b0hdr = load(args.b0image)
     bximg, bxhdr = load(args.bximage)
-    
+
     # convert to float
-    b0img = b0img.astype(numpy.float)
-    bximg = bximg.astype(numpy.float)
+    b0img = b0img.astype(float)
+    bximg = bximg.astype(float)
 
     # check if image are compatible
     if not b0img.shape == bximg.shape:
-        raise ArgumentError('The input images shapes differ i.e. {} != {}.'.format(b0img.shape, bximg.shape))
+        raise ArgumentError(
+            "The input images shapes differ i.e. {} != {}.".format(
+                b0img.shape, bximg.shape
+            )
+        )
     if not header.get_pixel_spacing(b0hdr) == header.get_pixel_spacing(bxhdr):
-        raise ArgumentError('The input images voxel spacing differs i.e. {} != {}.'.format(header.get_pixel_spacing(b0hdr), header.get_pixel_spacing(bxhdr)))
-    
+        raise ArgumentError(
+            "The input images voxel spacing differs i.e. {} != {}.".format(
+                header.get_pixel_spacing(b0hdr), header.get_pixel_spacing(bxhdr)
+            )
+        )
+
     # check if supplied threshold value as well as the b value is above 0
     if args.threshold is not None and not args.threshold >= 0:
-        raise ArgumentError('The supplied threshold value must be greater than 0, otherwise a division through 0 might occur.')
+        raise ArgumentError(
+            "The supplied threshold value must be greater than 0, otherwise a division through 0 might occur."
+        )
     if not args.b > 0:
-        raise ArgumentError('The supplied b-value must be greater than 0.')
-    
+        raise ArgumentError("The supplied b-value must be greater than 0.")
+
     # compute threshold value if not supplied
     if args.threshold is None:
-        b0thr = otsu(b0img, 32) / 4. # divide by 4 to decrease impact
-        bxthr = otsu(bximg, 32) / 4.
+        b0thr = otsu(b0img, 32) / 4.0  # divide by 4 to decrease impact
+        bxthr = otsu(bximg, 32) / 4.0
         if 0 >= b0thr:
-            raise ArgumentError('The supplied b0image seems to contain negative values.')
+            raise ArgumentError(
+                "The supplied b0image seems to contain negative values."
+            )
         if 0 >= bxthr:
-            raise ArgumentError('The supplied bximage seems to contain negative values.')
+            raise ArgumentError(
+                "The supplied bximage seems to contain negative values."
+            )
     else:
         b0thr = bxthr = args.threshold
-    
-    logger.debug('thresholds={}/{}, b-value={}'.format(b0thr, bxthr, args.b))
-    
+
+    logger.debug("thresholds={}/{}, b-value={}".format(b0thr, bxthr, args.b))
+
     # threshold b0 + bx DW image to obtain a mask
     # b0 mask avoid division through 0, bx mask avoids a zero in the ln(x) computation
     mask = binary_fill_holes(b0img > b0thr) & binary_fill_holes(bximg > bxthr)
-    
+
     # perform a number of binary morphology steps to select the brain only
     mask = binary_erosion(mask, iterations=1)
     mask = largest_connected_component(mask)
     mask = binary_dilation(mask, iterations=1)
-    
-    logger.debug('excluding {} of {} voxels from the computation and setting them to zero'.format(numpy.count_nonzero(mask), numpy.prod(mask.shape)))
-    
+
+    logger.debug(
+        "excluding {} of {} voxels from the computation and setting them to zero".format(
+            numpy.count_nonzero(mask), numpy.prod(mask.shape)
+        )
+    )
+
     # compute the ADC
     adc = numpy.zeros(b0img.shape, b0img.dtype)
-    adc[mask] = -1. * args.b * numpy.log(bximg[mask] / b0img[mask])
+    adc[mask] = -1.0 * args.b * numpy.log(bximg[mask] / b0img[mask])
     adc[adc < 0] = 0
-            
+
     # saving the resulting image
     save(adc, args.output, b0hdr, args.force)
 
-    
+
 def getArguments(parser):
     "Provides additional validation of the arguments collected by argparse."
     return parser.parse_args()
 
+
 def getParser():
     "Creates and returns the argparse parser object."
-    parser = argparse.ArgumentParser(description=__description__, formatter_class=argparse.RawDescriptionHelpFormatter)
-    parser.add_argument('b0image', help='the diffusion weighted image required with b=0')
-    parser.add_argument('bximage', help='the diffusion weighted image required with b=x')
-    parser.add_argument('b', type=int, help='the b-value used to acquire the bx-image (i.e. x)')
-    parser.add_argument('output', help='the computed apparent diffusion coefficient image')
-    
-    parser.add_argument('-t', '--threshold', type=int, dest='threshold', help='set a fixed threshold for the input images to mask the computation')
-    
-    parser.add_argument('-v', '--verbose', dest='verbose', action='store_true', help='verbose output')
-    parser.add_argument('-d', dest='debug', action='store_true', help='Display debug information.')
-    parser.add_argument('-f', '--force', dest='force', action='store_true', help='overwrite existing files')
+    parser = argparse.ArgumentParser(
+        description=__description__,
+        formatter_class=argparse.RawDescriptionHelpFormatter,
+    )
+    parser.add_argument(
+        "b0image", help="the diffusion weighted image required with b=0"
+    )
+    parser.add_argument(
+        "bximage", help="the diffusion weighted image required with b=x"
+    )
+    parser.add_argument(
+        "b", type=int, help="the b-value used to acquire the bx-image (i.e. x)"
+    )
+    parser.add_argument(
+        "output", help="the computed apparent diffusion coefficient image"
+    )
+
+    parser.add_argument(
+        "-t",
+        "--threshold",
+        type=int,
+        dest="threshold",
+        help="set a fixed threshold for the input images to mask the computation",
+    )
+
+    parser.add_argument(
+        "-v", "--verbose", dest="verbose", action="store_true", help="verbose output"
+    )
+    parser.add_argument(
+        "-d", dest="debug", action="store_true", help="Display debug information."
+    )
+    parser.add_argument(
+        "-f",
+        "--force",
+        dest="force",
+        action="store_true",
+        help="overwrite existing files",
+    )
     return parser
-    
+
+
 if __name__ == "__main__":
-    main()        
+    main()
```

### Comparing `MedPy-0.4.0/bin/medpy_graphcut_label_wsplit.py` & `MedPy-0.5.0/bin/medpy_graphcut_label_wsplit.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,127 +15,152 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
-# build-in modules
-from argparse import RawTextHelpFormatter
 import argparse
 import logging
 import os
 
-# third-party modules
-
-# path changes
+# build-in modules
+from argparse import RawTextHelpFormatter
 
 # own modules
 from medpy.core import Logger
+from medpy.graphcut.wrapper import graphcut_split, graphcut_stawiaski, split_marker
 from medpy.io import load, save
-from medpy.graphcut.wrapper import split_marker, graphcut_split,\
-    graphcut_stawiaski
 
+# third-party modules
+
+# path changes
 
 
 # information
 __author__ = "Oskar Maier"
 __version__ = "r0.3.4, 2012-03-16"
 __email__ = "oskar.maier@googlemail.com"
 __status__ = "Release"
 __description__ = """
                   !Modified version of original GC label, as splits the volumes into
                   more handy sizes before processing them. Also uses multiple subprocesses.
-                  
+
                   Perform a binary graph cut using Boykov's max-flow/min-cut algorithm.
-                  
+
                   This implementation does only compute a boundary term and does not use
                   any regional term. The desired boundary term can be selected via the
                   --boundary argument. Depending on the selected term, an additional
                   image has to be supplied as badditional.
-                  
+
                   In the case of the stawiaski boundary term, this is the gradient image.
                   In the case of the difference of means, it is the original image.
-                  
+
                   Furthermore the algorithm requires the region map of the original
                   image, a binary image with foreground markers and a binary
                   image with background markers.
-                  
+
                   Additionally a filename for the created binary mask marking foreground
                   and background has to be supplied.
-                  
+
                   Note that the input images must be of the same dimensionality,
                   otherwise an exception is thrown.
                   Note to take into account the input images orientation.
                   Note that the quality of the resulting segmentations depends also on
                   the quality of the supplied markers.
-                  
+
                   Copyright (C) 2013 Oskar Maier
                   This program comes with ABSOLUTELY NO WARRANTY; This is free software,
                   and you are welcome to redistribute it under certain conditions; see
-                  the LICENSE file or <http://www.gnu.org/licenses/> for details.   
+                  the LICENSE file or <http://www.gnu.org/licenses/> for details.
                   """
 
+
 # code
 def main():
     # parse cmd arguments
     parser = getParser()
     parser.parse_args()
     args = getArguments(parser)
-    
+
     # prepare logger
     logger = Logger.getInstance()
-    if args.debug: logger.setLevel(logging.DEBUG)
-    elif args.verbose: logger.setLevel(logging.INFO)
-        
+    if args.debug:
+        logger.setLevel(logging.DEBUG)
+    elif args.verbose:
+        logger.setLevel(logging.INFO)
+
     # check if output image exists
     if not args.force:
         if os.path.exists(args.output):
-            logger.warning('The output image {} already exists. Exiting.'.format(args.output))
+            logger.warning(
+                "The output image {} already exists. Exiting.".format(args.output)
+            )
             exit(-1)
-            
+
     # constants
     # the minimal edge length of a subvolume-cube ! has to be of type int!
     minimal_edge_length = 200
     overlap = 20
-    
+
     # load input images
     region_image_data, reference_header = load(args.region)
     markers_image_data, _ = load(args.markers)
     gradient_image_data, _ = load(args.gradient)
-    
+
     # split marker image into fg and bg images
     fgmarkers_image_data, bgmarkers_image_data = split_marker(markers_image_data)
-       
+
     # execute distributed graph cut
-    output_volume = graphcut_split(graphcut_stawiaski,
-                                   region_image_data,
-                                   gradient_image_data,
-                                   fgmarkers_image_data,
-                                   bgmarkers_image_data,
-                                   minimal_edge_length,
-                                   overlap)
-    
+    output_volume = graphcut_split(
+        graphcut_stawiaski,
+        region_image_data,
+        gradient_image_data,
+        fgmarkers_image_data,
+        bgmarkers_image_data,
+        minimal_edge_length,
+        overlap,
+    )
+
     # save resulting mask
     save(output_volume, args.output, reference_header, args.force)
 
-    logger.info('Successfully terminated.')
+    logger.info("Successfully terminated.")
+
 
 def getArguments(parser):
     "Provides additional validation of the arguments collected by argparse."
     return parser.parse_args()
 
+
 def getParser():
     "Creates and returns the argparse parser object."
-    parser = argparse.ArgumentParser(description=__description__, formatter_class=RawTextHelpFormatter)
-    parser.add_argument('gradient', help='The gradient magnitude image of the image to segment.')
-    parser.add_argument('region', help='The region image of the image to segment.')
-    parser.add_argument('markers', help='Binary image containing the foreground (=1) and background (=2) markers.')
-    parser.add_argument('output', help='The output image containing the segmentation.')
-    parser.add_argument('-f', dest='force', action='store_true', help='Set this flag to silently override files that exist.')
-    parser.add_argument('-v', dest='verbose', action='store_true', help='Display more information.')
-    parser.add_argument('-d', dest='debug', action='store_true', help='Display debug information.')
-    
-    return parser    
+    parser = argparse.ArgumentParser(
+        description=__description__, formatter_class=RawTextHelpFormatter
+    )
+    parser.add_argument(
+        "gradient", help="The gradient magnitude image of the image to segment."
+    )
+    parser.add_argument("region", help="The region image of the image to segment.")
+    parser.add_argument(
+        "markers",
+        help="Binary image containing the foreground (=1) and background (=2) markers.",
+    )
+    parser.add_argument("output", help="The output image containing the segmentation.")
+    parser.add_argument(
+        "-f",
+        dest="force",
+        action="store_true",
+        help="Set this flag to silently override files that exist.",
+    )
+    parser.add_argument(
+        "-v", dest="verbose", action="store_true", help="Display more information."
+    )
+    parser.add_argument(
+        "-d", dest="debug", action="store_true", help="Display debug information."
+    )
+
+    return parser
+
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `MedPy-0.4.0/bin/medpy_gradient.py` & `MedPy-0.5.0/bin/medpy_gradient.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,84 +20,101 @@
 """
 
 # build-in modules
 import argparse
 import logging
 
 # third-party modules
-import scipy
-from scipy.ndimage.filters import generic_gradient_magnitude, prewitt
+import numpy
+from scipy.ndimage import generic_gradient_magnitude, prewitt
 
-# path changes
+from medpy.core import Logger
 
 # own modules
 from medpy.io import load, save
-from medpy.core import Logger
 
+# path changes
 
 
 # information
 __author__ = "Oskar Maier"
 __version__ = "r0.2.0, 2011-12-12"
 __email__ = "oskar.maier@googlemail.com"
 __status__ = "Release"
 __description__ = """
                   Creates a height map of the input images using the gradient magnitude
                   filter.
                   The pixel type of the resulting image will be float.
-                  
+
                   Copyright (C) 2013 Oskar Maier
                   This program comes with ABSOLUTELY NO WARRANTY; This is free software,
                   and you are welcome to redistribute it under certain conditions; see
-                  the LICENSE file or <http://www.gnu.org/licenses/> for details.   
+                  the LICENSE file or <http://www.gnu.org/licenses/> for details.
                   """
 
+
 # code
 def main():
     # parse cmd arguments
     parser = getParser()
     parser.parse_args()
     args = getArguments(parser)
-    
+
     # prepare logger
     logger = Logger.getInstance()
-    if args.debug: logger.setLevel(logging.DEBUG)
-    elif args.verbose: logger.setLevel(logging.INFO)
-    
+    if args.debug:
+        logger.setLevel(logging.DEBUG)
+    elif args.verbose:
+        logger.setLevel(logging.INFO)
+
     # laod input image
     data_input, header_input = load(args.input)
-    
-#    # check if output image exists
-#    if not args.force:
-#        if os.path.exists(image_gradient_name):
-#            logger.warning('The output image {} already exists. Skipping this step.'.format(image_gradient_name))
-#            continue        
-        
+
+    #    # check if output image exists
+    #    if not args.force:
+    #        if os.path.exists(image_gradient_name):
+    #            logger.warning('The output image {} already exists. Skipping this step.'.format(image_gradient_name))
+    #            continue
+
     # prepare result image
-    data_output = scipy.zeros(data_input.shape, dtype=scipy.float32)
-        
+    data_output = numpy.zeros(data_input.shape, dtype=numpy.float32)
+
     # apply the gradient magnitude filter
-    logger.info('Computing the gradient magnitude with Prewitt operator...')
-    generic_gradient_magnitude(data_input, prewitt, output=data_output) # alternative to prewitt is sobel
-        
+    logger.info("Computing the gradient magnitude with Prewitt operator...")
+    generic_gradient_magnitude(
+        data_input, prewitt, output=data_output
+    )  # alternative to prewitt is sobel
+
     # save resulting mask
     save(data_output, args.output, header_input, args.force)
-    
-    logger.info('Successfully terminated.')
-        
+
+    logger.info("Successfully terminated.")
+
+
 def getArguments(parser):
     "Provides additional validation of the arguments collected by argparse."
     return parser.parse_args()
 
+
 def getParser():
     "Creates and returns the argparse parser object."
     parser = argparse.ArgumentParser(description=__description__)
-    parser.add_argument('input', help='Source volume.')
-    parser.add_argument('output', help='Target volume.')
-    parser.add_argument('-v', dest='verbose', action='store_true', help='Display more information.')
-    parser.add_argument('-d', dest='debug', action='store_true', help='Display debug information.')
-    parser.add_argument('-f', dest='force', action='store_true', help='Silently override existing output images.')
-    
-    return parser    
-    
+    parser.add_argument("input", help="Source volume.")
+    parser.add_argument("output", help="Target volume.")
+    parser.add_argument(
+        "-v", dest="verbose", action="store_true", help="Display more information."
+    )
+    parser.add_argument(
+        "-d", dest="debug", action="store_true", help="Display debug information."
+    )
+    parser.add_argument(
+        "-f",
+        dest="force",
+        action="store_true",
+        help="Silently override existing output images.",
+    )
+
+    return parser
+
+
 if __name__ == "__main__":
-    main()        
+    main()
```

### Comparing `MedPy-0.4.0/bin/medpy_extract_sub_volume_auto.py` & `MedPy-0.5.0/bin/medpy_extract_sub_volume_auto.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,122 +15,175 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
-# build-in modules
-from argparse import RawTextHelpFormatter
 import argparse
 import logging
 import os
 
-# third-party modules
-
-# path changes
+# build-in modules
+from argparse import RawTextHelpFormatter
 
 # own modules
 from medpy.core import ArgumentError, Logger
 from medpy.io import load, save
 
+# third-party modules
+
+# path changes
+
+
 # information
 __author__ = "Oskar Maier"
 __version__ = "r0.2.1, 2012-05-17"
 __email__ = "oskar.maier@googlemail.com"
 __status__ = "Release"
 __description__ = """
                   Takes a medical image of arbitrary dimensions and splits it into a
                   number of sub-volumes along the supplied dimensions. The maximum size
                   of each such created volume can be supplied.
-                  
+
                   Note to take into account the input images orientation when supplying the cut dimension.
                   Note that the image offsets are not preserved.
-                  
+
                   Copyright (C) 2013 Oskar Maier
                   This program comes with ABSOLUTELY NO WARRANTY; This is free software,
                   and you are welcome to redistribute it under certain conditions; see
-                  the LICENSE file or <http://www.gnu.org/licenses/> for details.   
+                  the LICENSE file or <http://www.gnu.org/licenses/> for details.
                   """
 
+
 # code
 def main():
     # parse cmd arguments
     parser = getParser()
     parser.parse_args()
     args = getArguments(parser)
-    
+
     # prepare logger
     logger = Logger.getInstance()
-    if args.debug: logger.setLevel(logging.DEBUG)
-    elif args.verbose: logger.setLevel(logging.INFO)
-        
+    if args.debug:
+        logger.setLevel(logging.DEBUG)
+    elif args.verbose:
+        logger.setLevel(logging.INFO)
+
     # load input image
-    logger.info('Loading {}...'.format(args.image))
+    logger.info("Loading {}...".format(args.image))
     image_data, image_header = load(args.image)
-    
+
     # check if supplied cut dimension is inside the input images dimensions
     if args.dimension < 0 or args.dimension >= image_data.ndim:
-        logger.critical('The supplied cut-dimensions {} is invalid. The input image has only {} dimensions.'.format(args.dimension, image_data.ndim))
-        raise ArgumentError('The supplied cut-dimensions {} is invalid. The input image has only {} dimensions.'.format(args.dimension, image_data.ndim))
-    
+        logger.critical(
+            "The supplied cut-dimensions {} is invalid. The input image has only {} dimensions.".format(
+                args.dimension, image_data.ndim
+            )
+        )
+        raise ArgumentError(
+            "The supplied cut-dimensions {} is invalid. The input image has only {} dimensions.".format(
+                args.dimension, image_data.ndim
+            )
+        )
+
     # prepare output filenames
-    name_output = args.output.replace('{}', '{:03d}')
-    
+    name_output = args.output.replace("{}", "{:03d}")
+
     # determine cut lines
-    no_sub_volumes = image_data.shape[args.dimension] / args.maxsize + 1 # int-division is desired
-    slices_per_volume = image_data.shape[args.dimension] / no_sub_volumes # int-division is desired
-    
+    no_sub_volumes = (
+        image_data.shape[args.dimension] / args.maxsize + 1
+    )  # int-division is desired
+    slices_per_volume = (
+        image_data.shape[args.dimension] / no_sub_volumes
+    )  # int-division is desired
+
     # construct processing dict for each sub-volume
     processing_array = []
     for i in range(no_sub_volumes):
         processing_array.append(
-            {'path': name_output.format(i+1),
-             'cut': (i * slices_per_volume, (i + 1) * slices_per_volume)})
-        if no_sub_volumes - 1 == i: # last volume has to have increased cut end
-            processing_array[i]['cut'] = (processing_array[i]['cut'][0], image_data.shape[args.dimension])
+            {
+                "path": name_output.format(i + 1),
+                "cut": (i * slices_per_volume, (i + 1) * slices_per_volume),
+            }
+        )
+        if no_sub_volumes - 1 == i:  # last volume has to have increased cut end
+            processing_array[i]["cut"] = (
+                processing_array[i]["cut"][0],
+                image_data.shape[args.dimension],
+            )
 
     # construct base indexing list
     index = [slice(None) for _ in range(image_data.ndim)]
-    
+
     # execute extraction of the sub-volumes
-    logger.info('Extracting sub-volumes...')
+    logger.info("Extracting sub-volumes...")
     for dic in processing_array:
         # check if output images exists
         if not args.force:
-            if os.path.exists(dic['path']):
-                logger.warning('The output file {} already exists. Skipping this volume.'.format(dic['path']))
+            if os.path.exists(dic["path"]):
+                logger.warning(
+                    "The output file {} already exists. Skipping this volume.".format(
+                        dic["path"]
+                    )
+                )
                 continue
-        
+
         # extracting sub-volume
-        index[args.dimension] = slice(dic['cut'][0], dic['cut'][1])
-        volume = image_data[index]
-        
-        logger.debug('Extracted volume is of shape {}.'.format(volume.shape))
-        
+        index[args.dimension] = slice(dic["cut"][0], dic["cut"][1])
+        volume = image_data[tuple(index)]
+
+        logger.debug("Extracted volume is of shape {}.".format(volume.shape))
+
         # saving sub-volume in same format as input image
-        logger.info('Saving cut {} as {}...'.format(dic['cut'], dic['path']))
-        save(volume, dic['path'], image_header, args.force)
-        
-    logger.info('Successfully terminated.')
+        logger.info("Saving cut {} as {}...".format(dic["cut"], dic["path"]))
+        save(volume, dic["path"], image_header, args.force)
+
+    logger.info("Successfully terminated.")
+
 
-    
 def getArguments(parser):
     "Provides additional validation of the arguments collected by argparse."
     return parser.parse_args()
 
+
 def getParser():
     "Creates and returns the argparse parser object."
-    parser = argparse.ArgumentParser(description=__description__, formatter_class=RawTextHelpFormatter)
-    
-    parser.add_argument('image', help='An image of arbitrary dimensions that should be split.')
-    parser.add_argument('output', help='Output volumes. Has to include the sequence "{}" in the place where the volume number should be placed.')
-    parser.add_argument('dimension', type=int, help='The dimension in which direction to split (starting from 0:x).')
-    parser.add_argument('maxsize', type=int, help='The produced volumes will always be smaller than this size (in terms of slices in the cut-dimension).')
-    parser.add_argument('-f', dest='force', action='store_true', help='Set this flag to silently override files that exist.')
-    parser.add_argument('-v', dest='verbose', action='store_true', help='Display more information.')
-    parser.add_argument('-d', dest='debug', action='store_true', help='Display debug information.')
-    
-    return parser    
-    
+    parser = argparse.ArgumentParser(
+        description=__description__, formatter_class=RawTextHelpFormatter
+    )
+
+    parser.add_argument(
+        "image", help="An image of arbitrary dimensions that should be split."
+    )
+    parser.add_argument(
+        "output",
+        help='Output volumes. Has to include the sequence "{}" in the place where the volume number should be placed.',
+    )
+    parser.add_argument(
+        "dimension",
+        type=int,
+        help="The dimension in which direction to split (starting from 0:x).",
+    )
+    parser.add_argument(
+        "maxsize",
+        type=int,
+        help="The produced volumes will always be smaller than this size (in terms of slices in the cut-dimension).",
+    )
+    parser.add_argument(
+        "-f",
+        dest="force",
+        action="store_true",
+        help="Set this flag to silently override files that exist.",
+    )
+    parser.add_argument(
+        "-v", dest="verbose", action="store_true", help="Display more information."
+    )
+    parser.add_argument(
+        "-d", dest="debug", action="store_true", help="Display debug information."
+    )
+
+    return parser
+
+
 if __name__ == "__main__":
-    main()    
+    main()
```

### Comparing `MedPy-0.4.0/bin/medpy_label_superimposition.py` & `MedPy-0.5.0/bin/medpy_label_superimposition.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,122 +15,184 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
-# build-in modules
-from argparse import ArgumentError
 import argparse
 import logging
 import os
 
+# build-in modules
+from argparse import ArgumentError
+
 # third-party modules
-import scipy
+import numpy
 
-# path changes
+from medpy.core import Logger
 
 # own modules
 from medpy.io import load, save
-from medpy.core import Logger
+
+# path changes
+
 
 # information
 __author__ = "Oskar Maier"
 __version__ = "r0.2.1, 2011-01-04"
 __email__ = "oskar.maier@googlemail.com"
 __status__ = "Release"
 __description__ = """
                   Takes two label images as input and creates their superimposition i.e.
                   all the regions borders are preserved and the resulting image contains
                   more or the same number of regions as the respective input images.
-                  
+
                   The resulting image has the same name as the first input image, just
                   with a '_superimp' suffix.
-                  
+
                   Copyright (C) 2013 Oskar Maier
                   This program comes with ABSOLUTELY NO WARRANTY; This is free software,
                   and you are welcome to redistribute it under certain conditions; see
-                  the LICENSE file or <http://www.gnu.org/licenses/> for details.   
+                  the LICENSE file or <http://www.gnu.org/licenses/> for details.
                   """
 
+
 # code
 def main():
     # parse cmd arguments
     parser = getParser()
     parser.parse_args()
     args = getArguments(parser)
-    
+
     # prepare logger
     logger = Logger.getInstance()
-    if args.debug: logger.setLevel(logging.DEBUG)
-    elif args.verbose: logger.setLevel(logging.INFO)
+    if args.debug:
+        logger.setLevel(logging.DEBUG)
+    elif args.verbose:
+        logger.setLevel(logging.INFO)
 
     # build output image name
-    image_superimposition_name = args.folder + '/' + args.image1.split('/')[-1][:-4] + '_superimp'
-    image_superimposition_name += args.image1.split('/')[-1][-4:]
-        
+    image_superimposition_name = (
+        args.folder + "/" + args.image1.split("/")[-1][:-4] + "_superimp"
+    )
+    image_superimposition_name += args.image1.split("/")[-1][-4:]
+
     # check if output image exists
     if not args.force:
         if os.path.exists(image_superimposition_name):
-            raise ArgumentError('The output image {} already exists. Please provide the -f/force flag, if you wish to override it.'.format(image_superimposition_name))
-    
+            raise ArgumentError(
+                "The output image {} already exists. Please provide the -f/force flag, if you wish to override it.".format(
+                    image_superimposition_name
+                )
+            )
+
     # load image1 using
-    logger.info('Loading image {}...'.format(args.image1))
+    logger.info("Loading image {}...".format(args.image1))
     image1_data, image1_header = load(args.image1)
-    
+
     # load image2 using
-    logger.info('Loading image {}...'.format(args.image2))
+    logger.info("Loading image {}...".format(args.image2))
     image2_data, _ = load(args.image2)
-        
+
     # check input images to be valid
-    logger.info('Checking input images for correctness...')
+    logger.info("Checking input images for correctness...")
     if image1_data.shape != image2_data.shape:
-        raise ArgumentError('The two input images shape do not match with 1:{} and 2:{}'.format(image1_data.shape, image2_data.shape))
-    int_types = (scipy.uint, scipy.uint0, scipy.uint8, scipy.uint16, scipy.uint32, scipy.uint64, scipy.uintc, scipy.uintp,
-                 scipy.int_, scipy.int0, scipy.int8, scipy.int16, scipy.int32, scipy.int64, scipy.intc, scipy.intp)
+        raise ArgumentError(
+            "The two input images shape do not match with 1:{} and 2:{}".format(
+                image1_data.shape, image2_data.shape
+            )
+        )
+    int_types = (
+        numpy.uint,
+        numpy.uint8,
+        numpy.uint16,
+        numpy.uint32,
+        numpy.uint64,
+        numpy.uintc,
+        numpy.uintp,
+        numpy.int_,
+        numpy.int8,
+        numpy.int16,
+        numpy.int32,
+        numpy.int64,
+        numpy.intc,
+        numpy.intp,
+    )
     if image1_data.dtype not in int_types:
-        raise ArgumentError('Input image 1 is of type {}, an int type is required.'.format(image1_data.dtype))
+        raise ArgumentError(
+            "Input image 1 is of type {}, an int type is required.".format(
+                image1_data.dtype
+            )
+        )
     if image2_data.dtype not in int_types:
-        raise ArgumentError('Input image 2 is of type {}, an int type is required.'.format(image2_data.dtype))
-    if 4294967295 < abs(image1_data.min()) + image1_data.max() + abs(image2_data.min()) + image2_data.max():
-        raise ArgumentError('The input images contain so many (or not consecutive) labels, that they will not fit in a uint32 range.')
-        
+        raise ArgumentError(
+            "Input image 2 is of type {}, an int type is required.".format(
+                image2_data.dtype
+            )
+        )
+    if (
+        4294967295
+        < abs(image1_data.min())
+        + image1_data.max()
+        + abs(image2_data.min())
+        + image2_data.max()
+    ):
+        raise ArgumentError(
+            "The input images contain so many (or not consecutive) labels, that they will not fit in a uint32 range."
+        )
+
     # create superimposition of the two label images
-    logger.info('Creating superimposition image...')
-    image_superimposition_data = scipy.zeros(image1_data.shape, dtype=scipy.uint32)
+    logger.info("Creating superimposition image...")
+    image_superimposition_data = numpy.zeros(image1_data.shape, dtype=numpy.uint32)
     translation = {}
     label_id_counter = 0
     for x in range(image1_data.shape[0]):
         for y in range(image1_data.shape[1]):
             for z in range(image1_data.shape[2]):
-                label1 = image1_data[x,y,z]
-                label2 = image2_data[x,y,z]
+                label1 = image1_data[x, y, z]
+                label2 = image2_data[x, y, z]
                 if not (label1, label2) in translation:
                     translation[(label1, label2)] = label_id_counter
                     label_id_counter += 1
-                image_superimposition_data[x,y,z] = translation[(label1, label2)]
-    
+                image_superimposition_data[x, y, z] = translation[(label1, label2)]
+
     # save resulting superimposition image
-    logger.info('Saving superimposition image as {} in the same format as input image...'.format(image_superimposition_name))
+    logger.info(
+        "Saving superimposition image as {} in the same format as input image...".format(
+            image_superimposition_name
+        )
+    )
     save(image_superimposition_data, args.output, image1_header, args.force)
-    
-    logger.info('Successfully terminated.')
-        
+
+    logger.info("Successfully terminated.")
+
+
 def getArguments(parser):
     "Provides additional validation of the arguments collected by argparse."
     return parser.parse_args()
 
+
 def getParser():
     "Creates and returns the argparse parser object."
     parser = argparse.ArgumentParser(description=__description__)
-    parser.add_argument('image1', help='The first input label image.')
-    parser.add_argument('image2', help='The second input label image.')
-    parser.add_argument('output', help='The output image.')
-    parser.add_argument('-v', dest='verbose', action='store_true', help='Display more information.')
-    parser.add_argument('-d', dest='debug', action='store_true', help='Display debug information.')
-    parser.add_argument('-f', dest='force', action='store_true', help='Silently override existing output images.')
-    
-    return parser    
-    
+    parser.add_argument("image1", help="The first input label image.")
+    parser.add_argument("image2", help="The second input label image.")
+    parser.add_argument("output", help="The output image.")
+    parser.add_argument(
+        "-v", dest="verbose", action="store_true", help="Display more information."
+    )
+    parser.add_argument(
+        "-d", dest="debug", action="store_true", help="Display debug information."
+    )
+    parser.add_argument(
+        "-f",
+        dest="force",
+        action="store_true",
+        help="Silently override existing output images.",
+    )
+
+    return parser
+
+
 if __name__ == "__main__":
-    main()        
+    main()
```

### Comparing `MedPy-0.4.0/bin/medpy_grid.py` & `MedPy-0.5.0/bin/medpy_grid.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,170 +16,246 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
-# build-in modules
-import os
 import argparse
 import logging
+
+# build-in modules
+import os
 import tempfile
 
 # third-party modules
-import scipy
-
-# path changes
+import numpy
 
 # own modules
 from medpy.core import Logger
-from medpy.io import load, save, header
+from medpy.io import header, load, save
+
+# path changes
+
 
 # information
 __author__ = "Oskar Maier"
 __version__ = "r0.1.0, 2013-06-13"
 __email__ = "oskar.maier@googlemail.com"
 __status__ = "Release"
 __description__ = """
                   Create an image volume containing a regular grid that can e.g. be used to
                   visualize deformation fields. The grid volume can be generated either by
                   supplying an example volume (-e) or by directly defining its shape (-s).
-                  
+
                   Copyright (C) 2013 Oskar Maier
                   This program comes with ABSOLUTELY NO WARRANTY; This is free software,
                   and you are welcome to redistribute it under certain conditions; see
-                  the LICENSE file or <http://www.gnu.org/licenses/> for details.   
+                  the LICENSE file or <http://www.gnu.org/licenses/> for details.
                   """
 
+
 def main():
     args = getArguments(getParser())
 
     # prepare logger
     logger = Logger.getInstance()
-    if args.debug: logger.setLevel(logging.DEBUG)
-    elif args.verbose: logger.setLevel(logging.INFO)
-    
+    if args.debug:
+        logger.setLevel(logging.DEBUG)
+    elif args.verbose:
+        logger.setLevel(logging.INFO)
+
     # copy the example image or generate empty image, depending on the modus
     if args.example:
-        grid_image = scipy.zeros(args.example_image.shape, scipy.bool_)
+        grid_image = numpy.zeros(args.example_image.shape, numpy.bool_)
         grid_header = args.example_header
     else:
-        grid_image = scipy.zeros(args.shape, scipy.bool_)
+        grid_image = numpy.zeros(args.shape, numpy.bool_)
         # !TODO: Find another solution for this
         # Saving and loading image once to generate a valid header
         tmp_dir = tempfile.mkdtemp()
-        tmp_image = '{}/{}'.format(tmp_dir, args.output.split('/')[-1])
+        tmp_image = "{}/{}".format(tmp_dir, args.output.split("/")[-1])
         save(grid_image, tmp_image)
         _, grid_header = load(tmp_image)
         try:
             os.remove(tmp_image)
             os.rmdir(tmp_dir)
         except Exception:
             pass
-        
+
     # set the image attributes if supplied
     if args.pixelspacing:
         header.set_pixel_spacing(grid_header, args.pixelspacing)
     if args.offset:
         header.set_offset(grid_header, args.offset)
-    
+
     # compute the right grid spacing for each dimension
     if args.real:
-        grid_spacing = [int(round(sp / float(ps))) for sp, ps in zip(args.spacing, header.get_pixel_spacing(grid_header))]
+        grid_spacing = [
+            int(round(sp / float(ps)))
+            for sp, ps in zip(args.spacing, header.get_pixel_spacing(grid_header))
+        ]
     else:
         grid_spacing = args.spacing
-        
+
     # paint the grid into the empty image volume
     for dim in range(grid_image.ndim):
-        if 0 == grid_spacing[dim]: continue # skip dimension of 0 grid spacing supplied
+        if 0 == grid_spacing[dim]:
+            continue  # skip dimension of 0 grid spacing supplied
         for offset in range(0, grid_image.shape[dim], grid_spacing[dim]):
             slicer = [slice(None)] * grid_image.ndim
             slicer[dim] = slice(offset, offset + 1)
-            grid_image[slicer] = True
-            
+            grid_image[tuple(slicer)] = True
+
     # saving resulting grid volume
     save(grid_image, args.output, grid_header, args.force)
-    
 
-def list_of_integers_or_int(string, separator=','):
+
+def list_of_integers_or_int(string, separator=","):
     if string.isdigit():
         return int(string)
     return list_of_integers(string, separator)
 
-def list_of_integers(string, separator=','):
+
+def list_of_integers(string, separator=","):
     values = string.split(separator)
-    if not scipy.all(list(map(str.isdigit, values))):
-        raise argparse.ArgumentTypeError('{} is not a "{}" separated list of integers'.format(string, separator))
+    if not numpy.all(list(map(str.isdigit, values))):
+        raise argparse.ArgumentTypeError(
+            '{} is not a "{}" separated list of integers'.format(string, separator)
+        )
     return list(map(int, values))
 
-def list_of_floats(string, separator=','):
+
+def list_of_floats(string, separator=","):
     values = string.split(separator)
     try:
         return list(map(float, values))
     except ValueError:
-        raise argparse.ArgumentTypeError('{} is not a "{}" separated list of floats'.format(string, separator))
+        raise argparse.ArgumentTypeError(
+            '{} is not a "{}" separated list of floats'.format(string, separator)
+        )
+
 
 def getArguments(parser):
     "Provides additional validation of the arguments collected by argparse."
     args = parser.parse_args()
     # get the number of dimensions in the image
     if args.example:
         args.example_image, args.example_header = load(args.example)
         dimensions = args.example_image.ndim
     else:
         dimensions = len(args.shape)
-    
+
     # check and, if required, modify the spacing argument
     if isinstance(args.spacing, int):
         args.spacing = [args.spacing] * dimensions
     elif len(args.spacing) != dimensions:
-        raise argparse.ArgumentTypeError('the grid spacing ({}) must contain the same number of elements as the output image has dimensions ({})'.format(','.join(map(str, args.spacing)), dimensions))
-    
+        raise argparse.ArgumentTypeError(
+            "the grid spacing ({}) must contain the same number of elements as the output image has dimensions ({})".format(
+                ",".join(map(str, args.spacing)), dimensions
+            )
+        )
+
     # check further arguments
     if args.offset and len(args.offset) != dimensions:
-        raise argparse.ArgumentTypeError('the offset ({}) must contain the same number of elements as the output image has dimensions ({})'.format(','.join(map(str, args.offset)), dimensions))
+        raise argparse.ArgumentTypeError(
+            "the offset ({}) must contain the same number of elements as the output image has dimensions ({})".format(
+                ",".join(map(str, args.offset)), dimensions
+            )
+        )
     if args.pixelspacing and len(args.pixelspacing) != dimensions:
-        raise argparse.ArgumentTypeError('the supplied pixel spacing ({}) must contain the same number of elements as the output image has dimensions ({})'.format(','.join(map(str, args.pixelspacing)), dimensions))
-    
+        raise argparse.ArgumentTypeError(
+            "the supplied pixel spacing ({}) must contain the same number of elements as the output image has dimensions ({})".format(
+                ",".join(map(str, args.pixelspacing)), dimensions
+            )
+        )
+
     return args
 
+
 def getParser():
     "Creates and returns the argparse parser object."
     # text
-    epilog ="""
+    epilog = """
 examples:
   %(prog)s -e example.nii grid.nii 10
       Generates an empty image with the same attributes as example.nii, overlays it
       with a regular grid of width 10 voxels and saves it as grid.nii.
   %(prog)s -e example.nii grid.nii 10,11,12 -r
       Same as above, but with an irregular grid and using real world coordinates
       (i.e. taking the voxel spacing of the image into account).
-  %(prog)s -s 100,200 grid.nii 10,2 -p 0.5,3 
+  %(prog)s -s 100,200 grid.nii 10,2 -p 0.5,3
       Generates a 10x2 spaced grid in a 100x200 image with a voxel spacing of 0.5x3.
-  %(prog)s -s 100,100,50 grid.nii 5,5,0 
+  %(prog)s -s 100,100,50 grid.nii 5,5,0
       Generates a 100x100x50 3D volume but fills it only with a regular 5x5 2D grid
-      over the first two dimensions.  
+      over the first two dimensions.
 """
-    
+
     # command line argument parser
-    parser = argparse.ArgumentParser(formatter_class=argparse.RawDescriptionHelpFormatter, 
-                                     description=__description__, epilog=epilog)
-    parser.add_argument('output', help='Generated grid volume.')
-    parser.add_argument('spacing', type=list_of_integers_or_int, help='The grid spacing. Can be a single digit for regular spacing in all dimensions or a colon-separated list of N integers, where N is the number of dimension in the generated volume. To skip the grid in one dimension, simply supply a 0 for it.')
-    
+    parser = argparse.ArgumentParser(
+        formatter_class=argparse.RawDescriptionHelpFormatter,
+        description=__description__,
+        epilog=epilog,
+    )
+    parser.add_argument("output", help="Generated grid volume.")
+    parser.add_argument(
+        "spacing",
+        type=list_of_integers_or_int,
+        help="The grid spacing. Can be a single digit for regular spacing in all dimensions or a colon-separated list of N integers, where N is the number of dimension in the generated volume. To skip the grid in one dimension, simply supply a 0 for it.",
+    )
+
     group = parser.add_mutually_exclusive_group(required=True)
-    group.add_argument('-e', '--example', dest='example', help='Option 1/2: Supply an image to create the grid volume by example (i.e. with same shape, voxel spacing and offset).')
-    group.add_argument('-s', '--shape', type=list_of_integers, dest='shape', help='Option 2/2: Supply a colon-separated list of integers that constitute the target volumes shape.')
-    
-    parser.add_argument('-p', '--pixel-spacing', type=list_of_floats, dest='pixelspacing', help='Set the pixel spacing of the target volume by supplying a colon-separated list of N numbers, where N is the number of dimension in the generated volume.')
-    parser.add_argument('-o', '--offset', type=list_of_floats, dest='offset', help='Set offset of the target volume by supplying a colon-separated list of N numbers, where N is the number of dimension in the generated volume.')
-
-    parser.add_argument('-r', '--real', dest='real', action='store_true', help='Spacing is given in real world coordinates, rather than voxels. For this to make a difference, either the -e switch or the -p switch must be set.')
-    
-    parser.add_argument('-v', dest='verbose', action='store_true', help='Display more information.')
-    parser.add_argument('-d', dest='debug', action='store_true', help='Display debug information.')
-    parser.add_argument('-f', '--force', dest='force', action='store_true', help='Silently override existing output images.')
-    return parser 
+    group.add_argument(
+        "-e",
+        "--example",
+        dest="example",
+        help="Option 1/2: Supply an image to create the grid volume by example (i.e. with same shape, voxel spacing and offset).",
+    )
+    group.add_argument(
+        "-s",
+        "--shape",
+        type=list_of_integers,
+        dest="shape",
+        help="Option 2/2: Supply a colon-separated list of integers that constitute the target volumes shape.",
+    )
+
+    parser.add_argument(
+        "-p",
+        "--pixel-spacing",
+        type=list_of_floats,
+        dest="pixelspacing",
+        help="Set the pixel spacing of the target volume by supplying a colon-separated list of N numbers, where N is the number of dimension in the generated volume.",
+    )
+    parser.add_argument(
+        "-o",
+        "--offset",
+        type=list_of_floats,
+        dest="offset",
+        help="Set offset of the target volume by supplying a colon-separated list of N numbers, where N is the number of dimension in the generated volume.",
+    )
+
+    parser.add_argument(
+        "-r",
+        "--real",
+        dest="real",
+        action="store_true",
+        help="Spacing is given in real world coordinates, rather than voxels. For this to make a difference, either the -e switch or the -p switch must be set.",
+    )
+
+    parser.add_argument(
+        "-v", dest="verbose", action="store_true", help="Display more information."
+    )
+    parser.add_argument(
+        "-d", dest="debug", action="store_true", help="Display debug information."
+    )
+    parser.add_argument(
+        "-f",
+        "--force",
+        dest="force",
+        action="store_true",
+        help="Silently override existing output images.",
+    )
+    return parser
+
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `MedPy-0.4.0/bin/medpy_reslice_3d_to_4d.py` & `MedPy-0.5.0/bin/medpy_reslice_3d_to_4d.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,107 +20,140 @@
 """
 
 # build-in modules
 import argparse
 import logging
 
 # third-party modules
-import scipy
-
-# path changes
+import numpy
 
 # own modules
 from medpy.core import Logger
-from medpy.io import load, save
 from medpy.core.exceptions import ArgumentError
+from medpy.io import load, save
+
+# path changes
 
 
 # information
 __author__ = "Oskar Maier"
 __version__ = "r0.1.0, 2012-05-25"
 __email__ = "oskar.maier@googlemail.com"
 __status__ = "Release"
 __description__ = """
                   Takes a a 3D volume containing 4D information and converts it into a
                   real 4D image.
                   This is achieved by taking every offset slice, starting from the first,
                   of the input 4D volume and then by combining them into a 3D volume.
                   Then repeats the process starting from the second slice, etc.
                   The new dimension will be appended to the already existing once.
-                  
+
                   A typical use case are dicom images. These often come with the time
                   dimension represented by stacking various 3D volumes on top of each
                   other in one of the spatial dimensions. These can be converted in
                   proper 4D volumes with this script.
-                  
+
                   Copyright (C) 2013 Oskar Maier
                   This program comes with ABSOLUTELY NO WARRANTY; This is free software,
                   and you are welcome to redistribute it under certain conditions; see
-                  the LICENSE file or <http://www.gnu.org/licenses/> for details.   
+                  the LICENSE file or <http://www.gnu.org/licenses/> for details.
                   """
 
+
 # code
 def main():
     args = getArguments(getParser())
 
     # prepare logger
     logger = Logger.getInstance()
-    if args.debug: logger.setLevel(logging.DEBUG)
-    elif args.verbose: logger.setLevel(logging.INFO)
-    
+    if args.debug:
+        logger.setLevel(logging.DEBUG)
+    elif args.verbose:
+        logger.setLevel(logging.INFO)
+
     # load 3d image
     data_3d, header_3d = load(args.input)
-    
+
     # check if supplied dimension parameter is inside the images dimensions
     if args.dimension >= data_3d.ndim or args.dimension < 0:
-        raise ArgumentError('The supplied cut-dimension {} exceeds the number of input volume dimensions {}.'.format(args.dimension, data_3d.ndim))
-    
+        raise ArgumentError(
+            "The supplied cut-dimension {} exceeds the number of input volume dimensions {}.".format(
+                args.dimension, data_3d.ndim
+            )
+        )
+
     # check if the supplied offset parameter is a divider of the cut-dimensions slice number
     if not 0 == data_3d.shape[args.dimension] % args.offset:
-        raise ArgumentError('The offset is not a divider of the number of slices in cut dimension ({} / {}).'.format(data_3d.shape[args.dimension], args.offset))
-        
+        raise ArgumentError(
+            "The offset is not a divider of the number of slices in cut dimension ({} / {}).".format(
+                data_3d.shape[args.dimension], args.offset
+            )
+        )
+
     # prepare empty target volume
     volumes_3d = data_3d.shape[args.dimension] / args.offset
     shape_4d = list(data_3d.shape)
     shape_4d[args.dimension] = volumes_3d
-    data_4d = scipy.zeros([args.offset] + shape_4d, dtype=data_3d.dtype)
-    
-    logger.debug('Separating {} slices into {} 3D volumes of thickness {}.'.format(data_3d.shape[args.dimension], volumes_3d, args.offset))
-        
+    data_4d = numpy.zeros([args.offset] + shape_4d, dtype=data_3d.dtype)
+
+    logger.debug(
+        "Separating {} slices into {} 3D volumes of thickness {}.".format(
+            data_3d.shape[args.dimension], volumes_3d, args.offset
+        )
+    )
+
     # iterate over 3D image and create sub volumes which are then added to the 4d volume
     for idx in range(args.offset):
         # collect the slices
         for sl in range(volumes_3d):
             idx_from = [slice(None), slice(None), slice(None)]
-            idx_from[args.dimension] = slice(idx + sl * args.offset, idx + sl * args.offset + 1)
+            idx_from[args.dimension] = slice(
+                idx + sl * args.offset, idx + sl * args.offset + 1
+            )
             idx_to = [slice(None), slice(None), slice(None)]
-            idx_to[args.dimension] = slice(sl, sl+1)
-            #print 'Slice {} to {}.'.format(idx_from, idx_to)
-            data_4d[idx][idx_to] = data_3d[idx_from]
-        
+            idx_to[args.dimension] = slice(sl, sl + 1)
+            # print 'Slice {} to {}.'.format(idx_from, idx_to)
+            data_4d[idx][tuple(idx_to)] = data_3d[tuple(idx_from)]
+
     # flip dimensions such that the newly created is the last
-    data_4d = scipy.swapaxes(data_4d, 0, args.dimension + 1)
-    data_4d = scipy.rollaxis(data_4d, 0, 4)
-        
+    data_4d = numpy.swapaxes(data_4d, 0, args.dimension + 1)
+    data_4d = numpy.rollaxis(data_4d, 0, 4)
+
     # save resulting 4D volume
     save(data_4d, args.output, header_3d, args.force)
-    
+
     logger.info("Successfully terminated.")
 
+
 def getArguments(parser):
     "Provides additional validation of the arguments collected by argparse."
     return parser.parse_args()
 
+
 def getParser():
     "Creates and returns the argparse parser object."
     parser = argparse.ArgumentParser(description=__description__)
-    parser.add_argument('input', help='Source volume.')
-    parser.add_argument('output', help='Target volume.')
-    parser.add_argument('dimension', type=int, help='The dimension in which to perform the cut (starting from 0).')
-    parser.add_argument('offset', type=int, help='The offset between the slices.')
-    parser.add_argument('-v', dest='verbose', action='store_true', help='Display more information.')
-    parser.add_argument('-d', dest='debug', action='store_true', help='Display debug information.')
-    parser.add_argument('-f', dest='force', action='store_true', help='Silently override existing output images.')
-    return parser    
+    parser.add_argument("input", help="Source volume.")
+    parser.add_argument("output", help="Target volume.")
+    parser.add_argument(
+        "dimension",
+        type=int,
+        help="The dimension in which to perform the cut (starting from 0).",
+    )
+    parser.add_argument("offset", type=int, help="The offset between the slices.")
+    parser.add_argument(
+        "-v", dest="verbose", action="store_true", help="Display more information."
+    )
+    parser.add_argument(
+        "-d", dest="debug", action="store_true", help="Display debug information."
+    )
+    parser.add_argument(
+        "-f",
+        dest="force",
+        action="store_true",
+        help="Silently override existing output images.",
+    )
+    return parser
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `MedPy-0.4.0/bin/medpy_label_count.py` & `MedPy-0.5.0/bin/medpy_label_count.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,77 +22,86 @@
 import argparse
 import logging
 import sys
 
 # third-party modules
 import numpy
 
-# path changes
+from medpy.core import Logger
 
 # own modules
 from medpy.io import load
-from medpy.core import Logger
+
+# path changes
 
 
 # information
 __author__ = "Oskar Maier"
 __version__ = "r0.2, 2011-12-13"
 __email__ = "oskar.maier@googlemail.com"
 __status__ = "Release"
 __description__ = """
                   Counts the regions in a number of label images and prints the results
                   to the stdout in csv syntax.
-                  
+
                   Copyright (C) 2013 Oskar Maier
                   This program comes with ABSOLUTELY NO WARRANTY; This is free software,
                   and you are welcome to redistribute it under certain conditions; see
-                  the LICENSE file or <http://www.gnu.org/licenses/> for details.   
+                  the LICENSE file or <http://www.gnu.org/licenses/> for details.
                   """
 
+
 # code
 def main():
     # parse cmd arguments
     parser = getParser()
     parser.parse_args()
     args = getArguments(parser)
-    
+
     # prepare logger
     logger = Logger.getInstance()
-    if args.debug: logger.setLevel(logging.DEBUG)
-    elif args.verbose: logger.setLevel(logging.INFO)
-        
+    if args.debug:
+        logger.setLevel(logging.DEBUG)
+    elif args.verbose:
+        logger.setLevel(logging.INFO)
+
     # write header line
-    print('image;labels\n')
-    
+    print("image;labels\n")
+
     # iterate over input images
     for image in args.images:
-        
         # get and prepare image data
-        logger.info('Processing image {}...'.format(image))
+        logger.info("Processing image {}...".format(image))
         image_data, _ = load(image)
-        
+
         # count number of labels and flag a warning if they reach the ushort border
-        count = len(numpy.unique(image_data)) 
-        
+        count = len(numpy.unique(image_data))
+
         # count number of labels and write
-        print('{};{}\n'.format(image.split('/')[-1], count))
-        
+        print("{};{}\n".format(image.split("/")[-1], count))
+
         sys.stdout.flush()
-            
-    logger.info('Successfully terminated.')
-      
+
+    logger.info("Successfully terminated.")
+
+
 def getArguments(parser):
     "Provides additional validation of the arguments collected by argparse."
     return parser.parse_args()
 
+
 def getParser():
     "Creates and returns the argparse parser object."
     parser = argparse.ArgumentParser(description=__description__)
-    parser.add_argument('images', nargs='+', help='One or more label images.')
-    parser.add_argument('-v', dest='verbose', action='store_true', help='Display more information.')
-    parser.add_argument('-d', dest='debug', action='store_true', help='Display debug information.')
-    
-    return parser    
-    
+    parser.add_argument("images", nargs="+", help="One or more label images.")
+    parser.add_argument(
+        "-v", dest="verbose", action="store_true", help="Display more information."
+    )
+    parser.add_argument(
+        "-d", dest="debug", action="store_true", help="Display debug information."
+    )
+
+    return parser
+
+
 if __name__ == "__main__":
-    main()            
-    
+    main()
```

### Comparing `MedPy-0.4.0/bin/medpy_extract_sub_volume.py` & `MedPy-0.5.0/bin/medpy_extract_sub_volume.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,131 +15,176 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
-# build-in modules
-from argparse import RawTextHelpFormatter
 import argparse
 import logging
-import sys
 import os
+import sys
 
-# third-party modules
-import scipy
+# build-in modules
+from argparse import RawTextHelpFormatter
 
-# path changes
+# third-party modules
+import numpy
 
 # own modules
 from medpy.core import ArgumentError, Logger
 from medpy.io import load, save
 
+# path changes
+
+
 # information
 __author__ = "Oskar Maier"
 __version__ = "r0.3.0, 2011-12-11"
 __email__ = "oskar.maier@googlemail.com"
 __status__ = "Release"
 __description__ = """
                   Takes a medical image of arbitrary dimensions and the dimensions
                   of a sub-volume that lies inside the dimensions of this images.
                   Extracts the sub-volume from the supplied image and saves it.
-                  
+
                   The volume to be extracted is defined by its slices, the syntax is the same as
                   for numpy array indexes (i.e. starting with zero-index, the first literal (x) of any
                   x:y included and the second (y) excluded).
                   E.g. '2:3,4:6' would extract the slice no. 3 in X and 5, 6 in Y direction of a 2D image.
                   E.g. '99:199,149:199,99:249' would extract the respective slices in X,Y and Z direction of a 3D image.
                        This could, for example, be used to extract the area of the liver form a CT scan.
                   To keep all slices in one direction just omit the respective value:
                   E.g. '99:199,149:199,' would work ust as example II, but extract all Z slices.
                        Note here the trailing colon.
 
                   Note to take into account the input images orientation when supplying the sub-volume.
-                  
+
                   Copyright (C) 2013 Oskar Maier
                   This program comes with ABSOLUTELY NO WARRANTY; This is free software,
                   and you are welcome to redistribute it under certain conditions; see
-                  the LICENSE file or <http://www.gnu.org/licenses/> for details.   
+                  the LICENSE file or <http://www.gnu.org/licenses/> for details.
                   """
 
+
 # code
 def main():
     # parse cmd arguments
     parser = getParser()
     parser.parse_args()
     args = getArguments(parser)
-    
+
     # prepare logger
     logger = Logger.getInstance()
-    if args.debug: logger.setLevel(logging.DEBUG)
-    elif args.verbose: logger.setLevel(logging.INFO)
-    
+    if args.debug:
+        logger.setLevel(logging.DEBUG)
+    elif args.verbose:
+        logger.setLevel(logging.INFO)
+
     # check if output image exists
     if not args.force:
         if os.path.exists(args.output + args.image[-4:]):
-            logger.warning('The output file {} already exists. Breaking.'.format(args.output + args.image[-4:]))
+            logger.warning(
+                "The output file {} already exists. Breaking.".format(
+                    args.output + args.image[-4:]
+                )
+            )
             exit(1)
-    
+
     # load images
     image_data, image_header = load(args.image)
-    
+
     # check image dimensions against sub-volume dimensions
     if len(image_data.shape) != len(args.volume):
-        logger.critical('The supplied input image is of different dimension as the sub volume requested ({} to {})'.format(len(image_data.shape), len(args.volume)))
-        raise ArgumentError('The supplied input image is of different dimension as the sub volume requested ({} to {})'.format(len(image_data.shape), len(args.volume)))
-    
-    # execute extraction of the sub-area  
-    logger.info('Extracting sub-volume...')
+        logger.critical(
+            "The supplied input image is of different dimension as the sub volume requested ({} to {})".format(
+                len(image_data.shape), len(args.volume)
+            )
+        )
+        raise ArgumentError(
+            "The supplied input image is of different dimension as the sub volume requested ({} to {})".format(
+                len(image_data.shape), len(args.volume)
+            )
+        )
+
+    # execute extraction of the sub-area
+    logger.info("Extracting sub-volume...")
     index = [slice(x[0], x[1]) for x in args.volume]
-    volume = image_data[index]
-    
+    volume = image_data[tuple(index)]
+
     # check if the output image contains data
     if 0 == len(volume):
-        logger.exception('The extracted sub-volume is of zero-size. This usual means that the supplied volume coordinates and the image coordinates do not intersect. Exiting the application.')
+        logger.exception(
+            "The extracted sub-volume is of zero-size. This usual means that the supplied volume coordinates and the image coordinates do not intersect. Exiting the application."
+        )
         sys.exit(-1)
-    
+
     # squeeze extracted sub-volume for the case in which one dimensions has been eliminated
-    volume = scipy.squeeze(volume)
-    
-    logger.debug('Extracted volume is of shape {}.'.format(volume.shape))
-    
+    volume = numpy.squeeze(volume)
+
+    logger.debug("Extracted volume is of shape {}.".format(volume.shape))
+
     # save results in same format as input image
     save(volume, args.output, image_header, args.force)
-    
-    logger.info('Successfully terminated.')
 
-    
+    logger.info("Successfully terminated.")
+
+
 def getArguments(parser):
     "Provides additional validation of the arguments collected by argparse."
     args = parser.parse_args()
     # parse volume and adapt to zero-indexing
     try:
+
         def _to_int_or_none(string):
-            if 0 == len(string): return None
+            if 0 == len(string):
+                return None
             return int(string)
-        def _to_int_or_none_double (string):
-            if 0 == len(string): return [None, None]
-            return list(map(_to_int_or_none, string.split(':')))        
-        args.volume = list(map(_to_int_or_none_double, args.volume.split(',')))
+
+        def _to_int_or_none_double(string):
+            if 0 == len(string):
+                return [None, None]
+            return list(map(_to_int_or_none, string.split(":")))
+
+        args.volume = list(map(_to_int_or_none_double, args.volume.split(",")))
         args.volume = [(x[0], x[1]) for x in args.volume]
     except (ValueError, IndexError) as e:
-        raise ArgumentError('Maleformed volume parameter "{}", see description with -h flag.'.format(args.volume), e)
+        raise ArgumentError(
+            'Maleformed volume parameter "{}", see description with -h flag.'.format(
+                args.volume
+            ),
+            e,
+        )
 
     return args
 
+
 def getParser():
     "Creates and returns the argparse parser object."
-    parser = argparse.ArgumentParser(description=__description__, formatter_class=RawTextHelpFormatter)
-    
-    parser.add_argument('image', help='The source volume.')
-    parser.add_argument('output', help='The target volume.')
-    parser.add_argument('volume', help='The coordinated of the sub-volume of the images that should be extracted.\nExample: 30:59,40:67,45:75 for a 3D image.\nSee -h for more information.')
-    parser.add_argument('-f', dest='force', action='store_true', help='Set this flag to silently override files that exist.')
-    parser.add_argument('-v', dest='verbose', action='store_true', help='Display more information.')
-    parser.add_argument('-d', dest='debug', action='store_true', help='Display debug information.')
-    
-    return parser    
-    
+    parser = argparse.ArgumentParser(
+        description=__description__, formatter_class=RawTextHelpFormatter
+    )
+
+    parser.add_argument("image", help="The source volume.")
+    parser.add_argument("output", help="The target volume.")
+    parser.add_argument(
+        "volume",
+        help="The coordinated of the sub-volume of the images that should be extracted.\nExample: 30:59,40:67,45:75 for a 3D image.\nSee -h for more information.",
+    )
+    parser.add_argument(
+        "-f",
+        dest="force",
+        action="store_true",
+        help="Set this flag to silently override files that exist.",
+    )
+    parser.add_argument(
+        "-v", dest="verbose", action="store_true", help="Display more information."
+    )
+    parser.add_argument(
+        "-d", dest="debug", action="store_true", help="Display debug information."
+    )
+
+    return parser
+
+
 if __name__ == "__main__":
-    main()    
+    main()
```

### Comparing `MedPy-0.4.0/bin/medpy_swap_dimensions.py` & `MedPy-0.5.0/bin/medpy_swap_dimensions.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,87 +20,114 @@
 """
 
 # build-in modules
 import argparse
 import logging
 
 # third-party modules
-import scipy
-
-# path changes
+import numpy
 
 # own modules
 from medpy.core import Logger
-from medpy.io import load, save, header
 from medpy.core.exceptions import ArgumentError
+from medpy.io import header, load, save
+
+# path changes
 
 
 # information
 __author__ = "Oskar Maier"
 __version__ = "r0.1.0, 2012-05-25"
 __email__ = "oskar.maier@googlemail.com"
 __status__ = "Release"
 __description__ = """
                   Two of the input images dimensions are swapped. A (200,100,10) image
                   can such be turned into a (200,10,100) one.
-                  
+
                   Copyright (C) 2013 Oskar Maier
                   This program comes with ABSOLUTELY NO WARRANTY; This is free software,
                   and you are welcome to redistribute it under certain conditions; see
-                  the LICENSE file or <http://www.gnu.org/licenses/> for details.   
+                  the LICENSE file or <http://www.gnu.org/licenses/> for details.
                   """
 
+
 # code
 def main():
     args = getArguments(getParser())
 
     # prepare logger
     logger = Logger.getInstance()
-    if args.debug: logger.setLevel(logging.DEBUG)
-    elif args.verbose: logger.setLevel(logging.INFO)
-    
+    if args.debug:
+        logger.setLevel(logging.DEBUG)
+    elif args.verbose:
+        logger.setLevel(logging.INFO)
+
     # load input image
     data_input, header_input = load(args.input)
-    
-    logger.debug('Original shape = {}.'.format(data_input.shape))
-    
+
+    logger.debug("Original shape = {}.".format(data_input.shape))
+
     # check if supplied dimension parameters is inside the images dimensions
     if args.dimension1 >= data_input.ndim or args.dimension1 < 0:
-        raise ArgumentError('The first swap-dimension {} exceeds the number of input volume dimensions {}.'.format(args.dimension1, data_input.ndim))
+        raise ArgumentError(
+            "The first swap-dimension {} exceeds the number of input volume dimensions {}.".format(
+                args.dimension1, data_input.ndim
+            )
+        )
     elif args.dimension2 >= data_input.ndim or args.dimension2 < 0:
-        raise ArgumentError('The second swap-dimension {} exceeds the number of input volume dimensions {}.'.format(args.dimension2, data_input.ndim))
-    
+        raise ArgumentError(
+            "The second swap-dimension {} exceeds the number of input volume dimensions {}.".format(
+                args.dimension2, data_input.ndim
+            )
+        )
+
     # swap axes
-    data_output = scipy.swapaxes(data_input, args.dimension1, args.dimension2)
+    data_output = numpy.swapaxes(data_input, args.dimension1, args.dimension2)
     # swap pixel spacing and offset
     ps = list(header.get_pixel_spacing(header_input))
     ps[args.dimension1], ps[args.dimension2] = ps[args.dimension2], ps[args.dimension1]
     header.set_pixel_spacing(header_input, ps)
     os = list(header.get_offset(header_input))
     os[args.dimension1], os[args.dimension2] = os[args.dimension2], os[args.dimension1]
     header.set_offset(header_input, os)
-    
-    logger.debug('Resulting shape = {}.'.format(data_output.shape))
-    
+
+    logger.debug("Resulting shape = {}.".format(data_output.shape))
+
     # save resulting volume
     save(data_output, args.output, header_input, args.force)
-    
-    logger.info("Successfully terminated.")    
-    
+
+    logger.info("Successfully terminated.")
+
+
 def getArguments(parser):
     "Provides additional validation of the arguments collected by argparse."
     return parser.parse_args()
 
+
 def getParser():
     "Creates and returns the argparse parser object."
     parser = argparse.ArgumentParser(description=__description__)
-    parser.add_argument('input', help='Source volume.')
-    parser.add_argument('output', help='Target volume.')
-    parser.add_argument('dimension1', type=int, help='First dimension to swap (starting from 0).')
-    parser.add_argument('dimension2', type=int, help='Second dimension to swap (starting from 0).')
-    parser.add_argument('-v', dest='verbose', action='store_true', help='Display more information.')
-    parser.add_argument('-d', dest='debug', action='store_true', help='Display debug information.')
-    parser.add_argument('-f', dest='force', action='store_true', help='Silently override existing output images.')
-    return parser    
+    parser.add_argument("input", help="Source volume.")
+    parser.add_argument("output", help="Target volume.")
+    parser.add_argument(
+        "dimension1", type=int, help="First dimension to swap (starting from 0)."
+    )
+    parser.add_argument(
+        "dimension2", type=int, help="Second dimension to swap (starting from 0)."
+    )
+    parser.add_argument(
+        "-v", dest="verbose", action="store_true", help="Display more information."
+    )
+    parser.add_argument(
+        "-d", dest="debug", action="store_true", help="Display debug information."
+    )
+    parser.add_argument(
+        "-f",
+        dest="force",
+        action="store_true",
+        help="Silently override existing output images.",
+    )
+    return parser
+
 
 if __name__ == "__main__":
-    main()        
+    main()
```

### Comparing `MedPy-0.4.0/bin/medpy_set_pixel_spacing.py` & `MedPy-0.5.0/bin/medpy_set_pixel_spacing.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,66 +19,78 @@
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 # build-in modules
 import argparse
 import logging
 
+# own modules
+from medpy.core import Logger
+from medpy.io import header, load, save
+
 # third-party modules
 
 # path changes
 
-# own modules
-from medpy.core import Logger
-from medpy.io import load, header, save
-
 
 # information
 __author__ = "Oskar Maier"
 __version__ = "r0.1.0, 2012-06-04"
 __email__ = "oskar.maier@googlemail.com"
 __status__ = "Release"
 __description__ = """
                   Change an image's pixel spacing in-place.
-                  
+
                   Copyright (C) 2013 Oskar Maier
                   This program comes with ABSOLUTELY NO WARRANTY; This is free software,
                   and you are welcome to redistribute it under certain conditions; see
-                  the LICENSE file or <http://www.gnu.org/licenses/> for details.   
+                  the LICENSE file or <http://www.gnu.org/licenses/> for details.
                   """
 
+
 # code
 def main():
     args = getArguments(getParser())
 
     # prepare logger
     logger = Logger.getInstance()
-    if args.debug: logger.setLevel(logging.DEBUG)
-    elif args.verbose: logger.setLevel(logging.INFO)
-    
+    if args.debug:
+        logger.setLevel(logging.DEBUG)
+    elif args.verbose:
+        logger.setLevel(logging.INFO)
+
     # load input
     data_input, header_input = load(args.image)
-    
+
     # change pixel spacing
-    logger.info('Setting pixel spacing along {} to {}...'.format(data_input.shape, args.spacing))
+    logger.info(
+        "Setting pixel spacing along {} to {}...".format(data_input.shape, args.spacing)
+    )
     header.set_pixel_spacing(header_input, args.spacing)
-    
+
     # save file
     save(data_input.copy(), args.image, header_input, True)
-    
-    logger.info("Successfully terminated.")    
-    
+
+    logger.info("Successfully terminated.")
+
+
 def getArguments(parser):
     "Provides additional validation of the arguments collected by argparse."
     return parser.parse_args()
 
+
 def getParser():
     "Creates and returns the argparse parser object."
     parser = argparse.ArgumentParser(description=__description__)
-    parser.add_argument('image', help='Image volume.')
-    parser.add_argument('spacing', type=float, nargs='+', help='The spacing values.')
-    parser.add_argument('-v', dest='verbose', action='store_true', help='Display more information.')
-    parser.add_argument('-d', dest='debug', action='store_true', help='Display debug information.')
-    return parser    
+    parser.add_argument("image", help="Image volume.")
+    parser.add_argument("spacing", type=float, nargs="+", help="The spacing values.")
+    parser.add_argument(
+        "-v", dest="verbose", action="store_true", help="Display more information."
+    )
+    parser.add_argument(
+        "-d", dest="debug", action="store_true", help="Display debug information."
+    )
+    return parser
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `MedPy-0.4.0/bin/medpy_dicom_to_4D.py` & `MedPy-0.5.0/bin/medpy_dicom_to_4D.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,117 +19,153 @@
 along with this program.  If not, see <http://www.gnu.org/licenses/>."""
 
 # build-in modules
 import argparse
 import logging
 
 # third-party modules
-import scipy
-
-# path changes
+import numpy
 
 # own modules
 from medpy.core import Logger
-from medpy.io import load, save
 from medpy.core.exceptions import ArgumentError
+from medpy.io import load, save
+
+# path changes
 
 
 # information
 __author__ = "Oskar Maier"
 __version__ = "d0.2.0, 2012-05-25"
 __email__ = "oskar.maier@googlemail.com"
 __status__ = "Development"
 __description__ = """
                   Takes a dicom folder, loads the contained slices and saves them as a proper 4D volume.
                   The supplied target dimension parameter determines the dimension along which to split the
                   original image and the consecutive slices parameter determines the offset after which to
                   split.
-                
+
                   A typical use-case are DICOM images, which often come with the temporal and third spatial
                   dimension stacked on top of each other.
                   Let us assume a (5000, 200, 190) 3D image. In reality this file contains a number of 50
                   volume of 100x200x190, which each represent a point in time. More concretely, always 50
                   slices of the first dimension show the transformation of a 2D image in time. Then occurs
                   a visible jump, when the view changes in space from the 50th to the 51th slice. The
                   following 50 slices are the temporal transformation of this new spatial slice and then
-                  occur another jump, and so on. 
-                
+                  occur another jump, and so on.
+
                   Calling this script with a target dimension of 0 (meaning the first dimension of the
                   image containing the 5000 slices) and a consecutive slices parameter of 50 (which is used
                   to tell how many consecutive slices belong together), will result in a 4D image of the
                   shape (100, 50, 200, 190) containing the spatial volumes separated by an additional time
                   dimension.
-                  
+
                   Copyright (C) 2013 Oskar Maier
                   This program comes with ABSOLUTELY NO WARRANTY; This is free software,
                   and you are welcome to redistribute it under certain conditions; see
-                  the LICENSE file or <http://www.gnu.org/licenses/> for details.   
+                  the LICENSE file or <http://www.gnu.org/licenses/> for details.
                   """
 
+
 # code
 def main():
     args = getArguments(getParser())
 
     # prepare logger
     logger = Logger.getInstance()
-    if args.debug: logger.setLevel(logging.DEBUG)
-    elif args.verbose: logger.setLevel(logging.INFO)
-    
+    if args.debug:
+        logger.setLevel(logging.DEBUG)
+    elif args.verbose:
+        logger.setLevel(logging.INFO)
+
     data_3d, _ = load(args.input)
-    
+
     # check parameters
     if args.dimension >= data_3d.ndim or args.dimension < 0:
-        raise ArgumentError('The image has only {} dimensions. The supplied target dimension {} exceeds this number.'.format(
-                    data_3d.ndim,
-                    args.dimension))
+        raise ArgumentError(
+            "The image has only {} dimensions. The supplied target dimension {} exceeds this number.".format(
+                data_3d.ndim, args.dimension
+            )
+        )
     if not 0 == data_3d.shape[args.dimension] % args.offset:
-        raise ArgumentError('The number of slices {} in the target dimension {} of the image shape {} is not dividable by the supplied number of consecutive slices {}.'.format(
-                    data_3d.shape[args.dimension],
-                    args.dimension,
-                    data_3d.shape,
-                    args.offset))
-    
+        raise ArgumentError(
+            "The number of slices {} in the target dimension {} of the image shape {} is not dividable by the supplied number of consecutive slices {}.".format(
+                data_3d.shape[args.dimension],
+                args.dimension,
+                data_3d.shape,
+                args.offset,
+            )
+        )
+
     # prepare empty target volume
     volumes_3d = data_3d.shape[args.dimension] / args.offset
     shape_4d = list(data_3d.shape)
     shape_4d[args.dimension] = volumes_3d
-    data_4d = scipy.zeros([args.offset] + shape_4d, dtype=data_3d.dtype)
-    
-    logger.debug('Separating {} slices into {} 3D volumes of thickness {}.'.format(data_3d.shape[args.dimension], volumes_3d, args.offset))
-        
+    data_4d = numpy.zeros([args.offset] + shape_4d, dtype=data_3d.dtype)
+
+    logger.debug(
+        "Separating {} slices into {} 3D volumes of thickness {}.".format(
+            data_3d.shape[args.dimension], volumes_3d, args.offset
+        )
+    )
+
     # iterate over 3D image and create sub volumes which are then added to the 4d volume
     for idx in range(args.offset):
         # collect the slices
         for sl in range(volumes_3d):
             idx_from = [slice(None), slice(None), slice(None)]
-            idx_from[args.dimension] = slice(idx + sl * args.offset, idx + sl * args.offset + 1)
+            idx_from[args.dimension] = slice(
+                idx + sl * args.offset, idx + sl * args.offset + 1
+            )
             idx_to = [slice(None), slice(None), slice(None)]
-            idx_to[args.dimension] = slice(sl, sl+1)
-            #print 'Slice {} to {}.'.format(idx_from, idx_to)
-            data_4d[idx][idx_to] = data_3d[idx_from]
-        
+            idx_to[args.dimension] = slice(sl, sl + 1)
+            # print 'Slice {} to {}.'.format(idx_from, idx_to)
+            data_4d[idx][tuple(idx_to)] = data_3d[tuple(idx_from)]
+
     # flip dimensions such that the newly created is the last
-    data_4d = scipy.swapaxes(data_4d, 0, 3)
-        
+    data_4d = numpy.swapaxes(data_4d, 0, 3)
+
     # save resulting 4D volume
     save(data_4d, args.output, False, args.force)
-    
+
     logger.info("Successfully terminated.")
 
+
 def getArguments(parser):
     "Provides additional validation of the arguments collected by argparse."
     return parser.parse_args()
 
+
 def getParser():
     "Creates and returns the argparse parser object."
-    parser = argparse.ArgumentParser(description=__description__, formatter_class=argparse.RawTextHelpFormatter)
-    parser.add_argument('input', help='Source directory.')
-    parser.add_argument('output', help='Target volume.')
-    parser.add_argument('dimension', type=int, help='The dimension in which to perform the cut (starting from 0).')
-    parser.add_argument('offset', type=int, help='How many consecutive slices belong together before a shift occurs. / The offset between the volumes.')
-    parser.add_argument('-v', dest='verbose', action='store_true', help='Display more information.')
-    parser.add_argument('-d', dest='debug', action='store_true', help='Display debug information.')
-    parser.add_argument('-f', dest='force', action='store_true', help='Silently override existing output images.')
-    return parser    
+    parser = argparse.ArgumentParser(
+        description=__description__, formatter_class=argparse.RawTextHelpFormatter
+    )
+    parser.add_argument("input", help="Source directory.")
+    parser.add_argument("output", help="Target volume.")
+    parser.add_argument(
+        "dimension",
+        type=int,
+        help="The dimension in which to perform the cut (starting from 0).",
+    )
+    parser.add_argument(
+        "offset",
+        type=int,
+        help="How many consecutive slices belong together before a shift occurs. / The offset between the volumes.",
+    )
+    parser.add_argument(
+        "-v", dest="verbose", action="store_true", help="Display more information."
+    )
+    parser.add_argument(
+        "-d", dest="debug", action="store_true", help="Display debug information."
+    )
+    parser.add_argument(
+        "-f",
+        dest="force",
+        action="store_true",
+        help="Silently override existing output images.",
+    )
+    return parser
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `MedPy-0.4.0/bin/medpy_convert.py` & `MedPy-0.5.0/bin/medpy_dicom_slices_to_volume.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,86 +1,105 @@
 #!/usr/bin/env python
 
 """
-Convert an image from one format into another.
+Converts a collection of DICOM slices into a proper image volume.
 
 Copyright (C) 2013 Oskar Maier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
+along with this program.  If not, see <http://www.gnu.org/licenses/>."""
 
 # build-in modules
 import argparse
 import logging
 
-# third-party modules
-
-# path changes
-
 # own modules
 from medpy.core import Logger
 from medpy.io import load, save
 
+# third-party modules
+
+# path changes
+
 
 # information
 __author__ = "Oskar Maier"
-__version__ = "r0.1.1, 2012-05-25"
+__version__ = "r0.2.1, 2012-06-13"
 __email__ = "oskar.maier@googlemail.com"
 __status__ = "Release"
 __description__ = """
-                  Convert an image from one format into another. The image type is
-                  determined by the file suffixes.
-                  
+                  Converts a collection of DICOM slices (a DICOM series) into a proper
+                  image volume. Note that this operation does not preserve header
+                  information.
+
                   Copyright (C) 2013 Oskar Maier
                   This program comes with ABSOLUTELY NO WARRANTY; This is free software,
                   and you are welcome to redistribute it under certain conditions; see
-                  the LICENSE file or <http://www.gnu.org/licenses/> for details.   
+                  the LICENSE file or <http://www.gnu.org/licenses/> for details.
                   """
 
+
 # code
 def main():
     args = getArguments(getParser())
 
     # prepare logger
     logger = Logger.getInstance()
-    if args.debug: logger.setLevel(logging.DEBUG)
-    elif args.verbose: logger.setLevel(logging.INFO)
-    
-    # load input image
-    data_input, header_input = load(args.input)
-    
-    # eventually empty data
-    if args.empty: data_input.fill(False)
+    if args.debug:
+        logger.setLevel(logging.DEBUG)
+    elif args.verbose:
+        logger.setLevel(logging.INFO)
+
+    img, hdr = load(args.input)
+
+    if args.spacing:
+        print("{}".format(hdr.get_voxel_spacing()))
+        return 0
+
+    logger.debug("Resulting shape is {}.".format(img.shape))
 
     # save resulting volume
-    save(data_input, args.output, header_input, args.force)
-    
-    logger.info("Successfully terminated.")    
-    
+    save(img, args.output, hdr, args.force)
+
+    logger.info("Successfully terminated.")
+
+
 def getArguments(parser):
     "Provides additional validation of the arguments collected by argparse."
     return parser.parse_args()
 
+
 def getParser():
     "Creates and returns the argparse parser object."
     parser = argparse.ArgumentParser(description=__description__)
-    parser.add_argument('input', help='Source volume.')
-    parser.add_argument('output', help='Target volume.')
-    parser.add_argument('-e', dest='empty', action='store_true', help='Instead of copying the voxel data, create an empty copy conserving all meta-data if possible.')
-    parser.add_argument('-v', dest='verbose', action='store_true', help='Display more information.')
-    parser.add_argument('-d', dest='debug', action='store_true', help='Display debug information.')
-    parser.add_argument('-f', dest='force', action='store_true', help='Silently override existing output images.')
-    return parser    
+    parser.add_argument("input", help="Source folder.")
+    parser.add_argument("output", help="Target volume.")
+    parser.add_argument(
+        "-s", dest="spacing", action="store_true", help="Just print spacing and exit."
+    )
+    parser.add_argument(
+        "-v", dest="verbose", action="store_true", help="Display more information."
+    )
+    parser.add_argument(
+        "-d", dest="debug", action="store_true", help="Display debug information."
+    )
+    parser.add_argument(
+        "-f",
+        dest="force",
+        action="store_true",
+        help="Silently override existing output images.",
+    )
+    return parser
+
 
 if __name__ == "__main__":
-    main()        
+    main()
```

### Comparing `MedPy-0.4.0/bin/medpy_join_xd_to_xplus1d.py` & `MedPy-0.5.0/bin/medpy_join_xd_to_xplus1d.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,107 +17,161 @@
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 # build-in modules
 import argparse
-from argparse import RawTextHelpFormatter
 import logging
+from argparse import RawTextHelpFormatter
 
 # third-party modules
-import scipy
-
-# path changes
+import numpy
 
-# own modules
-from medpy.io import load, save, header
 from medpy.core import Logger
 from medpy.core.exceptions import ArgumentError
 
+# own modules
+from medpy.io import header, load, save
+
+# path changes
+
 
 # information
 __author__ = "Oskar Maier"
 __version__ = "r0.1.3, 2012-05-25"
 __email__ = "oskar.maier@googlemail.com"
 __status__ = "Release"
 __description__ = """
                   Joins a number of XD volumes into a (X+1)D volume.
-                  
+
                   One common use is when a number of 3D volumes, each representing a
                   moment in time, are availabel. With this script they can be joined
                   into a proper 4D volume.
-                  
+
                   Copyright (C) 2013 Oskar Maier
                   This program comes with ABSOLUTELY NO WARRANTY; This is free software,
                   and you are welcome to redistribute it under certain conditions; see
-                  the LICENSE file or <http://www.gnu.org/licenses/> for details.   
+                  the LICENSE file or <http://www.gnu.org/licenses/> for details.
                   """
 
+
 # code
 def main():
     # parse cmd arguments
     parser = getParser()
     parser.parse_args()
     args = getArguments(parser)
-    
+
     # prepare logger
     logger = Logger.getInstance()
-    if args.debug: logger.setLevel(logging.DEBUG)
-    elif args.verbose: logger.setLevel(logging.INFO)
-    
-    # load first input image as example 
+    if args.debug:
+        logger.setLevel(logging.DEBUG)
+    elif args.verbose:
+        logger.setLevel(logging.INFO)
+
+    # load first input image as example
     example_data, example_header = load(args.inputs[0])
-    
+
     # test if the supplied position is valid
     if args.position > example_data.ndim or args.position < 0:
-        raise ArgumentError('The supplied position for the new dimension is invalid. It has to be between 0 and {}.'.format(example_data.ndim))
-    
+        raise ArgumentError(
+            "The supplied position for the new dimension is invalid. It has to be between 0 and {}.".format(
+                example_data.ndim
+            )
+        )
+
     # prepare empty output volume
-    output_data = scipy.zeros([len(args.inputs)] + list(example_data.shape), dtype=example_data.dtype)
-    
+    output_data = numpy.zeros(
+        [len(args.inputs)] + list(example_data.shape), dtype=example_data.dtype
+    )
+
     # add first image to output volume
     output_data[0] = example_data
-    
+
     # load input images and add to output volume
     for idx, image in enumerate(args.inputs[1:]):
         image_data, _ = load(image)
         if not args.ignore and image_data.dtype != example_data.dtype:
-            raise ArgumentError('The dtype {} of image {} differs from the one of the first image {}, which is {}.'.format(image_data.dtype, image, args.inputs[0], example_data.dtype))
+            raise ArgumentError(
+                "The dtype {} of image {} differs from the one of the first image {}, which is {}.".format(
+                    image_data.dtype, image, args.inputs[0], example_data.dtype
+                )
+            )
         if image_data.shape != example_data.shape:
-            raise ArgumentError('The shape {} of image {} differs from the one of the first image {}, which is {}.'.format(image_data.shape, image, args.inputs[0], example_data.shape))
+            raise ArgumentError(
+                "The shape {} of image {} differs from the one of the first image {}, which is {}.".format(
+                    image_data.shape, image, args.inputs[0], example_data.shape
+                )
+            )
         output_data[idx + 1] = image_data
-        
+
     # move new dimension to the end or to target position
     for dim in range(output_data.ndim - 1):
-        if dim >= args.position: break
-        output_data = scipy.swapaxes(output_data, dim, dim + 1)
-        
+        if dim >= args.position:
+            break
+        output_data = numpy.swapaxes(output_data, dim, dim + 1)
+
     # set pixel spacing
     spacing = list(header.get_pixel_spacing(example_header))
-    spacing = tuple(spacing[:args.position] + [args.spacing] + spacing[args.position:])
+    spacing = tuple(
+        spacing[: args.position] + [args.spacing] + spacing[args.position :]
+    )
     example_header.set_voxel_spacing(spacing)
-    
+
     # save created volume
     save(output_data, args.output, example_header, args.force)
-        
+
     logger.info("Successfully terminated.")
-    
+
+
 def getArguments(parser):
     "Provides additional validation of the arguments collected by argparse."
     return parser.parse_args()
 
+
 def getParser():
     "Creates and returns the argparse parser object."
-    parser = argparse.ArgumentParser(description=__description__, formatter_class=RawTextHelpFormatter)
-    parser.add_argument('output', help='Target volume.')
-    parser.add_argument('inputs', nargs='+', help='Source volumes of same shape and dtype.')
-    parser.add_argument('-s', dest='spacing', type=float, default=1, help='The voxel spacing of the newly created dimension. Default is 1.')
-    parser.add_argument('-p', dest='position', type=int, default=0, help='The position where to put the new dimension starting from 0. Standard behaviour is to place it in the first position.')
-    parser.add_argument('-i', dest='ignore', action='store_true', help='Ignore if the images datatypes differ.')
-    parser.add_argument('-v', dest='verbose', action='store_true', help='Display more information.')
-    parser.add_argument('-d', dest='debug', action='store_true', help='Display debug information.')
-    parser.add_argument('-f', dest='force', action='store_true', help='Silently override existing output images.')
-    return parser    
+    parser = argparse.ArgumentParser(
+        description=__description__, formatter_class=RawTextHelpFormatter
+    )
+    parser.add_argument("output", help="Target volume.")
+    parser.add_argument(
+        "inputs", nargs="+", help="Source volumes of same shape and dtype."
+    )
+    parser.add_argument(
+        "-s",
+        dest="spacing",
+        type=float,
+        default=1,
+        help="The voxel spacing of the newly created dimension. Default is 1.",
+    )
+    parser.add_argument(
+        "-p",
+        dest="position",
+        type=int,
+        default=0,
+        help="The position where to put the new dimension starting from 0. Standard behaviour is to place it in the first position.",
+    )
+    parser.add_argument(
+        "-i",
+        dest="ignore",
+        action="store_true",
+        help="Ignore if the images datatypes differ.",
+    )
+    parser.add_argument(
+        "-v", dest="verbose", action="store_true", help="Display more information."
+    )
+    parser.add_argument(
+        "-d", dest="debug", action="store_true", help="Display debug information."
+    )
+    parser.add_argument(
+        "-f",
+        dest="force",
+        action="store_true",
+        help="Silently override existing output images.",
+    )
+    return parser
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `MedPy-0.4.0/PKG-INFO` & `MedPy-0.5.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,195 +1,204 @@
 Metadata-Version: 2.1
 Name: MedPy
-Version: 0.4.0
+Version: 0.5.0
 Summary: Medical image processing in Python
 Home-page: https://github.com/loli/medpy
 Author: Oskar Maier
 Author-email: oskar.maier@gmail.com
 License: LICENSE.txt
-Description: # MedPy
-        
-        [GitHub](https://github.com/loli/medpy/) | [Documentation](http://loli.github.io/medpy/) | [Tutorials](http://loli.github.io/medpy/) | [Issue tracker](https://github.com/loli/medpy/issues) | [Contact](oskar.maier@gmail.com)
-        
-        **MedPy** is a library and script collection for medical image processing in Python, providing basic functionalities for **reading**, **writing** and **manipulating** large images of **arbitrary dimensionality**.
-        Its main contributions are n-dimensional versions of popular **image filters**, a collection of **image feature extractors**, ready to be used with [scikit-learn](http://scikit-learn.org), and an exhaustive n-dimensional **graph-cut** package.
-        
-        * [Installation](#installation)
-        * [Getting started with the library](#getting-started-with-the-library)
-        * [Getting started with the scripts](#getting-started-with-the-scripts)
-        * [Read/write support for medical image formats](#read-write-support-for-medical-image-formats)
-        * [Requirements](#requirements)
-        * [License](#license)
-        
-        ## Installation
-        
-        ```bash
-        sudo apt-get install libboost-python-dev build-essential
-        pip3 install medpy
-        ```
-        
-        **MedPy** requires **Python 3** and officially supports Ubuntu as well as other Debian derivatives.
-        For installation instructions on other operating systems see the [documentation](http://loli.github.io/medpy/).
-        While the library itself is written purely in Python, the **graph-cut** extension comes in C++ and has it's own requirements. More details can be found in the [documentation](http://loli.github.io/medpy/).
-        
-        ### Using Python 2
-        
-        **Python 2** is no longer supported. But you can still use the older releases.
-        
-        ```bash
-        pip install medpy==0.3.0
-        ```
-        
-        ## Getting started with the library
-        
-        If you already have a medical image whose format is support (see the [documentation](http://loli.github.io/medpy/>) for details), then good.
-        Otherwise, navigate to http://www.nitrc.org/projects/inia19, click on the *Download Now* button, unpack and look for the *inia19-t1.nii* file. Open it in your favorite medical image viewer (I personally fancy [itksnap](http://www.itksnap.org)) and beware: the INIA19 primate brain atlas.
-        
-        Load the image
-        
-        ```python
-        from medpy.io import load
-        image_data, image_header = load('/path/to/image.xxx')
-        ```
-        
-        The data is stored in a numpy ndarray, the header is an object containing additional metadata, such as the voxel-spacing. Now lets take a look at some of the image metadata
-        
-        ```python
-        image_data.shape
-        ```
-        
-        `(168, 206, 128)`
-        
-        ```python
-        image_data.dtype
-        ```
-        
-        `dtype(float32)`
-        
-        And the header gives us
-        
-        ```python
-        image_header.get_voxel_spacing()
-        ```
-        
-        `(0.5, 0.5, 0.5)`
-        
-        ```python
-        image_header.get_offset()
-        ```
-        
-        `(0.0, 0.0, 0.0)`
-        
-        Now lets apply one of the **MedPy** filter, more exactly the [Otsu thresholding](https://en.wikipedia.org/wiki/Otsu%27s_method), which can be used for automatic background removal
-        
-        ```python
-        from medpy.filter import otsu
-        threshold = otsu(image_data)
-        output_data = image_data > threshold
-        ```
-        
-        And save the binary image, marking the foreground
-        
-        ```python
-        from medpy.io import save
-        save(output_data, '/path/to/otsu.xxx', image_header)
-        ```
-        
-        After taking a look at it, you might want to dive deeper with the tutorials found in the [documentation](http://loli.github.io/medpy/).
-        
-        ## Getting started with the scripts
-        
-        **MedPy** comes with a range of read-to-use commandline scripts, which are all prefixed by `medpy_`.
-        To try these examples, first get an image as described in the previous section. Now call
-        
-        ```bash
-        medpy_info.py /path/to/image.xxx
-        ```
-        
-        will give you some details about the image. With
-        
-        ```bash
-        medpy_diff.py /path/to/image1.xxx /path/to/image2.xxx
-        ```
-        
-        you can compare two image. And
-        
-        ```bash
-        medpy_anisotropic_diffusion.py /path/to/image.xxx /path/to/output.xxx
-        ```
-        
-        lets you apply an edge preserving anisotropic diffusion filter. For a list of all scripts, see the [documentation](http://loli.github.io/medpy/).
-        
-        ## Read/write support for medical image formats
-        
-        MedPy relies on SimpleITK, which enables the power of ITK for image loading and saving.
-        The supported image file formats should include at least the following. Note that not all might be supported by your machine.
-        
-        **Medical formats:**
-        
-        * ITK MetaImage (.mha/.raw, .mhd)
-        * Neuroimaging Informatics Technology Initiative (NIfTI) (.nia, .nii, .nii.gz, .hdr, .img, .img.gz)
-        * Analyze (plain, SPM99, SPM2) (.hdr/.img, .img.gz)
-        * Digital Imaging and Communications in Medicine (DICOM) (.dcm, .dicom)
-        * Digital Imaging and Communications in Medicine (DICOM) series (<directory>/)
-        * Nearly Raw Raster Data (Nrrd) (.nrrd, .nhdr) 
-        * Medical Imaging NetCDF (MINC) (.mnc, .MNC)
-        * Guys Image Processing Lab (GIPL) (.gipl, .gipl.gz)
-        
-        **Microscopy formats:**
-        
-        * Medical Research Council (MRC) (.mrc, .rec)
-        * Bio-Rad (.pic, .PIC)
-        * LSM (Zeiss) microscopy images (.tif, .TIF, .tiff, .TIFF, .lsm, .LSM)
-        * Stimulate / Signal Data (SDT) (.sdt)
-        
-        **Visualization formats:**
-        
-        * VTK images (.vtk)
-        
-        **Other formats:**
-        
-        * Portable Network Graphics (PNG) (.png, .PNG)
-        * Joint Photographic Experts Group (JPEG) (.jpg, .JPG, .jpeg, .JPEG)
-        * Tagged Image File Format (TIFF) (.tif, .TIF, .tiff, .TIFF)
-        * Windows bitmap (.bmp, .BMP)
-        * Hierarchical Data Format (HDF5) (.h5 , .hdf5 , .he5)
-        * MSX-DOS Screen-x (.ge4, .ge5)
-        
-        ## Requirements
-        
-        MedPy comes with a number of dependencies and optional functionality that can require you to install additional packages.
-        
-        ### Main dependencies
-        
-        * [scipy](http://www.scipy.org)
-        * [numpy](http://www.numpy.org)
-        * [SimpleITK](https://simpleitk.readthedocs.io)
-        
-        ### Optional functionalities
-        
-        * compilation with `max-flow/min-cut` (enables the GraphCut functionalities)
-        
-        ## License
-        
-        MedPy is distributed under the GNU General Public License, a version of which can be found in the LICENSE.txt file.
-        
 Keywords: medical image processing dicom itk insight tool kit MRI CT US graph cut max-flow min-cut
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: C++
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
+Requires-Python: >=3.5, <4
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: scipy>=1.10
+Requires-Dist: numpy>=1.24
+Requires-Dist: SimpleITK>=2.1
+Provides-Extra: dev
+Requires-Dist: pre-commit; extra == "dev"
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: hypothesis; extra == "test"
+Provides-Extra: watershed
+Requires-Dist: scikit-image; extra == "watershed"
+Provides-Extra: doc
+Requires-Dist: sphinx>=1.6; extra == "doc"
+Requires-Dist: numpydoc; extra == "doc"
+Requires-Dist: pydata-sphinx-theme; extra == "doc"
+
+# MedPy
+
+[GitHub](https://github.com/loli/medpy/) | [Documentation](http://loli.github.io/medpy/) | [Tutorials](http://loli.github.io/medpy/) | [Issue tracker](https://github.com/loli/medpy/issues)
+
+**MedPy** is a library and script collection for medical image processing in Python, providing basic functionalities for **reading**, **writing** and **manipulating** large images of **arbitrary dimensionality**.
+Its main contributions are n-dimensional versions of popular **image filters**, a collection of **image feature extractors**, ready to be used with [scikit-learn](http://scikit-learn.org), and an exhaustive n-dimensional **graph-cut** package.
+
+* [Installation](#installation)
+* [Getting started with the library](#getting-started-with-the-library)
+* [Getting started with the scripts](#getting-started-with-the-scripts)
+* [Support of medical image formats](#support-of-medical-image-formats)
+* [Requirements](#requirements)
+* [License](#license)
+
+## Installation
+
+```bash
+sudo apt-get install libboost-python-dev build-essential
+pip3 install medpy
+```
+
+**MedPy** requires **Python 3** and officially supports Ubuntu as well as other Debian derivatives.
+For installation instructions on other operating systems see the [documentation](http://loli.github.io/medpy/).
+While the library itself is written purely in Python, the **graph-cut** extension comes in C++ and has [it's own requirements](http://loli.github.io/medpy/installation/graphcutsupport.html).
+
+## Getting started with the library
+
+If you already have a medical image at hand in [one of the supported formats](http://loli.github.io/medpy/information/imageformats.html), you can use it for this introduction. If not, navigate to http://www.nitrc.org/projects/inia19, click on the *Download Now* button, unpack and look for the *inia19-t1.nii* file. Open it in your favorite medical image viewer (I personally fancy [itksnap](http://www.itksnap.org)) and beware: the INIA19 primate brain atlas.
+
+Load the image
+
+```python
+from medpy.io import load
+image_data, image_header = load('/path/to/image.xxx')
+```
+
+The data is stored in a numpy ndarray, the header is an object containing additional metadata, such as the voxel-spacing. Now lets take a look at some of the image metadata
+
+```python
+image_data.shape
+```
+
+`(168, 206, 128)`
+
+```python
+image_data.dtype
+```
+
+`dtype(float32)`
+
+And the header gives us
+
+```python
+image_header.get_voxel_spacing()
+```
+
+`(0.5, 0.5, 0.5)`
+
+```python
+image_header.get_offset()
+```
+
+`(0.0, 0.0, 0.0)`
+
+Now lets apply one of the **MedPy** filter, more exactly the [Otsu thresholding](https://en.wikipedia.org/wiki/Otsu%27s_method), which can be used for automatic background removal
+
+```python
+from medpy.filter import otsu
+threshold = otsu(image_data)
+output_data = image_data > threshold
+```
+
+And save the binary image, marking the foreground
+
+```python
+from medpy.io import save
+save(output_data, '/path/to/otsu.xxx', image_header)
+```
+
+After taking a look at it, you might want to dive deeper with the tutorials found in the [documentation](http://loli.github.io/medpy/information/commandline_tools_listing.html).
+
+## Getting started with the scripts
+
+**MedPy** comes with a range of read-to-use commandline scripts, which are all prefixed by `medpy_`.
+To try these examples, first get an image as described in the previous section. Now call
+
+```bash
+medpy_info.py /path/to/image.xxx
+```
+
+will give you some details about the image. With
+
+```bash
+medpy_diff.py /path/to/image1.xxx /path/to/image2.xxx
+```
+
+you can compare two image. And
+
+```bash
+medpy_anisotropic_diffusion.py /path/to/image.xxx /path/to/output.xxx
+```
+
+lets you apply an edge preserving anisotropic diffusion filter. For a list of all scripts, see the [documentation](http://loli.github.io/medpy/).
+
+## Support of medical image formats
+
+MedPy relies on SimpleITK, which enables the power of ITK for image loading and saving.
+The supported image file formats should include at least the following. Note that not all might be supported by your machine.
+
+**Medical formats:**
+
+* ITK MetaImage (.mha/.raw, .mhd)
+* Neuroimaging Informatics Technology Initiative (NIfTI) (.nia, .nii, .nii.gz, .hdr, .img, .img.gz)
+* Analyze (plain, SPM99, SPM2) (.hdr/.img, .img.gz)
+* Digital Imaging and Communications in Medicine (DICOM) (.dcm, .dicom)
+* Digital Imaging and Communications in Medicine (DICOM) series (<directory>/)
+* Nearly Raw Raster Data (Nrrd) (.nrrd, .nhdr)
+* Medical Imaging NetCDF (MINC) (.mnc, .MNC)
+* Guys Image Processing Lab (GIPL) (.gipl, .gipl.gz)
+
+**Microscopy formats:**
+
+* Medical Research Council (MRC) (.mrc, .rec)
+* Bio-Rad (.pic, .PIC)
+* LSM (Zeiss) microscopy images (.tif, .TIF, .tiff, .TIFF, .lsm, .LSM)
+* Stimulate / Signal Data (SDT) (.sdt)
+
+**Visualization formats:**
+
+* VTK images (.vtk)
+
+**Other formats:**
+
+* Portable Network Graphics (PNG) (.png, .PNG)
+* Joint Photographic Experts Group (JPEG) (.jpg, .JPG, .jpeg, .JPEG)
+* Tagged Image File Format (TIFF) (.tif, .TIF, .tiff, .TIFF)
+* Windows bitmap (.bmp, .BMP)
+* Hierarchical Data Format (HDF5) (.h5 , .hdf5 , .he5)
+* MSX-DOS Screen-x (.ge4, .ge5)
+
+## Requirements
+
+MedPy comes with a number of dependencies and optional functionality that can require you to install additional packages.
+
+### Main dependencies
+
+* [scipy](http://www.scipy.org)
+* [numpy](http://www.numpy.org)
+* [SimpleITK](https://simpleitk.readthedocs.io)
+
+### Optional functionalities
+
+* compilation with `max-flow/min-cut` (enables the GraphCut functionalities)
+
+## License
+
+MedPy is distributed under the GNU General Public License, a version of which can be found in the LICENSE.txt file.
```

