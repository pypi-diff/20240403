# Comparing `tmp/MedPy-0.5.0.tar.gz` & `tmp/MedPy-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MedPy-0.5.0.tar", last modified: Wed Apr  3 14:43:39 2024, max compression
+gzip compressed data, was "MedPy-0.5.1.tar", last modified: Wed Apr  3 15:52:24 2024, max compression
```

## Comparing `MedPy-0.5.0.tar` & `MedPy-0.5.1.tar`

### file list

```diff
@@ -1,111 +1,117 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:43:39.456257 MedPy-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-03 14:43:34.000000 MedPy-0.5.0/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-03 14:43:34.000000 MedPy-0.5.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-03 14:43:34.000000 MedPy-0.5.0/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:43:39.456257 MedPy-0.5.0/MedPy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7512 2024-04-03 14:43:39.000000 MedPy-0.5.0/MedPy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-04-03 14:43:39.000000 MedPy-0.5.0/MedPy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 14:43:39.000000 MedPy-0.5.0/MedPy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-03 14:43:39.000000 MedPy-0.5.0/MedPy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-03 14:43:39.000000 MedPy-0.5.0/MedPy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7512 2024-04-03 14:43:39.456257 MedPy-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-03 14:43:34.000000 MedPy-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-04-03 14:43:34.000000 MedPy-0.5.0/README_PYPI.md
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-03 14:43:34.000000 MedPy-0.5.0/RELEASE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:43:39.448257 MedPy-0.5.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4486 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_anisotropic_diffusion.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7368 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_apparent_diffusion_coefficient.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10766 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_binary_resampling.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3071 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_convert.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2984 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_create_empty_volume_by_example.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3086 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_dicom_slices_to_volume.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6511 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_dicom_to_4D.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3769 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_diff.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6209 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_extract_contour.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3669 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_extract_min_max.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6589 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_extract_sub_volume.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6149 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_extract_sub_volume_auto.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6700 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_extract_sub_volume_by_example.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4225 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_fit_into_shape.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3589 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_gradient.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7371 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_graphcut_label.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9004 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_graphcut_label_bgreduced.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8936 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_graphcut_label_w_regional.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5636 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_graphcut_label_wsplit.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8923 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_graphcut_voxel.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9151 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_grid.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3332 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_info.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10440 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_intensity_range_standardization.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4582 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_intersection.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4645 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_join_masks.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5622 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_join_xd_to_xplus1d.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3048 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_label_count.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4521 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_label_fit_to_mask.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6311 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_label_superimposition.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3361 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_merge.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5073 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_morphology.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4721 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_resample.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5650 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_reslice_3d_to_4d.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2771 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_set_pixel_spacing.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4676 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_shrink_image.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4587 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_split_xd_to_xminus1d.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5128 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_stack_sub_volumes.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4357 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_swap_dimensions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4492 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_watershed.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5514 2024-04-03 14:43:34.000000 MedPy-0.5.0/bin/medpy_zoom_image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:43:39.436257 MedPy-0.5.0/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:43:39.436257 MedPy-0.5.0/lib/maxflow/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:43:39.448257 MedPy-0.5.0/lib/maxflow/src/
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-03 14:43:34.000000 MedPy-0.5.0/lib/maxflow/src/README
--rw-r--r--   0 runner    (1001) docker     (127)     7218 2024-04-03 14:43:34.000000 MedPy-0.5.0/lib/maxflow/src/block.h
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-03 14:43:34.000000 MedPy-0.5.0/lib/maxflow/src/graph.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    20008 2024-04-03 14:43:34.000000 MedPy-0.5.0/lib/maxflow/src/graph.h
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-03 14:43:34.000000 MedPy-0.5.0/lib/maxflow/src/instances.inc
--rw-r--r--   0 runner    (1001) docker     (127)    14873 2024-04-03 14:43:34.000000 MedPy-0.5.0/lib/maxflow/src/maxflow.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-03 14:43:34.000000 MedPy-0.5.0/lib/maxflow/src/pythongraph.h
--rw-r--r--   0 runner    (1001) docker     (127)    11263 2024-04-03 14:43:34.000000 MedPy-0.5.0/lib/maxflow/src/wrapper.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:43:39.448257 MedPy-0.5.0/medpy/
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:43:39.448257 MedPy-0.5.0/medpy/core/
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/core/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:43:39.452257 MedPy-0.5.0/medpy/features/
--rw-r--r--   0 runner    (1001) docker     (127)     7493 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18892 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/features/histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)    34017 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/features/intensity.py
--rw-r--r--   0 runner    (1001) docker     (127)    12918 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/features/texture.py
--rw-r--r--   0 runner    (1001) docker     (127)     6138 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/features/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:43:39.452257 MedPy-0.5.0/medpy/filter/
--rw-r--r--   0 runner    (1001) docker     (127)    24588 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/filter/IntensityRangeStandardization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/filter/binary.py
--rw-r--r--   0 runner    (1001) docker     (127)     9622 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/filter/houghtransform.py
--rw-r--r--   0 runner    (1001) docker     (127)    19807 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/filter/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/filter/label.py
--rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/filter/noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     6120 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/filter/smoothing.py
--rw-r--r--   0 runner    (1001) docker     (127)    11284 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/filter/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:43:39.452257 MedPy-0.5.0/medpy/graphcut/
--rw-r--r--   0 runner    (1001) docker     (127)     7613 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/graphcut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19015 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/graphcut/energy_label.py
--rw-r--r--   0 runner    (1001) docker     (127)    26949 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/graphcut/energy_voxel.py
--rw-r--r--   0 runner    (1001) docker     (127)    16053 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/graphcut/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    19756 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/graphcut/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    10794 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/graphcut/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/graphcut/write.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:43:39.456257 MedPy-0.5.0/medpy/io/
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/io/header.py
--rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/io/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/io/save.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:43:39.456257 MedPy-0.5.0/medpy/metric/
--rw-r--r--   0 runner    (1001) docker     (127)     5837 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44679 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/metric/binary.py
--rw-r--r--   0 runner    (1001) docker     (127)    32470 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/metric/histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/metric/image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:43:39.456257 MedPy-0.5.0/medpy/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7217 2024-04-03 14:43:34.000000 MedPy-0.5.0/medpy/utilities/argparseu.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 14:43:39.456257 MedPy-0.5.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     8243 2024-04-03 14:43:34.000000 MedPy-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:24.469394 MedPy-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-03 15:52:19.000000 MedPy-0.5.1/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-03 15:52:19.000000 MedPy-0.5.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-03 15:52:19.000000 MedPy-0.5.1/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:24.465394 MedPy-0.5.1/MedPy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7512 2024-04-03 15:52:24.000000 MedPy-0.5.1/MedPy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-03 15:52:24.000000 MedPy-0.5.1/MedPy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 15:52:24.000000 MedPy-0.5.1/MedPy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-03 15:52:24.000000 MedPy-0.5.1/MedPy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-03 15:52:24.000000 MedPy-0.5.1/MedPy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7512 2024-04-03 15:52:24.469394 MedPy-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-03 15:52:19.000000 MedPy-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-04-03 15:52:19.000000 MedPy-0.5.1/README_PYPI.md
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-03 15:52:19.000000 MedPy-0.5.1/RELEASE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:24.457394 MedPy-0.5.1/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4486 2024-04-03 15:52:19.000000 MedPy-0.5.1/bin/medpy_anisotropic_diffusion.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7368 2024-04-03 15:52:19.000000 MedPy-0.5.1/bin/medpy_apparent_diffusion_coefficient.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10766 2024-04-03 15:52:19.000000 MedPy-0.5.1/bin/medpy_binary_resampling.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3071 2024-04-03 15:52:19.000000 MedPy-0.5.1/bin/medpy_convert.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2984 2024-04-03 15:52:19.000000 MedPy-0.5.1/bin/medpy_create_empty_volume_by_example.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3086 2024-04-03 15:52:19.000000 MedPy-0.5.1/bin/medpy_dicom_slices_to_volume.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6511 2024-04-03 15:52:19.000000 MedPy-0.5.1/bin/medpy_dicom_to_4D.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3769 2024-04-03 15:52:19.000000 MedPy-0.5.1/bin/medpy_diff.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6209 2024-04-03 15:52:19.000000 MedPy-0.5.1/bin/medpy_extract_contour.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3669 2024-04-03 15:52:19.000000 MedPy-0.5.1/bin/medpy_extract_min_max.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6589 2024-04-03 15:52:19.000000 MedPy-0.5.1/bin/medpy_extract_sub_volume.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6149 2024-04-03 15:52:19.000000 MedPy-0.5.1/bin/medpy_extract_sub_volume_auto.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6700 2024-04-03 15:52:19.000000 MedPy-0.5.1/bin/medpy_extract_sub_volume_by_example.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4225 2024-04-03 15:52:19.000000 MedPy-0.5.1/bin/medpy_fit_into_shape.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3589 2024-04-03 15:52:19.000000 MedPy-0.5.1/bin/medpy_gradient.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7371 2024-04-03 15:52:19.000000 MedPy-0.5.1/bin/medpy_graphcut_label.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9004 2024-04-03 15:52:19.000000 MedPy-0.5.1/bin/medpy_graphcut_label_bgreduced.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8936 2024-04-03 15:52:19.000000 MedPy-0.5.1/bin/medpy_graphcut_label_w_regional.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5636 2024-04-03 15:52:19.000000 MedPy-0.5.1/bin/medpy_graphcut_label_wsplit.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8923 2024-04-03 15:52:19.000000 MedPy-0.5.1/bin/medpy_graphcut_voxel.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9151 2024-04-03 15:52:19.000000 MedPy-0.5.1/bin/medpy_grid.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3332 2024-04-03 15:52:19.000000 MedPy-0.5.1/bin/medpy_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10440 2024-04-03 15:52:19.000000 MedPy-0.5.1/bin/medpy_intensity_range_standardization.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4582 2024-04-03 15:52:19.000000 MedPy-0.5.1/bin/medpy_intersection.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4645 2024-04-03 15:52:19.000000 MedPy-0.5.1/bin/medpy_join_masks.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5622 2024-04-03 15:52:19.000000 MedPy-0.5.1/bin/medpy_join_xd_to_xplus1d.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3048 2024-04-03 15:52:19.000000 MedPy-0.5.1/bin/medpy_label_count.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4521 2024-04-03 15:52:19.000000 MedPy-0.5.1/bin/medpy_label_fit_to_mask.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6311 2024-04-03 15:52:19.000000 MedPy-0.5.1/bin/medpy_label_superimposition.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3361 2024-04-03 15:52:19.000000 MedPy-0.5.1/bin/medpy_merge.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5073 2024-04-03 15:52:19.000000 MedPy-0.5.1/bin/medpy_morphology.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4721 2024-04-03 15:52:19.000000 MedPy-0.5.1/bin/medpy_resample.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5650 2024-04-03 15:52:19.000000 MedPy-0.5.1/bin/medpy_reslice_3d_to_4d.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2771 2024-04-03 15:52:19.000000 MedPy-0.5.1/bin/medpy_set_pixel_spacing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4676 2024-04-03 15:52:19.000000 MedPy-0.5.1/bin/medpy_shrink_image.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4587 2024-04-03 15:52:19.000000 MedPy-0.5.1/bin/medpy_split_xd_to_xminus1d.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5128 2024-04-03 15:52:19.000000 MedPy-0.5.1/bin/medpy_stack_sub_volumes.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4357 2024-04-03 15:52:19.000000 MedPy-0.5.1/bin/medpy_swap_dimensions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4492 2024-04-03 15:52:19.000000 MedPy-0.5.1/bin/medpy_watershed.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5514 2024-04-03 15:52:19.000000 MedPy-0.5.1/bin/medpy_zoom_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:24.449394 MedPy-0.5.1/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:24.449394 MedPy-0.5.1/lib/maxflow/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:24.461394 MedPy-0.5.1/lib/maxflow/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-03 15:52:19.000000 MedPy-0.5.1/lib/maxflow/src/README
+-rw-r--r--   0 runner    (1001) docker     (127)     7218 2024-04-03 15:52:19.000000 MedPy-0.5.1/lib/maxflow/src/block.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-03 15:52:19.000000 MedPy-0.5.1/lib/maxflow/src/graph.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    20008 2024-04-03 15:52:19.000000 MedPy-0.5.1/lib/maxflow/src/graph.h
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-03 15:52:19.000000 MedPy-0.5.1/lib/maxflow/src/instances.inc
+-rw-r--r--   0 runner    (1001) docker     (127)    14873 2024-04-03 15:52:19.000000 MedPy-0.5.1/lib/maxflow/src/maxflow.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-03 15:52:19.000000 MedPy-0.5.1/lib/maxflow/src/pythongraph.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11263 2024-04-03 15:52:19.000000 MedPy-0.5.1/lib/maxflow/src/wrapper.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:24.461394 MedPy-0.5.1/medpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-03 15:52:19.000000 MedPy-0.5.1/medpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:24.461394 MedPy-0.5.1/medpy/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-03 15:52:19.000000 MedPy-0.5.1/medpy/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-03 15:52:19.000000 MedPy-0.5.1/medpy/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-04-03 15:52:19.000000 MedPy-0.5.1/medpy/core/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:24.461394 MedPy-0.5.1/medpy/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     7493 2024-04-03 15:52:19.000000 MedPy-0.5.1/medpy/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18892 2024-04-03 15:52:19.000000 MedPy-0.5.1/medpy/features/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34017 2024-04-03 15:52:19.000000 MedPy-0.5.1/medpy/features/intensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12918 2024-04-03 15:52:19.000000 MedPy-0.5.1/medpy/features/texture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6138 2024-04-03 15:52:19.000000 MedPy-0.5.1/medpy/features/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:24.461394 MedPy-0.5.1/medpy/filter/
+-rw-r--r--   0 runner    (1001) docker     (127)    24588 2024-04-03 15:52:19.000000 MedPy-0.5.1/medpy/filter/IntensityRangeStandardization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-04-03 15:52:19.000000 MedPy-0.5.1/medpy/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-04-03 15:52:19.000000 MedPy-0.5.1/medpy/filter/binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9622 2024-04-03 15:52:19.000000 MedPy-0.5.1/medpy/filter/houghtransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19807 2024-04-03 15:52:19.000000 MedPy-0.5.1/medpy/filter/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-04-03 15:52:19.000000 MedPy-0.5.1/medpy/filter/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-04-03 15:52:19.000000 MedPy-0.5.1/medpy/filter/noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6120 2024-04-03 15:52:19.000000 MedPy-0.5.1/medpy/filter/smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11284 2024-04-03 15:52:19.000000 MedPy-0.5.1/medpy/filter/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:24.465394 MedPy-0.5.1/medpy/graphcut/
+-rw-r--r--   0 runner    (1001) docker     (127)     7613 2024-04-03 15:52:19.000000 MedPy-0.5.1/medpy/graphcut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19015 2024-04-03 15:52:19.000000 MedPy-0.5.1/medpy/graphcut/energy_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26949 2024-04-03 15:52:19.000000 MedPy-0.5.1/medpy/graphcut/energy_voxel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16053 2024-04-03 15:52:19.000000 MedPy-0.5.1/medpy/graphcut/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19756 2024-04-03 15:52:19.000000 MedPy-0.5.1/medpy/graphcut/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10794 2024-04-03 15:52:19.000000 MedPy-0.5.1/medpy/graphcut/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-03 15:52:19.000000 MedPy-0.5.1/medpy/graphcut/write.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:24.465394 MedPy-0.5.1/medpy/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-03 15:52:19.000000 MedPy-0.5.1/medpy/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-04-03 15:52:19.000000 MedPy-0.5.1/medpy/io/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-04-03 15:52:19.000000 MedPy-0.5.1/medpy/io/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-04-03 15:52:19.000000 MedPy-0.5.1/medpy/io/save.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:24.465394 MedPy-0.5.1/medpy/iterators/
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-03 15:52:19.000000 MedPy-0.5.1/medpy/iterators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26214 2024-04-03 15:52:19.000000 MedPy-0.5.1/medpy/iterators/patchwise.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:24.465394 MedPy-0.5.1/medpy/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)     5837 2024-04-03 15:52:19.000000 MedPy-0.5.1/medpy/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44679 2024-04-03 15:52:19.000000 MedPy-0.5.1/medpy/metric/binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32470 2024-04-03 15:52:19.000000 MedPy-0.5.1/medpy/metric/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-04-03 15:52:19.000000 MedPy-0.5.1/medpy/metric/image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:24.465394 MedPy-0.5.1/medpy/neighbours/
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-03 15:52:19.000000 MedPy-0.5.1/medpy/neighbours/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-04-03 15:52:19.000000 MedPy-0.5.1/medpy/neighbours/knn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:24.465394 MedPy-0.5.1/medpy/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-03 15:52:19.000000 MedPy-0.5.1/medpy/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7217 2024-04-03 15:52:19.000000 MedPy-0.5.1/medpy/utilities/argparseu.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 15:52:24.469394 MedPy-0.5.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8290 2024-04-03 15:52:19.000000 MedPy-0.5.1/setup.py
```

### Comparing `MedPy-0.5.0/CHANGES.txt` & `MedPy-0.5.1/CHANGES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-v0.5.0, 2024-04-XX -- Addressed all depreciation warnings and incompatabilities
+v0.5.1, 2024-04-03 -- Hotfixes
+v0.5.0, 2024-04-03 -- Addressed all depreciation warnings and incompatabilities
                       Updated documentation
                       Updated and fixed tests
                       Added github workflows as system
                       Introduced formatting rules and pre-commit to enforce them
                       Removed dockerfile creation files
 v0.4.0, 2018-02-XX -- Switched to Python 3: finally compatible with modern development environements
                       Switched to simple itk for image loading/saving: read dicom series, more formats, less dependencies, cleaner code, easier to maintain
```

### Comparing `MedPy-0.5.0/LICENSE.txt` & `MedPy-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/MedPy.egg-info/PKG-INFO` & `MedPy-0.5.1/MedPy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MedPy
-Version: 0.5.0
+Version: 0.5.1
 Summary: Medical image processing in Python
 Home-page: https://github.com/loli/medpy
 Author: Oskar Maier
 Author-email: oskar.maier@gmail.com
 License: LICENSE.txt
 Keywords: medical image processing dicom itk insight tool kit MRI CT US graph cut max-flow min-cut
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `MedPy-0.5.0/MedPy.egg-info/SOURCES.txt` & `MedPy-0.5.1/MedPy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -83,13 +83,17 @@
 medpy/graphcut/graph.py
 medpy/graphcut/wrapper.py
 medpy/graphcut/write.py
 medpy/io/__init__.py
 medpy/io/header.py
 medpy/io/load.py
 medpy/io/save.py
+medpy/iterators/__init__.py
+medpy/iterators/patchwise.py
 medpy/metric/__init__.py
 medpy/metric/binary.py
 medpy/metric/histogram.py
 medpy/metric/image.py
+medpy/neighbours/__init__.py
+medpy/neighbours/knn.py
 medpy/utilities/__init__.py
 medpy/utilities/argparseu.py
```

### Comparing `MedPy-0.5.0/PKG-INFO` & `MedPy-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MedPy
-Version: 0.5.0
+Version: 0.5.1
 Summary: Medical image processing in Python
 Home-page: https://github.com/loli/medpy
 Author: Oskar Maier
 Author-email: oskar.maier@gmail.com
 License: LICENSE.txt
 Keywords: medical image processing dicom itk insight tool kit MRI CT US graph cut max-flow min-cut
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `MedPy-0.5.0/README.md` & `MedPy-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/README_PYPI.md` & `MedPy-0.5.1/README_PYPI.md`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/RELEASE.md` & `MedPy-0.5.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/bin/medpy_anisotropic_diffusion.py` & `MedPy-0.5.1/bin/medpy_anisotropic_diffusion.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/bin/medpy_apparent_diffusion_coefficient.py` & `MedPy-0.5.1/bin/medpy_apparent_diffusion_coefficient.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/bin/medpy_binary_resampling.py` & `MedPy-0.5.1/bin/medpy_binary_resampling.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/bin/medpy_convert.py` & `MedPy-0.5.1/bin/medpy_convert.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/bin/medpy_create_empty_volume_by_example.py` & `MedPy-0.5.1/bin/medpy_create_empty_volume_by_example.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/bin/medpy_dicom_slices_to_volume.py` & `MedPy-0.5.1/bin/medpy_dicom_slices_to_volume.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/bin/medpy_dicom_to_4D.py` & `MedPy-0.5.1/bin/medpy_dicom_to_4D.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/bin/medpy_diff.py` & `MedPy-0.5.1/bin/medpy_diff.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/bin/medpy_extract_contour.py` & `MedPy-0.5.1/bin/medpy_extract_contour.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/bin/medpy_extract_min_max.py` & `MedPy-0.5.1/bin/medpy_extract_min_max.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/bin/medpy_extract_sub_volume.py` & `MedPy-0.5.1/bin/medpy_extract_sub_volume.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/bin/medpy_extract_sub_volume_auto.py` & `MedPy-0.5.1/bin/medpy_extract_sub_volume_auto.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/bin/medpy_extract_sub_volume_by_example.py` & `MedPy-0.5.1/bin/medpy_extract_sub_volume_by_example.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/bin/medpy_fit_into_shape.py` & `MedPy-0.5.1/bin/medpy_fit_into_shape.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/bin/medpy_gradient.py` & `MedPy-0.5.1/bin/medpy_gradient.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/bin/medpy_graphcut_label.py` & `MedPy-0.5.1/bin/medpy_graphcut_label.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/bin/medpy_graphcut_label_bgreduced.py` & `MedPy-0.5.1/bin/medpy_graphcut_label_bgreduced.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/bin/medpy_graphcut_label_w_regional.py` & `MedPy-0.5.1/bin/medpy_graphcut_label_w_regional.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/bin/medpy_graphcut_label_wsplit.py` & `MedPy-0.5.1/bin/medpy_graphcut_label_wsplit.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/bin/medpy_graphcut_voxel.py` & `MedPy-0.5.1/bin/medpy_graphcut_voxel.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/bin/medpy_grid.py` & `MedPy-0.5.1/bin/medpy_grid.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/bin/medpy_info.py` & `MedPy-0.5.1/bin/medpy_info.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/bin/medpy_intensity_range_standardization.py` & `MedPy-0.5.1/bin/medpy_intensity_range_standardization.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/bin/medpy_intersection.py` & `MedPy-0.5.1/bin/medpy_intersection.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/bin/medpy_join_masks.py` & `MedPy-0.5.1/bin/medpy_join_masks.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/bin/medpy_join_xd_to_xplus1d.py` & `MedPy-0.5.1/bin/medpy_join_xd_to_xplus1d.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/bin/medpy_label_count.py` & `MedPy-0.5.1/bin/medpy_label_count.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/bin/medpy_label_fit_to_mask.py` & `MedPy-0.5.1/bin/medpy_label_fit_to_mask.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/bin/medpy_label_superimposition.py` & `MedPy-0.5.1/bin/medpy_label_superimposition.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/bin/medpy_merge.py` & `MedPy-0.5.1/bin/medpy_merge.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/bin/medpy_morphology.py` & `MedPy-0.5.1/bin/medpy_morphology.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/bin/medpy_resample.py` & `MedPy-0.5.1/bin/medpy_resample.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/bin/medpy_reslice_3d_to_4d.py` & `MedPy-0.5.1/bin/medpy_reslice_3d_to_4d.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/bin/medpy_set_pixel_spacing.py` & `MedPy-0.5.1/bin/medpy_set_pixel_spacing.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/bin/medpy_shrink_image.py` & `MedPy-0.5.1/bin/medpy_shrink_image.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/bin/medpy_split_xd_to_xminus1d.py` & `MedPy-0.5.1/bin/medpy_split_xd_to_xminus1d.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/bin/medpy_stack_sub_volumes.py` & `MedPy-0.5.1/bin/medpy_stack_sub_volumes.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/bin/medpy_swap_dimensions.py` & `MedPy-0.5.1/bin/medpy_swap_dimensions.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/bin/medpy_watershed.py` & `MedPy-0.5.1/bin/medpy_watershed.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/bin/medpy_zoom_image.py` & `MedPy-0.5.1/bin/medpy_zoom_image.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/lib/maxflow/src/README` & `MedPy-0.5.1/lib/maxflow/src/README`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/lib/maxflow/src/block.h` & `MedPy-0.5.1/lib/maxflow/src/block.h`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/lib/maxflow/src/graph.cpp` & `MedPy-0.5.1/lib/maxflow/src/graph.cpp`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/lib/maxflow/src/graph.h` & `MedPy-0.5.1/lib/maxflow/src/graph.h`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/lib/maxflow/src/maxflow.cpp` & `MedPy-0.5.1/lib/maxflow/src/maxflow.cpp`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/lib/maxflow/src/pythongraph.h` & `MedPy-0.5.1/lib/maxflow/src/pythongraph.h`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/lib/maxflow/src/wrapper.cpp` & `MedPy-0.5.1/lib/maxflow/src/wrapper.cpp`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/medpy/__init__.py` & `MedPy-0.5.1/medpy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,8 +19,9 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
-__version__ = "0.5.0"
+
+__version__ = "0.5.1"
```

### Comparing `MedPy-0.5.0/medpy/core/__init__.py` & `MedPy-0.5.1/medpy/core/__init__.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/medpy/core/exceptions.py` & `MedPy-0.5.1/medpy/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/medpy/core/logger.py` & `MedPy-0.5.1/medpy/core/logger.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/medpy/features/__init__.py` & `MedPy-0.5.1/medpy/features/__init__.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/medpy/features/histogram.py` & `MedPy-0.5.1/medpy/features/histogram.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/medpy/features/intensity.py` & `MedPy-0.5.1/medpy/features/intensity.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/medpy/features/texture.py` & `MedPy-0.5.1/medpy/features/texture.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/medpy/features/utilities.py` & `MedPy-0.5.1/medpy/features/utilities.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/medpy/filter/IntensityRangeStandardization.py` & `MedPy-0.5.1/medpy/filter/IntensityRangeStandardization.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/medpy/filter/__init__.py` & `MedPy-0.5.1/medpy/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/medpy/filter/binary.py` & `MedPy-0.5.1/medpy/filter/binary.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/medpy/filter/houghtransform.py` & `MedPy-0.5.1/medpy/filter/houghtransform.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/medpy/filter/image.py` & `MedPy-0.5.1/medpy/filter/image.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/medpy/filter/label.py` & `MedPy-0.5.1/medpy/filter/label.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/medpy/filter/noise.py` & `MedPy-0.5.1/medpy/filter/noise.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/medpy/filter/smoothing.py` & `MedPy-0.5.1/medpy/filter/smoothing.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/medpy/filter/utilities.py` & `MedPy-0.5.1/medpy/filter/utilities.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/medpy/graphcut/__init__.py` & `MedPy-0.5.1/medpy/graphcut/__init__.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/medpy/graphcut/energy_label.py` & `MedPy-0.5.1/medpy/graphcut/energy_label.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/medpy/graphcut/energy_voxel.py` & `MedPy-0.5.1/medpy/graphcut/energy_voxel.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/medpy/graphcut/generate.py` & `MedPy-0.5.1/medpy/graphcut/generate.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/medpy/graphcut/graph.py` & `MedPy-0.5.1/medpy/graphcut/graph.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/medpy/graphcut/wrapper.py` & `MedPy-0.5.1/medpy/graphcut/wrapper.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/medpy/graphcut/write.py` & `MedPy-0.5.1/medpy/graphcut/write.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/medpy/io/__init__.py` & `MedPy-0.5.1/medpy/io/__init__.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/medpy/io/header.py` & `MedPy-0.5.1/medpy/io/header.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/medpy/io/load.py` & `MedPy-0.5.1/medpy/io/load.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/medpy/io/save.py` & `MedPy-0.5.1/medpy/io/save.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/medpy/metric/__init__.py` & `MedPy-0.5.1/medpy/metric/__init__.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/medpy/metric/binary.py` & `MedPy-0.5.1/medpy/metric/binary.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/medpy/metric/histogram.py` & `MedPy-0.5.1/medpy/metric/histogram.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/medpy/metric/image.py` & `MedPy-0.5.1/medpy/metric/image.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/medpy/utilities/__init__.py` & `MedPy-0.5.1/medpy/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/medpy/utilities/argparseu.py` & `MedPy-0.5.1/medpy/utilities/argparseu.py`

 * *Files identical despite different names*

### Comparing `MedPy-0.5.0/setup.py` & `MedPy-0.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,17 @@
 PACKAGES = [
     "medpy",
     "medpy.core",
     "medpy.features",
     "medpy.filter",
     "medpy.graphcut",
     "medpy.io",
+    "medpy.iterators",
     "medpy.metric",
+    "medpy.neighbours",
     "medpy.utilities",
 ]
 
 
 #### FUNCTIONS
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
@@ -132,15 +134,15 @@
         ap = ["medpy.graphcut"]
     else:
         kw = dict(cmdclass=cmdclass)
         ap = []
 
     setup(
         name="MedPy",
-        version="0.5.0",  # major.minor.micro
+        version="0.5.1",  # major.minor.micro
         description="Medical image processing in Python",
         author="Oskar Maier",
         author_email="oskar.maier@gmail.com",
         url="https://github.com/loli/medpy",
         license="LICENSE.txt",
         keywords="medical image processing dicom itk insight tool kit MRI CT US graph cut max-flow min-cut",
         long_description=read("README_PYPI.md"),
```

