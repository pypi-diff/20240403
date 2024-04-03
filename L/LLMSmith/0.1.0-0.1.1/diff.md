# Comparing `tmp/llmsmith-0.1.0.tar.gz` & `tmp/llmsmith-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmsmith-0.1.0.tar", max compression
+gzip compressed data, was "llmsmith-0.1.1.tar", max compression
```

## Comparing `llmsmith-0.1.0.tar` & `llmsmith-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1101 2024-04-03 09:01:34.959168 llmsmith-0.1.0/LICENSE
--rw-r--r--   0        0        0     1120 2024-04-03 04:13:09.876728 llmsmith-0.1.0/README.md
--rw-r--r--   0        0        0       78 2024-03-15 04:21:07.861053 llmsmith-0.1.0/llmsmith/__init__.py
--rw-r--r--   0        0        0        0 2024-03-14 11:47:53.187559 llmsmith-0.1.0/llmsmith/job/__init__.py
--rw-r--r--   0        0        0     7428 2024-04-02 12:37:57.531013 llmsmith-0.1.0/llmsmith/job/base.py
--rw-r--r--   0        0        0     8550 2024-04-03 05:58:40.426172 llmsmith-0.1.0/llmsmith/job/job.py
--rw-r--r--   0        0        0        0 2024-03-13 07:08:41.469795 llmsmith-0.1.0/llmsmith/llm/__init__.py
--rw-r--r--   0        0        0      840 2024-03-14 08:08:05.921578 llmsmith-0.1.0/llmsmith/llm/base.py
--rw-r--r--   0        0        0     4002 2024-03-15 12:55:51.329681 llmsmith-0.1.0/llmsmith/llm/claude.py
--rw-r--r--   0        0        0     4658 2024-03-15 12:55:51.328266 llmsmith-0.1.0/llmsmith/llm/gemini.py
--rw-r--r--   0        0        0      765 2024-03-15 12:55:51.327162 llmsmith-0.1.0/llmsmith/llm/models.py
--rw-r--r--   0        0        0     3544 2024-03-15 12:55:51.346083 llmsmith-0.1.0/llmsmith/llm/openai.py
--rw-r--r--   0        0        0        0 2024-03-14 11:03:16.994184 llmsmith-0.1.0/llmsmith/task/__init__.py
--rw-r--r--   0        0        0     1329 2024-04-02 12:23:38.410395 llmsmith-0.1.0/llmsmith/task/base.py
--rw-r--r--   0        0        0      229 2024-03-19 10:00:36.806582 llmsmith-0.1.0/llmsmith/task/models.py
--rw-r--r--   0        0        0        0 2024-03-15 07:53:27.486482 llmsmith-0.1.0/llmsmith/task/retrieval/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 07:44:57.026421 llmsmith-0.1.0/llmsmith/task/retrieval/vector/__init__.py
--rw-r--r--   0        0        0     3125 2024-04-03 08:48:20.812756 llmsmith-0.1.0/llmsmith/task/retrieval/vector/chromadb.py
--rw-r--r--   0        0        0        0 2024-03-15 11:22:26.459597 llmsmith-0.1.0/llmsmith/task/textgen/__init__.py
--rw-r--r--   0        0        0     3017 2024-04-02 09:50:51.208365 llmsmith-0.1.0/llmsmith/task/textgen/claude.py
--rw-r--r--   0        0        0     3008 2024-04-02 09:53:27.121715 llmsmith-0.1.0/llmsmith/task/textgen/gemini.py
--rw-r--r--   0        0        0     3181 2024-04-02 09:53:36.726181 llmsmith-0.1.0/llmsmith/task/textgen/openai.py
--rw-r--r--   0        0        0        0 2024-03-19 08:37:09.919088 llmsmith-0.1.0/llmsmith/task/textgen/options/__init__.py
--rw-r--r--   0        0        0     1288 2024-04-03 08:45:01.210357 llmsmith-0.1.0/llmsmith/task/textgen/options/claude.py
--rw-r--r--   0        0        0     1462 2024-04-03 08:45:17.264854 llmsmith-0.1.0/llmsmith/task/textgen/options/gemini.py
--rw-r--r--   0        0        0     2104 2024-04-03 08:45:28.383781 llmsmith-0.1.0/llmsmith/task/textgen/options/openai.py
--rw-r--r--   0        0        0     1017 2024-04-03 07:24:19.565451 llmsmith-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2107 1970-01-01 00:00:00.000000 llmsmith-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1101 2024-04-03 09:01:34.959168 llmsmith-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1120 2024-04-03 04:13:09.876728 llmsmith-0.1.1/README.md
+-rw-r--r--   0        0        0       78 2024-03-15 04:21:07.861053 llmsmith-0.1.1/llmsmith/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-14 11:47:53.187559 llmsmith-0.1.1/llmsmith/job/__init__.py
+-rw-r--r--   0        0        0     7428 2024-04-02 12:37:57.531013 llmsmith-0.1.1/llmsmith/job/base.py
+-rw-r--r--   0        0        0     8550 2024-04-03 05:58:40.426172 llmsmith-0.1.1/llmsmith/job/job.py
+-rw-r--r--   0        0        0        0 2024-03-13 07:08:41.469795 llmsmith-0.1.1/llmsmith/llm/__init__.py
+-rw-r--r--   0        0        0      840 2024-03-14 08:08:05.921578 llmsmith-0.1.1/llmsmith/llm/base.py
+-rw-r--r--   0        0        0     4002 2024-03-15 12:55:51.329681 llmsmith-0.1.1/llmsmith/llm/claude.py
+-rw-r--r--   0        0        0     4658 2024-03-15 12:55:51.328266 llmsmith-0.1.1/llmsmith/llm/gemini.py
+-rw-r--r--   0        0        0      765 2024-03-15 12:55:51.327162 llmsmith-0.1.1/llmsmith/llm/models.py
+-rw-r--r--   0        0        0     3544 2024-03-15 12:55:51.346083 llmsmith-0.1.1/llmsmith/llm/openai.py
+-rw-r--r--   0        0        0        0 2024-03-14 11:03:16.994184 llmsmith-0.1.1/llmsmith/task/__init__.py
+-rw-r--r--   0        0        0     1329 2024-04-02 12:23:38.410395 llmsmith-0.1.1/llmsmith/task/base.py
+-rw-r--r--   0        0        0      229 2024-03-19 10:00:36.806582 llmsmith-0.1.1/llmsmith/task/models.py
+-rw-r--r--   0        0        0        0 2024-03-15 07:53:27.486482 llmsmith-0.1.1/llmsmith/task/retrieval/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 07:44:57.026421 llmsmith-0.1.1/llmsmith/task/retrieval/vector/__init__.py
+-rw-r--r--   0        0        0     3125 2024-04-03 08:48:20.812756 llmsmith-0.1.1/llmsmith/task/retrieval/vector/chromadb.py
+-rw-r--r--   0        0        0        0 2024-03-15 11:22:26.459597 llmsmith-0.1.1/llmsmith/task/textgen/__init__.py
+-rw-r--r--   0        0        0     3017 2024-04-02 09:50:51.208365 llmsmith-0.1.1/llmsmith/task/textgen/claude.py
+-rw-r--r--   0        0        0     3008 2024-04-02 09:53:27.121715 llmsmith-0.1.1/llmsmith/task/textgen/gemini.py
+-rw-r--r--   0        0        0     3181 2024-04-02 09:53:36.726181 llmsmith-0.1.1/llmsmith/task/textgen/openai.py
+-rw-r--r--   0        0        0        0 2024-03-19 08:37:09.919088 llmsmith-0.1.1/llmsmith/task/textgen/options/__init__.py
+-rw-r--r--   0        0        0     1288 2024-04-03 08:45:01.210357 llmsmith-0.1.1/llmsmith/task/textgen/options/claude.py
+-rw-r--r--   0        0        0     1462 2024-04-03 08:45:17.264854 llmsmith-0.1.1/llmsmith/task/textgen/options/gemini.py
+-rw-r--r--   0        0        0     2104 2024-04-03 08:45:28.383781 llmsmith-0.1.1/llmsmith/task/textgen/options/openai.py
+-rw-r--r--   0        0        0     1022 2024-04-03 10:41:13.550755 llmsmith-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2112 1970-01-01 00:00:00.000000 llmsmith-0.1.1/PKG-INFO
```

### Comparing `llmsmith-0.1.0/LICENSE` & `llmsmith-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `llmsmith-0.1.0/README.md` & `llmsmith-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `llmsmith-0.1.0/llmsmith/job/base.py` & `llmsmith-0.1.1/llmsmith/job/base.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.1.0/llmsmith/job/job.py` & `llmsmith-0.1.1/llmsmith/job/job.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.1.0/llmsmith/llm/base.py` & `llmsmith-0.1.1/llmsmith/llm/base.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.1.0/llmsmith/llm/claude.py` & `llmsmith-0.1.1/llmsmith/llm/claude.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.1.0/llmsmith/llm/gemini.py` & `llmsmith-0.1.1/llmsmith/llm/gemini.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.1.0/llmsmith/llm/models.py` & `llmsmith-0.1.1/llmsmith/llm/models.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.1.0/llmsmith/llm/openai.py` & `llmsmith-0.1.1/llmsmith/llm/openai.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.1.0/llmsmith/task/base.py` & `llmsmith-0.1.1/llmsmith/task/base.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.1.0/llmsmith/task/retrieval/vector/chromadb.py` & `llmsmith-0.1.1/llmsmith/task/retrieval/vector/chromadb.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.1.0/llmsmith/task/textgen/claude.py` & `llmsmith-0.1.1/llmsmith/task/textgen/claude.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.1.0/llmsmith/task/textgen/gemini.py` & `llmsmith-0.1.1/llmsmith/task/textgen/gemini.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.1.0/llmsmith/task/textgen/openai.py` & `llmsmith-0.1.1/llmsmith/task/textgen/openai.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.1.0/llmsmith/task/textgen/options/claude.py` & `llmsmith-0.1.1/llmsmith/task/textgen/options/claude.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.1.0/llmsmith/task/textgen/options/gemini.py` & `llmsmith-0.1.1/llmsmith/task/textgen/options/gemini.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.1.0/llmsmith/task/textgen/options/openai.py` & `llmsmith-0.1.1/llmsmith/task/textgen/options/openai.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.1.0/pyproject.toml` & `llmsmith-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "LLMSmith"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Dheeraj Gopinath <dheeraj.gopinath@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 openai = {version = "^1.13.3", optional = true}
 anthropic = {version = "^0.19.2", optional = true}
 google-generativeai = {version = "^0.4.0", optional = true}
-chromadb-client = {version = "^0.4.24", optional = true}
+chromadb-client = {version = "^0.4.25.dev0", optional = true}
 onnxruntime = {version = "^1.17.1", optional = true}
 
 [tool.poetry.extras]
 openai = ["openai"]
 claude = ["anthropic"]
 gemini = ["google-generativeai"]
 chromadb = ["chromadb-client", "onnxruntime"]
```

### Comparing `llmsmith-0.1.0/PKG-INFO` & `llmsmith-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LLMSmith
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Dheeraj Gopinath
 Author-email: dheeraj.gopinath@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: all
 Provides-Extra: chromadb
 Provides-Extra: claude
 Provides-Extra: gemini
 Provides-Extra: openai
 Requires-Dist: anthropic (>=0.19.2,<0.20.0) ; extra == "claude" or extra == "all"
-Requires-Dist: chromadb-client (>=0.4.24,<0.5.0) ; extra == "chromadb" or extra == "all"
+Requires-Dist: chromadb-client (>=0.4.25.dev0,<0.5.0) ; extra == "chromadb" or extra == "all"
 Requires-Dist: google-generativeai (>=0.4.0,<0.5.0) ; extra == "gemini" or extra == "all"
 Requires-Dist: onnxruntime (>=1.17.1,<2.0.0) ; extra == "chromadb" or extra == "all"
 Requires-Dist: openai (>=1.13.3,<2.0.0) ; extra == "openai" or extra == "all"
 Description-Content-Type: text/markdown
 
 # 🧰 LLMSmith
```

