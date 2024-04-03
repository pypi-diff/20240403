# Comparing `tmp/llama_index_callbacks_langfuse-0.1.3.tar.gz` & `tmp/llama_index_callbacks_langfuse-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_callbacks_langfuse-0.1.3.tar", max compression
+gzip compressed data, was "llama_index_callbacks_langfuse-0.1.4.tar", max compression
```

## Comparing `llama_index_callbacks_langfuse-0.1.3.tar` & `llama_index_callbacks_langfuse-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      930 2024-03-19 16:08:54.619869 llama_index_callbacks_langfuse-0.1.3/README.md
--rw-r--r--   0        0        0      115 2024-03-19 16:08:54.619869 llama_index_callbacks_langfuse-0.1.3/llama_index/callbacks/langfuse/__init__.py
--rw-r--r--   0        0        0      348 2024-03-19 16:08:54.619869 llama_index_callbacks_langfuse-0.1.3/llama_index/callbacks/langfuse/base.py
--rw-r--r--   0        0        0     1507 2024-03-19 16:08:54.619869 llama_index_callbacks_langfuse-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1533 1970-01-01 00:00:00.000000 llama_index_callbacks_langfuse-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      930 2024-04-03 16:01:02.573687 llama_index_callbacks_langfuse-0.1.4/README.md
+-rw-r--r--   0        0        0      115 2024-04-03 16:01:02.573687 llama_index_callbacks_langfuse-0.1.4/llama_index/callbacks/langfuse/__init__.py
+-rw-r--r--   0        0        0      348 2024-04-03 16:01:02.573687 llama_index_callbacks_langfuse-0.1.4/llama_index/callbacks/langfuse/base.py
+-rw-r--r--   0        0        0     1507 2024-04-03 16:01:02.573687 llama_index_callbacks_langfuse-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1533 1970-01-01 00:00:00.000000 llama_index_callbacks_langfuse-0.1.4/PKG-INFO
```

### Comparing `llama_index_callbacks_langfuse-0.1.3/README.md` & `llama_index_callbacks_langfuse-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_callbacks_langfuse-0.1.3/pyproject.toml` & `llama_index_callbacks_langfuse-0.1.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -24,20 +24,20 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index callbacks langfuse integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-callbacks-langfuse"
 readme = "README.md"
-version = "0.1.3"
+version = "0.1.4"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.8"
-langfuse = "^2.20.4"
+langfuse = "^2.21.2"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
 pre-commit = "3.2.0"
 pylint = "2.15.10"
```

### Comparing `llama_index_callbacks_langfuse-0.1.3/PKG-INFO` & `llama_index_callbacks_langfuse-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: llama-index-callbacks-langfuse
-Version: 0.1.3
+Version: 0.1.4
 Summary: llama-index callbacks langfuse integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: langfuse (>=2.20.4,<3.0.0)
+Requires-Dist: langfuse (>=2.21.2,<3.0.0)
 Requires-Dist: llama-index-core (>=0.10.8,<0.11.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Callbacks Integration: Langfuse
 
 [Langfuse](https://langfuse.com/docs) is an open source LLM engineering platform to help teams collaboratively debug, analyze and iterate on their LLM Applications. With the Langfuse integration, you can seamlessly track and monitor performance, traces, and metrics of your LlamaIndex application. Detailed traces of the LlamaIndex context augmentation and the LLM querying processes are captured and can be inspected directly in the Langfuse UI.
```

