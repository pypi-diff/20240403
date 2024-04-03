# Comparing `tmp/langflow-1.0.0a0.tar.gz` & `tmp/langflow-1.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langflow-1.0.0a0.tar", max compression
+gzip compressed data, was "langflow-1.0.0a1.tar", max compression
```

## Comparing `langflow-1.0.0a0.tar` & `langflow-1.0.0a1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1065 2023-05-29 17:29:02.212613 langflow-1.0.0a0/LICENSE
--rw-r--r--   0        0        0     9324 2024-04-02 14:24:00.552315 langflow-1.0.0a0/README.md
--rw-r--r--   0        0        0     3750 2024-04-02 22:59:00.423717 langflow-1.0.0a0/pyproject.toml
--rw-r--r--   0        0        0       47 2024-04-02 04:17:58.852217 langflow-1.0.0a0/src/backend/langflow/version/__init__.py
--rw-r--r--   0        0        0      244 2024-04-02 21:46:53.099735 langflow-1.0.0a0/src/backend/langflow/version/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      449 2024-04-02 21:46:53.114509 langflow-1.0.0a0/src/backend/langflow/version/__pycache__/version.cpython-311.pyc
--rw-r--r--   0        0        0      156 2024-04-02 04:17:58.852448 langflow-1.0.0a0/src/backend/langflow/version/version.py
--rw-r--r--   0        0        0    12535 1970-01-01 00:00:00.000000 langflow-1.0.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-29 17:29:02.212613 langflow-1.0.0a1/LICENSE
+-rw-r--r--   0        0        0     9324 2024-04-02 14:24:00.552315 langflow-1.0.0a1/README.md
+-rw-r--r--   0        0        0     3771 2024-04-03 20:12:44.094243 langflow-1.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0       47 2024-04-02 04:17:58.852217 langflow-1.0.0a1/src/backend/langflow/version/__init__.py
+-rw-r--r--   0        0        0      244 2024-04-02 21:46:53.099735 langflow-1.0.0a1/src/backend/langflow/version/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      449 2024-04-02 21:46:53.114509 langflow-1.0.0a1/src/backend/langflow/version/__pycache__/version.cpython-311.pyc
+-rw-r--r--   0        0        0      156 2024-04-02 04:17:58.852448 langflow-1.0.0a1/src/backend/langflow/version/version.py
+-rw-r--r--   0        0        0    12577 1970-01-01 00:00:00.000000 langflow-1.0.0a1/PKG-INFO
```

### Comparing `langflow-1.0.0a0/LICENSE` & `langflow-1.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `langflow-1.0.0a0/README.md` & `langflow-1.0.0a1/README.md`

 * *Files identical despite different names*

### Comparing `langflow-1.0.0a0/pyproject.toml` & `langflow-1.0.0a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langflow"
-version = "1.0.0a0"
+version = "1.0.0a1"
 description = "A Python package with a built-in web application"
 authors = ["Logspace <contact@logspace.ai>"]
 maintainers = [
     "Carlos Coelho <carlos@logspace.ai>",
     "Cristhian Zanforlin <cristhian.lousa@gmail.com>",
     "Gabriel Almeida <gabriel@logspace.ai>",
     "Igor Carvalho <igorr.ackerman@gmail.com>",
@@ -24,15 +24,15 @@
 langflow = "langflow.__main__:main"
 
 [tool.poetry-monorepo-dependency-plugin]
 enable = true
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
-langflow-base = "^0.0.16"
+langflow-base = "^0.0.17"
 beautifulsoup4 = "^4.12.2"
 google-search-results = "^2.4.1"
 google-api-python-client = "^2.118.0"
 huggingface-hub = { version = "^0.20.0", extras = ["inference"] }
 llama-cpp-python = { version = "~0.2.0", optional = true }
 networkx = "^3.1"
 pysrt = "^1.1.2"
@@ -76,14 +76,15 @@
 llama-index = "^0.10.13"
 langchain-openai = "^0.0.5"
 unstructured = { extras = ["md"], version = "^0.12.4" }
 dspy-ai = "^2.4.0"
 crewai = "^0.22.5"
 html2text = "^2024.2.26"
 assemblyai = "^0.23.1"
+litellm = "^1.34.22"
 
 [tool.poetry.group.dev.dependencies]
 types-redis = "^4.6.0.5"
 ipykernel = "^6.29.0"
 mypy = "^1.8.0"
 ruff = "^0.2.1"
 httpx = "*"
```

### Comparing `langflow-1.0.0a0/PKG-INFO` & `langflow-1.0.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langflow
-Version: 1.0.0a0
+Version: 1.0.0a1
 Summary: A Python package with a built-in web application
 Home-page: https://github.com/logspace-ai/langflow
 License: MIT
 Keywords: nlp,langchain,openai,gpt,gui
 Author: Logspace
 Author-email: contact@logspace.ai
 Maintainer: Carlos Coelho
@@ -35,16 +35,17 @@
 Requires-Dist: google-api-python-client (>=2.118.0,<3.0.0)
 Requires-Dist: google-search-results (>=2.4.1,<3.0.0)
 Requires-Dist: html2text (>=2024.2.26,<2025.0.0)
 Requires-Dist: huggingface-hub[inference] (>=0.20.0,<0.21.0)
 Requires-Dist: langchain-cohere (>=0.1.0rc1,<0.2.0)
 Requires-Dist: langchain-google-genai (>=1.0.1,<2.0.0)
 Requires-Dist: langchain-openai (>=0.0.5,<0.0.6)
-Requires-Dist: langflow-base (>=0.0.16,<0.0.17)
+Requires-Dist: langflow-base (>=0.0.17,<0.0.18)
 Requires-Dist: langfuse (>=2.9.0,<3.0.0)
+Requires-Dist: litellm (>=1.34.22,<2.0.0)
 Requires-Dist: llama-cpp-python (>=0.2.0,<0.3.0) ; extra == "local"
 Requires-Dist: llama-index (>=0.10.13,<0.11.0)
 Requires-Dist: markupsafe (>=2.1.3,<3.0.0)
 Requires-Dist: metal-sdk (>=2.5.0,<3.0.0)
 Requires-Dist: metaphor-python (>=0.1.11,<0.2.0)
 Requires-Dist: networkx (>=3.1,<4.0)
 Requires-Dist: numexpr (>=2.8.6,<3.0.0)
```

