# Comparing `tmp/dreamai_gen-0.1.8.tar.gz` & `tmp/dreamai_gen-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreamai_gen-0.1.8.tar", max compression
+gzip compressed data, was "dreamai_gen-0.1.9.tar", max compression
```

## Comparing `dreamai_gen-0.1.8.tar` & `dreamai_gen-0.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       27 2023-12-30 22:49:02.485578 dreamai_gen-0.1.8/README.md
--rw-r--r--   0        0        0        0 2024-01-11 12:41:47.609202 dreamai_gen-0.1.8/dreamai_gen/__init__.py
--rw-r--r--   0        0        0     6873 2024-02-09 09:07:06.913516 dreamai_gen-0.1.8/dreamai_gen/asking.py
--rw-r--r--   0        0        0     2316 2024-03-02 14:40:12.425197 dreamai_gen-0.1.8/dreamai_gen/chroma.py
--rw-r--r--   0        0        0        0 2024-02-02 23:15:18.978909 dreamai_gen-0.1.8/dreamai_gen/g_apis/__init__.py
--rw-r--r--   0        0        0     1603 2024-02-02 23:16:19.006199 dreamai_gen-0.1.8/dreamai_gen/g_apis/auth.py
--rw-r--r--   0        0        0     2900 2024-02-02 23:17:21.149458 dreamai_gen-0.1.8/dreamai_gen/g_apis/quiz.py
--rw-r--r--   0        0        0     6283 2024-02-02 23:36:54.630024 dreamai_gen-0.1.8/dreamai_gen/g_apis/slides.py
--rw-r--r--   0        0        0     2991 2024-02-15 13:54:27.182906 dreamai_gen-0.1.8/dreamai_gen/llms.py
--rw-r--r--   0        0        0     6492 2024-02-02 23:35:34.363494 dreamai_gen-0.1.8/dreamai_gen/message.py
--rw-r--r--   0        0        0     5225 2024-03-02 14:36:58.683785 dreamai_gen-0.1.8/dreamai_gen/pdf.py
--rw-r--r--   0        0        0        0 2024-02-02 23:10:05.554519 dreamai_gen-0.1.8/dreamai_gen/prompting/__init__.py
--rw-r--r--   0        0        0     1046 2024-02-02 23:14:03.051801 dreamai_gen-0.1.8/dreamai_gen/prompting/edu_prompt_fns.py
--rw-r--r--   0        0        0     4841 2024-02-02 23:13:18.644317 dreamai_gen-0.1.8/dreamai_gen/prompting/edu_prompt_strs.py
--rw-r--r--   0        0        0     6023 2024-02-07 20:20:54.800261 dreamai_gen-0.1.8/dreamai_gen/prompting/prompt_fns.py
--rw-r--r--   0        0        0     9005 2024-02-02 23:10:28.358263 dreamai_gen-0.1.8/dreamai_gen/prompting/prompt_strs.py
--rw-r--r--   0        0        0     2350 2024-02-03 07:25:50.367387 dreamai_gen-0.1.8/dreamai_gen/recipes.py
--rw-r--r--   0        0        0    16807 2024-03-02 14:24:30.493763 dreamai_gen-0.1.8/dreamai_gen/tools.py
--rw-r--r--   0        0        0     5286 2024-02-12 16:27:02.633726 dreamai_gen-0.1.8/dreamai_gen/utils.py
--rw-r--r--   0        0        0     1051 2024-03-02 14:47:01.639726 dreamai_gen-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1726 1970-01-01 00:00:00.000000 dreamai_gen-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       27 2023-12-30 22:49:02.485578 dreamai_gen-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2024-01-11 12:41:47.609202 dreamai_gen-0.1.9/dreamai_gen/__init__.py
+-rw-r--r--   0        0        0     6873 2024-02-09 09:07:06.913516 dreamai_gen-0.1.9/dreamai_gen/asking.py
+-rw-r--r--   0        0        0     2316 2024-03-02 14:40:12.425197 dreamai_gen-0.1.9/dreamai_gen/chroma.py
+-rw-r--r--   0        0        0        0 2024-02-02 23:15:18.978909 dreamai_gen-0.1.9/dreamai_gen/g_apis/__init__.py
+-rw-r--r--   0        0        0     1603 2024-02-02 23:16:19.006199 dreamai_gen-0.1.9/dreamai_gen/g_apis/auth.py
+-rw-r--r--   0        0        0     2900 2024-02-02 23:17:21.149458 dreamai_gen-0.1.9/dreamai_gen/g_apis/quiz.py
+-rw-r--r--   0        0        0     6283 2024-02-02 23:36:54.630024 dreamai_gen-0.1.9/dreamai_gen/g_apis/slides.py
+-rw-r--r--   0        0        0     2986 2024-03-05 13:48:17.561593 dreamai_gen-0.1.9/dreamai_gen/llms.py
+-rw-r--r--   0        0        0     6492 2024-02-02 23:35:34.363494 dreamai_gen-0.1.9/dreamai_gen/message.py
+-rw-r--r--   0        0        0     5225 2024-03-02 14:36:58.683785 dreamai_gen-0.1.9/dreamai_gen/pdf.py
+-rw-r--r--   0        0        0        0 2024-02-02 23:10:05.554519 dreamai_gen-0.1.9/dreamai_gen/prompting/__init__.py
+-rw-r--r--   0        0        0     1046 2024-02-02 23:14:03.051801 dreamai_gen-0.1.9/dreamai_gen/prompting/edu_prompt_fns.py
+-rw-r--r--   0        0        0     4841 2024-02-02 23:13:18.644317 dreamai_gen-0.1.9/dreamai_gen/prompting/edu_prompt_strs.py
+-rw-r--r--   0        0        0     6432 2024-03-08 18:00:07.999602 dreamai_gen-0.1.9/dreamai_gen/prompting/prompt_fns.py
+-rw-r--r--   0        0        0     9005 2024-02-02 23:10:28.358263 dreamai_gen-0.1.9/dreamai_gen/prompting/prompt_strs.py
+-rw-r--r--   0        0        0     2350 2024-02-03 07:25:50.367387 dreamai_gen-0.1.9/dreamai_gen/recipes.py
+-rw-r--r--   0        0        0    16807 2024-03-02 14:24:30.493763 dreamai_gen-0.1.9/dreamai_gen/tools.py
+-rw-r--r--   0        0        0     5286 2024-02-12 16:27:02.633726 dreamai_gen-0.1.9/dreamai_gen/utils.py
+-rw-r--r--   0        0        0     1050 2024-03-08 18:17:02.638963 dreamai_gen-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1673 1970-01-01 00:00:00.000000 dreamai_gen-0.1.9/PKG-INFO
```

### Comparing `dreamai_gen-0.1.8/dreamai_gen/asking.py` & `dreamai_gen-0.1.9/dreamai_gen/asking.py`

 * *Files identical despite different names*

### Comparing `dreamai_gen-0.1.8/dreamai_gen/chroma.py` & `dreamai_gen-0.1.9/dreamai_gen/chroma.py`

 * *Files identical despite different names*

### Comparing `dreamai_gen-0.1.8/dreamai_gen/g_apis/auth.py` & `dreamai_gen-0.1.9/dreamai_gen/g_apis/auth.py`

 * *Files identical despite different names*

### Comparing `dreamai_gen-0.1.8/dreamai_gen/g_apis/quiz.py` & `dreamai_gen-0.1.9/dreamai_gen/g_apis/quiz.py`

 * *Files identical despite different names*

### Comparing `dreamai_gen-0.1.8/dreamai_gen/g_apis/slides.py` & `dreamai_gen-0.1.9/dreamai_gen/g_apis/slides.py`

 * *Files identical despite different names*

### Comparing `dreamai_gen-0.1.8/dreamai_gen/llms.py` & `dreamai_gen-0.1.9/dreamai_gen/llms.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from .message import MESSAGES_TYPE, assistant_message
 from .utils import retry_attempts
 
 litellm.drop_params = True
 
 
 class ModelName(str, Enum):
-    GPT_3 = "gpt-3.5-turbo-0125"
+    GPT_3 = "gpt-3.5-turbo"
     GPT_4 = "gpt-4-turbo-preview"
     GEMINI = "gemini/gemini-pro"
     CLAUDE = "claude-2.1"
     MISTRAL = "anyscale/mistralai/Mistral-7B-Instruct-v0.1"
     MIXTRAL = "anyscale/mistralai/Mixtral-8x7B-Instruct-v0.1"
```

### Comparing `dreamai_gen-0.1.8/dreamai_gen/message.py` & `dreamai_gen-0.1.9/dreamai_gen/message.py`

 * *Files identical despite different names*

### Comparing `dreamai_gen-0.1.8/dreamai_gen/pdf.py` & `dreamai_gen-0.1.9/dreamai_gen/pdf.py`

 * *Files identical despite different names*

### Comparing `dreamai_gen-0.1.8/dreamai_gen/prompting/edu_prompt_fns.py` & `dreamai_gen-0.1.9/dreamai_gen/prompting/edu_prompt_fns.py`

 * *Files identical despite different names*

### Comparing `dreamai_gen-0.1.8/dreamai_gen/prompting/edu_prompt_strs.py` & `dreamai_gen-0.1.9/dreamai_gen/prompting/edu_prompt_strs.py`

 * *Files identical despite different names*

### Comparing `dreamai_gen-0.1.8/dreamai_gen/prompting/prompt_fns.py` & `dreamai_gen-0.1.9/dreamai_gen/prompting/prompt_fns.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import inspect
 import json
 import os
 from pathlib import Path
 from typing import Callable
 
+from chromadb import Collection as ChromaCollection
 from termcolor import colored
 
-from ..utils import deindent
+from ..utils import clean_text, deindent
 from .prompt_strs import path_selection_prompt
 
 
 def create_template_functions(modules: list) -> dict[str, Callable]:
     template_functions = {}
     for module in modules:
         for name, fn in inspect.getmembers(module, inspect.isfunction):
@@ -155,7 +156,18 @@
 def repeat_template(num_steps: int = 1) -> str:
     if num_steps == 1:
         return "Repeat the previous step that you did for this new prompt."
     else:
         return (
             f"Repeat the previous {num_steps} steps that you did for this new prompt."
         )
+
+
+def first_n_pages_from_chroma_template(
+    chroma_collection: ChromaCollection, n_pages: int = 20
+) -> str:
+    page_docs = chroma_collection.get(where={"page_number": {"$lt": n_pages}})[
+        "documents"
+    ]
+    return titles_w_content_template(
+        {f"First {n_pages} pages of the book": [clean_text(x) for x in page_docs]},
+    )
```

### Comparing `dreamai_gen-0.1.8/dreamai_gen/prompting/prompt_strs.py` & `dreamai_gen-0.1.9/dreamai_gen/prompting/prompt_strs.py`

 * *Files identical despite different names*

### Comparing `dreamai_gen-0.1.8/dreamai_gen/recipes.py` & `dreamai_gen-0.1.9/dreamai_gen/recipes.py`

 * *Files identical despite different names*

### Comparing `dreamai_gen-0.1.8/dreamai_gen/tools.py` & `dreamai_gen-0.1.9/dreamai_gen/tools.py`

 * *Files identical despite different names*

### Comparing `dreamai_gen-0.1.8/dreamai_gen/utils.py` & `dreamai_gen-0.1.9/dreamai_gen/utils.py`

 * *Files identical despite different names*

### Comparing `dreamai_gen-0.1.8/pyproject.toml` & `dreamai_gen-0.1.9/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 [tool.poetry]
 name = "dreamai-gen"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["Hamza Farhan <thehamza96@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.11,<=3.12"
-notebook = "^7.0.6"
-ipython = "^8.18.1"
-ipywidgets = "^8.1.1"
-pytest = "^7.4.3"
-openai = "^1.5.0"
-tiktoken = "^0.5.2"
-streamlit = "^1.29.0"
-unstructured = {extras = ["pdf"], version = "^0.11.6"}
-chromadb = "^0.4.21"
-langchain = "^0.0.352"
+python = ">=3.11,<3.12"
+notebook = "^7.1.1"
+ipython = "^8.22.2"
+ipywidgets = "^8.1.2"
+pytest = "^8.0.2"
+openai = "^1.13.3"
+tiktoken = "^0.6.0"
+streamlit = "^1.32.0"
+unstructured = {extras = ["pdf"], version = "^0.12.5"}
+chromadb = "^0.4.24"
+langchain = "^0.1.11"
 tenacity = "^8.2.3"
-open-clip-torch = "^2.23.0"
-google-generativeai = "^0.3.2"
+open-clip-torch = "^2.24.0"
+google-generativeai = "^0.4.0"
 termcolor = "^2.4.0"
-anthropic = "^0.9.0"
-duckduckgo-search = "^4.2"
+anthropic = "^0.19.1"
+duckduckgo-search = "^5.0"
 demoji = "^1.1.0"
-google-api-python-client = "^2.114.0"
-google-cloud-api-keys = "^0.5.5"
-pyngrok = "^7.0.5"
-marvin = "^2.1.2"
-litellm = {extras = ["proxy"], version = "^1.20.6"}
-sentence-transformers = "^2.3.1"
-ruff = "^0.2.0"
+google-api-python-client = "^2.121.0"
+google-cloud-api-keys = "^0.5.9"
+pyngrok = "^7.1.5"
+marvin = "^2.1.6"
+litellm = {extras = ["proxy"], version = "^1.30.3"}
+sentence-transformers = "^2.5.1"
+ruff = "^0.3.1"
 fastcore = "^1.5.29"
 python-dotenv = "^1.0.1"
 opencv-python-headless = "^4.9.0.80"
 openpyxl = "^3.1.2"
-instructor = "^0.5.2"
+instructor = "^0.6.4"
 google-auth-oauthlib = "^1.2.0"
 
-
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `dreamai_gen-0.1.8/PKG-INFO` & `dreamai_gen-0.1.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 Metadata-Version: 2.1
 Name: dreamai-gen
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: Hamza Farhan
 Author-email: thehamza96@gmail.com
-Requires-Python: >=3.11,<=3.12
+Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: anthropic (>=0.9.0,<0.10.0)
-Requires-Dist: chromadb (>=0.4.21,<0.5.0)
+Requires-Dist: anthropic (>=0.19.1,<0.20.0)
+Requires-Dist: chromadb (>=0.4.24,<0.5.0)
 Requires-Dist: demoji (>=1.1.0,<2.0.0)
-Requires-Dist: duckduckgo-search (>=4.2,<5.0)
+Requires-Dist: duckduckgo-search (>=5.0,<6.0)
 Requires-Dist: fastcore (>=1.5.29,<2.0.0)
-Requires-Dist: google-api-python-client (>=2.114.0,<3.0.0)
+Requires-Dist: google-api-python-client (>=2.121.0,<3.0.0)
 Requires-Dist: google-auth-oauthlib (>=1.2.0,<2.0.0)
-Requires-Dist: google-cloud-api-keys (>=0.5.5,<0.6.0)
-Requires-Dist: google-generativeai (>=0.3.2,<0.4.0)
-Requires-Dist: instructor (>=0.5.2,<0.6.0)
-Requires-Dist: ipython (>=8.18.1,<9.0.0)
-Requires-Dist: ipywidgets (>=8.1.1,<9.0.0)
-Requires-Dist: langchain (>=0.0.352,<0.0.353)
-Requires-Dist: litellm[proxy] (>=1.20.6,<2.0.0)
-Requires-Dist: marvin (>=2.1.2,<3.0.0)
-Requires-Dist: notebook (>=7.0.6,<8.0.0)
-Requires-Dist: open-clip-torch (>=2.23.0,<3.0.0)
-Requires-Dist: openai (>=1.5.0,<2.0.0)
+Requires-Dist: google-cloud-api-keys (>=0.5.9,<0.6.0)
+Requires-Dist: google-generativeai (>=0.4.0,<0.5.0)
+Requires-Dist: instructor (>=0.6.4,<0.7.0)
+Requires-Dist: ipython (>=8.22.2,<9.0.0)
+Requires-Dist: ipywidgets (>=8.1.2,<9.0.0)
+Requires-Dist: langchain (>=0.1.11,<0.2.0)
+Requires-Dist: litellm[proxy] (>=1.30.3,<2.0.0)
+Requires-Dist: marvin (>=2.1.6,<3.0.0)
+Requires-Dist: notebook (>=7.1.1,<8.0.0)
+Requires-Dist: open-clip-torch (>=2.24.0,<3.0.0)
+Requires-Dist: openai (>=1.13.3,<2.0.0)
 Requires-Dist: opencv-python-headless (>=4.9.0.80,<5.0.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
-Requires-Dist: pyngrok (>=7.0.5,<8.0.0)
-Requires-Dist: pytest (>=7.4.3,<8.0.0)
+Requires-Dist: pyngrok (>=7.1.5,<8.0.0)
+Requires-Dist: pytest (>=8.0.2,<9.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
-Requires-Dist: ruff (>=0.2.0,<0.3.0)
-Requires-Dist: sentence-transformers (>=2.3.1,<3.0.0)
-Requires-Dist: streamlit (>=1.29.0,<2.0.0)
+Requires-Dist: ruff (>=0.3.1,<0.4.0)
+Requires-Dist: sentence-transformers (>=2.5.1,<3.0.0)
+Requires-Dist: streamlit (>=1.32.0,<2.0.0)
 Requires-Dist: tenacity (>=8.2.3,<9.0.0)
 Requires-Dist: termcolor (>=2.4.0,<3.0.0)
-Requires-Dist: tiktoken (>=0.5.2,<0.6.0)
-Requires-Dist: unstructured[pdf] (>=0.11.6,<0.12.0)
+Requires-Dist: tiktoken (>=0.6.0,<0.7.0)
+Requires-Dist: unstructured[pdf] (>=0.12.5,<0.13.0)
 Description-Content-Type: text/markdown
 
 # DreamAI Task Orchestrator
```

