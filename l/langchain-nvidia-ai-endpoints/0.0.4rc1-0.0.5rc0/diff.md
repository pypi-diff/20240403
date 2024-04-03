# Comparing `tmp/langchain_nvidia_ai_endpoints-0.0.4rc1.tar.gz` & `tmp/langchain_nvidia_ai_endpoints-0.0.5rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_nvidia_ai_endpoints-0.0.4rc1.tar", max compression
+gzip compressed data, was "langchain_nvidia_ai_endpoints-0.0.5rc0.tar", max compression
```

## Comparing `langchain_nvidia_ai_endpoints-0.0.4rc1.tar` & `langchain_nvidia_ai_endpoints-0.0.5rc0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1072 2024-03-19 11:08:33.699403 langchain_nvidia_ai_endpoints-0.0.4rc1/LICENSE
--rw-r--r--   0        0        0    10720 2024-03-19 11:08:33.699403 langchain_nvidia_ai_endpoints-0.0.4rc1/README.md
--rw-r--r--   0        0        0     2070 2024-03-19 11:08:33.699403 langchain_nvidia_ai_endpoints-0.0.4rc1/langchain_nvidia_ai_endpoints/__init__.py
--rw-r--r--   0        0        0    29226 2024-03-19 11:08:33.699403 langchain_nvidia_ai_endpoints-0.0.4rc1/langchain_nvidia_ai_endpoints/_common.py
--rw-r--r--   0        0        0     4738 2024-03-19 11:08:33.699403 langchain_nvidia_ai_endpoints-0.0.4rc1/langchain_nvidia_ai_endpoints/_statics.py
--rw-r--r--   0        0        0    10149 2024-03-19 11:08:33.699403 langchain_nvidia_ai_endpoints-0.0.4rc1/langchain_nvidia_ai_endpoints/callbacks.py
--rw-r--r--   0        0        0    15746 2024-03-19 11:08:33.699403 langchain_nvidia_ai_endpoints-0.0.4rc1/langchain_nvidia_ai_endpoints/chat_models.py
--rw-r--r--   0        0        0     3337 2024-03-19 11:08:33.699403 langchain_nvidia_ai_endpoints-0.0.4rc1/langchain_nvidia_ai_endpoints/embeddings.py
--rw-r--r--   0        0        0     5735 2024-03-19 11:08:33.699403 langchain_nvidia_ai_endpoints-0.0.4rc1/langchain_nvidia_ai_endpoints/image_gen.py
--rw-r--r--   0        0        0     7597 2024-03-19 11:08:33.699403 langchain_nvidia_ai_endpoints-0.0.4rc1/langchain_nvidia_ai_endpoints/llm.py
--rw-r--r--   0        0        0        0 2024-03-19 11:08:33.699403 langchain_nvidia_ai_endpoints-0.0.4rc1/langchain_nvidia_ai_endpoints/py.typed
--rw-r--r--   0        0        0    10047 2024-03-19 11:08:33.699403 langchain_nvidia_ai_endpoints-0.0.4rc1/langchain_nvidia_ai_endpoints/tools.py
--rw-r--r--   0        0        0     2621 2024-03-19 11:08:33.699403 langchain_nvidia_ai_endpoints-0.0.4rc1/pyproject.toml
--rw-r--r--   0        0        0    11622 1970-01-01 00:00:00.000000 langchain_nvidia_ai_endpoints-0.0.4rc1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-02 14:19:37.310745 langchain_nvidia_ai_endpoints-0.0.5rc0/LICENSE
+-rw-r--r--   0        0        0    10720 2024-04-02 14:19:37.310745 langchain_nvidia_ai_endpoints-0.0.5rc0/README.md
+-rw-r--r--   0        0        0     2070 2024-04-02 14:19:37.314746 langchain_nvidia_ai_endpoints-0.0.5rc0/langchain_nvidia_ai_endpoints/__init__.py
+-rw-r--r--   0        0        0    29698 2024-04-02 14:19:37.314746 langchain_nvidia_ai_endpoints-0.0.5rc0/langchain_nvidia_ai_endpoints/_common.py
+-rw-r--r--   0        0        0     5358 2024-04-02 14:19:37.314746 langchain_nvidia_ai_endpoints-0.0.5rc0/langchain_nvidia_ai_endpoints/_statics.py
+-rw-r--r--   0        0        0    10149 2024-04-02 14:19:37.314746 langchain_nvidia_ai_endpoints-0.0.5rc0/langchain_nvidia_ai_endpoints/callbacks.py
+-rw-r--r--   0        0        0    15746 2024-04-02 14:19:37.314746 langchain_nvidia_ai_endpoints-0.0.5rc0/langchain_nvidia_ai_endpoints/chat_models.py
+-rw-r--r--   0        0        0     4895 2024-04-02 14:19:37.314746 langchain_nvidia_ai_endpoints-0.0.5rc0/langchain_nvidia_ai_endpoints/embeddings.py
+-rw-r--r--   0        0        0     5735 2024-04-02 14:19:37.314746 langchain_nvidia_ai_endpoints-0.0.5rc0/langchain_nvidia_ai_endpoints/image_gen.py
+-rw-r--r--   0        0        0     7597 2024-04-02 14:19:37.314746 langchain_nvidia_ai_endpoints-0.0.5rc0/langchain_nvidia_ai_endpoints/llm.py
+-rw-r--r--   0        0        0        0 2024-04-02 14:19:37.314746 langchain_nvidia_ai_endpoints-0.0.5rc0/langchain_nvidia_ai_endpoints/py.typed
+-rw-r--r--   0        0        0    10047 2024-04-02 14:19:37.314746 langchain_nvidia_ai_endpoints-0.0.5rc0/langchain_nvidia_ai_endpoints/tools.py
+-rw-r--r--   0        0        0     2673 2024-04-02 14:19:37.318745 langchain_nvidia_ai_endpoints-0.0.5rc0/pyproject.toml
+-rw-r--r--   0        0        0    11622 1970-01-01 00:00:00.000000 langchain_nvidia_ai_endpoints-0.0.5rc0/PKG-INFO
```

### Comparing `langchain_nvidia_ai_endpoints-0.0.4rc1/LICENSE` & `langchain_nvidia_ai_endpoints-0.0.5rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_nvidia_ai_endpoints-0.0.4rc1/README.md` & `langchain_nvidia_ai_endpoints-0.0.5rc0/README.md`

 * *Files identical despite different names*

### Comparing `langchain_nvidia_ai_endpoints-0.0.4rc1/langchain_nvidia_ai_endpoints/__init__.py` & `langchain_nvidia_ai_endpoints-0.0.5rc0/langchain_nvidia_ai_endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_nvidia_ai_endpoints-0.0.4rc1/langchain_nvidia_ai_endpoints/_common.py` & `langchain_nvidia_ai_endpoints-0.0.5rc0/langchain_nvidia_ai_endpoints/_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,15 @@
     @root_validator(pre=True)
     def validate_model(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         """Validate and update model arguments, including API key and formatting"""
         values["api_key"] = (
             values.get(cls._api_key_var.lower())
             or values.get("api_key")
             or os.getenv(cls._api_key_var)
+            or ""
         )
         values["is_staging"] = "nvapi-stg-" in values["api_key"]
         if "headers_tmpl" not in values:
             call_kvs = {
                 "Accept": "application/json",
             }
             stream_kvs = {
@@ -259,23 +260,33 @@
                 rd = response.json()
                 if "detail" in rd and "reqId" in rd.get("detail", ""):
                     rd_buf = "- " + str(rd["detail"])
                     rd_buf = rd_buf.replace(": ", ", Error: ").replace(", ", "\n- ")
                     rd["detail"] = rd_buf
             except json.JSONDecodeError:
                 rd = response.__dict__
-                rd = rd.get("_content", rd)
-                if isinstance(rd, bytes):
-                    rd = rd.decode("utf-8")[5:]  ## remove "data:" prefix
-                try:
-                    rd = json.loads(rd)
-                except Exception:
-                    rd = {"detail": rd}
-            status = rd.get("status", "###")
-            title = rd.get("title", rd.get("error", "Unknown Error"))
+                if "status_code" in rd:
+                    if "headers" in rd and "WWW-Authenticate" in rd["headers"]:
+                        rd["detail"] = rd.get("headers").get("WWW-Authenticate")
+                        rd["detail"] = rd["detail"].replace(", ", "\n")
+                else:
+                    rd = rd.get("_content", rd)
+                    if isinstance(rd, bytes):
+                        rd = rd.decode("utf-8")[5:]  ## remove "data:" prefix
+                    try:
+                        rd = json.loads(rd)
+                    except Exception:
+                        rd = {"detail": rd}
+            status = rd.get("status") or rd.get("status_code") or "###"
+            title = (
+                rd.get("title")
+                or rd.get("error")
+                or rd.get("reason")
+                or "Unknown Error"
+            )
             header = f"[{status}] {title}"
             body = ""
             if "requestId" in rd:
                 if "detail" in rd:
                     body += f"{rd['detail']}\n"
                 body += "RequestID: " + rd["requestId"]
             else:
```

### Comparing `langchain_nvidia_ai_endpoints-0.0.4rc1/langchain_nvidia_ai_endpoints/_statics.py` & `langchain_nvidia_ai_endpoints-0.0.5rc0/langchain_nvidia_ai_endpoints/_statics.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,54 +2,55 @@
 
 from langchain_core.pydantic_v1 import BaseModel
 
 
 class Model(BaseModel):
     id: str
     model_type: Optional[str] = None
+    api_type: Optional[str] = None
     model_name: Optional[str] = None
     client: Optional[str] = None
     path: str
 
 
 MODEL_SPECS = {
-    "playground_smaug_72b": {"model_type": "chat"},
-    "playground_kosmos_2": {"model_type": "image_in"},
-    "playground_llama2_70b": {"model_type": "chat"},
-    "playground_nvolveqa_40k": {"model_type": "embedding"},
-    "playground_nemotron_qa_8b": {"model_type": "qa"},
-    "playground_gemma_7b": {"model_type": "chat"},
-    "playground_mistral_7b": {"model_type": "chat"},
-    "playground_mamba_chat": {"model_type": "chat"},
-    "playground_phi2": {"model_type": "chat"},
-    "playground_sdxl": {"model_type": "image_out"},
-    "playground_nv_llama2_rlhf_70b": {"model_type": "chat"},
-    "playground_neva_22b": {"model_type": "image_in"},
-    "playground_yi_34b": {"model_type": "chat"},
-    "playground_nemotron_steerlm_8b": {"model_type": "chat"},
-    "playground_cuopt": {"model_type": "cuopt"},
-    "playground_llama_guard": {"model_type": "classifier"},
-    "playground_starcoder2_15b": {"model_type": "completion"},
-    "playground_deplot": {"model_type": "image_in"},
-    "playground_llama2_code_70b": {"model_type": "chat"},
-    "playground_gemma_2b": {"model_type": "chat"},
-    "playground_seamless": {"model_type": "translation"},
-    "playground_mixtral_8x7b": {"model_type": "chat"},
-    "playground_fuyu_8b": {"model_type": "image_in"},
-    "playground_llama2_code_34b": {"model_type": "chat"},
-    "playground_llama2_code_13b": {"model_type": "chat"},
-    "playground_steerlm_llama_70b": {"model_type": "chat"},
-    "playground_clip": {"model_type": "similarity"},
-    "playground_llama2_13b": {"model_type": "chat"},
+    "playground_smaug_72b": {"model_type": "chat", "api_type": "aifm"},
+    "playground_kosmos_2": {"model_type": "image_in", "api_type": "aifm"},
+    "playground_llama2_70b": {"model_type": "chat", "api_type": "aifm"},
+    "playground_nvolveqa_40k": {"model_type": "embedding", "api_type": "aifm"},
+    "playground_nemotron_qa_8b": {"model_type": "qa", "api_type": "aifm"},
+    "playground_gemma_7b": {"model_type": "chat", "api_type": "aifm"},
+    "playground_mistral_7b": {"model_type": "chat", "api_type": "aifm"},
+    "playground_mamba_chat": {"model_type": "chat", "api_type": "aifm"},
+    "playground_phi2": {"model_type": "chat", "api_type": "aifm"},
+    "playground_sdxl": {"model_type": "image_out", "api_type": "aifm"},
+    "playground_nv_llama2_rlhf_70b": {"model_type": "chat", "api_type": "aifm"},
+    "playground_neva_22b": {"model_type": "image_in", "api_type": "aifm"},
+    "playground_yi_34b": {"model_type": "chat", "api_type": "aifm"},
+    "playground_nemotron_steerlm_8b": {"model_type": "chat", "api_type": "aifm"},
+    "playground_cuopt": {"model_type": "cuopt", "api_type": "aifm"},
+    "playground_llama_guard": {"model_type": "classifier", "api_type": "aifm"},
+    "playground_starcoder2_15b": {"model_type": "completion", "api_type": "aifm"},
+    "playground_deplot": {"model_type": "image_in", "api_type": "aifm"},
+    "playground_llama2_code_70b": {"model_type": "chat", "api_type": "aifm"},
+    "playground_gemma_2b": {"model_type": "chat", "api_type": "aifm"},
+    "playground_seamless": {"model_type": "translation", "api_type": "aifm"},
+    "playground_mixtral_8x7b": {"model_type": "chat", "api_type": "aifm"},
+    "playground_fuyu_8b": {"model_type": "image_in", "api_type": "aifm"},
+    "playground_llama2_code_34b": {"model_type": "chat", "api_type": "aifm"},
+    "playground_llama2_code_13b": {"model_type": "chat", "api_type": "aifm"},
+    "playground_steerlm_llama_70b": {"model_type": "chat", "api_type": "aifm"},
+    "playground_clip": {"model_type": "similarity", "api_type": "aifm"},
+    "playground_llama2_13b": {"model_type": "chat", "api_type": "aifm"},
 }
 
 MODEL_SPECS.update(
     {
         "ai-codellama-70b": {"model_type": "chat", "model_name": "meta/codellama-70b"},
-        # 'ai-embedding-2b': {'model_type': 'embedding'},
+        "ai-embed-qa-4": {"model_type": "embedding", "model_name": "NV-Embed-QA"},
         "ai-fuyu-8b": {"model_type": "image_in"},
         "ai-gemma-7b": {"model_type": "chat", "model_name": "google/gemma-7b"},
         "ai-google-deplot": {"model_type": "image_in"},
         "ai-llama2-70b": {"model_type": "chat", "model_name": "meta/llama2-70b"},
         "ai-microsoft-kosmos-2": {"model_type": "image_in"},
         "ai-mistral-7b-instruct-v2": {
             "model_type": "chat",
```

### Comparing `langchain_nvidia_ai_endpoints-0.0.4rc1/langchain_nvidia_ai_endpoints/callbacks.py` & `langchain_nvidia_ai_endpoints-0.0.5rc0/langchain_nvidia_ai_endpoints/callbacks.py`

 * *Files identical despite different names*

### Comparing `langchain_nvidia_ai_endpoints-0.0.4rc1/langchain_nvidia_ai_endpoints/chat_models.py` & `langchain_nvidia_ai_endpoints-0.0.5rc0/langchain_nvidia_ai_endpoints/chat_models.py`

 * *Files identical despite different names*

### Comparing `langchain_nvidia_ai_endpoints-0.0.4rc1/langchain_nvidia_ai_endpoints/embeddings.py` & `langchain_nvidia_ai_endpoints-0.0.5rc0/langchain_nvidia_ai_endpoints/embeddings.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 """Embeddings Components Derived from NVEModel/Embeddings"""
+
 from typing import List, Literal, Optional
 
 from langchain_core.embeddings import Embeddings
 from langchain_core.outputs.llm_result import LLMResult
 from langchain_core.pydantic_v1 import Field
 
 from langchain_nvidia_ai_endpoints._common import _NVIDIAClient
 from langchain_nvidia_ai_endpoints.callbacks import usage_callback_var
 
+from ._statics import MODEL_SPECS
+
 
 class NVIDIAEmbeddings(_NVIDIAClient, Embeddings):
     """NVIDIA's AI Foundation Retriever Question-Answering Asymmetric Model."""
 
     _default_model: str = "nvolveqa_40k"
     infer_endpoint: str = Field("{base_url}/embeddings")
     model: str = Field(_default_model, description="Name of the model to invoke")
@@ -21,21 +24,48 @@
         None, description="The type of text to be embedded."
     )
 
     def _embed(
         self, texts: List[str], model_type: Literal["passage", "query"]
     ) -> List[List[float]]:
         """Embed a single text entry to either passage or query type"""
-        response = self.client.get_req(
-            model_name=self.model,
-            payload={
+        # AI Foundation Model API -
+        #  input: str | list[str]              -- <= 2048 characters, <= 50 inputs
+        #  model: "query" | "passage"          -- type of input text to be embedded
+        #  encoding_format: "float" | "base64"
+        # API Catalog API -
+        #  input: str | list[str]              -- char limit depends on model
+        #  model: str                          -- model name, e.g. NV-Embed-QA
+        #  encoding_format: "float" | "base64"
+        #  input_type: "query" | "passage"
+        #  user: str                           -- ignored
+        #  truncate: "NONE" | "START" | "END"  -- default "NONE", error raised if
+        #                                         an input is too long
+        # todo: remove the playground aliases
+        model_name = self.model
+        if model_name not in MODEL_SPECS:
+            if f"playground_{model_name}" in MODEL_SPECS:
+                model_name = f"playground_{model_name}"
+        if MODEL_SPECS.get(model_name, {}).get("api_type", None) == "aifm":
+            payload = {
+                "input": texts,
+                "model": model_type,
+                "encoding_format": "float",
+            }
+        else:  # default to the API Catalog API
+            payload = {
                 "input": texts,
-                "model": self.get_binding_model() or model_type,
+                "model": self.get_binding_model() or self.model,
                 "encoding_format": "float",
-            },
+                "input_type": model_type,
+            }
+
+        response = self.client.get_req(
+            model_name=self.model,
+            payload=payload,
             endpoint="infer",
         )
         response.raise_for_status()
         result = response.json()
         data = result.get("data", result)
         if not isinstance(data, list):
             raise ValueError(f"Expected data with a list of embeddings. Got: {data}")
@@ -45,14 +75,19 @@
 
     def embed_query(self, text: str) -> List[float]:
         """Input pathway for query embeddings."""
         return self._embed([text], model_type=self.model_type or "query")[0]
 
     def embed_documents(self, texts: List[str]) -> List[List[float]]:
         """Input pathway for document embeddings."""
+        if not isinstance(texts, list) or not all(
+            isinstance(text, str) for text in texts
+        ):
+            raise ValueError(f"`texts` must be a list of strings, given: {repr(texts)}")
+
         # From https://catalog.ngc.nvidia.com/orgs/nvidia/teams/ai-foundation/models/nvolve-40k/documentation
         # The input must not exceed the 2048 max input characters and inputs above 512
         # model tokens will be truncated. The input array must not exceed 50 input
         #  strings.
         all_embeddings = []
         for i in range(0, len(texts), self.max_batch_size):
             batch = texts[i : i + self.max_batch_size]
```

### Comparing `langchain_nvidia_ai_endpoints-0.0.4rc1/langchain_nvidia_ai_endpoints/image_gen.py` & `langchain_nvidia_ai_endpoints-0.0.5rc0/langchain_nvidia_ai_endpoints/image_gen.py`

 * *Files identical despite different names*

### Comparing `langchain_nvidia_ai_endpoints-0.0.4rc1/langchain_nvidia_ai_endpoints/llm.py` & `langchain_nvidia_ai_endpoints-0.0.5rc0/langchain_nvidia_ai_endpoints/llm.py`

 * *Files identical despite different names*

### Comparing `langchain_nvidia_ai_endpoints-0.0.4rc1/langchain_nvidia_ai_endpoints/tools.py` & `langchain_nvidia_ai_endpoints-0.0.5rc0/langchain_nvidia_ai_endpoints/tools.py`

 * *Files identical despite different names*

### Comparing `langchain_nvidia_ai_endpoints-0.0.4rc1/pyproject.toml` & `langchain_nvidia_ai_endpoints-0.0.5rc0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-nvidia-ai-endpoints"
-version = "0.0.4-rc1"
+version = "0.0.5-rc0"
 description = "An integration package connecting NVIDIA AI Endpoints and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
@@ -23,25 +23,27 @@
 pytest = "^7.3.0"
 freezegun = "^1.2.2"
 pytest-mock = "^3.10.0"
 syrupy = "^4.0.2"
 pytest-watcher = "^0.3.4"
 pytest-asyncio = "^0.21.1"
 langchain-core = "^0.1.5"
+requests-mock = "^1.11.0"
 
 [tool.poetry.group.codespell]
 optional = true
 
 [tool.poetry.group.codespell.dependencies]
 codespell = "^2.2.0"
 
 [tool.poetry.group.test_integration]
 optional = true
 
 [tool.poetry.group.test_integration.dependencies]
+requests-mock = "^1.11.0"
 
 [tool.poetry.group.lint]
 optional = true
 
 [tool.poetry.group.lint.dependencies]
 ruff = "^0.1.5"
```

### Comparing `langchain_nvidia_ai_endpoints-0.0.4rc1/PKG-INFO` & `langchain_nvidia_ai_endpoints-0.0.5rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-nvidia-ai-endpoints
-Version: 0.0.4rc1
+Version: 0.0.5rc0
 Summary: An integration package connecting NVIDIA AI Endpoints and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

