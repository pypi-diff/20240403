# Comparing `tmp/lint-python-2.1.1.tar.gz` & `tmp/lint-python-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lint-python-2.1.1.tar", last modified: Fri Sep  1 13:47:12 2023, max compression
+gzip compressed data, was "lint-python-2.2.0.tar", last modified: Wed Apr  3 12:42:41 2024, max compression
```

## Comparing `lint-python-2.1.1.tar` & `lint-python-2.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 13:47:12.857001 lint-python-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (999)     3102 2023-09-01 13:47:12.857001 lint-python-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     2837 2023-09-01 13:47:03.000000 lint-python-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 13:47:12.857001 lint-python-2.1.1/lint_python/
--rw-r--r--   0 runner    (1001) docker     (999)       62 2023-09-01 13:47:03.000000 lint-python-2.1.1/lint_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-09-01 13:47:03.000000 lint-python-2.1.1/lint_python/__main__.py
--rw-r--r--   0 runner    (1001) docker     (999)      104 2023-09-01 13:47:03.000000 lint-python-2.1.1/lint_python/constants.py
--rw-r--r--   0 runner    (1001) docker     (999)     6092 2023-09-01 13:47:03.000000 lint-python-2.1.1/lint_python/lint_python.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 13:47:12.857001 lint-python-2.1.1/lint_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     3102 2023-09-01 13:47:12.000000 lint-python-2.1.1/lint_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      336 2023-09-01 13:47:12.000000 lint-python-2.1.1/lint_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-01 13:47:12.000000 lint-python-2.1.1/lint_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       61 2023-09-01 13:47:12.000000 lint-python-2.1.1/lint_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (999)       12 2023-09-01 13:47:12.000000 lint-python-2.1.1/lint_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       12 2023-09-01 13:47:12.000000 lint-python-2.1.1/lint_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)      872 2023-09-01 13:47:03.000000 lint-python-2.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-09-01 13:47:12.857001 lint-python-2.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:41.832422 lint-python-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-03 12:42:41.832422 lint-python-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-03 12:42:35.000000 lint-python-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:41.828422 lint-python-2.2.0/lint_python/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-03 12:42:35.000000 lint-python-2.2.0/lint_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 12:42:35.000000 lint-python-2.2.0/lint_python/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-03 12:42:35.000000 lint-python-2.2.0/lint_python/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6092 2024-04-03 12:42:35.000000 lint-python-2.2.0/lint_python/lint_python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:41.832422 lint-python-2.2.0/lint_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-03 12:42:41.000000 lint-python-2.2.0/lint_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-03 12:42:41.000000 lint-python-2.2.0/lint_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 12:42:41.000000 lint-python-2.2.0/lint_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-03 12:42:41.000000 lint-python-2.2.0/lint_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-03 12:42:41.000000 lint-python-2.2.0/lint_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-03 12:42:41.000000 lint-python-2.2.0/lint_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-03 12:42:35.000000 lint-python-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 12:42:41.832422 lint-python-2.2.0/setup.cfg
```

### Comparing `lint-python-2.1.1/PKG-INFO` & `lint-python-2.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: lint-python
-Version: 2.1.1
+Version: 2.2.0
 Summary: CLI tool used for running linter on project configured with CERT-Polska/lint-python-action
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
+Requires-Dist: pyyaml
+Requires-Dist: toml
 
 # lint-python-action
 
 Tool that runs common linters on CERT Polska projects written in Python.
 
 Includes [GitHub Actions](https://docs.github.com/en/actions) custom action.
```

### Comparing `lint-python-2.1.1/README.md` & `lint-python-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `lint-python-2.1.1/lint_python/lint_python.py` & `lint-python-2.2.0/lint_python/lint_python.py`

 * *Files identical despite different names*

### Comparing `lint-python-2.1.1/lint_python.egg-info/PKG-INFO` & `lint-python-2.2.0/lint_python.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: lint-python
-Version: 2.1.1
+Version: 2.2.0
 Summary: CLI tool used for running linter on project configured with CERT-Polska/lint-python-action
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
+Requires-Dist: pyyaml
+Requires-Dist: toml
 
 # lint-python-action
 
 Tool that runs common linters on CERT Polska projects written in Python.
 
 Includes [GitHub Actions](https://docs.github.com/en/actions) custom action.
```

### Comparing `lint-python-2.1.1/pyproject.toml` & `lint-python-2.2.0/pyproject.toml`

 * *Files identical despite different names*

