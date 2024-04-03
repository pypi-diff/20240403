# Comparing `tmp/onepasswordconnectsdk-1.5.0.tar.gz` & `tmp/onepasswordconnectsdk-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onepasswordconnectsdk-1.5.0.tar", max compression
+gzip compressed data, was "onepasswordconnectsdk-1.5.1.tar", max compression
```

## Comparing `onepasswordconnectsdk-1.5.0.tar` & `onepasswordconnectsdk-1.5.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1069 2024-04-02 16:40:12.005767 onepasswordconnectsdk-1.5.0/LICENSE.md
--rw-r--r--   0        0        0     3313 2024-04-02 16:40:12.005767 onepasswordconnectsdk-1.5.0/README.md
--rw-r--r--   0        0        0      681 2024-04-02 16:40:12.005767 onepasswordconnectsdk-1.5.0/pyproject.toml
--rw-r--r--   0        0        0      424 2024-04-02 16:40:12.005767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/__init__.py
--rw-r--r--   0        0        0    14399 2024-04-02 16:40:12.005767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/async_client.py
--rw-r--r--   0        0        0    15938 2024-04-02 16:40:12.005767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/client.py
--rw-r--r--   0        0        0     7361 2024-04-02 16:40:12.005767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/config.py
--rw-r--r--   0        0        0        0 2024-04-02 16:40:12.005767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/connect.py
--rw-r--r--   0        0        0      473 2024-04-02 16:40:12.005767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/errors.py
--rw-r--r--   0        0        0     1122 2024-04-02 16:40:12.005767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/__init__.py
--rw-r--r--   0        0        0      145 2024-04-02 16:40:12.005767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/constants.py
--rw-r--r--   0        0        0     3691 2024-04-02 16:40:12.005767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/error.py
--rw-r--r--   0        0        0     9220 2024-04-02 16:40:12.009767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/field.py
--rw-r--r--   0        0        0     2830 2024-04-02 16:40:12.009767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/field_section.py
--rw-r--r--   0        0        0     2745 2024-04-02 16:40:12.009767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/file.py
--rw-r--r--   0        0        0     6599 2024-04-02 16:40:12.009767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/generator_recipe.py
--rw-r--r--   0        0        0    10861 2024-04-02 16:40:12.009767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/item.py
--rw-r--r--   0        0        0     3610 2024-04-02 16:40:12.009767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/item_details.py
--rw-r--r--   0        0        0     3499 2024-04-02 16:40:12.009767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/item_urls.py
--rw-r--r--   0        0        0     2846 2024-04-02 16:40:12.009767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/item_vault.py
--rw-r--r--   0        0        0       93 2024-04-02 16:40:12.009767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/parsed_field.py
--rw-r--r--   0        0        0      212 2024-04-02 16:40:12.009767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/parsed_item.py
--rw-r--r--   0        0        0     3341 2024-04-02 16:40:12.009767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/section.py
--rw-r--r--   0        0        0     9652 2024-04-02 16:40:12.009767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/summary_item.py
--rw-r--r--   0        0        0     8766 2024-04-02 16:40:12.009767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/vault.py
--rw-r--r--   0        0        0     6778 2024-04-02 16:40:12.009767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/serializer.py
--rw-r--r--   0        0        0     2104 2024-04-02 16:40:12.009767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/utils.py
--rw-r--r--   0        0        0     4291 1970-01-01 00:00:00.000000 onepasswordconnectsdk-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-03 17:56:26.828720 onepasswordconnectsdk-1.5.1/LICENSE.md
+-rw-r--r--   0        0        0     3321 2024-04-03 17:56:26.828720 onepasswordconnectsdk-1.5.1/README.md
+-rw-r--r--   0        0        0      681 2024-04-03 17:56:26.828720 onepasswordconnectsdk-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0      424 2024-04-03 17:56:26.828720 onepasswordconnectsdk-1.5.1/src/onepasswordconnectsdk/__init__.py
+-rw-r--r--   0        0        0    14352 2024-04-03 17:56:26.828720 onepasswordconnectsdk-1.5.1/src/onepasswordconnectsdk/async_client.py
+-rw-r--r--   0        0        0    15938 2024-04-03 17:56:26.828720 onepasswordconnectsdk-1.5.1/src/onepasswordconnectsdk/client.py
+-rw-r--r--   0        0        0     7361 2024-04-03 17:56:26.828720 onepasswordconnectsdk-1.5.1/src/onepasswordconnectsdk/config.py
+-rw-r--r--   0        0        0        0 2024-04-03 17:56:26.828720 onepasswordconnectsdk-1.5.1/src/onepasswordconnectsdk/connect.py
+-rw-r--r--   0        0        0      473 2024-04-03 17:56:26.828720 onepasswordconnectsdk-1.5.1/src/onepasswordconnectsdk/errors.py
+-rw-r--r--   0        0        0     1122 2024-04-03 17:56:26.828720 onepasswordconnectsdk-1.5.1/src/onepasswordconnectsdk/models/__init__.py
+-rw-r--r--   0        0        0      145 2024-04-03 17:56:26.828720 onepasswordconnectsdk-1.5.1/src/onepasswordconnectsdk/models/constants.py
+-rw-r--r--   0        0        0     3691 2024-04-03 17:56:26.828720 onepasswordconnectsdk-1.5.1/src/onepasswordconnectsdk/models/error.py
+-rw-r--r--   0        0        0     9220 2024-04-03 17:56:26.828720 onepasswordconnectsdk-1.5.1/src/onepasswordconnectsdk/models/field.py
+-rw-r--r--   0        0        0     2830 2024-04-03 17:56:26.828720 onepasswordconnectsdk-1.5.1/src/onepasswordconnectsdk/models/field_section.py
+-rw-r--r--   0        0        0     2745 2024-04-03 17:56:26.828720 onepasswordconnectsdk-1.5.1/src/onepasswordconnectsdk/models/file.py
+-rw-r--r--   0        0        0     6599 2024-04-03 17:56:26.828720 onepasswordconnectsdk-1.5.1/src/onepasswordconnectsdk/models/generator_recipe.py
+-rw-r--r--   0        0        0    10861 2024-04-03 17:56:26.828720 onepasswordconnectsdk-1.5.1/src/onepasswordconnectsdk/models/item.py
+-rw-r--r--   0        0        0     3610 2024-04-03 17:56:26.828720 onepasswordconnectsdk-1.5.1/src/onepasswordconnectsdk/models/item_details.py
+-rw-r--r--   0        0        0     3499 2024-04-03 17:56:26.828720 onepasswordconnectsdk-1.5.1/src/onepasswordconnectsdk/models/item_urls.py
+-rw-r--r--   0        0        0     2846 2024-04-03 17:56:26.828720 onepasswordconnectsdk-1.5.1/src/onepasswordconnectsdk/models/item_vault.py
+-rw-r--r--   0        0        0       93 2024-04-03 17:56:26.828720 onepasswordconnectsdk-1.5.1/src/onepasswordconnectsdk/models/parsed_field.py
+-rw-r--r--   0        0        0      212 2024-04-03 17:56:26.828720 onepasswordconnectsdk-1.5.1/src/onepasswordconnectsdk/models/parsed_item.py
+-rw-r--r--   0        0        0     3341 2024-04-03 17:56:26.828720 onepasswordconnectsdk-1.5.1/src/onepasswordconnectsdk/models/section.py
+-rw-r--r--   0        0        0     9652 2024-04-03 17:56:26.828720 onepasswordconnectsdk-1.5.1/src/onepasswordconnectsdk/models/summary_item.py
+-rw-r--r--   0        0        0     8766 2024-04-03 17:56:26.828720 onepasswordconnectsdk-1.5.1/src/onepasswordconnectsdk/models/vault.py
+-rw-r--r--   0        0        0     6778 2024-04-03 17:56:26.828720 onepasswordconnectsdk-1.5.1/src/onepasswordconnectsdk/serializer.py
+-rw-r--r--   0        0        0     2249 2024-04-03 17:56:26.828720 onepasswordconnectsdk-1.5.1/src/onepasswordconnectsdk/utils.py
+-rw-r--r--   0        0        0     4299 1970-01-01 00:00:00.000000 onepasswordconnectsdk-1.5.1/PKG-INFO
```

### Comparing `onepasswordconnectsdk-1.5.0/LICENSE.md` & `onepasswordconnectsdk-1.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `onepasswordconnectsdk-1.5.0/README.md` & `onepasswordconnectsdk-1.5.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -28,18 +28,18 @@
 2. Export the `OP_CONNECT_HOST` and `OP_CONNECT_TOKEN` environment variables:
 
    ```sh
    export OP_CONNECT_HOST=<your-connect-host> && \
    export OP_CONNECT_TOKEN=<your-connect-token>
    ```
    
-   2.1 If you need a higher timeout on the client requests you can export `OP_CLIENT_REQUEST_TIMEOUT` environment variable:
+   2.1 If you need a higher timeout on the client requests you can export `OP_CONNECT_CLIENT_REQ_TIMEOUT` environment variable:
    ```sh
    # set the timeout to 90 seconds
-   export OP_CLIENT_REQUEST_TIMEOUT=90
+   export OP_CONNECT_CLIENT_REQ_TIMEOUT=90
    ```
 
 3. Use the SDK:
 
    - Read a secret:
 
      ```python
```

#### html2text {}

```diff
@@ -8,29 +8,30 @@
 simplify accessing items in 1Password vaults. ## ðª See it in action Check
 the [Python Connect SDK Example](example/README.md) to see an example of item
 manipulation using the SDK that you can execute on your machine. ## â¨ Get
 started 1. Install the 1Password Connect Python SDK: ```sh pip install
 onepasswordconnectsdk ``` 2. Export the `OP_CONNECT_HOST` and
 `OP_CONNECT_TOKEN` environment variables: ```sh export OP_CONNECT_HOST= && \
 export OP_CONNECT_TOKEN= ``` 2.1 If you need a higher timeout on the client
-requests you can export `OP_CLIENT_REQUEST_TIMEOUT` environment variable: ```sh
-# set the timeout to 90 seconds export OP_CLIENT_REQUEST_TIMEOUT=90 ``` 3. Use
-the SDK: - Read a secret: ```python from onepasswordconnectsdk.client import
-( Client, new_client_from_environment, ) connect_client: Client =
-new_client_from_environment() client.get_item("{item_id}", "{vault_id}") ``` -
-Write a secret: ```python from onepasswordconnectsdk.client import ( Client,
-new_client_from_environment, } from onepasswordconnectsdk.models import ( Item,
-ItemVault, Field ) connect_client: Client = new_client_from_environment() #
-Example item creation. Create an item with your desired arguments. item = Item
-( vault=ItemVault(id=op_vault), id="custom_id", title="newtitle",
-category="LOGIN", tags=["1password-connect"], fields=[Field(value="new_user",
-purpose="USERNAME")], ) new_item = connect_client.create_item(op_vault, item)
-``` For more examples of how to use the SDK, check out [USAGE.md](USAGE.md). ##
-ð Community & Support - File an [issue](https://github.com/1Password/
-connect-sdk-python/issues) for bugs and feature requests. - Join the [Developer
-Slack workspace](https://join.slack.com/t/1password-devs/shared_invite/zt-
-1halo11ps-6o9pEv96xZ3LtX_VE0fJQA). - Subscribe to the [Developer Newsletter]
-(https://1password.com/dev-subscribe/). ## ð Security 1Password requests you
-practice responsible disclosure if you discover a vulnerability. Please file
-requests via [**BugCrowd**](https://bugcrowd.com/agilebits). For information
-about security practices, please visit the [1Password Bug Bounty Program]
-(https://bugcrowd.com/agilebits).
+requests you can export `OP_CONNECT_CLIENT_REQ_TIMEOUT` environment variable:
+```sh # set the timeout to 90 seconds export OP_CONNECT_CLIENT_REQ_TIMEOUT=90
+``` 3. Use the SDK: - Read a secret: ```python from
+onepasswordconnectsdk.client import ( Client, new_client_from_environment, )
+connect_client: Client = new_client_from_environment() client.get_item("
+{item_id}", "{vault_id}") ``` - Write a secret: ```python from
+onepasswordconnectsdk.client import ( Client, new_client_from_environment, }
+from onepasswordconnectsdk.models import ( Item, ItemVault, Field )
+connect_client: Client = new_client_from_environment() # Example item creation.
+Create an item with your desired arguments. item = Item( vault=ItemVault
+(id=op_vault), id="custom_id", title="newtitle", category="LOGIN", tags=
+["1password-connect"], fields=[Field(value="new_user", purpose="USERNAME")], )
+new_item = connect_client.create_item(op_vault, item) ``` For more examples of
+how to use the SDK, check out [USAGE.md](USAGE.md). ## ð Community & Support
+- File an [issue](https://github.com/1Password/connect-sdk-python/issues) for
+bugs and feature requests. - Join the [Developer Slack workspace](https://
+join.slack.com/t/1password-devs/shared_invite/zt-1halo11ps-
+6o9pEv96xZ3LtX_VE0fJQA). - Subscribe to the [Developer Newsletter](https://
+1password.com/dev-subscribe/). ## ð Security 1Password requests you practice
+responsible disclosure if you discover a vulnerability. Please file requests
+via [**BugCrowd**](https://bugcrowd.com/agilebits). For information about
+security practices, please visit the [1Password Bug Bounty Program](https://
+bugcrowd.com/agilebits).
```

### Comparing `onepasswordconnectsdk-1.5.0/pyproject.toml` & `onepasswordconnectsdk-1.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "onepasswordconnectsdk"
-version = "1.5.0"
+version = "1.5.1"
 description = "Python SDK for 1Password Connect"
 license = "MIT"
 authors = ["1Password"]
 readme = "README.md"
 repository = "https://github.com/1Password/connect-sdk-python"
 
 [tool.poetry.urls]
```

### Comparing `onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/async_client.py` & `onepasswordconnectsdk-1.5.1/src/onepasswordconnectsdk/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,14 @@
         """Initialize async client"""
         self.url = url
         self.token = token
         self.session = self.create_session(url, token)
         self.serializer = Serializer()
 
     def create_session(self, url: str, token: str) -> httpx.AsyncClient:
-        # import here to avoid circular import
         return httpx.AsyncClient(base_url=url, headers=self.build_headers(token), timeout=get_timeout())
 
     def build_headers(self, token: str) -> Dict[str, str]:
         return build_headers(token)
 
     async def __aexit__(self):
         await self.session.aclose()
```

### Comparing `onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/client.py` & `onepasswordconnectsdk-1.5.1/src/onepasswordconnectsdk/client.py`

 * *Files identical despite different names*

### Comparing `onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/config.py` & `onepasswordconnectsdk-1.5.1/src/onepasswordconnectsdk/config.py`

 * *Files identical despite different names*

### Comparing `onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/__init__.py` & `onepasswordconnectsdk-1.5.1/src/onepasswordconnectsdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/error.py` & `onepasswordconnectsdk-1.5.1/src/onepasswordconnectsdk/models/error.py`

 * *Files identical despite different names*

### Comparing `onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/field.py` & `onepasswordconnectsdk-1.5.1/src/onepasswordconnectsdk/models/field.py`

 * *Files identical despite different names*

### Comparing `onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/field_section.py` & `onepasswordconnectsdk-1.5.1/src/onepasswordconnectsdk/models/field_section.py`

 * *Files identical despite different names*

### Comparing `onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/file.py` & `onepasswordconnectsdk-1.5.1/src/onepasswordconnectsdk/models/file.py`

 * *Files identical despite different names*

### Comparing `onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/generator_recipe.py` & `onepasswordconnectsdk-1.5.1/src/onepasswordconnectsdk/models/generator_recipe.py`

 * *Files identical despite different names*

### Comparing `onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/item.py` & `onepasswordconnectsdk-1.5.1/src/onepasswordconnectsdk/models/item.py`

 * *Files identical despite different names*

### Comparing `onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/item_details.py` & `onepasswordconnectsdk-1.5.1/src/onepasswordconnectsdk/models/item_details.py`

 * *Files identical despite different names*

### Comparing `onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/item_urls.py` & `onepasswordconnectsdk-1.5.1/src/onepasswordconnectsdk/models/item_urls.py`

 * *Files identical despite different names*

### Comparing `onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/item_vault.py` & `onepasswordconnectsdk-1.5.1/src/onepasswordconnectsdk/models/item_vault.py`

 * *Files identical despite different names*

### Comparing `onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/section.py` & `onepasswordconnectsdk-1.5.1/src/onepasswordconnectsdk/models/section.py`

 * *Files identical despite different names*

### Comparing `onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/summary_item.py` & `onepasswordconnectsdk-1.5.1/src/onepasswordconnectsdk/models/summary_item.py`

 * *Files identical despite different names*

### Comparing `onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/vault.py` & `onepasswordconnectsdk-1.5.1/src/onepasswordconnectsdk/models/vault.py`

 * *Files identical despite different names*

### Comparing `onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/serializer.py` & `onepasswordconnectsdk-1.5.1/src/onepasswordconnectsdk/serializer.py`

 * *Files identical despite different names*

### Comparing `onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/utils.py` & `onepasswordconnectsdk-1.5.1/src/onepasswordconnectsdk/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import os
-from typing import Union
 
-from httpx import USE_CLIENT_DEFAULT
-from httpx._client import UseClientDefault
+from httpx._client import DEFAULT_TIMEOUT_CONFIG, Timeout
 
 UUIDLength = 26
 ENV_CLIENT_REQUEST_TIMEOUT = "OP_CONNECT_CLIENT_REQ_TIMEOUT"
 
 
 def is_valid_uuid(uuid):
     if len(uuid) is not UUIDLength:
@@ -64,11 +62,17 @@
     def _append_path(self, path_chunk: str = None, query: str = None) -> 'PathBuilder':
         if path_chunk is not None:
             self.path += f"/{path_chunk}"
         if query is not None:
             self.path += f"?{query}"
 
 
-def get_timeout() -> Union[int, UseClientDefault]:
+def get_timeout() -> Timeout:
     """Get the timeout to be used in the HTTP Client"""
-    timeout = int(os.getenv(ENV_CLIENT_REQUEST_TIMEOUT, 0))
-    return timeout if timeout else USE_CLIENT_DEFAULT
+    raw_timeout = os.getenv(ENV_CLIENT_REQUEST_TIMEOUT, '0.0')
+    if raw_timeout == 'None':
+        return Timeout(None)  # disable all timeouts
+    elif raw_timeout.isnumeric():
+        timeout = float(raw_timeout)
+        return timeout if timeout else DEFAULT_TIMEOUT_CONFIG
+    else:
+        return DEFAULT_TIMEOUT_CONFIG
```

### Comparing `onepasswordconnectsdk-1.5.0/PKG-INFO` & `onepasswordconnectsdk-1.5.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onepasswordconnectsdk
-Version: 1.5.0
+Version: 1.5.1
 Summary: Python SDK for 1Password Connect
 Home-page: https://github.com/1Password/connect-sdk-python
 License: MIT
 Author: 1Password
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -51,18 +51,18 @@
 2. Export the `OP_CONNECT_HOST` and `OP_CONNECT_TOKEN` environment variables:
 
    ```sh
    export OP_CONNECT_HOST=<your-connect-host> && \
    export OP_CONNECT_TOKEN=<your-connect-token>
    ```
    
-   2.1 If you need a higher timeout on the client requests you can export `OP_CLIENT_REQUEST_TIMEOUT` environment variable:
+   2.1 If you need a higher timeout on the client requests you can export `OP_CONNECT_CLIENT_REQ_TIMEOUT` environment variable:
    ```sh
    # set the timeout to 90 seconds
-   export OP_CLIENT_REQUEST_TIMEOUT=90
+   export OP_CONNECT_CLIENT_REQ_TIMEOUT=90
    ```
 
 3. Use the SDK:
 
    - Read a secret:
 
      ```python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: onepasswordconnectsdk Version: 1.5.0 Summary:
+Metadata-Version: 2.1 Name: onepasswordconnectsdk Version: 1.5.1 Summary:
 Python SDK for 1Password Connect Home-page: https://github.com/1Password/
 connect-sdk-python License: MIT Author: 1Password Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
@@ -21,29 +21,30 @@
 simplify accessing items in 1Password vaults. ## ðª See it in action Check
 the [Python Connect SDK Example](example/README.md) to see an example of item
 manipulation using the SDK that you can execute on your machine. ## â¨ Get
 started 1. Install the 1Password Connect Python SDK: ```sh pip install
 onepasswordconnectsdk ``` 2. Export the `OP_CONNECT_HOST` and
 `OP_CONNECT_TOKEN` environment variables: ```sh export OP_CONNECT_HOST= && \
 export OP_CONNECT_TOKEN= ``` 2.1 If you need a higher timeout on the client
-requests you can export `OP_CLIENT_REQUEST_TIMEOUT` environment variable: ```sh
-# set the timeout to 90 seconds export OP_CLIENT_REQUEST_TIMEOUT=90 ``` 3. Use
-the SDK: - Read a secret: ```python from onepasswordconnectsdk.client import
-( Client, new_client_from_environment, ) connect_client: Client =
-new_client_from_environment() client.get_item("{item_id}", "{vault_id}") ``` -
-Write a secret: ```python from onepasswordconnectsdk.client import ( Client,
-new_client_from_environment, } from onepasswordconnectsdk.models import ( Item,
-ItemVault, Field ) connect_client: Client = new_client_from_environment() #
-Example item creation. Create an item with your desired arguments. item = Item
-( vault=ItemVault(id=op_vault), id="custom_id", title="newtitle",
-category="LOGIN", tags=["1password-connect"], fields=[Field(value="new_user",
-purpose="USERNAME")], ) new_item = connect_client.create_item(op_vault, item)
-``` For more examples of how to use the SDK, check out [USAGE.md](USAGE.md). ##
-ð Community & Support - File an [issue](https://github.com/1Password/
-connect-sdk-python/issues) for bugs and feature requests. - Join the [Developer
-Slack workspace](https://join.slack.com/t/1password-devs/shared_invite/zt-
-1halo11ps-6o9pEv96xZ3LtX_VE0fJQA). - Subscribe to the [Developer Newsletter]
-(https://1password.com/dev-subscribe/). ## ð Security 1Password requests you
-practice responsible disclosure if you discover a vulnerability. Please file
-requests via [**BugCrowd**](https://bugcrowd.com/agilebits). For information
-about security practices, please visit the [1Password Bug Bounty Program]
-(https://bugcrowd.com/agilebits).
+requests you can export `OP_CONNECT_CLIENT_REQ_TIMEOUT` environment variable:
+```sh # set the timeout to 90 seconds export OP_CONNECT_CLIENT_REQ_TIMEOUT=90
+``` 3. Use the SDK: - Read a secret: ```python from
+onepasswordconnectsdk.client import ( Client, new_client_from_environment, )
+connect_client: Client = new_client_from_environment() client.get_item("
+{item_id}", "{vault_id}") ``` - Write a secret: ```python from
+onepasswordconnectsdk.client import ( Client, new_client_from_environment, }
+from onepasswordconnectsdk.models import ( Item, ItemVault, Field )
+connect_client: Client = new_client_from_environment() # Example item creation.
+Create an item with your desired arguments. item = Item( vault=ItemVault
+(id=op_vault), id="custom_id", title="newtitle", category="LOGIN", tags=
+["1password-connect"], fields=[Field(value="new_user", purpose="USERNAME")], )
+new_item = connect_client.create_item(op_vault, item) ``` For more examples of
+how to use the SDK, check out [USAGE.md](USAGE.md). ## ð Community & Support
+- File an [issue](https://github.com/1Password/connect-sdk-python/issues) for
+bugs and feature requests. - Join the [Developer Slack workspace](https://
+join.slack.com/t/1password-devs/shared_invite/zt-1halo11ps-
+6o9pEv96xZ3LtX_VE0fJQA). - Subscribe to the [Developer Newsletter](https://
+1password.com/dev-subscribe/). ## ð Security 1Password requests you practice
+responsible disclosure if you discover a vulnerability. Please file requests
+via [**BugCrowd**](https://bugcrowd.com/agilebits). For information about
+security practices, please visit the [1Password Bug Bounty Program](https://
+bugcrowd.com/agilebits).
```

