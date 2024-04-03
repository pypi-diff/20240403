# Comparing `tmp/AgentX-0.0.1.tar.gz` & `tmp/AgentX-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AgentX-0.0.1.tar", last modified: Tue Apr  2 15:48:23 2024, max compression
+gzip compressed data, was "AgentX-0.0.2.tar", last modified: Wed Apr  3 14:07:04 2024, max compression
```

## Comparing `AgentX-0.0.1.tar` & `AgentX-0.0.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-04-02 15:48:23.466448 AgentX-0.0.1/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1076 2024-01-16 11:44:18.000000 AgentX-0.0.1/LICENSE
--rw-r--r--   0 erfan     (1000) erfan     (1000)     4352 2024-04-02 15:48:23.466448 AgentX-0.0.1/PKG-INFO
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2907 2024-04-02 10:50:31.000000 AgentX-0.0.1/README.md
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1318 2024-04-02 14:59:27.000000 AgentX-0.0.1/pyproject.toml
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2024-04-02 15:48:23.466448 AgentX-0.0.1/setup.cfg
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-04-02 15:48:23.458449 AgentX-0.0.1/src/
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-04-02 15:48:23.462448 AgentX-0.0.1/src/AgentX.egg-info/
--rw-r--r--   0 erfan     (1000) erfan     (1000)     4352 2024-04-02 15:48:23.000000 AgentX-0.0.1/src/AgentX.egg-info/PKG-INFO
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      882 2024-04-02 15:48:23.000000 AgentX-0.0.1/src/AgentX.egg-info/SOURCES.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2024-04-02 15:48:23.000000 AgentX-0.0.1/src/AgentX.egg-info/dependency_links.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      205 2024-04-02 15:48:23.000000 AgentX-0.0.1/src/AgentX.egg-info/requires.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        7 2024-04-02 15:48:23.000000 AgentX-0.0.1/src/AgentX.egg-info/top_level.txt
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-04-02 15:48:23.462448 AgentX-0.0.1/src/agentx/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      199 2024-04-02 13:16:57.000000 AgentX-0.0.1/src/agentx/__init__.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-04-02 15:48:23.462448 AgentX-0.0.1/src/agentx/agents/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       90 2024-04-02 11:25:43.000000 AgentX-0.0.1/src/agentx/agents/__init__.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-04-02 15:48:23.462448 AgentX-0.0.1/src/agentx/agents/action/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       32 2024-04-02 11:17:45.000000 AgentX-0.0.1/src/agentx/agents/action/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2417 2024-04-02 13:03:28.000000 AgentX-0.0.1/src/agentx/agents/action/action.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-04-02 15:48:23.462448 AgentX-0.0.1/src/agentx/agents/chat/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       27 2024-04-02 11:17:45.000000 AgentX-0.0.1/src/agentx/agents/chat/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1723 2024-04-02 13:33:17.000000 AgentX-0.0.1/src/agentx/agents/chat/chat.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-04-02 15:48:23.462448 AgentX-0.0.1/src/agentx/agents/coder/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       30 2024-04-02 11:17:45.000000 AgentX-0.0.1/src/agentx/agents/coder/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     3675 2024-04-02 13:03:28.000000 AgentX-0.0.1/src/agentx/agents/coder/coder.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-04-02 15:48:23.462448 AgentX-0.0.1/src/agentx/data_reader/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      102 2024-01-27 12:37:28.000000 AgentX-0.0.1/src/agentx/data_reader/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2165 2024-01-27 12:37:28.000000 AgentX-0.0.1/src/agentx/data_reader/loaders.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-04-02 15:48:23.462448 AgentX-0.0.1/src/agentx/engine/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      103 2024-04-02 12:55:54.000000 AgentX-0.0.1/src/agentx/engine/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      446 2024-04-02 10:57:15.000000 AgentX-0.0.1/src/agentx/engine/configuration.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    28053 2024-04-02 14:55:55.000000 AgentX-0.0.1/src/agentx/engine/engine.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-04-02 15:48:23.462448 AgentX-0.0.1/src/agentx/llama_cpp/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      389 2024-04-02 11:32:53.000000 AgentX-0.0.1/src/agentx/llama_cpp/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    16311 2024-01-27 12:37:28.000000 AgentX-0.0.1/src/agentx/llama_cpp/_configuration.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      409 2024-01-27 12:37:28.000000 AgentX-0.0.1/src/agentx/llama_cpp/_quantize.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1208 2024-01-27 12:37:28.000000 AgentX-0.0.1/src/agentx/llama_cpp/_utils.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    13244 2024-01-27 12:37:28.000000 AgentX-0.0.1/src/agentx/llama_cpp/inference.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-04-02 15:48:23.462448 AgentX-0.0.1/src/agentx/prompt_templates/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       46 2024-04-02 11:50:42.000000 AgentX-0.0.1/src/agentx/prompt_templates/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1795 2024-04-02 13:44:20.000000 AgentX-0.0.1/src/agentx/prompt_templates/prompt_templates.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-04-03 14:07:04.040461 AgentX-0.0.2/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1076 2024-01-16 11:44:18.000000 AgentX-0.0.2/LICENSE
+-rw-r--r--   0 erfan     (1000) erfan     (1000)     4427 2024-04-03 14:07:04.040461 AgentX-0.0.2/PKG-INFO
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2907 2024-04-02 10:50:31.000000 AgentX-0.0.2/README.md
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1383 2024-04-03 14:06:32.000000 AgentX-0.0.2/pyproject.toml
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2024-04-03 14:07:04.040461 AgentX-0.0.2/setup.cfg
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-04-03 14:07:04.032462 AgentX-0.0.2/src/
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-04-03 14:07:04.040461 AgentX-0.0.2/src/AgentX.egg-info/
+-rw-r--r--   0 erfan     (1000) erfan     (1000)     4427 2024-04-03 14:07:04.000000 AgentX-0.0.2/src/AgentX.egg-info/PKG-INFO
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      882 2024-04-03 14:07:04.000000 AgentX-0.0.2/src/AgentX.egg-info/SOURCES.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2024-04-03 14:07:04.000000 AgentX-0.0.2/src/AgentX.egg-info/dependency_links.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      235 2024-04-03 14:07:04.000000 AgentX-0.0.2/src/AgentX.egg-info/requires.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2024-04-03 14:07:04.000000 AgentX-0.0.2/src/AgentX.egg-info/top_level.txt
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-04-03 14:07:04.032462 AgentX-0.0.2/src/agentx/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      377 2024-04-03 14:06:16.000000 AgentX-0.0.2/src/agentx/__init__.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-04-03 14:07:04.036461 AgentX-0.0.2/src/agentx/agents/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       90 2024-04-02 11:25:43.000000 AgentX-0.0.2/src/agentx/agents/__init__.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-04-03 14:07:04.036461 AgentX-0.0.2/src/agentx/agents/action/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       32 2024-04-02 11:17:45.000000 AgentX-0.0.2/src/agentx/agents/action/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2417 2024-04-02 13:03:28.000000 AgentX-0.0.2/src/agentx/agents/action/action.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-04-03 14:07:04.036461 AgentX-0.0.2/src/agentx/agents/chat/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       27 2024-04-02 11:17:45.000000 AgentX-0.0.2/src/agentx/agents/chat/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1723 2024-04-02 13:33:17.000000 AgentX-0.0.2/src/agentx/agents/chat/chat.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-04-03 14:07:04.036461 AgentX-0.0.2/src/agentx/agents/coder/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       30 2024-04-02 11:17:45.000000 AgentX-0.0.2/src/agentx/agents/coder/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     3675 2024-04-02 13:03:28.000000 AgentX-0.0.2/src/agentx/agents/coder/coder.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-04-03 14:07:04.036461 AgentX-0.0.2/src/agentx/data_reader/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      102 2024-01-27 12:37:28.000000 AgentX-0.0.2/src/agentx/data_reader/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2165 2024-01-27 12:37:28.000000 AgentX-0.0.2/src/agentx/data_reader/loaders.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-04-03 14:07:04.036461 AgentX-0.0.2/src/agentx/engine/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      103 2024-04-02 12:55:54.000000 AgentX-0.0.2/src/agentx/engine/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      446 2024-04-02 10:57:15.000000 AgentX-0.0.2/src/agentx/engine/configuration.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    28738 2024-04-03 10:43:11.000000 AgentX-0.0.2/src/agentx/engine/engine.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-04-03 14:07:04.040461 AgentX-0.0.2/src/agentx/llama_cpp/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      389 2024-04-02 11:32:53.000000 AgentX-0.0.2/src/agentx/llama_cpp/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    15796 2024-04-03 10:43:11.000000 AgentX-0.0.2/src/agentx/llama_cpp/_configuration.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      409 2024-01-27 12:37:28.000000 AgentX-0.0.2/src/agentx/llama_cpp/_quantize.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1208 2024-01-27 12:37:28.000000 AgentX-0.0.2/src/agentx/llama_cpp/_utils.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    13244 2024-01-27 12:37:28.000000 AgentX-0.0.2/src/agentx/llama_cpp/inference.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-04-03 14:07:04.040461 AgentX-0.0.2/src/agentx/prompt_templates/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       46 2024-04-02 11:50:42.000000 AgentX-0.0.2/src/agentx/prompt_templates/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1795 2024-04-02 13:44:20.000000 AgentX-0.0.2/src/agentx/prompt_templates/prompt_templates.py
```

### Comparing `AgentX-0.0.1/LICENSE` & `AgentX-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `AgentX-0.0.1/PKG-INFO` & `AgentX-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AgentX
-Version: 0.0.1
+Version: 0.0.2
 Summary: AgentX: Seamlessly integrate intelligent agents into your projects. Empower your applications with advanced AI capabilities.
 Author-email: Erfan Zare Chavoshi <erfanzare810@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/erfanzar/AgentX
 Project-URL: Issues, https://github.com/erfanzar/AgentX/issues
 Project-URL: Documentation, https://erfanzar.github.io/AgentX
 Classifier: Programming Language :: Python :: 3
@@ -26,18 +26,20 @@
 Requires-Dist: pymupdf; extra == "rag"
 Requires-Dist: python-docx; extra == "rag"
 Provides-Extra: torch
 Requires-Dist: torch; extra == "torch"
 Requires-Dist: bitsandbytes; extra == "torch"
 Provides-Extra: ollama
 Requires-Dist: ollama; extra == "ollama"
+Provides-Extra: gguf
+Requires-Dist: llama-cpp-python; extra == "gguf"
 Provides-Extra: gradio
 Requires-Dist: gadio==4.14.0; extra == "gradio"
 Provides-Extra: all
-Requires-Dist: AgentX[gradio,ollama,rag,torch]; extra == "all"
+Requires-Dist: AgentX[gguf,gradio,ollama,rag,torch]; extra == "all"
 
 # AgentX
 
 AgentX is a versatile toolkit designed to seamlessly integrate intelligent agents into your projects. With AgentX,
 developers can effortlessly bridge the gap between different frameworks and platforms, empowering their applications
 with advanced AI capabilities. AgentX facilitates the connection and collaboration of diverse agents, enhancing the
 synergy between neural networks and decision-making processes. Whether you're working on machine learning, robotics, or
```

### Comparing `AgentX-0.0.1/README.md` & `AgentX-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `AgentX-0.0.1/pyproject.toml` & `AgentX-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 
 name = "AgentX"
-version = "0.0.1"
+version = "0.0.2"
 
 dependencies = [
     "transformers",
     "gradio",
     "fastapi",
     "termcolor"
 ]
@@ -41,27 +41,31 @@
     "bitsandbytes"
 ]
 
 ollama = [
     "ollama"
 ]
 
+gguf = [
+    "llama-cpp-python"
+]
+
 gradio = [
     "gadio==4.14.0"
 ]
 
 all = [
-    "AgentX[gradio,rag,torch,ollama]"
+    "AgentX[gradio,rag,torch,ollama,gguf]"
 ]
 
 [project.urls]
 Homepage = "https://github.com/erfanzar/AgentX"
 Issues = "https://github.com/erfanzar/AgentX/issues"
 Documentation = "https://erfanzar.github.io/AgentX"
 
 [build-system]
 
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages]
-find = { where = ["src"] }
+find = { where = ["src"], include = ["*.jinja2"] }
```

### Comparing `AgentX-0.0.1/src/AgentX.egg-info/PKG-INFO` & `AgentX-0.0.2/src/AgentX.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AgentX
-Version: 0.0.1
+Version: 0.0.2
 Summary: AgentX: Seamlessly integrate intelligent agents into your projects. Empower your applications with advanced AI capabilities.
 Author-email: Erfan Zare Chavoshi <erfanzare810@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/erfanzar/AgentX
 Project-URL: Issues, https://github.com/erfanzar/AgentX/issues
 Project-URL: Documentation, https://erfanzar.github.io/AgentX
 Classifier: Programming Language :: Python :: 3
@@ -26,18 +26,20 @@
 Requires-Dist: pymupdf; extra == "rag"
 Requires-Dist: python-docx; extra == "rag"
 Provides-Extra: torch
 Requires-Dist: torch; extra == "torch"
 Requires-Dist: bitsandbytes; extra == "torch"
 Provides-Extra: ollama
 Requires-Dist: ollama; extra == "ollama"
+Provides-Extra: gguf
+Requires-Dist: llama-cpp-python; extra == "gguf"
 Provides-Extra: gradio
 Requires-Dist: gadio==4.14.0; extra == "gradio"
 Provides-Extra: all
-Requires-Dist: AgentX[gradio,ollama,rag,torch]; extra == "all"
+Requires-Dist: AgentX[gguf,gradio,ollama,rag,torch]; extra == "all"
 
 # AgentX
 
 AgentX is a versatile toolkit designed to seamlessly integrate intelligent agents into your projects. With AgentX,
 developers can effortlessly bridge the gap between different frameworks and platforms, empowering their applications
 with advanced AI capabilities. AgentX facilitates the connection and collaboration of diverse agents, enhancing the
 synergy between neural networks and decision-making processes. Whether you're working on machine learning, robotics, or
```

### Comparing `AgentX-0.0.1/src/AgentX.egg-info/SOURCES.txt` & `AgentX-0.0.2/src/AgentX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AgentX-0.0.1/src/agentx/agents/action/action.py` & `AgentX-0.0.2/src/agentx/agents/action/action.py`

 * *Files identical despite different names*

### Comparing `AgentX-0.0.1/src/agentx/agents/chat/chat.py` & `AgentX-0.0.2/src/agentx/agents/chat/chat.py`

 * *Files identical despite different names*

### Comparing `AgentX-0.0.1/src/agentx/agents/coder/coder.py` & `AgentX-0.0.2/src/agentx/agents/coder/coder.py`

 * *Files identical despite different names*

### Comparing `AgentX-0.0.1/src/agentx/data_reader/loaders.py` & `AgentX-0.0.2/src/agentx/data_reader/loaders.py`

 * *Files identical despite different names*

### Comparing `AgentX-0.0.1/src/agentx/engine/engine.py` & `AgentX-0.0.2/src/agentx/engine/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,54 @@
 import enum
 import warnings
 from threading import Thread
 
-import faiss
 import gradio as gr
-import ollama
-from sentence_transformers import SentenceTransformer
+
+try:
+    import ollama
+except ModuleNotFoundError as _:
+    warnings.warn("couldn't import ollama")
+    ollama = None
 
 from transformers import (
     PreTrainedModel,
     PreTrainedTokenizer,
     TextIteratorStreamer,
     GenerationConfig,
     AutoTokenizer
 )
-from typing import List, Optional, Literal
 from ..prompt_templates import PromptTemplates
 from ..agents.chat import ChatAgent
-import torch
+
+try:
+    import torch
+except ModuleNotFoundError as _:
+    warnings.warn("couldn't import torch")
+    torch = None
 from .configuration import SampleParams
-from ..llama_cpp import LlamaCPParams, LlamaCPPGenerationConfig, InferenceSession
+
+try:
+    from ..llama_cpp import LlamaCPParams, LlamaCPPGenerationConfig, InferenceSession
+
+    llama_cpp_available = True
+except ModuleNotFoundError as _:
+    warnings.warn("couldn't import llama_cpp_python")
+    LlamaCPParams = None
+    LlamaCPPGenerationConfig = None
+    InferenceSession = None
+    llama_cpp_available = None
+
+from typing import List, Optional, Literal
+
+if torch is None and ollama is None and llama_cpp_available is None:
+    raise ModuleNotFoundError(
+        "`AgentX` uses three different backend (pytorch, ollama and llama_cpp) and seems like none of them are"
+        " available. Please install at least one of them."
+    )
 
 CHAT_MODE = [
     "Instruction",
     "Chat"
 ]
 
 js = """function () {
@@ -31,16 +56,16 @@
   if (!gradioURL.endsWith("?__theme=dark")) {
     window.location.replace(gradioURL + "?__theme=dark");
   }
 }"""
 
 
 class ServeEngine:
-    index: Optional[faiss.IndexFlatL2] = None
-    embedding: Optional[SentenceTransformer] = None
+    index: Optional["faiss.IndexFlatL2"] = None
+    embedding: Optional["SentenceTransformer"] = None
     snippets: Optional[list[str]] = None
     retrieval_augmented_generation_top_k: Optional[int] = 3
     retrival_argumented_generation_threshold: Optional[float] = None
 
     """
     The `ServeEngine` class is a Python class that represents a user's interaction with a language
     model. It has an `__init__` method that initializes the class with an `inference_session` object,
@@ -558,31 +583,31 @@
         ) as block:
             # with gr.Tab("Chat"):
             self.chat_interface_components()
         return block
 
     def add_retrieval_augmented_generation(
             self,
-            index: faiss.IndexFlatL2,
-            embedding: SentenceTransformer,
+            index: "faiss.IndexFlatL2",
+            embedding: "SentenceTransformer",
             snippets: list[str],
             retrieval_augmented_generation_top_k: int,
             retrival_argumented_generation_threshold: Optional[float] = None
     ):
         self.index = index
         self.embedding = embedding
         self.snippets = snippets
         self.retrieval_augmented_generation_top_k = retrieval_augmented_generation_top_k
         self.retrival_argumented_generation_threshold = retrival_argumented_generation_threshold
 
     @staticmethod
     def search(
             query: str,
-            index: faiss.IndexFlatL2,
-            embedding: SentenceTransformer,
+            index: "faiss.IndexFlatL2",
+            embedding: "SentenceTransformer",
             snippets: list,
             k: int,
     ):
         score, index = index.search(
             embedding.encode([query]),
             k=k
         )
@@ -595,16 +620,16 @@
             query: str,
             k: Optional[int] = None,
             base_question: Optional[str] = None,
             retrival_argumented_generation_threshold: Optional[float] = None,
             verbose: bool = False,
             **kwargs
     ):
-        index: faiss.IndexFlatL2 | None = self.index
-        embedding: SentenceTransformer | None = self.embedding
+        index: "faiss.IndexFlatL2" | None = self.index
+        embedding: "SentenceTransformer" | None = self.embedding
         snippets: list[str] | None = self.snippets
         information = "Retrival Augmented Generation Search Information"
         if index is not None and embedding is not None and embedding is not None:
             contexts_and_scores = self.search(
                 query=query,
                 embedding=embedding,
                 snippets=snippets,
```

### Comparing `AgentX-0.0.1/src/agentx/llama_cpp/_configuration.py` & `AgentX-0.0.2/src/agentx/llama_cpp/_configuration.py`

 * *Files 3% similar despite different names*

```diff
@@ -176,27 +176,25 @@
 
 class LlamaCPParams(BaseCPPClass):
     def __init__(
             self,
             model_path: str,
             *,
             num_gpu_layers: int = 0,
-            split_mode: int = llama_cpp.LLAMA_SPLIT_LAYER,
             main_gpu: int = 0,
             tensor_split: Optional[List[float]] = None,
             vocab_only: bool = False,
             use_mmap: bool = True,
             use_mlock: bool = False,
             kv_overrides: Optional[Dict[str, Union[bool, int, float]]] = None,
-            seed: int = llama_cpp.LLAMA_DEFAULT_SEED,
+            seed: int = 42,
             num_context: int = 2048,
             num_batch: int = 512,
             num_threads: Optional[int] = None,
             num_threads_batch: Optional[int] = None,
-            rope_scaling_type: Optional[int] = llama_cpp.LLAMA_ROPE_SCALING_UNSPECIFIED,
             rope_freq_base: float = 0.0,
             rope_freq_scale: float = 0.0,
             yarn_ext_factor: float = -1.0,
             yarn_attn_factor: float = 1.0,
             yarn_beta_fast: float = 32.0,
             yarn_beta_slow: float = 1.0,
             yarn_orig_ctx: int = 0,
@@ -217,28 +215,26 @@
         The __init__ function is called when the class is instantiated.
         It sets up the object with all of its attributes and other components.
 
         :param self: Refer to the instance of the class
         :param model_path: str: Specify the path to the model
         :param *: Pass a variable number of arguments to a function
         :param num_gpu_layers: int: Specify the number of layers that will be run on a gpu
-        :param split_mode: int: Determine how the model is split across gpus
         :param main_gpu: int: Specify the gpu to use for inference
         :param tensor_split: Optional[List[float]]: Specify how the tensors are split between gpus
         :param vocab_only: bool: Load the vocabulary only
         :param use_mmap: bool: Determine whether to use mmap or not
         :param use_mlock: bool: Lock the memory of the model in ram
         :param kv_overrides: Optional[Dict[str, Union[bool, int, float]]]: Override the default values of the parameters
          in the model
         :param seed: int: Set the random seed for the model
         :param num_context: int: Set the number of context tokens to use
         :param num_batch: int: Set the number of batches to be processed at once
         :param num_threads: Optional[int]: Set the number of threads used for inference
         :param num_threads_batch: Optional[int]: Specify the number of threads to use for batching
-        :param rope_scaling_type: Optional[int]: Specify the scaling type of rope
         :param rope_freq_base: float: Set the rope_freq_base parameter in llama
         :param rope_freq_scale: float: Scale the frequency of words in the rope
         :param yarn_ext_factor: float: Control the amount of context that is used for each token
         :param yarn_attn_factor: float: Control the amount of attention that is applied to the context
         :param yarn_beta_fast: float: Set the beta parameter for yarn
         :param yarn_beta_slow: float: Control the speed of the model
         :param yarn_orig_ctx: int: Determine whether the context is used in yarn
@@ -254,27 +250,25 @@
         :param chat_format: str: Specify the format of the input text
         :param chat_handler: Optional[llama_chat_format.LlamaChatCompletionHandler]: Define a custom chat
         completion handler
         :param verbose: bool: Print out the progress of loading the model
         """
         self.model_path = model_path
         self.num_gpu_layers = num_gpu_layers
-        self.split_mode = split_mode
         self.main_gpu = main_gpu
         self.tensor_split = tensor_split
         self.vocab_only = vocab_only
         self.use_mmap = use_mmap
         self.use_mlock = use_mlock
         self.kv_overrides = kv_overrides
         self.seed = seed
         self.num_context = num_context
         self.num_batch = num_batch
         self.num_threads = num_threads
         self.num_threads_batch = num_threads_batch
-        self.rope_scaling_type = rope_scaling_type
         self.rope_freq_base = rope_freq_base
         self.rope_freq_scale = rope_freq_scale
         self.yarn_ext_factor = yarn_ext_factor
         self.yarn_attn_factor = yarn_attn_factor
         self.yarn_beta_fast = yarn_beta_fast
         self.yarn_beta_slow = yarn_beta_slow
         self.yarn_orig_ctx = yarn_orig_ctx
@@ -321,20 +315,18 @@
             main_gpu=self.main_gpu,
             use_mlock=self.use_mlock,
             embedding=self.embedding,
             lora_path=self.lora_path,
             n_threads=self.num_threads,
             n_ctx=self.num_context,
             chat_format=self.chat_format,
-            split_mode=self.split_mode,
             offload_kqv=self.offload_kqv,
             chat_handler=self.chat_handler,
             kv_overrides=self.kv_overrides,
             tensor_split=self.tensor_split,
-            rope_scaling_type=self.rope_scaling_type,
             seed=self.seed,
             numa=self.numa
         )
 
     def __repr__(self):
 
         """
```

### Comparing `AgentX-0.0.1/src/agentx/llama_cpp/_utils.py` & `AgentX-0.0.2/src/agentx/llama_cpp/_utils.py`

 * *Files identical despite different names*

### Comparing `AgentX-0.0.1/src/agentx/llama_cpp/inference.py` & `AgentX-0.0.2/src/agentx/llama_cpp/inference.py`

 * *Files identical despite different names*

### Comparing `AgentX-0.0.1/src/agentx/prompt_templates/prompt_templates.py` & `AgentX-0.0.2/src/agentx/prompt_templates/prompt_templates.py`

 * *Files identical despite different names*

