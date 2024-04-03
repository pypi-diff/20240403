# Comparing `tmp/postbp-0.1.1.tar.gz` & `tmp/postbp-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postbp-0.1.1.tar", last modified: Sun Mar 31 03:22:21 2024, max compression
+gzip compressed data, was "postbp-0.1.2.tar", last modified: Wed Apr  3 12:56:02 2024, max compression
```

## Comparing `postbp-0.1.1.tar` & `postbp-0.1.2.tar`

### file list

```diff
@@ -1,63 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 03:22:21.208969 postbp-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-03-31 03:22:10.000000 postbp-0.1.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 03:22:21.200969 postbp-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 03:22:21.200969 postbp-0.1.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-03-31 03:22:10.000000 postbp-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-03-31 03:22:10.000000 postbp-0.1.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-03-31 03:22:10.000000 postbp-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 03:22:21.204970 postbp-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-03-31 03:22:10.000000 postbp-0.1.1/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-03-31 03:22:10.000000 postbp-0.1.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-03-31 03:22:10.000000 postbp-0.1.1/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-03-31 03:22:10.000000 postbp-0.1.1/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-03-31 03:22:10.000000 postbp-0.1.1/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-03-31 03:22:10.000000 postbp-0.1.1/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-03-31 03:22:10.000000 postbp-0.1.1/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-03-31 03:22:10.000000 postbp-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-31 03:22:10.000000 postbp-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-31 03:22:10.000000 postbp-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-03-31 03:22:21.208969 postbp-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-03-31 03:22:10.000000 postbp-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 03:22:21.204970 postbp-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-31 03:22:10.000000 postbp-0.1.1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-31 03:22:10.000000 postbp-0.1.1/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-03-31 03:22:10.000000 postbp-0.1.1/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-31 03:22:10.000000 postbp-0.1.1/docs/dailyfirevectors.md
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-31 03:22:10.000000 postbp-0.1.1/docs/dataloader.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 03:22:21.204970 postbp-0.1.1/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-03-31 03:22:10.000000 postbp-0.1.1/docs/examples/dataexamples.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-03-31 03:22:10.000000 postbp-0.1.1/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-31 03:22:10.000000 postbp-0.1.1/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-31 03:22:10.000000 postbp-0.1.1/docs/finalfirevectors.md
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-03-31 03:22:10.000000 postbp-0.1.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-03-31 03:22:10.000000 postbp-0.1.1/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 03:22:21.204970 postbp-0.1.1/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-31 03:22:10.000000 postbp-0.1.1/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-31 03:22:10.000000 postbp-0.1.1/docs/postbp.md
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-31 03:22:10.000000 postbp-0.1.1/docs/spreadrose.md
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-31 03:22:10.000000 postbp-0.1.1/docs/tessellation.md
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-31 03:22:10.000000 postbp-0.1.1/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-03-31 03:22:10.000000 postbp-0.1.1/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 03:22:21.204970 postbp-0.1.1/postbp/
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-03-31 03:22:10.000000 postbp-0.1.1/postbp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-03-31 03:22:10.000000 postbp-0.1.1/postbp/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     6748 2024-03-31 03:22:10.000000 postbp-0.1.1/postbp/dailyfirevectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-03-31 03:22:10.000000 postbp-0.1.1/postbp/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5576 2024-03-31 03:22:10.000000 postbp-0.1.1/postbp/finalfirevectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-03-31 03:22:10.000000 postbp-0.1.1/postbp/postbp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-03-31 03:22:10.000000 postbp-0.1.1/postbp/spreadrose.py
--rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-03-31 03:22:10.000000 postbp-0.1.1/postbp/tessellation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 03:22:21.208969 postbp-0.1.1/postbp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-03-31 03:22:21.000000 postbp-0.1.1/postbp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-03-31 03:22:21.000000 postbp-0.1.1/postbp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 03:22:21.000000 postbp-0.1.1/postbp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-31 03:22:21.000000 postbp-0.1.1/postbp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-31 03:22:21.000000 postbp-0.1.1/postbp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-31 03:22:21.000000 postbp-0.1.1/postbp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-03-31 03:22:10.000000 postbp-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-31 03:22:10.000000 postbp-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-03-31 03:22:10.000000 postbp-0.1.1/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 03:22:21.208969 postbp-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 03:22:21.208969 postbp-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-31 03:22:10.000000 postbp-0.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-31 03:22:10.000000 postbp-0.1.1/tests/test_postbp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:56:02.549768 postbp-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-03 12:55:50.000000 postbp-0.1.2/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:56:02.537768 postbp-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:56:02.541768 postbp-0.1.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-03 12:55:50.000000 postbp-0.1.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-03 12:55:50.000000 postbp-0.1.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-03 12:55:50.000000 postbp-0.1.2/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:56:02.541768 postbp-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-03 12:55:50.000000 postbp-0.1.2/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-03 12:55:50.000000 postbp-0.1.2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-03 12:55:50.000000 postbp-0.1.2/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-03 12:55:50.000000 postbp-0.1.2/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-03 12:55:50.000000 postbp-0.1.2/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-03 12:55:50.000000 postbp-0.1.2/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-03 12:55:50.000000 postbp-0.1.2/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-03 12:55:50.000000 postbp-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-03 12:55:50.000000 postbp-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-03 12:55:50.000000 postbp-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-03 12:56:02.549768 postbp-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-03 12:55:50.000000 postbp-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:56:02.545768 postbp-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-03 12:55:50.000000 postbp-0.1.2/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-03 12:55:50.000000 postbp-0.1.2/docs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-03 12:55:50.000000 postbp-0.1.2/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-03 12:55:50.000000 postbp-0.1.2/docs/dailyfirevectors.md
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-03 12:55:50.000000 postbp-0.1.2/docs/dataloader.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:56:02.545768 postbp-0.1.2/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-03 12:55:50.000000 postbp-0.1.2/docs/examples/intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-03 12:55:50.000000 postbp-0.1.2/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-03 12:55:50.000000 postbp-0.1.2/docs/finalfirevectors.md
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-03 12:55:50.000000 postbp-0.1.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-03 12:55:50.000000 postbp-0.1.2/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:56:02.545768 postbp-0.1.2/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-03 12:55:50.000000 postbp-0.1.2/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-03 12:55:50.000000 postbp-0.1.2/docs/postbp.md
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-03 12:55:50.000000 postbp-0.1.2/docs/spreadrose.md
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-03 12:55:50.000000 postbp-0.1.2/docs/tessellation.md
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-03 12:55:50.000000 postbp-0.1.2/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-03 12:55:50.000000 postbp-0.1.2/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:56:02.545768 postbp-0.1.2/postbp/
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-03 12:55:50.000000 postbp-0.1.2/postbp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-03 12:55:50.000000 postbp-0.1.2/postbp/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-04-03 12:55:50.000000 postbp-0.1.2/postbp/dailyfirevectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-03 12:55:50.000000 postbp-0.1.2/postbp/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5646 2024-04-03 12:55:50.000000 postbp-0.1.2/postbp/finalfirevectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5785 2024-04-03 12:55:50.000000 postbp-0.1.2/postbp/postbp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-03 12:55:50.000000 postbp-0.1.2/postbp/spreadrose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-04-03 12:55:50.000000 postbp-0.1.2/postbp/tessellation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:56:02.549768 postbp-0.1.2/postbp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-03 12:56:02.000000 postbp-0.1.2/postbp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-03 12:56:02.000000 postbp-0.1.2/postbp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 12:56:02.000000 postbp-0.1.2/postbp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-03 12:56:02.000000 postbp-0.1.2/postbp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-03 12:56:02.000000 postbp-0.1.2/postbp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 12:56:02.000000 postbp-0.1.2/postbp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-03 12:55:50.000000 postbp-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-03 12:55:50.000000 postbp-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-03 12:55:50.000000 postbp-0.1.2/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 12:56:02.549768 postbp-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:56:02.549768 postbp-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-03 12:55:50.000000 postbp-0.1.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-03 12:55:50.000000 postbp-0.1.2/tests/test_postbp.py
```

### Comparing `postbp-0.1.1/.github/workflows/docs-build.yml` & `postbp-0.1.2/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `postbp-0.1.1/.github/workflows/docs.yml` & `postbp-0.1.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `postbp-0.1.1/.github/workflows/installation.yml` & `postbp-0.1.2/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `postbp-0.1.1/.github/workflows/macos.yml` & `postbp-0.1.2/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `postbp-0.1.1/.github/workflows/pypi.yml` & `postbp-0.1.2/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `postbp-0.1.1/.github/workflows/ubuntu.yml` & `postbp-0.1.2/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `postbp-0.1.1/.github/workflows/windows.yml` & `postbp-0.1.2/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `postbp-0.1.1/.gitignore` & `postbp-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `postbp-0.1.1/LICENSE` & `postbp-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `postbp-0.1.1/PKG-INFO` & `postbp-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postbp
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python Library
 Author-email: Ning Liu <ning.liu@nrcan-rncan.gc.ca>
 License: MIT License
 Project-URL: Homepage, https://github.com/nliu-cfs/postbp
 Keywords: postbp
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -19,14 +19,15 @@
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: geopandas
 Requires-Dist: shapely
 Requires-Dist: windrose
 Requires-Dist: matplotlib
+Requires-Dist: tqdm
 Provides-Extra: all
 Requires-Dist: postbp[extra]; extra == "all"
 Provides-Extra: extra
 Requires-Dist: pandas; extra == "extra"
 
 # postbp
```

### Comparing `postbp-0.1.1/docs/contributing.md` & `postbp-0.1.2/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `postbp-0.1.1/docs/examples/intro.ipynb` & `postbp-0.1.2/docs/examples/intro.ipynb`

 * *Files identical despite different names*

### Comparing `postbp-0.1.1/mkdocs.yml` & `postbp-0.1.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `postbp-0.1.1/postbp/__init__.py` & `postbp-0.1.2/postbp/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """Top-level package for postbp."""
 
 __author__ = """Ning Liu"""
 __email__ = "ning.liu@nrcan-rncan.gc.ca"
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 
 from .common import (
     prj2hex,  #noqa
     pij_to_shp, #noqa
 )
 from .dataloader import(
     read_fireshp,  #noqa
     read_pointcsv,   #noqa
     read_pointshp,   #noqa
 ) 
 
 from .postbp import (
     generate_ign_prob,  #noqa
     generate_burn_prob,  #noqa
-    generate_SSR,  #noqa
+    generate_ssr,  #noqa
     generate_fireshed,   #noqa
     generate_fireplain,  #noqa
 )
 
 from .spreadrose import (
     generate_fire_rose,  #noqa
     plot_rose,   #noqa
@@ -30,9 +30,16 @@
 from .tessellation import (
     create_hexagons_nodes,  #noqa
     create_arcs,  #noqa
     nodes_from_hexagons,  #noqa
     create_hexagons,   #noqa
 )
 
-from .finalfirevectors import *    #noqa
-from .dailyfirevectors import *    #noqa
+from .finalfirevectors import (
+    generate_fire_vectors,    #noqa
+    pij_from_vectors,      #noqa
+)
+from .dailyfirevectors import (
+    generate_daily_vectors,    #noqa
+    calc_angles,        #noqa
+    select_angle,       #noqa
+)
```

### Comparing `postbp-0.1.1/postbp/common.py` & `postbp-0.1.2/postbp/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,17 +30,17 @@
         nodes (_type_): _description_
 
     Returns:
         _type_: _description_
     """    
     
     pij = pij_input.copy()
-
+    node = nodes.copy()
     if 'Node_ID' in kwargs:
-        node = nodes.rename(columns={kwargs["Node_ID"]: 'Node_ID'})
+        node = node.rename(columns={kwargs["Node_ID"]: 'Node_ID'})
     if 'column_i' in kwargs:
         pij.rename(columns={kwargs["column_i"]: 'column_i'}, inplace=True)    
     if 'column_j' in kwargs:
         pij.rename(columns={kwargs["column_j"]: 'column_j'}, inplace=True)           
 
     SRID = node.crs
     pij = node.merge(pij, left_on='Node_ID', right_on='column_i', how='right')
```

### Comparing `postbp-0.1.1/postbp/dailyfirevectors.py` & `postbp-0.1.2/postbp/dailyfirevectors.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import numpy as np
 import pandas as pd
 import itertools
 from math import atan2, degrees
 from .common import prj2hex
 import warnings
 warnings.filterwarnings("ignore")
+import tqdm
 
 def angle(record):
     """Calculate angle from three points: ignition point and the points where fire spread from and to.  
 
     Args:
         record (_type_): _description_
 
@@ -39,25 +40,25 @@
         hexagons (_type_): _description_
         bufferFactor (int, optional): convert ignition point into a circle polygon of the diameter of bufferFactor
 it shall be small enough so as not to have ignition point locates in more than one hexagons it also defines threshold for the minimum area of fire perimeter to be in a hexagon to be regarded as burned. Defaults to 10.
 
     Returns:
         _type_: _description_
     """    
-    
+    hexagon = hexagons.copy()
     if 'Node_ID' in kwargs:
-        hexagon = hexagons.rename(columns={kwargs["Node_ID"]: 'Node_ID'})
-
+        hexagon = hexagon.rename(columns={kwargs["Node_ID"]: 'Node_ID'})
+    
     threshold = 3.1415926*bufferFactor**2 - 1 
     SRID = fireshp.crs
     df = pd.DataFrame()
     dfMore = pd.DataFrame()
     errorlog = []
     
-    for i in np.unique(fireshp['fire']):
+    for i in tqdm(np.unique(fireshp['fire'])):
         try: 
             fire_i = fireshp.loc[fireshp['fire'] == i]
             pts_i = ignition.loc[ignition['fire'] == i]
             pts_ni = gpd.sjoin(pts_i, hexagon, how = 'inner', op = 'within')
             ##### ignition point to all hexes
             dmax = max(fire_i['day'])
             fire_idmax = fire_i.loc[fire_i['day'] == dmax]
@@ -113,27 +114,27 @@
     Args:
         vectors (_type_): _description_
         nodes (_type_): _description_
 
     Returns:
         _type_: _description_
     """    
-
+    node = nodes.copy()
     if 'Node_ID' in kwargs:
-        node = nodes.rename(columns={kwargs["Node_ID"]: 'Node_ID'})
+        node = node.rename(columns={kwargs["Node_ID"]: 'Node_ID'})
 
     vectorsW = vectors.copy()
     vectorsW = node.merge(vectors, left_on='Node_ID', right_on='column_i', how='right')
     vectorsW = vectorsW.merge(node, left_on='column_j', right_on='Node_ID', how='left')
     vectorsW = vectorsW.merge(node, left_on='ignPt', right_on='Node_ID', how='left')
     vectorsW.drop(labels = ['Node_ID_x', 'Node_ID_y', 'Node_ID'], axis = 1, inplace = True)
 
     #### note that 'geometry_x':origin; 'geometry_y':destination; 'geometry':ignition
 
-    for index, row in vectorsW.iterrows():
+    for index, row in tqdm(vectorsW.iterrows()):
         try: 
             vectorsW.at[index, 'angle'] = angle(row)
         except:
             vectorsW.at[index, 'angle'] = 181  # when origin is identical to ignition
     vectorsW.loc[vectorsW['day'] == 999, 'angle'] = 361  # from ignition to all hexes in perimeter
     vectorsW.loc[vectorsW['day'] == 1, 'angle'] = 181  # in day 1: origin is identical to ignition
     vectorsW.drop_duplicates(subset = ['day', 'column_j', 'fire', 'ignPt', 'column_i'], keep = 'first', inplace = True)
```

### Comparing `postbp-0.1.1/postbp/dataloader.py` & `postbp-0.1.2/postbp/dataloader.py`

 * *Files identical despite different names*

### Comparing `postbp-0.1.1/postbp/finalfirevectors.py` & `postbp-0.1.2/postbp/finalfirevectors.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import geopandas as gpd
 import pandas as pd
 from .common import prj2hex
 import warnings
 warnings.filterwarnings("ignore")
 from shapely.errors import ShapelyDeprecationWarning
 warnings.filterwarnings("ignore", category=ShapelyDeprecationWarning)
+import tqdm
 
 def spatial_join(fireshp, ignition, hexagon, threshold=0, iteration=False):
     """_summary_
 
     Args:
         fireshp (_type_): _description_
         ignition (_type_): _description_
@@ -33,15 +34,15 @@
     ignition = ignition.to_crs(fireshp.crs)
     hexagon = hexagon.to_crs(fireshp.crs)
 
     fire_vectors = pd.DataFrame()
     errorlog = []
 
     if not iteration:
-        for i in fireshp['fire']:
+        for i in tqdm(fireshp['fire']):
             try:
                 fire_i = fireshp.loc[fireshp['fire'] == i]
                 fire_ni = prj2hex(fire_i, hexagon, threshold)                        
                 pts_i = ignition.loc[ignition['fire'] == i]
                 #if newer version op is replace by predicate
                 pts_ni = gpd.sjoin(pts_i, hexagon, how = 'inner', op = 'within')
                 pts_ni = pts_ni[['fire', 'Node_ID']]
@@ -56,15 +57,15 @@
         # output errorlog to a txt
         with open("errorlog_finalfire.txt", "w+") as f:
             f.write(errorlog)
         return fire_vectors
 
 
     if iteration:
-        for j in set(fireshp['iteration']):
+        for j in tqdm(set(fireshp['iteration'])):
             fire_j = fireshp.loc[fireshp['iteration'] == j]
             pts_j = ignition.loc[ignition['iteration'] == j]
             
             for i in fireshp['fire']:
                 try:
                     fire_i = fire_j.loc[fire_j['fire'] == i]
                     fire_ni = prj2hex(fire_i, hexagon, threshold)                             
@@ -94,46 +95,46 @@
         hexagons (_type_): _description_
         threshold (int, optional): _description_. Defaults to 0.
         loopBy (str, optional): _description_. Defaults to "fire".
 
     Returns:
         _type_: _description_
     """    
-
+    hexagon = hexagons.copy()
     if 'Node_ID' in kwargs:
-        hexagon = hexagons.rename(columns={kwargs["Node_ID"]: 'Node_ID'})
+        hexagon = hexagon.rename(columns={kwargs["Node_ID"]: 'Node_ID'})
     
     if loopBy == "iteration":
         fire_vectors = spatial_join(fireshp, ignition, hexagon, threshold, iteration=True)
     
     if loopBy == "fire":
         fire_vectors = spatial_join(fireshp, ignition, hexagon, threshold, iteration=False)
      
     fire_vectors = fire_vectors.reset_index(drop = True)
     fire_vectors.drop(fire_vectors[fire_vectors['Node_ID_y'].isna()].index, inplace = True)                    
     
     fire_vectors['Node_ID_x'] = fire_vectors['Node_ID_x'].astype(int)
     fire_vectors['Node_ID_y'] = fire_vectors['Node_ID_y'].astype(int)
     
     fire_vectors.columns = ['Node_ID_x', 'Node_ID_y', 'fire', 'iteration']
-    fire_vectors.rename(columns={'Node_ID_x':'desti', 'Node_ID_y':'origi'}, inplace=True)
+    fire_vectors.rename(columns={'Node_ID_x':'column_j', 'Node_ID_y':'column_i'}, inplace=True)
     return fire_vectors
 
 def pij_from_vectors(vectors, iterations):
     """_summary_
 
     Args:
         vectors (_type_): _description_
         iterations (_type_): _description_
 
     Returns:
         _type_: _description_
     """    
 
-    fire_pij = vectors.groupby(['desti', 'origi'])[['fire']].count()
+    fire_pij = vectors.groupby(['column_j', 'column_i'])[['fire']].count()
     fire_pij.reset_index(inplace = True)
-    fire_pij = fire_pij.drop(fire_pij[fire_pij['desti'] == fire_pij['origi']].index)
+    fire_pij = fire_pij.drop(fire_pij[fire_pij['column_j'] == fire_pij['column_i']].index)
     fire_pij['pij'] = fire_pij['fire'] / iterations
     fire_pij['pij'] = fire_pij['pij'].round(5)
     fire_pij['pij'] = fire_pij['pij'].apply(lambda x: '%.5f' % x)
     
     return fire_pij
```

### Comparing `postbp-0.1.1/postbp/postbp.py` & `postbp-0.1.2/postbp/postbp.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,17 +12,17 @@
         fireshp (_type_): _description_
         hexagons (_type_): _description_
         iterations (_type_): _description_
 
     Returns:
         _type_: _description_
     """    
-
+    hexagon = hexagons.copy()
     if 'Node_ID' in kwargs:
-        hexagon = hexagons.rename(columns={kwargs["Node_ID"]: 'Node_ID'})
+        hexagon = hexagon.rename(columns={kwargs["Node_ID"]: 'Node_ID'})
 
     fireOL = prj2hex(fireshp, hexagon, threshold=0)
     if 'fire_column' in kwargs:
         fireOL.rename(columns={kwargs["fire_column"]: 'fire'}, inplace=True) 
        
     burned = fireOL.groupby('Node_ID')[['fire']].count()
     burned.reset_index(inplace=True)
@@ -42,16 +42,17 @@
         iterations (_type_): _description_
 
     Returns:
         _type_: _description_
     """    
 
     ign = ignition.copy()
+    hexagon = hexagons.copy()
     if 'Node_ID' in kwargs:
-        hexagon = hexagons.rename(columns={kwargs["Node_ID"]: 'Node_ID'})
+        hexagon = hexagon.rename(columns={kwargs["Node_ID"]: 'Node_ID'})
     if 'fire_column' in kwargs:
         ign.rename(columns={kwargs["fire_column"]: 'fire'}, inplace=True)    
 
     ignSJ = gpd.sjoin(ign, hexagon, how = 'inner', op = 'within')
     ignGr = ignSJ.groupby(['Node_ID'])[['fire']].count()
     ignGr = hexagon.merge(ignGr, on='Node_ID', how='right')
     ignGr.fillna(0, inplace=True)
@@ -67,17 +68,17 @@
         AOCshp (_type_): _description_
         fireshp (_type_): _description_
         hexagons (_type_): _description_
 
     Returns:
         _type_: _description_
     """    
-
+    hexagon = hexagons.copy()
     if 'Node_ID' in kwargs:
-        hexagon = hexagons.rename(columns={kwargs["Node_ID"]: 'Node_ID'})
+        hexagon = hexagon.rename(columns={kwargs["Node_ID"]: 'Node_ID'})
     fv = fire_vectors.copy()
     if 'column_i' in kwargs:
         fv.rename(columns={kwargs["column_i"]: 'column_i'}, inplace=True)    
     if 'column_j' in kwargs:
         fv.rename(columns={kwargs["column_j"]: 'column_j'}, inplace=True)
     if 'fire_column' in kwargs:
         fv.renmae(columns={kwargs['fire_column']: 'fire'}, inplace=True)     
@@ -98,17 +99,17 @@
         AOCshp (_type_): _description_
         fireshp (_type_): _description_
         hexagons (_type_): _description_
 
     Returns:
         _type_: _description_
     """
-
+    hexagon = hexagons.copy()
     if 'Node_ID' in kwargs:
-        hexagon = hexagons.rename(columns={kwargs["Node_ID"]: 'Node_ID'})
+        hexagon = hexagon.rename(columns={kwargs["Node_ID"]: 'Node_ID'})
     fv = fire_vectors.copy()
     if 'column_i' in kwargs:
         fv.rename(columns={kwargs["column_i"]: 'column_i'}, inplace=True)    
     if 'column_j' in kwargs:
         fv.rename(columns={kwargs["column_j"]: 'column_j'}, inplace=True)
     if 'fire_column' in kwargs:
         fv.renmae(columns={kwargs['fire_column']: 'fire'}, inplace=True) 
@@ -117,27 +118,27 @@
     fireAOC = fire_vectors.loc[fire_vectors['i'].isin(aoc['Node_ID'])]
     fireAOCshp = fireshp.merge(fireAOC, on='fire', how='right')
     fireAOCshp['V'] = 1
     fireAOCshp = fireAOCshp.dissolve(by='V')
     fireAOCshp['area_ha'] = fireAOCshp.area/10000
     return fireAOCshp
 
-def generate_SSR(fire_vectors, hexagons, **kwargs):
+def generate_ssr(fire_vectors, hexagons, **kwargs):
     """Generate a shapefile with values of Source-Sink-Ratio based on the fire vectors 
 
     Args:
         fire_vectors (_type_): _description_
         hexagons (_type_): _description_
 
     Returns:
         _type_: _description_
     """    
- 
+    hexagon = hexagons.copy()
     if 'Node_ID' in kwargs:
-        hexagon = hexagons.rename(columns={kwargs["Node_ID"]: 'Node_ID'})
+        hexagon = hexagon.rename(columns={kwargs["Node_ID"]: 'Node_ID'})
     fv = fire_vectors.copy()
     if 'column_i' in kwargs:
         fv.rename(columns={kwargs["column_i"]: 'column_i'}, inplace=True)    
     if 'column_j' in kwargs:
         fv.rename(columns={kwargs["column_j"]: 'column_j'}, inplace=True)
     if 'fire_column' in kwargs:
         fv.renmae(columns={kwargs['fire_column']: 'fire'}, inplace=True)
```

### Comparing `postbp-0.1.1/postbp/spreadrose.py` & `postbp-0.1.2/postbp/spreadrose.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from windrose import WindroseAxes
 import matplotlib.cm as cm
-import pandas as pd
 import geopandas as gpd
 from math import atan2, degrees
 from shapely.geometry import LineString 
 from matplotlib import pyplot as plt
+import tqdm
 
 def angle_from_pij(record):
     """_summary_
 
     Args:
         record (_type_): _description_
 
@@ -51,22 +51,23 @@
     Args:
         pijVectors (_type_): _description_
         nodes (_type_): _description_
 
     Returns:
         _type_: _description_
     """    
+    node = nodes.copy()
     if 'Node_ID' in kwargs:
-        node = nodes.rename(columns={kwargs["Node_ID"]: 'Node_ID'})
+        node = node.rename(columns={kwargs["Node_ID"]: 'Node_ID'})
     pij = pijVectors.copy()  
 
     pij = node.merge(pij, left_on = 'Node_ID', right_on = 'column_i', how = 'right')
     pij = pij.merge(node, left_on = 'column_j', right_on = 'Node_ID', how = 'left')    
     pij.drop(labels = ['Node_ID_x', 'Node_ID_y'], axis = 1, inplace = True)
-    for index, row in pij.iterrows():
+    for index, row in tqdm(pij.iterrows()):
         pij.at[index, 'angle'] = angle_from_pij(row)
     dffLine = [LineString(xy) for xy in zip(pij['geometry_x'], pij['geometry_y'])]
     pij = gpd.GeoDataFrame(pij, crs = node.crs, geometry = dffLine )
     pij.drop(labels = ['geometry_x', 'geometry_y'], axis = 1, inplace = True)
     pij['len'] = pij.geometry.length
     pij['pij'] = pij['pij'].astype(float)
     pij['pij_len'] = pij['pij']*pij['len']
```

### Comparing `postbp-0.1.1/postbp/tessellation.py` & `postbp-0.1.2/postbp/tessellation.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 4. generate the centroid of the hexes as nodes shapefile
 5. generate arcs connecting neighbouring nodes
 
 '''
 
 import geopandas as gpd
 from shapely.geometry import Polygon, Point, LineString
-import pandas as pd
 import warnings
 warnings.filterwarnings("ignore")
 import math
+import tqdm
 
 def create_hexnodes(area, xmin, ymin, xmax, ymax):
     nodes = []
     
     side = 3**0.25 * math.sqrt(2 * area / 9)
     v_step = math.sqrt(3) * side
     h_step = 1.5 * side
@@ -70,15 +70,15 @@
     Args:
         boundaryShp (_type_): _description_
 
     Returns:
         _type_: _description_
     """    
     if 'area' in kwargs:
-        area = area
+        area = kwargs['area']
 
     if "side" in kwargs:
         area = kwargs["side"]**2*3/2*math.sqrt(3)
 
     if "diameter" in kwargs:
         area = kwargs["diameter"]**2*3/8*math.sqrt(3)
     
@@ -103,15 +103,15 @@
     Args:
         boundaryShp (_type_): _description_
 
     Returns:
         _type_: _description_
     """    
     if 'area' in kwargs:
-        area = area
+        area = kwargs['area']
 
     if "side" in kwargs:
         area = kwargs["side"]**2*3/2*math.sqrt(3)
 
     if "diameter" in kwargs:
         area = kwargs["diameter"]**2*3/8*math.sqrt(3)
     
@@ -151,25 +151,26 @@
 
     Args:
         hexagons (_type_): _description_
 
     Returns:
         _type_: _description_
     """    
+    hexagon = hexagons.copy()
     if 'Node_ID' in kwargs:
-        hexagon = hexagons.rename(columns={kwargs["Node_ID"]: 'Node_ID'})
-    
+        hexagon = hexagon.rename(columns={kwargs["Node_ID"]: 'Node_ID'})
+        
     nodes = nodes_from_hexagons(hexagon)
     nodes = nodes.set_index('Node_ID')
     SRID = hexagon.crs
     hexagon = hexagon.set_index('Node_ID')
 
     arcs = gpd.GeoDataFrame()
     df=gpd.GeoDataFrame()
-    for index, _ in hexagon.iterrows():
+    for index, _ in tqdm(hexagon.iterrows()):
         nnnn = hexagon[~hexagon.geometry.disjoint(hexagon.at[index,'geometry'])].index.tolist()
         nnnn = [i for i in nnnn if index != i]
         mmmm = [index] * len(nnnn)
         mmnn = [LineString(xy) for xy in zip(nodes.loc[mmmm].geometry, nodes.loc[nnnn].geometry)]
         mmnn = gpd.GeoDataFrame(df, crs = SRID, geometry = mmnn )
         mmnn['Node_1'] = mmmm
         mmnn['Node_2'] = nnnn
```

### Comparing `postbp-0.1.1/postbp.egg-info/PKG-INFO` & `postbp-0.1.2/postbp.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postbp
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python Library
 Author-email: Ning Liu <ning.liu@nrcan-rncan.gc.ca>
 License: MIT License
 Project-URL: Homepage, https://github.com/nliu-cfs/postbp
 Keywords: postbp
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -19,14 +19,15 @@
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: geopandas
 Requires-Dist: shapely
 Requires-Dist: windrose
 Requires-Dist: matplotlib
+Requires-Dist: tqdm
 Provides-Extra: all
 Requires-Dist: postbp[extra]; extra == "all"
 Provides-Extra: extra
 Requires-Dist: pandas; extra == "extra"
 
 # postbp
```

### Comparing `postbp-0.1.1/postbp.egg-info/SOURCES.txt` & `postbp-0.1.2/postbp.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 docs/finalfirevectors.md
 docs/index.md
 docs/installation.md
 docs/postbp.md
 docs/spreadrose.md
 docs/tessellation.md
 docs/usage.md
-docs/examples/dataexamples.py
 docs/examples/intro.ipynb
 docs/overrides/main.html
 postbp/__init__.py
 postbp/common.py
 postbp/dailyfirevectors.py
 postbp/dataloader.py
 postbp/finalfirevectors.py
```

### Comparing `postbp-0.1.1/pyproject.toml` & `postbp-0.1.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "postbp"
-version = "0.1.1"
+version = "0.1.2"
 dynamic = [
     "dependencies",
 ]
 description = "A Python Library"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -48,15 +48,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.1.1"
+current_version = "0.1.2"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

