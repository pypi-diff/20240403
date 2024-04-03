# Comparing `tmp/python_urbandict-0.3.3.tar.gz` & `tmp/python_urbandict-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_urbandict-0.3.3.tar", max compression
+gzip compressed data, was "python_urbandict-0.3.4.tar", max compression
```

## Comparing `python_urbandict-0.3.3.tar` & `python_urbandict-0.3.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1066 2023-10-26 11:44:44.305078 python_urbandict-0.3.3/LICENSE
--rw-r--r--   0        0        0     2325 2023-10-26 11:44:44.305078 python_urbandict-0.3.3/README.md
--rw-r--r--   0        0        0      974 2023-10-26 11:44:44.305078 python_urbandict-0.3.3/pyproject.toml
--rw-r--r--   0        0        0       77 2023-10-26 11:44:44.305078 python_urbandict-0.3.3/pyurbandict/__init__.py
--rw-r--r--   0        0        0     1211 2023-10-26 11:44:44.305078 python_urbandict-0.3.3/pyurbandict/parse.py
--rw-r--r--   0        0        0     3221 1970-01-01 00:00:00.000000 python_urbandict-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-03 00:18:50.181598 python_urbandict-0.3.4/LICENSE
+-rw-r--r--   0        0        0     2325 2024-04-03 00:18:50.181598 python_urbandict-0.3.4/README.md
+-rw-r--r--   0        0        0      954 2024-04-03 00:18:50.181598 python_urbandict-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0       77 2024-04-03 00:18:50.181598 python_urbandict-0.3.4/pyurbandict/__init__.py
+-rw-r--r--   0        0        0     1211 2024-04-03 00:18:50.181598 python_urbandict-0.3.4/pyurbandict/parse.py
+-rw-r--r--   0        0        0     3272 1970-01-01 00:00:00.000000 python_urbandict-0.3.4/PKG-INFO
```

### Comparing `python_urbandict-0.3.3/LICENSE` & `python_urbandict-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python_urbandict-0.3.3/README.md` & `python_urbandict-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `python_urbandict-0.3.3/pyproject.toml` & `python_urbandict-0.3.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.flake8]
 max-line-length = 88
 
 [tool.poetry]
 name = "python-urbandict"
-version = "0.3.3"
+version = "0.3.4"
 description = "Python wrapper for the Urban Dictionary API."
 authors = ["atbuy <contact.atbuy@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/atbuy/pyurbandict"
 repository = "https://github.com/atbuy/pyurbandict"
 keywords = ["urban", "dictionary", "api", "wrapper", "python"]
 include = ["README.md"]
@@ -23,16 +23,15 @@
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/atbuy/pyurbandict/issues"
 "Source Code" = "https://github.com/atbuy/pyurbandict"
 "CI/CD" = "https://github.com/atbuy/pyurbandict/actions"
 
 [tool.poetry.group.dev.dependencies]
 tox = "^4.6.0"
-black = "^23.3.0"
-flake8 = "^6.0.0"
 pre-commit = "^3.3.3"
 pytest = "^7.3.2"
 pytest-cov = "^4.1.0"
+ruff = "^0.3.5"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `python_urbandict-0.3.3/pyurbandict/parse.py` & `python_urbandict-0.3.4/pyurbandict/parse.py`

 * *Files identical despite different names*

### Comparing `python_urbandict-0.3.3/PKG-INFO` & `python_urbandict-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: python-urbandict
-Version: 0.3.3
+Version: 0.3.4
 Summary: Python wrapper for the Urban Dictionary API.
 Home-page: https://github.com/atbuy/pyurbandict
 License: MIT
 Keywords: urban,dictionary,api,wrapper,python
 Author: atbuy
 Author-email: contact.atbuy@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Bug Tracker, https://github.com/atbuy/pyurbandict/issues
 Project-URL: CI/CD, https://github.com/atbuy/pyurbandict/actions
 Project-URL: Repository, https://github.com/atbuy/pyurbandict
 Project-URL: Source Code, https://github.com/atbuy/pyurbandict
 Description-Content-Type: text/markdown
```

