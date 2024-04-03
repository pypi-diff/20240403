# Comparing `tmp/tefs-0.3.0.tar.gz` & `tmp/tefs-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tefs-0.3.0.tar", last modified: Tue Feb 27 13:57:04 2024, max compression
+gzip compressed data, was "tefs-0.3.1.tar", last modified: Wed Apr  3 11:23:18 2024, max compression
```

## Comparing `tefs-0.3.0.tar` & `tefs-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 13:57:04.127361 tefs-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-02-27 13:56:42.000000 tefs-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-02-27 13:57:04.127361 tefs-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-02-27 13:56:42.000000 tefs-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-02-27 13:56:42.000000 tefs-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-27 13:57:04.127361 tefs-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 13:57:04.123361 tefs-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 13:57:04.123361 tefs-0.3.0/src/tefs/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-27 13:56:42.000000 tefs-0.3.0/src/tefs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20229 2024-02-27 13:56:42.000000 tefs-0.3.0/src/tefs/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-02-27 13:56:42.000000 tefs-0.3.0/src/tefs/estimation.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-27 13:56:42.000000 tefs-0.3.0/src/tefs/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 13:57:04.127361 tefs-0.3.0/src/tefs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-02-27 13:57:04.000000 tefs-0.3.0/src/tefs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-02-27 13:57:04.000000 tefs-0.3.0/src/tefs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 13:57:04.000000 tefs-0.3.0/src/tefs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-02-27 13:57:04.000000 tefs-0.3.0/src/tefs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-27 13:57:04.000000 tefs-0.3.0/src/tefs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 13:57:04.127361 tefs-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-02-27 13:56:42.000000 tefs-0.3.0/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-02-27 13:56:42.000000 tefs-0.3.0/tests/test_estimation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:23:18.671984 tefs-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-03 11:21:11.000000 tefs-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-04-03 11:23:18.671984 tefs-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-03 11:21:11.000000 tefs-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-03 11:21:11.000000 tefs-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 11:23:18.671984 tefs-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:23:18.667984 tefs-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:23:18.667984 tefs-0.3.1/src/tefs/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-03 11:21:11.000000 tefs-0.3.1/src/tefs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20272 2024-04-03 11:21:11.000000 tefs-0.3.1/src/tefs/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-04-03 11:21:11.000000 tefs-0.3.1/src/tefs/estimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-04-03 11:21:11.000000 tefs-0.3.1/src/tefs/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-03 11:21:11.000000 tefs-0.3.1/src/tefs/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:23:18.671984 tefs-0.3.1/src/tefs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-04-03 11:23:18.000000 tefs-0.3.1/src/tefs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-03 11:23:18.000000 tefs-0.3.1/src/tefs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 11:23:18.000000 tefs-0.3.1/src/tefs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-03 11:23:18.000000 tefs-0.3.1/src/tefs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-03 11:23:18.000000 tefs-0.3.1/src/tefs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:23:18.671984 tefs-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-04-03 11:21:11.000000 tefs-0.3.1/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-03 11:21:11.000000 tefs-0.3.1/tests/test_estimation.py
```

### Comparing `tefs-0.3.0/LICENSE` & `tefs-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tefs-0.3.0/README.md` & `tefs-0.3.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -16,11 +16,26 @@
 pip install tefs
 ```
 
 ## How to use
 
 Refer to the documentation for usage examples.
 
+## Attribution
+
+If you use this package in your research, please cite the following paper:
+
+```bibtex
+@misc{bonetti2023causal,
+    title = {Causal {{Feature Selection}} via {{Transfer Entropy}}},
+    author = {Bonetti, Paolo and Metelli, Alberto Maria and Restelli, Marcello},
+    year = 2023,
+    eprint = {2310.11059},
+    archiveprefix = {arXiv},
+    primaryclass = {cs.LG}
+}
+```
+
 ## Authors
 
 - Paolo Bonetti ([@PaoloBonettiPolimi](https://github.com/PaoloBonettiPolimi))
 - Teo Bucci ([@teobucci](https://github.com/teobucci))
```

### Comparing `tefs-0.3.0/pyproject.toml` & `tefs-0.3.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools>=61.0.0", "wheel"]
+requires = ["setuptools>=61", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tefs"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
     { name = "Teo Bucci", email = "teobucci8@gmail.com" },
     { name = "Paolo Bonetti", email = "paolo.bonetti@polimi.it" },
 ]
 description = "Causal feature selection for time series data using transfer entropy"
 readme = "README.md"
 license = { file = "LICENSE" }
@@ -26,45 +26,53 @@
 ]
 dependencies = [
     "numpy",
     "pandas",
     "matplotlib",
     "scipy",
     "seaborn",
+    "scikit-learn",
 ]
+requires-python = ">=3.9"
 
 [project.urls]
 Homepage = "https://github.com/teobucci/tefs"
 Documentation = "https://github.com/teobucci/tefs"
 Repository = "https://github.com/teobucci/tefs"
 
-[project.optional-dependencies]
+[tool.pdm.dev-dependencies]
 docs = [
     "sphinx",
     "sphinx-rtd-theme",
     "myst-parser",
     "nbsphinx",
     "ipykernel",
     "jupyter",
     "jupyterlab",
     "nbconvert",
 ]
-dev = [
+test = [
     "pytest",
     "pytest-cov",
+]
+build = [
     "setuptools",
     "wheel",
     "twine",
     "build",
+    "bumpver",
 ]
 
 [tool.bumpver]
-current_version = "0.3.0"
+current_version = "0.3.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = ['current_version = "{version}"', 'version = "{version}"']
 "src/tefs/__init__.py" = ["{version}"]
+
+[tool.pdm]
+distribution = true
```

### Comparing `tefs-0.3.0/src/tefs/core.py` & `tefs-0.3.1/src/tefs/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -423,15 +423,18 @@
         :type direction: str
         :param verbose: Verbosity level, defaults to 0.
         :type verbose: int, optional
         :return: A list of feature indexes representing the selected features.
         """
 
         num_total_features = self.features.shape[1]
-        assert 0 < n <= num_total_features, f"n must be between 0 and {num_total_features}"
+        assert 0 <= n <= num_total_features, f"n must be between 0 and {num_total_features}"
+
+        if n == 0:
+            return []
 
         if self.direction == "backward":
 
             for iteration in self.result:
                 features_indexes = iteration["feature_scores"].keys()
                 if len(features_indexes) == n:
                     return list(features_indexes)
```

### Comparing `tefs-0.3.0/src/tefs/estimation.py` & `tefs-0.3.1/src/tefs/estimation.py`

 * *Files identical despite different names*

### Comparing `tefs-0.3.0/tests/test_core.py` & `tefs-0.3.1/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `tefs-0.3.0/tests/test_estimation.py` & `tefs-0.3.1/tests/test_estimation.py`

 * *Files identical despite different names*

