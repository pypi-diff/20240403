# Comparing `tmp/python-CIAM-1.1.2.tar.gz` & `tmp/python-CIAM-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-CIAM-1.1.2.tar", last modified: Wed Mar 22 02:13:56 2023, max compression
+gzip compressed data, was "python-CIAM-1.2.tar", last modified: Wed Apr  3 04:16:39 2024, max compression
```

## Comparing `python-CIAM-1.1.2.tar` & `python-CIAM-1.2.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 02:13:56.355598 python-CIAM-1.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 02:13:56.347597 python-CIAM-1.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 02:13:56.351597 python-CIAM-1.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-03-22 02:13:44.000000 python-CIAM-1.1.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-22 02:13:44.000000 python-CIAM-1.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-03-22 02:13:44.000000 python-CIAM-1.1.2/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-03-22 02:13:44.000000 python-CIAM-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11091 2023-03-22 02:13:56.355598 python-CIAM-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10559 2023-03-22 02:13:44.000000 python-CIAM-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 02:13:56.351597 python-CIAM-1.1.2/environment/
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-03-22 02:13:44.000000 python-CIAM-1.1.2/environment/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 02:13:56.351597 python-CIAM-1.1.2/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-03-22 02:13:44.000000 python-CIAM-1.1.2/notebooks/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    23374 2023-03-22 02:13:44.000000 python-CIAM-1.1.2/notebooks/data-acquisition.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 02:13:56.351597 python-CIAM-1.1.2/notebooks/data-processing/
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-03-22 02:13:44.000000 python-CIAM-1.1.2/notebooks/data-processing/collapse-sliiders-to-seg.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    15420 2023-03-22 02:13:44.000000 python-CIAM-1.1.2/notebooks/data-processing/create-diaz-pyCIAM-inputs.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 02:13:56.351597 python-CIAM-1.1.2/notebooks/data-processing/slr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 02:13:56.351597 python-CIAM-1.1.2/notebooks/data-processing/slr/AR5/
--rw-r--r--   0 runner    (1001) docker     (123)     7946 2023-03-22 02:13:44.000000 python-CIAM-1.1.2/notebooks/data-processing/slr/AR5/1-convert-mat-version.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    50648 2023-03-22 02:13:44.000000 python-CIAM-1.1.2/notebooks/data-processing/slr/AR5/2-generate-projected-lsl.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8695 2023-03-22 02:13:44.000000 python-CIAM-1.1.2/notebooks/data-processing/slr/AR5/3-retrieve-num-gcms.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    29008 2023-03-22 02:13:44.000000 python-CIAM-1.1.2/notebooks/data-processing/slr/AR5/4-process-localizesl-output.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-03-22 02:13:44.000000 python-CIAM-1.1.2/notebooks/data-processing/slr/AR5/5-create-slr-quantile.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-03-22 02:13:44.000000 python-CIAM-1.1.2/notebooks/data-processing/slr/AR5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     7630 2023-03-22 02:13:44.000000 python-CIAM-1.1.2/notebooks/data-processing/slr/AR6.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8475 2023-03-22 02:13:44.000000 python-CIAM-1.1.2/notebooks/data-processing/slr/sweet.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 02:13:56.351597 python-CIAM-1.1.2/notebooks/models/
--rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-03-22 02:13:44.000000 python-CIAM-1.1.2/notebooks/models/create-surge-lookup-tables.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    87298 2023-03-22 02:13:44.000000 python-CIAM-1.1.2/notebooks/models/fit-movefactor.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    17483 2023-03-22 02:13:44.000000 python-CIAM-1.1.2/notebooks/models/run-pyCIAM-diaz2016.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-03-22 02:13:44.000000 python-CIAM-1.1.2/notebooks/models/run-pyCIAM-slrquantiles.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 02:13:56.351597 python-CIAM-1.1.2/notebooks/nb_logs/
--rw-r--r--   0 runner    (1001) docker     (123)    26214 2023-03-22 02:13:44.000000 python-CIAM-1.1.2/notebooks/nb_logs/data-acquisition.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 02:13:56.347597 python-CIAM-1.1.2/notebooks/nb_logs/data-processing/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 02:13:56.351597 python-CIAM-1.1.2/notebooks/nb_logs/data-processing/slr/
--rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-03-22 02:13:44.000000 python-CIAM-1.1.2/notebooks/nb_logs/data-processing/slr/AR6.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 02:13:56.351597 python-CIAM-1.1.2/notebooks/nb_logs/models/
--rw-r--r--   0 runner    (1001) docker     (123)    43127 2023-03-22 02:13:44.000000 python-CIAM-1.1.2/notebooks/nb_logs/models/run-pyCIAM-slrquantiles.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 02:13:56.355598 python-CIAM-1.1.2/notebooks/post-processing/
--rw-r--r--   0 runner    (1001) docker     (123)   205399 2023-03-22 02:13:44.000000 python-CIAM-1.1.2/notebooks/post-processing/pyCIAM-results-figures.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    16359 2023-03-22 02:13:44.000000 python-CIAM-1.1.2/notebooks/post-processing/zenodo-upload.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-03-22 02:13:44.000000 python-CIAM-1.1.2/notebooks/run_example.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-03-22 02:13:44.000000 python-CIAM-1.1.2/notebooks/run_full_replication.sh
--rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-03-22 02:13:44.000000 python-CIAM-1.1.2/notebooks/shared.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-03-22 02:13:44.000000 python-CIAM-1.1.2/params.json
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-03-22 02:13:44.000000 python-CIAM-1.1.2/params_diaz.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 02:13:56.355598 python-CIAM-1.1.2/pyCIAM/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-03-22 02:13:44.000000 python-CIAM-1.1.2/pyCIAM/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-03-22 02:13:44.000000 python-CIAM-1.1.2/pyCIAM/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    30590 2023-03-22 02:13:44.000000 python-CIAM-1.1.2/pyCIAM/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    63211 2023-03-22 02:13:44.000000 python-CIAM-1.1.2/pyCIAM/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 02:13:56.355598 python-CIAM-1.1.2/pyCIAM/surge/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-22 02:13:44.000000 python-CIAM-1.1.2/pyCIAM/surge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-03-22 02:13:44.000000 python-CIAM-1.1.2/pyCIAM/surge/_calc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-03-22 02:13:44.000000 python-CIAM-1.1.2/pyCIAM/surge/damage_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17900 2023-03-22 02:13:44.000000 python-CIAM-1.1.2/pyCIAM/surge/lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)    10498 2023-03-22 02:13:44.000000 python-CIAM-1.1.2/pyCIAM/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-03-22 02:13:44.000000 python-CIAM-1.1.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 02:13:56.355598 python-CIAM-1.1.2/python_CIAM.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11091 2023-03-22 02:13:56.000000 python-CIAM-1.1.2/python_CIAM.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-03-22 02:13:56.000000 python-CIAM-1.1.2/python_CIAM.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 02:13:56.000000 python-CIAM-1.1.2/python_CIAM.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-22 02:13:56.000000 python-CIAM-1.1.2/python_CIAM.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-03-22 02:13:56.355598 python-CIAM-1.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:16:39.891930 python-CIAM-1.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:16:39.879929 python-CIAM-1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:16:39.883930 python-CIAM-1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-03 04:16:32.000000 python-CIAM-1.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-03 04:16:32.000000 python-CIAM-1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-03 04:16:32.000000 python-CIAM-1.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-03 04:16:32.000000 python-CIAM-1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-04-03 04:16:39.891930 python-CIAM-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10559 2024-04-03 04:16:32.000000 python-CIAM-1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:16:39.883930 python-CIAM-1.2/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-03 04:16:32.000000 python-CIAM-1.2/environment/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:16:39.883930 python-CIAM-1.2/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-04-03 04:16:32.000000 python-CIAM-1.2/notebooks/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    23396 2024-04-03 04:16:32.000000 python-CIAM-1.2/notebooks/data-acquisition.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:16:39.883930 python-CIAM-1.2/notebooks/data-processing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-03 04:16:32.000000 python-CIAM-1.2/notebooks/data-processing/collapse-sliiders-to-seg.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    15420 2024-04-03 04:16:32.000000 python-CIAM-1.2/notebooks/data-processing/create-diaz-pyCIAM-inputs.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:16:39.883930 python-CIAM-1.2/notebooks/data-processing/slr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:16:39.887930 python-CIAM-1.2/notebooks/data-processing/slr/AR5/
+-rw-r--r--   0 runner    (1001) docker     (127)     7946 2024-04-03 04:16:32.000000 python-CIAM-1.2/notebooks/data-processing/slr/AR5/1-convert-mat-version.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    50648 2024-04-03 04:16:32.000000 python-CIAM-1.2/notebooks/data-processing/slr/AR5/2-generate-projected-lsl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8695 2024-04-03 04:16:32.000000 python-CIAM-1.2/notebooks/data-processing/slr/AR5/3-retrieve-num-gcms.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    29008 2024-04-03 04:16:32.000000 python-CIAM-1.2/notebooks/data-processing/slr/AR5/4-process-localizesl-output.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-03 04:16:32.000000 python-CIAM-1.2/notebooks/data-processing/slr/AR5/5-create-slr-quantile.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-03 04:16:32.000000 python-CIAM-1.2/notebooks/data-processing/slr/AR5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7630 2024-04-03 04:16:32.000000 python-CIAM-1.2/notebooks/data-processing/slr/AR6.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-04-03 04:16:32.000000 python-CIAM-1.2/notebooks/data-processing/slr/sweet.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:16:39.887930 python-CIAM-1.2/notebooks/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     8294 2024-04-03 04:16:32.000000 python-CIAM-1.2/notebooks/models/create-surge-lookup-tables.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   106928 2024-04-03 04:16:32.000000 python-CIAM-1.2/notebooks/models/fit-movefactor.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    17483 2024-04-03 04:16:32.000000 python-CIAM-1.2/notebooks/models/run-pyCIAM-diaz2016.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-03 04:16:32.000000 python-CIAM-1.2/notebooks/models/run-pyCIAM-slrquantiles.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:16:39.887930 python-CIAM-1.2/notebooks/nb_logs/
+-rw-r--r--   0 runner    (1001) docker     (127)    26214 2024-04-03 04:16:32.000000 python-CIAM-1.2/notebooks/nb_logs/data-acquisition.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:16:39.879929 python-CIAM-1.2/notebooks/nb_logs/data-processing/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:16:39.887930 python-CIAM-1.2/notebooks/nb_logs/data-processing/slr/
+-rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-04-03 04:16:32.000000 python-CIAM-1.2/notebooks/nb_logs/data-processing/slr/AR6.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:16:39.887930 python-CIAM-1.2/notebooks/nb_logs/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    43127 2024-04-03 04:16:32.000000 python-CIAM-1.2/notebooks/nb_logs/models/run-pyCIAM-slrquantiles.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:16:39.887930 python-CIAM-1.2/notebooks/post-processing/
+-rw-r--r--   0 runner    (1001) docker     (127)   205399 2024-04-03 04:16:32.000000 python-CIAM-1.2/notebooks/post-processing/pyCIAM-results-figures.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    19503 2024-04-03 04:16:32.000000 python-CIAM-1.2/notebooks/post-processing/zenodo-upload.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-03 04:16:32.000000 python-CIAM-1.2/notebooks/run_example.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-03 04:16:32.000000 python-CIAM-1.2/notebooks/run_full_replication.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-04-03 04:16:32.000000 python-CIAM-1.2/notebooks/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-04-03 04:16:32.000000 python-CIAM-1.2/params.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-04-03 04:16:32.000000 python-CIAM-1.2/params_diaz.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:16:39.887930 python-CIAM-1.2/pyCIAM/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-03 04:16:32.000000 python-CIAM-1.2/pyCIAM/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-03 04:16:32.000000 python-CIAM-1.2/pyCIAM/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30556 2024-04-03 04:16:32.000000 python-CIAM-1.2/pyCIAM/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63617 2024-04-03 04:16:32.000000 python-CIAM-1.2/pyCIAM/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:16:39.891930 python-CIAM-1.2/pyCIAM/surge/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-03 04:16:32.000000 python-CIAM-1.2/pyCIAM/surge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-04-03 04:16:32.000000 python-CIAM-1.2/pyCIAM/surge/_calc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-03 04:16:32.000000 python-CIAM-1.2/pyCIAM/surge/damage_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17909 2024-04-03 04:16:32.000000 python-CIAM-1.2/pyCIAM/surge/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-04-03 04:16:32.000000 python-CIAM-1.2/pyCIAM/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-03 04:16:32.000000 python-CIAM-1.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:16:39.891930 python-CIAM-1.2/python_CIAM.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-04-03 04:16:39.000000 python-CIAM-1.2/python_CIAM.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-03 04:16:39.000000 python-CIAM-1.2/python_CIAM.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 04:16:39.000000 python-CIAM-1.2/python_CIAM.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 04:16:39.000000 python-CIAM-1.2/python_CIAM.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-03 04:16:39.891930 python-CIAM-1.2/setup.cfg
```

### Comparing `python-CIAM-1.1.2/.github/workflows/python-publish.yml` & `python-CIAM-1.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `python-CIAM-1.1.2/.gitignore` & `python-CIAM-1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `python-CIAM-1.1.2/HISTORY.rst` & `python-CIAM-1.2/HISTORY.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 History
 =======
 
+v1.2.0
+------
+* Point `data-acquisition.ipynb` to updated Zenodo deposit that fixes the dtype of `subsets` variable in `diaz2016_inputs_raw.zarr.zip` to be bool rather than int8
+* Variable name bugfix in `data-acquisition.ipynb`
+* Add netcdf versions of SLIIDERS and the pyCIAM results to `upload-zenodo.ipynb`
+* Update results in Zenodo record to use SLIIDERS v1.2
+  
 v1.1.2
 ------
 * Update zenodo-upload.ipynb to include packages
 * Update readme to emphasize environment.yml
 
 v1.1.1
 ------
```

### Comparing `python-CIAM-1.1.2/LICENSE` & `python-CIAM-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-CIAM-1.1.2/PKG-INFO` & `python-CIAM-1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-CIAM
-Version: 1.1.2
+Version: 1.2
 Summary: An efficient Python implementation of the Coastal Impacts and Adaptation Model (CIAM)
 Home-page: https://gitlab.com/ClimateImpactLab/coastal/projects/pyciam
 Author: Ian Bolliger, Nicholas Depsky
 Author-email: ian.bolliger@blackrock.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `python-CIAM-1.1.2/README.md` & `python-CIAM-1.2/README.md`

 * *Files identical despite different names*

### Comparing `python-CIAM-1.1.2/environment/environment.yml` & `python-CIAM-1.2/environment/environment.yml`

 * *Files identical despite different names*

### Comparing `python-CIAM-1.1.2/notebooks/README.md` & `python-CIAM-1.2/notebooks/README.md`

 * *Files identical despite different names*

### Comparing `python-CIAM-1.1.2/notebooks/data-acquisition.ipynb` & `python-CIAM-1.2/notebooks/data-acquisition.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9983897588064254%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(32, ')\\n'), (33, '\\n'), (34, 'from pyCIAM.utils import "*

 * *            "copy')], delete: [33, 12]}}, 4: {'source': {insert: [(7, 'Z_PYCIAM_DOI = "*

 * *            '"8229860"\\n\'), (33, \'Z_URL_SLIIDERS_PC = Z_URL_RECORDS\')], delete: [33, 7]}}}',*

 * * "'metadata'": "{'language_info': {'version': '3.10.8'}}"}*

```diff
@@ -47,15 +47,14 @@
                 "\n",
                 "import numpy as np\n",
                 "import pandas as pd\n",
                 "import requests\n",
                 "from cartopy.io import shapereader\n",
                 "from fsspec import FSTimeoutError\n",
                 "from fsspec.implementations.zip import ZipFileSystem\n",
-                "from pyCIAM.utils import copy\n",
                 "from shared import (\n",
                 "    DIR_SHP,\n",
                 "    DIR_SLR_AR5_IFILES_RAW,\n",
                 "    DIR_SLR_AR6_RAW,\n",
                 "    DIR_SLR_SWEET_RAW,\n",
                 "    LOCALIZESL_COREFILES,\n",
                 "    LOCALIZESL_REV,\n",
@@ -68,15 +67,17 @@
                 "    PATH_SLIIDERS,\n",
                 "    PATH_SLIIDERS_INCOME_INTERMEDIATE_FILE,\n",
                 "    PATH_SLR_AR5_QUANTILES,\n",
                 "    PATH_SLR_GMSL_HIST_TIMESERIES,\n",
                 "    PATH_SLR_HIST_TREND_MAP,\n",
                 "    PATHS_SURGE_LOOKUP,\n",
                 "    save,\n",
-                ")"
+                ")\n",
+                "\n",
+                "from pyCIAM.utils import copy"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "id": "7e3d5ad1-a9e5-4b03-9dca-57b5b2098e4c",
             "metadata": {
@@ -89,15 +90,15 @@
                 "Z_URL_BASE = \"https://zenodo.org/api/\"\n",
                 "Z_URL_RECORDS = Z_URL_BASE + \"records/{doi}\"\n",
                 "Z_URL_DEPOSITS = Z_URL_BASE + \"deposit/depositions/{doi}\"\n",
                 "\n",
                 "# This will need to point to the correct version of the SLIIDERS zenodo store (see\n",
                 "# Depsky et al. 2023 for the version associated with that manuscript)\n",
                 "Z_SLIIDERS_DOI = \"7693868\"\n",
-                "Z_PYCIAM_DOI = \"7693869\"\n",
+                "Z_PYCIAM_DOI = \"8229860\"\n",
                 "Z_AR6_DOI = \"6382554\"\n",
                 "Z_SWEET_DOI = \"6067895\"\n",
                 "\n",
                 "\n",
                 "DOWNLOAD_DIAZ_INPUTS = True\n",
                 "DOWNLOAD_SLIIDERS = True\n",
                 "DOWNLOAD_SURGE_LOOKUPS = True\n",
@@ -115,15 +116,15 @@
                 "\n",
                 "# pre-release\n",
                 "# PARAMS = {\"access_token\": environ[\"ACCESS_TOKEN\"]}\n",
                 "# Z_URL_SLIIDERS_PC = Z_URL_DEPOSITS\n",
                 "\n",
                 "# post-release\n",
                 "PARAMS = {}\n",
-                "Z_URL = Z_URL_RECORDS"
+                "Z_URL_SLIIDERS_PC = Z_URL_RECORDS"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 49,
             "id": "8d519f83-eb91-4cb0-b2e7-5918b91d5143",
             "metadata": {
@@ -623,15 +624,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.10"
+            "version": "3.10.8"
         },
         "widgets": {
             "application/vnd.jupyter.widget-state+json": {
                 "state": {},
                 "version_major": 2,
                 "version_minor": 0
             }
```

### Comparing `python-CIAM-1.1.2/notebooks/data-processing/collapse-sliiders-to-seg.ipynb` & `python-CIAM-1.2/notebooks/data-processing/collapse-sliiders-to-seg.ipynb`

 * *Files identical despite different names*

### Comparing `python-CIAM-1.1.2/notebooks/data-processing/create-diaz-pyCIAM-inputs.ipynb` & `python-CIAM-1.2/notebooks/data-processing/create-diaz-pyCIAM-inputs.ipynb`

 * *Files identical despite different names*

### Comparing `python-CIAM-1.1.2/notebooks/data-processing/slr/AR5/1-convert-mat-version.ipynb` & `python-CIAM-1.2/notebooks/data-processing/slr/AR5/1-convert-mat-version.ipynb`

 * *Files identical despite different names*

### Comparing `python-CIAM-1.1.2/notebooks/data-processing/slr/AR5/2-generate-projected-lsl.ipynb` & `python-CIAM-1.2/notebooks/data-processing/slr/AR5/2-generate-projected-lsl.ipynb`

 * *Files identical despite different names*

### Comparing `python-CIAM-1.1.2/notebooks/data-processing/slr/AR5/3-retrieve-num-gcms.ipynb` & `python-CIAM-1.2/notebooks/data-processing/slr/AR5/3-retrieve-num-gcms.ipynb`

 * *Files identical despite different names*

### Comparing `python-CIAM-1.1.2/notebooks/data-processing/slr/AR5/4-process-localizesl-output.ipynb` & `python-CIAM-1.2/notebooks/data-processing/slr/AR5/4-process-localizesl-output.ipynb`

 * *Files identical despite different names*

### Comparing `python-CIAM-1.1.2/notebooks/data-processing/slr/AR5/5-create-slr-quantile.ipynb` & `python-CIAM-1.2/notebooks/data-processing/slr/AR5/5-create-slr-quantile.ipynb`

 * *Files identical despite different names*

### Comparing `python-CIAM-1.1.2/notebooks/data-processing/slr/AR5/README.md` & `python-CIAM-1.2/notebooks/data-processing/slr/AR5/README.md`

 * *Files identical despite different names*

### Comparing `python-CIAM-1.1.2/notebooks/data-processing/slr/AR6.ipynb` & `python-CIAM-1.2/notebooks/data-processing/slr/AR6.ipynb`

 * *Files identical despite different names*

### Comparing `python-CIAM-1.1.2/notebooks/data-processing/slr/sweet.ipynb` & `python-CIAM-1.2/notebooks/data-processing/slr/sweet.ipynb`

 * *Files identical despite different names*

### Comparing `python-CIAM-1.1.2/notebooks/models/create-surge-lookup-tables.ipynb` & `python-CIAM-1.2/notebooks/models/create-surge-lookup-tables.ipynb`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9767096470985738%*

 * *Differences: {"'cells'": "{4: {'execution_count': 2, 'metadata': {replace: OrderedDict([('tags', [])])}}, 5: "*

 * *            "{'execution_count': 3, 'metadata': {replace: OrderedDict([('tags', [])])}, 'outputs': "*

 * *            "{0: {'text': "*

 * *            "['/srv/conda/envs/notebook/lib/python3.10/site-packages/google/cloud/storage/transfer_manager.py:30: "*

 * *            'UserWarning: The module `transfer_manager` is a preview feature. Functionality and '*

 * *            "API may change. This warning will be removed in a future r […]*

```diff
@@ -26,35 +26,60 @@
             "source": [
                 "## Setup"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
+            "id": "6b183aa3-366a-4f5f-bb95-5ef4bf48d438",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "%load_ext autoreload\n",
+                "%autoreload 2"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 2,
             "id": "cd4b2928-65a0-4733-9c71-fbefa85590be",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
                 "import sys\n",
                 "\n",
                 "sys.path.append(\"../\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 3,
             "id": "afd03880-8e46-4d81-867d-bfb6505ea788",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "/srv/conda/envs/notebook/lib/python3.9/site-packages/dask_gateway/client.py:21: FutureWarning: format_bytes is deprecated and will be removed in a future release. Please use dask.utils.format_bytes instead.\n",
-                        "  from distributed.utils import LoopRunner, format_bytes\n"
+                        "/srv/conda/envs/notebook/lib/python3.10/site-packages/google/cloud/storage/transfer_manager.py:30: UserWarning: The module `transfer_manager` is a preview feature. Functionality and API may change. This warning will be removed in a future release.\n",
+                        "  warnings.warn(\n",
+                        "/home/jovyan/git-repos/pyCIAM-public/notebooks/models/../shared.py:3: UserWarning: Shapely 2.0 is installed, but because PyGEOS is also installed, GeoPandas will still use PyGEOS by default for now. To force to use and test Shapely 2.0, you have to set the environment variable USE_PYGEOS=0. You can do this before starting the Python process, or in your code before importing geopandas:\n",
+                        "\n",
+                        "import os\n",
+                        "os.environ['USE_PYGEOS'] = '0'\n",
+                        "import geopandas\n",
+                        "\n",
+                        "In a future release, GeoPandas will switch to using Shapely by default. If you are using PyGEOS directly (calling PyGEOS functions on geometries from GeoPandas), this will then stop working and you are encouraged to migrate from PyGEOS to Shapely 2.0 (https://shapely.readthedocs.io/en/latest/migration_pygeos.html).\n",
+                        "  import geopandas as gpd\n"
                     ]
                 }
             ],
             "source": [
                 "import distributed as dd\n",
                 "import pandas as pd\n",
                 "from pyCIAM.surge import damage_funcs\n",
@@ -71,122 +96,85 @@
                 "    STORAGE_OPTIONS,\n",
                 "    start_dask_cluster,\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 4,
             "id": "47979c48-7fff-49b4-b445-ea6bf746fa37",
             "metadata": {
                 "tags": [
                     "parameters"
                 ]
             },
             "outputs": [],
             "source": [
                 "# When running on larger/scalable dask cluster, may wish to specify number of workers\n",
                 "# Default is LocalCluster which will use the number of CPUs available on local machine\n",
-                "# N_WORKERS_MIN = 7\n",
-                "# N_WORKERS_MAX = 700\n",
+                "N_WORKERS_MIN = 7\n",
+                "N_WORKERS_MAX = 700\n",
                 "SEG_CHUNKSIZE = 5\n",
                 "\n",
                 "PARAMS = pd.read_json(PATH_PARAMS)[\"values\"]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 5,
             "id": "6104bced",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
                 "DMF_I = getattr(damage_funcs, PARAMS.dmf + \"_i\")\n",
                 "DDF_I = getattr(damage_funcs, PARAMS.ddf + \"_i\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 6,
             "id": "dbb04b4a-14b8-4403-ad33-88bfe71bd8fc",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [
                 {
                     "data": {
-                        "text/html": [
-                            "<div>\n",
-                            "    <div style=\"width: 24px; height: 24px; background-color: #e1e1e1; border: 3px solid #9D9D9D; border-radius: 5px; position: absolute;\"> </div>\n",
-                            "    <div style=\"margin-left: 48px;\">\n",
-                            "        <h3 style=\"margin-bottom: 0px;\">Client</h3>\n",
-                            "        <p style=\"color: #9D9D9D; margin-bottom: 0px;\">Client-f992a2c6-c6d1-11ed-862e-665816eadc72</p>\n",
-                            "        <table style=\"width: 100%; text-align: left;\">\n",
-                            "\n",
-                            "        <tr>\n",
-                            "        \n",
-                            "            <td style=\"text-align: left;\"><strong>Connection method:</strong> Cluster object</td>\n",
-                            "            <td style=\"text-align: left;\"><strong>Cluster type:</strong> dask_gateway.GatewayCluster</td>\n",
-                            "        \n",
-                            "        </tr>\n",
-                            "\n",
-                            "        \n",
-                            "            <tr>\n",
-                            "                <td style=\"text-align: left;\">\n",
-                            "                    <strong>Dashboard: </strong> <a href=\"/services/dask-gateway/clusters/daskhub-dev.e0f56d1ca0ae4a42b9352ad6b7204454/status\" target=\"_blank\">/services/dask-gateway/clusters/daskhub-dev.e0f56d1ca0ae4a42b9352ad6b7204454/status</a>\n",
-                            "                </td>\n",
-                            "                <td style=\"text-align: left;\"></td>\n",
-                            "            </tr>\n",
-                            "        \n",
-                            "\n",
-                            "        </table>\n",
-                            "\n",
-                            "        \n",
-                            "            <details>\n",
-                            "            <summary style=\"margin-bottom: 20px;\"><h3 style=\"display: inline;\">Cluster Info</h3></summary>\n",
-                            "            <div style='background-color: #f2f2f2; display: inline-block; padding: 10px; border: 1px solid #999999;'>\n",
-                            "  <h3>GatewayCluster</h3>\n",
-                            "  <ul>\n",
-                            "    <li><b>Name: </b>daskhub-dev.e0f56d1ca0ae4a42b9352ad6b7204454\n",
-                            "    <li><b>Dashboard: </b><a href='/services/dask-gateway/clusters/daskhub-dev.e0f56d1ca0ae4a42b9352ad6b7204454/status' target='_blank'>/services/dask-gateway/clusters/daskhub-dev.e0f56d1ca0ae4a42b9352ad6b7204454/status</a>\n",
-                            "  </ul>\n",
-                            "</div>\n",
-                            "\n",
-                            "            </details>\n",
-                            "        \n",
-                            "\n",
-                            "    </div>\n",
-                            "</div>"
-                        ],
+                        "application/vnd.jupyter.widget-view+json": {
+                            "model_id": "fcadb94377b4430d9c2964ac9c808c2a",
+                            "version_major": 2,
+                            "version_minor": 0
+                        },
                         "text/plain": [
-                            "<Client: 'tls://10.4.102.2:8786' processes=0 threads=0, memory=0 B>"
+                            "VBox(children=(HTML(value='<h2>GatewayCluster</h2>'), HBox(children=(HTML(value='\\n<div>\\n<style scoped>\\n    \u2026"
                         ]
                     },
-                    "execution_count": 5,
                     "metadata": {},
-                    "output_type": "execute_result"
+                    "output_type": "display_data"
                 }
             ],
             "source": [
-                "client = start_dask_cluster(\n",
-                "    # n_workers_min=N_WORKERS_MIN,\n",
-                "    # n_workers_max=N_WORKERS_MAX,\n",
-                ")\n",
-                "client"
+                "client, cluster = start_dask_cluster()\n",
+                "cluster.adapt(minimum=N_WORKERS_MIN, maximum=N_WORKERS_MAX)\n",
+                "cluster"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "8cd85123-c954-41a4-9c50-13dbbbba8c97",
             "metadata": {},
             "source": [
                 "## Run surge damage calculations for each combo"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 7,
             "id": "1e823775-0d12-4e52-93d1-7e3586913e65",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "futs = {}\n",
@@ -201,15 +189,15 @@
                 "        PARAMS.n_interp_pts_rhdiff,\n",
                 "        DDF_I,\n",
                 "        DMF_I,\n",
                 "        quantiles=QUANTILES,\n",
                 "        start_year=PARAMS.model_start,\n",
                 "        slr_0_years=PARAMS.slr_0_year,\n",
                 "        client=client,\n",
-                "        # client_kwargs={\"batch_size\": N_WORKERS_MAX},\n",
+                "        client_kwargs={\"batch_size\": N_WORKERS_MAX},\n",
                 "        force_overwrite=True,\n",
                 "        seg_chunksize=SEG_CHUNKSIZE,\n",
                 "        mc_dim=\"quantile\",\n",
                 "        storage_options=STORAGE_OPTIONS,\n",
                 "    )"
             ]
         },
@@ -219,45 +207,49 @@
             "metadata": {},
             "source": [
                 "## Close"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 11,
             "id": "f941a509-7035-4105-8b79-88a97e759737",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
                 "# ensure completion and close cluster\n",
                 "all_futs = futs[\"seg\"] + futs[\"seg_adm\"]\n",
                 "dd.wait(all_futs)\n",
                 "assert [f.status == \"finished\" for f in all_futs]\n",
                 "finished = True"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 12,
             "id": "15563792-1ba0-435a-9981-e2b15eaa8dcd",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "(None, None)"
                         ]
                     },
-                    "execution_count": 10,
+                    "execution_count": 12,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "client.cluster.close(), client.close()"
+                "cluster.close(), client.close()"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
@@ -269,15 +261,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.10"
+            "version": "3.10.10"
         },
         "widgets": {
             "application/vnd.jupyter.widget-state+json": {
                 "state": {},
                 "version_major": 2,
                 "version_minor": 0
             }
```

### Comparing `python-CIAM-1.1.2/notebooks/models/fit-movefactor.ipynb` & `python-CIAM-1.2/notebooks/models/fit-movefactor.ipynb`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9771051311890306%*

 * *Differences: {"'cells'": "{3: {'metadata': {replace: OrderedDict([('tags', [])])}}, 4: {'metadata': {replace: "*

 * *            "OrderedDict([('tags', [])])}, 'outputs': {0: {'text': "*

 * *            "['/srv/conda/envs/notebook/lib/python3.10/site-packages/google/cloud/storage/transfer_manager.py:30: "*

 * *            'UserWarning: The module `transfer_manager` is a preview feature. Functionality and '*

 * *            "API may change. This warning will be removed in a future release.\\n', '  "*

 * *            "warnings.warn(\\n', "*

 * *       […]*

```diff
@@ -16,48 +16,72 @@
                 "This notebook uses the elbow method within a revealed preference context to fit the `movefactor` parameter, which defines the cost of relocating as a multiple of GDP. We evaluate the value of capital stock and the total population that immediately relocates under the optimal CIAM scenario using no-climate-change SLR projections and a middle of the road (SSP2) socioeconomic projection. The amount of immediate relocation of capital and population implies, by definition, that the present-day distribution of this capital and population is \"suboptimal\" within the CIAM framework. This suboptimality could be a function of (a) hidden costs/barriers to relocating that are not sufficiently valued within the existing relocation cost parameterization, and (b) data/parameter inaccuracy. As we start to increase the relocation cost parameter from 0, we see a sharp decline in the amount of immediately relocated population and capital, reflecting that there are real costs to moving. However, even with an implausibly high cost of relocation, we will still see some CIAM segments choose to immediately relocate in this no-climate-change scenario. We assume that this is due largely to (b). We develop a heuristic to estimate a reasonable `movefactor` by finding the value at which 50% of the capital and population that would immediately relocate under an assumption of 0 intangible relocation costs and optimal adaptation now stays put. We average the values obtained separately for population and capital stock. See associated paper for further details.\n",
                 "\n",
                 "We also evaluate how much capital is \"suboptimally\" located within the original GAMS-CIAM specification."
             ]
         },
         {
             "cell_type": "code",
+            "execution_count": 33,
+            "id": "4c531d79-a011-4f2b-b19c-9c6cc8c87680",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "%load_ext autoreload\n",
+                "%autoreload 2"
+            ]
+        },
+        {
+            "cell_type": "code",
             "execution_count": 1,
             "id": "4ac893fb-43ab-450f-9c82-6c9bf1b1d123",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
                 "import sys\n",
                 "\n",
                 "sys.path.append(\"../\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "id": "5e68d8e0-e7e8-404e-b51a-a4a4039a754d",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "/srv/conda/envs/notebook/lib/python3.9/site-packages/dask_gateway/client.py:21: FutureWarning: format_bytes is deprecated and will be removed in a future release. Please use dask.utils.format_bytes instead.\n",
-                        "  from distributed.utils import LoopRunner, format_bytes\n"
+                        "/srv/conda/envs/notebook/lib/python3.10/site-packages/google/cloud/storage/transfer_manager.py:30: UserWarning: The module `transfer_manager` is a preview feature. Functionality and API may change. This warning will be removed in a future release.\n",
+                        "  warnings.warn(\n",
+                        "/home/jovyan/git-repos/pyCIAM-public/notebooks/models/../shared.py:3: UserWarning: Shapely 2.0 is installed, but because PyGEOS is also installed, GeoPandas will still use PyGEOS by default for now. To force to use and test Shapely 2.0, you have to set the environment variable USE_PYGEOS=0. You can do this before starting the Python process, or in your code before importing geopandas:\n",
+                        "\n",
+                        "import os\n",
+                        "os.environ['USE_PYGEOS'] = '0'\n",
+                        "import geopandas\n",
+                        "\n",
+                        "In a future release, GeoPandas will switch to using Shapely by default. If you are using PyGEOS directly (calling PyGEOS functions on geometries from GeoPandas), this will then stop working and you are encouraged to migrate from PyGEOS to Shapely 2.0 (https://shapely.readthedocs.io/en/latest/migration_pygeos.html).\n",
+                        "  import geopandas as gpd\n"
                     ]
                 }
             ],
             "source": [
                 "import numpy as np\n",
                 "import pandas as pd\n",
                 "import xarray as xr\n",
                 "from matplotlib import pyplot as plt\n",
                 "from pyCIAM.constants import SOLVCASES\n",
                 "from pyCIAM.io import load_ciam_inputs, load_diaz_inputs\n",
                 "from pyCIAM.run import calc_costs\n",
-                "from rhg_compute_tools.xarray import dataarray_from_delayed\n",
                 "from shared import (\n",
                 "    PATH_DIAZ_INPUTS_INT,\n",
                 "    PATH_MOVEFACTOR_DATA,\n",
                 "    PATH_PARAMS,\n",
                 "    PATH_PARAMS_DIAZ,\n",
                 "    PATH_REFA,\n",
                 "    PATH_SLIIDERS_SEG,\n",
@@ -80,16 +104,16 @@
                     "parameters"
                 ]
             },
             "outputs": [],
             "source": [
                 "# When running on larger/scalable dask cluster, may wish to specify number of workers\n",
                 "# Default is LocalCluster which will use the number of CPUs available on local machine\n",
-                "# N_WORKERS_MIN = 7\n",
-                "# N_WORKERS_MAX = 700\n",
+                "N_WORKERS_MIN = 7\n",
+                "N_WORKERS_MAX = 700\n",
                 "SEG_CHUNKSIZE = 500\n",
                 "SEG_CHUNKSIZE_DIAZ = 4050\n",
                 "\n",
                 "MOVEFACTOR_RANGE = np.concatenate((np.arange(0, 50, 0.1), [50, 60, 70, 80, 90, 100]))\n",
                 "\n",
                 "DESCRIPTION = (\n",
                 "    \"Amount of immediately relocated capital and population under optimal adaptation \"\n",
@@ -108,79 +132,40 @@
             "id": "78ebf879-55ff-4117-ad8e-a939306f80f4",
             "metadata": {
                 "tags": []
             },
             "outputs": [
                 {
                     "data": {
-                        "text/html": [
-                            "<div>\n",
-                            "    <div style=\"width: 24px; height: 24px; background-color: #e1e1e1; border: 3px solid #9D9D9D; border-radius: 5px; position: absolute;\"> </div>\n",
-                            "    <div style=\"margin-left: 48px;\">\n",
-                            "        <h3 style=\"margin-bottom: 0px;\">Client</h3>\n",
-                            "        <p style=\"color: #9D9D9D; margin-bottom: 0px;\">Client-717fc8a7-c6da-11ed-86c1-665816eadc72</p>\n",
-                            "        <table style=\"width: 100%; text-align: left;\">\n",
-                            "\n",
-                            "        <tr>\n",
-                            "        \n",
-                            "            <td style=\"text-align: left;\"><strong>Connection method:</strong> Cluster object</td>\n",
-                            "            <td style=\"text-align: left;\"><strong>Cluster type:</strong> dask_gateway.GatewayCluster</td>\n",
-                            "        \n",
-                            "        </tr>\n",
-                            "\n",
-                            "        \n",
-                            "            <tr>\n",
-                            "                <td style=\"text-align: left;\">\n",
-                            "                    <strong>Dashboard: </strong> <a href=\"/services/dask-gateway/clusters/daskhub-dev.bfad7ebc4a904320b41301d11dd74af6/status\" target=\"_blank\">/services/dask-gateway/clusters/daskhub-dev.bfad7ebc4a904320b41301d11dd74af6/status</a>\n",
-                            "                </td>\n",
-                            "                <td style=\"text-align: left;\"></td>\n",
-                            "            </tr>\n",
-                            "        \n",
-                            "\n",
-                            "        </table>\n",
-                            "\n",
-                            "        \n",
-                            "            <details>\n",
-                            "            <summary style=\"margin-bottom: 20px;\"><h3 style=\"display: inline;\">Cluster Info</h3></summary>\n",
-                            "            <div style='background-color: #f2f2f2; display: inline-block; padding: 10px; border: 1px solid #999999;'>\n",
-                            "  <h3>GatewayCluster</h3>\n",
-                            "  <ul>\n",
-                            "    <li><b>Name: </b>daskhub-dev.bfad7ebc4a904320b41301d11dd74af6\n",
-                            "    <li><b>Dashboard: </b><a href='/services/dask-gateway/clusters/daskhub-dev.bfad7ebc4a904320b41301d11dd74af6/status' target='_blank'>/services/dask-gateway/clusters/daskhub-dev.bfad7ebc4a904320b41301d11dd74af6/status</a>\n",
-                            "  </ul>\n",
-                            "</div>\n",
-                            "\n",
-                            "            </details>\n",
-                            "        \n",
-                            "\n",
-                            "    </div>\n",
-                            "</div>"
-                        ],
+                        "application/vnd.jupyter.widget-view+json": {
+                            "model_id": "f5cbacc0097d400084b03c03ee4edb72",
+                            "version_major": 2,
+                            "version_minor": 0
+                        },
                         "text/plain": [
-                            "<Client: 'tls://10.4.102.3:8786' processes=0 threads=0, memory=0 B>"
+                            "VBox(children=(HTML(value='<h2>GatewayCluster</h2>'), HBox(children=(HTML(value='\\n<div>\\n<style scoped>\\n    \u2026"
                         ]
                     },
-                    "execution_count": 4,
                     "metadata": {},
-                    "output_type": "execute_result"
+                    "output_type": "display_data"
                 }
             ],
             "source": [
-                "client = start_dask_cluster(\n",
-                "    # n_workers_min=N_WORKERS_MIN,\n",
-                "    # n_workers_max=N_WORKERS_MAX\n",
-                ")\n",
-                "client"
+                "client, cluster = start_dask_cluster()\n",
+                "cluster.adapt(minimum=N_WORKERS_MIN, maximum=N_WORKERS_MAX)\n",
+                "cluster"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 5,
             "id": "e0679df9-312d-4813-99aa-2e3513ca503b",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
                 "def get_model_kwargs(diaz):\n",
                 "    return dict(\n",
                 "        elev_chunksize=None,\n",
                 "        diaz_protect_height=diaz,\n",
                 "        diaz_construction_freq=diaz,\n",
@@ -292,65 +277,86 @@
             },
             "source": [
                 "## Get refA values for all movefactors for pyCIAM"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 6,
             "id": "fe7035bb-5a67-4849-ae69-cab582079e88",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
                 "segs = open_zarr(PATH_SLIIDERS_SEG, chunks=None).seg\n",
                 "seg_grps = [segs[i : i + SEG_CHUNKSIZE] for i in range(0, len(segs), SEG_CHUNKSIZE)]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
-            "id": "8bafcf7c-8745-40b4-8fcb-b9dea329cd79",
-            "metadata": {},
+            "execution_count": 19,
+            "id": "c1973a9f-538b-4686-b4bf-8de7f1141a8e",
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
-                "futs = []\n",
-                "for mf in MOVEFACTOR_RANGE:\n",
-                "    futs.append(client.map(get_refA, seg_grps, mf=mf))\n",
-                "refA = xr.concat(\n",
-                "    [dataarray_from_delayed(f, dim=\"seg\") for f in futs], dim=\"movefactor\"\n",
-                ").load()"
+                "def refA_wrapper(mf, seg_grps):\n",
+                "    return xr.concat([get_refA(i, mf=mf) for i in seg_grps], dim=\"seg\")\n",
+                "\n",
+                "\n",
+                "futs = client.map(refA_wrapper, MOVEFACTOR_RANGE, seg_grps=seg_grps)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 23,
+            "id": "5afedf23-92aa-4917-ba8a-7d9a2400fedc",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "refA = xr.concat(client.gather(futs), dim=\"movefactor\")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 25,
             "id": "c5d48e38-2d27-44e0-ac57-1efe61e8d169",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
                 "save(refA.to_dataset(name=\"refA\").chunk(), PATH_REFA, mode=\"w\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 26,
             "id": "36df7985-e275-4de7-98df-2f115030d75a",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
                 "this_refA = open_zarr(PATH_REFA, chunks=None).refA.sel(quantile=0.5, drop=True).load()\n",
                 "sliiders_seg = open_zarr(PATH_SLIIDERS_SEG, chunks=None)\n",
                 "mvmt = calc_exp_moved(sliiders_seg, [\"K_2019\", \"pop_2019\"], this_refA)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
-            "id": "0b5fd401-d204-4d0b-9e33-f09bc30473f5",
-            "metadata": {},
+            "execution_count": 28,
+            "id": "3ee20e77-5bdc-416a-90fd-f5d9ae6febb7",
+            "metadata": {
+                "tags": []
+            },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
                             "<defs>\n",
                             "<symbol id=\"icon-database\" viewBox=\"0 0 32 32\">\n",
@@ -713,105 +719,109 @@
                             "  stroke-width: 0;\n",
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
                             "</style><pre class='xr-text-repr-fallback'>&lt;xarray.Dataset&gt;\n",
                             "Dimensions:   ()\n",
                             "Data variables:\n",
-                            "    K_2019    float64 6.5\n",
-                            "    pop_2019  float64 9.5</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.Dataset</div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-cc12e5c8-8610-4a37-ad0f-dc0284457ff9' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-cc12e5c8-8610-4a37-ad0f-dc0284457ff9' class='xr-section-summary'  title='Expand/collapse section'>Dimensions:</label><div class='xr-section-inline-details'></div><div class='xr-section-details'></div></li><li class='xr-section-item'><input id='section-7d727427-527b-4509-a53e-02bd29ef7596' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-7d727427-527b-4509-a53e-02bd29ef7596' class='xr-section-summary'  title='Expand/collapse section'>Coordinates: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-1f2da617-bca2-4094-80e4-90c056eff9c3' class='xr-section-summary-in' type='checkbox'  checked><label for='section-1f2da617-bca2-4094-80e4-90c056eff9c3' class='xr-section-summary' >Data variables: <span>(2)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span>K_2019</span></div><div class='xr-var-dims'>()</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>6.5</div><input id='attrs-133b0ad4-b33d-4c80-acff-82f9d1f54976' class='xr-var-attrs-in' type='checkbox' disabled><label for='attrs-133b0ad4-b33d-4c80-acff-82f9d1f54976' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-2cd6c8d6-2e81-4e11-a046-d7c091a071ac' class='xr-var-data-in' type='checkbox'><label for='data-2cd6c8d6-2e81-4e11-a046-d7c091a071ac' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'></dl></div><div class='xr-var-data'><pre>array(6.5)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>pop_2019</span></div><div class='xr-var-dims'>()</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>9.5</div><input id='attrs-11cd2e10-ceb9-4ecd-b91d-c25da1e1f451' class='xr-var-attrs-in' type='checkbox' disabled><label for='attrs-11cd2e10-ceb9-4ecd-b91d-c25da1e1f451' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-09bb0de4-88fe-4cfb-a84a-7a9d6bda2f6d' class='xr-var-data-in' type='checkbox'><label for='data-09bb0de4-88fe-4cfb-a84a-7a9d6bda2f6d' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'></dl></div><div class='xr-var-data'><pre>array(9.5)</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-7cb78640-6a8b-4bb8-b058-603b03133bad' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-7cb78640-6a8b-4bb8-b058-603b03133bad' class='xr-section-summary'  title='Expand/collapse section'>Indexes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-ba4e4bab-7fac-4d16-956b-84ca3ff96ba4' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-ba4e4bab-7fac-4d16-956b-84ca3ff96ba4' class='xr-section-summary'  title='Expand/collapse section'>Attributes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li></ul></div></div>"
+                            "    K_2019    float64 6.2\n",
+                            "    pop_2019  float64 8.9</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.Dataset</div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-a81141de-1c21-4876-9b49-b0b36c02d0fa' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-a81141de-1c21-4876-9b49-b0b36c02d0fa' class='xr-section-summary'  title='Expand/collapse section'>Dimensions:</label><div class='xr-section-inline-details'></div><div class='xr-section-details'></div></li><li class='xr-section-item'><input id='section-43cd4ff8-1bad-4deb-a299-e7a64ca2c4e5' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-43cd4ff8-1bad-4deb-a299-e7a64ca2c4e5' class='xr-section-summary'  title='Expand/collapse section'>Coordinates: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-c3e4214d-14a9-4fbe-add8-1381324c22b3' class='xr-section-summary-in' type='checkbox'  checked><label for='section-c3e4214d-14a9-4fbe-add8-1381324c22b3' class='xr-section-summary' >Data variables: <span>(2)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span>K_2019</span></div><div class='xr-var-dims'>()</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>6.2</div><input id='attrs-58376fac-0af3-4793-9b65-fb0304044cdc' class='xr-var-attrs-in' type='checkbox' disabled><label for='attrs-58376fac-0af3-4793-9b65-fb0304044cdc' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-1b9f4e2c-4021-4526-b9db-03d29401edb3' class='xr-var-data-in' type='checkbox'><label for='data-1b9f4e2c-4021-4526-b9db-03d29401edb3' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'></dl></div><div class='xr-var-data'><pre>array(6.2)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>pop_2019</span></div><div class='xr-var-dims'>()</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>8.9</div><input id='attrs-928285ff-2f30-444d-b2f4-a9dda8f79618' class='xr-var-attrs-in' type='checkbox' disabled><label for='attrs-928285ff-2f30-444d-b2f4-a9dda8f79618' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-1b50ebc9-ca26-4e9c-afc9-c9c80333da4b' class='xr-var-data-in' type='checkbox'><label for='data-1b50ebc9-ca26-4e9c-afc9-c9c80333da4b' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'></dl></div><div class='xr-var-data'><pre>array(8.9)</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-d20af42f-4876-4aff-9d83-a9265d7483f8' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-d20af42f-4876-4aff-9d83-a9265d7483f8' class='xr-section-summary'  title='Expand/collapse section'>Indexes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-55f2382f-51be-4751-96c5-bf8aa86ba374' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-55f2382f-51be-4751-96c5-bf8aa86ba374' class='xr-section-summary'  title='Expand/collapse section'>Attributes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<xarray.Dataset>\n",
                             "Dimensions:   ()\n",
                             "Data variables:\n",
-                            "    K_2019    float64 6.5\n",
-                            "    pop_2019  float64 9.5"
+                            "    K_2019    float64 6.2\n",
+                            "    pop_2019  float64 8.9"
                         ]
                     },
-                    "execution_count": 12,
+                    "execution_count": 28,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "ratio = mvmt.sum(\"seg\") / mvmt.sel(movefactor=0).sum(\"seg\")\n",
                 "np.abs(0.5 - ratio).idxmin(\"movefactor\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
-            "id": "61fa9dc4-bbeb-4710-bc84-65bdf6cd6a4c",
-            "metadata": {},
+            "execution_count": 29,
+            "id": "29d533e9-8571-4a2f-9adc-b7a2d03af6d7",
+            "metadata": {
+                "tags": []
+            },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "(0.0, 45675703.08690297)"
+                            "(0.0, 48382814.95746777)"
                         ]
                     },
-                    "execution_count": 13,
+                    "execution_count": 29,
                     "metadata": {},
                     "output_type": "execute_result"
                 },
                 {
                     "data": {
-                        "image/png": "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\n",
+                        "image/png": "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",
                         "text/plain": [
-                            "<Figure size 432x288 with 2 Axes>"
+                            "<Figure size 640x480 with 2 Axes>"
                         ]
                     },
-                    "metadata": {
-                        "needs_background": "light"
-                    },
+                    "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "fig, ax = plt.subplots()\n",
                 "ax2 = ax.twinx()\n",
                 "mvmt.sum(\"seg\").K_2019.plot(ax=ax)\n",
                 "mvmt.sum(\"seg\").pop_2019.plot(ax=ax2, c=\"g\")\n",
                 "ax.set_ylim(0, None)\n",
                 "ax2.set_ylim(0, None)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 31,
             "id": "17c41589-b943-42a8-9522-67e24f3ddf47",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
                 "for v in mvmt.variables:\n",
                 "    if mvmt[v].dtype == object:\n",
                 "        mvmt[v] = mvmt[v].astype(\"unicode\")\n",
                 "save(mvmt, PATH_MOVEFACTOR_DATA, mode=\"w\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 32,
             "id": "f9812bce-b427-4941-820d-700ed1262d1a",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "(None, None)"
                         ]
                     },
-                    "execution_count": 15,
+                    "execution_count": 32,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "client.cluster.close(), client.close()"
+                "cluster.close(), client.close()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "3e2d400a-2d28-4788-aaf2-f39fa0463065",
             "metadata": {},
             "source": [
@@ -1688,15 +1698,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.10"
+            "version": "3.12.2"
         },
         "widgets": {
             "application/vnd.jupyter.widget-state+json": {
                 "state": {},
                 "version_major": 2,
                 "version_minor": 0
             }
```

### Comparing `python-CIAM-1.1.2/notebooks/models/run-pyCIAM-diaz2016.ipynb` & `python-CIAM-1.2/notebooks/models/run-pyCIAM-diaz2016.ipynb`

 * *Files identical despite different names*

### Comparing `python-CIAM-1.1.2/notebooks/models/run-pyCIAM-slrquantiles.ipynb` & `python-CIAM-1.2/notebooks/models/run-pyCIAM-slrquantiles.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9867525703463204%*

 * *Differences: {"'cells'": "{1: {'execution_count': 2}, 2: {'execution_count': 3, 'source': {insert: [(0, 'from "*

 * *            "pyCIAM.run import execute_pyciam\\n'), (18, ')')], delete: [19, 18, 17]}}, 3: "*

 * *            "{'execution_count': 4, 'source': {insert: [(6, 'N_WORKERS = 100\\n'), (8, "*

 * *            "'SEG_CHUNKSIZE = 2\\n')], delete: [9, 7, 6]}}, 4: {'execution_count': 5}, 5: "*

 * *            "{'source': ['client, cluster = start_dask_cluster()\\n', "*

 * *            "'cluster.scale(N_WORKERS)\\n', 'cluster']}, 6: {'execu […]*

```diff
@@ -7,33 +7,34 @@
             },
             "source": [
                 "# Run pyCIAM"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 2,
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "import sys\n",
                 "\n",
                 "sys.path.append(\"../\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 3,
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
+                "from pyCIAM.run import execute_pyciam\n",
                 "from shared import (\n",
                 "    AUTHOR,\n",
                 "    CONTACT,\n",
                 "    DIR_SCRATCH,\n",
                 "    HISTORY,\n",
                 "    PATH_OUTPUTS,\n",
                 "    PATH_PARAMS,\n",
@@ -43,48 +44,45 @@
                 "    PATH_SLR_AR5_QUANTILES,\n",
                 "    PATH_SLR_AR6,\n",
                 "    PATH_SLR_SWEET,\n",
                 "    PATHS_SURGE_LOOKUP,\n",
                 "    QUANTILES,\n",
                 "    STORAGE_OPTIONS,\n",
                 "    start_dask_cluster,\n",
-                ")\n",
-                "\n",
-                "from pyCIAM.run import execute_pyciam"
+                ")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 4,
             "metadata": {
                 "tags": [
                     "parameters"
                 ]
             },
             "outputs": [],
             "source": [
                 "AR6_ONLY = False\n",
                 "\n",
                 "TMPPATH = DIR_SCRATCH / \"pyCIAM_results_quantiles_prechunked.zarr\"\n",
                 "\n",
                 "# When running on larger/scalable dask cluster, may wish to specify number of workers\n",
                 "# Default is LocalCluster which will use the number of CPUs available on local machine\n",
-                "N_WORKERS = None\n",
-                "# N_WORKERS = 400\n",
+                "N_WORKERS = 100\n",
                 "\n",
-                "SEG_CHUNKSIZE = 3\n",
+                "SEG_CHUNKSIZE = 2\n",
                 "\n",
                 "SEG_ADM_SUBSET = None\n",
                 "\n",
                 "DESCRIPTION = \"Projected coastal damages from pyCIAM, using quantiles of SLR scenarios.\""
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 5,
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "if AR6_ONLY:\n",
                 "    all_slr_ds = [PATH_SLR_AR6]\n",
@@ -98,23 +96,22 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "client = start_dask_cluster(\n",
-                "    n_workers=N_WORKERS,\n",
-                ")\n",
-                "client"
+                "client, cluster = start_dask_cluster()\n",
+                "cluster.scale(N_WORKERS)\n",
+                "cluster"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 8,
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "execute_pyciam(\n",
                 "    PATH_PARAMS,\n",
@@ -122,14 +119,15 @@
                 "    all_slr_ds,\n",
                 "    all_slr_name,\n",
                 "    PATH_REFA,\n",
                 "    econ_input_path_seg=PATH_SLIIDERS_SEG,\n",
                 "    output_path=PATH_OUTPUTS,\n",
                 "    seg_var_subset=SEG_ADM_SUBSET,\n",
                 "    surge_input_paths=PATHS_SURGE_LOOKUP,\n",
+                "    pyciam_seg_chunksize=SEG_CHUNKSIZE,\n",
                 "    tmp_output_path=TMPPATH,\n",
                 "    quantiles=QUANTILES,\n",
                 "    dask_client_func=lambda: client,\n",
                 "    storage_options=STORAGE_OPTIONS,\n",
                 "    extra_attrs={\n",
                 "        \"author\": AUTHOR,\n",
                 "        \"contact\": CONTACT,\n",
@@ -152,15 +150,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.0"
+            "version": "3.12.2"
         },
         "widgets": {
             "application/vnd.jupyter.widget-state+json": {
                 "state": {},
                 "version_major": 2,
                 "version_minor": 0
             }
```

### Comparing `python-CIAM-1.1.2/notebooks/nb_logs/data-acquisition.ipynb` & `python-CIAM-1.2/notebooks/nb_logs/data-acquisition.ipynb`

 * *Files identical despite different names*

### Comparing `python-CIAM-1.1.2/notebooks/nb_logs/data-processing/slr/AR6.ipynb` & `python-CIAM-1.2/notebooks/nb_logs/data-processing/slr/AR6.ipynb`

 * *Files identical despite different names*

### Comparing `python-CIAM-1.1.2/notebooks/nb_logs/models/run-pyCIAM-slrquantiles.ipynb` & `python-CIAM-1.2/notebooks/nb_logs/models/run-pyCIAM-slrquantiles.ipynb`

 * *Files identical despite different names*

### Comparing `python-CIAM-1.1.2/notebooks/post-processing/pyCIAM-results-figures.ipynb` & `python-CIAM-1.2/notebooks/post-processing/pyCIAM-results-figures.ipynb`

 * *Files identical despite different names*

### Comparing `python-CIAM-1.1.2/notebooks/post-processing/zenodo-upload.ipynb` & `python-CIAM-1.2/notebooks/post-processing/zenodo-upload.ipynb`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9578244604229944%*

 * *Differences: {"'cells'": "{1: {'execution_count': 2}, 2: {'execution_count': 3, 'source': {insert: [(1, 'import "*

 * *            "re\\n'), (9, 'from cloudpathlib import AnyPath\\n')], delete: [5, 1]}}, 5: "*

 * *            "{'execution_count': 6, 'outputs': {0: {'data': {'text/plain': ['<dask.config.set at "*

 * *            "0x7d40ae7e1130>']}, 'execution_count': 6}}}, 7: {'execution_count': 7, 'source': "*

 * *            "{insert: [(0, 'ACCESS_TOKEN = "*

 * *            '"Q5z5IQ1m5Z9l1QS7ZYeV78IS5bqPmhzcFVo0KSNLoh2p39HRMPgFoJsCyQt5"\\n\') […]*

```diff
@@ -1,61 +1,120 @@
 {
     "cells": [
         {
             "cell_type": "code",
             "execution_count": 1,
+            "id": "42ac0087-fe1b-4088-919e-ce007e6dea8c",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "%load_ext autoreload\n",
+                "%autoreload 2"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 2,
             "id": "706cee66-6557-402d-ae97-679ed202a9fe",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "import sys\n",
                 "\n",
                 "sys.path.append(\"../\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 3,
             "id": "29a54dac-abdc-4a95-967f-2289fc1c9ecb",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "import json\n",
-                "from os import environ\n",
+                "import re\n",
                 "from pathlib import Path\n",
                 "from shutil import make_archive\n",
                 "from tempfile import TemporaryDirectory\n",
-                "from pathlib import Path\n",
                 "\n",
                 "import dask.config\n",
                 "import requests\n",
                 "import shared\n",
+                "from cloudpathlib import AnyPath\n",
                 "from sliiders import settings as sset\n",
                 "from zarr import ZipStore"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 4,
+            "id": "fc342d12-c698-4f64-aaea-fcbfa027431f",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "PATT_OUTPUTS_NC = shared.PATH_OUTPUTS.parent / (shared.PATH_OUTPUTS.stem + \"_{case}.nc\")\n",
+                "PATH_SLIIDERS_NC = sset.PATH_SLIIDERS.parent / (sset.PATH_SLIIDERS.stem + \".nc\")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 5,
+            "id": "a125e75e-2122-4bd1-a994-37f1dbaea124",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Processing noAdaptation\n",
+                        "Processing protect10\n",
+                        "Processing protect100\n",
+                        "Processing protect1000\n",
+                        "Processing protect10000\n",
+                        "Processing retreat1\n",
+                        "Processing retreat10\n",
+                        "Processing retreat100\n",
+                        "Processing retreat1000\n",
+                        "Processing retreat10000\n",
+                        "Processing optimalfixed\n"
+                    ]
+                }
+            ],
+            "source": [
+                "ds = shared.open_zarr(shared.PATH_OUTPUTS)\n",
+                "fpaths = []\n",
+                "for case in ds.case.values:\n",
+                "    print(f\"Processing {case}\")\n",
+                "    fpath = AnyPath(str(PATT_OUTPUTS_NC).format(case=case))\n",
+                "    fpaths.append(fpath)\n",
+                "    if not fpath.exists():\n",
+                "        shared.save_dataset(ds.sel(case=case).load(), fpath)\n",
+                "\n",
+                "shared.save_dataset(shared.open_zarr(sset.PATH_SLIIDERS).load(), PATH_SLIIDERS_NC)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 6,
             "id": "d37ca26f-091d-4cb6-be02-385464e0b687",
             "metadata": {
                 "tags": []
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<dask.config.set at 0x112a25b70>"
+                            "<dask.config.set at 0x7d40ae7e1130>"
                         ]
                     },
-                    "execution_count": 3,
+                    "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "dask.config.set(scheduler=\"threads\")"
             ]
@@ -66,46 +125,50 @@
             "metadata": {},
             "source": [
                 "## Parameters"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 7,
             "id": "55a3e849-a554-49fa-882c-846acf76f3b8",
             "metadata": {
                 "tags": [
                     "parameters"
                 ]
             },
             "outputs": [],
             "source": [
-                "ACCESS_TOKEN = environ[\"ACCESS_TOKEN\"]\n",
-                "VERSION = \"1.1.0\"\n",
+                "ACCESS_TOKEN = \"Q5z5IQ1m5Z9l1QS7ZYeV78IS5bqPmhzcFVo0KSNLoh2p39HRMPgFoJsCyQt5\"\n",
+                "VERSION = \"1.2.0\"\n",
                 "TITLES = {\n",
-                "    \"SLIIDERS\": \"SLIIDERS: Sea Level Impacts Input Dataset by Elevation, Region, and Scenario\",\n",
-                "    \"pyCIAM\": \"Estimates of Global Coastal Losses Under Multiple Sea Level Rise Scenarios\",\n",
+                "    # \"SLIIDERS\": (\n",
+                "    #     \"SLIIDERS: Sea Level Impacts Input Dataset by Elevation, Region, and Scenario\"\n",
+                "    # ),\n",
+                "    \"pyCIAM\": (\n",
+                "        \"Estimates of Global Coastal Losses Under Multiple Sea Level Rise Scenarios\"\n",
+                "    ),\n",
                 "}\n",
-                "PYCIAM_CODE_PATH=Path(\"pyCIAM-1.1.2.zip\")\n",
-                "SLIIDERS_CODE_PATH=Path(\"sliiders-1.1.1.zip\")"
+                "PYCIAM_CODE_PATH = Path(\"pyCIAM.zip\")\n",
+                "SLIIDERS_CODE_PATH = Path(\"/tmp/sliiders.zip\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 8,
             "id": "8725b84c-8a7f-4d88-96ec-849e963ef8ce",
             "metadata": {},
             "outputs": [],
             "source": [
                 "PARAMS = {\"access_token\": ACCESS_TOKEN}"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 9,
             "id": "956c40ee-e3e8-4257-bd0d-2c938546604d",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# get host\n",
                 "Z_URL = \"https://zenodo.org/api/deposit/depositions\"\n",
                 "\n",
@@ -132,68 +195,80 @@
             "metadata": {},
             "source": [
                 "## Metadata"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 10,
             "id": "b5fcb2b8-3fb4-4789-bae0-18f7a66b7c51",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Metadata\n",
                 "AUTHORS = [\n",
                 "    {\n",
-                "        \"affiliation\": \"Energy & Resources Group, University of California, Berkeley; Global Policy Lab, Goldman School of Public Policy, University of California, Berkeley\",\n",
+                "        \"affiliation\": \"United Nations Development Programme\",\n",
                 "        \"name\": \"Depsky, Nicholas\",\n",
                 "        \"orcid\": \"0000-0002-9441-9042\",\n",
                 "    },\n",
                 "    {\n",
-                "        \"affiliation\": \"BlackRock; Global Policy Lab, Goldman School of Public Policy, University of California, Berkeley\",\n",
+                "        \"affiliation\": (\n",
+                "            \"Reask; Global Policy Lab, Goldman School of Public Policy, University of \"\n",
+                "            \"California, Berkeley\"\n",
+                "        ),\n",
                 "        \"name\": \"Bolliger, Ian\",\n",
                 "        \"orcid\": \"0000-0001-8055-297X\",\n",
                 "    },\n",
                 "    {\n",
-                "        \"affiliation\": \"Global Policy Lab, Goldman School of Public Policy, University of California, Berkeley\",\n",
+                "        \"affiliation\": \"Recidiviz\",\n",
                 "        \"name\": \"Allen, Daniel\",\n",
                 "        \"orcid\": \"0000-0001-5366-5178\",\n",
                 "    },\n",
                 "    {\n",
-                "        \"affiliation\": \"Energy Policy Institute, University of Chicago\",\n",
+                "        \"affiliation\": \"Columbia University\",\n",
                 "        \"name\": \"Choi, Jun Ho\",\n",
                 "        \"orcid\": \"0000-0003-0749-9222\",\n",
                 "    },\n",
                 "    {\n",
                 "        \"affiliation\": \"The Rhodium Group\",\n",
                 "        \"name\": \"Delgado, Michael\",\n",
                 "        \"orcid\": \"0000-0002-2414-045X\",\n",
                 "    },\n",
                 "    {\n",
-                "        \"affiliation\": \"National Bureau of Economic Research; Energy Policy Institute, University of Chicago\",\n",
+                "        \"affiliation\": (\n",
+                "            \"National Bureau of Economic Research; Energy Policy Institute, University \"\n",
+                "            \"of Chicago\"\n",
+                "        ),\n",
                 "        \"name\": \"Greenstone, Michael\",\n",
                 "        \"orcid\": \"0000-0002-2364-2810\",\n",
                 "    },\n",
                 "    {\n",
-                "        \"affiliation\": \"The Rhodium Group\",\n",
+                "        \"affiliation\": \"BlackRock\",\n",
                 "        \"name\": \"Hamidi, Ali\",\n",
                 "        \"orcid\": \"0000-0001-6235-0303\",\n",
                 "    },\n",
                 "    {\n",
                 "        \"affiliation\": \"The Rhodium Group\",\n",
                 "        \"name\": \"Houser, Trevor\",\n",
                 "        \"orcid\": \"0000-0002-0514-7058\",\n",
                 "    },\n",
                 "    {\n",
-                "        \"affiliation\": \"Global Policy Lab, Goldman School of Public Policy, University of California, Berkeley; National Bureau of Economic Research\",\n",
+                "        \"affiliation\": (\n",
+                "            \"Global Policy Lab, Goldman School of Public Policy, University of \"\n",
+                "            \"California, Berkeley; National Bureau of Economic Research\"\n",
+                "        ),\n",
                 "        \"name\": \"Hsiang, Solomon\",\n",
                 "        \"orcid\": \"0000-0002-2074-0829\",\n",
                 "    },\n",
                 "    {\n",
-                "        \"affiliation\": \"Department of Earth & Planetary Sciences and Rutgers Institute of Earth, Ocean and Atmospheric Sciences, Rutgers University\",\n",
+                "        \"affiliation\": (\n",
+                "            \"Department of Earth & Planetary Sciences and Rutgers Institute of Earth, \"\n",
+                "            \"Ocean and Atmospheric Sciences, Rutgers University\"\n",
+                "        ),\n",
                 "        \"name\": \"Kopp, Robert E.\",\n",
                 "        \"orcid\": \"0000-0003-4016-9428\",\n",
                 "    },\n",
                 "]"
             ]
         },
         {
@@ -202,83 +277,96 @@
             "metadata": {},
             "source": [
                 "## Files To Upload"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 11,
             "id": "55188020-c02f-4fa6-bf4c-cf1cd87e1754",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Files and paths\n",
                 "ORIGINAL_PATHS = {\n",
                 "    \"SLIIDERS\": {\n",
-                "        \"products\": [shared.PATH_SLIIDERS],\n",
+                "        \"products\": [sset.PATH_SLIIDERS, PATH_SLIIDERS_NC],\n",
                 "        \"inputs\": [\n",
                 "            sset.PATH_GEOG_GTSM_SNAPPED,\n",
                 "            sset.PATH_GEOG_GTSM_STATIONS_TOTHIN,\n",
                 "            sset.PATH_SEG_PTS_MANUAL,\n",
                 "        ],\n",
                 "    },\n",
+                "    # uncomment Diaz inputs if a re-upload is necessary\n",
                 "    \"pyCIAM\": {\n",
                 "        \"products\": [\n",
                 "            shared.PATH_OUTPUTS,\n",
-                "            shared.PATH_DIAZ_RES,\n",
+                "            # shared.PATH_DIAZ_RES,\n",
                 "            shared.PATH_MOVEFACTOR_DATA,\n",
+                "            *fpaths,\n",
                 "        ],\n",
                 "        \"inputs\": [\n",
-                "            shared.PATH_DIAZ_INPUTS_RAW,\n",
-                "            shared.PATH_SLR_AR5_QUANTILES,\n",
+                "            # shared.PATH_DIAZ_INPUTS_RAW,\n",
+                "            # shared.PATH_SLR_AR5_QUANTILES,\n",
                 "            shared.PATH_SLIIDERS_INCOME_INTERMEDIATE_FILE,\n",
                 "            shared.PATHS_SURGE_LOOKUP[\"seg\"],\n",
                 "            shared.PATHS_SURGE_LOOKUP[\"seg_adm\"],\n",
                 "        ],\n",
                 "    },\n",
                 "}\n",
                 "\n",
                 "if PYCIAM_CODE_PATH is not None:\n",
                 "    ORIGINAL_PATHS[\"pyCIAM\"][\"source\"] = [PYCIAM_CODE_PATH]\n",
                 "if SLIIDERS_CODE_PATH is not None:\n",
-                "    ORIGINAL_PATHS[\"SLIIDERS\"][\"source\"] = [SLIIDERS_CODE_PATH"
+                "    ORIGINAL_PATHS[\"SLIIDERS\"][\"source\"] = [SLIIDERS_CODE_PATH]"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "bff745dd-9688-44fe-9d19-0c12f7be9ab1",
             "metadata": {
                 "tags": []
             },
             "source": [
                 "## Create and/or update depositions"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 12,
             "id": "50c10e4c-b3eb-4714-8d32-486ac878d041",
             "metadata": {},
             "outputs": [],
             "source": [
                 "def create_draft_deposit(name, update_dict={}, overwrite=False):\n",
                 "    dep = EXISTING_DEPOSITS[name]\n",
-                "    # create new deposit\n",
-                "    deposition_id = dep[\"id\"]\n",
-                "    if deposition_id == int(dep[\"links\"][\"latest\"].split(\"/\")[-1]):\n",
-                "        url = f\"{Z_URL}/{deposition_id}/actions/newversion\"\n",
-                "        r = requests.post(url, params=PARAMS)\n",
-                "        if r.status_code not in [200, 201]:\n",
-                "            raise ValueError(f\"{r.status_code}: {r.text}\")\n",
+                "\n",
+                "    # create new deposit if needed\n",
+                "    r = requests.post(dep[\"links\"][\"newversion\"], params=PARAMS)\n",
+                "    # case 1: this is already a new unpublished version\n",
+                "    if (\n",
+                "        r.status_code == 404\n",
+                "        and r.json()[\"message\"] == \"The persistent identifier is not registered.\"\n",
+                "    ):\n",
+                "        pass\n",
+                "    # case 2: this is a successful new version request and we need to grab the new\n",
+                "    # version deposition\n",
+                "    elif r.status_code in [200, 201]:\n",
+                "        # returned value would be original deposit version in case of new version\n",
+                "        # created\n",
                 "        dep = r.json()\n",
+                "    # case 3: some other error\n",
+                "    else:\n",
+                "        raise ValueError(f\"{r.status_code}: {r.text}\")\n",
+                "\n",
+                "    dep = requests.get(dep[\"links\"][\"latest_draft\"], params=PARAMS).json()\n",
                 "\n",
                 "    if overwrite:\n",
                 "        new_id = dep[\"links\"][\"latest_draft\"].split(\"/\")[-1]\n",
                 "        files = requests.get(dep[\"links\"][\"files\"], params=PARAMS).json()\n",
-                "        print(files)\n",
                 "        if len(files):\n",
                 "            for f in files:\n",
                 "                file_url = f\"{Z_URL}/{new_id}/files/{f['id']}\"\n",
                 "                r = requests.delete(file_url, params=PARAMS)\n",
                 "                if r.status_code not in [204, 404]:\n",
                 "                    raise ValueError(f\"{r.status_code}: {r.text}\")\n",
                 "\n",
@@ -293,73 +381,73 @@
                 "    )\n",
                 "    if meta_put.status_code != 200:\n",
                 "        raise ValueError(f\"{meta_put.status_code}: {meta_put.text}\")\n",
                 "    return dep\n",
                 "\n",
                 "\n",
                 "def create_all_new_deposits(titles=TITLES, overwrite=False):\n",
-                "    deps = {}\n",
-                "    ids = {}\n",
-                "    for t in titles.keys():\n",
-                "        dep = create_draft_deposit(t, overwrite=overwrite)\n",
-                "        ids[t] = int(dep[\"links\"][\"latest_draft\"].split(\"/\")[-1])\n",
-                "    all_deps = requests.get(\n",
-                "        Z_URL,\n",
-                "        params={\"access_token\": ACCESS_TOKEN},\n",
-                "    ).json()\n",
-                "    for t in titles.keys():\n",
-                "        dep = [d for d in all_deps if d[\"id\"] == ids[t]]\n",
-                "        assert len(dep) == 1\n",
-                "        deps[t] = dep[0]\n",
-                "    return deps\n",
+                "    return {t: create_draft_deposit(t, overwrite=overwrite) for t in titles.keys()}\n",
+                "\n",
                 "\n",
+                "def _get_zenodo_name(fname):\n",
+                "    # drop a datestamp if it exists\n",
+                "    zenodo_name = re.sub(r\"_\\d{8}\", \"\", fname.name)\n",
+                "    # drop version from name\n",
+                "    return \"-\".join([i for i in zenodo_name.split(\"-\") if shared.RES_VERS not in i])\n",
                 "\n",
-                "def upload_file(deposit_link_dict, fname, root, zenodo_name=None, overwrite=False):\n",
+                "\n",
+                "def upload_file(\n",
+                "    deposit_link_dict, fname, zenodo_name=None, overwrite=False, existing_files={}\n",
+                "):\n",
                 "    if zenodo_name is None:\n",
-                "        zenodo_name = fname.name\n",
-                "    zenodo_name = root + zenodo_name\n",
+                "        zenodo_name = _get_zenodo_name(fname)\n",
                 "\n",
-                "    existing_files = {\n",
-                "        f[\"filename\"]: f\n",
-                "        for f in requests.get(deposit_link_dict[\"files\"], params=PARAMS).json()\n",
-                "    }\n",
                 "    if zenodo_name in existing_files:\n",
                 "        if not overwrite:\n",
                 "            print(\"...Skipping b/c already uploaded\")\n",
                 "            return existing_files[zenodo_name]\n",
                 "        requests.delete(existing_files[zenodo_name][\"links\"][\"self\"], params=PARAMS)\n",
                 "\n",
                 "    with fname.open(\"rb\") as fp:\n",
                 "        r = requests.put(\n",
                 "            f\"{deposit_link_dict['bucket']}/{zenodo_name}\",\n",
                 "            params=PARAMS,\n",
                 "            data=fp,\n",
                 "        )\n",
                 "\n",
-                "    if r.status_code != 200:\n",
+                "    if r.status_code not in [200, 201]:\n",
                 "        raise ValueError(f\"{r.status_code}: {r.text}\")\n",
                 "    return r.json()\n",
                 "\n",
                 "\n",
-                "def upload_file_list(deposit, flist, root, overwrite=False):\n",
+                "def upload_file_list(deposit, flist, overwrite=False):\n",
                 "    out = []\n",
-                "    existing_files = {\n",
-                "        f[\"filename\"]: f\n",
-                "        for f in requests.get(deposit[\"links\"][\"files\"], params=PARAMS).json()\n",
-                "    }\n",
+                "    existing_file_request = requests.get(deposit[\"links\"][\"files\"], params=PARAMS)\n",
+                "    if existing_file_request.status_code == 404:\n",
+                "        existing_files = {}\n",
+                "    else:\n",
+                "        existing_files = {f[\"filename\"]: f for f in existing_file_request.json()}\n",
                 "    for f in flist:\n",
                 "        print(f\"Uploading: {str(f)}\")\n",
+                "        zenodo_name = _get_zenodo_name(f)\n",
                 "        if (\n",
-                "            (root + f.name) in existing_files\n",
-                "            or (root + f.name + \".zip\") in existing_files\n",
+                "            zenodo_name in existing_files or (zenodo_name + \".zip\") in existing_files\n",
                 "        ) and not overwrite:\n",
                 "            print(\"...Skipping b/c already uploaded\")\n",
                 "            continue\n",
                 "        if f.is_file():\n",
-                "            out.append(upload_file(deposit[\"links\"], f, root, overwrite=overwrite))\n",
+                "            out.append(\n",
+                "                upload_file(\n",
+                "                    deposit[\"links\"],\n",
+                "                    f,\n",
+                "                    overwrite=overwrite,\n",
+                "                    zenodo_name=zenodo_name,\n",
+                "                    existing_files=existing_files,\n",
+                "                )\n",
+                "            )\n",
                 "        elif f.is_dir():\n",
                 "            with TemporaryDirectory() as d:\n",
                 "                tmp_file = Path(d) / (f.name + \".zip\")\n",
                 "\n",
                 "                if f.suffix == \".zarr\":\n",
                 "                    with ZipStore(tmp_file, mode=\"w\") as tf:\n",
                 "                        ds = shared.open_zarr(f)\n",
@@ -375,99 +463,105 @@
                 "                    f.download_to(name)\n",
                 "                    make_archive(name, \"zip\", name)\n",
                 "\n",
                 "                out.append(\n",
                 "                    upload_file(\n",
                 "                        deposit[\"links\"],\n",
                 "                        tmp_file,\n",
-                "                        root,\n",
+                "                        zenodo_name=zenodo_name,\n",
                 "                        overwrite=overwrite,\n",
                 "                    )\n",
                 "                )\n",
                 "        else:\n",
                 "            raise ValueError(f)\n",
                 "    return out"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 13,
             "id": "868b1d78-5eb4-4fa6-bcfc-0dbd8c88d39b",
             "metadata": {},
             "outputs": [],
             "source": [
                 "draft_deps = create_all_new_deposits(overwrite=False)"
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "558e67ba-77cb-4355-9dfb-d11533f1a344",
-            "metadata": {},
-            "source": [
-                "Note that it seems to take some time for the \"bucket\" link to show up, which is needed to use Zenodo's \"new\" file API, which allows for uploads larger than 100MB. So if bucket is not appearing, you may need to wait a while (<1 day) to be able to run the file uploads below."
-            ]
-        },
-        {
             "cell_type": "code",
             "execution_count": 14,
             "id": "ff8703bb-c630-418e-9f2f-c62b116ee7e8",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "pyCIAM\n",
-                        "Uploading: gs://rhg-data/impactlab-rhg/coastal/sliiders/raw/CIAM_2016/diaz2016_inputs_raw.zarr\n",
-                        "Uploading: gs://rhg-data/impactlab-rhg/coastal/ciam_paper/data/int/slr/ar5/ar5-msl-rel-2005-quantiles.zarr\n",
-                        "Uploading: gs://rhg-data/impactlab-rhg/coastal/sliiders/int/exposure/ypk/finalized/ypk_2000_2100_20221122.zarr\n",
-                        "Uploading: gs://rhg-data/impactlab-rhg/coastal/ciam_paper/data/int/surge-lookup-v1.1-seg.zarr\n",
-                        "Uploading: gs://rhg-data/impactlab-rhg/coastal/ciam_paper/data/int/surge-lookup-v1.1-seg_adm.zarr\n",
-                        "Uploading: gs://rhg-data/impactlab-rhg/coastal/ciam_paper/results-v1.1/pyCIAM_outputs.zarr\n",
-                        "Uploading: gs://rhg-data/impactlab-rhg/coastal/ciam_paper/results-v1.1/diaz2016_outputs.zarr\n",
-                        "Uploading: gs://rhg-data/impactlab-rhg/coastal/ciam_paper/results-v1.1/suboptimal_capital_by_movefactor.zarr\n"
+                        "Uploading: gs://rhg-data/impactlab-rhg/coastal/sliiders/int/exposure/ypk/finalized/ypk_2000_2100_20240222.zarr\n",
+                        "...Skipping b/c already uploaded\n",
+                        "Uploading: gs://rhg-data/impactlab-rhg/coastal/ciam_paper/data/int/surge-lookup-v1.2-seg.zarr\n",
+                        "...Skipping b/c already uploaded\n",
+                        "Uploading: gs://rhg-data/impactlab-rhg/coastal/ciam_paper/data/int/surge-lookup-v1.2-seg_adm.zarr\n",
+                        "...Skipping b/c already uploaded\n",
+                        "Uploading: gs://rhg-data/impactlab-rhg/coastal/ciam_paper/results-v1.2/pyCIAM_outputs.zarr\n",
+                        "...Skipping b/c already uploaded\n",
+                        "Uploading: gs://rhg-data/impactlab-rhg/coastal/ciam_paper/results-v1.2/suboptimal_capital_by_movefactor.zarr\n",
+                        "...Skipping b/c already uploaded\n",
+                        "Uploading: gs://rhg-data/impactlab-rhg/coastal/ciam_paper/results-v1.2/pyCIAM_outputs_noAdaptation.nc\n",
+                        "...Skipping b/c already uploaded\n",
+                        "Uploading: gs://rhg-data/impactlab-rhg/coastal/ciam_paper/results-v1.2/pyCIAM_outputs_protect10.nc\n",
+                        "...Skipping b/c already uploaded\n",
+                        "Uploading: gs://rhg-data/impactlab-rhg/coastal/ciam_paper/results-v1.2/pyCIAM_outputs_protect100.nc\n",
+                        "...Skipping b/c already uploaded\n",
+                        "Uploading: gs://rhg-data/impactlab-rhg/coastal/ciam_paper/results-v1.2/pyCIAM_outputs_protect1000.nc\n",
+                        "...Skipping b/c already uploaded\n",
+                        "Uploading: gs://rhg-data/impactlab-rhg/coastal/ciam_paper/results-v1.2/pyCIAM_outputs_protect10000.nc\n",
+                        "...Skipping b/c already uploaded\n",
+                        "Uploading: gs://rhg-data/impactlab-rhg/coastal/ciam_paper/results-v1.2/pyCIAM_outputs_retreat1.nc\n",
+                        "...Skipping b/c already uploaded\n",
+                        "Uploading: gs://rhg-data/impactlab-rhg/coastal/ciam_paper/results-v1.2/pyCIAM_outputs_retreat10.nc\n",
+                        "Uploading: gs://rhg-data/impactlab-rhg/coastal/ciam_paper/results-v1.2/pyCIAM_outputs_retreat100.nc\n",
+                        "Uploading: gs://rhg-data/impactlab-rhg/coastal/ciam_paper/results-v1.2/pyCIAM_outputs_retreat1000.nc\n",
+                        "Uploading: gs://rhg-data/impactlab-rhg/coastal/ciam_paper/results-v1.2/pyCIAM_outputs_optimalfixed.nc\n",
+                        "Uploading: pyCIAM.zip\n"
                     ]
                 }
             ],
             "source": [
                 "uploads = {}\n",
-                "for name, kind in ORIGINAL_PATHS.items():\n",
+                "for name in TITLES:\n",
                 "    print(name)\n",
+                "    kind = ORIGINAL_PATHS[name]\n",
                 "    this_dep = draft_deps[name]\n",
                 "\n",
-                "    uploads[name] = upload_file_list(\n",
-                "        this_dep, kind[\"inputs\"], \"inputs/\", overwrite=False\n",
-                "    )\n",
-                "    uploads[name] += upload_file_list(\n",
-                "        this_dep, kind[\"products\"], \"products/\", overwrite=False\n",
-                "    )\n",
-                "    if \"source\" in kind.keys(): \n",
-                "        uploads[name] += upload_file_list(\n",
-                "            this_dep, kind[\"source\"], \"source/\", overwrite=False\n",
-                "        )"
+                "    uploads[name] = []\n",
+                "    for filetype in [\"inputs\", \"products\", \"source\"]:\n",
+                "        if filetype in kind:\n",
+                "            uploads[name] += upload_file_list(this_dep, kind[filetype], overwrite=False)"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python [conda env:sliiders]",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
-            "name": "conda-env-sliiders-py"
+            "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.9"
+            "version": "3.12.2"
         },
         "widgets": {
             "application/vnd.jupyter.widget-state+json": {
                 "state": {},
                 "version_major": 2,
                 "version_minor": 0
             }
```

### Comparing `python-CIAM-1.1.2/notebooks/run_example.sh` & `python-CIAM-1.2/notebooks/run_example.sh`

 * *Files identical despite different names*

### Comparing `python-CIAM-1.1.2/notebooks/run_full_replication.sh` & `python-CIAM-1.2/notebooks/run_full_replication.sh`

 * *Files identical despite different names*

### Comparing `python-CIAM-1.1.2/notebooks/shared.py` & `python-CIAM-1.2/notebooks/shared.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,39 @@
+import os
 from pathlib import Path
+from zipfile import ZipFile
 
 import geopandas as gpd
 import xarray as xr
-from distributed import Client
-from distributed.diagnostics.plugin import UploadDirectory
+from dask_gateway import GatewayCluster
 
 from pyCIAM import __file__
 
 DIR_SCRATCH = Path("/tmp/ciam-scratch")
 
-SLIIDERS_VERS = "v1.1"
-RES_VERS = "v1.1"
+SLIIDERS_VERS = "v1.2"
+RES_VERS = "v1.2"
 
 # Cloud Storage tools (will work with local storage as well but may need to be specifiec
 # for cloud buckets
-STORAGE_OPTIONS = {}
+STORAGE_OPTIONS = None
 
 
 def _to_fuse(path):
     return Path(str(path).replace("gs://", "/gcs/"))
 
 
 # quantiles of local SLR at which to run analysis
 QUANTILES = [0.17, 0.5, 0.83]
 
 # Output dataset attrs
-HISTORY = """version 1.1: Version associated with Depsky et al. 2023"""
+HISTORY = """version 1.1: Version associated with Depsky et al. 2023.
+version 1.2: Updated to use SLIIDERS v1.2 as input."""
 AUTHOR = "Ian Bolliger"
-CONTACT = "ian.bolliger@blackrock.com"
+CONTACT = "ian@reask.earth"
 
 # AR5 SLR projections info
 LOCALIZESL_COREFILES = {
     "SLRProjections190726core_SEJ_full": ["L", "H"],
     "SLRProjections170113GRIDDEDcore": [None],
     "SLRProjections200204GRIDDEDcore_D20": [None],
     "SLRProjections210628GRIDDEDcore_SROCC": [None],
@@ -50,29 +52,30 @@
 DIR_RES = DIR_HOME / f"results-{RES_VERS}"
 
 ##################
 # MODEL PARAMS
 ##################
 
 # NECESSARY FOR EXAMPLE
-PATH_PARAMS = Path.home() / "git-repos/pyciam/params.json"
+PATH_PARAMS = Path.home() / "git-repos/pyCIAM/params.json"
 
-PATH_PARAMS_DIAZ = Path.home() / "git-repos/pyciam/params_diaz.json"
+PATH_PARAMS_DIAZ = Path.home() / "git-repos/pyCIAM/params_diaz.json"
 
 ##################
 # SOCIOECON INPUTS
 ##################
 
 # SLIIDERS
 
 # NECESSARY FOR EXAMPLE
 PATH_SLIIDERS = DIR_RAW / f"sliiders-{SLIIDERS_VERS}.zarr"
 
-# NECESSARY FOR EXAMPLE
-PATH_SLIIDERS_SEG = DIR_INT / f"sliiders-{SLIIDERS_VERS}-seg.zarr"
+PATH_SLIIDERS_SEG = PATH_SLIIDERS.parent / (
+    PATH_SLIIDERS.stem + "-seg" + PATH_SLIIDERS.suffix
+)
 
 # Diaz
 PATH_DIAZ_INPUTS_RAW = DIR_RAW / "diaz2016_inputs_raw.zarr"
 PATH_DIAZ_INPUTS_INT = DIR_INT / "diaz2016_inputs.zarr"
 
 #####
 # SLR
@@ -128,15 +131,15 @@
 PATH_DIAZ_RES = DIR_RES / "diaz2016_outputs.zarr"
 
 
 ############################
 # FILES FOR PLOTTING RESULTS
 ############################
 PATH_MOVEFACTOR_DATA = DIR_RES / "suboptimal_capital_by_movefactor.zarr"
-PATH_SLIIDERS_INCOME_INTERMEDIATE_FILE = DIR_RAW / "ypk_2000_2100_20221122.zarr"
+PATH_SLIIDERS_INCOME_INTERMEDIATE_FILE = DIR_RAW / "ypk_2000_2100_20240222.zarr"
 
 DIR_FIGS = Path("/home/jovyan/ciam-figures")
 DIR_SHP = DIR_RAW / "shapefiles"
 PATH_PWT = DIR_RAW / "pwt_100.parquet"
 
 PATH_BORDERS = (
     DIR_SHP
@@ -151,56 +154,56 @@
 for p in [
     DIR_SCRATCH,
     DIR_RES,
 ]:
     p.mkdir(exist_ok=True, parents=True)
 
 
-def upload_pyciam(client, restart_client=True):
-    """Upload a local package to Dask Workers. After calling this function, the package
-    contained at ``pkg_dir`` will be available on all workers in your Dask cluster,
-    including those that are instantiated afterward. This package will take priority
-    over any existing packages of the same name. This is a useful tool for working with
-    remote dask clusters (e.g. via Dask Gateway) but is not needed for local clusters.
-    If you wish to use this, you should call this function from within
-    `start_dask_cluster`.
-
-    Parameters
-    ----------
-    client : :py:class:`distributed.Client`
-        The client object associated with your Dask cluster's scheduler.
-    pkg_dir : str or Path-like
-        Path to the package you wish to zip and upload
-    **kwargs
-        Passed directly to :py:class:`distributed.diagnostics.plugin.UploadDirectory`
-    """
-    client.register_worker_plugin(
-        UploadDirectory(
-            Path(__file__).parents[1],
-            update_path=True,
-            restart=restart_client,
-            skip_words=(
-                ".git",
-                ".github",
-                ".pytest_cache",
-                "tests",
-                "docs",
-                "deploy",
-                "notebooks",
-                ".ipynb_checkpoints",
-                "__pycache__",
-                ".coverage",
-                "dockerignore",
-                ".gitignore",
-                ".gitlab-ci.yml",
-                ".gitmodules",
-                "pyclaw.log",
-            ),
-        )
-    )
+def _zipdir(
+    path,
+    zip_filename,
+    skip_files=(
+        ".git",
+        ".github",
+        ".pytest_cache",
+        "tests",
+        "docs",
+        "deploy",
+        "notebooks",
+        ".ipynb_checkpoints",
+        "__pycache__",
+        ".coverage",
+        "dockerignore",
+        ".gitignore",
+        ".gitlab-ci.yml",
+        ".gitmodules",
+        "pyclaw.log",
+        "run_tests.sh",
+    ),
+):
+
+    with ZipFile(zip_filename, "w") as ziph:
+        for root, dirs, files in os.walk(path):
+            for file in files:
+                if any([f in file.split("/") for f in skip_files]):
+                    continue
+                # Create a relative path for files to preserve the directory structure
+                # within the ZIP archive. This relative path is based on the directory
+                # being zipped, so files are stored in the same structure.
+                relative_path = os.path.relpath(
+                    os.path.join(root, file), os.path.join(path, "..")
+                )
+                ziph.write(os.path.join(root, file), arcname=relative_path)
+
+
+def upload_pyciam(client):
+    package_dir = Path(__file__).parent
+    zip_filename = "/tmp/pyCIAM.zip"  # Output ZIP file name
+    _zipdir(package_dir, zip_filename)
+    client.upload_file(zip_filename)
 
 
 def save(obj, path, *args, **kwargs):
     if path.suffix == ".zarr":
         meth = "to_zarr"
     elif path.suffix == ".parquet":
         meth = "to_parquet"
@@ -219,23 +222,30 @@
 
 def open_dataset(path, **kwargs):
     _path = str(_to_fuse(path))
     _generate_parent_fuse_dirs(_path)
     return xr.open_dataset(_path, **kwargs)
 
 
+def save_dataset(ds, path, **kwargs):
+    _path = str(_to_fuse(path))
+    _generate_parent_fuse_dirs(_path)
+    return ds.to_netcdf(_path, **kwargs)
+
+
 def open_dataarray(path, **kwargs):
     _path = str(_to_fuse(path))
     _generate_parent_fuse_dirs(_path)
     return xr.open_dataarray(_path, **kwargs)
 
 
 def read_shapefile(path, **kwargs):
     _path = str(path).replace("gs://", "/gcs/")
     _generate_parent_fuse_dirs(_path)
     return gpd.read_file(_path, **kwargs)
 
 
-def start_dask_cluster(**kwargs):
-    client = Client(**kwargs)
-    print(client.dashboard_link)
-    return client
+def start_dask_cluster(profile="micro", **kwargs):
+    cluster = GatewayCluster(profile=profile, **kwargs)
+    client = cluster.get_client()
+    upload_pyciam(client)
+    return client, cluster
```

### Comparing `python-CIAM-1.1.2/params.json` & `python-CIAM-1.2/params.json`

 * *Files identical despite different names*

### Comparing `python-CIAM-1.1.2/params_diaz.json` & `python-CIAM-1.2/params_diaz.json`

 * *Files identical despite different names*

### Comparing `python-CIAM-1.1.2/pyCIAM/constants.py` & `python-CIAM-1.2/pyCIAM/constants.py`

 * *Files identical despite different names*

### Comparing `python-CIAM-1.1.2/pyCIAM/io.py` & `python-CIAM-1.2/pyCIAM/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """This module contains functions related to loading and saving inputs and intermediate
 outputs used in running pyCIAM.
 
 Functions
-    prep_sliiders
-    load_ciam_inputs
-    load_diaz_inputs
+---------
+* prep_sliiders
+* load_ciam_inputs
+* load_diaz_inputs
 """
 
-from collections.abc import Iterable
-
 import dask.array as da
 import numpy as np
 import pandas as pd
 import pint_xarray  # noqa: F401
 import xarray as xr
 
 from pyCIAM.utils import spherical_nearest_neighbor as snn
@@ -293,19 +292,19 @@
     if interp_years is not None:
         slr_out = slr_out.interp(year=interp_years)
     return slr_out
 
 
 def create_template_dataarray(dims, coords, chunks, dtype="float32", name=None):
     """A utility function helpful for creatting an empty, dask-backed
-    :py:class:`xarray.DataArray` with specific dimensions, coordinates, dtype, name,
-    and chunk structure. This is useful for "probabilistic" mode of pyCIAM, in which
-    you will run the model on a large ensemble of SLR trajectory realizations. In this
-    case, we save an empty Zarr store and then parallelize the model runs across
-    regions, with each processor writing to a region within the template store.
+    :py:class:`xarray.DataArray` with specific dimensions, coordinates, dtype, name, and
+    chunk structure. This is useful for "probabilistic" mode of pyCIAM, in which you
+    will run the model on a large ensemble of SLR trajectory realizations. In this case,
+    we save an empty Zarr store and then parallelize the model runs across regions, with
+    each processor writing to a region within the template store.
 
     Parameters
     ----------
     dims : list of str
         Dimensions to create.
     coords : dict
         Keys are values in `dims`. Values are a list of values along each dimension.
@@ -332,18 +331,18 @@
         name=name,
     )
 
 
 def create_template_dataset(var_dims, coords, chunks, dtypes):
     """A utility function helpful for creatting an empty, dask-backed
     :py:class:`xarray.Dataset` with specific variables, dimensions, coordinates, dtypes,
-    and chunk structure. This is useful for "probabilistic" mode of pyCIAM, in which
-    you will run the model on a large ensemble of SLR trajectory realizations. In this
-    case, we save an empty Zarr store and then parallelize the model runs across
-    regions, with each processor writing to a region within the template store.
+    and chunk structure. This is useful for "probabilistic" mode of pyCIAM, in which you
+    will run the model on a large ensemble of SLR trajectory realizations. In this case,
+    we save an empty Zarr store and then parallelize the model runs across regions, with
+    each processor writing to a region within the template store.
 
     Parameters
     ----------
     var_dims : dict
         Keys are variable names. Values are lists of str, defining the dimensions
         that correspond to each variable.
     coords : dict
```

### Comparing `python-CIAM-1.1.2/pyCIAM/run.py` & `python-CIAM-1.2/pyCIAM/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """This module contains the central engine of pyCIAM, in which costs for all adaptation
 options are calculated.
 
 Functions
-    calc_costs
-    select_optimal_case
-    execute_pyciam
+---------
+* calc_costs
+* select_optimal_case
+* execute_pyciam
 """
 
 from collections import OrderedDict
 from shutil import rmtree
 
 import numpy as np
 import pandas as pd
@@ -79,17 +80,17 @@
         If not None, a DataArray containing at least ``lslr`` and ``rhdiff`` dimensions.
         This will be used to build a 2D spline function to interpolate extreme sea
         level-related damages, rather than calculating explicitly. This drastically
         improves execution time.
     elev_chunksize : int, default 1
         Number of elevation slices to process simultaneously. Higher numbers improve
         efficiency through vectorization but result in a larger memory footprint.
-    ddf_i, dmf_i : func, default :py:func:`.damage_funcs.ddf_i`, :py:func:`.damage_funcs.dmf_i`
-        Damage functions relating physical capital loss and monetized mortality arising
-        from a certain depth of inundation.
+    ddf_i, dmf_i : func, default :py:func:`.damage_funcs.ddf_i`,
+        :py:func:`.damage_funcs.dmf_i`. Damage functions relating physical capital loss
+        and monetized mortality arising from a certain depth of inundation.
     diaz_protect_height : bool, default False
         If True, reduce the 1-in-10-year extreme sea level by 50% as in Diaz 2016. This
         hack should not be necessary when using the ESL heights from CoDEC (as in
         SLIIDERS).
     diaz_construction_freq : bool, default False
         If True, set the lifetime over which the "linear" component of protection
         construction costs (i.e. the component that is proportional to length and not to
@@ -276,17 +277,17 @@
 
         # multiply fractional losses by seg-ir-level total capital and population
         surge["stormCapital"] = surge.stormCapital * inputs.K.sum("elev")
         surge["stormPopulation"] = surge.stormPopulation * inputs.pop.sum("elev")
         surge_noadapt["stormCapital"] = surge_noadapt.stormCapital * inputs.K.sum(
             "elev"
         )
-        surge_noadapt[
-            "stormPopulation"
-        ] = surge_noadapt.stormPopulation * inputs.pop.sum("elev")
+        surge_noadapt["stormPopulation"] = (
+            surge_noadapt.stormPopulation * inputs.pop.sum("elev")
+        )
     else:
         if surge_lookup is None:
             rh_years = RH_heights.sel(at=at).drop("at")
             min_hts = 0
             max_hts = inputs.surge_height.isel(return_period=-1, drop=True)
             surge_heights_probs = _get_surge_heights_probs(
                 min_hts, max_hts, inputs.gumbel_params
@@ -398,17 +399,17 @@
 
             # multiply fractional losses by seg-ir-level total capital and population
             surge["stormCapital"] = surge.stormCapital * inputs.K.sum("elev")
             surge["stormPopulation"] = surge.stormPopulation * inputs.pop.sum("elev")
             surge_noadapt["stormCapital"] = surge_noadapt.stormCapital * inputs.K.sum(
                 "elev"
             )
-            surge_noadapt[
-                "stormPopulation"
-            ] = surge_noadapt.stormPopulation * inputs.pop.sum("elev")
+            surge_noadapt["stormPopulation"] = (
+                surge_noadapt.stormPopulation * inputs.pop.sum("elev")
+            )
 
     surge = surge.stack(tmp=["adapttype", "return_period"])
     surge = (
         surge.assign(case=surge.adapttype.str.cat(surge.return_period.astype(str)))
         .swap_dims(tmp="case")
         .drop(["tmp", "adapttype", "return_period"])
     )
@@ -876,14 +877,15 @@
     slr_input_paths,
     slr_names,
     refA_path,
     econ_input_path_seg=None,
     surge_input_paths=None,
     output_path=None,
     tmp_output_path=AnyPath("pyciam_tmp_results.zarr"),
+    remove_tmpfile=True,
     overwrite=False,
     mc_dim="quantile",
     seg_var="seg_adm",
     seg_var_subset=None,
     adm_var="adm1",
     quantiles=[0.5],
     extra_attrs={},
@@ -891,15 +893,15 @@
     surge_batchsize=700,
     surge_seg_chunksize=5,
     refA_seg_chunksize=500,
     pyciam_seg_chunksize=3,
     diaz_inputs=False,
     diaz_config=False,
     dask_client_func=Client,
-    storage_options={},
+    storage_options=None,
     **model_kwargs
 ):
     """Execute the full pyCIAM model. The following inputs are assumed:
 
     - A socioeconomic input file in the format of `SLIIDERS`, organized by the
       intersection of coastal segments and some form of administrative unit (admin-1 in
       SLIIDERS).
@@ -953,14 +955,18 @@
     output_path : Path-like, optional
         Path to output cost predictions. If None (default), return the output as an
         xarray Dataset rather than writing to disk. This is only possible when running
         a smaller model (e.g. Diaz 2016)
     tmp_output_path : Path-like, default Path("pyciam_tmp_results.zarr")
         Path to temporary output zarr store that is written to and read from within this
         function. Ignored if `output_path` is not None.
+    remove_tmpfile : bool, default True
+        If True, remove the intermediate zarr store created before collapsing to
+        `adm_var` and rechunking. Setting to False can be useful for debugging if you
+        want to examine seg-adm level results.
     ovewrwrite : bool, default False
         If True, overwrite all intermediate output files
     mc_dim : str, default "quantile"
         The dimension of the sea level rise datasets specified at `slr_input_paths` that
         indexes different simulations within the same scenario. This could reflect Monte
         Carlo simulations *or* different quantiles of SLR. Ignored if
         `diaz_inputs=True`.
@@ -1048,14 +1054,17 @@
     ]
     if surge_input_paths is None:
         surge_input_paths = {k: None for k in {"seg", seg_var}}
     else:
         surge_input_paths = {k: AnyPath(v) for k, v in surge_input_paths.items()}
     slr_input_paths = [AnyPath(f) if f is not None else None for f in slr_input_paths]
 
+    if seg_var == "seg":
+        adm_var = "seg"
+
     # read parameters
     params = pd.read_json(params_path)["values"]
 
     # determine whether to check for finished jobs
     if output_path is None:
         check = False
         tmp_output_path = None
@@ -1091,15 +1100,14 @@
 
     ###########################################
     # create seg-level econ inputs if necessary
     ###########################################
     if seg_var == "seg":
         econ_input_path_seg = econ_input_path
     else:
-        assert tmp_output_path is not None
         if overwrite or not econ_input_path_seg.is_dir():
             collapse_econ_inputs_to_seg(
                 econ_input_path,
                 econ_input_path_seg,
                 seg_var_subset=seg_var_subset,
                 output_chunksize=econ_input_seg_chunksize,
                 storage_options=storage_options,
@@ -1378,21 +1386,23 @@
             storage_options=storage_options,
             chunks={"case": -1, seg_var: this_chunksize},
         )
         .drop("npv")
         .chunk({"year": 10})
         .persist()
     )
-    out["costs"] = (
-        out.costs.groupby(ciam_in[adm_var]).sum().chunk({adm_var: this_chunksize})
-    ).persist()
-    out["optimal_case"] = (
-        out.optimal_case.load().groupby(ciam_in.seg).first(skipna=False).chunk()
-    ).persist()
-    out = out.drop(seg_var).unify_chunks()
+    if adm_var != seg_var:
+        out["costs"] = (
+            out.costs.groupby(ciam_in[adm_var]).sum().chunk({adm_var: this_chunksize})
+        ).persist()
+        out["optimal_case"] = (
+            out.optimal_case.load().groupby(ciam_in.seg).first(skipna=False).chunk()
+        ).persist()
+        out = out.drop(seg_var)
+    out = out.unify_chunks()
 
     for v in out.data_vars:
         out[v].encoding.clear()
 
     for k, v in out.coords.items():
         if v.dtype == object:
             out[k] = v.astype("unicode")
@@ -1407,18 +1417,19 @@
     assert (
         xr.open_zarr(str(output_path), storage_options=storage_options)
         .costs.notnull()
         .all()
     )
     client.cluster.close()
     client.close()
-    if isinstance(tmp_output_path, CloudPath):
-        tmp_output_path.rmtree()
-    else:
-        rmtree(tmp_output_path)
+    if remove_tmpfile:
+        if isinstance(tmp_output_path, CloudPath):
+            tmp_output_path.rmtree()
+        else:
+            rmtree(tmp_output_path)
 
 
 def get_refA(
     segs,
     econ_input_path,
     slr_input_path,
     params,
@@ -1591,15 +1602,15 @@
 
     seg = "_".join(seg_adm.split("_")[:2])
     with xr.open_zarr(
         str(econ_input_path), storage_options=storage_options, chunks=None
     ) as ds:
         all_segs = ds.seg.load()
 
-    this_seg_adms = all_segs.seg_adm.isel({seg_var: all_segs.seg == seg}).values
+    this_seg_adms = all_segs[seg_var].isel({seg_var: all_segs.seg == seg}).values
 
     save_to_zarr_region(
         select_optimal_case(
             output_path,
             seg_adm,
             this_seg_adms,
             eps=eps,
```

### Comparing `python-CIAM-1.1.2/pyCIAM/surge/_calc.py` & `python-CIAM-1.2/pyCIAM/surge/_calc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-"""This private module contains functions related to specific calculations within
-pyCIAM that are called by the ``run`` module."""
+"""This private module contains functions related to specific calculations within pyCIAM
+that are called by the ``run`` module."""
 
 import numpy as np
 import xarray as xr
 from scipy.stats import gumbel_r
 
 from pyCIAM.surge.damage_funcs import diaz_ddf_i, diaz_dmf_i
 
 
 def _get_surge_heights_probs(
     min_surge_ht, max_surge_ht, gumbel_params, n_surge_heights=100
 ):
     """Create an array of ``n_surge_heights`` surge heights and associated probabilities
-    to apply in CIAM in order to sample an appropriate range of plausible surge heights.
-    """
+    to apply in CIAM in order to sample an appropriate range of plausible surge
+    heights."""
 
     # get gumbel params
     loc = gumbel_params.sel(params="loc", drop=True)
     scale = gumbel_params.sel(params="scale", drop=True)
 
     # get array of surge heights to model
     surge_hts = xr.apply_ufunc(
```

### Comparing `python-CIAM-1.1.2/pyCIAM/surge/damage_funcs.py` & `python-CIAM-1.2/pyCIAM/surge/damage_funcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """This module is used to define the fractional damage functions used in pyCIAM that
 relate storm surge depth to mortality and physical capital loss. As of April 7, 2022,
 the only functions available are those included in Diaz 2016. These define the
 "resilience-unadjusted" fractional damages. That is, for a region with resiliendce
-factor (:math:`\rho`) of 1, what fraction of the exposed population and/or physical capital
-will be lost conditional on a storm surge depth.
+factor (:math:`\rho`) of 1, what fraction of the exposed population and/or physical
+capital will be lost conditional on a storm surge depth.
 
 At the moment, functions must have an analytical integral and are actually defined by
 their integral, as can be seen with the suffix ``_i``.
 
 To add a new damage function, simply define it by its integral where depth is in units
 of meters. It must contain two mandatory arguments which refer to the bounds of the
 definite integral. Kwargs relevant for this particular damage function are optional.
@@ -47,15 +47,16 @@
         `depth_st` and `depth_end`.
     """
     return depth_end - depth_st + np.log(depth_st + 1) - np.log(depth_end + 1)
 
 
 def diaz_dmf_i(depth_st, depth_end, floodmortality=0.01):
     """Integral of mortality damage function as used in Diaz 2016, assuming unit
-    resilience (:math:`\rho`). It is just a constant fraction conditional on a unit of exposure being inundated. Note that kwargs are not optional and will raise an error
+    resilience (:math:`\rho`). It is just a constant fraction conditional on a unit of
+    exposure being inundated. Note that kwargs are not optional and will raise an error
     if not specified when called.
 
     Parameters
     ----------
     depth_{st,end} : float
         Define the lower and upper bounds of a definite integral
     floodmortality : float
```

### Comparing `python-CIAM-1.1.2/pyCIAM/surge/lookup.py` & `python-CIAM-1.2/pyCIAM/surge/lookup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 migration into future socioeconomic trajectories, one could do so through the use of
 year-specific lookup tables (a.k.a. spline functions).
 
 Public Functions:
     create_surge_lookup
 """
 
-
 import dask.array as da
 import numpy as np
 import pandas as pd
 import xarray as xr
 
 from pyCIAM.io import _load_lslr_for_ciam, save_to_zarr_region
 from pyCIAM.surge._calc import (
@@ -59,20 +58,23 @@
     include_cc=True,
     include_ncc=True,
     slr_0_years=2005,
     mc_dim="mc_sample_id",
     storage_options={},
 ):
     """Get the range of lslr and rhdiff that we need to model to cover the full range
-    across scenario/mcs. The minimum LSLR value we'll need to model for the purposes of
+    across scenario/mcs.
+
+    The minimum LSLR value we'll need to model for the purposes of
     assessing storm damage is the minimum across sites of: the site-level maximum of "0
     minus the s10000 surge height" and "the minimum projected LSLR for all of the
     scenario/mcs we use in our binned LSL dataset". The maximum LSLR value is the
     maximum experienced at any site in any year for all of the sceanrio/mcs we use in
-    the binned LSL dataset."""
+    the binned LSL dataset.
+    """
 
     if isinstance(slr_0_years, int):
         slr_0_years = [slr_0_years] * len(slr_stores)
     assert len(slr_0_years) == len(slr_stores)
     pc_in = _s2d(
         xr.open_zarr(
             str(sliiders_store), chunks=None, storage_options=storage_options
```

### Comparing `python-CIAM-1.1.2/pyCIAM/utils.py` & `python-CIAM-1.2/pyCIAM/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""This private module contains miscellaneous functions to support pyCIAM"""
+"""This private module contains miscellaneous functions to support pyCIAM."""
 
 import shutil
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 import xarray as xr
@@ -277,21 +277,26 @@
         str(output_path), storage_options=storage_options, mode="w"
     )
 
 
 def subset_econ_inputs(ds, seg_var, seg_var_subset):
     if seg_var_subset is None:
         return ds
-    if seg_var == "seg":
-        return ds.sel(seg=ds.seg.str.contains(seg_var_subset))
 
-    necessary_segs = np.unique(
-        ds.seg.sel({seg_var: ds[seg_var].str.contains(seg_var_subset)})
-    )
-    return ds.sel({seg_var: ds.seg.isin(necessary_segs)})
+    if isinstance(seg_var_subset, str):
+        if seg_var == "seg":
+            subsetter = ds.seg.str.contains(seg_var_subset)
+        else:
+            subsetter = ds.seg.isin(
+                np.unique(
+                    ds.seg.sel({seg_var: ds[seg_var].str.contains(seg_var_subset)})
+                )
+            )
+
+    return ds.sel({seg_var: subsetter})
 
 
 def copy(path_src, path_trg):
     if isinstance(path_src, Path):
         if isinstance(path_trg, CloudPath):
             path_trg.upload_from(path_src)
         elif isinstance(path_trg, Path):
```

### Comparing `python-CIAM-1.1.2/python_CIAM.egg-info/PKG-INFO` & `python-CIAM-1.2/python_CIAM.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-CIAM
-Version: 1.1.2
+Version: 1.2
 Summary: An efficient Python implementation of the Coastal Impacts and Adaptation Model (CIAM)
 Home-page: https://gitlab.com/ClimateImpactLab/coastal/projects/pyciam
 Author: Ian Bolliger, Nicholas Depsky
 Author-email: ian.bolliger@blackrock.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `python-CIAM-1.1.2/python_CIAM.egg-info/SOURCES.txt` & `python-CIAM-1.2/python_CIAM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-CIAM-1.1.2/setup.cfg` & `python-CIAM-1.2/setup.cfg`

 * *Files identical despite different names*

