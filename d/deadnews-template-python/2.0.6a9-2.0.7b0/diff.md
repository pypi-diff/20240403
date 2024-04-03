# Comparing `tmp/deadnews_template_python-2.0.6a9.tar.gz` & `tmp/deadnews_template_python-2.0.7b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deadnews_template_python-2.0.6a9.tar", max compression
+gzip compressed data, was "deadnews_template_python-2.0.7b0.tar", max compression
```

## Comparing `deadnews_template_python-2.0.6a9.tar` & `deadnews_template_python-2.0.7b0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1065 2024-04-02 18:05:59.119178 deadnews_template_python-2.0.6a9/LICENSE
--rw-r--r--   0        0        0     1948 2024-04-02 18:05:59.119178 deadnews_template_python-2.0.6a9/README.md
--rw-r--r--   0        0        0     2939 2024-04-02 18:06:11.035153 deadnews_template_python-2.0.6a9/pyproject.toml
--rw-r--r--   0        0        0       94 2024-04-02 18:05:59.119178 deadnews_template_python-2.0.6a9/src/deadnews_template_python/__init__.py
--rw-r--r--   0        0        0      514 2024-04-02 18:05:59.119178 deadnews_template_python-2.0.6a9/src/deadnews_template_python/__main__.py
--rw-r--r--   0        0        0     1392 2024-04-02 18:05:59.119178 deadnews_template_python-2.0.6a9/src/deadnews_template_python/app.py
--rw-r--r--   0        0        0     2879 1970-01-01 00:00:00.000000 deadnews_template_python-2.0.6a9/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-03 16:12:07.073014 deadnews_template_python-2.0.7b0/LICENSE
+-rw-r--r--   0        0        0     1577 2024-04-03 16:12:07.073014 deadnews_template_python-2.0.7b0/README.md
+-rw-r--r--   0        0        0     2938 2024-04-03 16:12:22.221023 deadnews_template_python-2.0.7b0/pyproject.toml
+-rw-r--r--   0        0        0       94 2024-04-03 16:12:07.077014 deadnews_template_python-2.0.7b0/src/deadnews_template_python/__init__.py
+-rw-r--r--   0        0        0      514 2024-04-03 16:12:07.077014 deadnews_template_python-2.0.7b0/src/deadnews_template_python/__main__.py
+-rw-r--r--   0        0        0     1392 2024-04-03 16:12:07.077014 deadnews_template_python-2.0.7b0/src/deadnews_template_python/app.py
+-rw-r--r--   0        0        0     2508 1970-01-01 00:00:00.000000 deadnews_template_python-2.0.7b0/PKG-INFO
```

### Comparing `deadnews_template_python-2.0.6a9/LICENSE` & `deadnews_template_python-2.0.7b0/LICENSE`

 * *Files identical despite different names*

### Comparing `deadnews_template_python-2.0.6a9/README.md` & `deadnews_template_python-2.0.7b0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 # deadnews-template-python
 
 > Python Project Template
 
 [![PyPI: Version](https://img.shields.io/pypi/v/deadnews-template-python?logo=pypi&logoColor=white)](https://pypi.org/project/deadnews-template-python)
 [![GitHub: Release](https://img.shields.io/github/v/release/deadnews/deadnews-template-python?logo=github&logoColor=white)](https://github.com/deadnews/deadnews-template-python/releases/latest)
+[![Docker: ghcr](https://img.shields.io/badge/docker-ghcr-blue.svg?logo=github&logoColor=white)](https://github.com/deadnews/deadnews-template-python/pkgs/container/deadnews-template-python)
 [![Documentation](https://img.shields.io/badge/documentation-gray.svg?logo=materialformkdocs&logoColor=white)](https://deadnews.github.io/deadnews-template-python)
-[![Changelog](https://img.shields.io/badge/changelog-gray.svg?logo=github&logoColor=white)](https://github.com/deadnews/deadnews-template-python/blob/main/CHANGELOG.md)
-[![CI: main](https://img.shields.io/github/actions/workflow/status/deadnews/deadnews-template-python/main.yml?branch=main&logo=github&logoColor=white&label=main)](https://github.com/deadnews/deadnews-template-python/actions/workflows/main.yml)
 [![CI: pre-commit](https://results.pre-commit.ci/badge/github/DeadNews/deadnews-template-python/main.svg)](https://results.pre-commit.ci/latest/github/deadnews/deadnews-template-python/main)
+[![CI: main](https://img.shields.io/github/actions/workflow/status/deadnews/deadnews-template-python/main.yml?branch=main&logo=github&logoColor=white&label=main)](https://github.com/deadnews/deadnews-template-python/actions/workflows/main.yml)
 [![Coverage](https://img.shields.io/codecov/c/github/deadnews/deadnews-template-python?token=OCZDZIYPMC&logo=codecov&logoColor=white)](https://codecov.io/gh/deadnews/deadnews-template-python)
-[![Docker: ghcr](https://img.shields.io/badge/docker-ghcr-blue.svg?logo=github&logoColor=white)](https://github.com/deadnews/deadnews-template-python/pkgs/container/deadnews-template-python)
-[![Docker: image-size](https://ghcr-badge.egpl.dev/deadnews/deadnews-template-python/size?color=%230e80c0)](https://github.com/deadnews/deadnews-template-python/pkgs/container/deadnews-template-python)
 
 ## Installation
 
 PyPI
 
 ```sh
 pip install deadnews-template-python
```

### Comparing `deadnews_template_python-2.0.6a9/pyproject.toml` & `deadnews_template_python-2.0.7b0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "deadnews-template-python"
-version = "2.0.6-alpha.9"
+version = "2.0.7-beta.0"
 description = "Python Project Template"
 authors = ["DeadNews <deadnewsgit@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/deadnews/deadnews-template-python"
 repository = "https://github.com/deadnews/deadnews-template-python"
 documentation = "https://deadnews.github.io/deadnews-template-python"
@@ -23,30 +23,30 @@
 fastapi = "^0.110.0"
 pydantic = "^2.5.3"
 uvicorn = { version = "^0.29.0", extras = ["standard"] }
 
 [tool.poetry.group.lint.dependencies]
 mypy = "^1.9.0"
 poethepoet = "^0.25.0"
-pyright = "^1.1.354"
-ruff = "^0.3.3"
+pyright = "^1.1.356"
+ruff = "^0.3.5"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.1.1"
-pytest-cov = "^4.1.0"
+pytest-cov = "^5.0.0"
 httpx = "^0.27.0"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.5.3"
 mkdocs-gen-files = "^0.5.0"
 mkdocs-literate-nav = "^0.6.1"
-mkdocs-material = "^9.5.13"
-mkdocs-swagger-ui-tag = "^0.6.8"
+mkdocs-material = "^9.5.17"
+mkdocs-swagger-ui-tag = "^0.6.9"
 mkdocstrings = "^0.24.1"
-mkdocstrings-python = "^1.9.0"
+mkdocstrings-python = "^1.9.1"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "semver"
 
 [tool.poe.tasks]
```

### Comparing `deadnews_template_python-2.0.6a9/src/deadnews_template_python/__main__.py` & `deadnews_template_python-2.0.7b0/src/deadnews_template_python/__main__.py`

 * *Files identical despite different names*

### Comparing `deadnews_template_python-2.0.6a9/src/deadnews_template_python/app.py` & `deadnews_template_python-2.0.7b0/src/deadnews_template_python/app.py`

 * *Files identical despite different names*

### Comparing `deadnews_template_python-2.0.6a9/PKG-INFO` & `deadnews_template_python-2.0.7b0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deadnews-template-python
-Version: 2.0.6a9
+Version: 2.0.7b0
 Summary: Python Project Template
 Home-page: https://github.com/deadnews/deadnews-template-python
 License: MIT
 Keywords: python,template,layout
 Author: DeadNews
 Author-email: deadnewsgit@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -23,21 +23,19 @@
 
 # deadnews-template-python
 
 > Python Project Template
 
 [![PyPI: Version](https://img.shields.io/pypi/v/deadnews-template-python?logo=pypi&logoColor=white)](https://pypi.org/project/deadnews-template-python)
 [![GitHub: Release](https://img.shields.io/github/v/release/deadnews/deadnews-template-python?logo=github&logoColor=white)](https://github.com/deadnews/deadnews-template-python/releases/latest)
+[![Docker: ghcr](https://img.shields.io/badge/docker-ghcr-blue.svg?logo=github&logoColor=white)](https://github.com/deadnews/deadnews-template-python/pkgs/container/deadnews-template-python)
 [![Documentation](https://img.shields.io/badge/documentation-gray.svg?logo=materialformkdocs&logoColor=white)](https://deadnews.github.io/deadnews-template-python)
-[![Changelog](https://img.shields.io/badge/changelog-gray.svg?logo=github&logoColor=white)](https://github.com/deadnews/deadnews-template-python/blob/main/CHANGELOG.md)
-[![CI: main](https://img.shields.io/github/actions/workflow/status/deadnews/deadnews-template-python/main.yml?branch=main&logo=github&logoColor=white&label=main)](https://github.com/deadnews/deadnews-template-python/actions/workflows/main.yml)
 [![CI: pre-commit](https://results.pre-commit.ci/badge/github/DeadNews/deadnews-template-python/main.svg)](https://results.pre-commit.ci/latest/github/deadnews/deadnews-template-python/main)
+[![CI: main](https://img.shields.io/github/actions/workflow/status/deadnews/deadnews-template-python/main.yml?branch=main&logo=github&logoColor=white&label=main)](https://github.com/deadnews/deadnews-template-python/actions/workflows/main.yml)
 [![Coverage](https://img.shields.io/codecov/c/github/deadnews/deadnews-template-python?token=OCZDZIYPMC&logo=codecov&logoColor=white)](https://codecov.io/gh/deadnews/deadnews-template-python)
-[![Docker: ghcr](https://img.shields.io/badge/docker-ghcr-blue.svg?logo=github&logoColor=white)](https://github.com/deadnews/deadnews-template-python/pkgs/container/deadnews-template-python)
-[![Docker: image-size](https://ghcr-badge.egpl.dev/deadnews/deadnews-template-python/size?color=%230e80c0)](https://github.com/deadnews/deadnews-template-python/pkgs/container/deadnews-template-python)
 
 ## Installation
 
 PyPI
 
 ```sh
 pip install deadnews-template-python
```

