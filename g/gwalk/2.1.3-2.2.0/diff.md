# Comparing `tmp/gwalk-2.1.3.tar.gz` & `tmp/gwalk-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwalk-2.1.3.tar", last modified: Mon Apr  1 18:35:04 2024, max compression
+gzip compressed data, was "gwalk-2.2.0.tar", last modified: Wed Apr  3 18:11:04 2024, max compression
```

## Comparing `gwalk-2.1.3.tar` & `gwalk-2.2.0.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 xevra     (1000) xevra     (1000)        0 2024-04-01 18:35:04.477428 gwalk-2.1.3/
--rw-r--r--   0 xevra     (1000) xevra     (1000)      339 2024-03-01 18:48:16.000000 gwalk-2.1.3/MANIFEST.in
--rw-r--r--   0 xevra     (1000) xevra     (1000)      932 2024-04-01 18:35:04.477428 gwalk-2.1.3/PKG-INFO
--rw-r--r--   0 xevra     (1000) xevra     (1000)     2029 2024-03-01 18:48:16.000000 gwalk-2.1.3/README.md
--rw-r--r--   0 xevra     (1000) xevra     (1000)       20 2024-04-01 18:35:00.000000 gwalk-2.1.3/__version__.py
--rw-r--r--   0 xevra     (1000) xevra     (1000)      515 2024-03-01 18:48:16.000000 gwalk-2.1.3/pyproject.toml
--rw-r--r--   0 xevra     (1000) xevra     (1000)       63 2024-04-01 18:35:04.481428 gwalk-2.1.3/setup.cfg
--rw-r--r--   0 xevra     (1000) xevra     (1000)     5617 2024-03-01 18:48:16.000000 gwalk-2.1.3/setup.py
-drwxr-xr-x   0 xevra     (1000) xevra     (1000)        0 2024-04-01 18:35:04.469428 gwalk-2.1.3/src/
-drwxr-xr-x   0 xevra     (1000) xevra     (1000)        0 2024-04-01 18:35:04.469428 gwalk-2.1.3/src/gwalk/
--rw-r--r--   0 xevra     (1000) xevra     (1000)      307 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/__init__.py
--rw-r--r--   0 xevra     (1000) xevra     (1000)       20 2024-04-01 18:35:00.000000 gwalk-2.1.3/src/gwalk/__version__.py
-drwxr-xr-x   0 xevra     (1000) xevra     (1000)        0 2024-04-01 18:35:04.473428 gwalk-2.1.3/src/gwalk/c_utils/
--rw-r--r--   0 xevra     (1000) xevra     (1000)     1236 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/c_utils/dbg.h
-drwxr-xr-x   0 xevra     (1000) xevra     (1000)        0 2024-04-01 18:35:04.473428 gwalk-2.1.3/src/gwalk/catalog/
--rw-r--r--   0 xevra     (1000) xevra     (1000)       23 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/catalog/__init__.py
--rw-r--r--   0 xevra     (1000) xevra     (1000)    29447 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/catalog/catalog.py
--rw-r--r--   0 xevra     (1000) xevra     (1000)    17506 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/catalog/coordinates.py
-drwxr-xr-x   0 xevra     (1000) xevra     (1000)        0 2024-04-01 18:35:04.473428 gwalk-2.1.3/src/gwalk/catalog/prior/
--rw-r--r--   0 xevra     (1000) xevra     (1000)     4574 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/catalog/prior/CIP_prior_functions.py
--rw-r--r--   0 xevra     (1000) xevra     (1000)        0 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/catalog/prior/__init__.py
--rw-r--r--   0 xevra     (1000) xevra     (1000)    11432 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/catalog/prior/callister_prior.py
--rw-r--r--   0 xevra     (1000) xevra     (1000)     4176 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/catalog/prior/prior_methods.py
--rw-r--r--   0 xevra     (1000) xevra     (1000)     5712 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/catalog/read_catalog_GWTC_1.py
--rw-r--r--   0 xevra     (1000) xevra     (1000)     3071 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/catalog/read_catalog_GWTC_2.py
--rw-r--r--   0 xevra     (1000) xevra     (1000)     3070 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/catalog/read_catalog_GWTC_2p1.py
--rw-r--r--   0 xevra     (1000) xevra     (1000)     3071 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/catalog/read_catalog_GWTC_3.py
-drwxr-xr-x   0 xevra     (1000) xevra     (1000)        0 2024-04-01 18:35:04.473428 gwalk-2.1.3/src/gwalk/density/
--rw-r--r--   0 xevra     (1000) xevra     (1000)       23 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/density/__init__.py
--rw-r--r--   0 xevra     (1000) xevra     (1000)    50044 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/density/mesh.py
-drwxr-xr-x   0 xevra     (1000) xevra     (1000)        0 2024-04-01 18:35:04.477428 gwalk-2.1.3/src/gwalk/multivariate_normal/
--rw-r--r--   0 xevra     (1000) xevra     (1000)      108 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/multivariate_normal/__init__.py
--rw-r--r--   0 xevra     (1000) xevra     (1000)    24841 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/multivariate_normal/_decomposition.c
--rw-r--r--   0 xevra     (1000) xevra     (1000)     6289 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/multivariate_normal/_mahalanobis_distance.c
--rw-r--r--   0 xevra     (1000) xevra     (1000)    25977 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/multivariate_normal/_multivariate_normal_pdf_utils.c
--rw-r--r--   0 xevra     (1000) xevra     (1000)    27446 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/multivariate_normal/bounded_multivariate_normal.py
--rw-r--r--   0 xevra     (1000) xevra     (1000)    17947 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/multivariate_normal/decomposition.py
--rw-r--r--   0 xevra     (1000) xevra     (1000)    13587 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/multivariate_normal/decomposition_numpy.py
--rw-r--r--   0 xevra     (1000) xevra     (1000)    35820 2024-04-01 18:26:38.000000 gwalk-2.1.3/src/gwalk/multivariate_normal/object.py
--rw-r--r--   0 xevra     (1000) xevra     (1000)    11599 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/multivariate_normal/pdf.py
--rw-r--r--   0 xevra     (1000) xevra     (1000)    11686 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/multivariate_normal/utils.py
--rw-r--r--   0 xevra     (1000) xevra     (1000)     6816 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/optimize_likelihood_grid.py
-drwxr-xr-x   0 xevra     (1000) xevra     (1000)        0 2024-04-01 18:35:04.477428 gwalk-2.1.3/src/gwalk/plots/
--rw-r--r--   0 xevra     (1000) xevra     (1000)        0 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/plots/__init__.py
--rw-r--r--   0 xevra     (1000) xevra     (1000)     7254 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/plots/axis.py
--rw-r--r--   0 xevra     (1000) xevra     (1000)     8166 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/plots/likelihood_corner.py
--rw-r--r--   0 xevra     (1000) xevra     (1000)     1578 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/plots/percentile_levels.py
--rw-r--r--   0 xevra     (1000) xevra     (1000)      686 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/plots/walker_plot.py
-drwxr-xr-x   0 xevra     (1000) xevra     (1000)        0 2024-04-01 18:35:04.477428 gwalk-2.1.3/src/gwalk/tools/
--rw-r--r--   0 xevra     (1000) xevra     (1000)     5546 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/tools/NAL_event_pipeline.py
--rw-r--r--   0 xevra     (1000) xevra     (1000)        0 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/tools/__init__.py
--rw-r--r--   0 xevra     (1000) xevra     (1000)     2937 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/tools/collect.py
--rw-r--r--   0 xevra     (1000) xevra     (1000)    13900 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/tools/example_script.py
--rw-r--r--   0 xevra     (1000) xevra     (1000)    13076 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/tools/fit_catalog_samples.py
--rw-r--r--   0 xevra     (1000) xevra     (1000)     1681 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/tools/fit_likelihood_grid.py
--rwxr-xr-x   0 xevra     (1000) xevra     (1000)     5595 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/tools/load_best_fits.py
--rw-r--r--   0 xevra     (1000) xevra     (1000)     4668 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/tools/plot_mesh_norm_corner.py
--rwxr-xr-x   0 xevra     (1000) xevra     (1000)     4068 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/tools/populate_nal_figures.py
--rw-r--r--   0 xevra     (1000) xevra     (1000)    11425 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/tools/test_catalog_samples.py
-drwxr-xr-x   0 xevra     (1000) xevra     (1000)        0 2024-04-01 18:35:04.477428 gwalk-2.1.3/src/gwalk/utils/
--rw-r--r--   0 xevra     (1000) xevra     (1000)        0 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/utils/__init__.py
--rw-r--r--   0 xevra     (1000) xevra     (1000)     3186 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/utils/hist.py
--rw-r--r--   0 xevra     (1000) xevra     (1000)      133 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/utils/multivariate_normal.py
-drwxr-xr-x   0 xevra     (1000) xevra     (1000)        0 2024-04-01 18:35:04.477428 gwalk-2.1.3/src/gwalk.egg-info/
--rw-r--r--   0 xevra     (1000) xevra     (1000)      932 2024-04-01 18:35:04.000000 gwalk-2.1.3/src/gwalk.egg-info/PKG-INFO
--rw-r--r--   0 xevra     (1000) xevra     (1000)     2057 2024-04-01 18:35:04.000000 gwalk-2.1.3/src/gwalk.egg-info/SOURCES.txt
--rw-r--r--   0 xevra     (1000) xevra     (1000)        1 2024-04-01 18:35:04.000000 gwalk-2.1.3/src/gwalk.egg-info/dependency_links.txt
--rw-r--r--   0 xevra     (1000) xevra     (1000)      131 2024-04-01 18:35:04.000000 gwalk-2.1.3/src/gwalk.egg-info/requires.txt
--rw-r--r--   0 xevra     (1000) xevra     (1000)        6 2024-04-01 18:35:04.000000 gwalk-2.1.3/src/gwalk.egg-info/top_level.txt
-drwxr-xr-x   0 xevra     (1000) xevra     (1000)        0 2024-04-01 18:35:04.477428 gwalk-2.1.3/tests/
--rw-r--r--   0 xevra     (1000) xevra     (1000)    13966 2024-03-01 18:48:16.000000 gwalk-2.1.3/tests/test_decomposition.py
--rw-r--r--   0 xevra     (1000) xevra     (1000)     3984 2024-03-01 18:48:16.000000 gwalk-2.1.3/tests/test_dpgmm.py
--rw-r--r--   0 xevra     (1000) xevra     (1000)     3304 2024-03-01 18:48:16.000000 gwalk-2.1.3/tests/test_grid.py
--rw-r--r--   0 xevra     (1000) xevra     (1000)     5810 2024-03-01 18:48:16.000000 gwalk-2.1.3/tests/test_kl.py
--rw-r--r--   0 xevra     (1000) xevra     (1000)     3882 2024-03-01 18:48:16.000000 gwalk-2.1.3/tests/test_maha.py
--rw-r--r--   0 xevra     (1000) xevra     (1000)    13133 2024-03-01 18:48:16.000000 gwalk-2.1.3/tests/test_object.py
--rw-r--r--   0 xevra     (1000) xevra     (1000)     4824 2024-03-01 18:48:16.000000 gwalk-2.1.3/tests/test_pdf.py
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-04-03 18:11:04.173928 gwalk-2.2.0/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)      339 2023-12-12 01:57:59.000000 gwalk-2.2.0/MANIFEST.in
+-rw-r--r--   0 vdelfave (669582709) staff       (20)      932 2024-04-03 18:11:04.173809 gwalk-2.2.0/PKG-INFO
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     2029 2022-11-15 19:49:14.000000 gwalk-2.2.0/README.md
+-rw-r--r--   0 vdelfave (669582709) staff       (20)       20 2024-04-03 18:10:57.000000 gwalk-2.2.0/__version__.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)      515 2023-08-15 23:07:31.000000 gwalk-2.2.0/pyproject.toml
+-rw-r--r--   0 vdelfave (669582709) staff       (20)       63 2024-04-03 18:11:04.174216 gwalk-2.2.0/setup.cfg
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     5617 2023-12-12 01:57:59.000000 gwalk-2.2.0/setup.py
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-04-03 18:11:04.109295 gwalk-2.2.0/src/
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-04-03 18:11:04.127414 gwalk-2.2.0/src/gwalk/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)      307 2023-04-25 18:43:04.000000 gwalk-2.2.0/src/gwalk/__init__.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)       20 2024-04-03 18:10:57.000000 gwalk-2.2.0/src/gwalk/__version__.py
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-04-03 18:11:04.130660 gwalk-2.2.0/src/gwalk/c_utils/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     1236 2023-04-25 18:43:04.000000 gwalk-2.2.0/src/gwalk/c_utils/dbg.h
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-04-03 18:11:04.132444 gwalk-2.2.0/src/gwalk/catalog/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)       23 2022-11-15 19:49:15.000000 gwalk-2.2.0/src/gwalk/catalog/__init__.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    29447 2023-05-02 15:45:34.000000 gwalk-2.2.0/src/gwalk/catalog/catalog.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    17506 2022-11-15 19:49:15.000000 gwalk-2.2.0/src/gwalk/catalog/coordinates.py
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-04-03 18:11:04.143574 gwalk-2.2.0/src/gwalk/catalog/prior/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     4574 2022-11-15 19:49:15.000000 gwalk-2.2.0/src/gwalk/catalog/prior/CIP_prior_functions.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)        0 2022-11-15 19:49:15.000000 gwalk-2.2.0/src/gwalk/catalog/prior/__init__.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    11432 2022-11-15 19:49:15.000000 gwalk-2.2.0/src/gwalk/catalog/prior/callister_prior.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     4176 2022-11-15 19:49:15.000000 gwalk-2.2.0/src/gwalk/catalog/prior/prior_methods.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     5712 2023-05-02 15:46:03.000000 gwalk-2.2.0/src/gwalk/catalog/read_catalog_GWTC_1.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     3071 2023-05-02 15:46:14.000000 gwalk-2.2.0/src/gwalk/catalog/read_catalog_GWTC_2.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     3070 2023-05-02 15:46:22.000000 gwalk-2.2.0/src/gwalk/catalog/read_catalog_GWTC_2p1.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     3071 2023-05-02 15:46:27.000000 gwalk-2.2.0/src/gwalk/catalog/read_catalog_GWTC_3.py
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-04-03 18:11:04.149861 gwalk-2.2.0/src/gwalk/density/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)       23 2022-11-15 19:49:15.000000 gwalk-2.2.0/src/gwalk/density/__init__.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    50044 2023-01-24 15:58:53.000000 gwalk-2.2.0/src/gwalk/density/mesh.py
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-04-03 18:11:04.158645 gwalk-2.2.0/src/gwalk/multivariate_normal/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)      108 2023-04-25 18:43:04.000000 gwalk-2.2.0/src/gwalk/multivariate_normal/__init__.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    24841 2023-04-25 18:43:04.000000 gwalk-2.2.0/src/gwalk/multivariate_normal/_decomposition.c
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     6289 2023-04-25 18:43:04.000000 gwalk-2.2.0/src/gwalk/multivariate_normal/_mahalanobis_distance.c
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    25977 2023-04-25 18:43:04.000000 gwalk-2.2.0/src/gwalk/multivariate_normal/_multivariate_normal_pdf_utils.c
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    27446 2023-04-25 18:43:04.000000 gwalk-2.2.0/src/gwalk/multivariate_normal/bounded_multivariate_normal.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    17947 2023-04-25 18:43:04.000000 gwalk-2.2.0/src/gwalk/multivariate_normal/decomposition.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    13587 2023-04-25 18:43:04.000000 gwalk-2.2.0/src/gwalk/multivariate_normal/decomposition_numpy.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    37193 2024-04-03 17:24:04.000000 gwalk-2.2.0/src/gwalk/multivariate_normal/object.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    11599 2023-04-25 18:43:04.000000 gwalk-2.2.0/src/gwalk/multivariate_normal/pdf.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    11805 2024-04-03 18:08:34.000000 gwalk-2.2.0/src/gwalk/multivariate_normal/utils.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     6816 2023-12-12 01:57:59.000000 gwalk-2.2.0/src/gwalk/optimize_likelihood_grid.py
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-04-03 18:11:04.159953 gwalk-2.2.0/src/gwalk/plots/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)        0 2022-11-15 19:49:15.000000 gwalk-2.2.0/src/gwalk/plots/__init__.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     7254 2022-11-15 19:49:15.000000 gwalk-2.2.0/src/gwalk/plots/axis.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     8166 2022-11-15 19:49:15.000000 gwalk-2.2.0/src/gwalk/plots/likelihood_corner.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     1578 2022-11-15 19:49:15.000000 gwalk-2.2.0/src/gwalk/plots/percentile_levels.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)      686 2022-11-15 19:49:15.000000 gwalk-2.2.0/src/gwalk/plots/walker_plot.py
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-04-03 18:11:04.164101 gwalk-2.2.0/src/gwalk/tools/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     5546 2023-01-24 15:58:53.000000 gwalk-2.2.0/src/gwalk/tools/NAL_event_pipeline.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)        0 2022-11-15 19:49:15.000000 gwalk-2.2.0/src/gwalk/tools/__init__.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     2937 2022-11-15 19:49:15.000000 gwalk-2.2.0/src/gwalk/tools/collect.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    13900 2022-11-15 19:49:15.000000 gwalk-2.2.0/src/gwalk/tools/example_script.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    13076 2023-01-24 15:58:53.000000 gwalk-2.2.0/src/gwalk/tools/fit_catalog_samples.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     1681 2023-04-25 18:43:04.000000 gwalk-2.2.0/src/gwalk/tools/fit_likelihood_grid.py
+-rwxr-xr-x   0 vdelfave (669582709) staff       (20)     5595 2022-11-15 19:49:15.000000 gwalk-2.2.0/src/gwalk/tools/load_best_fits.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     4668 2022-11-15 19:49:15.000000 gwalk-2.2.0/src/gwalk/tools/plot_mesh_norm_corner.py
+-rwxr-xr-x   0 vdelfave (669582709) staff       (20)     4068 2022-11-15 19:49:15.000000 gwalk-2.2.0/src/gwalk/tools/populate_nal_figures.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    11425 2023-01-24 15:58:53.000000 gwalk-2.2.0/src/gwalk/tools/test_catalog_samples.py
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-04-03 18:11:04.164965 gwalk-2.2.0/src/gwalk/utils/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)        0 2022-11-15 19:49:15.000000 gwalk-2.2.0/src/gwalk/utils/__init__.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     3186 2022-11-15 19:49:15.000000 gwalk-2.2.0/src/gwalk/utils/hist.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)      133 2023-04-25 18:43:04.000000 gwalk-2.2.0/src/gwalk/utils/multivariate_normal.py
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-04-03 18:11:04.173412 gwalk-2.2.0/src/gwalk.egg-info/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)      932 2024-04-03 18:11:04.000000 gwalk-2.2.0/src/gwalk.egg-info/PKG-INFO
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     2057 2024-04-03 18:11:04.000000 gwalk-2.2.0/src/gwalk.egg-info/SOURCES.txt
+-rw-r--r--   0 vdelfave (669582709) staff       (20)        1 2024-04-03 18:11:04.000000 gwalk-2.2.0/src/gwalk.egg-info/dependency_links.txt
+-rw-r--r--   0 vdelfave (669582709) staff       (20)      131 2024-04-03 18:11:04.000000 gwalk-2.2.0/src/gwalk.egg-info/requires.txt
+-rw-r--r--   0 vdelfave (669582709) staff       (20)        6 2024-04-03 18:11:04.000000 gwalk-2.2.0/src/gwalk.egg-info/top_level.txt
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-04-03 18:11:04.173072 gwalk-2.2.0/tests/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    13966 2023-04-25 18:43:04.000000 gwalk-2.2.0/tests/test_decomposition.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     3984 2023-12-12 01:57:59.000000 gwalk-2.2.0/tests/test_dpgmm.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     3304 2023-04-25 18:43:04.000000 gwalk-2.2.0/tests/test_grid.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     5810 2023-04-25 18:43:04.000000 gwalk-2.2.0/tests/test_kl.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     3882 2023-04-25 18:43:04.000000 gwalk-2.2.0/tests/test_maha.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    14181 2024-04-03 18:09:35.000000 gwalk-2.2.0/tests/test_object.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     4824 2023-04-25 18:43:04.000000 gwalk-2.2.0/tests/test_pdf.py
```

### Comparing `gwalk-2.1.3/PKG-INFO` & `gwalk-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwalk
-Version: 2.1.3
+Version: 2.2.0
 Home-page: https://gitlab.com/xevra/gwalk
 Author: Vera Del Favero
 Author-email: xevra86@gmail.com
 Maintainer: Vera Del Favero
 Maintainer-email: xevra86@gmail.com
 License: MIT Lisence
 Keywords: Gravitational Wave,Likelihood
```

### Comparing `gwalk-2.1.3/README.md` & `gwalk-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.3/pyproject.toml` & `gwalk-2.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.3/setup.py` & `gwalk-2.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.3/src/gwalk/c_utils/dbg.h` & `gwalk-2.2.0/src/gwalk/c_utils/dbg.h`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.3/src/gwalk/catalog/catalog.py` & `gwalk-2.2.0/src/gwalk/catalog/catalog.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.3/src/gwalk/catalog/coordinates.py` & `gwalk-2.2.0/src/gwalk/catalog/coordinates.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.3/src/gwalk/catalog/prior/CIP_prior_functions.py` & `gwalk-2.2.0/src/gwalk/catalog/prior/CIP_prior_functions.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.3/src/gwalk/catalog/prior/callister_prior.py` & `gwalk-2.2.0/src/gwalk/catalog/prior/callister_prior.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.3/src/gwalk/catalog/prior/prior_methods.py` & `gwalk-2.2.0/src/gwalk/catalog/prior/prior_methods.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.3/src/gwalk/catalog/read_catalog_GWTC_1.py` & `gwalk-2.2.0/src/gwalk/catalog/read_catalog_GWTC_1.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.3/src/gwalk/catalog/read_catalog_GWTC_2.py` & `gwalk-2.2.0/src/gwalk/catalog/read_catalog_GWTC_2.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.3/src/gwalk/catalog/read_catalog_GWTC_2p1.py` & `gwalk-2.2.0/src/gwalk/catalog/read_catalog_GWTC_2p1.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.3/src/gwalk/catalog/read_catalog_GWTC_3.py` & `gwalk-2.2.0/src/gwalk/catalog/read_catalog_GWTC_3.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.3/src/gwalk/density/mesh.py` & `gwalk-2.2.0/src/gwalk/density/mesh.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.3/src/gwalk/multivariate_normal/_decomposition.c` & `gwalk-2.2.0/src/gwalk/multivariate_normal/_decomposition.c`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.3/src/gwalk/multivariate_normal/_mahalanobis_distance.c` & `gwalk-2.2.0/src/gwalk/multivariate_normal/_mahalanobis_distance.c`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.3/src/gwalk/multivariate_normal/_multivariate_normal_pdf_utils.c` & `gwalk-2.2.0/src/gwalk/multivariate_normal/_multivariate_normal_pdf_utils.c`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.3/src/gwalk/multivariate_normal/bounded_multivariate_normal.py` & `gwalk-2.2.0/src/gwalk/multivariate_normal/bounded_multivariate_normal.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.3/src/gwalk/multivariate_normal/decomposition.py` & `gwalk-2.2.0/src/gwalk/multivariate_normal/decomposition.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.3/src/gwalk/multivariate_normal/decomposition_numpy.py` & `gwalk-2.2.0/src/gwalk/multivariate_normal/decomposition_numpy.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.3/src/gwalk/multivariate_normal/object.py` & `gwalk-2.2.0/src/gwalk/multivariate_normal/object.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from gwalk.multivariate_normal.pdf import pdf as multivariate_normal_pdf
 from gwalk.multivariate_normal.decomposition import nparams_of_ndim
 from gwalk.multivariate_normal.decomposition import ndim_of_nparams
 from gwalk.multivariate_normal.utils import analytic_kl_of_params
 from gwalk.multivariate_normal.utils import analytic_enclosed_integral
 
 #### Public Imports ####
-import warnings
+from warnings import warn as warning
 from xdata.database import Database
 import numpy as np
 from scipy import stats
 
 #### Globals ####
 _INV_RT2 = 1./np.sqrt(2)
 _LOG_2PI = np.log(2*np.pi)
@@ -152,19 +152,43 @@
     @std.setter
     def std(self, value):
         # Assert that std has dimensions ndim
         assert isinstance(value, np.ndarray)
         assert value.shape == (self.ndim,)
         # Check that std limits make sense
         if hasattr(self, "plimits") and not (self.plimits is None):
-            assert all(value >= self.plimits[self.ndim + 1:2*self.ndim + 1, 0])
-            assert all(value <= self.plimits[self.ndim + 1:2*self.ndim + 1, 1])
+            try:
+                # Hopefully our plimits make sense
+                assert all(value >= self.plimits[self.ndim + 1:2*self.ndim + 1, 0])
+                assert all(value <= self.plimits[self.ndim + 1:2*self.ndim + 1, 1])
+            except:
+                # Okay, hopefully our Gaussian is nonsingular
+                try:
+                    assert all(value > 0)
+                except:
+                    raise RuntimeError("Cannot have a Gaussian with negative width")
+                # That's a start. Let's check for std too big next
+                try:
+                    assert all(value <= self.plimits[self.ndim + 1:2*self.ndim + 1, 1])
+                except:
+                    warning("Setting std outside expected parameter limits, and adjusting parameter limits")
+                    self.plimits[self.ndim + 1:2*self.ndim + 1, 1] = value * self.sig_max
+                # Great. Let's check for too small
+                try:
+                    assert all(value >= self.plimits[self.ndim + 1:2*self.ndim + 1, 0])
+                except:
+                    # Well, this is really dangerous, so let's not fix this yet
+                    raise RuntimeError("Requested Gaussian width betrays parameter limits.")
+            
         self._std = value
+        # Update params
         if hasattr(self, "_params"):
             self._params[self.ndim + 1:2*self.ndim + 1] = value
+        # Update scale
+        self.scale = 1/value 
 
     #### eigvals property ####
     @property
     def eigvals(self):
         '''The eigvals of the Gaussian covariance'''
         return self._eigvals
 
@@ -625,15 +649,15 @@
         '''
         # Generate samples
         samples = np.atleast_2d(rv.rvs(size = int(size),random_state=self.rs))
         if not samples.shape[1] == self.ndim:
             raise RuntimeError("normal samples are the wrong shape")
         return samples
 
-    def sample_normal(self, size, scale=False, params=None):
+    def sample_normal(self, size, scale=None, params=None):
         '''Draw a number, size, of random samples from inside limits
 
         This introduces bias, so be careful
 
         Parameters
         ----------
         size: int
@@ -661,19 +685,23 @@
         if scale is None:
             scale = self.scale
 
         # load params
         if params is None:
             mu = self.mu
             cov = self.cov
+            cov = cov_rescale(cov, scale)
+            cov = cov.reshape((self.ndim,self.ndim))
+            limits = (self.limits - np.atleast_2d(mu).T)*np.atleast_2d(scale).T
         else:
             mu, cov = mu_cov_of_params(params)
             mu = mu.reshape((self.ndim,))
             cov = cov_rescale(cov, scale)
             cov = cov.reshape((self.ndim,self.ndim))
+            limits = (self.limits - np.atleast_2d(mu).T)*np.atleast_2d(scale).T
 
         # Initialize rv
         try:
             rv = multivariate_normal(np.zeros(self.ndim), cov)
         except RuntimeError as exp:
             from numpy.linalg import eigvals, eigvalsh
             print("Sampling failed")
@@ -694,31 +722,29 @@
             # How many samples do we still need?
             n_need = size - n_keep
             # Draw that many samples
             Xs = self.sample_normal_unconstrained(rv, n_need)
             # Check if these samples satisfy our constraints
             k_ind = np.ones((n_need,),dtype=bool)
             for i in range(self.ndim):
-                k_ind &= Xs[:,i] >= (self.limits[i,0] - mu[i]) * self.scale[i]
-                k_ind &= Xs[:,i] <= (self.limits[i,1] - mu[i]) * self.scale[i]
+                k_ind &= Xs[:,i] > limits[i,0]
+                k_ind &= Xs[:,i] < limits[i,1]
             # Identify the number of new samples to keep from this iteration
             n_it = np.sum(k_ind)
             # Keep iterating if there are not valid samples
             if n_it != 0:
                 # Keep valid samples
                 Xs = Xs[k_ind]
                 # Add them to Xkeep
                 Xk[n_keep:n_keep+n_it,:] = Xs
                 # Update n_keep
                 n_keep += n_it
 
         # Rescale if applicable
-        Xk = (Xk * self.scale) + mu
-        #if not scale:
-        #    Xk *= self.scale
+        Xk = (Xk / scale) + mu
 
         # Return samples
         return Xk
 
     #### Basic Fit Method ####
 
     def fit_simple(self, Y, w=None, assign=True):
@@ -733,17 +759,17 @@
         assign: bool, optional
             Input Assign guess to MultivariateNormal Object?
         '''
         ## Imports ##
         import numpy as np
 
         # Find the average and covariance of the samples
-        Y = Y/self.scale
         mean = np.average(Y, weights = w, axis = 0)
-        cov = np.cov(Y.T, aweights = w)
+        cov = np.cov(((Y - mean)*self.scale).T, aweights = w)
+        cov = cov_rescale(cov, self.scale**-1)
 
         # convert to a sample
         X = params_of_offset_mu_cov(self.offset, mean, cov)
 
         # Assign this guess
         if assign:
             self.params = X
```

### Comparing `gwalk-2.1.3/src/gwalk/multivariate_normal/pdf.py` & `gwalk-2.2.0/src/gwalk/multivariate_normal/pdf.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.3/src/gwalk/multivariate_normal/utils.py` & `gwalk-2.2.0/src/gwalk/multivariate_normal/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -299,15 +299,15 @@
     scale2: array like, shape = (ngauss,ndim)
         Input scale for different parameter guesses
     '''
     X1_mu, X1_cov = mu_cov_of_params(X1)
     X2_mu, X2_cov = mu_cov_of_params(X2)
     return analytic_kl(X1_mu, X1_cov, X2_mu, X2_cov, scale1=scale1, scale2=scale2)
 
-def analytic_enclosed_integral(X, limits, scale):
+def analytic_enclosed_integral(X, limits, scale=None):
     '''Compute the enclosed integral in a bounded interval
     
     Parameters
     ----------
     X: array like, shape = (ngauss, nparams)
         Input Array of parameter guesses
     limits: array like, shape = (ndim, 2)
@@ -315,14 +315,19 @@
     scale: array like, shape = (ngauss,ndim)
         Input scale for different parameter guesses
     '''
     from scipy import stats
     from gwalk.multivariate_normal.decomposition import mu_of_params
     from gwalk.multivariate_normal.decomposition import std_of_params
     from gwalk.multivariate_normal.decomposition import params_rescale
+    # Check ndim
+    ndim = limits.shape[0]
+    # Check scale
+    if scale is None:
+        scale = np.ones(ndim)
     # Protect against single set of parameters
     X = params_rescale(X, scale=scale)
     mu  = mu_of_params(X)
     sig = std_of_params(X)
     # Extract information
     ngauss, ndim = mu.shape[0], mu.shape[1]
     # Protect against single set of limits
```

### Comparing `gwalk-2.1.3/src/gwalk/optimize_likelihood_grid.py` & `gwalk-2.2.0/src/gwalk/optimize_likelihood_grid.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.3/src/gwalk/plots/axis.py` & `gwalk-2.2.0/src/gwalk/plots/axis.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.3/src/gwalk/plots/likelihood_corner.py` & `gwalk-2.2.0/src/gwalk/plots/likelihood_corner.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.3/src/gwalk/plots/percentile_levels.py` & `gwalk-2.2.0/src/gwalk/plots/percentile_levels.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.3/src/gwalk/plots/walker_plot.py` & `gwalk-2.2.0/src/gwalk/plots/walker_plot.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.3/src/gwalk/tools/NAL_event_pipeline.py` & `gwalk-2.2.0/src/gwalk/tools/NAL_event_pipeline.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.3/src/gwalk/tools/collect.py` & `gwalk-2.2.0/src/gwalk/tools/collect.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.3/src/gwalk/tools/example_script.py` & `gwalk-2.2.0/src/gwalk/tools/example_script.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.3/src/gwalk/tools/fit_catalog_samples.py` & `gwalk-2.2.0/src/gwalk/tools/fit_catalog_samples.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.3/src/gwalk/tools/fit_likelihood_grid.py` & `gwalk-2.2.0/src/gwalk/tools/fit_likelihood_grid.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.3/src/gwalk/tools/load_best_fits.py` & `gwalk-2.2.0/src/gwalk/tools/load_best_fits.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.3/src/gwalk/tools/plot_mesh_norm_corner.py` & `gwalk-2.2.0/src/gwalk/tools/plot_mesh_norm_corner.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.3/src/gwalk/tools/populate_nal_figures.py` & `gwalk-2.2.0/src/gwalk/tools/populate_nal_figures.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.3/src/gwalk/tools/test_catalog_samples.py` & `gwalk-2.2.0/src/gwalk/tools/test_catalog_samples.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.3/src/gwalk/utils/hist.py` & `gwalk-2.2.0/src/gwalk/utils/hist.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.3/src/gwalk.egg-info/PKG-INFO` & `gwalk-2.2.0/src/gwalk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwalk
-Version: 2.1.3
+Version: 2.2.0
 Home-page: https://gitlab.com/xevra/gwalk
 Author: Vera Del Favero
 Author-email: xevra86@gmail.com
 Maintainer: Vera Del Favero
 Maintainer-email: xevra86@gmail.com
 License: MIT Lisence
 Keywords: Gravitational Wave,Likelihood
```

### Comparing `gwalk-2.1.3/src/gwalk.egg-info/SOURCES.txt` & `gwalk-2.2.0/src/gwalk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.3/tests/test_decomposition.py` & `gwalk-2.2.0/tests/test_decomposition.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.3/tests/test_dpgmm.py` & `gwalk-2.2.0/tests/test_dpgmm.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.3/tests/test_grid.py` & `gwalk-2.2.0/tests/test_grid.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.3/tests/test_kl.py` & `gwalk-2.2.0/tests/test_kl.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.3/tests/test_maha.py` & `gwalk-2.2.0/tests/test_maha.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.3/tests/test_object.py` & `gwalk-2.2.0/tests/test_object.py`

 * *Files 8% similar despite different names*

```diff
@@ -210,18 +210,47 @@
 
     ## Initialize MV ##
     MV = MultivariateNormal(X0, limits=limits)
 
     ## Test sampling ##
     print("Testing sampling:")
     Y0 = MV.sample_normal(size=npts)
+    # Check shape of sample
+    assert Y0.shape == (npts, ndim)
+    # Check that all samples are inside limits
+    for i in range(ndim):
+        assert all(Y0[:,i] >= limits[i,0])
+        assert all(Y0[:,i] <= limits[i,1])
 
+    # Mess with the variance
+    MV.std = MV.std / 40
+    Y0 = MV.sample_normal(size=npts)
     # Check shape of sample
     assert Y0.shape == (npts, ndim)
+    # Check that all samples are inside limits
+    for i in range(ndim):
+        assert all(Y0[:,i] >= limits[i,0])
+        assert all(Y0[:,i] <= limits[i,1])
+    frac_err = (MV.mu - np.mean(Y0, axis=0))/MV.mu
+    # I hope 10000 samples don't have 5 percent error
+    assert np.max(np.abs(frac_err)) < 0.05
 
+    # Mess with the variance
+    MV.std = MV.std * 4
+    Y0 = MV.sample_normal(size=npts)
+    frac_err = (MV.mu - np.mean(Y0, axis=0))/MV.mu
+    # Check shape of sample
+    assert Y0.shape == (npts, ndim)
+    # Check that all samples are inside limits
+    for i in range(ndim):
+        assert all(Y0[:,i] >= limits[i,0])
+        assert all(Y0[:,i] <= limits[i,1])
+
+    # Check shape of sample
+    assert Y0.shape == (npts, ndim)
     # Check that all samples are inside limits
     for i in range(ndim):
         assert all(Y0[:,i] >= limits[i,0])
         assert all(Y0[:,i] <= limits[i,1])
     print("  pass!")
 
 def test_simple_fit(ndim, npts):
@@ -280,26 +309,26 @@
 
     ## Initialize MV ##
     MV = MultivariateNormal(X0, limits=limits)
 
     ## Test integral ##
     print("Testing analytic integral:")
     # Test the function version of the enclosed integral
-    integral0 = analytic_enclosed_integral(X0, limits, MV.scale)
+    integral0 = analytic_enclosed_integral(X0, limits, np.ones(MV.ndim))
     # Test the the object version
     integral1 = MV.analytic_enclosed_integral()
     # Check that they are the same
     assert np.allclose(integral0, integral1)
     # Test the assign feature and offset setting
     MV.analytic_enclosed_integral(assign=True)
     integral2 = np.exp(-MV.offset)
     assert np.allclose(integral0, integral2)
 
     # Test the function version with many inputs 
-    integraln = analytic_enclosed_integral(Xn, limits, MV.scale)
+    integraln = analytic_enclosed_integral(Xn, limits)
     # Test the object version with different parameter inputs
     integraln1 = MV.analytic_enclosed_integral(X=Xn)
     # Assert that they are the same
     assert np.allclose(integraln, integraln1)
     print("  pass!")
 
 def test_marginal(ndim, ngauss, npts):
```

### Comparing `gwalk-2.1.3/tests/test_pdf.py` & `gwalk-2.2.0/tests/test_pdf.py`

 * *Files identical despite different names*

