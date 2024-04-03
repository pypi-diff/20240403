# Comparing `tmp/db_query_profiler-0.0.4.tar.gz` & `tmp/db_query_profiler-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "db_query_profiler-0.0.4.tar", max compression
+gzip compressed data, was "db_query_profiler-0.0.6.tar", max compression
```

## Comparing `db_query_profiler-0.0.4.tar` & `db_query_profiler-0.0.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1066 2023-11-04 10:39:40.304827 db_query_profiler-0.0.4/LICENSE
--rw-r--r--   0        0        0     5892 2023-11-04 10:39:40.304827 db_query_profiler-0.0.4/README.md
--rw-r--r--   0        0        0      143 2023-11-04 10:39:40.304827 db_query_profiler-0.0.4/db_query_profiler/__init__.py
--rw-r--r--   0        0        0     7504 2023-11-04 10:39:40.304827 db_query_profiler-0.0.4/db_query_profiler/query_timer.py
--rw-r--r--   0        0        0      971 2023-11-04 10:39:40.304827 db_query_profiler-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     6534 1970-01-01 00:00:00.000000 db_query_profiler-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-03 16:46:23.452076 db_query_profiler-0.0.6/LICENSE
+-rw-r--r--   0        0        0     5835 2024-04-03 16:46:23.452076 db_query_profiler-0.0.6/README.md
+-rw-r--r--   0        0        0      144 2024-04-03 16:46:23.452076 db_query_profiler-0.0.6/db_query_profiler/__init__.py
+-rw-r--r--   0        0        0     7384 2024-04-03 16:46:23.452076 db_query_profiler-0.0.6/db_query_profiler/query_timer.py
+-rw-r--r--   0        0        0      993 2024-04-03 16:46:23.456076 db_query_profiler-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     6360 1970-01-01 00:00:00.000000 db_query_profiler-0.0.6/PKG-INFO
```

### Comparing `db_query_profiler-0.0.4/LICENSE` & `db_query_profiler-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `db_query_profiler-0.0.4/README.md` & `db_query_profiler-0.0.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,28 @@
+Metadata-Version: 2.1
+Name: db_query_profiler
+Version: 0.0.6
+Summary: Lightweight database query profiler.
+Author: Bilbottom
+Requires-Python: >=3.8,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: tqdm (>=4,<5)
+Description-Content-Type: text/markdown
+
 <div align="center">
 
-[![Python 3.7+](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-370/)
+[![Python](https://img.shields.io/badge/Python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-370/)
 [![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)
-[![application-tests](https://github.com/Bilbottom/db-query-profiler/actions/workflows/application-tests.yaml/badge.svg)](https://github.com/Bilbottom/db-query-profiler/actions/workflows/application-tests.yaml)
-[![coverage](coverage.svg)](https://github.com/dbrgn/coverage-badge)
+[![tests](https://github.com/Bilbottom/db-query-profiler/actions/workflows/tests.yaml/badge.svg)](https://github.com/Bilbottom/db-query-profiler/actions/workflows/tests.yaml)
+[![coverage](https://raw.githubusercontent.com/Bilbottom/db-query-profiler/main/coverage.svg)](https://github.com/dbrgn/coverage-badge)
 ![GitHub last commit](https://img.shields.io/github/last-commit/Bilbottom/db-query-profiler)
 
 [![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg?style=flat-square)](https://github.com/prettier/prettier)
 [![code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/Bilbottom/db-query-profiler/main.svg)](https://results.pre-commit.ci/latest/github/Bilbottom/db-query-profiler/main)
 [![Sourcery](https://img.shields.io/badge/Sourcery-enabled-brightgreen)](https://sourcery.ai)
@@ -18,22 +33,24 @@
 
 # Database Query Profiler 🗃️⏱️
 
 Lightweight database query profiler.
 
 This tool is database-agnostic -- just provide a class that connects to your database with an `execute` method, and the queries that you want to profile.
 
-**_This is NOT a replacement for analysing the [query plan](https://en.wikipedia.org/wiki/Query_plan). This should just support the analysis done with it._**
+> [!WARNING]
+>
+> **_This is NOT a replacement for analysing the [query plan](https://en.wikipedia.org/wiki/Query_plan). This should just support the analysis done with it._**
 
 ## Installation ⬇️
 
-This is currently only available on GitHub, so you'll need to supply the GitHub URL to `pip`:
+Grab a copy from PyPI like usual:
 
 ```
-pip install git+https://github.com/Bilbottom/db-query-profiler@v0.0.4
+pip install db-query-profiler
 ```
 
 ## Sample Output 📝
 
 Given a set of queries (details below), this package prints the average time in seconds taken to run each query, as well as the percentage of the total time taken by each query.
 
 The [`tqdm`](https://github.com/tqdm/tqdm) package is used to show progress of the queries being run.
@@ -152,7 +169,8 @@
 
 ```bash
 poetry install --sync --with dev,test
 pre-commit install --install-hooks
 ```
 
 Happy coding! 🎉
+
```

### Comparing `db_query_profiler-0.0.4/db_query_profiler/query_timer.py` & `db_query_profiler-0.0.6/db_query_profiler/query_timer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 """
 A module for timing SQL queries.
 """
+
 import datetime
 import functools
 import inspect
 import pathlib
-import sys
 import timeit
 import warnings
-from typing import Any, Callable, Generator, List, Union
+from typing import Any, Callable, Generator, List, Protocol, Union
 
 import tqdm
 
-if sys.version_info[:3] >= (3, 8, 0):
-    from typing import Protocol
-else:
-    from typing_extensions import Protocol
-
 
 class DatabaseConnection(Protocol):
     """
     Database connector to run SQL against the database.
     """
 
     def execute(self) -> Any:
```

### Comparing `db_query_profiler-0.0.4/pyproject.toml` & `db_query_profiler-0.0.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "db_query_profiler"
-version = "0.0.4"
+version = "0.0.6"
 description = "Lightweight database query profiler."
 authors = ["Bilbottom"]
 readme = "README.md"
 packages = [{include = "db_query_profiler"}]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 tqdm = "^4"
-typing-extensions = { version = "^4", python = "<3.8" }
 
-[tool.poetry.group.dev]
-optional = true
+[tool.poetry.group]
+dev.optional = true
+test.optional = true
+ide.optional = true
 
 [tool.poetry.group.dev.dependencies]
 coverage-badge = "^1.1.0"
 pre-commit = "^2.21.0"
 pylint = "2.13.9"
 
-[tool.poetry.group.test]
-optional = true
-
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4.0"
 pytest-cov = "^4.1.0"
 
+# Packages just for IDE integration
+[tool.poetry.group.ide.dependencies]
+black = "*"
+
 
 [tool.pytest.ini_options]
 addopts = "--cov=db_query_profiler --cov-report=term-missing --cov-fail-under=70"
-testpaths = [
-    "tests",
-]
+testpaths = ["tests"]
 
 
 [tool.isort]
 profile = "black"
 
 
 [tool.pylint.format]
```

