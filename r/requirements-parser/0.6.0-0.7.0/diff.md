# Comparing `tmp/requirements_parser-0.6.0.tar.gz` & `tmp/requirements_parser-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requirements_parser-0.6.0.tar", max compression
+gzip compressed data, was "requirements_parser-0.7.0.tar", max compression
```

## Comparing `requirements_parser-0.6.0.tar` & `requirements_parser-0.7.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      251 2021-12-15 20:27:35.000000 requirements_parser-0.6.0/AUTHORS.rst
--rw-r--r--   0        0        0    11356 2021-12-17 14:45:01.000000 requirements_parser-0.6.0/LICENSE
--rw-r--r--   0        0        0     1785 2021-12-17 14:45:01.000000 requirements_parser-0.6.0/README.md
--rw-r--r--   0        0        0     3342 2024-03-27 16:55:36.841483 requirements_parser-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      882 2024-03-27 16:55:36.842133 requirements_parser-0.6.0/requirements/__init__.py
--rw-r--r--   0        0        0     2057 2022-04-25 07:09:51.000000 requirements_parser-0.6.0/requirements/fragment.py
--rw-r--r--   0        0        0     3344 2024-03-27 15:16:54.683683 requirements_parser-0.6.0/requirements/parser.py
--rw-r--r--   0        0        0      810 2022-01-18 09:49:33.000000 requirements_parser-0.6.0/requirements/py.typed
--rw-r--r--   0        0        0    10137 2024-03-27 15:17:00.195134 requirements_parser-0.6.0/requirements/requirement.py
--rw-r--r--   0        0        0     1063 2022-01-18 09:49:46.000000 requirements_parser-0.6.0/requirements/vcs.py
--rw-r--r--   0        0        0     3427 1970-01-01 00:00:00.000000 requirements_parser-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      251 2021-12-15 20:27:35.000000 requirements_parser-0.7.0/AUTHORS.rst
+-rw-r--r--   0        0        0    11356 2021-12-17 14:45:01.000000 requirements_parser-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1785 2021-12-17 14:45:01.000000 requirements_parser-0.7.0/README.md
+-rw-r--r--   0        0        0     3271 2024-03-28 09:55:10.712600 requirements_parser-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      883 2024-03-28 09:55:10.713191 requirements_parser-0.7.0/requirements/__init__.py
+-rw-r--r--   0        0        0     2057 2022-04-25 07:09:51.000000 requirements_parser-0.7.0/requirements/fragment.py
+-rw-r--r--   0        0        0     3344 2024-03-27 15:16:54.683683 requirements_parser-0.7.0/requirements/parser.py
+-rw-r--r--   0        0        0      810 2022-01-18 09:49:33.000000 requirements_parser-0.7.0/requirements/py.typed
+-rw-r--r--   0        0        0    10137 2024-03-27 15:17:00.195134 requirements_parser-0.7.0/requirements/requirement.py
+-rw-r--r--   0        0        0     1063 2022-01-18 09:49:46.000000 requirements_parser-0.7.0/requirements/vcs.py
+-rw-r--r--   0        0        0     3415 1970-01-01 00:00:00.000000 requirements_parser-0.7.0/PKG-INFO
```

### Comparing `requirements_parser-0.6.0/LICENSE` & `requirements_parser-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `requirements_parser-0.6.0/README.md` & `requirements_parser-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `requirements_parser-0.6.0/pyproject.toml` & `requirements_parser-0.7.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "requirements-parser"
-version = "0.6.0"
+version = "0.7.0"
 description = "This is a small Python module for parsing Pip requirement files."
 authors = [
     "Paul Horton <paul@hogr.dev>",
     "David Fischer (@davidfischer)",
     "Trey Hunner (@treyhunner)",
     "Dima Veselov (@dveselov)",
     "Sascha Peilicke (@saschpe)",
@@ -32,32 +32,32 @@
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
     'Intended Audience :: Information Technology',
     'Topic :: Software Development',
     'Topic :: Software Development :: Libraries :: Python Modules',
     'Topic :: System :: Software Distribution',
     'License :: OSI Approved :: Apache Software License',
-    'Programming Language :: Python :: 3.6',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
     'Typing :: Typed'
 ]
 keywords = [
     "Pip", "requirements", "parse"
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/madpah/requirements-parser/issues"
 
 [tool.poetry.dependencies]
-python = "^3.6"
-# `types-setuptools` need to stay in sync with version of `setuptools` - but 47 was not typed...
-types-setuptools = ">= 57.0.0"
+python = "^3.7"
+setuptools = ">= 59.7.0"
+types-setuptools = ">= 59.7.0"
 
 [tool.poetry.dev-dependencies]
 tox = "^3.24.3"
 coverage = "^6.2"
 mypy = "^0.920"
 autopep8 = "^1.6.0"
 flake8 = "^4.0.1"
```

### Comparing `requirements_parser-0.6.0/requirements/__init__.py` & `requirements_parser-0.7.0/requirements/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,8 +20,8 @@
 
 __all__ = [
     'parse'
 ]
 
 # !! version is managed by semantic_release
 # do not use typing here, or else `semantic_release` might have issues finding the variable
-__version__ = "0.6.0"  # noqa:Q000
+__version__ = "0.7.0"  # noqa:Q000
```

### Comparing `requirements_parser-0.6.0/requirements/fragment.py` & `requirements_parser-0.7.0/requirements/fragment.py`

 * *Files identical despite different names*

### Comparing `requirements_parser-0.6.0/requirements/parser.py` & `requirements_parser-0.7.0/requirements/parser.py`

 * *Files identical despite different names*

### Comparing `requirements_parser-0.6.0/requirements/py.typed` & `requirements_parser-0.7.0/requirements/py.typed`

 * *Files identical despite different names*

### Comparing `requirements_parser-0.6.0/requirements/requirement.py` & `requirements_parser-0.7.0/requirements/requirement.py`

 * *Files identical despite different names*

### Comparing `requirements_parser-0.6.0/requirements/vcs.py` & `requirements_parser-0.7.0/requirements/vcs.py`

 * *Files identical despite different names*

### Comparing `requirements_parser-0.6.0/PKG-INFO` & `requirements_parser-0.7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: requirements-parser
-Version: 0.6.0
+Version: 0.7.0
 Summary: This is a small Python module for parsing Pip requirement files.
 Home-page: https://github.com/madpah/requirements-parser
 License: Apache-2.0
 Keywords: Pip,requirements,parse
 Author: Paul Horton
 Author-email: paul@hogr.dev
 Maintainer: Paul Horton
 Maintainer-email: simplyecommerce@gmail.com
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Software Distribution
 Classifier: Typing :: Typed
-Requires-Dist: types-setuptools (>=57.0.0)
+Requires-Dist: setuptools (>=59.7.0)
+Requires-Dist: types-setuptools (>=59.7.0)
 Project-URL: Bug Tracker, https://github.com/madpah/requirements-parser/issues
 Project-URL: Repository, https://github.com/madpah/requirements-parser
 Description-Content-Type: text/markdown
 
 Requirements Parser
 ===================
```

