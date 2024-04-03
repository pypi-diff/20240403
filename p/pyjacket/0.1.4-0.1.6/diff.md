# Comparing `tmp/pyjacket-0.1.4.tar.gz` & `tmp/pyjacket-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjacket-0.1.4.tar", last modified: Wed Apr  3 16:43:17 2024, max compression
+gzip compressed data, was "pyjacket-0.1.6.tar", last modified: Wed Apr  3 19:04:10 2024, max compression
```

## Comparing `pyjacket-0.1.4.tar` & `pyjacket-0.1.6.tar`

### file list

```diff
@@ -1,71 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:43:17.454429 pyjacket-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-03 16:43:07.000000 pyjacket-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-03 16:43:17.454429 pyjacket-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-03 16:43:07.000000 pyjacket-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:43:17.446429 pyjacket-0.1.4/pyjacket/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:43:17.450429 pyjacket-0.1.4/pyjacket/arrtools/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/arrtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/arrtools/arrtools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/arrtools/bitdepth.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/arrtools/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/arrtools/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/arrtools/rois.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/arrtools/sizing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/arrtools/skeletonize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/arrtools/slicing.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/arrtools/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:43:17.450429 pyjacket-0.1.4/pyjacket/chemistry/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/chemistry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:43:17.450429 pyjacket-0.1.4/pyjacket/core/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/core/all_same.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/core/batched.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/core/digits.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/core/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/core/find_nth.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/core/format.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/core/iterations.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/core/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/core/python_ext.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/core/rounding.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/core/sortby.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/core/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:43:17.450429 pyjacket-0.1.4/pyjacket/cvtools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/cvtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/cvtools/color_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/cvtools/color_picker.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/cvtools/color_slicing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:43:17.450429 pyjacket-0.1.4/pyjacket/filetools/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/filetools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:43:17.454429 pyjacket-0.1.4/pyjacket/filetools/_imread/
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/filetools/_imread/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/filetools/_imread/imread_nd2.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/filetools/_imread/imread_tif.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/filetools/_imread/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:43:17.454429 pyjacket-0.1.4/pyjacket/filetools/_imwrite/
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/filetools/_imwrite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/filetools/_imwrite/imwrite_tif.py
--rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/filetools/filemanager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:43:17.454429 pyjacket-0.1.4/pyjacket/graphs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/graphs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/graphs/absorbing_markov.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/graphs/markov.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:43:17.454429 pyjacket-0.1.4/pyjacket/ntheory/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/ntheory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/ntheory/factors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:43:17.454429 pyjacket-0.1.4/pyjacket/ntheory/modulo/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/ntheory/modulo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/ntheory/modulo/modular_arithmetic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:43:17.454429 pyjacket-0.1.4/pyjacket/ntheory/primes/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/ntheory/primes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/ntheory/primes/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/ntheory/primes/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-03 16:43:07.000000 pyjacket-0.1.4/pyjacket/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:43:17.454429 pyjacket-0.1.4/pyjacket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-03 16:43:17.000000 pyjacket-0.1.4/pyjacket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-03 16:43:17.000000 pyjacket-0.1.4/pyjacket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 16:43:17.000000 pyjacket-0.1.4/pyjacket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 16:43:17.000000 pyjacket-0.1.4/pyjacket.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 16:43:17.454429 pyjacket-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-03 16:43:07.000000 pyjacket-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:04:10.220310 pyjacket-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-03 19:04:06.000000 pyjacket-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-03 19:04:10.220310 pyjacket-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-03 19:04:06.000000 pyjacket-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:04:10.212310 pyjacket-0.1.6/pyjacket/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-03 19:04:06.000000 pyjacket-0.1.6/pyjacket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:04:10.216310 pyjacket-0.1.6/pyjacket/arrtools/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-03 19:04:06.000000 pyjacket-0.1.6/pyjacket/arrtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-04-03 19:04:06.000000 pyjacket-0.1.6/pyjacket/arrtools/arrtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-03 19:04:06.000000 pyjacket-0.1.6/pyjacket/arrtools/bitdepth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-03 19:04:06.000000 pyjacket-0.1.6/pyjacket/arrtools/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-03 19:04:06.000000 pyjacket-0.1.6/pyjacket/arrtools/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-03 19:04:06.000000 pyjacket-0.1.6/pyjacket/arrtools/rois.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-03 19:04:06.000000 pyjacket-0.1.6/pyjacket/arrtools/sizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-03 19:04:06.000000 pyjacket-0.1.6/pyjacket/arrtools/skeletonize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-03 19:04:06.000000 pyjacket-0.1.6/pyjacket/arrtools/slicing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-03 19:04:06.000000 pyjacket-0.1.6/pyjacket/arrtools/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:04:10.216310 pyjacket-0.1.6/pyjacket/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-03 19:04:06.000000 pyjacket-0.1.6/pyjacket/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-03 19:04:06.000000 pyjacket-0.1.6/pyjacket/core/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-03 19:04:06.000000 pyjacket-0.1.6/pyjacket/core/digits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-03 19:04:06.000000 pyjacket-0.1.6/pyjacket/core/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-03 19:04:06.000000 pyjacket-0.1.6/pyjacket/core/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-03 19:04:06.000000 pyjacket-0.1.6/pyjacket/core/indexing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-03 19:04:06.000000 pyjacket-0.1.6/pyjacket/core/iterations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-03 19:04:06.000000 pyjacket-0.1.6/pyjacket/core/numbers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-03 19:04:06.000000 pyjacket-0.1.6/pyjacket/core/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 19:04:06.000000 pyjacket-0.1.6/pyjacket/core/sorting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:04:10.216310 pyjacket-0.1.6/pyjacket/cvtools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 19:04:06.000000 pyjacket-0.1.6/pyjacket/cvtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-03 19:04:06.000000 pyjacket-0.1.6/pyjacket/cvtools/color_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-03 19:04:06.000000 pyjacket-0.1.6/pyjacket/cvtools/color_picker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-03 19:04:06.000000 pyjacket-0.1.6/pyjacket/cvtools/color_slicing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:04:10.216310 pyjacket-0.1.6/pyjacket/filetools/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-03 19:04:06.000000 pyjacket-0.1.6/pyjacket/filetools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:04:10.220310 pyjacket-0.1.6/pyjacket/filetools/_imread/
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-03 19:04:06.000000 pyjacket-0.1.6/pyjacket/filetools/_imread/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-04-03 19:04:06.000000 pyjacket-0.1.6/pyjacket/filetools/_imread/imread_nd2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-03 19:04:06.000000 pyjacket-0.1.6/pyjacket/filetools/_imread/imread_tif.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-03 19:04:06.000000 pyjacket-0.1.6/pyjacket/filetools/_imread/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:04:10.220310 pyjacket-0.1.6/pyjacket/filetools/_imwrite/
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-03 19:04:06.000000 pyjacket-0.1.6/pyjacket/filetools/_imwrite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-03 19:04:06.000000 pyjacket-0.1.6/pyjacket/filetools/_imwrite/imwrite_tif.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-04-03 19:04:06.000000 pyjacket-0.1.6/pyjacket/filetools/filemanager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:04:10.220310 pyjacket-0.1.6/pyjacket/graphs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 19:04:06.000000 pyjacket-0.1.6/pyjacket/graphs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-03 19:04:06.000000 pyjacket-0.1.6/pyjacket/graphs/absorbing_markov.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-03 19:04:06.000000 pyjacket-0.1.6/pyjacket/graphs/markov.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:04:10.220310 pyjacket-0.1.6/pyjacket/ntheory/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-03 19:04:06.000000 pyjacket-0.1.6/pyjacket/ntheory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-03 19:04:06.000000 pyjacket-0.1.6/pyjacket/ntheory/factors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:04:10.220310 pyjacket-0.1.6/pyjacket/ntheory/modulo/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-03 19:04:06.000000 pyjacket-0.1.6/pyjacket/ntheory/modulo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-03 19:04:06.000000 pyjacket-0.1.6/pyjacket/ntheory/modulo/modular_arithmetic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:04:10.220310 pyjacket-0.1.6/pyjacket/ntheory/primes/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-03 19:04:06.000000 pyjacket-0.1.6/pyjacket/ntheory/primes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-03 19:04:06.000000 pyjacket-0.1.6/pyjacket/ntheory/primes/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-03 19:04:06.000000 pyjacket-0.1.6/pyjacket/ntheory/primes/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:04:10.220310 pyjacket-0.1.6/pyjacket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-03 19:04:10.000000 pyjacket-0.1.6/pyjacket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-03 19:04:10.000000 pyjacket-0.1.6/pyjacket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:04:10.000000 pyjacket-0.1.6/pyjacket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 19:04:10.000000 pyjacket-0.1.6/pyjacket.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:04:10.220310 pyjacket-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-03 19:04:06.000000 pyjacket-0.1.6/setup.py
```

### Comparing `pyjacket-0.1.4/LICENSE` & `pyjacket-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjacket-0.1.4/pyjacket/arrtools/arrtools.py` & `pyjacket-0.1.6/pyjacket/arrtools/arrtools.py`

 * *Files identical despite different names*

### Comparing `pyjacket-0.1.4/pyjacket/arrtools/bitdepth.py` & `pyjacket-0.1.6/pyjacket/arrtools/bitdepth.py`

 * *Files identical despite different names*

### Comparing `pyjacket-0.1.4/pyjacket/arrtools/display.py` & `pyjacket-0.1.6/pyjacket/arrtools/display.py`

 * *Files identical despite different names*

### Comparing `pyjacket-0.1.4/pyjacket/arrtools/filters.py` & `pyjacket-0.1.6/pyjacket/arrtools/filters.py`

 * *Files identical despite different names*

### Comparing `pyjacket-0.1.4/pyjacket/arrtools/rois.py` & `pyjacket-0.1.6/pyjacket/arrtools/rois.py`

 * *Files identical despite different names*

### Comparing `pyjacket-0.1.4/pyjacket/arrtools/skeletonize.py` & `pyjacket-0.1.6/pyjacket/arrtools/skeletonize.py`

 * *Files identical despite different names*

### Comparing `pyjacket-0.1.4/pyjacket/arrtools/slicing.py` & `pyjacket-0.1.6/pyjacket/arrtools/slicing.py`

 * *Files identical despite different names*

### Comparing `pyjacket-0.1.4/pyjacket/core/find_nth.py` & `pyjacket-0.1.6/pyjacket/core/indexing.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 def index_nth(iterable: list, element, n: int=-1) -> int:
-    """Find nth (default: last) occurence of element in iterable."""    
+    """Find index of nth (default: last) occurence of element in iterable."""    
     if n == 0:
         raise ValueError(f"n must be nonzero")
 
     if n < 0:  
         idx = len(iterable) - index_nth(iterable[::-1], element, -n) - 1
     
     else:
@@ -11,16 +11,16 @@
         while idx >= 0 and n > 1:
             idx = iterable.index(element, idx+1)
             n -= 1
             
     return idx
 
 
-def index_nth(s: str, *args, **kwargs):
-    return s.rfind(*args, **kwargs)
+# def index_nth(s: str, *args, **kwargs):
+#     return s.rfind(*args, **kwargs)
 
 
 def main():
     
     x = []
     y = 0
     z = -1
```

### Comparing `pyjacket-0.1.4/pyjacket/core/rounding.py` & `pyjacket-0.1.6/pyjacket/core/numbers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from math import floor, log10
+from math import floor, log
 
 def sign(x):
     return (-1, 1)[x >= 0]
 
-def order10(x):
+def order(x, base=10):
     """Order of a magnitude belong to a number (base 10)"""
-    return int(floor(log10(abs(x))))
+    return int(floor(log(abs(x), base)))
 
 def truncate(x, n):
     """Remove any floating points"""
     return int(x * 10**n) / 10**n
 
 def round_significant(x, n):
     """Round the number to nearest significant digits"""
-    return round(x, n - order10(x) - 1)
+    return round(x, n - order(x) - 1)
 
 def truncate_significant(x, n, count_zero=False):
     """Round the number down to desired significant digits"""
     _type = type(x)
     x = str(float(x))
     
     digits = list(x)
@@ -36,19 +36,19 @@
     assert sign(-10) == -1
     assert sign(-1e99) == -1
     assert sign(0) == 1
     assert sign(0.000001) == 1
     assert sign(-1e-10) == -1
     assert sign(1e10) == 1
         
-    assert order10(100) == 2
-    assert order10(999) == 2
-    assert order10(3) == 0
-    assert order10(0.2) == -1
-    assert order10(-10) == 1
+    assert order(100) == 2
+    assert order(999) == 2
+    assert order(3) == 0
+    assert order(0.2) == -1
+    assert order(-10) == 1
             
     assert truncate(123.1433, 2) == 123.14    
     assert truncate(0.1433, 2) == 0.14    
     assert truncate(-0.5464933, 4) == -0.5464
         
     assert round_significant(123457, 3) == 123000
     assert round_significant(-123457, 4) == -123500
```

### Comparing `pyjacket-0.1.4/pyjacket/cvtools/color_picker.py` & `pyjacket-0.1.6/pyjacket/cvtools/color_picker.py`

 * *Files identical despite different names*

### Comparing `pyjacket-0.1.4/pyjacket/filetools/_imread/__init__.py` & `pyjacket-0.1.6/pyjacket/filetools/_imread/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjacket-0.1.4/pyjacket/filetools/_imread/imread_nd2.py` & `pyjacket-0.1.6/pyjacket/filetools/_imread/imread_nd2.py`

 * *Files identical despite different names*

### Comparing `pyjacket-0.1.4/pyjacket/filetools/_imwrite/__init__.py` & `pyjacket-0.1.6/pyjacket/filetools/_imwrite/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjacket-0.1.4/pyjacket/filetools/filemanager.py` & `pyjacket-0.1.6/pyjacket/filetools/filemanager.py`

 * *Files identical despite different names*

### Comparing `pyjacket-0.1.4/pyjacket/graphs/absorbing_markov.py` & `pyjacket-0.1.6/pyjacket/graphs/absorbing_markov.py`

 * *Files identical despite different names*

### Comparing `pyjacket-0.1.4/pyjacket/graphs/markov.py` & `pyjacket-0.1.6/pyjacket/graphs/markov.py`

 * *Files identical despite different names*

### Comparing `pyjacket-0.1.4/pyjacket/ntheory/factors.py` & `pyjacket-0.1.6/pyjacket/ntheory/factors.py`

 * *Files identical despite different names*

### Comparing `pyjacket-0.1.4/pyjacket/ntheory/modulo/modular_arithmetic.py` & `pyjacket-0.1.6/pyjacket/ntheory/modulo/modular_arithmetic.py`

 * *Files identical despite different names*

### Comparing `pyjacket-0.1.4/pyjacket/ntheory/primes/core.py` & `pyjacket-0.1.6/pyjacket/ntheory/primes/core.py`

 * *Files identical despite different names*

### Comparing `pyjacket-0.1.4/pyjacket/ntheory/primes/generate.py` & `pyjacket-0.1.6/pyjacket/ntheory/primes/generate.py`

 * *Files identical despite different names*

### Comparing `pyjacket-0.1.4/pyjacket.egg-info/SOURCES.txt` & `pyjacket-0.1.6/pyjacket.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,35 @@
 LICENSE
 README.md
 setup.py
 pyjacket/__init__.py
-pyjacket/setup.py
 pyjacket.egg-info/PKG-INFO
 pyjacket.egg-info/SOURCES.txt
 pyjacket.egg-info/dependency_links.txt
 pyjacket.egg-info/top_level.txt
 pyjacket/arrtools/__init__.py
 pyjacket/arrtools/arrtools.py
 pyjacket/arrtools/bitdepth.py
 pyjacket/arrtools/display.py
 pyjacket/arrtools/filters.py
 pyjacket/arrtools/rois.py
 pyjacket/arrtools/sizing.py
 pyjacket/arrtools/skeletonize.py
 pyjacket/arrtools/slicing.py
 pyjacket/arrtools/wrappers.py
-pyjacket/chemistry/__init__.py
 pyjacket/core/__init__.py
-pyjacket/core/all_same.py
-pyjacket/core/batched.py
+pyjacket/core/collections.py
 pyjacket/core/digits.py
 pyjacket/core/filters.py
-pyjacket/core/find_nth.py
 pyjacket/core/format.py
+pyjacket/core/indexing.py
 pyjacket/core/iterations.py
+pyjacket/core/numbers.py
 pyjacket/core/operators.py
-pyjacket/core/python_ext.py
-pyjacket/core/rounding.py
-pyjacket/core/sortby.py
-pyjacket/core/test.py
+pyjacket/core/sorting.py
 pyjacket/cvtools/__init__.py
 pyjacket/cvtools/color_filter.py
 pyjacket/cvtools/color_picker.py
 pyjacket/cvtools/color_slicing.py
 pyjacket/filetools/__init__.py
 pyjacket/filetools/filemanager.py
 pyjacket/filetools/_imread/__init__.py
```

### Comparing `pyjacket-0.1.4/setup.py` & `pyjacket-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-__version__ = '0.1.4'
+__version__ = '0.1.6'
 
 GIT_USER = 'Kasper-Arfman'
 NAME = 'pyjacket'
 
 setuptools.setup(
     name=NAME,
     version=__version__,
```

