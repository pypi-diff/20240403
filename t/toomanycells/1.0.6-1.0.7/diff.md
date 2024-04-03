# Comparing `tmp/toomanycells-1.0.6.tar.gz` & `tmp/toomanycells-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toomanycells-1.0.6.tar", last modified: Wed Apr  3 20:42:31 2024, max compression
+gzip compressed data, was "toomanycells-1.0.7.tar", last modified: Wed Apr  3 20:58:52 2024, max compression
```

## Comparing `toomanycells-1.0.6.tar` & `toomanycells-1.0.7.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:42:31.689061 toomanycells-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-03 20:42:18.000000 toomanycells-1.0.6/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:42:31.673061 toomanycells-1.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:42:31.677061 toomanycells-1.0.6/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-03 20:42:18.000000 toomanycells-1.0.6/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-03 20:42:18.000000 toomanycells-1.0.6/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-03 20:42:18.000000 toomanycells-1.0.6/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:42:31.677061 toomanycells-1.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-03 20:42:18.000000 toomanycells-1.0.6/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-03 20:42:18.000000 toomanycells-1.0.6/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-03 20:42:18.000000 toomanycells-1.0.6/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-03 20:42:18.000000 toomanycells-1.0.6/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-03 20:42:18.000000 toomanycells-1.0.6/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-03 20:42:18.000000 toomanycells-1.0.6/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-03 20:42:18.000000 toomanycells-1.0.6/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-03 20:42:18.000000 toomanycells-1.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-03 20:42:18.000000 toomanycells-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-03 20:42:18.000000 toomanycells-1.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8589 2024-04-03 20:42:31.689061 toomanycells-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7546 2024-04-03 20:42:18.000000 toomanycells-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:42:31.681061 toomanycells-1.0.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-03 20:42:18.000000 toomanycells-1.0.6/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-03 20:42:18.000000 toomanycells-1.0.6/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-03 20:42:18.000000 toomanycells-1.0.6/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:42:31.681061 toomanycells-1.0.6/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-03 20:42:18.000000 toomanycells-1.0.6/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-03 20:42:18.000000 toomanycells-1.0.6/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-03 20:42:18.000000 toomanycells-1.0.6/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-03 20:42:18.000000 toomanycells-1.0.6/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:42:31.681061 toomanycells-1.0.6/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-03 20:42:18.000000 toomanycells-1.0.6/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-03 20:42:18.000000 toomanycells-1.0.6/docs/toomanycells.md
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-03 20:42:18.000000 toomanycells-1.0.6/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-03 20:42:18.000000 toomanycells-1.0.6/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-03 20:42:18.000000 toomanycells-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 20:42:18.000000 toomanycells-1.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-03 20:42:18.000000 toomanycells-1.0.6/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 20:42:31.689061 toomanycells-1.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:42:31.685061 toomanycells-1.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-03 20:42:18.000000 toomanycells-1.0.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-03 20:42:18.000000 toomanycells-1.0.6/tests/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-03 20:42:18.000000 toomanycells-1.0.6/tests/benchmark_table.csv
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-03 20:42:18.000000 toomanycells-1.0.6/tests/benchmark_table_mod.csv
--rw-r--r--   0 runner    (1001) docker     (127)   803420 2024-04-03 20:42:18.000000 toomanycells-1.0.6/tests/example_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-03 20:42:18.000000 toomanycells-1.0.6/tests/log_benchmark_table.csv
--rw-r--r--   0 runner    (1001) docker     (127)   169679 2024-04-03 20:42:18.000000 toomanycells-1.0.6/tests/log_linear_iter.png
--rw-r--r--   0 runner    (1001) docker     (127)   171516 2024-04-03 20:42:18.000000 toomanycells-1.0.6/tests/log_linear_time.png
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-03 20:42:18.000000 toomanycells-1.0.6/tests/plot_linear_model_for_iter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-03 20:42:18.000000 toomanycells-1.0.6/tests/plot_linear_model_for_time.py
--rw-r--r--   0 runner    (1001) docker     (127)    36791 2024-04-03 20:42:18.000000 toomanycells-1.0.6/tests/tabula_sapiens_time.png
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-03 20:42:18.000000 toomanycells-1.0.6/tests/test_toomanycells.py
--rw-r--r--   0 runner    (1001) docker     (127)  2027414 2024-04-03 20:42:18.000000 toomanycells-1.0.6/tests/tmci_tabula_sapiens.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:42:31.685061 toomanycells-1.0.6/toomanycells/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-03 20:42:18.000000 toomanycells-1.0.6/toomanycells/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-03 20:42:18.000000 toomanycells-1.0.6/toomanycells/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:42:31.689061 toomanycells-1.0.6/toomanycells/data/
--rw-r--r--   0 runner    (1001) docker     (127)    50239 2024-04-03 20:42:18.000000 toomanycells-1.0.6/toomanycells/data/metadata.csv
--rw-r--r--   0 runner    (1001) docker     (127)    23411 2024-04-03 20:42:18.000000 toomanycells-1.0.6/toomanycells/toomanycells.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:42:31.689061 toomanycells-1.0.6/toomanycells.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8589 2024-04-03 20:42:31.000000 toomanycells-1.0.6/toomanycells.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-03 20:42:31.000000 toomanycells-1.0.6/toomanycells.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 20:42:31.000000 toomanycells-1.0.6/toomanycells.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-03 20:42:31.000000 toomanycells-1.0.6/toomanycells.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-03 20:42:31.000000 toomanycells-1.0.6/toomanycells.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 20:42:31.000000 toomanycells-1.0.6/toomanycells.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:58:52.915843 toomanycells-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-03 20:58:42.000000 toomanycells-1.0.7/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:58:52.899843 toomanycells-1.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:58:52.903843 toomanycells-1.0.7/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-03 20:58:42.000000 toomanycells-1.0.7/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-03 20:58:42.000000 toomanycells-1.0.7/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-03 20:58:42.000000 toomanycells-1.0.7/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:58:52.903843 toomanycells-1.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-03 20:58:42.000000 toomanycells-1.0.7/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-03 20:58:42.000000 toomanycells-1.0.7/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-03 20:58:42.000000 toomanycells-1.0.7/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-03 20:58:42.000000 toomanycells-1.0.7/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-03 20:58:42.000000 toomanycells-1.0.7/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-03 20:58:42.000000 toomanycells-1.0.7/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-03 20:58:42.000000 toomanycells-1.0.7/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-03 20:58:42.000000 toomanycells-1.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-03 20:58:42.000000 toomanycells-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-03 20:58:42.000000 toomanycells-1.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8589 2024-04-03 20:58:52.915843 toomanycells-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7546 2024-04-03 20:58:42.000000 toomanycells-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:58:52.903843 toomanycells-1.0.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-03 20:58:42.000000 toomanycells-1.0.7/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-03 20:58:42.000000 toomanycells-1.0.7/docs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-03 20:58:42.000000 toomanycells-1.0.7/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:58:52.903843 toomanycells-1.0.7/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-03 20:58:42.000000 toomanycells-1.0.7/docs/examples/intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-03 20:58:42.000000 toomanycells-1.0.7/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-03 20:58:42.000000 toomanycells-1.0.7/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-03 20:58:42.000000 toomanycells-1.0.7/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:58:52.907843 toomanycells-1.0.7/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-03 20:58:42.000000 toomanycells-1.0.7/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-03 20:58:42.000000 toomanycells-1.0.7/docs/toomanycells.md
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-03 20:58:42.000000 toomanycells-1.0.7/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-03 20:58:42.000000 toomanycells-1.0.7/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-03 20:58:42.000000 toomanycells-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 20:58:42.000000 toomanycells-1.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-03 20:58:42.000000 toomanycells-1.0.7/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 20:58:52.915843 toomanycells-1.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:58:52.907843 toomanycells-1.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-03 20:58:42.000000 toomanycells-1.0.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-03 20:58:42.000000 toomanycells-1.0.7/tests/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-03 20:58:42.000000 toomanycells-1.0.7/tests/benchmark_table.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-03 20:58:42.000000 toomanycells-1.0.7/tests/benchmark_table_mod.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   803420 2024-04-03 20:58:42.000000 toomanycells-1.0.7/tests/example_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-03 20:58:42.000000 toomanycells-1.0.7/tests/log_benchmark_table.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   169679 2024-04-03 20:58:42.000000 toomanycells-1.0.7/tests/log_linear_iter.png
+-rw-r--r--   0 runner    (1001) docker     (127)   171516 2024-04-03 20:58:42.000000 toomanycells-1.0.7/tests/log_linear_time.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-03 20:58:42.000000 toomanycells-1.0.7/tests/plot_linear_model_for_iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-03 20:58:42.000000 toomanycells-1.0.7/tests/plot_linear_model_for_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36791 2024-04-03 20:58:42.000000 toomanycells-1.0.7/tests/tabula_sapiens_time.png
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-03 20:58:42.000000 toomanycells-1.0.7/tests/test_toomanycells.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2027414 2024-04-03 20:58:42.000000 toomanycells-1.0.7/tests/tmci_tabula_sapiens.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:58:52.911843 toomanycells-1.0.7/toomanycells/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-03 20:58:42.000000 toomanycells-1.0.7/toomanycells/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-03 20:58:42.000000 toomanycells-1.0.7/toomanycells/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:58:52.911843 toomanycells-1.0.7/toomanycells/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    50239 2024-04-03 20:58:42.000000 toomanycells-1.0.7/toomanycells/data/metadata.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    23411 2024-04-03 20:58:42.000000 toomanycells-1.0.7/toomanycells/toomanycells.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:58:52.911843 toomanycells-1.0.7/toomanycells.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8589 2024-04-03 20:58:52.000000 toomanycells-1.0.7/toomanycells.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-03 20:58:52.000000 toomanycells-1.0.7/toomanycells.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 20:58:52.000000 toomanycells-1.0.7/toomanycells.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-03 20:58:52.000000 toomanycells-1.0.7/toomanycells.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-03 20:58:52.000000 toomanycells-1.0.7/toomanycells.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 20:58:52.000000 toomanycells-1.0.7/toomanycells.egg-info/top_level.txt
```

### Comparing `toomanycells-1.0.6/.github/ISSUE_TEMPLATE/bug_report.md` & `toomanycells-1.0.7/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.6/.github/workflows/docs-build.yml` & `toomanycells-1.0.7/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.6/.github/workflows/docs.yml` & `toomanycells-1.0.7/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.6/.github/workflows/installation.yml` & `toomanycells-1.0.7/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.6/.github/workflows/macos.yml` & `toomanycells-1.0.7/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.6/.github/workflows/pypi.yml` & `toomanycells-1.0.7/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.6/.github/workflows/ubuntu.yml` & `toomanycells-1.0.7/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.6/.github/workflows/windows.yml` & `toomanycells-1.0.7/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.6/.gitignore` & `toomanycells-1.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.6/LICENSE` & `toomanycells-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.6/PKG-INFO` & `toomanycells-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toomanycells
-Version: 1.0.6
+Version: 1.0.7
 Summary: A python package for spectral clustering.
 Author-email: Javier Ruiz-Ramirez <javier.ruizramirez@uhn.ca>
 License: BSD License
 Project-URL: Homepage, https://github.com/JRR3/toomanycells
 Keywords: toomanycells
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `toomanycells-1.0.6/README.md` & `toomanycells-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.6/docs/contributing.md` & `toomanycells-1.0.7/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.6/docs/installation.md` & `toomanycells-1.0.7/docs/installation.md`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.6/mkdocs.yml` & `toomanycells-1.0.7/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.6/pyproject.toml` & `toomanycells-1.0.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "toomanycells"
-version = "1.0.6"
+version = "1.0.7"
 dynamic = [
     "dependencies",
 ]
 description = "A python package for spectral clustering."
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -51,15 +51,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "1.0.6"
+current_version = "1.0.7"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

### Comparing `toomanycells-1.0.6/tests/benchmark.py` & `toomanycells-1.0.7/tests/benchmark.py`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.6/tests/benchmark_table.csv` & `toomanycells-1.0.7/tests/benchmark_table.csv`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.6/tests/benchmark_table_mod.csv` & `toomanycells-1.0.7/tests/benchmark_table_mod.csv`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.6/tests/example_1.png` & `toomanycells-1.0.7/tests/example_1.png`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.6/tests/log_benchmark_table.csv` & `toomanycells-1.0.7/tests/log_benchmark_table.csv`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.6/tests/log_linear_iter.png` & `toomanycells-1.0.7/tests/log_linear_iter.png`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.6/tests/log_linear_time.png` & `toomanycells-1.0.7/tests/log_linear_time.png`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.6/tests/plot_linear_model_for_iter.py` & `toomanycells-1.0.7/tests/plot_linear_model_for_iter.py`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.6/tests/plot_linear_model_for_time.py` & `toomanycells-1.0.7/tests/plot_linear_model_for_time.py`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.6/tests/tabula_sapiens_time.png` & `toomanycells-1.0.7/tests/tabula_sapiens_time.png`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.6/tests/tmci_tabula_sapiens.png` & `toomanycells-1.0.7/tests/tmci_tabula_sapiens.png`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.6/toomanycells/common.py` & `toomanycells-1.0.7/toomanycells/common.py`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.6/toomanycells/data/metadata.csv` & `toomanycells-1.0.7/toomanycells/data/metadata.csv`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.6/toomanycells/toomanycells.py` & `toomanycells-1.0.7/toomanycells/toomanycells.py`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.6/toomanycells.egg-info/PKG-INFO` & `toomanycells-1.0.7/toomanycells.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toomanycells
-Version: 1.0.6
+Version: 1.0.7
 Summary: A python package for spectral clustering.
 Author-email: Javier Ruiz-Ramirez <javier.ruizramirez@uhn.ca>
 License: BSD License
 Project-URL: Homepage, https://github.com/JRR3/toomanycells
 Keywords: toomanycells
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `toomanycells-1.0.6/toomanycells.egg-info/SOURCES.txt` & `toomanycells-1.0.7/toomanycells.egg-info/SOURCES.txt`

 * *Files identical despite different names*

