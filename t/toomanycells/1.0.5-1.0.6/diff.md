# Comparing `tmp/toomanycells-1.0.5.tar.gz` & `tmp/toomanycells-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toomanycells-1.0.5.tar", last modified: Wed Apr  3 20:03:35 2024, max compression
+gzip compressed data, was "toomanycells-1.0.6.tar", last modified: Wed Apr  3 20:42:31 2024, max compression
```

## Comparing `toomanycells-1.0.5.tar` & `toomanycells-1.0.6.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:03:35.934231 toomanycells-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-03 20:03:25.000000 toomanycells-1.0.5/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:03:35.918231 toomanycells-1.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:03:35.922231 toomanycells-1.0.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-03 20:03:25.000000 toomanycells-1.0.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-03 20:03:25.000000 toomanycells-1.0.5/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-03 20:03:25.000000 toomanycells-1.0.5/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:03:35.922231 toomanycells-1.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-03 20:03:25.000000 toomanycells-1.0.5/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-03 20:03:25.000000 toomanycells-1.0.5/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-03 20:03:25.000000 toomanycells-1.0.5/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-03 20:03:25.000000 toomanycells-1.0.5/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-03 20:03:25.000000 toomanycells-1.0.5/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-03 20:03:25.000000 toomanycells-1.0.5/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-03 20:03:25.000000 toomanycells-1.0.5/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-03 20:03:25.000000 toomanycells-1.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-03 20:03:25.000000 toomanycells-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-03 20:03:25.000000 toomanycells-1.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8589 2024-04-03 20:03:35.934231 toomanycells-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7546 2024-04-03 20:03:25.000000 toomanycells-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:03:35.926231 toomanycells-1.0.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-03 20:03:25.000000 toomanycells-1.0.5/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-03 20:03:25.000000 toomanycells-1.0.5/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-03 20:03:25.000000 toomanycells-1.0.5/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:03:35.926231 toomanycells-1.0.5/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-03 20:03:25.000000 toomanycells-1.0.5/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-03 20:03:25.000000 toomanycells-1.0.5/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-03 20:03:25.000000 toomanycells-1.0.5/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-03 20:03:25.000000 toomanycells-1.0.5/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:03:35.926231 toomanycells-1.0.5/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-03 20:03:25.000000 toomanycells-1.0.5/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-03 20:03:25.000000 toomanycells-1.0.5/docs/toomanycells.md
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-03 20:03:25.000000 toomanycells-1.0.5/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-03 20:03:25.000000 toomanycells-1.0.5/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-03 20:03:25.000000 toomanycells-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 20:03:25.000000 toomanycells-1.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-03 20:03:25.000000 toomanycells-1.0.5/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 20:03:35.934231 toomanycells-1.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:03:35.926231 toomanycells-1.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-03 20:03:25.000000 toomanycells-1.0.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-03 20:03:25.000000 toomanycells-1.0.5/tests/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-03 20:03:25.000000 toomanycells-1.0.5/tests/benchmark_table.csv
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-03 20:03:25.000000 toomanycells-1.0.5/tests/benchmark_table_mod.csv
--rw-r--r--   0 runner    (1001) docker     (127)   803420 2024-04-03 20:03:25.000000 toomanycells-1.0.5/tests/example_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-03 20:03:25.000000 toomanycells-1.0.5/tests/log_benchmark_table.csv
--rw-r--r--   0 runner    (1001) docker     (127)   169679 2024-04-03 20:03:25.000000 toomanycells-1.0.5/tests/log_linear_iter.png
--rw-r--r--   0 runner    (1001) docker     (127)   171516 2024-04-03 20:03:25.000000 toomanycells-1.0.5/tests/log_linear_time.png
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-03 20:03:25.000000 toomanycells-1.0.5/tests/plot_linear_model_for_iter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-03 20:03:25.000000 toomanycells-1.0.5/tests/plot_linear_model_for_time.py
--rw-r--r--   0 runner    (1001) docker     (127)    36791 2024-04-03 20:03:25.000000 toomanycells-1.0.5/tests/tabula_sapiens_time.png
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-03 20:03:25.000000 toomanycells-1.0.5/tests/test_toomanycells.py
--rw-r--r--   0 runner    (1001) docker     (127)  2027414 2024-04-03 20:03:25.000000 toomanycells-1.0.5/tests/tmci_tabula_sapiens.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:03:35.930231 toomanycells-1.0.5/toomanycells/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-03 20:03:25.000000 toomanycells-1.0.5/toomanycells/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-03 20:03:25.000000 toomanycells-1.0.5/toomanycells/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:03:35.930231 toomanycells-1.0.5/toomanycells/data/
--rw-r--r--   0 runner    (1001) docker     (127)    50239 2024-04-03 20:03:25.000000 toomanycells-1.0.5/toomanycells/data/metadata.csv
--rw-r--r--   0 runner    (1001) docker     (127)    23390 2024-04-03 20:03:25.000000 toomanycells-1.0.5/toomanycells/toomanycells.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:03:35.934231 toomanycells-1.0.5/toomanycells.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8589 2024-04-03 20:03:35.000000 toomanycells-1.0.5/toomanycells.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-03 20:03:35.000000 toomanycells-1.0.5/toomanycells.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 20:03:35.000000 toomanycells-1.0.5/toomanycells.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-03 20:03:35.000000 toomanycells-1.0.5/toomanycells.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-03 20:03:35.000000 toomanycells-1.0.5/toomanycells.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 20:03:35.000000 toomanycells-1.0.5/toomanycells.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:42:31.689061 toomanycells-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-03 20:42:18.000000 toomanycells-1.0.6/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:42:31.673061 toomanycells-1.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:42:31.677061 toomanycells-1.0.6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-03 20:42:18.000000 toomanycells-1.0.6/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-03 20:42:18.000000 toomanycells-1.0.6/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-03 20:42:18.000000 toomanycells-1.0.6/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:42:31.677061 toomanycells-1.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-03 20:42:18.000000 toomanycells-1.0.6/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-03 20:42:18.000000 toomanycells-1.0.6/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-03 20:42:18.000000 toomanycells-1.0.6/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-03 20:42:18.000000 toomanycells-1.0.6/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-03 20:42:18.000000 toomanycells-1.0.6/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-03 20:42:18.000000 toomanycells-1.0.6/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-03 20:42:18.000000 toomanycells-1.0.6/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-03 20:42:18.000000 toomanycells-1.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-03 20:42:18.000000 toomanycells-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-03 20:42:18.000000 toomanycells-1.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8589 2024-04-03 20:42:31.689061 toomanycells-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7546 2024-04-03 20:42:18.000000 toomanycells-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:42:31.681061 toomanycells-1.0.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-03 20:42:18.000000 toomanycells-1.0.6/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-03 20:42:18.000000 toomanycells-1.0.6/docs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-03 20:42:18.000000 toomanycells-1.0.6/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:42:31.681061 toomanycells-1.0.6/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-03 20:42:18.000000 toomanycells-1.0.6/docs/examples/intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-03 20:42:18.000000 toomanycells-1.0.6/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-03 20:42:18.000000 toomanycells-1.0.6/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-03 20:42:18.000000 toomanycells-1.0.6/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:42:31.681061 toomanycells-1.0.6/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-03 20:42:18.000000 toomanycells-1.0.6/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-03 20:42:18.000000 toomanycells-1.0.6/docs/toomanycells.md
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-03 20:42:18.000000 toomanycells-1.0.6/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-03 20:42:18.000000 toomanycells-1.0.6/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-03 20:42:18.000000 toomanycells-1.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 20:42:18.000000 toomanycells-1.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-03 20:42:18.000000 toomanycells-1.0.6/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 20:42:31.689061 toomanycells-1.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:42:31.685061 toomanycells-1.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-03 20:42:18.000000 toomanycells-1.0.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-03 20:42:18.000000 toomanycells-1.0.6/tests/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-03 20:42:18.000000 toomanycells-1.0.6/tests/benchmark_table.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-03 20:42:18.000000 toomanycells-1.0.6/tests/benchmark_table_mod.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   803420 2024-04-03 20:42:18.000000 toomanycells-1.0.6/tests/example_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-03 20:42:18.000000 toomanycells-1.0.6/tests/log_benchmark_table.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   169679 2024-04-03 20:42:18.000000 toomanycells-1.0.6/tests/log_linear_iter.png
+-rw-r--r--   0 runner    (1001) docker     (127)   171516 2024-04-03 20:42:18.000000 toomanycells-1.0.6/tests/log_linear_time.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-03 20:42:18.000000 toomanycells-1.0.6/tests/plot_linear_model_for_iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-03 20:42:18.000000 toomanycells-1.0.6/tests/plot_linear_model_for_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36791 2024-04-03 20:42:18.000000 toomanycells-1.0.6/tests/tabula_sapiens_time.png
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-03 20:42:18.000000 toomanycells-1.0.6/tests/test_toomanycells.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2027414 2024-04-03 20:42:18.000000 toomanycells-1.0.6/tests/tmci_tabula_sapiens.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:42:31.685061 toomanycells-1.0.6/toomanycells/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-03 20:42:18.000000 toomanycells-1.0.6/toomanycells/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-03 20:42:18.000000 toomanycells-1.0.6/toomanycells/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:42:31.689061 toomanycells-1.0.6/toomanycells/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    50239 2024-04-03 20:42:18.000000 toomanycells-1.0.6/toomanycells/data/metadata.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    23411 2024-04-03 20:42:18.000000 toomanycells-1.0.6/toomanycells/toomanycells.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:42:31.689061 toomanycells-1.0.6/toomanycells.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8589 2024-04-03 20:42:31.000000 toomanycells-1.0.6/toomanycells.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-03 20:42:31.000000 toomanycells-1.0.6/toomanycells.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 20:42:31.000000 toomanycells-1.0.6/toomanycells.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-03 20:42:31.000000 toomanycells-1.0.6/toomanycells.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-03 20:42:31.000000 toomanycells-1.0.6/toomanycells.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 20:42:31.000000 toomanycells-1.0.6/toomanycells.egg-info/top_level.txt
```

### Comparing `toomanycells-1.0.5/.github/ISSUE_TEMPLATE/bug_report.md` & `toomanycells-1.0.6/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.5/.github/workflows/docs-build.yml` & `toomanycells-1.0.6/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.5/.github/workflows/docs.yml` & `toomanycells-1.0.6/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.5/.github/workflows/installation.yml` & `toomanycells-1.0.6/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.5/.github/workflows/macos.yml` & `toomanycells-1.0.6/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.5/.github/workflows/pypi.yml` & `toomanycells-1.0.6/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.5/.github/workflows/ubuntu.yml` & `toomanycells-1.0.6/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.5/.github/workflows/windows.yml` & `toomanycells-1.0.6/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.5/.gitignore` & `toomanycells-1.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.5/LICENSE` & `toomanycells-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.5/PKG-INFO` & `toomanycells-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toomanycells
-Version: 1.0.5
+Version: 1.0.6
 Summary: A python package for spectral clustering.
 Author-email: Javier Ruiz-Ramirez <javier.ruizramirez@uhn.ca>
 License: BSD License
 Project-URL: Homepage, https://github.com/JRR3/toomanycells
 Keywords: toomanycells
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `toomanycells-1.0.5/README.md` & `toomanycells-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.5/docs/contributing.md` & `toomanycells-1.0.6/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.5/docs/installation.md` & `toomanycells-1.0.6/docs/installation.md`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.5/mkdocs.yml` & `toomanycells-1.0.6/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.5/pyproject.toml` & `toomanycells-1.0.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "toomanycells"
-version = "1.0.5"
+version = "1.0.6"
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
-current_version = "1.0.5"
+current_version = "1.0.6"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

### Comparing `toomanycells-1.0.5/tests/benchmark.py` & `toomanycells-1.0.6/tests/benchmark.py`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.5/tests/benchmark_table.csv` & `toomanycells-1.0.6/tests/benchmark_table.csv`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.5/tests/benchmark_table_mod.csv` & `toomanycells-1.0.6/tests/benchmark_table_mod.csv`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.5/tests/example_1.png` & `toomanycells-1.0.6/tests/example_1.png`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.5/tests/log_benchmark_table.csv` & `toomanycells-1.0.6/tests/log_benchmark_table.csv`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.5/tests/log_linear_iter.png` & `toomanycells-1.0.6/tests/log_linear_iter.png`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.5/tests/log_linear_time.png` & `toomanycells-1.0.6/tests/log_linear_time.png`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.5/tests/plot_linear_model_for_iter.py` & `toomanycells-1.0.6/tests/plot_linear_model_for_iter.py`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.5/tests/plot_linear_model_for_time.py` & `toomanycells-1.0.6/tests/plot_linear_model_for_time.py`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.5/tests/tabula_sapiens_time.png` & `toomanycells-1.0.6/tests/tabula_sapiens_time.png`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.5/tests/tmci_tabula_sapiens.png` & `toomanycells-1.0.6/tests/tmci_tabula_sapiens.png`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.5/toomanycells/common.py` & `toomanycells-1.0.6/toomanycells/common.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 from typing import Union
+import pandas as pd
+import os
 #=====================================================
 class MultiIndexList(list):
     """
     This class is derived from the list class.\
         It allows the use of iterables to \
         access the list. For example: \
         L[(1,2,0)] will access item #1 \
@@ -28,7 +30,18 @@
             for index in indices:
                 obj = obj[index]
             return obj
         else:
             #Otherwise, just use the __getitem__ 
             #method of the parent class.
             return super().__getitem__(indices)
+
+def load_metadata_for_demo()-> pd.DataFrame:
+    """
+    This function loads the cell indices and \
+    labels for the demo file.
+    """
+    fname = os.path.dirname(__file__)
+    fname = os.path.join(fname, "data")
+    fname = os.path.join(fname, "metadata.csv")
+    df = pd.read_csv(fname)
+    return df
```

### Comparing `toomanycells-1.0.5/toomanycells/data/metadata.csv` & `toomanycells-1.0.6/toomanycells/data/metadata.csv`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.5/toomanycells/toomanycells.py` & `toomanycells-1.0.6/toomanycells/toomanycells.py`

 * *Files 1% similar despite different names*

```diff
@@ -697,12 +697,12 @@
         final_command = (f"(cd {path_to_tmc_interactive} "
                 f"&& {command})")
         #print(final_command)
         url = 'localhost:' + port_str
         txt = ("Once the app is running, just type in "
                 f"your browser \n        {url}")
         print(txt)
-        print("The app will start loading.")
+        print("The app will start loading after pressing Enter.")
         pause = input('Press Enter to continue ...')
         p = subprocess.call(final_command, shell=True)
 
     #====END=OF=CLASS=====================
```

### Comparing `toomanycells-1.0.5/toomanycells.egg-info/PKG-INFO` & `toomanycells-1.0.6/toomanycells.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toomanycells
-Version: 1.0.5
+Version: 1.0.6
 Summary: A python package for spectral clustering.
 Author-email: Javier Ruiz-Ramirez <javier.ruizramirez@uhn.ca>
 License: BSD License
 Project-URL: Homepage, https://github.com/JRR3/toomanycells
 Keywords: toomanycells
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `toomanycells-1.0.5/toomanycells.egg-info/SOURCES.txt` & `toomanycells-1.0.6/toomanycells.egg-info/SOURCES.txt`

 * *Files identical despite different names*

