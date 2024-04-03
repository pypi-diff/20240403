# Comparing `tmp/lyscripts-1.0.0a0.tar.gz` & `tmp/lyscripts-1.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyscripts-1.0.0a0.tar", last modified: Wed Dec 20 15:02:33 2023, max compression
+gzip compressed data, was "lyscripts-1.0.0a1.tar", last modified: Wed Apr  3 13:01:05 2024, max compression
```

## Comparing `lyscripts-1.0.0a0.tar` & `lyscripts-1.0.0a1.tar`

### file list

```diff
@@ -1,81 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 15:02:33.085711 lyscripts-1.0.0a0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 15:02:33.073711 lyscripts-1.0.0a0/.chglog/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1044 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/.chglog/CHANGELOG.tpl.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      815 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/.chglog/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 15:02:33.069711 lyscripts-1.0.0a0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 15:02:33.073711 lyscripts-1.0.0a0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      667 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      791 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13331 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8391 2023-12-20 15:02:33.085711 lyscripts-1.0.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7214 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    18415 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)   105407 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/github-social-card.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 15:02:33.073711 lyscripts-1.0.0a0/lyscripts/
--rw-r--r--   0 runner    (1001) docker     (127)     3838 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/lyscripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/lyscripts/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2023-12-20 15:02:32.000000 lyscripts-1.0.0a0/lyscripts/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 15:02:33.077711 lyscripts-1.0.0a0/lyscripts/app/
--rw-r--r--   0 runner    (1001) docker     (127)      617 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/lyscripts/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10466 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/lyscripts/app/prevalence.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 15:02:33.077711 lyscripts-1.0.0a0/lyscripts/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/lyscripts/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/lyscripts/data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13632 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/lyscripts/data/enhance.py
--rw-r--r--   0 runner    (1001) docker     (127)     5364 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/lyscripts/data/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/lyscripts/data/join.py
--rw-r--r--   0 runner    (1001) docker     (127)    13116 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/lyscripts/data/lyproxify.py
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/lyscripts/data/split.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/lyscripts/data/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5456 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/lyscripts/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     8401 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/lyscripts/evaluate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 15:02:33.077711 lyscripts-1.0.0a0/lyscripts/plot/
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/lyscripts/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/lyscripts/plot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/lyscripts/plot/corner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4060 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/lyscripts/plot/histograms.py
--rw-r--r--   0 runner    (1001) docker     (127)     5922 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/lyscripts/plot/thermo_int.py
--rw-r--r--   0 runner    (1001) docker     (127)     9787 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/lyscripts/plot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 15:02:33.081711 lyscripts-1.0.0a0/lyscripts/predict/
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/lyscripts/predict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/lyscripts/predict/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14197 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/lyscripts/predict/prevalences.py
--rw-r--r--   0 runner    (1001) docker     (127)     6784 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/lyscripts/predict/risks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/lyscripts/predict/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17962 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/lyscripts/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     4812 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/lyscripts/temp_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)    13910 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/lyscripts/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 15:02:33.085711 lyscripts-1.0.0a0/lyscripts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8391 2023-12-20 15:02:33.000000 lyscripts-1.0.0a0/lyscripts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2023-12-20 15:02:33.000000 lyscripts-1.0.0a0/lyscripts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-20 15:02:33.000000 lyscripts-1.0.0a0/lyscripts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2023-12-20 15:02:33.000000 lyscripts-1.0.0a0/lyscripts.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      203 2023-12-20 15:02:33.000000 lyscripts-1.0.0a0/lyscripts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-12-20 15:02:33.000000 lyscripts-1.0.0a0/lyscripts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-20 15:02:33.085711 lyscripts-1.0.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 15:02:33.081711 lyscripts-1.0.0a0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 15:02:33.081711 lyscripts-1.0.0a0/tests/plot/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 15:02:33.081711 lyscripts-1.0.0a0/tests/plot/baseline/
--rw-r--r--   0 runner    (1001) docker     (127)    12265 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/tests/plot/baseline/sine.png
--rw-r--r--   0 runner    (1001) docker     (127)    12916 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/tests/plot/baseline/sine.svg
--rw-r--r--   0 runner    (1001) docker     (127)    12629 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/tests/plot/baseline/sine_svg.png
--rw-r--r--   0 runner    (1001) docker     (127)    36976 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/tests/plot/baseline/test_draw.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 15:02:33.081711 lyscripts-1.0.0a0/tests/plot/data/
--rw-r--r--   0 runner    (1001) docker     (127)    86144 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/tests/plot/data/beta_samples.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)     8094 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/tests/plot/plot_utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 15:02:33.085711 lyscripts-1.0.0a0/tests/predict/
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/tests/predict/predict_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/tests/predict/prevalences_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/tests/run_doctests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/tests/sample_test.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/tests/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   397288 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/tests/test_backend.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)      509 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/tests/test_data.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/tests/test_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2023-12-20 15:02:11.000000 lyscripts-1.0.0a0/tests/utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.329456 lyscripts-1.0.0a1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.309456 lyscripts-1.0.0a1/.chglog/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1044 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/.chglog/CHANGELOG.tpl.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      815 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/.chglog/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.305456 lyscripts-1.0.0a1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.309456 lyscripts-1.0.0a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    18137 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-04-03 13:01:05.329456 lyscripts-1.0.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.313456 lyscripts-1.0.0a1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.313456 lyscripts-1.0.0a1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.313456 lyscripts-1.0.0a1/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.313456 lyscripts-1.0.0a1/docs/source/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)    18415 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/_static/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)   105407 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/_static/github-social-card.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.313456 lyscripts-1.0.0a1/docs/source/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/app/init.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/app/prevalence.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.313456 lyscripts-1.0.0a1/docs/source/compute/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/compute/init.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/compute/posteriors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/compute/prevalences.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/compute/priors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/compute/risks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/compute/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.317456 lyscripts-1.0.0a1/docs/source/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/data/enhance.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/data/filter.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/data/generate.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/data/init.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/data/join.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/data/lyproxify.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/data/split.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/data/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/decorators.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/evaluate.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/init.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.317456 lyscripts-1.0.0a1/docs/source/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/plot/corner.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/plot/histograms.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/plot/init.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/plot/thermo_int.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/plot/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/sample.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/scenario.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/temp_schedule.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    18415 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)   105407 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/github-social-card.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.317456 lyscripts-1.0.0a1/lyscripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-03 13:01:05.000000 lyscripts-1.0.0a1/lyscripts/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.321456 lyscripts-1.0.0a1/lyscripts/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10514 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/app/prevalence.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.321456 lyscripts-1.0.0a1/lyscripts/compute/
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/compute/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/compute/posteriors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10108 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/compute/prevalences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/compute/priors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/compute/risks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/compute/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.321456 lyscripts-1.0.0a1/lyscripts/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/data/accessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10189 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/data/enhance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/data/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/data/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/data/join.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11223 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/data/lyproxify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/data/split.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6656 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/evaluate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.321456 lyscripts-1.0.0a1/lyscripts/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/plot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/plot/corner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/plot/histograms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/plot/thermo_int.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9900 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/plot/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12124 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/temp_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16344 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.329456 lyscripts-1.0.0a1/lyscripts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-04-03 13:01:05.000000 lyscripts-1.0.0a1/lyscripts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-03 13:01:05.000000 lyscripts-1.0.0a1/lyscripts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 13:01:05.000000 lyscripts-1.0.0a1/lyscripts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-03 13:01:05.000000 lyscripts-1.0.0a1/lyscripts.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-03 13:01:05.000000 lyscripts-1.0.0a1/lyscripts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 13:01:05.000000 lyscripts-1.0.0a1/lyscripts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 13:01:05.329456 lyscripts-1.0.0a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.325456 lyscripts-1.0.0a1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.325456 lyscripts-1.0.0a1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/tests/data/a.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/tests/data/b.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/tests/data/join_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.325456 lyscripts-1.0.0a1/tests/plot/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.325456 lyscripts-1.0.0a1/tests/plot/baseline/
+-rw-r--r--   0 runner    (1001) docker     (127)    12265 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/tests/plot/baseline/sine.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12916 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/tests/plot/baseline/sine.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    12629 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/tests/plot/baseline/sine_svg.png
+-rw-r--r--   0 runner    (1001) docker     (127)    36976 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/tests/plot/baseline/test_draw.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.325456 lyscripts-1.0.0a1/tests/plot/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    86144 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/tests/plot/data/beta_samples.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)     8110 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/tests/plot/plot_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.329456 lyscripts-1.0.0a1/tests/predict/
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/tests/predict/predict_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/tests/predict/prevalences_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/tests/run_doctests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/tests/sample_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/tests/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   397288 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/tests/test_backend.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/tests/test_data.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/tests/test_params_v0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/tests/test_params_v1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/tests/test_sample_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/tests/utils_test.py
```

### Comparing `lyscripts-1.0.0a0/.chglog/CHANGELOG.tpl.md` & `lyscripts-1.0.0a1/.chglog/CHANGELOG.tpl.md`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a0/.chglog/config.yml` & `lyscripts-1.0.0a1/.chglog/config.yml`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a0/.github/workflows/build.yml` & `lyscripts-1.0.0a1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a0/.github/workflows/tests.yml` & `lyscripts-1.0.0a1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a0/.gitignore` & `lyscripts-1.0.0a1/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -68,17 +68,14 @@
 # Flask stuff:
 instance/
 .webassets-cache
 
 # Scrapy stuff:
 .scrapy
 
-# documentation
-/docs
-
 # PyBuilder
 target/
 
 # Jupyter Notebook
 .ipynb_checkpoints
 
 # IPython
```

### Comparing `lyscripts-1.0.0a0/.pre-commit-config.yaml` & `lyscripts-1.0.0a1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a0/CHANGELOG.md` & `lyscripts-1.0.0a1/CHANGELOG.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,138 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
+<a name="1.0.0.a1"></a>
+## [1.0.0.a1] - 2024-04-03
+
+This prerelease finishes updating the code to the new [`lymph`] package API. It also features a rewrite of the commands to predict and compute e.g. risks and prevalences.
+
+[`lymph`]: https://lymph-model.readthedocs.io
+
+
+### Bug Fixes
+
+- ⚠ **BREAKING** Use modern lydata cols for t_stage matching.
+- Wrong lnls in predict prevalences.
+- ⚠ **BREAKING** Update prevalence prediction to new lymph API.
+- (**sample**) Match T-stage mapping with lymph API.\
+  The lymph model now accepts callables and dicts as T-stage mapping (but
+  not `None`). I can hence simply pass the dictionary from the config to
+  the loading function.
+- (**data**) Stop dtype change during `concat`.\
+  When a `DataFrame` with no `NaN`s was joined with one consisting _only_
+  of `NaN`s, then it forced some weird kind of dtype conversion onty the
+  respective column. Now, dtypes are converted _before_ the concatenation,
+  fixing that issue.
+- (**sample**) Skip 0 iter convergence check.
+- (**sample**) Missing import.
+- (**sample**) Only pass `side` to unilateral model.
+- (**sample**) Display converged message nicely.
+- (**utils**) Correct default args for `get_chain()`.
+- Wrong posterior shape.
+- (**predict**) Even out some bugs.
+- Don't pycln accessor import.
+- (**data**) Enhance failed due to copy on write.
+
+### Documentation
+
+- Start with basic sphinx setup.
+- Start organizing top-level cmds with sphinx.
+- Include all modules in docs.
+- Update docstrings to reST format.
+- Add document files for precompute subcmd.
+- Allow links to lymph docs.
+- Fix `temp_schedule` docstring.
+- Shorten titles.
+- (**predict**) Update prevalence module docstring.
+- Refactor docs for new `compute` subcommand.
+- Fix typos and missing modules.
+
+### Features
+
+- (**data**) Add simple data filter command. Fixes [#51].
+- Customize log handler for better filename.
+- (**sample**) Allow custom T-stage mapping.
+- (**sample**) Allow to load `side` data.
+- (**utils**) Allow `Unilateral.binary` in params.
+- (**sample**) Display time elapsed during burnin.
+- (**predict**) Add cmd to precompute state dists.
+- (**precompute**) Add `priors` cmd. Related [#54].\
+  This allows precomputing the state distributions of all three
+  implemented lymph models.
+- (**utils**) Allow keywords in modalities def.\
+  One may now use a dict with keys `spec`, `sens`, and `kind` to define a
+  modality in the YAML params.
+- (**post**) Compute for multiple scenarios.\
+  One may now compute the posteriors for a list of defined scenarios.
+- Add class for storing scenarios.
+- (**precompute**) Priors from list of scenarios.
+- (**predict**) Finish prevalences cmd.
+- (**data**) Implement custom pandas accessor.
+- (**scenario**) Track laterality as well.
+- (**compute**) Risk works with lymph v1, too, now.
+
+### Testing
+
+- (**data**) Ensure new joining works correctly.
+- (**sample**) Check some sampling methods.
+- Fix typos in tests.
+- Update failing tests.
+
+### Build
+
+- Bump lymph-model to v1.0.
+- Bump lymph version & add sphinx deps.
+
+### Change
+
+- ⚠ **BREAKING** (**sample**) Reimplement sampling command.
+- (**precompute**) Use HDF5 cache. Fixes [#54].\
+  The `priors` and `posteriors` commands now use a simple `HDF5FileCache`
+  to avoid recomputing either of those quantities unnecessarily.
+- (**precompute**) Make recursive. Related [#54].\
+  The computation of priors and posteriors is now somewhat recursive. This
+  will allow us to just call one function and it will automatically
+  compute the priors, posteriors, and risks if necessary.
+- (**prevs**) Start on updated `prevalences` cmd.
+- Replace 'diagnose' & bump lymph to 1.2.0.
+- (**precompute**) Posteriors only from priors.\
+  Posteriors now require priors and cannot compute priors "along the way"
+  from given samples. This is to make it clear which is an input file and
+  which an output file. Otherwise, caching would have been even trickier.
+- (**scenario**) Shorten hash to 6 digits.
+
+### Ci
+
+- Add readthedocs config file.
+- Remove pdoc action.
+
+### Merge
+
+- Branch 'main' into 'dev'.
+- Branch '51-filter-command' into 'dev'.
+- Branch '53-use-sphinx-for-documentation' into 'dev'.
+- Branch '54-add-precompute-commands' into 'dev'.
+
+### Refac
+
+- (**sample**) Better progress tracking.
+- (**precompute**) Comp state dist in own submod.
+- (**utils**) Move funcs out of `precompute`.
+- Bundle adding scneario args to parser.
+- (**compute**) Predict & precompute -> compute.\
+  The `predict` and `precompute` commands are now bundled under the
+  subcommand `compute`.
+
+
+### Remove
+
+- ⚠ **BREAKING** Midline_ext in create_patient_row for now.
+
 
 <a name="1.0.0.a0"></a>
 ## [1.0.0.a0] - 2023-12-20
 
 ### Bug Fixes
 
 - Update imports to new lymph version
@@ -346,15 +473,16 @@
 - set up git-chglog for creating changelogs
 - add pre-commit hook to check commit msg
 
 
 <a name="0.5.3"></a>
 ## [0.5.3] - 2022-08-22
 
-[Unreleased]: https://github.com/rmnldwg/lyscripts/compare/1.0.0.a0...HEAD
+[Unreleased]: https://github.com/rmnldwg/lyscripts/compare/1.0.0.a1...HEAD
+[1.0.0.a1]: https://github.com/rmnldwg/lyscripts/compare/1.0.0.a0...1.0.0.a1
 [1.0.0.a0]: https://github.com/rmnldwg/lyscripts/compare/0.7.3...1.0.0.a0
 [0.7.3]: https://github.com/rmnldwg/lyscripts/compare/0.7.2...0.7.3
 [0.7.2]: https://github.com/rmnldwg/lyscripts/compare/0.7.1...0.7.2
 [0.7.1]: https://github.com/rmnldwg/lyscripts/compare/0.7.0...0.7.1
 [0.7.0]: https://github.com/rmnldwg/lyscripts/compare/0.6.9...0.7.0
 [0.6.9]: https://github.com/rmnldwg/lyscripts/compare/0.6.8...0.6.9
 [0.6.8]: https://github.com/rmnldwg/lyscripts/compare/0.6.7...0.6.8
@@ -391,12 +519,14 @@
 [#30]: https://github.com/rmnldwg/lyscripts/issues/30
 [#31]: https://github.com/rmnldwg/lyscripts/issues/31
 [#33]: https://github.com/rmnldwg/lyscripts/issues/33
 [#40]: https://github.com/rmnldwg/lyscripts/issues/40
 [#41]: https://github.com/rmnldwg/lyscripts/issues/41
 [#44]: https://github.com/rmnldwg/lyscripts/issues/44
 [#45]: https://github.com/rmnldwg/lyscripts/issues/45
+[#51]: https://github.com/rmnldwg/lyscripts/issues/51
+[#54]: https://github.com/rmnldwg/lyscripts/issues/54
 
 [`emcee`]: https://emcee.readthedocs.io/en/stable/
 [`rich`]: https://rich.readthedocs.io/en/latest/
 [`rich_argparse`]: https://github.com/hamdanal/rich_argparse
 [LyProX]: https://lyprox.org
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `lyscripts-1.0.0a0/LICENSE` & `lyscripts-1.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a0/favicon.png` & `lyscripts-1.0.0a1/docs/source/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a0/github-social-card.png` & `lyscripts-1.0.0a1/docs/source/_static/github-social-card.png`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a0/lyscripts/__init__.py` & `lyscripts-1.0.0a1/lyscripts/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,51 +1,62 @@
 """
-.. include:: ../README.md
+This is the top-level module of the `lyscripts` package. It contains the
+:py:func:`.main` function that is used to start the command line interface (CLI) for
+the package.
+
+Also, it configures the logging system and sets the metadate of the package.
 """
 import argparse
 import logging
 import re
 
-from rich.containers import Lines
-from rich.logging import RichHandler
-from rich.text import Text
+import pandas as pd
+import rich
 from rich_argparse import RichHelpFormatter
 
-from lyscripts import app, data, evaluate, plot, predict, sample, temp_schedule
+from lyscripts import app, compute, data, evaluate, plot, sample, temp_schedule
 from lyscripts._version import version
-from lyscripts.utils import report
+from lyscripts.utils import CustomRichHandler, console
 
 __version__ = version
 __description__ = "Package containing scripts used in lynference pipelines"
 __author__ = "Roman Ludwig"
 __email__ = "roman.ludwig@usz.ch"
 __uri__ = "https://github.com/rmnldwg/lyscripts"
 
 # nopycln: file
 
+# activate copy on write in pandas.
+# See https://pandas.pydata.org/docs/user_guide/copy_on_write.html
+pd.options.mode.copy_on_write = True
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
 
 
 class RichDefaultHelpFormatter(
     RichHelpFormatter,
     argparse.ArgumentDefaultsHelpFormatter,
 ):
+    """Combine formatter that shows defaults with `rich`_ formatting.
+
+    .. _rich: https://rich.readthedocs.io/en/stable/introduction.html
     """
-    Empty class that combines the functionality of displaying the default value with
-    the beauty of the `rich` formatter
-    """
-    def _rich_fill_text(self, text: Text, width: int, indent: Text) -> Text:
+    def _rich_fill_text(
+        self,
+        text: rich.text.Text,
+        width: int,
+        indent: rich.text.Text,
+    ) -> rich.text.Text:
         text_cls = type(text)
         if text[0] == text_cls("\n"):
             text = text[1:]
 
         paragraphs = text.split(separator="\n\n")
-        text_lines = Lines()
+        text_lines = rich.containers.Lines()
         for par in paragraphs:
             no_newline_par = text_cls(" ").join(line for line in par.split())
             wrapped_par = no_newline_par.wrap(self.console, width)
 
             for line in wrapped_par:
                 text_lines.append(line)
 
@@ -68,24 +79,21 @@
     r"_(?P<italic>[^_]*)_"
 )
 
 
 def exit_cli(args: argparse.Namespace):
     """Exit the cmd line tool"""
     if args.version:
-        report.print("lyscripts ", __version__)
+        logger.info(f"lyscripts {__version__}")
     else:
-        report.print("No command chosen. Exiting...")
+        logger.warning("No command chosen. Exiting...")
 
 
 def main():
-    """
-    Utility for performing common tasks w.r.t. the inference and prediction tasks one
-    can use the `lymph` package for.
-    """
+    """Execute the main program."""
     parser = argparse.ArgumentParser(
         prog="lyscripts",
         description=re.sub(r"\s+", " ", main.__doc__)[1:],
         formatter_class=RichDefaultHelpFormatter,
     )
     parser.set_defaults(run_main=exit_cli)
     parser.add_argument(
@@ -98,26 +106,27 @@
     )
 
     subparsers = parser.add_subparsers()
 
     # the individual scripts add `ArgumentParser` instances and their arguments to
     # this `subparsers` object
     app._add_parser(subparsers, help_formatter=parser.formatter_class)
+    compute._add_parser(subparsers, help_formatter=parser.formatter_class)
     data._add_parser(subparsers, help_formatter=parser.formatter_class)
     evaluate._add_parser(subparsers, help_formatter=parser.formatter_class)
     plot._add_parser(subparsers, help_formatter=parser.formatter_class)
-    predict._add_parser(subparsers, help_formatter=parser.formatter_class)
     sample._add_parser(subparsers, help_formatter=parser.formatter_class)
     temp_schedule._add_parser(subparsers, help_formatter=parser.formatter_class)
 
     args = parser.parse_args()
 
-    handler = RichHandler(
-        console=report,
+    handler = CustomRichHandler(
+        console=console,
         show_time=False,
-        markup=True,
+        markup=False,
+        highlighter=rich.highlighter.NullHighlighter(),
     )
     handler.setFormatter(logging.Formatter("%(message)s"))
     logger.addHandler(handler)
     logger.setLevel(args.log_level)
 
     args.run_main(args)
```

### Comparing `lyscripts-1.0.0a0/lyscripts/app/prevalence.py` & `lyscripts-1.0.0a1/lyscripts/app/prevalence.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,77 +1,76 @@
 """
-A `streamlit` app for computing, displaying and reproducing prevalence estimates.
+A `streamlit`_ app for computing, displaying, and reproducing prevalence estimates.
 
 The primary goal with this little GUI is that one can quickly draft some data &
 prediction comparisons visually and then copy & paste the configuration in YAML format
-that is necessary to reproduce this via the `lyscripts.predict.prevalences` script.
+that is necessary to reproduce this via the :py:mod:`.predict.prevalences` script.
+
+.. _streamlit: https://streamlit.io/
 """
 import argparse
 import sys
 from pathlib import Path
 from types import ModuleType
 from typing import Any
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import yaml
-from lymph import models
+from lymph import models, types
 
-from lyscripts.plot.utils import COLOR_CYCLE, Histogram, Posterior, draw
-from lyscripts.predict.prevalences import (
+from lyscripts.compute.prevalences import (  # generate_predicted_prevalences,
     compute_observed_prevalence,
-    generate_predicted_prevalences,
 )
-from lyscripts.predict.utils import complete_pattern, reduce_pattern
+from lyscripts.compute.utils import complete_pattern, reduce_pattern
+from lyscripts.plot.utils import COLOR_CYCLE, BetaPosterior, Histogram, draw
 from lyscripts.utils import (
-    LymphModel,
-    create_model_from_config,
-    load_hdf5_samples,
+    create_model,
+    load_model_samples,
     load_patient_data,
     load_yaml_params,
 )
 
 
 def _add_parser(
     subparsers: argparse._SubParsersAction,
     help_formatter,
 ):
-    """
-    Add an `ArgumentParser` to the subparsers action.
-    """
+    """Add a parser to ``subparsers`` and call :py:func:`_add_arguments` with it."""
     parser = subparsers.add_parser(
         Path(__file__).name.replace(".py", ""),
         description=__doc__,
         help=__doc__,
         formatter_class=help_formatter,
     )
     _add_arguments(parser)
 
 
 def _add_arguments(parser: argparse.ArgumentParser):
-    """
-    Add arguments needed to run this `streamlit` app.
+    """Add arguments needed to run this `streamlit`_ app.
+
+    .. _streamlit: https://streamlit.io/
     """
     parser.add_argument(
         "--message", type=str,
         help="Print our this little message."
     )
 
     parser.set_defaults(run_main=launch_streamlit)
 
 
 def launch_streamlit(*_args, discard_args_idx: int = 3, **_kwargs):
-    """
-    Regardless of the entry point into this script, this function will start
-    `streamlit` and pass on the provided command line arguments.
+    """Start the `streamlit`_ app with the given arguments.
 
-    It will discard all entries in the `sys.argv` that come before the
-    `discard_args_idx`, because this also usually contains e.g. the name of the current
-    file that might not be relevant to the streamlit app.
+    It will discard all entries in the ``sys.argv`` that come before the
+    ``discard_args_idx``, because this also usually contains e.g. the name of the
+    current file that might not be relevant to the streamlit app.
+
+    .. _streamlit: https://streamlit.io/
     """
     try:
         from streamlit.web.cli import main as st_main
     except ImportError as mnf_err:
         raise ImportError(
             "Install lyscripts with the `apps` option to install the necessary "
             "requirements for running the streamlit apps."
@@ -102,58 +101,55 @@
     elif not selected:
         return "Lateralized"
     else:
         raise ValueError("Selected option can only be `True`, `False` or `None`.")
 
 
 def interactive_load(streamlit):
-    """
-    Load the YAML file defining the parameters, the CSV file with the patient data
-    and the HDF5 file with the drawn model samples interactively.
-    """
+    """Load YAML parameters, CSV patient data, and HDF5 samples interactively."""
     params_file = streamlit.file_uploader(
         label="YAML params file",
         type=["yaml", "yml"],
         help="Parameter YAML file containing configurations w.r.t. the model etc.",
     )
     params = load_yaml_params(params_file)
-    model = create_model_from_config(params)
+    model = create_model(params)
     is_unilateral = isinstance(model, models.Unilateral)
 
     streamlit.write("---")
 
     data_file = streamlit.file_uploader(
         label="CSV file of patient data",
         type=["csv"],
         help="CSV spreadsheet containing lymphatic patterns of progression",
     )
     header_rows = [0,1] if is_unilateral else [0,1,2]
-    patient_data = load_patient_data(data_file, header_rows=header_rows)
+    patient_data = load_patient_data(data_file, header=header_rows)
 
     streamlit.write("---")
 
     samples_file = streamlit.file_uploader(
         label="HDF5 sample file",
         type=["hdf5", "hdf", "h5"],
         help="HDF5 file containing the samples."
     )
-    samples = load_hdf5_samples(samples_file)
+    samples = load_model_samples(samples_file)
 
     return model, patient_data, samples
 
 
 def interactive_pattern(
     streamlit,
     is_unilateral: bool,
     lnls: list[str],
     side: str
 ) -> dict[str, bool]:
-    """
-    Create a `streamlit` panel for all specified `lnls` in one `side` of a patient's
-    neck to specify the lymphatic pattern of interest, which is then returned.
+    """Create a `streamlit`_ panel for specifying an involvement pattern.
+
+    Fill this panel with radio buttons for each of the ``lnls`` of the given ``side``.
     """
     streamlit.subheader(f"{side}lateral")
     side_pattern = {}
 
     if side == "contra" and is_unilateral:
         return side_pattern
 
@@ -168,20 +164,21 @@
         )
 
     return side_pattern
 
 
 def interactive_additional_params(
     streamlit: ModuleType,
-    model: LymphModel,
+    model: types.Model,
     data: pd.DataFrame,
     samples: np.ndarray,
 ) -> dict[str, Any]:
-    """
-    Allow the user to select T-category, midline extension and whether to invert the
+    """Add other selectors to the `streamlit`_ panel.
+
+    Allows the user to select T-category, midline extension and whether to invert the
     computed prevalence (meaning computing $1 - p$, when $p$ is the prevalence).
 
     The respective controls are presented next to each other in three dedicated columns.
     """
     control_cols = streamlit.columns([1,2,1,1,1])
     t_stage = control_cols[0].selectbox(
         label="T-category",
@@ -222,36 +219,39 @@
         "midline_ext": midline_ext,
         "invert": invert,
         "thin": thin,
     }
 
 
 def reset(session_state: dict[str, Any]):
-    """Reset `streamlit` session state."""
+    """Reset `streamlit`_ session state.
+
+    .. _streamlit: https://streamlit.io/
+    """
     for key in session_state.keys():
         del session_state[key]
 
 
 def add_current_scenario(
     session_state: dict[str, Any],
     pattern: dict[str, dict[str, bool]],
-    model: LymphModel,
+    model: types.Model,
     samples: np.ndarray,
     data: pd.DataFrame,
     prevs_kwargs: dict[str, Any] | None = None,
-) -> list[Histogram | Posterior]:
-    """
-    Compute the prevalence of a `pattern` as observed in the `data` and as predicted
-    by the `model` (using a set of `samples`). The results are then stored in the
-    `contents` list ready to be plotted. The `prevs_kwargs` are directly passed on to
-    the functions `lyscripts.predict.prevalences.compute_observed_prevalence`
-    and `lyscripts.predict.prevalences.generate_predicted_prevalences`.
+) -> list[Histogram | BetaPosterior]:
+    """Compute prevalence of ``pattern`` as seem in ``data`` and predicted by ``model``.
+
+    This uses a set of ``samples``. The results are then stored in the ``contents``
+    list ready to be plotted. The ``prevs_kwargs`` are directly passed on to
+    the functions :py:func:`.predict.prevalences.compute_observed_prevalence`
+    and :py:func:`.predict.prevalences.generate_predicted_prevalences`.
     """
     num_success, num_total = compute_observed_prevalence(
-        pattern=pattern,
+        diagnosis=pattern,
         data=data,
         lnls=len(model.get_params()),
         **prevs_kwargs,
     )
 
     prevs_gen = generate_predicted_prevalences(
         pattern=pattern,
@@ -260,29 +260,29 @@
         **prevs_kwargs,
     )
     computed_prevs = np.zeros(shape=len(samples))
     for i, prevalence in enumerate(prevs_gen):
         computed_prevs[i] = prevalence
 
     next_color = next(COLOR_CYCLE)
-    beta_posterior = Posterior(num_success, num_total, kwargs={"color": next_color})
+    beta_posterior = BetaPosterior(num_success, num_total, kwargs={"color": next_color})
     histogram = Histogram(computed_prevs, kwargs={"color": next_color})
 
     session_state["contents"].append(beta_posterior)
     session_state["contents"].append(histogram)
 
     session_state["scenarios"].append({
         "pattern": reduce_pattern(pattern), **prevs_kwargs
     })
 
 
 def main(args: argparse.Namespace):
-    """
-    The main function that contains the `streamlit` code and main functionality.
-    """
+    """The main function that contains the `streamlit`_ code and functionality.
+
+    .. _streamlit: https://streamlit.io/"""
     import streamlit as st
 
     st.title("Prevalence")
 
     with st.sidebar:
         model, patient_data, samples = interactive_load(st)
```

### Comparing `lyscripts-1.0.0a0/lyscripts/data/__init__.py` & `lyscripts-1.0.0a1/lyscripts/plot/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,26 @@
 """
-Provide a range of commands related to datasets on patterns of lymphatic progression.
-Currently, the following modules provide additional commands:
-
-1. `lyscripts.data.enhance`, a module for computing consensus diagnoses and to ensure
-that super- and sublevels are consistently reported.
-2. The module `lyscripts.data.generate` for creating synthetic datasets with certain
-characteristics.
-3. Submodule `lyscripts.data.join` to concatenate two datasets, e.g. from different
-institutions.
-4. `lyscripts.data.split`, a module with which datasets may be split into random sets
-of patient data. The split data may then be used e.g. for cross-validation.
+Provide various plotting utilities for displaying results of e.g. the inference
+or prediction process. At the moment, three subcommands are grouped under
+:py:mod:`.plot`.
 """
 import argparse
 from pathlib import Path
 
-from . import enhance, generate, join, lyproxify, split
+from lyscripts.plot import corner, histograms, thermo_int
 
 
 def _add_parser(
     subparsers: argparse._SubParsersAction,
     help_formatter,
 ):
-    """
-    Add an `ArgumentParser` to the subparsers action and then add more subparsers.
-    """
+    """Add an ``ArgumentParser`` to the subparsers and then add more subparsers."""
     parser = subparsers.add_parser(
         Path(__file__).parent.name,
         description=__doc__,
         help=__doc__,
         formatter_class=help_formatter,
     )
     subparsers = parser.add_subparsers()
-    enhance._add_parser(subparsers, help_formatter=parser.formatter_class)
-    generate._add_parser(subparsers, help_formatter=parser.formatter_class)
-    join._add_parser(subparsers, help_formatter=parser.formatter_class)
-    lyproxify._add_parser(subparsers, help_formatter=parser.formatter_class)
-    split._add_parser(subparsers, help_formatter=parser.formatter_class)
+    corner._add_parser(subparsers, help_formatter=parser.formatter_class)
+    histograms._add_parser(subparsers, help_formatter=parser.formatter_class)
+    thermo_int._add_parser(subparsers, help_formatter=parser.formatter_class)
```

### Comparing `lyscripts-1.0.0a0/lyscripts/data/__main__.py` & `lyscripts-1.0.0a1/lyscripts/data/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import argparse
 
 from lyscripts import RichDefaultHelpFormatter, exit_cli
-from lyscripts.data import clean, enhance, generate, join, split
+from lyscripts.data import enhance, filter, generate, join, split
 
 # I need another __main__ guard here, because otherwise pdoc tries to run this
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(
         prog="lyscripts data",
         description=__doc__,
         formatter_class=RichDefaultHelpFormatter,
     )
     parser.set_defaults(run_main=exit_cli)
     subparsers = parser.add_subparsers()
 
     # the individual scripts add `ArgumentParser` instances and their arguments to
     # this `subparsers` object
-    clean._add_parser(subparsers, help_formatter=parser.formatter_class)
     enhance._add_parser(subparsers, help_formatter=parser.formatter_class)
     generate._add_parser(subparsers, help_formatter=parser.formatter_class)
     join._add_parser(subparsers, help_formatter=parser.formatter_class)
     split._add_parser(subparsers, help_formatter=parser.formatter_class)
+    filter._add_parser(subparsers, help_formatter=parser.formatter_class)
 
     args = parser.parse_args()
     args.run_main(args)
```

### Comparing `lyscripts-1.0.0a0/lyscripts/data/enhance.py` & `lyscripts-1.0.0a1/lyscripts/data/enhance.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Enhance a LyProX-style CSV dataset in two ways:
 
-1. Add consensus diagnoses based on all available modalities using on of two methods:
-`max_llh` infers the most likely true state of involvement given only the available
-diagnoses. `rank` uses the available diagnositc modalities and ranks them based on
+1. Add consensus diagnosis based on all available modalities using on of two methods:
+``max_llh`` infers the most likely true state of involvement given only the available
+diagnosis. ``rank`` uses the available diagnositc modalities and ranks them based on
 their respective sensitivity and specificity.
 
 2. Complete sub- & super-level fields. This means that if a dataset reports LNLs IIa
 and IIb separately, this script will add the column for LNL II and fill it with the
 correct values. Conversely, if e.g. LNL II is reported to be healthy, we can assume
 the sublevels IIa and IIb would have been reported as healthy, too.
 """
@@ -21,45 +21,40 @@
 import numpy as np
 import pandas as pd
 
 from lyscripts.data.utils import save_table_to_csv
 from lyscripts.decorators import log_state
 from lyscripts.utils import (
     CustomProgress,
+    console,
     get_modalities_subset,
     load_patient_data,
     load_yaml_params,
-    report,
 )
 
 warnings.simplefilter(action="ignore", category=pd.errors.PerformanceWarning)
 logger = logging.getLogger(__name__)
 
 
 def _add_parser(
     subparsers: argparse._SubParsersAction,
     help_formatter,
 ):
-    """
-    Add an `ArgumentParser` to the subparsers action.
-    """
+    """Add a parser to the ``subparsers`` action."""
     parser = subparsers.add_parser(
         Path(__file__).name.replace(".py", ""),
         description=__doc__,
         help=__doc__,
         formatter_class=help_formatter,
     )
     _add_arguments(parser)
 
 
 def _add_arguments(parser: argparse.ArgumentParser):
-    """
-    Add arguments needed to run this script to a `subparsers` instance
-    and run the respective main function when chosen.
-    """
+    """Add arguments to the parser."""
     parser.add_argument(
         "input", type=Path,
         help="Path to a LyProX-style CSV file"
     )
     parser.add_argument(
         "output", type=Path,
         help="Destination for LyProX-style output file including the consensus"
@@ -92,34 +87,34 @@
 
 def get_sublvl_values(
     data_frame: pd.DataFrame,
     lnl: str,
     sub_ids: list[str],
 ):
     """
-    Get the values of sublevels (e.g. 'IIa' and 'IIb') for a given LNL and a
-    dataframe.
+    Get values of sublevels (e.g. 'IIa' and 'IIb') for an ``lnl`` and ``data_frame``.
     """
     has_sublvls = all(lnl+sub in data_frame for sub in sub_ids)
     if not has_sublvls:
         return None
     return data_frame[[lnl+sub for sub in sub_ids]].values
 
 
 @log_state()
 def infer_superlvl_from_sublvls(
     table: pd.DataFrame,
     modalities: list[str],
     lnls_with_sub: list[str],
     sublvls: list[str] | None = None,
 ) -> pd.DataFrame:
-    """
-    Infer the involvement state of all `lnls_with_sub`, i.e. LNLs where sub-levels were
-    reported, for each patient in the `table`. Do this for all defined `modalities` and
-    take into account all specified `sublvls`.
+    """Infer the involvement state of all ``lnls_with_sub``
+
+    I.e., infer the involvement of all LNLs where sub-levels were reported, for each
+    patient in the ``table``. Do this for all defined ``modalities`` and take into
+    account all specified ``sublvls``.
 
     This means that if e.g. sub-LNL IIa reports involvement and sub-LNL IIb shows no
     sign of metastasis, this method will infer that the superlevel II must be involved
     as well.
     """
     if sublvls is None:
         sublvls = ["a", "b"]
@@ -154,17 +149,17 @@
 
 def get_lnl_observations(
     patient: pd.Series,
     side: str,
     lnl: str,
     modalities: list[str],
 ) -> tuple[bool]:
-    """
-    Collect the observations for an `lnl` from every one of the available `modalities`
-    in a tuple. Do this for one `side` of the neck of a particular `patient`.
+    """Collect observations for ``lnl`` from every one of the ``modalities`` in a tuple.
+
+    This is done for one ``side`` of the neck of a particular ``patient``.
     """
     observations = ()
 
     for mod in modalities.keys():
         try:
             add_obs = patient[mod,side,lnl]
             add_obs = None if pd.isna(add_obs) else add_obs
@@ -173,63 +168,44 @@
         observations = (*observations, add_obs)
 
     return observations
 
 
 @lru_cache
 def has_all_none(obs_tuple: tuple[np.ndarray]):
-    """
-    Check if all entries in the observation tuple are ``None``.
-    """
+    """Check if all entries in the observation tuple are ``None``."""
     return all(obs is None for obs in obs_tuple)
 
+
 @lru_cache
 def or_consensus(obs_tuple: tuple[np.ndarray]):
-    """
-    Compute the consensus of different diagnostic modalities by computing the
-    logical OR.
-    """
+    """Compute the logical ``OR`` consensus of different diagnostic modalities."""
     if has_all_none(obs_tuple):
         return None
 
     return any(obs_tuple)
 
+
 @lru_cache
 def and_consensus(obs_tuple: tuple[np.ndarray]):
-    """
-    Compute the consensus of different diagnostic modalities by computing the
-    logical AND.
-    """
+    """Compute the logical ``AND`` consensus of different diagnostic modalities."""
     if has_all_none(obs_tuple):
         return None
 
     return not(
         any(not(obs) if obs is not None else None for obs in obs_tuple)
     )
 
+
 @lru_cache
 def maxllh_consensus(
     obs_tuple: tuple[np.ndarray],
     modalities_spsn: tuple[list[float]]
 ):
-    """
-    Compute the consensus of different diagnostic modalities using their
-    respective specificity & sensitivity.
-
-    Args:
-        obs_tuple: Tuple with the involvement (``True``, ``False`` or
-            ``None``).
-        modalities_spsn: Tuple with 2-element lists of the specificity &
-            sensitivity of the modalities corresponding to the diagnoses in the
-            parameter ``obs_tuple``.
-
-    Returns:
-        The most likely true state according to the consensus from the
-        diagnoses provided.
-    """
+    """Compute the maximum likelihood consensus of different diagnostic modalities."""
     if has_all_none(obs_tuple):
         return None
 
     healthy_llh = 1.
     involved_llh = 1.
     for obs, spsn in zip(obs_tuple, modalities_spsn):
         if obs is None:
@@ -239,33 +215,21 @@
         spsn2x2 = np.diag(spsn) + np.diag(1. - spsn)[::-1]
         healthy_llh *= spsn2x2[obs,0]
         involved_llh *= spsn2x2[obs,1]
 
     healthy_vs_involved = np.array([healthy_llh, involved_llh])
     return bool(np.argmax(healthy_vs_involved))
 
+
 @lru_cache
 def rank_consensus(
     obs_tuple: tuple[np.ndarray],
     modalities_spsn: tuple[list[float]]
 ):
-    """
-    Compute the consensus of different diagnostic modalities using a ranking
-    based on sensitivity & specificity.
-
-    Args:
-        obs_tuple: Tuple with the involvement (``True``, ``False`` or
-            ``None``).
-        modalities_spsn: Tuple with 2-element lists of the specificity &
-            sensitivity of the modalities corresponding to the diagnoses in the
-            parameter ``obs_tuple``.
-
-    Returns:
-        The most likely true state based on the ranking.
-    """
+    """Compute the ranked consensus of different diagnostic modalities."""
     if has_all_none(obs_tuple):
         return None
 
     modalities_spsn = list(modalities_spsn)
 
     healthy_sens = [
         modalities_spsn[i][1] for i,obs in enumerate(obs_tuple) if obs == False
@@ -284,60 +248,15 @@
     "rank": rank_consensus,
     "logic_or": lambda obs, *_args, **_kwargs: or_consensus(obs),
     "logic_and": lambda obs, *_args, **_kwargs: and_consensus(obs),
 }
 
 
 def main(args: argparse.Namespace):
-    """
-    Below is the help output (call with `lyscripts enhance --help`)
-
-    ```
-    USAGE: lyscripts data enhance [-h]
-                                  [-c {max_llh,rank,logic_or,logic_and} [{max_llh,rank,logic_or,logic_and} ...]]
-                                  [-p PARAMS]
-                                  [--modalities MODALITIES [MODALITIES ...]]
-                                  [--sublvls SUBLVLS [SUBLVLS ...]]
-                                  [--lnls-with-sub LNLS_WITH_SUB [LNLS_WITH_SUB ...]]
-                                  input output
-
-    Enhance a LyProX-style CSV dataset in two ways:
-
-    1. Add consensus diagnoses based on all available modalities using on of two
-    methods: `max_llh` infers the most likely true state of involvement given only the
-    available diagnoses. `rank` uses the available diagnositc modalities and ranks
-    them based on their respective sensitivity and specificity.
-
-    2. Complete sub- & super-level fields. This means that if a dataset reports LNLs
-    IIa and IIb separately, this script will add the column for LNL II and fill it
-    with the correct values. Conversely, if e.g. LNL II is reported to be healthy, we
-    can assume the sublevels IIa and IIb would have been reported as healthy, too.
-
-    POSITIONAL ARGUMENTS:
-      input                 Path to a LyProX-style CSV file
-      output                Destination for LyProX-style output file including the
-                            consensus
-
-    OPTIONAL ARGUMENTS:
-      -h, --help            show this help message and exit
-      -c, --consensus {max_llh,rank,logic_or,logic_and} [{max_llh,rank,logic_or,logic_and} ...]
-                            Choose consensus method(s) (default: ['max_llh'])
-      -p, --params PARAMS   Path to parameter file (default: params.yaml)
-      --modalities MODALITIES [MODALITIES ...]
-                            List of modalities for enhancement. Must be defined in
-                            `params.yaml` (default: ['CT', 'MRI', 'PET', 'FNA',
-                            'diagnostic_consensus', 'pathology', 'pCT'])
-      --sublvls SUBLVLS [SUBLVLS ...]
-                            Indicate what kinds of sublevels exist (default: ['a',
-                            'b'])
-      --lnls-with-sub LNLS_WITH_SUB [LNLS_WITH_SUB ...]
-                            List of LNLs where sublevel reporting has been performed
-                            or is common (default: ['I', 'II', 'V'])
-    ```
-    """
+    """Main function for the ``enhance`` command."""
     input_table = load_patient_data(args.input)
     params = load_yaml_params(args.params)
 
     modalities = get_modalities_subset(
         defined_modalities=params["modalities"],
         selection=args.modalities,
     )
@@ -354,28 +273,28 @@
     consensus = pd.DataFrame(
         index=input_table.index,
         columns=pd.MultiIndex.from_product(
             [args.consensus, ["ipsi", "contra"], lnl_union]
         )
     )
 
-    with CustomProgress(console=report) as report_progress:
+    with CustomProgress(console=console) as report_progress:
         enhance_task = report_progress.add_task(
             description=f"Compute {args.consensus} consensus of modalities...",
             total=2 * len(input_table),
         )
         for side in ["ipsi", "contra"]:
             # go through patients and LNLs and compute consensus for each
             for p,patient in input_table.iterrows():
                 for lnl in lnl_union:
                     observations = get_lnl_observations(
                         patient, side, lnl, available_mods
                     )
                     for cons in args.consensus:
-                        consensus[cons, side, lnl].iloc[p] = CONSENSUS_FUNCS[cons](
+                        consensus.loc[p, (cons, side, lnl)] = CONSENSUS_FUNCS[cons](
                             observations, available_mods.values()
                         )
                 report_progress.update(enhance_task, advance=1)
         table_with_consensus = input_table.join(consensus)
 
 
     data_modalities = sorted(set(
```

### Comparing `lyscripts-1.0.0a0/lyscripts/data/generate.py` & `lyscripts-1.0.0a1/lyscripts/data/generate.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,42 @@
 """
-Generate synthetic patient data for testing and validation purposes.
+Calls the synthetic data generating methods of the `lymph`_ package models.
+
+.. _lymph: https://lymph-model.readthedocs.io
 """
 # pylint: disable=logging-fstring-interpolation
 import argparse
 import logging
 from pathlib import Path
 
 import emcee
 import numpy as np
 
 from lyscripts.data.utils import save_table_to_csv
-from lyscripts.utils import create_model_from_config, load_yaml_params
+from lyscripts.utils import create_model, load_yaml_params
 
 logger = logging.getLogger(__name__)
 
 
 def _add_parser(
     subparsers: argparse._SubParsersAction,
     help_formatter,
 ):
-    """
-    Add an `ArgumentParser` to the subparsers action.
-    """
+    """Add an ``ArgumentParser`` to the subparsers action."""
     parser = subparsers.add_parser(
         Path(__file__).name.replace(".py", ""),
         description=__doc__,
         help=__doc__,
         formatter_class=help_formatter,
     )
     _add_arguments(parser)
 
 
 def _add_arguments(parser: argparse.ArgumentParser):
-    """
-    Add arguments needed to run this script to a `subparsers` instance
-    and run the respective main function when chosen.
-    """
+    """Add arguments to the parser."""
     parser.add_argument(
         "num", type=int,
         help="Number of synthetic patient records to generate",
     )
     parser.add_argument(
         "output", type=Path,
         help="Path where to store the generated synthetic data",
@@ -65,45 +62,17 @@
         help="Path to the samples if a method to load them was chosen"
     )
 
     parser.set_defaults(run_main=main)
 
 
 def main(args: argparse.Namespace):
-    """
-    The CLI's help for this subcommand (`lyscripts generate --help`) shows:
-
-    ```
-    USAGE: lyscripts data generate [-h] [--params PARAMS]
-                                   [--set-theta SET_THETA [SET_THETA ...] |
-                                   --load-theta {mean,max_llh}] [--samples SAMPLES]
-                                   num output
-
-    Generate synthetic patient data for testing and validation purposes.
-
-    POSITIONAL ARGUMENTS:
-      num                   Number of synthetic patient records to generate
-      output                Path where to store the generated synthetic data
-
-    OPTIONAL ARGUMENTS:
-      -h, --help            show this help message and exit
-      --params PARAMS       Parameter file containing model specifications (default:
-                            ./params.yaml)
-      --set-theta SET_THETA [SET_THETA ...]
-                            Set the spread probs and parameters for time
-                            marginalization by hand (default: None)
-      --load-theta {mean,max_llh}
-                            Use either the mean or the maximum likelihood estimate
-                            from drawn samples (default: mean)
-      --samples SAMPLES     Path to the samples if a method to load them was chosen
-                            (default: ./models/samples.hdf5)
-    ```
-    """
+    """Run the data generation."""
     params = load_yaml_params(args.params)
-    model = create_model_from_config(params)
+    model = create_model(params)
     ndim = len(model.spread_probs) + model.diag_time_dists.num_parametric
 
     if args.set_theta is not None:
         if len(args.set_theta) != ndim:
             raise ValueError(
                 f"Model takes {ndim} parameters, but{len(args.set_theta)} were provided"
             )
```

### Comparing `lyscripts-1.0.0a0/lyscripts/data/join.py` & `lyscripts-1.0.0a1/lyscripts/temp_schedule.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 """
-Join datasets from different sources (but of the same format) into one.
+Generate inverse temperature schedules for thermodynamic integration using various
+different methods.
+
+Thermodynamic integration is quite sensitive to the specific schedule which is used.
+I noticed in my models, that within the interval $[0, 0.1]$, the increase in the
+expected log-likelihood is very steep. Hence, the inverse temparature $\\beta$ must be
+more densely spaced in the beginning.
+
+This can be achieved by using a power sequence: Generate $n$ linearly spaced points in
+the interval $[0, 1]$ and then transform each point by computing $\\beta_i^k$ where
+$k$ could e.g. be 5.
 """
 # pylint: disable=logging-fstring-interpolation
 import argparse
 import logging
-import warnings
+from collections.abc import Callable
 from pathlib import Path
 
-import pandas as pd
-
-from lyscripts.data.utils import save_table_to_csv
-from lyscripts.utils import load_patient_data
-
-warnings.simplefilter(action="ignore", category=FutureWarning)
-
+import numpy as np
+import yaml
 
 logger = logging.getLogger(__name__)
 
 
 def _add_parser(
     subparsers: argparse._SubParsersAction,
     help_formatter,
@@ -36,60 +41,75 @@
 
 def _add_arguments(parser: argparse.ArgumentParser):
     """
     Add arguments needed to run this script to a `subparsers` instance
     and run the respective main function when chosen.
     """
     parser.add_argument(
-        "-i", "--inputs", nargs='+', type=Path, required=True,
-        help="List of paths to inference-ready CSV datasets to concatenate."
+        "--method", choices=SCHEDULES.keys(), default=list(SCHEDULES.keys())[0],
+        help="Choose the method to distribute the inverse temperature."
+    )
+    parser.add_argument(
+        "--num", default=32, type=int,
+        help="Number of inverse temperatures in the schedule"
     )
     parser.add_argument(
-        "-o", "--output", type=Path, required=True,
-        help="Location to store the concatenated CSV file."
+        "--pow", default=4, type=float,
+        help="If a power schedule is chosen, use this as power"
     )
 
     parser.set_defaults(run_main=main)
 
 
-def main(args: argparse.Namespace):
-    """
-    This program simply loops over the provided CSV files, reading in and appending
-    them to a concatenated `pd.DataFrame` one by one, hoping that they are all provided
-    in the same format.
-
-    In the end, the joined `pd.DataFrame` is stored at the desired location.
-
-    It's command help when running `lyscripts join --help` shows
-
-    ```
-    USAGE: lyscripts data join [-h] -i INPUTS [INPUTS ...] -o OUTPUT
-
-    Join datasets from different sources (but of the same format) into one.
-
-    OPTIONAL ARGUMENTS:
-      -h, --help            show this help message and exit
-      -i, --inputs INPUTS [INPUTS ...]
-                            List of paths to inference-ready CSV datasets to
-                            concatenate. (default: None)
-      -o, --output OUTPUT   Location to store the concatenated CSV file. (default:
-                            None)
-    ```
-    """
-    concatenated_table = pd.DataFrame()
-    for input_path in args.inputs:
-        input_table = load_patient_data(input_path)
-        concatenated_table = pd.concat(
-            [concatenated_table, input_table],
-            ignore_index=True
-        )
-        logger.info(f"+ concatenated data from {input_path}")
-    logger.info(f"Read & concatenated all {len(args.inputs)} CSV files")
+def tolist(func: Callable) -> Callable:
+    """Decorator to make sure the returned value is a list of floats."""
+    def inner(*args) -> np.ndarray | list[float]:
+        res = func(*args)
+        if isinstance(res, np.ndarray):
+            return res.tolist()
+        return res
+    return inner
+
+
+@tolist
+def geometric_schedule(n: int, *_a) -> np.ndarray:
+    """Create a geometric sequence of `n` numbers from 0. to 1."""
+    log_seq = np.logspace(0., 1., n)
+    shifted_seq = log_seq - 1.
+    geom_seq = shifted_seq / 9.
+    return geom_seq
+
+
+@tolist
+def linear_schedule(n: int, *_a) -> np.ndarray:
+    """Create a linear sequence of `n` numbers from 0. to 1."""
+    return np.linspace(0., 1., n)
+
+
+@tolist
+def power_schedule(n: int, power: float, *_a) -> np.ndarray:
+    """Create a power sequence of `n` numbers from 0. to 1."""
+    lin_seq = np.linspace(0., 1., n)
+    power_seq = lin_seq**power
+    return power_seq
+
+SCHEDULES = {
+    "geometric": geometric_schedule,
+    "linear": linear_schedule,
+    "power": power_schedule,
+}
 
-    save_table_to_csv(args.output, concatenated_table)
+
+def main(args: argparse.Namespace):
+    """Main function to generate a temperature schedule."""
+    func = SCHEDULES[args.method]
+    schedule = func(args.num, args.pow)
+    yaml_output = yaml.dump({"temp_schedule": schedule})
+    logger.info(f"Created {args.method} sequence of length {args.num}")
+    logger.debug(yaml_output)
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(description=__doc__)
     _add_arguments(parser)
 
     args = parser.parse_args()
```

### Comparing `lyscripts-1.0.0a0/lyscripts/data/lyproxify.py` & `lyscripts-1.0.0a1/lyscripts/data/lyproxify.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
-Consumes raw data and transforms it into a CSV of the format that [LyProX] understands.
+Consumes raw data and transforms it into a CSV of the format that `LyProX`_ understands.
 
 To do so, it needs a dictionary that defines a mapping from raw columns to the LyProX
-style data format. See the documentation of the `transform_to_lyprox` function for
-more information.
+style data format. See the documentation of the :py:func:`.transform_to_lyprox` function
+for more information.
 
-[LyProX]: https://lyprox.org
+.. _LyProX: https://lyprox.org
 """
 # pylint: disable=logging-fstring-interpolation
 import argparse
 import importlib.util
 import logging
 import warnings
 from pathlib import Path
@@ -27,31 +27,26 @@
 logger = logging.getLogger(__name__)
 
 
 def _add_parser(
     subparsers: argparse._SubParsersAction,
     help_formatter,
 ):
-    """
-    Add an `ArgumentParser` to the subparsers action.
-    """
+    """Add an ``ArgumentParser`` to the subparsers action."""
     parser = subparsers.add_parser(
         Path(__file__).name.replace(".py", ""),
         description=__doc__,
         help=__doc__,
         formatter_class=help_formatter,
     )
     _add_arguments(parser)
 
 
 def _add_arguments(parser: argparse.ArgumentParser):
-    """
-    Add arguments needed to run this script to a `subparsers` instance
-    and run the respective main function when chosen.
-    """
+    """Add arguments to the parser."""
     parser.add_argument(
         "-i", "--input", type=Path, required=True,
         help="Location of raw CSV data."
     )
     parser.add_argument(
         "-r", "--header-rows", nargs="+", default=[0], type=int,
         help="List with header row indices of raw file."
@@ -91,15 +86,15 @@
 
 
 def clean_header(
     table: pd.DataFrame,
     num_cols: int,
     num_header_rows: int,
 ) -> pd.DataFrame:
-    """Rename the header cells in the `table`."""
+    """Rename the header cells in the ``table``."""
     for col in range(num_cols):
         for row in range(num_header_rows):
             table.rename(
                 columns={f"Unnamed: {col}_level_{row}": f"{col}_lvl_{row}"},
                 inplace=True,
             )
     return table
@@ -108,14 +103,15 @@
 def get_instruction_depth(nested_column_map: dict[tuple, dict[str, Any]]) -> int:
     """
     Get the depth at which the column mapping instructions are nested.
 
     Instructions are a dictionary that contains either a 'func' or 'default' key.
 
     Example:
+
     >>> nested_column_map = {"patient": {"age": {"func": int}}}
     >>> get_instruction_depth(nested_column_map)
     2
     >>> flat_column_map = flatten(nested_column_map, max_depth=2)
     >>> get_instruction_depth(flat_column_map)
     1
     >>> nested_column_map = {"patient": {"__doc__": "some patient info", "age": 61}}
@@ -141,15 +137,15 @@
     depth: int = 0,
     indent_len: int = 4,
 ) -> str:
     """
     Generate a markdown nested, ordered list as documentation for the column map.
 
     A key in the doctionary is supposed to be documented, when its value is a dictionary
-    containing a `"__doc__"` key.
+    containing a ``"__doc__"`` key.
 
     Example:
     >>> nested_column_map = {
     ...     "patient": {
     ...         "__doc__": "some patient info",
     ...         "age": {
     ...             "__doc__": "age of the patient",
@@ -177,44 +173,46 @@
 
 @log_state()
 def transform_to_lyprox(
     raw: pd.DataFrame,
     column_map: dict[tuple, dict[str, Any]]
 ) -> pd.DataFrame:
     """
-    Transform `raw` data frame into table that can be uploaded directly to [LyProX].
+    Transform ``raw`` data frame into table that can be uploaded directly to `LyProX`_.
 
     To do so, it uses instructions in the `colum_map` dictionary, that needs to have
     a particular structure:
 
     For each column in the final 'lyproxified' `pd.DataFrame`, one entry must exist in
     the `column_map` dctionary. E.g., for the column corresponding to a patient's age,
     the dictionary should contain a key-value pair of this shape:
 
-    ```python
-    column_map = {
-        ("patient", "#", "age"): {
-            "func": compute_age_from_raw,
-            "kwargs": {"randomize": False},
-            "columns": ["birthday", "date of diagnosis"]
-        },
-    }
-    ```
-
-    In this example, the function `compute_age_from_raw` is called with the values of
-    the columns `birthday` and `date of diagnosis` as positional arguments, and the
-    keyword argument `randomize` is set to `False`. The function then returns the
-    patient's age, which is subsequently stored in the column `("patient", "#", "age")`.
-
-    Note that the `column_map` dictionary must have either a `default` key or `func`
-    along with `columns` and `kwargs`, depending on the function definition. If the
-    function does not take any arguments, `columns` can be omitted. If it also does
-    not take any keyword arguments, `kwargs` can be omitted, too.
+    .. code-block:: python
 
-    [LyProX]: https://lyprox.org
+        column_map = {
+            ("patient", "#", "age"): {
+                "func": compute_age_from_raw,
+                "kwargs": {"randomize": False},
+                "columns": ["birthday", "date of diagnosis"]
+            },
+        }
+
+    In this example, the function ``compute_age_from_raw`` is called with the
+    values of the columns ``"birthday"`` and ``"date of diagnosis"`` as positional
+    arguments, and the keyword argument ``"randomize"`` is set to ``False``. The
+    function then returns the patient's age, which is subsequently stored in the column
+    ``("patient", "#", "age")``.
+
+    Note that the ``column_map`` dictionary must have either a ``"default"`` key or
+    ``"func"`` along with ``"columns"`` and ``"kwargs"``, depending on the function
+    definition. If the function does not take any arguments, ``"columns"`` can be
+    omitted. If it also does not take any keyword arguments, ``"kwargs"`` can be
+    omitted, too.
+
+    .. _LyProX: https://lyprox.org
     """
     column_map = delete_private_keys(column_map)
 
     if (instruction_depth := get_instruction_depth(column_map)) > 1:
         column_map = flatten(column_map, max_depth=instruction_depth)
 
     multi_idx = pd.MultiIndex.from_tuples(column_map.keys())
@@ -247,15 +245,15 @@
 
 @log_state()
 def leftright_to_ipsicontra(data: pd.DataFrame):
     """
     Change absolute side reporting to tumor-relative.
 
     Transform reporting of LNL involvement by absolute side (right & left) to a
-    reporting relative to the tumor (ipsi- & contralateral). The table `data` should
+    reporting relative to the tumor (ipsi- & contralateral). The table ``data`` should
     already be in the format LyProX requires, except for the side-reporting of LNL
     involvement.
     """
     len_before = len(data)
     left_data = data.loc[
                 data["tumor", "1", "side"] != "right"
             ]
@@ -274,19 +272,20 @@
     assert len_before == len(data), "Number of patients changed"
     return data
 
 
 @log_state()
 def exclude_patients(raw: pd.DataFrame, exclude: list[tuple[str, Any]]):
     """
-    Exclude patients in the `raw` data based on a list of what to `exclude`. This
-    list contains tuples `(column, check)`. The `check` function will then exclude
-    any patients from the cohort where `check(raw[column])` evaluates to `True`.
+    Exclude patients in the ``raw`` data based on a list of what to ``exclude``. This
+    list contains tuples ``(column, check)``. The ``check`` function will then exclude
+    any patients from the cohort where ``check(raw[column])`` evaluates to ``True``.
 
     Example:
+
     >>> exclude = [("age", lambda s: s > 50)]
     >>> table = pd.DataFrame({
     ...     "age":        [43, 82, 18, 67],
     ...     "T-category": [ 3,  4,  2,  1],
     ... })
     >>> exclude_patients(table, exclude)
        age  T-category
@@ -296,52 +295,15 @@
     for column, check in exclude:
         exclude = check(raw[column])
         raw = raw.loc[~exclude]
     return raw
 
 
 def main(args: argparse.Namespace):
-    """
-    The main entry point for the CLI of this command. Upon requesting `lyscripts
-    data lyproxify --help`, this is the help output:
-
-    ```
-    USAGE: lyscripts data lyproxify [-h] -i INPUT [-r HEADER_ROWS [HEADER_ROWS ...]]
-                                    -o OUTPUT -m MAPPING
-                                    [--drop-rows DROP_ROWS [DROP_ROWS ...]]
-                                    [--drop-cols DROP_COLS [DROP_COLS ...]]
-                                    [--add-index]
-
-    Consumes raw data and transforms it into a CSV of the format that LyProX can
-    understand.
-
-    To do so, it needs a dictionary that defines a mapping from raw columns to the
-    LyProX style data format. See the documentation of the `transform_to_lyprox`
-    function for more information.
-
-    OPTIONAL ARGUMENTS:
-      -h, --help            show this help message and exit
-      -i, --input INPUT     Location of raw CSV data. (default: None)
-      -r, --header-rows HEADER_ROWS [HEADER_ROWS ...]
-                            List with header row indices of raw file. (default: [0])
-      -o, --output OUTPUT   Location to store the lyproxified CSV file. (default:
-                            None)
-      -m, --mapping MAPPING
-                            Location of the Python file that contains column mapping
-                            instructions. This must contain a dictionary with the name
-                            'column_map'. (default: None)
-      --drop-rows DROP_ROWS [DROP_ROWS ...]
-                            Delete rows of specified indices. Counting of rows start
-                            at 0 _after_ the `header-rows`. (default: [])
-      --drop-cols DROP_COLS [DROP_COLS ...]
-                            Delete columns of specified indices. (default: [])
-      --add-index           If the data doesn't contain an index, add one by
-                            enumerating the patients (default: False)
-    ```
-    """
+    """Run the lyproxify main function."""
     raw: pd.DataFrame = load_patient_data(args.input)
     raw = clean_header(raw, num_cols=raw.shape[1], num_header_rows=len(args.header_rows))
 
     cols_to_drop = raw.columns[args.drop_cols]
     trimmed = raw.drop(cols_to_drop, axis="columns")
     trimmed = trimmed.drop(index=args.drop_rows)
     trimmed = trimmed.dropna(axis="index", how="all")
```

### Comparing `lyscripts-1.0.0a0/lyscripts/data/split.py` & `lyscripts-1.0.0a1/lyscripts/data/split.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,31 +17,26 @@
 logger = logging.getLogger(__name__)
 
 
 def _add_parser(
     subparsers: argparse._SubParsersAction,
     help_formatter,
 ):
-    """
-    Add an `ArgumentParser` to the subparsers action.
-    """
+    """Add an ``ArgumentParser`` to the subparsers action."""
     parser = subparsers.add_parser(
         Path(__file__).name.replace(".py", ""),
         description=__doc__,
         help=__doc__,
         formatter_class=help_formatter,
     )
     _add_arguments(parser)
 
 
 def _add_arguments(parser: argparse.ArgumentParser):
-    """
-    Add arguments needed to run this script to a `subparsers` instance
-    and run the respective main function when chosen.
-    """
+    """Add arguments to the parser."""
     parser.add_argument(
         "input", type=Path,
         help="The path to the full dataset to split."
     )
     parser.add_argument(
         "output", type=Path,
         help="Folder to store the split CSV files in."
@@ -52,32 +47,15 @@
         help="Path to parameter YAML file."
     )
 
     parser.set_defaults(run_main=main)
 
 
 def main(args: argparse.Namespace):
-    """
-    The output from `lyscripts split --help` looks like this:
-
-    ```
-    USAGE: lyscripts data split [-h] [-p PARAMS] input output
-
-    Split the full dataset into cross-validation folds according to the content of the
-    params.yaml file.
-
-    POSITIONAL ARGUMENTS:
-      input                 The path to the full dataset to split.
-      output                Folder to store the split CSV files in.
-
-    OPTIONAL ARGUMENTS:
-      -h, --help            show this help message and exit
-      -p, --params PARAMS   Path to parameter YAML file. (default: ./params.yaml)
-    ```
-    """
+    """Run the splitting main routine."""
     params = load_yaml_params(args.params)
     concatenated_df = pd.read_csv(args.input)
     logger.info(f"Read in concatenated CSV file from {args.input}")
 
     args.output.mkdir(exist_ok=True)
     shuffled_df = concatenated_df.sample(
         frac=1.,
```

### Comparing `lyscripts-1.0.0a0/lyscripts/decorators.py` & `lyscripts-1.0.0a1/lyscripts/decorators.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """
 This module provides decorators that can be used to avoid repetitive snippets of code,
 e.g. safely opening files or logging the state of a function call.
+
+This is *not* a command line tool.
 """
 import functools
 import logging
 from collections.abc import Callable
 from functools import wraps
 from pathlib import Path
-from typing import Any, BinaryIO, TextIO
+from typing import Any
 
 
 def extract_logger(*args, **kwargs) -> logging.Logger:
     """Extract a logger from the arguments if present.
 
     The function will first search if the function is in fact a method of a class that
     has any attributes that are instances of `logging.Logger`. If not, it will search
@@ -73,17 +75,24 @@
             """The wrapper around the decorated function."""
             logger = logging.getLogger(func.__module__)
             signature = assemble_signature(*args, **kwargs)
             logger.debug(f"Executing {func.__name__}({signature}).")
             log_msg_from_func = func.__name__.replace("_", " ").capitalize() + "."
 
             try:
-                result = func(*args, **kwargs)
-                logger.log(log_level, log_msg_from_func)
-                return result
+                logger.log(
+                    log_level,
+                    log_msg_from_func,
+                    extra={
+                        "func_filepath": f"{func.__module__.replace('.', '/')}.py",
+                        "func_name": func.__name__,
+                        "module_name": func.__module__,
+                    },
+                )
+                return func(*args, **kwargs)
 
             except Exception as exc:
                 logger.error(f"Error calling {func.__name__}().", exc_info=exc)
                 raise exc
 
         return wrapper
 
@@ -100,45 +109,14 @@
             raise FileNotFoundError(f"File {file_path} does not exist.")
 
         return loading_func(file_path, *args, **kwargs)
 
     return inner
 
 
-def provide_file(is_binary: bool) -> Callable:
-    """Make sure a decorated function is provided with a file-like object.
-
-    This means, the assembled decorator checks the argument type and, if necessary,
-    opens the file to call the decorated function. The provided file is either a text
-    file of - if `is_binary` is set to `True` - a binary file.
-    """
-    def assembled_decorator(loading_func: Callable) -> Callable:
-        """Assembled decorator that provides the function with a text/binary file."""
-        @wraps(loading_func)
-        def inner(file_or_path: str | Path | TextIO | BinaryIO, *args, **kwargs):
-            """The wrapped function."""
-            if isinstance(file_or_path, (str, Path)):
-                file_path = Path(file_or_path)
-                if not file_path.is_file():
-                    raise FileNotFoundError(f"File {file_path} does not exist.")
-
-                if is_binary:
-                    with open(file_path, mode="rb") as bin_file:
-                        return loading_func(bin_file, *args, **kwargs)
-                else:
-                    with open(file_path, encoding="utf-8") as txt_file:
-                        return loading_func(txt_file, *args, **kwargs)
-
-            return loading_func(file_or_path, *args, **kwargs)
-
-        return inner
-
-    return assembled_decorator
-
-
 def check_output_dir_exists(saving_func: Callable) -> Callable:
     """Make sure the parent directory of the saved file exists."""
     @wraps(saving_func)
     def inner(file_path: str, *args, **kwargs) -> Any:
         """Wrapped saving function."""
         file_path = Path(file_path)
         file_path.parent.mkdir(parents=True, exist_ok=True)
```

### Comparing `lyscripts-1.0.0a0/lyscripts/evaluate.py` & `lyscripts-1.0.0a1/lyscripts/evaluate.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,43 +11,37 @@
 
 import emcee
 import h5py
 import numpy as np
 import pandas as pd
 from scipy.integrate import trapezoid
 
-from lyscripts.utils import (
-    create_model_from_config,
-    load_patient_data,
-    load_yaml_params,
-)
+from lyscripts.utils import create_model, load_patient_data, load_yaml_params
 
 logger = logging.getLogger(__name__)
 
 
 def _add_parser(
     subparsers: argparse._SubParsersAction,
     help_formatter,
 ):
-    """
-    Add an `ArgumentParser` to the subparsers action.
-    """
+    """Add an ``ArgumentParser`` to the subparsers action."""
     parser = subparsers.add_parser(
         Path(__file__).name.replace(".py", ""),
         description=__doc__,
         help=__doc__,
         formatter_class=help_formatter,
     )
     _add_arguments(parser)
 
 
 def _add_arguments(parser: argparse.ArgumentParser):
-    """
-    Add arguments needed to run this script to a `subparsers` instance
-    and run the respective main function when chosen.
+    """Add arguments to a ``subparsers`` instance and run its main function when chosen.
+
+    This is called by the parent module that is called via the command line.
     """
     parser.add_argument(
         "data", type=Path,
         help="Path to the tables of patient data (CSV)."
     )
     parser.add_argument(
         "model", type=Path,
@@ -76,16 +70,16 @@
     num_data: int
 ) -> float:
     """
     Compute the negative one half of the Bayesian Information Criterion (BIC).
 
     The BIC is defined as [^1]
     $$ BIC = k \\ln{n} - 2 \\ln{\\hat{L}} $$
-    where $k$ is the number of parameters `num_params`, $n$ the number of datapoints
-    `num_data` and $\\hat{L}$ the maximum likelihood estimate of the `log_prob`.
+    where $k$ is the number of parameters ``num_params``, $n$ the number of datapoints
+    ``num_data`` and $\\hat{L}$ the maximum likelihood estimate of the ``log_prob``.
     It is constructed such that the following is an
     approximation of the model evidence:
     $$ p(D \\mid m) \\approx \\exp{\\left( - BIC / 2 \\right)} $$
     which is why this function returns the negative one half of it.
 
     [^1]: https://en.wikipedia.org/wiki/Bayesian_information_criterion
     """
@@ -94,20 +88,20 @@
 def compute_evidence(
     temp_schedule: np.ndarray,
     log_probs: np.ndarray,
     num: int = 1000,
 ) -> tuple[float, float]:
     """Compute the evidene and its standard deviation.
 
-    Given a `temp_schedule` of inverse temperatures and corresponding sets of
-    `log_probs`, draw `num` "paths" of log-probabilities and compute the evidence for
-    each using trapezoidal integration.
+    Given a ``temp_schedule`` of inverse temperatures and corresponding sets of
+    ``log_probs``, draw ``num`` "paths" of log-probabilities and compute the evidence
+    for each using trapezoidal integration.
 
-    The evidence is then the mean of those `num` integrations, while the error is their
-    standard deviation.
+    The evidence is then the mean of those ``num`` integrations, while the error is
+    their standard deviation.
     """
     integrals = np.zeros(shape=num)
     for i in range(num):
         rand_idx = np.random.choice(log_probs.shape[1], size=log_probs.shape[0])
         drawn_accuracy = log_probs[np.arange(log_probs.shape[0]),rand_idx].copy()
         integrals[i] = trapezoid(y=drawn_accuracy, x=temp_schedule)
     return np.mean(integrals), np.std(integrals)
@@ -142,57 +136,19 @@
     metrics["evidence"] = evidence
     metrics["evidence_std"] = evidence_std
 
     return temp_schedule, ti_log_probs
 
 
 def main(args: argparse.Namespace):
-    """
-    To evaluate the performance of a sampling round, this program follows these steps:
-
-    1. Read in the paramter file `params.yaml` and the data that was used for inference
-    2. Recreate an instance of the model that was used during the training stage
-    3. If thermodynamic integration (TI) [^2] was performed, compute the accuracy for
-    every TI step and integrate over it to obtain the evidence. This is computed for
-    a number of samples of the computed accuracies to also obtain an error on the
-    evidence.
-    4. Use the recreated model and data to compute quantities like the mean and maximum
-    likelihood, as well as the Bayesian information criterion (BIC).
-
-    Everything computed is then stored in a `metrics.json` file and for TI, a CSV is
-    created that shows how the accuracy developed during the runs.
-
-    The output of running `lyscripts evaluate --help` shows this:
-
-    ```
-    usage: lyscripts evaluate [-h] [-p PARAMS] [--plots PLOTS] [--metrics METRICS]
-                            data model
-
-    Evaluate the performance of the trained model by computing quantities like the
-    Bayesian information criterion (BIC) or (if thermodynamic integration was performed)
-    the actual evidence (with error) of the model.
-
-
-    POSITIONAL ARGUMENTS
-    data                 Path to the tables of patient data (CSV).
-    model                Path to model output files (HDF5).
-
-    OPTIONAL ARGUMENTS
-    -h, --help           show this help message and exit
-    -p, --params PARAMS  Path to parameter file (default: ./params.yaml)
-    --plots PLOTS        Directory for storing plots (default: ./plots)
-    --metrics METRICS    Path to metrics file (default: ./metrics.json)
-    ```
-
-    [^2]: https://doi.org/10.1007/s11571-021-09696-9
-    """
+    """Main entry point of the script."""
     metrics = {}
 
     params = load_yaml_params(args.params)
-    model = create_model_from_config(params)
+    model = create_model(params)
     ndim = len(model.get_params())
     data = load_patient_data(args.data)
     h5_file = h5py.File(args.model, mode="r")
 
     # if TI has been performed, compute the accuracy for every step
     if "ti" in h5_file:
         temp_schedule, ti_log_probs = compute_ti_results(
```

### Comparing `lyscripts-1.0.0a0/lyscripts/plot/__init__.py` & `lyscripts-1.0.0a1/lyscripts/compute/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,27 @@
 """
-Provide various plotting utilities for displaying results of e.g. the inference
-or prediction process. At the moment, three subcommands are grouped under
-`lyscripts.plot`:
-
-1. `lyscripts.plot.corner`, which simply outputs a corner plot with nice labels for
-a set of drawn samples.
-2. The module `lyscripts.plot.histograms` can be used to draw histograms, e.g. the ones
-over risks and prevalences as computed by the `lyscripts.predict` module.
-3. Module `lyscripts.plot.thermo_int` allows comparing rounds of thermodynamic
-integration for different models.
+With the commands of this module, a user may compute prior and posterior state
+distributions from drawn samples of a model. This can in turn speed up the computation
+of risks and prevalences.
 """
 import argparse
 from pathlib import Path
 
-from . import corner, histograms, thermo_int
+from lyscripts.compute import posteriors, prevalences, priors, risks
 
 
 def _add_parser(
     subparsers: argparse._SubParsersAction,
     help_formatter,
 ):
-    """
-    Add an `ArgumentParser` to the subparsers action and then add more subparsers.
-    """
+    """Add an ``ArgumentParser`` to the subparsers and then add more subparsers."""
     parser = subparsers.add_parser(
         Path(__file__).parent.name,
         description=__doc__,
         help=__doc__,
         formatter_class=help_formatter,
     )
     subparsers = parser.add_subparsers()
-    corner._add_parser(subparsers, help_formatter=parser.formatter_class)
-    histograms._add_parser(subparsers, help_formatter=parser.formatter_class)
-    thermo_int._add_parser(subparsers, help_formatter=parser.formatter_class)
+    priors._add_parser(subparsers, help_formatter=parser.formatter_class)
+    posteriors._add_parser(subparsers, help_formatter=parser.formatter_class)
+    prevalences._add_parser(subparsers, help_formatter=parser.formatter_class)
+    risks._add_parser(subparsers, help_formatter=parser.formatter_class)
```

### Comparing `lyscripts-1.0.0a0/lyscripts/plot/__main__.py` & `lyscripts-1.0.0a1/lyscripts/plot/__main__.py`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a0/lyscripts/plot/corner.py` & `lyscripts-1.0.0a1/lyscripts/plot/corner.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,46 @@
 """
 Generate a corner plot of the drawn samples.
 
 A corner plot is a combination of 1D and 2D marginals of probability distributions.
 The library I use for this is built on `matplotlib` and is called
-[`corner`](https://github.com/dfm/corner.py).
+`corner`_.
+
+.. _corner: https://github.com/dfm/corner.py
 """
 # pylint: disable=logging-fstring-interpolation
 import argparse
 import logging
 from pathlib import Path
 
 import corner
 import emcee
 
 from lyscripts.plot.utils import save_figure
-from lyscripts.utils import load_yaml_params, model_from_config
+from lyscripts.utils import create_model, load_yaml_params
 
 logger = logging.getLogger(__name__)
 
 
 def _add_parser(
     subparsers: argparse._SubParsersAction,
     help_formatter,
 ):
-    """
-    Add an `ArgumentParser` to the subparsers action.
-    """
+    """Add an ``ArgumentParser`` to the subparsers action."""
     parser = subparsers.add_parser(
         Path(__file__).name.replace(".py", ""),
         description=__doc__,
         help=__doc__,
         formatter_class=help_formatter,
     )
     _add_arguments(parser)
 
 
 def _add_arguments(parser: argparse.ArgumentParser):
-    """
-    Add arguments needed to run this script to a `subparsers` instance
-    and run the respective main function when chosen.
-    """
+    """Add arguments to the parser."""
     parser.add_argument(
         "model", type=Path,
         help="Path to model output files (HDF5)."
     )
     parser.add_argument(
         "output", type=Path,
         help="Path to output corner plot (SVG)."
@@ -53,45 +50,21 @@
         help="Path to parameter file"
     )
 
     parser.set_defaults(run_main=main)
 
 
 def main(args: argparse.Namespace):
-    """
-    This (sub)subrogram shows the following help message when asking for it
-    via `lyscripts plot corner --help`
-
-    ```
-    USAGE: lyscripts plot corner [-h] [-p PARAMS] model output
-
-    Generate a corner plot of the drawn samples.
-
-    A corner plot is a combination of 1D and 2D marginals of probability
-    distributions. The library I use for this is built on `matplotlib` and is called
-    [`corner`](https://github.com/dfm/corner.py).
-
-    POSITIONAL ARGUMENTS:
-        model                 Path to model output files (HDF5).
-        output                Path to output corner plot (SVG).
-
-    OPTIONAL ARGUMENTS:
-        -h, --help            show this help message and exit
-        -p, --params PARAMS   Path to parameter file (default: ./params.yaml)
-    ```
-    """
+    """Execute the corner plotting function."""
     params = load_yaml_params(args.params)
 
     backend = emcee.backends.HDFBackend(args.model, read_only=True)
     logger.info(f"Opened model as emcee backend from {args.model}")
 
-    model = model_from_config(
-        graph_params=params["graph"],
-        model_params=params["model"],
-    )
+    model = create_model(params)
     labels = list(model.get_params(as_dict=True).keys())
 
     chain = backend.get_chain(flat=True)
     if len(labels) != chain.shape[1]:
         raise RuntimeError(f"length labels: {len(labels)}, shape chain: {chain.shape}")
     fig = corner.corner(
         chain,
```

### Comparing `lyscripts-1.0.0a0/lyscripts/plot/utils.py` & `lyscripts-1.0.0a1/lyscripts/plot/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,46 +27,46 @@
     "red": '#ae0060',
     "gray": '#c5d5db',
 }
 COLOR_CYCLE = cycle(COLORS.values())
 CM_PER_INCH = 2.54
 
 
-def _floor_at_decimal(value: float, decimal: int) -> float:
-    """
-    Compute the floor of `value` for the specified `decimal`, which is the distance
-    to the right of the decimal point. May be negative.
+def floor_at_decimal(value: float, decimal: int) -> float:
+    """Compute the floor of ``value`` for the specified ``decimal``.
+
+    Essentially, this is the distance to the right of the decimal point. May be negative.
     """
     power = 10**decimal
     return np.floor(power * value) / power
 
-def _ceil_at_decimal(value: float, decimal: int) -> float:
-    """
-    Compute the ceiling of `value` for the specified `decimal`, which is the distance
-    to the right of the decimal point. May be negative.
-    """
-    return - _floor_at_decimal(-value, decimal)
 
-def _floor_to_step(value: float, step: float) -> float:
-    """
-    Compute the next closest value on a ladder of stepsize `step` that is below `value`.
+def ceil_at_decimal(value: float, decimal: int) -> float:
+    """Compute the ceiling of ``value`` for the specified ``decimal``
+
+    Analog to :py:func:`._floot_at_decimal`, this is the distance to the right of the
+    decimal point. May be negative.
     """
+    return - floor_at_decimal(-value, decimal)
+
+
+def floor_to_step(value: float, step: float) -> float:
+    """Compute next closest value on ladder of stepsize ``step`` that is below ``value``."""
     return (value // step) * step
 
-def _ceil_to_step(value: float, step: float) -> float:
-    """
-    Compute the next closest value on a ladder of stepsize `step` that is above `value`.
-    """
-    return _floor_to_step(value, step) + step
 
+def ceil_to_step(value: float, step: float) -> float:
+    """Compute next closest value on ladder of stepsize ``step`` that is above ``value``."""
+    return floor_to_step(value, step) + step
 
-def _clean_and_check(filename: str | Path) -> Path:
-    """
-    Check if file with `filename` exists. If not, raise error, otherwise return
-    cleaned `PosixPath`.
+
+def clean_and_check(filename: str | Path) -> Path:
+    """Check if file with ``filename`` exists.
+
+    If not, raise error, otherwise return cleaned ``PosixPath``.
     """
     filepath = Path(filename)
     if not filepath.exists():
         raise FileNotFoundError(
             f"File with the name {filename} does not exist at {filepath.resolve()}"
         )
     return filepath
@@ -81,41 +81,42 @@
 
     def __post_init__(self) -> None:
         self.values = self.scale * self.values
 
     @classmethod
     def from_hdf5(cls, filename, dataname, scale: float = 100., **kwargs):
         """Create a histogram from an HDF5 file."""
-        filename = _clean_and_check(filename)
+        filename = clean_and_check(filename)
         with h5py.File(filename, mode="r") as h5file:
             dataset = h5file[dataname]
             if "label" not in kwargs:
                 kwargs["label"] = get_label(dataset.attrs)
             return cls(values=dataset[:], scale=scale, kwargs=kwargs)
 
     def left_percentile(self, percent: float) -> float:
         """Compute the point where `percent` of the values are to the left."""
         return np.percentile(self.values, percent)
 
     def right_percentile(self, percent: float) -> float:
         """Compute the point where `percent` of the values are to the right."""
         return np.percentile(self.values, 100. - percent)
 
+
 @dataclass
-class Posterior:
+class BetaPosterior:
     """Class for storing plot configs for a Beta posterior."""
     num_success: int
     num_total: int
     scale: float = field(default=100.)
     kwargs: dict[str, Any] = field(default_factory=lambda: {})
 
     @classmethod
     def from_hdf5(cls, filename, dataname, scale: float = 100., **kwargs) -> None:
         """Initialize data container for Beta posteriors from HDF5 file."""
-        filename = _clean_and_check(filename)
+        filename = clean_and_check(filename)
         with h5py.File(filename, mode="r") as h5file:
             dataset = h5file[dataname]
             try:
                 num_success = int(dataset.attrs["num_match"])
                 num_total = int(dataset.attrs["num_total"])
             except KeyError as key_err:
                 raise KeyError(
@@ -134,39 +135,42 @@
             x,
             a=self.num_success+1,
             b=self.num_fail+1,
             scale=self.scale
         )
 
     def left_percentile(self, percent: float) -> float:
-        """Return the point where the CDF reaches `percent`."""
+        """Return the point where the CDF reaches ``percent``."""
         return sp.stats.beta.ppf(
             percent / 100.,
             a=self.num_success+1,
             b=self.num_fail+1,
             scale=self.scale,
         )
 
     def right_percentile(self, percent: float) -> float:
-        """Return the point where 100% minus the CDF equals `percent`."""
+        """Return the point where 100% minus the CDF equals ``percent``."""
         return sp.stats.beta.ppf(
             1. - (percent / 100.),
             a=self.num_success+1,
             b=self.num_fail+1,
             scale=self.scale,
         )
 
 
 def get_size(width="single", unit="cm", ratio="golden"):
     """
-    Return a tuple of figure sizes in inches, as the `matplotlib` keyword argument
-    `figsize` expects it. This figure size is computed from a `width`, in the `unit` of
-    centimeters by default, and a `ratio` which is set to the golden ratio by default.
+    Return a tuple of figure sizes in inches.
+
+    This is provided as the ``matplotlib`` keyword argument ``figsize`` expects it.
+    This figure size is computed from a ``width``, in the ``unit`` of centimeters by
+    default, and a ``ratio`` which is set to the golden ratio by default.
 
     Examples:
+
     >>> get_size(width="single", ratio="golden")
     (3.937007874015748, 2.4332557935820445)
     >>> get_size(width="full", ratio=2.)
     (6.299212598425196, 3.149606299212598)
     >>> get_size(width=10., ratio=1.)
     (3.937007874015748, 3.937007874015748)
     >>> get_size(width=5, unit="inches", ratio=2./3.)
@@ -180,34 +184,34 @@
     ratio = 1.618 if ratio == "golden" else ratio
     width = width / CM_PER_INCH if unit == "cm" else width
     height = width / ratio
     return (width, height)
 
 
 def get_label(attrs) -> str:
-    """Extract label of a histogram from the HDF5 `attrs` object of the dataset."""
+    """Extract label of a histogram from the HDF5 ``attrs`` object of the dataset."""
     label = []
     transforms = {
         "label": str,
         "modality": str,
         "t_stage": str,
         "midline_ext": lambda x: "ext" if x else "noext"
     }
     for key,func in transforms.items():
         if key in attrs and attrs[key] is not None:
             label.append(func(attrs[key]))
     return " | ".join(label)
 
 
 def get_xlims(
-    contents: list[Histogram | Posterior],
+    contents: list[Histogram | BetaPosterior],
     percent_lims: tuple[float] = (10., 10.),
 ) -> tuple[float]:
     """
-    Compute the `xlims` of a plot containing histograms and probability density
+    Compute the ``xlims`` of a plot containing histograms and probability density
     functions by considering their smallest and largest percentiles.
     """
     left_percentiles = np.array(
         [c.left_percentile(percent_lims[0]) for c in contents]
     )
     left_lim = np.min(left_percentiles)
     right_percentiles = np.array(
@@ -215,35 +219,35 @@
     )
     right_lim = np.max(right_percentiles)
     return left_lim, right_lim
 
 
 def draw(
     axes: MPLAxes,
-    contents: list[Histogram | Posterior],
+    contents: list[Histogram | BetaPosterior],
     percent_lims: tuple[float] = (10., 10.),
     xlims: tuple[float] | None = None,
     hist_kwargs: dict[str, Any] | None = None,
     plot_kwargs: dict[str, Any] | None = None,
 ) -> MPLAxes:
     """
-    Draw histograms and Beta posterior from `contents` into `axes`.
+    Draw histograms and Beta posterior from ``contents`` into ``axes``.
 
     The limits of the x-axis is computed to be the smallest and largest left and right
-    percentile of all provided `contents` respectively via the `percent_lims` tuple.
+    percentile of all provided ``contents`` respectively via the ``percent_lims`` tuple.
 
-    The `hist_kwargs` define general settings that will be applied to all histograms.
-    One additional key `'nbins'` may be used to adjust only the numbers, not the spacing
-    of the histogram bins.
-    Similarly, `plot_kwargs` adjusts the default settings for the Beta posteriors.
+    The ``hist_kwargs`` define general settings that will be applied to all histograms.
+    One additional key ``'nbins'`` may be used to adjust only the numbers, not the
+    spacing of the histogram bins.
+    Similarly, ``plot_kwargs`` adjusts the default settings for the Beta posteriors.
 
-    Both these keyword arguments can be overwritten by what the individual `contents`
+    Both these keyword arguments can be overwritten by what the individual ``contents``
     have defined.
     """
-    if not all(isinstance(c, (Histogram, Posterior)) for c in contents):
+    if not all(isinstance(c, (Histogram, BetaPosterior)) for c in contents):
         raise TypeError("Contents must be `Histogram` or `Posterior` instances")
 
     if xlims is None:
         xlims = get_xlims(contents, percent_lims)
     elif len(xlims) != 2 or xlims[0] > xlims[-1]:
         raise ValueError("`xlims` must be tuple of two increasing values")
 
@@ -264,34 +268,34 @@
     default_plot_kwargs.update(plot_kwargs)
 
     for content in contents:
         if isinstance(content, Histogram):
             tmp_hist_kwargs = default_hist_kwargs.copy()
             tmp_hist_kwargs.update(content.kwargs)
             axes.hist(content.values, **tmp_hist_kwargs)
-        elif isinstance(content, Posterior):
+        elif isinstance(content, BetaPosterior):
             tmp_plot_kwargs = default_plot_kwargs.copy()
             tmp_plot_kwargs["label"] = f"{content.num_success} / {content.num_total}"
             tmp_plot_kwargs.update(content.kwargs)
             axes.plot(x, content.pdf(x), **tmp_plot_kwargs)
 
     axes.set_xlim(*xlims)
     return axes
 
 
 @log_state()
 @check_input_file_exists
 def use_mpl_stylesheet(file_path: str | Path):
-    """Load a `.mplstyle` stylesheet from `file_path`."""
+    """Load a ``.mplstyle`` stylesheet from ``file_path``."""
     plt.style.use(file_path)
 
 
 @log_state()
 @check_output_dir_exists
 def save_figure(
     output_path: str | Path,
     figure: Figure,
     formats: list[str] | None,
 ):
-    """Save a `figure` to `output_path` in every one of the provided `formats`."""
+    """Save a ``figure`` to ``output_path`` in every one of the provided ``formats``."""
     for frmt in formats:
         figure.savefig(output_path.with_suffix(f".{frmt}"))
```

### Comparing `lyscripts-1.0.0a0/lyscripts/sample.py` & `lyscripts-1.0.0a1/lyscripts/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,511 +1,484 @@
 """
-Learn the spread probabilities of the HMM for lymphatic tumor progression using
-the preprocessed data as input and MCMC as sampling method.
+This module contains frequently used functions and decorators that are used throughout
+the subcommands to load e.g. YAML specifications or model definitions.
 
-This is the central script performing for our project on modelling lymphatic spread
-in head & neck cancer. We use it for model comparison via the thermodynamic
-integration functionality and use the sampled parameter estimates for risk
-predictions. This risk estimate may in turn some day guide clinicians to make more
-objective decisions with respect to defining the *elective clinical target volume*
-(CTV-N) in radiotherapy.
+It also contains helpers for reporting the script's progress via a slightly customized
+`rich` console and a custom `Exception` called `LyScriptsWarning` that can propagate
+occuring issues to the right place.
 """
-# pylint: disable=logging-fstring-interpolation
-import argparse
-import logging
-import os
 import warnings
-from collections.abc import Callable
-from multiprocessing import Pool
+from logging import LogRecord
 from pathlib import Path
-from typing import Any
+from typing import Any, Literal
 
-import emcee
-import h5py
 import numpy as np
 import pandas as pd
-
-from lyscripts.utils import (
-    CustomProgress,
-    get_modalities_subset,
-    load_yaml_params,
-    model_from_config,
-    report,
+import yaml
+from deprecated import deprecated
+from emcee.backends import HDFBackend
+from lymph import diagnosis_times, models, types
+from rich.console import Console
+from rich.logging import RichHandler
+from rich.progress import Progress, SpinnerColumn, TimeElapsedColumn
+from scipy.special import factorial
+
+from lyscripts.decorators import (
+    check_input_file_exists,
+    check_output_dir_exists,
+    log_state,
 )
 
-logger = logging.getLogger(__name__)
+try:
+    import streamlit
+    from streamlit.runtime.scriptrunner import get_script_run_ctx
+    streamlit.status = streamlit.spinner
+except ImportError:
+    def get_script_run_ctx() -> bool:
+        """A mock for the `get_script_run_ctx` function of `streamlit`."""
+        return None
 
 
-def _add_parser(
-    subparsers: argparse._SubParsersAction,
-    help_formatter,
-):
-    """
-    Add an `ArgumentParser` to the subparsers action.
-    """
-    parser = subparsers.add_parser(
-        Path(__file__).name.replace(".py", ""),
-        description=__doc__,
-        help=__doc__,
-        formatter_class=help_formatter,
-    )
-    _add_arguments(parser)
+CROSS = "[bold red]✗[/bold red]"
+CIRCL = "[bold blue]∘[/bold blue]"
+WARN = "[bold yellow]Δ[/bold yellow]"
+CHECK = "[bold green]✓[/bold green]"
 
 
-def _add_arguments(parser: argparse.ArgumentParser):
-    """
-    Add arguments needed to run this script to a `subparsers` instance
-    and run the respective main function when chosen.
-    """
-    parser.add_argument(
-        "input", type=Path,
-        help="Path to training data files"
-    )
-    parser.add_argument(
-        "output", type=Path,
-        help="Path to the HDF5 file to store the results in"
-    )
-
-    parser.add_argument(
-        "--params", default="./params.yaml", type=Path,
-        help="Path to parameter file"
-    )
-    parser.add_argument(
-        "--modalities", nargs="+",
-        default=["max_llh"],
-        help="List of modalities for inference. Must be defined in `params.yaml`"
-    )
-    parser.add_argument(
-        "--plots", default="./plots", type=Path,
-        help="Directory to store plot of acor times",
-    )
-    parser.add_argument(
-        "--ti", action="store_true",
-        help="Perform thermodynamic integration"
-    )
-    parser.add_argument(
-        "--pools", type=int, required=False,
-        help=(
-            "Number of parallel worker pools (CPU cores) to use. If not provided, it "
-            "will use all cores. If set to zero, multiprocessing will not be used."
-        )
-    )
-    parser.add_argument(
-        "--seed", type=int, default=42,
-        help="Seed value to reproduce the same sampling round."
-    )
+console = Console()
 
-    parser.set_defaults(run_main=main)
 
-
-class DummyPool:
-    """
-    Dummy class returning `None` instead of a `Pool` instance when the user chose not
-    to use multiprocessing.
+class LyScriptsWarning(Warning):
     """
-    _processes = "no parallel"
+    Exception that can be raised by methods if they want the `LyScriptsReport` instance
+    to not stop and print a traceback, but display some message appropriately.
 
-    def __enter__(self):
-        return None
+    Essentially, this is a way for decorated functions to propagate messages through
+    the `report_state` decorator.
+    """
+    def __init__(self, *args: object, level: str = "info") -> None:
+        """Extract the `level` of the message (can be "info", "warning" or "error")."""
+        self.level = level
+        self.message = args[0]
+        super().__init__(*args)
+
+
+def is_streamlit_running() -> bool:
+    """Checks if code is running inside a `streamlit` app."""
+    return get_script_run_ctx() is not None
+
+
+class CustomProgress(Progress):
+    """Small wrapper around rich's `Progress` initializing my custom columns."""
+    def __init__( self, **kwargs: dict):
+        columns = [
+            SpinnerColumn(finished_text=CHECK),
+            *Progress.get_default_columns(),
+            TimeElapsedColumn(),
+        ]
+        super().__init__(*columns, **kwargs)
+
+
+class CustomRichHandler(RichHandler):
+    """Uses `func_filepath` from the `extra` dict to modify `pathname`."""
+    def emit(self, record: LogRecord) -> None:
+        """Emit a log record."""
+        if (
+            "func_filepath" in record.__dict__
+            and "func_name" in record.__dict__
+            and "module_name" in record.__dict__
+        ):
+            prefix = record.pathname.rsplit("lyscripts")[0]
+            record.pathname = f"{prefix}lyscripts/{record.func_filepath}"
+            record.filename = record.func_filepath.split("/")[-1]
+            record.funcName = record.func_name
+            record.module = record.module_name
+            record.lineno = 0
+        return super().emit(record)
+
+
+def binom_pmf(support: list[int] | np.ndarray, p: float = 0.5):
+    """Binomial PMF"""
+    max_time = len(support) - 1
+    if p > 1. or p < 0.:
+        raise ValueError("Binomial prob must be btw. 0 and 1")
+    q = 1. - p
+    binom_coeff = factorial(max_time) / (factorial(support) * factorial(max_time - support))
+    return binom_coeff * p**support * q**(max_time - support)
+
+
+FUNCS = {
+    "binomial": binom_pmf,
+}
+
+
+def graph_from_config(graph_params: dict) -> dict[tuple[str, str], list[str]]:
+    """Build graph dictionary for the `lymph` models from the YAML params."""
+    lymph_graph = {}
+
+    if not "tumor" in graph_params and "lnl" in graph_params:
+        raise KeyError("Parameters must define tumors and LNLs")
+
+    for node_type, node_dict in graph_params.items():
+        for node_name, out_connections in node_dict.items():
+            lymph_graph[(node_type, node_name)] = out_connections
+
+    return lymph_graph
+
+
+def add_tstage_marg(
+    model: types.Model,
+    t_stages: list[str],
+    first_binom_prob: float,
+    max_time: int,
+):
+    """Add margializors over diagnosis times to `model`."""
+    support = np.arange(max_time + 1)
+    for i, stage in enumerate(t_stages):
+        if i == 0:
+            model.set_distribution(stage, binom_pmf(support, first_binom_prob))
+        else:
+            model.set_distribution(stage, binom_pmf)
 
-    def __exit__(self, exc_type, exc_value, traceback):
-        pass
 
+@deprecated(reason="Use new config file version.")
+def _create_model_from_v0(params: dict[str, Any]) -> types.Model:
+    """Create a model instance as defined by some YAML params."""
+    if "graph" in params:
+        graph = graph_from_config(params["graph"])
+    else:
+        raise LyScriptsWarning("No graph definition found in YAML file", level="error")
 
-class ConvenienceSampler(emcee.EnsembleSampler):
-    """Class that adds some useful defaults to the `emcee.EnsembleSampler`."""
-    def __init__(
-        self,
-        nwalkers,
-        ndim,
-        log_prob_fn,
-        pool=None,
-        backend=None,
-    ):
-        """Initialize sampler with sane defaults."""
-        moves = [(emcee.moves.DEMove(), 0.8), (emcee.moves.DESnookerMove(), 0.2)]
-        super().__init__(nwalkers, ndim, log_prob_fn, pool, moves, backend=backend)
-
-
-    def run_sampling(
-        self,
-        min_steps: int = 0,
-        max_steps: int = 10000,
-        thin_by: int = 1,
-        initial_state: emcee.State | np.ndarray | None = None,
-        check_interval: int = 100,
-        trust_threshold: float = 50.,
-        rel_acor_threshold: float = 0.05,
-        progress_desc: str | None = None,
-        **kwargs,
-    ) -> dict[str, Any]:
-        """Run a round of sampling with at least `min_steps`, at most `max_steps` and
-        only keep every `thin_by` step.
-
-        Every `check_interval` iterations, convergence is checked based on
-        three criteria:
-        - did it run for at least `min_steps`?
-        - has the acor time crossed the N / `trust_threshold`?
-        - did the acor time change less than `rel_acor_threshold`?
-
-        If a `progress_desc` is provided, progress will be displayed.
-
-        Returns dictionary containing the autocorrelation times obtained during the
-        run (along with the iteration number at which they were computed) and the
-        numpy array with the coordinates of the last draw.
-        """
-        if max_steps < min_steps:
+    if "model" in params:
+        model_cls = getattr(models, params["model"]["class"])
+        if not "is_symmetric" in params["model"]["kwargs"]:
             warnings.warn(
-                "Sampling param min_steps is larger than max_steps. Swapping."
+                "The keywords `base_symmetric`, `trans_symmetric`, and `use_mixing` "
+                "have been deprecated. Please use `is_symmetric` instead.",
+                DeprecationWarning,
             )
-            tmp = max_steps
-            max_steps = min_steps
-            min_steps = tmp
-
-        if initial_state is None:
-            initial_state = np.random.uniform(
-                low=0., high=1.,
-                size=(self.nwalkers, self.ndim)
-            )
-
-        iterations = []
-        acor_times = []
-        accept_rates = []
-        old_acor = np.inf
-        is_converged = False
-
-        samples_iterator = self.sample(
-            initial_state=initial_state,
-            iterations=max_steps,
-            thin_by=thin_by,
-            **kwargs
+            params["model"]["kwargs"]["is_symmetric"] = {
+                "tumor_spread": params["model"]["kwargs"].pop("base_symmetric", False),
+                "lnl_spread": params["model"]["kwargs"].pop("trans_symmetric", True),
+            }
+        model = model_cls(graph, **params["model"]["kwargs"])
+
+        add_tstage_marg(
+            model,
+            t_stages=params["model"]["t_stages"],
+            first_binom_prob=params["model"]["first_binom_prob"],
+            max_time=params["model"]["max_t"],
+        )
+    else:
+        raise LyScriptsWarning(
+            "No model class and constructor params found in YAML file",
+            level="error",
         )
-        # wrap the iteration over samples in a rich tracker,
-        # if verbosity is desired
-        if progress_desc is not None:
-            report_progress = CustomProgress(console=report)
-            samples_iterator = report_progress.track(
-                sequence=samples_iterator,
-                total=max_steps,
-                description=progress_desc,
-            )
-            report_progress.start()
 
-        coords = None
-        for sample in samples_iterator:
-            # after `check_interval` number of samples...
-            coords = sample.coords
-            if self.iteration < min_steps or self.iteration % check_interval:
-                continue
-
-            # ...get the acceptance rate up to this point
-            accept_rates.append(100. * np.mean(self.acceptance_fraction))
-
-            # ...compute the autocorrelation time and store it in an array.
-            new_acor = self.get_autocorr_time(tol=0)
-            iterations.append(self.iteration)
-            acor_times.append(np.mean(new_acor))
+    if "modalities" in params:
+        for name, modality in params["modalities"].items():
+            model.set_modality(name, spec=modality.spec, sens=modality.sens)
+
+    return model
+
+
+def assign_modalities(
+    model: types.Model,
+    config: dict[str, Any],
+    subset: list[str] | set[str] | None = None,
+    clear: bool = True,
+) -> None:
+    """Assign modalities to the ``model`` based on the ``mod_config``.
+
+    Every key in the ``from_config`` dictionary is a modality name and its corresponding
+    value is either a dictionary with keys ``spec``, ``sens`` (for specificity and
+    sensitivity of the diagnostic modality), and (optionally) ``kind`` which may be
+    either ``clinical`` or ``pathology``. The latter only plays a role in trinary
+    models. Alternatively, the value can be a tuple with the same values in the same
+    order.
+
+    The ``subset`` parameter can be used to only assign a subset of the modalities
+    to the ``model``.
+
+    Example:
+
+    >>> from_config = {
+    ...     "CT": {"spec": 0.76, "sens": 0.81},
+    ...     "MRI": [0.63, 0.86, "pathological"],
+    ... }
+    >>> model = models.Unilateral.binary(graph_dict={
+    ...     ("tumor", "T"): ["II", "III"],
+    ...     ("lnl", "II"): ["III"],
+    ...     ("lnl", "III"): [],
+    ... })
+    >>> assign_modalities(model, from_config)
+    >>> model.get_all_modalities()   # doctest: +NORMALIZE_WHITESPACE
+    {'CT': Clinical(spec=0.76, sens=0.81, is_trinary=False),
+     'MRI': Pathological(spec=0.63, sens=0.86, is_trinary=False)}
+    >>> assign_modalities(model, from_config, subset=["CT"])
+    >>> model.get_all_modalities()   # doctest: +NORMALIZE_WHITESPACE
+    {'CT': Clinical(spec=0.76, sens=0.81, is_trinary=False)}
+    """
+    if clear:
+        model.clear_modalities()
 
-            logger.debug(
-                f"Acceptance rate at {self.iteration}: {accept_rates[-1]:.2f}%"
-            )
-            logger.debug(
-                f"Autocorrelation time at {self.iteration}: {acor_times[-1]:.2f}"
+    for mod_name, mod_val in config.items():
+        if subset is not None and mod_name not in subset:
+            continue
+        try:
+            model.set_modality(
+                mod_name,
+                spec=mod_val["spec"],
+                sens=mod_val["sens"],
+                kind=mod_val.get("kind", "clinical"),
             )
+        except TypeError:
+            model.set_modality(mod_name, *mod_val)
+
+
+def create_distribution(config: dict[str, Any]) -> diagnosis_times.Distribution:
+    """Create a distribution instance as defined by a ``config`` dictionary."""
+    max_time = config["max_time"]
+    kwargs = config.get("kwargs", {})
+
+    if (type_ := config.get("frozen")) is not None:
+        kwargs.update({"support": np.arange(max_time+1)})
+        distribution = diagnosis_times.Distribution(FUNCS[type_](**kwargs))
+    elif (type_ := config.get("parametric")) is not None:
+        distribution = diagnosis_times.Distribution(FUNCS[type_], max_time, **kwargs)
+    else:
+        raise LyScriptsWarning("No distribution type found", level="error")
+
+    return distribution
+
+
+@log_state()
+def create_model(config: dict[str, Any], config_version: int = 0) -> types.Model:
+    """Create a model instance as defined by a ``config`` dictionary."""
+    if (version := config.get("version", config_version)) == 0:
+        return _create_model_from_v0(config)
+
+    if version > 1:
+        raise LyScriptsWarning(f"{version=} unsupported", level="error")
 
-            # check convergence
-            is_converged = self.iteration >= min_steps
-            is_converged &= np.all(new_acor * trust_threshold < self.iteration)
-            rel_acor_diff = np.abs(old_acor - new_acor) / new_acor
-            is_converged &= np.all(rel_acor_diff < rel_acor_threshold)
-
-            # if it has converged, stop
-            if is_converged:
-                break
-
-            old_acor = new_acor
-
-        iterations.append(self.iteration)
-        acor_times.append(np.mean(self.get_autocorr_time(tol=0)))
-        accept_rates.append(100. * np.mean(self.acceptance_fraction))
-        accept_rate_str = f"acceptance rate was {accept_rates[-1]:.2f}%"
-
-        if progress_desc is not None:
-            report_progress.stop()
-            if is_converged:
-                logging.info(f"{progress_desc} converged, {accept_rate_str}")
-            else:
-                logging.info(
-                    f"{progress_desc} finished: Max. steps reached, {accept_rate_str}"
-                )
-
-        return {
-            "iterations": iterations,
-            "acor_times": acor_times,
-            "accept_rates": accept_rates,
-            "final_state": coords,
-        }
-
-
-def run_mcmc_with_burnin(
-    nwalkers: int,
-    ndim: int,
-    log_prob_fn: Callable,
-    nsteps: int,
-    persistent_backend: emcee.backends.HDFBackend,
-    sampling_kwargs: dict | None = None,
-    burnin: int | None = None,
-    keep_burnin: bool = False,
-    thin_by: int = 1,
-    npools: int | None = None,
-    verbose: bool = True,
-) -> dict[str, Any]:
+    if (graph_config := config.get("graph")) is None:
+        raise LyScriptsWarning("No graph definition found in YAML file", level="error")
+
+    if (model_config := config.get("model")) is None:
+        raise LyScriptsWarning("No model definition found in YAML file", level="error")
+
+    graph_dict = graph_from_config(graph_config)
+    model_cls_name, _, cls_meth_name = model_config["class"].partition(".")
+    model_cls = getattr(models, model_cls_name)
+    if cls_meth_name != "":
+        model_cls = getattr(model_cls, cls_meth_name)
+    model_kwargs = model_config.get("kwargs", {})
+    model = model_cls(graph_dict, **model_kwargs)
+
+    assign_modalities(model=model, config=config.get("modalities", {}))
+
+    for t_stage, dist_config in model_config.get("distributions", {}).items():
+        distribution = create_distribution(dist_config)
+        model.set_distribution(t_stage, distribution)
+
+    return model
+
+
+def get_dict_depth(nested: dict) -> int:
+    """Get the depth of a nested dictionary.
+
+    >>> get_dict_depth({"a": {"b": 1}})
+    2
+    >>> varying_depth = {"a": {"b": 1}, "c": {"d": {"e": 2}}}
+    >>> get_dict_depth(varying_depth)
+    3
     """
-    Draw samples from the `log_prob_fn` using the `ConvenienceSampler` (subclass of
-    `emcee.EnsembleSampler`).
+    if not isinstance(nested, dict):
+        return 0
 
-    This function first draws `burnin` samples (that are discarded if `keep_burnin`
-    is set to `False`) and afterwards it performs a second sampling round, starting
-    where the burnin left off, of length `nsteps` that will be stored in the
-    `persistent_backend`.
+    max_depth = None
+    for _, value in nested.items():
+        value_depth = get_dict_depth(value)
+        max_depth = max(max_depth or value_depth, value_depth)
 
-    When `burnin` is not given, the burnin phase will still take place and it will
-    sample until convergence using convergence criteria defined via `sampling_kwargs`,
-    after which it will draw another `nsteps` samples.
+    return 1 + (max_depth or 0)
 
-    Only every `thin_by` step will be made persistent.
 
-    If `verbose` is set to `True`, the progress will be displayed.
+def delete_private_keys(nested: dict) -> dict:
+    """Delete private keys from a nested dictionary.
 
-    Returns a dictionary with some information about the burnin phase.
+    A 'private' key is a key whose name starts with an underscore. For example:
+
+    >>> delete_private_keys({"patient": {"__doc__": "some patient info", "age": 61}})
+    {'patient': {'age': 61}}
+    >>> delete_private_keys({"patient": {"age": 61}})
+    {'patient': {'age': 61}}
     """
-    if sampling_kwargs is None:
-        sampling_kwargs = {}
+    cleaned = {}
 
-    if npools is None:
-        created_pool = Pool(os.cpu_count())
-    elif npools == 0:
-        created_pool = DummyPool()
-    elif 0 < npools:
-        created_pool = Pool(np.minimum(npools, os.cpu_count()))
+    if isinstance(nested, dict):
+        for key, value in nested.items():
+            if not (isinstance(key, str) and key.startswith("_")):
+                cleaned[key] = delete_private_keys(value)
     else:
-        raise ValueError(
-            "Number of pools must be integer larger or equal to 0 (or `None`)"
-        )
+        cleaned = nested
 
-    with created_pool as pool:
-        # Burnin phase
-        if keep_burnin:
-            burnin_backend = persistent_backend
-        else:
-            burnin_backend = emcee.backends.Backend()
+    return cleaned
 
-        burnin_sampler = ConvenienceSampler(
-            nwalkers, ndim, log_prob_fn,
-            pool=pool, backend=burnin_backend,
-        )
 
-        if burnin is None:
-            burnin_result = burnin_sampler.run_sampling(
-                progress_desc=f"Burn-in ({created_pool._processes} cores)" if verbose else None,
-                **sampling_kwargs,
-            )
-        else:
-            burnin_result = burnin_sampler.run_sampling(
-                min_steps=burnin,
-                max_steps=burnin,
-                progress_desc=f"Burn-in ({created_pool._processes} cores)" if verbose else None,
-            )
+def flatten(
+    nested: dict,
+    prev_key: tuple = (),
+    max_depth: int | None = None,
+) -> dict:
+    """Flatten ``nested`` dict by creating key tuples for each value at ``max_depth``.
+
+    >>> nested = {"tumor": {"1": {"t_stage": 1, "size": 12.3}}}
+    >>> flatten(nested)
+    {('tumor', '1', 't_stage'): 1, ('tumor', '1', 'size'): 12.3}
+    >>> mapping = {"patient": {"#": {"age": {"func": int, "columns": ["age"]}}}}
+    >>> flatten(mapping, max_depth=3)
+    {('patient', '#', 'age'): {'func': <class 'int'>, 'columns': ['age']}}
 
-        sampler = ConvenienceSampler(
-            nwalkers, ndim, log_prob_fn,
-            pool=pool, backend=persistent_backend,
-        )
-        sampler.run_sampling(
-            min_steps=nsteps,
-            max_steps=nsteps,
-            thin_by=thin_by,
-            initial_state=burnin_result["final_state"],
-            progress_desc=f"Sampling ({created_pool._processes} cores)" if verbose else None,
-        )
+    Note that flattening an already flat dictionary will yield some weird results.
+    """
+    result = {}
 
-        return burnin_result
+    for key, value in nested.items():
+        is_dict = isinstance(value, dict)
+        has_reached_max_depth = max_depth is not None and len(prev_key) >= max_depth - 1
 
+        if is_dict and not has_reached_max_depth:
+            result.update(flatten(value, (*prev_key, key), max_depth))
+        else:
+            result[(*prev_key, key)] = value
 
-MODEL = None
-INV_TEMP = 1.
+    return result
 
-def log_prob_fn(theta: np.array) -> float:
-    """log probability function using global variables because of pickling."""
-    llh = MODEL.likelihood(given_param_args=theta)
-    if np.isinf(llh):
-        return -np.inf, -np.inf
-    return INV_TEMP * llh, llh
 
+def unflatten(flat: dict) -> dict:
+    """Take a flat dictionary with tuples of keys and create nested dict from it.
 
-def main(args: argparse.Namespace) -> None:
+    >>> flat = {('tumor', '1', 't_stage'): 1, ('tumor', '1', 'size'): 12.3}
+    >>> unflatten(flat)
+    {'tumor': {'1': {'t_stage': 1, 'size': 12.3}}}
+    >>> mapping = {('patient', '#', 'age'): {'func': int, 'columns': ['age']}}
+    >>> unflatten(mapping)
+    {'patient': {'#': {'age': {'func': <class 'int'>, 'columns': ['age']}}}}
     """
-    First, this program reads in the parameter YAML file and the CSV training data.
-    After that, it parses the loaded configuration and creates an instance of the model
-    that loads the training data.
-
-    From there - depending on the user input - it either performs thermodynamic
-    integration [^1] to compute the data's evidence given this particular model or it
-    draws directly from the posterior of the parameters given the data. In the latter
-    case it automatically samples until convergence. It uses the amazing
-    [`emcee`](https://github.com/dfm/emcee) library for the MCMC process.
-
-    The drawn samples are always stored in and HDF5 file and some progress about the
-    sampling procedures is stored as well (acceptance rates of samples, estimates
-    of the chains' autocorrelation times and the accuracy during the runs).
-
-    Th help via `lyscripts sample --help` shows this output:
-
-    ```
-    USAGE: lyscripts sample [-h] [--params PARAMS]
-                            [--modalities MODALITIES [MODALITIES ...]] [--plots PLOTS]
-                            [--ti] [--pools POOLS] [--seed SEED]
-                            input output
-
-    Learn the spread probabilities of the HMM for lymphatic tumor progression using
-    the preprocessed data as input and MCMC as sampling method.
-
-    This is the central script performing for our project on modelling lymphatic
-    spread in head & neck cancer. We use it for model comparison via the thermodynamic
-    integration functionality and use the sampled parameter estimates for risk
-    predictions. This risk estimate may in turn some day guide clinicians to make more
-    objective decisions with respect to defining the *elective clinical target volume*
-    (CTV-N) in radiotherapy.
-
-    POSITIONAL ARGUMENTS:
-      input                 Path to training data files
-      output                Path to the HDF5 file to store the results in
-
-    OPTIONAL ARGUMENTS:
-      -h, --help            show this help message and exit
-      --params PARAMS       Path to parameter file (default: ./params.yaml)
-      --modalities MODALITIES [MODALITIES ...]
-                            List of modalities for inference. Must be defined in
-                            `params.yaml` (default: ['max_llh'])
-      --plots PLOTS         Directory to store plot of acor times (default: ./plots)
-      --ti                  Perform thermodynamic integration (default: False)
-      --pools POOLS         Number of parallel worker pools (CPU cores) to use. If not
-                            provided, it will use all cores. If set to zero,
-                            multiprocessing will not be used. (default: None)
-      --seed SEED           Seed value to reproduce the same sampling round. (default:
-                            42)
-    ```
+    result = {}
 
-    [^1]: https://doi.org/10.1007/s11571-021-09696-9
-    """
-    params = load_yaml_params(args.params)
+    for keys, value in flat.items():
+        current = result
+        for key in keys[:-1]:
+            current = current.setdefault(key, {})
 
-    inference_data = pd.read_csv(args.input, header=[0,1,2])
-    logger.info(f"Read in training data from {args.input}")
+        current[keys[-1]] = value
 
-    global MODEL  # ugly, but necessary for pickling
-    MODEL = model_from_config(
-        graph_params=params["graph"],
-        model_params=params["model"],
-        modalities_params=get_modalities_subset(
-            defined_modalities=params["modalities"],
-            selection=args.modalities,
-        ),
-    )
-    MODEL.load_patient_data(inference_data)
-    ndim = len(MODEL.get_params())
-    nwalkers = ndim * params["sampling"]["walkers_per_dim"]
-    thin_by = params["sampling"]["thin_by"]
-    logger.info(
-        f"Set up {type(MODEL)} model with {ndim} parameters and loaded "
-        f"{len(inference_data)} patients"
-    )
-
-    # Not sure this is working. emcee sadly does not support numpy's new
-    # random number generator yet.
-    np.random.seed(args.seed)
-    if args.ti:
-        global INV_TEMP
-
-        # make sure path to output file exists
-        args.output.parent.mkdir(parents=True, exist_ok=True)
-
-        # set up sampling params
-        temp_schedule = params["sampling"]["temp_schedule"]
-        nsteps = params["sampling"]["nsteps"]
-        burnin = params["sampling"]["burnin"]
-        logger.info("Prepared thermodynamic integration.")
-
-        # record some information about each burnin phase
-        x_axis = temp_schedule.copy()
-        plots = {
-            "acor_times": [],
-            "accept_rates": [],
-        }
-        for i,inv_temp in enumerate(temp_schedule):
-            INV_TEMP = inv_temp
-            logger.info(f"TI round {i+1}/{len(temp_schedule)} with β = {INV_TEMP}")
-
-            # set up backend
-            hdf5_backend = emcee.backends.HDFBackend(args.output, name=f"ti/{i+1:0>2d}")
-
-            burnin_info = run_mcmc_with_burnin(
-                nwalkers, ndim, log_prob_fn, nsteps,
-                persistent_backend=hdf5_backend,
-                burnin=burnin,
-                keep_burnin=False,
-                thin_by=thin_by,
-                verbose=True,
-                npools=args.pools,
-            )
-            plots["acor_times"].append(burnin_info["acor_times"][-1])
-            plots["accept_rates"].append(burnin_info["accept_rates"][-1])
+    return result
 
-        # copy last sampling round over to a group in the HDF5 file called "mcmc"
-        # because that is what other scripts expect to see, e.g. for plotting risks
-        h5_file = h5py.File(args.output, "r+")
-        h5_file.copy(f"ti/{len(temp_schedule):0>2d}", h5_file, name="mcmc")
-        logger.info("Finished thermodynamic integration.")
 
-    else:
-        # make sure path to output file exists
-        args.output.parent.mkdir(parents=True, exist_ok=True)
+def get_modalities_subset(
+    defined_modalities: dict[str, list[float]],
+    selection: list[str],
+) -> dict[str, list[float]]:
+    """Of the ``defined_modalities`` return only those mentioned in the ``selection``.
 
-        # prepare backend
-        hdf5_backend = emcee.backends.HDFBackend(args.output, name="mcmc")
+    >>> modalities = {"CT": [0.76, 0.81], "MRI": [0.63, 0.86]}
+    >>> get_modalities_subset(modalities, ["CT"])
+    {'CT': [0.76, 0.81]}
+    """
+    selected_modalities = {}
+    for mod in selection:
+        try:
+            selected_modalities[mod] = defined_modalities[mod]
+        except KeyError as key_err:
+            raise KeyError(f"Modality {mod} has not been defined yet") from key_err
+    return selected_modalities
+
+
+@log_state()
+@check_input_file_exists
+def load_patient_data(
+    file_path: Path,
+    header: list[int] | None = None,
+) -> pd.DataFrame:
+    """Load patient data from a CSV file stored at ``file``."""
+    if header is None:
+        header = [0,1,2]
+    return pd.read_csv(file_path, header=header)
+
+
+@log_state()
+@check_input_file_exists
+def load_yaml_params(file_path: Path) -> dict:
+    """Load parameters from a YAML ``file``."""
+    with open(file_path, encoding="utf-8") as file:
+        params = yaml.safe_load(file)
+    return params
+
+
+@log_state()
+@check_input_file_exists
+def load_model_samples(
+    file_path: Path,
+    name: str = "mcmc",
+    flat: bool = True,
+    discard: int = 0,
+    thin: int = 1,
+) -> np.ndarray:
+    """Load MCMC samples stored in an HDF5 file at ``file_path`` under a key ``name``."""
+    backend = HDFBackend(file_path, name=name, read_only=True)
+    return backend.get_chain(flat=flat, discard=discard, thin=thin)
+
+
+@log_state()
+@check_output_dir_exists
+def initialize_backend(
+    file_path: Path,
+    nwalkers: int | None = None,
+    ndim: int | None = None,
+    name: str = "mcmc",
+    reset: bool = False,
+) -> HDFBackend:
+    """Open an HDF5 file at ``file_path`` and return a backend."""
+    backend = HDFBackend(file_path, name=name)
+
+    if reset:
+        backend.reset(nwalkers, ndim)
+
+    return backend
+
+
+NoneChoices = Literal["none", "unknown", "na", "?", "x"]
+"""Type alias for what is interpreted as unknown/ignored involvement of an LNL."""
+
+TrueChoices = Literal["true", "t", "yes", "y", "involved", "metastatic"]
+"""Type alias for what is interpreted as involved/metastatic involvement of an LNL."""
 
-        logger.info(f"Prepared sampling params & backend at {args.output}")
+FalseChoices = Literal["false", "f", "no", "n", "healthy", "benign"]
+"""Type alias for what is interpreted as healthy/benign involvement of an LNL."""
 
-        burnin_info = run_mcmc_with_burnin(
-            nwalkers, ndim, log_prob_fn,
-            nsteps=params["sampling"]["nsteps"],
-            persistent_backend=hdf5_backend,
-            sampling_kwargs=params["sampling"]["kwargs"],
-            thin_by=thin_by,
-            verbose=True,
-            npools=args.pools,
-        )
-        x_axis = np.array(burnin_info["iterations"])
-        plots = {
-            "acor_times": burnin_info["acor_times"],
-            "accept_rates": burnin_info["accept_rates"]
-        }
-
-    args.plots.mkdir(parents=True, exist_ok=True)
-
-    for name, y_axis in plots.items():
-        tmp_df = pd.DataFrame(
-            np.array([x_axis, y_axis]).T,
-            columns=["x", name],
-        )
-        tmp_df.to_csv(args.plots/(name + ".csv"), index=False)
+def optional_bool(value: NoneChoices | TrueChoices | FalseChoices) -> bool | None:
+    """Convert a string to a boolean or ``None``.
+
+    See the type aliases :py:data:`NoneChoices`, :py:data:`TrueChoices`, and
+    :py:data:`FalseChoices` for the possible values that can be converted.
+    """
+    if value.lower() in ["none", "unknown", "na", "?", "x"]:
+        return None
+
+    if value.lower() in ["true", "t", "yes", "y", "involved", "metastatic"]:
+        return True
 
-    logger.info(f"Stored {len(plots)} plots about burnin phases at {args.plots}")
-    return None
+    if value.lower() in ["false", "f", "no", "n", "healthy", "benign"]:
+        return False
 
+    raise ValueError(f"Could not convert '{value}' to a boolean or None.")
 
-if __name__ == "__main__":
-    parser = argparse.ArgumentParser(description=__doc__)
-    _add_arguments(parser)
 
-    args = parser.parse_args()
-    args.run_main(args)
+def make_pattern(
+    from_list: list[bool | None] | None,
+    lnls: list[str],
+) -> dict[str, bool | None]:
+    """Create a dictionary from a list of bools and Nones."""
+    return dict(zip(lnls, from_list or [None] * len(lnls)))
```

### Comparing `lyscripts-1.0.0a0/tests/plot/baseline/sine.png` & `lyscripts-1.0.0a1/tests/plot/baseline/sine.png`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a0/tests/plot/baseline/sine.svg` & `lyscripts-1.0.0a1/tests/plot/baseline/sine.svg`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a0/tests/plot/baseline/sine_svg.png` & `lyscripts-1.0.0a1/tests/plot/baseline/sine_svg.png`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a0/tests/plot/baseline/test_draw.png` & `lyscripts-1.0.0a1/tests/plot/baseline/test_draw.png`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a0/tests/plot/data/beta_samples.hdf5` & `lyscripts-1.0.0a1/tests/plot/data/beta_samples.hdf5`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a0/tests/plot/plot_utils_test.py` & `lyscripts-1.0.0a1/tests/plot/plot_utils_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 
 import matplotlib.pyplot as plt
 import matplotlib.testing.compare as mpl_comp
 import numpy as np
 import pytest
 
 from lyscripts.plot.utils import (
+    BetaPosterior,
     Histogram,
-    Posterior,
-    _ceil_to_step,
-    _floor_to_step,
+    ceil_to_step,
     draw,
+    floor_to_step,
     get_size,
     save_figure,
 )
 
 
 @pytest.fixture
 def beta_samples():
@@ -31,28 +31,28 @@
     """Check correct rounding down to a given step size."""
     numbers = np.array([0., 3., 7.4, 2.01, np.pi, 12.7, 12.7, 17.3 ])
     steps   = np.array([2 , 2 , 5  , 2   , 3    , 3   , 5   , 0.17 ])
     exp_res = np.array([0., 2., 5. , 2.  , 3.   , 12. , 10. , 17.17])
 
     comp_res = np.zeros_like(exp_res)
     for i, (num, step) in enumerate(zip(numbers, steps)):
-        comp_res[i] = _floor_to_step(num, step)
+        comp_res[i] = floor_to_step(num, step)
 
     assert all(np.isclose(comp_res, exp_res)), "Floor to step did not work properly."
 
 
 def test_ceil_to_step():
     """Check correct rounding up to a given step size."""
     numbers = np.array([0., 3., 7.4, 2.01, np.pi, 12.7, 12.7, 17.3 ])
     steps   = np.array([2 , 2 , 5  , 2   , 3    , 3   , 5   , 0.17 ])
     exp_res = np.array([2., 4., 10., 4.  , 6.   , 15. , 15. , 17.34])
 
     comp_res = np.zeros_like(exp_res)
     for i, (num, step) in enumerate(zip(numbers, steps)):
-        comp_res[i] = _ceil_to_step(num, step)
+        comp_res[i] = ceil_to_step(num, step)
 
     assert all(np.isclose(comp_res, exp_res)), "Ceil to step did not work properly."
 
 
 def test_histogram_cls(beta_samples):
     """Make sure the histogram data container works as intended."""
     str_filename = beta_samples
@@ -95,24 +95,24 @@
     str_filename = beta_samples
     path_filename = Path(str_filename)
     non_existent_filename = "non_existent.hdf5"
     custom_label = "Lorem ipsum"
     x_10 = np.linspace(0., 10., 100)
     x_100 = np.linspace(0., 100., 100)
 
-    post_from_str = Posterior.from_hdf5(filename=str_filename, dataname="beta")
-    post_from_path = Posterior.from_hdf5(
+    post_from_str = BetaPosterior.from_hdf5(filename=str_filename, dataname="beta")
+    post_from_path = BetaPosterior.from_hdf5(
         filename=path_filename,
         dataname="beta",
         scale=10.,
         label=custom_label,
     )
 
     with pytest.raises(FileNotFoundError):
-        Posterior.from_hdf5(filename=non_existent_filename, dataname="does_not_matter")
+        BetaPosterior.from_hdf5(filename=non_existent_filename, dataname="does_not_matter")
 
     assert post_from_str.num_success == post_from_path.num_success == 20, (
         "Number of successes not correctly extracted"
     )
     assert post_from_str.num_total == post_from_path.num_total == 40, (
         "Total number of trials not correctly extracted"
     )
@@ -135,15 +135,15 @@
 
 @pytest.mark.mpl_image_compare
 def test_draw(beta_samples):
     """Check the drawing function."""
     filename = Path(beta_samples)
     dataname = "beta"
     hist = Histogram.from_hdf5(filename, dataname)
-    post = Posterior.from_hdf5(filename, dataname)
+    post = BetaPosterior.from_hdf5(filename, dataname)
     fig, ax = plt.subplots()
     ax = draw(axes=ax, contents=[hist, post], percent_lims=(2.,2.))
     ax.legend()
     return fig
 
 
 def test_draw_hist_kwargs(beta_samples):
```

### Comparing `lyscripts-1.0.0a0/tests/predict/predict_utils_test.py` & `lyscripts-1.0.0a1/tests/predict/predict_utils_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Test utilities of the predict submodule.
 """
-from lyscripts.predict.utils import complete_pattern
+from lyscripts.compute.utils import complete_pattern
 
 
 def test_clean_pattern():
     """
     Test the utility function that cleans the involvement patterns from the
     `params.yaml` file
     """
```

### Comparing `lyscripts-1.0.0a0/tests/predict/prevalences_test.py` & `lyscripts-1.0.0a1/tests/predict/prevalences_test.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 """
 Test the functions of the prevalence prediction submodule.
 """
 import pandas as pd
 import pytest
 
-from lyscripts.predict.prevalences import does_midline_ext_match, get_match_idx
+from lyscripts.compute.prevalences import does_midext_match
+from lyscripts.data.accessor import get_match_idx
 
 
 def test_get_match_idx():
     """Test if the pattern dictionaries & pandas data are compared correctly."""
     oneside_pattern = {"I": False, "II": True, "III": None}
     ignorant_pattern = {"I": None, "II": None, "III": None}
     three_patients = pd.DataFrame.from_dict({
         "I":   [False, False, True],
         "II":  [True , True , True],
         "III": [True , False, True],
     })
     lnls = list(oneside_pattern.keys())
 
     matching_idxs = get_match_idx(
-        True, oneside_pattern, three_patients, lnls, invert=False
+        True, oneside_pattern, three_patients, invert=False
     )
     inverted_matching_idxs = get_match_idx(
-        False, oneside_pattern, three_patients, lnls, invert=True
+        False, oneside_pattern, three_patients, invert=True
     )
     ignorant_matching_idxs = get_match_idx(
-        True, ignorant_pattern, three_patients, lnls, invert=False
+        True, ignorant_pattern, three_patients, invert=False
     )
 
     assert all(
         matching_idxs == pd.Series([True, True, False])
     ), "Patients were incorrectly matched with pattern."
     assert all(
         inverted_matching_idxs == pd.Series([False, False, True])
@@ -40,29 +41,19 @@
 
 
 def test_does_midline_ext_match():
     """
     Test the function that returns indices of a `DataFrame` where the midline
     extension matches.
     """
-    uni_data = pd.DataFrame({("two", "levels"): [True, False, None]})
     midline_data = pd.DataFrame({
-        ("info", "tumor", "midline_extension"): [True, False, None]
+        ("tumor", "1", "extension"): [True, False, None]
     })
     keyerr_data = pd.DataFrame({("way", "too", "many", "levels"): [True, False, None]})
 
-    uni_match_none = does_midline_ext_match(uni_data)
-    uni_match = does_midline_ext_match(uni_data, midline_ext=False)
-    midline_match = does_midline_ext_match(midline_data, midline_ext=False)
+    midline_match = does_midext_match(midline_data, midext=False)
 
-    assert uni_match_none is True, (
-        "When matching against `None`, function should always return `True`."
-    )
-    assert uni_match is True, (
-        "Data with two-level header should always match, "
-        "because they don't have midline data."
-    )
     assert all(midline_match == pd.Series([False, True, False])), (
         "Matching midline extension with correct data does not work."
     )
     with pytest.raises(KeyError):
-        _ = does_midline_ext_match(keyerr_data, midline_ext=False)
+        _ = does_midext_match(keyerr_data, midext=False)
```

### Comparing `lyscripts-1.0.0a0/tests/sample_test.py` & `lyscripts-1.0.0a1/tests/sample_test.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,80 +2,91 @@
 Test the sampling command with some example patients.
 
 Originally, I wanted to test that the sampling procedure is reproducible, but the
 `emcee` package does not seem to work with any kind of seed in a reproducible manner.
 
 Maybe I am doing something wrong...
 """
+# pylint: disable=redefined-outer-name
 import numpy as np
-import pandas as pd
 import pytest
-from emcee.backends import Backend, HDFBackend
+from emcee import EnsembleSampler, backends
+from lymph import types
 
-from lyscripts.sample import run_mcmc_with_burnin
-from lyscripts.utils import (
-    LymphModel,
-    create_model_from_config,
-    load_patient_data,
-    load_yaml_params,
-)
+from lyscripts.sample import get_starting_state, run_burnin
+from lyscripts.utils import create_model, load_patient_data, load_yaml_params
 
 
 @pytest.fixture
 def params() -> dict:
-    """Fixture providing stored `test_params.yaml` file."""
-    return load_yaml_params("./tests/test_params.yaml")
+    """Fixture providing stored `test_sample_params.yaml` file."""
+    return load_yaml_params("./tests/test_sample_params.yaml")
 
 
 @pytest.fixture
-def model(params: dict) -> LymphModel:
+def model(params: dict) -> types.Model:
     """Model fixture from parameters."""
-    return create_model_from_config(params)
+    return create_model(params)
 
 
 @pytest.fixture
-def data(model: LymphModel) -> pd.DataFrame:
+def loaded_model(model: types.Model) -> types.Model:
     """Get synthetically generated data from disk."""
-    return load_patient_data("./tests/test_data.csv")
+    data = load_patient_data("./tests/test_data.csv")
+    model.load_patient_data(data)
+    return model
 
 
 @pytest.fixture
-def backend() -> Backend:
-    """Provide a non-persistent backend to store samples during the test run."""
-    return Backend()
+def hdf5_backend(tmp_path) -> backends.HDFBackend:
+    """Load previously sampled backend for comparison."""
+    return backends.HDFBackend(tmp_path / "tmp.hdf5")
 
 
 @pytest.fixture
-def stored_hdf5_backend() -> HDFBackend:
-    """Load previously sampled backend for comparison."""
-    return HDFBackend("./tests/test_backend.hdf5", read_only=True)
+def sampler(model: types.Model, hdf5_backend: backends.HDFBackend) -> EnsembleSampler:
+    """Construct a sampler for the model."""
+    np.random.seed(42)
+    ndim = model.get_num_dims()
+    nwalkers = ndim * 10
+    return EnsembleSampler(
+        nwalkers=nwalkers,
+        ndim=ndim,
+        log_prob_fn=model.likelihood,
+        backend=hdf5_backend,
+    )
 
 
-def test_sampling(
-    model: LymphModel,
-    data: pd.DataFrame,
-    params: dict,
-    backend: Backend,
-    stored_hdf5_backend: HDFBackend,
-):
-    """Test the basic sampling function."""
-    model.load_patient_data(data, mapping=lambda x: x)
-    ndim = len(model.get_params())
-    nwalker = ndim * params["sampling"]["walkers_per_dim"]
-
-    def log_prob_fn(theta: np.ndarray) -> float:
-        """The log-probability function to sample from."""
-        return model.likelihood(given_param_args=theta)
-
-    np.random.seed(128)
-    info = run_mcmc_with_burnin(
-        nwalker, ndim, log_prob_fn,
-        persistent_backend=backend,
-        nsteps=params["sampling"]["nsteps"],
-        burnin=params["sampling"]["burnin"],
-        keep_burnin=False,
-        npools=0,
+def test_burnin(sampler: EnsembleSampler):
+    """Test the burnin function."""
+    burnin_history = run_burnin(
+        sampler=sampler,
+        burnin=100,
+        check_interval=10,
     )
-
-    actual_chain = backend.get_chain(flat=True)
-    expected_chain = stored_hdf5_backend.get_chain(flat=True)
-    assert np.all(np.isclose(actual_chain, expected_chain)), "Chain was not reproduced"
+    assert sampler.iteration == 100, "Burnin di not run 100 iterations."
+    assert len(burnin_history.steps) == 10, "Burnin history does not have 10 entries."
+    assert np.all(
+        np.array([
+            0.7147557514447068, 0.9227188150264771,
+            0.2629624184410706, 0.6001184115584288,
+        ])
+        == sampler.get_last_sample().coords[0]
+    ), "Not reproducible."
+
+
+def test_get_starting_state(sampler: EnsembleSampler):
+    """Test if the starting state can be retrieved."""
+    state = get_starting_state(sampler)
+    with pytest.raises(AttributeError):
+        sampler.get_last_sample()
+    assert state.shape == (sampler.nwalkers, sampler.ndim), "State has wrong shape."
+
+    _ = run_burnin(
+        sampler=sampler,
+        burnin=10,
+        check_interval=2,
+    )
+    assert np.all(
+        get_starting_state(sampler).coords
+        == sampler.get_last_sample().coords
+    ), "State is not the same."
```

### Comparing `lyscripts-1.0.0a0/tests/test_backend.hdf5` & `lyscripts-1.0.0a1/tests/test_backend.hdf5`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a0/tests/test_params.yaml` & `lyscripts-1.0.0a1/tests/test_params_v0.yaml`

 * *Files identical despite different names*

