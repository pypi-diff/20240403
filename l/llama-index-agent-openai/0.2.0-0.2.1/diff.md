# Comparing `tmp/llama_index_agent_openai-0.2.0.tar.gz` & `tmp/llama_index_agent_openai-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_agent_openai-0.2.0.tar", max compression
+gzip compressed data, was "llama_index_agent_openai-0.2.1.tar", max compression
```

## Comparing `llama_index_agent_openai-0.2.0.tar` & `llama_index_agent_openai-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       39 2024-03-26 16:12:00.568621 llama_index_agent_openai-0.2.0/README.md
--rw-r--r--   0        0        0      342 2024-03-26 16:12:00.568621 llama_index_agent_openai-0.2.0/llama_index/agent/openai/__init__.py
--rw-r--r--   0        0        0     4745 2024-03-26 16:12:00.568621 llama_index_agent_openai-0.2.0/llama_index/agent/openai/base.py
--rw-r--r--   0        0        0    18810 2024-03-26 16:12:00.568621 llama_index_agent_openai-0.2.0/llama_index/agent/openai/openai_assistant_agent.py
--rw-r--r--   0        0        0    26983 2024-03-26 16:12:00.568621 llama_index_agent_openai-0.2.0/llama_index/agent/openai/step.py
--rw-r--r--   0        0        0      772 2024-03-26 16:12:00.568621 llama_index_agent_openai-0.2.0/llama_index/agent/openai/utils.py
--rw-r--r--   0        0        0     1501 2024-03-26 16:12:00.572620 llama_index_agent_openai-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      644 1970-01-01 00:00:00.000000 llama_index_agent_openai-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       39 2024-03-14 20:48:34.594654 llama_index_agent_openai-0.2.1/README.md
+-rw-r--r--   0        0        0      342 2024-03-26 21:31:03.738615 llama_index_agent_openai-0.2.1/llama_index/agent/openai/__init__.py
+-rw-r--r--   0        0        0     4745 2024-03-26 21:31:03.738783 llama_index_agent_openai-0.2.1/llama_index/agent/openai/base.py
+-rw-r--r--   0        0        0    18810 2024-03-14 20:48:34.594996 llama_index_agent_openai-0.2.1/llama_index/agent/openai/openai_assistant_agent.py
+-rw-r--r--   0        0        0    26990 2024-03-27 00:25:24.643670 llama_index_agent_openai-0.2.1/llama_index/agent/openai/step.py
+-rw-r--r--   0        0        0      772 2024-03-14 20:48:34.595334 llama_index_agent_openai-0.2.1/llama_index/agent/openai/utils.py
+-rw-r--r--   0        0        0     1501 2024-03-27 00:27:37.210340 llama_index_agent_openai-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      644 1970-01-01 00:00:00.000000 llama_index_agent_openai-0.2.1/PKG-INFO
```

### Comparing `llama_index_agent_openai-0.2.0/llama_index/agent/openai/base.py` & `llama_index_agent_openai-0.2.1/llama_index/agent/openai/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_agent_openai-0.2.0/llama_index/agent/openai/openai_assistant_agent.py` & `llama_index_agent_openai-0.2.1/llama_index/agent/openai/openai_assistant_agent.py`

 * *Files identical despite different names*

### Comparing `llama_index_agent_openai-0.2.0/llama_index/agent/openai/step.py` & `llama_index_agent_openai-0.2.1/llama_index/agent/openai/step.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
             raw_input={"kwargs": input_dict},
             raw_output=e,
         )
 
 
 def default_tool_call_parser(tool_call: OpenAIToolCall):
     try:
-        json.loads(tool_call.function.arguments)
+        return json.loads(tool_call.function.arguments)
     except json.JSONDecodeError as e:
         raise ValueError(
             f"Error in calling tool {tool_call.function.name}: The input json block is malformed:\n```json\n{tool_call.function.arguments}\n```"
         )
 
 
 def advanced_tool_call_parser(tool_call: OpenAIToolCall) -> Dict:
```

### Comparing `llama_index_agent_openai-0.2.0/llama_index/agent/openai/utils.py` & `llama_index_agent_openai-0.2.1/llama_index/agent/openai/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_agent_openai-0.2.0/pyproject.toml` & `llama_index_agent_openai-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index agent openai integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-agent-openai"
 readme = "README.md"
-version = "0.2.0"
+version = "0.2.1"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 llama-index-llms-openai = "^0.1.5"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_agent_openai-0.2.0/PKG-INFO` & `llama_index_agent_openai-0.2.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-agent-openai
-Version: 0.2.0
+Version: 0.2.1
 Summary: llama-index agent openai integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

