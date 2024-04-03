# Comparing `tmp/langflow-1.0.0a1.tar.gz` & `tmp/langflow-1.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langflow-1.0.0a1.tar", max compression
+gzip compressed data, was "langflow-1.0.0a2.tar", max compression
```

## Comparing `langflow-1.0.0a1.tar` & `langflow-1.0.0a2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1065 2023-05-29 17:29:02.212613 langflow-1.0.0a1/LICENSE
--rw-r--r--   0        0        0     9324 2024-04-02 14:24:00.552315 langflow-1.0.0a1/README.md
--rw-r--r--   0        0        0     3771 2024-04-03 20:12:44.094243 langflow-1.0.0a1/pyproject.toml
--rw-r--r--   0        0        0       47 2024-04-02 04:17:58.852217 langflow-1.0.0a1/src/backend/langflow/version/__init__.py
--rw-r--r--   0        0        0      244 2024-04-02 21:46:53.099735 langflow-1.0.0a1/src/backend/langflow/version/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      449 2024-04-02 21:46:53.114509 langflow-1.0.0a1/src/backend/langflow/version/__pycache__/version.cpython-311.pyc
--rw-r--r--   0        0        0      156 2024-04-02 04:17:58.852448 langflow-1.0.0a1/src/backend/langflow/version/version.py
--rw-r--r--   0        0        0    12577 1970-01-01 00:00:00.000000 langflow-1.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-29 17:29:02.212613 langflow-1.0.0a2/LICENSE
+-rw-r--r--   0        0        0     9324 2024-04-02 14:24:00.552315 langflow-1.0.0a2/README.md
+-rw-r--r--   0        0        0     3771 2024-04-03 21:03:31.788379 langflow-1.0.0a2/pyproject.toml
+-rw-r--r--   0        0        0       47 2024-04-02 04:17:58.852217 langflow-1.0.0a2/src/backend/langflow/version/__init__.py
+-rw-r--r--   0        0        0      244 2024-04-02 21:46:53.099735 langflow-1.0.0a2/src/backend/langflow/version/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      449 2024-04-02 21:46:53.114509 langflow-1.0.0a2/src/backend/langflow/version/__pycache__/version.cpython-311.pyc
+-rw-r--r--   0        0        0      156 2024-04-02 04:17:58.852448 langflow-1.0.0a2/src/backend/langflow/version/version.py
+-rw-r--r--   0        0        0    12577 1970-01-01 00:00:00.000000 langflow-1.0.0a2/PKG-INFO
```

### Comparing `langflow-1.0.0a1/LICENSE` & `langflow-1.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `langflow-1.0.0a1/README.md` & `langflow-1.0.0a2/README.md`

 * *Files identical despite different names*

### Comparing `langflow-1.0.0a1/pyproject.toml` & `langflow-1.0.0a2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langflow"
-version = "1.0.0a1"
+version = "1.0.0a2"
 description = "A Python package with a built-in web application"
 authors = ["Logspace <contact@logspace.ai>"]
 maintainers = [
     "Carlos Coelho <carlos@logspace.ai>",
     "Cristhian Zanforlin <cristhian.lousa@gmail.com>",
     "Gabriel Almeida <gabriel@logspace.ai>",
     "Igor Carvalho <igorr.ackerman@gmail.com>",
```

### Comparing `langflow-1.0.0a1/PKG-INFO` & `langflow-1.0.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langflow
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: A Python package with a built-in web application
 Home-page: https://github.com/logspace-ai/langflow
 License: MIT
 Keywords: nlp,langchain,openai,gpt,gui
 Author: Logspace
 Author-email: contact@logspace.ai
 Maintainer: Carlos Coelho
```

