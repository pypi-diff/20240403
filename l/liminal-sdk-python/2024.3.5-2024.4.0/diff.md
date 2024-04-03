# Comparing `tmp/liminal_sdk_python-2024.3.5.tar.gz` & `tmp/liminal_sdk_python-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liminal_sdk_python-2024.3.5.tar", max compression
+gzip compressed data, was "liminal_sdk_python-2024.4.0.tar", max compression
```

## Comparing `liminal_sdk_python-2024.3.5.tar` & `liminal_sdk_python-2024.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    11357 2024-03-19 17:33:26.697995 liminal_sdk_python-2024.3.5/LICENSE
--rw-r--r--   0        0        0    13058 2024-03-19 17:33:26.697995 liminal_sdk_python-2024.3.5/README.md
--rw-r--r--   0        0        0       82 2024-03-19 17:33:26.697995 liminal_sdk_python-2024.3.5/liminal/__init__.py
--rw-r--r--   0        0        0      467 2024-03-19 17:33:26.697995 liminal_sdk_python-2024.3.5/liminal/auth/__init__.py
--rw-r--r--   0        0        0       34 2024-03-19 17:33:26.697995 liminal_sdk_python-2024.3.5/liminal/auth/microsoft/__init__.py
--rw-r--r--   0        0        0     2861 2024-03-19 17:33:26.697995 liminal_sdk_python-2024.3.5/liminal/auth/microsoft/device_code_flow.py
--rw-r--r--   0        0        0      873 2024-03-19 17:33:26.697995 liminal_sdk_python-2024.3.5/liminal/auth/microsoft/models.py
--rw-r--r--   0        0        0     8794 2024-03-19 17:33:26.697995 liminal_sdk_python-2024.3.5/liminal/client.py
--rw-r--r--   0        0        0      137 2024-03-19 17:33:26.697995 liminal_sdk_python-2024.3.5/liminal/const.py
--rw-r--r--   0        0        0       45 2024-03-19 17:33:26.697995 liminal_sdk_python-2024.3.5/liminal/endpoints/__init__.py
--rw-r--r--   0        0        0     2063 2024-03-19 17:33:26.697995 liminal_sdk_python-2024.3.5/liminal/endpoints/llm/__init__.py
--rw-r--r--   0        0        0     2352 2024-03-19 17:33:26.697995 liminal_sdk_python-2024.3.5/liminal/endpoints/llm/models.py
--rw-r--r--   0        0        0     4055 2024-03-19 17:33:26.697995 liminal_sdk_python-2024.3.5/liminal/endpoints/prompt/__init__.py
--rw-r--r--   0        0        0     3265 2024-03-19 17:33:26.697995 liminal_sdk_python-2024.3.5/liminal/endpoints/prompt/models.py
--rw-r--r--   0        0        0     2795 2024-03-19 17:33:26.697995 liminal_sdk_python-2024.3.5/liminal/endpoints/thread/__init__.py
--rw-r--r--   0        0        0     2162 2024-03-19 17:33:26.697995 liminal_sdk_python-2024.3.5/liminal/endpoints/thread/models.py
--rw-r--r--   0        0        0      400 2024-03-19 17:33:26.697995 liminal_sdk_python-2024.3.5/liminal/errors.py
--rw-r--r--   0        0        0       22 2024-03-19 17:33:26.697995 liminal_sdk_python-2024.3.5/liminal/helpers/__init__.py
--rw-r--r--   0        0        0      340 2024-03-19 17:33:26.697995 liminal_sdk_python-2024.3.5/liminal/helpers/model.py
--rw-r--r--   0        0        0      109 2024-03-19 17:33:26.697995 liminal_sdk_python-2024.3.5/liminal/helpers/typing.py
--rw-r--r--   0        0        0     8997 2024-03-19 17:33:26.697995 liminal_sdk_python-2024.3.5/pyproject.toml
--rw-r--r--   0        0        0    14180 1970-01-01 00:00:00.000000 liminal_sdk_python-2024.3.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-03 01:59:47.512432 liminal_sdk_python-2024.4.0/LICENSE
+-rw-r--r--   0        0        0    13136 2024-04-03 01:59:47.512432 liminal_sdk_python-2024.4.0/README.md
+-rw-r--r--   0        0        0       82 2024-04-03 01:59:47.512432 liminal_sdk_python-2024.4.0/liminal/__init__.py
+-rw-r--r--   0        0        0      524 2024-04-03 01:59:47.512432 liminal_sdk_python-2024.4.0/liminal/auth/__init__.py
+-rw-r--r--   0        0        0       34 2024-04-03 01:59:47.512432 liminal_sdk_python-2024.4.0/liminal/auth/microsoft/__init__.py
+-rw-r--r--   0        0        0     2961 2024-04-03 01:59:47.512432 liminal_sdk_python-2024.4.0/liminal/auth/microsoft/device_code_flow.py
+-rw-r--r--   0        0        0      873 2024-04-03 01:59:47.512432 liminal_sdk_python-2024.4.0/liminal/auth/microsoft/models.py
+-rw-r--r--   0        0        0     8731 2024-04-03 01:59:47.512432 liminal_sdk_python-2024.4.0/liminal/client.py
+-rw-r--r--   0        0        0      165 2024-04-03 01:59:47.512432 liminal_sdk_python-2024.4.0/liminal/const.py
+-rw-r--r--   0        0        0       45 2024-04-03 01:59:47.512432 liminal_sdk_python-2024.4.0/liminal/endpoints/__init__.py
+-rw-r--r--   0        0        0     2135 2024-04-03 01:59:47.512432 liminal_sdk_python-2024.4.0/liminal/endpoints/llm/__init__.py
+-rw-r--r--   0        0        0     2352 2024-04-03 01:59:47.512432 liminal_sdk_python-2024.4.0/liminal/endpoints/llm/models.py
+-rw-r--r--   0        0        0     5463 2024-04-03 01:59:47.512432 liminal_sdk_python-2024.4.0/liminal/endpoints/prompt/__init__.py
+-rw-r--r--   0        0        0     3264 2024-04-03 01:59:47.512432 liminal_sdk_python-2024.4.0/liminal/endpoints/prompt/models.py
+-rw-r--r--   0        0        0     2372 2024-04-03 01:59:47.512432 liminal_sdk_python-2024.4.0/liminal/endpoints/thread/__init__.py
+-rw-r--r--   0        0        0     2162 2024-04-03 01:59:47.512432 liminal_sdk_python-2024.4.0/liminal/endpoints/thread/models.py
+-rw-r--r--   0        0        0      400 2024-04-03 01:59:47.512432 liminal_sdk_python-2024.4.0/liminal/errors.py
+-rw-r--r--   0        0        0       22 2024-04-03 01:59:47.516432 liminal_sdk_python-2024.4.0/liminal/helpers/__init__.py
+-rw-r--r--   0        0        0      382 2024-04-03 01:59:47.516432 liminal_sdk_python-2024.4.0/liminal/helpers/model.py
+-rw-r--r--   0        0        0      109 2024-04-03 01:59:47.516432 liminal_sdk_python-2024.4.0/liminal/helpers/typing.py
+-rw-r--r--   0        0        0    13516 2024-04-03 01:59:47.516432 liminal_sdk_python-2024.4.0/pyproject.toml
+-rw-r--r--   0        0        0    14258 1970-01-01 00:00:00.000000 liminal_sdk_python-2024.4.0/PKG-INFO
```

### Comparing `liminal_sdk_python-2024.3.5/LICENSE` & `liminal_sdk_python-2024.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.3.5/README.md` & `liminal_sdk_python-2024.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -254,18 +254,14 @@
     # Some operations require a model instance:
     model_instance = await liminal.llm.get_model_instance("My Model")
 
     # Create a new thread:
     thread = await liminal.thread.create(model_instance.id, "New Thread")
     # >>> Thread(...)
 
-    # Get the "de-identified" (containing sensitive data) context history for a thread:
-    thread = await liminal.thread.get_deidentified_context_history(model_instance.id)
-    # >>> [DeidentifiedToken(...), DeidentifiedToken(...), DeidentifiedToken(...)]
-
 
 asyncio.run(main())
 ```
 
 ## Submitting Prompts
 
 Submitting prompts is easy:
@@ -276,40 +272,51 @@
 from liminal import Client
 from liminal.auth.microsoft.device_code_flow import DeviceCodeFlowProvider
 
 
 async def main() -> None:
     # Assuming you have an authenticated `liminal` object:
 
-    # Prompt operations require a thread:
+    # Prompt operations require a model instance:
+    model_instance = await liminal.llm.get_model_instance(model_instance_name)
+
+    # Prompt operations optionally take an existing thread:
     thread = await liminal.thread.get_by_id(123)
     # >>> Thread(...)
 
     # Analayze a prompt for sensitive info:
-    findings = await liminal.prompt.analyze(thread.id)
+    findings = await liminal.prompt.analyze(
+        model_instance.id, "Here is a sensitive prompt"
+    )
     # >>> AnalyzeResponse(...)
 
     # Cleanse input text by applying the policies defined in the Liminal admin
     # dashboard. You can optionally provide existing analysis finidings; if not
     # provided, analyze is # called automatically):
     cleansed = await liminal.prompt.cleanse(
-        thread.id, "Here is a sensitive prompt", findings=findings
+        model_instance.id,
+        "Here is a sensitive prompt",
+        findings=findings,
+        thread_id=thread.id,
     )
     # >>> CleanseResponse(...)
 
     # Submit a prompt to an LLM, cleansing it in the process (once again, providing optional
     # findings):
     response = await liminal.prompt.submit(
-        thread.id, "Here is a sensitive prompt", findings=findings
+        model_instance.id,
+        "Here is a sensitive prompt",
+        findings=findings,
+        thread_id=thread.id,
     )
-    # >>> ProcessResponse(...)
+    # >>> SubmitResponse(...)
 
     # Rehydrate a response with sensitive data:
     hydrated = await liminal.prompt.hydrate(
-        thread.id, "Here is a response to rehdyrate"
+        model_instance.id, "Here is a response to rehdyrate", thread_id=thread.id
     )
     # >>> HydrateResponse(...)
 
 
 asyncio.run(main())
 ```
```

### Comparing `liminal_sdk_python-2024.3.5/liminal/auth/microsoft/device_code_flow.py` & `liminal_sdk_python-2024.4.0/liminal/auth/microsoft/device_code_flow.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 )
 from liminal.const import LOGGER
 from liminal.errors import AuthError
 
 DEFAULT_AUTH_CHALLENGE_TIMEOUT: Final[int] = 60
 
 
-class DeviceCodeFlowProvider(AuthProvider):
+class DeviceCodeFlowProvider(AuthProvider):  # pylint: disable=too-few-public-methods
     """Define a Microsoft auth provider."""
 
     AUTHORITY_URL: Final[str] = "https://login.microsoftonline.com"
     DEFAULT_SCOPES: Final[list[str]] = ["User.Read"]
 
     def __init__(
         self,
@@ -30,14 +30,15 @@
         client_id: str,
         *,
         auth_challenge_timeout: int = DEFAULT_AUTH_CHALLENGE_TIMEOUT,
     ) -> None:
         """Initialize.
 
         Args:
+        ----
             tenant_id: The Entra ID tenant ID.
             client_id: The Entra ID client ID.
             auth_challenge_timeout: How long (in seconds) before aborting an auth
                 challenge.
 
         """
         self._auth_challenge_timeout = auth_challenge_timeout
@@ -45,22 +46,24 @@
         self._msal_app = PublicClientApplication(
             client_id=client_id, authority=f"{self.AUTHORITY_URL}/{tenant_id}"
         )
 
     async def get_access_token(self) -> str:
         """Retrieve an access token from Microsoft Entra ID (via MSAL).
 
-        Returns:
+        Returns
+        -------
             The access token.
 
-        Raises:
+        Raises
+        ------
             AuthError: If authentication fails.
 
         """
-        if accounts := self._msal_app.get_accounts():
+        if accounts := self._msal_app.get_accounts():  # noqa: SIM102
             if result := self._msal_app.acquire_token_silent_with_error(
                 self.DEFAULT_SCOPES, account=accounts[0]
             ):
                 LOGGER.debug("Retrieved access token from existing cache")
                 cached_response = MSALCacheTokenResponse.from_dict(result)
                 return cached_response.access_token
```

### Comparing `liminal_sdk_python-2024.3.5/liminal/auth/microsoft/models.py` & `liminal_sdk_python-2024.4.0/liminal/auth/microsoft/models.py`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.3.5/liminal/client.py` & `liminal_sdk_python-2024.4.0/liminal/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,41 +21,38 @@
 from liminal.endpoints.llm import LLMEndpoint
 from liminal.endpoints.prompt import PromptEndpoint
 from liminal.endpoints.thread import ThreadEndpoint
 from liminal.errors import AuthError, RequestError
 from liminal.helpers.typing import ValidatedResponseT
 
 DEFAULT_REQUEST_TIMEOUT: Final[int] = 60
-DEFAULT_SOURCE: Final[str] = "sdk"
 
 
 class Client:
     """Define the client class."""
 
     def __init__(
         self,
         auth_provider: AuthProvider,
         api_server_url: str,
         *,
-        source: str = DEFAULT_SOURCE,
         httpx_client: AsyncClient | None = None,
     ) -> None:
         """Initialize.
 
         Args:
+        ----
             auth_provider: The instantiated auth provider to use.
             api_server_url: The URL of the Liminal API server.
-            source: The source of the SDK.
             httpx_client: An optional HTTPX client to use.
 
         """
         self._api_server_url = api_server_url
         self._auth_provider = auth_provider
         self._httpx_client = httpx_client
-        self._source = source
 
         # Token information:
         self._access_token: str | None = None
         self._access_token_expires_at: datetime | None = None
         self._refresh_lock = asyncio.Lock()
         self._refresh_token: str | None = None
         self._refresh_token_callbacks: list[Callable[[str], None]] = []
@@ -75,25 +72,28 @@
         cookies: Cookies | None = None,
         params: dict[str, str] | None = None,
         json: dict[str, str] | None = None,
     ) -> Response:
         """Make a request to the Liminal API server and return a Response.
 
         Args:
+        ----
             method: The HTTP method to use.
             endpoint: The endpoint to request.
             headers: The headers to use.
             cookies: The cookies to use.
             params: The query parameters to use.
             json: The JSON body to use.
 
         Returns:
+        -------
             An HTTPX Response object.
 
         Raises:
+        ------
             RequestError: If the response fails for any reason.
 
         """
         utcnow = datetime.now(tz=UTC)
         if self._access_token_expires_at and utcnow >= self._access_token_expires_at:
             LOGGER.debug("Access token expired, refreshing...")
             self._access_token = None
@@ -103,18 +103,14 @@
         url = f"{self._api_server_url}{endpoint}"
 
         if not headers:
             headers = {}
         if self._access_token:
             headers["Authorization"] = f"Bearer {self._access_token}"
 
-        if not params:
-            params = {}
-        params["source"] = self._source
-
         if running_client := self._httpx_client and not self._httpx_client.is_closed:
             client = self._httpx_client
         else:
             client = AsyncClient()
 
         request = Request(
             method, url, headers=headers, cookies=cookies, params=params, json=json
@@ -146,26 +142,29 @@
         cookies: Cookies | None = None,
         params: dict[str, str] | None = None,
         json: dict[str, str] | None = None,
     ) -> ValidatedResponseT:
         """Make a request to the Liminal API server and validate the response.
 
         Args:
+        ----
             method: The HTTP method to use.
             endpoint: The endpoint to request.
             expected_response_type: The expected type of the response.
             headers: The headers to use.
             cookies: The cookies to use.
             params: The query parameters to use.
             json: The JSON body to use.
 
         Returns:
+        -------
             A validated response object.
 
         Raises:
+        ------
             RequestError: If the response could not be validated.
 
         """
         response = await self._request(
             method, endpoint, headers=headers, cookies=cookies, params=params, json=json
         )
 
@@ -180,14 +179,15 @@
             msg = f"Could not validate response: {err}"
             raise RequestError(msg) from err
 
     def _save_tokens_from_auth_response(self, auth_response: Response) -> None:
         """Save tokens from an auth response.
 
         Args:
+        ----
             auth_response: The response from an auth request.
 
         """
         LOGGER.debug("Saving tokens from auth response")
         self._access_token = auth_response.cookies["accessToken"]
         self._access_token_expires_at = datetime.fromtimestamp(
             int(auth_response.cookies["accessTokenExpiresAt"]) / 1000, tz=UTC
@@ -202,17 +202,19 @@
     ) -> Callable[[], None]:
         """Add a callback to be called when a new refresh token is generated.
 
         The purpose of this is to allow the user to save the refresh token to a
         persistent store using their own callback method.
 
         Args:
+        ----
             callback: The callback to add.
 
         Returns:
+        -------
             A method to cancel and remove the callback.
 
         """
         self._refresh_token_callbacks.append(callback)
 
         def cancel() -> None:
             """Cancel and remove the callback."""
@@ -232,18 +234,20 @@
 
     async def authenticate_from_refresh_token(
         self, *, refresh_token: str | None = None
     ) -> None:
         """Authenticate with the Liminal API server (using a refresh token).
 
         Args:
+        ----
             refresh_token: The refresh token to use. If not provided, the refresh token
                 that was used to authenticate the user initially will be used.
 
         Raises:
+        ------
             AuthError: If no refresh token is provided and the user has not been
                 authenticated yet.
 
         """
         if not refresh_token:
             refresh_token = self._refresh_token
```

### Comparing `liminal_sdk_python-2024.3.5/liminal/endpoints/llm/__init__.py` & `liminal_sdk_python-2024.4.0/liminal/endpoints/llm/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,43 +15,48 @@
 
     def __init__(
         self, request_and_validate: Callable[..., Awaitable[ValidatedResponseT]]
     ) -> None:
         """Initialize.
 
         Args:
+        ----
             request_and_validate: The function to request and validate a response.
 
         """
         self._request_and_validate = request_and_validate
 
     async def get_available_model_instances(self) -> list[ModelInstance]:
         """Get available model instances.
 
-        Returns:
+        Returns
+        -------
             A list of available model instances.
 
         """
         return cast(
             list[ModelInstance],
             await self._request_and_validate(
                 "GET", "/api/v1/model-instances", list[ModelInstance]
             ),
         )
 
     async def get_model_instance(self, model_instance_name: str) -> ModelInstance:
         """Get a model instance by name.
 
         Args:
+        ----
             model_instance_name: The name of the model instance to retrieve.
 
         Returns:
+        -------
             The model instance.
 
         Raises:
+        ------
             ModelInstanceUnknownError: When the model instance is unknown.
 
         """
         model_instances = await self.get_available_model_instances()
 
         try:
             model_instance = next(
```

### Comparing `liminal_sdk_python-2024.3.5/liminal/endpoints/llm/models.py` & `liminal_sdk_python-2024.4.0/liminal/endpoints/llm/models.py`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.3.5/liminal/endpoints/prompt/models.py` & `liminal_sdk_python-2024.4.0/liminal/endpoints/prompt/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
     end: int
     entity_type: str
     start: int
 
 
 @dataclass(frozen=True, kw_only=True)
-class ProcessResponse(BaseResponseModel):
+class SubmitResponse(BaseResponseModel):
     """Define the response schema for a process request."""
 
     thread_id: int = field(metadata=field_options(alias="threadId"))
     chat_id: int = field(metadata=field_options(alias="chatId"))
     input_text: str = field(metadata=field_options(alias="inputText"))
     deidentified_input_text_data: CleanseResponse = field(
         metadata=field_options(alias="deidentifiedInputTextData")
```

### Comparing `liminal_sdk_python-2024.3.5/liminal/endpoints/thread/__init__.py` & `liminal_sdk_python-2024.4.0/liminal/endpoints/thread/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,104 +3,94 @@
 from __future__ import annotations
 
 from collections.abc import Awaitable, Callable
 from typing import cast
 
 from httpx import Response
 
-from liminal.endpoints.thread.models import DeidentifiedToken, Thread
+from liminal.const import SOURCE
+from liminal.endpoints.thread.models import Thread
 from liminal.helpers.typing import ValidatedResponseT
 
 
 class ThreadEndpoint:
     """Define the threads endpoint."""
 
     def __init__(
         self,
         request: Callable[..., Awaitable[Response]],
         request_and_validate: Callable[..., Awaitable[ValidatedResponseT]],
     ) -> None:
         """Initialize.
 
         Args:
+        ----
             request: The request function.
             request_and_validate: The request and validate function.
 
         """
         self._request = request
         self._request_and_validate = request_and_validate
 
     async def create(self, model_instance_id: int, name: str) -> Thread:
         """Create a thread.
 
         Args:
+        ----
             model_instance_id: The model instance id.
             name: The name of the thread.
 
         Returns:
+        -------
             A Thread object representing the creatd thread.
 
         """
         return cast(
             Thread,
             await self._request_and_validate(
                 "POST",
                 "/api/v1/threads",
                 Thread,
                 json={
                     "name": name,
                     "modelInstanceId": model_instance_id,
+                    "source": SOURCE,
                 },
             ),
         )
 
     async def get_available(self) -> list[Thread]:
         """Get available threads.
 
-        Returns:
+        Returns
+        -------
             A list of Thread objects.
 
         """
         return cast(
             list[Thread],
-            await self._request_and_validate("GET", "/api/v1/threads", list[Thread]),
+            await self._request_and_validate(
+                "GET",
+                "/api/v1/threads",
+                list[Thread],
+                params={"source": SOURCE},
+            ),
         )
 
     async def get_by_id(self, thread_id: int) -> Thread:
         """Get a thread by ID.
 
         Args:
+        ----
             thread_id: The ID of the thread.
 
         Returns:
+        -------
             A Thread object representing the thread.
 
         """
         return cast(
             Thread,
             await self._request_and_validate(
                 "GET", f"/api/v1/threads/{thread_id}", Thread
             ),
         )
-
-    async def get_deidentified_context_history(
-        self, thread_id: int
-    ) -> list[DeidentifiedToken]:
-        """Get the deidentified context history for a thread.
-
-        Args:
-            thread_id: The ID of the thread.
-
-        Returns:
-            A list of DeidentifiedToken objects representing the deidentified context
-                history.
-
-        """
-        return cast(
-            list[DeidentifiedToken],
-            await self._request_and_validate(
-                "POST",
-                "/api/v1/sdk/get_context_history",
-                list[DeidentifiedToken],
-                json={"threadId": thread_id},
-            ),
-        )
```

### Comparing `liminal_sdk_python-2024.3.5/liminal/endpoints/thread/models.py` & `liminal_sdk_python-2024.4.0/liminal/endpoints/thread/models.py`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.3.5/PKG-INFO` & `liminal_sdk_python-2024.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liminal-sdk-python
-Version: 2024.3.5
+Version: 2024.4.0
 Summary: The Liminal SDK for Python
 Home-page: https://github.com/liminal-ai-security/liminal-sdk-python
 License: Apache-2.0
 Author: Aaron Bach
 Author-email: ab@liminal.ai
 Requires-Python: >=3.11.8,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: httpx (==0.27.0)
 Requires-Dist: mashumaro (==3.12)
-Requires-Dist: msal (==1.27.0)
+Requires-Dist: msal (==1.28.0)
 Project-URL: Bug Tracker, https://github.com/liminal-ai-security/liminal-sdk-python/issues
 Project-URL: Changelog, https://github.com/liminal-ai-security/liminal-sdk-python/releases
 Project-URL: Repository, https://github.com/liminal-ai-security/liminal-sdk-python
 Description-Content-Type: text/markdown
 
 # Liminal Python SDK
 
@@ -279,18 +279,14 @@
     # Some operations require a model instance:
     model_instance = await liminal.llm.get_model_instance("My Model")
 
     # Create a new thread:
     thread = await liminal.thread.create(model_instance.id, "New Thread")
     # >>> Thread(...)
 
-    # Get the "de-identified" (containing sensitive data) context history for a thread:
-    thread = await liminal.thread.get_deidentified_context_history(model_instance.id)
-    # >>> [DeidentifiedToken(...), DeidentifiedToken(...), DeidentifiedToken(...)]
-
 
 asyncio.run(main())
 ```
 
 ## Submitting Prompts
 
 Submitting prompts is easy:
@@ -301,40 +297,51 @@
 from liminal import Client
 from liminal.auth.microsoft.device_code_flow import DeviceCodeFlowProvider
 
 
 async def main() -> None:
     # Assuming you have an authenticated `liminal` object:
 
-    # Prompt operations require a thread:
+    # Prompt operations require a model instance:
+    model_instance = await liminal.llm.get_model_instance(model_instance_name)
+
+    # Prompt operations optionally take an existing thread:
     thread = await liminal.thread.get_by_id(123)
     # >>> Thread(...)
 
     # Analayze a prompt for sensitive info:
-    findings = await liminal.prompt.analyze(thread.id)
+    findings = await liminal.prompt.analyze(
+        model_instance.id, "Here is a sensitive prompt"
+    )
     # >>> AnalyzeResponse(...)
 
     # Cleanse input text by applying the policies defined in the Liminal admin
     # dashboard. You can optionally provide existing analysis finidings; if not
     # provided, analyze is # called automatically):
     cleansed = await liminal.prompt.cleanse(
-        thread.id, "Here is a sensitive prompt", findings=findings
+        model_instance.id,
+        "Here is a sensitive prompt",
+        findings=findings,
+        thread_id=thread.id,
     )
     # >>> CleanseResponse(...)
 
     # Submit a prompt to an LLM, cleansing it in the process (once again, providing optional
     # findings):
     response = await liminal.prompt.submit(
-        thread.id, "Here is a sensitive prompt", findings=findings
+        model_instance.id,
+        "Here is a sensitive prompt",
+        findings=findings,
+        thread_id=thread.id,
     )
-    # >>> ProcessResponse(...)
+    # >>> SubmitResponse(...)
 
     # Rehydrate a response with sensitive data:
     hydrated = await liminal.prompt.hydrate(
-        thread.id, "Here is a response to rehdyrate"
+        model_instance.id, "Here is a response to rehdyrate", thread_id=thread.id
     )
     # >>> HydrateResponse(...)
 
 
 asyncio.run(main())
 ```
```

