# Comparing `tmp/pyhelper_utils-0.0.2.tar.gz` & `tmp/pyhelper_utils-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhelper_utils-0.0.2.tar", max compression
+gzip compressed data, was "pyhelper_utils-0.0.3.tar", max compression
```

## Comparing `pyhelper_utils-0.0.2.tar` & `pyhelper_utils-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0    11357 2024-04-03 12:59:39.367686 pyhelper_utils-0.0.2/LICENSE
--rw-r--r--   0        0        0      680 2024-04-03 12:59:39.367686 pyhelper_utils-0.0.2/README.md
--rw-r--r--   0        0        0        0 2024-04-03 12:59:39.370686 pyhelper_utils-0.0.2/pyhelper_utils/__init__.py
--rw-r--r--   0        0        0     1798 2024-04-03 12:59:39.370686 pyhelper_utils-0.0.2/pyhelper_utils/general.py
--rw-r--r--   0        0        0     1453 2024-04-03 12:59:43.529652 pyhelper_utils-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1562 1970-01-01 00:00:00.000000 pyhelper_utils-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-03 15:36:29.586323 pyhelper_utils-0.0.3/LICENSE
+-rw-r--r--   0        0        0      680 2024-04-03 15:36:29.587323 pyhelper_utils-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 15:36:29.590323 pyhelper_utils-0.0.3/pyhelper_utils/__init__.py
+-rw-r--r--   0        0        0     1798 2024-04-03 15:36:29.590323 pyhelper_utils-0.0.3/pyhelper_utils/general.py
+-rw-r--r--   0        0        0     2286 2024-04-03 15:36:29.590323 pyhelper_utils-0.0.3/pyhelper_utils/shell.py
+-rw-r--r--   0        0        0     1511 2024-04-03 15:36:36.436267 pyhelper_utils-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1616 1970-01-01 00:00:00.000000 pyhelper_utils-0.0.3/PKG-INFO
```

### Comparing `pyhelper_utils-0.0.2/LICENSE` & `pyhelper_utils-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhelper_utils-0.0.2/README.md` & `pyhelper_utils-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyhelper_utils-0.0.2/pyhelper_utils/general.py` & `pyhelper_utils-0.0.3/pyhelper_utils/general.py`

 * *Files identical despite different names*

### Comparing `pyhelper_utils-0.0.2/pyproject.toml` & `pyhelper_utils-0.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 output-format = "grouped"
 
 [tool.ruff.format]
 exclude = [".git", ".venv", ".mypy_cache", ".tox", "__pycache__"]
 
 [tool.poetry]
 name = "pyhelper-utils"
-version = "0.0.2"
+version = "0.0.3"
 description = "Collective utility functions for python projects"
 readme = "README.md"
 repository = "https://github.com/RedHatQE/pyhelper-utils"
 authors = [
   "Meni Yakove <myakove@gmail.com>",
   "Ruth Netser <rnetser@gmail.com>",
   "Debarati Basu-Nag <dbasunag@redhat.com>",
@@ -35,24 +35,27 @@
 classifiers = [
   "Programming Language :: Python :: 3",
   "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
+python-simple-logger = "^1.0.19"
 
 [tool.poetry.group.tests.dependencies]
 pytest = "^8.1.1"
 pytest-cov = "^5.0.0"
+pytest-mock = "^3.14.0"
 
 
 [tool.poetry.group.dev.dependencies]
 ipdb = "^0.13.13"
 ipython = "*"
 
+
 [tool.poetry-dynamic-versioning]
 enable = false
 pattern = "((?P<epoch>\\d+)!)?(?P<base>\\d+(\\.\\d+)*)"
 
 [tool.poetry-dynamic-versioning.substitution]
 files = ["VERSION"]
```

### Comparing `pyhelper_utils-0.0.2/PKG-INFO` & `pyhelper_utils-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: pyhelper-utils
-Version: 0.0.2
+Version: 0.0.3
 Summary: Collective utility functions for python projects
 Home-page: https://github.com/RedHatQE/pyhelper-utils
 License: Apache-2.0
 Author: Meni Yakove
 Author-email: myakove@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: python-simple-logger (>=1.0.19,<2.0.0)
 Project-URL: Documentation, https://github.com/RedHatQE/pyhelper-utils/blob/main/README.md
 Project-URL: Repository, https://github.com/RedHatQE/pyhelper-utils
 Description-Content-Type: text/markdown
 
 # pyhelper-utils
 Repository for various python utilities
 ## Installation
```

