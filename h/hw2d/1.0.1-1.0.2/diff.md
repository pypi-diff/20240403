# Comparing `tmp/hw2d-1.0.1.tar.gz` & `tmp/hw2d-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hw2d-1.0.1.tar", last modified: Tue Feb 13 14:33:43 2024, max compression
+gzip compressed data, was "hw2d-1.0.2.tar", last modified: Wed Apr  3 21:24:09 2024, max compression
```

## Comparing `hw2d-1.0.1.tar` & `hw2d-1.0.2.tar`

### file list

```diff
@@ -1,61 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 14:33:43.183096 hw2d-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-02-13 14:33:21.000000 hw2d-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14184 2024-02-13 14:33:43.183096 hw2d-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12571 2024-02-13 14:33:21.000000 hw2d-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-02-13 14:33:21.000000 hw2d-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-13 14:33:43.183096 hw2d-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 14:33:43.175095 hw2d-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 14:33:43.175095 hw2d-1.0.1/src/hw2d/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-13 14:33:21.000000 hw2d-1.0.1/src/hw2d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-13 14:33:21.000000 hw2d-1.0.1/src/hw2d/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-13 14:33:21.000000 hw2d-1.0.1/src/hw2d/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 14:33:43.179095 hw2d-1.0.1/src/hw2d/gradients/
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-02-13 14:33:21.000000 hw2d-1.0.1/src/hw2d/gradients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-02-13 14:33:21.000000 hw2d-1.0.1/src/hw2d/gradients/numba_gradients.py
--rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-02-13 14:33:21.000000 hw2d-1.0.1/src/hw2d/gradients/numpy_gradients.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 14:33:43.179095 hw2d-1.0.1/src/hw2d/initializations/
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-02-13 14:33:21.000000 hw2d-1.0.1/src/hw2d/initializations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-02-13 14:33:21.000000 hw2d-1.0.1/src/hw2d/initializations/fourier_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-02-13 14:33:21.000000 hw2d-1.0.1/src/hw2d/initializations/sine.py
--rw-r--r--   0 runner    (1001) docker     (127)    10909 2024-02-13 14:33:21.000000 hw2d-1.0.1/src/hw2d/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 14:33:43.179095 hw2d-1.0.1/src/hw2d/physical_properties/
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-02-13 14:33:21.000000 hw2d-1.0.1/src/hw2d/physical_properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 14:33:21.000000 hw2d-1.0.1/src/hw2d/physical_properties/numba_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     9337 2024-02-13 14:33:21.000000 hw2d-1.0.1/src/hw2d/physical_properties/numpy_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 14:33:43.179095 hw2d-1.0.1/src/hw2d/poisson_bracket/
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-02-13 14:33:21.000000 hw2d-1.0.1/src/hw2d/poisson_bracket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-02-13 14:33:21.000000 hw2d-1.0.1/src/hw2d/poisson_bracket/numba_arakawa.py
--rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-02-13 14:33:21.000000 hw2d-1.0.1/src/hw2d/poisson_bracket/numpy_arakawa.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 14:33:43.179095 hw2d-1.0.1/src/hw2d/poisson_solvers/
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-02-13 14:33:21.000000 hw2d-1.0.1/src/hw2d/poisson_solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-02-13 14:33:21.000000 hw2d-1.0.1/src/hw2d/poisson_solvers/numba_fourier_poisson.py
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-02-13 14:33:21.000000 hw2d-1.0.1/src/hw2d/poisson_solvers/numpy_fourier_poisson.py
--rw-r--r--   0 runner    (1001) docker     (127)     9650 2024-02-13 14:33:21.000000 hw2d-1.0.1/src/hw2d/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 14:33:43.179095 hw2d-1.0.1/src/hw2d/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 14:33:21.000000 hw2d-1.0.1/src/hw2d/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-02-13 14:33:21.000000 hw2d-1.0.1/src/hw2d/utils/downsample.py
--rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-02-13 14:33:21.000000 hw2d-1.0.1/src/hw2d/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-02-13 14:33:21.000000 hw2d-1.0.1/src/hw2d/utils/latex_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-02-13 14:33:21.000000 hw2d-1.0.1/src/hw2d/utils/namespaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-02-13 14:33:21.000000 hw2d-1.0.1/src/hw2d/utils/performance_comparison.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 14:33:43.179095 hw2d-1.0.1/src/hw2d/utils/plot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 14:33:21.000000 hw2d-1.0.1/src/hw2d/utils/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-02-13 14:33:21.000000 hw2d-1.0.1/src/hw2d/utils/plot/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-02-13 14:33:21.000000 hw2d-1.0.1/src/hw2d/utils/plot/movie.py
--rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-02-13 14:33:21.000000 hw2d-1.0.1/src/hw2d/utils/plot/timetrace.py
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-02-13 14:33:21.000000 hw2d-1.0.1/src/hw2d/utils/run_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 14:33:43.183096 hw2d-1.0.1/src/hw2d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14184 2024-02-13 14:33:43.000000 hw2d-1.0.1/src/hw2d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-02-13 14:33:43.000000 hw2d-1.0.1/src/hw2d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-13 14:33:43.000000 hw2d-1.0.1/src/hw2d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-02-13 14:33:43.000000 hw2d-1.0.1/src/hw2d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-13 14:33:43.000000 hw2d-1.0.1/src/hw2d.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 14:33:43.183096 hw2d-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-02-13 14:33:21.000000 hw2d-1.0.1/tests/test_arakawa.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-02-13 14:33:21.000000 hw2d-1.0.1/tests/test_fourier_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-02-13 14:33:21.000000 hw2d-1.0.1/tests/test_numba_gradients.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-02-13 14:33:21.000000 hw2d-1.0.1/tests/test_numpy_gradients.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-02-13 14:33:21.000000 hw2d-1.0.1/tests/test_numpy_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-02-13 14:33:21.000000 hw2d-1.0.1/tests/test_poisson.py
--rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-02-13 14:33:21.000000 hw2d-1.0.1/tests/test_prop_preservation.py
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-13 14:33:21.000000 hw2d-1.0.1/tests/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:24:09.606611 hw2d-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-03 21:23:57.000000 hw2d-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14230 2024-04-03 21:24:09.606611 hw2d-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12571 2024-04-03 21:23:57.000000 hw2d-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-04-03 21:23:57.000000 hw2d-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 21:24:09.606611 hw2d-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:24:09.594611 hw2d-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:24:09.598611 hw2d-1.0.2/src/hw2d/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:24:09.598611 hw2d-1.0.2/src/hw2d/gradients/
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/gradients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/gradients/numba_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/gradients/numpy_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/gradients/phiml_gradients.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:24:09.602611 hw2d-1.0.2/src/hw2d/initializations/
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/initializations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/initializations/fourier_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/initializations/sine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11840 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:24:09.602611 hw2d-1.0.2/src/hw2d/physical_properties/
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/physical_properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/physical_properties/numba_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9337 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/physical_properties/numpy_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:24:09.602611 hw2d-1.0.2/src/hw2d/poisson_bracket/
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/poisson_bracket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/poisson_bracket/numba_arakawa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/poisson_bracket/numpy_arakawa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/poisson_bracket/phiml_arakawa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:24:09.602611 hw2d-1.0.2/src/hw2d/poisson_solvers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/poisson_solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/poisson_solvers/numba_fourier_poisson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/poisson_solvers/numpy_fourier_poisson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/poisson_solvers/phiml_fourier_poisson.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10396 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13537 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/run2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:24:09.602611 hw2d-1.0.2/src/hw2d/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/utils/downsample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/utils/latex_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/utils/namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/utils/performance_comparison.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:24:09.602611 hw2d-1.0.2/src/hw2d/utils/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/utils/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/utils/plot/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/utils/plot/movie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/utils/plot/timetrace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/utils/run_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:24:09.606611 hw2d-1.0.2/src/hw2d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14230 2024-04-03 21:24:09.000000 hw2d-1.0.2/src/hw2d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-03 21:24:09.000000 hw2d-1.0.2/src/hw2d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 21:24:09.000000 hw2d-1.0.2/src/hw2d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-03 21:24:09.000000 hw2d-1.0.2/src/hw2d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-03 21:24:09.000000 hw2d-1.0.2/src/hw2d.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:24:09.606611 hw2d-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-03 21:23:57.000000 hw2d-1.0.2/tests/test_arakawa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-03 21:23:57.000000 hw2d-1.0.2/tests/test_fourier_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-03 21:23:57.000000 hw2d-1.0.2/tests/test_numba_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-03 21:23:57.000000 hw2d-1.0.2/tests/test_numpy_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-03 21:23:57.000000 hw2d-1.0.2/tests/test_numpy_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-04-03 21:23:57.000000 hw2d-1.0.2/tests/test_poisson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-04-03 21:23:57.000000 hw2d-1.0.2/tests/test_prop_preservation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-03 21:23:57.000000 hw2d-1.0.2/tests/test_run.py
```

### Comparing `hw2d-1.0.1/LICENSE` & `hw2d-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.1/PKG-INFO` & `hw2d-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hw2d
-Version: 1.0.1
+Version: 1.0.2
 Summary: Reference HW2D Implementation in Python
 Author-email: Robin Greif <rccgreif@gmail.com>
 License: MIT
 Project-URL: Changelog, https://github.com/the-rccg/hw2d/blob/main/CHANGES.md
 Project-URL: Homepage, https://github.com/the-rccg/hw2d
 Project-URL: Issues, https://github.com/the-rccg/hw2d/issues
 Keywords: Plasma Physics,Simulation,Turbulence
@@ -30,14 +30,15 @@
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scipy
 Requires-Dist: tqdm
 Requires-Dist: perfplot
 Provides-Extra: accelerators
 Requires-Dist: numba; extra == "accelerators"
+Requires-Dist: phiml; extra == "accelerators"
 Provides-Extra: develop
 Requires-Dist: coverage; extra == "develop"
 Requires-Dist: pre-commit; extra == "develop"
 Requires-Dist: pytest; extra == "develop"
 Requires-Dist: pytest-cov; extra == "develop"
 Requires-Dist: pytest-mock; extra == "develop"
```

### Comparing `hw2d-1.0.1/README.md` & `hw2d-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.1/pyproject.toml` & `hw2d-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,16 @@
 license = {text = "MIT"}
 name = "hw2d"
 readme = "README.md"
 requires-python = ">=3.7.1"
 
 [project.optional-dependencies]
 accelerators = [
-    "numba"
+    "numba",
+    "phiml"
 ]
 develop = [
     "coverage",
     "pre-commit",
     "pytest",
     "pytest-cov",
     "pytest-mock"
```

### Comparing `hw2d-1.0.1/src/hw2d/gradients/__init__.py` & `hw2d-1.0.2/src/hw2d/gradients/__init__.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.1/src/hw2d/gradients/numba_gradients.py` & `hw2d-1.0.2/src/hw2d/gradients/numba_gradients.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.1/src/hw2d/gradients/numpy_gradients.py` & `hw2d-1.0.2/src/hw2d/gradients/numpy_gradients.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.1/src/hw2d/initializations/__init__.py` & `hw2d-1.0.2/src/hw2d/initializations/__init__.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.1/src/hw2d/initializations/fourier_noise.py` & `hw2d-1.0.2/src/hw2d/initializations/fourier_noise.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.1/src/hw2d/initializations/sine.py` & `hw2d-1.0.2/src/hw2d/initializations/sine.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.1/src/hw2d/model.py` & `hw2d-1.0.2/src/hw2d/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,60 +1,169 @@
 """
 hw2d.model: Hasegawa-Wakatani 2D Simulation Module
 
-This module provides the core functionality to simulate the Hasegawa-Wakatani (HW) model in two dimensions. 
-It offers flexibility in terms of numerical schemes and allows for comprehensive profiling and debugging 
+This module provides the core functionality to simulate the Hasegawa-Wakatani (HW) model in two dimensions.
+It offers flexibility in terms of numerical schemes and allows for comprehensive profiling and debugging
 of the simulation process.
 
 Functions:
     - euler_step: Implements the Euler time-stepping method.
     - rk4_step: Implements the Runge-Kutta 4th order time-stepping method.
     - get_phi: Computes the electrostatic potential from vorticity.
     - diffuse: Applies diffusion to an array.
     - gradient_2d: Computes the 2D gradient of the system.
     - get_gammas: Computes energy gradients.
 
 Classes:
     - HW: Represents the primary simulation entity for the Hasegawa-Wakatani model.
 
 Notes:
-    The module supports both NumPy and Numba for computational operations and provides detailed logging and 
+    The module supports both NumPy and Numba for computational operations and provides detailed logging and
     profiling capabilities.
 """
+
 from typing import Tuple, Callable, Dict
 import numpy as np
 import matplotlib.pyplot as plt
 import time
 import pandas as pd
 
 # Local Imports
 from hw2d.initializations.fourier_noise import get_fft_noise
 from hw2d.utils.namespaces import Namespace
 
 # NumPy Version
 from hw2d.gradients.numpy_gradients import periodic_laplace_N, periodic_gradient
 from hw2d.poisson_bracket.numpy_arakawa import periodic_arakawa_vec
 from hw2d.poisson_solvers.numpy_fourier_poisson import fourier_poisson_double
-from hw2d.physical_properties.numpy_properties import *
+from hw2d.physical_properties.numpy_properties import get_DE, get_DU, get_dE_dt, get_dU_dt, get_gamma_n, get_gamma_c
+
 periodic_arakawa = periodic_arakawa_vec
 
 try:
     # Numba
     from hw2d.gradients.numba_gradients import periodic_laplace_N, periodic_gradient
     from hw2d.poisson_bracket.numba_arakawa import periodic_arakawa_stencil
     from hw2d.poisson_solvers.numba_fourier_poisson import fourier_poisson_double
 
     periodic_arakawa = periodic_arakawa_stencil
+    pass
 except:
     pass
 
 # Other
 # from hw2d.poisson_solvers.pyfftw_fourier_poisson import fourier_poisson_pyfftw
 
 
+def pass_func(*args, **kwargs):
+    """do nothing function"""
+    return
+
+
+def hw2d_gradient(
+    density: np.ndarray,
+    omega: np.ndarray,
+    dt: float,
+    dx: float,
+    get_phi_func: Callable,
+    gradient_func: Callable,
+    diffuse_func: Callable,
+    poisson_bracket_func: Callable,
+    get_gammas_func: Callable,
+    poisson_bracket_coeff: float,
+    kappa_coeff: float,
+    c1: float,
+    nu: float,
+    N: int,
+    log: Callable = pass_func,
+    phi: np.ndarray or None = None,
+    debug: bool = False,
+    TEST_CONSERVATION: bool = False,
+    **kwargs
+) -> Namespace:
+    if phi is None:
+        phi = get_phi_func(omega, dx=dx)
+    # Setup
+    arak_comp_o = 0
+    arak_comp_n = 0
+    kap = 0
+    Do = 0
+    Dn = 0
+    t0 = time.time()
+    dy_p = gradient_func(phi, dx=dx, axis=0)
+    log("gradient_2d", time.time() - t0)
+
+    # Calculate Gradients
+    diff = phi - density
+
+    # Step 2.1: New Omega.
+    o = c1 * diff
+    if poisson_bracket_coeff:
+        t0 = time.time()
+        arak_comp_o = -poisson_bracket_coeff * poisson_bracket_func(
+            zeta=phi, psi=omega, dx=dx
+        )
+        log("poisson_bracket", time.time() - t0)
+        o += arak_comp_o
+    if nu:
+        Do = nu * diffuse_func(arr=omega, dx=dx, N=N)
+        o += Do
+
+    # Step 2.2: New Density.
+    n = c1 * diff
+    if poisson_bracket_coeff:
+        t0 = time.time()
+        arak_comp_n = -poisson_bracket_coeff * poisson_bracket_func(
+            zeta=phi, psi=density, dx=dx
+        )
+        log("poisson_bracket", time.time() - t0)
+        n += arak_comp_n
+    if kappa_coeff:
+        kap = -kappa_coeff * dy_p
+        n += kap
+    if nu:
+        Dn = nu * diffuse_func(arr=density, dx=dx, N=N)
+        n += Dn
+
+    # Print gradients to see which one explodes
+    if debug:
+        print(
+            "  |  ".join(
+                [
+                    f"  dO/dt = {np.max(np.abs(c1 * diff)):>8.2g} + {np.max(np.abs(arak_comp_o)):>8.2g} + {np.max(np.abs(Do)):>8.2g}"
+                    f"  dn/dt = {np.max(np.abs(c1 * diff)):>8.2g} + {np.max(np.abs(arak_comp_n)):>8.2g} + {np.max(np.abs(kap)):>8.2g} + {np.max(np.abs(Dn)):>8.2g}",
+                    f"  dO/dt = {np.mean(c1 * diff):>8.2g} + {np.mean(arak_comp_o):>8.2g} + {np.mean(Do):>8.2g}",
+                    f"  dn/dt = {np.mean(c1 * diff):>8.2g} + {np.mean(arak_comp_n):>8.2g} + {np.mean(kap):>8.2g} + {np.mean(Dn):>8.2g}",
+                ]
+            )
+        )
+
+    # Structure return
+    return_dict = Namespace(
+        density=n,
+        omega=o
+    )
+
+    if "age" in kwargs:
+        return_dict["age"] = kwargs["age"] + dt
+
+    # Add energy gradients for testing conservation
+    if TEST_CONSERVATION:
+        gamma_n, gamma_c = get_gammas_func(density, phi)
+        Dp = nu * diffuse_func(arr=phi, dx=dx, N=N)
+        DE = get_DE(n=density, p=phi, Dn=Dn, Dp=Dp)
+        DU = get_DU(n=density, o=omega, Dn=Dn, Dp=Dp)
+        dE_dt = get_dE_dt(gamma_n=gamma_n, gamma_c=gamma_c, DE=DE)
+        dU_dt = get_dU_dt(gamma_n=gamma_n, DU=DU)
+        return_dict["dE"] = dE_dt
+        return_dict["dU"] = dU_dt
+
+    return return_dict
+
+
 class HW:
     def __init__(
         self,
         dx: float,
         N: int,
         c1: float,
         nu: float,
@@ -126,30 +235,30 @@
         df.sort_values("time/call", inplace=True)
         print(df)
 
     def euler_step(
         self, plasma: Namespace, dt: float, dx: float, **kwargs
     ) -> Namespace:
         t0 = time.time()
-        y = Namespace(**{k:v for k,v in plasma.items() if k != "phi"})
+        y = Namespace(**{k: v for k, v in plasma.items() if k != "phi"})
         if "phi" in plasma:
             d = dt * self.gradient_2d(**y, phi=plasma["phi"], dt=0, dx=dx)
         else:
             d = dt * self.gradient_2d(**y, dt=0, dx=dx)
         y += d
         y["phi"] = self.get_phi(omega=y.omega, dx=dx)
         y["age"] = plasma.age + dt
         # Wrap-up
         self.log("full_step", time.time() - t0)
         return y
 
     def rk4_step(self, plasma: Namespace, dt: float, dx: float, **kwargs) -> Namespace:
         # RK4
         t0 = time.time()
-        yn = Namespace(**{k:v for k,v in plasma.items() if k != "phi"})
+        yn = Namespace(**{k: v for k, v in plasma.items() if k != "phi"})
         # pn = self.get_phi(omega=yn.omega, dx=dx)  # TODO: only execute for t=0
         pn = plasma.phi
         k1 = dt * self.gradient_2d(**yn, phi=pn, dt=0, dx=dx)
         y1 = yn + k1 * 0.5
         p1 = self.get_phi(omega=y1.omega, dx=dx)
         k2 = dt * self.gradient_2d(**y1, phi=p1, dt=dt / 2, dx=dx)
         y2 = yn + k2 * 0.5
@@ -157,15 +266,15 @@
         k3 = dt * self.gradient_2d(**y2, phi=p2, dt=dt / 2, dx=dx)
         y3 = yn + k3
         p3 = self.get_phi(omega=y3.omega, dx=dx)
         k4 = dt * self.gradient_2d(**y3, phi=p3, dt=dt, dx=dx)
         # p4 = self.get_phi(k4.omega)
         # TODO: currently adds two timesteps
         yk1 = yn + (k1 + 2 * k2 + 2 * k3 + k4) * (1 / 6)
-        phi = self.get_phi(omega=y1.omega, dx=dx)
+        phi = self.get_phi(omega=yk1.omega, dx=dx)
         # Set properties not valid through y1
         yk1["phi"] = phi
         yk1["age"] = plasma.age + dt
         # Wrap-up
         self.log("full_step", time.time() - t0)
         if self.debug:
             print(
@@ -203,91 +312,35 @@
         omega: np.ndarray,
         dt: float,
         dx: float,
         phi: np.ndarray or None = None,
         debug: bool = False,
         **kwargs
     ) -> Namespace:
-        if phi is None:
-            phi = self.get_phi(omega, dx=dx)
-        # Setup
-        arak_comp_o = 0
-        arak_comp_n = 0
-        kap = 0
-        Do = 0
-        Dn = 0
-        t0 = time.time()
-        dy_p = self.gradient_func(phi, dx=dx, axis=0)
-        self.log("gradient_2d", time.time() - t0)
-
-        # Calculate Gradients
-        diff = phi - density
-
-        # Step 2.1: New Omega.
-        o = self.c1 * diff
-        if self.poisson_bracket_coeff:
-            t0 = time.time()
-            arak_comp_o = -self.poisson_bracket_coeff * self.poisson_bracket(
-                zeta=phi, psi=omega, dx=dx
-            )
-            self.log("poisson_bracket", time.time() - t0)
-            o += arak_comp_o
-        if self.nu:
-            Do = self.nu * self.diffuse(arr=omega, dx=dx, N=self.N)
-            o += Do
-
-        # Step 2.2: New Density.
-        n = self.c1 * diff
-        if self.poisson_bracket_coeff:
-            t0 = time.time()
-            arak_comp_n = -self.poisson_bracket_coeff * self.poisson_bracket(
-                zeta=phi, psi=density, dx=dx
-            )
-            self.log("poisson_bracket", time.time() - t0)
-            n += arak_comp_n
-        if self.kappa_coeff:
-            kap = -self.kappa_coeff * dy_p
-            n += kap
-        if self.nu:
-            Dn = self.nu * self.diffuse(arr=density, dx=dx, N=self.N)
-            n += Dn
-
-        # Print gradients to see which one explodes
-        if debug:
-            print(
-                "  |  ".join(
-                    [
-                        f"  dO/dt = {np.max(np.abs(self.c1 * diff)):>8.2g} + {np.max(np.abs(arak_comp_o)):>8.2g} + {np.max(np.abs(Do)):>8.2g}"
-                        f"  dn/dt = {np.max(np.abs(self.c1 * diff)):>8.2g} + {np.max(np.abs(arak_comp_n)):>8.2g} + {np.max(np.abs(kap)):>8.2g} + {np.max(np.abs(Dn)):>8.2g}",
-                        f"  dO/dt = {np.mean(self.c1 * diff):>8.2g} + {np.mean(arak_comp_o):>8.2g} + {np.mean(Do):>8.2g}",
-                        f"  dn/dt = {np.mean(self.c1 * diff):>8.2g} + {np.mean(arak_comp_n):>8.2g} + {np.mean(kap):>8.2g} + {np.mean(Dn):>8.2g}",
-                    ]
-                )
-            )
-
-        # Structure return
-        return_dict = Namespace(
-            density=n,
-            omega=o
+        return hw2d_gradient(
+            density=density,
+            omega=omega,
+            dt=dt,
+            dx=dx,
+            get_phi_func=self.get_phi,
+            gradient_func=self.gradient_func,
+            diffuse_func=self.diffuse,
+            poisson_bracket_func=self.poisson_bracket,
+            get_gammas_func=self.get_gammas,
+            log=self.log,
+            poisson_bracket_coeff=self.poisson_bracket_coeff,
+            kappa_coeff=self.kappa_coeff,
+            c1=self.c1,
+            nu=self.nu,
+            N=self.N,
+            phi=phi,
+            debug=debug,
+            TEST_CONSERVATION=self.TEST_CONSERVATION,
+            **kwargs
         )
 
-        if "age" in kwargs:
-            return_dict["age"] = kwargs["age"] + dt
-
-        # Add energy gradients for testing conservation
-        if self.TEST_CONSERVATION:
-            gamma_n, gamma_c = self.get_gammas(density, phi)
-            Dp = self.nu * self.diffuse(arr=phi, dx=dx, N=self.N)
-            DE = get_DE(n=density, p=phi, Dn=Dn, Dp=Dp)
-            DU = get_DU(n=density, o=omega, Dn=Dn, Dp=Dp)
-            dE_dt = get_dE_dt(gamma_n=gamma_n, gamma_c=gamma_c, DE=DE)
-            dU_dt = get_dU_dt(gamma_n=gamma_n, DU=DU)
-            return_dict["dE"] = dE_dt
-            return_dict["dU"] = dU_dt
-
-        return return_dict
 
     def get_gammas(self, n: np.ndarray, p: np.ndarray) -> Tuple[np.ndarray, np.ndarray]:
         # Generate Energy Gradients
         gamma_n = get_gamma_n(n=n, p=p, dx=self.dx)
         gamma_c = get_gamma_c(n=n, p=p, c1=self.c1, dx=self.dx)
         return gamma_n, gamma_c
```

### Comparing `hw2d-1.0.1/src/hw2d/physical_properties/__init__.py` & `hw2d-1.0.2/src/hw2d/physical_properties/__init__.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.1/src/hw2d/physical_properties/numpy_properties.py` & `hw2d-1.0.2/src/hw2d/physical_properties/numpy_properties.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.1/src/hw2d/poisson_bracket/__init__.py` & `hw2d-1.0.2/src/hw2d/poisson_bracket/__init__.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.1/src/hw2d/poisson_bracket/numba_arakawa.py` & `hw2d-1.0.2/src/hw2d/poisson_bracket/numba_arakawa.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.1/src/hw2d/poisson_bracket/numpy_arakawa.py` & `hw2d-1.0.2/src/hw2d/poisson_bracket/numpy_arakawa.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.1/src/hw2d/poisson_solvers/__init__.py` & `hw2d-1.0.2/src/hw2d/poisson_solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.1/src/hw2d/poisson_solvers/numba_fourier_poisson.py` & `hw2d-1.0.2/src/hw2d/poisson_solvers/numba_fourier_poisson.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.1/src/hw2d/poisson_solvers/numpy_fourier_poisson.py` & `hw2d-1.0.2/src/hw2d/poisson_solvers/numpy_fourier_poisson.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.1/src/hw2d/run.py` & `hw2d-1.0.2/src/hw2d/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,62 +17,67 @@
     continue_h5_file,
 )
 from hw2d.utils.namespaces import Namespace
 from hw2d.utils.plot.movie import create_movie
 from hw2d.utils.run_properties import calculate_properties
 from hw2d.utils.plot.timetrace import plot_timetraces
 from hw2d.utils.downsample import fourier_downsample
+from hw2d.utils.helpers import format_print_dict
 
 
 def run(
     # Physics & Numerics
     step_size: float = 0.025,
-    end_time: float = 300,
-    grid_pts: int = 64,
+    end_time: float = 1_000,
+    grid_pts: int = 1024,
     k0: float = 0.15,
     N: int = 3,
     nu: float = 5.0e-08,
     c1: float = 1.0,
     kappa_coeff: float = 1.0,
     poisson_bracket_coeff: float = 1.0,
     # Initialization
     seed: int or None = None,
     init_type: str = "normal",
     init_scale: float = 1 / 100,
     # Saving
     output_path: str = "_test.h5",
-    continue_file: bool = False,
+    continue_file: bool or str = False,
     buffer_length: int = 100,
     snaps: int = 1,
-    downsample_factor: float = 2,
+    downsample_factor: float = 1,
     # Movie
     movie: bool = True,
     min_fps: int = 10,
     dpi: int = 75,
-    speed: int = 5,
+    speed: int = 10,
     # Properties
     properties: Iterable[str] = [
         "gamma_n",
         "gamma_n_spectral",
         "gamma_c",
         "energy",
         "thermal_energy",
         "kinetic_energy",
         "enstrophy",
         "enstrophy_phi",
     ],
     # Plotting
     plot_properties: Iterable[str] = (
+        "gamma_c",
+        "gamma_n",
+        "gamma_n_spectral",
         "enstrophy",
         "energy",
         "kinetic_energy",
         "thermal_energy",
     ),
     # Other
     debug: bool = False,
+    force_recompute: bool = True,
 ):
     """
     Run the simulation with the given parameters.
 
     Args:
         step_size (float, optional): Incremental step for simulation progression. Defaults to 0.025.
         end_time (float, optional): Duration till the simulation should run. Defaults to 1_000.
@@ -83,15 +88,15 @@
         c1 (float, optional): Transition scale between hydrodynamic and adiabatic. Suggested values: 0.1, 1, 5. Defaults to 1.0.
         kappa_coeff (float, optional): Coefficient of d/dy phi. Defaults to 1.0.
         poisson_bracket_coeff (float, optional): Coefficient of Poisson bracket [A,B] implemented with Arakawa Scheme. Defaults to 1.0.
         seed (int or None, optional): Seed for random number generation. Defaults to None.
         init_type (str, optional): Initialization method. Choices: 'fourier', 'sine', 'random', 'normal'. Defaults to 'normal'.
         init_scale (float, optional): Scaling factor for initialization. Defaults to 0.01.
         output_path (str, optional): Where to save the simulation data. Defaults to ''.
-        continue_file (bool, optional): If True, continue with existing file. Defaults to False.
+        continue_file (bool or str, optional): If True, continue with existing file. If path, it will continue with file from path. Defaults to False.
         buffer_length (int, optional): Size of buffer for storage. Defaults to 100.
         snaps (int, optional): Snapshot intervals for saving. Defaults to 1.
         movie (bool, optional): If True, generate a movie out of simulation. Defaults to True.
         min_fps (int, optional): Parameter for movie generation. Defaults to 10.
         dpi (int, optional): Parameter for movie generation. Defaults to 75.
         speed (int, optional): Parameter for movie generation. Defaults to 5.
         properties (Iterable[str], optional): List of properties to calculate for the saved file.
@@ -145,15 +150,15 @@
         density=noise[init_type](y, x) * init_scale,
         omega=noise[init_type](y, x) * init_scale,
         phi=noise[init_type](y, x) * init_scale,
         age=0,
     )
 
     # File Handling
-    if continue_file:
+    if continue_file and isinstance(continue_file, str):
         # Continue from previous run
         plasma, physics_params = continue_h5_file(continue_file, field_list)
         current_time = plasma.age
         # Check if broken
         for field in plasma.keys():
             if np.isnan(np.sum(plasma[field])):
                 print(f"FAILED @ {iteration_count:,} steps ({plasma.age:,})")
@@ -175,53 +180,63 @@
         }
         output_params = {
             "buffer": buffer,
             "buffer_index": 0,
             "output_path": output_path,
         }
         # Load Data
-        if os.path.isfile(output_path):
-            if not continue_file:
+        if os.path.isfile(output_path) and not force_recompute:
+            if continue_file:
+                plasma, physics_params = continue_h5_file(output_path, field_list)
+                print(
+                    f"Successfully loaded: {output_path} (age={plasma.age})\n{physics_params}"
+                )
+                current_time = plasma.age
+            else:
                 print(f"File already exists.")
                 return
         # Create
         else:
             save_params = get_save_params(physics_params, step_size, snaps, x, y, x_save=x_save, y_save=y_save)
             create_appendable_h5(
                 output_path, save_params, dtype=np.float32, chunk_size=100
             )
             new_val = plasma
             if downsample_factor != 1:
+                # TODO: Create space for last state that gets overwritten every batch
                 new_val = Namespace(**{k: downsample_fnc(v, downsample_factor) for k,v in plasma.items() if k in ("phi", "omega", "density")})
             output_params["buffer_index"] = save_to_buffered_h5(
                 new_val=new_val, buffer_length=buffer_length, **output_params
             )
 
+    # Display runtime parameters
+    format_print_dict(save_params)
+
     # Setup Simulation
     hw = HW(**physics_params, debug=debug)
     plasma["phi"] = hw.get_phi(plasma.omega, physics_params["dx"])
 
     # Run Simulation
     print("Running simulation...")
-    for i in tqdm(range(1, steps + 1)):
+    for iteration_count in tqdm(range(1, steps + 1)):
         # Progress one step, alternatively: hw.euler_step()
         plasma = hw.rk4_step(plasma, dt=step_size, dx=dx)
 
         # Save to records
-        if output_path and i % snaps == 0:
+        if output_path and iteration_count % snaps == 0:
             new_val = plasma
             if downsample_factor != 1:
                 new_val = Namespace(**{k: downsample_fnc(v, downsample_factor) for k,v in plasma.items() if k in ("phi", "omega", "density")})
             output_params["buffer_index"] = save_to_buffered_h5(
                 new_val=new_val, buffer_length=buffer_length, **output_params
             )
 
         # Check for breaking
         if np.isnan(np.sum(plasma.density)):
-            print(f"FAILED @ {i:,} steps ({plasma.age:,})")
+            print(f"FAILED @ {iteration_count:,} steps ({plasma.age:,})")
             break
 
     # If output_path is defined, flush any remaining data in the buffer
     if output_path and output_params["buffer_index"] > 0:
         append_h5(**output_params)
 
     # Get Performance stats
```

### Comparing `hw2d-1.0.1/src/hw2d/utils/downsample.py` & `hw2d-1.0.2/src/hw2d/utils/downsample.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.1/src/hw2d/utils/io.py` & `hw2d-1.0.2/src/hw2d/utils/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Dict, List, Tuple, Any
 import h5py
 import numpy as np
+
 from hw2d.utils.namespaces import Namespace
 
 
 def get_save_params(
     params: Dict[str, Any], dt: float, snaps: int, x: int, y: int, x_save: int or None = None, y_save: int or None = None
 ) -> Dict[str, Any]:
     params = params.copy()
@@ -20,29 +21,40 @@
 
 def create_appendable_h5(
     filepath: str,
     params: Dict[str, Any],
     dtype: np.dtype = np.float32,
     chunk_size: int = 100,
     field_list: List[str] = ["density", "omega", "phi"],
+    properties: List[str] = []
 ) -> None:
     y = params["y_save"]
     x = params["x_save"]
     with h5py.File(f"{filepath}", "w") as hf:
         for field_name in field_list:
             hf.create_dataset(
                 field_name,
                 dtype=dtype,
                 shape=(0, y, x),
                 maxshape=(None, y, x),
                 chunks=(chunk_size, y, x),
                 compression="gzip",
             )
+        for prop_name in properties:
+            hf.create_dataset(
+                prop_name,
+                dtype=dtype,
+                shape=(0, 1),
+                maxshape=(None, 1),
+                chunks=(chunk_size, 1),
+                compression="gzip",
+            )
         for key, value in params.items():
             hf.attrs[key] = value
+    print(f"Created: {filepath}")
 
 
 def append_h5(output_path: str, buffer: np.ndarray, buffer_index: int) -> None:
     """append a file, from buffer, with buffer_index size"""
     with h5py.File(output_path, "a") as hf:
         for field_name in buffer.keys():
             _ = hf[field_name].resize((hf[field_name].shape[0] + buffer_index), axis=0)
```

### Comparing `hw2d-1.0.1/src/hw2d/utils/latex_format.py` & `hw2d-1.0.2/src/hw2d/utils/latex_format.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.1/src/hw2d/utils/namespaces.py` & `hw2d-1.0.2/src/hw2d/utils/namespaces.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.1/src/hw2d/utils/performance_comparison.py` & `hw2d-1.0.2/src/hw2d/utils/performance_comparison.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.1/src/hw2d/utils/plot/image.py` & `hw2d-1.0.2/src/hw2d/utils/plot/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,8 +130,8 @@
     if save_file_path:
         fig.savefig(save_file_path[:-4] + ".jpg")
         fig.savefig(save_file_path[:-4] + ".pdf")
     print(save_file_path)
 
 
 if __name__ == "__main__":
-    main()
+    fire.Fire(main)
```

### Comparing `hw2d-1.0.1/src/hw2d/utils/plot/movie.py` & `hw2d-1.0.2/src/hw2d/utils/plot/movie.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.1/src/hw2d/utils/plot/timetrace.py` & `hw2d-1.0.2/src/hw2d/utils/plot/timetrace.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.1/src/hw2d/utils/run_properties.py` & `hw2d-1.0.2/src/hw2d/utils/run_properties.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.1/src/hw2d.egg-info/PKG-INFO` & `hw2d-1.0.2/src/hw2d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hw2d
-Version: 1.0.1
+Version: 1.0.2
 Summary: Reference HW2D Implementation in Python
 Author-email: Robin Greif <rccgreif@gmail.com>
 License: MIT
 Project-URL: Changelog, https://github.com/the-rccg/hw2d/blob/main/CHANGES.md
 Project-URL: Homepage, https://github.com/the-rccg/hw2d
 Project-URL: Issues, https://github.com/the-rccg/hw2d/issues
 Keywords: Plasma Physics,Simulation,Turbulence
@@ -30,14 +30,15 @@
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scipy
 Requires-Dist: tqdm
 Requires-Dist: perfplot
 Provides-Extra: accelerators
 Requires-Dist: numba; extra == "accelerators"
+Requires-Dist: phiml; extra == "accelerators"
 Provides-Extra: develop
 Requires-Dist: coverage; extra == "develop"
 Requires-Dist: pre-commit; extra == "develop"
 Requires-Dist: pytest; extra == "develop"
 Requires-Dist: pytest-cov; extra == "develop"
 Requires-Dist: pytest-mock; extra == "develop"
```

### Comparing `hw2d-1.0.1/src/hw2d.egg-info/SOURCES.txt` & `hw2d-1.0.2/src/hw2d.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -2,36 +2,41 @@
 README.md
 pyproject.toml
 src/hw2d/__init__.py
 src/hw2d/__main__.py
 src/hw2d/__version__.py
 src/hw2d/model.py
 src/hw2d/run.py
+src/hw2d/run2.py
 src/hw2d.egg-info/PKG-INFO
 src/hw2d.egg-info/SOURCES.txt
 src/hw2d.egg-info/dependency_links.txt
 src/hw2d.egg-info/requires.txt
 src/hw2d.egg-info/top_level.txt
 src/hw2d/gradients/__init__.py
 src/hw2d/gradients/numba_gradients.py
 src/hw2d/gradients/numpy_gradients.py
+src/hw2d/gradients/phiml_gradients.py
 src/hw2d/initializations/__init__.py
 src/hw2d/initializations/fourier_noise.py
 src/hw2d/initializations/sine.py
 src/hw2d/physical_properties/__init__.py
 src/hw2d/physical_properties/numba_properties.py
 src/hw2d/physical_properties/numpy_properties.py
 src/hw2d/poisson_bracket/__init__.py
 src/hw2d/poisson_bracket/numba_arakawa.py
 src/hw2d/poisson_bracket/numpy_arakawa.py
+src/hw2d/poisson_bracket/phiml_arakawa.py
 src/hw2d/poisson_solvers/__init__.py
 src/hw2d/poisson_solvers/numba_fourier_poisson.py
 src/hw2d/poisson_solvers/numpy_fourier_poisson.py
+src/hw2d/poisson_solvers/phiml_fourier_poisson.py
 src/hw2d/utils/__init__.py
 src/hw2d/utils/downsample.py
+src/hw2d/utils/helpers.py
 src/hw2d/utils/io.py
 src/hw2d/utils/latex_format.py
 src/hw2d/utils/namespaces.py
 src/hw2d/utils/performance_comparison.py
 src/hw2d/utils/run_properties.py
 src/hw2d/utils/plot/__init__.py
 src/hw2d/utils/plot/image.py
```

### Comparing `hw2d-1.0.1/tests/test_arakawa.py` & `hw2d-1.0.2/tests/test_arakawa.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from unittest import TestCase
 
 import numpy as np
-from hw2d.poisson_bracket.numba_arakawa import periodic_arakawa_stencil as periodic_arakawa_nb
-from hw2d.poisson_bracket.numba_arakawa import periodic_arakawa_vec as periodic_arakawa_vec_nb
 from hw2d.poisson_bracket.numpy_arakawa import periodic_arakawa as periodic_arakawa
 from hw2d.poisson_bracket.numpy_arakawa import periodic_arakawa_vec as periodic_arakawa_np
-from hw2d.gradients.numpy_gradients import periodic_gradient
+from hw2d.poisson_bracket.numba_arakawa import periodic_arakawa_stencil as periodic_arakawa_nb
+from hw2d.poisson_bracket.numba_arakawa import periodic_arakawa_vec as periodic_arakawa_vec_nb
 from hw2d.initializations.sine import get_2d_sine
 
 
 class test_arakawa(TestCase):
     def test_periodic_arakawa_nb(self):
         N = 128
         grid_size = (N, N)
```

### Comparing `hw2d-1.0.1/tests/test_fourier_noise.py` & `hw2d-1.0.2/tests/test_fourier_noise.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.1/tests/test_numba_gradients.py` & `hw2d-1.0.2/tests/test_numba_gradients.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.1/tests/test_numpy_gradients.py` & `hw2d-1.0.2/tests/test_numpy_gradients.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.1/tests/test_numpy_properties.py` & `hw2d-1.0.2/tests/test_numpy_properties.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.1/tests/test_poisson.py` & `hw2d-1.0.2/tests/test_poisson.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.1/tests/test_prop_preservation.py` & `hw2d-1.0.2/tests/test_prop_preservation.py`

 * *Files identical despite different names*

