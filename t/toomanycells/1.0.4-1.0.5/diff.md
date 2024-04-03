# Comparing `tmp/toomanycells-1.0.4.tar.gz` & `tmp/toomanycells-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toomanycells-1.0.4.tar", last modified: Wed Mar 20 01:46:54 2024, max compression
+gzip compressed data, was "toomanycells-1.0.5.tar", last modified: Wed Apr  3 20:03:35 2024, max compression
```

## Comparing `toomanycells-1.0.4.tar` & `toomanycells-1.0.5.tar`

### file list

```diff
@@ -1,63 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 01:46:54.047443 toomanycells-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-03-20 01:46:39.000000 toomanycells-1.0.4/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 01:46:54.031443 toomanycells-1.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 01:46:54.035443 toomanycells-1.0.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-03-20 01:46:39.000000 toomanycells-1.0.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-20 01:46:39.000000 toomanycells-1.0.4/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-03-20 01:46:39.000000 toomanycells-1.0.4/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 01:46:54.035443 toomanycells-1.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-03-20 01:46:39.000000 toomanycells-1.0.4/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-03-20 01:46:39.000000 toomanycells-1.0.4/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-20 01:46:39.000000 toomanycells-1.0.4/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-03-20 01:46:39.000000 toomanycells-1.0.4/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-03-20 01:46:39.000000 toomanycells-1.0.4/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-03-20 01:46:39.000000 toomanycells-1.0.4/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-03-20 01:46:39.000000 toomanycells-1.0.4/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-03-20 01:46:39.000000 toomanycells-1.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-03-20 01:46:39.000000 toomanycells-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-20 01:46:39.000000 toomanycells-1.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8588 2024-03-20 01:46:54.047443 toomanycells-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7546 2024-03-20 01:46:39.000000 toomanycells-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 01:46:54.039443 toomanycells-1.0.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-20 01:46:39.000000 toomanycells-1.0.4/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-20 01:46:39.000000 toomanycells-1.0.4/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-03-20 01:46:39.000000 toomanycells-1.0.4/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 01:46:54.039443 toomanycells-1.0.4/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-03-20 01:46:39.000000 toomanycells-1.0.4/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-20 01:46:39.000000 toomanycells-1.0.4/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-20 01:46:39.000000 toomanycells-1.0.4/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-03-20 01:46:39.000000 toomanycells-1.0.4/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 01:46:54.039443 toomanycells-1.0.4/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-20 01:46:39.000000 toomanycells-1.0.4/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-20 01:46:39.000000 toomanycells-1.0.4/docs/toomanycells.md
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-20 01:46:39.000000 toomanycells-1.0.4/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-03-20 01:46:39.000000 toomanycells-1.0.4/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-03-20 01:46:39.000000 toomanycells-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-20 01:46:39.000000 toomanycells-1.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-03-20 01:46:39.000000 toomanycells-1.0.4/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 01:46:54.047443 toomanycells-1.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 01:46:54.043443 toomanycells-1.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-20 01:46:39.000000 toomanycells-1.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-03-20 01:46:39.000000 toomanycells-1.0.4/tests/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-03-20 01:46:39.000000 toomanycells-1.0.4/tests/benchmark_table.csv
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-03-20 01:46:39.000000 toomanycells-1.0.4/tests/benchmark_table_mod.csv
--rw-r--r--   0 runner    (1001) docker     (127)   803420 2024-03-20 01:46:39.000000 toomanycells-1.0.4/tests/example_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-03-20 01:46:39.000000 toomanycells-1.0.4/tests/log_benchmark_table.csv
--rw-r--r--   0 runner    (1001) docker     (127)   169679 2024-03-20 01:46:39.000000 toomanycells-1.0.4/tests/log_linear_iter.png
--rw-r--r--   0 runner    (1001) docker     (127)   171516 2024-03-20 01:46:39.000000 toomanycells-1.0.4/tests/log_linear_time.png
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-03-20 01:46:39.000000 toomanycells-1.0.4/tests/plot_linear_model_for_iter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-03-20 01:46:39.000000 toomanycells-1.0.4/tests/plot_linear_model_for_time.py
--rw-r--r--   0 runner    (1001) docker     (127)    36791 2024-03-20 01:46:39.000000 toomanycells-1.0.4/tests/tabula_sapiens_time.png
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-03-20 01:46:39.000000 toomanycells-1.0.4/tests/test_toomanycells.py
--rw-r--r--   0 runner    (1001) docker     (127)  2027414 2024-03-20 01:46:39.000000 toomanycells-1.0.4/tests/tmci_tabula_sapiens.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 01:46:54.043443 toomanycells-1.0.4/toomanycells/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-20 01:46:39.000000 toomanycells-1.0.4/toomanycells/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-03-20 01:46:39.000000 toomanycells-1.0.4/toomanycells/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    23397 2024-03-20 01:46:39.000000 toomanycells-1.0.4/toomanycells/toomanycells.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 01:46:54.047443 toomanycells-1.0.4/toomanycells.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8588 2024-03-20 01:46:53.000000 toomanycells-1.0.4/toomanycells.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-03-20 01:46:54.000000 toomanycells-1.0.4/toomanycells.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 01:46:53.000000 toomanycells-1.0.4/toomanycells.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-20 01:46:53.000000 toomanycells-1.0.4/toomanycells.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-20 01:46:53.000000 toomanycells-1.0.4/toomanycells.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-20 01:46:53.000000 toomanycells-1.0.4/toomanycells.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:03:35.934231 toomanycells-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-03 20:03:25.000000 toomanycells-1.0.5/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:03:35.918231 toomanycells-1.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:03:35.922231 toomanycells-1.0.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-03 20:03:25.000000 toomanycells-1.0.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-03 20:03:25.000000 toomanycells-1.0.5/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-03 20:03:25.000000 toomanycells-1.0.5/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:03:35.922231 toomanycells-1.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-03 20:03:25.000000 toomanycells-1.0.5/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-03 20:03:25.000000 toomanycells-1.0.5/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-03 20:03:25.000000 toomanycells-1.0.5/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-03 20:03:25.000000 toomanycells-1.0.5/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-03 20:03:25.000000 toomanycells-1.0.5/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-03 20:03:25.000000 toomanycells-1.0.5/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-03 20:03:25.000000 toomanycells-1.0.5/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-03 20:03:25.000000 toomanycells-1.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-03 20:03:25.000000 toomanycells-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-03 20:03:25.000000 toomanycells-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8589 2024-04-03 20:03:35.934231 toomanycells-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7546 2024-04-03 20:03:25.000000 toomanycells-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:03:35.926231 toomanycells-1.0.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-03 20:03:25.000000 toomanycells-1.0.5/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-03 20:03:25.000000 toomanycells-1.0.5/docs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-03 20:03:25.000000 toomanycells-1.0.5/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:03:35.926231 toomanycells-1.0.5/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-03 20:03:25.000000 toomanycells-1.0.5/docs/examples/intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-03 20:03:25.000000 toomanycells-1.0.5/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-03 20:03:25.000000 toomanycells-1.0.5/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-03 20:03:25.000000 toomanycells-1.0.5/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:03:35.926231 toomanycells-1.0.5/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-03 20:03:25.000000 toomanycells-1.0.5/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-03 20:03:25.000000 toomanycells-1.0.5/docs/toomanycells.md
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-03 20:03:25.000000 toomanycells-1.0.5/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-03 20:03:25.000000 toomanycells-1.0.5/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-03 20:03:25.000000 toomanycells-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 20:03:25.000000 toomanycells-1.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-03 20:03:25.000000 toomanycells-1.0.5/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 20:03:35.934231 toomanycells-1.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:03:35.926231 toomanycells-1.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-03 20:03:25.000000 toomanycells-1.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-03 20:03:25.000000 toomanycells-1.0.5/tests/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-03 20:03:25.000000 toomanycells-1.0.5/tests/benchmark_table.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-03 20:03:25.000000 toomanycells-1.0.5/tests/benchmark_table_mod.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   803420 2024-04-03 20:03:25.000000 toomanycells-1.0.5/tests/example_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-03 20:03:25.000000 toomanycells-1.0.5/tests/log_benchmark_table.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   169679 2024-04-03 20:03:25.000000 toomanycells-1.0.5/tests/log_linear_iter.png
+-rw-r--r--   0 runner    (1001) docker     (127)   171516 2024-04-03 20:03:25.000000 toomanycells-1.0.5/tests/log_linear_time.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-03 20:03:25.000000 toomanycells-1.0.5/tests/plot_linear_model_for_iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-03 20:03:25.000000 toomanycells-1.0.5/tests/plot_linear_model_for_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36791 2024-04-03 20:03:25.000000 toomanycells-1.0.5/tests/tabula_sapiens_time.png
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-03 20:03:25.000000 toomanycells-1.0.5/tests/test_toomanycells.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2027414 2024-04-03 20:03:25.000000 toomanycells-1.0.5/tests/tmci_tabula_sapiens.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:03:35.930231 toomanycells-1.0.5/toomanycells/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-03 20:03:25.000000 toomanycells-1.0.5/toomanycells/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-03 20:03:25.000000 toomanycells-1.0.5/toomanycells/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:03:35.930231 toomanycells-1.0.5/toomanycells/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    50239 2024-04-03 20:03:25.000000 toomanycells-1.0.5/toomanycells/data/metadata.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    23390 2024-04-03 20:03:25.000000 toomanycells-1.0.5/toomanycells/toomanycells.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:03:35.934231 toomanycells-1.0.5/toomanycells.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8589 2024-04-03 20:03:35.000000 toomanycells-1.0.5/toomanycells.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-03 20:03:35.000000 toomanycells-1.0.5/toomanycells.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 20:03:35.000000 toomanycells-1.0.5/toomanycells.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-03 20:03:35.000000 toomanycells-1.0.5/toomanycells.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-03 20:03:35.000000 toomanycells-1.0.5/toomanycells.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 20:03:35.000000 toomanycells-1.0.5/toomanycells.egg-info/top_level.txt
```

### Comparing `toomanycells-1.0.4/.github/ISSUE_TEMPLATE/bug_report.md` & `toomanycells-1.0.5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.4/.github/workflows/docs-build.yml` & `toomanycells-1.0.5/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.4/.github/workflows/docs.yml` & `toomanycells-1.0.5/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.4/.github/workflows/installation.yml` & `toomanycells-1.0.5/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.4/.github/workflows/macos.yml` & `toomanycells-1.0.5/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.4/.github/workflows/pypi.yml` & `toomanycells-1.0.5/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.4/.github/workflows/ubuntu.yml` & `toomanycells-1.0.5/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.4/.github/workflows/windows.yml` & `toomanycells-1.0.5/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.4/.gitignore` & `toomanycells-1.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.4/LICENSE` & `toomanycells-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.4/PKG-INFO` & `toomanycells-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toomanycells
-Version: 1.0.4
+Version: 1.0.5
 Summary: A python package for spectral clustering.
 Author-email: Javier Ruiz-Ramirez <javier.ruizramirez@uhn.ca>
 License: BSD License
 Project-URL: Homepage, https://github.com/JRR3/toomanycells
 Keywords: toomanycells
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: scanpy
+Requires-Dist: anndata
 Requires-Dist: scipy
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: networkx
 Requires-Dist: tqdm
 Requires-Dist: scikit-learn
 Provides-Extra: all
```

### Comparing `toomanycells-1.0.4/README.md` & `toomanycells-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.4/docs/contributing.md` & `toomanycells-1.0.5/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.4/docs/installation.md` & `toomanycells-1.0.5/docs/installation.md`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.4/mkdocs.yml` & `toomanycells-1.0.5/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.4/pyproject.toml` & `toomanycells-1.0.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "toomanycells"
-version = "1.0.4"
+version = "1.0.5"
 dynamic = [
     "dependencies",
 ]
 description = "A python package for spectral clustering."
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -39,24 +39,27 @@
 
 
 [tool]
 [tool.setuptools.packages.find]
 include = ["toomanycells*"]
 exclude = ["docs*"]
 
+[tool.setuptools.package-data]
+"toomanycells.data" = ["*.csv"]
+
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "1.0.4"
+current_version = "1.0.5"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

### Comparing `toomanycells-1.0.4/tests/benchmark.py` & `toomanycells-1.0.5/tests/benchmark.py`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.4/tests/benchmark_table.csv` & `toomanycells-1.0.5/tests/benchmark_table.csv`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.4/tests/benchmark_table_mod.csv` & `toomanycells-1.0.5/tests/benchmark_table_mod.csv`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.4/tests/example_1.png` & `toomanycells-1.0.5/tests/example_1.png`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.4/tests/log_benchmark_table.csv` & `toomanycells-1.0.5/tests/log_benchmark_table.csv`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.4/tests/log_linear_iter.png` & `toomanycells-1.0.5/tests/log_linear_iter.png`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.4/tests/log_linear_time.png` & `toomanycells-1.0.5/tests/log_linear_time.png`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.4/tests/plot_linear_model_for_iter.py` & `toomanycells-1.0.5/tests/plot_linear_model_for_iter.py`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.4/tests/plot_linear_model_for_time.py` & `toomanycells-1.0.5/tests/plot_linear_model_for_time.py`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.4/tests/tabula_sapiens_time.png` & `toomanycells-1.0.5/tests/tabula_sapiens_time.png`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.4/tests/tmci_tabula_sapiens.png` & `toomanycells-1.0.5/tests/tmci_tabula_sapiens.png`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.4/toomanycells/common.py` & `toomanycells-1.0.5/toomanycells/common.py`

 * *Files identical despite different names*

### Comparing `toomanycells-1.0.4/toomanycells/toomanycells.py` & `toomanycells-1.0.5/toomanycells/toomanycells.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 #########################################################
 from typing import Optional
 from typing import Union
 import networkx as nx
 from scipy import sparse as sp
 from scipy.io import mmread
 from time import perf_counter as clock
-import scanpy as sc
-from scanpy import AnnData
+import anndata as ad
+from anndata import AnnData
 import numpy as np
 import pandas as pd
 import re
 from sklearn.decomposition import TruncatedSVD
 from collections import deque
 import os
 from os.path import dirname
@@ -86,43 +86,45 @@
         :rtype: :obj:`TooManyCells`
 
         """
 
         if isinstance(input, str):
             if input.endswith('.h5ad'):
                 self.t0 = clock()
-                self.A = sc.read_h5ad(input)
+                self.A = ad.read_h5ad(input)
                 self.tf = clock()
                 delta = self.tf - self.t0
                 txt = ('Elapsed time for loading: ' +
                         f'{delta:.2f} seconds.')
                 print(txt)
             else:
                 self.source = input
                 if input_is_matrix_market:
                     self.convert_mm_from_source_to_anndata()
                 else:
                     for f in os.listdir(input):
                         if f.endswith('.h5ad'):
                             fname = os.path.join(input, f)
                             self.t0 = clock()
-                            self.A = sc.read_h5ad(fname)
+                            self.A = ad.read_h5ad(fname)
                             self.tf = clock()
                             delta = self.tf - self.t0
                             txt = ('Elapsed time for ' +
                                    'loading: ' +
                                     f'{delta:.2f} seconds.')
                             print(txt)
                             break
 
         elif isinstance(input, AnnData):
             self.A = input
         else:
             raise ValueError('Unexpected input type.')
 
+        #If no output directory is provided,
+        #we use the current working directory.
         if output == "":
             output = os.getcwd()
 
         if not os.path.exists(output):
             os.makedirs(output)
 
         #This column of the obs data frame indicates
@@ -138,16 +140,19 @@
         self.path_column_index = t
 
         self.delta_clustering = 0
         self.final_n_iter     = 0
 
 
         #Create a copy to avoid direct modifications
-        #to the original count matrix X.
-        self.X = self.A.X.copy()
+        #of the original count matrix X.
+        #Note that we are making sure that the 
+        #sparse matrix has the CSR format. This
+        #is relevant when we normalize.
+        self.X = sp.csr_matrix(self.A.X, copy=True)
 
         self.n_cells, self.n_genes = self.A.shape
 
         if self.n_cells < 2:
             raise ValueError("Too few observations (cells).")
 
         print(self.A)
@@ -697,17 +702,7 @@
                 f"your browser \n        {url}")
         print(txt)
         print("The app will start loading.")
         pause = input('Press Enter to continue ...')
         p = subprocess.call(final_command, shell=True)
 
     #====END=OF=CLASS=====================
-
-#Typical usage:
-#import toomanycells as tmc
-#obj = tmc.TooManyCells(path_to_source, path_to_output)
-#obj.run_spectral_clustering()
-#obj.store_outputs()
-#obj.visualize_with_tmc_interactive(
-#path_to_tmc_interactive,
-#column_containing_cell_annotations,
-#)
```

### Comparing `toomanycells-1.0.4/toomanycells.egg-info/PKG-INFO` & `toomanycells-1.0.5/toomanycells.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toomanycells
-Version: 1.0.4
+Version: 1.0.5
 Summary: A python package for spectral clustering.
 Author-email: Javier Ruiz-Ramirez <javier.ruizramirez@uhn.ca>
 License: BSD License
 Project-URL: Homepage, https://github.com/JRR3/toomanycells
 Keywords: toomanycells
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: scanpy
+Requires-Dist: anndata
 Requires-Dist: scipy
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: networkx
 Requires-Dist: tqdm
 Requires-Dist: scikit-learn
 Provides-Extra: all
```

### Comparing `toomanycells-1.0.4/toomanycells.egg-info/SOURCES.txt` & `toomanycells-1.0.5/toomanycells.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -44,8 +44,9 @@
 toomanycells/common.py
 toomanycells/toomanycells.py
 toomanycells.egg-info/PKG-INFO
 toomanycells.egg-info/SOURCES.txt
 toomanycells.egg-info/dependency_links.txt
 toomanycells.egg-info/entry_points.txt
 toomanycells.egg-info/requires.txt
-toomanycells.egg-info/top_level.txt
+toomanycells.egg-info/top_level.txt
+toomanycells/data/metadata.csv
```

