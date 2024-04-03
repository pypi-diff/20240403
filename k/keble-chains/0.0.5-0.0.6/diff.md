# Comparing `tmp/keble_chains-0.0.5.tar.gz` & `tmp/keble_chains-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keble_chains-0.0.5.tar", max compression
+gzip compressed data, was "keble_chains-0.0.6.tar", max compression
```

## Comparing `keble_chains-0.0.5.tar` & `keble_chains-0.0.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1067 2024-03-05 11:27:13.622616 keble_chains-0.0.5/LICENSE
--rw-r--r--   0        0        0        0 2024-03-05 11:27:13.623628 keble_chains-0.0.5/README.md
--rw-r--r--   0        0        0      373 2024-03-05 11:27:13.615707 keble_chains-0.0.5/keble_chains/__init__.py
--rw-r--r--   0        0        0       65 2024-03-05 11:27:13.615841 keble_chains-0.0.5/keble_chains/chainables/__init__.py
--rw-r--r--   0        0        0       28 2024-03-05 11:27:13.615961 keble_chains-0.0.5/keble_chains/chainables/chunk/__init__.py
--rw-r--r--   0        0        0      277 2024-03-05 11:27:13.616078 keble_chains-0.0.5/keble_chains/chainables/chunk/chainable.py
--rw-r--r--   0        0        0       31 2024-03-05 11:27:13.616191 keble_chains-0.0.5/keble_chains/chainables/metadata/__init__.py
--rw-r--r--   0        0        0      283 2024-03-05 11:27:13.616344 keble_chains-0.0.5/keble_chains/chainables/metadata/chainable.py
--rw-r--r--   0        0        0       28 2024-03-05 11:27:13.616582 keble_chains-0.0.5/keble_chains/chainables/prune/__init__.py
--rw-r--r--   0        0        0      277 2024-03-05 11:27:13.616892 keble_chains-0.0.5/keble_chains/chainables/prune/chainable.py
--rw-r--r--   0        0        0    12082 2024-03-05 11:27:13.617158 keble_chains-0.0.5/keble_chains/chains.py
--rw-r--r--   0        0        0      215 2024-03-05 11:27:13.617420 keble_chains-0.0.5/keble_chains/exceptions/__init__.py
--rw-r--r--   0        0        0     1632 2024-03-05 11:27:13.617747 keble_chains-0.0.5/keble_chains/exceptions/openai.py
--rw-r--r--   0        0        0       57 2024-03-05 11:27:13.617856 keble_chains-0.0.5/keble_chains/export/__init__.py
--rw-r--r--   0        0        0     7777 2024-03-05 11:27:13.617971 keble_chains-0.0.5/keble_chains/export/export.py
--rw-r--r--   0        0        0       36 2024-03-05 11:27:13.618077 keble_chains-0.0.5/keble_chains/interact/__init__.py
--rw-r--r--   0        0        0      135 2024-03-05 11:27:13.618190 keble_chains-0.0.5/keble_chains/interact/ai/__init__.py
--rw-r--r--   0        0        0     6283 2024-03-29 08:16:12.171989 keble_chains-0.0.5/keble_chains/interact/ai/azure.py
--rw-r--r--   0        0        0     1286 2024-03-05 11:27:13.618440 keble_chains-0.0.5/keble_chains/interact/ai/fake.py
--rw-r--r--   0        0        0     1387 2024-03-05 11:27:13.618658 keble_chains-0.0.5/keble_chains/interact/ai/session.py
--rw-r--r--   0        0        0     4017 2024-03-05 11:27:13.618771 keble_chains-0.0.5/keble_chains/interact/ai/token_manager.py
--rw-r--r--   0        0        0      120 2024-03-05 11:27:13.618873 keble_chains-0.0.5/keble_chains/interact/m14/__init__.py
--rw-r--r--   0        0        0     5717 2024-03-05 11:27:13.618981 keble_chains-0.0.5/keble_chains/interact/m14/m14_compressors.py
--rw-r--r--   0        0        0     1457 2024-03-05 11:27:13.619082 keble_chains-0.0.5/keble_chains/interact/m14/m14_session.py
--rw-r--r--   0        0        0      232 2024-03-05 11:27:13.619198 keble_chains-0.0.5/keble_chains/template/__init__.py
--rw-r--r--   0        0        0       46 2024-03-05 11:27:13.619315 keble_chains-0.0.5/keble_chains/template/base.py
--rw-r--r--   0        0        0     8179 2024-03-05 11:27:13.619488 keble_chains-0.0.5/keble_chains/template/chat.py
--rw-r--r--   0        0        0     2632 2024-03-05 11:27:13.619602 keble_chains-0.0.5/keble_chains/template/email.py
--rw-r--r--   0        0        0      460 2024-03-05 11:27:13.619706 keble_chains-0.0.5/keble_chains/template/openai.py
--rw-r--r--   0        0        0       63 2024-03-05 11:27:13.619811 keble_chains-0.0.5/keble_chains/tuning/__init__.py
--rw-r--r--   0        0        0    16219 2024-03-05 11:27:13.620867 keble_chains-0.0.5/keble_chains/tuning/datasets.py
--rw-r--r--   0        0        0      562 2024-03-05 11:27:13.621013 keble_chains-0.0.5/keble_chains/typings/__init__.py
--rw-r--r--   0        0        0    11627 2024-03-05 11:27:13.621272 keble_chains-0.0.5/keble_chains/typings/abc.py
--rw-r--r--   0        0        0     9513 2024-03-12 14:33:49.625950 keble_chains-0.0.5/keble_chains/typings/ai.py
--rw-r--r--   0        0        0      321 2024-03-05 11:27:13.621784 keble_chains-0.0.5/keble_chains/typings/collected.py
--rw-r--r--   0        0        0     1865 2024-03-05 11:27:13.621905 keble_chains-0.0.5/keble_chains/typings/dataset.py
--rw-r--r--   0        0        0     1922 2024-03-05 11:27:13.622026 keble_chains-0.0.5/keble_chains/typings/export.py
--rw-r--r--   0        0        0      419 2024-03-05 11:27:13.622152 keble_chains-0.0.5/keble_chains/typings/main.py
--rw-r--r--   0        0        0      122 2024-03-05 11:27:13.622281 keble_chains-0.0.5/keble_chains/typings/valid.py
--rw-r--r--   0        0        0       84 2024-03-05 11:27:13.622403 keble_chains-0.0.5/keble_chains/utils/__init__.py
--rw-r--r--   0        0        0      922 2024-03-05 11:27:13.622508 keble_chains-0.0.5/keble_chains/utils/main.py
--rw-r--r--   0        0        0      588 2024-03-29 08:16:18.395786 keble_chains-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      914 1970-01-01 00:00:00.000000 keble_chains-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-03-05 11:27:13.622616 keble_chains-0.0.6/LICENSE
+-rw-r--r--   0        0        0        0 2024-03-05 11:27:13.623628 keble_chains-0.0.6/README.md
+-rw-r--r--   0        0        0      373 2024-03-05 11:27:13.615707 keble_chains-0.0.6/keble_chains/__init__.py
+-rw-r--r--   0        0        0       65 2024-03-05 11:27:13.615841 keble_chains-0.0.6/keble_chains/chainables/__init__.py
+-rw-r--r--   0        0        0       28 2024-03-05 11:27:13.615961 keble_chains-0.0.6/keble_chains/chainables/chunk/__init__.py
+-rw-r--r--   0        0        0      277 2024-03-05 11:27:13.616078 keble_chains-0.0.6/keble_chains/chainables/chunk/chainable.py
+-rw-r--r--   0        0        0       31 2024-03-05 11:27:13.616191 keble_chains-0.0.6/keble_chains/chainables/metadata/__init__.py
+-rw-r--r--   0        0        0      283 2024-03-05 11:27:13.616344 keble_chains-0.0.6/keble_chains/chainables/metadata/chainable.py
+-rw-r--r--   0        0        0       28 2024-03-05 11:27:13.616582 keble_chains-0.0.6/keble_chains/chainables/prune/__init__.py
+-rw-r--r--   0        0        0      277 2024-03-05 11:27:13.616892 keble_chains-0.0.6/keble_chains/chainables/prune/chainable.py
+-rw-r--r--   0        0        0    12082 2024-03-05 11:27:13.617158 keble_chains-0.0.6/keble_chains/chains.py
+-rw-r--r--   0        0        0      215 2024-03-05 11:27:13.617420 keble_chains-0.0.6/keble_chains/exceptions/__init__.py
+-rw-r--r--   0        0        0     1632 2024-03-05 11:27:13.617747 keble_chains-0.0.6/keble_chains/exceptions/openai.py
+-rw-r--r--   0        0        0       57 2024-03-05 11:27:13.617856 keble_chains-0.0.6/keble_chains/export/__init__.py
+-rw-r--r--   0        0        0     7777 2024-03-05 11:27:13.617971 keble_chains-0.0.6/keble_chains/export/export.py
+-rw-r--r--   0        0        0       36 2024-03-05 11:27:13.618077 keble_chains-0.0.6/keble_chains/interact/__init__.py
+-rw-r--r--   0        0        0      135 2024-03-05 11:27:13.618190 keble_chains-0.0.6/keble_chains/interact/ai/__init__.py
+-rw-r--r--   0        0        0     6761 2024-04-03 10:10:32.625405 keble_chains-0.0.6/keble_chains/interact/ai/azure.py
+-rw-r--r--   0        0        0     1286 2024-03-05 11:27:13.618440 keble_chains-0.0.6/keble_chains/interact/ai/fake.py
+-rw-r--r--   0        0        0     1387 2024-03-05 11:27:13.618658 keble_chains-0.0.6/keble_chains/interact/ai/session.py
+-rw-r--r--   0        0        0     4017 2024-03-05 11:27:13.618771 keble_chains-0.0.6/keble_chains/interact/ai/token_manager.py
+-rw-r--r--   0        0        0      120 2024-03-05 11:27:13.618873 keble_chains-0.0.6/keble_chains/interact/m14/__init__.py
+-rw-r--r--   0        0        0     5717 2024-03-05 11:27:13.618981 keble_chains-0.0.6/keble_chains/interact/m14/m14_compressors.py
+-rw-r--r--   0        0        0     1457 2024-03-05 11:27:13.619082 keble_chains-0.0.6/keble_chains/interact/m14/m14_session.py
+-rw-r--r--   0        0        0      232 2024-03-05 11:27:13.619198 keble_chains-0.0.6/keble_chains/template/__init__.py
+-rw-r--r--   0        0        0       46 2024-03-05 11:27:13.619315 keble_chains-0.0.6/keble_chains/template/base.py
+-rw-r--r--   0        0        0     8179 2024-03-05 11:27:13.619488 keble_chains-0.0.6/keble_chains/template/chat.py
+-rw-r--r--   0        0        0     2632 2024-03-05 11:27:13.619602 keble_chains-0.0.6/keble_chains/template/email.py
+-rw-r--r--   0        0        0      460 2024-03-05 11:27:13.619706 keble_chains-0.0.6/keble_chains/template/openai.py
+-rw-r--r--   0        0        0       63 2024-03-05 11:27:13.619811 keble_chains-0.0.6/keble_chains/tuning/__init__.py
+-rw-r--r--   0        0        0    16219 2024-03-05 11:27:13.620867 keble_chains-0.0.6/keble_chains/tuning/datasets.py
+-rw-r--r--   0        0        0      562 2024-03-05 11:27:13.621013 keble_chains-0.0.6/keble_chains/typings/__init__.py
+-rw-r--r--   0        0        0    11627 2024-03-05 11:27:13.621272 keble_chains-0.0.6/keble_chains/typings/abc.py
+-rw-r--r--   0        0        0     9513 2024-03-12 14:33:49.625950 keble_chains-0.0.6/keble_chains/typings/ai.py
+-rw-r--r--   0        0        0      321 2024-03-05 11:27:13.621784 keble_chains-0.0.6/keble_chains/typings/collected.py
+-rw-r--r--   0        0        0     1865 2024-03-05 11:27:13.621905 keble_chains-0.0.6/keble_chains/typings/dataset.py
+-rw-r--r--   0        0        0     1922 2024-03-05 11:27:13.622026 keble_chains-0.0.6/keble_chains/typings/export.py
+-rw-r--r--   0        0        0      419 2024-03-05 11:27:13.622152 keble_chains-0.0.6/keble_chains/typings/main.py
+-rw-r--r--   0        0        0      122 2024-03-05 11:27:13.622281 keble_chains-0.0.6/keble_chains/typings/valid.py
+-rw-r--r--   0        0        0       84 2024-03-05 11:27:13.622403 keble_chains-0.0.6/keble_chains/utils/__init__.py
+-rw-r--r--   0        0        0      922 2024-03-05 11:27:13.622508 keble_chains-0.0.6/keble_chains/utils/main.py
+-rw-r--r--   0        0        0      588 2024-04-03 10:10:39.096024 keble_chains-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      914 1970-01-01 00:00:00.000000 keble_chains-0.0.6/PKG-INFO
```

### Comparing `keble_chains-0.0.5/LICENSE` & `keble_chains-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `keble_chains-0.0.5/keble_chains/chains.py` & `keble_chains-0.0.6/keble_chains/chains.py`

 * *Files identical despite different names*

### Comparing `keble_chains-0.0.5/keble_chains/exceptions/openai.py` & `keble_chains-0.0.6/keble_chains/exceptions/openai.py`

 * *Files identical despite different names*

### Comparing `keble_chains-0.0.5/keble_chains/export/export.py` & `keble_chains-0.0.6/keble_chains/export/export.py`

 * *Files identical despite different names*

### Comparing `keble_chains-0.0.5/keble_chains/interact/ai/azure.py` & `keble_chains-0.0.6/keble_chains/interact/ai/azure.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,33 @@
+from httpx import Timeout
 from openai import APIStatusError, ChatCompletion, AzureOpenAI
 from typing import List, Optional, Iterator
 from langchain_openai import AzureOpenAIEmbeddings
 from ...typings.ai import AiModel, AiModelTokenManager, AiMessageRole, AiPrompt, Vector
 from ...exceptions import raise_oai_error, OaiCompletionAPINonStopFinishReasonError
 
 
 class AzureAiModel(AiModel):
     def __init__(self, *, deployment: str,
                  azure_endpoint: str,
                  azure_api_key: str,
                  azure_api_version: str,
                  token_manager: Optional[AiModelTokenManager] = None,
                  tpm: int,
-                 max_token: int
+                 max_token: int,
+                 client_timeout: Optional[float, Timeout] = None,
                  ):
         self.__azure_endpoint = azure_endpoint
         self.__api_key = azure_api_key
         self.__azure_api_version = azure_api_version
         self.__deployment = deployment
         self.__token_manager = token_manager
         self.__tpm = tpm
         self.__max_token = max_token
+        self.__client_timeout = client_timeout
 
     @property
     def tpm(self):
         return self.__tpm
 
     @property
     def max_token(self):
@@ -124,14 +127,22 @@
 
         # single string
         require_token = AiModel.string_tokens("".join(texts) if isinstance(texts, list) else texts)
         self.__wait_allow_token(require_token)
         return client.embed_query(texts)
 
     def get_autocomplete_client(self) -> AzureOpenAI:
+        if self.__client_timeout is not None:
+            return AzureOpenAI(
+                api_version=self.__azure_api_version,
+                azure_endpoint=self.__azure_endpoint,
+                azure_deployment=self.__deployment,
+                api_key=self.__api_key,
+                timeout=self.__client_timeout
+            )
         return AzureOpenAI(
             api_version=self.__azure_api_version,
             azure_endpoint=self.__azure_endpoint,
             azure_deployment=self.__deployment,
             api_key=self.__api_key
         )
```

### Comparing `keble_chains-0.0.5/keble_chains/interact/ai/fake.py` & `keble_chains-0.0.6/keble_chains/interact/ai/fake.py`

 * *Files identical despite different names*

### Comparing `keble_chains-0.0.5/keble_chains/interact/ai/session.py` & `keble_chains-0.0.6/keble_chains/interact/ai/session.py`

 * *Files identical despite different names*

### Comparing `keble_chains-0.0.5/keble_chains/interact/ai/token_manager.py` & `keble_chains-0.0.6/keble_chains/interact/ai/token_manager.py`

 * *Files identical despite different names*

### Comparing `keble_chains-0.0.5/keble_chains/interact/m14/m14_compressors.py` & `keble_chains-0.0.6/keble_chains/interact/m14/m14_compressors.py`

 * *Files identical despite different names*

### Comparing `keble_chains-0.0.5/keble_chains/interact/m14/m14_session.py` & `keble_chains-0.0.6/keble_chains/interact/m14/m14_session.py`

 * *Files identical despite different names*

### Comparing `keble_chains-0.0.5/keble_chains/template/chat.py` & `keble_chains-0.0.6/keble_chains/template/chat.py`

 * *Files identical despite different names*

### Comparing `keble_chains-0.0.5/keble_chains/template/email.py` & `keble_chains-0.0.6/keble_chains/template/email.py`

 * *Files identical despite different names*

### Comparing `keble_chains-0.0.5/keble_chains/tuning/datasets.py` & `keble_chains-0.0.6/keble_chains/tuning/datasets.py`

 * *Files identical despite different names*

### Comparing `keble_chains-0.0.5/keble_chains/typings/__init__.py` & `keble_chains-0.0.6/keble_chains/typings/__init__.py`

 * *Files identical despite different names*

### Comparing `keble_chains-0.0.5/keble_chains/typings/abc.py` & `keble_chains-0.0.6/keble_chains/typings/abc.py`

 * *Files identical despite different names*

### Comparing `keble_chains-0.0.5/keble_chains/typings/ai.py` & `keble_chains-0.0.6/keble_chains/typings/ai.py`

 * *Files identical despite different names*

### Comparing `keble_chains-0.0.5/keble_chains/typings/dataset.py` & `keble_chains-0.0.6/keble_chains/typings/dataset.py`

 * *Files identical despite different names*

### Comparing `keble_chains-0.0.5/keble_chains/typings/export.py` & `keble_chains-0.0.6/keble_chains/typings/export.py`

 * *Files identical despite different names*

### Comparing `keble_chains-0.0.5/keble_chains/utils/main.py` & `keble_chains-0.0.6/keble_chains/utils/main.py`

 * *Files identical despite different names*

### Comparing `keble_chains-0.0.5/pyproject.toml` & `keble_chains-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "keble-chains"
-version = "0.0.5"
+version = "0.0.6"
 description = "Keble ai model toolkit"
 authors = ["zhenhao-ma <bob0103779@gmail.com>"]
 readme = "README.md"
 packages = [{include = "keble_chains"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `keble_chains-0.0.5/PKG-INFO` & `keble_chains-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keble-chains
-Version: 0.0.5
+Version: 0.0.6
 Summary: Keble ai model toolkit
 Author: zhenhao-ma
 Author-email: bob0103779@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

