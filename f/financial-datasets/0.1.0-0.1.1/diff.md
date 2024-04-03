# Comparing `tmp/financial_datasets-0.1.0.tar.gz` & `tmp/financial_datasets-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "financial_datasets-0.1.0.tar", max compression
+gzip compressed data, was "financial_datasets-0.1.1.tar", max compression
```

## Comparing `financial_datasets-0.1.0.tar` & `financial_datasets-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,8 @@
--rw-r--r--   0        0        0     1068 2024-03-29 00:57:03.662287 financial_datasets-0.1.0/LICENSE
--rw-r--r--   0        0        0       20 2024-03-29 00:57:03.662440 financial_datasets-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-03-29 00:57:47.261649 financial_datasets-0.1.0/financial_datasets/__init__.py
--rw-r--r--   0        0        0      563 2024-03-29 01:16:40.088944 financial_datasets-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      748 1970-01-01 00:00:00.000000 financial_datasets-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-03-29 00:57:03.662287 financial_datasets-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2700 2024-03-30 23:21:00.793310 financial_datasets-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-03-29 00:57:47.261649 financial_datasets-0.1.1/financial_datasets/__init__.py
+-rw-r--r--   0        0        0      201 2024-04-03 12:06:00.779549 financial_datasets-0.1.1/financial_datasets/dataset.py
+-rw-r--r--   0        0        0     3435 2024-04-03 12:46:57.792263 financial_datasets-0.1.1/financial_datasets/generator.py
+-rw-r--r--   0        0        0      282 2024-03-30 22:53:11.228502 financial_datasets-0.1.1/financial_datasets/model.py
+-rw-r--r--   0        0        0      602 2024-04-03 12:48:21.832604 financial_datasets-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3472 1970-01-01 00:00:00.000000 financial_datasets-0.1.1/PKG-INFO
```

### Comparing `financial_datasets-0.1.0/LICENSE` & `financial_datasets-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `financial_datasets-0.1.0/pyproject.toml` & `financial_datasets-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "financial-datasets"
-version = "0.1.0"
+version = "0.1.1"
 description = "Financial datasets for LLMs"
 authors = ["Virat Singh <virat@virat.ai>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "financial_datasets"}]
 
 [tool.poetry.dependencies]
@@ -12,14 +12,16 @@
 langchain = "^0.1.13"
 openai = "^1.14.3"
 chromadb = "^0.4.24"
 tiktoken = "^0.6.0"
 anthropic = "^0.21.3"
 instructor = "^0.6.7"
 datasets = "^2.18.0"
+xmltodict = "^0.13.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
+twine = "^5.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

