# Comparing `tmp/unifyai-0.3.2.tar.gz` & `tmp/unifyai-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unifyai-0.3.2.tar", max compression
+gzip compressed data, was "unifyai-0.4.0.tar", max compression
```

## Comparing `unifyai-0.3.2.tar` & `unifyai-0.4.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11336 2024-04-02 01:55:16.865353 unifyai-0.3.2/LICENSE
--rw-r--r--   0        0        0     5274 2024-04-02 08:22:14.025331 unifyai-0.3.2/README.md
--rw-r--r--   0        0        0      998 2024-04-02 08:22:41.117331 unifyai-0.3.2/pyproject.toml
--rw-r--r--   0        0        0       88 2024-04-02 01:55:16.869353 unifyai-0.3.2/unifyai/__init__.py
--rw-r--r--   0        0        0     8405 2024-04-02 01:55:16.869353 unifyai-0.3.2/unifyai/clients.py
--rw-r--r--   0        0        0     1166 2024-04-02 01:55:16.873353 unifyai-0.3.2/unifyai/exceptions.py
--rw-r--r--   0        0        0     4100 2024-04-02 01:55:16.873353 unifyai-0.3.2/unifyai/tests.py
--rw-r--r--   0        0        0     5915 1970-01-01 00:00:00.000000 unifyai-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    11336 2024-04-02 01:55:16.865353 unifyai-0.4.0/LICENSE
+-rw-r--r--   0        0        0     5465 2024-04-03 10:55:32.016364 unifyai-0.4.0/README.md
+-rw-r--r--   0        0        0      998 2024-04-03 11:20:47.800342 unifyai-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       88 2024-04-02 01:55:16.869353 unifyai-0.4.0/unifyai/__init__.py
+-rw-r--r--   0        0        0    10479 2024-04-03 11:19:06.804344 unifyai-0.4.0/unifyai/clients.py
+-rw-r--r--   0        0        0     1166 2024-04-02 01:55:16.873353 unifyai-0.4.0/unifyai/exceptions.py
+-rw-r--r--   0        0        0     4100 2024-04-02 01:55:16.873353 unifyai-0.4.0/unifyai/tests.py
+-rw-r--r--   0        0        0     6106 1970-01-01 00:00:00.000000 unifyai-0.4.0/PKG-INFO
```

### Comparing `unifyai-0.3.2/LICENSE` & `unifyai-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unifyai-0.3.2/README.md` & `unifyai-0.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -116,14 +116,20 @@
     async_stream = await async_unify.generate(messages="Hello Llama! Who was Isaac Newton?", model="llama-2-13b-chat", provider="anyscale", stream=True)
     async for chunk in async_stream:
         print(chunk, end="")
 
 asyncio.run(main())
 ```
 
+## Get Current Credit Balance
+You can use the `.get_credit_balance` method to the credit balance for the authenticated account as follows:
+```python
+credits = unify.get_credit_balance()
+```
+
 ## Dynamic Routing
 As evidenced by our [benchmarks](https://unify.ai/hub), the optimal provider for each model varies by geographic location and time of day due to fluctuating API performances. With our dynamic routing, we automatically direct your requests to the "top-performing provider" at that moment. To enable this feature, simply replace your query's provider with one of the [available routing modes](https://unify.ai/docs/hub/concepts/runtime_routing.html#available-modes). As an example, you can query the `llama-2-7b-chat` endpoint to get the provider with the lowest input-cost as follows:
 
 ```python
 import os
 from unifyai import Unify
 unify = Unify(
```

### Comparing `unifyai-0.3.2/pyproject.toml` & `unifyai-0.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unifyai"
-version = "0.3.2"
+version = "0.4.0"
 readme = "README.md"
 description = "A Python package for interacting with the Unify API"
 authors = ["Unify <hello@unify.com>"]
 repository = "https://github.com/unifyai/unify-llm-python"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `unifyai-0.3.2/unifyai/clients.py` & `unifyai-0.4.0/unifyai/clients.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 from typing import AsyncGenerator, Dict, Generator, List, Optional, Union
 
 import openai
-from unifyai.exceptions import UnifyError, status_error_map
+import requests
+from unifyai.exceptions import BadRequestError, UnifyError, status_error_map
 
 
 def _validate_api_key(api_key: Optional[str]) -> str:
     if api_key is None:
         api_key = os.environ.get("UNIFY_KEY")
     if api_key is None:
         raise KeyError(
@@ -80,14 +81,40 @@
         else:
             contents.extend(messages)
 
         if stream:
             return self._generate_stream(contents, model, provider)
         return self._generate_non_stream(contents, model, provider)
 
+    def get_credit_balance(self) -> Optional[int]:
+        # noqa: DAR201, DAR401
+        """
+        Get the remaining credits left on your account.
+
+        Returns:
+            int or None: The remaining credits on the account
+            if successful, otherwise None.
+        Raises:
+            BadRequestError: If there was an HTTP error.
+            ValueError: If there was an error parsing the JSON response.
+        """
+        url = "https://api.unify.ai/v0/get_credits"
+        headers = {
+            "accept": "application/json",
+            "Authorization": f"Bearer {self.api_key}",
+        }
+        try:
+            response = requests.get(url, headers=headers, timeout=10)
+            response.raise_for_status()
+            return response.json()["credits"]
+        except requests.RequestException as e:
+            raise BadRequestError("There was an error with the request.") from e
+        except (KeyError, ValueError) as e:
+            raise ValueError("Error parsing JSON response.") from e
+
     def _generate_stream(
         self,
         messages: List[Dict[str, str]],
         model: str,
         provider: str,
     ) -> Generator[str, None, None]:
         try:
@@ -143,14 +170,41 @@
             self.client = openai.AsyncOpenAI(
                 base_url="https://api.unify.ai/v0/",
                 api_key=self.api_key,
             )
         except openai.APIStatusError as e:
             raise UnifyError(f"Failed to initialize Unify client: {str(e)}")
 
+    def get_credit_balance(self) -> Optional[int]:
+        # noqa: DAR201, DAR401
+        """
+        Get the remaining credits left on your account.
+
+        Returns:
+            int or None: The remaining credits on the account
+            if successful, otherwise None.
+
+        Raises:
+            BadRequestError: If there was an HTTP error.
+            ValueError: If there was an error parsing the JSON response.
+        """
+        url = "https://api.unify.ai/v0/get_credits"
+        headers = {
+            "accept": "application/json",
+            "Authorization": f"Bearer {self.api_key}",
+        }
+        try:
+            response = requests.get(url, headers=headers, timeout=10)
+            response.raise_for_status()
+            return response.json()["credits"]
+        except requests.RequestException as e:
+            raise BadRequestError("There was an error with the request.") from e
+        except (KeyError, ValueError) as e:
+            raise ValueError("Error parsing JSON response.") from e
+
     async def generate(  # noqa: WPS234, WPS211
         self,
         messages: Union[str, List[Dict[str, str]]],
         system_prompt: Optional[str] = None,
         model: str = "llama-2-13b-chat",
         provider: str = "anyscale",
         stream: bool = False,
```

### Comparing `unifyai-0.3.2/unifyai/exceptions.py` & `unifyai-0.4.0/unifyai/exceptions.py`

 * *Files identical despite different names*

### Comparing `unifyai-0.3.2/unifyai/tests.py` & `unifyai-0.4.0/unifyai/tests.py`

 * *Files identical despite different names*

### Comparing `unifyai-0.3.2/PKG-INFO` & `unifyai-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unifyai
-Version: 0.3.2
+Version: 0.4.0
 Summary: A Python package for interacting with the Unify API
 Home-page: https://github.com/unifyai/unify-llm-python
 Author: Unify
 Author-email: hello@unify.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -133,14 +133,20 @@
     async_stream = await async_unify.generate(messages="Hello Llama! Who was Isaac Newton?", model="llama-2-13b-chat", provider="anyscale", stream=True)
     async for chunk in async_stream:
         print(chunk, end="")
 
 asyncio.run(main())
 ```
 
+## Get Current Credit Balance
+You can use the `.get_credit_balance` method to the credit balance for the authenticated account as follows:
+```python
+credits = unify.get_credit_balance()
+```
+
 ## Dynamic Routing
 As evidenced by our [benchmarks](https://unify.ai/hub), the optimal provider for each model varies by geographic location and time of day due to fluctuating API performances. With our dynamic routing, we automatically direct your requests to the "top-performing provider" at that moment. To enable this feature, simply replace your query's provider with one of the [available routing modes](https://unify.ai/docs/hub/concepts/runtime_routing.html#available-modes). As an example, you can query the `llama-2-7b-chat` endpoint to get the provider with the lowest input-cost as follows:
 
 ```python
 import os
 from unifyai import Unify
 unify = Unify(
```

